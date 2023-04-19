# Comparing `tmp/asana-preview-1.0.2.tar.gz` & `tmp/asana-preview-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/python-asana-preview/python-asana-preview/dist/.tmp-y1is_qa7/asana-preview-1.0.2.tar", last modified: Fri Apr 14 18:45:39 2023, max compression
+gzip compressed data, was "/home/runner/work/python-asana-preview/python-asana-preview/dist/.tmp-nl2_yapc/asana-preview-1.0.3.tar", last modified: Wed Apr 19 21:12:58 2023, max compression
```

## Comparing `asana-preview-1.0.2.tar` & `asana-preview-1.0.3.tar`

### file list

```diff
@@ -1,228 +1,228 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:45:39.000000 asana-preview-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-14 18:45:30.000000 asana-preview-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-14 18:45:39.000000 asana-preview-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-04-14 18:45:30.000000 asana-preview-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:45:39.000000 asana-preview-1.0.2/asana_preview/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:45:39.000000 asana-preview-1.0.2/asana_preview/api/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/api/events_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    15631 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/api/projects_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8796 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/api/sections_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/api/stories_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    32576 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/api/tasks_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/api/users_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    39420 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:45:39.000000 asana-preview-1.0.2/asana_preview/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16486 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:45:39.000000 asana-preview-1.0.2/asana_preview/model/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14450 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/asana_named_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    11458 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/asana_named_resource_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    11846 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/asana_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    23974 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/custom_field_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15390 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/custom_field_base_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    19803 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/custom_field_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)    17203 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/custom_field_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/custom_field_compact_all_of_date_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    32959 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/custom_field_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    20265 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/custom_field_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    14345 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/custom_field_setting_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)    11645 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/custom_field_setting_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    16084 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/custom_field_setting_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12923 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/custom_field_setting_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    15102 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/enum_option.py
--rw-r--r--   0 runner    (1001) docker     (123)    12479 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/enum_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    11679 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13998 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/error_response5_xx.py
--rw-r--r--   0 runner    (1001) docker     (123)    11726 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/error_response5_xx_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/error_response5_xx_all_of_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    12041 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/error_response_errors_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    14117 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/event_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    15698 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/event_response_change.py
--rw-r--r--   0 runner    (1001) docker     (123)    14285 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/event_response_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)    14291 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/event_response_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    14395 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/event_response_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    12228 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/get_events200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    14094 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/get_events401_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/get_events401_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/get_events401_response_all_of_errors_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    14094 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/get_events403_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/get_events403_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/get_events403_response_all_of_errors_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    14094 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/get_events404_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/get_events404_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/get_events404_response_all_of_errors_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    14416 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/get_events412_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12124 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/get_events412_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/get_events412_response_all_of_errors_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/get_events500_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/get_events500_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/get_events500_response_all_of_errors_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/get_project200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11624 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/get_projects200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11964 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/get_sections_for_project200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/get_stories_for_task200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/get_task200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11934 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/get_tasks_for_project200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/get_user200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/like.py
--rw-r--r--   0 runner    (1001) docker     (123)    11723 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/next_page.py
--rw-r--r--   0 runner    (1001) docker     (123)    23004 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/project_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    19567 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/project_base_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    14296 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/project_brief_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)    11627 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/project_brief_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    14729 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/project_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)    12086 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/project_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    28963 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    17331 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/project_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    15562 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/project_status_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12762 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/project_status_base_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    14569 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/project_status_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)    11895 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/project_status_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/project_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12889 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/project_status_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    14560 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/project_template_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)    11876 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/project_template_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    14581 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/section_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/section_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    15589 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/status_update_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)    12920 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/status_update_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    16666 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/story_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)    14097 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/story_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    14689 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/tag_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/tag_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    22243 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/task_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    18242 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/task_base_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    11575 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/task_base_all_of_external.py
--rw-r--r--   0 runner    (1001) docker     (123)    15523 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/task_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)    12895 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/task_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    36129 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/task_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    25145 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/task_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/task_response_all_of_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/team_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/team_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    15264 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/user_base_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/user_base_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    12546 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/user_base_response_all_of_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)    14545 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/user_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)    11917 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/user_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    15982 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12001 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/user_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    14505 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/workspace_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)    11852 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model/workspace_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    82577 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:45:39.000000 asana-preview-1.0.2/asana_preview/models/
--rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14254 2023-04-14 18:45:30.000000 asana-preview-1.0.2/asana_preview/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:45:39.000000 asana-preview-1.0.2/asana_preview.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-14 18:45:39.000000 asana-preview-1.0.2/asana_preview.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8742 2023-04-14 18:45:39.000000 asana-preview-1.0.2/asana_preview.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:45:39.000000 asana-preview-1.0.2/asana_preview.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-14 18:45:39.000000 asana-preview-1.0.2/asana_preview.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-14 18:45:39.000000 asana-preview-1.0.2/asana_preview.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-14 18:45:39.000000 asana-preview-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-14 18:45:30.000000 asana-preview-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:45:39.000000 asana-preview-1.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_asana_named_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_asana_named_resource_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_asana_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_custom_field_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_custom_field_base_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_custom_field_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_custom_field_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_custom_field_compact_all_of_date_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_custom_field_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_custom_field_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_custom_field_setting_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_custom_field_setting_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_custom_field_setting_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_custom_field_setting_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_enum_option.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_enum_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_error_response5_xx.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_error_response5_xx_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_error_response5_xx_all_of_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_error_response_errors_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_event_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_event_response_change.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_event_response_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_event_response_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_event_response_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_events_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_get_events200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_get_events401_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_get_events401_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_get_events401_response_all_of_errors_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_get_events403_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_get_events403_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_get_events403_response_all_of_errors_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_get_events404_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_get_events404_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_get_events404_response_all_of_errors_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_get_events412_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_get_events412_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_get_events412_response_all_of_errors_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_get_events500_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_get_events500_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_get_events500_response_all_of_errors_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_get_project200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_get_projects200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_get_sections_for_project200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_get_stories_for_task200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_get_task200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_get_tasks_for_project200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_get_user200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_like.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_next_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_project_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_project_base_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_project_brief_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_project_brief_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_project_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_project_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_project_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_project_status_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_project_status_base_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_project_status_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_project_status_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_project_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_project_status_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_project_template_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_project_template_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_projects_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_section_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_section_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_sections_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_status_update_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_status_update_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_stories_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_story_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_story_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_tag_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_tag_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_task_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_task_base_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_task_base_all_of_external.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_task_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_task_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_task_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_task_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_task_response_all_of_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_tasks_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_team_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_team_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_user_base_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_user_base_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_user_base_response_all_of_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_user_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_user_compact_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_user_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_users_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_workspace_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-14 18:45:30.000000 asana-preview-1.0.2/test/test_workspace_compact_all_of.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:12:58.000000 asana-preview-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-19 21:12:49.000000 asana-preview-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-04-19 21:12:58.000000 asana-preview-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-04-19 21:12:49.000000 asana-preview-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:12:58.000000 asana-preview-1.0.3/asana_preview/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:12:58.000000 asana-preview-1.0.3/asana_preview/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/api/events_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15631 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/api/projects_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8796 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/api/sections_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/api/stories_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32576 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/api/tasks_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/api/users_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39420 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:12:58.000000 asana-preview-1.0.3/asana_preview/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16486 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:12:58.000000 asana-preview-1.0.3/asana_preview/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14450 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/asana_named_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11458 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/asana_named_resource_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11846 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/asana_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23974 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/custom_field_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15390 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/custom_field_base_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19803 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/custom_field_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17203 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/custom_field_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/custom_field_compact_all_of_date_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32959 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/custom_field_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20265 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/custom_field_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14345 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/custom_field_setting_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11645 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/custom_field_setting_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16084 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/custom_field_setting_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12923 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/custom_field_setting_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15102 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/enum_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12479 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/enum_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11679 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13998 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/error_response5_xx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11726 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/error_response5_xx_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/error_response5_xx_all_of_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12041 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/error_response_errors_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14117 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/event_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15698 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/event_response_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14285 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/event_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14291 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/event_response_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14395 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/event_response_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12228 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/get_events200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14094 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/get_events401_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/get_events401_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/get_events401_response_all_of_errors_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14094 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/get_events403_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/get_events403_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/get_events403_response_all_of_errors_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14094 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/get_events404_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/get_events404_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/get_events404_response_all_of_errors_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14416 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/get_events412_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12124 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/get_events412_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/get_events412_response_all_of_errors_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/get_events500_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/get_events500_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/get_events500_response_all_of_errors_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/get_project200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11624 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/get_projects200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11964 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/get_sections_for_project200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/get_stories_for_task200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/get_task200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11934 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/get_tasks_for_project200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/get_user200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/like.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11723 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/next_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23004 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/project_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19567 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/project_base_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14296 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/project_brief_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11627 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/project_brief_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14729 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/project_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12086 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/project_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28963 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17331 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/project_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15562 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/project_status_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12762 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/project_status_base_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14569 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/project_status_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11895 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/project_status_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/project_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12889 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/project_status_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14560 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/project_template_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11876 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/project_template_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14581 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/section_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/section_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15589 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/status_update_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12920 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/status_update_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16666 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/story_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14097 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/story_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14689 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/tag_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/tag_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22243 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/task_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18242 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/task_base_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11575 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/task_base_all_of_external.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15523 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/task_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12895 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/task_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36129 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/task_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25145 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/task_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/task_response_all_of_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/team_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/team_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15264 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/user_base_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/user_base_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12546 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/user_base_response_all_of_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14545 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/user_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11917 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/user_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15982 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12001 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/user_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14505 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/workspace_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11852 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model/workspace_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82577 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:12:58.000000 asana-preview-1.0.3/asana_preview/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14254 2023-04-19 21:12:49.000000 asana-preview-1.0.3/asana_preview/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:12:58.000000 asana-preview-1.0.3/asana_preview.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-04-19 21:12:58.000000 asana-preview-1.0.3/asana_preview.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8742 2023-04-19 21:12:58.000000 asana-preview-1.0.3/asana_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 21:12:58.000000 asana-preview-1.0.3/asana_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-19 21:12:58.000000 asana-preview-1.0.3/asana_preview.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-19 21:12:58.000000 asana-preview-1.0.3/asana_preview.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-19 21:12:58.000000 asana-preview-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-19 21:12:49.000000 asana-preview-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:12:58.000000 asana-preview-1.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_asana_named_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_asana_named_resource_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_asana_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_custom_field_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_custom_field_base_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_custom_field_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_custom_field_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_custom_field_compact_all_of_date_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_custom_field_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_custom_field_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_custom_field_setting_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_custom_field_setting_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_custom_field_setting_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_custom_field_setting_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_enum_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_enum_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_error_response5_xx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_error_response5_xx_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_error_response5_xx_all_of_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_error_response_errors_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_event_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_event_response_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_event_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_event_response_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_event_response_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_events_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_get_events200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_get_events401_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_get_events401_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_get_events401_response_all_of_errors_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_get_events403_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_get_events403_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_get_events403_response_all_of_errors_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_get_events404_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_get_events404_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_get_events404_response_all_of_errors_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_get_events412_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_get_events412_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_get_events412_response_all_of_errors_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_get_events500_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_get_events500_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_get_events500_response_all_of_errors_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_get_project200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_get_projects200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_get_sections_for_project200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_get_stories_for_task200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_get_task200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_get_tasks_for_project200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_get_user200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_like.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_next_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_project_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_project_base_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_project_brief_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_project_brief_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_project_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_project_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_project_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_project_status_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_project_status_base_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_project_status_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_project_status_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_project_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_project_status_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_project_template_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_project_template_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_projects_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_section_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_section_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_sections_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_status_update_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_status_update_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_stories_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_story_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_story_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_tag_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_tag_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_task_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_task_base_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_task_base_all_of_external.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_task_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_task_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_task_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_task_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_task_response_all_of_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_tasks_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_team_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_team_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_user_base_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_user_base_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_user_base_response_all_of_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_user_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_user_compact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_user_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_users_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_workspace_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-19 21:12:49.000000 asana-preview-1.0.3/test/test_workspace_compact_all_of.py
```

### Comparing `asana-preview-1.0.2/LICENSE` & `asana-preview-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/PKG-INFO` & `asana-preview-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: asana-preview
-Version: 1.0.2
+Version: 1.0.3
 Summary: Asana
 Home-page: 
 Author: Asana Support
 Author-email: team@openapitools.org
 License: Apache 2.0
 Keywords: OpenAPI,OpenAPI-Generator,Asana
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # asana-preview [![PyPi Version][pypi-image]][pypi-url]
-This is the interface for interacting with the Asana platform
 
