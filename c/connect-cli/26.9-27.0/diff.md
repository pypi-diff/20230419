# Comparing `tmp/connect_cli-26.9.tar.gz` & `tmp/connect_cli-27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connect_cli-26.9.tar", max compression
+gzip compressed data, was "connect_cli-27.0.tar", max compression
```

## Comparing `connect_cli-26.9.tar` & `connect_cli-27.0.tar`

### file list

```diff
@@ -1,275 +1,287 @@
--rw-r--r--   0        0        0    11357 2022-11-10 08:18:26.682743 connect_cli-26.9/LICENSE
--rw-r--r--   0        0        0     3070 2022-11-10 08:18:26.682743 connect_cli-26.9/README.md
--rw-r--r--   0        0        0     1821 2022-11-10 08:20:54.777071 connect_cli-26.9/connect/.data/connect_reports/.github/workflows/build.yml
--rw-r--r--   0        0        0      166 2022-11-10 08:20:54.777071 connect_cli-26.9/connect/.data/connect_reports/.gitignore
--rw-r--r--   0        0        0    10756 2022-11-10 08:20:54.777071 connect_cli-26.9/connect/.data/connect_reports/LICENSE
--rw-r--r--   0        0        0      708 2022-11-10 08:20:54.777071 connect_cli-26.9/connect/.data/connect_reports/README.md
--rw-r--r--   0        0        0   122573 2022-11-10 08:20:54.777071 connect_cli-26.9/connect/.data/connect_reports/poetry.lock
--rw-r--r--   0        0        0     1221 2022-11-10 08:20:54.777071 connect_cli-26.9/connect/.data/connect_reports/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-10 08:20:54.777071 connect_cli-26.9/connect/.data/connect_reports/reports/__init__.py
--rw-r--r--   0        0        0      215 2022-11-10 08:20:54.777071 connect_cli-26.9/connect/.data/connect_reports/reports/billing_requests/Readme.md
--rw-r--r--   0        0        0        0 2022-11-10 08:20:54.777071 connect_cli-26.9/connect/.data/connect_reports/reports/billing_requests/__init__.py
--rw-r--r--   0        0        0     3762 2022-11-10 08:20:54.777071 connect_cli-26.9/connect/.data/connect_reports/reports/billing_requests/entrypoint.py
--rw-r--r--   0        0        0     9038 2022-11-10 08:20:54.777071 connect_cli-26.9/connect/.data/connect_reports/reports/billing_requests/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0      377 2022-11-10 08:20:54.777071 connect_cli-26.9/connect/.data/connect_reports/reports/billing_requests_line_item/Readme.md
--rw-r--r--   0        0        0        0 2022-11-10 08:20:54.777071 connect_cli-26.9/connect/.data/connect_reports/reports/billing_requests_line_item/__init__.py
--rw-r--r--   0        0        0     4313 2022-11-10 08:20:54.777071 connect_cli-26.9/connect/.data/connect_reports/reports/billing_requests_line_item/entrypoint.py
--rw-r--r--   0        0        0     9214 2022-11-10 08:20:54.777071 connect_cli-26.9/connect/.data/connect_reports/reports/billing_requests_line_item/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0      151 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/contract_list/Readme.md
--rw-r--r--   0        0        0        0 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/contract_list/__init__.py
--rw-r--r--   0        0        0     3114 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/contract_list/entrypoint.py
--rw-r--r--   0        0        0     8883 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/contract_list/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0      175 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/customers_list/Readme.md
--rw-r--r--   0        0        0        0 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/customers_list/__init__.py
--rw-r--r--   0        0        0     3595 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/customers_list/entrypoint.py
--rw-r--r--   0        0        0     8914 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/customers_list/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0      546 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/executive_fullfilment_requests/Readme.md
--rw-r--r--   0        0        0        0 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/executive_fullfilment_requests/__init__.py
--rw-r--r--   0        0        0     6342 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/executive_fullfilment_requests/constants.py
--rw-r--r--   0        0        0    17376 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/executive_fullfilment_requests/entrypoint.py
--rw-r--r--   0        0        0     5254 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/executive_fullfilment_requests/templates/pdf/img/ClouBlue-Logo.png
--rw-r--r--   0        0        0     3180 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/executive_fullfilment_requests/templates/pdf/template.css
--rw-r--r--   0        0        0     1280 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/executive_fullfilment_requests/templates/pdf/template.html.j2
--rw-r--r--   0        0        0      240 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/fulfillment_requests/Readme.md
--rw-r--r--   0        0        0        0 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/fulfillment_requests/__init__.py
--rw-r--r--   0        0        0     4536 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/fulfillment_requests/entrypoint.py
--rw-r--r--   0        0        0     9160 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/fulfillment_requests/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0      301 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/fulfillment_requests_failed/Readme.md
--rw-r--r--   0        0        0        0 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/fulfillment_requests_failed/__init__.py
--rw-r--r--   0        0        0     4016 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/fulfillment_requests_failed/entrypoint.py
--rw-r--r--   0        0        0     9050 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/fulfillment_requests_failed/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0      328 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/fulfillment_requests_line_item/Readme.md
--rw-r--r--   0        0        0        0 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/fulfillment_requests_line_item/__init__.py
--rw-r--r--   0        0        0     4809 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/fulfillment_requests_line_item/entrypoint.py
--rw-r--r--   0        0        0     9143 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/fulfillment_requests_line_item/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0      186 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/listing_list/Readme.md
--rw-r--r--   0        0        0        0 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/listing_list/__init__.py
--rw-r--r--   0        0        0     2632 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/listing_list/entrypoint.py
--rw-r--r--   0        0        0     8703 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/listing_list/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0      194 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/listing_requests/Readme.md
--rw-r--r--   0        0        0        0 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/listing_requests/__init__.py
--rw-r--r--   0        0        0     2870 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/listing_requests/entrypoint.py
--rw-r--r--   0        0        0     8746 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/listing_requests/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0      117 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/Readme.md
--rw-r--r--   0        0        0        0 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/__init__.py
--rw-r--r--   0        0        0     2591 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/entrypoint.py
--rwxr-xr-x   0        0        0     7209 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-connect-alone.png
--rw-r--r--   0        0        0    33448 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-logo.png
--rw-r--r--   0        0        0    11287 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-small-color-disabled.png
--rw-r--r--   0        0        0     9404 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-small-color-enabled.png
--rw-r--r--   0        0        0    91722 2022-11-10 08:20:54.781072 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/connect-logo.png
--rw-r--r--   0        0        0   465078 2022-11-10 08:20:54.785071 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cover-bg.png
--rw-r--r--   0        0        0    10941 2022-11-10 08:20:54.785071 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/imc-small-color.png
--rw-r--r--   0        0        0    16685 2022-11-10 08:20:54.785071 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/ClouBlue-Logo-Black.png
--rw-r--r--   0        0        0     3555 2022-11-10 08:20:54.785071 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/ClouBlue-Logo-White.png
--rw-r--r--   0        0        0     5254 2022-11-10 08:20:54.785071 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/ClouBlue-Logo.png
--rw-r--r--   0        0        0     8250 2022-11-10 08:20:54.785071 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/accordo.png
--rw-r--r--   0        0        0     1311 2022-11-10 08:20:54.785071 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/acronis-blue.png
--rw-r--r--   0        0        0     1968 2022-11-10 08:20:54.785071 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/acronis-white.png
--rw-r--r--   0        0        0   124929 2022-11-10 08:20:54.785071 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/adobe.jpeg
--rw-r--r--   0        0        0    10421 2022-11-10 08:20:54.785071 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/airtame.png
--rw-r--r--   0        0        0      876 2022-11-10 08:20:54.785071 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/allyhub.png
--rw-r--r--   0        0        0     4615 2022-11-10 08:20:54.785071 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/alsid.png
--rw-r--r--   0        0        0    12369 2022-11-10 08:20:54.785071 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/anchor.png
--rw-r--r--   0        0        0     5200 2022-11-10 08:20:54.785071 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/australia.png
--rw-r--r--   0        0        0     3371 2022-11-10 08:20:54.785071 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/austria.png
--rw-r--r--   0        0        0    60306 2022-11-10 08:20:54.785071 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/aws.png
--rw-r--r--   0        0        0     3030 2022-11-10 08:20:54.785071 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/belgium.png
--rw-r--r--   0        0        0     5606 2022-11-10 08:20:54.785071 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/brazil.png
--rw-r--r--   0        0        0     3693 2022-11-10 08:20:54.785071 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/canada.png
--rw-r--r--   0        0        0     3870 2022-11-10 08:20:54.785071 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/chile.png
--rw-r--r--   0        0        0     3086 2022-11-10 08:20:54.785071 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/colombia.png
--rw-r--r--   0        0        0     3670 2022-11-10 08:20:54.785071 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/france.png
--rw-r--r--   0        0        0     3212 2022-11-10 08:20:54.785071 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/germany.png
--rw-r--r--   0        0        0     4521 2022-11-10 08:20:54.785071 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/hong-kong.png
--rw-r--r--   0        0        0    12000 2022-11-10 08:20:54.785071 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/icon.png
--rw-r--r--   0        0        0     4491 2022-11-10 08:20:54.785071 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/india.png
--rw-r--r--   0        0        0     3622 2022-11-10 08:20:54.785071 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/italy.png
--rw-r--r--   0        0        0     5096 2022-11-10 08:20:54.785071 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/malaysia.png
--rw-r--r--   0        0        0     3897 2022-11-10 08:20:54.785071 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/mexico.png
--rw-r--r--   0        0        0     3633 2022-11-10 08:20:54.785071 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/netherlands.png
--rw-r--r--   0        0        0     5173 2022-11-10 08:20:54.785071 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/new-zealand.png
--rw-r--r--   0        0        0     4163 2022-11-10 08:20:54.785071 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/singapore.png
--rw-r--r--   0        0        0     4670 2022-11-10 08:20:54.785071 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/spain.png
--rw-r--r--   0        0        0     4802 2022-11-10 08:20:54.785071 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/sweden.png
--rw-r--r--   0        0        0     3622 2022-11-10 08:20:54.785071 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/switzerland.png
--rw-r--r--   0        0        0     4073 2022-11-10 08:20:54.789071 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/turkey.png
--rw-r--r--   0        0        0     3350 2022-11-10 08:20:54.789071 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/uae.png
--rw-r--r--   0        0        0     5583 2022-11-10 08:20:54.789071 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/uk.png
--rw-r--r--   0        0        0     4892 2022-11-10 08:20:54.789071 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/usa.png
--rw-r--r--   0        0        0     4063 2022-11-10 08:20:54.789071 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/template.css
--rw-r--r--   0        0        0     1736 2022-11-10 08:20:54.789071 connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/template.html.j2
--rw-r--r--   0        0        0      592 2022-11-10 08:20:54.789071 connect_cli-26.9/connect/.data/connect_reports/reports/sla/Readme.md
--rw-r--r--   0        0        0        0 2022-11-10 08:20:54.789071 connect_cli-26.9/connect/.data/connect_reports/reports/sla/__init__.py
--rw-r--r--   0        0        0     4077 2022-11-10 08:20:54.789071 connect_cli-26.9/connect/.data/connect_reports/reports/sla/entrypoint.py
--rw-r--r--   0        0        0     9679 2022-11-10 08:20:54.789071 connect_cli-26.9/connect/.data/connect_reports/reports/sla/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0      260 2022-11-10 08:20:54.789071 connect_cli-26.9/connect/.data/connect_reports/reports/subscription_list/Readme.md
--rw-r--r--   0        0        0        0 2022-11-10 08:20:54.789071 connect_cli-26.9/connect/.data/connect_reports/reports/subscription_list/__init__.py
--rw-r--r--   0        0        0     6276 2022-11-10 08:20:54.789071 connect_cli-26.9/connect/.data/connect_reports/reports/subscription_list/entrypoint.py
--rw-r--r--   0        0        0     9302 2022-11-10 08:20:54.789071 connect_cli-26.9/connect/.data/connect_reports/reports/subscription_list/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0      203 2022-11-10 08:20:54.789071 connect_cli-26.9/connect/.data/connect_reports/reports/tier_configuration_list/Readme.md
--rw-r--r--   0        0        0        0 2022-11-10 08:20:54.789071 connect_cli-26.9/connect/.data/connect_reports/reports/tier_configuration_list/__init__.py
--rw-r--r--   0        0        0     4282 2022-11-10 08:20:54.789071 connect_cli-26.9/connect/.data/connect_reports/reports/tier_configuration_list/entrypoint.py
--rw-r--r--   0        0        0     8925 2022-11-10 08:20:54.789071 connect_cli-26.9/connect/.data/connect_reports/reports/tier_configuration_list/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0      228 2022-11-10 08:20:54.789071 connect_cli-26.9/connect/.data/connect_reports/reports/tier_configuration_requests/Readme.md
--rw-r--r--   0        0        0        0 2022-11-10 08:20:54.789071 connect_cli-26.9/connect/.data/connect_reports/reports/tier_configuration_requests/__init__.py
--rw-r--r--   0        0        0     5119 2022-11-10 08:20:54.789071 connect_cli-26.9/connect/.data/connect_reports/reports/tier_configuration_requests/entrypoint.py
--rw-r--r--   0        0        0     9070 2022-11-10 08:20:54.789071 connect_cli-26.9/connect/.data/connect_reports/reports/tier_configuration_requests/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0      431 2022-11-10 08:20:54.789071 connect_cli-26.9/connect/.data/connect_reports/reports/usage_in_subscription/Readme.md
--rw-r--r--   0        0        0        0 2022-11-10 08:20:54.789071 connect_cli-26.9/connect/.data/connect_reports/reports/usage_in_subscription/__init__.py
--rw-r--r--   0        0        0     4106 2022-11-10 08:20:54.789071 connect_cli-26.9/connect/.data/connect_reports/reports/usage_in_subscription/entrypoint.py
--rw-r--r--   0        0        0     9137 2022-11-10 08:20:54.789071 connect_cli-26.9/connect/.data/connect_reports/reports/usage_in_subscription/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0     1318 2022-11-10 08:20:54.789071 connect_cli-26.9/connect/.data/connect_reports/reports/utils.py
--rw-r--r--   0        0        0    36124 2022-11-10 08:20:54.777071 connect_cli-26.9/connect/.data/connect_reports/reports.json
--rw-r--r--   0        0        0      245 2022-11-10 08:20:54.789071 connect_cli-26.9/connect/.data/connect_reports/sonar-project.properties
--rw-r--r--   0        0        0      321 2022-11-10 08:20:54.789071 connect_cli-26.9/connect/.data/connect_reports/tox.ini
--rw-r--r--   0        0        0      352 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/__init__.py
--rw-r--r--   0        0        0     1479 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/ccli.py
--rw-r--r--   0        0        0       54 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/core/__init__.py
--rw-r--r--   0        0        0        0 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/core/account/__init__.py
--rw-r--r--   0        0        0     2450 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/core/account/commands.py
--rw-r--r--   0        0        0     1233 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/core/account/helpers.py
--rw-r--r--   0        0        0     2781 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/core/base.py
--rw-r--r--   0        0        0     4049 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/core/config.py
--rw-r--r--   0        0        0      690 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/core/constants.py
--rw-r--r--   0        0        0     1424 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/core/http.py
--rw-r--r--   0        0        0      838 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/core/plugins.py
--rw-r--r--   0        0        0     6790 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/core/terminal.py
--rw-r--r--   0        0        0     3167 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/core/utils.py
--rw-r--r--   0        0        0        0 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/__init__.py
--rw-r--r--   0        0        0        0 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/customer/__init__.py
--rw-r--r--   0        0        0     2138 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/customer/commands.py
--rw-r--r--   0        0        0      738 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/customer/constants.py
--rw-r--r--   0        0        0     5923 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/customer/export.py
--rw-r--r--   0        0        0    12430 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/customer/sync.py
--rw-r--r--   0        0        0        0 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/locale/__init__.py
--rw-r--r--   0        0        0     1363 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/locale/commands.py
--rw-r--r--   0        0        0      306 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/play/__init__.py
--rw-r--r--   0        0        0     2486 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/play/commands.py
--rw-r--r--   0        0        0     2395 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/play/context.py
--rw-r--r--   0        0        0      428 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/play/save.py
--rw-r--r--   0        0        0     1500 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/play/script.py
--rw-r--r--   0        0        0        0 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/product/__init__.py
--rw-r--r--   0        0        0     1674 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/product/api.py
--rw-r--r--   0        0        0     8631 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/product/clone.py
--rw-r--r--   0        0        0     9677 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/product/commands.py
--rw-r--r--   0        0        0     1012 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/product/constants.py
--rw-r--r--   0        0        0    33269 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/product/export.py
--rw-r--r--   0        0        0      828 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/product/sync/__init__.py
--rw-r--r--   0        0        0     5919 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/product/sync/actions.py
--rw-r--r--   0        0        0    10140 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/product/sync/capabilities.py
--rw-r--r--   0        0        0     3881 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/product/sync/configuration_values.py
--rw-r--r--   0        0        0     5129 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/product/sync/general.py
--rw-r--r--   0        0        0    11854 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/product/sync/items.py
--rw-r--r--   0        0        0     5739 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/product/sync/media.py
--rw-r--r--   0        0        0     9351 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/product/sync/params.py
--rw-r--r--   0        0        0     3598 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/product/sync/static_resources.py
--rw-r--r--   0        0        0     5455 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/product/sync/templates.py
--rw-r--r--   0        0        0      961 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/product/utils.py
--rw-r--r--   0        0        0        0 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/project/__init__.py
--rw-r--r--   0        0        0     3740 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/project/commands.py
--rw-r--r--   0        0        0        0 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/project/extension/__init__.py
--rw-r--r--   0        0        0     2630 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/project/extension/constants.py
--rw-r--r--   0        0        0     6277 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/project/extension/helpers.py
--rw-r--r--   0        0        0      103 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/__init__.py.j2
--rw-r--r--   0        0        0      852 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/anvil.py.j2
--rw-r--r--   0        0        0     3093 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/events.py.j2
--rw-r--r--   0        0        0      464 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/extension.json.j2
--rw-r--r--   0        0        0      341 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/schemas.py.j2
--rw-r--r--   0        0        0        0 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/static/.gitkeep.j2
--rw-r--r--   0        0        0     4092 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/webapp.py.j2
--rw-r--r--   0        0        0      702 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.${project_slug}_dev.env.j2
--rw-r--r--   0        0        0     1083 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.eslintrc.yaml.j2
--rw-r--r--   0        0        0      231 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.flake8.j2
--rw-r--r--   0        0        0     1309 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.github/workflows/test.yml.j2
--rw-r--r--   0        0        0       96 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.gitignore.j2
--rw-r--r--   0        0        0       63 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/CHANGELOG.md.j2
--rw-r--r--   0        0        0      301 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/Dockerfile.j2
--rw-r--r--   0        0        0     1659 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/HOWTO.md.j2
--rw-r--r--   0        0        0    14063 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/LICENSE.j2
--rw-r--r--   0        0        0      195 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/README.md.j2
--rw-r--r--   0        0        0      111 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/__mocks__/fileMock.js.j2
--rw-r--r--   0        0        0       97 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/__mocks__/styleMock.js.j2
--rw-r--r--   0        0        0       39 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/babel.config.json.j2
--rw-r--r--   0        0        0      756 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/docker-compose.yml.j2
--rw-r--r--   0        0        0      944 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/jest.config.js.j2
--rw-r--r--   0        0        0     1208 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/package.json.j2
--rw-r--r--   0        0        0       29 2022-11-10 08:18:26.686743 connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/poetry.toml.j2
--rw-r--r--   0        0        0     1969 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/pyproject.toml.j2
--rw-r--r--   0        0        0      103 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/__init__.py.j2
--rw-r--r--   0        0        0      559 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/conftest.py.j2
--rw-r--r--   0        0        0      553 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_anvil.py.j2
--rw-r--r--   0        0        0     2608 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_events.py.j2
--rw-r--r--   0        0        0     5182 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_webapp.py.j2
--rw-r--r--   0        0        0      729 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/pages/index.html.j2
--rw-r--r--   0        0        0      928 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/pages/settings.html.j2
--rw-r--r--   0        0        0     2550 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/components.js.j2
--rw-r--r--   0        0        0      323 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/pages/index.js.j2
--rw-r--r--   0        0        0      320 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/pages/settings.js.j2
--rw-r--r--   0        0        0     2119 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/pages.js.j2
--rw-r--r--   0        0        0     1222 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/utils.js.j2
--rw-r--r--   0        0        0     6381 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/styles/index.css.j2
--rw-r--r--   0        0        0     6319 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/tests/components.spec.js.j2
--rw-r--r--   0        0        0     9181 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/tests/pages.spec.js.j2
--rw-r--r--   0        0        0     4352 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/tests/utils.spec.js.j2
--rw-r--r--   0        0        0     1937 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/webpack.config.js.j2
--rw-r--r--   0        0        0     3349 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/extension/utils.py
--rw-r--r--   0        0        0    12031 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/extension/wizard.py
--rw-r--r--   0        0        0     5726 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/renderer.py
--rw-r--r--   0        0        0        0 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/report/__init__.py
--rw-r--r--   0        0        0     8611 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/report/helpers.py
--rw-r--r--   0        0        0       73 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/report/templates/add/${initial_report_slug}/README.md.j2
--rw-r--r--   0        0        0        0 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/report/templates/add/${initial_report_slug}/__init__.py.j2
--rw-r--r--   0        0        0     1507 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/report/templates/add/${initial_report_slug}/entrypoint.py.j2
--rw-r--r--   0        0        0        0 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/report/templates/add/${initial_report_slug}/templates/pdf/template.css.j2
--rw-r--r--   0        0        0      499 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/report/templates/add/${initial_report_slug}/templates/pdf/template.html.j2.j2
--rw-r--r--   0        0        0      150 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/report/templates/add/${initial_report_slug}/templates/xml/template.xml.j2.j2
--rw-r--r--   0        0        0       69 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/README.md.j2
--rw-r--r--   0        0        0        0 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/__init__.py.j2
--rw-r--r--   0        0        0     1507 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/entrypoint.py.j2
--rw-r--r--   0        0        0        0 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/templates/pdf/template.css.j2
--rw-r--r--   0        0        0      518 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/templates/pdf/template.html.j2.j2
--rw-r--r--   0        0        0      150 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/templates/xml/template.xml.j2.j2
--rw-r--r--   0        0        0      271 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/.flake8.j2
--rw-r--r--   0        0        0      803 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/.github/workflows/build.yml.j2
--rw-r--r--   0        0        0       37 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/.gitignore.j2
--rw-r--r--   0        0        0      458 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/HOWTO.md.j2
--rw-r--r--   0        0        0    14063 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/LICENSE.j2
--rw-r--r--   0        0        0      138 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/README.md.j2
--rw-r--r--   0        0        0       29 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/poetry.toml.j2
--rw-r--r--   0        0        0     1352 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/pyproject.toml.j2
--rw-r--r--   0        0        0     2589 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/reports.json.j2
--rw-r--r--   0        0        0      103 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/tests/__init__.py.j2
--rw-r--r--   0        0        0     6397 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/tests/conftest.py.j2
--rw-r--r--   0        0        0     2534 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/tests/test_${project_slug}.py.j2
--rw-r--r--   0        0        0     5891 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/report/validations.py
--rw-r--r--   0        0        0     8602 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/report/wizard.py
--rw-r--r--   0        0        0     1403 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/utils.py
--rw-r--r--   0        0        0     2354 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/project/validators.py
--rw-r--r--   0        0        0        0 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/report/__init__.py
--rw-r--r--   0        0        0     2422 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/report/commands.py
--rw-r--r--   0        0        0       86 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/report/constants.py
--rw-r--r--   0        0        0     6210 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/report/helpers.py
--rw-r--r--   0        0        0     2812 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/report/utils.py
--rw-r--r--   0        0        0     8418 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/report/wizard.py
--rw-r--r--   0        0        0        0 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/shared/__init__.py
--rw-r--r--   0        0        0     2442 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/shared/base.py
--rw-r--r--   0        0        0     1973 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/shared/constants.py
--rw-r--r--   0        0        0       46 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/shared/exceptions.py
--rw-r--r--   0        0        0     2303 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/shared/export.py
--rw-r--r--   0        0        0     6248 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/shared/sync_stats.py
--rw-r--r--   0        0        0     5669 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/shared/translation_attr_sync.py
--rw-r--r--   0        0        0     6388 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/shared/translation_sync.py
--rw-r--r--   0        0        0     1996 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/shared/translations_synchronizers.py
--rw-r--r--   0        0        0     6794 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/shared/utils.py
--rw-r--r--   0        0        0        0 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/translation/__init__.py
--rw-r--r--   0        0        0      720 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/translation/activate.py
--rw-r--r--   0        0        0     6869 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/translation/commands.py
--rw-r--r--   0        0        0     1049 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/translation/constants.py
--rw-r--r--   0        0        0     1229 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/translation/export.py
--rw-r--r--   0        0        0      967 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/translation/primarize.py
--rw-r--r--   0        0        0     8879 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/translation/translation_sync.py
--rw-r--r--   0        0        0      832 2022-11-10 08:18:26.690743 connect_cli-26.9/connect/cli/plugins/translation/utils.py
--rw-r--r--   0        0        0     3370 2022-11-10 08:20:55.473082 connect_cli-26.9/pyproject.toml
--rw-r--r--   0        0        0    10454 1970-01-01 00:00:00.000000 connect_cli-26.9/setup.py
--rw-r--r--   0        0        0     4975 1970-01-01 00:00:00.000000 connect_cli-26.9/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-19 06:48:02.393923 connect_cli-27.0/LICENSE
+-rw-r--r--   0        0        0     3280 2023-04-19 06:48:02.393923 connect_cli-27.0/README.md
+-rw-r--r--   0        0        0     1823 2023-04-19 06:50:55.191892 connect_cli-27.0/connect/.data/connect_reports/.github/workflows/build.yml
+-rw-r--r--   0        0        0      166 2023-04-19 06:50:55.191892 connect_cli-27.0/connect/.data/connect_reports/.gitignore
+-rw-r--r--   0        0        0    10756 2023-04-19 06:50:55.191892 connect_cli-27.0/connect/.data/connect_reports/LICENSE
+-rw-r--r--   0        0        0      708 2023-04-19 06:50:55.191892 connect_cli-27.0/connect/.data/connect_reports/README.md
+-rw-r--r--   0        0        0   122573 2023-04-19 06:50:55.191892 connect_cli-27.0/connect/.data/connect_reports/poetry.lock
+-rw-r--r--   0        0        0     1221 2023-04-19 06:50:55.191892 connect_cli-27.0/connect/.data/connect_reports/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-19 06:50:55.191892 connect_cli-27.0/connect/.data/connect_reports/reports/__init__.py
+-rw-r--r--   0        0        0      215 2023-04-19 06:50:55.191892 connect_cli-27.0/connect/.data/connect_reports/reports/billing_requests/Readme.md
+-rw-r--r--   0        0        0        0 2023-04-19 06:50:55.191892 connect_cli-27.0/connect/.data/connect_reports/reports/billing_requests/__init__.py
+-rw-r--r--   0        0        0     3762 2023-04-19 06:50:55.191892 connect_cli-27.0/connect/.data/connect_reports/reports/billing_requests/entrypoint.py
+-rw-r--r--   0        0        0     9038 2023-04-19 06:50:55.191892 connect_cli-27.0/connect/.data/connect_reports/reports/billing_requests/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0      377 2023-04-19 06:50:55.191892 connect_cli-27.0/connect/.data/connect_reports/reports/billing_requests_line_item/Readme.md
+-rw-r--r--   0        0        0        0 2023-04-19 06:50:55.191892 connect_cli-27.0/connect/.data/connect_reports/reports/billing_requests_line_item/__init__.py
+-rw-r--r--   0        0        0     4313 2023-04-19 06:50:55.191892 connect_cli-27.0/connect/.data/connect_reports/reports/billing_requests_line_item/entrypoint.py
+-rw-r--r--   0        0        0     9214 2023-04-19 06:50:55.191892 connect_cli-27.0/connect/.data/connect_reports/reports/billing_requests_line_item/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0      151 2023-04-19 06:50:55.191892 connect_cli-27.0/connect/.data/connect_reports/reports/contract_list/Readme.md
+-rw-r--r--   0        0        0        0 2023-04-19 06:50:55.191892 connect_cli-27.0/connect/.data/connect_reports/reports/contract_list/__init__.py
+-rw-r--r--   0        0        0     3114 2023-04-19 06:50:55.191892 connect_cli-27.0/connect/.data/connect_reports/reports/contract_list/entrypoint.py
+-rw-r--r--   0        0        0     8883 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/contract_list/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0      175 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/customers_list/Readme.md
+-rw-r--r--   0        0        0        0 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/customers_list/__init__.py
+-rw-r--r--   0        0        0     3595 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/customers_list/entrypoint.py
+-rw-r--r--   0        0        0     8914 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/customers_list/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0      546 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/executive_fullfilment_requests/Readme.md
+-rw-r--r--   0        0        0        0 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/executive_fullfilment_requests/__init__.py
+-rw-r--r--   0        0        0     6376 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/executive_fullfilment_requests/constants.py
+-rw-r--r--   0        0        0    17465 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/executive_fullfilment_requests/entrypoint.py
+-rw-r--r--   0        0        0     5254 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/executive_fullfilment_requests/templates/pdf/img/ClouBlue-Logo.png
+-rw-r--r--   0        0        0     3180 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/executive_fullfilment_requests/templates/pdf/template.css
+-rw-r--r--   0        0        0     1280 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/executive_fullfilment_requests/templates/pdf/template.html.j2
+-rw-r--r--   0        0        0      240 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/fulfillment_requests/Readme.md
+-rw-r--r--   0        0        0        0 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/fulfillment_requests/__init__.py
+-rw-r--r--   0        0        0     4584 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/fulfillment_requests/entrypoint.py
+-rw-r--r--   0        0        0     9160 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/fulfillment_requests/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0      301 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/fulfillment_requests_failed/Readme.md
+-rw-r--r--   0        0        0        0 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/fulfillment_requests_failed/__init__.py
+-rw-r--r--   0        0        0     4064 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/fulfillment_requests_failed/entrypoint.py
+-rw-r--r--   0        0        0     9050 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/fulfillment_requests_failed/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0      328 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/fulfillment_requests_line_item/Readme.md
+-rw-r--r--   0        0        0        0 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/fulfillment_requests_line_item/__init__.py
+-rw-r--r--   0        0        0     4982 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/fulfillment_requests_line_item/entrypoint.py
+-rw-r--r--   0        0        0     9234 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/fulfillment_requests_line_item/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0      180 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/helpdesk/Readme.md
+-rw-r--r--   0        0        0        0 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/helpdesk/__init__.py
+-rw-r--r--   0        0        0     2635 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/helpdesk/entrypoint.py
+-rw-r--r--   0        0        0     8749 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/helpdesk/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0      186 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/listing_list/Readme.md
+-rw-r--r--   0        0        0        0 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/listing_list/__init__.py
+-rw-r--r--   0        0        0     2632 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/listing_list/entrypoint.py
+-rw-r--r--   0        0        0     8703 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/listing_list/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0      194 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/listing_requests/Readme.md
+-rw-r--r--   0        0        0        0 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/listing_requests/__init__.py
+-rw-r--r--   0        0        0     2870 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/listing_requests/entrypoint.py
+-rw-r--r--   0        0        0     8746 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/listing_requests/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0      117 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/Readme.md
+-rw-r--r--   0        0        0        0 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/__init__.py
+-rw-r--r--   0        0        0     2582 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/entrypoint.py
+-rwxr-xr-x   0        0        0     7209 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-connect-alone.png
+-rw-r--r--   0        0        0    33448 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-logo.png
+-rw-r--r--   0        0        0    11287 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-small-color-disabled.png
+-rw-r--r--   0        0        0     9404 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-small-color-enabled.png
+-rw-r--r--   0        0        0    91722 2023-04-19 06:50:55.195892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/connect-logo.png
+-rw-r--r--   0        0        0   465078 2023-04-19 06:50:55.199892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cover-bg.png
+-rw-r--r--   0        0        0    10941 2023-04-19 06:50:55.199892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/imc-small-color.png
+-rw-r--r--   0        0        0    16685 2023-04-19 06:50:55.199892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/ClouBlue-Logo-Black.png
+-rw-r--r--   0        0        0     3555 2023-04-19 06:50:55.199892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/ClouBlue-Logo-White.png
+-rw-r--r--   0        0        0     5254 2023-04-19 06:50:55.199892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/ClouBlue-Logo.png
+-rw-r--r--   0        0        0     8250 2023-04-19 06:50:55.199892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/accordo.png
+-rw-r--r--   0        0        0     1311 2023-04-19 06:50:55.199892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/acronis-blue.png
+-rw-r--r--   0        0        0     1968 2023-04-19 06:50:55.199892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/acronis-white.png
+-rw-r--r--   0        0        0   124929 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/adobe.jpeg
+-rw-r--r--   0        0        0    10421 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/airtame.png
+-rw-r--r--   0        0        0      876 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/allyhub.png
+-rw-r--r--   0        0        0     4615 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/alsid.png
+-rw-r--r--   0        0        0    12369 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/anchor.png
+-rw-r--r--   0        0        0     5200 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/australia.png
+-rw-r--r--   0        0        0     3371 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/austria.png
+-rw-r--r--   0        0        0    60306 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/aws.png
+-rw-r--r--   0        0        0     3030 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/belgium.png
+-rw-r--r--   0        0        0     5606 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/brazil.png
+-rw-r--r--   0        0        0     3693 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/canada.png
+-rw-r--r--   0        0        0     3870 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/chile.png
+-rw-r--r--   0        0        0     3086 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/colombia.png
+-rw-r--r--   0        0        0     3670 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/france.png
+-rw-r--r--   0        0        0     3212 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/germany.png
+-rw-r--r--   0        0        0     4521 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/hong-kong.png
+-rw-r--r--   0        0        0    12000 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/icon.png
+-rw-r--r--   0        0        0     4491 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/india.png
+-rw-r--r--   0        0        0     3622 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/italy.png
+-rw-r--r--   0        0        0     5096 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/malaysia.png
+-rw-r--r--   0        0        0     3897 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/mexico.png
+-rw-r--r--   0        0        0     3633 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/netherlands.png
+-rw-r--r--   0        0        0     5173 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/new-zealand.png
+-rw-r--r--   0        0        0     4163 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/singapore.png
+-rw-r--r--   0        0        0     4670 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/spain.png
+-rw-r--r--   0        0        0     4802 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/sweden.png
+-rw-r--r--   0        0        0     3622 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/switzerland.png
+-rw-r--r--   0        0        0     4073 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/turkey.png
+-rw-r--r--   0        0        0     3350 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/uae.png
+-rw-r--r--   0        0        0     5583 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/uk.png
+-rw-r--r--   0        0        0     4892 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/usa.png
+-rw-r--r--   0        0        0     4063 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/template.css
+-rw-r--r--   0        0        0     1736 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/template.html.j2
+-rw-r--r--   0        0        0      592 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/sla/Readme.md
+-rw-r--r--   0        0        0        0 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/sla/__init__.py
+-rw-r--r--   0        0        0     4125 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/sla/entrypoint.py
+-rw-r--r--   0        0        0     9679 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/sla/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0      260 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/subscription_list/Readme.md
+-rw-r--r--   0        0        0        0 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/subscription_list/__init__.py
+-rw-r--r--   0        0        0     6276 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/subscription_list/entrypoint.py
+-rw-r--r--   0        0        0     9302 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/subscription_list/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0      203 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/tier_configuration_list/Readme.md
+-rw-r--r--   0        0        0        0 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/tier_configuration_list/__init__.py
+-rw-r--r--   0        0        0     4282 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/tier_configuration_list/entrypoint.py
+-rw-r--r--   0        0        0     8925 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/tier_configuration_list/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0      228 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/tier_configuration_requests/Readme.md
+-rw-r--r--   0        0        0        0 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/tier_configuration_requests/__init__.py
+-rw-r--r--   0        0        0     5119 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/tier_configuration_requests/entrypoint.py
+-rw-r--r--   0        0        0     9070 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/tier_configuration_requests/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0      431 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/usage_in_subscription/Readme.md
+-rw-r--r--   0        0        0        0 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/usage_in_subscription/__init__.py
+-rw-r--r--   0        0        0     4106 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/usage_in_subscription/entrypoint.py
+-rw-r--r--   0        0        0     9137 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/usage_in_subscription/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0     1318 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/reports/utils.py
+-rw-r--r--   0        0        0    37904 2023-04-19 06:50:55.191892 connect_cli-27.0/connect/.data/connect_reports/reports.json
+-rw-r--r--   0        0        0      245 2023-04-19 06:50:55.203892 connect_cli-27.0/connect/.data/connect_reports/sonar-project.properties
+-rw-r--r--   0        0        0      321 2023-04-19 06:50:55.207892 connect_cli-27.0/connect/.data/connect_reports/tox.ini
+-rw-r--r--   0        0        0      352 2023-04-19 06:48:02.393923 connect_cli-27.0/connect/cli/__init__.py
+-rw-r--r--   0        0        0     1712 2023-04-19 06:48:02.393923 connect_cli-27.0/connect/cli/ccli.py
+-rw-r--r--   0        0        0       54 2023-04-19 06:48:02.393923 connect_cli-27.0/connect/cli/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 06:48:02.393923 connect_cli-27.0/connect/cli/core/account/__init__.py
+-rw-r--r--   0        0        0     2433 2023-04-19 06:48:02.393923 connect_cli-27.0/connect/cli/core/account/commands.py
+-rw-r--r--   0        0        0     1233 2023-04-19 06:48:02.393923 connect_cli-27.0/connect/cli/core/account/helpers.py
+-rw-r--r--   0        0        0     2781 2023-04-19 06:48:02.393923 connect_cli-27.0/connect/cli/core/base.py
+-rw-r--r--   0        0        0     4049 2023-04-19 06:48:02.393923 connect_cli-27.0/connect/cli/core/config.py
+-rw-r--r--   0        0        0      573 2023-04-19 06:48:02.393923 connect_cli-27.0/connect/cli/core/constants.py
+-rw-r--r--   0        0        0     1424 2023-04-19 06:48:02.393923 connect_cli-27.0/connect/cli/core/http.py
+-rw-r--r--   0        0        0      838 2023-04-19 06:48:02.393923 connect_cli-27.0/connect/cli/core/plugins.py
+-rw-r--r--   0        0        0     6809 2023-04-19 06:48:02.393923 connect_cli-27.0/connect/cli/core/terminal.py
+-rw-r--r--   0        0        0     3167 2023-04-19 06:48:02.393923 connect_cli-27.0/connect/cli/core/utils.py
+-rw-r--r--   0        0        0        0 2023-04-19 06:48:02.393923 connect_cli-27.0/connect/cli/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 06:48:02.393923 connect_cli-27.0/connect/cli/plugins/customer/__init__.py
+-rw-r--r--   0        0        0     2138 2023-04-19 06:48:02.393923 connect_cli-27.0/connect/cli/plugins/customer/commands.py
+-rw-r--r--   0        0        0      526 2023-04-19 06:48:02.393923 connect_cli-27.0/connect/cli/plugins/customer/constants.py
+-rw-r--r--   0        0        0     5923 2023-04-19 06:48:02.393923 connect_cli-27.0/connect/cli/plugins/customer/export.py
+-rw-r--r--   0        0        0    12428 2023-04-19 06:48:02.393923 connect_cli-27.0/connect/cli/plugins/customer/sync.py
+-rw-r--r--   0        0        0        0 2023-04-19 06:48:02.393923 connect_cli-27.0/connect/cli/plugins/locale/__init__.py
+-rw-r--r--   0        0        0     1363 2023-04-19 06:48:02.393923 connect_cli-27.0/connect/cli/plugins/locale/commands.py
+-rw-r--r--   0        0        0      306 2023-04-19 06:48:02.393923 connect_cli-27.0/connect/cli/plugins/play/__init__.py
+-rw-r--r--   0        0        0     2486 2023-04-19 06:48:02.393923 connect_cli-27.0/connect/cli/plugins/play/commands.py
+-rw-r--r--   0        0        0     2395 2023-04-19 06:48:02.393923 connect_cli-27.0/connect/cli/plugins/play/context.py
+-rw-r--r--   0        0        0      428 2023-04-19 06:48:02.393923 connect_cli-27.0/connect/cli/plugins/play/save.py
+-rw-r--r--   0        0        0     1501 2023-04-19 06:48:02.393923 connect_cli-27.0/connect/cli/plugins/play/script.py
+-rw-r--r--   0        0        0        0 2023-04-19 06:48:02.393923 connect_cli-27.0/connect/cli/plugins/product/__init__.py
+-rw-r--r--   0        0        0     1675 2023-04-19 06:48:02.393923 connect_cli-27.0/connect/cli/plugins/product/api.py
+-rw-r--r--   0        0        0     8631 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/product/clone.py
+-rw-r--r--   0        0        0     9677 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/product/commands.py
+-rw-r--r--   0        0        0     1012 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/product/constants.py
+-rw-r--r--   0        0        0    33243 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/product/export.py
+-rw-r--r--   0        0        0      846 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/product/sync/__init__.py
+-rw-r--r--   0        0        0     5912 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/product/sync/actions.py
+-rw-r--r--   0        0        0    10140 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/product/sync/capabilities.py
+-rw-r--r--   0        0        0     3881 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/product/sync/configuration_values.py
+-rw-r--r--   0        0        0     5129 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/product/sync/general.py
+-rw-r--r--   0        0        0    11839 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/product/sync/items.py
+-rw-r--r--   0        0        0     5740 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/product/sync/media.py
+-rw-r--r--   0        0        0     9351 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/product/sync/params.py
+-rw-r--r--   0        0        0     3598 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/product/sync/static_resources.py
+-rw-r--r--   0        0        0     5457 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/product/sync/templates.py
+-rw-r--r--   0        0        0      961 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/product/utils.py
+-rw-r--r--   0        0        0        0 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/__init__.py
+-rw-r--r--   0        0        0     5328 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/commands.py
+-rw-r--r--   0        0        0        0 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/__init__.py
+-rw-r--r--   0        0        0      411 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/constants.py
+-rw-r--r--   0        0        0    10313 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/helpers.py
+-rw-r--r--   0        0        0      103 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/__init__.py.j2
+-rw-r--r--   0        0        0      852 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/anvil.py.j2
+-rw-r--r--   0        0        0     2920 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/events.py.j2
+-rw-r--r--   0        0        0      464 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/extension.json.j2
+-rw-r--r--   0        0        0      560 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/schemas.py.j2
+-rw-r--r--   0        0        0        0 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/static/.gitkeep.j2
+-rw-r--r--   0        0        0     1762 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/tfnapp.py.j2
+-rw-r--r--   0        0        0     7295 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/webapp.py.j2
+-rw-r--r--   0        0        0      702 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.${project_slug}_dev.env.j2
+-rw-r--r--   0        0        0     1083 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.eslintrc.yaml.j2
+-rw-r--r--   0        0        0      231 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.flake8.j2
+-rw-r--r--   0        0        0     1309 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.github/workflows/test.yml.j2
+-rw-r--r--   0        0        0       96 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.gitignore.j2
+-rw-r--r--   0        0        0       63 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/CHANGELOG.md.j2
+-rw-r--r--   0        0        0      301 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/Dockerfile.j2
+-rw-r--r--   0        0        0     1661 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/HOWTO.md.j2
+-rw-r--r--   0        0        0    14063 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/LICENSE.j2
+-rw-r--r--   0        0        0      195 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/README.md.j2
+-rw-r--r--   0        0        0      111 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/__mocks__/fileMock.js.j2
+-rw-r--r--   0        0        0       97 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/__mocks__/styleMock.js.j2
+-rw-r--r--   0        0        0       39 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/babel.config.json.j2
+-rw-r--r--   0        0        0      774 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/docker-compose.yml.j2
+-rw-r--r--   0        0        0      944 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/jest.config.js.j2
+-rw-r--r--   0        0        0     1246 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/package.json.j2
+-rw-r--r--   0        0        0       29 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/poetry.toml.j2
+-rw-r--r--   0        0        0     1960 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/pyproject.toml.j2
+-rw-r--r--   0        0        0      103 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/__init__.py.j2
+-rw-r--r--   0        0        0      559 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/conftest.py.j2
+-rw-r--r--   0        0        0      553 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_anvil.py.j2
+-rw-r--r--   0        0        0     2602 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_events.py.j2
+-rw-r--r--   0        0        0     1046 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_tfnapp.py.j2
+-rw-r--r--   0        0        0     8794 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_webapp.py.j2
+-rw-r--r--   0        0        0      947 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/images/mkp.svg.j2
+-rw-r--r--   0        0        0      729 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/pages/index.html.j2
+-rw-r--r--   0        0        0      928 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/pages/settings.html.j2
+-rw-r--r--   0        0        0      470 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/pages/transformations/copy.html.j2
+-rw-r--r--   0        0        0     1590 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/pages/transformations/manual.html.j2
+-rw-r--r--   0        0        0     2609 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/components.js.j2
+-rw-r--r--   0        0        0      323 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/pages/index.js.j2
+-rw-r--r--   0        0        0      320 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/pages/settings.js.j2
+-rw-r--r--   0        0        0      267 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/pages/transformations/copy.js.j2
+-rw-r--r--   0        0        0      308 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/pages/transformations/manual.js.j2
+-rw-r--r--   0        0        0    10273 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/pages.js.j2
+-rw-r--r--   0        0        0     1579 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/utils.js.j2
+-rw-r--r--   0        0        0     6381 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/styles/index.css.j2
+-rw-r--r--   0        0        0      693 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/styles/manual.css.j2
+-rw-r--r--   0        0        0     6508 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/tests/components.spec.js.j2
+-rw-r--r--   0        0        0     9181 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/tests/pages.spec.js.j2
+-rw-r--r--   0        0        0     4352 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/tests/utils.spec.js.j2
+-rw-r--r--   0        0        0     2512 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/webpack.config.js.j2
+-rw-r--r--   0        0        0     4496 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/utils.py
+-rw-r--r--   0        0        0      920 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/validators.py
+-rw-r--r--   0        0        0    12120 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/extension/wizard.py
+-rw-r--r--   0        0        0     5792 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/renderer.py
+-rw-r--r--   0        0        0        0 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/report/__init__.py
+-rw-r--r--   0        0        0     8611 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/report/helpers.py
+-rw-r--r--   0        0        0       73 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/report/templates/add/${initial_report_slug}/README.md.j2
+-rw-r--r--   0        0        0        0 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/report/templates/add/${initial_report_slug}/__init__.py.j2
+-rw-r--r--   0        0        0     1507 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/report/templates/add/${initial_report_slug}/entrypoint.py.j2
+-rw-r--r--   0        0        0        0 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/report/templates/add/${initial_report_slug}/templates/pdf/template.css.j2
+-rw-r--r--   0        0        0      499 2023-04-19 06:48:02.397923 connect_cli-27.0/connect/cli/plugins/project/report/templates/add/${initial_report_slug}/templates/pdf/template.html.j2.j2
+-rw-r--r--   0        0        0      150 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/project/report/templates/add/${initial_report_slug}/templates/xml/template.xml.j2.j2
+-rw-r--r--   0        0        0       69 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/README.md.j2
+-rw-r--r--   0        0        0        0 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/__init__.py.j2
+-rw-r--r--   0        0        0     1507 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/entrypoint.py.j2
+-rw-r--r--   0        0        0        0 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/templates/pdf/template.css.j2
+-rw-r--r--   0        0        0      518 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/templates/pdf/template.html.j2.j2
+-rw-r--r--   0        0        0      150 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/templates/xml/template.xml.j2.j2
+-rw-r--r--   0        0        0      271 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/.flake8.j2
+-rw-r--r--   0        0        0      803 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/.github/workflows/build.yml.j2
+-rw-r--r--   0        0        0       37 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/.gitignore.j2
+-rw-r--r--   0        0        0      458 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/HOWTO.md.j2
+-rw-r--r--   0        0        0    14063 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/LICENSE.j2
+-rw-r--r--   0        0        0      138 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/README.md.j2
+-rw-r--r--   0        0        0       29 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/poetry.toml.j2
+-rw-r--r--   0        0        0     1352 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/pyproject.toml.j2
+-rw-r--r--   0        0        0     2589 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/reports.json.j2
+-rw-r--r--   0        0        0      103 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/tests/__init__.py.j2
+-rw-r--r--   0        0        0     6397 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/tests/conftest.py.j2
+-rw-r--r--   0        0        0     2534 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/tests/test_${project_slug}.py.j2
+-rw-r--r--   0        0        0     5878 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/project/report/validations.py
+-rw-r--r--   0        0        0     8603 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/project/report/wizard.py
+-rw-r--r--   0        0        0     1403 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/project/utils.py
+-rw-r--r--   0        0        0     2798 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/project/validators.py
+-rw-r--r--   0        0        0        0 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/report/__init__.py
+-rw-r--r--   0        0        0     2405 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/report/commands.py
+-rw-r--r--   0        0        0       86 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/report/constants.py
+-rw-r--r--   0        0        0     6210 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/report/helpers.py
+-rw-r--r--   0        0        0     2812 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/report/utils.py
+-rw-r--r--   0        0        0     8418 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/report/wizard.py
+-rw-r--r--   0        0        0        0 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/shared/__init__.py
+-rw-r--r--   0        0        0     2442 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/shared/base.py
+-rw-r--r--   0        0        0     1973 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/shared/constants.py
+-rw-r--r--   0        0        0       46 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/shared/exceptions.py
+-rw-r--r--   0        0        0     2304 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/shared/export.py
+-rw-r--r--   0        0        0     6248 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/shared/sync_stats.py
+-rw-r--r--   0        0        0     5666 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/shared/translation_attr_sync.py
+-rw-r--r--   0        0        0     6390 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/shared/translation_sync.py
+-rw-r--r--   0        0        0     1996 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/shared/translations_synchronizers.py
+-rw-r--r--   0        0        0     6794 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/shared/utils.py
+-rw-r--r--   0        0        0        0 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/translation/__init__.py
+-rw-r--r--   0        0        0      707 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/translation/activate.py
+-rw-r--r--   0        0        0     6869 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/translation/commands.py
+-rw-r--r--   0        0        0      795 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/translation/constants.py
+-rw-r--r--   0        0        0     1216 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/translation/export.py
+-rw-r--r--   0        0        0      950 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/translation/primarize.py
+-rw-r--r--   0        0        0     8876 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/translation/translation_sync.py
+-rw-r--r--   0        0        0      832 2023-04-19 06:48:02.401923 connect_cli-27.0/connect/cli/plugins/translation/utils.py
+-rw-r--r--   0        0        0     3955 2023-04-19 06:50:55.947883 connect_cli-27.0/pyproject.toml
+-rw-r--r--   0        0        0     5186 1970-01-01 00:00:00.000000 connect_cli-27.0/PKG-INFO
```

### Comparing `connect_cli-26.9/LICENSE` & `connect_cli-27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/README.md` & `connect_cli-27.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # CloudBlue Connect Command Line Interface
 
-![pyversions](https://img.shields.io/pypi/pyversions/connect-cli.svg) [![PyPi Status](https://img.shields.io/pypi/v/connect-cli.svg)](https://pypi.org/project/connect-cli/) ![PyPI - Downloads](https://img.shields.io/pypi/dm/connect-cli) ![Docker Pulls](https://img.shields.io/docker/pulls/cloudblueconnect/connect-cli) ![GitHub Workflow Status](https://img.shields.io/github/workflow/status/cloudblue/connect-cli/Build%20Connect%20Command%20Line%20Client) [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=connect-cli&metric=coverage)](https://sonarcloud.io/summary/new_code?id=connect-cli) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=connect-cli&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=connect-cli)
+![pyversions](https://img.shields.io/pypi/pyversions/connect-cli.svg) [![PyPi Status](https://img.shields.io/pypi/v/connect-cli.svg)](https://pypi.org/project/connect-cli/) ![PyPI - Downloads](https://img.shields.io/pypi/dm/connect-cli) ![Docker Pulls](https://img.shields.io/docker/pulls/cloudblueconnect/connect-cli) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/cloudblue/connect-cli/build.yml?branch=master) [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=connect-cli&metric=coverage)](https://sonarcloud.io/summary/new_code?id=connect-cli) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=connect-cli&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=connect-cli)
 
 ## Introduction
 
 The CloudBlue Connect Command Line Interface (CLI) is an extensible unified tool to perform various automation scenarios. With just one tool, you can control multiple Connect modules from the command line and automate them through scripts.
 
 Since it is extensible, users can write their own plugins to extend its functionalities.
 
@@ -66,14 +66,19 @@
 * [Products](docs/products_usage.md)
 * [Customers](docs/customers_usage.md)
 * [Reports](docs/reports_usage.md)
 * [Translations](docs/translations_usage.md)
 * [Projects](docs/project_usage.md)
 
 
+## Development
+We use `isort` library to order and format our imports, and we check it using `flake8-isort` library (automatically on `flake8` run).  
+For convenience you may run `poetry run isort .` to order imports.
+
+
 ## Run tests
 
 `connect-cli` uses [poetry](https://python-poetry.org/) for dependencies management and packaging.
 
 To run the `connect-cli` tests suite run:
 
 ```
```

### Comparing `connect_cli-26.9/connect/.data/connect_reports/.github/workflows/build.yml` & `connect_cli-27.0/connect/.data/connect_reports/.github/workflows/build.yml`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     branches: [ master ]
 
 jobs:
   tests:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [3.8, 3.9, 3.10.1]
+        python-version: ['3.8', '3.9', '3.10']
     steps:
     - uses: actions/checkout@v2
       with:
         fetch-depth: 0
         submodules: true
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
@@ -40,15 +40,15 @@
     steps:
       - uses: actions/checkout@v2
         with:
           fetch-depth: 0
       - name: Set up Python 3.10.1
         uses: actions/setup-python@v2
         with:
-          python-version: '3.10.1'
+          python-version: '3.10'
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install poetry
           poetry install
       - name: Generate coverage report
         run: |
```

### Comparing `connect_cli-26.9/connect/.data/connect_reports/LICENSE` & `connect_cli-27.0/connect/.data/connect_reports/LICENSE`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/README.md` & `connect_cli-27.0/connect/.data/connect_reports/README.md`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/poetry.lock` & `connect_cli-27.0/connect/.data/connect_reports/poetry.lock`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/pyproject.toml` & `connect_cli-27.0/connect/.data/connect_reports/pyproject.toml`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/billing_requests/entrypoint.py` & `connect_cli-27.0/connect/.data/connect_reports/reports/billing_requests/entrypoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (c) 2021, CloudBlue
+# Copyright (c) 2023, CloudBlue
 # All rights reserved.
 #
 
 from connect.client import R
 
 from ..utils import convert_to_datetime, get_basic_value, get_value
```

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/billing_requests/templates/xlsx/template.xlsx` & `connect_cli-27.0/connect/.data/connect_reports/reports/billing_requests/templates/xlsx/template.xlsx`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/billing_requests_line_item/entrypoint.py` & `connect_cli-27.0/connect/.data/connect_reports/reports/billing_requests_line_item/entrypoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (c) 2021, CloudBlue
+# Copyright (c) 2023, CloudBlue
 # All rights reserved.
 #
 
 from connect.client import R
 
 from ..utils import convert_to_datetime, get_basic_value, get_value
```

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/billing_requests_line_item/templates/xlsx/template.xlsx` & `connect_cli-27.0/connect/.data/connect_reports/reports/billing_requests_line_item/templates/xlsx/template.xlsx`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/contract_list/entrypoint.py` & `connect_cli-27.0/connect/.data/connect_reports/reports/contract_list/entrypoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (c) 2021, CloudBlue
+# Copyright (c) 2023, CloudBlue
 # All rights reserved.
 #
 
 from connect.client import R
 
 from ..utils import convert_to_datetime, get_basic_value, get_value
```

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/contract_list/templates/xlsx/template.xlsx` & `connect_cli-27.0/connect/.data/connect_reports/reports/contract_list/templates/xlsx/template.xlsx`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/customers_list/entrypoint.py` & `connect_cli-27.0/connect/.data/connect_reports/reports/customers_list/entrypoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (c) 2021, CloudBlue
+# Copyright (c) 2023, CloudBlue
 # All rights reserved.
 #
 
 from connect.client import R
 
 from ..utils import get_basic_value, get_value
```

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/customers_list/templates/xlsx/template.xlsx` & `connect_cli-27.0/connect/.data/connect_reports/reports/customers_list/templates/xlsx/template.xlsx`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/executive_fullfilment_requests/Readme.md` & `connect_cli-27.0/connect/.data/connect_reports/reports/executive_fullfilment_requests/Readme.md`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/executive_fullfilment_requests/constants.py` & `connect_cli-27.0/connect/.data/connect_reports/reports/executive_fullfilment_requests/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 ELEMENTS_PER_CHART = 10
 
 COUNTRIES = {
     "AW": "Aruba",
     "AF": "Afghanistan",
     "AO": "Angola",
     "AI": "Anguilla",
+    "AN": "Netherlands Antilles",
     "AX": "Åland Islands",
     "AL": "Albania",
     "AD": "Andorra",
     "AE": "United Arab Emirates",
     "AR": "Argentina",
     "AM": "Armenia",
     "AS": "American Samoa",
```

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/executive_fullfilment_requests/entrypoint.py` & `connect_cli-27.0/connect/.data/connect_reports/reports/executive_fullfilment_requests/entrypoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (c) 2021, CloudBlue
+# Copyright (c) 2023, CloudBlue
 # All rights reserved.
 #
 import pathlib
 from datetime import date
 from tempfile import NamedTemporaryFile
 from collections import namedtuple
 import math
@@ -36,15 +36,20 @@
     query &= R().created.le(parameters['date']['before'])
     query &= R().status.oneof(final_status)
 
     if parameters.get('product') and parameters['product']['all'] is False:
         query &= R().asset.product.id.oneof(parameters['product']['choices'])
     if parameters.get('rr_type') and parameters['rr_type']['all'] is False:
         query &= R().type.oneof(parameters['rr_type']['choices'])
-    return client.requests.filter(query).select('-asset.params', '-asset.configuration')
+    return client.requests.filter(query).select(
+        '-asset.params',
+        '-asset.configuration',
+        '-activation_key',
+        '-template',
+    )
 
 
 def _get_request_count_group_by_type(client, parameters):
     final_status = (
         'approved', 'failed', 'revoked',
     )
     rr_types = ('adjustment', 'purchase', 'change', 'suspend', 'resume', 'cancel')
@@ -430,15 +435,15 @@
     product['provision_times'].append(request['provision_time'])
     report_data['product'][product_id] = product
 
 
 def _process_country_data(report_data, request):
     country = get_dict_element(request, 'asset', 'tiers', 'customer', 'contact_info', 'country')
     if country:
-        country_name = COUNTRIES[country.upper()]
+        country_name = COUNTRIES.get(country.upper(), "Antarctica")
 
         country_data = report_data['country'].get(
             country_name,
             {'amount': 0},
         )
         country_data['amount'] += 1
         report_data['country'][country_name] = country_data
```

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/executive_fullfilment_requests/templates/pdf/img/ClouBlue-Logo.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/executive_fullfilment_requests/templates/pdf/img/ClouBlue-Logo.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/executive_fullfilment_requests/templates/pdf/template.css` & `connect_cli-27.0/connect/.data/connect_reports/reports/executive_fullfilment_requests/templates/pdf/template.css`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/executive_fullfilment_requests/templates/pdf/template.html.j2` & `connect_cli-27.0/connect/.data/connect_reports/reports/executive_fullfilment_requests/templates/pdf/template.html.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/fulfillment_requests/entrypoint.py` & `connect_cli-27.0/connect/.data/connect_reports/reports/fulfillment_requests/entrypoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (c) 2021, CloudBlue
+# Copyright (c) 2023, CloudBlue
 # All rights reserved.
 #
 
 from connect.client import R
 
 from ..utils import convert_to_datetime, get_basic_value, get_value, today_str
 
@@ -71,14 +71,16 @@
     if parameters.get('hub') and parameters['hub']['all'] is False:
         query &= R().asset.connection.hub.id.oneof(parameters['hub']['choices'])
 
     return client.requests.filter(query).select(
         '-asset.items',
         '-asset.params',
         '-asset.configuration',
+        '-activation_key',
+        '-template',
     )
 
 
 def _process_line(request, connection):
     return (
         get_basic_value(request, 'id'),
         get_basic_value(request, 'type'),
```

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/fulfillment_requests/templates/xlsx/template.xlsx` & `connect_cli-27.0/connect/.data/connect_reports/reports/fulfillment_requests/templates/xlsx/template.xlsx`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/fulfillment_requests_failed/entrypoint.py` & `connect_cli-27.0/connect/.data/connect_reports/reports/fulfillment_requests_failed/entrypoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (c) 2021, CloudBlue
+# Copyright (c) 2023, CloudBlue
 # All rights reserved.
 #
 
 from connect.client import R
 
 from ..utils import convert_to_datetime, get_basic_value, get_value, today_str
 
@@ -63,14 +63,16 @@
     if parameters.get('connection_type') and parameters['connection_type']['all'] is False:
         query &= R().asset.connection.type.oneof(parameters['connection_type']['choices'])
 
     return client.requests.filter(query).select(
         '-asset.items',
         '-asset.params,'
         '-asset.configuration',
+        '-activation_key',
+        '-template',
     )
 
 
 def _process_line(request, connection):
     return (
         get_basic_value(request, 'id'),
         get_basic_value(request, 'type'),
```

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/fulfillment_requests_failed/templates/xlsx/template.xlsx` & `connect_cli-27.0/connect/.data/connect_reports/reports/fulfillment_requests_failed/templates/xlsx/template.xlsx`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/fulfillment_requests_line_item/entrypoint.py` & `connect_cli-27.0/connect/.data/connect_reports/reports/fulfillment_requests_line_item/entrypoint.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (c) 2021, CloudBlue
+# Copyright (c) 2023, CloudBlue
 # All rights reserved.
 #
 
 from connect.client import R
 
 from ..utils import convert_to_datetime, get_basic_value, get_value, today_str
 
 HEADERS = (
-    'Request ID', 'Request Type',
+    'Request ID', 'Request Type', 'Request Status',
     'Created At', 'Updated At', 'Exported At',
     'Item ID', 'Item Name', 'Item Type', 'Item Unit Of measure', 'Item MPN', 'Item Period',
     'Quantity', 'Customer ID', 'Customer Name', 'Customer External ID',
     'Tier 1 ID', 'Tier 1 Name', 'Tier 1 External ID',
     'Tier 2 ID', 'Tier 2 Name', 'Tier 2 External ID',
     'Provider ID', 'Provider Name', 'Vendor ID', 'Vendor Name',
     'Product ID', 'Product Name', 'Asset ID', 'Asset External ID',
-    'Transaction Type', 'Hub ID', 'Hub Name', 'Request Status',
+    'Transaction Type', 'Hub ID', 'Hub Name', 'Asset Status',
 )
 
 
 def generate(
     client=None,
     parameters=None,
     progress_callback=None,
@@ -68,21 +68,27 @@
     else:
         query &= R().status.oneof(all_types)
     if parameters.get('mkp') and parameters['mkp']['all'] is False:
         query &= R().asset.marketplace.id.oneof(parameters['mkp']['choices'])
     if parameters.get('hub') and parameters['hub']['all'] is False:
         query &= R().asset.connection.hub.id.oneof(parameters['hub']['choices'])
 
-    return client.requests.filter(query).all()
+    return client.requests.filter(query).select(
+        '-asset.params,'
+        '-asset.configuration',
+        '-activation_key',
+        '-template',
+    )
 
 
 def _process_line(item, request, connection):
     return (
         get_basic_value(request, 'id'),
         get_basic_value(request, 'type'),
+        get_basic_value(request, 'status'),
         convert_to_datetime(
             get_basic_value(request, 'created'),
         ),
         convert_to_datetime(
             get_basic_value(request, 'updated'),
         ),
         today_str(),
```

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/fulfillment_requests_line_item/templates/xlsx/template.xlsx` & `connect_cli-27.0/connect/.data/connect_reports/reports/listing_list/templates/xlsx/template.xlsx`

 * *Files 16% similar despite different names*

```diff
@@ -137,436 +137,408 @@
 00000880: cbb4 e480 fa84 53ec ad82 b4b7 b720 9a29  ......S...... .)
 00000890: 66e5 ffb9 43db f606 9f82 791f d1f3 1909  f...C.....y.....
 000008a0: 493c 0d79 00d1 e8d4 212b f8c1 45f6 08f2  I<.y....!+..E...
 000008b0: bcfc 664d 79ce 6bc1 a3fa 0ce5 1cab 4b1e  ..fMy.k.......K.
 000008c0: aa35 3d7c 8674 2087 c847 1f7f 2992 73e5  .5=|.t ..G..).s.
 000008d0: a299 bb55 efe1 7442 fbca 29bf dbf2 2ccb  ...U..tB..)...,.
 000008e0: f4ef 66e4 c9c7 d5df 0000 00ff ff03 0050  ..f............P
-000008f0: 4b03 0414 0006 0008 0000 0021 006a e588  K..........!.j..
-00000900: 47e6 0200 00c0 0600 000f 0000 0078 6c2f  G............xl/
-00000910: 776f 726b 626f 6f6b 2e78 6d6c a455 514f  workbook.xml.UQO
-00000920: db30 107e 9fb4 ff90 597d 4d1d 8736 2d11  .0.~....Y}M..6-.
-00000930: 292a 74dd 2a6d 131a 031e 2bd7 7189 8563  )*t.*m....+.q..c
-00000940: 67b6 438b 10ff 7de7 b429 94be 3088 5a3b  g.C...}..)..0.Z;
-00000950: 9773 3e7f 77f7 9d73 72ba 2e65 70cf 8d15  .s>.w..sr..ep...
-00000960: 5a65 8874 2314 70c5 742e d46d 86ae fe4c  Ze.t#.p.t..m...L
-00000970: c321 0aac a32a a752 2b9e a107 6ed1 e9e8  .!...*.R+...n...
-00000980: f3a7 9395 3677 0bad ef02 0050 3643 8573  ....6w.....P6C.s
-00000990: 558a b165 052f a9ed ea8a 2bf0 2cb5 29a9  U..e./....+.,.).
-000009a0: 03d3 dc62 5b19 4e73 5b70 ee4a 89e3 284a  ...b[.Ns[p.J..(J
-000009b0: 7049 8542 1b84 d4bc 0543 2f97 82f1 8966  pI.B.....C/....f
-000009c0: 75c9 95db 8018 2ea9 03fa b610 956d d14a  u............m.J
-000009d0: f616 b892 9abb ba0a 992e 2b80 5808 29dc  ..........+.X.).
-000009e0: 4303 8a82 92a5 b35b a50d 5d48 087b 4dfa  C......[..]H.{M.
-000009f0: c1da c02f 813f 8960 88db 9dc0 75b0 5529  .../.?.`....u.U)
-00000a00: 98d1 562f 5d17 a0f1 86f4 41fc 24c2 84ec  ..V/].....A.$...
-00000a10: a560 7d98 83b7 21f5 b0e1 f7c2 d770 c7ca  .`}...!......p..
-00000a20: 24ef 6495 ecb0 9267 3012 7d18 8d80 b41a  $.d....g0.}.....
-00000a30: ada4 90bc 77a2 f577 dc62 343a 590a c9af  ....w..w.b4:Y...
-00000a40: 37d2 0d68 55fd a2a5 af94 4481 a4d6 7dcd  7..hU.....D...}.
-00000a50: 85e3 7986 0660 ea15 df7b 60ea eaac 1612  ..y..`...{`.....
-00000a60: bc84 c471 84f0 6827 e70b 0306 d47e 2c1d  ...q..h'.....~,.
-00000a70: 378a 3a7e ae95 03a9 6da9 7f54 560d f679  7.:~....m..TV..y
-00000a80: a141 c4c1 6ffe b716 8643 ef80 8420 1c18  .A..o....C... ..
-00000a90: 294b e9c2 5e50 5704 b591 19c2 5716 e203  )K..^PW.....W...
-00000aa0: 8d18 4670 ab7a 8b81 93e2 cc61 b699 4326  ..Fp.z.....a..C&
-00000ab0: 0566 8a39 3f1b 5e69 e3ec ced7 daed bcac  .f.9?.^i........
-00000ac0: 25e4 4dfa f699 1b60 0099 b1f8 8596 e961  %.M....`.......a
-00000ad0: e3fc 879a 29f3 c9c4 90c0 4d90 9bfb d7c9  ....).....M.....
-00000ae0: 8458 4dda 2af6 c299 00ee 6793 1f50 b54b  .XM.*.....g..P.K
-00000af0: 7a0f 3504 a5e4 db16 9ff9 221d cd15 3329  z.5......."...3)
-00000b00: 993f 4efb 496f d0eb 9370 328e 86e1 71d2  .?N.Io...p2...q.
-00000b10: 3b0b 8f07 fdf3 f06c 3898 46c3 afd1 208e  ;......l8.F... .
-00000b20: 074f 108c 4952 a669 ed8a ad3c 3c74 867a  .O..IR.i...<<t.z
-00000b30: 5ed0 af5d 3fe9 baf5 9028 ad45 fe4c e331  ^..]?....(.E.L.1
-00000b40: da5e a19f 5f0d adef c907 ec0f c26b c157  .^.._........k.W
-00000b50: f659 48de 0cd6 3742 e57a 95a1 a324 4e20  .YH...7B.z...$N 
-00000b60: aa87 d6ee 4760 ad1a e78d c85d 012b fac3  ....G`.....].+..
-00000b70: deee d977 2e6e 0b60 1c47 c42f 8486 f1cc  ...w.n.`.G./....
-00000b80: 32b4 c768 b261 3485 2bf4 c31e 23fc 8252  2..h.a4.+...#..R
-00000b90: 73e4 02b5 660e 54d3 2613 ea28 9cec fe30  s...f.T.&..(...0
-00000ba0: f629 86d3 cca4 7e07 33cb 4953 c2f6 a59c  .)....~.3.IS....
-00000bb0: 2f85 e2b9 6f2e 8078 616d 81e6 6ba9 caee  /...o..xam..k...
-00000bc0: 7c2a 7cc3 78d4 05b5 dcf7 1ca3 f2b2 8587  |*|.x...........
-00000bd0: 180a 91e7 dc7f 62d0 c8af fad2 1977 48da  ......b......wH.
-00000be0: 197f eb90 13fc 0215 04b3 bf23 c0b0 0b13  ...........#....
-00000bf0: f8c9 136d 9a15 b71f 9fd1 3f00 0000 ffff  ...m......?.....
-00000c00: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
-00000c10: e4ac 1593 eb02 0000 1f07 0000 0d00 0000  ................
-00000c20: 786c 2f73 7479 6c65 732e 786d 6ca4 55db  xl/styles.xml.U.
-00000c30: 8e9b 3010 7daf d47f b0fc 4eb8 0448 8842  ..0.}.....N..H.B
-00000c40: 564d b248 2b6d ab4a bb95 faea 8049 acf5  VM.H+m.J.....I..
-00000c50: 0519 2725 adfa ef1d 0321 acb6 6ab7 dbbc  ..'%.....!..j...
-00000c60: d81e c667 cecc 194f 9637 8de0 e844 75cd  ...g...O.7...Du.
-00000c70: 944c b13f f130 a232 5705 93fb 147f 79cc  .L.?.0.2W.....y.
-00000c80: 9c39 46b5 21b2 205c 499a e233 adf1 cdea  .9F.!. \I..3....
-00000c90: fdbb 656d ce9c 3e1c 2835 0820 649d e283  ..em..>.(5. d...
-00000ca0: 31d5 c275 ebfc 4005 a927 aaa2 12be 944a  1..u..@..'.....J
-00000cb0: 0b62 e0a8 f76e 5d69 4a8a da5e 12dc 0d3c  .b...n]iJ..^...<
-00000cc0: 2f76 0561 1277 080b 91bf 0644 10fd 74ac  /v.a.w.....D..t.
-00000cd0: 9c5c 898a 18b6 639c 9973 8b85 91c8 1777  .\....c..s.....w
-00000ce0: 7ba9 34d9 71a0 daf8 21c9 51e3 c73a 408d  {.4.q...!.Q..:@.
-00000cf0: be04 69ad 2fe2 0896 6b55 abd2 4c00 d755  ..i./...kU..L..U
-00000d00: 65c9 72fa 926e e226 2ec9 af48 80fc 3624  e.r..n.&...H..6$
-00000d10: 3f72 bde0 59ee 8d7e 2352 e86a 7a62 563e  ?r..Y..~#R.jzbV>
-00000d20: bc5a 964a 9a1a e5ea 280d 8809 446d 0916  .Z.J....(...Dm..
-00000d30: 4f52 7d93 99fd 648d 9dd7 6a59 7f47 27c2  OR}...d...jY.G'.
-00000d40: c1e2 6377 b5cc 1557 1a19 900e 2ad7 5a24  ..cw...W....*.Z$
-00000d50: 11b4 f3d8 10ce 769a 59b7 9208 c6cf 9d39  ......v.Y......9
-00000d60: b086 56ed de4f 30a8 bd35 ba96 47bf d470  ..V..O0..5..G..p
-00000d70: 8971 3eb0 9a5a 0260 582d 413e 43b5 cce0  .q>..Z.`X-A>C...
-00000d80: 80fa fde3 b982 f012 3aad 8369 fdfe e2bd  ........:..i....
-00000d90: d7e4 ec07 d1eb 2fd4 8ab3 c2b2 d86f c649  ....../......o.I
-00000da0: 43e7 1b66 ebe6 7893 204c 92d9 ccb7 bfd9  C..f..x. L......
-00000db0: 3c99 5aec 5def cd64 411b 5aa4 380e db90  <.Z.]..dA.Z.8...
-00000dc0: a32c 6cc6 2de3 7681 c477 4a17 f0b4 ae82  .,l.-.v..wJ.....
-00000dd0: 5c4c ab25 a7a5 0154 cdf6 07bb 1a55 d918  \L.%...T.....U..
-00000de0: ca18 68bf d5b2 6064 af24 e1b6 961d c8b0  ..h...`d.$......
-00000df0: 01d8 9c72 fe60 9fdf d7f2 1976 5322 7914  ...r.`.....vS"y.
-00000e00: 9930 7740 0fd2 b12a 5cb6 c0ab df76 78dd  .0w@...*\....vx.
-00000e10: c1e2 8fd1 3aec 116c 0075 fa77 58d4 9403  ....:..l.u.wX...
-00000e20: fe2b 6e07 188d 490d b711 a92a 7eb6 fdd1  .+n...I....*~...
-00000e30: b764 cb15 d88d 4af0 ac00 432a c836 6f8a  .d....J...C*.6o.
-00000e40: 3fd9 d9c3 e119 f474 d0ee c838 88fc 9be4  ?......t...8....
-00000e50: 01b3 68ae e5f4 acb6 c6ce 91b6 d043 14a8  ..h..........C..
-00000e60: 6a41 4b72 e4e6 71f8 98e2 ebfe 232d d851  jAKr..q.....#-.Q
-00000e70: 2483 d767 7652 a685 48f1 757f 6f55 f763  $..gvR..H.u.oU.c
-00000e80: 1b83 36e6 be86 b702 2b3a 6a96 e21f b7eb  ..6.....+:j.....
-00000e90: 59b2 bdcd 0267 eead e74e 38a5 9193 44eb  Y....g...N8...D.
-00000ea0: ad13 859b f576 9b25 5ee0 6d7e 8ea6 d97f  .....v.%^.m~....
-00000eb0: ccb2 76f8 82c0 7eb8 a839 4c3c dd27 dba7  ..v...~..9L<.'..
-00000ec0: f870 b5a5 7874 e8e8 b7dd 0fb4 c7dc 9320  .p..xt......... 
-00000ed0: f63e 44be e764 53cf 77c2 98cc 9d79 3c8d  .>D..dS.w....y<.
-00000ee0: 9c2c f283 6d1c ae6f a32c 1a71 8fde 38f3  .,..m..o.,.q..8.
-00000ef0: 3cd7 f7bb e969 c947 0bc3 04e5 4c5e b4ba  <....i.G....L^..
-00000f00: 2834 b682 4870 fc43 12ee 4509 f7fa cfb6  (4..Hp.C..E.....
-00000f10: fa05 0000 ffff 0300 504b 0304 1400 0600  ........PK......
-00000f20: 0800 0000 2100 e9a6 25b8 6606 0000 531b  ....!...%.f...S.
-00000f30: 0000 1300 0000 786c 2f74 6865 6d65 2f74  ......xl/theme/t
-00000f40: 6865 6d65 312e 786d 6cec 59cd 6e1b 3710  heme1.xml.Y.n.7.
-00000f50: be17 e83b 107b 4f2c d992 6219 9103 4b96  ...;.{O,..b...K.
-00000f60: e236 7162 d84a 8a1c a95d 6a97 1177 b920  .6qb.J...]j..w. 
-00000f70: 293b ba15 c9b1 4081 a269 d14b 81de 7a28  );....@..i.K..z(
-00000f80: da06 4880 5ed2 a771 9ba2 4d81 bc42 87e4  ..H.^..q..M..B..
-00000f90: 4a5a 5a54 6c27 06fa 171d 6c2d f7e3 fccf  JZZTl'....l-....
-00000fa0: 7086 ba7a ed41 cad0 2111 92f2 ac15 542f  p..z.A..!.....T/
-00000fb0: 5702 44b2 9047 348b 5bc1 9d7e efd2 7a80  W.D..G4.[..~..z.
-00000fc0: a4c2 5984 19cf 482b 9810 195c db7c ffbd  ..Y...H+...\.|..
-00000fd0: ab78 4325 2425 08f6 6772 03b7 8244 a97c  .xC%$%..gr...D.|
-00000fe0: 6365 4586 b08c e565 9e93 0cde 0db9 48b1  ceE....e......H.
-00000ff0: 8247 11af 4402 1f01 dd94 adac 562a 8d95  .G..D.......V*..
-00001000: 14d3 2c40 194e 81ec ede1 9086 04f5 35c9  ..,@.N........5.
-00001010: 6073 4abc cbe0 3153 522f 844c 1c68 d2c4  `sJ...1SR/.L.h..
-00001020: d961 b0d1 a8aa 1172 223b 4ca0 43cc 5a01  .a.....r";L.C.Z.
-00001030: f089 f851 9f3c 5001 6258 2a78 d10a 2ae6  ...Q.<P.bX*x..*.
-00001040: 13ac 6c5e 5dc1 1bc5 26a6 96ec 2ded eb99  ..l^]...&...-...
-00001050: 4fb1 afd8 108d 560d 4f11 0f66 4cab bd5a  O.....V.O..fL..Z
-00001060: f3ca f68c be01 30b5 88eb 76bb 9d6e 7546  ......0...v..nuF
-00001070: cf00 7018 82a6 5696 32cd 5a6f bdda 9ed2  ..p...V.2.Zo....
-00001080: 2c81 ecd7 45da 9d4a bd52 73f1 25fa 6b0b  ,...E..J.Rs.%.k.
-00001090: 3237 dbed 76bd 59c8 6289 1a90 fd5a 5bc0  27..v.Y.b....Z[.
-000010a0: af57 1ab5 ad55 076f 4016 5f5f c0d7 da5b  .W...U.o@.__...[
-000010b0: 9d4e c3c1 1b90 c537 16f0 bd2b cd46 cdc5  .N.....7...+.F..
-000010c0: 1b50 c268 365a 406b 87f6 7a05 f519 64c8  .P.h6Z@k..z...d.
-000010d0: d98e 17be 0ef0 f54a 019f a320 1a66 d1a5  .......J... .f..
-000010e0: 590c 79a6 96c5 5a8a ef73 d103 8006 32ac  Y.y...Z..s....2.
-000010f0: 6886 d424 2743 1c42 1477 703a 1014 6b06  h..$'C.B.wp:..k.
-00001100: 7883 e0d2 1bbb 14ca 8525 cd0b c950 d05c  x........%...P.\
-00001110: b582 0f73 0c19 31a7 f7ea f9f7 af9e 3f45  ...s..1.......?E
-00001120: af9e 3f39 7ef8 ecf8 e14f c78f 1e1d 3ffc  ..?9~....O....?.
-00001130: d1d2 7236 eee0 2c2e 6f7c f9ed 677f 7efd  ..r6..,.o|..g.~.
-00001140: 31fa e3e9 372f 1f7f e1c7 cb32 fed7 1f3e  1...7/.....2...>
-00001150: f9e5 e7cf fd40 c8a0 b944 2fbe 7cf2 dbb3  .....@...D/.|...
-00001160: 272f befa f4f7 ef1e 7be0 5b02 0fca f03e  '/......{.[....>
-00001170: 4d89 44b7 c811 dae7 29e8 660c e34a 4e06  M.D.....).f..JN.
-00001180: e27c 3bfa 09a6 ce0e 9c00 6d0f e9ae 4a1c  .|;.......m...J.
-00001190: e0ad 0966 3e5c 9bb8 c6bb 2ba0 78f8 80d7  ...f>\....+.x...
-000011a0: c7f7 1d59 0f12 3156 d4c3 f946 923a c05d  ...Y..1V...F.:.]
-000011b0: ce59 9b0b af01 6e68 5e25 0bf7 c759 ec67  .Y....nh^%...Y.g
-000011c0: 2ec6 65dc 3ec6 873e de1d 9c39 aeed 8e73  ..e.>..>...9...s
-000011d0: a89a d3a0 746c df49 8823 e61e c399 c231  ....tl.I.#.....1
-000011e0: c988 42fa 1d1f 11e2 d1ee 1ea5 8e5d 7769  ..B..........]wi
-000011f0: 28b8 e443 85ee 51d4 c6d4 6b92 3e1d 3881  (..C..Q...k.>.8.
-00001200: 34df b443 53f0 cbc4 a733 b8da b1cd ee5d  4..CS....3.....]
-00001210: d4e6 cca7 f536 3974 9190 1098 7984 ef13  .....69t....y...
-00001220: e698 f13a 1e2b 9cfa 48f6 71ca ca06 bf89  ...:.+..H.q.....
-00001230: 55e2 13f2 6022 c232 ae2b 1578 3a26 8ca3  U...`".2.+.x:&..
-00001240: 6e44 a4f4 edb9 2d40 df92 d36f 60a8 575e  nD....-@...o`.W^
-00001250: b7ef b249 ea22 85a2 231f cd9b 98f3 3272  ...I."..#.....2r
-00001260: 9b8f 3a09 4e73 afcc 344b cad8 0fe4 0842  ..:.Ns..4K.....B
-00001270: 14a3 3dae 7cf0 5dee 6688 7e06 3fe0 6ca9  ..=.|.].f.~.?.l.
-00001280: bbef 52e2 b8fb f442 7087 c68e 48f3 00d1  ..R....Bp...H...
-00001290: 6fc6 a2a8 da4e fd4d 69f6 ba62 cc28 54e3  o....N.Mi..b.(T.
-000012a0: 77c5 787a 3a6d c1d1 e44b 899d 1325 7819  w.xz:m...K...%x.
-000012b0: ee5f 5878 b7f1 38db 2310 eb8b 07cf bbba  ._Xx..8.#.......
-000012c0: fbae ee06 fff9 babb 2c97 cf5a 6de7 0516  ........,..Zm...
-000012d0: 9ae4 795f 6cba e474 6993 3ca4 8c1d a809  ..y_l..ti.<.....
-000012e0: 2337 a5e9 9325 1c16 510f 164d 036f a6b8  #7...%..Q..M.o..
-000012f0: d9d0 9427 f0b5 28ee 0e2e 16d8 ec41 82ab  ...'..(......A..
-00001300: 8fa8 4a0e 129c 438f 5d35 235f 2c0b d2b1  ..J...C.]5#_,...
-00001310: 4439 9730 db99 6533 7c92 13b4 cd38 49a1  D9.0..e3|....8I.
-00001320: cd36 9361 5dcf 0cb6 1e48 ac76 7964 97d7  .6.a]....H.vyd..
-00001330: cab3 e18c 8c99 1463 337f 4e19 ad69 0267  .......c3.N..i.g
-00001340: 65b6 76e5 ed98 55ad 544b cde6 aa56 35a2  e.v...U.TK...V5.
-00001350: 9952 e7a8 3653 197c b8a8 1a2c ceac 095d  .R..6S.|...,...]
-00001360: 0882 de05 acdc 8011 5dcb 0eb3 0966 24d2  ........]....f$.
-00001370: 76b7 73f3 d42d 9af5 85ba 4826 3822 858f  v.s..-....H&8"..
-00001380: b4de 8b3e aa1a 274d 6365 1a46 1e1f e939  ...>..'Mce.F...9
-00001390: ef14 1f95 b835 35d9 b7e0 7616 2795 d9d5  .....55...v.'...
-000013a0: 96b0 9b7a ef6d bc34 1d6e e75e d279 7b22  ...z.m.4.n.^.y{"
-000013b0: 1d59 564e 4e96 a1a3 56d0 acaf d603 14e2  .YVNN...V.......
-000013c0: bc15 0c61 ac85 af69 0e5e 97ba f1c3 2c86  ...a...i.^....,.
-000013d0: bba1 5009 1bf6 a726 b309 d7b9 379b feb0  ..P....&....7...
-000013e0: acc2 4d85 b5fb 82c2 4e1d c885 54db 5826  ..M.....N...T.X&
-000013f0: 3634 ccab 2204 5866 8670 23ff 6a1d cc7a  64..".Xf.p#.j..z
-00001400: 510a d848 7f03 29d6 d621 18fe 3629 c08e  Q..H..)..!..6)..
-00001410: ae6b c970 4842 5576 7669 c5dc 5118 4051  .k.pHBUvvi..Q.@Q
-00001420: 4af9 5811 7190 4447 68c0 c662 1f83 fb75  J.X.q.DGh..b...u
-00001430: a882 3e11 9570 3b61 2a82 7e80 ab34 6d6d  ..>..p;a*.~..4mm
-00001440: f3ca 2dce 45d2 952f b00c ceae 6396 27b8  ..-.E../....c.'.
-00001450: 28b7 3a45 a799 6ce1 268f 6732 9827 2bad  (.:E..l.&.g2.'+.
-00001460: 110f 74f3 ca6e 943b bf2a 26e5 2f48 9572  ..t..n.;.*&./H.r
-00001470: 18ff cf54 d1e7 095c 17ac 45da 0321 dce4  ...T...\..E..!..
-00001480: 0a8c 74be b602 2e54 c2a1 0ae5 090d 7b02  ..t....T......{.
-00001490: 2eb9 4ced 8068 81eb 5878 0d41 05f7 c9e6  ..L..h..Xx.A....
-000014a0: bf20 87fa bfcd 394b c3a4 354c 7d6a 9fc6  . ....9K..5L}j..
-000014b0: 4850 388f 5422 08d9 83b2 64a2 ef14 62d5  HP8.T"....d...b.
-000014c0: e2ec b224 5941 c844 5449 5c99 5bb1 07e4  ...$YA.DTI\.[...
-000014d0: 90b0 beae 810d 7db6 0728 8150 37d5 a428  ......}..(.P7..(
-000014e0: 0306 7732 fedc e722 8306 b16e 72fe a99d  ..w2..."...nr...
-000014f0: 8f4d e6f3 b607 ba3b b02d 96dd 7fc6 5ea4  .M.....;.-....^.
-00001500: 562a faa5 a3a0 e93d fb4c 4f35 2b07 af39  V*.....=.LO5+..9
-00001510: d8cf 79d4 da8a b5a0 f16a fdcc 476d 0e97  ..y......j..Gm..
-00001520: 3e48 ff81 f38f 8a90 d91f 27f4 81da e7fb  >H........'.....
-00001530: 505b 11fc d660 db2b 0451 7dc9 361e 4817  P[...`.+.Q}.6.H.
-00001540: 485b 1e07 d038 d945 1b4c 9a94 6d58 8aee  H[...8.E.L..mX..
-00001550: f6c2 db28 b891 2e3a dd19 5fc8 d237 e974  ...(...:.._..7.t
-00001560: cf69 ec59 73e6 b273 72f1 f5dd e7f9 8c5d  .i.Ys..sr......]
-00001570: 58d8 b175 b9d3 f598 1a92 f664 8aea f668  X..u.......d...h
-00001580: 3ac8 18c7 985f b5ca 3f3c f1c1 7d70 f436  :...._..?<..}p.6
-00001590: 5cf1 8f99 92f6 6aff 015c f1c1 9461 7f24  \.....j..\...a.$
-000015a0: 80e4 b7ce 355b 37ff 0200 00ff ff03 0050  ....5[7........P
-000015b0: 4b03 0414 0006 0008 0000 0021 0005 f4c1  K..........!....
-000015c0: f053 0400 00e4 1000 0018 0000 0078 6c2f  .S...........xl/
-000015d0: 776f 726b 7368 6565 7473 2f73 6865 6574  worksheets/sheet
-000015e0: 312e 786d 6cac 585b 93da 3614 7eef 4cff  1.xml.X[..6.~.L.
-000015f0: 83c7 efd8 966c ae03 649c 6569 b64d 9a34  .....l..d.ei.M.4
-00001600: d7b6 6fc2 08f0 ac6d 114b c0ee 74f2 df73  ..o....m.K..t..s
-00001610: 6423 63cb 2a05 5266 170b f39d 4fe7 f2e9  d#c.*.Rf....O...
-00001620: 5862 fce2 294d ac3d cd79 ccb2 898d 1ccf  Xb..)M.=.y......
-00001630: b668 16b1 659c ad27 f6a7 8ff3 cec0 b6b8  .h..e..'........
-00001640: 20d9 9224 2ca3 13fb 9972 fbc5 f4e7 9fc6   ..$,....r......
-00001650: 0796 3ff2 0da5 c202 868c 4fec 8d10 db91  ..?.......O.....
-00001660: ebf2 6843 53c2 1db6 a519 7cb3 6279 4a04  ..hCS.....|.byJ.
-00001670: 7ccc d72e dfe6 942c 0ba3 3471 b1e7 f5dc  |......,..4q....
-00001680: 94c4 995d 328c f24b 38d8 6a15 4774 c6a2  ...]2..K8.j.Gt..
-00001690: 5d4a 3351 92e4 3421 02fc e79b 78cb 155b  ]J3Q..4!....x..[
-000016a0: 1a5d 4297 92fc 71b7 ed44 2cdd 02c5 224e  .]B...q..D,..."N
-000016b0: 62f1 5c90 da56 1a8d 1ed6 19cb c922 81b8  b.\..V......."..
-000016c0: 9f50 4022 eb29 873f 0cff be9a a6b8 df9a  .P@".).?........
-000016d0: 298d a39c 71b6 120e 30bb a5cf edf0 87ee  )...q...0.......
-000016e0: d025 51c5 d48e ff22 1a14 b839 ddc7 b280  .%Q...."...9....
-000016f0: 272a 7c9b 4ba8 5b71 e113 997f 2359 af22  '*|.K.[q....#Y."
-00001700: 93e9 ca47 bb78 39b1 fff1 8eaf 0e5c 917c  ...G.x9......\.|
-00001710: f33a 1e92 6fb5 d737 7b3a 5ec6 5061 1995  .:..o..7{:^.Pa..
-00001720: 95d3 d5c4 0ed1 28fc 05d9 ee74 5c08 e873  ......(....t\..s
-00001730: 4c0f bc36 b604 597c a009 8d04 8549 906d  L..6..Y|.....I.m
-00001740: 497d 2e18 7b94 c007 b8e5 0125 2f00 9292  I}..{......%/...
-00001750: 4422 ded3 3b9a 24c0 0ca1 f2af e524 584e  D"..;.$......$XN
-00001760: e056 33d4 c76a b679 a1e8 77b9 b520 9cde  .V3..j.y..w.. ..
-00001770: b1e4 4bbc 141b 9812 56ce 92ae c82e 11a7  ..K.....V.......
-00001780: 9b03 67e0 63cf 47b8 5b7d f99e 1d5e d178  ..g.c.G.[}...^.x
-00001790: bd11 6002 77d9 4e24 7146 5fd3 3d4d c0ae  ..`.w.N$qF_.=M..
-000017a0: 70bd d0d4 68f9 3ca3 3c02 9183 ef4e e157  p...h.<.<....N.W
-000017b0: c412 7002 dead 3496 8b15 344a 9eca 608f  ..p...4...4J..`.
-000017c0: 3ec0 628d 765c b054 3925 c3a9 0c20 cec2  >.b.v\.T9%... ..
-000017d0: 00ae 87a3 0178 70c6 00ca 5618 0495 0146  .....xp...V....F
-000017e0: 0eea 055e 4f06 a419 3642 915e d5a7 0678  ...^O...6B.^...x
-000017f0: c104 d7e3 d467 98ea 86bd a321 5c95 2124  .....g.....!\.!$
-00001800: fa9a a9fb 4706 b81e 1982 6ead 2cd7 5041  ....G.....n.,.PA
-00001810: 7a8b 2886 e712 7836 0f52 2565 d160 f0a3  z.(...x6.R%e.`..
-00001820: eea0 4a01 52ef 1755 1429 0dc8 8132 6927  ..J.R..U.)...2i'
-00001830: b45e 01a4 5420 07ca 64e8 f895 b0af c920  .^..T ..d...... 
-00001840: 0229 95f1 9f34 7573 39e4 fa29 c96a b2fa  .)...4us9..).j..
-00001850: 8f60 949e d049 50e8 e660 94b4 d0ff a02d  .`...IP..`.....-
-00001860: a4c4 2507 ff2e f546 6540 8765 fc35 41de  ..%....Fe@.e.5A.
-00001870: 1a0c 56ca 9483 1f55 2656 ca94 83cb 82c1  ..V....U&V......
-00001880: 5577 3a29 53ba 728d bab0 92aa 1c5c 1043  Uw:)S.r......\.C
-00001890: a339 2a65 e25a b7bb 767e 2548 d91e af9d  .9*e.Z..v~%H....
-000018a0: 5f29 13df deea b012 a41c 5c3b bfd2 1fae  _)........\;....
-000018b0: e9ef d646 8995 32e5 e0b2 fafb 4a7f 72a0  ...F..2.....J.r.
-000018c0: da0c 94e2 dce3 49a9 cc3f dbff ce36 645f  ......I..?...6d_
-000018d0: c94e 0eae 4c99 afe4 2607 cae5 8163 7ca6  .N..L...&....c|.
-000018e0: bae5 c3bb d859 cc88 20d3 71ce 0e16 6cf9  .....Y.. .q...l.
-000018f0: c075 be25 7203 8d46 92c7 f8f0 8787 b8c4  .u.%r..F........
-00001900: 8612 5c98 c0a6 80c3 8666 3ff5 c6ee 1e76  ..\......f?....v
-00001910: 29d1 11f1 b28d 404d c45d 1be1 6b90 9901  ).....@M.]..k...
-00001920: 829b 2cf7 6d88 8698 1b48 9a1c b09b d3a3  ..,.m....H......
-00001930: 099a 8857 6d44 b789 7868 237a 4dc4 af6d  ...WmD..xh#zM..m
-00001940: 44bf 89f8 ad8d 1834 11af db88 6113 f1c6  D......4....a...
-00001950: 9077 ad34 bf1b 205a e2df 1a20 5a5a df19  .w.4.. Z... ZZ..
-00001960: 12af b1fc 6180 682c ef0d 10bf 19d1 0703  ....a.h,........
-00001970: 442b cf47 0344 abcf 2703 442b d067 0344  D+.G.D..'.D+.g.D
-00001980: cbee 9736 c4d7 b2fb a781 45ab f35f 0688  ...6......E.._..
-00001990: 56e8 bf0d 05d0 f212 1a16 21d2 1213 9a96  V.........!.....
-000019a0: a196 99d0 b010 9196 9ad0 b012 9116 5568  ..............Uh
-000019b0: 588a 480b 2b34 2c46 a4e5 581e aef4 e588  X.H.+4,F..X.....
-000019c0: 4f49 76a1 5da9 d350 d9bf c84e b079 9c08  OIv.]..P...N.y..
-000019d0: 9a37 0e68 a783 5e10 04e1 a08b c28e 1ff6  .7.h..^.........
-000019e0: ee3a c341 f0b2 1306 c8eb 0cfb c8ef df07  .:.A............
-000019f0: b339 beef 7d93 a784 2d59 d337 245f c719  .9..}...-Y.7$_..
-00001a00: b712 ba2a 0e3c 7de8 a279 794c f21c f941  ...*.<}..yyL...A
-00001a10: b06d d1f9 164c c0f9 a618 6ee0 d704 0a6d  .m...L....n....m
-00001a20: d193 2d77 c518 b852 7e90 67b8 eaf7 89e9  ..-w...R~.g.....
-00001a30: 7700 0000 ffff 0300 504b 0304 1400 0600  w.......PK......
-00001a40: 0800 0000 2100 83fd 7ca1 6501 0000 2f04  ....!...|.e.../.
-00001a50: 0000 1400 0000 786c 2f73 6861 7265 6453  ......xl/sharedS
-00001a60: 7472 696e 6773 2e78 6d6c 7c93 5b4f 0231  trings.xml|.[O.1
-00001a70: 1085 df4d fc0f 4ddf 75b9 24c6 98dd 2504  ...M..M.u.$...%.
-00001a80: 31f2 20a2 82ef 753b 4013 daae 9da9 817f  1. ...u;@.......
-00001a90: 6fb9 262e 238f 7bbe cce9 d9b9 e4bd b55d  o.&.#.{........]
-00001aa0: 891f 0868 bc2b 64fb b625 05b8 ca6b e316  ...h.+d..%...k..
-00001ab0: 859c 4d9f 6eee a540 524e ab95 7750 c80d  ..M.n..@RN..wP..
-00001ac0: a0ec 95d7 5739 2289 54eb b090 4ba2 fa21  ....W9".T...K..!
-00001ad0: cbb0 5a82 5578 eb6b 7089 cc7d b08a d267  ..Z.Ux.kp..}...g
-00001ae0: 5864 5807 501a 9700 6457 59a7 d5ba cbac  XdX.P...dWY.....
-00001af0: 324e 8aca 4747 85ec 76a5 88ce 7c47 189c  2N..GG..v...|G..
-00001b00: 8432 4753 e654 be43 92d3 63a3 c73c a332  .2GS.T.C..c..<.2
-00001b10: cfb6 ea5f 32dd d4d0 64c3 75ed 0381 167d  ..._2...d.u....}
-00001b20: 6aa2 1181 65dc 76f2 58d9 33ab 1de0 ded8  j...e.v.X.3.....
-00001b30: 8199 3324 5ee7 c282 c218 f8e2 97c9 980d  ..3$^...........
-00001b40: 3181 60bc 6ea2 b7a8 1c19 da34 f541 44f2  1.`.n......4.AD.
-00001b50: 1602 93fd 84b8 fc27 385c 1304 a756 8cc1  .......'8\...V..
-00001b60: 2478 1d2b aec9 47c2 39f7 1181 abd9 eb17  $x.+..G.9.......
-00001b70: 9e9b 06e5 5055 9496 4e70 9d7d 8e5f 4cc8  ....PU..Np.}._L.
-00001b80: adca c538 6ec8 0729 8ad8 6cdb d4a4 96b5  ...8n..)..l.....
-00001b90: 19bb 03e0 1c0f e8d2 1f6c 5d3b ffb9 76d8  .........l];..v.
-00001ba0: 9c3b d78e b8e0 fa09 4e7b 6ec0 07c0 654d  .;......N{n...eM
-00001bb0: 03fa 313a a5e1 c7ba 67ec 5ea4 9be4 2f64  ..1:....g.^.../d
-00001bc0: 56eb 3392 a583 2f7f 0100 00ff ff03 0050  V.3.../........P
-00001bd0: 4b03 0414 0006 0008 0000 0021 003f 1004  K..........!.?..
-00001be0: 2b55 0100 006e 0200 0011 0008 0164 6f63  +U...n.......doc
-00001bf0: 5072 6f70 732f 636f 7265 2e78 6d6c 20a2  Props/core.xml .
-00001c00: 0401 28a0 0001 0000 0000 0000 0000 0000  ..(.............
-00001c10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ca0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001cb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001cc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001cd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000008f0: 4b03 0414 0006 0008 0000 0021 0091 d238  K..........!...8
+00000900: c2dd 0200 00b7 0600 000f 0000 0078 6c2f  .............xl/
+00000910: 776f 726b 626f 6f6b 2e78 6d6c a455 df6f  workbook.xml.U.o
+00000920: da30 107e 9fb4 ff21 b378 0d8e f991 a288  .0.~...!.x......
+00000930: 5075 a568 48dd 84d6 b57d 44c6 31c4 aa63  Pu.hH....}D.1..c
+00000940: 67b6 2954 55ff f79d 1342 a1bc 746d 0476  g.)TU....B..tm.v
+00000950: 2ee7 7cfe eeee 3b67 78be 2d64 f0c8 8d15  ..|...;gx.-d....
+00000960: 5aa5 88b4 2314 70c5 7426 d42a 45b7 7f26  Z...#.p.t&.*E..&
+00000970: e100 05d6 5195 51a9 154f d113 b7e8 7cf4  ....Q.Q..O....|.
+00000980: f5cb 70a3 cdc3 42eb 8700 0094 4d51 ee5c  ..p...B.....MQ.\
+00000990: 9960 6c59 ce0b 6adb bae4 0a3c 4b6d 0aea  .`lY..j....<Km..
+000009a0: c034 2b6c 4bc3 6966 73ce 5d21 7127 8a62  .4+lK.ifs.]!q'.b
+000009b0: 5c50 a150 8d90 98f7 60e8 e552 303e d66c  \P.P....`..R0>.l
+000009c0: 5d70 e56a 10c3 2575 40df e6a2 b40d 5ac1  ]p.j..%u@.....Z.
+000009d0: de03 5750 f3b0 2e43 a68b 1220 1642 0af7  ..WP...C... .B..
+000009e0: 5481 a2a0 60c9 74a5 b4a1 0b09 616f 493f  T...`.t.....aoI?
+000009f0: d81a f8c5 f027 110c 9d66 2770 9d6c 5508  .....'...f'p.lU.
+00000a00: 66b4 d54b d706 685c 933e 899f 4498 90a3  f..K..h\.>..D...
+00000a10: 146c 4f73 f03e a41e 36fc 51f8 1aee 5999  .lOs.>..6.Q...Y.
+00000a20: f883 ace2 3d56 fc0a 46a2 4fa3 1190 56a5  ....=V..F.O...V.
+00000a30: 9504 92f7 41b4 fe9e 5b07 8d86 4b21 f95d  ....A...[...K!.]
+00000a40: 2ddd 8096 e52f 5af8 4a49 1448 6add 5526  -..../Z.JI.Hj.U&
+00000a50: 1ccf 5274 06a6 def0 a307 665d 7e5f 0b09  ..Rt......f]~_..
+00000a60: 5e42 3a9d 08e1 d15e ce33 0306 d4fe 423a  ^B:....^.3....B:
+00000a70: 6e14 75fc 522b 0752 db51 ffac ac2a eccb  n.u.R+.R.Q...*..
+00000a80: 5c83 8883 dffc ef5a 180e bd03 1282 7060  \......Z......p`
+00000a90: a42c a10b 3ba3 2e0f d646 a608 df5a 880f  .,..;....F...Z..
+00000aa0: 3462 18c1 8dea 2d06 4e8a 3387 593d 874c  4b....-.N.3.Y=.L
+00000ab0: 0acc 1473 7e36 bcd4 c6d9 bdaf b19b 590a  ...s~6........Y.
+00000ac0: eba0 b9e7 7ec6 071a a6a7 0df3 1f2a a6cc  ....~........*..
+00000ad0: 2711 43e2 eae0 eafb b749 8418 4dd2 2875  '.C......I..M.(u
+00000ae0: e64c 00f7 d3f1 3554 eb86 3e42 ed40 21d9  .L....5T..>B.@!.
+00000af0: aeb5 a7be 38dd b962 2621 f3e7 cbab 2ef9  ....8..b&!......
+00000b00: de19 8cc3 c9c5 d538 8ce3 1e09 07f1 a417  .......8........
+00000b10: 8ec1 ecc6 dd98 c483 b317 08c6 c409 d374  ...............t
+00000b20: edf2 9d2c 3c74 8a7a 5ec8 6f5d 3fe9 b6f1  ...,<t.z^.o]?...
+00000b30: 9028 598b ec95 c673 b4bb 423f bf19 1adf  .(Y....s..B?....
+00000b40: 8b0f d81f 8077 826f ecab 80bc 196c ef85  .....w.o.....l..
+00000b50: caf4 2645 ddc1 590f a27a 6aec 7e04 d6a6  ..&E..Y..zj.~...
+00000b60: 72de 8bcc e5b0 a23f f02b ea67 3fb8 58e5  r......?.+.g?.X.
+00000b70: c0b8 1311 bf10 1ac5 334b d111 a371 cd68  ........3K...q.h
+00000b80: 0257 e887 2346 f880 5275 d402 b56a 0e54  .W..#F..Ru...j.T
+00000b90: d51e 63ea 289c e8fe 10f6 2986 53cc 247e  ..c.(.....).S.$~
+00000ba0: 0733 cd48 55c2 e6a5 8c2f 85e2 996f 2a80  .3.HU..../...o*.
+00000bb0: 38b0 7640 f3ad 5445 7b3e 11be 513c ea82  8.v@..TE{>..Q<..
+00000bc0: 5aee 7b8d 5179 d3c0 430c b9c8 32ee 3f2d  Z.{.Qy..C...2.?-
+00000bd0: 68e4 577d 6b5d b448 d2ba 6e91 213e 0005  h.W}k].H..n.!>..
+00000be0: bd1c 6f08 286c 6602 3f79 9e55 8fe2 e69b  ..o.(lf.?y.U....
+00000bf0: 33fa 0700 00ff ff03 0050 4b03 0414 0006  3........PK.....
+00000c00: 0008 0000 0021 00e4 ac15 93eb 0200 001f  .....!..........
+00000c10: 0700 000d 0000 0078 6c2f 7374 796c 6573  .......xl/styles
+00000c20: 2e78 6d6c a455 db8e 9b30 107d afd4 7fb0  .xml.U...0.}....
+00000c30: fc4e b804 4888 4256 4db2 482b 6dab 4abb  .N..H.BVM.H+m.J.
+00000c40: 95fa ea80 49ac f505 1927 25ad faef 1d03  ....I....'%.....
+00000c50: 21ac b66a b7db bcd8 1ec6 67ce cc19 4f96  !..j......g...O.
+00000c60: 378d e0e8 4475 cd94 4cb1 3ff1 30a2 3257  7...Du..L.?.0.2W
+00000c70: 0593 fb14 7f79 cc9c 3946 b521 b220 5c49  .....y..9F.!. \I
+00000c80: 9ae2 33ad f1cd eafd bb65 6dce 9c3e 1c28  ..3......em..>.(
+00000c90: 3508 2064 9de2 8331 d5c2 75eb fc40 05a9  5. d...1..u..@..
+00000ca0: 27aa a212 be94 4a0b 62e0 a8f7 6e5d 694a  '.....J.b...n]iJ
+00000cb0: 8ada 5e12 dc0d 3c2f 7605 6112 7708 0b91  ..^...</v.a.w...
+00000cc0: bf06 4410 fd74 ac9c 5c89 8a18 b663 9c99  ..D..t..\....c..
+00000cd0: 738b 8591 c817 777b a934 d971 a0da f821  s.....w{.4.q...!
+00000ce0: c951 e3c7 3a40 8dbe 0469 ad2f e208 966b  .Q..:@...i./...k
+00000cf0: 55ab d24c 00d7 5565 c972 fa92 6ee2 262e  U..L..Ue.r..n.&.
+00000d00: c9af 4880 fc36 243f 72bd e059 ee8d 7e23  ..H..6$?r..Y..~#
+00000d10: 52e8 6a7a 6256 3ebc 5a96 4a9a 1ae5 ea28  R.jzbV>.Z.J....(
+00000d20: 0d88 0944 6d09 164f 527d 9399 fd64 8d9d  ...Dm..OR}...d..
+00000d30: d76a 597f 4727 c2c1 e263 77b5 cc15 571a  .jY.G'...cw...W.
+00000d40: 1990 0e2a d75a 2411 b4f3 d810 ce76 9a59  ...*.Z$......v.Y
+00000d50: b792 08c6 cf9d 39b0 8656 edde 4f30 a8bd  ......9..V..O0..
+00000d60: 35ba 9647 bfd4 7089 713e b09a 5a02 6058  5..G..p.q>..Z.`X
+00000d70: 2d41 3e43 b5cc e080 fafd e3b9 82f0 123a  -A>C...........:
+00000d80: ad83 69fd fee2 bdd7 e4ec 07d1 eb2f d48a  ..i........../..
+00000d90: b3c2 b2d8 6fc6 4943 e71b 66eb e678 9320  ....o.IC..f..x. 
+00000da0: 4c92 d9cc b7bf d93c 995a ec5d efcd 6441  L......<.Z.]..dA
+00000db0: 1b5a a438 0edb 90a3 2c6c c62d e376 81c4  .Z.8....,l.-.v..
+00000dc0: 774a 17f0 b4ae 825c 4cab 25a7 a501 54cd  wJ.....\L.%...T.
+00000dd0: f607 bb1a 55d9 18ca 1868 bfd5 b260 64af  ....U....h...`d.
+00000de0: 24e1 b696 1dc8 b001 d89c 72fe 609f dfd7  $.........r.`...
+00000df0: f219 7653 2279 1499 3077 400f d2b1 2a5c  ..vS"y..0w@...*\
+00000e00: b6c0 abdf 7678 ddc1 e28f d13a ec11 6c00  ....vx.....:..l.
+00000e10: 75fa 7758 d494 03fe 2b6e 0718 8d49 0db7  u.wX....+n...I..
+00000e20: 11a9 2a7e b6fd d1b7 64cb 15d8 8d4a f0ac  ..*~....d....J..
+00000e30: 0043 2ac8 366f 8a3f d9d9 c3e1 19f4 74d0  .C*.6o.?......t.
+00000e40: eec8 3888 fc9b e401 b368 aee5 f4ac b6c6  ..8......h......
+00000e50: ce91 b6d0 4314 a86a 414b 72e4 e671 f898  ....C..jAKr..q..
+00000e60: e2eb fe23 2dd8 5124 83d7 6776 52a6 8548  ...#-.Q$..gvR..H
+00000e70: f175 7f6f 55f7 631b 8336 e6be 86b7 022b  .u.oU.c..6.....+
+00000e80: 3a6a 96e2 1fb7 eb59 b2bd cd02 67ee ade7  :j.....Y....g...
+00000e90: 4e38 a591 9344 ebad 1385 9bf5 769b 255e  N8...D......v.%^
+00000ea0: e06d 7e8e a6d9 7fcc b276 f882 c07e b8a8  .m~......v...~..
+00000eb0: 394c 3cdd 27db a7f8 70b5 a578 74e8 e8b7  9L<.'...p..xt...
+00000ec0: dd0f b4c7 dc93 20f6 3e44 bee7 6453 cf77  ...... .>D..dS.w
+00000ed0: c298 cc9d 793c 8d9c 2cf2 836d 1cae 6fa3  ....y<..,..m..o.
+00000ee0: 2c1a 718f de38 f33c d7f7 bbe9 69c9 470b  ,.q..8.<....i.G.
+00000ef0: c304 e54c 5eb4 ba28 34b6 8248 70fc 4312  ...L^..(4..Hp.C.
+00000f00: ee45 09f7 facf b6fa 0500 00ff ff03 0050  .E.............P
+00000f10: 4b03 0414 0006 0008 0000 0021 00e9 a625  K..........!...%
+00000f20: b866 0600 0053 1b00 0013 0000 0078 6c2f  .f...S.......xl/
+00000f30: 7468 656d 652f 7468 656d 6531 2e78 6d6c  theme/theme1.xml
+00000f40: ec59 cd6e 1b37 10be 17e8 3b10 7b4f 2cd9  .Y.n.7....;.{O,.
+00000f50: 9262 1991 034b 96e2 3671 62d8 4a8a 1ca9  .b...K..6qb.J...
+00000f60: 5d6a 9711 77b9 2029 3bba 15c9 b140 81a2  ]j..w. );....@..
+00000f70: 69d1 4b81 de7a 28da 0648 805e d2a7 719b  i.K..z(..H.^..q.
+00000f80: a24d 81bc 4287 e44a 5a5a 546c 2706 fa17  .M..B..JZZTl'...
+00000f90: 1d6c 2df7 e3fc cf70 86ba 7aed 41ca d021  .l-....p..z.A..!
+00000fa0: 1192 f2ac 1554 2f57 0244 b290 4734 8b5b  .....T/W.D..G4.[
+00000fb0: c19d 7eef d27a 80a4 c259 8419 cf48 2b98  ..~..z...Y...H+.
+00000fc0: 1019 5cdb 7cff bdab 7843 2524 2508 f667  ..\.|...xC%$%..g
+00000fd0: 7203 b782 44a9 7c63 6545 86b0 8ce5 659e  r...D.|ceE....e.
+00000fe0: 930c de0d b948 b182 4711 af44 021f 01dd  .....H..G..D....
+00000ff0: 94ad ac56 2a8d 9514 d32c 4019 4e81 eced  ...V*....,@.N...
+00001000: e190 8604 f535 c960 734a bccb e031 5352  .....5.`sJ...1SR
+00001010: 2f84 4c1c 68d2 c4d9 61b0 d1a8 aa11 7222  /.L.h...a.....r"
+00001020: 3b4c a043 cc5a 01f0 89f8 519f 3c50 0162  ;L.C.Z....Q.<P.b
+00001030: 582a 78d1 0a2a e613 ac6c 5e5d c11b c526  X*x..*...l^]...&
+00001040: a696 ec2d edeb 994f b1af d810 8d56 0d4f  ...-...O.....V.O
+00001050: 110f 664c abbd 5af3 caf6 8cbe 0130 b588  ..fL..Z......0..
+00001060: eb76 bb9d 6e75 46cf 0070 1882 a656 9632  .v..nuF..p...V.2
+00001070: cd5a 6fbd da9e d22c 81ec d745 da9d 4abd  .Zo....,...E..J.
+00001080: 5273 f125 fa6b 0b32 37db ed76 bd59 c862  Rs.%.k.27..v.Y.b
+00001090: 891a 90fd 5a5b c0af 571a b5ad 5507 6f40  ....Z[..W...U.o@
+000010a0: 165f 5fc0 d7da 5b9d 4ec3 c11b 90c5 3716  .__...[.N.....7.
+000010b0: f0bd 2bcd 46cd c51b 50c2 6836 5a40 6b87  ..+.F...P.h6Z@k.
+000010c0: f67a 05f5 1964 c8d9 8e17 be0e f0f5 4a01  .z...d........J.
+000010d0: 9fa3 201a 66d1 a559 0c79 a696 c55a 8aef  .. .f..Y.y...Z..
+000010e0: 73d1 0380 0632 ac68 86d4 2427 431c 4214  s....2.h..$'C.B.
+000010f0: 7770 3a10 146b 0678 83e0 d21b bb14 ca85  wp:..k.x........
+00001100: 25cd 0bc9 50d0 5cb5 820f 730c 1931 a7f7  %...P.\...s..1..
+00001110: eaf9 f7af 9e3f 45af 9e3f 397e f8ec f8e1  .....?E..?9~....
+00001120: 4fc7 8f1e 1d3f fcd1 d272 36ee e02c 2e6f  O....?...r6..,.o
+00001130: 7cf9 ed67 7f7e fd31 fae3 e937 2f1f 7fe1  |..g.~.1...7/...
+00001140: c7cb 32fe d71f 3ef9 e5e7 cffd 40c8 a0b9  ..2...>.....@...
+00001150: 442f be7c f2db b327 2fbe faf4 f7ef 1e7b  D/.|...'/......{
+00001160: e05b 020f caf0 3e4d 8944 b7c8 11da e729  .[....>M.D.....)
+00001170: e866 0ce3 4a4e 06e2 7c3b fa09 a6ce 0e9c  .f..JN..|;......
+00001180: 006d 0fe9 ae4a 1ce0 ad09 663e 5c9b b8c6  .m...J....f>\...
+00001190: bb2b a078 f880 d7c7 f71d 590f 1231 56d4  .+.x......Y..1V.
+000011a0: c3f9 4692 3ac0 5dce 599b 0baf 016e 685e  ..F.:.].Y....nh^
+000011b0: 250b f7c7 59ec 672e c665 dc3e c687 3ede  %...Y.g..e.>..>.
+000011c0: 1d9c 39ae ed8e 73a8 9ad3 a074 6cdf 4988  ..9...s....tl.I.
+000011d0: 23e6 1ec3 99c2 31c9 8842 fa1d 1f11 e2d1  #.....1..B......
+000011e0: ee1e a58e 5d77 6928 b8e4 4385 ee51 d4c6  ....]wi(..C..Q..
+000011f0: d46b 923e 1d38 8134 dfb4 4353 f0cb c4a7  .k.>.8.4..CS....
+00001200: 33b8 dab1 cdee 5dd4 e6cc a7f5 3639 7491  3.....].....69t.
+00001210: 9010 9879 84ef 13e6 98f1 3a1e 2b9c fa48  ...y......:.+..H
+00001220: f671 caca 06bf 8955 e213 f260 22c2 32ae  .q.....U...`".2.
+00001230: 2b15 783a 268c a36e 44a4 f4ed b92d 40df  +.x:&..nD....-@.
+00001240: 92d3 6f60 a857 5eb7 efb2 49ea 2285 a223  ..o`.W^...I."..#
+00001250: 1fcd 9b98 f332 729b 8f3a 094e 73af cc34  .....2r..:.Ns..4
+00001260: 4bca d80f e408 4214 a33d ae7c f05d ee66  K.....B..=.|.].f
+00001270: 887e 063f e06c a9bb ef52 e2b8 fbf4 4270  .~.?.l...R....Bp
+00001280: 87c6 8e48 f300 d16f c6a2 a8da 4efd 4d69  ...H...o....N.Mi
+00001290: f6ba 62cc 2854 e377 c578 7a3a 6dc1 d1e4  ..b.(T.w.xz:m...
+000012a0: 4b89 9d13 2578 19ee 5f58 78b7 f138 db23  K...%x.._Xx..8.#
+000012b0: 10eb 8b07 cfbb bafb aeee 06ff f9ba bb2c  ...............,
+000012c0: 97cf 5a6d e705 169a e479 5f6c bae4 7469  ..Zm.....y_l..ti
+000012d0: 933c a48c 1da8 0923 37a5 e993 251c 1651  .<.....#7...%..Q
+000012e0: 0f16 4d03 6fa6 b8d9 d094 27f0 b528 ee0e  ..M.o.....'..(..
+000012f0: 2e16 d8ec 4182 ab8f a84a 0e12 9c43 8f5d  ....A....J...C.]
+00001300: 3523 5f2c 0bd2 b144 3997 30db 9965 337c  5#_,...D9.0..e3|
+00001310: 9213 b4cd 3849 a1cd 3693 615d cf0c b61e  ....8I..6.a]....
+00001320: 48ac 7679 6497 d7ca b3e1 8c8c 9914 6333  H.vyd.........c3
+00001330: 7f4e 19ad 6902 6765 b676 e5ed 9855 ad54  .N..i.ge.v...U.T
+00001340: 4bcd e6aa 5635 a299 52e7 a836 5319 7cb8  K...V5..R..6S.|.
+00001350: a81a 2cce ac09 5d08 82de 05ac dc80 115d  ..,...]........]
+00001360: cb0e b309 6624 d276 b773 f3d4 2d9a f585  ....f$.v.s..-...
+00001370: ba48 2638 2285 8fb4 de8b 3eaa 1a27 4d63  .H&8".....>..'Mc
+00001380: 651a 461e 1fe9 39ef 141f 95b8 3535 d9b7  e.F...9.....55..
+00001390: e076 1627 95d9 d596 b09b 7aef 6dbc 341d  .v.'......z.m.4.
+000013a0: 6ee7 5ed2 797b 221d 5956 4e4e 96a1 a356  n.^.y{".YVNN...V
+000013b0: d0ac afd6 0314 e2bc 150c 61ac 85af 690e  ..........a...i.
+000013c0: 5e97 baf1 c32c 86bb a150 091b f6a7 26b3  ^....,...P....&.
+000013d0: 09d7 b937 9bfe b0ac c24d 85b5 fb82 c24e  ...7.....M.....N
+000013e0: 1dc8 8554 db58 2636 34cc ab22 0458 6686  ...T.X&64..".Xf.
+000013f0: 7023 ff6a 1dcc 7a51 0ad8 487f 0329 d6d6  p#.j..zQ..H..)..
+00001400: 2118 fe36 29c0 8eae 6bc9 7048 4255 7676  !..6)...k.pHBUvv
+00001410: 69c5 dc51 1840 514a f958 1171 9044 4768  i..Q.@QJ.X.q.DGh
+00001420: c0c6 621f 83fb 75a8 823e 1195 703b 612a  ..b...u..>..p;a*
+00001430: 827e 80ab 346d 6df3 ca2d ce45 d295 2fb0  .~..4mm..-.E../.
+00001440: 0cce ae63 9627 b828 b73a 45a7 996c e126  ...c.'.(.:E..l.&
+00001450: 8f67 3298 272b ad11 0f74 f3ca 6e94 3bbf  .g2.'+...t..n.;.
+00001460: 2a26 e52f 4895 7218 ffcf 54d1 e709 5c17  *&./H.r...T...\.
+00001470: ac45 da03 21dc e40a 8c74 beb6 022e 54c2  .E..!....t....T.
+00001480: a10a e509 0d7b 022e b94c ed80 6881 eb58  .....{...L..h..X
+00001490: 780d 4105 f7c9 e6bf 2087 fabf cd39 4bc3  x.A..... ....9K.
+000014a0: a435 4c7d 6a9f c648 5038 8f54 2208 d983  .5L}j..HP8.T"...
+000014b0: b264 a2ef 1462 d5e2 ecb2 2459 41c8 4454  .d...b....$YA.DT
+000014c0: 495c 995b b107 e490 b0be ae81 0d7d b607  I\.[.........}..
+000014d0: 2881 5037 d5a4 2803 0677 32fe dce7 2283  (.P7..(..w2...".
+000014e0: 06b1 6e72 fea9 9d8f 4de6 f3b6 07ba 3bb0  ..nr....M.....;.
+000014f0: 2d96 dd7f c65e a456 2afa a5a3 a0e9 3dfb  -....^.V*.....=.
+00001500: 4c4f 352b 07af 39d8 cf79 d4da 8ab5 a0f1  LO5+..9..y......
+00001510: 6afd cc47 6d0e 973e 48ff 81f3 8f8a 90d9  j..Gm..>H.......
+00001520: 1f27 f481 dae7 fb50 5b11 fcd6 60db 2b04  .'.....P[...`.+.
+00001530: 517d c936 1e48 1748 5b1e 07d0 38d9 451b  Q}.6.H.H[...8.E.
+00001540: 4c9a 946d 588a eef6 c2db 28b8 912e 3add  L..mX.....(...:.
+00001550: 195f c8d2 37e9 74cf 69ec 5973 e6b2 7372  ._..7.t.i.Ys..sr
+00001560: f1f5 dde7 f98c 5d58 d8b1 75b9 d3f5 981a  ......]X..u.....
+00001570: 92f6 648a eaf6 683a c818 c798 5fb5 ca3f  ..d...h:...._..?
+00001580: 3cf1 c17d 70f4 365c f18f 9992 f66a ff01  <..}p.6\.....j..
+00001590: 5cf1 c194 617f 2480 e4b7 ce35 5b37 ff02  \...a.$....5[7..
+000015a0: 0000 ffff 0300 504b 0304 1400 0600 0800  ......PK........
+000015b0: 0000 2100 92e6 ccb8 1e03 0000 e808 0000  ..!.............
+000015c0: 1800 0000 786c 2f77 6f72 6b73 6865 6574  ....xl/worksheet
+000015d0: 732f 7368 6565 7431 2e78 6d6c 9c56 6b6f  s/sheet1.xml.Vko
+000015e0: da30 14fd 3e69 ff21 caf7 3c1c 4278 08a8  .0..>i.!..<.Bx..
+000015f0: 2894 b55b 274d 7b7e 368e 0356 9338 b3cd  (..['M{~6..V.8..
+00001600: a39a fadf 77ed 3c20 4d55 d122 889d e49c  ....w.< MU."....
+00001610: 73cf 8daf 2f99 5c1d b3d4 da53 2119 cfa7  s.../.\....S!...
+00001620: 3672 7ddb a239 e131 cb37 53fb d7cf 9533  6r}..9.1.7S....3
+00001630: b42d a970 1ee3 94e7 746a 3f52 695f cd3e  .-.p....tj?Ri_.>
+00001640: 7e98 1cb8 7890 5b4a 9505 0ab9 9cda 5ba5  ~...x.[J......[.
+00001650: 8ab1 e749 b2a5 1996 2e2f 680e 7712 2e32  ...I...../h.w..2
+00001660: ace0 546c 3c59 088a 6343 ca52 2ff0 fdc8  ..Tl<Y..cC.R/...
+00001670: cb30 cbed 5261 2c2e d1e0 49c2 085d 72b2  .0..Ra,...I..]r.
+00001680: cb68 ae4a 1141 53ac c0bf dcb2 42d6 6a19  .h.J.AS.....B.j.
+00001690: b944 2ec3 e261 5738 8467 0548 ac59 cad4  .D...aW8.g.H.Y..
+000016a0: a311 b5ad 8c8c ef36 3917 789d 42de 4714  .......69.x.B.G.
+000016b0: 6262 1d05 7c03 f8f5 ea30 e67a 2752 c688  bb..|....0.z'R..
+000016c0: e092 27ca 0565 aff4 dc4d 7fe4 8d3c 4c1a  ..'..e...M...<L.
+000016d0: a56e fe17 c9a0 d013 74cf f402 9ea4 82f7  .n......t.......
+000016e0: 5942 fd46 2b38 89f5 de29 1635 62fa 7189  YB.F+8...).5b.q.
+000016f0: f18e c553 fb9f 5f7d 1c18 913e f88e 8ff4  ...S.._}...>....
+00001700: e1ec f364 cf26 3183 15d6 5959 8226 537b  ...d.&1...YY.&S{
+00001710: 8ec6 f7c8 f666 1353 3fbf 193d c8b3 b9a5  .....f.S?..=....
+00001720: f0fa 074d 2951 1462 20db d2e5 b9e6 fc41  ...M)Q.b ......A
+00001730: 03ef e092 0f8a d200 b422 268a ede9 82a6  ........."&.....
+00001740: 2908 43a6 f26f 1923 d001 bc26 c2f9 bc8e  ).C..o.#...&....
+00001750: b632 05fd 4d58 6b2c e982 a77f 58ac b610  .2..MXk,....X...
+00001760: 1236 4e4c 13bc 4bd5 e9e2 d01d f602 bf87  .6NL..K.........
+00001770: 827e 73f3 3b3f dc52 b6d9 2aa0 c055 be53  .~s.;?.R..*..U.S
+00001780: 29cb e93d ddd3 1478 c6ba 29a9 71fc b8a4  )..=...x..).q...
+00001790: 9240 8d83 77d7 f822 3c05 1370 b432 a6f7  .@..w.."<..p.2..
+000017a0: 2a94 283e 96c9 961e 82f0 2c1e d949 c5b3  *.(>......,..I..
+000017b0: da9d ceab 6142 c286 09e3 a172 0f56 5e21  ....aB.....r.V^!
+000017c0: c0f2 1942 d810 02e4 a228 f423 9dd9 3362  ...B.....(.#..3b
+000017d0: 2b27 6def 3c34 c08d 128c 55e8 5794 ce89  +'m.<4....U.W...
+000017e0: 5145 84b1 265e 98ed a062 c258 3361 adde  QE..&^...b.X3a..
+000017f0: 621a 5aa0 310d 63a5 10f6 2f7b d2a3 8a09  b.Z.1.c.../{....
+00001800: e33b 63eb ba2a 9719 266f 8c8e 9a12 d11b  .;c..*..&o......
+00001810: a2aa 9137 e68e ea62 d193 cbe2 7b65 a19a  ...7...b....{e..
+00001820: 5db4 c40a cf26 821f 2ce8 6ee0 4216 58ff  ]....&..,.n.B.X.
+00001830: 57a0 b196 7bb1 d0a1 4e35 76ae c186 021b  W...{...N5v.....
+00001840: 40c2 e6dd cf46 136f 0f3b 9254 88eb 2e02  @....F.o.;.T....
+00001850: a136 64d1 850c da88 6517 316c 236e ba08  .6d.....e.1l#n..
+00001860: bf8d 58bd 60e4 19e4 d30b 90b6 c86d 1711  ..X.`........m..
+00001870: b411 775d 44bf 8df8 dc45 446d c497 2ea2  ..w]D....EDm....
+00001880: d746 408f 7dfe dcc3 06e1 c142 d63d b15c  .F@.}......B.=.\
+00001890: 59bc 537c c552 45c5 7997 3e35 fb30 0ce7  Y.S|.RE.y.>5.0..
+000018a0: c33e 9a3b bd79 b470 46c3 f0da 9987 c877  .>.;.y.pF......w
+000018b0: 4603 d41b dc84 cb55 7013 3de9 0e51 e00d  F......Up.=..Q..
+000018c0: fd8a c586 e5d2 4a69 62ba de00 ba84 287b  ......Jib.....({
+000018d0: a5ef ea13 c50b 5312 6bae a0b7 99e9 16de  ......S.k.......
+000018e0: 2828 d48b efc2 fd84 7370 529e e846 debc  ((......spR..F..
+000018f0: a3cc fe03 0000 ffff 0300 504b 0304 1400  ..........PK....
+00001900: 0600 0800 0000 2100 fd3b 0d27 ea00 0000  ......!..;.'....
+00001910: df01 0000 1400 0000 786c 2f73 6861 7265  ........xl/share
+00001920: 6453 7472 696e 6773 2e78 6d6c 7491 414b  dStrings.xmlt.AK
+00001930: 0331 1085 ef82 ff21 e46e b3f6 2022 d914  .1.....!.n.. "..
+00001940: d956 1044 04ad f7b0 9976 039b 49cc 4c4a  .V.D.....v..I.LJ
+00001950: fdf7 462a 0a92 1ee7 7d3c debc 19bd 3a86  ..F*....}<....:.
+00001960: 591c 2093 8fd8 cbeb 4527 05e0 189d c77d  Y. .....E'.....}
+00001970: 2fb7 6f0f 57b7 5210 5b74 768e 08bd fc04  /.o.W.R.[tv.....
+00001980: 922b 7379 a189 5854 2f52 2f27 e674 a714  .+sy..XT/R/'.t..
+00001990: 8d13 044b 8b98 002b d9c5 1c2c d731 ef15  ...K...+...,.1..
+000019a0: a50c d6d1 04c0 6156 cbae bb51 c17a 9462  ......aV...Q.z.b
+000019b0: 8c05 b9e6 2ea5 28e8 3f0a 0cbf 82d1 e48d  ......(.?.......
+000019c0: 66b3 39a6 9819 9cb8 67ad d868 f52d 9fd0  f.9.....g..h.-..
+000019d0: 4b8e ae8c 2c1e d7e7 c8b3 0df0 9fbd 03ba  K...,...........
+000019e0: 981b a61f d0f2 d4a4 8377 9045 3beb c45a  .........w.E;..Z
+000019f0: c6a1 166f 2fbf 4dee 0c79 f2c4 f5fe 8da8  ...o/.M..y......
+00001a00: 2122 67db 6cfc ca96 0bfd 7555 f541 e60b  !"g.l.....uU.A..
+00001a10: 0000 ffff 0300 504b 0304 1400 0600 0800  ......PK........
+00001a20: 0000 2100 bdd0 296d 5601 0000 6e02 0000  ..!...)mV...n...
+00001a30: 1100 0801 646f 6350 726f 7073 2f63 6f72  ....docProps/cor
+00001a40: 652e 786d 6c20 a204 0128 a000 0100 0000  e.xml ...(......
+00001a50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001a60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001a70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001a80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001a90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001aa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ab0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ac0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ad0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ae0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001af0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001b00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001b10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001b20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001b30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001b40: 0000 0000 0000 0000 0000 0000 0084 925f  ..............._
+00001b50: 4bc3 3014 c5df 05bf 43c9 7b9b fe99 6384  K.0.....C.{...c.
+00001b60: b603 953d 3914 9c28 be85 e476 0bb6 4948  ...=9..(...v..IH
+00001b70: a25d bfbd 69bb d50e 051f 73cf c92f e75c  .]..i.....s../.\
+00001b80: 92af 8f4d 1d7c 81b1 42c9 0225 518c 0290  ...M.|..B..%Q...
+00001b90: 4c71 21f7 057a d96d c215 0aac a392 d35a  Lq!..z.m.......Z
+00001ba0: 4928 5007 16ad cbeb ab9c 69c2 9481 27a3  I(P.......i...'.
+00001bb0: 3418 27c0 069e 242d 61ba 4007 e734 c1d8  4.'...$-a.@..4..
+00001bc0: b203 34d4 46de 21bd 5829 d350 e78f 668f  ..4.F.!.X).P..f.
+00001bd0: 3565 1f74 0f38 8de3 256e c051 4e1d c53d  5e.t.8..%n.QN..=
+00001be0: 30d4 1311 9d90 9c4d 48fd 69ea 01c0 1986  0......MH.i.....
+00001bf0: 1a1a 90ce e224 4af0 8fd7 8169 ec9f 1706  .....$J....i....
+00001c00: 65e6 6c84 ebb4 ef74 8a3b 6773 368a 93fb  e.l....t.;gs6...
+00001c10: 68c5 646c db36 6ab3 2186 cf9f e0b7 edc3  h.dl.6j.!.......
+00001c20: f350 3514 b2df 1503 54e6 9c11 6680 3a65  .P5.....T...f.:e
+00001c30: cabe bfee 8e75 8e67 c37e 8135 b56e eb77  .....u.g.~.5.n.w
+00001c40: 5d09 e0b7 5db9 15cc 28ab 2a17 3c56 9560  ]...]...(.*.<V.`
+00001c50: 10bc 5830 39fe 6df4 f0a1 cbf8 02f0 c0a7  ..X09.m.........
+00001c60: 2363 97b3 f29a dddd ef36 a84c e334 0e93  #c.......6.L.4..
+00001c70: 248c 6f76 f18a 644b 92ae defb 1c17 f7fb  $.ov..dK........
+00001c80: b4e3 a039 a5f9 9798 8659 bc4b 1664 9192  ...9.....Y.K.d..
+00001c90: 349b 11cf 8072 c87d f943 ca6f 0000 00ff  4....r.}.C.o....
+00001ca0: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
+00001cb0: 00b5 219a f690 0100 000d 0300 0010 0008  ..!.............
+00001cc0: 0164 6f63 5072 6f70 732f 6170 702e 786d  .docProps/app.xm
+00001cd0: 6c20 a204 0128 a000 0100 0000 0000 0000  l ...(..........
 00001ce0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001cf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001d00: 0000 0000 0000 8492 5f4b c330 14c5 df05  ........_K.0....
-00001d10: bf43 c97b 9bfe 61b3 94b6 0395 3d39 14ac  .C.{..a.....=9..
-00001d20: 28be 85e4 760b b649 48a2 5dbf bd69 bbd5  (...v..IH.]..i..
-00001d30: 0e05 1f73 cfc9 2fe7 5c92 6f8e 6de3 7d81  ...s../.\.o.m.}.
-00001d40: 365c 8a02 4541 883c 1054 322e f605 7aa9  6\..EA.<.T2...z.
-00001d50: b67e 8a3c 6389 60a4 9102 0ad4 8341 9bf2  .~.<c.`......A..
-00001d60: fa2a a72a a352 c393 960a b4e5 603c 4712  .*.*.R......`<G.
-00001d70: 26a3 aa40 076b 5586 b1a1 0768 8909 9c43  &..@.kU....h...C
-00001d80: 38b1 96ba 25d6 1df5 1e2b 423f c81e 701c  8...%....+B?..p.
-00001d90: 866b dc82 258c 5882 07a0 af66 223a 2119  .k..%.X....f":!.
-00001da0: 9d91 ea53 3723 8051 0c0d b420 acc1 5110  ...S7#.Q... ..Q.
-00001db0: e11f af05 dd9a 3f2f 8cca c2d9 72db 2bd7  ......?/....r.+.
-00001dc0: e914 77c9 6674 1267 f7d1 f0d9 d875 5dd0  ..w.ft.g.....u].
-00001dd0: 2563 0c97 3fc2 6fbb 87e7 b1aa cfc5 b02b  %c..?.o........+
-00001de0: 0aa8 cc19 cda8 0662 a52e 87fe aa3f 3639  .......b.....?69
-00001df0: 5e0c 8705 36c4 d89d db75 cd81 ddf6 e58e  ^...6....u......
-00001e00: 532d 8dac adf7 58d7 9c82 f762 40e7 f8b7  S-....X....b@...
-00001e10: d1c1 c72e d30b c03c 972e 9bba 9c95 d7e4  .......<........
-00001e20: eebe daa2 320e e3d0 8f22 3f5c 5561 9a25  ....2...."?\Ua.%
-00001e30: eb2c 4edf 871c 17f7 87b4 d3a0 3da5 f997  .,N.........=...
-00001e40: 18fb 4958 458e 9866 ab9b 05f1 0c28 c7dc  ..IXE..f.....(..
-00001e50: 973f a4fc 0600 00ff ff03 0050 4b03 0414  .?.........PK...
-00001e60: 0006 0008 0000 0021 00b5 219a f690 0100  .......!..!.....
-00001e70: 000d 0300 0010 0008 0164 6f63 5072 6f70  .........docProp
-00001e80: 732f 6170 702e 786d 6c20 a204 0128 a000  s/app.xml ...(..
-00001e90: 0100 0000 0000 0000 0000 0000 0000 0000  ................
-00001ea0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f90: 009c 9241 6edb 3010 45f7 0572 0782 fb98  ...An.0.E..r....
-00001fa0: 7212 0485 4131 2892 065e 34a8 013b d94f  r...A1(..^4..;.O
-00001fb0: a991 c596 2605 722c d8bd 4dcf d28b 7524  ....&.r,..M...u$
-00001fc0: 218e dc74 d5dd 70e6 f3f3 f193 faee b0f3  !..t..p.........
-00001fd0: a2c3 945d 0ca5 9ccf 0a29 30d8 58b9 b02d  ...].....)0.X..-
-00001fe0: e5f3 e6f1 f2a3 1499 2054 e063 c052 1e31  ........ T.c.R.1
-00001ff0: cb3b 73f1 41af 526c 3191 c32c d822 e452  .;s.A.Rl1..,.".R
-00002000: 3644 ed42 a96c 1bdc 419e f138 f0a4 8e69  6D.B.l..A..8...i
-00002010: 07c4 cbb4 55b1 ae9d c587 68f7 3b0c a4ae  ....U.....h.;...
-00002020: 8ae2 56e1 8130 5458 5db6 2743 393a 2e3a  ..V..0TX].'C9:.:
-00002030: fa5f d32a da9e 2fbf 6c8e 2d03 1bfd a96d  ._.*../.l.-....m
-00002040: bdb3 407c 4bf3 e46c 8a39 d624 9ec0 ba40  ..@|K..l.9.$...@
-00002050: 3137 e2f3 c1a2 d76a 2ad3 ccb9 46bb 4f8e  17.....j*...F.O.
-00002060: 8ea6 d06a bad4 6b0b 1eef f908 5383 cfa8  ...j..k.....S...
-00002070: d55b 432f 11fa f856 e052 36ba a345 8796  .[C/...V.R6..E..
-00002080: 6212 d9fd e400 afa4 f806 197b b052 7690  b..........{.Rv.
-00002090: 1c04 62c0 5e36 2e86 dab7 9992 59c6 ef90  ..b.^6......Y...
-000020a0: 4585 c2fe fee5 edde 47ad 5837 ce86 72ba  E.......G.X7..r.
-000020b0: 655a bb1b 331f 045c 9c0b 7b83 9187 07e7  eZ..3..\..{.....
-000020c0: a41b 471e f3d7 7a05 89fe 013e 9f82 0f0c  ..G...z....>....
-000020d0: 23f6 88f3 0004 efe8 867b f339 7f39 7f71  #........{.9.9.q
-000020e0: e147 7e6e 3791 37e1 6b80 e74d bd6e 2061  .G~n7.7.k..M.n a
-000020f0: c599 9f02 3e35 f492 b34b be37 b96f 206c  ....>5...K.7.o l
-00002100: b17a d5bc 1ff4 0fff 32fe 6e33 bf9d 15d7  .z......2.n3....
-00002110: 05bf e4a4 a7d5 db3f 367f 0000 00ff ff03  .......?6.......
-00002120: 0050 4b01 022d 0014 0006 0008 0000 0021  .PK..-.........!
-00002130: 0062 ee9d 685e 0100 0090 0400 0013 0000  .b..h^..........
-00002140: 0000 0000 0000 0000 0000 0000 0000 005b  ...............[
-00002150: 436f 6e74 656e 745f 5479 7065 735d 2e78  Content_Types].x
-00002160: 6d6c 504b 0102 2d00 1400 0600 0800 0000  mlPK..-.........
-00002170: 2100 b555 3023 f400 0000 4c02 0000 0b00  !..U0#....L.....
-00002180: 0000 0000 0000 0000 0000 0000 9703 0000  ................
-00002190: 5f72 656c 732f 2e72 656c 7350 4b01 022d  _rels/.relsPK..-
-000021a0: 0014 0006 0008 0000 0021 0081 3e94 97f3  .........!..>...
-000021b0: 0000 00ba 0200 001a 0000 0000 0000 0000  ................
-000021c0: 0000 0000 00bc 0600 0078 6c2f 5f72 656c  .........xl/_rel
-000021d0: 732f 776f 726b 626f 6f6b 2e78 6d6c 2e72  s/workbook.xml.r
-000021e0: 656c 7350 4b01 022d 0014 0006 0008 0000  elsPK..-........
-000021f0: 0021 006a e588 47e6 0200 00c0 0600 000f  .!.j..G.........
-00002200: 0000 0000 0000 0000 0000 0000 00ef 0800  ................
-00002210: 0078 6c2f 776f 726b 626f 6f6b 2e78 6d6c  .xl/workbook.xml
-00002220: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
-00002230: e4ac 1593 eb02 0000 1f07 0000 0d00 0000  ................
-00002240: 0000 0000 0000 0000 0000 020c 0000 786c  ..............xl
-00002250: 2f73 7479 6c65 732e 786d 6c50 4b01 022d  /styles.xmlPK..-
-00002260: 0014 0006 0008 0000 0021 00e9 a625 b866  .........!...%.f
-00002270: 0600 0053 1b00 0013 0000 0000 0000 0000  ...S............
-00002280: 0000 0000 0018 0f00 0078 6c2f 7468 656d  .........xl/them
-00002290: 652f 7468 656d 6531 2e78 6d6c 504b 0102  e/theme1.xmlPK..
-000022a0: 2d00 1400 0600 0800 0000 2100 05f4 c1f0  -.........!.....
-000022b0: 5304 0000 e410 0000 1800 0000 0000 0000  S...............
-000022c0: 0000 0000 0000 af15 0000 786c 2f77 6f72  ..........xl/wor
-000022d0: 6b73 6865 6574 732f 7368 6565 7431 2e78  ksheets/sheet1.x
-000022e0: 6d6c 504b 0102 2d00 1400 0600 0800 0000  mlPK..-.........
-000022f0: 2100 83fd 7ca1 6501 0000 2f04 0000 1400  !...|.e.../.....
-00002300: 0000 0000 0000 0000 0000 0000 381a 0000  ............8...
-00002310: 786c 2f73 6861 7265 6453 7472 696e 6773  xl/sharedStrings
-00002320: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
-00002330: 0000 2100 3f10 042b 5501 0000 6e02 0000  ..!.?..+U...n...
-00002340: 1100 0000 0000 0000 0000 0000 0000 cf1b  ................
-00002350: 0000 646f 6350 726f 7073 2f63 6f72 652e  ..docProps/core.
-00002360: 786d 6c50 4b01 022d 0014 0006 0008 0000  xmlPK..-........
-00002370: 0021 00b5 219a f690 0100 000d 0300 0010  .!..!...........
-00002380: 0000 0000 0000 0000 0000 0000 005b 1e00  .............[..
-00002390: 0064 6f63 5072 6f70 732f 6170 702e 786d  .docProps/app.xm
-000023a0: 6c50 4b05 0600 0000 000a 000a 0080 0200  lPK.............
-000023b0: 0021 2100 0000 00                        .!!....
+00001d00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001da0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001db0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001dc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001dd0: 0000 0000 0000 0000 009c 9241 6edb 3010  ...........An.0.
+00001de0: 45f7 0572 0782 fb98 7212 0485 4131 2892  E..r....r...A1(.
+00001df0: 065e 34a8 013b d94f a991 c596 2605 722c  .^4..;.O....&.r,
+00001e00: d8bd 4dcf d28b 7524 218e dc74 d5dd 70e6  ..M...u$!..t..p.
+00001e10: f3f3 f193 faee b0f3 a2c3 945d 0ca5 9ccf  ...........]....
+00001e20: 0a29 30d8 58b9 b02d e5f3 e6f1 f2a3 1499  .)0.X..-........
+00001e30: 2054 e063 c052 1e31 cb3b 73f1 41af 526c   T.c.R.1.;s.A.Rl
+00001e40: 3191 c32c d822 e452 3644 ed42 a96c 1bdc  1..,.".R6D.B.l..
+00001e50: 419e f138 f0a4 8e69 07c4 cbb4 55b1 ae9d  A..8...i....U...
+00001e60: c587 68f7 3b0c a4ae 8ae2 56e1 8130 5458  ..h.;.....V..0TX
+00001e70: 5db6 2743 393a 2e3a fa5f d32a da9e 2fbf  ].'C9:.:._.*../.
+00001e80: 6c8e 2d03 1bfd a96d bdb3 407c 4bf3 e46c  l.-....m..@|K..l
+00001e90: 8a39 d624 9ec0 ba40 3137 e2f3 c1a2 d76a  .9.$...@17.....j
+00001ea0: 2ad3 ccb9 46bb 4f8e 8ea6 d06a bad4 6b0b  *...F.O....j..k.
+00001eb0: 1eef f908 5383 cfa8 d55b 432f 11fa f856  ....S....[C/...V
+00001ec0: e052 36ba a345 8796 6212 d9fd e400 afa4  .R6..E..b.......
+00001ed0: f806 197b b052 7690 1c04 62c0 5e36 2e86  ...{.Rv...b.^6..
+00001ee0: dab7 9992 59c6 ef90 4585 c2fe fee5 edde  ....Y...E.......
+00001ef0: 47ad 5837 ce86 72ba 655a bb1b 331f 045c  G.X7..r.eZ..3..\
+00001f00: 9c0b 7b83 9187 07e7 a41b 471e f3d7 7a05  ..{.......G...z.
+00001f10: 89fe 013e 9f82 0f0c 23f6 88f3 0004 efe8  ...>....#.......
+00001f20: 867b f339 7f39 7f71 e147 7e6e 3791 37e1  .{.9.9.q.G~n7.7.
+00001f30: 6b80 e74d bd6e 2061 c599 9f02 3e35 f492  k..M.n a....>5..
+00001f40: b34b be37 b96f 206c b17a d5bc 1ff4 0fff  .K.7.o l.z......
+00001f50: 32fe 6e33 bf9d 15d7 05bf e4a4 a7d5 db3f  2.n3...........?
+00001f60: 367f 0000 00ff ff03 0050 4b01 022d 0014  6........PK..-..
+00001f70: 0006 0008 0000 0021 0062 ee9d 685e 0100  .......!.b..h^..
+00001f80: 0090 0400 0013 0000 0000 0000 0000 0000  ................
+00001f90: 0000 0000 0000 005b 436f 6e74 656e 745f  .......[Content_
+00001fa0: 5479 7065 735d 2e78 6d6c 504b 0102 2d00  Types].xmlPK..-.
+00001fb0: 1400 0600 0800 0000 2100 b555 3023 f400  ........!..U0#..
+00001fc0: 0000 4c02 0000 0b00 0000 0000 0000 0000  ..L.............
+00001fd0: 0000 0000 9703 0000 5f72 656c 732f 2e72  ........_rels/.r
+00001fe0: 656c 7350 4b01 022d 0014 0006 0008 0000  elsPK..-........
+00001ff0: 0021 0081 3e94 97f3 0000 00ba 0200 001a  .!..>...........
+00002000: 0000 0000 0000 0000 0000 0000 00bc 0600  ................
+00002010: 0078 6c2f 5f72 656c 732f 776f 726b 626f  .xl/_rels/workbo
+00002020: 6f6b 2e78 6d6c 2e72 656c 7350 4b01 022d  ok.xml.relsPK..-
+00002030: 0014 0006 0008 0000 0021 0091 d238 c2dd  .........!...8..
+00002040: 0200 00b7 0600 000f 0000 0000 0000 0000  ................
+00002050: 0000 0000 00ef 0800 0078 6c2f 776f 726b  .........xl/work
+00002060: 626f 6f6b 2e78 6d6c 504b 0102 2d00 1400  book.xmlPK..-...
+00002070: 0600 0800 0000 2100 e4ac 1593 eb02 0000  ......!.........
+00002080: 1f07 0000 0d00 0000 0000 0000 0000 0000  ................
+00002090: 0000 f90b 0000 786c 2f73 7479 6c65 732e  ......xl/styles.
+000020a0: 786d 6c50 4b01 022d 0014 0006 0008 0000  xmlPK..-........
+000020b0: 0021 00e9 a625 b866 0600 0053 1b00 0013  .!...%.f...S....
+000020c0: 0000 0000 0000 0000 0000 0000 000f 0f00  ................
+000020d0: 0078 6c2f 7468 656d 652f 7468 656d 6531  .xl/theme/theme1
+000020e0: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
+000020f0: 0000 2100 92e6 ccb8 1e03 0000 e808 0000  ..!.............
+00002100: 1800 0000 0000 0000 0000 0000 0000 a615  ................
+00002110: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
+00002120: 7368 6565 7431 2e78 6d6c 504b 0102 2d00  sheet1.xmlPK..-.
+00002130: 1400 0600 0800 0000 2100 fd3b 0d27 ea00  ........!..;.'..
+00002140: 0000 df01 0000 1400 0000 0000 0000 0000  ................
+00002150: 0000 0000 fa18 0000 786c 2f73 6861 7265  ........xl/share
+00002160: 6453 7472 696e 6773 2e78 6d6c 504b 0102  dStrings.xmlPK..
+00002170: 2d00 1400 0600 0800 0000 2100 bdd0 296d  -.........!...)m
+00002180: 5601 0000 6e02 0000 1100 0000 0000 0000  V...n...........
+00002190: 0000 0000 0000 161a 0000 646f 6350 726f  ..........docPro
+000021a0: 7073 2f63 6f72 652e 786d 6c50 4b01 022d  ps/core.xmlPK..-
+000021b0: 0014 0006 0008 0000 0021 00b5 219a f690  .........!..!...
+000021c0: 0100 000d 0300 0010 0000 0000 0000 0000  ................
+000021d0: 0000 0000 00a3 1c00 0064 6f63 5072 6f70  .........docProp
+000021e0: 732f 6170 702e 786d 6c50 4b05 0600 0000  s/app.xmlPK.....
+000021f0: 000a 000a 0080 0200 0069 1f00 0000 00    .........i.....
```

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/listing_list/entrypoint.py` & `connect_cli-27.0/connect/.data/connect_reports/reports/listing_list/entrypoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (c) 2021, CloudBlue
+# Copyright (c) 2023, CloudBlue
 # All rights reserved.
 #
 
 from connect.client import R
 
 from ..utils import convert_to_datetime, get_basic_value, get_value, today_str
```

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/listing_list/templates/xlsx/template.xlsx` & `connect_cli-27.0/connect/.data/connect_reports/reports/fulfillment_requests_line_item/templates/xlsx/template.xlsx`

 * *Files 14% similar despite different names*

```diff
@@ -137,408 +137,442 @@
 00000880: cbb4 e480 fa84 53ec ad82 b4b7 b720 9a29  ......S...... .)
 00000890: 66e5 ffb9 43db f606 9f82 791f d1f3 1909  f...C.....y.....
 000008a0: 493c 0d79 00d1 e8d4 212b f8c1 45f6 08f2  I<.y....!+..E...
 000008b0: bcfc 664d 79ce 6bc1 a3fa 0ce5 1cab 4b1e  ..fMy.k.......K.
 000008c0: aa35 3d7c 8674 2087 c847 1f7f 2992 73e5  .5=|.t ..G..).s.
 000008d0: a299 bb55 efe1 7442 fbca 29bf dbf2 2ccb  ...U..tB..)...,.
 000008e0: f4ef 66e4 c9c7 d5df 0000 00ff ff03 0050  ..f............P
-000008f0: 4b03 0414 0006 0008 0000 0021 0091 d238  K..........!...8
-00000900: c2dd 0200 00b7 0600 000f 0000 0078 6c2f  .............xl/
-00000910: 776f 726b 626f 6f6b 2e78 6d6c a455 df6f  workbook.xml.U.o
-00000920: da30 107e 9fb4 ff21 b378 0d8e f991 a288  .0.~...!.x......
-00000930: 5075 a568 48dd 84d6 b57d 44c6 31c4 aa63  Pu.hH....}D.1..c
-00000940: 67b6 2954 55ff f79d 1342 a1bc 746d 0476  g.)TU....B..tm.v
-00000950: 2ee7 7cfe eeee 3b67 78be 2d64 f0c8 8d15  ..|...;gx.-d....
-00000960: 5aa5 88b4 2314 70c5 7426 d42a 45b7 7f26  Z...#.p.t&.*E..&
-00000970: e100 05d6 5195 51a9 154f d113 b7e8 7cf4  ....Q.Q..O....|.
-00000980: f5cb 70a3 cdc3 42eb 8700 0094 4d51 ee5c  ..p...B.....MQ.\
-00000990: 9960 6c59 ce0b 6adb bae4 0a3c 4b6d 0aea  .`lY..j....<Km..
-000009a0: c034 2b6c 4bc3 6966 73ce 5d21 7127 8a62  .4+lK.ifs.]!q'.b
-000009b0: 5c50 a150 8d90 98f7 60e8 e552 303e d66c  \P.P....`..R0>.l
-000009c0: 5d70 e56a 10c3 2575 40df e6a2 b40d 5ac1  ]p.j..%u@.....Z.
-000009d0: de03 5750 f3b0 2e43 a68b 1220 1642 0af7  ..WP...C... .B..
-000009e0: 5481 a2a0 60c9 74a5 b4a1 0b09 616f 493f  T...`.t.....aoI?
-000009f0: d81a f8c5 f027 110c 9d66 2770 9d6c 5508  .....'...f'p.lU.
-00000a00: 66b4 d54b d706 685c 933e 899f 4498 90a3  f..K..h\.>..D...
-00000a10: 146c 4f73 f03e a41e 36fc 51f8 1aee 5999  .lOs.>..6.Q...Y.
-00000a20: f883 ace2 3d56 fc0a 46a2 4fa3 1190 56a5  ....=V..F.O...V.
-00000a30: 9504 92f7 41b4 fe9e 5b07 8d86 4b21 f95d  ....A...[...K!.]
-00000a40: 2ddd 8096 e52f 5af8 4a49 1448 6add 5526  -..../Z.JI.Hj.U&
-00000a50: 1ccf 5274 06a6 def0 a307 665d 7e5f 0b09  ..Rt......f]~_..
-00000a60: 5e42 3a9d 08e1 d15e ce33 0306 d4fe 423a  ^B:....^.3....B:
-00000a70: 6e14 75fc 522b 0752 db51 ffac ac2a eccb  n.u.R+.R.Q...*..
-00000a80: 5c83 8883 dffc ef5a 180e bd03 1282 7060  \......Z......p`
-00000a90: a42c a10b 3ba3 2e0f d646 a608 df5a 880f  .,..;....F...Z..
-00000aa0: 3462 18c1 8dea 2d06 4e8a 3387 593d 874c  4b....-.N.3.Y=.L
-00000ab0: 0acc 1473 7e36 bcd4 c6d9 bdaf b19b 590a  ...s~6........Y.
-00000ac0: eba0 b9e7 7ec6 071a a6a7 0df3 1f2a a6cc  ....~........*..
-00000ad0: 2711 43e2 eae0 eafb b749 8418 4dd2 2875  '.C......I..M.(u
-00000ae0: e64c 00f7 d3f1 3554 eb86 3e42 ed40 21d9  .L....5T..>B.@!.
-00000af0: aeb5 a7be 38dd b962 2621 f3e7 cbab 2ef9  ....8..b&!......
-00000b00: de19 8cc3 c9c5 d538 8ce3 1e09 07f1 a417  .......8........
-00000b10: 8ec1 ecc6 dd98 c483 b317 08c6 c409 d374  ...............t
-00000b20: edf2 9d2c 3c74 8a7a 5ec8 6f5d 3fe9 b6f1  ...,<t.z^.o]?...
-00000b30: 9028 598b ec95 c673 b4bb 423f bf19 1adf  .(Y....s..B?....
-00000b40: 8b0f d81f 8077 826f ecab 80bc 196c ef85  .....w.o.....l..
-00000b50: caf4 2645 ddc1 590f a27a 6aec 7e04 d6a6  ..&E..Y..zj.~...
-00000b60: 72de 8bcc e5b0 a23f f02b ea67 3fb8 58e5  r......?.+.g?.X.
-00000b70: c0b8 1311 bf10 1ac5 334b d111 a371 cd68  ........3K...q.h
-00000b80: 0257 e887 2346 f880 5275 d402 b56a 0e54  .W..#F..Ru...j.T
-00000b90: d51e 63ea 289c e8fe 10f6 2986 53cc 247e  ..c.(.....).S.$~
-00000ba0: 0733 cd48 55c2 e6a5 8c2f 85e2 996f 2a80  .3.HU..../...o*.
-00000bb0: 38b0 7640 f3ad 5445 7b3e 11be 513c ea82  8.v@..TE{>..Q<..
-00000bc0: 5aee 7b8d 5179 d3c0 430c b9c8 32ee 3f2d  Z.{.Qy..C...2.?-
-00000bd0: 68e4 577d 6b5d b448 d2ba 6e91 213e 0005  h.W}k].H..n.!>..
-00000be0: bd1c 6f08 286c 6602 3f79 9e55 8fe2 e69b  ..o.(lf.?y.U....
-00000bf0: 33fa 0700 00ff ff03 0050 4b03 0414 0006  3........PK.....
-00000c00: 0008 0000 0021 00e4 ac15 93eb 0200 001f  .....!..........
-00000c10: 0700 000d 0000 0078 6c2f 7374 796c 6573  .......xl/styles
-00000c20: 2e78 6d6c a455 db8e 9b30 107d afd4 7fb0  .xml.U...0.}....
-00000c30: fc4e b804 4888 4256 4db2 482b 6dab 4abb  .N..H.BVM.H+m.J.
-00000c40: 95fa ea80 49ac f505 1927 25ad faef 1d03  ....I....'%.....
-00000c50: 21ac b66a b7db bcd8 1ec6 67ce cc19 4f96  !..j......g...O.
-00000c60: 378d e0e8 4475 cd94 4cb1 3ff1 30a2 3257  7...Du..L.?.0.2W
-00000c70: 0593 fb14 7f79 cc9c 3946 b521 b220 5c49  .....y..9F.!. \I
-00000c80: 9ae2 33ad f1cd eafd bb65 6dce 9c3e 1c28  ..3......em..>.(
-00000c90: 3508 2064 9de2 8331 d5c2 75eb fc40 05a9  5. d...1..u..@..
-00000ca0: 27aa a212 be94 4a0b 62e0 a8f7 6e5d 694a  '.....J.b...n]iJ
-00000cb0: 8ada 5e12 dc0d 3c2f 7605 6112 7708 0b91  ..^...</v.a.w...
-00000cc0: bf06 4410 fd74 ac9c 5c89 8a18 b663 9c99  ..D..t..\....c..
-00000cd0: 738b 8591 c817 777b a934 d971 a0da f821  s.....w{.4.q...!
-00000ce0: c951 e3c7 3a40 8dbe 0469 ad2f e208 966b  .Q..:@...i./...k
-00000cf0: 55ab d24c 00d7 5565 c972 fa92 6ee2 262e  U..L..Ue.r..n.&.
-00000d00: c9af 4880 fc36 243f 72bd e059 ee8d 7e23  ..H..6$?r..Y..~#
-00000d10: 52e8 6a7a 6256 3ebc 5a96 4a9a 1ae5 ea28  R.jzbV>.Z.J....(
-00000d20: 0d88 0944 6d09 164f 527d 9399 fd64 8d9d  ...Dm..OR}...d..
-00000d30: d76a 597f 4727 c2c1 e263 77b5 cc15 571a  .jY.G'...cw...W.
-00000d40: 1990 0e2a d75a 2411 b4f3 d810 ce76 9a59  ...*.Z$......v.Y
-00000d50: b792 08c6 cf9d 39b0 8656 edde 4f30 a8bd  ......9..V..O0..
-00000d60: 35ba 9647 bfd4 7089 713e b09a 5a02 6058  5..G..p.q>..Z.`X
-00000d70: 2d41 3e43 b5cc e080 fafd e3b9 82f0 123a  -A>C...........:
-00000d80: ad83 69fd fee2 bdd7 e4ec 07d1 eb2f d48a  ..i........../..
-00000d90: b3c2 b2d8 6fc6 4943 e71b 66eb e678 9320  ....o.IC..f..x. 
-00000da0: 4c92 d9cc b7bf d93c 995a ec5d efcd 6441  L......<.Z.]..dA
-00000db0: 1b5a a438 0edb 90a3 2c6c c62d e376 81c4  .Z.8....,l.-.v..
-00000dc0: 774a 17f0 b4ae 825c 4cab 25a7 a501 54cd  wJ.....\L.%...T.
-00000dd0: f607 bb1a 55d9 18ca 1868 bfd5 b260 64af  ....U....h...`d.
-00000de0: 24e1 b696 1dc8 b001 d89c 72fe 609f dfd7  $.........r.`...
-00000df0: f219 7653 2279 1499 3077 400f d2b1 2a5c  ..vS"y..0w@...*\
-00000e00: b6c0 abdf 7678 ddc1 e28f d13a ec11 6c00  ....vx.....:..l.
-00000e10: 75fa 7758 d494 03fe 2b6e 0718 8d49 0db7  u.wX....+n...I..
-00000e20: 11a9 2a7e b6fd d1b7 64cb 15d8 8d4a f0ac  ..*~....d....J..
-00000e30: 0043 2ac8 366f 8a3f d9d9 c3e1 19f4 74d0  .C*.6o.?......t.
-00000e40: eec8 3888 fc9b e401 b368 aee5 f4ac b6c6  ..8......h......
-00000e50: ce91 b6d0 4314 a86a 414b 72e4 e671 f898  ....C..jAKr..q..
-00000e60: e2eb fe23 2dd8 5124 83d7 6776 52a6 8548  ...#-.Q$..gvR..H
-00000e70: f175 7f6f 55f7 631b 8336 e6be 86b7 022b  .u.oU.c..6.....+
-00000e80: 3a6a 96e2 1fb7 eb59 b2bd cd02 67ee ade7  :j.....Y....g...
-00000e90: 4e38 a591 9344 ebad 1385 9bf5 769b 255e  N8...D......v.%^
-00000ea0: e06d 7e8e a6d9 7fcc b276 f882 c07e b8a8  .m~......v...~..
-00000eb0: 394c 3cdd 27db a7f8 70b5 a578 74e8 e8b7  9L<.'...p..xt...
-00000ec0: dd0f b4c7 dc93 20f6 3e44 bee7 6453 cf77  ...... .>D..dS.w
-00000ed0: c298 cc9d 793c 8d9c 2cf2 836d 1cae 6fa3  ....y<..,..m..o.
-00000ee0: 2c1a 718f de38 f33c d7f7 bbe9 69c9 470b  ,.q..8.<....i.G.
-00000ef0: c304 e54c 5eb4 ba28 34b6 8248 70fc 4312  ...L^..(4..Hp.C.
-00000f00: ee45 09f7 facf b6fa 0500 00ff ff03 0050  .E.............P
-00000f10: 4b03 0414 0006 0008 0000 0021 00e9 a625  K..........!...%
-00000f20: b866 0600 0053 1b00 0013 0000 0078 6c2f  .f...S.......xl/
-00000f30: 7468 656d 652f 7468 656d 6531 2e78 6d6c  theme/theme1.xml
-00000f40: ec59 cd6e 1b37 10be 17e8 3b10 7b4f 2cd9  .Y.n.7....;.{O,.
-00000f50: 9262 1991 034b 96e2 3671 62d8 4a8a 1ca9  .b...K..6qb.J...
-00000f60: 5d6a 9711 77b9 2029 3bba 15c9 b140 81a2  ]j..w. );....@..
-00000f70: 69d1 4b81 de7a 28da 0648 805e d2a7 719b  i.K..z(..H.^..q.
-00000f80: a24d 81bc 4287 e44a 5a5a 546c 2706 fa17  .M..B..JZZTl'...
-00000f90: 1d6c 2df7 e3fc cf70 86ba 7aed 41ca d021  .l-....p..z.A..!
-00000fa0: 1192 f2ac 1554 2f57 0244 b290 4734 8b5b  .....T/W.D..G4.[
-00000fb0: c19d 7eef d27a 80a4 c259 8419 cf48 2b98  ..~..z...Y...H+.
-00000fc0: 1019 5cdb 7cff bdab 7843 2524 2508 f667  ..\.|...xC%$%..g
-00000fd0: 7203 b782 44a9 7c63 6545 86b0 8ce5 659e  r...D.|ceE....e.
-00000fe0: 930c de0d b948 b182 4711 af44 021f 01dd  .....H..G..D....
-00000ff0: 94ad ac56 2a8d 9514 d32c 4019 4e81 eced  ...V*....,@.N...
-00001000: e190 8604 f535 c960 734a bccb e031 5352  .....5.`sJ...1SR
-00001010: 2f84 4c1c 68d2 c4d9 61b0 d1a8 aa11 7222  /.L.h...a.....r"
-00001020: 3b4c a043 cc5a 01f0 89f8 519f 3c50 0162  ;L.C.Z....Q.<P.b
-00001030: 582a 78d1 0a2a e613 ac6c 5e5d c11b c526  X*x..*...l^]...&
-00001040: a696 ec2d edeb 994f b1af d810 8d56 0d4f  ...-...O.....V.O
-00001050: 110f 664c abbd 5af3 caf6 8cbe 0130 b588  ..fL..Z......0..
-00001060: eb76 bb9d 6e75 46cf 0070 1882 a656 9632  .v..nuF..p...V.2
-00001070: cd5a 6fbd da9e d22c 81ec d745 da9d 4abd  .Zo....,...E..J.
-00001080: 5273 f125 fa6b 0b32 37db ed76 bd59 c862  Rs.%.k.27..v.Y.b
-00001090: 891a 90fd 5a5b c0af 571a b5ad 5507 6f40  ....Z[..W...U.o@
-000010a0: 165f 5fc0 d7da 5b9d 4ec3 c11b 90c5 3716  .__...[.N.....7.
-000010b0: f0bd 2bcd 46cd c51b 50c2 6836 5a40 6b87  ..+.F...P.h6Z@k.
-000010c0: f67a 05f5 1964 c8d9 8e17 be0e f0f5 4a01  .z...d........J.
-000010d0: 9fa3 201a 66d1 a559 0c79 a696 c55a 8aef  .. .f..Y.y...Z..
-000010e0: 73d1 0380 0632 ac68 86d4 2427 431c 4214  s....2.h..$'C.B.
-000010f0: 7770 3a10 146b 0678 83e0 d21b bb14 ca85  wp:..k.x........
-00001100: 25cd 0bc9 50d0 5cb5 820f 730c 1931 a7f7  %...P.\...s..1..
-00001110: eaf9 f7af 9e3f 45af 9e3f 397e f8ec f8e1  .....?E..?9~....
-00001120: 4fc7 8f1e 1d3f fcd1 d272 36ee e02c 2e6f  O....?...r6..,.o
-00001130: 7cf9 ed67 7f7e fd31 fae3 e937 2f1f 7fe1  |..g.~.1...7/...
-00001140: c7cb 32fe d71f 3ef9 e5e7 cffd 40c8 a0b9  ..2...>.....@...
-00001150: 442f be7c f2db b327 2fbe faf4 f7ef 1e7b  D/.|...'/......{
-00001160: e05b 020f caf0 3e4d 8944 b7c8 11da e729  .[....>M.D.....)
-00001170: e866 0ce3 4a4e 06e2 7c3b fa09 a6ce 0e9c  .f..JN..|;......
-00001180: 006d 0fe9 ae4a 1ce0 ad09 663e 5c9b b8c6  .m...J....f>\...
-00001190: bb2b a078 f880 d7c7 f71d 590f 1231 56d4  .+.x......Y..1V.
-000011a0: c3f9 4692 3ac0 5dce 599b 0baf 016e 685e  ..F.:.].Y....nh^
-000011b0: 250b f7c7 59ec 672e c665 dc3e c687 3ede  %...Y.g..e.>..>.
-000011c0: 1d9c 39ae ed8e 73a8 9ad3 a074 6cdf 4988  ..9...s....tl.I.
-000011d0: 23e6 1ec3 99c2 31c9 8842 fa1d 1f11 e2d1  #.....1..B......
-000011e0: ee1e a58e 5d77 6928 b8e4 4385 ee51 d4c6  ....]wi(..C..Q..
-000011f0: d46b 923e 1d38 8134 dfb4 4353 f0cb c4a7  .k.>.8.4..CS....
-00001200: 33b8 dab1 cdee 5dd4 e6cc a7f5 3639 7491  3.....].....69t.
-00001210: 9010 9879 84ef 13e6 98f1 3a1e 2b9c fa48  ...y......:.+..H
-00001220: f671 caca 06bf 8955 e213 f260 22c2 32ae  .q.....U...`".2.
-00001230: 2b15 783a 268c a36e 44a4 f4ed b92d 40df  +.x:&..nD....-@.
-00001240: 92d3 6f60 a857 5eb7 efb2 49ea 2285 a223  ..o`.W^...I."..#
-00001250: 1fcd 9b98 f332 729b 8f3a 094e 73af cc34  .....2r..:.Ns..4
-00001260: 4bca d80f e408 4214 a33d ae7c f05d ee66  K.....B..=.|.].f
-00001270: 887e 063f e06c a9bb ef52 e2b8 fbf4 4270  .~.?.l...R....Bp
-00001280: 87c6 8e48 f300 d16f c6a2 a8da 4efd 4d69  ...H...o....N.Mi
-00001290: f6ba 62cc 2854 e377 c578 7a3a 6dc1 d1e4  ..b.(T.w.xz:m...
-000012a0: 4b89 9d13 2578 19ee 5f58 78b7 f138 db23  K...%x.._Xx..8.#
-000012b0: 10eb 8b07 cfbb bafb aeee 06ff f9ba bb2c  ...............,
-000012c0: 97cf 5a6d e705 169a e479 5f6c bae4 7469  ..Zm.....y_l..ti
-000012d0: 933c a48c 1da8 0923 37a5 e993 251c 1651  .<.....#7...%..Q
-000012e0: 0f16 4d03 6fa6 b8d9 d094 27f0 b528 ee0e  ..M.o.....'..(..
-000012f0: 2e16 d8ec 4182 ab8f a84a 0e12 9c43 8f5d  ....A....J...C.]
-00001300: 3523 5f2c 0bd2 b144 3997 30db 9965 337c  5#_,...D9.0..e3|
-00001310: 9213 b4cd 3849 a1cd 3693 615d cf0c b61e  ....8I..6.a]....
-00001320: 48ac 7679 6497 d7ca b3e1 8c8c 9914 6333  H.vyd.........c3
-00001330: 7f4e 19ad 6902 6765 b676 e5ed 9855 ad54  .N..i.ge.v...U.T
-00001340: 4bcd e6aa 5635 a299 52e7 a836 5319 7cb8  K...V5..R..6S.|.
-00001350: a81a 2cce ac09 5d08 82de 05ac dc80 115d  ..,...]........]
-00001360: cb0e b309 6624 d276 b773 f3d4 2d9a f585  ....f$.v.s..-...
-00001370: ba48 2638 2285 8fb4 de8b 3eaa 1a27 4d63  .H&8".....>..'Mc
-00001380: 651a 461e 1fe9 39ef 141f 95b8 3535 d9b7  e.F...9.....55..
-00001390: e076 1627 95d9 d596 b09b 7aef 6dbc 341d  .v.'......z.m.4.
-000013a0: 6ee7 5ed2 797b 221d 5956 4e4e 96a1 a356  n.^.y{".YVNN...V
-000013b0: d0ac afd6 0314 e2bc 150c 61ac 85af 690e  ..........a...i.
-000013c0: 5e97 baf1 c32c 86bb a150 091b f6a7 26b3  ^....,...P....&.
-000013d0: 09d7 b937 9bfe b0ac c24d 85b5 fb82 c24e  ...7.....M.....N
-000013e0: 1dc8 8554 db58 2636 34cc ab22 0458 6686  ...T.X&64..".Xf.
-000013f0: 7023 ff6a 1dcc 7a51 0ad8 487f 0329 d6d6  p#.j..zQ..H..)..
-00001400: 2118 fe36 29c0 8eae 6bc9 7048 4255 7676  !..6)...k.pHBUvv
-00001410: 69c5 dc51 1840 514a f958 1171 9044 4768  i..Q.@QJ.X.q.DGh
-00001420: c0c6 621f 83fb 75a8 823e 1195 703b 612a  ..b...u..>..p;a*
-00001430: 827e 80ab 346d 6df3 ca2d ce45 d295 2fb0  .~..4mm..-.E../.
-00001440: 0cce ae63 9627 b828 b73a 45a7 996c e126  ...c.'.(.:E..l.&
-00001450: 8f67 3298 272b ad11 0f74 f3ca 6e94 3bbf  .g2.'+...t..n.;.
-00001460: 2a26 e52f 4895 7218 ffcf 54d1 e709 5c17  *&./H.r...T...\.
-00001470: ac45 da03 21dc e40a 8c74 beb6 022e 54c2  .E..!....t....T.
-00001480: a10a e509 0d7b 022e b94c ed80 6881 eb58  .....{...L..h..X
-00001490: 780d 4105 f7c9 e6bf 2087 fabf cd39 4bc3  x.A..... ....9K.
-000014a0: a435 4c7d 6a9f c648 5038 8f54 2208 d983  .5L}j..HP8.T"...
-000014b0: b264 a2ef 1462 d5e2 ecb2 2459 41c8 4454  .d...b....$YA.DT
-000014c0: 495c 995b b107 e490 b0be ae81 0d7d b607  I\.[.........}..
-000014d0: 2881 5037 d5a4 2803 0677 32fe dce7 2283  (.P7..(..w2...".
-000014e0: 06b1 6e72 fea9 9d8f 4de6 f3b6 07ba 3bb0  ..nr....M.....;.
-000014f0: 2d96 dd7f c65e a456 2afa a5a3 a0e9 3dfb  -....^.V*.....=.
-00001500: 4c4f 352b 07af 39d8 cf79 d4da 8ab5 a0f1  LO5+..9..y......
-00001510: 6afd cc47 6d0e 973e 48ff 81f3 8f8a 90d9  j..Gm..>H.......
-00001520: 1f27 f481 dae7 fb50 5b11 fcd6 60db 2b04  .'.....P[...`.+.
-00001530: 517d c936 1e48 1748 5b1e 07d0 38d9 451b  Q}.6.H.H[...8.E.
-00001540: 4c9a 946d 588a eef6 c2db 28b8 912e 3add  L..mX.....(...:.
-00001550: 195f c8d2 37e9 74cf 69ec 5973 e6b2 7372  ._..7.t.i.Ys..sr
-00001560: f1f5 dde7 f98c 5d58 d8b1 75b9 d3f5 981a  ......]X..u.....
-00001570: 92f6 648a eaf6 683a c818 c798 5fb5 ca3f  ..d...h:...._..?
-00001580: 3cf1 c17d 70f4 365c f18f 9992 f66a ff01  <..}p.6\.....j..
-00001590: 5cf1 c194 617f 2480 e4b7 ce35 5b37 ff02  \...a.$....5[7..
-000015a0: 0000 ffff 0300 504b 0304 1400 0600 0800  ......PK........
-000015b0: 0000 2100 92e6 ccb8 1e03 0000 e808 0000  ..!.............
-000015c0: 1800 0000 786c 2f77 6f72 6b73 6865 6574  ....xl/worksheet
-000015d0: 732f 7368 6565 7431 2e78 6d6c 9c56 6b6f  s/sheet1.xml.Vko
-000015e0: da30 14fd 3e69 ff21 caf7 3c1c 4278 08a8  .0..>i.!..<.Bx..
-000015f0: 2894 b55b 274d 7b7e 368e 0356 9338 b3cd  (..['M{~6..V.8..
-00001600: a39a fadf 77ed 3c20 4d55 d122 889d e49c  ....w.< MU."....
-00001610: 73cf 8daf 2f99 5c1d b3d4 da53 2119 cfa7  s.../.\....S!...
-00001620: 3672 7ddb a239 e131 cb37 53fb d7cf 9533  6r}..9.1.7S....3
-00001630: b42d a970 1ee3 94e7 746a 3f52 695f cd3e  .-.p....tj?Ri_.>
-00001640: 7e98 1cb8 7890 5b4a 9505 0ab9 9cda 5ba5  ~...x.[J......[.
-00001650: 8ab1 e749 b2a5 1996 2e2f 680e 7712 2e32  ...I...../h.w..2
-00001660: ace0 546c 3c59 088a 6343 ca52 2ff0 fdc8  ..Tl<Y..cC.R/...
-00001670: cb30 cbed 5261 2c2e d1e0 49c2 085d 72b2  .0..Ra,...I..]r.
-00001680: cb68 ae4a 1141 53ac c0bf dcb2 42d6 6a19  .h.J.AS.....B.j.
-00001690: b944 2ec3 e261 5738 8467 0548 ac59 cad4  .D...aW8.g.H.Y..
-000016a0: a311 b5ad 8c8c ef36 3917 789d 42de 4714  .......69.x.B.G.
-000016b0: 6262 1d05 7c03 f8f5 ea30 e67a 2752 c688  bb..|....0.z'R..
-000016c0: e092 27ca 0565 aff4 dc4d 7fe4 8d3c 4c1a  ..'..e...M...<L.
-000016d0: a56e fe17 c9a0 d013 74cf f402 9ea4 82f7  .n......t.......
-000016e0: 5942 fd46 2b38 89f5 de29 1635 62fa 7189  YB.F+8...).5b.q.
-000016f0: f18e c553 fb9f 5f7d 1c18 913e f88e 8ff4  ...S.._}...>....
-00001700: e1ec f364 cf26 3183 15d6 5959 8226 537b  ...d.&1...YY.&S{
-00001710: 8ec6 f7c8 f666 1353 3fbf 193d c8b3 b9a5  .....f.S?..=....
-00001720: f0fa 074d 2951 1462 20db d2e5 b9e6 fc41  ...M)Q.b ......A
-00001730: 03ef e092 0f8a d200 b422 268a ede9 82a6  ........."&.....
-00001740: 2908 43a6 f26f 1923 d001 bc26 c2f9 bc8e  ).C..o.#...&....
-00001750: b632 05fd 4d58 6b2c e982 a77f 58ac b610  .2..MXk,....X...
-00001760: 1236 4e4c 13bc 4bd5 e9e2 d01d f602 bf87  .6NL..K.........
-00001770: 827e 73f3 3b3f dc52 b6d9 2aa0 c055 be53  .~s.;?.R..*..U.S
-00001780: 29cb e93d ddd3 1478 c6ba 29a9 71fc b8a4  )..=...x..).q...
-00001790: 9240 8d83 77d7 f822 3c05 1370 b432 a6f7  .@..w.."<..p.2..
-000017a0: 2a94 283e 96c9 961e 82f0 2c1e d949 c5b3  *.(>......,..I..
-000017b0: da9d ceab 6142 c286 09e3 a172 0f56 5e21  ....aB.....r.V^!
-000017c0: c0f2 1942 d810 02e4 a228 f423 9dd9 3362  ...B.....(.#..3b
-000017d0: 2b27 6def 3c34 c08d 128c 55e8 5794 ce89  +'m.<4....U.W...
-000017e0: 5145 84b1 265e 98ed a062 c258 3361 adde  QE..&^...b.X3a..
-000017f0: 621a 5aa0 310d 63a5 10f6 2f7b d2a3 8a09  b.Z.1.c.../{....
-00001800: e33b 63eb ba2a 9719 266f 8c8e 9a12 d11b  .;c..*..&o......
-00001810: a2aa 9137 e68e ea62 d193 cbe2 7b65 a19a  ...7...b....{e..
-00001820: 5db4 c40a cf26 821f 2ce8 6ee0 4216 58ff  ]....&..,.n.B.X.
-00001830: 57a0 b196 7bb1 d0a1 4e35 76ae c186 021b  W...{...N5v.....
-00001840: 40c2 e6dd cf46 136f 0f3b 9254 88eb 2e02  @....F.o.;.T....
-00001850: a136 64d1 850c da88 6517 316c 236e ba08  .6d.....e.1l#n..
-00001860: bf8d 58bd 60e4 19e4 d30b 90b6 c86d 1711  ..X.`........m..
-00001870: b411 775d 44bf 8df8 dc45 446d c497 2ea2  ..w]D....EDm....
-00001880: d746 408f 7dfe dcc3 06e1 c142 d63d b15c  .F@.}......B.=.\
-00001890: 59bc 537c c552 45c5 7997 3e35 fb30 0ce7  Y.S|.RE.y.>5.0..
-000018a0: c33e 9a3b bd79 b470 46c3 f0da 9987 c877  .>.;.y.pF......w
-000018b0: 4603 d41b dc84 cb55 7013 3de9 0e51 e00d  F......Up.=..Q..
-000018c0: fd8a c586 e5d2 4a69 62ba de00 ba84 287b  ......Jib.....({
-000018d0: a5ef ea13 c50b 5312 6bae a0b7 99e9 16de  ......S.k.......
-000018e0: 2828 d48b efc2 fd84 7370 529e e846 debc  ((......spR..F..
-000018f0: a3cc fe03 0000 ffff 0300 504b 0304 1400  ..........PK....
-00001900: 0600 0800 0000 2100 fd3b 0d27 ea00 0000  ......!..;.'....
-00001910: df01 0000 1400 0000 786c 2f73 6861 7265  ........xl/share
-00001920: 6453 7472 696e 6773 2e78 6d6c 7491 414b  dStrings.xmlt.AK
-00001930: 0331 1085 ef82 ff21 e46e b3f6 2022 d914  .1.....!.n.. "..
-00001940: d956 1044 04ad f7b0 9976 039b 49cc 4c4a  .V.D.....v..I.LJ
-00001950: fdf7 462a 0a92 1ee7 7d3c debc 19bd 3a86  ..F*....}<....:.
-00001960: 591c 2093 8fd8 cbeb 4527 05e0 189d c77d  Y. .....E'.....}
-00001970: 2fb7 6f0f 57b7 5210 5b74 768e 08bd fc04  /.o.W.R.[tv.....
-00001980: 922b 7379 a189 5854 2f52 2f27 e674 a714  .+sy..XT/R/'.t..
-00001990: 8d13 044b 8b98 002b d9c5 1c2c d731 ef15  ...K...+...,.1..
-000019a0: a50c d6d1 04c0 6156 cbae bb51 c17a 9462  ......aV...Q.z.b
-000019b0: 8c05 b9e6 2ea5 28e8 3f0a 0cbf 82d1 e48d  ......(.?.......
-000019c0: 66b3 39a6 9819 9cb8 67ad d868 f52d 9fd0  f.9.....g..h.-..
-000019d0: 4b8e ae8c 2c1e d7e7 c8b3 0df0 9fbd 03ba  K...,...........
-000019e0: 981b a61f d0f2 d4a4 8377 9045 3beb c45a  .........w.E;..Z
-000019f0: c6a1 166f 2fbf 4dee 0c79 f2c4 f5fe 8da8  ...o/.M..y......
-00001a00: 2122 67db 6cfc ca96 0bfd 7555 f541 e60b  !"g.l.....uU.A..
-00001a10: 0000 ffff 0300 504b 0304 1400 0600 0800  ......PK........
-00001a20: 0000 2100 bdd0 296d 5601 0000 6e02 0000  ..!...)mV...n...
-00001a30: 1100 0801 646f 6350 726f 7073 2f63 6f72  ....docProps/cor
-00001a40: 652e 786d 6c20 a204 0128 a000 0100 0000  e.xml ...(......
-00001a50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001a60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001a70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001a80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001a90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001aa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ab0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ac0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ad0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ae0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001af0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001b00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001b10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001b20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001b30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001b40: 0000 0000 0000 0000 0000 0000 0084 925f  ..............._
-00001b50: 4bc3 3014 c5df 05bf 43c9 7b9b fe99 6384  K.0.....C.{...c.
-00001b60: b603 953d 3914 9c28 be85 e476 0bb6 4948  ...=9..(...v..IH
-00001b70: a25d bfbd 69bb d50e 051f 73cf c92f e75c  .]..i.....s../.\
-00001b80: 92af 8f4d 1d7c 81b1 42c9 0225 518c 0290  ...M.|..B..%Q...
-00001b90: 4c71 21f7 057a d96d c215 0aac a392 d35a  Lq!..z.m.......Z
-00001ba0: 4928 5007 16ad cbeb ab9c 69c2 9481 27a3  I(P.......i...'.
-00001bb0: 3418 27c0 069e 242d 61ba 4007 e734 c1d8  4.'...$-a.@..4..
-00001bc0: b203 34d4 46de 21bd 5829 d350 e78f 668f  ..4.F.!.X).P..f.
-00001bd0: 3565 1f74 0f38 8de3 256e c051 4e1d c53d  5e.t.8..%n.QN..=
-00001be0: 30d4 1311 9d90 9c4d 48fd 69ea 01c0 1986  0......MH.i.....
-00001bf0: 1a1a 90ce e224 4af0 8fd7 8169 ec9f 1706  .....$J....i....
-00001c00: 65e6 6c84 ebb4 ef74 8a3b 6773 368a 93fb  e.l....t.;gs6...
-00001c10: 68c5 646c db36 6ab3 2186 cf9f e0b7 edc3  h.dl.6j.!.......
-00001c20: f350 3514 b2df 1503 54e6 9c11 6680 3a65  .P5.....T...f.:e
-00001c30: cabe bfee 8e75 8e67 c37e 8135 b56e eb77  .....u.g.~.5.n.w
-00001c40: 5d09 e0b7 5db9 15cc 28ab 2a17 3c56 9560  ]...]...(.*.<V.`
-00001c50: 10bc 5830 39fe 6df4 f0a1 cbf8 02f0 c0a7  ..X09.m.........
-00001c60: 2363 97b3 f29a dddd ef36 a84c e334 0e93  #c.......6.L.4..
-00001c70: 248c 6f76 f18a 644b 92ae defb 1c17 f7fb  $.ov..dK........
-00001c80: b4e3 a039 a5f9 9798 8659 bc4b 1664 9192  ...9.....Y.K.d..
-00001c90: 349b 11cf 8072 c87d f943 ca6f 0000 00ff  4....r.}.C.o....
-00001ca0: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
-00001cb0: 00b5 219a f690 0100 000d 0300 0010 0008  ..!.............
-00001cc0: 0164 6f63 5072 6f70 732f 6170 702e 786d  .docProps/app.xm
-00001cd0: 6c20 a204 0128 a000 0100 0000 0000 0000  l ...(..........
+000008f0: 4b03 0414 0006 0008 0000 0021 00c9 2d55  K..........!..-U
+00000900: 1fec 0200 00bd 0600 000f 0000 0078 6c2f  .............xl/
+00000910: 776f 726b 626f 6f6b 2e78 6d6c a455 df4f  workbook.xml.U.O
+00000920: db30 107e 9fb4 ff21 b378 4d1d f717 6d44  .0.~...!.xM...mD
+00000930: 8a0a 5d45 a56d aac6 80c7 ca75 5c62 e1d8  ..]E.m.....u\b..
+00000940: 99ed d020 c4ff be73 d200 a52f 0ca2 c6ce  ... ...s.../....
+00000950: e5dc cfdf dd7d e79c 9c56 b90c eeb9 b142  .....}...V.....B
+00000960: ab04 914e 8402 ae98 4e85 ba4d d0d5 9f79  ...N....N..M...y
+00000970: 3842 8175 54a5 546a c513 f4c0 2d3a 9d7c  8B.uT.Tj....-:.|
+00000980: fd72 b2d5 e66e adf5 5d00 00ca 2628 73ae  .r...n..]...&(s.
+00000990: 8831 b62c e339 b51d 5d70 059e 8d36 3975  .1.,.9..]p...69u
+000009a0: 609a 5b6c 0bc3 696a 33ce 5d2e 7137 8a86  `.[l..ij3.].q7..
+000009b0: 38a7 42a1 0621 36ef c1d0 9b8d 607c a659  8.B..!6.....`|.Y
+000009c0: 9973 e51a 10c3 2575 40df 66a2 b02d 5ace  .s....%u@.f..-Z.
+000009d0: de03 9753 7357 1621 d379 0110 6b21 857b  ...SsW.!.y..k!.{
+000009e0: a841 5190 b378 71ab b4a1 6b09 6157 6410  .AQ..xq...k.aWd.
+000009f0: 5406 7e43 b849 0443 b7dd 095c 075b e582  T.~C.I.C...\.[..
+00000a00: 196d f5c6 7500 1a37 a40f e227 1126 642f  .m..u..7...'.&d/
+00000a10: 05d5 610e de87 d4c7 86df 0b5f c367 5666  ..a........_.gVf
+00000a20: f841 56c3 67ac e10b 1889 3e8d 4640 5ab5  .AV.g.....>.F@Z.
+00000a30: 5662 48de 07d1 06cf dcba 6872 b211 925f  VbH.......hr..._
+00000a40: 37d2 0d68 51fc a2b9 af94 4481 a4d6 7d4f  7..hQ.....D...}O
+00000a50: 85e3 6982 8ec1 d45b bef7 c294 c559 2924  ..i....[.....Y)$
+00000a60: 7809 21dd 08e1 c9b3 9c97 060c a8fd 543a  x.!...........T:
+00000a70: 6e14 75fc 5c2b 0752 db51 ffac ac6a ecf3  n.u.\+.R.Q...j..
+00000a80: 4c83 8883 dffc 6f29 0c87 de01 0941 3830  L.....o).....A80
+00000a90: 5216 d3b5 5d52 9705 a591 09c2 5716 e203  R...]R......W...
+00000aa0: 8d18 4670 ab7a 8b81 93e2 cc61 d6cc a1e1  ..Fp.z.....a....
+00000ab0: 8536 ce42 729a 7953 4ac8 8df4 2db2 32b0  .6.Br.ySJ...-.2.
+00000ac0: 0b44 6f57 5228 be82 9ce4 18ee 025a 865b  .DoWR(.......Z.[
+00000ad0: 5c49 5be1 5742 a687 5df3 1f52 a6cc 6712  \I[.WB..]..R..g.
+00000ae0: 43f6 9a08 9be7 b799 8440 4ddc ca75 e94c  C........@M..u.L
+00000af0: 00cf 8bd9 0f28 d925 bd87 0282 4cd2 5d7f  .....(.%....L.].
+00000b00: 2f7c 857a 2bc5 4c4c 568f e3e1 60dc 1f1f  /|.z+.LLV...`...
+00000b10: 8fc2 d194 4cc3 6eaf 4fc2 f1a8 3f0e cfe6  ....L.n.O...?...
+00000b20: 7dd2 1ff4 cece 7add de13 0463 8631 d3b4  }.....z....c.1..
+00000b30: 74d9 4e1b 1e3a 417d 10c2 81eb 27ad 5a0f  t.N..:A}....'.Z.
+00000b40: 89e2 52a4 2f34 1ea3 dd15 faf9 cdd0 fa9e  ..R./4..........
+00000b50: 7cc0 fe14 bc16 7c6b 5f54 e4cd a0ba 112a  |.....|k_T.....*
+00000b60: d5db 04f5 46fd 08a2 7a68 ed81 b7b6 b5f3  ....F...zh......
+00000b70: 46a4 2e83 1503 58d2 bebb e0e2 3603 c6dd  F.....X.....6...
+00000b80: 88f8 85d0 2d9e 5982 f618 cd1a 4673 b842  ....-.Y.....Fs.B
+00000b90: 3fec 31c2 af28 d5e7 2d50 abe7 40d5 3d32  ?.1..(..-P..@.=2
+00000ba0: a38e c2b1 ee4f 629f 6238 ca4c ec77 308b  .....Ob.b8.L.w0.
+00000bb0: 94d4 256c ff94 f20d a826 f59d 0510 afac  ..%l.....&......
+00000bc0: 1dd0 aa92 2aef ace6 c277 8b47 5d53 cb7d  ....*....w.G]S.}
+00000bd0: c331 2a2f 5b78 8821 1369 cafd f705 4dfc  .1*/[x.!.i....M.
+00000be0: aa6f 47d3 2312 1f4d 2f8e c809 7e85 0a82  .oG.#..M/...~...
+00000bf0: d9df 1160 d8d2 047e f244 eb4e c5ed 9767  ...`...~.D.N...g
+00000c00: f20f 0000 ffff 0300 504b 0304 1400 0600  ........PK......
+00000c10: 0800 0000 2100 e4ac 1593 eb02 0000 1f07  ....!...........
+00000c20: 0000 0d00 0000 786c 2f73 7479 6c65 732e  ......xl/styles.
+00000c30: 786d 6ca4 55db 8e9b 3010 7daf d47f b0fc  xml.U...0.}.....
+00000c40: 4eb8 0448 8842 564d b248 2b6d ab4a bb95  N..H.BVM.H+m.J..
+00000c50: faea 8049 acf5 0519 2725 adfa ef1d 0321  ...I....'%.....!
+00000c60: acb6 6ab7 dbbc d81e c667 cecc 194f 9637  ..j......g...O.7
+00000c70: 8de0 e844 75cd 944c b13f f130 a232 5705  ...Du..L.?.0.2W.
+00000c80: 93fb 147f 79cc 9c39 46b5 21b2 205c 499a  ....y..9F.!. \I.
+00000c90: e233 adf1 cdea fdbb 656d ce9c 3e1c 2835  .3......em..>.(5
+00000ca0: 0820 649d e283 31d5 c275 ebfc 4005 a927  . d...1..u..@..'
+00000cb0: aaa2 12be 944a 0b62 e0a8 f76e 5d69 4a8a  .....J.b...n]iJ.
+00000cc0: da5e 12dc 0d3c 2f76 0561 1277 080b 91bf  .^...</v.a.w....
+00000cd0: 0644 10fd 74ac 9c5c 898a 18b6 639c 9973  .D..t..\....c..s
+00000ce0: 8b85 91c8 1777 7ba9 34d9 71a0 daf8 21c9  .....w{.4.q...!.
+00000cf0: 51e3 c73a 408d be04 69ad 2fe2 0896 6b55  Q..:@...i./...kU
+00000d00: abd2 4c00 d755 65c9 72fa 926e e226 2ec9  ..L..Ue.r..n.&..
+00000d10: af48 80fc 3624 3f72 bde0 59ee 8d7e 2352  .H..6$?r..Y..~#R
+00000d20: e86a 7a62 563e bc5a 964a 9a1a e5ea 280d  .jzbV>.Z.J....(.
+00000d30: 8809 446d 0916 4f52 7d93 99fd 648d 9dd7  ..Dm..OR}...d...
+00000d40: 6a59 7f47 27c2 c1e2 6377 b5cc 1557 1a19  jY.G'...cw...W..
+00000d50: 900e 2ad7 5a24 11b4 f3d8 10ce 769a 59b7  ..*.Z$......v.Y.
+00000d60: 9208 c6cf 9d39 b086 56ed de4f 30a8 bd35  .....9..V..O0..5
+00000d70: ba96 47bf d470 8971 3eb0 9a5a 0260 582d  ..G..p.q>..Z.`X-
+00000d80: 413e 43b5 cce0 80fa fde3 b982 f012 3aad  A>C...........:.
+00000d90: 8369 fdfe e2bd d7e4 ec07 d1eb 2fd4 8ab3  .i........../...
+00000da0: c2b2 d86f c649 43e7 1b66 ebe6 7893 204c  ...o.IC..f..x. L
+00000db0: 92d9 ccb7 bfd9 3c99 5aec 5def cd64 411b  ......<.Z.]..dA.
+00000dc0: 5aa4 380e db90 a32c 6cc6 2de3 7681 c477  Z.8....,l.-.v..w
+00000dd0: 4a17 f0b4 ae82 5c4c ab25 a7a5 0154 cdf6  J.....\L.%...T..
+00000de0: 07bb 1a55 d918 ca18 68bf d5b2 6064 af24  ...U....h...`d.$
+00000df0: e1b6 961d c8b0 01d8 9c72 fe60 9fdf d7f2  .........r.`....
+00000e00: 1976 5322 7914 9930 7740 0fd2 b12a 5cb6  .vS"y..0w@...*\.
+00000e10: c0ab df76 78dd c1e2 8fd1 3aec 116c 0075  ...vx.....:..l.u
+00000e20: fa77 58d4 9403 fe2b 6e07 188d 490d b711  .wX....+n...I...
+00000e30: a92a 7eb6 fdd1 b764 cb15 d88d 4af0 ac00  .*~....d....J...
+00000e40: 432a c836 6f8a 3fd9 d9c3 e119 f474 d0ee  C*.6o.?......t..
+00000e50: c838 88fc 9be4 01b3 68ae e5f4 acb6 c6ce  .8......h.......
+00000e60: 91b6 d043 14a8 6a41 4b72 e4e6 71f8 98e2  ...C..jAKr..q...
+00000e70: ebfe 232d d851 2483 d767 7652 a685 48f1  ..#-.Q$..gvR..H.
+00000e80: 757f 6f55 f763 1b83 36e6 be86 b702 2b3a  u.oU.c..6.....+:
+00000e90: 6a96 e21f b7eb 59b2 bdcd 0267 eead e74e  j.....Y....g...N
+00000ea0: 38a5 9193 44eb ad13 859b f576 9b25 5ee0  8...D......v.%^.
+00000eb0: 6d7e 8ea6 d97f ccb2 76f8 82c0 7eb8 a839  m~......v...~..9
+00000ec0: 4c3c dd27 dba7 f870 b5a5 7874 e8e8 b7dd  L<.'...p..xt....
+00000ed0: 0fb4 c7dc 9320 f63e 44be e764 53cf 77c2  ..... .>D..dS.w.
+00000ee0: 98cc 9d79 3c8d 9c2c f283 6d1c ae6f a32c  ...y<..,..m..o.,
+00000ef0: 1a71 8fde 38f3 3cd7 f7bb e969 c947 0bc3  .q..8.<....i.G..
+00000f00: 04e5 4c5e b4ba 2834 b682 4870 fc43 12ee  ..L^..(4..Hp.C..
+00000f10: 4509 f7fa cfb6 fa05 0000 ffff 0300 504b  E.............PK
+00000f20: 0304 1400 0600 0800 0000 2100 e9a6 25b8  ..........!...%.
+00000f30: 6606 0000 531b 0000 1300 0000 786c 2f74  f...S.......xl/t
+00000f40: 6865 6d65 2f74 6865 6d65 312e 786d 6cec  heme/theme1.xml.
+00000f50: 59cd 6e1b 3710 be17 e83b 107b 4f2c d992  Y.n.7....;.{O,..
+00000f60: 6219 9103 4b96 e236 7162 d84a 8a1c a95d  b...K..6qb.J...]
+00000f70: 6a97 1177 b920 293b ba15 c9b1 4081 a269  j..w. );....@..i
+00000f80: d14b 81de 7a28 da06 4880 5ed2 a771 9ba2  .K..z(..H.^..q..
+00000f90: 4d81 bc42 87e4 4a5a 5a54 6c27 06fa 171d  M..B..JZZTl'....
+00000fa0: 6c2d f7e3 fccf 7086 ba7a ed41 cad0 2111  l-....p..z.A..!.
+00000fb0: 92f2 ac15 542f 5702 44b2 9047 348b 5bc1  ....T/W.D..G4.[.
+00000fc0: 9d7e efd2 7a80 a4c2 5984 19cf 482b 9810  .~..z...Y...H+..
+00000fd0: 195c db7c ffbd ab78 4325 2425 08f6 6772  .\.|...xC%$%..gr
+00000fe0: 03b7 8244 a97c 6365 4586 b08c e565 9e93  ...D.|ceE....e..
+00000ff0: 0cde 0db9 48b1 8247 11af 4402 1f01 dd94  ....H..G..D.....
+00001000: adac 562a 8d95 14d3 2c40 194e 81ec ede1  ..V*....,@.N....
+00001010: 9086 04f5 35c9 6073 4abc cbe0 3153 522f  ....5.`sJ...1SR/
+00001020: 844c 1c68 d2c4 d961 b0d1 a8aa 1172 223b  .L.h...a.....r";
+00001030: 4ca0 43cc 5a01 f089 f851 9f3c 5001 6258  L.C.Z....Q.<P.bX
+00001040: 2a78 d10a 2ae6 13ac 6c5e 5dc1 1bc5 26a6  *x..*...l^]...&.
+00001050: 96ec 2ded eb99 4fb1 afd8 108d 560d 4f11  ..-...O.....V.O.
+00001060: 0f66 4cab bd5a f3ca f68c be01 30b5 88eb  .fL..Z......0...
+00001070: 76bb 9d6e 7546 cf00 7018 82a6 5696 32cd  v..nuF..p...V.2.
+00001080: 5a6f bdda 9ed2 2c81 ecd7 45da 9d4a bd52  Zo....,...E..J.R
+00001090: 73f1 25fa 6b0b 3237 dbed 76bd 59c8 6289  s.%.k.27..v.Y.b.
+000010a0: 1a90 fd5a 5bc0 af57 1ab5 ad55 076f 4016  ...Z[..W...U.o@.
+000010b0: 5f5f c0d7 da5b 9d4e c3c1 1b90 c537 16f0  __...[.N.....7..
+000010c0: bd2b cd46 cdc5 1b50 c268 365a 406b 87f6  .+.F...P.h6Z@k..
+000010d0: 7a05 f519 64c8 d98e 17be 0ef0 f54a 019f  z...d........J..
+000010e0: a320 1a66 d1a5 590c 79a6 96c5 5a8a ef73  . .f..Y.y...Z..s
+000010f0: d103 8006 32ac 6886 d424 2743 1c42 1477  ....2.h..$'C.B.w
+00001100: 703a 1014 6b06 7883 e0d2 1bbb 14ca 8525  p:..k.x........%
+00001110: cd0b c950 d05c b582 0f73 0c19 31a7 f7ea  ...P.\...s..1...
+00001120: f9f7 af9e 3f45 af9e 3f39 7ef8 ecf8 e14f  ....?E..?9~....O
+00001130: c78f 1e1d 3ffc d1d2 7236 eee0 2c2e 6f7c  ....?...r6..,.o|
+00001140: f9ed 677f 7efd 31fa e3e9 372f 1f7f e1c7  ..g.~.1...7/....
+00001150: cb32 fed7 1f3e f9e5 e7cf fd40 c8a0 b944  .2...>.....@...D
+00001160: 2fbe 7cf2 dbb3 272f befa f4f7 ef1e 7be0  /.|...'/......{.
+00001170: 5b02 0fca f03e 4d89 44b7 c811 dae7 29e8  [....>M.D.....).
+00001180: 660c e34a 4e06 e27c 3bfa 09a6 ce0e 9c00  f..JN..|;.......
+00001190: 6d0f e9ae 4a1c e0ad 0966 3e5c 9bb8 c6bb  m...J....f>\....
+000011a0: 2ba0 78f8 80d7 c7f7 1d59 0f12 3156 d4c3  +.x......Y..1V..
+000011b0: f946 923a c05d ce59 9b0b af01 6e68 5e25  .F.:.].Y....nh^%
+000011c0: 0bf7 c759 ec67 2ec6 65dc 3ec6 873e de1d  ...Y.g..e.>..>..
+000011d0: 9c39 aeed 8e73 a89a d3a0 746c df49 8823  .9...s....tl.I.#
+000011e0: e61e c399 c231 c988 42fa 1d1f 11e2 d1ee  .....1..B.......
+000011f0: 1ea5 8e5d 7769 28b8 e443 85ee 51d4 c6d4  ...]wi(..C..Q...
+00001200: 6b92 3e1d 3881 34df b443 53f0 cbc4 a733  k.>.8.4..CS....3
+00001210: b8da b1cd ee5d d4e6 cca7 f536 3974 9190  .....].....69t..
+00001220: 1098 7984 ef13 e698 f13a 1e2b 9cfa 48f6  ..y......:.+..H.
+00001230: 71ca ca06 bf89 55e2 13f2 6022 c232 ae2b  q.....U...`".2.+
+00001240: 1578 3a26 8ca3 6e44 a4f4 edb9 2d40 df92  .x:&..nD....-@..
+00001250: d36f 60a8 575e b7ef b249 ea22 85a2 231f  .o`.W^...I."..#.
+00001260: cd9b 98f3 3272 9b8f 3a09 4e73 afcc 344b  ....2r..:.Ns..4K
+00001270: cad8 0fe4 0842 14a3 3dae 7cf0 5dee 6688  .....B..=.|.].f.
+00001280: 7e06 3fe0 6ca9 bbef 52e2 b8fb f442 7087  ~.?.l...R....Bp.
+00001290: c68e 48f3 00d1 6fc6 a2a8 da4e fd4d 69f6  ..H...o....N.Mi.
+000012a0: ba62 cc28 54e3 77c5 787a 3a6d c1d1 e44b  .b.(T.w.xz:m...K
+000012b0: 899d 1325 7819 ee5f 5878 b7f1 38db 2310  ...%x.._Xx..8.#.
+000012c0: eb8b 07cf bbba fbae ee06 fff9 babb 2c97  ..............,.
+000012d0: cf5a 6de7 0516 9ae4 795f 6cba e474 6993  .Zm.....y_l..ti.
+000012e0: 3ca4 8c1d a809 2337 a5e9 9325 1c16 510f  <.....#7...%..Q.
+000012f0: 164d 036f a6b8 d9d0 9427 f0b5 28ee 0e2e  .M.o.....'..(...
+00001300: 16d8 ec41 82ab 8fa8 4a0e 129c 438f 5d35  ...A....J...C.]5
+00001310: 235f 2c0b d2b1 4439 9730 db99 6533 7c92  #_,...D9.0..e3|.
+00001320: 13b4 cd38 49a1 cd36 9361 5dcf 0cb6 1e48  ...8I..6.a]....H
+00001330: ac76 7964 97d7 cab3 e18c 8c99 1463 337f  .vyd.........c3.
+00001340: 4e19 ad69 0267 65b6 76e5 ed98 55ad 544b  N..i.ge.v...U.TK
+00001350: cde6 aa56 35a2 9952 e7a8 3653 197c b8a8  ...V5..R..6S.|..
+00001360: 1a2c ceac 095d 0882 de05 acdc 8011 5dcb  .,...]........].
+00001370: 0eb3 0966 24d2 76b7 73f3 d42d 9af5 85ba  ...f$.v.s..-....
+00001380: 4826 3822 858f b4de 8b3e aa1a 274d 6365  H&8".....>..'Mce
+00001390: 1a46 1e1f e939 ef14 1f95 b835 35d9 b7e0  .F...9.....55...
+000013a0: 7616 2795 d9d5 96b0 9b7a ef6d bc34 1d6e  v.'......z.m.4.n
+000013b0: e75e d279 7b22 1d59 564e 4e96 a1a3 56d0  .^.y{".YVNN...V.
+000013c0: acaf d603 14e2 bc15 0c61 ac85 af69 0e5e  .........a...i.^
+000013d0: 97ba f1c3 2c86 bba1 5009 1bf6 a726 b309  ....,...P....&..
+000013e0: d7b9 379b feb0 acc2 4d85 b5fb 82c2 4e1d  ..7.....M.....N.
+000013f0: c885 54db 5826 3634 ccab 2204 5866 8670  ..T.X&64..".Xf.p
+00001400: 23ff 6a1d cc7a 510a d848 7f03 29d6 d621  #.j..zQ..H..)..!
+00001410: 18fe 3629 c08e ae6b c970 4842 5576 7669  ..6)...k.pHBUvvi
+00001420: c5dc 5118 4051 4af9 5811 7190 4447 68c0  ..Q.@QJ.X.q.DGh.
+00001430: c662 1f83 fb75 a882 3e11 9570 3b61 2a82  .b...u..>..p;a*.
+00001440: 7e80 ab34 6d6d f3ca 2dce 45d2 952f b00c  ~..4mm..-.E../..
+00001450: ceae 6396 27b8 28b7 3a45 a799 6ce1 268f  ..c.'.(.:E..l.&.
+00001460: 6732 9827 2bad 110f 74f3 ca6e 943b bf2a  g2.'+...t..n.;.*
+00001470: 26e5 2f48 9572 18ff cf54 d1e7 095c 17ac  &./H.r...T...\..
+00001480: 45da 0321 dce4 0a8c 74be b602 2e54 c2a1  E..!....t....T..
+00001490: 0ae5 090d 7b02 2eb9 4ced 8068 81eb 5878  ....{...L..h..Xx
+000014a0: 0d41 05f7 c9e6 bf20 87fa bfcd 394b c3a4  .A..... ....9K..
+000014b0: 354c 7d6a 9fc6 4850 388f 5422 08d9 83b2  5L}j..HP8.T"....
+000014c0: 64a2 ef14 62d5 e2ec b224 5941 c844 5449  d...b....$YA.DTI
+000014d0: 5c99 5bb1 07e4 90b0 beae 810d 7db6 0728  \.[.........}..(
+000014e0: 8150 37d5 a428 0306 7732 fedc e722 8306  .P7..(..w2..."..
+000014f0: b16e 72fe a99d 8f4d e6f3 b607 ba3b b02d  .nr....M.....;.-
+00001500: 96dd 7fc6 5ea4 562a faa5 a3a0 e93d fb4c  ....^.V*.....=.L
+00001510: 4f35 2b07 af39 d8cf 79d4 da8a b5a0 f16a  O5+..9..y......j
+00001520: fdcc 476d 0e97 3e48 ff81 f38f 8a90 d91f  ..Gm..>H........
+00001530: 27f4 81da e7fb 505b 11fc d660 db2b 0451  '.....P[...`.+.Q
+00001540: 7dc9 361e 4817 485b 1e07 d038 d945 1b4c  }.6.H.H[...8.E.L
+00001550: 9a94 6d58 8aee f6c2 db28 b891 2e3a dd19  ..mX.....(...:..
+00001560: 5fc8 d237 e974 cf69 ec59 73e6 b273 72f1  _..7.t.i.Ys..sr.
+00001570: f5dd e7f9 8c5d 58d8 b175 b9d3 f598 1a92  .....]X..u......
+00001580: f664 8aea f668 3ac8 18c7 985f b5ca 3f3c  .d...h:...._..?<
+00001590: f1c1 7d70 f436 5cf1 8f99 92f6 6aff 015c  ..}p.6\.....j..\
+000015a0: f1c1 9461 7f24 80e4 b7ce 355b 37ff 0200  ...a.$....5[7...
+000015b0: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
+000015c0: 0021 00af 3b1e 8da1 0400 0009 1100 0018  .!..;...........
+000015d0: 0000 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
+000015e0: 2f73 6865 6574 312e 786d 6cac 955b 6f9b  /sheet1.xml..[o.
+000015f0: 3014 c7df 27ed 3b20 bf07 b049 b324 0aad  0...'.; ...I.$..
+00001600: aa56 552b ed61 5a77 7976 8c93 5835 38b3  .VU+.aZwyv..X58.
+00001610: 9d4b 35ed bbef 1830 a1cb 9a06 b628 8113  .K5....0.....(..
+00001620: c3f9 9fdb 0f33 bbda e732 d872 6d84 2a52  .....3...2.rm.*R
+00001630: 84c3 1805 bc60 2a13 c532 455f bfdc 0dc6  .....`*..2E_....
+00001640: 2830 9616 1995 aae0 297a e606 5d5d be7f  (0......)z..]]..
+00001650: 37db 29fd 6456 9cdb 0014 0a93 a295 b5eb  7.).dV..........
+00001660: 6914 19b6 e239 35a1 5af3 02ae 2c94 cea9  i....95.Z...,...
+00001670: 85bf 7a19 99b5 e634 2b9d 7219 9138 1e45  ..z....4+.r..8.E
+00001680: 3915 05aa 14a6 fa1c 0db5 5808 c66f 15db  9.........X..o..
+00001690: e4bc b095 88e6 925a c8df acc4 da78 b59c  .......Z.....x..
+000016a0: 9d23 9753 fdb4 590f 98ca d720 3117 52d8  .#.S..Y.... 1.R.
+000016b0: e752 1405 399b 3e2c 0ba5 e95c 42dd 7b3c  .R..9.>,...\B.{<
+000016c0: a42c d86b f812 f825 3e4c b97e 1429 174c  .,.k...%>L.~.).L
+000016d0: 2ba3 1636 04e5 a8ca f9b8 fc49 3489 286b  +..6.......I4.(k
+000016e0: 948e eb3f 4b06 0f23 cdb7 c20d f020 45fa  ...?K..#..... E.
+000016f0: a584 2f1a 2d72 104b 7a8a 8d1a 31d7 2e3d  ../.-r.Kz...1..=
+00001700: dd88 2c45 3fe3 fa33 8033 7687 7810 6377  ..,E?..3.3v.x.cw
+00001710: 687d 7ea1 cb59 2660 c2ae aa40 f345 8aae  h}~..Y&`...@.E..
+00001720: f1f4 fa1e a3e8 7256 02f4 4df0 9d69 d981  ......rV..M..i..
+00001730: a5f3 472e 39b3 1c82 6014 383e e74a 3db9  ..G.9...`.8>.J=.
+00001740: 1b1f 6029 0649 53de e024 29b3 62cb 6fb8  ..`).IS..$).b.o.
+00001750: 9429 ba81 52cd 8f32 0898 1020 6a22 b46d  .)..R..2... j".m
+00001760: 1fed ae24 fa93 0ee6 d4f0 1b25 bf8b ccae  ...$.......%....
+00001770: 2024 3c39 195f d08d b487 c571 384e 489c   $<9._.....q8NH.
+00001780: 6072 d15c fcac 76f7 5c2c 5716 5c60 556d  `r.\..v.\,W.\`Um
+00001790: ac14 05ff c8b7 5c82 5f99 7ac9 d434 7bbe  ......\._.z..4{.
+000017a0: e586 01e4 907b 58e6 c594 8424 e018 e4c2  .....{X....$....
+000017b0: 3dac c028 dd57 c5d6 39c0 c3ca 36c6 aadc  =..(.W..9...6...
+000017c0: 27e5 ca69 1ca0 ced2 01a6 b1ab 1d20 8313  '..i......... ..
+000017d0: 0ec3 da01 eeaa 1d08 0ef1 6818 8f5c 417f  ..........h..\A.
+000017e0: 38be 28c5 65d5 0e3d aa95 e0fc b652 dbf1  8.(.e..=.....R..
+000017f0: 43ed 0867 ef08 8dee 121a 7a52 560d e75a  C..g......zRV..Z
+00001800: 6178 d11a 4b17 a989 ef38 a4f0 7a07 4f36  ax..K....8..z.O6
+00001810: 0237 5373 8c56 53e8 9d0f f613 75c6 7923  .7Ss.VS.....u.y#
+00001820: c530 fc8a 9a16 05c7 1d6d 8f00 7b0c 9ce1  .0.......m..{...
+00001830: a34c c2a4 21bb 4b0b 1df3 55fc 0354 fdeb  .L..!.K...U..T..
+00001840: f758 e116 576f 14e3 81c2 07a2 70ef 623c  .X..Wo......p.b<
+00001850: 5bf8 3fc0 851b bac0 789d f517 0f34 d45a  [.?.....x....4.Z
+00001860: 3693 b480 ec5b 0cf1 643a e35f c924 9e4c  6....[..d:._.$.L
+00001870: 679c 598c 2793 1cc8 7475 75a1 8b78 549d  g.Y.'...tuu..xT.
+00001880: 7146 0d2f 9ae9 c974 7b5b cfbd 8678 209d  qF./...t{[...x .
+00001890: d135 be27 93f4 dfeb 8807 d219 5de3 7bfe  .5.'........].{.
+000018a0: 488b bfbe 3b65 e2c9 74c6 79f3 4f3c 7fce  H...;e..t.y.O<..
+000018b0: f0db 0c8c f1c4 fb29 69de 6827 f7bf 931b  .......)i.h'....
+000018c0: 72e2 b173 46c7 9625 1e37 67f8 94c7 e15f  r..sF..%.7g...._
+000018d0: 5faa 51f9 f6fe 0d00 00ff ff00 0000 ffff  _.Q.............
+000018e0: 6cd4 d96a c330 1005 d05f 31fa 803a 63b9  l..j.0..._1..:c.
+000018f0: 5b50 0c6a dd7d df97 37e3 1afa 9496 c8a4  [P.j.}..7.......
+00001900: eddf 5729 8530 77ee 9b11 c723 e60e a390  ..W).0w....#....
+00001910: de87 616c bbb1 6bc2 e2e3 ab58 cc9c b822  ..al..k....X..."
+00001920: 7d76 f394 bfa6 be76 c5b7 d45d 3f7d fb69  }v.....v...]?}.i
+00001930: 87d4 0ff3 71e6 261b 956b 42bf b271 85ff  ....q.&..kB..q..
+00001940: 7ec9 e729 9f2e 9b49 2897 4d28 fb7f b167  ~..)...I(.M(...g
+00001950: 8568 b16f 4505 455a 4b3c 5439 20a4 d217  .h.oE.EZK<T9 ...
+00001960: 1d92 8bb4 3822 45b4 38b6 a2d6 e2c4 8a4d  ....8"E.8......M
+00001970: 2d4e add8 d2e2 cc8a 6d2d cead d8d1 e2c2  -N......m-......
+00001980: 8a5d 2d2e c968 20f8 2b42 20f8 6b42 20f8  .]-..h .+B .kB .
+00001990: 1b12 3c54 b925 04aa dc11 e275 47f7 84c0  ..<T.%.....uG...
+000019a0: 781e 0881 f93c 1202 037a 2204 d27d b6c4  x....<...z"..}..
+000019b0: 43ba 2fa4 0acc f995 1018 7424 4b28 104c  C./.......t$K(.L
+000019c0: 646b 08c9 44b2 8802 d144 b289 02d9 44b2  dk..D....D....D.
+000019d0: 8a02 6d45 b28b 827d 916d 1408 3992 7df4  ..mE...}.m..9.}.
+000019e0: ebde cbfc a4e5 b768 fdc6 fd02 0000 ffff  .......h........
+000019f0: 0000 00ff ff3c 8e5d 0b82 3018 46ff cad8  .....<.]..0.F...
+00001a00: fdd2 e5fc c409 ab94 6efa 110b dfe9 c89a  ........n.......
+00001a10: cc57 0aa2 ffde 2ae8 ee39 7038 3cb5 5ed1  .W....*..9p8<.^.
+00001a20: 7576 42f0 c483 9154 f14a 1d39 250f 5fad  uvB....T.J.9%._.
+00001a30: b697 f429 8450 45ca 154b 54b6 6765 2176  ...).PE..KT.ge!v
+00001a40: 4c09 1eb3 32e7 49de 8a43 b76d b317 8d9a  L...2.I..C.m....
+00001a50: 7ad6 039c b41f ec6d 2113 1894 34de e429  z......m!...4..)
+00001a60: 25de 0ee3 1fd0 cd92 86fc d921 baeb 778e  %..........!..w.
+00001a70: a07b f01f 3bc8 c6b9 70e5 07a1 19dd 9dbf  .{..;...p.......
+00001a80: 2c23 0036 6f00 0000 ffff 0300 504b 0304  ,#.6o.......PK..
+00001a90: 1400 0600 0800 0000 2100 546e 48d2 6b01  ........!.TnH.k.
+00001aa0: 0000 4b04 0000 1400 0000 786c 2f73 6861  ..K.......xl/sha
+00001ab0: 7265 6453 7472 696e 6773 2e78 6d6c 7c94  redStrings.xml|.
+00001ac0: cb4e c330 1045 f748 fc83 e53d a404 8410  .N.0.E.H...=....
+00001ad0: 4a82 2a1e 8205 a540 cade c403 b514 dbc1  J.*....@........
+00001ae0: 33ae dabf c77d 4a84 6997 b947 737d 3d33  3....}J.i..Gs}=3
+00001af0: 4e71 33b7 ad98 4140 e35d 29cf 4e07 5280  Nq3...A@.]).N.R.
+00001b00: 6bbc 36ee bb94 93fa e1e4 4a0a 24e5 b46a  k.6.......J.$..j
+00001b10: bd83 522e 00e5 4d75 7c54 2092 48b5 0e4b  ..R...Mu|T .H..K
+00001b20: 3925 eaae b30c 9b29 5885 a7be 0397 c897  9%.....)X.......
+00001b30: 0f56 51fa 0cdf 1976 0194 c629 00d9 36cb  .VQ....v...)..6.
+00001b40: 0783 cbcc 2ae3 a468 7c74 54ca f30b 29a2  ....*..h|tT...).
+00001b50: 333f 116e 7742 55a0 a90a aade 20c9 e9b0  3?.nwBU..... ...
+00001b60: a7bb 22a3 aac8 96ea 5f52 2f3a e8b3 fb79  .."....._R/:...y
+00001b70: e703 8116 43ea a327 02cb b8ad e491 b2ff  ....C..'........
+00001b80: ac56 803b 6305 26ce 9078 f912 1614 c6c0  .V.;c.&..x......
+00001b90: 173f 8f47 6c88 3104 e375 1fbd 46e5 c8d0  .?.Gl.1..u..F...
+00001ba0: a2af df46 246f 2130 d977 88cb bf83 f773  ...F$o!0.w.....s
+00001bb0: 82e0 54cb 188c 83d7 b1e1 9abc 259c f310  ..T.........%...
+00001bc0: 11b8 9ab5 7ee0 b83a 2887 aaa1 b474 82eb  ....~..:(....t..
+00001bd0: ec63 fc64 422e 552e c676 43de 4951 c47e  .c.dB.U..vC.IQ.~
+00001be0: db6a 935a 76c6 d86d 00e7 b841 876e b074  .j.Zv..m...A.n.t
+00001bf0: cdf7 b9e6 6cce 956b 2e0e b87e 80d3 9e1b  ....l..k...~....
+00001c00: f006 7059 d380 6646 a734 fc58 d78c dd8b  ..pY..fF.4.X....
+00001c10: f426 f917 32e9 f41e b29e 6cbf d159 fa19  .&..2.....l..Y..
+00001c20: 54bf 0000 00ff ff03 0050 4b03 0414 0006  T........PK.....
+00001c30: 0008 0000 0021 00ad bc57 c556 0100 006e  .....!...W.V...n
+00001c40: 0200 0011 0008 0164 6f63 5072 6f70 732f  .......docProps/
+00001c50: 636f 7265 2e78 6d6c 20a2 0401 28a0 0001  core.xml ...(...
+00001c60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001c70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001c80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001c90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ca0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001cb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001cc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001cd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ce0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001cf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001d60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001d70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001d80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001d90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001da0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001db0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001dc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001dd0: 0000 0000 0000 0000 009c 9241 6edb 3010  ...........An.0.
-00001de0: 45f7 0572 0782 fb98 7212 0485 4131 2892  E..r....r...A1(.
-00001df0: 065e 34a8 013b d94f a991 c596 2605 722c  .^4..;.O....&.r,
-00001e00: d8bd 4dcf d28b 7524 218e dc74 d5dd 70e6  ..M...u$!..t..p.
-00001e10: f3f3 f193 faee b0f3 a2c3 945d 0ca5 9ccf  ...........]....
-00001e20: 0a29 30d8 58b9 b02d e5f3 e6f1 f2a3 1499  .)0.X..-........
-00001e30: 2054 e063 c052 1e31 cb3b 73f1 41af 526c   T.c.R.1.;s.A.Rl
-00001e40: 3191 c32c d822 e452 3644 ed42 a96c 1bdc  1..,.".R6D.B.l..
-00001e50: 419e f138 f0a4 8e69 07c4 cbb4 55b1 ae9d  A..8...i....U...
-00001e60: c587 68f7 3b0c a4ae 8ae2 56e1 8130 5458  ..h.;.....V..0TX
-00001e70: 5db6 2743 393a 2e3a fa5f d32a da9e 2fbf  ].'C9:.:._.*../.
-00001e80: 6c8e 2d03 1bfd a96d bdb3 407c 4bf3 e46c  l.-....m..@|K..l
-00001e90: 8a39 d624 9ec0 ba40 3137 e2f3 c1a2 d76a  .9.$...@17.....j
-00001ea0: 2ad3 ccb9 46bb 4f8e 8ea6 d06a bad4 6b0b  *...F.O....j..k.
-00001eb0: 1eef f908 5383 cfa8 d55b 432f 11fa f856  ....S....[C/...V
-00001ec0: e052 36ba a345 8796 6212 d9fd e400 afa4  .R6..E..b.......
-00001ed0: f806 197b b052 7690 1c04 62c0 5e36 2e86  ...{.Rv...b.^6..
-00001ee0: dab7 9992 59c6 ef90 4585 c2fe fee5 edde  ....Y...E.......
-00001ef0: 47ad 5837 ce86 72ba 655a bb1b 331f 045c  G.X7..r.eZ..3..\
-00001f00: 9c0b 7b83 9187 07e7 a41b 471e f3d7 7a05  ..{.......G...z.
-00001f10: 89fe 013e 9f82 0f0c 23f6 88f3 0004 efe8  ...>....#.......
-00001f20: 867b f339 7f39 7f71 e147 7e6e 3791 37e1  .{.9.9.q.G~n7.7.
-00001f30: 6b80 e74d bd6e 2061 c599 9f02 3e35 f492  k..M.n a....>5..
-00001f40: b34b be37 b96f 206c b17a d5bc 1ff4 0fff  .K.7.o l.z......
-00001f50: 32fe 6e33 bf9d 15d7 05bf e4a4 a7d5 db3f  2.n3...........?
-00001f60: 367f 0000 00ff ff03 0050 4b01 022d 0014  6........PK..-..
-00001f70: 0006 0008 0000 0021 0062 ee9d 685e 0100  .......!.b..h^..
-00001f80: 0090 0400 0013 0000 0000 0000 0000 0000  ................
-00001f90: 0000 0000 0000 005b 436f 6e74 656e 745f  .......[Content_
-00001fa0: 5479 7065 735d 2e78 6d6c 504b 0102 2d00  Types].xmlPK..-.
-00001fb0: 1400 0600 0800 0000 2100 b555 3023 f400  ........!..U0#..
-00001fc0: 0000 4c02 0000 0b00 0000 0000 0000 0000  ..L.............
-00001fd0: 0000 0000 9703 0000 5f72 656c 732f 2e72  ........_rels/.r
-00001fe0: 656c 7350 4b01 022d 0014 0006 0008 0000  elsPK..-........
-00001ff0: 0021 0081 3e94 97f3 0000 00ba 0200 001a  .!..>...........
-00002000: 0000 0000 0000 0000 0000 0000 00bc 0600  ................
-00002010: 0078 6c2f 5f72 656c 732f 776f 726b 626f  .xl/_rels/workbo
-00002020: 6f6b 2e78 6d6c 2e72 656c 7350 4b01 022d  ok.xml.relsPK..-
-00002030: 0014 0006 0008 0000 0021 0091 d238 c2dd  .........!...8..
-00002040: 0200 00b7 0600 000f 0000 0000 0000 0000  ................
-00002050: 0000 0000 00ef 0800 0078 6c2f 776f 726b  .........xl/work
-00002060: 626f 6f6b 2e78 6d6c 504b 0102 2d00 1400  book.xmlPK..-...
-00002070: 0600 0800 0000 2100 e4ac 1593 eb02 0000  ......!.........
-00002080: 1f07 0000 0d00 0000 0000 0000 0000 0000  ................
-00002090: 0000 f90b 0000 786c 2f73 7479 6c65 732e  ......xl/styles.
-000020a0: 786d 6c50 4b01 022d 0014 0006 0008 0000  xmlPK..-........
-000020b0: 0021 00e9 a625 b866 0600 0053 1b00 0013  .!...%.f...S....
-000020c0: 0000 0000 0000 0000 0000 0000 000f 0f00  ................
-000020d0: 0078 6c2f 7468 656d 652f 7468 656d 6531  .xl/theme/theme1
-000020e0: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
-000020f0: 0000 2100 92e6 ccb8 1e03 0000 e808 0000  ..!.............
-00002100: 1800 0000 0000 0000 0000 0000 0000 a615  ................
-00002110: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
-00002120: 7368 6565 7431 2e78 6d6c 504b 0102 2d00  sheet1.xmlPK..-.
-00002130: 1400 0600 0800 0000 2100 fd3b 0d27 ea00  ........!..;.'..
-00002140: 0000 df01 0000 1400 0000 0000 0000 0000  ................
-00002150: 0000 0000 fa18 0000 786c 2f73 6861 7265  ........xl/share
-00002160: 6453 7472 696e 6773 2e78 6d6c 504b 0102  dStrings.xmlPK..
-00002170: 2d00 1400 0600 0800 0000 2100 bdd0 296d  -.........!...)m
-00002180: 5601 0000 6e02 0000 1100 0000 0000 0000  V...n...........
-00002190: 0000 0000 0000 161a 0000 646f 6350 726f  ..........docPro
-000021a0: 7073 2f63 6f72 652e 786d 6c50 4b01 022d  ps/core.xmlPK..-
-000021b0: 0014 0006 0008 0000 0021 00b5 219a f690  .........!..!...
-000021c0: 0100 000d 0300 0010 0000 0000 0000 0000  ................
-000021d0: 0000 0000 00a3 1c00 0064 6f63 5072 6f70  .........docProp
-000021e0: 732f 6170 702e 786d 6c50 4b05 0600 0000  s/app.xmlPK.....
-000021f0: 000a 000a 0080 0200 0069 1f00 0000 00    .........i.....
+00001d60: 7c92 514f c320 1485 df4d fc0f 0def 2db4  |.QO. ...M....-.
+00001d70: 8b73 236d 97a8 d993 8b26 6ed1 f846 e076  .s#m.....&n..F.v
+00001d80: 23b6 4000 ddf6 efa5 ed56 bb68 7ce4 9ec3  #.@......V.h|...
+00001d90: c739 37e4 8b43 5347 5f60 9dd4 aa40 6942  .97..CSG_`...@iB
+00001da0: 5004 8a6b 21d5 b640 9bf5 329e a1c8 79a6  P..k!..@..2...y.
+00001db0: 04ab b582 021d c1a1 4579 7d95 7343 b9b6  ........Ey}.sC..
+00001dc0: f06c b501 eb25 b828 9094 a3dc 1468 e7bd  .l...%.(.....h..
+00001dd0: a118 3bbe 8386 b924 3854 102b 6d1b e6c3  ..;....$8T.+m...
+00001de0: d16e b161 fc83 6d01 6784 4c71 039e 09e6  .n.a..m.g.Lq....
+00001df0: 196e 81b1 1988 e884 147c 409a 4f5b 7700  .n.......|@.O[w.
+00001e00: c131 d4d0 80f2 0ea7 498a 7fbc 1e6c e3fe  .1......I....l..
+00001e10: bcd0 2923 6723 fdd1 844e a7b8 63b6 e0bd  ..)#g#...N..c...
+00001e20: 38b8 0f4e 0ec6 fd7e 9fec 275d 8c90 3fc5  8..N...~..']..?.
+00001e30: 6fab c797 ae6a 2c55 bb2b 0ea8 cc05 a7dc  o....j,U.+......
+00001e40: 02f3 da96 6d7f 733c d439 1e0d db05 d6cc  ....m.s<.9......
+00001e50: f955 d875 2541 dc1d cb95 e456 3b5d f9e8  .U.u%A.....V;]..
+00001e60: a9aa 2487 68e3 c0e6 f8b7 31c0 bb2e fd0b  ..$.h.....1.....
+00001e70: 20a2 908e f65d ceca ebe4 fe61 bd44 6546   ....].....a.DeF
+00001e80: 3212 a769 4c6e d664 4627 539a cdde db1c  2..iLn.dF'S.....
+00001e90: 17f7 dbb4 fda0 39a5 f99f 98b5 c42c 5b93  ......9......,[.
+00001ea0: 3925 b794 cc47 c433 a0ec 725f fe90 f21b  9%...G.3..r_....
+00001eb0: 0000 ffff 0300 504b 0304 1400 0600 0800  ......PK........
+00001ec0: 0000 2100 b521 9af6 9001 0000 0d03 0000  ..!..!..........
+00001ed0: 1000 0801 646f 6350 726f 7073 2f61 7070  ....docProps/app
+00001ee0: 2e78 6d6c 20a2 0401 28a0 0001 0000 0000  .xml ...(.......
+00001ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001fe0: 0000 0000 0000 0000 0000 0000 9c92 416e  ..............An
+00001ff0: db30 1045 f705 7207 82fb 9872 1204 8541  .0.E..r....r...A
+00002000: 3128 9206 5e34 a801 3bd9 4fa9 91c5 9626  1(..^4..;.O....&
+00002010: 0572 2cd8 bd4d cfd2 8b75 2421 8edc 74d5  .r,..M...u$!..t.
+00002020: dd70 e6f3 f3f1 93fa eeb0 f3a2 c394 5d0c  .p............].
+00002030: a59c cf0a 2930 d858 b9b0 2de5 f3e6 f1f2  ....)0.X..-.....
+00002040: a314 9920 54e0 63c0 521e 31cb 3b73 f141  ... T.c.R.1.;s.A
+00002050: af52 6c31 91c3 2cd8 22e4 5236 44ed 42a9  .Rl1..,.".R6D.B.
+00002060: 6c1b dc41 9ef1 38f0 a48e 6907 c4cb b455  l..A..8...i....U
+00002070: b1ae 9dc5 8768 f73b 0ca4 ae8a e256 e181  .....h.;.....V..
+00002080: 3054 585d b627 4339 3a2e 3afa 5fd3 2ada  0TX].'C9:.:._.*.
+00002090: 9e2f bf6c 8e2d 031b fda9 6dbd b340 7c4b  ./.l.-....m..@|K
+000020a0: f3e4 6c8a 39d6 249e c0ba 4031 37e2 f3c1  ..l.9.$...@17...
+000020b0: a2d7 6a2a d3cc b946 bb4f 8e8e a6d0 6aba  ..j*...F.O....j.
+000020c0: d46b 0b1e eff9 0853 83cf a8d5 5b43 2f11  .k.....S....[C/.
+000020d0: faf8 56e0 5236 baa3 4587 9662 12d9 fde4  ..V.R6..E..b....
+000020e0: 00af a4f8 0619 7bb0 5276 901c 0462 c05e  ......{.Rv...b.^
+000020f0: 362e 86da b799 9259 c6ef 9045 85c2 fefe  6......Y...E....
+00002100: e5ed de47 ad58 37ce 8672 ba65 5abb 1b33  ...G.X7..r.eZ..3
+00002110: 1f04 5c9c 0b7b 8391 8707 e7a4 1b47 1ef3  ..\..{.......G..
+00002120: d77a 0589 fe01 3e9f 820f 0c23 f688 f300  .z....>....#....
+00002130: 04ef e886 7bf3 397f 397f 71e1 477e 6e37  ....{.9.9.q.G~n7
+00002140: 9137 e16b 80e7 4dbd 6e20 61c5 999f 023e  .7.k..M.n a....>
+00002150: 35f4 92b3 4bbe 37b9 6f20 6cb1 7ad5 bc1f  5...K.7.o l.z...
+00002160: f40f ff32 fe6e 33bf 9d15 d705 bfe4 a4a7  ...2.n3.........
+00002170: d5db 3f36 7f00 0000 ffff 0300 504b 0102  ..?6........PK..
+00002180: 2d00 1400 0600 0800 0000 2100 62ee 9d68  -.........!.b..h
+00002190: 5e01 0000 9004 0000 1300 0000 0000 0000  ^...............
+000021a0: 0000 0000 0000 0000 0000 5b43 6f6e 7465  ..........[Conte
+000021b0: 6e74 5f54 7970 6573 5d2e 786d 6c50 4b01  nt_Types].xmlPK.
+000021c0: 022d 0014 0006 0008 0000 0021 00b5 5530  .-.........!..U0
+000021d0: 23f4 0000 004c 0200 000b 0000 0000 0000  #....L..........
+000021e0: 0000 0000 0000 0097 0300 005f 7265 6c73  ..........._rels
+000021f0: 2f2e 7265 6c73 504b 0102 2d00 1400 0600  /.relsPK..-.....
+00002200: 0800 0000 2100 813e 9497 f300 0000 ba02  ....!..>........
+00002210: 0000 1a00 0000 0000 0000 0000 0000 0000  ................
+00002220: bc06 0000 786c 2f5f 7265 6c73 2f77 6f72  ....xl/_rels/wor
+00002230: 6b62 6f6f 6b2e 786d 6c2e 7265 6c73 504b  kbook.xml.relsPK
+00002240: 0102 2d00 1400 0600 0800 0000 2100 c92d  ..-.........!..-
+00002250: 551f ec02 0000 bd06 0000 0f00 0000 0000  U...............
+00002260: 0000 0000 0000 0000 ef08 0000 786c 2f77  ............xl/w
+00002270: 6f72 6b62 6f6f 6b2e 786d 6c50 4b01 022d  orkbook.xmlPK..-
+00002280: 0014 0006 0008 0000 0021 00e4 ac15 93eb  .........!......
+00002290: 0200 001f 0700 000d 0000 0000 0000 0000  ................
+000022a0: 0000 0000 0008 0c00 0078 6c2f 7374 796c  .........xl/styl
+000022b0: 6573 2e78 6d6c 504b 0102 2d00 1400 0600  es.xmlPK..-.....
+000022c0: 0800 0000 2100 e9a6 25b8 6606 0000 531b  ....!...%.f...S.
+000022d0: 0000 1300 0000 0000 0000 0000 0000 0000  ................
+000022e0: 1e0f 0000 786c 2f74 6865 6d65 2f74 6865  ....xl/theme/the
+000022f0: 6d65 312e 786d 6c50 4b01 022d 0014 0006  me1.xmlPK..-....
+00002300: 0008 0000 0021 00af 3b1e 8da1 0400 0009  .....!..;.......
+00002310: 1100 0018 0000 0000 0000 0000 0000 0000  ................
+00002320: 00b5 1500 0078 6c2f 776f 726b 7368 6565  .....xl/workshee
+00002330: 7473 2f73 6865 6574 312e 786d 6c50 4b01  ts/sheet1.xmlPK.
+00002340: 022d 0014 0006 0008 0000 0021 0054 6e48  .-.........!.TnH
+00002350: d26b 0100 004b 0400 0014 0000 0000 0000  .k...K..........
+00002360: 0000 0000 0000 008c 1a00 0078 6c2f 7368  ...........xl/sh
+00002370: 6172 6564 5374 7269 6e67 732e 786d 6c50  aredStrings.xmlP
+00002380: 4b01 022d 0014 0006 0008 0000 0021 00ad  K..-.........!..
+00002390: bc57 c556 0100 006e 0200 0011 0000 0000  .W.V...n........
+000023a0: 0000 0000 0000 0000 0029 1c00 0064 6f63  .........)...doc
+000023b0: 5072 6f70 732f 636f 7265 2e78 6d6c 504b  Props/core.xmlPK
+000023c0: 0102 2d00 1400 0600 0800 0000 2100 b521  ..-.........!..!
+000023d0: 9af6 9001 0000 0d03 0000 1000 0000 0000  ................
+000023e0: 0000 0000 0000 0000 b61e 0000 646f 6350  ............docP
+000023f0: 726f 7073 2f61 7070 2e78 6d6c 504b 0506  rops/app.xmlPK..
+00002400: 0000 0000 0a00 0a00 8002 0000 7c21 0000  ............|!..
+00002410: 0000                                     ..
```

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/listing_requests/entrypoint.py` & `connect_cli-27.0/connect/.data/connect_reports/reports/listing_requests/entrypoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (c) 2021, CloudBlue
+# Copyright (c) 2023, CloudBlue
 # All rights reserved.
 #
 
 from connect.client import R
 
 from ..utils import convert_to_datetime, get_basic_value, get_value, today_str
```

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/listing_requests/templates/xlsx/template.xlsx` & `connect_cli-27.0/connect/.data/connect_reports/reports/listing_requests/templates/xlsx/template.xlsx`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/entrypoint.py` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/entrypoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (c) 2021, Globex Corporation
+# Copyright (c) 2023, CloudBlue
 # All rights reserved.
 #
 
 from datetime import date
 
 from connect.client.rql import R
```

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-connect-alone.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-connect-alone.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-logo.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-logo.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-small-color-disabled.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-small-color-disabled.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-small-color-enabled.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-small-color-enabled.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/connect-logo.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/connect-logo.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cover-bg.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cover-bg.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/imc-small-color.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/imc-small-color.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/ClouBlue-Logo-Black.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/ClouBlue-Logo-Black.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/ClouBlue-Logo-White.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/ClouBlue-Logo-White.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/ClouBlue-Logo.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/ClouBlue-Logo.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/accordo.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/accordo.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/acronis-blue.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/acronis-blue.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/acronis-white.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/acronis-white.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/adobe.jpeg` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/adobe.jpeg`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/airtame.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/airtame.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/allyhub.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/allyhub.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/alsid.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/alsid.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/anchor.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/anchor.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/australia.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/australia.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/austria.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/austria.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/aws.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/aws.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/belgium.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/belgium.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/brazil.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/brazil.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/canada.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/canada.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/chile.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/chile.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/colombia.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/colombia.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/france.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/france.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/germany.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/germany.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/hong-kong.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/hong-kong.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/icon.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/icon.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/india.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/india.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/italy.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/italy.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/malaysia.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/malaysia.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/mexico.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/mexico.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/netherlands.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/netherlands.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/new-zealand.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/new-zealand.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/singapore.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/singapore.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/spain.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/spain.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/sweden.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/sweden.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/switzerland.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/switzerland.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/turkey.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/turkey.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/uae.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/uae.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/uk.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/uk.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/usa.png` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/usa.png`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/template.css` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/template.css`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/products_catalog/templates/pdf/template.html.j2` & `connect_cli-27.0/connect/.data/connect_reports/reports/products_catalog/templates/pdf/template.html.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/sla/Readme.md` & `connect_cli-27.0/connect/.data/connect_reports/reports/sla/Readme.md`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/sla/entrypoint.py` & `connect_cli-27.0/connect/.data/connect_reports/reports/sla/entrypoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (c) 2021, CloudBlue
+# Copyright (c) 2023, CloudBlue
 # All rights reserved.
 #
 import datetime
 
 from connect.client import R
 
 from ..utils import convert_to_datetime, get_dict_element
@@ -33,14 +33,16 @@
         query &= R().asset.connection.type.oneof(parameters['trans_type']['choices'])
     if parameters.get('product') and parameters['product']['all'] is False:
         query &= R().asset.product.id.oneof(parameters['product']['choices'])
     requests = client.requests.filter(query).select(
         '-asset.items',
         '-asset.params',
         '-asset.configuration',
+        '-activation_key',
+        '-template',
     ).order_by('created')
 
     total = requests.count()
 
     progress = 0
 
     levels = {
```

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/sla/templates/xlsx/template.xlsx` & `connect_cli-27.0/connect/.data/connect_reports/reports/sla/templates/xlsx/template.xlsx`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/subscription_list/entrypoint.py` & `connect_cli-27.0/connect/.data/connect_reports/reports/subscription_list/entrypoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (c) 2021, CloudBlue
+# Copyright (c) 2023, CloudBlue
 # All rights reserved.
 #
 
 from connect.client import ClientError, R
 
 from ..utils import convert_to_datetime, get_value
```

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/subscription_list/templates/xlsx/template.xlsx` & `connect_cli-27.0/connect/.data/connect_reports/reports/subscription_list/templates/xlsx/template.xlsx`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/tier_configuration_list/entrypoint.py` & `connect_cli-27.0/connect/.data/connect_reports/reports/tier_configuration_list/entrypoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (c) 2021, CloudBlue
+# Copyright (c) 2023, CloudBlue
 # All rights reserved.
 #
 
 from connect.client import R
 
 from ..utils import convert_to_datetime, get_basic_value, get_value, today_str
```

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/tier_configuration_list/templates/xlsx/template.xlsx` & `connect_cli-27.0/connect/.data/connect_reports/reports/tier_configuration_list/templates/xlsx/template.xlsx`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/tier_configuration_requests/entrypoint.py` & `connect_cli-27.0/connect/.data/connect_reports/reports/tier_configuration_requests/entrypoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (c) 2021, CloudBlue
+# Copyright (c) 2023, CloudBlue
 # All rights reserved.
 #
 
 from connect.client import R
 
 from ..utils import convert_to_datetime, get_basic_value, get_value, today_str
```

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/tier_configuration_requests/templates/xlsx/template.xlsx` & `connect_cli-27.0/connect/.data/connect_reports/reports/tier_configuration_requests/templates/xlsx/template.xlsx`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/usage_in_subscription/entrypoint.py` & `connect_cli-27.0/connect/.data/connect_reports/reports/usage_in_subscription/entrypoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (c) 2021, CloudBlue
+# Copyright (c) 2023, CloudBlue
 # All rights reserved.
 #
 from concurrent import futures
 
 from connect.client import R
 from connect.client import ClientError
```

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/usage_in_subscription/templates/xlsx/template.xlsx` & `connect_cli-27.0/connect/.data/connect_reports/reports/usage_in_subscription/templates/xlsx/template.xlsx`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports/utils.py` & `connect_cli-27.0/connect/.data/connect_reports/reports/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (c) 2021, CloudBlue
+# Copyright (c) 2023, CloudBlue
 # All rights reserved.
 #
 
 from datetime import datetime
 from threading import Lock
 import collections
```

### Comparing `connect_cli-26.9/connect/.data/connect_reports/reports.json` & `connect_cli-27.0/connect/.data/connect_reports/reports.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9939309056956116%*

 * *Differences: {"'reports'": "{0: {'renderers': {0: {'description': 'Export data in Microsoft Excel 2020 "*

 * *              "format'}}}, 1: {'renderers': {0: {'description': 'Export data in Microsoft Excel "*

 * *              "2020 format'}}}, 2: {'renderers': {0: {'description': 'Export data in Microsoft "*

 * *              "Excel 2020 format'}}}, 3: {'renderers': {0: {'description': 'Export data in "*

 * *              "Microsoft Excel 2020 format'}}}, 4: {'renderers': {0: {'description': 'Export data "*

 * *              "in Microsoft Exce […]*

```diff
@@ -111,15 +111,15 @@
             "renderers": [
                 {
                     "args": {
                         "start_col": 1,
                         "start_row": 2
                     },
                     "default": true,
-                    "description": "Export data in Microsoft Excel 2020 format.",
+                    "description": "Export data in Microsoft Excel 2020 format",
                     "id": "xlsx",
                     "template": "reports/fulfillment_requests/templates/xlsx/template.xlsx",
                     "type": "xlsx"
                 },
                 {
                     "default": false,
                     "description": "Export data as JSON",
@@ -227,15 +227,15 @@
             "renderers": [
                 {
                     "args": {
                         "start_col": 1,
                         "start_row": 2
                     },
                     "default": true,
-                    "description": "Export data in Microsoft Excel 2020 format.",
+                    "description": "Export data in Microsoft Excel 2020 format",
                     "id": "xlsx",
                     "template": "reports/fulfillment_requests_line_item/templates/xlsx/template.xlsx",
                     "type": "xlsx"
                 },
                 {
                     "default": false,
                     "description": "Export data as JSON",
@@ -328,15 +328,15 @@
             "renderers": [
                 {
                     "args": {
                         "start_col": 1,
                         "start_row": 2
                     },
                     "default": true,
-                    "description": "Export data in Microsoft Excel 2020 format.",
+                    "description": "Export data in Microsoft Excel 2020 format",
                     "id": "xlsx",
                     "template": "reports/fulfillment_requests_failed/templates/xlsx/template.xlsx",
                     "type": "xlsx"
                 },
                 {
                     "default": false,
                     "description": "Export data as JSON",
@@ -386,15 +386,15 @@
             "renderers": [
                 {
                     "args": {
                         "start_col": 1,
                         "start_row": 2
                     },
                     "default": true,
-                    "description": "Export data in Microsoft Excel 2020 format.",
+                    "description": "Export data in Microsoft Excel 2020 format",
                     "id": "xlsx",
                     "template": "reports/billing_requests/templates/xlsx/template.xlsx",
                     "type": "xlsx"
                 },
                 {
                     "default": false,
                     "description": "Export data as JSON",
@@ -444,15 +444,15 @@
             "renderers": [
                 {
                     "args": {
                         "start_col": 1,
                         "start_row": 2
                     },
                     "default": true,
-                    "description": "Export data in Microsoft Excel 2020 format.",
+                    "description": "Export data in Microsoft Excel 2020 format",
                     "id": "xlsx",
                     "template": "reports/billing_requests_line_item/templates/xlsx/template.xlsx",
                     "type": "xlsx"
                 },
                 {
                     "default": false,
                     "description": "Export data as JSON",
@@ -563,15 +563,15 @@
             "renderers": [
                 {
                     "args": {
                         "start_col": 1,
                         "start_row": 2
                     },
                     "default": true,
-                    "description": "Export data in Microsoft Excel 2020 format.",
+                    "description": "Export data in Microsoft Excel 2020 format",
                     "id": "xlsx",
                     "template": "reports/subscription_list/templates/xlsx/template.xlsx",
                     "type": "xlsx"
                 },
                 {
                     "default": false,
                     "description": "Export data as JSON",
@@ -667,15 +667,15 @@
             "renderers": [
                 {
                     "args": {
                         "start_col": 1,
                         "start_row": 2
                     },
                     "default": true,
-                    "description": "Export data in Microsoft Excel 2020 format.",
+                    "description": "Export data in Microsoft Excel 2020 format",
                     "id": "xlsx",
                     "template": "reports/tier_configuration_requests/templates/xlsx/template.xlsx",
                     "type": "xlsx"
                 },
                 {
                     "default": false,
                     "description": "Export data as JSON",
@@ -742,15 +742,15 @@
             "renderers": [
                 {
                     "args": {
                         "start_col": 1,
                         "start_row": 2
                     },
                     "default": true,
-                    "description": "Export data in Microsoft Excel 2020 format.",
+                    "description": "Export data in Microsoft Excel 2020 format",
                     "id": "xlsx",
                     "template": "reports/tier_configuration_list/templates/xlsx/template.xlsx",
                     "type": "xlsx"
                 },
                 {
                     "default": false,
                     "description": "Export data as JSON",
@@ -829,15 +829,15 @@
             "renderers": [
                 {
                     "args": {
                         "start_col": 1,
                         "start_row": 2
                     },
                     "default": true,
-                    "description": "Export data in Microsoft Excel 2020 format.",
+                    "description": "Export data in Microsoft Excel 2020 format",
                     "id": "xlsx",
                     "template": "reports/listing_requests/templates/xlsx/template.xlsx",
                     "type": "xlsx"
                 },
                 {
                     "default": false,
                     "description": "Export data as JSON",
@@ -903,15 +903,15 @@
             "renderers": [
                 {
                     "args": {
                         "start_col": 1,
                         "start_row": 2
                     },
                     "default": true,
-                    "description": "Export data in Microsoft Excel 2020 format.",
+                    "description": "Export data in Microsoft Excel 2020 format",
                     "id": "xlsx",
                     "template": "reports/listing_list/templates/xlsx/template.xlsx",
                     "type": "xlsx"
                 },
                 {
                     "default": false,
                     "description": "Export data as JSON",
@@ -967,15 +967,15 @@
             "renderers": [
                 {
                     "args": {
                         "start_col": 1,
                         "start_row": 2
                     },
                     "default": true,
-                    "description": "Export data in Microsoft Excel 2020 format.",
+                    "description": "Export data in Microsoft Excel 2020 format",
                     "id": "xlsx",
                     "template": "reports/customers_list/templates/xlsx/template.xlsx",
                     "type": "xlsx"
                 },
                 {
                     "default": false,
                     "description": "Export data as JSON",
@@ -1058,15 +1058,15 @@
             "renderers": [
                 {
                     "args": {
                         "start_col": 1,
                         "start_row": 2
                     },
                     "default": true,
-                    "description": "Export data in Microsoft Excel 2020 format.",
+                    "description": "Export data in Microsoft Excel 2020 format",
                     "id": "xlsx",
                     "template": "reports/contract_list/templates/xlsx/template.xlsx",
                     "type": "xlsx"
                 },
                 {
                     "default": false,
                     "description": "Export data as JSON",
@@ -1109,15 +1109,15 @@
             "renderers": [
                 {
                     "args": {
                         "start_col": 1,
                         "start_row": 2
                     },
                     "default": true,
-                    "description": "Export data in Microsoft Excel 2020 format.",
+                    "description": "Export data in Microsoft Excel 2020 format",
                     "id": "xlsx",
                     "template": "reports/usage_in_subscription/templates/xlsx/template.xlsx",
                     "type": "xlsx"
                 },
                 {
                     "default": false,
                     "description": "Export data as JSON",
@@ -1206,15 +1206,15 @@
             "renderers": [
                 {
                     "args": {
                         "start_col": 1,
                         "start_row": 2
                     },
                     "default": true,
-                    "description": "Export data in Microsoft Excel 2020 format.",
+                    "description": "Export data in Microsoft Excel 2020 format",
                     "id": "xlsx",
                     "template": "reports/sla/templates/xlsx/template.xlsx",
                     "type": "xlsx"
                 }
             ],
             "report_spec": "2"
         },
@@ -1304,11 +1304,80 @@
                     "description": "Export data as PDF (portrait)",
                     "id": "pdf",
                     "template": "reports/executive_fullfilment_requests/templates/pdf/template.html.j2",
                     "type": "pdf"
                 }
             ],
             "report_spec": "2"
+        },
+        {
+            "audience": [
+                "provider",
+                "vendor"
+            ],
+            "entrypoint": "reports.helpdesk.entrypoint.generate",
+            "name": "HelpDesk report",
+            "parameters": [
+                {
+                    "description": "Provide the time period to create the report",
+                    "id": "date",
+                    "name": "Report period",
+                    "required": true,
+                    "type": "date_range"
+                },
+                {
+                    "choices": [
+                        {
+                            "label": "Inquiring",
+                            "value": "inquiring"
+                        },
+                        {
+                            "label": "Pending",
+                            "value": "pending"
+                        },
+                        {
+                            "label": "Resolved",
+                            "value": "resolved"
+                        },
+                        {
+                            "label": "Closed",
+                            "value": "closed"
+                        }
+                    ],
+                    "description": "Select the status of ticket you want to include in report",
+                    "id": "ticket_status",
+                    "name": "Tickets in status",
+                    "required": true,
+                    "type": "checkbox"
+                }
+            ],
+            "readme_file": "reports/helpdesk/Readme.md",
+            "renderers": [
+                {
+                    "args": {
+                        "start_col": 1,
+                        "start_row": 2
+                    },
+                    "default": true,
+                    "description": "Export data in Microsoft Excel 2020 format",
+                    "id": "xlsx",
+                    "template": "reports/helpdesk/templates/xlsx/template.xlsx",
+                    "type": "xlsx"
+                },
+                {
+                    "default": false,
+                    "description": "Export data as JSON",
+                    "id": "json",
+                    "type": "json"
+                },
+                {
+                    "default": false,
+                    "description": "Export data as CSV",
+                    "id": "csv",
+                    "type": "csv"
+                }
+            ],
+            "report_spec": "2"
         }
     ],
     "version": "1.0.0"
 }
```

### Comparing `connect_cli-26.9/connect/cli/ccli.py` & `connect_cli-27.0/connect/cli/ccli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 # -*- coding: utf-8 -*-
 
 # This file is part of the Ingram Micro Cloud Blue Connect connect-cli.
 # Copyright (c) 2019-2021 Ingram Micro. All Rights Reserved.
+import io
+import sys
+
 import click
 
 from connect.cli.core.base import cli
 from connect.cli.core.constants import CAIRO_NOT_FOUND_ERROR
 from connect.cli.core.plugins import load_plugins
 
 
 def main():
+    _set_stdout_unbuffered()
     _ignore_openpyxl_warnings()
     try:
         import uvloop
         uvloop.install()
     except ImportError:
         pass
     print('')
@@ -40,9 +44,14 @@
     uses some custom extension).
     To avoid losing data validation, it should be re-created each time the file is saved by the cli.
     """
     import warnings
     warnings.filterwarnings('ignore', category=UserWarning, module='openpyxl.worksheet._reader')
 
 
+def _set_stdout_unbuffered():  # pragma: no cover
+    if 'pytest' not in sys.modules:
+        sys.stdout = io.TextIOWrapper(open(sys.stdout.fileno(), 'wb', 0), write_through=True)
+
+
 if __name__ == '__main__':
     main()  # pragma: no cover
```

### Comparing `connect_cli-26.9/connect/cli/core/account/commands.py` & `connect_cli-27.0/connect/cli/core/account/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,15 @@
 
 # This file is part of the Ingram Micro Cloud Blue Connect connect-cli.
 # Copyright (c) 2019-2021 Ingram Micro. All Rights Reserved.
 
 import click
 from click import ClickException
 
-from connect.cli.core.account.helpers import (
-    activate_account,
-    add_account,
-    remove_account,
-)
+from connect.cli.core.account.helpers import activate_account, add_account, remove_account
 from connect.cli.core.config import pass_config
 from connect.cli.core.constants import DEFAULT_ENDPOINT
 from connect.cli.core.terminal import console
 from connect.cli.core.utils import field_to_check_mark
 
 
 @click.group(name='account', short_help='Manage configured accounts.')
```

### Comparing `connect_cli-26.9/connect/cli/core/account/helpers.py` & `connect_cli-27.0/connect/cli/core/account/helpers.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 # This file is part of the Ingram Micro Cloud Blue Connect connect-cli.
 # Copyright (c) 2019-2021 Ingram Micro. All Rights Reserved.
 
 import click
-
 from connect.client import ClientError, ConnectClient
+
 from connect.cli.core.http import RequestLogger
 
 
 def add_account(config, api_key, endpoint):
     try:
         client = ConnectClient(
             api_key=api_key,
```

### Comparing `connect_cli-26.9/connect/cli/core/base.py` & `connect_cli-27.0/connect/cli/core/base.py`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/cli/core/config.py` & `connect_cli-27.0/connect/cli/core/config.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 # Copyright (c) 2019-2021 Ingram Micro. All Rights Reserved.
 
 import json
 import os
 from dataclasses import dataclass
 
 from click import ClickException, make_pass_decorator
-
 from connect.client import ConnectClient
+
 from connect.cli.core.constants import DEFAULT_ENDPOINT
 from connect.cli.core.http import RequestLogger
 
 
 @dataclass
 class Account:
     id: str
```

### Comparing `connect_cli-26.9/connect/cli/core/constants.py` & `connect_cli-27.0/connect/cli/core/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # -*- coding: utf-8 -*-
 
 # This file is part of the Ingram Micro Cloud Blue Connect connect-cli.
 # Copyright (c) 2019-2021 Ingram Micro. All Rights Reserved.
 
 DEFAULT_ENDPOINT = 'https://api.connect.cloudblue.com/public/v1'
-DEFAULT_USER_AGENT = 'CloudBlue Connect CLI/'
-DEFAULT_BAR_FORMAT = '{desc:<70.69}{percentage:3.0f}%|{bar:30}{r_bar}'
 
 CAIRO_NOT_FOUND_ERROR = """Connect CLI depends on Cairo which is not present on the system.
 If so, please follow the instructions to install it at https://github.com/cloudblue/connect-cli
 and make sure your PATH environment variable includes also the Cairo shared libraries folder.
 """
 
 PYPI_JSON_API_URL = 'https://pypi.org/pypi/connect-cli/json'
```

### Comparing `connect_cli-26.9/connect/cli/core/http.py` & `connect_cli-27.0/connect/cli/core/http.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import platform
 from http import HTTPStatus
 
 import click
+from connect.client import ClientError, RequestLogger as _RequestLogger
 
 from connect.cli import get_version
 from connect.cli.core.terminal import console
-from connect.client import ClientError, RequestLogger as _RequestLogger
 
 
 def get_user_agent():
     version = get_version()
     pimpl = platform.python_implementation()
     pver = platform.python_version()
     sysname = platform.system()
```

### Comparing `connect_cli-26.9/connect/cli/core/plugins.py` & `connect_cli-27.0/connect/cli/core/plugins.py`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/cli/core/terminal.py` & `connect_cli-27.0/connect/cli/core/terminal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,31 @@
-import os
 import contextlib
+import os
 
 from click.exceptions import Abort
+from connect.utils.terminal.markdown import render
 from rich import box
 from rich.console import Console as _Console, Group
 from rich.live import Live
-from rich.status import Status as _Status
-from rich.style import Style
 from rich.panel import Panel
-from rich.prompt import Confirm
 from rich.progress import (
-    BarColumn, MofNCompleteColumn, Progress, SpinnerColumn,
-    TaskProgressColumn, TextColumn, TimeElapsedColumn,
+    BarColumn,
+    MofNCompleteColumn,
+    Progress,
+    SpinnerColumn,
+    TaskProgressColumn,
+    TextColumn,
+    TimeElapsedColumn,
 )
+from rich.prompt import Confirm
+from rich.status import Status as _Status
+from rich.style import Style
 from rich.table import Table
 from rich.text import Text
 
-from connect.utils.terminal.markdown import render
-
 
 def get_style(
     fg=None,
     bg=None,
     bold=None,
     dim=None,
     underline=None,
```

### Comparing `connect_cli-26.9/connect/cli/core/utils.py` & `connect_cli-27.0/connect/cli/core/utils.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 # This file is part of the Ingram Micro Cloud Blue Connect connect-cli.
 # Copyright (c) 2019-2022 Ingram Micro. All Rights Reserved.
 import os
 from collections import OrderedDict
 from importlib.metadata import entry_points
 
-from packaging.version import InvalidVersion, Version
 import click
 import requests
+from packaging.version import InvalidVersion, Version
 
 from connect.cli import get_version
 from connect.cli.core.constants import PYPI_JSON_API_URL
 from connect.cli.core.terminal import console
 
 
 def _get_correct_sorted_versions(tags):
```

### Comparing `connect_cli-26.9/connect/cli/plugins/customer/commands.py` & `connect_cli-27.0/connect/cli/plugins/customer/commands.py`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/cli/plugins/customer/export.py` & `connect_cli-27.0/connect/cli/plugins/customer/export.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
+from connect.client import ClientError
 from iso3166 import countries
 from openpyxl import Workbook
 from openpyxl.styles import PatternFill
 from openpyxl.styles.colors import Color
 from openpyxl.worksheet.datavalidation import DataValidation
 
 from connect.cli.core.http import handle_http_error
 from connect.cli.core.terminal import console
 from connect.cli.core.utils import validate_output_options
 from connect.cli.plugins.customer.constants import COL_HEADERS
-from connect.client import ClientError
 
 
 def dump_customers(client, account_id, output_file, output_path=None):  # noqa: CCR001
     output_file = validate_output_options(
         output_path, output_file, default_dir_name=account_id, default_file_name='customers',
     )
     try:
```

### Comparing `connect_cli-26.9/connect/cli/plugins/customer/sync.py` & `connect_cli-27.0/connect/cli/plugins/customer/sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import uuid
 from collections import namedtuple
+from zipfile import BadZipFile
 
 import phonenumbers
 from click import ClickException
-
 from connect.client import ClientError, R
-
-from zipfile import BadZipFile
-
 from openpyxl import load_workbook
 from openpyxl.utils.exceptions import InvalidFileException
 
 from connect.cli.core.terminal import console
-from connect.cli.plugins.shared.sync_stats import SynchronizerStatsSingleModule
-from connect.cli.plugins.shared.exceptions import SheetNotFoundError
 from connect.cli.plugins.customer.constants import COL_HEADERS
+from connect.cli.plugins.shared.exceptions import SheetNotFoundError
+from connect.cli.plugins.shared.sync_stats import SynchronizerStatsSingleModule
+
 
 fields = (v.replace(' ', '_').lower() for v in COL_HEADERS.values())
 
 _RowData = namedtuple('RowData', fields)
 
 
 class CustomerSynchronizer:
```

### Comparing `connect_cli-26.9/connect/cli/plugins/locale/commands.py` & `connect_cli-27.0/connect/cli/plugins/locale/commands.py`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/cli/plugins/play/commands.py` & `connect_cli-27.0/connect/cli/plugins/play/commands.py`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/cli/plugins/play/context.py` & `connect_cli-27.0/connect/cli/plugins/play/context.py`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/cli/plugins/play/script.py` & `connect_cli-27.0/connect/cli/plugins/play/script.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # -*- coding: utf-8 -*-
 
 # This file is part of the Ingram Micro Cloud Blue Connect connect-cli.
 # Copyright (c) 2021 Ingram Micro. All Rights Reserved.
 import re
 from typing import List
 
-from connect.cli.plugins.play.context import Context
 from connect.client import ConnectClient
 
+from connect.cli.plugins.play.context import Context
+
 
 class OptionWrapper:
     def __init__(self, *args, **kwargs):
         self.args = args
         self.kwargs = kwargs
```

### Comparing `connect_cli-26.9/connect/cli/plugins/product/api.py` & `connect_cli-27.0/connect/cli/plugins/product/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
 
 # This file is part of the Ingram Micro Cloud Blue Connect connect-cli.
 # Copyright (c) 2019-2021 Ingram Micro. All Rights Reserved.
 
-from connect.cli.core.http import handle_http_error
 from connect.client import ClientError, R
 
+from connect.cli.core.http import handle_http_error
+
 
 def create_unit(client, data):
     try:
         res = client.ns('settings').units.create(data)
     except ClientError as error:
         handle_http_error(error)
     return res
```

### Comparing `connect_cli-26.9/connect/cli/plugins/product/clone.py` & `connect_cli-27.0/connect/cli/plugins/product/clone.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from datetime import datetime
 
 from click import ClickException
+from connect.client import ClientError
 from fs.tempfs import TempFS
 from openpyxl import load_workbook
 
 from connect.cli.plugins.product.export import dump_product
 from connect.cli.plugins.product.sync import (
     ActionsSynchronizer,
     CapabilitiesSynchronizer,
     GeneralSynchronizer,
     ItemSynchronizer,
     MediaSynchronizer,
     ParamsSynchronizer,
     TemplatesSynchronizer,
 )
-from connect.client import ClientError
 from connect.cli.plugins.shared.translations_synchronizers import sync_product_translations
 from connect.cli.plugins.shared.utils import get_translation_attributes_sheets
 
 
 class ProductCloner:
     def __init__(self, config, source_account, destination_account, product_id, progress, stats):
         self.fs = TempFS(identifier=f'_clone_{product_id}')
```

### Comparing `connect_cli-26.9/connect/cli/plugins/product/commands.py` & `connect_cli-27.0/connect/cli/plugins/product/commands.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,35 +3,35 @@
 # This file is part of the Ingram Micro Cloud Blue Connect connect-cli.
 # Copyright (c) 2019-2022 Ingram Micro. All Rights Reserved.
 
 from functools import partial
 
 import click
 from click.exceptions import ClickException
+from connect.client import ClientError, R
 
 from connect.cli.core import group
 from connect.cli.core.config import pass_config
 from connect.cli.core.terminal import console
-from connect.cli.plugins.shared.sync_stats import SynchronizerStats
-from connect.cli.plugins.shared.exceptions import SheetNotFoundError
-from connect.cli.plugins.shared.translations_synchronizers import sync_product_translations
 from connect.cli.plugins.product.clone import ProductCloner
 from connect.cli.plugins.product.export import dump_product
 from connect.cli.plugins.product.sync import (
     ActionsSynchronizer,
     CapabilitiesSynchronizer,
     ConfigurationValuesSynchronizer,
     GeneralSynchronizer,
     ItemSynchronizer,
     MediaSynchronizer,
     ParamsSynchronizer,
     StaticResourcesSynchronizer,
     TemplatesSynchronizer,
 )
-from connect.client import ClientError, R
+from connect.cli.plugins.shared.exceptions import SheetNotFoundError
+from connect.cli.plugins.shared.sync_stats import SynchronizerStats
+from connect.cli.plugins.shared.translations_synchronizers import sync_product_translations
 
 
 @group(name='product', short_help='Manage product definitions.')
 def grp_product():
     pass  # pragma: no cover
```

### Comparing `connect_cli-26.9/connect/cli/plugins/product/constants.py` & `connect_cli-27.0/connect/cli/plugins/product/constants.py`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/cli/plugins/product/export.py` & `connect_cli-27.0/connect/cli/plugins/product/export.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,44 +1,38 @@
 # -*- coding: utf-8 -*-
 
 # This file is part of the Ingram Micro Cloud Blue Connect connect-cli.
 # Copyright (c) 2019-2022 Ingram Micro. All Rights Reserved.
 
-import os
 import copy
 import json
+import os
 from datetime import datetime
 from urllib import parse
 
 import requests
 from click import ClickException
+from connect.client import ClientError, R
 from openpyxl import Workbook
 from openpyxl.styles import Alignment, Font, PatternFill
-from openpyxl.styles.colors import Color, WHITE
+from openpyxl.styles.colors import WHITE, Color
 from openpyxl.utils import quote_sheetname
 from openpyxl.worksheet.datavalidation import DataValidation
 
-from connect.cli.core.http import (
-    format_http_status,
-    handle_http_error,
-)
+from connect.cli.core.http import format_http_status, handle_http_error
 from connect.cli.core.utils import validate_output_options
 from connect.cli.plugins.product.constants import PARAM_TYPES
 from connect.cli.plugins.product.utils import get_json_object_for_param
-from connect.cli.plugins.shared.export import (
-    alter_attributes_sheet,
-    get_translation_workbook,
-)
+from connect.cli.plugins.shared.export import alter_attributes_sheet, get_translation_workbook
 from connect.cli.plugins.shared.utils import (
     fill_translation_row,
     get_col_headers_by_ws_type,
     get_col_limit_by_ws_type,
     setup_locale_data_validation,
 )
-from connect.client import ClientError, R
 
 
 def _setup_locales_list(ws, client):
     """
     Fill list of locales to use with DataValidation.
     """
     locales = client.ns('localization').locales.all()
```

### Comparing `connect_cli-26.9/connect/cli/plugins/product/sync/__init__.py` & `connect_cli-27.0/connect/cli/plugins/product/sync/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 from connect.cli.plugins.product.sync.actions import ActionsSynchronizer  # noqa: F401
 from connect.cli.plugins.product.sync.capabilities import CapabilitiesSynchronizer  # noqa: F401
-from connect.cli.plugins.product.sync.configuration_values import ConfigurationValuesSynchronizer  # noqa: F401
+from connect.cli.plugins.product.sync.configuration_values import (  # noqa: F401
+    ConfigurationValuesSynchronizer,
+)
 from connect.cli.plugins.product.sync.general import GeneralSynchronizer  # noqa: F401
 from connect.cli.plugins.product.sync.items import ItemSynchronizer  # noqa: F401
 from connect.cli.plugins.product.sync.media import MediaSynchronizer  # noqa: F401
 from connect.cli.plugins.product.sync.params import ParamsSynchronizer  # noqa: F401
-from connect.cli.plugins.product.sync.static_resources import StaticResourcesSynchronizer  # noqa: F401
+from connect.cli.plugins.product.sync.static_resources import (  # noqa: F401
+    StaticResourcesSynchronizer,
+)
 from connect.cli.plugins.product.sync.templates import TemplatesSynchronizer  # noqa: F401
```

### Comparing `connect_cli-26.9/connect/cli/plugins/product/sync/actions.py` & `connect_cli-27.0/connect/cli/plugins/product/sync/actions.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 # This file is part of the Ingram Micro Cloud Blue Connect connect-cli.
 # Copyright (c) 2019-2021 Ingram Micro. All Rights Reserved.
 
 import re
 from collections import namedtuple
 from functools import partial
 
-from connect.cli.plugins.shared.base import ProductSynchronizer
-from connect.cli.plugins.shared.constants import (
-    ACTIONS_HEADERS,
-)
 from connect.client import ClientError
 
+from connect.cli.plugins.shared.base import ProductSynchronizer
+from connect.cli.plugins.shared.constants import ACTIONS_HEADERS
+
+
 fields = (v.replace(' ', '_').lower() for v in ACTIONS_HEADERS.values())
 
 _RowData = namedtuple('RowData', fields)
 
 
 class ActionsSynchronizer(ProductSynchronizer):
     def __init__(self, client, progress, stats):
```

### Comparing `connect_cli-26.9/connect/cli/plugins/product/sync/capabilities.py` & `connect_cli-27.0/connect/cli/plugins/product/sync/capabilities.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from collections import namedtuple
 
 from connect.cli.plugins.product.constants import CAPABILITIES
+from connect.cli.plugins.product.utils import cleanup_product_for_update
 from connect.cli.plugins.shared.base import ProductSynchronizer
 from connect.cli.plugins.shared.constants import CAPABILITIES_COLS_HEADERS
-from connect.cli.plugins.product.utils import cleanup_product_for_update
 
 
 fields = (v.replace(' ', '_').lower() for v in CAPABILITIES_COLS_HEADERS.values())
 
 _RowData = namedtuple('RowData', fields)
```

### Comparing `connect_cli-26.9/connect/cli/plugins/product/sync/configuration_values.py` & `connect_cli-27.0/connect/cli/plugins/product/sync/configuration_values.py`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/cli/plugins/product/sync/general.py` & `connect_cli-27.0/connect/cli/plugins/product/sync/general.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-import os
 import json
+import os
 from mimetypes import guess_type
 
 from click import ClickException
+from connect.client import ClientError
 
-from connect.cli.plugins.shared.base import ProductSynchronizer
 from connect.cli.plugins.product.utils import cleanup_product_for_update
-from connect.client import ClientError
+from connect.cli.plugins.shared.base import ProductSynchronizer
 
 
 class GeneralSynchronizer(ProductSynchronizer):
     def __init__(self, client, progress):
         self._category = None
         self._media_path = None
         super(GeneralSynchronizer, self).__init__(client, progress)
```

### Comparing `connect_cli-26.9/connect/cli/plugins/product/sync/items.py` & `connect_cli-27.0/connect/cli/plugins/product/sync/items.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 # -*- coding: utf-8 -*-
 
 # This file is part of the Ingram Micro Cloud Blue Connect connect-cli.
 # Copyright (c) 2019-2021 Ingram Micro. All Rights Reserved.
 
 from collections import namedtuple
 
-from connect.cli.plugins.product.constants import (
-    BILLING_PERIOD,
-    COMMITMENT,
-    PRECISIONS,
-)
-from connect.cli.plugins.shared.base import ProductSynchronizer
-from connect.cli.plugins.shared.constants import ITEMS_COLS_HEADERS
+from connect.client.rql import R
+
 from connect.cli.plugins.product.api import (
     create_item,
     create_unit,
     delete_item,
     get_item,
     get_item_by_mpn,
     update_item,
 )
-from connect.client.rql import R
+from connect.cli.plugins.product.constants import BILLING_PERIOD, COMMITMENT, PRECISIONS
+from connect.cli.plugins.shared.base import ProductSynchronizer
+from connect.cli.plugins.shared.constants import ITEMS_COLS_HEADERS
+
 
 fields = (v.replace(' ', '_').lower() for v in ITEMS_COLS_HEADERS.values())
 
 _RowData = namedtuple('RowData', fields)
 
 
 class ItemSynchronizer(ProductSynchronizer):
```

### Comparing `connect_cli-26.9/connect/cli/plugins/product/sync/media.py` & `connect_cli-27.0/connect/cli/plugins/product/sync/media.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # -*- coding: utf-8 -*-
 
 # This file is part of the Ingram Micro Cloud Blue Connect connect-cli.
 # Copyright (c) 2019-2021 Ingram Micro. All Rights Reserved.
+import json
 import os
 from collections import namedtuple
-from urllib.parse import urlparse
-import json
 from mimetypes import guess_type
+from urllib.parse import urlparse
 
-from connect.cli.plugins.shared.constants import MEDIA_COLS_HEADERS
-from connect.cli.plugins.shared.base import ProductSynchronizer
 from connect.client import ClientError
 
+from connect.cli.plugins.shared.base import ProductSynchronizer
+from connect.cli.plugins.shared.constants import MEDIA_COLS_HEADERS
+
 
 fields = (v.replace(' ', '_').lower() for v in MEDIA_COLS_HEADERS.values())
 
 _RowData = namedtuple('RowData', fields)
 
 
 class MediaSynchronizer(ProductSynchronizer):
```

### Comparing `connect_cli-26.9/connect/cli/plugins/product/sync/params.py` & `connect_cli-27.0/connect/cli/plugins/product/sync/params.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 # This file is part of the Ingram Micro Cloud Blue Connect connect-cli.
 # Copyright (c) 2019-2021 Ingram Micro. All Rights Reserved.
 import json
 import re
 from collections import namedtuple
 from json.decoder import JSONDecodeError
 
+from connect.client import ClientError
 from openpyxl.styles import Alignment
 
 from connect.cli.plugins.product.constants import PARAM_TYPES
+from connect.cli.plugins.product.utils import ParamSwitchNotSupported, get_json_object_for_param
 from connect.cli.plugins.shared.base import ProductSynchronizer
 from connect.cli.plugins.shared.constants import PARAMS_COLS_HEADERS
-from connect.cli.plugins.product.utils import get_json_object_for_param, ParamSwitchNotSupported
-from connect.client import ClientError
 
 
 fields = (v.replace(' ', '_').lower() for v in PARAMS_COLS_HEADERS.values())
 
 _RowData = namedtuple('RowData', fields)
```

### Comparing `connect_cli-26.9/connect/cli/plugins/product/sync/static_resources.py` & `connect_cli-27.0/connect/cli/plugins/product/sync/static_resources.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from collections import namedtuple
 from urllib.parse import urlparse
 
-from connect.cli.plugins.shared.constants import STATIC_LINK_HEADERS
-from connect.cli.plugins.shared.base import ProductSynchronizer
 from connect.cli.plugins.product.utils import cleanup_product_for_update
+from connect.cli.plugins.shared.base import ProductSynchronizer
+from connect.cli.plugins.shared.constants import STATIC_LINK_HEADERS
 
 
 fields = (v.replace(' ', '_').lower() for v in STATIC_LINK_HEADERS.values())
 
 _RowData = namedtuple('RowData', fields)
```

### Comparing `connect_cli-26.9/connect/cli/plugins/product/sync/templates.py` & `connect_cli-27.0/connect/cli/plugins/product/sync/templates.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # -*- coding: utf-8 -*-
 
 # This file is part of the Ingram Micro Cloud Blue Connect connect-cli.
 # Copyright (c) 2019-2021 Ingram Micro. All Rights Reserved.
 
 from collections import namedtuple
 
-from connect.cli.plugins.shared.constants import TEMPLATES_HEADERS
-from connect.cli.plugins.shared.base import ProductSynchronizer
 from connect.client import ClientError
 
+from connect.cli.plugins.shared.base import ProductSynchronizer
+from connect.cli.plugins.shared.constants import TEMPLATES_HEADERS
+
+
 fields = (v.replace(' ', '_').lower() for v in TEMPLATES_HEADERS.values())
 
 _RowData = namedtuple('RowData', fields)
 
 
 class TemplatesSynchronizer(ProductSynchronizer):
     def __init__(self, client, progress, stats):
```

### Comparing `connect_cli-26.9/connect/cli/plugins/product/utils.py` & `connect_cli-27.0/connect/cli/plugins/product/utils.py`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/cli/plugins/project/commands.py` & `connect_cli-27.0/connect/cli/plugins/project/commands.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,14 +14,38 @@
 from connect.cli.plugins.project.report.helpers import (
     add_report,
     bootstrap_report_project,
     validate_report_project,
 )
 
 
+class Mutex(click.Option):
+    def __init__(self, *args, **kwargs):
+        self.conflict_with: list = kwargs.pop("conflict_with")
+
+        assert self.conflict_with, "'conflict_with' parameter required"
+
+        help_str = kwargs.get("help", "")
+        help_str += f' This option is mutually exclusive with {", ".join(self.conflict_with)}.'
+        kwargs["help"] = help_str.strip()
+        super(Mutex, self).__init__(*args, **kwargs)
+
+    def handle_parse_result(self, ctx, opts, args):
+        current_opt: bool = self.name in opts
+        for mutex_opt in self.conflict_with:
+            if mutex_opt in opts:
+                if current_opt:
+                    raise click.UsageError(
+                        f'Illegal usage: options {self.name} and {mutex_opt} are mutually exclusive.',
+                    )
+                else:
+                    self.prompt = None
+        return super(Mutex, self).handle_parse_result(ctx, opts, args)
+
+
 @group(name='project', short_help='Manage project definitions.')
 def grp_project():
     pass  # pragma: no cover
 
 
 # REPORTS
 @grp_project.group(
@@ -108,17 +132,43 @@
 )
 @click.option(
     '--force-overwrite', '-f',
     is_flag=True,
     help='Overwrite the destination project directory if exists.',
     default=False,
 )
+@click.option(
+    '--save-answers', '-s',
+    default=None,
+    type=click.Path(exists=False, file_okay=True, dir_okay=False),
+    required=False,
+    help='Path to JSON file where to save wizard answers.',
+    cls=Mutex,
+    conflict_with=['load_answers'],
+)
+@click.option(
+    '--load-answers', '-l',
+    default=None,
+    type=click.Path(exists=True, file_okay=True, dir_okay=False),
+    required=False,
+    help='Path to JSON file from where load wizard answers.',
+    cls=Mutex,
+    conflict_with=['save_answers'],
+)
 @pass_config
-def cmd_bootstrap_extension_project(config, output_dir, force_overwrite):
-    bootstrap_extension_project(config, output_dir, force_overwrite)
+def cmd_bootstrap_extension_project(
+        config, output_dir, force_overwrite, save_answers, load_answers,
+):
+    bootstrap_extension_project(
+        config,
+        output_dir,
+        force_overwrite,
+        save_answers,
+        load_answers,
+    )
 
 
 @grp_project_extension.command(
     name='validate',
     short_help='Validate given extension project.',
 )
 @click.argument(
```

### Comparing `connect_cli-26.9/connect/cli/plugins/project/extension/helpers.py` & `connect_cli-27.0/connect/cli/plugins/project/extension/helpers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,48 +1,75 @@
 import collections
+import json
 import os
 
 import yaml
 from click.exceptions import ClickException
+from connect.eaas.core.validation.validators import get_validators
 from interrogatio.core.dialog import dialogus
 
 from connect.cli import get_version
 from connect.cli.core.terminal import console
-from connect.cli.plugins.project.utils import show_validation_result_table
-from connect.cli.plugins.project.renderer import BoilerplateRenderer
 from connect.cli.plugins.project.extension.utils import (
     get_event_definitions,
     get_pypi_runner_version,
     initialize_git_repository,
 )
 from connect.cli.plugins.project.extension.wizard import (
     EXTENSION_BOOTSTRAP_WIZARD_INTRO,
     get_questions,
     get_summary,
 )
-from connect.eaas.core.validation.validators import get_validators
+from connect.cli.plugins.project.renderer import BoilerplateRenderer
+from connect.cli.plugins.project.utils import show_validation_result_table
+from connect.cli.plugins.project.validators import ProjectDirValidator
 
 
-def bootstrap_extension_project(config, output_dir, overwrite):  # noqa: CCR001
+def bootstrap_extension_project(  # noqa: CCR001
+        config, output_dir, overwrite, save_answers, load_answers,
+):
     console.secho('Bootstraping extension project...\n', fg='blue')
 
+    if save_answers and os.path.exists(save_answers):
+        raise ClickException(f'Answers cannot be saved, because {save_answers} already exists.')
+
     statuses_by_event = collections.defaultdict(lambda: collections.defaultdict())
 
     definitions = get_event_definitions(config)
     grouped_definitions = collections.defaultdict(lambda: collections.defaultdict(list))
 
     for elem in definitions:
         statuses_by_event[elem['extension_type']][elem['type']] = elem['object_statuses']
         grouped_definitions[elem['extension_type']][elem['category']].append(elem)
 
+    questions = get_questions(config, grouped_definitions)
+
+    if load_answers:
+        try:
+            with open(load_answers) as fp:
+                loaded_answers = json.load(fp)
+
+            for question in questions:
+                if question['name'] in loaded_answers:
+                    question['default'] = loaded_answers[question['name']]
+        except Exception as e:
+            raise ClickException(f'Can not load or parse answers from {load_answers}: {e}')
+
+    if not overwrite:
+        for q in questions:
+            if q['name'] == 'project_slug':
+                q['validators'].append(ProjectDirValidator(output_dir))
+                break
+
     answers = dialogus(
-        get_questions(config, grouped_definitions),
+        questions,
         'Extension project bootstrap',
         intro=EXTENSION_BOOTSTRAP_WIZARD_INTRO,
         summary=get_summary,
+        fast_forward=load_answers is not None,
         finish_text='Create',
         previous_text='Back',
     )
 
     if not answers:
         raise ClickException('Aborted by user input')
 
@@ -56,38 +83,61 @@
     for var, answer in answers.items():
         ctx.update({var: answer})
 
     project_dir = os.path.join(output_dir, ctx['project_slug'])
     if not overwrite and os.path.exists(project_dir):
         raise ClickException(f'The destination directory {project_dir} already exists.')
 
+    if save_answers:
+        with open(save_answers, 'w') as fp:
+            json.dump(answers, fp, indent=2)
+        console.echo()
+        console.secho(f'Answers saved to {save_answers}', fg='green')
+        console.echo()
+
     exclude = []
 
     if answers['use_github_actions'] == 'n':
         exclude.extend(['.github', '.github/**/*'])
 
+    application_types = answers.get('application_types', [])
+
     if answers.get('webapp_supports_ui') != 'y':
         exclude.extend([
             os.path.join('${package_name}', 'static', '.gitkeep'),
             'ui',
             'ui/**/*',
             'package.json.j2',
             'webpack.config.js.j2',
             '__mocks__',
             '__mocks__/*',
             '.eslintrc.yaml.j2',
             'babel.config.json.j2',
             'jest.config.js.j2',
         ])
 
-    application_types = answers.get('application_types', [])
-    if answers['extension_type'] != 'multiaccount':
-        application_types.append('events')
+    elif 'tfnapp' not in application_types:
+        exclude.extend([
+            'ui/pages/transformations',
+            'ui/pages/transformations/*',
+            'ui/src/pages/transformations',
+            'ui/src/pages/transformations/*',
+            'ui/styles/manual.css.j2',
+        ])
+    else:
+        exclude.extend([
+            'ui/pages/index.html.j2',
+            'ui/pages/settings.html.j2',
+            'ui/src/pages/index.js.j2',
+            'ui/src/pages/settings.js.j2',
+            'ui/tests/pages.spec.js.j2',
+            'ui/tests/utils.spec.js.j2',
+        ])
 
-    for app_type in ['anvil', 'events', 'webapp']:
+    for app_type in ['anvil', 'events', 'webapp', 'tfnapp']:
         if app_type not in application_types:
             exclude.append(
                 os.path.join(
                     '${package_name}',
                     f'{app_type}.py.j2',
                 ),
             )
@@ -147,32 +197,86 @@
             f'Warning/errors have been found while validating the Extension Project {project_dir}.',
             fg='yellow',
         )
     else:
         console.secho(f'Extension Project {project_dir} has been successfully validated.', fg='green')
 
 
-def bump_runner_extension_project(project_dir: str):
+def _update_docker_file_runner_from(dockerfile: str, latest_version: str):
+    to_be_replaced = False
+    last_runner = f'cloudblueconnect/connect-extension-runner:{latest_version}'
+    lines = []
+    with open(dockerfile, 'r') as f:
+        for line in f.readlines():
+            content = line.split()
+            if (
+                content
+                and content[0] == 'FROM'
+                and content[1].startswith(
+                    'cloudblueconnect/connect-extension-runner:',
+                )
+                and content[1].strip() != last_runner
+            ):
+                lines.append(line.replace(content[1], last_runner))
+                to_be_replaced = True
+            else:
+                lines.append(line)
+    if to_be_replaced:
+        with open(dockerfile, 'w') as f:
+            f.writelines(lines)
+    return to_be_replaced
+
+
+def bump_runner_extension_project(project_dir: str):  # noqa: CCR001
     console.secho(f'Bumping runner version on project {project_dir}...\n', fg='blue')
 
+    updated_files = set()
     latest_version = get_pypi_runner_version()
+    latest_runner_version = f'cloudblueconnect/connect-extension-runner:{latest_version}'
     docker_compose_file = os.path.join(project_dir, 'docker-compose.yml')
     if not os.path.isfile(docker_compose_file):
         raise ClickException(f'Mandatory `docker-compose.yml` file on directory `{project_dir}` is missing.')
     try:
         with open(docker_compose_file, 'r') as file_reader:
             data = yaml.load(file_reader, Loader=yaml.FullLoader)
             for service in data['services']:
-                if 'image' in data['services'][service]:
+                if (
+                    'image' in data['services'][service]
+                    and data['services'][service]['image'].startswith(
+                        'cloudblueconnect/connect-extension-runner:',
+                    )
+                    and data['services'][service]['image'] != latest_runner_version
+                ):
                     runner_image = data['services'][service]['image']
                     runner_version = runner_image.split(':')[-1]
                     updated_image = runner_image.replace(runner_version, latest_version)
                     data['services'][service]['image'] = updated_image
+                    updated_files.add(docker_compose_file)
+                elif 'build' in data['services'][service]:
+                    dockerfile = data['services'][service]['build'].get('dockerfile', 'Dockerfile')
+                    dockerfile_path = os.path.join(project_dir, dockerfile)
+                    if not os.path.isfile(dockerfile_path):
+                        raise ClickException(
+                            f'The expected dockerfile `{dockerfile_path}` specified in '
+                            f'{docker_compose_file} is missing.',
+                        )
+                    if (
+                        dockerfile_path not in updated_files
+                        and _update_docker_file_runner_from(dockerfile_path, latest_version)
+                    ):
+                        updated_files.add(dockerfile_path)
         with open(docker_compose_file, 'w') as file_writer:
             yaml.dump(data, file_writer, sort_keys=False)
     except yaml.YAMLError as error:
         raise ClickException(
             '`docker_compose.yml` file is not properly formatted. Please review it.\n'
             f'Error: {error}',
         )
 
-    console.secho(f'Runner version has been successfully updated to {latest_version}', fg='green')
+    if updated_files:
+        console.secho(
+            f'Runner version has been successfully updated to {latest_version}. The following '
+            f'files have been updated:\n{",".join(updated_files)}',
+            fg='green',
+        )
+    else:
+        console.secho(f'Nothing to update to {latest_version}', fg='yellow')
```

### Comparing `connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/anvil.py.j2` & `connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/anvil.py.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/events.py.j2` & `connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/events.py.j2`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 # -*- coding: utf-8 -*-
 #
 # Copyright (c) {% now 'utc', '%Y' %}, {{ author }}
 # All rights reserved.
 #
 from connect.eaas.core.decorators import (
     event,
-    {%- if include_schedules_example == 'y' %}
+    {%- if 'scheduled' in event_types %}
     schedulable,
     {%- endif %}
     {%- if include_variables_example == 'y' %}
     variables,
     {%- endif %}
 )
-{%- if extension_type != 'multiaccount' %}
-from connect.eaas.core.extension import EventsApplicationBase
-{%- endif %}
-{%- if extension_type == 'multiaccount' and 'events' in application_types %}
+{%- if 'events' in application_types %}
 from connect.eaas.core.extension import EventsApplicationBase
 {%- endif %}
 from connect.eaas.core.responses import (
     {%- if background %}
     BackgroundResponse,
     {%- endif %}
     {%- if interactive %}
     InteractiveResponse,
     {%- endif %}
-    {%- if include_schedules_example == 'y' %}
+    {%- if 'scheduled' in event_types %}
     ScheduledExecutionResponse,
     {%- endif %}
 )
 
 
 {% if include_variables_example == 'y' -%}
 @variables([
@@ -82,15 +79,15 @@
             headers={'X-Custom-Header': 'value'},
             body=request,
         )
 
     {% endfor -%}
 
 
-    {% if include_schedules_example == 'y' -%}
+    {% if 'scheduled' in event_types -%}
     @schedulable('Schedulable method', 'It can be used to test DevOps scheduler.')
     {% if use_asyncio == 'y' %}async {% endif %}def execute_scheduled_processing(self, schedule):
         self.logger.info(
             f"Received event for schedule  {schedule['id']}",
         )
         return ScheduledExecutionResponse.done()
```

### Comparing `connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.${project_slug}_dev.env.j2` & `connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.${project_slug}_dev.env.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.eslintrc.yaml.j2` & `connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.eslintrc.yaml.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.github/workflows/test.yml.j2` & `connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.github/workflows/test.yml.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/HOWTO.md.j2` & `connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/HOWTO.md.j2`

 * *Files 1% similar despite different names*

```diff
@@ -21,24 +21,24 @@
 
 > please note that in this way you will run the docker container and if you do changes on the code you will need to stop it and start it again.
 
 
 If you would like to develop and test at the same time, we recommend you run your project using the command:
 
 ```sh
-$ docker compose up {{ project_slug }}_bash
+$ docker compose run {{ project_slug }}_bash
 ```
 
 Once you get the interactive shell an help banner will be displayed to inform you about the included tools that can help you with the development of your extension.
 
 
 Additionally, a basic boilerplate for writing unit tests has been created, you can run the tests using:
 
 ```sh
-$ docker compose up {{ project_slug }}_test
+$ docker compose run {{ project_slug }}_test
 ```
 
 
 ## Community Resources
 
 Please take note of these links in order to get additional information:
```

### Comparing `connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/LICENSE.j2` & `connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/LICENSE.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/docker-compose.yml.j2` & `connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/docker-compose.yml.j2`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 services:
   {{project_slug}}_dev:
     container_name: {{project_slug}}_dev
     build:
       context: .
     working_dir: /extension
-    command: cextrun -d
+    command: cextrun -d --no-rich-logging
     volumes: 
       - .:/extension
     env_file:
       - .{{ project_slug }}_dev.env
 
   {{project_slug}}_bash:
     container_name: {{project_slug}}_bash
```

### Comparing `connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/jest.config.js.j2` & `connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/jest.config.js.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/package.json.j2` & `connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/package.json.j2`

 * *Files 4% similar despite different names*

```diff
@@ -33,10 +33,11 @@
     "html-webpack-plugin": "^5.5.0",
     "jest": "^28.1.0",
     "jest-environment-jsdom": "28.1.0",
     "jest-transform-stub": "^2.0.0",
     "mini-css-extract-plugin": "^2.6.1",
     "style-loader": "^3.3.1",
     "webpack": "^5.74.0",
-    "webpack-cli": "^4.10.0"
+    "webpack-cli": "^4.10.0",
+    "copy-webpack-plugin": "^11.0.0"
   }
 }
```

### Comparing `connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/pyproject.toml.j2` & `connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/pyproject.toml.j2`

 * *Files 17% similar despite different names*

```diff
@@ -6,27 +6,30 @@
 license = "{{ license }}"
 packages = [
     { include = "{{ package_name }}" }
 ]
 readme = "./README.md"
 
 [tool.poetry.plugins."connect.eaas.ext"]
-{%- if extension_type != 'multiaccount' or extension_type == 'multiaccount' and 'events' in application_types %}
+{%- if 'events' in application_types %}
 "eventsapp" = "{{ package_name }}.events:{{ project_slug|replace("_", " ")|title|replace(" ", "") }}EventsApplication"
 {%- endif %}
-{%- if extension_type == 'multiaccount' and 'webapp' in application_types %}
+{%- if 'webapp' in application_types %}
 "webapp" = "{{ package_name }}.webapp:{{ project_slug|replace("_", " ")|title|replace(" ", "") }}WebApplication"
 {%- endif %}
-{%- if extension_type == 'multiaccount' and 'anvil' in application_types %}
+{%- if 'anvil' in application_types %}
 "anvilapp" = "{{ package_name }}.anvil:{{ project_slug|replace("_", " ")|title|replace(" ", "") }}AnvilApplication"
 {%- endif %}
+{%- if 'tfnapp' in application_types %}
+"tfnapp" = "{{ package_name }}.tfnapp:{{ project_slug|replace("_", " ")|title|replace(" ", "") }}TransformationsApplication"
+{%- endif %}
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
-connect-eaas-core = ">=26.10,<27"
+connect-eaas-core = ">=27.14,<28"
 
 [tool.poetry.dev-dependencies]
 pytest = ">=6.1.2,<8"
 pytest-cov = ">=2.10.1,<5"
 pytest-mock = "^3.3.1"
 mock = { version = "^4.0.3", markers = "python_version < '3.8'" }
 coverage = {extras = ["toml"], version = ">=5.3,<7"}
@@ -38,15 +41,14 @@
 flake8-import-order = "~0.18"
 flake8-broken-line = ">=0.3,<0.7"
 flake8-comprehensions = "^3.3.1"
 flake8-debugger = "^4.0.0"
 flake8-eradicate = "^1.0.0"
 flake8-string-format = "^0.3.0"
 pytest-asyncio = "^0.15.1"
-connect-devops-testing-library = "24.*"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 testpaths = "tests"
```

### Comparing `connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/conftest.py.j2` & `connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/conftest.py.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_anvil.py.j2` & `connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_anvil.py.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_events.py.j2` & `connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_events.py.j2`

 * *Files 8% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     ext = {{ project_slug|replace("_", " ")|title|replace(" ", "") }}EventsApplication({% if use_asyncio == 'y' %}async_connect_client{% else %}connect_client{% endif %}, logger, config)
     result = {% if use_asyncio == 'y' %}await {% endif %}ext.handle_{{ interactive_event }}(request)
     assert result.status == 'success'
     assert result.body == request
 
 {% endfor -%}
 
-{% if include_schedules_example == 'y' -%}
+{% if 'scheduled' in event_types -%}
 {% if use_asyncio == 'y' %}
 @pytest.mark.asyncio
 {%- endif %}
 {% if use_asyncio == 'y' %}async {% endif %}def test_execute_scheduled_processing(
     {% if use_asyncio == 'y' %}async_connect_client{% else %}connect_client{% endif %},
     {% if use_asyncio == 'y' %}async_client_mocker_factory{% else %}client_mocker_factory{% endif %},
     logger,
```

### Comparing `connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/pages/index.html.j2` & `connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/pages/index.html.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/pages/settings.html.j2` & `connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/pages/settings.html.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/components.js.j2` & `connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/components.js.j2`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 /*
 Copyright (c) {% now 'utc', '%Y' %}, {{ author }}
 All rights reserved.
 */
 // prepare UI components
+{% if extension_type != 'transformations' -%}
 export const prepareMarketplaces = (marketplaces) => {
   try {
     return marketplaces.reduce((list, marketplace) => `${list}<li class="list-item">
         <div class="list-item-image">
           <img src="${marketplace.icon}" alt="Thumbnail">
         </div>
         <div class="list-item-content">
@@ -64,14 +65,15 @@
 };
 
 export const addEventListener = (id, event, callback) => {
   const element = document.getElementById(id);
   element.addEventListener(event, callback);
 };
 
+{% endif -%}
 // render UI components - show/hide
 export const showComponent = (id) => {
   if (!id) return;
   const element = document.getElementById(id);
   element.classList.remove('hidden');
 };
```

### Comparing `connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/utils.js.j2` & `connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/utils.js.j2`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 
 /*
 Copyright (c) {% now 'utc', '%Y' %}, {{ author }}
 All rights reserved.
 */
 // API calls to the backend
+{%- if extension_type != 'transformations' %}
 export const getSettings = () => fetch('/api/settings').then((response) => response.json());
 
 export const getChart = () => fetch('/api/chart').then((response) => response.json());
 
 export const getMarketplaces = () => fetch('/api/marketplaces').then((response) => response.json());
 
 export const updateSettings = (settings) => fetch('/api/settings', {
@@ -34,7 +35,19 @@
 ) => checkboxes.map((checkbox) => allMarketplaces.find(
   (marketplace) => marketplace.id === checkbox.value,
 ));
 
 export const processCheckboxes = (
   checkboxes,
 ) => Array.from(checkboxes).filter(checkbox => checkbox.checked);
+
+{%- else %}
+/* eslint-disable import/prefer-default-export */
+export const validate = (functionName, data) => fetch(`/api/validate/${functionName}`, {
+  method: 'POST',
+  headers: {
+    'Content-Type': 'application/json',
+  },
+  body: JSON.stringify(data),
+}).then((response) => response.json());
+
+{%- endif %}
```

### Comparing `connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/styles/index.css.j2` & `connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/styles/index.css.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/tests/components.spec.js.j2` & `connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/tests/components.spec.js.j2`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 /*
 Copyright (c) {% now 'utc', '%Y' %}, {{ author }}
 All rights reserved.
 */
-import {
+{%- if 'tfnapp' in application_types %}import {
+  hideComponent,
+  showComponent,
+} from '@/components';
+{%- else %}import {
   addEventListener,
   disableButton,
   enableButton,
   hideComponent,
   prepareChart,
   prepareMarketplaces,
   prepareMarketplacesWithSwitch,
   renderChart,
   renderMarketplaces,
   showComponent,
 } from '@/components';
+{%- endif %}
 
 
 describe('components.js', () => {
-  describe('prepareMarketplaces', () => {
+  {% if extension_type != 'transformations' -%}describe('prepareMarketplaces', () => {
     test('returns "" if marketplaces is empty', () => {
       const result = prepareMarketplaces([]);
       expect(result).toBe('');
     });
 
     test('returns "" if marketplaces is not array', () => {
       const result = prepareMarketplaces({});
@@ -150,14 +155,15 @@
       document.body.innerHTML = '<button id="button"></button>';
       const callback = jest.fn();
       addEventListener('button', 'click', callback);
       document.getElementById('button').click();
       expect(callback).toBeCalled();
     });
   });
+  {% endif -%}
 
   describe('showLoader', () => {
     beforeEach(() => {
       document.body.innerHTML = '<div id="loader" class="hidden"></div>';
       showComponent('loader');
     });
     it('shows a loader', () => {
```

### Comparing `connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/tests/pages.spec.js.j2` & `connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/tests/pages.spec.js.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/tests/utils.spec.js.j2` & `connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/tests/utils.spec.js.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/webpack.config.js.j2` & `connect_cli-27.0/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/webpack.config.js.j2`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 All rights reserved.
 */
 const path = require('path');
 const htmlWebpackPlugin = require('html-webpack-plugin');
 const MiniCssExtractPlugin = require("mini-css-extract-plugin");
 const CssMinimizerPlugin = require("css-minimizer-webpack-plugin");
 const ESLintPlugin = require('eslint-webpack-plugin');
+const CopyWebpackPlugin = require('copy-webpack-plugin');
 
 const generateHtmlPlugin = (title) => {
   const moduleName = title.toLowerCase();
 
   return new htmlWebpackPlugin({
     title,
     filename: `${moduleName}.html`,
@@ -23,21 +24,34 @@
   res = [];
   pagesArray.forEach(page => {
     res.push(generateHtmlPlugin(page));
   })
   return res;
 }
 
-const pages = populateHtmlPlugins(["Index", "Settings"]);
+const pages = populateHtmlPlugins([
+  {%- if 'tfnapp' in application_types %}
+  "Transformations/Copy",
+  "Transformations/Manual",
+  {%- else %}
+  "Index",
+  "Settings",
+  {%- endif %}
+ ]);
 
 module.exports = {
   mode: 'production',
   entry: {
+    {%- if 'tfnapp' in application_types %}
+    ['transformations/copy']: __dirname + "/ui/src/pages/transformations/copy.js",
+    ['transformations/manual']: __dirname + "/ui/src/pages/transformations/manual.js",
+    {%- else %}
     index: __dirname + "/ui/src/pages/index.js",
-    settings: __dirname + "/ui/src/pages/settings.js"
+    settings: __dirname + "/ui/src/pages/settings.js",
+    {%- endif %}
   },
   output: {
     filename: '[name].[contenthash].js',
     path: path.resolve(__dirname, '{{ package_name }}/static'),
     clean: true,
   },
   optimization: {
@@ -52,16 +66,21 @@
     },
      minimizer: [
       new CssMinimizerPlugin(),
     ],
   },
   plugins: [
     ...pages,
+    new CopyWebpackPlugin({
+      patterns: [
+        { from: __dirname + "/ui/images", to: "images" },
+      ],
+    }),
     new MiniCssExtractPlugin({
-      filename: "index.css",
+      filename: "[name].[contenthash].css",
       chunkFilename: "[id].css",
     }),
     new ESLintPlugin(),
   ],
   module: {
     rules: [
       {
```

### Comparing `connect_cli-26.9/connect/cli/plugins/project/extension/wizard.py` & `connect_cli-27.0/connect/cli/plugins/project/extension/wizard.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from functools import partial
 from urllib.parse import urlparse
 
 from interrogatio.validators import RequiredValidator
 
 from connect.cli.plugins.project.extension.utils import (
+    check_event_type_applicable,
     check_eventsapp_feature_not_selected,
-    check_extension_events_applicable,
-    check_extension_interactive_events_applicable,
     check_extension_not_multi_account,
     check_webapp_feature_not_selected,
+    get_application_types,
+    get_available_event_types,
     get_background_events,
+    get_default_application_types,
     get_extension_types,
     get_interactive_events,
 )
+from connect.cli.plugins.project.extension.validators import AppTypesValidator, UISupportValidator
 from connect.cli.plugins.project.utils import slugify
 from connect.cli.plugins.project.validators import PythonIdentifierValidator
 
 
 EXTENSION_BOOTSTRAP_WIZARD_INTRO = (
     'Welcome to the Connect Extension Project Bootstrap utility.\n'
     'Using this utility multiple data will be collected in order to create a project\n'
@@ -24,14 +27,15 @@
     'to start writing your code.\n\n'
     'For more information please visit https://connect.cloudblue.com/community/modules/devops\n'
     'Have a nice trip!\n'
 )
 
 
 def get_summary(data):  # pragma: no cover
+
     def value(variable_name, formatted=False):
         if not data.get(variable_name):
             return ''
 
         data_value = data[variable_name]['formatted_value' if formatted else 'value']
 
         return data_value or '-'
@@ -49,32 +53,29 @@
     <b>Environment ID:</b> {value('environment_id')}
     <b>Server Address:</b> {value('server_address')}
 """
 
     extension = f"""<b><blue>Extension</blue></b>
     <b>Type:</b> {value('extension_type', formatted=True)}
 """
-    if value('extension_type') == 'multiaccount':
+    if value('extension_type') in ('multiaccount', 'transformations'):
         extension += f"""    <b>Audience:</b> {value('extension_audience', formatted=True)}
 """
         extension += f"""    <b>Features:</b> {value('application_types', formatted=True)}
 """
-    if 'webapp' in value('application_types'):
-        extension += f"""    <b>UI support:</b> {value('webapp_supports_ui', formatted=True)}
+
+    event_answers = f"""    <b>Events:</b> {value('event_types', formatted=True)}
 """
 
-    event_answers = ''
-    for category in ['background', 'interactive']:
-        event_answers += f"""<b><blue>{value('extension_type', formatted=True)} {category} events:</blue></b>
-    {value(category, formatted=True)}
+    if 'webapp' in value('application_types'):
+        extension += f"""    <b>UI support:</b> {value('webapp_supports_ui', formatted=True)}
 """
 
     examples = f"""<b><blue>Examples</blue></b>
-    <b>Schedulables:</b> {value('include_schedules_example', formatted=True)} - """
-    examples += f"""<b>Variables:</b> {value('include_variables_example', formatted=True)}"""
+    <b>Variables:</b> {value('include_variables_example', formatted=True)}"""
 
     return common + extension + event_answers + examples
 
 
 def get_questions(config, definitions):
     project = [
         {
@@ -87,25 +88,53 @@
         },
         {
             'name': 'project_slug',
             'label': 'Project: root',
             'type': 'input',
             'description': 'Choose a name for the root folder of your Extension module.',
             'default': lambda ctx: slugify(ctx['project_name']),
-            'validators': (RequiredValidator(message='Please, provide a project root folder.'),),
+            'validators': [RequiredValidator(message='Please, provide a project root folder.')],
         },
         {
             'name': 'description',
             'label': 'Project: description',
             'type': 'input',
             'description': 'Briefly describe your Extension:',
             'default': 'Project description',
             'validators': (RequiredValidator(message='Please, provide a description.'),),
         },
         {
+            'name': 'version',
+            'label': 'Project: version',
+            'type': 'input',
+            'description': 'Introduce a version identifier for your Extension:',
+            'default': '0.1.0',
+            'validators': (RequiredValidator(message='Please, provide a version.'),),
+        },
+        {
+            'name': 'author',
+            'label': 'Project: author',
+            'type': 'input',
+            'description': 'Enter the name of the Extension author:',
+            'default': 'Globex Corporation',
+            'validators': (RequiredValidator(message='Please, provide an author name.'),),
+        },
+        {
+            'name': 'license',
+            'label': 'Project: license',
+            'type': 'selectone',
+            'description': 'Choose an Open Source license for your Extension:',
+            'values': [
+                ('Apache Software License 2.0', 'Apache Software License 2.0'),
+                ('MIT', 'MIT'),
+                ('BSD', 'BSD'),
+            ],
+            'formatting_template': '${label}',
+        },
+        {
             'name': 'package_name',
             'label': 'Project: package',
             'type': 'input',
             'description': (
                 'Choose a name for the root python package of your extension module.'
                 ' This must be a valid python\nidentifier:'
             ),
@@ -123,42 +152,14 @@
             'values': [
                 ('n', 'No'),
                 ('y', 'Yes'),
             ],
             'formatting_template': '${label}',
         },
         {
-            'name': 'author',
-            'label': 'Project: author',
-            'type': 'input',
-            'description': 'Enter the name of the Extension author:',
-            'default': 'Globex Corporation',
-            'validators': (RequiredValidator(message='Please, provide an author name.'),),
-        },
-        {
-            'name': 'version',
-            'label': 'Project: version',
-            'type': 'input',
-            'description': 'Introduce a version identifier for your Extension:',
-            'default': '0.1.0',
-            'validators': (RequiredValidator(message='Please, provide a version.'),),
-        },
-        {
-            'name': 'license',
-            'label': 'Project: license',
-            'type': 'selectone',
-            'description': 'Choose an Open Source license for your Extension:',
-            'values': [
-                ('Apache Software License 2.0', 'Apache Software License 2.0'),
-                ('MIT', 'MIT'),
-                ('BSD', 'BSD'),
-            ],
-            'formatting_template': '${label}',
-        },
-        {
             'name': 'use_github_actions',
             'label': 'Project: CI',
             'type': 'selectone',
             'description': (
                 'If you plan to host the Extension code on GitHub, are you also planning\n'
                 'to use GitHub actions as your continuous integration system ?'
             ),
@@ -168,14 +169,22 @@
             ],
             'formatting_template': '${label}',
         },
     ]
 
     environment = [
         {
+            'name': 'server_address',
+            'label': 'Config: API hostname',
+            'type': 'input',
+            'description': 'Connect API hostname: ',
+            'default': urlparse(config.active.endpoint).netloc,
+            'validators': (RequiredValidator(message='Please, provide the API hostname.'),),
+        },
+        {
             'name': 'api_key',
             'label': 'Config: API key',
             'type': 'input',
             'description': (
                 'Enter the API key that will be used to authenticate API calls to Connect:\n'
                 'The API key can be created within the integration module of Connect.\n'
                 'It defaults to the current active CLI account.'
@@ -185,27 +194,19 @@
         },
         {
             'name': 'environment_id',
             'label': 'Config: environment ID',
             'type': 'input',
             'description': (
                 'Enter the DevOps environment identifier to which your Extension will connect:\n'
-                'It can be found in the DevOps module of Connect within the Local Access widget.\n'
-                'See: https://connect.cloudblue.com/community/modules/devops/user-interface/#Service_Details'
+                'It can be found in the DevOps module of Connect within the Local Access widget.\nSee: '
+                'https://connect.cloudblue.com/community/modules/devops/user-interface/#Environment_ID_Specification'
             ),
             'validators': (RequiredValidator(message='Please, provide a DevOps environment ID.'),),
         },
-        {
-            'name': 'server_address',
-            'label': 'Config: API hostname',
-            'type': 'input',
-            'description': 'Connect API hostname: ',
-            'default': urlparse(config.active.endpoint).netloc,
-            'validators': (RequiredValidator(message='Please, provide the API hostname.'),),
-        },
     ]
 
     extension_type = [
         {
             'name': 'extension_type',
             'label': 'Extension: Extension type',
             'type': 'selectone',
@@ -228,79 +229,79 @@
             'validators': (RequiredValidator(message='Please, select at least one option.'),),
         },
         {
             'name': 'application_types',
             'label': 'Extension: Features',
             'type': 'selectmany',
             'description': 'Which features do you want to support in your extension: ',
-            'values': [
-                ('events', 'Events Processing'),
-                ('webapp', 'Web Application'),
-                ('anvil', 'Anvil Application'),
-            ],
+            'values': get_application_types,
+            'default': get_default_application_types,
             'formatting_template': '${label}',
-            'disabled': check_extension_not_multi_account,
+            'validators': (
+                RequiredValidator(message='Please, select at least one option.'),
+                AppTypesValidator(),
+            ),
+        },
+        {
+            'name': 'event_types',
+            'label': 'Extension: Events type',
+            'type': 'selectmany',
+            'description': 'Which types of event do you want to support in your extension: ',
+            'values': partial(get_available_event_types, definitions),
+            'formatting_template': '${label}',
+            'disabled': check_eventsapp_feature_not_selected,
             'validators': (RequiredValidator(message='Please, select at least one option.'),),
         },
         {
             'name': 'webapp_supports_ui',
             'label': 'Extension: WebApp',
             'type': 'selectone',
             'description': 'Does your web application plug into the Connect UI ? ',
             'values': [
                 ('n', 'No'),
                 ('y', 'Yes'),
             ],
+            'default': 'y',
             'formatting_template': '${label}',
             'disabled': check_webapp_feature_not_selected,
+            'validators': (UISupportValidator(),),
         },
     ]
 
     event_questions = [
         {
             'name': 'background',
             'label': 'Extension: Background events',
             'type': 'selectmany',
             'description': (
                 'What types of background'
                 'events do you want your Extension to process?'
             ),
             'values': partial(get_background_events, definitions),
             'formatting_template': '${label}',
-            'disabled': check_extension_events_applicable,
+            'disabled': partial(check_event_type_applicable, 'background'),
             'validators': (RequiredValidator(message='Please, select at least one option.'),),
         },
         {
             'name': 'interactive',
             'label': 'Extension: Interactive events',
             'type': 'selectmany',
             'description': (
                 'What types of interactive'
                 'events do you want your Extension to process?'
             ),
             'values': partial(get_interactive_events, definitions),
-            'disabled': partial(check_extension_interactive_events_applicable, definitions),
+            'disabled': partial(check_event_type_applicable, 'interactive'),
             'formatting_template': '${label}',
+            'validators': (RequiredValidator(message='Please, select at least one option.'),),
         },
     ]
 
     examples = [
         {
-            'name': 'include_schedules_example',
-            'label': 'Examples: schedulables',
-            'type': 'selectone',
-            'description': 'Do you want to include an example of schedulable method ? ',
-            'values': [
-                ('n', 'No'),
-                ('y', 'Yes'),
-            ],
-            'disabled': check_eventsapp_feature_not_selected,
-            'formatting_template': '${label}',
-        },
-        {
             'name': 'include_variables_example',
             'label': 'Examples: variables',
             'type': 'selectone',
             'description': 'Do you want to include an example of environment variables ? ',
             'values': [
                 ('n', 'No'),
                 ('y', 'Yes'),
```

### Comparing `connect_cli-26.9/connect/cli/plugins/project/renderer.py` & `connect_cli-27.0/connect/cli/plugins/project/renderer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 
 # This file is part of the Ingram Micro Cloud Blue Connect connect-cli.
 # Copyright (c) 2019-2022 Ingram Micro. All Rights Reserved.
-import os
 import fnmatch
-from string import Template
-from pathlib import Path
+import os
 import shutil
 import tempfile
+from pathlib import Path
+from string import Template
 
 from jinja2 import Environment, FileSystemLoader, select_autoescape
 
 from connect.cli.core.terminal import console
 from connect.cli.plugins.project.utils import purge_dir
 
 
@@ -89,16 +89,17 @@
                 console.print(
                     f'Folder {directory.replace(output_dir, "")}'
                     ' created [bold green]\u2713[/bold green]',
                 )
 
     def render(self):
         if self.overwrite:
-            purge_dir(self.output_dir)
-            console.print(f'Directory {self.output_dir} deleted.')
+            prj_dir = os.path.join(self.output_dir, self.context['project_slug'])
+            purge_dir(prj_dir)
+            console.print(f'Directory {prj_dir} deleted.')
 
         with tempfile.TemporaryDirectory() as tmpdir:
             self._create_directories(output_dir=tmpdir)
             if self.pre_render_function:
                 self.pre_render_function(tmpdir, self.context)
                 console.print('pre_render_function executed [bold green]\u2713[/bold green]')
             with console.status('[magenta]Generating files'):
```

### Comparing `connect_cli-26.9/connect/cli/plugins/project/report/helpers.py` & `connect_cli-27.0/connect/cli/plugins/project/report/helpers.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 #  Copyright © 2022 CloudBlue. All rights reserved.
 
+import functools
 import json
 import os
-import functools
 
 from click import ClickException
 from interrogatio.core.dialog import dialogus
 from openpyxl import Workbook
 
 from connect.cli import get_version
 from connect.cli.core.terminal import console
+from connect.cli.plugins.project.renderer import BoilerplateRenderer
+from connect.cli.plugins.project.report.validations import validate_reports_json, validators
 from connect.cli.plugins.project.report.wizard import (
     ADD_REPORT_QUESTIONS,
     BOOTSTRAP_QUESTIONS,
     BOOTSTRAP_SUMMARY,
     REPORT_ADD_WIZARD_INTRO,
     REPORT_BOOTSTRAP_WIZARD_INTRO,
     REPORT_SUMMARY,
 )
 from connect.cli.plugins.project.utils import show_validation_result_table
-from connect.cli.plugins.project.report.validations import validate_reports_json, validators
-from connect.cli.plugins.project.renderer import BoilerplateRenderer
 
 
 def bootstrap_report_project(output_dir, overwrite):
     console.secho('Bootstraping report project...\n', fg='blue')
 
     answers = dialogus(
         BOOTSTRAP_QUESTIONS,
```

### Comparing `connect_cli-26.9/connect/cli/plugins/project/report/templates/add/${initial_report_slug}/entrypoint.py.j2` & `connect_cli-27.0/connect/cli/plugins/project/report/templates/add/${initial_report_slug}/entrypoint.py.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/entrypoint.py.j2` & `connect_cli-27.0/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/entrypoint.py.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/templates/pdf/template.html.j2.j2` & `connect_cli-27.0/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/templates/pdf/template.html.j2.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/.github/workflows/build.yml.j2` & `connect_cli-27.0/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/.github/workflows/build.yml.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/LICENSE.j2` & `connect_cli-27.0/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/LICENSE.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/pyproject.toml.j2` & `connect_cli-27.0/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/pyproject.toml.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/reports.json.j2` & `connect_cli-27.0/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/reports.json.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/tests/conftest.py.j2` & `connect_cli-27.0/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/tests/conftest.py.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/tests/test_${project_slug}.py.j2` & `connect_cli-27.0/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/tests/test_${project_slug}.py.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/cli/plugins/project/report/validations.py` & `connect_cli-27.0/connect/cli/plugins/project/report/validations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 
 #  Copyright © 2022 CloudBlue. All rights reserved.
 
+import importlib
+import inspect
 import json
 import os
 import sys
-import inspect
-import importlib
-
-from poetry.core.constraints.version import parse_constraint, Version
 
 from connect.reports.parser import parse
-from connect.reports.validator import (
-    validate,
-    validate_with_schema,
-)
+from connect.reports.validator import validate, validate_with_schema
+from poetry.core.constraints.version import Version, parse_constraint
+
+from connect.cli.core.utils import get_last_cli_version
 from connect.cli.plugins.project.validators import (
-    get_code_context,
-    load_project_toml_file,
     ValidationItem,
     ValidationResult,
+    get_code_context,
+    load_project_toml_file,
 )
-from connect.cli.core.utils import get_last_cli_version
 
 
 def validate_pyproject_toml(project_dir, context):
     messages = []
     data = load_project_toml_file(project_dir)
     if isinstance(data, ValidationResult):
         return data
```

### Comparing `connect_cli-26.9/connect/cli/plugins/project/report/wizard.py` & `connect_cli-27.0/connect/cli/plugins/project/report/wizard.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from interrogatio.validators import RequiredValidator
 
 from connect.cli.plugins.project.utils import slugify
 from connect.cli.plugins.project.validators import PythonIdentifierValidator
 
+
 REPORT_BOOTSTRAP_WIZARD_INTRO = (
     'Welcome to the Connect Reports Project Bootstrap utility.\n'
     'Using this utility multiple data will be collected in order to create a project\n'
     'skeleton for your Connect Reports. This skeleton will contain all needed things\n'
     'to start writing your code.\n\n'
     'For more information please visit https://connect.cloudblue.com/community/sdk/connect-reports-sdk\n'
     'Have a nice trip!\n'
```

### Comparing `connect_cli-26.9/connect/cli/plugins/project/utils.py` & `connect_cli-27.0/connect/cli/plugins/project/utils.py`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import shutil
 import stat
 
 from rich import box
 from rich.markdown import Markdown
-from rich.table import Table
 from rich.syntax import Syntax
+from rich.table import Table
 
 from connect.cli.core.terminal import console
 
 
 def force_delete(func, path, exc_info):
     os.chmod(path, stat.S_IWRITE)
     func(path)
```

### Comparing `connect_cli-26.9/connect/cli/plugins/project/validators.py` & `connect_cli-27.0/connect/cli/plugins/project/validators.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,44 @@
 import dataclasses
-import os
 import inspect
+import os
 from typing import List, Literal, Optional
 
+import toml
 from interrogatio.core.exceptions import ValidationError
 from interrogatio.validators import Validator
-import toml
 
 
 class PythonIdentifierValidator(Validator):
 
     def validate(self, value, context=None):
         if not value:
             return
         if not value.isidentifier():
             raise ValidationError('Introduced data is not a valid Python identifier')
 
 
+class ProjectDirValidator(Validator):
+
+    def __init__(
+        self,
+        output_dir,
+        message='The root folder for your project already exist.',
+    ):
+        super().__init__(message=message)
+        self.output_dir = output_dir
+
+    def validate(self, value, context=None):
+        if not value:
+            return
+        project_dir = os.path.join(self.output_dir, value)
+        if os.path.exists(project_dir):
+            raise ValidationError(self.message)
+
+
 @dataclasses.dataclass
 class ValidationItem:
     level: Literal['WARNING', 'ERROR']
     message: str
     file: Optional[str] = None
     start_line: Optional[int] = None
     lineno: Optional[int] = None
@@ -59,22 +77,21 @@
 
 def load_project_toml_file(path):
     descriptor_file = os.path.join(path, 'pyproject.toml')
     if not os.path.isfile(descriptor_file):
         return ValidationResult(
             items=[
                 ValidationItem(
-                    'ERROR',
+                    'WARNING',
                     (
-                        f'The mandatory *pyproject.toml* project descriptor file is not present in the folder {path}.'
+                        f'The *pyproject.toml* project descriptor file is not present in the folder {path}.'
                     ),
                     descriptor_file,
                 ),
             ],
-            must_exit=True,
         )
     try:
         return toml.load(descriptor_file)
     except toml.TomlDecodeError:
         return ValidationResult(
             items=[
                 ValidationItem(
```

### Comparing `connect_cli-26.9/connect/cli/plugins/report/commands.py` & `connect_cli-27.0/connect/cli/plugins/report/commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 import os
 from datetime import datetime
 
 import click
 
 from connect.cli.core import group
 from connect.cli.core.config import pass_config
-from connect.cli.plugins.report.helpers import (
-    execute_report,
-    list_reports,
-    show_report_info,
-)
+from connect.cli.plugins.report.helpers import execute_report, list_reports, show_report_info
 
 
 DEFAULT_REPORT_DIR = os.path.normpath(
     os.path.join(os.path.dirname(__file__), '../../../.data/connect_reports'),
 )
```

### Comparing `connect_cli-26.9/connect/cli/plugins/report/helpers.py` & `connect_cli-27.0/connect/cli/plugins/report/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 import inspect
 import json
 import os
 from datetime import datetime
 
 import pytz
 from click import ClickException
+from connect.client import AsyncConnectClient, ConnectClient
+from connect.reports.constants import CLI_ENV
+from connect.reports.datamodels import Account, Report
+from connect.reports.parser import parse
+from connect.reports.renderers import get_renderer
+from connect.reports.validator import validate, validate_with_schema
 
-from connect.cli.core.http import get_user_agent, RequestLogger
+from connect.cli.core.http import RequestLogger, get_user_agent
 from connect.cli.core.terminal import console
 from connect.cli.core.utils import field_to_check_mark
 from connect.cli.plugins.report.constants import AVAILABLE_REPORTS
 from connect.cli.plugins.report.utils import (
+    Progress,
     get_renderer_by_id,
     get_report_by_id,
     get_report_entrypoint,
     handle_report_exception,
-    Progress,
 )
 from connect.cli.plugins.report.wizard import get_report_inputs
-from connect.client import AsyncConnectClient, ConnectClient
-from connect.reports.constants import CLI_ENV
-from connect.reports.datamodels import Account, Report
-from connect.reports.parser import parse
-from connect.reports.renderers import get_renderer
-from connect.reports.validator import validate, validate_with_schema
 
 
 def load_repo(repo_dir):
     cfg = os.path.join(repo_dir, 'reports.json')
     if not os.path.isfile(cfg):
         raise ClickException(
             f'The directory `{repo_dir}` is not a reports project root directory.',
```

### Comparing `connect_cli-26.9/connect/cli/plugins/report/utils.py` & `connect_cli-27.0/connect/cli/plugins/report/utils.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import json
 import sys
 import traceback
 from datetime import timezone
 from importlib import import_module
 
 from click import ClickException
+from connect.client import ClientError
 
 from connect.cli.core.terminal import console
-from connect.client import ClientError
 
 
 def convert_to_utc_input(date):
     return date.astimezone(timezone.utc).isoformat()
 
 
 def get_report_by_id(repo, local_id):
```

### Comparing `connect_cli-26.9/connect/cli/plugins/report/wizard.py` & `connect_cli-27.0/connect/cli/plugins/report/wizard.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-import json
 import datetime
+import json
 import time
 
 from click import ClickException
+from connect.client import R
 from interrogatio import dialogus
+from interrogatio.core.exceptions import ValidationError
 from interrogatio.validators import (
     DateTimeRangeValidator,
     DateTimeValidator,
     RequiredValidator,
     Validator,
 )
-from interrogatio.core.exceptions import ValidationError
 
 from connect.cli.plugins.report.utils import convert_to_utc_input
-from connect.client import R
 
 
 class ObjectValidator(Validator):
 
     def validate(self, value, context=None):
         if not value:
             return
```

### Comparing `connect_cli-26.9/connect/cli/plugins/shared/base.py` & `connect_cli-27.0/connect/cli/plugins/shared/base.py`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/cli/plugins/shared/constants.py` & `connect_cli-27.0/connect/cli/plugins/shared/constants.py`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/cli/plugins/shared/export.py` & `connect_cli-27.0/connect/cli/plugins/shared/export.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from copy import copy
 from io import BytesIO
 
 from click import ClickException
+from connect.client import ClientError
 from openpyxl import load_workbook
 from openpyxl.styles import Alignment
+from openpyxl.utils import get_column_letter
 from openpyxl.worksheet.datavalidation import DataValidation
 from openpyxl.worksheet.filters import AutoFilter
-from openpyxl.utils import get_column_letter
 
-from connect.client import ClientError
 from connect.cli.core.http import format_http_status, handle_http_error
 from connect.cli.plugins.translation.utils import insert_column_ws
 
+
 EXCEL_CONTENT_TYPE = 'application/vnd.openxmlformats-officedocument.spreadsheetml.sheet'
 
 
 def get_translation_workbook(client, translation_id):
     try:
         xls_data = client.ns('localization').translations[translation_id].action('attributes').get(
             headers={'Accept': EXCEL_CONTENT_TYPE},
```

### Comparing `connect_cli-26.9/connect/cli/plugins/shared/sync_stats.py` & `connect_cli-27.0/connect/cli/plugins/shared/sync_stats.py`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/connect/cli/plugins/shared/translation_attr_sync.py` & `connect_cli-27.0/connect/cli/plugins/shared/translation_attr_sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 # -*- coding: utf-8 -*-
 
 # This file is part of the Ingram Micro Cloud Blue Connect connect-cli.
 # Copyright (c) 2019-2022 Ingram Micro. All Rights Reserved.
 import math
 from collections import namedtuple
+from zipfile import BadZipFile
 
 import click
-
 from connect.client import ClientError
-
-from zipfile import BadZipFile
-
 from openpyxl import load_workbook
 from openpyxl.utils.exceptions import InvalidFileException
 
-from connect.cli.plugins.shared.sync_stats import SynchronizerStats
-from connect.cli.plugins.shared.exceptions import SheetNotFoundError
 from connect.cli.plugins.shared.constants import ATTRIBUTES_SHEET_COLUMNS
+from connect.cli.plugins.shared.exceptions import SheetNotFoundError
+from connect.cli.plugins.shared.sync_stats import SynchronizerStats
 
 
 class TranslationAttributesSynchronizer:
     """
     Synchronize the attributes of a translation from excel file.
     """
     _MAX_BATCH_SIZE = 10
```

### Comparing `connect_cli-26.9/connect/cli/plugins/shared/translation_sync.py` & `connect_cli-27.0/connect/cli/plugins/shared/translation_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 
 # This file is part of the Ingram Micro Cloud Blue Connect connect-cli.
 # Copyright (c) 2019-2022 Ingram Micro. All Rights Reserved.
 
 from collections import defaultdict, namedtuple
 from functools import partial
 
-from connect.cli.plugins.shared.constants import TRANSLATION_HEADERS
+from connect.client import ClientError
+
 from connect.cli.plugins.shared.base import ProductSynchronizer
+from connect.cli.plugins.shared.constants import TRANSLATION_HEADERS
 from connect.cli.plugins.shared.utils import fill_translation_row, setup_locale_data_validation
-from connect.client import ClientError
+
 
 fields = (v.replace(' ', '_').lower() for v in TRANSLATION_HEADERS.values())
 
 _RowData = namedtuple('RowData', fields)
 
 
 class TranslationsSynchronizer(ProductSynchronizer):
```

### Comparing `connect_cli-26.9/connect/cli/plugins/shared/translations_synchronizers.py` & `connect_cli-27.0/connect/cli/plugins/shared/translations_synchronizers.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from click import ClickException
 
-from connect.cli.plugins.shared.translation_sync import TranslationsSynchronizer
+from connect.cli.plugins.shared.exceptions import SheetNotFoundError
 from connect.cli.plugins.shared.translation_attr_sync import TranslationAttributesSynchronizer
+from connect.cli.plugins.shared.translation_sync import TranslationsSynchronizer
 from connect.cli.plugins.shared.utils import (
     get_translation_attributes_sheets,
     wait_for_autotranslation,
 )
-from connect.cli.plugins.shared.exceptions import SheetNotFoundError
 
 
 def translations_sync(client, progress, input_file, stats, save):
     synchronizer = TranslationsSynchronizer(client, progress, stats)
     synchronizer.open(input_file, 'Translations')
     synchronizer.sync()
     if save:
```

### Comparing `connect_cli-26.9/connect/cli/plugins/shared/utils.py` & `connect_cli-27.0/connect/cli/plugins/shared/utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 # This file is part of the Ingram Micro Cloud Blue Connect connect-cli.
 # Copyright (c) 2019-2022 Ingram Micro. All Rights Reserved.
 import re
 from time import sleep
 
 import click
+from connect.client import ClientError
 from openpyxl import load_workbook
 from openpyxl.styles import Alignment
 from openpyxl.utils import quote_sheetname
 from openpyxl.worksheet.datavalidation import DataValidation
 
-from connect.client import ClientError
 from connect.cli.core.http import handle_http_error
 from connect.cli.plugins.shared.constants import (
     ACTIONS_HEADERS,
     CAPABILITIES_COLS_HEADERS,
     CONFIGURATION_HEADERS,
     ITEMS_COLS_HEADERS,
     MEDIA_COLS_HEADERS,
```

### Comparing `connect_cli-26.9/connect/cli/plugins/translation/activate.py` & `connect_cli-27.0/connect/cli/plugins/translation/activate.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 import click
-
 from connect.client import ClientError
-from connect.cli.core.http import (
-    format_http_status,
-    handle_http_error,
-)
+
+from connect.cli.core.http import format_http_status, handle_http_error
 
 
 def activate_translation(client, translation_id):
     try:
         payload = {
             'status': 'active',
         }
```

### Comparing `connect_cli-26.9/connect/cli/plugins/translation/commands.py` & `connect_cli-27.0/connect/cli/plugins/translation/commands.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import click
 
 from connect.cli.core import group
 from connect.cli.core.config import pass_config
 from connect.cli.core.terminal import console
 from connect.cli.core.utils import field_to_check_mark
 from connect.cli.plugins.shared.sync_stats import SynchronizerStats
-from connect.cli.plugins.shared.utils import wait_for_autotranslation
 from connect.cli.plugins.shared.translation_attr_sync import TranslationAttributesSynchronizer
+from connect.cli.plugins.shared.utils import wait_for_autotranslation
 from connect.cli.plugins.translation.activate import activate_translation
 from connect.cli.plugins.translation.export import dump_translation
 from connect.cli.plugins.translation.primarize import primarize_translation
 from connect.cli.plugins.translation.translation_sync import TranslationSynchronizer
 
 
 @group(name='translation', short_help='Manage translations.')
```

### Comparing `connect_cli-26.9/connect/cli/plugins/translation/constants.py` & `connect_cli-27.0/connect/cli/plugins/translation/constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,14 @@
 # -*- coding: utf-8 -*-
 
 # This file is part of the Ingram Micro Cloud Blue Connect connect-cli.
 # Copyright (c) 2019-2022 Ingram Micro. All Rights Reserved.
 
 from collections import namedtuple
 
-TRANSLATION_TABLE_HEADER = """
-
-
-
-| ID | Context_ID | Context_Type | Context_Name |Locale  | Auto | Status | Primary | Owner |
-|:--------|:-----------|:-----------:|:-----------:|:-----------:|:-----------:|:-----------:|:-----------:|:-----------:|
-"""
 
 FieldSettings = namedtuple('FieldSettings', ['row_idx', 'title'])
 
 GENERAL_SHEET_FIELDS = {
     'translation_id': FieldSettings(1, 'Translation'),
     'owner_id': FieldSettings(2, 'Translation Owner ID'),
     'owner_name': FieldSettings(3, 'Translation Owner Name'),
```

### Comparing `connect_cli-26.9/connect/cli/plugins/translation/export.py` & `connect_cli-27.0/connect/cli/plugins/translation/export.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,15 @@
 
 # This file is part of the Ingram Micro Cloud Blue Connect connect-cli.
 # Copyright (c) 2019-2022 Ingram Micro. All Rights Reserved.
 
 from openpyxl.worksheet.datavalidation import DataValidation
 
 from connect.cli.core.utils import validate_output_options
-from connect.cli.plugins.shared.export import (
-    alter_attributes_sheet,
-    get_translation_workbook,
-)
+from connect.cli.plugins.shared.export import alter_attributes_sheet, get_translation_workbook
 
 
 def dump_translation(
     client, translation_id, output_file, output_path=None,
 ):
     output_file = validate_output_options(output_path, output_file, default_dir_name=translation_id)
     wb = get_translation_workbook(client, translation_id)
```

### Comparing `connect_cli-26.9/connect/cli/plugins/translation/primarize.py` & `connect_cli-27.0/connect/cli/plugins/translation/primarize.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 import click
-
 from connect.client import ClientError, ConnectClient
-from connect.cli.core.http import (
-    format_http_status,
-    handle_http_error,
-    RequestLogger,
-)
+
+from connect.cli.core.http import RequestLogger, format_http_status, handle_http_error
 
 
 def primarize_translation(
     api_url, api_key,
     translation_id,
 ):
     try:
```

### Comparing `connect_cli-26.9/connect/cli/plugins/translation/translation_sync.py` & `connect_cli-27.0/connect/cli/plugins/translation/translation_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 # -*- coding: utf-8 -*-
 
 # This file is part of the Ingram Micro Cloud Blue Connect connect-cli.
 # Copyright (c) 2019-2022 Ingram Micro. All Rights Reserved.
 
 from types import SimpleNamespace
+from zipfile import BadZipFile
 
 import click
-
 from connect.client import ClientError
-
-from zipfile import BadZipFile
-
 from openpyxl import load_workbook
 from openpyxl.utils.exceptions import InvalidFileException
 
 from connect.cli.core.http import handle_http_error
 from connect.cli.core.terminal import console
-from connect.cli.plugins.shared.sync_stats import SynchronizerStats
 from connect.cli.plugins.shared.exceptions import SheetNotFoundError
+from connect.cli.plugins.shared.sync_stats import SynchronizerStats
 from connect.cli.plugins.translation.constants import GENERAL_SHEET_FIELDS
 
 
 class TranslationSynchronizer:
     """
     Synchronize a translation from excel file. It may update an existing
     translation or create a new one depending on some checks.
```

### Comparing `connect_cli-26.9/connect/cli/plugins/translation/utils.py` & `connect_cli-27.0/connect/cli/plugins/translation/utils.py`

 * *Files identical despite different names*

### Comparing `connect_cli-26.9/pyproject.toml` & `connect_cli-27.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "connect-cli"
-version = "26.9"
+version = "27.0"
 description = "CloudBlue Connect Command Line Interface"
 authors = ["CloudBlue LLC"]
 license = "Apache-2.0"
 
 packages = [
     { include = "connect" },
 ]
@@ -54,48 +54,50 @@
 
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
 click = "^8.1.3"
 openpyxl = "^3.0.7"
 connect-openapi-client = ">=25.15"
-interrogatio = "^2.2.2"
+interrogatio = "^2.3.1"
 connect-markdown-renderer = ">=2.0.1,<3"
 iso3166 = "^1.0.1"
 phonenumbers = "^8.12.19"
 connect-reports-core = "26.*"
 requests = "^2.25.1"
 toml = "^0.10.2"
 Jinja2 = "^3.1.2"
 jinja2-time = "^0.2.0"
-connect-eaas-core = ">=26.12,<27"
+connect-eaas-core = ">=27.13,<28"
 rich = "^12.4.1"
 poetry-core = "^1.3.0"  
 uvloop = { version = "^0.16.0", markers = "sys_platform == \"linux\" or sys_platform == \"darwin\"" }
 fs = "^2.4.12"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.test.dependencies]
 pytest = "^6.1.2"
 pytest-cov = "^2.10.1"
 pytest-mock = "^3.3.1"
 freezegun = "^1.2.1"
 coverage = {extras = ["toml"], version = "^5.3"}
 responses = "^0.20.0"
 flake8 = "^5.0"
 flake8-bugbear = "^22"
 flake8-cognitive-complexity = "^0.1"
 flake8-commas = "^2.1"
 flake8-future-import = "~0.4"
-flake8-import-order = "~0.18"
+flake8-isort = "5.*"
 flake8-broken-line = "~0.5"
 flake8-comprehensions = "^3.10"
 flake8-debugger = "^4.0.0"
 flake8-eradicate = "^1.3.0"
 flake8-string-format = "^0.3.0"
+flake8-pyproject = "^1.2.2"
 ipython = "^7.21.0"
+isort = "5.*"
 wheel = "^0.37.0"
 Faker = "^13.11.0"
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "setuptools>42"]
 build-backend = "poetry.core.masonry.api"
@@ -127,7 +129,38 @@
 exclude_lines = [
     "pragma: no cover",
     "def __str__",
     "def __repr__",
     "raise NotImplementedError",
     "if __name__ == .__main__.:",
 ]
+
+
+[tool.flake8]
+exclude = [
+    ".idea",
+    ".vscode",
+    ".git",
+    "resources",
+    "*.eggs",
+    "tests/fixtures",
+    "connect/.data",
+    "venv"
+]
+
+show_source = true
+max_line_length = 120
+max_cognitive_complexity = 15
+ignore = ["FI1", "W503"]
+
+
+[tool.isort]
+src_paths = "*"
+sections = ["FUTURE", "STDLIB", "THIRDPARTY", "FIRSTPARTY", "LOCALFOLDER"]
+group_by_package = true
+multi_line_output = 3
+force_grid_wrap = 4
+combine_as_imports = true
+use_parentheses = true
+include_trailing_comma = true
+line_length = 100
+lines_after_imports = 2
```

### Comparing `connect_cli-26.9/PKG-INFO` & `connect_cli-27.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connect-cli
-Version: 26.9
+Version: 27.0
 Summary: CloudBlue Connect Command Line Interface
 Home-page: https://connect.cloudblue.com
 License: Apache-2.0
 Keywords: fulfillment,command,line,interface,utility,cli,vendor,connect,cloudblue
 Author: CloudBlue LLC
 Requires-Python: >=3.8,<4
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,36 +18,36 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: connect-eaas-core (>=26.12,<27)
+Requires-Dist: connect-eaas-core (>=27.13,<28)
 Requires-Dist: connect-markdown-renderer (>=2.0.1,<3)
 Requires-Dist: connect-openapi-client (>=25.15)
 Requires-Dist: connect-reports-core (>=26.0.0,<27.0.0)
 Requires-Dist: fs (>=2.4.12,<3.0.0)
-Requires-Dist: interrogatio (>=2.2.2,<3.0.0)
+Requires-Dist: interrogatio (>=2.3.1,<3.0.0)
 Requires-Dist: iso3166 (>=1.0.1,<2.0.0)
 Requires-Dist: jinja2-time (>=0.2.0,<0.3.0)
 Requires-Dist: openpyxl (>=3.0.7,<4.0.0)
 Requires-Dist: phonenumbers (>=8.12.19,<9.0.0)
 Requires-Dist: poetry-core (>=1.3.0,<2.0.0)
 Requires-Dist: requests (>=2.25.1,<3.0.0)
 Requires-Dist: rich (>=12.4.1,<13.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
-Requires-Dist: uvloop (>=0.16.0,<0.17.0); sys_platform == "linux" or sys_platform == "darwin"
+Requires-Dist: uvloop (>=0.16.0,<0.17.0) ; sys_platform == "linux" or sys_platform == "darwin"
 Project-URL: Documentation, https://connect.cloudblue.com/community/sdk/cli/
 Project-URL: Repository, https://github.com/cloudblue/connect-cli
 Description-Content-Type: text/markdown
 
 # CloudBlue Connect Command Line Interface
 
-![pyversions](https://img.shields.io/pypi/pyversions/connect-cli.svg) [![PyPi Status](https://img.shields.io/pypi/v/connect-cli.svg)](https://pypi.org/project/connect-cli/) ![PyPI - Downloads](https://img.shields.io/pypi/dm/connect-cli) ![Docker Pulls](https://img.shields.io/docker/pulls/cloudblueconnect/connect-cli) ![GitHub Workflow Status](https://img.shields.io/github/workflow/status/cloudblue/connect-cli/Build%20Connect%20Command%20Line%20Client) [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=connect-cli&metric=coverage)](https://sonarcloud.io/summary/new_code?id=connect-cli) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=connect-cli&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=connect-cli)
+![pyversions](https://img.shields.io/pypi/pyversions/connect-cli.svg) [![PyPi Status](https://img.shields.io/pypi/v/connect-cli.svg)](https://pypi.org/project/connect-cli/) ![PyPI - Downloads](https://img.shields.io/pypi/dm/connect-cli) ![Docker Pulls](https://img.shields.io/docker/pulls/cloudblueconnect/connect-cli) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/cloudblue/connect-cli/build.yml?branch=master) [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=connect-cli&metric=coverage)](https://sonarcloud.io/summary/new_code?id=connect-cli) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=connect-cli&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=connect-cli)
 
 ## Introduction
 
 The CloudBlue Connect Command Line Interface (CLI) is an extensible unified tool to perform various automation scenarios. With just one tool, you can control multiple Connect modules from the command line and automate them through scripts.
 
 Since it is extensible, users can write their own plugins to extend its functionalities.
 
@@ -109,14 +109,19 @@
 * [Products](docs/products_usage.md)
 * [Customers](docs/customers_usage.md)
 * [Reports](docs/reports_usage.md)
 * [Translations](docs/translations_usage.md)
 * [Projects](docs/project_usage.md)
 
 
+## Development
+We use `isort` library to order and format our imports, and we check it using `flake8-isort` library (automatically on `flake8` run).  
+For convenience you may run `poetry run isort .` to order imports.
+
+
 ## Run tests
 
 `connect-cli` uses [poetry](https://python-poetry.org/) for dependencies management and packaging.
 
 To run the `connect-cli` tests suite run:
 
 ```
```

