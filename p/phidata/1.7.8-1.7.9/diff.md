# Comparing `tmp/phidata-1.7.8.tar.gz` & `tmp/phidata-1.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phidata-1.7.8.tar", last modified: Wed Jun 21 12:33:30 2023, max compression
+gzip compressed data, was "phidata-1.7.9.tar", last modified: Fri Jul  7 12:54:31 2023, max compression
```

## Comparing `phidata-1.7.8.tar` & `phidata-1.7.9.tar`

### file list

```diff
@@ -1,531 +1,532 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.282010 phidata-1.7.8/
--rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-06-21 12:33:02.000000 phidata-1.7.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-06-21 12:33:30.282010 phidata-1.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-21 12:33:02.000000 phidata-1.7.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.194009 phidata-1.7.8/phidata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.194009 phidata-1.7.8/phidata/airflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/airflow/airflow_installed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.194009 phidata-1.7.8/phidata/airflow/operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/airflow/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/airflow/operators/empty.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.198009 phidata-1.7.8/phidata/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.198009 phidata-1.7.8/phidata/app/airflow/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   100927 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/airflow/airflow_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    30469 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/airflow/airflow_flower.py
--rw-r--r--   0 runner    (1001) docker     (123)    30508 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/airflow/airflow_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    30505 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/airflow/airflow_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    30515 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/airflow/airflow_webserver.py
--rw-r--r--   0 runner    (1001) docker     (123)    30710 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/airflow/airflow_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.198009 phidata-1.7.8/phidata/app/alertmanager/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/alertmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47889 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/alertmanager/alertmanager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.202009 phidata-1.7.8/phidata/app/amundsen/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/amundsen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48031 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/amundsen/frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    48032 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/amundsen/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    47944 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/amundsen/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.202009 phidata-1.7.8/phidata/app/assistant/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49912 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/assistant/assistant.py
--rw-r--r--   0 runner    (1001) docker     (123)    30166 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/aws_app.py
--rw-r--r--   0 runner    (1001) docker     (123)    17164 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/base_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.202009 phidata-1.7.8/phidata/app/cadvisor/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/cadvisor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49678 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/cadvisor/cadvisor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.202009 phidata-1.7.8/phidata/app/databox/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/databox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    86151 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/databox/databox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.206009 phidata-1.7.8/phidata/app/db/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/db/base_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.206009 phidata-1.7.8/phidata/app/django/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27483 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/django/django_app.py
--rw-r--r--   0 runner    (1001) docker     (123)    30070 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/django/django_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)    17172 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/docker_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.206009 phidata-1.7.8/phidata/app/elastic/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/elastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/elastic/elastic_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.206009 phidata-1.7.8/phidata/app/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48675 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/elasticsearch/elasticsearch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.206009 phidata-1.7.8/phidata/app/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20266 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/fastapi/fastapi_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.210009 phidata-1.7.8/phidata/app/grafana/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/grafana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49781 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/grafana/grafana.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.210009 phidata-1.7.8/phidata/app/jupyter/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27093 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/jupyter/jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)    46942 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/jupyter/jupyter_hub.py
--rw-r--r--   0 runner    (1001) docker     (123)    93432 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/jupyter/jupyter_lab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.210009 phidata-1.7.8/phidata/app/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/k8s/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/k8s/dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/k8s/url.py
--rw-r--r--   0 runner    (1001) docker     (123)    37830 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/k8s_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.210009 phidata-1.7.8/phidata/app/mysql/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49110 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/mysql/mysql_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.210009 phidata-1.7.8/phidata/app/neo4j/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/neo4j/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47856 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/neo4j/neo4j.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.210009 phidata-1.7.8/phidata/app/nodeexporter/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/nodeexporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47898 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/nodeexporter/nodeexporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    38495 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/phidata_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.210009 phidata-1.7.8/phidata/app/postgres/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53156 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/postgres/postgres_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.210009 phidata-1.7.8/phidata/app/prometheus/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/prometheus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49051 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/prometheus/prometheus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.214009 phidata-1.7.8/phidata/app/qdrant/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/qdrant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19992 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/qdrant/qdrant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.214009 phidata-1.7.8/phidata/app/redis/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49058 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/redis/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)    53296 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/redis/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.214009 phidata-1.7.8/phidata/app/server/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18424 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/server/api_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    58714 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/server/server_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.214009 phidata-1.7.8/phidata/app/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49424 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/spark/spark_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17222 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/spark/spark_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    17332 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/spark/spark_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.214009 phidata-1.7.8/phidata/app/streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20207 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/streamlit/streamlit_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.218009 phidata-1.7.8/phidata/app/superset/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/superset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71570 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/superset/superset_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    22925 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/superset/superset_init.py
--rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/superset/superset_webserver.py
--rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/superset/superset_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    22917 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/superset/superset_worker_beat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.218009 phidata-1.7.8/phidata/app/traefik/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/traefik/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   115905 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/traefik/crds.py
--rw-r--r--   0 runner    (1001) docker     (123)    48190 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/traefik/ingress_route.py
--rw-r--r--   0 runner    (1001) docker     (123)    44972 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/app/traefik/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.218009 phidata-1.7.8/phidata/asset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/asset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.218009 phidata-1.7.8/phidata/asset/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/asset/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/asset/aws/aws_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)    24787 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/asset/data_asset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.218009 phidata-1.7.8/phidata/asset/local/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/asset/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14564 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/asset/local/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/asset/local/local_asset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.218009 phidata-1.7.8/phidata/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.218009 phidata-1.7.8/phidata/aws/athena/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/athena/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.222009 phidata-1.7.8/phidata/aws/create/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/create/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.222009 phidata-1.7.8/phidata/aws/create/iam/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/create/iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/create/iam/eks_admin_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/create/iam/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    23058 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.222009 phidata-1.7.8/phidata/aws/enums/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/enums/manager_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.222009 phidata-1.7.8/phidata/aws/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.222009 phidata-1.7.8/phidata/aws/resource/acm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/acm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10630 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/acm/certificate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.222009 phidata-1.7.8/phidata/aws/resource/athena/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/athena/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.222009 phidata-1.7.8/phidata/aws/resource/cloudformation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/cloudformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10882 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/cloudformation/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.222009 phidata-1.7.8/phidata/aws/resource/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/ec2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21341 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/ec2/security_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/ec2/subnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/ec2/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.226009 phidata-1.7.8/phidata/aws/resource/ecs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/ecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/ecs/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    26253 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/ecs/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    19630 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/ecs/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    22397 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/ecs/task_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/ecs/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.226009 phidata-1.7.8/phidata/aws/resource/eks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/eks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/eks/addon.py
--rw-r--r--   0 runner    (1001) docker     (123)    30104 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/eks/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    13731 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/eks/fargate_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    23785 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/eks/kubeconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    23742 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/eks/node_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.226009 phidata-1.7.8/phidata/aws/resource/elasticache/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/elasticache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15823 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/elasticache/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/elasticache/subnet_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.226009 phidata-1.7.8/phidata/aws/resource/elb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/elb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/elb/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/elb/load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/elb/target_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.226009 phidata-1.7.8/phidata/aws/resource/emr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/emr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/emr/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.230009 phidata-1.7.8/phidata/aws/resource/glue/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12850 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/glue/crawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.230009 phidata-1.7.8/phidata/aws/resource/iam/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/iam/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/iam/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9828 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/iam/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.230009 phidata-1.7.8/phidata/aws/resource/rds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/rds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36056 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/rds/db_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    35380 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/rds/db_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/rds/db_subnet_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.230009 phidata-1.7.8/phidata/aws/resource/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/s3/bucket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.230009 phidata-1.7.8/phidata/aws/resource/secret/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/secret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11398 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/secret/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/secret/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     9688 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/resource/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.230009 phidata-1.7.8/phidata/aws/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21797 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/s3/csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    24100 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/s3/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14394 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/s3/dataset_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/s3/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    22470 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/aws/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.234010 phidata-1.7.8/phidata/checks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/checks/check.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/checks/not_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.234010 phidata-1.7.8/phidata/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/decorators/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/decorators/validate_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.234010 phidata-1.7.8/phidata/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/docker/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/docker/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/docker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/docker/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/docker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/docker/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.238010 phidata-1.7.8/phidata/docker/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/docker/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/docker/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16440 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/docker/resource/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/docker/resource/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    14552 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/docker/resource/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/docker/resource/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/docker/resource/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/docker/resource/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/docker/resource/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.238010 phidata-1.7.8/phidata/docker/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/docker/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/docker/utils/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    24179 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/docker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.238010 phidata-1.7.8/phidata/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/exceptions/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/exceptions/task.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/exceptions/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.238010 phidata-1.7.8/phidata/infra/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/infra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/infra/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/infra/args.py
--rw-r--r--   0 runner    (1001) docker     (123)    15390 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/infra/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12048 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/infra/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.242010 phidata-1.7.8/phidata/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.242010 phidata-1.7.8/phidata/k8s/create/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/create/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.242010 phidata-1.7.8/phidata/k8s/create/apiextensions_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/create/apiextensions_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.242010 phidata-1.7.8/phidata/k8s/create/apiextensions_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/create/apiextensions_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.242010 phidata-1.7.8/phidata/k8s/create/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/create/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.242010 phidata-1.7.8/phidata/k8s/create/apps/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/create/apps/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/create/apps/v1/deployment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.242010 phidata-1.7.8/phidata/k8s/create/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/create/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/create/common/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/create/common/port.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.242010 phidata-1.7.8/phidata/k8s/create/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/create/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.246010 phidata-1.7.8/phidata/k8s/create/core/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/create/core/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/create/core/v1/config_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/create/core/v1/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/create/core/v1/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/create/core/v1/persistent_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/create/core/v1/persistent_volume_claim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/create/core/v1/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/create/core/v1/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/create/core/v1/service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/create/core/v1/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.246010 phidata-1.7.8/phidata/k8s/create/crb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/create/crb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/create/crb/eks_admin_crb.py
--rw-r--r--   0 runner    (1001) docker     (123)    19062 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/create/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/create/kubeconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.246010 phidata-1.7.8/phidata/k8s/create/networking_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/create/networking_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.246010 phidata-1.7.8/phidata/k8s/create/networking_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/create/networking_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/create/networking_k8s_io/v1/ingress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.246010 phidata-1.7.8/phidata/k8s/create/rbac_authorization_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/create/rbac_authorization_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.246010 phidata-1.7.8/phidata/k8s/create/rbac_authorization_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/create/rbac_authorization_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.250010 phidata-1.7.8/phidata/k8s/create/storage_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/create/storage_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.250010 phidata-1.7.8/phidata/k8s/create/storage_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/create/storage_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/create/storage_k8s_io/v1/storage_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.250010 phidata-1.7.8/phidata/k8s/enums/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/enums/api_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/enums/api_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/enums/image_pull_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/enums/kind.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/enums/manager_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/enums/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/enums/pv.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/enums/restart_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/enums/service_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/enums/storage_class.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/enums/volume_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.254010 phidata-1.7.8/phidata/k8s/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.254010 phidata-1.7.8/phidata/k8s/resource/apiextensions_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/apiextensions_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.254010 phidata-1.7.8/phidata/k8s/resource/apiextensions_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/apiextensions_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    15390 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.254010 phidata-1.7.8/phidata/k8s/resource/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.254010 phidata-1.7.8/phidata/k8s/resource/apps/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/apps/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/apps/v1/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/apps/v1/deployment_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.254010 phidata-1.7.8/phidata/k8s/resource/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.258010 phidata-1.7.8/phidata/k8s/resource/core/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/core/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/core/v1/config_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    18530 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/core/v1/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/core/v1/local_object_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/core/v1/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/core/v1/node_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/core/v1/object_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/core/v1/persistent_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/core/v1/persistent_volume_claim.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/core/v1/pod.py
--rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/core/v1/pod_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/core/v1/pod_template_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/core/v1/resource_requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/core/v1/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)    18982 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/core/v1/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/core/v1/service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/core/v1/toleration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/core/v1/topology_spread_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/core/v1/volume.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/core/v1/volume_node_affinity.py
--rw-r--r--   0 runner    (1001) docker     (123)    13397 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/core/v1/volume_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/kubeconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.262010 phidata-1.7.8/phidata/k8s/resource/meta/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.262010 phidata-1.7.8/phidata/k8s/resource/meta/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/meta/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/meta/v1/label_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/meta/v1/object_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.262010 phidata-1.7.8/phidata/k8s/resource/networking_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/networking_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.262010 phidata-1.7.8/phidata/k8s/resource/networking_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/networking_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10026 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/networking_k8s_io/v1/ingress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.262010 phidata-1.7.8/phidata/k8s/resource/rbac_authorization_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/rbac_authorization_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.262010 phidata-1.7.8/phidata/k8s/resource/rbac_authorization_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/rbac_authorization_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.262010 phidata-1.7.8/phidata/k8s/resource/storage_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/storage_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.262010 phidata-1.7.8/phidata/k8s/resource/storage_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/storage_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10127 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/resource/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.262010 phidata-1.7.8/phidata/k8s/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/utils/pod.py
--rw-r--r--   0 runner    (1001) docker     (123)    43059 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/k8s/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.262010 phidata-1.7.8/phidata/llm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/llm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.266010 phidata-1.7.8/phidata/llm/duckdb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/llm/duckdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/llm/duckdb/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/llm/duckdb/chain.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/llm/duckdb/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/llm/duckdb/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/llm/duckdb/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/llm/duckdb/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.266010 phidata-1.7.8/phidata/product/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/product/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29505 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/product/data_product.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.266010 phidata-1.7.8/phidata/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/resource/reference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.266010 phidata-1.7.8/phidata/table/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.266010 phidata-1.7.8/phidata/table/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/table/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/table/local/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    23516 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/table/local/local_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/table/local/parquet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.270010 phidata-1.7.8/phidata/table/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/table/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/table/s3/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/table/s3/parquet.py
--rw-r--r--   0 runner    (1001) docker     (123)    23064 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/table/s3/s3_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.270010 phidata-1.7.8/phidata/table/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/table/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/table/sql/postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)    35497 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/table/sql/sql_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.270010 phidata-1.7.8/phidata/task/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.270010 phidata-1.7.8/phidata/task/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/task/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.270010 phidata-1.7.8/phidata/task/aws/athena/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/task/aws/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/task/aws/athena/run_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.270010 phidata-1.7.8/phidata/task/aws/emr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/task/aws/emr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/task/aws/emr/create_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/task/aws/emr/delete_cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.270010 phidata-1.7.8/phidata/task/aws/glue/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/task/aws/glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/task/aws/glue/start_crawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/task/decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.274010 phidata-1.7.8/phidata/task/dev/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/task/dev/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.274010 phidata-1.7.8/phidata/task/download/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/task/download/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.274010 phidata-1.7.8/phidata/task/download/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/task/download/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/task/download/s3/to_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.274010 phidata-1.7.8/phidata/task/download/url/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/task/download/url/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/task/download/url/to_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/task/download/url/to_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/task/download/url/to_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.274010 phidata-1.7.8/phidata/task/plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/task/plot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.274010 phidata-1.7.8/phidata/task/plot/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/task/plot/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/task/plot/sql/query.py
--rw-r--r--   0 runner    (1001) docker     (123)    12300 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/task/python_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.274010 phidata-1.7.8/phidata/task/run/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/task/run/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.274010 phidata-1.7.8/phidata/task/run/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/task/run/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/task/run/sql/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/task/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/task/task_relatives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.274010 phidata-1.7.8/phidata/task/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/task/upload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.274010 phidata-1.7.8/phidata/task/upload/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/task/upload/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/task/upload/file/to_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/task/upload/file/to_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.278010 phidata-1.7.8/phidata/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/types/airflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/types/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/types/phidata_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/types/run_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.282010 phidata-1.7.8/phidata/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/utils/cli_console.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/utils/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/utils/dttm.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/utils/env_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/utils/env_var.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/utils/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/utils/get_python_objects_from_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/utils/json_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/utils/k8s.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/utils/print_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/utils/workspace_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/utils/yaml_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.282010 phidata-1.7.8/phidata/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/workflow/decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.282010 phidata-1.7.8/phidata/workflow/dev/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/workflow/dev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42342 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/workflow/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/workflow/workflow_relatives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.282010 phidata-1.7.8/phidata/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11316 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/workspace/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-06-21 12:33:02.000000 phidata-1.7.8/phidata/workspace/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.194009 phidata-1.7.8/phidata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-06-21 12:33:30.000000 phidata-1.7.8/phidata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13984 2023-06-21 12:33:30.000000 phidata-1.7.8/phidata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 12:33:30.000000 phidata-1.7.8/phidata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-21 12:33:30.000000 phidata-1.7.8/phidata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-21 12:33:30.000000 phidata-1.7.8/phidata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-21 12:33:02.000000 phidata-1.7.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 12:33:30.282010 phidata-1.7.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-21 12:33:02.000000 phidata-1.7.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:33:30.282010 phidata-1.7.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-21 12:33:02.000000 phidata-1.7.8/tests/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.529434 phidata-1.7.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-07-07 12:54:03.000000 phidata-1.7.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-07-07 12:54:31.529434 phidata-1.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-07-07 12:54:03.000000 phidata-1.7.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.441435 phidata-1.7.9/phidata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.441435 phidata-1.7.9/phidata/airflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/airflow/airflow_installed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.441435 phidata-1.7.9/phidata/airflow/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/airflow/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/airflow/operators/empty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.441435 phidata-1.7.9/phidata/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.445435 phidata-1.7.9/phidata/app/airflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100927 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/airflow/airflow_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30469 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/airflow/airflow_flower.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30508 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/airflow/airflow_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30505 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/airflow/airflow_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30515 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/airflow/airflow_webserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30710 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/airflow/airflow_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.445435 phidata-1.7.9/phidata/app/alertmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/alertmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47889 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/alertmanager/alertmanager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.445435 phidata-1.7.9/phidata/app/amundsen/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/amundsen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48031 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/amundsen/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48032 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/amundsen/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47944 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/amundsen/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.449435 phidata-1.7.9/phidata/app/assistant/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49912 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/assistant/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30166 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/aws_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17164 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/base_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.449435 phidata-1.7.9/phidata/app/cadvisor/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/cadvisor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49678 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/cadvisor/cadvisor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.449435 phidata-1.7.9/phidata/app/databox/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/databox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86151 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/databox/databox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.449435 phidata-1.7.9/phidata/app/db/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/db/base_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/db/db_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.449435 phidata-1.7.9/phidata/app/django/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27483 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/django/django_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30070 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/django/django_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17172 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/docker_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.449435 phidata-1.7.9/phidata/app/elastic/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/elastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/elastic/elastic_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.449435 phidata-1.7.9/phidata/app/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48675 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/elasticsearch/elasticsearch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.449435 phidata-1.7.9/phidata/app/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20266 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/fastapi/fastapi_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.453435 phidata-1.7.9/phidata/app/grafana/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/grafana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49781 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/grafana/grafana.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.453435 phidata-1.7.9/phidata/app/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27093 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/jupyter/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46942 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/jupyter/jupyter_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93432 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/jupyter/jupyter_lab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.453435 phidata-1.7.9/phidata/app/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/k8s/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/k8s/dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/k8s/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37830 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/k8s_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.453435 phidata-1.7.9/phidata/app/mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49110 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/mysql/mysql_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.453435 phidata-1.7.9/phidata/app/neo4j/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/neo4j/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47856 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/neo4j/neo4j.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.453435 phidata-1.7.9/phidata/app/nodeexporter/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/nodeexporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47898 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/nodeexporter/nodeexporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38495 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/phidata_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.453435 phidata-1.7.9/phidata/app/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53156 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/postgres/postgres_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.457435 phidata-1.7.9/phidata/app/prometheus/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/prometheus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49051 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/prometheus/prometheus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.457435 phidata-1.7.9/phidata/app/qdrant/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/qdrant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12372 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/qdrant/qdrant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.457435 phidata-1.7.9/phidata/app/redis/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49058 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/redis/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53296 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/redis/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.457435 phidata-1.7.9/phidata/app/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18424 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/server/api_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58714 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/server/server_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.457435 phidata-1.7.9/phidata/app/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49424 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/spark/spark_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17222 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/spark/spark_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17332 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/spark/spark_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.457435 phidata-1.7.9/phidata/app/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20207 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/streamlit/streamlit_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.461435 phidata-1.7.9/phidata/app/superset/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/superset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71570 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/superset/superset_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22925 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/superset/superset_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/superset/superset_webserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/superset/superset_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22917 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/superset/superset_worker_beat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.461435 phidata-1.7.9/phidata/app/traefik/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/traefik/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115905 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/traefik/crds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48190 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/traefik/ingress_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44972 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/app/traefik/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.461435 phidata-1.7.9/phidata/asset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/asset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.461435 phidata-1.7.9/phidata/asset/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/asset/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/asset/aws/aws_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24787 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/asset/data_asset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.465435 phidata-1.7.9/phidata/asset/local/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/asset/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14564 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/asset/local/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/asset/local/local_asset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.465435 phidata-1.7.9/phidata/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.465435 phidata-1.7.9/phidata/aws/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/athena/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.465435 phidata-1.7.9/phidata/aws/create/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/create/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.465435 phidata-1.7.9/phidata/aws/create/iam/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/create/iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/create/iam/eks_admin_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/create/iam/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23058 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.465435 phidata-1.7.9/phidata/aws/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/enums/manager_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.469435 phidata-1.7.9/phidata/aws/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.469435 phidata-1.7.9/phidata/aws/resource/acm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/acm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10630 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/acm/certificate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.469435 phidata-1.7.9/phidata/aws/resource/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/athena/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.469435 phidata-1.7.9/phidata/aws/resource/cloudformation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/cloudformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10882 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/cloudformation/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.469435 phidata-1.7.9/phidata/aws/resource/ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/ec2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21341 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/ec2/security_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/ec2/subnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/ec2/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.473435 phidata-1.7.9/phidata/aws/resource/ecs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/ecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/ecs/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26253 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/ecs/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19630 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/ecs/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22397 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/ecs/task_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/ecs/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.473435 phidata-1.7.9/phidata/aws/resource/eks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/eks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/eks/addon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30104 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/eks/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13731 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/eks/fargate_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23785 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/eks/kubeconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23742 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/eks/node_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.473435 phidata-1.7.9/phidata/aws/resource/elasticache/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/elasticache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15823 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/elasticache/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/elasticache/subnet_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.473435 phidata-1.7.9/phidata/aws/resource/elb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/elb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/elb/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/elb/load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/elb/target_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.473435 phidata-1.7.9/phidata/aws/resource/emr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/emr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/emr/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.473435 phidata-1.7.9/phidata/aws/resource/glue/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12850 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/glue/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.477435 phidata-1.7.9/phidata/aws/resource/iam/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/iam/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/iam/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9828 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/iam/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.477435 phidata-1.7.9/phidata/aws/resource/rds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/rds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36056 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/rds/db_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35380 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/rds/db_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/rds/db_subnet_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.477435 phidata-1.7.9/phidata/aws/resource/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/s3/bucket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.477435 phidata-1.7.9/phidata/aws/resource/secret/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/secret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11398 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/secret/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/secret/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9688 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/resource/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.477435 phidata-1.7.9/phidata/aws/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21797 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/s3/csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24100 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/s3/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14394 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/s3/dataset_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/s3/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22470 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/aws/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.481435 phidata-1.7.9/phidata/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/checks/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/checks/not_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.481435 phidata-1.7.9/phidata/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/decorators/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/decorators/validate_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.481435 phidata-1.7.9/phidata/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/docker/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/docker/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/docker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/docker/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/docker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/docker/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.485435 phidata-1.7.9/phidata/docker/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/docker/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/docker/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16440 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/docker/resource/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/docker/resource/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14773 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/docker/resource/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/docker/resource/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/docker/resource/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/docker/resource/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/docker/resource/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.485435 phidata-1.7.9/phidata/docker/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/docker/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/docker/utils/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24179 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/docker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.485435 phidata-1.7.9/phidata/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/exceptions/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/exceptions/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/exceptions/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.485435 phidata-1.7.9/phidata/infra/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/infra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/infra/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/infra/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15390 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/infra/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12048 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/infra/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.489435 phidata-1.7.9/phidata/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.489435 phidata-1.7.9/phidata/k8s/create/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/create/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.489435 phidata-1.7.9/phidata/k8s/create/apiextensions_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/create/apiextensions_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.489435 phidata-1.7.9/phidata/k8s/create/apiextensions_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/create/apiextensions_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.489435 phidata-1.7.9/phidata/k8s/create/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/create/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.489435 phidata-1.7.9/phidata/k8s/create/apps/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/create/apps/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/create/apps/v1/deployment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.489435 phidata-1.7.9/phidata/k8s/create/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/create/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/create/common/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/create/common/port.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.493435 phidata-1.7.9/phidata/k8s/create/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/create/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.493435 phidata-1.7.9/phidata/k8s/create/core/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/create/core/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/create/core/v1/config_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/create/core/v1/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/create/core/v1/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/create/core/v1/persistent_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/create/core/v1/persistent_volume_claim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/create/core/v1/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/create/core/v1/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/create/core/v1/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/create/core/v1/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.493435 phidata-1.7.9/phidata/k8s/create/crb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/create/crb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/create/crb/eks_admin_crb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19062 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/create/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/create/kubeconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.493435 phidata-1.7.9/phidata/k8s/create/networking_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/create/networking_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.493435 phidata-1.7.9/phidata/k8s/create/networking_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/create/networking_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/create/networking_k8s_io/v1/ingress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.493435 phidata-1.7.9/phidata/k8s/create/rbac_authorization_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/create/rbac_authorization_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.493435 phidata-1.7.9/phidata/k8s/create/rbac_authorization_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/create/rbac_authorization_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.497434 phidata-1.7.9/phidata/k8s/create/storage_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/create/storage_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.497434 phidata-1.7.9/phidata/k8s/create/storage_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/create/storage_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/create/storage_k8s_io/v1/storage_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.497434 phidata-1.7.9/phidata/k8s/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/enums/api_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/enums/api_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/enums/image_pull_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/enums/kind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/enums/manager_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/enums/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/enums/pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/enums/restart_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/enums/service_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/enums/storage_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/enums/volume_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.501434 phidata-1.7.9/phidata/k8s/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.501434 phidata-1.7.9/phidata/k8s/resource/apiextensions_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/apiextensions_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.501434 phidata-1.7.9/phidata/k8s/resource/apiextensions_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/apiextensions_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15390 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.501434 phidata-1.7.9/phidata/k8s/resource/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.501434 phidata-1.7.9/phidata/k8s/resource/apps/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/apps/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/apps/v1/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/apps/v1/deployment_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.501434 phidata-1.7.9/phidata/k8s/resource/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.505434 phidata-1.7.9/phidata/k8s/resource/core/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/core/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/core/v1/config_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18530 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/core/v1/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/core/v1/local_object_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/core/v1/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/core/v1/node_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/core/v1/object_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/core/v1/persistent_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/core/v1/persistent_volume_claim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/core/v1/pod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/core/v1/pod_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/core/v1/pod_template_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/core/v1/resource_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/core/v1/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18982 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/core/v1/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/core/v1/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/core/v1/toleration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/core/v1/topology_spread_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/core/v1/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/core/v1/volume_node_affinity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13397 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/core/v1/volume_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/kubeconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.505434 phidata-1.7.9/phidata/k8s/resource/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.509434 phidata-1.7.9/phidata/k8s/resource/meta/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/meta/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/meta/v1/label_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/meta/v1/object_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.509434 phidata-1.7.9/phidata/k8s/resource/networking_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/networking_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.509434 phidata-1.7.9/phidata/k8s/resource/networking_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/networking_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10026 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/networking_k8s_io/v1/ingress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.509434 phidata-1.7.9/phidata/k8s/resource/rbac_authorization_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/rbac_authorization_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.509434 phidata-1.7.9/phidata/k8s/resource/rbac_authorization_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/rbac_authorization_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.509434 phidata-1.7.9/phidata/k8s/resource/storage_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/storage_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.509434 phidata-1.7.9/phidata/k8s/resource/storage_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/storage_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10127 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/resource/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.509434 phidata-1.7.9/phidata/k8s/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/utils/pod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43059 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/k8s/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.509434 phidata-1.7.9/phidata/llm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/llm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.513434 phidata-1.7.9/phidata/llm/duckdb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/llm/duckdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/llm/duckdb/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/llm/duckdb/chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/llm/duckdb/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/llm/duckdb/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/llm/duckdb/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/llm/duckdb/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.513434 phidata-1.7.9/phidata/product/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/product/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29505 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/product/data_product.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.513434 phidata-1.7.9/phidata/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/resource/reference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.513434 phidata-1.7.9/phidata/table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.513434 phidata-1.7.9/phidata/table/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/table/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/table/local/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23516 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/table/local/local_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/table/local/parquet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.513434 phidata-1.7.9/phidata/table/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/table/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/table/s3/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/table/s3/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23064 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/table/s3/s3_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.517434 phidata-1.7.9/phidata/table/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/table/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/table/sql/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35497 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/table/sql/sql_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.517434 phidata-1.7.9/phidata/task/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.517434 phidata-1.7.9/phidata/task/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/task/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.517434 phidata-1.7.9/phidata/task/aws/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/task/aws/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/task/aws/athena/run_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.517434 phidata-1.7.9/phidata/task/aws/emr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/task/aws/emr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/task/aws/emr/create_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/task/aws/emr/delete_cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.517434 phidata-1.7.9/phidata/task/aws/glue/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/task/aws/glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/task/aws/glue/start_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/task/decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.517434 phidata-1.7.9/phidata/task/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/task/dev/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.517434 phidata-1.7.9/phidata/task/download/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/task/download/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.517434 phidata-1.7.9/phidata/task/download/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/task/download/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/task/download/s3/to_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.521434 phidata-1.7.9/phidata/task/download/url/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/task/download/url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/task/download/url/to_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/task/download/url/to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/task/download/url/to_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.521434 phidata-1.7.9/phidata/task/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/task/plot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.521434 phidata-1.7.9/phidata/task/plot/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/task/plot/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/task/plot/sql/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12300 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/task/python_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.521434 phidata-1.7.9/phidata/task/run/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/task/run/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.521434 phidata-1.7.9/phidata/task/run/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/task/run/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/task/run/sql/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/task/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/task/task_relatives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.521434 phidata-1.7.9/phidata/task/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/task/upload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.521434 phidata-1.7.9/phidata/task/upload/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/task/upload/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/task/upload/file/to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/task/upload/file/to_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.521434 phidata-1.7.9/phidata/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/types/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/types/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/types/phidata_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/types/run_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.525434 phidata-1.7.9/phidata/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/utils/cli_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/utils/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/utils/dttm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/utils/env_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/utils/env_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/utils/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/utils/get_python_objects_from_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/utils/json_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/utils/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/utils/print_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/utils/workspace_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/utils/yaml_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.525434 phidata-1.7.9/phidata/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/workflow/decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.529434 phidata-1.7.9/phidata/workflow/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/workflow/dev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42342 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/workflow/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/workflow/workflow_relatives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.529434 phidata-1.7.9/phidata/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11316 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/workspace/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-07-07 12:54:03.000000 phidata-1.7.9/phidata/workspace/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.441435 phidata-1.7.9/phidata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-07-07 12:54:31.000000 phidata-1.7.9/phidata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14009 2023-07-07 12:54:31.000000 phidata-1.7.9/phidata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:54:31.000000 phidata-1.7.9/phidata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-07 12:54:31.000000 phidata-1.7.9/phidata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 12:54:31.000000 phidata-1.7.9/phidata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-07 12:54:03.000000 phidata-1.7.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 12:54:31.529434 phidata-1.7.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-07 12:54:03.000000 phidata-1.7.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:54:31.529434 phidata-1.7.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-07 12:54:03.000000 phidata-1.7.9/tests/test_placeholder.py
```

### Comparing `phidata-1.7.8/LICENSE` & `phidata-1.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/PKG-INFO` & `phidata-1.7.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: phidata
-Version: 1.7.8
+Version: 1.7.9
 Summary: Phidata is a toolkit for building applications using OSS
 Author-email: Ashpreet Bedi <ashpreet@phidata.com>
 Project-URL: homepage, https://phidata.com
 Project-URL: documentation, https://docs.phidata.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: aws
 License-File: LICENSE
 
 <h1 align="center">
   phidata
 </h1>
 <p align="center">
