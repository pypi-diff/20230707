# Comparing `tmp/scriptworker-8.1.1.tar.gz` & `tmp/scriptworker-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scriptworker-8.1.1.tar", last modified: Tue Feb 13 10:56:25 2018, max compression
+gzip compressed data, was "dist/scriptworker-9.0.0.tar", last modified: Tue Feb 27 19:41:24 2018, max compression
```

## Comparing `scriptworker-8.1.1.tar` & `scriptworker-9.0.0.tar`

### file list

```diff
@@ -1,141 +1,136 @@
-drwxr-xr-x   0 jlorenzo  (1000) jlorenzo  (1000)        0 2018-02-13 10:56:25.000000 scriptworker-8.1.1/
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)    29891 2018-02-13 10:54:57.000000 scriptworker-8.1.1/CHANGELOG.md
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)       90 2018-02-13 10:54:57.000000 scriptworker-8.1.1/version.json
-drwxr-xr-x   0 jlorenzo  (1000) jlorenzo  (1000)        0 2018-02-13 10:56:25.000000 scriptworker-8.1.1/helper_scripts/
--rwxr-xr-x   0 jlorenzo  (1000) jlorenzo  (1000)      478 2017-03-20 10:09:57.000000 scriptworker-8.1.1/helper_scripts/gpg_helper.sh
--rwxr-xr-x   0 jlorenzo  (1000) jlorenzo  (1000)     2344 2017-03-20 10:09:57.000000 scriptworker-8.1.1/helper_scripts/create_gpg_keys.py
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)      416 2018-02-13 10:56:25.000000 scriptworker-8.1.1/PKG-INFO
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)      115 2017-01-13 09:46:40.000000 scriptworker-8.1.1/requirements-docs.txt
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)       47 2017-01-13 15:14:06.000000 scriptworker-8.1.1/.coveragerc
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)      563 2017-03-20 10:09:57.000000 scriptworker-8.1.1/MANIFEST.in
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)    27748 2018-01-25 10:18:48.000000 scriptworker-8.1.1/requirements-test-prod.txt
-drwxr-xr-x   0 jlorenzo  (1000) jlorenzo  (1000)        0 2018-02-13 10:56:25.000000 scriptworker-8.1.1/scriptworker/
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)     2634 2018-01-11 10:46:58.000000 scriptworker-8.1.1/scriptworker/exceptions.py
-drwxr-xr-x   0 jlorenzo  (1000) jlorenzo  (1000)        0 2018-02-13 10:56:25.000000 scriptworker-8.1.1/scriptworker/test/
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)     2012 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/test_version.py
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)    11537 2018-01-25 10:18:48.000000 scriptworker-8.1.1/scriptworker/test/test_integration.py
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)     2436 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/test_context.py
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)     8339 2018-01-31 17:21:15.000000 scriptworker-8.1.1/scriptworker/test/__init__.py
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)     4653 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/test_client.py
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)    10713 2018-01-31 17:21:15.000000 scriptworker-8.1.1/scriptworker/test/test_task.py
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)    31285 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/test_gpg.py
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)    54082 2018-01-31 17:21:15.000000 scriptworker-8.1.1/scriptworker/test/test_cot_verify.py
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)     3945 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/test_log.py
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)    12885 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/test_artifacts.py
-drwxr-xr-x   0 jlorenzo  (1000) jlorenzo  (1000)        0 2018-02-13 10:56:25.000000 scriptworker-8.1.1/scriptworker/test/data/
--rwxr-xr-x   0 jlorenzo  (1000) jlorenzo  (1000)      198 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/gpg.sh
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)     9532 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/test_git_repo.tgz
-drwxr-xr-x   0 jlorenzo  (1000) jlorenzo  (1000)        0 2018-02-13 10:56:25.000000 scriptworker-8.1.1/scriptworker/test/data/gpg/
-drwxr-xr-x   0 jlorenzo  (1000) jlorenzo  (1000)        0 2018-02-13 10:56:25.000000 scriptworker-8.1.1/scriptworker/test/data/gpg/private-keys-v1.d/
--rw-------   0 jlorenzo  (1000) jlorenzo  (1000)      977 2018-02-13 10:14:17.000000 scriptworker-8.1.1/scriptworker/test/data/gpg/private-keys-v1.d/13435A7D795A0EDFE123D5A451B6A5B670DFA9FF.key
--rw-------   0 jlorenzo  (1000) jlorenzo  (1000)      977 2018-02-13 10:14:17.000000 scriptworker-8.1.1/scriptworker/test/data/gpg/private-keys-v1.d/45BC537FED9E18BCAF3D395776DCE3202608DC6A.key
--rw-------   0 jlorenzo  (1000) jlorenzo  (1000)      977 2018-02-13 10:14:13.000000 scriptworker-8.1.1/scriptworker/test/data/gpg/private-keys-v1.d/C5988D51364F8C7A157E276A346622A8ACA94653.key
--rw-------   0 jlorenzo  (1000) jlorenzo  (1000)      977 2018-02-13 10:14:17.000000 scriptworker-8.1.1/scriptworker/test/data/gpg/private-keys-v1.d/78458D66CA889DAEB13DECD75729160BAA505783.key
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)     3230 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/gpg/pubring.gpg
-drwxr-xr-x   0 jlorenzo  (1000) jlorenzo  (1000)        0 2018-02-13 10:56:25.000000 scriptworker-8.1.1/scriptworker/test/data/gpg/keys/
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)     1880 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/gpg/keys/docker.root@example.com.sec
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)      996 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/gpg/keys/scriptworker@example.com.pub
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)     1851 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/gpg/keys/unknown@example.com.sec
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)      996 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/gpg/keys/docker.root@example.com.pub
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)     1880 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/gpg/keys/scriptworker@example.com.sec
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)      992 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/gpg/keys/docker@example.com.pub
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)     1876 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/gpg/keys/docker@example.com.sec
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)      968 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/gpg/keys/unknown@example.com.pub
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)        0 2018-02-13 10:14:13.000000 scriptworker-8.1.1/scriptworker/test/data/gpg/.gpg-v21-migrated
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)      525 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/gpg/0.gpg
--rw-------   0 jlorenzo  (1000) jlorenzo  (1000)      600 2018-02-13 10:14:18.000000 scriptworker-8.1.1/scriptworker/test/data/gpg/random_seed
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)        2 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/gpg/0
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)     1440 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/gpg/trustdb.gpg
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)      212 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/gpg/gpg.conf
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)     5246 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/gpg/secring.gpg
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)      133 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/cot_config_schema.json
-drwxr-xr-x   0 jlorenzo  (1000) jlorenzo  (1000)        0 2018-02-13 10:56:25.000000 scriptworker-8.1.1/scriptworker/test/data/pubkeys/
-drwxr-xr-x   0 jlorenzo  (1000) jlorenzo  (1000)        0 2018-02-13 10:56:25.000000 scriptworker-8.1.1/scriptworker/test/data/pubkeys/unsigned/
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)      926 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/pubkeys/unsigned/D1B5423204A833E7A3420C803112C5A1B0BB87EA.unsigned.pub
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)      926 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/pubkeys/unsigned/EB55E1CED1FF0956E2BFE6C8D0B3B9C1094A9A3F.unsigned.pub
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)      926 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/pubkeys/unsigned/3F4DF62D10F3AD93E98119180C0D5CA75269246A.unsigned.pub
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)      926 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/pubkeys/unsigned/36E592251DFD8D491E6E9BE701222703321F2BA2.unsigned.pub
-drwxr-xr-x   0 jlorenzo  (1000) jlorenzo  (1000)        0 2018-02-13 10:56:25.000000 scriptworker-8.1.1/scriptworker/test/data/pubkeys/docker@example.com/
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)     1316 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/pubkeys/docker@example.com/3F4DF62D10F3AD93E98119180C0D5CA75269246A.pub
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)     1316 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/pubkeys/docker@example.com/36E592251DFD8D491E6E9BE701222703321F2BA2.pub
-drwxr-xr-x   0 jlorenzo  (1000) jlorenzo  (1000)        0 2018-02-13 10:56:25.000000 scriptworker-8.1.1/scriptworker/test/data/pubkeys/docker.root@example.com/
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)     1316 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/pubkeys/docker.root@example.com/EB55E1CED1FF0956E2BFE6C8D0B3B9C1094A9A3F.pub
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)     1316 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/pubkeys/docker.root@example.com/D1B5423204A833E7A3420C803112C5A1B0BB87EA.pub
-drwxr-xr-x   0 jlorenzo  (1000) jlorenzo  (1000)        0 2018-02-13 10:56:25.000000 scriptworker-8.1.1/scriptworker/test/data/pubkeys/data/
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)      528 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/pubkeys/data/EB55E1CED1FF0956E2BFE6C8D0B3B9C1094A9A3F.asc
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)      528 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/pubkeys/data/3F4DF62D10F3AD93E98119180C0D5CA75269246A.asc
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)      528 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/pubkeys/data/D1B5423204A833E7A3420C803112C5A1B0BB87EA.asc
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)      528 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/pubkeys/data/36E592251DFD8D491E6E9BE701222703321F2BA2.asc
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)     1782 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/pubkeys/manifest.json
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)       98 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/basic_task.json
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)      652 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/basic_schema.json
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)       28 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/client_credentials.json
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)      355 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/no_creds.json
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)       15 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/cot_config.json
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)       32 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/bad.json
--rwxr-xr-x   0 jlorenzo  (1000) jlorenzo  (1000)     4621 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/gen1000keys.py
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)        2 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/partial_credentials.json
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)      795 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/azure.xml
-drwxr-xr-x   0 jlorenzo  (1000) jlorenzo  (1000)        0 2018-02-13 10:56:25.000000 scriptworker-8.1.1/scriptworker/test/data/cotv2/
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)     2986 2018-01-25 10:18:48.000000 scriptworker-8.1.1/scriptworker/test/data/cotv2/decision_hg-push.json
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)   115188 2018-01-25 10:18:48.000000 scriptworker-8.1.1/scriptworker/test/data/cotv2/actions.json
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)     8482 2018-01-25 10:18:48.000000 scriptworker-8.1.1/scriptworker/test/data/cotv2/action_relpro.json
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)     2949 2018-01-25 10:18:48.000000 scriptworker-8.1.1/scriptworker/test/data/cotv2/cron.json
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)     7800 2018-01-25 10:18:48.000000 scriptworker-8.1.1/scriptworker/test/data/cotv2/.taskcluster.yml
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)      683 2018-01-25 10:18:48.000000 scriptworker-8.1.1/scriptworker/test/data/cotv2/parameters.yml
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)     9003 2018-01-25 10:18:48.000000 scriptworker-8.1.1/scriptworker/test/data/cotv2/projects.yml
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000) 10118318 2018-01-25 10:18:48.000000 scriptworker-8.1.1/scriptworker/test/data/cotv2/task-graph.json
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)      386 2018-01-25 10:18:48.000000 scriptworker-8.1.1/scriptworker/test/data/cotv2/pushlog.json
-drwxr-xr-x   0 jlorenzo  (1000) jlorenzo  (1000)        0 2018-02-13 10:56:25.000000 scriptworker-8.1.1/scriptworker/test/data/artifacts/
-drwxr-xr-x   0 jlorenzo  (1000) jlorenzo  (1000)        0 2018-02-13 10:56:25.000000 scriptworker-8.1.1/scriptworker/test/data/artifacts/public/
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)        4 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/artifacts/public/foo
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)        4 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/artifacts/public/baz
-drwxr-xr-x   0 jlorenzo  (1000) jlorenzo  (1000)        0 2018-02-13 10:56:25.000000 scriptworker-8.1.1/scriptworker/test/data/artifacts/public/logs/
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)        4 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/artifacts/public/logs/bar
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)      452 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/good.json
--rwxr-xr-x   0 jlorenzo  (1000) jlorenzo  (1000)     6286 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/check_pubkeys.py
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)     1824 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/long_running.py
--rwxr-xr-x   0 jlorenzo  (1000) jlorenzo  (1000)      135 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/data/write_file.sh
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)     6427 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/test_worker.py
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)     3147 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/test/test_cot_generate.py
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)    14362 2018-01-25 10:18:48.000000 scriptworker-8.1.1/scriptworker/test/test_utils.py
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)     8528 2018-01-11 10:46:58.000000 scriptworker-8.1.1/scriptworker/test/test_config.py
-drwxr-xr-x   0 jlorenzo  (1000) jlorenzo  (1000)        0 2018-02-13 10:56:25.000000 scriptworker-8.1.1/scriptworker/cot/
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)       43 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/cot/__init__.py
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)    70815 2018-01-31 17:21:15.000000 scriptworker-8.1.1/scriptworker/cot/verify.py
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)     3657 2018-01-25 10:18:48.000000 scriptworker-8.1.1/scriptworker/cot/generate.py
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)    20925 2018-01-25 10:18:48.000000 scriptworker-8.1.1/scriptworker/utils.py
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)       20 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/__init__.py
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)     6426 2018-01-25 10:18:48.000000 scriptworker-8.1.1/scriptworker/context.py
--rwxr-xr-x   0 jlorenzo  (1000) jlorenzo  (1000)     2768 2018-02-13 10:54:57.000000 scriptworker-8.1.1/scriptworker/version.py
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)    15577 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/artifacts.py
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)     2949 2018-01-25 10:18:48.000000 scriptworker-8.1.1/scriptworker/client.py
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)     8218 2018-01-25 10:18:48.000000 scriptworker-8.1.1/scriptworker/config.py
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)     4975 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/log.py
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)    13122 2018-01-31 17:21:15.000000 scriptworker-8.1.1/scriptworker/constants.py
-drwxr-xr-x   0 jlorenzo  (1000) jlorenzo  (1000)        0 2018-02-13 10:56:25.000000 scriptworker-8.1.1/scriptworker/data/
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)     1206 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/data/cot_v1_schema.json
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)     4185 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/worker.py
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)    58522 2018-01-03 17:25:20.000000 scriptworker-8.1.1/scriptworker/gpg.py
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)    15800 2018-01-31 17:21:15.000000 scriptworker-8.1.1/scriptworker/task.py
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)     2550 2018-02-13 10:45:40.000000 scriptworker-8.1.1/setup.py
-drwxr-xr-x   0 jlorenzo  (1000) jlorenzo  (1000)        0 2018-02-13 10:56:25.000000 scriptworker-8.1.1/scriptworker.egg-info/
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)      416 2018-02-13 10:56:25.000000 scriptworker-8.1.1/scriptworker.egg-info/PKG-INFO
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)     4921 2018-02-13 10:56:25.000000 scriptworker-8.1.1/scriptworker.egg-info/SOURCES.txt
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)       13 2018-02-13 10:56:25.000000 scriptworker-8.1.1/scriptworker.egg-info/top_level.txt
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)      133 2018-02-13 10:56:25.000000 scriptworker-8.1.1/scriptworker.egg-info/requires.txt
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)        1 2018-02-13 10:56:25.000000 scriptworker-8.1.1/scriptworker.egg-info/dependency_links.txt
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)        1 2017-01-06 15:17:38.000000 scriptworker-8.1.1/scriptworker.egg-info/not-zip-safe
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)      174 2018-02-13 10:56:25.000000 scriptworker-8.1.1/scriptworker.egg-info/entry_points.txt
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)      133 2018-02-13 10:45:40.000000 scriptworker-8.1.1/requirements-dev.txt
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)      824 2018-01-03 13:15:15.000000 scriptworker-8.1.1/tox.ini
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)    15792 2018-01-25 10:18:48.000000 scriptworker-8.1.1/requirements-prod.txt
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)     2856 2017-01-13 09:46:40.000000 scriptworker-8.1.1/CONTRIBUTING.rst
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)       61 2018-02-13 10:56:25.000000 scriptworker-8.1.1/setup.cfg
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)    15922 2017-01-13 09:46:40.000000 scriptworker-8.1.1/LICENSE
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)      155 2017-01-13 09:46:40.000000 scriptworker-8.1.1/requirements-test-dev.txt
-drwxr-xr-x   0 jlorenzo  (1000) jlorenzo  (1000)        0 2018-02-13 10:56:25.000000 scriptworker-8.1.1/docker/
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)      867 2017-01-11 16:36:10.000000 scriptworker-8.1.1/docker/Dockerfile.gnupg
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)      425 2017-01-06 13:56:42.000000 scriptworker-8.1.1/docker/Dockerfile.test
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)      636 2017-01-06 13:56:42.000000 scriptworker-8.1.1/docker/gnupg.yaml
--rw-r--r--   0 jlorenzo  (1000) jlorenzo  (1000)     2857 2017-10-17 13:23:13.000000 scriptworker-8.1.1/README.rst
+drwxr-xr-x   0 asasaki    (501) staff       (20)        0 2018-02-27 19:41:24.000000 scriptworker-9.0.0/
+-rw-r--r--   0 asasaki    (501) staff       (20)      416 2018-02-27 19:41:24.000000 scriptworker-9.0.0/PKG-INFO
+-rw-r--r--   0 asasaki    (501) staff       (20)       92 2018-02-27 00:49:41.000000 scriptworker-9.0.0/version.json
+drwxr-xr-x   0 asasaki    (501) staff       (20)        0 2018-02-27 19:41:23.000000 scriptworker-9.0.0/scriptworker.egg-info/
+-rw-r--r--   0 asasaki    (501) staff       (20)      416 2018-02-27 19:41:23.000000 scriptworker-9.0.0/scriptworker.egg-info/PKG-INFO
+-rw-r--r--   0 asasaki    (501) staff       (20)        1 2016-08-29 19:15:34.000000 scriptworker-9.0.0/scriptworker.egg-info/not-zip-safe
+-rw-r--r--   0 asasaki    (501) staff       (20)     4556 2018-02-27 19:41:23.000000 scriptworker-9.0.0/scriptworker.egg-info/SOURCES.txt
+-rw-r--r--   0 asasaki    (501) staff       (20)      174 2018-02-27 19:41:23.000000 scriptworker-9.0.0/scriptworker.egg-info/entry_points.txt
+-rw-r--r--   0 asasaki    (501) staff       (20)      133 2018-02-27 19:41:23.000000 scriptworker-9.0.0/scriptworker.egg-info/requires.txt
+-rw-r--r--   0 asasaki    (501) staff       (20)       13 2018-02-27 19:41:23.000000 scriptworker-9.0.0/scriptworker.egg-info/top_level.txt
+-rw-r--r--   0 asasaki    (501) staff       (20)        1 2018-02-27 19:41:23.000000 scriptworker-9.0.0/scriptworker.egg-info/dependency_links.txt
+drwxr-xr-x   0 asasaki    (501) staff       (20)        0 2018-02-27 19:41:23.000000 scriptworker-9.0.0/scriptworker/
+-rw-r--r--   0 asasaki    (501) staff       (20)     4464 2018-02-27 00:47:22.000000 scriptworker-9.0.0/scriptworker/worker.py
+-rw-r--r--   0 asasaki    (501) staff       (20)    15800 2018-02-08 18:27:02.000000 scriptworker-9.0.0/scriptworker/task.py
+-rw-r--r--   0 asasaki    (501) staff       (20)     8218 2018-01-19 00:15:19.000000 scriptworker-9.0.0/scriptworker/config.py
+-rwxr-xr-x   0 asasaki    (501) staff       (20)     2768 2018-02-27 00:49:38.000000 scriptworker-9.0.0/scriptworker/version.py
+drwxr-xr-x   0 asasaki    (501) staff       (20)        0 2018-02-27 19:41:23.000000 scriptworker-9.0.0/scriptworker/test/
+-rw-r--r--   0 asasaki    (501) staff       (20)     3147 2017-01-23 18:55:15.000000 scriptworker-9.0.0/scriptworker/test/test_cot_generate.py
+-rw-r--r--   0 asasaki    (501) staff       (20)     2012 2016-08-29 19:21:38.000000 scriptworker-9.0.0/scriptworker/test/test_version.py
+-rw-r--r--   0 asasaki    (501) staff       (20)    54105 2018-02-27 00:47:22.000000 scriptworker-9.0.0/scriptworker/test/test_cot_verify.py
+-rw-r--r--   0 asasaki    (501) staff       (20)    14362 2018-01-22 17:06:32.000000 scriptworker-9.0.0/scriptworker/test/test_utils.py
+-rw-r--r--   0 asasaki    (501) staff       (20)    10713 2018-02-08 18:27:02.000000 scriptworker-9.0.0/scriptworker/test/test_task.py
+-rw-r--r--   0 asasaki    (501) staff       (20)     8339 2018-02-08 18:27:02.000000 scriptworker-9.0.0/scriptworker/test/__init__.py
+-rw-r--r--   0 asasaki    (501) staff       (20)    12885 2018-01-03 18:14:09.000000 scriptworker-9.0.0/scriptworker/test/test_artifacts.py
+-rw-r--r--   0 asasaki    (501) staff       (20)     3945 2017-08-22 21:59:28.000000 scriptworker-9.0.0/scriptworker/test/test_log.py
+-rw-r--r--   0 asasaki    (501) staff       (20)     7232 2018-02-27 00:47:22.000000 scriptworker-9.0.0/scriptworker/test/test_worker.py
+-rw-r--r--   0 asasaki    (501) staff       (20)     8528 2018-01-04 22:23:23.000000 scriptworker-9.0.0/scriptworker/test/test_config.py
+-rw-r--r--   0 asasaki    (501) staff       (20)     2436 2017-01-23 18:55:15.000000 scriptworker-9.0.0/scriptworker/test/test_context.py
+-rw-r--r--   0 asasaki    (501) staff       (20)    11540 2018-02-27 00:47:22.000000 scriptworker-9.0.0/scriptworker/test/test_integration.py
+-rw-r--r--   0 asasaki    (501) staff       (20)    31285 2018-01-03 18:14:09.000000 scriptworker-9.0.0/scriptworker/test/test_gpg.py
+-rw-r--r--   0 asasaki    (501) staff       (20)     4653 2017-01-23 18:55:15.000000 scriptworker-9.0.0/scriptworker/test/test_client.py
+drwxr-xr-x   0 asasaki    (501) staff       (20)        0 2018-02-27 19:41:23.000000 scriptworker-9.0.0/scriptworker/test/data/
+-rw-r--r--   0 asasaki    (501) staff       (20)     9532 2017-02-09 15:02:57.000000 scriptworker-9.0.0/scriptworker/test/data/test_git_repo.tgz
+-rw-r--r--   0 asasaki    (501) staff       (20)        2 2016-08-29 19:21:38.000000 scriptworker-9.0.0/scriptworker/test/data/partial_credentials.json
+-rwxr-xr-x   0 asasaki    (501) staff       (20)     4621 2017-01-23 18:55:15.000000 scriptworker-9.0.0/scriptworker/test/data/gen1000keys.py
+drwxr-xr-x   0 asasaki    (501) staff       (20)        0 2018-02-27 19:41:23.000000 scriptworker-9.0.0/scriptworker/test/data/artifacts/
+drwxr-xr-x   0 asasaki    (501) staff       (20)        0 2018-02-27 19:41:23.000000 scriptworker-9.0.0/scriptworker/test/data/artifacts/public/
+drwxr-xr-x   0 asasaki    (501) staff       (20)        0 2018-02-27 19:41:23.000000 scriptworker-9.0.0/scriptworker/test/data/artifacts/public/logs/
+-rw-r--r--   0 asasaki    (501) staff       (20)        4 2016-08-29 19:21:38.000000 scriptworker-9.0.0/scriptworker/test/data/artifacts/public/logs/bar
+-rw-r--r--   0 asasaki    (501) staff       (20)        4 2016-08-29 19:21:38.000000 scriptworker-9.0.0/scriptworker/test/data/artifacts/public/foo
+-rw-r--r--   0 asasaki    (501) staff       (20)        4 2016-08-29 19:21:38.000000 scriptworker-9.0.0/scriptworker/test/data/artifacts/public/baz
+-rwxr-xr-x   0 asasaki    (501) staff       (20)      198 2016-08-29 19:21:38.000000 scriptworker-9.0.0/scriptworker/test/data/gpg.sh
+drwxr-xr-x   0 asasaki    (501) staff       (20)        0 2018-02-27 19:41:24.000000 scriptworker-9.0.0/scriptworker/test/data/cotv2/
+-rw-r--r--   0 asasaki    (501) staff       (20)      683 2018-01-19 00:15:19.000000 scriptworker-9.0.0/scriptworker/test/data/cotv2/parameters.yml
+-rw-r--r--   0 asasaki    (501) staff       (20)     2986 2018-01-19 00:15:19.000000 scriptworker-9.0.0/scriptworker/test/data/cotv2/decision_hg-push.json
+-rw-r--r--   0 asasaki    (501) staff       (20)     2949 2018-01-19 00:15:19.000000 scriptworker-9.0.0/scriptworker/test/data/cotv2/cron.json
+-rw-r--r--   0 asasaki    (501) staff       (20)     8482 2018-01-19 00:15:19.000000 scriptworker-9.0.0/scriptworker/test/data/cotv2/action_relpro.json
+-rw-r--r--   0 asasaki    (501) staff       (20)   115188 2018-01-19 00:15:19.000000 scriptworker-9.0.0/scriptworker/test/data/cotv2/actions.json
+-rw-r--r--   0 asasaki    (501) staff       (20)     9003 2018-01-19 00:15:19.000000 scriptworker-9.0.0/scriptworker/test/data/cotv2/projects.yml
+-rw-r--r--   0 asasaki    (501) staff       (20)      386 2018-01-19 00:15:19.000000 scriptworker-9.0.0/scriptworker/test/data/cotv2/pushlog.json
+-rw-r--r--   0 asasaki    (501) staff       (20)     7800 2018-01-19 00:15:19.000000 scriptworker-9.0.0/scriptworker/test/data/cotv2/.taskcluster.yml
+-rw-r--r--   0 asasaki    (501) staff       (20) 10118318 2018-01-19 00:15:19.000000 scriptworker-9.0.0/scriptworker/test/data/cotv2/task-graph.json
+drwxr-xr-x   0 asasaki    (501) staff       (20)        0 2018-02-27 19:41:24.000000 scriptworker-9.0.0/scriptworker/test/data/gpg/
+-rw-r--r--   0 asasaki    (501) staff       (20)        2 2016-08-29 19:21:38.000000 scriptworker-9.0.0/scriptworker/test/data/gpg/0
+-rw-r--r--   0 asasaki    (501) staff       (20)     5246 2016-09-02 00:01:12.000000 scriptworker-9.0.0/scriptworker/test/data/gpg/secring.gpg
+-rw-r--r--   0 asasaki    (501) staff       (20)     3230 2016-09-02 00:01:12.000000 scriptworker-9.0.0/scriptworker/test/data/gpg/pubring.gpg
+-rw-r--r--   0 asasaki    (501) staff       (20)    26819 2016-09-01 23:58:55.000000 scriptworker-9.0.0/scriptworker/test/data/gpg/pubring.gpg~
+-rw-------   0 asasaki    (501) staff       (20)      600 2018-01-19 02:42:04.000000 scriptworker-9.0.0/scriptworker/test/data/gpg/random_seed
+-rw-r--r--   0 asasaki    (501) staff       (20)      525 2016-08-29 19:21:38.000000 scriptworker-9.0.0/scriptworker/test/data/gpg/0.gpg
+drwxr-xr-x   0 asasaki    (501) staff       (20)        0 2018-02-27 19:41:24.000000 scriptworker-9.0.0/scriptworker/test/data/gpg/keys/
+-rw-r--r--   0 asasaki    (501) staff       (20)      992 2016-08-29 19:21:38.000000 scriptworker-9.0.0/scriptworker/test/data/gpg/keys/docker@example.com.pub
+-rw-r--r--   0 asasaki    (501) staff       (20)     1851 2016-08-29 19:21:38.000000 scriptworker-9.0.0/scriptworker/test/data/gpg/keys/unknown@example.com.sec
+-rw-r--r--   0 asasaki    (501) staff       (20)     1880 2016-08-29 19:21:38.000000 scriptworker-9.0.0/scriptworker/test/data/gpg/keys/docker.root@example.com.sec
+-rw-r--r--   0 asasaki    (501) staff       (20)      996 2016-08-29 19:21:38.000000 scriptworker-9.0.0/scriptworker/test/data/gpg/keys/scriptworker@example.com.pub
+-rw-r--r--   0 asasaki    (501) staff       (20)     1876 2016-08-29 19:21:38.000000 scriptworker-9.0.0/scriptworker/test/data/gpg/keys/docker@example.com.sec
+-rw-r--r--   0 asasaki    (501) staff       (20)      968 2016-08-29 19:21:38.000000 scriptworker-9.0.0/scriptworker/test/data/gpg/keys/unknown@example.com.pub
+-rw-r--r--   0 asasaki    (501) staff       (20)      996 2016-08-29 19:21:38.000000 scriptworker-9.0.0/scriptworker/test/data/gpg/keys/docker.root@example.com.pub
+-rw-r--r--   0 asasaki    (501) staff       (20)     1880 2016-08-29 19:21:38.000000 scriptworker-9.0.0/scriptworker/test/data/gpg/keys/scriptworker@example.com.sec
+-rw-r--r--   0 asasaki    (501) staff       (20)      212 2016-09-15 22:28:44.000000 scriptworker-9.0.0/scriptworker/test/data/gpg/gpg.conf
+-rw-r--r--   0 asasaki    (501) staff       (20)     1440 2016-08-29 19:21:38.000000 scriptworker-9.0.0/scriptworker/test/data/gpg/trustdb.gpg
+-rwxr-xr-x   0 asasaki    (501) staff       (20)     6286 2016-10-31 17:41:11.000000 scriptworker-9.0.0/scriptworker/test/data/check_pubkeys.py
+-rw-r--r--   0 asasaki    (501) staff       (20)      133 2016-10-31 17:41:11.000000 scriptworker-9.0.0/scriptworker/test/data/cot_config_schema.json
+-rw-r--r--   0 asasaki    (501) staff       (20)     1824 2016-08-29 19:21:38.000000 scriptworker-9.0.0/scriptworker/test/data/long_running.py
+-rw-r--r--   0 asasaki    (501) staff       (20)      452 2017-01-23 18:55:15.000000 scriptworker-9.0.0/scriptworker/test/data/good.json
+-rwxr-xr-x   0 asasaki    (501) staff       (20)      135 2016-08-29 19:21:38.000000 scriptworker-9.0.0/scriptworker/test/data/write_file.sh
+-rw-r--r--   0 asasaki    (501) staff       (20)       32 2016-08-29 19:21:38.000000 scriptworker-9.0.0/scriptworker/test/data/bad.json
+-rw-r--r--   0 asasaki    (501) staff       (20)       15 2016-10-31 17:41:11.000000 scriptworker-9.0.0/scriptworker/test/data/cot_config.json
+-rw-r--r--   0 asasaki    (501) staff       (20)      795 2016-08-29 19:21:38.000000 scriptworker-9.0.0/scriptworker/test/data/azure.xml
+-rw-r--r--   0 asasaki    (501) staff       (20)      652 2016-08-29 19:21:38.000000 scriptworker-9.0.0/scriptworker/test/data/basic_schema.json
+-rw-r--r--   0 asasaki    (501) staff       (20)       28 2016-08-29 19:21:38.000000 scriptworker-9.0.0/scriptworker/test/data/client_credentials.json
+drwxr-xr-x   0 asasaki    (501) staff       (20)        0 2018-02-27 19:41:24.000000 scriptworker-9.0.0/scriptworker/test/data/pubkeys/
+drwxr-xr-x   0 asasaki    (501) staff       (20)        0 2018-02-27 19:41:24.000000 scriptworker-9.0.0/scriptworker/test/data/pubkeys/docker@example.com/
+-rw-r--r--   0 asasaki    (501) staff       (20)     1316 2016-09-15 22:28:44.000000 scriptworker-9.0.0/scriptworker/test/data/pubkeys/docker@example.com/3F4DF62D10F3AD93E98119180C0D5CA75269246A.pub
+-rw-r--r--   0 asasaki    (501) staff       (20)     1316 2016-09-15 22:28:44.000000 scriptworker-9.0.0/scriptworker/test/data/pubkeys/docker@example.com/36E592251DFD8D491E6E9BE701222703321F2BA2.pub
+drwxr-xr-x   0 asasaki    (501) staff       (20)        0 2018-02-27 19:41:24.000000 scriptworker-9.0.0/scriptworker/test/data/pubkeys/unsigned/
+-rw-r--r--   0 asasaki    (501) staff       (20)      926 2016-09-15 22:28:44.000000 scriptworker-9.0.0/scriptworker/test/data/pubkeys/unsigned/D1B5423204A833E7A3420C803112C5A1B0BB87EA.unsigned.pub
+-rw-r--r--   0 asasaki    (501) staff       (20)      926 2016-09-15 22:28:44.000000 scriptworker-9.0.0/scriptworker/test/data/pubkeys/unsigned/36E592251DFD8D491E6E9BE701222703321F2BA2.unsigned.pub
+-rw-r--r--   0 asasaki    (501) staff       (20)      926 2016-09-15 22:28:44.000000 scriptworker-9.0.0/scriptworker/test/data/pubkeys/unsigned/EB55E1CED1FF0956E2BFE6C8D0B3B9C1094A9A3F.unsigned.pub
+-rw-r--r--   0 asasaki    (501) staff       (20)      926 2016-09-15 22:28:44.000000 scriptworker-9.0.0/scriptworker/test/data/pubkeys/unsigned/3F4DF62D10F3AD93E98119180C0D5CA75269246A.unsigned.pub
+-rw-r--r--   0 asasaki    (501) staff       (20)     1782 2016-09-15 22:28:44.000000 scriptworker-9.0.0/scriptworker/test/data/pubkeys/manifest.json
+drwxr-xr-x   0 asasaki    (501) staff       (20)        0 2018-02-27 19:41:24.000000 scriptworker-9.0.0/scriptworker/test/data/pubkeys/docker.root@example.com/
+-rw-r--r--   0 asasaki    (501) staff       (20)     1316 2016-09-15 22:28:44.000000 scriptworker-9.0.0/scriptworker/test/data/pubkeys/docker.root@example.com/EB55E1CED1FF0956E2BFE6C8D0B3B9C1094A9A3F.pub
+-rw-r--r--   0 asasaki    (501) staff       (20)     1316 2016-09-15 22:28:44.000000 scriptworker-9.0.0/scriptworker/test/data/pubkeys/docker.root@example.com/D1B5423204A833E7A3420C803112C5A1B0BB87EA.pub
+drwxr-xr-x   0 asasaki    (501) staff       (20)        0 2018-02-27 19:41:24.000000 scriptworker-9.0.0/scriptworker/test/data/pubkeys/data/
+-rw-r--r--   0 asasaki    (501) staff       (20)      528 2016-09-15 22:28:44.000000 scriptworker-9.0.0/scriptworker/test/data/pubkeys/data/D1B5423204A833E7A3420C803112C5A1B0BB87EA.asc
+-rw-r--r--   0 asasaki    (501) staff       (20)      528 2016-09-15 22:28:44.000000 scriptworker-9.0.0/scriptworker/test/data/pubkeys/data/36E592251DFD8D491E6E9BE701222703321F2BA2.asc
+-rw-r--r--   0 asasaki    (501) staff       (20)      528 2016-09-15 22:28:44.000000 scriptworker-9.0.0/scriptworker/test/data/pubkeys/data/EB55E1CED1FF0956E2BFE6C8D0B3B9C1094A9A3F.asc
+-rw-r--r--   0 asasaki    (501) staff       (20)      528 2016-09-15 22:28:44.000000 scriptworker-9.0.0/scriptworker/test/data/pubkeys/data/3F4DF62D10F3AD93E98119180C0D5CA75269246A.asc
+-rw-r--r--   0 asasaki    (501) staff       (20)      355 2017-01-23 18:55:15.000000 scriptworker-9.0.0/scriptworker/test/data/no_creds.json
+-rw-r--r--   0 asasaki    (501) staff       (20)       98 2016-08-29 19:21:38.000000 scriptworker-9.0.0/scriptworker/test/data/basic_task.json
+-rw-r--r--   0 asasaki    (501) staff       (20)     4975 2017-08-22 21:59:28.000000 scriptworker-9.0.0/scriptworker/log.py
+-rw-r--r--   0 asasaki    (501) staff       (20)     2949 2018-01-19 00:15:19.000000 scriptworker-9.0.0/scriptworker/client.py
+-rw-r--r--   0 asasaki    (501) staff       (20)    13406 2018-02-27 00:47:22.000000 scriptworker-9.0.0/scriptworker/constants.py
+-rw-r--r--   0 asasaki    (501) staff       (20)       20 2017-01-23 18:55:15.000000 scriptworker-9.0.0/scriptworker/__init__.py
+drwxr-xr-x   0 asasaki    (501) staff       (20)        0 2018-02-27 19:41:23.000000 scriptworker-9.0.0/scriptworker/cot/
+-rw-r--r--   0 asasaki    (501) staff       (20)     3657 2018-01-19 00:15:19.000000 scriptworker-9.0.0/scriptworker/cot/generate.py
+-rw-r--r--   0 asasaki    (501) staff       (20)       43 2017-01-23 18:55:15.000000 scriptworker-9.0.0/scriptworker/cot/__init__.py
+-rw-r--r--   0 asasaki    (501) staff       (20)    71274 2018-02-27 00:47:22.000000 scriptworker-9.0.0/scriptworker/cot/verify.py
+-rw-r--r--   0 asasaki    (501) staff       (20)    58522 2018-01-03 18:14:09.000000 scriptworker-9.0.0/scriptworker/gpg.py
+-rw-r--r--   0 asasaki    (501) staff       (20)     6426 2018-01-19 00:15:19.000000 scriptworker-9.0.0/scriptworker/context.py
+-rw-r--r--   0 asasaki    (501) staff       (20)    20925 2018-01-22 17:06:32.000000 scriptworker-9.0.0/scriptworker/utils.py
+-rw-r--r--   0 asasaki    (501) staff       (20)     2634 2018-01-04 22:23:23.000000 scriptworker-9.0.0/scriptworker/exceptions.py
+-rw-r--r--   0 asasaki    (501) staff       (20)    15577 2018-01-03 18:14:09.000000 scriptworker-9.0.0/scriptworker/artifacts.py
+drwxr-xr-x   0 asasaki    (501) staff       (20)        0 2018-02-27 19:41:23.000000 scriptworker-9.0.0/scriptworker/data/
+-rw-r--r--   0 asasaki    (501) staff       (20)     1206 2016-09-15 22:28:44.000000 scriptworker-9.0.0/scriptworker/data/cot_v1_schema.json
+drwxr-xr-x   0 asasaki    (501) staff       (20)        0 2018-02-27 19:41:23.000000 scriptworker-9.0.0/docker/
+-rw-r--r--   0 asasaki    (501) staff       (20)      425 2017-02-27 20:04:36.000000 scriptworker-9.0.0/docker/Dockerfile.test
+-rw-r--r--   0 asasaki    (501) staff       (20)      636 2017-01-23 18:55:15.000000 scriptworker-9.0.0/docker/gnupg.yaml
+-rw-r--r--   0 asasaki    (501) staff       (20)      867 2017-02-13 02:22:12.000000 scriptworker-9.0.0/docker/Dockerfile.gnupg
+-rw-r--r--   0 asasaki    (501) staff       (20)    15922 2016-07-15 21:53:54.000000 scriptworker-9.0.0/LICENSE
+-rw-r--r--   0 asasaki    (501) staff       (20)      155 2017-01-23 18:55:15.000000 scriptworker-9.0.0/requirements-test-dev.txt
+-rw-r--r--   0 asasaki    (501) staff       (20)     2856 2016-08-29 19:21:38.000000 scriptworker-9.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 asasaki    (501) staff       (20)    30197 2018-02-27 01:07:41.000000 scriptworker-9.0.0/CHANGELOG.md
+-rw-r--r--   0 asasaki    (501) staff       (20)    17001 2018-02-27 02:12:27.000000 scriptworker-9.0.0/requirements-prod.txt
+-rw-r--r--   0 asasaki    (501) staff       (20)      115 2017-01-23 18:55:15.000000 scriptworker-9.0.0/requirements-docs.txt
+-rw-r--r--   0 asasaki    (501) staff       (20)      563 2017-03-20 18:52:24.000000 scriptworker-9.0.0/MANIFEST.in
+-rw-r--r--   0 asasaki    (501) staff       (20)       47 2016-08-29 19:21:38.000000 scriptworker-9.0.0/.coveragerc
+-rw-r--r--   0 asasaki    (501) staff       (20)    28361 2018-02-27 02:12:27.000000 scriptworker-9.0.0/requirements-test-prod.txt
+-rw-r--r--   0 asasaki    (501) staff       (20)     2550 2018-02-21 10:40:32.000000 scriptworker-9.0.0/setup.py
+-rw-r--r--   0 asasaki    (501) staff       (20)      133 2018-02-21 10:40:32.000000 scriptworker-9.0.0/requirements-dev.txt
+-rw-r--r--   0 asasaki    (501) staff       (20)      824 2017-10-20 18:55:51.000000 scriptworker-9.0.0/tox.ini
+-rw-r--r--   0 asasaki    (501) staff       (20)       82 2018-02-27 19:41:24.000000 scriptworker-9.0.0/setup.cfg
+-rw-r--r--   0 asasaki    (501) staff       (20)     2857 2018-01-03 18:14:09.000000 scriptworker-9.0.0/README.rst
+drwxr-xr-x   0 asasaki    (501) staff       (20)        0 2018-02-27 19:41:23.000000 scriptworker-9.0.0/helper_scripts/
+-rwxr-xr-x   0 asasaki    (501) staff       (20)      478 2017-03-20 18:52:24.000000 scriptworker-9.0.0/helper_scripts/gpg_helper.sh
+-rwxr-xr-x   0 asasaki    (501) staff       (20)     2344 2018-02-27 00:49:15.000000 scriptworker-9.0.0/helper_scripts/create_gpg_keys.py
```

### Comparing `scriptworker-8.1.1/CHANGELOG.md` & `scriptworker-9.0.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 # Change Log
 All notable changes to this project will be documented in this file.
 This project adheres to [Semantic Versioning](http://semver.org/).
 
+## [9.0.0] - 2018-02-27
+### Added
+- added support for bouncer scriptworker
+
+### Changed
+- renamed `run_loop` to `run_tasks`
+- `run_tasks` now shuts down gracefully after receiving a SIGTERM: it finishes the current task(s), and exits.
+
+### Fixed
+- `run_tasks` now sleeps 5 if there were no tasks claimed.
+
 ## [8.1.1] - 2018-02-13
 ### Fixed
 - Freeze aiohttp to 2.x.y
 
 ## [8.1.0] - 2018-01-31
 ### Added
 - `valid_vcs_rules`, `source_env_prefix`, `extra_run_task_arguments` depend on `cot_product`
```

### Comparing `scriptworker-8.1.1/helper_scripts/create_gpg_keys.py` & `scriptworker-9.0.0/helper_scripts/create_gpg_keys.py`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/MANIFEST.in` & `scriptworker-9.0.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/requirements-test-prod.txt` & `scriptworker-9.0.0/requirements-test-prod.txt`

 * *Files 11% similar despite different names*

```diff
@@ -10,89 +10,91 @@
     --hash=sha512:1b3e3c8c09308a84364d561de459ab8915cbd7cc43b7747e31582574b0f0cd7b1d3628c39b22d9c6f6a4d16226749ac1667290bc560482d997c53cfff5c832b7 \
     --hash=sha512:9a5af29dfdd74827c5d0032906daf821eaed27f0c20759af0acf29ae2b8d704300b508788832341a0014a78301ad1b726c5898e3a6fa49258c666e8d318ccda0 \
     --hash=sha512:1890e6b8aa96beb51f7a196ca287fd6ed905b99e6d139d7b29174478ce3947c0dd7bbe933116836a8276a483811054d928bc55774a5eb542789c3779b7b042bd \
     --hash=sha512:a9d2e9ae96e80e8cf8ae5a62513ac945093ef0aa59106e20ef650a1ed196748c5cd321f1da6ffaa965f4fb1b266cdaf5937bac3714d67df495855d5938645e90 \
     --hash=sha512:13733054619053893f4a8d75c1da020a87e1f697b007ab182be06b5b941b49c4cb3dc6f9ff131be6bc10fc727ad7334fa5401346f3a77140aed0f86280532fce \
     --hash=sha512:5ff411ddbbf733ad52334015a04eb061998803ff94ad474ea2d534a713aa302cdfadde908ff2bb1dbd4f13e1a1fb99786f8dd1be1e061fcb6a7c0f471e41591f \
     --hash=sha512:4ae6c5843688f45751ddb14a8b6f16f58b1f8a4805be430afa4035857b1826be95a8422395d64ac88282f9edd57f35fee5d1b6a4dab9093d47491d300d2079f3
-aiohttp==2.3.9 \
-    --hash=sha512:80d1fe481d6ce7d465252e27951c50f96e005ef54dd0fdf49269e2267d6b096a3a0c9e6a3aef75854559dbf57760651a7f36e1fdab3263cc0b33a17ade8d34cf \
-    --hash=sha512:5049d881d33bbbcb9997eef5ccc9eccff675c0f425806765b36af861ae10756fd8ec67b810b2a28436931b746077266aa1a450dc610a3cc36c195b4fd29b1804 \
-    --hash=sha512:8c599a34591b26d0c46e2c626a7e7c714b66ead04fbe130ce91ad1ded9953f4886beeb8e3551725460927ac177b95d03566b1fbaad7baebc30bbbeb600a599ab \
-    --hash=sha512:be8a6db5eb9f5974443ec26da816fcaaed59a1592d2686085523b13f732c5e25191cd47f27327b35fbdf4303ba9a6cd3a45f7f04a4c914544261c9af7a3cbee5 \
-    --hash=sha512:fb11ad5b2c849b107372e8d6a2b0fa2e29ddb83d524da8b036f4df03ed79292f2328fe5c6b80d7cc0b57059d27fcb151789238ce7f18f8eb6d34e9ede543a5e5 \
-    --hash=sha512:904ee46b2468c3fb9a7582e55a741cbb68294e9ae4feafc3493d4761345ebcc13969c76b87368d38ae3ca1aead47ca05577f20dd85342244c352cc0679b63d01 \
-    --hash=sha512:92df4fb2f369b663b544bc82813872e09c7171f7ddafdfa52ba0170eccb6e8ac0a75d1784f40a5559f9fecea84c8876157ee47918cb3eabb159176bf0ec84b26 \
-    --hash=sha512:798ef8f226613090595f0135a4b3441e084a16bb66ef085853a0463c05f4a1d275c4fd64013b0a23d8f28dbee53a689516f56a0f44526e5c537271792a175896 \
-    --hash=sha512:17ed05007b6e18d8d116ea188c0477dbfc5653d1d76cbfe521398f40e153a1d07223688a8a819190ed8c3f5a377930b25da1bb458822fbbfc16e3d17b190b07b \
-    --hash=sha512:5fb010146e341263db44e5e64277914a426aa3c5399c9d08965ab401119edcc45104075a52b80fdd8180dd444c2bd367e4bb5b2914afc63ae3f92e95643437e1 \
-    --hash=sha512:883905e1e6de254eba677143f03d9c5b308d5dd8826d07313b9da630ca6787478ce4c3bfbe11e3c808bc4179b3adab5140087b1cca2ee6bb80ee2bf3c315e713 \
-    --hash=sha512:af4a10ae986acac3909e3301e9a2cd232eea87f97ec30cc1ee12e62e926d57ba618f706bebe4f1599dd1352099d25f40a458ad497ed02b91316fc3d331f91d66 \
-    --hash=sha512:e0675ecbe27ef12f2165c2e8f3ed05e2205786797e72f0ae7ee2bede1fca1b932a41837fdacd2083195c30049f0d3ba020589144683aae3353c31d279e42a7ce \
-    --hash=sha512:944001747640008791d90820304ce8f0bff50e30c661a72fdd46f2c523996f0f25419bc231c8dfe298233c9a75c26ceab8370ec7c3fed06a17b9f6582d01a9fe \
-    --hash=sha512:bba4ed6ee2cffc53fbb8562135da1018cb2c0416af78ddb209a582c86215cef5ce4db17262b58d834f87e9103d0ce47539cc7507cd5ed9f8ee3aa69c3c4f6f5f \
-    --hash=sha512:0fe2bbcfc5b9b145a129ebee3b802e9dff5bc00030ce1fa5cea8bb63575be71c657289a92a020fb4fe8b9b5d5a0871234a630c3e9562a464cd43741b19a3b82f
-arrow==0.12.0 \
-    --hash=sha512:bbe4bd0b80de680079fdd5e4575750525df714a98945ea7b8e28b88def0bb094a928083d0afb71d5d7e9294feadf44d070239b5566c866a0fe67fbb7274061b5
-async_generator==1.8 \
-    --hash=sha512:cdf87f8858ea896b36bd52167866fc528cb3abdaaeec51cda0eb8319e18737260b1d4a0584b7d60f00e36c1647a54771b5198ffda84eed148b53c07aedd956b4 \
-    --hash=sha512:7203994d6f00e2cae9e923ea76fa145a2caaba73bb9b16419d875936bf7b8078aad1b1f99d311ad4b88a00b06093031977e70e62435846f7e6e85b899e382f68
+aiohttp==2.3.10 \
+    --hash=sha512:15345f91cff581f6b6b9ec099504564749a4f054b60cb5757e8af740235aea0711cb8c15ad1dc54a0caedf73039493b5a1d21a98e2a80c5c0f3d83a63cc58ea1 \
+    --hash=sha512:9cad43b6021d40f8d4bf01e7d64f7d2fb26eeab112476b34141ffa450338078a7fd3aa56fdd782994c2b7215e28d6d0bf573f7696600625a16bebd871eae2393 \
+    --hash=sha512:0da9d1b885a16adf1d4f6ca63cbbf92c747e242a02d7d95c6f453fff57a84506cb7c36dbd93b1708a4eddd1c248da22a1eaf39864432daafd598b6531074ef99 \
+    --hash=sha512:3527178423dbc5a3c55dc1d13b3ab341f28be07edf3eb0c68c9fccb08dddc9ea1c26bbcffe361e42069d1472a0abaf4e8a9d274b6049664698160b55e6a40b76 \
+    --hash=sha512:8b4691d6aa9146c14a1cdf0f488cbca804654fa58311d15f34f9b1edbaed59d923e34b4ef28a0b206eb99fbf078fa41bf2cf3e36e9dc116679f5aec997c2cf09 \
+    --hash=sha512:05e581a5c08f16443b10a8c49e9e7c2cfbd0ca3d95e4150bd59458c0c865429fab6fbd37aba53402ceac5fd3dceecfcbce48e8c7389b9b74c7eb17ecbfc35699 \
+    --hash=sha512:b3caaaffdec94e5a542a5d0246e6c4a88ea290d4a03fdb3a0c43cdbe646ff44a0a9ad4c5dfef08e017ea4edf6ebc7d6dbe06b435439b0b743d7cf09479c35f6f \
+    --hash=sha512:7581a091f011578fbf689b9245e2f307599e1694e97f0baf66973632ad1e4c6370722f4d1c41f7213854e206639a11a6c3f73eff2cb57baf5482648aa48d33ba \
+    --hash=sha512:438f6377a00556094cf2185953dca6296ab4c99dc06e15477408a91833b691868ff5c3ccca65cbd2c5b13eccf3ee8f0e834c5c530b25da62e549e503d14a74c3 \
+    --hash=sha512:4256dda88eb9de3606964828a213fbd587d75ee81a8867471cb6884212901df9d2e0caf26e98eeb1fe5f3204e324ad6600724042ac5cf1d16dc972343ac26432 \
+    --hash=sha512:aff7e3c900f6f4a0a04dfaab4d3f2577ac2f3927fb39014f0d2d651d4c524cb7eb2950257e24bfd3d66fad6aecb0965229c20959cff5c0cf8037a885c55b6481 \
+    --hash=sha512:5daca902c8148154589e9611d81709883c4d9880d9812b868eb81619ae324420fa4e6caebb6484418d898c0bc2013c00dcb69cf677337733a157f5d8570fc972 \
+    --hash=sha512:de8e714f5aedca9d5ccc734961200bd78b1c567c58a2bd54ed777903d68df3295280f2606d374322ef9923644a0389947ea0b5756e02d6f84c0f2d3d9265f633 \
+    --hash=sha512:ec9c454d782e4f4f5d191521eeeeaa9e39a7fc193d6cff876214233b2dd8df1e43ac69ae1654ccb8fc968e9f6b0880cdcc8c464754ca86d52d599fa25e313be0 \
+    --hash=sha512:cf83e1357eefb8bdf1542850d66d8007d620e4050b5715dc83f4a921d36ce9ce47d0d13c5d85f2b0ff8318d2877eec2f63b931bd47417a81a538327af927da3e \
+    --hash=sha512:12ce972a5dfd3b02012ae766e580e6cbd48756429e600f868036fe009063b528245b75c9b7040a29816a5c8425aa6f5b037f45bcb653ecc8856cba03257ca015 \
+    --hash=sha512:cf83e1357eefb8bdf1542850d66d8007d620e4050b5715dc83f4a921d36ce9ce47d0d13c5d85f2b0ff8318d2877eec2f63b931bd47417a81a538327af927da3e \
+    --hash=sha512:54590f2a4fdd32d63d3e6acb33eeb827dcb7ebc0ec63eeaf7fe1c4914a8e14db919d251518677f991b443b73a2f1341b39dcd9abb614d3599dae2bbb0708c8d6 \
+    --hash=sha512:87afdb9531cbdfe6547ea5564d4fd97a75aa7c9749bb8f53a8e67d3976d43d02b9b5dd6a06886bb81ca5c23a60f2517e3049397c091727db505698bdc5898c70 \
+    --hash=sha512:cf83e1357eefb8bdf1542850d66d8007d620e4050b5715dc83f4a921d36ce9ce47d0d13c5d85f2b0ff8318d2877eec2f63b931bd47417a81a538327af927da3e \
+    --hash=sha512:151f3e0817cabb523e0d843f0fff66a7474a0a86c8a6af2cfae040633a6cecdf9e27c3587ae33b1a61be1e70f6765f26593f4f24e2328b97dd93a54f67548047 \
+    --hash=sha512:cf83e1357eefb8bdf1542850d66d8007d620e4050b5715dc83f4a921d36ce9ce47d0d13c5d85f2b0ff8318d2877eec2f63b931bd47417a81a538327af927da3e
+arrow==0.12.1 \
+    --hash=sha512:f18449d3629ff5630aa77f6068e7cd3e2ee32ba35e1d0d972b03fff1dd817d2d936a38cdde45b2b8f218df5c1ce3e316404e33103d8bc82af9bcc377e37afb09
+async_generator==1.9 \
+    --hash=sha512:4358eb299493b388a317c19a2ba53c7263720cf1a53d1de9e7a59230d6a568e7544b9c38a145303af18113f67cf9a31a5c3bc58e4a2b31b17d6117f67ba0f151 \
+    --hash=sha512:c4e3295cf51e2d06ea240f9cefd135984f9e61ab6cff28f76a3a83321f7c2d811f51f8909d17d901331b55f304683b4e072d16262f5311622402568009b2d1cb
 async_timeout==2.0.0 \
     --hash=sha512:bc5a170662083abf018ac8ecde1f8c3182c543abcd6323e565f9493cd19c703f11ab0deb9f3385f85c31977959c84d393efb3219539a90ba7ff0ba69110e8bdc \
     --hash=sha512:c0f5688c24a470de0d8d390980464eb0574cf3b86e39864533bd8de53282ebc4c4d4db135f8b9eea8b7a8be342219c09bc12e58a4108f2483e94bb68e684a91f
 attrs==17.4.0 \
     --hash=sha512:701ecd6e25b5d5aab54e38c8a6e172e0db5bd8dcd13e66d31e8479fd2abdf2c422b40b1cc413de7504db67e9bb4e7f594a9ac947c3a58520112c3ae24f7ef94c \
     --hash=sha512:b631cd5af1be7c78175230363a3cf9d37cb0237d87b24f994812b5734985d114708d5bf7ee5d92b8b13c6b8daa313efde4a9f60f0630df0b62bbcf4928a016ff
 certifi==2018.1.18 \
     --hash=sha512:bc5f15eb111ee52b177727226b5bd459df38b9227ff4e24c4611b163ccd576f19d8a8025109a2e39e236190a81bd93150ab6c54cd4a5fb719ec89f0b14b5a8bd \
     --hash=sha512:5a419fcd6ad2dc095e126bcff40127b4549cc0556e19157b142c6f27b284448eb3124fb92a72b147d6734d9f3ff212212dcbf364e127c2691ab94a9736cee032
 chardet==3.0.4 \
     --hash=sha512:bfae58c8ea19c87cc9c9bf3d0b6146bfdb3630346bd954fe8e9f7da1f09da1fc0d6943ff04802798a665ea3b610ee2d65658ce84fe5a89f9e93625ea396a17f4 \
-    --hash=sha512:61a03b23447a2bfe52ceed4dd1b9afdb5784da1933a623776883ee9f297e341f633e27f0ce0230bd5fdc5fdb5382105ab42736a74a417ddeb9f83af57455dba5
-coverage==4.4.2 \
-    --hash=sha512:bccc792c2fb749c21b6cecea93ea952ff92bec90c01ac7e25551bc8e2cbe7f27e2c2ed7690033fa53f8a09d751d781e6f72667029f550639d60536e798ae36c7 \
-    --hash=sha512:a51ee87fe27ebdebd935a4329c99887efe5c4011de52f2f8236bbe1526881f18c2ccaa78104282bad86f758b320c5660a0733d53f5f8fb6bbb28151caa03c73d \
-    --hash=sha512:85389b309e36b4f54a3415054996792130a5f0139666c27d00240236c4e409779955580e8b8555bc77bdd164841c91ef32d0a02a54d340fe2ff3d7b43f9a905a \
-    --hash=sha512:3725c3141bbc6829d4b57ebed5e84cb6cd6293c58f994f3c61c1b390ef8cf72b130d7ce66cb581fbf23c729e5615a95c246f63b585d173c616a19e3cf2399925 \
-    --hash=sha512:8ce8a81f217cdc0e3efcdbcc44d571468185ec35743e572eafcd19ff4945ae508c355e891700975274fc4c0b7f7876029b3e79339aae7a5629d3926fb249304f \
-    --hash=sha512:62a90a969ad25ea2075e746a2df49e00083aeb5714bbe9c6f25f9de7854bfb8579480a12094946c96666271d63bd2b8e656e9e34989e10d42c64b04c9d823267 \
-    --hash=sha512:15538adf6597df17cb8089bc8e1f0ccae854d25e1213e6b66a6b287c80fe24fe1551e3f5318f0662025980c9a62f56b9557801813c7edf37d1a060d38e16af6a \
-    --hash=sha512:bd402165eaacf89e136f47950877f3bdd1976a281110e6b52a145c0f44385ab6bb3acd89b14e5a89d73f44274e78b1875f962d27854e58a72b5ee828d744d9b3 \
-    --hash=sha512:117adb94168c8afc4d8b928d6a740ef9a482c4d1e9352f0f43eb0e7339bf7ea9ea3beea507beea2dbb6fd9477fb9e557b591f503cd0bbc023c4ba43c718d298a \
-    --hash=sha512:25943d5dd211ed2bfd18a994eae26326f7ae65f5c88c1a92409de2e17c82f96df0934e05eb8379fbfc3795e9761a95d5de6bf6120f09999276e94a4bf1802433 \
-    --hash=sha512:e15e13fb177e560a21ad6f9595c00d54b6457102c74219148621818712277ce6364ad6d5c565566240a4d9919fd7ec6eb16a573f0a6f544cb46f3a7f3872d9d1 \
-    --hash=sha512:e30208009886eeb9f84d28eb68324c7934e9dcde9b8995e8548ea2b7b294be26239fcc0184bb00cd2da28c95b1940bdfd7b7571053bc33f83247da4b886974c5 \
-    --hash=sha512:264635d2099369fb0e047af6b6b452d7a05a0a3c24374e3d43bad79942afbdd9665c2d9338070a3a45ce97904e3da0b25495c3c917aca6ef5db1ed7b56147845 \
-    --hash=sha512:534b002ea6f19c69fa7486b1daeca00a89cb42cc723e198cb4f3e2f2305dd218d7799c2ba9b1ee3682b51e195ec786825a75db0497e3b9b71154cfabf430440e \
-    --hash=sha512:545816334c0d072bb623d5c0557cc47a2b597cc4aaeb4a1db7db4ea3355d557947ff47ec23459c597dfa12af432c0bcbc28b67b91fe583e3ec3619e722d9063b \
-    --hash=sha512:d041eb28b167afc181fea2bc14e69ed22d926dd61b0a22623c4b2b5171659bb9a54ef660a0199acfff53d9ab58bfad3ed42ce6ac875cd9431e315d9ce42aa1db \
-    --hash=sha512:852b808e86d2e7fc74e0ef40b474b65b69af867380f1ce7ec43c806a2eca7633e81dbda8e910a4db2bd67d7edbf5707a3e3b9e4cd240507a22c47ca88e6069a1 \
-    --hash=sha512:090054cf77ae5e0ebc810bf341d2973c152a0f2bf5750a8f0741ae7aa4e5cce51267efe7808bd3382ba0504bcdb38aaac24bf3383d7452069bead432cc25b07b \
-    --hash=sha512:46b5190e76752aa204ae009335242cd630d85a3ef09d51551f067e58fab82e738a3867add23ab32e851f859713097a4a8395fe94efb3456aa14b6ec2b877a919 \
-    --hash=sha512:6d6ac90767e5bf71d5cd3e806dd4024e8e5815179070999a03f8f49d1662a999793cb6dda9e91d60d15bd4fed630f0c47b6eb53b0457a29700f20d73fe11ac95 \
-    --hash=sha512:74ab4d8d2d1372ac51518ccb4f43cd0fb388468664ccb4ec65a0672c0a6a9983f7f37a3342e0f38a522e1160bc040af6ac900575eb11defe5561be8ef1ba4dd6 \
-    --hash=sha512:2954d1ec57832c78a8388bd7fe5087170e059f78fb306082ba198d59edee9a94386c7f85d1d3a5f4f880e73e84a7ef9b38c3fccff510f0c9f596672eaecc4322 \
-    --hash=sha512:0bff09501bd25ec661c7d7489063019c97b66c84a79baf8ead1d28e6799a8979c72af75c1d12f54f533621985466d2aa77271c9a07aaa61d5755104313e6512b \
-    --hash=sha512:eae28ca65c5ca93c9cf03042b71f3fbd67462a31b803425feade2978028d7be1cfead7e7dc3efcfbf28462ac5e74e7e77f71750047808d3ace39d43e30930948 \
-    --hash=sha512:2f4de760d9a87567efe3b88357591541f91993cd80bce7e9c39fad90221c7aad9cd8ff58cc7a889cc65b9359515788244309382b6cdce3e240995a8ce51d2d7c \
-    --hash=sha512:3abacabe58140d2eece5f3a0325a1e22fd846432af8063111e6df71e7d98d2cc612bcf49869f2f4a283cde415b474a9bf53f9e62c33bfb1a1f0bddaa806e9207 \
-    --hash=sha512:fa50b5759fcb162fa32b07fef2619f256a8c690b08c87240f083776237ddd6d26ee9e3d64b04d2d040293fcdf921c681049db958a207ff574eb45db0e23a6420 \
-    --hash=sha512:2bced102e42dfb1722ef62cbab5da9cf3ee7acf3789d615bc4626c404f97044304d15e1fe8c3f4b5bbe248d5b0d720b354eda2908440a194254d91300029d39b \
-    --hash=sha512:459802b78ebc4eee914053de31263b4cfbec29273fa104203289b2b0225968491572b582c21aa27af42f43d09e70165b84cadb395df9122d5eb7949878fc7a0d \
-    --hash=sha512:8e99eb0f5019b0392470d3cbd0d22d7928989975b6a4e39b9f7c894a8909284dc80fc0b48ede93f3d6f5a576ee00ecd5d266ce97e69a455893626ab127a6a45a \
-    --hash=sha512:44521359995356f165279bcba539b9aae89bfee99b309abdb7cd65df67f198ef10cf6ae810e0e7006a748ee7610fe459790ae6cfbf233038c0c1a5958299eaff \
-    --hash=sha512:f4c2414c18b983443d9117a23087dc84182d7373a91853cd820a1eb6ae73fd20f0c8647c6f9476f31f26dcf995596375c9ff5bbbb09984ebab9909811323f3a0 \
-    --hash=sha512:01d9afe2aedacbc1a0f9a702676251fcad4f5298a60a92c72b70e74e903a04ca1733d9f9da0cbbfbbd4201ca7f1b91d27824b2cc80d4393de3ec44ad63ac316b \
-    --hash=sha512:67e72021539dbad9cf1400d4b620cb8ce71c143a622e08f1027ba34d2b4032e4e26fd222c8dde217bfc3ce0cbac9d2efd72f00fa20d0d18c6e7a7b38953fde69 \
-    --hash=sha512:f4ad60b860e587b93b4b85470851b6bc34e29157132c2ed3b06e198a00414ad9dd8239ee04769558bbad7eabbd8cad5ca52e0b3bfaae8f9218239ff029b2f96f \
-    --hash=sha512:b1d4ba1a34197d06d6294ecdbfac47fc083a20cf259e0d612bb4bb956b833c0dbc1de6ed4376b6f52eb9c9c9e4fbf74c6a4993ab933b52eeb988b2e7bb621539 \
-    --hash=sha512:ff6de9c49bb0023db2d3ca0663347548184b8b4135cbf2238f9514e0aaa20c5c1ada89a5b05413853614bf646367cbdff9f4a63d41b2bcb2c2e160b3a0a26edf \
-    --hash=sha512:a3513a577717a165480d6464ac7c93cb5e09ff771670033e013a110e6c202fd868d3ec7e0e163b21c7330aafa6d922fa4e35cb5528a7e4d195d8f4dfe68b9ebe \
-    --hash=sha512:cb2c2b31908ad336249ae1dfe36f25f8ae3a9b676fe234bd84ab7e5f63a773bfa295109e3f538c23fea3838f04f23ab93888404d032e38a7935a0f02b816a78e \
-    --hash=sha512:e1de2899c03673589aafb179cf91960eee05bb00afa3093bea2731b7d5adf12ffc754e51f9dca464938c6bde08f98d84af293bce517e91b7dced644be3b004dd
+    --hash=sha512:cf83e1357eefb8bdf1542850d66d8007d620e4050b5715dc83f4a921d36ce9ce47d0d13c5d85f2b0ff8318d2877eec2f63b931bd47417a81a538327af927da3e
+coverage==4.5.1 \
+    --hash=sha512:d4b9569efa13c9a316a0bc99e7c163a474ed7022df0445ed5811e0ad4e53f0316472e3c8b8540f995d0d6abaae5025796d876f5322e63819fb469a7f1a5419a9 \
+    --hash=sha512:d6788611162a863a8a274473b6dcdaefadccd0f42f6732431cdb12ebd5300987eb3db29df0f305528bbe9766b87baba9a6dca0460089cab5aa11b1ca727d3af8 \
+    --hash=sha512:fee28f472b893d8531b7b6b65681cc59e39627de4c9c6d91c043943793eb586f1427a8b18f8b50cc507fab30c5652ddad5d01d9c368e5488254e36bae1627ac4 \
+    --hash=sha512:a7892f7106be5ab0670d32b4e8d10ec9e1336e4706d94666c084be17f4519672aa84c2dbfa4028b43433ea51ed29ffe175ab3908b91f5329578c7a6bbde7df91 \
+    --hash=sha512:8510d0846aa24b5fbbdd74c0e38ab29c8fce7cc96ff473f4b52fa8044fcafcfb54449e8aaab29efe7c73a3530167231412b14ccf10e6cb34c9838adf63826019 \
+    --hash=sha512:2b5ad59f6570e22021ab96a9cba9bfad78469a248dec032a227a2fccd1b110ab7f38a5076a44a1a471b37077e7100b0f9c51fe370b8467f9dbedae498a042581 \
+    --hash=sha512:2520e0ba3adf1485e7d583ff1f14643bdbe531b4062353780b80737d08330adddb7ab6ad869a2542a261760b4be1d050182fe0f91061610463ee972298fe518e \
+    --hash=sha512:45126acc107f5a7fcb015c9b866a3b0d0101e9211fdecc5843f334fea28a2d80db1048e752d1d6f860687c9f289e03678cf2d92a77779a355b9b186a772d3353 \
+    --hash=sha512:dba0935c4079bfce694866d6598408db305b82063ed4b0dcaf5d4260a70b25118aa3d72ff81ba3326dcb6377734c4fa5811740543331ce6eb1c9886e621217ac \
+    --hash=sha512:55decd6e6d369682b67c9a82ccf5772538e004279a657d6d9f75482ff20896360b37b4841d08d79996ce16956bb863d2a2bb33e2ee7d5b06fd3e79adf96548df \
+    --hash=sha512:c718f78a365a5b610cb2f1fe8ca646b83d6439912cfb9f787e57cc84dc84eea6f3150660231acd093dfa84d2f4f8135f7f2512fb05a1978e1b12c3fd8b23f505 \
+    --hash=sha512:45abe32fa09505e436c8cae010e3866399dee551c13fb5a35da57cd296502b9f266332d278671ebdb7ccab941326daeb1e27118821862e249ee985ef4a6d0d35 \
+    --hash=sha512:d987c1fee355cfc7d6bdc89234295b7dd35941449f14dc5c8efac28bb98894f9a78d558dd02a05457a97916de070ae386127be7197efc3b511c4f7a7f056f189 \
+    --hash=sha512:f96a049d5dda5b2ca4e135a561d8ad9a1a511603e553996e07ee6e46a3573afea1ffe895d2897e3c2347ecf186588b62b6d3d821d1f87109319081777d1c0fd8 \
+    --hash=sha512:4ae653511277a5bb984142286e01157e1a068c01a16c825adf06287e569cc516ca056e6fefcb05b2038f31ca261b5fa8ef345a6c0274650b3de175a694188b95 \
+    --hash=sha512:7927c89140e844f56917746f41a866755ffcb72d8028bd23ab055446f90231d0c1f4ccc29d67fada8155a5c927b4559f3e263e49659755dc847ebd4b7aa6e392 \
+    --hash=sha512:338a31e1a1856073501a02eaefaae2c18df27140598472d34a8432c9c25225296eab81567729a2cc165a4c9d8faeabb1e3bbb52ce840d394ba0f0c5f6baf2528 \
+    --hash=sha512:5ad7ec5b9be01298957c22704a2689e2e9c9c3dc12e11570fbc4a5f382432a854bcea75e4419e953175da3aa2ee1d2ec2f244886db5188f7cc8d9e231b29cc2e \
+    --hash=sha512:4757a11361a9d4f757082f885512e6b4de24b60344646ad09741c84e4fb4f08813f05aa18a7acb3451a331a91fb9d27ef411bf9348b54d3d7cd3074e4645f41b \
+    --hash=sha512:798fd2eb99a17cdcfd7b2f2d95fc319fb860e041b982b4e7c9d1ccbff41c35f19d5ca16e3605e2222cd30a4ed3cddfe94149b1b2ec27a54efd1ea6474b9ccb1b \
+    --hash=sha512:e01685335bd44d0c767429568adc5fb3669417354b62d634bb06fcdfaa959102ff1105f3b108046047a4dffd24bbce5bf81fcdd61b49a45f2aad32a83034dc9c \
+    --hash=sha512:980260b63b49b697a543184e0233996ba6fa4df8c6976227ae6c20dd650f1a094f4115a3e999222e73806f191bf7ce2a2848bd60a690dd1737b102928f25f3bc \
+    --hash=sha512:b202a7278ebb3c87d6fcd2f1cff7dc88d78fa7eae709a73e6207c6212f962e706f84f22c14dad6c5c3e8be7eef7c1806c3f66e8f1e557c6127aea0a97a797b0f \
+    --hash=sha512:b0b004871cfd6f1b949a4ddc37544a73c1446602109b671c6752baa3776e4f08dfe340c1c75299c62612c43fba652ee92e3481bb39ecb7e9b02643a041becac4 \
+    --hash=sha512:9dd03ce95b1a107337b226d46dcd9e6fdf3b388426ac0508cb1b6c5c43423f22b8b35828e9d89dcc08483525b3bc2de1334fe7e85bfaae9d64f64933ef9fe3ce \
+    --hash=sha512:d0662ad14ebb76454571ed5b083e62bd35e57cd801f627dd1d286ccfce7c271109a814f73e26fb402d60c23ae08ac96f29ca62a43cbbcb027e72b349ec9f296f \
+    --hash=sha512:9c0b13abc5376eaff78c4e7f2a945bb86965969ea1ab3571d2209f91df078c1a779ee42f47bf96e62fe9bd63668e49edfaa0b00525c18d2cbbd155781fa2201b \
+    --hash=sha512:82742a572549400778cad99057b1ced4c36b61e917983148eccc86bfa6340de8cfefc4f743e79ff876b641e0b9d21307dd6bde78638a6b20dd8ad215068dda25 \
+    --hash=sha512:d329341278272c48270cb8eb712257ce9970c665606351064d02ce37424c42407e833e4688e938c3e88804451e15cb5287dedc91e0fe5a66cb5cc201f791ab1c \
+    --hash=sha512:3d84ef3f2078ced6010f7192fb5fbe1c0f12c11118cb756ff8b46c453327ec61639f47799b8338a0565033641abbcc6e3c5f394020cab2ffdddec04bb489bf1f \
+    --hash=sha512:9b24bda59e374374dbd48973d118e039fdeeff3d193411533aed90e3d425ddd5ad5419903e2cc7a719a4ff04bbd066eb3e11e153ee8df339dae03dcc8c25b9c0 \
+    --hash=sha512:ac9dc454f928a9e7fbd8e4a98bfce0511415cac69e80cf0a098afa504d9c6585c2eeac0553f20d3edd297770f5744e8f03ddb0a17f62bde70caf3779d11e32b9 \
+    --hash=sha512:1bed7f91763ae47fc7a0548766029328f059c25fbdd292f2b313d867b93f161cb35b9e612894682b1f486d52c91e06ff7173a2274d6d098657e69de35768f854 \
+    --hash=sha512:89e12e4b7ee82e2f2f92c75697ac30bdbc214d9b8fb0bd5aa21e657eac1800f8fb1b44ae9c1d8ae07666d0b0d9a5a1f681b555fcc2d141f1ad15ab589e005243 \
+    --hash=sha512:b388092fe437bfc8bc10205ffaa5a43e418e39e1f0e3509ef03721149c5904455142eadfc28d414007f93e5d0deb39231b59b35cba82ea884809c60020b1cfa3 \
+    --hash=sha512:0d656cb22528744a8ef0853f2fa7b96f20fdd49f3c439c3211076e6aac1509c216138e31e24ba92e3945ad4dc81d58ef4b147c092e888a1acbc840d8187617e8
 defusedxml==0.5.0 \
     --hash=sha512:b72237ba3c62f6178b80fc3718f90966f3cd70c4ada6ab27f271c5ec4a5e77f9d560232223cca8f3dab0b41e1e40895f488f1cd27e0989fc49733805200450ea \
     --hash=sha512:71e1a604df9be41ded454bcdfa63610e897eb405295d7365fcddfc5f50f7572c36f0bd91a4a1fdf47d1b097637bd9fdcf08f1cdb73e2fe64eea0320a7532e452
 dictdiffer==0.7.0 \
     --hash=sha512:dc593b33101802b014b6f6aa58b165827da9ee1eef92787a9da5fcbf1bfadf390cb50bb9095f320b5adc57a015621e0b8dd2269b58c89803e7f4018585a890e9 \
     --hash=sha512:a57f5b3fb25fca4e33e4816a66babaa6a0345b48c4743ab51df672d37bcb5e0073b1bd5a87dfe1e416869045715a86f33de23c7173151f79317c76b412455c5f
 flake8==3.5.0 \
@@ -105,56 +107,59 @@
     --hash=sha512:767a599aacbe87328b3e36bd85e0841870760ed9bd95dd3a4a9084edc6f0ae89f8203d565c2b075f16f1db21b647c17b2aa59b08e4702109d7e5f79f36d9f3fa \
     --hash=sha512:5d5d9c487e3fcfa3a51d226ca81b8c559e2dffaa657f902d4afc47551677c0e889bf168297a56e816eead2aa45e8a9f4ca1674e8f7c9dc653bb2a01a95132e28
 frozendict==1.2 \
     --hash=sha512:095cf5f6f8b02bf5666e04200431992bf4b3160aae3464d528bc256b1ab643e29dda78fe94d9e8c983dbfe66cd2459e0559122e17b6b8660c0552adc5318b3da
 idna==2.6 \
     --hash=sha512:d6f64f657f1c97edfc6f92582e9fcb6c7fbee0e830b5e830d9b03483adf82400819158eff44aa0a4d05f42ecee0cc728f58589f0ce5f70e87f50dd4fa1cb8c63 \
     --hash=sha512:cb5dbfab44c4d11521c67f9d29391f184d1267a3da6dc89f4ed12c60a7a909d5c7474c3ea2bddd0af7063f4f620e87a8dd586bb07e8b961b30b1dd7c969704c2
+idna_ssl==1.0.0 \
+    --hash=sha512:d1f7479cc3edff164bb26deb05af757906ba91241bc668f1b087560087a89f741a0b36e166bfb8142128ceed6008621ab36a2556ed2304ea6374c19982bc663a
 json-e==2.5.0 \
     --hash=sha512:8e557758bc5089db5b3a6c22e3de77e3c2db59f46699e118d1adfeea6d6649c21748a410445875cf99b389794fd4bcd16d87d95368bae34a29b5f9e636cb2310
 jsonschema==2.6.0 \
     --hash=sha512:d0be26145ea5ec8d701f636016e3cdd068a603170c527584bf9722bcdee4570ea657ed0744f8e435cab34aade569fffc1f55db9e68b6b7b7b0151020a2602946 \
     --hash=sha512:03f916abd023b32fbe60f91718d6f2f94d8834bd1bd8ec85ab02f591a145161275c2cde25b037c4d2e94703b870159feb776d3556f011e4c394d2e20ab897b0b
 mccabe==0.6.1 \
     --hash=sha512:9cebc6bd1c8c0201072c8c18fac5e250544ec61d6421e75e7db31a526e3f5daa5e9afae8e1ac85ed7df23d3e3216950ee311051230c685044432dabd81a3e14a \
     --hash=sha512:d8fc251a29790887c14c5932c5172b4cd578cd37ccf14cb96e80f0b97f27023427ea032d14e1e2a99d72627b055eb285f60db69e679ecd79d90a34b0255703d8
 mock==2.0.0 \
     --hash=sha512:e13e7cfa175966d62765d42a79f1678219294bc24ce172741af1623e17a2dc840f9b013e2659e8a7f451758057e66b547bfebb7f9591eb50184c4a42824a6e7c \
     --hash=sha512:a08007651b749d2843b94f5045d74c122958888290aea21930455538a854e6b04c07115e21d82edde996154bf597d7a8784a2f4213cbabc49a98dec22dd92238
 mohawk==0.3.4 \
     --hash=sha512:7cdbc98b5bbdc269ebbc614b818dcd35e118b7722293bdba89e5c1bb5dbd92bd6c113895ec893a7ceeb696c67ef894b61f1131729724fce7574e36707fa16714 \
     --hash=sha512:f5a5d99d80e7806f92d5078d4d6a7f0b1fd1d4759a9897cfd178fe1ed07b27831c707dbd9b8b6a735d392845e532f2805e27cfd78e69ea72f22efaac1dafc9a5
-multidict==4.0.0 \
-    --hash=sha512:b0886af392db8c94a7e70ff65eb3bde61b78ee02119fdd1fee595613d0c49cd067b7c7b154f9bc6e489dd8b7727d2b91d930b7df9695ad788572ed7152d269e9 \
-    --hash=sha512:96ed55d0f9c785a70c5097a4367c21b1fb5cfd03335958c59653d61c77798141422fcbc2e374ad950d8c3e44634c50c1e8117703fc4ecbd3ef7251522413f028 \
-    --hash=sha512:44111b919c1fa517e80e85f2d1c99940daf6fe54e9015a5749d6c18afe82881c8b5e79d8abc66720ac12367625351735c86786528b6b4fdcf454c4b39af40776 \
-    --hash=sha512:90aa9a096b6cf8ad7e49ba8256fb54fb3c9318d1a2cf6388ddb1de0f9d373feeaed28dfaecbc93db813eadc306cfd8877bf5232ff287e518e311c37babbbed8c \
-    --hash=sha512:a872fe9e69328202bc8ad8ba0c156283dee973b34dcfe2addae47e674a1cf39e3fa657dd758fe2e640a2f0d6cc422e7e999ed6120b92470ec737cf2d08d7d516 \
-    --hash=sha512:fefbb27563cd8cb8d20d1006cbfa8788f9102b9d6584d158dcfe433f324a64357b8d8e6668ab60acf68ecd9a397b2844a7564c183a7b8bb570fb308c43407898 \
-    --hash=sha512:6704547bcb712949a94c012e9a8a97e5688d0cbda8d011da3649ad54bda8a6716ca7732821251212036dfcc59424bd4796529d50732bfa48766bac3ff80c7c83 \
-    --hash=sha512:9e81a3c98d895ab02b7b8df72e63ec2c69553837f16fe910e3b023e5138bdda1afef93cf5b22679adf2c70b3c077f21397a6506ca4240f547fdacf3aff12a36f \
-    --hash=sha512:6525cd4da5d3949ba873ceb533634a9addb99ba236bbcd71de8541241e9e0b440bf5f0a423b3736325ef1577ea2f9a204d0a152ed943f17dcaabc011e70bf474 \
-    --hash=sha512:9306ac40900c7435ab10453b5334d00768d062dbf53daf5899b410b59ddd6ff77ea89c7f89537628b23cbce5233982e509fb301fe6adf8c18d20e5414ad3644d \
-    --hash=sha512:8ceb5d0efb0fdb0f040ef21a13064f7dcdcf70fea6e0cb50c3d381ebda8f0e0c8259f3a54dd5a33631fd545f879d417dd4b5d2439b2a24280ff4367d36732b37 \
-    --hash=sha512:a5366f793666813e4d657854e05f41385d232da6146e0c113d45282c5a3983ab7d16a2dfe3af4cfab004370f5abbd47c639e027ef1e91d74c9384650759e767d \
-    --hash=sha512:7b618ce9de23e3ae68a9f141f6ee7462eab82bf6c61651224dc9ee0abe38482ec01132b30a76d681d8cb85564754e5b2bf1973ad4b5ed7dc742d40e20cde59a4 \
-    --hash=sha512:a9ceef2e07ef98c1e37f68551e1605ad622b739dc1054127bd4ac450cf837563aaebdd4652b97f68f8d8debf6b9ae3098e74dfb60d14f23246b1b1983c5ebed1 \
-    --hash=sha512:5ede1479992906bbae17f423f23a169e0e8c31b3bb894f50320d9c7cb4507284c9a60e41023873f1f9f09d555cd3f932792e0c883d4cee8abef22c5acd976884 \
-    --hash=sha512:ea3c1067d9abb79601e216e8a8455ed40f7c3128109e511aa66b6aff0887fd7ee160f8b0706d3042b2d47ad29c84be0cfef76512c10dbda96fad27162b3cece3 \
-    --hash=sha512:9b0dd0447ee375fe60fd84846d62f5e2ccae1d435d921e1e0ae831f7e20d02f14ebb80781437eb0f01e1aff9d42c3eb84dad41e1d6bcf78035c294d31593cdb2 \
-    --hash=sha512:4306b885f0538b44b2ecbf3b1cbb7556dafd89e7c974e5f7720c1ab6b9e3b636d5792495c9697cb2df2bd8fb2ff7c4777f5f8a913b6952ec00ce1dbdc4fbcb03 \
-    --hash=sha512:a9a00dceff365766faf9799820716aca35d0a4fc619dde1554db25a96cff4c36ca4dd9c16d4c0ec75ee55e91a017dff32120d48c617a31103ce1f06b92384968 \
-    --hash=sha512:1eacd18580403a647234397e5089a05f77ca7e0bb2c32c4c1c56c788122daf6b0f70fb3efe0bd9135addcf879367308984ddcd5368210a86ed796f06efd85d29 \
-    --hash=sha512:0f7d8e75e62090aee2decbab07478c250a1a5d61e46115a44c2fac4b0bffc4779b80c942bb18eabff5a3e53f20ad6ddf4935865d0055a80f5367be7f2e06f3c8
+multidict==4.1.0 \
+    --hash=sha512:c8facfe9d66f724f3696ed2b4e388c361e604350148fd46d355fdf15e3af4e39b3999308234fbffbc91bce8c92c221406ff544ca59d7ed7625ab9560e83d4171 \
+    --hash=sha512:de32a0442d00e3c7afe432c311b72fd087bd2ba430d608b0e6d89cf2cef570b242e6096cf4d4cbef3682618b0afb06e023051a65203cd60d311832f82aa93087 \
+    --hash=sha512:e1ab81e09860dec0bb5ae6c490e4628bb4796225b50283c8dad920f92d961217637415c69ee687b5cff6f997cd3e21fe2da2ea3636d0d4edb18707672fd48dc2 \
+    --hash=sha512:3efd0769e1e177cfb24c5565b0257b7154f56d7388b6f0b755dea701c17755d7faf2f03a61e2058bcab901351277d4ed989e4a8ff86b8c8b4070159f2e021b42 \
+    --hash=sha512:5f0fd64d80e688c351f2a4c666f18cbaec994450a890f30b73c706b60a69cd5b475b28cbc9daff9b2b6cb4b08d641226b7e6cc98bd19bba7029fc7dd8cab80aa \
+    --hash=sha512:ead267a4a7be9bfe1f383df01b186b7cdca0433c3afdd4ac7f06ffafc0ca6146ccb474130ba50132951edd0141352ade377dc8f85c476a3e79d9319772316a47 \
+    --hash=sha512:fe90c2a4a2af944e9fc29e85bcdcf1a43ad1f8482dea0eb46b76a6a91049d5cc648a118dde94f1795fa00b490c378205d6f8176092a443fe3716efb11c44766d \
+    --hash=sha512:0975ef4501a97ed5c3d81572015c10a57354647251ceb7500527d4ff44d16c2ec0046b045de1a0de0f52cc9692713e87770f9a9cb5828413c3731a4230963842 \
+    --hash=sha512:811dd4d170a0c66fb8ca59fd005f748c87753ae9acbb4bc4e2a912427237345bce27cf12b4958e2538db92971309afb2f8f92148cfa7e50f5da367afe54ac231 \
+    --hash=sha512:a4321ed67e9715e1fcb15520c8234c7b6bc4dc54569cf237255bf7488a3e31b4f6e39d64741a8703aa71265f4bec865cb46900c80548c19fb58fe873d332d2a9 \
+    --hash=sha512:557c7b5f28fbfbe7f93dae9e14dfa8dc249e4d36106768eaebac8aa9afc5ddda702d4b14b916111a3b9b56fb3c13f65d45a44e60670f2402b3a3302f75147cf2 \
+    --hash=sha512:6e87baeb187fc95c68b7e8211adb8c8a22594572c0dcea99b57dc7c854d6016e5b0695e8c1ba4f026ef4da6103dc67afd1c925d9ebeae931ab24e58495e9cba1 \
+    --hash=sha512:d68f839c6a478b5901e5f29c18f8b386f1082ed2291da89dba69f98faa1b95fe07529cfd885d6753532711fbf231d3163f072cb98b47085a6a8b525b310c5a7f \
+    --hash=sha512:56c2cf11a64674bc56b7f3c7fa72c2148928b75c28f81cb54c3d400ce171e71248c31cb2c7d8bb7af4661b9ec7a5e18fbba8a58e4673519bcdd3bde13f3ca59a \
+    --hash=sha512:925adffc96d8280b6aaf7c9d37fb910cde0ec1c1a89738170e924250387a2a5a5f57fafd923c220d146c6093f0ab11b0d0775d302a2657424c836807074ccd99 \
+    --hash=sha512:6a04bb8ae10b4c86cc27439d32b2ca120ca0afd1d2620632a31369cad9b790ac1214b912bdbeeaf185d79bc9b38018450f848575016d64941b85d60a3cf31c0f \
+    --hash=sha512:ead23a4ec6ff0a7751d0e8aa9875edb6e5585bf4f403f6c2219046e694778e4d388c2c502109e52950d783255ff2fbf15ddde8d616a9620ab05b61673dcefaae \
+    --hash=sha512:38c14d7d02fd857c25831e5989e72fe31b7df99faa058216c1748c4dcc79a2be6f24b1244615691b195fa1d516adba8785fe471483a58db6f6c4e2e72d20eddc \
+    --hash=sha512:f67defed931c0d1d0b3480c3b11a49e9ec7a8db4770ec5b31f1b44541ecadb4737c7d62958b82dd8a2fa34e45c0d9fbc739db04a51de8a7e52f4dd7910700173 \
+    --hash=sha512:5b65d3aa926ef03a84949901fab2b2385b790f8f0ce7855b32bc6e9600486cb33cddf8f127baf29b4abfac3eb1f806fe8224ab09a4a40c6f5374bf5d62d20fa2 \
+    --hash=sha512:e2afae7192ce99656f7550a38a036130e19ad5de107a8495cb91458843cf9ae6d013f5bc7d3435074105716ad22bc96fe256ae470e34b8fc5992274bcc10f376 \
+    --hash=sha512:4485298f4faedd48750d5a3a8c9b0c52fdee90e51ca84f1755b229ae8b6f40590d938f95193958d5c77a7c0e399e896f8db6fab57ed6697ea4e5e791535e4b70
 pbr==3.1.1 \
     --hash=sha512:52aa2bbfbd9c2c13e492318a8412cc69c5758a80b39906aab374c6ca25f4c2f0e28835fdb371210c887654690e3fe9845346dc0e82e889d545ea2c6828d0cd85 \
     --hash=sha512:c01fb83678f8fc3acddc153dd341a17ed9d602b6770f0ff244b1c5b54c37d4ddcbd0c3d726f7d7020865819e02797c1c79a0c15e9ee2ae5c1510fce7112b2a3a
-pexpect==4.3.1 \
-    --hash=sha512:ef8e0153c2c079919bc3a5182f3d3bf865670f8748322f4f6e39f05c06f396640bd73471aa7eca9e3aa78c7fdd7323369820a38b818cc60fcd5ea166bb2b7014 \
-    --hash=sha512:eb1416aa1f803d52a3c3663ea1b982f34489d1924df44bf2d36ba63699fa8c98c04437f4bf49a312dfcd01c35b062acb93095fcde7055595fd4c11b933039cff
+pexpect==4.4.0 \
+    --hash=sha512:eb546b2c02aeb727ccf633a3776a69046854f12a44df954814085a3bde3af4d87e95b8ae4f5fc21dd55d8413049c9f4972ef18fd90b535971eff193194e5716f \
+    --hash=sha512:c3ac018b0f55075ab2bb7f07d672b5c1ee2823f43577c93dedd8f828f6f31e5270afe56b2cee95cf5626f137978a5f0a7145ab4eb74bbad4818a42e6b329db6e
 pluggy==0.6.0 \
     --hash=sha512:dd58dabe2e65eee64d62c8748c2bbd99457288e99b819eb12312f2acdb0740ac46fd08f83522bc992297b9f14eec14c216c2c9688580f68393bf6fc609e65812
 ptyprocess==0.5.2 \
     --hash=sha512:fead464aa93e099300f49e6e4742fb4234c15a1ac7d842e93acedfc011a2d3eaf913bdb2a89dd559bed09eed0fc35aad911f350123d7663aaa740822cdfa67e2 \
     --hash=sha512:cb4e70855d388a6ff691e2a244c072a5a50cf39cdf727e3a4218817bf5ac722c4b49f0dbfd80204259998eba137492690759b8908bfea925842b9f7fc83ee553
 py==1.5.2 \
     --hash=sha512:e785ad3fc6888e71a46cc59397b0cef83fc77555c132e115c3532554e0903d91e44d13ef17364e0d91e1b019e4f9b390d4b3f4092eefaa466dc157b374ae7753 \
@@ -165,26 +170,26 @@
 pydocstyle==2.1.1 \
     --hash=sha512:7bf9e7f35af02cf2da7090316e4c42bd21015604ef6388e88feae7322843b407097bbbb7d12eadbdf179f94db2f7502a8eafc17464e27e5262ccb310be5ef2cf \
     --hash=sha512:e3cc922df3fa2c581d9086dbfc7fc2618dc4b2ea5d9b41b7b15625c02a1110e6390b771f696086b32f2c0635f2c0d4ced779211dcaf960d9660e0f52d9269c1d \
     --hash=sha512:815c604c81e6cf7824dd29af24797534e078860d4bbbaa35962beebc7284fe27e2c4238fa806a57225680f0d96c2bef544e0243a98efdc61ac59253aba7d5e5c
 pyflakes==1.6.0 \
     --hash=sha512:340f63ed287bfc0bcbe924a5692b7dad1694c874ffe9ce279f744db0726efe42c57573b4416cd5d4cd1fb1a5b3262fb76ba7b8cfab1f00b65771cdb67b7c0062 \
     --hash=sha512:7e9c2aad6ebed638a1354cef51c7e1f68b25e59f8caf4694997a9afecd7cd8baa629a9363297ac0d961430f007fd22dcae7dae1bcbd7838a3b5d4285063bc7c5
-pytest==3.3.2 \
-    --hash=sha512:9de2c5911f57fb170e63006b0563000017c226bbf3da658b53ee37667a8c91cd0a916f644cbb13dc154fd152cbc9a46ec19a6ea1d655a74cf6133bc11bb6a293 \
-    --hash=sha512:a2fadf30634f9c2bf88a7d6d4f306efff91e58d6bee04a7021e955ceaad6da61ddeab2fa40265579bfbe8dacc279eda8d3b9bc56c80c171b6feffcda6a977eca
+pytest==3.4.1 \
+    --hash=sha512:d13acd0c2a079722e20509b402b73ce9d4f6147b894a7677ebeb384038bf3c090f23427fe2d462ff13739cd9d208887eb836618dd983e314628f777ee17efe15 \
+    --hash=sha512:75f728840cde6512619a03ce75fd0b04cb9d57a99f381366a0f9c10ffa3210448e7e85505357bfa9bfb0cca11cdedda2c0e091e5473ed82707a2597f234e659a
 pytest-asyncio==0.8.0 \
     --hash=sha512:ffae02204356ad8c936dca7d3982eda220d886d3f75619696e3146e6aacacdfc1212eed096613f9d1b3f7aa002ce9aeb8fb1a97341877c01018b59a38f05b196 \
     --hash=sha512:791ee1b47726e85edea93d1ed86d024fd6e7126dd0a46af20b97ca2198843306f536deeea67ee16208f174424cce7518b3576ed7bb6256e6adf8226f5ea878e8
 pytest-cov==2.5.1 \
     --hash=sha512:868131d6ea6dd28deec6d653dec23ceb7d3adccfa2c6bcc0a3126bbb11e924e71f200676461b2202f274ce6e14d1799feb0917e3081817d9e8583271c18a43de \
     --hash=sha512:6f62aa052cfdc49d3013e1ff8115599ef44fbb7ebe43f01299e93636637c2498f21974e2427ce70b383f20fcbbfb0c78aea695b6df5487b1991259e7b9b690e9
-pytest-mock==1.6.3 \
-    --hash=sha512:6857f373728d3f2c6b152d4f89da3590e2e74795695dc9f4f3704a4e0250e49d705ce0de4121a801ac35c83217678a95a5023338124293ca74db406941f5072a \
-    --hash=sha512:dccd339385c38b5c407b708674908cc5110dd317a12aa801a9216652371e6249d67f5dd163ae93b4a6f45b158b1e2b899bb6cbf019038840f4c82ae32b256856
+pytest-mock==1.7.0 \
+    --hash=sha512:519505d862151158caa2514804fbaab1c61fe279bf5a1c11c0d6fe6ad6d5b1217f32ec5d1ecf35224e2cb7cc62c5fc9975f47325b274cda9748686447abebbf6 \
+    --hash=sha512:a7915f5f19a6157f05f00a2b8e922a22a0faf1353432b70054bf6da811b71ae119a8b494a2c4910e4af694c6d9278cbbb62a00451ad3bc286558340e592b572d
 python-dateutil==2.6.1 \
     --hash=sha512:f16dd29fc975629f594dd2683a525e2a86acb020bf8962558d19040b14ac6f19d4ab07a910d6bb55c9db3cc02b5472774a3a05ccc86cf624ca5e5144463646db \
     --hash=sha512:1eb4fc12d30a21631cd5c86be87f3293e5132d668f9f24d36fd0056030cb2001b0851fb4a46218fa40ad95ebf35f9d6622bcf84080593adf417b2b7554850283
 python-gnupg==0.4.1 \
     --hash=sha512:0920a1de4d98a745f7747280672975db04c40b59ea4436745cdbefa86a0c88bfdc086d6dd312c82a0a9e9f8cafb5651f8e17d86e0ee37282b5fc36e7ac8d1a1e \
     --hash=sha512:b60d13ad518061e231e141588f3a2dd91e92aa5c62152337204a2b09ed1293a935eb105034098af607bf4ce002dbcc90e0cf8bcfcd2ea23805c81ab02642f8a4
 requests==2.18.4 \
@@ -207,21 +212,21 @@
     --hash=sha512:ff19b2bb7ac963379f1cccd4973ad9eb4dabfbda976cde7caba50ad010d8fa57c1cba91d63e3e0512e44cc7d350bc9270fbd9b30db1bd55f7d9c239e7623d066
 urllib3==1.22 \
     --hash=sha512:b46a3b5622ab36348f2740d69ca1f2b82fa62623ea426ae6c09a58e136e79cf0ddcf4a7338b80a760dc9516a30f7ad5ad7612324917beb8d036df9f0b7233005 \
     --hash=sha512:132b69d7f390916bdcde66d46fbf0189d0c1f976f91778dcb0a9ef8174487b7bb4b37b9139e84f7c70234803be95284448aba0b820f3b54530c0c497ca7a1dc9
 virtualenv==15.1.0 \
     --hash=sha512:9988af801d9ad15c3f9831489ee9b49b54388e8349be201e7f7db3f2f1e59d033d3117f12e2f1909d65f052c5f1eacd87a894c6f7f703d770add3a0179e95863 \
     --hash=sha512:d7e95b8c017ec076210f30b6fd4bb44be2f7dc0257492c25bb00fee597d3ade34226d03539180f1edaf2d27b361f8efdabb92d3476e13785b890878ee1295cb2
-yarl==1.0.0 \
-    --hash=sha512:d183f42725223b5858412bee7845b084888420621c5f180ffdbeeffd7a84b1dede0c699156f8bbac7a4bbce855634779d7e636dc0bb59fbdbbd84c3cecdc4146 \
-    --hash=sha512:387eedd2be9187f07d2bf06489db0371c46b316c10bbb4fb4661a01954ad18466dee9570680ce11949eccfdb8351cc2e072b22f928eab1ed26170f5c620669ac \
-    --hash=sha512:dc6d430f98209658b134ab38061e4aa7413f7ee0ec91c2eb01bfb2066bfdaa5f81a86b1fdce185f45545a89a534a3899213d2788345cabdcba0311a42a69c19c \
-    --hash=sha512:887f0bb28bffc9b209609253b512f58ee092a490847f09aa37e71f17a172ff79e0cb39cddb3222ad2e94101a523fce977543829eefa884a56f7ab30528c582fa \
-    --hash=sha512:c92016c962ad079f70c08d9c630d4d82a0191d1cc26e6cbcc23995ad2ac33ac1e2003fc3c62e975772bad11d394917f58ad4e699f3cfeb04f1df98164efd191b \
-    --hash=sha512:bd88b56359655d098024fe42f631458ae2f5fe3e8c2aa8ab5b2a73c3e152e5f13dee32de351b5e07b7339cefe9fe0f93cfa782cad92aa5c95a07c92789337cc2 \
-    --hash=sha512:c7a45c94400d478382461ab934012c689f2335908e73a621bd591869db78379bf273355c9a565874d8369316cfdf156d97921c3ab4b2f57e60fb1762f4459c4b \
-    --hash=sha512:fbddbd5d56d0abad05457b3ecd147360f47be0ddb11c93d7eff7c48323640921de44228cb8083c530b9dafad965a24044d439e9ed8b1aeec74a07707c429d7eb \
-    --hash=sha512:79e8268c81e51bab06a6c840347a19944f5264d7a59e2484dbddd539e0520ee7d86b7dc4d852be98a8070898758d969961abaaae7260ccdb6e2a9382b559bd1f \
-    --hash=sha512:d88f4660679af4798a28574383864af8b5106eb87747ebefb11f1dd3de3ddc335c00f7689850ede975e74b25e235f7e17903d69c19b9176ac8d3a656ef1f6817 \
-    --hash=sha512:9ff3d45a713f8323f427e9a8a6785a50d82a72d19585634ad38a13a39dce4596f5c1a16404cf86ecd24bcefdbc6081f02d2e34bb2c050ae75875cfe5fc552183 \
-    --hash=sha512:08ad737e0570c8a7417e8f9ab061e8d1ce38810e39b4b335e9df7bd3d3fd9e5a9ef4867170be99212aa6ff4f48bdf38448c9b13b61e5d80f7db164f9022fd280 \
-    --hash=sha512:7da760b6c51d8f19fc2602285de24c3a9cce64d21fe957f3ae5c80ca2d89a7e9bcb6682b8a060cf11cf398e6c01d9395e9ca07a5f2bc0a6b24ce5307564dae19
+yarl==1.1.1 \
+    --hash=sha512:e7923405d70e1444a9a6b4aea8bc22e73375badcb1f4d2202ce4b00062c9da8b8b4fad520c5274b4d682422aa0f8cae4f3b64a4773cf9ed959c431f13f267b71 \
+    --hash=sha512:9e1cb76cea335038143b2cc701d1132ee100b02b5ee1dae2303038dae0da2bbb74e135052d451f14825ba3542e2bdc050ffbd292f7d12819e953cd26d6c30efd \
+    --hash=sha512:12d9608fbad83ec49c2eaa1cff376d4bcccfe5a0a87075402a17e19756a7cf22cf9fa16d9ee48bc663c70a8e8c4b904445253703105c53d4d346076b76e13d1d \
+    --hash=sha512:19baea347f0501374e077c6218fa54cc262f266d2a827411b1f718f7f5155d8440fc2e7096b47e92f1aa4abf864a5114a8e80be553517e365b5ed89a037a953c \
+    --hash=sha512:5f3879c4afc140de3c7619dcdb780a2ae26ef96e032b9f6c0aad259b35775b5a9f3ccfde851c6c45bf94114ceb7b4948bddf4c03ce1393cf867baad662a0e06e \
+    --hash=sha512:6e52236596d1c8b7e19d5781deb4d9f3ece4f2de79b641359d0e3b2042de0d3ec67a7bdf748e013b32fb60d72e7c75c39998299b8a2de0bbaa75792611fb9f79 \
+    --hash=sha512:347f9d71e805d5ae8fcff4d4d0040f6ca7297126a3a9d58abc3e54a3b8afd6522c789fb24fc26761285bb4647917378620abe72b713994db65e64d8bfcb158b4 \
+    --hash=sha512:303eb2c4e918169b21494b39a8f6efb1e08878725a5893b2234ff76f058378caea2870787f7cd059bc2cc4e4aa8261a738bf29aeef64ed355e69c5236743076e \
+    --hash=sha512:8ecf10cb982e444a7dc076053f7e6bac5e85234d16a09602da23f5e8ad94586dc89877088121661934a01152f79aaeb560bd0ac6aa38cfbba309116053e04ff0 \
+    --hash=sha512:dd047052f142c854a73384eeeeff6a28af5302532b48da74359f398ec09da298c34e064565273bdcad3ec6e4cf8d3da258624b6721a19f9f5552b07bb17f5e01 \
+    --hash=sha512:ccdc805986d37dcafcede47d1f40a8855e8e7b3afd810a5bd3c6b769db88f8360237f04ec882bcd4c7e821c9817e15662080c318c81167c127ddc772217f3c97 \
+    --hash=sha512:8646d48c3c4a0fbd785111cf7c222fb249e865493b288227dd179b74572ef3ac4f487a74c40797adfd7c64eaff0fd2572eda92b0f90e43c737f0cf19aceb15a4 \
+    --hash=sha512:fe53e24401e91994d04fd7274200f92168bb08d78c460b49e800646a3e4611f6baefca4ede5b2b6727f2e6e4cd51296ca834305c0e2fb377ac3a928463f995cd
```

### Comparing `scriptworker-8.1.1/scriptworker/exceptions.py` & `scriptworker-9.0.0/scriptworker/exceptions.py`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/test_version.py` & `scriptworker-9.0.0/scriptworker/test/test_version.py`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/test_integration.py` & `scriptworker-9.0.0/scriptworker/test/test_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         result = event_loop.run_until_complete(
             create_task(context, task_id, task_group_id)
         )
         assert result['status']['state'] == 'pending'
         with remember_cwd():
             os.chdir(os.path.dirname(context.config['work_dir']))
             status = event_loop.run_until_complete(
-                worker.run_loop(context, creds_key="integration_credentials")
+                worker.run_tasks(context, creds_key="integration_credentials")
             )
         assert status == 1
         result = event_loop.run_until_complete(
             task_status(context, task_id)
         )
         assert result['status']['state'] == 'failed'
 
