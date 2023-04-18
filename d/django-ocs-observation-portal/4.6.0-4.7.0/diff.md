# Comparing `tmp/django_ocs_observation_portal-4.6.0.tar.gz` & `tmp/django_ocs_observation_portal-4.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_ocs_observation_portal-4.6.0.tar", max compression
+gzip compressed data, was "django_ocs_observation_portal-4.7.0.tar", max compression
```

## Comparing `django_ocs_observation_portal-4.6.0.tar` & `django_ocs_observation_portal-4.7.0.tar`

### file list

```diff
@@ -1,202 +1,204 @@
--rw-r--r--   0        0        0    35149 2023-04-10 19:41:27.990839 django_ocs_observation_portal-4.6.0/LICENSE
--rw-r--r--   0        0        0    39207 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/README.md
--rw-r--r--   0        0        0        0 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/__init__.py
--rw-r--r--   0        0        0     1187 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/admin.py
--rw-r--r--   0        0        0      224 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/apps.py
--rw-r--r--   0        0        0      651 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/backends.py
--rw-r--r--   0        0        0     2008 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/forms.py
--rw-r--r--   0        0        0        0 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/management/commands/__init__.py
--rw-r--r--   0        0        0     1970 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/management/commands/create_application.py
--rw-r--r--   0        0        0     2027 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/management/commands/create_user.py
--rw-r--r--   0        0        0      802 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/management/commands/generateschema_mocked.py
--rw-r--r--   0        0        0     2416 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/management/commands/init_e2e_credentials.py
--rw-r--r--   0        0        0     1403 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/management/commands/updateclientusers.py
--rw-r--r--   0        0        0     1276 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/migrations/0001_initial.py
--rw-r--r--   0        0        0      395 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/migrations/0002_profile_terms_accepted.py
--rw-r--r--   0        0        0      835 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/migrations/0003_bulk_create_users_api.py
--rw-r--r--   0        0        0        0 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/migrations/__init__.py
--rw-r--r--   0        0        0     3589 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/models.py
--rw-r--r--   0        0        0     5648 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/oauth2_migrations/0001_initial.py
--rw-r--r--   0        0        0     3266 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/oauth2_migrations/0002_auto_20210715_0630.py
--rw-r--r--   0        0        0     1714 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/oauth2_migrations/0003_alter_accesstoken_user_alter_application_user_and_more.py
--rw-r--r--   0        0        0        0 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/oauth2_migrations/__init__.py
--rw-r--r--   0        0        0     1841 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/permissions.py
--rw-r--r--   0        0        0     9168 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/serializers.py
--rw-r--r--   0        0        0        0 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/signals/__init__.py
--rw-r--r--   0        0        0     1272 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/signals/handlers.py
--rw-r--r--   0        0        0     2065 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/tasks.py
--rw-r--r--   0        0        0      197 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/templates/auth/logged_in_state.html
--rw-r--r--   0        0        0      170 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/templates/base.html
--rw-r--r--   0        0        0      330 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/templates/bulkapi-account-created-email.txt
--rw-r--r--   0        0        0      638 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/templates/redoc.html
--rw-r--r--   0        0        0      589 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/templates/registration/activation_complete.html
--rw-r--r--   0        0        0     2131 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/templates/registration/activation_email.html
--rwxr-xr-x   0        0        0      483 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/templates/registration/login.html
--rw-r--r--   0        0        0      327 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/templates/registration/registration_form.html
--rw-r--r--   0        0        0      974 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/test_utils.py
--rw-r--r--   0        0        0     9376 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/test_views.py
--rw-r--r--   0        0        0    28161 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/tests.py
--rw-r--r--   0        0        0      281 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/throttling.py
--rw-r--r--   0        0        0      964 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/urls.py
--rw-r--r--   0        0        0     6522 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/views.py
--rw-r--r--   0        0        0       23 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/common/__init__.py
--rw-r--r--   0        0        0    35076 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/common/configdb.py
--rw-r--r--   0        0        0    26068 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/common/doc_examples.py
--rw-r--r--   0        0        0     3622 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/common/downtimedb.py
--rw-r--r--   0        0        0     1283 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/common/middleware.py
--rw-r--r--   0        0        0     2984 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/common/mixins.py
--rw-r--r--   0        0        0    15015 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/common/rise_set_utils.py
--rw-r--r--   0        0        0     8137 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/common/schema.py
--rw-r--r--   0        0        0    17629 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/common/state_changes.py
--rw-r--r--   0        0        0    14532 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/common/telescope_states.py
--rw-r--r--   0        0        0     2012 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/common/test_configdb.py
--rw-r--r--   0        0        0        0 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/common/test_data/__init__.py
--rw-r--r--   0        0        0   106356 2023-04-10 19:41:27.998840 django_ocs_observation_portal-4.6.0/observation_portal/common/test_data/configdb.json
--rw-r--r--   0        0        0    14960 2023-04-10 19:41:27.998840 django_ocs_observation_portal-4.6.0/observation_portal/common/test_data/doc_configdb.json
--rw-r--r--   0        0        0 10749196 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/common/test_data/es_telescope_states_data.txt
--rw-r--r--   0        0        0     4932 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/common/test_helpers.py
--rw-r--r--   0        0        0    54539 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/common/test_state_changes.py
--rw-r--r--   0        0        0    27685 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/common/test_telescope_states.py
--rw-r--r--   0        0        0     1773 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/common/utils.py
--rw-r--r--   0        0        0        0 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/observations/__init__.py
--rw-r--r--   0        0        0     2470 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/observations/admin.py
--rw-r--r--   0        0        0      236 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/observations/apps.py
--rw-r--r--   0        0        0     4596 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/observations/filters.py
--rw-r--r--   0        0        0      614 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/observations/forms.py
--rw-r--r--   0        0        0        0 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/observations/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/observations/management/commands/__init__.py
--rw-r--r--   0        0        0     1661 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/observations/management/commands/populate_time_charged.py
--rw-r--r--   0        0        0     6658 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/observations/management/commands/time_accounting.py
--rw-r--r--   0        0        0     5063 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/observations/migrations/0001_initial.py
--rw-r--r--   0        0        0      399 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/observations/migrations/0002_auto_20190408_1908.py
--rw-r--r--   0        0        0      550 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/observations/migrations/0003_auto_20190514_0005.py
--rw-r--r--   0        0        0      473 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/observations/migrations/0004_observation_priority.py
--rw-r--r--   0        0        0     1069 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/observations/migrations/0005_auto_20210116_0033.py
--rw-r--r--   0        0        0      484 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/observations/migrations/0006_alter_summary_events.py
--rw-r--r--   0        0        0      358 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/observations/migrations/0007_alter_configurationstatus_unique_together.py
--rw-r--r--   0        0        0      542 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/observations/migrations/0008_configurationstatus_time_charged.py
--rw-r--r--   0        0        0        0 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/observations/migrations/__init__.py
--rw-r--r--   0        0        0    13134 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/observations/models.py
--rw-r--r--   0        0        0    21866 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/observations/serializers.py
--rw-r--r--   0        0        0        0 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/observations/signals/__init__.py
--rw-r--r--   0        0        0      981 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/observations/signals/handlers.py
--rw-r--r--   0        0        0      443 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/observations/tasks.py
--rw-r--r--   0        0        0      425 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/observations/templates/observations/observation_changeform.html
--rw-r--r--   0        0        0        0 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/observations/test/__init__.py
--rw-r--r--   0        0        0   128718 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/observations/test/tests.py
--rw-r--r--   0        0        0     5676 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/observations/time_accounting.py
--rw-r--r--   0        0        0     2260 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/observations/views.py
--rw-r--r--   0        0        0    11820 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/observations/viewsets.py
--rw-r--r--   0        0        0        0 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/__init__.py
--rw-r--r--   0        0        0     4401 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/admin.py
--rw-r--r--   0        0        0      227 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/apps.py
--rw-r--r--   0        0        0     2867 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/filters.py
--rw-r--r--   0        0        0     4731 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/forms.py
--rw-r--r--   0        0        0        0 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/management/commands/__init__.py
--rw-r--r--   0        0        0     4286 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/management/commands/create_proposal.py
--rw-r--r--   0        0        0     1445 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/management/commands/create_semester.py
--rw-r--r--   0        0        0     6532 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/migrations/0001_initial.py
--rw-r--r--   0        0        0     1172 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/migrations/0002_auto_20190815_1942.py
--rw-r--r--   0        0        0      461 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/migrations/0003_auto_20210203_0022.py
--rw-r--r--   0        0        0      690 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/migrations/0004_auto_20210617_0908.py
--rw-r--r--   0        0        0      733 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/migrations/0005_auto_20210604_2154.py
--rw-r--r--   0        0        0      631 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/migrations/0006_auto_20210604_2155.py
--rw-r--r--   0        0        0      595 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/migrations/0007_remove_timeallocation_instrument_type.py
--rw-r--r--   0        0        0      910 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/migrations/0008_auto_20210708_1623.py
--rw-r--r--   0        0        0        0 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/migrations/__init__.py
--rw-r--r--   0        0        0    13225 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/models.py
--rw-r--r--   0        0        0     2597 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/notifications.py
--rw-r--r--   0        0        0     2784 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/serializers.py
--rw-r--r--   0        0        0        0 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/signals/__init__.py
--rw-r--r--   0        0        0      654 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/signals/handlers.py
--rw-r--r--   0        0        0      726 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/tasks.py
--rw-r--r--   0        0        0      280 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/templates/proposals/added.txt
--rw-r--r--   0        0        0      309 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/templates/proposals/invitation.txt
--rw-r--r--   0        0        0      750 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/templates/proposals/requestfailurelimit.txt
--rw-r--r--   0        0        0      527 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/templates/proposals/requestgroupcomplete.txt
--rw-r--r--   0        0        0     1380 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/templates/proposals/timeallocationreminder.html
--rw-r--r--   0        0        0    45521 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/test_api.py
--rw-r--r--   0        0        0    18777 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/tests.py
--rw-r--r--   0        0        0    13908 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/viewsets.py
--rw-r--r--   0        0        0        0 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/__init__.py
--rw-r--r--   0        0        0     5060 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/admin.py
--rw-r--r--   0        0        0      239 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/apps.py
--rw-r--r--   0        0        0     2053 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/cadence.py
--rw-r--r--   0        0        0     8095 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/contention.py
--rw-r--r--   0        0        0    16127 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/duration_utils.py
--rw-r--r--   0        0        0     3126 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/filters.py
--rw-r--r--   0        0        0      766 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/forms.py
--rw-r--r--   0        0        0        0 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/management/commands/__init__.py
--rw-r--r--   0        0        0    14120 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/management/commands/create_example_requests.py
--rw-r--r--   0        0        0    25262 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0001_initial.py
--rw-r--r--   0        0        0     2533 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0002_auto_20190319_1814.py
--rw-r--r--   0        0        0      594 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0003_acquisitionconfig_exposure_time.py
--rw-r--r--   0        0        0      575 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0004_auto_20190410_0103.py
--rw-r--r--   0        0        0      385 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0005_auto_20190501_2103.py
--rw-r--r--   0        0        0      926 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0006_auto_20190514_0005.py
--rw-r--r--   0        0        0      922 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0007_auto_20190516_1713.py
--rw-r--r--   0        0        0      589 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0008_auto_20190516_2055.py
--rw-r--r--   0        0        0      977 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0009_auto_20190518_0023.py
--rw-r--r--   0        0        0     2180 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0010_auto_20190612_0048.py
--rw-r--r--   0        0        0      536 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0011_auto_20190702_2014.py
--rw-r--r--   0        0        0     1488 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0012_auto_20191123_0233.py
--rw-r--r--   0        0        0     1158 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0013_auto_20191220_0711.py
--rw-r--r--   0        0        0     1036 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0014_auto_20210123_0715.py
--rw-r--r--   0        0        0     1072 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0015_auto_20210323_0635.py
--rw-r--r--   0        0        0      456 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0016_auto_20210525_0643.py
--rw-r--r--   0        0        0      546 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0017_request_extra_params.py
--rw-r--r--   0        0        0     2512 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0018_alter_acquisitionconfig_extra_params_and_more.py
--rw-r--r--   0        0        0      731 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0019_request_configuration_repeats.py
--rw-r--r--   0        0        0      681 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0020_alter_constraints_max_lunar_phase.py
--rw-r--r--   0        0        0      586 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0021_request_optimization_type.py
--rw-r--r--   0        0        0      577 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0022_alter_constraints_max_seeing.py
--rw-r--r--   0        0        0      632 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0023_alter_target_epochofperih.py
--rw-r--r--   0        0        0        0 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/__init__.py
--rw-r--r--   0        0        0    36336 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/models.py
--rw-r--r--   0        0        0     8037 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/pattern_expansion.py
--rw-r--r--   0        0        0     7545 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/request_utils.py
--rw-r--r--   0        0        0    53248 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/serializers.py
--rw-r--r--   0        0        0       23 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/signals/__init__.py
--rw-r--r--   0        0        0     1538 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/signals/handlers.py
--rw-r--r--   0        0        0     4344 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/target_helpers.py
--rw-r--r--   0        0        0      296 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/tasks.py
--rw-r--r--   0        0        0        0 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/test/__init__.py
--rw-r--r--   0        0        0   595296 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/test/data/blocks.json
--rw-r--r--   0        0        0    37647 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/test/test.py
--rw-r--r--   0        0        0   188357 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/test/test_api.py
--rw-r--r--   0        0        0     3346 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/test/test_cadence.py
--rw-r--r--   0        0        0     2596 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/test/test_helpers.py
--rw-r--r--   0        0        0    42192 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/test/test_request_utils.py
--rw-r--r--   0        0        0     4295 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/test/test_views.py
--rw-r--r--   0        0        0    10712 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/views.py
--rw-r--r--   0        0        0    19248 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/viewsets.py
--rw-r--r--   0        0        0        0 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/__init__.py
--rw-r--r--   0        0        0     4712 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/admin.py
--rw-r--r--   0        0        0      124 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/apps.py
--rw-r--r--   0        0        0     1718 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/filters.py
--rw-r--r--   0        0        0     5775 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/migrations/0001_initial.py
--rw-r--r--   0        0        0      450 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/migrations/0002_timerequest_instrument_types.py
--rw-r--r--   0        0        0      620 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/migrations/0003_auto_20210604_2155.py
--rw-r--r--   0        0        0      346 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/migrations/0004_remove_timerequest_instrument.py
--rw-r--r--   0        0        0      728 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/migrations/0005_auto_20210708_1623.py
--rw-r--r--   0        0        0        0 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/migrations/__init__.py
--rw-r--r--   0        0        0    10686 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/models.py
--rw-r--r--   0        0        0    13642 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/serializers.py
--rw-r--r--   0        0        0      375 2023-04-10 19:41:28.038843 django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/templates/sciapplications/approved.txt
--rw-r--r--   0        0        0      318 2023-04-10 19:41:28.038843 django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/templates/sciapplications/ddt_submitted.txt
--rw-r--r--   0        0        0    11505 2023-04-10 19:41:28.038843 django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/test_admin.py
--rw-r--r--   0        0        0    54563 2023-04-10 19:41:28.038843 django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/test_api.py
--rw-r--r--   0        0        0     7046 2023-04-10 19:41:28.038843 django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/tests.py
--rw-r--r--   0        0        0     6480 2023-04-10 19:41:28.038843 django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/viewsets.py
--rw-r--r--   0        0        0    23236 2023-04-10 19:41:28.038843 django_ocs_observation_portal-4.6.0/observation_portal/settings.py
--rw-r--r--   0        0        0      920 2023-04-10 19:41:28.038843 django_ocs_observation_portal-4.6.0/observation_portal/task_scheduler.py
--rw-r--r--   0        0        0      601 2023-04-10 19:41:28.038843 django_ocs_observation_portal-4.6.0/observation_portal/test_runner.py
--rw-r--r--   0        0        0     1776 2023-04-10 19:41:28.038843 django_ocs_observation_portal-4.6.0/observation_portal/test_settings.py
--rw-r--r--   0        0        0     5507 2023-04-10 19:41:28.038843 django_ocs_observation_portal-4.6.0/observation_portal/urls.py
--rw-r--r--   0        0        0      413 2023-04-10 19:41:28.038843 django_ocs_observation_portal-4.6.0/observation_portal/wsgi.py
--rw-r--r--   0        0        0     2043 2023-04-10 19:41:28.038843 django_ocs_observation_portal-4.6.0/pyproject.toml
--rw-r--r--   0        0        0    41514 1970-01-01 00:00:00.000000 django_ocs_observation_portal-4.6.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-18 23:52:27.669418 django_ocs_observation_portal-4.7.0/LICENSE
+-rw-r--r--   0        0        0    39207 2023-04-18 23:52:27.669418 django_ocs_observation_portal-4.7.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-18 23:52:27.669418 django_ocs_observation_portal-4.7.0/observation_portal/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 23:52:27.669418 django_ocs_observation_portal-4.7.0/observation_portal/accounts/__init__.py
+-rw-r--r--   0        0        0     1187 2023-04-18 23:52:27.669418 django_ocs_observation_portal-4.7.0/observation_portal/accounts/admin.py
+-rw-r--r--   0        0        0      224 2023-04-18 23:52:27.669418 django_ocs_observation_portal-4.7.0/observation_portal/accounts/apps.py
+-rw-r--r--   0        0        0      651 2023-04-18 23:52:27.669418 django_ocs_observation_portal-4.7.0/observation_portal/accounts/backends.py
+-rw-r--r--   0        0        0     2008 2023-04-18 23:52:27.669418 django_ocs_observation_portal-4.7.0/observation_portal/accounts/forms.py
+-rw-r--r--   0        0        0        0 2023-04-18 23:52:27.669418 django_ocs_observation_portal-4.7.0/observation_portal/accounts/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 23:52:27.669418 django_ocs_observation_portal-4.7.0/observation_portal/accounts/management/commands/__init__.py
+-rw-r--r--   0        0        0     1970 2023-04-18 23:52:27.669418 django_ocs_observation_portal-4.7.0/observation_portal/accounts/management/commands/create_application.py
+-rw-r--r--   0        0        0     2027 2023-04-18 23:52:27.669418 django_ocs_observation_portal-4.7.0/observation_portal/accounts/management/commands/create_user.py
+-rw-r--r--   0        0        0      802 2023-04-18 23:52:27.669418 django_ocs_observation_portal-4.7.0/observation_portal/accounts/management/commands/generateschema_mocked.py
+-rw-r--r--   0        0        0     2416 2023-04-18 23:52:27.669418 django_ocs_observation_portal-4.7.0/observation_portal/accounts/management/commands/init_e2e_credentials.py
+-rw-r--r--   0        0        0     1403 2023-04-18 23:52:27.669418 django_ocs_observation_portal-4.7.0/observation_portal/accounts/management/commands/updateclientusers.py
+-rw-r--r--   0        0        0     1276 2023-04-18 23:52:27.669418 django_ocs_observation_portal-4.7.0/observation_portal/accounts/migrations/0001_initial.py
+-rw-r--r--   0        0        0      395 2023-04-18 23:52:27.669418 django_ocs_observation_portal-4.7.0/observation_portal/accounts/migrations/0002_profile_terms_accepted.py
+-rw-r--r--   0        0        0      835 2023-04-18 23:52:27.669418 django_ocs_observation_portal-4.7.0/observation_portal/accounts/migrations/0003_bulk_create_users_api.py
+-rw-r--r--   0        0        0        0 2023-04-18 23:52:27.669418 django_ocs_observation_portal-4.7.0/observation_portal/accounts/migrations/__init__.py
+-rw-r--r--   0        0        0     3589 2023-04-18 23:52:27.669418 django_ocs_observation_portal-4.7.0/observation_portal/accounts/models.py
+-rw-r--r--   0        0        0     5648 2023-04-18 23:52:27.669418 django_ocs_observation_portal-4.7.0/observation_portal/accounts/oauth2_migrations/0001_initial.py
+-rw-r--r--   0        0        0     3266 2023-04-18 23:52:27.669418 django_ocs_observation_portal-4.7.0/observation_portal/accounts/oauth2_migrations/0002_auto_20210715_0630.py
+-rw-r--r--   0        0        0     1714 2023-04-18 23:52:27.669418 django_ocs_observation_portal-4.7.0/observation_portal/accounts/oauth2_migrations/0003_alter_accesstoken_user_alter_application_user_and_more.py
+-rw-r--r--   0        0        0        0 2023-04-18 23:52:27.669418 django_ocs_observation_portal-4.7.0/observation_portal/accounts/oauth2_migrations/__init__.py
+-rw-r--r--   0        0        0     1841 2023-04-18 23:52:27.669418 django_ocs_observation_portal-4.7.0/observation_portal/accounts/permissions.py
+-rw-r--r--   0        0        0     9168 2023-04-18 23:52:27.669418 django_ocs_observation_portal-4.7.0/observation_portal/accounts/serializers.py
+-rw-r--r--   0        0        0        0 2023-04-18 23:52:27.669418 django_ocs_observation_portal-4.7.0/observation_portal/accounts/signals/__init__.py
+-rw-r--r--   0        0        0     1272 2023-04-18 23:52:27.669418 django_ocs_observation_portal-4.7.0/observation_portal/accounts/signals/handlers.py
+-rw-r--r--   0        0        0     2065 2023-04-18 23:52:27.669418 django_ocs_observation_portal-4.7.0/observation_portal/accounts/tasks.py
+-rw-r--r--   0        0        0      197 2023-04-18 23:52:27.669418 django_ocs_observation_portal-4.7.0/observation_portal/accounts/templates/auth/logged_in_state.html
+-rw-r--r--   0        0        0      170 2023-04-18 23:52:27.669418 django_ocs_observation_portal-4.7.0/observation_portal/accounts/templates/base.html
+-rw-r--r--   0        0        0      330 2023-04-18 23:52:27.669418 django_ocs_observation_portal-4.7.0/observation_portal/accounts/templates/bulkapi-account-created-email.txt
+-rw-r--r--   0        0        0      638 2023-04-18 23:52:27.669418 django_ocs_observation_portal-4.7.0/observation_portal/accounts/templates/redoc.html
+-rw-r--r--   0        0        0      589 2023-04-18 23:52:27.673418 django_ocs_observation_portal-4.7.0/observation_portal/accounts/templates/registration/activation_complete.html
+-rw-r--r--   0        0        0     2131 2023-04-18 23:52:27.673418 django_ocs_observation_portal-4.7.0/observation_portal/accounts/templates/registration/activation_email.html
+-rwxr-xr-x   0        0        0      483 2023-04-18 23:52:27.673418 django_ocs_observation_portal-4.7.0/observation_portal/accounts/templates/registration/login.html
+-rw-r--r--   0        0        0      327 2023-04-18 23:52:27.673418 django_ocs_observation_portal-4.7.0/observation_portal/accounts/templates/registration/registration_form.html
+-rw-r--r--   0        0        0      974 2023-04-18 23:52:27.673418 django_ocs_observation_portal-4.7.0/observation_portal/accounts/test_utils.py
+-rw-r--r--   0        0        0     9376 2023-04-18 23:52:27.673418 django_ocs_observation_portal-4.7.0/observation_portal/accounts/test_views.py
+-rw-r--r--   0        0        0    28161 2023-04-18 23:52:27.673418 django_ocs_observation_portal-4.7.0/observation_portal/accounts/tests.py
+-rw-r--r--   0        0        0      281 2023-04-18 23:52:27.673418 django_ocs_observation_portal-4.7.0/observation_portal/accounts/throttling.py
+-rw-r--r--   0        0        0      964 2023-04-18 23:52:27.673418 django_ocs_observation_portal-4.7.0/observation_portal/accounts/urls.py
+-rw-r--r--   0        0        0     6522 2023-04-18 23:52:27.673418 django_ocs_observation_portal-4.7.0/observation_portal/accounts/views.py
+-rw-r--r--   0        0        0       23 2023-04-18 23:52:27.673418 django_ocs_observation_portal-4.7.0/observation_portal/common/__init__.py
+-rw-r--r--   0        0        0    35228 2023-04-18 23:52:27.673418 django_ocs_observation_portal-4.7.0/observation_portal/common/configdb.py
+-rw-r--r--   0        0        0    26068 2023-04-18 23:52:27.673418 django_ocs_observation_portal-4.7.0/observation_portal/common/doc_examples.py
+-rw-r--r--   0        0        0     3622 2023-04-18 23:52:27.673418 django_ocs_observation_portal-4.7.0/observation_portal/common/downtimedb.py
+-rw-r--r--   0        0        0     1283 2023-04-18 23:52:27.673418 django_ocs_observation_portal-4.7.0/observation_portal/common/middleware.py
+-rw-r--r--   0        0        0     2984 2023-04-18 23:52:27.673418 django_ocs_observation_portal-4.7.0/observation_portal/common/mixins.py
+-rw-r--r--   0        0        0    15015 2023-04-18 23:52:27.673418 django_ocs_observation_portal-4.7.0/observation_portal/common/rise_set_utils.py
+-rw-r--r--   0        0        0     8137 2023-04-18 23:52:27.673418 django_ocs_observation_portal-4.7.0/observation_portal/common/schema.py
+-rw-r--r--   0        0        0    17629 2023-04-18 23:52:27.673418 django_ocs_observation_portal-4.7.0/observation_portal/common/state_changes.py
+-rw-r--r--   0        0        0    14532 2023-04-18 23:52:27.673418 django_ocs_observation_portal-4.7.0/observation_portal/common/telescope_states.py
+-rw-r--r--   0        0        0     2012 2023-04-18 23:52:27.673418 django_ocs_observation_portal-4.7.0/observation_portal/common/test_configdb.py
+-rw-r--r--   0        0        0        0 2023-04-18 23:52:27.673418 django_ocs_observation_portal-4.7.0/observation_portal/common/test_data/__init__.py
+-rw-r--r--   0        0        0   106356 2023-04-18 23:52:27.673418 django_ocs_observation_portal-4.7.0/observation_portal/common/test_data/configdb.json
+-rw-r--r--   0        0        0    14960 2023-04-18 23:52:27.673418 django_ocs_observation_portal-4.7.0/observation_portal/common/test_data/doc_configdb.json
+-rw-r--r--   0        0        0 10749196 2023-04-18 23:52:27.697419 django_ocs_observation_portal-4.7.0/observation_portal/common/test_data/es_telescope_states_data.txt
+-rw-r--r--   0        0        0     4932 2023-04-18 23:52:27.697419 django_ocs_observation_portal-4.7.0/observation_portal/common/test_helpers.py
+-rw-r--r--   0        0        0    54539 2023-04-18 23:52:27.697419 django_ocs_observation_portal-4.7.0/observation_portal/common/test_state_changes.py
+-rw-r--r--   0        0        0    27685 2023-04-18 23:52:27.697419 django_ocs_observation_portal-4.7.0/observation_portal/common/test_telescope_states.py
+-rw-r--r--   0        0        0     1773 2023-04-18 23:52:27.697419 django_ocs_observation_portal-4.7.0/observation_portal/common/utils.py
+-rw-r--r--   0        0        0        0 2023-04-18 23:52:27.697419 django_ocs_observation_portal-4.7.0/observation_portal/observations/__init__.py
+-rw-r--r--   0        0        0     2470 2023-04-18 23:52:27.697419 django_ocs_observation_portal-4.7.0/observation_portal/observations/admin.py
+-rw-r--r--   0        0        0      236 2023-04-18 23:52:27.697419 django_ocs_observation_portal-4.7.0/observation_portal/observations/apps.py
+-rw-r--r--   0        0        0     4596 2023-04-18 23:52:27.697419 django_ocs_observation_portal-4.7.0/observation_portal/observations/filters.py
+-rw-r--r--   0        0        0      614 2023-04-18 23:52:27.697419 django_ocs_observation_portal-4.7.0/observation_portal/observations/forms.py
+-rw-r--r--   0        0        0        0 2023-04-18 23:52:27.697419 django_ocs_observation_portal-4.7.0/observation_portal/observations/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 23:52:27.697419 django_ocs_observation_portal-4.7.0/observation_portal/observations/management/commands/__init__.py
+-rw-r--r--   0        0        0     1661 2023-04-18 23:52:27.697419 django_ocs_observation_portal-4.7.0/observation_portal/observations/management/commands/populate_time_charged.py
+-rw-r--r--   0        0        0     6658 2023-04-18 23:52:27.697419 django_ocs_observation_portal-4.7.0/observation_portal/observations/management/commands/time_accounting.py
+-rw-r--r--   0        0        0     5063 2023-04-18 23:52:27.697419 django_ocs_observation_portal-4.7.0/observation_portal/observations/migrations/0001_initial.py
+-rw-r--r--   0        0        0      399 2023-04-18 23:52:27.697419 django_ocs_observation_portal-4.7.0/observation_portal/observations/migrations/0002_auto_20190408_1908.py
+-rw-r--r--   0        0        0      550 2023-04-18 23:52:27.697419 django_ocs_observation_portal-4.7.0/observation_portal/observations/migrations/0003_auto_20190514_0005.py
+-rw-r--r--   0        0        0      473 2023-04-18 23:52:27.697419 django_ocs_observation_portal-4.7.0/observation_portal/observations/migrations/0004_observation_priority.py
+-rw-r--r--   0        0        0     1069 2023-04-18 23:52:27.697419 django_ocs_observation_portal-4.7.0/observation_portal/observations/migrations/0005_auto_20210116_0033.py
+-rw-r--r--   0        0        0      484 2023-04-18 23:52:27.697419 django_ocs_observation_portal-4.7.0/observation_portal/observations/migrations/0006_alter_summary_events.py
+-rw-r--r--   0        0        0      358 2023-04-18 23:52:27.697419 django_ocs_observation_portal-4.7.0/observation_portal/observations/migrations/0007_alter_configurationstatus_unique_together.py
+-rw-r--r--   0        0        0      542 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/observations/migrations/0008_configurationstatus_time_charged.py
+-rw-r--r--   0        0        0        0 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/observations/migrations/__init__.py
+-rw-r--r--   0        0        0    13134 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/observations/models.py
+-rw-r--r--   0        0        0    21866 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/observations/serializers.py
+-rw-r--r--   0        0        0        0 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/observations/signals/__init__.py
+-rw-r--r--   0        0        0      981 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/observations/signals/handlers.py
+-rw-r--r--   0        0        0      443 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/observations/tasks.py
+-rw-r--r--   0        0        0      425 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/observations/templates/observations/observation_changeform.html
+-rw-r--r--   0        0        0        0 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/observations/test/__init__.py
+-rw-r--r--   0        0        0   128718 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/observations/test/tests.py
+-rw-r--r--   0        0        0     5676 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/observations/time_accounting.py
+-rw-r--r--   0        0        0     2260 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/observations/views.py
+-rw-r--r--   0        0        0    11820 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/observations/viewsets.py
+-rw-r--r--   0        0        0        0 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/proposals/__init__.py
+-rw-r--r--   0        0        0     4401 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/proposals/admin.py
+-rw-r--r--   0        0        0      227 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/proposals/apps.py
+-rw-r--r--   0        0        0     2867 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/proposals/filters.py
+-rw-r--r--   0        0        0     4760 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/proposals/forms.py
+-rw-r--r--   0        0        0        0 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/proposals/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/proposals/management/commands/__init__.py
+-rw-r--r--   0        0        0     4286 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/proposals/management/commands/create_proposal.py
+-rw-r--r--   0        0        0     1445 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/proposals/management/commands/create_semester.py
+-rw-r--r--   0        0        0     6532 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/proposals/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1172 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/proposals/migrations/0002_auto_20190815_1942.py
+-rw-r--r--   0        0        0      461 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/proposals/migrations/0003_auto_20210203_0022.py
+-rw-r--r--   0        0        0      690 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/proposals/migrations/0004_auto_20210617_0908.py
+-rw-r--r--   0        0        0      733 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/proposals/migrations/0005_auto_20210604_2154.py
+-rw-r--r--   0        0        0      631 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/proposals/migrations/0006_auto_20210604_2155.py
+-rw-r--r--   0        0        0      595 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/proposals/migrations/0007_remove_timeallocation_instrument_type.py
+-rw-r--r--   0        0        0      910 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/proposals/migrations/0008_auto_20210708_1623.py
+-rw-r--r--   0        0        0      357 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/proposals/migrations/0009_alter_semester_options.py
+-rw-r--r--   0        0        0        0 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/proposals/migrations/__init__.py
+-rw-r--r--   0        0        0    13278 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/proposals/models.py
+-rw-r--r--   0        0        0     2597 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/proposals/notifications.py
+-rw-r--r--   0        0        0     2784 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/proposals/serializers.py
+-rw-r--r--   0        0        0        0 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/proposals/signals/__init__.py
+-rw-r--r--   0        0        0      654 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/proposals/signals/handlers.py
+-rw-r--r--   0        0        0      726 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/proposals/tasks.py
+-rw-r--r--   0        0        0      280 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/proposals/templates/proposals/added.txt
+-rw-r--r--   0        0        0      309 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/proposals/templates/proposals/invitation.txt
+-rw-r--r--   0        0        0      750 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/proposals/templates/proposals/requestfailurelimit.txt
+-rw-r--r--   0        0        0      527 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/proposals/templates/proposals/requestgroupcomplete.txt
+-rw-r--r--   0        0        0     1380 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/proposals/templates/proposals/timeallocationreminder.html
+-rw-r--r--   0        0        0    45521 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/proposals/test_api.py
+-rw-r--r--   0        0        0    18777 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/proposals/tests.py
+-rw-r--r--   0        0        0    13908 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/proposals/viewsets.py
+-rw-r--r--   0        0        0        0 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/__init__.py
+-rw-r--r--   0        0        0     5060 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/admin.py
+-rw-r--r--   0        0        0      239 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/apps.py
+-rw-r--r--   0        0        0     2053 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/cadence.py
+-rw-r--r--   0        0        0     8095 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/contention.py
+-rw-r--r--   0        0        0    16127 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/duration_utils.py
+-rw-r--r--   0        0        0     3126 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/filters.py
+-rw-r--r--   0        0        0      766 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/forms.py
+-rw-r--r--   0        0        0        0 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/management/commands/__init__.py
+-rw-r--r--   0        0        0    14120 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/management/commands/create_example_requests.py
+-rw-r--r--   0        0        0    25262 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2533 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0002_auto_20190319_1814.py
+-rw-r--r--   0        0        0      594 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0003_acquisitionconfig_exposure_time.py
+-rw-r--r--   0        0        0      575 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0004_auto_20190410_0103.py
+-rw-r--r--   0        0        0      385 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0005_auto_20190501_2103.py
+-rw-r--r--   0        0        0      926 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0006_auto_20190514_0005.py
+-rw-r--r--   0        0        0      922 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0007_auto_20190516_1713.py
+-rw-r--r--   0        0        0      589 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0008_auto_20190516_2055.py
+-rw-r--r--   0        0        0      977 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0009_auto_20190518_0023.py
+-rw-r--r--   0        0        0     2180 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0010_auto_20190612_0048.py
+-rw-r--r--   0        0        0      536 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0011_auto_20190702_2014.py
+-rw-r--r--   0        0        0     1488 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0012_auto_20191123_0233.py
+-rw-r--r--   0        0        0     1158 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0013_auto_20191220_0711.py
+-rw-r--r--   0        0        0     1036 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0014_auto_20210123_0715.py
+-rw-r--r--   0        0        0     1072 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0015_auto_20210323_0635.py
+-rw-r--r--   0        0        0      456 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0016_auto_20210525_0643.py
+-rw-r--r--   0        0        0      546 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0017_request_extra_params.py
+-rw-r--r--   0        0        0     2512 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0018_alter_acquisitionconfig_extra_params_and_more.py
+-rw-r--r--   0        0        0      731 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0019_request_configuration_repeats.py
+-rw-r--r--   0        0        0      681 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0020_alter_constraints_max_lunar_phase.py
+-rw-r--r--   0        0        0      586 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0021_request_optimization_type.py
+-rw-r--r--   0        0        0      577 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0022_alter_constraints_max_seeing.py
+-rw-r--r--   0        0        0      632 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0023_alter_target_epochofperih.py
+-rw-r--r--   0        0        0        0 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/__init__.py
+-rw-r--r--   0        0        0    36336 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/models.py
+-rw-r--r--   0        0        0     8037 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/pattern_expansion.py
+-rw-r--r--   0        0        0     7545 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/request_utils.py
+-rw-r--r--   0        0        0    53248 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/serializers.py
+-rw-r--r--   0        0        0       23 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/signals/__init__.py
+-rw-r--r--   0        0        0     1538 2023-04-18 23:52:27.701418 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/signals/handlers.py
+-rw-r--r--   0        0        0     4344 2023-04-18 23:52:27.705419 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/target_helpers.py
+-rw-r--r--   0        0        0      296 2023-04-18 23:52:27.705419 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/tasks.py
+-rw-r--r--   0        0        0        0 2023-04-18 23:52:27.705419 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/test/__init__.py
+-rw-r--r--   0        0        0   595296 2023-04-18 23:52:27.705419 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/test/data/blocks.json
+-rw-r--r--   0        0        0    37647 2023-04-18 23:52:27.705419 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/test/test.py
+-rw-r--r--   0        0        0   188357 2023-04-18 23:52:27.705419 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/test/test_api.py
+-rw-r--r--   0        0        0     3346 2023-04-18 23:52:27.705419 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/test/test_cadence.py
+-rw-r--r--   0        0        0     2596 2023-04-18 23:52:27.705419 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/test/test_helpers.py
+-rw-r--r--   0        0        0    42192 2023-04-18 23:52:27.705419 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/test/test_request_utils.py
+-rw-r--r--   0        0        0     4295 2023-04-18 23:52:27.705419 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/test/test_views.py
+-rw-r--r--   0        0        0    10712 2023-04-18 23:52:27.705419 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/views.py
+-rw-r--r--   0        0        0    19248 2023-04-18 23:52:27.705419 django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/viewsets.py
+-rw-r--r--   0        0        0        0 2023-04-18 23:52:27.705419 django_ocs_observation_portal-4.7.0/observation_portal/sciapplications/__init__.py
+-rw-r--r--   0        0        0     4712 2023-04-18 23:52:27.705419 django_ocs_observation_portal-4.7.0/observation_portal/sciapplications/admin.py
+-rw-r--r--   0        0        0      124 2023-04-18 23:52:27.705419 django_ocs_observation_portal-4.7.0/observation_portal/sciapplications/apps.py
+-rw-r--r--   0        0        0     1718 2023-04-18 23:52:27.705419 django_ocs_observation_portal-4.7.0/observation_portal/sciapplications/filters.py
+-rw-r--r--   0        0        0     5775 2023-04-18 23:52:27.705419 django_ocs_observation_portal-4.7.0/observation_portal/sciapplications/migrations/0001_initial.py
+-rw-r--r--   0        0        0      450 2023-04-18 23:52:27.705419 django_ocs_observation_portal-4.7.0/observation_portal/sciapplications/migrations/0002_timerequest_instrument_types.py
+-rw-r--r--   0        0        0      620 2023-04-18 23:52:27.705419 django_ocs_observation_portal-4.7.0/observation_portal/sciapplications/migrations/0003_auto_20210604_2155.py
+-rw-r--r--   0        0        0      346 2023-04-18 23:52:27.705419 django_ocs_observation_portal-4.7.0/observation_portal/sciapplications/migrations/0004_remove_timerequest_instrument.py
+-rw-r--r--   0        0        0      728 2023-04-18 23:52:27.705419 django_ocs_observation_portal-4.7.0/observation_portal/sciapplications/migrations/0005_auto_20210708_1623.py
+-rw-r--r--   0        0        0      357 2023-04-18 23:52:27.705419 django_ocs_observation_portal-4.7.0/observation_portal/sciapplications/migrations/0006_alter_instrument_options.py
+-rw-r--r--   0        0        0        0 2023-04-18 23:52:27.705419 django_ocs_observation_portal-4.7.0/observation_portal/sciapplications/migrations/__init__.py
+-rw-r--r--   0        0        0    10731 2023-04-18 23:52:27.705419 django_ocs_observation_portal-4.7.0/observation_portal/sciapplications/models.py
+-rw-r--r--   0        0        0    13642 2023-04-18 23:52:27.705419 django_ocs_observation_portal-4.7.0/observation_portal/sciapplications/serializers.py
+-rw-r--r--   0        0        0      375 2023-04-18 23:52:27.705419 django_ocs_observation_portal-4.7.0/observation_portal/sciapplications/templates/sciapplications/approved.txt
+-rw-r--r--   0        0        0      318 2023-04-18 23:52:27.705419 django_ocs_observation_portal-4.7.0/observation_portal/sciapplications/templates/sciapplications/ddt_submitted.txt
+-rw-r--r--   0        0        0    11505 2023-04-18 23:52:27.705419 django_ocs_observation_portal-4.7.0/observation_portal/sciapplications/test_admin.py
+-rw-r--r--   0        0        0    54563 2023-04-18 23:52:27.705419 django_ocs_observation_portal-4.7.0/observation_portal/sciapplications/test_api.py
+-rw-r--r--   0        0        0     7046 2023-04-18 23:52:27.705419 django_ocs_observation_portal-4.7.0/observation_portal/sciapplications/tests.py
+-rw-r--r--   0        0        0     6480 2023-04-18 23:52:27.705419 django_ocs_observation_portal-4.7.0/observation_portal/sciapplications/viewsets.py
+-rw-r--r--   0        0        0    23236 2023-04-18 23:52:27.705419 django_ocs_observation_portal-4.7.0/observation_portal/settings.py
+-rw-r--r--   0        0        0      920 2023-04-18 23:52:27.705419 django_ocs_observation_portal-4.7.0/observation_portal/task_scheduler.py
+-rw-r--r--   0        0        0      601 2023-04-18 23:52:27.705419 django_ocs_observation_portal-4.7.0/observation_portal/test_runner.py
+-rw-r--r--   0        0        0     1776 2023-04-18 23:52:27.705419 django_ocs_observation_portal-4.7.0/observation_portal/test_settings.py
+-rw-r--r--   0        0        0     5507 2023-04-18 23:52:27.705419 django_ocs_observation_portal-4.7.0/observation_portal/urls.py
+-rw-r--r--   0        0        0      413 2023-04-18 23:52:27.705419 django_ocs_observation_portal-4.7.0/observation_portal/wsgi.py
+-rw-r--r--   0        0        0     2043 2023-04-18 23:52:27.709419 django_ocs_observation_portal-4.7.0/pyproject.toml
+-rw-r--r--   0        0        0    41514 1970-01-01 00:00:00.000000 django_ocs_observation_portal-4.7.0/PKG-INFO
```

### Comparing `django_ocs_observation_portal-4.6.0/LICENSE` & `django_ocs_observation_portal-4.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/README.md` & `django_ocs_observation_portal-4.7.0/README.md`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/accounts/admin.py` & `django_ocs_observation_portal-4.7.0/observation_portal/accounts/admin.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/accounts/backends.py` & `django_ocs_observation_portal-4.7.0/observation_portal/accounts/backends.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/accounts/forms.py` & `django_ocs_observation_portal-4.7.0/observation_portal/accounts/forms.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/accounts/management/commands/create_application.py` & `django_ocs_observation_portal-4.7.0/observation_portal/accounts/management/commands/create_application.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/accounts/management/commands/create_user.py` & `django_ocs_observation_portal-4.7.0/observation_portal/accounts/management/commands/create_user.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/accounts/management/commands/generateschema_mocked.py` & `django_ocs_observation_portal-4.7.0/observation_portal/accounts/management/commands/generateschema_mocked.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/accounts/management/commands/init_e2e_credentials.py` & `django_ocs_observation_portal-4.7.0/observation_portal/accounts/management/commands/init_e2e_credentials.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/accounts/management/commands/updateclientusers.py` & `django_ocs_observation_portal-4.7.0/observation_portal/accounts/management/commands/updateclientusers.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/accounts/migrations/0001_initial.py` & `django_ocs_observation_portal-4.7.0/observation_portal/accounts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/accounts/migrations/0003_bulk_create_users_api.py` & `django_ocs_observation_portal-4.7.0/observation_portal/accounts/migrations/0003_bulk_create_users_api.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/accounts/models.py` & `django_ocs_observation_portal-4.7.0/observation_portal/accounts/models.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/accounts/oauth2_migrations/0001_initial.py` & `django_ocs_observation_portal-4.7.0/observation_portal/accounts/oauth2_migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/accounts/oauth2_migrations/0002_auto_20210715_0630.py` & `django_ocs_observation_portal-4.7.0/observation_portal/accounts/oauth2_migrations/0002_auto_20210715_0630.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/accounts/oauth2_migrations/0003_alter_accesstoken_user_alter_application_user_and_more.py` & `django_ocs_observation_portal-4.7.0/observation_portal/accounts/oauth2_migrations/0003_alter_accesstoken_user_alter_application_user_and_more.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/accounts/permissions.py` & `django_ocs_observation_portal-4.7.0/observation_portal/accounts/permissions.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/accounts/serializers.py` & `django_ocs_observation_portal-4.7.0/observation_portal/accounts/serializers.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/accounts/signals/handlers.py` & `django_ocs_observation_portal-4.7.0/observation_portal/accounts/signals/handlers.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/accounts/tasks.py` & `django_ocs_observation_portal-4.7.0/observation_portal/accounts/tasks.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/accounts/templates/redoc.html` & `django_ocs_observation_portal-4.7.0/observation_portal/accounts/templates/redoc.html`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/accounts/templates/registration/activation_complete.html` & `django_ocs_observation_portal-4.7.0/observation_portal/accounts/templates/registration/activation_complete.html`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/accounts/templates/registration/activation_email.html` & `django_ocs_observation_portal-4.7.0/observation_portal/accounts/templates/registration/activation_email.html`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/accounts/test_utils.py` & `django_ocs_observation_portal-4.7.0/observation_portal/accounts/test_utils.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/accounts/test_views.py` & `django_ocs_observation_portal-4.7.0/observation_portal/accounts/test_views.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/accounts/tests.py` & `django_ocs_observation_portal-4.7.0/observation_portal/accounts/tests.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/accounts/urls.py` & `django_ocs_observation_portal-4.7.0/observation_portal/accounts/urls.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/accounts/views.py` & `django_ocs_observation_portal-4.7.0/observation_portal/accounts/views.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/common/configdb.py` & `django_ocs_observation_portal-4.7.0/observation_portal/common/configdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,20 +158,22 @@
         telescope_names = set()
         for site in self.get_site_data():
             for enclosure in site['enclosure_set']:
                 for telescope in enclosure['telescope_set']:
                     telescope_names.add(telescope['name'].strip().lower())
         return [(telescope_name, telescope_name) for telescope_name in telescope_names]
 
