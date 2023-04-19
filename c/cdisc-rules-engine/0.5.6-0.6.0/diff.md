# Comparing `tmp/cdisc-rules-engine-0.5.6.tar.gz` & `tmp/cdisc-rules-engine-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdisc-rules-engine-0.5.6.tar", last modified: Tue Feb 14 17:11:33 2023, max compression
+gzip compressed data, was "cdisc-rules-engine-0.6.0.tar", last modified: Wed Apr 19 15:20:33 2023, max compression
```

## Comparing `cdisc-rules-engine-0.5.6.tar` & `cdisc-rules-engine-0.6.0.tar`

### file list

```diff
@@ -1,188 +1,215 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:11:33.758983 cdisc-rules-engine-0.5.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-02-14 17:11:33.758983 cdisc-rules-engine-0.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:11:33.742982 cdisc-rules-engine-0.5.6/cdisc_rules_engine/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:11:33.746982 cdisc-rules-engine-0.5.6/cdisc_rules_engine/config/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:11:33.746982 cdisc-rules-engine-0.5.6/cdisc_rules_engine/constants/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/constants/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/constants/define_xml_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/constants/domains.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/constants/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/constants/rule_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:11:33.746982 cdisc-rules-engine-0.5.6/cdisc_rules_engine/dummy_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/dummy_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/dummy_models/dummy_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/dummy_models/dummy_variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:11:33.746982 cdisc-rules-engine-0.5.6/cdisc_rules_engine/enums/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/enums/base_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/enums/default_file_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/enums/execution_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/enums/library_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/enums/optional_condition_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/enums/progress_parameter_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/enums/report_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/enums/rule_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/enums/sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/enums/variable_roles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:11:33.746982 cdisc-rules-engine-0.5.6/cdisc_rules_engine/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/exceptions/custom_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:11:33.746982 cdisc-rules-engine-0.5.6/cdisc_rules_engine/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/interfaces/cache_service_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/interfaces/condition_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/interfaces/config_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/interfaces/data_reader_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/interfaces/data_service_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/interfaces/dictionary_term_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/interfaces/factory_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/interfaces/logger_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/interfaces/representation_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/interfaces/terms_factory_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:11:33.750982 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/base_validation_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/dataset_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/dataset_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/dataset_variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:11:33.750982 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/define/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/define/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/define/value_level_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:11:33.750982 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/dictionaries/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/dictionaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/dictionaries/abstract_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/dictionaries/dictionary_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/dictionaries/get_dictionary_terms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:11:33.750982 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/dictionaries/meddra/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/dictionaries/meddra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/dictionaries/meddra/meddra_file_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/dictionaries/meddra/meddra_terms_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/dictionaries/meddra/meddra_variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:11:33.750982 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/dictionaries/meddra/terms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/dictionaries/meddra/terms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/dictionaries/meddra/terms/meddra_term.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/dictionaries/meddra/terms/term_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:11:33.750982 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/dictionaries/whodrug/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/dictionaries/whodrug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/dictionaries/whodrug/atc_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/dictionaries/whodrug/atc_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/dictionaries/whodrug/base_whodrug_term.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/dictionaries/whodrug/drug_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/dictionaries/whodrug/whodrug_file_names.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/dictionaries/whodrug/whodrug_record_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/dictionaries/whodrug/whodrug_terms_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/dictionaries/whodrug/whodrug_variable_names.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/failed_validation_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/operation_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/record_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:11:33.750982 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/rule_conditions/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/rule_conditions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/rule_conditions/allowed_conditions_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/rule_conditions/condition_composite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/rule_conditions/condition_composite_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/rule_conditions/not_condition_composite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/rule_conditions/single_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/rule_validation_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/test_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/validation_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/validation_error_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/validation_error_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/variable_metadata_container.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:11:33.754982 cdisc-rules-engine-0.5.6/cdisc_rules_engine/operations/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/operations/base_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/operations/dataset_column_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/operations/day_data_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/operations/distinct.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/operations/extract_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/operations/library_column_order.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/operations/max_date.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/operations/maximum.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/operations/mean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/operations/meddra_code_references_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/operations/meddra_code_term_pairs_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/operations/meddra_term_references_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/operations/min_date.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/operations/minimum.py
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/operations/operations_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/operations/record_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/operations/variable_count.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/operations/variable_exists.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/operations/variable_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/operations/variable_permissibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/operations/variable_value_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/operations/whodrug_hierarchy_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/operations/whodrug_references_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/plugin_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    25912 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/rules_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:11:33.754982 cdisc-rules-engine-0.5.6/cdisc_rules_engine/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/serializers/base_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/serializers/dataset_metadata_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/serializers/rule_serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:11:33.754982 cdisc-rules-engine-0.5.6/cdisc_rules_engine/serializers/term_serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/serializers/term_serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/serializers/term_serializers/atc_classification_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/serializers/term_serializers/atc_text_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/serializers/term_serializers/base_whodrug_term_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/serializers/term_serializers/drug_dictionary_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/serializers/term_serializers/meddra_term_serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:11:33.754982 cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/adam_variable_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:11:33.758983 cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/cache/cache_populator_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/cache/cache_service_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/cache/in_memory_cache_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/cache/redis_cache_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    20318 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/cdisc_library_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:11:33.758983 cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/data_readers/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/data_readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/data_readers/data_reader_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/data_readers/xpt_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:11:33.758983 cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/data_services/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/data_services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/data_services/base_data_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/data_services/data_service_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/data_services/dummy_data_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     7647 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/data_services/local_data_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/dataset_metadata_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11701 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/define_xml_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:11:33.758983 cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/logging/console_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/logging/logging_service_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:11:33.758983 cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/reporting/base_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/reporting/excel_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/reporting/excel_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/reporting/json_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/reporting/report_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:11:33.758983 cdisc-rules-engine-0.5.6/cdisc_rules_engine/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14773 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/utilities/data_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/utilities/dataset_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/utilities/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/utilities/progress_displayers.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/utilities/reporting_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    19220 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/utilities/rule_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/utilities/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-02-14 17:11:00.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine/utilities/validation_output_container.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:11:33.746982 cdisc-rules-engine-0.5.6/cdisc_rules_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-02-14 17:11:33.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-02-14 17:11:33.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 17:11:33.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-02-14 17:11:33.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-14 17:11:33.000000 cdisc-rules-engine-0.5.6/cdisc_rules_engine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-14 17:11:33.758983 cdisc-rules-engine-0.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-02-14 17:11:01.000000 cdisc-rules-engine-0.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:20:33.089201 cdisc-rules-engine-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-19 15:20:33.089201 cdisc-rules-engine-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:20:33.069201 cdisc-rules-engine-0.6.0/TestRule/
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/TestRule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:20:33.069201 cdisc-rules-engine-0.6.0/cdisc_rule_tester/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rule_tester/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:20:33.069201 cdisc-rules-engine-0.6.0/cdisc_rule_tester/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rule_tester/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rule_tester/models/rule_tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:20:33.069201 cdisc-rules-engine-0.6.0/cdisc_rules_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:20:33.069201 cdisc-rules-engine-0.6.0/cdisc_rules_engine/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:20:33.073201 cdisc-rules-engine-0.6.0/cdisc_rules_engine/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/constants/cache_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/constants/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/constants/define_xml_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/constants/domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/constants/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/constants/permissibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/constants/rule_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:20:33.073201 cdisc-rules-engine-0.6.0/cdisc_rules_engine/dataset_builders/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/dataset_builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/dataset_builders/base_dataset_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/dataset_builders/content_metadata_dataset_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/dataset_builders/contents_dataset_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/dataset_builders/dataset_builder_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/dataset_builders/define_variables_dataset_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/dataset_builders/domain_list_dataset_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/dataset_builders/variables_metadata_dataset_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/dataset_builders/variables_metadata_with_define_dataset_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:20:33.073201 cdisc-rules-engine-0.6.0/cdisc_rules_engine/dummy_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/dummy_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/dummy_models/dummy_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/dummy_models/dummy_variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:20:33.073201 cdisc-rules-engine-0.6.0/cdisc_rules_engine/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/enums/base_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/enums/default_file_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/enums/execution_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/enums/library_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/enums/optional_condition_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/enums/progress_parameter_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/enums/report_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/enums/rule_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/enums/sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/enums/variable_roles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:20:33.073201 cdisc-rules-engine-0.6.0/cdisc_rules_engine/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/exceptions/custom_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:20:33.073201 cdisc-rules-engine-0.6.0/cdisc_rules_engine/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/interfaces/cache_service_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/interfaces/condition_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/interfaces/config_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/interfaces/data_reader_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/interfaces/data_service_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/interfaces/dictionary_term_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/interfaces/factory_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/interfaces/logger_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/interfaces/representation_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/interfaces/terms_factory_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:20:33.077201 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/base_validation_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/dataset_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/dataset_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/dataset_variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:20:33.077201 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/define/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/define/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/define/value_level_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:20:33.077201 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/dictionaries/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/dictionaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/dictionaries/abstract_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/dictionaries/dictionary_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/dictionaries/get_dictionary_terms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:20:33.077201 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/dictionaries/meddra/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/dictionaries/meddra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/dictionaries/meddra/meddra_file_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/dictionaries/meddra/meddra_terms_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/dictionaries/meddra/meddra_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:20:33.077201 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/dictionaries/meddra/terms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/dictionaries/meddra/terms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/dictionaries/meddra/terms/meddra_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/dictionaries/meddra/terms/term_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:20:33.081201 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/dictionaries/whodrug/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/dictionaries/whodrug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/dictionaries/whodrug/atc_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/dictionaries/whodrug/atc_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/dictionaries/whodrug/base_whodrug_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/dictionaries/whodrug/drug_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/dictionaries/whodrug/whodrug_file_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/dictionaries/whodrug/whodrug_record_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/dictionaries/whodrug/whodrug_terms_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/dictionaries/whodrug/whodrug_variable_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/failed_validation_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/operation_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/record_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:20:33.081201 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/rule_conditions/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/rule_conditions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/rule_conditions/allowed_conditions_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/rule_conditions/condition_composite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/rule_conditions/condition_composite_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/rule_conditions/not_condition_composite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/rule_conditions/single_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/rule_validation_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/validation_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/validation_error_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/validation_error_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/variable_metadata_container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:20:33.085201 cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/base_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/dataset_column_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/day_data_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/distinct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/domain_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/expected_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/extract_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/library_column_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/library_model_column_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/max_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/maximum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/meddra_code_references_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/meddra_code_term_pairs_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/meddra_term_references_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/min_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/minimum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/operations_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/parent_library_model_column_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/permissible_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/record_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/required_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/study_domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/valid_codelist_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/variable_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/variable_exists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/variable_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/variable_permissibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/variable_value_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/whodrug_hierarchy_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/whodrug_references_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/plugin_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16834 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/rules_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:20:33.085201 cdisc-rules-engine-0.6.0/cdisc_rules_engine/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/serializers/base_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/serializers/dataset_metadata_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/serializers/rule_serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:20:33.085201 cdisc-rules-engine-0.6.0/cdisc_rules_engine/serializers/term_serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/serializers/term_serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/serializers/term_serializers/atc_classification_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/serializers/term_serializers/atc_text_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/serializers/term_serializers/base_whodrug_term_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/serializers/term_serializers/drug_dictionary_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/serializers/term_serializers/meddra_term_serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:20:33.085201 cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/adam_variable_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:20:33.085201 cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13088 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/cache/cache_populator_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/cache/cache_service_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/cache/in_memory_cache_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/cache/redis_cache_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20318 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/cdisc_library_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:20:33.085201 cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/data_readers/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/data_readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/data_readers/data_reader_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/data_readers/xpt_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:20:33.085201 cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/data_services/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/data_services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/data_services/base_data_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/data_services/data_service_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/data_services/dummy_data_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/data_services/local_data_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/dataset_metadata_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11701 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/define_xml_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:20:33.089201 cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/logging/console_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/logging/logging_service_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:20:33.089201 cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/reporting/base_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/reporting/excel_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/reporting/excel_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/reporting/json_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/reporting/report_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:20:33.089201 cdisc-rules-engine-0.6.0/cdisc_rules_engine/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14773 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/utilities/data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/utilities/dataset_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/utilities/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/utilities/progress_displayers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/utilities/reporting_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19536 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/utilities/rule_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/utilities/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-19 15:20:03.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine/utilities/validation_output_container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:20:33.069201 cdisc-rules-engine-0.6.0/cdisc_rules_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-19 15:20:33.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9579 2023-04-19 15:20:33.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 15:20:33.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-19 15:20:33.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-19 15:20:33.000000 cdisc-rules-engine-0.6.0/cdisc_rules_engine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 15:20:33.089201 cdisc-rules-engine-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-19 15:20:04.000000 cdisc-rules-engine-0.6.0/setup.py
```

### Comparing `cdisc-rules-engine-0.5.6/LICENSE` & `cdisc-rules-engine-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/README.md` & `cdisc-rules-engine-0.6.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 Clone the repository and run `core.py --help` to see the full list of commands.
 
 Run `core.py validate --help` to see the list of validation options.
 ```
   -ca, --cache TEXT               Relative path to cache files containing pre
                                   loaded metadata and rules
-  -p, --pool-size INTEGER         Number of parallel processes for validation
+  -ps, --pool-size INTEGER         Number of parallel processes for validation
   -d, --data TEXT                 Path to directory containing data files
   -dp, --dataset-path TEXT        Absolute path to dataset file
   -l, --log-level [info|debug|error|critical|disabled|warn]
                                   Sets log level for engine logs, logs are
                                   disabled by default
   -rt, --report-template TEXT     File path of report template to use for
                                   excel output
```

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/config/config.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/config/config.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/constants/__init__.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/dummy_models/dummy_dataset.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/dummy_models/dummy_dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
             for variable_data in dataset_data.get("variables", [])
         ]
         self.data = pd.DataFrame.from_dict(dataset_data.get("records", {}))
 
     def get_metadata(self):
         return {
             "dataset_size": [self.filesize or 1000],
-            "dataset_name": [self.domain or "test"],
+            "dataset_name": [self.filename.split(".")[0].upper() or "test"],
             "dataset_label": [self.label or "test"],
             "filename": [self.filename],
         }
 
     def validate(self, dataset_data):
         required_values = ["domain"]
         for value in required_values:
