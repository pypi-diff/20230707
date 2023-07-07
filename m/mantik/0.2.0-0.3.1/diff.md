# Comparing `tmp/mantik-0.2.0.tar.gz` & `tmp/mantik-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mantik-0.2.0.tar", max compression
+gzip compressed data, was "mantik-0.3.1.tar", max compression
```

## Comparing `mantik-0.2.0.tar` & `mantik-0.3.1.tar`

### file list

```diff
@@ -1,177 +1,191 @@
--rw-r--r--   0        0        0     1092 2023-04-18 14:25:32.607202 mantik-0.2.0/LICENSE
--rw-r--r--   0        0        0      506 2023-04-18 14:25:32.607202 mantik-0.2.0/README.md
--rw-r--r--   0        0        0     1925 2023-04-18 14:25:32.627204 mantik-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      217 2023-04-18 14:25:32.627204 mantik-0.2.0/src/mantik/__init__.py
--rw-r--r--   0        0        0       69 2023-04-18 14:25:32.627204 mantik-0.2.0/src/mantik/cli/__init__.py
--rw-r--r--   0        0        0     1241 2023-04-18 14:25:32.627204 mantik-0.2.0/src/mantik/cli/init.py
--rw-r--r--   0        0        0       71 2023-04-18 14:25:32.627204 mantik-0.2.0/src/mantik/cli/main.py
--rw-r--r--   0        0        0      234 2023-04-18 14:25:32.627204 mantik-0.2.0/src/mantik/cli/runs/__init__.py
--rw-r--r--   0        0        0       88 2023-04-18 14:25:32.627204 mantik-0.2.0/src/mantik/cli/runs/_arguments.py
--rw-r--r--   0        0        0      659 2023-04-18 14:25:32.627204 mantik-0.2.0/src/mantik/cli/runs/_callbacks.py
--rw-r--r--   0        0        0     1427 2023-04-18 14:25:32.627204 mantik-0.2.0/src/mantik/cli/runs/_options.py
--rw-r--r--   0        0        0      723 2023-04-18 14:25:32.627204 mantik-0.2.0/src/mantik/cli/runs/cancel.py
--rw-r--r--   0        0        0     1608 2023-04-18 14:25:32.627204 mantik-0.2.0/src/mantik/cli/runs/download.py
--rw-r--r--   0        0        0     1153 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/cli/runs/info.py
--rw-r--r--   0        0        0     2669 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/cli/runs/list.py
--rw-r--r--   0        0        0      723 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/cli/runs/logs.py
--rw-r--r--   0        0        0      116 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/cli/runs/runs.py
--rw-r--r--   0        0        0      696 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/cli/runs/status.py
--rw-r--r--   0        0        0     3026 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/cli/runs/submit.py
--rw-r--r--   0        0        0      316 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/compute_backend_service/__init__.py
--rw-r--r--   0        0        0     1739 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/compute_backend_service/_bearer.py
--rw-r--r--   0        0        0     3486 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/compute_backend_service/api.py
--rw-r--r--   0        0        0     1648 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/compute_backend_service/app.py
--rw-r--r--   0        0        0     3251 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/compute_backend_service/backend.py
--rw-r--r--   0        0        0     8072 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/compute_backend_service/client.py
--rw-r--r--   0        0        0     3297 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/compute_backend_service/exceptions.py
--rw-r--r--   0        0        0      324 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/compute_backend_service/models.py
--rw-r--r--   0        0        0     1196 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/compute_backend_service/settings.py
--rw-r--r--   0        0        0        0 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/mlflow_server/__init__.py
--rw-r--r--   0        0        0      126 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/mlflow_server/flask/__init__.py
--rw-r--r--   0        0        0     1160 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/mlflow_server/flask/_header.py
--rw-r--r--   0        0        0       90 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/mlflow_server/flask/api/__init__.py
--rw-r--r--   0        0        0       85 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/mlflow_server/flask/api/_exceptions.py
--rw-r--r--   0        0        0     1339 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/mlflow_server/flask/api/_get.py
--rw-r--r--   0        0        0      455 2023-04-18 14:25:32.628204 mantik-0.2.0/src/mantik/mlflow_server/flask/api/health.py
--rw-r--r--   0        0        0      109 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/flask/api/models/__init__.py
--rw-r--r--   0        0        0     1328 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/flask/api/models/requests.py
--rw-r--r--   0        0        0     1342 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/flask/api/models/responses.py
--rw-r--r--   0        0        0     1871 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/flask/api/tokens.py
--rw-r--r--   0        0        0       46 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/flask/app.py
--rw-r--r--   0        0        0     1796 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/flask/before_requests.py
--rw-r--r--   0        0        0      722 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/flask/skip.py
--rw-r--r--   0        0        0       41 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/gunicorn/__init__.py
--rw-r--r--   0        0        0     1278 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/gunicorn/_app.py
--rw-r--r--   0        0        0      882 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/gunicorn/_cli_args.py
--rw-r--r--   0        0        0      614 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/gunicorn/_env.py
--rw-r--r--   0        0        0      364 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/gunicorn/_options.py
--rw-r--r--   0        0        0      961 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/gunicorn/_stores.py
--rw-r--r--   0        0        0      508 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/gunicorn/run.py
--rw-r--r--   0        0        0      212 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/tokens/__init__.py
--rw-r--r--   0        0        0      256 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/tokens/cognito/__init__.py
--rw-r--r--   0        0        0     3612 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/tokens/cognito/_auth.py
--rw-r--r--   0        0        0     1532 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/tokens/cognito/api.py
--rw-r--r--   0        0        0     2053 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/tokens/cognito/client.py
--rw-r--r--   0        0        0     1659 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/tokens/cognito/credentials.py
--rw-r--r--   0        0        0      218 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/tokens/cognito/exceptions.py
--rw-r--r--   0        0        0     1250 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/tokens/cognito/tokens.py
--rw-r--r--   0        0        0      604 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/tokens/exceptions.py
--rw-r--r--   0        0        0     2127 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/tokens/jwks.py
--rw-r--r--   0        0        0     3248 2023-04-18 14:25:32.629204 mantik-0.2.0/src/mantik/mlflow_server/tokens/jwt.py
--rw-r--r--   0        0        0     3688 2023-04-18 14:25:32.630204 mantik-0.2.0/src/mantik/mlflow_server/tokens/verifier.py
--rw-r--r--   0        0        0        0 2023-04-18 14:25:32.630204 mantik-0.2.0/src/mantik/py.typed
--rw-r--r--   0        0        0      243 2023-04-18 14:25:32.630204 mantik-0.2.0/src/mantik/testing/__init__.py
--rw-r--r--   0        0        0     8518 2023-04-18 14:25:32.630204 mantik-0.2.0/src/mantik/testing/cognito.py
--rw-r--r--   0        0        0     2438 2023-04-18 14:25:32.630204 mantik-0.2.0/src/mantik/testing/config.py
--rw-r--r--   0        0        0      601 2023-04-18 14:25:32.630204 mantik-0.2.0/src/mantik/testing/contexts.py
--rw-r--r--   0        0        0     1251 2023-04-18 14:25:32.630204 mantik-0.2.0/src/mantik/testing/env.py
--rw-r--r--   0        0        0    12408 2023-04-18 14:25:32.630204 mantik-0.2.0/src/mantik/testing/mlflow_server.py
--rw-r--r--   0        0        0     6725 2023-04-18 14:25:32.630204 mantik-0.2.0/src/mantik/testing/pyunicore.py
--rw-r--r--   0        0        0      927 2023-04-18 14:25:32.630204 mantik-0.2.0/src/mantik/testing/requests.py
--rw-r--r--   0        0        0     1110 2023-04-18 14:25:32.630204 mantik-0.2.0/src/mantik/testing/token.py
--rw-r--r--   0        0        0       64 2023-04-18 14:25:32.630204 mantik-0.2.0/src/mantik/tracking/__init__.py
--rw-r--r--   0        0        0       73 2023-04-18 14:25:32.630204 mantik-0.2.0/src/mantik/tracking/_server/__init__.py
--rw-r--r--   0        0        0     1259 2023-04-18 14:25:32.630204 mantik-0.2.0/src/mantik/tracking/_server/_credentials.py
--rw-r--r--   0        0        0     3183 2023-04-18 14:25:32.630204 mantik-0.2.0/src/mantik/tracking/_server/api.py
--rw-r--r--   0        0        0     2586 2023-04-18 14:25:32.630204 mantik-0.2.0/src/mantik/tracking/_server/tokens.py
--rw-r--r--   0        0        0      920 2023-04-18 14:25:32.630204 mantik-0.2.0/src/mantik/tracking/environment.py
--rw-r--r--   0        0        0     2017 2023-04-18 14:25:32.630204 mantik-0.2.0/src/mantik/tracking/track.py
--rw-r--r--   0        0        0      250 2023-04-18 14:25:32.630204 mantik-0.2.0/src/mantik/unicore/__init__.py
--rw-r--r--   0        0        0     2799 2023-04-18 14:25:32.630204 mantik-0.2.0/src/mantik/unicore/_connect.py
--rw-r--r--   0        0        0     7939 2023-04-18 14:25:32.631204 mantik-0.2.0/src/mantik/unicore/backend.py
--rw-r--r--   0        0        0     3190 2023-04-18 14:25:32.631204 mantik-0.2.0/src/mantik/unicore/client.py
--rw-r--r--   0        0        0      226 2023-04-18 14:25:32.631204 mantik-0.2.0/src/mantik/unicore/config/__init__.py
--rw-r--r--   0        0        0      535 2023-04-18 14:25:32.631204 mantik-0.2.0/src/mantik/unicore/config/_base.py
--rw-r--r--   0        0        0     2776 2023-04-18 14:25:32.631204 mantik-0.2.0/src/mantik/unicore/config/_utils.py
--rw-r--r--   0        0        0     3886 2023-04-18 14:25:32.631204 mantik-0.2.0/src/mantik/unicore/config/core.py
--rw-r--r--   0        0        0     2876 2023-04-18 14:25:32.631204 mantik-0.2.0/src/mantik/unicore/config/environment.py
--rw-r--r--   0        0        0     7445 2023-04-18 14:25:32.631204 mantik-0.2.0/src/mantik/unicore/config/executable.py
--rw-r--r--   0        0        0     1072 2023-04-18 14:25:32.631204 mantik-0.2.0/src/mantik/unicore/config/read.py
--rw-r--r--   0        0        0     2739 2023-04-18 14:25:32.631204 mantik-0.2.0/src/mantik/unicore/config/resources.py
--rw-r--r--   0        0        0     3895 2023-04-18 14:25:32.631204 mantik-0.2.0/src/mantik/unicore/config/validate.py
--rw-r--r--   0        0        0      542 2023-04-18 14:25:32.631204 mantik-0.2.0/src/mantik/unicore/exceptions.py
--rw-r--r--   0        0        0     3458 2023-04-18 14:25:32.631204 mantik-0.2.0/src/mantik/unicore/job.py
--rw-r--r--   0        0        0     5644 2023-04-18 14:25:32.631204 mantik-0.2.0/src/mantik/unicore/properties.py
--rw-r--r--   0        0        0     2946 2023-04-18 14:25:32.631204 mantik-0.2.0/src/mantik/unicore/submitted_run.py
--rw-r--r--   0        0        0       67 2023-04-18 14:25:32.631204 mantik-0.2.0/src/mantik/unicore/utils/__init__.py
--rw-r--r--   0        0        0     1997 2023-04-18 14:25:32.631204 mantik-0.2.0/src/mantik/unicore/utils/upload.py
--rw-r--r--   0        0        0      763 2023-04-18 14:25:32.631204 mantik-0.2.0/src/mantik/unicore/utils/zip.py
--rw-r--r--   0        0        0     4054 2023-04-18 14:25:32.631204 mantik-0.2.0/src/mantik/unicore/working_dir.py
--rw-r--r--   0        0        0      105 2023-04-18 14:25:32.631204 mantik-0.2.0/src/mantik/utils/__init__.py
--rw-r--r--   0        0        0     2151 2023-04-18 14:25:32.631204 mantik-0.2.0/src/mantik/utils/env.py
--rw-r--r--   0        0        0      471 2023-04-18 14:25:32.632205 mantik-0.2.0/src/mantik/utils/mlflow.py
--rw-r--r--   0        0        0      615 2023-04-18 14:25:32.632205 mantik-0.2.0/src/mantik/utils/temp_dir.py
--rw-r--r--   0        0        0      320 2023-04-18 14:25:32.632205 mantik-0.2.0/src/mantik/utils/urls.py
--rw-r--r--   0        0        0      163 2023-04-18 14:25:32.632205 mantik-0.2.0/src/tests/resources/broken-project/MLproject
--rw-r--r--   0        0        0       77 2023-04-18 14:25:32.632205 mantik-0.2.0/src/tests/resources/broken-project/README.md
--rw-r--r--   0        0        0      248 2023-04-18 14:25:32.632205 mantik-0.2.0/src/tests/resources/broken-project/unicore-config.md
--rw-r--r--   0        0        0      574 2023-04-18 14:25:32.632205 mantik-0.2.0/src/tests/resources/cognito/auth-response.json
--rw-r--r--   0        0        0      159 2023-04-18 14:25:32.632205 mantik-0.2.0/src/tests/resources/cognito/different-client.json
--rw-r--r--   0        0        0      649 2023-04-18 14:25:32.632205 mantik-0.2.0/src/tests/resources/cognito/incorrect-login-credentials-response.json
--rw-r--r--   0        0        0      578 2023-04-18 14:25:32.632205 mantik-0.2.0/src/tests/resources/cognito/refresh-response.json
--rw-r--r--   0        0        0      631 2023-04-18 14:25:32.632205 mantik-0.2.0/src/tests/resources/cognito/refresh-token-expired-response.json
--rw-r--r--   0        0        0      623 2023-04-18 14:25:32.632205 mantik-0.2.0/src/tests/resources/cognito/refresh-token-invalid-response.json
--rw-r--r--   0        0        0      614 2023-04-18 14:25:32.632205 mantik-0.2.0/src/tests/resources/cognito/user-not-found-response.json
--rw-r--r--   0        0        0       57 2023-04-18 14:25:32.632205 mantik-0.2.0/src/tests/resources/test-project/Dockerfile
--rw-r--r--   0        0        0      182 2023-04-18 14:25:32.632205 mantik-0.2.0/src/tests/resources/test-project/MLproject
--rw-r--r--   0        0        0      168 2023-04-18 14:25:32.632205 mantik-0.2.0/src/tests/resources/test-project/config-with-errors.yaml
--rw-r--r--   0        0        0      536 2023-04-18 14:25:32.632205 mantik-0.2.0/src/tests/resources/test-project/main.py
--rw-r--r--   0        0        0        0 2023-04-18 14:25:32.632205 mantik-0.2.0/src/tests/resources/test-project/mantik-test.sif
--rw-r--r--   0        0        0       50 2023-04-18 14:25:32.632205 mantik-0.2.0/src/tests/resources/test-project/recipe.def
--rw-r--r--   0        0        0        0 2023-04-18 14:25:32.632205 mantik-0.2.0/src/tests/resources/test-project/test_subfolder/test.py
--rw-r--r--   0        0        0      246 2023-04-18 14:25:32.632205 mantik-0.2.0/src/tests/resources/test-project/unicore-config.json
--rw-r--r--   0        0        0      193 2023-04-18 14:25:32.632205 mantik-0.2.0/src/tests/resources/test-project/unicore-config.yaml
--rw-r--r--   0        0        0     2879 2023-04-18 14:25:32.632205 mantik-0.2.0/src/tests/resources/unicore-responses/job-property-response.json
--rw-r--r--   0        0        0      193 2023-04-18 14:25:32.632205 mantik-0.2.0/src/tests/unit/cli/conftest.py
--rw-r--r--   0        0        0      537 2023-04-18 14:25:32.633205 mantik-0.2.0/src/tests/unit/cli/runs/conftest.py
--rw-r--r--   0        0        0      555 2023-04-18 14:25:32.633205 mantik-0.2.0/src/tests/unit/cli/runs/test_cancel.py
--rw-r--r--   0        0        0     3201 2023-04-18 14:25:32.633205 mantik-0.2.0/src/tests/unit/cli/runs/test_download.py
--rw-r--r--   0        0        0     3506 2023-04-18 14:25:32.633205 mantik-0.2.0/src/tests/unit/cli/runs/test_info.py
--rw-r--r--   0        0        0      831 2023-04-18 14:25:32.633205 mantik-0.2.0/src/tests/unit/cli/runs/test_list.py
--rw-r--r--   0        0        0     1564 2023-04-18 14:25:32.633205 mantik-0.2.0/src/tests/unit/cli/runs/test_logs.py
--rw-r--r--   0        0        0      823 2023-04-18 14:25:32.633205 mantik-0.2.0/src/tests/unit/cli/runs/test_options.py
--rw-r--r--   0        0        0     1560 2023-04-18 14:25:32.633205 mantik-0.2.0/src/tests/unit/cli/runs/test_status.py
--rw-r--r--   0        0        0     5434 2023-04-18 14:25:32.633205 mantik-0.2.0/src/tests/unit/cli/runs/test_submit.py
--rw-r--r--   0        0        0      780 2023-04-18 14:25:32.633205 mantik-0.2.0/src/tests/unit/cli/test_init.py
--rw-r--r--   0        0        0     3920 2023-04-18 14:25:32.633205 mantik-0.2.0/src/tests/unit/compute_backend_service/conftest.py
--rw-r--r--   0        0        0     5719 2023-04-18 14:25:32.633205 mantik-0.2.0/src/tests/unit/compute_backend_service/test_api.py
--rw-r--r--   0        0        0      738 2023-04-18 14:25:32.633205 mantik-0.2.0/src/tests/unit/compute_backend_service/test_app.py
--rw-r--r--   0        0        0     3175 2023-04-18 14:25:32.633205 mantik-0.2.0/src/tests/unit/compute_backend_service/test_client.py
--rw-r--r--   0        0        0     1168 2023-04-18 14:25:32.633205 mantik-0.2.0/src/tests/unit/compute_backend_service/test_compute_backend.py
--rw-r--r--   0        0        0     8638 2023-04-18 14:25:32.633205 mantik-0.2.0/src/tests/unit/compute_backend_service/test_exception_handler.py
--rw-r--r--   0        0        0      327 2023-04-18 14:25:32.633205 mantik-0.2.0/src/tests/unit/compute_backend_service/test_models.py
--rw-r--r--   0        0        0     1479 2023-04-18 14:25:32.633205 mantik-0.2.0/src/tests/unit/conftest.py
--rw-r--r--   0        0        0     1585 2023-04-18 14:25:32.633205 mantik-0.2.0/src/tests/unit/mlflow_server/conftest.py
--rw-r--r--   0        0        0      191 2023-04-18 14:25:32.633205 mantik-0.2.0/src/tests/unit/mlflow_server/flask/api/test_health_api.py
--rw-r--r--   0        0        0     4375 2023-04-18 14:25:32.633205 mantik-0.2.0/src/tests/unit/mlflow_server/flask/api/test_tokens_api.py
--rw-r--r--   0        0        0      607 2023-04-18 14:25:32.634205 mantik-0.2.0/src/tests/unit/mlflow_server/flask/conftest.py
--rw-r--r--   0        0        0      894 2023-04-18 14:25:32.634205 mantik-0.2.0/src/tests/unit/mlflow_server/flask/test_flask_app.py
--rw-r--r--   0        0        0      469 2023-04-18 14:25:32.634205 mantik-0.2.0/src/tests/unit/mlflow_server/flask/test_skip.py
--rw-r--r--   0        0        0      391 2023-04-18 14:25:32.634205 mantik-0.2.0/src/tests/unit/mlflow_server/gunicorn/test_run.py
--rw-r--r--   0        0        0     4139 2023-04-18 14:25:32.634205 mantik-0.2.0/src/tests/unit/mlflow_server/tokens/cognito/test_auth.py
--rw-r--r--   0        0        0     2807 2023-04-18 14:25:32.634205 mantik-0.2.0/src/tests/unit/mlflow_server/tokens/test_verifier.py
--rw-r--r--   0        0        0     3121 2023-04-18 14:25:32.634205 mantik-0.2.0/src/tests/unit/tracking/_server/test_server_api.py
--rw-r--r--   0        0        0     1123 2023-04-18 14:25:32.634205 mantik-0.2.0/src/tests/unit/tracking/_server/test_tokens.py
--rw-r--r--   0        0        0     1838 2023-04-18 14:25:32.634205 mantik-0.2.0/src/tests/unit/tracking/test_credentials.py
--rw-r--r--   0        0        0     5525 2023-04-18 14:25:32.634205 mantik-0.2.0/src/tests/unit/tracking/test_track.py
--rw-r--r--   0        0        0     1211 2023-04-18 14:25:32.634205 mantik-0.2.0/src/tests/unit/unicore/config/conftest.py
--rw-r--r--   0        0        0    10055 2023-04-18 14:25:32.634205 mantik-0.2.0/src/tests/unit/unicore/config/test_core.py
--rw-r--r--   0        0        0     3136 2023-04-18 14:25:32.634205 mantik-0.2.0/src/tests/unit/unicore/config/test_environment.py
--rw-r--r--   0        0        0     1765 2023-04-18 14:25:32.634205 mantik-0.2.0/src/tests/unit/unicore/config/test_executable.py
--rw-r--r--   0        0        0     1945 2023-04-18 14:25:32.634205 mantik-0.2.0/src/tests/unit/unicore/config/test_read.py
--rw-r--r--   0        0        0     2981 2023-04-18 14:25:32.634205 mantik-0.2.0/src/tests/unit/unicore/config/test_utils.py
--rw-r--r--   0        0        0     8372 2023-04-18 14:25:32.634205 mantik-0.2.0/src/tests/unit/unicore/config/test_validate.py
--rw-r--r--   0        0        0     2629 2023-04-18 14:25:32.634205 mantik-0.2.0/src/tests/unit/unicore/conftest.py
--rw-r--r--   0        0        0     4259 2023-04-18 14:25:32.635205 mantik-0.2.0/src/tests/unit/unicore/test_backend.py
--rw-r--r--   0        0        0     1231 2023-04-18 14:25:32.635205 mantik-0.2.0/src/tests/unit/unicore/test_client_wrapper.py
--rw-r--r--   0        0        0     1870 2023-04-18 14:25:32.635205 mantik-0.2.0/src/tests/unit/unicore/test_connect.py
--rw-r--r--   0        0        0      516 2023-04-18 14:25:32.635205 mantik-0.2.0/src/tests/unit/unicore/test_exceptions.py
--rw-r--r--   0        0        0     1551 2023-04-18 14:25:32.635205 mantik-0.2.0/src/tests/unit/unicore/test_properties.py
--rw-r--r--   0        0        0     3707 2023-04-18 14:25:32.635205 mantik-0.2.0/src/tests/unit/unicore/test_submitted_run.py
--rw-r--r--   0        0        0     4240 2023-04-18 14:25:32.635205 mantik-0.2.0/src/tests/unit/unicore/utils/test_upload.py
--rw-r--r--   0        0        0      775 2023-04-18 14:25:32.635205 mantik-0.2.0/src/tests/unit/utils/conftest.py
--rw-r--r--   0        0        0      736 2023-04-18 14:25:32.635205 mantik-0.2.0/src/tests/unit/utils/test_env.py
--rw-r--r--   0        0        0      285 2023-04-18 14:25:32.635205 mantik-0.2.0/src/tests/unit/utils/test_temp_dir.py
--rw-r--r--   0        0        0      633 2023-04-18 14:25:32.635205 mantik-0.2.0/src/tests/unit/utils/test_urls.py
--rw-r--r--   0        0        0     2187 1970-01-01 00:00:00.000000 mantik-0.2.0/setup.py
--rw-r--r--   0        0        0     1984 1970-01-01 00:00:00.000000 mantik-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-07-07 10:18:58.040744 mantik-0.3.1/LICENSE
+-rw-r--r--   0        0        0      508 2023-07-07 10:18:58.040744 mantik-0.3.1/README.md
+-rw-r--r--   0        0        0     1997 2023-07-07 10:18:58.059744 mantik-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      251 2023-07-07 10:18:58.059744 mantik-0.3.1/src/mantik/__init__.py
+-rw-r--r--   0        0        0      103 2023-07-07 10:18:58.060745 mantik-0.3.1/src/mantik/authentication/__init__.py
+-rw-r--r--   0        0        0     1698 2023-07-07 10:18:58.060745 mantik-0.3.1/src/mantik/authentication/api.py
+-rw-r--r--   0        0        0     1386 2023-07-07 10:18:58.060745 mantik-0.3.1/src/mantik/authentication/auth.py
+-rw-r--r--   0        0        0     2265 2023-07-07 10:18:58.060745 mantik-0.3.1/src/mantik/authentication/tokens.py
+-rw-r--r--   0        0        0      107 2023-07-07 10:18:58.060745 mantik-0.3.1/src/mantik/cli/__init__.py
+-rw-r--r--   0        0        0     1257 2023-07-07 10:18:58.060745 mantik-0.3.1/src/mantik/cli/init.py
+-rw-r--r--   0        0        0       71 2023-07-07 10:18:58.060745 mantik-0.3.1/src/mantik/cli/main.py
+-rw-r--r--   0        0        0       59 2023-07-07 10:18:58.060745 mantik-0.3.1/src/mantik/cli/remote_file_service/__init__.py
+-rw-r--r--   0        0        0     3156 2023-07-07 10:18:58.060745 mantik-0.3.1/src/mantik/cli/remote_file_service/unicore_file_service.py
+-rw-r--r--   0        0        0      234 2023-07-07 10:18:58.060745 mantik-0.3.1/src/mantik/cli/runs/__init__.py
+-rw-r--r--   0        0        0       88 2023-07-07 10:18:58.060745 mantik-0.3.1/src/mantik/cli/runs/_arguments.py
+-rw-r--r--   0        0        0      659 2023-07-07 10:18:58.060745 mantik-0.3.1/src/mantik/cli/runs/_callbacks.py
+-rw-r--r--   0        0        0     1427 2023-07-07 10:18:58.060745 mantik-0.3.1/src/mantik/cli/runs/_options.py
+-rw-r--r--   0        0        0      723 2023-07-07 10:18:58.060745 mantik-0.3.1/src/mantik/cli/runs/cancel.py
+-rw-r--r--   0        0        0     1608 2023-07-07 10:18:58.060745 mantik-0.3.1/src/mantik/cli/runs/download.py
+-rw-r--r--   0        0        0     1153 2023-07-07 10:18:58.060745 mantik-0.3.1/src/mantik/cli/runs/info.py
+-rw-r--r--   0        0        0     2669 2023-07-07 10:18:58.060745 mantik-0.3.1/src/mantik/cli/runs/list.py
+-rw-r--r--   0        0        0      723 2023-07-07 10:18:58.060745 mantik-0.3.1/src/mantik/cli/runs/logs.py
+-rw-r--r--   0        0        0      116 2023-07-07 10:18:58.060745 mantik-0.3.1/src/mantik/cli/runs/runs.py
+-rw-r--r--   0        0        0      696 2023-07-07 10:18:58.060745 mantik-0.3.1/src/mantik/cli/runs/status.py
+-rw-r--r--   0        0        0     3026 2023-07-07 10:18:58.060745 mantik-0.3.1/src/mantik/cli/runs/submit.py
+-rw-r--r--   0        0        0      316 2023-07-07 10:18:58.060745 mantik-0.3.1/src/mantik/compute_backend_service/__init__.py
+-rw-r--r--   0        0        0     1739 2023-07-07 10:18:58.060745 mantik-0.3.1/src/mantik/compute_backend_service/_bearer.py
+-rw-r--r--   0        0        0     3486 2023-07-07 10:18:58.061745 mantik-0.3.1/src/mantik/compute_backend_service/api.py
+-rw-r--r--   0        0        0     1648 2023-07-07 10:18:58.061745 mantik-0.3.1/src/mantik/compute_backend_service/app.py
+-rw-r--r--   0        0        0     3251 2023-07-07 10:18:58.061745 mantik-0.3.1/src/mantik/compute_backend_service/backend.py
+-rw-r--r--   0        0        0     8072 2023-07-07 10:18:58.061745 mantik-0.3.1/src/mantik/compute_backend_service/client.py
+-rw-r--r--   0        0        0     3297 2023-07-07 10:18:58.061745 mantik-0.3.1/src/mantik/compute_backend_service/exceptions.py
+-rw-r--r--   0        0        0      324 2023-07-07 10:18:58.061745 mantik-0.3.1/src/mantik/compute_backend_service/models.py
+-rw-r--r--   0        0        0     1196 2023-07-07 10:18:58.061745 mantik-0.3.1/src/mantik/compute_backend_service/settings.py
+-rw-r--r--   0        0        0        0 2023-07-07 10:18:58.109745 mantik-0.3.1/src/mantik/mlflow_server/__init__.py
+-rw-r--r--   0        0        0      126 2023-07-07 10:18:58.061745 mantik-0.3.1/src/mantik/mlflow_server/flask/__init__.py
+-rw-r--r--   0        0        0     1379 2023-07-07 10:18:58.061745 mantik-0.3.1/src/mantik/mlflow_server/flask/_header.py
+-rw-r--r--   0        0        0       90 2023-07-07 10:18:58.061745 mantik-0.3.1/src/mantik/mlflow_server/flask/api/__init__.py
+-rw-r--r--   0        0        0       85 2023-07-07 10:18:58.061745 mantik-0.3.1/src/mantik/mlflow_server/flask/api/_exceptions.py
+-rw-r--r--   0        0        0     1339 2023-07-07 10:18:58.061745 mantik-0.3.1/src/mantik/mlflow_server/flask/api/_get.py
+-rw-r--r--   0        0        0      455 2023-07-07 10:18:58.061745 mantik-0.3.1/src/mantik/mlflow_server/flask/api/health.py
+-rw-r--r--   0        0        0      109 2023-07-07 10:18:58.061745 mantik-0.3.1/src/mantik/mlflow_server/flask/api/models/__init__.py
+-rw-r--r--   0        0        0     1328 2023-07-07 10:18:58.061745 mantik-0.3.1/src/mantik/mlflow_server/flask/api/models/requests.py
+-rw-r--r--   0        0        0     1342 2023-07-07 10:18:58.061745 mantik-0.3.1/src/mantik/mlflow_server/flask/api/models/responses.py
+-rw-r--r--   0        0        0     1871 2023-07-07 10:18:58.061745 mantik-0.3.1/src/mantik/mlflow_server/flask/api/tokens.py
+-rw-r--r--   0        0        0       46 2023-07-07 10:18:58.061745 mantik-0.3.1/src/mantik/mlflow_server/flask/app.py
+-rw-r--r--   0        0        0     1829 2023-07-07 10:18:58.061745 mantik-0.3.1/src/mantik/mlflow_server/flask/before_requests.py
+-rw-r--r--   0        0        0      722 2023-07-07 10:18:58.061745 mantik-0.3.1/src/mantik/mlflow_server/flask/skip.py
+-rw-r--r--   0        0        0       41 2023-07-07 10:18:58.062744 mantik-0.3.1/src/mantik/mlflow_server/gunicorn/__init__.py
+-rw-r--r--   0        0        0     1278 2023-07-07 10:18:58.062744 mantik-0.3.1/src/mantik/mlflow_server/gunicorn/_app.py
+-rw-r--r--   0        0        0      882 2023-07-07 10:18:58.062744 mantik-0.3.1/src/mantik/mlflow_server/gunicorn/_cli_args.py
+-rw-r--r--   0        0        0      614 2023-07-07 10:18:58.062744 mantik-0.3.1/src/mantik/mlflow_server/gunicorn/_env.py
+-rw-r--r--   0        0        0      596 2023-07-07 10:18:58.062744 mantik-0.3.1/src/mantik/mlflow_server/gunicorn/_options.py
+-rw-r--r--   0        0        0      961 2023-07-07 10:18:58.062744 mantik-0.3.1/src/mantik/mlflow_server/gunicorn/_stores.py
+-rw-r--r--   0        0        0      610 2023-07-07 10:18:58.062744 mantik-0.3.1/src/mantik/mlflow_server/gunicorn/run.py
+-rw-r--r--   0        0        0      212 2023-07-07 10:18:58.062744 mantik-0.3.1/src/mantik/mlflow_server/tokens/__init__.py
+-rw-r--r--   0        0        0      256 2023-07-07 10:18:58.062744 mantik-0.3.1/src/mantik/mlflow_server/tokens/cognito/__init__.py
+-rw-r--r--   0        0        0     3612 2023-07-07 10:18:58.062744 mantik-0.3.1/src/mantik/mlflow_server/tokens/cognito/_auth.py
+-rw-r--r--   0        0        0     1532 2023-07-07 10:18:58.062744 mantik-0.3.1/src/mantik/mlflow_server/tokens/cognito/api.py
+-rw-r--r--   0        0        0     2053 2023-07-07 10:18:58.062744 mantik-0.3.1/src/mantik/mlflow_server/tokens/cognito/client.py
+-rw-r--r--   0        0        0     1659 2023-07-07 10:18:58.062744 mantik-0.3.1/src/mantik/mlflow_server/tokens/cognito/credentials.py
+-rw-r--r--   0        0        0      218 2023-07-07 10:18:58.062744 mantik-0.3.1/src/mantik/mlflow_server/tokens/cognito/exceptions.py
+-rw-r--r--   0        0        0     1250 2023-07-07 10:18:58.062744 mantik-0.3.1/src/mantik/mlflow_server/tokens/cognito/tokens.py
+-rw-r--r--   0        0        0      604 2023-07-07 10:18:58.062744 mantik-0.3.1/src/mantik/mlflow_server/tokens/exceptions.py
+-rw-r--r--   0        0        0     2127 2023-07-07 10:18:58.062744 mantik-0.3.1/src/mantik/mlflow_server/tokens/jwks.py
+-rw-r--r--   0        0        0     3248 2023-07-07 10:18:58.062744 mantik-0.3.1/src/mantik/mlflow_server/tokens/jwt.py
+-rw-r--r--   0        0        0     3688 2023-07-07 10:18:58.062744 mantik-0.3.1/src/mantik/mlflow_server/tokens/verifier.py
+-rw-r--r--   0        0        0        0 2023-07-07 10:18:58.111745 mantik-0.3.1/src/mantik/py.typed
+-rw-r--r--   0        0        0       56 2023-07-07 10:18:58.062744 mantik-0.3.1/src/mantik/remote_file_service/__init__.py
+-rw-r--r--   0        0        0     2540 2023-07-07 10:18:58.062744 mantik-0.3.1/src/mantik/remote_file_service/abstract_file_service.py
+-rw-r--r--   0        0        0     7817 2023-07-07 10:18:58.063745 mantik-0.3.1/src/mantik/remote_file_service/data_client.py
+-rw-r--r--   0        0        0     9020 2023-07-07 10:18:58.063745 mantik-0.3.1/src/mantik/remote_file_service/unicore_file_service.py
+-rw-r--r--   0        0        0      285 2023-07-07 10:18:58.063745 mantik-0.3.1/src/mantik/testing/__init__.py
+-rw-r--r--   0        0        0     8518 2023-07-07 10:18:58.063745 mantik-0.3.1/src/mantik/testing/cognito.py
+-rw-r--r--   0        0        0     2438 2023-07-07 10:18:58.063745 mantik-0.3.1/src/mantik/testing/config.py
+-rw-r--r--   0        0        0      601 2023-07-07 10:18:58.063745 mantik-0.3.1/src/mantik/testing/contexts.py
+-rw-r--r--   0        0        0     1274 2023-07-07 10:18:58.063745 mantik-0.3.1/src/mantik/testing/env.py
+-rw-r--r--   0        0        0    12408 2023-07-07 10:18:58.063745 mantik-0.3.1/src/mantik/testing/mlflow_server.py
+-rw-r--r--   0        0        0     6725 2023-07-07 10:18:58.063745 mantik-0.3.1/src/mantik/testing/pyunicore.py
+-rw-r--r--   0        0        0     2061 2023-07-07 10:18:58.063745 mantik-0.3.1/src/mantik/testing/remote_file_service.py
+-rw-r--r--   0        0        0      927 2023-07-07 10:18:58.063745 mantik-0.3.1/src/mantik/testing/requests.py
+-rw-r--r--   0        0        0     1111 2023-07-07 10:18:58.063745 mantik-0.3.1/src/mantik/testing/token.py
+-rw-r--r--   0        0        0       29 2023-07-07 10:18:58.063745 mantik-0.3.1/src/mantik/tracking/__init__.py
+-rw-r--r--   0        0        0      920 2023-07-07 10:18:58.063745 mantik-0.3.1/src/mantik/tracking/environment.py
+-rw-r--r--   0        0        0     1108 2023-07-07 10:18:58.063745 mantik-0.3.1/src/mantik/tracking/track.py
+-rw-r--r--   0        0        0      250 2023-07-07 10:18:58.063745 mantik-0.3.1/src/mantik/unicore/__init__.py
+-rw-r--r--   0        0        0     2799 2023-07-07 10:18:58.063745 mantik-0.3.1/src/mantik/unicore/_connect.py
+-rw-r--r--   0        0        0     7949 2023-07-07 10:18:58.063745 mantik-0.3.1/src/mantik/unicore/backend.py
+-rw-r--r--   0        0        0     3190 2023-07-07 10:18:58.063745 mantik-0.3.1/src/mantik/unicore/client.py
+-rw-r--r--   0        0        0      226 2023-07-07 10:18:58.064745 mantik-0.3.1/src/mantik/unicore/config/__init__.py
+-rw-r--r--   0        0        0      535 2023-07-07 10:18:58.064745 mantik-0.3.1/src/mantik/unicore/config/_base.py
+-rw-r--r--   0        0        0     2776 2023-07-07 10:18:58.064745 mantik-0.3.1/src/mantik/unicore/config/_utils.py
+-rw-r--r--   0        0        0     4489 2023-07-07 10:18:58.064745 mantik-0.3.1/src/mantik/unicore/config/core.py
+-rw-r--r--   0        0        0     2876 2023-07-07 10:18:58.064745 mantik-0.3.1/src/mantik/unicore/config/environment.py
+-rw-r--r--   0        0        0     7484 2023-07-07 10:18:58.064745 mantik-0.3.1/src/mantik/unicore/config/executable.py
+-rw-r--r--   0        0        0     1072 2023-07-07 10:18:58.064745 mantik-0.3.1/src/mantik/unicore/config/read.py
+-rw-r--r--   0        0        0     2739 2023-07-07 10:18:58.064745 mantik-0.3.1/src/mantik/unicore/config/resources.py
+-rw-r--r--   0        0        0     3895 2023-07-07 10:18:58.064745 mantik-0.3.1/src/mantik/unicore/config/validate.py
+-rw-r--r--   0        0        0      542 2023-07-07 10:18:58.064745 mantik-0.3.1/src/mantik/unicore/exceptions.py
+-rw-r--r--   0        0        0     3458 2023-07-07 10:18:58.064745 mantik-0.3.1/src/mantik/unicore/job.py
+-rw-r--r--   0        0        0     5644 2023-07-07 10:18:58.064745 mantik-0.3.1/src/mantik/unicore/properties.py
+-rw-r--r--   0        0        0     2946 2023-07-07 10:18:58.064745 mantik-0.3.1/src/mantik/unicore/submitted_run.py
+-rw-r--r--   0        0        0       67 2023-07-07 10:18:58.064745 mantik-0.3.1/src/mantik/unicore/utils/__init__.py
+-rw-r--r--   0        0        0     1997 2023-07-07 10:18:58.064745 mantik-0.3.1/src/mantik/unicore/utils/upload.py
+-rw-r--r--   0        0        0      763 2023-07-07 10:18:58.064745 mantik-0.3.1/src/mantik/unicore/utils/zip.py
+-rw-r--r--   0        0        0     4054 2023-07-07 10:18:58.064745 mantik-0.3.1/src/mantik/unicore/working_dir.py
+-rw-r--r--   0        0        0      136 2023-07-07 10:18:58.064745 mantik-0.3.1/src/mantik/utils/__init__.py
+-rw-r--r--   0        0        0     2151 2023-07-07 10:18:58.064745 mantik-0.3.1/src/mantik/utils/env.py
+-rw-r--r--   0        0        0       38 2023-07-07 10:18:58.064745 mantik-0.3.1/src/mantik/utils/mantik_api/__init__.py
+-rw-r--r--   0        0        0     3685 2023-07-07 10:18:58.064745 mantik-0.3.1/src/mantik/utils/mantik_api/client.py
+-rw-r--r--   0        0        0     1259 2023-07-07 10:18:58.064745 mantik-0.3.1/src/mantik/utils/mantik_api/credentials.py
+-rw-r--r--   0        0        0     1054 2023-07-07 10:18:58.065744 mantik-0.3.1/src/mantik/utils/mantik_api/data_repository.py
+-rw-r--r--   0        0        0      471 2023-07-07 10:18:58.065744 mantik-0.3.1/src/mantik/utils/mlflow.py
+-rw-r--r--   0        0        0      615 2023-07-07 10:18:58.065744 mantik-0.3.1/src/mantik/utils/temp_dir.py
+-rw-r--r--   0        0        0      320 2023-07-07 10:18:58.065744 mantik-0.3.1/src/mantik/utils/urls.py
+-rw-r--r--   0        0        0      163 2023-07-07 10:18:58.065744 mantik-0.3.1/src/tests/resources/broken-project/MLproject
+-rw-r--r--   0        0        0       77 2023-07-07 10:18:58.065744 mantik-0.3.1/src/tests/resources/broken-project/README.md
+-rw-r--r--   0        0        0      248 2023-07-07 10:18:58.065744 mantik-0.3.1/src/tests/resources/broken-project/unicore-config.md
+-rw-r--r--   0        0        0      574 2023-07-07 10:18:58.065744 mantik-0.3.1/src/tests/resources/cognito/auth-response.json
+-rw-r--r--   0        0        0      159 2023-07-07 10:18:58.065744 mantik-0.3.1/src/tests/resources/cognito/different-client.json
+-rw-r--r--   0        0        0      649 2023-07-07 10:18:58.065744 mantik-0.3.1/src/tests/resources/cognito/incorrect-login-credentials-response.json
+-rw-r--r--   0        0        0      578 2023-07-07 10:18:58.065744 mantik-0.3.1/src/tests/resources/cognito/refresh-response.json
+-rw-r--r--   0        0        0      631 2023-07-07 10:18:58.065744 mantik-0.3.1/src/tests/resources/cognito/refresh-token-expired-response.json
+-rw-r--r--   0        0        0      623 2023-07-07 10:18:58.065744 mantik-0.3.1/src/tests/resources/cognito/refresh-token-invalid-response.json
+-rw-r--r--   0        0        0      614 2023-07-07 10:18:58.065744 mantik-0.3.1/src/tests/resources/cognito/user-not-found-response.json
+-rw-r--r--   0        0        0       57 2023-07-07 10:18:58.065744 mantik-0.3.1/src/tests/resources/test-project/Dockerfile
+-rw-r--r--   0        0        0      182 2023-07-07 10:18:58.065744 mantik-0.3.1/src/tests/resources/test-project/MLproject
+-rw-r--r--   0        0        0      168 2023-07-07 10:18:58.065744 mantik-0.3.1/src/tests/resources/test-project/config-with-errors.yaml
+-rw-r--r--   0        0        0      536 2023-07-07 10:18:58.065744 mantik-0.3.1/src/tests/resources/test-project/main.py
+-rw-r--r--   0        0        0        0 2023-07-07 10:18:58.118746 mantik-0.3.1/src/tests/resources/test-project/mantik-test.sif
+-rw-r--r--   0        0        0       50 2023-07-07 10:18:58.065744 mantik-0.3.1/src/tests/resources/test-project/recipe.def
+-rw-r--r--   0        0        0        0 2023-07-07 10:18:58.118746 mantik-0.3.1/src/tests/resources/test-project/test_subfolder/test.py
+-rw-r--r--   0        0        0      246 2023-07-07 10:18:58.065744 mantik-0.3.1/src/tests/resources/test-project/unicore-config.json
+-rw-r--r--   0        0        0      193 2023-07-07 10:18:58.065744 mantik-0.3.1/src/tests/resources/test-project/unicore-config.yaml
+-rw-r--r--   0        0        0     2879 2023-07-07 10:18:58.065744 mantik-0.3.1/src/tests/resources/unicore-responses/job-property-response.json
+-rw-r--r--   0        0        0     1837 2023-07-07 10:18:58.066745 mantik-0.3.1/src/tests/unit/athentication/test_credentials.py
+-rw-r--r--   0        0        0     2391 2023-07-07 10:18:58.066745 mantik-0.3.1/src/tests/unit/athentication/test_server_api.py
+-rw-r--r--   0        0        0     1121 2023-07-07 10:18:58.066745 mantik-0.3.1/src/tests/unit/athentication/test_tokens.py
+-rw-r--r--   0        0        0      193 2023-07-07 10:18:58.066745 mantik-0.3.1/src/tests/unit/cli/conftest.py
+-rw-r--r--   0        0        0     4338 2023-07-07 10:18:58.066745 mantik-0.3.1/src/tests/unit/cli/remote_file_service/test_unicore_file_service.py
+-rw-r--r--   0        0        0      537 2023-07-07 10:18:58.066745 mantik-0.3.1/src/tests/unit/cli/runs/conftest.py
+-rw-r--r--   0        0        0      555 2023-07-07 10:18:58.066745 mantik-0.3.1/src/tests/unit/cli/runs/test_cancel.py
+-rw-r--r--   0        0        0     3201 2023-07-07 10:18:58.066745 mantik-0.3.1/src/tests/unit/cli/runs/test_download.py
+-rw-r--r--   0        0        0     3506 2023-07-07 10:18:58.066745 mantik-0.3.1/src/tests/unit/cli/runs/test_info.py
+-rw-r--r--   0        0        0      831 2023-07-07 10:18:58.066745 mantik-0.3.1/src/tests/unit/cli/runs/test_list.py
+-rw-r--r--   0        0        0     1564 2023-07-07 10:18:58.066745 mantik-0.3.1/src/tests/unit/cli/runs/test_logs.py
+-rw-r--r--   0        0        0      823 2023-07-07 10:18:58.066745 mantik-0.3.1/src/tests/unit/cli/runs/test_options.py
+-rw-r--r--   0        0        0     1560 2023-07-07 10:18:58.066745 mantik-0.3.1/src/tests/unit/cli/runs/test_status.py
+-rw-r--r--   0        0        0     5433 2023-07-07 10:18:58.066745 mantik-0.3.1/src/tests/unit/cli/runs/test_submit.py
+-rw-r--r--   0        0        0      780 2023-07-07 10:18:58.066745 mantik-0.3.1/src/tests/unit/cli/test_init.py
+-rw-r--r--   0        0        0     3920 2023-07-07 10:18:58.066745 mantik-0.3.1/src/tests/unit/compute_backend_service/conftest.py
+-rw-r--r--   0        0        0     5719 2023-07-07 10:18:58.066745 mantik-0.3.1/src/tests/unit/compute_backend_service/test_api.py
+-rw-r--r--   0        0        0      738 2023-07-07 10:18:58.067745 mantik-0.3.1/src/tests/unit/compute_backend_service/test_app.py
+-rw-r--r--   0        0        0     3175 2023-07-07 10:18:58.067745 mantik-0.3.1/src/tests/unit/compute_backend_service/test_client.py
+-rw-r--r--   0        0        0     1202 2023-07-07 10:18:58.067745 mantik-0.3.1/src/tests/unit/compute_backend_service/test_compute_backend.py
+-rw-r--r--   0        0        0     8711 2023-07-07 10:18:58.067745 mantik-0.3.1/src/tests/unit/compute_backend_service/test_exception_handler.py
+-rw-r--r--   0        0        0      327 2023-07-07 10:18:58.067745 mantik-0.3.1/src/tests/unit/compute_backend_service/test_models.py
+-rw-r--r--   0        0        0     3525 2023-07-07 10:18:58.067745 mantik-0.3.1/src/tests/unit/conftest.py
+-rw-r--r--   0        0        0     1585 2023-07-07 10:18:58.067745 mantik-0.3.1/src/tests/unit/mlflow_server/conftest.py
+-rw-r--r--   0        0        0      191 2023-07-07 10:18:58.067745 mantik-0.3.1/src/tests/unit/mlflow_server/flask/api/test_health_api.py
+-rw-r--r--   0        0        0     4375 2023-07-07 10:18:58.067745 mantik-0.3.1/src/tests/unit/mlflow_server/flask/api/test_tokens_api.py
+-rw-r--r--   0        0        0      607 2023-07-07 10:18:58.067745 mantik-0.3.1/src/tests/unit/mlflow_server/flask/conftest.py
+-rw-r--r--   0        0        0     1126 2023-07-07 10:18:58.067745 mantik-0.3.1/src/tests/unit/mlflow_server/flask/test_flask_app.py
+-rw-r--r--   0        0        0      469 2023-07-07 10:18:58.067745 mantik-0.3.1/src/tests/unit/mlflow_server/flask/test_skip.py
+-rw-r--r--   0        0        0      391 2023-07-07 10:18:58.067745 mantik-0.3.1/src/tests/unit/mlflow_server/gunicorn/test_run.py
+-rw-r--r--   0        0        0     4139 2023-07-07 10:18:58.067745 mantik-0.3.1/src/tests/unit/mlflow_server/tokens/cognito/test_auth.py
+-rw-r--r--   0        0        0     2807 2023-07-07 10:18:58.067745 mantik-0.3.1/src/tests/unit/mlflow_server/tokens/test_verifier.py
+-rw-r--r--   0        0        0     1479 2023-07-07 10:18:58.067745 mantik-0.3.1/src/tests/unit/remote_file_service/conftest.py
+-rw-r--r--   0        0        0    10246 2023-07-07 10:18:58.067745 mantik-0.3.1/src/tests/unit/remote_file_service/test_data_client.py
+-rw-r--r--   0        0        0     5655 2023-07-07 10:18:58.067745 mantik-0.3.1/src/tests/unit/tracking/test_track.py
+-rw-r--r--   0        0        0     1211 2023-07-07 10:18:58.068745 mantik-0.3.1/src/tests/unit/unicore/config/conftest.py
+-rw-r--r--   0        0        0    10081 2023-07-07 10:18:58.068745 mantik-0.3.1/src/tests/unit/unicore/config/test_core.py
+-rw-r--r--   0        0        0     3136 2023-07-07 10:18:58.068745 mantik-0.3.1/src/tests/unit/unicore/config/test_environment.py
+-rw-r--r--   0        0        0     1765 2023-07-07 10:18:58.068745 mantik-0.3.1/src/tests/unit/unicore/config/test_executable.py
+-rw-r--r--   0        0        0     1945 2023-07-07 10:18:58.068745 mantik-0.3.1/src/tests/unit/unicore/config/test_read.py
+-rw-r--r--   0        0        0     2981 2023-07-07 10:18:58.068745 mantik-0.3.1/src/tests/unit/unicore/config/test_utils.py
+-rw-r--r--   0        0        0     8372 2023-07-07 10:18:58.068745 mantik-0.3.1/src/tests/unit/unicore/config/test_validate.py
+-rw-r--r--   0        0        0     2681 2023-07-07 10:18:58.068745 mantik-0.3.1/src/tests/unit/unicore/conftest.py
+-rw-r--r--   0        0        0     5025 2023-07-07 10:18:58.068745 mantik-0.3.1/src/tests/unit/unicore/test_backend.py
+-rw-r--r--   0        0        0     1231 2023-07-07 10:18:58.068745 mantik-0.3.1/src/tests/unit/unicore/test_client_wrapper.py
+-rw-r--r--   0        0        0     1870 2023-07-07 10:18:58.068745 mantik-0.3.1/src/tests/unit/unicore/test_connect.py
+-rw-r--r--   0        0        0      516 2023-07-07 10:18:58.068745 mantik-0.3.1/src/tests/unit/unicore/test_exceptions.py
+-rw-r--r--   0        0        0     1551 2023-07-07 10:18:58.068745 mantik-0.3.1/src/tests/unit/unicore/test_properties.py
+-rw-r--r--   0        0        0     3707 2023-07-07 10:18:58.068745 mantik-0.3.1/src/tests/unit/unicore/test_submitted_run.py
+-rw-r--r--   0        0        0     4240 2023-07-07 10:18:58.068745 mantik-0.3.1/src/tests/unit/unicore/utils/test_upload.py
+-rw-r--r--   0        0        0      775 2023-07-07 10:18:58.068745 mantik-0.3.1/src/tests/unit/utils/conftest.py
+-rw-r--r--   0        0        0     3577 2023-07-07 10:18:58.068745 mantik-0.3.1/src/tests/unit/utils/mantik_api/test_mantik_api.py
+-rw-r--r--   0        0        0      736 2023-07-07 10:18:58.068745 mantik-0.3.1/src/tests/unit/utils/test_env.py
+-rw-r--r--   0        0        0      285 2023-07-07 10:18:58.068745 mantik-0.3.1/src/tests/unit/utils/test_temp_dir.py
+-rw-r--r--   0        0        0      633 2023-07-07 10:18:58.069745 mantik-0.3.1/src/tests/unit/utils/test_urls.py
+-rw-r--r--   0        0        0     2053 1970-01-01 00:00:00.000000 mantik-0.3.1/PKG-INFO
```

### Comparing `mantik-0.2.0/LICENSE` & `mantik-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/pyproject.toml` & `mantik-0.3.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mantik"
-version = "0.2.0"
+version = "0.3.1"
 description = "mantik for mlflow"
 authors = [
     "Fabian Emmerich <fabian.emmerich@4-cast.de>",
     "Thomas Seidler <thomas.seidler@ambrosys.de>",
 ]
 maintainers = [
     "Elia Boscaini <elia.boscaini@ambrosys.de>",
@@ -32,34 +32,35 @@
 
 [tool.poetry.plugins."mlflow.project_backend"]
 "unicore" = "mantik.unicore.backend:UnicoreBackend"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 mlflow = "2.2.2"
-pyunicore = "^0.9.16"
+pyunicore = {extras = ["crypto", "fs", "fuse"], version = "^0.15.0"}
 fastapi = "^0.78.0"
 requests = "^2.27.1"
 pydantic = "^1.9.0"
 python-multipart = "^0.0.5"
 uvicorn = {extras = ["standard"], version = "^0.17.6"}
 boto3 = "^1.23.6"
 Flask = "^2.1.2"
 python-jose = "^3.3.0"
 click = "^8.1.3"
 PyYAML = "^6.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
-pytest-cov = "^3.0.0"
+pytest-cov = "^4.0.0"
 pre-commit = "^2.17.0"
 fastapi = {extras = ["testclient"], version = "^0.78.0"}
 freezegun = "^1.2.1"
-requests-mock = "^1.9.3"
 pytest-custom-exit-code = "^0.3.0"
+requests-mock = "^1.11.0"
+pytest-mock = "^3.11.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 addopts = "--cov=mantik --cov-report term-missing"
```

### Comparing `mantik-0.2.0/src/mantik/cli/init.py` & `mantik-0.3.1/src/mantik/cli/init.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,21 +9,22 @@
     "--no-export",
     is_flag=True,
     show_default=True,
     default=False,
     help="Strip the `export` prefix of the output.",
 )
 def initialize_tracking(no_export: bool) -> None:
