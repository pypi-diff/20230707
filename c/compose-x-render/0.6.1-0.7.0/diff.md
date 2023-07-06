# Comparing `tmp/compose_x_render-0.6.1.tar.gz` & `tmp/compose_x_render-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compose_x_render-0.6.1.tar", max compression
+gzip compressed data, was "compose_x_render-0.7.0.tar", max compression
```

## Comparing `compose_x_render-0.6.1.tar` & `compose_x_render-0.7.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0    16725 2022-03-14 15:39:11.439179 compose_x_render-0.6.1/LICENSE
--rw-r--r--   0        0        0      304 2022-03-14 15:39:11.439179 compose_x_render-0.6.1/MANIFEST.in
--rw-r--r--   0        0        0      220 2022-11-02 19:01:30.104964 compose_x_render-0.6.1/compose_x_render/__init__.py
--rw-r--r--   0        0        0     1890 2022-10-10 10:25:38.369629 compose_x_render-0.6.1/compose_x_render/cli.py
--rw-r--r--   0        0        0    26292 2022-11-02 19:01:30.378960 compose_x_render-0.6.1/compose_x_render/compose-spec.json
--rw-r--r--   0        0        0    12366 2022-11-02 18:50:53.487351 compose_x_render-0.6.1/compose_x_render/compose_x_render.py
--rw-r--r--   0        0        0      256 2022-10-10 10:25:38.482628 compose_x_render-0.6.1/compose_x_render/consts.py
--rw-r--r--   0        0        0     1669 2022-10-10 10:25:38.332630 compose_x_render-0.6.1/compose_x_render/envsubst.py
--rw-r--r--   0        0        0     2613 2022-11-02 18:49:19.698596 compose_x_render-0.6.1/compose_x_render/list_management.py
--rw-r--r--   0        0        0     3572 2022-10-10 10:25:38.365630 compose_x_render-0.6.1/compose_x_render/networking.py
--rw-r--r--   0        0        0     2493 2022-11-02 19:01:30.104964 compose_x_render-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 compose_x_render-0.6.1/setup.py
--rw-r--r--   0        0        0     1442 1970-01-01 00:00:00.000000 compose_x_render-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    16725 2022-03-14 15:39:11.439179 compose_x_render-0.7.0/LICENSE
+-rw-r--r--   0        0        0      304 2022-03-14 15:39:11.439179 compose_x_render-0.7.0/MANIFEST.in
+-rw-r--r--   0        0        0      220 2023-07-06 23:27:30.124557 compose_x_render-0.7.0/compose_x_render/__init__.py
+-rw-r--r--   0        0        0     1890 2022-10-10 10:25:38.369629 compose_x_render-0.7.0/compose_x_render/cli.py
+-rw-r--r--   0        0        0    27379 2023-07-06 23:27:30.716563 compose_x_render-0.7.0/compose_x_render/compose-spec.json
+-rw-r--r--   0        0        0    12390 2023-07-06 22:53:59.841920 compose_x_render-0.7.0/compose_x_render/compose_x_render.py
+-rw-r--r--   0        0        0      256 2022-10-10 10:25:38.482628 compose_x_render-0.7.0/compose_x_render/consts.py
+-rw-r--r--   0        0        0     1669 2022-10-10 10:25:38.332630 compose_x_render-0.7.0/compose_x_render/envsubst.py
+-rw-r--r--   0        0        0     2613 2022-11-02 18:49:19.698596 compose_x_render-0.7.0/compose_x_render/list_management.py
+-rw-r--r--   0        0        0     3571 2023-07-06 23:27:30.678563 compose_x_render-0.7.0/compose_x_render/networking.py
+-rw-r--r--   0        0        0     2389 2023-07-06 23:27:30.124557 compose_x_render-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1136 1970-01-01 00:00:00.000000 compose_x_render-0.7.0/PKG-INFO
```

### Comparing `compose_x_render-0.6.1/LICENSE` & `compose_x_render-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `compose_x_render-0.6.1/compose_x_render/cli.py` & `compose_x_render-0.7.0/compose_x_render/cli.py`

 * *Files identical despite different names*

