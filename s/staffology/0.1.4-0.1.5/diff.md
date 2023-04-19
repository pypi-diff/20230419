# Comparing `tmp/staffology-0.1.4.tar.gz` & `tmp/staffology-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "staffology-0.1.4.tar", last modified: Mon Nov 21 10:11:12 2022, max compression
+gzip compressed data, was "staffology-0.1.5.tar", last modified: Wed Apr 19 11:49:50 2023, max compression
```

## Comparing `staffology-0.1.4.tar` & `staffology-0.1.5.tar`

### file list

```diff
@@ -1,978 +1,978 @@
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:12.225598 staffology-0.1.4/
--rw-r--r--   0 isikkaplan   (501) staff       (20)      524 2022-11-21 10:11:12.225377 staffology-0.1.4/PKG-INFO
--rw-r--r--   0 isikkaplan   (501) staff       (20)      135 2022-10-21 20:55:55.000000 staffology-0.1.4/README.md
--rw-r--r--   0 isikkaplan   (501) staff       (20)       38 2022-11-21 10:11:12.225653 staffology-0.1.4/setup.cfg
--rw-r--r--   0 isikkaplan   (501) staff       (20)      666 2022-11-21 10:10:39.000000 staffology-0.1.4/setup.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:11.926969 staffology-0.1.4/staffology/
--rw-r--r--   0 isikkaplan   (501) staff       (20)      167 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/__init__.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:11.928247 staffology-0.1.4/staffology/api/
--rw-r--r--   0 isikkaplan   (501) staff       (20)       47 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/__init__.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:11.932200 staffology-0.1.4/staffology/api/account/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/account/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4467 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/account/activate_account.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4029 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/account/change_email_address_account.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3201 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/account/create_api_key_account.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1579 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/account/create_demo_employer_account.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1620 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/account/delete_api_key_account.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3846 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/account/get_account.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2458 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/account/get_api_key_account.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2674 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/account/get_employer_defaults_account.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3653 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/account/get_invitations_account.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4011 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/account/get_tenant_account.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2462 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/account/list_api_keys_account.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4020 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/account/profile_account.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4165 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/account/set_employer_defaults_account.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3190 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/account/update_cookie_preferences_account.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3600 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/account/update_photo_account.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1905 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/account/verify_account.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3581 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/account/verify_response_account.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:11.935261 staffology-0.1.4/staffology/api/attachment_order/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/attachment_order/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2810 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/attachment_order/add_document_attachment_order.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2572 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/attachment_order/create_attachment_order.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2344 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/attachment_order/delete_attachment_order.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2604 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/attachment_order/delete_document_attachment_order.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4114 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/attachment_order/get_attachment_order.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4408 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/attachment_order/get_document_attachment_order.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3562 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/attachment_order/index_attachment_order.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4366 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/attachment_order/payments_attachment_order.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4674 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/attachment_order/update_attachment_order.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:11.935852 staffology-0.1.4/staffology/api/audit/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/audit/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     7628 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/audit/employer_audit_list_audit.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:11.940648 staffology-0.1.4/staffology/api/auto_enrolment/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/auto_enrolment/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3787 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/auto_enrolment/assess_auto_enrolment.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2321 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/auto_enrolment/delete_auto_enrolment.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4015 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/auto_enrolment/email_letter_auto_enrolment.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3692 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/auto_enrolment/get_auto_enrolment.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3468 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/auto_enrolment/get_last_auto_enrolment.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4847 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/auto_enrolment/get_letter_auto_enrolment.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3591 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/auto_enrolment/list_auto_enrolment.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2522 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/auto_enrolment/mark_letter_as_sent_auto_enrolment.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3234 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/auto_enrolment/pending_letters_auto_enrolment.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3743 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/auto_enrolment/pending_postponement_letters_auto_enrolment.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5710 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/auto_enrolment/reenrol_auto_enrolment.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     8269 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/auto_enrolment/set_state_auto_enrolment.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:11.941758 staffology-0.1.4/staffology/api/benefits/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/benefits/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2441 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/benefits/create_benefits.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2280 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/benefits/delete_benefits.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3901 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/benefits/get_benefits.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3490 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/benefits/index_benefits.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4254 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/benefits/update_benefits.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:11.943839 staffology-0.1.4/staffology/api/billing/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/billing/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2668 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/billing/bill_billing.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2809 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/billing/bill_csv_billing.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2715 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/billing/bills_billing.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2324 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/billing/confirm_direct_debit_mandate_billing.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1646 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/billing/delete_direct_debit_mandate_billing.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2708 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/billing/direct_debit_mandate_billing.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5825 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/billing/get_usage_stats_billing.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3794 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/billing/setup_direct_debit_mandate_billing.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:11.945729 staffology-0.1.4/staffology/api/bureau/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/bureau/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4802 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/bureau/employers_bureau.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3397 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/bureau/get_processor_user_bureau.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3325 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/bureau/get_report_pack_bureau.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3026 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/bureau/get_settings_bureau.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2907 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/bureau/processor_users_bureau.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3715 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/bureau/update_settings_bureau.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:11.950047 staffology-0.1.4/staffology/api/cis_300/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/cis_300/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4217 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/cis_300/create_cis_300.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2209 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/cis_300/delete_cis_300.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3404 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/cis_300/get_cis_300.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3521 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/cis_300/list_cis_300.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4328 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/cis_300/mark_as_accepted_cis_300.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3346 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/cis_300/requiring_attention_cis_300.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3492 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/cis_300/submit_cis_300.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3873 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/cis_300/update_cis_300.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:11.952368 staffology-0.1.4/staffology/api/cis_verification/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/cis_verification/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4765 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/cis_verification/create_cis_verification.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2241 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/cis_verification/delete_cis_verification.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3679 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/cis_verification/get_cis_verification.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3667 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/cis_verification/list_cis_verification.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4527 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/cis_verification/mark_as_accepted_cis_verification.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3496 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/cis_verification/requiring_attention_cis_verification.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3755 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/cis_verification/submit_cis_verification.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5001 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/cis_verification/update_cis_verification.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:11.955070 staffology-0.1.4/staffology/api/department/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/department/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3758 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/department/create_department.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1978 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/department/delete_department.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3154 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/department/get_department.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3116 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/department/index_department.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3891 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/department/update_department.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:11.956856 staffology-0.1.4/staffology/api/dps/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/dps/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3445 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/dps/apply_dps.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3058 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/dps/check_for_notices_dps.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1759 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/dps/delete_all_dps.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1866 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/dps/delete_dps.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3098 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/dps/get_dps.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2964 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/dps/get_dps_settings_dps.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4316 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/dps/list_notices_dps.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3982 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/dps/parse_xml_dps.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3826 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/dps/update_dps_settings_dps.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:11.958509 staffology-0.1.4/staffology/api/email/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/email/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3286 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/email/get_email_email.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2983 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/email/get_mail_settings_email.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4442 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/email/index_email.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3247 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/email/resend_email_email.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3770 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/email/test_mail_settings_email.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4262 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/email/update_mail_settings_email.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2163 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/email/verify_mail_settings_email.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4179 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/email/verify_mail_settings_response_email.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:11.965847 staffology-0.1.4/staffology/api/employee/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/employee/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2848 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employee/apply_pay_increase_employee.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2631 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employee/apply_pay_options_employee.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5920 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employee/average_weekly_earnings_employee.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5396 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employee/base_daily_rate_employee.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5401 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employee/base_hourly_rate_employee.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4227 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employee/create_employee.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1874 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employee/delete_employee.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2270 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employee/delete_multiple_employee.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1868 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employee/delete_photo_employee.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4372 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employee/expiring_rtw_employee.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3412 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employee/get_department_memberships_employee.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2942 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employee/get_employee.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6463 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employee/import_csv_employee.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6677 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employee/index_employee.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4092 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employee/leavers_employee.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3286 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employee/mark_as_leavers_employee.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4720 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employee/minimum_wage_employee.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3899 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employee/pay_run_entries_employee.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2184 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employee/re_hire_employee.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3933 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employee/search_by_payroll_code_employee.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5236 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employee/search_employee.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4140 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employee/set_department_memberships_employee.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2789 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employee/set_on_hold_employee.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3835 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employee/update_employee.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4777 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employee/update_photo_employee.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:11.977551 staffology-0.1.4/staffology/api/employer/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/employer/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3835 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employer/apply_year_end_employer.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4781 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employer/calendar_employer.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3390 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employer/create_employer.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3014 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employer/custom_payslip_employer.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1627 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employer/delete_employer.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2917 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employer/get_automation_settings_employer.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2527 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employer/get_employer.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3024 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employer/get_employer_opening_balances_employer.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3042 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employer/get_group_memberships_employer.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4309 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employer/import_csv_employer.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3439 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employer/index_employer.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2990 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employer/list_users_employer.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2182 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employer/remove_user_employer.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3155 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employer/review_year_end_employer.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3203 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employer/rti_requiring_attention_employer.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4731 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employer/search_employees_employer.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3190 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employer/search_employer.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3797 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employer/set_group_memberships_employer.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2316 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employer/set_owner_employer.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3428 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employer/suggest_pay_code_employer.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3678 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employer/update_automation_settings_employer.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4166 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employer/update_custom_payslip_employer.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3214 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employer/update_employer.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3690 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employer/update_employer_opening_balances_employer.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4234 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employer/update_logo_employer.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:11.981219 staffology-0.1.4/staffology/api/employer_group/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/employer_group/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3320 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employer_group/create_employer_group.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1748 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employer_group/delete_employer_group.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3044 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employer_group/get_employer_group.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2674 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employer_group/index_employer_group.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3320 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employer_group/update_employer_group.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:11.981850 staffology-0.1.4/staffology/api/employer_template/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/employer_template/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3546 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employer_template/get_employer_template.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3206 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employer_template/index_employer_template.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4949 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/employer_template/update_employer_template.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:11.984955 staffology-0.1.4/staffology/api/engine/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/engine/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6709 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/engine/calculate_ni_engine.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)    10355 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/engine/calculate_tax_engine.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2706 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/engine/config_engine.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     7051 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/engine/get_national_insurance_thresholds_engine.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2933 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/engine/get_tenant_branding_engine.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:11.989392 staffology-0.1.4/staffology/api/eps/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/eps/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3623 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/eps/create_eps.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2148 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/eps/delete_eps.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3469 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/eps/get_eps.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3590 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/eps/list_eps.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4373 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/eps/mark_as_accepted_eps.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4022 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/eps/recoverable_amounts_eps.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3427 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/eps/requiring_attention_eps.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3517 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/eps/submit_eps.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3871 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/eps/update_eps.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:11.994255 staffology-0.1.4/staffology/api/exb/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/exb/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3467 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/exb/annual_values_exb.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3685 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/exb/create_exb.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2148 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/exb/delete_exb.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3501 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/exb/get_exb.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3554 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/exb/list_exb.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4405 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/exb/mark_as_accepted_exb.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3455 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/exb/requiring_attention_exb.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3541 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/exb/submit_exb.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3895 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/exb/update_exb.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:12.003089 staffology-0.1.4/staffology/api/external_data/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/external_data/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5238 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/external_data/authorize_external_data.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3852 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/external_data/companies_external_data.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2226 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/external_data/disconnect_external_data.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4170 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/external_data/employee_external_data.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4304 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/external_data/employee_logs_external_data.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4259 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/external_data/employees_external_data.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2234 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/external_data/get_config_data_external_data.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2604 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/external_data/get_request_external_data.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4302 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/external_data/import_employees_external_data.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3640 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/external_data/list_external_data.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3686 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/external_data/nominal_codes_external_data.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6315 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/external_data/pension_contributions_csv_external_data.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6885 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/external_data/post_journal_external_data.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)    11133 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/external_data/post_payments_external_data.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2840 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/external_data/post_request_external_data.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3600 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/external_data/push_employees_external_data.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2877 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/external_data/push_p11_ds_external_data.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3220 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/external_data/push_p11d_external_data.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2631 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/external_data/push_p45_external_data.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3169 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/external_data/push_p60_external_data.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4406 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/external_data/push_payslips_external_data.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3108 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/external_data/push_pension_letter_external_data.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2496 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/external_data/respond_external_data.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2572 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/external_data/set_config_data_external_data.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3656 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/external_data/set_credentials_external_data.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3954 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/external_data/sync_all_employees_external_data.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4462 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/external_data/sync_employee_external_data.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3681 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/external_data/sync_leave_external_data.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5881 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/external_data/time_and_attendance_external_data.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5668 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/external_data/update_employee_external_data.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:12.006754 staffology-0.1.4/staffology/api/fps/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/fps/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3943 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/fps/create_fps.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2196 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/fps/delete_fps.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3465 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/fps/get_fps.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3574 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/fps/list_fps.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4345 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/fps/mark_as_accepted_fps.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4948 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/fps/most_recent_for_employee_fps.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3403 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/fps/requiring_attention_fps.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3505 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/fps/submit_fps.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3859 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/fps/update_fps.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:12.007947 staffology-0.1.4/staffology/api/hmrc_payment/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/hmrc_payment/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4966 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/hmrc_payment/bank_payment_hmrc_payment.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4133 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/hmrc_payment/get_hmrc_payment.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3678 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/hmrc_payment/index_hmrc_payment.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4933 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/hmrc_payment/update_hmrc_payment.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:12.009429 staffology-0.1.4/staffology/api/import_/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/import_/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2587 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/import_/create_payments_csv_mapping_import.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1999 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/import_/delete_payment_csv_mapping_import.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4070 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/import_/import_employee_pay_import.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3193 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/import_/list_payments_csv_mappings_import.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3772 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/import_/payments_csv_mapping_csv_file_import.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3297 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/import_/payments_csv_mapping_import.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4470 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/import_/update_payments_csv_mapping_import.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:12.010329 staffology-0.1.4/staffology/api/invitation/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/invitation/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2545 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/invitation/accept_invitation.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3998 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/invitation/create_invitation.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1953 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/invitation/delete_invitation.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3113 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/invitation/get_invitation.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3479 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/invitation/index_invitation.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:12.011973 staffology-0.1.4/staffology/api/leave/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/leave/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2723 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/leave/add_document_leave.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2534 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/leave/create_leave.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2553 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/leave/delete_document_leave.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2269 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/leave/delete_leave.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     7001 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/leave/find_linked_piw_leave.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4317 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/leave/get_document_leave.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3856 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/leave/get_leave.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3463 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/leave/index_leave.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4546 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/leave/update_leave.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:12.013688 staffology-0.1.4/staffology/api/loan/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/loan/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2714 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/loan/add_document_loan.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2437 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/loan/create_loan.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2549 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/loan/delete_document_loan.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2265 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/loan/delete_loan.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4309 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/loan/get_document_loan.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3835 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/loan/get_loan.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3507 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/loan/index_loan.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4340 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/loan/update_loan.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:12.015909 staffology-0.1.4/staffology/api/note/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/note/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2714 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/note/add_document_note.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2407 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/note/create_note.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2549 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/note/delete_document_note.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2265 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/note/delete_note.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4309 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/note/get_document_note.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3835 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/note/get_note.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3459 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/note/index_note.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4074 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/note/update_note.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:12.019245 staffology-0.1.4/staffology/api/nvr/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/nvr/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3631 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/nvr/create_nvr.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2148 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/nvr/delete_nvr.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3437 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/nvr/get_nvr.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3582 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/nvr/list_nvr.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4349 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/nvr/mark_as_accepted_nvr.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3427 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/nvr/requiring_attention_nvr.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3561 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/nvr/submit_nvr.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3867 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/nvr/update_nvr.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:12.021153 staffology-0.1.4/staffology/api/opening_balances/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/opening_balances/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5874 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/opening_balances/get_nic_summaries_opening_balances.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3700 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/opening_balances/get_opening_balances.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5580 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/opening_balances/update_nic_summaries_opening_balances.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4321 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/opening_balances/update_opening_balances.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6021 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/opening_balances/update_p45_opening_balances.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5777 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/opening_balances/update_termination_payments_opening_balances.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:12.026831 staffology-0.1.4/staffology/api/pay_code/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/pay_code/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4514 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_code/create_pay_code.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1963 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_code/delete_pay_code.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3089 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_code/get_pay_code.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3884 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_code/index_pay_code.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3418 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_code/nominal_code_mappings_pay_code.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4144 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_code/update_nominal_code_mappings_pay_code.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4679 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_code/update_pay_code.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:12.043822 staffology-0.1.4/staffology/api/pay_run/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/pay_run/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5718 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_run/aeo_pay_run.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     7194 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_run/changes_for_pay_run_entry_pay_run.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5544 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_run/changes_pay_run.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4578 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_run/create_next_pay_run_pay_run.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3089 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_run/delete_pay_run.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     7449 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_run/finalise_pay_run_pay_run.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5079 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_run/get_pay_run_entry_pay_run.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5282 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_run/get_pay_run_events_pay_run.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5928 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_run/get_pay_run_journal_pay_run.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5099 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_run/get_pay_run_pay_codes_pay_run.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4812 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_run/get_pay_run_pay_run.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5703 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_run/get_pay_run_warnings_pay_run.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4534 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_run/get_pay_runs_pay_run.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5122 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_run/import_pay_pay_run.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6620 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_run/import_time_and_attendance_pay_run.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5897 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_run/import_umbrella_pay_pay_run.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3317 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_run/last_pay_run_entry_for_employee_pay_run.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6420 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_run/leave_pay_run.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6322 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_run/pay_run_entry_umbrella_payment_pay_run.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6228 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_run/re_open_pay_run_pay_run.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3411 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_run/send_payslip_emails_pay_run.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2978 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_run/start_next_pay_run_pay_run.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     7850 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_run/update_pay_run_entry_pay_run.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6879 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_run/update_pay_run_pay_run.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6303 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_run/update_payment_date_pay_run.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6362 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_run/ytd_pay_run.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5517 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_run/zeroise_pay_run_entries_pay_run.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:12.053215 staffology-0.1.4/staffology/api/pay_schedule/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/pay_schedule/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2985 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_schedule/create_pay_schedule.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3423 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_schedule/create_with_optional_ordinal_pay_schedule.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2682 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_schedule/delete_pay_schedule.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3076 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_schedule/delete_with_optional_ordinal_pay_schedule.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3632 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_schedule/get_all_pay_schedule.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4340 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_schedule/get_pay_schedule.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6344 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_schedule/get_periods_pay_schedule.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4968 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_schedule/get_with_optional_ordinal_pay_schedule.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4962 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_schedule/save_pay_schedule.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5671 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_schedule/save_with_optional_ordinal_pay_schedule.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5649 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pay_schedule/update_pay_schedule_period_pay_schedule.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:12.060853 staffology-0.1.4/staffology/api/payee/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/payee/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3603 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/payee/create_payee.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1929 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/payee/delete_payee.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3004 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/payee/get_payee.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3071 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/payee/index_payee.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3696 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/payee/update_payee.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:12.061566 staffology-0.1.4/staffology/api/pension/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/pension/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3303 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pension/get_pension.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2452 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pension/remove_pension.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4052 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pension/update_pension.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:12.067273 staffology-0.1.4/staffology/api/pension_scheme/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/pension_scheme/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5861 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pension_scheme/contributions_for_payrun_pension_scheme.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4737 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pension_scheme/contributions_pension_scheme.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3549 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pension_scheme/create_pension_scheme.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1887 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pension_scheme/delete_pension_scheme.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3430 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pension_scheme/employees_pension_scheme.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3029 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pension_scheme/get_pension_scheme.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2951 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pension_scheme/index_pension_scheme.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4620 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pension_scheme/list_contributions_pension_scheme.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4289 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pension_scheme/mark_as_sent_pension_scheme.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2567 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pension_scheme/resubmit_contributions_pension_scheme.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3761 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/pension_scheme/update_pension_scheme.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:12.068880 staffology-0.1.4/staffology/api/post/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/post/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4656 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/post/create_post.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2447 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/post/delete_post.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4302 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/post/get_post.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4382 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/post/index_post.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4852 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/post/update_post.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:12.070125 staffology-0.1.4/staffology/api/processing_note/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/processing_note/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2558 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/processing_note/add_document_processing_note.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6258 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/processing_note/create_processing_note.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2324 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/processing_note/delete_document_processing_note.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3956 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/processing_note/get_document_processing_note.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5145 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/processing_note/get_processing_note.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5787 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/processing_note/list_processing_note.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:12.071613 staffology-0.1.4/staffology/api/report_pack/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/report_pack/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3997 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/report_pack/create_report_pack.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1956 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/report_pack/delete_report_pack.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3117 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/report_pack/get_report_pack.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3118 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/report_pack/index_report_pack.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4090 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/report_pack/update_report_pack.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:12.081527 staffology-0.1.4/staffology/api/reports/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/reports/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4088 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/ae_assessments_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4848 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/aeo_statement_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     7121 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/analysis_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     9954 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/bank_payment_instructions_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4234 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/cis_300_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5309 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/cis_statement_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4100 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/cis_sub_contractor_summary_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6691 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/cost_analysis_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6864 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/cost_of_employment_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2400 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/email_p45_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3177 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/email_p60_multiple_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2761 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/email_p60_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5093 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/employee_benefits_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     8415 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/employee_export_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3598 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/employer_export_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5590 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/example_payslip_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4091 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/exb_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4969 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/fps_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6195 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/full_summary_of_pay_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5731 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/furlough_report_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     7250 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/get_pay_run_csv_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     7304 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/gross_to_net_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4476 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/holiday_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6697 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/hourly_pay_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6146 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/ni_letter_validation_report_employees_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6104 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/ni_letter_validation_report_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5190 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/p11_detailed_multiple_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4551 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/p11_detailed_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4510 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/p11_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4667 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/p11d_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5556 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/p30_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4066 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/p32_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4332 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/p45_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6365 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/p60_multiple_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4658 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/p60_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6537 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/papdis_file_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6485 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/pay_run_csv_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     7667 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/pay_run_payments_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     8391 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/pay_run_summary_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5825 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/payrun_ytd_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6187 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/payslip_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     7169 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/payslips_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3892 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/right_to_work_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6753 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/statutory_pay_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4334 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/tax_code_changes_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     7400 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/umbrella_reconciliation_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)    12086 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/variance_report_reports.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3953 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/reports/ytd_reports.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:12.082984 staffology-0.1.4/staffology/api/tag/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/tag/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3438 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tag/create_tag.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1943 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tag/delete_tag.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3000 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tag/get_tag.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3053 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tag/index_tag.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3438 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tag/update_tag.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:12.090119 staffology-0.1.4/staffology/api/tenant/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/tenant/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1974 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tenant/add_admin_user_tenant.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2947 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tenant/admin_users_tenant.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3620 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tenant/bill_tenant.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3616 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tenant/bills_tenant.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4390 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tenant/create_bills_tenant.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4300 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tenant/create_tenant.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2640 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tenant/disabled_tenant.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2469 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tenant/employer_creation_tenant.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3359 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tenant/employer_usage_tenant.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3347 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tenant/employer_users_tenant.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3880 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tenant/get_rti_submission_settings_tenant.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2939 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tenant/get_tenant.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4361 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tenant/get_users_with_no_billable_activity_tenant.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1976 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tenant/remove_admin_user_tenant.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2475 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tenant/set_accounting_id_tenant.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2546 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tenant/set_bureau_redirect_email_address_tenant.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2310 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tenant/set_monthly_minimum_tenant.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2929 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tenant/set_omnipresent_role_tenant.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2526 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tenant/set_tenant_tenant.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3944 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tenant/update_bill_tenant.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3963 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tenant/update_css_colors_tenant.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2963 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tenant/update_css_tenant.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3840 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tenant/update_fav_icon_tenant.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3822 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tenant/update_logo_tenant.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4685 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tenant/update_rti_submission_settings_tenant.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4624 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tenant/update_tenant.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3572 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tenant/usage_tenant.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3219 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tenant/user_bills_tenant.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3355 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tenant/user_employers_tenant.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3020 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tenant/user_tenant.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3583 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tenant/users_search_tenant.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5788 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tenant/users_tenant.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6032 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tenant/weekly_activity_tenant.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:12.091209 staffology-0.1.4/staffology/api/tenant_email/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/tenant_email/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3080 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tenant_email/get_email_tenant_email.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2777 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tenant_email/get_mail_settings_tenant_email.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4240 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tenant_email/index_tenant_email.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3045 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tenant_email/resend_email_tenant_email.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3576 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tenant_email/test_mail_settings_tenant_email.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4056 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/tenant_email/update_mail_settings_tenant_email.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:12.092726 staffology-0.1.4/staffology/api/webhook/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/webhook/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2138 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/webhook/create_webhook.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1939 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/webhook/delete_webhook.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3048 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/webhook/get_webhook.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3089 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/webhook/index_webhook.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3652 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/webhook/payload_webhook.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4711 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/webhook/payloads_webhook.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2296 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/webhook/sample_webhook.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3522 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/webhook/update_webhook.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:12.094637 staffology-0.1.4/staffology/api/working_pattern/
--rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/api/working_pattern/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3895 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/working_pattern/create_working_pattern.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1974 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/working_pattern/delete_working_pattern.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3203 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/working_pattern/get_working_pattern.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3192 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/working_pattern/index_working_pattern.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4020 2022-11-20 17:35:39.000000 staffology-0.1.4/staffology/api/working_pattern/update_working_pattern.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1821 2022-10-22 17:54:53.000000 staffology-0.1.4/staffology/client.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:12.225098 staffology-0.1.4/staffology/models/
--rw-r--r--   0 isikkaplan   (501) staff       (20)    21567 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/__init__.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2449 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/add_document_attachment_order_multipart_data.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2396 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/add_document_leave_multipart_data.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2391 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/add_document_loan_multipart_data.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2391 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/add_document_note_multipart_data.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2444 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/add_document_processing_note_multipart_data.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2954 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/address.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      536 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/ae_action.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     8144 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/ae_assessment.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4933 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/ae_assessment_action.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      661 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/ae_employee_state.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      670 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/ae_exclusion_code.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      498 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/ae_status.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      453 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/ae_statutory_letter.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      451 2022-11-15 11:04:28.000000 staffology-0.1.4/staffology/models/ae_uk_worker.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     7439 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/analysis_report.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4485 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/analysis_report_line.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1288 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/analysis_report_line_value.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2105 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/analysis_report_report_response.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1245 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/apply_year_end_employer_json_body.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)    14648 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/attachment_order.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     8352 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/attachment_order_payment.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2171 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/attachment_order_report_response.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      526 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/attachment_order_type.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      187 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/audit_event_action.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      299 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/auth_scheme.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     7538 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/auto_enrolment.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     9087 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/auto_enrolment_settings.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      280 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/auto_pilot_finalise_time.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)    11651 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/automation_settings.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5908 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/average_weekly_earnings.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      308 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/average_weekly_earnings_result.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      217 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/background_task_status.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2663 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/bank_details.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      250 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/bank_holiday_collection.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4510 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/bank_payment_instruction.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2188 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/bank_payment_instruction_report_response.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      978 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/bank_payment_instructions_csv_format.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)    10745 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/benefit.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      438 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/benefit_declaration_type.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      256 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/benefit_details_asset_type.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)    13095 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/benefit_details_car.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      259 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/benefit_details_car_power_type.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      661 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/benefit_details_class_1a_type.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5487 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/benefit_details_loan.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      640 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/benefit_details_non_class_1a_type.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      651 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/benefit_details_payment_type.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      652 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/benefit_details_use_of_asset_type.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      926 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/benefit_type.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3523 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/bureau_settings.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2426 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/calendar_entry.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      639 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/calendar_entry_type.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     7108 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/car_charge.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1626 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/car_charge_rate.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6614 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/change_summary.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6666 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/cis_300.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1963 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/cis_300_declarations.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2025 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/cis_300_report_response.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1112 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/cis_contractor.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4562 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/cis_details.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1191 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/cis_partnership.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2710 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/cis_request.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3440 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/cis_return.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     7140 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/cis_statement.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2491 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/cis_statement_list_report_response.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)    10729 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/cis_sub_contractor.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4957 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/cis_sub_contractor_summary.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2596 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/cis_sub_contractor_summary_list_report_response.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      231 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/cis_sub_contractor_type.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      241 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/cis_tax_status.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6646 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/cis_verification.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4340 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/cis_verification_details.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      847 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/cookie_preference.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)    10798 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/cost_analysis_report.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2148 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/cost_analysis_report_report_response.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1768 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/cost_breakdown.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1232 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/cost_breakdown_breakdown.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     7248 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/cost_of_employment_report.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3517 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/cost_of_employment_report_line.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2191 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/cost_of_employment_report_report_response.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      539 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/country.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      354 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/csv_file_format.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      487 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/deferal_period_type.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2003 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/department.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2312 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/department_membership.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2475 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/direct_debit_mandate.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2786 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/directorship_details.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      274 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/dps_data_type.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     7871 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/dps_notice.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3293 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/dps_settings.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1931 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/email_attachment.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2108 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/emp_refs.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     8573 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/employee.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1703 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/employee_benefits_report.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2188 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/employee_benefits_report_report_response.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      191 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/employee_status.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2912 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/employee_ytd_values.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)    17518 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/employer.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3973 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/employer_defaults.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6470 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/employer_email.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1554 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/employer_group.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1819 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/employer_group_membership.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2226 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/employer_item.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5945 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/employer_opening_balances.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1021 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/employer_settings.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4969 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/employer_template.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      777 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/employer_template_type.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)    16647 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/employment_details.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      894 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/entity_type.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)    10088 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/eps.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1936 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/eps_account.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1533 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/eps_apprenticeship_levy.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1753 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/eps_de_minimis_state_aid.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2206 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/eps_final_submission.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     7921 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/exb.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1297 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/exb_declarations.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      770 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/exb_employer.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1532 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/exb_p11_db.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2767 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/exb_p11_db_class_1a.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1212 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/exb_p11_db_class_1a_adjustment.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2951 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/exb_p11_db_class_1a_adjustments.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1253 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/exb_p11_db_class_1a_total_benefit.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)    10408 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/exb_p11d.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2824 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/exb_p11d_employee.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1992 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/exb_report_response.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4481 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/expenses_and_benefits.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1547 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/external_data_company.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4412 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/external_data_provider.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      927 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/external_data_provider_id.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      319 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/external_data_provider_type.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4873 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/external_employee_mapping.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      503 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/external_employee_mapping_status.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2999 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/external_provider_conversation.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1767 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/field_modification.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1248 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/finalise_pay_run_pay_run_json_body.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1273 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/fixed_code.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     7793 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/fps.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1293 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/fps_benefit.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4213 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/fps_car.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1401 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/fps_car_fuel.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4218 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/fps_employee.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3878 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/fps_employee_details.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1445 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/fps_employee_details_partner_details.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)    11375 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/fps_employee_figs_to_date.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2362 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/fps_employee_flexible_drawdown.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4394 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/fps_employee_n_iletters_and_values.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)    15255 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/fps_employee_payment.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2594 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/fps_employee_starter.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1145 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/fps_employee_starter_occ_pension.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1550 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/fps_employee_tax_code.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1122 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/fps_employee_trivial_commutation_payment.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1423 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/fps_employer_pay_id_changed.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     8173 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/fps_employment.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2764 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/fps_fields.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      691 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/fps_late_reason.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1992 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/fps_report_response.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1581 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/from_to_dates.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1863 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/full_payment_submission.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     7731 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/full_summary_of_pay_report.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2432 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/full_summary_of_pay_report_line.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2194 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/full_summary_of_pay_report_report_response.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      550 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/furlough_calculation_basis.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)    19604 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/furlough_report.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     8079 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/furlough_report_line.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2105 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/furlough_report_report_response.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      426 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/gender.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4308 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/gov_talk.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1835 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/gov_talk_error.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6204 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/gov_talk_submission.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     7803 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/gross_to_net_report.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4073 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/gross_to_net_report_cis_line.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5622 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/gross_to_net_report_line.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2131 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/gross_to_net_report_report_response.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     7462 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/hmrc_details.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)    22294 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/hmrc_liability.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1583 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/hmrc_payment.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3472 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/holiday_report.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2804 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/holiday_report_line.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2095 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/holiday_report_report_response.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      204 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/holiday_type.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6529 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/hourly_pay_report.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2707 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/hourly_pay_report_line.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2118 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/hourly_pay_report_report_response.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      274 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/hours_normally_worked.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2226 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/html_email_settings.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      476 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/html_insertion_point.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2401 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/import_csv_employee_multipart_data.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2401 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/import_csv_employer_multipart_data.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4206 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/invitation.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1432 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/item.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2416 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/item_list_report_response.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)    18608 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/leave.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      207 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/leave_pay_type.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)    17264 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/leave_settings.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      715 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/leave_type.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2576 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/leaver_details.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4722 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/linked_piw.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      455 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/linked_piw_result.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6632 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/loan.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1503 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/loan_charge.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1350 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/log_entry.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4885 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/mail_settings.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      555 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/marital_status.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2518 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/mileage_allowance_payments_rate.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      189 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/mileage_vehicle_type.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2985 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/monthly_minimum.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)    10563 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/national_insurance_calculation.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     9403 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/national_insurance_calculation_base.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3276 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/national_insurance_calculation_period_values.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4270 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/national_insurance_code.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1715 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/national_minimum_wage.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1563 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/ni_letter_error.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     8009 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/ni_letter_validation_report.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4737 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/ni_letter_validation_report_line.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2211 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/ni_letter_validation_report_report_response.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     7633 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/nic_summary.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2253 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/nominal_code_mapping.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4920 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/note.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      227 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/note_type.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5406 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/nvr.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2924 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/nvr_employee.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2600 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/nvr_employee_details.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      798 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/nvr_employment.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1817 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/nvr_request.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     9634 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/opening_balances.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2597 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/overseas_employer_details.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      526 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/overseas_secondment_status.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     7444 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/p11.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)    13456 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/p11_detailed.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4193 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/p11_detailed_ni_values.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2292 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/p11_detailed_report_response.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5743 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/p11_line.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4870 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/p11_ni_and_stat_payments_line.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3753 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/p11_ni_and_stat_payments_totals_line.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1313 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/p11_ni_values.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4330 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/p11_paye_line.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3055 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/p11_paye_summary.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2516 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/p11_paye_totals_line.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2248 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/p11_report_response.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2963 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/p11d_asset_available.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1795 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/p11d_asset_available_collection.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1778 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/p11d_asset_transferred_collection.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5955 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/p11d_car.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2577 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/p11d_car_collection.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1140 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/p11d_car_free_fuel_withdrawn.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2943 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/p11d_desc_other.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3887 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/p11d_expenses.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2838 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/p11d_loan.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1675 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/p11d_loan_collection.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3027 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/p11d_other.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2018 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/p11d_payment_collection.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4656 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/p11d_single_item.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5152 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/p11d_vans.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3103 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/p32.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1992 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/p32_report_response.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4957 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/papdis_document.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2592 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/papdis_document_report_response.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5579 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/papdis_employee.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     7264 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/papdis_employee_assessment.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2290 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/papdis_employee_contact.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2362 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/papdis_employee_contact_postal_address.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4570 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/papdis_employee_contribution.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2886 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/papdis_employee_exit.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3137 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/papdis_employee_identity.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1703 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/papdis_employee_name.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1728 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/papdis_employee_pay.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4907 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/papdis_employer.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      583 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/papdis_message_function_code.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6528 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/papdis_payroll_period.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2024 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/papdis_pension_provider.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      433 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/papdis_version.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1701 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/partner_details.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      454 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/pay_basis.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)    12649 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/pay_code.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      616 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/pay_code_calculation_type.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      182 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/pay_code_multiplier_type.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     8471 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/pay_line.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      483 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/pay_method.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)    11290 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/pay_options.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5028 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/pay_options_import.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      323 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/pay_period_event_type.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      265 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/pay_periods.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)    10817 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/pay_run.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1746 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/pay_run_changes.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2183 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/pay_run_cost_summary.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      533 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/pay_run_csv_type.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)    27061 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/pay_run_entry.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5434 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/pay_run_journal.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5017 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/pay_run_payment.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      589 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/pay_run_state.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2351 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/pay_run_state_change.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      298 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/pay_run_state_change_reason.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3787 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/pay_run_summary_line.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2572 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/pay_run_summary_line_i_enumerable_report_response.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)    26077 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/pay_run_totals.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)    14562 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/pay_schedule.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5767 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/pay_schedule_period.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3970 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/pay_schedule_period_event.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2674 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/pay_schedule_period_events_config.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1662 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/payee.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      517 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/payee_type.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      553 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/payment_date_type.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6160 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/payments_csv_mapping.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3052 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/payments_csv_mapping_column.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      185 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/payments_csv_mapping_type.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2199 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/payroll_value_type.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)    10079 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/payrun_email.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     8168 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/payrun_payments_report.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2356 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/payrun_payments_report_report_response.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)    12529 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/payslip.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     8097 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/payslip_customisation.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6232 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/payslip_line.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      505 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/payslip_line_type.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2248 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/payslip_report_response.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1483 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/pdf_paper_margins.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      178 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/pdf_paper_orientation.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      498 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/pdf_paper_size.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      206 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/pdf_password_type.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)    15515 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/pension.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2172 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/pension_administrator.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      253 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/pension_contribution_level_type.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5147 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/pension_contributions_submission.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      285 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/pension_csv_format.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     9278 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/pension_provider.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      238 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/pension_rule.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)    10459 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/pension_scheme.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2248 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/pension_selection.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)    10702 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/pension_summary.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1719 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/pensioner_payroll.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     8780 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/personal_details.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1940 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/post.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      515 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/pro_rata_rule.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4338 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/processing_note.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6041 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/recoverable_amounts.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1522 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/report.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      234 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/report_custom_css_option.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1930 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/report_pack.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1809 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/report_response.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3041 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/right_to_work.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      571 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/right_to_work_document_type.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3170 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/right_to_work_report.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2512 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/right_to_work_report_line.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2141 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/right_to_work_report_report_response.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      213 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/role.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2266 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/rti_agent.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1654 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/rti_contact.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2526 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/rti_employee_address.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1742 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/rti_employee_name.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      659 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/rti_sender_type.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6101 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/rti_submission_settings.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1499 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/rti_validation_warning.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      474 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/rti_validation_warning_type.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      169 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/smtp_encryption.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2451 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/smtp_settings.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      458 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/starter_declaration.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3151 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/starter_details.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2176 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/statutory_pay.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6556 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/statutory_pay_report.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3230 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/statutory_pay_report_line.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2148 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/statutory_pay_report_report_response.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1063 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/string_string_key_value_pair.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      483 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/student_loan.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1107 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/student_loan_recovered.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      520 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/submission_status.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1194 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/tag.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     7740 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/tax_and_ni.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1407 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/tax_bracket.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1523 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/tax_code_change.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2577 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/tax_code_change_report.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2161 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/tax_code_change_report_report_response.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3712 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/tax_code_change_values.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      268 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/tax_year.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2365 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/teachers_pension_details.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      294 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/teachers_pension_employment_type.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)    11499 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/tenant.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1941 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/tenant_billing_settings.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6462 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/tenant_email.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1612 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/tenant_html_insertion.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1631 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/tenant_item.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2738 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/tiered_pension.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1913 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/tiered_pension_rate.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3873 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/umbrella_payment.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6655 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/umbrella_reconciliation_report.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6174 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/umbrella_reconciliation_report_line.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2248 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/umbrella_reconciliation_report_report_response.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4094 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/umbrella_settings.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2414 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/update_fav_icon_tenant_multipart_data.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2406 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/update_logo_employer_multipart_data.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2396 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/update_logo_tenant_multipart_data.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2406 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/update_photo_account_multipart_data.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2411 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/update_photo_employee_multipart_data.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     6030 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/usage_bill.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)    21914 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/user.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2772 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/user_authorization.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      439 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/user_category.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     8130 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/user_display_preferences.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1364 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/user_industry.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      581 2022-11-15 11:04:53.000000 staffology-0.1.4/staffology/models/user_job_type.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      294 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/userstart_page.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1815 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/utm_info.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2939 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/value_override.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     7374 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/variance_report.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2105 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/variance_report_report_response.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2244 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/veteran_details.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3044 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/webhook.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      285 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/webhook_event.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     4062 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/webhook_payload.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     7711 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/worker_group.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     5505 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/working_pattern.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)    10176 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/year_end.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1912 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/year_end_tax_code_change.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2361 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/ytd_pay_run_multipart_data.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     3216 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/ytd_report.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     2055 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/ytd_report_report_response.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)     1923 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/models/ytd_value.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      274 2022-11-21 10:10:39.000000 staffology-0.1.4/staffology/propagate_exceptions.py
--rw-r--r--   0 isikkaplan   (501) staff       (20)      939 2022-10-16 21:45:52.000000 staffology-0.1.4/staffology/types.py
-drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2022-11-21 10:11:11.928114 staffology-0.1.4/staffology.egg-info/
--rw-r--r--   0 isikkaplan   (501) staff       (20)      524 2022-11-21 10:11:11.000000 staffology-0.1.4/staffology.egg-info/PKG-INFO
--rw-r--r--   0 isikkaplan   (501) staff       (20)    41463 2022-11-21 10:11:11.000000 staffology-0.1.4/staffology.egg-info/SOURCES.txt
--rw-r--r--   0 isikkaplan   (501) staff       (20)        1 2022-11-21 10:11:11.000000 staffology-0.1.4/staffology.egg-info/dependency_links.txt
--rw-r--r--   0 isikkaplan   (501) staff       (20)       12 2022-11-21 10:11:11.000000 staffology-0.1.4/staffology.egg-info/requires.txt
--rw-r--r--   0 isikkaplan   (501) staff       (20)       11 2022-11-21 10:11:11.000000 staffology-0.1.4/staffology.egg-info/top_level.txt
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.500973 staffology-0.1.5/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      524 2023-04-19 11:49:50.500214 staffology-0.1.5/PKG-INFO
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      135 2022-10-21 20:55:55.000000 staffology-0.1.5/README.md
+-rw-r--r--   0 isikkaplan   (501) staff       (20)       38 2023-04-19 11:49:50.501040 staffology-0.1.5/setup.cfg
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      666 2023-04-19 11:48:15.000000 staffology-0.1.5/setup.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.329784 staffology-0.1.5/staffology/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      167 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/__init__.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.330659 staffology-0.1.5/staffology/api/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)       47 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/__init__.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.334066 staffology-0.1.5/staffology/api/account/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/account/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4467 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/account/activate_account.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4029 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/account/change_email_address_account.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3201 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/account/create_api_key_account.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1579 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/account/create_demo_employer_account.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1620 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/account/delete_api_key_account.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3846 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/account/get_account.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2458 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/account/get_api_key_account.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2674 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/account/get_employer_defaults_account.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3653 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/account/get_invitations_account.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4011 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/account/get_tenant_account.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2462 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/account/list_api_keys_account.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4020 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/account/profile_account.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4165 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/account/set_employer_defaults_account.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3190 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/account/update_cookie_preferences_account.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3600 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/account/update_photo_account.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1905 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/account/verify_account.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3581 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/account/verify_response_account.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.335715 staffology-0.1.5/staffology/api/attachment_order/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/attachment_order/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2810 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/attachment_order/add_document_attachment_order.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2572 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/attachment_order/create_attachment_order.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2344 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/attachment_order/delete_attachment_order.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2604 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/attachment_order/delete_document_attachment_order.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4114 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/attachment_order/get_attachment_order.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4408 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/attachment_order/get_document_attachment_order.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3562 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/attachment_order/index_attachment_order.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4366 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/attachment_order/payments_attachment_order.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4674 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/attachment_order/update_attachment_order.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.335960 staffology-0.1.5/staffology/api/audit/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/audit/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     7628 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/audit/employer_audit_list_audit.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.338185 staffology-0.1.5/staffology/api/auto_enrolment/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/auto_enrolment/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3787 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/auto_enrolment/assess_auto_enrolment.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2321 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/auto_enrolment/delete_auto_enrolment.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4015 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/auto_enrolment/email_letter_auto_enrolment.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3692 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/auto_enrolment/get_auto_enrolment.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3468 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/auto_enrolment/get_last_auto_enrolment.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4847 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/auto_enrolment/get_letter_auto_enrolment.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3591 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/auto_enrolment/list_auto_enrolment.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2522 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/auto_enrolment/mark_letter_as_sent_auto_enrolment.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3234 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/auto_enrolment/pending_letters_auto_enrolment.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3743 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/auto_enrolment/pending_postponement_letters_auto_enrolment.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5710 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/auto_enrolment/reenrol_auto_enrolment.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     8269 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/auto_enrolment/set_state_auto_enrolment.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.339234 staffology-0.1.5/staffology/api/benefits/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/benefits/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2441 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/benefits/create_benefits.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2280 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/benefits/delete_benefits.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3901 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/benefits/get_benefits.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3490 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/benefits/index_benefits.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4254 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/benefits/update_benefits.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.340858 staffology-0.1.5/staffology/api/billing/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/billing/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2668 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/billing/bill_billing.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2809 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/billing/bill_csv_billing.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2715 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/billing/bills_billing.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2324 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/billing/confirm_direct_debit_mandate_billing.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1646 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/billing/delete_direct_debit_mandate_billing.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2708 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/billing/direct_debit_mandate_billing.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5825 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/billing/get_usage_stats_billing.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3794 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/billing/setup_direct_debit_mandate_billing.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.342017 staffology-0.1.5/staffology/api/bureau/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/bureau/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4802 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/bureau/employers_bureau.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3397 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/bureau/get_processor_user_bureau.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3325 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/bureau/get_report_pack_bureau.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3026 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/bureau/get_settings_bureau.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2907 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/bureau/processor_users_bureau.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3715 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/bureau/update_settings_bureau.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.343307 staffology-0.1.5/staffology/api/cis_300/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/cis_300/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4217 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/cis_300/create_cis_300.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2209 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/cis_300/delete_cis_300.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3404 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/cis_300/get_cis_300.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3521 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/cis_300/list_cis_300.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4328 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/cis_300/mark_as_accepted_cis_300.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3346 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/cis_300/requiring_attention_cis_300.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3492 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/cis_300/submit_cis_300.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3873 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/cis_300/update_cis_300.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.344728 staffology-0.1.5/staffology/api/cis_verification/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/cis_verification/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4765 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/cis_verification/create_cis_verification.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2241 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/cis_verification/delete_cis_verification.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3679 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/cis_verification/get_cis_verification.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3667 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/cis_verification/list_cis_verification.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4527 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/cis_verification/mark_as_accepted_cis_verification.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3496 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/cis_verification/requiring_attention_cis_verification.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3755 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/cis_verification/submit_cis_verification.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5001 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/cis_verification/update_cis_verification.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.345567 staffology-0.1.5/staffology/api/department/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/department/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3758 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/department/create_department.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1978 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/department/delete_department.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3154 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/department/get_department.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3116 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/department/index_department.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3891 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/department/update_department.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.349783 staffology-0.1.5/staffology/api/dps/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/dps/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3445 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/dps/apply_dps.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3058 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/dps/check_for_notices_dps.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1759 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/dps/delete_all_dps.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1866 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/dps/delete_dps.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3098 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/dps/get_dps.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2964 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/dps/get_dps_settings_dps.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4316 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/dps/list_notices_dps.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3982 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/dps/parse_xml_dps.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3826 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/dps/update_dps_settings_dps.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.351158 staffology-0.1.5/staffology/api/email/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/email/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3286 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/email/get_email_email.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2983 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/email/get_mail_settings_email.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4442 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/email/index_email.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3247 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/email/resend_email_email.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3770 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/email/test_mail_settings_email.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4262 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/email/update_mail_settings_email.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2163 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/email/verify_mail_settings_email.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4179 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/email/verify_mail_settings_response_email.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.355594 staffology-0.1.5/staffology/api/employee/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/employee/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2848 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employee/apply_pay_increase_employee.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2631 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employee/apply_pay_options_employee.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5920 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employee/average_weekly_earnings_employee.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5396 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employee/base_daily_rate_employee.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5401 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employee/base_hourly_rate_employee.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4227 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employee/create_employee.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1874 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employee/delete_employee.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2270 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employee/delete_multiple_employee.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1868 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employee/delete_photo_employee.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4372 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employee/expiring_rtw_employee.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3412 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employee/get_department_memberships_employee.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2942 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employee/get_employee.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6463 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employee/import_csv_employee.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6677 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employee/index_employee.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4092 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employee/leavers_employee.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3286 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employee/mark_as_leavers_employee.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4720 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employee/minimum_wage_employee.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3899 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employee/pay_run_entries_employee.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2184 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employee/re_hire_employee.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3933 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employee/search_by_payroll_code_employee.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5236 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employee/search_employee.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4140 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employee/set_department_memberships_employee.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2789 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employee/set_on_hold_employee.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3835 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employee/update_employee.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4777 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employee/update_photo_employee.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.360875 staffology-0.1.5/staffology/api/employer/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/employer/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3835 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employer/apply_year_end_employer.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4781 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employer/calendar_employer.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3390 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employer/create_employer.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3014 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employer/custom_payslip_employer.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1627 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employer/delete_employer.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2917 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employer/get_automation_settings_employer.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2527 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employer/get_employer.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3024 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employer/get_employer_opening_balances_employer.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3042 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employer/get_group_memberships_employer.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4309 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employer/import_csv_employer.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3439 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employer/index_employer.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2990 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employer/list_users_employer.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2182 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employer/remove_user_employer.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3155 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employer/review_year_end_employer.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3203 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employer/rti_requiring_attention_employer.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4731 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employer/search_employees_employer.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3190 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employer/search_employer.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3797 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employer/set_group_memberships_employer.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2316 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employer/set_owner_employer.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3428 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employer/suggest_pay_code_employer.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3678 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employer/update_automation_settings_employer.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4166 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employer/update_custom_payslip_employer.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3214 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employer/update_employer.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3690 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employer/update_employer_opening_balances_employer.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4234 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employer/update_logo_employer.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.362367 staffology-0.1.5/staffology/api/employer_group/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/employer_group/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3320 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employer_group/create_employer_group.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1748 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employer_group/delete_employer_group.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3044 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employer_group/get_employer_group.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2674 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employer_group/index_employer_group.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3320 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employer_group/update_employer_group.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.363059 staffology-0.1.5/staffology/api/employer_template/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/employer_template/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3546 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employer_template/get_employer_template.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3206 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employer_template/index_employer_template.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4949 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/employer_template/update_employer_template.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.364054 staffology-0.1.5/staffology/api/engine/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/engine/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6709 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/engine/calculate_ni_engine.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)    10355 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/engine/calculate_tax_engine.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2706 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/engine/config_engine.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     7051 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/engine/get_national_insurance_thresholds_engine.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2933 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/engine/get_tenant_branding_engine.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.365604 staffology-0.1.5/staffology/api/eps/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/eps/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3623 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/eps/create_eps.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2148 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/eps/delete_eps.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3469 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/eps/get_eps.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3590 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/eps/list_eps.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4373 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/eps/mark_as_accepted_eps.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4022 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/eps/recoverable_amounts_eps.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3427 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/eps/requiring_attention_eps.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3517 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/eps/submit_eps.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3871 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/eps/update_eps.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.367063 staffology-0.1.5/staffology/api/exb/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/exb/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3467 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/exb/annual_values_exb.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3685 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/exb/create_exb.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2148 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/exb/delete_exb.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3501 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/exb/get_exb.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3554 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/exb/list_exb.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4405 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/exb/mark_as_accepted_exb.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3455 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/exb/requiring_attention_exb.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3541 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/exb/submit_exb.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3895 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/exb/update_exb.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.378445 staffology-0.1.5/staffology/api/external_data/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/external_data/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5238 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/external_data/authorize_external_data.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3852 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/external_data/companies_external_data.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2226 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/external_data/disconnect_external_data.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4170 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/external_data/employee_external_data.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4304 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/external_data/employee_logs_external_data.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4259 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/external_data/employees_external_data.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2234 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/external_data/get_config_data_external_data.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2604 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/external_data/get_request_external_data.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4302 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/external_data/import_employees_external_data.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3640 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/external_data/list_external_data.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3686 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/external_data/nominal_codes_external_data.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6315 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/external_data/pension_contributions_csv_external_data.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6885 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/external_data/post_journal_external_data.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)    11133 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/external_data/post_payments_external_data.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2840 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/external_data/post_request_external_data.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3600 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/external_data/push_employees_external_data.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2877 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/external_data/push_p11_ds_external_data.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3220 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/external_data/push_p11d_external_data.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2631 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/external_data/push_p45_external_data.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3169 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/external_data/push_p60_external_data.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4406 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/external_data/push_payslips_external_data.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3108 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/external_data/push_pension_letter_external_data.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2496 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/external_data/respond_external_data.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2572 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/external_data/set_config_data_external_data.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3656 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/external_data/set_credentials_external_data.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3954 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/external_data/sync_all_employees_external_data.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4462 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/external_data/sync_employee_external_data.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3681 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/external_data/sync_leave_external_data.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5881 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/external_data/time_and_attendance_external_data.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5668 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/external_data/update_employee_external_data.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.380139 staffology-0.1.5/staffology/api/fps/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/fps/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3943 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/fps/create_fps.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2196 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/fps/delete_fps.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3465 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/fps/get_fps.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3574 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/fps/list_fps.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4345 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/fps/mark_as_accepted_fps.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4948 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/fps/most_recent_for_employee_fps.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3403 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/fps/requiring_attention_fps.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3505 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/fps/submit_fps.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3859 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/fps/update_fps.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.380890 staffology-0.1.5/staffology/api/hmrc_payment/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/hmrc_payment/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4966 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/hmrc_payment/bank_payment_hmrc_payment.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4133 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/hmrc_payment/get_hmrc_payment.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3678 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/hmrc_payment/index_hmrc_payment.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4933 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/hmrc_payment/update_hmrc_payment.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.382053 staffology-0.1.5/staffology/api/import_/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/import_/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2587 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/import_/create_payments_csv_mapping_import.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1999 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/import_/delete_payment_csv_mapping_import.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4070 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/import_/import_employee_pay_import.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3193 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/import_/list_payments_csv_mappings_import.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3772 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/import_/payments_csv_mapping_csv_file_import.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3297 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/import_/payments_csv_mapping_import.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4470 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/import_/update_payments_csv_mapping_import.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.382840 staffology-0.1.5/staffology/api/invitation/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/invitation/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2545 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/invitation/accept_invitation.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3998 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/invitation/create_invitation.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1953 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/invitation/delete_invitation.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3113 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/invitation/get_invitation.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3479 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/invitation/index_invitation.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.384200 staffology-0.1.5/staffology/api/leave/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/leave/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2723 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/leave/add_document_leave.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2534 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/leave/create_leave.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2553 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/leave/delete_document_leave.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2269 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/leave/delete_leave.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     7001 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/leave/find_linked_piw_leave.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4317 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/leave/get_document_leave.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3856 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/leave/get_leave.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3463 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/leave/index_leave.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4546 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/leave/update_leave.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.385430 staffology-0.1.5/staffology/api/loan/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/loan/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2714 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/loan/add_document_loan.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2437 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/loan/create_loan.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2549 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/loan/delete_document_loan.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2265 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/loan/delete_loan.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4309 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/loan/get_document_loan.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3835 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/loan/get_loan.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3507 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/loan/index_loan.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4340 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/loan/update_loan.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.387121 staffology-0.1.5/staffology/api/note/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/note/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2714 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/note/add_document_note.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2407 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/note/create_note.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2549 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/note/delete_document_note.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2265 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/note/delete_note.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4309 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/note/get_document_note.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3835 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/note/get_note.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3459 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/note/index_note.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4074 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/note/update_note.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.388500 staffology-0.1.5/staffology/api/nvr/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/nvr/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3631 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/nvr/create_nvr.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2148 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/nvr/delete_nvr.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3437 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/nvr/get_nvr.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3582 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/nvr/list_nvr.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4349 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/nvr/mark_as_accepted_nvr.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3427 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/nvr/requiring_attention_nvr.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3561 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/nvr/submit_nvr.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3867 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/nvr/update_nvr.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.389498 staffology-0.1.5/staffology/api/opening_balances/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/opening_balances/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5874 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/opening_balances/get_nic_summaries_opening_balances.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3700 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/opening_balances/get_opening_balances.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5580 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/opening_balances/update_nic_summaries_opening_balances.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4321 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/opening_balances/update_opening_balances.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6021 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/opening_balances/update_p45_opening_balances.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5777 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/opening_balances/update_termination_payments_opening_balances.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.390620 staffology-0.1.5/staffology/api/pay_code/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/pay_code/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4514 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_code/create_pay_code.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1963 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_code/delete_pay_code.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3089 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_code/get_pay_code.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3884 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_code/index_pay_code.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3418 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_code/nominal_code_mappings_pay_code.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4144 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_code/update_nominal_code_mappings_pay_code.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4679 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_code/update_pay_code.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.395583 staffology-0.1.5/staffology/api/pay_run/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/pay_run/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5718 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_run/aeo_pay_run.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     7194 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_run/changes_for_pay_run_entry_pay_run.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5544 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_run/changes_pay_run.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4578 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_run/create_next_pay_run_pay_run.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3089 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_run/delete_pay_run.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     7449 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_run/finalise_pay_run_pay_run.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5079 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_run/get_pay_run_entry_pay_run.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5282 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_run/get_pay_run_events_pay_run.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5928 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_run/get_pay_run_journal_pay_run.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5099 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_run/get_pay_run_pay_codes_pay_run.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4812 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_run/get_pay_run_pay_run.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5703 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_run/get_pay_run_warnings_pay_run.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4534 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_run/get_pay_runs_pay_run.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5122 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_run/import_pay_pay_run.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6620 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_run/import_time_and_attendance_pay_run.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5897 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_run/import_umbrella_pay_pay_run.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3317 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_run/last_pay_run_entry_for_employee_pay_run.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6420 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_run/leave_pay_run.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6322 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_run/pay_run_entry_umbrella_payment_pay_run.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6228 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_run/re_open_pay_run_pay_run.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3411 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_run/send_payslip_emails_pay_run.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2978 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_run/start_next_pay_run_pay_run.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     7850 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_run/update_pay_run_entry_pay_run.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6879 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_run/update_pay_run_pay_run.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6303 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_run/update_payment_date_pay_run.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6362 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_run/ytd_pay_run.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5517 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_run/zeroise_pay_run_entries_pay_run.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.397533 staffology-0.1.5/staffology/api/pay_schedule/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/pay_schedule/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2985 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_schedule/create_pay_schedule.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3423 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_schedule/create_with_optional_ordinal_pay_schedule.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2682 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_schedule/delete_pay_schedule.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3076 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_schedule/delete_with_optional_ordinal_pay_schedule.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3632 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_schedule/get_all_pay_schedule.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4340 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_schedule/get_pay_schedule.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6344 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_schedule/get_periods_pay_schedule.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4968 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_schedule/get_with_optional_ordinal_pay_schedule.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4962 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_schedule/save_pay_schedule.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5671 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_schedule/save_with_optional_ordinal_pay_schedule.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5649 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pay_schedule/update_pay_schedule_period_pay_schedule.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.398442 staffology-0.1.5/staffology/api/payee/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/payee/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3603 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/payee/create_payee.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1929 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/payee/delete_payee.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3004 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/payee/get_payee.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3071 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/payee/index_payee.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3696 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/payee/update_payee.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.399073 staffology-0.1.5/staffology/api/pension/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/pension/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3303 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pension/get_pension.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2452 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pension/remove_pension.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4052 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pension/update_pension.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.401221 staffology-0.1.5/staffology/api/pension_scheme/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/pension_scheme/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5861 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pension_scheme/contributions_for_payrun_pension_scheme.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4737 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pension_scheme/contributions_pension_scheme.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3549 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pension_scheme/create_pension_scheme.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1887 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pension_scheme/delete_pension_scheme.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3430 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pension_scheme/employees_pension_scheme.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3029 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pension_scheme/get_pension_scheme.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2951 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pension_scheme/index_pension_scheme.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4620 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pension_scheme/list_contributions_pension_scheme.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4289 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pension_scheme/mark_as_sent_pension_scheme.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2567 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pension_scheme/resubmit_contributions_pension_scheme.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3761 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/pension_scheme/update_pension_scheme.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.402218 staffology-0.1.5/staffology/api/post/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/post/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4656 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/post/create_post.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2447 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/post/delete_post.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4302 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/post/get_post.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4382 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/post/index_post.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4852 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/post/update_post.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.403281 staffology-0.1.5/staffology/api/processing_note/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/processing_note/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2558 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/processing_note/add_document_processing_note.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6258 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/processing_note/create_processing_note.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2324 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/processing_note/delete_document_processing_note.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3956 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/processing_note/get_document_processing_note.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5145 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/processing_note/get_processing_note.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5787 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/processing_note/list_processing_note.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.404171 staffology-0.1.5/staffology/api/report_pack/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/report_pack/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3997 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/report_pack/create_report_pack.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1956 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/report_pack/delete_report_pack.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3117 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/report_pack/get_report_pack.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3118 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/report_pack/index_report_pack.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4090 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/report_pack/update_report_pack.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.412061 staffology-0.1.5/staffology/api/reports/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/reports/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4088 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/ae_assessments_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4848 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/aeo_statement_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     7121 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/analysis_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     9954 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/bank_payment_instructions_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4234 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/cis_300_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5309 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/cis_statement_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4100 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/cis_sub_contractor_summary_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6691 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/cost_analysis_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6864 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/cost_of_employment_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2400 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/email_p45_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3177 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/email_p60_multiple_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2761 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/email_p60_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5093 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/employee_benefits_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     8415 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/employee_export_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3598 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/employer_export_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5590 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/example_payslip_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4091 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/exb_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4969 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/fps_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6195 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/full_summary_of_pay_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5731 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/furlough_report_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     7250 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/get_pay_run_csv_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     7304 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/gross_to_net_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4476 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/holiday_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6697 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/hourly_pay_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6146 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/ni_letter_validation_report_employees_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6104 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/ni_letter_validation_report_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5190 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/p11_detailed_multiple_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4551 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/p11_detailed_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4510 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/p11_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4667 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/p11d_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5556 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/p30_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4066 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/p32_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4332 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/p45_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6365 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/p60_multiple_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4658 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/p60_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6537 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/papdis_file_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6485 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/pay_run_csv_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     7667 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/pay_run_payments_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     8391 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/pay_run_summary_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5825 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/payrun_ytd_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6187 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/payslip_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     7169 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/payslips_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3892 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/right_to_work_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6753 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/statutory_pay_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4334 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/tax_code_changes_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     7400 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/umbrella_reconciliation_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)    12086 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/variance_report_reports.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3953 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/reports/ytd_reports.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.412928 staffology-0.1.5/staffology/api/tag/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/tag/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3438 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tag/create_tag.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1943 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tag/delete_tag.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3000 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tag/get_tag.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3053 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tag/index_tag.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3438 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tag/update_tag.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.418343 staffology-0.1.5/staffology/api/tenant/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/tenant/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1974 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tenant/add_admin_user_tenant.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2947 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tenant/admin_users_tenant.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3620 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tenant/bill_tenant.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3616 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tenant/bills_tenant.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4390 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tenant/create_bills_tenant.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4300 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tenant/create_tenant.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2640 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tenant/disabled_tenant.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2469 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tenant/employer_creation_tenant.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3359 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tenant/employer_usage_tenant.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3347 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tenant/employer_users_tenant.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3880 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tenant/get_rti_submission_settings_tenant.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2939 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tenant/get_tenant.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4361 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tenant/get_users_with_no_billable_activity_tenant.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1976 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tenant/remove_admin_user_tenant.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2475 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tenant/set_accounting_id_tenant.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2546 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tenant/set_bureau_redirect_email_address_tenant.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2310 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tenant/set_monthly_minimum_tenant.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2929 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tenant/set_omnipresent_role_tenant.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2526 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tenant/set_tenant_tenant.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3944 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tenant/update_bill_tenant.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3963 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tenant/update_css_colors_tenant.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2963 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tenant/update_css_tenant.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3840 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tenant/update_fav_icon_tenant.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3822 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tenant/update_logo_tenant.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4685 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tenant/update_rti_submission_settings_tenant.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4624 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tenant/update_tenant.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3572 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tenant/usage_tenant.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3219 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tenant/user_bills_tenant.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3355 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tenant/user_employers_tenant.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3020 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tenant/user_tenant.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3583 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tenant/users_search_tenant.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5788 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tenant/users_tenant.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6032 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tenant/weekly_activity_tenant.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.419335 staffology-0.1.5/staffology/api/tenant_email/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/tenant_email/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3080 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tenant_email/get_email_tenant_email.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2777 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tenant_email/get_mail_settings_tenant_email.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4240 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tenant_email/index_tenant_email.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3045 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tenant_email/resend_email_tenant_email.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3576 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tenant_email/test_mail_settings_tenant_email.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4056 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/tenant_email/update_mail_settings_tenant_email.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.420879 staffology-0.1.5/staffology/api/webhook/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/webhook/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2138 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/webhook/create_webhook.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1939 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/webhook/delete_webhook.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3048 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/webhook/get_webhook.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3089 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/webhook/index_webhook.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3652 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/webhook/payload_webhook.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4711 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/webhook/payloads_webhook.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2296 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/webhook/sample_webhook.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3522 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/webhook/update_webhook.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.421767 staffology-0.1.5/staffology/api/working_pattern/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        0 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/api/working_pattern/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3895 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/working_pattern/create_working_pattern.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1974 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/working_pattern/delete_working_pattern.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3203 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/working_pattern/get_working_pattern.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3192 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/working_pattern/index_working_pattern.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4020 2022-11-20 17:35:39.000000 staffology-0.1.5/staffology/api/working_pattern/update_working_pattern.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1821 2022-10-22 17:54:53.000000 staffology-0.1.5/staffology/client.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.499957 staffology-0.1.5/staffology/models/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)    21567 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/__init__.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2449 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/add_document_attachment_order_multipart_data.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2396 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/add_document_leave_multipart_data.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2391 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/add_document_loan_multipart_data.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2391 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/add_document_note_multipart_data.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2444 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/add_document_processing_note_multipart_data.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2954 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/address.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      536 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/ae_action.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     8144 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/ae_assessment.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4933 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/ae_assessment_action.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      661 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/ae_employee_state.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      670 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/ae_exclusion_code.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      498 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/ae_status.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      453 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/ae_statutory_letter.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      451 2022-11-15 11:04:28.000000 staffology-0.1.5/staffology/models/ae_uk_worker.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     7439 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/analysis_report.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4485 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/analysis_report_line.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1288 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/analysis_report_line_value.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2105 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/analysis_report_report_response.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1245 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/apply_year_end_employer_json_body.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)    14648 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/attachment_order.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     8352 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/attachment_order_payment.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2171 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/attachment_order_report_response.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      526 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/attachment_order_type.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      187 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/audit_event_action.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      299 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/auth_scheme.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     7538 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/auto_enrolment.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     9087 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/auto_enrolment_settings.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      280 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/auto_pilot_finalise_time.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)    11651 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/automation_settings.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5908 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/average_weekly_earnings.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      308 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/average_weekly_earnings_result.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      217 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/background_task_status.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2663 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/bank_details.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      250 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/bank_holiday_collection.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4510 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/bank_payment_instruction.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2188 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/bank_payment_instruction_report_response.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      978 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/bank_payment_instructions_csv_format.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)    10745 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/benefit.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      438 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/benefit_declaration_type.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      256 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/benefit_details_asset_type.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)    13095 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/benefit_details_car.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      259 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/benefit_details_car_power_type.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      661 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/benefit_details_class_1a_type.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5487 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/benefit_details_loan.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      640 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/benefit_details_non_class_1a_type.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      651 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/benefit_details_payment_type.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      652 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/benefit_details_use_of_asset_type.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      926 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/benefit_type.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3523 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/bureau_settings.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2426 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/calendar_entry.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      639 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/calendar_entry_type.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     7108 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/car_charge.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1626 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/car_charge_rate.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6614 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/change_summary.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6666 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/cis_300.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1963 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/cis_300_declarations.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2025 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/cis_300_report_response.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1112 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/cis_contractor.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4562 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/cis_details.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1191 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/cis_partnership.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2710 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/cis_request.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3440 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/cis_return.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     7140 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/cis_statement.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2491 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/cis_statement_list_report_response.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)    10729 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/cis_sub_contractor.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4957 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/cis_sub_contractor_summary.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2596 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/cis_sub_contractor_summary_list_report_response.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      231 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/cis_sub_contractor_type.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      241 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/cis_tax_status.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6646 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/cis_verification.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4340 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/cis_verification_details.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      847 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/cookie_preference.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)    10798 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/cost_analysis_report.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2148 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/cost_analysis_report_report_response.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1768 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/cost_breakdown.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1232 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/cost_breakdown_breakdown.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     7248 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/cost_of_employment_report.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3517 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/cost_of_employment_report_line.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2191 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/cost_of_employment_report_report_response.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      539 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/country.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      354 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/csv_file_format.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      487 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/deferal_period_type.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2003 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/department.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2312 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/department_membership.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2475 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/direct_debit_mandate.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2786 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/directorship_details.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      274 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/dps_data_type.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     7871 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/dps_notice.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3293 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/dps_settings.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1931 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/email_attachment.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2108 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/emp_refs.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     8573 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/employee.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1703 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/employee_benefits_report.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2188 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/employee_benefits_report_report_response.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      191 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/employee_status.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2912 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/employee_ytd_values.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)    17518 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/employer.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3973 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/employer_defaults.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6470 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/employer_email.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1554 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/employer_group.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1819 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/employer_group_membership.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2226 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/employer_item.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5945 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/employer_opening_balances.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1021 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/employer_settings.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4969 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/employer_template.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      777 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/employer_template_type.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)    16647 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/employment_details.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      894 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/entity_type.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)    10088 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/eps.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1936 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/eps_account.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1533 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/eps_apprenticeship_levy.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1753 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/eps_de_minimis_state_aid.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2206 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/eps_final_submission.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     7921 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/exb.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1297 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/exb_declarations.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      770 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/exb_employer.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1532 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/exb_p11_db.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2767 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/exb_p11_db_class_1a.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1212 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/exb_p11_db_class_1a_adjustment.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2951 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/exb_p11_db_class_1a_adjustments.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1253 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/exb_p11_db_class_1a_total_benefit.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)    10408 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/exb_p11d.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2824 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/exb_p11d_employee.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1992 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/exb_report_response.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4481 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/expenses_and_benefits.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1547 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/external_data_company.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4412 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/external_data_provider.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      927 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/external_data_provider_id.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      319 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/external_data_provider_type.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4873 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/external_employee_mapping.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      503 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/external_employee_mapping_status.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2999 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/external_provider_conversation.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1767 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/field_modification.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1248 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/finalise_pay_run_pay_run_json_body.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1273 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/fixed_code.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     7793 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/fps.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1293 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/fps_benefit.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4213 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/fps_car.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1401 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/fps_car_fuel.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4218 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/fps_employee.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3878 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/fps_employee_details.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1445 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/fps_employee_details_partner_details.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)    11375 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/fps_employee_figs_to_date.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2362 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/fps_employee_flexible_drawdown.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4394 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/fps_employee_n_iletters_and_values.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)    15255 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/fps_employee_payment.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2594 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/fps_employee_starter.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1145 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/fps_employee_starter_occ_pension.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1550 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/fps_employee_tax_code.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1122 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/fps_employee_trivial_commutation_payment.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1423 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/fps_employer_pay_id_changed.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     8173 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/fps_employment.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2764 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/fps_fields.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      691 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/fps_late_reason.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1992 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/fps_report_response.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1581 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/from_to_dates.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1863 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/full_payment_submission.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     7731 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/full_summary_of_pay_report.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2432 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/full_summary_of_pay_report_line.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2194 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/full_summary_of_pay_report_report_response.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      550 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/furlough_calculation_basis.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)    19604 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/furlough_report.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     8079 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/furlough_report_line.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2105 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/furlough_report_report_response.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      426 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/gender.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4308 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/gov_talk.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1835 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/gov_talk_error.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6204 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/gov_talk_submission.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     7803 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/gross_to_net_report.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4073 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/gross_to_net_report_cis_line.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5622 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/gross_to_net_report_line.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2131 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/gross_to_net_report_report_response.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     7462 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/hmrc_details.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)    22294 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/hmrc_liability.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1583 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/hmrc_payment.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3472 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/holiday_report.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2804 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/holiday_report_line.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2095 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/holiday_report_report_response.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      204 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/holiday_type.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6529 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/hourly_pay_report.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2707 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/hourly_pay_report_line.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2118 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/hourly_pay_report_report_response.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      274 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/hours_normally_worked.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2226 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/html_email_settings.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      476 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/html_insertion_point.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2401 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/import_csv_employee_multipart_data.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2401 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/import_csv_employer_multipart_data.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4206 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/invitation.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1432 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/item.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2416 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/item_list_report_response.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)    18608 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/leave.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      207 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/leave_pay_type.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)    17264 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/leave_settings.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      715 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/leave_type.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2576 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/leaver_details.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4722 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/linked_piw.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      455 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/linked_piw_result.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6632 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/loan.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1503 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/loan_charge.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1350 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/log_entry.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4885 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/mail_settings.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      555 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/marital_status.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2518 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/mileage_allowance_payments_rate.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      189 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/mileage_vehicle_type.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2985 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/monthly_minimum.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)    10563 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/national_insurance_calculation.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     9403 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/national_insurance_calculation_base.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3276 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/national_insurance_calculation_period_values.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4270 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/national_insurance_code.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1715 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/national_minimum_wage.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1563 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/ni_letter_error.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     8009 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/ni_letter_validation_report.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4737 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/ni_letter_validation_report_line.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2211 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/ni_letter_validation_report_report_response.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     7633 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/nic_summary.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2253 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/nominal_code_mapping.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4920 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/note.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      227 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/note_type.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5406 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/nvr.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2924 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/nvr_employee.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2600 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/nvr_employee_details.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      798 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/nvr_employment.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1817 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/nvr_request.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     9634 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/opening_balances.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2597 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/overseas_employer_details.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      526 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/overseas_secondment_status.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     7444 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/p11.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)    13456 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/p11_detailed.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4193 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/p11_detailed_ni_values.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2292 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/p11_detailed_report_response.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5743 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/p11_line.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4870 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/p11_ni_and_stat_payments_line.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3753 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/p11_ni_and_stat_payments_totals_line.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1313 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/p11_ni_values.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4330 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/p11_paye_line.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3055 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/p11_paye_summary.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2516 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/p11_paye_totals_line.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2248 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/p11_report_response.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2963 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/p11d_asset_available.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1795 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/p11d_asset_available_collection.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1778 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/p11d_asset_transferred_collection.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5955 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/p11d_car.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2577 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/p11d_car_collection.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1140 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/p11d_car_free_fuel_withdrawn.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2943 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/p11d_desc_other.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3887 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/p11d_expenses.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2838 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/p11d_loan.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1675 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/p11d_loan_collection.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3027 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/p11d_other.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2018 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/p11d_payment_collection.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4656 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/p11d_single_item.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5152 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/p11d_vans.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3103 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/p32.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1992 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/p32_report_response.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4957 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/papdis_document.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2592 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/papdis_document_report_response.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5579 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/papdis_employee.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     7264 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/papdis_employee_assessment.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2290 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/papdis_employee_contact.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2362 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/papdis_employee_contact_postal_address.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4570 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/papdis_employee_contribution.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2886 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/papdis_employee_exit.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3137 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/papdis_employee_identity.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1703 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/papdis_employee_name.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1728 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/papdis_employee_pay.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4907 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/papdis_employer.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      583 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/papdis_message_function_code.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6528 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/papdis_payroll_period.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2024 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/papdis_pension_provider.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      433 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/papdis_version.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1701 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/partner_details.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      454 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/pay_basis.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)    12649 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/pay_code.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      616 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/pay_code_calculation_type.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      182 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/pay_code_multiplier_type.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     8471 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/pay_line.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      483 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/pay_method.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)    11290 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/pay_options.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5028 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/pay_options_import.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      323 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/pay_period_event_type.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      265 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/pay_periods.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)    10817 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/pay_run.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1746 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/pay_run_changes.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2183 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/pay_run_cost_summary.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      533 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/pay_run_csv_type.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)    27061 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/pay_run_entry.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5434 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/pay_run_journal.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5017 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/pay_run_payment.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      589 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/pay_run_state.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2351 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/pay_run_state_change.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      298 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/pay_run_state_change_reason.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3787 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/pay_run_summary_line.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2572 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/pay_run_summary_line_i_enumerable_report_response.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)    26077 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/pay_run_totals.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)    14562 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/pay_schedule.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5767 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/pay_schedule_period.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3970 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/pay_schedule_period_event.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2674 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/pay_schedule_period_events_config.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1662 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/payee.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      517 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/payee_type.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      553 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/payment_date_type.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6160 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/payments_csv_mapping.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3052 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/payments_csv_mapping_column.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      185 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/payments_csv_mapping_type.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2199 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/payroll_value_type.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)    10079 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/payrun_email.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     8168 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/payrun_payments_report.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2356 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/payrun_payments_report_report_response.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)    12529 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/payslip.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     8097 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/payslip_customisation.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6232 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/payslip_line.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      505 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/payslip_line_type.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2248 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/payslip_report_response.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1483 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/pdf_paper_margins.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      178 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/pdf_paper_orientation.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      498 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/pdf_paper_size.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      206 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/pdf_password_type.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)    15515 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/pension.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2172 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/pension_administrator.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      253 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/pension_contribution_level_type.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5147 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/pension_contributions_submission.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      285 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/pension_csv_format.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     9278 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/pension_provider.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      238 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/pension_rule.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)    10459 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/pension_scheme.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2248 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/pension_selection.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)    10702 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/pension_summary.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1719 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/pensioner_payroll.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     8780 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/personal_details.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1940 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/post.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      515 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/pro_rata_rule.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4338 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/processing_note.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6041 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/recoverable_amounts.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1522 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/report.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      234 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/report_custom_css_option.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1930 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/report_pack.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1809 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/report_response.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3041 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/right_to_work.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      571 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/right_to_work_document_type.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3170 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/right_to_work_report.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2512 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/right_to_work_report_line.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2141 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/right_to_work_report_report_response.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      213 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/role.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2266 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/rti_agent.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1654 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/rti_contact.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2526 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/rti_employee_address.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1742 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/rti_employee_name.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      659 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/rti_sender_type.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6101 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/rti_submission_settings.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1499 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/rti_validation_warning.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      474 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/rti_validation_warning_type.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      169 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/smtp_encryption.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2451 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/smtp_settings.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      458 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/starter_declaration.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3151 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/starter_details.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2176 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/statutory_pay.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6556 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/statutory_pay_report.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3230 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/statutory_pay_report_line.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2148 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/statutory_pay_report_report_response.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1063 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/string_string_key_value_pair.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      483 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/student_loan.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1107 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/student_loan_recovered.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      520 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/submission_status.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1194 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/tag.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     7740 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/tax_and_ni.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1407 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/tax_bracket.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1523 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/tax_code_change.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2577 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/tax_code_change_report.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2161 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/tax_code_change_report_report_response.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3712 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/tax_code_change_values.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      996 2023-04-19 11:47:56.000000 staffology-0.1.5/staffology/models/tax_year.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2365 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/teachers_pension_details.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      294 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/teachers_pension_employment_type.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)    11499 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/tenant.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1941 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/tenant_billing_settings.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6462 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/tenant_email.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1612 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/tenant_html_insertion.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1631 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/tenant_item.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2738 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/tiered_pension.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1913 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/tiered_pension_rate.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3873 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/umbrella_payment.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6655 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/umbrella_reconciliation_report.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6174 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/umbrella_reconciliation_report_line.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2248 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/umbrella_reconciliation_report_report_response.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4094 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/umbrella_settings.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2414 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/update_fav_icon_tenant_multipart_data.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2406 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/update_logo_employer_multipart_data.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2396 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/update_logo_tenant_multipart_data.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2406 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/update_photo_account_multipart_data.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2411 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/update_photo_employee_multipart_data.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     6030 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/usage_bill.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)    21914 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/user.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2772 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/user_authorization.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      439 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/user_category.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     8130 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/user_display_preferences.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1364 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/user_industry.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      581 2022-11-15 11:04:53.000000 staffology-0.1.5/staffology/models/user_job_type.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      294 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/userstart_page.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1815 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/utm_info.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2939 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/value_override.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     7374 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/variance_report.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2105 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/variance_report_report_response.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2244 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/veteran_details.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3044 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/webhook.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      285 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/webhook_event.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     4062 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/webhook_payload.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     7711 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/worker_group.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     5505 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/working_pattern.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)    10176 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/year_end.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1912 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/year_end_tax_code_change.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2361 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/ytd_pay_run_multipart_data.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     3216 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/ytd_report.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     2055 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/ytd_report_report_response.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)     1923 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/models/ytd_value.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      274 2022-11-21 10:10:39.000000 staffology-0.1.5/staffology/propagate_exceptions.py
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      939 2022-10-16 21:45:52.000000 staffology-0.1.5/staffology/types.py
+drwxr-xr-x   0 isikkaplan   (501) staff       (20)        0 2023-04-19 11:49:50.330546 staffology-0.1.5/staffology.egg-info/
+-rw-r--r--   0 isikkaplan   (501) staff       (20)      524 2023-04-19 11:49:50.000000 staffology-0.1.5/staffology.egg-info/PKG-INFO
+-rw-r--r--   0 isikkaplan   (501) staff       (20)    41463 2023-04-19 11:49:50.000000 staffology-0.1.5/staffology.egg-info/SOURCES.txt
+-rw-r--r--   0 isikkaplan   (501) staff       (20)        1 2023-04-19 11:49:50.000000 staffology-0.1.5/staffology.egg-info/dependency_links.txt
+-rw-r--r--   0 isikkaplan   (501) staff       (20)       12 2023-04-19 11:49:50.000000 staffology-0.1.5/staffology.egg-info/requires.txt
+-rw-r--r--   0 isikkaplan   (501) staff       (20)       11 2023-04-19 11:49:50.000000 staffology-0.1.5/staffology.egg-info/top_level.txt
```

### Comparing `staffology-0.1.4/PKG-INFO` & `staffology-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: staffology
-Version: 0.1.4
+Version: 0.1.5
 Summary: Staffology openapi client with authentication patch
 Home-page: https://github.com/ihorizonUK/staffology
 Author: isik-kaplan
 Author-email: isik@ihorizon.co.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.7