-    """Initialize the tracking to mantik and print the required environment
-    variables.
+    """Initialize the authentication to mantik and
+    print the required environment variables.
 
     It is not possible to set environment variables in a parent process
     (or shell) from a subprocess (e.g. Python). Thus, the `init` command prints
     the bash export statement with the required environment variable for
-    tracking to mantik. As a consequence, the output can be directly used to set
+    authentication to mantik.
+    As a consequence, the output can be directly used to set
     the environment variable in the parent process by using the `eval` bash
     command:
 
     \b
     ```shell
     eval $(mantik init)
     ```
```

### Comparing `mantik-0.2.0/src/mantik/cli/runs/_callbacks.py` & `mantik-0.3.1/src/mantik/cli/runs/_callbacks.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/cli/runs/_options.py` & `mantik-0.3.1/src/mantik/cli/runs/_options.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/cli/runs/cancel.py` & `mantik-0.3.1/src/mantik/cli/runs/cancel.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/cli/runs/download.py` & `mantik-0.3.1/src/mantik/cli/runs/download.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/cli/runs/info.py` & `mantik-0.3.1/src/mantik/cli/runs/info.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/cli/runs/list.py` & `mantik-0.3.1/src/mantik/cli/runs/list.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/cli/runs/logs.py` & `mantik-0.3.1/src/mantik/cli/runs/logs.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/cli/runs/status.py` & `mantik-0.3.1/src/mantik/cli/runs/status.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/cli/runs/submit.py` & `mantik-0.3.1/src/mantik/cli/runs/submit.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/compute_backend_service/_bearer.py` & `mantik-0.3.1/src/mantik/compute_backend_service/_bearer.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/compute_backend_service/api.py` & `mantik-0.3.1/src/mantik/compute_backend_service/api.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/compute_backend_service/app.py` & `mantik-0.3.1/src/mantik/compute_backend_service/app.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/compute_backend_service/backend.py` & `mantik-0.3.1/src/mantik/compute_backend_service/backend.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/compute_backend_service/client.py` & `mantik-0.3.1/src/mantik/compute_backend_service/client.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/compute_backend_service/exceptions.py` & `mantik-0.3.1/src/mantik/compute_backend_service/exceptions.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/compute_backend_service/settings.py` & `mantik-0.3.1/src/mantik/compute_backend_service/settings.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/mlflow_server/flask/api/_get.py` & `mantik-0.3.1/src/mantik/mlflow_server/flask/api/_get.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/mlflow_server/flask/api/models/requests.py` & `mantik-0.3.1/src/mantik/mlflow_server/flask/api/models/requests.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/mlflow_server/flask/api/models/responses.py` & `mantik-0.3.1/src/mantik/mlflow_server/flask/api/models/responses.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/mlflow_server/flask/api/tokens.py` & `mantik-0.3.1/src/mantik/mlflow_server/flask/api/tokens.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/mlflow_server/flask/before_requests.py` & `mantik-0.3.1/src/mantik/mlflow_server/flask/before_requests.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     """
     if _skip_authentication(flask.request):
         return
 
     try:
         _verify_token(flask.request)
     except AuthenticationFailedException as e:
-        logger.exception(
+        logger.debug(
             "Token in request headers %s is not valid",
             flask.request.headers,
             exc_info=True,
         )
         return flask.make_response(str(e), 401)
     return
 
@@ -60,10 +60,11 @@
 def _verify_token(request: flask.Request) -> None:
     verifier = tokens.verifier.TokenVerifier(secret_required=True)
     try:
         token = _header.get_authorization_token(request)
         verifier.verify_token(token)
     except (
         _header.MissingAuthorizationHeaderException,
+        _header.EmptyTokenException,
         tokens.exceptions.VerificationFailedException,
     ) as e:
         raise AuthenticationFailedException(str(e))
```

### Comparing `mantik-0.2.0/src/mantik/mlflow_server/flask/skip.py` & `mantik-0.3.1/src/mantik/mlflow_server/flask/skip.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/mlflow_server/gunicorn/_app.py` & `mantik-0.3.1/src/mantik/mlflow_server/gunicorn/_app.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/mlflow_server/gunicorn/_cli_args.py` & `mantik-0.3.1/src/mantik/mlflow_server/gunicorn/_cli_args.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/mlflow_server/gunicorn/_env.py` & `mantik-0.3.1/src/mantik/mlflow_server/gunicorn/_env.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/mlflow_server/gunicorn/_stores.py` & `mantik-0.3.1/src/mantik/mlflow_server/gunicorn/_stores.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/mlflow_server/tokens/cognito/_auth.py` & `mantik-0.3.1/src/mantik/mlflow_server/tokens/cognito/_auth.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/mlflow_server/tokens/cognito/api.py` & `mantik-0.3.1/src/mantik/mlflow_server/tokens/cognito/api.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/mlflow_server/tokens/cognito/client.py` & `mantik-0.3.1/src/mantik/mlflow_server/tokens/cognito/client.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/mlflow_server/tokens/cognito/credentials.py` & `mantik-0.3.1/src/mantik/mlflow_server/tokens/cognito/credentials.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/mlflow_server/tokens/cognito/tokens.py` & `mantik-0.3.1/src/mantik/mlflow_server/tokens/cognito/tokens.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/mlflow_server/tokens/exceptions.py` & `mantik-0.3.1/src/mantik/mlflow_server/tokens/exceptions.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/mlflow_server/tokens/jwks.py` & `mantik-0.3.1/src/mantik/mlflow_server/tokens/jwks.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/mlflow_server/tokens/jwt.py` & `mantik-0.3.1/src/mantik/mlflow_server/tokens/jwt.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/mlflow_server/tokens/verifier.py` & `mantik-0.3.1/src/mantik/mlflow_server/tokens/verifier.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/testing/cognito.py` & `mantik-0.3.1/src/mantik/testing/cognito.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/testing/config.py` & `mantik-0.3.1/src/mantik/testing/config.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/testing/contexts.py` & `mantik-0.3.1/src/mantik/testing/contexts.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/testing/env.py` & `mantik-0.3.1/src/mantik/testing/env.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,31 +13,35 @@
         Name of the variable.
     expected_value : str or None
         Expected value.
 
     Raises
     ------
     AssertionError
-        If given environment variable does not have the expected value.
+        If given environment variable
+        does not have the expected value.
 
     """
     value = os.environ.get(key, None)
     assert value == expected_value
 
 
 def assert_conflicting_mlflow_env_vars_not_set() -> None:
