# Comparing `tmp/aws_emr_launch-2.0.0-py3-none-any.whl.zip` & `tmp/aws_emr_launch-2.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,175 +1,175 @@
-Zip file size: 135591 bytes, number of entries: 173
--rw-r--r--  2.0 unx      771 b- defN 22-Jun-07 17:48 aws_emr_launch/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 22-Jun-07 17:48 aws_emr_launch/constructs/__init__.py
--rw-r--r--  2.0 unx      902 b- defN 22-Jun-07 17:48 aws_emr_launch/constructs/base.py
--rw-r--r--  2.0 unx        0 b- defN 22-Jun-07 17:48 aws_emr_launch/constructs/emr_constructs/__init__.py
--rw-r--r--  2.0 unx    13342 b- defN 22-Jun-07 17:48 aws_emr_launch/constructs/emr_constructs/cluster_configuration.py
--rw-r--r--  2.0 unx     5085 b- defN 22-Jun-07 17:48 aws_emr_launch/constructs/emr_constructs/emr_code.py
--rw-r--r--  2.0 unx    26450 b- defN 22-Jun-07 17:48 aws_emr_launch/constructs/emr_constructs/emr_profile.py
--rw-r--r--  2.0 unx        0 b- defN 22-Jun-07 17:48 aws_emr_launch/constructs/iam_roles/__init__.py
--rw-r--r--  2.0 unx     6827 b- defN 22-Jun-07 17:48 aws_emr_launch/constructs/iam_roles/emr_roles.py
--rw-r--r--  2.0 unx      203 b- defN 22-Jun-07 17:48 aws_emr_launch/constructs/lambdas/__init__.py
--rw-r--r--  2.0 unx    12464 b- defN 22-Jun-07 17:48 aws_emr_launch/constructs/lambdas/emr_lambdas.py
--rw-r--r--  2.0 unx        0 b- defN 22-Jun-07 17:48 aws_emr_launch/constructs/managed_configurations/__init__.py
--rw-r--r--  2.0 unx     8951 b- defN 22-Jun-07 17:48 aws_emr_launch/constructs/managed_configurations/autoscaling_configuration.py
--rw-r--r--  2.0 unx     7274 b- defN 22-Jun-07 17:48 aws_emr_launch/constructs/managed_configurations/instance_fleet_configuration.py
--rw-r--r--  2.0 unx     6969 b- defN 22-Jun-07 17:48 aws_emr_launch/constructs/managed_configurations/instance_group_configuration.py
--rw-r--r--  2.0 unx        0 b- defN 22-Jun-07 17:48 aws_emr_launch/constructs/security_groups/__init__.py
--rw-r--r--  2.0 unx     3271 b- defN 22-Jun-07 17:48 aws_emr_launch/constructs/security_groups/emr.py
--rw-r--r--  2.0 unx        0 b- defN 22-Jun-07 17:48 aws_emr_launch/constructs/step_functions/__init__.py
--rw-r--r--  2.0 unx     6603 b- defN 22-Jun-07 17:48 aws_emr_launch/constructs/step_functions/emr_chains.py
--rw-r--r--  2.0 unx    16196 b- defN 22-Jun-07 17:48 aws_emr_launch/constructs/step_functions/emr_launch_function.py
--rw-r--r--  2.0 unx    29100 b- defN 22-Jun-07 17:48 aws_emr_launch/constructs/step_functions/emr_tasks.py
--rw-r--r--  2.0 unx      123 b- defN 22-Jun-07 17:48 aws_emr_launch/control_plane/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 22-Jun-07 17:48 aws_emr_launch/control_plane/constructs/__init__.py
--rw-r--r--  2.0 unx      608 b- defN 22-Jun-07 17:48 aws_emr_launch/control_plane/constructs/control_plane_stack.py
--rw-r--r--  2.0 unx      203 b- defN 22-Jun-07 17:48 aws_emr_launch/control_plane/constructs/lambdas/__init__.py
--rw-r--r--  2.0 unx     7028 b- defN 22-Jun-07 17:48 aws_emr_launch/control_plane/constructs/lambdas/apis.py
--rw-r--r--  2.0 unx        0 b- defN 22-Jun-07 17:48 aws_emr_launch/control_plane/lambda_sources/__init__.py
--rw-rw-r--  2.0 unx     6178 b- defN 22-Jun-07 17:48 aws_emr_launch/control_plane/lambda_sources/apis/get_list_apis.py
--rw-rw-r--  2.0 unx      926 b- defN 22-Jun-07 17:48 aws_emr_launch/lambda_sources/LICENSE
--rw-r--r--  2.0 unx        0 b- defN 22-Jun-07 17:48 aws_emr_launch/lambda_sources/__init__.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Jun-07 17:48 aws_emr_launch/lambda_sources/emr_utilities/check_cluster_status/__init__.py
--rw-rw-r--  2.0 unx     4009 b- defN 22-Jun-07 17:48 aws_emr_launch/lambda_sources/emr_utilities/check_cluster_status/lambda_source.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Jun-07 17:48 aws_emr_launch/lambda_sources/emr_utilities/fail_if_cluster_running/__init__.py
--rw-rw-r--  2.0 unx     2779 b- defN 22-Jun-07 17:48 aws_emr_launch/lambda_sources/emr_utilities/fail_if_cluster_running/lambda_source.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Jun-07 17:48 aws_emr_launch/lambda_sources/emr_utilities/load_cluster_configuration/__init__.py
--rw-rw-r--  2.0 unx     6140 b- defN 22-Jun-07 17:48 aws_emr_launch/lambda_sources/emr_utilities/load_cluster_configuration/lambda_source.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Jun-07 17:48 aws_emr_launch/lambda_sources/emr_utilities/override_cluster_configs/__init__.py
--rw-rw-r--  2.0 unx     3415 b- defN 22-Jun-07 17:48 aws_emr_launch/lambda_sources/emr_utilities/override_cluster_configs/lambda_source.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Jun-07 17:48 aws_emr_launch/lambda_sources/emr_utilities/override_step_args/__init__.py
--rw-rw-r--  2.0 unx     1008 b- defN 22-Jun-07 17:48 aws_emr_launch/lambda_sources/emr_utilities/override_step_args/lambda_source.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Jun-07 17:48 aws_emr_launch/lambda_sources/emr_utilities/parse_json_string/__init__.py
--rw-rw-r--  2.0 unx      560 b- defN 22-Jun-07 17:48 aws_emr_launch/lambda_sources/emr_utilities/parse_json_string/lambda_source.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Jun-07 17:48 aws_emr_launch/lambda_sources/emr_utilities/run_job_flow/__init__.py
--rw-rw-r--  2.0 unx     6530 b- defN 22-Jun-07 17:48 aws_emr_launch/lambda_sources/emr_utilities/run_job_flow/lambda_source.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Jun-07 17:48 aws_emr_launch/lambda_sources/emr_utilities/update_cluster_tags/__init__.py
--rw-rw-r--  2.0 unx     1565 b- defN 22-Jun-07 17:48 aws_emr_launch/lambda_sources/emr_utilities/update_cluster_tags/lambda_source.py
--rw-rw-r--  2.0 unx       29 b- defN 22-Jun-07 17:48 aws_emr_launch/lambda_sources/layers/emr_config_utils/requirements.txt
--rw-rw-r--  2.0 unx     1905 b- defN 22-Jun-07 17:48 examples/README.md
--rw-r--r--  2.0 unx        0 b- defN 22-Jun-07 17:48 examples/__init__.py
--rwxrwxr-x  2.0 unx      626 b- defN 22-Jun-07 17:48 examples/deploy_all.sh
--rw-r--r--  2.0 unx        0 b- defN 22-Jun-07 17:48 examples/cluster_configurations/__init__.py
--rw-r--r--  2.0 unx     3139 b- defN 22-Jun-07 17:48 examples/cluster_configurations/app.py
--rw-rw-r--  2.0 unx       32 b- defN 22-Jun-07 17:48 examples/cluster_configurations/cdk.json
--rwxrwxr-x  2.0 unx       59 b- defN 22-Jun-07 17:48 examples/cluster_configurations/bootstrap_source/test_bootstrap.sh
--rw-rw-r--  2.0 unx        0 b- defN 22-Jun-07 17:48 examples/cluster_configurations/jars/example_0.jar
--rw-rw-r--  2.0 unx        0 b- defN 22-Jun-07 17:48 examples/cluster_configurations/jars/example_1.jar
--rw-r--r--  2.0 unx        0 b- defN 22-Jun-07 17:48 examples/control_plane/__init__.py
--rw-r--r--  2.0 unx      182 b- defN 22-Jun-07 17:48 examples/control_plane/app.py
--rw-rw-r--  2.0 unx       32 b- defN 22-Jun-07 17:48 examples/control_plane/cdk.json
--rw-r--r--  2.0 unx        0 b- defN 22-Jun-07 17:48 examples/emr_launch_function/__init__.py
--rw-r--r--  2.0 unx     1495 b- defN 22-Jun-07 17:48 examples/emr_launch_function/app.py
--rw-rw-r--  2.0 unx       32 b- defN 22-Jun-07 17:48 examples/emr_launch_function/cdk.json
--rw-r--r--  2.0 unx        0 b- defN 22-Jun-07 17:48 examples/emr_profiles/__init__.py
--rw-r--r--  2.0 unx     2395 b- defN 22-Jun-07 17:48 examples/emr_profiles/app.py
--rw-rw-r--  2.0 unx       32 b- defN 22-Jun-07 17:48 examples/emr_profiles/cdk.json
--rw-r--r--  2.0 unx        0 b- defN 22-Jun-07 17:48 examples/environment_stack/__init__.py
--rw-r--r--  2.0 unx     2174 b- defN 22-Jun-07 17:48 examples/environment_stack/app.py
--rw-rw-r--  2.0 unx       32 b- defN 22-Jun-07 17:48 examples/environment_stack/cdk.json
--rw-r--r--  2.0 unx        0 b- defN 22-Jun-07 17:48 examples/persistent_cluster_pipeline/__init__.py
--rw-r--r--  2.0 unx     3866 b- defN 22-Jun-07 17:48 examples/persistent_cluster_pipeline/app.py
--rw-rw-r--  2.0 unx       32 b- defN 22-Jun-07 17:48 examples/persistent_cluster_pipeline/cdk.json
--rw-rw-r--  2.0 unx       80 b- defN 22-Jun-07 17:48 examples/persistent_cluster_pipeline/step_sources/phase_1/test_step_0.sh
--rw-rw-r--  2.0 unx       80 b- defN 22-Jun-07 17:48 examples/persistent_cluster_pipeline/step_sources/phase_1/test_step_1.sh
--rw-rw-r--  2.0 unx       80 b- defN 22-Jun-07 17:48 examples/persistent_cluster_pipeline/step_sources/phase_1/test_step_2.sh
--rw-rw-r--  2.0 unx       80 b- defN 22-Jun-07 17:48 examples/persistent_cluster_pipeline/step_sources/phase_1/test_step_3.sh
--rw-rw-r--  2.0 unx       80 b- defN 22-Jun-07 17:48 examples/persistent_cluster_pipeline/step_sources/phase_1/test_step_4.sh
--rw-rw-r--  2.0 unx       16 b- defN 22-Jun-07 17:48 examples/persistent_cluster_pipeline/step_sources/phase_2/test_step_0.hql
--rw-rw-r--  2.0 unx       16 b- defN 22-Jun-07 17:48 examples/persistent_cluster_pipeline/step_sources/phase_2/test_step_1.hql
--rw-rw-r--  2.0 unx       16 b- defN 22-Jun-07 17:48 examples/persistent_cluster_pipeline/step_sources/phase_2/test_step_2.hql
--rw-rw-r--  2.0 unx       16 b- defN 22-Jun-07 17:48 examples/persistent_cluster_pipeline/step_sources/phase_2/test_step_3.hql
--rw-rw-r--  2.0 unx       16 b- defN 22-Jun-07 17:48 examples/persistent_cluster_pipeline/step_sources/phase_2/test_step_4.hql
--rw-r--r--  2.0 unx        0 b- defN 22-Jun-07 17:48 examples/sns_triggered_pipeline/__init__.py
--rw-r--r--  2.0 unx     6060 b- defN 22-Jun-07 17:48 examples/sns_triggered_pipeline/app.py
--rw-rw-r--  2.0 unx       32 b- defN 22-Jun-07 17:48 examples/sns_triggered_pipeline/cdk.json
--rw-rw-r--  2.0 unx      946 b- defN 22-Jun-07 17:48 examples/sns_triggered_pipeline/lambda_sources/execute_pipeline.py
--rw-rw-r--  2.0 unx      132 b- defN 22-Jun-07 17:48 examples/sns_triggered_pipeline/step_sources/test_step_0.py
--rw-rw-r--  2.0 unx      132 b- defN 22-Jun-07 17:48 examples/sns_triggered_pipeline/step_sources/test_step_1.py
--rw-rw-r--  2.0 unx      132 b- defN 22-Jun-07 17:48 examples/sns_triggered_pipeline/step_sources/test_step_2.py
--rw-rw-r--  2.0 unx      132 b- defN 22-Jun-07 17:48 examples/sns_triggered_pipeline/step_sources/test_step_3.py
--rw-rw-r--  2.0 unx      132 b- defN 22-Jun-07 17:48 examples/sns_triggered_pipeline/step_sources/test_step_4.py
--rw-rw-r--  2.0 unx     2821 b- defN 22-Jun-07 17:48 examples/spark_batch_orchestration/README.md
--rw-r--r--  2.0 unx        0 b- defN 22-Jun-07 17:48 examples/spark_batch_orchestration/__init__.py
--rw-r--r--  2.0 unx     3564 b- defN 22-Jun-07 17:48 examples/spark_batch_orchestration/app.py
--rw-rw-r--  2.0 unx      145 b- defN 22-Jun-07 17:48 examples/spark_batch_orchestration/cdk.json
--rw-rw-r--  2.0 unx      627 b- defN 22-Jun-07 17:48 examples/spark_batch_orchestration/config.json
--rw-rw-r--  2.0 unx      207 b- defN 22-Jun-07 17:48 examples/spark_batch_orchestration/deploy.sh
--rw-r--r--  2.0 unx     1103 b- defN 22-Jun-07 17:48 examples/spark_batch_orchestration/setup.py
--rw-r--r--  2.0 unx        0 b- defN 22-Jun-07 17:48 examples/spark_batch_orchestration/infrastructure/__init__.py
--rw-rw-r--  2.0 unx     3322 b- defN 22-Jun-07 17:48 examples/spark_batch_orchestration/infrastructure/emr_launch/README.md
--rw-rw-r--  2.0 unx     9355 b- defN 22-Jun-07 17:48 examples/spark_batch_orchestration/infrastructure/emr_launch/cluster_definition.py
--rw-rw-r--  2.0 unx     6576 b- defN 22-Jun-07 17:48 examples/spark_batch_orchestration/infrastructure/emr_launch/instance_group_config.py
--rw-rw-r--  2.0 unx       45 b- defN 22-Jun-07 17:48 examples/spark_batch_orchestration/infrastructure/emr_launch/bootstrap_actions/install_boto3.sh
--rw-r--r--  2.0 unx        0 b- defN 22-Jun-07 17:48 examples/spark_batch_orchestration/infrastructure/emr_orchestration/__init__.py
--rw-r--r--  2.0 unx     6826 b- defN 22-Jun-07 17:48 examples/spark_batch_orchestration/infrastructure/emr_orchestration/stack.py
--rw-r--r--  2.0 unx        0 b- defN 22-Jun-07 17:48 examples/spark_batch_orchestration/infrastructure/emr_orchestration/steps/__init__.py
--rw-r--r--  2.0 unx     2868 b- defN 22-Jun-07 17:48 examples/spark_batch_orchestration/infrastructure/emr_orchestration/steps/data_ingestion.py
--rw-r--r--  2.0 unx     2572 b- defN 22-Jun-07 17:48 examples/spark_batch_orchestration/infrastructure/emr_orchestration/steps/data_preparation.py
--rw-r--r--  2.0 unx        0 b- defN 22-Jun-07 17:48 examples/spark_batch_orchestration/infrastructure/emr_trigger/__init__.py
--rw-r--r--  2.0 unx     2096 b- defN 22-Jun-07 17:48 examples/spark_batch_orchestration/infrastructure/emr_trigger/stack.py
--rw-r--r--  2.0 unx        0 b- defN 22-Jun-07 17:48 examples/spark_batch_orchestration/infrastructure/emr_trigger/lambda_source/__init__.py
--rw-r--r--  2.0 unx     6913 b- defN 22-Jun-07 17:48 examples/spark_batch_orchestration/infrastructure/emr_trigger/lambda_source/trigger.py
--rw-r--r--  2.0 unx        0 b- defN 22-Jun-07 17:48 examples/spark_batch_orchestration/infrastructure/job_summary/__init__.py
--rw-r--r--  2.0 unx     4063 b- defN 22-Jun-07 17:48 examples/spark_batch_orchestration/infrastructure/job_summary/stack.py
--rw-r--r--  2.0 unx        0 b- defN 22-Jun-07 17:48 examples/spark_batch_orchestration/infrastructure/job_summary/lambda_source/__init__.py
--rw-r--r--  2.0 unx     4389 b- defN 22-Jun-07 17:48 examples/spark_batch_orchestration/infrastructure/job_summary/lambda_source/extracting.py
--rw-r--r--  2.0 unx     2095 b- defN 22-Jun-07 17:48 examples/spark_batch_orchestration/infrastructure/job_summary/lambda_source/fetching.py
--rw-r--r--  2.0 unx      443 b- defN 22-Jun-07 17:48 examples/spark_batch_orchestration/infrastructure/job_summary/lambda_source/helpers.py
--rw-r--r--  2.0 unx     2267 b- defN 22-Jun-07 17:48 examples/spark_batch_orchestration/infrastructure/job_summary/lambda_source/main.py
--rw-r--r--  2.0 unx     6113 b- defN 22-Jun-07 17:48 examples/spark_batch_orchestration/infrastructure/job_summary/lambda_source/rendering.py
--rw-rw-r--  2.0 unx     2746 b- defN 22-Jun-07 17:48 examples/terraform_pipeline/README.md
--rw-rw-r--  2.0 unx      483 b- defN 22-Jun-07 17:48 examples/terraform_pipeline/bin/deploy.sh
--rw-rw-r--  2.0 unx      581 b- defN 22-Jun-07 17:48 examples/terraform_pipeline/emr_pipeline/spark_script.py
--rw-rw-r--  2.0 unx     1134 b- defN 22-Jun-07 17:48 examples/terraform_pipeline/emr_pipeline/emr_launch/README.md
--rw-rw-r--  2.0 unx     3322 b- defN 22-Jun-07 17:48 examples/terraform_pipeline/emr_pipeline/emr_launch/infrastructure/README.md
--rw-rw-r--  2.0 unx        0 b- defN 22-Jun-07 17:48 examples/terraform_pipeline/emr_pipeline/emr_launch/infrastructure/__init__.py
--rw-rw-r--  2.0 unx       32 b- defN 22-Jun-07 17:48 examples/terraform_pipeline/emr_pipeline/emr_launch/infrastructure/cdk.json
--rw-rw-r--  2.0 unx     9018 b- defN 22-Jun-07 17:48 examples/terraform_pipeline/emr_pipeline/emr_launch/infrastructure/cluster_definition.py
--rw-rw-r--  2.0 unx     6576 b- defN 22-Jun-07 17:48 examples/terraform_pipeline/emr_pipeline/emr_launch/infrastructure/instance_group_config.py
--rwxrwxr-x  2.0 unx     2017 b- defN 22-Jun-07 17:48 examples/terraform_pipeline/emr_pipeline/emr_launch/infrastructure/main.py
--rw-rw-r--  2.0 unx      424 b- defN 22-Jun-07 17:48 examples/terraform_pipeline/emr_pipeline/emr_launch/utils/cdk_deploy.sh
--rw-rw-r--  2.0 unx      283 b- defN 22-Jun-07 17:48 examples/terraform_pipeline/emr_pipeline/emr_launch/utils/cdk_destroy.sh
--rw-rw-r--  2.0 unx     5138 b- defN 22-Jun-07 17:48 examples/terraform_pipeline/emr_pipeline/emr_step_function/pipeline.json
--rw-rw-r--  2.0 unx        0 b- defN 22-Jun-07 17:48 examples/terraform_pipeline/emr_pipeline/emr_step_function/lambda/__init__.py
--rw-rw-r--  2.0 unx      506 b- defN 22-Jun-07 17:48 examples/terraform_pipeline/emr_pipeline/emr_step_function/lambda/lambda_parse_json.py
--rw-r--r--  2.0 unx        0 b- defN 22-Jun-07 17:48 examples/transient_cluster_pipeline/__init__.py
--rw-r--r--  2.0 unx     6852 b- defN 22-Jun-07 17:48 examples/transient_cluster_pipeline/app.py
--rw-rw-r--  2.0 unx       32 b- defN 22-Jun-07 17:48 examples/transient_cluster_pipeline/cdk.json
--rw-rw-r--  2.0 unx    21056 b- defN 22-Jun-07 17:48 examples/transient_cluster_pipeline/pipeline.json
--rw-rw-r--  2.0 unx       80 b- defN 22-Jun-07 17:48 examples/transient_cluster_pipeline/step_sources/phase_1/test_step_0.sh
--rw-rw-r--  2.0 unx       80 b- defN 22-Jun-07 17:48 examples/transient_cluster_pipeline/step_sources/phase_1/test_step_1.sh
--rw-rw-r--  2.0 unx       80 b- defN 22-Jun-07 17:48 examples/transient_cluster_pipeline/step_sources/phase_1/test_step_2.sh
--rw-rw-r--  2.0 unx       80 b- defN 22-Jun-07 17:48 examples/transient_cluster_pipeline/step_sources/phase_1/test_step_3.sh
--rw-rw-r--  2.0 unx       80 b- defN 22-Jun-07 17:48 examples/transient_cluster_pipeline/step_sources/phase_1/test_step_4.sh
--rw-rw-r--  2.0 unx       80 b- defN 22-Jun-07 17:48 examples/transient_cluster_pipeline/step_sources/phase_1/test_validation.sh
--rw-rw-r--  2.0 unx       16 b- defN 22-Jun-07 17:48 examples/transient_cluster_pipeline/step_sources/phase_2/test_step_0.hql
--rw-rw-r--  2.0 unx       16 b- defN 22-Jun-07 17:48 examples/transient_cluster_pipeline/step_sources/phase_2/test_step_1.hql
--rw-rw-r--  2.0 unx       16 b- defN 22-Jun-07 17:48 examples/transient_cluster_pipeline/step_sources/phase_2/test_step_2.hql
--rw-rw-r--  2.0 unx       16 b- defN 22-Jun-07 17:48 examples/transient_cluster_pipeline/step_sources/phase_2/test_step_3.hql
--rw-rw-r--  2.0 unx       16 b- defN 22-Jun-07 17:48 examples/transient_cluster_pipeline/step_sources/phase_2/test_step_4.hql
--rw-rw-r--  2.0 unx       16 b- defN 22-Jun-07 17:48 examples/transient_cluster_pipeline/step_sources/phase_2/test_validation.hql
--rw-r--r--  2.0 unx        0 b- defN 22-Jun-07 17:48 tests/aws_emr_launch/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 22-Jun-07 17:48 tests/aws_emr_launch/constructs/__init__.py
--rw-r--r--  2.0 unx      650 b- defN 22-Jun-07 17:48 tests/aws_emr_launch/constructs/test_iam_roles.py
--rw-r--r--  2.0 unx      494 b- defN 22-Jun-07 17:48 tests/aws_emr_launch/constructs/test_security_groups.py
--rw-r--r--  2.0 unx        0 b- defN 22-Jun-07 17:48 tests/aws_emr_launch/constructs/emr_constructs/__init__.py
--rw-r--r--  2.0 unx     4039 b- defN 22-Jun-07 17:48 tests/aws_emr_launch/constructs/emr_constructs/test_cluster_configuration.py
--rw-r--r--  2.0 unx     9803 b- defN 22-Jun-07 17:48 tests/aws_emr_launch/constructs/emr_constructs/test_emr_profile.py
--rw-r--r--  2.0 unx        0 b- defN 22-Jun-07 17:48 tests/aws_emr_launch/constructs/managed_configurations/__init__.py
--rw-r--r--  2.0 unx     9708 b- defN 22-Jun-07 17:48 tests/aws_emr_launch/constructs/managed_configurations/test_autoscaling_configuration.py
--rw-r--r--  2.0 unx     4799 b- defN 22-Jun-07 17:48 tests/aws_emr_launch/constructs/managed_configurations/test_instance_fleet_configuration.py
--rw-r--r--  2.0 unx     4192 b- defN 22-Jun-07 17:48 tests/aws_emr_launch/constructs/managed_configurations/test_instance_group_configuration.py
--rw-r--r--  2.0 unx      126 b- defN 22-Jun-07 17:48 tests/aws_emr_launch/control_plane/__init__.py
--rw-r--r--  2.0 unx      185 b- defN 22-Jun-07 17:48 tests/aws_emr_launch/control_plane/test_control_plane.py
--rw-r--r--  2.0 unx        0 b- defN 22-Jun-07 17:48 tests/aws_emr_launch/control_plane/constructs/__init__.py
--rw-r--r--  2.0 unx      419 b- defN 22-Jun-07 17:48 tests/aws_emr_launch/control_plane/constructs/test_lambdas.py
--rw-r--r--  2.0 unx        0 b- defN 22-Jun-07 17:48 tests/aws_emr_launch/control_plane/lambda_sources/__init__.py
--rw-rw-r--  2.0 unx    10142 b- defN 22-Jun-07 17:55 aws_emr_launch-2.0.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     9577 b- defN 22-Jun-07 17:55 aws_emr_launch-2.0.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       67 b- defN 22-Jun-07 17:55 aws_emr_launch-2.0.0.dist-info/NOTICE
--rw-rw-r--  2.0 unx        6 b- defN 22-Jun-07 17:55 aws_emr_launch-2.0.0.dist-info/VERSION
--rw-r--r--  2.0 unx       92 b- defN 22-Jun-07 17:55 aws_emr_launch-2.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       30 b- defN 22-Jun-07 17:55 aws_emr_launch-2.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    20056 b- defN 22-Jun-07 17:55 aws_emr_launch-2.0.0.dist-info/RECORD
-173 files, 413291 bytes uncompressed, 101459 bytes compressed:  75.5%
+Zip file size: 135739 bytes, number of entries: 173
+-rw-r--r--  2.0 unx      771 b- defN 23-Jul-07 17:42 aws_emr_launch/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-07 17:42 aws_emr_launch/constructs/__init__.py
+-rw-r--r--  2.0 unx      902 b- defN 23-Jul-07 17:42 aws_emr_launch/constructs/base.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-07 17:42 aws_emr_launch/constructs/emr_constructs/__init__.py
+-rw-r--r--  2.0 unx    13342 b- defN 23-Jul-07 17:42 aws_emr_launch/constructs/emr_constructs/cluster_configuration.py
+-rw-r--r--  2.0 unx     5085 b- defN 23-Jul-07 17:42 aws_emr_launch/constructs/emr_constructs/emr_code.py
+-rw-r--r--  2.0 unx    26450 b- defN 23-Jul-07 17:42 aws_emr_launch/constructs/emr_constructs/emr_profile.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-07 17:42 aws_emr_launch/constructs/iam_roles/__init__.py
+-rw-r--r--  2.0 unx     6827 b- defN 23-Jul-07 17:42 aws_emr_launch/constructs/iam_roles/emr_roles.py
+-rw-r--r--  2.0 unx      203 b- defN 23-Jul-07 17:42 aws_emr_launch/constructs/lambdas/__init__.py
+-rw-r--r--  2.0 unx    12464 b- defN 23-Jul-07 17:42 aws_emr_launch/constructs/lambdas/emr_lambdas.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-07 17:42 aws_emr_launch/constructs/managed_configurations/__init__.py
+-rw-r--r--  2.0 unx     8951 b- defN 23-Jul-07 17:42 aws_emr_launch/constructs/managed_configurations/autoscaling_configuration.py
+-rw-r--r--  2.0 unx     7274 b- defN 23-Jul-07 17:42 aws_emr_launch/constructs/managed_configurations/instance_fleet_configuration.py
+-rw-r--r--  2.0 unx     6969 b- defN 23-Jul-07 17:42 aws_emr_launch/constructs/managed_configurations/instance_group_configuration.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-07 17:42 aws_emr_launch/constructs/security_groups/__init__.py
+-rw-r--r--  2.0 unx     3271 b- defN 23-Jul-07 17:42 aws_emr_launch/constructs/security_groups/emr.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-07 17:42 aws_emr_launch/constructs/step_functions/__init__.py
+-rw-r--r--  2.0 unx     6603 b- defN 23-Jul-07 17:42 aws_emr_launch/constructs/step_functions/emr_chains.py
+-rw-r--r--  2.0 unx    16196 b- defN 23-Jul-07 17:42 aws_emr_launch/constructs/step_functions/emr_launch_function.py
+-rw-r--r--  2.0 unx    29148 b- defN 23-Jul-07 17:42 aws_emr_launch/constructs/step_functions/emr_tasks.py
+-rw-r--r--  2.0 unx      123 b- defN 23-Jul-07 17:42 aws_emr_launch/control_plane/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-07 17:42 aws_emr_launch/control_plane/constructs/__init__.py
+-rw-r--r--  2.0 unx      608 b- defN 23-Jul-07 17:42 aws_emr_launch/control_plane/constructs/control_plane_stack.py
+-rw-r--r--  2.0 unx      203 b- defN 23-Jul-07 17:42 aws_emr_launch/control_plane/constructs/lambdas/__init__.py
+-rw-r--r--  2.0 unx     7028 b- defN 23-Jul-07 17:42 aws_emr_launch/control_plane/constructs/lambdas/apis.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-07 17:42 aws_emr_launch/control_plane/lambda_sources/__init__.py
+-rw-rw-r--  2.0 unx     6178 b- defN 23-Jul-07 17:42 aws_emr_launch/control_plane/lambda_sources/apis/get_list_apis.py
+-rw-rw-r--  2.0 unx      926 b- defN 23-Jul-07 17:42 aws_emr_launch/lambda_sources/LICENSE
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-07 17:42 aws_emr_launch/lambda_sources/__init__.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-07 17:42 aws_emr_launch/lambda_sources/emr_utilities/check_cluster_status/__init__.py
+-rw-rw-r--  2.0 unx     4009 b- defN 23-Jul-07 17:42 aws_emr_launch/lambda_sources/emr_utilities/check_cluster_status/lambda_source.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-07 17:42 aws_emr_launch/lambda_sources/emr_utilities/fail_if_cluster_running/__init__.py
+-rw-rw-r--  2.0 unx     2779 b- defN 23-Jul-07 17:42 aws_emr_launch/lambda_sources/emr_utilities/fail_if_cluster_running/lambda_source.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-07 17:42 aws_emr_launch/lambda_sources/emr_utilities/load_cluster_configuration/__init__.py
+-rw-rw-r--  2.0 unx     6140 b- defN 23-Jul-07 17:42 aws_emr_launch/lambda_sources/emr_utilities/load_cluster_configuration/lambda_source.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-07 17:42 aws_emr_launch/lambda_sources/emr_utilities/override_cluster_configs/__init__.py
+-rw-rw-r--  2.0 unx     3415 b- defN 23-Jul-07 17:42 aws_emr_launch/lambda_sources/emr_utilities/override_cluster_configs/lambda_source.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-07 17:42 aws_emr_launch/lambda_sources/emr_utilities/override_step_args/__init__.py
+-rw-rw-r--  2.0 unx     1008 b- defN 23-Jul-07 17:42 aws_emr_launch/lambda_sources/emr_utilities/override_step_args/lambda_source.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-07 17:42 aws_emr_launch/lambda_sources/emr_utilities/parse_json_string/__init__.py
+-rw-rw-r--  2.0 unx      560 b- defN 23-Jul-07 17:42 aws_emr_launch/lambda_sources/emr_utilities/parse_json_string/lambda_source.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-07 17:42 aws_emr_launch/lambda_sources/emr_utilities/run_job_flow/__init__.py
+-rw-rw-r--  2.0 unx     6530 b- defN 23-Jul-07 17:42 aws_emr_launch/lambda_sources/emr_utilities/run_job_flow/lambda_source.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-07 17:42 aws_emr_launch/lambda_sources/emr_utilities/update_cluster_tags/__init__.py
+-rw-rw-r--  2.0 unx     1565 b- defN 23-Jul-07 17:42 aws_emr_launch/lambda_sources/emr_utilities/update_cluster_tags/lambda_source.py
+-rw-rw-r--  2.0 unx       29 b- defN 23-Jul-07 17:42 aws_emr_launch/lambda_sources/layers/emr_config_utils/requirements.txt
+-rw-rw-r--  2.0 unx     1905 b- defN 23-Jul-07 17:42 examples/README.md
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-07 17:42 examples/__init__.py
+-rwxrwxr-x  2.0 unx      626 b- defN 23-Jul-07 17:42 examples/deploy_all.sh
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-07 17:42 examples/cluster_configurations/__init__.py
+-rw-r--r--  2.0 unx     3139 b- defN 23-Jul-07 17:42 examples/cluster_configurations/app.py
+-rw-rw-r--  2.0 unx       32 b- defN 23-Jul-07 17:42 examples/cluster_configurations/cdk.json
+-rwxrwxr-x  2.0 unx       59 b- defN 23-Jul-07 17:42 examples/cluster_configurations/bootstrap_source/test_bootstrap.sh
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-07 17:42 examples/cluster_configurations/jars/example_0.jar
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-07 17:42 examples/cluster_configurations/jars/example_1.jar
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-07 17:42 examples/control_plane/__init__.py
+-rw-r--r--  2.0 unx      182 b- defN 23-Jul-07 17:42 examples/control_plane/app.py
+-rw-rw-r--  2.0 unx       32 b- defN 23-Jul-07 17:42 examples/control_plane/cdk.json
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-07 17:42 examples/emr_launch_function/__init__.py
+-rw-r--r--  2.0 unx     1495 b- defN 23-Jul-07 17:42 examples/emr_launch_function/app.py
+-rw-rw-r--  2.0 unx       32 b- defN 23-Jul-07 17:42 examples/emr_launch_function/cdk.json
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-07 17:42 examples/emr_profiles/__init__.py
+-rw-r--r--  2.0 unx     2395 b- defN 23-Jul-07 17:42 examples/emr_profiles/app.py
+-rw-rw-r--  2.0 unx       32 b- defN 23-Jul-07 17:42 examples/emr_profiles/cdk.json
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-07 17:42 examples/environment_stack/__init__.py
+-rw-r--r--  2.0 unx     2174 b- defN 23-Jul-07 17:42 examples/environment_stack/app.py
+-rw-rw-r--  2.0 unx       32 b- defN 23-Jul-07 17:42 examples/environment_stack/cdk.json
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-07 17:42 examples/persistent_cluster_pipeline/__init__.py
+-rw-r--r--  2.0 unx     3866 b- defN 23-Jul-07 17:42 examples/persistent_cluster_pipeline/app.py
+-rw-rw-r--  2.0 unx       32 b- defN 23-Jul-07 17:42 examples/persistent_cluster_pipeline/cdk.json
+-rw-rw-r--  2.0 unx       80 b- defN 23-Jul-07 17:42 examples/persistent_cluster_pipeline/step_sources/phase_1/test_step_0.sh
+-rw-rw-r--  2.0 unx       80 b- defN 23-Jul-07 17:42 examples/persistent_cluster_pipeline/step_sources/phase_1/test_step_1.sh
+-rw-rw-r--  2.0 unx       80 b- defN 23-Jul-07 17:42 examples/persistent_cluster_pipeline/step_sources/phase_1/test_step_2.sh
+-rw-rw-r--  2.0 unx       80 b- defN 23-Jul-07 17:42 examples/persistent_cluster_pipeline/step_sources/phase_1/test_step_3.sh
+-rw-rw-r--  2.0 unx       80 b- defN 23-Jul-07 17:42 examples/persistent_cluster_pipeline/step_sources/phase_1/test_step_4.sh
+-rw-rw-r--  2.0 unx       16 b- defN 23-Jul-07 17:42 examples/persistent_cluster_pipeline/step_sources/phase_2/test_step_0.hql
+-rw-rw-r--  2.0 unx       16 b- defN 23-Jul-07 17:42 examples/persistent_cluster_pipeline/step_sources/phase_2/test_step_1.hql
+-rw-rw-r--  2.0 unx       16 b- defN 23-Jul-07 17:42 examples/persistent_cluster_pipeline/step_sources/phase_2/test_step_2.hql
+-rw-rw-r--  2.0 unx       16 b- defN 23-Jul-07 17:42 examples/persistent_cluster_pipeline/step_sources/phase_2/test_step_3.hql
+-rw-rw-r--  2.0 unx       16 b- defN 23-Jul-07 17:42 examples/persistent_cluster_pipeline/step_sources/phase_2/test_step_4.hql
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-07 17:42 examples/sns_triggered_pipeline/__init__.py
+-rw-r--r--  2.0 unx     6060 b- defN 23-Jul-07 17:42 examples/sns_triggered_pipeline/app.py
+-rw-rw-r--  2.0 unx       32 b- defN 23-Jul-07 17:42 examples/sns_triggered_pipeline/cdk.json
+-rw-rw-r--  2.0 unx      946 b- defN 23-Jul-07 17:42 examples/sns_triggered_pipeline/lambda_sources/execute_pipeline.py
+-rw-rw-r--  2.0 unx      132 b- defN 23-Jul-07 17:42 examples/sns_triggered_pipeline/step_sources/test_step_0.py
+-rw-rw-r--  2.0 unx      132 b- defN 23-Jul-07 17:42 examples/sns_triggered_pipeline/step_sources/test_step_1.py
+-rw-rw-r--  2.0 unx      132 b- defN 23-Jul-07 17:42 examples/sns_triggered_pipeline/step_sources/test_step_2.py
+-rw-rw-r--  2.0 unx      132 b- defN 23-Jul-07 17:42 examples/sns_triggered_pipeline/step_sources/test_step_3.py
+-rw-rw-r--  2.0 unx      132 b- defN 23-Jul-07 17:42 examples/sns_triggered_pipeline/step_sources/test_step_4.py
+-rw-rw-r--  2.0 unx     2821 b- defN 23-Jul-07 17:42 examples/spark_batch_orchestration/README.md
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-07 17:42 examples/spark_batch_orchestration/__init__.py
+-rw-r--r--  2.0 unx     3564 b- defN 23-Jul-07 17:42 examples/spark_batch_orchestration/app.py
+-rw-rw-r--  2.0 unx      145 b- defN 23-Jul-07 17:42 examples/spark_batch_orchestration/cdk.json
+-rw-rw-r--  2.0 unx      627 b- defN 23-Jul-07 17:42 examples/spark_batch_orchestration/config.json
+-rw-rw-r--  2.0 unx      207 b- defN 23-Jul-07 17:42 examples/spark_batch_orchestration/deploy.sh
+-rw-r--r--  2.0 unx     1103 b- defN 23-Jul-07 17:42 examples/spark_batch_orchestration/setup.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-07 17:42 examples/spark_batch_orchestration/infrastructure/__init__.py
+-rw-rw-r--  2.0 unx     3322 b- defN 23-Jul-07 17:42 examples/spark_batch_orchestration/infrastructure/emr_launch/README.md
+-rw-rw-r--  2.0 unx     9355 b- defN 23-Jul-07 17:42 examples/spark_batch_orchestration/infrastructure/emr_launch/cluster_definition.py
+-rw-rw-r--  2.0 unx     6576 b- defN 23-Jul-07 17:42 examples/spark_batch_orchestration/infrastructure/emr_launch/instance_group_config.py
+-rw-rw-r--  2.0 unx       45 b- defN 23-Jul-07 17:42 examples/spark_batch_orchestration/infrastructure/emr_launch/bootstrap_actions/install_boto3.sh
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-07 17:42 examples/spark_batch_orchestration/infrastructure/emr_orchestration/__init__.py
+-rw-r--r--  2.0 unx     6826 b- defN 23-Jul-07 17:42 examples/spark_batch_orchestration/infrastructure/emr_orchestration/stack.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-07 17:42 examples/spark_batch_orchestration/infrastructure/emr_orchestration/steps/__init__.py
+-rw-r--r--  2.0 unx     2868 b- defN 23-Jul-07 17:42 examples/spark_batch_orchestration/infrastructure/emr_orchestration/steps/data_ingestion.py
+-rw-r--r--  2.0 unx     2572 b- defN 23-Jul-07 17:42 examples/spark_batch_orchestration/infrastructure/emr_orchestration/steps/data_preparation.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-07 17:42 examples/spark_batch_orchestration/infrastructure/emr_trigger/__init__.py
+-rw-r--r--  2.0 unx     2096 b- defN 23-Jul-07 17:42 examples/spark_batch_orchestration/infrastructure/emr_trigger/stack.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-07 17:42 examples/spark_batch_orchestration/infrastructure/emr_trigger/lambda_source/__init__.py
+-rw-r--r--  2.0 unx     6913 b- defN 23-Jul-07 17:42 examples/spark_batch_orchestration/infrastructure/emr_trigger/lambda_source/trigger.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-07 17:42 examples/spark_batch_orchestration/infrastructure/job_summary/__init__.py
+-rw-r--r--  2.0 unx     4063 b- defN 23-Jul-07 17:42 examples/spark_batch_orchestration/infrastructure/job_summary/stack.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-07 17:42 examples/spark_batch_orchestration/infrastructure/job_summary/lambda_source/__init__.py
+-rw-r--r--  2.0 unx     4389 b- defN 23-Jul-07 17:42 examples/spark_batch_orchestration/infrastructure/job_summary/lambda_source/extracting.py
+-rw-r--r--  2.0 unx     2095 b- defN 23-Jul-07 17:42 examples/spark_batch_orchestration/infrastructure/job_summary/lambda_source/fetching.py
+-rw-r--r--  2.0 unx      443 b- defN 23-Jul-07 17:42 examples/spark_batch_orchestration/infrastructure/job_summary/lambda_source/helpers.py
+-rw-r--r--  2.0 unx     2267 b- defN 23-Jul-07 17:42 examples/spark_batch_orchestration/infrastructure/job_summary/lambda_source/main.py
+-rw-r--r--  2.0 unx     6113 b- defN 23-Jul-07 17:42 examples/spark_batch_orchestration/infrastructure/job_summary/lambda_source/rendering.py
+-rw-rw-r--  2.0 unx     2746 b- defN 23-Jul-07 17:42 examples/terraform_pipeline/README.md
+-rw-rw-r--  2.0 unx      483 b- defN 23-Jul-07 17:42 examples/terraform_pipeline/bin/deploy.sh
+-rw-rw-r--  2.0 unx      581 b- defN 23-Jul-07 17:42 examples/terraform_pipeline/emr_pipeline/spark_script.py
+-rw-rw-r--  2.0 unx     1134 b- defN 23-Jul-07 17:42 examples/terraform_pipeline/emr_pipeline/emr_launch/README.md
+-rw-rw-r--  2.0 unx     3322 b- defN 23-Jul-07 17:42 examples/terraform_pipeline/emr_pipeline/emr_launch/infrastructure/README.md
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-07 17:42 examples/terraform_pipeline/emr_pipeline/emr_launch/infrastructure/__init__.py
+-rw-rw-r--  2.0 unx       32 b- defN 23-Jul-07 17:42 examples/terraform_pipeline/emr_pipeline/emr_launch/infrastructure/cdk.json
+-rw-rw-r--  2.0 unx     9018 b- defN 23-Jul-07 17:42 examples/terraform_pipeline/emr_pipeline/emr_launch/infrastructure/cluster_definition.py
+-rw-rw-r--  2.0 unx     6576 b- defN 23-Jul-07 17:42 examples/terraform_pipeline/emr_pipeline/emr_launch/infrastructure/instance_group_config.py
+-rwxrwxr-x  2.0 unx     2017 b- defN 23-Jul-07 17:42 examples/terraform_pipeline/emr_pipeline/emr_launch/infrastructure/main.py
+-rw-rw-r--  2.0 unx      424 b- defN 23-Jul-07 17:42 examples/terraform_pipeline/emr_pipeline/emr_launch/utils/cdk_deploy.sh
+-rw-rw-r--  2.0 unx      283 b- defN 23-Jul-07 17:42 examples/terraform_pipeline/emr_pipeline/emr_launch/utils/cdk_destroy.sh
+-rw-rw-r--  2.0 unx     5138 b- defN 23-Jul-07 17:42 examples/terraform_pipeline/emr_pipeline/emr_step_function/pipeline.json
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-07 17:42 examples/terraform_pipeline/emr_pipeline/emr_step_function/lambda/__init__.py
+-rw-rw-r--  2.0 unx      506 b- defN 23-Jul-07 17:42 examples/terraform_pipeline/emr_pipeline/emr_step_function/lambda/lambda_parse_json.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-07 17:42 examples/transient_cluster_pipeline/__init__.py
+-rw-r--r--  2.0 unx     6852 b- defN 23-Jul-07 17:42 examples/transient_cluster_pipeline/app.py
+-rw-rw-r--  2.0 unx       32 b- defN 23-Jul-07 17:42 examples/transient_cluster_pipeline/cdk.json
+-rw-rw-r--  2.0 unx    21056 b- defN 23-Jul-07 17:42 examples/transient_cluster_pipeline/pipeline.json
+-rw-rw-r--  2.0 unx       80 b- defN 23-Jul-07 17:42 examples/transient_cluster_pipeline/step_sources/phase_1/test_step_0.sh
+-rw-rw-r--  2.0 unx       80 b- defN 23-Jul-07 17:42 examples/transient_cluster_pipeline/step_sources/phase_1/test_step_1.sh
+-rw-rw-r--  2.0 unx       80 b- defN 23-Jul-07 17:42 examples/transient_cluster_pipeline/step_sources/phase_1/test_step_2.sh
+-rw-rw-r--  2.0 unx       80 b- defN 23-Jul-07 17:42 examples/transient_cluster_pipeline/step_sources/phase_1/test_step_3.sh
+-rw-rw-r--  2.0 unx       80 b- defN 23-Jul-07 17:42 examples/transient_cluster_pipeline/step_sources/phase_1/test_step_4.sh
+-rw-rw-r--  2.0 unx       80 b- defN 23-Jul-07 17:42 examples/transient_cluster_pipeline/step_sources/phase_1/test_validation.sh
+-rw-rw-r--  2.0 unx       16 b- defN 23-Jul-07 17:42 examples/transient_cluster_pipeline/step_sources/phase_2/test_step_0.hql
+-rw-rw-r--  2.0 unx       16 b- defN 23-Jul-07 17:42 examples/transient_cluster_pipeline/step_sources/phase_2/test_step_1.hql
+-rw-rw-r--  2.0 unx       16 b- defN 23-Jul-07 17:42 examples/transient_cluster_pipeline/step_sources/phase_2/test_step_2.hql
+-rw-rw-r--  2.0 unx       16 b- defN 23-Jul-07 17:42 examples/transient_cluster_pipeline/step_sources/phase_2/test_step_3.hql
+-rw-rw-r--  2.0 unx       16 b- defN 23-Jul-07 17:42 examples/transient_cluster_pipeline/step_sources/phase_2/test_step_4.hql
+-rw-rw-r--  2.0 unx       16 b- defN 23-Jul-07 17:42 examples/transient_cluster_pipeline/step_sources/phase_2/test_validation.hql
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-07 17:42 tests/aws_emr_launch/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-07 17:42 tests/aws_emr_launch/constructs/__init__.py
+-rw-r--r--  2.0 unx      650 b- defN 23-Jul-07 17:42 tests/aws_emr_launch/constructs/test_iam_roles.py
+-rw-r--r--  2.0 unx      494 b- defN 23-Jul-07 17:42 tests/aws_emr_launch/constructs/test_security_groups.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-07 17:42 tests/aws_emr_launch/constructs/emr_constructs/__init__.py
+-rw-r--r--  2.0 unx     4039 b- defN 23-Jul-07 17:42 tests/aws_emr_launch/constructs/emr_constructs/test_cluster_configuration.py
+-rw-r--r--  2.0 unx     9803 b- defN 23-Jul-07 17:42 tests/aws_emr_launch/constructs/emr_constructs/test_emr_profile.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-07 17:42 tests/aws_emr_launch/constructs/managed_configurations/__init__.py
+-rw-r--r--  2.0 unx     9708 b- defN 23-Jul-07 17:42 tests/aws_emr_launch/constructs/managed_configurations/test_autoscaling_configuration.py
+-rw-r--r--  2.0 unx     4799 b- defN 23-Jul-07 17:42 tests/aws_emr_launch/constructs/managed_configurations/test_instance_fleet_configuration.py
+-rw-r--r--  2.0 unx     4192 b- defN 23-Jul-07 17:42 tests/aws_emr_launch/constructs/managed_configurations/test_instance_group_configuration.py
+-rw-r--r--  2.0 unx      126 b- defN 23-Jul-07 17:42 tests/aws_emr_launch/control_plane/__init__.py
+-rw-r--r--  2.0 unx      185 b- defN 23-Jul-07 17:42 tests/aws_emr_launch/control_plane/test_control_plane.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-07 17:42 tests/aws_emr_launch/control_plane/constructs/__init__.py
+-rw-r--r--  2.0 unx      419 b- defN 23-Jul-07 17:42 tests/aws_emr_launch/control_plane/constructs/test_lambdas.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-07 17:42 tests/aws_emr_launch/control_plane/lambda_sources/__init__.py
+-rw-rw-r--  2.0 unx    10142 b- defN 23-Jul-07 17:51 aws_emr_launch-2.0.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     9924 b- defN 23-Jul-07 17:51 aws_emr_launch-2.0.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       67 b- defN 23-Jul-07 17:51 aws_emr_launch-2.0.1.dist-info/NOTICE
+-rw-rw-r--  2.0 unx        6 b- defN 23-Jul-07 17:51 aws_emr_launch-2.0.1.dist-info/VERSION
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-07 17:51 aws_emr_launch-2.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       30 b- defN 23-Jul-07 17:51 aws_emr_launch-2.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    20056 b- defN 23-Jul-07 17:51 aws_emr_launch-2.0.1.dist-info/RECORD
+173 files, 413686 bytes uncompressed, 101607 bytes compressed:  75.4%
```

## zipnote {}

```diff
@@ -492,29 +492,29 @@
 
 Filename: tests/aws_emr_launch/control_plane/constructs/test_lambdas.py
 Comment: 
 
 Filename: tests/aws_emr_launch/control_plane/lambda_sources/__init__.py
 Comment: 
 
