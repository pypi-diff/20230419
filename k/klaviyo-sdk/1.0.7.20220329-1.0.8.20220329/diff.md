# Comparing `tmp/klaviyo-sdk-1.0.7.20220329.tar.gz` & `tmp/klaviyo-sdk-1.0.8.20220329.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klaviyo-sdk-1.0.7.20220329.tar", last modified: Tue Oct 25 18:30:58 2022, max compression
+gzip compressed data, was "klaviyo-sdk-1.0.8.20220329.tar", last modified: Wed Apr 19 19:05:06 2023, max compression
```

## Comparing `klaviyo-sdk-1.0.7.20220329.tar` & `klaviyo-sdk-1.0.8.20220329.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 local      (503) staff       (20)        0 2022-10-25 18:30:58.128345 klaviyo-sdk-1.0.7.20220329/
--rw-r--r--   0 local      (503) staff       (20)     1063 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.7.20220329/LICENSE
--rw-r--r--   0 local      (503) staff       (20)     1745 2022-10-25 18:30:58.128485 klaviyo-sdk-1.0.7.20220329/PKG-INFO
--rw-r--r--   0 local      (503) staff       (20)     1245 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.7.20220329/README.md
--rw-r--r--   0 local      (503) staff       (20)      103 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.7.20220329/pyproject.toml
--rw-r--r--   0 local      (503) staff       (20)      785 2022-10-25 18:30:58.129064 klaviyo-sdk-1.0.7.20220329/setup.cfg
-drwxr-xr-x   0 local      (503) staff       (20)        0 2022-10-25 18:30:58.085616 klaviyo-sdk-1.0.7.20220329/src/
-drwxr-xr-x   0 local      (503) staff       (20)        0 2022-10-25 18:30:58.088168 klaviyo-sdk-1.0.7.20220329/src/klaviyo_sdk/
--rw-r--r--   0 local      (503) staff       (20)       78 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.7.20220329/src/klaviyo_sdk/__init__.py
--rw-r--r--   0 local      (503) staff       (20)      501 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.7.20220329/src/klaviyo_sdk/custom_retry.py
--rw-r--r--   0 local      (503) staff       (20)     9850 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.7.20220329/src/klaviyo_sdk/wrapper.py
-drwxr-xr-x   0 local      (503) staff       (20)        0 2022-10-25 18:30:58.089485 klaviyo-sdk-1.0.7.20220329/src/klaviyo_sdk.egg-info/
--rw-r--r--   0 local      (503) staff       (20)     1745 2022-10-25 18:30:58.000000 klaviyo-sdk-1.0.7.20220329/src/klaviyo_sdk.egg-info/PKG-INFO
--rw-r--r--   0 local      (503) staff       (20)     5680 2022-10-25 18:30:58.000000 klaviyo-sdk-1.0.7.20220329/src/klaviyo_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 local      (503) staff       (20)        1 2022-10-25 18:30:58.000000 klaviyo-sdk-1.0.7.20220329/src/klaviyo_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 local      (503) staff       (20)      119 2022-10-25 18:30:58.000000 klaviyo-sdk-1.0.7.20220329/src/klaviyo_sdk.egg-info/requires.txt
--rw-r--r--   0 local      (503) staff       (20)       27 2022-10-25 18:30:58.000000 klaviyo-sdk-1.0.7.20220329/src/klaviyo_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 local      (503) staff       (20)        0 2022-10-25 18:30:58.090579 klaviyo-sdk-1.0.7.20220329/src/swagger_client/
--rw-r--r--   0 local      (503) staff       (20)     7853 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/__init__.py
-drwxr-xr-x   0 local      (503) staff       (20)        0 2022-10-25 18:30:58.092987 klaviyo-sdk-1.0.7.20220329/src/swagger_client/api/
--rw-r--r--   0 local      (503) staff       (20)      512 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/api/__init__.py
--rw-r--r--   0 local      (503) staff       (20)    39918 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/api/campaigns_api.py
--rw-r--r--   0 local      (503) staff       (20)     5626 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/api/data_privacy_api.py
--rw-r--r--   0 local      (503) staff       (20)    66520 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/api/lists__segments_api.py
--rw-r--r--   0 local      (503) staff       (20)    22259 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/api/metrics_api.py
--rw-r--r--   0 local      (503) staff       (20)    28958 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/api/profiles_api.py
--rw-r--r--   0 local      (503) staff       (20)    29688 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/api/templates_api.py
--rw-r--r--   0 local      (503) staff       (20)    26448 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/api/track__identify_api.py
--rw-r--r--   0 local      (503) staff       (20)    25256 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/api_client.py
--rw-r--r--   0 local      (503) staff       (20)     8146 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/configuration.py
-drwxr-xr-x   0 local      (503) staff       (20)        0 2022-10-25 18:30:58.128078 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/
--rw-r--r--   0 local      (503) staff       (20)     7276 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/__init__.py
--rw-r--r--   0 local      (503) staff       (20)     2373 2022-10-25 18:30:46.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/ascending.py
--rw-r--r--   0 local      (503) staff       (20)     2605 2022-10-25 18:30:46.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/campaign.py
--rw-r--r--   0 local      (503) staff       (20)    10331 2022-10-25 18:30:46.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/campaign_campaign_id_body.py
--rw-r--r--   0 local      (503) staff       (20)     4568 2022-10-25 18:30:46.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/campaign_id_clone_body.py
--rw-r--r--   0 local      (503) staff       (20)     3483 2022-10-25 18:30:46.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/campaign_id_schedule_body.py
--rw-r--r--   0 local      (503) staff       (20)     4178 2022-10-25 18:30:46.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/campaign_template.py
--rw-r--r--   0 local      (503) staff       (20)     4868 2022-10-25 18:30:46.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/check_membership_request.py
--rw-r--r--   0 local      (503) staff       (20)     2429 2022-10-25 18:30:46.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/check_membership_response.py
--rw-r--r--   0 local      (503) staff       (20)     2685 2022-10-25 18:30:46.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/check_membership_response_inner.py
--rw-r--r--   0 local      (503) staff       (20)     2972 2022-10-25 18:30:46.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/delete_email.py
--rw-r--r--   0 local      (503) staff       (20)     3060 2022-10-25 18:30:46.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/delete_person.py
--rw-r--r--   0 local      (503) staff       (20)     3182 2022-10-25 18:30:46.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/delete_phone.py
--rw-r--r--   0 local      (503) staff       (20)     6994 2022-10-25 18:30:46.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/deprecated_get_list_response.py
--rw-r--r--   0 local      (503) staff       (20)     6601 2022-10-25 18:30:46.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/deprecated_get_list_response_data.py
--rw-r--r--   0 local      (503) staff       (20)     2377 2022-10-25 18:30:46.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/descending.py
--rw-r--r--   0 local      (503) staff       (20)     3957 2022-10-25 18:30:46.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/emailtemplate_template_id_body.py
--rw-r--r--   0 local      (503) staff       (20)     2681 2022-10-25 18:30:46.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/global_exclusion_response_data.py
--rw-r--r--   0 local      (503) staff       (20)     5271 2022-10-25 18:30:46.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/global_exclusion_response_data_data.py
--rw-r--r--   0 local      (503) staff       (20)     3952 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/identify_payload.py
--rw-r--r--   0 local      (503) staff       (20)     3172 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/identify_payload_post.py
--rw-r--r--   0 local      (503) staff       (20)    11750 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/identify_payload_properties.py
--rw-r--r--   0 local      (503) staff       (20)     2641 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/inline_response200.py
--rw-r--r--   0 local      (503) staff       (20)     2968 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/inline_response2001.py
--rw-r--r--   0 local      (503) staff       (20)     2649 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/inline_response20010.py
--rw-r--r--   0 local      (503) staff       (20)     2649 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/inline_response20011.py
--rw-r--r--   0 local      (503) staff       (20)     5271 2022-10-25 18:17:23.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/inline_response20011_data.py
--rw-r--r--   0 local      (503) staff       (20)     2649 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/inline_response20012.py
--rw-r--r--   0 local      (503) staff       (20)     5271 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/inline_response20012_data.py
--rw-r--r--   0 local      (503) staff       (20)     2649 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/inline_response20013.py
--rw-r--r--   0 local      (503) staff       (20)     2649 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/inline_response20014.py
--rw-r--r--   0 local      (503) staff       (20)     2645 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/inline_response2002.py
--rw-r--r--   0 local      (503) staff       (20)     2645 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/inline_response2003.py
--rw-r--r--   0 local      (503) staff       (20)     2645 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/inline_response2004.py
--rw-r--r--   0 local      (503) staff       (20)     2645 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/inline_response2005.py
--rw-r--r--   0 local      (503) staff       (20)     2645 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/inline_response2006.py
--rw-r--r--   0 local      (503) staff       (20)     2645 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/inline_response2007.py
--rw-r--r--   0 local      (503) staff       (20)     5920 2022-10-25 18:17:23.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/inline_response2007_records.py
--rw-r--r--   0 local      (503) staff       (20)     2645 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/inline_response2008.py
--rw-r--r--   0 local      (503) staff       (20)     5920 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/inline_response2008_records.py
--rw-r--r--   0 local      (503) staff       (20)     2645 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/inline_response2009.py
--rw-r--r--   0 local      (503) staff       (20)     5211 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/inline_response2009_records.py
--rw-r--r--   0 local      (503) staff       (20)     3227 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/list_id_members_body.py
--rw-r--r--   0 local      (503) staff       (20)     4624 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/list_id_members_body1.py
--rw-r--r--   0 local      (503) staff       (20)     3243 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/list_id_subscribe_body.py
--rw-r--r--   0 local      (503) staff       (20)     2653 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/list_id_subscribe_body1.py
--rw-r--r--   0 local      (503) staff       (20)     3175 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/list_list_id_body.py
--rw-r--r--   0 local      (503) staff       (20)     2453 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/list_subscribe_post_response_data.py
--rw-r--r--   0 local      (503) staff       (20)     4606 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/list_subscribe_post_response_data_inner.py
--rw-r--r--   0 local      (503) staff       (20)     2401 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/measurement_count.py
--rw-r--r--   0 local      (503) staff       (20)     2393 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/measurement_sum.py
--rw-r--r--   0 local      (503) staff       (20)     2405 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/measurement_unique.py
--rw-r--r--   0 local      (503) staff       (20)     2401 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/measurement_value.py
--rw-r--r--   0 local      (503) staff       (20)     2597 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/metric.py
--rw-r--r--   0 local      (503) staff       (20)     2621 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/metric_export.py
--rw-r--r--   0 local      (503) staff       (20)     3668 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/metric_export_data.py
--rw-r--r--   0 local      (503) staff       (20)     6315 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/metric_export_metric.py
--rw-r--r--   0 local      (503) staff       (20)     3738 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/metric_export_results.py
--rw-r--r--   0 local      (503) staff       (20)     4871 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/metric_integration.py
--rw-r--r--   0 local      (503) staff       (20)     2629 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/metric_timeline.py
--rw-r--r--   0 local      (503) staff       (20)     8704 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/metric_timeline_data.py
--rw-r--r--   0 local      (503) staff       (20)     3177 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/metric_timeline_event_properties.py
--rw-r--r--   0 local      (503) staff       (20)     3633 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/metric_timeline_person.py
--rw-r--r--   0 local      (503) staff       (20)     2377 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/model200ok.py
--rw-r--r--   0 local      (503) staff       (20)     2517 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/one_ofidentify_payload_properties_your_custom_field.py
--rw-r--r--   0 local      (503) staff       (20)     2429 2022-10-25 18:17:23.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/one_ofinline_response2006.py
--rw-r--r--   0 local      (503) staff       (20)     2505 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/one_oftrack_payload_properties_your_custom_field.py
--rw-r--r--   0 local      (503) staff       (20)     2421 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/one_oftrack_payload_time.py
--rw-r--r--   0 local      (503) staff       (20)     3247 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/people_exchange_body.py
--rw-r--r--   0 local      (503) staff       (20)     3155 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/people_exclusions_body.py
--rw-r--r--   0 local      (503) staff       (20)     2597 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/person.py
--rw-r--r--   0 local      (503) staff       (20)     2980 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/privacy_email.py
--rw-r--r--   0 local      (503) staff       (20)     3036 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/privacy_id.py
--rw-r--r--   0 local      (503) staff       (20)     3120 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/privacy_phone.py
--rw-r--r--   0 local      (503) staff       (20)     2389 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/reason_bounced.py
--rw-r--r--   0 local      (503) staff       (20)     2409 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/reason_invalid_email.py
--rw-r--r--   0 local      (503) staff       (20)     2425 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/reason_manually_excluded.py
--rw-r--r--   0 local      (503) staff       (20)     2409 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/reason_reported_spam.py
--rw-r--r--   0 local      (503) staff       (20)     2409 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/reason_unsubscribed.py
--rw-r--r--   0 local      (503) staff       (20)     2637 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/rendered_template.py
--rw-r--r--   0 local      (503) staff       (20)     3633 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/renderedtemplate_data.py
--rw-r--r--   0 local      (503) staff       (20)     2385 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/since_integer.py
--rw-r--r--   0 local      (503) staff       (20)     2381 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/since_string.py
--rw-r--r--   0 local      (503) staff       (20)     2381 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/string_array.py
--rw-r--r--   0 local      (503) staff       (20)     2605 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/template.py
--rw-r--r--   0 local      (503) staff       (20)     3231 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/template_id_clone_body.py
--rw-r--r--   0 local      (503) staff       (20)     3858 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/template_id_render_body.py
--rw-r--r--   0 local      (503) staff       (20)     7559 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/template_id_send_body.py
--rw-r--r--   0 local      (503) staff       (20)     5594 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/track_payload.py
--rw-r--r--   0 local      (503) staff       (20)     3935 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/track_payload_customer_properties.py
--rw-r--r--   0 local      (503) staff       (20)     3242 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/track_payload_post.py
--rw-r--r--   0 local      (503) staff       (20)     4753 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/track_payload_properties.py
--rw-r--r--   0 local      (503) staff       (20)     2365 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/unit_day.py
--rw-r--r--   0 local      (503) staff       (20)     2373 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/unit_month.py
--rw-r--r--   0 local      (503) staff       (20)     2369 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/unit_week.py
--rw-r--r--   0 local      (503) staff       (20)    10651 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/v1_campaigns_body.py
--rw-r--r--   0 local      (503) staff       (20)     3986 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/v1_emailtemplates_body.py
--rw-r--r--   0 local      (503) staff       (20)     2617 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/v2_lists_body.py
--rw-r--r--   0 local      (503) staff       (20)    12965 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.7.20220329/src/swagger_client/rest.py
+drwxr-xr-x   0 local      (503) staff       (20)        0 2023-04-19 19:05:06.166721 klaviyo-sdk-1.0.8.20220329/
+-rw-r--r--   0 local      (503) staff       (20)     1063 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.8.20220329/LICENSE
+-rw-r--r--   0 local      (503) staff       (20)    14466 2023-04-19 19:05:06.166908 klaviyo-sdk-1.0.8.20220329/PKG-INFO
+-rw-r--r--   0 local      (503) staff       (20)    13956 2023-04-19 19:04:05.000000 klaviyo-sdk-1.0.8.20220329/README.md
+-rw-r--r--   0 local      (503) staff       (20)      103 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.8.20220329/pyproject.toml
+-rw-r--r--   0 local      (503) staff       (20)      794 2023-04-19 19:05:06.167669 klaviyo-sdk-1.0.8.20220329/setup.cfg
+drwxr-xr-x   0 local      (503) staff       (20)        0 2023-04-19 19:05:06.116825 klaviyo-sdk-1.0.8.20220329/src/
+drwxr-xr-x   0 local      (503) staff       (20)        0 2023-04-19 19:05:06.120140 klaviyo-sdk-1.0.8.20220329/src/klaviyo_sdk/
+-rw-r--r--   0 local      (503) staff       (20)       78 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.8.20220329/src/klaviyo_sdk/__init__.py
+-rw-r--r--   0 local      (503) staff       (20)      501 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.8.20220329/src/klaviyo_sdk/custom_retry.py
+-rw-r--r--   0 local      (503) staff       (20)     9850 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.8.20220329/src/klaviyo_sdk/wrapper.py
+drwxr-xr-x   0 local      (503) staff       (20)        0 2023-04-19 19:05:06.122294 klaviyo-sdk-1.0.8.20220329/src/klaviyo_sdk.egg-info/
+-rw-r--r--   0 local      (503) staff       (20)    14466 2023-04-19 19:05:06.000000 klaviyo-sdk-1.0.8.20220329/src/klaviyo_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 local      (503) staff       (20)     5680 2023-04-19 19:05:06.000000 klaviyo-sdk-1.0.8.20220329/src/klaviyo_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 local      (503) staff       (20)        1 2023-04-19 19:05:06.000000 klaviyo-sdk-1.0.8.20220329/src/klaviyo_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 local      (503) staff       (20)      119 2023-04-19 19:05:06.000000 klaviyo-sdk-1.0.8.20220329/src/klaviyo_sdk.egg-info/requires.txt
+-rw-r--r--   0 local      (503) staff       (20)       27 2023-04-19 19:05:06.000000 klaviyo-sdk-1.0.8.20220329/src/klaviyo_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 local      (503) staff       (20)        0 2023-04-19 19:05:06.123939 klaviyo-sdk-1.0.8.20220329/src/swagger_client/
+-rw-r--r--   0 local      (503) staff       (20)     7853 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/__init__.py
+drwxr-xr-x   0 local      (503) staff       (20)        0 2023-04-19 19:05:06.127225 klaviyo-sdk-1.0.8.20220329/src/swagger_client/api/
+-rw-r--r--   0 local      (503) staff       (20)      512 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/api/__init__.py
+-rw-r--r--   0 local      (503) staff       (20)    39918 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/api/campaigns_api.py
+-rw-r--r--   0 local      (503) staff       (20)     5626 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/api/data_privacy_api.py
+-rw-r--r--   0 local      (503) staff       (20)    66520 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/api/lists__segments_api.py
+-rw-r--r--   0 local      (503) staff       (20)    22259 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/api/metrics_api.py
+-rw-r--r--   0 local      (503) staff       (20)    28958 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/api/profiles_api.py
+-rw-r--r--   0 local      (503) staff       (20)    29688 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/api/templates_api.py
+-rw-r--r--   0 local      (503) staff       (20)    26448 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/api/track__identify_api.py
+-rw-r--r--   0 local      (503) staff       (20)    25256 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/api_client.py
+-rw-r--r--   0 local      (503) staff       (20)     8146 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/configuration.py
+drwxr-xr-x   0 local      (503) staff       (20)        0 2023-04-19 19:05:06.166429 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/
+-rw-r--r--   0 local      (503) staff       (20)     7276 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/__init__.py
+-rw-r--r--   0 local      (503) staff       (20)     2373 2022-10-25 18:30:46.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/ascending.py
+-rw-r--r--   0 local      (503) staff       (20)     2605 2022-10-25 18:30:46.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/campaign.py
+-rw-r--r--   0 local      (503) staff       (20)    10331 2022-10-25 18:30:46.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/campaign_campaign_id_body.py
+-rw-r--r--   0 local      (503) staff       (20)     4568 2022-10-25 18:30:46.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/campaign_id_clone_body.py
+-rw-r--r--   0 local      (503) staff       (20)     3483 2022-10-25 18:30:46.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/campaign_id_schedule_body.py
+-rw-r--r--   0 local      (503) staff       (20)     4178 2022-10-25 18:30:46.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/campaign_template.py
+-rw-r--r--   0 local      (503) staff       (20)     4868 2022-10-25 18:30:46.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/check_membership_request.py
+-rw-r--r--   0 local      (503) staff       (20)     2429 2022-10-25 18:30:46.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/check_membership_response.py
+-rw-r--r--   0 local      (503) staff       (20)     2685 2022-10-25 18:30:46.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/check_membership_response_inner.py
+-rw-r--r--   0 local      (503) staff       (20)     2972 2022-10-25 18:30:46.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/delete_email.py
+-rw-r--r--   0 local      (503) staff       (20)     3060 2022-10-25 18:30:46.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/delete_person.py
+-rw-r--r--   0 local      (503) staff       (20)     3182 2022-10-25 18:30:46.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/delete_phone.py
+-rw-r--r--   0 local      (503) staff       (20)     6994 2022-10-25 18:30:46.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/deprecated_get_list_response.py
+-rw-r--r--   0 local      (503) staff       (20)     6601 2022-10-25 18:30:46.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/deprecated_get_list_response_data.py
+-rw-r--r--   0 local      (503) staff       (20)     2377 2022-10-25 18:30:46.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/descending.py
+-rw-r--r--   0 local      (503) staff       (20)     3957 2022-10-25 18:30:46.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/emailtemplate_template_id_body.py
+-rw-r--r--   0 local      (503) staff       (20)     2681 2022-10-25 18:30:46.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/global_exclusion_response_data.py
+-rw-r--r--   0 local      (503) staff       (20)     5271 2022-10-25 18:30:46.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/global_exclusion_response_data_data.py
+-rw-r--r--   0 local      (503) staff       (20)     3952 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/identify_payload.py
+-rw-r--r--   0 local      (503) staff       (20)     3172 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/identify_payload_post.py
+-rw-r--r--   0 local      (503) staff       (20)    11750 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/identify_payload_properties.py
+-rw-r--r--   0 local      (503) staff       (20)     2641 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/inline_response200.py
+-rw-r--r--   0 local      (503) staff       (20)     2968 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/inline_response2001.py
+-rw-r--r--   0 local      (503) staff       (20)     2649 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/inline_response20010.py
+-rw-r--r--   0 local      (503) staff       (20)     2649 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/inline_response20011.py
+-rw-r--r--   0 local      (503) staff       (20)     5271 2022-10-25 18:17:23.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/inline_response20011_data.py
+-rw-r--r--   0 local      (503) staff       (20)     2649 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/inline_response20012.py
+-rw-r--r--   0 local      (503) staff       (20)     5271 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/inline_response20012_data.py
+-rw-r--r--   0 local      (503) staff       (20)     2649 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/inline_response20013.py
+-rw-r--r--   0 local      (503) staff       (20)     2649 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/inline_response20014.py
+-rw-r--r--   0 local      (503) staff       (20)     2645 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/inline_response2002.py
+-rw-r--r--   0 local      (503) staff       (20)     2645 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/inline_response2003.py
+-rw-r--r--   0 local      (503) staff       (20)     2645 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/inline_response2004.py
+-rw-r--r--   0 local      (503) staff       (20)     2645 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/inline_response2005.py
+-rw-r--r--   0 local      (503) staff       (20)     2645 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/inline_response2006.py
+-rw-r--r--   0 local      (503) staff       (20)     2645 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/inline_response2007.py
+-rw-r--r--   0 local      (503) staff       (20)     5920 2022-10-25 18:17:23.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/inline_response2007_records.py
+-rw-r--r--   0 local      (503) staff       (20)     2645 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/inline_response2008.py
+-rw-r--r--   0 local      (503) staff       (20)     5920 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/inline_response2008_records.py
+-rw-r--r--   0 local      (503) staff       (20)     2645 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/inline_response2009.py
+-rw-r--r--   0 local      (503) staff       (20)     5211 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/inline_response2009_records.py
+-rw-r--r--   0 local      (503) staff       (20)     3227 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/list_id_members_body.py
+-rw-r--r--   0 local      (503) staff       (20)     4624 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/list_id_members_body1.py
+-rw-r--r--   0 local      (503) staff       (20)     3243 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/list_id_subscribe_body.py
+-rw-r--r--   0 local      (503) staff       (20)     2653 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/list_id_subscribe_body1.py
+-rw-r--r--   0 local      (503) staff       (20)     3175 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/list_list_id_body.py
+-rw-r--r--   0 local      (503) staff       (20)     2453 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/list_subscribe_post_response_data.py
+-rw-r--r--   0 local      (503) staff       (20)     4606 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/list_subscribe_post_response_data_inner.py
+-rw-r--r--   0 local      (503) staff       (20)     2401 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/measurement_count.py
+-rw-r--r--   0 local      (503) staff       (20)     2393 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/measurement_sum.py
+-rw-r--r--   0 local      (503) staff       (20)     2405 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/measurement_unique.py
+-rw-r--r--   0 local      (503) staff       (20)     2401 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/measurement_value.py
+-rw-r--r--   0 local      (503) staff       (20)     2597 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/metric.py
+-rw-r--r--   0 local      (503) staff       (20)     2621 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/metric_export.py
+-rw-r--r--   0 local      (503) staff       (20)     3668 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/metric_export_data.py
+-rw-r--r--   0 local      (503) staff       (20)     6315 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/metric_export_metric.py
+-rw-r--r--   0 local      (503) staff       (20)     3738 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/metric_export_results.py
+-rw-r--r--   0 local      (503) staff       (20)     4871 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/metric_integration.py
+-rw-r--r--   0 local      (503) staff       (20)     2629 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/metric_timeline.py
+-rw-r--r--   0 local      (503) staff       (20)     8704 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/metric_timeline_data.py
+-rw-r--r--   0 local      (503) staff       (20)     3177 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/metric_timeline_event_properties.py
+-rw-r--r--   0 local      (503) staff       (20)     3633 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/metric_timeline_person.py
+-rw-r--r--   0 local      (503) staff       (20)     2377 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/model200ok.py
+-rw-r--r--   0 local      (503) staff       (20)     2517 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/one_ofidentify_payload_properties_your_custom_field.py
+-rw-r--r--   0 local      (503) staff       (20)     2429 2022-10-25 18:17:23.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/one_ofinline_response2006.py
+-rw-r--r--   0 local      (503) staff       (20)     2505 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/one_oftrack_payload_properties_your_custom_field.py
+-rw-r--r--   0 local      (503) staff       (20)     2421 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/one_oftrack_payload_time.py
+-rw-r--r--   0 local      (503) staff       (20)     3247 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/people_exchange_body.py
+-rw-r--r--   0 local      (503) staff       (20)     3155 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/people_exclusions_body.py
+-rw-r--r--   0 local      (503) staff       (20)     2597 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/person.py
+-rw-r--r--   0 local      (503) staff       (20)     2980 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/privacy_email.py
+-rw-r--r--   0 local      (503) staff       (20)     3036 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/privacy_id.py
+-rw-r--r--   0 local      (503) staff       (20)     3120 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/privacy_phone.py
+-rw-r--r--   0 local      (503) staff       (20)     2389 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/reason_bounced.py
+-rw-r--r--   0 local      (503) staff       (20)     2409 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/reason_invalid_email.py
+-rw-r--r--   0 local      (503) staff       (20)     2425 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/reason_manually_excluded.py
+-rw-r--r--   0 local      (503) staff       (20)     2409 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/reason_reported_spam.py
+-rw-r--r--   0 local      (503) staff       (20)     2409 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/reason_unsubscribed.py
+-rw-r--r--   0 local      (503) staff       (20)     2637 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/rendered_template.py
+-rw-r--r--   0 local      (503) staff       (20)     3633 2022-10-25 18:30:47.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/renderedtemplate_data.py
+-rw-r--r--   0 local      (503) staff       (20)     2385 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/since_integer.py
+-rw-r--r--   0 local      (503) staff       (20)     2381 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/since_string.py
+-rw-r--r--   0 local      (503) staff       (20)     2381 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/string_array.py
+-rw-r--r--   0 local      (503) staff       (20)     2605 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/template.py
+-rw-r--r--   0 local      (503) staff       (20)     3231 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/template_id_clone_body.py
+-rw-r--r--   0 local      (503) staff       (20)     3858 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/template_id_render_body.py
+-rw-r--r--   0 local      (503) staff       (20)     7559 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/template_id_send_body.py
+-rw-r--r--   0 local      (503) staff       (20)     5594 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/track_payload.py
+-rw-r--r--   0 local      (503) staff       (20)     3935 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/track_payload_customer_properties.py
+-rw-r--r--   0 local      (503) staff       (20)     3242 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/track_payload_post.py
+-rw-r--r--   0 local      (503) staff       (20)     4753 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/track_payload_properties.py
+-rw-r--r--   0 local      (503) staff       (20)     2365 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/unit_day.py
+-rw-r--r--   0 local      (503) staff       (20)     2373 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/unit_month.py
+-rw-r--r--   0 local      (503) staff       (20)     2369 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/unit_week.py
+-rw-r--r--   0 local      (503) staff       (20)    10651 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/v1_campaigns_body.py
+-rw-r--r--   0 local      (503) staff       (20)     3986 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/v1_emailtemplates_body.py
+-rw-r--r--   0 local      (503) staff       (20)     2617 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/v2_lists_body.py
+-rw-r--r--   0 local      (503) staff       (20)    12965 2022-10-25 18:30:48.000000 klaviyo-sdk-1.0.8.20220329/src/swagger_client/rest.py
```

### Comparing `klaviyo-sdk-1.0.7.20220329/LICENSE` & `klaviyo-sdk-1.0.8.20220329/LICENSE`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/setup.cfg` & `klaviyo-sdk-1.0.8.20220329/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = klaviyo-sdk
-version = 1.0.7.20220329
+version = 1.0.8.20220329
 author = Klaviyo Developers
 author_email = developers@klaviyo.com
-description = Klaviyo Python SDK
+description = Klaviyo Python SDK (LEGACY)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/klaviyo/klaviyo-python-sdk
 project_urls = 
 	API Docs = https://developers.klaviyo.com/
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `klaviyo-sdk-1.0.7.20220329/src/klaviyo_sdk/wrapper.py` & `klaviyo-sdk-1.0.8.20220329/src/klaviyo_sdk/wrapper.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/klaviyo_sdk.egg-info/SOURCES.txt` & `klaviyo-sdk-1.0.8.20220329/src/klaviyo_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/__init__.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/__init__.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/api/__init__.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/api/campaigns_api.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/api/campaigns_api.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/api/data_privacy_api.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/api/data_privacy_api.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/api/lists__segments_api.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/api/lists__segments_api.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/api/metrics_api.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/api/metrics_api.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/api/profiles_api.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/api/profiles_api.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/api/templates_api.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/api/templates_api.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/api/track__identify_api.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/api/track__identify_api.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/api_client.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/configuration.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/__init__.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/ascending.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/ascending.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/campaign.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/campaign.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/campaign_campaign_id_body.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/campaign_campaign_id_body.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/campaign_id_clone_body.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/campaign_id_clone_body.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/campaign_id_schedule_body.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/campaign_id_schedule_body.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/campaign_template.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/campaign_template.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/check_membership_request.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/check_membership_request.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/check_membership_response.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/check_membership_response.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/check_membership_response_inner.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/check_membership_response_inner.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/delete_email.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/delete_email.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/delete_person.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/delete_person.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/delete_phone.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/delete_phone.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/deprecated_get_list_response.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/deprecated_get_list_response.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/deprecated_get_list_response_data.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/deprecated_get_list_response_data.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/descending.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/descending.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/emailtemplate_template_id_body.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/emailtemplate_template_id_body.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/global_exclusion_response_data.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/global_exclusion_response_data.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/global_exclusion_response_data_data.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/global_exclusion_response_data_data.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/identify_payload.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/identify_payload.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/identify_payload_post.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/identify_payload_post.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/identify_payload_properties.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/identify_payload_properties.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/inline_response200.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/inline_response200.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/inline_response2001.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/inline_response2001.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/inline_response20010.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/inline_response20010.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/inline_response20011.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/inline_response20011.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/inline_response20011_data.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/inline_response20011_data.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/inline_response20012.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/inline_response20012.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/inline_response20012_data.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/inline_response20012_data.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/inline_response20013.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/inline_response20013.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/inline_response20014.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/inline_response20014.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/inline_response2002.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/inline_response2002.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/inline_response2003.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/inline_response2003.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/inline_response2004.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/inline_response2004.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/inline_response2005.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/inline_response2005.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/inline_response2006.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/inline_response2006.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/inline_response2007.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/inline_response2007.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/inline_response2007_records.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/inline_response2007_records.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/inline_response2008.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/inline_response2008.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/inline_response2008_records.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/inline_response2008_records.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/inline_response2009.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/inline_response2009.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/inline_response2009_records.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/inline_response2009_records.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/list_id_members_body.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/list_id_members_body.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/list_id_members_body1.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/list_id_members_body1.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/list_id_subscribe_body.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/list_id_subscribe_body.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/list_id_subscribe_body1.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/list_id_subscribe_body1.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/list_list_id_body.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/list_list_id_body.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/list_subscribe_post_response_data.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/list_subscribe_post_response_data.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/list_subscribe_post_response_data_inner.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/list_subscribe_post_response_data_inner.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/measurement_count.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/measurement_count.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/measurement_sum.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/measurement_sum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/measurement_unique.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/measurement_unique.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/measurement_value.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/measurement_value.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/metric.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/metric.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/metric_export.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/metric_export.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/metric_export_data.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/metric_export_data.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/metric_export_metric.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/metric_export_metric.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/metric_export_results.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/metric_export_results.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/metric_integration.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/metric_integration.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/metric_timeline.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/metric_timeline.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/metric_timeline_data.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/metric_timeline_data.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/metric_timeline_event_properties.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/metric_timeline_event_properties.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/metric_timeline_person.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/metric_timeline_person.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/model200ok.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/model200ok.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/one_ofidentify_payload_properties_your_custom_field.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/one_ofidentify_payload_properties_your_custom_field.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/one_ofinline_response2006.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/one_ofinline_response2006.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/one_oftrack_payload_properties_your_custom_field.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/one_oftrack_payload_properties_your_custom_field.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/one_oftrack_payload_time.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/one_oftrack_payload_time.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/people_exchange_body.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/people_exchange_body.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/people_exclusions_body.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/people_exclusions_body.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/person.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/person.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/privacy_email.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/privacy_email.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/privacy_id.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/privacy_id.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/privacy_phone.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/privacy_phone.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/reason_bounced.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/reason_bounced.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/reason_invalid_email.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/reason_invalid_email.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/reason_manually_excluded.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/reason_manually_excluded.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/reason_reported_spam.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/reason_reported_spam.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/reason_unsubscribed.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/reason_unsubscribed.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/rendered_template.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/rendered_template.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/renderedtemplate_data.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/renderedtemplate_data.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/since_integer.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/since_integer.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/since_string.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/since_string.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/string_array.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/string_array.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/template.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/template.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/template_id_clone_body.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/template_id_clone_body.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/template_id_render_body.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/template_id_render_body.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/template_id_send_body.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/template_id_send_body.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/track_payload.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/track_payload.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/track_payload_customer_properties.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/track_payload_customer_properties.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/track_payload_post.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/track_payload_post.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/track_payload_properties.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/track_payload_properties.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/unit_day.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/unit_day.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/unit_month.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/unit_month.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/unit_week.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/unit_week.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/v1_campaigns_body.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/v1_campaigns_body.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/v1_emailtemplates_body.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/v1_emailtemplates_body.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/models/v2_lists_body.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/models/v2_lists_body.py`

 * *Files identical despite different names*

### Comparing `klaviyo-sdk-1.0.7.20220329/src/swagger_client/rest.py` & `klaviyo-sdk-1.0.8.20220329/src/swagger_client/rest.py`

 * *Files identical despite different names*