-    """Assert that the conflicting environemnt variables of mlflow are not set.
+    """
+    Assert that the conflicting environemnt variables of mlflow are not set.
 
     If `MLFLOW_TRACKING_USERNAME` or `MLFLOW_TRACKING_PASSWORD` are set, they
     are preferred by mlflow over `MLFLOW_TRACKING_TOKEN`, and thus, prevent
     the tracking from succeeding.
 
     """
     assert os.getenv(utils.mlflow.TRACKING_USERNAME_ENV_VAR) is None
     assert os.getenv(utils.mlflow.TRACKING_PASSWORD_ENV_VAR) is None
 
 
 def assert_correct_tracking_token_env_var_set(expected_access_token) -> None:
-    """Assert that the correct tracking token environment variable is set."""
+    """
+    Assert that the correct tracking token environment variable is set.
+    """
     assert (
         os.getenv(utils.mlflow.TRACKING_TOKEN_ENV_VAR) == expected_access_token
     )
```

### Comparing `mantik-0.2.0/src/mantik/testing/mlflow_server.py` & `mantik-0.3.1/src/mantik/testing/mlflow_server.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/testing/pyunicore.py` & `mantik-0.3.1/src/mantik/testing/pyunicore.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 import mantik.unicore as unicore
 import mantik.unicore.job as job_wrapper
 import mantik.unicore.properties as properties_wrapper
 import mantik.unicore.submitted_run as submitted_run
 
 
 class FakeTransport:
-    def __init__(self, auth_token: str = "test_token", oidc: bool = True):
-        self.auth_token = auth_token
+    def __init__(self, credential: str = "test_token", oidc: bool = True):
+        self.credential = credential
         self.oidc = oidc
 
 
 class FakeJob:
     def __init__(
         self,
         transport: FakeTransport,
```

### Comparing `mantik-0.2.0/src/mantik/testing/requests.py` & `mantik-0.3.1/src/mantik/testing/requests.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/tracking/_server/_credentials.py` & `mantik-0.3.1/src/mantik/utils/mantik_api/credentials.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/tracking/_server/api.py` & `mantik-0.3.1/src/mantik/utils/mantik_api/client.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,112 +1,125 @@
+import logging
+import os
 import typing as t
+import uuid
 
 import requests
 
-import mantik.mlflow_server.flask.api as _api
-import mantik.mlflow_server.tokens.cognito.exceptions as exceptions
-import mantik.tracking._server._credentials as _credentials
-import mantik.tracking._server.tokens as _tokens
-import mantik.utils as utils
+import mantik.utils.mantik_api.credentials as credentials
+import mantik.utils.mantik_api.data_repository as data_repository
 
+MANTIK_API_URL_ENV_VAR = "MANTIK_API_URL"
+MANTIK_API_URL = "https://api.cloud.mantik.ai"
 
-def create_tokens(
-    credentials: t.Optional[_credentials.Credentials] = None,
-) -> _tokens.Tokens:
-    """Get the required tokens from the Cognito API.
-
-    Raises
-    ------
-    RuntimeError
-        If MLflow tracking URI environment variable is not set.
-
-    """
-    if credentials is None:
-        credentials = _credentials.Credentials.from_env()
-    return _get_tokens(
-        url=_create_api_url(_api.tokens.CREATE_TOKEN_API_PATH),
-        data=credentials.to_dict(),
+_TOKENS_API_PATH_PREFIX = "/mantik-api/mantik/tokens"
+MANTIK_API_CREATE_TOKEN_API_PATH = f"{_TOKENS_API_PATH_PREFIX}/create"
+MANTIK_API_REFRESH_TOKEN_API_PATH = f"{_TOKENS_API_PATH_PREFIX}/refresh"
+
+logger = logging.getLogger(__name__)
+
+
+def create_data_repository(
+    add_data_repository: data_repository.AddDataRepositoryModel,
+    project_id: uuid.UUID,
+    token: str,
+):
+    data = add_data_repository.to_dict()
+    endpoint = f"/mantik-api/projects/{str(project_id)}/data"
+    response = _send_request_to_mantik_api("POST", data, endpoint, token)
+    logger.info(
+        f'A new data repository with id: {response.json()["dataRepositoryId"]} '
+        f"and name: {add_data_repository.data_repository_name} at "
+        f"{add_data_repository.uri} has been created"
     )
 
 
-def refresh_tokens(
-    tokens: _tokens.Tokens,
-    credentials: t.Optional[_credentials.Credentials] = None,
-) -> _tokens.Tokens:
-    """Refresh the tokens.
-
-    Raises
-    ------
-    RuntimeError
-        If MLflow tracking URI environment variable is not set.
-
-    Notes
-    -----
-    Refreshing a password requires to send the refresh token instead of the
-    user's password.
-
-    """
-    if credentials is None:
-        credentials = _credentials.Credentials.from_env()
-    data = {
-        **credentials.to_dict(include_password=False),
-        "refresh_token": tokens.refresh_token,
-    }
-    try:
-        return _get_tokens(
-            url=_create_api_url(_api.tokens.REFRESH_TOKEN_API_PATH),
-            data=data,
-            refresh_token=tokens.refresh_token,
-        )
-    except requests.HTTPError as e:
-        if _refresh_token_has_expired(e) or _refresh_token_is_invalid(e):
-            return create_tokens(credentials)
-        raise e
+def delete_data_repository(
+    project_id: uuid.UUID,
+    data_repository_id: uuid.UUID,
+    token: str,
+):
+    data = {}
+    endpoint = (
+        f"/mantik-api/projects/{str(project_id)}/data/{str(data_repository_id)}"
+    )
+    _send_request_to_mantik_api("DELETE", data, endpoint, token)
+    logger.info(
+        f"Data repository with id: {data_repository_id} has been deleted"
+    )
 
 
-def _refresh_token_has_expired(e: requests.HTTPError) -> bool:
-    return (
-        e.response.status_code == 401
-        and exceptions.REFRESH_TOKEN_EXPIRED_ERROR_MESSAGE in e.response.text
-    )
+def get_data_repositories(
+    project_id: uuid.UUID,
+    token: str,
+) -> t.List[t.Dict]:
+    endpoint = f"/mantik-api/projects/{str(project_id)}/data"
+    response = _send_request_to_mantik_api("GET", {}, endpoint, token)
+    return response.json()["dataRepositories"]
 
 
-def _refresh_token_is_invalid(e: requests.HTTPError) -> bool:
-    return (
-        e.response.status_code == 401
-        and exceptions.REFRESH_TOKEN_INVALID_ERROR_MESSAGE in e.response.text
+def create_tokens(
+    access_credentials: t.Optional[credentials.Credentials] = None,
+) -> t.Dict:
+    """Get tokens from the Mantik API."""
+    if access_credentials is None:
+        access_credentials = credentials.Credentials.from_env()
+    response = _send_request_to_mantik_api(
+        "POST", access_credentials.to_dict(), MANTIK_API_CREATE_TOKEN_API_PATH
     )
+    return response.json()
 
 
-def _create_api_url(endpoint: str) -> str:
-    # If the request path contains double slashes, the request
-    # is not forwarded to the API but to the UI and, thus, fails.
-    mlflow_tracking_uri = utils.env.get_required_env_var(
-        utils.mlflow.TRACKING_URI_ENV_VAR
-    )
-    if mlflow_tracking_uri is None:
-        raise RuntimeError(
-            f"MLflow tracking URI environment variable not set "
-            f"('{utils.mlflow.TRACKING_URI_ENV_VAR}')"
-        )
-    return utils.urls.ensure_https_and_remove_double_slashes_from_path(
-        f"{mlflow_tracking_uri}/{endpoint}"
+def refresh_tokens(
+    refresh_token: str,
+    access_credentials: t.Optional[credentials.Credentials] = None,
+) -> t.Dict:
+    """Get tokens from the Mantik API."""
+    if access_credentials is None:
+        access_credentials = credentials.Credentials.from_env()
+    data = {
+        **access_credentials.to_dict(include_password=False),
+        "refresh_token": refresh_token,
+    }
+    response = _send_request_to_mantik_api(
+        "POST", data, MANTIK_API_REFRESH_TOKEN_API_PATH
     )
+    return response.json()
 
 
-def _get_tokens(
-    url: str, data: t.Dict, refresh_token: t.Optional[str] = None
-) -> _tokens.Tokens:
-    response = _get_response(url=url, data=data)
-    return _tokens.Tokens.from_response(
-        response=response,
-        refresh_token=refresh_token,
+def _send_request_to_mantik_api(
+    method: str,
+    data: dict,
+    url_endpoint: str,
+    token: t.Optional[str] = None,
+) -> requests.Response:
+    base_url = os.environ.get(MANTIK_API_URL_ENV_VAR, MANTIK_API_URL)
+    url = _clean_double_slashes(f"{base_url}{url_endpoint}")
+    header = (
+        {
+            "Authorization": f"Bearer {token}",
+            "Accept": "application/json",
+        }
+        if token
+        else None
     )
+    request = {"url": url, "json": data, "headers": header}
+    try:
+        response = requests.request(method, **request)
+        response.raise_for_status()
+    except requests.HTTPError:
+        logger.exception(
+            "Call to Mantik API %s with data %s failed",
+            url,
+            data,
+            exc_info=True,
+        )
+        raise
+    else:
+        return response
 
 
-def _get_response(url: str, data: t.Dict) -> requests.Response:
-    response = requests.post(
-        url=url,
-        json=data,
-    )
-    response.raise_for_status()
-    return response
+def _clean_double_slashes(url: str) -> str:
+    scheme, rest = url.split("://", 1)
+    clean_rest = rest.replace("//", "/")
+    clean_url = f"{scheme}://{clean_rest}"
+    return clean_url
```

### Comparing `mantik-0.2.0/src/mantik/tracking/_server/tokens.py` & `mantik-0.3.1/src/mantik/authentication/tokens.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,24 @@
 import dataclasses
 import datetime
 import json
 import pathlib
 import typing as t
 
-import requests
-
 
 @dataclasses.dataclass(frozen=True)
 class Tokens:
     """Holds AWS Cognito auth tokens."""
 
     access_token: str
     refresh_token: str
     expires_at: datetime.datetime
     __encoding = "utf-8"
 
     @classmethod
-    def from_response(
-        cls, response: requests.Response, refresh_token: t.Optional[str] = None
-    ) -> "Tokens":
-        """Create from response."""
-        return cls.from_json_response(
-            response=response.json(),
-            refresh_token=refresh_token,
-        )
-
-    @classmethod
     def from_json_response(
         cls, response: t.Dict, refresh_token: t.Optional[str] = None
     ) -> "Tokens":
         """Create from JSON response."""
         access_token = response["AccessToken"]
         expires_at = datetime.datetime.fromisoformat(response["ExpiresAt"])
         if refresh_token is None:
```

### Comparing `mantik-0.2.0/src/mantik/tracking/environment.py` & `mantik-0.3.1/src/mantik/tracking/environment.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/unicore/_connect.py` & `mantik-0.3.1/src/mantik/unicore/_connect.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     logger.debug("Connection properties: %s", client.properties)
     return client
 
 
 def _create_transport(user: str, password: str) -> pyunicore.Transport:
     logger.debug("Creating transport for user %s", user)
     token = _create_token(user=user, password=password)
-    return pyunicore.Transport(auth_token=token, oidc=False)
+    return pyunicore.Transport(credential=token, oidc=False)
 
 
 def _create_token(user: str, password: str) -> str:
     token = f"{user}:{password}".encode()
     return base64.b64encode(token).decode("ascii")
```

### Comparing `mantik-0.2.0/src/mantik/unicore/backend.py` & `mantik-0.3.1/src/mantik/unicore/backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,15 +248,15 @@
 
 
 def create_job_description(
     config: core.Config,
     entry_point: _project_spec.EntryPoint,
     parameters: t.Dict,
     storage_dir: str,
-):
+) -> t.Dict:
     arguments = _create_arguments(
         entry_point=entry_point, parameters=parameters, storage_dir=storage_dir
     )
     job_description = {
         "Arguments": arguments,
         **config.to_dict(),
     }
```

### Comparing `mantik-0.2.0/src/mantik/unicore/client.py` & `mantik-0.3.1/src/mantik/unicore/client.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/unicore/config/_base.py` & `mantik-0.3.1/src/mantik/unicore/config/_base.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/unicore/config/_utils.py` & `mantik-0.3.1/src/mantik/unicore/config/_utils.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/unicore/config/core.py` & `mantik-0.3.1/src/mantik/unicore/config/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import mantik.unicore.config.resources as _resources
 import mantik.utils.env as env
 
 
 _USERNAME_ENV_VAR = "MANTIK_UNICORE_USERNAME"
 _PASSWORD_ENV_VAR = "MANTIK_UNICORE_PASSWORD"
 _PROJECT_ENV_VAR = "MANTIK_UNICORE_PROJECT"
+_UNICORE_AUTH_SERVER_URL_ENV_VAR = "MANTIK_UNICORE_AUTH_SERVER_URL"
 
 logger = logging.getLogger(__name__)
 
 
 @dataclasses.dataclass
 class Config(_base.ConfigObject):
     """The backend config for the UNICORE MLflow backend."""
@@ -116,8 +117,27 @@
             "Project": self.project,
             "Resources": self.resources,
             "Environment": self.environment.variables,
             "User precommand": self.environment.get_precommand(),
             "Executable": self.environment.execution.as_execution_command(),
             "RunUserPrecommandOnLoginNode": False,
         }
+
+        key_values = optional_add_srun_cpus_per_task_to_environment(
+            key_values, self.resources.cpus
+        )
+
         return _utils.create_dict_with_not_none_values(**key_values)
+
+
+def optional_add_srun_cpus_per_task_to_environment(
+    key_values: dict, cpus: t.Optional[int]
+) -> dict:
+    if cpus is None:
+        return key_values
+
+    environment = key_values.get("Environment") or {}
+    srun_cpus_per_task = environment.get("SRUN_CPUS_PER_TASK")
+
+    if srun_cpus_per_task is None:
+        key_values.setdefault("Environment", {})["SRUN_CPUS_PER_TASK"] = cpus
+    return key_values
```

### Comparing `mantik-0.2.0/src/mantik/unicore/config/environment.py` & `mantik-0.3.1/src/mantik/unicore/config/environment.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/unicore/config/executable.py` & `mantik-0.3.1/src/mantik/unicore/config/executable.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     """
 
     path: pathlib.Path
     type: str = _LOCAL_IMAGE_TYPE
 
     def __post_init__(self) -> None:
         """Check that the given type is correct."""