@@ -182,15 +182,15 @@
             create_task(context, task_id, task_group_id)
         )
         assert result['status']['state'] == 'pending'
         with remember_cwd():
             os.chdir(os.path.dirname(context.config['work_dir']))
             with pytest.raises(RuntimeError):
                 event_loop.run_until_complete(
-                    worker.run_loop(context, creds_key="integration_credentials")
+                    worker.run_tasks(context, creds_key="integration_credentials")
                 )
                 # Because we're using asyncio to kill tasks in the loop,
                 # we're going to hit a RuntimeError
         result = event_loop.run_until_complete(task_status(context, task_id))
         # TODO We need to be able to ensure this is 'failed'.
         assert result['status']['state'] in ('failed', 'running')
 
@@ -199,15 +199,15 @@
 @pytest.mark.skipif(os.environ.get("NO_TESTS_OVER_WIRE"), reason=SKIP_REASON)
 @pytest.mark.parametrize("context_function", [get_context, get_temp_creds_context])
 def test_empty_queue(event_loop, context_function):
     with context_function(None) as context:
         with remember_cwd():
             os.chdir(os.path.dirname(context.config['work_dir']))
             status = event_loop.run_until_complete(
-                worker.run_loop(context, creds_key="integration_credentials")
+                worker.run_tasks(context, creds_key="integration_credentials")
             )
         assert status is None
 
 
 # temp_creds {{{1
 @pytest.mark.skipif(os.environ.get("NO_TESTS_OVER_WIRE"), reason=SKIP_REASON)
 @pytest.mark.parametrize("context_function", [get_context, get_temp_creds_context])
