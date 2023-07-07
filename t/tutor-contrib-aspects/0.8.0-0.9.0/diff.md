# Comparing `tmp/tutor-contrib-aspects-0.8.0.tar.gz` & `tmp/tutor-contrib-aspects-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tutor-contrib-aspects-0.8.0.tar", last modified: Thu Jul  6 14:38:35 2023, max compression
+gzip compressed data, was "tutor-contrib-aspects-0.9.0.tar", last modified: Thu Jul  6 15:04:11 2023, max compression
```

## Comparing `tutor-contrib-aspects-0.8.0.tar` & `tutor-contrib-aspects-0.9.0.tar`

### file list

```diff
@@ -1,118 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.909980 tutor-contrib-aspects-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12239 2023-07-06 14:38:35.909980 tutor-contrib-aspects-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-06 14:38:35.909980 tutor-contrib-aspects-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.897980 tutor-contrib-aspects-0.8.0/tutor_contrib_aspects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12239 2023-07-06 14:38:35.000000 tutor-contrib-aspects-0.8.0/tutor_contrib_aspects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-07-06 14:38:35.000000 tutor-contrib-aspects-0.8.0/tutor_contrib_aspects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 14:38:35.000000 tutor-contrib-aspects-0.8.0/tutor_contrib_aspects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-06 14:38:35.000000 tutor-contrib-aspects-0.8.0/tutor_contrib_aspects.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 14:38:35.000000 tutor-contrib-aspects-0.8.0/tutor_contrib_aspects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 14:38:35.000000 tutor-contrib-aspects-0.8.0/tutor_contrib_aspects.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.897980 tutor-contrib-aspects-0.8.0/tutoraspects/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.901980 tutor-contrib-aspects-0.8.0/tutoraspects/patches/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/patches/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/patches/caddyfile
--rw-r--r--   0 runner    (1001) docker     (123)    16514 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/patches/k8s-deployments
--rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/patches/k8s-jobs
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/patches/k8s-services
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/patches/k8s-volumes
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/patches/kustomization-configmapgenerator
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/patches/local-docker-compose-dev-services
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/patches/local-docker-compose-jobs-services
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/patches/local-docker-compose-services
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/patches/openedx-cms-common-settings
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/patches/superset-extra-assets
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/patches/superset-jinja-filters
--rw-r--r--   0 runner    (1001) docker     (123)    22371 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.901980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.897980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.901980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.897980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.901980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/dbt/dbt_project.yml
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/dbt/packages.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/dbt/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.901980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.901980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.901980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0001_get_org_from_course_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0002_raw_xapi_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0003_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0004_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0005_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0006_navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0007_event_sink.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0008_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.905980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/scripts/alembic.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      654 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/scripts/clickhouse-demo-xapi-data.sh
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.897980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/clickhouse/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.905980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/clickhouse/config/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/clickhouse/config/docker_config.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.897980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/ralph/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.905980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/ralph/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/ralph/config/env
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.905980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/
--rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/auth.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.905980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.905980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/docker/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2113 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/docker/requirements-local.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.905980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/
--rw-r--r--   0 runner    (1001) docker     (123)    45916 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/assets.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.905980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/dim_course_videos.sql
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/dim_courses.sql
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_enrollments.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_enrollments_by_day.sql
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_transcript_usage.sql
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_video_plays.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.905980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/security/
--rw-r--r--   0 runner    (1001) docker     (123)    95955 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/security/roles.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.905980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/vector/
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/vector/file.toml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/vector/k8s.toml
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/vector/local.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.905980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/vector/partials/
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/vector/partials/common-pre.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.909980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/build/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/build/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.909980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/build/aspects/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/build/aspects/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/build/aspects/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.909980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/build/aspects-superset/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/build/aspects-superset/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.897980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/jobs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.909980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/jobs/init/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/jobs/init/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.909980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/jobs/init/aspects/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/jobs/init/aspects/init-aspects.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.909980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/jobs/init/clickhouse/
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.909980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/jobs/init/superset/
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/jobs/init/superset/init-mysql.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/jobs/init/superset/init-openedx.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     2852 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/base-docker-compose-services
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.673563 tutor-contrib-aspects-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12239 2023-07-06 15:04:11.673563 tutor-contrib-aspects-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-06 15:04:11.673563 tutor-contrib-aspects-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.661563 tutor-contrib-aspects-0.9.0/tutor_contrib_aspects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12239 2023-07-06 15:04:11.000000 tutor-contrib-aspects-0.9.0/tutor_contrib_aspects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-07-06 15:04:11.000000 tutor-contrib-aspects-0.9.0/tutor_contrib_aspects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 15:04:11.000000 tutor-contrib-aspects-0.9.0/tutor_contrib_aspects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-06 15:04:11.000000 tutor-contrib-aspects-0.9.0/tutor_contrib_aspects.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 15:04:11.000000 tutor-contrib-aspects-0.9.0/tutor_contrib_aspects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 15:04:11.000000 tutor-contrib-aspects-0.9.0/tutor_contrib_aspects.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.661563 tutor-contrib-aspects-0.9.0/tutoraspects/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/commands_v0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/commands_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.665563 tutor-contrib-aspects-0.9.0/tutoraspects/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/patches/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/patches/caddyfile
+-rw-r--r--   0 runner    (1001) docker     (123)    16514 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/patches/k8s-deployments
+-rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/patches/k8s-jobs
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/patches/k8s-services
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/patches/k8s-volumes
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/patches/kustomization-configmapgenerator
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/patches/local-docker-compose-dev-services
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/patches/local-docker-compose-jobs-services
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/patches/local-docker-compose-services
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/patches/openedx-cms-common-settings
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/patches/superset-extra-assets
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/patches/superset-jinja-filters
+-rw-r--r--   0 runner    (1001) docker     (123)    19884 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.665563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.661563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.665563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.657563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.665563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/dbt/dbt_project.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/dbt/packages.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/dbt/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.665563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.665563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.669563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0001_get_org_from_course_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0002_raw_xapi_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0003_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0004_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0005_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0006_navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0007_event_sink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0008_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.669563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/scripts/alembic.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      654 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/scripts/clickhouse-demo-xapi-data.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.657563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/clickhouse/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.669563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/clickhouse/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/clickhouse/config/docker_config.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.657563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/ralph/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.669563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/ralph/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/ralph/config/env
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.669563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/auth.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.669563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.669563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/docker/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2113 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/docker/requirements-local.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.669563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/
+-rw-r--r--   0 runner    (1001) docker     (123)    45916 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/assets.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.669563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/dim_course_videos.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/dim_courses.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_enrollments.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_enrollments_by_day.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_transcript_usage.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_video_plays.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.669563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/security/
+-rw-r--r--   0 runner    (1001) docker     (123)    95955 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/security/roles.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.673563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/vector/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/vector/file.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/vector/k8s.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/vector/local.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.673563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/vector/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/vector/partials/common-pre.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.673563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/build/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/build/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.673563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/build/aspects/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/build/aspects/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/build/aspects/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.673563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/build/aspects-superset/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/build/aspects-superset/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.661563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/jobs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.673563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/jobs/init/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/jobs/init/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.673563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/jobs/init/aspects/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/jobs/init/aspects/init-aspects.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.673563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/jobs/init/clickhouse/
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:04:11.673563 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/jobs/init/superset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/jobs/init/superset/init-mysql.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/jobs/init/superset/init-openedx.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2852 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-06 15:04:04.000000 tutor-contrib-aspects-0.9.0/tutoraspects/templates/base-docker-compose-services
```

### Comparing `tutor-contrib-aspects-0.8.0/PKG-INFO` & `tutor-contrib-aspects-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-contrib-aspects
-Version: 0.8.0
+Version: 0.9.0
 Summary: Aspects plugin for Tutor
 Home-page: https://github.com/open-craft/tutor-contrib-aspects
 Author: The Open edX Community
 License: AGPLv3
 Project-URL: Code, https://github.com/open-craft/tutor-contrib-aspects
 Project-URL: Issue tracker, https://github.com/open-craft/tutor-contrib-aspects/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tutor-contrib-aspects-0.8.0/README.rst` & `tutor-contrib-aspects-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/setup.py` & `tutor-contrib-aspects-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutor_contrib_aspects.egg-info/PKG-INFO` & `tutor-contrib-aspects-0.9.0/tutor_contrib_aspects.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-contrib-aspects