+        self.type = self.type.lower()
         self._ensure_valid_path_type()
         self._ensure_path_conform_to_type()
 
     @property
     def path_has_to_be_checked(self) -> bool:
         return self.type == _LOCAL_IMAGE_TYPE
 
@@ -156,15 +157,15 @@
         singularity_image_path = self._get_singularity_image_path()
         return (
             "srun singularity run "
             "--cleanenv "
             # Pass MLFLOW_TRACKING_URI variable if set, otherwise set to default
             # folder
             f"{_create_env_var_str(mlflow_utils.TRACKING_URI_ENV_VAR, default='file://$PWD/mlruns')} "  # noqa
-            # Pass tracking token if set
+            # Pass tracking  token if set
             f"{_create_optional_env_str(mlflow_utils.TRACKING_TOKEN_ENV_VAR)} "
             # Pass MLFLOW_EXPERIMENT_NAME variable if set
             f"{_create_optional_env_str(mlflow_utils.EXPERIMENT_NAME_ENV_VAR)} "
             # Pass Experiment ID if set
             f"{_create_optional_env_str(mlflow_utils.EXPERIMENT_ID_ENV_VAR)} "
             f"{singularity_image_path}"
         )
```

### Comparing `mantik-0.2.0/src/mantik/unicore/config/read.py` & `mantik-0.3.1/src/mantik/unicore/config/read.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/unicore/config/resources.py` & `mantik-0.3.1/src/mantik/unicore/config/resources.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/unicore/config/validate.py` & `mantik-0.3.1/src/mantik/unicore/config/validate.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/unicore/exceptions.py` & `mantik-0.3.1/src/mantik/unicore/exceptions.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/unicore/job.py` & `mantik-0.3.1/src/mantik/unicore/job.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/unicore/properties.py` & `mantik-0.3.1/src/mantik/unicore/properties.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/unicore/submitted_run.py` & `mantik-0.3.1/src/mantik/unicore/submitted_run.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/unicore/utils/upload.py` & `mantik-0.3.1/src/mantik/unicore/utils/upload.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/unicore/utils/zip.py` & `mantik-0.3.1/src/mantik/unicore/utils/zip.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/unicore/working_dir.py` & `mantik-0.3.1/src/mantik/unicore/working_dir.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/utils/env.py` & `mantik-0.3.1/src/mantik/utils/env.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/mantik/utils/temp_dir.py` & `mantik-0.3.1/src/mantik/utils/temp_dir.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/tests/resources/cognito/auth-response.json` & `mantik-0.3.1/src/tests/resources/cognito/auth-response.json`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/tests/resources/cognito/incorrect-login-credentials-response.json` & `mantik-0.3.1/src/tests/resources/cognito/incorrect-login-credentials-response.json`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/tests/resources/cognito/refresh-response.json` & `mantik-0.3.1/src/tests/resources/cognito/refresh-response.json`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/tests/resources/cognito/refresh-token-expired-response.json` & `mantik-0.3.1/src/tests/resources/cognito/refresh-token-expired-response.json`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/tests/resources/cognito/refresh-token-invalid-response.json` & `mantik-0.3.1/src/tests/resources/cognito/refresh-token-invalid-response.json`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/tests/resources/cognito/user-not-found-response.json` & `mantik-0.3.1/src/tests/resources/cognito/user-not-found-response.json`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/tests/resources/test-project/main.py` & `mantik-0.3.1/src/tests/resources/test-project/main.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/tests/resources/unicore-responses/job-property-response.json` & `mantik-0.3.1/src/tests/resources/unicore-responses/job-property-response.json`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/tests/unit/cli/runs/conftest.py` & `mantik-0.3.1/src/tests/unit/cli/runs/conftest.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/tests/unit/cli/runs/test_cancel.py` & `mantik-0.3.1/src/tests/unit/cli/runs/test_cancel.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/tests/unit/cli/runs/test_download.py` & `mantik-0.3.1/src/tests/unit/cli/runs/test_download.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/tests/unit/cli/runs/test_info.py` & `mantik-0.3.1/src/tests/unit/cli/runs/test_info.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/tests/unit/cli/runs/test_list.py` & `mantik-0.3.1/src/tests/unit/cli/runs/test_list.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/tests/unit/cli/runs/test_logs.py` & `mantik-0.3.1/src/tests/unit/cli/runs/test_logs.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/tests/unit/cli/runs/test_options.py` & `mantik-0.3.1/src/tests/unit/cli/runs/test_options.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/tests/unit/cli/runs/test_status.py` & `mantik-0.3.1/src/tests/unit/cli/runs/test_status.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/tests/unit/cli/runs/test_submit.py` & `mantik-0.3.1/src/tests/unit/cli/runs/test_submit.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import pytest
 
 import mantik.cli.main as main
 import mantik.cli.runs.submit as submit
 import mantik.compute_backend_service.api as api
 import mantik.compute_backend_service.client as _client
 import mantik.testing.token as testing_token
-import mantik.tracking._server._credentials as _credentials
 import mantik.unicore.config.core as core
 import mantik.utils as utils
+import mantik.utils.mantik_api.credentials as _credentials
 
 TEST_MLFLOW_TRACKING_URI = "https://test-uri.com"
 ENV_VARS = {
     core._USERNAME_ENV_VAR: "test-user",
     core._PASSWORD_ENV_VAR: "test-password",
     core._PROJECT_ENV_VAR: "test-project",
     utils.mlflow.TRACKING_URI_ENV_VAR: TEST_MLFLOW_TRACKING_URI,
```