```

### Comparing `scriptworker-8.1.1/scriptworker/test/test_context.py` & `scriptworker-9.0.0/scriptworker/test/test_context.py`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/__init__.py` & `scriptworker-9.0.0/scriptworker/test/__init__.py`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/test_client.py` & `scriptworker-9.0.0/scriptworker/test/test_client.py`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/test_task.py` & `scriptworker-9.0.0/scriptworker/test/test_task.py`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/test_gpg.py` & `scriptworker-9.0.0/scriptworker/test/test_gpg.py`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/test_cot_verify.py` & `scriptworker-9.0.0/scriptworker/test/test_cot_verify.py`

 * *Files identical despite different names*

```diff
@@ -1411,17 +1411,17 @@
     docker_image_link.task['payload']['command'] = ["illegal", "command!"]
     with pytest.raises(CoTError):
         await cotverify.verify_docker_image_task(chain, docker_image_link)
 
 
 # verify_scriptworker_task {{{1
 @pytest.mark.parametrize("func", ["verify_balrog_task", "verify_beetmover_task",
-                                  "verify_pushapk_task", "verify_shipit_task",
-                                  "verify_signing_task", "verify_partials_task",
-                                  "verify_scriptworker_task"])
+                                  "verify_bouncer_task", "verify_pushapk_task",
+                                  "verify_shipit_task", "verify_signing_task",
+                                  "verify_partials_task", "verify_scriptworker_task"])
 @pytest.mark.asyncio
 async def test_verify_scriptworker_task(chain, build_link, func):
     build_link.worker_impl = 'scriptworker'
     await getattr(cotverify, func)(chain, build_link)
 
 
 @pytest.mark.parametrize("func", ["verify_balrog_task", "verify_beetmover_task",
```