```

### Comparing `staffology-0.1.4/setup.py` & `staffology-0.1.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name='staffology',
-    version='0.1.4',
+    version='0.1.5',
     packages=find_packages(),
     url='https://github.com/ihorizonUK/staffology',
     description="Staffology openapi client with authentication patch",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='isik-kaplan',
     author_email='isik@ihorizon.co.uk',
```

### Comparing `staffology-0.1.4/staffology/api/account/activate_account.py` & `staffology-0.1.5/staffology/api/account/activate_account.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/account/change_email_address_account.py` & `staffology-0.1.5/staffology/api/account/change_email_address_account.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/account/create_api_key_account.py` & `staffology-0.1.5/staffology/api/account/create_api_key_account.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/account/create_demo_employer_account.py` & `staffology-0.1.5/staffology/api/account/create_demo_employer_account.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/account/delete_api_key_account.py` & `staffology-0.1.5/staffology/api/account/delete_api_key_account.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/account/get_account.py` & `staffology-0.1.5/staffology/api/account/get_account.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/account/get_api_key_account.py` & `staffology-0.1.5/staffology/api/account/get_api_key_account.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/account/get_employer_defaults_account.py` & `staffology-0.1.5/staffology/api/account/get_employer_defaults_account.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/account/get_invitations_account.py` & `staffology-0.1.5/staffology/api/account/get_invitations_account.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/account/get_tenant_account.py` & `staffology-0.1.5/staffology/api/account/get_tenant_account.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/account/list_api_keys_account.py` & `staffology-0.1.5/staffology/api/account/list_api_keys_account.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/account/profile_account.py` & `staffology-0.1.5/staffology/api/account/profile_account.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/account/set_employer_defaults_account.py` & `staffology-0.1.5/staffology/api/account/set_employer_defaults_account.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/account/update_cookie_preferences_account.py` & `staffology-0.1.5/staffology/api/account/update_cookie_preferences_account.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/account/update_photo_account.py` & `staffology-0.1.5/staffology/api/account/update_photo_account.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/account/verify_account.py` & `staffology-0.1.5/staffology/api/account/verify_account.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/account/verify_response_account.py` & `staffology-0.1.5/staffology/api/account/verify_response_account.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/attachment_order/add_document_attachment_order.py` & `staffology-0.1.5/staffology/api/attachment_order/add_document_attachment_order.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/attachment_order/create_attachment_order.py` & `staffology-0.1.5/staffology/api/attachment_order/create_attachment_order.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/attachment_order/delete_attachment_order.py` & `staffology-0.1.5/staffology/api/attachment_order/delete_attachment_order.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/attachment_order/delete_document_attachment_order.py` & `staffology-0.1.5/staffology/api/attachment_order/delete_document_attachment_order.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/attachment_order/get_attachment_order.py` & `staffology-0.1.5/staffology/api/attachment_order/get_attachment_order.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/attachment_order/get_document_attachment_order.py` & `staffology-0.1.5/staffology/api/attachment_order/get_document_attachment_order.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/attachment_order/index_attachment_order.py` & `staffology-0.1.5/staffology/api/attachment_order/index_attachment_order.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/attachment_order/payments_attachment_order.py` & `staffology-0.1.5/staffology/api/attachment_order/payments_attachment_order.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/attachment_order/update_attachment_order.py` & `staffology-0.1.5/staffology/api/attachment_order/update_attachment_order.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/audit/employer_audit_list_audit.py` & `staffology-0.1.5/staffology/api/audit/employer_audit_list_audit.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/auto_enrolment/assess_auto_enrolment.py` & `staffology-0.1.5/staffology/api/auto_enrolment/assess_auto_enrolment.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/auto_enrolment/delete_auto_enrolment.py` & `staffology-0.1.5/staffology/api/auto_enrolment/delete_auto_enrolment.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/auto_enrolment/email_letter_auto_enrolment.py` & `staffology-0.1.5/staffology/api/auto_enrolment/email_letter_auto_enrolment.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/auto_enrolment/get_auto_enrolment.py` & `staffology-0.1.5/staffology/api/auto_enrolment/get_auto_enrolment.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/auto_enrolment/get_last_auto_enrolment.py` & `staffology-0.1.5/staffology/api/auto_enrolment/get_last_auto_enrolment.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/auto_enrolment/get_letter_auto_enrolment.py` & `staffology-0.1.5/staffology/api/auto_enrolment/get_letter_auto_enrolment.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/auto_enrolment/list_auto_enrolment.py` & `staffology-0.1.5/staffology/api/auto_enrolment/list_auto_enrolment.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/auto_enrolment/mark_letter_as_sent_auto_enrolment.py` & `staffology-0.1.5/staffology/api/auto_enrolment/mark_letter_as_sent_auto_enrolment.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/auto_enrolment/pending_letters_auto_enrolment.py` & `staffology-0.1.5/staffology/api/auto_enrolment/pending_letters_auto_enrolment.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/auto_enrolment/pending_postponement_letters_auto_enrolment.py` & `staffology-0.1.5/staffology/api/auto_enrolment/pending_postponement_letters_auto_enrolment.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/auto_enrolment/reenrol_auto_enrolment.py` & `staffology-0.1.5/staffology/api/auto_enrolment/reenrol_auto_enrolment.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/auto_enrolment/set_state_auto_enrolment.py` & `staffology-0.1.5/staffology/api/auto_enrolment/set_state_auto_enrolment.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/benefits/create_benefits.py` & `staffology-0.1.5/staffology/api/benefits/create_benefits.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/benefits/delete_benefits.py` & `staffology-0.1.5/staffology/api/benefits/delete_benefits.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/benefits/get_benefits.py` & `staffology-0.1.5/staffology/api/benefits/get_benefits.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/benefits/index_benefits.py` & `staffology-0.1.5/staffology/api/benefits/index_benefits.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/benefits/update_benefits.py` & `staffology-0.1.5/staffology/api/benefits/update_benefits.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/billing/bill_billing.py` & `staffology-0.1.5/staffology/api/billing/bill_billing.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/billing/bill_csv_billing.py` & `staffology-0.1.5/staffology/api/billing/bill_csv_billing.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/billing/bills_billing.py` & `staffology-0.1.5/staffology/api/billing/bills_billing.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/billing/confirm_direct_debit_mandate_billing.py` & `staffology-0.1.5/staffology/api/billing/confirm_direct_debit_mandate_billing.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/billing/delete_direct_debit_mandate_billing.py` & `staffology-0.1.5/staffology/api/billing/delete_direct_debit_mandate_billing.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/billing/direct_debit_mandate_billing.py` & `staffology-0.1.5/staffology/api/billing/direct_debit_mandate_billing.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/billing/get_usage_stats_billing.py` & `staffology-0.1.5/staffology/api/billing/get_usage_stats_billing.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/billing/setup_direct_debit_mandate_billing.py` & `staffology-0.1.5/staffology/api/billing/setup_direct_debit_mandate_billing.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/bureau/employers_bureau.py` & `staffology-0.1.5/staffology/api/bureau/employers_bureau.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/bureau/get_processor_user_bureau.py` & `staffology-0.1.5/staffology/api/bureau/get_processor_user_bureau.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/bureau/get_report_pack_bureau.py` & `staffology-0.1.5/staffology/api/bureau/get_report_pack_bureau.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/bureau/get_settings_bureau.py` & `staffology-0.1.5/staffology/api/bureau/get_settings_bureau.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/bureau/processor_users_bureau.py` & `staffology-0.1.5/staffology/api/bureau/processor_users_bureau.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/bureau/update_settings_bureau.py` & `staffology-0.1.5/staffology/api/bureau/update_settings_bureau.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/cis_300/create_cis_300.py` & `staffology-0.1.5/staffology/api/cis_300/create_cis_300.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/cis_300/delete_cis_300.py` & `staffology-0.1.5/staffology/api/cis_300/delete_cis_300.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/cis_300/get_cis_300.py` & `staffology-0.1.5/staffology/api/cis_300/get_cis_300.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/cis_300/list_cis_300.py` & `staffology-0.1.5/staffology/api/cis_300/list_cis_300.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/cis_300/mark_as_accepted_cis_300.py` & `staffology-0.1.5/staffology/api/cis_300/mark_as_accepted_cis_300.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/cis_300/requiring_attention_cis_300.py` & `staffology-0.1.5/staffology/api/cis_300/requiring_attention_cis_300.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/cis_300/submit_cis_300.py` & `staffology-0.1.5/staffology/api/cis_300/submit_cis_300.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/cis_300/update_cis_300.py` & `staffology-0.1.5/staffology/api/cis_300/update_cis_300.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/cis_verification/create_cis_verification.py` & `staffology-0.1.5/staffology/api/cis_verification/create_cis_verification.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/cis_verification/delete_cis_verification.py` & `staffology-0.1.5/staffology/api/cis_verification/delete_cis_verification.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/cis_verification/get_cis_verification.py` & `staffology-0.1.5/staffology/api/cis_verification/get_cis_verification.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/cis_verification/list_cis_verification.py` & `staffology-0.1.5/staffology/api/cis_verification/list_cis_verification.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/cis_verification/mark_as_accepted_cis_verification.py` & `staffology-0.1.5/staffology/api/cis_verification/mark_as_accepted_cis_verification.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/cis_verification/requiring_attention_cis_verification.py` & `staffology-0.1.5/staffology/api/cis_verification/requiring_attention_cis_verification.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/cis_verification/submit_cis_verification.py` & `staffology-0.1.5/staffology/api/cis_verification/submit_cis_verification.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/cis_verification/update_cis_verification.py` & `staffology-0.1.5/staffology/api/cis_verification/update_cis_verification.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/department/create_department.py` & `staffology-0.1.5/staffology/api/department/create_department.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/department/delete_department.py` & `staffology-0.1.5/staffology/api/department/delete_department.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/department/get_department.py` & `staffology-0.1.5/staffology/api/department/get_department.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/department/index_department.py` & `staffology-0.1.5/staffology/api/department/index_department.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/department/update_department.py` & `staffology-0.1.5/staffology/api/department/update_department.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/dps/apply_dps.py` & `staffology-0.1.5/staffology/api/dps/apply_dps.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/dps/check_for_notices_dps.py` & `staffology-0.1.5/staffology/api/dps/check_for_notices_dps.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/dps/delete_all_dps.py` & `staffology-0.1.5/staffology/api/dps/delete_all_dps.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/dps/delete_dps.py` & `staffology-0.1.5/staffology/api/dps/delete_dps.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/dps/get_dps.py` & `staffology-0.1.5/staffology/api/dps/get_dps.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/dps/get_dps_settings_dps.py` & `staffology-0.1.5/staffology/api/dps/get_dps_settings_dps.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/dps/list_notices_dps.py` & `staffology-0.1.5/staffology/api/dps/list_notices_dps.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/dps/parse_xml_dps.py` & `staffology-0.1.5/staffology/api/dps/parse_xml_dps.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/dps/update_dps_settings_dps.py` & `staffology-0.1.5/staffology/api/dps/update_dps_settings_dps.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/email/get_email_email.py` & `staffology-0.1.5/staffology/api/email/get_email_email.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/email/get_mail_settings_email.py` & `staffology-0.1.5/staffology/api/email/get_mail_settings_email.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/email/index_email.py` & `staffology-0.1.5/staffology/api/email/index_email.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/email/resend_email_email.py` & `staffology-0.1.5/staffology/api/email/resend_email_email.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/email/test_mail_settings_email.py` & `staffology-0.1.5/staffology/api/email/test_mail_settings_email.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/email/update_mail_settings_email.py` & `staffology-0.1.5/staffology/api/email/update_mail_settings_email.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/email/verify_mail_settings_email.py` & `staffology-0.1.5/staffology/api/email/verify_mail_settings_email.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/email/verify_mail_settings_response_email.py` & `staffology-0.1.5/staffology/api/email/verify_mail_settings_response_email.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employee/apply_pay_increase_employee.py` & `staffology-0.1.5/staffology/api/employee/apply_pay_increase_employee.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employee/apply_pay_options_employee.py` & `staffology-0.1.5/staffology/api/employee/apply_pay_options_employee.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employee/average_weekly_earnings_employee.py` & `staffology-0.1.5/staffology/api/employee/average_weekly_earnings_employee.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employee/base_daily_rate_employee.py` & `staffology-0.1.5/staffology/api/employee/base_daily_rate_employee.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employee/base_hourly_rate_employee.py` & `staffology-0.1.5/staffology/api/employee/base_hourly_rate_employee.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employee/create_employee.py` & `staffology-0.1.5/staffology/api/employee/create_employee.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employee/delete_employee.py` & `staffology-0.1.5/staffology/api/employee/delete_employee.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employee/delete_multiple_employee.py` & `staffology-0.1.5/staffology/api/employee/delete_multiple_employee.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employee/delete_photo_employee.py` & `staffology-0.1.5/staffology/api/employee/delete_photo_employee.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employee/expiring_rtw_employee.py` & `staffology-0.1.5/staffology/api/employee/expiring_rtw_employee.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employee/get_department_memberships_employee.py` & `staffology-0.1.5/staffology/api/employee/get_department_memberships_employee.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employee/get_employee.py` & `staffology-0.1.5/staffology/api/employee/get_employee.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employee/import_csv_employee.py` & `staffology-0.1.5/staffology/api/employee/import_csv_employee.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employee/index_employee.py` & `staffology-0.1.5/staffology/api/employee/index_employee.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employee/leavers_employee.py` & `staffology-0.1.5/staffology/api/employee/leavers_employee.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employee/mark_as_leavers_employee.py` & `staffology-0.1.5/staffology/api/employee/mark_as_leavers_employee.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employee/minimum_wage_employee.py` & `staffology-0.1.5/staffology/api/employee/minimum_wage_employee.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employee/pay_run_entries_employee.py` & `staffology-0.1.5/staffology/api/employee/pay_run_entries_employee.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employee/re_hire_employee.py` & `staffology-0.1.5/staffology/api/employee/re_hire_employee.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employee/search_by_payroll_code_employee.py` & `staffology-0.1.5/staffology/api/employee/search_by_payroll_code_employee.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employee/search_employee.py` & `staffology-0.1.5/staffology/api/employee/search_employee.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employee/set_department_memberships_employee.py` & `staffology-0.1.5/staffology/api/employee/set_department_memberships_employee.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employee/set_on_hold_employee.py` & `staffology-0.1.5/staffology/api/employee/set_on_hold_employee.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employee/update_employee.py` & `staffology-0.1.5/staffology/api/employee/update_employee.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employee/update_photo_employee.py` & `staffology-0.1.5/staffology/api/employee/update_photo_employee.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employer/apply_year_end_employer.py` & `staffology-0.1.5/staffology/api/employer/apply_year_end_employer.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employer/calendar_employer.py` & `staffology-0.1.5/staffology/api/employer/calendar_employer.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employer/create_employer.py` & `staffology-0.1.5/staffology/api/employer/create_employer.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employer/custom_payslip_employer.py` & `staffology-0.1.5/staffology/api/employer/custom_payslip_employer.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employer/delete_employer.py` & `staffology-0.1.5/staffology/api/employer/delete_employer.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employer/get_automation_settings_employer.py` & `staffology-0.1.5/staffology/api/employer/get_automation_settings_employer.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employer/get_employer.py` & `staffology-0.1.5/staffology/api/employer/get_employer.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employer/get_employer_opening_balances_employer.py` & `staffology-0.1.5/staffology/api/employer/get_employer_opening_balances_employer.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employer/get_group_memberships_employer.py` & `staffology-0.1.5/staffology/api/employer/get_group_memberships_employer.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employer/import_csv_employer.py` & `staffology-0.1.5/staffology/api/employer/import_csv_employer.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employer/index_employer.py` & `staffology-0.1.5/staffology/api/employer/index_employer.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employer/list_users_employer.py` & `staffology-0.1.5/staffology/api/employer/list_users_employer.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employer/remove_user_employer.py` & `staffology-0.1.5/staffology/api/employer/remove_user_employer.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employer/review_year_end_employer.py` & `staffology-0.1.5/staffology/api/employer/review_year_end_employer.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employer/rti_requiring_attention_employer.py` & `staffology-0.1.5/staffology/api/employer/rti_requiring_attention_employer.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employer/search_employees_employer.py` & `staffology-0.1.5/staffology/api/employer/search_employees_employer.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employer/search_employer.py` & `staffology-0.1.5/staffology/api/employer/search_employer.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employer/set_group_memberships_employer.py` & `staffology-0.1.5/staffology/api/employer/set_group_memberships_employer.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employer/set_owner_employer.py` & `staffology-0.1.5/staffology/api/employer/set_owner_employer.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employer/suggest_pay_code_employer.py` & `staffology-0.1.5/staffology/api/employer/suggest_pay_code_employer.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employer/update_automation_settings_employer.py` & `staffology-0.1.5/staffology/api/employer/update_automation_settings_employer.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employer/update_custom_payslip_employer.py` & `staffology-0.1.5/staffology/api/employer/update_custom_payslip_employer.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employer/update_employer.py` & `staffology-0.1.5/staffology/api/employer/update_employer.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employer/update_employer_opening_balances_employer.py` & `staffology-0.1.5/staffology/api/employer/update_employer_opening_balances_employer.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employer/update_logo_employer.py` & `staffology-0.1.5/staffology/api/employer/update_logo_employer.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employer_group/create_employer_group.py` & `staffology-0.1.5/staffology/api/employer_group/create_employer_group.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employer_group/delete_employer_group.py` & `staffology-0.1.5/staffology/api/employer_group/delete_employer_group.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employer_group/get_employer_group.py` & `staffology-0.1.5/staffology/api/employer_group/get_employer_group.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employer_group/index_employer_group.py` & `staffology-0.1.5/staffology/api/employer_group/index_employer_group.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employer_group/update_employer_group.py` & `staffology-0.1.5/staffology/api/employer_group/update_employer_group.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employer_template/get_employer_template.py` & `staffology-0.1.5/staffology/api/employer_template/get_employer_template.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employer_template/index_employer_template.py` & `staffology-0.1.5/staffology/api/employer_template/index_employer_template.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/employer_template/update_employer_template.py` & `staffology-0.1.5/staffology/api/employer_template/update_employer_template.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/engine/calculate_ni_engine.py` & `staffology-0.1.5/staffology/api/engine/calculate_ni_engine.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/engine/calculate_tax_engine.py` & `staffology-0.1.5/staffology/api/engine/calculate_tax_engine.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/engine/config_engine.py` & `staffology-0.1.5/staffology/api/engine/config_engine.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/engine/get_national_insurance_thresholds_engine.py` & `staffology-0.1.5/staffology/api/engine/get_national_insurance_thresholds_engine.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/engine/get_tenant_branding_engine.py` & `staffology-0.1.5/staffology/api/engine/get_tenant_branding_engine.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/eps/create_eps.py` & `staffology-0.1.5/staffology/api/eps/create_eps.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/eps/delete_eps.py` & `staffology-0.1.5/staffology/api/eps/delete_eps.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/eps/get_eps.py` & `staffology-0.1.5/staffology/api/eps/get_eps.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/eps/list_eps.py` & `staffology-0.1.5/staffology/api/eps/list_eps.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/eps/mark_as_accepted_eps.py` & `staffology-0.1.5/staffology/api/eps/mark_as_accepted_eps.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/eps/recoverable_amounts_eps.py` & `staffology-0.1.5/staffology/api/eps/recoverable_amounts_eps.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/eps/requiring_attention_eps.py` & `staffology-0.1.5/staffology/api/eps/requiring_attention_eps.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/eps/submit_eps.py` & `staffology-0.1.5/staffology/api/eps/submit_eps.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/eps/update_eps.py` & `staffology-0.1.5/staffology/api/eps/update_eps.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/exb/annual_values_exb.py` & `staffology-0.1.5/staffology/api/exb/annual_values_exb.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/exb/create_exb.py` & `staffology-0.1.5/staffology/api/exb/create_exb.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/exb/delete_exb.py` & `staffology-0.1.5/staffology/api/exb/delete_exb.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/exb/get_exb.py` & `staffology-0.1.5/staffology/api/exb/get_exb.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/exb/list_exb.py` & `staffology-0.1.5/staffology/api/exb/list_exb.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/exb/mark_as_accepted_exb.py` & `staffology-0.1.5/staffology/api/exb/mark_as_accepted_exb.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/exb/requiring_attention_exb.py` & `staffology-0.1.5/staffology/api/exb/requiring_attention_exb.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/exb/submit_exb.py` & `staffology-0.1.5/staffology/api/exb/submit_exb.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/exb/update_exb.py` & `staffology-0.1.5/staffology/api/exb/update_exb.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/external_data/authorize_external_data.py` & `staffology-0.1.5/staffology/api/external_data/authorize_external_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/external_data/companies_external_data.py` & `staffology-0.1.5/staffology/api/external_data/companies_external_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/external_data/disconnect_external_data.py` & `staffology-0.1.5/staffology/api/external_data/disconnect_external_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/external_data/employee_external_data.py` & `staffology-0.1.5/staffology/api/external_data/employee_external_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/external_data/employee_logs_external_data.py` & `staffology-0.1.5/staffology/api/external_data/employee_logs_external_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/external_data/employees_external_data.py` & `staffology-0.1.5/staffology/api/external_data/employees_external_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/external_data/get_config_data_external_data.py` & `staffology-0.1.5/staffology/api/external_data/get_config_data_external_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/external_data/get_request_external_data.py` & `staffology-0.1.5/staffology/api/external_data/get_request_external_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/external_data/import_employees_external_data.py` & `staffology-0.1.5/staffology/api/external_data/import_employees_external_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/external_data/list_external_data.py` & `staffology-0.1.5/staffology/api/external_data/list_external_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/external_data/nominal_codes_external_data.py` & `staffology-0.1.5/staffology/api/external_data/nominal_codes_external_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/external_data/pension_contributions_csv_external_data.py` & `staffology-0.1.5/staffology/api/external_data/pension_contributions_csv_external_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/external_data/post_journal_external_data.py` & `staffology-0.1.5/staffology/api/external_data/post_journal_external_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/external_data/post_payments_external_data.py` & `staffology-0.1.5/staffology/api/external_data/post_payments_external_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/external_data/post_request_external_data.py` & `staffology-0.1.5/staffology/api/external_data/post_request_external_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/external_data/push_employees_external_data.py` & `staffology-0.1.5/staffology/api/external_data/push_employees_external_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/external_data/push_p11_ds_external_data.py` & `staffology-0.1.5/staffology/api/external_data/push_p11_ds_external_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/external_data/push_p11d_external_data.py` & `staffology-0.1.5/staffology/api/external_data/push_p11d_external_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/external_data/push_p45_external_data.py` & `staffology-0.1.5/staffology/api/external_data/push_p45_external_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/external_data/push_p60_external_data.py` & `staffology-0.1.5/staffology/api/external_data/push_p60_external_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/external_data/push_payslips_external_data.py` & `staffology-0.1.5/staffology/api/external_data/push_payslips_external_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/external_data/push_pension_letter_external_data.py` & `staffology-0.1.5/staffology/api/external_data/push_pension_letter_external_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/external_data/respond_external_data.py` & `staffology-0.1.5/staffology/api/external_data/respond_external_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/external_data/set_config_data_external_data.py` & `staffology-0.1.5/staffology/api/external_data/set_config_data_external_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/external_data/set_credentials_external_data.py` & `staffology-0.1.5/staffology/api/external_data/set_credentials_external_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/external_data/sync_all_employees_external_data.py` & `staffology-0.1.5/staffology/api/external_data/sync_all_employees_external_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/external_data/sync_employee_external_data.py` & `staffology-0.1.5/staffology/api/external_data/sync_employee_external_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/external_data/sync_leave_external_data.py` & `staffology-0.1.5/staffology/api/external_data/sync_leave_external_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/external_data/time_and_attendance_external_data.py` & `staffology-0.1.5/staffology/api/external_data/time_and_attendance_external_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/external_data/update_employee_external_data.py` & `staffology-0.1.5/staffology/api/external_data/update_employee_external_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/fps/create_fps.py` & `staffology-0.1.5/staffology/api/fps/create_fps.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/fps/delete_fps.py` & `staffology-0.1.5/staffology/api/fps/delete_fps.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/fps/get_fps.py` & `staffology-0.1.5/staffology/api/fps/get_fps.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/fps/list_fps.py` & `staffology-0.1.5/staffology/api/fps/list_fps.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/fps/mark_as_accepted_fps.py` & `staffology-0.1.5/staffology/api/fps/mark_as_accepted_fps.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/fps/most_recent_for_employee_fps.py` & `staffology-0.1.5/staffology/api/fps/most_recent_for_employee_fps.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/fps/requiring_attention_fps.py` & `staffology-0.1.5/staffology/api/fps/requiring_attention_fps.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/fps/submit_fps.py` & `staffology-0.1.5/staffology/api/fps/submit_fps.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/fps/update_fps.py` & `staffology-0.1.5/staffology/api/fps/update_fps.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/hmrc_payment/bank_payment_hmrc_payment.py` & `staffology-0.1.5/staffology/api/hmrc_payment/bank_payment_hmrc_payment.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/hmrc_payment/get_hmrc_payment.py` & `staffology-0.1.5/staffology/api/hmrc_payment/get_hmrc_payment.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/hmrc_payment/index_hmrc_payment.py` & `staffology-0.1.5/staffology/api/hmrc_payment/index_hmrc_payment.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/hmrc_payment/update_hmrc_payment.py` & `staffology-0.1.5/staffology/api/hmrc_payment/update_hmrc_payment.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/import_/create_payments_csv_mapping_import.py` & `staffology-0.1.5/staffology/api/import_/create_payments_csv_mapping_import.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/import_/delete_payment_csv_mapping_import.py` & `staffology-0.1.5/staffology/api/import_/delete_payment_csv_mapping_import.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/import_/import_employee_pay_import.py` & `staffology-0.1.5/staffology/api/import_/import_employee_pay_import.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/import_/list_payments_csv_mappings_import.py` & `staffology-0.1.5/staffology/api/import_/list_payments_csv_mappings_import.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/import_/payments_csv_mapping_csv_file_import.py` & `staffology-0.1.5/staffology/api/import_/payments_csv_mapping_csv_file_import.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/import_/payments_csv_mapping_import.py` & `staffology-0.1.5/staffology/api/import_/payments_csv_mapping_import.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/import_/update_payments_csv_mapping_import.py` & `staffology-0.1.5/staffology/api/import_/update_payments_csv_mapping_import.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/invitation/accept_invitation.py` & `staffology-0.1.5/staffology/api/invitation/accept_invitation.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/invitation/create_invitation.py` & `staffology-0.1.5/staffology/api/invitation/create_invitation.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/invitation/delete_invitation.py` & `staffology-0.1.5/staffology/api/invitation/delete_invitation.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/invitation/get_invitation.py` & `staffology-0.1.5/staffology/api/invitation/get_invitation.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/invitation/index_invitation.py` & `staffology-0.1.5/staffology/api/invitation/index_invitation.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/leave/add_document_leave.py` & `staffology-0.1.5/staffology/api/leave/add_document_leave.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/leave/create_leave.py` & `staffology-0.1.5/staffology/api/leave/create_leave.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/leave/delete_document_leave.py` & `staffology-0.1.5/staffology/api/leave/delete_document_leave.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/leave/delete_leave.py` & `staffology-0.1.5/staffology/api/leave/delete_leave.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/leave/find_linked_piw_leave.py` & `staffology-0.1.5/staffology/api/leave/find_linked_piw_leave.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/leave/get_document_leave.py` & `staffology-0.1.5/staffology/api/leave/get_document_leave.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/leave/get_leave.py` & `staffology-0.1.5/staffology/api/leave/get_leave.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/leave/index_leave.py` & `staffology-0.1.5/staffology/api/leave/index_leave.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/leave/update_leave.py` & `staffology-0.1.5/staffology/api/leave/update_leave.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/loan/add_document_loan.py` & `staffology-0.1.5/staffology/api/loan/add_document_loan.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/loan/create_loan.py` & `staffology-0.1.5/staffology/api/loan/create_loan.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/loan/delete_document_loan.py` & `staffology-0.1.5/staffology/api/loan/delete_document_loan.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/loan/delete_loan.py` & `staffology-0.1.5/staffology/api/loan/delete_loan.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/loan/get_document_loan.py` & `staffology-0.1.5/staffology/api/loan/get_document_loan.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/loan/get_loan.py` & `staffology-0.1.5/staffology/api/loan/get_loan.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/loan/index_loan.py` & `staffology-0.1.5/staffology/api/loan/index_loan.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/loan/update_loan.py` & `staffology-0.1.5/staffology/api/loan/update_loan.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/note/add_document_note.py` & `staffology-0.1.5/staffology/api/note/add_document_note.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/note/create_note.py` & `staffology-0.1.5/staffology/api/note/create_note.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/note/delete_document_note.py` & `staffology-0.1.5/staffology/api/note/delete_document_note.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/note/delete_note.py` & `staffology-0.1.5/staffology/api/note/delete_note.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/note/get_document_note.py` & `staffology-0.1.5/staffology/api/note/get_document_note.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/note/get_note.py` & `staffology-0.1.5/staffology/api/note/get_note.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/note/index_note.py` & `staffology-0.1.5/staffology/api/note/index_note.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/note/update_note.py` & `staffology-0.1.5/staffology/api/note/update_note.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/nvr/create_nvr.py` & `staffology-0.1.5/staffology/api/nvr/create_nvr.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/nvr/delete_nvr.py` & `staffology-0.1.5/staffology/api/nvr/delete_nvr.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/nvr/get_nvr.py` & `staffology-0.1.5/staffology/api/nvr/get_nvr.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/nvr/list_nvr.py` & `staffology-0.1.5/staffology/api/nvr/list_nvr.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/nvr/mark_as_accepted_nvr.py` & `staffology-0.1.5/staffology/api/nvr/mark_as_accepted_nvr.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/nvr/requiring_attention_nvr.py` & `staffology-0.1.5/staffology/api/nvr/requiring_attention_nvr.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/nvr/submit_nvr.py` & `staffology-0.1.5/staffology/api/nvr/submit_nvr.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/nvr/update_nvr.py` & `staffology-0.1.5/staffology/api/nvr/update_nvr.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/opening_balances/get_nic_summaries_opening_balances.py` & `staffology-0.1.5/staffology/api/opening_balances/get_nic_summaries_opening_balances.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/opening_balances/get_opening_balances.py` & `staffology-0.1.5/staffology/api/opening_balances/get_opening_balances.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/opening_balances/update_nic_summaries_opening_balances.py` & `staffology-0.1.5/staffology/api/opening_balances/update_nic_summaries_opening_balances.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/opening_balances/update_opening_balances.py` & `staffology-0.1.5/staffology/api/opening_balances/update_opening_balances.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/opening_balances/update_p45_opening_balances.py` & `staffology-0.1.5/staffology/api/opening_balances/update_p45_opening_balances.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/opening_balances/update_termination_payments_opening_balances.py` & `staffology-0.1.5/staffology/api/opening_balances/update_termination_payments_opening_balances.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_code/create_pay_code.py` & `staffology-0.1.5/staffology/api/pay_code/create_pay_code.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_code/delete_pay_code.py` & `staffology-0.1.5/staffology/api/pay_code/delete_pay_code.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_code/get_pay_code.py` & `staffology-0.1.5/staffology/api/pay_code/get_pay_code.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_code/index_pay_code.py` & `staffology-0.1.5/staffology/api/pay_code/index_pay_code.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_code/nominal_code_mappings_pay_code.py` & `staffology-0.1.5/staffology/api/pay_code/nominal_code_mappings_pay_code.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_code/update_nominal_code_mappings_pay_code.py` & `staffology-0.1.5/staffology/api/pay_code/update_nominal_code_mappings_pay_code.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_code/update_pay_code.py` & `staffology-0.1.5/staffology/api/pay_code/update_pay_code.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_run/aeo_pay_run.py` & `staffology-0.1.5/staffology/api/pay_run/aeo_pay_run.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_run/changes_for_pay_run_entry_pay_run.py` & `staffology-0.1.5/staffology/api/pay_run/changes_for_pay_run_entry_pay_run.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_run/changes_pay_run.py` & `staffology-0.1.5/staffology/api/pay_run/changes_pay_run.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_run/create_next_pay_run_pay_run.py` & `staffology-0.1.5/staffology/api/pay_run/create_next_pay_run_pay_run.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_run/delete_pay_run.py` & `staffology-0.1.5/staffology/api/pay_run/delete_pay_run.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_run/finalise_pay_run_pay_run.py` & `staffology-0.1.5/staffology/api/pay_run/finalise_pay_run_pay_run.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_run/get_pay_run_entry_pay_run.py` & `staffology-0.1.5/staffology/api/pay_run/get_pay_run_entry_pay_run.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_run/get_pay_run_events_pay_run.py` & `staffology-0.1.5/staffology/api/pay_run/get_pay_run_events_pay_run.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_run/get_pay_run_journal_pay_run.py` & `staffology-0.1.5/staffology/api/pay_run/get_pay_run_journal_pay_run.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_run/get_pay_run_pay_codes_pay_run.py` & `staffology-0.1.5/staffology/api/pay_run/get_pay_run_pay_codes_pay_run.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_run/get_pay_run_pay_run.py` & `staffology-0.1.5/staffology/api/pay_run/get_pay_run_pay_run.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_run/get_pay_run_warnings_pay_run.py` & `staffology-0.1.5/staffology/api/pay_run/get_pay_run_warnings_pay_run.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_run/get_pay_runs_pay_run.py` & `staffology-0.1.5/staffology/api/pay_run/get_pay_runs_pay_run.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_run/import_pay_pay_run.py` & `staffology-0.1.5/staffology/api/pay_run/import_pay_pay_run.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_run/import_time_and_attendance_pay_run.py` & `staffology-0.1.5/staffology/api/pay_run/import_time_and_attendance_pay_run.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_run/import_umbrella_pay_pay_run.py` & `staffology-0.1.5/staffology/api/pay_run/import_umbrella_pay_pay_run.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_run/last_pay_run_entry_for_employee_pay_run.py` & `staffology-0.1.5/staffology/api/pay_run/last_pay_run_entry_for_employee_pay_run.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_run/leave_pay_run.py` & `staffology-0.1.5/staffology/api/pay_run/leave_pay_run.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_run/pay_run_entry_umbrella_payment_pay_run.py` & `staffology-0.1.5/staffology/api/pay_run/pay_run_entry_umbrella_payment_pay_run.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_run/re_open_pay_run_pay_run.py` & `staffology-0.1.5/staffology/api/pay_run/re_open_pay_run_pay_run.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_run/send_payslip_emails_pay_run.py` & `staffology-0.1.5/staffology/api/pay_run/send_payslip_emails_pay_run.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_run/start_next_pay_run_pay_run.py` & `staffology-0.1.5/staffology/api/pay_run/start_next_pay_run_pay_run.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_run/update_pay_run_entry_pay_run.py` & `staffology-0.1.5/staffology/api/pay_run/update_pay_run_entry_pay_run.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_run/update_pay_run_pay_run.py` & `staffology-0.1.5/staffology/api/pay_run/update_pay_run_pay_run.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_run/update_payment_date_pay_run.py` & `staffology-0.1.5/staffology/api/pay_run/update_payment_date_pay_run.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_run/ytd_pay_run.py` & `staffology-0.1.5/staffology/api/pay_run/ytd_pay_run.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_run/zeroise_pay_run_entries_pay_run.py` & `staffology-0.1.5/staffology/api/pay_run/zeroise_pay_run_entries_pay_run.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_schedule/create_pay_schedule.py` & `staffology-0.1.5/staffology/api/pay_schedule/create_pay_schedule.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_schedule/create_with_optional_ordinal_pay_schedule.py` & `staffology-0.1.5/staffology/api/pay_schedule/create_with_optional_ordinal_pay_schedule.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_schedule/delete_pay_schedule.py` & `staffology-0.1.5/staffology/api/pay_schedule/delete_pay_schedule.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_schedule/delete_with_optional_ordinal_pay_schedule.py` & `staffology-0.1.5/staffology/api/pay_schedule/delete_with_optional_ordinal_pay_schedule.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_schedule/get_all_pay_schedule.py` & `staffology-0.1.5/staffology/api/pay_schedule/get_all_pay_schedule.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_schedule/get_pay_schedule.py` & `staffology-0.1.5/staffology/api/pay_schedule/get_pay_schedule.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_schedule/get_periods_pay_schedule.py` & `staffology-0.1.5/staffology/api/pay_schedule/get_periods_pay_schedule.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_schedule/get_with_optional_ordinal_pay_schedule.py` & `staffology-0.1.5/staffology/api/pay_schedule/get_with_optional_ordinal_pay_schedule.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_schedule/save_pay_schedule.py` & `staffology-0.1.5/staffology/api/pay_schedule/save_pay_schedule.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_schedule/save_with_optional_ordinal_pay_schedule.py` & `staffology-0.1.5/staffology/api/pay_schedule/save_with_optional_ordinal_pay_schedule.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pay_schedule/update_pay_schedule_period_pay_schedule.py` & `staffology-0.1.5/staffology/api/pay_schedule/update_pay_schedule_period_pay_schedule.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/payee/create_payee.py` & `staffology-0.1.5/staffology/api/payee/create_payee.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/payee/delete_payee.py` & `staffology-0.1.5/staffology/api/payee/delete_payee.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/payee/get_payee.py` & `staffology-0.1.5/staffology/api/payee/get_payee.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/payee/index_payee.py` & `staffology-0.1.5/staffology/api/payee/index_payee.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/payee/update_payee.py` & `staffology-0.1.5/staffology/api/payee/update_payee.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pension/get_pension.py` & `staffology-0.1.5/staffology/api/pension/get_pension.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pension/remove_pension.py` & `staffology-0.1.5/staffology/api/pension/remove_pension.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pension/update_pension.py` & `staffology-0.1.5/staffology/api/pension/update_pension.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pension_scheme/contributions_for_payrun_pension_scheme.py` & `staffology-0.1.5/staffology/api/pension_scheme/contributions_for_payrun_pension_scheme.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pension_scheme/contributions_pension_scheme.py` & `staffology-0.1.5/staffology/api/pension_scheme/contributions_pension_scheme.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pension_scheme/create_pension_scheme.py` & `staffology-0.1.5/staffology/api/pension_scheme/create_pension_scheme.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pension_scheme/delete_pension_scheme.py` & `staffology-0.1.5/staffology/api/pension_scheme/delete_pension_scheme.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pension_scheme/employees_pension_scheme.py` & `staffology-0.1.5/staffology/api/pension_scheme/employees_pension_scheme.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pension_scheme/get_pension_scheme.py` & `staffology-0.1.5/staffology/api/pension_scheme/get_pension_scheme.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pension_scheme/index_pension_scheme.py` & `staffology-0.1.5/staffology/api/pension_scheme/index_pension_scheme.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pension_scheme/list_contributions_pension_scheme.py` & `staffology-0.1.5/staffology/api/pension_scheme/list_contributions_pension_scheme.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pension_scheme/mark_as_sent_pension_scheme.py` & `staffology-0.1.5/staffology/api/pension_scheme/mark_as_sent_pension_scheme.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pension_scheme/resubmit_contributions_pension_scheme.py` & `staffology-0.1.5/staffology/api/pension_scheme/resubmit_contributions_pension_scheme.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/pension_scheme/update_pension_scheme.py` & `staffology-0.1.5/staffology/api/pension_scheme/update_pension_scheme.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/post/create_post.py` & `staffology-0.1.5/staffology/api/post/create_post.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/post/delete_post.py` & `staffology-0.1.5/staffology/api/post/delete_post.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/post/get_post.py` & `staffology-0.1.5/staffology/api/post/get_post.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/post/index_post.py` & `staffology-0.1.5/staffology/api/post/index_post.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/post/update_post.py` & `staffology-0.1.5/staffology/api/post/update_post.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/processing_note/add_document_processing_note.py` & `staffology-0.1.5/staffology/api/processing_note/add_document_processing_note.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/processing_note/create_processing_note.py` & `staffology-0.1.5/staffology/api/processing_note/create_processing_note.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/processing_note/delete_document_processing_note.py` & `staffology-0.1.5/staffology/api/processing_note/delete_document_processing_note.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/processing_note/get_document_processing_note.py` & `staffology-0.1.5/staffology/api/processing_note/get_document_processing_note.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/processing_note/get_processing_note.py` & `staffology-0.1.5/staffology/api/processing_note/get_processing_note.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/processing_note/list_processing_note.py` & `staffology-0.1.5/staffology/api/processing_note/list_processing_note.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/report_pack/create_report_pack.py` & `staffology-0.1.5/staffology/api/report_pack/create_report_pack.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/report_pack/delete_report_pack.py` & `staffology-0.1.5/staffology/api/report_pack/delete_report_pack.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/report_pack/get_report_pack.py` & `staffology-0.1.5/staffology/api/report_pack/get_report_pack.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/report_pack/index_report_pack.py` & `staffology-0.1.5/staffology/api/report_pack/index_report_pack.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/report_pack/update_report_pack.py` & `staffology-0.1.5/staffology/api/report_pack/update_report_pack.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/ae_assessments_reports.py` & `staffology-0.1.5/staffology/api/reports/ae_assessments_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/aeo_statement_reports.py` & `staffology-0.1.5/staffology/api/reports/aeo_statement_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/analysis_reports.py` & `staffology-0.1.5/staffology/api/reports/analysis_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/bank_payment_instructions_reports.py` & `staffology-0.1.5/staffology/api/reports/bank_payment_instructions_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/cis_300_reports.py` & `staffology-0.1.5/staffology/api/reports/cis_300_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/cis_statement_reports.py` & `staffology-0.1.5/staffology/api/reports/cis_statement_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/cis_sub_contractor_summary_reports.py` & `staffology-0.1.5/staffology/api/reports/cis_sub_contractor_summary_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/cost_analysis_reports.py` & `staffology-0.1.5/staffology/api/reports/cost_analysis_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/cost_of_employment_reports.py` & `staffology-0.1.5/staffology/api/reports/cost_of_employment_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/email_p45_reports.py` & `staffology-0.1.5/staffology/api/reports/email_p45_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/email_p60_multiple_reports.py` & `staffology-0.1.5/staffology/api/reports/email_p60_multiple_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/email_p60_reports.py` & `staffology-0.1.5/staffology/api/reports/email_p60_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/employee_benefits_reports.py` & `staffology-0.1.5/staffology/api/reports/employee_benefits_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/employee_export_reports.py` & `staffology-0.1.5/staffology/api/reports/employee_export_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/employer_export_reports.py` & `staffology-0.1.5/staffology/api/reports/employer_export_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/example_payslip_reports.py` & `staffology-0.1.5/staffology/api/reports/example_payslip_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/exb_reports.py` & `staffology-0.1.5/staffology/api/reports/exb_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/fps_reports.py` & `staffology-0.1.5/staffology/api/reports/fps_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/full_summary_of_pay_reports.py` & `staffology-0.1.5/staffology/api/reports/full_summary_of_pay_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/furlough_report_reports.py` & `staffology-0.1.5/staffology/api/reports/furlough_report_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/get_pay_run_csv_reports.py` & `staffology-0.1.5/staffology/api/reports/get_pay_run_csv_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/gross_to_net_reports.py` & `staffology-0.1.5/staffology/api/reports/gross_to_net_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/holiday_reports.py` & `staffology-0.1.5/staffology/api/reports/holiday_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/hourly_pay_reports.py` & `staffology-0.1.5/staffology/api/reports/hourly_pay_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/ni_letter_validation_report_employees_reports.py` & `staffology-0.1.5/staffology/api/reports/ni_letter_validation_report_employees_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/ni_letter_validation_report_reports.py` & `staffology-0.1.5/staffology/api/reports/ni_letter_validation_report_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/p11_detailed_multiple_reports.py` & `staffology-0.1.5/staffology/api/reports/p11_detailed_multiple_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/p11_detailed_reports.py` & `staffology-0.1.5/staffology/api/reports/p11_detailed_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/p11_reports.py` & `staffology-0.1.5/staffology/api/reports/p11_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/p11d_reports.py` & `staffology-0.1.5/staffology/api/reports/p11d_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/p30_reports.py` & `staffology-0.1.5/staffology/api/reports/p30_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/p32_reports.py` & `staffology-0.1.5/staffology/api/reports/p32_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/p45_reports.py` & `staffology-0.1.5/staffology/api/reports/p45_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/p60_multiple_reports.py` & `staffology-0.1.5/staffology/api/reports/p60_multiple_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/p60_reports.py` & `staffology-0.1.5/staffology/api/reports/p60_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/papdis_file_reports.py` & `staffology-0.1.5/staffology/api/reports/papdis_file_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/pay_run_csv_reports.py` & `staffology-0.1.5/staffology/api/reports/pay_run_csv_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/pay_run_payments_reports.py` & `staffology-0.1.5/staffology/api/reports/pay_run_payments_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/pay_run_summary_reports.py` & `staffology-0.1.5/staffology/api/reports/pay_run_summary_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/payrun_ytd_reports.py` & `staffology-0.1.5/staffology/api/reports/payrun_ytd_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/payslip_reports.py` & `staffology-0.1.5/staffology/api/reports/payslip_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/payslips_reports.py` & `staffology-0.1.5/staffology/api/reports/payslips_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/right_to_work_reports.py` & `staffology-0.1.5/staffology/api/reports/right_to_work_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/statutory_pay_reports.py` & `staffology-0.1.5/staffology/api/reports/statutory_pay_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/tax_code_changes_reports.py` & `staffology-0.1.5/staffology/api/reports/tax_code_changes_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/umbrella_reconciliation_reports.py` & `staffology-0.1.5/staffology/api/reports/umbrella_reconciliation_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/variance_report_reports.py` & `staffology-0.1.5/staffology/api/reports/variance_report_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/reports/ytd_reports.py` & `staffology-0.1.5/staffology/api/reports/ytd_reports.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tag/create_tag.py` & `staffology-0.1.5/staffology/api/tag/create_tag.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tag/delete_tag.py` & `staffology-0.1.5/staffology/api/tag/delete_tag.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tag/get_tag.py` & `staffology-0.1.5/staffology/api/tag/get_tag.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tag/index_tag.py` & `staffology-0.1.5/staffology/api/tag/index_tag.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tag/update_tag.py` & `staffology-0.1.5/staffology/api/tag/update_tag.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tenant/add_admin_user_tenant.py` & `staffology-0.1.5/staffology/api/tenant/add_admin_user_tenant.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tenant/admin_users_tenant.py` & `staffology-0.1.5/staffology/api/tenant/admin_users_tenant.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tenant/bill_tenant.py` & `staffology-0.1.5/staffology/api/tenant/bill_tenant.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tenant/bills_tenant.py` & `staffology-0.1.5/staffology/api/tenant/bills_tenant.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tenant/create_bills_tenant.py` & `staffology-0.1.5/staffology/api/tenant/create_bills_tenant.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tenant/create_tenant.py` & `staffology-0.1.5/staffology/api/tenant/create_tenant.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tenant/disabled_tenant.py` & `staffology-0.1.5/staffology/api/tenant/disabled_tenant.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tenant/employer_creation_tenant.py` & `staffology-0.1.5/staffology/api/tenant/employer_creation_tenant.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tenant/employer_usage_tenant.py` & `staffology-0.1.5/staffology/api/tenant/employer_usage_tenant.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tenant/employer_users_tenant.py` & `staffology-0.1.5/staffology/api/tenant/employer_users_tenant.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tenant/get_rti_submission_settings_tenant.py` & `staffology-0.1.5/staffology/api/tenant/get_rti_submission_settings_tenant.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tenant/get_tenant.py` & `staffology-0.1.5/staffology/api/tenant/get_tenant.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tenant/get_users_with_no_billable_activity_tenant.py` & `staffology-0.1.5/staffology/api/tenant/get_users_with_no_billable_activity_tenant.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tenant/remove_admin_user_tenant.py` & `staffology-0.1.5/staffology/api/tenant/remove_admin_user_tenant.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tenant/set_accounting_id_tenant.py` & `staffology-0.1.5/staffology/api/tenant/set_accounting_id_tenant.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tenant/set_bureau_redirect_email_address_tenant.py` & `staffology-0.1.5/staffology/api/tenant/set_bureau_redirect_email_address_tenant.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tenant/set_monthly_minimum_tenant.py` & `staffology-0.1.5/staffology/api/tenant/set_monthly_minimum_tenant.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tenant/set_omnipresent_role_tenant.py` & `staffology-0.1.5/staffology/api/tenant/set_omnipresent_role_tenant.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tenant/set_tenant_tenant.py` & `staffology-0.1.5/staffology/api/tenant/set_tenant_tenant.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tenant/update_bill_tenant.py` & `staffology-0.1.5/staffology/api/tenant/update_bill_tenant.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tenant/update_css_colors_tenant.py` & `staffology-0.1.5/staffology/api/tenant/update_css_colors_tenant.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tenant/update_css_tenant.py` & `staffology-0.1.5/staffology/api/tenant/update_css_tenant.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tenant/update_fav_icon_tenant.py` & `staffology-0.1.5/staffology/api/tenant/update_fav_icon_tenant.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tenant/update_logo_tenant.py` & `staffology-0.1.5/staffology/api/tenant/update_logo_tenant.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tenant/update_rti_submission_settings_tenant.py` & `staffology-0.1.5/staffology/api/tenant/update_rti_submission_settings_tenant.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tenant/update_tenant.py` & `staffology-0.1.5/staffology/api/tenant/update_tenant.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tenant/usage_tenant.py` & `staffology-0.1.5/staffology/api/tenant/usage_tenant.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tenant/user_bills_tenant.py` & `staffology-0.1.5/staffology/api/tenant/user_bills_tenant.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tenant/user_employers_tenant.py` & `staffology-0.1.5/staffology/api/tenant/user_employers_tenant.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tenant/user_tenant.py` & `staffology-0.1.5/staffology/api/tenant/user_tenant.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tenant/users_search_tenant.py` & `staffology-0.1.5/staffology/api/tenant/users_search_tenant.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tenant/users_tenant.py` & `staffology-0.1.5/staffology/api/tenant/users_tenant.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tenant/weekly_activity_tenant.py` & `staffology-0.1.5/staffology/api/tenant/weekly_activity_tenant.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tenant_email/get_email_tenant_email.py` & `staffology-0.1.5/staffology/api/tenant_email/get_email_tenant_email.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tenant_email/get_mail_settings_tenant_email.py` & `staffology-0.1.5/staffology/api/tenant_email/get_mail_settings_tenant_email.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tenant_email/index_tenant_email.py` & `staffology-0.1.5/staffology/api/tenant_email/index_tenant_email.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tenant_email/resend_email_tenant_email.py` & `staffology-0.1.5/staffology/api/tenant_email/resend_email_tenant_email.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tenant_email/test_mail_settings_tenant_email.py` & `staffology-0.1.5/staffology/api/tenant_email/test_mail_settings_tenant_email.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/tenant_email/update_mail_settings_tenant_email.py` & `staffology-0.1.5/staffology/api/tenant_email/update_mail_settings_tenant_email.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/webhook/create_webhook.py` & `staffology-0.1.5/staffology/api/webhook/create_webhook.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/webhook/delete_webhook.py` & `staffology-0.1.5/staffology/api/webhook/delete_webhook.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/webhook/get_webhook.py` & `staffology-0.1.5/staffology/api/webhook/get_webhook.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/webhook/index_webhook.py` & `staffology-0.1.5/staffology/api/webhook/index_webhook.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/webhook/payload_webhook.py` & `staffology-0.1.5/staffology/api/webhook/payload_webhook.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/webhook/payloads_webhook.py` & `staffology-0.1.5/staffology/api/webhook/payloads_webhook.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/webhook/sample_webhook.py` & `staffology-0.1.5/staffology/api/webhook/sample_webhook.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/webhook/update_webhook.py` & `staffology-0.1.5/staffology/api/webhook/update_webhook.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/working_pattern/create_working_pattern.py` & `staffology-0.1.5/staffology/api/working_pattern/create_working_pattern.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/working_pattern/delete_working_pattern.py` & `staffology-0.1.5/staffology/api/working_pattern/delete_working_pattern.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/working_pattern/get_working_pattern.py` & `staffology-0.1.5/staffology/api/working_pattern/get_working_pattern.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/working_pattern/index_working_pattern.py` & `staffology-0.1.5/staffology/api/working_pattern/index_working_pattern.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/api/working_pattern/update_working_pattern.py` & `staffology-0.1.5/staffology/api/working_pattern/update_working_pattern.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/client.py` & `staffology-0.1.5/staffology/client.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/__init__.py` & `staffology-0.1.5/staffology/models/__init__.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/add_document_attachment_order_multipart_data.py` & `staffology-0.1.5/staffology/models/add_document_attachment_order_multipart_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/add_document_leave_multipart_data.py` & `staffology-0.1.5/staffology/models/add_document_leave_multipart_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/add_document_loan_multipart_data.py` & `staffology-0.1.5/staffology/models/add_document_loan_multipart_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/add_document_note_multipart_data.py` & `staffology-0.1.5/staffology/models/add_document_note_multipart_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/add_document_processing_note_multipart_data.py` & `staffology-0.1.5/staffology/models/add_document_processing_note_multipart_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/address.py` & `staffology-0.1.5/staffology/models/address.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/ae_action.py` & `staffology-0.1.5/staffology/models/ae_action.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/ae_assessment.py` & `staffology-0.1.5/staffology/models/ae_assessment.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/ae_assessment_action.py` & `staffology-0.1.5/staffology/models/ae_assessment_action.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/ae_employee_state.py` & `staffology-0.1.5/staffology/models/ae_employee_state.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/ae_exclusion_code.py` & `staffology-0.1.5/staffology/models/ae_exclusion_code.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/analysis_report.py` & `staffology-0.1.5/staffology/models/analysis_report.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/analysis_report_line.py` & `staffology-0.1.5/staffology/models/analysis_report_line.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/analysis_report_line_value.py` & `staffology-0.1.5/staffology/models/analysis_report_line_value.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/analysis_report_report_response.py` & `staffology-0.1.5/staffology/models/analysis_report_report_response.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/apply_year_end_employer_json_body.py` & `staffology-0.1.5/staffology/models/apply_year_end_employer_json_body.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/attachment_order.py` & `staffology-0.1.5/staffology/models/attachment_order.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/attachment_order_payment.py` & `staffology-0.1.5/staffology/models/attachment_order_payment.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/attachment_order_report_response.py` & `staffology-0.1.5/staffology/models/attachment_order_report_response.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/attachment_order_type.py` & `staffology-0.1.5/staffology/models/attachment_order_type.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/auto_enrolment.py` & `staffology-0.1.5/staffology/models/auto_enrolment.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/auto_enrolment_settings.py` & `staffology-0.1.5/staffology/models/auto_enrolment_settings.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/automation_settings.py` & `staffology-0.1.5/staffology/models/automation_settings.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/average_weekly_earnings.py` & `staffology-0.1.5/staffology/models/average_weekly_earnings.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/bank_details.py` & `staffology-0.1.5/staffology/models/bank_details.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/bank_payment_instruction.py` & `staffology-0.1.5/staffology/models/bank_payment_instruction.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/bank_payment_instruction_report_response.py` & `staffology-0.1.5/staffology/models/bank_payment_instruction_report_response.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/bank_payment_instructions_csv_format.py` & `staffology-0.1.5/staffology/models/bank_payment_instructions_csv_format.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/benefit.py` & `staffology-0.1.5/staffology/models/benefit.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/benefit_details_car.py` & `staffology-0.1.5/staffology/models/benefit_details_car.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/benefit_details_class_1a_type.py` & `staffology-0.1.5/staffology/models/benefit_details_class_1a_type.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/benefit_details_loan.py` & `staffology-0.1.5/staffology/models/benefit_details_loan.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/benefit_details_non_class_1a_type.py` & `staffology-0.1.5/staffology/models/benefit_details_non_class_1a_type.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/benefit_details_payment_type.py` & `staffology-0.1.5/staffology/models/benefit_details_payment_type.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/benefit_details_use_of_asset_type.py` & `staffology-0.1.5/staffology/models/benefit_details_use_of_asset_type.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/benefit_type.py` & `staffology-0.1.5/staffology/models/benefit_type.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/bureau_settings.py` & `staffology-0.1.5/staffology/models/bureau_settings.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/calendar_entry.py` & `staffology-0.1.5/staffology/models/calendar_entry.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/calendar_entry_type.py` & `staffology-0.1.5/staffology/models/calendar_entry_type.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/car_charge.py` & `staffology-0.1.5/staffology/models/car_charge.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/car_charge_rate.py` & `staffology-0.1.5/staffology/models/car_charge_rate.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/change_summary.py` & `staffology-0.1.5/staffology/models/change_summary.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/cis_300.py` & `staffology-0.1.5/staffology/models/cis_300.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/cis_300_declarations.py` & `staffology-0.1.5/staffology/models/cis_300_declarations.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/cis_300_report_response.py` & `staffology-0.1.5/staffology/models/cis_300_report_response.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/cis_contractor.py` & `staffology-0.1.5/staffology/models/cis_contractor.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/cis_details.py` & `staffology-0.1.5/staffology/models/cis_details.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/cis_partnership.py` & `staffology-0.1.5/staffology/models/cis_partnership.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/cis_request.py` & `staffology-0.1.5/staffology/models/cis_request.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/cis_return.py` & `staffology-0.1.5/staffology/models/cis_return.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/cis_statement.py` & `staffology-0.1.5/staffology/models/cis_statement.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/cis_statement_list_report_response.py` & `staffology-0.1.5/staffology/models/cis_statement_list_report_response.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/cis_sub_contractor.py` & `staffology-0.1.5/staffology/models/cis_sub_contractor.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/cis_sub_contractor_summary.py` & `staffology-0.1.5/staffology/models/cis_sub_contractor_summary.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/cis_sub_contractor_summary_list_report_response.py` & `staffology-0.1.5/staffology/models/cis_sub_contractor_summary_list_report_response.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/cis_verification.py` & `staffology-0.1.5/staffology/models/cis_verification.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/cis_verification_details.py` & `staffology-0.1.5/staffology/models/cis_verification_details.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/cookie_preference.py` & `staffology-0.1.5/staffology/models/cookie_preference.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/cost_analysis_report.py` & `staffology-0.1.5/staffology/models/cost_analysis_report.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/cost_analysis_report_report_response.py` & `staffology-0.1.5/staffology/models/cost_analysis_report_report_response.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/cost_breakdown.py` & `staffology-0.1.5/staffology/models/cost_breakdown.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/cost_breakdown_breakdown.py` & `staffology-0.1.5/staffology/models/cost_breakdown_breakdown.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/cost_of_employment_report.py` & `staffology-0.1.5/staffology/models/cost_of_employment_report.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/cost_of_employment_report_line.py` & `staffology-0.1.5/staffology/models/cost_of_employment_report_line.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/cost_of_employment_report_report_response.py` & `staffology-0.1.5/staffology/models/cost_of_employment_report_report_response.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/country.py` & `staffology-0.1.5/staffology/models/country.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/department.py` & `staffology-0.1.5/staffology/models/department.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/department_membership.py` & `staffology-0.1.5/staffology/models/department_membership.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/direct_debit_mandate.py` & `staffology-0.1.5/staffology/models/direct_debit_mandate.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/directorship_details.py` & `staffology-0.1.5/staffology/models/directorship_details.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/dps_notice.py` & `staffology-0.1.5/staffology/models/dps_notice.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/dps_settings.py` & `staffology-0.1.5/staffology/models/dps_settings.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/email_attachment.py` & `staffology-0.1.5/staffology/models/email_attachment.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/emp_refs.py` & `staffology-0.1.5/staffology/models/emp_refs.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/employee.py` & `staffology-0.1.5/staffology/models/employee.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/employee_benefits_report.py` & `staffology-0.1.5/staffology/models/employee_benefits_report.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/employee_benefits_report_report_response.py` & `staffology-0.1.5/staffology/models/employee_benefits_report_report_response.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/employee_ytd_values.py` & `staffology-0.1.5/staffology/models/employee_ytd_values.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/employer.py` & `staffology-0.1.5/staffology/models/employer.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/employer_defaults.py` & `staffology-0.1.5/staffology/models/employer_defaults.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/employer_email.py` & `staffology-0.1.5/staffology/models/employer_email.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/employer_group.py` & `staffology-0.1.5/staffology/models/employer_group.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/employer_group_membership.py` & `staffology-0.1.5/staffology/models/employer_group_membership.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/employer_item.py` & `staffology-0.1.5/staffology/models/employer_item.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/employer_opening_balances.py` & `staffology-0.1.5/staffology/models/employer_opening_balances.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/employer_settings.py` & `staffology-0.1.5/staffology/models/employer_settings.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/employer_template.py` & `staffology-0.1.5/staffology/models/employer_template.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/employer_template_type.py` & `staffology-0.1.5/staffology/models/employer_template_type.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/employment_details.py` & `staffology-0.1.5/staffology/models/employment_details.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/entity_type.py` & `staffology-0.1.5/staffology/models/entity_type.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/eps.py` & `staffology-0.1.5/staffology/models/eps.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/eps_account.py` & `staffology-0.1.5/staffology/models/eps_account.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/eps_apprenticeship_levy.py` & `staffology-0.1.5/staffology/models/eps_apprenticeship_levy.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/eps_de_minimis_state_aid.py` & `staffology-0.1.5/staffology/models/eps_de_minimis_state_aid.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/eps_final_submission.py` & `staffology-0.1.5/staffology/models/eps_final_submission.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/exb.py` & `staffology-0.1.5/staffology/models/exb.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/exb_declarations.py` & `staffology-0.1.5/staffology/models/exb_declarations.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/exb_employer.py` & `staffology-0.1.5/staffology/models/exb_employer.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/exb_p11_db.py` & `staffology-0.1.5/staffology/models/exb_p11_db.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/exb_p11_db_class_1a.py` & `staffology-0.1.5/staffology/models/exb_p11_db_class_1a.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/exb_p11_db_class_1a_adjustment.py` & `staffology-0.1.5/staffology/models/exb_p11_db_class_1a_adjustment.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/exb_p11_db_class_1a_adjustments.py` & `staffology-0.1.5/staffology/models/exb_p11_db_class_1a_adjustments.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/exb_p11_db_class_1a_total_benefit.py` & `staffology-0.1.5/staffology/models/exb_p11_db_class_1a_total_benefit.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/exb_p11d.py` & `staffology-0.1.5/staffology/models/exb_p11d.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/exb_p11d_employee.py` & `staffology-0.1.5/staffology/models/exb_p11d_employee.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/exb_report_response.py` & `staffology-0.1.5/staffology/models/exb_report_response.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/expenses_and_benefits.py` & `staffology-0.1.5/staffology/models/expenses_and_benefits.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/external_data_company.py` & `staffology-0.1.5/staffology/models/external_data_company.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/external_data_provider.py` & `staffology-0.1.5/staffology/models/external_data_provider.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/external_data_provider_id.py` & `staffology-0.1.5/staffology/models/external_data_provider_id.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/external_employee_mapping.py` & `staffology-0.1.5/staffology/models/external_employee_mapping.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/external_provider_conversation.py` & `staffology-0.1.5/staffology/models/external_provider_conversation.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/field_modification.py` & `staffology-0.1.5/staffology/models/field_modification.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/finalise_pay_run_pay_run_json_body.py` & `staffology-0.1.5/staffology/models/finalise_pay_run_pay_run_json_body.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/fixed_code.py` & `staffology-0.1.5/staffology/models/fixed_code.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/fps.py` & `staffology-0.1.5/staffology/models/fps.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/fps_benefit.py` & `staffology-0.1.5/staffology/models/fps_benefit.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/fps_car.py` & `staffology-0.1.5/staffology/models/fps_car.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/fps_car_fuel.py` & `staffology-0.1.5/staffology/models/fps_car_fuel.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/fps_employee.py` & `staffology-0.1.5/staffology/models/fps_employee.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/fps_employee_details.py` & `staffology-0.1.5/staffology/models/fps_employee_details.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/fps_employee_details_partner_details.py` & `staffology-0.1.5/staffology/models/fps_employee_details_partner_details.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/fps_employee_figs_to_date.py` & `staffology-0.1.5/staffology/models/fps_employee_figs_to_date.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/fps_employee_flexible_drawdown.py` & `staffology-0.1.5/staffology/models/fps_employee_flexible_drawdown.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/fps_employee_n_iletters_and_values.py` & `staffology-0.1.5/staffology/models/fps_employee_n_iletters_and_values.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/fps_employee_payment.py` & `staffology-0.1.5/staffology/models/fps_employee_payment.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/fps_employee_starter.py` & `staffology-0.1.5/staffology/models/fps_employee_starter.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/fps_employee_starter_occ_pension.py` & `staffology-0.1.5/staffology/models/fps_employee_starter_occ_pension.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/fps_employee_tax_code.py` & `staffology-0.1.5/staffology/models/fps_employee_tax_code.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/fps_employee_trivial_commutation_payment.py` & `staffology-0.1.5/staffology/models/fps_employee_trivial_commutation_payment.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/fps_employer_pay_id_changed.py` & `staffology-0.1.5/staffology/models/fps_employer_pay_id_changed.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/fps_employment.py` & `staffology-0.1.5/staffology/models/fps_employment.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/fps_fields.py` & `staffology-0.1.5/staffology/models/fps_fields.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/fps_late_reason.py` & `staffology-0.1.5/staffology/models/fps_late_reason.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/fps_report_response.py` & `staffology-0.1.5/staffology/models/fps_report_response.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/from_to_dates.py` & `staffology-0.1.5/staffology/models/from_to_dates.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/full_payment_submission.py` & `staffology-0.1.5/staffology/models/full_payment_submission.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/full_summary_of_pay_report.py` & `staffology-0.1.5/staffology/models/full_summary_of_pay_report.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/full_summary_of_pay_report_line.py` & `staffology-0.1.5/staffology/models/full_summary_of_pay_report_line.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/full_summary_of_pay_report_report_response.py` & `staffology-0.1.5/staffology/models/full_summary_of_pay_report_report_response.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/furlough_calculation_basis.py` & `staffology-0.1.5/staffology/models/furlough_calculation_basis.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/furlough_report.py` & `staffology-0.1.5/staffology/models/furlough_report.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/furlough_report_line.py` & `staffology-0.1.5/staffology/models/furlough_report_line.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/furlough_report_report_response.py` & `staffology-0.1.5/staffology/models/furlough_report_report_response.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/gov_talk.py` & `staffology-0.1.5/staffology/models/gov_talk.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/gov_talk_error.py` & `staffology-0.1.5/staffology/models/gov_talk_error.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/gov_talk_submission.py` & `staffology-0.1.5/staffology/models/gov_talk_submission.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/gross_to_net_report.py` & `staffology-0.1.5/staffology/models/gross_to_net_report.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/gross_to_net_report_cis_line.py` & `staffology-0.1.5/staffology/models/gross_to_net_report_cis_line.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/gross_to_net_report_line.py` & `staffology-0.1.5/staffology/models/gross_to_net_report_line.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/gross_to_net_report_report_response.py` & `staffology-0.1.5/staffology/models/gross_to_net_report_report_response.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/hmrc_details.py` & `staffology-0.1.5/staffology/models/hmrc_details.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/hmrc_liability.py` & `staffology-0.1.5/staffology/models/hmrc_liability.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/hmrc_payment.py` & `staffology-0.1.5/staffology/models/hmrc_payment.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/holiday_report.py` & `staffology-0.1.5/staffology/models/holiday_report.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/holiday_report_line.py` & `staffology-0.1.5/staffology/models/holiday_report_line.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/holiday_report_report_response.py` & `staffology-0.1.5/staffology/models/holiday_report_report_response.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/hourly_pay_report.py` & `staffology-0.1.5/staffology/models/hourly_pay_report.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/hourly_pay_report_line.py` & `staffology-0.1.5/staffology/models/hourly_pay_report_line.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/hourly_pay_report_report_response.py` & `staffology-0.1.5/staffology/models/hourly_pay_report_report_response.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/html_email_settings.py` & `staffology-0.1.5/staffology/models/html_email_settings.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/import_csv_employee_multipart_data.py` & `staffology-0.1.5/staffology/models/import_csv_employee_multipart_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/import_csv_employer_multipart_data.py` & `staffology-0.1.5/staffology/models/import_csv_employer_multipart_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/invitation.py` & `staffology-0.1.5/staffology/models/invitation.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/item.py` & `staffology-0.1.5/staffology/models/item.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/item_list_report_response.py` & `staffology-0.1.5/staffology/models/item_list_report_response.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/leave.py` & `staffology-0.1.5/staffology/models/leave.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/leave_settings.py` & `staffology-0.1.5/staffology/models/leave_settings.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/leave_type.py` & `staffology-0.1.5/staffology/models/leave_type.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/leaver_details.py` & `staffology-0.1.5/staffology/models/leaver_details.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/linked_piw.py` & `staffology-0.1.5/staffology/models/linked_piw.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/loan.py` & `staffology-0.1.5/staffology/models/loan.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/loan_charge.py` & `staffology-0.1.5/staffology/models/loan_charge.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/log_entry.py` & `staffology-0.1.5/staffology/models/log_entry.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/mail_settings.py` & `staffology-0.1.5/staffology/models/mail_settings.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/marital_status.py` & `staffology-0.1.5/staffology/models/marital_status.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/mileage_allowance_payments_rate.py` & `staffology-0.1.5/staffology/models/mileage_allowance_payments_rate.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/monthly_minimum.py` & `staffology-0.1.5/staffology/models/monthly_minimum.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/national_insurance_calculation.py` & `staffology-0.1.5/staffology/models/national_insurance_calculation.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/national_insurance_calculation_base.py` & `staffology-0.1.5/staffology/models/national_insurance_calculation_base.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/national_insurance_calculation_period_values.py` & `staffology-0.1.5/staffology/models/national_insurance_calculation_period_values.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/national_insurance_code.py` & `staffology-0.1.5/staffology/models/national_insurance_code.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/national_minimum_wage.py` & `staffology-0.1.5/staffology/models/national_minimum_wage.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/ni_letter_error.py` & `staffology-0.1.5/staffology/models/ni_letter_error.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/ni_letter_validation_report.py` & `staffology-0.1.5/staffology/models/ni_letter_validation_report.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/ni_letter_validation_report_line.py` & `staffology-0.1.5/staffology/models/ni_letter_validation_report_line.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/ni_letter_validation_report_report_response.py` & `staffology-0.1.5/staffology/models/ni_letter_validation_report_report_response.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/nic_summary.py` & `staffology-0.1.5/staffology/models/nic_summary.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/nominal_code_mapping.py` & `staffology-0.1.5/staffology/models/nominal_code_mapping.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/note.py` & `staffology-0.1.5/staffology/models/note.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/nvr.py` & `staffology-0.1.5/staffology/models/nvr.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/nvr_employee.py` & `staffology-0.1.5/staffology/models/nvr_employee.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/nvr_employee_details.py` & `staffology-0.1.5/staffology/models/nvr_employee_details.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/nvr_employment.py` & `staffology-0.1.5/staffology/models/nvr_employment.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/nvr_request.py` & `staffology-0.1.5/staffology/models/nvr_request.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/opening_balances.py` & `staffology-0.1.5/staffology/models/opening_balances.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/overseas_employer_details.py` & `staffology-0.1.5/staffology/models/overseas_employer_details.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/overseas_secondment_status.py` & `staffology-0.1.5/staffology/models/overseas_secondment_status.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/p11.py` & `staffology-0.1.5/staffology/models/p11.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/p11_detailed.py` & `staffology-0.1.5/staffology/models/p11_detailed.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/p11_detailed_ni_values.py` & `staffology-0.1.5/staffology/models/p11_detailed_ni_values.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/p11_detailed_report_response.py` & `staffology-0.1.5/staffology/models/p11_detailed_report_response.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/p11_line.py` & `staffology-0.1.5/staffology/models/p11_line.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/p11_ni_and_stat_payments_line.py` & `staffology-0.1.5/staffology/models/p11_ni_and_stat_payments_line.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/p11_ni_and_stat_payments_totals_line.py` & `staffology-0.1.5/staffology/models/p11_ni_and_stat_payments_totals_line.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/p11_ni_values.py` & `staffology-0.1.5/staffology/models/p11_ni_values.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/p11_paye_line.py` & `staffology-0.1.5/staffology/models/p11_paye_line.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/p11_paye_summary.py` & `staffology-0.1.5/staffology/models/p11_paye_summary.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/p11_paye_totals_line.py` & `staffology-0.1.5/staffology/models/p11_paye_totals_line.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/p11_report_response.py` & `staffology-0.1.5/staffology/models/p11_report_response.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/p11d_asset_available.py` & `staffology-0.1.5/staffology/models/p11d_asset_available.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/p11d_asset_available_collection.py` & `staffology-0.1.5/staffology/models/p11d_asset_available_collection.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/p11d_asset_transferred_collection.py` & `staffology-0.1.5/staffology/models/p11d_asset_transferred_collection.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/p11d_car.py` & `staffology-0.1.5/staffology/models/p11d_car.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/p11d_car_collection.py` & `staffology-0.1.5/staffology/models/p11d_car_collection.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/p11d_car_free_fuel_withdrawn.py` & `staffology-0.1.5/staffology/models/p11d_car_free_fuel_withdrawn.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/p11d_desc_other.py` & `staffology-0.1.5/staffology/models/p11d_desc_other.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/p11d_expenses.py` & `staffology-0.1.5/staffology/models/p11d_expenses.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/p11d_loan.py` & `staffology-0.1.5/staffology/models/p11d_loan.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/p11d_loan_collection.py` & `staffology-0.1.5/staffology/models/p11d_loan_collection.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/p11d_other.py` & `staffology-0.1.5/staffology/models/p11d_other.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/p11d_payment_collection.py` & `staffology-0.1.5/staffology/models/p11d_payment_collection.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/p11d_single_item.py` & `staffology-0.1.5/staffology/models/p11d_single_item.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/p11d_vans.py` & `staffology-0.1.5/staffology/models/p11d_vans.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/p32.py` & `staffology-0.1.5/staffology/models/p32.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/p32_report_response.py` & `staffology-0.1.5/staffology/models/p32_report_response.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/papdis_document.py` & `staffology-0.1.5/staffology/models/papdis_document.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/papdis_document_report_response.py` & `staffology-0.1.5/staffology/models/papdis_document_report_response.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/papdis_employee.py` & `staffology-0.1.5/staffology/models/papdis_employee.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/papdis_employee_assessment.py` & `staffology-0.1.5/staffology/models/papdis_employee_assessment.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/papdis_employee_contact.py` & `staffology-0.1.5/staffology/models/papdis_employee_contact.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/papdis_employee_contact_postal_address.py` & `staffology-0.1.5/staffology/models/papdis_employee_contact_postal_address.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/papdis_employee_contribution.py` & `staffology-0.1.5/staffology/models/papdis_employee_contribution.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/papdis_employee_exit.py` & `staffology-0.1.5/staffology/models/papdis_employee_exit.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/papdis_employee_identity.py` & `staffology-0.1.5/staffology/models/papdis_employee_identity.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/papdis_employee_name.py` & `staffology-0.1.5/staffology/models/papdis_employee_name.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/papdis_employee_pay.py` & `staffology-0.1.5/staffology/models/papdis_employee_pay.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/papdis_employer.py` & `staffology-0.1.5/staffology/models/papdis_employer.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/papdis_message_function_code.py` & `staffology-0.1.5/staffology/models/papdis_message_function_code.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/papdis_payroll_period.py` & `staffology-0.1.5/staffology/models/papdis_payroll_period.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/papdis_pension_provider.py` & `staffology-0.1.5/staffology/models/papdis_pension_provider.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/partner_details.py` & `staffology-0.1.5/staffology/models/partner_details.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/pay_code.py` & `staffology-0.1.5/staffology/models/pay_code.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/pay_code_calculation_type.py` & `staffology-0.1.5/staffology/models/pay_code_calculation_type.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/pay_line.py` & `staffology-0.1.5/staffology/models/pay_line.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/pay_options.py` & `staffology-0.1.5/staffology/models/pay_options.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/pay_options_import.py` & `staffology-0.1.5/staffology/models/pay_options_import.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/pay_run.py` & `staffology-0.1.5/staffology/models/pay_run.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/pay_run_changes.py` & `staffology-0.1.5/staffology/models/pay_run_changes.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/pay_run_cost_summary.py` & `staffology-0.1.5/staffology/models/pay_run_cost_summary.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/pay_run_csv_type.py` & `staffology-0.1.5/staffology/models/pay_run_csv_type.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/pay_run_entry.py` & `staffology-0.1.5/staffology/models/pay_run_entry.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/pay_run_journal.py` & `staffology-0.1.5/staffology/models/pay_run_journal.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/pay_run_payment.py` & `staffology-0.1.5/staffology/models/pay_run_payment.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/pay_run_state.py` & `staffology-0.1.5/staffology/models/pay_run_state.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/pay_run_state_change.py` & `staffology-0.1.5/staffology/models/pay_run_state_change.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/pay_run_summary_line.py` & `staffology-0.1.5/staffology/models/pay_run_summary_line.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/pay_run_summary_line_i_enumerable_report_response.py` & `staffology-0.1.5/staffology/models/pay_run_summary_line_i_enumerable_report_response.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/pay_run_totals.py` & `staffology-0.1.5/staffology/models/pay_run_totals.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/pay_schedule.py` & `staffology-0.1.5/staffology/models/pay_schedule.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/pay_schedule_period.py` & `staffology-0.1.5/staffology/models/pay_schedule_period.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/pay_schedule_period_event.py` & `staffology-0.1.5/staffology/models/pay_schedule_period_event.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/pay_schedule_period_events_config.py` & `staffology-0.1.5/staffology/models/pay_schedule_period_events_config.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/payee.py` & `staffology-0.1.5/staffology/models/payee.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/payee_type.py` & `staffology-0.1.5/staffology/models/payee_type.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/payment_date_type.py` & `staffology-0.1.5/staffology/models/payment_date_type.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/payments_csv_mapping.py` & `staffology-0.1.5/staffology/models/payments_csv_mapping.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/payments_csv_mapping_column.py` & `staffology-0.1.5/staffology/models/payments_csv_mapping_column.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/payroll_value_type.py` & `staffology-0.1.5/staffology/models/payroll_value_type.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/payrun_email.py` & `staffology-0.1.5/staffology/models/payrun_email.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/payrun_payments_report.py` & `staffology-0.1.5/staffology/models/payrun_payments_report.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/payrun_payments_report_report_response.py` & `staffology-0.1.5/staffology/models/payrun_payments_report_report_response.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/payslip.py` & `staffology-0.1.5/staffology/models/payslip.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/payslip_customisation.py` & `staffology-0.1.5/staffology/models/payslip_customisation.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/payslip_line.py` & `staffology-0.1.5/staffology/models/payslip_line.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/payslip_report_response.py` & `staffology-0.1.5/staffology/models/payslip_report_response.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/pdf_paper_margins.py` & `staffology-0.1.5/staffology/models/pdf_paper_margins.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/pension.py` & `staffology-0.1.5/staffology/models/pension.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/pension_administrator.py` & `staffology-0.1.5/staffology/models/pension_administrator.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/pension_contributions_submission.py` & `staffology-0.1.5/staffology/models/pension_contributions_submission.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/pension_provider.py` & `staffology-0.1.5/staffology/models/pension_provider.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/pension_scheme.py` & `staffology-0.1.5/staffology/models/pension_scheme.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/pension_selection.py` & `staffology-0.1.5/staffology/models/pension_selection.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/pension_summary.py` & `staffology-0.1.5/staffology/models/pension_summary.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/pensioner_payroll.py` & `staffology-0.1.5/staffology/models/pensioner_payroll.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/personal_details.py` & `staffology-0.1.5/staffology/models/personal_details.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/post.py` & `staffology-0.1.5/staffology/models/post.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/pro_rata_rule.py` & `staffology-0.1.5/staffology/models/pro_rata_rule.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/processing_note.py` & `staffology-0.1.5/staffology/models/processing_note.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/recoverable_amounts.py` & `staffology-0.1.5/staffology/models/recoverable_amounts.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/report.py` & `staffology-0.1.5/staffology/models/report.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/report_pack.py` & `staffology-0.1.5/staffology/models/report_pack.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/report_response.py` & `staffology-0.1.5/staffology/models/report_response.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/right_to_work.py` & `staffology-0.1.5/staffology/models/right_to_work.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/right_to_work_document_type.py` & `staffology-0.1.5/staffology/models/right_to_work_document_type.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/right_to_work_report.py` & `staffology-0.1.5/staffology/models/right_to_work_report.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/right_to_work_report_line.py` & `staffology-0.1.5/staffology/models/right_to_work_report_line.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/right_to_work_report_report_response.py` & `staffology-0.1.5/staffology/models/right_to_work_report_report_response.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/rti_agent.py` & `staffology-0.1.5/staffology/models/rti_agent.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/rti_contact.py` & `staffology-0.1.5/staffology/models/rti_contact.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/rti_employee_address.py` & `staffology-0.1.5/staffology/models/rti_employee_address.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/rti_employee_name.py` & `staffology-0.1.5/staffology/models/rti_employee_name.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/rti_sender_type.py` & `staffology-0.1.5/staffology/models/rti_sender_type.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/rti_submission_settings.py` & `staffology-0.1.5/staffology/models/rti_submission_settings.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/rti_validation_warning.py` & `staffology-0.1.5/staffology/models/rti_validation_warning.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/smtp_settings.py` & `staffology-0.1.5/staffology/models/smtp_settings.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/starter_details.py` & `staffology-0.1.5/staffology/models/starter_details.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/statutory_pay.py` & `staffology-0.1.5/staffology/models/statutory_pay.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/statutory_pay_report.py` & `staffology-0.1.5/staffology/models/statutory_pay_report.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/statutory_pay_report_line.py` & `staffology-0.1.5/staffology/models/statutory_pay_report_line.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/statutory_pay_report_report_response.py` & `staffology-0.1.5/staffology/models/statutory_pay_report_report_response.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/string_string_key_value_pair.py` & `staffology-0.1.5/staffology/models/string_string_key_value_pair.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/student_loan_recovered.py` & `staffology-0.1.5/staffology/models/student_loan_recovered.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/submission_status.py` & `staffology-0.1.5/staffology/models/submission_status.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/tag.py` & `staffology-0.1.5/staffology/models/tag.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/tax_and_ni.py` & `staffology-0.1.5/staffology/models/tax_and_ni.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/tax_bracket.py` & `staffology-0.1.5/staffology/models/tax_bracket.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/tax_code_change.py` & `staffology-0.1.5/staffology/models/tax_code_change.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/tax_code_change_report.py` & `staffology-0.1.5/staffology/models/tax_code_change_report.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/tax_code_change_report_report_response.py` & `staffology-0.1.5/staffology/models/tax_code_change_report_report_response.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/tax_code_change_values.py` & `staffology-0.1.5/staffology/models/tax_code_change_values.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/teachers_pension_details.py` & `staffology-0.1.5/staffology/models/teachers_pension_details.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/tenant.py` & `staffology-0.1.5/staffology/models/tenant.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/tenant_billing_settings.py` & `staffology-0.1.5/staffology/models/tenant_billing_settings.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/tenant_email.py` & `staffology-0.1.5/staffology/models/tenant_email.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/tenant_html_insertion.py` & `staffology-0.1.5/staffology/models/tenant_html_insertion.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/tenant_item.py` & `staffology-0.1.5/staffology/models/tenant_item.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/tiered_pension.py` & `staffology-0.1.5/staffology/models/tiered_pension.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/tiered_pension_rate.py` & `staffology-0.1.5/staffology/models/tiered_pension_rate.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/umbrella_payment.py` & `staffology-0.1.5/staffology/models/umbrella_payment.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/umbrella_reconciliation_report.py` & `staffology-0.1.5/staffology/models/umbrella_reconciliation_report.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/umbrella_reconciliation_report_line.py` & `staffology-0.1.5/staffology/models/umbrella_reconciliation_report_line.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/umbrella_reconciliation_report_report_response.py` & `staffology-0.1.5/staffology/models/umbrella_reconciliation_report_report_response.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/umbrella_settings.py` & `staffology-0.1.5/staffology/models/umbrella_settings.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/update_fav_icon_tenant_multipart_data.py` & `staffology-0.1.5/staffology/models/update_fav_icon_tenant_multipart_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/update_logo_employer_multipart_data.py` & `staffology-0.1.5/staffology/models/update_logo_employer_multipart_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/update_logo_tenant_multipart_data.py` & `staffology-0.1.5/staffology/models/update_logo_tenant_multipart_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/update_photo_account_multipart_data.py` & `staffology-0.1.5/staffology/models/update_photo_account_multipart_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/update_photo_employee_multipart_data.py` & `staffology-0.1.5/staffology/models/update_photo_employee_multipart_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/usage_bill.py` & `staffology-0.1.5/staffology/models/usage_bill.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/user.py` & `staffology-0.1.5/staffology/models/user.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/user_authorization.py` & `staffology-0.1.5/staffology/models/user_authorization.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/user_display_preferences.py` & `staffology-0.1.5/staffology/models/user_display_preferences.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/user_industry.py` & `staffology-0.1.5/staffology/models/user_industry.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/user_job_type.py` & `staffology-0.1.5/staffology/models/user_job_type.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/utm_info.py` & `staffology-0.1.5/staffology/models/utm_info.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/value_override.py` & `staffology-0.1.5/staffology/models/value_override.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/variance_report.py` & `staffology-0.1.5/staffology/models/variance_report.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/variance_report_report_response.py` & `staffology-0.1.5/staffology/models/variance_report_report_response.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/veteran_details.py` & `staffology-0.1.5/staffology/models/veteran_details.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/webhook.py` & `staffology-0.1.5/staffology/models/webhook.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/webhook_payload.py` & `staffology-0.1.5/staffology/models/webhook_payload.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/worker_group.py` & `staffology-0.1.5/staffology/models/worker_group.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/working_pattern.py` & `staffology-0.1.5/staffology/models/working_pattern.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/year_end.py` & `staffology-0.1.5/staffology/models/year_end.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/year_end_tax_code_change.py` & `staffology-0.1.5/staffology/models/year_end_tax_code_change.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/ytd_pay_run_multipart_data.py` & `staffology-0.1.5/staffology/models/ytd_pay_run_multipart_data.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/ytd_report.py` & `staffology-0.1.5/staffology/models/ytd_report.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/ytd_report_report_response.py` & `staffology-0.1.5/staffology/models/ytd_report_report_response.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/models/ytd_value.py` & `staffology-0.1.5/staffology/models/ytd_value.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology/types.py` & `staffology-0.1.5/staffology/types.py`

 * *Files identical despite different names*

### Comparing `staffology-0.1.4/staffology.egg-info/PKG-INFO` & `staffology-0.1.5/staffology.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: staffology
-Version: 0.1.4
+Version: 0.1.5
 Summary: Staffology openapi client with authentication patch
 Home-page: https://github.com/ihorizonUK/staffology
 Author: isik-kaplan
 Author-email: isik@ihorizon.co.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.7
```

### Comparing `staffology-0.1.4/staffology.egg-info/SOURCES.txt` & `staffology-0.1.5/staffology.egg-info/SOURCES.txt`

 * *Files identical despite different names*