-Version: 0.8.0
+Version: 0.9.0
 Summary: Aspects plugin for Tutor
 Home-page: https://github.com/open-craft/tutor-contrib-aspects
 Author: The Open edX Community
 License: AGPLv3
 Project-URL: Code, https://github.com/open-craft/tutor-contrib-aspects
 Project-URL: Issue tracker, https://github.com/open-craft/tutor-contrib-aspects/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tutor-contrib-aspects-0.8.0/tutor_contrib_aspects.egg-info/SOURCES.txt` & `tutor-contrib-aspects-0.9.0/tutor_contrib_aspects.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 tutor_contrib_aspects.egg-info/SOURCES.txt
 tutor_contrib_aspects.egg-info/dependency_links.txt
 tutor_contrib_aspects.egg-info/entry_points.txt
 tutor_contrib_aspects.egg-info/requires.txt
 tutor_contrib_aspects.egg-info/top_level.txt
 tutoraspects/__about__.py
 tutoraspects/__init__.py
+tutoraspects/commands_v0.py
+tutoraspects/commands_v1.py
 tutoraspects/plugin.py
 tutoraspects/patches/.gitignore
 tutoraspects/patches/caddyfile
 tutoraspects/patches/k8s-deployments
 tutoraspects/patches/k8s-jobs
 tutoraspects/patches/k8s-services
 tutoraspects/patches/k8s-volumes