### Comparing `mantik-0.2.0/src/tests/unit/cli/test_init.py` & `mantik-0.3.1/src/tests/unit/cli/test_init.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/tests/unit/compute_backend_service/conftest.py` & `mantik-0.3.1/src/tests/unit/compute_backend_service/conftest.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/tests/unit/compute_backend_service/test_api.py` & `mantik-0.3.1/src/tests/unit/compute_backend_service/test_api.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/tests/unit/compute_backend_service/test_app.py` & `mantik-0.3.1/src/tests/unit/compute_backend_service/test_app.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/tests/unit/compute_backend_service/test_client.py` & `mantik-0.3.1/src/tests/unit/compute_backend_service/test_client.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/tests/unit/compute_backend_service/test_compute_backend.py` & `mantik-0.3.1/src/tests/unit/compute_backend_service/test_compute_backend.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 
 @unittest.mock.patch("mlflow.projects.run")
 def test_handle_submit_run_request(
     mock_run, submit_run_request_data, submit_run_request_files
 ):
     mock_run.return_value.run_id = "1"
     mock_run.return_value.job_id = "2"
-    utils.env.set_env_vars({utils.mlflow.TRACKING_URI_ENV_VAR: "foo"})
-    response = backend.handle_submit_run_request(
-        **submit_run_request_data, **submit_run_request_files
-    )
-    assert response
-    mock_run.assert_called()
-    # Assert that secret environment variables are unset
-    testing.env.assert_env_var(core._USERNAME_ENV_VAR, None)
+    with utils.env.env_vars_set({utils.mlflow.TRACKING_URI_ENV_VAR: "foo"}):
+        response = backend.handle_submit_run_request(
+            **submit_run_request_data, **submit_run_request_files
+        )
+        assert response
+        mock_run.assert_called()
+        # Assert that secret environment variables are unset
+        testing.env.assert_env_var(core._USERNAME_ENV_VAR, None)
 
 
 def test_unzip_to_tmp(zipped_content):
     with tempfile.TemporaryDirectory() as directory:
         backend._unzip_to_file(zipped_content, directory)
         files = list(
             map(
```

### Comparing `mantik-0.2.0/src/tests/unit/compute_backend_service/test_exception_handler.py` & `mantik-0.3.1/src/tests/unit/compute_backend_service/test_exception_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,17 +157,19 @@
         "this mlflow error occurred: Could not "
         "find non-existent-entry-point among "
         "entry points ['main'] or interpret "
         "non-existent-entry-point as a runnable script. "
         "Supported script file "
         "extensions: ['.py', '.sh']\"}"
     )
-    # Note: Experiment ID environment variable is set implicitly here,
+    # Note: Experiment ID environment variable and Mlflow tracking uri,
+    # is set implicitly here,
     # breaking other tests
     os.environ.pop("MLFLOW_EXPERIMENT_ID")
+    os.environ.pop("MLFLOW_TRACKING_URI")
 
 
 @unittest.mock.patch(
     "mantik.compute_backend_service.backend.handle_submit_run_request",
     **{"return_value.raiseError.side_effect": Exception},
 )
 def test_custom_500_internal_server_error(
```

### Comparing `mantik-0.2.0/src/tests/unit/mlflow_server/conftest.py` & `mantik-0.3.1/src/tests/unit/mlflow_server/conftest.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/tests/unit/mlflow_server/flask/api/test_tokens_api.py` & `mantik-0.3.1/src/tests/unit/mlflow_server/flask/api/test_tokens_api.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/tests/unit/mlflow_server/flask/conftest.py` & `mantik-0.3.1/src/tests/unit/mlflow_server/flask/conftest.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/tests/unit/mlflow_server/tokens/cognito/test_auth.py` & `mantik-0.3.1/src/tests/unit/mlflow_server/tokens/cognito/test_auth.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/tests/unit/mlflow_server/tokens/test_verifier.py` & `mantik-0.3.1/src/tests/unit/mlflow_server/tokens/test_verifier.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/tests/unit/tracking/_server/test_tokens.py` & `mantik-0.3.1/src/tests/unit/athentication/test_tokens.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import datetime
 import pathlib
 
 import freezegun
 import pytest
 
-import mantik.tracking._server.tokens as _tokens
+import mantik.authentication.tokens as _tokens
 
 
 @pytest.fixture()
 def tokens():
     return _tokens.Tokens(
         access_token="test-access-token",
         refresh_token="test-refresh-token",
```

### Comparing `mantik-0.2.0/src/tests/unit/tracking/test_credentials.py` & `mantik-0.3.1/src/tests/unit/athentication/test_credentials.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import contextlib
 
 import pytest
 
-import mantik.tracking._server._credentials as _credentials
 import mantik.utils.env as env
+import mantik.utils.mantik_api.credentials as _credentials
 
 # Variables have to be renamed for testing. Otherwise, the actual
 # variables will be replaced and reset if it is set at the time of the test.
 # This does not allow testing cases where the environment variables are not set
 # by the user.
 _credentials._MANTIK_USERNAME_ENV_VAR = "TEST_MANTIK_USERNAME_ENV_VAR"
 _credentials._MANTIK_PASSWORD_ENV_VAR = "TEST_MANTIK_PASSWORD_ENV_VAR"
```

### Comparing `mantik-0.2.0/src/tests/unit/tracking/test_track.py` & `mantik-0.3.1/src/tests/unit/tracking/test_track.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import datetime
 import os
 import typing as t
 
-import mantik.mlflow_server.flask.api as _api
+import mantik.authentication.auth as auth
+import mantik.authentication.tokens as _tokens
 import mantik.mlflow_server.tokens.cognito.exceptions as exceptions
 import mantik.testing.env
 import mantik.testing.token as testing_token
-import mantik.tracking._server.tokens as _tokens
 import mantik.tracking.track as track
 import mantik.utils as utils
+import mantik.utils.mantik_api.client as mantik_api
 
 
 def test_track_without_existing_tokens(
     requests_mock,
     tmp_dir_as_test_mantik_folder,
     required_env_vars,
-    mlflow_tracking_uri,
     token_expiration_date,
 ):
     requests_mock.post(
-        url=f"{mlflow_tracking_uri}{_api.tokens.CREATE_TOKEN_API_PATH}",
+        url=f"{mantik_api.MANTIK_API_URL}"
+        f"{mantik_api.MANTIK_API_CREATE_TOKEN_API_PATH}",
         json={
             "AccessToken": "test-access-token",
             "RefreshToken": "test-refresh-token",
             "ExpiresAt": token_expiration_date.isoformat(),
         },
     )
 
@@ -39,15 +40,14 @@
     access_token="test-stored-access-token",
     refresh_token="test-stored-refresh-token",
 )
 def test_track_with_existing_valid_tokens(
     monkeypatch,
     tmp_dir_as_test_mantik_folder,
     required_env_vars,
-    mlflow_tracking_uri,
     token_expiration_date,
 ):
     _init_tracking_and_assert_expected(
         env_vars=required_env_vars,
         expected_access_token="test-stored-access-token",
     )
 
@@ -57,19 +57,19 @@
     refresh_token="test-stored-refresh-token",
     expires_at=datetime.datetime(2020, 1, 1),
 )
 def test_track_with_existing_expired_token(
     requests_mock,
     tmp_dir_as_test_mantik_folder,
     required_env_vars,
-    mlflow_tracking_uri,
     token_expiration_date,
 ):
     requests_mock.post(
-        url=f"{mlflow_tracking_uri}{_api.tokens.REFRESH_TOKEN_API_PATH}",
+        url=f"{mantik_api.MANTIK_API_URL}"
+        f"{mantik_api.MANTIK_API_REFRESH_TOKEN_API_PATH}",
         json={
             "AccessToken": "test-refreshed-access-token",
             "ExpiresAt": token_expiration_date.isoformat(),
         },
     )
 
     _init_tracking_and_assert_expected(
@@ -81,85 +81,91 @@
 @testing_token.set_token(
     access_token="test-stored-expired-access-token", refresh_token="test-stored"
 )
 def test_track_with_existing_expired_token_and_expired_refresh_token(
     requests_mock,
     tmp_dir_as_test_mantik_folder,
     required_env_vars,
-    mlflow_tracking_uri,
     token_expiration_date,
 ):
     # Mock refresh api to return expired error
     requests_mock.post(
-        url=f"{mlflow_tracking_uri}{_api.tokens.REFRESH_TOKEN_API_PATH}",
+        url=f"{mantik_api.MANTIK_API_URL}"
+        f"{mantik_api.MANTIK_API_REFRESH_TOKEN_API_PATH}",
         status_code=401,
         text=exceptions.REFRESH_TOKEN_EXPIRED_ERROR_MESSAGE,
     )
     # Mock get api to return refreshed tokens
     requests_mock.post(
-        url=(f"{mlflow_tracking_uri}" f"{_api.tokens.CREATE_TOKEN_API_PATH}"),
+        url=(
+            f"{mantik_api.MANTIK_API_URL}"
+            f"{mantik_api.MANTIK_API_CREATE_TOKEN_API_PATH}"
+        ),
         json={
             "AccessToken": "test-refreshed-access-token",
             "RefreshToken": "test-refreshed-refresh-token",
             "ExpiresAt": token_expiration_date.isoformat(),
         },
     )
 
     tokens = _tokens.Tokens(
         access_token="test-stored-expired-access-token",
         refresh_token="test-stored-refresh-token",
         expires_at=datetime.datetime(2020, 1, 1),
     )
-    tokens.write_to_file(track._MANTIK_TOKEN_FILE)
+    tokens.write_to_file(auth._MANTIK_TOKEN_FILE)
 
     _init_tracking_and_assert_expected(
         env_vars=required_env_vars,
         expected_access_token="test-refreshed-access-token",
     )
 
-    result_tokens = _tokens.Tokens.from_file(track._MANTIK_TOKEN_FILE)
+    result_tokens = _tokens.Tokens.from_file(auth._MANTIK_TOKEN_FILE)
     assert result_tokens.access_token == "test-refreshed-access-token"
     assert result_tokens.refresh_token == "test-refreshed-refresh-token"
     assert result_tokens.expires_at == token_expiration_date
 
 
 @testing_token.set_token(
     access_token="test-stored-expired-access-token",
     refresh_token="test-stored-invalid-refresh-token",
     expires_at=datetime.datetime(2020, 1, 1),
 )
 def test_track_with_existing_invalid_refresh_token(
     requests_mock,
     tmp_dir_as_test_mantik_folder,
     required_env_vars,
-    mlflow_tracking_uri,
     token_expiration_date,
 ):
     # Mock refresh api to return invalid error
     requests_mock.post(
-        url=f"{mlflow_tracking_uri}{_api.tokens.REFRESH_TOKEN_API_PATH}",
+        url=f"{mantik_api.MANTIK_API_URL}"
+        f"{mantik_api.MANTIK_API_REFRESH_TOKEN_API_PATH}",
         status_code=401,
         text=exceptions.REFRESH_TOKEN_INVALID_ERROR_MESSAGE,
     )
     # Mock get api to return refreshed tokens
     requests_mock.post(
-        url=(f"{mlflow_tracking_uri}" f"{_api.tokens.CREATE_TOKEN_API_PATH}"),
+        url=(
+            f"{mantik_api.MANTIK_API_URL}"
+            f"{mantik_api.MANTIK_API_CREATE_TOKEN_API_PATH}"
+        ),
         json={
             "AccessToken": "test-refreshed-access-token",
             "RefreshToken": "test-refreshed-refresh-token",
             "ExpiresAt": token_expiration_date.isoformat(),
         },
     )
 
     _init_tracking_and_assert_expected(
         env_vars=required_env_vars,
         expected_access_token="test-refreshed-access-token",
     )
 
-    result_tokens = _tokens.Tokens.from_file(track._MANTIK_TOKEN_FILE)
+    result_tokens = _tokens.Tokens.from_file(auth._MANTIK_TOKEN_FILE)
     assert result_tokens.access_token == "test-refreshed-access-token"
     assert result_tokens.refresh_token == "test-refreshed-refresh-token"
     assert result_tokens.expires_at == token_expiration_date
 
 
 def _init_tracking_and_assert_expected(
     env_vars: t.Dict[str, str],
```

### Comparing `mantik-0.2.0/src/tests/unit/unicore/config/conftest.py` & `mantik-0.3.1/src/tests/unit/unicore/config/conftest.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/tests/unit/unicore/config/test_core.py` & `mantik-0.3.1/src/tests/unit/unicore/config/test_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,15 +231,15 @@
                         "CPUs": 48,
                         "CPUsPerNode": 24,
                         "Memory": "10GiB",
                         "Reservation": "test-reservation",
                         "NodeConstraints": "test-node-constraints",
                         "QoS": "test-qos",
                     },
-                    "Environment": {"TEST": "test"},
+                    "Environment": {"TEST": "test", "SRUN_CPUS_PER_TASK": 48},
                     "Executable": "srun singularity run --cleanenv --env "
                     "MLFLOW_TRACKING_URI=${MLFLOW_TRACKING_URI:"
                     "-file://$PWD/mlruns} "
                     "${MLFLOW_TRACKING_TOKEN:+--env "
                     "MLFLOW_TRACKING_TOKEN=$MLFLOW_TRACKING_TOKEN} "
                     "${MLFLOW_EXPERIMENT_NAME:+--env "
                     "MLFLOW_EXPERIMENT_NAME=$MLFLOW_EXPERIMENT_NAME} "
```

### Comparing `mantik-0.2.0/src/tests/unit/unicore/config/test_environment.py` & `mantik-0.3.1/src/tests/unit/unicore/config/test_environment.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/tests/unit/unicore/config/test_executable.py` & `mantik-0.3.1/src/tests/unit/unicore/config/test_executable.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/tests/unit/unicore/config/test_read.py` & `mantik-0.3.1/src/tests/unit/unicore/config/test_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         backend_config["UnicoreApiUrl"]
         == "https://zam2125.zam.kfa-juelich.de:9112/JUWELS/rest/core"
     )
     assert backend_config["Resources"]["Queue"] == "devel"
     assert backend_config["Resources"]["Nodes"] == 2
     assert backend_config["Environment"]["Singularity"] == {
         "Path": "mantik-test.sif",
-        "Type": "local",
+        "Type": "lOcAl",
     }
 
 
 def test_read_config_unsupported_type():
     unsupported_format = ".yamml"
     with pytest.raises(mantik.unicore.exceptions.ConfigValidationError) as e:
         read.read_config(pathlib.Path(f"backend-config{unsupported_format}"))
@@ -36,23 +36,23 @@
         backend_config["UnicoreApiUrl"]
         == "https://zam2125.zam.kfa-juelich.de:9112/JUWELS/rest/core"
     )
     assert backend_config["Resources"]["Queue"] == "devel"
     assert backend_config["Resources"]["Nodes"] == 2
     assert backend_config["Environment"]["Singularity"] == {
         "Path": "mantik-test.sif",
-        "Type": "local",
+        "Type": "lOcAl",
     }
 
 
 def test_read_json_config(unicore_config_json):
     backend_config = read._read_yaml_config(unicore_config_json)
     assert (
         backend_config["UnicoreApiUrl"]
         == "https://zam2125.zam.kfa-juelich.de:9112/JUWELS/rest/core"
     )
     assert backend_config["Resources"]["Queue"] == "devel"
     assert backend_config["Resources"]["Nodes"] == 2
     assert backend_config["Environment"]["Singularity"] == {
         "Path": "mantik-test.sif",
-        "Type": "local",
+        "Type": "lOcAl",
     }
