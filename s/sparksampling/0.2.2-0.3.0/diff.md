# Comparing `tmp/sparksampling-0.2.2.tar.gz` & `tmp/sparksampling-0.3.0.tar.gz`

## Comparing `sparksampling-0.2.2.tar` & `sparksampling-0.3.0.tar`

### file list

```diff
@@ -1,100 +1,100 @@
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 sparksampling-0.2.2/.editorconfig
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 sparksampling-0.2.2/.gitattributes
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 sparksampling-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 sparksampling-0.2.2/.travis.yml
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 sparksampling-0.2.2/MANIFEST.in
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 sparksampling-0.2.2/RELEASE.md
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 sparksampling-0.2.2/pip.conf
--rw-r--r--   0        0        0    11324 2020-02-02 00:00:00.000000 sparksampling-0.2.2/client/LICENSE
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 sparksampling-0.2.2/client/README.md
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 sparksampling-0.2.2/client/RELEASE.md
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 sparksampling-0.2.2/client/pyproject.toml
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 sparksampling-0.2.2/client/dockerbuild/config.json
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 sparksampling-0.2.2/client/dockerbuild/ssc.Dockerfile
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sparksampling-0.2.2/client/sparksampling_client/__init__.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 sparksampling-0.2.2/client/sparksampling_client/cli.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 sparksampling-0.2.2/client/sparksampling_client/config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparksampling-0.2.2/client/sparksampling_client/logging.py
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 sparksampling-0.2.2/client/sparksampling_client/session.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparksampling-0.2.2/client/sparksampling_client/proto/__init__.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 sparksampling-0.2.2/client/sparksampling_client/proto/sampling_service_pb2.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 sparksampling-0.2.2/client/sparksampling_client/proto/sampling_service_pb2_grpc.py
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 sparksampling-0.2.2/client/tests/test_apply.py
--rw-r--r--   0        0        0  2988942 2020-02-02 00:00:00.000000 sparksampling-0.2.2/data/10w_x_10.csv
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 sparksampling-0.2.2/data/empty.csv
--rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 sparksampling-0.2.2/data/iris.csv
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 sparksampling-0.2.2/data/relation-a.csv
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 sparksampling-0.2.2/data/relation-b.csv
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 sparksampling-0.2.2/data/relation-c.csv
--rw-r--r--   0        0        0   943860 2020-02-02 00:00:00.000000 sparksampling-0.2.2/data/ten_million_top1k.csv
--rw-r--r--   0        0        0    15359 2020-02-02 00:00:00.000000 sparksampling-0.2.2/data/unbalance_500v50_10.csv
--rw-r--r--   0        0        0  1518641 2020-02-02 00:00:00.000000 sparksampling-0.2.2/data/unbalance_5w1k_10.csv
--rw-r--r--   0        0        0  1634682 2020-02-02 00:00:00.000000 sparksampling-0.2.2/data/unbalance_5w5k_10.csv
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 sparksampling-0.2.2/dockerbuild/pysparksampling-dev.Dockerfile
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 sparksampling-0.2.2/dockerbuild/pysparksampling.Dockerfile
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 sparksampling-0.2.2/example/extension-example/DEVELOP.md
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 sparksampling-0.2.2/example/extension-example/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparksampling-0.2.2/example/extension-example/sparksampling/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparksampling-0.2.2/example/extension-example/sparksampling/evaluation_extension/__init__.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 sparksampling-0.2.2/example/extension-example/sparksampling/evaluation_extension/example_extension/__init__.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 sparksampling-0.2.2/example/extension-example/sparksampling/evaluation_extension/example_extension/example_extension.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 sparksampling-0.2.2/k8s/spark-sampling-deployment.yaml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 sparksampling-0.2.2/k8s/spark-sampling-headless-service.yaml
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 sparksampling-0.2.2/k8s/spark-sampling-service.yaml
--rwxr-xr-x   0        0        0      151 2020-02-02 00:00:00.000000 sparksampling-0.2.2/k8s/start.sh
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling/__init__.py
--rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling/app.py
--rw-r--r--   0        0        0     6601 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling/config.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling/default_app_config.py
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling/engine_factory.py
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling/error.py
--rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling/mixin.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling/sdk.py
--rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling/service.py
--rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling/utilities.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling/engine/__init__.py
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling/engine/base_engine.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling/engine/dummy_engine.py
--rw-r--r--   0        0        0    11737 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling/engine/rms_engine.py
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling/engine/sms_engine.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling/engine/stop_engine.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling/evaluation/__init__.py
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling/evaluation/base_hook.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling/evaluation/dummy_hook.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling/evaluation/hook_msg.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling/evaluation/warn_hook.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling/evaluation_extension/__init__.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling/evaluation_extension/dummy_extension/__init__.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling/evaluation_extension/dummy_extension/dummy_hook.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling/file_format/__init__.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling/file_format/base_file_format.py
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling/file_format/csv_file_imp.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling/file_format/file_factory.py
--rw-r--r--   0        0        0     5779 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling/file_format/output_adapter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling/proto/__init__.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling/proto/sampling_service_pb2.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling/proto/sampling_service_pb2_grpc.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling/sample/__init__.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling/sample/base_sampling.py
--rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling/sample/cluster_sampling_imp.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling/sample/random_sampling_imp.py
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling/sample/sampling_factory.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling/sample/simple_sampling_imp.py
--rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling/sample/stratified_sampling_imp.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling_proto/README.md
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling_proto/pyproject.toml
--rw-r--r--   0        0        0     7201 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling_proto/pb/sampling_service.proto
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling_proto/sparksampling_proto/__init__.py
--rw-r--r--   0        0        0     7469 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling_proto/sparksampling_proto/sampling_service_pb2.py
--rw-r--r--   0        0        0     5796 2020-02-02 00:00:00.000000 sparksampling-0.2.2/sparksampling_proto/sparksampling_proto/sampling_service_pb2_grpc.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 sparksampling-0.2.2/tests/conftest.py
--rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 sparksampling-0.2.2/tests/test_feature.py
--rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 sparksampling-0.2.2/tests/test_rms_engine.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 sparksampling-0.2.2/tests/test_s3.py
--rw-r--r--   0        0        0    13415 2020-02-02 00:00:00.000000 sparksampling-0.2.2/tests/test_sms_sampling.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 sparksampling-0.2.2/tests/utilities.py
--rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 sparksampling-0.2.2/.gitignore
--rw-r--r--   0        0        0    11324 2020-02-02 00:00:00.000000 sparksampling-0.2.2/LICENSE
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 sparksampling-0.2.2/README.md
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 sparksampling-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 sparksampling-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 sparksampling-0.3.0/.editorconfig
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 sparksampling-0.3.0/.gitattributes
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 sparksampling-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 sparksampling-0.3.0/.travis.yml
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 sparksampling-0.3.0/MANIFEST.in
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 sparksampling-0.3.0/RELEASE.md
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 sparksampling-0.3.0/pip.conf
+-rw-r--r--   0        0        0    11324 2020-02-02 00:00:00.000000 sparksampling-0.3.0/client/LICENSE
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 sparksampling-0.3.0/client/README.md
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 sparksampling-0.3.0/client/RELEASE.md
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 sparksampling-0.3.0/client/pyproject.toml
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 sparksampling-0.3.0/client/dockerbuild/config.json
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 sparksampling-0.3.0/client/dockerbuild/ssc.Dockerfile
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sparksampling-0.3.0/client/sparksampling_client/__init__.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 sparksampling-0.3.0/client/sparksampling_client/cli.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 sparksampling-0.3.0/client/sparksampling_client/config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparksampling-0.3.0/client/sparksampling_client/logging.py
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 sparksampling-0.3.0/client/sparksampling_client/session.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparksampling-0.3.0/client/sparksampling_client/proto/__init__.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 sparksampling-0.3.0/client/sparksampling_client/proto/sampling_service_pb2.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 sparksampling-0.3.0/client/sparksampling_client/proto/sampling_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 sparksampling-0.3.0/client/tests/test_apply.py
+-rw-r--r--   0        0        0  2988942 2020-02-02 00:00:00.000000 sparksampling-0.3.0/data/10w_x_10.csv
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 sparksampling-0.3.0/data/empty.csv
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 sparksampling-0.3.0/data/iris.csv
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 sparksampling-0.3.0/data/relation-a.csv
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 sparksampling-0.3.0/data/relation-b.csv
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 sparksampling-0.3.0/data/relation-c.csv
+-rw-r--r--   0        0        0   943860 2020-02-02 00:00:00.000000 sparksampling-0.3.0/data/ten_million_top1k.csv
+-rw-r--r--   0        0        0    15359 2020-02-02 00:00:00.000000 sparksampling-0.3.0/data/unbalance_500v50_10.csv
+-rw-r--r--   0        0        0  1518641 2020-02-02 00:00:00.000000 sparksampling-0.3.0/data/unbalance_5w1k_10.csv
+-rw-r--r--   0        0        0  1634682 2020-02-02 00:00:00.000000 sparksampling-0.3.0/data/unbalance_5w5k_10.csv
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 sparksampling-0.3.0/dockerbuild/pysparksampling-dev.Dockerfile
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 sparksampling-0.3.0/dockerbuild/pysparksampling.Dockerfile
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 sparksampling-0.3.0/example/extension-example/DEVELOP.md
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 sparksampling-0.3.0/example/extension-example/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparksampling-0.3.0/example/extension-example/sparksampling/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparksampling-0.3.0/example/extension-example/sparksampling/evaluation_extension/__init__.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 sparksampling-0.3.0/example/extension-example/sparksampling/evaluation_extension/example_extension/__init__.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 sparksampling-0.3.0/example/extension-example/sparksampling/evaluation_extension/example_extension/example_extension.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 sparksampling-0.3.0/k8s/spark-sampling-deployment.yaml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 sparksampling-0.3.0/k8s/spark-sampling-headless-service.yaml
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 sparksampling-0.3.0/k8s/spark-sampling-service.yaml
+-rwxr-xr-x   0        0        0      151 2020-02-02 00:00:00.000000 sparksampling-0.3.0/k8s/start.sh
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling/__init__.py
+-rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling/app.py
+-rw-r--r--   0        0        0     6601 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling/config.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling/default_app_config.py
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling/engine_factory.py
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling/error.py
+-rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling/mixin.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling/sdk.py
+-rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling/service.py
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling/utilities.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling/engine/__init__.py
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling/engine/base_engine.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling/engine/dummy_engine.py
+-rw-r--r--   0        0        0    11737 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling/engine/rms_engine.py
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling/engine/sms_engine.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling/engine/stop_engine.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling/evaluation/__init__.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling/evaluation/base_hook.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling/evaluation/dummy_hook.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling/evaluation/hook_msg.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling/evaluation/warn_hook.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling/evaluation_extension/__init__.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling/evaluation_extension/dummy_extension/__init__.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling/evaluation_extension/dummy_extension/dummy_hook.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling/file_format/__init__.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling/file_format/base_file_format.py
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling/file_format/csv_file_imp.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling/file_format/file_factory.py
+-rw-r--r--   0        0        0     5779 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling/file_format/output_adapter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling/proto/__init__.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling/proto/sampling_service_pb2.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling/proto/sampling_service_pb2_grpc.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling/sample/__init__.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling/sample/base_sampling.py
+-rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling/sample/cluster_sampling_imp.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling/sample/random_sampling_imp.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling/sample/sampling_factory.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling/sample/simple_sampling_imp.py
+-rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling/sample/stratified_sampling_imp.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling_proto/README.md
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling_proto/pyproject.toml
+-rw-r--r--   0        0        0     7201 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling_proto/pb/sampling_service.proto
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling_proto/sparksampling_proto/__init__.py
+-rw-r--r--   0        0        0     7621 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling_proto/sparksampling_proto/sampling_service_pb2.py
+-rw-r--r--   0        0        0     5934 2020-02-02 00:00:00.000000 sparksampling-0.3.0/sparksampling_proto/sparksampling_proto/sampling_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 sparksampling-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 sparksampling-0.3.0/tests/test_feature.py
+-rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 sparksampling-0.3.0/tests/test_rms_engine.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 sparksampling-0.3.0/tests/test_s3.py
+-rw-r--r--   0        0        0    13415 2020-02-02 00:00:00.000000 sparksampling-0.3.0/tests/test_sms_sampling.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 sparksampling-0.3.0/tests/utilities.py
+-rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 sparksampling-0.3.0/.gitignore
+-rw-r--r--   0        0        0    11324 2020-02-02 00:00:00.000000 sparksampling-0.3.0/LICENSE
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 sparksampling-0.3.0/README.md
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 sparksampling-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 sparksampling-0.3.0/PKG-INFO
```