```

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/patches/k8s-deployments` & `tutor-contrib-aspects-0.9.0/tutoraspects/patches/k8s-deployments`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/patches/k8s-jobs` & `tutor-contrib-aspects-0.9.0/tutoraspects/patches/k8s-jobs`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/patches/k8s-services` & `tutor-contrib-aspects-0.9.0/tutoraspects/patches/k8s-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/patches/k8s-volumes` & `tutor-contrib-aspects-0.9.0/tutoraspects/patches/k8s-volumes`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/patches/kustomization-configmapgenerator` & `tutor-contrib-aspects-0.9.0/tutoraspects/patches/kustomization-configmapgenerator`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/patches/local-docker-compose-dev-services` & `tutor-contrib-aspects-0.9.0/tutoraspects/patches/local-docker-compose-dev-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/patches/local-docker-compose-jobs-services` & `tutor-contrib-aspects-0.9.0/tutoraspects/patches/local-docker-compose-jobs-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/patches/local-docker-compose-services` & `tutor-contrib-aspects-0.9.0/tutoraspects/patches/local-docker-compose-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/plugin.py` & `tutor-contrib-aspects-0.9.0/tutoraspects/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 import bcrypt
 import click
 import pkg_resources
 import yaml
 from tutor import hooks
 
 from .__about__ import __version__
+from .commands_v0 import COMMANDS as TUTOR_V0_COMMANDS
+from .commands_v1 import COMMANDS as TUTOR_V1_COMMANDS
 
 ########################################
 # CONFIGURATION
 ########################################
 
 hooks.Filters.CONFIG_DEFAULTS.add_items(
     [
@@ -314,21 +316,29 @@
     ("superset", ("aspects", "jobs", "init", "superset", "init-superset.sh"), 95),
     ("lms", ("aspects", "jobs", "init", "superset", "init-openedx.sh"), 96),
 ]
 
 # For each task added to MY_INIT_TASKS, we load the task template
 # and add it to the CLI_DO_INIT_TASKS filter, which tells Tutor to
 # run it as part of the `init` job.
-for service, template_path, priority in MY_INIT_TASKS:
-    full_path: str = pkg_resources.resource_filename(
-        "tutoraspects", os.path.join("templates", *template_path)
-    )
-    with open(full_path, encoding="utf-8") as init_task_file:
-        init_task: str = init_task_file.read()
-    hooks.Filters.CLI_DO_INIT_TASKS.add_item((service, init_task), priority=priority)
+try:
+    for service, template_path, priority in MY_INIT_TASKS:
+        hooks.Filters.COMMANDS_INIT.add_item(
+            (service, template_path)
+        )  # pylint: disable=no-member
+except AttributeError as e:
+    for service, template_path, priority in MY_INIT_TASKS:
+        full_path: str = pkg_resources.resource_filename(
+            "tutoraspects", os.path.join("templates", *template_path)
+        )
+        with open(full_path, encoding="utf-8") as init_task_file:
+            init_task: str = init_task_file.read()
+        hooks.Filters.CLI_DO_INIT_TASKS.add_item(
+            (service, init_task), priority=priority
+        )
 
 ########################################
 # DOCKER IMAGE MANAGEMENT
 ########################################
 
 
 # Images to be built by `tutor images build`.
@@ -421,112 +431,30 @@
         pkg_resources.resource_filename("tutoraspects", "patches"),
         "*",
     )
 ):
     with open(path, encoding="utf-8") as patch_file:
         hooks.Filters.ENV_PATCHES.add_item((os.path.basename(path), patch_file.read()))
 
-
 ########################################
 # CUSTOM JOBS (a.k.a. "do-commands")
 ########################################
-# Ex: "tutor local do load-xapi-test-data"
-@click.command()
-@click.option("-n", "--num_batches", default=100)
-@click.option("-s", "--batch_size", default=100)
-def load_xapi_test_data(num_batches: int, batch_size: int) -> list[tuple[str, str]]:
-    """
-    Job that loads bogus test xAPI data to ClickHouse via Ralph.
-    """
-    return [
-        (
-            "echo 'Making demo xapi script executable...' && "
-            "chmod +x /app/aspects/scripts/clickhouse-demo-xapi-data.sh && "
-            "echo 'Done. Running script...' && "
-            f"bash /app/aspects/scripts/clickhouse-demo-xapi-data.sh {num_batches}"
-            f" {batch_size} && "
-            "echo 'Done!';",
-        ),
-    ]
-
-
-# Ex: "tutor local do dbt "
-@click.command(context_settings={"ignore_unknown_options": True})
-@click.option(
-    "-c",
-    "--command",
-    default="run",
-    type=click.UNPROCESSED,
-    help="""The full dbt command to run configured ClickHouse database, wrapped in
-         double quotes. The list of commands can be found in the CLI section here:
-         https://docs.getdbt.com/reference/dbt-commands
-         
-         Examples: 
-         
-         tutor local do dbt -c "test"
-         
-         tutor local do dbt -c "run -m enrollments_by_day --threads 4"
-         """,
-)
-def dbt(command: string) -> list[tuple[str, str]]:
-    """
-    Job that proxies dbt commands to a container which runs them against ClickHouse.
-    """
-    return [
-        (
-            "aspects",
-            "echo 'Making dbt script executable...' && "
-            "chmod +x /app/aspects/scripts/dbt.sh && "
-            f"echo 'Running dbt {command}' && "
-            f"bash /app/aspects/scripts/dbt.sh {command} && "
-            "echo 'Done!';",
-        ),
-    ]
-
-
-# Ex: "tutor local do alembic "
-@click.command(context_settings={"ignore_unknown_options": True})
-@click.option(
-    "-c",
-    "--command",
-    default="run",
-    type=click.UNPROCESSED,
-    help="""The full alembic command to run configured ClickHouse database, wrapped in
-            double quotes. The list of commands can be found in the CLI section here:
-            https://alembic.sqlalchemy.org/en/latest/cli.html#command-reference
-            Examples:
-            
-            tutor local do alembic -c "current" # Show current revision
-            tutor local do alembic -c "history" # Show revision history
-            tutor local do alembic -c "revision --autogenerate -m 'Add new table'" # Create new revision
-            tutor local do alembic -c "upgrade head" # Upgrade to latest migrations
-            tutor local do alembic -c "downgrade base" # Downgrade to base migration
-         """,
-)
-def alembic(command: string) -> list[tuple[str, str]]:
-    """
-    Job that proxies alembic commands to a container which runs them against ClickHouse.
-    """
-    return [
-        (
-            "aspects",
-            "echo 'Making dbt script executable...' && "
-            "chmod +x /app/aspects/scripts/dbt.sh && "
-            f"bash /app/aspects/scripts/alembic.sh {command} && "
-            "echo 'Done!';",
-        ),
-    ]
-
-
-# Add the command function to CLI_DO_COMMANDS:
-hooks.Filters.CLI_DO_COMMANDS.add_item(load_xapi_test_data)
-hooks.Filters.CLI_DO_COMMANDS.add_item(dbt)
-hooks.Filters.CLI_DO_COMMANDS.add_item(alembic)
-
-
+# To keep compatibility with tutor14 we need to add the commands
+# directly to the dev|k8s|local command groups.
+try:
+    CLI_DO_COMMANDS = hooks.Filters.CLI_DO_COMMANDS
+except AttributeError:
+    from tutor.commands import dev, k8s, local
+
+    for f in TUTOR_V0_COMMANDS:
+        for mode in [dev.dev, local.local, k8s.k8s]:
+            mode.add_command(f)
+else:
+    for f in TUTOR_V1_COMMANDS:
+        CLI_DO_COMMANDS.add_item(f)
 #######################################
 # CUSTOM CLI COMMANDS
 #######################################
 
 # Your plugin can also add custom commands directly to the Tutor CLI.
 # These commands are run directly on the user's host computer
 # (unlike jobs, which are run in containers).
```

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml` & `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/README.rst` & `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/README.rst`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/env.py` & `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/env.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0001_get_org_from_course_url.py` & `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0001_get_org_from_course_url.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0002_raw_xapi_table.py` & `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0002_raw_xapi_table.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0003_enrollment.py` & `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0003_enrollment.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0004_video.py` & `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0004_video.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0005_problem.py` & `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0005_problem.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0006_navigation.py` & `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0006_navigation.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0007_event_sink.py` & `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0007_event_sink.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0008_vector.py` & `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0008_vector.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic.ini` & `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/scripts/clickhouse-demo-xapi-data.sh` & `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/scripts/clickhouse-demo-xapi-data.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh` & `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/ralph/config/env` & `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/ralph/config/env`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh` & `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/assets.yaml` & `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/assets.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py` & `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py` & `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py` & `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py` & `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/dim_course_videos.sql` & `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/dim_course_videos.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/dim_courses.sql` & `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/dim_courses.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_enrollments.sql` & `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_enrollments.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_enrollments_by_day.sql` & `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_enrollments_by_day.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_transcript_usage.sql` & `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_transcript_usage.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_video_plays.sql` & `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_video_plays.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py` & `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py` & `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/security/roles.json` & `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/superset/security/roles.json`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml` & `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh` & `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/jobs/init/superset/init-mysql.sh` & `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/jobs/init/superset/init-mysql.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/jobs/init/superset/init-openedx.sh` & `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/jobs/init/superset/init-openedx.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh` & `tutor-contrib-aspects-0.9.0/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.8.0/tutoraspects/templates/base-docker-compose-services` & `tutor-contrib-aspects-0.9.0/tutoraspects/templates/base-docker-compose-services`

 * *Files identical despite different names*