```

### Comparing `mantik-0.2.0/src/tests/unit/unicore/config/test_utils.py` & `mantik-0.3.1/src/tests/unit/unicore/config/test_utils.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/tests/unit/unicore/config/test_validate.py` & `mantik-0.3.1/src/tests/unit/unicore/config/test_validate.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/tests/unit/unicore/conftest.py` & `mantik-0.3.1/src/tests/unit/unicore/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,16 @@
         api_url="test-url",
         user="user",
         password="password",
         project="test-project",
         environment=config.environment.Environment(
             execution=executable.Singularity(
                 path=pathlib.Path("mantik-test.sif"),
-            )
+            ),
+            variables={"SRUN_CPUS_PER_TASK": 100},
         ),
         resources=config.resources.Resources(queue="batch"),
         exclude=["*.py", "*.sif"],
     )
 
 
 @pytest.fixture()
```

### Comparing `mantik-0.2.0/src/tests/unit/unicore/test_client_wrapper.py` & `mantik-0.3.1/src/tests/unit/unicore/test_client_wrapper.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/tests/unit/unicore/test_connect.py` & `mantik-0.3.1/src/tests/unit/unicore/test_connect.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/tests/unit/unicore/test_exceptions.py` & `mantik-0.3.1/src/tests/unit/unicore/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/tests/unit/unicore/test_properties.py` & `mantik-0.3.1/src/tests/unit/unicore/test_properties.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/tests/unit/unicore/test_submitted_run.py` & `mantik-0.3.1/src/tests/unit/unicore/test_submitted_run.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/tests/unit/unicore/utils/test_upload.py` & `mantik-0.3.1/src/tests/unit/unicore/utils/test_upload.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/tests/unit/utils/conftest.py` & `mantik-0.3.1/src/tests/unit/utils/conftest.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/tests/unit/utils/test_env.py` & `mantik-0.3.1/src/tests/unit/utils/test_env.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/src/tests/unit/utils/test_urls.py` & `mantik-0.3.1/src/tests/unit/utils/test_urls.py`

 * *Files identical despite different names*

### Comparing `mantik-0.2.0/PKG-INFO` & `mantik-0.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mantik
-Version: 0.2.0
+Version: 0.3.1
 Summary: mantik for mlflow
 Home-page: https://mantik.ai/
 License: MIT
 Keywords: mlflow,machine learning,hpc,unicore
 Author: Fabian Emmerich
 Author-email: fabian.emmerich@4-cast.de
 Maintainer: Elia Boscaini
