# Comparing `tmp/indy-node-1.9.2.dev1069.tar.gz` & `tmp/indy-node-1.9.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/indy-node-1.9.2.dev1069.tar", last modified: Thu Aug 29 07:29:56 2019, max compression
+gzip compressed data, was "dist/indy-node-1.9.2rc1.tar", last modified: Thu Aug 29 11:08:59 2019, max compression
```

## Comparing `indy-node-1.9.2.dev1069.tar` & `indy-node-1.9.2rc1.tar`

### file list

```diff
@@ -1,551 +1,553 @@
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/
--rw-rw-r--   0 sovrin    (1003)     1004      145 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/MANIFEST.in
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_common/
--rw-rw-r--   0 sovrin    (1003)     1004     1584 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/config_helper.py
--rw-rw-r--   0 sovrin    (1003)     1004     2821 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/req_utils.py
--rw-rw-r--   0 sovrin    (1003)     1004    17898 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/types.py
--rw-rw-r--   0 sovrin    (1003)     1004     3082 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/strict_types.py
--rw-rw-r--   0 sovrin    (1003)     1004      189 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/did_method.py
--rw-rw-r--   0 sovrin    (1003)     1004     2168 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/setup_util.py
--rw-rw-r--   0 sovrin    (1003)     1004      743 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/exceptions.py
--rw-rw-r--   0 sovrin    (1003)     1004      821 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/txn_util.py
--rw-rw-r--   0 sovrin    (1003)     1004      702 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/roles.py
--rw-rw-r--   0 sovrin    (1003)     1004      328 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/generates_request.py
--rw-rw-r--   0 sovrin    (1003)     1004      109 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/serialization.py
--rw-rw-r--   0 sovrin    (1003)     1004     2835 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/config.py
--rw-rw-r--   0 sovrin    (1003)     1004     4853 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/util.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004     4882 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/auth.py
--rw-rw-r--   0 sovrin    (1003)     1004     2247 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/node_version_fallback.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_common/test/
--rw-rw-r--   0 sovrin    (1003)     1004     3334 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/conftest.py
--rw-rw-r--   0 sovrin    (1003)     1004     6149 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/test_transactions.py
--rw-rw-r--   0 sovrin    (1003)     1004     5390 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/test_req_utils_claim_def.py
--rw-rw-r--   0 sovrin    (1003)     1004      899 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/test_strict_schema.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_common/test/types/
--rw-rw-r--   0 sovrin    (1003)     1004      838 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/types/test_claim_def_sub_schema.py
--rw-rw-r--   0 sovrin    (1003)     1004     1211 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/types/test_schema_schema.py
--rw-rw-r--   0 sovrin    (1003)     1004      812 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/types/test_claim_def_get_schema.py
--rw-rw-r--   0 sovrin    (1003)     1004     1263 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/types/test_get_schema_schema.py
--rw-rw-r--   0 sovrin    (1003)     1004      672 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/types/test_get_revoc_reg_delta_schema.py
--rw-rw-r--   0 sovrin    (1003)     1004     2415 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/types/test_auth_rule_schema.py
--rw-rw-r--   0 sovrin    (1003)     1004     1730 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/types/test_revoc_def_submit_schema.py
--rw-rw-r--   0 sovrin    (1003)     1004     8233 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/types/test_attrib.py
--rw-rw-r--   0 sovrin    (1003)     1004      802 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/types/test_attrib_schema.py
--rw-rw-r--   0 sovrin    (1003)     1004      758 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/types/test_discl_schema.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/types/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004     1137 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/types/test_pool_upg_schema.py
--rw-rw-r--   0 sovrin    (1003)     1004      534 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/types/test_get_revoc_reg_def_schema.py
--rw-rw-r--   0 sovrin    (1003)     1004      809 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/types/test_get_attrib_schema.py
--rw-rw-r--   0 sovrin    (1003)     1004      688 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/types/test_pool_config_schema.py
--rw-rw-r--   0 sovrin    (1003)     1004     1666 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/types/test_revoc_def_entry_submit_schema.py
--rw-rw-r--   0 sovrin    (1003)     1004      619 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/types/test_get_revoc_reg_entry_schema.py
--rw-rw-r--   0 sovrin    (1003)     1004      651 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/types/test_get_nym_schema.py
--rw-rw-r--   0 sovrin    (1003)     1004     1032 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/types/test_get_auth_rule_schema.py
--rw-rw-r--   0 sovrin    (1003)     1004       86 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/__init__.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_common/test/version/
--rw-rw-r--   0 sovrin    (1003)     1004      849 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/version/test_version.py
--rw-rw-r--   0 sovrin    (1003)     1004     3610 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/version/test_node_version_fallback.py
--rw-rw-r--   0 sovrin    (1003)     1004     1163 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/version/test_node_version.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/version/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004       41 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/__main__.py
--rw-rw-r--   0 sovrin    (1003)     1004      948 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/constants.py
--rw-rw-r--   0 sovrin    (1003)     1004     1429 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/test_strict_types.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_common/test/state/
--rw-rw-r--   0 sovrin    (1003)     1004     1603 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/state/test_state_path.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/state/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004     4112 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/test_req_utils_schema.py
--rw-rw-r--   0 sovrin    (1003)     1004     1661 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/helper.py
--rw-rw-r--   0 sovrin    (1003)     1004      779 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/test_roles.py
--rw-rw-r--   0 sovrin    (1003)     1004      405 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/test_util.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_common/test/auth/
--rw-rw-r--   0 sovrin    (1003)     1004     8147 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/auth/test_auth_constraint.py
--rw-rw-r--   0 sovrin    (1003)     1004    10385 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/auth/test_endorser_authorizer.py
--rw-rw-r--   0 sovrin    (1003)     1004     2506 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/auth/conftest.py
--rw-rw-r--   0 sovrin    (1003)     1004     1295 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/auth/test_auth_rev_reg_def_with_new_auth_map.py
--rw-rw-r--   0 sovrin    (1003)     1004      767 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/auth/test_auth_for_auth_rule_new_auth_map.py
--rw-rw-r--   0 sovrin    (1003)     1004      905 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/auth/test_auth_anyone.py
--rw-rw-r--   0 sovrin    (1003)     1004     3953 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/auth/test_auth_strategies.py
--rw-rw-r--   0 sovrin    (1003)     1004     2993 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/auth/test_config_ledger_auth_strategy.py
--rw-rw-r--   0 sovrin    (1003)     1004     7295 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/auth/test_auth_node_with_new_auth_map.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_common/test/auth/multi_sig/
--rw-rw-r--   0 sovrin    (1003)     1004     1763 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/auth/multi_sig/conftest.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/auth/multi_sig/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004     1779 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/auth/multi_sig/test_auth_multi_sig_for_5_owners.py
--rw-rw-r--   0 sovrin    (1003)     1004     1228 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/auth/multi_sig/test_auth_multi_sig_for_1_owner.py
--rw-rw-r--   0 sovrin    (1003)     1004      678 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/auth/test_auth_txn_author_agreement_with_new_auth_map.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/auth/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004     1178 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/auth/test_auth_schema_with_new_auth_map.py
--rw-rw-r--   0 sovrin    (1003)     1004     8259 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/auth/test_role_authorizer.py
--rw-rw-r--   0 sovrin    (1003)     1004     2291 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/auth/test_auth_pool_upgrade_with_new_auth_map.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_common/test/auth/metadata/
--rw-rw-r--   0 sovrin    (1003)     1004     2201 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/auth/metadata/conftest.py
--rw-rw-r--   0 sovrin    (1003)     1004    18072 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/auth/metadata/test_auth_rule_with_metadata_composite.py
--rw-rw-r--   0 sovrin    (1003)     1004    17163 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/auth/metadata/test_auth_rule_with_metadata_simple.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/auth/metadata/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004    13228 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/auth/metadata/test_auth_rule_with_metadata_complex.py
--rw-rw-r--   0 sovrin    (1003)     1004     5845 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/auth/metadata/test_error_messages.py
--rw-rw-r--   0 sovrin    (1003)     1004     4305 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/auth/metadata/helper.py
--rw-rw-r--   0 sovrin    (1003)     1004      290 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/auth/test_helper.py
--rw-rw-r--   0 sovrin    (1003)     1004     3641 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/auth/test_composite_authorizer.py
--rw-rw-r--   0 sovrin    (1003)     1004      637 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/auth/test_auth_pool_restart_with_new_auth_map.py
--rw-rw-r--   0 sovrin    (1003)     1004    18387 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/auth/test_auth_nym_with_new_auth_map.py
--rw-rw-r--   0 sovrin    (1003)     1004     1280 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/auth/test_auth_claim_def_with_new_auth_map.py
--rw-rw-r--   0 sovrin    (1003)     1004     1787 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/auth/test_auth_actions.py
--rw-rw-r--   0 sovrin    (1003)     1004      732 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/auth/test_auth_pool_config_new_auth_map.py
--rw-rw-r--   0 sovrin    (1003)     1004      668 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/auth/test_txn_author_agreement_aml_with_new_auth_map.py
--rw-rw-r--   0 sovrin    (1003)     1004      698 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/test/auth/test_auth_validator_info_with_new_auth_map.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_common/authorize/
--rw-rw-r--   0 sovrin    (1003)     1004    13588 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/authorize/auth_map.py
--rw-rw-r--   0 sovrin    (1003)     1004    11703 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/authorize/authorizer.py
--rw-rw-r--   0 sovrin    (1003)     1004     4198 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/authorize/auth_request_validator.py
--rw-rw-r--   0 sovrin    (1003)     1004     3541 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/authorize/auth_cons_strategies.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/authorize/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004    10499 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/authorize/auth_constraints.py
--rw-rw-r--   0 sovrin    (1003)     1004      177 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/authorize/helper.py
--rw-rw-r--   0 sovrin    (1003)     1004     2483 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/authorize/auth_actions.py
--rw-rw-r--   0 sovrin    (1003)     1004     1193 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/transactions.py
--rw-rw-r--   0 sovrin    (1003)     1004     4203 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/constants.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_common/migration/
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/migration/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004     1437 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/migration/helper.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_common/state/
--rw-rw-r--   0 sovrin    (1003)     1004      263 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/state/state_constants.py
--rw-rw-r--   0 sovrin    (1003)     1004      203 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/state/config.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/state/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004    13879 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/state/domain.py
--rw-rw-r--   0 sovrin    (1003)     1004     1810 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/node_version.py
--rw-rw-r--   0 sovrin    (1003)     1004     3357 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/identity.py
--rw-rw-r--   0 sovrin    (1003)     1004      768 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/version.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_common/pool/
--rw-rw-r--   0 sovrin    (1003)     1004      172 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/pool/pool.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/pool/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004      451 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/init_util.py
--rw-rw-r--   0 sovrin    (1003)     1004     1329 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_common/config_util.py
--rw-rw-r--   0 sovrin    (1003)     1004    10590 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/README.md
--rw-r--r--   0 sovrin    (1003)     1004       38 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/setup.cfg
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/data/
--rw-rw-r--   0 sovrin    (1003)     1004   331264 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/data/nssm_original.exe
--rw-rw-r--   0 sovrin    (1003)     1004       74 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/data/node_control.conf
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/data/__init__.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/data/migrations/
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/data/migrations/deb/
--rw-rw-r--   0 sovrin    (1003)     1004     2263 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/data/migrations/deb/1_3_433_to_1_3_434.py
--rw-rw-r--   0 sovrin    (1003)     1004     8907 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/data/migrations/deb/helper_1_0_96_to_1_0_97.py
--rw-rw-r--   0 sovrin    (1003)     1004     6923 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/data/migrations/deb/1_3_396_to_1_3_397.py
--rw-rw-r--   0 sovrin    (1003)     1004     3143 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/data/migrations/deb/1_2_233_to_1_2_234.py
--rw-rw-r--   0 sovrin    (1003)     1004     8607 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/data/migrations/deb/disabled_1_0_97_to_1_0_96.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/data/migrations/deb/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004      397 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/data/migrations/deb/1_4_500_to_1_4_501.py
--rw-rw-r--   0 sovrin    (1003)     1004     1301 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/data/migrations/deb/1_1_150_to_1_1_151.py
--rw-rw-r--   0 sovrin    (1003)     1004      447 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/data/migrations/deb/1_2_273_to_1_2_274.py
--rw-rw-r--   0 sovrin    (1003)     1004      395 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/data/migrations/deb/1_6_703_to_1_6_704.py
--rwxrwxr-x   0 sovrin    (1003)     1004     2461 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/data/migrations/deb/1_9_1_to_1_9_2.py
--rw-rw-r--   0 sovrin    (1003)     1004      753 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/data/migrations/deb/1_0_96_to_1_0_97.py
--rw-rw-r--   0 sovrin    (1003)     1004    16402 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/data/migrations/deb/1_3_428_to_1_3_429.py
--rw-rw-r--   0 sovrin    (1003)     1004     7760 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/data/migrations/deb/1_2_188_to_1_2_189.py
--rw-rw-r--   0 sovrin    (1003)     1004     1681 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/data/migrations/README.md
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/data/migrations/__init__.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/tools/
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/tools/diagnostics/
--rwxrwxr-x   0 sovrin    (1003)     1004    39315 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/tools/diagnostics/nsdiff
--rwxrwxr-x   0 sovrin    (1003)     1004    16829 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/tools/diagnostics/nsreplay
--rwxrwxr-x   0 sovrin    (1003)     1004    27357 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/tools/diagnostics/nscapture
--rw-rw-r--   0 sovrin    (1003)     1004     3504 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/setup.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/server/
--rw-rw-r--   0 sovrin    (1003)     1004      365 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/config_helper.py
--rw-rw-r--   0 sovrin    (1003)     1004     1820 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/validator_info_tool.py
--rw-rw-r--   0 sovrin    (1003)     1004     3012 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/client_authn.py
--rw-rw-r--   0 sovrin    (1003)     1004     1802 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/upgrade_log.py
--rw-rw-r--   0 sovrin    (1003)     1004     9339 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/restarter.py
--rw-rw-r--   0 sovrin    (1003)     1004      912 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/restart_log.py
--rw-rw-r--   0 sovrin    (1003)     1004    11641 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/node.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004    10454 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/revocation_strategy.py
--rw-rw-r--   0 sovrin    (1003)     1004     1141 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/pool_config.py
--rw-rw-r--   0 sovrin    (1003)     1004      867 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/node_authn.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/config_req_handlers/
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/config_req_handlers/auth_rule/
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/config_req_handlers/auth_rule/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004     1942 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/config_req_handlers/auth_rule/auth_rules_handler.py
--rw-rw-r--   0 sovrin    (1003)     1004     2397 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/config_req_handlers/auth_rule/static_auth_rule_helper.py
--rw-rw-r--   0 sovrin    (1003)     1004     2291 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/config_req_handlers/auth_rule/abstract_auth_rule_handler.py
--rw-rw-r--   0 sovrin    (1003)     1004     1840 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/config_req_handlers/auth_rule/auth_rule_handler.py
--rw-rw-r--   0 sovrin    (1003)     1004      920 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/config_req_handlers/txn_author_agreement_handler.py
--rw-rw-r--   0 sovrin    (1003)     1004     1027 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/config_req_handlers/node_upgrade_handler.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/config_req_handlers/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004     4583 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/config_req_handlers/pool_upgrade_handler.py
--rw-rw-r--   0 sovrin    (1003)     1004     1774 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/config_req_handlers/pool_config_handler.py
--rw-rw-r--   0 sovrin    (1003)     1004      978 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/config_req_handlers/txn_author_agreement_aml_handler.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/action_req_handlers/
--rw-rw-r--   0 sovrin    (1003)     1004     2059 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/action_req_handlers/pool_restart_handler.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/action_req_handlers/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004     2494 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/action_req_handlers/validator_info_handler.py
--rw-rw-r--   0 sovrin    (1003)     1004      243 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/action_req_handlers/utils.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/read_req_handlers/
--rw-rw-r--   0 sovrin    (1003)     1004     2482 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/read_req_handlers/get_schema_handler.py
--rw-rw-r--   0 sovrin    (1003)     1004     3227 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/read_req_handlers/get_attribute_handler.py
--rw-rw-r--   0 sovrin    (1003)     1004     2290 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/read_req_handlers/get_claim_def_handler.py
--rw-rw-r--   0 sovrin    (1003)     1004     1685 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/read_req_handlers/get_nym_handler.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/read_req_handlers/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004     8596 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/read_req_handlers/get_revoc_reg_delta_handler.py
--rw-rw-r--   0 sovrin    (1003)     1004     1196 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/read_req_handlers/get_revoc_reg_def_handler.py
--rw-rw-r--   0 sovrin    (1003)     1004     2937 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/read_req_handlers/get_revoc_reg_handler.py
--rw-rw-r--   0 sovrin    (1003)     1004     4298 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/read_req_handlers/get_auth_rule_handler.py
--rw-rw-r--   0 sovrin    (1003)     1004     1274 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/config_batch_handler.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/__init__.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/domain_req_handlers/
--rw-rw-r--   0 sovrin    (1003)     1004     5918 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/domain_req_handlers/nym_handler.py
--rw-rw-r--   0 sovrin    (1003)     1004     9634 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/domain_req_handlers/attribute_handler.py
--rw-rw-r--   0 sovrin    (1003)     1004     3877 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/domain_req_handlers/schema_handler.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/domain_req_handlers/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004     1850 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/domain_req_handlers/idr_cache_nym_handler.py
--rw-rw-r--   0 sovrin    (1003)     1004     5685 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/domain_req_handlers/revoc_reg_def_handler.py
--rw-rw-r--   0 sovrin    (1003)     1004     6943 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/domain_req_handlers/revoc_reg_entry_handler.py
--rw-rw-r--   0 sovrin    (1003)     1004     5141 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/domain_req_handlers/claim_def_handler.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/pool_req_handlers/
--rw-rw-r--   0 sovrin    (1003)     1004     3724 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/pool_req_handlers/node_handler.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/pool_req_handlers/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004     1069 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/idr_cache_batch_handler.py
--rw-rw-r--   0 sovrin    (1003)     1004      462 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/request_handlers/utils.py
--rw-rw-r--   0 sovrin    (1003)     1004     5565 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/action_log.py
--rw-rw-r--   0 sovrin    (1003)     1004    20740 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/upgrader.py
--rw-rw-r--   0 sovrin    (1003)     1004    15060 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/node_bootstrap.py
--rw-rw-r--   0 sovrin    (1003)     1004     3785 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/node_maintainer.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/server/plugin/
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/server/plugin/__init__.py
--rw-r--r--   0 sovrin    (1003)     1004      137 2019-08-29 07:29:55.000000 indy-node-1.9.2.dev1069/indy_node/__manifest__.json
--rw-rw-r--   0 sovrin    (1003)     1004     3010 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004     2251 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/__metadata__.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/test/
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/test/txn_validation/
--rw-rw-r--   0 sovrin    (1003)     1004     1670 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/txn_validation/test_pool_upgrade_validation.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/txn_validation/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004    19952 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/txn_validation/test_send_attrib_validation.py
--rw-rw-r--   0 sovrin    (1003)     1004     4356 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/txn_validation/test_send_get_nym_validation.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/test/auth_rule/
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/
--rw-rw-r--   0 sovrin    (1003)     1004     3921 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/edit_auth_rules.py
--rw-rw-r--   0 sovrin    (1003)     1004     3130 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/restart.py
--rw-rw-r--   0 sovrin    (1003)     1004     3771 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/node_properties.py
--rw-rw-r--   0 sovrin    (1003)     1004     8654 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/revoc_reg_def.py
--rw-rw-r--   0 sovrin    (1003)     1004     3230 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/key_rotation.py
--rw-rw-r--   0 sovrin    (1003)     1004     3242 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/txn_author_agreement.py
--rw-rw-r--   0 sovrin    (1003)     1004     7781 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/revoc_reg_entry.py
--rw-rw-r--   0 sovrin    (1003)     1004    11863 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/test_auth_rule_using.py
--rw-rw-r--   0 sovrin    (1003)     1004     5111 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/upgrade.py
--rw-rw-r--   0 sovrin    (1003)     1004     4144 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/basic.py
--rw-rw-r--   0 sovrin    (1003)     1004     4248 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/add_roles.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004     7861 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/node_services.py
--rw-rw-r--   0 sovrin    (1003)     1004     3100 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/schema.py
--rw-rw-r--   0 sovrin    (1003)     1004     5690 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/claim_def.py
--rw-rw-r--   0 sovrin    (1003)     1004     2852 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/pool_config.py
--rw-rw-r--   0 sovrin    (1003)     1004     3365 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/txn_author_agreement_aml.py
--rw-rw-r--   0 sovrin    (1003)     1004    10935 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/edit_roles.py
--rw-rw-r--   0 sovrin    (1003)     1004     3219 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/validator_info.py
--rw-rw-r--   0 sovrin    (1003)     1004     3584 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/edit_attrib.py
--rw-rw-r--   0 sovrin    (1003)     1004     3892 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/add_attrib.py
--rw-rw-r--   0 sovrin    (1003)     1004     3328 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/edit_auth_rule.py
--rw-rw-r--   0 sovrin    (1003)     1004     2226 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/auth_rule/test_check_rule_for_add_action_changing.py
--rw-rw-r--   0 sovrin    (1003)     1004     1328 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/auth_rule/test_txn_with_different_signature_and_idr.py
--rw-rw-r--   0 sovrin    (1003)     1004     2220 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/auth_rule/test_check_rule_for_edit_action_changing.py
--rw-rw-r--   0 sovrin    (1003)     1004    11665 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/auth_rule/test_get_auth_rule.py
--rw-rw-r--   0 sovrin    (1003)     1004     7978 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/auth_rule/test_auth_rules_transaction.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/auth_rule/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004     3207 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/auth_rule/test_catching_up_auth_rule_txn.py
--rw-rw-r--   0 sovrin    (1003)     1004     6353 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/auth_rule/test_multisig_auth_rule.py
--rw-rw-r--   0 sovrin    (1003)     1004     7213 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/auth_rule/test_constraint_field.py
--rw-rw-r--   0 sovrin    (1003)     1004     7859 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/auth_rule/test_auth_rule_transaction.py
--rw-rw-r--   0 sovrin    (1003)     1004     2155 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/auth_rule/test_use_modified_rules_from_uncommitted.py
--rw-rw-r--   0 sovrin    (1003)     1004     6288 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/auth_rule/helper.py
--rw-rw-r--   0 sovrin    (1003)     1004     4470 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/auth_rule/test_auth_map.py
--rw-rw-r--   0 sovrin    (1003)     1004     4276 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/auth_rule/test_revert_auth_rule_changing.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/test/replay/
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/replay/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004     8776 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/replay/test_successive_batch_no_state_change.py
--rw-rw-r--   0 sovrin    (1003)     1004     2881 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/replay/test_state_regenerated_from_ledger.py
--rw-rw-r--   0 sovrin    (1003)     1004    16534 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/conftest.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/test/txn_author_agreement/
--rw-rw-r--   0 sovrin    (1003)     1004     3239 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/txn_author_agreement/test_node_taa.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/txn_author_agreement/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004     1178 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/txn_author_agreement/test_get_taa_aml.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/
--rw-rw-r--   0 sovrin    (1003)     1004      776 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_pool_upgrade_same_version.py
--rw-rw-r--   0 sovrin    (1003)     1004     1363 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_pool_upgrade_no_loop_reinstall_unsuccessful.py
--rw-rw-r--   0 sovrin    (1003)     1004     7723 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/conftest.py
--rw-rw-r--   0 sovrin    (1003)     1004     1544 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_upgrade_timeout.py
--rw-rw-r--   0 sovrin    (1003)     1004      989 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_pool_upgrade_same_version_reinstall.py
--rw-rw-r--   0 sovrin    (1003)     1004     1035 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_upgrade_pool_with_demoted_nodes.py
--rw-rw-r--   0 sovrin    (1003)     1004     5902 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_upgrader.py
--rw-rw-r--   0 sovrin    (1003)     1004      881 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_pool_upgrade_cancel.py
--rw-rw-r--   0 sovrin    (1003)     1004     2432 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_control_tool_performs_migrations.py
--rw-rw-r--   0 sovrin    (1003)     1004     2064 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_restart_log.py
--rw-rw-r--   0 sovrin    (1003)     1004     1450 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_handles_forced_upgrade_on_propagate.py
--rw-rw-r--   0 sovrin    (1003)     1004      748 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_schedules_upgrade_after_pool_ledger_update.py
--rw-rw-r--   0 sovrin    (1003)     1004     1979 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_does_not_reschedule_canceled_upgrade.py
--rw-rw-r--   0 sovrin    (1003)     1004     6869 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_migration_util.py
--rw-rw-r--   0 sovrin    (1003)     1004     1699 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_control_tool_processes_invalid_data.py
--rw-rw-r--   0 sovrin    (1003)     1004     2585 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_upgrade_unsuccessful.py
--rw-rw-r--   0 sovrin    (1003)     1004     1687 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_forced_upgrade_if_ordered_and_then_request_received.py
--rw-rw-r--   0 sovrin    (1003)     1004     1434 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_upgrade_rescheduled_view_change.py
--rw-rw-r--   0 sovrin    (1003)     1004     1339 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_schedules_upgrade_after_restart.py
--rw-rw-r--   0 sovrin    (1003)     1004     1409 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_pool_upgrade_no_loop_reinstall.py
--rw-rw-r--   0 sovrin    (1003)     1004     1292 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_handles_forced_upgrade_on_client_request.py
--rw-rw-r--   0 sovrin    (1003)     1004      464 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_pool_upgrade_force_scheduled_only_once.py
--rw-rw-r--   0 sovrin    (1003)     1004     1368 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_pool_upgrade_no_loop_unsuccessful.py
--rw-rw-r--   0 sovrin    (1003)     1004     3138 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_communication_with_control_service.py
--rw-rw-r--   0 sovrin    (1003)     1004      943 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_send_node_upgrade.py
--rw-rw-r--   0 sovrin    (1003)     1004     2445 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_pool_upgrade_reject.py
--rw-rw-r--   0 sovrin    (1003)     1004     1087 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_version_parsing.py
--rw-rw-r--   0 sovrin    (1003)     1004     2226 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_reschedules_upgrade_for_proper_datetime.py
--rw-rw-r--   0 sovrin    (1003)     1004     1362 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_forced_upgrade_no_consensus_on_single_node.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004       60 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_schedules_upgrade.py
--rw-rw-r--   0 sovrin    (1003)     1004     2729 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_control_tool_removes_backups.py
--rw-rw-r--   0 sovrin    (1003)     1004     1469 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_pool_upgrade_no_loop_force.py
--rw-rw-r--   0 sovrin    (1003)     1004     1309 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_control_tool_receives_messages.py
--rw-rw-r--   0 sovrin    (1003)     1004     1753 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_reschedule_upgrade_lower_version.py
--rw-rw-r--   0 sovrin    (1003)     1004     1346 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_pool_upgrade_no_loop.py
--rw-rw-r--   0 sovrin    (1003)     1004     3319 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_control_tool_resolves_dependencies.py
--rw-rw-r--   0 sovrin    (1003)     1004     1300 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_sustain_invalid_upgrade_txn.py
--rw-rw-r--   0 sovrin    (1003)     1004     3392 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_upgrade.py
--rw-rw-r--   0 sovrin    (1003)     1004       89 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_schedules_upgrade_exp_force_false.py
--rw-rw-r--   0 sovrin    (1003)     1004     2544 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_control_tool_restores_from_backups.py
--rw-rw-r--   0 sovrin    (1003)     1004     3965 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_pool_upgrade_through_catchup.py
--rw-rw-r--   0 sovrin    (1003)     1004     2491 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_get_deps_with_filter.py
--rw-rw-r--   0 sovrin    (1003)     1004     2053 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_broken_connection_control_tool.py
--rw-rw-r--   0 sovrin    (1003)     1004     1783 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_migration_tool.py
--rw-rw-r--   0 sovrin    (1003)     1004     8245 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_action_log.py
--rw-rw-r--   0 sovrin    (1003)     1004    12665 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/helper.py
--rw-rw-r--   0 sovrin    (1003)     1004     1819 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_control_tool_creates_backups.py
--rw-rw-r--   0 sovrin    (1003)     1004     3126 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_upgrade_log.py
--rw-rw-r--   0 sovrin    (1003)     1004     2680 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_forced_upgrade_if_request_received_after_propagate.py
--rw-rw-r--   0 sovrin    (1003)     1004     4278 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_control_tool_resolves_dep_top_level.py
--rw-rw-r--   0 sovrin    (1003)     1004       87 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_schedules_upgrade_exp_force_true.py
--rw-rw-r--   0 sovrin    (1003)     1004     1168 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_upgrade_in_progress.py
--rw-rw-r--   0 sovrin    (1003)     1004     1276 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_force_upgrade_process_in_view_change.py
--rw-rw-r--   0 sovrin    (1003)     1004      842 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_pool_upgrade_same_time_different_days.py
--rw-rw-r--   0 sovrin    (1003)     1004     1355 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_pool_upgrade_no_loop_force_unsuccessful.py
--rw-rw-r--   0 sovrin    (1003)     1004     1290 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_schedules_upgrade_for_proper_datetime.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/test/nym_txn/
--rw-rw-r--   0 sovrin    (1003)     1004      123 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/nym_txn/conftest.py
--rw-rw-r--   0 sovrin    (1003)     1004     3759 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/nym_txn/test_demote_network_monitor.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/nym_txn/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004    10184 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/nym_txn/test_nym_auth_rules.py
--rw-rw-r--   0 sovrin    (1003)     1004     3656 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/nym_txn/test_nym_blacklisting.py
--rw-rw-r--   0 sovrin    (1003)     1004    19171 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/nym_txn/test_send_nym_validation.py
--rw-rw-r--   0 sovrin    (1003)     1004     1389 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/nym_txn/test_nym_resend.py
--rw-rw-r--   0 sovrin    (1003)     1004      570 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/nym_txn/test_nym.py
--rw-rw-r--   0 sovrin    (1003)     1004     6523 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/nym_txn/test_create_did_without_endorser.py
--rw-rw-r--   0 sovrin    (1003)     1004     5687 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/nym_txn/test_nym_additional.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/test/catchup/
--rw-rw-r--   0 sovrin    (1003)     1004      685 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/catchup/conftest.py
--rw-rw-r--   0 sovrin    (1003)     1004     5956 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/catchup/test_requests_post_new_node_catchup.py
--rw-rw-r--   0 sovrin    (1003)     1004     1640 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/catchup/test_requests_post_multiple_new_nodes.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/catchup/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004     5826 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/catchup/test_batch_rejected_and_later_ordered_on_catchup.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/test/node_control_utils/
--rw-rw-r--   0 sovrin    (1003)     1004     5420 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/node_control_utils/test_debian_version.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/node_control_utils/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004     6740 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/node_control_utils/test_node_control_util.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/test/node_txn/
--rw-rw-r--   0 sovrin    (1003)     1004    30407 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/node_txn/test_send_node_validation.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/node_txn/__init__.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/test/view_change/
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/view_change/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004     6473 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/view_change/test_view_change_during_alternating_unstash.py
--rw-rw-r--   0 sovrin    (1003)     1004       86 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/__init__.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/test/request_propagates/
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/request_propagates/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004     3202 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/request_propagates/test_request_propagates.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/test/tools/
--rw-rw-r--   0 sovrin    (1003)     1004     4149 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/tools/test_nsreplay.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/tools/__init__.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/test/memory_debugging/
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/memory_debugging/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004     9772 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/memory_debugging/test_memory_debugging.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/test/did/
--rw-rw-r--   0 sovrin    (1003)     1004     2631 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/did/conftest.py
--rw-rw-r--   0 sovrin    (1003)     1004     1456 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/did/test_did_with_abbreviated_verkey.py
--rw-rw-r--   0 sovrin    (1003)     1004     1512 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/did/test_did_with_no_verkey.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/did/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004     1446 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/did/test_did_with_full_verkey.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/test/package/
--rw-rw-r--   0 sovrin    (1003)     1004     2345 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/package/test_metadata.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/package/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004       39 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/__main__.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/test/validator_info/
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/validator_info/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004     1486 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/validator_info/test_validator_info_command.py
--rw-rw-r--   0 sovrin    (1003)     1004     6733 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/validator_info/test_validator_info.py
--rw-rw-r--   0 sovrin    (1003)     1004     1183 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/validator_info/test_validator_info_handler.py
--rw-rw-r--   0 sovrin    (1003)     1004     1326 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/validator_info/helper.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/test/request_handlers/
--rw-rw-r--   0 sovrin    (1003)     1004     2465 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/request_handlers/conftest.py
--rw-rw-r--   0 sovrin    (1003)     1004     4529 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/request_handlers/test_nym_handler.py
--rw-rw-r--   0 sovrin    (1003)     1004     3080 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/request_handlers/test_attrib_handler.py
--rw-rw-r--   0 sovrin    (1003)     1004     2158 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/request_handlers/test_txn_author_agreement_aml_handler.py
--rw-rw-r--   0 sovrin    (1003)     1004     2172 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/request_handlers/test_revert_uncommitted_state.py
--rw-rw-r--   0 sovrin    (1003)     1004     7365 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/request_handlers/test_claim_def_handler.py
--rw-rw-r--   0 sovrin    (1003)     1004     4389 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/request_handlers/test_auth_rule_handler.py
--rw-rw-r--   0 sovrin    (1003)     1004     6300 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/request_handlers/test_pool_upgrade_handler.py
--rw-rw-r--   0 sovrin    (1003)     1004     3875 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/request_handlers/test_get_auth_rule_handler.py
--rw-rw-r--   0 sovrin    (1003)     1004     4847 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/request_handlers/test_update_state_config_req_handler.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/request_handlers/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004     2360 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/request_handlers/test_schema_handler.py
--rw-rw-r--   0 sovrin    (1003)     1004     4000 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/request_handlers/test_revoc_reg_def_handler.py
--rw-rw-r--   0 sovrin    (1003)     1004     6599 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/request_handlers/test_revoc_reg_entry_handler.py
--rw-rw-r--   0 sovrin    (1003)     1004     2844 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/request_handlers/test_txn_author_agreement_handler.py
--rw-rw-r--   0 sovrin    (1003)     1004     4451 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/request_handlers/test_auth_rules_handler.py
--rw-rw-r--   0 sovrin    (1003)     1004     1100 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/request_handlers/helper.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/test/claim_def/
--rw-rw-r--   0 sovrin    (1003)     1004     7206 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/claim_def/test_send_claim_def.py
--rw-rw-r--   0 sovrin    (1003)     1004     3081 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/claim_def/test_send_get_claim_def.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/claim_def/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004     2750 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/claim_def/test_claim_def_auth_rule.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/test/suspension/
--rw-rw-r--   0 sovrin    (1003)     1004     3957 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/suspension/test_suspension.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/suspension/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004     2612 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/suspension/test_node_suspension.py
--rw-rw-r--   0 sovrin    (1003)     1004     2132 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/suspension/test_nym_suspension.py
--rw-rw-r--   0 sovrin    (1003)     1004      360 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/suspension/helper.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/test/attrib_txn/
--rw-rw-r--   0 sovrin    (1003)     1004     5674 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/attrib_txn/test_send_get_attr.py
--rw-rw-r--   0 sovrin    (1003)     1004    19751 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/attrib_txn/test_nym_attrib.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/attrib_txn/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004     1551 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/attrib_txn/test_attrib_txn_digest.py
--rw-rw-r--   0 sovrin    (1003)     1004     1431 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/attrib_txn/test_n_minus_f_pool_processes_attrib.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/test/schema/
--rw-rw-r--   0 sovrin    (1003)     1004     2622 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/schema/test_send_schema.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/schema/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004     5768 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/schema/test_send_get_schema.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/test/pool_config/
--rw-rw-r--   0 sovrin    (1003)     1004      812 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/pool_config/conftest.py
--rw-rw-r--   0 sovrin    (1003)     1004     4150 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/pool_config/test_pool_config.py
--rw-rw-r--   0 sovrin    (1003)     1004     2220 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/pool_config/test_send_pool_config.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/pool_config/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004     2277 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/pool_config/test_send_pool_config_only_trustee.py
--rw-rw-r--   0 sovrin    (1003)     1004     1025 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/pool_config/helper.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/test/anon_creds/
--rw-rw-r--   0 sovrin    (1003)     1004     8019 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/anon_creds/test_state_proof_for_get_request.py
--rw-rw-r--   0 sovrin    (1003)     1004    16006 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/anon_creds/conftest.py
--rw-rw-r--   0 sovrin    (1003)     1004     5656 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/anon_creds/test_get_revoc_reg_delta_send_by_default.py
--rw-rw-r--   0 sovrin    (1003)     1004     1702 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/anon_creds/test_get_revoc_reg_delta_with_none_results.py
--rw-rw-r--   0 sovrin    (1003)     1004     6698 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/anon_creds/test_revoc_reg_entry_validation.py
--rw-rw-r--   0 sovrin    (1003)     1004     1323 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/anon_creds/test_integration_get_revoc_delta.py
--rw-rw-r--   0 sovrin    (1003)     1004     3711 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/anon_creds/test_get_revoc_reg_def_send.py
--rw-rw-r--   0 sovrin    (1003)     1004     4558 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/anon_creds/test_get_revoc_reg_delta_unit.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/anon_creds/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004     1307 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/anon_creds/test_get_revoc_reg_delta_validation.py
--rw-rw-r--   0 sovrin    (1003)     1004     1982 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/anon_creds/test_revoc_def_send.py
--rw-rw-r--   0 sovrin    (1003)     1004     2423 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/anon_creds/test_incorrect_revoc_reg_def.py
--rw-rw-r--   0 sovrin    (1003)     1004     4873 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/anon_creds/test_get_revoc_reg_delta_send_by_demand.py
--rw-rw-r--   0 sovrin    (1003)     1004     1300 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/anon_creds/test_revoc_def_validation.py
--rw-rw-r--   0 sovrin    (1003)     1004     1902 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/anon_creds/test_get_revoc_reg_send.py
--rw-rw-r--   0 sovrin    (1003)     1004     7036 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/anon_creds/helper.py
--rw-rw-r--   0 sovrin    (1003)     1004      932 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/anon_creds/test_get_revoc_reg_entry.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/test/endorser/
--rw-rw-r--   0 sovrin    (1003)     1004     8467 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/endorser/test_send_by_endorser.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/endorser/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004     1019 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/endorser/helper.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/test/persistence/
--rw-rw-r--   0 sovrin    (1003)     1004     2392 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/persistence/test_idr_cache_update_after_catchup.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/persistence/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004     1798 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/persistence/test_idr_cache.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/test/state_proof/
--rw-rw-r--   0 sovrin    (1003)     1004      986 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/state_proof/conftest.py
--rw-rw-r--   0 sovrin    (1003)     1004     1235 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/state_proof/test_asking_one_node.py
--rw-rw-r--   0 sovrin    (1003)     1004    13533 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/state_proof/test_state_proof_for_get_requests.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/state_proof/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004     1925 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/state_proof/helper.py
--rw-rw-r--   0 sovrin    (1003)     1004     3865 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/state_proof/test_state_proof_for_missing_data.py
--rw-rw-r--   0 sovrin    (1003)     1004    13048 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/state_proof/test_state_multi_proofs_for_get_requests.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/test/api/
--rw-rw-r--   0 sovrin    (1003)     1004      334 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/api/test_schema_reply.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/api/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004     1659 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/api/test_attrib_reply.py
--rw-rw-r--   0 sovrin    (1003)     1004      724 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/api/test_nym_reply.py
--rw-rw-r--   0 sovrin    (1003)     1004     1410 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/api/test_claim_def_reply.py
--rw-rw-r--   0 sovrin    (1003)     1004     5675 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/api/helper.py
--rw-rw-r--   0 sovrin    (1003)     1004    11131 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/helper.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/test/write_permission/
--rw-rw-r--   0 sovrin    (1003)     1004    15933 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/write_permission/test_revocation_write_permission.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/write_permission/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004     4279 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/write_permission/test_send_write_permission_no_client.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/test/pool_restart/
--rw-rw-r--   0 sovrin    (1003)     1004     1494 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/pool_restart/test_restart_on_inconsistency.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/pool_restart/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004      341 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/pool_restart/test_pool_restart_now_with_empty_datetime.py
--rw-rw-r--   0 sovrin    (1003)     1004     5379 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/pool_restart/test_pool_restart.py
--rw-rw-r--   0 sovrin    (1003)     1004     1703 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/pool_restart/test_fail_pool_restart.py
--rw-rw-r--   0 sovrin    (1003)     1004     3540 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/pool_restart/helper.py
--rw-rw-r--   0 sovrin    (1003)     1004     1818 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/pool_restart/test_pool_restarts_one_by_one.py
--rw-rw-r--   0 sovrin    (1003)     1004     1882 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/pool_restart/test_node_control_tool_for_restart.py
--rw-rw-r--   0 sovrin    (1003)     1004     1723 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/pool_restart/test_pool_restarts_one_by_one_with_restart_now.py
--rw-rw-r--   0 sovrin    (1003)     1004       97 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/test/waits.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/utils/
--rw-rw-r--   0 sovrin    (1003)     1004    13534 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/utils/node_control_utils.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/utils/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004     1972 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/utils/node_runner.py
--rw-rw-r--   0 sovrin    (1003)     1004    12183 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/utils/node_control_tool.py
--rw-rw-r--   0 sovrin    (1003)     1004     5050 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/utils/migration_tool.py
--rw-rw-r--   0 sovrin    (1003)     1004       23 2019-08-29 07:29:55.000000 indy-node-1.9.2.dev1069/indy_node/__version__.json
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/persistence/
--rw-rw-r--   0 sovrin    (1003)     1004     5961 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/persistence/idr_cache.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/persistence/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004      648 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/persistence/attribute_store.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node/general_config/
--rw-rw-r--   0 sovrin    (1003)     1004       92 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/general_config/general_config.py
--rw-rw-r--   0 sovrin    (1003)     1004      449 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/general_config/ubuntu_platform_config.py
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/general_config/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004       17 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/indy_node/general_config/windows_platform_config.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node.egg-info/
--rw-r--r--   0 sovrin    (1003)     1004       34 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node.egg-info/top_level.txt
--rw-r--r--   0 sovrin    (1003)     1004    23300 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node.egg-info/SOURCES.txt
--rw-r--r--   0 sovrin    (1003)     1004      161 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node.egg-info/requires.txt
--rw-r--r--   0 sovrin    (1003)     1004        1 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node.egg-info/dependency_links.txt
--rw-r--r--   0 sovrin    (1003)     1004      332 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/indy_node.egg-info/PKG-INFO
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/sample/
--rw-rw-r--   0 sovrin    (1003)     1004     1054 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/sample/thrift-loan-application.indy
--rw-rw-r--   0 sovrin    (1003)     1004      217 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/sample/acme-bob-connection-request.indy
--rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/sample/__init__.py
--rw-rw-r--   0 sovrin    (1003)     1004      256 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/sample/faber-request.indy
--rw-rw-r--   0 sovrin    (1003)     1004      171 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/sample/faber-bob-connection-request.indy
--rw-rw-r--   0 sovrin    (1003)     1004      214 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/sample/thrift-bob-connection-request.indy
--rw-rw-r--   0 sovrin    (1003)     1004      285 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/sample/acme-job-application-no-pr.indy
--rw-rw-r--   0 sovrin    (1003)     1004      627 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/sample/acme-job-application.indy
--rw-rw-r--   0 sovrin    (1003)     1004      387 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/post-setup.py
-drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/scripts/
--rwxrwxr-x   0 sovrin    (1003)     1004     2764 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/scripts/node_address_list
--rw-rw-r--   0 sovrin    (1003)     1004       56 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/scripts/restart_upgrade_agent.bat
--rwxrwxr-x   0 sovrin    (1003)     1004    10814 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/scripts/get_metrics
--rw-rw-r--   0 sovrin    (1003)     1004      111 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/scripts/restart_indy_node.bat
--rwxrwxr-x   0 sovrin    (1003)     1004      313 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/scripts/setup_indy_node_iptables
--rwxrwxr-x   0 sovrin    (1003)     1004     1202 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/scripts/init_indy_keys
--rwxrwxr-x   0 sovrin    (1003)     1004     6695 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/scripts/current_validators
--rw-rw-r--   0 sovrin    (1003)     1004      625 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/scripts/restart_indy_node_ubuntu1604.sh
--rwxrwxr-x   0 sovrin    (1003)     1004      853 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/scripts/generate_indy_pool_transactions
--rw-rw-r--   0 sovrin    (1003)     1004      151 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/scripts/delete_indy_node.bat
--rwxrwxr-x   0 sovrin    (1003)     1004      773 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/scripts/upgrade_indy_node_ubuntu1604.sh
--rw-rw-r--   0 sovrin    (1003)     1004     1744 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/scripts/install_indy_node.bat
--rw-rw-r--   0 sovrin    (1003)     1004      149 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/scripts/restart_sovrin_node_ubuntu1604.sh
--rwxrwxr-x   0 sovrin    (1003)     1004     1350 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/scripts/setup_iptables
--rw-rw-r--   0 sovrin    (1003)     1004      844 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/scripts/complete_rebranding_upgrade_ubuntu1604.sh
--rw-rw-r--   0 sovrin    (1003)     1004     1536 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/scripts/get_keys
--rwxrwxr-x   0 sovrin    (1003)     1004      593 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/scripts/start_indy_node
--rwxrwxr-x   0 sovrin    (1003)     1004     1126 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/scripts/init_bls_keys
--rwxrwxr-x   0 sovrin    (1003)     1004      773 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/scripts/upgrade_indy_node_ubuntu1604_test.sh
--rwxrwxr-x   0 sovrin    (1003)     1004     1005 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/scripts/create_dirs.sh
--rw-rw-r--   0 sovrin    (1003)     1004      692 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/scripts/start_node_control_tool
--rwxrwxr-x   0 sovrin    (1003)     1004    25341 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/scripts/validator-info-history
--rw-rw-r--   0 sovrin    (1003)     1004      458 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/scripts/upgrade_indy_node_test.bat
--rw-rw-r--   0 sovrin    (1003)     1004      453 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/scripts/install_nssm.bat
--rw-rw-r--   0 sovrin    (1003)     1004      356 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/scripts/upgrade_indy_node.bat
--rwxrwxr-x   0 sovrin    (1003)     1004    27623 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/scripts/validator-info
--rwxrwxr-x   0 sovrin    (1003)     1004      969 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/scripts/clear_node.py
--rw-rw-r--   0 sovrin    (1003)     1004     1979 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/scripts/generate_bls_proof_of_possession
--rwxrwxr-x   0 sovrin    (1003)     1004     6627 2019-08-29 07:29:50.000000 indy-node-1.9.2.dev1069/scripts/read_ledger
--rw-r--r--   0 sovrin    (1003)     1004      332 2019-08-29 07:29:56.000000 indy-node-1.9.2.dev1069/PKG-INFO
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/
+-rw-rw-r--   0 sovrin    (1003)     1004      145 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/MANIFEST.in
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_common/
+-rw-rw-r--   0 sovrin    (1003)     1004     1584 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/config_helper.py
+-rw-rw-r--   0 sovrin    (1003)     1004     2821 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/req_utils.py
+-rw-rw-r--   0 sovrin    (1003)     1004    17898 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/types.py
+-rw-rw-r--   0 sovrin    (1003)     1004     3082 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/strict_types.py
+-rw-rw-r--   0 sovrin    (1003)     1004      189 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/did_method.py
+-rw-rw-r--   0 sovrin    (1003)     1004     2168 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/setup_util.py
+-rw-rw-r--   0 sovrin    (1003)     1004      743 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/exceptions.py
+-rw-rw-r--   0 sovrin    (1003)     1004      821 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/txn_util.py
+-rw-rw-r--   0 sovrin    (1003)     1004      702 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/roles.py
+-rw-rw-r--   0 sovrin    (1003)     1004      328 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/generates_request.py
+-rw-rw-r--   0 sovrin    (1003)     1004      109 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/serialization.py
+-rw-rw-r--   0 sovrin    (1003)     1004     2835 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/config.py
+-rw-rw-r--   0 sovrin    (1003)     1004     4853 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/util.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004     4882 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/auth.py
+-rw-rw-r--   0 sovrin    (1003)     1004     2247 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/node_version_fallback.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_common/test/
+-rw-rw-r--   0 sovrin    (1003)     1004     3334 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/conftest.py
+-rw-rw-r--   0 sovrin    (1003)     1004     6149 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/test_transactions.py
+-rw-rw-r--   0 sovrin    (1003)     1004     5390 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/test_req_utils_claim_def.py
+-rw-rw-r--   0 sovrin    (1003)     1004      899 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/test_strict_schema.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_common/test/types/
+-rw-rw-r--   0 sovrin    (1003)     1004      838 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/types/test_claim_def_sub_schema.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1211 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/types/test_schema_schema.py
+-rw-rw-r--   0 sovrin    (1003)     1004      812 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/types/test_claim_def_get_schema.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1263 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/types/test_get_schema_schema.py
+-rw-rw-r--   0 sovrin    (1003)     1004      672 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/types/test_get_revoc_reg_delta_schema.py
+-rw-rw-r--   0 sovrin    (1003)     1004     2415 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/types/test_auth_rule_schema.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1730 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/types/test_revoc_def_submit_schema.py
+-rw-rw-r--   0 sovrin    (1003)     1004     8233 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/types/test_attrib.py
+-rw-rw-r--   0 sovrin    (1003)     1004      802 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/types/test_attrib_schema.py
+-rw-rw-r--   0 sovrin    (1003)     1004      758 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/types/test_discl_schema.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/types/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1137 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/types/test_pool_upg_schema.py
+-rw-rw-r--   0 sovrin    (1003)     1004      534 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/types/test_get_revoc_reg_def_schema.py
+-rw-rw-r--   0 sovrin    (1003)     1004      809 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/types/test_get_attrib_schema.py
+-rw-rw-r--   0 sovrin    (1003)     1004      688 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/types/test_pool_config_schema.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1666 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/types/test_revoc_def_entry_submit_schema.py
+-rw-rw-r--   0 sovrin    (1003)     1004      619 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/types/test_get_revoc_reg_entry_schema.py
+-rw-rw-r--   0 sovrin    (1003)     1004      651 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/types/test_get_nym_schema.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1032 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/types/test_get_auth_rule_schema.py
+-rw-rw-r--   0 sovrin    (1003)     1004       86 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/__init__.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_common/test/version/
+-rw-rw-r--   0 sovrin    (1003)     1004      849 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/version/test_version.py
+-rw-rw-r--   0 sovrin    (1003)     1004     3610 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/version/test_node_version_fallback.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1163 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/version/test_node_version.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/version/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004       41 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/__main__.py
+-rw-rw-r--   0 sovrin    (1003)     1004      948 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/constants.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1429 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/test_strict_types.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_common/test/state/
+-rw-rw-r--   0 sovrin    (1003)     1004     1603 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/state/test_state_path.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/state/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004     4112 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/test_req_utils_schema.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1661 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/helper.py
+-rw-rw-r--   0 sovrin    (1003)     1004      779 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/test_roles.py
+-rw-rw-r--   0 sovrin    (1003)     1004      405 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/test_util.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_common/test/auth/
+-rw-rw-r--   0 sovrin    (1003)     1004     8147 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/auth/test_auth_constraint.py
+-rw-rw-r--   0 sovrin    (1003)     1004    10385 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/auth/test_endorser_authorizer.py
+-rw-rw-r--   0 sovrin    (1003)     1004     2506 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/auth/conftest.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1295 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/auth/test_auth_rev_reg_def_with_new_auth_map.py
+-rw-rw-r--   0 sovrin    (1003)     1004      767 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/auth/test_auth_for_auth_rule_new_auth_map.py
+-rw-rw-r--   0 sovrin    (1003)     1004      905 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/auth/test_auth_anyone.py
+-rw-rw-r--   0 sovrin    (1003)     1004     3953 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/auth/test_auth_strategies.py
+-rw-rw-r--   0 sovrin    (1003)     1004     2993 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/auth/test_config_ledger_auth_strategy.py
+-rw-rw-r--   0 sovrin    (1003)     1004     7295 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/auth/test_auth_node_with_new_auth_map.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_common/test/auth/multi_sig/
+-rw-rw-r--   0 sovrin    (1003)     1004     1763 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/auth/multi_sig/conftest.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/auth/multi_sig/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1779 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/auth/multi_sig/test_auth_multi_sig_for_5_owners.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1228 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/auth/multi_sig/test_auth_multi_sig_for_1_owner.py
+-rw-rw-r--   0 sovrin    (1003)     1004      678 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/auth/test_auth_txn_author_agreement_with_new_auth_map.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/auth/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1178 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/auth/test_auth_schema_with_new_auth_map.py
+-rw-rw-r--   0 sovrin    (1003)     1004     8259 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/auth/test_role_authorizer.py
+-rw-rw-r--   0 sovrin    (1003)     1004     2291 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/auth/test_auth_pool_upgrade_with_new_auth_map.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_common/test/auth/metadata/
+-rw-rw-r--   0 sovrin    (1003)     1004     2201 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/auth/metadata/conftest.py
+-rw-rw-r--   0 sovrin    (1003)     1004    18072 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/auth/metadata/test_auth_rule_with_metadata_composite.py
+-rw-rw-r--   0 sovrin    (1003)     1004    17163 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/auth/metadata/test_auth_rule_with_metadata_simple.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/auth/metadata/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004    13228 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/auth/metadata/test_auth_rule_with_metadata_complex.py
+-rw-rw-r--   0 sovrin    (1003)     1004     5845 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/auth/metadata/test_error_messages.py
+-rw-rw-r--   0 sovrin    (1003)     1004     4305 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/auth/metadata/helper.py
+-rw-rw-r--   0 sovrin    (1003)     1004      290 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/auth/test_helper.py
+-rw-rw-r--   0 sovrin    (1003)     1004     3641 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/auth/test_composite_authorizer.py
+-rw-rw-r--   0 sovrin    (1003)     1004      637 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/auth/test_auth_pool_restart_with_new_auth_map.py
+-rw-rw-r--   0 sovrin    (1003)     1004    18387 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/auth/test_auth_nym_with_new_auth_map.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1280 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/auth/test_auth_claim_def_with_new_auth_map.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1787 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/auth/test_auth_actions.py
+-rw-rw-r--   0 sovrin    (1003)     1004      732 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/auth/test_auth_pool_config_new_auth_map.py
+-rw-rw-r--   0 sovrin    (1003)     1004      668 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/auth/test_txn_author_agreement_aml_with_new_auth_map.py
+-rw-rw-r--   0 sovrin    (1003)     1004      698 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/test/auth/test_auth_validator_info_with_new_auth_map.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_common/authorize/
+-rw-rw-r--   0 sovrin    (1003)     1004    13588 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/authorize/auth_map.py
+-rw-rw-r--   0 sovrin    (1003)     1004    11703 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/authorize/authorizer.py
+-rw-rw-r--   0 sovrin    (1003)     1004     4198 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/authorize/auth_request_validator.py
+-rw-rw-r--   0 sovrin    (1003)     1004     3541 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/authorize/auth_cons_strategies.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/authorize/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004    10499 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/authorize/auth_constraints.py
+-rw-rw-r--   0 sovrin    (1003)     1004      177 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/authorize/helper.py
+-rw-rw-r--   0 sovrin    (1003)     1004     2483 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/authorize/auth_actions.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1193 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/transactions.py
+-rw-rw-r--   0 sovrin    (1003)     1004     4203 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/constants.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_common/migration/
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/migration/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1437 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/migration/helper.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_common/state/
+-rw-rw-r--   0 sovrin    (1003)     1004      263 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/state/state_constants.py
+-rw-rw-r--   0 sovrin    (1003)     1004      203 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/state/config.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/state/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004    13879 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/state/domain.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1810 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/node_version.py
+-rw-rw-r--   0 sovrin    (1003)     1004     3357 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/identity.py
+-rw-rw-r--   0 sovrin    (1003)     1004      768 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/version.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_common/pool/
+-rw-rw-r--   0 sovrin    (1003)     1004      172 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/pool/pool.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/pool/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004      451 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/init_util.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1329 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_common/config_util.py
+-rw-rw-r--   0 sovrin    (1003)     1004    10590 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/README.md
+-rw-r--r--   0 sovrin    (1003)     1004       38 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/setup.cfg
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/data/
+-rw-rw-r--   0 sovrin    (1003)     1004   331264 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/data/nssm_original.exe
+-rw-rw-r--   0 sovrin    (1003)     1004       74 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/data/node_control.conf
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/data/__init__.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/data/migrations/
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/data/migrations/deb/
+-rw-rw-r--   0 sovrin    (1003)     1004     3143 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/data/migrations/deb/1_2_50_to_1_2_51.py
+-rw-rw-r--   0 sovrin    (1003)     1004     2263 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/data/migrations/deb/1_3_433_to_1_3_434.py
+-rw-rw-r--   0 sovrin    (1003)     1004     8907 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/data/migrations/deb/helper_1_0_28_to_1_0_29.py
+-rw-rw-r--   0 sovrin    (1003)     1004     6923 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/data/migrations/deb/1_3_396_to_1_3_397.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/data/migrations/deb/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004      397 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/data/migrations/deb/1_4_500_to_1_4_501.py
+-rw-rw-r--   0 sovrin    (1003)     1004      447 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/data/migrations/deb/1_2_51_to_1_2_52.py
+-rw-rw-r--   0 sovrin    (1003)     1004     7760 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/data/migrations/deb/1_2_44_to_1_2_45.py
+-rw-rw-r--   0 sovrin    (1003)     1004      395 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/data/migrations/deb/1_6_703_to_1_6_704.py
+-rw-rw-r--   0 sovrin    (1003)     1004      753 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/data/migrations/deb/1_0_28_to_1_0_29.py
+-rw-rw-r--   0 sovrin    (1003)     1004      757 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/data/migrations/deb/1_1_37_to_1_1_38.py
+-rw-rw-r--   0 sovrin    (1003)     1004     6952 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/data/migrations/deb/helper_1_1_37_to_1_1_38.py
+-rwxrwxr-x   0 sovrin    (1003)     1004     2461 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/data/migrations/deb/1_9_1_to_1_9_2.py
+-rw-rw-r--   0 sovrin    (1003)     1004    16402 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/data/migrations/deb/1_3_428_to_1_3_429.py
+-rw-rw-r--   0 sovrin    (1003)     1004     8607 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/data/migrations/deb/disabled_1_0_29_to_1_0_28.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1301 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/data/migrations/deb/1_1_43_to_1_2_44.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1681 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/data/migrations/README.md
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/data/migrations/__init__.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:58.000000 indy-node-1.9.2rc1/tools/
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/tools/diagnostics/
+-rwxrwxr-x   0 sovrin    (1003)     1004    39315 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/tools/diagnostics/nsdiff
+-rwxrwxr-x   0 sovrin    (1003)     1004    16829 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/tools/diagnostics/nsreplay
+-rwxrwxr-x   0 sovrin    (1003)     1004    27357 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/tools/diagnostics/nscapture
+-rw-rw-r--   0 sovrin    (1003)     1004     3497 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/setup.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/server/
+-rw-rw-r--   0 sovrin    (1003)     1004      365 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/config_helper.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1820 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/validator_info_tool.py
+-rw-rw-r--   0 sovrin    (1003)     1004     3012 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/client_authn.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1802 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/upgrade_log.py
+-rw-rw-r--   0 sovrin    (1003)     1004     9339 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/restarter.py
+-rw-rw-r--   0 sovrin    (1003)     1004      912 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/restart_log.py
+-rw-rw-r--   0 sovrin    (1003)     1004    11641 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/node.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004    10454 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/revocation_strategy.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1141 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/pool_config.py
+-rw-rw-r--   0 sovrin    (1003)     1004      867 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/node_authn.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/config_req_handlers/
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/config_req_handlers/auth_rule/
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/config_req_handlers/auth_rule/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1942 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/config_req_handlers/auth_rule/auth_rules_handler.py
+-rw-rw-r--   0 sovrin    (1003)     1004     2397 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/config_req_handlers/auth_rule/static_auth_rule_helper.py
+-rw-rw-r--   0 sovrin    (1003)     1004     2291 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/config_req_handlers/auth_rule/abstract_auth_rule_handler.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1840 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/config_req_handlers/auth_rule/auth_rule_handler.py
+-rw-rw-r--   0 sovrin    (1003)     1004      920 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/config_req_handlers/txn_author_agreement_handler.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1027 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/config_req_handlers/node_upgrade_handler.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/config_req_handlers/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004     4583 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/config_req_handlers/pool_upgrade_handler.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1774 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/config_req_handlers/pool_config_handler.py
+-rw-rw-r--   0 sovrin    (1003)     1004      978 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/config_req_handlers/txn_author_agreement_aml_handler.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/action_req_handlers/
+-rw-rw-r--   0 sovrin    (1003)     1004     2059 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/action_req_handlers/pool_restart_handler.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/action_req_handlers/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004     2494 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/action_req_handlers/validator_info_handler.py
+-rw-rw-r--   0 sovrin    (1003)     1004      243 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/action_req_handlers/utils.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/read_req_handlers/
+-rw-rw-r--   0 sovrin    (1003)     1004     2482 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/read_req_handlers/get_schema_handler.py
+-rw-rw-r--   0 sovrin    (1003)     1004     3227 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/read_req_handlers/get_attribute_handler.py
+-rw-rw-r--   0 sovrin    (1003)     1004     2290 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/read_req_handlers/get_claim_def_handler.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1685 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/read_req_handlers/get_nym_handler.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/read_req_handlers/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004     8596 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/read_req_handlers/get_revoc_reg_delta_handler.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1196 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/read_req_handlers/get_revoc_reg_def_handler.py
+-rw-rw-r--   0 sovrin    (1003)     1004     2937 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/read_req_handlers/get_revoc_reg_handler.py
+-rw-rw-r--   0 sovrin    (1003)     1004     4298 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/read_req_handlers/get_auth_rule_handler.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1274 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/config_batch_handler.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/__init__.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/domain_req_handlers/
+-rw-rw-r--   0 sovrin    (1003)     1004     5918 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/domain_req_handlers/nym_handler.py
+-rw-rw-r--   0 sovrin    (1003)     1004     9634 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/domain_req_handlers/attribute_handler.py
+-rw-rw-r--   0 sovrin    (1003)     1004     3877 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/domain_req_handlers/schema_handler.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/domain_req_handlers/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1850 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/domain_req_handlers/idr_cache_nym_handler.py
+-rw-rw-r--   0 sovrin    (1003)     1004     5685 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/domain_req_handlers/revoc_reg_def_handler.py
+-rw-rw-r--   0 sovrin    (1003)     1004     6943 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/domain_req_handlers/revoc_reg_entry_handler.py
+-rw-rw-r--   0 sovrin    (1003)     1004     5141 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/domain_req_handlers/claim_def_handler.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/pool_req_handlers/
+-rw-rw-r--   0 sovrin    (1003)     1004     3724 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/pool_req_handlers/node_handler.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/pool_req_handlers/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1069 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/idr_cache_batch_handler.py
+-rw-rw-r--   0 sovrin    (1003)     1004      462 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/request_handlers/utils.py
+-rw-rw-r--   0 sovrin    (1003)     1004     5565 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/action_log.py
+-rw-rw-r--   0 sovrin    (1003)     1004    20740 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/upgrader.py
+-rw-rw-r--   0 sovrin    (1003)     1004    15991 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/node_bootstrap.py
+-rw-rw-r--   0 sovrin    (1003)     1004     3785 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/node_maintainer.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/server/plugin/
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/server/plugin/__init__.py
+-rw-r--r--   0 sovrin    (1003)     1004      132 2019-08-29 11:08:58.000000 indy-node-1.9.2rc1/indy_node/__manifest__.json
+-rw-rw-r--   0 sovrin    (1003)     1004     3010 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004     2251 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/__metadata__.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/test/
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/test/txn_validation/
+-rw-rw-r--   0 sovrin    (1003)     1004     1670 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/txn_validation/test_pool_upgrade_validation.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/txn_validation/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004    19952 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/txn_validation/test_send_attrib_validation.py
+-rw-rw-r--   0 sovrin    (1003)     1004     4356 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/txn_validation/test_send_get_nym_validation.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/test/auth_rule/
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/
+-rw-rw-r--   0 sovrin    (1003)     1004     3921 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/edit_auth_rules.py
+-rw-rw-r--   0 sovrin    (1003)     1004     3130 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/restart.py
+-rw-rw-r--   0 sovrin    (1003)     1004     3771 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/node_properties.py
+-rw-rw-r--   0 sovrin    (1003)     1004     8654 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/revoc_reg_def.py
+-rw-rw-r--   0 sovrin    (1003)     1004     3230 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/key_rotation.py
+-rw-rw-r--   0 sovrin    (1003)     1004     3242 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/txn_author_agreement.py
+-rw-rw-r--   0 sovrin    (1003)     1004     7781 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/revoc_reg_entry.py
+-rw-rw-r--   0 sovrin    (1003)     1004    11863 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/test_auth_rule_using.py
+-rw-rw-r--   0 sovrin    (1003)     1004     5111 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/upgrade.py
+-rw-rw-r--   0 sovrin    (1003)     1004     4144 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/basic.py
+-rw-rw-r--   0 sovrin    (1003)     1004     4248 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/add_roles.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004     7861 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/node_services.py
+-rw-rw-r--   0 sovrin    (1003)     1004     3100 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/schema.py
+-rw-rw-r--   0 sovrin    (1003)     1004     5690 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/claim_def.py
+-rw-rw-r--   0 sovrin    (1003)     1004     2852 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/pool_config.py
+-rw-rw-r--   0 sovrin    (1003)     1004     3365 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/txn_author_agreement_aml.py
+-rw-rw-r--   0 sovrin    (1003)     1004    10935 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/edit_roles.py
+-rw-rw-r--   0 sovrin    (1003)     1004     3219 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/validator_info.py
+-rw-rw-r--   0 sovrin    (1003)     1004     3584 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/edit_attrib.py
+-rw-rw-r--   0 sovrin    (1003)     1004     3892 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/add_attrib.py
+-rw-rw-r--   0 sovrin    (1003)     1004     3328 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/edit_auth_rule.py
+-rw-rw-r--   0 sovrin    (1003)     1004     2226 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/auth_rule/test_check_rule_for_add_action_changing.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1328 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/auth_rule/test_txn_with_different_signature_and_idr.py
+-rw-rw-r--   0 sovrin    (1003)     1004     2220 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/auth_rule/test_check_rule_for_edit_action_changing.py
+-rw-rw-r--   0 sovrin    (1003)     1004    11665 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/auth_rule/test_get_auth_rule.py
+-rw-rw-r--   0 sovrin    (1003)     1004     7978 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/auth_rule/test_auth_rules_transaction.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/auth_rule/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004     3207 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/auth_rule/test_catching_up_auth_rule_txn.py
+-rw-rw-r--   0 sovrin    (1003)     1004     6353 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/auth_rule/test_multisig_auth_rule.py
+-rw-rw-r--   0 sovrin    (1003)     1004     7213 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/auth_rule/test_constraint_field.py
+-rw-rw-r--   0 sovrin    (1003)     1004     7859 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/auth_rule/test_auth_rule_transaction.py
+-rw-rw-r--   0 sovrin    (1003)     1004     2155 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/auth_rule/test_use_modified_rules_from_uncommitted.py
+-rw-rw-r--   0 sovrin    (1003)     1004     6288 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/auth_rule/helper.py
+-rw-rw-r--   0 sovrin    (1003)     1004     4470 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/auth_rule/test_auth_map.py
+-rw-rw-r--   0 sovrin    (1003)     1004     4276 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/auth_rule/test_revert_auth_rule_changing.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/test/replay/
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/replay/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004     8776 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/replay/test_successive_batch_no_state_change.py
+-rw-rw-r--   0 sovrin    (1003)     1004     2881 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/replay/test_state_regenerated_from_ledger.py
+-rw-rw-r--   0 sovrin    (1003)     1004    15867 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/conftest.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/test/txn_author_agreement/
+-rw-rw-r--   0 sovrin    (1003)     1004     3239 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/txn_author_agreement/test_node_taa.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/txn_author_agreement/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1178 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/txn_author_agreement/test_get_taa_aml.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/
+-rw-rw-r--   0 sovrin    (1003)     1004      776 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_pool_upgrade_same_version.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1363 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_pool_upgrade_no_loop_reinstall_unsuccessful.py
+-rw-rw-r--   0 sovrin    (1003)     1004     7723 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/conftest.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1544 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_upgrade_timeout.py
+-rw-rw-r--   0 sovrin    (1003)     1004      989 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_pool_upgrade_same_version_reinstall.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1035 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_upgrade_pool_with_demoted_nodes.py
+-rw-rw-r--   0 sovrin    (1003)     1004     5902 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_upgrader.py
+-rw-rw-r--   0 sovrin    (1003)     1004      881 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_pool_upgrade_cancel.py
+-rw-rw-r--   0 sovrin    (1003)     1004     2432 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_control_tool_performs_migrations.py
+-rw-rw-r--   0 sovrin    (1003)     1004     2064 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_restart_log.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1450 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_handles_forced_upgrade_on_propagate.py
+-rw-rw-r--   0 sovrin    (1003)     1004      748 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_schedules_upgrade_after_pool_ledger_update.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1979 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_does_not_reschedule_canceled_upgrade.py
+-rw-rw-r--   0 sovrin    (1003)     1004     6869 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_migration_util.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1699 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_control_tool_processes_invalid_data.py
+-rw-rw-r--   0 sovrin    (1003)     1004     2585 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_upgrade_unsuccessful.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1687 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_forced_upgrade_if_ordered_and_then_request_received.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1434 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_upgrade_rescheduled_view_change.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1339 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_schedules_upgrade_after_restart.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1409 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_pool_upgrade_no_loop_reinstall.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1292 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_handles_forced_upgrade_on_client_request.py
+-rw-rw-r--   0 sovrin    (1003)     1004      464 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_pool_upgrade_force_scheduled_only_once.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1368 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_pool_upgrade_no_loop_unsuccessful.py
+-rw-rw-r--   0 sovrin    (1003)     1004     3138 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_communication_with_control_service.py
+-rw-rw-r--   0 sovrin    (1003)     1004      943 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_send_node_upgrade.py
+-rw-rw-r--   0 sovrin    (1003)     1004     2445 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_pool_upgrade_reject.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1087 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_version_parsing.py
+-rw-rw-r--   0 sovrin    (1003)     1004     2226 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_reschedules_upgrade_for_proper_datetime.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1362 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_forced_upgrade_no_consensus_on_single_node.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004       60 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_schedules_upgrade.py
+-rw-rw-r--   0 sovrin    (1003)     1004     2729 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_control_tool_removes_backups.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1469 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_pool_upgrade_no_loop_force.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1309 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_control_tool_receives_messages.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1753 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_reschedule_upgrade_lower_version.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1346 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_pool_upgrade_no_loop.py
+-rw-rw-r--   0 sovrin    (1003)     1004     3319 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_control_tool_resolves_dependencies.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1300 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_sustain_invalid_upgrade_txn.py
+-rw-rw-r--   0 sovrin    (1003)     1004     3392 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_upgrade.py
+-rw-rw-r--   0 sovrin    (1003)     1004       89 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_schedules_upgrade_exp_force_false.py
+-rw-rw-r--   0 sovrin    (1003)     1004     2544 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_control_tool_restores_from_backups.py
+-rw-rw-r--   0 sovrin    (1003)     1004     3965 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_pool_upgrade_through_catchup.py
+-rw-rw-r--   0 sovrin    (1003)     1004     2491 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_get_deps_with_filter.py
+-rw-rw-r--   0 sovrin    (1003)     1004     2053 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_broken_connection_control_tool.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1783 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_migration_tool.py
+-rw-rw-r--   0 sovrin    (1003)     1004     8245 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_action_log.py
+-rw-rw-r--   0 sovrin    (1003)     1004    12665 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/helper.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1819 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_control_tool_creates_backups.py
+-rw-rw-r--   0 sovrin    (1003)     1004     3126 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_upgrade_log.py
+-rw-rw-r--   0 sovrin    (1003)     1004     2680 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_forced_upgrade_if_request_received_after_propagate.py
+-rw-rw-r--   0 sovrin    (1003)     1004     4278 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_control_tool_resolves_dep_top_level.py
+-rw-rw-r--   0 sovrin    (1003)     1004       87 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_schedules_upgrade_exp_force_true.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1168 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_upgrade_in_progress.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1262 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_force_upgrade_process_in_view_change.py
+-rw-rw-r--   0 sovrin    (1003)     1004      842 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_pool_upgrade_same_time_different_days.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1355 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_pool_upgrade_no_loop_force_unsuccessful.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1290 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_schedules_upgrade_for_proper_datetime.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/test/nym_txn/
+-rw-rw-r--   0 sovrin    (1003)     1004      123 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/nym_txn/conftest.py
+-rw-rw-r--   0 sovrin    (1003)     1004     3759 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/nym_txn/test_demote_network_monitor.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/nym_txn/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004    10184 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/nym_txn/test_nym_auth_rules.py
+-rw-rw-r--   0 sovrin    (1003)     1004     3656 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/nym_txn/test_nym_blacklisting.py
+-rw-rw-r--   0 sovrin    (1003)     1004    19171 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/nym_txn/test_send_nym_validation.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1389 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/nym_txn/test_nym_resend.py
+-rw-rw-r--   0 sovrin    (1003)     1004      570 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/nym_txn/test_nym.py
+-rw-rw-r--   0 sovrin    (1003)     1004     6523 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/nym_txn/test_create_did_without_endorser.py
+-rw-rw-r--   0 sovrin    (1003)     1004     5687 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/nym_txn/test_nym_additional.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/test/catchup/
+-rw-rw-r--   0 sovrin    (1003)     1004      685 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/catchup/conftest.py
+-rw-rw-r--   0 sovrin    (1003)     1004     5956 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/catchup/test_requests_post_new_node_catchup.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1640 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/catchup/test_requests_post_multiple_new_nodes.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/catchup/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004     5644 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/catchup/test_batch_rejected_and_later_ordered_on_catchup.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/test/node_control_utils/
+-rw-rw-r--   0 sovrin    (1003)     1004     5420 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/node_control_utils/test_debian_version.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/node_control_utils/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004     6740 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/node_control_utils/test_node_control_util.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/test/node_txn/
+-rw-rw-r--   0 sovrin    (1003)     1004    30407 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/node_txn/test_send_node_validation.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/node_txn/__init__.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/test/view_change/
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/view_change/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004     6473 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/view_change/test_view_change_during_alternating_unstash.py
+-rw-rw-r--   0 sovrin    (1003)     1004       86 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/__init__.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/test/request_propagates/
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/request_propagates/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004     3202 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/request_propagates/test_request_propagates.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/test/tools/
+-rw-rw-r--   0 sovrin    (1003)     1004     4065 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/tools/test_nsreplay.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/tools/__init__.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/test/memory_debugging/
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/memory_debugging/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004     9772 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/memory_debugging/test_memory_debugging.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/test/did/
+-rw-rw-r--   0 sovrin    (1003)     1004     2631 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/did/conftest.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1456 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/did/test_did_with_abbreviated_verkey.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1512 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/did/test_did_with_no_verkey.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/did/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1446 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/did/test_did_with_full_verkey.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/test/package/
+-rw-rw-r--   0 sovrin    (1003)     1004     2345 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/package/test_metadata.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/package/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004       39 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/__main__.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/test/validator_info/
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/validator_info/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1486 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/validator_info/test_validator_info_command.py
+-rw-rw-r--   0 sovrin    (1003)     1004     6719 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/validator_info/test_validator_info.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1183 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/validator_info/test_validator_info_handler.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1326 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/validator_info/helper.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/test/request_handlers/
+-rw-rw-r--   0 sovrin    (1003)     1004     2465 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/request_handlers/conftest.py
+-rw-rw-r--   0 sovrin    (1003)     1004     4529 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/request_handlers/test_nym_handler.py
+-rw-rw-r--   0 sovrin    (1003)     1004     3080 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/request_handlers/test_attrib_handler.py
+-rw-rw-r--   0 sovrin    (1003)     1004     2158 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/request_handlers/test_txn_author_agreement_aml_handler.py
+-rw-rw-r--   0 sovrin    (1003)     1004     2066 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/request_handlers/test_revert_uncommitted_state.py
+-rw-rw-r--   0 sovrin    (1003)     1004     7365 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/request_handlers/test_claim_def_handler.py
+-rw-rw-r--   0 sovrin    (1003)     1004     4389 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/request_handlers/test_auth_rule_handler.py
+-rw-rw-r--   0 sovrin    (1003)     1004     6300 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/request_handlers/test_pool_upgrade_handler.py
+-rw-rw-r--   0 sovrin    (1003)     1004     3875 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/request_handlers/test_get_auth_rule_handler.py
+-rw-rw-r--   0 sovrin    (1003)     1004     5357 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/request_handlers/test_update_state_config_req_handler.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/request_handlers/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004     2360 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/request_handlers/test_schema_handler.py
+-rw-rw-r--   0 sovrin    (1003)     1004     4000 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/request_handlers/test_revoc_reg_def_handler.py
+-rw-rw-r--   0 sovrin    (1003)     1004     6599 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/request_handlers/test_revoc_reg_entry_handler.py
+-rw-rw-r--   0 sovrin    (1003)     1004     2844 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/request_handlers/test_txn_author_agreement_handler.py
+-rw-rw-r--   0 sovrin    (1003)     1004     4451 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/request_handlers/test_auth_rules_handler.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1100 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/request_handlers/helper.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/test/claim_def/
+-rw-rw-r--   0 sovrin    (1003)     1004     7206 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/claim_def/test_send_claim_def.py
+-rw-rw-r--   0 sovrin    (1003)     1004     3081 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/claim_def/test_send_get_claim_def.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/claim_def/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004     2750 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/claim_def/test_claim_def_auth_rule.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/test/suspension/
+-rw-rw-r--   0 sovrin    (1003)     1004     3957 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/suspension/test_suspension.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/suspension/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004     2612 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/suspension/test_node_suspension.py
+-rw-rw-r--   0 sovrin    (1003)     1004     2132 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/suspension/test_nym_suspension.py
+-rw-rw-r--   0 sovrin    (1003)     1004      360 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/suspension/helper.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/test/attrib_txn/
+-rw-rw-r--   0 sovrin    (1003)     1004     5674 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/attrib_txn/test_send_get_attr.py
+-rw-rw-r--   0 sovrin    (1003)     1004    19751 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/attrib_txn/test_nym_attrib.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/attrib_txn/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1551 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/attrib_txn/test_attrib_txn_digest.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1431 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/attrib_txn/test_n_minus_f_pool_processes_attrib.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/test/schema/
+-rw-rw-r--   0 sovrin    (1003)     1004     2622 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/schema/test_send_schema.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/schema/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004     5768 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/schema/test_send_get_schema.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/test/pool_config/
+-rw-rw-r--   0 sovrin    (1003)     1004      812 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/pool_config/conftest.py
+-rw-rw-r--   0 sovrin    (1003)     1004     4150 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/pool_config/test_pool_config.py
+-rw-rw-r--   0 sovrin    (1003)     1004     2220 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/pool_config/test_send_pool_config.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/pool_config/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004     2277 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/pool_config/test_send_pool_config_only_trustee.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1025 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/pool_config/helper.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/test/anon_creds/
+-rw-rw-r--   0 sovrin    (1003)     1004     8019 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/anon_creds/test_state_proof_for_get_request.py
+-rw-rw-r--   0 sovrin    (1003)     1004    16006 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/anon_creds/conftest.py
+-rw-rw-r--   0 sovrin    (1003)     1004     5656 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/anon_creds/test_get_revoc_reg_delta_send_by_default.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1702 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/anon_creds/test_get_revoc_reg_delta_with_none_results.py
+-rw-rw-r--   0 sovrin    (1003)     1004     6698 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/anon_creds/test_revoc_reg_entry_validation.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1323 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/anon_creds/test_integration_get_revoc_delta.py
+-rw-rw-r--   0 sovrin    (1003)     1004     3711 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/anon_creds/test_get_revoc_reg_def_send.py
+-rw-rw-r--   0 sovrin    (1003)     1004     4558 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/anon_creds/test_get_revoc_reg_delta_unit.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/anon_creds/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1307 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/anon_creds/test_get_revoc_reg_delta_validation.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1982 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/anon_creds/test_revoc_def_send.py
+-rw-rw-r--   0 sovrin    (1003)     1004     2423 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/anon_creds/test_incorrect_revoc_reg_def.py
+-rw-rw-r--   0 sovrin    (1003)     1004     4873 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/anon_creds/test_get_revoc_reg_delta_send_by_demand.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1300 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/anon_creds/test_revoc_def_validation.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1902 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/anon_creds/test_get_revoc_reg_send.py
+-rw-rw-r--   0 sovrin    (1003)     1004     7036 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/anon_creds/helper.py
+-rw-rw-r--   0 sovrin    (1003)     1004      932 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/anon_creds/test_get_revoc_reg_entry.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/test/endorser/
+-rw-rw-r--   0 sovrin    (1003)     1004     8467 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/endorser/test_send_by_endorser.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/endorser/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1223 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/endorser/helper.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/test/persistence/
+-rw-rw-r--   0 sovrin    (1003)     1004     2392 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/persistence/test_idr_cache_update_after_catchup.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/persistence/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1798 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/persistence/test_idr_cache.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/test/state_proof/
+-rw-rw-r--   0 sovrin    (1003)     1004      986 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/state_proof/conftest.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1235 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/state_proof/test_asking_one_node.py
+-rw-rw-r--   0 sovrin    (1003)     1004    13533 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/state_proof/test_state_proof_for_get_requests.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/state_proof/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1925 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/state_proof/helper.py
+-rw-rw-r--   0 sovrin    (1003)     1004     3865 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/state_proof/test_state_proof_for_missing_data.py
+-rw-rw-r--   0 sovrin    (1003)     1004    13048 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/state_proof/test_state_multi_proofs_for_get_requests.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/test/api/
+-rw-rw-r--   0 sovrin    (1003)     1004      334 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/api/test_schema_reply.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/api/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1659 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/api/test_attrib_reply.py
+-rw-rw-r--   0 sovrin    (1003)     1004      724 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/api/test_nym_reply.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1410 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/api/test_claim_def_reply.py
+-rw-rw-r--   0 sovrin    (1003)     1004     5675 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/api/helper.py
+-rw-rw-r--   0 sovrin    (1003)     1004    11131 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/helper.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/test/write_permission/
+-rw-rw-r--   0 sovrin    (1003)     1004    15933 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/write_permission/test_revocation_write_permission.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/write_permission/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004     4279 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/write_permission/test_send_write_permission_no_client.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/test/pool_restart/
+-rw-rw-r--   0 sovrin    (1003)     1004     1494 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/pool_restart/test_restart_on_inconsistency.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/pool_restart/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004      341 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/pool_restart/test_pool_restart_now_with_empty_datetime.py
+-rw-rw-r--   0 sovrin    (1003)     1004     5379 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/pool_restart/test_pool_restart.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1703 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/pool_restart/test_fail_pool_restart.py
+-rw-rw-r--   0 sovrin    (1003)     1004     3540 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/pool_restart/helper.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1818 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/pool_restart/test_pool_restarts_one_by_one.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1882 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/pool_restart/test_node_control_tool_for_restart.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1723 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/pool_restart/test_pool_restarts_one_by_one_with_restart_now.py
+-rw-rw-r--   0 sovrin    (1003)     1004       97 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/test/waits.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/utils/
+-rw-rw-r--   0 sovrin    (1003)     1004    13534 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/utils/node_control_utils.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/utils/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1972 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/utils/node_runner.py
+-rw-rw-r--   0 sovrin    (1003)     1004    12183 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/utils/node_control_tool.py
+-rw-rw-r--   0 sovrin    (1003)     1004     5050 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/utils/migration_tool.py
+-rw-rw-r--   0 sovrin    (1003)     1004       19 2019-08-29 11:08:57.000000 indy-node-1.9.2rc1/indy_node/__version__.json
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/persistence/
+-rw-rw-r--   0 sovrin    (1003)     1004     5961 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/persistence/idr_cache.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/persistence/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004      648 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/persistence/attribute_store.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node/general_config/
+-rw-rw-r--   0 sovrin    (1003)     1004       92 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/general_config/general_config.py
+-rw-rw-r--   0 sovrin    (1003)     1004      449 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/general_config/ubuntu_platform_config.py
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/general_config/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004       17 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/indy_node/general_config/windows_platform_config.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/indy_node.egg-info/
+-rw-r--r--   0 sovrin    (1003)     1004       34 2019-08-29 11:08:58.000000 indy-node-1.9.2rc1/indy_node.egg-info/top_level.txt
+-rw-r--r--   0 sovrin    (1003)     1004    23379 2019-08-29 11:08:58.000000 indy-node-1.9.2rc1/indy_node.egg-info/SOURCES.txt
+-rw-r--r--   0 sovrin    (1003)     1004      154 2019-08-29 11:08:58.000000 indy-node-1.9.2rc1/indy_node.egg-info/requires.txt
+-rw-r--r--   0 sovrin    (1003)     1004        1 2019-08-29 11:08:58.000000 indy-node-1.9.2rc1/indy_node.egg-info/dependency_links.txt
+-rw-r--r--   0 sovrin    (1003)     1004      327 2019-08-29 11:08:58.000000 indy-node-1.9.2rc1/indy_node.egg-info/PKG-INFO
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/sample/
+-rw-rw-r--   0 sovrin    (1003)     1004     1054 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/sample/thrift-loan-application.indy
+-rw-rw-r--   0 sovrin    (1003)     1004      217 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/sample/acme-bob-connection-request.indy
+-rw-rw-r--   0 sovrin    (1003)     1004        0 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/sample/__init__.py
+-rw-rw-r--   0 sovrin    (1003)     1004      256 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/sample/faber-request.indy
+-rw-rw-r--   0 sovrin    (1003)     1004      171 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/sample/faber-bob-connection-request.indy
+-rw-rw-r--   0 sovrin    (1003)     1004      214 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/sample/thrift-bob-connection-request.indy
+-rw-rw-r--   0 sovrin    (1003)     1004      285 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/sample/acme-job-application-no-pr.indy
+-rw-rw-r--   0 sovrin    (1003)     1004      627 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/sample/acme-job-application.indy
+-rw-rw-r--   0 sovrin    (1003)     1004      387 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/post-setup.py
+drwxr-xr-x   0 sovrin    (1003)     1004        0 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/scripts/
+-rwxrwxr-x   0 sovrin    (1003)     1004     2764 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/scripts/node_address_list
+-rw-rw-r--   0 sovrin    (1003)     1004       56 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/scripts/restart_upgrade_agent.bat
+-rwxrwxr-x   0 sovrin    (1003)     1004    10814 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/scripts/get_metrics
+-rw-rw-r--   0 sovrin    (1003)     1004      111 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/scripts/restart_indy_node.bat
+-rwxrwxr-x   0 sovrin    (1003)     1004      313 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/scripts/setup_indy_node_iptables
+-rwxrwxr-x   0 sovrin    (1003)     1004     1202 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/scripts/init_indy_keys
+-rwxrwxr-x   0 sovrin    (1003)     1004     6695 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/scripts/current_validators
+-rw-rw-r--   0 sovrin    (1003)     1004      625 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/scripts/restart_indy_node_ubuntu1604.sh
+-rwxrwxr-x   0 sovrin    (1003)     1004      853 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/scripts/generate_indy_pool_transactions
+-rw-rw-r--   0 sovrin    (1003)     1004      151 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/scripts/delete_indy_node.bat
+-rwxrwxr-x   0 sovrin    (1003)     1004      773 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/scripts/upgrade_indy_node_ubuntu1604.sh
+-rw-rw-r--   0 sovrin    (1003)     1004     1744 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/scripts/install_indy_node.bat
+-rw-rw-r--   0 sovrin    (1003)     1004      149 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/scripts/restart_sovrin_node_ubuntu1604.sh
+-rwxrwxr-x   0 sovrin    (1003)     1004     1350 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/scripts/setup_iptables
+-rw-rw-r--   0 sovrin    (1003)     1004      844 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/scripts/complete_rebranding_upgrade_ubuntu1604.sh
+-rw-rw-r--   0 sovrin    (1003)     1004     1536 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/scripts/get_keys
+-rwxrwxr-x   0 sovrin    (1003)     1004      593 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/scripts/start_indy_node
+-rwxrwxr-x   0 sovrin    (1003)     1004     1126 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/scripts/init_bls_keys
+-rwxrwxr-x   0 sovrin    (1003)     1004      773 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/scripts/upgrade_indy_node_ubuntu1604_test.sh
+-rwxrwxr-x   0 sovrin    (1003)     1004     1005 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/scripts/create_dirs.sh
+-rw-rw-r--   0 sovrin    (1003)     1004      692 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/scripts/start_node_control_tool
+-rwxrwxr-x   0 sovrin    (1003)     1004    25341 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/scripts/validator-info-history
+-rw-rw-r--   0 sovrin    (1003)     1004      458 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/scripts/upgrade_indy_node_test.bat
+-rw-rw-r--   0 sovrin    (1003)     1004      453 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/scripts/install_nssm.bat
+-rw-rw-r--   0 sovrin    (1003)     1004      356 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/scripts/upgrade_indy_node.bat
+-rwxrwxr-x   0 sovrin    (1003)     1004    27623 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/scripts/validator-info
+-rwxrwxr-x   0 sovrin    (1003)     1004      969 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/scripts/clear_node.py
+-rw-rw-r--   0 sovrin    (1003)     1004     1979 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/scripts/generate_bls_proof_of_possession
+-rwxrwxr-x   0 sovrin    (1003)     1004     6627 2019-08-29 11:08:52.000000 indy-node-1.9.2rc1/scripts/read_ledger
+-rw-r--r--   0 sovrin    (1003)     1004      327 2019-08-29 11:08:59.000000 indy-node-1.9.2rc1/PKG-INFO
```

### Comparing `indy-node-1.9.2.dev1069/indy_common/config_helper.py` & `indy-node-1.9.2rc1/indy_common/config_helper.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/req_utils.py` & `indy-node-1.9.2rc1/indy_common/req_utils.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/types.py` & `indy-node-1.9.2rc1/indy_common/types.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/strict_types.py` & `indy-node-1.9.2rc1/indy_common/strict_types.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/setup_util.py` & `indy-node-1.9.2rc1/indy_common/setup_util.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/exceptions.py` & `indy-node-1.9.2rc1/indy_common/exceptions.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/txn_util.py` & `indy-node-1.9.2rc1/indy_common/txn_util.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/roles.py` & `indy-node-1.9.2rc1/indy_common/roles.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/config.py` & `indy-node-1.9.2rc1/indy_common/config.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/util.py` & `indy-node-1.9.2rc1/indy_common/util.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/auth.py` & `indy-node-1.9.2rc1/indy_common/auth.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/node_version_fallback.py` & `indy-node-1.9.2rc1/indy_common/node_version_fallback.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/conftest.py` & `indy-node-1.9.2rc1/indy_common/test/conftest.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/test_transactions.py` & `indy-node-1.9.2rc1/indy_common/test/test_transactions.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/test_req_utils_claim_def.py` & `indy-node-1.9.2rc1/indy_common/test/test_req_utils_claim_def.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/test_strict_schema.py` & `indy-node-1.9.2rc1/indy_common/test/test_strict_schema.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/types/test_claim_def_sub_schema.py` & `indy-node-1.9.2rc1/indy_common/test/types/test_claim_def_sub_schema.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/types/test_schema_schema.py` & `indy-node-1.9.2rc1/indy_common/test/types/test_schema_schema.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/types/test_claim_def_get_schema.py` & `indy-node-1.9.2rc1/indy_common/test/types/test_claim_def_get_schema.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/types/test_get_schema_schema.py` & `indy-node-1.9.2rc1/indy_common/test/types/test_get_schema_schema.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/types/test_get_revoc_reg_delta_schema.py` & `indy-node-1.9.2rc1/indy_common/test/types/test_get_revoc_reg_delta_schema.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/types/test_auth_rule_schema.py` & `indy-node-1.9.2rc1/indy_common/test/types/test_auth_rule_schema.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/types/test_revoc_def_submit_schema.py` & `indy-node-1.9.2rc1/indy_common/test/types/test_revoc_def_submit_schema.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/types/test_attrib.py` & `indy-node-1.9.2rc1/indy_common/test/types/test_attrib.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/types/test_attrib_schema.py` & `indy-node-1.9.2rc1/indy_common/test/types/test_attrib_schema.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/types/test_discl_schema.py` & `indy-node-1.9.2rc1/indy_common/test/types/test_discl_schema.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/types/test_pool_upg_schema.py` & `indy-node-1.9.2rc1/indy_common/test/types/test_pool_upg_schema.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/types/test_get_revoc_reg_def_schema.py` & `indy-node-1.9.2rc1/indy_common/test/types/test_get_revoc_reg_def_schema.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/types/test_get_attrib_schema.py` & `indy-node-1.9.2rc1/indy_common/test/types/test_get_attrib_schema.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/types/test_pool_config_schema.py` & `indy-node-1.9.2rc1/indy_common/test/types/test_pool_config_schema.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/types/test_revoc_def_entry_submit_schema.py` & `indy-node-1.9.2rc1/indy_common/test/types/test_revoc_def_entry_submit_schema.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/types/test_get_revoc_reg_entry_schema.py` & `indy-node-1.9.2rc1/indy_common/test/types/test_get_revoc_reg_entry_schema.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/types/test_get_nym_schema.py` & `indy-node-1.9.2rc1/indy_common/test/types/test_get_nym_schema.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/types/test_get_auth_rule_schema.py` & `indy-node-1.9.2rc1/indy_common/test/types/test_get_auth_rule_schema.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/version/test_version.py` & `indy-node-1.9.2rc1/indy_common/test/version/test_version.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/version/test_node_version_fallback.py` & `indy-node-1.9.2rc1/indy_common/test/version/test_node_version_fallback.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/version/test_node_version.py` & `indy-node-1.9.2rc1/indy_common/test/version/test_node_version.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/constants.py` & `indy-node-1.9.2rc1/indy_common/test/constants.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/test_strict_types.py` & `indy-node-1.9.2rc1/indy_common/test/test_strict_types.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/state/test_state_path.py` & `indy-node-1.9.2rc1/indy_common/test/state/test_state_path.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/test_req_utils_schema.py` & `indy-node-1.9.2rc1/indy_common/test/test_req_utils_schema.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/helper.py` & `indy-node-1.9.2rc1/indy_common/test/helper.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/test_roles.py` & `indy-node-1.9.2rc1/indy_common/test/test_roles.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/auth/test_auth_constraint.py` & `indy-node-1.9.2rc1/indy_common/test/auth/test_auth_constraint.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/auth/test_endorser_authorizer.py` & `indy-node-1.9.2rc1/indy_common/test/auth/test_endorser_authorizer.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/auth/conftest.py` & `indy-node-1.9.2rc1/indy_common/test/auth/conftest.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/auth/test_auth_rev_reg_def_with_new_auth_map.py` & `indy-node-1.9.2rc1/indy_common/test/auth/test_auth_rev_reg_def_with_new_auth_map.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/auth/test_auth_for_auth_rule_new_auth_map.py` & `indy-node-1.9.2rc1/indy_common/test/auth/test_auth_for_auth_rule_new_auth_map.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/auth/test_auth_anyone.py` & `indy-node-1.9.2rc1/indy_common/test/auth/test_auth_anyone.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/auth/test_auth_strategies.py` & `indy-node-1.9.2rc1/indy_common/test/auth/test_auth_strategies.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/auth/test_config_ledger_auth_strategy.py` & `indy-node-1.9.2rc1/indy_common/test/auth/test_config_ledger_auth_strategy.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/auth/test_auth_node_with_new_auth_map.py` & `indy-node-1.9.2rc1/indy_common/test/auth/test_auth_node_with_new_auth_map.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/auth/multi_sig/conftest.py` & `indy-node-1.9.2rc1/indy_common/test/auth/multi_sig/conftest.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/auth/multi_sig/test_auth_multi_sig_for_5_owners.py` & `indy-node-1.9.2rc1/indy_common/test/auth/multi_sig/test_auth_multi_sig_for_5_owners.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/auth/multi_sig/test_auth_multi_sig_for_1_owner.py` & `indy-node-1.9.2rc1/indy_common/test/auth/multi_sig/test_auth_multi_sig_for_1_owner.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/auth/test_auth_txn_author_agreement_with_new_auth_map.py` & `indy-node-1.9.2rc1/indy_common/test/auth/test_auth_txn_author_agreement_with_new_auth_map.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/auth/test_auth_schema_with_new_auth_map.py` & `indy-node-1.9.2rc1/indy_common/test/auth/test_auth_schema_with_new_auth_map.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/auth/test_role_authorizer.py` & `indy-node-1.9.2rc1/indy_common/test/auth/test_role_authorizer.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/auth/test_auth_pool_upgrade_with_new_auth_map.py` & `indy-node-1.9.2rc1/indy_common/test/auth/test_auth_pool_upgrade_with_new_auth_map.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/auth/metadata/conftest.py` & `indy-node-1.9.2rc1/indy_common/test/auth/metadata/conftest.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/auth/metadata/test_auth_rule_with_metadata_composite.py` & `indy-node-1.9.2rc1/indy_common/test/auth/metadata/test_auth_rule_with_metadata_composite.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/auth/metadata/test_auth_rule_with_metadata_simple.py` & `indy-node-1.9.2rc1/indy_common/test/auth/metadata/test_auth_rule_with_metadata_simple.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/auth/metadata/test_auth_rule_with_metadata_complex.py` & `indy-node-1.9.2rc1/indy_common/test/auth/metadata/test_auth_rule_with_metadata_complex.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/auth/metadata/test_error_messages.py` & `indy-node-1.9.2rc1/indy_common/test/auth/metadata/test_error_messages.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/auth/metadata/helper.py` & `indy-node-1.9.2rc1/indy_common/test/auth/metadata/helper.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/auth/test_composite_authorizer.py` & `indy-node-1.9.2rc1/indy_common/test/auth/test_composite_authorizer.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/auth/test_auth_pool_restart_with_new_auth_map.py` & `indy-node-1.9.2rc1/indy_common/test/auth/test_auth_pool_restart_with_new_auth_map.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/auth/test_auth_nym_with_new_auth_map.py` & `indy-node-1.9.2rc1/indy_common/test/auth/test_auth_nym_with_new_auth_map.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/auth/test_auth_claim_def_with_new_auth_map.py` & `indy-node-1.9.2rc1/indy_common/test/auth/test_auth_claim_def_with_new_auth_map.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/auth/test_auth_actions.py` & `indy-node-1.9.2rc1/indy_common/test/auth/test_auth_actions.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/auth/test_auth_pool_config_new_auth_map.py` & `indy-node-1.9.2rc1/indy_common/test/auth/test_auth_pool_config_new_auth_map.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/auth/test_txn_author_agreement_aml_with_new_auth_map.py` & `indy-node-1.9.2rc1/indy_common/test/auth/test_txn_author_agreement_aml_with_new_auth_map.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/test/auth/test_auth_validator_info_with_new_auth_map.py` & `indy-node-1.9.2rc1/indy_common/test/auth/test_auth_validator_info_with_new_auth_map.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/authorize/auth_map.py` & `indy-node-1.9.2rc1/indy_common/authorize/auth_map.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/authorize/authorizer.py` & `indy-node-1.9.2rc1/indy_common/authorize/authorizer.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/authorize/auth_request_validator.py` & `indy-node-1.9.2rc1/indy_common/authorize/auth_request_validator.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/authorize/auth_cons_strategies.py` & `indy-node-1.9.2rc1/indy_common/authorize/auth_cons_strategies.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/authorize/auth_constraints.py` & `indy-node-1.9.2rc1/indy_common/authorize/auth_constraints.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/authorize/auth_actions.py` & `indy-node-1.9.2rc1/indy_common/authorize/auth_actions.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/transactions.py` & `indy-node-1.9.2rc1/indy_common/transactions.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/constants.py` & `indy-node-1.9.2rc1/indy_common/constants.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/migration/helper.py` & `indy-node-1.9.2rc1/indy_common/migration/helper.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/state/domain.py` & `indy-node-1.9.2rc1/indy_common/state/domain.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/node_version.py` & `indy-node-1.9.2rc1/indy_common/node_version.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/identity.py` & `indy-node-1.9.2rc1/indy_common/identity.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/version.py` & `indy-node-1.9.2rc1/indy_common/version.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_common/config_util.py` & `indy-node-1.9.2rc1/indy_common/config_util.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/README.md` & `indy-node-1.9.2rc1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -55,29 +55,29 @@
     - [indy-plenum](https://github.com/hyperledger/indy-plenum)-based implementation of distributed ledger
     - Extends plenum's base pool functionality with specific transactions support (CLAIM_DEF, SCHEMA, POOL_UPGRADE, etc.)
 - indy-common
     - Common code for indy-node
 - scripts
     - Some scripts that can be run for installed Node (in particular, scripts to start Nodes, generate keys, prepare test Network, etc.)
 - doc
-    - A folder with documentation
+    - a folder with documentation
 - dev-setup
-    - A folder with scripts helping to configure development environment (python, dependencies, projects, virtual environment)
+    - a folder with scripts helping to configure development environment (python, dependencies, projects, virtual environment)
 
 ## Dependent Projects
 
 - [indy-plenum](https://github.com/hyperledger/indy-plenum)
     - The heart of the distributed ledger technology inside Hyperledger Indy.
     - Most probably you will need to make changes in Plenum if you want to contribute to Indy.
       So, if you want to work with Indy Node, you will need to have the Plenum code as well in most of the cases
       and work with two projects at the same time
       (see [How to Start Working with the Code](#how-to-start-working-with-the-code) below).
 - [indy-sdk](https://github.com/hyperledger/indy-sdk)
     - An official SDK for Indy.
-    - It contains client and anoncreds implementation
+    - it contains client and anoncreds implementation
     - You don't need it to contribute to Indy-Node. But please use indy-sdk for your own applications dealing with Indy ecosystem.
 - [indy-crypto](https://github.com/hyperledger/indy-crypto)
     - A shared crypto library
     - It's based on [AMCL](https://github.com/milagro-crypto/amcl)
     - In particular, it contains BLS multi-signature crypto needed for state proofs support in Indy.
 
 ## Contact us
```

### Comparing `indy-node-1.9.2.dev1069/data/nssm_original.exe` & `indy-node-1.9.2rc1/data/nssm_original.exe`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/data/migrations/deb/1_3_433_to_1_3_434.py` & `indy-node-1.9.2rc1/data/migrations/deb/1_3_433_to_1_3_434.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/data/migrations/deb/helper_1_0_96_to_1_0_97.py` & `indy-node-1.9.2rc1/data/migrations/deb/helper_1_0_28_to_1_0_29.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/data/migrations/deb/1_3_396_to_1_3_397.py` & `indy-node-1.9.2rc1/data/migrations/deb/1_3_396_to_1_3_397.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/data/migrations/deb/1_2_233_to_1_2_234.py` & `indy-node-1.9.2rc1/data/migrations/deb/1_2_50_to_1_2_51.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/data/migrations/deb/disabled_1_0_97_to_1_0_96.py` & `indy-node-1.9.2rc1/data/migrations/deb/disabled_1_0_29_to_1_0_28.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/data/migrations/deb/1_1_150_to_1_1_151.py` & `indy-node-1.9.2rc1/data/migrations/deb/1_1_43_to_1_2_44.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/data/migrations/deb/1_9_1_to_1_9_2.py` & `indy-node-1.9.2rc1/data/migrations/deb/1_9_1_to_1_9_2.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/data/migrations/deb/1_0_96_to_1_0_97.py` & `indy-node-1.9.2rc1/data/migrations/deb/1_0_28_to_1_0_29.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 logger = getlogger()
 
 migration_script_path = \
     os.path.normpath(
         os.path.join(
             os.path.dirname(os.path.abspath(__file__)),
-            'helper_1_0_96_to_1_0_97.py'))
+            'helper_1_0_28_to_1_0_29.py'))
 
 logger.info('script path {}'.format(migration_script_path))
 ret = subprocess.run(
     compose_cmd(
         ["su -c 'python3 {}' sovrin".format(migration_script_path)]
     ),
     shell=True,
```

### Comparing `indy-node-1.9.2.dev1069/data/migrations/deb/1_3_428_to_1_3_429.py` & `indy-node-1.9.2rc1/data/migrations/deb/1_3_428_to_1_3_429.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/data/migrations/deb/1_2_188_to_1_2_189.py` & `indy-node-1.9.2rc1/data/migrations/deb/1_2_44_to_1_2_45.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/data/migrations/README.md` & `indy-node-1.9.2rc1/data/migrations/README.md`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/tools/diagnostics/nsdiff` & `indy-node-1.9.2rc1/tools/diagnostics/nsdiff`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/tools/diagnostics/nsreplay` & `indy-node-1.9.2rc1/tools/diagnostics/nsreplay`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/tools/diagnostics/nscapture` & `indy-node-1.9.2rc1/tools/diagnostics/nscapture`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/setup.py` & `indy-node-1.9.2rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     package_data={
         '': ['*.txt', '*.md', '*.rst', '*.json', '*.conf', '*.html',
              '*.css', '*.ico', '*.png', 'LICENSE', 'LEGAL', '*.indy']},
     include_package_data=True,
     data_files=[(
         (BASE_DIR, ['data/nssm_original.exe'])
     )],
-    install_requires=['indy-plenum==1.9.2.dev876',
+    install_requires=['indy-plenum==1.9.2',
                       'timeout-decorator==0.4.0',
                       'distro==1.3.0'],
     setup_requires=['pytest-runner'],
     extras_require={
         'tests': tests_require
     },
     tests_require=tests_require,
```

### Comparing `indy-node-1.9.2.dev1069/indy_node/server/validator_info_tool.py` & `indy-node-1.9.2rc1/indy_node/server/validator_info_tool.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/server/client_authn.py` & `indy-node-1.9.2rc1/indy_node/server/client_authn.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/server/upgrade_log.py` & `indy-node-1.9.2rc1/indy_node/server/upgrade_log.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/server/restarter.py` & `indy-node-1.9.2rc1/indy_node/server/restarter.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/server/restart_log.py` & `indy-node-1.9.2rc1/indy_node/server/restart_log.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/server/node.py` & `indy-node-1.9.2rc1/indy_node/server/node.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/server/revocation_strategy.py` & `indy-node-1.9.2rc1/indy_node/server/revocation_strategy.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/server/pool_config.py` & `indy-node-1.9.2rc1/indy_node/server/pool_config.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/server/node_authn.py` & `indy-node-1.9.2rc1/indy_node/server/node_authn.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/server/request_handlers/config_req_handlers/auth_rule/auth_rules_handler.py` & `indy-node-1.9.2rc1/indy_node/server/request_handlers/config_req_handlers/auth_rule/auth_rules_handler.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/server/request_handlers/config_req_handlers/auth_rule/static_auth_rule_helper.py` & `indy-node-1.9.2rc1/indy_node/server/request_handlers/config_req_handlers/auth_rule/static_auth_rule_helper.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/server/request_handlers/config_req_handlers/auth_rule/abstract_auth_rule_handler.py` & `indy-node-1.9.2rc1/indy_node/server/request_handlers/config_req_handlers/auth_rule/abstract_auth_rule_handler.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/server/request_handlers/config_req_handlers/auth_rule/auth_rule_handler.py` & `indy-node-1.9.2rc1/indy_node/server/request_handlers/config_req_handlers/auth_rule/auth_rule_handler.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/server/request_handlers/config_req_handlers/txn_author_agreement_handler.py` & `indy-node-1.9.2rc1/indy_node/server/request_handlers/config_req_handlers/txn_author_agreement_handler.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/server/request_handlers/config_req_handlers/node_upgrade_handler.py` & `indy-node-1.9.2rc1/indy_node/server/request_handlers/config_req_handlers/node_upgrade_handler.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/server/request_handlers/config_req_handlers/pool_upgrade_handler.py` & `indy-node-1.9.2rc1/indy_node/server/request_handlers/config_req_handlers/pool_upgrade_handler.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/server/request_handlers/config_req_handlers/pool_config_handler.py` & `indy-node-1.9.2rc1/indy_node/server/request_handlers/config_req_handlers/pool_config_handler.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/server/request_handlers/config_req_handlers/txn_author_agreement_aml_handler.py` & `indy-node-1.9.2rc1/indy_node/server/request_handlers/config_req_handlers/txn_author_agreement_aml_handler.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/server/request_handlers/action_req_handlers/pool_restart_handler.py` & `indy-node-1.9.2rc1/indy_node/server/request_handlers/action_req_handlers/pool_restart_handler.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/server/request_handlers/action_req_handlers/validator_info_handler.py` & `indy-node-1.9.2rc1/indy_node/server/request_handlers/action_req_handlers/validator_info_handler.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/server/request_handlers/read_req_handlers/get_schema_handler.py` & `indy-node-1.9.2rc1/indy_node/server/request_handlers/read_req_handlers/get_schema_handler.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/server/request_handlers/read_req_handlers/get_attribute_handler.py` & `indy-node-1.9.2rc1/indy_node/server/request_handlers/read_req_handlers/get_attribute_handler.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/server/request_handlers/read_req_handlers/get_claim_def_handler.py` & `indy-node-1.9.2rc1/indy_node/server/request_handlers/read_req_handlers/get_claim_def_handler.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/server/request_handlers/read_req_handlers/get_nym_handler.py` & `indy-node-1.9.2rc1/indy_node/server/request_handlers/read_req_handlers/get_nym_handler.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/server/request_handlers/read_req_handlers/get_revoc_reg_delta_handler.py` & `indy-node-1.9.2rc1/indy_node/server/request_handlers/read_req_handlers/get_revoc_reg_delta_handler.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/server/request_handlers/read_req_handlers/get_revoc_reg_def_handler.py` & `indy-node-1.9.2rc1/indy_node/server/request_handlers/read_req_handlers/get_revoc_reg_def_handler.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/server/request_handlers/read_req_handlers/get_revoc_reg_handler.py` & `indy-node-1.9.2rc1/indy_node/server/request_handlers/read_req_handlers/get_revoc_reg_handler.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/server/request_handlers/read_req_handlers/get_auth_rule_handler.py` & `indy-node-1.9.2rc1/indy_node/server/request_handlers/read_req_handlers/get_auth_rule_handler.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/server/request_handlers/config_batch_handler.py` & `indy-node-1.9.2rc1/indy_node/server/request_handlers/config_batch_handler.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/server/request_handlers/domain_req_handlers/nym_handler.py` & `indy-node-1.9.2rc1/indy_node/server/request_handlers/domain_req_handlers/nym_handler.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/server/request_handlers/domain_req_handlers/attribute_handler.py` & `indy-node-1.9.2rc1/indy_node/server/request_handlers/domain_req_handlers/attribute_handler.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/server/request_handlers/domain_req_handlers/schema_handler.py` & `indy-node-1.9.2rc1/indy_node/server/request_handlers/domain_req_handlers/schema_handler.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/server/request_handlers/domain_req_handlers/idr_cache_nym_handler.py` & `indy-node-1.9.2rc1/indy_node/server/request_handlers/domain_req_handlers/idr_cache_nym_handler.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/server/request_handlers/domain_req_handlers/revoc_reg_def_handler.py` & `indy-node-1.9.2rc1/indy_node/server/request_handlers/domain_req_handlers/revoc_reg_def_handler.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/server/request_handlers/domain_req_handlers/revoc_reg_entry_handler.py` & `indy-node-1.9.2rc1/indy_node/server/request_handlers/domain_req_handlers/revoc_reg_entry_handler.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/server/request_handlers/domain_req_handlers/claim_def_handler.py` & `indy-node-1.9.2rc1/indy_node/server/request_handlers/domain_req_handlers/claim_def_handler.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/server/request_handlers/pool_req_handlers/node_handler.py` & `indy-node-1.9.2rc1/indy_node/server/request_handlers/pool_req_handlers/node_handler.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/server/request_handlers/idr_cache_batch_handler.py` & `indy-node-1.9.2rc1/indy_node/server/request_handlers/idr_cache_batch_handler.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/server/action_log.py` & `indy-node-1.9.2rc1/indy_node/server/action_log.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/server/upgrader.py` & `indy-node-1.9.2rc1/indy_node/server/upgrader.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/server/node_bootstrap.py` & `indy-node-1.9.2rc1/indy_node/server/node_bootstrap.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,26 +73,26 @@
         )
 
     def init_attribute_storage(self):
         # ToDo: refactor this on pluggable handlers integration phase
         attr_store = self.init_attribute_store()
         self.node.db_manager.register_new_store(ATTRIB_LABEL, attr_store)
 
-    def _init_storages(self, domain_storage=None):
-        super()._init_storages(domain_storage)
+    def init_storages(self, storage=None):
+        super().init_storages()
         self.init_idr_cache_storage()
         self.init_attribute_storage()
 
-    def _register_pool_req_handlers(self):
+    def register_pool_req_handlers(self):
         node_handler = NodeHandler(self.node.db_manager,
                                    self.node.bls_bft.bls_crypto_verifier,
                                    self.node.write_req_validator)
         self.node.write_manager.register_req_handler(node_handler)
 
-    def _register_domain_req_handlers(self):
+    def register_domain_req_handlers(self):
         # Read handlers
         get_nym_handler = GetNymHandler(database_manager=self.node.db_manager)
         get_attribute_handler = GetAttributeHandler(database_manager=self.node.db_manager)
         get_schema_handler = GetSchemaHandler(database_manager=self.node.db_manager)
         get_claim_def_handler = GetClaimDefHandler(database_manager=self.node.db_manager)
         get_revoc_reg_def_handler = GetRevocRegDefHandler(database_manager=self.node.db_manager)
         get_revoc_reg_handler = GetRevocRegHandler(database_manager=self.node.db_manager)
@@ -127,15 +127,15 @@
         self.node.read_manager.register_req_handler(get_attribute_handler)
         self.node.read_manager.register_req_handler(get_schema_handler)
         self.node.read_manager.register_req_handler(get_claim_def_handler)
         self.node.read_manager.register_req_handler(get_revoc_reg_def_handler)
         self.node.read_manager.register_req_handler(get_revoc_reg_handler)
         self.node.read_manager.register_req_handler(get_revoc_reg_delta_handler)
 
-    def _register_config_req_handlers(self):
+    def register_config_req_handlers(self):
         # Read handlers
         get_auth_rule_handler = GetAuthRuleHandler(database_manager=self.node.db_manager,
                                                    write_req_validator=self.node.write_req_validator)
         # Write handlers
         auth_rule_handler = AuthRuleHandler(database_manager=self.node.db_manager,
                                             write_req_validator=self.node.write_req_validator)
         auth_rules_handler = AuthRulesHandler(database_manager=self.node.db_manager,
@@ -164,31 +164,31 @@
         self.node.write_manager.register_req_handler(taa_handler)
         self.node.write_manager.register_req_handler(node_upgrade_handler)
         # Register read handlers
         self.node.read_manager.register_req_handler(get_auth_rule_handler)
         self.node.read_manager.register_req_handler(get_taa_aml_handler)
         self.node.read_manager.register_req_handler(get_taa_handler)
 
-    def _register_action_req_handlers(self):
+    def register_action_req_handlers(self):
         # Action handlers
         pool_restart_handler = PoolRestartHandler(database_manager=self.node.db_manager,
                                                   write_req_validator=self.node.write_req_validator,
                                                   restarter=self.node.restarter)
         validator_info_handler = ValidatorInfoHandler(database_manager=self.node.db_manager,
                                                       write_req_validator=self.node.write_req_validator,
                                                       info_tool=self.node._info_tool)
         # Register action handlers
         self.node.action_manager.register_action_handler(pool_restart_handler)
         self.node.action_manager.register_action_handler(validator_info_handler)
 
-    def _register_domain_batch_handlers(self):
-        super()._register_domain_batch_handlers()
+    def register_domain_batch_handlers(self):
+        super().register_domain_batch_handlers()
         self.register_idr_cache_batch_handler()
 
-    def _register_config_batch_handlers(self):
+    def register_config_batch_handlers(self):
         config_batch_handler = ConfigBatchHandler(database_manager=self.node.db_manager,
                                                   upgrader=self.node.upgrader,
                                                   pool_config=self.node.poolCfg)
         self.node.write_manager.register_batch_handler(config_batch_handler)
 
     def register_idr_cache_nym_handler(self):
         idr_cache_nym_handler = IdrCacheNymHandler(database_manager=self.node.db_manager)
@@ -197,14 +197,34 @@
     def register_idr_cache_batch_handler(self):
         idr_cache_batch_handler = IdrCacheBatchHandler(database_manager=self.node.db_manager)
         self.node.write_manager.register_batch_handler(idr_cache_batch_handler)
 
     def init_pool_config(self):
         return PoolConfig(self.node.configLedger)
 
+    def init_domain_ledger(self):
+        """
+        This is usually an implementation of Ledger
+        """
+        if self.node.config.primaryStorage is None:
+            genesis_txn_initiator = GenesisTxnInitiatorFromFile(
+                self.node.genesis_dir, self.node.config.domainTransactionsFile)
+            return Ledger(
+                CompactMerkleTree(
+                    hashStore=self.node.getHashStore('domain')),
+                dataDir=self.node.dataLocation,
+                fileName=self.node.config.domainTransactionsFile,
+                ensureDurability=self.node.config.EnsureLedgerDurability,
+                genesis_txn_initiator=genesis_txn_initiator)
+        else:
+            return initStorage(self.node.config.primaryStorage,
+                               name=self.node.name + NODE_PRIMARY_STORAGE_SUFFIX,
+                               dataDir=self.node.dataLocation,
+                               config=self.node.config)
+
     def init_upgrader(self):
         return Upgrader(self.node.id,
                         self.node.name,
                         self.node.dataLocation,
                         self.node.config,
                         self.node.configLedger,
                         actionFailedCallback=self.node.postConfigLedgerCaughtUp,
@@ -212,16 +232,16 @@
 
     def init_restarter(self):
         return Restarter(self.node.id,
                          self.node.name,
                          self.node.dataLocation,
                          self.node.config)
 
-    def _init_common_managers(self):
-        super()._init_common_managers()
+    def init_common_managers(self):
+        super().init_common_managers()
         self.node.upgrader = self.init_upgrader()
         self.node.restarter = self.init_restarter()
         self.node.poolCfg = self.init_pool_config()
 
     def _init_write_request_validator(self):
         constraint_serializer = ConstraintsSerializer(domain_state_serializer)
         config_state = self.node.states[CONFIG_LEDGER_ID]
```

### Comparing `indy-node-1.9.2.dev1069/indy_node/server/node_maintainer.py` & `indy-node-1.9.2rc1/indy_node/server/node_maintainer.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/__init__.py` & `indy-node-1.9.2rc1/indy_node/__init__.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/__metadata__.py` & `indy-node-1.9.2rc1/indy_node/__metadata__.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/txn_validation/test_pool_upgrade_validation.py` & `indy-node-1.9.2rc1/indy_node/test/txn_validation/test_pool_upgrade_validation.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/txn_validation/test_send_attrib_validation.py` & `indy-node-1.9.2rc1/indy_node/test/txn_validation/test_send_attrib_validation.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/txn_validation/test_send_get_nym_validation.py` & `indy-node-1.9.2rc1/indy_node/test/txn_validation/test_send_get_nym_validation.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/edit_auth_rules.py` & `indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/edit_auth_rules.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/restart.py` & `indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/restart.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/node_properties.py` & `indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/node_properties.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/revoc_reg_def.py` & `indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/revoc_reg_def.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/key_rotation.py` & `indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/key_rotation.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/txn_author_agreement.py` & `indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/txn_author_agreement.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/revoc_reg_entry.py` & `indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/revoc_reg_entry.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/test_auth_rule_using.py` & `indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/test_auth_rule_using.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/upgrade.py` & `indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/upgrade.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/basic.py` & `indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/basic.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/add_roles.py` & `indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/add_roles.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/node_services.py` & `indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/node_services.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/schema.py` & `indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/schema.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/claim_def.py` & `indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/claim_def.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/pool_config.py` & `indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/pool_config.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/txn_author_agreement_aml.py` & `indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/txn_author_agreement_aml.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/edit_roles.py` & `indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/edit_roles.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/validator_info.py` & `indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/validator_info.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/edit_attrib.py` & `indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/edit_attrib.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/add_attrib.py` & `indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/add_attrib.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/auth_rule/auth_framework/edit_auth_rule.py` & `indy-node-1.9.2rc1/indy_node/test/auth_rule/auth_framework/edit_auth_rule.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/auth_rule/test_check_rule_for_add_action_changing.py` & `indy-node-1.9.2rc1/indy_node/test/auth_rule/test_check_rule_for_add_action_changing.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/auth_rule/test_txn_with_different_signature_and_idr.py` & `indy-node-1.9.2rc1/indy_node/test/auth_rule/test_txn_with_different_signature_and_idr.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/auth_rule/test_check_rule_for_edit_action_changing.py` & `indy-node-1.9.2rc1/indy_node/test/auth_rule/test_check_rule_for_edit_action_changing.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/auth_rule/test_get_auth_rule.py` & `indy-node-1.9.2rc1/indy_node/test/auth_rule/test_get_auth_rule.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/auth_rule/test_auth_rules_transaction.py` & `indy-node-1.9.2rc1/indy_node/test/auth_rule/test_auth_rules_transaction.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/auth_rule/test_catching_up_auth_rule_txn.py` & `indy-node-1.9.2rc1/indy_node/test/auth_rule/test_catching_up_auth_rule_txn.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/auth_rule/test_multisig_auth_rule.py` & `indy-node-1.9.2rc1/indy_node/test/auth_rule/test_multisig_auth_rule.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/auth_rule/test_constraint_field.py` & `indy-node-1.9.2rc1/indy_node/test/auth_rule/test_constraint_field.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/auth_rule/test_auth_rule_transaction.py` & `indy-node-1.9.2rc1/indy_node/test/auth_rule/test_auth_rule_transaction.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/auth_rule/test_use_modified_rules_from_uncommitted.py` & `indy-node-1.9.2rc1/indy_node/test/auth_rule/test_use_modified_rules_from_uncommitted.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/auth_rule/helper.py` & `indy-node-1.9.2rc1/indy_node/test/auth_rule/helper.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/auth_rule/test_auth_map.py` & `indy-node-1.9.2rc1/indy_node/test/auth_rule/test_auth_map.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/auth_rule/test_revert_auth_rule_changing.py` & `indy-node-1.9.2rc1/indy_node/test/auth_rule/test_revert_auth_rule_changing.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/replay/test_successive_batch_no_state_change.py` & `indy-node-1.9.2rc1/indy_node/test/replay/test_successive_batch_no_state_change.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/replay/test_state_regenerated_from_ledger.py` & `indy-node-1.9.2rc1/indy_node/test/replay/test_state_regenerated_from_ledger.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/conftest.py` & `indy-node-1.9.2rc1/indy_node/test/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,22 +7,20 @@
 from common.serializers.serialization import domain_state_serializer
 from indy_common.authorize.auth_constraints import ConstraintsSerializer
 from indy_common.authorize.auth_map import auth_map
 from indy_common.authorize.auth_request_validator import WriteRequestValidator
 from indy_common.test.constants import IDENTIFIERS
 from indy_node.persistence.attribute_store import AttributeStore
 from indy_node.persistence.idr_cache import IdrCache
-from indy_node.server.node import Node
 from indy_node.server.node_bootstrap import NodeBootstrap
 from ledger.compact_merkle_tree import CompactMerkleTree
 from plenum.bls.bls_store import BlsStore
 from plenum.common.exceptions import UnauthorizedClientRequest
 from plenum.common.ledger import Ledger
 from plenum.server.database_manager import DatabaseManager
-from plenum.server.request_managers.action_request_manager import ActionRequestManager
 from plenum.server.request_managers.read_request_manager import ReadRequestManager
 from plenum.server.request_managers.write_request_manager import WriteRequestManager
 from plenum.test.pool_transactions.helper import sdk_add_new_nym, sdk_pool_refresh, prepare_new_node_data, \
     create_and_start_new_node, prepare_node_request, sdk_sign_and_send_prepared_request
 from plenum.test.testing_utils import FakeSomething
 from state.pruning_state import PruningState
 from storage.kv_in_memory import KeyValueStorageInMemory
@@ -375,43 +373,33 @@
     return FakeSomething()
 
 
 @pytest.fixture(scope="module")
 def fake_node(db_manager, fake_pool_cfg, fake_upgrader, fake_restarter, fake_pool_manager):
     wm = WriteRequestManager(database_manager=db_manager)
     rm = ReadRequestManager()
-    am = ActionRequestManager()
-    return FakeSomething(name="fake_node",
-                         dataLocation="//place_that_cannot_exist",
-                         genesis_dir="//place_that_cannot_exist",
-                         ledger_ids=Node.ledger_ids,
-                         write_manager=wm,
+    return FakeSomething(write_manager=wm,
                          read_manager=rm,
-                         action_manager=am,
                          db_manager=db_manager,
                          write_req_validator=write_auth_req_validator,
-                         config=FakeSomething(
-                             stewardThreshold=20,
-                             poolTransactionsFile="//pool_genesis_that_cannot_exist",
-                             domainTransactionsFile="//domain_genesis_that_cannot_exist"
-                         ),
+                         config=FakeSomething(stewardThreshold=20),
                          poolCfg=fake_pool_cfg,
                          upgrader=fake_upgrader,
                          restarter=fake_restarter,
                          poolManager=fake_pool_manager)
 
 
 @pytest.fixture(scope="module")
 def _managers(write_auth_req_validator,
               fake_node):
     nbs = TestNodeBootstrap(fake_node)
-    nbs._register_domain_req_handlers()
-    nbs._register_domain_batch_handlers()
-    nbs._register_config_req_handlers()
-    nbs._register_config_batch_handlers()
+    nbs.register_domain_req_handlers()
+    nbs.register_domain_batch_handlers()
+    nbs.register_config_req_handlers()
+    nbs.register_config_batch_handlers()
     return fake_node.write_manager, fake_node.read_manager
 
 
 @pytest.fixture(scope="module")
 def write_manager(_managers):
     return _managers[0]
```

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/txn_author_agreement/test_node_taa.py` & `indy-node-1.9.2rc1/indy_node/test/txn_author_agreement/test_node_taa.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/txn_author_agreement/test_get_taa_aml.py` & `indy-node-1.9.2rc1/indy_node/test/txn_author_agreement/test_get_taa_aml.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_pool_upgrade_same_version.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_pool_upgrade_same_version.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_pool_upgrade_no_loop_reinstall_unsuccessful.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_pool_upgrade_no_loop_reinstall_unsuccessful.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/conftest.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/conftest.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_upgrade_timeout.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_upgrade_timeout.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_pool_upgrade_same_version_reinstall.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_pool_upgrade_same_version_reinstall.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_upgrade_pool_with_demoted_nodes.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_upgrade_pool_with_demoted_nodes.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_upgrader.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_upgrader.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_pool_upgrade_cancel.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_pool_upgrade_cancel.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_control_tool_performs_migrations.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_control_tool_performs_migrations.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_restart_log.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_restart_log.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_handles_forced_upgrade_on_propagate.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_handles_forced_upgrade_on_propagate.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_schedules_upgrade_after_pool_ledger_update.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_schedules_upgrade_after_pool_ledger_update.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_does_not_reschedule_canceled_upgrade.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_does_not_reschedule_canceled_upgrade.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_migration_util.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_migration_util.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_control_tool_processes_invalid_data.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_control_tool_processes_invalid_data.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_upgrade_unsuccessful.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_upgrade_unsuccessful.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_forced_upgrade_if_ordered_and_then_request_received.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_forced_upgrade_if_ordered_and_then_request_received.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_upgrade_rescheduled_view_change.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_upgrade_rescheduled_view_change.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_schedules_upgrade_after_restart.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_schedules_upgrade_after_restart.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_pool_upgrade_no_loop_reinstall.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_pool_upgrade_no_loop_reinstall.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_handles_forced_upgrade_on_client_request.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_handles_forced_upgrade_on_client_request.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_pool_upgrade_no_loop_unsuccessful.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_pool_upgrade_no_loop_unsuccessful.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_communication_with_control_service.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_communication_with_control_service.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_send_node_upgrade.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_send_node_upgrade.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_pool_upgrade_reject.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_pool_upgrade_reject.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_version_parsing.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_version_parsing.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_reschedules_upgrade_for_proper_datetime.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_reschedules_upgrade_for_proper_datetime.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_forced_upgrade_no_consensus_on_single_node.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_forced_upgrade_no_consensus_on_single_node.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_control_tool_removes_backups.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_control_tool_removes_backups.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_pool_upgrade_no_loop_force.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_pool_upgrade_no_loop_force.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_control_tool_receives_messages.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_control_tool_receives_messages.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_reschedule_upgrade_lower_version.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_reschedule_upgrade_lower_version.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_pool_upgrade_no_loop.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_pool_upgrade_no_loop.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_control_tool_resolves_dependencies.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_control_tool_resolves_dependencies.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_sustain_invalid_upgrade_txn.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_sustain_invalid_upgrade_txn.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_upgrade.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_upgrade.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_control_tool_restores_from_backups.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_control_tool_restores_from_backups.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_pool_upgrade_through_catchup.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_pool_upgrade_through_catchup.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_get_deps_with_filter.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_get_deps_with_filter.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_broken_connection_control_tool.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_broken_connection_control_tool.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_migration_tool.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_migration_tool.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_action_log.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_action_log.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/helper.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/helper.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_control_tool_creates_backups.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_control_tool_creates_backups.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_upgrade_log.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_upgrade_log.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_forced_upgrade_if_request_received_after_propagate.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_forced_upgrade_if_request_received_after_propagate.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_control_tool_resolves_dep_top_level.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_control_tool_resolves_dep_top_level.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_upgrade_in_progress.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_upgrade_in_progress.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_force_upgrade_process_in_view_change.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_force_upgrade_process_in_view_change.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import pytest
 
 from indy_common.constants import POOL_UPGRADE
 from indy_node.server.node import Node
 from plenum.common.constants import FORCE, TXN_TYPE
 from plenum.test.helper import sdk_gen_request
-from plenum.test.primary_selection.test_view_changer_primary_selection import FakeNode
+from plenum.test.primary_selection.test_primary_selector import FakeNode
 
 
 @pytest.fixture(scope='function')
 def fake_node(tdir, tconf):
     node = FakeNode(tdir, config=tconf)
     node.unpackClientMsg = functools.partial(Node.unpackClientMsg, node)
     node.is_request_need_quorum = functools.partial(Node.is_request_need_quorum, node)
```

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_pool_upgrade_same_time_different_days.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_pool_upgrade_same_time_different_days.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_pool_upgrade_no_loop_force_unsuccessful.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_pool_upgrade_no_loop_force_unsuccessful.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/upgrade/test_node_schedules_upgrade_for_proper_datetime.py` & `indy-node-1.9.2rc1/indy_node/test/upgrade/test_node_schedules_upgrade_for_proper_datetime.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/nym_txn/test_demote_network_monitor.py` & `indy-node-1.9.2rc1/indy_node/test/nym_txn/test_demote_network_monitor.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/nym_txn/test_nym_auth_rules.py` & `indy-node-1.9.2rc1/indy_node/test/nym_txn/test_nym_auth_rules.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/nym_txn/test_nym_blacklisting.py` & `indy-node-1.9.2rc1/indy_node/test/nym_txn/test_nym_blacklisting.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/nym_txn/test_send_nym_validation.py` & `indy-node-1.9.2rc1/indy_node/test/nym_txn/test_send_nym_validation.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/nym_txn/test_nym_resend.py` & `indy-node-1.9.2rc1/indy_node/test/nym_txn/test_nym_resend.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/nym_txn/test_nym.py` & `indy-node-1.9.2rc1/indy_node/test/nym_txn/test_nym.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/nym_txn/test_create_did_without_endorser.py` & `indy-node-1.9.2rc1/indy_node/test/nym_txn/test_create_did_without_endorser.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/nym_txn/test_nym_additional.py` & `indy-node-1.9.2rc1/indy_node/test/nym_txn/test_nym_additional.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/catchup/conftest.py` & `indy-node-1.9.2rc1/indy_node/test/catchup/conftest.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/catchup/test_requests_post_new_node_catchup.py` & `indy-node-1.9.2rc1/indy_node/test/catchup/test_requests_post_new_node_catchup.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/catchup/test_requests_post_multiple_new_nodes.py` & `indy-node-1.9.2rc1/indy_node/test/catchup/test_requests_post_multiple_new_nodes.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/catchup/test_batch_rejected_and_later_ordered_on_catchup.py` & `indy-node-1.9.2rc1/indy_node/test/catchup/test_batch_rejected_and_later_ordered_on_catchup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from types import MethodType
 
 import logging
 import pytest
 
 from indy_node.server.node import Node
 from plenum.common.batched import Batched
-from plenum.server.consensus.ordering_service import OrderingService
 from plenum.test.delayers import cDelay, lsDelay
 from plenum.test.pool_transactions.helper import sdk_add_new_nym
 from plenum.test.test_node import getNonPrimaryReplicas
 from stp_core.common.log import getlogger
 from stp_core.loop.eventually import eventually
 
 logger = getlogger()
@@ -78,42 +77,41 @@
     12. Prior to ledgers synchronization the slow node processes the stashed
     Commits messages and orders batch.
     13. The slow node synchronizes its ledgers and completes the catch-up.
     """
 
     non_primary_replicas_of_master = getNonPrimaryReplicas(nodeSet, 0)
     slow_node = non_primary_replicas_of_master[0].node
-    slow_os = slow_node.master_replica._ordering_service
 
     slow_node.nodeIbStasher.delay(cDelay(300))
     slow_node.start_catchup = MethodType(patched_start_catchup, slow_node)
 
     no_more_catchups_needed_call_times_before = \
         slow_node.spylog.count(Node.no_more_catchups_needed.__name__)
     on_batch_rejected_call_times_before = \
-        slow_os.spylog.count(OrderingService.post_batch_rejection.__name__)
+        slow_node.spylog.count(Node.onBatchRejected.__name__)
     on_batch_created_call_times_before = \
-        slow_os.spylog.count(OrderingService.post_batch_creation.__name__)
+        slow_node.spylog.count(Node.onBatchCreated.__name__)
     process_ordered_call_times_before = \
         slow_node.spylog.count(Node.processOrdered.__name__)
 
     send_random_requests(looper, sdk_pool_handle, sdk_wallet_endorser, 1)
 
     slow_node.start_catchup()
 
     def check_catchup_done():
         assert slow_node.spylog.count(Node.no_more_catchups_needed.__name__) > \
                no_more_catchups_needed_call_times_before
 
     looper.run(eventually(check_catchup_done, retryWait=1, timeout=10))
 
     on_batch_rejected_call_times_after = \
-        slow_os.spylog.count(OrderingService.post_batch_rejection.__name__)
+        slow_node.spylog.count(Node.onBatchRejected.__name__)
     on_batch_created_call_times_after = \
-        slow_os.spylog.count(OrderingService.post_batch_creation.__name__)
+        slow_node.spylog.count(Node.onBatchCreated.__name__)
     process_ordered_call_times_after = \
         slow_node.spylog.count(Node.processOrdered.__name__)
 
     assert on_batch_rejected_call_times_after \
            - on_batch_rejected_call_times_before == 1
 
     assert on_batch_created_call_times_after \
```

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/node_control_utils/test_debian_version.py` & `indy-node-1.9.2rc1/indy_node/test/node_control_utils/test_debian_version.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/node_control_utils/test_node_control_util.py` & `indy-node-1.9.2rc1/indy_node/test/node_control_utils/test_node_control_util.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/node_txn/test_send_node_validation.py` & `indy-node-1.9.2rc1/indy_node/test/node_txn/test_send_node_validation.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/view_change/test_view_change_during_alternating_unstash.py` & `indy-node-1.9.2rc1/indy_node/test/view_change/test_view_change_during_alternating_unstash.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/request_propagates/test_request_propagates.py` & `indy-node-1.9.2rc1/indy_node/test/request_propagates/test_request_propagates.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/tools/test_nsreplay.py` & `indy-node-1.9.2rc1/indy_node/test/tools/test_nsreplay.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,15 +79,14 @@
 
 
 @pytest.yield_fixture(scope="session", autouse=True)
 def warncheck(warnfilters):
     pass
 
 
-@pytest.mark.skip(reason="Need to fix nsreplay due to OrderingService integration")
 def test_end_to_end_replay(looper,
                            tdir,
                            tdirWithPoolTxns,
                            tdirWithDomainTxns,
                            nodeSet,
                            sdk_pool_handle,
                            sdk_wallet_endorser
```

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/memory_debugging/test_memory_debugging.py` & `indy-node-1.9.2rc1/indy_node/test/memory_debugging/test_memory_debugging.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/did/conftest.py` & `indy-node-1.9.2rc1/indy_node/test/did/conftest.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/did/test_did_with_abbreviated_verkey.py` & `indy-node-1.9.2rc1/indy_node/test/did/test_did_with_abbreviated_verkey.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/did/test_did_with_no_verkey.py` & `indy-node-1.9.2rc1/indy_node/test/did/test_did_with_no_verkey.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/did/test_did_with_full_verkey.py` & `indy-node-1.9.2rc1/indy_node/test/did/test_did_with_full_verkey.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/package/test_metadata.py` & `indy-node-1.9.2rc1/indy_node/test/package/test_metadata.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/validator_info/test_validator_info_command.py` & `indy-node-1.9.2rc1/indy_node/test/validator_info/test_validator_info_command.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/validator_info/test_validator_info.py` & `indy-node-1.9.2rc1/indy_node/test/validator_info/test_validator_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 
 from indy_node.test.state_proof.helper import sdk_submit_operation_and_get_result
 from plenum.common.constants import TARGET_NYM, RAW, NAME, VERSION, ORIGIN
 
 # noinspection PyUnresolvedReferences
 from plenum.common.ledger import Ledger
-from plenum.test.primary_selection.test_view_changer_primary_selection import FakeLedger
+from plenum.test.primary_selection.test_primary_selector import FakeLedger
 from plenum.test.validator_info.conftest import info, node  # qa
 
 from indy_common.constants import TXN_TYPE, DATA, GET_NYM, GET_ATTR, GET_SCHEMA, GET_CLAIM_DEF, REF, SIGNATURE_TYPE
 from indy_node.__metadata__ import __version__ as node_pgk_version
 
 PERIOD_SEC = 1
 TEST_NODE_NAME = 'Alpha'
```

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/validator_info/test_validator_info_handler.py` & `indy-node-1.9.2rc1/indy_node/test/validator_info/test_validator_info_handler.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/validator_info/helper.py` & `indy-node-1.9.2rc1/indy_node/test/validator_info/helper.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/request_handlers/conftest.py` & `indy-node-1.9.2rc1/indy_node/test/request_handlers/conftest.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/request_handlers/test_nym_handler.py` & `indy-node-1.9.2rc1/indy_node/test/request_handlers/test_nym_handler.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/request_handlers/test_attrib_handler.py` & `indy-node-1.9.2rc1/indy_node/test/request_handlers/test_attrib_handler.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/request_handlers/test_txn_author_agreement_aml_handler.py` & `indy-node-1.9.2rc1/indy_node/test/request_handlers/test_txn_author_agreement_aml_handler.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/request_handlers/test_claim_def_handler.py` & `indy-node-1.9.2rc1/indy_node/test/request_handlers/test_claim_def_handler.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/request_handlers/test_auth_rule_handler.py` & `indy-node-1.9.2rc1/indy_node/test/request_handlers/test_auth_rule_handler.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/request_handlers/test_pool_upgrade_handler.py` & `indy-node-1.9.2rc1/indy_node/test/request_handlers/test_pool_upgrade_handler.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/request_handlers/test_get_auth_rule_handler.py` & `indy-node-1.9.2rc1/indy_node/test/request_handlers/test_get_auth_rule_handler.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/request_handlers/test_update_state_config_req_handler.py` & `indy-node-1.9.2rc1/indy_node/test/request_handlers/test_update_state_config_req_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 import functools
+import os
 
 import pytest
 import time
 import json
 
+from common.serializers.serialization import domain_state_serializer
 from indy_common.authorize.auth_actions import AuthActionAdd
-from indy_common.authorize.auth_constraints import AuthConstraint
+from indy_common.authorize.auth_constraints import AuthConstraint, ConstraintsSerializer
 from indy_common.state import config
-from plenum.common.constants import NYM, ROLE, TRUSTEE, STEWARD, CONFIG_LEDGER_ID, TXN_METADATA, \
+from indy_node.server.node_bootstrap import NodeBootstrap
+from ledger.compact_merkle_tree import CompactMerkleTree
+from plenum.common.constants import TXN_TYPE, NYM, ROLE, TRUSTEE, STEWARD, CONFIG_LEDGER_ID, TXN_METADATA, \
     TXN_METADATA_SEQ_NO
+from plenum.common.ledger import Ledger
 from plenum.common.txn_util import reqToTxn, get_payload_data
+from plenum.common.util import randomString
+from plenum.server.database_manager import DatabaseManager
+from plenum.server.replica import Replica
 from plenum.common.request import Request
-from plenum.server.ledgers_bootstrap import LedgersBootstrap
+from plenum.server.request_managers.write_request_manager import WriteRequestManager
 from plenum.test.testing_utils import FakeSomething
 from state.pruning_state import PruningState
 from storage.kv_in_memory import KeyValueStorageInMemory
 
 from indy_node.test.helper import build_auth_rule_request_json
 
 
@@ -87,28 +95,28 @@
     txn = reqToTxn(request)
     txn[TXN_METADATA][TXN_METADATA_SEQ_NO] = 1
     """Add txn to ledger"""
     db_manager.get_ledger(CONFIG_LEDGER_ID).appendTxns([txn])
     db_manager.get_ledger(CONFIG_LEDGER_ID).commitTxns(req_count)
     # ToDo: ugly fix... Refactor this on pluggable req handler integration phase
     init_state_from_ledger = functools.partial(
-        LedgersBootstrap._init_state_from_ledger,
+        NodeBootstrap.init_state_from_ledger,
         FakeSomething(
-            db_manager=db_manager,
-            write_manager=write_manager,
-            _update_txn_with_extra_data=lambda txn: txn))
+            node=FakeSomething(update_txn_with_extra_data=lambda txn: txn,
+                write_manager=write_manager)))
     """Check that txn is not exist in state"""
     assert db_manager.get_state(CONFIG_LEDGER_ID).get(config.make_state_path_for_auth_rule(action.get_action_id()),
                             isCommitted=False) is None
     assert db_manager.get_state(CONFIG_LEDGER_ID).get(config.make_state_path_for_auth_rule(action.get_action_id()),
                             isCommitted=True) is None
     txns_from_ledger = [t for t in db_manager.get_ledger(CONFIG_LEDGER_ID).getAllTxn()]
     """Check, that txn exist in ledger"""
     assert len(txns_from_ledger) == 1
     assert get_payload_data(txns_from_ledger[0][1]) == get_payload_data(txn)
     """Emulating node starting"""
-    init_state_from_ledger(CONFIG_LEDGER_ID)
+    init_state_from_ledger(db_manager.get_state(CONFIG_LEDGER_ID),
+                           db_manager.get_ledger(CONFIG_LEDGER_ID))
     """Check that txn was added into state"""
     from_state = db_manager.get_state(CONFIG_LEDGER_ID) .get(
         config.make_state_path_for_auth_rule(action.get_action_id()),
         isCommitted=True)
     assert constraint_serializer.deserialize(from_state) == constraint
```

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/request_handlers/test_schema_handler.py` & `indy-node-1.9.2rc1/indy_node/test/request_handlers/test_schema_handler.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/request_handlers/test_revoc_reg_def_handler.py` & `indy-node-1.9.2rc1/indy_node/test/request_handlers/test_revoc_reg_def_handler.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/request_handlers/test_revoc_reg_entry_handler.py` & `indy-node-1.9.2rc1/indy_node/test/request_handlers/test_revoc_reg_entry_handler.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/request_handlers/test_txn_author_agreement_handler.py` & `indy-node-1.9.2rc1/indy_node/test/request_handlers/test_txn_author_agreement_handler.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/request_handlers/test_auth_rules_handler.py` & `indy-node-1.9.2rc1/indy_node/test/request_handlers/test_auth_rules_handler.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/request_handlers/helper.py` & `indy-node-1.9.2rc1/indy_node/test/request_handlers/helper.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/claim_def/test_send_claim_def.py` & `indy-node-1.9.2rc1/indy_node/test/claim_def/test_send_claim_def.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/claim_def/test_send_get_claim_def.py` & `indy-node-1.9.2rc1/indy_node/test/claim_def/test_send_get_claim_def.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/claim_def/test_claim_def_auth_rule.py` & `indy-node-1.9.2rc1/indy_node/test/claim_def/test_claim_def_auth_rule.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/suspension/test_suspension.py` & `indy-node-1.9.2rc1/indy_node/test/suspension/test_suspension.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/suspension/test_node_suspension.py` & `indy-node-1.9.2rc1/indy_node/test/suspension/test_node_suspension.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/suspension/test_nym_suspension.py` & `indy-node-1.9.2rc1/indy_node/test/suspension/test_nym_suspension.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/attrib_txn/test_send_get_attr.py` & `indy-node-1.9.2rc1/indy_node/test/attrib_txn/test_send_get_attr.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/attrib_txn/test_nym_attrib.py` & `indy-node-1.9.2rc1/indy_node/test/attrib_txn/test_nym_attrib.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/attrib_txn/test_attrib_txn_digest.py` & `indy-node-1.9.2rc1/indy_node/test/attrib_txn/test_attrib_txn_digest.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/attrib_txn/test_n_minus_f_pool_processes_attrib.py` & `indy-node-1.9.2rc1/indy_node/test/attrib_txn/test_n_minus_f_pool_processes_attrib.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/schema/test_send_schema.py` & `indy-node-1.9.2rc1/indy_node/test/schema/test_send_schema.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/schema/test_send_get_schema.py` & `indy-node-1.9.2rc1/indy_node/test/schema/test_send_get_schema.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/pool_config/conftest.py` & `indy-node-1.9.2rc1/indy_node/test/pool_config/conftest.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/pool_config/test_pool_config.py` & `indy-node-1.9.2rc1/indy_node/test/pool_config/test_pool_config.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/pool_config/test_send_pool_config.py` & `indy-node-1.9.2rc1/indy_node/test/pool_config/test_send_pool_config.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/pool_config/test_send_pool_config_only_trustee.py` & `indy-node-1.9.2rc1/indy_node/test/pool_config/test_send_pool_config_only_trustee.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/pool_config/helper.py` & `indy-node-1.9.2rc1/indy_node/test/pool_config/helper.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/anon_creds/test_state_proof_for_get_request.py` & `indy-node-1.9.2rc1/indy_node/test/anon_creds/test_state_proof_for_get_request.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/anon_creds/conftest.py` & `indy-node-1.9.2rc1/indy_node/test/anon_creds/conftest.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/anon_creds/test_get_revoc_reg_delta_send_by_default.py` & `indy-node-1.9.2rc1/indy_node/test/anon_creds/test_get_revoc_reg_delta_send_by_default.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/anon_creds/test_get_revoc_reg_delta_with_none_results.py` & `indy-node-1.9.2rc1/indy_node/test/anon_creds/test_get_revoc_reg_delta_with_none_results.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/anon_creds/test_revoc_reg_entry_validation.py` & `indy-node-1.9.2rc1/indy_node/test/anon_creds/test_revoc_reg_entry_validation.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/anon_creds/test_integration_get_revoc_delta.py` & `indy-node-1.9.2rc1/indy_node/test/anon_creds/test_integration_get_revoc_delta.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/anon_creds/test_get_revoc_reg_def_send.py` & `indy-node-1.9.2rc1/indy_node/test/anon_creds/test_get_revoc_reg_def_send.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/anon_creds/test_get_revoc_reg_delta_unit.py` & `indy-node-1.9.2rc1/indy_node/test/anon_creds/test_get_revoc_reg_delta_unit.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/anon_creds/test_get_revoc_reg_delta_validation.py` & `indy-node-1.9.2rc1/indy_node/test/anon_creds/test_get_revoc_reg_delta_validation.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/anon_creds/test_revoc_def_send.py` & `indy-node-1.9.2rc1/indy_node/test/anon_creds/test_revoc_def_send.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/anon_creds/test_incorrect_revoc_reg_def.py` & `indy-node-1.9.2rc1/indy_node/test/anon_creds/test_incorrect_revoc_reg_def.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/anon_creds/test_get_revoc_reg_delta_send_by_demand.py` & `indy-node-1.9.2rc1/indy_node/test/anon_creds/test_get_revoc_reg_delta_send_by_demand.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/anon_creds/test_revoc_def_validation.py` & `indy-node-1.9.2rc1/indy_node/test/anon_creds/test_revoc_def_validation.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/anon_creds/test_get_revoc_reg_send.py` & `indy-node-1.9.2rc1/indy_node/test/anon_creds/test_get_revoc_reg_send.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/anon_creds/helper.py` & `indy-node-1.9.2rc1/indy_node/test/anon_creds/helper.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/anon_creds/test_get_revoc_reg_entry.py` & `indy-node-1.9.2rc1/indy_node/test/anon_creds/test_get_revoc_reg_entry.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/endorser/test_send_by_endorser.py` & `indy-node-1.9.2rc1/indy_node/test/endorser/test_send_by_endorser.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/persistence/test_idr_cache_update_after_catchup.py` & `indy-node-1.9.2rc1/indy_node/test/persistence/test_idr_cache_update_after_catchup.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/persistence/test_idr_cache.py` & `indy-node-1.9.2rc1/indy_node/test/persistence/test_idr_cache.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/state_proof/conftest.py` & `indy-node-1.9.2rc1/indy_node/test/state_proof/conftest.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/state_proof/test_asking_one_node.py` & `indy-node-1.9.2rc1/indy_node/test/state_proof/test_asking_one_node.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/state_proof/test_state_proof_for_get_requests.py` & `indy-node-1.9.2rc1/indy_node/test/state_proof/test_state_proof_for_get_requests.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/state_proof/helper.py` & `indy-node-1.9.2rc1/indy_node/test/state_proof/helper.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/state_proof/test_state_proof_for_missing_data.py` & `indy-node-1.9.2rc1/indy_node/test/state_proof/test_state_proof_for_missing_data.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/state_proof/test_state_multi_proofs_for_get_requests.py` & `indy-node-1.9.2rc1/indy_node/test/state_proof/test_state_multi_proofs_for_get_requests.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/api/test_attrib_reply.py` & `indy-node-1.9.2rc1/indy_node/test/api/test_attrib_reply.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/api/test_nym_reply.py` & `indy-node-1.9.2rc1/indy_node/test/api/test_nym_reply.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/api/test_claim_def_reply.py` & `indy-node-1.9.2rc1/indy_node/test/api/test_claim_def_reply.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/api/helper.py` & `indy-node-1.9.2rc1/indy_node/test/api/helper.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/helper.py` & `indy-node-1.9.2rc1/indy_node/test/helper.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/write_permission/test_revocation_write_permission.py` & `indy-node-1.9.2rc1/indy_node/test/write_permission/test_revocation_write_permission.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/write_permission/test_send_write_permission_no_client.py` & `indy-node-1.9.2rc1/indy_node/test/write_permission/test_send_write_permission_no_client.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/pool_restart/test_restart_on_inconsistency.py` & `indy-node-1.9.2rc1/indy_node/test/pool_restart/test_restart_on_inconsistency.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/pool_restart/test_pool_restart.py` & `indy-node-1.9.2rc1/indy_node/test/pool_restart/test_pool_restart.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/pool_restart/test_fail_pool_restart.py` & `indy-node-1.9.2rc1/indy_node/test/pool_restart/test_fail_pool_restart.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/pool_restart/helper.py` & `indy-node-1.9.2rc1/indy_node/test/pool_restart/helper.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/pool_restart/test_pool_restarts_one_by_one.py` & `indy-node-1.9.2rc1/indy_node/test/pool_restart/test_pool_restarts_one_by_one.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/pool_restart/test_node_control_tool_for_restart.py` & `indy-node-1.9.2rc1/indy_node/test/pool_restart/test_node_control_tool_for_restart.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/test/pool_restart/test_pool_restarts_one_by_one_with_restart_now.py` & `indy-node-1.9.2rc1/indy_node/test/pool_restart/test_pool_restarts_one_by_one_with_restart_now.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/utils/node_control_utils.py` & `indy-node-1.9.2rc1/indy_node/utils/node_control_utils.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/utils/node_runner.py` & `indy-node-1.9.2rc1/indy_node/utils/node_runner.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/utils/node_control_tool.py` & `indy-node-1.9.2rc1/indy_node/utils/node_control_tool.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/utils/migration_tool.py` & `indy-node-1.9.2rc1/indy_node/utils/migration_tool.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/persistence/idr_cache.py` & `indy-node-1.9.2rc1/indy_node/persistence/idr_cache.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node/persistence/attribute_store.py` & `indy-node-1.9.2rc1/indy_node/persistence/attribute_store.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/indy_node.egg-info/SOURCES.txt` & `indy-node-1.9.2rc1/indy_node.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 post-setup.py
 setup.py
 data/__init__.py
 data/node_control.conf
 data/nssm_original.exe
 data/migrations/README.md
 data/migrations/__init__.py
-data/migrations/deb/1_0_96_to_1_0_97.py
-data/migrations/deb/1_1_150_to_1_1_151.py
-data/migrations/deb/1_2_188_to_1_2_189.py
-data/migrations/deb/1_2_233_to_1_2_234.py
-data/migrations/deb/1_2_273_to_1_2_274.py
+data/migrations/deb/1_0_28_to_1_0_29.py
+data/migrations/deb/1_1_37_to_1_1_38.py
+data/migrations/deb/1_1_43_to_1_2_44.py
+data/migrations/deb/1_2_44_to_1_2_45.py
+data/migrations/deb/1_2_50_to_1_2_51.py
+data/migrations/deb/1_2_51_to_1_2_52.py
 data/migrations/deb/1_3_396_to_1_3_397.py
 data/migrations/deb/1_3_428_to_1_3_429.py
 data/migrations/deb/1_3_433_to_1_3_434.py
 data/migrations/deb/1_4_500_to_1_4_501.py
 data/migrations/deb/1_6_703_to_1_6_704.py
 data/migrations/deb/1_9_1_to_1_9_2.py
 data/migrations/deb/__init__.py
-data/migrations/deb/disabled_1_0_97_to_1_0_96.py
-data/migrations/deb/helper_1_0_96_to_1_0_97.py
+data/migrations/deb/disabled_1_0_29_to_1_0_28.py
+data/migrations/deb/helper_1_0_28_to_1_0_29.py
+data/migrations/deb/helper_1_1_37_to_1_1_38.py
 indy_common/__init__.py
 indy_common/auth.py
 indy_common/config.py
 indy_common/config_helper.py
 indy_common/config_util.py
 indy_common/constants.py
 indy_common/did_method.py
```

### Comparing `indy-node-1.9.2.dev1069/sample/thrift-loan-application.indy` & `indy-node-1.9.2rc1/sample/thrift-loan-application.indy`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/sample/acme-job-application.indy` & `indy-node-1.9.2rc1/sample/acme-job-application.indy`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/scripts/node_address_list` & `indy-node-1.9.2rc1/scripts/node_address_list`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/scripts/get_metrics` & `indy-node-1.9.2rc1/scripts/get_metrics`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/scripts/init_indy_keys` & `indy-node-1.9.2rc1/scripts/init_indy_keys`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/scripts/current_validators` & `indy-node-1.9.2rc1/scripts/current_validators`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/scripts/restart_indy_node_ubuntu1604.sh` & `indy-node-1.9.2rc1/scripts/restart_indy_node_ubuntu1604.sh`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/scripts/generate_indy_pool_transactions` & `indy-node-1.9.2rc1/scripts/generate_indy_pool_transactions`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/scripts/upgrade_indy_node_ubuntu1604.sh` & `indy-node-1.9.2rc1/scripts/upgrade_indy_node_ubuntu1604.sh`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/scripts/install_indy_node.bat` & `indy-node-1.9.2rc1/scripts/install_indy_node.bat`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/scripts/setup_iptables` & `indy-node-1.9.2rc1/scripts/setup_iptables`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/scripts/complete_rebranding_upgrade_ubuntu1604.sh` & `indy-node-1.9.2rc1/scripts/complete_rebranding_upgrade_ubuntu1604.sh`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/scripts/get_keys` & `indy-node-1.9.2rc1/scripts/get_keys`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/scripts/start_indy_node` & `indy-node-1.9.2rc1/scripts/start_indy_node`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/scripts/init_bls_keys` & `indy-node-1.9.2rc1/scripts/init_bls_keys`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/scripts/upgrade_indy_node_ubuntu1604_test.sh` & `indy-node-1.9.2rc1/scripts/upgrade_indy_node_ubuntu1604_test.sh`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/scripts/create_dirs.sh` & `indy-node-1.9.2rc1/scripts/create_dirs.sh`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/scripts/start_node_control_tool` & `indy-node-1.9.2rc1/scripts/start_node_control_tool`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/scripts/validator-info-history` & `indy-node-1.9.2rc1/scripts/validator-info-history`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/scripts/validator-info` & `indy-node-1.9.2rc1/scripts/validator-info`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/scripts/clear_node.py` & `indy-node-1.9.2rc1/scripts/clear_node.py`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/scripts/generate_bls_proof_of_possession` & `indy-node-1.9.2rc1/scripts/generate_bls_proof_of_possession`

 * *Files identical despite different names*

### Comparing `indy-node-1.9.2.dev1069/scripts/read_ledger` & `indy-node-1.9.2rc1/scripts/read_ledger`

 * *Files identical despite different names*