### Comparing `scriptworker-8.1.1/scriptworker/test/test_log.py` & `scriptworker-9.0.0/scriptworker/test/test_log.py`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/test_artifacts.py` & `scriptworker-9.0.0/scriptworker/test/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/data/test_git_repo.tgz` & `scriptworker-9.0.0/scriptworker/test/data/test_git_repo.tgz`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/data/gpg/pubring.gpg` & `scriptworker-9.0.0/scriptworker/test/data/gpg/pubring.gpg`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/data/gpg/keys/docker.root@example.com.sec` & `scriptworker-9.0.0/scriptworker/test/data/gpg/keys/docker.root@example.com.sec`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/data/gpg/keys/scriptworker@example.com.pub` & `scriptworker-9.0.0/scriptworker/test/data/gpg/keys/scriptworker@example.com.pub`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/data/gpg/keys/unknown@example.com.sec` & `scriptworker-9.0.0/scriptworker/test/data/gpg/keys/unknown@example.com.sec`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/data/gpg/keys/docker.root@example.com.pub` & `scriptworker-9.0.0/scriptworker/test/data/gpg/keys/docker.root@example.com.pub`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/data/gpg/keys/scriptworker@example.com.sec` & `scriptworker-9.0.0/scriptworker/test/data/gpg/keys/scriptworker@example.com.sec`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/data/gpg/keys/docker@example.com.pub` & `scriptworker-9.0.0/scriptworker/test/data/gpg/keys/docker@example.com.pub`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/data/gpg/keys/docker@example.com.sec` & `scriptworker-9.0.0/scriptworker/test/data/gpg/keys/docker@example.com.sec`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/data/gpg/keys/unknown@example.com.pub` & `scriptworker-9.0.0/scriptworker/test/data/gpg/keys/unknown@example.com.pub`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/data/gpg/0.gpg` & `scriptworker-9.0.0/scriptworker/test/data/gpg/0.gpg`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/data/gpg/trustdb.gpg` & `scriptworker-9.0.0/scriptworker/test/data/gpg/trustdb.gpg`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/data/gpg/secring.gpg` & `scriptworker-9.0.0/scriptworker/test/data/gpg/secring.gpg`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/data/pubkeys/unsigned/D1B5423204A833E7A3420C803112C5A1B0BB87EA.unsigned.pub` & `scriptworker-9.0.0/scriptworker/test/data/pubkeys/unsigned/D1B5423204A833E7A3420C803112C5A1B0BB87EA.unsigned.pub`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/data/pubkeys/unsigned/EB55E1CED1FF0956E2BFE6C8D0B3B9C1094A9A3F.unsigned.pub` & `scriptworker-9.0.0/scriptworker/test/data/pubkeys/unsigned/EB55E1CED1FF0956E2BFE6C8D0B3B9C1094A9A3F.unsigned.pub`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/data/pubkeys/unsigned/3F4DF62D10F3AD93E98119180C0D5CA75269246A.unsigned.pub` & `scriptworker-9.0.0/scriptworker/test/data/pubkeys/unsigned/3F4DF62D10F3AD93E98119180C0D5CA75269246A.unsigned.pub`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/data/pubkeys/unsigned/36E592251DFD8D491E6E9BE701222703321F2BA2.unsigned.pub` & `scriptworker-9.0.0/scriptworker/test/data/pubkeys/unsigned/36E592251DFD8D491E6E9BE701222703321F2BA2.unsigned.pub`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/data/pubkeys/docker@example.com/3F4DF62D10F3AD93E98119180C0D5CA75269246A.pub` & `scriptworker-9.0.0/scriptworker/test/data/pubkeys/docker@example.com/3F4DF62D10F3AD93E98119180C0D5CA75269246A.pub`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/data/pubkeys/docker@example.com/36E592251DFD8D491E6E9BE701222703321F2BA2.pub` & `scriptworker-9.0.0/scriptworker/test/data/pubkeys/docker@example.com/36E592251DFD8D491E6E9BE701222703321F2BA2.pub`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/data/pubkeys/docker.root@example.com/EB55E1CED1FF0956E2BFE6C8D0B3B9C1094A9A3F.pub` & `scriptworker-9.0.0/scriptworker/test/data/pubkeys/docker.root@example.com/EB55E1CED1FF0956E2BFE6C8D0B3B9C1094A9A3F.pub`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/data/pubkeys/docker.root@example.com/D1B5423204A833E7A3420C803112C5A1B0BB87EA.pub` & `scriptworker-9.0.0/scriptworker/test/data/pubkeys/docker.root@example.com/D1B5423204A833E7A3420C803112C5A1B0BB87EA.pub`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/data/pubkeys/data/EB55E1CED1FF0956E2BFE6C8D0B3B9C1094A9A3F.asc` & `scriptworker-9.0.0/scriptworker/test/data/pubkeys/data/EB55E1CED1FF0956E2BFE6C8D0B3B9C1094A9A3F.asc`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/data/pubkeys/data/3F4DF62D10F3AD93E98119180C0D5CA75269246A.asc` & `scriptworker-9.0.0/scriptworker/test/data/pubkeys/data/3F4DF62D10F3AD93E98119180C0D5CA75269246A.asc`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/data/pubkeys/data/D1B5423204A833E7A3420C803112C5A1B0BB87EA.asc` & `scriptworker-9.0.0/scriptworker/test/data/pubkeys/data/D1B5423204A833E7A3420C803112C5A1B0BB87EA.asc`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/data/pubkeys/data/36E592251DFD8D491E6E9BE701222703321F2BA2.asc` & `scriptworker-9.0.0/scriptworker/test/data/pubkeys/data/36E592251DFD8D491E6E9BE701222703321F2BA2.asc`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/data/pubkeys/manifest.json` & `scriptworker-9.0.0/scriptworker/test/data/pubkeys/manifest.json`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/data/basic_schema.json` & `scriptworker-9.0.0/scriptworker/test/data/basic_schema.json`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/data/gen1000keys.py` & `scriptworker-9.0.0/scriptworker/test/data/gen1000keys.py`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/data/azure.xml` & `scriptworker-9.0.0/scriptworker/test/data/azure.xml`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/data/cotv2/decision_hg-push.json` & `scriptworker-9.0.0/scriptworker/test/data/cotv2/decision_hg-push.json`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/data/cotv2/actions.json` & `scriptworker-9.0.0/scriptworker/test/data/cotv2/actions.json`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/data/cotv2/action_relpro.json` & `scriptworker-9.0.0/scriptworker/test/data/cotv2/action_relpro.json`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/data/cotv2/cron.json` & `scriptworker-9.0.0/scriptworker/test/data/cotv2/cron.json`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/data/cotv2/.taskcluster.yml` & `scriptworker-9.0.0/scriptworker/test/data/cotv2/.taskcluster.yml`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/data/cotv2/parameters.yml` & `scriptworker-9.0.0/scriptworker/test/data/cotv2/parameters.yml`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/data/cotv2/projects.yml` & `scriptworker-9.0.0/scriptworker/test/data/cotv2/projects.yml`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/data/cotv2/task-graph.json` & `scriptworker-9.0.0/scriptworker/test/data/cotv2/task-graph.json`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/data/check_pubkeys.py` & `scriptworker-9.0.0/scriptworker/test/data/check_pubkeys.py`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/data/long_running.py` & `scriptworker-9.0.0/scriptworker/test/data/long_running.py`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/test_worker.py` & `scriptworker-9.0.0/scriptworker/test/test_worker.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 import json
 import mock
 import os
 import pytest
 import tempfile
 import shutil
 import sys