@@ -13,26 +13,27 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: Flask (>=2.1.2,<3.0.0)
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: boto3 (>=1.23.6,<2.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: fastapi (>=0.78.0,<0.79.0)
 Requires-Dist: mlflow (==2.2.2)
 Requires-Dist: pydantic (>=1.9.0,<2.0.0)
 Requires-Dist: python-jose (>=3.3.0,<4.0.0)
 Requires-Dist: python-multipart (>=0.0.5,<0.0.6)
-Requires-Dist: pyunicore (>=0.9.16,<0.10.0)
+Requires-Dist: pyunicore[crypto,fs,fuse] (>=0.15.0,<0.16.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: uvicorn[standard] (>=0.17.6,<0.18.0)
 Project-URL: Documentation, https://mantik-ai.gitlab.io/mantik
 Project-URL: Repository, https://gitlab.com/mantik-ai/mantik
 Description-Content-Type: text/markdown
 
 # mantik - plugin for MLflow with HPC (UNICORE)
@@ -45,7 +46,9 @@
 ```shell
 mlflow run --backend unicore --backend-config <path to config> <path to project>
 ```
 
 For a quickstart see [our documentation](https://mantik-ai.gitlab.io/mantik/quickstart.html)
 
 Service desk email: contact-project+mantik-ai-mantik-42525397-issue-@incoming.gitlab.com
+
+
```