```

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/enums/default_file_paths.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/enums/default_file_paths.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/enums/rule_types.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/enums/rule_types.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/exceptions/custom_exceptions.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/exceptions/custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/interfaces/__init__.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/interfaces/cache_service_interface.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/interfaces/cache_service_interface.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/interfaces/condition_interface.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/interfaces/condition_interface.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/interfaces/data_service_interface.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/interfaces/data_service_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     ) -> pd.DataFrame:
         """
         Generic function to return dataset based on the type.
         dataset_type param can be: contents, metadata, variables_metadata.
         """
 
     @abstractmethod
-    def join_split_datasets(self, func_to_call: Callable, dataset_names, **kwargs):
+    def concat_split_datasets(self, func_to_call: Callable, dataset_names, **kwargs):
         """
         Accepts a list of split dataset filenames,
         downloads all of them and merges into a single DataFrame.
         """
 
     @abstractmethod
     def get_define_xml_contents(self, dataset_name: str) -> bytes:
```

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/interfaces/logger_interface.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/interfaces/logger_interface.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/interfaces/terms_factory_interface.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/interfaces/terms_factory_interface.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/actions.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/actions.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/dataset_variable.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/dataset_variable.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/define/value_level_metadata.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/define/value_level_metadata.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/dictionaries/abstract_factory.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/dictionaries/abstract_factory.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/dictionaries/get_dictionary_terms.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/dictionaries/get_dictionary_terms.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/dictionaries/meddra/meddra_terms_factory.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/dictionaries/meddra/meddra_terms_factory.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/dictionaries/meddra/terms/meddra_term.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/dictionaries/meddra/terms/meddra_term.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/dictionaries/whodrug/atc_classification.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/dictionaries/whodrug/atc_classification.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/dictionaries/whodrug/atc_text.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/dictionaries/whodrug/atc_text.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/dictionaries/whodrug/base_whodrug_term.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/dictionaries/whodrug/base_whodrug_term.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/dictionaries/whodrug/drug_dict.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/dictionaries/whodrug/drug_dict.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/dictionaries/whodrug/whodrug_terms_factory.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/dictionaries/whodrug/whodrug_terms_factory.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/failed_validation_entity.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/failed_validation_entity.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/operation_params.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/operation_params.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/record_variable.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/record_variable.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/rule.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         if cls.is_cdisc_rule_metadata(rule_metadata):
             authorities = rule_metadata.get("Authorities", [])
             executable_rule = {
                 "core_id": rule_metadata.get("Core", {}).get("Id"),
                 "author": "CDISC",
                 "reference": cls.parse_references(authorities),
                 "sensitivity": rule_metadata.get("Sensitivity"),
-                "executability": rule_metadata.get("Executability", "").lower(),
+                "executability": (rule_metadata.get("Executability") or "").lower(),
                 "description": rule_metadata.get("Description"),
                 "authorities": authorities,
                 "standards": cls.parse_standards(authorities),
                 "classes": rule_metadata.get("Scope", {}).get("Classes"),
                 "domains": rule_metadata.get("Scope", {}).get("Domains"),
                 "rule_type": rule_metadata.get("Rule_Type"),
                 "conditions": cls.parse_conditions(rule_metadata.get("Check")),
```

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/rule_conditions/condition_composite.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/rule_conditions/condition_composite.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/rule_conditions/condition_composite_factory.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/rule_conditions/condition_composite_factory.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/rule_conditions/not_condition_composite.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/rule_conditions/not_condition_composite.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/rule_conditions/single_condition.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/rule_conditions/single_condition.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/validation_error_container.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/validation_error_container.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/validation_error_entity.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/validation_error_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,11 +21,11 @@
     def to_representation(self) -> dict:
         representation: dict = {
             "value": self.value,
         }
         if self._row is not None:
             representation["row"] = self._row
         if self._usubjid:
-            representation["uSubjId"] = self._usubjid
+            representation["USUBJID"] = self._usubjid
         if self._sequence:
-            representation["seq"] = self._sequence
+            representation["SEQ"] = self._sequence
         return representation
```

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/models/variable_metadata_container.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/models/variable_metadata_container.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from cdisc_rules_engine.interfaces import RepresentationInterface
 
 
 class VariableMetadataContainer(RepresentationInterface):
     def __init__(self, contents_metadata: dict):
         variable_names = contents_metadata["variable_names"]
+        self.formats = contents_metadata["variable_formats"]
         self.names = variable_names
         self.order = [(variable_names.index(name) + 1) for name in variable_names]
         self.labels = contents_metadata["variable_name_to_label_map"].values()
         self.sizes = contents_metadata["variable_name_to_size_map"].values()
         self.data_types = contents_metadata["variable_name_to_data_type_map"].values()
 
     def to_representation(self) -> dict:
         return {
             "variable_name": self.names,
             "variable_order": self.order,
             "variable_label": self.labels,
             "variable_size": self.sizes,
             "variable_data_type": self.data_types,
+            "variable_format": self.formats,
         }
```

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/operations/base_operation.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/variable_value_count.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,60 +1,51 @@
 import pandas as pd
-from cdisc_rules_engine.models.operation_params import OperationParams
-from abc import abstractmethod
-
-from cdisc_rules_engine.interfaces import (
-    CacheServiceInterface,
-    DataServiceInterface,
+from cdisc_rules_engine.operations.base_operation import BaseOperation
+import asyncio
+from collections import Counter
+from typing import List
+from cdisc_rules_engine.utilities.utils import (
+    get_corresponding_datasets,
+    is_split_dataset,
 )
 
 
-class BaseOperation:
-    def __init__(
-        self,
-        params: OperationParams,
-        original_dataset: pd.DataFrame,
-        cache_service: CacheServiceInterface,
-        data_service: DataServiceInterface,
-    ):
-        self.params = params
-        self.cache = cache_service
-        self.data_service = data_service
-        self.evaluation_dataset = original_dataset
-
-    @abstractmethod
+class VariableValueCount(BaseOperation):
     def _execute_operation(self):
-        """Perform operation calculations."""
-        pass
-
-    def execute(self) -> pd.DataFrame:
-        result = self._execute_operation()
-        return self._handle_operation_result(result)
-
-    def _handle_operation_result(self, result) -> pd.DataFrame:
-        if self.params.grouping:
-            return self._handle_grouped_result(result)
-        elif isinstance(result, dict):
-            return self._handle_dictionary_result(result)
-        elif isinstance(result, pd.Series):
-            self.evaluation_dataset[self.params.operation_id] = result
-            return self.evaluation_dataset
+        # get metadata
+        variable_value_count = asyncio.run(self._get_all_study_variable_value_counts())
+        return variable_value_count
+
+    async def _get_all_study_variable_value_counts(self) -> dict:
+        """
+        Returns a mapping of variable values to the number
+        of times that value appears in the study.
+        """
+        datasets_with_unique_domains = list(
+            {dataset["domain"]: dataset for dataset in self.params.datasets}.values()
+        )
+        coroutines = [
+            self._get_dataset_variable_value_count(dataset)
+            for dataset in datasets_with_unique_domains
+        ]
+        dataset_variable_value_counts: List[Counter] = await asyncio.gather(*coroutines)
+        return dict(sum(dataset_variable_value_counts, Counter()))
+
+    async def _get_dataset_variable_value_count(self, dataset: dict) -> Counter:
+        domain = dataset.get("domain")
+        if is_split_dataset(self.params.datasets, domain):
+            files = [
+                f"{self.params.directory_path}/{dataset.get('filename')}"
+                for dataset in get_corresponding_datasets(self.params.datasets, domain)
+            ]
+            data: pd.DataFrame = self.data_service.join_split_datasets(
+                self.data_service.get_dataset, files
+            )
         else:
-            # Handle single results
-            self.evaluation_dataset[self.params.operation_id] = pd.Series(
-                [result] * len(self.evaluation_dataset)
+            data: pd.DataFrame = self.data_service.get_dataset(
+                f"{self.params.directory_path}/{dataset.get('filename')}"
             )
-            return self.evaluation_dataset
-
-    def _handle_grouped_result(self, result):
-        # Handle grouped results
-        result = result.rename(columns={self.params.target: self.params.operation_id})
-        target_columns = self.params.grouping + [self.params.operation_id]
-        return self.evaluation_dataset.merge(
-            result[target_columns], on=self.params.grouping, how="left"
-        )
-
-    def _handle_dictionary_result(self, result):
-        self.evaluation_dataset[self.params.operation_id] = [result] * len(
-            self.evaluation_dataset
-        )
-        return self.evaluation_dataset
+        target_variable = self.params.target.replace("--", domain, 1)
+        if target_variable in data:
+            return Counter(data[target_variable].unique())
+        else:
+            return Counter()
```

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/operations/day_data_validator.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/day_data_validator.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/operations/distinct.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/distinct.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/operations/library_column_order.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/library_model_column_order.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,52 @@
 from typing import List, Optional, Tuple
 
 from cdisc_rules_engine.constants.classes import (
     DETECTABLE_CLASSES,
-    GENERAL_OBSERVATIONS_CLASS,
 )
-from cdisc_rules_engine.enums.variable_roles import VariableRoles
 from cdisc_rules_engine.operations.base_operation import BaseOperation
 from cdisc_rules_engine.utilities.utils import (
     get_model_details_cache_key,
     get_standard_details_cache_key,
     search_in_list_of_dicts,
+    convert_library_class_name_to_ct_class,
 )
+from collections import OrderedDict
 
 
-class LibraryColumnOrder(BaseOperation):
+class LibraryModelColumnOrder(BaseOperation):
     def _execute_operation(self):
         """
         Fetches column order for a given domain from the CDISC library.
         Returns it as a Series of lists like:
         0    ["STUDYID", "DOMAIN", ...]
         1    ["STUDYID", "DOMAIN", ...]
         2    ["STUDYID", "DOMAIN", ...]
         ...
 
         Length of Series is equal to the length of given dataframe.
         The lists with column names are sorted
         in accordance to "ordinal" key of library metadata.
         """
+        return self._get_variable_names_list(self.params.domain, self.params.dataframe)
 
+    def _get_variable_names_list(self, domain, dataframe):
         # get variables metadata from the standard model
         variables_metadata: List[
             dict
-        ] = self._get_variables_metadata_from_standard_model()
-
+        ] = self._get_variables_metadata_from_standard_model(domain, dataframe)
         # create a list of variable names in accordance to the "ordinal" key