+import signal
+
 from scriptworker.constants import STATUSES
 from scriptworker.exceptions import ScriptWorkerException
 import scriptworker.worker as worker
 from . import event_loop, noop_async, noop_sync, rw_context, successful_queue, tmpdir
 
 assert rw_context, tmpdir  # silence flake8
 assert successful_queue, event_loop  # silence flake8
@@ -50,14 +52,39 @@
         mocker.patch.object(sys, 'argv', new=['x', tmp])
         with pytest.raises(ScriptWorkerException):
             worker.main()
     finally:
         os.remove(tmp)
 
 
+def test_main_sigterm(mocker, context, event_loop):
+    """Test that sending SIGTERM causes the main loop to stop after the next
+    call to async_main."""
+    config = dict(context.config)
+    config['poll_interval'] = 1
+    creds = {'fake_creds': True}
+    config['credentials'] = deepcopy(creds)
+
+    async def async_main(arg):
+        # Send SIGTERM to ourselves so that we stop
+        os.kill(os.getpid(), signal.SIGTERM)
+        return True
+
+    try:
+        _, tmp = tempfile.mkstemp()
+        with open(tmp, "w") as fh:
+            json.dump(config, fh)
+        del(config['credentials'])
+        mocker.patch.object(worker, 'async_main', new=async_main)
+        mocker.patch.object(sys, 'argv', new=['x', tmp])
+        worker.main()
+    finally:
+        os.remove(tmp)
+
+
 # async_main {{{1
 def test_async_main(context, event_loop, mocker, tmpdir):
     path = "{}.tmp".format(context.config['base_gpg_home_dir'])
 
     async def tweak_lockfile(_):
         path = "{}.tmp".format(context.config['base_gpg_home_dir'])
         try:
@@ -72,15 +99,15 @@
             with open(lockfile, "w") as fh:
                 print("locked:", file=fh)
 
     def exit(*args, **kwargs):
         sys.exit()
 
     try:
-        mocker.patch.object(worker, 'run_loop', new=tweak_lockfile)
+        mocker.patch.object(worker, 'run_tasks', new=tweak_lockfile)
         mocker.patch.object(asyncio, 'sleep', new=noop_async)
         mocker.patch.object(worker, 'rm', new=noop_sync)
         mocker.patch.object(os, 'rename', new=noop_sync)
         mocker.patch.object(worker, 'rm_lockfile', new=exit)
         event_loop.run_until_complete(worker.async_main(context))
         event_loop.run_until_complete(worker.async_main(context))
         with pytest.raises(SystemExit):
@@ -88,17 +115,17 @@
                 worker.async_main(context)
             )
     finally:
         if os.path.exists(path):
             shutil.rmtree(path)
 
 
-# run_loop {{{1
+# run_tasks {{{1
 @pytest.mark.parametrize("verify_cot", (True, False))
-def test_mocker_run_loop(context, successful_queue, event_loop, verify_cot, mocker):
+def test_mocker_run_tasks(context, successful_queue, event_loop, verify_cot, mocker):
     task = {"foo": "bar", "credentials": {"a": "b"}, "task": {'task_defn': True}}
 
     successful_queue.task = task
     async def claim_work(*args, **kwargs):
         return {'tasks': [deepcopy(task)]}
 
     async def run_task(*args, **kwargs):
@@ -114,42 +141,42 @@
     mocker.patch.object(worker, "prepare_to_run_task", new=noop_sync)
     mocker.patch.object(worker, "run_task", new=run_task)
     mocker.patch.object(worker, "ChainOfTrust", new=fake_cot)
     mocker.patch.object(worker, "verify_chain_of_trust", new=noop_async)
     mocker.patch.object(worker, "generate_cot", new=noop_sync)
     mocker.patch.object(worker, "upload_artifacts", new=noop_async)
     mocker.patch.object(worker, "complete_task", new=noop_async)
-    status = event_loop.run_until_complete(worker.run_loop(context))
+    status = event_loop.run_until_complete(worker.run_tasks(context))
     assert status == task
 
 
-def test_mocker_run_loop_noop(context, successful_queue, event_loop, mocker):
+def test_mocker_run_tasks_noop(context, successful_queue, event_loop, mocker):
     context.queue = successful_queue
     mocker.patch.object(worker, "claim_work", new=noop_async)
     mocker.patch.object(worker, "reclaim_task", new=noop_async)
     mocker.patch.object(worker, "prepare_to_run_task", new=noop_sync)
     mocker.patch.object(worker, "run_task", new=noop_async)
     mocker.patch.object(worker, "generate_cot", new=noop_sync)
     mocker.patch.object(worker, "upload_artifacts", new=noop_async)
     mocker.patch.object(worker, "complete_task", new=noop_async)
-    status = event_loop.run_until_complete(worker.run_loop(context))
+    status = event_loop.run_until_complete(worker.run_tasks(context))
     assert context.credentials is None
     assert status is None
 
 
 @pytest.mark.parametrize("func_to_raise,exc,expected", ((
     'run_task', ScriptWorkerException, ScriptWorkerException.exit_code
 ), (
     'upload_artifacts', ScriptWorkerException, ScriptWorkerException.exit_code
 ), (
     'upload_artifacts', aiohttp.ClientError, STATUSES['intermittent-task']
 )))