-Filename: aws_emr_launch-2.0.0.dist-info/LICENSE
+Filename: aws_emr_launch-2.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: aws_emr_launch-2.0.0.dist-info/METADATA
+Filename: aws_emr_launch-2.0.1.dist-info/METADATA
 Comment: 
 
-Filename: aws_emr_launch-2.0.0.dist-info/NOTICE
+Filename: aws_emr_launch-2.0.1.dist-info/NOTICE
 Comment: 
 
-Filename: aws_emr_launch-2.0.0.dist-info/VERSION
+Filename: aws_emr_launch-2.0.1.dist-info/VERSION
 Comment: 
 
-Filename: aws_emr_launch-2.0.0.dist-info/WHEEL
+Filename: aws_emr_launch-2.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: aws_emr_launch-2.0.0.dist-info/top_level.txt
+Filename: aws_emr_launch-2.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: aws_emr_launch-2.0.0.dist-info/RECORD
+Filename: aws_emr_launch-2.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aws_emr_launch/constructs/step_functions/emr_tasks.py

```diff
@@ -226,14 +226,15 @@
         stack = aws_cdk.Stack.of(self)
 
         policy_statements = list()
 
         policy_statements.append(
             iam.PolicyStatement(
                 actions=[
+                    "elasticmapreduce:AddTags",
                     "elasticmapreduce:RunJobFlow",
                     "elasticmapreduce:DescribeCluster",
                     "elasticmapreduce:TerminateJobFlows",
                 ],
                 resources=["*"],
             )
         )
```