-        variable_names_list = [
-            var["name"].replace("--", self.params.domain) for var in variables_metadata
-        ]
-        return variable_names_list
+        variable_names_list = self._replace_variable_wildcards(
+            variables_metadata, domain
+        )
+        return list(OrderedDict.fromkeys(variable_names_list))
 
-    def _get_variables_metadata_from_standard_model(self) -> List[dict]:
+    def _get_variables_metadata_from_standard_model(
+        self, domain, dataframe
+    ) -> List[dict]:
         """
         Gets variables metadata for the given class and domain from cache.
         The cache stores CDISC Library metadata.
 
         Return example:
         [
             {
@@ -65,101 +68,54 @@
         # get model details from cache
         cache_key: str = get_standard_details_cache_key(
             self.params.standard, self.params.standard_version
         )
 
         standard_details: dict = self.cache.get(cache_key) or {}
         model = standard_details.get("_links", {}).get("model")
-        class_details, domain_details = self._get_class_and_domain_metadata(
-            standard_details
-        )
         model_type, model_version = self._get_model_type_and_version(model)
         model_cache_key = get_model_details_cache_key(model_type, model_version)
         model_details = self.cache.get(model_cache_key) or {}
+        domain_details = self._get_model_domain_metadata(model_details, domain)
+        variables_metadata = []
 
-        # model class details includes all variables allowed in the domain
-        model_class_details: dict = self._get_class_metadata(
-            model_details, class_details.get("name")
-        )
-        variables_metadata: List[dict] = model_class_details.get("classVariables", [])
-        variables_metadata.sort(key=lambda item: item["ordinal"])
-
-        if class_details.get("name") in DETECTABLE_CLASSES:
-            # if the class is one of Interventions, Findings, or Events
-            # and the standard is SDTMIG
-            # -> add General Observation class variables to variables metadata
-            gen_obs_class_metadata: dict = self._get_class_metadata(
-                model_details, GENERAL_OBSERVATIONS_CLASS
+        if domain_details:
+            # Domain found in the model
+            class_name = convert_library_class_name_to_ct_class(
+                domain_details["_links"]["parentClass"]["title"]
             )
-            identifiers_metadata, timing_metadata = self._sort_class_variables_by_role(
-                gen_obs_class_metadata["classVariables"]
+            class_details = self._get_class_metadata(model_details, class_name)
+            variables_metadata = domain_details.get("datasetVariables", [])
+            variables_metadata.sort(key=lambda item: item["ordinal"])
+        else:
+            # Domain not found in the model. Detect class name from data
+            class_name = self.data_service.get_dataset_class(
+                dataframe, self.params.dataset_path, self.params.datasets
             )
+            class_name = convert_library_class_name_to_ct_class(class_name)
+            class_details = self._get_class_metadata(model_details, class_name)
+
+        if class_name in DETECTABLE_CLASSES:
+            (
+                identifiers_metadata,
+                variables_metadata,
+                timing_metadata,
+            ) = self.get_allowed_class_variables(model_details, class_details)
             # Identifiers are added to the beginning and Timing to the end
             if identifiers_metadata:
-                identifiers_metadata.sort(key=lambda item: item["ordinal"])
                 variables_metadata = identifiers_metadata + variables_metadata
             if timing_metadata:
-                timing_metadata.sort(key=lambda item: item["ordinal"])
                 variables_metadata = variables_metadata + timing_metadata
 
         return variables_metadata
 
-    def _get_model_type_and_version(self, model_link) -> Tuple:
-        link = model_link.get("href")
-        if "sdtm" in link:
-            model_type = "sdtm"
-            model_version = link.split("/")[-1]
-        else:
-            # TODO expand to support CDASH and ADAM
-            model_type = ""
-            model_version = ""
-        return model_type, model_version
-
-    def _get_class_metadata(
-        self,
-        model_details: dict,
-        dataset_class: str,
-    ) -> dict:
-        """
-        Extracts metadata of a certain class
-        from given standard model details.
-        """
-        class_metadata: Optional[dict] = search_in_list_of_dicts(
-            model_details.get("classes", []),
-            lambda item: item["name"] == dataset_class,
+    def _get_model_domain_metadata(self, model_details, domain_name) -> Tuple:
+        # Get domain metadata from model
+        domain_details: Optional[dict] = search_in_list_of_dicts(
+            model_details.get("datasets", []), lambda item: item["name"] == domain_name
         )
-        if not class_metadata:
-            raise ValueError(
-                f"Variables metadata is not found in CDISC Library. "
-                f"standard={self.params.standard}, "
-                f"version={self.params.standard_version}, "
-                f"class={dataset_class}"
-            )
-        return class_metadata
 
-    def _get_class_and_domain_metadata(self, standard_details) -> Tuple:
-        # Get domain and class details for domain. This logic is specific
-        # to SDTM based standards. Needs to be expanded for other models
-        for c in standard_details.get("classes"):
-            domain_details = search_in_list_of_dicts(
-                c.get("datasets", []), lambda item: item["name"] == self.params.domain
-            )
-            if domain_details:
-                return c, domain_details
-        return {}, {}
-
-    def _sort_class_variables_by_role(
-        self, class_variables: List[dict]
-    ) -> Tuple[List[dict], List[dict]]:
-        """
-        Sorts given class variables by role into 2 lists:
-        Identifiers and Timing
-        """
-        identifier_vars: List[dict] = []
-        timing_vars: List[dict] = []
-        for variable in class_variables:
-            role: str = variable.get("role")
-            if role == VariableRoles.IDENTIFIER.value:
-                identifier_vars.append(variable)
-            elif role == VariableRoles.TIMING.value:
-                timing_vars.append(variable)
-        return identifier_vars, timing_vars
+        return domain_details
+
+    @staticmethod
+    def _replace_variable_wildcards(variables_metadata, domain):
+        return [var["name"].replace("--", domain) for var in variables_metadata]
```

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/operations/max_date.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/max_date.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/operations/meddra_code_references_validator.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/meddra_code_references_validator.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/operations/meddra_code_term_pairs_validator.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/meddra_code_term_pairs_validator.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/operations/meddra_term_references_validator.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/meddra_term_references_validator.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/operations/min_date.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/min_date.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/operations/operations_factory.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/operations_factory.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,17 +3,24 @@
 from cdisc_rules_engine.interfaces import FactoryInterface
 from cdisc_rules_engine.operations.base_operation import BaseOperation
 from cdisc_rules_engine.operations.dataset_column_order import DatasetColumnOrder
 from cdisc_rules_engine.operations.day_data_validator import DayDataValidator
 from cdisc_rules_engine.operations.distinct import Distinct
 from cdisc_rules_engine.operations.extract_metadata import ExtractMetadata
 from cdisc_rules_engine.operations.library_column_order import LibraryColumnOrder
+from cdisc_rules_engine.operations.library_model_column_order import (
+    LibraryModelColumnOrder,
+)
+from cdisc_rules_engine.operations.parent_library_model_column_order import (
+    ParentLibraryModelColumnOrder,
+)
 from cdisc_rules_engine.operations.max_date import MaxDate
 from cdisc_rules_engine.operations.maximum import Maximum
 from cdisc_rules_engine.operations.mean import Mean
+from cdisc_rules_engine.operations.domain_label import DomainLabel
 from cdisc_rules_engine.operations.meddra_code_references_validator import (
     MedDRACodeReferencesValidator,
 )
 from cdisc_rules_engine.operations.meddra_code_term_pairs_validator import (
     MedDRACodeTermPairsValidator,
 )
 from cdisc_rules_engine.operations.meddra_term_references_validator import (
@@ -29,23 +36,30 @@
     WhodrugReferencesValidator,
 )
 from cdisc_rules_engine.operations.whodrug_hierarchy_validator import (
     WhodrugHierarchyValidator,
 )
 from cdisc_rules_engine.operations.variable_permissibility import VariablePermissibility
 from cdisc_rules_engine.operations.variable_count import VariableCount
+from cdisc_rules_engine.operations.required_variables import RequiredVariables
+from cdisc_rules_engine.operations.expected_variables import ExpectedVariables
+from cdisc_rules_engine.operations.permissible_variables import PermissibleVariables
+from cdisc_rules_engine.operations.study_domains import StudyDomains
+from cdisc_rules_engine.operations.valid_codelist_dates import ValidCodelistDates
 
 
 class OperationsFactory(FactoryInterface):
     _operations_map = {
         "distinct": Distinct,
         "dy": DayDataValidator,
         "extract_metadata": ExtractMetadata,
         "get_column_order_from_dataset": DatasetColumnOrder,
         "get_column_order_from_library": LibraryColumnOrder,
+        "get_model_column_order": LibraryModelColumnOrder,
+        "get_parent_model_column_order": ParentLibraryModelColumnOrder,
         "max": Maximum,
         "max_date": MaxDate,
         "mean": Mean,
         "min": Minimum,
         "min_date": MinDate,
         "record_count": RecordCount,
         "valid_meddra_code_references": MedDRACodeReferencesValidator,
@@ -54,14 +68,20 @@
         "valid_meddra_term_references": MedDRATermReferencesValidator,
         "valid_meddra_code_term_pairs": MedDRACodeTermPairsValidator,
         "variable_exists": VariableExists,
         "variable_names": VariableNames,
         "variable_permissibilities": VariablePermissibility,
         "variable_value_count": VariableValueCount,
         "variable_count": VariableCount,
+        "domain_label": DomainLabel,
+        "required_variables": RequiredVariables,
+        "expected_variables": ExpectedVariables,
+        "permissible_variables": PermissibleVariables,
+        "study_domains": StudyDomains,
+        "valid_codelist_dates": ValidCodelistDates,
     }
 
     @classmethod
     def register_service(cls, name: str, operation: Type[BaseOperation]) -> None:
         """
         Save mapping of operation name and it's implementation
         """
```

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/operations/variable_count.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/variable_count.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/operations/variable_names.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/variable_names.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/operations/variable_permissibility.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/variable_permissibility.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/operations/variable_value_count.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/dataset_builders/base_dataset_builder.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,75 @@
+from abc import abstractmethod
+from cdisc_rules_engine.constants.define_xml_constants import DEFINE_XML_FILE_NAME
+from cdisc_rules_engine.services.define_xml_reader import DefineXMLReader
 import pandas as pd
-from cdisc_rules_engine.operations.base_operation import BaseOperation
-import asyncio
-from collections import Counter
-from typing import List
 from cdisc_rules_engine.utilities.utils import (
-    get_corresponding_datasets,
+    get_directory_path,
     is_split_dataset,
+    get_corresponding_datasets,
 )
+from typing import List
 
 
-class VariableValueCount(BaseOperation):
-    def _execute_operation(self):
-        # get metadata
-        variable_value_count = asyncio.run(self._get_all_study_variable_value_counts())
-        return variable_value_count
+class BaseDatasetBuilder:
+    def __init__(
+        self,
+        rule,
+        data_service,
+        cache_service,
+        rule_processor,
+        data_processor,
+        dataset_path,
+        datasets,
+        domain,
+    ):
+        self.data_service = data_service
+        self.cache = cache_service
+        self.data_processor = data_processor
+        self.rule_processor = rule_processor
+        self.dataset_path = dataset_path
+        self.datasets = datasets
+        self.domain = domain
+        self.rule = rule
 
-    async def _get_all_study_variable_value_counts(self) -> dict:
+    @abstractmethod
+    def build(self) -> pd.DataFrame:
         """
