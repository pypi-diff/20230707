# Comparing `tmp/pulumi_akamai-4.6.0a1688398728.tar.gz` & `tmp/pulumi_akamai-5.0.0a1688662273.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_akamai-4.6.0a1688398728.tar", last modified: Mon Jul  3 15:43:49 2023, max compression
+gzip compressed data, was "pulumi_akamai-5.0.0a1688662273.tar", last modified: Thu Jul  6 16:58:20 2023, max compression
```

## Comparing `pulumi_akamai-4.6.0a1688398728.tar` & `pulumi_akamai-5.0.0a1688662273.tar`

### file list

```diff
@@ -1,247 +1,276 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:43:49.942645 pulumi_akamai-4.6.0a1688398728/
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-03 15:43:49.942645 pulumi_akamai-4.6.0a1688398728/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:43:49.934645 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/
--rw-r--r--   0 runner    (1001) docker     (123)    27506 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1554270 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    21333 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_activations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10773 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_advanced_settings_evasive_path_match.py
--rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_advanced_settings_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_advanced_settings_pragma_header.py
--rw-r--r--   0 runner    (1001) docker     (123)    15113 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_advanced_settings_prefetch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11236 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_api_constraints_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)    12592 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_api_request_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)    14951 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_attack_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    11212 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_by_pass_network_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    20518 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9676 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_configuration_rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_custom_deny.py
--rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_custom_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    12783 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_custom_rule_action.py
--rw-r--r--   0 runner    (1001) docker     (123)    17001 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_eval_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    13089 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_eval_penalty_box.py
--rw-r--r--   0 runner    (1001) docker     (123)    14538 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_eval_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    17481 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_ip_geo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_ip_geo_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9253 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_malware_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    14854 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_malware_policy_action.py
--rw-r--r--   0 runner    (1001) docker     (123)    10858 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_malware_policy_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11026 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_malware_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_match_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_match_target_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)    12987 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_penalty_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_rate_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    14508 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_rate_policy_action.py
--rw-r--r--   0 runner    (1001) docker     (123)    10433 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_rate_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_reputation_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    12618 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_reputation_profile_action.py
--rw-r--r--   0 runner    (1001) docker     (123)    14387 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_reputation_profile_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_reputation_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)    14063 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    13718 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_rule_upgrade.py
--rw-r--r--   0 runner    (1001) docker     (123)    17082 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_security_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_security_policy_rename.py
--rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_selected_hostnames.py
--rw-r--r--   0 runner    (1001) docker     (123)    17536 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_siem_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    19373 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_slow_post.py
--rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_slow_post_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_threat_intel.py
--rw-r--r--   0 runner    (1001) docker     (123)     9060 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_version_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    15899 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_waf_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    10910 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_waf_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)    13004 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_wap_selected_hostnames.py
--rw-r--r--   0 runner    (1001) docker     (123)    11169 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/appsec_advanced_settings_attack_payload_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    11290 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/appsec_advanced_settings_request_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    19609 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/cloudlets_application_load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/cloudlets_application_load_balancer_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19277 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/cloudlets_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    13766 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/cloudlets_policy_activation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:43:49.938645 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11104 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    14717 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/cp_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    47004 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/cps_dv_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/cps_dv_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    44892 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/cps_third_party_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (123)    27347 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/cps_upload_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)    58490 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/datastream.py
--rw-r--r--   0 runner    (1001) docker     (123)    78637 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/dns_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    21162 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/dns_zone.py
--rw-r--r--   0 runner    (1001) docker     (123)    22811 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edge_host_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    18627 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edge_kv.py
--rw-r--r--   0 runner    (1001) docker     (123)    15813 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edge_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edge_workers_activation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:43:49.938645 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edgedns/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edgedns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edgedns/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    78911 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edgedns/dns_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    21414 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edgedns/dns_zone.py
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edgedns/get_authorities_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edgedns/get_dns_record_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edgedns/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edgekv_group_items.py
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_advanced_settings_evasive_path_match.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_advanced_settings_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_advanced_settings_pragma_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_advanced_settings_prefetch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_api_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_api_request_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_attack_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_bypass_network_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_configuration_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_contracts_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_custom_deny.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_custom_rule_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_custom_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_eval_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_eval_penalty_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_eval_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_export_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_failover_hostnames.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_hostname_coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_hostname_coverage_match_targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_hostname_coverage_overlapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_ip_geo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_malware_content_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_malware_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_malware_policy_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_match_targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_penalty_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_rate_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_rate_policy_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_reputation_profile_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_reputation_profile_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_reputation_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_rule_upgrade_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_security_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9257 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_security_policy_protections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_selectable_hostnames.py
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_selected_hostnames.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_siem_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_siem_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_slow_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_threat_intel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_tuning_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_version_notes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_waf_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_wap_selected_hostnames.py
--rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_appsec_advanced_settings_attack_payload_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_appsec_advanced_settings_request_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_authorities_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cloudlets_api_prioritization_match_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     8855 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cloudlets_application_load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cloudlets_application_load_balancer_match_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cloudlets_audience_segmentation_match_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cloudlets_edge_redirector_match_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cloudlets_forward_rewrite_match_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cloudlets_phased_release_match_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cloudlets_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cloudlets_request_control_match_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cloudlets_visitor_prioritization_match_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cp_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cps_csr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cps_deployments.py
--rw-r--r--   0 runner    (1001) docker     (123)    11639 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cps_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cps_enrollments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cps_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_datastream_activation_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_datastream_dataset_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_datastreams.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_dns_record_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_edge_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_edge_worker_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_edge_workers_property_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_edge_workers_resource_tier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_edgekv_group_items.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_edgekv_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_gtm_default_datacenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_iam_contact_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_iam_countries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_iam_grantable_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_iam_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_iam_states.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_iam_supported_langs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_iam_timeout_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_iam_timezones.py
--rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_network_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_properties_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_hostnames.py
--rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_include.py
--rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_include_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_include_parents.py
--rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_include_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_includes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_products.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_rule_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_rules_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_rules_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    11604 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/gtm_asmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    11692 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/gtm_cidrmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    29745 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/gtm_datacenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    44869 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/gtm_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    11648 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/gtm_geomap.py
--rw-r--r--   0 runner    (1001) docker     (123)    55296 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/gtm_property.py
--rw-r--r--   0 runner    (1001) docker     (123)    26762 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/gtm_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    10813 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/iam_blocked_user_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/iam_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/iam_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    48065 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/iam_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    20282 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/network_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    18214 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/network_list_activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/network_list_description.py
--rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/network_list_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)  1210373 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:43:49.938645 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/properties/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23565 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/properties/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14967 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/properties/cp_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    23127 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/properties/edge_host_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/properties/get_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/properties/get_cp_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/properties/get_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/properties/get_property_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    21783 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/properties/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    42326 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/properties/property.py
--rw-r--r--   0 runner    (1001) docker     (123)    27649 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/properties/property_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)    42054 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/property.py
--rw-r--r--   0 runner    (1001) docker     (123)    27267 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/property_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)    22902 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/property_include.py
--rw-r--r--   0 runner    (1001) docker     (123)    24971 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/property_include_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)    22466 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:43:49.942645 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/trafficmanagement/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/trafficmanagement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28679 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/trafficmanagement/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/trafficmanagement/get_gtm_default_datacenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/trafficmanagement/gtm_a_smap.py
--rw-r--r--   0 runner    (1001) docker     (123)    12007 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/trafficmanagement/gtm_cidrmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    30093 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/trafficmanagement/gtm_datacenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    45173 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/trafficmanagement/gtm_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    11952 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/trafficmanagement/gtm_geomap.py
--rw-r--r--   0 runner    (1001) docker     (123)    55622 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/trafficmanagement/gtm_property.py
--rw-r--r--   0 runner    (1001) docker     (123)    27088 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/trafficmanagement/gtm_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    26637 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/trafficmanagement/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:43:49.938645 pulumi_akamai-4.6.0a1688398728/pulumi_akamai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9865 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 15:43:49.942645 pulumi_akamai-4.6.0a1688398728/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:58:20.785963 pulumi_akamai-5.0.0a1688662273/
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-06 16:58:20.785963 pulumi_akamai-5.0.0a1688662273/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:58:20.785963 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/
+-rw-r--r--   0 runner    (1001) docker     (123)    31717 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1564777 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23160 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10773 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_advanced_settings_evasive_path_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_advanced_settings_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_advanced_settings_pragma_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15113 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_advanced_settings_prefetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11236 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_api_constraints_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12592 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_api_request_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14951 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_attack_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11212 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_by_pass_network_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20518 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9676 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_configuration_rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_custom_deny.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_custom_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12783 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_custom_rule_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17001 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_eval_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13089 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_eval_penalty_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14538 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_eval_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17481 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_ip_geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_ip_geo_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9253 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_malware_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14854 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_malware_policy_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10858 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_malware_policy_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11026 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_malware_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_match_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_match_target_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12987 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_penalty_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_rate_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14508 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_rate_policy_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10433 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_rate_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_reputation_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12618 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_reputation_profile_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14387 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_reputation_profile_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_reputation_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14063 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13718 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_rule_upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17082 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_security_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_security_policy_rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_selected_hostnames.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17536 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_siem_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19373 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_slow_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_slow_post_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_threat_intel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9060 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_version_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15899 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_waf_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10910 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_waf_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13004 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_wap_selected_hostnames.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11169 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/appsec_advanced_settings_attack_payload_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11290 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/appsec_advanced_settings_request_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10456 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/botman_akamai_bot_category_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/botman_bot_analytics_cookie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8848 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/botman_bot_category_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10194 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/botman_bot_detection_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8901 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/botman_bot_management_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/botman_challenge_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7531 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/botman_challenge_interception_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/botman_client_side_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/botman_conditional_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/botman_custom_bot_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10456 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/botman_custom_bot_category_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/botman_custom_bot_category_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/botman_custom_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/botman_custom_defined_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/botman_custom_deny_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/botman_javascript_injection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/botman_recategorized_akamai_defined_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7954 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/botman_serve_alternate_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/botman_transactional_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/botman_transactional_endpoint_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19609 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/cloudlets_application_load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/cloudlets_application_load_balancer_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19277 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/cloudlets_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13766 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/cloudlets_policy_activation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:58:20.785963 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11104 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16454 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/cp_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47610 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/cps_dv_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/cps_dv_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44892 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/cps_third_party_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27347 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/cps_upload_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58490 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/datastream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78637 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/dns_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21162 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/dns_zone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24548 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/edge_host_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19695 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/edge_kv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15813 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/edge_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/edge_workers_activation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:58:20.785963 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/edgedns/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/edgedns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/edgedns/get_authorities_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/edgedns/get_dns_record_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/edgekv_group_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_advanced_settings_evasive_path_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_advanced_settings_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_advanced_settings_pragma_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_advanced_settings_prefetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_api_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_api_request_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_attack_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_bypass_network_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_configuration_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_contracts_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_custom_deny.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_custom_rule_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_custom_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_eval_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_eval_penalty_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_eval_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_export_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_failover_hostnames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_hostname_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_hostname_coverage_match_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_hostname_coverage_overlapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_ip_geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_malware_content_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_malware_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_malware_policy_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_match_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_penalty_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_rate_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_rate_policy_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_reputation_profile_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_reputation_profile_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_reputation_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_rule_upgrade_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_security_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_security_policy_protections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_selectable_hostnames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_selected_hostnames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_siem_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_siem_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_slow_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_threat_intel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_tuning_recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_version_notes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_waf_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_wap_selected_hostnames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_appsec_advanced_settings_attack_payload_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_appsec_advanced_settings_request_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_authorities_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_botman_akamai_bot_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_botman_akamai_bot_category_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_botman_akamai_defined_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_botman_bot_analytics_cookie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_botman_bot_analytics_cookie_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_botman_bot_category_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_botman_bot_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_botman_bot_detection_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_botman_bot_endpoint_coverage_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_botman_bot_management_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_botman_challenge_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_botman_challenge_interception_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_botman_client_side_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_botman_conditional_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_botman_custom_bot_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_botman_custom_bot_category_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_botman_custom_bot_category_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_botman_custom_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_botman_custom_defined_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_botman_custom_deny_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_botman_javascript_injection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_botman_recategorized_akamai_defined_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_botman_response_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_botman_serve_alternate_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_botman_transactional_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_botman_transactional_endpoint_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_cloudlets_api_prioritization_match_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_cloudlets_application_load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_cloudlets_application_load_balancer_match_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_cloudlets_audience_segmentation_match_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_cloudlets_edge_redirector_match_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_cloudlets_forward_rewrite_match_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_cloudlets_phased_release_match_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_cloudlets_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_cloudlets_request_control_match_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_cloudlets_visitor_prioritization_match_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_cp_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_cps_csr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_cps_deployments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11939 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_cps_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_cps_enrollments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_cps_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_datastream_activation_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_datastream_dataset_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_datastreams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_dns_record_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_edge_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_edge_worker_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_edge_workers_property_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_edge_workers_resource_tier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_edgekv_group_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_edgekv_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_gtm_datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_gtm_datacenters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_gtm_default_datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_iam_contact_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_iam_countries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_iam_grantable_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_iam_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_iam_states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_iam_supported_langs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_iam_timeout_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_iam_timezones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_network_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_properties_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_property_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_property_hostnames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_property_include.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_property_include_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_property_include_parents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_property_include_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_property_includes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_property_products.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_property_rule_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_property_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_property_rules_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_property_rules_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11604 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/gtm_asmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11692 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/gtm_cidrmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29745 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/gtm_datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44869 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/gtm_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11648 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/gtm_geomap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55296 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/gtm_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26762 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/gtm_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10813 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/iam_blocked_user_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/iam_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/iam_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48609 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/iam_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20282 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/network_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18805 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/network_list_activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/network_list_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/network_list_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1231072 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:58:20.785963 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/properties/get_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/properties/get_cp_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/properties/get_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/properties/get_property_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47346 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28470 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/property_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22902 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/property_include.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24971 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/property_include_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25793 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:58:20.785963 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/trafficmanagement/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/trafficmanagement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai/trafficmanagement/get_gtm_default_datacenter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:58:20.785963 pulumi_akamai-5.0.0a1688662273/pulumi_akamai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11411 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/pulumi_akamai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 16:58:20.785963 pulumi_akamai-5.0.0a1688662273/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-06 16:58:20.000000 pulumi_akamai-5.0.0a1688662273/setup.py
```

### Comparing `pulumi_akamai-4.6.0a1688398728/PKG-INFO` & `pulumi_akamai-5.0.0a1688662273/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_akamai
-Version: 4.6.0a1688398728
+Version: 5.0.0a1688662273
 Summary: A Pulumi package for creating and managing akamai cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-akamai
 Keywords: pulumi akamai
 Platform: UNKNOWN
 Requires-Python: >=3.7
@@ -34,15 +34,15 @@
 
     $ pip install pulumi_akamai
 
 ### Go
 
 To use from Go, use `go get` to grab the latest version of the library
 
-    $ go get github.com/pulumi/pulumi-akamai/sdk/v4
+    $ go get github.com/pulumi/pulumi-akamai/sdk/v5
 
 ### .NET
 
 To use from .NET, install using `dotnet add package`:
 
     $ dotnet add package Pulumi.Akamai
```

### Comparing `pulumi_akamai-4.6.0a1688398728/README.md` & `pulumi_akamai-5.0.0a1688662273/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     $ pip install pulumi_akamai
 
 ### Go
 
 To use from Go, use `go get` to grab the latest version of the library
 
-    $ go get github.com/pulumi/pulumi-akamai/sdk/v4
+    $ go get github.com/pulumi/pulumi-akamai/sdk/v5
 
 ### .NET
 
 To use from .NET, install using `dotnet add package`:
 
     $ dotnet add package Pulumi.Akamai
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/__init__.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -50,14 +50,34 @@
 from .app_sec_threat_intel import *
 from .app_sec_version_nodes import *
 from .app_sec_waf_mode import *
 from .app_sec_waf_protection import *
 from .app_sec_wap_selected_hostnames import *
 from .appsec_advanced_settings_attack_payload_logging import *
 from .appsec_advanced_settings_request_body import *
+from .botman_akamai_bot_category_action import *
+from .botman_bot_analytics_cookie import *
+from .botman_bot_category_exception import *
+from .botman_bot_detection_action import *
+from .botman_bot_management_settings import *
+from .botman_challenge_action import *
+from .botman_challenge_interception_rules import *
+from .botman_client_side_security import *
+from .botman_conditional_action import *
+from .botman_custom_bot_category import *
+from .botman_custom_bot_category_action import *
+from .botman_custom_bot_category_sequence import *
+from .botman_custom_client import *
+from .botman_custom_defined_bot import *
+from .botman_custom_deny_action import *
+from .botman_javascript_injection import *
+from .botman_recategorized_akamai_defined_bot import *
+from .botman_serve_alternate_action import *
+from .botman_transactional_endpoint import *
+from .botman_transactional_endpoint_protection import *
 from .cloudlets_application_load_balancer import *
 from .cloudlets_application_load_balancer_activation import *
 from .cloudlets_policy import *
 from .cloudlets_policy_activation import *
 from .cp_code import *
 from .cps_dv_enrollment import *
 from .cps_dv_validation import *
@@ -118,14 +138,40 @@
 from .get_app_sec_tuning_recommendations import *
 from .get_app_sec_version_notes import *
 from .get_app_sec_waf_mode import *
 from .get_app_sec_wap_selected_hostnames import *
 from .get_appsec_advanced_settings_attack_payload_logging import *
 from .get_appsec_advanced_settings_request_body import *
 from .get_authorities_set import *
+from .get_botman_akamai_bot_category import *
+from .get_botman_akamai_bot_category_action import *
+from .get_botman_akamai_defined_bot import *
+from .get_botman_bot_analytics_cookie import *
+from .get_botman_bot_analytics_cookie_values import *
+from .get_botman_bot_category_exception import *
+from .get_botman_bot_detection import *
+from .get_botman_bot_detection_action import *
+from .get_botman_bot_endpoint_coverage_report import *
+from .get_botman_bot_management_settings import *
+from .get_botman_challenge_action import *
+from .get_botman_challenge_interception_rules import *
+from .get_botman_client_side_security import *
+from .get_botman_conditional_action import *
+from .get_botman_custom_bot_category import *
+from .get_botman_custom_bot_category_action import *
+from .get_botman_custom_bot_category_sequence import *
+from .get_botman_custom_client import *
+from .get_botman_custom_defined_bot import *
+from .get_botman_custom_deny_action import *
+from .get_botman_javascript_injection import *
+from .get_botman_recategorized_akamai_defined_bot import *
+from .get_botman_response_action import *
+from .get_botman_serve_alternate_action import *
+from .get_botman_transactional_endpoint import *
+from .get_botman_transactional_endpoint_protection import *
 from .get_cloudlets_api_prioritization_match_rule import *
 from .get_cloudlets_application_load_balancer import *
 from .get_cloudlets_application_load_balancer_match_rule import *
 from .get_cloudlets_audience_segmentation_match_rule import *
 from .get_cloudlets_edge_redirector_match_rule import *
 from .get_cloudlets_forward_rewrite_match_rule import *
 from .get_cloudlets_phased_release_match_rule import *
@@ -148,14 +194,16 @@
 from .get_edge_worker_activation import *
 from .get_edge_workers_property_rules import *
 from .get_edge_workers_resource_tier import *
 from .get_edgekv_group_items import *
 from .get_edgekv_groups import *
 from .get_group import *
 from .get_groups import *
+from .get_gtm_datacenter import *
+from .get_gtm_datacenters import *
 from .get_gtm_default_datacenter import *
 from .get_iam_contact_types import *
 from .get_iam_countries import *
 from .get_iam_grantable_roles import *
 from .get_iam_roles import *
 from .get_iam_states import *
 from .get_iam_supported_langs import *
@@ -217,30 +265,14 @@
     trafficmanagement = _utilities.lazy_import('pulumi_akamai.trafficmanagement')
 
 _utilities.register(
     resource_modules="""
 [
  {
   "pkg": "akamai",
-  "mod": "edgedns/dnsRecord",
-  "fqn": "pulumi_akamai.edgedns",
-  "classes": {
-   "akamai:edgedns/dnsRecord:DnsRecord": "DnsRecord"
-  }
- },
- {
-  "pkg": "akamai",
-  "mod": "edgedns/dnsZone",
-  "fqn": "pulumi_akamai.edgedns",
-  "classes": {
-   "akamai:edgedns/dnsZone:DnsZone": "DnsZone"
-  }
- },
- {
-  "pkg": "akamai",
   "mod": "index/appSecActivations",
   "fqn": "pulumi_akamai",
   "classes": {
    "akamai:index/appSecActivations:AppSecActivations": "AppSecActivations"
   }
  },
  {
@@ -625,14 +657,174 @@
   "fqn": "pulumi_akamai",
   "classes": {
    "akamai:index/appsecAdvancedSettingsRequestBody:AppsecAdvancedSettingsRequestBody": "AppsecAdvancedSettingsRequestBody"
   }
  },
  {
   "pkg": "akamai",
+  "mod": "index/botmanAkamaiBotCategoryAction",
+  "fqn": "pulumi_akamai",
+  "classes": {
+   "akamai:index/botmanAkamaiBotCategoryAction:BotmanAkamaiBotCategoryAction": "BotmanAkamaiBotCategoryAction"
+  }
+ },
+ {
+  "pkg": "akamai",
+  "mod": "index/botmanBotAnalyticsCookie",
+  "fqn": "pulumi_akamai",
+  "classes": {
+   "akamai:index/botmanBotAnalyticsCookie:BotmanBotAnalyticsCookie": "BotmanBotAnalyticsCookie"
+  }
+ },
+ {
+  "pkg": "akamai",
+  "mod": "index/botmanBotCategoryException",
+  "fqn": "pulumi_akamai",
+  "classes": {
+   "akamai:index/botmanBotCategoryException:BotmanBotCategoryException": "BotmanBotCategoryException"
+  }
+ },
+ {
+  "pkg": "akamai",
+  "mod": "index/botmanBotDetectionAction",
+  "fqn": "pulumi_akamai",
+  "classes": {
+   "akamai:index/botmanBotDetectionAction:BotmanBotDetectionAction": "BotmanBotDetectionAction"
+  }
+ },
+ {
+  "pkg": "akamai",
+  "mod": "index/botmanBotManagementSettings",
+  "fqn": "pulumi_akamai",
+  "classes": {
+   "akamai:index/botmanBotManagementSettings:BotmanBotManagementSettings": "BotmanBotManagementSettings"
+  }
+ },
+ {
+  "pkg": "akamai",
+  "mod": "index/botmanChallengeAction",
+  "fqn": "pulumi_akamai",
+  "classes": {
+   "akamai:index/botmanChallengeAction:BotmanChallengeAction": "BotmanChallengeAction"
+  }
+ },
+ {
+  "pkg": "akamai",
+  "mod": "index/botmanChallengeInterceptionRules",
+  "fqn": "pulumi_akamai",
+  "classes": {
+   "akamai:index/botmanChallengeInterceptionRules:BotmanChallengeInterceptionRules": "BotmanChallengeInterceptionRules"
+  }
+ },
+ {
+  "pkg": "akamai",
+  "mod": "index/botmanClientSideSecurity",
+  "fqn": "pulumi_akamai",
+  "classes": {
+   "akamai:index/botmanClientSideSecurity:BotmanClientSideSecurity": "BotmanClientSideSecurity"
+  }
+ },
+ {
+  "pkg": "akamai",
+  "mod": "index/botmanConditionalAction",
+  "fqn": "pulumi_akamai",
+  "classes": {
+   "akamai:index/botmanConditionalAction:BotmanConditionalAction": "BotmanConditionalAction"
+  }
+ },
+ {
+  "pkg": "akamai",
+  "mod": "index/botmanCustomBotCategory",
+  "fqn": "pulumi_akamai",
+  "classes": {
+   "akamai:index/botmanCustomBotCategory:BotmanCustomBotCategory": "BotmanCustomBotCategory"
+  }
+ },
+ {
+  "pkg": "akamai",
+  "mod": "index/botmanCustomBotCategoryAction",
+  "fqn": "pulumi_akamai",
+  "classes": {
+   "akamai:index/botmanCustomBotCategoryAction:BotmanCustomBotCategoryAction": "BotmanCustomBotCategoryAction"
+  }
+ },
+ {
+  "pkg": "akamai",
+  "mod": "index/botmanCustomBotCategorySequence",
+  "fqn": "pulumi_akamai",
+  "classes": {
+   "akamai:index/botmanCustomBotCategorySequence:BotmanCustomBotCategorySequence": "BotmanCustomBotCategorySequence"
+  }
+ },
+ {
+  "pkg": "akamai",
+  "mod": "index/botmanCustomClient",
+  "fqn": "pulumi_akamai",
+  "classes": {
+   "akamai:index/botmanCustomClient:BotmanCustomClient": "BotmanCustomClient"
+  }
+ },
+ {
+  "pkg": "akamai",
+  "mod": "index/botmanCustomDefinedBot",
+  "fqn": "pulumi_akamai",
+  "classes": {
+   "akamai:index/botmanCustomDefinedBot:BotmanCustomDefinedBot": "BotmanCustomDefinedBot"
+  }
+ },
+ {
+  "pkg": "akamai",
+  "mod": "index/botmanCustomDenyAction",
+  "fqn": "pulumi_akamai",
+  "classes": {
+   "akamai:index/botmanCustomDenyAction:BotmanCustomDenyAction": "BotmanCustomDenyAction"
+  }
+ },
+ {
+  "pkg": "akamai",
+  "mod": "index/botmanJavascriptInjection",
+  "fqn": "pulumi_akamai",
+  "classes": {
+   "akamai:index/botmanJavascriptInjection:BotmanJavascriptInjection": "BotmanJavascriptInjection"
+  }
+ },
+ {
+  "pkg": "akamai",
+  "mod": "index/botmanRecategorizedAkamaiDefinedBot",
+  "fqn": "pulumi_akamai",
+  "classes": {
+   "akamai:index/botmanRecategorizedAkamaiDefinedBot:BotmanRecategorizedAkamaiDefinedBot": "BotmanRecategorizedAkamaiDefinedBot"
+  }
+ },
+ {
+  "pkg": "akamai",
+  "mod": "index/botmanServeAlternateAction",
+  "fqn": "pulumi_akamai",
+  "classes": {
+   "akamai:index/botmanServeAlternateAction:BotmanServeAlternateAction": "BotmanServeAlternateAction"
+  }
+ },
+ {
+  "pkg": "akamai",
+  "mod": "index/botmanTransactionalEndpoint",
+  "fqn": "pulumi_akamai",
+  "classes": {
+   "akamai:index/botmanTransactionalEndpoint:BotmanTransactionalEndpoint": "BotmanTransactionalEndpoint"
+  }
+ },
+ {
+  "pkg": "akamai",
+  "mod": "index/botmanTransactionalEndpointProtection",
+  "fqn": "pulumi_akamai",
+  "classes": {
+   "akamai:index/botmanTransactionalEndpointProtection:BotmanTransactionalEndpointProtection": "BotmanTransactionalEndpointProtection"
+  }
+ },
+ {
+  "pkg": "akamai",
   "mod": "index/cloudletsApplicationLoadBalancer",
   "fqn": "pulumi_akamai",
   "classes": {
    "akamai:index/cloudletsApplicationLoadBalancer:CloudletsApplicationLoadBalancer": "CloudletsApplicationLoadBalancer"
   }
  },
  {
@@ -910,102 +1102,14 @@
  {
   "pkg": "akamai",
   "mod": "index/propertyIncludeActivation",
   "fqn": "pulumi_akamai",
   "classes": {
    "akamai:index/propertyIncludeActivation:PropertyIncludeActivation": "PropertyIncludeActivation"
   }
- },
- {
-  "pkg": "akamai",
-  "mod": "properties/cpCode",
-  "fqn": "pulumi_akamai.properties",
-  "classes": {
-   "akamai:properties/cpCode:CpCode": "CpCode"
-  }
- },
- {
-  "pkg": "akamai",
-  "mod": "properties/edgeHostName",
-  "fqn": "pulumi_akamai.properties",
-  "classes": {
-   "akamai:properties/edgeHostName:EdgeHostName": "EdgeHostName"
-  }
- },
- {
-  "pkg": "akamai",
-  "mod": "properties/property",
-  "fqn": "pulumi_akamai.properties",
-  "classes": {
-   "akamai:properties/property:Property": "Property"
-  }
- },
- {
-  "pkg": "akamai",
-  "mod": "properties/propertyActivation",
-  "fqn": "pulumi_akamai.properties",
-  "classes": {
-   "akamai:properties/propertyActivation:PropertyActivation": "PropertyActivation"
-  }
- },
- {
-  "pkg": "akamai",
-  "mod": "trafficmanagement/gtmASmap",
-  "fqn": "pulumi_akamai.trafficmanagement",
-  "classes": {
-   "akamai:trafficmanagement/gtmASmap:GtmASmap": "GtmASmap"
-  }
- },
- {
-  "pkg": "akamai",
-  "mod": "trafficmanagement/gtmCidrmap",
-  "fqn": "pulumi_akamai.trafficmanagement",
-  "classes": {
-   "akamai:trafficmanagement/gtmCidrmap:GtmCidrmap": "GtmCidrmap"
-  }
- },
- {
-  "pkg": "akamai",
-  "mod": "trafficmanagement/gtmDatacenter",
-  "fqn": "pulumi_akamai.trafficmanagement",
-  "classes": {
-   "akamai:trafficmanagement/gtmDatacenter:GtmDatacenter": "GtmDatacenter"
-  }
- },
- {
-  "pkg": "akamai",
-  "mod": "trafficmanagement/gtmDomain",
-  "fqn": "pulumi_akamai.trafficmanagement",
-  "classes": {
-   "akamai:trafficmanagement/gtmDomain:GtmDomain": "GtmDomain"
-  }
- },
- {
-  "pkg": "akamai",
-  "mod": "trafficmanagement/gtmGeomap",
-  "fqn": "pulumi_akamai.trafficmanagement",
-  "classes": {
-   "akamai:trafficmanagement/gtmGeomap:GtmGeomap": "GtmGeomap"
-  }
- },
- {
-  "pkg": "akamai",
-  "mod": "trafficmanagement/gtmProperty",
-  "fqn": "pulumi_akamai.trafficmanagement",
-  "classes": {
-   "akamai:trafficmanagement/gtmProperty:GtmProperty": "GtmProperty"
-  }
- },
- {
-  "pkg": "akamai",
-  "mod": "trafficmanagement/gtmResource",
-  "fqn": "pulumi_akamai.trafficmanagement",
-  "classes": {
-   "akamai:trafficmanagement/gtmResource:GtmResource": "GtmResource"
-  }
  }
 ]
 """,
     resource_packages="""
 [
  {
   "pkg": "akamai",
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/_inputs.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,19 +50,27 @@
     'GtmGeomapDefaultDatacenterArgs',
     'GtmPropertyLivenessTestArgs',
     'GtmPropertyLivenessTestHttpHeaderArgs',
     'GtmPropertyStaticRrSetArgs',
     'GtmPropertyTrafficTargetArgs',
     'GtmResourceResourceInstanceArgs',
     'PropertyActivationComplianceRecordArgs',
+    'PropertyActivationComplianceRecordNoncomplianceReasonEmergencyArgs',
+    'PropertyActivationComplianceRecordNoncomplianceReasonNoProductionTrafficArgs',
+    'PropertyActivationComplianceRecordNoncomplianceReasonNoneArgs',
+    'PropertyActivationComplianceRecordNoncomplianceReasonOtherArgs',
     'PropertyActivationRuleErrorArgs',
     'PropertyActivationRuleWarningArgs',
     'PropertyHostnameArgs',
     'PropertyHostnameCertStatusArgs',
     'PropertyIncludeActivationComplianceRecordArgs',
+    'PropertyIncludeActivationComplianceRecordNoncomplianceReasonEmergencyArgs',
+    'PropertyIncludeActivationComplianceRecordNoncomplianceReasonNoProductionTrafficArgs',
+    'PropertyIncludeActivationComplianceRecordNoncomplianceReasonNoneArgs',
+    'PropertyIncludeActivationComplianceRecordNoncomplianceReasonOtherArgs',
     'PropertyOriginArgs',
     'PropertyRuleErrorArgs',
     'PropertyRuleWarningArgs',
     'ProviderAppsecArgs',
     'ProviderConfigArgs',
     'ProviderDnsArgs',
     'ProviderGtmArgs',
@@ -4005,14 +4013,17 @@
     @handout_cname.setter
     def handout_cname(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "handout_cname", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
+        warnings.warn("""The attribute `name` has been deprecated. Any reads or writes on this attribute are ignored""", DeprecationWarning)
+        pulumi.log.warn("""name is deprecated: The attribute `name` has been deprecated. Any reads or writes on this attribute are ignored""")
+
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
@@ -4097,60 +4108,124 @@
     def use_default_load_object(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "use_default_load_object", value)
 
 
 @pulumi.input_type
 class PropertyActivationComplianceRecordArgs:
     def __init__(__self__, *,
-                 noncompliance_reason: pulumi.Input[str],
+                 noncompliance_reason_emergency: Optional[pulumi.Input['PropertyActivationComplianceRecordNoncomplianceReasonEmergencyArgs']] = None,
+                 noncompliance_reason_no_production_traffic: Optional[pulumi.Input['PropertyActivationComplianceRecordNoncomplianceReasonNoProductionTrafficArgs']] = None,
+                 noncompliance_reason_none: Optional[pulumi.Input['PropertyActivationComplianceRecordNoncomplianceReasonNoneArgs']] = None,
+                 noncompliance_reason_other: Optional[pulumi.Input['PropertyActivationComplianceRecordNoncomplianceReasonOtherArgs']] = None):
+        if noncompliance_reason_emergency is not None:
+            pulumi.set(__self__, "noncompliance_reason_emergency", noncompliance_reason_emergency)
+        if noncompliance_reason_no_production_traffic is not None:
+            pulumi.set(__self__, "noncompliance_reason_no_production_traffic", noncompliance_reason_no_production_traffic)
+        if noncompliance_reason_none is not None:
+            pulumi.set(__self__, "noncompliance_reason_none", noncompliance_reason_none)
+        if noncompliance_reason_other is not None:
+            pulumi.set(__self__, "noncompliance_reason_other", noncompliance_reason_other)
+
+    @property
+    @pulumi.getter(name="noncomplianceReasonEmergency")
+    def noncompliance_reason_emergency(self) -> Optional[pulumi.Input['PropertyActivationComplianceRecordNoncomplianceReasonEmergencyArgs']]:
+        return pulumi.get(self, "noncompliance_reason_emergency")
+
+    @noncompliance_reason_emergency.setter
+    def noncompliance_reason_emergency(self, value: Optional[pulumi.Input['PropertyActivationComplianceRecordNoncomplianceReasonEmergencyArgs']]):
+        pulumi.set(self, "noncompliance_reason_emergency", value)
+
+    @property
+    @pulumi.getter(name="noncomplianceReasonNoProductionTraffic")
+    def noncompliance_reason_no_production_traffic(self) -> Optional[pulumi.Input['PropertyActivationComplianceRecordNoncomplianceReasonNoProductionTrafficArgs']]:
+        return pulumi.get(self, "noncompliance_reason_no_production_traffic")
+
+    @noncompliance_reason_no_production_traffic.setter
+    def noncompliance_reason_no_production_traffic(self, value: Optional[pulumi.Input['PropertyActivationComplianceRecordNoncomplianceReasonNoProductionTrafficArgs']]):
+        pulumi.set(self, "noncompliance_reason_no_production_traffic", value)
+
+    @property
+    @pulumi.getter(name="noncomplianceReasonNone")
+    def noncompliance_reason_none(self) -> Optional[pulumi.Input['PropertyActivationComplianceRecordNoncomplianceReasonNoneArgs']]:
+        return pulumi.get(self, "noncompliance_reason_none")
+
+    @noncompliance_reason_none.setter
+    def noncompliance_reason_none(self, value: Optional[pulumi.Input['PropertyActivationComplianceRecordNoncomplianceReasonNoneArgs']]):
+        pulumi.set(self, "noncompliance_reason_none", value)
+
+    @property
+    @pulumi.getter(name="noncomplianceReasonOther")
+    def noncompliance_reason_other(self) -> Optional[pulumi.Input['PropertyActivationComplianceRecordNoncomplianceReasonOtherArgs']]:
+        return pulumi.get(self, "noncompliance_reason_other")
+
+    @noncompliance_reason_other.setter
+    def noncompliance_reason_other(self, value: Optional[pulumi.Input['PropertyActivationComplianceRecordNoncomplianceReasonOtherArgs']]):
+        pulumi.set(self, "noncompliance_reason_other", value)
+
+
+@pulumi.input_type
+class PropertyActivationComplianceRecordNoncomplianceReasonEmergencyArgs:
+    def __init__(__self__, *,
+                 ticket_id: Optional[pulumi.Input[str]] = None):
+        if ticket_id is not None:
+            pulumi.set(__self__, "ticket_id", ticket_id)
+
+    @property
+    @pulumi.getter(name="ticketId")
+    def ticket_id(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "ticket_id")
+
+    @ticket_id.setter
+    def ticket_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "ticket_id", value)
+
+
+@pulumi.input_type
+class PropertyActivationComplianceRecordNoncomplianceReasonNoProductionTrafficArgs:
+    def __init__(__self__, *,
+                 ticket_id: Optional[pulumi.Input[str]] = None):
+        if ticket_id is not None:
+            pulumi.set(__self__, "ticket_id", ticket_id)
+
+    @property
+    @pulumi.getter(name="ticketId")
+    def ticket_id(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "ticket_id")
+
+    @ticket_id.setter
+    def ticket_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "ticket_id", value)
+
+
+@pulumi.input_type
+class PropertyActivationComplianceRecordNoncomplianceReasonNoneArgs:
+    def __init__(__self__, *,
                  customer_email: Optional[pulumi.Input[str]] = None,
-                 other_noncompliance_reason: Optional[pulumi.Input[str]] = None,
                  peer_reviewed_by: Optional[pulumi.Input[str]] = None,
                  ticket_id: Optional[pulumi.Input[str]] = None,
                  unit_tested: Optional[pulumi.Input[bool]] = None):
-        pulumi.set(__self__, "noncompliance_reason", noncompliance_reason)
         if customer_email is not None:
             pulumi.set(__self__, "customer_email", customer_email)
-        if other_noncompliance_reason is not None:
-            pulumi.set(__self__, "other_noncompliance_reason", other_noncompliance_reason)
         if peer_reviewed_by is not None:
             pulumi.set(__self__, "peer_reviewed_by", peer_reviewed_by)
         if ticket_id is not None:
             pulumi.set(__self__, "ticket_id", ticket_id)
         if unit_tested is not None:
             pulumi.set(__self__, "unit_tested", unit_tested)
 
     @property
-    @pulumi.getter(name="noncomplianceReason")
-    def noncompliance_reason(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "noncompliance_reason")
-
-    @noncompliance_reason.setter
-    def noncompliance_reason(self, value: pulumi.Input[str]):
-        pulumi.set(self, "noncompliance_reason", value)
-
-    @property
     @pulumi.getter(name="customerEmail")
     def customer_email(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "customer_email")
 
     @customer_email.setter
     def customer_email(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "customer_email", value)
 
     @property
-    @pulumi.getter(name="otherNoncomplianceReason")
-    def other_noncompliance_reason(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "other_noncompliance_reason")
-
-    @other_noncompliance_reason.setter
-    def other_noncompliance_reason(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "other_noncompliance_reason", value)
-
-    @property
     @pulumi.getter(name="peerReviewedBy")
     def peer_reviewed_by(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "peer_reviewed_by")
 
     @peer_reviewed_by.setter
     def peer_reviewed_by(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "peer_reviewed_by", value)
@@ -4171,14 +4246,43 @@
 
     @unit_tested.setter
     def unit_tested(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "unit_tested", value)
 
 
 @pulumi.input_type
+class PropertyActivationComplianceRecordNoncomplianceReasonOtherArgs:
+    def __init__(__self__, *,
+                 other_noncompliance_reason: Optional[pulumi.Input[str]] = None,
+                 ticket_id: Optional[pulumi.Input[str]] = None):
+        if other_noncompliance_reason is not None:
+            pulumi.set(__self__, "other_noncompliance_reason", other_noncompliance_reason)
+        if ticket_id is not None:
+            pulumi.set(__self__, "ticket_id", ticket_id)
+
+    @property
+    @pulumi.getter(name="otherNoncomplianceReason")
+    def other_noncompliance_reason(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "other_noncompliance_reason")
+
+    @other_noncompliance_reason.setter
+    def other_noncompliance_reason(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "other_noncompliance_reason", value)
+
+    @property
+    @pulumi.getter(name="ticketId")
+    def ticket_id(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "ticket_id")
+
+    @ticket_id.setter
+    def ticket_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "ticket_id", value)
+
+
+@pulumi.input_type
 class PropertyActivationRuleErrorArgs:
     def __init__(__self__, *,
                  behavior_name: Optional[pulumi.Input[str]] = None,
                  detail: Optional[pulumi.Input[str]] = None,
                  error_location: Optional[pulumi.Input[str]] = None,
                  instance: Optional[pulumi.Input[str]] = None,
                  status_code: Optional[pulumi.Input[int]] = None,
@@ -4478,60 +4582,124 @@
     def target(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "target", value)
 
 
 @pulumi.input_type
 class PropertyIncludeActivationComplianceRecordArgs:
     def __init__(__self__, *,
-                 noncompliance_reason: pulumi.Input[str],
+                 noncompliance_reason_emergency: Optional[pulumi.Input['PropertyIncludeActivationComplianceRecordNoncomplianceReasonEmergencyArgs']] = None,
+                 noncompliance_reason_no_production_traffic: Optional[pulumi.Input['PropertyIncludeActivationComplianceRecordNoncomplianceReasonNoProductionTrafficArgs']] = None,
+                 noncompliance_reason_none: Optional[pulumi.Input['PropertyIncludeActivationComplianceRecordNoncomplianceReasonNoneArgs']] = None,
+                 noncompliance_reason_other: Optional[pulumi.Input['PropertyIncludeActivationComplianceRecordNoncomplianceReasonOtherArgs']] = None):
+        if noncompliance_reason_emergency is not None:
+            pulumi.set(__self__, "noncompliance_reason_emergency", noncompliance_reason_emergency)
+        if noncompliance_reason_no_production_traffic is not None:
+            pulumi.set(__self__, "noncompliance_reason_no_production_traffic", noncompliance_reason_no_production_traffic)
+        if noncompliance_reason_none is not None:
+            pulumi.set(__self__, "noncompliance_reason_none", noncompliance_reason_none)
+        if noncompliance_reason_other is not None:
+            pulumi.set(__self__, "noncompliance_reason_other", noncompliance_reason_other)
+
+    @property
+    @pulumi.getter(name="noncomplianceReasonEmergency")
+    def noncompliance_reason_emergency(self) -> Optional[pulumi.Input['PropertyIncludeActivationComplianceRecordNoncomplianceReasonEmergencyArgs']]:
+        return pulumi.get(self, "noncompliance_reason_emergency")
+
+    @noncompliance_reason_emergency.setter
+    def noncompliance_reason_emergency(self, value: Optional[pulumi.Input['PropertyIncludeActivationComplianceRecordNoncomplianceReasonEmergencyArgs']]):
+        pulumi.set(self, "noncompliance_reason_emergency", value)
+
+    @property
+    @pulumi.getter(name="noncomplianceReasonNoProductionTraffic")
+    def noncompliance_reason_no_production_traffic(self) -> Optional[pulumi.Input['PropertyIncludeActivationComplianceRecordNoncomplianceReasonNoProductionTrafficArgs']]:
+        return pulumi.get(self, "noncompliance_reason_no_production_traffic")
+
+    @noncompliance_reason_no_production_traffic.setter
+    def noncompliance_reason_no_production_traffic(self, value: Optional[pulumi.Input['PropertyIncludeActivationComplianceRecordNoncomplianceReasonNoProductionTrafficArgs']]):
+        pulumi.set(self, "noncompliance_reason_no_production_traffic", value)
+
+    @property
+    @pulumi.getter(name="noncomplianceReasonNone")
+    def noncompliance_reason_none(self) -> Optional[pulumi.Input['PropertyIncludeActivationComplianceRecordNoncomplianceReasonNoneArgs']]:
+        return pulumi.get(self, "noncompliance_reason_none")
+
+    @noncompliance_reason_none.setter
+    def noncompliance_reason_none(self, value: Optional[pulumi.Input['PropertyIncludeActivationComplianceRecordNoncomplianceReasonNoneArgs']]):
+        pulumi.set(self, "noncompliance_reason_none", value)
+
+    @property
+    @pulumi.getter(name="noncomplianceReasonOther")
+    def noncompliance_reason_other(self) -> Optional[pulumi.Input['PropertyIncludeActivationComplianceRecordNoncomplianceReasonOtherArgs']]:
+        return pulumi.get(self, "noncompliance_reason_other")
+
+    @noncompliance_reason_other.setter
+    def noncompliance_reason_other(self, value: Optional[pulumi.Input['PropertyIncludeActivationComplianceRecordNoncomplianceReasonOtherArgs']]):
+        pulumi.set(self, "noncompliance_reason_other", value)
+
+
+@pulumi.input_type
+class PropertyIncludeActivationComplianceRecordNoncomplianceReasonEmergencyArgs:
+    def __init__(__self__, *,
+                 ticket_id: Optional[pulumi.Input[str]] = None):
+        if ticket_id is not None:
+            pulumi.set(__self__, "ticket_id", ticket_id)
+
+    @property
+    @pulumi.getter(name="ticketId")
+    def ticket_id(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "ticket_id")
+
+    @ticket_id.setter
+    def ticket_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "ticket_id", value)
+
+
+@pulumi.input_type
+class PropertyIncludeActivationComplianceRecordNoncomplianceReasonNoProductionTrafficArgs:
+    def __init__(__self__, *,
+                 ticket_id: Optional[pulumi.Input[str]] = None):
+        if ticket_id is not None:
+            pulumi.set(__self__, "ticket_id", ticket_id)
+
+    @property
+    @pulumi.getter(name="ticketId")
+    def ticket_id(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "ticket_id")
+
+    @ticket_id.setter
+    def ticket_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "ticket_id", value)
+
+
+@pulumi.input_type
+class PropertyIncludeActivationComplianceRecordNoncomplianceReasonNoneArgs:
+    def __init__(__self__, *,
                  customer_email: Optional[pulumi.Input[str]] = None,
-                 other_noncompliance_reason: Optional[pulumi.Input[str]] = None,
                  peer_reviewed_by: Optional[pulumi.Input[str]] = None,
                  ticket_id: Optional[pulumi.Input[str]] = None,
                  unit_tested: Optional[pulumi.Input[bool]] = None):
-        pulumi.set(__self__, "noncompliance_reason", noncompliance_reason)
         if customer_email is not None:
             pulumi.set(__self__, "customer_email", customer_email)
-        if other_noncompliance_reason is not None:
-            pulumi.set(__self__, "other_noncompliance_reason", other_noncompliance_reason)
         if peer_reviewed_by is not None:
             pulumi.set(__self__, "peer_reviewed_by", peer_reviewed_by)
         if ticket_id is not None:
             pulumi.set(__self__, "ticket_id", ticket_id)
         if unit_tested is not None:
             pulumi.set(__self__, "unit_tested", unit_tested)
 
     @property
-    @pulumi.getter(name="noncomplianceReason")
-    def noncompliance_reason(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "noncompliance_reason")
-
-    @noncompliance_reason.setter
-    def noncompliance_reason(self, value: pulumi.Input[str]):
-        pulumi.set(self, "noncompliance_reason", value)
-
-    @property
     @pulumi.getter(name="customerEmail")
     def customer_email(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "customer_email")
 
     @customer_email.setter
     def customer_email(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "customer_email", value)
 
     @property
-    @pulumi.getter(name="otherNoncomplianceReason")
-    def other_noncompliance_reason(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "other_noncompliance_reason")
-
-    @other_noncompliance_reason.setter
-    def other_noncompliance_reason(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "other_noncompliance_reason", value)
-
-    @property
     @pulumi.getter(name="peerReviewedBy")
     def peer_reviewed_by(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "peer_reviewed_by")
 
     @peer_reviewed_by.setter
     def peer_reviewed_by(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "peer_reviewed_by", value)
@@ -4552,14 +4720,43 @@
 
     @unit_tested.setter
     def unit_tested(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "unit_tested", value)
 
 
 @pulumi.input_type
+class PropertyIncludeActivationComplianceRecordNoncomplianceReasonOtherArgs:
+    def __init__(__self__, *,
+                 other_noncompliance_reason: Optional[pulumi.Input[str]] = None,
+                 ticket_id: Optional[pulumi.Input[str]] = None):
+        if other_noncompliance_reason is not None:
+            pulumi.set(__self__, "other_noncompliance_reason", other_noncompliance_reason)
+        if ticket_id is not None:
+            pulumi.set(__self__, "ticket_id", ticket_id)
+
+    @property
+    @pulumi.getter(name="otherNoncomplianceReason")
+    def other_noncompliance_reason(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "other_noncompliance_reason")
+
+    @other_noncompliance_reason.setter
+    def other_noncompliance_reason(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "other_noncompliance_reason", value)
+
+    @property
+    @pulumi.getter(name="ticketId")
+    def ticket_id(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "ticket_id")
+
+    @ticket_id.setter
+    def ticket_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "ticket_id", value)
+
+
+@pulumi.input_type
 class PropertyOriginArgs:
     def __init__(__self__, *,
                  cache_key_hostname: Optional[pulumi.Input[str]] = None,
                  compress: Optional[pulumi.Input[bool]] = None,
                  enable_true_client_ip: Optional[pulumi.Input[bool]] = None,
                  forward_hostname: Optional[pulumi.Input[str]] = None,
                  hostname: Optional[pulumi.Input[str]] = None,
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/_utilities.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_activations.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_activations.py`

 * *Files 14% similar despite different names*

```diff
@@ -87,14 +87,17 @@
 
     @property
     @pulumi.getter
     def activate(self) -> Optional[pulumi.Input[bool]]:
         """
         Whether to activate or deactivate the specified security configuration and version
         """
+        warnings.warn("""The setting activate has been deprecated; \"terraform apply\" will always perform activation. (Use \"terraform destroy\" for deactivation.)""", DeprecationWarning)
+        pulumi.log.warn("""activate is deprecated: The setting activate has been deprecated; \"terraform apply\" will always perform activation. (Use \"terraform destroy\" for deactivation.)""")
+
         return pulumi.get(self, "activate")
 
     @activate.setter
     def activate(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "activate", value)
 
     @property
@@ -123,14 +126,17 @@
 
     @property
     @pulumi.getter
     def notes(self) -> Optional[pulumi.Input[str]]:
         """
         Note describing the activation
         """
+        warnings.warn("""The setting notes has been deprecated. Use \"note\" instead.""", DeprecationWarning)
+        pulumi.log.warn("""notes is deprecated: The setting notes has been deprecated. Use \"note\" instead.""")
+
         return pulumi.get(self, "notes")
 
     @notes.setter
     def notes(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "notes", value)
 
 
@@ -181,14 +187,17 @@
 
     @property
     @pulumi.getter
     def activate(self) -> Optional[pulumi.Input[bool]]:
         """
         Whether to activate or deactivate the specified security configuration and version
         """
+        warnings.warn("""The setting activate has been deprecated; \"terraform apply\" will always perform activation. (Use \"terraform destroy\" for deactivation.)""", DeprecationWarning)
+        pulumi.log.warn("""activate is deprecated: The setting activate has been deprecated; \"terraform apply\" will always perform activation. (Use \"terraform destroy\" for deactivation.)""")
+
         return pulumi.get(self, "activate")
 
     @activate.setter
     def activate(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "activate", value)
 
     @property
@@ -229,14 +238,17 @@
 
     @property
     @pulumi.getter
     def notes(self) -> Optional[pulumi.Input[str]]:
         """
         Note describing the activation
         """
+        warnings.warn("""The setting notes has been deprecated. Use \"note\" instead.""", DeprecationWarning)
+        pulumi.log.warn("""notes is deprecated: The setting notes has been deprecated. Use \"note\" instead.""")
+
         return pulumi.get(self, "notes")
 
     @notes.setter
     def notes(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "notes", value)
 
     @property
@@ -410,14 +422,17 @@
 
     @property
     @pulumi.getter
     def activate(self) -> pulumi.Output[Optional[bool]]:
         """
         Whether to activate or deactivate the specified security configuration and version
         """
+        warnings.warn("""The setting activate has been deprecated; \"terraform apply\" will always perform activation. (Use \"terraform destroy\" for deactivation.)""", DeprecationWarning)
+        pulumi.log.warn("""activate is deprecated: The setting activate has been deprecated; \"terraform apply\" will always perform activation. (Use \"terraform destroy\" for deactivation.)""")
+
         return pulumi.get(self, "activate")
 
     @property
     @pulumi.getter(name="configId")
     def config_id(self) -> pulumi.Output[int]:
         """
         Unique identifier of the security configuration to be activated
@@ -442,14 +457,17 @@
 
     @property
     @pulumi.getter
     def notes(self) -> pulumi.Output[Optional[str]]:
         """
         Note describing the activation
         """
+        warnings.warn("""The setting notes has been deprecated. Use \"note\" instead.""", DeprecationWarning)
+        pulumi.log.warn("""notes is deprecated: The setting notes has been deprecated. Use \"note\" instead.""")
+
         return pulumi.get(self, "notes")
 
     @property
     @pulumi.getter(name="notificationEmails")
     def notification_emails(self) -> pulumi.Output[Sequence[str]]:
         """
         List of email addresses to be notified with the results of the activation
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_advanced_settings_evasive_path_match.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_advanced_settings_evasive_path_match.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_advanced_settings_logging.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_advanced_settings_logging.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_advanced_settings_pragma_header.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_advanced_settings_pragma_header.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_advanced_settings_prefetch.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_advanced_settings_prefetch.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_api_constraints_protection.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_api_constraints_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_api_request_constraints.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_api_request_constraints.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_attack_group.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_attack_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_by_pass_network_list.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_by_pass_network_list.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_configuration.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_configuration_rename.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_configuration_rename.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_custom_deny.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_custom_deny.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_custom_rule.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_custom_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_custom_rule_action.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_custom_rule_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_eval.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_eval.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_eval_group.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_eval_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_eval_penalty_box.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_eval_penalty_box.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_eval_rule.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_eval_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_ip_geo.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_ip_geo.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_ip_geo_protection.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_ip_geo_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_malware_policy.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_malware_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_malware_policy_action.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_malware_policy_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_malware_policy_actions.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_malware_policy_actions.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_malware_protection.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_malware_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_match_target.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_match_target.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_match_target_sequence.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_match_target_sequence.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_penalty_box.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_penalty_box.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_rate_policy.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_rate_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_rate_policy_action.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_rate_policy_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_rate_protection.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_rate_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_reputation_profile.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_reputation_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_reputation_profile_action.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_reputation_profile_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_reputation_profile_analysis.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_reputation_profile_analysis.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_reputation_protection.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_reputation_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_rule.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_rule_upgrade.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_rule_upgrade.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_security_policy.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_security_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_security_policy_rename.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_security_policy_rename.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_selected_hostnames.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_selected_hostnames.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_siem_settings.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_siem_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_slow_post.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_slow_post.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_slow_post_protection.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_slow_post_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_threat_intel.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_threat_intel.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_version_nodes.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_version_nodes.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_waf_mode.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_waf_mode.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_waf_protection.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_waf_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_wap_selected_hostnames.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/app_sec_wap_selected_hostnames.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/appsec_advanced_settings_attack_payload_logging.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/appsec_advanced_settings_attack_payload_logging.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/appsec_advanced_settings_request_body.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/appsec_advanced_settings_request_body.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/cloudlets_application_load_balancer.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/cloudlets_application_load_balancer.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/cloudlets_application_load_balancer_activation.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/cloudlets_application_load_balancer_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/cloudlets_policy.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/cloudlets_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/cloudlets_policy_activation.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/cloudlets_policy_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/config/outputs.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/config/vars.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/cp_code.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/cp_code.py`

 * *Files 21% similar despite different names*

```diff
@@ -47,14 +47,17 @@
             pulumi.set(__self__, "product", product)
         if product_id is not None:
             pulumi.set(__self__, "product_id", product_id)
 
     @property
     @pulumi.getter
     def contract(self) -> Optional[pulumi.Input[str]]:
+        warnings.warn("""The setting \"contract\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""contract is deprecated: The setting \"contract\" has been deprecated.""")
+
         return pulumi.get(self, "contract")
 
     @contract.setter
     def contract(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "contract", value)
 
     @property
@@ -65,14 +68,17 @@
     @contract_id.setter
     def contract_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "contract_id", value)
 
     @property
     @pulumi.getter
     def group(self) -> Optional[pulumi.Input[str]]:
+        warnings.warn("""The setting \"group\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""group is deprecated: The setting \"group\" has been deprecated.""")
+
         return pulumi.get(self, "group")
 
     @group.setter
     def group(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "group", value)
 
     @property
@@ -92,14 +98,17 @@
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def product(self) -> Optional[pulumi.Input[str]]:
+        warnings.warn("""The setting \"product\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""product is deprecated: The setting \"product\" has been deprecated.""")
+
         return pulumi.get(self, "product")
 
     @product.setter
     def product(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "product", value)
 
     @property
@@ -148,14 +157,17 @@
             pulumi.set(__self__, "product", product)
         if product_id is not None:
             pulumi.set(__self__, "product_id", product_id)
 
     @property
     @pulumi.getter
     def contract(self) -> Optional[pulumi.Input[str]]:
+        warnings.warn("""The setting \"contract\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""contract is deprecated: The setting \"contract\" has been deprecated.""")
+
         return pulumi.get(self, "contract")
 
     @contract.setter
     def contract(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "contract", value)
 
     @property
@@ -166,14 +178,17 @@
     @contract_id.setter
     def contract_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "contract_id", value)
 
     @property
     @pulumi.getter
     def group(self) -> Optional[pulumi.Input[str]]:
+        warnings.warn("""The setting \"group\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""group is deprecated: The setting \"group\" has been deprecated.""")
+
         return pulumi.get(self, "group")
 
     @group.setter
     def group(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "group", value)
 
     @property
@@ -193,14 +208,17 @@
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def product(self) -> Optional[pulumi.Input[str]]:
+        warnings.warn("""The setting \"product\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""product is deprecated: The setting \"product\" has been deprecated.""")
+
         return pulumi.get(self, "product")
 
     @product.setter
     def product(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "product", value)
 
     @property
@@ -325,24 +343,30 @@
         __props__.__dict__["product"] = product
         __props__.__dict__["product_id"] = product_id
         return CpCode(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def contract(self) -> pulumi.Output[str]:
+        warnings.warn("""The setting \"contract\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""contract is deprecated: The setting \"contract\" has been deprecated.""")
+
         return pulumi.get(self, "contract")
 
     @property
     @pulumi.getter(name="contractId")
     def contract_id(self) -> pulumi.Output[str]:
         return pulumi.get(self, "contract_id")
 
     @property
     @pulumi.getter
     def group(self) -> pulumi.Output[str]:
+        warnings.warn("""The setting \"group\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""group is deprecated: The setting \"group\" has been deprecated.""")
+
         return pulumi.get(self, "group")
 
     @property
     @pulumi.getter(name="groupId")
     def group_id(self) -> pulumi.Output[str]:
         return pulumi.get(self, "group_id")
 
@@ -350,14 +374,17 @@
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def product(self) -> pulumi.Output[str]:
+        warnings.warn("""The setting \"product\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""product is deprecated: The setting \"product\" has been deprecated.""")
+
         return pulumi.get(self, "product")
 
     @property
     @pulumi.getter(name="productId")
     def product_id(self) -> pulumi.Output[str]:
         return pulumi.get(self, "product_id")
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/cps_dv_enrollment.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/cps_dv_enrollment.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,14 +231,17 @@
 
     @property
     @pulumi.getter(name="enableMultiStackedCertificates")
     def enable_multi_stacked_certificates(self) -> Optional[pulumi.Input[bool]]:
         """
         Enable Dual-Stacked certificate deployment for enrollment
         """
+        warnings.warn("""Deprecated, don't use; always false""", DeprecationWarning)
+        pulumi.log.warn("""enable_multi_stacked_certificates is deprecated: Deprecated, don't use; always false""")
+
         return pulumi.get(self, "enable_multi_stacked_certificates")
 
     @enable_multi_stacked_certificates.setter
     def enable_multi_stacked_certificates(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_multi_stacked_certificates", value)
 
     @property
@@ -454,14 +457,17 @@
 
     @property
     @pulumi.getter(name="enableMultiStackedCertificates")
     def enable_multi_stacked_certificates(self) -> Optional[pulumi.Input[bool]]:
         """
         Enable Dual-Stacked certificate deployment for enrollment
         """
+        warnings.warn("""Deprecated, don't use; always false""", DeprecationWarning)
+        pulumi.log.warn("""enable_multi_stacked_certificates is deprecated: Deprecated, don't use; always false""")
+
         return pulumi.get(self, "enable_multi_stacked_certificates")
 
     @enable_multi_stacked_certificates.setter
     def enable_multi_stacked_certificates(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_multi_stacked_certificates", value)
 
     @property
@@ -874,14 +880,17 @@
 
     @property
     @pulumi.getter(name="enableMultiStackedCertificates")
     def enable_multi_stacked_certificates(self) -> pulumi.Output[Optional[bool]]:
         """
         Enable Dual-Stacked certificate deployment for enrollment
         """
+        warnings.warn("""Deprecated, don't use; always false""", DeprecationWarning)
+        pulumi.log.warn("""enable_multi_stacked_certificates is deprecated: Deprecated, don't use; always false""")
+
         return pulumi.get(self, "enable_multi_stacked_certificates")
 
     @property
     @pulumi.getter(name="httpChallenges")
     def http_challenges(self) -> pulumi.Output[Sequence['outputs.CpsDvEnrollmentHttpChallenge']]:
         """
         HTTP challenge information
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/cps_dv_validation.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/cps_dv_validation.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/cps_third_party_enrollment.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/cps_third_party_enrollment.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/cps_upload_certificate.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/cps_upload_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/datastream.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/datastream.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/dns_record.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/dns_record.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/dns_zone.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/dns_zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edge_host_name.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/edge_host_name.py`

 * *Files 16% similar despite different names*

```diff
@@ -86,14 +86,17 @@
     @certificate.setter
     def certificate(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "certificate", value)
 
     @property
     @pulumi.getter
     def contract(self) -> Optional[pulumi.Input[str]]:
+        warnings.warn("""The setting \"contract\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""contract is deprecated: The setting \"contract\" has been deprecated.""")
+
         return pulumi.get(self, "contract")
 
     @contract.setter
     def contract(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "contract", value)
 
     @property
@@ -104,14 +107,17 @@
     @contract_id.setter
     def contract_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "contract_id", value)
 
     @property
     @pulumi.getter
     def group(self) -> Optional[pulumi.Input[str]]:
+        warnings.warn("""The setting \"group\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""group is deprecated: The setting \"group\" has been deprecated.""")
+
         return pulumi.get(self, "group")
 
     @group.setter
     def group(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "group", value)
 
     @property
@@ -122,14 +128,17 @@
     @group_id.setter
     def group_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "group_id", value)
 
     @property
     @pulumi.getter
     def product(self) -> Optional[pulumi.Input[str]]:
+        warnings.warn("""The setting \"product\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""product is deprecated: The setting \"product\" has been deprecated.""")
+
         return pulumi.get(self, "product")
 
     @product.setter
     def product(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "product", value)
 
     @property
@@ -225,14 +234,17 @@
     @certificate.setter
     def certificate(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "certificate", value)
 
     @property
     @pulumi.getter
     def contract(self) -> Optional[pulumi.Input[str]]:
+        warnings.warn("""The setting \"contract\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""contract is deprecated: The setting \"contract\" has been deprecated.""")
+
         return pulumi.get(self, "contract")
 
     @contract.setter
     def contract(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "contract", value)
 
     @property
@@ -252,14 +264,17 @@
     @edge_hostname.setter
     def edge_hostname(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "edge_hostname", value)
 
     @property
     @pulumi.getter
     def group(self) -> Optional[pulumi.Input[str]]:
+        warnings.warn("""The setting \"group\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""group is deprecated: The setting \"group\" has been deprecated.""")
+
         return pulumi.get(self, "group")
 
     @group.setter
     def group(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "group", value)
 
     @property
@@ -279,14 +294,17 @@
     @ip_behavior.setter
     def ip_behavior(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ip_behavior", value)
 
     @property
     @pulumi.getter
     def product(self) -> Optional[pulumi.Input[str]]:
+        warnings.warn("""The setting \"product\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""product is deprecated: The setting \"product\" has been deprecated.""")
+
         return pulumi.get(self, "product")
 
     @product.setter
     def product(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "product", value)
 
     @property
@@ -468,14 +486,17 @@
     @pulumi.getter
     def certificate(self) -> pulumi.Output[Optional[int]]:
         return pulumi.get(self, "certificate")
 
     @property
     @pulumi.getter
     def contract(self) -> pulumi.Output[str]:
+        warnings.warn("""The setting \"contract\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""contract is deprecated: The setting \"contract\" has been deprecated.""")
+
         return pulumi.get(self, "contract")
 
     @property
     @pulumi.getter(name="contractId")
     def contract_id(self) -> pulumi.Output[str]:
         return pulumi.get(self, "contract_id")
 
@@ -483,14 +504,17 @@
     @pulumi.getter(name="edgeHostname")
     def edge_hostname(self) -> pulumi.Output[str]:
         return pulumi.get(self, "edge_hostname")
 
     @property
     @pulumi.getter
     def group(self) -> pulumi.Output[str]:
+        warnings.warn("""The setting \"group\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""group is deprecated: The setting \"group\" has been deprecated.""")
+
         return pulumi.get(self, "group")
 
     @property
     @pulumi.getter(name="groupId")
     def group_id(self) -> pulumi.Output[str]:
         return pulumi.get(self, "group_id")
 
@@ -498,14 +522,17 @@
     @pulumi.getter(name="ipBehavior")
     def ip_behavior(self) -> pulumi.Output[str]:
         return pulumi.get(self, "ip_behavior")
 
     @property
     @pulumi.getter
     def product(self) -> pulumi.Output[str]:
+        warnings.warn("""The setting \"product\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""product is deprecated: The setting \"product\" has been deprecated.""")
+
         return pulumi.get(self, "product")
 
     @property
     @pulumi.getter(name="productId")
     def product_id(self) -> pulumi.Output[str]:
         return pulumi.get(self, "product_id")
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edge_kv.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/edge_kv.py`

 * *Files 6% similar despite different names*

```diff
@@ -105,14 +105,17 @@
 
     @property
     @pulumi.getter(name="initialDatas")
     def initial_datas(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['EdgeKvInitialDataArgs']]]]:
         """
         List of pairs to initialize the namespace. Just meaningful for creation, updates will be ignored.
         """
+        warnings.warn("""The attribute 'initial_data' has been deprecated. To manage edgeKV items use 'akamai_edgekv_group_items' resource instead.""", DeprecationWarning)
+        pulumi.log.warn("""initial_datas is deprecated: The attribute 'initial_data' has been deprecated. To manage edgeKV items use 'akamai_edgekv_group_items' resource instead.""")
+
         return pulumi.get(self, "initial_datas")
 
     @initial_datas.setter
     def initial_datas(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['EdgeKvInitialDataArgs']]]]):
         pulumi.set(self, "initial_datas", value)
 
 
@@ -176,14 +179,17 @@
 
     @property
     @pulumi.getter(name="initialDatas")
     def initial_datas(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['EdgeKvInitialDataArgs']]]]:
         """
         List of pairs to initialize the namespace. Just meaningful for creation, updates will be ignored.
         """
+        warnings.warn("""The attribute 'initial_data' has been deprecated. To manage edgeKV items use 'akamai_edgekv_group_items' resource instead.""", DeprecationWarning)
+        pulumi.log.warn("""initial_datas is deprecated: The attribute 'initial_data' has been deprecated. To manage edgeKV items use 'akamai_edgekv_group_items' resource instead.""")
+
         return pulumi.get(self, "initial_datas")
 
     @initial_datas.setter
     def initial_datas(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['EdgeKvInitialDataArgs']]]]):
         pulumi.set(self, "initial_datas", value)
 
     @property
@@ -361,14 +367,17 @@
 
     @property
     @pulumi.getter(name="initialDatas")
     def initial_datas(self) -> pulumi.Output[Optional[Sequence['outputs.EdgeKvInitialData']]]:
         """
         List of pairs to initialize the namespace. Just meaningful for creation, updates will be ignored.
         """
+        warnings.warn("""The attribute 'initial_data' has been deprecated. To manage edgeKV items use 'akamai_edgekv_group_items' resource instead.""", DeprecationWarning)
+        pulumi.log.warn("""initial_datas is deprecated: The attribute 'initial_data' has been deprecated. To manage edgeKV items use 'akamai_edgekv_group_items' resource instead.""")
+
         return pulumi.get(self, "initial_datas")
 
     @property
     @pulumi.getter(name="namespaceName")
     def namespace_name(self) -> pulumi.Output[str]:
         """
         Name for the EKV namespace
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edge_worker.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/edge_worker.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edge_workers_activation.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/edge_workers_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edgedns/dns_zone.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/gtm_resource.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,539 +3,611 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from .. import _utilities
+from . import _utilities
 from . import outputs
 from ._inputs import *
 
-__all__ = ['DnsZoneArgs', 'DnsZone']
+__all__ = ['GtmResourceArgs', 'GtmResource']
 
 @pulumi.input_type
-class DnsZoneArgs:
+class GtmResourceArgs:
     def __init__(__self__, *,
-                 contract: pulumi.Input[str],
+                 aggregation_type: pulumi.Input[str],
+                 domain: pulumi.Input[str],
                  type: pulumi.Input[str],
-                 zone: pulumi.Input[str],
-                 comment: Optional[pulumi.Input[str]] = None,
-                 end_customer_id: Optional[pulumi.Input[str]] = None,
-                 group: Optional[pulumi.Input[str]] = None,
-                 masters: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 sign_and_serve: Optional[pulumi.Input[bool]] = None,
-                 sign_and_serve_algorithm: Optional[pulumi.Input[str]] = None,
-                 target: Optional[pulumi.Input[str]] = None,
-                 tsig_key: Optional[pulumi.Input['DnsZoneTsigKeyArgs']] = None):
+                 constrained_property: Optional[pulumi.Input[str]] = None,
+                 decay_rate: Optional[pulumi.Input[float]] = None,
+                 description: Optional[pulumi.Input[str]] = None,
+                 host_header: Optional[pulumi.Input[str]] = None,
+                 leader_string: Optional[pulumi.Input[str]] = None,
+                 least_squares_decay: Optional[pulumi.Input[float]] = None,
+                 load_imbalance_percentage: Optional[pulumi.Input[float]] = None,
+                 max_u_multiplicative_increment: Optional[pulumi.Input[float]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 resource_instances: Optional[pulumi.Input[Sequence[pulumi.Input['GtmResourceResourceInstanceArgs']]]] = None,
+                 upper_bound: Optional[pulumi.Input[int]] = None,
+                 wait_on_complete: Optional[pulumi.Input[bool]] = None):
         """
-        The set of arguments for constructing a DnsZone resource.
+        The set of arguments for constructing a GtmResource resource.
         """
-        pulumi.set(__self__, "contract", contract)
+        pulumi.set(__self__, "aggregation_type", aggregation_type)
+        pulumi.set(__self__, "domain", domain)
         pulumi.set(__self__, "type", type)
-        pulumi.set(__self__, "zone", zone)
-        if comment is not None:
-            pulumi.set(__self__, "comment", comment)
-        if end_customer_id is not None:
-            pulumi.set(__self__, "end_customer_id", end_customer_id)
-        if group is not None:
-            pulumi.set(__self__, "group", group)
-        if masters is not None:
-            pulumi.set(__self__, "masters", masters)
-        if sign_and_serve is not None:
-            pulumi.set(__self__, "sign_and_serve", sign_and_serve)
-        if sign_and_serve_algorithm is not None:
-            pulumi.set(__self__, "sign_and_serve_algorithm", sign_and_serve_algorithm)
-        if target is not None:
-            pulumi.set(__self__, "target", target)
-        if tsig_key is not None:
-            pulumi.set(__self__, "tsig_key", tsig_key)
+        if constrained_property is not None:
+            pulumi.set(__self__, "constrained_property", constrained_property)
+        if decay_rate is not None:
+            pulumi.set(__self__, "decay_rate", decay_rate)
+        if description is not None:
+            pulumi.set(__self__, "description", description)
+        if host_header is not None:
+            pulumi.set(__self__, "host_header", host_header)
+        if leader_string is not None:
+            pulumi.set(__self__, "leader_string", leader_string)
+        if least_squares_decay is not None:
+            pulumi.set(__self__, "least_squares_decay", least_squares_decay)
+        if load_imbalance_percentage is not None:
+            pulumi.set(__self__, "load_imbalance_percentage", load_imbalance_percentage)
+        if max_u_multiplicative_increment is not None:
+            pulumi.set(__self__, "max_u_multiplicative_increment", max_u_multiplicative_increment)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if resource_instances is not None:
+            pulumi.set(__self__, "resource_instances", resource_instances)
+        if upper_bound is not None:
+            pulumi.set(__self__, "upper_bound", upper_bound)
+        if wait_on_complete is not None:
+            pulumi.set(__self__, "wait_on_complete", wait_on_complete)
+
+    @property
+    @pulumi.getter(name="aggregationType")
+    def aggregation_type(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "aggregation_type")
+
+    @aggregation_type.setter
+    def aggregation_type(self, value: pulumi.Input[str]):
+        pulumi.set(self, "aggregation_type", value)
 
     @property
     @pulumi.getter
-    def contract(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "contract")
-
-    @contract.setter
-    def contract(self, value: pulumi.Input[str]):
-        pulumi.set(self, "contract", value)
+    def domain(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "domain")
+
+    @domain.setter
+    def domain(self, value: pulumi.Input[str]):
+        pulumi.set(self, "domain", value)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
     @property
-    @pulumi.getter
-    def zone(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "zone")
+    @pulumi.getter(name="constrainedProperty")
+    def constrained_property(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "constrained_property")
+
+    @constrained_property.setter
+    def constrained_property(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "constrained_property", value)
+
+    @property
+    @pulumi.getter(name="decayRate")
+    def decay_rate(self) -> Optional[pulumi.Input[float]]:
+        return pulumi.get(self, "decay_rate")
 
-    @zone.setter
-    def zone(self, value: pulumi.Input[str]):
-        pulumi.set(self, "zone", value)
+    @decay_rate.setter
+    def decay_rate(self, value: Optional[pulumi.Input[float]]):
+        pulumi.set(self, "decay_rate", value)
 
     @property
     @pulumi.getter
-    def comment(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "comment")
+    def description(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "description")
 
-    @comment.setter
-    def comment(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "comment", value)
+    @description.setter
+    def description(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "description", value)
 
     @property
-    @pulumi.getter(name="endCustomerId")
-    def end_customer_id(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "end_customer_id")
+    @pulumi.getter(name="hostHeader")
+    def host_header(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "host_header")
 
-    @end_customer_id.setter
-    def end_customer_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "end_customer_id", value)
+    @host_header.setter
+    def host_header(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "host_header", value)
 
     @property
-    @pulumi.getter
-    def group(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "group")
+    @pulumi.getter(name="leaderString")
+    def leader_string(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "leader_string")
 
-    @group.setter
-    def group(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "group", value)
+    @leader_string.setter
+    def leader_string(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "leader_string", value)
 
     @property
-    @pulumi.getter
-    def masters(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        return pulumi.get(self, "masters")
+    @pulumi.getter(name="leastSquaresDecay")
+    def least_squares_decay(self) -> Optional[pulumi.Input[float]]:
+        return pulumi.get(self, "least_squares_decay")
 
-    @masters.setter
-    def masters(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "masters", value)
+    @least_squares_decay.setter
+    def least_squares_decay(self, value: Optional[pulumi.Input[float]]):
+        pulumi.set(self, "least_squares_decay", value)
 
     @property
-    @pulumi.getter(name="signAndServe")
-    def sign_and_serve(self) -> Optional[pulumi.Input[bool]]:
-        return pulumi.get(self, "sign_and_serve")
+    @pulumi.getter(name="loadImbalancePercentage")
+    def load_imbalance_percentage(self) -> Optional[pulumi.Input[float]]:
+        return pulumi.get(self, "load_imbalance_percentage")
 
-    @sign_and_serve.setter
-    def sign_and_serve(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "sign_and_serve", value)
+    @load_imbalance_percentage.setter
+    def load_imbalance_percentage(self, value: Optional[pulumi.Input[float]]):
+        pulumi.set(self, "load_imbalance_percentage", value)
 
     @property
-    @pulumi.getter(name="signAndServeAlgorithm")
-    def sign_and_serve_algorithm(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "sign_and_serve_algorithm")
+    @pulumi.getter(name="maxUMultiplicativeIncrement")
+    def max_u_multiplicative_increment(self) -> Optional[pulumi.Input[float]]:
+        return pulumi.get(self, "max_u_multiplicative_increment")
 
-    @sign_and_serve_algorithm.setter
-    def sign_and_serve_algorithm(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "sign_and_serve_algorithm", value)
+    @max_u_multiplicative_increment.setter
+    def max_u_multiplicative_increment(self, value: Optional[pulumi.Input[float]]):
+        pulumi.set(self, "max_u_multiplicative_increment", value)
 
     @property
     @pulumi.getter
-    def target(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "target")
+    def name(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "name")
 
-    @target.setter
-    def target(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "target", value)
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter(name="tsigKey")
-    def tsig_key(self) -> Optional[pulumi.Input['DnsZoneTsigKeyArgs']]:
-        return pulumi.get(self, "tsig_key")
+    @pulumi.getter(name="resourceInstances")
+    def resource_instances(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['GtmResourceResourceInstanceArgs']]]]:
+        return pulumi.get(self, "resource_instances")
 
-    @tsig_key.setter
-    def tsig_key(self, value: Optional[pulumi.Input['DnsZoneTsigKeyArgs']]):
-        pulumi.set(self, "tsig_key", value)
+    @resource_instances.setter
+    def resource_instances(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['GtmResourceResourceInstanceArgs']]]]):
+        pulumi.set(self, "resource_instances", value)
+
+    @property
+    @pulumi.getter(name="upperBound")
+    def upper_bound(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "upper_bound")
+
+    @upper_bound.setter
+    def upper_bound(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "upper_bound", value)
+
+    @property
+    @pulumi.getter(name="waitOnComplete")
+    def wait_on_complete(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "wait_on_complete")
+
+    @wait_on_complete.setter
+    def wait_on_complete(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "wait_on_complete", value)
 
 
 @pulumi.input_type
-class _DnsZoneState:
+class _GtmResourceState:
     def __init__(__self__, *,
-                 activation_state: Optional[pulumi.Input[str]] = None,
-                 alias_count: Optional[pulumi.Input[int]] = None,
-                 comment: Optional[pulumi.Input[str]] = None,
-                 contract: Optional[pulumi.Input[str]] = None,
-                 end_customer_id: Optional[pulumi.Input[str]] = None,
-                 group: Optional[pulumi.Input[str]] = None,
-                 masters: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 sign_and_serve: Optional[pulumi.Input[bool]] = None,
-                 sign_and_serve_algorithm: Optional[pulumi.Input[str]] = None,
-                 target: Optional[pulumi.Input[str]] = None,
-                 tsig_key: Optional[pulumi.Input['DnsZoneTsigKeyArgs']] = None,
+                 aggregation_type: Optional[pulumi.Input[str]] = None,
+                 constrained_property: Optional[pulumi.Input[str]] = None,
+                 decay_rate: Optional[pulumi.Input[float]] = None,
+                 description: Optional[pulumi.Input[str]] = None,
+                 domain: Optional[pulumi.Input[str]] = None,
+                 host_header: Optional[pulumi.Input[str]] = None,
+                 leader_string: Optional[pulumi.Input[str]] = None,
+                 least_squares_decay: Optional[pulumi.Input[float]] = None,
+                 load_imbalance_percentage: Optional[pulumi.Input[float]] = None,
+                 max_u_multiplicative_increment: Optional[pulumi.Input[float]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 resource_instances: Optional[pulumi.Input[Sequence[pulumi.Input['GtmResourceResourceInstanceArgs']]]] = None,
                  type: Optional[pulumi.Input[str]] = None,
-                 version_id: Optional[pulumi.Input[str]] = None,
-                 zone: Optional[pulumi.Input[str]] = None):
+                 upper_bound: Optional[pulumi.Input[int]] = None,
+                 wait_on_complete: Optional[pulumi.Input[bool]] = None):
         """
-        Input properties used for looking up and filtering DnsZone resources.
+        Input properties used for looking up and filtering GtmResource resources.
         """
-        if activation_state is not None:
-            pulumi.set(__self__, "activation_state", activation_state)
-        if alias_count is not None:
-            pulumi.set(__self__, "alias_count", alias_count)
-        if comment is not None:
-            pulumi.set(__self__, "comment", comment)
-        if contract is not None:
-            pulumi.set(__self__, "contract", contract)
-        if end_customer_id is not None:
-            pulumi.set(__self__, "end_customer_id", end_customer_id)
-        if group is not None:
-            pulumi.set(__self__, "group", group)
-        if masters is not None:
-            pulumi.set(__self__, "masters", masters)
-        if sign_and_serve is not None:
-            pulumi.set(__self__, "sign_and_serve", sign_and_serve)
-        if sign_and_serve_algorithm is not None:
-            pulumi.set(__self__, "sign_and_serve_algorithm", sign_and_serve_algorithm)
-        if target is not None:
-            pulumi.set(__self__, "target", target)
-        if tsig_key is not None:
-            pulumi.set(__self__, "tsig_key", tsig_key)
+        if aggregation_type is not None:
+            pulumi.set(__self__, "aggregation_type", aggregation_type)
+        if constrained_property is not None:
+            pulumi.set(__self__, "constrained_property", constrained_property)
+        if decay_rate is not None:
+            pulumi.set(__self__, "decay_rate", decay_rate)
+        if description is not None:
+            pulumi.set(__self__, "description", description)
+        if domain is not None:
+            pulumi.set(__self__, "domain", domain)
+        if host_header is not None:
+            pulumi.set(__self__, "host_header", host_header)
+        if leader_string is not None:
+            pulumi.set(__self__, "leader_string", leader_string)
+        if least_squares_decay is not None:
+            pulumi.set(__self__, "least_squares_decay", least_squares_decay)
+        if load_imbalance_percentage is not None:
+            pulumi.set(__self__, "load_imbalance_percentage", load_imbalance_percentage)
+        if max_u_multiplicative_increment is not None:
+            pulumi.set(__self__, "max_u_multiplicative_increment", max_u_multiplicative_increment)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if resource_instances is not None:
+            pulumi.set(__self__, "resource_instances", resource_instances)
         if type is not None:
             pulumi.set(__self__, "type", type)
-        if version_id is not None:
-            pulumi.set(__self__, "version_id", version_id)
-        if zone is not None:
-            pulumi.set(__self__, "zone", zone)
+        if upper_bound is not None:
+            pulumi.set(__self__, "upper_bound", upper_bound)
+        if wait_on_complete is not None:
+            pulumi.set(__self__, "wait_on_complete", wait_on_complete)
+
+    @property
+    @pulumi.getter(name="aggregationType")
+    def aggregation_type(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "aggregation_type")
+
+    @aggregation_type.setter
+    def aggregation_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "aggregation_type", value)
 
     @property
-    @pulumi.getter(name="activationState")
-    def activation_state(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "activation_state")
+    @pulumi.getter(name="constrainedProperty")
+    def constrained_property(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "constrained_property")
 
-    @activation_state.setter
-    def activation_state(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "activation_state", value)
+    @constrained_property.setter
+    def constrained_property(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "constrained_property", value)
 
     @property
-    @pulumi.getter(name="aliasCount")
-    def alias_count(self) -> Optional[pulumi.Input[int]]:
-        return pulumi.get(self, "alias_count")
+    @pulumi.getter(name="decayRate")
+    def decay_rate(self) -> Optional[pulumi.Input[float]]:
+        return pulumi.get(self, "decay_rate")
 
-    @alias_count.setter
-    def alias_count(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "alias_count", value)
+    @decay_rate.setter
+    def decay_rate(self, value: Optional[pulumi.Input[float]]):
+        pulumi.set(self, "decay_rate", value)
 
     @property
     @pulumi.getter
-    def comment(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "comment")
+    def description(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "description")
 
-    @comment.setter
-    def comment(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "comment", value)
+    @description.setter
+    def description(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter
-    def contract(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "contract")
+    def domain(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "domain")
 
-    @contract.setter
-    def contract(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "contract", value)
+    @domain.setter
+    def domain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "domain", value)
 
     @property
-    @pulumi.getter(name="endCustomerId")
-    def end_customer_id(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "end_customer_id")
+    @pulumi.getter(name="hostHeader")
+    def host_header(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "host_header")
 
-    @end_customer_id.setter
-    def end_customer_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "end_customer_id", value)
+    @host_header.setter
+    def host_header(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "host_header", value)
 
     @property
-    @pulumi.getter
-    def group(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "group")
+    @pulumi.getter(name="leaderString")
+    def leader_string(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "leader_string")
 
-    @group.setter
-    def group(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "group", value)
+    @leader_string.setter
+    def leader_string(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "leader_string", value)
 
     @property
-    @pulumi.getter
-    def masters(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        return pulumi.get(self, "masters")
+    @pulumi.getter(name="leastSquaresDecay")
+    def least_squares_decay(self) -> Optional[pulumi.Input[float]]:
+        return pulumi.get(self, "least_squares_decay")
 
-    @masters.setter
-    def masters(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "masters", value)
+    @least_squares_decay.setter
+    def least_squares_decay(self, value: Optional[pulumi.Input[float]]):
+        pulumi.set(self, "least_squares_decay", value)
 
     @property
-    @pulumi.getter(name="signAndServe")
-    def sign_and_serve(self) -> Optional[pulumi.Input[bool]]:
-        return pulumi.get(self, "sign_and_serve")
+    @pulumi.getter(name="loadImbalancePercentage")
+    def load_imbalance_percentage(self) -> Optional[pulumi.Input[float]]:
+        return pulumi.get(self, "load_imbalance_percentage")
 
-    @sign_and_serve.setter
-    def sign_and_serve(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "sign_and_serve", value)
+    @load_imbalance_percentage.setter
+    def load_imbalance_percentage(self, value: Optional[pulumi.Input[float]]):
+        pulumi.set(self, "load_imbalance_percentage", value)
 
     @property
-    @pulumi.getter(name="signAndServeAlgorithm")
-    def sign_and_serve_algorithm(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "sign_and_serve_algorithm")
+    @pulumi.getter(name="maxUMultiplicativeIncrement")
+    def max_u_multiplicative_increment(self) -> Optional[pulumi.Input[float]]:
+        return pulumi.get(self, "max_u_multiplicative_increment")
 
-    @sign_and_serve_algorithm.setter
-    def sign_and_serve_algorithm(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "sign_and_serve_algorithm", value)
+    @max_u_multiplicative_increment.setter
+    def max_u_multiplicative_increment(self, value: Optional[pulumi.Input[float]]):
+        pulumi.set(self, "max_u_multiplicative_increment", value)
 
     @property
     @pulumi.getter
-    def target(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "target")
+    def name(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "name")
 
-    @target.setter
-    def target(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "target", value)
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter(name="tsigKey")
-    def tsig_key(self) -> Optional[pulumi.Input['DnsZoneTsigKeyArgs']]:
-        return pulumi.get(self, "tsig_key")
+    @pulumi.getter(name="resourceInstances")
+    def resource_instances(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['GtmResourceResourceInstanceArgs']]]]:
+        return pulumi.get(self, "resource_instances")
 
-    @tsig_key.setter
-    def tsig_key(self, value: Optional[pulumi.Input['DnsZoneTsigKeyArgs']]):
-        pulumi.set(self, "tsig_key", value)
+    @resource_instances.setter
+    def resource_instances(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['GtmResourceResourceInstanceArgs']]]]):
+        pulumi.set(self, "resource_instances", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
     @property
-    @pulumi.getter(name="versionId")
-    def version_id(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "version_id")
+    @pulumi.getter(name="upperBound")
+    def upper_bound(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "upper_bound")
 
-    @version_id.setter
-    def version_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "version_id", value)
+    @upper_bound.setter
+    def upper_bound(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "upper_bound", value)
 
     @property
-    @pulumi.getter
-    def zone(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "zone")
-
-    @zone.setter
-    def zone(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "zone", value)
-
+    @pulumi.getter(name="waitOnComplete")
+    def wait_on_complete(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "wait_on_complete")
 
-warnings.warn("""akamai.edgedns/dnszone.DnsZone has been deprecated in favor of akamai.index/dnszone.DnsZone""", DeprecationWarning)
+    @wait_on_complete.setter
+    def wait_on_complete(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "wait_on_complete", value)
 
 
-class DnsZone(pulumi.CustomResource):
-    warnings.warn("""akamai.edgedns/dnszone.DnsZone has been deprecated in favor of akamai.index/dnszone.DnsZone""", DeprecationWarning)
-
+class GtmResource(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 comment: Optional[pulumi.Input[str]] = None,
-                 contract: Optional[pulumi.Input[str]] = None,
-                 end_customer_id: Optional[pulumi.Input[str]] = None,
-                 group: Optional[pulumi.Input[str]] = None,
-                 masters: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 sign_and_serve: Optional[pulumi.Input[bool]] = None,
-                 sign_and_serve_algorithm: Optional[pulumi.Input[str]] = None,
-                 target: Optional[pulumi.Input[str]] = None,
-                 tsig_key: Optional[pulumi.Input[pulumi.InputType['DnsZoneTsigKeyArgs']]] = None,
+                 aggregation_type: Optional[pulumi.Input[str]] = None,
+                 constrained_property: Optional[pulumi.Input[str]] = None,
+                 decay_rate: Optional[pulumi.Input[float]] = None,
+                 description: Optional[pulumi.Input[str]] = None,
+                 domain: Optional[pulumi.Input[str]] = None,
+                 host_header: Optional[pulumi.Input[str]] = None,
+                 leader_string: Optional[pulumi.Input[str]] = None,
+                 least_squares_decay: Optional[pulumi.Input[float]] = None,
+                 load_imbalance_percentage: Optional[pulumi.Input[float]] = None,
+                 max_u_multiplicative_increment: Optional[pulumi.Input[float]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 resource_instances: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['GtmResourceResourceInstanceArgs']]]]] = None,
                  type: Optional[pulumi.Input[str]] = None,
-                 zone: Optional[pulumi.Input[str]] = None,
+                 upper_bound: Optional[pulumi.Input[int]] = None,
+                 wait_on_complete: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
-        Create a DnsZone resource with the given unique name, props, and options.
+        Create a GtmResource resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: DnsZoneArgs,
+                 args: GtmResourceArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a DnsZone resource with the given unique name, props, and options.
+        Create a GtmResource resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
-        :param DnsZoneArgs args: The arguments to use to populate this resource's properties.
+        :param GtmResourceArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(DnsZoneArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(GtmResourceArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 comment: Optional[pulumi.Input[str]] = None,
-                 contract: Optional[pulumi.Input[str]] = None,
-                 end_customer_id: Optional[pulumi.Input[str]] = None,
-                 group: Optional[pulumi.Input[str]] = None,
-                 masters: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 sign_and_serve: Optional[pulumi.Input[bool]] = None,
-                 sign_and_serve_algorithm: Optional[pulumi.Input[str]] = None,
-                 target: Optional[pulumi.Input[str]] = None,
-                 tsig_key: Optional[pulumi.Input[pulumi.InputType['DnsZoneTsigKeyArgs']]] = None,
+                 aggregation_type: Optional[pulumi.Input[str]] = None,
+                 constrained_property: Optional[pulumi.Input[str]] = None,
+                 decay_rate: Optional[pulumi.Input[float]] = None,
+                 description: Optional[pulumi.Input[str]] = None,
+                 domain: Optional[pulumi.Input[str]] = None,
+                 host_header: Optional[pulumi.Input[str]] = None,
+                 leader_string: Optional[pulumi.Input[str]] = None,
+                 least_squares_decay: Optional[pulumi.Input[float]] = None,
+                 load_imbalance_percentage: Optional[pulumi.Input[float]] = None,
+                 max_u_multiplicative_increment: Optional[pulumi.Input[float]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 resource_instances: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['GtmResourceResourceInstanceArgs']]]]] = None,
                  type: Optional[pulumi.Input[str]] = None,
-                 zone: Optional[pulumi.Input[str]] = None,
+                 upper_bound: Optional[pulumi.Input[int]] = None,
+                 wait_on_complete: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
-        pulumi.log.warn("""DnsZone is deprecated: akamai.edgedns/dnszone.DnsZone has been deprecated in favor of akamai.index/dnszone.DnsZone""")
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = DnsZoneArgs.__new__(DnsZoneArgs)
+            __props__ = GtmResourceArgs.__new__(GtmResourceArgs)
 
-            __props__.__dict__["comment"] = comment
-            if contract is None and not opts.urn:
-                raise TypeError("Missing required property 'contract'")
-            __props__.__dict__["contract"] = contract
-            __props__.__dict__["end_customer_id"] = end_customer_id
-            __props__.__dict__["group"] = group
-            __props__.__dict__["masters"] = masters
-            __props__.__dict__["sign_and_serve"] = sign_and_serve
-            __props__.__dict__["sign_and_serve_algorithm"] = sign_and_serve_algorithm
-            __props__.__dict__["target"] = target
-            __props__.__dict__["tsig_key"] = tsig_key
+            if aggregation_type is None and not opts.urn:
+                raise TypeError("Missing required property 'aggregation_type'")
+            __props__.__dict__["aggregation_type"] = aggregation_type
+            __props__.__dict__["constrained_property"] = constrained_property
+            __props__.__dict__["decay_rate"] = decay_rate
+            __props__.__dict__["description"] = description
+            if domain is None and not opts.urn:
+                raise TypeError("Missing required property 'domain'")
+            __props__.__dict__["domain"] = domain
+            __props__.__dict__["host_header"] = host_header
+            __props__.__dict__["leader_string"] = leader_string
+            __props__.__dict__["least_squares_decay"] = least_squares_decay
+            __props__.__dict__["load_imbalance_percentage"] = load_imbalance_percentage
+            __props__.__dict__["max_u_multiplicative_increment"] = max_u_multiplicative_increment
+            __props__.__dict__["name"] = name
+            __props__.__dict__["resource_instances"] = resource_instances
             if type is None and not opts.urn:
                 raise TypeError("Missing required property 'type'")
             __props__.__dict__["type"] = type
-            if zone is None and not opts.urn:
-                raise TypeError("Missing required property 'zone'")
-            __props__.__dict__["zone"] = zone
-            __props__.__dict__["activation_state"] = None
-            __props__.__dict__["alias_count"] = None
-            __props__.__dict__["version_id"] = None
-        super(DnsZone, __self__).__init__(
-            'akamai:edgedns/dnsZone:DnsZone',
+            __props__.__dict__["upper_bound"] = upper_bound
+            __props__.__dict__["wait_on_complete"] = wait_on_complete
+        alias_opts = pulumi.ResourceOptions(aliases=[pulumi.Alias(type_="akamai:trafficmanagement/gtmResource:GtmResource")])
+        opts = pulumi.ResourceOptions.merge(opts, alias_opts)
+        super(GtmResource, __self__).__init__(
+            'akamai:index/gtmResource:GtmResource',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            activation_state: Optional[pulumi.Input[str]] = None,
-            alias_count: Optional[pulumi.Input[int]] = None,
-            comment: Optional[pulumi.Input[str]] = None,
-            contract: Optional[pulumi.Input[str]] = None,
-            end_customer_id: Optional[pulumi.Input[str]] = None,
-            group: Optional[pulumi.Input[str]] = None,
-            masters: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-            sign_and_serve: Optional[pulumi.Input[bool]] = None,
-            sign_and_serve_algorithm: Optional[pulumi.Input[str]] = None,
-            target: Optional[pulumi.Input[str]] = None,
-            tsig_key: Optional[pulumi.Input[pulumi.InputType['DnsZoneTsigKeyArgs']]] = None,
+            aggregation_type: Optional[pulumi.Input[str]] = None,
+            constrained_property: Optional[pulumi.Input[str]] = None,
+            decay_rate: Optional[pulumi.Input[float]] = None,
+            description: Optional[pulumi.Input[str]] = None,
+            domain: Optional[pulumi.Input[str]] = None,
+            host_header: Optional[pulumi.Input[str]] = None,
+            leader_string: Optional[pulumi.Input[str]] = None,
+            least_squares_decay: Optional[pulumi.Input[float]] = None,
+            load_imbalance_percentage: Optional[pulumi.Input[float]] = None,
+            max_u_multiplicative_increment: Optional[pulumi.Input[float]] = None,
+            name: Optional[pulumi.Input[str]] = None,
+            resource_instances: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['GtmResourceResourceInstanceArgs']]]]] = None,
             type: Optional[pulumi.Input[str]] = None,
-            version_id: Optional[pulumi.Input[str]] = None,
-            zone: Optional[pulumi.Input[str]] = None) -> 'DnsZone':
+            upper_bound: Optional[pulumi.Input[int]] = None,
+            wait_on_complete: Optional[pulumi.Input[bool]] = None) -> 'GtmResource':
         """
-        Get an existing DnsZone resource's state with the given name, id, and optional extra
+        Get an existing GtmResource resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _DnsZoneState.__new__(_DnsZoneState)
+        __props__ = _GtmResourceState.__new__(_GtmResourceState)
 
-        __props__.__dict__["activation_state"] = activation_state
-        __props__.__dict__["alias_count"] = alias_count
-        __props__.__dict__["comment"] = comment
-        __props__.__dict__["contract"] = contract
-        __props__.__dict__["end_customer_id"] = end_customer_id
-        __props__.__dict__["group"] = group
-        __props__.__dict__["masters"] = masters
-        __props__.__dict__["sign_and_serve"] = sign_and_serve
-        __props__.__dict__["sign_and_serve_algorithm"] = sign_and_serve_algorithm
-        __props__.__dict__["target"] = target
-        __props__.__dict__["tsig_key"] = tsig_key
+        __props__.__dict__["aggregation_type"] = aggregation_type
+        __props__.__dict__["constrained_property"] = constrained_property
+        __props__.__dict__["decay_rate"] = decay_rate
+        __props__.__dict__["description"] = description
+        __props__.__dict__["domain"] = domain
+        __props__.__dict__["host_header"] = host_header
+        __props__.__dict__["leader_string"] = leader_string
+        __props__.__dict__["least_squares_decay"] = least_squares_decay
+        __props__.__dict__["load_imbalance_percentage"] = load_imbalance_percentage
+        __props__.__dict__["max_u_multiplicative_increment"] = max_u_multiplicative_increment
+        __props__.__dict__["name"] = name
+        __props__.__dict__["resource_instances"] = resource_instances
         __props__.__dict__["type"] = type
-        __props__.__dict__["version_id"] = version_id
-        __props__.__dict__["zone"] = zone
-        return DnsZone(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["upper_bound"] = upper_bound
+        __props__.__dict__["wait_on_complete"] = wait_on_complete
+        return GtmResource(resource_name, opts=opts, __props__=__props__)
+
+    @property
+    @pulumi.getter(name="aggregationType")
+    def aggregation_type(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "aggregation_type")
 
     @property
-    @pulumi.getter(name="activationState")
-    def activation_state(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "activation_state")
+    @pulumi.getter(name="constrainedProperty")
+    def constrained_property(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "constrained_property")
 
     @property
-    @pulumi.getter(name="aliasCount")
-    def alias_count(self) -> pulumi.Output[int]:
-        return pulumi.get(self, "alias_count")
+    @pulumi.getter(name="decayRate")
+    def decay_rate(self) -> pulumi.Output[Optional[float]]:
+        return pulumi.get(self, "decay_rate")
 
     @property
     @pulumi.getter
-    def comment(self) -> pulumi.Output[Optional[str]]:
-        return pulumi.get(self, "comment")
+    def description(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
-    def contract(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "contract")
+    def domain(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "domain")
 
     @property
-    @pulumi.getter(name="endCustomerId")
-    def end_customer_id(self) -> pulumi.Output[Optional[str]]:
-        return pulumi.get(self, "end_customer_id")
+    @pulumi.getter(name="hostHeader")
+    def host_header(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "host_header")
 
     @property
-    @pulumi.getter
-    def group(self) -> pulumi.Output[Optional[str]]:
-        return pulumi.get(self, "group")
+    @pulumi.getter(name="leaderString")
+    def leader_string(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "leader_string")
 
     @property
-    @pulumi.getter
-    def masters(self) -> pulumi.Output[Optional[Sequence[str]]]:
-        return pulumi.get(self, "masters")
+    @pulumi.getter(name="leastSquaresDecay")
+    def least_squares_decay(self) -> pulumi.Output[Optional[float]]:
+        return pulumi.get(self, "least_squares_decay")
 
     @property
-    @pulumi.getter(name="signAndServe")
-    def sign_and_serve(self) -> pulumi.Output[Optional[bool]]:
-        return pulumi.get(self, "sign_and_serve")
+    @pulumi.getter(name="loadImbalancePercentage")
+    def load_imbalance_percentage(self) -> pulumi.Output[Optional[float]]:
+        return pulumi.get(self, "load_imbalance_percentage")
 
     @property
-    @pulumi.getter(name="signAndServeAlgorithm")
-    def sign_and_serve_algorithm(self) -> pulumi.Output[Optional[str]]:
-        return pulumi.get(self, "sign_and_serve_algorithm")
+    @pulumi.getter(name="maxUMultiplicativeIncrement")
+    def max_u_multiplicative_increment(self) -> pulumi.Output[Optional[float]]:
+        return pulumi.get(self, "max_u_multiplicative_increment")
 
     @property
     @pulumi.getter
-    def target(self) -> pulumi.Output[Optional[str]]:
-        return pulumi.get(self, "target")
+    def name(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "name")
 
     @property
-    @pulumi.getter(name="tsigKey")
-    def tsig_key(self) -> pulumi.Output[Optional['outputs.DnsZoneTsigKey']]:
-        return pulumi.get(self, "tsig_key")
+    @pulumi.getter(name="resourceInstances")
+    def resource_instances(self) -> pulumi.Output[Optional[Sequence['outputs.GtmResourceResourceInstance']]]:
+        return pulumi.get(self, "resource_instances")
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Output[str]:
         return pulumi.get(self, "type")
 
     @property
-    @pulumi.getter(name="versionId")
-    def version_id(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "version_id")
+    @pulumi.getter(name="upperBound")
+    def upper_bound(self) -> pulumi.Output[Optional[int]]:
+        return pulumi.get(self, "upper_bound")
 
     @property
-    @pulumi.getter
-    def zone(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "zone")
+    @pulumi.getter(name="waitOnComplete")
+    def wait_on_complete(self) -> pulumi.Output[Optional[bool]]:
+        return pulumi.get(self, "wait_on_complete")
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edgedns/get_authorities_set.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/edgedns/get_authorities_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,17 +72,17 @@
     pulumi.log.warn("""get_authorities_set is deprecated: akamai.edgedns/getauthoritiesset.getAuthoritiesSet has been deprecated in favor of akamai.index/getauthoritiesset.getAuthoritiesSet""")
     __args__ = dict()
     __args__['contract'] = contract
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:edgedns/getAuthoritiesSet:getAuthoritiesSet', __args__, opts=opts, typ=GetAuthoritiesSetResult).value
 
     return AwaitableGetAuthoritiesSetResult(
-        authorities=__ret__.authorities,
-        contract=__ret__.contract,
-        id=__ret__.id)
+        authorities=pulumi.get(__ret__, 'authorities'),
+        contract=pulumi.get(__ret__, 'contract'),
+        id=pulumi.get(__ret__, 'id'))
 
 
 @_utilities.lift_output_func(get_authorities_set)
 def get_authorities_set_output(contract: Optional[pulumi.Input[str]] = None,
                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAuthoritiesSetResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edgedns/get_dns_record_set.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/edgedns/get_dns_record_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,19 +94,19 @@
     __args__['host'] = host
     __args__['recordType'] = record_type
     __args__['zone'] = zone
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:edgedns/getDnsRecordSet:getDnsRecordSet', __args__, opts=opts, typ=GetDnsRecordSetResult).value
 
     return AwaitableGetDnsRecordSetResult(
-        host=__ret__.host,
-        id=__ret__.id,
-        rdatas=__ret__.rdatas,
-        record_type=__ret__.record_type,
-        zone=__ret__.zone)
+        host=pulumi.get(__ret__, 'host'),
+        id=pulumi.get(__ret__, 'id'),
+        rdatas=pulumi.get(__ret__, 'rdatas'),
+        record_type=pulumi.get(__ret__, 'record_type'),
+        zone=pulumi.get(__ret__, 'zone'))
 
 
 @_utilities.lift_output_func(get_dns_record_set)
 def get_dns_record_set_output(host: Optional[pulumi.Input[str]] = None,
                               record_type: Optional[pulumi.Input[str]] = None,
                               zone: Optional[pulumi.Input[str]] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDnsRecordSetResult]:
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edgekv_group_items.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/edgekv_group_items.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_advanced_settings_evasive_path_match.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_advanced_settings_evasive_path_match.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,19 +89,19 @@
     __args__ = dict()
     __args__['configId'] = config_id
     __args__['securityPolicyId'] = security_policy_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecAdvancedSettingsEvasivePathMatch:getAppSecAdvancedSettingsEvasivePathMatch', __args__, opts=opts, typ=GetAppSecAdvancedSettingsEvasivePathMatchResult).value
 
     return AwaitableGetAppSecAdvancedSettingsEvasivePathMatchResult(
-        config_id=__ret__.config_id,
-        id=__ret__.id,
-        json=__ret__.json,
-        output_text=__ret__.output_text,
-        security_policy_id=__ret__.security_policy_id)
+        config_id=pulumi.get(__ret__, 'config_id'),
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        output_text=pulumi.get(__ret__, 'output_text'),
+        security_policy_id=pulumi.get(__ret__, 'security_policy_id'))
 
 
 @_utilities.lift_output_func(get_app_sec_advanced_settings_evasive_path_match)
 def get_app_sec_advanced_settings_evasive_path_match_output(config_id: Optional[pulumi.Input[int]] = None,
                                                             security_policy_id: Optional[pulumi.Input[Optional[str]]] = None,
                                                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecAdvancedSettingsEvasivePathMatchResult]:
     """
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_advanced_settings_logging.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_advanced_settings_logging.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,19 +89,19 @@
     __args__ = dict()
     __args__['configId'] = config_id
     __args__['securityPolicyId'] = security_policy_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecAdvancedSettingsLogging:getAppSecAdvancedSettingsLogging', __args__, opts=opts, typ=GetAppSecAdvancedSettingsLoggingResult).value
 
     return AwaitableGetAppSecAdvancedSettingsLoggingResult(
-        config_id=__ret__.config_id,
-        id=__ret__.id,
-        json=__ret__.json,
-        output_text=__ret__.output_text,
-        security_policy_id=__ret__.security_policy_id)
+        config_id=pulumi.get(__ret__, 'config_id'),
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        output_text=pulumi.get(__ret__, 'output_text'),
+        security_policy_id=pulumi.get(__ret__, 'security_policy_id'))
 
 
 @_utilities.lift_output_func(get_app_sec_advanced_settings_logging)
 def get_app_sec_advanced_settings_logging_output(config_id: Optional[pulumi.Input[int]] = None,
                                                  security_policy_id: Optional[pulumi.Input[Optional[str]]] = None,
                                                  opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecAdvancedSettingsLoggingResult]:
     """
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_advanced_settings_pragma_header.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_advanced_settings_pragma_header.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,19 +89,19 @@
     __args__ = dict()
     __args__['configId'] = config_id
     __args__['securityPolicyId'] = security_policy_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecAdvancedSettingsPragmaHeader:getAppSecAdvancedSettingsPragmaHeader', __args__, opts=opts, typ=GetAppSecAdvancedSettingsPragmaHeaderResult).value
 
     return AwaitableGetAppSecAdvancedSettingsPragmaHeaderResult(
-        config_id=__ret__.config_id,
-        id=__ret__.id,
-        json=__ret__.json,
-        output_text=__ret__.output_text,
-        security_policy_id=__ret__.security_policy_id)
+        config_id=pulumi.get(__ret__, 'config_id'),
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        output_text=pulumi.get(__ret__, 'output_text'),
+        security_policy_id=pulumi.get(__ret__, 'security_policy_id'))
 
 
 @_utilities.lift_output_func(get_app_sec_advanced_settings_pragma_header)
 def get_app_sec_advanced_settings_pragma_header_output(config_id: Optional[pulumi.Input[int]] = None,
                                                        security_policy_id: Optional[pulumi.Input[Optional[str]]] = None,
                                                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecAdvancedSettingsPragmaHeaderResult]:
     """
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_advanced_settings_prefetch.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_advanced_settings_prefetch.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,18 +78,18 @@
     """
     __args__ = dict()
     __args__['configId'] = config_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecAdvancedSettingsPrefetch:getAppSecAdvancedSettingsPrefetch', __args__, opts=opts, typ=GetAppSecAdvancedSettingsPrefetchResult).value
 
     return AwaitableGetAppSecAdvancedSettingsPrefetchResult(
-        config_id=__ret__.config_id,
-        id=__ret__.id,
-        json=__ret__.json,
-        output_text=__ret__.output_text)
+        config_id=pulumi.get(__ret__, 'config_id'),
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        output_text=pulumi.get(__ret__, 'output_text'))
 
 
 @_utilities.lift_output_func(get_app_sec_advanced_settings_prefetch)
 def get_app_sec_advanced_settings_prefetch_output(config_id: Optional[pulumi.Input[int]] = None,
                                                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecAdvancedSettingsPrefetchResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_api_endpoints.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_api_endpoints.py`

 * *Files 9% similar despite different names*

```diff
@@ -109,21 +109,21 @@
     __args__['apiName'] = api_name
     __args__['configId'] = config_id
     __args__['securityPolicyId'] = security_policy_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecApiEndpoints:getAppSecApiEndpoints', __args__, opts=opts, typ=GetAppSecApiEndpointsResult).value
 
     return AwaitableGetAppSecApiEndpointsResult(
-        api_name=__ret__.api_name,
-        config_id=__ret__.config_id,
-        id=__ret__.id,
-        id_lists=__ret__.id_lists,
-        json=__ret__.json,
-        output_text=__ret__.output_text,
-        security_policy_id=__ret__.security_policy_id)
+        api_name=pulumi.get(__ret__, 'api_name'),
+        config_id=pulumi.get(__ret__, 'config_id'),
+        id=pulumi.get(__ret__, 'id'),
+        id_lists=pulumi.get(__ret__, 'id_lists'),
+        json=pulumi.get(__ret__, 'json'),
+        output_text=pulumi.get(__ret__, 'output_text'),
+        security_policy_id=pulumi.get(__ret__, 'security_policy_id'))
 
 
 @_utilities.lift_output_func(get_app_sec_api_endpoints)
 def get_app_sec_api_endpoints_output(api_name: Optional[pulumi.Input[Optional[str]]] = None,
                                      config_id: Optional[pulumi.Input[int]] = None,
                                      security_policy_id: Optional[pulumi.Input[Optional[str]]] = None,
                                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecApiEndpointsResult]:
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_api_request_constraints.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_api_request_constraints.py`

 * *Files 8% similar despite different names*

```diff
@@ -100,20 +100,20 @@
     __args__['apiId'] = api_id
     __args__['configId'] = config_id
     __args__['securityPolicyId'] = security_policy_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecApiRequestConstraints:getAppSecApiRequestConstraints', __args__, opts=opts, typ=GetAppSecApiRequestConstraintsResult).value
 
     return AwaitableGetAppSecApiRequestConstraintsResult(
-        api_id=__ret__.api_id,
-        config_id=__ret__.config_id,
-        id=__ret__.id,
-        json=__ret__.json,
-        output_text=__ret__.output_text,
-        security_policy_id=__ret__.security_policy_id)
+        api_id=pulumi.get(__ret__, 'api_id'),
+        config_id=pulumi.get(__ret__, 'config_id'),
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        output_text=pulumi.get(__ret__, 'output_text'),
+        security_policy_id=pulumi.get(__ret__, 'security_policy_id'))
 
 
 @_utilities.lift_output_func(get_app_sec_api_request_constraints)
 def get_app_sec_api_request_constraints_output(api_id: Optional[pulumi.Input[Optional[int]]] = None,
                                                config_id: Optional[pulumi.Input[int]] = None,
                                                security_policy_id: Optional[pulumi.Input[str]] = None,
                                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecApiRequestConstraintsResult]:
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_attack_groups.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_attack_groups.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,22 +118,22 @@
     __args__['attackGroup'] = attack_group
     __args__['configId'] = config_id
     __args__['securityPolicyId'] = security_policy_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecAttackGroups:getAppSecAttackGroups', __args__, opts=opts, typ=GetAppSecAttackGroupsResult).value
 
     return AwaitableGetAppSecAttackGroupsResult(
-        attack_group=__ret__.attack_group,
-        attack_group_action=__ret__.attack_group_action,
-        condition_exception=__ret__.condition_exception,
-        config_id=__ret__.config_id,
-        id=__ret__.id,
-        json=__ret__.json,
-        output_text=__ret__.output_text,
-        security_policy_id=__ret__.security_policy_id)
+        attack_group=pulumi.get(__ret__, 'attack_group'),
+        attack_group_action=pulumi.get(__ret__, 'attack_group_action'),
+        condition_exception=pulumi.get(__ret__, 'condition_exception'),
+        config_id=pulumi.get(__ret__, 'config_id'),
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        output_text=pulumi.get(__ret__, 'output_text'),
+        security_policy_id=pulumi.get(__ret__, 'security_policy_id'))
 
 
 @_utilities.lift_output_func(get_app_sec_attack_groups)
 def get_app_sec_attack_groups_output(attack_group: Optional[pulumi.Input[Optional[str]]] = None,
                                      config_id: Optional[pulumi.Input[int]] = None,
                                      security_policy_id: Optional[pulumi.Input[str]] = None,
                                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecAttackGroupsResult]:
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_bypass_network_lists.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_bypass_network_lists.py`

 * *Files 5% similar despite different names*

```diff
@@ -98,20 +98,20 @@
     __args__ = dict()
     __args__['configId'] = config_id
     __args__['securityPolicyId'] = security_policy_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecBypassNetworkLists:getAppSecBypassNetworkLists', __args__, opts=opts, typ=GetAppSecBypassNetworkListsResult).value
 
     return AwaitableGetAppSecBypassNetworkListsResult(
-        bypass_network_lists=__ret__.bypass_network_lists,
-        config_id=__ret__.config_id,
-        id=__ret__.id,
-        json=__ret__.json,
-        output_text=__ret__.output_text,
-        security_policy_id=__ret__.security_policy_id)
+        bypass_network_lists=pulumi.get(__ret__, 'bypass_network_lists'),
+        config_id=pulumi.get(__ret__, 'config_id'),
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        output_text=pulumi.get(__ret__, 'output_text'),
+        security_policy_id=pulumi.get(__ret__, 'security_policy_id'))
 
 
 @_utilities.lift_output_func(get_app_sec_bypass_network_lists)
 def get_app_sec_bypass_network_lists_output(config_id: Optional[pulumi.Input[int]] = None,
                                             security_policy_id: Optional[pulumi.Input[str]] = None,
                                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecBypassNetworkListsResult]:
     """
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_configuration.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_configuration.py`

 * *Files 5% similar despite different names*

```diff
@@ -105,21 +105,21 @@
     """
     __args__ = dict()
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecConfiguration:getAppSecConfiguration', __args__, opts=opts, typ=GetAppSecConfigurationResult).value
 
     return AwaitableGetAppSecConfigurationResult(
-        config_id=__ret__.config_id,
-        id=__ret__.id,
-        latest_version=__ret__.latest_version,
-        name=__ret__.name,
-        output_text=__ret__.output_text,
-        production_version=__ret__.production_version,
-        staging_version=__ret__.staging_version)
+        config_id=pulumi.get(__ret__, 'config_id'),
+        id=pulumi.get(__ret__, 'id'),
+        latest_version=pulumi.get(__ret__, 'latest_version'),
+        name=pulumi.get(__ret__, 'name'),
+        output_text=pulumi.get(__ret__, 'output_text'),
+        production_version=pulumi.get(__ret__, 'production_version'),
+        staging_version=pulumi.get(__ret__, 'staging_version'))
 
 
 @_utilities.lift_output_func(get_app_sec_configuration)
 def get_app_sec_configuration_output(name: Optional[pulumi.Input[Optional[str]]] = None,
                                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecConfigurationResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_configuration_version.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_configuration_version.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,21 +107,21 @@
     __args__ = dict()
     __args__['configId'] = config_id
     __args__['version'] = version
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecConfigurationVersion:getAppSecConfigurationVersion', __args__, opts=opts, typ=GetAppSecConfigurationVersionResult).value
 
     return AwaitableGetAppSecConfigurationVersionResult(
-        config_id=__ret__.config_id,
-        id=__ret__.id,
-        latest_version=__ret__.latest_version,
-        output_text=__ret__.output_text,
-        production_status=__ret__.production_status,
-        staging_status=__ret__.staging_status,
-        version=__ret__.version)
+        config_id=pulumi.get(__ret__, 'config_id'),
+        id=pulumi.get(__ret__, 'id'),
+        latest_version=pulumi.get(__ret__, 'latest_version'),
+        output_text=pulumi.get(__ret__, 'output_text'),
+        production_status=pulumi.get(__ret__, 'production_status'),
+        staging_status=pulumi.get(__ret__, 'staging_status'),
+        version=pulumi.get(__ret__, 'version'))
 
 
 @_utilities.lift_output_func(get_app_sec_configuration_version)
 def get_app_sec_configuration_version_output(config_id: Optional[pulumi.Input[int]] = None,
                                              version: Optional[pulumi.Input[Optional[int]]] = None,
                                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecConfigurationVersionResult]:
     """
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_contracts_groups.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_contracts_groups.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,21 +107,21 @@
     __args__ = dict()
     __args__['contractid'] = contractid
     __args__['groupid'] = groupid
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecContractsGroups:getAppSecContractsGroups', __args__, opts=opts, typ=GetAppSecContractsGroupsResult).value
 
     return AwaitableGetAppSecContractsGroupsResult(
-        contractid=__ret__.contractid,
-        default_contractid=__ret__.default_contractid,
-        default_groupid=__ret__.default_groupid,
-        groupid=__ret__.groupid,
-        id=__ret__.id,
-        json=__ret__.json,
-        output_text=__ret__.output_text)
+        contractid=pulumi.get(__ret__, 'contractid'),
+        default_contractid=pulumi.get(__ret__, 'default_contractid'),
+        default_groupid=pulumi.get(__ret__, 'default_groupid'),
+        groupid=pulumi.get(__ret__, 'groupid'),
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        output_text=pulumi.get(__ret__, 'output_text'))
 
 
 @_utilities.lift_output_func(get_app_sec_contracts_groups)
 def get_app_sec_contracts_groups_output(contractid: Optional[pulumi.Input[Optional[str]]] = None,
                                         groupid: Optional[pulumi.Input[Optional[int]]] = None,
                                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecContractsGroupsResult]:
     """
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_custom_deny.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_custom_deny.py`

 * *Files 6% similar despite different names*

```diff
@@ -89,19 +89,19 @@
     __args__ = dict()
     __args__['configId'] = config_id
     __args__['customDenyId'] = custom_deny_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecCustomDeny:getAppSecCustomDeny', __args__, opts=opts, typ=GetAppSecCustomDenyResult).value
 
     return AwaitableGetAppSecCustomDenyResult(
-        config_id=__ret__.config_id,
-        custom_deny_id=__ret__.custom_deny_id,
-        id=__ret__.id,
-        json=__ret__.json,
-        output_text=__ret__.output_text)
+        config_id=pulumi.get(__ret__, 'config_id'),
+        custom_deny_id=pulumi.get(__ret__, 'custom_deny_id'),
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        output_text=pulumi.get(__ret__, 'output_text'))
 
 
 @_utilities.lift_output_func(get_app_sec_custom_deny)
 def get_app_sec_custom_deny_output(config_id: Optional[pulumi.Input[int]] = None,
                                    custom_deny_id: Optional[pulumi.Input[Optional[str]]] = None,
                                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecCustomDenyResult]:
     """
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_custom_rule_actions.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_custom_rule_actions.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,19 +91,19 @@
     __args__['configId'] = config_id
     __args__['customRuleId'] = custom_rule_id
     __args__['securityPolicyId'] = security_policy_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecCustomRuleActions:getAppSecCustomRuleActions', __args__, opts=opts, typ=GetAppSecCustomRuleActionsResult).value
 
     return AwaitableGetAppSecCustomRuleActionsResult(
-        config_id=__ret__.config_id,
-        custom_rule_id=__ret__.custom_rule_id,
-        id=__ret__.id,
-        output_text=__ret__.output_text,
-        security_policy_id=__ret__.security_policy_id)
+        config_id=pulumi.get(__ret__, 'config_id'),
+        custom_rule_id=pulumi.get(__ret__, 'custom_rule_id'),
+        id=pulumi.get(__ret__, 'id'),
+        output_text=pulumi.get(__ret__, 'output_text'),
+        security_policy_id=pulumi.get(__ret__, 'security_policy_id'))
 
 
 @_utilities.lift_output_func(get_app_sec_custom_rule_actions)
 def get_app_sec_custom_rule_actions_output(config_id: Optional[pulumi.Input[int]] = None,
                                            custom_rule_id: Optional[pulumi.Input[Optional[int]]] = None,
                                            security_policy_id: Optional[pulumi.Input[str]] = None,
                                            opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecCustomRuleActionsResult]:
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_custom_rules.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_custom_rules.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,19 +89,19 @@
     __args__ = dict()
     __args__['configId'] = config_id
     __args__['customRuleId'] = custom_rule_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecCustomRules:getAppSecCustomRules', __args__, opts=opts, typ=GetAppSecCustomRulesResult).value
 
     return AwaitableGetAppSecCustomRulesResult(
-        config_id=__ret__.config_id,
-        custom_rule_id=__ret__.custom_rule_id,
-        id=__ret__.id,
-        json=__ret__.json,
-        output_text=__ret__.output_text)
+        config_id=pulumi.get(__ret__, 'config_id'),
+        custom_rule_id=pulumi.get(__ret__, 'custom_rule_id'),
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        output_text=pulumi.get(__ret__, 'output_text'))
 
 
 @_utilities.lift_output_func(get_app_sec_custom_rules)
 def get_app_sec_custom_rules_output(config_id: Optional[pulumi.Input[int]] = None,
                                     custom_rule_id: Optional[pulumi.Input[Optional[int]]] = None,
                                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecCustomRulesResult]:
     """
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_eval.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_eval.py`

 * *Files 8% similar despite different names*

```diff
@@ -80,18 +80,18 @@
     __args__ = dict()
     __args__['configId'] = config_id
     __args__['securityPolicyId'] = security_policy_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecEval:getAppSecEval', __args__, opts=opts, typ=GetAppSecEvalResult).value
 
     return AwaitableGetAppSecEvalResult(
-        config_id=__ret__.config_id,
-        id=__ret__.id,
-        output_text=__ret__.output_text,
-        security_policy_id=__ret__.security_policy_id)
+        config_id=pulumi.get(__ret__, 'config_id'),
+        id=pulumi.get(__ret__, 'id'),
+        output_text=pulumi.get(__ret__, 'output_text'),
+        security_policy_id=pulumi.get(__ret__, 'security_policy_id'))
 
 
 @_utilities.lift_output_func(get_app_sec_eval)
 def get_app_sec_eval_output(config_id: Optional[pulumi.Input[int]] = None,
                             security_policy_id: Optional[pulumi.Input[str]] = None,
                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecEvalResult]:
     """
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_eval_groups.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_eval_groups.py`

 * *Files 12% similar despite different names*

```diff
@@ -118,22 +118,22 @@
     __args__['attackGroup'] = attack_group
     __args__['configId'] = config_id
     __args__['securityPolicyId'] = security_policy_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecEvalGroups:getAppSecEvalGroups', __args__, opts=opts, typ=GetAppSecEvalGroupsResult).value
 
     return AwaitableGetAppSecEvalGroupsResult(
-        attack_group=__ret__.attack_group,
-        attack_group_action=__ret__.attack_group_action,
-        condition_exception=__ret__.condition_exception,
-        config_id=__ret__.config_id,
-        id=__ret__.id,
-        json=__ret__.json,
-        output_text=__ret__.output_text,
-        security_policy_id=__ret__.security_policy_id)
+        attack_group=pulumi.get(__ret__, 'attack_group'),
+        attack_group_action=pulumi.get(__ret__, 'attack_group_action'),
+        condition_exception=pulumi.get(__ret__, 'condition_exception'),
+        config_id=pulumi.get(__ret__, 'config_id'),
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        output_text=pulumi.get(__ret__, 'output_text'),
+        security_policy_id=pulumi.get(__ret__, 'security_policy_id'))
 
 
 @_utilities.lift_output_func(get_app_sec_eval_groups)
 def get_app_sec_eval_groups_output(attack_group: Optional[pulumi.Input[Optional[str]]] = None,
                                    config_id: Optional[pulumi.Input[int]] = None,
                                    security_policy_id: Optional[pulumi.Input[str]] = None,
                                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecEvalGroupsResult]:
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_eval_penalty_box.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_eval_penalty_box.py`

 * *Files 7% similar despite different names*

```diff
@@ -98,20 +98,20 @@
     __args__ = dict()
     __args__['configId'] = config_id
     __args__['securityPolicyId'] = security_policy_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecEvalPenaltyBox:getAppSecEvalPenaltyBox', __args__, opts=opts, typ=GetAppSecEvalPenaltyBoxResult).value
 
     return AwaitableGetAppSecEvalPenaltyBoxResult(
-        action=__ret__.action,
-        config_id=__ret__.config_id,
-        enabled=__ret__.enabled,
-        id=__ret__.id,
-        output_text=__ret__.output_text,
-        security_policy_id=__ret__.security_policy_id)
+        action=pulumi.get(__ret__, 'action'),
+        config_id=pulumi.get(__ret__, 'config_id'),
+        enabled=pulumi.get(__ret__, 'enabled'),
+        id=pulumi.get(__ret__, 'id'),
+        output_text=pulumi.get(__ret__, 'output_text'),
+        security_policy_id=pulumi.get(__ret__, 'security_policy_id'))
 
 
 @_utilities.lift_output_func(get_app_sec_eval_penalty_box)
 def get_app_sec_eval_penalty_box_output(config_id: Optional[pulumi.Input[int]] = None,
                                         security_policy_id: Optional[pulumi.Input[str]] = None,
                                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecEvalPenaltyBoxResult]:
     """
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_eval_rules.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_rules.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,44 +6,44 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
-    'GetAppSecEvalRulesResult',
-    'AwaitableGetAppSecEvalRulesResult',
-    'get_app_sec_eval_rules',
-    'get_app_sec_eval_rules_output',
+    'GetAppSecRulesResult',
+    'AwaitableGetAppSecRulesResult',
+    'get_app_sec_rules',
+    'get_app_sec_rules_output',
 ]
 
 @pulumi.output_type
-class GetAppSecEvalRulesResult:
+class GetAppSecRulesResult:
     """
-    A collection of values returned by getAppSecEvalRules.
+    A collection of values returned by getAppSecRules.
     """
-    def __init__(__self__, condition_exception=None, config_id=None, eval_rule_action=None, id=None, json=None, output_text=None, rule_id=None, security_policy_id=None):
+    def __init__(__self__, condition_exception=None, config_id=None, id=None, json=None, output_text=None, rule_action=None, rule_id=None, security_policy_id=None):
         if condition_exception and not isinstance(condition_exception, str):
             raise TypeError("Expected argument 'condition_exception' to be a str")
         pulumi.set(__self__, "condition_exception", condition_exception)
         if config_id and not isinstance(config_id, int):
             raise TypeError("Expected argument 'config_id' to be a int")
         pulumi.set(__self__, "config_id", config_id)
-        if eval_rule_action and not isinstance(eval_rule_action, str):
-            raise TypeError("Expected argument 'eval_rule_action' to be a str")
-        pulumi.set(__self__, "eval_rule_action", eval_rule_action)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
         if json and not isinstance(json, str):
             raise TypeError("Expected argument 'json' to be a str")
         pulumi.set(__self__, "json", json)
         if output_text and not isinstance(output_text, str):
             raise TypeError("Expected argument 'output_text' to be a str")
         pulumi.set(__self__, "output_text", output_text)
+        if rule_action and not isinstance(rule_action, str):
+            raise TypeError("Expected argument 'rule_action' to be a str")
+        pulumi.set(__self__, "rule_action", rule_action)
         if rule_id and not isinstance(rule_id, int):
             raise TypeError("Expected argument 'rule_id' to be a int")
         pulumi.set(__self__, "rule_id", rule_id)
         if security_policy_id and not isinstance(security_policy_id, str):
             raise TypeError("Expected argument 'security_policy_id' to be a str")
         pulumi.set(__self__, "security_policy_id", security_policy_id)
 
@@ -54,19 +54,14 @@
 
     @property
     @pulumi.getter(name="configId")
     def config_id(self) -> int:
         return pulumi.get(self, "config_id")
 
     @property
-    @pulumi.getter(name="evalRuleAction")
-    def eval_rule_action(self) -> str:
-        return pulumi.get(self, "eval_rule_action")
-
-    @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
@@ -77,67 +72,72 @@
 
     @property
     @pulumi.getter(name="outputText")
     def output_text(self) -> str:
         return pulumi.get(self, "output_text")
 
     @property
+    @pulumi.getter(name="ruleAction")
+    def rule_action(self) -> str:
+        return pulumi.get(self, "rule_action")
+
+    @property
     @pulumi.getter(name="ruleId")
     def rule_id(self) -> Optional[int]:
         return pulumi.get(self, "rule_id")
 
     @property
     @pulumi.getter(name="securityPolicyId")
     def security_policy_id(self) -> str:
         return pulumi.get(self, "security_policy_id")
 
 
-class AwaitableGetAppSecEvalRulesResult(GetAppSecEvalRulesResult):
+class AwaitableGetAppSecRulesResult(GetAppSecRulesResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetAppSecEvalRulesResult(
+        return GetAppSecRulesResult(
             condition_exception=self.condition_exception,
             config_id=self.config_id,
-            eval_rule_action=self.eval_rule_action,
             id=self.id,
             json=self.json,
             output_text=self.output_text,
+            rule_action=self.rule_action,
             rule_id=self.rule_id,
             security_policy_id=self.security_policy_id)
 
 
-def get_app_sec_eval_rules(config_id: Optional[int] = None,
-                           rule_id: Optional[int] = None,
-                           security_policy_id: Optional[str] = None,
-                           opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetAppSecEvalRulesResult:
+def get_app_sec_rules(config_id: Optional[int] = None,
+                      rule_id: Optional[int] = None,
+                      security_policy_id: Optional[str] = None,
+                      opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetAppSecRulesResult:
     """
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
     __args__['configId'] = config_id
     __args__['ruleId'] = rule_id
     __args__['securityPolicyId'] = security_policy_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecEvalRules:getAppSecEvalRules', __args__, opts=opts, typ=GetAppSecEvalRulesResult).value
+    __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecRules:getAppSecRules', __args__, opts=opts, typ=GetAppSecRulesResult).value
 
-    return AwaitableGetAppSecEvalRulesResult(
-        condition_exception=__ret__.condition_exception,
-        config_id=__ret__.config_id,
-        eval_rule_action=__ret__.eval_rule_action,
-        id=__ret__.id,
-        json=__ret__.json,
-        output_text=__ret__.output_text,
-        rule_id=__ret__.rule_id,
-        security_policy_id=__ret__.security_policy_id)
-
-
-@_utilities.lift_output_func(get_app_sec_eval_rules)
-def get_app_sec_eval_rules_output(config_id: Optional[pulumi.Input[int]] = None,
-                                  rule_id: Optional[pulumi.Input[Optional[int]]] = None,
-                                  security_policy_id: Optional[pulumi.Input[str]] = None,
-                                  opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecEvalRulesResult]:
+    return AwaitableGetAppSecRulesResult(
+        condition_exception=pulumi.get(__ret__, 'condition_exception'),
+        config_id=pulumi.get(__ret__, 'config_id'),
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        output_text=pulumi.get(__ret__, 'output_text'),
+        rule_action=pulumi.get(__ret__, 'rule_action'),
+        rule_id=pulumi.get(__ret__, 'rule_id'),
+        security_policy_id=pulumi.get(__ret__, 'security_policy_id'))
+
+
+@_utilities.lift_output_func(get_app_sec_rules)
+def get_app_sec_rules_output(config_id: Optional[pulumi.Input[int]] = None,
+                             rule_id: Optional[pulumi.Input[Optional[int]]] = None,
+                             security_policy_id: Optional[pulumi.Input[str]] = None,
+                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecRulesResult]:
     """
     Use this data source to access information about an existing resource.
     """
     ...
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_export_configuration.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_export_configuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,20 +100,20 @@
     __args__['configId'] = config_id
     __args__['searches'] = searches
     __args__['version'] = version
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecExportConfiguration:getAppSecExportConfiguration', __args__, opts=opts, typ=GetAppSecExportConfigurationResult).value
 
     return AwaitableGetAppSecExportConfigurationResult(
-        config_id=__ret__.config_id,
-        id=__ret__.id,
-        json=__ret__.json,
-        output_text=__ret__.output_text,
-        searches=__ret__.searches,
-        version=__ret__.version)
+        config_id=pulumi.get(__ret__, 'config_id'),
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        output_text=pulumi.get(__ret__, 'output_text'),
+        searches=pulumi.get(__ret__, 'searches'),
+        version=pulumi.get(__ret__, 'version'))
 
 
 @_utilities.lift_output_func(get_app_sec_export_configuration)
 def get_app_sec_export_configuration_output(config_id: Optional[pulumi.Input[int]] = None,
                                             searches: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                                             version: Optional[pulumi.Input[int]] = None,
                                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecExportConfigurationResult]:
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_failover_hostnames.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_failover_hostnames.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,19 +87,19 @@
     """
     __args__ = dict()
     __args__['configId'] = config_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecFailoverHostnames:getAppSecFailoverHostnames', __args__, opts=opts, typ=GetAppSecFailoverHostnamesResult).value
 
     return AwaitableGetAppSecFailoverHostnamesResult(
-        config_id=__ret__.config_id,
-        hostnames=__ret__.hostnames,
-        id=__ret__.id,
-        json=__ret__.json,
-        output_text=__ret__.output_text)
+        config_id=pulumi.get(__ret__, 'config_id'),
+        hostnames=pulumi.get(__ret__, 'hostnames'),
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        output_text=pulumi.get(__ret__, 'output_text'))
 
 
 @_utilities.lift_output_func(get_app_sec_failover_hostnames)
 def get_app_sec_failover_hostnames_output(config_id: Optional[pulumi.Input[int]] = None,
                                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecFailoverHostnamesResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_hostname_coverage.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_hostname_coverage.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,10 +66,10 @@
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecHostnameCoverage:getAppSecHostnameCoverage', __args__, opts=opts, typ=GetAppSecHostnameCoverageResult).value
 
     return AwaitableGetAppSecHostnameCoverageResult(
-        id=__ret__.id,
-        json=__ret__.json,
-        output_text=__ret__.output_text)
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        output_text=pulumi.get(__ret__, 'output_text'))
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_hostname_coverage_match_targets.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_hostname_coverage_match_targets.py`

 * *Files 7% similar despite different names*

```diff
@@ -89,19 +89,19 @@
     __args__ = dict()
     __args__['configId'] = config_id
     __args__['hostname'] = hostname
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecHostnameCoverageMatchTargets:getAppSecHostnameCoverageMatchTargets', __args__, opts=opts, typ=GetAppSecHostnameCoverageMatchTargetsResult).value
 
     return AwaitableGetAppSecHostnameCoverageMatchTargetsResult(
-        config_id=__ret__.config_id,
-        hostname=__ret__.hostname,
-        id=__ret__.id,
-        json=__ret__.json,
-        output_text=__ret__.output_text)
+        config_id=pulumi.get(__ret__, 'config_id'),
+        hostname=pulumi.get(__ret__, 'hostname'),
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        output_text=pulumi.get(__ret__, 'output_text'))
 
 
 @_utilities.lift_output_func(get_app_sec_hostname_coverage_match_targets)
 def get_app_sec_hostname_coverage_match_targets_output(config_id: Optional[pulumi.Input[int]] = None,
                                                        hostname: Optional[pulumi.Input[str]] = None,
                                                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecHostnameCoverageMatchTargetsResult]:
     """
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_hostname_coverage_overlapping.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_hostname_coverage_overlapping.py`

 * *Files 12% similar despite different names*

```diff
@@ -89,19 +89,19 @@
     __args__ = dict()
     __args__['configId'] = config_id
     __args__['hostname'] = hostname
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecHostnameCoverageOverlapping:getAppSecHostnameCoverageOverlapping', __args__, opts=opts, typ=GetAppSecHostnameCoverageOverlappingResult).value
 
     return AwaitableGetAppSecHostnameCoverageOverlappingResult(
-        config_id=__ret__.config_id,
-        hostname=__ret__.hostname,
-        id=__ret__.id,
-        json=__ret__.json,
-        output_text=__ret__.output_text)
+        config_id=pulumi.get(__ret__, 'config_id'),
+        hostname=pulumi.get(__ret__, 'hostname'),
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        output_text=pulumi.get(__ret__, 'output_text'))
 
 
 @_utilities.lift_output_func(get_app_sec_hostname_coverage_overlapping)
 def get_app_sec_hostname_coverage_overlapping_output(config_id: Optional[pulumi.Input[int]] = None,
                                                      hostname: Optional[pulumi.Input[str]] = None,
                                                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecHostnameCoverageOverlappingResult]:
     """
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_ip_geo.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_ip_geo.py`

 * *Files 8% similar despite different names*

```diff
@@ -116,22 +116,22 @@
     __args__ = dict()
     __args__['configId'] = config_id
     __args__['securityPolicyId'] = security_policy_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecIPGeo:getAppSecIPGeo', __args__, opts=opts, typ=GetAppSecIPGeoResult).value
 
     return AwaitableGetAppSecIPGeoResult(
-        config_id=__ret__.config_id,
-        exception_ip_network_lists=__ret__.exception_ip_network_lists,
-        geo_network_lists=__ret__.geo_network_lists,
-        id=__ret__.id,
-        ip_network_lists=__ret__.ip_network_lists,
-        mode=__ret__.mode,
-        output_text=__ret__.output_text,
-        security_policy_id=__ret__.security_policy_id)
+        config_id=pulumi.get(__ret__, 'config_id'),
+        exception_ip_network_lists=pulumi.get(__ret__, 'exception_ip_network_lists'),
+        geo_network_lists=pulumi.get(__ret__, 'geo_network_lists'),
+        id=pulumi.get(__ret__, 'id'),
+        ip_network_lists=pulumi.get(__ret__, 'ip_network_lists'),
+        mode=pulumi.get(__ret__, 'mode'),
+        output_text=pulumi.get(__ret__, 'output_text'),
+        security_policy_id=pulumi.get(__ret__, 'security_policy_id'))
 
 
 @_utilities.lift_output_func(get_app_sec_ip_geo)
 def get_app_sec_ip_geo_output(config_id: Optional[pulumi.Input[int]] = None,
                               security_policy_id: Optional[pulumi.Input[str]] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecIPGeoResult]:
     """
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_malware_content_types.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_malware_content_types.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,18 +78,18 @@
     """
     __args__ = dict()
     __args__['configId'] = config_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecMalwareContentTypes:getAppSecMalwareContentTypes', __args__, opts=opts, typ=GetAppSecMalwareContentTypesResult).value
 
     return AwaitableGetAppSecMalwareContentTypesResult(
-        config_id=__ret__.config_id,
-        id=__ret__.id,
-        json=__ret__.json,
-        output_text=__ret__.output_text)
+        config_id=pulumi.get(__ret__, 'config_id'),
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        output_text=pulumi.get(__ret__, 'output_text'))
 
 
 @_utilities.lift_output_func(get_app_sec_malware_content_types)
 def get_app_sec_malware_content_types_output(config_id: Optional[pulumi.Input[int]] = None,
                                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecMalwareContentTypesResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_malware_policies.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_malware_policies.py`

 * *Files 6% similar despite different names*

```diff
@@ -89,19 +89,19 @@
     __args__ = dict()
     __args__['configId'] = config_id
     __args__['malwarePolicyId'] = malware_policy_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecMalwarePolicies:getAppSecMalwarePolicies', __args__, opts=opts, typ=GetAppSecMalwarePoliciesResult).value
 
     return AwaitableGetAppSecMalwarePoliciesResult(
-        config_id=__ret__.config_id,
-        id=__ret__.id,
-        json=__ret__.json,
-        malware_policy_id=__ret__.malware_policy_id,
-        output_text=__ret__.output_text)
+        config_id=pulumi.get(__ret__, 'config_id'),
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        malware_policy_id=pulumi.get(__ret__, 'malware_policy_id'),
+        output_text=pulumi.get(__ret__, 'output_text'))
 
 
 @_utilities.lift_output_func(get_app_sec_malware_policies)
 def get_app_sec_malware_policies_output(config_id: Optional[pulumi.Input[int]] = None,
                                         malware_policy_id: Optional[pulumi.Input[Optional[int]]] = None,
                                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecMalwarePoliciesResult]:
     """
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_malware_policy_actions.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_malware_policy_actions.py`

 * *Files 7% similar despite different names*

```diff
@@ -91,19 +91,19 @@
     __args__['configId'] = config_id
     __args__['malwarePolicyId'] = malware_policy_id
     __args__['securityPolicyId'] = security_policy_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecMalwarePolicyActions:getAppSecMalwarePolicyActions', __args__, opts=opts, typ=GetAppSecMalwarePolicyActionsResult).value
 
     return AwaitableGetAppSecMalwarePolicyActionsResult(
-        config_id=__ret__.config_id,
-        id=__ret__.id,
-        malware_policy_id=__ret__.malware_policy_id,
-        output_text=__ret__.output_text,
-        security_policy_id=__ret__.security_policy_id)
+        config_id=pulumi.get(__ret__, 'config_id'),
+        id=pulumi.get(__ret__, 'id'),
+        malware_policy_id=pulumi.get(__ret__, 'malware_policy_id'),
+        output_text=pulumi.get(__ret__, 'output_text'),
+        security_policy_id=pulumi.get(__ret__, 'security_policy_id'))
 
 
 @_utilities.lift_output_func(get_app_sec_malware_policy_actions)
 def get_app_sec_malware_policy_actions_output(config_id: Optional[pulumi.Input[int]] = None,
                                               malware_policy_id: Optional[pulumi.Input[Optional[int]]] = None,
                                               security_policy_id: Optional[pulumi.Input[str]] = None,
                                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecMalwarePolicyActionsResult]:
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_match_targets.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_match_targets.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,19 +89,19 @@
     __args__ = dict()
     __args__['configId'] = config_id
     __args__['matchTargetId'] = match_target_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecMatchTargets:getAppSecMatchTargets', __args__, opts=opts, typ=GetAppSecMatchTargetsResult).value
 
     return AwaitableGetAppSecMatchTargetsResult(
-        config_id=__ret__.config_id,
-        id=__ret__.id,
-        json=__ret__.json,
-        match_target_id=__ret__.match_target_id,
-        output_text=__ret__.output_text)
+        config_id=pulumi.get(__ret__, 'config_id'),
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        match_target_id=pulumi.get(__ret__, 'match_target_id'),
+        output_text=pulumi.get(__ret__, 'output_text'))
 
 
 @_utilities.lift_output_func(get_app_sec_match_targets)
 def get_app_sec_match_targets_output(config_id: Optional[pulumi.Input[int]] = None,
                                      match_target_id: Optional[pulumi.Input[Optional[int]]] = None,
                                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecMatchTargetsResult]:
     """
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_penalty_box.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_penalty_box.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,20 +98,20 @@
     __args__ = dict()
     __args__['configId'] = config_id
     __args__['securityPolicyId'] = security_policy_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecPenaltyBox:getAppSecPenaltyBox', __args__, opts=opts, typ=GetAppSecPenaltyBoxResult).value
 
     return AwaitableGetAppSecPenaltyBoxResult(
-        action=__ret__.action,
-        config_id=__ret__.config_id,
-        enabled=__ret__.enabled,
-        id=__ret__.id,
-        output_text=__ret__.output_text,
-        security_policy_id=__ret__.security_policy_id)
+        action=pulumi.get(__ret__, 'action'),
+        config_id=pulumi.get(__ret__, 'config_id'),
+        enabled=pulumi.get(__ret__, 'enabled'),
+        id=pulumi.get(__ret__, 'id'),
+        output_text=pulumi.get(__ret__, 'output_text'),
+        security_policy_id=pulumi.get(__ret__, 'security_policy_id'))
 
 
 @_utilities.lift_output_func(get_app_sec_penalty_box)
 def get_app_sec_penalty_box_output(config_id: Optional[pulumi.Input[int]] = None,
                                    security_policy_id: Optional[pulumi.Input[str]] = None,
                                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecPenaltyBoxResult]:
     """
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_rate_policies.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_rate_policies.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,19 +89,19 @@
     __args__ = dict()
     __args__['configId'] = config_id
     __args__['ratePolicyId'] = rate_policy_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecRatePolicies:getAppSecRatePolicies', __args__, opts=opts, typ=GetAppSecRatePoliciesResult).value
 
     return AwaitableGetAppSecRatePoliciesResult(
-        config_id=__ret__.config_id,
-        id=__ret__.id,
-        json=__ret__.json,
-        output_text=__ret__.output_text,
-        rate_policy_id=__ret__.rate_policy_id)
+        config_id=pulumi.get(__ret__, 'config_id'),
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        output_text=pulumi.get(__ret__, 'output_text'),
+        rate_policy_id=pulumi.get(__ret__, 'rate_policy_id'))
 
 
 @_utilities.lift_output_func(get_app_sec_rate_policies)
 def get_app_sec_rate_policies_output(config_id: Optional[pulumi.Input[int]] = None,
                                      rate_policy_id: Optional[pulumi.Input[Optional[int]]] = None,
                                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecRatePoliciesResult]:
     """
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_rate_policy_actions.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_rate_policy_actions.py`

 * *Files 5% similar despite different names*

```diff
@@ -91,19 +91,19 @@
     __args__['configId'] = config_id
     __args__['ratePolicyId'] = rate_policy_id
     __args__['securityPolicyId'] = security_policy_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecRatePolicyActions:getAppSecRatePolicyActions', __args__, opts=opts, typ=GetAppSecRatePolicyActionsResult).value
 
     return AwaitableGetAppSecRatePolicyActionsResult(
-        config_id=__ret__.config_id,
-        id=__ret__.id,
-        output_text=__ret__.output_text,
-        rate_policy_id=__ret__.rate_policy_id,
-        security_policy_id=__ret__.security_policy_id)
+        config_id=pulumi.get(__ret__, 'config_id'),
+        id=pulumi.get(__ret__, 'id'),
+        output_text=pulumi.get(__ret__, 'output_text'),
+        rate_policy_id=pulumi.get(__ret__, 'rate_policy_id'),
+        security_policy_id=pulumi.get(__ret__, 'security_policy_id'))
 
 
 @_utilities.lift_output_func(get_app_sec_rate_policy_actions)
 def get_app_sec_rate_policy_actions_output(config_id: Optional[pulumi.Input[int]] = None,
                                            rate_policy_id: Optional[pulumi.Input[Optional[int]]] = None,
                                            security_policy_id: Optional[pulumi.Input[str]] = None,
                                            opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecRatePolicyActionsResult]:
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_reputation_profile_actions.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_reputation_profile_actions.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,21 +109,21 @@
     __args__['configId'] = config_id
     __args__['reputationProfileId'] = reputation_profile_id
     __args__['securityPolicyId'] = security_policy_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecReputationProfileActions:getAppSecReputationProfileActions', __args__, opts=opts, typ=GetAppSecReputationProfileActionsResult).value
 
     return AwaitableGetAppSecReputationProfileActionsResult(
-        action=__ret__.action,
-        config_id=__ret__.config_id,
-        id=__ret__.id,
-        json=__ret__.json,
-        output_text=__ret__.output_text,
-        reputation_profile_id=__ret__.reputation_profile_id,
-        security_policy_id=__ret__.security_policy_id)
+        action=pulumi.get(__ret__, 'action'),
+        config_id=pulumi.get(__ret__, 'config_id'),
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        output_text=pulumi.get(__ret__, 'output_text'),
+        reputation_profile_id=pulumi.get(__ret__, 'reputation_profile_id'),
+        security_policy_id=pulumi.get(__ret__, 'security_policy_id'))
 
 
 @_utilities.lift_output_func(get_app_sec_reputation_profile_actions)
 def get_app_sec_reputation_profile_actions_output(config_id: Optional[pulumi.Input[int]] = None,
                                                   reputation_profile_id: Optional[pulumi.Input[Optional[int]]] = None,
                                                   security_policy_id: Optional[pulumi.Input[str]] = None,
                                                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecReputationProfileActionsResult]:
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_reputation_profile_analysis.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_reputation_profile_analysis.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,19 +89,19 @@
     __args__ = dict()
     __args__['configId'] = config_id
     __args__['securityPolicyId'] = security_policy_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecReputationProfileAnalysis:getAppSecReputationProfileAnalysis', __args__, opts=opts, typ=GetAppSecReputationProfileAnalysisResult).value
 
     return AwaitableGetAppSecReputationProfileAnalysisResult(
-        config_id=__ret__.config_id,
-        id=__ret__.id,
-        json=__ret__.json,
-        output_text=__ret__.output_text,
-        security_policy_id=__ret__.security_policy_id)
+        config_id=pulumi.get(__ret__, 'config_id'),
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        output_text=pulumi.get(__ret__, 'output_text'),
+        security_policy_id=pulumi.get(__ret__, 'security_policy_id'))
 
 
 @_utilities.lift_output_func(get_app_sec_reputation_profile_analysis)
 def get_app_sec_reputation_profile_analysis_output(config_id: Optional[pulumi.Input[int]] = None,
                                                    security_policy_id: Optional[pulumi.Input[str]] = None,
                                                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecReputationProfileAnalysisResult]:
     """
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_reputation_profiles.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_reputation_profiles.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,19 +89,19 @@
     __args__ = dict()
     __args__['configId'] = config_id
     __args__['reputationProfileId'] = reputation_profile_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecReputationProfiles:getAppSecReputationProfiles', __args__, opts=opts, typ=GetAppSecReputationProfilesResult).value
 
     return AwaitableGetAppSecReputationProfilesResult(
-        config_id=__ret__.config_id,
-        id=__ret__.id,
-        json=__ret__.json,
-        output_text=__ret__.output_text,
-        reputation_profile_id=__ret__.reputation_profile_id)
+        config_id=pulumi.get(__ret__, 'config_id'),
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        output_text=pulumi.get(__ret__, 'output_text'),
+        reputation_profile_id=pulumi.get(__ret__, 'reputation_profile_id'))
 
 
 @_utilities.lift_output_func(get_app_sec_reputation_profiles)
 def get_app_sec_reputation_profiles_output(config_id: Optional[pulumi.Input[int]] = None,
                                            reputation_profile_id: Optional[pulumi.Input[Optional[int]]] = None,
                                            opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecReputationProfilesResult]:
     """
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_rule_upgrade_details.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_rule_upgrade_details.py`

 * *Files 6% similar despite different names*

```diff
@@ -89,19 +89,19 @@
     __args__ = dict()
     __args__['configId'] = config_id
     __args__['securityPolicyId'] = security_policy_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecRuleUpgradeDetails:getAppSecRuleUpgradeDetails', __args__, opts=opts, typ=GetAppSecRuleUpgradeDetailsResult).value
 
     return AwaitableGetAppSecRuleUpgradeDetailsResult(
-        config_id=__ret__.config_id,
-        id=__ret__.id,
-        json=__ret__.json,
-        output_text=__ret__.output_text,
-        security_policy_id=__ret__.security_policy_id)
+        config_id=pulumi.get(__ret__, 'config_id'),
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        output_text=pulumi.get(__ret__, 'output_text'),
+        security_policy_id=pulumi.get(__ret__, 'security_policy_id'))
 
 
 @_utilities.lift_output_func(get_app_sec_rule_upgrade_details)
 def get_app_sec_rule_upgrade_details_output(config_id: Optional[pulumi.Input[int]] = None,
                                             security_policy_id: Optional[pulumi.Input[str]] = None,
                                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecRuleUpgradeDetailsResult]:
     """
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_rules.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_tuning_recommendations.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,55 +6,52 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
-    'GetAppSecRulesResult',
-    'AwaitableGetAppSecRulesResult',
-    'get_app_sec_rules',
-    'get_app_sec_rules_output',
+    'GetAppSecTuningRecommendationsResult',
+    'AwaitableGetAppSecTuningRecommendationsResult',
+    'get_app_sec_tuning_recommendations',
+    'get_app_sec_tuning_recommendations_output',
 ]
 
 @pulumi.output_type
-class GetAppSecRulesResult:
+class GetAppSecTuningRecommendationsResult:
     """
-    A collection of values returned by getAppSecRules.
+    A collection of values returned by getAppSecTuningRecommendations.
     """
-    def __init__(__self__, condition_exception=None, config_id=None, id=None, json=None, output_text=None, rule_action=None, rule_id=None, security_policy_id=None):
-        if condition_exception and not isinstance(condition_exception, str):
-            raise TypeError("Expected argument 'condition_exception' to be a str")
-        pulumi.set(__self__, "condition_exception", condition_exception)
+    def __init__(__self__, attack_group=None, config_id=None, id=None, json=None, rule_id=None, ruleset_type=None, security_policy_id=None):
+        if attack_group and not isinstance(attack_group, str):
+            raise TypeError("Expected argument 'attack_group' to be a str")
+        pulumi.set(__self__, "attack_group", attack_group)
         if config_id and not isinstance(config_id, int):
             raise TypeError("Expected argument 'config_id' to be a int")
         pulumi.set(__self__, "config_id", config_id)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
         if json and not isinstance(json, str):
             raise TypeError("Expected argument 'json' to be a str")
         pulumi.set(__self__, "json", json)
-        if output_text and not isinstance(output_text, str):
-            raise TypeError("Expected argument 'output_text' to be a str")
-        pulumi.set(__self__, "output_text", output_text)
-        if rule_action and not isinstance(rule_action, str):
-            raise TypeError("Expected argument 'rule_action' to be a str")
-        pulumi.set(__self__, "rule_action", rule_action)
         if rule_id and not isinstance(rule_id, int):
             raise TypeError("Expected argument 'rule_id' to be a int")
         pulumi.set(__self__, "rule_id", rule_id)
+        if ruleset_type and not isinstance(ruleset_type, str):
+            raise TypeError("Expected argument 'ruleset_type' to be a str")
+        pulumi.set(__self__, "ruleset_type", ruleset_type)
         if security_policy_id and not isinstance(security_policy_id, str):
             raise TypeError("Expected argument 'security_policy_id' to be a str")
         pulumi.set(__self__, "security_policy_id", security_policy_id)
 
     @property
-    @pulumi.getter(name="conditionException")
-    def condition_exception(self) -> str:
-        return pulumi.get(self, "condition_exception")
+    @pulumi.getter(name="attackGroup")
+    def attack_group(self) -> Optional[str]:
+        return pulumi.get(self, "attack_group")
 
     @property
     @pulumi.getter(name="configId")
     def config_id(self) -> int:
         return pulumi.get(self, "config_id")
 
     @property
@@ -67,77 +64,76 @@
 
     @property
     @pulumi.getter
     def json(self) -> str:
         return pulumi.get(self, "json")
 
     @property
-    @pulumi.getter(name="outputText")
-    def output_text(self) -> str:
-        return pulumi.get(self, "output_text")
-
-    @property
-    @pulumi.getter(name="ruleAction")
-    def rule_action(self) -> str:
-        return pulumi.get(self, "rule_action")
-
-    @property
     @pulumi.getter(name="ruleId")
     def rule_id(self) -> Optional[int]:
         return pulumi.get(self, "rule_id")
 
     @property
+    @pulumi.getter(name="rulesetType")
+    def ruleset_type(self) -> Optional[str]:
+        return pulumi.get(self, "ruleset_type")
+
+    @property
     @pulumi.getter(name="securityPolicyId")
-    def security_policy_id(self) -> str:
+    def security_policy_id(self) -> Optional[str]:
         return pulumi.get(self, "security_policy_id")
 
 
-class AwaitableGetAppSecRulesResult(GetAppSecRulesResult):
+class AwaitableGetAppSecTuningRecommendationsResult(GetAppSecTuningRecommendationsResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetAppSecRulesResult(
-            condition_exception=self.condition_exception,
+        return GetAppSecTuningRecommendationsResult(
+            attack_group=self.attack_group,
             config_id=self.config_id,
             id=self.id,
             json=self.json,
-            output_text=self.output_text,
-            rule_action=self.rule_action,
             rule_id=self.rule_id,
+            ruleset_type=self.ruleset_type,
             security_policy_id=self.security_policy_id)
 
 
-def get_app_sec_rules(config_id: Optional[int] = None,
-                      rule_id: Optional[int] = None,
-                      security_policy_id: Optional[str] = None,
-                      opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetAppSecRulesResult:
+def get_app_sec_tuning_recommendations(attack_group: Optional[str] = None,
+                                       config_id: Optional[int] = None,
+                                       rule_id: Optional[int] = None,
+                                       ruleset_type: Optional[str] = None,
+                                       security_policy_id: Optional[str] = None,
+                                       opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetAppSecTuningRecommendationsResult:
     """
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
+    __args__['attackGroup'] = attack_group
     __args__['configId'] = config_id
     __args__['ruleId'] = rule_id
+    __args__['rulesetType'] = ruleset_type
     __args__['securityPolicyId'] = security_policy_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecRules:getAppSecRules', __args__, opts=opts, typ=GetAppSecRulesResult).value
+    __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecTuningRecommendations:getAppSecTuningRecommendations', __args__, opts=opts, typ=GetAppSecTuningRecommendationsResult).value
 
-    return AwaitableGetAppSecRulesResult(
-        condition_exception=__ret__.condition_exception,
-        config_id=__ret__.config_id,
-        id=__ret__.id,
-        json=__ret__.json,
-        output_text=__ret__.output_text,
-        rule_action=__ret__.rule_action,
-        rule_id=__ret__.rule_id,
-        security_policy_id=__ret__.security_policy_id)
-
-
-@_utilities.lift_output_func(get_app_sec_rules)
-def get_app_sec_rules_output(config_id: Optional[pulumi.Input[int]] = None,
-                             rule_id: Optional[pulumi.Input[Optional[int]]] = None,
-                             security_policy_id: Optional[pulumi.Input[str]] = None,
-                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecRulesResult]:
+    return AwaitableGetAppSecTuningRecommendationsResult(
+        attack_group=pulumi.get(__ret__, 'attack_group'),
+        config_id=pulumi.get(__ret__, 'config_id'),
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        rule_id=pulumi.get(__ret__, 'rule_id'),
+        ruleset_type=pulumi.get(__ret__, 'ruleset_type'),
+        security_policy_id=pulumi.get(__ret__, 'security_policy_id'))
+
+
+@_utilities.lift_output_func(get_app_sec_tuning_recommendations)
+def get_app_sec_tuning_recommendations_output(attack_group: Optional[pulumi.Input[Optional[str]]] = None,
+                                              config_id: Optional[pulumi.Input[int]] = None,
+                                              rule_id: Optional[pulumi.Input[Optional[int]]] = None,
+                                              ruleset_type: Optional[pulumi.Input[Optional[str]]] = None,
+                                              security_policy_id: Optional[pulumi.Input[Optional[str]]] = None,
+                                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecTuningRecommendationsResult]:
     """
     Use this data source to access information about an existing resource.
     """
     ...
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_security_policy.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_security_policy.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,21 +107,21 @@
     __args__ = dict()
     __args__['configId'] = config_id
     __args__['securityPolicyName'] = security_policy_name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecSecurityPolicy:getAppSecSecurityPolicy', __args__, opts=opts, typ=GetAppSecSecurityPolicyResult).value
 
     return AwaitableGetAppSecSecurityPolicyResult(
-        config_id=__ret__.config_id,
-        id=__ret__.id,
-        json=__ret__.json,
-        output_text=__ret__.output_text,
-        security_policy_id=__ret__.security_policy_id,
-        security_policy_id_lists=__ret__.security_policy_id_lists,
-        security_policy_name=__ret__.security_policy_name)
+        config_id=pulumi.get(__ret__, 'config_id'),
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        output_text=pulumi.get(__ret__, 'output_text'),
+        security_policy_id=pulumi.get(__ret__, 'security_policy_id'),
+        security_policy_id_lists=pulumi.get(__ret__, 'security_policy_id_lists'),
+        security_policy_name=pulumi.get(__ret__, 'security_policy_name'))
 
 
 @_utilities.lift_output_func(get_app_sec_security_policy)
 def get_app_sec_security_policy_output(config_id: Optional[pulumi.Input[int]] = None,
                                        security_policy_name: Optional[pulumi.Input[Optional[str]]] = None,
                                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecSecurityPolicyResult]:
     """
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_security_policy_protections.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_security_policy_protections.py`

 * *Files 4% similar despite different names*

```diff
@@ -161,27 +161,27 @@
     __args__ = dict()
     __args__['configId'] = config_id
     __args__['securityPolicyId'] = security_policy_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecSecurityPolicyProtections:getAppSecSecurityPolicyProtections', __args__, opts=opts, typ=GetAppSecSecurityPolicyProtectionsResult).value
 
     return AwaitableGetAppSecSecurityPolicyProtectionsResult(
-        apply_api_constraints=__ret__.apply_api_constraints,
-        apply_application_layer_controls=__ret__.apply_application_layer_controls,
-        apply_botman_controls=__ret__.apply_botman_controls,
-        apply_malware_controls=__ret__.apply_malware_controls,
-        apply_network_layer_controls=__ret__.apply_network_layer_controls,
-        apply_rate_controls=__ret__.apply_rate_controls,
-        apply_reputation_controls=__ret__.apply_reputation_controls,
-        apply_slow_post_controls=__ret__.apply_slow_post_controls,
-        config_id=__ret__.config_id,
-        id=__ret__.id,
-        json=__ret__.json,
-        output_text=__ret__.output_text,
-        security_policy_id=__ret__.security_policy_id)
+        apply_api_constraints=pulumi.get(__ret__, 'apply_api_constraints'),
+        apply_application_layer_controls=pulumi.get(__ret__, 'apply_application_layer_controls'),
+        apply_botman_controls=pulumi.get(__ret__, 'apply_botman_controls'),
+        apply_malware_controls=pulumi.get(__ret__, 'apply_malware_controls'),
+        apply_network_layer_controls=pulumi.get(__ret__, 'apply_network_layer_controls'),
+        apply_rate_controls=pulumi.get(__ret__, 'apply_rate_controls'),
+        apply_reputation_controls=pulumi.get(__ret__, 'apply_reputation_controls'),
+        apply_slow_post_controls=pulumi.get(__ret__, 'apply_slow_post_controls'),
+        config_id=pulumi.get(__ret__, 'config_id'),
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        output_text=pulumi.get(__ret__, 'output_text'),
+        security_policy_id=pulumi.get(__ret__, 'security_policy_id'))
 
 
 @_utilities.lift_output_func(get_app_sec_security_policy_protections)
 def get_app_sec_security_policy_protections_output(config_id: Optional[pulumi.Input[int]] = None,
                                                    security_policy_id: Optional[pulumi.Input[str]] = None,
                                                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecSecurityPolicyProtectionsResult]:
     """
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_selectable_hostnames.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_selectable_hostnames.py`

 * *Files 3% similar despite different names*

```diff
@@ -131,23 +131,23 @@
     __args__['configId'] = config_id
     __args__['contractid'] = contractid
     __args__['groupid'] = groupid
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecSelectableHostnames:getAppSecSelectableHostnames', __args__, opts=opts, typ=GetAppSecSelectableHostnamesResult).value
 
     return AwaitableGetAppSecSelectableHostnamesResult(
-        active_in_production=__ret__.active_in_production,
-        active_in_staging=__ret__.active_in_staging,
-        config_id=__ret__.config_id,
-        contractid=__ret__.contractid,
-        groupid=__ret__.groupid,
-        hostnames=__ret__.hostnames,
-        hostnames_json=__ret__.hostnames_json,
-        id=__ret__.id,
-        output_text=__ret__.output_text)
+        active_in_production=pulumi.get(__ret__, 'active_in_production'),
+        active_in_staging=pulumi.get(__ret__, 'active_in_staging'),
+        config_id=pulumi.get(__ret__, 'config_id'),
+        contractid=pulumi.get(__ret__, 'contractid'),
+        groupid=pulumi.get(__ret__, 'groupid'),
+        hostnames=pulumi.get(__ret__, 'hostnames'),
+        hostnames_json=pulumi.get(__ret__, 'hostnames_json'),
+        id=pulumi.get(__ret__, 'id'),
+        output_text=pulumi.get(__ret__, 'output_text'))
 
 
 @_utilities.lift_output_func(get_app_sec_selectable_hostnames)
 def get_app_sec_selectable_hostnames_output(active_in_production: Optional[pulumi.Input[Optional[bool]]] = None,
                                             active_in_staging: Optional[pulumi.Input[Optional[bool]]] = None,
                                             config_id: Optional[pulumi.Input[Optional[int]]] = None,
                                             contractid: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_selected_hostnames.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_selected_hostnames.py`

 * *Files 6% similar despite different names*

```diff
@@ -87,19 +87,19 @@
     """
     __args__ = dict()
     __args__['configId'] = config_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecSelectedHostnames:getAppSecSelectedHostnames', __args__, opts=opts, typ=GetAppSecSelectedHostnamesResult).value
 
     return AwaitableGetAppSecSelectedHostnamesResult(
-        config_id=__ret__.config_id,
-        hostnames=__ret__.hostnames,
-        hostnames_json=__ret__.hostnames_json,
-        id=__ret__.id,
-        output_text=__ret__.output_text)
+        config_id=pulumi.get(__ret__, 'config_id'),
+        hostnames=pulumi.get(__ret__, 'hostnames'),
+        hostnames_json=pulumi.get(__ret__, 'hostnames_json'),
+        id=pulumi.get(__ret__, 'id'),
+        output_text=pulumi.get(__ret__, 'output_text'))
 
 
 @_utilities.lift_output_func(get_app_sec_selected_hostnames)
 def get_app_sec_selected_hostnames_output(config_id: Optional[pulumi.Input[int]] = None,
                                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecSelectedHostnamesResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_siem_definitions.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_siem_definitions.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,18 +78,18 @@
     """
     __args__ = dict()
     __args__['siemDefinitionName'] = siem_definition_name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecSiemDefinitions:getAppSecSiemDefinitions', __args__, opts=opts, typ=GetAppSecSiemDefinitionsResult).value
 
     return AwaitableGetAppSecSiemDefinitionsResult(
-        id=__ret__.id,
-        json=__ret__.json,
-        output_text=__ret__.output_text,
-        siem_definition_name=__ret__.siem_definition_name)
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        output_text=pulumi.get(__ret__, 'output_text'),
+        siem_definition_name=pulumi.get(__ret__, 'siem_definition_name'))
 
 
 @_utilities.lift_output_func(get_app_sec_siem_definitions)
 def get_app_sec_siem_definitions_output(siem_definition_name: Optional[pulumi.Input[Optional[str]]] = None,
                                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecSiemDefinitionsResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_siem_settings.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_siem_settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -78,18 +78,18 @@
     """
     __args__ = dict()
     __args__['configId'] = config_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecSiemSettings:getAppSecSiemSettings', __args__, opts=opts, typ=GetAppSecSiemSettingsResult).value
 
     return AwaitableGetAppSecSiemSettingsResult(
-        config_id=__ret__.config_id,
-        id=__ret__.id,
-        json=__ret__.json,
-        output_text=__ret__.output_text)
+        config_id=pulumi.get(__ret__, 'config_id'),
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        output_text=pulumi.get(__ret__, 'output_text'))
 
 
 @_utilities.lift_output_func(get_app_sec_siem_settings)
 def get_app_sec_siem_settings_output(config_id: Optional[pulumi.Input[int]] = None,
                                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecSiemSettingsResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_slow_post.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_slow_post.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,19 +89,19 @@
     __args__ = dict()
     __args__['configId'] = config_id
     __args__['securityPolicyId'] = security_policy_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecSlowPost:getAppSecSlowPost', __args__, opts=opts, typ=GetAppSecSlowPostResult).value
 
     return AwaitableGetAppSecSlowPostResult(
-        config_id=__ret__.config_id,
-        id=__ret__.id,
-        json=__ret__.json,
-        output_text=__ret__.output_text,
-        security_policy_id=__ret__.security_policy_id)
+        config_id=pulumi.get(__ret__, 'config_id'),
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        output_text=pulumi.get(__ret__, 'output_text'),
+        security_policy_id=pulumi.get(__ret__, 'security_policy_id'))
 
 
 @_utilities.lift_output_func(get_app_sec_slow_post)
 def get_app_sec_slow_post_output(config_id: Optional[pulumi.Input[int]] = None,
                                  security_policy_id: Optional[pulumi.Input[str]] = None,
                                  opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecSlowPostResult]:
     """
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_threat_intel.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_threat_intel.py`

 * *Files 7% similar despite different names*

```diff
@@ -98,20 +98,20 @@
     __args__ = dict()
     __args__['configId'] = config_id
     __args__['securityPolicyId'] = security_policy_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecThreatIntel:getAppSecThreatIntel', __args__, opts=opts, typ=GetAppSecThreatIntelResult).value
 
     return AwaitableGetAppSecThreatIntelResult(
-        config_id=__ret__.config_id,
-        id=__ret__.id,
-        json=__ret__.json,
-        output_text=__ret__.output_text,
-        security_policy_id=__ret__.security_policy_id,
-        threat_intel=__ret__.threat_intel)
+        config_id=pulumi.get(__ret__, 'config_id'),
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        output_text=pulumi.get(__ret__, 'output_text'),
+        security_policy_id=pulumi.get(__ret__, 'security_policy_id'),
+        threat_intel=pulumi.get(__ret__, 'threat_intel'))
 
 
 @_utilities.lift_output_func(get_app_sec_threat_intel)
 def get_app_sec_threat_intel_output(config_id: Optional[pulumi.Input[int]] = None,
                                     security_policy_id: Optional[pulumi.Input[str]] = None,
                                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecThreatIntelResult]:
     """
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_tuning_recommendations.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_property_include.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,134 +6,148 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
-    'GetAppSecTuningRecommendationsResult',
-    'AwaitableGetAppSecTuningRecommendationsResult',
-    'get_app_sec_tuning_recommendations',
-    'get_app_sec_tuning_recommendations_output',
+    'GetPropertyIncludeResult',
+    'AwaitableGetPropertyIncludeResult',
+    'get_property_include',
+    'get_property_include_output',
 ]
 
 @pulumi.output_type
-class GetAppSecTuningRecommendationsResult:
+class GetPropertyIncludeResult:
     """
-    A collection of values returned by getAppSecTuningRecommendations.
+    A collection of values returned by getPropertyInclude.
     """
-    def __init__(__self__, attack_group=None, config_id=None, id=None, json=None, rule_id=None, ruleset_type=None, security_policy_id=None):
-        if attack_group and not isinstance(attack_group, str):
-            raise TypeError("Expected argument 'attack_group' to be a str")
-        pulumi.set(__self__, "attack_group", attack_group)
-        if config_id and not isinstance(config_id, int):
-            raise TypeError("Expected argument 'config_id' to be a int")
-        pulumi.set(__self__, "config_id", config_id)
+    def __init__(__self__, contract_id=None, group_id=None, id=None, include_id=None, latest_version=None, name=None, production_version=None, staging_version=None, type=None):
+        if contract_id and not isinstance(contract_id, str):
+            raise TypeError("Expected argument 'contract_id' to be a str")
+        pulumi.set(__self__, "contract_id", contract_id)
+        if group_id and not isinstance(group_id, str):
+            raise TypeError("Expected argument 'group_id' to be a str")
+        pulumi.set(__self__, "group_id", group_id)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
-        if json and not isinstance(json, str):
-            raise TypeError("Expected argument 'json' to be a str")
-        pulumi.set(__self__, "json", json)
-        if rule_id and not isinstance(rule_id, int):
-            raise TypeError("Expected argument 'rule_id' to be a int")
-        pulumi.set(__self__, "rule_id", rule_id)
-        if ruleset_type and not isinstance(ruleset_type, str):
-            raise TypeError("Expected argument 'ruleset_type' to be a str")
-        pulumi.set(__self__, "ruleset_type", ruleset_type)
-        if security_policy_id and not isinstance(security_policy_id, str):
-            raise TypeError("Expected argument 'security_policy_id' to be a str")
-        pulumi.set(__self__, "security_policy_id", security_policy_id)
-
-    @property
-    @pulumi.getter(name="attackGroup")
-    def attack_group(self) -> Optional[str]:
-        return pulumi.get(self, "attack_group")
-
-    @property
-    @pulumi.getter(name="configId")
-    def config_id(self) -> int:
-        return pulumi.get(self, "config_id")
+        if include_id and not isinstance(include_id, str):
+            raise TypeError("Expected argument 'include_id' to be a str")
+        pulumi.set(__self__, "include_id", include_id)
+        if latest_version and not isinstance(latest_version, int):
+            raise TypeError("Expected argument 'latest_version' to be a int")
+        pulumi.set(__self__, "latest_version", latest_version)
+        if name and not isinstance(name, str):
+            raise TypeError("Expected argument 'name' to be a str")
+        pulumi.set(__self__, "name", name)
+        if production_version and not isinstance(production_version, int):
+            raise TypeError("Expected argument 'production_version' to be a int")
+        pulumi.set(__self__, "production_version", production_version)
+        if staging_version and not isinstance(staging_version, int):
+            raise TypeError("Expected argument 'staging_version' to be a int")
+        pulumi.set(__self__, "staging_version", staging_version)
+        if type and not isinstance(type, str):
+            raise TypeError("Expected argument 'type' to be a str")
+        pulumi.set(__self__, "type", type)
+
+    @property
+    @pulumi.getter(name="contractId")
+    def contract_id(self) -> str:
+        return pulumi.get(self, "contract_id")
+
+    @property
+    @pulumi.getter(name="groupId")
+    def group_id(self) -> str:
+        return pulumi.get(self, "group_id")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
+    @pulumi.getter(name="includeId")
+    def include_id(self) -> str:
+        return pulumi.get(self, "include_id")
+
+    @property
+    @pulumi.getter(name="latestVersion")
+    def latest_version(self) -> int:
+        return pulumi.get(self, "latest_version")
+
+    @property
     @pulumi.getter
-    def json(self) -> str:
-        return pulumi.get(self, "json")
+    def name(self) -> str:
+        return pulumi.get(self, "name")
 
     @property
-    @pulumi.getter(name="ruleId")
-    def rule_id(self) -> Optional[int]:
-        return pulumi.get(self, "rule_id")
+    @pulumi.getter(name="productionVersion")
+    def production_version(self) -> int:
+        return pulumi.get(self, "production_version")
 
     @property
-    @pulumi.getter(name="rulesetType")
-    def ruleset_type(self) -> Optional[str]:
-        return pulumi.get(self, "ruleset_type")
+    @pulumi.getter(name="stagingVersion")
+    def staging_version(self) -> int:
+        return pulumi.get(self, "staging_version")
 
     @property
-    @pulumi.getter(name="securityPolicyId")
-    def security_policy_id(self) -> Optional[str]:
-        return pulumi.get(self, "security_policy_id")
+    @pulumi.getter
+    def type(self) -> str:
+        return pulumi.get(self, "type")
 
 
-class AwaitableGetAppSecTuningRecommendationsResult(GetAppSecTuningRecommendationsResult):
+class AwaitableGetPropertyIncludeResult(GetPropertyIncludeResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetAppSecTuningRecommendationsResult(
-            attack_group=self.attack_group,
-            config_id=self.config_id,
+        return GetPropertyIncludeResult(
+            contract_id=self.contract_id,
+            group_id=self.group_id,
             id=self.id,
-            json=self.json,
-            rule_id=self.rule_id,
-            ruleset_type=self.ruleset_type,
-            security_policy_id=self.security_policy_id)
+            include_id=self.include_id,
+            latest_version=self.latest_version,
+            name=self.name,
+            production_version=self.production_version,
+            staging_version=self.staging_version,
+            type=self.type)
 
 
-def get_app_sec_tuning_recommendations(attack_group: Optional[str] = None,
-                                       config_id: Optional[int] = None,
-                                       rule_id: Optional[int] = None,
-                                       ruleset_type: Optional[str] = None,
-                                       security_policy_id: Optional[str] = None,
-                                       opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetAppSecTuningRecommendationsResult:
+def get_property_include(contract_id: Optional[str] = None,
+                         group_id: Optional[str] = None,
+                         include_id: Optional[str] = None,
+                         opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPropertyIncludeResult:
     """
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
-    __args__['attackGroup'] = attack_group
-    __args__['configId'] = config_id
-    __args__['ruleId'] = rule_id
-    __args__['rulesetType'] = ruleset_type
-    __args__['securityPolicyId'] = security_policy_id
+    __args__['contractId'] = contract_id
+    __args__['groupId'] = group_id
+    __args__['includeId'] = include_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecTuningRecommendations:getAppSecTuningRecommendations', __args__, opts=opts, typ=GetAppSecTuningRecommendationsResult).value
+    __ret__ = pulumi.runtime.invoke('akamai:index/getPropertyInclude:getPropertyInclude', __args__, opts=opts, typ=GetPropertyIncludeResult).value
 
-    return AwaitableGetAppSecTuningRecommendationsResult(
-        attack_group=__ret__.attack_group,
-        config_id=__ret__.config_id,
-        id=__ret__.id,
-        json=__ret__.json,
-        rule_id=__ret__.rule_id,
-        ruleset_type=__ret__.ruleset_type,
-        security_policy_id=__ret__.security_policy_id)
-
-
-@_utilities.lift_output_func(get_app_sec_tuning_recommendations)
-def get_app_sec_tuning_recommendations_output(attack_group: Optional[pulumi.Input[Optional[str]]] = None,
-                                              config_id: Optional[pulumi.Input[int]] = None,
-                                              rule_id: Optional[pulumi.Input[Optional[int]]] = None,
-                                              ruleset_type: Optional[pulumi.Input[Optional[str]]] = None,
-                                              security_policy_id: Optional[pulumi.Input[Optional[str]]] = None,
-                                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecTuningRecommendationsResult]:
+    return AwaitableGetPropertyIncludeResult(
+        contract_id=pulumi.get(__ret__, 'contract_id'),
+        group_id=pulumi.get(__ret__, 'group_id'),
+        id=pulumi.get(__ret__, 'id'),
+        include_id=pulumi.get(__ret__, 'include_id'),
+        latest_version=pulumi.get(__ret__, 'latest_version'),
+        name=pulumi.get(__ret__, 'name'),
+        production_version=pulumi.get(__ret__, 'production_version'),
+        staging_version=pulumi.get(__ret__, 'staging_version'),
+        type=pulumi.get(__ret__, 'type'))
+
+
+@_utilities.lift_output_func(get_property_include)
+def get_property_include_output(contract_id: Optional[pulumi.Input[str]] = None,
+                                group_id: Optional[pulumi.Input[str]] = None,
+                                include_id: Optional[pulumi.Input[str]] = None,
+                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPropertyIncludeResult]:
     """
     Use this data source to access information about an existing resource.
     """
     ...
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_version_notes.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_version_notes.py`

 * *Files 8% similar despite different names*

```diff
@@ -78,18 +78,18 @@
     """
     __args__ = dict()
     __args__['configId'] = config_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecVersionNotes:getAppSecVersionNotes', __args__, opts=opts, typ=GetAppSecVersionNotesResult).value
 
     return AwaitableGetAppSecVersionNotesResult(
-        config_id=__ret__.config_id,
-        id=__ret__.id,
-        json=__ret__.json,
-        output_text=__ret__.output_text)
+        config_id=pulumi.get(__ret__, 'config_id'),
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        output_text=pulumi.get(__ret__, 'output_text'))
 
 
 @_utilities.lift_output_func(get_app_sec_version_notes)
 def get_app_sec_version_notes_output(config_id: Optional[pulumi.Input[int]] = None,
                                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecVersionNotesResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_waf_mode.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_waf_mode.py`

 * *Files 22% similar despite different names*

```diff
@@ -134,24 +134,24 @@
     __args__ = dict()
     __args__['configId'] = config_id
     __args__['securityPolicyId'] = security_policy_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecWafMode:getAppSecWafMode', __args__, opts=opts, typ=GetAppSecWafModeResult).value
 
     return AwaitableGetAppSecWafModeResult(
-        config_id=__ret__.config_id,
-        current_ruleset=__ret__.current_ruleset,
-        eval_expiration_date=__ret__.eval_expiration_date,
-        eval_ruleset=__ret__.eval_ruleset,
-        eval_status=__ret__.eval_status,
-        id=__ret__.id,
-        json=__ret__.json,
-        mode=__ret__.mode,
-        output_text=__ret__.output_text,
-        security_policy_id=__ret__.security_policy_id)
+        config_id=pulumi.get(__ret__, 'config_id'),
+        current_ruleset=pulumi.get(__ret__, 'current_ruleset'),
+        eval_expiration_date=pulumi.get(__ret__, 'eval_expiration_date'),
+        eval_ruleset=pulumi.get(__ret__, 'eval_ruleset'),
+        eval_status=pulumi.get(__ret__, 'eval_status'),
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        mode=pulumi.get(__ret__, 'mode'),
+        output_text=pulumi.get(__ret__, 'output_text'),
+        security_policy_id=pulumi.get(__ret__, 'security_policy_id'))
 
 
 @_utilities.lift_output_func(get_app_sec_waf_mode)
 def get_app_sec_waf_mode_output(config_id: Optional[pulumi.Input[int]] = None,
                                 security_policy_id: Optional[pulumi.Input[str]] = None,
                                 opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecWafModeResult]:
     """
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_wap_selected_hostnames.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_app_sec_wap_selected_hostnames.py`

 * *Files 16% similar despite different names*

```diff
@@ -125,23 +125,23 @@
     __args__ = dict()
     __args__['configId'] = config_id
     __args__['securityPolicyId'] = security_policy_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppSecWapSelectedHostnames:getAppSecWapSelectedHostnames', __args__, opts=opts, typ=GetAppSecWapSelectedHostnamesResult).value
 
     return AwaitableGetAppSecWapSelectedHostnamesResult(
-        config_id=__ret__.config_id,
-        evaluated_hosts=__ret__.evaluated_hosts,
-        id=__ret__.id,
-        json=__ret__.json,
-        match_targets=__ret__.match_targets,
-        output_text=__ret__.output_text,
-        protected_hosts=__ret__.protected_hosts,
-        security_policy_id=__ret__.security_policy_id,
-        selected_hosts=__ret__.selected_hosts)
+        config_id=pulumi.get(__ret__, 'config_id'),
+        evaluated_hosts=pulumi.get(__ret__, 'evaluated_hosts'),
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        match_targets=pulumi.get(__ret__, 'match_targets'),
+        output_text=pulumi.get(__ret__, 'output_text'),
+        protected_hosts=pulumi.get(__ret__, 'protected_hosts'),
+        security_policy_id=pulumi.get(__ret__, 'security_policy_id'),
+        selected_hosts=pulumi.get(__ret__, 'selected_hosts'))
 
 
 @_utilities.lift_output_func(get_app_sec_wap_selected_hostnames)
 def get_app_sec_wap_selected_hostnames_output(config_id: Optional[pulumi.Input[int]] = None,
                                               security_policy_id: Optional[pulumi.Input[str]] = None,
                                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSecWapSelectedHostnamesResult]:
     """
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_appsec_advanced_settings_attack_payload_logging.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_appsec_advanced_settings_attack_payload_logging.py`

 * *Files 10% similar despite different names*

```diff
@@ -89,19 +89,19 @@
     __args__ = dict()
     __args__['configId'] = config_id
     __args__['securityPolicyId'] = security_policy_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppsecAdvancedSettingsAttackPayloadLogging:getAppsecAdvancedSettingsAttackPayloadLogging', __args__, opts=opts, typ=GetAppsecAdvancedSettingsAttackPayloadLoggingResult).value
 
     return AwaitableGetAppsecAdvancedSettingsAttackPayloadLoggingResult(
-        config_id=__ret__.config_id,
-        id=__ret__.id,
-        json=__ret__.json,
-        output_text=__ret__.output_text,
-        security_policy_id=__ret__.security_policy_id)
+        config_id=pulumi.get(__ret__, 'config_id'),
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        output_text=pulumi.get(__ret__, 'output_text'),
+        security_policy_id=pulumi.get(__ret__, 'security_policy_id'))
 
 
 @_utilities.lift_output_func(get_appsec_advanced_settings_attack_payload_logging)
 def get_appsec_advanced_settings_attack_payload_logging_output(config_id: Optional[pulumi.Input[int]] = None,
                                                                security_policy_id: Optional[pulumi.Input[Optional[str]]] = None,
                                                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppsecAdvancedSettingsAttackPayloadLoggingResult]:
     """
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_appsec_advanced_settings_request_body.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_appsec_advanced_settings_request_body.py`

 * *Files 12% similar despite different names*

```diff
@@ -89,19 +89,19 @@
     __args__ = dict()
     __args__['configId'] = config_id
     __args__['securityPolicyId'] = security_policy_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAppsecAdvancedSettingsRequestBody:getAppsecAdvancedSettingsRequestBody', __args__, opts=opts, typ=GetAppsecAdvancedSettingsRequestBodyResult).value
 
     return AwaitableGetAppsecAdvancedSettingsRequestBodyResult(
-        config_id=__ret__.config_id,
-        id=__ret__.id,
-        json=__ret__.json,
-        output_text=__ret__.output_text,
-        security_policy_id=__ret__.security_policy_id)
+        config_id=pulumi.get(__ret__, 'config_id'),
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        output_text=pulumi.get(__ret__, 'output_text'),
+        security_policy_id=pulumi.get(__ret__, 'security_policy_id'))
 
 
 @_utilities.lift_output_func(get_appsec_advanced_settings_request_body)
 def get_appsec_advanced_settings_request_body_output(config_id: Optional[pulumi.Input[int]] = None,
                                                      security_policy_id: Optional[pulumi.Input[Optional[str]]] = None,
                                                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppsecAdvancedSettingsRequestBodyResult]:
     """
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_authorities_set.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_authorities_set.py`

 * *Files 13% similar despite different names*

```diff
@@ -69,17 +69,17 @@
     """
     __args__ = dict()
     __args__['contract'] = contract
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getAuthoritiesSet:getAuthoritiesSet', __args__, opts=opts, typ=GetAuthoritiesSetResult).value
 
     return AwaitableGetAuthoritiesSetResult(
-        authorities=__ret__.authorities,
-        contract=__ret__.contract,
-        id=__ret__.id)
+        authorities=pulumi.get(__ret__, 'authorities'),
+        contract=pulumi.get(__ret__, 'contract'),
+        id=pulumi.get(__ret__, 'id'))
 
 
 @_utilities.lift_output_func(get_authorities_set)
 def get_authorities_set_output(contract: Optional[pulumi.Input[str]] = None,
                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAuthoritiesSetResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cloudlets_api_prioritization_match_rule.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_cloudlets_api_prioritization_match_rule.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,17 +71,17 @@
     """
     __args__ = dict()
     __args__['matchRules'] = match_rules
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getCloudletsApiPrioritizationMatchRule:getCloudletsApiPrioritizationMatchRule', __args__, opts=opts, typ=GetCloudletsApiPrioritizationMatchRuleResult).value
 
     return AwaitableGetCloudletsApiPrioritizationMatchRuleResult(
-        id=__ret__.id,
-        json=__ret__.json,
-        match_rules=__ret__.match_rules)
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        match_rules=pulumi.get(__ret__, 'match_rules'))
 
 
 @_utilities.lift_output_func(get_cloudlets_api_prioritization_match_rule)
 def get_cloudlets_api_prioritization_match_rule_output(match_rules: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetCloudletsApiPrioritizationMatchRuleMatchRuleArgs']]]]] = None,
                                                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCloudletsApiPrioritizationMatchRuleResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cloudlets_application_load_balancer.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_cloudlets_application_load_balancer.py`

 * *Files 4% similar despite different names*

```diff
@@ -180,29 +180,29 @@
     __args__ = dict()
     __args__['originId'] = origin_id
     __args__['version'] = version
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getCloudletsApplicationLoadBalancer:getCloudletsApplicationLoadBalancer', __args__, opts=opts, typ=GetCloudletsApplicationLoadBalancerResult).value
 
     return AwaitableGetCloudletsApplicationLoadBalancerResult(
-        balancing_type=__ret__.balancing_type,
-        created_by=__ret__.created_by,
-        created_date=__ret__.created_date,
-        data_centers=__ret__.data_centers,
-        deleted=__ret__.deleted,
-        description=__ret__.description,
-        id=__ret__.id,
-        immutable=__ret__.immutable,
-        last_modified_by=__ret__.last_modified_by,
-        last_modified_date=__ret__.last_modified_date,
-        liveness_settings=__ret__.liveness_settings,
-        origin_id=__ret__.origin_id,
-        type=__ret__.type,
-        version=__ret__.version,
-        warnings=__ret__.warnings)
+        balancing_type=pulumi.get(__ret__, 'balancing_type'),
+        created_by=pulumi.get(__ret__, 'created_by'),
+        created_date=pulumi.get(__ret__, 'created_date'),
+        data_centers=pulumi.get(__ret__, 'data_centers'),
+        deleted=pulumi.get(__ret__, 'deleted'),
+        description=pulumi.get(__ret__, 'description'),
+        id=pulumi.get(__ret__, 'id'),
+        immutable=pulumi.get(__ret__, 'immutable'),
+        last_modified_by=pulumi.get(__ret__, 'last_modified_by'),
+        last_modified_date=pulumi.get(__ret__, 'last_modified_date'),
+        liveness_settings=pulumi.get(__ret__, 'liveness_settings'),
+        origin_id=pulumi.get(__ret__, 'origin_id'),
+        type=pulumi.get(__ret__, 'type'),
+        version=pulumi.get(__ret__, 'version'),
+        warnings=pulumi.get(__ret__, 'warnings'))
 
 
 @_utilities.lift_output_func(get_cloudlets_application_load_balancer)
 def get_cloudlets_application_load_balancer_output(origin_id: Optional[pulumi.Input[str]] = None,
                                                    version: Optional[pulumi.Input[Optional[int]]] = None,
                                                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCloudletsApplicationLoadBalancerResult]:
     """
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cloudlets_application_load_balancer_match_rule.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_cloudlets_application_load_balancer_match_rule.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,17 +71,17 @@
     """
     __args__ = dict()
     __args__['matchRules'] = match_rules
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getCloudletsApplicationLoadBalancerMatchRule:getCloudletsApplicationLoadBalancerMatchRule', __args__, opts=opts, typ=GetCloudletsApplicationLoadBalancerMatchRuleResult).value
 
     return AwaitableGetCloudletsApplicationLoadBalancerMatchRuleResult(
-        id=__ret__.id,
-        json=__ret__.json,
-        match_rules=__ret__.match_rules)
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        match_rules=pulumi.get(__ret__, 'match_rules'))
 
 
 @_utilities.lift_output_func(get_cloudlets_application_load_balancer_match_rule)
 def get_cloudlets_application_load_balancer_match_rule_output(match_rules: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetCloudletsApplicationLoadBalancerMatchRuleMatchRuleArgs']]]]] = None,
                                                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCloudletsApplicationLoadBalancerMatchRuleResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cloudlets_audience_segmentation_match_rule.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_cloudlets_audience_segmentation_match_rule.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,17 +71,17 @@
     """
     __args__ = dict()
     __args__['matchRules'] = match_rules
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getCloudletsAudienceSegmentationMatchRule:getCloudletsAudienceSegmentationMatchRule', __args__, opts=opts, typ=GetCloudletsAudienceSegmentationMatchRuleResult).value
 
     return AwaitableGetCloudletsAudienceSegmentationMatchRuleResult(
-        id=__ret__.id,
-        json=__ret__.json,
-        match_rules=__ret__.match_rules)
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        match_rules=pulumi.get(__ret__, 'match_rules'))
 
 
 @_utilities.lift_output_func(get_cloudlets_audience_segmentation_match_rule)
 def get_cloudlets_audience_segmentation_match_rule_output(match_rules: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetCloudletsAudienceSegmentationMatchRuleMatchRuleArgs']]]]] = None,
                                                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCloudletsAudienceSegmentationMatchRuleResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cloudlets_edge_redirector_match_rule.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_cloudlets_edge_redirector_match_rule.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,17 +71,17 @@
     """
     __args__ = dict()
     __args__['matchRules'] = match_rules
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getCloudletsEdgeRedirectorMatchRule:getCloudletsEdgeRedirectorMatchRule', __args__, opts=opts, typ=GetCloudletsEdgeRedirectorMatchRuleResult).value
 
     return AwaitableGetCloudletsEdgeRedirectorMatchRuleResult(
-        id=__ret__.id,
-        json=__ret__.json,
-        match_rules=__ret__.match_rules)
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        match_rules=pulumi.get(__ret__, 'match_rules'))
 
 
 @_utilities.lift_output_func(get_cloudlets_edge_redirector_match_rule)
 def get_cloudlets_edge_redirector_match_rule_output(match_rules: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetCloudletsEdgeRedirectorMatchRuleMatchRuleArgs']]]]] = None,
                                                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCloudletsEdgeRedirectorMatchRuleResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cloudlets_forward_rewrite_match_rule.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_cloudlets_forward_rewrite_match_rule.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,17 +71,17 @@
     """
     __args__ = dict()
     __args__['matchRules'] = match_rules
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getCloudletsForwardRewriteMatchRule:getCloudletsForwardRewriteMatchRule', __args__, opts=opts, typ=GetCloudletsForwardRewriteMatchRuleResult).value
 
     return AwaitableGetCloudletsForwardRewriteMatchRuleResult(
-        id=__ret__.id,
-        json=__ret__.json,
-        match_rules=__ret__.match_rules)
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        match_rules=pulumi.get(__ret__, 'match_rules'))
 
 
 @_utilities.lift_output_func(get_cloudlets_forward_rewrite_match_rule)
 def get_cloudlets_forward_rewrite_match_rule_output(match_rules: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetCloudletsForwardRewriteMatchRuleMatchRuleArgs']]]]] = None,
                                                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCloudletsForwardRewriteMatchRuleResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cloudlets_phased_release_match_rule.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_cloudlets_phased_release_match_rule.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,17 +71,17 @@
     """
     __args__ = dict()
     __args__['matchRules'] = match_rules
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getCloudletsPhasedReleaseMatchRule:getCloudletsPhasedReleaseMatchRule', __args__, opts=opts, typ=GetCloudletsPhasedReleaseMatchRuleResult).value
 
     return AwaitableGetCloudletsPhasedReleaseMatchRuleResult(
-        id=__ret__.id,
-        json=__ret__.json,
-        match_rules=__ret__.match_rules)
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        match_rules=pulumi.get(__ret__, 'match_rules'))
 
 
 @_utilities.lift_output_func(get_cloudlets_phased_release_match_rule)
 def get_cloudlets_phased_release_match_rule_output(match_rules: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetCloudletsPhasedReleaseMatchRuleMatchRuleArgs']]]]] = None,
                                                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCloudletsPhasedReleaseMatchRuleResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cloudlets_policy.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_cloudlets_policy.py`

 * *Files 16% similar despite different names*

```diff
@@ -189,30 +189,30 @@
     __args__ = dict()
     __args__['policyId'] = policy_id
     __args__['version'] = version
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getCloudletsPolicy:getCloudletsPolicy', __args__, opts=opts, typ=GetCloudletsPolicyResult).value
 
     return AwaitableGetCloudletsPolicyResult(
-        activations=__ret__.activations,
-        api_version=__ret__.api_version,
-        cloudlet_code=__ret__.cloudlet_code,
-        cloudlet_id=__ret__.cloudlet_id,
-        description=__ret__.description,
-        group_id=__ret__.group_id,
-        id=__ret__.id,
-        match_rule_format=__ret__.match_rule_format,
-        match_rules=__ret__.match_rules,
-        name=__ret__.name,
-        policy_id=__ret__.policy_id,
-        revision_id=__ret__.revision_id,
-        rules_locked=__ret__.rules_locked,
-        version=__ret__.version,
-        version_description=__ret__.version_description,
-        warnings=__ret__.warnings)
+        activations=pulumi.get(__ret__, 'activations'),
+        api_version=pulumi.get(__ret__, 'api_version'),
+        cloudlet_code=pulumi.get(__ret__, 'cloudlet_code'),
+        cloudlet_id=pulumi.get(__ret__, 'cloudlet_id'),
+        description=pulumi.get(__ret__, 'description'),
+        group_id=pulumi.get(__ret__, 'group_id'),
+        id=pulumi.get(__ret__, 'id'),
+        match_rule_format=pulumi.get(__ret__, 'match_rule_format'),
+        match_rules=pulumi.get(__ret__, 'match_rules'),
+        name=pulumi.get(__ret__, 'name'),
+        policy_id=pulumi.get(__ret__, 'policy_id'),
+        revision_id=pulumi.get(__ret__, 'revision_id'),
+        rules_locked=pulumi.get(__ret__, 'rules_locked'),
+        version=pulumi.get(__ret__, 'version'),
+        version_description=pulumi.get(__ret__, 'version_description'),
+        warnings=pulumi.get(__ret__, 'warnings'))
 
 
 @_utilities.lift_output_func(get_cloudlets_policy)
 def get_cloudlets_policy_output(policy_id: Optional[pulumi.Input[int]] = None,
                                 version: Optional[pulumi.Input[Optional[int]]] = None,
                                 opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCloudletsPolicyResult]:
     """
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cloudlets_request_control_match_rule.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_cloudlets_request_control_match_rule.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,17 +71,17 @@
     """
     __args__ = dict()
     __args__['matchRules'] = match_rules
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getCloudletsRequestControlMatchRule:getCloudletsRequestControlMatchRule', __args__, opts=opts, typ=GetCloudletsRequestControlMatchRuleResult).value
 
     return AwaitableGetCloudletsRequestControlMatchRuleResult(
-        id=__ret__.id,
-        json=__ret__.json,
-        match_rules=__ret__.match_rules)
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        match_rules=pulumi.get(__ret__, 'match_rules'))
 
 
 @_utilities.lift_output_func(get_cloudlets_request_control_match_rule)
 def get_cloudlets_request_control_match_rule_output(match_rules: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetCloudletsRequestControlMatchRuleMatchRuleArgs']]]]] = None,
                                                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCloudletsRequestControlMatchRuleResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cloudlets_visitor_prioritization_match_rule.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_cloudlets_visitor_prioritization_match_rule.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,17 +71,17 @@
     """
     __args__ = dict()
     __args__['matchRules'] = match_rules
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getCloudletsVisitorPrioritizationMatchRule:getCloudletsVisitorPrioritizationMatchRule', __args__, opts=opts, typ=GetCloudletsVisitorPrioritizationMatchRuleResult).value
 
     return AwaitableGetCloudletsVisitorPrioritizationMatchRuleResult(
-        id=__ret__.id,
-        json=__ret__.json,
-        match_rules=__ret__.match_rules)
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        match_rules=pulumi.get(__ret__, 'match_rules'))
 
 
 @_utilities.lift_output_func(get_cloudlets_visitor_prioritization_match_rule)
 def get_cloudlets_visitor_prioritization_match_rule_output(match_rules: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetCloudletsVisitorPrioritizationMatchRuleMatchRuleArgs']]]]] = None,
                                                            opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCloudletsVisitorPrioritizationMatchRuleResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_contract.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_contract.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,32 +20,31 @@
 class GetContractResult:
     """
     A collection of values returned by getContract.
     """
     def __init__(__self__, group=None, group_id=None, group_name=None, id=None):
         if group and not isinstance(group, str):
             raise TypeError("Expected argument 'group' to be a str")
-        if group is not None:
-            warnings.warn("""The setting \"group\" has been deprecated.""", DeprecationWarning)
-            pulumi.log.warn("""group is deprecated: The setting \"group\" has been deprecated.""")
-
         pulumi.set(__self__, "group", group)
         if group_id and not isinstance(group_id, str):
             raise TypeError("Expected argument 'group_id' to be a str")
         pulumi.set(__self__, "group_id", group_id)
         if group_name and not isinstance(group_name, str):
             raise TypeError("Expected argument 'group_name' to be a str")
         pulumi.set(__self__, "group_name", group_name)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
 
     @property
     @pulumi.getter
     def group(self) -> Optional[str]:
+        warnings.warn("""The setting \"group\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""group is deprecated: The setting \"group\" has been deprecated.""")
+
         return pulumi.get(self, "group")
 
     @property
     @pulumi.getter(name="groupId")
     def group_id(self) -> str:
         return pulumi.get(self, "group_id")
 
@@ -86,18 +85,18 @@
     __args__['group'] = group
     __args__['groupId'] = group_id
     __args__['groupName'] = group_name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getContract:getContract', __args__, opts=opts, typ=GetContractResult).value
 
     return AwaitableGetContractResult(
-        group=__ret__.group,
-        group_id=__ret__.group_id,
-        group_name=__ret__.group_name,
-        id=__ret__.id)
+        group=pulumi.get(__ret__, 'group'),
+        group_id=pulumi.get(__ret__, 'group_id'),
+        group_name=pulumi.get(__ret__, 'group_name'),
+        id=pulumi.get(__ret__, 'id'))
 
 
 @_utilities.lift_output_func(get_contract)
 def get_contract_output(group: Optional[pulumi.Input[Optional[str]]] = None,
                         group_id: Optional[pulumi.Input[Optional[str]]] = None,
                         group_name: Optional[pulumi.Input[Optional[str]]] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetContractResult]:
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_contracts.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_contracts.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,9 +58,9 @@
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getContracts:getContracts', __args__, opts=opts, typ=GetContractsResult).value
 
     return AwaitableGetContractsResult(
-        contracts=__ret__.contracts,
-        id=__ret__.id)
+        contracts=pulumi.get(__ret__, 'contracts'),
+        id=pulumi.get(__ret__, 'id'))
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cp_code.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/properties/get_cp_code.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,45 +3,39 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from . import _utilities
+from .. import _utilities
 
 __all__ = [
     'GetCpCodeResult',
     'AwaitableGetCpCodeResult',
     'get_cp_code',
     'get_cp_code_output',
 ]
 
+warnings.warn("""akamai.properties/getcpcode.getCpCode has been deprecated in favor of akamai.index/getcpcode.getCpCode""", DeprecationWarning)
+
 @pulumi.output_type
 class GetCpCodeResult:
     """
     A collection of values returned by getCpCode.
     """
     def __init__(__self__, contract=None, contract_id=None, group=None, group_id=None, id=None, name=None, product_ids=None):
         if contract and not isinstance(contract, str):
             raise TypeError("Expected argument 'contract' to be a str")
-        if contract is not None:
-            warnings.warn("""The setting \"contract\" has been deprecated.""", DeprecationWarning)
-            pulumi.log.warn("""contract is deprecated: The setting \"contract\" has been deprecated.""")
-
         pulumi.set(__self__, "contract", contract)
         if contract_id and not isinstance(contract_id, str):
             raise TypeError("Expected argument 'contract_id' to be a str")
         pulumi.set(__self__, "contract_id", contract_id)
         if group and not isinstance(group, str):
             raise TypeError("Expected argument 'group' to be a str")
-        if group is not None:
-            warnings.warn("""The setting \"group\" has been deprecated.""", DeprecationWarning)
-            pulumi.log.warn("""group is deprecated: The setting \"group\" has been deprecated.""")
-
         pulumi.set(__self__, "group", group)
         if group_id and not isinstance(group_id, str):
             raise TypeError("Expected argument 'group_id' to be a str")
         pulumi.set(__self__, "group_id", group_id)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
@@ -51,24 +45,30 @@
         if product_ids and not isinstance(product_ids, list):
             raise TypeError("Expected argument 'product_ids' to be a list")
         pulumi.set(__self__, "product_ids", product_ids)
 
     @property
     @pulumi.getter
     def contract(self) -> str:
+        warnings.warn("""The setting \"contract\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""contract is deprecated: The setting \"contract\" has been deprecated.""")
+
         return pulumi.get(self, "contract")
 
     @property
     @pulumi.getter(name="contractId")
     def contract_id(self) -> str:
         return pulumi.get(self, "contract_id")
 
     @property
     @pulumi.getter
     def group(self) -> str:
+        warnings.warn("""The setting \"group\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""group is deprecated: The setting \"group\" has been deprecated.""")
+
         return pulumi.get(self, "group")
 
     @property
     @pulumi.getter(name="groupId")
     def group_id(self) -> str:
         return pulumi.get(self, "group_id")
 
@@ -111,37 +111,39 @@
                 group: Optional[str] = None,
                 group_id: Optional[str] = None,
                 name: Optional[str] = None,
                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetCpCodeResult:
     """
     Use this data source to access information about an existing resource.
     """
+    pulumi.log.warn("""get_cp_code is deprecated: akamai.properties/getcpcode.getCpCode has been deprecated in favor of akamai.index/getcpcode.getCpCode""")
     __args__ = dict()
     __args__['contract'] = contract
     __args__['contractId'] = contract_id
     __args__['group'] = group
     __args__['groupId'] = group_id
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('akamai:index/getCpCode:getCpCode', __args__, opts=opts, typ=GetCpCodeResult).value
+    __ret__ = pulumi.runtime.invoke('akamai:properties/getCpCode:getCpCode', __args__, opts=opts, typ=GetCpCodeResult).value
 
     return AwaitableGetCpCodeResult(
-        contract=__ret__.contract,
-        contract_id=__ret__.contract_id,
-        group=__ret__.group,
-        group_id=__ret__.group_id,
-        id=__ret__.id,
-        name=__ret__.name,
-        product_ids=__ret__.product_ids)
+        contract=pulumi.get(__ret__, 'contract'),
+        contract_id=pulumi.get(__ret__, 'contract_id'),
+        group=pulumi.get(__ret__, 'group'),
+        group_id=pulumi.get(__ret__, 'group_id'),
+        id=pulumi.get(__ret__, 'id'),
+        name=pulumi.get(__ret__, 'name'),
+        product_ids=pulumi.get(__ret__, 'product_ids'))
 
 
 @_utilities.lift_output_func(get_cp_code)
 def get_cp_code_output(contract: Optional[pulumi.Input[Optional[str]]] = None,
                        contract_id: Optional[pulumi.Input[Optional[str]]] = None,
                        group: Optional[pulumi.Input[Optional[str]]] = None,
                        group_id: Optional[pulumi.Input[Optional[str]]] = None,
                        name: Optional[pulumi.Input[str]] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCpCodeResult]:
     """
     Use this data source to access information about an existing resource.
     """
+    pulumi.log.warn("""get_cp_code is deprecated: akamai.properties/getcpcode.getCpCode has been deprecated in favor of akamai.index/getcpcode.getCpCode""")
     ...
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cps_csr.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_cps_csr.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,18 +78,18 @@
     """
     __args__ = dict()
     __args__['enrollmentId'] = enrollment_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getCpsCsr:getCpsCsr', __args__, opts=opts, typ=GetCpsCsrResult).value
 
     return AwaitableGetCpsCsrResult(
-        csr_ecdsa=__ret__.csr_ecdsa,
-        csr_rsa=__ret__.csr_rsa,
-        enrollment_id=__ret__.enrollment_id,
-        id=__ret__.id)
+        csr_ecdsa=pulumi.get(__ret__, 'csr_ecdsa'),
+        csr_rsa=pulumi.get(__ret__, 'csr_rsa'),
+        enrollment_id=pulumi.get(__ret__, 'enrollment_id'),
+        id=pulumi.get(__ret__, 'id'))
 
 
 @_utilities.lift_output_func(get_cps_csr)
 def get_cps_csr_output(enrollment_id: Optional[pulumi.Input[int]] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCpsCsrResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cps_deployments.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_cps_deployments.py`

 * *Files 5% similar despite different names*

```diff
@@ -114,22 +114,22 @@
     """
     __args__ = dict()
     __args__['enrollmentId'] = enrollment_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getCpsDeployments:getCpsDeployments', __args__, opts=opts, typ=GetCpsDeploymentsResult).value
 
     return AwaitableGetCpsDeploymentsResult(
-        auto_renewal_start_time=__ret__.auto_renewal_start_time,
-        enrollment_id=__ret__.enrollment_id,
-        expiry_date=__ret__.expiry_date,
-        id=__ret__.id,
-        production_certificate_ecdsa=__ret__.production_certificate_ecdsa,
-        production_certificate_rsa=__ret__.production_certificate_rsa,
-        staging_certificate_ecdsa=__ret__.staging_certificate_ecdsa,
-        staging_certificate_rsa=__ret__.staging_certificate_rsa)
+        auto_renewal_start_time=pulumi.get(__ret__, 'auto_renewal_start_time'),
+        enrollment_id=pulumi.get(__ret__, 'enrollment_id'),
+        expiry_date=pulumi.get(__ret__, 'expiry_date'),
+        id=pulumi.get(__ret__, 'id'),
+        production_certificate_ecdsa=pulumi.get(__ret__, 'production_certificate_ecdsa'),
+        production_certificate_rsa=pulumi.get(__ret__, 'production_certificate_rsa'),
+        staging_certificate_ecdsa=pulumi.get(__ret__, 'staging_certificate_ecdsa'),
+        staging_certificate_rsa=pulumi.get(__ret__, 'staging_certificate_rsa'))
 
 
 @_utilities.lift_output_func(get_cps_deployments)
 def get_cps_deployments_output(enrollment_id: Optional[pulumi.Input[int]] = None,
                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCpsDeploymentsResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cps_enrollment.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_cps_enrollment.py`

 * *Files 7% similar despite different names*

```diff
@@ -223,34 +223,34 @@
     """
     __args__ = dict()
     __args__['enrollmentId'] = enrollment_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getCPSEnrollment:getCPSEnrollment', __args__, opts=opts, typ=GetCPSEnrollmentResult).value
 
     return AwaitableGetCPSEnrollmentResult(
-        admin_contacts=__ret__.admin_contacts,
-        certificate_chain_type=__ret__.certificate_chain_type,
-        certificate_type=__ret__.certificate_type,
-        common_name=__ret__.common_name,
-        contract_id=__ret__.contract_id,
-        csrs=__ret__.csrs,
-        dns_challenges=__ret__.dns_challenges,
-        enable_multi_stacked_certificates=__ret__.enable_multi_stacked_certificates,
-        enrollment_id=__ret__.enrollment_id,
-        http_challenges=__ret__.http_challenges,
-        id=__ret__.id,
-        network_configurations=__ret__.network_configurations,
-        organizations=__ret__.organizations,
-        registration_authority=__ret__.registration_authority,
-        sans=__ret__.sans,
-        secure_network=__ret__.secure_network,
-        signature_algorithm=__ret__.signature_algorithm,
-        sni_only=__ret__.sni_only,
-        tech_contacts=__ret__.tech_contacts,
-        validation_type=__ret__.validation_type)
+        admin_contacts=pulumi.get(__ret__, 'admin_contacts'),
+        certificate_chain_type=pulumi.get(__ret__, 'certificate_chain_type'),
+        certificate_type=pulumi.get(__ret__, 'certificate_type'),
+        common_name=pulumi.get(__ret__, 'common_name'),
+        contract_id=pulumi.get(__ret__, 'contract_id'),
+        csrs=pulumi.get(__ret__, 'csrs'),
+        dns_challenges=pulumi.get(__ret__, 'dns_challenges'),
+        enable_multi_stacked_certificates=pulumi.get(__ret__, 'enable_multi_stacked_certificates'),
+        enrollment_id=pulumi.get(__ret__, 'enrollment_id'),
+        http_challenges=pulumi.get(__ret__, 'http_challenges'),
+        id=pulumi.get(__ret__, 'id'),
+        network_configurations=pulumi.get(__ret__, 'network_configurations'),
+        organizations=pulumi.get(__ret__, 'organizations'),
+        registration_authority=pulumi.get(__ret__, 'registration_authority'),
+        sans=pulumi.get(__ret__, 'sans'),
+        secure_network=pulumi.get(__ret__, 'secure_network'),
+        signature_algorithm=pulumi.get(__ret__, 'signature_algorithm'),
+        sni_only=pulumi.get(__ret__, 'sni_only'),
+        tech_contacts=pulumi.get(__ret__, 'tech_contacts'),
+        validation_type=pulumi.get(__ret__, 'validation_type'))
 
 
 @_utilities.lift_output_func(get_cps_enrollment)
 def get_cps_enrollment_output(enrollment_id: Optional[pulumi.Input[int]] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCPSEnrollmentResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cps_enrollments.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_cps_enrollments.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,17 +70,17 @@
     """
     __args__ = dict()
     __args__['contractId'] = contract_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getCPSEnrollments:getCPSEnrollments', __args__, opts=opts, typ=GetCPSEnrollmentsResult).value
 
     return AwaitableGetCPSEnrollmentsResult(
-        contract_id=__ret__.contract_id,
-        enrollments=__ret__.enrollments,
-        id=__ret__.id)
+        contract_id=pulumi.get(__ret__, 'contract_id'),
+        enrollments=pulumi.get(__ret__, 'enrollments'),
+        id=pulumi.get(__ret__, 'id'))
 
 
 @_utilities.lift_output_func(get_cps_enrollments)
 def get_cps_enrollments_output(contract_id: Optional[pulumi.Input[str]] = None,
                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCPSEnrollmentsResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cps_warnings.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_cps_warnings.py`

 * *Files 9% similar despite different names*

```diff
@@ -57,9 +57,9 @@
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getCpsWarnings:getCpsWarnings', __args__, opts=opts, typ=GetCpsWarningsResult).value
 
     return AwaitableGetCpsWarningsResult(
-        id=__ret__.id,
-        warnings=__ret__.warnings)
+        id=pulumi.get(__ret__, 'id'),
+        warnings=pulumi.get(__ret__, 'warnings'))
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_datastream_activation_history.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_datastream_activation_history.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,17 +70,17 @@
     """
     __args__ = dict()
     __args__['streamId'] = stream_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getDatastreamActivationHistory:getDatastreamActivationHistory', __args__, opts=opts, typ=GetDatastreamActivationHistoryResult).value
 
     return AwaitableGetDatastreamActivationHistoryResult(
-        activations=__ret__.activations,
-        id=__ret__.id,
-        stream_id=__ret__.stream_id)
+        activations=pulumi.get(__ret__, 'activations'),
+        id=pulumi.get(__ret__, 'id'),
+        stream_id=pulumi.get(__ret__, 'stream_id'))
 
 
 @_utilities.lift_output_func(get_datastream_activation_history)
 def get_datastream_activation_history_output(stream_id: Optional[pulumi.Input[int]] = None,
                                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDatastreamActivationHistoryResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_datastream_dataset_fields.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_datastream_dataset_fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,17 +70,17 @@
     """
     __args__ = dict()
     __args__['templateName'] = template_name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getDatastreamDatasetFields:getDatastreamDatasetFields', __args__, opts=opts, typ=GetDatastreamDatasetFieldsResult).value
 
     return AwaitableGetDatastreamDatasetFieldsResult(
-        fields=__ret__.fields,
-        id=__ret__.id,
-        template_name=__ret__.template_name)
+        fields=pulumi.get(__ret__, 'fields'),
+        id=pulumi.get(__ret__, 'id'),
+        template_name=pulumi.get(__ret__, 'template_name'))
 
 
 @_utilities.lift_output_func(get_datastream_dataset_fields)
 def get_datastream_dataset_fields_output(template_name: Optional[pulumi.Input[Optional[str]]] = None,
                                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDatastreamDatasetFieldsResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_datastreams.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_datastreams.py`

 * *Files 14% similar despite different names*

```diff
@@ -70,17 +70,17 @@
     """
     __args__ = dict()
     __args__['groupId'] = group_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getDatastreams:getDatastreams', __args__, opts=opts, typ=GetDatastreamsResult).value
 
     return AwaitableGetDatastreamsResult(
-        group_id=__ret__.group_id,
-        id=__ret__.id,
-        streams=__ret__.streams)
+        group_id=pulumi.get(__ret__, 'group_id'),
+        id=pulumi.get(__ret__, 'id'),
+        streams=pulumi.get(__ret__, 'streams'))
 
 
 @_utilities.lift_output_func(get_datastreams)
 def get_datastreams_output(group_id: Optional[pulumi.Input[Optional[str]]] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDatastreamsResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_dns_record_set.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_dns_record_set.py`

 * *Files 14% similar despite different names*

```diff
@@ -91,19 +91,19 @@
     __args__['host'] = host
     __args__['recordType'] = record_type
     __args__['zone'] = zone
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getDnsRecordSet:getDnsRecordSet', __args__, opts=opts, typ=GetDnsRecordSetResult).value
 
     return AwaitableGetDnsRecordSetResult(
-        host=__ret__.host,
-        id=__ret__.id,
-        rdatas=__ret__.rdatas,
-        record_type=__ret__.record_type,
-        zone=__ret__.zone)
+        host=pulumi.get(__ret__, 'host'),
+        id=pulumi.get(__ret__, 'id'),
+        rdatas=pulumi.get(__ret__, 'rdatas'),
+        record_type=pulumi.get(__ret__, 'record_type'),
+        zone=pulumi.get(__ret__, 'zone'))
 
 
 @_utilities.lift_output_func(get_dns_record_set)
 def get_dns_record_set_output(host: Optional[pulumi.Input[str]] = None,
                               record_type: Optional[pulumi.Input[str]] = None,
                               zone: Optional[pulumi.Input[str]] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDnsRecordSetResult]:
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_edge_worker.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_edge_worker.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,23 +125,23 @@
     __args__ = dict()
     __args__['edgeworkerId'] = edgeworker_id
     __args__['localBundle'] = local_bundle
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getEdgeWorker:getEdgeWorker', __args__, opts=opts, typ=GetEdgeWorkerResult).value
 
     return AwaitableGetEdgeWorkerResult(
-        edgeworker_id=__ret__.edgeworker_id,
-        group_id=__ret__.group_id,
-        id=__ret__.id,
-        local_bundle=__ret__.local_bundle,
-        local_bundle_hash=__ret__.local_bundle_hash,
-        name=__ret__.name,
-        resource_tier_id=__ret__.resource_tier_id,
-        version=__ret__.version,
-        warnings=__ret__.warnings)
+        edgeworker_id=pulumi.get(__ret__, 'edgeworker_id'),
+        group_id=pulumi.get(__ret__, 'group_id'),
+        id=pulumi.get(__ret__, 'id'),
+        local_bundle=pulumi.get(__ret__, 'local_bundle'),
+        local_bundle_hash=pulumi.get(__ret__, 'local_bundle_hash'),
+        name=pulumi.get(__ret__, 'name'),
+        resource_tier_id=pulumi.get(__ret__, 'resource_tier_id'),
+        version=pulumi.get(__ret__, 'version'),
+        warnings=pulumi.get(__ret__, 'warnings'))
 
 
 @_utilities.lift_output_func(get_edge_worker)
 def get_edge_worker_output(edgeworker_id: Optional[pulumi.Input[int]] = None,
                            local_bundle: Optional[pulumi.Input[Optional[str]]] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetEdgeWorkerResult]:
     """
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_edge_worker_activation.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_edge_worker_activation.py`

 * *Files 10% similar despite different names*

```diff
@@ -89,19 +89,19 @@
     __args__ = dict()
     __args__['edgeworkerId'] = edgeworker_id
     __args__['network'] = network
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getEdgeWorkerActivation:getEdgeWorkerActivation', __args__, opts=opts, typ=GetEdgeWorkerActivationResult).value
 
     return AwaitableGetEdgeWorkerActivationResult(
-        activation_id=__ret__.activation_id,
-        edgeworker_id=__ret__.edgeworker_id,
-        id=__ret__.id,
-        network=__ret__.network,
-        version=__ret__.version)
+        activation_id=pulumi.get(__ret__, 'activation_id'),
+        edgeworker_id=pulumi.get(__ret__, 'edgeworker_id'),
+        id=pulumi.get(__ret__, 'id'),
+        network=pulumi.get(__ret__, 'network'),
+        version=pulumi.get(__ret__, 'version'))
 
 
 @_utilities.lift_output_func(get_edge_worker_activation)
 def get_edge_worker_activation_output(edgeworker_id: Optional[pulumi.Input[int]] = None,
                                       network: Optional[pulumi.Input[str]] = None,
                                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetEdgeWorkerActivationResult]:
     """
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_edge_workers_property_rules.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_edge_workers_property_rules.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,17 +69,17 @@
     """
     __args__ = dict()
     __args__['edgeworkerId'] = edgeworker_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getEdgeWorkersPropertyRules:getEdgeWorkersPropertyRules', __args__, opts=opts, typ=GetEdgeWorkersPropertyRulesResult).value
 
     return AwaitableGetEdgeWorkersPropertyRulesResult(
-        edgeworker_id=__ret__.edgeworker_id,
-        id=__ret__.id,
-        json=__ret__.json)
+        edgeworker_id=pulumi.get(__ret__, 'edgeworker_id'),
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'))
 
 
 @_utilities.lift_output_func(get_edge_workers_property_rules)
 def get_edge_workers_property_rules_output(edgeworker_id: Optional[pulumi.Input[int]] = None,
                                            opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetEdgeWorkersPropertyRulesResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_edge_workers_resource_tier.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_edge_workers_resource_tier.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,18 +80,18 @@
     __args__ = dict()
     __args__['contractId'] = contract_id
     __args__['resourceTierName'] = resource_tier_name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getEdgeWorkersResourceTier:getEdgeWorkersResourceTier', __args__, opts=opts, typ=GetEdgeWorkersResourceTierResult).value
 
     return AwaitableGetEdgeWorkersResourceTierResult(
-        contract_id=__ret__.contract_id,
-        id=__ret__.id,
-        resource_tier_id=__ret__.resource_tier_id,
-        resource_tier_name=__ret__.resource_tier_name)
+        contract_id=pulumi.get(__ret__, 'contract_id'),
+        id=pulumi.get(__ret__, 'id'),
+        resource_tier_id=pulumi.get(__ret__, 'resource_tier_id'),
+        resource_tier_name=pulumi.get(__ret__, 'resource_tier_name'))
 
 
 @_utilities.lift_output_func(get_edge_workers_resource_tier)
 def get_edge_workers_resource_tier_output(contract_id: Optional[pulumi.Input[str]] = None,
                                           resource_tier_name: Optional[pulumi.Input[str]] = None,
                                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetEdgeWorkersResourceTierResult]:
     """
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_edgekv_group_items.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_edgekv_group_items.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,19 +91,19 @@
     __args__['groupName'] = group_name
     __args__['namespaceName'] = namespace_name
     __args__['network'] = network
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getEdgekvGroupItems:getEdgekvGroupItems', __args__, opts=opts, typ=GetEdgekvGroupItemsResult).value
 
     return AwaitableGetEdgekvGroupItemsResult(
-        group_name=__ret__.group_name,
-        id=__ret__.id,
-        items=__ret__.items,
-        namespace_name=__ret__.namespace_name,
-        network=__ret__.network)
+        group_name=pulumi.get(__ret__, 'group_name'),
+        id=pulumi.get(__ret__, 'id'),
+        items=pulumi.get(__ret__, 'items'),
+        namespace_name=pulumi.get(__ret__, 'namespace_name'),
+        network=pulumi.get(__ret__, 'network'))
 
 
 @_utilities.lift_output_func(get_edgekv_group_items)
 def get_edgekv_group_items_output(group_name: Optional[pulumi.Input[str]] = None,
                                   namespace_name: Optional[pulumi.Input[str]] = None,
                                   network: Optional[pulumi.Input[str]] = None,
                                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetEdgekvGroupItemsResult]:
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_edgekv_groups.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_edgekv_groups.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,18 +80,18 @@
     __args__ = dict()
     __args__['namespaceName'] = namespace_name
     __args__['network'] = network
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getEdgekvGroups:getEdgekvGroups', __args__, opts=opts, typ=GetEdgekvGroupsResult).value
 
     return AwaitableGetEdgekvGroupsResult(
-        groups=__ret__.groups,
-        id=__ret__.id,
-        namespace_name=__ret__.namespace_name,
-        network=__ret__.network)
+        groups=pulumi.get(__ret__, 'groups'),
+        id=pulumi.get(__ret__, 'id'),
+        namespace_name=pulumi.get(__ret__, 'namespace_name'),
+        network=pulumi.get(__ret__, 'network'))
 
 
 @_utilities.lift_output_func(get_edgekv_groups)
 def get_edgekv_groups_output(namespace_name: Optional[pulumi.Input[str]] = None,
                              network: Optional[pulumi.Input[str]] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetEdgekvGroupsResult]:
     """
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_group.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,39 +20,34 @@
 class GetGroupResult:
     """
     A collection of values returned by getGroup.
     """
     def __init__(__self__, contract=None, contract_id=None, group_name=None, id=None, name=None):
         if contract and not isinstance(contract, str):
             raise TypeError("Expected argument 'contract' to be a str")
-        if contract is not None:
-            warnings.warn("""The setting \"contract\" has been deprecated.""", DeprecationWarning)
-            pulumi.log.warn("""contract is deprecated: The setting \"contract\" has been deprecated.""")
-
         pulumi.set(__self__, "contract", contract)
         if contract_id and not isinstance(contract_id, str):
             raise TypeError("Expected argument 'contract_id' to be a str")
         pulumi.set(__self__, "contract_id", contract_id)
         if group_name and not isinstance(group_name, str):
             raise TypeError("Expected argument 'group_name' to be a str")
         pulumi.set(__self__, "group_name", group_name)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
         if name and not isinstance(name, str):
             raise TypeError("Expected argument 'name' to be a str")
-        if name is not None:
-            warnings.warn("""The setting \"name\" has been deprecated.""", DeprecationWarning)
-            pulumi.log.warn("""name is deprecated: The setting \"name\" has been deprecated.""")
-
         pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def contract(self) -> str:
+        warnings.warn("""The setting \"contract\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""contract is deprecated: The setting \"contract\" has been deprecated.""")
+
         return pulumi.get(self, "contract")
 
     @property
     @pulumi.getter(name="contractId")
     def contract_id(self) -> str:
         return pulumi.get(self, "contract_id")
 
@@ -68,14 +63,17 @@
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def name(self) -> str:
+        warnings.warn("""The setting \"name\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""name is deprecated: The setting \"name\" has been deprecated.""")
+
         return pulumi.get(self, "name")
 
 
 class AwaitableGetGroupResult(GetGroupResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -101,19 +99,19 @@
     __args__['contractId'] = contract_id
     __args__['groupName'] = group_name
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getGroup:getGroup', __args__, opts=opts, typ=GetGroupResult).value
 
     return AwaitableGetGroupResult(
-        contract=__ret__.contract,
-        contract_id=__ret__.contract_id,
-        group_name=__ret__.group_name,
-        id=__ret__.id,
-        name=__ret__.name)
+        contract=pulumi.get(__ret__, 'contract'),
+        contract_id=pulumi.get(__ret__, 'contract_id'),
+        group_name=pulumi.get(__ret__, 'group_name'),
+        id=pulumi.get(__ret__, 'id'),
+        name=pulumi.get(__ret__, 'name'))
 
 
 @_utilities.lift_output_func(get_group)
 def get_group_output(contract: Optional[pulumi.Input[Optional[str]]] = None,
                      contract_id: Optional[pulumi.Input[Optional[str]]] = None,
                      group_name: Optional[pulumi.Input[Optional[str]]] = None,
                      name: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_groups.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_groups.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,9 +58,9 @@
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getGroups:getGroups', __args__, opts=opts, typ=GetGroupsResult).value
 
     return AwaitableGetGroupsResult(
-        groups=__ret__.groups,
-        id=__ret__.id)
+        groups=pulumi.get(__ret__, 'groups'),
+        id=pulumi.get(__ret__, 'id'))
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_gtm_default_datacenter.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_gtm_default_datacenter.py`

 * *Files 9% similar despite different names*

```diff
@@ -89,19 +89,19 @@
     __args__ = dict()
     __args__['datacenter'] = datacenter
     __args__['domain'] = domain
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getGtmDefaultDatacenter:getGtmDefaultDatacenter', __args__, opts=opts, typ=GetGtmDefaultDatacenterResult).value
 
     return AwaitableGetGtmDefaultDatacenterResult(
-        datacenter=__ret__.datacenter,
-        datacenter_id=__ret__.datacenter_id,
-        domain=__ret__.domain,
-        id=__ret__.id,
-        nickname=__ret__.nickname)
+        datacenter=pulumi.get(__ret__, 'datacenter'),
+        datacenter_id=pulumi.get(__ret__, 'datacenter_id'),
+        domain=pulumi.get(__ret__, 'domain'),
+        id=pulumi.get(__ret__, 'id'),
+        nickname=pulumi.get(__ret__, 'nickname'))
 
 
 @_utilities.lift_output_func(get_gtm_default_datacenter)
 def get_gtm_default_datacenter_output(datacenter: Optional[pulumi.Input[Optional[int]]] = None,
                                       domain: Optional[pulumi.Input[str]] = None,
                                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetGtmDefaultDatacenterResult]:
     """
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_iam_contact_types.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_iam_contact_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,9 +57,9 @@
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getIamContactTypes:getIamContactTypes', __args__, opts=opts, typ=GetIamContactTypesResult).value
 
     return AwaitableGetIamContactTypesResult(
-        contact_types=__ret__.contact_types,
-        id=__ret__.id)
+        contact_types=pulumi.get(__ret__, 'contact_types'),
+        id=pulumi.get(__ret__, 'id'))
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_iam_countries.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_iam_countries.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,9 +57,9 @@
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getIamCountries:getIamCountries', __args__, opts=opts, typ=GetIamCountriesResult).value
 
     return AwaitableGetIamCountriesResult(
-        countries=__ret__.countries,
-        id=__ret__.id)
+        countries=pulumi.get(__ret__, 'countries'),
+        id=pulumi.get(__ret__, 'id'))
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_iam_grantable_roles.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_iam_grantable_roles.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,9 +58,9 @@
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getIamGrantableRoles:getIamGrantableRoles', __args__, opts=opts, typ=GetIamGrantableRolesResult).value
 
     return AwaitableGetIamGrantableRolesResult(
-        grantable_roles=__ret__.grantable_roles,
-        id=__ret__.id)
+        grantable_roles=pulumi.get(__ret__, 'grantable_roles'),
+        id=pulumi.get(__ret__, 'id'))
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_iam_roles.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_iam_roles.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,9 +58,9 @@
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getIamRoles:getIamRoles', __args__, opts=opts, typ=GetIamRolesResult).value
 
     return AwaitableGetIamRolesResult(
-        id=__ret__.id,
-        roles=__ret__.roles)
+        id=pulumi.get(__ret__, 'id'),
+        roles=pulumi.get(__ret__, 'roles'))
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_iam_states.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_iam_states.py`

 * *Files 13% similar despite different names*

```diff
@@ -69,17 +69,17 @@
     """
     __args__ = dict()
     __args__['country'] = country
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getIamStates:getIamStates', __args__, opts=opts, typ=GetIamStatesResult).value
 
     return AwaitableGetIamStatesResult(
-        country=__ret__.country,
-        id=__ret__.id,
-        states=__ret__.states)
+        country=pulumi.get(__ret__, 'country'),
+        id=pulumi.get(__ret__, 'id'),
+        states=pulumi.get(__ret__, 'states'))
 
 
 @_utilities.lift_output_func(get_iam_states)
 def get_iam_states_output(country: Optional[pulumi.Input[str]] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetIamStatesResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_iam_supported_langs.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_iam_supported_langs.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,9 +57,9 @@
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getIamSupportedLangs:getIamSupportedLangs', __args__, opts=opts, typ=GetIamSupportedLangsResult).value
 
     return AwaitableGetIamSupportedLangsResult(
-        id=__ret__.id,
-        languages=__ret__.languages)
+        id=pulumi.get(__ret__, 'id'),
+        languages=pulumi.get(__ret__, 'languages'))
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_iam_timeout_policies.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_iam_timeout_policies.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,9 +57,9 @@
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getIamTimeoutPolicies:getIamTimeoutPolicies', __args__, opts=opts, typ=GetIamTimeoutPoliciesResult).value
 
     return AwaitableGetIamTimeoutPoliciesResult(
-        id=__ret__.id,
-        policies=__ret__.policies)
+        id=pulumi.get(__ret__, 'id'),
+        policies=pulumi.get(__ret__, 'policies'))
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_iam_timezones.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_iam_timezones.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,9 +58,9 @@
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getIamTimezones:getIamTimezones', __args__, opts=opts, typ=GetIamTimezonesResult).value
 
     return AwaitableGetIamTimezonesResult(
-        id=__ret__.id,
-        timezones=__ret__.timezones)
+        id=pulumi.get(__ret__, 'id'),
+        timezones=pulumi.get(__ret__, 'timezones'))
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_network_lists.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_network_lists.py`

 * *Files 5% similar despite different names*

```diff
@@ -127,23 +127,23 @@
     __args__['name'] = name
     __args__['networkListId'] = network_list_id
     __args__['type'] = type
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getNetworkLists:getNetworkLists', __args__, opts=opts, typ=GetNetworkListsResult).value
 
     return AwaitableGetNetworkListsResult(
-        contract_id=__ret__.contract_id,
-        group_id=__ret__.group_id,
-        id=__ret__.id,
-        json=__ret__.json,
-        lists=__ret__.lists,
-        name=__ret__.name,
-        network_list_id=__ret__.network_list_id,
-        output_text=__ret__.output_text,
-        type=__ret__.type)
+        contract_id=pulumi.get(__ret__, 'contract_id'),
+        group_id=pulumi.get(__ret__, 'group_id'),
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        lists=pulumi.get(__ret__, 'lists'),
+        name=pulumi.get(__ret__, 'name'),
+        network_list_id=pulumi.get(__ret__, 'network_list_id'),
+        output_text=pulumi.get(__ret__, 'output_text'),
+        type=pulumi.get(__ret__, 'type'))
 
 
 @_utilities.lift_output_func(get_network_lists)
 def get_network_lists_output(name: Optional[pulumi.Input[Optional[str]]] = None,
                              network_list_id: Optional[pulumi.Input[Optional[str]]] = None,
                              type: Optional[pulumi.Input[Optional[str]]] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetNetworkListsResult]:
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_properties.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_properties.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,18 +81,18 @@
     __args__ = dict()
     __args__['contractId'] = contract_id
     __args__['groupId'] = group_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getProperties:getProperties', __args__, opts=opts, typ=GetPropertiesResult).value
 
     return AwaitableGetPropertiesResult(
-        contract_id=__ret__.contract_id,
-        group_id=__ret__.group_id,
-        id=__ret__.id,
-        properties=__ret__.properties)
+        contract_id=pulumi.get(__ret__, 'contract_id'),
+        group_id=pulumi.get(__ret__, 'group_id'),
+        id=pulumi.get(__ret__, 'id'),
+        properties=pulumi.get(__ret__, 'properties'))
 
 
 @_utilities.lift_output_func(get_properties)
 def get_properties_output(contract_id: Optional[pulumi.Input[str]] = None,
                           group_id: Optional[pulumi.Input[str]] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPropertiesResult]:
     """
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_properties_search.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_properties_search.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,18 +81,18 @@
     __args__ = dict()
     __args__['key'] = key
     __args__['value'] = value
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getPropertiesSearch:getPropertiesSearch', __args__, opts=opts, typ=GetPropertiesSearchResult).value
 
     return AwaitableGetPropertiesSearchResult(
-        id=__ret__.id,
-        key=__ret__.key,
-        properties=__ret__.properties,
-        value=__ret__.value)
+        id=pulumi.get(__ret__, 'id'),
+        key=pulumi.get(__ret__, 'key'),
+        properties=pulumi.get(__ret__, 'properties'),
+        value=pulumi.get(__ret__, 'value'))
 
 
 @_utilities.lift_output_func(get_properties_search)
 def get_properties_search_output(key: Optional[pulumi.Input[str]] = None,
                                  value: Optional[pulumi.Input[str]] = None,
                                  opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPropertiesSearchResult]:
     """
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_property.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,18 +80,18 @@
     __args__ = dict()
     __args__['name'] = name
     __args__['version'] = version
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getProperty:getProperty', __args__, opts=opts, typ=GetPropertyResult).value
 
     return AwaitableGetPropertyResult(
-        id=__ret__.id,
-        name=__ret__.name,
-        rules=__ret__.rules,
-        version=__ret__.version)
+        id=pulumi.get(__ret__, 'id'),
+        name=pulumi.get(__ret__, 'name'),
+        rules=pulumi.get(__ret__, 'rules'),
+        version=pulumi.get(__ret__, 'version'))
 
 
 @_utilities.lift_output_func(get_property)
 def get_property_output(name: Optional[pulumi.Input[str]] = None,
                         version: Optional[pulumi.Input[Optional[int]]] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPropertyResult]:
     """
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_activation.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_property_activation.py`

 * *Files 5% similar despite different names*

```diff
@@ -136,24 +136,24 @@
     __args__['network'] = network
     __args__['propertyId'] = property_id
     __args__['version'] = version
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getPropertyActivation:getPropertyActivation', __args__, opts=opts, typ=GetPropertyActivationResult).value
 
     return AwaitableGetPropertyActivationResult(
-        activation_id=__ret__.activation_id,
-        contacts=__ret__.contacts,
-        errors=__ret__.errors,
-        id=__ret__.id,
-        network=__ret__.network,
-        note=__ret__.note,
-        property_id=__ret__.property_id,
-        status=__ret__.status,
-        version=__ret__.version,
-        warnings=__ret__.warnings)
+        activation_id=pulumi.get(__ret__, 'activation_id'),
+        contacts=pulumi.get(__ret__, 'contacts'),
+        errors=pulumi.get(__ret__, 'errors'),
+        id=pulumi.get(__ret__, 'id'),
+        network=pulumi.get(__ret__, 'network'),
+        note=pulumi.get(__ret__, 'note'),
+        property_id=pulumi.get(__ret__, 'property_id'),
+        status=pulumi.get(__ret__, 'status'),
+        version=pulumi.get(__ret__, 'version'),
+        warnings=pulumi.get(__ret__, 'warnings'))
 
 
 @_utilities.lift_output_func(get_property_activation)
 def get_property_activation_output(network: Optional[pulumi.Input[Optional[str]]] = None,
                                    property_id: Optional[pulumi.Input[str]] = None,
                                    version: Optional[pulumi.Input[int]] = None,
                                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPropertyActivationResult]:
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_hostnames.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_property_hostnames.py`

 * *Files 10% similar despite different names*

```diff
@@ -101,20 +101,20 @@
     __args__['contractId'] = contract_id
     __args__['groupId'] = group_id
     __args__['propertyId'] = property_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getPropertyHostnames:getPropertyHostnames', __args__, opts=opts, typ=GetPropertyHostnamesResult).value
 
     return AwaitableGetPropertyHostnamesResult(
-        contract_id=__ret__.contract_id,
-        group_id=__ret__.group_id,
-        hostnames=__ret__.hostnames,
-        id=__ret__.id,
-        property_id=__ret__.property_id,
-        version=__ret__.version)
+        contract_id=pulumi.get(__ret__, 'contract_id'),
+        group_id=pulumi.get(__ret__, 'group_id'),
+        hostnames=pulumi.get(__ret__, 'hostnames'),
+        id=pulumi.get(__ret__, 'id'),
+        property_id=pulumi.get(__ret__, 'property_id'),
+        version=pulumi.get(__ret__, 'version'))
 
 
 @_utilities.lift_output_func(get_property_hostnames)
 def get_property_hostnames_output(contract_id: Optional[pulumi.Input[str]] = None,
                                   group_id: Optional[pulumi.Input[str]] = None,
                                   property_id: Optional[pulumi.Input[str]] = None,
                                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPropertyHostnamesResult]:
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_include.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_property_include_activation.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,53 +6,53 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
-    'GetPropertyIncludeResult',
-    'AwaitableGetPropertyIncludeResult',
-    'get_property_include',
-    'get_property_include_output',
+    'GetPropertyIncludeActivationResult',
+    'AwaitableGetPropertyIncludeActivationResult',
+    'get_property_include_activation',
+    'get_property_include_activation_output',
 ]
 
 @pulumi.output_type
-class GetPropertyIncludeResult:
+class GetPropertyIncludeActivationResult:
     """
-    A collection of values returned by getPropertyInclude.
+    A collection of values returned by getPropertyIncludeActivation.
     """
-    def __init__(__self__, contract_id=None, group_id=None, id=None, include_id=None, latest_version=None, name=None, production_version=None, staging_version=None, type=None):
+    def __init__(__self__, contract_id=None, group_id=None, id=None, include_id=None, name=None, network=None, note=None, notify_emails=None, version=None):
         if contract_id and not isinstance(contract_id, str):
             raise TypeError("Expected argument 'contract_id' to be a str")
         pulumi.set(__self__, "contract_id", contract_id)
         if group_id and not isinstance(group_id, str):
             raise TypeError("Expected argument 'group_id' to be a str")
         pulumi.set(__self__, "group_id", group_id)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
         if include_id and not isinstance(include_id, str):
             raise TypeError("Expected argument 'include_id' to be a str")
         pulumi.set(__self__, "include_id", include_id)
-        if latest_version and not isinstance(latest_version, int):
-            raise TypeError("Expected argument 'latest_version' to be a int")
-        pulumi.set(__self__, "latest_version", latest_version)
         if name and not isinstance(name, str):
             raise TypeError("Expected argument 'name' to be a str")
         pulumi.set(__self__, "name", name)
-        if production_version and not isinstance(production_version, int):
-            raise TypeError("Expected argument 'production_version' to be a int")
-        pulumi.set(__self__, "production_version", production_version)
-        if staging_version and not isinstance(staging_version, int):
-            raise TypeError("Expected argument 'staging_version' to be a int")
-        pulumi.set(__self__, "staging_version", staging_version)
-        if type and not isinstance(type, str):
-            raise TypeError("Expected argument 'type' to be a str")
-        pulumi.set(__self__, "type", type)
+        if network and not isinstance(network, str):
+            raise TypeError("Expected argument 'network' to be a str")
+        pulumi.set(__self__, "network", network)
+        if note and not isinstance(note, str):
+            raise TypeError("Expected argument 'note' to be a str")
+        pulumi.set(__self__, "note", note)
+        if notify_emails and not isinstance(notify_emails, list):
+            raise TypeError("Expected argument 'notify_emails' to be a list")
+        pulumi.set(__self__, "notify_emails", notify_emails)
+        if version and not isinstance(version, str):
+            raise TypeError("Expected argument 'version' to be a str")
+        pulumi.set(__self__, "version", version)
 
     @property
     @pulumi.getter(name="contractId")
     def contract_id(self) -> str:
         return pulumi.get(self, "contract_id")
 
     @property
@@ -70,84 +70,87 @@
 
     @property
     @pulumi.getter(name="includeId")
     def include_id(self) -> str:
         return pulumi.get(self, "include_id")
 
     @property
-    @pulumi.getter(name="latestVersion")
-    def latest_version(self) -> int:
-        return pulumi.get(self, "latest_version")
-
-    @property
     @pulumi.getter
     def name(self) -> str:
         return pulumi.get(self, "name")
 
     @property
-    @pulumi.getter(name="productionVersion")
-    def production_version(self) -> int:
-        return pulumi.get(self, "production_version")
+    @pulumi.getter
+    def network(self) -> str:
+        return pulumi.get(self, "network")
+
+    @property
+    @pulumi.getter
+    def note(self) -> str:
+        return pulumi.get(self, "note")
 
     @property
-    @pulumi.getter(name="stagingVersion")
-    def staging_version(self) -> int:
-        return pulumi.get(self, "staging_version")
+    @pulumi.getter(name="notifyEmails")
+    def notify_emails(self) -> Sequence[str]:
+        return pulumi.get(self, "notify_emails")
 
     @property
     @pulumi.getter
-    def type(self) -> str:
-        return pulumi.get(self, "type")
+    def version(self) -> str:
+        return pulumi.get(self, "version")
 
 
-class AwaitableGetPropertyIncludeResult(GetPropertyIncludeResult):
+class AwaitableGetPropertyIncludeActivationResult(GetPropertyIncludeActivationResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetPropertyIncludeResult(
+        return GetPropertyIncludeActivationResult(
             contract_id=self.contract_id,
             group_id=self.group_id,
             id=self.id,
             include_id=self.include_id,
-            latest_version=self.latest_version,
             name=self.name,
-            production_version=self.production_version,
-            staging_version=self.staging_version,
-            type=self.type)
+            network=self.network,
+            note=self.note,
+            notify_emails=self.notify_emails,
+            version=self.version)
 
 
-def get_property_include(contract_id: Optional[str] = None,
-                         group_id: Optional[str] = None,
-                         include_id: Optional[str] = None,
-                         opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPropertyIncludeResult:
+def get_property_include_activation(contract_id: Optional[str] = None,
+                                    group_id: Optional[str] = None,
+                                    include_id: Optional[str] = None,
+                                    network: Optional[str] = None,
+                                    opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPropertyIncludeActivationResult:
     """
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
     __args__['contractId'] = contract_id
     __args__['groupId'] = group_id
     __args__['includeId'] = include_id
+    __args__['network'] = network
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('akamai:index/getPropertyInclude:getPropertyInclude', __args__, opts=opts, typ=GetPropertyIncludeResult).value
+    __ret__ = pulumi.runtime.invoke('akamai:index/getPropertyIncludeActivation:getPropertyIncludeActivation', __args__, opts=opts, typ=GetPropertyIncludeActivationResult).value
 
-    return AwaitableGetPropertyIncludeResult(
-        contract_id=__ret__.contract_id,
-        group_id=__ret__.group_id,
-        id=__ret__.id,
-        include_id=__ret__.include_id,
-        latest_version=__ret__.latest_version,
-        name=__ret__.name,
-        production_version=__ret__.production_version,
-        staging_version=__ret__.staging_version,
-        type=__ret__.type)
-
-
-@_utilities.lift_output_func(get_property_include)
-def get_property_include_output(contract_id: Optional[pulumi.Input[str]] = None,
-                                group_id: Optional[pulumi.Input[str]] = None,
-                                include_id: Optional[pulumi.Input[str]] = None,
-                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPropertyIncludeResult]:
+    return AwaitableGetPropertyIncludeActivationResult(
+        contract_id=pulumi.get(__ret__, 'contract_id'),
+        group_id=pulumi.get(__ret__, 'group_id'),
+        id=pulumi.get(__ret__, 'id'),
+        include_id=pulumi.get(__ret__, 'include_id'),
+        name=pulumi.get(__ret__, 'name'),
+        network=pulumi.get(__ret__, 'network'),
+        note=pulumi.get(__ret__, 'note'),
+        notify_emails=pulumi.get(__ret__, 'notify_emails'),
+        version=pulumi.get(__ret__, 'version'))
+
+
+@_utilities.lift_output_func(get_property_include_activation)
+def get_property_include_activation_output(contract_id: Optional[pulumi.Input[str]] = None,
+                                           group_id: Optional[pulumi.Input[str]] = None,
+                                           include_id: Optional[pulumi.Input[str]] = None,
+                                           network: Optional[pulumi.Input[str]] = None,
+                                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPropertyIncludeActivationResult]:
     """
     Use this data source to access information about an existing resource.
     """
     ...
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_include_activation.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_property_include_rules.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
-    'GetPropertyIncludeActivationResult',
-    'AwaitableGetPropertyIncludeActivationResult',
-    'get_property_include_activation',
-    'get_property_include_activation_output',
+    'GetPropertyIncludeRulesResult',
+    'AwaitableGetPropertyIncludeRulesResult',
+    'get_property_include_rules',
+    'get_property_include_rules_output',
 ]
 
 @pulumi.output_type
-class GetPropertyIncludeActivationResult:
+class GetPropertyIncludeRulesResult:
     """
-    A collection of values returned by getPropertyIncludeActivation.
+    A collection of values returned by getPropertyIncludeRules.
     """
-    def __init__(__self__, contract_id=None, group_id=None, id=None, include_id=None, name=None, network=None, note=None, notify_emails=None, version=None):
+    def __init__(__self__, contract_id=None, group_id=None, id=None, include_id=None, name=None, rule_errors=None, rule_format=None, rule_warnings=None, rules=None, type=None, version=None):
         if contract_id and not isinstance(contract_id, str):
             raise TypeError("Expected argument 'contract_id' to be a str")
         pulumi.set(__self__, "contract_id", contract_id)
         if group_id and not isinstance(group_id, str):
             raise TypeError("Expected argument 'group_id' to be a str")
         pulumi.set(__self__, "group_id", group_id)
         if id and not isinstance(id, str):
@@ -33,25 +33,31 @@
         pulumi.set(__self__, "id", id)
         if include_id and not isinstance(include_id, str):
             raise TypeError("Expected argument 'include_id' to be a str")
         pulumi.set(__self__, "include_id", include_id)
         if name and not isinstance(name, str):
             raise TypeError("Expected argument 'name' to be a str")
         pulumi.set(__self__, "name", name)
-        if network and not isinstance(network, str):
-            raise TypeError("Expected argument 'network' to be a str")
-        pulumi.set(__self__, "network", network)
-        if note and not isinstance(note, str):
-            raise TypeError("Expected argument 'note' to be a str")
-        pulumi.set(__self__, "note", note)
-        if notify_emails and not isinstance(notify_emails, list):
-            raise TypeError("Expected argument 'notify_emails' to be a list")
-        pulumi.set(__self__, "notify_emails", notify_emails)
-        if version and not isinstance(version, str):
-            raise TypeError("Expected argument 'version' to be a str")
+        if rule_errors and not isinstance(rule_errors, str):
+            raise TypeError("Expected argument 'rule_errors' to be a str")
+        pulumi.set(__self__, "rule_errors", rule_errors)
+        if rule_format and not isinstance(rule_format, str):
+            raise TypeError("Expected argument 'rule_format' to be a str")
+        pulumi.set(__self__, "rule_format", rule_format)
+        if rule_warnings and not isinstance(rule_warnings, str):
+            raise TypeError("Expected argument 'rule_warnings' to be a str")
+        pulumi.set(__self__, "rule_warnings", rule_warnings)
+        if rules and not isinstance(rules, str):
+            raise TypeError("Expected argument 'rules' to be a str")
+        pulumi.set(__self__, "rules", rules)
+        if type and not isinstance(type, str):
+            raise TypeError("Expected argument 'type' to be a str")
+        pulumi.set(__self__, "type", type)
+        if version and not isinstance(version, int):
+            raise TypeError("Expected argument 'version' to be a int")
         pulumi.set(__self__, "version", version)
 
     @property
     @pulumi.getter(name="contractId")
     def contract_id(self) -> str:
         return pulumi.get(self, "contract_id")
 
@@ -75,82 +81,96 @@
 
     @property
     @pulumi.getter
     def name(self) -> str:
         return pulumi.get(self, "name")
 
     @property
-    @pulumi.getter
-    def network(self) -> str:
-        return pulumi.get(self, "network")
+    @pulumi.getter(name="ruleErrors")
+    def rule_errors(self) -> str:
+        return pulumi.get(self, "rule_errors")
+
+    @property
+    @pulumi.getter(name="ruleFormat")
+    def rule_format(self) -> str:
+        return pulumi.get(self, "rule_format")
+
+    @property
+    @pulumi.getter(name="ruleWarnings")
+    def rule_warnings(self) -> str:
+        return pulumi.get(self, "rule_warnings")
 
     @property
     @pulumi.getter
-    def note(self) -> str:
-        return pulumi.get(self, "note")
+    def rules(self) -> str:
+        return pulumi.get(self, "rules")
 
     @property
-    @pulumi.getter(name="notifyEmails")
-    def notify_emails(self) -> Sequence[str]:
-        return pulumi.get(self, "notify_emails")
+    @pulumi.getter
+    def type(self) -> str:
+        return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
-    def version(self) -> str:
+    def version(self) -> int:
         return pulumi.get(self, "version")
 
 
-class AwaitableGetPropertyIncludeActivationResult(GetPropertyIncludeActivationResult):
+class AwaitableGetPropertyIncludeRulesResult(GetPropertyIncludeRulesResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetPropertyIncludeActivationResult(
+        return GetPropertyIncludeRulesResult(
             contract_id=self.contract_id,
             group_id=self.group_id,
             id=self.id,
             include_id=self.include_id,
             name=self.name,
-            network=self.network,
-            note=self.note,
-            notify_emails=self.notify_emails,
+            rule_errors=self.rule_errors,
+            rule_format=self.rule_format,
+            rule_warnings=self.rule_warnings,
+            rules=self.rules,
+            type=self.type,
             version=self.version)
 
 
-def get_property_include_activation(contract_id: Optional[str] = None,
-                                    group_id: Optional[str] = None,
-                                    include_id: Optional[str] = None,
-                                    network: Optional[str] = None,
-                                    opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPropertyIncludeActivationResult:
+def get_property_include_rules(contract_id: Optional[str] = None,
+                               group_id: Optional[str] = None,
+                               include_id: Optional[str] = None,
+                               version: Optional[int] = None,
+                               opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPropertyIncludeRulesResult:
     """
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
     __args__['contractId'] = contract_id
     __args__['groupId'] = group_id
     __args__['includeId'] = include_id
-    __args__['network'] = network
+    __args__['version'] = version
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('akamai:index/getPropertyIncludeActivation:getPropertyIncludeActivation', __args__, opts=opts, typ=GetPropertyIncludeActivationResult).value
+    __ret__ = pulumi.runtime.invoke('akamai:index/getPropertyIncludeRules:getPropertyIncludeRules', __args__, opts=opts, typ=GetPropertyIncludeRulesResult).value
 
-    return AwaitableGetPropertyIncludeActivationResult(
-        contract_id=__ret__.contract_id,
-        group_id=__ret__.group_id,
-        id=__ret__.id,
-        include_id=__ret__.include_id,
-        name=__ret__.name,
-        network=__ret__.network,
-        note=__ret__.note,
-        notify_emails=__ret__.notify_emails,
-        version=__ret__.version)
-
-
-@_utilities.lift_output_func(get_property_include_activation)
-def get_property_include_activation_output(contract_id: Optional[pulumi.Input[str]] = None,
-                                           group_id: Optional[pulumi.Input[str]] = None,
-                                           include_id: Optional[pulumi.Input[str]] = None,
-                                           network: Optional[pulumi.Input[str]] = None,
-                                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPropertyIncludeActivationResult]:
+    return AwaitableGetPropertyIncludeRulesResult(
+        contract_id=pulumi.get(__ret__, 'contract_id'),
+        group_id=pulumi.get(__ret__, 'group_id'),
+        id=pulumi.get(__ret__, 'id'),
+        include_id=pulumi.get(__ret__, 'include_id'),
+        name=pulumi.get(__ret__, 'name'),
+        rule_errors=pulumi.get(__ret__, 'rule_errors'),
+        rule_format=pulumi.get(__ret__, 'rule_format'),
+        rule_warnings=pulumi.get(__ret__, 'rule_warnings'),
+        rules=pulumi.get(__ret__, 'rules'),
+        type=pulumi.get(__ret__, 'type'),
+        version=pulumi.get(__ret__, 'version'))
+
+
+@_utilities.lift_output_func(get_property_include_rules)
+def get_property_include_rules_output(contract_id: Optional[pulumi.Input[str]] = None,
+                                      group_id: Optional[pulumi.Input[str]] = None,
+                                      include_id: Optional[pulumi.Input[str]] = None,
+                                      version: Optional[pulumi.Input[int]] = None,
+                                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPropertyIncludeRulesResult]:
     """
     Use this data source to access information about an existing resource.
     """
     ...
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_include_parents.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_property_include_parents.py`

 * *Files 8% similar despite different names*

```diff
@@ -92,19 +92,19 @@
     __args__['contractId'] = contract_id
     __args__['groupId'] = group_id
     __args__['includeId'] = include_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getPropertyIncludeParents:getPropertyIncludeParents', __args__, opts=opts, typ=GetPropertyIncludeParentsResult).value
 
     return AwaitableGetPropertyIncludeParentsResult(
-        contract_id=__ret__.contract_id,
-        group_id=__ret__.group_id,
-        id=__ret__.id,
-        include_id=__ret__.include_id,
-        parents=__ret__.parents)
+        contract_id=pulumi.get(__ret__, 'contract_id'),
+        group_id=pulumi.get(__ret__, 'group_id'),
+        id=pulumi.get(__ret__, 'id'),
+        include_id=pulumi.get(__ret__, 'include_id'),
+        parents=pulumi.get(__ret__, 'parents'))
 
 
 @_utilities.lift_output_func(get_property_include_parents)
 def get_property_include_parents_output(contract_id: Optional[pulumi.Input[str]] = None,
                                         group_id: Optional[pulumi.Input[str]] = None,
                                         include_id: Optional[pulumi.Input[str]] = None,
                                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPropertyIncludeParentsResult]:
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_include_rules.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_property_rules.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,171 +6,144 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
-    'GetPropertyIncludeRulesResult',
-    'AwaitableGetPropertyIncludeRulesResult',
-    'get_property_include_rules',
-    'get_property_include_rules_output',
+    'GetPropertyRulesResult',
+    'AwaitableGetPropertyRulesResult',
+    'get_property_rules',
+    'get_property_rules_output',
 ]
 
 @pulumi.output_type
-class GetPropertyIncludeRulesResult:
+class GetPropertyRulesResult:
     """
-    A collection of values returned by getPropertyIncludeRules.
+    A collection of values returned by getPropertyRules.
     """
-    def __init__(__self__, contract_id=None, group_id=None, id=None, include_id=None, name=None, rule_errors=None, rule_format=None, rule_warnings=None, rules=None, type=None, version=None):
+    def __init__(__self__, contract_id=None, errors=None, group_id=None, id=None, property_id=None, rule_format=None, rules=None, version=None):
         if contract_id and not isinstance(contract_id, str):
             raise TypeError("Expected argument 'contract_id' to be a str")
         pulumi.set(__self__, "contract_id", contract_id)
+        if errors and not isinstance(errors, str):
+            raise TypeError("Expected argument 'errors' to be a str")
+        pulumi.set(__self__, "errors", errors)
         if group_id and not isinstance(group_id, str):
             raise TypeError("Expected argument 'group_id' to be a str")
         pulumi.set(__self__, "group_id", group_id)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
-        if include_id and not isinstance(include_id, str):
-            raise TypeError("Expected argument 'include_id' to be a str")
-        pulumi.set(__self__, "include_id", include_id)
-        if name and not isinstance(name, str):
-            raise TypeError("Expected argument 'name' to be a str")
-        pulumi.set(__self__, "name", name)
-        if rule_errors and not isinstance(rule_errors, str):
-            raise TypeError("Expected argument 'rule_errors' to be a str")
-        pulumi.set(__self__, "rule_errors", rule_errors)
+        if property_id and not isinstance(property_id, str):
+            raise TypeError("Expected argument 'property_id' to be a str")
+        pulumi.set(__self__, "property_id", property_id)
         if rule_format and not isinstance(rule_format, str):
             raise TypeError("Expected argument 'rule_format' to be a str")
         pulumi.set(__self__, "rule_format", rule_format)
-        if rule_warnings and not isinstance(rule_warnings, str):
-            raise TypeError("Expected argument 'rule_warnings' to be a str")
-        pulumi.set(__self__, "rule_warnings", rule_warnings)
         if rules and not isinstance(rules, str):
             raise TypeError("Expected argument 'rules' to be a str")
         pulumi.set(__self__, "rules", rules)
-        if type and not isinstance(type, str):
-            raise TypeError("Expected argument 'type' to be a str")
-        pulumi.set(__self__, "type", type)
         if version and not isinstance(version, int):
             raise TypeError("Expected argument 'version' to be a int")
         pulumi.set(__self__, "version", version)
 
     @property
     @pulumi.getter(name="contractId")
     def contract_id(self) -> str:
         return pulumi.get(self, "contract_id")
 
     @property
+    @pulumi.getter
+    def errors(self) -> str:
+        return pulumi.get(self, "errors")
+
+    @property
     @pulumi.getter(name="groupId")
     def group_id(self) -> str:
         return pulumi.get(self, "group_id")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
-    @pulumi.getter(name="includeId")
-    def include_id(self) -> str:
-        return pulumi.get(self, "include_id")
-
-    @property
-    @pulumi.getter
-    def name(self) -> str:
-        return pulumi.get(self, "name")
-
-    @property
-    @pulumi.getter(name="ruleErrors")
-    def rule_errors(self) -> str:
-        return pulumi.get(self, "rule_errors")
+    @pulumi.getter(name="propertyId")
+    def property_id(self) -> str:
+        return pulumi.get(self, "property_id")
 
     @property
     @pulumi.getter(name="ruleFormat")
-    def rule_format(self) -> str:
+    def rule_format(self) -> Optional[str]:
         return pulumi.get(self, "rule_format")
 
     @property
-    @pulumi.getter(name="ruleWarnings")
-    def rule_warnings(self) -> str:
-        return pulumi.get(self, "rule_warnings")
-
-    @property
     @pulumi.getter
     def rules(self) -> str:
         return pulumi.get(self, "rules")
 
     @property
     @pulumi.getter
-    def type(self) -> str:
-        return pulumi.get(self, "type")
-
-    @property
-    @pulumi.getter
     def version(self) -> int:
         return pulumi.get(self, "version")
 
 
-class AwaitableGetPropertyIncludeRulesResult(GetPropertyIncludeRulesResult):
+class AwaitableGetPropertyRulesResult(GetPropertyRulesResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetPropertyIncludeRulesResult(
+        return GetPropertyRulesResult(
             contract_id=self.contract_id,
+            errors=self.errors,
             group_id=self.group_id,
             id=self.id,
-            include_id=self.include_id,
-            name=self.name,
-            rule_errors=self.rule_errors,
+            property_id=self.property_id,
             rule_format=self.rule_format,
-            rule_warnings=self.rule_warnings,
             rules=self.rules,
-            type=self.type,
             version=self.version)
 
 
-def get_property_include_rules(contract_id: Optional[str] = None,
-                               group_id: Optional[str] = None,
-                               include_id: Optional[str] = None,
-                               version: Optional[int] = None,
-                               opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPropertyIncludeRulesResult:
+def get_property_rules(contract_id: Optional[str] = None,
+                       group_id: Optional[str] = None,
+                       property_id: Optional[str] = None,
+                       rule_format: Optional[str] = None,
+                       version: Optional[int] = None,
+                       opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPropertyRulesResult:
     """
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
     __args__['contractId'] = contract_id
     __args__['groupId'] = group_id
-    __args__['includeId'] = include_id
+    __args__['propertyId'] = property_id
+    __args__['ruleFormat'] = rule_format
     __args__['version'] = version
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('akamai:index/getPropertyIncludeRules:getPropertyIncludeRules', __args__, opts=opts, typ=GetPropertyIncludeRulesResult).value
+    __ret__ = pulumi.runtime.invoke('akamai:index/getPropertyRules:getPropertyRules', __args__, opts=opts, typ=GetPropertyRulesResult).value
 
-    return AwaitableGetPropertyIncludeRulesResult(
-        contract_id=__ret__.contract_id,
-        group_id=__ret__.group_id,
-        id=__ret__.id,
-        include_id=__ret__.include_id,
-        name=__ret__.name,
-        rule_errors=__ret__.rule_errors,
-        rule_format=__ret__.rule_format,
-        rule_warnings=__ret__.rule_warnings,
-        rules=__ret__.rules,
-        type=__ret__.type,
-        version=__ret__.version)
-
-
-@_utilities.lift_output_func(get_property_include_rules)
-def get_property_include_rules_output(contract_id: Optional[pulumi.Input[str]] = None,
-                                      group_id: Optional[pulumi.Input[str]] = None,
-                                      include_id: Optional[pulumi.Input[str]] = None,
-                                      version: Optional[pulumi.Input[int]] = None,
-                                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPropertyIncludeRulesResult]:
+    return AwaitableGetPropertyRulesResult(
+        contract_id=pulumi.get(__ret__, 'contract_id'),
+        errors=pulumi.get(__ret__, 'errors'),
+        group_id=pulumi.get(__ret__, 'group_id'),
+        id=pulumi.get(__ret__, 'id'),
+        property_id=pulumi.get(__ret__, 'property_id'),
+        rule_format=pulumi.get(__ret__, 'rule_format'),
+        rules=pulumi.get(__ret__, 'rules'),
+        version=pulumi.get(__ret__, 'version'))
+
+
+@_utilities.lift_output_func(get_property_rules)
+def get_property_rules_output(contract_id: Optional[pulumi.Input[Optional[str]]] = None,
+                              group_id: Optional[pulumi.Input[Optional[str]]] = None,
+                              property_id: Optional[pulumi.Input[str]] = None,
+                              rule_format: Optional[pulumi.Input[Optional[str]]] = None,
+                              version: Optional[pulumi.Input[Optional[int]]] = None,
+                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPropertyRulesResult]:
     """
     Use this data source to access information about an existing resource.
     """
     ...
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_includes.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_property_includes.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,20 +104,20 @@
     __args__['groupId'] = group_id
     __args__['parentProperty'] = parent_property
     __args__['type'] = type
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getPropertyIncludes:getPropertyIncludes', __args__, opts=opts, typ=GetPropertyIncludesResult).value
 
     return AwaitableGetPropertyIncludesResult(
-        contract_id=__ret__.contract_id,
-        group_id=__ret__.group_id,
-        id=__ret__.id,
-        includes=__ret__.includes,
-        parent_property=__ret__.parent_property,
-        type=__ret__.type)
+        contract_id=pulumi.get(__ret__, 'contract_id'),
+        group_id=pulumi.get(__ret__, 'group_id'),
+        id=pulumi.get(__ret__, 'id'),
+        includes=pulumi.get(__ret__, 'includes'),
+        parent_property=pulumi.get(__ret__, 'parent_property'),
+        type=pulumi.get(__ret__, 'type'))
 
 
 @_utilities.lift_output_func(get_property_includes)
 def get_property_includes_output(contract_id: Optional[pulumi.Input[str]] = None,
                                  group_id: Optional[pulumi.Input[str]] = None,
                                  parent_property: Optional[pulumi.Input[Optional[pulumi.InputType['GetPropertyIncludesParentPropertyArgs']]]] = None,
                                  type: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_products.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_property_products.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,17 +70,17 @@
     """
     __args__ = dict()
     __args__['contractId'] = contract_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getPropertyProducts:getPropertyProducts', __args__, opts=opts, typ=GetPropertyProductsResult).value
 
     return AwaitableGetPropertyProductsResult(
-        contract_id=__ret__.contract_id,
-        id=__ret__.id,
-        products=__ret__.products)
+        contract_id=pulumi.get(__ret__, 'contract_id'),
+        id=pulumi.get(__ret__, 'id'),
+        products=pulumi.get(__ret__, 'products'))
 
 
 @_utilities.lift_output_func(get_property_products)
 def get_property_products_output(contract_id: Optional[pulumi.Input[str]] = None,
                                  opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPropertyProductsResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_rule_formats.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_property_rule_formats.py`

 * *Files 12% similar despite different names*

```diff
@@ -57,9 +57,9 @@
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getPropertyRuleFormats:getPropertyRuleFormats', __args__, opts=opts, typ=GetPropertyRuleFormatsResult).value
 
     return AwaitableGetPropertyRuleFormatsResult(
-        id=__ret__.id,
-        rule_formats=__ret__.rule_formats)
+        id=pulumi.get(__ret__, 'id'),
+        rule_formats=pulumi.get(__ret__, 'rule_formats'))
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_rules.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/properties/get_property_rules.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,23 +3,25 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from . import _utilities
+from .. import _utilities
 
 __all__ = [
     'GetPropertyRulesResult',
     'AwaitableGetPropertyRulesResult',
     'get_property_rules',
     'get_property_rules_output',
 ]
 
+warnings.warn("""akamai.properties/getpropertyrules.getPropertyRules has been deprecated in favor of akamai.index/getpropertyrules.getPropertyRules""", DeprecationWarning)
+
 @pulumi.output_type
 class GetPropertyRulesResult:
     """
     A collection of values returned by getPropertyRules.
     """
     def __init__(__self__, contract_id=None, errors=None, group_id=None, id=None, property_id=None, rule_format=None, rules=None, version=None):
         if contract_id and not isinstance(contract_id, str):
@@ -112,38 +114,40 @@
                        property_id: Optional[str] = None,
                        rule_format: Optional[str] = None,
                        version: Optional[int] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPropertyRulesResult:
     """
     Use this data source to access information about an existing resource.
     """
+    pulumi.log.warn("""get_property_rules is deprecated: akamai.properties/getpropertyrules.getPropertyRules has been deprecated in favor of akamai.index/getpropertyrules.getPropertyRules""")
     __args__ = dict()
     __args__['contractId'] = contract_id
     __args__['groupId'] = group_id
     __args__['propertyId'] = property_id
     __args__['ruleFormat'] = rule_format
     __args__['version'] = version
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('akamai:index/getPropertyRules:getPropertyRules', __args__, opts=opts, typ=GetPropertyRulesResult).value
+    __ret__ = pulumi.runtime.invoke('akamai:properties/getPropertyRules:getPropertyRules', __args__, opts=opts, typ=GetPropertyRulesResult).value
 
     return AwaitableGetPropertyRulesResult(
-        contract_id=__ret__.contract_id,
-        errors=__ret__.errors,
-        group_id=__ret__.group_id,
-        id=__ret__.id,
-        property_id=__ret__.property_id,
-        rule_format=__ret__.rule_format,
-        rules=__ret__.rules,
-        version=__ret__.version)
+        contract_id=pulumi.get(__ret__, 'contract_id'),
+        errors=pulumi.get(__ret__, 'errors'),
+        group_id=pulumi.get(__ret__, 'group_id'),
+        id=pulumi.get(__ret__, 'id'),
+        property_id=pulumi.get(__ret__, 'property_id'),
+        rule_format=pulumi.get(__ret__, 'rule_format'),
+        rules=pulumi.get(__ret__, 'rules'),
+        version=pulumi.get(__ret__, 'version'))
 
 
 @_utilities.lift_output_func(get_property_rules)
 def get_property_rules_output(contract_id: Optional[pulumi.Input[Optional[str]]] = None,
                               group_id: Optional[pulumi.Input[Optional[str]]] = None,
                               property_id: Optional[pulumi.Input[str]] = None,
                               rule_format: Optional[pulumi.Input[Optional[str]]] = None,
                               version: Optional[pulumi.Input[Optional[int]]] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPropertyRulesResult]:
     """
     Use this data source to access information about an existing resource.
     """
+    pulumi.log.warn("""get_property_rules is deprecated: akamai.properties/getpropertyrules.getPropertyRules has been deprecated in favor of akamai.index/getpropertyrules.getPropertyRules""")
     ...
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_rules_builder.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_property_rules_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,18 +80,18 @@
     """
     __args__ = dict()
     __args__['rulesV20230105'] = rules_v20230105
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getPropertyRulesBuilder:getPropertyRulesBuilder', __args__, opts=opts, typ=GetPropertyRulesBuilderResult).value
 
     return AwaitableGetPropertyRulesBuilderResult(
-        id=__ret__.id,
-        json=__ret__.json,
-        rule_format=__ret__.rule_format,
-        rules_v20230105=__ret__.rules_v20230105)
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        rule_format=pulumi.get(__ret__, 'rule_format'),
+        rules_v20230105=pulumi.get(__ret__, 'rules_v20230105'))
 
 
 @_utilities.lift_output_func(get_property_rules_builder)
 def get_property_rules_builder_output(rules_v20230105: Optional[pulumi.Input[Optional[pulumi.InputType['GetPropertyRulesBuilderRulesV20230105Args']]]] = None,
                                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPropertyRulesBuilderResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_rules_template.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_property_rules_template.py`

 * *Files 10% similar despite different names*

```diff
@@ -115,21 +115,21 @@
     __args__['varDefinitionFile'] = var_definition_file
     __args__['varValuesFile'] = var_values_file
     __args__['variables'] = variables
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:index/getPropertyRulesTemplate:getPropertyRulesTemplate', __args__, opts=opts, typ=GetPropertyRulesTemplateResult).value
 
     return AwaitableGetPropertyRulesTemplateResult(
-        id=__ret__.id,
-        json=__ret__.json,
-        template_file=__ret__.template_file,
-        templates=__ret__.templates,
-        var_definition_file=__ret__.var_definition_file,
-        var_values_file=__ret__.var_values_file,
-        variables=__ret__.variables)
+        id=pulumi.get(__ret__, 'id'),
+        json=pulumi.get(__ret__, 'json'),
+        template_file=pulumi.get(__ret__, 'template_file'),
+        templates=pulumi.get(__ret__, 'templates'),
+        var_definition_file=pulumi.get(__ret__, 'var_definition_file'),
+        var_values_file=pulumi.get(__ret__, 'var_values_file'),
+        variables=pulumi.get(__ret__, 'variables'))
 
 
 @_utilities.lift_output_func(get_property_rules_template)
 def get_property_rules_template_output(template_file: Optional[pulumi.Input[Optional[str]]] = None,
                                        templates: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetPropertyRulesTemplateTemplateArgs']]]]] = None,
                                        var_definition_file: Optional[pulumi.Input[Optional[str]]] = None,
                                        var_values_file: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/gtm_asmap.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/gtm_asmap.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/gtm_cidrmap.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/gtm_cidrmap.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/gtm_datacenter.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/gtm_datacenter.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/gtm_domain.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/gtm_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/gtm_geomap.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/gtm_geomap.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/gtm_property.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/gtm_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/gtm_resource.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/property_activation.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,607 +7,605 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from ._inputs import *
 
-__all__ = ['GtmResourceArgs', 'GtmResource']
+__all__ = ['PropertyActivationArgs', 'PropertyActivation']
 
 @pulumi.input_type
-class GtmResourceArgs:
+class PropertyActivationArgs:
     def __init__(__self__, *,
-                 aggregation_type: pulumi.Input[str],
-                 domain: pulumi.Input[str],
-                 type: pulumi.Input[str],
-                 constrained_property: Optional[pulumi.Input[str]] = None,
-                 decay_rate: Optional[pulumi.Input[float]] = None,
-                 description: Optional[pulumi.Input[str]] = None,
-                 host_header: Optional[pulumi.Input[str]] = None,
-                 leader_string: Optional[pulumi.Input[str]] = None,
-                 least_squares_decay: Optional[pulumi.Input[float]] = None,
-                 load_imbalance_percentage: Optional[pulumi.Input[float]] = None,
-                 max_u_multiplicative_increment: Optional[pulumi.Input[float]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 resource_instances: Optional[pulumi.Input[Sequence[pulumi.Input['GtmResourceResourceInstanceArgs']]]] = None,
-                 upper_bound: Optional[pulumi.Input[int]] = None,
-                 wait_on_complete: Optional[pulumi.Input[bool]] = None):
+                 contacts: pulumi.Input[Sequence[pulumi.Input[str]]],
+                 version: pulumi.Input[int],
+                 activation_id: Optional[pulumi.Input[str]] = None,
+                 auto_acknowledge_rule_warnings: Optional[pulumi.Input[bool]] = None,
+                 compliance_record: Optional[pulumi.Input['PropertyActivationComplianceRecordArgs']] = None,
+                 network: Optional[pulumi.Input[str]] = None,
+                 note: Optional[pulumi.Input[str]] = None,
+                 property: Optional[pulumi.Input[str]] = None,
+                 property_id: Optional[pulumi.Input[str]] = None,
+                 rule_errors: Optional[pulumi.Input[Sequence[pulumi.Input['PropertyActivationRuleErrorArgs']]]] = None,
+                 rule_warnings: Optional[pulumi.Input[Sequence[pulumi.Input['PropertyActivationRuleWarningArgs']]]] = None):
         """
-        The set of arguments for constructing a GtmResource resource.
+        The set of arguments for constructing a PropertyActivation resource.
+        :param pulumi.Input[bool] auto_acknowledge_rule_warnings: automatically acknowledge all rule warnings for activation to continue. default is true
+        :param pulumi.Input['PropertyActivationComplianceRecordArgs'] compliance_record: Provides an audit record when activating on a production network
+        :param pulumi.Input[str] note: assigns a log message to the activation request
         """
-        pulumi.set(__self__, "aggregation_type", aggregation_type)
-        pulumi.set(__self__, "domain", domain)
-        pulumi.set(__self__, "type", type)
-        if constrained_property is not None:
-            pulumi.set(__self__, "constrained_property", constrained_property)
-        if decay_rate is not None:
-            pulumi.set(__self__, "decay_rate", decay_rate)
-        if description is not None:
-            pulumi.set(__self__, "description", description)
-        if host_header is not None:
-            pulumi.set(__self__, "host_header", host_header)
-        if leader_string is not None:
-            pulumi.set(__self__, "leader_string", leader_string)
-        if least_squares_decay is not None:
-            pulumi.set(__self__, "least_squares_decay", least_squares_decay)
-        if load_imbalance_percentage is not None:
-            pulumi.set(__self__, "load_imbalance_percentage", load_imbalance_percentage)
-        if max_u_multiplicative_increment is not None:
-            pulumi.set(__self__, "max_u_multiplicative_increment", max_u_multiplicative_increment)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
-        if resource_instances is not None:
-            pulumi.set(__self__, "resource_instances", resource_instances)
-        if upper_bound is not None:
-            pulumi.set(__self__, "upper_bound", upper_bound)
-        if wait_on_complete is not None:
-            pulumi.set(__self__, "wait_on_complete", wait_on_complete)
-
-    @property
-    @pulumi.getter(name="aggregationType")
-    def aggregation_type(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "aggregation_type")
-
-    @aggregation_type.setter
-    def aggregation_type(self, value: pulumi.Input[str]):
-        pulumi.set(self, "aggregation_type", value)
+        pulumi.set(__self__, "contacts", contacts)
+        pulumi.set(__self__, "version", version)
+        if activation_id is not None:
+            pulumi.set(__self__, "activation_id", activation_id)
+        if auto_acknowledge_rule_warnings is not None:
+            pulumi.set(__self__, "auto_acknowledge_rule_warnings", auto_acknowledge_rule_warnings)
+        if compliance_record is not None:
+            pulumi.set(__self__, "compliance_record", compliance_record)
+        if network is not None:
+            pulumi.set(__self__, "network", network)
+        if note is not None:
+            pulumi.set(__self__, "note", note)
+        if property is not None:
+            warnings.warn("""The setting \"property\" has been deprecated.""", DeprecationWarning)
+            pulumi.log.warn("""property is deprecated: The setting \"property\" has been deprecated.""")
+        if property is not None:
+            pulumi.set(__self__, "property", property)
+        if property_id is not None:
+            pulumi.set(__self__, "property_id", property_id)
+        if rule_errors is not None:
+            pulumi.set(__self__, "rule_errors", rule_errors)
+        if rule_warnings is not None:
+            warnings.warn("""Rule warnings will not be set in state anymore""", DeprecationWarning)
+            pulumi.log.warn("""rule_warnings is deprecated: Rule warnings will not be set in state anymore""")
+        if rule_warnings is not None:
+            pulumi.set(__self__, "rule_warnings", rule_warnings)
 
     @property
     @pulumi.getter
-    def domain(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "domain")
-
-    @domain.setter
-    def domain(self, value: pulumi.Input[str]):
-        pulumi.set(self, "domain", value)
+    def contacts(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
+        return pulumi.get(self, "contacts")
+
+    @contacts.setter
+    def contacts(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
+        pulumi.set(self, "contacts", value)
 
     @property
     @pulumi.getter
-    def type(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "type")
-
-    @type.setter
-    def type(self, value: pulumi.Input[str]):
-        pulumi.set(self, "type", value)
+    def version(self) -> pulumi.Input[int]:
+        return pulumi.get(self, "version")
+
+    @version.setter
+    def version(self, value: pulumi.Input[int]):
+        pulumi.set(self, "version", value)
+
+    @property
+    @pulumi.getter(name="activationId")
+    def activation_id(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "activation_id")
+
+    @activation_id.setter
+    def activation_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "activation_id", value)
 
     @property
-    @pulumi.getter(name="constrainedProperty")
-    def constrained_property(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "constrained_property")
+    @pulumi.getter(name="autoAcknowledgeRuleWarnings")
+    def auto_acknowledge_rule_warnings(self) -> Optional[pulumi.Input[bool]]:
+        """
+        automatically acknowledge all rule warnings for activation to continue. default is true
+        """
+        return pulumi.get(self, "auto_acknowledge_rule_warnings")
 
-    @constrained_property.setter
-    def constrained_property(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "constrained_property", value)
+    @auto_acknowledge_rule_warnings.setter
+    def auto_acknowledge_rule_warnings(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "auto_acknowledge_rule_warnings", value)
 
     @property
-    @pulumi.getter(name="decayRate")
-    def decay_rate(self) -> Optional[pulumi.Input[float]]:
-        return pulumi.get(self, "decay_rate")
+    @pulumi.getter(name="complianceRecord")
+    def compliance_record(self) -> Optional[pulumi.Input['PropertyActivationComplianceRecordArgs']]:
+        """
+        Provides an audit record when activating on a production network
+        """
+        return pulumi.get(self, "compliance_record")
 
-    @decay_rate.setter
-    def decay_rate(self, value: Optional[pulumi.Input[float]]):
-        pulumi.set(self, "decay_rate", value)
+    @compliance_record.setter
+    def compliance_record(self, value: Optional[pulumi.Input['PropertyActivationComplianceRecordArgs']]):
+        pulumi.set(self, "compliance_record", value)
 
     @property
     @pulumi.getter
-    def description(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "description")
+    def network(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "network")
 
-    @description.setter
-    def description(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "description", value)
+    @network.setter
+    def network(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "network", value)
 
     @property
-    @pulumi.getter(name="hostHeader")
-    def host_header(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "host_header")
+    @pulumi.getter
+    def note(self) -> Optional[pulumi.Input[str]]:
+        """
+        assigns a log message to the activation request
+        """
+        return pulumi.get(self, "note")
 
-    @host_header.setter
-    def host_header(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "host_header", value)
+    @note.setter
+    def note(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "note", value)
 
     @property
-    @pulumi.getter(name="leaderString")
-    def leader_string(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "leader_string")
+    @pulumi.getter(name="propertyId")
+    def property_id(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "property_id")
 
-    @leader_string.setter
-    def leader_string(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "leader_string", value)
+    @property_id.setter
+    def property_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "property_id", value)
 
     @property
-    @pulumi.getter(name="leastSquaresDecay")
-    def least_squares_decay(self) -> Optional[pulumi.Input[float]]:
-        return pulumi.get(self, "least_squares_decay")
+    @pulumi.getter(name="ruleErrors")
+    def rule_errors(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PropertyActivationRuleErrorArgs']]]]:
+        return pulumi.get(self, "rule_errors")
 
-    @least_squares_decay.setter
-    def least_squares_decay(self, value: Optional[pulumi.Input[float]]):
-        pulumi.set(self, "least_squares_decay", value)
+    @rule_errors.setter
+    def rule_errors(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PropertyActivationRuleErrorArgs']]]]):
+        pulumi.set(self, "rule_errors", value)
 
     @property
-    @pulumi.getter(name="loadImbalancePercentage")
-    def load_imbalance_percentage(self) -> Optional[pulumi.Input[float]]:
-        return pulumi.get(self, "load_imbalance_percentage")
+    @pulumi.getter(name="ruleWarnings")
+    def rule_warnings(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PropertyActivationRuleWarningArgs']]]]:
+        warnings.warn("""Rule warnings will not be set in state anymore""", DeprecationWarning)
+        pulumi.log.warn("""rule_warnings is deprecated: Rule warnings will not be set in state anymore""")
 
-    @load_imbalance_percentage.setter
-    def load_imbalance_percentage(self, value: Optional[pulumi.Input[float]]):
-        pulumi.set(self, "load_imbalance_percentage", value)
+        return pulumi.get(self, "rule_warnings")
 
-    @property
-    @pulumi.getter(name="maxUMultiplicativeIncrement")
-    def max_u_multiplicative_increment(self) -> Optional[pulumi.Input[float]]:
-        return pulumi.get(self, "max_u_multiplicative_increment")
-
-    @max_u_multiplicative_increment.setter
-    def max_u_multiplicative_increment(self, value: Optional[pulumi.Input[float]]):
-        pulumi.set(self, "max_u_multiplicative_increment", value)
+    @rule_warnings.setter
+    def rule_warnings(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PropertyActivationRuleWarningArgs']]]]):
+        pulumi.set(self, "rule_warnings", value)
 
     @property
     @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
-
-    @property
-    @pulumi.getter(name="resourceInstances")
-    def resource_instances(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['GtmResourceResourceInstanceArgs']]]]:
-        return pulumi.get(self, "resource_instances")
-
-    @resource_instances.setter
-    def resource_instances(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['GtmResourceResourceInstanceArgs']]]]):
-        pulumi.set(self, "resource_instances", value)
+    def property(self) -> Optional[pulumi.Input[str]]:
+        warnings.warn("""The setting \"property\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""property is deprecated: The setting \"property\" has been deprecated.""")
 
-    @property
-    @pulumi.getter(name="upperBound")
-    def upper_bound(self) -> Optional[pulumi.Input[int]]:
-        return pulumi.get(self, "upper_bound")
-
-    @upper_bound.setter
-    def upper_bound(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "upper_bound", value)
-
-    @property
-    @pulumi.getter(name="waitOnComplete")
-    def wait_on_complete(self) -> Optional[pulumi.Input[bool]]:
-        return pulumi.get(self, "wait_on_complete")
+        return pulumi.get(self, "property")
 
-    @wait_on_complete.setter
-    def wait_on_complete(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "wait_on_complete", value)
+    @property.setter
+    def property(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "property", value)
 
 
 @pulumi.input_type
-class _GtmResourceState:
+class _PropertyActivationState:
     def __init__(__self__, *,
-                 aggregation_type: Optional[pulumi.Input[str]] = None,
-                 constrained_property: Optional[pulumi.Input[str]] = None,
-                 decay_rate: Optional[pulumi.Input[float]] = None,
-                 description: Optional[pulumi.Input[str]] = None,
-                 domain: Optional[pulumi.Input[str]] = None,
-                 host_header: Optional[pulumi.Input[str]] = None,
-                 leader_string: Optional[pulumi.Input[str]] = None,
-                 least_squares_decay: Optional[pulumi.Input[float]] = None,
-                 load_imbalance_percentage: Optional[pulumi.Input[float]] = None,
-                 max_u_multiplicative_increment: Optional[pulumi.Input[float]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 resource_instances: Optional[pulumi.Input[Sequence[pulumi.Input['GtmResourceResourceInstanceArgs']]]] = None,
-                 type: Optional[pulumi.Input[str]] = None,
-                 upper_bound: Optional[pulumi.Input[int]] = None,
-                 wait_on_complete: Optional[pulumi.Input[bool]] = None):
+                 activation_id: Optional[pulumi.Input[str]] = None,
+                 auto_acknowledge_rule_warnings: Optional[pulumi.Input[bool]] = None,
+                 compliance_record: Optional[pulumi.Input['PropertyActivationComplianceRecordArgs']] = None,
+                 contacts: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 errors: Optional[pulumi.Input[str]] = None,
+                 network: Optional[pulumi.Input[str]] = None,
+                 note: Optional[pulumi.Input[str]] = None,
+                 property: Optional[pulumi.Input[str]] = None,
+                 property_id: Optional[pulumi.Input[str]] = None,
+                 rule_errors: Optional[pulumi.Input[Sequence[pulumi.Input['PropertyActivationRuleErrorArgs']]]] = None,
+                 rule_warnings: Optional[pulumi.Input[Sequence[pulumi.Input['PropertyActivationRuleWarningArgs']]]] = None,
+                 status: Optional[pulumi.Input[str]] = None,
+                 version: Optional[pulumi.Input[int]] = None,
+                 warnings: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering GtmResource resources.
+        Input properties used for looking up and filtering PropertyActivation resources.
+        :param pulumi.Input[bool] auto_acknowledge_rule_warnings: automatically acknowledge all rule warnings for activation to continue. default is true
+        :param pulumi.Input['PropertyActivationComplianceRecordArgs'] compliance_record: Provides an audit record when activating on a production network
+        :param pulumi.Input[str] note: assigns a log message to the activation request
         """
-        if aggregation_type is not None:
-            pulumi.set(__self__, "aggregation_type", aggregation_type)
-        if constrained_property is not None:
-            pulumi.set(__self__, "constrained_property", constrained_property)
-        if decay_rate is not None:
-            pulumi.set(__self__, "decay_rate", decay_rate)
-        if description is not None:
-            pulumi.set(__self__, "description", description)
-        if domain is not None:
-            pulumi.set(__self__, "domain", domain)
-        if host_header is not None:
-            pulumi.set(__self__, "host_header", host_header)
-        if leader_string is not None:
-            pulumi.set(__self__, "leader_string", leader_string)
-        if least_squares_decay is not None:
-            pulumi.set(__self__, "least_squares_decay", least_squares_decay)
-        if load_imbalance_percentage is not None:
-            pulumi.set(__self__, "load_imbalance_percentage", load_imbalance_percentage)
-        if max_u_multiplicative_increment is not None:
-            pulumi.set(__self__, "max_u_multiplicative_increment", max_u_multiplicative_increment)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
-        if resource_instances is not None:
-            pulumi.set(__self__, "resource_instances", resource_instances)
-        if type is not None:
-            pulumi.set(__self__, "type", type)
-        if upper_bound is not None:
-            pulumi.set(__self__, "upper_bound", upper_bound)
-        if wait_on_complete is not None:
-            pulumi.set(__self__, "wait_on_complete", wait_on_complete)
+        if activation_id is not None:
+            pulumi.set(__self__, "activation_id", activation_id)
+        if auto_acknowledge_rule_warnings is not None:
+            pulumi.set(__self__, "auto_acknowledge_rule_warnings", auto_acknowledge_rule_warnings)
+        if compliance_record is not None:
+            pulumi.set(__self__, "compliance_record", compliance_record)
+        if contacts is not None:
+            pulumi.set(__self__, "contacts", contacts)
+        if errors is not None:
+            pulumi.set(__self__, "errors", errors)
+        if network is not None:
+            pulumi.set(__self__, "network", network)
+        if note is not None:
+            pulumi.set(__self__, "note", note)
+        if property is not None:
+            warnings.warn("""The setting \"property\" has been deprecated.""", DeprecationWarning)
+            pulumi.log.warn("""property is deprecated: The setting \"property\" has been deprecated.""")
+        if property is not None:
+            pulumi.set(__self__, "property", property)
+        if property_id is not None:
+            pulumi.set(__self__, "property_id", property_id)
+        if rule_errors is not None:
+            pulumi.set(__self__, "rule_errors", rule_errors)
+        if rule_warnings is not None:
+            warnings.warn("""Rule warnings will not be set in state anymore""", DeprecationWarning)
+            pulumi.log.warn("""rule_warnings is deprecated: Rule warnings will not be set in state anymore""")
+        if rule_warnings is not None:
+            pulumi.set(__self__, "rule_warnings", rule_warnings)
+        if status is not None:
+            pulumi.set(__self__, "status", status)
+        if version is not None:
+            pulumi.set(__self__, "version", version)
+        if warnings is not None:
+            pulumi.set(__self__, "warnings", warnings)
+
+    @property
+    @pulumi.getter(name="activationId")
+    def activation_id(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "activation_id")
+
+    @activation_id.setter
+    def activation_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "activation_id", value)
 
     @property
-    @pulumi.getter(name="aggregationType")
-    def aggregation_type(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "aggregation_type")
+    @pulumi.getter(name="autoAcknowledgeRuleWarnings")
+    def auto_acknowledge_rule_warnings(self) -> Optional[pulumi.Input[bool]]:
+        """
+        automatically acknowledge all rule warnings for activation to continue. default is true
+        """
+        return pulumi.get(self, "auto_acknowledge_rule_warnings")
 
-    @aggregation_type.setter
-    def aggregation_type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "aggregation_type", value)
+    @auto_acknowledge_rule_warnings.setter
+    def auto_acknowledge_rule_warnings(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "auto_acknowledge_rule_warnings", value)
 
     @property
-    @pulumi.getter(name="constrainedProperty")
-    def constrained_property(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "constrained_property")
+    @pulumi.getter(name="complianceRecord")
+    def compliance_record(self) -> Optional[pulumi.Input['PropertyActivationComplianceRecordArgs']]:
+        """
+        Provides an audit record when activating on a production network
+        """
+        return pulumi.get(self, "compliance_record")
 
-    @constrained_property.setter
-    def constrained_property(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "constrained_property", value)
+    @compliance_record.setter
+    def compliance_record(self, value: Optional[pulumi.Input['PropertyActivationComplianceRecordArgs']]):
+        pulumi.set(self, "compliance_record", value)
 
     @property
-    @pulumi.getter(name="decayRate")
-    def decay_rate(self) -> Optional[pulumi.Input[float]]:
-        return pulumi.get(self, "decay_rate")
+    @pulumi.getter
+    def contacts(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        return pulumi.get(self, "contacts")
 
-    @decay_rate.setter
-    def decay_rate(self, value: Optional[pulumi.Input[float]]):
-        pulumi.set(self, "decay_rate", value)
+    @contacts.setter
+    def contacts(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "contacts", value)
 
     @property
     @pulumi.getter
-    def description(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "description")
+    def errors(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "errors")
 
-    @description.setter
-    def description(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "description", value)
+    @errors.setter
+    def errors(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "errors", value)
 
     @property
     @pulumi.getter
-    def domain(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "domain")
+    def network(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "network")
 
-    @domain.setter
-    def domain(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "domain", value)
+    @network.setter
+    def network(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "network", value)
 
     @property
-    @pulumi.getter(name="hostHeader")
-    def host_header(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "host_header")
+    @pulumi.getter
+    def note(self) -> Optional[pulumi.Input[str]]:
+        """
+        assigns a log message to the activation request
+        """
+        return pulumi.get(self, "note")
 
-    @host_header.setter
-    def host_header(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "host_header", value)
+    @note.setter
+    def note(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "note", value)
 
     @property
-    @pulumi.getter(name="leaderString")
-    def leader_string(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "leader_string")
+    @pulumi.getter(name="propertyId")
+    def property_id(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "property_id")
 
-    @leader_string.setter
-    def leader_string(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "leader_string", value)
+    @property_id.setter
+    def property_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "property_id", value)
 
     @property
-    @pulumi.getter(name="leastSquaresDecay")
-    def least_squares_decay(self) -> Optional[pulumi.Input[float]]:
-        return pulumi.get(self, "least_squares_decay")
+    @pulumi.getter(name="ruleErrors")
+    def rule_errors(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PropertyActivationRuleErrorArgs']]]]:
+        return pulumi.get(self, "rule_errors")
 
-    @least_squares_decay.setter
-    def least_squares_decay(self, value: Optional[pulumi.Input[float]]):
-        pulumi.set(self, "least_squares_decay", value)
+    @rule_errors.setter
+    def rule_errors(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PropertyActivationRuleErrorArgs']]]]):
+        pulumi.set(self, "rule_errors", value)
 
     @property
-    @pulumi.getter(name="loadImbalancePercentage")
-    def load_imbalance_percentage(self) -> Optional[pulumi.Input[float]]:
-        return pulumi.get(self, "load_imbalance_percentage")
+    @pulumi.getter(name="ruleWarnings")
+    def rule_warnings(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PropertyActivationRuleWarningArgs']]]]:
+        warnings.warn("""Rule warnings will not be set in state anymore""", DeprecationWarning)
+        pulumi.log.warn("""rule_warnings is deprecated: Rule warnings will not be set in state anymore""")
 
-    @load_imbalance_percentage.setter
-    def load_imbalance_percentage(self, value: Optional[pulumi.Input[float]]):
-        pulumi.set(self, "load_imbalance_percentage", value)
+        return pulumi.get(self, "rule_warnings")
 
-    @property
-    @pulumi.getter(name="maxUMultiplicativeIncrement")
-    def max_u_multiplicative_increment(self) -> Optional[pulumi.Input[float]]:
-        return pulumi.get(self, "max_u_multiplicative_increment")
-
-    @max_u_multiplicative_increment.setter
-    def max_u_multiplicative_increment(self, value: Optional[pulumi.Input[float]]):
-        pulumi.set(self, "max_u_multiplicative_increment", value)
+    @rule_warnings.setter
+    def rule_warnings(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PropertyActivationRuleWarningArgs']]]]):
+        pulumi.set(self, "rule_warnings", value)
 
     @property
     @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "name")
+    def status(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "status")
 
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
+    @status.setter
+    def status(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "status", value)
 
     @property
-    @pulumi.getter(name="resourceInstances")
-    def resource_instances(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['GtmResourceResourceInstanceArgs']]]]:
-        return pulumi.get(self, "resource_instances")
+    @pulumi.getter
+    def version(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "version")
 
-    @resource_instances.setter
-    def resource_instances(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['GtmResourceResourceInstanceArgs']]]]):
-        pulumi.set(self, "resource_instances", value)
+    @version.setter
+    def version(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "version", value)
 
     @property
     @pulumi.getter
-    def type(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "type")
+    def warnings(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "warnings")
 
-    @type.setter
-    def type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "type", value)
+    @warnings.setter
+    def warnings(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "warnings", value)
 
     @property
-    @pulumi.getter(name="upperBound")
-    def upper_bound(self) -> Optional[pulumi.Input[int]]:
-        return pulumi.get(self, "upper_bound")
-
-    @upper_bound.setter
-    def upper_bound(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "upper_bound", value)
+    @pulumi.getter
+    def property(self) -> Optional[pulumi.Input[str]]:
+        warnings.warn("""The setting \"property\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""property is deprecated: The setting \"property\" has been deprecated.""")
 
-    @property
-    @pulumi.getter(name="waitOnComplete")
-    def wait_on_complete(self) -> Optional[pulumi.Input[bool]]:
-        return pulumi.get(self, "wait_on_complete")
+        return pulumi.get(self, "property")
 
-    @wait_on_complete.setter
-    def wait_on_complete(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "wait_on_complete", value)
+    @property.setter
+    def property(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "property", value)
 
 
-class GtmResource(pulumi.CustomResource):
+class PropertyActivation(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 aggregation_type: Optional[pulumi.Input[str]] = None,
-                 constrained_property: Optional[pulumi.Input[str]] = None,
-                 decay_rate: Optional[pulumi.Input[float]] = None,
-                 description: Optional[pulumi.Input[str]] = None,
-                 domain: Optional[pulumi.Input[str]] = None,
-                 host_header: Optional[pulumi.Input[str]] = None,
-                 leader_string: Optional[pulumi.Input[str]] = None,
-                 least_squares_decay: Optional[pulumi.Input[float]] = None,
-                 load_imbalance_percentage: Optional[pulumi.Input[float]] = None,
-                 max_u_multiplicative_increment: Optional[pulumi.Input[float]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 resource_instances: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['GtmResourceResourceInstanceArgs']]]]] = None,
-                 type: Optional[pulumi.Input[str]] = None,
-                 upper_bound: Optional[pulumi.Input[int]] = None,
-                 wait_on_complete: Optional[pulumi.Input[bool]] = None,
+                 activation_id: Optional[pulumi.Input[str]] = None,
+                 auto_acknowledge_rule_warnings: Optional[pulumi.Input[bool]] = None,
+                 compliance_record: Optional[pulumi.Input[pulumi.InputType['PropertyActivationComplianceRecordArgs']]] = None,
+                 contacts: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 network: Optional[pulumi.Input[str]] = None,
+                 note: Optional[pulumi.Input[str]] = None,
+                 property: Optional[pulumi.Input[str]] = None,
+                 property_id: Optional[pulumi.Input[str]] = None,
+                 rule_errors: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PropertyActivationRuleErrorArgs']]]]] = None,
+                 rule_warnings: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PropertyActivationRuleWarningArgs']]]]] = None,
+                 version: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
-        Create a GtmResource resource with the given unique name, props, and options.
+        Create a PropertyActivation resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[bool] auto_acknowledge_rule_warnings: automatically acknowledge all rule warnings for activation to continue. default is true
+        :param pulumi.Input[pulumi.InputType['PropertyActivationComplianceRecordArgs']] compliance_record: Provides an audit record when activating on a production network
+        :param pulumi.Input[str] note: assigns a log message to the activation request
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: GtmResourceArgs,
+                 args: PropertyActivationArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a GtmResource resource with the given unique name, props, and options.
+        Create a PropertyActivation resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
-        :param GtmResourceArgs args: The arguments to use to populate this resource's properties.
+        :param PropertyActivationArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(GtmResourceArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(PropertyActivationArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 aggregation_type: Optional[pulumi.Input[str]] = None,
-                 constrained_property: Optional[pulumi.Input[str]] = None,
-                 decay_rate: Optional[pulumi.Input[float]] = None,
-                 description: Optional[pulumi.Input[str]] = None,
-                 domain: Optional[pulumi.Input[str]] = None,
-                 host_header: Optional[pulumi.Input[str]] = None,
-                 leader_string: Optional[pulumi.Input[str]] = None,
-                 least_squares_decay: Optional[pulumi.Input[float]] = None,
-                 load_imbalance_percentage: Optional[pulumi.Input[float]] = None,
-                 max_u_multiplicative_increment: Optional[pulumi.Input[float]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 resource_instances: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['GtmResourceResourceInstanceArgs']]]]] = None,
-                 type: Optional[pulumi.Input[str]] = None,
-                 upper_bound: Optional[pulumi.Input[int]] = None,
-                 wait_on_complete: Optional[pulumi.Input[bool]] = None,
+                 activation_id: Optional[pulumi.Input[str]] = None,
+                 auto_acknowledge_rule_warnings: Optional[pulumi.Input[bool]] = None,
+                 compliance_record: Optional[pulumi.Input[pulumi.InputType['PropertyActivationComplianceRecordArgs']]] = None,
+                 contacts: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 network: Optional[pulumi.Input[str]] = None,
+                 note: Optional[pulumi.Input[str]] = None,
+                 property: Optional[pulumi.Input[str]] = None,
+                 property_id: Optional[pulumi.Input[str]] = None,
+                 rule_errors: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PropertyActivationRuleErrorArgs']]]]] = None,
+                 rule_warnings: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PropertyActivationRuleWarningArgs']]]]] = None,
+                 version: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = GtmResourceArgs.__new__(GtmResourceArgs)
+            __props__ = PropertyActivationArgs.__new__(PropertyActivationArgs)
 
-            if aggregation_type is None and not opts.urn:
-                raise TypeError("Missing required property 'aggregation_type'")
-            __props__.__dict__["aggregation_type"] = aggregation_type
-            __props__.__dict__["constrained_property"] = constrained_property
-            __props__.__dict__["decay_rate"] = decay_rate
-            __props__.__dict__["description"] = description
-            if domain is None and not opts.urn:
-                raise TypeError("Missing required property 'domain'")
-            __props__.__dict__["domain"] = domain
-            __props__.__dict__["host_header"] = host_header
-            __props__.__dict__["leader_string"] = leader_string
-            __props__.__dict__["least_squares_decay"] = least_squares_decay
-            __props__.__dict__["load_imbalance_percentage"] = load_imbalance_percentage
-            __props__.__dict__["max_u_multiplicative_increment"] = max_u_multiplicative_increment
-            __props__.__dict__["name"] = name
-            __props__.__dict__["resource_instances"] = resource_instances
-            if type is None and not opts.urn:
-                raise TypeError("Missing required property 'type'")
-            __props__.__dict__["type"] = type
-            __props__.__dict__["upper_bound"] = upper_bound
-            __props__.__dict__["wait_on_complete"] = wait_on_complete
-        alias_opts = pulumi.ResourceOptions(aliases=[pulumi.Alias(type_="akamai:trafficmanagement/gtmResource:GtmResource")])
+            __props__.__dict__["activation_id"] = activation_id
+            __props__.__dict__["auto_acknowledge_rule_warnings"] = auto_acknowledge_rule_warnings
+            __props__.__dict__["compliance_record"] = compliance_record
+            if contacts is None and not opts.urn:
+                raise TypeError("Missing required property 'contacts'")
+            __props__.__dict__["contacts"] = contacts
+            __props__.__dict__["network"] = network
+            __props__.__dict__["note"] = note
+            if property is not None and not opts.urn:
+                warnings.warn("""The setting \"property\" has been deprecated.""", DeprecationWarning)
+                pulumi.log.warn("""property is deprecated: The setting \"property\" has been deprecated.""")
+            __props__.__dict__["property"] = property
+            __props__.__dict__["property_id"] = property_id
+            __props__.__dict__["rule_errors"] = rule_errors
+            if rule_warnings is not None and not opts.urn:
+                warnings.warn("""Rule warnings will not be set in state anymore""", DeprecationWarning)
+                pulumi.log.warn("""rule_warnings is deprecated: Rule warnings will not be set in state anymore""")
+            __props__.__dict__["rule_warnings"] = rule_warnings
+            if version is None and not opts.urn:
+                raise TypeError("Missing required property 'version'")
+            __props__.__dict__["version"] = version
+            __props__.__dict__["errors"] = None
+            __props__.__dict__["status"] = None
+            __props__.__dict__["warnings"] = None
+        alias_opts = pulumi.ResourceOptions(aliases=[pulumi.Alias(type_="akamai:properties/propertyActivation:PropertyActivation")])
         opts = pulumi.ResourceOptions.merge(opts, alias_opts)
-        super(GtmResource, __self__).__init__(
-            'akamai:index/gtmResource:GtmResource',
+        super(PropertyActivation, __self__).__init__(
+            'akamai:index/propertyActivation:PropertyActivation',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            aggregation_type: Optional[pulumi.Input[str]] = None,
-            constrained_property: Optional[pulumi.Input[str]] = None,
-            decay_rate: Optional[pulumi.Input[float]] = None,
-            description: Optional[pulumi.Input[str]] = None,
-            domain: Optional[pulumi.Input[str]] = None,
-            host_header: Optional[pulumi.Input[str]] = None,
-            leader_string: Optional[pulumi.Input[str]] = None,
-            least_squares_decay: Optional[pulumi.Input[float]] = None,
-            load_imbalance_percentage: Optional[pulumi.Input[float]] = None,
-            max_u_multiplicative_increment: Optional[pulumi.Input[float]] = None,
-            name: Optional[pulumi.Input[str]] = None,
-            resource_instances: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['GtmResourceResourceInstanceArgs']]]]] = None,
-            type: Optional[pulumi.Input[str]] = None,
-            upper_bound: Optional[pulumi.Input[int]] = None,
-            wait_on_complete: Optional[pulumi.Input[bool]] = None) -> 'GtmResource':
+            activation_id: Optional[pulumi.Input[str]] = None,
+            auto_acknowledge_rule_warnings: Optional[pulumi.Input[bool]] = None,
+            compliance_record: Optional[pulumi.Input[pulumi.InputType['PropertyActivationComplianceRecordArgs']]] = None,
+            contacts: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            errors: Optional[pulumi.Input[str]] = None,
+            network: Optional[pulumi.Input[str]] = None,
+            note: Optional[pulumi.Input[str]] = None,
+            property: Optional[pulumi.Input[str]] = None,
+            property_id: Optional[pulumi.Input[str]] = None,
+            rule_errors: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PropertyActivationRuleErrorArgs']]]]] = None,
+            rule_warnings: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PropertyActivationRuleWarningArgs']]]]] = None,
+            status: Optional[pulumi.Input[str]] = None,
+            version: Optional[pulumi.Input[int]] = None,
+            warnings: Optional[pulumi.Input[str]] = None) -> 'PropertyActivation':
         """
-        Get an existing GtmResource resource's state with the given name, id, and optional extra
+        Get an existing PropertyActivation resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[bool] auto_acknowledge_rule_warnings: automatically acknowledge all rule warnings for activation to continue. default is true
+        :param pulumi.Input[pulumi.InputType['PropertyActivationComplianceRecordArgs']] compliance_record: Provides an audit record when activating on a production network
+        :param pulumi.Input[str] note: assigns a log message to the activation request
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _GtmResourceState.__new__(_GtmResourceState)
+        __props__ = _PropertyActivationState.__new__(_PropertyActivationState)
 
-        __props__.__dict__["aggregation_type"] = aggregation_type
-        __props__.__dict__["constrained_property"] = constrained_property
-        __props__.__dict__["decay_rate"] = decay_rate
-        __props__.__dict__["description"] = description
-        __props__.__dict__["domain"] = domain
-        __props__.__dict__["host_header"] = host_header
-        __props__.__dict__["leader_string"] = leader_string
-        __props__.__dict__["least_squares_decay"] = least_squares_decay
-        __props__.__dict__["load_imbalance_percentage"] = load_imbalance_percentage
-        __props__.__dict__["max_u_multiplicative_increment"] = max_u_multiplicative_increment
-        __props__.__dict__["name"] = name
-        __props__.__dict__["resource_instances"] = resource_instances
-        __props__.__dict__["type"] = type
-        __props__.__dict__["upper_bound"] = upper_bound
-        __props__.__dict__["wait_on_complete"] = wait_on_complete
-        return GtmResource(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["activation_id"] = activation_id
+        __props__.__dict__["auto_acknowledge_rule_warnings"] = auto_acknowledge_rule_warnings
+        __props__.__dict__["compliance_record"] = compliance_record
+        __props__.__dict__["contacts"] = contacts
+        __props__.__dict__["errors"] = errors
+        __props__.__dict__["network"] = network
+        __props__.__dict__["note"] = note
+        __props__.__dict__["property"] = property
+        __props__.__dict__["property_id"] = property_id
+        __props__.__dict__["rule_errors"] = rule_errors
+        __props__.__dict__["rule_warnings"] = rule_warnings
+        __props__.__dict__["status"] = status
+        __props__.__dict__["version"] = version
+        __props__.__dict__["warnings"] = warnings
+        return PropertyActivation(resource_name, opts=opts, __props__=__props__)
+
+    @property
+    @pulumi.getter(name="activationId")
+    def activation_id(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "activation_id")
 
     @property
-    @pulumi.getter(name="aggregationType")
-    def aggregation_type(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "aggregation_type")
+    @pulumi.getter(name="autoAcknowledgeRuleWarnings")
+    def auto_acknowledge_rule_warnings(self) -> pulumi.Output[Optional[bool]]:
+        """
+        automatically acknowledge all rule warnings for activation to continue. default is true
+        """
+        return pulumi.get(self, "auto_acknowledge_rule_warnings")
 
     @property
-    @pulumi.getter(name="constrainedProperty")
-    def constrained_property(self) -> pulumi.Output[Optional[str]]:
-        return pulumi.get(self, "constrained_property")
+    @pulumi.getter(name="complianceRecord")
+    def compliance_record(self) -> pulumi.Output[Optional['outputs.PropertyActivationComplianceRecord']]:
+        """
+        Provides an audit record when activating on a production network
+        """
+        return pulumi.get(self, "compliance_record")
 
     @property
-    @pulumi.getter(name="decayRate")
-    def decay_rate(self) -> pulumi.Output[Optional[float]]:
-        return pulumi.get(self, "decay_rate")
+    @pulumi.getter
+    def contacts(self) -> pulumi.Output[Sequence[str]]:
+        return pulumi.get(self, "contacts")
 
     @property
     @pulumi.getter
-    def description(self) -> pulumi.Output[Optional[str]]:
-        return pulumi.get(self, "description")
+    def errors(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "errors")
 
     @property
     @pulumi.getter
-    def domain(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "domain")
+    def network(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "network")
 
     @property
-    @pulumi.getter(name="hostHeader")
-    def host_header(self) -> pulumi.Output[Optional[str]]:
-        return pulumi.get(self, "host_header")
+    @pulumi.getter
+    def note(self) -> pulumi.Output[Optional[str]]:
+        """
+        assigns a log message to the activation request
+        """
+        return pulumi.get(self, "note")
 
     @property
-    @pulumi.getter(name="leaderString")
-    def leader_string(self) -> pulumi.Output[Optional[str]]:
-        return pulumi.get(self, "leader_string")
+    @pulumi.getter(name="propertyId")
+    def property_id(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "property_id")
 
     @property
-    @pulumi.getter(name="leastSquaresDecay")
-    def least_squares_decay(self) -> pulumi.Output[Optional[float]]:
-        return pulumi.get(self, "least_squares_decay")
+    @pulumi.getter(name="ruleErrors")
+    def rule_errors(self) -> pulumi.Output[Sequence['outputs.PropertyActivationRuleError']]:
+        return pulumi.get(self, "rule_errors")
 
     @property
-    @pulumi.getter(name="loadImbalancePercentage")
-    def load_imbalance_percentage(self) -> pulumi.Output[Optional[float]]:
-        return pulumi.get(self, "load_imbalance_percentage")
+    @pulumi.getter(name="ruleWarnings")
+    def rule_warnings(self) -> pulumi.Output[Sequence['outputs.PropertyActivationRuleWarning']]:
+        warnings.warn("""Rule warnings will not be set in state anymore""", DeprecationWarning)
+        pulumi.log.warn("""rule_warnings is deprecated: Rule warnings will not be set in state anymore""")
 
-    @property
-    @pulumi.getter(name="maxUMultiplicativeIncrement")
-    def max_u_multiplicative_increment(self) -> pulumi.Output[Optional[float]]:
-        return pulumi.get(self, "max_u_multiplicative_increment")
+        return pulumi.get(self, "rule_warnings")
 
     @property
     @pulumi.getter
-    def name(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "name")
+    def status(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "status")
 
     @property
-    @pulumi.getter(name="resourceInstances")
-    def resource_instances(self) -> pulumi.Output[Optional[Sequence['outputs.GtmResourceResourceInstance']]]:
-        return pulumi.get(self, "resource_instances")
+    @pulumi.getter
+    def version(self) -> pulumi.Output[int]:
+        return pulumi.get(self, "version")
 
     @property
     @pulumi.getter
-    def type(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "type")
+    def warnings(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "warnings")
 
     @property
-    @pulumi.getter(name="upperBound")
-    def upper_bound(self) -> pulumi.Output[Optional[int]]:
-        return pulumi.get(self, "upper_bound")
+    @pulumi.getter
+    def property(self) -> pulumi.Output[str]:
+        warnings.warn("""The setting \"property\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""property is deprecated: The setting \"property\" has been deprecated.""")
 
-    @property
-    @pulumi.getter(name="waitOnComplete")
-    def wait_on_complete(self) -> pulumi.Output[Optional[bool]]:
-        return pulumi.get(self, "wait_on_complete")
+        return pulumi.get(self, "property")
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/iam_blocked_user_properties.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/iam_blocked_user_properties.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/iam_group.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/iam_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/iam_role.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/iam_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/iam_user.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/iam_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -536,14 +536,17 @@
 
     @property
     @pulumi.getter(name="isLocked")
     def is_locked(self) -> Optional[pulumi.Input[bool]]:
         """
         The user's lock status
         """
+        warnings.warn("""The setting \"is_locked\" has been deprecated. Please use \"lock\" setting instead""", DeprecationWarning)
+        pulumi.log.warn("""is_locked is deprecated: The setting \"is_locked\" has been deprecated. Please use \"lock\" setting instead""")
+
         return pulumi.get(self, "is_locked")
 
     @is_locked.setter
     def is_locked(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "is_locked", value)
 
     @property
@@ -1039,14 +1042,17 @@
 
     @property
     @pulumi.getter(name="isLocked")
     def is_locked(self) -> pulumi.Output[bool]:
         """
         The user's lock status
         """
+        warnings.warn("""The setting \"is_locked\" has been deprecated. Please use \"lock\" setting instead""", DeprecationWarning)
+        pulumi.log.warn("""is_locked is deprecated: The setting \"is_locked\" has been deprecated. Please use \"lock\" setting instead""")
+
         return pulumi.get(self, "is_locked")
 
     @property
     @pulumi.getter(name="jobTitle")
     def job_title(self) -> pulumi.Output[Optional[str]]:
         """
         The user's position at your company
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/network_list.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/network_list.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/network_list_activations.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/network_list_activations.py`

 * *Files 8% similar despite different names*

```diff
@@ -76,14 +76,17 @@
     @sync_point.setter
     def sync_point(self, value: pulumi.Input[int]):
         pulumi.set(self, "sync_point", value)
 
     @property
     @pulumi.getter
     def activate(self) -> Optional[pulumi.Input[bool]]:
+        warnings.warn("""The setting \"activate\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""activate is deprecated: The setting \"activate\" has been deprecated.""")
+
         return pulumi.get(self, "activate")
 
     @activate.setter
     def activate(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "activate", value)
 
     @property
@@ -147,14 +150,17 @@
             pulumi.set(__self__, "status", status)
         if sync_point is not None:
             pulumi.set(__self__, "sync_point", sync_point)
 
     @property
     @pulumi.getter
     def activate(self) -> Optional[pulumi.Input[bool]]:
+        warnings.warn("""The setting \"activate\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""activate is deprecated: The setting \"activate\" has been deprecated.""")
+
         return pulumi.get(self, "activate")
 
     @activate.setter
     def activate(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "activate", value)
 
     @property
@@ -349,14 +355,17 @@
         __props__.__dict__["status"] = status
         __props__.__dict__["sync_point"] = sync_point
         return NetworkListActivations(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def activate(self) -> pulumi.Output[Optional[bool]]:
+        warnings.warn("""The setting \"activate\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""activate is deprecated: The setting \"activate\" has been deprecated.""")
+
         return pulumi.get(self, "activate")
 
     @property
     @pulumi.getter
     def network(self) -> pulumi.Output[Optional[str]]:
         """
         The Akamai network on which the list is activated: STAGING or PRODUCTION
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/network_list_description.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/network_list_description.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/network_list_subscription.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/network_list_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/outputs.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,19 +51,27 @@
     'GtmGeomapDefaultDatacenter',
     'GtmPropertyLivenessTest',
     'GtmPropertyLivenessTestHttpHeader',
     'GtmPropertyStaticRrSet',
     'GtmPropertyTrafficTarget',
     'GtmResourceResourceInstance',
     'PropertyActivationComplianceRecord',
+    'PropertyActivationComplianceRecordNoncomplianceReasonEmergency',
+    'PropertyActivationComplianceRecordNoncomplianceReasonNoProductionTraffic',
+    'PropertyActivationComplianceRecordNoncomplianceReasonNone',
+    'PropertyActivationComplianceRecordNoncomplianceReasonOther',
     'PropertyActivationRuleError',
     'PropertyActivationRuleWarning',
     'PropertyHostname',
     'PropertyHostnameCertStatus',
     'PropertyIncludeActivationComplianceRecord',
+    'PropertyIncludeActivationComplianceRecordNoncomplianceReasonEmergency',
+    'PropertyIncludeActivationComplianceRecordNoncomplianceReasonNoProductionTraffic',
+    'PropertyIncludeActivationComplianceRecordNoncomplianceReasonNone',
+    'PropertyIncludeActivationComplianceRecordNoncomplianceReasonOther',
     'PropertyOrigin',
     'PropertyRuleError',
     'PropertyRuleWarning',
     'GetCPSEnrollmentAdminContactResult',
     'GetCPSEnrollmentCsrResult',
     'GetCPSEnrollmentDnsChallengeResult',
     'GetCPSEnrollmentHttpChallengeResult',
@@ -123,14 +131,19 @@
     'GetDatastreamActivationHistoryActivationResult',
     'GetDatastreamDatasetFieldsFieldResult',
     'GetDatastreamDatasetFieldsFieldDatasetFieldResult',
     'GetDatastreamsStreamResult',
     'GetDatastreamsStreamErrorResult',
     'GetDatastreamsStreamPropertyResult',
     'GetGroupsGroupResult',
+    'GetGtmDatacenterDefaultLoadObjectResult',
+    'GetGtmDatacenterLinkResult',
+    'GetGtmDatacentersDatacenterResult',
+    'GetGtmDatacentersDatacenterDefaultLoadObjectResult',
+    'GetGtmDatacentersDatacenterLinkResult',
     'GetIamGrantableRolesGrantableRoleResult',
     'GetIamRolesRoleResult',
     'GetIamTimezonesTimezoneResult',
     'GetPropertiesPropertyResult',
     'GetPropertiesSearchPropertyResult',
     'GetPropertyHostnamesHostnameResult',
     'GetPropertyHostnamesHostnameCertStatusResult',
@@ -3817,14 +3830,17 @@
     @pulumi.getter(name="handoutCname")
     def handout_cname(self) -> Optional[str]:
         return pulumi.get(self, "handout_cname")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
+        warnings.warn("""The attribute `name` has been deprecated. Any reads or writes on this attribute are ignored""", DeprecationWarning)
+        pulumi.log.warn("""name is deprecated: The attribute `name` has been deprecated. Any reads or writes on this attribute are ignored""")
+
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def servers(self) -> Optional[Sequence[str]]:
         return pulumi.get(self, "servers")
 
@@ -3904,73 +3920,174 @@
 
 
 @pulumi.output_type
 class PropertyActivationComplianceRecord(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
-        if key == "noncomplianceReason":
-            suggest = "noncompliance_reason"
-        elif key == "customerEmail":
+        if key == "noncomplianceReasonEmergency":
+            suggest = "noncompliance_reason_emergency"
+        elif key == "noncomplianceReasonNoProductionTraffic":
+            suggest = "noncompliance_reason_no_production_traffic"
+        elif key == "noncomplianceReasonNone":
+            suggest = "noncompliance_reason_none"
+        elif key == "noncomplianceReasonOther":
+            suggest = "noncompliance_reason_other"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in PropertyActivationComplianceRecord. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        PropertyActivationComplianceRecord.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        PropertyActivationComplianceRecord.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 noncompliance_reason_emergency: Optional['outputs.PropertyActivationComplianceRecordNoncomplianceReasonEmergency'] = None,
+                 noncompliance_reason_no_production_traffic: Optional['outputs.PropertyActivationComplianceRecordNoncomplianceReasonNoProductionTraffic'] = None,
+                 noncompliance_reason_none: Optional['outputs.PropertyActivationComplianceRecordNoncomplianceReasonNone'] = None,
+                 noncompliance_reason_other: Optional['outputs.PropertyActivationComplianceRecordNoncomplianceReasonOther'] = None):
+        if noncompliance_reason_emergency is not None:
+            pulumi.set(__self__, "noncompliance_reason_emergency", noncompliance_reason_emergency)
+        if noncompliance_reason_no_production_traffic is not None:
+            pulumi.set(__self__, "noncompliance_reason_no_production_traffic", noncompliance_reason_no_production_traffic)
+        if noncompliance_reason_none is not None:
+            pulumi.set(__self__, "noncompliance_reason_none", noncompliance_reason_none)
+        if noncompliance_reason_other is not None:
+            pulumi.set(__self__, "noncompliance_reason_other", noncompliance_reason_other)
+
+    @property
+    @pulumi.getter(name="noncomplianceReasonEmergency")
+    def noncompliance_reason_emergency(self) -> Optional['outputs.PropertyActivationComplianceRecordNoncomplianceReasonEmergency']:
+        return pulumi.get(self, "noncompliance_reason_emergency")
+
+    @property
+    @pulumi.getter(name="noncomplianceReasonNoProductionTraffic")
+    def noncompliance_reason_no_production_traffic(self) -> Optional['outputs.PropertyActivationComplianceRecordNoncomplianceReasonNoProductionTraffic']:
+        return pulumi.get(self, "noncompliance_reason_no_production_traffic")
+
+    @property
+    @pulumi.getter(name="noncomplianceReasonNone")
+    def noncompliance_reason_none(self) -> Optional['outputs.PropertyActivationComplianceRecordNoncomplianceReasonNone']:
+        return pulumi.get(self, "noncompliance_reason_none")
+
+    @property
+    @pulumi.getter(name="noncomplianceReasonOther")
+    def noncompliance_reason_other(self) -> Optional['outputs.PropertyActivationComplianceRecordNoncomplianceReasonOther']:
+        return pulumi.get(self, "noncompliance_reason_other")
+
+
+@pulumi.output_type
+class PropertyActivationComplianceRecordNoncomplianceReasonEmergency(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "ticketId":
+            suggest = "ticket_id"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in PropertyActivationComplianceRecordNoncomplianceReasonEmergency. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        PropertyActivationComplianceRecordNoncomplianceReasonEmergency.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        PropertyActivationComplianceRecordNoncomplianceReasonEmergency.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 ticket_id: Optional[str] = None):
+        if ticket_id is not None:
+            pulumi.set(__self__, "ticket_id", ticket_id)
+
+    @property
+    @pulumi.getter(name="ticketId")
+    def ticket_id(self) -> Optional[str]:
+        return pulumi.get(self, "ticket_id")
+
+
+@pulumi.output_type
+class PropertyActivationComplianceRecordNoncomplianceReasonNoProductionTraffic(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "ticketId":
+            suggest = "ticket_id"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in PropertyActivationComplianceRecordNoncomplianceReasonNoProductionTraffic. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        PropertyActivationComplianceRecordNoncomplianceReasonNoProductionTraffic.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        PropertyActivationComplianceRecordNoncomplianceReasonNoProductionTraffic.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 ticket_id: Optional[str] = None):
+        if ticket_id is not None:
+            pulumi.set(__self__, "ticket_id", ticket_id)
+
+    @property
+    @pulumi.getter(name="ticketId")
+    def ticket_id(self) -> Optional[str]:
+        return pulumi.get(self, "ticket_id")
+
+
+@pulumi.output_type
+class PropertyActivationComplianceRecordNoncomplianceReasonNone(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "customerEmail":
             suggest = "customer_email"
-        elif key == "otherNoncomplianceReason":
-            suggest = "other_noncompliance_reason"
         elif key == "peerReviewedBy":
             suggest = "peer_reviewed_by"
         elif key == "ticketId":
             suggest = "ticket_id"
         elif key == "unitTested":
             suggest = "unit_tested"
 
         if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in PropertyActivationComplianceRecord. Access the value via the '{suggest}' property getter instead.")
+            pulumi.log.warn(f"Key '{key}' not found in PropertyActivationComplianceRecordNoncomplianceReasonNone. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
-        PropertyActivationComplianceRecord.__key_warning(key)
+        PropertyActivationComplianceRecordNoncomplianceReasonNone.__key_warning(key)
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
-        PropertyActivationComplianceRecord.__key_warning(key)
+        PropertyActivationComplianceRecordNoncomplianceReasonNone.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
-                 noncompliance_reason: str,
                  customer_email: Optional[str] = None,
-                 other_noncompliance_reason: Optional[str] = None,
                  peer_reviewed_by: Optional[str] = None,
                  ticket_id: Optional[str] = None,
                  unit_tested: Optional[bool] = None):
-        pulumi.set(__self__, "noncompliance_reason", noncompliance_reason)
         if customer_email is not None:
             pulumi.set(__self__, "customer_email", customer_email)
-        if other_noncompliance_reason is not None:
-            pulumi.set(__self__, "other_noncompliance_reason", other_noncompliance_reason)
         if peer_reviewed_by is not None:
             pulumi.set(__self__, "peer_reviewed_by", peer_reviewed_by)
         if ticket_id is not None:
             pulumi.set(__self__, "ticket_id", ticket_id)
         if unit_tested is not None:
             pulumi.set(__self__, "unit_tested", unit_tested)
 
     @property
-    @pulumi.getter(name="noncomplianceReason")
-    def noncompliance_reason(self) -> str:
-        return pulumi.get(self, "noncompliance_reason")
-
-    @property
     @pulumi.getter(name="customerEmail")
     def customer_email(self) -> Optional[str]:
         return pulumi.get(self, "customer_email")
 
     @property
-    @pulumi.getter(name="otherNoncomplianceReason")
-    def other_noncompliance_reason(self) -> Optional[str]:
-        return pulumi.get(self, "other_noncompliance_reason")
-
-    @property
     @pulumi.getter(name="peerReviewedBy")
     def peer_reviewed_by(self) -> Optional[str]:
         return pulumi.get(self, "peer_reviewed_by")
 
     @property
     @pulumi.getter(name="ticketId")
     def ticket_id(self) -> Optional[str]:
@@ -3979,14 +4096,54 @@
     @property
     @pulumi.getter(name="unitTested")
     def unit_tested(self) -> Optional[bool]:
         return pulumi.get(self, "unit_tested")
 
 
 @pulumi.output_type
+class PropertyActivationComplianceRecordNoncomplianceReasonOther(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "otherNoncomplianceReason":
+            suggest = "other_noncompliance_reason"
+        elif key == "ticketId":
+            suggest = "ticket_id"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in PropertyActivationComplianceRecordNoncomplianceReasonOther. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        PropertyActivationComplianceRecordNoncomplianceReasonOther.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        PropertyActivationComplianceRecordNoncomplianceReasonOther.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 other_noncompliance_reason: Optional[str] = None,
+                 ticket_id: Optional[str] = None):
+        if other_noncompliance_reason is not None:
+            pulumi.set(__self__, "other_noncompliance_reason", other_noncompliance_reason)
+        if ticket_id is not None:
+            pulumi.set(__self__, "ticket_id", ticket_id)
+
+    @property
+    @pulumi.getter(name="otherNoncomplianceReason")
+    def other_noncompliance_reason(self) -> Optional[str]:
+        return pulumi.get(self, "other_noncompliance_reason")
+
+    @property
+    @pulumi.getter(name="ticketId")
+    def ticket_id(self) -> Optional[str]:
+        return pulumi.get(self, "ticket_id")
+
+
+@pulumi.output_type
 class PropertyActivationRuleError(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "behaviorName":
             suggest = "behavior_name"
         elif key == "errorLocation":
@@ -4280,73 +4437,174 @@
 
 
 @pulumi.output_type
 class PropertyIncludeActivationComplianceRecord(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
-        if key == "noncomplianceReason":
-            suggest = "noncompliance_reason"
-        elif key == "customerEmail":
+        if key == "noncomplianceReasonEmergency":
+            suggest = "noncompliance_reason_emergency"
+        elif key == "noncomplianceReasonNoProductionTraffic":
+            suggest = "noncompliance_reason_no_production_traffic"
+        elif key == "noncomplianceReasonNone":
+            suggest = "noncompliance_reason_none"
+        elif key == "noncomplianceReasonOther":
+            suggest = "noncompliance_reason_other"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in PropertyIncludeActivationComplianceRecord. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        PropertyIncludeActivationComplianceRecord.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        PropertyIncludeActivationComplianceRecord.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 noncompliance_reason_emergency: Optional['outputs.PropertyIncludeActivationComplianceRecordNoncomplianceReasonEmergency'] = None,
+                 noncompliance_reason_no_production_traffic: Optional['outputs.PropertyIncludeActivationComplianceRecordNoncomplianceReasonNoProductionTraffic'] = None,
+                 noncompliance_reason_none: Optional['outputs.PropertyIncludeActivationComplianceRecordNoncomplianceReasonNone'] = None,
+                 noncompliance_reason_other: Optional['outputs.PropertyIncludeActivationComplianceRecordNoncomplianceReasonOther'] = None):
+        if noncompliance_reason_emergency is not None:
+            pulumi.set(__self__, "noncompliance_reason_emergency", noncompliance_reason_emergency)
+        if noncompliance_reason_no_production_traffic is not None:
+            pulumi.set(__self__, "noncompliance_reason_no_production_traffic", noncompliance_reason_no_production_traffic)
+        if noncompliance_reason_none is not None:
+            pulumi.set(__self__, "noncompliance_reason_none", noncompliance_reason_none)
+        if noncompliance_reason_other is not None:
+            pulumi.set(__self__, "noncompliance_reason_other", noncompliance_reason_other)
+
+    @property
+    @pulumi.getter(name="noncomplianceReasonEmergency")
+    def noncompliance_reason_emergency(self) -> Optional['outputs.PropertyIncludeActivationComplianceRecordNoncomplianceReasonEmergency']:
+        return pulumi.get(self, "noncompliance_reason_emergency")
+
+    @property
+    @pulumi.getter(name="noncomplianceReasonNoProductionTraffic")
+    def noncompliance_reason_no_production_traffic(self) -> Optional['outputs.PropertyIncludeActivationComplianceRecordNoncomplianceReasonNoProductionTraffic']:
+        return pulumi.get(self, "noncompliance_reason_no_production_traffic")
+
+    @property
+    @pulumi.getter(name="noncomplianceReasonNone")
+    def noncompliance_reason_none(self) -> Optional['outputs.PropertyIncludeActivationComplianceRecordNoncomplianceReasonNone']:
+        return pulumi.get(self, "noncompliance_reason_none")
+
+    @property
+    @pulumi.getter(name="noncomplianceReasonOther")
+    def noncompliance_reason_other(self) -> Optional['outputs.PropertyIncludeActivationComplianceRecordNoncomplianceReasonOther']:
+        return pulumi.get(self, "noncompliance_reason_other")
+
+
+@pulumi.output_type
+class PropertyIncludeActivationComplianceRecordNoncomplianceReasonEmergency(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "ticketId":
+            suggest = "ticket_id"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in PropertyIncludeActivationComplianceRecordNoncomplianceReasonEmergency. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        PropertyIncludeActivationComplianceRecordNoncomplianceReasonEmergency.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        PropertyIncludeActivationComplianceRecordNoncomplianceReasonEmergency.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 ticket_id: Optional[str] = None):
+        if ticket_id is not None:
+            pulumi.set(__self__, "ticket_id", ticket_id)
+
+    @property
+    @pulumi.getter(name="ticketId")
+    def ticket_id(self) -> Optional[str]:
+        return pulumi.get(self, "ticket_id")
+
+
+@pulumi.output_type
+class PropertyIncludeActivationComplianceRecordNoncomplianceReasonNoProductionTraffic(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "ticketId":
+            suggest = "ticket_id"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in PropertyIncludeActivationComplianceRecordNoncomplianceReasonNoProductionTraffic. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        PropertyIncludeActivationComplianceRecordNoncomplianceReasonNoProductionTraffic.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        PropertyIncludeActivationComplianceRecordNoncomplianceReasonNoProductionTraffic.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 ticket_id: Optional[str] = None):
+        if ticket_id is not None:
+            pulumi.set(__self__, "ticket_id", ticket_id)
+
+    @property
+    @pulumi.getter(name="ticketId")
+    def ticket_id(self) -> Optional[str]:
+        return pulumi.get(self, "ticket_id")
+
+
+@pulumi.output_type
+class PropertyIncludeActivationComplianceRecordNoncomplianceReasonNone(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "customerEmail":
             suggest = "customer_email"
-        elif key == "otherNoncomplianceReason":
-            suggest = "other_noncompliance_reason"
         elif key == "peerReviewedBy":
             suggest = "peer_reviewed_by"
         elif key == "ticketId":
             suggest = "ticket_id"
         elif key == "unitTested":
             suggest = "unit_tested"
 
         if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in PropertyIncludeActivationComplianceRecord. Access the value via the '{suggest}' property getter instead.")
+            pulumi.log.warn(f"Key '{key}' not found in PropertyIncludeActivationComplianceRecordNoncomplianceReasonNone. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
-        PropertyIncludeActivationComplianceRecord.__key_warning(key)
+        PropertyIncludeActivationComplianceRecordNoncomplianceReasonNone.__key_warning(key)
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
-        PropertyIncludeActivationComplianceRecord.__key_warning(key)
+        PropertyIncludeActivationComplianceRecordNoncomplianceReasonNone.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
-                 noncompliance_reason: str,
                  customer_email: Optional[str] = None,
-                 other_noncompliance_reason: Optional[str] = None,
                  peer_reviewed_by: Optional[str] = None,
                  ticket_id: Optional[str] = None,
                  unit_tested: Optional[bool] = None):
-        pulumi.set(__self__, "noncompliance_reason", noncompliance_reason)
         if customer_email is not None:
             pulumi.set(__self__, "customer_email", customer_email)
-        if other_noncompliance_reason is not None:
-            pulumi.set(__self__, "other_noncompliance_reason", other_noncompliance_reason)
         if peer_reviewed_by is not None:
             pulumi.set(__self__, "peer_reviewed_by", peer_reviewed_by)
         if ticket_id is not None:
             pulumi.set(__self__, "ticket_id", ticket_id)
         if unit_tested is not None:
             pulumi.set(__self__, "unit_tested", unit_tested)
 
     @property
-    @pulumi.getter(name="noncomplianceReason")
-    def noncompliance_reason(self) -> str:
-        return pulumi.get(self, "noncompliance_reason")
-
-    @property
     @pulumi.getter(name="customerEmail")
     def customer_email(self) -> Optional[str]:
         return pulumi.get(self, "customer_email")
 
     @property
-    @pulumi.getter(name="otherNoncomplianceReason")
-    def other_noncompliance_reason(self) -> Optional[str]:
-        return pulumi.get(self, "other_noncompliance_reason")
-
-    @property
     @pulumi.getter(name="peerReviewedBy")
     def peer_reviewed_by(self) -> Optional[str]:
         return pulumi.get(self, "peer_reviewed_by")
 
     @property
     @pulumi.getter(name="ticketId")
     def ticket_id(self) -> Optional[str]:
@@ -4355,14 +4613,54 @@
     @property
     @pulumi.getter(name="unitTested")
     def unit_tested(self) -> Optional[bool]:
         return pulumi.get(self, "unit_tested")
 
 
 @pulumi.output_type
+class PropertyIncludeActivationComplianceRecordNoncomplianceReasonOther(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "otherNoncomplianceReason":
+            suggest = "other_noncompliance_reason"
+        elif key == "ticketId":
+            suggest = "ticket_id"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in PropertyIncludeActivationComplianceRecordNoncomplianceReasonOther. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        PropertyIncludeActivationComplianceRecordNoncomplianceReasonOther.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        PropertyIncludeActivationComplianceRecordNoncomplianceReasonOther.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 other_noncompliance_reason: Optional[str] = None,
+                 ticket_id: Optional[str] = None):
+        if other_noncompliance_reason is not None:
+            pulumi.set(__self__, "other_noncompliance_reason", other_noncompliance_reason)
+        if ticket_id is not None:
+            pulumi.set(__self__, "ticket_id", ticket_id)
+
+    @property
+    @pulumi.getter(name="otherNoncomplianceReason")
+    def other_noncompliance_reason(self) -> Optional[str]:
+        return pulumi.get(self, "other_noncompliance_reason")
+
+    @property
+    @pulumi.getter(name="ticketId")
+    def ticket_id(self) -> Optional[str]:
+        return pulumi.get(self, "ticket_id")
+
+
+@pulumi.output_type
 class PropertyOrigin(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "cacheKeyHostname":
             suggest = "cache_key_hostname"
         elif key == "enableTrueClientIp":
@@ -8020,14 +8318,221 @@
     @property
     @pulumi.getter(name="parentGroupId")
     def parent_group_id(self) -> str:
         return pulumi.get(self, "parent_group_id")
 
 
 @pulumi.output_type
+class GetGtmDatacenterDefaultLoadObjectResult(dict):
+    def __init__(__self__, *,
+                 load_object: str,
+                 load_object_port: int,
+                 load_servers: Sequence[str]):
+        pulumi.set(__self__, "load_object", load_object)
+        pulumi.set(__self__, "load_object_port", load_object_port)
+        pulumi.set(__self__, "load_servers", load_servers)
+
+    @property
+    @pulumi.getter(name="loadObject")
+    def load_object(self) -> str:
+        return pulumi.get(self, "load_object")
+
+    @property
+    @pulumi.getter(name="loadObjectPort")
+    def load_object_port(self) -> int:
+        return pulumi.get(self, "load_object_port")
+
+    @property
+    @pulumi.getter(name="loadServers")
+    def load_servers(self) -> Sequence[str]:
+        return pulumi.get(self, "load_servers")
+
+
+@pulumi.output_type
+class GetGtmDatacenterLinkResult(dict):
+    def __init__(__self__, *,
+                 href: str,
+                 rel: str):
+        pulumi.set(__self__, "href", href)
+        pulumi.set(__self__, "rel", rel)
+
+    @property
+    @pulumi.getter
+    def href(self) -> str:
+        return pulumi.get(self, "href")
+
+    @property
+    @pulumi.getter
+    def rel(self) -> str:
+        return pulumi.get(self, "rel")
+
+
+@pulumi.output_type
+class GetGtmDatacentersDatacenterResult(dict):
+    def __init__(__self__, *,
+                 city: str,
+                 clone_of: int,
+                 cloud_server_host_header_override: bool,
+                 cloud_server_targeting: bool,
+                 continent: str,
+                 country: str,
+                 datacenter_id: int,
+                 default_load_objects: Sequence['outputs.GetGtmDatacentersDatacenterDefaultLoadObjectResult'],
+                 latitude: float,
+                 links: Sequence['outputs.GetGtmDatacentersDatacenterLinkResult'],
+                 longitude: float,
+                 nickname: str,
+                 score_penalty: int,
+                 servermonitor_pool: str,
+                 state_or_province: str,
+                 virtual: bool):
+        pulumi.set(__self__, "city", city)
+        pulumi.set(__self__, "clone_of", clone_of)
+        pulumi.set(__self__, "cloud_server_host_header_override", cloud_server_host_header_override)
+        pulumi.set(__self__, "cloud_server_targeting", cloud_server_targeting)
+        pulumi.set(__self__, "continent", continent)
+        pulumi.set(__self__, "country", country)
+        pulumi.set(__self__, "datacenter_id", datacenter_id)
+        pulumi.set(__self__, "default_load_objects", default_load_objects)
+        pulumi.set(__self__, "latitude", latitude)
+        pulumi.set(__self__, "links", links)
+        pulumi.set(__self__, "longitude", longitude)
+        pulumi.set(__self__, "nickname", nickname)
+        pulumi.set(__self__, "score_penalty", score_penalty)
+        pulumi.set(__self__, "servermonitor_pool", servermonitor_pool)
+        pulumi.set(__self__, "state_or_province", state_or_province)
+        pulumi.set(__self__, "virtual", virtual)
+
+    @property
+    @pulumi.getter
+    def city(self) -> str:
+        return pulumi.get(self, "city")
+
+    @property
+    @pulumi.getter(name="cloneOf")
+    def clone_of(self) -> int:
+        return pulumi.get(self, "clone_of")
+
+    @property
+    @pulumi.getter(name="cloudServerHostHeaderOverride")
+    def cloud_server_host_header_override(self) -> bool:
+        return pulumi.get(self, "cloud_server_host_header_override")
+
+    @property
+    @pulumi.getter(name="cloudServerTargeting")
+    def cloud_server_targeting(self) -> bool:
+        return pulumi.get(self, "cloud_server_targeting")
+
+    @property
+    @pulumi.getter
+    def continent(self) -> str:
+        return pulumi.get(self, "continent")
+
+    @property
+    @pulumi.getter
+    def country(self) -> str:
+        return pulumi.get(self, "country")
+
+    @property
+    @pulumi.getter(name="datacenterId")
+    def datacenter_id(self) -> int:
+        return pulumi.get(self, "datacenter_id")
+
+    @property
+    @pulumi.getter(name="defaultLoadObjects")
+    def default_load_objects(self) -> Sequence['outputs.GetGtmDatacentersDatacenterDefaultLoadObjectResult']:
+        return pulumi.get(self, "default_load_objects")
+
+    @property
+    @pulumi.getter
+    def latitude(self) -> float:
+        return pulumi.get(self, "latitude")
+
+    @property
+    @pulumi.getter
+    def links(self) -> Sequence['outputs.GetGtmDatacentersDatacenterLinkResult']:
+        return pulumi.get(self, "links")
+
+    @property
+    @pulumi.getter
+    def longitude(self) -> float:
+        return pulumi.get(self, "longitude")
+
+    @property
+    @pulumi.getter
+    def nickname(self) -> str:
+        return pulumi.get(self, "nickname")
+
+    @property
+    @pulumi.getter(name="scorePenalty")
+    def score_penalty(self) -> int:
+        return pulumi.get(self, "score_penalty")
+
+    @property
+    @pulumi.getter(name="servermonitorPool")
+    def servermonitor_pool(self) -> str:
+        return pulumi.get(self, "servermonitor_pool")
+
+    @property
+    @pulumi.getter(name="stateOrProvince")
+    def state_or_province(self) -> str:
+        return pulumi.get(self, "state_or_province")
+
+    @property
+    @pulumi.getter
+    def virtual(self) -> bool:
+        return pulumi.get(self, "virtual")
+
+
+@pulumi.output_type
+class GetGtmDatacentersDatacenterDefaultLoadObjectResult(dict):
+    def __init__(__self__, *,
+                 load_object: str,
+                 load_object_port: int,
+                 load_servers: Sequence[str]):
+        pulumi.set(__self__, "load_object", load_object)
+        pulumi.set(__self__, "load_object_port", load_object_port)
+        pulumi.set(__self__, "load_servers", load_servers)
+
+    @property
+    @pulumi.getter(name="loadObject")
+    def load_object(self) -> str:
+        return pulumi.get(self, "load_object")
+
+    @property
+    @pulumi.getter(name="loadObjectPort")
+    def load_object_port(self) -> int:
+        return pulumi.get(self, "load_object_port")
+
+    @property
+    @pulumi.getter(name="loadServers")
+    def load_servers(self) -> Sequence[str]:
+        return pulumi.get(self, "load_servers")
+
+
+@pulumi.output_type
+class GetGtmDatacentersDatacenterLinkResult(dict):
+    def __init__(__self__, *,
+                 href: str,
+                 rel: str):
+        pulumi.set(__self__, "href", href)
+        pulumi.set(__self__, "rel", rel)
+
+    @property
+    @pulumi.getter
+    def href(self) -> str:
+        return pulumi.get(self, "href")
+
+    @property
+    @pulumi.getter
+    def rel(self) -> str:
+        return pulumi.get(self, "rel")
+
+
+@pulumi.output_type
 class GetIamGrantableRolesGrantableRoleResult(dict):
     def __init__(__self__, *,
                  description: str,
                  granted_role_id: int,
                  name: str):
         pulumi.set(__self__, "description", description)
         pulumi.set(__self__, "granted_role_id", granted_role_id)
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/properties/_inputs.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/property_include.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,656 +3,567 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from .. import _utilities
+from . import _utilities
 
-__all__ = [
-    'PropertyActivationComplianceRecordArgs',
-    'PropertyActivationRuleErrorArgs',
-    'PropertyActivationRuleWarningArgs',
-    'PropertyHostnameArgs',
-    'PropertyHostnameCertStatusArgs',
-    'PropertyOriginArgs',
-    'PropertyRuleErrorArgs',
-    'PropertyRuleWarningArgs',
-]
+__all__ = ['PropertyIncludeArgs', 'PropertyInclude']
 
 @pulumi.input_type
-class PropertyActivationComplianceRecordArgs:
+class PropertyIncludeArgs:
     def __init__(__self__, *,
-                 noncompliance_reason: pulumi.Input[str],
-                 customer_email: Optional[pulumi.Input[str]] = None,
-                 other_noncompliance_reason: Optional[pulumi.Input[str]] = None,
-                 peer_reviewed_by: Optional[pulumi.Input[str]] = None,
-                 ticket_id: Optional[pulumi.Input[str]] = None,
-                 unit_tested: Optional[pulumi.Input[bool]] = None):
-        pulumi.set(__self__, "noncompliance_reason", noncompliance_reason)
-        if customer_email is not None:
-            pulumi.set(__self__, "customer_email", customer_email)
-        if other_noncompliance_reason is not None:
-            pulumi.set(__self__, "other_noncompliance_reason", other_noncompliance_reason)
-        if peer_reviewed_by is not None:
-            pulumi.set(__self__, "peer_reviewed_by", peer_reviewed_by)
-        if ticket_id is not None:
-            pulumi.set(__self__, "ticket_id", ticket_id)
-        if unit_tested is not None:
-            pulumi.set(__self__, "unit_tested", unit_tested)
-
-    @property
-    @pulumi.getter(name="noncomplianceReason")
-    def noncompliance_reason(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "noncompliance_reason")
-
-    @noncompliance_reason.setter
-    def noncompliance_reason(self, value: pulumi.Input[str]):
-        pulumi.set(self, "noncompliance_reason", value)
-
-    @property
-    @pulumi.getter(name="customerEmail")
-    def customer_email(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "customer_email")
-
-    @customer_email.setter
-    def customer_email(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "customer_email", value)
-
-    @property
-    @pulumi.getter(name="otherNoncomplianceReason")
-    def other_noncompliance_reason(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "other_noncompliance_reason")
-
-    @other_noncompliance_reason.setter
-    def other_noncompliance_reason(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "other_noncompliance_reason", value)
-
-    @property
-    @pulumi.getter(name="peerReviewedBy")
-    def peer_reviewed_by(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "peer_reviewed_by")
-
-    @peer_reviewed_by.setter
-    def peer_reviewed_by(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "peer_reviewed_by", value)
-
-    @property
-    @pulumi.getter(name="ticketId")
-    def ticket_id(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "ticket_id")
-
-    @ticket_id.setter
-    def ticket_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "ticket_id", value)
-
-    @property
-    @pulumi.getter(name="unitTested")
-    def unit_tested(self) -> Optional[pulumi.Input[bool]]:
-        return pulumi.get(self, "unit_tested")
-
-    @unit_tested.setter
-    def unit_tested(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "unit_tested", value)
-
-
-@pulumi.input_type
-class PropertyActivationRuleErrorArgs:
-    def __init__(__self__, *,
-                 behavior_name: Optional[pulumi.Input[str]] = None,
-                 detail: Optional[pulumi.Input[str]] = None,
-                 error_location: Optional[pulumi.Input[str]] = None,
-                 instance: Optional[pulumi.Input[str]] = None,
-                 status_code: Optional[pulumi.Input[int]] = None,
-                 title: Optional[pulumi.Input[str]] = None,
-                 type: Optional[pulumi.Input[str]] = None):
-        if behavior_name is not None:
-            pulumi.set(__self__, "behavior_name", behavior_name)
-        if detail is not None:
-            pulumi.set(__self__, "detail", detail)
-        if error_location is not None:
-            pulumi.set(__self__, "error_location", error_location)
-        if instance is not None:
-            pulumi.set(__self__, "instance", instance)
-        if status_code is not None:
-            pulumi.set(__self__, "status_code", status_code)
-        if title is not None:
-            pulumi.set(__self__, "title", title)
-        if type is not None:
-            pulumi.set(__self__, "type", type)
-
-    @property
-    @pulumi.getter(name="behaviorName")
-    def behavior_name(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "behavior_name")
-
-    @behavior_name.setter
-    def behavior_name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "behavior_name", value)
-
-    @property
-    @pulumi.getter
-    def detail(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "detail")
-
-    @detail.setter
-    def detail(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "detail", value)
-
-    @property
-    @pulumi.getter(name="errorLocation")
-    def error_location(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "error_location")
-
-    @error_location.setter
-    def error_location(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "error_location", value)
-
-    @property
-    @pulumi.getter
-    def instance(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "instance")
-
-    @instance.setter
-    def instance(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "instance", value)
-
-    @property
-    @pulumi.getter(name="statusCode")
-    def status_code(self) -> Optional[pulumi.Input[int]]:
-        return pulumi.get(self, "status_code")
-
-    @status_code.setter
-    def status_code(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "status_code", value)
-
-    @property
-    @pulumi.getter
-    def title(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "title")
-
-    @title.setter
-    def title(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "title", value)
-
-    @property
-    @pulumi.getter
-    def type(self) -> Optional[pulumi.Input[str]]:
+                 contract_id: pulumi.Input[str],
+                 group_id: pulumi.Input[str],
+                 rule_format: pulumi.Input[str],
+                 type: pulumi.Input[str],
+                 name: Optional[pulumi.Input[str]] = None,
+                 product_id: Optional[pulumi.Input[str]] = None,
+                 rules: Optional[pulumi.Input[str]] = None):
+        """
+        The set of arguments for constructing a PropertyInclude resource.
+        :param pulumi.Input[str] contract_id: Identifies the contract to which the include is assigned
+        :param pulumi.Input[str] group_id: Identifies the group to which the include is assigned
+        :param pulumi.Input[str] rule_format: Indicates the versioned set of features and criteria
+        :param pulumi.Input[str] type: Specifies the type of the include, either 'MICROSERVICES' or 'COMMON_SETTINGS'
+        :param pulumi.Input[str] name: A descriptive name for the include
+        :param pulumi.Input[str] product_id: The product assigned to the include
+        :param pulumi.Input[str] rules: Property Rules as JSON
+        """
+        pulumi.set(__self__, "contract_id", contract_id)
+        pulumi.set(__self__, "group_id", group_id)
+        pulumi.set(__self__, "rule_format", rule_format)
+        pulumi.set(__self__, "type", type)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if product_id is not None:
+            pulumi.set(__self__, "product_id", product_id)
+        if rules is not None:
+            pulumi.set(__self__, "rules", rules)
+
+    @property
+    @pulumi.getter(name="contractId")
+    def contract_id(self) -> pulumi.Input[str]:
+        """
+        Identifies the contract to which the include is assigned
+        """
+        return pulumi.get(self, "contract_id")
+
+    @contract_id.setter
+    def contract_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "contract_id", value)
+
+    @property
+    @pulumi.getter(name="groupId")
+    def group_id(self) -> pulumi.Input[str]:
+        """
+        Identifies the group to which the include is assigned
+        """
+        return pulumi.get(self, "group_id")
+
+    @group_id.setter
+    def group_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "group_id", value)
+
+    @property
+    @pulumi.getter(name="ruleFormat")
+    def rule_format(self) -> pulumi.Input[str]:
+        """
+        Indicates the versioned set of features and criteria
+        """
+        return pulumi.get(self, "rule_format")
+
+    @rule_format.setter
+    def rule_format(self, value: pulumi.Input[str]):
+        pulumi.set(self, "rule_format", value)
+
+    @property
+    @pulumi.getter
+    def type(self) -> pulumi.Input[str]:
+        """
+        Specifies the type of the include, either 'MICROSERVICES' or 'COMMON_SETTINGS'
+        """
         return pulumi.get(self, "type")
 
     @type.setter
-    def type(self, value: Optional[pulumi.Input[str]]):
+    def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
-
-@pulumi.input_type
-class PropertyActivationRuleWarningArgs:
-    def __init__(__self__, *,
-                 behavior_name: Optional[pulumi.Input[str]] = None,
-                 detail: Optional[pulumi.Input[str]] = None,
-                 error_location: Optional[pulumi.Input[str]] = None,
-                 instance: Optional[pulumi.Input[str]] = None,
-                 status_code: Optional[pulumi.Input[int]] = None,
-                 title: Optional[pulumi.Input[str]] = None,
-                 type: Optional[pulumi.Input[str]] = None):
-        if behavior_name is not None:
-            pulumi.set(__self__, "behavior_name", behavior_name)
-        if detail is not None:
-            pulumi.set(__self__, "detail", detail)
-        if error_location is not None:
-            pulumi.set(__self__, "error_location", error_location)
-        if instance is not None:
-            pulumi.set(__self__, "instance", instance)
-        if status_code is not None:
-            pulumi.set(__self__, "status_code", status_code)
-        if title is not None:
-            pulumi.set(__self__, "title", title)
-        if type is not None:
-            pulumi.set(__self__, "type", type)
-
-    @property
-    @pulumi.getter(name="behaviorName")
-    def behavior_name(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "behavior_name")
-
-    @behavior_name.setter
-    def behavior_name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "behavior_name", value)
-
-    @property
-    @pulumi.getter
-    def detail(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "detail")
-
-    @detail.setter
-    def detail(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "detail", value)
-
-    @property
-    @pulumi.getter(name="errorLocation")
-    def error_location(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "error_location")
-
-    @error_location.setter
-    def error_location(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "error_location", value)
-
     @property
     @pulumi.getter
-    def instance(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "instance")
-
-    @instance.setter
-    def instance(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "instance", value)
-
-    @property
-    @pulumi.getter(name="statusCode")
-    def status_code(self) -> Optional[pulumi.Input[int]]:
-        return pulumi.get(self, "status_code")
-
-    @status_code.setter
-    def status_code(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "status_code", value)
+    def name(self) -> Optional[pulumi.Input[str]]:
+        """
+        A descriptive name for the include
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
+
+    @property
+    @pulumi.getter(name="productId")
+    def product_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        The product assigned to the include
+        """
+        return pulumi.get(self, "product_id")
+
+    @product_id.setter
+    def product_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "product_id", value)
 
     @property
     @pulumi.getter
-    def title(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "title")
-
-    @title.setter
-    def title(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "title", value)
-
-    @property
-    @pulumi.getter
-    def type(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "type")
-
-    @type.setter
-    def type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "type", value)
+    def rules(self) -> Optional[pulumi.Input[str]]:
+        """
+        Property Rules as JSON
+        """
+        return pulumi.get(self, "rules")
+
+    @rules.setter
+    def rules(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "rules", value)
 
 
 @pulumi.input_type
-class PropertyHostnameArgs:
+class _PropertyIncludeState:
     def __init__(__self__, *,
-                 cert_provisioning_type: pulumi.Input[str],
-                 cname_from: pulumi.Input[str],
-                 cname_to: pulumi.Input[str],
-                 cert_statuses: Optional[pulumi.Input[Sequence[pulumi.Input['PropertyHostnameCertStatusArgs']]]] = None,
-                 cname_type: Optional[pulumi.Input[str]] = None,
-                 edge_hostname_id: Optional[pulumi.Input[str]] = None):
-        pulumi.set(__self__, "cert_provisioning_type", cert_provisioning_type)
-        pulumi.set(__self__, "cname_from", cname_from)
-        pulumi.set(__self__, "cname_to", cname_to)
-        if cert_statuses is not None:
-            pulumi.set(__self__, "cert_statuses", cert_statuses)
-        if cname_type is not None:
-            pulumi.set(__self__, "cname_type", cname_type)
-        if edge_hostname_id is not None:
-            pulumi.set(__self__, "edge_hostname_id", edge_hostname_id)
-
-    @property
-    @pulumi.getter(name="certProvisioningType")
-    def cert_provisioning_type(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "cert_provisioning_type")
-
-    @cert_provisioning_type.setter
-    def cert_provisioning_type(self, value: pulumi.Input[str]):
-        pulumi.set(self, "cert_provisioning_type", value)
-
-    @property
-    @pulumi.getter(name="cnameFrom")
-    def cname_from(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "cname_from")
-
-    @cname_from.setter
-    def cname_from(self, value: pulumi.Input[str]):
-        pulumi.set(self, "cname_from", value)
-
-    @property
-    @pulumi.getter(name="cnameTo")
-    def cname_to(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "cname_to")
-
-    @cname_to.setter
-    def cname_to(self, value: pulumi.Input[str]):
-        pulumi.set(self, "cname_to", value)
-
-    @property
-    @pulumi.getter(name="certStatuses")
-    def cert_statuses(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PropertyHostnameCertStatusArgs']]]]:
-        return pulumi.get(self, "cert_statuses")
-
-    @cert_statuses.setter
-    def cert_statuses(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PropertyHostnameCertStatusArgs']]]]):
-        pulumi.set(self, "cert_statuses", value)
-
-    @property
-    @pulumi.getter(name="cnameType")
-    def cname_type(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "cname_type")
-
-    @cname_type.setter
-    def cname_type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "cname_type", value)
-
-    @property
-    @pulumi.getter(name="edgeHostnameId")
-    def edge_hostname_id(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "edge_hostname_id")
-
-    @edge_hostname_id.setter
-    def edge_hostname_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "edge_hostname_id", value)
-
-
-@pulumi.input_type
-class PropertyHostnameCertStatusArgs:
-    def __init__(__self__, *,
-                 hostname: Optional[pulumi.Input[str]] = None,
-                 production_status: Optional[pulumi.Input[str]] = None,
-                 staging_status: Optional[pulumi.Input[str]] = None,
-                 target: Optional[pulumi.Input[str]] = None):
-        if hostname is not None:
-            pulumi.set(__self__, "hostname", hostname)
-        if production_status is not None:
-            pulumi.set(__self__, "production_status", production_status)
-        if staging_status is not None:
-            pulumi.set(__self__, "staging_status", staging_status)
-        if target is not None:
-            pulumi.set(__self__, "target", target)
-
-    @property
-    @pulumi.getter
-    def hostname(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "hostname")
-
-    @hostname.setter
-    def hostname(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "hostname", value)
-
-    @property
-    @pulumi.getter(name="productionStatus")
-    def production_status(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "production_status")
-
-    @production_status.setter
-    def production_status(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "production_status", value)
-
-    @property
-    @pulumi.getter(name="stagingStatus")
-    def staging_status(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "staging_status")
-
-    @staging_status.setter
-    def staging_status(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "staging_status", value)
-
-    @property
-    @pulumi.getter
-    def target(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "target")
-
-    @target.setter
-    def target(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "target", value)
-
-
-@pulumi.input_type
-class PropertyOriginArgs:
-    def __init__(__self__, *,
-                 cache_key_hostname: Optional[pulumi.Input[str]] = None,
-                 compress: Optional[pulumi.Input[bool]] = None,
-                 enable_true_client_ip: Optional[pulumi.Input[bool]] = None,
-                 forward_hostname: Optional[pulumi.Input[str]] = None,
-                 hostname: Optional[pulumi.Input[str]] = None,
-                 port: Optional[pulumi.Input[int]] = None):
-        if cache_key_hostname is not None:
-            pulumi.set(__self__, "cache_key_hostname", cache_key_hostname)
-        if compress is not None:
-            pulumi.set(__self__, "compress", compress)
-        if enable_true_client_ip is not None:
-            pulumi.set(__self__, "enable_true_client_ip", enable_true_client_ip)
-        if forward_hostname is not None:
-            pulumi.set(__self__, "forward_hostname", forward_hostname)
-        if hostname is not None:
-            pulumi.set(__self__, "hostname", hostname)
-        if port is not None:
-            pulumi.set(__self__, "port", port)
-
-    @property
-    @pulumi.getter(name="cacheKeyHostname")
-    def cache_key_hostname(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "cache_key_hostname")
-
-    @cache_key_hostname.setter
-    def cache_key_hostname(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "cache_key_hostname", value)
-
-    @property
-    @pulumi.getter
-    def compress(self) -> Optional[pulumi.Input[bool]]:
-        return pulumi.get(self, "compress")
-
-    @compress.setter
-    def compress(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "compress", value)
-
-    @property
-    @pulumi.getter(name="enableTrueClientIp")
-    def enable_true_client_ip(self) -> Optional[pulumi.Input[bool]]:
-        return pulumi.get(self, "enable_true_client_ip")
-
-    @enable_true_client_ip.setter
-    def enable_true_client_ip(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "enable_true_client_ip", value)
-
-    @property
-    @pulumi.getter(name="forwardHostname")
-    def forward_hostname(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "forward_hostname")
-
-    @forward_hostname.setter
-    def forward_hostname(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "forward_hostname", value)
-
-    @property
-    @pulumi.getter
-    def hostname(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "hostname")
-
-    @hostname.setter
-    def hostname(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "hostname", value)
-
-    @property
-    @pulumi.getter
-    def port(self) -> Optional[pulumi.Input[int]]:
-        return pulumi.get(self, "port")
-
-    @port.setter
-    def port(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "port", value)
-
-
-@pulumi.input_type
-class PropertyRuleErrorArgs:
-    def __init__(__self__, *,
-                 behavior_name: Optional[pulumi.Input[str]] = None,
-                 detail: Optional[pulumi.Input[str]] = None,
-                 error_location: Optional[pulumi.Input[str]] = None,
-                 instance: Optional[pulumi.Input[str]] = None,
-                 status_code: Optional[pulumi.Input[int]] = None,
-                 title: Optional[pulumi.Input[str]] = None,
+                 contract_id: Optional[pulumi.Input[str]] = None,
+                 group_id: Optional[pulumi.Input[str]] = None,
+                 latest_version: Optional[pulumi.Input[int]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 product_id: Optional[pulumi.Input[str]] = None,
+                 production_version: Optional[pulumi.Input[str]] = None,
+                 rule_errors: Optional[pulumi.Input[str]] = None,
+                 rule_format: Optional[pulumi.Input[str]] = None,
+                 rule_warnings: Optional[pulumi.Input[str]] = None,
+                 rules: Optional[pulumi.Input[str]] = None,
+                 staging_version: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None):
-        if behavior_name is not None:
-            pulumi.set(__self__, "behavior_name", behavior_name)
-        if detail is not None:
-            pulumi.set(__self__, "detail", detail)
-        if error_location is not None:
-            pulumi.set(__self__, "error_location", error_location)
-        if instance is not None:
-            pulumi.set(__self__, "instance", instance)
-        if status_code is not None:
-            pulumi.set(__self__, "status_code", status_code)
-        if title is not None:
-            pulumi.set(__self__, "title", title)
+        """
+        Input properties used for looking up and filtering PropertyInclude resources.
+        :param pulumi.Input[str] contract_id: Identifies the contract to which the include is assigned
+        :param pulumi.Input[str] group_id: Identifies the group to which the include is assigned
+        :param pulumi.Input[int] latest_version: Specifies the most recent version of the include
+        :param pulumi.Input[str] name: A descriptive name for the include
+        :param pulumi.Input[str] product_id: The product assigned to the include
+        :param pulumi.Input[str] production_version: The most recent version to be activated to the production network
+        :param pulumi.Input[str] rule_errors: Rule validation errors
+        :param pulumi.Input[str] rule_format: Indicates the versioned set of features and criteria
+        :param pulumi.Input[str] rule_warnings: Rule validation warnings
+        :param pulumi.Input[str] rules: Property Rules as JSON
+        :param pulumi.Input[str] staging_version: The most recent version to be activated to the staging network
+        :param pulumi.Input[str] type: Specifies the type of the include, either 'MICROSERVICES' or 'COMMON_SETTINGS'
+        """
+        if contract_id is not None:
+            pulumi.set(__self__, "contract_id", contract_id)
+        if group_id is not None:
+            pulumi.set(__self__, "group_id", group_id)
+        if latest_version is not None:
+            pulumi.set(__self__, "latest_version", latest_version)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if product_id is not None:
+            pulumi.set(__self__, "product_id", product_id)
+        if production_version is not None:
+            pulumi.set(__self__, "production_version", production_version)
+        if rule_errors is not None:
+            pulumi.set(__self__, "rule_errors", rule_errors)
+        if rule_format is not None:
+            pulumi.set(__self__, "rule_format", rule_format)
+        if rule_warnings is not None:
+            pulumi.set(__self__, "rule_warnings", rule_warnings)
+        if rules is not None:
+            pulumi.set(__self__, "rules", rules)
+        if staging_version is not None:
+            pulumi.set(__self__, "staging_version", staging_version)
         if type is not None:
             pulumi.set(__self__, "type", type)
 
     @property
-    @pulumi.getter(name="behaviorName")
-    def behavior_name(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "behavior_name")
-
-    @behavior_name.setter
-    def behavior_name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "behavior_name", value)
+    @pulumi.getter(name="contractId")
+    def contract_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        Identifies the contract to which the include is assigned
+        """
+        return pulumi.get(self, "contract_id")
+
+    @contract_id.setter
+    def contract_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "contract_id", value)
 
     @property
-    @pulumi.getter
-    def detail(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "detail")
+    @pulumi.getter(name="groupId")
+    def group_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        Identifies the group to which the include is assigned
+        """
+        return pulumi.get(self, "group_id")
 
-    @detail.setter
-    def detail(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "detail", value)
+    @group_id.setter
+    def group_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "group_id", value)
 
     @property
-    @pulumi.getter(name="errorLocation")
-    def error_location(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "error_location")
+    @pulumi.getter(name="latestVersion")
+    def latest_version(self) -> Optional[pulumi.Input[int]]:
+        """
+        Specifies the most recent version of the include
+        """
+        return pulumi.get(self, "latest_version")
 
-    @error_location.setter
-    def error_location(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "error_location", value)
+    @latest_version.setter
+    def latest_version(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "latest_version", value)
 
     @property
     @pulumi.getter
-    def instance(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "instance")
+    def name(self) -> Optional[pulumi.Input[str]]:
+        """
+        A descriptive name for the include
+        """
+        return pulumi.get(self, "name")
 
-    @instance.setter
-    def instance(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "instance", value)
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter(name="statusCode")
-    def status_code(self) -> Optional[pulumi.Input[int]]:
-        return pulumi.get(self, "status_code")
+    @pulumi.getter(name="productId")
+    def product_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        The product assigned to the include
+        """
+        return pulumi.get(self, "product_id")
 
-    @status_code.setter
-    def status_code(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "status_code", value)
+    @product_id.setter
+    def product_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "product_id", value)
 
     @property
-    @pulumi.getter
-    def title(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "title")
+    @pulumi.getter(name="productionVersion")
+    def production_version(self) -> Optional[pulumi.Input[str]]:
+        """
+        The most recent version to be activated to the production network
+        """
+        return pulumi.get(self, "production_version")
 
-    @title.setter
-    def title(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "title", value)
+    @production_version.setter
+    def production_version(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "production_version", value)
 
     @property
-    @pulumi.getter
-    def type(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "type")
-
-    @type.setter
-    def type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "type", value)
-
-
-@pulumi.input_type
-class PropertyRuleWarningArgs:
-    def __init__(__self__, *,
-                 behavior_name: Optional[pulumi.Input[str]] = None,
-                 detail: Optional[pulumi.Input[str]] = None,
-                 error_location: Optional[pulumi.Input[str]] = None,
-                 instance: Optional[pulumi.Input[str]] = None,
-                 status_code: Optional[pulumi.Input[int]] = None,
-                 title: Optional[pulumi.Input[str]] = None,
-                 type: Optional[pulumi.Input[str]] = None):
-        if behavior_name is not None:
-            pulumi.set(__self__, "behavior_name", behavior_name)
-        if detail is not None:
-            pulumi.set(__self__, "detail", detail)
-        if error_location is not None:
-            pulumi.set(__self__, "error_location", error_location)
-        if instance is not None:
-            pulumi.set(__self__, "instance", instance)
-        if status_code is not None:
-            pulumi.set(__self__, "status_code", status_code)
-        if title is not None:
-            pulumi.set(__self__, "title", title)
-        if type is not None:
-            pulumi.set(__self__, "type", type)
+    @pulumi.getter(name="ruleErrors")
+    def rule_errors(self) -> Optional[pulumi.Input[str]]:
+        """
+        Rule validation errors
+        """
+        return pulumi.get(self, "rule_errors")
 
-    @property
-    @pulumi.getter(name="behaviorName")
-    def behavior_name(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "behavior_name")
-
-    @behavior_name.setter
-    def behavior_name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "behavior_name", value)
+    @rule_errors.setter
+    def rule_errors(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "rule_errors", value)
 
     @property
-    @pulumi.getter
-    def detail(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "detail")
+    @pulumi.getter(name="ruleFormat")
+    def rule_format(self) -> Optional[pulumi.Input[str]]:
+        """
+        Indicates the versioned set of features and criteria
+        """
+        return pulumi.get(self, "rule_format")
 
-    @detail.setter
-    def detail(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "detail", value)
+    @rule_format.setter
+    def rule_format(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "rule_format", value)
 
     @property
-    @pulumi.getter(name="errorLocation")
-    def error_location(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "error_location")
+    @pulumi.getter(name="ruleWarnings")
+    def rule_warnings(self) -> Optional[pulumi.Input[str]]:
+        """
+        Rule validation warnings
+        """
+        return pulumi.get(self, "rule_warnings")
 
-    @error_location.setter
-    def error_location(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "error_location", value)
+    @rule_warnings.setter
+    def rule_warnings(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "rule_warnings", value)
 
     @property
     @pulumi.getter
-    def instance(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "instance")
-
-    @instance.setter
-    def instance(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "instance", value)
+    def rules(self) -> Optional[pulumi.Input[str]]:
+        """
+        Property Rules as JSON
+        """
+        return pulumi.get(self, "rules")
 
-    @property
-    @pulumi.getter(name="statusCode")
-    def status_code(self) -> Optional[pulumi.Input[int]]:
-        return pulumi.get(self, "status_code")
-
-    @status_code.setter
-    def status_code(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "status_code", value)
+    @rules.setter
+    def rules(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "rules", value)
 
     @property
-    @pulumi.getter
-    def title(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "title")
+    @pulumi.getter(name="stagingVersion")
+    def staging_version(self) -> Optional[pulumi.Input[str]]:
+        """
+        The most recent version to be activated to the staging network
+        """
+        return pulumi.get(self, "staging_version")
 
-    @title.setter
-    def title(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "title", value)
+    @staging_version.setter
+    def staging_version(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "staging_version", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
+        """
+        Specifies the type of the include, either 'MICROSERVICES' or 'COMMON_SETTINGS'
+        """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
 
+class PropertyInclude(pulumi.CustomResource):
+    @overload
+    def __init__(__self__,
+                 resource_name: str,
+                 opts: Optional[pulumi.ResourceOptions] = None,
+                 contract_id: Optional[pulumi.Input[str]] = None,
+                 group_id: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 product_id: Optional[pulumi.Input[str]] = None,
+                 rule_format: Optional[pulumi.Input[str]] = None,
+                 rules: Optional[pulumi.Input[str]] = None,
+                 type: Optional[pulumi.Input[str]] = None,
+                 __props__=None):
+        """
+        Create a PropertyInclude resource with the given unique name, props, and options.
+        :param str resource_name: The name of the resource.
+        :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] contract_id: Identifies the contract to which the include is assigned
+        :param pulumi.Input[str] group_id: Identifies the group to which the include is assigned
+        :param pulumi.Input[str] name: A descriptive name for the include
+        :param pulumi.Input[str] product_id: The product assigned to the include
+        :param pulumi.Input[str] rule_format: Indicates the versioned set of features and criteria
+        :param pulumi.Input[str] rules: Property Rules as JSON
+        :param pulumi.Input[str] type: Specifies the type of the include, either 'MICROSERVICES' or 'COMMON_SETTINGS'
+        """
+        ...
+    @overload
+    def __init__(__self__,
+                 resource_name: str,
+                 args: PropertyIncludeArgs,
+                 opts: Optional[pulumi.ResourceOptions] = None):
+        """
+        Create a PropertyInclude resource with the given unique name, props, and options.
+        :param str resource_name: The name of the resource.
+        :param PropertyIncludeArgs args: The arguments to use to populate this resource's properties.
+        :param pulumi.ResourceOptions opts: Options for the resource.
+        """
+        ...
+    def __init__(__self__, resource_name: str, *args, **kwargs):
+        resource_args, opts = _utilities.get_resource_args_opts(PropertyIncludeArgs, pulumi.ResourceOptions, *args, **kwargs)
+        if resource_args is not None:
+            __self__._internal_init(resource_name, opts, **resource_args.__dict__)
+        else:
+            __self__._internal_init(resource_name, *args, **kwargs)
+
+    def _internal_init(__self__,
+                 resource_name: str,
+                 opts: Optional[pulumi.ResourceOptions] = None,
+                 contract_id: Optional[pulumi.Input[str]] = None,
+                 group_id: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 product_id: Optional[pulumi.Input[str]] = None,
+                 rule_format: Optional[pulumi.Input[str]] = None,
+                 rules: Optional[pulumi.Input[str]] = None,
+                 type: Optional[pulumi.Input[str]] = None,
+                 __props__=None):
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
+        if not isinstance(opts, pulumi.ResourceOptions):
+            raise TypeError('Expected resource options to be a ResourceOptions instance')
+        if opts.id is None:
+            if __props__ is not None:
+                raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
+            __props__ = PropertyIncludeArgs.__new__(PropertyIncludeArgs)
+
+            if contract_id is None and not opts.urn:
+                raise TypeError("Missing required property 'contract_id'")
+            __props__.__dict__["contract_id"] = contract_id
+            if group_id is None and not opts.urn:
+                raise TypeError("Missing required property 'group_id'")
+            __props__.__dict__["group_id"] = group_id
+            __props__.__dict__["name"] = name
+            __props__.__dict__["product_id"] = product_id
+            if rule_format is None and not opts.urn:
+                raise TypeError("Missing required property 'rule_format'")
+            __props__.__dict__["rule_format"] = rule_format
+            __props__.__dict__["rules"] = rules
+            if type is None and not opts.urn:
+                raise TypeError("Missing required property 'type'")
+            __props__.__dict__["type"] = type
+            __props__.__dict__["latest_version"] = None
+            __props__.__dict__["production_version"] = None
+            __props__.__dict__["rule_errors"] = None
+            __props__.__dict__["rule_warnings"] = None
+            __props__.__dict__["staging_version"] = None
+        super(PropertyInclude, __self__).__init__(
+            'akamai:index/propertyInclude:PropertyInclude',
+            resource_name,
+            __props__,
+            opts)
+
+    @staticmethod
+    def get(resource_name: str,
+            id: pulumi.Input[str],
+            opts: Optional[pulumi.ResourceOptions] = None,
+            contract_id: Optional[pulumi.Input[str]] = None,
+            group_id: Optional[pulumi.Input[str]] = None,
+            latest_version: Optional[pulumi.Input[int]] = None,
+            name: Optional[pulumi.Input[str]] = None,
+            product_id: Optional[pulumi.Input[str]] = None,
+            production_version: Optional[pulumi.Input[str]] = None,
+            rule_errors: Optional[pulumi.Input[str]] = None,
+            rule_format: Optional[pulumi.Input[str]] = None,
+            rule_warnings: Optional[pulumi.Input[str]] = None,
+            rules: Optional[pulumi.Input[str]] = None,
+            staging_version: Optional[pulumi.Input[str]] = None,
+            type: Optional[pulumi.Input[str]] = None) -> 'PropertyInclude':
+        """
+        Get an existing PropertyInclude resource's state with the given name, id, and optional extra
+        properties used to qualify the lookup.
+
+        :param str resource_name: The unique name of the resulting resource.
+        :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
+        :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] contract_id: Identifies the contract to which the include is assigned
+        :param pulumi.Input[str] group_id: Identifies the group to which the include is assigned
+        :param pulumi.Input[int] latest_version: Specifies the most recent version of the include
+        :param pulumi.Input[str] name: A descriptive name for the include
+        :param pulumi.Input[str] product_id: The product assigned to the include
+        :param pulumi.Input[str] production_version: The most recent version to be activated to the production network
+        :param pulumi.Input[str] rule_errors: Rule validation errors
+        :param pulumi.Input[str] rule_format: Indicates the versioned set of features and criteria
+        :param pulumi.Input[str] rule_warnings: Rule validation warnings
+        :param pulumi.Input[str] rules: Property Rules as JSON
+        :param pulumi.Input[str] staging_version: The most recent version to be activated to the staging network
+        :param pulumi.Input[str] type: Specifies the type of the include, either 'MICROSERVICES' or 'COMMON_SETTINGS'
+        """
+        opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
+
+        __props__ = _PropertyIncludeState.__new__(_PropertyIncludeState)
+
+        __props__.__dict__["contract_id"] = contract_id
+        __props__.__dict__["group_id"] = group_id
+        __props__.__dict__["latest_version"] = latest_version
+        __props__.__dict__["name"] = name
+        __props__.__dict__["product_id"] = product_id
+        __props__.__dict__["production_version"] = production_version
+        __props__.__dict__["rule_errors"] = rule_errors
+        __props__.__dict__["rule_format"] = rule_format
+        __props__.__dict__["rule_warnings"] = rule_warnings
+        __props__.__dict__["rules"] = rules
+        __props__.__dict__["staging_version"] = staging_version
+        __props__.__dict__["type"] = type
+        return PropertyInclude(resource_name, opts=opts, __props__=__props__)
+
+    @property
+    @pulumi.getter(name="contractId")
+    def contract_id(self) -> pulumi.Output[str]:
+        """
+        Identifies the contract to which the include is assigned
+        """
+        return pulumi.get(self, "contract_id")
+
+    @property
+    @pulumi.getter(name="groupId")
+    def group_id(self) -> pulumi.Output[str]:
+        """
+        Identifies the group to which the include is assigned
+        """
+        return pulumi.get(self, "group_id")
+
+    @property
+    @pulumi.getter(name="latestVersion")
+    def latest_version(self) -> pulumi.Output[int]:
+        """
+        Specifies the most recent version of the include
+        """
+        return pulumi.get(self, "latest_version")
+
+    @property
+    @pulumi.getter
+    def name(self) -> pulumi.Output[str]:
+        """
+        A descriptive name for the include
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter(name="productId")
+    def product_id(self) -> pulumi.Output[Optional[str]]:
+        """
+        The product assigned to the include
+        """
+        return pulumi.get(self, "product_id")
+
+    @property
+    @pulumi.getter(name="productionVersion")
+    def production_version(self) -> pulumi.Output[str]:
+        """
+        The most recent version to be activated to the production network
+        """
+        return pulumi.get(self, "production_version")
+
+    @property
+    @pulumi.getter(name="ruleErrors")
+    def rule_errors(self) -> pulumi.Output[str]:
+        """
+        Rule validation errors
+        """
+        return pulumi.get(self, "rule_errors")
+
+    @property
+    @pulumi.getter(name="ruleFormat")
+    def rule_format(self) -> pulumi.Output[str]:
+        """
+        Indicates the versioned set of features and criteria
+        """
+        return pulumi.get(self, "rule_format")
+
+    @property
+    @pulumi.getter(name="ruleWarnings")
+    def rule_warnings(self) -> pulumi.Output[str]:
+        """
+        Rule validation warnings
+        """
+        return pulumi.get(self, "rule_warnings")
+
+    @property
+    @pulumi.getter
+    def rules(self) -> pulumi.Output[str]:
+        """
+        Property Rules as JSON
+        """
+        return pulumi.get(self, "rules")
+
+    @property
+    @pulumi.getter(name="stagingVersion")
+    def staging_version(self) -> pulumi.Output[str]:
+        """
+        The most recent version to be activated to the staging network
+        """
+        return pulumi.get(self, "staging_version")
+
+    @property
+    @pulumi.getter
+    def type(self) -> pulumi.Output[str]:
+        """
+        Specifies the type of the include, either 'MICROSERVICES' or 'COMMON_SETTINGS'
+        """
+        return pulumi.get(self, "type")
+
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/properties/edge_host_name.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/provider.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,529 +3,478 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from .. import _utilities
+from . import _utilities
+from ._inputs import *
 
-__all__ = ['EdgeHostNameArgs', 'EdgeHostName']
+__all__ = ['ProviderArgs', 'Provider']
 
 @pulumi.input_type
-class EdgeHostNameArgs:
+class ProviderArgs:
     def __init__(__self__, *,
-                 edge_hostname: pulumi.Input[str],
-                 ip_behavior: pulumi.Input[str],
-                 certificate: Optional[pulumi.Input[int]] = None,
-                 contract: Optional[pulumi.Input[str]] = None,
-                 contract_id: Optional[pulumi.Input[str]] = None,
-                 group: Optional[pulumi.Input[str]] = None,
-                 group_id: Optional[pulumi.Input[str]] = None,
-                 product: Optional[pulumi.Input[str]] = None,
-                 product_id: Optional[pulumi.Input[str]] = None,
-                 status_update_emails: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 use_cases: Optional[pulumi.Input[str]] = None):
-        """
-        The set of arguments for constructing a EdgeHostName resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] status_update_emails: Email address that should receive updates on the IP behavior update request. Required for update operation.
-        :param pulumi.Input[str] use_cases: A JSON encoded list of use cases
-        """
-        pulumi.set(__self__, "edge_hostname", edge_hostname)
-        pulumi.set(__self__, "ip_behavior", ip_behavior)
-        if certificate is not None:
-            pulumi.set(__self__, "certificate", certificate)
-        if contract is not None:
-            warnings.warn("""The setting \"contract\" has been deprecated.""", DeprecationWarning)
-            pulumi.log.warn("""contract is deprecated: The setting \"contract\" has been deprecated.""")
-        if contract is not None:
-            pulumi.set(__self__, "contract", contract)
-        if contract_id is not None:
-            pulumi.set(__self__, "contract_id", contract_id)
-        if group is not None:
-            warnings.warn("""The setting \"group\" has been deprecated.""", DeprecationWarning)
-            pulumi.log.warn("""group is deprecated: The setting \"group\" has been deprecated.""")
-        if group is not None:
-            pulumi.set(__self__, "group", group)
-        if group_id is not None:
-            pulumi.set(__self__, "group_id", group_id)
-        if product is not None:
-            warnings.warn("""The setting \"product\" has been deprecated.""", DeprecationWarning)
-            pulumi.log.warn("""product is deprecated: The setting \"product\" has been deprecated.""")
-        if product is not None:
-            pulumi.set(__self__, "product", product)
-        if product_id is not None:
-            pulumi.set(__self__, "product_id", product_id)
-        if status_update_emails is not None:
-            pulumi.set(__self__, "status_update_emails", status_update_emails)
-        if use_cases is not None:
-            pulumi.set(__self__, "use_cases", use_cases)
-
-    @property
-    @pulumi.getter(name="edgeHostname")
-    def edge_hostname(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "edge_hostname")
-
-    @edge_hostname.setter
-    def edge_hostname(self, value: pulumi.Input[str]):
-        pulumi.set(self, "edge_hostname", value)
-
-    @property
-    @pulumi.getter(name="ipBehavior")
-    def ip_behavior(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "ip_behavior")
-
-    @ip_behavior.setter
-    def ip_behavior(self, value: pulumi.Input[str]):
-        pulumi.set(self, "ip_behavior", value)
+                 appsec_section: Optional[pulumi.Input[str]] = None,
+                 appsecs: Optional[pulumi.Input[Sequence[pulumi.Input['ProviderAppsecArgs']]]] = None,
+                 cache_enabled: Optional[pulumi.Input[bool]] = None,
+                 config: Optional[pulumi.Input['ProviderConfigArgs']] = None,
+                 config_section: Optional[pulumi.Input[str]] = None,
+                 dns: Optional[pulumi.Input['ProviderDnsArgs']] = None,
+                 dns_section: Optional[pulumi.Input[str]] = None,
+                 edgerc: Optional[pulumi.Input[str]] = None,
+                 gtm: Optional[pulumi.Input['ProviderGtmArgs']] = None,
+                 gtm_section: Optional[pulumi.Input[str]] = None,
+                 networklist_section: Optional[pulumi.Input[str]] = None,
+                 networks: Optional[pulumi.Input[Sequence[pulumi.Input['ProviderNetworkArgs']]]] = None,
+                 papi_section: Optional[pulumi.Input[str]] = None,
+                 property: Optional[pulumi.Input['ProviderPropertyArgs']] = None,
+                 property_section: Optional[pulumi.Input[str]] = None,
+                 request_limit: Optional[pulumi.Input[int]] = None):
+        """
+        The set of arguments for constructing a Provider resource.
+        :param pulumi.Input[str] config_section: The section of the edgerc file to use for configuration
+        :param pulumi.Input[int] request_limit: The maximum number of API requests to be made per second (0 for no limit)
+        """
+        if appsec_section is not None:
+            warnings.warn("""The setting \"appsec_section\" has been deprecated.""", DeprecationWarning)
+            pulumi.log.warn("""appsec_section is deprecated: The setting \"appsec_section\" has been deprecated.""")
+        if appsec_section is not None:
+            pulumi.set(__self__, "appsec_section", appsec_section)
+        if appsecs is not None:
+            warnings.warn("""The setting \"appsec\" has been deprecated.""", DeprecationWarning)
+            pulumi.log.warn("""appsecs is deprecated: The setting \"appsec\" has been deprecated.""")
+        if appsecs is not None:
+            pulumi.set(__self__, "appsecs", appsecs)
+        if cache_enabled is not None:
+            pulumi.set(__self__, "cache_enabled", cache_enabled)
+        if config is not None:
+            pulumi.set(__self__, "config", config)
+        if config_section is not None:
+            pulumi.set(__self__, "config_section", config_section)
+        if dns is not None:
+            warnings.warn("""The setting \"dns\" has been deprecated.""", DeprecationWarning)
+            pulumi.log.warn("""dns is deprecated: The setting \"dns\" has been deprecated.""")
+        if dns is not None:
+            pulumi.set(__self__, "dns", dns)
+        if dns_section is not None:
+            warnings.warn("""The setting \"dns_section\" has been deprecated.""", DeprecationWarning)
+            pulumi.log.warn("""dns_section is deprecated: The setting \"dns_section\" has been deprecated.""")
+        if dns_section is not None:
+            pulumi.set(__self__, "dns_section", dns_section)
+        if edgerc is not None:
+            pulumi.set(__self__, "edgerc", edgerc)
+        if gtm is not None:
+            warnings.warn("""The setting \"gtm\" has been deprecated.""", DeprecationWarning)
+            pulumi.log.warn("""gtm is deprecated: The setting \"gtm\" has been deprecated.""")
+        if gtm is not None:
+            pulumi.set(__self__, "gtm", gtm)
+        if gtm_section is not None:
+            warnings.warn("""The setting \"gtm_section\" has been deprecated.""", DeprecationWarning)
+            pulumi.log.warn("""gtm_section is deprecated: The setting \"gtm_section\" has been deprecated.""")
+        if gtm_section is not None:
+            pulumi.set(__self__, "gtm_section", gtm_section)
+        if networklist_section is not None:
+            warnings.warn("""The setting \"networklist_section\" has been deprecated.""", DeprecationWarning)
+            pulumi.log.warn("""networklist_section is deprecated: The setting \"networklist_section\" has been deprecated.""")
+        if networklist_section is not None:
+            pulumi.set(__self__, "networklist_section", networklist_section)
+        if networks is not None:
+            pulumi.set(__self__, "networks", networks)
+        if papi_section is not None:
+            warnings.warn("""The setting \"papi_section\" has been deprecated.""", DeprecationWarning)
+            pulumi.log.warn("""papi_section is deprecated: The setting \"papi_section\" has been deprecated.""")
+        if papi_section is not None:
+            pulumi.set(__self__, "papi_section", papi_section)
+        if property is not None:
+            warnings.warn("""The setting \"property\" has been deprecated.""", DeprecationWarning)
+            pulumi.log.warn("""property is deprecated: The setting \"property\" has been deprecated.""")
+        if property is not None:
+            pulumi.set(__self__, "property", property)
+        if property_section is not None:
+            warnings.warn("""The setting \"property_section\" has been deprecated.""", DeprecationWarning)
+            pulumi.log.warn("""property_section is deprecated: The setting \"property_section\" has been deprecated.""")
+        if property_section is not None:
+            pulumi.set(__self__, "property_section", property_section)
+        if request_limit is not None:
+            pulumi.set(__self__, "request_limit", request_limit)
 
     @property
-    @pulumi.getter
-    def certificate(self) -> Optional[pulumi.Input[int]]:
-        return pulumi.get(self, "certificate")
+    @pulumi.getter(name="appsecSection")
+    def appsec_section(self) -> Optional[pulumi.Input[str]]:
+        warnings.warn("""The setting \"appsec_section\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""appsec_section is deprecated: The setting \"appsec_section\" has been deprecated.""")
+
+        return pulumi.get(self, "appsec_section")
 
-    @certificate.setter
-    def certificate(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "certificate", value)
+    @appsec_section.setter
+    def appsec_section(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "appsec_section", value)
 
     @property
     @pulumi.getter
-    def contract(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "contract")
+    def appsecs(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProviderAppsecArgs']]]]:
+        warnings.warn("""The setting \"appsec\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""appsecs is deprecated: The setting \"appsec\" has been deprecated.""")
 
-    @contract.setter
-    def contract(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "contract", value)
+        return pulumi.get(self, "appsecs")
+
+    @appsecs.setter
+    def appsecs(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ProviderAppsecArgs']]]]):
+        pulumi.set(self, "appsecs", value)
 
     @property
-    @pulumi.getter(name="contractId")
-    def contract_id(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "contract_id")
+    @pulumi.getter(name="cacheEnabled")
+    def cache_enabled(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "cache_enabled")
 
-    @contract_id.setter
-    def contract_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "contract_id", value)
+    @cache_enabled.setter
+    def cache_enabled(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "cache_enabled", value)
 
     @property
     @pulumi.getter
-    def group(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "group")
+    def config(self) -> Optional[pulumi.Input['ProviderConfigArgs']]:
+        return pulumi.get(self, "config")
 
-    @group.setter
-    def group(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "group", value)
+    @config.setter
+    def config(self, value: Optional[pulumi.Input['ProviderConfigArgs']]):
+        pulumi.set(self, "config", value)
 
     @property
-    @pulumi.getter(name="groupId")
-    def group_id(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "group_id")
+    @pulumi.getter(name="configSection")
+    def config_section(self) -> Optional[pulumi.Input[str]]:
+        """
+        The section of the edgerc file to use for configuration
+        """
+        return pulumi.get(self, "config_section")
 
-    @group_id.setter
-    def group_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "group_id", value)
+    @config_section.setter
+    def config_section(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "config_section", value)
 
     @property
     @pulumi.getter
-    def product(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "product")
+    def dns(self) -> Optional[pulumi.Input['ProviderDnsArgs']]:
+        warnings.warn("""The setting \"dns\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""dns is deprecated: The setting \"dns\" has been deprecated.""")
 
-    @product.setter
-    def product(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "product", value)
-
-    @property
-    @pulumi.getter(name="productId")
-    def product_id(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "product_id")
-
-    @product_id.setter
-    def product_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "product_id", value)
-
-    @property
-    @pulumi.getter(name="statusUpdateEmails")
-    def status_update_emails(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        Email address that should receive updates on the IP behavior update request. Required for update operation.
-        """
-        return pulumi.get(self, "status_update_emails")
+        return pulumi.get(self, "dns")
 
-    @status_update_emails.setter
-    def status_update_emails(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "status_update_emails", value)
+    @dns.setter
+    def dns(self, value: Optional[pulumi.Input['ProviderDnsArgs']]):
+        pulumi.set(self, "dns", value)
 
     @property
-    @pulumi.getter(name="useCases")
-    def use_cases(self) -> Optional[pulumi.Input[str]]:
-        """
-        A JSON encoded list of use cases
-        """
-        return pulumi.get(self, "use_cases")
+    @pulumi.getter(name="dnsSection")
+    def dns_section(self) -> Optional[pulumi.Input[str]]:
+        warnings.warn("""The setting \"dns_section\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""dns_section is deprecated: The setting \"dns_section\" has been deprecated.""")
 
-    @use_cases.setter
-    def use_cases(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "use_cases", value)
+        return pulumi.get(self, "dns_section")
 
-
-@pulumi.input_type
-class _EdgeHostNameState:
-    def __init__(__self__, *,
-                 certificate: Optional[pulumi.Input[int]] = None,
-                 contract: Optional[pulumi.Input[str]] = None,
-                 contract_id: Optional[pulumi.Input[str]] = None,
-                 edge_hostname: Optional[pulumi.Input[str]] = None,
-                 group: Optional[pulumi.Input[str]] = None,
-                 group_id: Optional[pulumi.Input[str]] = None,
-                 ip_behavior: Optional[pulumi.Input[str]] = None,
-                 product: Optional[pulumi.Input[str]] = None,
-                 product_id: Optional[pulumi.Input[str]] = None,
-                 status_update_emails: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 use_cases: Optional[pulumi.Input[str]] = None):
-        """
-        Input properties used for looking up and filtering EdgeHostName resources.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] status_update_emails: Email address that should receive updates on the IP behavior update request. Required for update operation.
-        :param pulumi.Input[str] use_cases: A JSON encoded list of use cases
-        """
-        if certificate is not None:
-            pulumi.set(__self__, "certificate", certificate)
-        if contract is not None:
-            warnings.warn("""The setting \"contract\" has been deprecated.""", DeprecationWarning)
-            pulumi.log.warn("""contract is deprecated: The setting \"contract\" has been deprecated.""")
-        if contract is not None:
-            pulumi.set(__self__, "contract", contract)
-        if contract_id is not None:
-            pulumi.set(__self__, "contract_id", contract_id)
-        if edge_hostname is not None:
-            pulumi.set(__self__, "edge_hostname", edge_hostname)
-        if group is not None:
-            warnings.warn("""The setting \"group\" has been deprecated.""", DeprecationWarning)
-            pulumi.log.warn("""group is deprecated: The setting \"group\" has been deprecated.""")
-        if group is not None:
-            pulumi.set(__self__, "group", group)
-        if group_id is not None:
-            pulumi.set(__self__, "group_id", group_id)
-        if ip_behavior is not None:
-            pulumi.set(__self__, "ip_behavior", ip_behavior)
-        if product is not None:
-            warnings.warn("""The setting \"product\" has been deprecated.""", DeprecationWarning)
-            pulumi.log.warn("""product is deprecated: The setting \"product\" has been deprecated.""")
-        if product is not None:
-            pulumi.set(__self__, "product", product)
-        if product_id is not None:
-            pulumi.set(__self__, "product_id", product_id)
-        if status_update_emails is not None:
-            pulumi.set(__self__, "status_update_emails", status_update_emails)
-        if use_cases is not None:
-            pulumi.set(__self__, "use_cases", use_cases)
+    @dns_section.setter
+    def dns_section(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "dns_section", value)
 
     @property
     @pulumi.getter
-    def certificate(self) -> Optional[pulumi.Input[int]]:
-        return pulumi.get(self, "certificate")
+    def edgerc(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "edgerc")
 
-    @certificate.setter
-    def certificate(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "certificate", value)
+    @edgerc.setter
+    def edgerc(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "edgerc", value)
 
     @property
     @pulumi.getter
-    def contract(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "contract")
-
-    @contract.setter
-    def contract(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "contract", value)
+    def gtm(self) -> Optional[pulumi.Input['ProviderGtmArgs']]:
+        warnings.warn("""The setting \"gtm\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""gtm is deprecated: The setting \"gtm\" has been deprecated.""")
 
-    @property
-    @pulumi.getter(name="contractId")
-    def contract_id(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "contract_id")
+        return pulumi.get(self, "gtm")
 
-    @contract_id.setter
-    def contract_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "contract_id", value)
+    @gtm.setter
+    def gtm(self, value: Optional[pulumi.Input['ProviderGtmArgs']]):
+        pulumi.set(self, "gtm", value)
 
     @property
-    @pulumi.getter(name="edgeHostname")
-    def edge_hostname(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "edge_hostname")
+    @pulumi.getter(name="gtmSection")
+    def gtm_section(self) -> Optional[pulumi.Input[str]]:
+        warnings.warn("""The setting \"gtm_section\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""gtm_section is deprecated: The setting \"gtm_section\" has been deprecated.""")
 
-    @edge_hostname.setter
-    def edge_hostname(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "edge_hostname", value)
+        return pulumi.get(self, "gtm_section")
 
-    @property
-    @pulumi.getter
-    def group(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "group")
-
-    @group.setter
-    def group(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "group", value)
+    @gtm_section.setter
+    def gtm_section(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "gtm_section", value)
 
     @property
-    @pulumi.getter(name="groupId")
-    def group_id(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "group_id")
+    @pulumi.getter(name="networklistSection")
+    def networklist_section(self) -> Optional[pulumi.Input[str]]:
+        warnings.warn("""The setting \"networklist_section\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""networklist_section is deprecated: The setting \"networklist_section\" has been deprecated.""")
 
-    @group_id.setter
-    def group_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "group_id", value)
+        return pulumi.get(self, "networklist_section")
 
-    @property
-    @pulumi.getter(name="ipBehavior")
-    def ip_behavior(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "ip_behavior")
-
-    @ip_behavior.setter
-    def ip_behavior(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "ip_behavior", value)
+    @networklist_section.setter
+    def networklist_section(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "networklist_section", value)
 
     @property
     @pulumi.getter
-    def product(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "product")
+    def networks(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProviderNetworkArgs']]]]:
+        return pulumi.get(self, "networks")
 
-    @product.setter
-    def product(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "product", value)
+    @networks.setter
+    def networks(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ProviderNetworkArgs']]]]):
+        pulumi.set(self, "networks", value)
 
     @property
-    @pulumi.getter(name="productId")
-    def product_id(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "product_id")
+    @pulumi.getter(name="papiSection")
+    def papi_section(self) -> Optional[pulumi.Input[str]]:
+        warnings.warn("""The setting \"papi_section\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""papi_section is deprecated: The setting \"papi_section\" has been deprecated.""")
+
+        return pulumi.get(self, "papi_section")
 
-    @product_id.setter
-    def product_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "product_id", value)
+    @papi_section.setter
+    def papi_section(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "papi_section", value)
 
     @property
-    @pulumi.getter(name="statusUpdateEmails")
-    def status_update_emails(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        Email address that should receive updates on the IP behavior update request. Required for update operation.
-        """
-        return pulumi.get(self, "status_update_emails")
+    @pulumi.getter(name="propertySection")
+    def property_section(self) -> Optional[pulumi.Input[str]]:
+        warnings.warn("""The setting \"property_section\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""property_section is deprecated: The setting \"property_section\" has been deprecated.""")
+
+        return pulumi.get(self, "property_section")
 
-    @status_update_emails.setter
-    def status_update_emails(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "status_update_emails", value)
+    @property_section.setter
+    def property_section(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "property_section", value)
 
     @property
-    @pulumi.getter(name="useCases")
-    def use_cases(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="requestLimit")
+    def request_limit(self) -> Optional[pulumi.Input[int]]:
         """
-        A JSON encoded list of use cases
+        The maximum number of API requests to be made per second (0 for no limit)
         """
-        return pulumi.get(self, "use_cases")
+        return pulumi.get(self, "request_limit")
 
-    @use_cases.setter
-    def use_cases(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "use_cases", value)
+    @request_limit.setter
+    def request_limit(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "request_limit", value)
 
+    @property
+    @pulumi.getter
+    def property(self) -> Optional[pulumi.Input['ProviderPropertyArgs']]:
+        warnings.warn("""The setting \"property\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""property is deprecated: The setting \"property\" has been deprecated.""")
 
-warnings.warn("""akamai.properties/edgehostname.EdgeHostName has been deprecated in favor of akamai.index/edgehostname.EdgeHostName""", DeprecationWarning)
+        return pulumi.get(self, "property")
 
+    @property.setter
+    def property(self, value: Optional[pulumi.Input['ProviderPropertyArgs']]):
+        pulumi.set(self, "property", value)
 
-class EdgeHostName(pulumi.CustomResource):
-    warnings.warn("""akamai.properties/edgehostname.EdgeHostName has been deprecated in favor of akamai.index/edgehostname.EdgeHostName""", DeprecationWarning)
 
+class Provider(pulumi.ProviderResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 certificate: Optional[pulumi.Input[int]] = None,
-                 contract: Optional[pulumi.Input[str]] = None,
-                 contract_id: Optional[pulumi.Input[str]] = None,
-                 edge_hostname: Optional[pulumi.Input[str]] = None,
-                 group: Optional[pulumi.Input[str]] = None,
-                 group_id: Optional[pulumi.Input[str]] = None,
-                 ip_behavior: Optional[pulumi.Input[str]] = None,
-                 product: Optional[pulumi.Input[str]] = None,
-                 product_id: Optional[pulumi.Input[str]] = None,
-                 status_update_emails: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 use_cases: Optional[pulumi.Input[str]] = None,
+                 appsec_section: Optional[pulumi.Input[str]] = None,
+                 appsecs: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProviderAppsecArgs']]]]] = None,
+                 cache_enabled: Optional[pulumi.Input[bool]] = None,
+                 config: Optional[pulumi.Input[pulumi.InputType['ProviderConfigArgs']]] = None,
+                 config_section: Optional[pulumi.Input[str]] = None,
+                 dns: Optional[pulumi.Input[pulumi.InputType['ProviderDnsArgs']]] = None,
+                 dns_section: Optional[pulumi.Input[str]] = None,
+                 edgerc: Optional[pulumi.Input[str]] = None,
+                 gtm: Optional[pulumi.Input[pulumi.InputType['ProviderGtmArgs']]] = None,
+                 gtm_section: Optional[pulumi.Input[str]] = None,
+                 networklist_section: Optional[pulumi.Input[str]] = None,
+                 networks: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProviderNetworkArgs']]]]] = None,
+                 papi_section: Optional[pulumi.Input[str]] = None,
+                 property: Optional[pulumi.Input[pulumi.InputType['ProviderPropertyArgs']]] = None,
+                 property_section: Optional[pulumi.Input[str]] = None,
+                 request_limit: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
-        Create a EdgeHostName resource with the given unique name, props, and options.
+        The provider type for the akamai package. By default, resources use package-wide configuration
+        settings, however an explicit `Provider` instance may be created and passed during resource
+        construction to achieve fine-grained programmatic control over provider settings. See the
+        [documentation](https://www.pulumi.com/docs/reference/programming-model/#providers) for more information.
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] status_update_emails: Email address that should receive updates on the IP behavior update request. Required for update operation.
-        :param pulumi.Input[str] use_cases: A JSON encoded list of use cases
+        :param pulumi.Input[str] config_section: The section of the edgerc file to use for configuration
+        :param pulumi.Input[int] request_limit: The maximum number of API requests to be made per second (0 for no limit)
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: EdgeHostNameArgs,
+                 args: Optional[ProviderArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a EdgeHostName resource with the given unique name, props, and options.
+        The provider type for the akamai package. By default, resources use package-wide configuration
+        settings, however an explicit `Provider` instance may be created and passed during resource
+        construction to achieve fine-grained programmatic control over provider settings. See the
+        [documentation](https://www.pulumi.com/docs/reference/programming-model/#providers) for more information.
+
         :param str resource_name: The name of the resource.
-        :param EdgeHostNameArgs args: The arguments to use to populate this resource's properties.
+        :param ProviderArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(EdgeHostNameArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(ProviderArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 certificate: Optional[pulumi.Input[int]] = None,
-                 contract: Optional[pulumi.Input[str]] = None,
-                 contract_id: Optional[pulumi.Input[str]] = None,
-                 edge_hostname: Optional[pulumi.Input[str]] = None,
-                 group: Optional[pulumi.Input[str]] = None,
-                 group_id: Optional[pulumi.Input[str]] = None,
-                 ip_behavior: Optional[pulumi.Input[str]] = None,
-                 product: Optional[pulumi.Input[str]] = None,
-                 product_id: Optional[pulumi.Input[str]] = None,
-                 status_update_emails: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 use_cases: Optional[pulumi.Input[str]] = None,
+                 appsec_section: Optional[pulumi.Input[str]] = None,
+                 appsecs: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProviderAppsecArgs']]]]] = None,
+                 cache_enabled: Optional[pulumi.Input[bool]] = None,
+                 config: Optional[pulumi.Input[pulumi.InputType['ProviderConfigArgs']]] = None,
+                 config_section: Optional[pulumi.Input[str]] = None,
+                 dns: Optional[pulumi.Input[pulumi.InputType['ProviderDnsArgs']]] = None,
+                 dns_section: Optional[pulumi.Input[str]] = None,
+                 edgerc: Optional[pulumi.Input[str]] = None,
+                 gtm: Optional[pulumi.Input[pulumi.InputType['ProviderGtmArgs']]] = None,
+                 gtm_section: Optional[pulumi.Input[str]] = None,
+                 networklist_section: Optional[pulumi.Input[str]] = None,
+                 networks: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProviderNetworkArgs']]]]] = None,
+                 papi_section: Optional[pulumi.Input[str]] = None,
+                 property: Optional[pulumi.Input[pulumi.InputType['ProviderPropertyArgs']]] = None,
+                 property_section: Optional[pulumi.Input[str]] = None,
+                 request_limit: Optional[pulumi.Input[int]] = None,
                  __props__=None):
-        pulumi.log.warn("""EdgeHostName is deprecated: akamai.properties/edgehostname.EdgeHostName has been deprecated in favor of akamai.index/edgehostname.EdgeHostName""")
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = EdgeHostNameArgs.__new__(EdgeHostNameArgs)
+            __props__ = ProviderArgs.__new__(ProviderArgs)
 
-            __props__.__dict__["certificate"] = certificate
-            if contract is not None and not opts.urn:
-                warnings.warn("""The setting \"contract\" has been deprecated.""", DeprecationWarning)
-                pulumi.log.warn("""contract is deprecated: The setting \"contract\" has been deprecated.""")
-            __props__.__dict__["contract"] = contract
-            __props__.__dict__["contract_id"] = contract_id
-            if edge_hostname is None and not opts.urn:
-                raise TypeError("Missing required property 'edge_hostname'")
-            __props__.__dict__["edge_hostname"] = edge_hostname
-            if group is not None and not opts.urn:
-                warnings.warn("""The setting \"group\" has been deprecated.""", DeprecationWarning)
-                pulumi.log.warn("""group is deprecated: The setting \"group\" has been deprecated.""")
-            __props__.__dict__["group"] = group
-            __props__.__dict__["group_id"] = group_id
-            if ip_behavior is None and not opts.urn:
-                raise TypeError("Missing required property 'ip_behavior'")
-            __props__.__dict__["ip_behavior"] = ip_behavior
-            if product is not None and not opts.urn:
-                warnings.warn("""The setting \"product\" has been deprecated.""", DeprecationWarning)
-                pulumi.log.warn("""product is deprecated: The setting \"product\" has been deprecated.""")
-            __props__.__dict__["product"] = product
-            __props__.__dict__["product_id"] = product_id
-            __props__.__dict__["status_update_emails"] = status_update_emails
-            __props__.__dict__["use_cases"] = use_cases
-        super(EdgeHostName, __self__).__init__(
-            'akamai:properties/edgeHostName:EdgeHostName',
+            if appsec_section is not None and not opts.urn:
+                warnings.warn("""The setting \"appsec_section\" has been deprecated.""", DeprecationWarning)
+                pulumi.log.warn("""appsec_section is deprecated: The setting \"appsec_section\" has been deprecated.""")
+            __props__.__dict__["appsec_section"] = appsec_section
+            if appsecs is not None and not opts.urn:
+                warnings.warn("""The setting \"appsec\" has been deprecated.""", DeprecationWarning)
+                pulumi.log.warn("""appsecs is deprecated: The setting \"appsec\" has been deprecated.""")
+            __props__.__dict__["appsecs"] = pulumi.Output.from_input(appsecs).apply(pulumi.runtime.to_json) if appsecs is not None else None
+            __props__.__dict__["cache_enabled"] = pulumi.Output.from_input(cache_enabled).apply(pulumi.runtime.to_json) if cache_enabled is not None else None
+            __props__.__dict__["config"] = pulumi.Output.from_input(config).apply(pulumi.runtime.to_json) if config is not None else None
+            __props__.__dict__["config_section"] = config_section
+            if dns is not None and not opts.urn:
+                warnings.warn("""The setting \"dns\" has been deprecated.""", DeprecationWarning)
+                pulumi.log.warn("""dns is deprecated: The setting \"dns\" has been deprecated.""")
+            __props__.__dict__["dns"] = pulumi.Output.from_input(dns).apply(pulumi.runtime.to_json) if dns is not None else None
+            if dns_section is not None and not opts.urn:
+                warnings.warn("""The setting \"dns_section\" has been deprecated.""", DeprecationWarning)
+                pulumi.log.warn("""dns_section is deprecated: The setting \"dns_section\" has been deprecated.""")
+            __props__.__dict__["dns_section"] = dns_section
+            __props__.__dict__["edgerc"] = edgerc
+            if gtm is not None and not opts.urn:
+                warnings.warn("""The setting \"gtm\" has been deprecated.""", DeprecationWarning)
+                pulumi.log.warn("""gtm is deprecated: The setting \"gtm\" has been deprecated.""")
+            __props__.__dict__["gtm"] = pulumi.Output.from_input(gtm).apply(pulumi.runtime.to_json) if gtm is not None else None
+            if gtm_section is not None and not opts.urn:
+                warnings.warn("""The setting \"gtm_section\" has been deprecated.""", DeprecationWarning)
+                pulumi.log.warn("""gtm_section is deprecated: The setting \"gtm_section\" has been deprecated.""")
+            __props__.__dict__["gtm_section"] = gtm_section
+            if networklist_section is not None and not opts.urn:
+                warnings.warn("""The setting \"networklist_section\" has been deprecated.""", DeprecationWarning)
+                pulumi.log.warn("""networklist_section is deprecated: The setting \"networklist_section\" has been deprecated.""")
+            __props__.__dict__["networklist_section"] = networklist_section
+            __props__.__dict__["networks"] = pulumi.Output.from_input(networks).apply(pulumi.runtime.to_json) if networks is not None else None
+            if papi_section is not None and not opts.urn:
+                warnings.warn("""The setting \"papi_section\" has been deprecated.""", DeprecationWarning)
+                pulumi.log.warn("""papi_section is deprecated: The setting \"papi_section\" has been deprecated.""")
+            __props__.__dict__["papi_section"] = papi_section
+            if property is not None and not opts.urn:
+                warnings.warn("""The setting \"property\" has been deprecated.""", DeprecationWarning)
+                pulumi.log.warn("""property is deprecated: The setting \"property\" has been deprecated.""")
+            __props__.__dict__["property"] = pulumi.Output.from_input(property).apply(pulumi.runtime.to_json) if property is not None else None
+            if property_section is not None and not opts.urn:
+                warnings.warn("""The setting \"property_section\" has been deprecated.""", DeprecationWarning)
+                pulumi.log.warn("""property_section is deprecated: The setting \"property_section\" has been deprecated.""")
+            __props__.__dict__["property_section"] = property_section
+            __props__.__dict__["request_limit"] = pulumi.Output.from_input(request_limit).apply(pulumi.runtime.to_json) if request_limit is not None else None
+        super(Provider, __self__).__init__(
+            'akamai',
             resource_name,
             __props__,
             opts)
 
-    @staticmethod
-    def get(resource_name: str,
-            id: pulumi.Input[str],
-            opts: Optional[pulumi.ResourceOptions] = None,
-            certificate: Optional[pulumi.Input[int]] = None,
-            contract: Optional[pulumi.Input[str]] = None,
-            contract_id: Optional[pulumi.Input[str]] = None,
-            edge_hostname: Optional[pulumi.Input[str]] = None,
-            group: Optional[pulumi.Input[str]] = None,
-            group_id: Optional[pulumi.Input[str]] = None,
-            ip_behavior: Optional[pulumi.Input[str]] = None,
-            product: Optional[pulumi.Input[str]] = None,
-            product_id: Optional[pulumi.Input[str]] = None,
-            status_update_emails: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-            use_cases: Optional[pulumi.Input[str]] = None) -> 'EdgeHostName':
-        """
-        Get an existing EdgeHostName resource's state with the given name, id, and optional extra
-        properties used to qualify the lookup.
-
-        :param str resource_name: The unique name of the resulting resource.
-        :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
-        :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] status_update_emails: Email address that should receive updates on the IP behavior update request. Required for update operation.
-        :param pulumi.Input[str] use_cases: A JSON encoded list of use cases
-        """
-        opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
-
-        __props__ = _EdgeHostNameState.__new__(_EdgeHostNameState)
-
-        __props__.__dict__["certificate"] = certificate
-        __props__.__dict__["contract"] = contract
-        __props__.__dict__["contract_id"] = contract_id
-        __props__.__dict__["edge_hostname"] = edge_hostname
-        __props__.__dict__["group"] = group
-        __props__.__dict__["group_id"] = group_id
-        __props__.__dict__["ip_behavior"] = ip_behavior
-        __props__.__dict__["product"] = product
-        __props__.__dict__["product_id"] = product_id
-        __props__.__dict__["status_update_emails"] = status_update_emails
-        __props__.__dict__["use_cases"] = use_cases
-        return EdgeHostName(resource_name, opts=opts, __props__=__props__)
-
     @property
-    @pulumi.getter
-    def certificate(self) -> pulumi.Output[Optional[int]]:
-        return pulumi.get(self, "certificate")
+    @pulumi.getter(name="appsecSection")
+    def appsec_section(self) -> pulumi.Output[Optional[str]]:
+        warnings.warn("""The setting \"appsec_section\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""appsec_section is deprecated: The setting \"appsec_section\" has been deprecated.""")
 
-    @property
-    @pulumi.getter
-    def contract(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "contract")
+        return pulumi.get(self, "appsec_section")
 
     @property
-    @pulumi.getter(name="contractId")
-    def contract_id(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "contract_id")
+    @pulumi.getter(name="configSection")
+    def config_section(self) -> pulumi.Output[Optional[str]]:
+        """
+        The section of the edgerc file to use for configuration
+        """
+        return pulumi.get(self, "config_section")
 
     @property
-    @pulumi.getter(name="edgeHostname")
-    def edge_hostname(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "edge_hostname")
+    @pulumi.getter(name="dnsSection")
+    def dns_section(self) -> pulumi.Output[Optional[str]]:
+        warnings.warn("""The setting \"dns_section\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""dns_section is deprecated: The setting \"dns_section\" has been deprecated.""")
+
+        return pulumi.get(self, "dns_section")
 
     @property
     @pulumi.getter
-    def group(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "group")
+    def edgerc(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "edgerc")
 
     @property
-    @pulumi.getter(name="groupId")
-    def group_id(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "group_id")
+    @pulumi.getter(name="gtmSection")
+    def gtm_section(self) -> pulumi.Output[Optional[str]]:
+        warnings.warn("""The setting \"gtm_section\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""gtm_section is deprecated: The setting \"gtm_section\" has been deprecated.""")
 
-    @property
-    @pulumi.getter(name="ipBehavior")
-    def ip_behavior(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "ip_behavior")
+        return pulumi.get(self, "gtm_section")
 
     @property
-    @pulumi.getter
-    def product(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "product")
+    @pulumi.getter(name="networklistSection")
+    def networklist_section(self) -> pulumi.Output[Optional[str]]:
+        warnings.warn("""The setting \"networklist_section\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""networklist_section is deprecated: The setting \"networklist_section\" has been deprecated.""")
 
-    @property
-    @pulumi.getter(name="productId")
-    def product_id(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "product_id")
+        return pulumi.get(self, "networklist_section")
 
     @property
-    @pulumi.getter(name="statusUpdateEmails")
-    def status_update_emails(self) -> pulumi.Output[Optional[Sequence[str]]]:
-        """
-        Email address that should receive updates on the IP behavior update request. Required for update operation.
-        """
-        return pulumi.get(self, "status_update_emails")
+    @pulumi.getter(name="papiSection")
+    def papi_section(self) -> pulumi.Output[Optional[str]]:
+        warnings.warn("""The setting \"papi_section\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""papi_section is deprecated: The setting \"papi_section\" has been deprecated.""")
+
+        return pulumi.get(self, "papi_section")
 
     @property
-    @pulumi.getter(name="useCases")
-    def use_cases(self) -> pulumi.Output[Optional[str]]:
-        """
-        A JSON encoded list of use cases
-        """
-        return pulumi.get(self, "use_cases")
+    @pulumi.getter(name="propertySection")
+    def property_section(self) -> pulumi.Output[Optional[str]]:
+        warnings.warn("""The setting \"property_section\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""property_section is deprecated: The setting \"property_section\" has been deprecated.""")
+
+        return pulumi.get(self, "property_section")
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/properties/get_activation.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/properties/get_activation.py`

 * *Files 11% similar despite different names*

```diff
@@ -139,24 +139,24 @@
     __args__['network'] = network
     __args__['propertyId'] = property_id
     __args__['version'] = version
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:properties/getActivation:getActivation', __args__, opts=opts, typ=GetActivationResult).value
 
     return AwaitableGetActivationResult(
-        activation_id=__ret__.activation_id,
-        contacts=__ret__.contacts,
-        errors=__ret__.errors,
-        id=__ret__.id,
-        network=__ret__.network,
-        note=__ret__.note,
-        property_id=__ret__.property_id,
-        status=__ret__.status,
-        version=__ret__.version,
-        warnings=__ret__.warnings)
+        activation_id=pulumi.get(__ret__, 'activation_id'),
+        contacts=pulumi.get(__ret__, 'contacts'),
+        errors=pulumi.get(__ret__, 'errors'),
+        id=pulumi.get(__ret__, 'id'),
+        network=pulumi.get(__ret__, 'network'),
+        note=pulumi.get(__ret__, 'note'),
+        property_id=pulumi.get(__ret__, 'property_id'),
+        status=pulumi.get(__ret__, 'status'),
+        version=pulumi.get(__ret__, 'version'),
+        warnings=pulumi.get(__ret__, 'warnings'))
 
 
 @_utilities.lift_output_func(get_activation)
 def get_activation_output(network: Optional[pulumi.Input[Optional[str]]] = None,
                           property_id: Optional[pulumi.Input[str]] = None,
                           version: Optional[pulumi.Input[int]] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetActivationResult]:
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/properties/get_cp_code.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/get_cp_code.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,47 +3,37 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from .. import _utilities
+from . import _utilities
 
 __all__ = [
     'GetCpCodeResult',
     'AwaitableGetCpCodeResult',
     'get_cp_code',
     'get_cp_code_output',
 ]
 
-warnings.warn("""akamai.properties/getcpcode.getCpCode has been deprecated in favor of akamai.index/getcpcode.getCpCode""", DeprecationWarning)
-
 @pulumi.output_type
 class GetCpCodeResult:
     """
     A collection of values returned by getCpCode.
     """
     def __init__(__self__, contract=None, contract_id=None, group=None, group_id=None, id=None, name=None, product_ids=None):
         if contract and not isinstance(contract, str):
             raise TypeError("Expected argument 'contract' to be a str")
-        if contract is not None:
-            warnings.warn("""The setting \"contract\" has been deprecated.""", DeprecationWarning)
-            pulumi.log.warn("""contract is deprecated: The setting \"contract\" has been deprecated.""")
-
         pulumi.set(__self__, "contract", contract)
         if contract_id and not isinstance(contract_id, str):
             raise TypeError("Expected argument 'contract_id' to be a str")
         pulumi.set(__self__, "contract_id", contract_id)
         if group and not isinstance(group, str):
             raise TypeError("Expected argument 'group' to be a str")
-        if group is not None:
-            warnings.warn("""The setting \"group\" has been deprecated.""", DeprecationWarning)
-            pulumi.log.warn("""group is deprecated: The setting \"group\" has been deprecated.""")
-
         pulumi.set(__self__, "group", group)
         if group_id and not isinstance(group_id, str):
             raise TypeError("Expected argument 'group_id' to be a str")
         pulumi.set(__self__, "group_id", group_id)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
@@ -53,24 +43,30 @@
         if product_ids and not isinstance(product_ids, list):
             raise TypeError("Expected argument 'product_ids' to be a list")
         pulumi.set(__self__, "product_ids", product_ids)
 
     @property
     @pulumi.getter
     def contract(self) -> str:
+        warnings.warn("""The setting \"contract\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""contract is deprecated: The setting \"contract\" has been deprecated.""")
+
         return pulumi.get(self, "contract")
 
     @property
     @pulumi.getter(name="contractId")
     def contract_id(self) -> str:
         return pulumi.get(self, "contract_id")
 
     @property
     @pulumi.getter
     def group(self) -> str:
+        warnings.warn("""The setting \"group\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""group is deprecated: The setting \"group\" has been deprecated.""")
+
         return pulumi.get(self, "group")
 
     @property
     @pulumi.getter(name="groupId")
     def group_id(self) -> str:
         return pulumi.get(self, "group_id")
 
@@ -113,39 +109,37 @@
                 group: Optional[str] = None,
                 group_id: Optional[str] = None,
                 name: Optional[str] = None,
                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetCpCodeResult:
     """
     Use this data source to access information about an existing resource.
     """
-    pulumi.log.warn("""get_cp_code is deprecated: akamai.properties/getcpcode.getCpCode has been deprecated in favor of akamai.index/getcpcode.getCpCode""")
     __args__ = dict()
     __args__['contract'] = contract
     __args__['contractId'] = contract_id
     __args__['group'] = group
     __args__['groupId'] = group_id
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('akamai:properties/getCpCode:getCpCode', __args__, opts=opts, typ=GetCpCodeResult).value
+    __ret__ = pulumi.runtime.invoke('akamai:index/getCpCode:getCpCode', __args__, opts=opts, typ=GetCpCodeResult).value
 
     return AwaitableGetCpCodeResult(
-        contract=__ret__.contract,
-        contract_id=__ret__.contract_id,
-        group=__ret__.group,
-        group_id=__ret__.group_id,
-        id=__ret__.id,
-        name=__ret__.name,
-        product_ids=__ret__.product_ids)
+        contract=pulumi.get(__ret__, 'contract'),
+        contract_id=pulumi.get(__ret__, 'contract_id'),
+        group=pulumi.get(__ret__, 'group'),
+        group_id=pulumi.get(__ret__, 'group_id'),
+        id=pulumi.get(__ret__, 'id'),
+        name=pulumi.get(__ret__, 'name'),
+        product_ids=pulumi.get(__ret__, 'product_ids'))
 
 
 @_utilities.lift_output_func(get_cp_code)
 def get_cp_code_output(contract: Optional[pulumi.Input[Optional[str]]] = None,
                        contract_id: Optional[pulumi.Input[Optional[str]]] = None,
                        group: Optional[pulumi.Input[Optional[str]]] = None,
                        group_id: Optional[pulumi.Input[Optional[str]]] = None,
                        name: Optional[pulumi.Input[str]] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCpCodeResult]:
     """
     Use this data source to access information about an existing resource.
     """
-    pulumi.log.warn("""get_cp_code is deprecated: akamai.properties/getcpcode.getCpCode has been deprecated in favor of akamai.index/getcpcode.getCpCode""")
     ...
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/properties/get_property.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/properties/get_property.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,18 +83,18 @@
     __args__ = dict()
     __args__['name'] = name
     __args__['version'] = version
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:properties/getProperty:getProperty', __args__, opts=opts, typ=GetPropertyResult).value
 
     return AwaitableGetPropertyResult(
-        id=__ret__.id,
-        name=__ret__.name,
-        rules=__ret__.rules,
-        version=__ret__.version)
+        id=pulumi.get(__ret__, 'id'),
+        name=pulumi.get(__ret__, 'name'),
+        rules=pulumi.get(__ret__, 'rules'),
+        version=pulumi.get(__ret__, 'version'))
 
 
 @_utilities.lift_output_func(get_property)
 def get_property_output(name: Optional[pulumi.Input[str]] = None,
                         version: Optional[pulumi.Input[Optional[int]]] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPropertyResult]:
     """
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/properties/outputs.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/property_include_activation.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,635 +3,553 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from .. import _utilities
+from . import _utilities
 from . import outputs
+from ._inputs import *
 
-__all__ = [
-    'PropertyActivationComplianceRecord',
-    'PropertyActivationRuleError',
-    'PropertyActivationRuleWarning',
-    'PropertyHostname',
-    'PropertyHostnameCertStatus',
-    'PropertyOrigin',
-    'PropertyRuleError',
-    'PropertyRuleWarning',
-]
-
-@pulumi.output_type
-class PropertyActivationComplianceRecord(dict):
-    @staticmethod
-    def __key_warning(key: str):
-        suggest = None
-        if key == "noncomplianceReason":
-            suggest = "noncompliance_reason"
-        elif key == "customerEmail":
-            suggest = "customer_email"
-        elif key == "otherNoncomplianceReason":
-            suggest = "other_noncompliance_reason"
-        elif key == "peerReviewedBy":
-            suggest = "peer_reviewed_by"
-        elif key == "ticketId":
-            suggest = "ticket_id"
-        elif key == "unitTested":
-            suggest = "unit_tested"
-
-        if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in PropertyActivationComplianceRecord. Access the value via the '{suggest}' property getter instead.")
-
-    def __getitem__(self, key: str) -> Any:
-        PropertyActivationComplianceRecord.__key_warning(key)
-        return super().__getitem__(key)
-
-    def get(self, key: str, default = None) -> Any:
-        PropertyActivationComplianceRecord.__key_warning(key)
-        return super().get(key, default)
-
-    def __init__(__self__, *,
-                 noncompliance_reason: str,
-                 customer_email: Optional[str] = None,
-                 other_noncompliance_reason: Optional[str] = None,
-                 peer_reviewed_by: Optional[str] = None,
-                 ticket_id: Optional[str] = None,
-                 unit_tested: Optional[bool] = None):
-        pulumi.set(__self__, "noncompliance_reason", noncompliance_reason)
-        if customer_email is not None:
-            pulumi.set(__self__, "customer_email", customer_email)
-        if other_noncompliance_reason is not None:
-            pulumi.set(__self__, "other_noncompliance_reason", other_noncompliance_reason)
-        if peer_reviewed_by is not None:
-            pulumi.set(__self__, "peer_reviewed_by", peer_reviewed_by)
-        if ticket_id is not None:
-            pulumi.set(__self__, "ticket_id", ticket_id)
-        if unit_tested is not None:
-            pulumi.set(__self__, "unit_tested", unit_tested)
-
-    @property
-    @pulumi.getter(name="noncomplianceReason")
-    def noncompliance_reason(self) -> str:
-        return pulumi.get(self, "noncompliance_reason")
-
-    @property
-    @pulumi.getter(name="customerEmail")
-    def customer_email(self) -> Optional[str]:
-        return pulumi.get(self, "customer_email")
-
-    @property
-    @pulumi.getter(name="otherNoncomplianceReason")
-    def other_noncompliance_reason(self) -> Optional[str]:
-        return pulumi.get(self, "other_noncompliance_reason")
-
-    @property
-    @pulumi.getter(name="peerReviewedBy")
-    def peer_reviewed_by(self) -> Optional[str]:
-        return pulumi.get(self, "peer_reviewed_by")
-
-    @property
-    @pulumi.getter(name="ticketId")
-    def ticket_id(self) -> Optional[str]:
-        return pulumi.get(self, "ticket_id")
-
-    @property
-    @pulumi.getter(name="unitTested")
-    def unit_tested(self) -> Optional[bool]:
-        return pulumi.get(self, "unit_tested")
-
-
-@pulumi.output_type
-class PropertyActivationRuleError(dict):
-    @staticmethod
-    def __key_warning(key: str):
-        suggest = None
-        if key == "behaviorName":
-            suggest = "behavior_name"
-        elif key == "errorLocation":
-            suggest = "error_location"
-        elif key == "statusCode":
-            suggest = "status_code"
-
-        if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in PropertyActivationRuleError. Access the value via the '{suggest}' property getter instead.")
-
-    def __getitem__(self, key: str) -> Any:
-        PropertyActivationRuleError.__key_warning(key)
-        return super().__getitem__(key)
-
-    def get(self, key: str, default = None) -> Any:
-        PropertyActivationRuleError.__key_warning(key)
-        return super().get(key, default)
-
-    def __init__(__self__, *,
-                 behavior_name: Optional[str] = None,
-                 detail: Optional[str] = None,
-                 error_location: Optional[str] = None,
-                 instance: Optional[str] = None,
-                 status_code: Optional[int] = None,
-                 title: Optional[str] = None,
-                 type: Optional[str] = None):
-        if behavior_name is not None:
-            pulumi.set(__self__, "behavior_name", behavior_name)
-        if detail is not None:
-            pulumi.set(__self__, "detail", detail)
-        if error_location is not None:
-            pulumi.set(__self__, "error_location", error_location)
-        if instance is not None:
-            pulumi.set(__self__, "instance", instance)
-        if status_code is not None:
-            pulumi.set(__self__, "status_code", status_code)
-        if title is not None:
-            pulumi.set(__self__, "title", title)
-        if type is not None:
-            pulumi.set(__self__, "type", type)
-
-    @property
-    @pulumi.getter(name="behaviorName")
-    def behavior_name(self) -> Optional[str]:
-        return pulumi.get(self, "behavior_name")
-
-    @property
-    @pulumi.getter
-    def detail(self) -> Optional[str]:
-        return pulumi.get(self, "detail")
-
-    @property
-    @pulumi.getter(name="errorLocation")
-    def error_location(self) -> Optional[str]:
-        return pulumi.get(self, "error_location")
-
-    @property
-    @pulumi.getter
-    def instance(self) -> Optional[str]:
-        return pulumi.get(self, "instance")
-
-    @property
-    @pulumi.getter(name="statusCode")
-    def status_code(self) -> Optional[int]:
-        return pulumi.get(self, "status_code")
-
-    @property
-    @pulumi.getter
-    def title(self) -> Optional[str]:
-        return pulumi.get(self, "title")
-
-    @property
-    @pulumi.getter
-    def type(self) -> Optional[str]:
-        return pulumi.get(self, "type")
-
-
-@pulumi.output_type
-class PropertyActivationRuleWarning(dict):
-    @staticmethod
-    def __key_warning(key: str):
-        suggest = None
-        if key == "behaviorName":
-            suggest = "behavior_name"
-        elif key == "errorLocation":
-            suggest = "error_location"
-        elif key == "statusCode":
-            suggest = "status_code"
-
-        if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in PropertyActivationRuleWarning. Access the value via the '{suggest}' property getter instead.")
-
-    def __getitem__(self, key: str) -> Any:
-        PropertyActivationRuleWarning.__key_warning(key)
-        return super().__getitem__(key)
-
-    def get(self, key: str, default = None) -> Any:
-        PropertyActivationRuleWarning.__key_warning(key)
-        return super().get(key, default)
-
-    def __init__(__self__, *,
-                 behavior_name: Optional[str] = None,
-                 detail: Optional[str] = None,
-                 error_location: Optional[str] = None,
-                 instance: Optional[str] = None,
-                 status_code: Optional[int] = None,
-                 title: Optional[str] = None,
-                 type: Optional[str] = None):
-        if behavior_name is not None:
-            pulumi.set(__self__, "behavior_name", behavior_name)
-        if detail is not None:
-            pulumi.set(__self__, "detail", detail)
-        if error_location is not None:
-            pulumi.set(__self__, "error_location", error_location)
-        if instance is not None:
-            pulumi.set(__self__, "instance", instance)
-        if status_code is not None:
-            pulumi.set(__self__, "status_code", status_code)
-        if title is not None:
-            pulumi.set(__self__, "title", title)
-        if type is not None:
-            pulumi.set(__self__, "type", type)
-
-    @property
-    @pulumi.getter(name="behaviorName")
-    def behavior_name(self) -> Optional[str]:
-        return pulumi.get(self, "behavior_name")
-
-    @property
-    @pulumi.getter
-    def detail(self) -> Optional[str]:
-        return pulumi.get(self, "detail")
-
-    @property
-    @pulumi.getter(name="errorLocation")
-    def error_location(self) -> Optional[str]:
-        return pulumi.get(self, "error_location")
-
-    @property
-    @pulumi.getter
-    def instance(self) -> Optional[str]:
-        return pulumi.get(self, "instance")
-
-    @property
-    @pulumi.getter(name="statusCode")
-    def status_code(self) -> Optional[int]:
-        return pulumi.get(self, "status_code")
-
-    @property
-    @pulumi.getter
-    def title(self) -> Optional[str]:
-        return pulumi.get(self, "title")
-
-    @property
-    @pulumi.getter
-    def type(self) -> Optional[str]:
-        return pulumi.get(self, "type")
-
-
-@pulumi.output_type
-class PropertyHostname(dict):
-    @staticmethod
-    def __key_warning(key: str):
-        suggest = None
-        if key == "certProvisioningType":
-            suggest = "cert_provisioning_type"
-        elif key == "cnameFrom":
-            suggest = "cname_from"
-        elif key == "cnameTo":
-            suggest = "cname_to"
-        elif key == "certStatuses":
-            suggest = "cert_statuses"
-        elif key == "cnameType":
-            suggest = "cname_type"
-        elif key == "edgeHostnameId":
-            suggest = "edge_hostname_id"
-
-        if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in PropertyHostname. Access the value via the '{suggest}' property getter instead.")
-
-    def __getitem__(self, key: str) -> Any:
-        PropertyHostname.__key_warning(key)
-        return super().__getitem__(key)
-
-    def get(self, key: str, default = None) -> Any:
-        PropertyHostname.__key_warning(key)
-        return super().get(key, default)
-
-    def __init__(__self__, *,
-                 cert_provisioning_type: str,
-                 cname_from: str,
-                 cname_to: str,
-                 cert_statuses: Optional[Sequence['outputs.PropertyHostnameCertStatus']] = None,
-                 cname_type: Optional[str] = None,
-                 edge_hostname_id: Optional[str] = None):
-        pulumi.set(__self__, "cert_provisioning_type", cert_provisioning_type)
-        pulumi.set(__self__, "cname_from", cname_from)
-        pulumi.set(__self__, "cname_to", cname_to)
-        if cert_statuses is not None:
-            pulumi.set(__self__, "cert_statuses", cert_statuses)
-        if cname_type is not None:
-            pulumi.set(__self__, "cname_type", cname_type)
-        if edge_hostname_id is not None:
-            pulumi.set(__self__, "edge_hostname_id", edge_hostname_id)
-
-    @property
-    @pulumi.getter(name="certProvisioningType")
-    def cert_provisioning_type(self) -> str:
-        return pulumi.get(self, "cert_provisioning_type")
-
-    @property
-    @pulumi.getter(name="cnameFrom")
-    def cname_from(self) -> str:
-        return pulumi.get(self, "cname_from")
-
-    @property
-    @pulumi.getter(name="cnameTo")
-    def cname_to(self) -> str:
-        return pulumi.get(self, "cname_to")
-
-    @property
-    @pulumi.getter(name="certStatuses")
-    def cert_statuses(self) -> Optional[Sequence['outputs.PropertyHostnameCertStatus']]:
-        return pulumi.get(self, "cert_statuses")
-
-    @property
-    @pulumi.getter(name="cnameType")
-    def cname_type(self) -> Optional[str]:
-        return pulumi.get(self, "cname_type")
-
-    @property
-    @pulumi.getter(name="edgeHostnameId")
-    def edge_hostname_id(self) -> Optional[str]:
-        return pulumi.get(self, "edge_hostname_id")
-
-
-@pulumi.output_type
-class PropertyHostnameCertStatus(dict):
-    @staticmethod
-    def __key_warning(key: str):
-        suggest = None
-        if key == "productionStatus":
-            suggest = "production_status"
-        elif key == "stagingStatus":
-            suggest = "staging_status"
-
-        if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in PropertyHostnameCertStatus. Access the value via the '{suggest}' property getter instead.")
-
-    def __getitem__(self, key: str) -> Any:
-        PropertyHostnameCertStatus.__key_warning(key)
-        return super().__getitem__(key)
-
-    def get(self, key: str, default = None) -> Any:
-        PropertyHostnameCertStatus.__key_warning(key)
-        return super().get(key, default)
+__all__ = ['PropertyIncludeActivationArgs', 'PropertyIncludeActivation']
 
+@pulumi.input_type
+class PropertyIncludeActivationArgs:
     def __init__(__self__, *,
-                 hostname: Optional[str] = None,
-                 production_status: Optional[str] = None,
-                 staging_status: Optional[str] = None,
-                 target: Optional[str] = None):
-        if hostname is not None:
-            pulumi.set(__self__, "hostname", hostname)
-        if production_status is not None:
-            pulumi.set(__self__, "production_status", production_status)
-        if staging_status is not None:
-            pulumi.set(__self__, "staging_status", staging_status)
-        if target is not None:
-            pulumi.set(__self__, "target", target)
-
-    @property
-    @pulumi.getter
-    def hostname(self) -> Optional[str]:
-        return pulumi.get(self, "hostname")
-
-    @property
-    @pulumi.getter(name="productionStatus")
-    def production_status(self) -> Optional[str]:
-        return pulumi.get(self, "production_status")
-
-    @property
-    @pulumi.getter(name="stagingStatus")
-    def staging_status(self) -> Optional[str]:
-        return pulumi.get(self, "staging_status")
-
-    @property
-    @pulumi.getter
-    def target(self) -> Optional[str]:
-        return pulumi.get(self, "target")
+                 contract_id: pulumi.Input[str],
+                 group_id: pulumi.Input[str],
+                 include_id: pulumi.Input[str],
+                 network: pulumi.Input[str],
+                 notify_emails: pulumi.Input[Sequence[pulumi.Input[str]]],
+                 version: pulumi.Input[int],
+                 auto_acknowledge_rule_warnings: Optional[pulumi.Input[bool]] = None,
+                 compliance_record: Optional[pulumi.Input['PropertyIncludeActivationComplianceRecordArgs']] = None,
+                 note: Optional[pulumi.Input[str]] = None):
+        """
+        The set of arguments for constructing a PropertyIncludeActivation resource.
+        :param pulumi.Input[str] contract_id: The contract under which the include is activated
+        :param pulumi.Input[str] group_id: The group under which the include is activated
+        :param pulumi.Input[str] include_id: The unique identifier of the include
+        :param pulumi.Input[str] network: The network for which the activation will be performed
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] notify_emails: The list of email addresses to notify about an activation status
+        :param pulumi.Input[int] version: The unique identifier of the include
+        :param pulumi.Input[bool] auto_acknowledge_rule_warnings: Automatically acknowledge all rule warnings for activation and continue
+        :param pulumi.Input['PropertyIncludeActivationComplianceRecordArgs'] compliance_record: Provides an audit record when activating on a production network
+        :param pulumi.Input[str] note: The note to assign to a log message of the activation request
+        """
+        pulumi.set(__self__, "contract_id", contract_id)
+        pulumi.set(__self__, "group_id", group_id)
+        pulumi.set(__self__, "include_id", include_id)
+        pulumi.set(__self__, "network", network)
+        pulumi.set(__self__, "notify_emails", notify_emails)
+        pulumi.set(__self__, "version", version)
+        if auto_acknowledge_rule_warnings is not None:
+            pulumi.set(__self__, "auto_acknowledge_rule_warnings", auto_acknowledge_rule_warnings)
+        if compliance_record is not None:
+            pulumi.set(__self__, "compliance_record", compliance_record)
+        if note is not None:
+            pulumi.set(__self__, "note", note)
+
+    @property
+    @pulumi.getter(name="contractId")
+    def contract_id(self) -> pulumi.Input[str]:
+        """
+        The contract under which the include is activated
+        """
+        return pulumi.get(self, "contract_id")
+
+    @contract_id.setter
+    def contract_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "contract_id", value)
+
+    @property
+    @pulumi.getter(name="groupId")
+    def group_id(self) -> pulumi.Input[str]:
+        """
+        The group under which the include is activated
+        """
+        return pulumi.get(self, "group_id")
+
+    @group_id.setter
+    def group_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "group_id", value)
+
+    @property
+    @pulumi.getter(name="includeId")
+    def include_id(self) -> pulumi.Input[str]:
+        """
+        The unique identifier of the include
+        """
+        return pulumi.get(self, "include_id")
+
+    @include_id.setter
+    def include_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "include_id", value)
+
+    @property
+    @pulumi.getter
+    def network(self) -> pulumi.Input[str]:
+        """
+        The network for which the activation will be performed
+        """
+        return pulumi.get(self, "network")
+
+    @network.setter
+    def network(self, value: pulumi.Input[str]):
+        pulumi.set(self, "network", value)
+
+    @property
+    @pulumi.getter(name="notifyEmails")
+    def notify_emails(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
+        """
+        The list of email addresses to notify about an activation status
+        """
+        return pulumi.get(self, "notify_emails")
+
+    @notify_emails.setter
+    def notify_emails(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
+        pulumi.set(self, "notify_emails", value)
+
+    @property
+    @pulumi.getter
+    def version(self) -> pulumi.Input[int]:
+        """
+        The unique identifier of the include
+        """
+        return pulumi.get(self, "version")
+
+    @version.setter
+    def version(self, value: pulumi.Input[int]):
+        pulumi.set(self, "version", value)
+
+    @property
+    @pulumi.getter(name="autoAcknowledgeRuleWarnings")
+    def auto_acknowledge_rule_warnings(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Automatically acknowledge all rule warnings for activation and continue
+        """
+        return pulumi.get(self, "auto_acknowledge_rule_warnings")
+
+    @auto_acknowledge_rule_warnings.setter
+    def auto_acknowledge_rule_warnings(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "auto_acknowledge_rule_warnings", value)
+
+    @property
+    @pulumi.getter(name="complianceRecord")
+    def compliance_record(self) -> Optional[pulumi.Input['PropertyIncludeActivationComplianceRecordArgs']]:
+        """
+        Provides an audit record when activating on a production network
+        """
+        return pulumi.get(self, "compliance_record")
+
+    @compliance_record.setter
+    def compliance_record(self, value: Optional[pulumi.Input['PropertyIncludeActivationComplianceRecordArgs']]):
+        pulumi.set(self, "compliance_record", value)
+
+    @property
+    @pulumi.getter
+    def note(self) -> Optional[pulumi.Input[str]]:
+        """
+        The note to assign to a log message of the activation request
+        """
+        return pulumi.get(self, "note")
+
+    @note.setter
+    def note(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "note", value)
 
 
-@pulumi.output_type
-class PropertyOrigin(dict):
-    @staticmethod
-    def __key_warning(key: str):
-        suggest = None
-        if key == "cacheKeyHostname":
-            suggest = "cache_key_hostname"
-        elif key == "enableTrueClientIp":
-            suggest = "enable_true_client_ip"
-        elif key == "forwardHostname":
-            suggest = "forward_hostname"
-
-        if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in PropertyOrigin. Access the value via the '{suggest}' property getter instead.")
-
-    def __getitem__(self, key: str) -> Any:
-        PropertyOrigin.__key_warning(key)
-        return super().__getitem__(key)
-
-    def get(self, key: str, default = None) -> Any:
-        PropertyOrigin.__key_warning(key)
-        return super().get(key, default)
-
+@pulumi.input_type
+class _PropertyIncludeActivationState:
     def __init__(__self__, *,
-                 cache_key_hostname: Optional[str] = None,
-                 compress: Optional[bool] = None,
-                 enable_true_client_ip: Optional[bool] = None,
-                 forward_hostname: Optional[str] = None,
-                 hostname: Optional[str] = None,
-                 port: Optional[int] = None):
-        if cache_key_hostname is not None:
-            pulumi.set(__self__, "cache_key_hostname", cache_key_hostname)
-        if compress is not None:
-            pulumi.set(__self__, "compress", compress)
-        if enable_true_client_ip is not None:
-            pulumi.set(__self__, "enable_true_client_ip", enable_true_client_ip)
-        if forward_hostname is not None:
-            pulumi.set(__self__, "forward_hostname", forward_hostname)
-        if hostname is not None:
-            pulumi.set(__self__, "hostname", hostname)
-        if port is not None:
-            pulumi.set(__self__, "port", port)
+                 auto_acknowledge_rule_warnings: Optional[pulumi.Input[bool]] = None,
+                 compliance_record: Optional[pulumi.Input['PropertyIncludeActivationComplianceRecordArgs']] = None,
+                 contract_id: Optional[pulumi.Input[str]] = None,
+                 group_id: Optional[pulumi.Input[str]] = None,
+                 include_id: Optional[pulumi.Input[str]] = None,
+                 network: Optional[pulumi.Input[str]] = None,
+                 note: Optional[pulumi.Input[str]] = None,
+                 notify_emails: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 validations: Optional[pulumi.Input[str]] = None,
+                 version: Optional[pulumi.Input[int]] = None):
+        """
+        Input properties used for looking up and filtering PropertyIncludeActivation resources.
+        :param pulumi.Input[bool] auto_acknowledge_rule_warnings: Automatically acknowledge all rule warnings for activation and continue
+        :param pulumi.Input['PropertyIncludeActivationComplianceRecordArgs'] compliance_record: Provides an audit record when activating on a production network
+        :param pulumi.Input[str] contract_id: The contract under which the include is activated
+        :param pulumi.Input[str] group_id: The group under which the include is activated
+        :param pulumi.Input[str] include_id: The unique identifier of the include
+        :param pulumi.Input[str] network: The network for which the activation will be performed
+        :param pulumi.Input[str] note: The note to assign to a log message of the activation request
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] notify_emails: The list of email addresses to notify about an activation status
+        :param pulumi.Input[str] validations: The validation information in JSON format
+        :param pulumi.Input[int] version: The unique identifier of the include
+        """
+        if auto_acknowledge_rule_warnings is not None:
+            pulumi.set(__self__, "auto_acknowledge_rule_warnings", auto_acknowledge_rule_warnings)
+        if compliance_record is not None:
+            pulumi.set(__self__, "compliance_record", compliance_record)
+        if contract_id is not None:
+            pulumi.set(__self__, "contract_id", contract_id)
+        if group_id is not None:
+            pulumi.set(__self__, "group_id", group_id)
+        if include_id is not None:
+            pulumi.set(__self__, "include_id", include_id)
+        if network is not None:
+            pulumi.set(__self__, "network", network)
+        if note is not None:
+            pulumi.set(__self__, "note", note)
+        if notify_emails is not None:
+            pulumi.set(__self__, "notify_emails", notify_emails)
+        if validations is not None:
+            pulumi.set(__self__, "validations", validations)
+        if version is not None:
+            pulumi.set(__self__, "version", version)
+
+    @property
+    @pulumi.getter(name="autoAcknowledgeRuleWarnings")
+    def auto_acknowledge_rule_warnings(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Automatically acknowledge all rule warnings for activation and continue
+        """
+        return pulumi.get(self, "auto_acknowledge_rule_warnings")
+
+    @auto_acknowledge_rule_warnings.setter
+    def auto_acknowledge_rule_warnings(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "auto_acknowledge_rule_warnings", value)
+
+    @property
+    @pulumi.getter(name="complianceRecord")
+    def compliance_record(self) -> Optional[pulumi.Input['PropertyIncludeActivationComplianceRecordArgs']]:
+        """
+        Provides an audit record when activating on a production network
+        """
+        return pulumi.get(self, "compliance_record")
+
+    @compliance_record.setter
+    def compliance_record(self, value: Optional[pulumi.Input['PropertyIncludeActivationComplianceRecordArgs']]):
+        pulumi.set(self, "compliance_record", value)
+
+    @property
+    @pulumi.getter(name="contractId")
+    def contract_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        The contract under which the include is activated
+        """
+        return pulumi.get(self, "contract_id")
+
+    @contract_id.setter
+    def contract_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "contract_id", value)
+
+    @property
+    @pulumi.getter(name="groupId")
+    def group_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        The group under which the include is activated
+        """
+        return pulumi.get(self, "group_id")
+
+    @group_id.setter
+    def group_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "group_id", value)
+
+    @property
+    @pulumi.getter(name="includeId")
+    def include_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        The unique identifier of the include
+        """
+        return pulumi.get(self, "include_id")
+
+    @include_id.setter
+    def include_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "include_id", value)
+
+    @property
+    @pulumi.getter
+    def network(self) -> Optional[pulumi.Input[str]]:
+        """
+        The network for which the activation will be performed
+        """
+        return pulumi.get(self, "network")
+
+    @network.setter
+    def network(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "network", value)
+
+    @property
+    @pulumi.getter
+    def note(self) -> Optional[pulumi.Input[str]]:
+        """
+        The note to assign to a log message of the activation request
+        """
+        return pulumi.get(self, "note")
+
+    @note.setter
+    def note(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "note", value)
+
+    @property
+    @pulumi.getter(name="notifyEmails")
+    def notify_emails(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        The list of email addresses to notify about an activation status
+        """
+        return pulumi.get(self, "notify_emails")
+
+    @notify_emails.setter
+    def notify_emails(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "notify_emails", value)
+
+    @property
+    @pulumi.getter
+    def validations(self) -> Optional[pulumi.Input[str]]:
+        """
+        The validation information in JSON format
+        """
+        return pulumi.get(self, "validations")
+
+    @validations.setter
+    def validations(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "validations", value)
+
+    @property
+    @pulumi.getter
+    def version(self) -> Optional[pulumi.Input[int]]:
+        """
+        The unique identifier of the include
+        """
+        return pulumi.get(self, "version")
+
+    @version.setter
+    def version(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "version", value)
+
+
+class PropertyIncludeActivation(pulumi.CustomResource):
+    @overload
+    def __init__(__self__,
+                 resource_name: str,
+                 opts: Optional[pulumi.ResourceOptions] = None,
+                 auto_acknowledge_rule_warnings: Optional[pulumi.Input[bool]] = None,
+                 compliance_record: Optional[pulumi.Input[pulumi.InputType['PropertyIncludeActivationComplianceRecordArgs']]] = None,
+                 contract_id: Optional[pulumi.Input[str]] = None,
+                 group_id: Optional[pulumi.Input[str]] = None,
+                 include_id: Optional[pulumi.Input[str]] = None,
+                 network: Optional[pulumi.Input[str]] = None,
+                 note: Optional[pulumi.Input[str]] = None,
+                 notify_emails: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 version: Optional[pulumi.Input[int]] = None,
+                 __props__=None):
+        """
+        Create a PropertyIncludeActivation resource with the given unique name, props, and options.
+        :param str resource_name: The name of the resource.
+        :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[bool] auto_acknowledge_rule_warnings: Automatically acknowledge all rule warnings for activation and continue
+        :param pulumi.Input[pulumi.InputType['PropertyIncludeActivationComplianceRecordArgs']] compliance_record: Provides an audit record when activating on a production network
+        :param pulumi.Input[str] contract_id: The contract under which the include is activated
+        :param pulumi.Input[str] group_id: The group under which the include is activated
+        :param pulumi.Input[str] include_id: The unique identifier of the include
+        :param pulumi.Input[str] network: The network for which the activation will be performed
+        :param pulumi.Input[str] note: The note to assign to a log message of the activation request
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] notify_emails: The list of email addresses to notify about an activation status
+        :param pulumi.Input[int] version: The unique identifier of the include
+        """
+        ...
+    @overload
+    def __init__(__self__,
+                 resource_name: str,
+                 args: PropertyIncludeActivationArgs,
+                 opts: Optional[pulumi.ResourceOptions] = None):
+        """
+        Create a PropertyIncludeActivation resource with the given unique name, props, and options.
+        :param str resource_name: The name of the resource.
+        :param PropertyIncludeActivationArgs args: The arguments to use to populate this resource's properties.
+        :param pulumi.ResourceOptions opts: Options for the resource.
+        """
+        ...
+    def __init__(__self__, resource_name: str, *args, **kwargs):
+        resource_args, opts = _utilities.get_resource_args_opts(PropertyIncludeActivationArgs, pulumi.ResourceOptions, *args, **kwargs)
+        if resource_args is not None:
+            __self__._internal_init(resource_name, opts, **resource_args.__dict__)
+        else:
+            __self__._internal_init(resource_name, *args, **kwargs)
+
+    def _internal_init(__self__,
+                 resource_name: str,
+                 opts: Optional[pulumi.ResourceOptions] = None,
+                 auto_acknowledge_rule_warnings: Optional[pulumi.Input[bool]] = None,
+                 compliance_record: Optional[pulumi.Input[pulumi.InputType['PropertyIncludeActivationComplianceRecordArgs']]] = None,
+                 contract_id: Optional[pulumi.Input[str]] = None,
+                 group_id: Optional[pulumi.Input[str]] = None,
+                 include_id: Optional[pulumi.Input[str]] = None,
+                 network: Optional[pulumi.Input[str]] = None,
+                 note: Optional[pulumi.Input[str]] = None,
+                 notify_emails: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 version: Optional[pulumi.Input[int]] = None,
+                 __props__=None):
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
+        if not isinstance(opts, pulumi.ResourceOptions):
+            raise TypeError('Expected resource options to be a ResourceOptions instance')
+        if opts.id is None:
+            if __props__ is not None:
+                raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
+            __props__ = PropertyIncludeActivationArgs.__new__(PropertyIncludeActivationArgs)
+
+            __props__.__dict__["auto_acknowledge_rule_warnings"] = auto_acknowledge_rule_warnings
+            __props__.__dict__["compliance_record"] = compliance_record
+            if contract_id is None and not opts.urn:
+                raise TypeError("Missing required property 'contract_id'")
+            __props__.__dict__["contract_id"] = contract_id
+            if group_id is None and not opts.urn:
+                raise TypeError("Missing required property 'group_id'")
+            __props__.__dict__["group_id"] = group_id
+            if include_id is None and not opts.urn:
+                raise TypeError("Missing required property 'include_id'")
+            __props__.__dict__["include_id"] = include_id
+            if network is None and not opts.urn:
+                raise TypeError("Missing required property 'network'")
+            __props__.__dict__["network"] = network
+            __props__.__dict__["note"] = note
+            if notify_emails is None and not opts.urn:
+                raise TypeError("Missing required property 'notify_emails'")
+            __props__.__dict__["notify_emails"] = notify_emails
+            if version is None and not opts.urn:
+                raise TypeError("Missing required property 'version'")
+            __props__.__dict__["version"] = version
+            __props__.__dict__["validations"] = None
+        super(PropertyIncludeActivation, __self__).__init__(
+            'akamai:index/propertyIncludeActivation:PropertyIncludeActivation',
+            resource_name,
+            __props__,
+            opts)
 
-    @property
-    @pulumi.getter(name="cacheKeyHostname")
-    def cache_key_hostname(self) -> Optional[str]:
-        return pulumi.get(self, "cache_key_hostname")
-
-    @property
-    @pulumi.getter
-    def compress(self) -> Optional[bool]:
-        return pulumi.get(self, "compress")
-
-    @property
-    @pulumi.getter(name="enableTrueClientIp")
-    def enable_true_client_ip(self) -> Optional[bool]:
-        return pulumi.get(self, "enable_true_client_ip")
-
-    @property
-    @pulumi.getter(name="forwardHostname")
-    def forward_hostname(self) -> Optional[str]:
-        return pulumi.get(self, "forward_hostname")
-
-    @property
-    @pulumi.getter
-    def hostname(self) -> Optional[str]:
-        return pulumi.get(self, "hostname")
-
-    @property
-    @pulumi.getter
-    def port(self) -> Optional[int]:
-        return pulumi.get(self, "port")
-
-
-@pulumi.output_type
-class PropertyRuleError(dict):
     @staticmethod
-    def __key_warning(key: str):
-        suggest = None
-        if key == "behaviorName":
-            suggest = "behavior_name"
-        elif key == "errorLocation":
-            suggest = "error_location"
-        elif key == "statusCode":
-            suggest = "status_code"
-
-        if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in PropertyRuleError. Access the value via the '{suggest}' property getter instead.")
-
-    def __getitem__(self, key: str) -> Any:
-        PropertyRuleError.__key_warning(key)
-        return super().__getitem__(key)
-
-    def get(self, key: str, default = None) -> Any:
-        PropertyRuleError.__key_warning(key)
-        return super().get(key, default)
-
-    def __init__(__self__, *,
-                 behavior_name: Optional[str] = None,
-                 detail: Optional[str] = None,
-                 error_location: Optional[str] = None,
-                 instance: Optional[str] = None,
-                 status_code: Optional[int] = None,
-                 title: Optional[str] = None,
-                 type: Optional[str] = None):
-        if behavior_name is not None:
-            pulumi.set(__self__, "behavior_name", behavior_name)
-        if detail is not None:
-            pulumi.set(__self__, "detail", detail)
-        if error_location is not None:
-            pulumi.set(__self__, "error_location", error_location)
-        if instance is not None:
-            pulumi.set(__self__, "instance", instance)
-        if status_code is not None:
-            pulumi.set(__self__, "status_code", status_code)
-        if title is not None:
-            pulumi.set(__self__, "title", title)
-        if type is not None:
-            pulumi.set(__self__, "type", type)
-
-    @property
-    @pulumi.getter(name="behaviorName")
-    def behavior_name(self) -> Optional[str]:
-        return pulumi.get(self, "behavior_name")
-
-    @property
-    @pulumi.getter
-    def detail(self) -> Optional[str]:
-        return pulumi.get(self, "detail")
-
-    @property
-    @pulumi.getter(name="errorLocation")
-    def error_location(self) -> Optional[str]:
-        return pulumi.get(self, "error_location")
-
-    @property
-    @pulumi.getter
-    def instance(self) -> Optional[str]:
-        return pulumi.get(self, "instance")
-
-    @property
-    @pulumi.getter(name="statusCode")
-    def status_code(self) -> Optional[int]:
-        return pulumi.get(self, "status_code")
-
-    @property
-    @pulumi.getter
-    def title(self) -> Optional[str]:
-        return pulumi.get(self, "title")
-
-    @property
-    @pulumi.getter
-    def type(self) -> Optional[str]:
-        return pulumi.get(self, "type")
-
-
-@pulumi.output_type
-class PropertyRuleWarning(dict):
-    @staticmethod
-    def __key_warning(key: str):
-        suggest = None
-        if key == "behaviorName":
-            suggest = "behavior_name"
-        elif key == "errorLocation":
-            suggest = "error_location"
-        elif key == "statusCode":
-            suggest = "status_code"
-
-        if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in PropertyRuleWarning. Access the value via the '{suggest}' property getter instead.")
-
-    def __getitem__(self, key: str) -> Any:
-        PropertyRuleWarning.__key_warning(key)
-        return super().__getitem__(key)
-
-    def get(self, key: str, default = None) -> Any:
-        PropertyRuleWarning.__key_warning(key)
-        return super().get(key, default)
-
-    def __init__(__self__, *,
-                 behavior_name: Optional[str] = None,
-                 detail: Optional[str] = None,
-                 error_location: Optional[str] = None,
-                 instance: Optional[str] = None,
-                 status_code: Optional[int] = None,
-                 title: Optional[str] = None,
-                 type: Optional[str] = None):
-        if behavior_name is not None:
-            pulumi.set(__self__, "behavior_name", behavior_name)
-        if detail is not None:
-            pulumi.set(__self__, "detail", detail)
-        if error_location is not None:
-            pulumi.set(__self__, "error_location", error_location)
-        if instance is not None:
-            pulumi.set(__self__, "instance", instance)
-        if status_code is not None:
-            pulumi.set(__self__, "status_code", status_code)
-        if title is not None:
-            pulumi.set(__self__, "title", title)
-        if type is not None:
-            pulumi.set(__self__, "type", type)
-
-    @property
-    @pulumi.getter(name="behaviorName")
-    def behavior_name(self) -> Optional[str]:
-        return pulumi.get(self, "behavior_name")
-
-    @property
-    @pulumi.getter
-    def detail(self) -> Optional[str]:
-        return pulumi.get(self, "detail")
-
-    @property
-    @pulumi.getter(name="errorLocation")
-    def error_location(self) -> Optional[str]:
-        return pulumi.get(self, "error_location")
-
-    @property
-    @pulumi.getter
-    def instance(self) -> Optional[str]:
-        return pulumi.get(self, "instance")
-
-    @property
-    @pulumi.getter(name="statusCode")
-    def status_code(self) -> Optional[int]:
-        return pulumi.get(self, "status_code")
-
-    @property
-    @pulumi.getter
-    def title(self) -> Optional[str]:
-        return pulumi.get(self, "title")
-
-    @property
-    @pulumi.getter
-    def type(self) -> Optional[str]:
-        return pulumi.get(self, "type")
-
+    def get(resource_name: str,
+            id: pulumi.Input[str],
+            opts: Optional[pulumi.ResourceOptions] = None,
+            auto_acknowledge_rule_warnings: Optional[pulumi.Input[bool]] = None,
+            compliance_record: Optional[pulumi.Input[pulumi.InputType['PropertyIncludeActivationComplianceRecordArgs']]] = None,
+            contract_id: Optional[pulumi.Input[str]] = None,
+            group_id: Optional[pulumi.Input[str]] = None,
+            include_id: Optional[pulumi.Input[str]] = None,
+            network: Optional[pulumi.Input[str]] = None,
+            note: Optional[pulumi.Input[str]] = None,
+            notify_emails: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            validations: Optional[pulumi.Input[str]] = None,
+            version: Optional[pulumi.Input[int]] = None) -> 'PropertyIncludeActivation':
+        """
+        Get an existing PropertyIncludeActivation resource's state with the given name, id, and optional extra
+        properties used to qualify the lookup.
+
+        :param str resource_name: The unique name of the resulting resource.
+        :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
+        :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[bool] auto_acknowledge_rule_warnings: Automatically acknowledge all rule warnings for activation and continue
+        :param pulumi.Input[pulumi.InputType['PropertyIncludeActivationComplianceRecordArgs']] compliance_record: Provides an audit record when activating on a production network
+        :param pulumi.Input[str] contract_id: The contract under which the include is activated
+        :param pulumi.Input[str] group_id: The group under which the include is activated
+        :param pulumi.Input[str] include_id: The unique identifier of the include
+        :param pulumi.Input[str] network: The network for which the activation will be performed
+        :param pulumi.Input[str] note: The note to assign to a log message of the activation request
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] notify_emails: The list of email addresses to notify about an activation status
+        :param pulumi.Input[str] validations: The validation information in JSON format
+        :param pulumi.Input[int] version: The unique identifier of the include
+        """
+        opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
+
+        __props__ = _PropertyIncludeActivationState.__new__(_PropertyIncludeActivationState)
+
+        __props__.__dict__["auto_acknowledge_rule_warnings"] = auto_acknowledge_rule_warnings
+        __props__.__dict__["compliance_record"] = compliance_record
+        __props__.__dict__["contract_id"] = contract_id
+        __props__.__dict__["group_id"] = group_id
+        __props__.__dict__["include_id"] = include_id
+        __props__.__dict__["network"] = network
+        __props__.__dict__["note"] = note
+        __props__.__dict__["notify_emails"] = notify_emails
+        __props__.__dict__["validations"] = validations
+        __props__.__dict__["version"] = version
+        return PropertyIncludeActivation(resource_name, opts=opts, __props__=__props__)
+
+    @property
+    @pulumi.getter(name="autoAcknowledgeRuleWarnings")
+    def auto_acknowledge_rule_warnings(self) -> pulumi.Output[Optional[bool]]:
+        """
+        Automatically acknowledge all rule warnings for activation and continue
+        """
+        return pulumi.get(self, "auto_acknowledge_rule_warnings")
+
+    @property
+    @pulumi.getter(name="complianceRecord")
+    def compliance_record(self) -> pulumi.Output[Optional['outputs.PropertyIncludeActivationComplianceRecord']]:
+        """
+        Provides an audit record when activating on a production network
+        """
+        return pulumi.get(self, "compliance_record")
+
+    @property
+    @pulumi.getter(name="contractId")
+    def contract_id(self) -> pulumi.Output[str]:
+        """
+        The contract under which the include is activated
+        """
+        return pulumi.get(self, "contract_id")
+
+    @property
+    @pulumi.getter(name="groupId")
+    def group_id(self) -> pulumi.Output[str]:
+        """
+        The group under which the include is activated
+        """
+        return pulumi.get(self, "group_id")
+
+    @property
+    @pulumi.getter(name="includeId")
+    def include_id(self) -> pulumi.Output[str]:
+        """
+        The unique identifier of the include
+        """
+        return pulumi.get(self, "include_id")
+
+    @property
+    @pulumi.getter
+    def network(self) -> pulumi.Output[str]:
+        """
+        The network for which the activation will be performed
+        """
+        return pulumi.get(self, "network")
+
+    @property
+    @pulumi.getter
+    def note(self) -> pulumi.Output[Optional[str]]:
+        """
+        The note to assign to a log message of the activation request
+        """
+        return pulumi.get(self, "note")
+
+    @property
+    @pulumi.getter(name="notifyEmails")
+    def notify_emails(self) -> pulumi.Output[Sequence[str]]:
+        """
+        The list of email addresses to notify about an activation status
+        """
+        return pulumi.get(self, "notify_emails")
+
+    @property
+    @pulumi.getter
+    def validations(self) -> pulumi.Output[str]:
+        """
+        The validation information in JSON format
+        """
+        return pulumi.get(self, "validations")
+
+    @property
+    @pulumi.getter
+    def version(self) -> pulumi.Output[int]:
+        """
+        The unique identifier of the include
+        """
+        return pulumi.get(self, "version")
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/properties/property.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/property.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from .. import _utilities
+from . import _utilities
 from . import outputs
 from ._inputs import *
 
 __all__ = ['PropertyArgs', 'Property']
 
 @pulumi.input_type
 class PropertyArgs:
@@ -100,23 +100,29 @@
             pulumi.log.warn("""variables is deprecated: The setting \"variables\" has been deprecated.""")
         if variables is not None:
             pulumi.set(__self__, "variables", variables)
 
     @property
     @pulumi.getter
     def contacts(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        warnings.warn("""The setting \"contact\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""contacts is deprecated: The setting \"contact\" has been deprecated.""")
+
         return pulumi.get(self, "contacts")
 
     @contacts.setter
     def contacts(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "contacts", value)
 
     @property
     @pulumi.getter
     def contract(self) -> Optional[pulumi.Input[str]]:
+        warnings.warn("""The setting \"contract\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""contract is deprecated: The setting \"contract\" has been deprecated.""")
+
         return pulumi.get(self, "contract")
 
     @contract.setter
     def contract(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "contract", value)
 
     @property
@@ -130,23 +136,29 @@
     @contract_id.setter
     def contract_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "contract_id", value)
 
     @property
     @pulumi.getter(name="cpCode")
     def cp_code(self) -> Optional[pulumi.Input[str]]:
+        warnings.warn("""The setting \"cp_code\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""cp_code is deprecated: The setting \"cp_code\" has been deprecated.""")
+
         return pulumi.get(self, "cp_code")
 
     @cp_code.setter
     def cp_code(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cp_code", value)
 
     @property
     @pulumi.getter
     def group(self) -> Optional[pulumi.Input[str]]:
+        warnings.warn("""The setting \"group\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""group is deprecated: The setting \"group\" has been deprecated.""")
+
         return pulumi.get(self, "group")
 
     @group.setter
     def group(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "group", value)
 
     @property
@@ -169,14 +181,17 @@
     @hostnames.setter
     def hostnames(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PropertyHostnameArgs']]]]):
         pulumi.set(self, "hostnames", value)
 
     @property
     @pulumi.getter(name="isSecure")
     def is_secure(self) -> Optional[pulumi.Input[bool]]:
+        warnings.warn("""The setting \"is_secure\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""is_secure is deprecated: The setting \"is_secure\" has been deprecated.""")
+
         return pulumi.get(self, "is_secure")
 
     @is_secure.setter
     def is_secure(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "is_secure", value)
 
     @property
@@ -190,23 +205,29 @@
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def origins(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PropertyOriginArgs']]]]:
+        warnings.warn("""The setting \"origin\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""origins is deprecated: The setting \"origin\" has been deprecated.""")
+
         return pulumi.get(self, "origins")
 
     @origins.setter
     def origins(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PropertyOriginArgs']]]]):
         pulumi.set(self, "origins", value)
 
     @property
     @pulumi.getter
     def product(self) -> Optional[pulumi.Input[str]]:
+        warnings.warn("""The setting \"product\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""product is deprecated: The setting \"product\" has been deprecated.""")
+
         return pulumi.get(self, "product")
 
     @product.setter
     def product(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "product", value)
 
     @property
@@ -232,14 +253,17 @@
     @rule_format.setter
     def rule_format(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "rule_format", value)
 
     @property
     @pulumi.getter(name="ruleWarnings")
     def rule_warnings(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PropertyRuleWarningArgs']]]]:
+        warnings.warn("""Rule warnings will not be set in state anymore""", DeprecationWarning)
+        pulumi.log.warn("""rule_warnings is deprecated: Rule warnings will not be set in state anymore""")
+
         return pulumi.get(self, "rule_warnings")
 
     @rule_warnings.setter
     def rule_warnings(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PropertyRuleWarningArgs']]]]):
         pulumi.set(self, "rule_warnings", value)
 
     @property
@@ -253,14 +277,17 @@
     @rules.setter
     def rules(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "rules", value)
 
     @property
     @pulumi.getter
     def variables(self) -> Optional[pulumi.Input[str]]:
+        warnings.warn("""The setting \"variables\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""variables is deprecated: The setting \"variables\" has been deprecated.""")
+
         return pulumi.get(self, "variables")
 
     @variables.setter
     def variables(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "variables", value)
 
 
@@ -370,23 +397,29 @@
             pulumi.log.warn("""variables is deprecated: The setting \"variables\" has been deprecated.""")
         if variables is not None:
             pulumi.set(__self__, "variables", variables)
 
     @property
     @pulumi.getter
     def contacts(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        warnings.warn("""The setting \"contact\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""contacts is deprecated: The setting \"contact\" has been deprecated.""")
+
         return pulumi.get(self, "contacts")
 
     @contacts.setter
     def contacts(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "contacts", value)
 
     @property
     @pulumi.getter
     def contract(self) -> Optional[pulumi.Input[str]]:
+        warnings.warn("""The setting \"contract\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""contract is deprecated: The setting \"contract\" has been deprecated.""")
+
         return pulumi.get(self, "contract")
 
     @contract.setter
     def contract(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "contract", value)
 
     @property
@@ -400,23 +433,29 @@
     @contract_id.setter
     def contract_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "contract_id", value)
 
     @property
     @pulumi.getter(name="cpCode")
     def cp_code(self) -> Optional[pulumi.Input[str]]:
+        warnings.warn("""The setting \"cp_code\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""cp_code is deprecated: The setting \"cp_code\" has been deprecated.""")
+
         return pulumi.get(self, "cp_code")
 
     @cp_code.setter
     def cp_code(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cp_code", value)
 
     @property
     @pulumi.getter
     def group(self) -> Optional[pulumi.Input[str]]:
+        warnings.warn("""The setting \"group\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""group is deprecated: The setting \"group\" has been deprecated.""")
+
         return pulumi.get(self, "group")
 
     @group.setter
     def group(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "group", value)
 
     @property
@@ -439,14 +478,17 @@
     @hostnames.setter
     def hostnames(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PropertyHostnameArgs']]]]):
         pulumi.set(self, "hostnames", value)
 
     @property
     @pulumi.getter(name="isSecure")
     def is_secure(self) -> Optional[pulumi.Input[bool]]:
+        warnings.warn("""The setting \"is_secure\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""is_secure is deprecated: The setting \"is_secure\" has been deprecated.""")
+
         return pulumi.get(self, "is_secure")
 
     @is_secure.setter
     def is_secure(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "is_secure", value)
 
     @property
@@ -472,23 +514,29 @@
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def origins(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PropertyOriginArgs']]]]:
+        warnings.warn("""The setting \"origin\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""origins is deprecated: The setting \"origin\" has been deprecated.""")
+
         return pulumi.get(self, "origins")
 
     @origins.setter
     def origins(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PropertyOriginArgs']]]]):
         pulumi.set(self, "origins", value)
 
     @property
     @pulumi.getter
     def product(self) -> Optional[pulumi.Input[str]]:
+        warnings.warn("""The setting \"product\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""product is deprecated: The setting \"product\" has been deprecated.""")
+
         return pulumi.get(self, "product")
 
     @product.setter
     def product(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "product", value)
 
     @property
@@ -547,14 +595,17 @@
     @rule_format.setter
     def rule_format(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "rule_format", value)
 
     @property
     @pulumi.getter(name="ruleWarnings")
     def rule_warnings(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PropertyRuleWarningArgs']]]]:
+        warnings.warn("""Rule warnings will not be set in state anymore""", DeprecationWarning)
+        pulumi.log.warn("""rule_warnings is deprecated: Rule warnings will not be set in state anymore""")
+
         return pulumi.get(self, "rule_warnings")
 
     @rule_warnings.setter
     def rule_warnings(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PropertyRuleWarningArgs']]]]):
         pulumi.set(self, "rule_warnings", value)
 
     @property
@@ -580,27 +631,25 @@
     @staging_version.setter
     def staging_version(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "staging_version", value)
 
     @property
     @pulumi.getter
     def variables(self) -> Optional[pulumi.Input[str]]:
+        warnings.warn("""The setting \"variables\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""variables is deprecated: The setting \"variables\" has been deprecated.""")
+
         return pulumi.get(self, "variables")
 
     @variables.setter
     def variables(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "variables", value)
 
 
-warnings.warn("""akamai.properties/property.Property has been deprecated in favor of akamai.index/property.Property""", DeprecationWarning)
-
-
 class Property(pulumi.CustomResource):
-    warnings.warn("""akamai.properties/property.Property has been deprecated in favor of akamai.index/property.Property""", DeprecationWarning)
-
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  contacts: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  contract: Optional[pulumi.Input[str]] = None,
                  contract_id: Optional[pulumi.Input[str]] = None,
@@ -665,15 +714,14 @@
                  product: Optional[pulumi.Input[str]] = None,
                  product_id: Optional[pulumi.Input[str]] = None,
                  rule_format: Optional[pulumi.Input[str]] = None,
                  rule_warnings: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PropertyRuleWarningArgs']]]]] = None,
                  rules: Optional[pulumi.Input[str]] = None,
                  variables: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        pulumi.log.warn("""Property is deprecated: akamai.properties/property.Property has been deprecated in favor of akamai.index/property.Property""")
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = PropertyArgs.__new__(PropertyArgs)
@@ -722,16 +770,18 @@
                 pulumi.log.warn("""variables is deprecated: The setting \"variables\" has been deprecated.""")
             __props__.__dict__["variables"] = variables
             __props__.__dict__["latest_version"] = None
             __props__.__dict__["production_version"] = None
             __props__.__dict__["read_version"] = None
             __props__.__dict__["rule_errors"] = None
             __props__.__dict__["staging_version"] = None
+        alias_opts = pulumi.ResourceOptions(aliases=[pulumi.Alias(type_="akamai:properties/property:Property")])
+        opts = pulumi.ResourceOptions.merge(opts, alias_opts)
         super(Property, __self__).__init__(
-            'akamai:properties/property:Property',
+            'akamai:index/property:Property',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
@@ -801,37 +851,49 @@
         __props__.__dict__["staging_version"] = staging_version
         __props__.__dict__["variables"] = variables
         return Property(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def contacts(self) -> pulumi.Output[Optional[Sequence[str]]]:
+        warnings.warn("""The setting \"contact\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""contacts is deprecated: The setting \"contact\" has been deprecated.""")
+
         return pulumi.get(self, "contacts")
 
     @property
     @pulumi.getter
     def contract(self) -> pulumi.Output[str]:
+        warnings.warn("""The setting \"contract\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""contract is deprecated: The setting \"contract\" has been deprecated.""")
+
         return pulumi.get(self, "contract")
 
     @property
     @pulumi.getter(name="contractId")
     def contract_id(self) -> pulumi.Output[str]:
         """
         Contract ID to be assigned to the Property
         """
         return pulumi.get(self, "contract_id")
 
     @property
     @pulumi.getter(name="cpCode")
     def cp_code(self) -> pulumi.Output[Optional[str]]:
+        warnings.warn("""The setting \"cp_code\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""cp_code is deprecated: The setting \"cp_code\" has been deprecated.""")
+
         return pulumi.get(self, "cp_code")
 
     @property
     @pulumi.getter
     def group(self) -> pulumi.Output[str]:
+        warnings.warn("""The setting \"group\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""group is deprecated: The setting \"group\" has been deprecated.""")
+
         return pulumi.get(self, "group")
 
     @property
     @pulumi.getter(name="groupId")
     def group_id(self) -> pulumi.Output[str]:
         """
         Group ID to be assigned to the Property
@@ -842,14 +904,17 @@
     @pulumi.getter
     def hostnames(self) -> pulumi.Output[Optional[Sequence['outputs.PropertyHostname']]]:
         return pulumi.get(self, "hostnames")
 
     @property
     @pulumi.getter(name="isSecure")
     def is_secure(self) -> pulumi.Output[Optional[bool]]:
+        warnings.warn("""The setting \"is_secure\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""is_secure is deprecated: The setting \"is_secure\" has been deprecated.""")
+
         return pulumi.get(self, "is_secure")
 
     @property
     @pulumi.getter(name="latestVersion")
     def latest_version(self) -> pulumi.Output[int]:
         """
         Property's current latest version number
@@ -863,19 +928,25 @@
         Name to give to the Property (must be unique)
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def origins(self) -> pulumi.Output[Optional[Sequence['outputs.PropertyOrigin']]]:
+        warnings.warn("""The setting \"origin\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""origins is deprecated: The setting \"origin\" has been deprecated.""")
+
         return pulumi.get(self, "origins")
 
     @property
     @pulumi.getter
     def product(self) -> pulumi.Output[str]:
+        warnings.warn("""The setting \"product\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""product is deprecated: The setting \"product\" has been deprecated.""")
+
         return pulumi.get(self, "product")
 
     @property
     @pulumi.getter(name="productId")
     def product_id(self) -> pulumi.Output[str]:
         """
         Product ID to be assigned to the Property
@@ -910,14 +981,17 @@
         Specify the rule format version (defaults to latest version available when created)
         """
         return pulumi.get(self, "rule_format")
 
     @property
     @pulumi.getter(name="ruleWarnings")
     def rule_warnings(self) -> pulumi.Output[Sequence['outputs.PropertyRuleWarning']]:
+        warnings.warn("""Rule warnings will not be set in state anymore""", DeprecationWarning)
+        pulumi.log.warn("""rule_warnings is deprecated: Rule warnings will not be set in state anymore""")
+
         return pulumi.get(self, "rule_warnings")
 
     @property
     @pulumi.getter
     def rules(self) -> pulumi.Output[str]:
         """
         Property Rules as JSON
@@ -931,9 +1005,12 @@
         Property's version currently activated in staging (zero when not active in staging)
         """
         return pulumi.get(self, "staging_version")
 
     @property
     @pulumi.getter
     def variables(self) -> pulumi.Output[Optional[str]]:
+        warnings.warn("""The setting \"variables\" has been deprecated.""", DeprecationWarning)
+        pulumi.log.warn("""variables is deprecated: The setting \"variables\" has been deprecated.""")
+
         return pulumi.get(self, "variables")
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/trafficmanagement/get_gtm_default_datacenter.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/trafficmanagement/get_gtm_default_datacenter.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,19 +92,19 @@
     __args__ = dict()
     __args__['datacenter'] = datacenter
     __args__['domain'] = domain
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:trafficmanagement/getGtmDefaultDatacenter:getGtmDefaultDatacenter', __args__, opts=opts, typ=GetGtmDefaultDatacenterResult).value
 
     return AwaitableGetGtmDefaultDatacenterResult(
-        datacenter=__ret__.datacenter,
-        datacenter_id=__ret__.datacenter_id,
-        domain=__ret__.domain,
-        id=__ret__.id,
-        nickname=__ret__.nickname)
+        datacenter=pulumi.get(__ret__, 'datacenter'),
+        datacenter_id=pulumi.get(__ret__, 'datacenter_id'),
+        domain=pulumi.get(__ret__, 'domain'),
+        id=pulumi.get(__ret__, 'id'),
+        nickname=pulumi.get(__ret__, 'nickname'))
 
 
 @_utilities.lift_output_func(get_gtm_default_datacenter)
 def get_gtm_default_datacenter_output(datacenter: Optional[pulumi.Input[Optional[int]]] = None,
                                       domain: Optional[pulumi.Input[str]] = None,
                                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetGtmDefaultDatacenterResult]:
     """
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/trafficmanagement/gtm_a_smap.py` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai/botman_custom_bot_category_action.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,274 +3,234 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from .. import _utilities
-from . import outputs
-from ._inputs import *
+from . import _utilities
 
-__all__ = ['GtmASmapArgs', 'GtmASmap']
+__all__ = ['BotmanCustomBotCategoryActionArgs', 'BotmanCustomBotCategoryAction']
 
 @pulumi.input_type
-class GtmASmapArgs:
+class BotmanCustomBotCategoryActionArgs:
     def __init__(__self__, *,
-                 default_datacenter: pulumi.Input['GtmASmapDefaultDatacenterArgs'],
-                 domain: pulumi.Input[str],
-                 assignments: Optional[pulumi.Input[Sequence[pulumi.Input['GtmASmapAssignmentArgs']]]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 wait_on_complete: Optional[pulumi.Input[bool]] = None):
+                 category_id: pulumi.Input[str],
+                 config_id: pulumi.Input[int],
+                 custom_bot_category_action: pulumi.Input[str],
+                 security_policy_id: pulumi.Input[str]):
         """
-        The set of arguments for constructing a GtmASmap resource.
+        The set of arguments for constructing a BotmanCustomBotCategoryAction resource.
         """
-        pulumi.set(__self__, "default_datacenter", default_datacenter)
-        pulumi.set(__self__, "domain", domain)
-        if assignments is not None:
-            pulumi.set(__self__, "assignments", assignments)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
-        if wait_on_complete is not None:
-            pulumi.set(__self__, "wait_on_complete", wait_on_complete)
+        pulumi.set(__self__, "category_id", category_id)
+        pulumi.set(__self__, "config_id", config_id)
+        pulumi.set(__self__, "custom_bot_category_action", custom_bot_category_action)
+        pulumi.set(__self__, "security_policy_id", security_policy_id)
 
     @property
-    @pulumi.getter(name="defaultDatacenter")
-    def default_datacenter(self) -> pulumi.Input['GtmASmapDefaultDatacenterArgs']:
-        return pulumi.get(self, "default_datacenter")
+    @pulumi.getter(name="categoryId")
+    def category_id(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "category_id")
 
-    @default_datacenter.setter
-    def default_datacenter(self, value: pulumi.Input['GtmASmapDefaultDatacenterArgs']):
-        pulumi.set(self, "default_datacenter", value)
+    @category_id.setter
+    def category_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "category_id", value)
 
     @property
-    @pulumi.getter
-    def domain(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "domain")
+    @pulumi.getter(name="configId")
+    def config_id(self) -> pulumi.Input[int]:
+        return pulumi.get(self, "config_id")
 
-    @domain.setter
-    def domain(self, value: pulumi.Input[str]):
-        pulumi.set(self, "domain", value)
+    @config_id.setter
+    def config_id(self, value: pulumi.Input[int]):
+        pulumi.set(self, "config_id", value)
 
     @property
-    @pulumi.getter
-    def assignments(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['GtmASmapAssignmentArgs']]]]:
-        return pulumi.get(self, "assignments")
+    @pulumi.getter(name="customBotCategoryAction")
+    def custom_bot_category_action(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "custom_bot_category_action")
 
-    @assignments.setter
-    def assignments(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['GtmASmapAssignmentArgs']]]]):
-        pulumi.set(self, "assignments", value)
+    @custom_bot_category_action.setter
+    def custom_bot_category_action(self, value: pulumi.Input[str]):
+        pulumi.set(self, "custom_bot_category_action", value)
 
     @property
-    @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "name")
+    @pulumi.getter(name="securityPolicyId")
+    def security_policy_id(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "security_policy_id")
 
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
-
-    @property
-    @pulumi.getter(name="waitOnComplete")
-    def wait_on_complete(self) -> Optional[pulumi.Input[bool]]:
-        return pulumi.get(self, "wait_on_complete")
-
-    @wait_on_complete.setter
-    def wait_on_complete(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "wait_on_complete", value)
+    @security_policy_id.setter
+    def security_policy_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "security_policy_id", value)
 
 
 @pulumi.input_type
-class _GtmASmapState:
+class _BotmanCustomBotCategoryActionState:
     def __init__(__self__, *,
-                 assignments: Optional[pulumi.Input[Sequence[pulumi.Input['GtmASmapAssignmentArgs']]]] = None,
-                 default_datacenter: Optional[pulumi.Input['GtmASmapDefaultDatacenterArgs']] = None,
-                 domain: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 wait_on_complete: Optional[pulumi.Input[bool]] = None):
+                 category_id: Optional[pulumi.Input[str]] = None,
+                 config_id: Optional[pulumi.Input[int]] = None,
+                 custom_bot_category_action: Optional[pulumi.Input[str]] = None,
+                 security_policy_id: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering GtmASmap resources.
+        Input properties used for looking up and filtering BotmanCustomBotCategoryAction resources.
         """
-        if assignments is not None:
-            pulumi.set(__self__, "assignments", assignments)
-        if default_datacenter is not None:
-            pulumi.set(__self__, "default_datacenter", default_datacenter)
-        if domain is not None:
-            pulumi.set(__self__, "domain", domain)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
-        if wait_on_complete is not None:
-            pulumi.set(__self__, "wait_on_complete", wait_on_complete)
-
-    @property
-    @pulumi.getter
-    def assignments(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['GtmASmapAssignmentArgs']]]]:
-        return pulumi.get(self, "assignments")
-
-    @assignments.setter
-    def assignments(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['GtmASmapAssignmentArgs']]]]):
-        pulumi.set(self, "assignments", value)
+        if category_id is not None:
+            pulumi.set(__self__, "category_id", category_id)
+        if config_id is not None:
+            pulumi.set(__self__, "config_id", config_id)
+        if custom_bot_category_action is not None:
+            pulumi.set(__self__, "custom_bot_category_action", custom_bot_category_action)
+        if security_policy_id is not None:
+            pulumi.set(__self__, "security_policy_id", security_policy_id)
 
     @property
-    @pulumi.getter(name="defaultDatacenter")
-    def default_datacenter(self) -> Optional[pulumi.Input['GtmASmapDefaultDatacenterArgs']]:
-        return pulumi.get(self, "default_datacenter")
+    @pulumi.getter(name="categoryId")
+    def category_id(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "category_id")
 
-    @default_datacenter.setter
-    def default_datacenter(self, value: Optional[pulumi.Input['GtmASmapDefaultDatacenterArgs']]):
-        pulumi.set(self, "default_datacenter", value)
+    @category_id.setter
+    def category_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "category_id", value)
 
     @property
-    @pulumi.getter
-    def domain(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "domain")
+    @pulumi.getter(name="configId")
+    def config_id(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "config_id")
 
-    @domain.setter
-    def domain(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "domain", value)
+    @config_id.setter
+    def config_id(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "config_id", value)
 
     @property
-    @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "name")
+    @pulumi.getter(name="customBotCategoryAction")
+    def custom_bot_category_action(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "custom_bot_category_action")
 
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
+    @custom_bot_category_action.setter
+    def custom_bot_category_action(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "custom_bot_category_action", value)
 
     @property
-    @pulumi.getter(name="waitOnComplete")
-    def wait_on_complete(self) -> Optional[pulumi.Input[bool]]:
-        return pulumi.get(self, "wait_on_complete")
+    @pulumi.getter(name="securityPolicyId")
+    def security_policy_id(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "security_policy_id")
 
-    @wait_on_complete.setter
-    def wait_on_complete(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "wait_on_complete", value)
+    @security_policy_id.setter
+    def security_policy_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "security_policy_id", value)
 
 
-warnings.warn("""akamai.trafficmanagement/gtmasmap.GtmASmap has been deprecated in favor of akamai.index/gtmasmap.GtmAsmap""", DeprecationWarning)
-
-
-class GtmASmap(pulumi.CustomResource):
-    warnings.warn("""akamai.trafficmanagement/gtmasmap.GtmASmap has been deprecated in favor of akamai.index/gtmasmap.GtmAsmap""", DeprecationWarning)
-
+class BotmanCustomBotCategoryAction(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 assignments: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['GtmASmapAssignmentArgs']]]]] = None,
-                 default_datacenter: Optional[pulumi.Input[pulumi.InputType['GtmASmapDefaultDatacenterArgs']]] = None,
-                 domain: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 wait_on_complete: Optional[pulumi.Input[bool]] = None,
+                 category_id: Optional[pulumi.Input[str]] = None,
+                 config_id: Optional[pulumi.Input[int]] = None,
+                 custom_bot_category_action: Optional[pulumi.Input[str]] = None,
+                 security_policy_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Create a GtmASmap resource with the given unique name, props, and options.
+        Create a BotmanCustomBotCategoryAction resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: GtmASmapArgs,
+                 args: BotmanCustomBotCategoryActionArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a GtmASmap resource with the given unique name, props, and options.
+        Create a BotmanCustomBotCategoryAction resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
-        :param GtmASmapArgs args: The arguments to use to populate this resource's properties.
+        :param BotmanCustomBotCategoryActionArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(GtmASmapArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(BotmanCustomBotCategoryActionArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 assignments: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['GtmASmapAssignmentArgs']]]]] = None,
-                 default_datacenter: Optional[pulumi.Input[pulumi.InputType['GtmASmapDefaultDatacenterArgs']]] = None,
-                 domain: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 wait_on_complete: Optional[pulumi.Input[bool]] = None,
+                 category_id: Optional[pulumi.Input[str]] = None,
+                 config_id: Optional[pulumi.Input[int]] = None,
+                 custom_bot_category_action: Optional[pulumi.Input[str]] = None,
+                 security_policy_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        pulumi.log.warn("""GtmASmap is deprecated: akamai.trafficmanagement/gtmasmap.GtmASmap has been deprecated in favor of akamai.index/gtmasmap.GtmAsmap""")
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = GtmASmapArgs.__new__(GtmASmapArgs)
+            __props__ = BotmanCustomBotCategoryActionArgs.__new__(BotmanCustomBotCategoryActionArgs)
 
-            __props__.__dict__["assignments"] = assignments
-            if default_datacenter is None and not opts.urn:
-                raise TypeError("Missing required property 'default_datacenter'")
-            __props__.__dict__["default_datacenter"] = default_datacenter
-            if domain is None and not opts.urn:
-                raise TypeError("Missing required property 'domain'")
-            __props__.__dict__["domain"] = domain
-            __props__.__dict__["name"] = name
-            __props__.__dict__["wait_on_complete"] = wait_on_complete
-        super(GtmASmap, __self__).__init__(
-            'akamai:trafficmanagement/gtmASmap:GtmASmap',
+            if category_id is None and not opts.urn:
+                raise TypeError("Missing required property 'category_id'")
+            __props__.__dict__["category_id"] = category_id
+            if config_id is None and not opts.urn:
+                raise TypeError("Missing required property 'config_id'")
+            __props__.__dict__["config_id"] = config_id
+            if custom_bot_category_action is None and not opts.urn:
+                raise TypeError("Missing required property 'custom_bot_category_action'")
+            __props__.__dict__["custom_bot_category_action"] = custom_bot_category_action
+            if security_policy_id is None and not opts.urn:
+                raise TypeError("Missing required property 'security_policy_id'")
+            __props__.__dict__["security_policy_id"] = security_policy_id
+        super(BotmanCustomBotCategoryAction, __self__).__init__(
+            'akamai:index/botmanCustomBotCategoryAction:BotmanCustomBotCategoryAction',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            assignments: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['GtmASmapAssignmentArgs']]]]] = None,
-            default_datacenter: Optional[pulumi.Input[pulumi.InputType['GtmASmapDefaultDatacenterArgs']]] = None,
-            domain: Optional[pulumi.Input[str]] = None,
-            name: Optional[pulumi.Input[str]] = None,
-            wait_on_complete: Optional[pulumi.Input[bool]] = None) -> 'GtmASmap':
+            category_id: Optional[pulumi.Input[str]] = None,
+            config_id: Optional[pulumi.Input[int]] = None,
+            custom_bot_category_action: Optional[pulumi.Input[str]] = None,
+            security_policy_id: Optional[pulumi.Input[str]] = None) -> 'BotmanCustomBotCategoryAction':
         """
-        Get an existing GtmASmap resource's state with the given name, id, and optional extra
+        Get an existing BotmanCustomBotCategoryAction resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _GtmASmapState.__new__(_GtmASmapState)
+        __props__ = _BotmanCustomBotCategoryActionState.__new__(_BotmanCustomBotCategoryActionState)
 
-        __props__.__dict__["assignments"] = assignments
-        __props__.__dict__["default_datacenter"] = default_datacenter
-        __props__.__dict__["domain"] = domain
-        __props__.__dict__["name"] = name
-        __props__.__dict__["wait_on_complete"] = wait_on_complete
-        return GtmASmap(resource_name, opts=opts, __props__=__props__)
-
-    @property
-    @pulumi.getter
-    def assignments(self) -> pulumi.Output[Optional[Sequence['outputs.GtmASmapAssignment']]]:
-        return pulumi.get(self, "assignments")
+        __props__.__dict__["category_id"] = category_id
+        __props__.__dict__["config_id"] = config_id
+        __props__.__dict__["custom_bot_category_action"] = custom_bot_category_action
+        __props__.__dict__["security_policy_id"] = security_policy_id
+        return BotmanCustomBotCategoryAction(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter(name="defaultDatacenter")
-    def default_datacenter(self) -> pulumi.Output['outputs.GtmASmapDefaultDatacenter']:
-        return pulumi.get(self, "default_datacenter")
+    @pulumi.getter(name="categoryId")
+    def category_id(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "category_id")
 
     @property
-    @pulumi.getter
-    def domain(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "domain")
+    @pulumi.getter(name="configId")
+    def config_id(self) -> pulumi.Output[int]:
+        return pulumi.get(self, "config_id")
 
     @property
-    @pulumi.getter
-    def name(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "name")
+    @pulumi.getter(name="customBotCategoryAction")
+    def custom_bot_category_action(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "custom_bot_category_action")
 
     @property
-    @pulumi.getter(name="waitOnComplete")
-    def wait_on_complete(self) -> pulumi.Output[Optional[bool]]:
-        return pulumi.get(self, "wait_on_complete")
+    @pulumi.getter(name="securityPolicyId")
+    def security_policy_id(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "security_policy_id")
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai.egg-info/PKG-INFO` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-akamai
-Version: 4.6.0a1688398728
+Version: 5.0.0a1688662273
 Summary: A Pulumi package for creating and managing akamai cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-akamai
 Keywords: pulumi akamai
 Platform: UNKNOWN
 Requires-Python: >=3.7
@@ -34,15 +34,15 @@
 
     $ pip install pulumi_akamai
 
 ### Go
 
 To use from Go, use `go get` to grab the latest version of the library
 
-    $ go get github.com/pulumi/pulumi-akamai/sdk/v4
+    $ go get github.com/pulumi/pulumi-akamai/sdk/v5
 
 ### .NET
 
 To use from .NET, install using `dotnet add package`:
 
     $ dotnet add package Pulumi.Akamai
```

### Comparing `pulumi_akamai-4.6.0a1688398728/pulumi_akamai.egg-info/SOURCES.txt` & `pulumi_akamai-5.0.0a1688662273/pulumi_akamai.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -48,14 +48,34 @@
 pulumi_akamai/app_sec_threat_intel.py
 pulumi_akamai/app_sec_version_nodes.py
 pulumi_akamai/app_sec_waf_mode.py
 pulumi_akamai/app_sec_waf_protection.py
 pulumi_akamai/app_sec_wap_selected_hostnames.py
 pulumi_akamai/appsec_advanced_settings_attack_payload_logging.py
 pulumi_akamai/appsec_advanced_settings_request_body.py
+pulumi_akamai/botman_akamai_bot_category_action.py
+pulumi_akamai/botman_bot_analytics_cookie.py
+pulumi_akamai/botman_bot_category_exception.py
+pulumi_akamai/botman_bot_detection_action.py
+pulumi_akamai/botman_bot_management_settings.py
+pulumi_akamai/botman_challenge_action.py
+pulumi_akamai/botman_challenge_interception_rules.py
+pulumi_akamai/botman_client_side_security.py
+pulumi_akamai/botman_conditional_action.py
+pulumi_akamai/botman_custom_bot_category.py
+pulumi_akamai/botman_custom_bot_category_action.py
+pulumi_akamai/botman_custom_bot_category_sequence.py
+pulumi_akamai/botman_custom_client.py
+pulumi_akamai/botman_custom_defined_bot.py
+pulumi_akamai/botman_custom_deny_action.py
+pulumi_akamai/botman_javascript_injection.py
+pulumi_akamai/botman_recategorized_akamai_defined_bot.py
+pulumi_akamai/botman_serve_alternate_action.py
+pulumi_akamai/botman_transactional_endpoint.py
+pulumi_akamai/botman_transactional_endpoint_protection.py
 pulumi_akamai/cloudlets_application_load_balancer.py
 pulumi_akamai/cloudlets_application_load_balancer_activation.py
 pulumi_akamai/cloudlets_policy.py
 pulumi_akamai/cloudlets_policy_activation.py
 pulumi_akamai/cp_code.py
 pulumi_akamai/cps_dv_enrollment.py
 pulumi_akamai/cps_dv_validation.py
@@ -116,14 +136,40 @@
 pulumi_akamai/get_app_sec_tuning_recommendations.py
 pulumi_akamai/get_app_sec_version_notes.py
 pulumi_akamai/get_app_sec_waf_mode.py
 pulumi_akamai/get_app_sec_wap_selected_hostnames.py
 pulumi_akamai/get_appsec_advanced_settings_attack_payload_logging.py
 pulumi_akamai/get_appsec_advanced_settings_request_body.py
 pulumi_akamai/get_authorities_set.py
+pulumi_akamai/get_botman_akamai_bot_category.py
+pulumi_akamai/get_botman_akamai_bot_category_action.py
+pulumi_akamai/get_botman_akamai_defined_bot.py
+pulumi_akamai/get_botman_bot_analytics_cookie.py
+pulumi_akamai/get_botman_bot_analytics_cookie_values.py
+pulumi_akamai/get_botman_bot_category_exception.py
+pulumi_akamai/get_botman_bot_detection.py
+pulumi_akamai/get_botman_bot_detection_action.py
+pulumi_akamai/get_botman_bot_endpoint_coverage_report.py
+pulumi_akamai/get_botman_bot_management_settings.py
+pulumi_akamai/get_botman_challenge_action.py
+pulumi_akamai/get_botman_challenge_interception_rules.py
+pulumi_akamai/get_botman_client_side_security.py
+pulumi_akamai/get_botman_conditional_action.py
+pulumi_akamai/get_botman_custom_bot_category.py
+pulumi_akamai/get_botman_custom_bot_category_action.py
+pulumi_akamai/get_botman_custom_bot_category_sequence.py
+pulumi_akamai/get_botman_custom_client.py
+pulumi_akamai/get_botman_custom_defined_bot.py
+pulumi_akamai/get_botman_custom_deny_action.py
+pulumi_akamai/get_botman_javascript_injection.py
+pulumi_akamai/get_botman_recategorized_akamai_defined_bot.py
+pulumi_akamai/get_botman_response_action.py
+pulumi_akamai/get_botman_serve_alternate_action.py
+pulumi_akamai/get_botman_transactional_endpoint.py
+pulumi_akamai/get_botman_transactional_endpoint_protection.py
 pulumi_akamai/get_cloudlets_api_prioritization_match_rule.py
 pulumi_akamai/get_cloudlets_application_load_balancer.py
 pulumi_akamai/get_cloudlets_application_load_balancer_match_rule.py
 pulumi_akamai/get_cloudlets_audience_segmentation_match_rule.py
 pulumi_akamai/get_cloudlets_edge_redirector_match_rule.py
 pulumi_akamai/get_cloudlets_forward_rewrite_match_rule.py
 pulumi_akamai/get_cloudlets_phased_release_match_rule.py
@@ -146,14 +192,16 @@
 pulumi_akamai/get_edge_worker_activation.py
 pulumi_akamai/get_edge_workers_property_rules.py
 pulumi_akamai/get_edge_workers_resource_tier.py
 pulumi_akamai/get_edgekv_group_items.py
 pulumi_akamai/get_edgekv_groups.py
 pulumi_akamai/get_group.py
 pulumi_akamai/get_groups.py
+pulumi_akamai/get_gtm_datacenter.py
+pulumi_akamai/get_gtm_datacenters.py
 pulumi_akamai/get_gtm_default_datacenter.py
 pulumi_akamai/get_iam_contact_types.py
 pulumi_akamai/get_iam_countries.py
 pulumi_akamai/get_iam_grantable_roles.py
 pulumi_akamai/get_iam_roles.py
 pulumi_akamai/get_iam_states.py
 pulumi_akamai/get_iam_supported_langs.py
@@ -204,35 +252,16 @@
 pulumi_akamai.egg-info/not-zip-safe
 pulumi_akamai.egg-info/requires.txt
 pulumi_akamai.egg-info/top_level.txt
 pulumi_akamai/config/__init__.py
 pulumi_akamai/config/outputs.py
 pulumi_akamai/config/vars.py
 pulumi_akamai/edgedns/__init__.py
-pulumi_akamai/edgedns/_inputs.py
-pulumi_akamai/edgedns/dns_record.py
-pulumi_akamai/edgedns/dns_zone.py
 pulumi_akamai/edgedns/get_authorities_set.py
 pulumi_akamai/edgedns/get_dns_record_set.py
-pulumi_akamai/edgedns/outputs.py
 pulumi_akamai/properties/__init__.py
-pulumi_akamai/properties/_inputs.py
-pulumi_akamai/properties/cp_code.py
-pulumi_akamai/properties/edge_host_name.py
 pulumi_akamai/properties/get_activation.py
 pulumi_akamai/properties/get_cp_code.py
 pulumi_akamai/properties/get_property.py
 pulumi_akamai/properties/get_property_rules.py
-pulumi_akamai/properties/outputs.py
-pulumi_akamai/properties/property.py
-pulumi_akamai/properties/property_activation.py
 pulumi_akamai/trafficmanagement/__init__.py
-pulumi_akamai/trafficmanagement/_inputs.py
-pulumi_akamai/trafficmanagement/get_gtm_default_datacenter.py
-pulumi_akamai/trafficmanagement/gtm_a_smap.py
-pulumi_akamai/trafficmanagement/gtm_cidrmap.py
-pulumi_akamai/trafficmanagement/gtm_datacenter.py
-pulumi_akamai/trafficmanagement/gtm_domain.py
-pulumi_akamai/trafficmanagement/gtm_geomap.py
-pulumi_akamai/trafficmanagement/gtm_property.py
-pulumi_akamai/trafficmanagement/gtm_resource.py
-pulumi_akamai/trafficmanagement/outputs.py
+pulumi_akamai/trafficmanagement/get_gtm_default_datacenter.py
```

### Comparing `pulumi_akamai-4.6.0a1688398728/setup.py` & `pulumi_akamai-5.0.0a1688662273/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "4.6.0a1688398728"
-PLUGIN_VERSION = "4.6.0-alpha.1688398728+6ae4f9e0"
+VERSION = "5.0.0a1688662273"
+PLUGIN_VERSION = "5.0.0-alpha.1688662273+cf01e9bf"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'akamai', PLUGIN_VERSION])
         except OSError as error:
```