### Comparing `compose_x_render-0.6.1/compose_x_render/compose-spec.json` & `compose_x_render-0.7.0/compose_x_render/compose-spec.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9270528742261759%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2019-09/schema#'",*

 * * "'definitions'": "{'service': {'properties': {'build': {'oneOf': {1: {'properties': "*

 * *                  "{'dockerfile_inline': OrderedDict([('type', 'string')]), 'no_cache': "*

 * *                  "OrderedDict([('type', 'boolean')]), 'additional_contexts': "*

 * *                  "OrderedDict([('$ref', '#/definitions/list_or_dict')]), 'pull': "*

 * *                  "OrderedDict([('type', 'boolean')]), 'privileged': OrderedDict([('type', "*

 * *              […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "$schema": "http://json-schema.org/draft/2019-09/schema#",
+    "$schema": "https://json-schema.org/draft/2019-09/schema#",
     "additionalProperties": false,
     "definitions": {
         "blkio_limit": {
             "additionalProperties": false,
             "properties": {
                 "path": {
                     "type": "string"
@@ -25,14 +25,30 @@
                 },
                 "weight": {
                     "type": "integer"
                 }
             },
             "type": "object"
         },
+        "command": {
+            "oneOf": [
+                {
+                    "type": "null"
+                },
+                {
+                    "type": "string"
+                },
+                {
+                    "items": {
+                        "type": "string"
+                    },
+                    "type": "array"
+                }
+            ]
+        },
         "config": {
             "additionalProperties": false,
             "id": "#/definitions/config",
             "patternProperties": {
                 "^x-": {}
             },
             "properties": {
@@ -384,14 +400,37 @@
                 "timeout": {
                     "format": "duration",
                     "type": "string"
                 }
             },
             "type": "object"
         },
+        "include": {
+            "id": "#/definitions/include",
+            "oneOf": [
+                {
+                    "type": "string"
+                },
+                {
+                    "additionalProperties": false,
+                    "properties": {
+                        "env_file": {
+                            "$ref": "#/definitions/string_or_list"
+                        },
+                        "path": {
+                            "$ref": "#/definitions/string_or_list"
+                        },
+                        "project_directory": {
+                            "type": "string"
+                        }
+                    },
+                    "type": "object"
+                }
+            ]
+        },
         "list_of_strings": {
             "items": {
                 "type": "string"
             },
             "type": "array",
             "uniqueItems": true
         },
@@ -547,14 +586,17 @@
                                 "string",
                                 "number"
                             ]
                         }
                     },
                     "type": "object"
                 },