-        Returns a mapping of variable values to the number
-        of times that value appears in the study.
+        Returns correct dataframe to operate on
         """
-        datasets_with_unique_domains = list(
-            {dataset["domain"]: dataset for dataset in self.params.datasets}.values()
-        )
-        coroutines = [
-            self._get_dataset_variable_value_count(dataset)
-            for dataset in datasets_with_unique_domains
-        ]
-        dataset_variable_value_counts: List[Counter] = await asyncio.gather(*coroutines)
-        return dict(sum(dataset_variable_value_counts, Counter()))
+        pass
 
-    async def _get_dataset_variable_value_count(self, dataset: dict) -> Counter:
-        domain = dataset.get("domain")
-        if is_split_dataset(self.params.datasets, domain):
-            files = [
-                f"{self.params.directory_path}/{dataset.get('filename')}"
-                for dataset in get_corresponding_datasets(self.params.datasets, domain)
-            ]
-            data: pd.DataFrame = self.data_service.join_split_datasets(
-                self.data_service.get_dataset, files
-            )
-        else:
-            data: pd.DataFrame = self.data_service.get_dataset(
-                f"{self.params.directory_path}/{dataset.get('filename')}"
+    def get_dataset(self, **kwargs):
+        # If validating dataset content, ensure split datasets are handled.
+        if is_split_dataset(self.datasets, self.domain):
+            # Handle split datasets for content checks.
+            # A content check is any check that is not in the list of rule types
+            dataset: pd.DataFrame = self.data_service.concat_split_datasets(
+                func_to_call=self.build,
+                dataset_names=self.get_corresponding_datasets_names(),
+                **kwargs,
             )
-        target_variable = self.params.target.replace("--", domain, 1)
-        if target_variable in data:
-            return Counter(data[target_variable].unique())
         else:
-            return Counter()
+            # single dataset. the most common case
+            dataset: pd.DataFrame = self.build()
+        return dataset
+
+    def get_corresponding_datasets_names(self) -> List[str]:
+        directory_path = get_directory_path(self.dataset_path)
+        return [
+            f"{directory_path}/{dataset['filename']}"
+            for dataset in get_corresponding_datasets(self.datasets, self.domain)
+        ]
+
+    def get_define_xml_variables_metadata(self) -> List[dict]:
+        """
+        Gets Define XML variables metadata.
+        """
+        directory_path = get_directory_path(self.dataset_path)
+        define_xml_path: str = f"{directory_path}/{DEFINE_XML_FILE_NAME}"
+        define_xml_contents: bytes = self.data_service.get_define_xml_contents(
+            dataset_name=define_xml_path
+        )
+        define_xml_reader = DefineXMLReader.from_file_contents(
+            define_xml_contents, cache_service_obj=self.cache
+        )
+        return define_xml_reader.extract_variables_metadata(domain_name=self.domain)
```

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/operations/whodrug_hierarchy_validator.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/whodrug_hierarchy_validator.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/operations/whodrug_references_validator.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/operations/whodrug_references_validator.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/plugin_loader.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/plugin_loader.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/serializers/__init__.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/serializers/dataset_metadata_serializer.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/serializers/dataset_metadata_serializer.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/serializers/rule_serializer.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/serializers/rule_serializer.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/serializers/term_serializers/atc_classification_serializer.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/serializers/term_serializers/atc_classification_serializer.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/serializers/term_serializers/atc_text_serializer.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/serializers/term_serializers/atc_text_serializer.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/serializers/term_serializers/drug_dictionary_serializer.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/serializers/term_serializers/drug_dictionary_serializer.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/serializers/term_serializers/meddra_term_serializer.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/serializers/term_serializers/meddra_term_serializer.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/adam_variable_reader.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/adam_variable_reader.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/cache/cache_populator_service.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/cache/cache_populator_service.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 )
 from cdisc_rules_engine.services.cdisc_library_service import CDISCLibraryService
 from cdisc_rules_engine.utilities.utils import (
     get_library_variables_metadata_cache_key,
     get_standard_details_cache_key,
     get_model_details_cache_key,
 )
+from cdisc_rules_engine.constants.cache_constants import PUBLISHED_CT_PACKAGES
 
 
 class CachePopulator:
     def __init__(
         self, cache: CacheServiceInterface, library_service: CDISCLibraryService
     ):
         self.cache = cache
@@ -45,14 +46,22 @@
                 rules.get("rules", []), "core_id", prefix=rules.get("key_prefix")
             )
 
         # save codelists to cache as a map of codelist to terms
         codelist_term_maps = await self._get_codelist_term_maps()
         self.cache.add_batch(codelist_term_maps, "package")
 
+        # Add a list of all published ct packages to the cache
+        available_packages = [
+            package.get("package")
+            for package in codelist_term_maps
+            if "package" in package
+        ]
+        self.cache.add(PUBLISHED_CT_PACKAGES, available_packages)
+
         # save standard codelists to cache as a map of variable to allowed_values
         standards = self.library_service.get_all_tabulation_ig_standards()
         standards.extend(self.library_service.get_all_collection_ig_standards())
         standards.extend(self.library_service.get_all_analysis_ig_standards())
 
         variable_codelist_maps = await self._get_variable_codelist_maps(standards)
         self.cache.add_batch(variable_codelist_maps, "name")
@@ -73,14 +82,49 @@
         variables_metadata: Iterable[dict] = await self._get_variables_metadata(
             standards
         )
         self.cache.add_batch(variables_metadata, "cache_key", pop_cache_key=True)
 
         return self.cache
 
+    async def load_codelists(self, packages: List[str]):
+        coroutines = [
+            self._async_get_codelist_terms_map(package) for package in packages
+        ]
+        codelist_term_maps = await asyncio.gather(*coroutines)
+        self.cache.add_batch(codelist_term_maps, "package")
+
+    async def load_available_ct_packages(self):
+        packages = self.library_service.get_all_ct_packages()
+        available_packages = [
+            package.get("href", "").split("/")[-1] for package in packages
+        ]
+        self.cache.add(PUBLISHED_CT_PACKAGES, available_packages)
+
+    async def load_standard(self, standard: str, version: str):
+        standards = [{"href": f"/mdr/{standard}/{version}"}]
+        variable_codelist_maps = await self._get_variable_codelist_maps(standards)
+        self.cache.add_batch(variable_codelist_maps, "name")
+        # save details of all standards to cache
+        standards_details: List[dict] = await self._async_get_details_of_all_standards(
+            standards
+        )
+        self.cache.add_batch(standards_details, "cache_key", pop_cache_key=True)
+
+        # save details of all standard's models to cache
+        standards_models: Iterable[
+            dict
+        ] = await self._async_get_details_of_all_standards_models(standards_details)
+        self.cache.add_batch(standards_models, "cache_key", pop_cache_key=True)
+        # save variables metadata to cache
+        variables_metadata: Iterable[dict] = await self._get_variables_metadata(
+            standards
+        )
+        self.cache.add_batch(variables_metadata, "cache_key", pop_cache_key=True)
+
     def save_rules_locally(self, file_path: str):
         """
         Store cached rules in rules.pkl in cache path directory
         """
         rules_data = self.cache.filter_cache("rules")
         with open(file_path, "wb") as f:
             pickle.dump(rules_data, f)
```

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/cache/cache_service_factory.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/cache/cache_service_factory.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/cache/in_memory_cache_service.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/cache/in_memory_cache_service.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/cache/redis_cache_service.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/cache/redis_cache_service.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/cdisc_library_service.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/cdisc_library_service.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/data_readers/data_reader_factory.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/data_readers/data_reader_factory.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/data_readers/xpt_reader.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/data_readers/xpt_reader.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/data_services/base_data_service.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/data_services/base_data_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 import asyncio
 from abc import ABC
 from functools import wraps, partial
-from typing import Callable, List, Optional, Iterable
+from typing import Callable, List, Optional, Iterable, Iterator
+from concurrent.futures import ThreadPoolExecutor
 
 import numpy as np
 import pandas as pd
 
 from cdisc_rules_engine.constants.domains import AP_DOMAIN_LENGTH
 from cdisc_rules_engine.interfaces import (
     CacheServiceInterface,
     ConfigInterface,
     DataServiceInterface,
 )
+from cdisc_rules_engine.constants.classes import (
+    FINDINGS,
+    FINDINGS_ABOUT,
+    EVENTS,
+    INTERVENTIONS,
+)
 from cdisc_rules_engine.models.dataset_types import DatasetTypes
 from cdisc_rules_engine.services import logger
 from cdisc_rules_engine.services.data_readers import DataReaderFactory
 from cdisc_rules_engine.utilities.utils import (
     get_dataset_cache_key_from_path,
     get_directory_path,
     search_in_list_of_dicts,
@@ -93,55 +100,53 @@
             DatasetTypes.METADATA.value: self.get_dataset_metadata,
             DatasetTypes.VARIABLES_METADATA.value: self.get_variables_metadata,
         }
         return dataset_type_to_function_map[dataset_type](
             dataset_name=dataset_name, **params
         )
 
-    def join_split_datasets(
+    def concat_split_datasets(
         self, func_to_call: Callable, dataset_names: List[str], **kwargs
     ) -> pd.DataFrame:
         """
         Accepts a list of split dataset filenames, asynchronously downloads
         all of them and merges into a single DataFrame.
 
         function_to_call must accept dataset_name and kwargs
         as input parameters and return pandas DataFrame.
         """
         # pop drop_duplicates param at the beginning to avoid passing it to func_to_call
         drop_duplicates: bool = kwargs.pop("drop_duplicates", False)
 
         # download datasets asynchronously
-        coroutines = [
-            self._async_get_dataset(func_to_call, name, **kwargs)
-            for name in dataset_names
-        ]
-        loop = asyncio.get_event_loop()
-        datasets: Iterable[pd.DataFrame] = loop.run_until_complete(
-            asyncio.gather(*coroutines)
+        datasets: Iterable[pd.DataFrame] = self._async_get_datasets(
+            func_to_call, dataset_names, **kwargs
         )
 
-        # join datasets
-        joined_dataset: pd.DataFrame = pd.concat(
+        # concat datasets
+        full_dataset: pd.DataFrame = pd.concat(
             [dataset for dataset in datasets],
             ignore_index=True,
         )
         if drop_duplicates:
-            joined_dataset.drop_duplicates()
-        return joined_dataset
+            full_dataset.drop_duplicates()
+        return full_dataset
 
     def get_dataset_class(
         self, dataset: pd.DataFrame, file_path: str, datasets: List[dict]
     ) -> Optional[str]:
         if self._contains_topic_variable(dataset, "TERM"):
-            return "Events"
+            return EVENTS
         elif self._contains_topic_variable(dataset, "TRT"):
-            return "Interventions"
+            return INTERVENTIONS
         elif self._contains_topic_variable(dataset, "TESTCD"):
-            return "Findings"
+            if self._contains_topic_variable(dataset, "OBJ"):
+                return FINDINGS_ABOUT
+            else:
+                return FINDINGS
         elif self._is_associated_persons(dataset):
             return self._get_associated_persons_inherit_class(
                 dataset, file_path, datasets
             )
         else:
             # Default case, unknown class
             return None
@@ -182,15 +187,18 @@
             return None
 
     def _contains_topic_variable(self, dataset, variable):
         """
         Checks if the given dataset-class string ends with a particular variable string.
         Returns True/False
         """
-        return dataset.columns.str.endswith(variable).any()
+        if "DOMAIN" not in dataset:
+            return False
+        domain = dataset["DOMAIN"].values[0]
+        return domain.upper() + variable in dataset
 
     def _domain_starts_with(self, domain, variable):
         """
         Checks if the given dataset-class string starts with
          a particular variable string.
         Returns True/False
         """
@@ -212,7 +220,24 @@
         """
         Asynchronously executes passed function_to_call.
         """
         loop = asyncio.get_event_loop()
         return await loop.run_in_executor(
             None, partial(function_to_call, dataset_name=dataset_name, **kwargs)
         )
+
+    def _async_get_datasets(
+        self, function_to_call: Callable, dataset_names: List[str], **kwargs
+    ) -> Iterator[pd.DataFrame]:
+        """
+        The method uses multithreading to download each
+        dataset in dataset_names param in parallel.
+
+        function_to_call param is a function that downloads
+        one dataset. So, this function is asynchronously called
+        for each item of dataset_names param.
+        """
+        with ThreadPoolExecutor() as executor:
+            return executor.map(
+                lambda name: function_to_call(dataset_name=name, **kwargs),
+                dataset_names,
+            )
```

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/data_services/data_service_factory.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/data_services/data_service_factory.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/data_services/dummy_data_service.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/data_services/dummy_data_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import datetime
 from io import IOBase
-from typing import List, Optional, Callable
+from typing import List, Optional
 
 import pandas as pd
 
 from cdisc_rules_engine.dummy_models.dummy_dataset import DummyDataset
 from cdisc_rules_engine.exceptions.custom_exceptions import DatasetNotFoundError
 from cdisc_rules_engine.interfaces import CacheServiceInterface, ConfigInterface
 from cdisc_rules_engine.models.dataset_metadata import DatasetMetadata
@@ -23,14 +23,15 @@
         cache_service: CacheServiceInterface,
         reader_factory: DataReaderFactory,
         config: ConfigInterface,
         **kwargs,
     ):
         super(DummyDataService, self).__init__(cache_service, reader_factory, config)
         self.data: List[DummyDataset] = kwargs.get("data")
+        self.define_xml: str = kwargs.get("define_xml")
 
     @classmethod
     def get_instance(
         cls, cache_service: CacheServiceInterface, config: ConfigInterface, **kwargs
     ):
         return cls(
             cache_service=cache_service,
@@ -80,14 +81,15 @@
     def get_variables_metadata(self, dataset_name: str, **params) -> pd.DataFrame:
         metadata_to_return = {
             "variable_name": [],
             "variable_order": [],
             "variable_label": [],
             "variable_size": [],
             "variable_data_type": [],
+            "variable_format": [],
         }
         dataset: DummyDataset = self.get_dataset_data(dataset_name)
         for i, variable in enumerate(dataset.variables):
             metadata_to_return["variable_name"] = metadata_to_return[
                 "variable_name"
             ] + [variable.name]
             metadata_to_return["variable_order"] = metadata_to_return[
@@ -98,15 +100,17 @@
             ] + [variable.label]
             metadata_to_return["variable_size"] = metadata_to_return[
                 "variable_size"
             ] + [variable.length]
             metadata_to_return["variable_data_type"] = metadata_to_return[
                 "variable_data_type"
             ] + [variable.type]
-
+            metadata_to_return["variable_format"] = metadata_to_return[
+                "variable_format"
+            ] + [variable.format]
         return pd.DataFrame.from_dict(metadata_to_return)
 
     def get_dataset_by_type(
         self, dataset_name: str, dataset_type: str, **params
     ) -> pd.DataFrame:
         dataset_type_to_function_map: dict = {
             DatasetTypes.CONTENTS.value: self.get_dataset,
@@ -114,22 +118,19 @@
             DatasetTypes.VARIABLES_METADATA.value: self.get_variables_metadata,
         }
         return dataset_type_to_function_map[dataset_type](
             dataset_name=dataset_name, **params
         )
 
     def get_define_xml_contents(self, dataset_name: str) -> bytes:
-        pass
+        return bytes(self.define_xml)
 
     def has_all_files(self, prefix: str, file_names: List[str]) -> bool:
         return True
 
-    def join_split_datasets(self, func_to_call: Callable, dataset_names, **kwargs):
-        pass
-
     def read_data(self, file_path: str) -> IOBase:
         pass
 
     def __get_dataset_metadata(self, dataset_name: str, **kwargs) -> dict:
         dataset: Optional[DummyDataset] = self.get_dataset_data(dataset_name)
         metadata_to_return = {}
         if dataset:
```

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/data_services/local_data_service.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/data_services/local_data_service.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
-from concurrent.futures import ThreadPoolExecutor
 from io import IOBase
-from typing import Callable, Iterator, List, Optional, Tuple
+from typing import List, Optional, Tuple
 
 import pandas
 
 from cdisc_rules_engine.interfaces import CacheServiceInterface, ConfigInterface
 from cdisc_rules_engine.models.dataset_metadata import DatasetMetadata
 from cdisc_rules_engine.models.dataset_types import DatasetTypes
 from cdisc_rules_engine.models.variable_metadata_container import (
@@ -126,61 +125,24 @@
             DatasetTypes.METADATA.value: self.get_dataset_metadata,
             DatasetTypes.VARIABLES_METADATA.value: self.get_variables_metadata,
         }
         return dataset_type_to_function_map[dataset_type](
             dataset_name=dataset_name, **params
         )
 
-    def join_split_datasets(
-        self, func_to_call: Callable, dataset_names: List[str], **kwargs
-    ) -> pandas.DataFrame:
-        """
-        Accepts a list of split dataset filenames,
-        downloads all of them and merges into a single DataFrame.
-        """
-        # popping drop_duplicates param at the beginning to avoid
-        # passing it to func_to_call
-        drop_duplicates: bool = kwargs.pop("drop_duplicates", False)
-        datasets: Iterator[pandas.DataFrame] = self._async_get_datasets(
-            func_to_call, dataset_names, **kwargs
-        )
-        joined_dataset: pandas.DataFrame = pandas.concat(
-            [dataset for dataset in datasets],
-            ignore_index=True,
-        )
-        if drop_duplicates:
-            joined_dataset.drop_duplicates()
-        return joined_dataset
-
-    def _async_get_datasets(
-        self, function_to_call: Callable, dataset_names: List[str], **kwargs
-    ) -> Iterator[pandas.DataFrame]:
-        """
-        The method uses multithreading to download each
-        dataset in dataset_names param in parallel.
-
-        function_to_call param is a function that downloads
-        one dataset. So, this function is asynchronously called
-        for each item of dataset_names param.
-        """
-        with ThreadPoolExecutor() as executor:
-            return executor.map(
-                lambda name: function_to_call(dataset_name=name, **kwargs),
-                dataset_names,
-            )
-
     def read_metadata(self, file_path: str) -> dict:
         file_size = os.path.getsize(file_path)
+        file_name = extract_file_name_from_path_string(file_path)
         file_metadata = {
             "path": file_path,
-            "name": extract_file_name_from_path_string(file_path),
+            "name": file_name,
             "size": file_size,
         }
         with open(file_path, "rb") as f:
-            contents_metadata = DatasetMetadataReader(f.read()).read()
+            contents_metadata = DatasetMetadataReader(f.read(), file_name).read()
 
         return {
             "file_metadata": file_metadata,
             "contents_metadata": contents_metadata,
         }
 
     def read_data(self, file_path: str) -> IOBase:
```

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/dataset_metadata_reader.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/dataset_metadata_reader.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,61 +13,66 @@
     """
     Responsibility of the class is to read metadata
     from .xpt file.
     """
 
     # TODO. Maybe in future it is worth having multiple constructors
     #  like from_bytes, from_file etc. But now there is no immediate need for that.
-    def __init__(self, contents_in_bytes: bytes):
+    def __init__(self, contents_in_bytes: bytes, file_name: str):
         self._file_contents = contents_in_bytes
         self._metadata_container = None
         self._domain_name = None
+        self._dataset_name = file_name.split(".")[0].upper()
 
     def read(self) -> dict:
         """
         Extracts metadata from binary contents of .xpt file.
         """
         dataset_container = xport.v56.loads(self._file_contents)
         dataset_id = next(iter(dataset_container))
         dataset = dataset_container.get(dataset_id)
         self._domain_name = self._extract_domain_name(dataset)
         self._metadata_container = {
             "variable_labels": list(dataset.contents.Label.values),
             "variable_names": list(dataset.contents.Variable.values),
+            "variable_formats": list(dataset.contents.Format.values),
             "variable_name_to_label_map": pd.Series(
                 dataset.contents.Label.values, index=dataset.contents.Variable
             ).to_dict(),
             "variable_name_to_data_type_map": pd.Series(
                 dataset.contents.Type.values, index=dataset.contents.Variable
             ).to_dict(),
             "variable_name_to_size_map": pd.Series(
                 dataset.contents.Length.values, index=dataset.contents.Variable
             ).to_dict(),
             "number_of_variables": len(dataset.columns),
             "dataset_label": dataset.dataset_label,
             "domain_name": self._domain_name,
-            "dataset_name": dataset.name,
+            "dataset_name": self._dataset_name,
             "dataset_modification_date": dataset.modified.isoformat(),
         }
         self._domain_name = self._extract_domain_name(dataset)
         self._convert_variable_types()
         self._metadata_container["adam_info"] = self._extract_adam_info(
             self._metadata_container["variable_names"]
         )
         logger.info(f"Extracted dataset metadata. metadata={self._metadata_container}")
         return self._metadata_container
 
     def _extract_domain_name(self, df):
-        first_row = df.iloc[0]
-        if "DOMAIN" in first_row:
-            domain_name = first_row["DOMAIN"]
-            if isinstance(domain_name, bytes):
-                return domain_name.decode("utf-8")
-            else:
-                return str(domain_name)
+        try:
+            first_row = df.iloc[0]
+            if "DOMAIN" in first_row:
+                domain_name = first_row["DOMAIN"]
+                if isinstance(domain_name, bytes):
+                    return domain_name.decode("utf-8")
+                else:
+                    return str(domain_name)
+        except IndexError:
+            pass
         return None
 
     def _convert_variable_types(self):
         """
         Converts variable types to the format that
         rule authors use.
         """
@@ -87,23 +92,24 @@
     def _to_dict(self) -> dict:
         """
         This method is used to transform metadata_container
         object into dictionary.
         """
         return {
             "variable_labels": self._metadata_container.column_labels,
+            "variable_formats": self._metadata_container.column_formats,
             "variable_names": self._metadata_container.column_names,
-            "variable_name_to_label_map": self._metadata_container.column_names_to_labels,
-            "variable_name_to_data_type_map": self._metadata_container.readstat_variable_types,
-            "variable_name_to_size_map": self._metadata_container.variable_storage_width,
+            "variable_name_to_label_map": self._metadata_container.column_names_to_labels,  # noqa
+            "variable_name_to_data_type_map": self._metadata_container.readstat_variable_types,  # noqa
+            "variable_name_to_size_map": self._metadata_container.variable_storage_width,  # noqa
             "number_of_variables": self._metadata_container.number_columns,
             "dataset_label": self._metadata_container.file_label,
             "domain_name": self._domain_name,
-            "dataset_name": self._metadata_container.table_name,
-            "dataset_modification_date": self._metadata_container.dataset_modification_date,
+            "dataset_name": self._dataset_name,
+            "dataset_modification_date": self._metadata_container.dataset_modification_date,  # noqa
         }
 
     def _extract_adam_info(self, variable_names):
         ad = AdamVariableReader()
         adam_columns = ad.extract_columns(variable_names)
         for column in adam_columns:
             ad.check_y(column)
```

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/define_xml_reader.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/define_xml_reader.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/logging/console_logger.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/logging/console_logger.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/logging/logging_service_factory.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/logging/logging_service_factory.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/reporting/base_report.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/reporting/base_report.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,17 +33,16 @@
     def get_summary_data(self) -> List[List]:
         """
         Generates the Issue Summary data that goes into the export.
         Each row is represented by a list or a dict containing the following
         information:
         return [
             "Dataset",
-            "RuleID",
+            "CORE-ID",
             "Message",
-            "Executability",
             "Issues",
             "Explanation"
         ]
         """
         summary_data = []
         for validation_result in self._results:
             if validation_result.execution_status == "success":
@@ -51,52 +50,53 @@
                     dataset = result.get("domain")
                     if (
                         result.get("errors")
                         and result.get("executionStatus") == "success"
                     ):
                         summary_item = {
                             "dataset": dataset,
-                            "rule_id": validation_result.id,
+                            "core_id": validation_result.id,
                             "message": result.get("message"),
-                            "executability": validation_result.executability,
                             "issues": len(result.get("errors")),
                         }
 
                         if self._item_type == "list":
                             summary_data.extend([[*summary_item.values()]])
                         elif self._item_type == "dict":
                             summary_data.extend([summary_item])
 
         return sorted(
             summary_data,
             key=lambda x: (x[0], x[1])
             if (self._item_type == "list")
-            else (x["dataset"], x["rule_id"]),
+            else (x["dataset"], x["core_id"]),
         )
 
     def get_detailed_data(self) -> List[List]:
         detailed_data = []
         for validation_result in self._results:
             detailed_data = detailed_data + self._generate_error_details(
                 validation_result
             )
         return sorted(
             detailed_data,
             key=lambda x: (x[0], x[3])
             if (self._item_type == "list")
-            else (x["rule_id"], x["dataset"]),
+            else (x["core_id"], x["dataset"]),
         )
 
-    def _generate_error_details(self, validation_result) -> List[List]:
+    def _generate_error_details(
+        self, validation_result: RuleValidationResult
+    ) -> List[List]:
         """
         Generates the Issue details data that goes into the excel export.
         Each row is represented by a list or a dict containing the following
         information:
         return [
-            "RuleID",
+            "CORE-ID",
             "Message",
             "Executability",
             "Dataset",
             "USUBJID",
             "Record",
             "Sequence",
             "Variable(s)",
@@ -105,21 +105,21 @@
         """
         errors = []
         for result in validation_result.results or []:
             if result.get("errors", []) and result.get("executionStatus") == "success":
                 variables = result.get("variables", [])
                 for error in result.get("errors"):
                     error_item = {
-                        "rule_id": validation_result.id,
+                        "core_id": validation_result.id,
                         "message": result.get("message"),
                         "executability": validation_result.executability,
                         "dataset": result.get("domain"),
-                        "uSubjId": error.get("uSubjId", ""),
+                        "USUBJID": error.get("USUBJID", ""),
                         "row": error.get("row", ""),
-                        "seq": error.get("seq", ""),
+                        "SEQ": error.get("SEQ", ""),
                     }
 
                     if self._item_type == "list":
                         error_item["variables"] = ", ".join(variables)
                         error_item["values"] = ", ".join(
                             [
                                 str(error.get("value", {}).get(variable))
@@ -138,38 +138,44 @@
 
     def get_rules_report_data(self) -> List[List]:
         """
         Generates the rules report data that goes into the excel export.
         Each row is represented by a list or a dict containing the following
         information:
         [
-            "RuleID",
+            "CORE-ID",
             "Version",
+            "CDISC RuleID",
+            "FDA RuleID",
+            "PMDA RuleID",
             "Message",
             "Status"
         ]
         """
         rules_report = []
         for validation_result in self._results:
             rules_item = {
-                "rule_id": validation_result.id,
+                "core_id": validation_result.id,
                 "version": "1",
+                "cdisc_rule_id": validation_result.cdisc_rule_id,
+                "fda_rule_id": validation_result.fda_rule_id,
+                "pmda_rule_id": validation_result.pmda_rule_id,
                 "message": validation_result.message,
                 "status": ExecutionStatus.SUCCESS.value.upper()
                 if validation_result.execution_status == ExecutionStatus.SUCCESS.value
                 else ExecutionStatus.SKIPPED.value.upper(),
             }
             if self._item_type == "list":
                 rules_report.append([*rules_item.values()])
             elif self._item_type == "dict":
                 rules_report.append(rules_item)
 
         return sorted(
             rules_report,
-            key=lambda x: x[0] if (self._item_type == "list") else x["rule_id"],
+            key=lambda x: x[0] if (self._item_type == "list") else x["core_id"],
         )
 
     @property
     @abstractmethod
     def _file_format(self) -> str:
         pass
```

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/reporting/excel_report.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/reporting/excel_report.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 from datetime import datetime
 from typing import BinaryIO, List, Optional, Iterable
 
 from openpyxl import Workbook
-from openpyxl.styles import Alignment
 
+from version import __version__
 from cdisc_rules_engine.enums.report_types import ReportTypes
 from cdisc_rules_engine.models.rule_validation_result import RuleValidationResult
 from cdisc_rules_engine.models.validation_args import Validation_args
 from .base_report import BaseReport
 from .excel_writer import (
     excel_open_workbook,
     excel_update_worksheet,
@@ -49,28 +49,29 @@
         detailed_data = self.get_detailed_data()
         rules_report_data = self.get_rules_report_data()
         excel_update_worksheet(wb["Issue Summary"], summary_data, dict(wrap_text=True))
         excel_update_worksheet(wb["Issue Details"], detailed_data, dict(wrap_text=True))
         excel_update_worksheet(
             wb["Rules Report"], rules_report_data, dict(wrap_text=True)
         )
-        wb["Conformance Details"]["B2"] = ",\n".join(self._dataset_paths[:5])
-        wb["Conformance Details"]["B2"].alignment = Alignment(wrapText=True)
         # write conformance data
-        wb["Conformance Details"]["B3"] = (
+        wb["Conformance Details"]["B2"] = (
             datetime.now().replace(microsecond=0).isoformat()
         )
-        wb["Conformance Details"]["B4"] = f"{round(self._elapsed_time, 2)} seconds"
-        # write bundle details
-        wb["Conformance Details"]["B8"] = standard.upper()
-        wb["Conformance Details"]["B9"] = f"V{version}"
-        wb["Conformance Details"]["B10"] = ", ".join(cdiscCt)
-        wb["Conformance Details"]["B11"] = define_version
-        wb["Conformance Details"]["B14"] = self._args.meddra
-        wb["Conformance Details"]["B15"] = self._args.whodrug
+        wb["Conformance Details"]["B3"] = f"{round(self._elapsed_time, 2)} seconds"
+        wb["Conformance Details"]["B4"] = __version__
+        # write standards details
+        wb["Conformance Details"]["B7"] = standard.upper()
+        wb["Conformance Details"]["B8"] = f"V{version}"
+        wb["Conformance Details"]["B9"] = ", ".join(cdiscCt)
+        wb["Conformance Details"]["B10"] = define_version
+        if self._args.meddra:
+            wb["Conformance Details"]["B13"] = self._args.meddra
+        if self._args.whodrug:
+            wb["Conformance Details"]["B14"] = self._args.whodrug
         return wb
 
     def write_report(self):
         logger = logging.getLogger("validator")
 
         try:
             define_version: str = self._args.define_version or get_define_version(
```

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/reporting/excel_writer.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/reporting/excel_writer.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/reporting/json_report.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/reporting/json_report.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/services/reporting/report_factory.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/services/reporting/report_factory.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/utilities/data_processor.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/utilities/data_processor.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/utilities/dataset_preprocessor.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/utilities/dataset_preprocessor.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,14 @@
             ]
             result = self._merge_datasets(
                 left_dataset=result,
                 left_dataset_domain_name=self._dataset_domain,
                 right_dataset=other_dataset,
                 right_dataset_domain_details=domain_details,
             )
-
         logger.info(f"Dataset after preprocessing = {result}")
         return result
 
     def _is_split_domain(self, domain: str) -> bool:
         return domain == self._dataset_domain
 
     def _download_dataset(self, filename: str) -> pd.DataFrame:
```

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/utilities/decorators.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/utilities/decorators.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/utilities/progress_displayers.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/utilities/progress_displayers.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/utilities/reporting_utilities.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/utilities/reporting_utilities.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,12 +9,12 @@
     """
     Method used to extract define version from xml file located
      in the same directory with datasets
     """
     if not dataset_paths:
         return None
     path_to_data = os.path.dirname(dataset_paths[0])
-    if DEFINE_XML_FILE_NAME not in os.listdir(path_to_data):
+    if not path_to_data or DEFINE_XML_FILE_NAME not in os.listdir(path_to_data):
         return None
     path_to_define = "/".join([path_to_data, DEFINE_XML_FILE_NAME])
     define_xml_reader = DefineXMLReader.from_filename(path_to_define)
     return define_xml_reader.get_define_version()
```

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/utilities/rule_processor.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/utilities/rule_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import re
 from typing import List, Optional, Set, Union, Tuple
 
 import pandas as pd
 
-from cdisc_rules_engine.constants.classes import DETECTABLE_CLASSES
+from cdisc_rules_engine.constants.classes import (
+    DETECTABLE_CLASSES,
+    FINDINGS_ABOUT,
+    FINDINGS,
+)
 from cdisc_rules_engine.constants.domains import (
     AP_DOMAIN,
     APFA_DOMAIN,
     SUPPLEMENTARY_DOMAINS,
 )
 from cdisc_rules_engine.constants.rule_constants import ALL_KEYWORD
 from cdisc_rules_engine.interfaces import ConditionInterface
@@ -170,25 +174,28 @@
         is_excluded = False
         if included_classes:
             dataset = self.data_service.get_dataset(dataset_name=file_path)
             class_name = self.data_service.get_dataset_class(
                 dataset, file_path, datasets
             )
             if (
-                class_name not in included_classes
-                and ALL_KEYWORD not in included_classes
-            ):
+                (class_name not in included_classes)
+                and not (class_name == FINDINGS_ABOUT and FINDINGS in included_classes)
+            ) and ALL_KEYWORD not in included_classes:
                 is_included = False
 
         if excluded_classes:
             dataset = self.data_service.get_dataset(dataset_name=file_path)
             class_name = self.data_service.get_dataset_class(
                 dataset, file_path, datasets
             )
-            if class_name and class_name in excluded_classes:
+            if class_name and (
+                (class_name in excluded_classes)
+                or (class_name == FINDINGS_ABOUT and FINDINGS in excluded_classes)
+            ):
                 is_excluded = True
         return is_included and not is_excluded
 
     def valid_rule_structure(self, rule) -> bool:
         required_keys = ["standards", "core_id"]
         for key in required_keys:
             if key not in rule:
@@ -263,17 +270,18 @@
         # check cache
         cache_key = get_operations_cache_key(
             directory_path=operation_params.directory_path,
             operation_name=operation_params.operation_name,
             domain=operation_params.domain,
             grouping=";".join(operation_params.grouping),
             target_variable=operation_params.target,
+            dataset_path=operation_params.dataset_path,
         )
-        result = self.cache.get(cache_key)
-        if result:
+        result: pd.DataFrame = self.cache.get(cache_key)
+        if result is not None:
             return result
 
         if not self.is_current_domain(
             operation_params.dataframe, operation_params.domain
         ):
             # download other domain
             domain_details: dict = search_in_list_of_dicts(
```

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/utilities/utils.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/utilities/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 from cdisc_rules_engine.constants.domains import (
     AP_DOMAIN,
     APFA_DOMAIN,
     APRELSUB_DOMAIN,
     SUPPLEMENTARY_DOMAINS,
 )
+from cdisc_rules_engine.constants.classes import SPECIAL_PURPOSE
 from cdisc_rules_engine.enums.execution_status import ExecutionStatus
 from cdisc_rules_engine.interfaces import ConditionInterface
 from cdisc_rules_engine.models.base_validation_entity import BaseValidationEntity
 
 
 def convert_file_size(size_in_bytes: int, desired_unit: str) -> float:
     """
@@ -171,20 +172,21 @@
 
 def get_operations_cache_key(
     directory_path: str,
     domain: str = None,
     operation_name: str = None,
     grouping: str = None,
     target_variable: str = None,
+    dataset_path: str = None,
 ) -> str:
     """
     Creates the cache key for operations.
     """
     key = f"operations/{directory_path}"
-    optional_items = [domain, operation_name, grouping, target_variable]
+    optional_items = [domain, operation_name, grouping, target_variable, dataset_path]
     for item in optional_items:
         if item:
             key = f"{key}/{item}"
     return key
 
 
 def get_directory_path(dataset_path):
@@ -305,9 +307,14 @@
 def get_dictionary_path(directory_path: str, file_name: str) -> str:
     """
     Creates a path to dictionary directory or file.
     """
     return os.path.join(directory_path, file_name)
 
 
+def convert_library_class_name_to_ct_class(class_name: str):
+    conversions = {"special-purpose": SPECIAL_PURPOSE}
+    return conversions.get(class_name.lower(), class_name.upper())
+
+
 def decode_line(line: bytes) -> str:
     return line.decode("utf-8").replace("\n", "").replace("\r", "")
```

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine/utilities/validation_output_container.py` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine/utilities/validation_output_container.py`

 * *Files identical despite different names*

### Comparing `cdisc-rules-engine-0.5.6/cdisc_rules_engine.egg-info/SOURCES.txt` & `cdisc-rules-engine-0.6.0/cdisc_rules_engine.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,41 @@
 LICENSE
 README.md
 setup.py
+TestRule/__init__.py
+cdisc_rule_tester/__init__.py
+cdisc_rule_tester/models/__init__.py
+cdisc_rule_tester/models/rule_tester.py
 cdisc_rules_engine/__init__.py
 cdisc_rules_engine/plugin_loader.py
 cdisc_rules_engine/rules_engine.py
 cdisc_rules_engine.egg-info/PKG-INFO
 cdisc_rules_engine.egg-info/SOURCES.txt
 cdisc_rules_engine.egg-info/dependency_links.txt
 cdisc_rules_engine.egg-info/requires.txt
 cdisc_rules_engine.egg-info/top_level.txt
 cdisc_rules_engine/config/__init__.py
 cdisc_rules_engine/config/config.py
 cdisc_rules_engine/constants/__init__.py
+cdisc_rules_engine/constants/cache_constants.py
 cdisc_rules_engine/constants/classes.py
 cdisc_rules_engine/constants/define_xml_constants.py
 cdisc_rules_engine/constants/domains.py
 cdisc_rules_engine/constants/patterns.py
+cdisc_rules_engine/constants/permissibility.py
 cdisc_rules_engine/constants/rule_constants.py
+cdisc_rules_engine/dataset_builders/__init__.py
+cdisc_rules_engine/dataset_builders/base_dataset_builder.py
+cdisc_rules_engine/dataset_builders/content_metadata_dataset_builder.py
+cdisc_rules_engine/dataset_builders/contents_dataset_builder.py
+cdisc_rules_engine/dataset_builders/dataset_builder_factory.py
+cdisc_rules_engine/dataset_builders/define_variables_dataset_builder.py
+cdisc_rules_engine/dataset_builders/domain_list_dataset_builder.py
+cdisc_rules_engine/dataset_builders/variables_metadata_dataset_builder.py
+cdisc_rules_engine/dataset_builders/variables_metadata_with_define_dataset_builder.py
 cdisc_rules_engine/dummy_models/__init__.py
 cdisc_rules_engine/dummy_models/dummy_dataset.py
 cdisc_rules_engine/dummy_models/dummy_variable.py
 cdisc_rules_engine/enums/__init__.py
 cdisc_rules_engine/enums/base_enum.py
 cdisc_rules_engine/enums/default_file_paths.py
 cdisc_rules_engine/enums/execution_status.py
@@ -89,26 +104,34 @@
 cdisc_rules_engine/models/rule_conditions/not_condition_composite.py
 cdisc_rules_engine/models/rule_conditions/single_condition.py
 cdisc_rules_engine/operations/__init__.py
 cdisc_rules_engine/operations/base_operation.py
 cdisc_rules_engine/operations/dataset_column_order.py
 cdisc_rules_engine/operations/day_data_validator.py
 cdisc_rules_engine/operations/distinct.py
+cdisc_rules_engine/operations/domain_label.py
+cdisc_rules_engine/operations/expected_variables.py
 cdisc_rules_engine/operations/extract_metadata.py
 cdisc_rules_engine/operations/library_column_order.py
+cdisc_rules_engine/operations/library_model_column_order.py
 cdisc_rules_engine/operations/max_date.py
 cdisc_rules_engine/operations/maximum.py
 cdisc_rules_engine/operations/mean.py
 cdisc_rules_engine/operations/meddra_code_references_validator.py
 cdisc_rules_engine/operations/meddra_code_term_pairs_validator.py
 cdisc_rules_engine/operations/meddra_term_references_validator.py
 cdisc_rules_engine/operations/min_date.py
 cdisc_rules_engine/operations/minimum.py
 cdisc_rules_engine/operations/operations_factory.py
+cdisc_rules_engine/operations/parent_library_model_column_order.py
+cdisc_rules_engine/operations/permissible_variables.py
 cdisc_rules_engine/operations/record_count.py
+cdisc_rules_engine/operations/required_variables.py
+cdisc_rules_engine/operations/study_domains.py
+cdisc_rules_engine/operations/valid_codelist_dates.py
 cdisc_rules_engine/operations/variable_count.py
 cdisc_rules_engine/operations/variable_exists.py
 cdisc_rules_engine/operations/variable_names.py
 cdisc_rules_engine/operations/variable_permissibility.py
 cdisc_rules_engine/operations/variable_value_count.py
 cdisc_rules_engine/operations/whodrug_hierarchy_validator.py
 cdisc_rules_engine/operations/whodrug_references_validator.py
```

### Comparing `cdisc-rules-engine-0.5.6/setup.py` & `cdisc-rules-engine-0.6.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     url="https://github.com/cdisc-org/cdisc-rules-engine",
     packages=setuptools.find_packages(exclude=["scripts", "tests"]),
     license="MIT",
     include_package_data=True,
     python_requires=">=3.8",
     install_requires=[
         "pandas>=1.3.5",
-        "business-rules-enhanced==1.2.6",
+        "business-rules-enhanced==1.3.4",
         "python-dotenv==0.20.0",
         "cdisc-library-client==0.1.4",
         "odmlib==0.1.4",
         "xport==3.6.1",
         "redis==4.0.2",
         "openpyxl==3.0.10",
         "importlib-metadata==5.0.0",
```