-- Package version: 1.0.2
+This is a [preview version](https://forum.asana.com/t/try-an-early-preview-of-our-new-node-js-and-python-sdks/394881) of Asana's new python client library. For feedback and feature requests, please leave a comment on [this forum thread](https://forum.asana.com/t/try-an-early-preview-of-our-new-node-js-and-python-sdks/394881) or through [the feedback form on our documentation site](https://form-beta.asana.com/?k=C4sELCq6hAUsoWEY0kJwAA&d=15793206719)
+
+- Package version: 1.0.3
 
 ## Requirements.
 
 Python >=3.6
 
 ## Installation & Usage
 ### pip install
@@ -57,15 +58,15 @@
 
 # Configure Bearer authorization: personal_access_token
 configuration = asana_preview.Configuration(
     access_token = 'PERSONAL_ACCESS_TOKEN'
 )
 
 # Enter a context with an instance of the API client
-with asana.ApiClient(configuration) as api_client:
+with asana_preview.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = users_api.UsersApi(api_client)
     user_gid = "me" # str | A string identifying a user. This can either be the string "me", an email, or the gid of a user.
     opt_fields = ["email", "name", "workspaces"] # [str] | Defines fields to return.  Some requests return *compact* representations of objects in order to conserve resources and complete the request more efficiently. Other times requests return more information than you may need. This option allows you to list the exact set of fields that the API should be sure to return for the objects. The field names should be provided as paths, described below.  The gid of included objects will always be returned, regardless of the field options. (optional)
 
     # Example passing only required values
     try:
```

### Comparing `asana-preview-1.0.2/README.md` & `asana-preview-1.0.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # asana-preview [![PyPi Version][pypi-image]][pypi-url]
-This is the interface for interacting with the Asana platform
 
-- Package version: 1.0.2
+This is a [preview version](https://forum.asana.com/t/try-an-early-preview-of-our-new-node-js-and-python-sdks/394881) of Asana's new python client library. For feedback and feature requests, please leave a comment on [this forum thread](https://forum.asana.com/t/try-an-early-preview-of-our-new-node-js-and-python-sdks/394881) or through [the feedback form on our documentation site](https://form-beta.asana.com/?k=C4sELCq6hAUsoWEY0kJwAA&d=15793206719)
+
+- Package version: 1.0.3
 
 ## Requirements.
 
 Python >=3.6
 
 ## Installation & Usage
 ### pip install
@@ -44,15 +45,15 @@
 
 # Configure Bearer authorization: personal_access_token
 configuration = asana_preview.Configuration(
     access_token = 'PERSONAL_ACCESS_TOKEN'
 )
 
 # Enter a context with an instance of the API client
-with asana.ApiClient(configuration) as api_client:
+with asana_preview.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = users_api.UsersApi(api_client)
     user_gid = "me" # str | A string identifying a user. This can either be the string "me", an email, or the gid of a user.
     opt_fields = ["email", "name", "workspaces"] # [str] | Defines fields to return.  Some requests return *compact* representations of objects in order to conserve resources and complete the request more efficiently. Other times requests return more information than you may need. This option allows you to list the exact set of fields that the API should be sure to return for the objects. The field names should be provided as paths, described below.  The gid of included objects will always be returned, regardless of the field options. (optional)
 
     # Example passing only required values
     try:
```

### Comparing `asana-preview-1.0.2/asana_preview/__init__.py` & `asana-preview-1.0.3/asana_preview/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     This is the interface for interacting with the Asana platform  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "1.0.2"
+__version__ = "1.0.3"
 
 # import ApiClient
 from asana_preview.api_client import ApiClient
 
 # import Configuration
 from asana_preview.configuration import Configuration
```

### Comparing `asana-preview-1.0.2/asana_preview/api/events_api.py` & `asana-preview-1.0.3/asana_preview/api/events_api.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/api/projects_api.py` & `asana-preview-1.0.3/asana_preview/api/projects_api.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/api/sections_api.py` & `asana-preview-1.0.3/asana_preview/api/sections_api.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/api/stories_api.py` & `asana-preview-1.0.3/asana_preview/api/stories_api.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/api/tasks_api.py` & `asana-preview-1.0.3/asana_preview/api/tasks_api.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/api/users_api.py` & `asana-preview-1.0.3/asana_preview/api/users_api.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/api_client.py` & `asana-preview-1.0.3/asana_preview/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,20 +73,20 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.0.2/python'
+        self.user_agent = 'OpenAPI-Generator/1.0.3/python'
         # Add custom header
         self.default_headers['X-Asana-Client-Lib'] = urlencode(
             {
                 'language': 'PythonPreview',
-                'version': "1.0.2",
+                'version': "1.0.3",
                 'language_version': platform.python_version(),
                 'os': platform.system(),
                 'os_version': platform.release()
             }
         )
 
     def __enter__(self):
```

### Comparing `asana-preview-1.0.2/asana_preview/apis/__init__.py` & `asana-preview-1.0.3/asana_preview/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/configuration.py` & `asana-preview-1.0.3/asana_preview/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -384,15 +384,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.0\n"\
-               "SDK Package Version: 1.0.2".\
+               "SDK Package Version: 1.0.3".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `asana-preview-1.0.2/asana_preview/exceptions.py` & `asana-preview-1.0.3/asana_preview/exceptions.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/asana_named_resource.py` & `asana-preview-1.0.3/asana_preview/model/asana_named_resource.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/asana_named_resource_all_of.py` & `asana-preview-1.0.3/asana_preview/model/asana_named_resource_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/asana_resource.py` & `asana-preview-1.0.3/asana_preview/model/asana_resource.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/custom_field_base.py` & `asana-preview-1.0.3/asana_preview/model/custom_field_base.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/custom_field_base_all_of.py` & `asana-preview-1.0.3/asana_preview/model/custom_field_base_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/custom_field_compact.py` & `asana-preview-1.0.3/asana_preview/model/custom_field_compact.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/custom_field_compact_all_of.py` & `asana-preview-1.0.3/asana_preview/model/custom_field_compact_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/custom_field_compact_all_of_date_value.py` & `asana-preview-1.0.3/asana_preview/model/custom_field_compact_all_of_date_value.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/custom_field_response.py` & `asana-preview-1.0.3/asana_preview/model/custom_field_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/custom_field_response_all_of.py` & `asana-preview-1.0.3/asana_preview/model/custom_field_response_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/custom_field_setting_compact.py` & `asana-preview-1.0.3/asana_preview/model/custom_field_setting_compact.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/custom_field_setting_compact_all_of.py` & `asana-preview-1.0.3/asana_preview/model/custom_field_setting_compact_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/custom_field_setting_response.py` & `asana-preview-1.0.3/asana_preview/model/custom_field_setting_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/custom_field_setting_response_all_of.py` & `asana-preview-1.0.3/asana_preview/model/custom_field_setting_response_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/enum_option.py` & `asana-preview-1.0.3/asana_preview/model/enum_option.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/enum_option_all_of.py` & `asana-preview-1.0.3/asana_preview/model/enum_option_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/error_response.py` & `asana-preview-1.0.3/asana_preview/model/error_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/error_response5_xx.py` & `asana-preview-1.0.3/asana_preview/model/error_response5_xx.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/error_response5_xx_all_of.py` & `asana-preview-1.0.3/asana_preview/model/error_response5_xx_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/error_response5_xx_all_of_errors.py` & `asana-preview-1.0.3/asana_preview/model/error_response5_xx_all_of_errors.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/error_response_errors_inner.py` & `asana-preview-1.0.3/asana_preview/model/error_response_errors_inner.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/event_response.py` & `asana-preview-1.0.3/asana_preview/model/event_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/event_response_change.py` & `asana-preview-1.0.3/asana_preview/model/event_response_change.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/event_response_parent.py` & `asana-preview-1.0.3/asana_preview/model/event_response_parent.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/event_response_resource.py` & `asana-preview-1.0.3/asana_preview/model/event_response_resource.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/event_response_user.py` & `asana-preview-1.0.3/asana_preview/model/event_response_user.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/get_events200_response.py` & `asana-preview-1.0.3/asana_preview/model/get_events200_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/get_events401_response.py` & `asana-preview-1.0.3/asana_preview/model/get_events401_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/get_events401_response_all_of.py` & `asana-preview-1.0.3/asana_preview/model/get_events401_response_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/get_events401_response_all_of_errors_inner.py` & `asana-preview-1.0.3/asana_preview/model/get_events401_response_all_of_errors_inner.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/get_events403_response.py` & `asana-preview-1.0.3/asana_preview/model/get_events403_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/get_events403_response_all_of.py` & `asana-preview-1.0.3/asana_preview/model/get_events403_response_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/get_events403_response_all_of_errors_inner.py` & `asana-preview-1.0.3/asana_preview/model/get_events403_response_all_of_errors_inner.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/get_events404_response.py` & `asana-preview-1.0.3/asana_preview/model/get_events404_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/get_events404_response_all_of.py` & `asana-preview-1.0.3/asana_preview/model/get_events404_response_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/get_events404_response_all_of_errors_inner.py` & `asana-preview-1.0.3/asana_preview/model/get_events404_response_all_of_errors_inner.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/get_events412_response.py` & `asana-preview-1.0.3/asana_preview/model/get_events412_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/get_events412_response_all_of.py` & `asana-preview-1.0.3/asana_preview/model/get_events412_response_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/get_events412_response_all_of_errors_inner.py` & `asana-preview-1.0.3/asana_preview/model/get_events412_response_all_of_errors_inner.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/get_events500_response.py` & `asana-preview-1.0.3/asana_preview/model/get_events500_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/get_events500_response_all_of.py` & `asana-preview-1.0.3/asana_preview/model/get_events500_response_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/get_events500_response_all_of_errors_inner.py` & `asana-preview-1.0.3/asana_preview/model/get_events500_response_all_of_errors_inner.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/get_project200_response.py` & `asana-preview-1.0.3/asana_preview/model/get_project200_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/get_projects200_response.py` & `asana-preview-1.0.3/asana_preview/model/get_projects200_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/get_sections_for_project200_response.py` & `asana-preview-1.0.3/asana_preview/model/get_sections_for_project200_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/get_stories_for_task200_response.py` & `asana-preview-1.0.3/asana_preview/model/get_stories_for_task200_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/get_task200_response.py` & `asana-preview-1.0.3/asana_preview/model/get_task200_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/get_tasks_for_project200_response.py` & `asana-preview-1.0.3/asana_preview/model/get_tasks_for_project200_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/get_user200_response.py` & `asana-preview-1.0.3/asana_preview/model/get_user200_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/like.py` & `asana-preview-1.0.3/asana_preview/model/like.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/next_page.py` & `asana-preview-1.0.3/asana_preview/model/next_page.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/project_base.py` & `asana-preview-1.0.3/asana_preview/model/project_base.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/project_base_all_of.py` & `asana-preview-1.0.3/asana_preview/model/project_base_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/project_brief_compact.py` & `asana-preview-1.0.3/asana_preview/model/project_brief_compact.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/project_brief_compact_all_of.py` & `asana-preview-1.0.3/asana_preview/model/project_brief_compact_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/project_compact.py` & `asana-preview-1.0.3/asana_preview/model/project_compact.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/project_compact_all_of.py` & `asana-preview-1.0.3/asana_preview/model/project_compact_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/project_response.py` & `asana-preview-1.0.3/asana_preview/model/project_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/project_response_all_of.py` & `asana-preview-1.0.3/asana_preview/model/project_response_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/project_status_base.py` & `asana-preview-1.0.3/asana_preview/model/project_status_base.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/project_status_base_all_of.py` & `asana-preview-1.0.3/asana_preview/model/project_status_base_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/project_status_compact.py` & `asana-preview-1.0.3/asana_preview/model/project_status_compact.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/project_status_compact_all_of.py` & `asana-preview-1.0.3/asana_preview/model/project_status_compact_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/project_status_response.py` & `asana-preview-1.0.3/asana_preview/model/project_status_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/project_status_response_all_of.py` & `asana-preview-1.0.3/asana_preview/model/project_status_response_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/project_template_compact.py` & `asana-preview-1.0.3/asana_preview/model/project_template_compact.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/project_template_compact_all_of.py` & `asana-preview-1.0.3/asana_preview/model/project_template_compact_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/section_compact.py` & `asana-preview-1.0.3/asana_preview/model/section_compact.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/section_compact_all_of.py` & `asana-preview-1.0.3/asana_preview/model/section_compact_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/status_update_compact.py` & `asana-preview-1.0.3/asana_preview/model/status_update_compact.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/status_update_compact_all_of.py` & `asana-preview-1.0.3/asana_preview/model/status_update_compact_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/story_compact.py` & `asana-preview-1.0.3/asana_preview/model/story_compact.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/story_compact_all_of.py` & `asana-preview-1.0.3/asana_preview/model/story_compact_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/tag_compact.py` & `asana-preview-1.0.3/asana_preview/model/tag_compact.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/tag_compact_all_of.py` & `asana-preview-1.0.3/asana_preview/model/tag_compact_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/task_base.py` & `asana-preview-1.0.3/asana_preview/model/task_base.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/task_base_all_of.py` & `asana-preview-1.0.3/asana_preview/model/task_base_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/task_base_all_of_external.py` & `asana-preview-1.0.3/asana_preview/model/task_base_all_of_external.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/task_compact.py` & `asana-preview-1.0.3/asana_preview/model/task_compact.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/task_compact_all_of.py` & `asana-preview-1.0.3/asana_preview/model/task_compact_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/task_response.py` & `asana-preview-1.0.3/asana_preview/model/task_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/task_response_all_of.py` & `asana-preview-1.0.3/asana_preview/model/task_response_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/task_response_all_of_memberships.py` & `asana-preview-1.0.3/asana_preview/model/task_response_all_of_memberships.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/team_compact.py` & `asana-preview-1.0.3/asana_preview/model/team_compact.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/team_compact_all_of.py` & `asana-preview-1.0.3/asana_preview/model/team_compact_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/user_base_response.py` & `asana-preview-1.0.3/asana_preview/model/user_base_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/user_base_response_all_of.py` & `asana-preview-1.0.3/asana_preview/model/user_base_response_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/user_base_response_all_of_photo.py` & `asana-preview-1.0.3/asana_preview/model/user_base_response_all_of_photo.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/user_compact.py` & `asana-preview-1.0.3/asana_preview/model/user_compact.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/user_compact_all_of.py` & `asana-preview-1.0.3/asana_preview/model/user_compact_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/user_response.py` & `asana-preview-1.0.3/asana_preview/model/user_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/user_response_all_of.py` & `asana-preview-1.0.3/asana_preview/model/user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/workspace_compact.py` & `asana-preview-1.0.3/asana_preview/model/workspace_compact.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model/workspace_compact_all_of.py` & `asana-preview-1.0.3/asana_preview/model/workspace_compact_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/model_utils.py` & `asana-preview-1.0.3/asana_preview/model_utils.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/models/__init__.py` & `asana-preview-1.0.3/asana_preview/models/__init__.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview/rest.py` & `asana-preview-1.0.3/asana_preview/rest.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/asana_preview.egg-info/PKG-INFO` & `asana-preview-1.0.3/asana_preview.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: asana-preview
-Version: 1.0.2
+Version: 1.0.3
 Summary: Asana
 Home-page: 
 Author: Asana Support
 Author-email: team@openapitools.org
 License: Apache 2.0
 Keywords: OpenAPI,OpenAPI-Generator,Asana
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # asana-preview [![PyPi Version][pypi-image]][pypi-url]
-This is the interface for interacting with the Asana platform
 
-- Package version: 1.0.2
+This is a [preview version](https://forum.asana.com/t/try-an-early-preview-of-our-new-node-js-and-python-sdks/394881) of Asana's new python client library. For feedback and feature requests, please leave a comment on [this forum thread](https://forum.asana.com/t/try-an-early-preview-of-our-new-node-js-and-python-sdks/394881) or through [the feedback form on our documentation site](https://form-beta.asana.com/?k=C4sELCq6hAUsoWEY0kJwAA&d=15793206719)
+
+- Package version: 1.0.3
 
 ## Requirements.
 
 Python >=3.6
 
 ## Installation & Usage
 ### pip install
@@ -57,15 +58,15 @@
 
 # Configure Bearer authorization: personal_access_token
 configuration = asana_preview.Configuration(
     access_token = 'PERSONAL_ACCESS_TOKEN'
 )
 
 # Enter a context with an instance of the API client
-with asana.ApiClient(configuration) as api_client:
+with asana_preview.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = users_api.UsersApi(api_client)
     user_gid = "me" # str | A string identifying a user. This can either be the string "me", an email, or the gid of a user.
     opt_fields = ["email", "name", "workspaces"] # [str] | Defines fields to return.  Some requests return *compact* representations of objects in order to conserve resources and complete the request more efficiently. Other times requests return more information than you may need. This option allows you to list the exact set of fields that the API should be sure to return for the objects. The field names should be provided as paths, described below.  The gid of included objects will always be returned, regardless of the field options. (optional)
 
     # Example passing only required values
     try:
```

### Comparing `asana-preview-1.0.2/asana_preview.egg-info/SOURCES.txt` & `asana-preview-1.0.3/asana_preview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/setup.py` & `asana-preview-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 
 
 import os
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "asana-preview"
-VERSION = "1.0.2"
+VERSION = "1.0.3"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `asana-preview-1.0.2/test/test_asana_named_resource.py` & `asana-preview-1.0.3/test/test_asana_named_resource.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_asana_named_resource_all_of.py` & `asana-preview-1.0.3/test/test_asana_named_resource_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_asana_resource.py` & `asana-preview-1.0.3/test/test_asana_resource.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_custom_field_base.py` & `asana-preview-1.0.3/test/test_custom_field_base.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_custom_field_base_all_of.py` & `asana-preview-1.0.3/test/test_custom_field_base_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_custom_field_compact.py` & `asana-preview-1.0.3/test/test_custom_field_compact.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_custom_field_compact_all_of.py` & `asana-preview-1.0.3/test/test_custom_field_compact_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_custom_field_compact_all_of_date_value.py` & `asana-preview-1.0.3/test/test_custom_field_compact_all_of_date_value.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_custom_field_response.py` & `asana-preview-1.0.3/test/test_custom_field_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_custom_field_response_all_of.py` & `asana-preview-1.0.3/test/test_custom_field_response_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_custom_field_setting_compact.py` & `asana-preview-1.0.3/test/test_custom_field_setting_compact.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_custom_field_setting_compact_all_of.py` & `asana-preview-1.0.3/test/test_custom_field_setting_compact_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_custom_field_setting_response.py` & `asana-preview-1.0.3/test/test_custom_field_setting_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_custom_field_setting_response_all_of.py` & `asana-preview-1.0.3/test/test_custom_field_setting_response_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_enum_option.py` & `asana-preview-1.0.3/test/test_enum_option.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_enum_option_all_of.py` & `asana-preview-1.0.3/test/test_enum_option_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_error_response.py` & `asana-preview-1.0.3/test/test_error_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_error_response5_xx.py` & `asana-preview-1.0.3/test/test_error_response5_xx.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_error_response5_xx_all_of.py` & `asana-preview-1.0.3/test/test_error_response5_xx_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_error_response5_xx_all_of_errors.py` & `asana-preview-1.0.3/test/test_error_response5_xx_all_of_errors.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_error_response_errors_inner.py` & `asana-preview-1.0.3/test/test_error_response_errors_inner.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_event_response.py` & `asana-preview-1.0.3/test/test_event_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_event_response_change.py` & `asana-preview-1.0.3/test/test_event_response_change.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_event_response_parent.py` & `asana-preview-1.0.3/test/test_event_response_parent.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_event_response_resource.py` & `asana-preview-1.0.3/test/test_event_response_resource.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_event_response_user.py` & `asana-preview-1.0.3/test/test_event_response_user.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_events_api.py` & `asana-preview-1.0.3/test/test_events_api.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_get_events200_response.py` & `asana-preview-1.0.3/test/test_get_events200_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_get_events401_response.py` & `asana-preview-1.0.3/test/test_get_events401_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_get_events401_response_all_of.py` & `asana-preview-1.0.3/test/test_get_events401_response_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_get_events401_response_all_of_errors_inner.py` & `asana-preview-1.0.3/test/test_get_events401_response_all_of_errors_inner.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_get_events403_response.py` & `asana-preview-1.0.3/test/test_get_events403_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_get_events403_response_all_of.py` & `asana-preview-1.0.3/test/test_get_events403_response_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_get_events403_response_all_of_errors_inner.py` & `asana-preview-1.0.3/test/test_get_events403_response_all_of_errors_inner.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_get_events404_response.py` & `asana-preview-1.0.3/test/test_get_events404_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_get_events404_response_all_of.py` & `asana-preview-1.0.3/test/test_get_events404_response_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_get_events404_response_all_of_errors_inner.py` & `asana-preview-1.0.3/test/test_get_events404_response_all_of_errors_inner.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_get_events412_response.py` & `asana-preview-1.0.3/test/test_get_events412_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_get_events412_response_all_of.py` & `asana-preview-1.0.3/test/test_get_events412_response_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_get_events412_response_all_of_errors_inner.py` & `asana-preview-1.0.3/test/test_get_events412_response_all_of_errors_inner.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_get_events500_response.py` & `asana-preview-1.0.3/test/test_get_events500_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_get_events500_response_all_of.py` & `asana-preview-1.0.3/test/test_get_events500_response_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_get_events500_response_all_of_errors_inner.py` & `asana-preview-1.0.3/test/test_get_events500_response_all_of_errors_inner.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_get_project200_response.py` & `asana-preview-1.0.3/test/test_get_project200_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_get_projects200_response.py` & `asana-preview-1.0.3/test/test_get_projects200_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_get_sections_for_project200_response.py` & `asana-preview-1.0.3/test/test_get_sections_for_project200_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_get_stories_for_task200_response.py` & `asana-preview-1.0.3/test/test_get_stories_for_task200_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_get_task200_response.py` & `asana-preview-1.0.3/test/test_get_task200_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_get_tasks_for_project200_response.py` & `asana-preview-1.0.3/test/test_get_tasks_for_project200_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_get_user200_response.py` & `asana-preview-1.0.3/test/test_get_user200_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_like.py` & `asana-preview-1.0.3/test/test_like.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_next_page.py` & `asana-preview-1.0.3/test/test_next_page.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_project_base.py` & `asana-preview-1.0.3/test/test_project_base.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_project_base_all_of.py` & `asana-preview-1.0.3/test/test_project_base_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_project_brief_compact.py` & `asana-preview-1.0.3/test/test_project_brief_compact.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_project_brief_compact_all_of.py` & `asana-preview-1.0.3/test/test_project_brief_compact_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_project_compact.py` & `asana-preview-1.0.3/test/test_project_compact.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_project_compact_all_of.py` & `asana-preview-1.0.3/test/test_project_compact_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_project_response.py` & `asana-preview-1.0.3/test/test_project_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_project_response_all_of.py` & `asana-preview-1.0.3/test/test_project_response_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_project_status_base.py` & `asana-preview-1.0.3/test/test_project_status_base.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_project_status_base_all_of.py` & `asana-preview-1.0.3/test/test_project_status_base_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_project_status_compact.py` & `asana-preview-1.0.3/test/test_project_status_compact.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_project_status_compact_all_of.py` & `asana-preview-1.0.3/test/test_project_status_compact_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_project_status_response.py` & `asana-preview-1.0.3/test/test_project_status_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_project_status_response_all_of.py` & `asana-preview-1.0.3/test/test_project_status_response_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_project_template_compact.py` & `asana-preview-1.0.3/test/test_project_template_compact.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_project_template_compact_all_of.py` & `asana-preview-1.0.3/test/test_project_template_compact_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_projects_api.py` & `asana-preview-1.0.3/test/test_projects_api.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_section_compact.py` & `asana-preview-1.0.3/test/test_section_compact.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_section_compact_all_of.py` & `asana-preview-1.0.3/test/test_section_compact_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_sections_api.py` & `asana-preview-1.0.3/test/test_sections_api.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_status_update_compact.py` & `asana-preview-1.0.3/test/test_status_update_compact.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_status_update_compact_all_of.py` & `asana-preview-1.0.3/test/test_status_update_compact_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_stories_api.py` & `asana-preview-1.0.3/test/test_stories_api.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_story_compact.py` & `asana-preview-1.0.3/test/test_story_compact.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_story_compact_all_of.py` & `asana-preview-1.0.3/test/test_story_compact_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_tag_compact.py` & `asana-preview-1.0.3/test/test_tag_compact.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_tag_compact_all_of.py` & `asana-preview-1.0.3/test/test_tag_compact_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_task_base.py` & `asana-preview-1.0.3/test/test_task_base.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_task_base_all_of.py` & `asana-preview-1.0.3/test/test_task_base_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_task_base_all_of_external.py` & `asana-preview-1.0.3/test/test_task_base_all_of_external.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_task_compact.py` & `asana-preview-1.0.3/test/test_task_compact.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_task_compact_all_of.py` & `asana-preview-1.0.3/test/test_task_compact_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_task_response.py` & `asana-preview-1.0.3/test/test_task_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_task_response_all_of.py` & `asana-preview-1.0.3/test/test_task_response_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_task_response_all_of_memberships.py` & `asana-preview-1.0.3/test/test_task_response_all_of_memberships.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_tasks_api.py` & `asana-preview-1.0.3/test/test_tasks_api.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_team_compact.py` & `asana-preview-1.0.3/test/test_team_compact.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_team_compact_all_of.py` & `asana-preview-1.0.3/test/test_team_compact_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_user_base_response.py` & `asana-preview-1.0.3/test/test_user_base_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_user_base_response_all_of.py` & `asana-preview-1.0.3/test/test_user_base_response_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_user_base_response_all_of_photo.py` & `asana-preview-1.0.3/test/test_user_base_response_all_of_photo.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_user_compact.py` & `asana-preview-1.0.3/test/test_user_compact.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_user_compact_all_of.py` & `asana-preview-1.0.3/test/test_user_compact_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_user_response.py` & `asana-preview-1.0.3/test/test_user_response.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_user_response_all_of.py` & `asana-preview-1.0.3/test/test_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_users_api.py` & `asana-preview-1.0.3/test/test_users_api.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_workspace_compact.py` & `asana-preview-1.0.3/test/test_workspace_compact.py`

 * *Files identical despite different names*

### Comparing `asana-preview-1.0.2/test/test_workspace_compact_all_of.py` & `asana-preview-1.0.3/test/test_workspace_compact_all_of.py`

 * *Files identical despite different names*