-def test_mocker_run_loop_exception(context, successful_queue, event_loop,
+def test_mocker_run_tasks_exception(context, successful_queue, event_loop,
                                    mocker, func_to_raise, exc, expected):
-    """Raise an exception within the run_loop try/excepts and make sure the
+    """Raise an exception within the run_tasks try/excepts and make sure the
     status is changed
     """
     task = {"foo": "bar", "credentials": {"a": "b"}, "task": {'task_defn': True}}
 
     async def claim_work(*args, **kwargs):
         return {'tasks': [task]}
 
@@ -169,9 +196,9 @@
         mocker.patch.object(worker, "run_task", new=run_task)
     mocker.patch.object(worker, "generate_cot", new=noop_sync)
     if func_to_raise == "upload_artifacts":
         mocker.patch.object(worker, "upload_artifacts", new=fail)
     else:
         mocker.patch.object(worker, "upload_artifacts", new=noop_async)
     mocker.patch.object(worker, "complete_task", new=noop_async)
-    status = event_loop.run_until_complete(worker.run_loop(context))
+    status = event_loop.run_until_complete(worker.run_tasks(context))
     assert status == expected
```

### Comparing `scriptworker-8.1.1/scriptworker/test/test_cot_generate.py` & `scriptworker-9.0.0/scriptworker/test/test_cot_generate.py`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/test_utils.py` & `scriptworker-9.0.0/scriptworker/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/test/test_config.py` & `scriptworker-9.0.0/scriptworker/test/test_config.py`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/cot/verify.py` & `scriptworker-9.0.0/scriptworker/cot/verify.py`

 * *Files 1% similar despite different names*

```diff
@@ -409,14 +409,15 @@
         frozendict: maps the valid task types (e.g., signing) to their validation functions.
 
     """
     return frozendict({
         'scriptworker': verify_scriptworker_task,
         'balrog': verify_balrog_task,
         'beetmover': verify_beetmover_task,
+        'bouncer': verify_bouncer_task,
         'build': verify_build_task,
         'l10n': verify_build_task,
         'repackage': verify_build_task,
         'action': verify_parent_task,
         'decision': verify_parent_task,
         'docker-image': verify_docker_image_task,
         'pushapk': verify_pushapk_task,
@@ -1473,14 +1474,30 @@
 
     Currently the only check is to make sure it was run on a scriptworker.
 
     Args:
         chain (ChainOfTrust): the chain we're operating on
         obj (ChainOfTrust or LinkOfTrust): the trust object for the beetmover task.
 
+    Raises:
+        CoTError: on error.
+
+    """
+    return await verify_scriptworker_task(chain, obj)
+
+
+async def verify_bouncer_task(chain, obj):
+    """Verify the bouncer trust object.
+
+    Currently the only check is to make sure it was run on a scriptworker.
+
+    Args:
+        chain (ChainOfTrust): the chain we're operating on
+        obj (ChainOfTrust or LinkOfTrust): the trust object for the beetmover task.
+
     Raises:
         CoTError: on error.
 
     """
     return await verify_scriptworker_task(chain, obj)
```

### Comparing `scriptworker-8.1.1/scriptworker/cot/generate.py` & `scriptworker-9.0.0/scriptworker/cot/generate.py`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/utils.py` & `scriptworker-9.0.0/scriptworker/utils.py`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/context.py` & `scriptworker-9.0.0/scriptworker/context.py`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/version.py` & `scriptworker-9.0.0/scriptworker/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             'Version tuple is non-semver-compliant {} length!'.format(version_len)
         )
     return version_string
 
 
 # 1}}}
 # Semantic versioning 2.0.0  http://semver.org/
-__version__ = (8, 1, 1)
+__version__ = (9, 0, 0)
 __version_string__ = get_version_string(__version__)
 
 
 # write_version {{{1
 def write_version(name=None, path=None):
     """Write the version info to ../version.json, for setup.py.
```

### Comparing `scriptworker-8.1.1/scriptworker/artifacts.py` & `scriptworker-9.0.0/scriptworker/artifacts.py`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/client.py` & `scriptworker-9.0.0/scriptworker/client.py`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/config.py` & `scriptworker-9.0.0/scriptworker/config.py`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/log.py` & `scriptworker-9.0.0/scriptworker/log.py`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/constants.py` & `scriptworker-9.0.0/scriptworker/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,14 +158,15 @@
 
     # scriptworker identification
     "scriptworker_worker_types": (
         "balrogworker-v1",
         "beetmoverworker-v1",
         "pushapk-v1",
         "signing-linux-v1",
+        "treescriptworker-v1"
     ),
     "scriptworker_provisioners": (
         "scriptworker-prov-v1",
     ),
 
     # valid hash algorithms for chain of trust artifacts
     "valid_hash_algorithms": (
@@ -222,29 +223,37 @@
     'cot_restricted_scopes': {
         'by-cot-product': frozendict({
             'firefox': frozendict({
                 'project:releng:balrog:server:nightly': 'all-nightly-branches',
                 'project:releng:balrog:server:beta': 'beta',
                 'project:releng:balrog:server:release': 'release',
                 'project:releng:balrog:server:esr': 'esr',
+
+                'project:releng:beetmover:bucket:nightly': 'all-nightly-branches',
                 'project:releng:beetmover:bucket:release': 'all-release-branches',
-                'project:releng:googleplay:release': 'release',
-                'project:releng:signing:cert:release-signing': 'all-release-branches',
-                'project:releng:googleplay:beta': 'beta',
+
+                'project:releng:bouncer:server:production': 'all-production-branches',
+                'project:releng:bouncer:server:staging': 'all-staging-branches',
+
                 # As part of the Dawn project we decided to use the Aurora Google Play
                 # app to ship Firefox Nightly. This means that the "nightly" trees need
                 # to have the scopes to ship to this product.
                 # https://bugzilla.mozilla.org/show_bug.cgi?id=1357808 has additional
                 # background and discussion.
                 'project:releng:googleplay:aurora': 'nightly',
-                'project:releng:beetmover:bucket:nightly': 'all-nightly-branches',
+                'project:releng:googleplay:beta': 'beta',
+                'project:releng:googleplay:release': 'release',
+
                 'project:releng:signing:cert:nightly-signing': 'all-nightly-branches',
+                'project:releng:signing:cert:release-signing': 'all-release-branches',
 
                 'project:releng:ship-it:production': 'all-production-branches',
                 'project:releng:ship-it:staging': 'all-staging-branches',
+
+                'project:releng:treescript:action:push': 'all-release-branches',
             }),
             'thunderbird': frozendict({
             }),
         }),
     },
     # Map restricted-level to trees
     'cot_restricted_trees': {
```

### Comparing `scriptworker-8.1.1/scriptworker/data/cot_v1_schema.json` & `scriptworker-9.0.0/scriptworker/data/cot_v1_schema.json`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/worker.py` & `scriptworker-9.0.0/scriptworker/worker.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 """
 import aiohttp
 import arrow
 import asyncio
 import logging
 import os
 import sys
+import signal
 
 from scriptworker.artifacts import upload_artifacts
 from scriptworker.config import get_context_from_cmdln
 from scriptworker.constants import STATUSES
 from scriptworker.cot.generate import generate_cot
 from scriptworker.cot.verify import ChainOfTrust, verify_chain_of_trust
 from scriptworker.gpg import get_tmp_base_gpg_home_dir, is_lockfile_present, rm_lockfile
@@ -22,16 +23,19 @@
 from scriptworker.task import claim_work, complete_task, prepare_to_run_task, \
     reclaim_task, run_task, worst_level
 from scriptworker.utils import cleanup, rm
 
 log = logging.getLogger(__name__)
 
 
-async def run_loop(context, creds_key="credentials"):
-    """Split this out of the async_main while loop for easier testing.
+async def run_tasks(context, creds_key="credentials"):
+    """Run any tasks returned by claimWork.
+
+    Returns the integer status of the task that was run, or None if no task was
+    run.
 
     args:
         context (scriptworker.context.Context): the scriptworker context.
         creds_key (str, optional): when reading the creds file, this dict key
             corresponds to the credentials value we want to use.  Defaults to
             "credentials".
 
@@ -39,15 +43,15 @@
         int: status
         None: if no task run.
 
     """
     loop = asyncio.get_event_loop()
     tasks = await claim_work(context)
     status = None
-    if not tasks:
+    if not tasks or not tasks.get('tasks', []):
         await asyncio.sleep(context.config['poll_interval'])
         return status
 
     # Assume only a single task, but should more than one fall through,
     # run them sequentially.  A side effect is our return status will
     # be the status of the final task run.
     for task_defn in tasks.get('tasks', []):
@@ -73,43 +77,51 @@
             log.error("Hit aiohttp error: {}".format(e))
         await complete_task(context, status)
         cleanup(context)
     return status
 
 
 async def async_main(context):
-    """Run the main async loop.
+    """Set up and run tasks for this iteration.
 
     http://docs.taskcluster.net/queue/worker-interaction/
 
-    This is a simple loop, mainly to keep each function more testable.
-
     Args:
         context (scriptworker.context.Context): the scriptworker context.
     """
     tmp_gpg_home = get_tmp_base_gpg_home_dir(context)
     state = is_lockfile_present(context, "scriptworker", logging.DEBUG)
     if os.path.exists(tmp_gpg_home) and state == "ready":
         try:
             rm(context.config['base_gpg_home_dir'])
             os.rename(tmp_gpg_home, context.config['base_gpg_home_dir'])
         finally:
             rm_lockfile(context)
-    await run_loop(context)
+    await run_tasks(context)
 
 
 def main():
     """Scriptworker entry point: get everything set up, then enter the main loop."""
     context, credentials = get_context_from_cmdln(sys.argv[1:])
     log.info("Scriptworker starting up at {} UTC".format(arrow.utcnow().format()))
     cleanup(context)
     conn = aiohttp.TCPConnector(limit=context.config['aiohttp_max_connections'])
     loop = asyncio.get_event_loop()
+
+    done = False
+
+    def _handle_sigterm(signum, frame):
+        nonlocal done
+        log.info("SIGTERM received; shutting down after next task")
+        done = True
+
+    signal.signal(signal.SIGTERM, _handle_sigterm)
+
     with aiohttp.ClientSession(connector=conn) as session:
         context.session = session
         context.credentials = credentials
-        while True:
+        while not done:
             try:
                 loop.run_until_complete(async_main(context))
             except Exception:
                 log.critical("Fatal exception", exc_info=1)
                 raise
```

### Comparing `scriptworker-8.1.1/scriptworker/gpg.py` & `scriptworker-9.0.0/scriptworker/gpg.py`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker/task.py` & `scriptworker-9.0.0/scriptworker/task.py`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/setup.py` & `scriptworker-9.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/scriptworker.egg-info/SOURCES.txt` & `scriptworker-9.0.0/scriptworker.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -80,34 +80,30 @@
 scriptworker/test/data/cotv2/actions.json
 scriptworker/test/data/cotv2/cron.json
 scriptworker/test/data/cotv2/decision_hg-push.json
 scriptworker/test/data/cotv2/parameters.yml
 scriptworker/test/data/cotv2/projects.yml
 scriptworker/test/data/cotv2/pushlog.json
 scriptworker/test/data/cotv2/task-graph.json
-scriptworker/test/data/gpg/.gpg-v21-migrated
 scriptworker/test/data/gpg/0
 scriptworker/test/data/gpg/0.gpg
 scriptworker/test/data/gpg/gpg.conf
 scriptworker/test/data/gpg/pubring.gpg
+scriptworker/test/data/gpg/pubring.gpg~
 scriptworker/test/data/gpg/random_seed
 scriptworker/test/data/gpg/secring.gpg
 scriptworker/test/data/gpg/trustdb.gpg
 scriptworker/test/data/gpg/keys/docker.root@example.com.pub
 scriptworker/test/data/gpg/keys/docker.root@example.com.sec
 scriptworker/test/data/gpg/keys/docker@example.com.pub
 scriptworker/test/data/gpg/keys/docker@example.com.sec
 scriptworker/test/data/gpg/keys/scriptworker@example.com.pub
 scriptworker/test/data/gpg/keys/scriptworker@example.com.sec
 scriptworker/test/data/gpg/keys/unknown@example.com.pub
 scriptworker/test/data/gpg/keys/unknown@example.com.sec
-scriptworker/test/data/gpg/private-keys-v1.d/13435A7D795A0EDFE123D5A451B6A5B670DFA9FF.key
-scriptworker/test/data/gpg/private-keys-v1.d/45BC537FED9E18BCAF3D395776DCE3202608DC6A.key
-scriptworker/test/data/gpg/private-keys-v1.d/78458D66CA889DAEB13DECD75729160BAA505783.key
-scriptworker/test/data/gpg/private-keys-v1.d/C5988D51364F8C7A157E276A346622A8ACA94653.key
 scriptworker/test/data/pubkeys/manifest.json
 scriptworker/test/data/pubkeys/data/36E592251DFD8D491E6E9BE701222703321F2BA2.asc
 scriptworker/test/data/pubkeys/data/3F4DF62D10F3AD93E98119180C0D5CA75269246A.asc
 scriptworker/test/data/pubkeys/data/D1B5423204A833E7A3420C803112C5A1B0BB87EA.asc
 scriptworker/test/data/pubkeys/data/EB55E1CED1FF0956E2BFE6C8D0B3B9C1094A9A3F.asc
 scriptworker/test/data/pubkeys/docker.root@example.com/D1B5423204A833E7A3420C803112C5A1B0BB87EA.pub
 scriptworker/test/data/pubkeys/docker.root@example.com/EB55E1CED1FF0956E2BFE6C8D0B3B9C1094A9A3F.pub
```

### Comparing `scriptworker-8.1.1/tox.ini` & `scriptworker-9.0.0/tox.ini`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/requirements-prod.txt` & `scriptworker-9.0.0/requirements-prod.txt`

 * *Files 11% similar despite different names*

```diff
@@ -10,33 +10,39 @@
     --hash=sha512:1b3e3c8c09308a84364d561de459ab8915cbd7cc43b7747e31582574b0f0cd7b1d3628c39b22d9c6f6a4d16226749ac1667290bc560482d997c53cfff5c832b7 \
     --hash=sha512:9a5af29dfdd74827c5d0032906daf821eaed27f0c20759af0acf29ae2b8d704300b508788832341a0014a78301ad1b726c5898e3a6fa49258c666e8d318ccda0 \
     --hash=sha512:1890e6b8aa96beb51f7a196ca287fd6ed905b99e6d139d7b29174478ce3947c0dd7bbe933116836a8276a483811054d928bc55774a5eb542789c3779b7b042bd \
     --hash=sha512:a9d2e9ae96e80e8cf8ae5a62513ac945093ef0aa59106e20ef650a1ed196748c5cd321f1da6ffaa965f4fb1b266cdaf5937bac3714d67df495855d5938645e90 \
     --hash=sha512:13733054619053893f4a8d75c1da020a87e1f697b007ab182be06b5b941b49c4cb3dc6f9ff131be6bc10fc727ad7334fa5401346f3a77140aed0f86280532fce \
     --hash=sha512:5ff411ddbbf733ad52334015a04eb061998803ff94ad474ea2d534a713aa302cdfadde908ff2bb1dbd4f13e1a1fb99786f8dd1be1e061fcb6a7c0f471e41591f \
     --hash=sha512:4ae6c5843688f45751ddb14a8b6f16f58b1f8a4805be430afa4035857b1826be95a8422395d64ac88282f9edd57f35fee5d1b6a4dab9093d47491d300d2079f3
-aiohttp==2.3.9 \
-    --hash=sha512:80d1fe481d6ce7d465252e27951c50f96e005ef54dd0fdf49269e2267d6b096a3a0c9e6a3aef75854559dbf57760651a7f36e1fdab3263cc0b33a17ade8d34cf \
-    --hash=sha512:5049d881d33bbbcb9997eef5ccc9eccff675c0f425806765b36af861ae10756fd8ec67b810b2a28436931b746077266aa1a450dc610a3cc36c195b4fd29b1804 \
-    --hash=sha512:8c599a34591b26d0c46e2c626a7e7c714b66ead04fbe130ce91ad1ded9953f4886beeb8e3551725460927ac177b95d03566b1fbaad7baebc30bbbeb600a599ab \
-    --hash=sha512:be8a6db5eb9f5974443ec26da816fcaaed59a1592d2686085523b13f732c5e25191cd47f27327b35fbdf4303ba9a6cd3a45f7f04a4c914544261c9af7a3cbee5 \
-    --hash=sha512:fb11ad5b2c849b107372e8d6a2b0fa2e29ddb83d524da8b036f4df03ed79292f2328fe5c6b80d7cc0b57059d27fcb151789238ce7f18f8eb6d34e9ede543a5e5 \
-    --hash=sha512:904ee46b2468c3fb9a7582e55a741cbb68294e9ae4feafc3493d4761345ebcc13969c76b87368d38ae3ca1aead47ca05577f20dd85342244c352cc0679b63d01 \
-    --hash=sha512:92df4fb2f369b663b544bc82813872e09c7171f7ddafdfa52ba0170eccb6e8ac0a75d1784f40a5559f9fecea84c8876157ee47918cb3eabb159176bf0ec84b26 \
-    --hash=sha512:798ef8f226613090595f0135a4b3441e084a16bb66ef085853a0463c05f4a1d275c4fd64013b0a23d8f28dbee53a689516f56a0f44526e5c537271792a175896 \
-    --hash=sha512:17ed05007b6e18d8d116ea188c0477dbfc5653d1d76cbfe521398f40e153a1d07223688a8a819190ed8c3f5a377930b25da1bb458822fbbfc16e3d17b190b07b \
-    --hash=sha512:5fb010146e341263db44e5e64277914a426aa3c5399c9d08965ab401119edcc45104075a52b80fdd8180dd444c2bd367e4bb5b2914afc63ae3f92e95643437e1 \
-    --hash=sha512:883905e1e6de254eba677143f03d9c5b308d5dd8826d07313b9da630ca6787478ce4c3bfbe11e3c808bc4179b3adab5140087b1cca2ee6bb80ee2bf3c315e713 \
-    --hash=sha512:af4a10ae986acac3909e3301e9a2cd232eea87f97ec30cc1ee12e62e926d57ba618f706bebe4f1599dd1352099d25f40a458ad497ed02b91316fc3d331f91d66 \
-    --hash=sha512:e0675ecbe27ef12f2165c2e8f3ed05e2205786797e72f0ae7ee2bede1fca1b932a41837fdacd2083195c30049f0d3ba020589144683aae3353c31d279e42a7ce \
-    --hash=sha512:944001747640008791d90820304ce8f0bff50e30c661a72fdd46f2c523996f0f25419bc231c8dfe298233c9a75c26ceab8370ec7c3fed06a17b9f6582d01a9fe \
-    --hash=sha512:bba4ed6ee2cffc53fbb8562135da1018cb2c0416af78ddb209a582c86215cef5ce4db17262b58d834f87e9103d0ce47539cc7507cd5ed9f8ee3aa69c3c4f6f5f \
-    --hash=sha512:0fe2bbcfc5b9b145a129ebee3b802e9dff5bc00030ce1fa5cea8bb63575be71c657289a92a020fb4fe8b9b5d5a0871234a630c3e9562a464cd43741b19a3b82f
-arrow==0.12.0 \
-    --hash=sha512:bbe4bd0b80de680079fdd5e4575750525df714a98945ea7b8e28b88def0bb094a928083d0afb71d5d7e9294feadf44d070239b5566c866a0fe67fbb7274061b5
+aiohttp==2.3.10 \
+    --hash=sha512:15345f91cff581f6b6b9ec099504564749a4f054b60cb5757e8af740235aea0711cb8c15ad1dc54a0caedf73039493b5a1d21a98e2a80c5c0f3d83a63cc58ea1 \
+    --hash=sha512:9cad43b6021d40f8d4bf01e7d64f7d2fb26eeab112476b34141ffa450338078a7fd3aa56fdd782994c2b7215e28d6d0bf573f7696600625a16bebd871eae2393 \
+    --hash=sha512:0da9d1b885a16adf1d4f6ca63cbbf92c747e242a02d7d95c6f453fff57a84506cb7c36dbd93b1708a4eddd1c248da22a1eaf39864432daafd598b6531074ef99 \
+    --hash=sha512:3527178423dbc5a3c55dc1d13b3ab341f28be07edf3eb0c68c9fccb08dddc9ea1c26bbcffe361e42069d1472a0abaf4e8a9d274b6049664698160b55e6a40b76 \
+    --hash=sha512:8b4691d6aa9146c14a1cdf0f488cbca804654fa58311d15f34f9b1edbaed59d923e34b4ef28a0b206eb99fbf078fa41bf2cf3e36e9dc116679f5aec997c2cf09 \
+    --hash=sha512:05e581a5c08f16443b10a8c49e9e7c2cfbd0ca3d95e4150bd59458c0c865429fab6fbd37aba53402ceac5fd3dceecfcbce48e8c7389b9b74c7eb17ecbfc35699 \
+    --hash=sha512:b3caaaffdec94e5a542a5d0246e6c4a88ea290d4a03fdb3a0c43cdbe646ff44a0a9ad4c5dfef08e017ea4edf6ebc7d6dbe06b435439b0b743d7cf09479c35f6f \
+    --hash=sha512:7581a091f011578fbf689b9245e2f307599e1694e97f0baf66973632ad1e4c6370722f4d1c41f7213854e206639a11a6c3f73eff2cb57baf5482648aa48d33ba \
+    --hash=sha512:438f6377a00556094cf2185953dca6296ab4c99dc06e15477408a91833b691868ff5c3ccca65cbd2c5b13eccf3ee8f0e834c5c530b25da62e549e503d14a74c3 \
+    --hash=sha512:4256dda88eb9de3606964828a213fbd587d75ee81a8867471cb6884212901df9d2e0caf26e98eeb1fe5f3204e324ad6600724042ac5cf1d16dc972343ac26432 \
+    --hash=sha512:aff7e3c900f6f4a0a04dfaab4d3f2577ac2f3927fb39014f0d2d651d4c524cb7eb2950257e24bfd3d66fad6aecb0965229c20959cff5c0cf8037a885c55b6481 \
+    --hash=sha512:5daca902c8148154589e9611d81709883c4d9880d9812b868eb81619ae324420fa4e6caebb6484418d898c0bc2013c00dcb69cf677337733a157f5d8570fc972 \
+    --hash=sha512:de8e714f5aedca9d5ccc734961200bd78b1c567c58a2bd54ed777903d68df3295280f2606d374322ef9923644a0389947ea0b5756e02d6f84c0f2d3d9265f633 \
+    --hash=sha512:ec9c454d782e4f4f5d191521eeeeaa9e39a7fc193d6cff876214233b2dd8df1e43ac69ae1654ccb8fc968e9f6b0880cdcc8c464754ca86d52d599fa25e313be0 \
+    --hash=sha512:0dbf0a40d31ecab8129595975fb9aa28bcc8587d3409afe45800c402b177140e8190f54df82b03227597dcd17d776449efd12038eb3926023767df66ff2ec039 \
+    --hash=sha512:cf83e1357eefb8bdf1542850d66d8007d620e4050b5715dc83f4a921d36ce9ce47d0d13c5d85f2b0ff8318d2877eec2f63b931bd47417a81a538327af927da3e \
+    --hash=sha512:20f9ed5ee61487914f190e4cbcd4ed50b3c9805a368ac54a0440bbebc09966d8bd46812ea15b157825faba0a445a30cfec32b182b3bda47d13a71f2be62c7411 \
+    --hash=sha512:cf83e1357eefb8bdf1542850d66d8007d620e4050b5715dc83f4a921d36ce9ce47d0d13c5d85f2b0ff8318d2877eec2f63b931bd47417a81a538327af927da3e \
+    --hash=sha512:87afdb9531cbdfe6547ea5564d4fd97a75aa7c9749bb8f53a8e67d3976d43d02b9b5dd6a06886bb81ca5c23a60f2517e3049397c091727db505698bdc5898c70 \
+    --hash=sha512:049587b76d99365daebbf8ee9a6fca3c291cd797c26ffa16437119e1ec1616f4648601a56b6a506f92df5a420d8194f8bae11076e1f56963657da5615ce98b0d \
+    --hash=sha512:cf83e1357eefb8bdf1542850d66d8007d620e4050b5715dc83f4a921d36ce9ce47d0d13c5d85f2b0ff8318d2877eec2f63b931bd47417a81a538327af927da3e \
+    --hash=sha512:e4ea725bbd3d7d749f2ec21eea1ff9f5c836fbeaa17ad72f77e378c69b008448e57503175bee6adff86110f65edc915cb6368df3011d1d9d61cf47718b086be0
+arrow==0.12.1 \
+    --hash=sha512:cf83e1357eefb8bdf1542850d66d8007d620e4050b5715dc83f4a921d36ce9ce47d0d13c5d85f2b0ff8318d2877eec2f63b931bd47417a81a538327af927da3e
 async_timeout==2.0.0 \
     --hash=sha512:bc5a170662083abf018ac8ecde1f8c3182c543abcd6323e565f9493cd19c703f11ab0deb9f3385f85c31977959c84d393efb3219539a90ba7ff0ba69110e8bdc \
     --hash=sha512:c0f5688c24a470de0d8d390980464eb0574cf3b86e39864533bd8de53282ebc4c4d4db135f8b9eea8b7a8be342219c09bc12e58a4108f2483e94bb68e684a91f
 certifi==2018.1.18 \
     --hash=sha512:bc5f15eb111ee52b177727226b5bd459df38b9227ff4e24c4611b163ccd576f19d8a8025109a2e39e236190a81bd93150ab6c54cd4a5fb719ec89f0b14b5a8bd \
     --hash=sha512:5a419fcd6ad2dc095e126bcff40127b4549cc0556e19157b142c6f27b284448eb3124fb92a72b147d6734d9f3ff212212dcbf364e127c2691ab94a9736cee032
 chardet==3.0.4 \
@@ -49,47 +55,50 @@
     --hash=sha512:dc593b33101802b014b6f6aa58b165827da9ee1eef92787a9da5fcbf1bfadf390cb50bb9095f320b5adc57a015621e0b8dd2269b58c89803e7f4018585a890e9 \
     --hash=sha512:a57f5b3fb25fca4e33e4816a66babaa6a0345b48c4743ab51df672d37bcb5e0073b1bd5a87dfe1e416869045715a86f33de23c7173151f79317c76b412455c5f
 frozendict==1.2 \
     --hash=sha512:095cf5f6f8b02bf5666e04200431992bf4b3160aae3464d528bc256b1ab643e29dda78fe94d9e8c983dbfe66cd2459e0559122e17b6b8660c0552adc5318b3da
 idna==2.6 \
     --hash=sha512:d6f64f657f1c97edfc6f92582e9fcb6c7fbee0e830b5e830d9b03483adf82400819158eff44aa0a4d05f42ecee0cc728f58589f0ce5f70e87f50dd4fa1cb8c63 \
     --hash=sha512:cb5dbfab44c4d11521c67f9d29391f184d1267a3da6dc89f4ed12c60a7a909d5c7474c3ea2bddd0af7063f4f620e87a8dd586bb07e8b961b30b1dd7c969704c2
+idna_ssl==1.0.0 \
+    --hash=sha512:d1f7479cc3edff164bb26deb05af757906ba91241bc668f1b087560087a89f741a0b36e166bfb8142128ceed6008621ab36a2556ed2304ea6374c19982bc663a
 json-e==2.5.0 \
     --hash=sha512:8e557758bc5089db5b3a6c22e3de77e3c2db59f46699e118d1adfeea6d6649c21748a410445875cf99b389794fd4bcd16d87d95368bae34a29b5f9e636cb2310
 jsonschema==2.6.0 \
     --hash=sha512:d0be26145ea5ec8d701f636016e3cdd068a603170c527584bf9722bcdee4570ea657ed0744f8e435cab34aade569fffc1f55db9e68b6b7b7b0151020a2602946 \
     --hash=sha512:03f916abd023b32fbe60f91718d6f2f94d8834bd1bd8ec85ab02f591a145161275c2cde25b037c4d2e94703b870159feb776d3556f011e4c394d2e20ab897b0b
 mohawk==0.3.4 \
     --hash=sha512:7cdbc98b5bbdc269ebbc614b818dcd35e118b7722293bdba89e5c1bb5dbd92bd6c113895ec893a7ceeb696c67ef894b61f1131729724fce7574e36707fa16714 \
     --hash=sha512:f5a5d99d80e7806f92d5078d4d6a7f0b1fd1d4759a9897cfd178fe1ed07b27831c707dbd9b8b6a735d392845e532f2805e27cfd78e69ea72f22efaac1dafc9a5
-multidict==4.0.0 \
-    --hash=sha512:b0886af392db8c94a7e70ff65eb3bde61b78ee02119fdd1fee595613d0c49cd067b7c7b154f9bc6e489dd8b7727d2b91d930b7df9695ad788572ed7152d269e9 \
-    --hash=sha512:96ed55d0f9c785a70c5097a4367c21b1fb5cfd03335958c59653d61c77798141422fcbc2e374ad950d8c3e44634c50c1e8117703fc4ecbd3ef7251522413f028 \
-    --hash=sha512:44111b919c1fa517e80e85f2d1c99940daf6fe54e9015a5749d6c18afe82881c8b5e79d8abc66720ac12367625351735c86786528b6b4fdcf454c4b39af40776 \
-    --hash=sha512:90aa9a096b6cf8ad7e49ba8256fb54fb3c9318d1a2cf6388ddb1de0f9d373feeaed28dfaecbc93db813eadc306cfd8877bf5232ff287e518e311c37babbbed8c \
-    --hash=sha512:a872fe9e69328202bc8ad8ba0c156283dee973b34dcfe2addae47e674a1cf39e3fa657dd758fe2e640a2f0d6cc422e7e999ed6120b92470ec737cf2d08d7d516 \
-    --hash=sha512:fefbb27563cd8cb8d20d1006cbfa8788f9102b9d6584d158dcfe433f324a64357b8d8e6668ab60acf68ecd9a397b2844a7564c183a7b8bb570fb308c43407898 \
-    --hash=sha512:6704547bcb712949a94c012e9a8a97e5688d0cbda8d011da3649ad54bda8a6716ca7732821251212036dfcc59424bd4796529d50732bfa48766bac3ff80c7c83 \
-    --hash=sha512:9e81a3c98d895ab02b7b8df72e63ec2c69553837f16fe910e3b023e5138bdda1afef93cf5b22679adf2c70b3c077f21397a6506ca4240f547fdacf3aff12a36f \
-    --hash=sha512:6525cd4da5d3949ba873ceb533634a9addb99ba236bbcd71de8541241e9e0b440bf5f0a423b3736325ef1577ea2f9a204d0a152ed943f17dcaabc011e70bf474 \
-    --hash=sha512:9306ac40900c7435ab10453b5334d00768d062dbf53daf5899b410b59ddd6ff77ea89c7f89537628b23cbce5233982e509fb301fe6adf8c18d20e5414ad3644d \
-    --hash=sha512:8ceb5d0efb0fdb0f040ef21a13064f7dcdcf70fea6e0cb50c3d381ebda8f0e0c8259f3a54dd5a33631fd545f879d417dd4b5d2439b2a24280ff4367d36732b37 \
-    --hash=sha512:a5366f793666813e4d657854e05f41385d232da6146e0c113d45282c5a3983ab7d16a2dfe3af4cfab004370f5abbd47c639e027ef1e91d74c9384650759e767d \
-    --hash=sha512:7b618ce9de23e3ae68a9f141f6ee7462eab82bf6c61651224dc9ee0abe38482ec01132b30a76d681d8cb85564754e5b2bf1973ad4b5ed7dc742d40e20cde59a4 \
-    --hash=sha512:a9ceef2e07ef98c1e37f68551e1605ad622b739dc1054127bd4ac450cf837563aaebdd4652b97f68f8d8debf6b9ae3098e74dfb60d14f23246b1b1983c5ebed1 \
-    --hash=sha512:5ede1479992906bbae17f423f23a169e0e8c31b3bb894f50320d9c7cb4507284c9a60e41023873f1f9f09d555cd3f932792e0c883d4cee8abef22c5acd976884 \
-    --hash=sha512:ea3c1067d9abb79601e216e8a8455ed40f7c3128109e511aa66b6aff0887fd7ee160f8b0706d3042b2d47ad29c84be0cfef76512c10dbda96fad27162b3cece3 \
-    --hash=sha512:9b0dd0447ee375fe60fd84846d62f5e2ccae1d435d921e1e0ae831f7e20d02f14ebb80781437eb0f01e1aff9d42c3eb84dad41e1d6bcf78035c294d31593cdb2 \
-    --hash=sha512:4306b885f0538b44b2ecbf3b1cbb7556dafd89e7c974e5f7720c1ab6b9e3b636d5792495c9697cb2df2bd8fb2ff7c4777f5f8a913b6952ec00ce1dbdc4fbcb03 \
-    --hash=sha512:a9a00dceff365766faf9799820716aca35d0a4fc619dde1554db25a96cff4c36ca4dd9c16d4c0ec75ee55e91a017dff32120d48c617a31103ce1f06b92384968 \
-    --hash=sha512:1eacd18580403a647234397e5089a05f77ca7e0bb2c32c4c1c56c788122daf6b0f70fb3efe0bd9135addcf879367308984ddcd5368210a86ed796f06efd85d29 \
-    --hash=sha512:0f7d8e75e62090aee2decbab07478c250a1a5d61e46115a44c2fac4b0bffc4779b80c942bb18eabff5a3e53f20ad6ddf4935865d0055a80f5367be7f2e06f3c8
-pexpect==4.3.1 \
-    --hash=sha512:ef8e0153c2c079919bc3a5182f3d3bf865670f8748322f4f6e39f05c06f396640bd73471aa7eca9e3aa78c7fdd7323369820a38b818cc60fcd5ea166bb2b7014 \
-    --hash=sha512:eb1416aa1f803d52a3c3663ea1b982f34489d1924df44bf2d36ba63699fa8c98c04437f4bf49a312dfcd01c35b062acb93095fcde7055595fd4c11b933039cff
+multidict==4.1.0 \
+    --hash=sha512:c8facfe9d66f724f3696ed2b4e388c361e604350148fd46d355fdf15e3af4e39b3999308234fbffbc91bce8c92c221406ff544ca59d7ed7625ab9560e83d4171 \
+    --hash=sha512:de32a0442d00e3c7afe432c311b72fd087bd2ba430d608b0e6d89cf2cef570b242e6096cf4d4cbef3682618b0afb06e023051a65203cd60d311832f82aa93087 \
+    --hash=sha512:e1ab81e09860dec0bb5ae6c490e4628bb4796225b50283c8dad920f92d961217637415c69ee687b5cff6f997cd3e21fe2da2ea3636d0d4edb18707672fd48dc2 \
+    --hash=sha512:3efd0769e1e177cfb24c5565b0257b7154f56d7388b6f0b755dea701c17755d7faf2f03a61e2058bcab901351277d4ed989e4a8ff86b8c8b4070159f2e021b42 \
+    --hash=sha512:5f0fd64d80e688c351f2a4c666f18cbaec994450a890f30b73c706b60a69cd5b475b28cbc9daff9b2b6cb4b08d641226b7e6cc98bd19bba7029fc7dd8cab80aa \
+    --hash=sha512:ead267a4a7be9bfe1f383df01b186b7cdca0433c3afdd4ac7f06ffafc0ca6146ccb474130ba50132951edd0141352ade377dc8f85c476a3e79d9319772316a47 \
+    --hash=sha512:fe90c2a4a2af944e9fc29e85bcdcf1a43ad1f8482dea0eb46b76a6a91049d5cc648a118dde94f1795fa00b490c378205d6f8176092a443fe3716efb11c44766d \
+    --hash=sha512:0975ef4501a97ed5c3d81572015c10a57354647251ceb7500527d4ff44d16c2ec0046b045de1a0de0f52cc9692713e87770f9a9cb5828413c3731a4230963842 \
+    --hash=sha512:811dd4d170a0c66fb8ca59fd005f748c87753ae9acbb4bc4e2a912427237345bce27cf12b4958e2538db92971309afb2f8f92148cfa7e50f5da367afe54ac231 \
+    --hash=sha512:a4321ed67e9715e1fcb15520c8234c7b6bc4dc54569cf237255bf7488a3e31b4f6e39d64741a8703aa71265f4bec865cb46900c80548c19fb58fe873d332d2a9 \
+    --hash=sha512:557c7b5f28fbfbe7f93dae9e14dfa8dc249e4d36106768eaebac8aa9afc5ddda702d4b14b916111a3b9b56fb3c13f65d45a44e60670f2402b3a3302f75147cf2 \
+    --hash=sha512:6e87baeb187fc95c68b7e8211adb8c8a22594572c0dcea99b57dc7c854d6016e5b0695e8c1ba4f026ef4da6103dc67afd1c925d9ebeae931ab24e58495e9cba1 \
+    --hash=sha512:d68f839c6a478b5901e5f29c18f8b386f1082ed2291da89dba69f98faa1b95fe07529cfd885d6753532711fbf231d3163f072cb98b47085a6a8b525b310c5a7f \
+    --hash=sha512:56c2cf11a64674bc56b7f3c7fa72c2148928b75c28f81cb54c3d400ce171e71248c31cb2c7d8bb7af4661b9ec7a5e18fbba8a58e4673519bcdd3bde13f3ca59a \
+    --hash=sha512:925adffc96d8280b6aaf7c9d37fb910cde0ec1c1a89738170e924250387a2a5a5f57fafd923c220d146c6093f0ab11b0d0775d302a2657424c836807074ccd99 \
+    --hash=sha512:6a04bb8ae10b4c86cc27439d32b2ca120ca0afd1d2620632a31369cad9b790ac1214b912bdbeeaf185d79bc9b38018450f848575016d64941b85d60a3cf31c0f \
+    --hash=sha512:ead23a4ec6ff0a7751d0e8aa9875edb6e5585bf4f403f6c2219046e694778e4d388c2c502109e52950d783255ff2fbf15ddde8d616a9620ab05b61673dcefaae \
+    --hash=sha512:38c14d7d02fd857c25831e5989e72fe31b7df99faa058216c1748c4dcc79a2be6f24b1244615691b195fa1d516adba8785fe471483a58db6f6c4e2e72d20eddc \
+    --hash=sha512:f67defed931c0d1d0b3480c3b11a49e9ec7a8db4770ec5b31f1b44541ecadb4737c7d62958b82dd8a2fa34e45c0d9fbc739db04a51de8a7e52f4dd7910700173 \
+    --hash=sha512:5b65d3aa926ef03a84949901fab2b2385b790f8f0ce7855b32bc6e9600486cb33cddf8f127baf29b4abfac3eb1f806fe8224ab09a4a40c6f5374bf5d62d20fa2 \
+    --hash=sha512:e2afae7192ce99656f7550a38a036130e19ad5de107a8495cb91458843cf9ae6d013f5bc7d3435074105716ad22bc96fe256ae470e34b8fc5992274bcc10f376 \
+    --hash=sha512:4485298f4faedd48750d5a3a8c9b0c52fdee90e51ca84f1755b229ae8b6f40590d938f95193958d5c77a7c0e399e896f8db6fab57ed6697ea4e5e791535e4b70
+pexpect==4.4.0 \
+    --hash=sha512:eb546b2c02aeb727ccf633a3776a69046854f12a44df954814085a3bde3af4d87e95b8ae4f5fc21dd55d8413049c9f4972ef18fd90b535971eff193194e5716f \
+    --hash=sha512:c3ac018b0f55075ab2bb7f07d672b5c1ee2823f43577c93dedd8f828f6f31e5270afe56b2cee95cf5626f137978a5f0a7145ab4eb74bbad4818a42e6b329db6e
 ptyprocess==0.5.2 \
     --hash=sha512:fead464aa93e099300f49e6e4742fb4234c15a1ac7d842e93acedfc011a2d3eaf913bdb2a89dd559bed09eed0fc35aad911f350123d7663aaa740822cdfa67e2 \
     --hash=sha512:cb4e70855d388a6ff691e2a244c072a5a50cf39cdf727e3a4218817bf5ac722c4b49f0dbfd80204259998eba137492690759b8908bfea925842b9f7fc83ee553
 python-dateutil==2.6.1 \
     --hash=sha512:f16dd29fc975629f594dd2683a525e2a86acb020bf8962558d19040b14ac6f19d4ab07a910d6bb55c9db3cc02b5472774a3a05ccc86cf624ca5e5144463646db \
     --hash=sha512:1eb4fc12d30a21631cd5c86be87f3293e5132d668f9f24d36fd0056030cb2001b0851fb4a46218fa40ad95ebf35f9d6622bcf84080593adf417b2b7554850283
 python-gnupg==0.4.1 \
@@ -109,21 +118,21 @@
     --hash=sha512:887573b59e63b839f15a55d466405696d9715a61d95b2f3eb1ad96189a169fbd8d847761fe3050be1ae88da63011304e4774a34a3e460898fe72ae570fe6444b
 urllib3==1.22 \
     --hash=sha512:b46a3b5622ab36348f2740d69ca1f2b82fa62623ea426ae6c09a58e136e79cf0ddcf4a7338b80a760dc9516a30f7ad5ad7612324917beb8d036df9f0b7233005 \
     --hash=sha512:132b69d7f390916bdcde66d46fbf0189d0c1f976f91778dcb0a9ef8174487b7bb4b37b9139e84f7c70234803be95284448aba0b820f3b54530c0c497ca7a1dc9
 virtualenv==15.1.0 \
     --hash=sha512:9988af801d9ad15c3f9831489ee9b49b54388e8349be201e7f7db3f2f1e59d033d3117f12e2f1909d65f052c5f1eacd87a894c6f7f703d770add3a0179e95863 \
     --hash=sha512:d7e95b8c017ec076210f30b6fd4bb44be2f7dc0257492c25bb00fee597d3ade34226d03539180f1edaf2d27b361f8efdabb92d3476e13785b890878ee1295cb2
-yarl==1.0.0 \
-    --hash=sha512:d183f42725223b5858412bee7845b084888420621c5f180ffdbeeffd7a84b1dede0c699156f8bbac7a4bbce855634779d7e636dc0bb59fbdbbd84c3cecdc4146 \
-    --hash=sha512:387eedd2be9187f07d2bf06489db0371c46b316c10bbb4fb4661a01954ad18466dee9570680ce11949eccfdb8351cc2e072b22f928eab1ed26170f5c620669ac \
-    --hash=sha512:dc6d430f98209658b134ab38061e4aa7413f7ee0ec91c2eb01bfb2066bfdaa5f81a86b1fdce185f45545a89a534a3899213d2788345cabdcba0311a42a69c19c \
-    --hash=sha512:887f0bb28bffc9b209609253b512f58ee092a490847f09aa37e71f17a172ff79e0cb39cddb3222ad2e94101a523fce977543829eefa884a56f7ab30528c582fa \
-    --hash=sha512:c92016c962ad079f70c08d9c630d4d82a0191d1cc26e6cbcc23995ad2ac33ac1e2003fc3c62e975772bad11d394917f58ad4e699f3cfeb04f1df98164efd191b \
-    --hash=sha512:bd88b56359655d098024fe42f631458ae2f5fe3e8c2aa8ab5b2a73c3e152e5f13dee32de351b5e07b7339cefe9fe0f93cfa782cad92aa5c95a07c92789337cc2 \
-    --hash=sha512:c7a45c94400d478382461ab934012c689f2335908e73a621bd591869db78379bf273355c9a565874d8369316cfdf156d97921c3ab4b2f57e60fb1762f4459c4b \
-    --hash=sha512:fbddbd5d56d0abad05457b3ecd147360f47be0ddb11c93d7eff7c48323640921de44228cb8083c530b9dafad965a24044d439e9ed8b1aeec74a07707c429d7eb \
-    --hash=sha512:79e8268c81e51bab06a6c840347a19944f5264d7a59e2484dbddd539e0520ee7d86b7dc4d852be98a8070898758d969961abaaae7260ccdb6e2a9382b559bd1f \
-    --hash=sha512:d88f4660679af4798a28574383864af8b5106eb87747ebefb11f1dd3de3ddc335c00f7689850ede975e74b25e235f7e17903d69c19b9176ac8d3a656ef1f6817 \
-    --hash=sha512:9ff3d45a713f8323f427e9a8a6785a50d82a72d19585634ad38a13a39dce4596f5c1a16404cf86ecd24bcefdbc6081f02d2e34bb2c050ae75875cfe5fc552183 \
-    --hash=sha512:08ad737e0570c8a7417e8f9ab061e8d1ce38810e39b4b335e9df7bd3d3fd9e5a9ef4867170be99212aa6ff4f48bdf38448c9b13b61e5d80f7db164f9022fd280 \
-    --hash=sha512:7da760b6c51d8f19fc2602285de24c3a9cce64d21fe957f3ae5c80ca2d89a7e9bcb6682b8a060cf11cf398e6c01d9395e9ca07a5f2bc0a6b24ce5307564dae19
+yarl==1.1.1 \
+    --hash=sha512:e7923405d70e1444a9a6b4aea8bc22e73375badcb1f4d2202ce4b00062c9da8b8b4fad520c5274b4d682422aa0f8cae4f3b64a4773cf9ed959c431f13f267b71 \
+    --hash=sha512:9e1cb76cea335038143b2cc701d1132ee100b02b5ee1dae2303038dae0da2bbb74e135052d451f14825ba3542e2bdc050ffbd292f7d12819e953cd26d6c30efd \
+    --hash=sha512:12d9608fbad83ec49c2eaa1cff376d4bcccfe5a0a87075402a17e19756a7cf22cf9fa16d9ee48bc663c70a8e8c4b904445253703105c53d4d346076b76e13d1d \
+    --hash=sha512:19baea347f0501374e077c6218fa54cc262f266d2a827411b1f718f7f5155d8440fc2e7096b47e92f1aa4abf864a5114a8e80be553517e365b5ed89a037a953c \
+    --hash=sha512:5f3879c4afc140de3c7619dcdb780a2ae26ef96e032b9f6c0aad259b35775b5a9f3ccfde851c6c45bf94114ceb7b4948bddf4c03ce1393cf867baad662a0e06e \
+    --hash=sha512:6e52236596d1c8b7e19d5781deb4d9f3ece4f2de79b641359d0e3b2042de0d3ec67a7bdf748e013b32fb60d72e7c75c39998299b8a2de0bbaa75792611fb9f79 \
+    --hash=sha512:347f9d71e805d5ae8fcff4d4d0040f6ca7297126a3a9d58abc3e54a3b8afd6522c789fb24fc26761285bb4647917378620abe72b713994db65e64d8bfcb158b4 \
+    --hash=sha512:303eb2c4e918169b21494b39a8f6efb1e08878725a5893b2234ff76f058378caea2870787f7cd059bc2cc4e4aa8261a738bf29aeef64ed355e69c5236743076e \
+    --hash=sha512:8ecf10cb982e444a7dc076053f7e6bac5e85234d16a09602da23f5e8ad94586dc89877088121661934a01152f79aaeb560bd0ac6aa38cfbba309116053e04ff0 \
+    --hash=sha512:dd047052f142c854a73384eeeeff6a28af5302532b48da74359f398ec09da298c34e064565273bdcad3ec6e4cf8d3da258624b6721a19f9f5552b07bb17f5e01 \
+    --hash=sha512:ccdc805986d37dcafcede47d1f40a8855e8e7b3afd810a5bd3c6b769db88f8360237f04ec882bcd4c7e821c9817e15662080c318c81167c127ddc772217f3c97 \
+    --hash=sha512:8646d48c3c4a0fbd785111cf7c222fb249e865493b288227dd179b74572ef3ac4f487a74c40797adfd7c64eaff0fd2572eda92b0f90e43c737f0cf19aceb15a4 \
+    --hash=sha512:fe53e24401e91994d04fd7274200f92168bb08d78c460b49e800646a3e4611f6baefca4ede5b2b6727f2e6e4cd51296ca834305c0e2fb377ac3a928463f995cd
```

### Comparing `scriptworker-8.1.1/CONTRIBUTING.rst` & `scriptworker-9.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/LICENSE` & `scriptworker-9.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/docker/Dockerfile.gnupg` & `scriptworker-9.0.0/docker/Dockerfile.gnupg`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/docker/gnupg.yaml` & `scriptworker-9.0.0/docker/gnupg.yaml`

 * *Files identical despite different names*

### Comparing `scriptworker-8.1.1/README.rst` & `scriptworker-9.0.0/README.rst`

 * *Files identical despite different names*