-    <em>A toolkit for building applications using open source tools</em>
+    <em>Run open source tools using python</em>
 </p>
 
 <p align="center">
 <a href="https://python.org/pypi/phidata" target="_blank">
     <img src="https://img.shields.io/pypi/v/phidata?color=blue&label=version" alt="version">
 </a>
 <a href="https://github.com/phidatahq/phidata" target="_blank">
@@ -38,19 +38,19 @@
 
 [//]: # (</a>)
 
 </p>
 
 ---
 
-Open source tools can be used to build powerful software, but are difficult to run in production settings.
+### Phidata is a toolkit for building applications with open source tools.
 
-- Phidata makes it easy to run tools like FastApi, Django, Jupyter, Airflow and Superset.
-- Phidata packages these tools into LLM Apps, Web Apps and Data Platforms.
-- Phidata runs your application locally for development and production on AWS, using 1 command.
+- Phidata makes it easy to run tools like FastApi, Django, Jupyter, Streamlit, Airflow and Superset.
+- Use these tools to build LLM Apps, Web Apps and Data Platforms.
+- Run locally for development and production on AWS, with 1 command.
 
 ## 🚀 How it works
 
 - **Create your codebase** from a template using `phi ws create`
 - **Run your app locally** using `phi ws up dev:docker`
 - **Run your app on AWS** using `phi ws up prd:aws`
 
@@ -62,39 +62,32 @@
 - Install [docker desktop](https://docs.docker.com/desktop/install/mac-install/)
 
 ### Setup
 
 Open the `terminal` and create a python virtual environment
 
 ```shell
-python3 -m venv ~/.venvs/aienv
-source ~/.venvs/aienv/bin/activate
+python3 -m venv ~/.venvs/labenv
+source ~/.venvs/labenv/bin/activate
 ```
 
 Install `phidata`
 
 ```shell
 pip install phidata
 ```
 
 ### Define `DockerConfig` that runs a `Jupyter` app
 
-Create a file `resources.py`
-
-```shell
-touch resources.py
-```
-
-Add the following code to `resources.py`
+Create a file `resources.py` and add the following code to it
 
 ```python
 from phidata.app.jupyter import Jupyter
 from phidata.docker.config import DockerConfig
 
-
 dev_docker_config = DockerConfig(
     apps=[
         # -*- Run Jupyter on port 8888
         Jupyter(mount_workspace=True)
     ],
 )
 ```
```

#### html2text {}

```diff
@@ -1,31 +1,30 @@
-Metadata-Version: 2.1 Name: phidata Version: 1.7.8 Summary: Phidata is a
+Metadata-Version: 2.1 Name: phidata Version: 1.7.9 Summary: Phidata is a
 toolkit for building applications using OSS Author-email: Ashpreet Bedi
 phidata.com> Project-URL: homepage, https://phidata.com Project-URL:
 documentation, https://docs.phidata.com Requires-Python: >=3.7 Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: aws License-
 File: LICENSE
                              ****** phidata ******
-          A toolkit for building applications using open source tools
+                      Run open source tools using python
   [version] [pythonversion] [downloads] [build-status] [//]: # ()_[//]:_#_(_
                            [test-status])_[//]:_#_()
---- Open source tools can be used to build powerful software, but are difficult
-to run in production settings. - Phidata makes it easy to run tools like
-FastApi, Django, Jupyter, Airflow and Superset. - Phidata packages these tools
-into LLM Apps, Web Apps and Data Platforms. - Phidata runs your application
-locally for development and production on AWS, using 1 command. ## ð How it
-works - **Create your codebase** from a template using `phi ws create` - **Run
-your app locally** using `phi ws up dev:docker` - **Run your app on AWS** using
-`phi ws up prd:aws` ## Basic Example: Run a Jupyter Notebook ### Requirements -
-python 3.7+ - Install [docker desktop](https://docs.docker.com/desktop/install/
-mac-install/) ### Setup Open the `terminal` and create a python virtual
-environment ```shell python3 -m venv ~/.venvs/aienv source ~/.venvs/aienv/bin/
-activate ``` Install `phidata` ```shell pip install phidata ``` ### Define
-`DockerConfig` that runs a `Jupyter` app Create a file `resources.py` ```shell
-touch resources.py ``` Add the following code to `resources.py` ```python from
+--- ### Phidata is a toolkit for building applications with open source tools.
+- Phidata makes it easy to run tools like FastApi, Django, Jupyter, Streamlit,
+Airflow and Superset. - Use these tools to build LLM Apps, Web Apps and Data
+Platforms. - Run locally for development and production on AWS, with 1 command.
+## ð How it works - **Create your codebase** from a template using `phi ws
+create` - **Run your app locally** using `phi ws up dev:docker` - **Run your
+app on AWS** using `phi ws up prd:aws` ## Basic Example: Run a Jupyter Notebook
+### Requirements - python 3.7+ - Install [docker desktop](https://
+docs.docker.com/desktop/install/mac-install/) ### Setup Open the `terminal` and
+create a python virtual environment ```shell python3 -m venv ~/.venvs/labenv
+source ~/.venvs/labenv/bin/activate ``` Install `phidata` ```shell pip install
+phidata ``` ### Define `DockerConfig` that runs a `Jupyter` app Create a file
+`resources.py` and add the following code to it ```python from
 phidata.app.jupyter import Jupyter from phidata.docker.config import
 DockerConfig dev_docker_config = DockerConfig( apps=[ # -*- Run Jupyter on port
 8888 Jupyter(mount_workspace=True) ], ) ``` ### Start the app ```shell phi
 start resources.py ``` - Open the browser and go to `http://localhost:8888` -
 Password is `admin` ### Stop the app ```shell phi stop resources.py ``` ## More
 Information: - **Documentation**: https://docs.phidata.com - **Questions:**
 Chat with us on Discord - **Email**: help@phidata.com
```

### Comparing `phidata-1.7.8/README.md` & `phidata-1.7.9/phidata.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,25 @@
+Metadata-Version: 2.1
+Name: phidata
+Version: 1.7.9
+Summary: Phidata is a toolkit for building applications using OSS
+Author-email: Ashpreet Bedi <ashpreet@phidata.com>
+Project-URL: homepage, https://phidata.com
+Project-URL: documentation, https://docs.phidata.com
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: aws
+License-File: LICENSE
+
 <h1 align="center">
   phidata
 </h1>
 <p align="center">
-    <em>A toolkit for building applications using open source tools</em>
+    <em>Run open source tools using python</em>
 </p>
 
 <p align="center">
 <a href="https://python.org/pypi/phidata" target="_blank">
     <img src="https://img.shields.io/pypi/v/phidata?color=blue&label=version" alt="version">
 </a>
 <a href="https://github.com/phidatahq/phidata" target="_blank">
@@ -25,19 +38,19 @@
 
 [//]: # (</a>)
 
 </p>
 
 ---
 
-Open source tools can be used to build powerful software, but are difficult to run in production settings.
+### Phidata is a toolkit for building applications with open source tools.
 
-- Phidata makes it easy to run tools like FastApi, Django, Jupyter, Airflow and Superset.
-- Phidata packages these tools into LLM Apps, Web Apps and Data Platforms.
-- Phidata runs your application locally for development and production on AWS, using 1 command.
+- Phidata makes it easy to run tools like FastApi, Django, Jupyter, Streamlit, Airflow and Superset.
+- Use these tools to build LLM Apps, Web Apps and Data Platforms.
+- Run locally for development and production on AWS, with 1 command.
 
 ## 🚀 How it works
 
 - **Create your codebase** from a template using `phi ws create`
 - **Run your app locally** using `phi ws up dev:docker`
 - **Run your app on AWS** using `phi ws up prd:aws`
 
@@ -49,39 +62,32 @@
 - Install [docker desktop](https://docs.docker.com/desktop/install/mac-install/)
 
 ### Setup
 
 Open the `terminal` and create a python virtual environment
 
 ```shell
-python3 -m venv ~/.venvs/aienv
-source ~/.venvs/aienv/bin/activate
+python3 -m venv ~/.venvs/labenv
+source ~/.venvs/labenv/bin/activate
 ```
 
 Install `phidata`
 
 ```shell
 pip install phidata
 ```
 
 ### Define `DockerConfig` that runs a `Jupyter` app
 
-Create a file `resources.py`
-
-```shell
-touch resources.py
-```
-
-Add the following code to `resources.py`
+Create a file `resources.py` and add the following code to it
 
 ```python
 from phidata.app.jupyter import Jupyter
 from phidata.docker.config import DockerConfig
 
-
 dev_docker_config = DockerConfig(
     apps=[
         # -*- Run Jupyter on port 8888
         Jupyter(mount_workspace=True)
     ],
 )
 ```
```

#### html2text {}

```diff
@@ -1,25 +1,30 @@
+Metadata-Version: 2.1 Name: phidata Version: 1.7.9 Summary: Phidata is a
+toolkit for building applications using OSS Author-email: Ashpreet Bedi
+phidata.com> Project-URL: homepage, https://phidata.com Project-URL:
+documentation, https://docs.phidata.com Requires-Python: >=3.7 Description-
+Content-Type: text/markdown Provides-Extra: dev Provides-Extra: aws License-
+File: LICENSE
                              ****** phidata ******
-          A toolkit for building applications using open source tools
+                      Run open source tools using python
   [version] [pythonversion] [downloads] [build-status] [//]: # ()_[//]:_#_(_
                            [test-status])_[//]:_#_()
---- Open source tools can be used to build powerful software, but are difficult
-to run in production settings. - Phidata makes it easy to run tools like
-FastApi, Django, Jupyter, Airflow and Superset. - Phidata packages these tools
-into LLM Apps, Web Apps and Data Platforms. - Phidata runs your application
-locally for development and production on AWS, using 1 command. ## ð How it
-works - **Create your codebase** from a template using `phi ws create` - **Run
-your app locally** using `phi ws up dev:docker` - **Run your app on AWS** using
-`phi ws up prd:aws` ## Basic Example: Run a Jupyter Notebook ### Requirements -
-python 3.7+ - Install [docker desktop](https://docs.docker.com/desktop/install/
-mac-install/) ### Setup Open the `terminal` and create a python virtual
-environment ```shell python3 -m venv ~/.venvs/aienv source ~/.venvs/aienv/bin/
-activate ``` Install `phidata` ```shell pip install phidata ``` ### Define
-`DockerConfig` that runs a `Jupyter` app Create a file `resources.py` ```shell
-touch resources.py ``` Add the following code to `resources.py` ```python from
+--- ### Phidata is a toolkit for building applications with open source tools.
+- Phidata makes it easy to run tools like FastApi, Django, Jupyter, Streamlit,
+Airflow and Superset. - Use these tools to build LLM Apps, Web Apps and Data
+Platforms. - Run locally for development and production on AWS, with 1 command.
+## ð How it works - **Create your codebase** from a template using `phi ws
+create` - **Run your app locally** using `phi ws up dev:docker` - **Run your
+app on AWS** using `phi ws up prd:aws` ## Basic Example: Run a Jupyter Notebook
+### Requirements - python 3.7+ - Install [docker desktop](https://
+docs.docker.com/desktop/install/mac-install/) ### Setup Open the `terminal` and
+create a python virtual environment ```shell python3 -m venv ~/.venvs/labenv
+source ~/.venvs/labenv/bin/activate ``` Install `phidata` ```shell pip install
+phidata ``` ### Define `DockerConfig` that runs a `Jupyter` app Create a file
+`resources.py` and add the following code to it ```python from
 phidata.app.jupyter import Jupyter from phidata.docker.config import
 DockerConfig dev_docker_config = DockerConfig( apps=[ # -*- Run Jupyter on port
 8888 Jupyter(mount_workspace=True) ], ) ``` ### Start the app ```shell phi
 start resources.py ``` - Open the browser and go to `http://localhost:8888` -
 Password is `admin` ### Stop the app ```shell phi stop resources.py ``` ## More
 Information: - **Documentation**: https://docs.phidata.com - **Questions:**
 Chat with us on Discord - **Email**: help@phidata.com
```

### Comparing `phidata-1.7.8/phidata/airflow/operators/empty.py` & `phidata-1.7.9/phidata/airflow/operators/empty.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/airflow/airflow_base.py` & `phidata-1.7.9/phidata/app/airflow/airflow_base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/airflow/airflow_flower.py` & `phidata-1.7.9/phidata/app/airflow/airflow_flower.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/airflow/airflow_manager.py` & `phidata-1.7.9/phidata/app/airflow/airflow_manager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/airflow/airflow_scheduler.py` & `phidata-1.7.9/phidata/app/airflow/airflow_scheduler.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/airflow/airflow_webserver.py` & `phidata-1.7.9/phidata/app/airflow/airflow_webserver.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/airflow/airflow_worker.py` & `phidata-1.7.9/phidata/app/airflow/airflow_worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/alertmanager/alertmanager.py` & `phidata-1.7.9/phidata/app/alertmanager/alertmanager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/amundsen/frontend.py` & `phidata-1.7.9/phidata/app/amundsen/frontend.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/amundsen/metadata.py` & `phidata-1.7.9/phidata/app/amundsen/metadata.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/amundsen/search.py` & `phidata-1.7.9/phidata/app/amundsen/search.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/assistant/assistant.py` & `phidata-1.7.9/phidata/app/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/aws_app.py` & `phidata-1.7.9/phidata/app/aws_app.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/base_app.py` & `phidata-1.7.9/phidata/app/base_app.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/cadvisor/cadvisor.py` & `phidata-1.7.9/phidata/app/cadvisor/cadvisor.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/databox/databox.py` & `phidata-1.7.9/phidata/app/databox/databox.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/db/base_db.py` & `phidata-1.7.9/phidata/app/db/base_db.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/django/django_app.py` & `phidata-1.7.9/phidata/app/django/django_app.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/django/django_backup.py` & `phidata-1.7.9/phidata/app/django/django_backup.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/docker_app.py` & `phidata-1.7.9/phidata/app/docker_app.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/elastic/elastic_app.py` & `phidata-1.7.9/phidata/app/elastic/elastic_app.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/elasticsearch/elasticsearch.py` & `phidata-1.7.9/phidata/app/elasticsearch/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/fastapi/fastapi_server.py` & `phidata-1.7.9/phidata/app/fastapi/fastapi_server.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/grafana/grafana.py` & `phidata-1.7.9/phidata/app/grafana/grafana.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/group.py` & `phidata-1.7.9/phidata/app/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/jupyter/jupyter.py` & `phidata-1.7.9/phidata/app/jupyter/jupyter.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/jupyter/jupyter_hub.py` & `phidata-1.7.9/phidata/app/jupyter/jupyter_hub.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/jupyter/jupyter_lab.py` & `phidata-1.7.9/phidata/app/jupyter/jupyter_lab.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/k8s/app.py` & `phidata-1.7.9/phidata/app/k8s/app.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/k8s/dir.py` & `phidata-1.7.9/phidata/app/k8s/dir.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/k8s/url.py` & `phidata-1.7.9/phidata/app/k8s/url.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/k8s_app.py` & `phidata-1.7.9/phidata/app/k8s_app.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/mysql/mysql_db.py` & `phidata-1.7.9/phidata/app/mysql/mysql_db.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/neo4j/neo4j.py` & `phidata-1.7.9/phidata/app/neo4j/neo4j.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/nodeexporter/nodeexporter.py` & `phidata-1.7.9/phidata/app/nodeexporter/nodeexporter.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/phidata_app.py` & `phidata-1.7.9/phidata/app/phidata_app.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/postgres/postgres_db.py` & `phidata-1.7.9/phidata/app/postgres/postgres_db.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/prometheus/prometheus.py` & `phidata-1.7.9/phidata/app/prometheus/prometheus.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/qdrant/qdrant.py` & `phidata-1.7.9/phidata/app/streamlit/streamlit_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,31 +10,31 @@
     ImagePullPolicy,
     RestartPolicy,
     ServiceType,
 )
 from phidata.utils.log import logger
 
 
-class QdrantArgs(AwsAppArgs, DockerAppArgs, K8sAppArgs):
+class StreamlitAppArgs(AwsAppArgs, DockerAppArgs, K8sAppArgs):
     pass
 
 
-class Qdrant(AwsApp, DockerApp, K8sApp):
+class StreamlitApp(AwsApp, DockerApp, K8sApp):
     def __init__(
         self,
-        name: str = "qdrant",
+        name: str = "streamlit",
         version: str = "1",
         enabled: bool = True,
         # -*- Image Configuration,
         # Image can be provided as a DockerImage object or as image_name:image_tag
         image: Optional[Any] = None,
-        image_name: str = "qdrant/qdrant",
-        image_tag: str = "v1.2.2",
-        entrypoint: Optional[Union[str, List[str]]] = None,
-        command: Optional[Union[str, List]] = None,
+        image_name: str = "phidata/streamlit",
+        image_tag: str = "1.23",
+        entrypoint: Optional[Union[str, List]] = None,
+        command: Optional[Union[str, List]] = "streamlit hello",
         # -*- Debug Mode
         debug_mode: bool = False,
         # -*- Python Configuration,
         # Install python dependencies using a requirements.txt file,
         install_requirements: bool = False,
         # Path to the requirements.txt file relative to the workspace_root,
         requirements_file: str = "requirements.txt",
@@ -56,19 +56,19 @@
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # -*- Container Ports,
         # Open a container port if open_container_port=True,
         open_container_port: bool = True,
         # Port number on the container,
-        container_port: int = 6333,
+        container_port: int = 9095,
         # Port name (only used by the K8sContainer),
         container_port_name: str = "http",
         # Host port to map to the container port,
-        container_host_port: int = 6333,
+        container_host_port: int = 9095,
         # -*- Workspace Volume,
         # Mount the workspace directory on the container,
         mount_workspace: bool = False,
         workspace_volume_name: Optional[str] = None,
         workspace_volume_type: Optional[WorkspaceVolumeType] = None,
         # Path to mount the workspace volume inside the container,
         workspace_dir_container_path: str = "/usr/local/app",
@@ -159,15 +159,15 @@
         topology_spread_when_unsatisfiable: Optional[str] = None,
         # -*- Service Configuration,
         create_service: bool = False,
         service_name: Optional[str] = None,
         # Type: ServiceType,
         service_type: Optional[Any] = None,
         # The port exposed by the service.,
-        service_port: int = 6333,
+        service_port: int = 9095,
         # The node_port exposed by the service if service_type = ServiceType.NODE_PORT,
         service_node_port: Optional[int] = None,
         # The target_port is the port to access on the pods targeted by the service.,
         # It can be the port number or port name on the pod.,
         service_target_port: Optional[Union[str, int]] = None,
         # Extra ports exposed by the webserver service. Type: List[CreatePort],
         service_ports: Optional[List[Any]] = None,
@@ -207,14 +207,16 @@
         # Type: CreateClusterRoleBinding,
         cluster_role_binding: Optional[Any] = None,
         # -*- AWS Configuration,
         aws_subnets: Optional[List[str]] = None,
         aws_security_groups: Optional[List[Any]] = None,
         # -*- ECS Configuration,
         ecs_cluster: Optional[Any] = None,
+        # If ecs_cluster is None, create a new cluster with ecs_cluster_name,
+        ecs_cluster_name: Optional[str] = None,
         ecs_launch_type: str = "FARGATE",
         ecs_task_cpu: str = "1024",
         ecs_task_memory: str = "2048",
         ecs_service_count: int = 1,
         assign_public_ip: bool = True,
         ecs_enable_exec: bool = True,
         # -*- LoadBalancer Configuration,
@@ -264,16 +266,17 @@
         use_cache: bool = True,
         #  -*- Other args,
         print_env_on_load: bool = False,
         # Extra kwargs used to capture additional args,
         **extra_kwargs,
     ):
         super().__init__()
+
         try:
-            self.args: QdrantArgs = QdrantArgs(
+            self.args: StreamlitAppArgs = StreamlitAppArgs(
                 name=name,
                 version=version,
                 enabled=enabled,
                 image=image,
                 image_name=image_name,
                 image_tag=image_tag,
                 entrypoint=entrypoint,
@@ -356,14 +359,15 @@
                 cr_name=cr_name,
                 cluster_role=cluster_role,
                 crb_name=crb_name,
                 cluster_role_binding=cluster_role_binding,
                 aws_subnets=aws_subnets,
                 aws_security_groups=aws_security_groups,
                 ecs_cluster=ecs_cluster,
+                ecs_cluster_name=ecs_cluster_name,
                 ecs_launch_type=ecs_launch_type,
                 ecs_task_cpu=ecs_task_cpu,
                 ecs_task_memory=ecs_task_memory,
                 ecs_service_count=ecs_service_count,
                 assign_public_ip=assign_public_ip,
                 ecs_enable_exec=ecs_enable_exec,
                 load_balancer=load_balancer,
```

### Comparing `phidata-1.7.8/phidata/app/redis/redis.py` & `phidata-1.7.9/phidata/app/redis/redis.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/redis/stack.py` & `phidata-1.7.9/phidata/app/redis/stack.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/server/api_server.py` & `phidata-1.7.9/phidata/app/server/api_server.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/server/server_base.py` & `phidata-1.7.9/phidata/app/server/server_base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/spark/spark_base.py` & `phidata-1.7.9/phidata/app/spark/spark_base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/spark/spark_driver.py` & `phidata-1.7.9/phidata/app/spark/spark_driver.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/spark/spark_worker.py` & `phidata-1.7.9/phidata/app/spark/spark_worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/streamlit/streamlit_app.py` & `phidata-1.7.9/phidata/app/superset/superset_webserver.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,194 +1,276 @@
 from pathlib import Path
 from typing import Optional, Dict, Any, List, Union
 
-from phidata.app.aws_app import AwsApp, AwsAppArgs
-from phidata.app.base_app import WorkspaceVolumeType
-from phidata.app.docker_app import DockerApp, DockerAppArgs
-from phidata.app.k8s_app import (
-    K8sApp,
-    K8sAppArgs,
+from phidata.app.superset.superset_base import (
+    SupersetBase,
+    ServiceType,
+    DbApp,
+    WorkspaceVolumeType,
     ImagePullPolicy,
     RestartPolicy,
-    ServiceType,
 )
-from phidata.utils.log import logger
-
 
-class StreamlitAppArgs(AwsAppArgs, DockerAppArgs, K8sAppArgs):
-    pass
 
-
-class StreamlitApp(AwsApp, DockerApp, K8sApp):
+class SupersetWebserver(SupersetBase):
     def __init__(
         self,
-        name: str = "streamlit",
+        name: str = "superset-ws",
         version: str = "1",
         enabled: bool = True,
         # -*- Image Configuration,
         # Image can be provided as a DockerImage object or as image_name:image_tag
         image: Optional[Any] = None,
-        image_name: str = "phidata/streamlit",
-        image_tag: str = "1.23",
+        image_name: str = "phidata/superset",
+        image_tag: str = "2.0.1",
         entrypoint: Optional[Union[str, List]] = None,
-        command: Optional[Union[str, List]] = "streamlit hello",
-        # -*- Debug Mode
-        debug_mode: bool = False,
-        # -*- Python Configuration,
+        command: Optional[Union[str, List]] = "webserver",
         # Install python dependencies using a requirements.txt file,
+        # Sets the REQUIREMENTS_LOCAL & REQUIREMENTS_FILE_PATH env var to requirements_file,
         install_requirements: bool = False,
         # Path to the requirements.txt file relative to the workspace_root,
         requirements_file: str = "requirements.txt",
+        # -*- Superset Configuration,
+        # Configure Superset db,
+        wait_for_db: bool = False,
+        # Connect to database using a DbApp,
+        db_app: Optional[DbApp] = None,
+        # Provide database connection details manually,
+        # db_user can be provided here or as the,
+        # DATABASE_USER env var in the secrets_file,
+        db_user: Optional[str] = None,
+        # db_password can be provided here or as the,
+        # DATABASE_PASSWORD env var in the secrets_file,
+        db_password: Optional[str] = None,
+        # db_schema can be provided here or as the,
+        # DATABASE_DB env var in the secrets_file,
+        db_schema: Optional[str] = None,
+        # db_host can be provided here or as the,
+        # DATABASE_HOST env var in the secrets_file,
+        db_host: Optional[str] = None,
+        # db_port can be provided here or as the,
+        # DATABASE_PORT env var in the secrets_file,
+        db_port: Optional[int] = None,
+        # db_driver can be provided here or as the,
+        # DATABASE_DIALECT env var in the secrets_file,
+        db_dialect: Optional[str] = None,
+        # Configure superset redis,
+        wait_for_redis: bool = False,
+        # Connect to redis using a PhidataApp,
+        redis_app: Optional[DbApp] = None,
+        # redis_host can be provided here or as the,
+        # REDIS_HOST env var in the secrets_file,
+        redis_host: Optional[str] = None,
+        # redis_port can be provided here or as the,
+        # REDIS_PORT env var in the secrets_file,
+        redis_port: Optional[int] = None,
+        # redis_driver can be provided here or as the,
+        # REDIS_DRIVER env var in the secrets_file,
+        redis_driver: Optional[str] = None,
+        # -*- Container Configuration,
+        container_name: Optional[str] = None,
+        # Set the SUPERSET_CONFIG_PATH env var,
+        superset_config_path: Optional[str] = None,
+        # Set the FLASK_ENV env var,
+        flask_env: str = "production",
+        # Set the SUPERSET_ENV env var,
+        superset_env: str = "production",
         # Set the PYTHONPATH env var,
-        set_python_path: bool = False,
-        # Manually provide the PYTHONPATH,
+        # defaults to "/app/pythonpath:/app/docker/pythonpath_dev",
         python_path: Optional[str] = None,
-        # Add paths to the PYTHONPATH env var,
-        # If python_path is provided, this value is ignored,
-        add_python_paths: Optional[List[str]] = None,
-        # -*- Container Environment,
-        # Add env variables to container,
+        # Add labels to the container,
+        container_labels: Optional[Dict[str, Any]] = None,
+        # Container env passed to the PhidataApp,
+        # Add env variables to container env,
         env: Optional[Dict[str, Any]] = None,
         # Read env variables from a file in yaml format,
         env_file: Optional[Path] = None,
-        # Add secret variables to container,
+        # Container secrets,
+        # Add secret variables to container env,
         secrets: Optional[Dict[str, Any]] = None,
         # Read secret variables from a file in yaml format,
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
-        # -*- Container Ports,
+        # Container ports,
         # Open a container port if open_container_port=True,
-        open_container_port: bool = True,
+        open_container_port: bool = False,
         # Port number on the container,
-        container_port: int = 9095,
-        # Port name (only used by the K8sContainer),
+        container_port: int = 8000,
+        # Port name: Only used by the K8sContainer,
         container_port_name: str = "http",
-        # Host port to map to the container port,
-        container_host_port: int = 9095,
-        # -*- Workspace Volume,
+        # Host port: Only used by the DockerContainer,
+        container_host_port: int = 8000,
+        # Open the app port if open_app_port=True,
+        open_app_port: bool = True,
+        # App port number on the container,
+        # Set the SUPERSET_PORT env var,
+        app_port: int = 8088,
+        # Only used by the K8sContainer,
+        app_port_name: str = "app",
+        # Only used by the DockerContainer,
+        app_host_port: int = 8088,
+        # Container volumes,
         # Mount the workspace directory on the container,
         mount_workspace: bool = False,
         workspace_volume_name: Optional[str] = None,
         workspace_volume_type: Optional[WorkspaceVolumeType] = None,
-        # Path to mount the workspace volume inside the container,
-        workspace_dir_container_path: str = "/usr/local/app",
-        # Add the workspace name to the container path,
-        add_workspace_name_to_container_path: bool = False,
-        # -*- If workspace_volume_type=WorkspaceVolumeType.HostPath,
-        # Mount workspace_dir to workspace_dir_container_path,
-        # If None, use the workspace_root,
-        workspace_dir: Optional[str] = None,
-        # -*- Container Configuration,
-        container_name: Optional[str] = None,
+        # Path to mount the workspace volume,
+        # This is the parent directory for the workspace on the container,
+        # i.e. the ws is mounted as a subdir in this dir,
+        # eg: if ws name is: idata, workspace_root would be: /mnt/workspaces/idata,
+        workspace_volume_container_path: str = "/mnt/workspaces",
+        # How to mount the workspace volume,
+        # Option 1: Mount the workspace from the host machine,
+        # If None, use the workspace_root_path,
+        # Note: This is the default on DockerContainers. We assume that DockerContainers,
+        # are running locally on the user's machine so the local workspace_root_path,
+        # is mounted to the workspace_volume_container_path,
+        workspace_volume_host_path: Optional[str] = None,
+        # Option 2: Load the workspace from git using a git-sync sidecar container,
+        # This the default on K8sContainers.,
+        create_git_sync_sidecar: bool = False,
+        # Required to create an initial copy of the workspace,
+        create_git_sync_init_container: bool = True,
+        git_sync_image_name: str = "k8s.gcr.io/git-sync",
+        git_sync_image_tag: str = "v3.1.1",
+        git_sync_repo: Optional[str] = None,
+        git_sync_branch: Optional[str] = None,
+        git_sync_wait: int = 1,
+        # Configure resources volume. Only on docker,
+        # Superset resources directory relative to the workspace_root,
+        # This directory contains all the files required by superset.,
+        # eg: docker-bootstrap.sh,
+        # This dir is mounted to the `/app/docker` directory on the container,
+        mount_resources: bool = False,
+        resources_dir: str = "workspace/superset",
+        resources_dir_container_path: str = "/app/docker",
+        resources_volume_name: Optional[str] = None,
+        # -*- Docker configuration,
         # Run container in the background and return a Container object.,
         container_detach: bool = True,
         # Enable auto-removal of the container on daemon side when the container’s process exits.,
         container_auto_remove: bool = True,
         # Remove the container when it has finished running. Default: True.,
         container_remove: bool = True,
         # Username or UID to run commands as inside the container.,
         container_user: Optional[Union[str, int]] = None,
         # Keep STDIN open even if not attached.,
         container_stdin_open: bool = True,
-        # Return logs from STDOUT when container_detach=False.,
-        container_stdout: Optional[bool] = True,
-        # Return logs from STDERR when container_detach=False.,
-        container_stderr: Optional[bool] = True,
         container_tty: bool = True,
         # Specify a test to perform to check that the container is healthy.,
         container_healthcheck: Optional[Dict[str, Any]] = None,
         # Optional hostname for the container.,
         container_hostname: Optional[str] = None,
         # Platform in the format os[/arch[/variant]].,
         container_platform: Optional[str] = None,
         # Path to the working directory.,
         container_working_dir: Optional[str] = None,
-        # Add labels to the container,
-        container_labels: Optional[Dict[str, str]] = None,
         # Restart the container when it exits. Configured as a dictionary with keys:,
         # Name: One of on-failure, or always.,
         # MaximumRetryCount: Number of times to restart the container on failure.,
         # For example: {"Name": "on-failure", "MaximumRetryCount": 5},
-        container_restart_policy: Optional[Dict[str, Any]] = None,
+        container_restart_policy_docker: Optional[Dict[str, Any]] = None,
         # Add volumes to DockerContainer,
         # container_volumes is a dictionary which adds the volumes to mount,
         # inside the container. The key is either the host path or a volume name,,
         # and the value is a dictionary with 2 keys:,
         #   bind - The path to mount the volume inside the container,
         #   mode - Either rw to mount the volume read/write, or ro to mount it read-only.,
         # For example:,
         # {,
         #   '/home/user1/': {'bind': '/mnt/vol2', 'mode': 'rw'},,
         #   '/var/www': {'bind': '/mnt/vol1', 'mode': 'ro'},
         # },
-        container_volumes: Optional[Dict[str, dict]] = None,
+        container_volumes_docker: Optional[Dict[str, dict]] = None,
         # Add ports to DockerContainer,
         # The keys of the dictionary are the ports to bind inside the container,,
         # either as an integer or a string in the form port/protocol, where the protocol is either tcp, udp.,
         # The values of the dictionary are the corresponding ports to open on the host, which can be either:,
         #   - The port number, as an integer.,
         #       For example, {'2222/tcp': 3333} will expose port 2222 inside the container as port 3333 on the host.,
         #   - None, to assign a random host port. For example, {'2222/tcp': None}.,
         #   - A tuple of (address, port) if you want to specify the host interface.,
         #       For example, {'1111/tcp': ('127.0.0.1', 1111)}.,
         #   - A list of integers, if you want to bind multiple host ports to a single container port.,
         #       For example, {'1111/tcp': [1234, 4567]}.,
-        container_ports: Optional[Dict[str, Any]] = None,
-        # -*- Pod Configuration,
+        container_ports_docker: Optional[Dict[str, Any]] = None,
+        # -*- K8s configuration,
+        # K8s Deployment configuration,
+        replicas: int = 1,
         pod_name: Optional[str] = None,
-        pod_annotations: Optional[Dict[str, str]] = None,
-        pod_node_selector: Optional[Dict[str, str]] = None,
-        # -*- Secret Configuration,
+        deploy_name: Optional[str] = None,
         secret_name: Optional[str] = None,
-        # -*- Configmap Configuration,
         configmap_name: Optional[str] = None,
-        # -*- Deployment Configuration,
-        replicas: int = 1,
-        deploy_name: Optional[str] = None,
         # Type: ImagePullPolicy,
-        image_pull_policy: Optional[Any] = None,
+        image_pull_policy: Optional[ImagePullPolicy] = None,
+        pod_annotations: Optional[Dict[str, str]] = None,
+        pod_node_selector: Optional[Dict[str, str]] = None,
         # Type: RestartPolicy,
-        deploy_restart_policy: Optional[Any] = None,
+        deploy_restart_policy: Optional[RestartPolicy] = None,
         deploy_labels: Optional[Dict[str, Any]] = None,
         termination_grace_period_seconds: Optional[int] = None,
-        # Key to spread the pods across a topology,
+        # How to spread the deployment across a topology,
+        # Key to spread the pods across,
         topology_spread_key: Optional[str] = None,
         # The degree to which pods may be unevenly distributed,
         topology_spread_max_skew: Optional[int] = None,
         # How to deal with a pod if it doesn't satisfy the spread constraint.,
         topology_spread_when_unsatisfiable: Optional[str] = None,
-        # -*- Service Configuration,
+        # K8s Service Configuration,
         create_service: bool = False,
         service_name: Optional[str] = None,
         # Type: ServiceType,
         service_type: Optional[Any] = None,
         # The port exposed by the service.,
-        service_port: int = 9095,
+        service_port: int = 8000,
         # The node_port exposed by the service if service_type = ServiceType.NODE_PORT,
         service_node_port: Optional[int] = None,
         # The target_port is the port to access on the pods targeted by the service.,
         # It can be the port number or port name on the pod.,
         service_target_port: Optional[Union[str, int]] = None,
         # Extra ports exposed by the webserver service. Type: List[CreatePort],
         service_ports: Optional[List[Any]] = None,
+        # Service labels,
         service_labels: Optional[Dict[str, Any]] = None,
+        # Service annotations,
         service_annotations: Optional[Dict[str, str]] = None,
         # If ServiceType == ServiceType.LoadBalancer,
         service_health_check_node_port: Optional[int] = None,
         service_internal_traffic_policy: Optional[str] = None,
         service_load_balancer_class: Optional[str] = None,
         service_load_balancer_ip: Optional[str] = None,
         service_load_balancer_source_ranges: Optional[List[str]] = None,
         service_allocate_load_balancer_node_ports: Optional[bool] = None,
-        # -*- Ingress Configuration,
-        create_ingress: bool = False,
-        ingress_name: Optional[str] = None,
-        ingress_annotations: Optional[Dict[str, str]] = None,
-        # -*- RBAC Configuration,
+        # App Service Configuration,
+        create_app_service: bool = True,
+        # Configure the app service,
+        app_svc_name: Optional[str] = None,
+        app_svc_type: Optional[ServiceType] = None,
+        # The port that will be exposed by the service.,
+        app_svc_port: int = 8088,
+        # The node_port that will be exposed by the service if app_svc_type = ServiceType.NODE_PORT,
+        app_node_port: Optional[int] = None,
+        # The app_target_port is the port to access on the pods targeted by the service.,
+        # It can be the port number or port name on the pod.,
+        app_target_port: Optional[Union[str, int]] = None,
+        # Extra ports exposed by the app service,
+        app_svc_ports: Optional[List[Any]] = None,
+        # Add labels to app service,
+        app_svc_labels: Optional[Dict[str, Any]] = None,
+        # Add annotations to app service,
+        app_svc_annotations: Optional[Dict[str, str]] = None,
+        # If ServiceType == LoadBalancer,
+        app_svc_health_check_node_port: Optional[int] = None,
+        app_svc_internal_taffic_policy: Optional[str] = None,
+        app_svc_load_balancer_class: Optional[str] = None,
+        app_svc_load_balancer_ip: Optional[str] = None,
+        app_svc_load_balancer_source_ranges: Optional[List[str]] = None,
+        app_svc_allocate_load_balancer_node_ports: Optional[bool] = None,
+        # K8s RBAC Configuration,
         use_rbac: bool = False,
         # Create a Namespace with name ns_name & default values,
         ns_name: Optional[str] = None,
         # or Provide the full Namespace definition,
         # Type: CreateNamespace,
         namespace: Optional[Any] = None,
         # Create a ServiceAccount with name sa_name & default values,
@@ -202,210 +284,185 @@
         # Type: CreateClusterRole,
         cluster_role: Optional[Any] = None,
         # Create a ClusterRoleBinding with name crb_name & default values,
         crb_name: Optional[str] = None,
         # or Provide the full ClusterRoleBinding definition,
         # Type: CreateClusterRoleBinding,
         cluster_role_binding: Optional[Any] = None,
-        # -*- AWS Configuration,
-        aws_subnets: Optional[List[str]] = None,
-        aws_security_groups: Optional[List[Any]] = None,
-        # -*- ECS Configuration,
-        ecs_cluster: Optional[Any] = None,
-        # If ecs_cluster is None, create a new cluster with ecs_cluster_name,
-        ecs_cluster_name: Optional[str] = None,
-        ecs_launch_type: str = "FARGATE",
-        ecs_task_cpu: str = "1024",
-        ecs_task_memory: str = "2048",
-        ecs_service_count: int = 1,
-        assign_public_ip: bool = True,
-        ecs_enable_exec: bool = True,
-        # -*- LoadBalancer Configuration,
-        load_balancer: Optional[Any] = None,
-        listener: Optional[Any] = None,
-        # Create a load balancer if load_balancer is None,
-        create_load_balancer: bool = False,
-        # HTTP or HTTPS,
-        load_balancer_protocol: str = "HTTP",
-        load_balancer_security_groups: Optional[List[Any]] = None,
-        # Default 80 for HTTP and 443 for HTTPS,
-        load_balancer_port: Optional[int] = None,
-        load_balancer_certificate: Optional[Any] = None,
-        load_balancer_certificate_arn: Optional[str] = None,
-        # -*- TargetGroup Configuration,
-        target_group: Optional[Any] = None,
-        # HTTP or HTTPS,
-        target_group_protocol: str = "HTTP",
-        # Default 80 for HTTP and 443 for HTTPS,
-        target_group_port: Optional[int] = None,
-        target_group_type: str = "ip",
-        health_check_protocol: Optional[str] = None,
-        health_check_port: Optional[str] = None,
-        health_check_enabled: Optional[bool] = None,
-        health_check_path: Optional[str] = None,
-        health_check_interval_seconds: Optional[int] = None,
-        health_check_timeout_seconds: Optional[int] = None,
-        healthy_threshold_count: Optional[int] = None,
-        unhealthy_threshold_count: Optional[int] = None,
-        #  -*- Resource Control,
-        skip_create: bool = False,
-        skip_read: bool = False,
-        skip_update: bool = False,
-        recreate_on_update: bool = False,
-        skip_delete: bool = False,
-        wait_for_creation: bool = True,
-        wait_for_update: bool = True,
-        wait_for_deletion: bool = True,
-        waiter_delay: int = 30,
-        waiter_max_attempts: int = 50,
-        #  -*- Save Resources to output directory,
-        # If True, save the resources to files,
-        save_output: bool = False,
-        # The resource directory for the output files,
-        resource_dir: Optional[str] = None,
-        # Skip creation if resource with the same name is active,
+        # Add additional Kubernetes resources to the App,
+        # Type: CreateSecret,
+        extra_secrets: Optional[List[Any]] = None,
+        # Type: CreateConfigMap,
+        extra_configmaps: Optional[List[Any]] = None,
+        # Type: CreateService,
+        extra_services: Optional[List[Any]] = None,
+        # Type: CreateDeployment,
+        extra_deployments: Optional[List[Any]] = None,
+        # Type: CreatePersistentVolume,
+        extra_pvs: Optional[List[Any]] = None,
+        # Type: CreatePVC,
+        extra_pvcs: Optional[List[Any]] = None,
+        # Type: CreateContainer,
+        extra_containers: Optional[List[Any]] = None,
+        # Type: CreateContainer,
+        extra_init_containers: Optional[List[Any]] = None,
+        # Type: CreatePort,
+        extra_ports: Optional[List[Any]] = None,
+        # Type: CreateVolume,
+        extra_volumes: Optional[List[Any]] = None,
+        # Type: CreateStorageClass,
+        extra_storage_classes: Optional[List[Any]] = None,
+        # Type: CreateCustomObject,
+        extra_custom_objects: Optional[List[Any]] = None,
+        # Type: CreateCustomResourceDefinition,
+        extra_crds: Optional[List[Any]] = None,
+        # Other args,
+        print_env_on_load: bool = True,
+        # If True, skip resource creation if active resources with the same name exist.,
         use_cache: bool = True,
-        #  -*- Other args,
-        print_env_on_load: bool = False,
-        # Extra kwargs used to capture additional args,
-        **extra_kwargs,
+        # Set SUPERSET_LOAD_EXAMPLES = "yes",
+        load_examples: bool = False,
+        **kwargs,
     ):
-        super().__init__()
-
-        try:
-            self.args: StreamlitAppArgs = StreamlitAppArgs(
-                name=name,
-                version=version,
-                enabled=enabled,
-                image=image,
-                image_name=image_name,
-                image_tag=image_tag,
-                entrypoint=entrypoint,
-                command=command,
-                debug_mode=debug_mode,
-                install_requirements=install_requirements,
-                requirements_file=requirements_file,
-                set_python_path=set_python_path,
-                python_path=python_path,
-                add_python_paths=add_python_paths,
-                env=env,
-                env_file=env_file,
-                secrets=secrets,
-                secrets_file=secrets_file,
-                aws_secrets=aws_secrets,
-                open_container_port=open_container_port,
-                container_port=container_port,
-                container_port_name=container_port_name,
-                container_host_port=container_host_port,
-                mount_workspace=mount_workspace,
-                workspace_volume_name=workspace_volume_name,
-                workspace_volume_type=workspace_volume_type,
-                workspace_dir_container_path=workspace_dir_container_path,
-                add_workspace_name_to_container_path=add_workspace_name_to_container_path,
-                workspace_dir=workspace_dir,
-                container_name=container_name,
-                container_detach=container_detach,
-                container_auto_remove=container_auto_remove,
-                container_remove=container_remove,
-                container_user=container_user,
-                container_stdin_open=container_stdin_open,
-                container_stdout=container_stdout,
-                container_stderr=container_stderr,
-                container_tty=container_tty,
-                container_healthcheck=container_healthcheck,
-                container_hostname=container_hostname,
-                container_platform=container_platform,
-                container_working_dir=container_working_dir,
-                container_labels=container_labels,
-                container_restart_policy=container_restart_policy,
-                container_volumes=container_volumes,
-                container_ports=container_ports,
-                pod_name=pod_name,
-                pod_annotations=pod_annotations,
-                pod_node_selector=pod_node_selector,
-                secret_name=secret_name,
-                configmap_name=configmap_name,
-                replicas=replicas,
-                deploy_name=deploy_name,
-                image_pull_policy=image_pull_policy,
-                deploy_restart_policy=deploy_restart_policy,
-                deploy_labels=deploy_labels,
-                termination_grace_period_seconds=termination_grace_period_seconds,
-                topology_spread_key=topology_spread_key,
-                topology_spread_max_skew=topology_spread_max_skew,
-                topology_spread_when_unsatisfiable=topology_spread_when_unsatisfiable,
-                create_service=create_service,
-                service_name=service_name,
-                service_type=service_type,
-                service_port=service_port,
-                service_node_port=service_node_port,
-                service_target_port=service_target_port,
-                service_ports=service_ports,
-                service_labels=service_labels,
-                service_annotations=service_annotations,
-                service_health_check_node_port=service_health_check_node_port,
-                service_internal_traffic_policy=service_internal_traffic_policy,
-                service_load_balancer_class=service_load_balancer_class,
-                service_load_balancer_ip=service_load_balancer_ip,
-                service_load_balancer_source_ranges=service_load_balancer_source_ranges,
-                service_allocate_load_balancer_node_ports=service_allocate_load_balancer_node_ports,
-                create_ingress=create_ingress,
-                ingress_name=ingress_name,
-                ingress_annotations=ingress_annotations,
-                use_rbac=use_rbac,
-                ns_name=ns_name,
-                namespace=namespace,
-                sa_name=sa_name,
-                service_account=service_account,
-                cr_name=cr_name,
-                cluster_role=cluster_role,
-                crb_name=crb_name,
-                cluster_role_binding=cluster_role_binding,
-                aws_subnets=aws_subnets,
-                aws_security_groups=aws_security_groups,
-                ecs_cluster=ecs_cluster,
-                ecs_cluster_name=ecs_cluster_name,
-                ecs_launch_type=ecs_launch_type,
-                ecs_task_cpu=ecs_task_cpu,
-                ecs_task_memory=ecs_task_memory,
-                ecs_service_count=ecs_service_count,
-                assign_public_ip=assign_public_ip,
-                ecs_enable_exec=ecs_enable_exec,
-                load_balancer=load_balancer,
-                listener=listener,
-                create_load_balancer=create_load_balancer,
-                load_balancer_protocol=load_balancer_protocol,
-                load_balancer_security_groups=load_balancer_security_groups,
-                load_balancer_port=load_balancer_port,
-                load_balancer_certificate=load_balancer_certificate,
-                load_balancer_certificate_arn=load_balancer_certificate_arn,
-                target_group=target_group,
-                target_group_protocol=target_group_protocol,
-                target_group_port=target_group_port,
-                target_group_type=target_group_type,
-                health_check_protocol=health_check_protocol,
-                health_check_port=health_check_port,
-                health_check_enabled=health_check_enabled,
-                health_check_path=health_check_path,
-                health_check_interval_seconds=health_check_interval_seconds,
-                health_check_timeout_seconds=health_check_timeout_seconds,
-                healthy_threshold_count=healthy_threshold_count,
-                unhealthy_threshold_count=unhealthy_threshold_count,
-                skip_create=skip_create,
-                skip_read=skip_read,
-                skip_update=skip_update,
-                recreate_on_update=recreate_on_update,
-                skip_delete=skip_delete,
-                wait_for_creation=wait_for_creation,
-                wait_for_update=wait_for_update,
-                wait_for_deletion=wait_for_deletion,
-                waiter_delay=waiter_delay,
-                waiter_max_attempts=waiter_max_attempts,
-                save_output=save_output,
-                resource_dir=resource_dir,
-                use_cache=use_cache,
-                print_env_on_load=print_env_on_load,
-                **extra_kwargs,
-            )
-        except Exception as e:
-            logger.error(f"Args for {self.name} are not valid: {e}")
-            raise
+        super().__init__(
+            name=name,
+            version=version,
+            enabled=enabled,
+            image=image,
+            image_name=image_name,
+            image_tag=image_tag,
+            entrypoint=entrypoint,
+            command=command,
+            install_requirements=install_requirements,
+            requirements_file=requirements_file,
+            wait_for_db=wait_for_db,
+            db_app=db_app,
+            db_user=db_user,
+            db_password=db_password,
+            db_schema=db_schema,
+            db_host=db_host,
+            db_port=db_port,
+            db_dialect=db_dialect,
+            wait_for_redis=wait_for_redis,
+            redis_app=redis_app,
+            redis_host=redis_host,
+            redis_port=redis_port,
+            redis_driver=redis_driver,
+            container_name=container_name,
+            superset_config_path=superset_config_path,
+            flask_env=flask_env,
+            superset_env=superset_env,
+            python_path=python_path,
+            container_labels=container_labels,
+            env=env,
+            env_file=env_file,
+            secrets=secrets,
+            secrets_file=secrets_file,
+            aws_secrets=aws_secrets,
+            open_container_port=open_container_port,
+            container_port=container_port,
+            container_port_name=container_port_name,
+            container_host_port=container_host_port,
+            open_app_port=open_app_port,
+            app_port=app_port,
+            app_port_name=app_port_name,
+            app_host_port=app_host_port,
+            mount_workspace=mount_workspace,
+            workspace_volume_name=workspace_volume_name,
+            workspace_volume_type=workspace_volume_type,
+            workspace_volume_container_path=workspace_volume_container_path,
+            workspace_volume_host_path=workspace_volume_host_path,
+            create_git_sync_sidecar=create_git_sync_sidecar,
+            create_git_sync_init_container=create_git_sync_init_container,
+            git_sync_image_name=git_sync_image_name,
+            git_sync_image_tag=git_sync_image_tag,
+            git_sync_repo=git_sync_repo,
+            git_sync_branch=git_sync_branch,
+            git_sync_wait=git_sync_wait,
+            mount_resources=mount_resources,
+            resources_dir=resources_dir,
+            resources_dir_container_path=resources_dir_container_path,
+            resources_volume_name=resources_volume_name,
+            container_detach=container_detach,
+            container_auto_remove=container_auto_remove,
+            container_remove=container_remove,
+            container_user=container_user,
+            container_stdin_open=container_stdin_open,
+            container_tty=container_tty,
+            container_healthcheck=container_healthcheck,
+            container_hostname=container_hostname,
+            container_platform=container_platform,
+            container_working_dir=container_working_dir,
+            container_restart_policy_docker=container_restart_policy_docker,
+            container_volumes_docker=container_volumes_docker,
+            container_ports_docker=container_ports_docker,
+            replicas=replicas,
+            pod_name=pod_name,
+            deploy_name=deploy_name,
+            secret_name=secret_name,
+            configmap_name=configmap_name,
+            image_pull_policy=image_pull_policy,
+            pod_annotations=pod_annotations,
+            pod_node_selector=pod_node_selector,
+            deploy_restart_policy=deploy_restart_policy,
+            deploy_labels=deploy_labels,
+            termination_grace_period_seconds=termination_grace_period_seconds,
+            topology_spread_key=topology_spread_key,
+            topology_spread_max_skew=topology_spread_max_skew,
+            topology_spread_when_unsatisfiable=topology_spread_when_unsatisfiable,
+            create_service=create_service,
+            service_name=service_name,
+            service_type=service_type,
+            service_port=service_port,
+            service_node_port=service_node_port,
+            service_target_port=service_target_port,
+            service_ports=service_ports,
+            service_labels=service_labels,
+            service_annotations=service_annotations,
+            service_health_check_node_port=service_health_check_node_port,
+            service_internal_traffic_policy=service_internal_traffic_policy,
+            service_load_balancer_class=service_load_balancer_class,
+            service_load_balancer_ip=service_load_balancer_ip,
+            service_load_balancer_source_ranges=service_load_balancer_source_ranges,
+            service_allocate_load_balancer_node_ports=service_allocate_load_balancer_node_ports,
+            create_app_service=create_app_service,
+            app_svc_name=app_svc_name,
+            app_svc_type=app_svc_type,
+            app_svc_port=app_svc_port,
+            app_node_port=app_node_port,
+            app_target_port=app_target_port,
+            app_svc_ports=app_svc_ports,
+            app_svc_labels=app_svc_labels,
+            app_svc_annotations=app_svc_annotations,
+            app_svc_health_check_node_port=app_svc_health_check_node_port,
+            app_svc_internal_taffic_policy=app_svc_internal_taffic_policy,
+            app_svc_load_balancer_class=app_svc_load_balancer_class,
+            app_svc_load_balancer_ip=app_svc_load_balancer_ip,
+            app_svc_load_balancer_source_ranges=app_svc_load_balancer_source_ranges,
+            app_svc_allocate_load_balancer_node_ports=app_svc_allocate_load_balancer_node_ports,
+            use_rbac=use_rbac,
+            ns_name=ns_name,
+            namespace=namespace,
+            sa_name=sa_name,
+            service_account=service_account,
+            cr_name=cr_name,
+            cluster_role=cluster_role,
+            crb_name=crb_name,
+            cluster_role_binding=cluster_role_binding,
+            extra_secrets=extra_secrets,
+            extra_configmaps=extra_configmaps,
+            extra_services=extra_services,
+            extra_deployments=extra_deployments,
+            extra_pvs=extra_pvs,
+            extra_pvcs=extra_pvcs,
+            extra_containers=extra_containers,
+            extra_init_containers=extra_init_containers,
+            extra_ports=extra_ports,
+            extra_volumes=extra_volumes,
+            extra_storage_classes=extra_storage_classes,
+            extra_custom_objects=extra_custom_objects,
+            extra_crds=extra_crds,
+            print_env_on_load=print_env_on_load,
+            use_cache=use_cache,
+            load_examples=load_examples,
+            **kwargs,
+        )
```

### Comparing `phidata-1.7.8/phidata/app/superset/superset_base.py` & `phidata-1.7.9/phidata/app/superset/superset_base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/superset/superset_init.py` & `phidata-1.7.9/phidata/app/superset/superset_init.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/superset/superset_webserver.py` & `phidata-1.7.9/phidata/app/superset/superset_worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,27 +7,27 @@
     DbApp,
     WorkspaceVolumeType,
     ImagePullPolicy,
     RestartPolicy,
 )
 
 
-class SupersetWebserver(SupersetBase):
+class SupersetWorker(SupersetBase):
     def __init__(
         self,
-        name: str = "superset-ws",
+        name: str = "superset-worker",
         version: str = "1",
         enabled: bool = True,
         # -*- Image Configuration,
         # Image can be provided as a DockerImage object or as image_name:image_tag
         image: Optional[Any] = None,
         image_name: str = "phidata/superset",
         image_tag: str = "2.0.1",
         entrypoint: Optional[Union[str, List]] = None,
-        command: Optional[Union[str, List]] = "webserver",
+        command: Optional[Union[str, List]] = "worker",
         # Install python dependencies using a requirements.txt file,
         # Sets the REQUIREMENTS_LOCAL & REQUIREMENTS_FILE_PATH env var to requirements_file,
         install_requirements: bool = False,
         # Path to the requirements.txt file relative to the workspace_root,
         requirements_file: str = "requirements.txt",
         # -*- Superset Configuration,
         # Configure Superset db,
@@ -97,15 +97,15 @@
         # Port number on the container,
         container_port: int = 8000,
         # Port name: Only used by the K8sContainer,
         container_port_name: str = "http",
         # Host port: Only used by the DockerContainer,
         container_host_port: int = 8000,
         # Open the app port if open_app_port=True,
-        open_app_port: bool = True,
+        open_app_port: bool = False,
         # App port number on the container,
         # Set the SUPERSET_PORT env var,
         app_port: int = 8088,
         # Only used by the K8sContainer,
         app_port_name: str = "app",
         # Only used by the DockerContainer,
         app_host_port: int = 8088,
@@ -238,15 +238,15 @@
         service_health_check_node_port: Optional[int] = None,
         service_internal_traffic_policy: Optional[str] = None,
         service_load_balancer_class: Optional[str] = None,
         service_load_balancer_ip: Optional[str] = None,
         service_load_balancer_source_ranges: Optional[List[str]] = None,
         service_allocate_load_balancer_node_ports: Optional[bool] = None,
         # App Service Configuration,
-        create_app_service: bool = True,
+        create_app_service: bool = False,
         # Configure the app service,
         app_svc_name: Optional[str] = None,
         app_svc_type: Optional[ServiceType] = None,
         # The port that will be exposed by the service.,
         app_svc_port: int = 8088,
         # The node_port that will be exposed by the service if app_svc_type = ServiceType.NODE_PORT,
         app_node_port: Optional[int] = None,
```

### Comparing `phidata-1.7.8/phidata/app/superset/superset_worker.py` & `phidata-1.7.9/phidata/app/superset/superset_worker_beat.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,27 +7,27 @@
     DbApp,
     WorkspaceVolumeType,
     ImagePullPolicy,
     RestartPolicy,
 )
 
 
-class SupersetWorker(SupersetBase):
+class SupersetWorkerBeat(SupersetBase):
     def __init__(
         self,
-        name: str = "superset-worker",
+        name: str = "superset-worker-beat",
         version: str = "1",
         enabled: bool = True,
         # -*- Image Configuration,
         # Image can be provided as a DockerImage object or as image_name:image_tag
         image: Optional[Any] = None,
         image_name: str = "phidata/superset",
         image_tag: str = "2.0.1",
         entrypoint: Optional[Union[str, List]] = None,
-        command: Optional[Union[str, List]] = "worker",
+        command: Optional[Union[str, List]] = "beat",
         # Install python dependencies using a requirements.txt file,
         # Sets the REQUIREMENTS_LOCAL & REQUIREMENTS_FILE_PATH env var to requirements_file,
         install_requirements: bool = False,
         # Path to the requirements.txt file relative to the workspace_root,
         requirements_file: str = "requirements.txt",
         # -*- Superset Configuration,
         # Configure Superset db,
```

### Comparing `phidata-1.7.8/phidata/app/traefik/crds.py` & `phidata-1.7.9/phidata/app/traefik/crds.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/traefik/ingress_route.py` & `phidata-1.7.9/phidata/app/traefik/ingress_route.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/app/traefik/router.py` & `phidata-1.7.9/phidata/app/traefik/router.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/asset/aws/aws_asset.py` & `phidata-1.7.9/phidata/asset/aws/aws_asset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/asset/data_asset.py` & `phidata-1.7.9/phidata/asset/data_asset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/asset/local/file.py` & `phidata-1.7.9/phidata/asset/local/file.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/asset/local/local_asset.py` & `phidata-1.7.9/phidata/asset/local/local_asset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/api_client.py` & `phidata-1.7.9/phidata/aws/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/athena/query.py` & `phidata-1.7.9/phidata/aws/athena/query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/config.py` & `phidata-1.7.9/phidata/aws/config.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/create/iam/eks_admin_role.py` & `phidata-1.7.9/phidata/aws/create/iam/eks_admin_role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/create/iam/role.py` & `phidata-1.7.9/phidata/aws/create/iam/role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/driver.py` & `phidata-1.7.9/phidata/aws/driver.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/enums/manager_status.py` & `phidata-1.7.9/phidata/aws/enums/manager_status.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/manager.py` & `phidata-1.7.9/phidata/aws/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/resource/acm/certificate.py` & `phidata-1.7.9/phidata/aws/resource/acm/certificate.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/resource/athena/query.py` & `phidata-1.7.9/phidata/aws/resource/athena/query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/resource/base.py` & `phidata-1.7.9/phidata/aws/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/resource/cloudformation/stack.py` & `phidata-1.7.9/phidata/aws/resource/cloudformation/stack.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/resource/ec2/security_group.py` & `phidata-1.7.9/phidata/aws/resource/ec2/security_group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/resource/ec2/subnet.py` & `phidata-1.7.9/phidata/aws/resource/ec2/subnet.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/resource/ec2/volume.py` & `phidata-1.7.9/phidata/aws/resource/ec2/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/resource/ecs/cluster.py` & `phidata-1.7.9/phidata/aws/resource/ecs/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/resource/ecs/container.py` & `phidata-1.7.9/phidata/aws/resource/ecs/container.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/resource/ecs/service.py` & `phidata-1.7.9/phidata/aws/resource/ecs/service.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/resource/ecs/task_definition.py` & `phidata-1.7.9/phidata/aws/resource/ecs/task_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/resource/ecs/volume.py` & `phidata-1.7.9/phidata/aws/resource/ecs/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/resource/eks/addon.py` & `phidata-1.7.9/phidata/aws/resource/eks/addon.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/resource/eks/cluster.py` & `phidata-1.7.9/phidata/aws/resource/eks/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/resource/eks/fargate_profile.py` & `phidata-1.7.9/phidata/aws/resource/eks/fargate_profile.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/resource/eks/kubeconfig.py` & `phidata-1.7.9/phidata/aws/resource/eks/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/resource/eks/node_group.py` & `phidata-1.7.9/phidata/aws/resource/eks/node_group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/resource/elasticache/cluster.py` & `phidata-1.7.9/phidata/aws/resource/elasticache/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/resource/elasticache/subnet_group.py` & `phidata-1.7.9/phidata/aws/resource/elasticache/subnet_group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/resource/elb/listener.py` & `phidata-1.7.9/phidata/aws/resource/elb/listener.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/resource/elb/load_balancer.py` & `phidata-1.7.9/phidata/aws/resource/elb/load_balancer.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/resource/elb/target_group.py` & `phidata-1.7.9/phidata/aws/resource/elb/target_group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/resource/emr/cluster.py` & `phidata-1.7.9/phidata/aws/resource/emr/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/resource/glue/crawler.py` & `phidata-1.7.9/phidata/aws/resource/glue/crawler.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/resource/group.py` & `phidata-1.7.9/phidata/aws/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/resource/iam/group.py` & `phidata-1.7.9/phidata/aws/resource/iam/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/resource/iam/policy.py` & `phidata-1.7.9/phidata/aws/resource/iam/policy.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/resource/iam/role.py` & `phidata-1.7.9/phidata/aws/resource/iam/role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/resource/rds/db_cluster.py` & `phidata-1.7.9/phidata/aws/resource/rds/db_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/resource/rds/db_instance.py` & `phidata-1.7.9/phidata/aws/resource/rds/db_instance.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/resource/rds/db_subnet_group.py` & `phidata-1.7.9/phidata/aws/resource/rds/db_subnet_group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/resource/s3/bucket.py` & `phidata-1.7.9/phidata/aws/resource/s3/bucket.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/resource/secret/manager.py` & `phidata-1.7.9/phidata/aws/resource/secret/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/resource/secret/reader.py` & `phidata-1.7.9/phidata/aws/resource/secret/reader.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/resource/types.py` & `phidata-1.7.9/phidata/aws/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/resource/utils.py` & `phidata-1.7.9/phidata/aws/resource/utils.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/s3/csv_dataset.py` & `phidata-1.7.9/phidata/aws/s3/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/s3/dataset.py` & `phidata-1.7.9/phidata/aws/s3/dataset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/s3/dataset_base.py` & `phidata-1.7.9/phidata/aws/s3/dataset_base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/s3/object.py` & `phidata-1.7.9/phidata/aws/s3/object.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/aws/worker.py` & `phidata-1.7.9/phidata/aws/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/base.py` & `phidata-1.7.9/phidata/base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/checks/check.py` & `phidata-1.7.9/phidata/checks/check.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/checks/not_empty.py` & `phidata-1.7.9/phidata/checks/not_empty.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/constants.py` & `phidata-1.7.9/phidata/constants.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/decorators/timer.py` & `phidata-1.7.9/phidata/decorators/timer.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/decorators/validate_env.py` & `phidata-1.7.9/phidata/decorators/validate_env.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/docker/api_client.py` & `phidata-1.7.9/phidata/docker/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/docker/args.py` & `phidata-1.7.9/phidata/docker/args.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/docker/config.py` & `phidata-1.7.9/phidata/docker/config.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/docker/enums.py` & `phidata-1.7.9/phidata/docker/enums.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/docker/manager.py` & `phidata-1.7.9/phidata/docker/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/docker/resource/base.py` & `phidata-1.7.9/phidata/docker/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/docker/resource/container.py` & `phidata-1.7.9/phidata/docker/resource/container.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/docker/resource/group.py` & `phidata-1.7.9/phidata/docker/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/docker/resource/image.py` & `phidata-1.7.9/phidata/docker/resource/image.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,14 +107,16 @@
             print_info(f"    dockerfile: {self.dockerfile}")
         logger.debug(f"platform: {self.platform}")
         logger.debug(f"nocache: {nocache}")
         logger.debug(f"pull: {pull}")
 
         last_status = None
         last_build_log = None
+        build_log_output: List[Any] = []
+        build_step_progress: List[str] = []
         try:
             _api_client: DockerClient = docker_client.api_client
             build_stream = _api_client.api.build(
                 tag=self.get_name_tag(),
                 path=self.path,
                 dockerfile=self.dockerfile,
                 nocache=nocache,
@@ -134,18 +136,18 @@
                 platform=self.platform,
                 isolation=self.isolation,
                 use_config_proxy=self.use_config_proxy,
                 decode=True,
             )
 
             with Live(transient=True, console=console) as live_log:
-                progress: List[str] = []
                 for build_log in build_stream:
                     if build_log != last_build_log:
                         last_build_log = build_log
+                        build_log_output.append(build_log)
 
                     build_status: str = build_log.get("status")
                     if build_status is not None:
                         _status = build_status.lower()
                         if _status in (
                             "waiting",
                             "downloading",
@@ -156,43 +158,44 @@
                             continue
                         if build_status != last_status:
                             logger.debug(build_status)
                             last_status = build_status
 
                     if build_log.get("error", None) is not None:
                         live_log.stop()
+                        # logger.error(build_log_output[-10:])
                         print_error(build_log["error"])
                         print_error(f"Image build failed: {self.get_name_tag()}")
                         return None
 
                     stream = build_log.get("stream", None)
                     if stream is None or stream == "\n":
                         continue
                     stream = stream.strip()
 
                     if "Step" in stream and self.print_build_log:
-                        progress = []
+                        build_step_progress = []
                         print_info(stream)
                     else:
-                        progress.append(stream)
-                        if len(progress) > 10:
-                            progress.pop(0)
+                        build_step_progress.append(stream)
+                        if len(build_step_progress) > 10:
+                            build_step_progress.pop(0)
 
                     if "error" in stream.lower():
                         print(stream)
                         live_log.stop()
                         print_error(f"Image build failed: {self.get_name_tag()}")
                         return None
                     if build_log.get("aux", None) is not None:
                         logger.debug("build_log['aux'] :{}".format(build_log["aux"]))
                         self.image_build_id = build_log.get("aux", {}).get("ID")
 
                     # Render table
                     table = Table(show_edge=False, show_header=False, show_lines=False)
-                    for line in progress:
+                    for line in build_step_progress:
                         table.add_row(line, style="dim")
                     live_log.update(table)
 
             if self.push_image:
                 print_info(f"Pushing {self.get_name_tag()}")
                 with Live(transient=True, console=console) as live_log:
                     push_status = {}
```

### Comparing `phidata-1.7.8/phidata/docker/resource/network.py` & `phidata-1.7.9/phidata/docker/resource/network.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/docker/resource/types.py` & `phidata-1.7.9/phidata/docker/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/docker/resource/utils.py` & `phidata-1.7.9/phidata/docker/resource/utils.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/docker/resource/volume.py` & `phidata-1.7.9/phidata/docker/resource/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/docker/utils/container.py` & `phidata-1.7.9/phidata/docker/utils/container.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/docker/worker.py` & `phidata-1.7.9/phidata/docker/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/infra/args.py` & `phidata-1.7.9/phidata/infra/args.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/infra/config.py` & `phidata-1.7.9/phidata/infra/config.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/infra/resource.py` & `phidata-1.7.9/phidata/infra/resource.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/api_client.py` & `phidata-1.7.9/phidata/k8s/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/args.py` & `phidata-1.7.9/phidata/k8s/args.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/config.py` & `phidata-1.7.9/phidata/k8s/config.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py` & `phidata-1.7.9/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py` & `phidata-1.7.9/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/create/apps/v1/deployment.py` & `phidata-1.7.9/phidata/k8s/create/apps/v1/deployment.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/create/common/port.py` & `phidata-1.7.9/phidata/k8s/create/common/port.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/create/core/v1/config_map.py` & `phidata-1.7.9/phidata/k8s/create/core/v1/config_map.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/create/core/v1/container.py` & `phidata-1.7.9/phidata/k8s/create/core/v1/container.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/create/core/v1/namespace.py` & `phidata-1.7.9/phidata/k8s/create/core/v1/namespace.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/create/core/v1/persistent_volume.py` & `phidata-1.7.9/phidata/k8s/create/core/v1/persistent_volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/create/core/v1/persistent_volume_claim.py` & `phidata-1.7.9/phidata/k8s/create/core/v1/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/create/core/v1/secret.py` & `phidata-1.7.9/phidata/k8s/create/core/v1/secret.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/create/core/v1/service.py` & `phidata-1.7.9/phidata/k8s/create/core/v1/service.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/create/core/v1/service_account.py` & `phidata-1.7.9/phidata/k8s/create/core/v1/service_account.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/create/core/v1/volume.py` & `phidata-1.7.9/phidata/k8s/create/core/v1/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/create/crb/eks_admin_crb.py` & `phidata-1.7.9/phidata/k8s/create/crb/eks_admin_crb.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/create/group.py` & `phidata-1.7.9/phidata/k8s/create/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/create/kubeconfig.py` & `phidata-1.7.9/phidata/k8s/create/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/create/networking_k8s_io/v1/ingress.py` & `phidata-1.7.9/phidata/k8s/create/networking_k8s_io/v1/ingress.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py` & `phidata-1.7.9/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py` & `phidata-1.7.9/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/create/storage_k8s_io/v1/storage_class.py` & `phidata-1.7.9/phidata/k8s/create/storage_k8s_io/v1/storage_class.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/enums/api_version.py` & `phidata-1.7.9/phidata/k8s/enums/api_version.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/enums/kind.py` & `phidata-1.7.9/phidata/k8s/enums/kind.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/enums/manager_status.py` & `phidata-1.7.9/phidata/k8s/enums/manager_status.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/enums/pv.py` & `phidata-1.7.9/phidata/k8s/enums/pv.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/manager.py` & `phidata-1.7.9/phidata/k8s/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py` & `phidata-1.7.9/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py` & `phidata-1.7.9/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/resource/apps/v1/deployment.py` & `phidata-1.7.9/phidata/k8s/resource/apps/v1/deployment.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/resource/apps/v1/deployment_strategy.py` & `phidata-1.7.9/phidata/k8s/resource/apps/v1/deployment_strategy.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/resource/base.py` & `phidata-1.7.9/phidata/k8s/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/resource/core/v1/config_map.py` & `phidata-1.7.9/phidata/k8s/resource/core/v1/config_map.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/resource/core/v1/container.py` & `phidata-1.7.9/phidata/k8s/resource/core/v1/container.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/resource/core/v1/local_object_reference.py` & `phidata-1.7.9/phidata/k8s/resource/core/v1/local_object_reference.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/resource/core/v1/namespace.py` & `phidata-1.7.9/phidata/k8s/resource/core/v1/namespace.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/resource/core/v1/node_selector.py` & `phidata-1.7.9/phidata/k8s/resource/core/v1/node_selector.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/resource/core/v1/object_reference.py` & `phidata-1.7.9/phidata/k8s/resource/core/v1/object_reference.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/resource/core/v1/persistent_volume.py` & `phidata-1.7.9/phidata/k8s/resource/core/v1/persistent_volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/resource/core/v1/persistent_volume_claim.py` & `phidata-1.7.9/phidata/k8s/resource/core/v1/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/resource/core/v1/pod.py` & `phidata-1.7.9/phidata/k8s/resource/core/v1/pod.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/resource/core/v1/pod_spec.py` & `phidata-1.7.9/phidata/k8s/resource/core/v1/pod_spec.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/resource/core/v1/pod_template_spec.py` & `phidata-1.7.9/phidata/k8s/resource/core/v1/pod_template_spec.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/resource/core/v1/resource_requirements.py` & `phidata-1.7.9/phidata/k8s/resource/core/v1/resource_requirements.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/resource/core/v1/secret.py` & `phidata-1.7.9/phidata/k8s/resource/core/v1/secret.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/resource/core/v1/service.py` & `phidata-1.7.9/phidata/k8s/resource/core/v1/service.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/resource/core/v1/service_account.py` & `phidata-1.7.9/phidata/k8s/resource/core/v1/service_account.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/resource/core/v1/toleration.py` & `phidata-1.7.9/phidata/k8s/resource/core/v1/toleration.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/resource/core/v1/topology_spread_constraints.py` & `phidata-1.7.9/phidata/k8s/resource/core/v1/topology_spread_constraints.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/resource/core/v1/volume.py` & `phidata-1.7.9/phidata/k8s/resource/core/v1/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/resource/core/v1/volume_node_affinity.py` & `phidata-1.7.9/phidata/k8s/resource/core/v1/volume_node_affinity.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/resource/core/v1/volume_source.py` & `phidata-1.7.9/phidata/k8s/resource/core/v1/volume_source.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/resource/group.py` & `phidata-1.7.9/phidata/k8s/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/resource/kubeconfig.py` & `phidata-1.7.9/phidata/k8s/resource/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/resource/meta/v1/label_selector.py` & `phidata-1.7.9/phidata/k8s/resource/meta/v1/label_selector.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/resource/meta/v1/object_meta.py` & `phidata-1.7.9/phidata/k8s/resource/meta/v1/object_meta.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/resource/networking_k8s_io/v1/ingress.py` & `phidata-1.7.9/phidata/k8s/resource/networking_k8s_io/v1/ingress.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py` & `phidata-1.7.9/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py` & `phidata-1.7.9/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py` & `phidata-1.7.9/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/resource/types.py` & `phidata-1.7.9/phidata/k8s/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/resource/utils.py` & `phidata-1.7.9/phidata/k8s/resource/utils.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/utils/pod.py` & `phidata-1.7.9/phidata/k8s/utils/pod.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/k8s/worker.py` & `phidata-1.7.9/phidata/k8s/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/llm/duckdb/agent.py` & `phidata-1.7.9/phidata/llm/duckdb/agent.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/llm/duckdb/chain.py` & `phidata-1.7.9/phidata/llm/duckdb/chain.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/llm/duckdb/connection.py` & `phidata-1.7.9/phidata/llm/duckdb/connection.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/llm/duckdb/loader.py` & `phidata-1.7.9/phidata/llm/duckdb/loader.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/llm/duckdb/query.py` & `phidata-1.7.9/phidata/llm/duckdb/query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/llm/duckdb/tool.py` & `phidata-1.7.9/phidata/llm/duckdb/tool.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/product/data_product.py` & `phidata-1.7.9/phidata/product/data_product.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/table/local/csv.py` & `phidata-1.7.9/phidata/table/local/csv.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/table/local/local_table.py` & `phidata-1.7.9/phidata/table/local/local_table.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/table/local/parquet.py` & `phidata-1.7.9/phidata/table/local/parquet.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/table/s3/csv.py` & `phidata-1.7.9/phidata/table/s3/csv.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/table/s3/parquet.py` & `phidata-1.7.9/phidata/table/s3/parquet.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/table/s3/s3_table.py` & `phidata-1.7.9/phidata/table/s3/s3_table.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/table/sql/postgres.py` & `phidata-1.7.9/phidata/table/sql/postgres.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/table/sql/sql_table.py` & `phidata-1.7.9/phidata/table/sql/sql_table.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/task/aws/athena/run_query.py` & `phidata-1.7.9/phidata/task/aws/athena/run_query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/task/aws/emr/create_cluster.py` & `phidata-1.7.9/phidata/task/aws/emr/create_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/task/aws/emr/delete_cluster.py` & `phidata-1.7.9/phidata/task/aws/emr/delete_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/task/aws/glue/start_crawler.py` & `phidata-1.7.9/phidata/task/aws/glue/start_crawler.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/task/decorator.py` & `phidata-1.7.9/phidata/task/decorator.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/task/download/s3/to_file.py` & `phidata-1.7.9/phidata/task/download/s3/to_file.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/task/download/url/to_file.py` & `phidata-1.7.9/phidata/task/download/url/to_file.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/task/download/url/to_s3.py` & `phidata-1.7.9/phidata/task/download/url/to_s3.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/task/download/url/to_sql.py` & `phidata-1.7.9/phidata/task/download/url/to_sql.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/task/plot/sql/query.py` & `phidata-1.7.9/phidata/task/plot/sql/query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/task/python_task.py` & `phidata-1.7.9/phidata/task/python_task.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/task/run/sql/query.py` & `phidata-1.7.9/phidata/task/run/sql/query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/task/task.py` & `phidata-1.7.9/phidata/task/task.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/task/task_relatives.py` & `phidata-1.7.9/phidata/task/task_relatives.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/task/upload/file/to_s3.py` & `phidata-1.7.9/phidata/task/upload/file/to_s3.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/task/upload/file/to_sql.py` & `phidata-1.7.9/phidata/task/upload/file/to_sql.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/types/airflow.py` & `phidata-1.7.9/phidata/types/airflow.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/types/context.py` & `phidata-1.7.9/phidata/types/context.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/types/phidata_runtime.py` & `phidata-1.7.9/phidata/types/phidata_runtime.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/utils/cli_console.py` & `phidata-1.7.9/phidata/utils/cli_console.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/utils/common.py` & `phidata-1.7.9/phidata/utils/common.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/utils/compare.py` & `phidata-1.7.9/phidata/utils/compare.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/utils/context.py` & `phidata-1.7.9/phidata/utils/context.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/utils/dttm.py` & `phidata-1.7.9/phidata/utils/dttm.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/utils/enums.py` & `phidata-1.7.9/phidata/utils/enums.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/utils/env_file.py` & `phidata-1.7.9/phidata/utils/env_file.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/utils/env_var.py` & `phidata-1.7.9/phidata/utils/env_var.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/utils/filesystem.py` & `phidata-1.7.9/phidata/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/utils/get_python_objects_from_module.py` & `phidata-1.7.9/phidata/utils/get_python_objects_from_module.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/utils/json_io.py` & `phidata-1.7.9/phidata/utils/json_io.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/utils/k8s.py` & `phidata-1.7.9/phidata/utils/k8s.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/utils/log.py` & `phidata-1.7.9/phidata/utils/log.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/utils/print_table.py` & `phidata-1.7.9/phidata/utils/print_table.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/utils/workspace_path.py` & `phidata-1.7.9/phidata/utils/workspace_path.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/utils/yaml_io.py` & `phidata-1.7.9/phidata/utils/yaml_io.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/workflow/decorator.py` & `phidata-1.7.9/phidata/workflow/decorator.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/workflow/workflow.py` & `phidata-1.7.9/phidata/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/workflow/workflow_relatives.py` & `phidata-1.7.9/phidata/workflow/workflow_relatives.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/workspace/config.py` & `phidata-1.7.9/phidata/workspace/config.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.8/phidata/workspace/settings.py` & `phidata-1.7.9/phidata/workspace/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     dev_mysql_enabled: bool = False
     dev_postgres_enabled: bool = False
     dev_prometheus_enabled: bool = False
     dev_redis_enabled: bool = False
     dev_spark_enabled: bool = False
     dev_superset_enabled: bool = False
     dev_traefik_enabled: bool = False
+    dev_vectordb_enabled: bool = False
     #
     # -*- Staging settings
     #
     stg_env: str = "stg"
     # Staging git repo branch: used to git-sync DAGs and Charts
     stg_branch: str = "main"
     # Key for naming staging resources
@@ -82,14 +83,15 @@
     stg_postgres_enabled: bool = False
     stg_prometheus_enabled: bool = False
     stg_redis_enabled: bool = False
     stg_spark_enabled: bool = False
     stg_superset_enabled: bool = False
     stg_traefik_enabled: bool = False
     stg_whoami_enabled: bool = False
+    stg_vectordb_enabled: bool = False
     #
     # -*- Production settings
     #
     prd_env: str = "prd"
     # Production git repo branch: used to git-sync DAGs and Charts
     prd_branch: str = "main"
     # Key for naming production resources
@@ -114,14 +116,15 @@
     prd_postgres_enabled: bool = False
     prd_prometheus_enabled: bool = False
     prd_redis_enabled: bool = False
     prd_spark_enabled: bool = False
     prd_superset_enabled: bool = False
     prd_traefik_enabled: bool = False
     prd_whoami_enabled: bool = False
+    prd_vectordb_enabled: bool = False
     #
     # -*- AWS settings
     #
     # Region for AWS resources
     aws_region: Optional[str] = None
     # Availability Zones for AWS resources
     aws_az1: Optional[str] = None
```

### Comparing `phidata-1.7.8/phidata.egg-info/PKG-INFO` & `phidata-1.7.9/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,12 @@
-Metadata-Version: 2.1
-Name: phidata
-Version: 1.7.8
-Summary: Phidata is a toolkit for building applications using OSS
-Author-email: Ashpreet Bedi <ashpreet@phidata.com>
-Project-URL: homepage, https://phidata.com
-Project-URL: documentation, https://docs.phidata.com
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: aws
-License-File: LICENSE
-
 <h1 align="center">
   phidata
 </h1>
 <p align="center">
-    <em>A toolkit for building applications using open source tools</em>
+    <em>Run open source tools using python</em>
 </p>
 
 <p align="center">
 <a href="https://python.org/pypi/phidata" target="_blank">
     <img src="https://img.shields.io/pypi/v/phidata?color=blue&label=version" alt="version">
 </a>
 <a href="https://github.com/phidatahq/phidata" target="_blank">
@@ -38,19 +25,19 @@
 
 [//]: # (</a>)
 
 </p>
 
 ---
 
-Open source tools can be used to build powerful software, but are difficult to run in production settings.
+### Phidata is a toolkit for building applications with open source tools.
 
-- Phidata makes it easy to run tools like FastApi, Django, Jupyter, Airflow and Superset.
-- Phidata packages these tools into LLM Apps, Web Apps and Data Platforms.
-- Phidata runs your application locally for development and production on AWS, using 1 command.
+- Phidata makes it easy to run tools like FastApi, Django, Jupyter, Streamlit, Airflow and Superset.
+- Use these tools to build LLM Apps, Web Apps and Data Platforms.
+- Run locally for development and production on AWS, with 1 command.
 
 ## 🚀 How it works
 
 - **Create your codebase** from a template using `phi ws create`
 - **Run your app locally** using `phi ws up dev:docker`
 - **Run your app on AWS** using `phi ws up prd:aws`
 
@@ -62,39 +49,32 @@
 - Install [docker desktop](https://docs.docker.com/desktop/install/mac-install/)
 
 ### Setup
 
 Open the `terminal` and create a python virtual environment
 
 ```shell
-python3 -m venv ~/.venvs/aienv
-source ~/.venvs/aienv/bin/activate
+python3 -m venv ~/.venvs/labenv
+source ~/.venvs/labenv/bin/activate
 ```
 
 Install `phidata`
 
 ```shell
 pip install phidata
 ```
 
 ### Define `DockerConfig` that runs a `Jupyter` app
 
-Create a file `resources.py`
-
-```shell
-touch resources.py
-```
-
-Add the following code to `resources.py`
+Create a file `resources.py` and add the following code to it
 
 ```python
 from phidata.app.jupyter import Jupyter
 from phidata.docker.config import DockerConfig
 
-
 dev_docker_config = DockerConfig(
     apps=[
         # -*- Run Jupyter on port 8888
         Jupyter(mount_workspace=True)
     ],
 )
 ```
```

#### html2text {}

```diff
@@ -1,31 +1,24 @@
-Metadata-Version: 2.1 Name: phidata Version: 1.7.8 Summary: Phidata is a
-toolkit for building applications using OSS Author-email: Ashpreet Bedi
-phidata.com> Project-URL: homepage, https://phidata.com Project-URL:
-documentation, https://docs.phidata.com Requires-Python: >=3.7 Description-
-Content-Type: text/markdown Provides-Extra: dev Provides-Extra: aws License-
-File: LICENSE
                              ****** phidata ******
-          A toolkit for building applications using open source tools
+                      Run open source tools using python
   [version] [pythonversion] [downloads] [build-status] [//]: # ()_[//]:_#_(_
                            [test-status])_[//]:_#_()
---- Open source tools can be used to build powerful software, but are difficult
-to run in production settings. - Phidata makes it easy to run tools like
-FastApi, Django, Jupyter, Airflow and Superset. - Phidata packages these tools
-into LLM Apps, Web Apps and Data Platforms. - Phidata runs your application
-locally for development and production on AWS, using 1 command. ## ð How it
-works - **Create your codebase** from a template using `phi ws create` - **Run
-your app locally** using `phi ws up dev:docker` - **Run your app on AWS** using
-`phi ws up prd:aws` ## Basic Example: Run a Jupyter Notebook ### Requirements -
-python 3.7+ - Install [docker desktop](https://docs.docker.com/desktop/install/
-mac-install/) ### Setup Open the `terminal` and create a python virtual
-environment ```shell python3 -m venv ~/.venvs/aienv source ~/.venvs/aienv/bin/
-activate ``` Install `phidata` ```shell pip install phidata ``` ### Define
-`DockerConfig` that runs a `Jupyter` app Create a file `resources.py` ```shell
-touch resources.py ``` Add the following code to `resources.py` ```python from
+--- ### Phidata is a toolkit for building applications with open source tools.
+- Phidata makes it easy to run tools like FastApi, Django, Jupyter, Streamlit,
+Airflow and Superset. - Use these tools to build LLM Apps, Web Apps and Data
+Platforms. - Run locally for development and production on AWS, with 1 command.
+## ð How it works - **Create your codebase** from a template using `phi ws
+create` - **Run your app locally** using `phi ws up dev:docker` - **Run your
+app on AWS** using `phi ws up prd:aws` ## Basic Example: Run a Jupyter Notebook
+### Requirements - python 3.7+ - Install [docker desktop](https://
+docs.docker.com/desktop/install/mac-install/) ### Setup Open the `terminal` and
+create a python virtual environment ```shell python3 -m venv ~/.venvs/labenv
+source ~/.venvs/labenv/bin/activate ``` Install `phidata` ```shell pip install
+phidata ``` ### Define `DockerConfig` that runs a `Jupyter` app Create a file
+`resources.py` and add the following code to it ```python from
 phidata.app.jupyter import Jupyter from phidata.docker.config import
 DockerConfig dev_docker_config = DockerConfig( apps=[ # -*- Run Jupyter on port
 8888 Jupyter(mount_workspace=True) ], ) ``` ### Start the app ```shell phi
 start resources.py ``` - Open the browser and go to `http://localhost:8888` -
 Password is `admin` ### Stop the app ```shell phi stop resources.py ``` ## More
 Information: - **Documentation**: https://docs.phidata.com - **Questions:**
 Chat with us on Discord - **Email**: help@phidata.com
```

### Comparing `phidata-1.7.8/phidata.egg-info/SOURCES.txt` & `phidata-1.7.9/phidata.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 phidata/app/assistant/assistant.py
 phidata/app/cadvisor/__init__.py
 phidata/app/cadvisor/cadvisor.py
 phidata/app/databox/__init__.py
 phidata/app/databox/databox.py
 phidata/app/db/__init__.py
 phidata/app/db/base_db.py
+phidata/app/db/db_app.py
 phidata/app/django/__init__.py
 phidata/app/django/django_app.py
 phidata/app/django/django_backup.py
 phidata/app/elastic/__init__.py
 phidata/app/elastic/elastic_app.py
 phidata/app/elasticsearch/__init__.py
 phidata/app/elasticsearch/elasticsearch.py
```

### Comparing `phidata-1.7.8/pyproject.toml` & `phidata-1.7.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [project]
 name = "phidata"
-version = "1.7.8"
+version = "1.7.9"
 description = "Phidata is a toolkit for building applications using OSS"
 requires-python = ">=3.7"
 readme = "README.md"
 authors = [
   {name = "Ashpreet Bedi", email = "ashpreet@phidata.com"}
 ]
 
 dependencies = [
   "boto3>=1.26.76,<1.26.77",
   "botocore>=1.29.76,<1.29.77",
-  "phiterm==1.7.8",
+  "phiterm==1.7.9",
   "pyarrow",
   "pydantic",
 ]
 
 [project.optional-dependencies]
 dev = [
     "mypy",
```