+                "environment": {
+                    "type": "string"
+                },
                 "external": {
                     "properties": {
                         "name": {
                             "type": "string"
                         }
                     },
                     "type": [
@@ -580,14 +622,20 @@
         "service": {
             "additionalProperties": false,
             "id": "#/definitions/service",
             "patternProperties": {
                 "^x-": {}
             },
             "properties": {
+                "annotations": {
+                    "$ref": "#/definitions/list_or_dict"
+                },
+                "attach": {
+                    "type": "boolean"
+                },
                 "blkio_config": {
                     "additionalProperties": false,
                     "properties": {
                         "device_read_bps": {
                             "items": {
                                 "$ref": "#/definitions/blkio_limit"
                             },
@@ -630,14 +678,17 @@
                         },
                         {
                             "additionalProperties": false,
                             "patternProperties": {
                                 "^x-": {}
                             },
                             "properties": {
+                                "additional_contexts": {
+                                    "$ref": "#/definitions/list_or_dict"
+                                },
                                 "args": {
                                     "$ref": "#/definitions/list_or_dict"
                                 },
                                 "cache_from": {
                                     "items": {
                                         "type": "string"
                                     },
@@ -651,35 +702,62 @@
                                 },
                                 "context": {
                                     "type": "string"
                                 },
                                 "dockerfile": {
                                     "type": "string"
                                 },
+                                "dockerfile_inline": {
+                                    "type": "string"
+                                },
                                 "extra_hosts": {
                                     "$ref": "#/definitions/list_or_dict"
                                 },
                                 "isolation": {
                                     "type": "string"
                                 },
                                 "labels": {
                                     "$ref": "#/definitions/list_or_dict"
                                 },
                                 "network": {
                                     "type": "string"
                                 },
+                                "no_cache": {
+                                    "type": "boolean"
+                                },
+                                "platforms": {
+                                    "items": {
+                                        "type": "string"
+                                    },
+                                    "type": "array"
+                                },
+                                "privileged": {
+                                    "type": "boolean"
+                                },
+                                "pull": {
+                                    "type": "boolean"
+                                },
+                                "secrets": {
+                                    "$ref": "#/definitions/service_config_or_secret"
+                                },
                                 "shm_size": {
                                     "type": [
                                         "integer",
                                         "string"
                                     ]
                                 },
                                 "ssh": {
                                     "$ref": "#/definitions/list_or_dict"
                                 },
+                                "tags": {
+                                    "items": {
+                                        "type": "string"
+                                    },
+                                    "type": "array"
+                                },
                                 "target": {
                                     "type": "string"
                                 }
                             },
                             "type": "object"
                         }
                     ]
@@ -694,63 +772,29 @@
                 "cap_drop": {
                     "items": {
                         "type": "string"
                     },
                     "type": "array",
                     "uniqueItems": true
                 },
+                "cgroup": {
+                    "enum": [
+                        "host",
+                        "private"
+                    ],
+                    "type": "string"
+                },
                 "cgroup_parent": {
                     "type": "string"
                 },
                 "command": {
-                    "oneOf": [
-                        {
-                            "type": "string"
-                        },
-                        {
-                            "items": {
-                                "type": "string"
-                            },
-                            "type": "array"
-                        }
-                    ]
+                    "$ref": "#/definitions/command"
                 },
                 "configs": {
-                    "items": {
-                        "oneOf": [
-                            {
-                                "type": "string"
-                            },
-                            {
-                                "additionalProperties": false,
-                                "patternProperties": {
-                                    "^x-": {}
-                                },
-                                "properties": {
-                                    "gid": {
-                                        "type": "string"
-                                    },
-                                    "mode": {
-                                        "type": "number"
-                                    },
-                                    "source": {
-                                        "type": "string"
-                                    },
-                                    "target": {
-                                        "type": "string"
-                                    },
-                                    "uid": {
-                                        "type": "string"
-                                    }
-                                },
-                                "type": "object"
-                            }
-                        ]
-                    },
-                    "type": "array"
+                    "$ref": "#/definitions/service_config_or_secret"
                 },
                 "container_name": {
                     "type": "string"
                 },
                 "cpu_count": {
                     "minimum": 0,
                     "type": "integer"
@@ -831,14 +875,21 @@
                                         "condition": {
                                             "enum": [
                                                 "service_started",
                                                 "service_healthy",
                                                 "service_completed_successfully"
                                             ],
                                             "type": "string"
+                                        },
+                                        "required": {
+                                            "default": true,
+                                            "type": "boolean"
+                                        },
+                                        "restart": {
+                                            "type": "boolean"
                                         }
                                     },
                                     "required": [
                                         "condition"
                                     ],
                                     "type": "object"
                                 }
@@ -873,25 +924,15 @@
                 "dns_search": {
                     "$ref": "#/definitions/string_or_list"
                 },
                 "domainname": {
                     "type": "string"
                 },
                 "entrypoint": {
-                    "oneOf": [
-                        {
-                            "type": "string"
-                        },
-                        {
-                            "items": {
-                                "type": "string"
-                            },
-                            "type": "array"
-                        }
-                    ]
+                    "$ref": "#/definitions/command"
                 },
                 "env_file": {
                     "$ref": "#/definitions/string_or_list"
                 },
                 "environment": {
                     "$ref": "#/definitions/list_or_dict"
                 },
@@ -1162,46 +1203,15 @@
                 "runtime": {
                     "type": "string"
                 },
                 "scale": {
                     "type": "integer"
                 },
                 "secrets": {
-                    "items": {
-                        "oneOf": [
-                            {
-                                "type": "string"
-                            },
-                            {
-                                "additionalProperties": false,
-                                "patternProperties": {
-                                    "^x-": {}
-                                },
-                                "properties": {
-                                    "gid": {
-                                        "type": "string"
-                                    },
-                                    "mode": {
-                                        "type": "number"
-                                    },
-                                    "source": {
-                                        "type": "string"
-                                    },
-                                    "target": {
-                                        "type": "string"
-                                    },
-                                    "uid": {
-                                        "type": "string"
-                                    }
-                                },
-                                "type": "object"
-                            }
-                        ]
-                    },
-                    "type": "array"
+                    "$ref": "#/definitions/service_config_or_secret"
                 },
                 "security_opt": {
                     "items": {
                         "type": "string"
                     },
                     "type": "array",
                     "uniqueItems": true
@@ -1267,14 +1277,17 @@
                 },
                 "user": {
                     "type": "string"
                 },
                 "userns_mode": {
                     "type": "string"
                 },
+                "uts": {
+                    "type": "string"
+                },
                 "volumes": {
                     "items": {
                         "oneOf": [
                             {
                                 "type": "string"
                             },
                             {
@@ -1319,14 +1332,17 @@
                                     },
                                     "tmpfs": {
                                         "additionalProperties": false,
                                         "patternProperties": {
                                             "^x-": {}
                                         },
                                         "properties": {
+                                            "mode": {
+                                                "type": "number"
+                                            },
                                             "size": {
                                                 "oneOf": [
                                                     {
                                                         "minimum": 0,
                                                         "type": "integer"
                                                     },
                                                     {
@@ -1372,14 +1388,48 @@
                 },
                 "working_dir": {
                     "type": "string"
                 }
             },
             "type": "object"
         },
+        "service_config_or_secret": {
+            "items": {
+                "oneOf": [
+                    {
+                        "type": "string"
+                    },
+                    {
+                        "additionalProperties": false,
+                        "patternProperties": {
+                            "^x-": {}
+                        },
+                        "properties": {
+                            "gid": {
+                                "type": "string"
+                            },
+                            "mode": {
+                                "type": "number"
+                            },
+                            "source": {
+                                "type": "string"
+                            },
+                            "target": {
+                                "type": "string"
+                            },
+                            "uid": {
+                                "type": "string"
+                            }
+                        },
+                        "type": "object"
+                    }
+                ]
+            },
+            "type": "array"
+        },
         "string_or_list": {
             "oneOf": [
                 {
                     "type": "string"
                 },
                 {
                     "$ref": "#/definitions/list_of_strings"
@@ -1448,16 +1498,25 @@
             "patternProperties": {
                 "^[a-zA-Z0-9._-]+$": {
                     "$ref": "#/definitions/config"
                 }
             },
             "type": "object"
         },
+        "include": {
+            "description": "compose sub-projects to be included.",
+            "items": {
+                "$ref": "#/definitions/include",
+                "type": "object"
+            },
+            "type": "array"
+        },
         "name": {
             "description": "define the Compose project name, until user defines one explicitly.",
+            "pattern": "^[a-z0-9][a-z0-9_-]*$",
             "type": "string"
         },
         "networks": {
             "id": "#/properties/networks",
             "patternProperties": {
                 "^[a-zA-Z0-9._-]+$": {
                     "$ref": "#/definitions/network"
```

### Comparing `compose_x_render-0.6.1/compose_x_render/compose_x_render.py` & `compose_x_render-0.7.0/compose_x_render/compose_x_render.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,15 @@
 
 
 def load_compose_file(file_path) -> Union[dict, list]:
     """
     Read docker compose file content and load with YAML
     """
     with open(file_path) as composex_fd:
-        return yaml.load(composex_fd.read(), Loader=Loader)
+        return json.loads(json.dumps(yaml.load(composex_fd.read(), Loader=Loader)))
 
 
 def merge_definitions(
     original_def: dict, override_def: dict, nested: bool = False
 ) -> dict:
     """
     Merges resources and non services definitions together.
```

### Comparing `compose_x_render-0.6.1/compose_x_render/envsubst.py` & `compose_x_render-0.7.0/compose_x_render/envsubst.py`

 * *Files identical despite different names*

### Comparing `compose_x_render-0.6.1/compose_x_render/list_management.py` & `compose_x_render-0.7.0/compose_x_render/list_management.py`

 * *Files identical despite different names*

### Comparing `compose_x_render-0.6.1/compose_x_render/networking.py` & `compose_x_render-0.7.0/compose_x_render/networking.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,14 @@
         service_ports.append(new_port)
     elif service_ports and not keyisset("published", new_port):
         if new_port["target"] not in [
             _port["target"] for _port in same_protocol_target_not_published_ports
         ]:
             service_ports.append(new_port)
     elif service_ports and keyisset("published", new_port):
-
         if new_port["published"] not in [
             _port["published"] for _port in same_protocol_published_ports
         ]:
             service_ports.append(new_port)
         elif new_port["published"] in [
             _port["published"] for _port in same_protocol_published_ports
         ]:
```

### Comparing `compose_x_render-0.6.1/pyproject.toml` & `compose_x_render-0.7.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,68 +1,65 @@
 [tool.poetry]
 name = "compose_x_render"
-version = "0.6.1"
+version = "0.7.0"
 description = "Library & Tool to compile/merge compose files with top level extension fields"
 authors = ["John Preston <john@compose-x.io>"]
 license = "MPL-2.0"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
     "Intended Audience :: System Administrators",
     "Intended Audience :: Information Technology",
     "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 keywords = ["compose-x", "aws", "jsonschema", "docker", "compose-spec"]
 include = [
     "MANIFEST.in",
     "LICENSE",
     "compose_x_render/compose-spec.json"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
-PyYAML = ">=5.4.1.0,<7.0"
+python = "^3.8"
+PyYAML = ">=5,<7.0"
 argparse = "^1.4.0"
 compose-x-common = "^1.2"
-jsonschema = ">=3.2.0,<5.0"
+jsonschema = ">=4.15,<5.0"
 importlib-resources = "^5.4.0"
 
 [tool.poetry.extras]
 aws = ["boto3"]
 
 [tool.poetry.dev-dependencies]
-sphinx-material = "^0.0.34"
-isort = "^5.10.1"
-black = "^22.3"
+sphinx-material = "^0.0.35"
+isort = "^5.10"
+black = "^23.3"
 Sphinx = "^4.4.0"
 tbump = "^6.7.0"
-pre-commit = "^2.17.0"
+pre-commit = "^3.3"
 behave = "^1.2.6"
-coverage = "^5.5"
-flake8 = "^3.9.2"
-tox = "^3.24.5"
-pytest = "^6.2.5"
-twine = "^3.7.1"
-pyupgrade = "^3.0.0"
+coverage = "^7.2"
+pytest = "^7.4"
+twine = "^4.0"
+pyupgrade = "^3.8"
 
 [tool.poetry.scripts]
 compose-x-render = "compose_x_render.cli:main"
 ecs-compose-x-render = "compose_x_render.cli:main"
 
 [tool.tbump]
 github_url = "https://github.com/compose-x/compose_x_render"
 
 [tool.tbump.version]
-current = "0.6.1"
+current = "0.7.0"
 
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
@@ -102,9 +99,9 @@
 source = ["compose_x_render"]
 omit = ["compose_x_render/cli.py"]
 
 [tool.coverage.report]
 show_missing = true
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `compose_x_render-0.6.1/PKG-INFO` & `compose_x_render-0.7.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,27 @@
 Metadata-Version: 2.1
 Name: compose-x-render
-Version: 0.6.1
+Version: 0.7.0
 Summary: Library & Tool to compile/merge compose files with top level extension fields
 License: MPL-2.0
 Keywords: compose-x,aws,jsonschema,docker,compose-spec
 Author: John Preston
 Author-email: john@compose-x.io
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: aws
-Requires-Dist: PyYAML (>=5.4.1.0,<7.0)
+Requires-Dist: PyYAML (>=5,<7.0)
 Requires-Dist: argparse (>=1.4.0,<2.0.0)
 Requires-Dist: compose-x-common (>=1.2,<2.0)
 Requires-Dist: importlib-resources (>=5.4.0,<6.0.0)
-Requires-Dist: jsonschema (>=3.2.0,<5.0)
+Requires-Dist: jsonschema (>=4.15,<5.0)
```