## Comparing `aws_emr_launch-2.0.0.dist-info/LICENSE` & `aws_emr_launch-2.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aws_emr_launch-2.0.0.dist-info/METADATA` & `aws_emr_launch-2.0.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-emr-launch
-Version: 2.0.0
+Version: 2.0.1
 Summary: AWS EMR Launch modules
 Home-page: https://github.com/awslabs/aws-emr-launch/
 Author: Chauncy McCaughey
 Author-email: chamcca@amazon.com
 License: UNKNOWN
 Keywords: aws,cdk
 Platform: UNKNOWN
@@ -17,14 +17,17 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: NOTICE
+License-File: VERSION
 Requires-Dist: logzero (~=1.5.0)
 
 # EMR Launch
 
 > An [AWS Professional Service](https://aws.amazon.com/professional-services/) open source initiative | aws-proserve-opensource@amazon.com
 
 ![Python Version](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9-brightgreen.svg)
@@ -38,15 +41,15 @@
 
 - defining reusable Security, Resource, and Launch Configurations enabling developers to __Define Once and Reuse__
 - separating the definition of Cluster Security Configurations and Cluster Resource Configurations into reusable and shareable Constructs
 - providing a suite of Tools to simplify the construction of Orchestration Pipelines using Step Functions and EMR Clusters
 
 ## Concepts (and Constructs)
 
-This library utilizes the AWS CDK for deployement and management of resources. It is recommended that users familiarize themselves with the CDK's basic concepts and usage.
+This library utilizes the AWS CDK for deployment and management of resources. It is recommended that users familiarize themselves with the CDK's basic concepts and usage.
 
 ### EMR Profile
 
 An EMR Profile (`emr_profile`) is a reusable definition of the security profile used by an EMR Cluster. This includes:
 
 - __Service Role__: an IAM Role used by the EMR Service to manage the Cluster
 - __Instance Role__: an IAM Role used by the EC2 Instances in an EMR Cluster
@@ -106,14 +109,20 @@
 To avoid circular references with CDK dependencies this package will not install CDK and Boto3. These should be
 installed manually from one of the `requirements.txt` files (depending on the version of `aws-emr-launch`).
 
 It is recommended that a Python3 `venv` be used for all CDK builds and deployments.
 
 To get up and running quickly:
 
+### Prerequisites
+
+The AWS CDK v2.x utilizes containers to automate some tasks. EMR Launch uses and deploys a CDK `PythonLayerVersion`, this Construct uses a container to create the bundle for the Lambda Layer. As such, a `docker` runtime is required to deploy.
+
+### Deployment
+
 1. Install the [CDK CLI](https://docs.aws.amazon.com/cdk/latest/guide/getting_started.html)
 
    ```bash
    npm install -g aws-cdk
    ```
 
 2. Use your mechanism of choice to create and activate a Python3 `venv`:
@@ -122,15 +131,15 @@
    python3 -m venv .env
    source .env/bin/activate
    ```
 
 3. Install the CDK and Boto3 minimum requirements:
 
    ```bash
-   pip install -r requirements.txt
+   pip install -r requirements-2.x.txt
    ```
 
 4. Install `aws-emr-launch` package:
 
    ```bash
    pip install aws-emr-launch
    ```
```

## Comparing `aws_emr_launch-2.0.0.dist-info/RECORD` & `aws_emr_launch-2.0.1.dist-info/RECORD`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 aws_emr_launch/constructs/managed_configurations/instance_fleet_configuration.py,sha256=uSOz3LcalS5su1IJUJIaI3VbOPtCKpRIF276LRfmEHs,7274
 aws_emr_launch/constructs/managed_configurations/instance_group_configuration.py,sha256=HcAP2HlpA5VP4KwCpRdsdd2kfApgEzwDzHj1rBBe2Tw,6969
 aws_emr_launch/constructs/security_groups/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 aws_emr_launch/constructs/security_groups/emr.py,sha256=5JrqXZM5wq21BDI8L3E9dEAEGaAy_zwHCOVhqX9Du84,3271
 aws_emr_launch/constructs/step_functions/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 aws_emr_launch/constructs/step_functions/emr_chains.py,sha256=2YGI7YASElKB0_B9HuddzqE1ZaS1G62BHlHH2bR_4Ds,6603
 aws_emr_launch/constructs/step_functions/emr_launch_function.py,sha256=6gZXPZE4A3hKMfpWhUTQEx2cBLOo6IKktsED4rbC8eI,16196
-aws_emr_launch/constructs/step_functions/emr_tasks.py,sha256=PahISeKXeaBnInN2wTS1RVws8Ku7larCMMc8C7dwSPM,29100
+aws_emr_launch/constructs/step_functions/emr_tasks.py,sha256=KvDpMhPetzpzSx_TRUFbFDr-ErQqcO2M4tSxOUOE4rk,29148
 aws_emr_launch/control_plane/__init__.py,sha256=onCG5Rp0L6ejCw8sAXoz-8RaMOmW3TgPBWHNQ_z9pA4,123
 aws_emr_launch/control_plane/constructs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 aws_emr_launch/control_plane/constructs/control_plane_stack.py,sha256=jSDuC5jFc1VNYZO7AJRyhmFkOPM53T_0CerXOcqVWJg,608
 aws_emr_launch/control_plane/constructs/lambdas/__init__.py,sha256=iQvwugoeQKdbWw7fgIHc83ew3m7urRqDCptS4-XV3X8,203
 aws_emr_launch/control_plane/constructs/lambdas/apis.py,sha256=7VqzWOsUhca6-oDnzK1Oob1RKUXzVkcVG3TOXPKo2wc,7028
 aws_emr_launch/control_plane/lambda_sources/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 aws_emr_launch/control_plane/lambda_sources/apis/get_list_apis.py,sha256=2w9NbhK8bdsCRj2qwAqFA2czrulQMGCKqEXUYCBb7Gs,6178
@@ -160,14 +160,14 @@
 tests/aws_emr_launch/constructs/managed_configurations/test_instance_fleet_configuration.py,sha256=6GbKETIhxefUR84Pyw6pf20hN6ZVX4Xj261JwiWI1Jk,4799
 tests/aws_emr_launch/constructs/managed_configurations/test_instance_group_configuration.py,sha256=xSCETF1gaofScU0rmF1-eIEta2KeXa5FifWRmxxEVZQ,4192
 tests/aws_emr_launch/control_plane/__init__.py,sha256=W0tkDPyB2amscJHwx5idmUBaJrJ0WlbmNzJSSeLE0sI,126
 tests/aws_emr_launch/control_plane/test_control_plane.py,sha256=ate-rqGJFGfOLvOV5bxn8iWQ4YfcbxtYYrtQOnSUWO0,185
 tests/aws_emr_launch/control_plane/constructs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/aws_emr_launch/control_plane/constructs/test_lambdas.py,sha256=XNLEODETQ33enbzq80zoJi2ILbLjn32fzY9hhay59cQ,419
 tests/aws_emr_launch/control_plane/lambda_sources/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-aws_emr_launch-2.0.0.dist-info/LICENSE,sha256=CeipvOyAZxBGUsFoaFqwkx54aPnIKEtm9a5u2uXxEws,10142
-aws_emr_launch-2.0.0.dist-info/METADATA,sha256=72UT46QjG8xEz_KbEZGgICiWG7c-d-Psfl2vu6dYv_g,9577
-aws_emr_launch-2.0.0.dist-info/NOTICE,sha256=1CkO1kwu3Q_OHYTj-d-yiBJA_lNN73a4zSntavaD4oc,67
-aws_emr_launch-2.0.0.dist-info/VERSION,sha256=wo_MpTY3vIjhJK8XJd8Ty5jGne3v1i-zzb4c22t2BiQ,6
-aws_emr_launch-2.0.0.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-aws_emr_launch-2.0.0.dist-info/top_level.txt,sha256=kTuTOICYaehSowBG7X9YBPiXLjTrr1A7cx0FfDy60cg,30
-aws_emr_launch-2.0.0.dist-info/RECORD,,
+aws_emr_launch-2.0.1.dist-info/LICENSE,sha256=CeipvOyAZxBGUsFoaFqwkx54aPnIKEtm9a5u2uXxEws,10142
+aws_emr_launch-2.0.1.dist-info/METADATA,sha256=5c2HDegcfnZMtn2uu5gnnjyYYdQPpixspGej3GW3JMQ,9924
+aws_emr_launch-2.0.1.dist-info/NOTICE,sha256=1CkO1kwu3Q_OHYTj-d-yiBJA_lNN73a4zSntavaD4oc,67
+aws_emr_launch-2.0.1.dist-info/VERSION,sha256=_oQPUvtVeNP3frSXEV6wLGA2YBw6U-YN95lccna6p3o,6
+aws_emr_launch-2.0.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+aws_emr_launch-2.0.1.dist-info/top_level.txt,sha256=kTuTOICYaehSowBG7X9YBPiXLjTrr1A7cx0FfDy60cg,30
+aws_emr_launch-2.0.1.dist-info/RECORD,,
```

