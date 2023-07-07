# Comparing `tmp/asana_preview-1.0.7.tar.gz` & `tmp/asana_preview-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/python-asana-preview/python-asana-preview/dist/.tmp-97cjs_vj/asana_preview-1.0.7.tar", last modified: Mon Jul  3 19:39:53 2023, max compression
+gzip compressed data, was "/home/runner/work/python-asana-preview/python-asana-preview/dist/.tmp-sj92c_xp/asana_preview-1.0.8.tar", last modified: Fri Jul  7 20:43:04 2023, max compression
```

## Comparing `asana_preview-1.0.7.tar` & `asana_preview-1.0.8.tar`

### file list

```diff
@@ -1,914 +1,918 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:39:53.000000 asana_preview-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-03 19:39:53.000000 asana_preview-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    59290 2023-07-03 19:39:44.000000 asana_preview-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:39:53.000000 asana_preview-1.0.7/asana_preview/
--rw-r--r--   0 runner    (1001) docker     (123)    36136 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:39:53.000000 asana_preview-1.0.7/asana_preview/api/
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23646 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/api/attachments_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12527 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/api/audit_log_api_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/api/batch_api_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13741 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/api/custom_field_settings_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    45245 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/api/custom_fields_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/api/events_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27360 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/api/goal_relationships_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    52947 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/api/goals_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/api/jobs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18699 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/api/memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/api/organization_exports_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18543 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/api/portfolio_memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    63752 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/api/portfolios_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    20933 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/api/project_briefs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/api/project_memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21913 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/api/project_statuses_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    28293 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/api/project_templates_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   107816 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/api/projects_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/api/rules_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    35837 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/api/sections_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21760 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/api/status_updates_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27300 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/api/stories_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    45876 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/api/tags_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   163541 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/api/tasks_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    24353 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/api/team_memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    40712 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/api/teams_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11681 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/api/time_periods_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    28130 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/api/time_tracking_entries_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11675 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/api/typeahead_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/api/user_task_lists_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    28905 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/api/users_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29484 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/api/webhooks_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18371 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/api/workspace_memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27463 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/api/workspaces_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25183 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:39:53.000000 asana_preview-1.0.7/asana_preview/models/
--rw-r--r--   0 runner    (1001) docker     (123)    33879 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/add_custom_field_setting_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/add_followers_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/add_members_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/all_of_project_response_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/all_of_project_template_base_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/all_of_project_template_response_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/all_of_story_response_new_date_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/all_of_story_response_old_date_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/all_of_task_response_assignee_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/all_of_user_task_list_base_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/all_of_user_task_list_base_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/all_of_user_task_list_compact_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/all_of_user_task_list_compact_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/all_of_user_task_list_request_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/all_of_user_task_list_request_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/all_of_user_task_list_response_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/all_of_user_task_list_response_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/all_of_workspace_membership_response_user_task_list_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/all_of_workspace_membership_response_user_task_list_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/asana_named_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/asana_named_resource_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/asana_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/attachment_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/attachment_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/attachment_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    14064 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/attachment_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/attachment_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/attachment_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/attachment_response_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     8729 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/audit_log_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/audit_log_event_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/audit_log_event_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     8838 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/audit_log_event_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/audit_log_event_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/audit_log_event_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/batch_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/batch_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/batch_request_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/batch_request_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/batch_request_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/batch_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/batch_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/create_membership_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/create_time_tracking_entry_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    30420 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/custom_field_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/custom_field_base_date_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/custom_field_base_enum_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/custom_field_base_enum_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    16739 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/custom_field_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/custom_field_gid_enum_options_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    34312 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/custom_field_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    33924 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/custom_field_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/custom_field_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/custom_field_response_created_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/custom_field_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/custom_field_response_people_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/custom_field_setting_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/custom_field_setting_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/custom_field_setting_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/custom_field_setting_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    35868 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/custom_field_setting_response_custom_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/custom_field_setting_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/custom_field_setting_response_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/custom_field_setting_response_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/custom_fields_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/custom_fields_custom_field_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/date_variable_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/date_variable_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/empty_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/empty_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/enum_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/enum_option_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/enum_option_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/enum_option_insert_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     8757 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/enum_option_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/enum_options_enum_option_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/enum_options_insert_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/error_response_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7955 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/event_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/event_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     9221 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/event_response_change.py
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/event_response_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/event_response_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/event_response_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goal_add_subgoal_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goal_add_supporting_relationship_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goal_add_supporting_work_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goal_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goal_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goal_gid_add_followers_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goal_gid_add_supporting_relationship_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goal_gid_remove_followers_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goal_gid_remove_supporting_relationship_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goal_gid_set_metric_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goal_gid_set_metric_current_value_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goal_membership_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goal_membership_base_goal.py
--rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goal_membership_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goal_membership_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    15542 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goal_metric_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goal_metric_current_value_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    15686 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goal_metric_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goal_relationship_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goal_relationship_base_supported_goal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goal_relationship_base_supporting_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8105 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goal_relationship_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goal_relationship_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goal_relationship_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goal_relationship_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goal_relationship_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goal_relationships_goal_relationship_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goal_remove_subgoal_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goal_remove_supporting_relationship_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    14351 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goal_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    13884 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goal_request_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    18927 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goal_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goal_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goal_response_current_status_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goal_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goal_response_likes.py
--rw-r--r--   0 runner    (1001) docker     (123)    17038 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goal_response_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goal_response_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goal_response_time_period.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goal_response_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    15329 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goal_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goals_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/goals_goal_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/job_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/job_base_new_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/job_base_new_project_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/job_base_new_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/job_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     8940 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/job_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/job_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/like.py
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/member_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/membership_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/membership_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/membership_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/membership_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/memberships_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/memberships_membership_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/message_base_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/modify_dependencies_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/modify_dependents_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     8622 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/organization_export_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8706 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/organization_export_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/organization_export_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     8734 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/organization_export_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/organization_export_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/organization_exports_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/portfolio_add_item_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/portfolio_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/portfolio_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/portfolio_gid_add_custom_field_setting_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/portfolio_gid_add_item_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/portfolio_gid_add_members_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/portfolio_gid_remove_custom_field_setting_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/portfolio_gid_remove_item_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/portfolio_gid_remove_members_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/portfolio_membership_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/portfolio_membership_base_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/portfolio_membership_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/portfolio_membership_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/portfolio_membership_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/portfolio_membership_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/portfolio_remove_item_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/portfolio_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    18230 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/portfolio_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/portfolio_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/portfolio_response_current_status_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/portfolio_response_custom_field_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    17399 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/portfolio_response_custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/portfolio_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/portfolio_response_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/portfolios_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/portfolios_portfolio_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/preview.py
--rw-r--r--   0 runner    (1001) docker     (123)    20495 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11697 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_base_current_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_base_current_status_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_base_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_brief_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_brief_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_brief_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_brief_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_brief_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_brief_response_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_briefs_project_brief_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_duplicate_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_duplicate_request_schedule_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_gid_add_custom_field_setting_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_gid_add_followers_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_gid_add_members_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_gid_duplicate_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_gid_project_briefs_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_gid_project_statuses_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_gid_remove_custom_field_setting_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_gid_remove_followers_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_gid_remove_members_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_gid_save_as_template_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_gid_sections_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_membership_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_membership_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_membership_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_membership_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_membership_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_membership_response_member.py
--rw-r--r--   0 runner    (1001) docker     (123)    24286 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    31095 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_response_completed_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_response_created_from_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_response_project_brief.py
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_response_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_save_as_template_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_section_insert_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7805 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_status_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_status_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_status_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11565 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_status_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_status_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    12987 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_template_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_template_base_requested_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_template_base_requested_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_template_base_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_template_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_template_gid_instantiate_project_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     9448 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_template_instantiate_project_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_template_instantiate_project_request_requested_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_template_instantiate_project_request_requested_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_template_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_template_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/project_template_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/projects_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/projects_project_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/remove_custom_field_setting_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/remove_followers_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/remove_members_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/requested_role_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/rule_trigger_gid_run_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/rule_trigger_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/rule_trigger_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/rule_trigger_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/section_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/section_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/section_gid_add_task_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/section_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7358 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/section_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/section_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/section_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/section_task_insert_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/sections_insert_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/sections_section_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     9879 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/status_update_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/status_update_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)    10929 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/status_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    19665 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/status_update_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/status_update_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/status_update_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/status_update_response_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/status_updates_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/stories_story_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/story_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/story_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/story_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    48927 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/story_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/story_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/story_response_assignee.py
--rw-r--r--   0 runner    (1001) docker     (123)    17099 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/story_response_custom_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/story_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/story_response_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/story_response_old_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/story_response_old_enum_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/story_response_old_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/story_response_previews.py
--rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/story_response_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/story_response_story.py
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/story_response_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/story_response_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/story_response_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/tag_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/tag_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/tag_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/tag_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/tag_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/tag_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/tags_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/task_add_followers_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/task_add_project_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/task_add_tag_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    35097 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/task_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/task_base_completed_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/task_base_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/task_base_external.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/task_base_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/task_base_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     6613 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/task_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/task_count_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/task_count_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/task_duplicate_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/task_gid_add_dependencies_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/task_gid_add_dependents_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/task_gid_add_followers_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/task_gid_add_project_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/task_gid_add_tag_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/task_gid_duplicate_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/task_gid_remove_dependencies_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/task_gid_remove_dependents_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/task_gid_remove_followers_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/task_gid_remove_project_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/task_gid_remove_tag_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/task_gid_set_parent_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/task_gid_stories_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/task_gid_subtasks_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/task_gid_time_tracking_entries_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/task_remove_followers_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/task_remove_project_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/task_remove_tag_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    43510 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/task_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    44580 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/task_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/task_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    34464 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/task_response_custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/task_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/task_response_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/task_response_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/task_response_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/task_set_parent_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/tasks_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/tasks_task_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/team_add_user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/team_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/team_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/team_gid_add_user_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/team_gid_projects_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/team_gid_remove_user_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/team_membership_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/team_membership_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/team_membership_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/team_membership_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/team_membership_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/team_remove_user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    19673 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/team_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    20553 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/team_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/team_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/team_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/team_response_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/teams_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/teams_body1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/template_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/time_period_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/time_period_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/time_period_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/time_period_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/time_period_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/time_tracking_entries_time_tracking_entry_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/time_tracking_entry_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/time_tracking_entry_base_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/time_tracking_entry_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/time_tracking_entry_compact_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/update_time_tracking_entry_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/user_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/user_base_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/user_base_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/user_base_response_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/user_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/user_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/user_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/user_task_list_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/user_task_list_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/user_task_list_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/user_task_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/user_task_list_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/webhook_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/webhook_compact_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/webhook_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/webhook_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/webhook_request_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    11774 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/webhook_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/webhook_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/webhook_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/webhook_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/webhooks_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/webhooks_webhook_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/workspace_add_user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/workspace_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/workspace_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/workspace_gid_add_user_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/workspace_gid_projects_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/workspace_gid_remove_user_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/workspace_gid_tags_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/workspace_membership_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/workspace_membership_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/workspace_membership_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/workspace_membership_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/workspace_membership_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/workspace_membership_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/workspace_membership_response_user_task_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/workspace_membership_response_vacation_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/workspace_remove_user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/workspace_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/workspace_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/workspace_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/models/workspaces_workspace_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    13139 2023-07-03 19:39:44.000000 asana_preview-1.0.7/asana_preview/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:39:53.000000 asana_preview-1.0.7/asana_preview.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-03 19:39:53.000000 asana_preview-1.0.7/asana_preview.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    38839 2023-07-03 19:39:53.000000 asana_preview-1.0.7/asana_preview.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:39:53.000000 asana_preview-1.0.7/asana_preview.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-03 19:39:53.000000 asana_preview-1.0.7/asana_preview.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-03 19:39:53.000000 asana_preview-1.0.7/asana_preview.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:39:53.000000 asana_preview-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-03 19:39:44.000000 asana_preview-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:39:53.000000 asana_preview-1.0.7/test/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_add_custom_field_setting_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_add_followers_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_add_members_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_all_of_project_response_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_all_of_project_template_base_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_all_of_project_template_response_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_all_of_story_response_new_date_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_all_of_story_response_old_date_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_all_of_task_response_assignee_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_all_of_user_task_list_base_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_all_of_user_task_list_base_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_all_of_user_task_list_compact_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_all_of_user_task_list_compact_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_all_of_user_task_list_request_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_all_of_user_task_list_request_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_all_of_user_task_list_response_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_all_of_user_task_list_response_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_all_of_workspace_membership_response_user_task_list_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_all_of_workspace_membership_response_user_task_list_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_asana_named_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_asana_named_resource_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_asana_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_attachment_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_attachment_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_attachment_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_attachment_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_attachment_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_attachment_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_attachment_response_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_attachments_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_audit_log_api_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_audit_log_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_audit_log_event_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_audit_log_event_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_audit_log_event_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_audit_log_event_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_audit_log_event_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_batch_api_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_batch_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_batch_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_batch_request_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_batch_request_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_batch_request_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_batch_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_batch_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_create_membership_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_create_time_tracking_entry_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_custom_field_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_custom_field_base_date_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_custom_field_base_enum_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_custom_field_base_enum_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_custom_field_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_custom_field_gid_enum_options_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_custom_field_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_custom_field_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_custom_field_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_custom_field_response_created_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_custom_field_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_custom_field_response_people_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_custom_field_setting_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_custom_field_setting_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_custom_field_setting_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_custom_field_setting_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_custom_field_setting_response_custom_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_custom_field_setting_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_custom_field_setting_response_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_custom_field_setting_response_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_custom_field_settings_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_custom_fields_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_custom_fields_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_custom_fields_custom_field_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_date_variable_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_date_variable_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_empty_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_empty_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_enum_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_enum_option_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_enum_option_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_enum_option_insert_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_enum_option_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_enum_options_enum_option_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_enum_options_insert_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_error_response_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_event_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_event_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_event_response_change.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_event_response_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_event_response_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_event_response_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_events_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goal_add_subgoal_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goal_add_supporting_relationship_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goal_add_supporting_work_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goal_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goal_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goal_gid_add_followers_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goal_gid_add_supporting_relationship_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goal_gid_remove_followers_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goal_gid_remove_supporting_relationship_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goal_gid_set_metric_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goal_gid_set_metric_current_value_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goal_membership_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goal_membership_base_goal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goal_membership_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goal_membership_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goal_metric_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goal_metric_current_value_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goal_metric_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goal_relationship_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goal_relationship_base_supported_goal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goal_relationship_base_supporting_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goal_relationship_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goal_relationship_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goal_relationship_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goal_relationship_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goal_relationship_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goal_relationships_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goal_relationships_goal_relationship_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goal_remove_subgoal_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goal_remove_supporting_relationship_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goal_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goal_request_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goal_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goal_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goal_response_current_status_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goal_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goal_response_likes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goal_response_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goal_response_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goal_response_time_period.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goal_response_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goal_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goals_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goals_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_goals_goal_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_job_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_job_base_new_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_job_base_new_project_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_job_base_new_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_job_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_job_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_job_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_jobs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_like.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_member_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_membership_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_membership_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_membership_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_membership_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_memberships_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_memberships_membership_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_message_base_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_modify_dependencies_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_modify_dependents_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_organization_export_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_organization_export_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_organization_export_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_organization_export_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_organization_export_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_organization_exports_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_organization_exports_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_portfolio_add_item_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_portfolio_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_portfolio_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_portfolio_gid_add_custom_field_setting_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_portfolio_gid_add_item_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_portfolio_gid_add_members_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_portfolio_gid_remove_custom_field_setting_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_portfolio_gid_remove_item_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_portfolio_gid_remove_members_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_portfolio_membership_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_portfolio_membership_base_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_portfolio_membership_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_portfolio_membership_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_portfolio_membership_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_portfolio_membership_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_portfolio_memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_portfolio_remove_item_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_portfolio_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_portfolio_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_portfolio_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_portfolio_response_current_status_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_portfolio_response_custom_field_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_portfolio_response_custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_portfolio_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_portfolio_response_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_portfolios_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_portfolios_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_portfolios_portfolio_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_base_current_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_base_current_status_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_base_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_brief_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_brief_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_brief_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_brief_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_brief_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_brief_response_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_briefs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_briefs_project_brief_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_duplicate_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_duplicate_request_schedule_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_gid_add_custom_field_setting_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_gid_add_followers_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_gid_add_members_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_gid_duplicate_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_gid_project_briefs_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_gid_project_statuses_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_gid_remove_custom_field_setting_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_gid_remove_followers_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_gid_remove_members_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_gid_save_as_template_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_gid_sections_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_membership_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_membership_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_membership_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_membership_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_membership_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_membership_response_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_response_completed_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_response_created_from_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_response_project_brief.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_response_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_save_as_template_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_section_insert_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_status_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_status_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_status_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_status_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_status_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_statuses_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_template_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_template_base_requested_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_template_base_requested_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_template_base_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_template_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_template_gid_instantiate_project_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_template_instantiate_project_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_template_instantiate_project_request_requested_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_template_instantiate_project_request_requested_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_template_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_template_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_template_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_project_templates_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_projects_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_projects_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_projects_project_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_remove_custom_field_setting_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_remove_followers_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_remove_members_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_requested_role_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_rule_trigger_gid_run_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_rule_trigger_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_rule_trigger_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_rule_trigger_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_rules_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_section_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_section_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_section_gid_add_task_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_section_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_section_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_section_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_section_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_section_task_insert_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_sections_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_sections_insert_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_sections_section_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_status_update_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_status_update_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_status_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_status_update_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_status_update_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_status_update_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_status_update_response_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_status_updates_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_status_updates_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_stories_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_stories_story_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_story_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_story_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_story_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_story_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_story_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_story_response_assignee.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_story_response_custom_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_story_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_story_response_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_story_response_old_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_story_response_old_enum_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_story_response_old_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_story_response_previews.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_story_response_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_story_response_story.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_story_response_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_story_response_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_story_response_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_tag_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_tag_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_tag_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_tag_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_tag_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_tags_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_tags_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_task_add_followers_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_task_add_project_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_task_add_tag_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_task_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_task_base_completed_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_task_base_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_task_base_external.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_task_base_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_task_base_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_task_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_task_count_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_task_count_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_task_duplicate_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_task_gid_add_dependencies_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_task_gid_add_dependents_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_task_gid_add_followers_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_task_gid_add_project_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_task_gid_add_tag_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_task_gid_duplicate_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_task_gid_remove_dependencies_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_task_gid_remove_dependents_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_task_gid_remove_followers_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_task_gid_remove_project_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_task_gid_remove_tag_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_task_gid_set_parent_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_task_gid_stories_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_task_gid_subtasks_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_task_gid_time_tracking_entries_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_task_remove_followers_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_task_remove_project_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_task_remove_tag_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_task_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_task_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_task_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_task_response_custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_task_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_task_response_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_task_response_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_task_response_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_task_set_parent_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_tasks_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_tasks_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_tasks_task_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_team_add_user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_team_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_team_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_team_gid_add_user_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_team_gid_projects_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_team_gid_remove_user_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_team_membership_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_team_membership_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_team_membership_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_team_membership_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_team_membership_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_team_memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_team_remove_user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_team_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_team_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_team_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_team_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_team_response_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_teams_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_teams_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_teams_body1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_template_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_time_period_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_time_period_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_time_period_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_time_period_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_time_period_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_time_periods_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_time_tracking_entries_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_time_tracking_entries_time_tracking_entry_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_time_tracking_entry_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_time_tracking_entry_base_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_time_tracking_entry_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_time_tracking_entry_compact_array.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_typeahead_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_update_time_tracking_entry_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_user_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_user_base_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_user_base_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_user_base_response_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_user_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_user_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_user_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_user_task_list_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_user_task_list_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_user_task_list_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_user_task_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_user_task_list_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_user_task_lists_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_users_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_webhook_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_webhook_compact_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_webhook_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_webhook_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_webhook_request_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_webhook_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_webhook_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_webhook_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_webhook_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_webhooks_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_webhooks_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_webhooks_webhook_gid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_workspace_add_user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_workspace_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_workspace_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_workspace_gid_add_user_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_workspace_gid_projects_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_workspace_gid_remove_user_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_workspace_gid_tags_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_workspace_membership_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_workspace_membership_compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_workspace_membership_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_workspace_membership_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_workspace_membership_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_workspace_membership_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_workspace_membership_response_user_task_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_workspace_membership_response_vacation_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_workspace_memberships_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_workspace_remove_user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_workspace_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_workspace_response_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_workspace_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_workspaces_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-03 19:39:44.000000 asana_preview-1.0.7/test/test_workspaces_workspace_gid_body.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:43:04.000000 asana_preview-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-07 20:43:04.000000 asana_preview-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    59356 2023-07-07 20:42:52.000000 asana_preview-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:43:04.000000 asana_preview-1.0.8/asana_preview/
+-rw-r--r--   0 runner    (1001) docker     (123)    36222 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:43:04.000000 asana_preview-1.0.8/asana_preview/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23646 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/api/attachments_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12527 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/api/audit_log_api_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/api/batch_api_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13741 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/api/custom_field_settings_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45245 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/api/custom_fields_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7763 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/api/events_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27360 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/api/goal_relationships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52947 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/api/goals_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/api/jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18699 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/api/memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/api/organization_exports_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18543 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/api/portfolio_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63752 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/api/portfolios_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20933 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/api/project_briefs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/api/project_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21913 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/api/project_statuses_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28293 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/api/project_templates_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107816 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/api/projects_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/api/rules_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35837 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/api/sections_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21760 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/api/status_updates_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27300 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/api/stories_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45876 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/api/tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   163541 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/api/tasks_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24353 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/api/team_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40712 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/api/teams_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11681 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/api/time_periods_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28130 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/api/time_tracking_entries_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11675 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/api/typeahead_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/api/user_task_lists_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28905 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/api/users_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29484 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/api/webhooks_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18371 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/api/workspace_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27463 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/api/workspaces_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25183 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:43:04.000000 asana_preview-1.0.8/asana_preview/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    33965 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/add_custom_field_setting_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/add_followers_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/add_members_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/all_of_project_response_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/all_of_project_template_base_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/all_of_project_template_response_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/all_of_story_response_new_date_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/all_of_story_response_old_date_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/all_of_task_response_assignee_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/all_of_user_task_list_base_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/all_of_user_task_list_base_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/all_of_user_task_list_compact_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/all_of_user_task_list_compact_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/all_of_user_task_list_request_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/all_of_user_task_list_request_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/all_of_user_task_list_response_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/all_of_user_task_list_response_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/all_of_workspace_membership_response_user_task_list_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/all_of_workspace_membership_response_user_task_list_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/asana_named_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/asana_named_resource_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/asana_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/attachment_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/attachment_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/attachment_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14064 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/attachment_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/attachment_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/attachment_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/attachment_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8729 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/audit_log_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/audit_log_event_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/audit_log_event_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8838 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/audit_log_event_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/audit_log_event_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/audit_log_event_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/batch_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/batch_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/batch_request_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/batch_request_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/batch_request_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/batch_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/batch_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/create_membership_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/create_time_tracking_entry_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30420 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/custom_field_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/custom_field_base_date_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/custom_field_base_enum_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/custom_field_base_enum_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16739 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/custom_field_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/custom_field_gid_enum_options_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34312 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/custom_field_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33924 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/custom_field_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/custom_field_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/custom_field_response_created_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/custom_field_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/custom_field_response_people_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/custom_field_setting_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/custom_field_setting_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/custom_field_setting_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/custom_field_setting_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35868 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/custom_field_setting_response_custom_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/custom_field_setting_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/custom_field_setting_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/custom_field_setting_response_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/custom_fields_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/custom_fields_custom_field_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/date_variable_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/date_variable_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/empty_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/empty_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/enum_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/enum_option_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/enum_option_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/enum_option_insert_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8757 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/enum_option_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/enum_options_enum_option_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/enum_options_insert_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/error_response_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7955 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/event_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/event_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9221 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/event_response_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/event_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/event_response_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/event_response_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goal_add_subgoal_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goal_add_supporting_relationship_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goal_add_supporting_work_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goal_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goal_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goal_gid_add_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goal_gid_add_supporting_relationship_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goal_gid_remove_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goal_gid_remove_supporting_relationship_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goal_gid_set_metric_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goal_gid_set_metric_current_value_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goal_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goal_membership_base_goal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goal_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goal_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15542 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goal_metric_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goal_metric_current_value_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15686 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goal_metric_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goal_relationship_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goal_relationship_base_supported_goal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goal_relationship_base_supporting_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8105 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goal_relationship_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goal_relationship_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goal_relationship_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goal_relationship_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goal_relationship_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goal_relationships_goal_relationship_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goal_remove_subgoal_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goal_remove_supporting_relationship_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14351 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goal_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13884 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goal_request_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18927 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goal_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goal_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goal_response_current_status_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goal_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goal_response_likes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17038 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goal_response_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goal_response_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goal_response_time_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goal_response_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15329 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goal_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goals_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/goals_goal_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/inline_response412.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/inline_response412_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/job_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/job_base_new_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/job_base_new_project_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/job_base_new_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/job_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8940 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/job_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/job_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/like.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/member_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/membership_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/membership_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/membership_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/memberships_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/memberships_membership_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/message_base_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/modify_dependencies_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/modify_dependents_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8622 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/organization_export_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8706 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/organization_export_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/organization_export_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8734 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/organization_export_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/organization_export_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/organization_exports_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/portfolio_add_item_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/portfolio_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/portfolio_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/portfolio_gid_add_custom_field_setting_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/portfolio_gid_add_item_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/portfolio_gid_add_members_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/portfolio_gid_remove_custom_field_setting_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/portfolio_gid_remove_item_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/portfolio_gid_remove_members_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/portfolio_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/portfolio_membership_base_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/portfolio_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/portfolio_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/portfolio_membership_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/portfolio_membership_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/portfolio_remove_item_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/portfolio_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18230 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/portfolio_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/portfolio_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/portfolio_response_current_status_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/portfolio_response_custom_field_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17399 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/portfolio_response_custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/portfolio_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/portfolio_response_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/portfolios_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/portfolios_portfolio_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20495 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11697 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_base_current_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_base_current_status_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_base_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_brief_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_brief_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_brief_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_brief_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_brief_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_brief_response_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_briefs_project_brief_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_duplicate_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_duplicate_request_schedule_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_gid_add_custom_field_setting_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_gid_add_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_gid_add_members_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_gid_duplicate_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_gid_project_briefs_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_gid_project_statuses_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_gid_remove_custom_field_setting_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_gid_remove_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_gid_remove_members_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_gid_save_as_template_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_gid_sections_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_membership_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_membership_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_membership_response_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24286 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31095 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_response_completed_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_response_created_from_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_response_project_brief.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_response_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_save_as_template_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_section_insert_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7805 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_status_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_status_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_status_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11565 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_status_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_status_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12987 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_template_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_template_base_requested_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_template_base_requested_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_template_base_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_template_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_template_gid_instantiate_project_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9448 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_template_instantiate_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_template_instantiate_project_request_requested_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_template_instantiate_project_request_requested_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_template_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_template_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/project_template_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/projects_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/projects_project_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/remove_custom_field_setting_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/remove_followers_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/remove_members_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/requested_role_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/rule_trigger_gid_run_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/rule_trigger_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/rule_trigger_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/rule_trigger_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/section_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/section_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/section_gid_add_task_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/section_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7358 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/section_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/section_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/section_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/section_task_insert_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/sections_insert_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/sections_section_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9879 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/status_update_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/status_update_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10929 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/status_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19665 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/status_update_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/status_update_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/status_update_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/status_update_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/status_updates_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/stories_story_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/story_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/story_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/story_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48927 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/story_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/story_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/story_response_assignee.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17099 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/story_response_custom_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/story_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/story_response_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/story_response_old_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/story_response_old_enum_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/story_response_old_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/story_response_previews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/story_response_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/story_response_story.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/story_response_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/story_response_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/story_response_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/tag_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/tag_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/tag_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/tag_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/tag_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/tags_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/task_add_followers_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/task_add_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/task_add_tag_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35097 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/task_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/task_base_completed_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/task_base_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/task_base_external.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/task_base_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/task_base_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6613 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/task_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/task_count_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/task_count_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/task_duplicate_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/task_gid_add_dependencies_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/task_gid_add_dependents_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/task_gid_add_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/task_gid_add_project_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/task_gid_add_tag_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/task_gid_duplicate_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/task_gid_remove_dependencies_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/task_gid_remove_dependents_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/task_gid_remove_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/task_gid_remove_project_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/task_gid_remove_tag_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/task_gid_set_parent_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/task_gid_stories_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/task_gid_subtasks_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/task_gid_time_tracking_entries_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/task_remove_followers_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/task_remove_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/task_remove_tag_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43510 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44580 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/task_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/task_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34464 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/task_response_custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/task_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/task_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/task_response_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/task_response_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/task_set_parent_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/tasks_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/tasks_task_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/team_add_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/team_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/team_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/team_gid_add_user_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/team_gid_projects_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/team_gid_remove_user_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/team_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/team_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/team_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/team_membership_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/team_membership_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/team_remove_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19673 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/team_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20553 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/team_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/team_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/team_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/team_response_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/teams_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/teams_body1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/template_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/time_period_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/time_period_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/time_period_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/time_period_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/time_period_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/time_tracking_entries_time_tracking_entry_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/time_tracking_entry_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/time_tracking_entry_base_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/time_tracking_entry_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/time_tracking_entry_compact_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/update_time_tracking_entry_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/user_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/user_base_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/user_base_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/user_base_response_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/user_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/user_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/user_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/user_task_list_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/user_task_list_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/user_task_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/user_task_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/user_task_list_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/webhook_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/webhook_compact_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/webhook_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/webhook_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/webhook_request_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11774 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/webhook_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/webhook_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/webhook_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/webhook_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/webhooks_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/webhooks_webhook_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/workspace_add_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/workspace_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/workspace_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/workspace_gid_add_user_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/workspace_gid_projects_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/workspace_gid_remove_user_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/workspace_gid_tags_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/workspace_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/workspace_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/workspace_membership_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/workspace_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/workspace_membership_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/workspace_membership_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/workspace_membership_response_user_task_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/workspace_membership_response_vacation_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/workspace_remove_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/workspace_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/workspace_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/workspace_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/models/workspaces_workspace_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13139 2023-07-07 20:42:52.000000 asana_preview-1.0.8/asana_preview/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:43:04.000000 asana_preview-1.0.8/asana_preview.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-07 20:43:04.000000 asana_preview-1.0.8/asana_preview.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    39003 2023-07-07 20:43:04.000000 asana_preview-1.0.8/asana_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 20:43:04.000000 asana_preview-1.0.8/asana_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-07 20:43:04.000000 asana_preview-1.0.8/asana_preview.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-07 20:43:04.000000 asana_preview-1.0.8/asana_preview.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 20:43:04.000000 asana_preview-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-07 20:42:52.000000 asana_preview-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:43:04.000000 asana_preview-1.0.8/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_add_custom_field_setting_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_add_followers_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_add_members_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_all_of_project_response_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_all_of_project_template_base_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_all_of_project_template_response_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_all_of_story_response_new_date_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_all_of_story_response_old_date_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_all_of_task_response_assignee_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_all_of_user_task_list_base_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_all_of_user_task_list_base_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_all_of_user_task_list_compact_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_all_of_user_task_list_compact_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_all_of_user_task_list_request_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_all_of_user_task_list_request_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_all_of_user_task_list_response_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_all_of_user_task_list_response_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_all_of_workspace_membership_response_user_task_list_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_all_of_workspace_membership_response_user_task_list_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_asana_named_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_asana_named_resource_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_asana_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_attachment_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_attachment_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_attachment_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_attachment_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_attachment_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_attachment_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_attachment_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_attachments_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_audit_log_api_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_audit_log_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_audit_log_event_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_audit_log_event_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_audit_log_event_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_audit_log_event_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_audit_log_event_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_batch_api_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_batch_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_batch_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_batch_request_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_batch_request_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_batch_request_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_batch_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_batch_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_create_membership_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_create_time_tracking_entry_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_custom_field_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_custom_field_base_date_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_custom_field_base_enum_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_custom_field_base_enum_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_custom_field_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_custom_field_gid_enum_options_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_custom_field_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_custom_field_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_custom_field_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_custom_field_response_created_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_custom_field_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_custom_field_response_people_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_custom_field_setting_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_custom_field_setting_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_custom_field_setting_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_custom_field_setting_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_custom_field_setting_response_custom_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_custom_field_setting_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_custom_field_setting_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_custom_field_setting_response_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_custom_field_settings_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_custom_fields_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_custom_fields_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_custom_fields_custom_field_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_date_variable_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_date_variable_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_empty_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_empty_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_enum_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_enum_option_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_enum_option_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_enum_option_insert_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_enum_option_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_enum_options_enum_option_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_enum_options_insert_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_error_response_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_event_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_event_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_event_response_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_event_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_event_response_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_event_response_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_events_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goal_add_subgoal_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goal_add_supporting_relationship_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goal_add_supporting_work_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goal_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goal_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goal_gid_add_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goal_gid_add_supporting_relationship_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goal_gid_remove_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goal_gid_remove_supporting_relationship_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goal_gid_set_metric_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goal_gid_set_metric_current_value_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goal_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goal_membership_base_goal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goal_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goal_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goal_metric_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goal_metric_current_value_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goal_metric_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goal_relationship_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goal_relationship_base_supported_goal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goal_relationship_base_supporting_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goal_relationship_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goal_relationship_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goal_relationship_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goal_relationship_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goal_relationship_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goal_relationships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goal_relationships_goal_relationship_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goal_remove_subgoal_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goal_remove_supporting_relationship_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goal_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goal_request_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goal_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goal_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goal_response_current_status_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goal_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goal_response_likes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goal_response_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goal_response_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goal_response_time_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goal_response_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goal_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goals_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goals_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_goals_goal_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_inline_response412.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_inline_response412_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_job_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_job_base_new_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_job_base_new_project_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_job_base_new_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_job_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_job_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_job_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_like.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_member_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_membership_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_membership_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_membership_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_memberships_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_memberships_membership_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_message_base_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_modify_dependencies_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_modify_dependents_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_organization_export_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_organization_export_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_organization_export_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_organization_export_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_organization_export_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_organization_exports_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_organization_exports_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_portfolio_add_item_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_portfolio_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_portfolio_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_portfolio_gid_add_custom_field_setting_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_portfolio_gid_add_item_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_portfolio_gid_add_members_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_portfolio_gid_remove_custom_field_setting_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_portfolio_gid_remove_item_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_portfolio_gid_remove_members_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_portfolio_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_portfolio_membership_base_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_portfolio_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_portfolio_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_portfolio_membership_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_portfolio_membership_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_portfolio_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_portfolio_remove_item_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_portfolio_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_portfolio_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_portfolio_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_portfolio_response_current_status_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_portfolio_response_custom_field_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_portfolio_response_custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_portfolio_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_portfolio_response_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_portfolios_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_portfolios_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_portfolios_portfolio_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_base_current_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_base_current_status_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_base_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_brief_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_brief_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_brief_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_brief_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_brief_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_brief_response_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_briefs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_briefs_project_brief_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_duplicate_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_duplicate_request_schedule_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_gid_add_custom_field_setting_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_gid_add_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_gid_add_members_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_gid_duplicate_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_gid_project_briefs_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_gid_project_statuses_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_gid_remove_custom_field_setting_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_gid_remove_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_gid_remove_members_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_gid_save_as_template_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_gid_sections_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_membership_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_membership_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_membership_response_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_response_completed_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_response_created_from_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_response_project_brief.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_response_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_save_as_template_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_section_insert_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_status_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_status_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_status_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_status_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_status_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_statuses_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_template_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_template_base_requested_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_template_base_requested_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_template_base_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_template_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_template_gid_instantiate_project_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_template_instantiate_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_template_instantiate_project_request_requested_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_template_instantiate_project_request_requested_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_template_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_template_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_template_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_project_templates_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_projects_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_projects_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_projects_project_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_remove_custom_field_setting_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_remove_followers_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_remove_members_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_requested_role_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_rule_trigger_gid_run_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_rule_trigger_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_rule_trigger_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_rule_trigger_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_rules_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_section_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_section_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_section_gid_add_task_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_section_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_section_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_section_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_section_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_section_task_insert_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_sections_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_sections_insert_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_sections_section_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_status_update_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_status_update_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_status_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_status_update_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_status_update_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_status_update_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_status_update_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_status_updates_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_status_updates_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_stories_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_stories_story_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_story_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_story_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_story_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_story_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_story_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_story_response_assignee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_story_response_custom_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_story_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_story_response_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_story_response_old_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_story_response_old_enum_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_story_response_old_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_story_response_previews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_story_response_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_story_response_story.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_story_response_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_story_response_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_story_response_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_tag_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_tag_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_tag_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_tag_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_tag_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_tags_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_task_add_followers_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_task_add_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_task_add_tag_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_task_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_task_base_completed_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_task_base_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_task_base_external.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_task_base_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_task_base_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_task_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_task_count_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_task_count_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_task_duplicate_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_task_gid_add_dependencies_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_task_gid_add_dependents_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_task_gid_add_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_task_gid_add_project_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_task_gid_add_tag_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_task_gid_duplicate_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_task_gid_remove_dependencies_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_task_gid_remove_dependents_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_task_gid_remove_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_task_gid_remove_project_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_task_gid_remove_tag_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_task_gid_set_parent_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_task_gid_stories_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_task_gid_subtasks_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_task_gid_time_tracking_entries_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_task_remove_followers_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_task_remove_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_task_remove_tag_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_task_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_task_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_task_response_custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_task_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_task_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_task_response_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_task_response_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_task_set_parent_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_tasks_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_tasks_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_tasks_task_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_team_add_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_team_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_team_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_team_gid_add_user_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_team_gid_projects_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_team_gid_remove_user_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_team_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_team_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_team_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_team_membership_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_team_membership_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_team_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_team_remove_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_team_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_team_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_team_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_team_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_team_response_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_teams_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_teams_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_teams_body1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_template_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_time_period_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_time_period_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_time_period_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_time_period_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_time_period_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_time_periods_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_time_tracking_entries_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_time_tracking_entries_time_tracking_entry_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_time_tracking_entry_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_time_tracking_entry_base_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_time_tracking_entry_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_time_tracking_entry_compact_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_typeahead_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_update_time_tracking_entry_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_user_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_user_base_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_user_base_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_user_base_response_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_user_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_user_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_user_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_user_task_list_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_user_task_list_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_user_task_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_user_task_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_user_task_list_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_user_task_lists_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_users_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_webhook_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_webhook_compact_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_webhook_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_webhook_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_webhook_request_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_webhook_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_webhook_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_webhook_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_webhook_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_webhooks_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_webhooks_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_webhooks_webhook_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_workspace_add_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_workspace_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_workspace_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_workspace_gid_add_user_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_workspace_gid_projects_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_workspace_gid_remove_user_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_workspace_gid_tags_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_workspace_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_workspace_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_workspace_membership_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_workspace_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_workspace_membership_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_workspace_membership_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_workspace_membership_response_user_task_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_workspace_membership_response_vacation_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_workspace_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_workspace_remove_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_workspace_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_workspace_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_workspace_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_workspaces_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-07 20:42:52.000000 asana_preview-1.0.8/test/test_workspaces_workspace_gid_body.py
```

### Comparing `asana_preview-1.0.7/README.md` & `asana_preview-1.0.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # asana_preview
 This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
 - API version: 1.0