### Comparing `sparksampling-0.2.2/.pre-commit-config.yaml` & `sparksampling-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/RELEASE.md` & `sparksampling-0.3.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/client/LICENSE` & `sparksampling-0.3.0/client/LICENSE`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/client/README.md` & `sparksampling-0.3.0/client/README.md`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/client/RELEASE.md` & `sparksampling-0.3.0/client/RELEASE.md`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/client/pyproject.toml` & `sparksampling-0.3.0/client/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "sparksampling_client"
 description = "client for sparksampling"
 keywords = ["sparksampling_client", "pyspark-sampling"]
 requires-python = ">=3.7"
 dependencies = [
     'click',
-    'sparksampling_proto==0.0.1',
+    'sparksampling_proto==0.1.0',
 ]
 dynamic = ["version", ]
 classifiers = [
     'Development Status :: 2 - Pre-Alpha',
     'Intended Audience :: Developers',
     'Natural Language :: English',
     'Programming Language :: Python :: 3',
```

### Comparing `sparksampling-0.2.2/client/sparksampling_client/cli.py` & `sparksampling-0.3.0/client/sparksampling_client/cli.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/client/sparksampling_client/config.py` & `sparksampling-0.3.0/client/sparksampling_client/config.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/client/sparksampling_client/session.py` & `sparksampling-0.3.0/client/sparksampling_client/session.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/client/tests/test_apply.py` & `sparksampling-0.3.0/client/tests/test_apply.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/data/10w_x_10.csv` & `sparksampling-0.3.0/data/10w_x_10.csv`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/data/iris.csv` & `sparksampling-0.3.0/data/iris.csv`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/data/ten_million_top1k.csv` & `sparksampling-0.3.0/data/ten_million_top1k.csv`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/data/unbalance_500v50_10.csv` & `sparksampling-0.3.0/data/unbalance_500v50_10.csv`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/data/unbalance_5w1k_10.csv` & `sparksampling-0.3.0/data/unbalance_5w1k_10.csv`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/data/unbalance_5w5k_10.csv` & `sparksampling-0.3.0/data/unbalance_5w5k_10.csv`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/example/extension-example/DEVELOP.md` & `sparksampling-0.3.0/example/extension-example/DEVELOP.md`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/example/extension-example/setup.py` & `sparksampling-0.3.0/example/extension-example/setup.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/k8s/spark-sampling-deployment.yaml` & `sparksampling-0.3.0/k8s/spark-sampling-deployment.yaml`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/sparksampling/app.py` & `sparksampling-0.3.0/sparksampling/app.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/sparksampling/config.py` & `sparksampling-0.3.0/sparksampling/config.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/sparksampling/engine_factory.py` & `sparksampling-0.3.0/sparksampling/engine_factory.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/sparksampling/error.py` & `sparksampling-0.3.0/sparksampling/error.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/sparksampling/mixin.py` & `sparksampling-0.3.0/sparksampling/mixin.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/sparksampling/service.py` & `sparksampling-0.3.0/sparksampling/service.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/sparksampling/utilities.py` & `sparksampling-0.3.0/sparksampling/utilities.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/sparksampling/engine/base_engine.py` & `sparksampling-0.3.0/sparksampling/engine/base_engine.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/sparksampling/engine/dummy_engine.py` & `sparksampling-0.3.0/sparksampling/engine/dummy_engine.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/sparksampling/engine/rms_engine.py` & `sparksampling-0.3.0/sparksampling/engine/rms_engine.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/sparksampling/engine/sms_engine.py` & `sparksampling-0.3.0/sparksampling/engine/sms_engine.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/sparksampling/evaluation/__init__.py` & `sparksampling-0.3.0/sparksampling/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/sparksampling/evaluation/base_hook.py` & `sparksampling-0.3.0/sparksampling/evaluation/base_hook.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/sparksampling/file_format/base_file_format.py` & `sparksampling-0.3.0/sparksampling/file_format/base_file_format.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/sparksampling/file_format/csv_file_imp.py` & `sparksampling-0.3.0/sparksampling/file_format/csv_file_imp.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/sparksampling/file_format/file_factory.py` & `sparksampling-0.3.0/sparksampling/file_format/file_factory.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/sparksampling/file_format/output_adapter.py` & `sparksampling-0.3.0/sparksampling/file_format/output_adapter.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/sparksampling/sample/base_sampling.py` & `sparksampling-0.3.0/sparksampling/sample/base_sampling.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/sparksampling/sample/cluster_sampling_imp.py` & `sparksampling-0.3.0/sparksampling/sample/cluster_sampling_imp.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/sparksampling/sample/random_sampling_imp.py` & `sparksampling-0.3.0/sparksampling/sample/random_sampling_imp.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/sparksampling/sample/sampling_factory.py` & `sparksampling-0.3.0/sparksampling/sample/sampling_factory.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/sparksampling/sample/simple_sampling_imp.py` & `sparksampling-0.3.0/sparksampling/sample/simple_sampling_imp.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/sparksampling/sample/stratified_sampling_imp.py` & `sparksampling-0.3.0/sparksampling/sample/stratified_sampling_imp.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/sparksampling_proto/pyproject.toml` & `sparksampling-0.3.0/sparksampling_proto/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 requires = ["hatchling", ]
 build-backend = "hatchling.build"
 
 [project]
 name = "sparksampling-proto"
 description = "python proto for sparksampling"
 keywords = ["sparksampling"]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dependencies = [
     'grpcio>=1.51.0',
+    'grpcio-tools>=1.15.0',
     'protobuf>=4',
 ]
 dynamic = ["version", ]
 
 [[project.authors]]
 name = "Wh1isper"
 email = "9573586@qq.com"
```

### Comparing `sparksampling-0.2.2/sparksampling_proto/pb/sampling_service.proto` & `sparksampling-0.3.0/sparksampling_proto/pb/sampling_service.proto`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/sparksampling_proto/sparksampling_proto/sampling_service_pb2.py` & `sparksampling-0.3.0/sparksampling_proto/sparksampling_proto/sampling_service_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,63 +1,64 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: sampling_service.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
+
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-
-
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16sampling_service.proto\"\xea\x01\n\x0fSamplingRequest\x12,\n\x0fsampling_method\x18\x01 \x01(\x0e\x32\x13.SamplingMethodType\x12$\n\x0b\x66ile_format\x18\x02 \x01(\x0e\x32\x0f.FileFormatType\x12$\n\rsampling_conf\x18\x03 \x01(\x0b\x32\r.SamplingConf\x12$\n\x0b\x66ormat_conf\x18\x04 \x01(\x0b\x32\x0f.FileFormatConf\x12\x12\n\ninput_path\x18\x05 \x01(\t\x12\x13\n\x0boutput_path\x18\x06 \x01(\t\x12\x0e\n\x06job_id\x18\x07 \x01(\t\"\x1f\n\rCancelRequest\x12\x0e\n\x06job_id\x18\x01 \x01(\t\"/\n\x0e\x43\x61ncelResponse\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\"\xcf\x01\n\x10SamplingResponse\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12,\n\x04\x64\x61ta\x18\x03 \x01(\x0b\x32\x1e.SamplingResponse.ResponseData\x1an\n\x0cResponseData\x12(\n\x0eparent_request\x18\x01 \x01(\x0b\x32\x10.SamplingRequest\x12\x14\n\x0csampled_path\x18\x02 \x01(\t\x12\x1e\n\x08hook_msg\x18\x03 \x03(\x0b\x32\x0c.HookMessage\"#\n\x04\x64ict\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\xbe\x01\n\x0cSamplingConf\x12\x10\n\x08\x66raction\x18\x01 \x01(\t\x12\x18\n\x10with_replacement\x18\x02 \x01(\x08\x12\x0c\n\x04seed\x18\x03 \x01(\r\x12\x16\n\x0estratified_key\x18\x04 \x01(\t\x12\r\n\x05\x63ount\x18\x05 \x01(\r\x12\x14\n\x0csampling_col\x18\x06 \x03(\t\x12\x10\n\x08group_by\x18\x07 \x01(\t\x12\x11\n\tgroup_num\x18\x08 \x01(\r\x12\x12\n\nensure_col\x18\t \x01(\x08\"2\n\x0e\x46ileFormatConf\x12\x13\n\x0bwith_header\x18\x01 \x01(\x08\x12\x0b\n\x03sep\x18\x02 \x01(\t\"\xb0\x08\n\x17RelationSamplingRequest\x12?\n\x0fsampling_stages\x18\x01 \x03(\x0b\x32&.RelationSamplingRequest.SamplingStage\x12?\n\x0frelation_stages\x18\x02 \x03(\x0b\x32&.RelationSamplingRequest.RelationStage\x12\x0e\n\x06job_id\x18\x03 \x01(\t\x12\x34\n\x17\x64\x65\x66\x61ult_sampling_method\x18\x04 \x01(\x0e\x32\x13.SamplingMethodType\x12,\n\x15\x64\x65\x66\x61ult_sampling_conf\x18\x05 \x01(\x0b\x32\r.SamplingConf\x12,\n\x13\x64\x65\x66\x61ult_file_format\x18\x06 \x01(\x0e\x32\x0f.FileFormatType\x12,\n\x13\x64\x65\x66\x61ult_format_conf\x18\x07 \x01(\x0b\x32\x0f.FileFormatConf\x12\x0f\n\x07\x64ry_run\x18\x08 \x01(\x08\x1a\x8e\x02\n\rSamplingStage\x12\x12\n\ninput_path\x18\x01 \x01(\t\x12\x12\n\ninput_name\x18\x02 \x01(\t\x12\x13\n\x0boutput_path\x18\x03 \x01(\t\x12\x12\n\noutput_col\x18\x04 \x03(\t\x12\x0c\n\x04name\x18\x05 \x01(\t\x12,\n\x0fsampling_method\x18\x06 \x01(\x0e\x32\x13.SamplingMethodType\x12$\n\rsampling_conf\x18\x07 \x01(\x0b\x32\r.SamplingConf\x12$\n\x0b\x66ile_format\x18\x08 \x01(\x0e\x32\x0f.FileFormatType\x12$\n\x0b\x66ormat_conf\x18\t \x01(\x0b\x32\x0f.FileFormatConf\x1a\xad\x01\n\x08Relation\x12\x15\n\rrelation_path\x18\x01 \x01(\t\x12\x15\n\rrelation_name\x18\x02 \x01(\t\x12\x14\n\x0crelation_col\x18\x03 \x01(\t\x12\x11\n\tinput_col\x18\x04 \x01(\t\x12$\n\x0b\x66ile_format\x18\x05 \x01(\x0e\x32\x0f.FileFormatType\x12$\n\x0b\x66ormat_conf\x18\x06 \x01(\x0b\x32\x0f.FileFormatConf\x1a\xf0\x01\n\rRelationStage\x12\x12\n\ninput_path\x18\x01 \x01(\t\x12\x12\n\ninput_name\x18\x02 \x01(\t\x12\x13\n\x0boutput_path\x18\x03 \x01(\t\x12\x12\n\noutput_col\x18\x04 \x03(\t\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x34\n\trelations\x18\x06 \x03(\x0b\x32!.RelationSamplingRequest.Relation\x12$\n\x0b\x66ile_format\x18\x07 \x01(\x0e\x32\x0f.FileFormatType\x12$\n\x0b\x66ormat_conf\x18\x08 \x01(\x0b\x32\x0f.FileFormatConf\"\xbe\x02\n\x18RelationSamplingResponse\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x34\n\x04\x64\x61ta\x18\x03 \x01(\x0b\x32&.RelationSamplingResponse.ResponseData\x1aR\n\x0cSampleResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x14\n\x0csampled_path\x18\x02 \x01(\t\x12\x1e\n\x08hook_msg\x18\x03 \x03(\x0b\x32\x0c.HookMessage\x1ay\n\x0cResponseData\x12\x30\n\x0eparent_request\x18\x01 \x01(\x0b\x32\x18.RelationSamplingRequest\x12\x37\n\x07results\x18\x02 \x03(\x0b\x32&.RelationSamplingResponse.SampleResult\"E\n\x0bHookMessage\x12\x11\n\thook_name\x18\x01 \x01(\t\x12\x0e\n\x06period\x18\x02 \x01(\t\x12\x13\n\x04meta\x18\x03 \x03(\x0b\x32\x05.pair\"\"\n\x04pair\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t*\x9d\x01\n\x12SamplingMethodType\x12\x12\n\x0eUNKNOWN_METHOD\x10\x00\x12\x1a\n\x16RANDOM_SAMPLING_METHOD\x10\x01\x12\x1e\n\x1aSTRATIFIED_SAMPLING_METHOD\x10\x02\x12\x1a\n\x16SIMPLE_SAMPLING_METHOD\x10\x03\x12\x1b\n\x17\x43LUSTER_SAMPLING_METHOD\x10\x04*9\n\x0e\x46ileFormatType\x12\x12\n\x0eUNKNOWN_FORMAT\x10\x00\x12\x13\n\x0f\x46ILE_FORMAT_CSV\x10\x01\x32\xca\x01\n\x14SparkSamplingService\x12\x34\n\x0bSamplingJob\x12\x10.SamplingRequest\x1a\x11.SamplingResponse\"\x00\x12L\n\x13RelationSamplingJob\x12\x18.RelationSamplingRequest\x1a\x19.RelationSamplingResponse\"\x00\x12.\n\tCancelJob\x12\x0e.CancelRequest\x1a\x0f.CancelResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
+    b'\n\x16sampling_service.proto"\xea\x01\n\x0fSamplingRequest\x12,\n\x0fsampling_method\x18\x01 \x01(\x0e\x32\x13.SamplingMethodType\x12$\n\x0b\x66ile_format\x18\x02 \x01(\x0e\x32\x0f.FileFormatType\x12$\n\rsampling_conf\x18\x03 \x01(\x0b\x32\r.SamplingConf\x12$\n\x0b\x66ormat_conf\x18\x04 \x01(\x0b\x32\x0f.FileFormatConf\x12\x12\n\ninput_path\x18\x05 \x01(\t\x12\x13\n\x0boutput_path\x18\x06 \x01(\t\x12\x0e\n\x06job_id\x18\x07 \x01(\t"\x1f\n\rCancelRequest\x12\x0e\n\x06job_id\x18\x01 \x01(\t"/\n\x0e\x43\x61ncelResponse\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t"\xcf\x01\n\x10SamplingResponse\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12,\n\x04\x64\x61ta\x18\x03 \x01(\x0b\x32\x1e.SamplingResponse.ResponseData\x1an\n\x0cResponseData\x12(\n\x0eparent_request\x18\x01 \x01(\x0b\x32\x10.SamplingRequest\x12\x14\n\x0csampled_path\x18\x02 \x01(\t\x12\x1e\n\x08hook_msg\x18\x03 \x03(\x0b\x32\x0c.HookMessage"#\n\x04\x64ict\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t"\xbe\x01\n\x0cSamplingConf\x12\x10\n\x08\x66raction\x18\x01 \x01(\t\x12\x18\n\x10with_replacement\x18\x02 \x01(\x08\x12\x0c\n\x04seed\x18\x03 \x01(\r\x12\x16\n\x0estratified_key\x18\x04 \x01(\t\x12\r\n\x05\x63ount\x18\x05 \x01(\r\x12\x14\n\x0csampling_col\x18\x06 \x03(\t\x12\x10\n\x08group_by\x18\x07 \x01(\t\x12\x11\n\tgroup_num\x18\x08 \x01(\r\x12\x12\n\nensure_col\x18\t \x01(\x08"2\n\x0e\x46ileFormatConf\x12\x13\n\x0bwith_header\x18\x01 \x01(\x08\x12\x0b\n\x03sep\x18\x02 \x01(\t"\xb0\x08\n\x17RelationSamplingRequest\x12?\n\x0fsampling_stages\x18\x01 \x03(\x0b\x32&.RelationSamplingRequest.SamplingStage\x12?\n\x0frelation_stages\x18\x02 \x03(\x0b\x32&.RelationSamplingRequest.RelationStage\x12\x0e\n\x06job_id\x18\x03 \x01(\t\x12\x34\n\x17\x64\x65\x66\x61ult_sampling_method\x18\x04 \x01(\x0e\x32\x13.SamplingMethodType\x12,\n\x15\x64\x65\x66\x61ult_sampling_conf\x18\x05 \x01(\x0b\x32\r.SamplingConf\x12,\n\x13\x64\x65\x66\x61ult_file_format\x18\x06 \x01(\x0e\x32\x0f.FileFormatType\x12,\n\x13\x64\x65\x66\x61ult_format_conf\x18\x07 \x01(\x0b\x32\x0f.FileFormatConf\x12\x0f\n\x07\x64ry_run\x18\x08 \x01(\x08\x1a\x8e\x02\n\rSamplingStage\x12\x12\n\ninput_path\x18\x01 \x01(\t\x12\x12\n\ninput_name\x18\x02 \x01(\t\x12\x13\n\x0boutput_path\x18\x03 \x01(\t\x12\x12\n\noutput_col\x18\x04 \x03(\t\x12\x0c\n\x04name\x18\x05 \x01(\t\x12,\n\x0fsampling_method\x18\x06 \x01(\x0e\x32\x13.SamplingMethodType\x12$\n\rsampling_conf\x18\x07 \x01(\x0b\x32\r.SamplingConf\x12$\n\x0b\x66ile_format\x18\x08 \x01(\x0e\x32\x0f.FileFormatType\x12$\n\x0b\x66ormat_conf\x18\t \x01(\x0b\x32\x0f.FileFormatConf\x1a\xad\x01\n\x08Relation\x12\x15\n\rrelation_path\x18\x01 \x01(\t\x12\x15\n\rrelation_name\x18\x02 \x01(\t\x12\x14\n\x0crelation_col\x18\x03 \x01(\t\x12\x11\n\tinput_col\x18\x04 \x01(\t\x12$\n\x0b\x66ile_format\x18\x05 \x01(\x0e\x32\x0f.FileFormatType\x12$\n\x0b\x66ormat_conf\x18\x06 \x01(\x0b\x32\x0f.FileFormatConf\x1a\xf0\x01\n\rRelationStage\x12\x12\n\ninput_path\x18\x01 \x01(\t\x12\x12\n\ninput_name\x18\x02 \x01(\t\x12\x13\n\x0boutput_path\x18\x03 \x01(\t\x12\x12\n\noutput_col\x18\x04 \x03(\t\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x34\n\trelations\x18\x06 \x03(\x0b\x32!.RelationSamplingRequest.Relation\x12$\n\x0b\x66ile_format\x18\x07 \x01(\x0e\x32\x0f.FileFormatType\x12$\n\x0b\x66ormat_conf\x18\x08 \x01(\x0b\x32\x0f.FileFormatConf"\xbe\x02\n\x18RelationSamplingResponse\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x34\n\x04\x64\x61ta\x18\x03 \x01(\x0b\x32&.RelationSamplingResponse.ResponseData\x1aR\n\x0cSampleResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x14\n\x0csampled_path\x18\x02 \x01(\t\x12\x1e\n\x08hook_msg\x18\x03 \x03(\x0b\x32\x0c.HookMessage\x1ay\n\x0cResponseData\x12\x30\n\x0eparent_request\x18\x01 \x01(\x0b\x32\x18.RelationSamplingRequest\x12\x37\n\x07results\x18\x02 \x03(\x0b\x32&.RelationSamplingResponse.SampleResult"E\n\x0bHookMessage\x12\x11\n\thook_name\x18\x01 \x01(\t\x12\x0e\n\x06period\x18\x02 \x01(\t\x12\x13\n\x04meta\x18\x03 \x03(\x0b\x32\x05.pair""\n\x04pair\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t*\x9d\x01\n\x12SamplingMethodType\x12\x12\n\x0eUNKNOWN_METHOD\x10\x00\x12\x1a\n\x16RANDOM_SAMPLING_METHOD\x10\x01\x12\x1e\n\x1aSTRATIFIED_SAMPLING_METHOD\x10\x02\x12\x1a\n\x16SIMPLE_SAMPLING_METHOD\x10\x03\x12\x1b\n\x17\x43LUSTER_SAMPLING_METHOD\x10\x04*9\n\x0e\x46ileFormatType\x12\x12\n\x0eUNKNOWN_FORMAT\x10\x00\x12\x13\n\x0f\x46ILE_FORMAT_CSV\x10\x01\x32\xca\x01\n\x14SparkSamplingService\x12\x34\n\x0bSamplingJob\x12\x10.SamplingRequest\x1a\x11.SamplingResponse"\x00\x12L\n\x13RelationSamplingJob\x12\x18.RelationSamplingRequest\x1a\x19.RelationSamplingResponse"\x00\x12.\n\tCancelJob\x12\x0e.CancelRequest\x1a\x0f.CancelResponse"\x00\x62\x06proto3'
+)
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sampling_service_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "sampling_service_pb2", globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
-  DESCRIPTOR._options = None
-  _SAMPLINGMETHODTYPE._serialized_start=2341
-  _SAMPLINGMETHODTYPE._serialized_end=2498
-  _FILEFORMATTYPE._serialized_start=2500
-  _FILEFORMATTYPE._serialized_end=2557
-  _SAMPLINGREQUEST._serialized_start=27
-  _SAMPLINGREQUEST._serialized_end=261
-  _CANCELREQUEST._serialized_start=263
-  _CANCELREQUEST._serialized_end=294
-  _CANCELRESPONSE._serialized_start=296
-  _CANCELRESPONSE._serialized_end=343
-  _SAMPLINGRESPONSE._serialized_start=346
-  _SAMPLINGRESPONSE._serialized_end=553
-  _SAMPLINGRESPONSE_RESPONSEDATA._serialized_start=443
-  _SAMPLINGRESPONSE_RESPONSEDATA._serialized_end=553
-  _DICT._serialized_start=555
-  _DICT._serialized_end=590
-  _SAMPLINGCONF._serialized_start=593
-  _SAMPLINGCONF._serialized_end=783
-  _FILEFORMATCONF._serialized_start=785
-  _FILEFORMATCONF._serialized_end=835
-  _RELATIONSAMPLINGREQUEST._serialized_start=838
-  _RELATIONSAMPLINGREQUEST._serialized_end=1910
-  _RELATIONSAMPLINGREQUEST_SAMPLINGSTAGE._serialized_start=1221
-  _RELATIONSAMPLINGREQUEST_SAMPLINGSTAGE._serialized_end=1491
-  _RELATIONSAMPLINGREQUEST_RELATION._serialized_start=1494
-  _RELATIONSAMPLINGREQUEST_RELATION._serialized_end=1667
-  _RELATIONSAMPLINGREQUEST_RELATIONSTAGE._serialized_start=1670
-  _RELATIONSAMPLINGREQUEST_RELATIONSTAGE._serialized_end=1910
-  _RELATIONSAMPLINGRESPONSE._serialized_start=1913
-  _RELATIONSAMPLINGRESPONSE._serialized_end=2231
-  _RELATIONSAMPLINGRESPONSE_SAMPLERESULT._serialized_start=2026
-  _RELATIONSAMPLINGRESPONSE_SAMPLERESULT._serialized_end=2108
-  _RELATIONSAMPLINGRESPONSE_RESPONSEDATA._serialized_start=2110
-  _RELATIONSAMPLINGRESPONSE_RESPONSEDATA._serialized_end=2231
-  _HOOKMESSAGE._serialized_start=2233
-  _HOOKMESSAGE._serialized_end=2302
-  _PAIR._serialized_start=2304
-  _PAIR._serialized_end=2338
-  _SPARKSAMPLINGSERVICE._serialized_start=2560
-  _SPARKSAMPLINGSERVICE._serialized_end=2762
+    DESCRIPTOR._options = None
+    _SAMPLINGMETHODTYPE._serialized_start = 2341
+    _SAMPLINGMETHODTYPE._serialized_end = 2498
+    _FILEFORMATTYPE._serialized_start = 2500
+    _FILEFORMATTYPE._serialized_end = 2557
+    _SAMPLINGREQUEST._serialized_start = 27
+    _SAMPLINGREQUEST._serialized_end = 261
+    _CANCELREQUEST._serialized_start = 263
+    _CANCELREQUEST._serialized_end = 294
+    _CANCELRESPONSE._serialized_start = 296
+    _CANCELRESPONSE._serialized_end = 343
+    _SAMPLINGRESPONSE._serialized_start = 346
+    _SAMPLINGRESPONSE._serialized_end = 553
+    _SAMPLINGRESPONSE_RESPONSEDATA._serialized_start = 443
+    _SAMPLINGRESPONSE_RESPONSEDATA._serialized_end = 553
+    _DICT._serialized_start = 555
+    _DICT._serialized_end = 590
+    _SAMPLINGCONF._serialized_start = 593
+    _SAMPLINGCONF._serialized_end = 783
+    _FILEFORMATCONF._serialized_start = 785
+    _FILEFORMATCONF._serialized_end = 835
+    _RELATIONSAMPLINGREQUEST._serialized_start = 838
+    _RELATIONSAMPLINGREQUEST._serialized_end = 1910
+    _RELATIONSAMPLINGREQUEST_SAMPLINGSTAGE._serialized_start = 1221
+    _RELATIONSAMPLINGREQUEST_SAMPLINGSTAGE._serialized_end = 1491
+    _RELATIONSAMPLINGREQUEST_RELATION._serialized_start = 1494
+    _RELATIONSAMPLINGREQUEST_RELATION._serialized_end = 1667
+    _RELATIONSAMPLINGREQUEST_RELATIONSTAGE._serialized_start = 1670
+    _RELATIONSAMPLINGREQUEST_RELATIONSTAGE._serialized_end = 1910
+    _RELATIONSAMPLINGRESPONSE._serialized_start = 1913
+    _RELATIONSAMPLINGRESPONSE._serialized_end = 2231
+    _RELATIONSAMPLINGRESPONSE_SAMPLERESULT._serialized_start = 2026
+    _RELATIONSAMPLINGRESPONSE_SAMPLERESULT._serialized_end = 2108
+    _RELATIONSAMPLINGRESPONSE_RESPONSEDATA._serialized_start = 2110
+    _RELATIONSAMPLINGRESPONSE_RESPONSEDATA._serialized_end = 2231
+    _HOOKMESSAGE._serialized_start = 2233
+    _HOOKMESSAGE._serialized_end = 2302
+    _PAIR._serialized_start = 2304
+    _PAIR._serialized_end = 2338
+    _SPARKSAMPLINGSERVICE._serialized_start = 2560
+    _SPARKSAMPLINGSERVICE._serialized_end = 2762
 # @@protoc_insertion_point(module_scope)
```

### Comparing `sparksampling-0.2.2/sparksampling_proto/sparksampling_proto/sampling_service_pb2_grpc.py` & `sparksampling-0.3.0/sparksampling_proto/sparksampling_proto/sampling_service_pb2_grpc.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,122 +11,159 @@
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.SamplingJob = channel.unary_unary(
-                '/SparkSamplingService/SamplingJob',
-                request_serializer=sampling__service__pb2.SamplingRequest.SerializeToString,
-                response_deserializer=sampling__service__pb2.SamplingResponse.FromString,
-                )
+            "/SparkSamplingService/SamplingJob",
+            request_serializer=sampling__service__pb2.SamplingRequest.SerializeToString,
+            response_deserializer=sampling__service__pb2.SamplingResponse.FromString,
+        )
         self.RelationSamplingJob = channel.unary_unary(
-                '/SparkSamplingService/RelationSamplingJob',
-                request_serializer=sampling__service__pb2.RelationSamplingRequest.SerializeToString,
-                response_deserializer=sampling__service__pb2.RelationSamplingResponse.FromString,
-                )
+            "/SparkSamplingService/RelationSamplingJob",
+            request_serializer=sampling__service__pb2.RelationSamplingRequest.SerializeToString,
+            response_deserializer=sampling__service__pb2.RelationSamplingResponse.FromString,
+        )
         self.CancelJob = channel.unary_unary(
-                '/SparkSamplingService/CancelJob',
-                request_serializer=sampling__service__pb2.CancelRequest.SerializeToString,
-                response_deserializer=sampling__service__pb2.CancelResponse.FromString,
-                )
+            "/SparkSamplingService/CancelJob",
+            request_serializer=sampling__service__pb2.CancelRequest.SerializeToString,
+            response_deserializer=sampling__service__pb2.CancelResponse.FromString,
+        )
 
 
 class SparkSamplingServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def SamplingJob(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
+        context.set_details("Method not implemented!")
+        raise NotImplementedError("Method not implemented!")
 
     def RelationSamplingJob(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
+        context.set_details("Method not implemented!")
+        raise NotImplementedError("Method not implemented!")
 
     def CancelJob(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
+        context.set_details("Method not implemented!")
+        raise NotImplementedError("Method not implemented!")
 
 
 def add_SparkSamplingServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
-            'SamplingJob': grpc.unary_unary_rpc_method_handler(
-                    servicer.SamplingJob,
-                    request_deserializer=sampling__service__pb2.SamplingRequest.FromString,
-                    response_serializer=sampling__service__pb2.SamplingResponse.SerializeToString,
-            ),
-            'RelationSamplingJob': grpc.unary_unary_rpc_method_handler(
-                    servicer.RelationSamplingJob,
-                    request_deserializer=sampling__service__pb2.RelationSamplingRequest.FromString,
-                    response_serializer=sampling__service__pb2.RelationSamplingResponse.SerializeToString,
-            ),
-            'CancelJob': grpc.unary_unary_rpc_method_handler(
-                    servicer.CancelJob,
-                    request_deserializer=sampling__service__pb2.CancelRequest.FromString,
-                    response_serializer=sampling__service__pb2.CancelResponse.SerializeToString,
-            ),
+        "SamplingJob": grpc.unary_unary_rpc_method_handler(
+            servicer.SamplingJob,
+            request_deserializer=sampling__service__pb2.SamplingRequest.FromString,
+            response_serializer=sampling__service__pb2.SamplingResponse.SerializeToString,
+        ),
+        "RelationSamplingJob": grpc.unary_unary_rpc_method_handler(
+            servicer.RelationSamplingJob,
+            request_deserializer=sampling__service__pb2.RelationSamplingRequest.FromString,
+            response_serializer=sampling__service__pb2.RelationSamplingResponse.SerializeToString,
+        ),
+        "CancelJob": grpc.unary_unary_rpc_method_handler(
+            servicer.CancelJob,
+            request_deserializer=sampling__service__pb2.CancelRequest.FromString,
+            response_serializer=sampling__service__pb2.CancelResponse.SerializeToString,
+        ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'SparkSamplingService', rpc_method_handlers)
+        "SparkSamplingService", rpc_method_handlers
+    )
     server.add_generic_rpc_handlers((generic_handler,))
 
 
- # This class is part of an EXPERIMENTAL API.
+# This class is part of an EXPERIMENTAL API.
 class SparkSamplingService(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def SamplingJob(request,
+    def SamplingJob(
+        request,
+        target,
+        options=(),
+        channel_credentials=None,
+        call_credentials=None,
+        insecure=False,
+        compression=None,
+        wait_for_ready=None,
+        timeout=None,
+        metadata=None,
+    ):
+        return grpc.experimental.unary_unary(
+            request,
             target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/SparkSamplingService/SamplingJob',
+            "/SparkSamplingService/SamplingJob",
             sampling__service__pb2.SamplingRequest.SerializeToString,
             sampling__service__pb2.SamplingResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+        )
 
     @staticmethod
-    def RelationSamplingJob(request,
+    def RelationSamplingJob(
+        request,
+        target,
+        options=(),
+        channel_credentials=None,
+        call_credentials=None,
+        insecure=False,
+        compression=None,
+        wait_for_ready=None,
+        timeout=None,
+        metadata=None,
+    ):
+        return grpc.experimental.unary_unary(
+            request,
             target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/SparkSamplingService/RelationSamplingJob',
+            "/SparkSamplingService/RelationSamplingJob",
             sampling__service__pb2.RelationSamplingRequest.SerializeToString,
             sampling__service__pb2.RelationSamplingResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+        )
 
     @staticmethod
-    def CancelJob(request,
+    def CancelJob(
+        request,
+        target,
+        options=(),
+        channel_credentials=None,
+        call_credentials=None,
+        insecure=False,
+        compression=None,
+        wait_for_ready=None,
+        timeout=None,
+        metadata=None,
+    ):
+        return grpc.experimental.unary_unary(
+            request,
             target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/SparkSamplingService/CancelJob',
+            "/SparkSamplingService/CancelJob",
             sampling__service__pb2.CancelRequest.SerializeToString,
             sampling__service__pb2.CancelResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+        )
```

### Comparing `sparksampling-0.2.2/tests/conftest.py` & `sparksampling-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/tests/test_feature.py` & `sparksampling-0.3.0/tests/test_feature.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/tests/test_rms_engine.py` & `sparksampling-0.3.0/tests/test_rms_engine.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/tests/test_s3.py` & `sparksampling-0.3.0/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/tests/test_sms_sampling.py` & `sparksampling-0.3.0/tests/test_sms_sampling.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/.gitignore` & `sparksampling-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/LICENSE` & `sparksampling-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/README.md` & `sparksampling-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `sparksampling-0.2.2/pyproject.toml` & `sparksampling-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 [build-system]
-requires = ["hatchling", ]
+requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sparksampling"
 description = "pyspark-sampling"
 keywords = ["sparksampling", "pyspark-sampling"]
-requires-python = ">=3.7"
+requires-python = ">=3.10"
 dependencies = [
-    "sparksampling-proto==0.0.1",
+    "sparksampling-proto>=0.1.0",
     'pyspark',
     'findspark',
     'traitlets',
     'pandas>=1.2',
     'requests',
     'kubernetes',
     'boto3',
     'grpcio-tools',
-    'graphlib_backport',
 ]
-dynamic = ["version", ]
+dynamic = ["version"]
 classifiers = [
     'Development Status :: 2 - Pre-Alpha',
     'Intended Audience :: Developers',
     'Natural Language :: English',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.5',
     'Programming Language :: Python :: 3.6',
@@ -32,19 +31,15 @@
 ]
 
 [project.scripts]
 sparksampling = "sparksampling.app:main"
 
 
 [project.optional-dependencies]
-test = [
-    "pytest",
-    "pytest-grpc",
-    "pre-commit",
-]
+test = ["pytest", "pytest-grpc", "pre-commit"]
 
 [[project.authors]]
 name = "Wh1isper"
 email = "9573586@qq.com"
 
 [project.readme]
 file = "README.md"
@@ -53,11 +48,11 @@
 [project.license]
 text = "Apache License 2.0"
 
 [project.urls]
 Source = "https://github.com/Wh1isper/pyspark-sampling"
 
 [tool.check-manifest]
-ignore = [".*", ]
+ignore = [".*"]
 
 [tool.hatch.version]
 path = "sparksampling/__init__.py"
```

### Comparing `sparksampling-0.2.2/PKG-INFO` & `sparksampling-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: sparksampling
-Version: 0.2.2
+Version: 0.3.0
 Summary: pyspark-sampling
 Project-URL: Source, https://github.com/Wh1isper/pyspark-sampling
 Author-email: Wh1isper <9573586@qq.com>
 License: Apache License 2.0
 License-File: LICENSE
 Keywords: pyspark-sampling,sparksampling
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Requires-Dist: boto3
 Requires-Dist: findspark
-Requires-Dist: graphlib-backport
 Requires-Dist: grpcio-tools
 Requires-Dist: kubernetes
 Requires-Dist: pandas>=1.2
 Requires-Dist: pyspark
 Requires-Dist: requests
-Requires-Dist: sparksampling-proto==0.0.1
+Requires-Dist: sparksampling-proto>=0.1.0
 Requires-Dist: traitlets
 Provides-Extra: test
 Requires-Dist: pre-commit; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-grpc; extra == 'test'
 Description-Content-Type: text/markdown
```