-    def get_instrument_type_tuples(self):
+    def get_instrument_type_tuples(self, exclude_disabled=False):
         instrument_types = set()
         for site in self.get_site_data():
             for enclosure in site['enclosure_set']:
                 for telescope in enclosure['telescope_set']:
                     for instrument in telescope['instrument_set']:
+                        if exclude_disabled and instrument.get('state', '') == 'DISABLED':
+                            continue
                         instrument_types.add(instrument['instrument_type']['code'].upper())
         return [(instrument_type, instrument_type) for instrument_type in instrument_types]
 
     def get_instrument_name_tuples(self):
         instrument_names = set()
         for site in self.get_site_data():
             for enclosure in site['enclosure_set']:
```

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/common/doc_examples.py` & `django_ocs_observation_portal-4.7.0/observation_portal/common/doc_examples.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/common/downtimedb.py` & `django_ocs_observation_portal-4.7.0/observation_portal/common/downtimedb.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/common/middleware.py` & `django_ocs_observation_portal-4.7.0/observation_portal/common/middleware.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/common/mixins.py` & `django_ocs_observation_portal-4.7.0/observation_portal/common/mixins.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/common/rise_set_utils.py` & `django_ocs_observation_portal-4.7.0/observation_portal/common/rise_set_utils.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/common/schema.py` & `django_ocs_observation_portal-4.7.0/observation_portal/common/schema.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/common/state_changes.py` & `django_ocs_observation_portal-4.7.0/observation_portal/common/state_changes.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/common/telescope_states.py` & `django_ocs_observation_portal-4.7.0/observation_portal/common/telescope_states.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/common/test_configdb.py` & `django_ocs_observation_portal-4.7.0/observation_portal/common/test_configdb.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/common/test_data/configdb.json` & `django_ocs_observation_portal-4.7.0/observation_portal/common/test_data/configdb.json`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/common/test_data/doc_configdb.json` & `django_ocs_observation_portal-4.7.0/observation_portal/common/test_data/doc_configdb.json`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/common/test_data/es_telescope_states_data.txt` & `django_ocs_observation_portal-4.7.0/observation_portal/common/test_data/es_telescope_states_data.txt`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/common/test_helpers.py` & `django_ocs_observation_portal-4.7.0/observation_portal/common/test_helpers.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/common/test_state_changes.py` & `django_ocs_observation_portal-4.7.0/observation_portal/common/test_state_changes.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/common/test_telescope_states.py` & `django_ocs_observation_portal-4.7.0/observation_portal/common/test_telescope_states.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/common/utils.py` & `django_ocs_observation_portal-4.7.0/observation_portal/common/utils.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/observations/admin.py` & `django_ocs_observation_portal-4.7.0/observation_portal/observations/admin.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/observations/filters.py` & `django_ocs_observation_portal-4.7.0/observation_portal/observations/filters.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/observations/forms.py` & `django_ocs_observation_portal-4.7.0/observation_portal/observations/forms.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/observations/management/commands/populate_time_charged.py` & `django_ocs_observation_portal-4.7.0/observation_portal/observations/management/commands/populate_time_charged.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/observations/management/commands/time_accounting.py` & `django_ocs_observation_portal-4.7.0/observation_portal/observations/management/commands/time_accounting.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/observations/migrations/0001_initial.py` & `django_ocs_observation_portal-4.7.0/observation_portal/observations/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/observations/migrations/0003_auto_20190514_0005.py` & `django_ocs_observation_portal-4.7.0/observation_portal/observations/migrations/0003_auto_20190514_0005.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/observations/migrations/0005_auto_20210116_0033.py` & `django_ocs_observation_portal-4.7.0/observation_portal/observations/migrations/0005_auto_20210116_0033.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/observations/migrations/0008_configurationstatus_time_charged.py` & `django_ocs_observation_portal-4.7.0/observation_portal/observations/migrations/0008_configurationstatus_time_charged.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/observations/models.py` & `django_ocs_observation_portal-4.7.0/observation_portal/observations/models.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/observations/serializers.py` & `django_ocs_observation_portal-4.7.0/observation_portal/observations/serializers.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/observations/signals/handlers.py` & `django_ocs_observation_portal-4.7.0/observation_portal/observations/signals/handlers.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/observations/test/tests.py` & `django_ocs_observation_portal-4.7.0/observation_portal/observations/test/tests.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/observations/time_accounting.py` & `django_ocs_observation_portal-4.7.0/observation_portal/observations/time_accounting.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/observations/views.py` & `django_ocs_observation_portal-4.7.0/observation_portal/observations/views.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/observations/viewsets.py` & `django_ocs_observation_portal-4.7.0/observation_portal/observations/viewsets.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/proposals/admin.py` & `django_ocs_observation_portal-4.7.0/observation_portal/proposals/admin.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/proposals/filters.py` & `django_ocs_observation_portal-4.7.0/observation_portal/proposals/filters.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/proposals/forms.py` & `django_ocs_observation_portal-4.7.0/observation_portal/proposals/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 class TimeAllocationForm(forms.ModelForm):
     class Meta:
         model = TimeAllocation
         fields = '__all__'
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.fields['instrument_types'] = forms.MultipleChoiceField(choices=configdb.get_instrument_type_tuples())
+        self.fields['instrument_types'] = forms.MultipleChoiceField(choices=sorted(configdb.get_instrument_type_tuples(exclude_disabled=True)))
 
     def clean(self):
         cleaned_data = super().clean()
         if self.instance.pk is None:
             return
         instrument_types_changed = cleaned_data.get('instrument_types') != self.instance.instrument_types
         semester_changed = cleaned_data.get('semester') != self.instance.semester