-- Package version: 1.0.7
+- Package version: 1.0.8
 - Build package: com.asana.codegen.PythonClientCodegenGenerator
 For more information, please visit [https://asana.com/support](https://asana.com/support)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
@@ -435,14 +435,16 @@
  - [GoalResponseMetric](docs/GoalResponseMetric.md)
  - [GoalResponseTeam](docs/GoalResponseTeam.md)
  - [GoalResponseTimePeriod](docs/GoalResponseTimePeriod.md)
  - [GoalResponseWorkspace](docs/GoalResponseWorkspace.md)
  - [GoalUpdateRequest](docs/GoalUpdateRequest.md)
  - [GoalsBody](docs/GoalsBody.md)
  - [GoalsGoalGidBody](docs/GoalsGoalGidBody.md)
+ - [InlineResponse412](docs/InlineResponse412.md)
+ - [InlineResponse412Errors](docs/InlineResponse412Errors.md)
  - [JobBase](docs/JobBase.md)
  - [JobBaseNewProject](docs/JobBaseNewProject.md)
  - [JobBaseNewProjectTemplate](docs/JobBaseNewProjectTemplate.md)
  - [JobBaseNewTask](docs/JobBaseNewTask.md)
  - [JobCompact](docs/JobCompact.md)
  - [JobResponse](docs/JobResponse.md)
  - [JobResponseData](docs/JobResponseData.md)
@@ -450,15 +452,14 @@
  - [MemberCompact](docs/MemberCompact.md)
  - [MembershipRequest](docs/MembershipRequest.md)
  - [MembershipResponse](docs/MembershipResponse.md)
  - [MembershipResponseArray](docs/MembershipResponseArray.md)
  - [MembershipResponseData](docs/MembershipResponseData.md)
  - [MembershipsBody](docs/MembershipsBody.md)
  - [MembershipsMembershipGidBody](docs/MembershipsMembershipGidBody.md)
- - [MessageBaseData](docs/MessageBaseData.md)
  - [ModifyDependenciesRequest](docs/ModifyDependenciesRequest.md)
  - [ModifyDependentsRequest](docs/ModifyDependentsRequest.md)
  - [OrganizationExportBase](docs/OrganizationExportBase.md)
  - [OrganizationExportCompact](docs/OrganizationExportCompact.md)
  - [OrganizationExportRequest](docs/OrganizationExportRequest.md)
  - [OrganizationExportResponse](docs/OrganizationExportResponse.md)
  - [OrganizationExportResponseData](docs/OrganizationExportResponseData.md)
```

### Comparing `asana_preview-1.0.7/asana_preview/__init__.py` & `asana_preview-1.0.8/asana_preview/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,14 +178,16 @@
 from asana_preview.models.goal_response_metric import GoalResponseMetric
 from asana_preview.models.goal_response_team import GoalResponseTeam
 from asana_preview.models.goal_response_time_period import GoalResponseTimePeriod
 from asana_preview.models.goal_response_workspace import GoalResponseWorkspace
 from asana_preview.models.goal_update_request import GoalUpdateRequest
 from asana_preview.models.goals_body import GoalsBody
 from asana_preview.models.goals_goal_gid_body import GoalsGoalGidBody
+from asana_preview.models.inline_response412 import InlineResponse412
+from asana_preview.models.inline_response412_errors import InlineResponse412Errors
 from asana_preview.models.job_base import JobBase
 from asana_preview.models.job_base_new_project import JobBaseNewProject
 from asana_preview.models.job_base_new_project_template import JobBaseNewProjectTemplate
 from asana_preview.models.job_base_new_task import JobBaseNewTask
 from asana_preview.models.job_compact import JobCompact
 from asana_preview.models.job_response import JobResponse
 from asana_preview.models.job_response_data import JobResponseData
@@ -193,15 +195,14 @@
 from asana_preview.models.member_compact import MemberCompact
 from asana_preview.models.membership_request import MembershipRequest
 from asana_preview.models.membership_response import MembershipResponse
 from asana_preview.models.membership_response_array import MembershipResponseArray
 from asana_preview.models.membership_response_data import MembershipResponseData
 from asana_preview.models.memberships_body import MembershipsBody
 from asana_preview.models.memberships_membership_gid_body import MembershipsMembershipGidBody
-from asana_preview.models.message_base_data import MessageBaseData
 from asana_preview.models.modify_dependencies_request import ModifyDependenciesRequest
 from asana_preview.models.modify_dependents_request import ModifyDependentsRequest
 from asana_preview.models.organization_export_base import OrganizationExportBase
 from asana_preview.models.organization_export_compact import OrganizationExportCompact
 from asana_preview.models.organization_export_request import OrganizationExportRequest
 from asana_preview.models.organization_export_response import OrganizationExportResponse
 from asana_preview.models.organization_export_response_data import OrganizationExportResponseData
```

### Comparing `asana_preview-1.0.7/asana_preview/api/__init__.py` & `asana_preview-1.0.8/asana_preview/api/__init__.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/api/attachments_api.py` & `asana_preview-1.0.8/asana_preview/api/attachments_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/api/audit_log_api_api.py` & `asana_preview-1.0.8/asana_preview/api/audit_log_api_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/api/batch_api_api.py` & `asana_preview-1.0.8/asana_preview/api/batch_api_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/api/custom_field_settings_api.py` & `asana_preview-1.0.8/asana_preview/api/custom_field_settings_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/api/custom_fields_api.py` & `asana_preview-1.0.8/asana_preview/api/custom_fields_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/api/events_api.py` & `asana_preview-1.0.8/asana_preview/api/events_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
     def get_events(self, resource, **kwargs):  # noqa: E501
         """Get events on a resource  # noqa: E501
 
-        Returns the full record for all events that have occurred since the sync token was created.  A `GET` request to the endpoint `/[path_to_resource]/events` can be made in lieu of including the resource ID in the data for the request.  Asana limits a single sync token to 100 events. If more than 100 events exist for a given resource, `has_more: true` will be returned in the response, indicating that there are more events to pull.   *Note: The resource returned will be the resource that triggered the event. This may be different from the one that the events were requested for. For example, a subscription to a project will contain events for tasks contained within the project.*  # noqa: E501
+        Returns the full record for all events that have occurred since the sync token was created.  A `GET` request to the endpoint `/[path_to_resource]/events` can be made in lieu of including the resource ID in the data for the request.  Asana limits a single sync token to 100 events. If more than 100 events exist for a given resource, `has_more: true` will be returned in the response, indicating that there are more events to pull.  *Note: The resource returned will be the resource that triggered the event. This may be different from the one that the events were requested for. For example, a subscription to a project will contain events for tasks contained within the project.*  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_events(resource, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str resource: A resource ID to subscribe to. The resource can be a task or project. (required)
@@ -55,15 +55,15 @@
         else:
             (data) = self.get_events_with_http_info(resource, **kwargs)  # noqa: E501
             return data
 
     def get_events_with_http_info(self, resource, **kwargs):  # noqa: E501
         """Get events on a resource  # noqa: E501
 
-        Returns the full record for all events that have occurred since the sync token was created.  A `GET` request to the endpoint `/[path_to_resource]/events` can be made in lieu of including the resource ID in the data for the request.  Asana limits a single sync token to 100 events. If more than 100 events exist for a given resource, `has_more: true` will be returned in the response, indicating that there are more events to pull.   *Note: The resource returned will be the resource that triggered the event. This may be different from the one that the events were requested for. For example, a subscription to a project will contain events for tasks contained within the project.*  # noqa: E501
+        Returns the full record for all events that have occurred since the sync token was created.  A `GET` request to the endpoint `/[path_to_resource]/events` can be made in lieu of including the resource ID in the data for the request.  Asana limits a single sync token to 100 events. If more than 100 events exist for a given resource, `has_more: true` will be returned in the response, indicating that there are more events to pull.  *Note: The resource returned will be the resource that triggered the event. This may be different from the one that the events were requested for. For example, a subscription to a project will contain events for tasks contained within the project.*  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_events_with_http_info(resource, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str resource: A resource ID to subscribe to. The resource can be a task or project. (required)
```

### Comparing `asana_preview-1.0.7/asana_preview/api/goal_relationships_api.py` & `asana_preview-1.0.8/asana_preview/api/goal_relationships_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/api/goals_api.py` & `asana_preview-1.0.8/asana_preview/api/goals_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/api/jobs_api.py` & `asana_preview-1.0.8/asana_preview/api/jobs_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/api/memberships_api.py` & `asana_preview-1.0.8/asana_preview/api/memberships_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/api/organization_exports_api.py` & `asana_preview-1.0.8/asana_preview/api/organization_exports_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/api/portfolio_memberships_api.py` & `asana_preview-1.0.8/asana_preview/api/portfolio_memberships_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/api/portfolios_api.py` & `asana_preview-1.0.8/asana_preview/api/portfolios_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/api/project_briefs_api.py` & `asana_preview-1.0.8/asana_preview/api/project_briefs_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/api/project_memberships_api.py` & `asana_preview-1.0.8/asana_preview/api/project_memberships_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/api/project_statuses_api.py` & `asana_preview-1.0.8/asana_preview/api/project_statuses_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/api/project_templates_api.py` & `asana_preview-1.0.8/asana_preview/api/project_templates_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/api/projects_api.py` & `asana_preview-1.0.8/asana_preview/api/projects_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/api/rules_api.py` & `asana_preview-1.0.8/asana_preview/api/rules_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/api/sections_api.py` & `asana_preview-1.0.8/asana_preview/api/sections_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/api/status_updates_api.py` & `asana_preview-1.0.8/asana_preview/api/status_updates_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/api/stories_api.py` & `asana_preview-1.0.8/asana_preview/api/stories_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/api/tags_api.py` & `asana_preview-1.0.8/asana_preview/api/tags_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/api/tasks_api.py` & `asana_preview-1.0.8/asana_preview/api/tasks_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/api/team_memberships_api.py` & `asana_preview-1.0.8/asana_preview/api/team_memberships_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/api/teams_api.py` & `asana_preview-1.0.8/asana_preview/api/teams_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/api/time_periods_api.py` & `asana_preview-1.0.8/asana_preview/api/time_periods_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/api/time_tracking_entries_api.py` & `asana_preview-1.0.8/asana_preview/api/time_tracking_entries_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/api/typeahead_api.py` & `asana_preview-1.0.8/asana_preview/api/typeahead_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/api/user_task_lists_api.py` & `asana_preview-1.0.8/asana_preview/api/user_task_lists_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/api/users_api.py` & `asana_preview-1.0.8/asana_preview/api/users_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/api/webhooks_api.py` & `asana_preview-1.0.8/asana_preview/api/webhooks_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/api/workspace_memberships_api.py` & `asana_preview-1.0.8/asana_preview/api/workspace_memberships_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/api/workspaces_api.py` & `asana_preview-1.0.8/asana_preview/api/workspaces_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/api_client.py` & `asana_preview-1.0.8/asana_preview/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         self.pool = ThreadPool()
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Swagger-Codegen/1.0.7/python'
+        self.user_agent = 'Swagger-Codegen/1.0.8/python'
 
     def __del__(self):
         self.pool.close()
         self.pool.join()
 
     @property
     def user_agent(self):
```

### Comparing `asana_preview-1.0.7/asana_preview/configuration.py` & `asana_preview-1.0.8/asana_preview/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,9 +245,9 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0\n"\
-               "SDK Package Version: 1.0.7".\
+               "SDK Package Version: 1.0.8".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `asana_preview-1.0.7/asana_preview/models/__init__.py` & `asana_preview-1.0.8/asana_preview/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,14 +139,16 @@
 from asana_preview.models.goal_response_metric import GoalResponseMetric
 from asana_preview.models.goal_response_team import GoalResponseTeam
 from asana_preview.models.goal_response_time_period import GoalResponseTimePeriod
 from asana_preview.models.goal_response_workspace import GoalResponseWorkspace
 from asana_preview.models.goal_update_request import GoalUpdateRequest
 from asana_preview.models.goals_body import GoalsBody
 from asana_preview.models.goals_goal_gid_body import GoalsGoalGidBody
+from asana_preview.models.inline_response412 import InlineResponse412
+from asana_preview.models.inline_response412_errors import InlineResponse412Errors
 from asana_preview.models.job_base import JobBase
 from asana_preview.models.job_base_new_project import JobBaseNewProject
 from asana_preview.models.job_base_new_project_template import JobBaseNewProjectTemplate
 from asana_preview.models.job_base_new_task import JobBaseNewTask
 from asana_preview.models.job_compact import JobCompact
 from asana_preview.models.job_response import JobResponse
 from asana_preview.models.job_response_data import JobResponseData
@@ -154,15 +156,14 @@
 from asana_preview.models.member_compact import MemberCompact
 from asana_preview.models.membership_request import MembershipRequest
 from asana_preview.models.membership_response import MembershipResponse
 from asana_preview.models.membership_response_array import MembershipResponseArray
 from asana_preview.models.membership_response_data import MembershipResponseData
 from asana_preview.models.memberships_body import MembershipsBody
 from asana_preview.models.memberships_membership_gid_body import MembershipsMembershipGidBody
-from asana_preview.models.message_base_data import MessageBaseData
 from asana_preview.models.modify_dependencies_request import ModifyDependenciesRequest
 from asana_preview.models.modify_dependents_request import ModifyDependentsRequest
 from asana_preview.models.organization_export_base import OrganizationExportBase
 from asana_preview.models.organization_export_compact import OrganizationExportCompact
 from asana_preview.models.organization_export_request import OrganizationExportRequest
 from asana_preview.models.organization_export_response import OrganizationExportResponse
 from asana_preview.models.organization_export_response_data import OrganizationExportResponseData
```

### Comparing `asana_preview-1.0.7/asana_preview/models/add_custom_field_setting_request.py` & `asana_preview-1.0.8/asana_preview/models/add_custom_field_setting_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/add_followers_request.py` & `asana_preview-1.0.8/asana_preview/models/add_followers_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/add_members_request.py` & `asana_preview-1.0.8/asana_preview/models/add_members_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/all_of_project_response_owner.py` & `asana_preview-1.0.8/asana_preview/models/all_of_project_response_owner.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/all_of_project_template_base_owner.py` & `asana_preview-1.0.8/asana_preview/models/all_of_project_template_base_owner.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/all_of_project_template_response_owner.py` & `asana_preview-1.0.8/asana_preview/models/all_of_project_template_response_owner.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/all_of_story_response_new_date_value.py` & `asana_preview-1.0.8/asana_preview/models/all_of_story_response_new_date_value.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/all_of_story_response_old_date_value.py` & `asana_preview-1.0.8/asana_preview/models/all_of_story_response_old_date_value.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/all_of_task_response_assignee_section.py` & `asana_preview-1.0.8/asana_preview/models/all_of_task_response_assignee_section.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/all_of_user_task_list_base_owner.py` & `asana_preview-1.0.8/asana_preview/models/all_of_user_task_list_base_owner.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/all_of_user_task_list_base_workspace.py` & `asana_preview-1.0.8/asana_preview/models/all_of_user_task_list_base_workspace.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/all_of_user_task_list_compact_owner.py` & `asana_preview-1.0.8/asana_preview/models/all_of_user_task_list_compact_owner.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/all_of_user_task_list_compact_workspace.py` & `asana_preview-1.0.8/asana_preview/models/all_of_user_task_list_compact_workspace.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/all_of_user_task_list_request_owner.py` & `asana_preview-1.0.8/asana_preview/models/all_of_user_task_list_request_owner.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/all_of_user_task_list_request_workspace.py` & `asana_preview-1.0.8/asana_preview/models/all_of_user_task_list_request_workspace.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/all_of_user_task_list_response_owner.py` & `asana_preview-1.0.8/asana_preview/models/all_of_user_task_list_response_owner.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/all_of_user_task_list_response_workspace.py` & `asana_preview-1.0.8/asana_preview/models/all_of_user_task_list_response_workspace.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/all_of_workspace_membership_response_user_task_list_owner.py` & `asana_preview-1.0.8/asana_preview/models/all_of_workspace_membership_response_user_task_list_owner.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/all_of_workspace_membership_response_user_task_list_workspace.py` & `asana_preview-1.0.8/asana_preview/models/all_of_workspace_membership_response_user_task_list_workspace.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/asana_named_resource.py` & `asana_preview-1.0.8/asana_preview/models/asana_named_resource.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/asana_named_resource_array.py` & `asana_preview-1.0.8/asana_preview/models/asana_named_resource_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/asana_resource.py` & `asana_preview-1.0.8/asana_preview/models/asana_resource.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/attachment_base.py` & `asana_preview-1.0.8/asana_preview/models/attachment_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/attachment_compact.py` & `asana_preview-1.0.8/asana_preview/models/attachment_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/attachment_request.py` & `asana_preview-1.0.8/asana_preview/models/attachment_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/attachment_response.py` & `asana_preview-1.0.8/asana_preview/models/attachment_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/attachment_response_array.py` & `asana_preview-1.0.8/asana_preview/models/attachment_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/attachment_response_data.py` & `asana_preview-1.0.8/asana_preview/models/attachment_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/attachment_response_parent.py` & `asana_preview-1.0.8/asana_preview/models/attachment_response_parent.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/audit_log_event.py` & `asana_preview-1.0.8/asana_preview/models/audit_log_event.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/audit_log_event_actor.py` & `asana_preview-1.0.8/asana_preview/models/audit_log_event_actor.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/audit_log_event_array.py` & `asana_preview-1.0.8/asana_preview/models/audit_log_event_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/audit_log_event_context.py` & `asana_preview-1.0.8/asana_preview/models/audit_log_event_context.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/audit_log_event_details.py` & `asana_preview-1.0.8/asana_preview/models/audit_log_event_details.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/audit_log_event_resource.py` & `asana_preview-1.0.8/asana_preview/models/audit_log_event_resource.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/batch_body.py` & `asana_preview-1.0.8/asana_preview/models/batch_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/batch_request.py` & `asana_preview-1.0.8/asana_preview/models/batch_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/batch_request_action.py` & `asana_preview-1.0.8/asana_preview/models/batch_request_action.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/batch_request_actions.py` & `asana_preview-1.0.8/asana_preview/models/batch_request_actions.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/batch_request_options.py` & `asana_preview-1.0.8/asana_preview/models/batch_request_options.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/batch_response.py` & `asana_preview-1.0.8/asana_preview/models/batch_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/batch_response_array.py` & `asana_preview-1.0.8/asana_preview/models/batch_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/create_membership_request.py` & `asana_preview-1.0.8/asana_preview/models/create_membership_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/create_time_tracking_entry_request.py` & `asana_preview-1.0.8/asana_preview/models/create_time_tracking_entry_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/custom_field_base.py` & `asana_preview-1.0.8/asana_preview/models/custom_field_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/custom_field_base_date_value.py` & `asana_preview-1.0.8/asana_preview/models/custom_field_base_date_value.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/custom_field_base_enum_options.py` & `asana_preview-1.0.8/asana_preview/models/custom_field_base_enum_options.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/custom_field_base_enum_value.py` & `asana_preview-1.0.8/asana_preview/models/custom_field_base_enum_value.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/custom_field_compact.py` & `asana_preview-1.0.8/asana_preview/models/custom_field_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/custom_field_gid_enum_options_body.py` & `asana_preview-1.0.8/asana_preview/models/custom_field_gid_enum_options_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/custom_field_request.py` & `asana_preview-1.0.8/asana_preview/models/custom_field_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/custom_field_response.py` & `asana_preview-1.0.8/asana_preview/models/custom_field_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/custom_field_response_array.py` & `asana_preview-1.0.8/asana_preview/models/custom_field_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/custom_field_response_created_by.py` & `asana_preview-1.0.8/asana_preview/models/custom_field_response_created_by.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/custom_field_response_data.py` & `asana_preview-1.0.8/asana_preview/models/custom_field_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/custom_field_response_people_value.py` & `asana_preview-1.0.8/asana_preview/models/custom_field_response_people_value.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/custom_field_setting_base.py` & `asana_preview-1.0.8/asana_preview/models/custom_field_setting_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/custom_field_setting_compact.py` & `asana_preview-1.0.8/asana_preview/models/custom_field_setting_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/custom_field_setting_response.py` & `asana_preview-1.0.8/asana_preview/models/custom_field_setting_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/custom_field_setting_response_array.py` & `asana_preview-1.0.8/asana_preview/models/custom_field_setting_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/custom_field_setting_response_custom_field.py` & `asana_preview-1.0.8/asana_preview/models/custom_field_setting_response_custom_field.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/custom_field_setting_response_data.py` & `asana_preview-1.0.8/asana_preview/models/custom_field_setting_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/custom_field_setting_response_parent.py` & `asana_preview-1.0.8/asana_preview/models/custom_field_setting_response_parent.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/custom_field_setting_response_project.py` & `asana_preview-1.0.8/asana_preview/models/custom_field_setting_response_project.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/custom_fields_body.py` & `asana_preview-1.0.8/asana_preview/models/custom_fields_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/custom_fields_custom_field_gid_body.py` & `asana_preview-1.0.8/asana_preview/models/custom_fields_custom_field_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/date_variable_compact.py` & `asana_preview-1.0.8/asana_preview/models/date_variable_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/date_variable_request.py` & `asana_preview-1.0.8/asana_preview/models/date_variable_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/empty_response.py` & `asana_preview-1.0.8/asana_preview/models/empty_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/empty_response_data.py` & `asana_preview-1.0.8/asana_preview/models/empty_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/enum_option.py` & `asana_preview-1.0.8/asana_preview/models/enum_option.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/enum_option_base.py` & `asana_preview-1.0.8/asana_preview/models/enum_option_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/enum_option_data.py` & `asana_preview-1.0.8/asana_preview/models/enum_option_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/enum_option_insert_request.py` & `asana_preview-1.0.8/asana_preview/models/enum_option_insert_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/enum_option_request.py` & `asana_preview-1.0.8/asana_preview/models/enum_option_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/enum_options_enum_option_gid_body.py` & `asana_preview-1.0.8/asana_preview/models/enum_options_enum_option_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/enum_options_insert_body.py` & `asana_preview-1.0.8/asana_preview/models/enum_options_insert_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/error.py` & `asana_preview-1.0.8/asana_preview/models/error.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/error_response.py` & `asana_preview-1.0.8/asana_preview/models/error_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/error_response_errors.py` & `asana_preview-1.0.8/asana_preview/models/error_response_errors.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/event_response.py` & `asana_preview-1.0.8/asana_preview/models/event_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/event_response_array.py` & `asana_preview-1.0.8/asana_preview/models/event_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/event_response_change.py` & `asana_preview-1.0.8/asana_preview/models/event_response_change.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/event_response_parent.py` & `asana_preview-1.0.8/asana_preview/models/event_response_parent.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/event_response_resource.py` & `asana_preview-1.0.8/asana_preview/models/event_response_resource.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/event_response_user.py` & `asana_preview-1.0.8/asana_preview/models/event_response_user.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goal_add_subgoal_request.py` & `asana_preview-1.0.8/asana_preview/models/goal_add_subgoal_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goal_add_supporting_relationship_request.py` & `asana_preview-1.0.8/asana_preview/models/goal_add_supporting_relationship_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goal_add_supporting_work_request.py` & `asana_preview-1.0.8/asana_preview/models/goal_add_supporting_work_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goal_base.py` & `asana_preview-1.0.8/asana_preview/models/goal_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goal_compact.py` & `asana_preview-1.0.8/asana_preview/models/goal_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goal_gid_add_followers_body.py` & `asana_preview-1.0.8/asana_preview/models/goal_gid_add_followers_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goal_gid_add_supporting_relationship_body.py` & `asana_preview-1.0.8/asana_preview/models/goal_gid_add_supporting_relationship_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goal_gid_remove_followers_body.py` & `asana_preview-1.0.8/asana_preview/models/goal_gid_remove_followers_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goal_gid_remove_supporting_relationship_body.py` & `asana_preview-1.0.8/asana_preview/models/goal_gid_remove_supporting_relationship_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goal_gid_set_metric_body.py` & `asana_preview-1.0.8/asana_preview/models/goal_gid_set_metric_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goal_gid_set_metric_current_value_body.py` & `asana_preview-1.0.8/asana_preview/models/goal_gid_set_metric_current_value_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goal_membership_base.py` & `asana_preview-1.0.8/asana_preview/models/goal_membership_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goal_membership_base_goal.py` & `asana_preview-1.0.8/asana_preview/models/goal_membership_base_goal.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goal_membership_compact.py` & `asana_preview-1.0.8/asana_preview/models/goal_membership_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goal_membership_response.py` & `asana_preview-1.0.8/asana_preview/models/goal_membership_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goal_metric_base.py` & `asana_preview-1.0.8/asana_preview/models/goal_metric_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goal_metric_current_value_request.py` & `asana_preview-1.0.8/asana_preview/models/goal_metric_current_value_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goal_metric_request.py` & `asana_preview-1.0.8/asana_preview/models/goal_metric_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goal_relationship_base.py` & `asana_preview-1.0.8/asana_preview/models/goal_relationship_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goal_relationship_base_supported_goal.py` & `asana_preview-1.0.8/asana_preview/models/goal_relationship_base_supported_goal.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goal_relationship_base_supporting_resource.py` & `asana_preview-1.0.8/asana_preview/models/goal_relationship_base_supporting_resource.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goal_relationship_compact.py` & `asana_preview-1.0.8/asana_preview/models/goal_relationship_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goal_relationship_request.py` & `asana_preview-1.0.8/asana_preview/models/goal_relationship_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goal_relationship_response.py` & `asana_preview-1.0.8/asana_preview/models/goal_relationship_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goal_relationship_response_array.py` & `asana_preview-1.0.8/asana_preview/models/goal_relationship_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goal_relationship_response_data.py` & `asana_preview-1.0.8/asana_preview/models/goal_relationship_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goal_relationships_goal_relationship_gid_body.py` & `asana_preview-1.0.8/asana_preview/models/goal_relationships_goal_relationship_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goal_remove_subgoal_request.py` & `asana_preview-1.0.8/asana_preview/models/goal_remove_subgoal_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goal_remove_supporting_relationship_request.py` & `asana_preview-1.0.8/asana_preview/models/goal_remove_supporting_relationship_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goal_request.py` & `asana_preview-1.0.8/asana_preview/models/goal_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goal_request_base.py` & `asana_preview-1.0.8/asana_preview/models/goal_request_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goal_response.py` & `asana_preview-1.0.8/asana_preview/models/goal_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goal_response_array.py` & `asana_preview-1.0.8/asana_preview/models/goal_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goal_response_current_status_update.py` & `asana_preview-1.0.8/asana_preview/models/goal_response_current_status_update.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goal_response_data.py` & `asana_preview-1.0.8/asana_preview/models/goal_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goal_response_likes.py` & `asana_preview-1.0.8/asana_preview/models/goal_response_likes.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goal_response_metric.py` & `asana_preview-1.0.8/asana_preview/models/goal_response_metric.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goal_response_team.py` & `asana_preview-1.0.8/asana_preview/models/goal_response_team.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goal_response_time_period.py` & `asana_preview-1.0.8/asana_preview/models/goal_response_time_period.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goal_response_workspace.py` & `asana_preview-1.0.8/asana_preview/models/goal_response_workspace.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goal_update_request.py` & `asana_preview-1.0.8/asana_preview/models/goal_update_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goals_body.py` & `asana_preview-1.0.8/asana_preview/models/goals_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/goals_goal_gid_body.py` & `asana_preview-1.0.8/asana_preview/models/goals_goal_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/job_base.py` & `asana_preview-1.0.8/asana_preview/models/job_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/job_base_new_project.py` & `asana_preview-1.0.8/asana_preview/models/job_base_new_project.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/job_base_new_project_template.py` & `asana_preview-1.0.8/asana_preview/models/job_base_new_project_template.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/job_base_new_task.py` & `asana_preview-1.0.8/asana_preview/models/job_base_new_task.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/job_compact.py` & `asana_preview-1.0.8/asana_preview/models/job_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/job_response.py` & `asana_preview-1.0.8/asana_preview/models/job_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/job_response_data.py` & `asana_preview-1.0.8/asana_preview/models/job_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/like.py` & `asana_preview-1.0.8/asana_preview/models/like.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/member_compact.py` & `asana_preview-1.0.8/asana_preview/models/member_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/membership_request.py` & `asana_preview-1.0.8/asana_preview/models/membership_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/membership_response.py` & `asana_preview-1.0.8/asana_preview/models/membership_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/membership_response_array.py` & `asana_preview-1.0.8/asana_preview/models/membership_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/membership_response_data.py` & `asana_preview-1.0.8/asana_preview/models/membership_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/memberships_body.py` & `asana_preview-1.0.8/asana_preview/models/memberships_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/memberships_membership_gid_body.py` & `asana_preview-1.0.8/asana_preview/models/memberships_membership_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/message_base_data.py` & `asana_preview-1.0.8/asana_preview/models/message_base_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/modify_dependencies_request.py` & `asana_preview-1.0.8/asana_preview/models/modify_dependencies_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/modify_dependents_request.py` & `asana_preview-1.0.8/asana_preview/models/modify_dependents_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/organization_export_base.py` & `asana_preview-1.0.8/asana_preview/models/organization_export_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/organization_export_compact.py` & `asana_preview-1.0.8/asana_preview/models/organization_export_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/organization_export_request.py` & `asana_preview-1.0.8/asana_preview/models/organization_export_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/organization_export_response.py` & `asana_preview-1.0.8/asana_preview/models/organization_export_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/organization_export_response_data.py` & `asana_preview-1.0.8/asana_preview/models/organization_export_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/organization_exports_body.py` & `asana_preview-1.0.8/asana_preview/models/organization_exports_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/portfolio_add_item_request.py` & `asana_preview-1.0.8/asana_preview/models/portfolio_add_item_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/portfolio_base.py` & `asana_preview-1.0.8/asana_preview/models/portfolio_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/portfolio_compact.py` & `asana_preview-1.0.8/asana_preview/models/portfolio_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/portfolio_gid_add_custom_field_setting_body.py` & `asana_preview-1.0.8/asana_preview/models/portfolio_gid_add_custom_field_setting_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/portfolio_gid_add_item_body.py` & `asana_preview-1.0.8/asana_preview/models/portfolio_gid_add_item_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/portfolio_gid_add_members_body.py` & `asana_preview-1.0.8/asana_preview/models/portfolio_gid_add_members_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/portfolio_gid_remove_custom_field_setting_body.py` & `asana_preview-1.0.8/asana_preview/models/portfolio_gid_remove_custom_field_setting_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/portfolio_gid_remove_item_body.py` & `asana_preview-1.0.8/asana_preview/models/portfolio_gid_remove_item_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/portfolio_gid_remove_members_body.py` & `asana_preview-1.0.8/asana_preview/models/portfolio_gid_remove_members_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/portfolio_membership_base.py` & `asana_preview-1.0.8/asana_preview/models/portfolio_membership_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/portfolio_membership_base_portfolio.py` & `asana_preview-1.0.8/asana_preview/models/portfolio_membership_base_portfolio.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/portfolio_membership_compact.py` & `asana_preview-1.0.8/asana_preview/models/portfolio_membership_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/portfolio_membership_response.py` & `asana_preview-1.0.8/asana_preview/models/portfolio_membership_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/portfolio_membership_response_array.py` & `asana_preview-1.0.8/asana_preview/models/portfolio_membership_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/portfolio_membership_response_data.py` & `asana_preview-1.0.8/asana_preview/models/portfolio_membership_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/portfolio_remove_item_request.py` & `asana_preview-1.0.8/asana_preview/models/portfolio_remove_item_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/portfolio_request.py` & `asana_preview-1.0.8/asana_preview/models/portfolio_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/portfolio_response.py` & `asana_preview-1.0.8/asana_preview/models/portfolio_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/portfolio_response_array.py` & `asana_preview-1.0.8/asana_preview/models/portfolio_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/portfolio_response_current_status_update.py` & `asana_preview-1.0.8/asana_preview/models/portfolio_response_current_status_update.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/portfolio_response_custom_field_settings.py` & `asana_preview-1.0.8/asana_preview/models/portfolio_response_custom_field_settings.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/portfolio_response_custom_fields.py` & `asana_preview-1.0.8/asana_preview/models/portfolio_response_custom_fields.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/portfolio_response_data.py` & `asana_preview-1.0.8/asana_preview/models/portfolio_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/portfolio_response_workspace.py` & `asana_preview-1.0.8/asana_preview/models/portfolio_response_workspace.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/portfolios_body.py` & `asana_preview-1.0.8/asana_preview/models/portfolios_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/portfolios_portfolio_gid_body.py` & `asana_preview-1.0.8/asana_preview/models/portfolios_portfolio_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/preview.py` & `asana_preview-1.0.8/asana_preview/models/preview.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_base.py` & `asana_preview-1.0.8/asana_preview/models/project_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_base_current_status.py` & `asana_preview-1.0.8/asana_preview/models/project_base_current_status.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_base_current_status_update.py` & `asana_preview-1.0.8/asana_preview/models/project_base_current_status_update.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_base_workspace.py` & `asana_preview-1.0.8/asana_preview/models/project_base_workspace.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_brief_base.py` & `asana_preview-1.0.8/asana_preview/models/project_brief_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_brief_compact.py` & `asana_preview-1.0.8/asana_preview/models/project_brief_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_brief_request.py` & `asana_preview-1.0.8/asana_preview/models/project_brief_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_brief_response.py` & `asana_preview-1.0.8/asana_preview/models/project_brief_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_brief_response_data.py` & `asana_preview-1.0.8/asana_preview/models/project_brief_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_brief_response_project.py` & `asana_preview-1.0.8/asana_preview/models/project_brief_response_project.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_briefs_project_brief_gid_body.py` & `asana_preview-1.0.8/asana_preview/models/project_briefs_project_brief_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_compact.py` & `asana_preview-1.0.8/asana_preview/models/project_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_duplicate_request.py` & `asana_preview-1.0.8/asana_preview/models/project_duplicate_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -104,36 +104,30 @@
 
         self._team = team
 
     @property
     def include(self):
         """Gets the include of this ProjectDuplicateRequest.  # noqa: E501
 
-        The elements that will be duplicated to the new project. Tasks are always included.  # noqa: E501
+        A comma-separated list of elements that will be duplicated to the new project. Tasks are always included. ##### Fields - forms - members - notes - task_assignee - task_attachments - task_dates - task_dependencies - task_followers - task_notes - task_projects - task_subtasks - task_tags  # noqa: E501
 
         :return: The include of this ProjectDuplicateRequest.  # noqa: E501
         :rtype: str
         """
         return self._include
 
     @include.setter
     def include(self, include):
         """Sets the include of this ProjectDuplicateRequest.
 
-        The elements that will be duplicated to the new project. Tasks are always included.  # noqa: E501
+        A comma-separated list of elements that will be duplicated to the new project. Tasks are always included. ##### Fields - forms - members - notes - task_assignee - task_attachments - task_dates - task_dependencies - task_followers - task_notes - task_projects - task_subtasks - task_tags  # noqa: E501
 
         :param include: The include of this ProjectDuplicateRequest.  # noqa: E501
         :type: str
         """
-        allowed_values = ["members", "notes", "forms", "task_notes", "task_assignee", "task_subtasks", "task_attachments", "task_dates", "task_dependencies", "task_followers", "task_tags", "task_projects"]  # noqa: E501
-        if include not in allowed_values:
-            raise ValueError(
-                "Invalid value for `include` ({0}), must be one of {1}"  # noqa: E501
-                .format(include, allowed_values)
-            )
 
         self._include = include
 
     @property
     def schedule_dates(self):
         """Gets the schedule_dates of this ProjectDuplicateRequest.  # noqa: E501
```

### Comparing `asana_preview-1.0.7/asana_preview/models/project_duplicate_request_schedule_dates.py` & `asana_preview-1.0.8/asana_preview/models/project_duplicate_request_schedule_dates.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_gid_add_custom_field_setting_body.py` & `asana_preview-1.0.8/asana_preview/models/project_gid_add_custom_field_setting_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_gid_add_followers_body.py` & `asana_preview-1.0.8/asana_preview/models/project_gid_add_followers_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_gid_add_members_body.py` & `asana_preview-1.0.8/asana_preview/models/project_gid_add_members_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_gid_duplicate_body.py` & `asana_preview-1.0.8/asana_preview/models/project_gid_duplicate_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_gid_project_briefs_body.py` & `asana_preview-1.0.8/asana_preview/models/project_gid_project_briefs_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_gid_project_statuses_body.py` & `asana_preview-1.0.8/asana_preview/models/project_gid_project_statuses_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_gid_remove_custom_field_setting_body.py` & `asana_preview-1.0.8/asana_preview/models/project_gid_remove_custom_field_setting_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_gid_remove_followers_body.py` & `asana_preview-1.0.8/asana_preview/models/project_gid_remove_followers_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_gid_remove_members_body.py` & `asana_preview-1.0.8/asana_preview/models/project_gid_remove_members_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_gid_save_as_template_body.py` & `asana_preview-1.0.8/asana_preview/models/project_gid_save_as_template_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_gid_sections_body.py` & `asana_preview-1.0.8/asana_preview/models/project_gid_sections_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_membership_base.py` & `asana_preview-1.0.8/asana_preview/models/project_membership_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_membership_compact.py` & `asana_preview-1.0.8/asana_preview/models/project_membership_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_membership_response.py` & `asana_preview-1.0.8/asana_preview/models/project_membership_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_membership_response_array.py` & `asana_preview-1.0.8/asana_preview/models/project_membership_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_membership_response_data.py` & `asana_preview-1.0.8/asana_preview/models/project_membership_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_membership_response_member.py` & `asana_preview-1.0.8/asana_preview/models/project_membership_response_member.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_request.py` & `asana_preview-1.0.8/asana_preview/models/project_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_response.py` & `asana_preview-1.0.8/asana_preview/models/project_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_response_array.py` & `asana_preview-1.0.8/asana_preview/models/project_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_response_completed_by.py` & `asana_preview-1.0.8/asana_preview/models/project_response_completed_by.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_response_created_from_template.py` & `asana_preview-1.0.8/asana_preview/models/project_response_created_from_template.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_response_data.py` & `asana_preview-1.0.8/asana_preview/models/project_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_response_project_brief.py` & `asana_preview-1.0.8/asana_preview/models/project_response_project_brief.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_response_team.py` & `asana_preview-1.0.8/asana_preview/models/project_response_team.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_save_as_template_request.py` & `asana_preview-1.0.8/asana_preview/models/project_save_as_template_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_section_insert_request.py` & `asana_preview-1.0.8/asana_preview/models/project_section_insert_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_status_base.py` & `asana_preview-1.0.8/asana_preview/models/project_status_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_status_compact.py` & `asana_preview-1.0.8/asana_preview/models/project_status_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_status_request.py` & `asana_preview-1.0.8/asana_preview/models/project_status_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_status_response.py` & `asana_preview-1.0.8/asana_preview/models/project_status_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_status_response_array.py` & `asana_preview-1.0.8/asana_preview/models/project_status_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_status_response_data.py` & `asana_preview-1.0.8/asana_preview/models/project_status_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_template_base.py` & `asana_preview-1.0.8/asana_preview/models/project_template_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_template_base_requested_dates.py` & `asana_preview-1.0.8/asana_preview/models/project_template_base_requested_dates.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_template_base_requested_roles.py` & `asana_preview-1.0.8/asana_preview/models/project_template_base_requested_roles.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_template_base_team.py` & `asana_preview-1.0.8/asana_preview/models/project_template_base_team.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_template_compact.py` & `asana_preview-1.0.8/asana_preview/models/project_template_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_template_gid_instantiate_project_body.py` & `asana_preview-1.0.8/asana_preview/models/project_template_gid_instantiate_project_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_template_instantiate_project_request.py` & `asana_preview-1.0.8/asana_preview/models/project_template_instantiate_project_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_template_instantiate_project_request_requested_dates.py` & `asana_preview-1.0.8/asana_preview/models/project_template_instantiate_project_request_requested_dates.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_template_instantiate_project_request_requested_roles.py` & `asana_preview-1.0.8/asana_preview/models/project_template_instantiate_project_request_requested_roles.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_template_response.py` & `asana_preview-1.0.8/asana_preview/models/project_template_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_template_response_array.py` & `asana_preview-1.0.8/asana_preview/models/project_template_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/project_template_response_data.py` & `asana_preview-1.0.8/asana_preview/models/project_template_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/projects_body.py` & `asana_preview-1.0.8/asana_preview/models/projects_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/projects_project_gid_body.py` & `asana_preview-1.0.8/asana_preview/models/projects_project_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/remove_custom_field_setting_request.py` & `asana_preview-1.0.8/asana_preview/models/remove_custom_field_setting_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/remove_followers_request.py` & `asana_preview-1.0.8/asana_preview/models/remove_followers_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/remove_members_request.py` & `asana_preview-1.0.8/asana_preview/models/remove_members_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/requested_role_request.py` & `asana_preview-1.0.8/asana_preview/models/requested_role_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/rule_trigger_gid_run_body.py` & `asana_preview-1.0.8/asana_preview/models/rule_trigger_gid_run_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/rule_trigger_request.py` & `asana_preview-1.0.8/asana_preview/models/rule_trigger_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/rule_trigger_response.py` & `asana_preview-1.0.8/asana_preview/models/rule_trigger_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/rule_trigger_response_data.py` & `asana_preview-1.0.8/asana_preview/models/rule_trigger_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/section_base.py` & `asana_preview-1.0.8/asana_preview/models/section_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/section_compact.py` & `asana_preview-1.0.8/asana_preview/models/section_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/section_gid_add_task_body.py` & `asana_preview-1.0.8/asana_preview/models/section_gid_add_task_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/section_request.py` & `asana_preview-1.0.8/asana_preview/models/section_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/section_response.py` & `asana_preview-1.0.8/asana_preview/models/section_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/section_response_array.py` & `asana_preview-1.0.8/asana_preview/models/section_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/section_response_data.py` & `asana_preview-1.0.8/asana_preview/models/section_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/section_task_insert_request.py` & `asana_preview-1.0.8/asana_preview/models/section_task_insert_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/sections_insert_body.py` & `asana_preview-1.0.8/asana_preview/models/sections_insert_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/sections_section_gid_body.py` & `asana_preview-1.0.8/asana_preview/models/sections_section_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/status_update_base.py` & `asana_preview-1.0.8/asana_preview/models/status_update_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/status_update_compact.py` & `asana_preview-1.0.8/asana_preview/models/status_update_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/status_update_request.py` & `asana_preview-1.0.8/asana_preview/models/status_update_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/status_update_response.py` & `asana_preview-1.0.8/asana_preview/models/status_update_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/status_update_response_array.py` & `asana_preview-1.0.8/asana_preview/models/status_update_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/status_update_response_data.py` & `asana_preview-1.0.8/asana_preview/models/status_update_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/status_update_response_parent.py` & `asana_preview-1.0.8/asana_preview/models/status_update_response_parent.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/status_updates_body.py` & `asana_preview-1.0.8/asana_preview/models/status_updates_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/stories_story_gid_body.py` & `asana_preview-1.0.8/asana_preview/models/stories_story_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/story_base.py` & `asana_preview-1.0.8/asana_preview/models/story_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/story_compact.py` & `asana_preview-1.0.8/asana_preview/models/story_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/story_request.py` & `asana_preview-1.0.8/asana_preview/models/story_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/story_response.py` & `asana_preview-1.0.8/asana_preview/models/story_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/story_response_array.py` & `asana_preview-1.0.8/asana_preview/models/story_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/story_response_assignee.py` & `asana_preview-1.0.8/asana_preview/models/story_response_assignee.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/story_response_custom_field.py` & `asana_preview-1.0.8/asana_preview/models/story_response_custom_field.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/story_response_data.py` & `asana_preview-1.0.8/asana_preview/models/story_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/story_response_dates.py` & `asana_preview-1.0.8/asana_preview/models/story_response_dates.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/story_response_old_dates.py` & `asana_preview-1.0.8/asana_preview/models/story_response_old_dates.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/story_response_old_enum_value.py` & `asana_preview-1.0.8/asana_preview/models/story_response_old_enum_value.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/story_response_old_section.py` & `asana_preview-1.0.8/asana_preview/models/story_response_old_section.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/story_response_previews.py` & `asana_preview-1.0.8/asana_preview/models/story_response_previews.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/story_response_project.py` & `asana_preview-1.0.8/asana_preview/models/story_response_project.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/story_response_story.py` & `asana_preview-1.0.8/asana_preview/models/story_response_story.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/story_response_tag.py` & `asana_preview-1.0.8/asana_preview/models/story_response_tag.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/story_response_target.py` & `asana_preview-1.0.8/asana_preview/models/story_response_target.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/story_response_task.py` & `asana_preview-1.0.8/asana_preview/models/story_response_task.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/tag_base.py` & `asana_preview-1.0.8/asana_preview/models/tag_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/tag_compact.py` & `asana_preview-1.0.8/asana_preview/models/tag_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/tag_request.py` & `asana_preview-1.0.8/asana_preview/models/tag_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/tag_response.py` & `asana_preview-1.0.8/asana_preview/models/tag_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/tag_response_array.py` & `asana_preview-1.0.8/asana_preview/models/tag_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/tag_response_data.py` & `asana_preview-1.0.8/asana_preview/models/tag_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/tags_body.py` & `asana_preview-1.0.8/asana_preview/models/tags_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/task_add_followers_request.py` & `asana_preview-1.0.8/asana_preview/models/task_add_followers_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/task_add_project_request.py` & `asana_preview-1.0.8/asana_preview/models/task_add_project_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/task_add_tag_request.py` & `asana_preview-1.0.8/asana_preview/models/task_add_tag_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/task_base.py` & `asana_preview-1.0.8/asana_preview/models/task_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/task_base_completed_by.py` & `asana_preview-1.0.8/asana_preview/models/task_base_completed_by.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/task_base_dependencies.py` & `asana_preview-1.0.8/asana_preview/models/task_base_dependencies.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/task_base_external.py` & `asana_preview-1.0.8/asana_preview/models/task_base_external.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/task_base_memberships.py` & `asana_preview-1.0.8/asana_preview/models/task_base_memberships.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/task_base_section.py` & `asana_preview-1.0.8/asana_preview/models/task_base_section.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/task_compact.py` & `asana_preview-1.0.8/asana_preview/models/task_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/task_count_response.py` & `asana_preview-1.0.8/asana_preview/models/task_count_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/task_count_response_data.py` & `asana_preview-1.0.8/asana_preview/models/task_count_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/task_duplicate_request.py` & `asana_preview-1.0.8/asana_preview/models/task_duplicate_request.py`

 * *Files 17% similar despite different names*

```diff
@@ -70,36 +70,30 @@
 
         self._name = name
 
     @property
     def include(self):
         """Gets the include of this TaskDuplicateRequest.  # noqa: E501
 
-        The fields that will be duplicated to the new task.  # noqa: E501
+        A comma-separated list of fields that will be duplicated to the new task. ##### Fields - assignee - attachments - dates - dependencies - followers - notes - parent - projects - subtasks - tags  # noqa: E501
 
         :return: The include of this TaskDuplicateRequest.  # noqa: E501
         :rtype: str
         """
         return self._include
 
     @include.setter
     def include(self, include):
         """Sets the include of this TaskDuplicateRequest.
 
-        The fields that will be duplicated to the new task.  # noqa: E501
+        A comma-separated list of fields that will be duplicated to the new task. ##### Fields - assignee - attachments - dates - dependencies - followers - notes - parent - projects - subtasks - tags  # noqa: E501
 
         :param include: The include of this TaskDuplicateRequest.  # noqa: E501
         :type: str
         """
-        allowed_values = ["notes", "assignee", "subtasks", "attachments", "tags", "followers", "projects", "dates", "dependencies", "parent"]  # noqa: E501
-        if include not in allowed_values:
-            raise ValueError(
-                "Invalid value for `include` ({0}), must be one of {1}"  # noqa: E501
-                .format(include, allowed_values)
-            )
 
         self._include = include
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `asana_preview-1.0.7/asana_preview/models/task_gid_add_dependencies_body.py` & `asana_preview-1.0.8/asana_preview/models/task_gid_add_dependencies_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/task_gid_add_dependents_body.py` & `asana_preview-1.0.8/asana_preview/models/task_gid_add_dependents_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/task_gid_add_followers_body.py` & `asana_preview-1.0.8/asana_preview/models/task_gid_add_followers_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/task_gid_add_project_body.py` & `asana_preview-1.0.8/asana_preview/models/task_gid_add_project_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/task_gid_add_tag_body.py` & `asana_preview-1.0.8/asana_preview/models/task_gid_add_tag_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/task_gid_duplicate_body.py` & `asana_preview-1.0.8/asana_preview/models/task_gid_duplicate_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/task_gid_remove_dependencies_body.py` & `asana_preview-1.0.8/asana_preview/models/task_gid_remove_dependencies_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/task_gid_remove_dependents_body.py` & `asana_preview-1.0.8/asana_preview/models/task_gid_remove_dependents_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/task_gid_remove_followers_body.py` & `asana_preview-1.0.8/asana_preview/models/task_gid_remove_followers_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/task_gid_remove_project_body.py` & `asana_preview-1.0.8/asana_preview/models/task_gid_remove_project_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/task_gid_remove_tag_body.py` & `asana_preview-1.0.8/asana_preview/models/task_gid_remove_tag_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/task_gid_set_parent_body.py` & `asana_preview-1.0.8/asana_preview/models/task_gid_set_parent_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/task_gid_stories_body.py` & `asana_preview-1.0.8/asana_preview/models/task_gid_stories_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/task_gid_subtasks_body.py` & `asana_preview-1.0.8/asana_preview/models/task_gid_subtasks_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/task_gid_time_tracking_entries_body.py` & `asana_preview-1.0.8/asana_preview/models/task_gid_time_tracking_entries_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/task_remove_followers_request.py` & `asana_preview-1.0.8/asana_preview/models/task_remove_followers_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/task_remove_project_request.py` & `asana_preview-1.0.8/asana_preview/models/task_remove_project_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/task_remove_tag_request.py` & `asana_preview-1.0.8/asana_preview/models/task_remove_tag_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/task_request.py` & `asana_preview-1.0.8/asana_preview/models/task_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/task_response.py` & `asana_preview-1.0.8/asana_preview/models/task_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/task_response_array.py` & `asana_preview-1.0.8/asana_preview/models/task_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/task_response_custom_fields.py` & `asana_preview-1.0.8/asana_preview/models/task_response_custom_fields.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/task_response_data.py` & `asana_preview-1.0.8/asana_preview/models/task_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/task_response_parent.py` & `asana_preview-1.0.8/asana_preview/models/task_response_parent.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/task_response_tags.py` & `asana_preview-1.0.8/asana_preview/models/task_response_tags.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/task_response_workspace.py` & `asana_preview-1.0.8/asana_preview/models/task_response_workspace.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/task_set_parent_request.py` & `asana_preview-1.0.8/asana_preview/models/task_set_parent_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/tasks_body.py` & `asana_preview-1.0.8/asana_preview/models/tasks_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/tasks_task_gid_body.py` & `asana_preview-1.0.8/asana_preview/models/tasks_task_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/team_add_user_request.py` & `asana_preview-1.0.8/asana_preview/models/team_add_user_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/team_base.py` & `asana_preview-1.0.8/asana_preview/models/team_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/team_compact.py` & `asana_preview-1.0.8/asana_preview/models/team_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/team_gid_add_user_body.py` & `asana_preview-1.0.8/asana_preview/models/team_gid_add_user_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/team_gid_projects_body.py` & `asana_preview-1.0.8/asana_preview/models/team_gid_projects_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/team_gid_remove_user_body.py` & `asana_preview-1.0.8/asana_preview/models/team_gid_remove_user_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/team_membership_base.py` & `asana_preview-1.0.8/asana_preview/models/team_membership_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/team_membership_compact.py` & `asana_preview-1.0.8/asana_preview/models/team_membership_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/team_membership_response.py` & `asana_preview-1.0.8/asana_preview/models/team_membership_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/team_membership_response_array.py` & `asana_preview-1.0.8/asana_preview/models/team_membership_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/team_membership_response_data.py` & `asana_preview-1.0.8/asana_preview/models/team_membership_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/team_remove_user_request.py` & `asana_preview-1.0.8/asana_preview/models/team_remove_user_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/team_request.py` & `asana_preview-1.0.8/asana_preview/models/team_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/team_response.py` & `asana_preview-1.0.8/asana_preview/models/team_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/team_response_array.py` & `asana_preview-1.0.8/asana_preview/models/team_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/team_response_data.py` & `asana_preview-1.0.8/asana_preview/models/team_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/team_response_organization.py` & `asana_preview-1.0.8/asana_preview/models/team_response_organization.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/teams_body.py` & `asana_preview-1.0.8/asana_preview/models/teams_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/teams_body1.py` & `asana_preview-1.0.8/asana_preview/models/teams_body1.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/template_role.py` & `asana_preview-1.0.8/asana_preview/models/template_role.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/time_period_base.py` & `asana_preview-1.0.8/asana_preview/models/time_period_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/time_period_compact.py` & `asana_preview-1.0.8/asana_preview/models/time_period_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/time_period_response.py` & `asana_preview-1.0.8/asana_preview/models/time_period_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/time_period_response_array.py` & `asana_preview-1.0.8/asana_preview/models/time_period_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/time_period_response_data.py` & `asana_preview-1.0.8/asana_preview/models/time_period_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/time_tracking_entries_time_tracking_entry_gid_body.py` & `asana_preview-1.0.8/asana_preview/models/time_tracking_entries_time_tracking_entry_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/time_tracking_entry_base.py` & `asana_preview-1.0.8/asana_preview/models/time_tracking_entry_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/time_tracking_entry_base_data.py` & `asana_preview-1.0.8/asana_preview/models/time_tracking_entry_base_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/time_tracking_entry_compact.py` & `asana_preview-1.0.8/asana_preview/models/time_tracking_entry_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/time_tracking_entry_compact_array.py` & `asana_preview-1.0.8/asana_preview/models/time_tracking_entry_compact_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/update_time_tracking_entry_request.py` & `asana_preview-1.0.8/asana_preview/models/update_time_tracking_entry_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/user_base.py` & `asana_preview-1.0.8/asana_preview/models/user_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/user_base_response.py` & `asana_preview-1.0.8/asana_preview/models/user_base_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/user_base_response_data.py` & `asana_preview-1.0.8/asana_preview/models/user_base_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/user_base_response_photo.py` & `asana_preview-1.0.8/asana_preview/models/user_base_response_photo.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/user_compact.py` & `asana_preview-1.0.8/asana_preview/models/user_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/user_request.py` & `asana_preview-1.0.8/asana_preview/models/user_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/user_response.py` & `asana_preview-1.0.8/asana_preview/models/user_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/user_response_array.py` & `asana_preview-1.0.8/asana_preview/models/user_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/user_response_data.py` & `asana_preview-1.0.8/asana_preview/models/user_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/user_task_list_base.py` & `asana_preview-1.0.8/asana_preview/models/user_task_list_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/user_task_list_compact.py` & `asana_preview-1.0.8/asana_preview/models/user_task_list_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/user_task_list_request.py` & `asana_preview-1.0.8/asana_preview/models/user_task_list_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/user_task_list_response.py` & `asana_preview-1.0.8/asana_preview/models/user_task_list_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/user_task_list_response_data.py` & `asana_preview-1.0.8/asana_preview/models/user_task_list_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/webhook_compact.py` & `asana_preview-1.0.8/asana_preview/models/webhook_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/webhook_compact_resource.py` & `asana_preview-1.0.8/asana_preview/models/webhook_compact_resource.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/webhook_filter.py` & `asana_preview-1.0.8/asana_preview/models/webhook_filter.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/webhook_request.py` & `asana_preview-1.0.8/asana_preview/models/webhook_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/webhook_request_filters.py` & `asana_preview-1.0.8/asana_preview/models/webhook_request_filters.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/webhook_response.py` & `asana_preview-1.0.8/asana_preview/models/webhook_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/webhook_response_array.py` & `asana_preview-1.0.8/asana_preview/models/webhook_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/webhook_response_data.py` & `asana_preview-1.0.8/asana_preview/models/webhook_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/webhook_update_request.py` & `asana_preview-1.0.8/asana_preview/models/webhook_update_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/webhooks_body.py` & `asana_preview-1.0.8/asana_preview/models/webhooks_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/webhooks_webhook_gid_body.py` & `asana_preview-1.0.8/asana_preview/models/webhooks_webhook_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/workspace_add_user_request.py` & `asana_preview-1.0.8/asana_preview/models/workspace_add_user_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/workspace_base.py` & `asana_preview-1.0.8/asana_preview/models/workspace_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/workspace_compact.py` & `asana_preview-1.0.8/asana_preview/models/workspace_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/workspace_gid_add_user_body.py` & `asana_preview-1.0.8/asana_preview/models/workspace_gid_add_user_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/workspace_gid_projects_body.py` & `asana_preview-1.0.8/asana_preview/models/workspace_gid_projects_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/workspace_gid_remove_user_body.py` & `asana_preview-1.0.8/asana_preview/models/workspace_gid_remove_user_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/workspace_gid_tags_body.py` & `asana_preview-1.0.8/asana_preview/models/workspace_gid_tags_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/workspace_membership_base.py` & `asana_preview-1.0.8/asana_preview/models/workspace_membership_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/workspace_membership_compact.py` & `asana_preview-1.0.8/asana_preview/models/workspace_membership_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/workspace_membership_request.py` & `asana_preview-1.0.8/asana_preview/models/workspace_membership_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/workspace_membership_response.py` & `asana_preview-1.0.8/asana_preview/models/workspace_membership_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/workspace_membership_response_array.py` & `asana_preview-1.0.8/asana_preview/models/workspace_membership_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/workspace_membership_response_data.py` & `asana_preview-1.0.8/asana_preview/models/workspace_membership_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/workspace_membership_response_user_task_list.py` & `asana_preview-1.0.8/asana_preview/models/workspace_membership_response_user_task_list.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/workspace_membership_response_vacation_dates.py` & `asana_preview-1.0.8/asana_preview/models/workspace_membership_response_vacation_dates.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/workspace_remove_user_request.py` & `asana_preview-1.0.8/asana_preview/models/workspace_remove_user_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/workspace_request.py` & `asana_preview-1.0.8/asana_preview/models/workspace_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/workspace_response.py` & `asana_preview-1.0.8/asana_preview/models/workspace_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/workspace_response_array.py` & `asana_preview-1.0.8/asana_preview/models/workspace_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/workspace_response_data.py` & `asana_preview-1.0.8/asana_preview/models/workspace_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/models/workspaces_workspace_gid_body.py` & `asana_preview-1.0.8/asana_preview/models/workspaces_workspace_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview/rest.py` & `asana_preview-1.0.8/asana_preview/rest.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/asana_preview.egg-info/SOURCES.txt` & `asana_preview-1.0.8/asana_preview.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -170,14 +170,16 @@
 asana_preview/models/goal_response_metric.py
 asana_preview/models/goal_response_team.py
 asana_preview/models/goal_response_time_period.py
 asana_preview/models/goal_response_workspace.py
 asana_preview/models/goal_update_request.py
 asana_preview/models/goals_body.py
 asana_preview/models/goals_goal_gid_body.py
+asana_preview/models/inline_response412.py
+asana_preview/models/inline_response412_errors.py
 asana_preview/models/job_base.py
 asana_preview/models/job_base_new_project.py
 asana_preview/models/job_base_new_project_template.py
 asana_preview/models/job_base_new_task.py
 asana_preview/models/job_compact.py
 asana_preview/models/job_response.py
 asana_preview/models/job_response_data.py
@@ -591,14 +593,16 @@
 test/test_goal_response_team.py
 test/test_goal_response_time_period.py
 test/test_goal_response_workspace.py
 test/test_goal_update_request.py
 test/test_goals_api.py
 test/test_goals_body.py
 test/test_goals_goal_gid_body.py
+test/test_inline_response412.py
+test/test_inline_response412_errors.py
 test/test_job_base.py
 test/test_job_base_new_project.py
 test/test_job_base_new_project_template.py
 test/test_job_base_new_task.py
 test/test_job_compact.py
 test/test_job_response.py
 test/test_job_response_data.py
```

### Comparing `asana_preview-1.0.7/setup.py` & `asana_preview-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "asana_preview"
-VERSION = "1.0.7"
+VERSION = "1.0.8"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `asana_preview-1.0.7/test/test_add_custom_field_setting_request.py` & `asana_preview-1.0.8/test/test_add_custom_field_setting_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_add_followers_request.py` & `asana_preview-1.0.8/test/test_add_followers_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_add_members_request.py` & `asana_preview-1.0.8/test/test_add_members_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_all_of_project_response_owner.py` & `asana_preview-1.0.8/test/test_all_of_project_response_owner.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_all_of_project_template_base_owner.py` & `asana_preview-1.0.8/test/test_all_of_project_template_base_owner.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_all_of_project_template_response_owner.py` & `asana_preview-1.0.8/test/test_all_of_project_template_response_owner.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_all_of_story_response_new_date_value.py` & `asana_preview-1.0.8/test/test_all_of_story_response_new_date_value.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_all_of_story_response_old_date_value.py` & `asana_preview-1.0.8/test/test_all_of_story_response_old_date_value.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_all_of_task_response_assignee_section.py` & `asana_preview-1.0.8/test/test_all_of_task_response_assignee_section.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_all_of_user_task_list_base_owner.py` & `asana_preview-1.0.8/test/test_all_of_user_task_list_base_owner.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_all_of_user_task_list_base_workspace.py` & `asana_preview-1.0.8/test/test_all_of_user_task_list_base_workspace.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_all_of_user_task_list_compact_owner.py` & `asana_preview-1.0.8/test/test_all_of_user_task_list_compact_owner.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_all_of_user_task_list_compact_workspace.py` & `asana_preview-1.0.8/test/test_all_of_user_task_list_compact_workspace.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_all_of_user_task_list_request_owner.py` & `asana_preview-1.0.8/test/test_all_of_user_task_list_request_owner.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_all_of_user_task_list_request_workspace.py` & `asana_preview-1.0.8/test/test_all_of_user_task_list_request_workspace.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_all_of_user_task_list_response_owner.py` & `asana_preview-1.0.8/test/test_all_of_user_task_list_response_owner.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_all_of_user_task_list_response_workspace.py` & `asana_preview-1.0.8/test/test_all_of_user_task_list_response_workspace.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_all_of_workspace_membership_response_user_task_list_owner.py` & `asana_preview-1.0.8/test/test_all_of_workspace_membership_response_user_task_list_owner.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_all_of_workspace_membership_response_user_task_list_workspace.py` & `asana_preview-1.0.8/test/test_all_of_workspace_membership_response_user_task_list_workspace.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_asana_named_resource.py` & `asana_preview-1.0.8/test/test_asana_named_resource.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_asana_named_resource_array.py` & `asana_preview-1.0.8/test/test_asana_named_resource_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_asana_resource.py` & `asana_preview-1.0.8/test/test_asana_resource.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_attachment_base.py` & `asana_preview-1.0.8/test/test_attachment_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_attachment_compact.py` & `asana_preview-1.0.8/test/test_attachment_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_attachment_request.py` & `asana_preview-1.0.8/test/test_attachment_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_attachment_response.py` & `asana_preview-1.0.8/test/test_attachment_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_attachment_response_array.py` & `asana_preview-1.0.8/test/test_attachment_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_attachment_response_data.py` & `asana_preview-1.0.8/test/test_attachment_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_attachment_response_parent.py` & `asana_preview-1.0.8/test/test_attachment_response_parent.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_attachments_api.py` & `asana_preview-1.0.8/test/test_attachments_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_audit_log_api_api.py` & `asana_preview-1.0.8/test/test_audit_log_api_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_audit_log_event.py` & `asana_preview-1.0.8/test/test_audit_log_event.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_audit_log_event_actor.py` & `asana_preview-1.0.8/test/test_audit_log_event_actor.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_audit_log_event_array.py` & `asana_preview-1.0.8/test/test_audit_log_event_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_audit_log_event_context.py` & `asana_preview-1.0.8/test/test_audit_log_event_context.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_audit_log_event_details.py` & `asana_preview-1.0.8/test/test_audit_log_event_details.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_audit_log_event_resource.py` & `asana_preview-1.0.8/test/test_audit_log_event_resource.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_batch_api_api.py` & `asana_preview-1.0.8/test/test_batch_api_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_batch_body.py` & `asana_preview-1.0.8/test/test_batch_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_batch_request.py` & `asana_preview-1.0.8/test/test_batch_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_batch_request_action.py` & `asana_preview-1.0.8/test/test_batch_request_action.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_batch_request_actions.py` & `asana_preview-1.0.8/test/test_batch_request_actions.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_batch_request_options.py` & `asana_preview-1.0.8/test/test_batch_request_options.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_batch_response.py` & `asana_preview-1.0.8/test/test_batch_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_batch_response_array.py` & `asana_preview-1.0.8/test/test_batch_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_create_membership_request.py` & `asana_preview-1.0.8/test/test_create_membership_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_create_time_tracking_entry_request.py` & `asana_preview-1.0.8/test/test_create_time_tracking_entry_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_custom_field_base.py` & `asana_preview-1.0.8/test/test_custom_field_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_custom_field_base_date_value.py` & `asana_preview-1.0.8/test/test_custom_field_base_date_value.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_custom_field_base_enum_options.py` & `asana_preview-1.0.8/test/test_custom_field_base_enum_options.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_custom_field_base_enum_value.py` & `asana_preview-1.0.8/test/test_custom_field_base_enum_value.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_custom_field_compact.py` & `asana_preview-1.0.8/test/test_custom_field_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_custom_field_gid_enum_options_body.py` & `asana_preview-1.0.8/test/test_custom_field_gid_enum_options_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_custom_field_request.py` & `asana_preview-1.0.8/test/test_custom_field_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_custom_field_response.py` & `asana_preview-1.0.8/test/test_custom_field_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_custom_field_response_array.py` & `asana_preview-1.0.8/test/test_custom_field_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_custom_field_response_created_by.py` & `asana_preview-1.0.8/test/test_custom_field_response_created_by.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_custom_field_response_data.py` & `asana_preview-1.0.8/test/test_custom_field_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_custom_field_response_people_value.py` & `asana_preview-1.0.8/test/test_custom_field_response_people_value.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_custom_field_setting_base.py` & `asana_preview-1.0.8/test/test_custom_field_setting_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_custom_field_setting_compact.py` & `asana_preview-1.0.8/test/test_custom_field_setting_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_custom_field_setting_response.py` & `asana_preview-1.0.8/test/test_custom_field_setting_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_custom_field_setting_response_array.py` & `asana_preview-1.0.8/test/test_custom_field_setting_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_custom_field_setting_response_custom_field.py` & `asana_preview-1.0.8/test/test_custom_field_setting_response_custom_field.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_custom_field_setting_response_data.py` & `asana_preview-1.0.8/test/test_custom_field_setting_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_custom_field_setting_response_parent.py` & `asana_preview-1.0.8/test/test_custom_field_setting_response_parent.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_custom_field_setting_response_project.py` & `asana_preview-1.0.8/test/test_custom_field_setting_response_project.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_custom_field_settings_api.py` & `asana_preview-1.0.8/test/test_custom_field_settings_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_custom_fields_api.py` & `asana_preview-1.0.8/test/test_custom_fields_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_custom_fields_body.py` & `asana_preview-1.0.8/test/test_custom_fields_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_custom_fields_custom_field_gid_body.py` & `asana_preview-1.0.8/test/test_custom_fields_custom_field_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_date_variable_compact.py` & `asana_preview-1.0.8/test/test_date_variable_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_date_variable_request.py` & `asana_preview-1.0.8/test/test_date_variable_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_empty_response.py` & `asana_preview-1.0.8/test/test_empty_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_empty_response_data.py` & `asana_preview-1.0.8/test/test_empty_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_enum_option.py` & `asana_preview-1.0.8/test/test_enum_option.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_enum_option_base.py` & `asana_preview-1.0.8/test/test_enum_option_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_enum_option_data.py` & `asana_preview-1.0.8/test/test_enum_option_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_enum_option_insert_request.py` & `asana_preview-1.0.8/test/test_enum_option_insert_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_enum_option_request.py` & `asana_preview-1.0.8/test/test_enum_option_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_enum_options_enum_option_gid_body.py` & `asana_preview-1.0.8/test/test_enum_options_enum_option_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_enum_options_insert_body.py` & `asana_preview-1.0.8/test/test_enum_options_insert_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_error.py` & `asana_preview-1.0.8/test/test_error.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_error_response.py` & `asana_preview-1.0.8/test/test_error_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_error_response_errors.py` & `asana_preview-1.0.8/test/test_error_response_errors.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_event_response.py` & `asana_preview-1.0.8/test/test_event_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_event_response_array.py` & `asana_preview-1.0.8/test/test_event_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_event_response_change.py` & `asana_preview-1.0.8/test/test_event_response_change.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_event_response_parent.py` & `asana_preview-1.0.8/test/test_event_response_parent.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_event_response_resource.py` & `asana_preview-1.0.8/test/test_event_response_resource.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_event_response_user.py` & `asana_preview-1.0.8/test/test_event_response_user.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_events_api.py` & `asana_preview-1.0.8/test/test_events_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goal_add_subgoal_request.py` & `asana_preview-1.0.8/test/test_goal_add_subgoal_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goal_add_supporting_relationship_request.py` & `asana_preview-1.0.8/test/test_goal_add_supporting_relationship_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goal_add_supporting_work_request.py` & `asana_preview-1.0.8/test/test_goal_add_supporting_work_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goal_base.py` & `asana_preview-1.0.8/test/test_goal_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goal_compact.py` & `asana_preview-1.0.8/test/test_goal_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goal_gid_add_followers_body.py` & `asana_preview-1.0.8/test/test_goal_gid_add_followers_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goal_gid_add_supporting_relationship_body.py` & `asana_preview-1.0.8/test/test_goal_gid_add_supporting_relationship_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goal_gid_remove_followers_body.py` & `asana_preview-1.0.8/test/test_goal_gid_remove_followers_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goal_gid_remove_supporting_relationship_body.py` & `asana_preview-1.0.8/test/test_goal_gid_remove_supporting_relationship_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goal_gid_set_metric_body.py` & `asana_preview-1.0.8/test/test_goal_gid_set_metric_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goal_gid_set_metric_current_value_body.py` & `asana_preview-1.0.8/test/test_goal_gid_set_metric_current_value_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goal_membership_base.py` & `asana_preview-1.0.8/test/test_goal_membership_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goal_membership_base_goal.py` & `asana_preview-1.0.8/test/test_goal_membership_base_goal.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goal_membership_compact.py` & `asana_preview-1.0.8/test/test_goal_membership_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goal_membership_response.py` & `asana_preview-1.0.8/test/test_goal_membership_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goal_metric_base.py` & `asana_preview-1.0.8/test/test_goal_metric_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goal_metric_current_value_request.py` & `asana_preview-1.0.8/test/test_goal_metric_current_value_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goal_metric_request.py` & `asana_preview-1.0.8/test/test_goal_metric_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goal_relationship_base.py` & `asana_preview-1.0.8/test/test_goal_relationship_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goal_relationship_base_supported_goal.py` & `asana_preview-1.0.8/test/test_goal_relationship_base_supported_goal.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goal_relationship_base_supporting_resource.py` & `asana_preview-1.0.8/test/test_goal_relationship_base_supporting_resource.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goal_relationship_compact.py` & `asana_preview-1.0.8/test/test_goal_relationship_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goal_relationship_request.py` & `asana_preview-1.0.8/test/test_goal_relationship_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goal_relationship_response.py` & `asana_preview-1.0.8/test/test_goal_relationship_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goal_relationship_response_array.py` & `asana_preview-1.0.8/test/test_goal_relationship_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goal_relationship_response_data.py` & `asana_preview-1.0.8/test/test_goal_relationship_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goal_relationships_api.py` & `asana_preview-1.0.8/test/test_goal_relationships_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goal_relationships_goal_relationship_gid_body.py` & `asana_preview-1.0.8/test/test_goal_relationships_goal_relationship_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goal_remove_subgoal_request.py` & `asana_preview-1.0.8/test/test_goal_remove_subgoal_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goal_remove_supporting_relationship_request.py` & `asana_preview-1.0.8/test/test_goal_remove_supporting_relationship_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goal_request.py` & `asana_preview-1.0.8/test/test_goal_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goal_request_base.py` & `asana_preview-1.0.8/test/test_goal_request_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goal_response.py` & `asana_preview-1.0.8/test/test_goal_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goal_response_array.py` & `asana_preview-1.0.8/test/test_goal_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goal_response_current_status_update.py` & `asana_preview-1.0.8/test/test_goal_response_current_status_update.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goal_response_data.py` & `asana_preview-1.0.8/test/test_goal_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goal_response_likes.py` & `asana_preview-1.0.8/test/test_goal_response_likes.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goal_response_metric.py` & `asana_preview-1.0.8/test/test_goal_response_metric.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goal_response_team.py` & `asana_preview-1.0.8/test/test_goal_response_team.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goal_response_time_period.py` & `asana_preview-1.0.8/test/test_goal_response_time_period.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goal_response_workspace.py` & `asana_preview-1.0.8/test/test_goal_response_workspace.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goal_update_request.py` & `asana_preview-1.0.8/test/test_goal_update_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goals_api.py` & `asana_preview-1.0.8/test/test_goals_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goals_body.py` & `asana_preview-1.0.8/test/test_goals_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_goals_goal_gid_body.py` & `asana_preview-1.0.8/test/test_goals_goal_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_job_base.py` & `asana_preview-1.0.8/test/test_job_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_job_base_new_project.py` & `asana_preview-1.0.8/test/test_job_base_new_project.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_job_base_new_project_template.py` & `asana_preview-1.0.8/test/test_job_base_new_project_template.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_job_base_new_task.py` & `asana_preview-1.0.8/test/test_job_base_new_task.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_job_compact.py` & `asana_preview-1.0.8/test/test_job_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_job_response.py` & `asana_preview-1.0.8/test/test_job_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_job_response_data.py` & `asana_preview-1.0.8/test/test_job_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_jobs_api.py` & `asana_preview-1.0.8/test/test_jobs_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_like.py` & `asana_preview-1.0.8/test/test_like.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_member_compact.py` & `asana_preview-1.0.8/test/test_member_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_membership_request.py` & `asana_preview-1.0.8/test/test_membership_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_membership_response.py` & `asana_preview-1.0.8/test/test_membership_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_membership_response_array.py` & `asana_preview-1.0.8/test/test_membership_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_membership_response_data.py` & `asana_preview-1.0.8/test/test_membership_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_memberships_api.py` & `asana_preview-1.0.8/test/test_memberships_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_memberships_body.py` & `asana_preview-1.0.8/test/test_memberships_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_memberships_membership_gid_body.py` & `asana_preview-1.0.8/test/test_memberships_membership_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_message_base_data.py` & `asana_preview-1.0.8/test/test_message_base_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_modify_dependencies_request.py` & `asana_preview-1.0.8/test/test_modify_dependencies_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_modify_dependents_request.py` & `asana_preview-1.0.8/test/test_modify_dependents_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_organization_export_base.py` & `asana_preview-1.0.8/test/test_organization_export_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_organization_export_compact.py` & `asana_preview-1.0.8/test/test_organization_export_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_organization_export_request.py` & `asana_preview-1.0.8/test/test_organization_export_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_organization_export_response.py` & `asana_preview-1.0.8/test/test_organization_export_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_organization_export_response_data.py` & `asana_preview-1.0.8/test/test_organization_export_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_organization_exports_api.py` & `asana_preview-1.0.8/test/test_organization_exports_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_organization_exports_body.py` & `asana_preview-1.0.8/test/test_organization_exports_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_portfolio_add_item_request.py` & `asana_preview-1.0.8/test/test_portfolio_add_item_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_portfolio_base.py` & `asana_preview-1.0.8/test/test_portfolio_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_portfolio_compact.py` & `asana_preview-1.0.8/test/test_portfolio_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_portfolio_gid_add_custom_field_setting_body.py` & `asana_preview-1.0.8/test/test_portfolio_gid_add_custom_field_setting_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_portfolio_gid_add_item_body.py` & `asana_preview-1.0.8/test/test_portfolio_gid_add_item_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_portfolio_gid_add_members_body.py` & `asana_preview-1.0.8/test/test_portfolio_gid_add_members_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_portfolio_gid_remove_custom_field_setting_body.py` & `asana_preview-1.0.8/test/test_portfolio_gid_remove_custom_field_setting_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_portfolio_gid_remove_item_body.py` & `asana_preview-1.0.8/test/test_portfolio_gid_remove_item_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_portfolio_gid_remove_members_body.py` & `asana_preview-1.0.8/test/test_portfolio_gid_remove_members_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_portfolio_membership_base.py` & `asana_preview-1.0.8/test/test_portfolio_membership_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_portfolio_membership_base_portfolio.py` & `asana_preview-1.0.8/test/test_portfolio_membership_base_portfolio.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_portfolio_membership_compact.py` & `asana_preview-1.0.8/test/test_portfolio_membership_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_portfolio_membership_response.py` & `asana_preview-1.0.8/test/test_portfolio_membership_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_portfolio_membership_response_array.py` & `asana_preview-1.0.8/test/test_portfolio_membership_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_portfolio_membership_response_data.py` & `asana_preview-1.0.8/test/test_portfolio_membership_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_portfolio_memberships_api.py` & `asana_preview-1.0.8/test/test_portfolio_memberships_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_portfolio_remove_item_request.py` & `asana_preview-1.0.8/test/test_portfolio_remove_item_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_portfolio_request.py` & `asana_preview-1.0.8/test/test_portfolio_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_portfolio_response.py` & `asana_preview-1.0.8/test/test_portfolio_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_portfolio_response_array.py` & `asana_preview-1.0.8/test/test_portfolio_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_portfolio_response_current_status_update.py` & `asana_preview-1.0.8/test/test_portfolio_response_current_status_update.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_portfolio_response_custom_field_settings.py` & `asana_preview-1.0.8/test/test_portfolio_response_custom_field_settings.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_portfolio_response_custom_fields.py` & `asana_preview-1.0.8/test/test_portfolio_response_custom_fields.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_portfolio_response_data.py` & `asana_preview-1.0.8/test/test_portfolio_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_portfolio_response_workspace.py` & `asana_preview-1.0.8/test/test_portfolio_response_workspace.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_portfolios_api.py` & `asana_preview-1.0.8/test/test_portfolios_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_portfolios_body.py` & `asana_preview-1.0.8/test/test_portfolios_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_portfolios_portfolio_gid_body.py` & `asana_preview-1.0.8/test/test_portfolios_portfolio_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_preview.py` & `asana_preview-1.0.8/test/test_preview.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_base.py` & `asana_preview-1.0.8/test/test_project_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_base_current_status.py` & `asana_preview-1.0.8/test/test_project_base_current_status.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_base_current_status_update.py` & `asana_preview-1.0.8/test/test_project_base_current_status_update.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_base_workspace.py` & `asana_preview-1.0.8/test/test_project_base_workspace.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_brief_base.py` & `asana_preview-1.0.8/test/test_project_brief_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_brief_compact.py` & `asana_preview-1.0.8/test/test_project_brief_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_brief_request.py` & `asana_preview-1.0.8/test/test_project_brief_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_brief_response.py` & `asana_preview-1.0.8/test/test_project_brief_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_brief_response_data.py` & `asana_preview-1.0.8/test/test_project_brief_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_brief_response_project.py` & `asana_preview-1.0.8/test/test_project_brief_response_project.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_briefs_api.py` & `asana_preview-1.0.8/test/test_project_briefs_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_briefs_project_brief_gid_body.py` & `asana_preview-1.0.8/test/test_project_briefs_project_brief_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_compact.py` & `asana_preview-1.0.8/test/test_project_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_duplicate_request.py` & `asana_preview-1.0.8/test/test_project_duplicate_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_duplicate_request_schedule_dates.py` & `asana_preview-1.0.8/test/test_project_duplicate_request_schedule_dates.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_gid_add_custom_field_setting_body.py` & `asana_preview-1.0.8/test/test_project_gid_add_custom_field_setting_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_gid_add_followers_body.py` & `asana_preview-1.0.8/test/test_project_gid_add_followers_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_gid_add_members_body.py` & `asana_preview-1.0.8/test/test_project_gid_add_members_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_gid_duplicate_body.py` & `asana_preview-1.0.8/test/test_project_gid_duplicate_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_gid_project_briefs_body.py` & `asana_preview-1.0.8/test/test_project_gid_project_briefs_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_gid_project_statuses_body.py` & `asana_preview-1.0.8/test/test_project_gid_project_statuses_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_gid_remove_custom_field_setting_body.py` & `asana_preview-1.0.8/test/test_project_gid_remove_custom_field_setting_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_gid_remove_followers_body.py` & `asana_preview-1.0.8/test/test_project_gid_remove_followers_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_gid_remove_members_body.py` & `asana_preview-1.0.8/test/test_project_gid_remove_members_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_gid_save_as_template_body.py` & `asana_preview-1.0.8/test/test_project_gid_save_as_template_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_gid_sections_body.py` & `asana_preview-1.0.8/test/test_project_gid_sections_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_membership_base.py` & `asana_preview-1.0.8/test/test_project_membership_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_membership_compact.py` & `asana_preview-1.0.8/test/test_project_membership_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_membership_response.py` & `asana_preview-1.0.8/test/test_project_membership_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_membership_response_array.py` & `asana_preview-1.0.8/test/test_project_membership_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_membership_response_data.py` & `asana_preview-1.0.8/test/test_project_membership_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_membership_response_member.py` & `asana_preview-1.0.8/test/test_project_membership_response_member.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_memberships_api.py` & `asana_preview-1.0.8/test/test_project_memberships_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_request.py` & `asana_preview-1.0.8/test/test_project_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_response.py` & `asana_preview-1.0.8/test/test_project_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_response_array.py` & `asana_preview-1.0.8/test/test_project_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_response_completed_by.py` & `asana_preview-1.0.8/test/test_project_response_completed_by.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_response_created_from_template.py` & `asana_preview-1.0.8/test/test_project_response_created_from_template.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_response_data.py` & `asana_preview-1.0.8/test/test_project_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_response_project_brief.py` & `asana_preview-1.0.8/test/test_project_response_project_brief.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_response_team.py` & `asana_preview-1.0.8/test/test_project_response_team.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_save_as_template_request.py` & `asana_preview-1.0.8/test/test_project_save_as_template_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_section_insert_request.py` & `asana_preview-1.0.8/test/test_project_section_insert_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_status_base.py` & `asana_preview-1.0.8/test/test_project_status_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_status_compact.py` & `asana_preview-1.0.8/test/test_project_status_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_status_request.py` & `asana_preview-1.0.8/test/test_project_status_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_status_response.py` & `asana_preview-1.0.8/test/test_project_status_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_status_response_array.py` & `asana_preview-1.0.8/test/test_project_status_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_status_response_data.py` & `asana_preview-1.0.8/test/test_project_status_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_statuses_api.py` & `asana_preview-1.0.8/test/test_project_statuses_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_template_base.py` & `asana_preview-1.0.8/test/test_project_template_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_template_base_requested_dates.py` & `asana_preview-1.0.8/test/test_project_template_base_requested_dates.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_template_base_requested_roles.py` & `asana_preview-1.0.8/test/test_project_template_base_requested_roles.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_template_base_team.py` & `asana_preview-1.0.8/test/test_project_template_base_team.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_template_compact.py` & `asana_preview-1.0.8/test/test_project_template_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_template_gid_instantiate_project_body.py` & `asana_preview-1.0.8/test/test_project_template_gid_instantiate_project_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_template_instantiate_project_request.py` & `asana_preview-1.0.8/test/test_project_template_instantiate_project_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_template_instantiate_project_request_requested_dates.py` & `asana_preview-1.0.8/test/test_project_template_instantiate_project_request_requested_dates.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_template_instantiate_project_request_requested_roles.py` & `asana_preview-1.0.8/test/test_project_template_instantiate_project_request_requested_roles.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_template_response.py` & `asana_preview-1.0.8/test/test_project_template_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_template_response_array.py` & `asana_preview-1.0.8/test/test_project_template_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_template_response_data.py` & `asana_preview-1.0.8/test/test_project_template_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_project_templates_api.py` & `asana_preview-1.0.8/test/test_project_templates_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_projects_api.py` & `asana_preview-1.0.8/test/test_projects_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_projects_body.py` & `asana_preview-1.0.8/test/test_projects_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_projects_project_gid_body.py` & `asana_preview-1.0.8/test/test_projects_project_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_remove_custom_field_setting_request.py` & `asana_preview-1.0.8/test/test_remove_custom_field_setting_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_remove_followers_request.py` & `asana_preview-1.0.8/test/test_remove_followers_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_remove_members_request.py` & `asana_preview-1.0.8/test/test_remove_members_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_requested_role_request.py` & `asana_preview-1.0.8/test/test_requested_role_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_rule_trigger_gid_run_body.py` & `asana_preview-1.0.8/test/test_rule_trigger_gid_run_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_rule_trigger_request.py` & `asana_preview-1.0.8/test/test_rule_trigger_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_rule_trigger_response.py` & `asana_preview-1.0.8/test/test_rule_trigger_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_rule_trigger_response_data.py` & `asana_preview-1.0.8/test/test_rule_trigger_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_rules_api.py` & `asana_preview-1.0.8/test/test_rules_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_section_base.py` & `asana_preview-1.0.8/test/test_section_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_section_compact.py` & `asana_preview-1.0.8/test/test_section_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_section_gid_add_task_body.py` & `asana_preview-1.0.8/test/test_section_gid_add_task_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_section_request.py` & `asana_preview-1.0.8/test/test_section_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_section_response.py` & `asana_preview-1.0.8/test/test_section_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_section_response_array.py` & `asana_preview-1.0.8/test/test_section_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_section_response_data.py` & `asana_preview-1.0.8/test/test_section_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_section_task_insert_request.py` & `asana_preview-1.0.8/test/test_section_task_insert_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_sections_api.py` & `asana_preview-1.0.8/test/test_sections_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_sections_insert_body.py` & `asana_preview-1.0.8/test/test_sections_insert_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_sections_section_gid_body.py` & `asana_preview-1.0.8/test/test_sections_section_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_status_update_base.py` & `asana_preview-1.0.8/test/test_status_update_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_status_update_compact.py` & `asana_preview-1.0.8/test/test_status_update_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_status_update_request.py` & `asana_preview-1.0.8/test/test_status_update_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_status_update_response.py` & `asana_preview-1.0.8/test/test_status_update_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_status_update_response_array.py` & `asana_preview-1.0.8/test/test_status_update_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_status_update_response_data.py` & `asana_preview-1.0.8/test/test_status_update_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_status_update_response_parent.py` & `asana_preview-1.0.8/test/test_status_update_response_parent.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_status_updates_api.py` & `asana_preview-1.0.8/test/test_status_updates_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_status_updates_body.py` & `asana_preview-1.0.8/test/test_status_updates_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_stories_api.py` & `asana_preview-1.0.8/test/test_stories_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_stories_story_gid_body.py` & `asana_preview-1.0.8/test/test_stories_story_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_story_base.py` & `asana_preview-1.0.8/test/test_story_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_story_compact.py` & `asana_preview-1.0.8/test/test_story_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_story_request.py` & `asana_preview-1.0.8/test/test_story_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_story_response.py` & `asana_preview-1.0.8/test/test_story_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_story_response_array.py` & `asana_preview-1.0.8/test/test_story_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_story_response_assignee.py` & `asana_preview-1.0.8/test/test_story_response_assignee.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_story_response_custom_field.py` & `asana_preview-1.0.8/test/test_story_response_custom_field.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_story_response_data.py` & `asana_preview-1.0.8/test/test_story_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_story_response_dates.py` & `asana_preview-1.0.8/test/test_story_response_dates.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_story_response_old_dates.py` & `asana_preview-1.0.8/test/test_story_response_old_dates.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_story_response_old_enum_value.py` & `asana_preview-1.0.8/test/test_story_response_old_enum_value.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_story_response_old_section.py` & `asana_preview-1.0.8/test/test_story_response_old_section.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_story_response_previews.py` & `asana_preview-1.0.8/test/test_story_response_previews.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_story_response_project.py` & `asana_preview-1.0.8/test/test_story_response_project.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_story_response_story.py` & `asana_preview-1.0.8/test/test_story_response_story.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_story_response_tag.py` & `asana_preview-1.0.8/test/test_story_response_tag.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_story_response_target.py` & `asana_preview-1.0.8/test/test_story_response_target.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_story_response_task.py` & `asana_preview-1.0.8/test/test_story_response_task.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_tag_base.py` & `asana_preview-1.0.8/test/test_tag_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_tag_compact.py` & `asana_preview-1.0.8/test/test_tag_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_tag_request.py` & `asana_preview-1.0.8/test/test_tag_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_tag_response.py` & `asana_preview-1.0.8/test/test_tag_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_tag_response_array.py` & `asana_preview-1.0.8/test/test_tag_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_tag_response_data.py` & `asana_preview-1.0.8/test/test_tag_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_tags_api.py` & `asana_preview-1.0.8/test/test_tags_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_tags_body.py` & `asana_preview-1.0.8/test/test_tags_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_task_add_followers_request.py` & `asana_preview-1.0.8/test/test_task_add_followers_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_task_add_project_request.py` & `asana_preview-1.0.8/test/test_task_add_project_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_task_add_tag_request.py` & `asana_preview-1.0.8/test/test_task_add_tag_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_task_base.py` & `asana_preview-1.0.8/test/test_task_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_task_base_completed_by.py` & `asana_preview-1.0.8/test/test_task_base_completed_by.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_task_base_dependencies.py` & `asana_preview-1.0.8/test/test_task_base_dependencies.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_task_base_external.py` & `asana_preview-1.0.8/test/test_task_base_external.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_task_base_memberships.py` & `asana_preview-1.0.8/test/test_task_base_memberships.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_task_base_section.py` & `asana_preview-1.0.8/test/test_task_base_section.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_task_compact.py` & `asana_preview-1.0.8/test/test_task_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_task_count_response.py` & `asana_preview-1.0.8/test/test_task_count_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_task_count_response_data.py` & `asana_preview-1.0.8/test/test_task_count_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_task_duplicate_request.py` & `asana_preview-1.0.8/test/test_task_duplicate_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_task_gid_add_dependencies_body.py` & `asana_preview-1.0.8/test/test_task_gid_add_dependencies_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_task_gid_add_dependents_body.py` & `asana_preview-1.0.8/test/test_task_gid_add_dependents_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_task_gid_add_followers_body.py` & `asana_preview-1.0.8/test/test_task_gid_add_followers_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_task_gid_add_project_body.py` & `asana_preview-1.0.8/test/test_task_gid_add_project_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_task_gid_add_tag_body.py` & `asana_preview-1.0.8/test/test_task_gid_add_tag_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_task_gid_duplicate_body.py` & `asana_preview-1.0.8/test/test_task_gid_duplicate_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_task_gid_remove_dependencies_body.py` & `asana_preview-1.0.8/test/test_task_gid_remove_dependencies_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_task_gid_remove_dependents_body.py` & `asana_preview-1.0.8/test/test_task_gid_remove_dependents_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_task_gid_remove_followers_body.py` & `asana_preview-1.0.8/test/test_task_gid_remove_followers_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_task_gid_remove_project_body.py` & `asana_preview-1.0.8/test/test_task_gid_remove_project_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_task_gid_remove_tag_body.py` & `asana_preview-1.0.8/test/test_task_gid_remove_tag_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_task_gid_set_parent_body.py` & `asana_preview-1.0.8/test/test_task_gid_set_parent_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_task_gid_stories_body.py` & `asana_preview-1.0.8/test/test_task_gid_stories_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_task_gid_subtasks_body.py` & `asana_preview-1.0.8/test/test_task_gid_subtasks_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_task_gid_time_tracking_entries_body.py` & `asana_preview-1.0.8/test/test_task_gid_time_tracking_entries_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_task_remove_followers_request.py` & `asana_preview-1.0.8/test/test_task_remove_followers_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_task_remove_project_request.py` & `asana_preview-1.0.8/test/test_task_remove_project_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_task_remove_tag_request.py` & `asana_preview-1.0.8/test/test_task_remove_tag_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_task_request.py` & `asana_preview-1.0.8/test/test_task_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_task_response.py` & `asana_preview-1.0.8/test/test_task_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_task_response_array.py` & `asana_preview-1.0.8/test/test_task_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_task_response_custom_fields.py` & `asana_preview-1.0.8/test/test_task_response_custom_fields.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_task_response_data.py` & `asana_preview-1.0.8/test/test_task_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_task_response_parent.py` & `asana_preview-1.0.8/test/test_task_response_parent.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_task_response_tags.py` & `asana_preview-1.0.8/test/test_task_response_tags.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_task_response_workspace.py` & `asana_preview-1.0.8/test/test_task_response_workspace.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_task_set_parent_request.py` & `asana_preview-1.0.8/test/test_task_set_parent_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_tasks_api.py` & `asana_preview-1.0.8/test/test_tasks_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_tasks_body.py` & `asana_preview-1.0.8/test/test_tasks_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_tasks_task_gid_body.py` & `asana_preview-1.0.8/test/test_tasks_task_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_team_add_user_request.py` & `asana_preview-1.0.8/test/test_team_add_user_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_team_base.py` & `asana_preview-1.0.8/test/test_team_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_team_compact.py` & `asana_preview-1.0.8/test/test_team_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_team_gid_add_user_body.py` & `asana_preview-1.0.8/test/test_team_gid_add_user_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_team_gid_projects_body.py` & `asana_preview-1.0.8/test/test_team_gid_projects_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_team_gid_remove_user_body.py` & `asana_preview-1.0.8/test/test_team_gid_remove_user_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_team_membership_base.py` & `asana_preview-1.0.8/test/test_team_membership_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_team_membership_compact.py` & `asana_preview-1.0.8/test/test_team_membership_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_team_membership_response.py` & `asana_preview-1.0.8/test/test_team_membership_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_team_membership_response_array.py` & `asana_preview-1.0.8/test/test_team_membership_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_team_membership_response_data.py` & `asana_preview-1.0.8/test/test_team_membership_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_team_memberships_api.py` & `asana_preview-1.0.8/test/test_team_memberships_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_team_remove_user_request.py` & `asana_preview-1.0.8/test/test_team_remove_user_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_team_request.py` & `asana_preview-1.0.8/test/test_team_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_team_response.py` & `asana_preview-1.0.8/test/test_team_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_team_response_array.py` & `asana_preview-1.0.8/test/test_team_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_team_response_data.py` & `asana_preview-1.0.8/test/test_team_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_team_response_organization.py` & `asana_preview-1.0.8/test/test_team_response_organization.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_teams_api.py` & `asana_preview-1.0.8/test/test_teams_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_teams_body.py` & `asana_preview-1.0.8/test/test_teams_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_teams_body1.py` & `asana_preview-1.0.8/test/test_teams_body1.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_template_role.py` & `asana_preview-1.0.8/test/test_template_role.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_time_period_base.py` & `asana_preview-1.0.8/test/test_time_period_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_time_period_compact.py` & `asana_preview-1.0.8/test/test_time_period_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_time_period_response.py` & `asana_preview-1.0.8/test/test_time_period_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_time_period_response_array.py` & `asana_preview-1.0.8/test/test_time_period_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_time_period_response_data.py` & `asana_preview-1.0.8/test/test_time_period_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_time_periods_api.py` & `asana_preview-1.0.8/test/test_time_periods_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_time_tracking_entries_api.py` & `asana_preview-1.0.8/test/test_time_tracking_entries_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_time_tracking_entries_time_tracking_entry_gid_body.py` & `asana_preview-1.0.8/test/test_time_tracking_entries_time_tracking_entry_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_time_tracking_entry_base.py` & `asana_preview-1.0.8/test/test_time_tracking_entry_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_time_tracking_entry_base_data.py` & `asana_preview-1.0.8/test/test_time_tracking_entry_base_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_time_tracking_entry_compact.py` & `asana_preview-1.0.8/test/test_time_tracking_entry_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_time_tracking_entry_compact_array.py` & `asana_preview-1.0.8/test/test_time_tracking_entry_compact_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_typeahead_api.py` & `asana_preview-1.0.8/test/test_typeahead_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_update_time_tracking_entry_request.py` & `asana_preview-1.0.8/test/test_update_time_tracking_entry_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_user_base.py` & `asana_preview-1.0.8/test/test_user_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_user_base_response.py` & `asana_preview-1.0.8/test/test_user_base_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_user_base_response_data.py` & `asana_preview-1.0.8/test/test_user_base_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_user_base_response_photo.py` & `asana_preview-1.0.8/test/test_user_base_response_photo.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_user_compact.py` & `asana_preview-1.0.8/test/test_user_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_user_request.py` & `asana_preview-1.0.8/test/test_user_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_user_response.py` & `asana_preview-1.0.8/test/test_user_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_user_response_array.py` & `asana_preview-1.0.8/test/test_user_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_user_response_data.py` & `asana_preview-1.0.8/test/test_user_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_user_task_list_base.py` & `asana_preview-1.0.8/test/test_user_task_list_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_user_task_list_compact.py` & `asana_preview-1.0.8/test/test_user_task_list_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_user_task_list_request.py` & `asana_preview-1.0.8/test/test_user_task_list_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_user_task_list_response.py` & `asana_preview-1.0.8/test/test_user_task_list_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_user_task_list_response_data.py` & `asana_preview-1.0.8/test/test_user_task_list_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_user_task_lists_api.py` & `asana_preview-1.0.8/test/test_user_task_lists_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_users_api.py` & `asana_preview-1.0.8/test/test_users_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_webhook_compact.py` & `asana_preview-1.0.8/test/test_webhook_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_webhook_compact_resource.py` & `asana_preview-1.0.8/test/test_webhook_compact_resource.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_webhook_filter.py` & `asana_preview-1.0.8/test/test_webhook_filter.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_webhook_request.py` & `asana_preview-1.0.8/test/test_webhook_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_webhook_request_filters.py` & `asana_preview-1.0.8/test/test_webhook_request_filters.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_webhook_response.py` & `asana_preview-1.0.8/test/test_webhook_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_webhook_response_array.py` & `asana_preview-1.0.8/test/test_webhook_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_webhook_response_data.py` & `asana_preview-1.0.8/test/test_webhook_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_webhook_update_request.py` & `asana_preview-1.0.8/test/test_webhook_update_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_webhooks_api.py` & `asana_preview-1.0.8/test/test_webhooks_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_webhooks_body.py` & `asana_preview-1.0.8/test/test_webhooks_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_webhooks_webhook_gid_body.py` & `asana_preview-1.0.8/test/test_webhooks_webhook_gid_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_workspace_add_user_request.py` & `asana_preview-1.0.8/test/test_workspace_add_user_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_workspace_base.py` & `asana_preview-1.0.8/test/test_workspace_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_workspace_compact.py` & `asana_preview-1.0.8/test/test_workspace_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_workspace_gid_add_user_body.py` & `asana_preview-1.0.8/test/test_workspace_gid_add_user_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_workspace_gid_projects_body.py` & `asana_preview-1.0.8/test/test_workspace_gid_projects_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_workspace_gid_remove_user_body.py` & `asana_preview-1.0.8/test/test_workspace_gid_remove_user_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_workspace_gid_tags_body.py` & `asana_preview-1.0.8/test/test_workspace_gid_tags_body.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_workspace_membership_base.py` & `asana_preview-1.0.8/test/test_workspace_membership_base.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_workspace_membership_compact.py` & `asana_preview-1.0.8/test/test_workspace_membership_compact.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_workspace_membership_request.py` & `asana_preview-1.0.8/test/test_workspace_membership_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_workspace_membership_response.py` & `asana_preview-1.0.8/test/test_workspace_membership_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_workspace_membership_response_array.py` & `asana_preview-1.0.8/test/test_workspace_membership_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_workspace_membership_response_data.py` & `asana_preview-1.0.8/test/test_workspace_membership_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_workspace_membership_response_user_task_list.py` & `asana_preview-1.0.8/test/test_workspace_membership_response_user_task_list.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_workspace_membership_response_vacation_dates.py` & `asana_preview-1.0.8/test/test_workspace_membership_response_vacation_dates.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_workspace_memberships_api.py` & `asana_preview-1.0.8/test/test_workspace_memberships_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_workspace_remove_user_request.py` & `asana_preview-1.0.8/test/test_workspace_remove_user_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_workspace_request.py` & `asana_preview-1.0.8/test/test_workspace_request.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_workspace_response.py` & `asana_preview-1.0.8/test/test_workspace_response.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_workspace_response_array.py` & `asana_preview-1.0.8/test/test_workspace_response_array.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_workspace_response_data.py` & `asana_preview-1.0.8/test/test_workspace_response_data.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_workspaces_api.py` & `asana_preview-1.0.8/test/test_workspaces_api.py`

 * *Files identical despite different names*

### Comparing `asana_preview-1.0.7/test/test_workspaces_workspace_gid_body.py` & `asana_preview-1.0.8/test/test_workspaces_workspace_gid_body.py`

 * *Files identical despite different names*