```

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/proposals/management/commands/create_proposal.py` & `django_ocs_observation_portal-4.7.0/observation_portal/proposals/management/commands/create_proposal.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/proposals/management/commands/create_semester.py` & `django_ocs_observation_portal-4.7.0/observation_portal/proposals/management/commands/create_semester.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/proposals/migrations/0001_initial.py` & `django_ocs_observation_portal-4.7.0/observation_portal/proposals/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/proposals/migrations/0002_auto_20190815_1942.py` & `django_ocs_observation_portal-4.7.0/observation_portal/proposals/migrations/0002_auto_20190815_1942.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/proposals/migrations/0004_auto_20210617_0908.py` & `django_ocs_observation_portal-4.7.0/observation_portal/proposals/migrations/0004_auto_20210617_0908.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/proposals/migrations/0005_auto_20210604_2154.py` & `django_ocs_observation_portal-4.7.0/observation_portal/proposals/migrations/0005_auto_20210604_2154.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/proposals/migrations/0006_auto_20210604_2155.py` & `django_ocs_observation_portal-4.7.0/observation_portal/proposals/migrations/0006_auto_20210604_2155.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/proposals/migrations/0007_remove_timeallocation_instrument_type.py` & `django_ocs_observation_portal-4.7.0/observation_portal/proposals/migrations/0007_remove_timeallocation_instrument_type.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/proposals/migrations/0008_auto_20210708_1623.py` & `django_ocs_observation_portal-4.7.0/observation_portal/proposals/migrations/0008_auto_20210708_1623.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/proposals/models.py` & `django_ocs_observation_portal-4.7.0/observation_portal/proposals/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,17 @@
 
 class Semester(models.Model):
     id = models.CharField(primary_key=True, max_length=20)
     start = models.DateTimeField()
     end = models.DateTimeField()
     proposals = models.ManyToManyField("Proposal", through="TimeAllocation")
 
+    class Meta:
+        ordering = ["-start", "id"]
+
     @classmethod
     def current_semesters(cls, future=False):
         semesters = cls.objects.filter(end__gte=timezone.now())
         if not future:
             semesters = semesters.filter(start__lte=timezone.now())
         return semesters
```

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/proposals/notifications.py` & `django_ocs_observation_portal-4.7.0/observation_portal/proposals/notifications.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/proposals/serializers.py` & `django_ocs_observation_portal-4.7.0/observation_portal/proposals/serializers.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/proposals/signals/handlers.py` & `django_ocs_observation_portal-4.7.0/observation_portal/proposals/signals/handlers.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/proposals/tasks.py` & `django_ocs_observation_portal-4.7.0/observation_portal/proposals/tasks.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/proposals/templates/proposals/requestfailurelimit.txt` & `django_ocs_observation_portal-4.7.0/observation_portal/proposals/templates/proposals/requestfailurelimit.txt`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/proposals/templates/proposals/requestgroupcomplete.txt` & `django_ocs_observation_portal-4.7.0/observation_portal/proposals/templates/proposals/requestgroupcomplete.txt`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/proposals/templates/proposals/timeallocationreminder.html` & `django_ocs_observation_portal-4.7.0/observation_portal/proposals/templates/proposals/timeallocationreminder.html`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/proposals/test_api.py` & `django_ocs_observation_portal-4.7.0/observation_portal/proposals/test_api.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/proposals/tests.py` & `django_ocs_observation_portal-4.7.0/observation_portal/proposals/tests.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/proposals/viewsets.py` & `django_ocs_observation_portal-4.7.0/observation_portal/proposals/viewsets.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/admin.py` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/admin.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/cadence.py` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/cadence.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/contention.py` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/contention.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/duration_utils.py` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/duration_utils.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/filters.py` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/filters.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/forms.py` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/forms.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/management/commands/create_example_requests.py` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/management/commands/create_example_requests.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0001_initial.py` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0002_auto_20190319_1814.py` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0002_auto_20190319_1814.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0003_acquisitionconfig_exposure_time.py` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0003_acquisitionconfig_exposure_time.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0004_auto_20190410_0103.py` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0004_auto_20190410_0103.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0006_auto_20190514_0005.py` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0006_auto_20190514_0005.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0007_auto_20190516_1713.py` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0007_auto_20190516_1713.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0008_auto_20190516_2055.py` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0008_auto_20190516_2055.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0009_auto_20190518_0023.py` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0009_auto_20190518_0023.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0010_auto_20190612_0048.py` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0010_auto_20190612_0048.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0011_auto_20190702_2014.py` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0011_auto_20190702_2014.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0012_auto_20191123_0233.py` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0012_auto_20191123_0233.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0013_auto_20191220_0711.py` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0013_auto_20191220_0711.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0014_auto_20210123_0715.py` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0014_auto_20210123_0715.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0015_auto_20210323_0635.py` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0015_auto_20210323_0635.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0017_request_extra_params.py` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0017_request_extra_params.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0018_alter_acquisitionconfig_extra_params_and_more.py` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0018_alter_acquisitionconfig_extra_params_and_more.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0019_request_configuration_repeats.py` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0019_request_configuration_repeats.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0020_alter_constraints_max_lunar_phase.py` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0020_alter_constraints_max_lunar_phase.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0021_request_optimization_type.py` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0021_request_optimization_type.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0022_alter_constraints_max_seeing.py` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0022_alter_constraints_max_seeing.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0023_alter_target_epochofperih.py` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/migrations/0023_alter_target_epochofperih.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/models.py` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/models.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/pattern_expansion.py` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/pattern_expansion.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/request_utils.py` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/request_utils.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/serializers.py` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/serializers.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/signals/handlers.py` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/signals/handlers.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/target_helpers.py` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/target_helpers.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/test/data/blocks.json` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/test/data/blocks.json`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/test/test.py` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/test/test.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/test/test_api.py` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/test/test_api.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/test/test_cadence.py` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/test/test_cadence.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/test/test_helpers.py` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/test/test_helpers.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/test/test_request_utils.py` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/test/test_request_utils.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/test/test_views.py` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/test/test_views.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/views.py` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/views.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/viewsets.py` & `django_ocs_observation_portal-4.7.0/observation_portal/requestgroups/viewsets.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/admin.py` & `django_ocs_observation_portal-4.7.0/observation_portal/sciapplications/admin.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/filters.py` & `django_ocs_observation_portal-4.7.0/observation_portal/sciapplications/filters.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/migrations/0001_initial.py` & `django_ocs_observation_portal-4.7.0/observation_portal/sciapplications/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/migrations/0003_auto_20210604_2155.py` & `django_ocs_observation_portal-4.7.0/observation_portal/sciapplications/migrations/0003_auto_20210604_2155.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/migrations/0005_auto_20210708_1623.py` & `django_ocs_observation_portal-4.7.0/observation_portal/sciapplications/migrations/0005_auto_20210708_1623.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/models.py` & `django_ocs_observation_portal-4.7.0/observation_portal/sciapplications/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,17 @@
     pass
 
 
 class Instrument(models.Model):
     code = models.CharField(max_length=50)
     display = models.CharField(max_length=50)
 
+    class Meta:
+        ordering = ["code"]
+
     @cached_property
     def telescope_name(self):
         instrument_type_to_telescope_name = configdb.get_telescope_name_by_instrument_types(exclude_states=['DISABLED'])
         return instrument_type_to_telescope_name.get(self.code.upper(), '')
 
     def __str__(self):
         return self.display
```

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/serializers.py` & `django_ocs_observation_portal-4.7.0/observation_portal/sciapplications/serializers.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/test_admin.py` & `django_ocs_observation_portal-4.7.0/observation_portal/sciapplications/test_admin.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/test_api.py` & `django_ocs_observation_portal-4.7.0/observation_portal/sciapplications/test_api.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/tests.py` & `django_ocs_observation_portal-4.7.0/observation_portal/sciapplications/tests.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/viewsets.py` & `django_ocs_observation_portal-4.7.0/observation_portal/sciapplications/viewsets.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/settings.py` & `django_ocs_observation_portal-4.7.0/observation_portal/settings.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/task_scheduler.py` & `django_ocs_observation_portal-4.7.0/observation_portal/task_scheduler.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/test_runner.py` & `django_ocs_observation_portal-4.7.0/observation_portal/test_runner.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/test_settings.py` & `django_ocs_observation_portal-4.7.0/observation_portal/test_settings.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/observation_portal/urls.py` & `django_ocs_observation_portal-4.7.0/observation_portal/urls.py`

 * *Files identical despite different names*

### Comparing `django_ocs_observation_portal-4.6.0/pyproject.toml` & `django_ocs_observation_portal-4.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-ocs-observation-portal"
-version = "4.6.0"
+version = "4.7.0"
 description = "The Observatory Control System (OCS) Observation Portal django apps"
 license = "GPL-3.0-only"
 authors = ["Observatory Control System Project <ocs@lco.global>"]
 readme = "README.md"
 homepage = "https://observatorycontrolsystem.github.io"
 repository = "https://github.com/observatorycontrolsystem/observation-portal"
 keywords = [
```

### Comparing `django_ocs_observation_portal-4.6.0/PKG-INFO` & `django_ocs_observation_portal-4.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ocs-observation-portal
-Version: 4.6.0
+Version: 4.7.0
 Summary: The Observatory Control System (OCS) Observation Portal django apps
 Home-page: https://observatorycontrolsystem.github.io
 License: GPL-3.0-only
 Keywords: observations,astronomy,astrophysics,cosmology,science
 Author: Observatory Control System Project
 Author-email: ocs@lco.global
 Requires-Python: >=3.8,<3.11
```

