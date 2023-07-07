# Comparing `tmp/cr_api_client-4.1.0.tar.gz` & `tmp/cr_api_client-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cr_api_client-4.1.0.tar", max compression
+gzip compressed data, was "cr_api_client-4.3.0.tar", max compression
```

## Comparing `cr_api_client-4.1.0.tar` & `cr_api_client-4.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1056 2023-05-30 08:35:39.548784 cr_api_client-4.1.0/LICENSE
--rw-r--r--   0        0        0    11574 2023-05-30 08:35:39.548784 cr_api_client-4.1.0/README.md
--rw-r--r--   0        0        0      746 2023-05-30 08:35:39.548784 cr_api_client-4.1.0/cr_api_client/__init__.py
--rw-r--r--   0        0        0     2161 2023-05-30 08:35:39.548784 cr_api_client-4.1.0/cr_api_client/config.py
--rw-r--r--   0        0        0    96267 2023-05-30 08:35:39.552785 cr_api_client-4.1.0/cr_api_client/core_api.py
--rwxr-xr-x   0        0        0   121386 2023-05-30 08:35:39.552785 cr_api_client-4.1.0/cr_api_client/cyber_range.py
--rw-r--r--   0        0        0    20513 2023-05-30 08:35:39.552785 cr_api_client-4.1.0/cr_api_client/provisioning_api.py
--rw-r--r--   0        0        0     7843 2023-05-30 08:35:39.552785 cr_api_client-4.1.0/cr_api_client/publish_api.py
--rw-r--r--   0        0        0    23935 2023-05-30 08:35:39.552785 cr_api_client-4.1.0/cr_api_client/redteam_api.py
--rw-r--r--   0        0        0     6861 2023-05-30 08:35:39.552785 cr_api_client-4.1.0/cr_api_client/topology/TopologyElements.py
--rw-r--r--   0        0        0    14750 2023-05-30 08:35:39.552785 cr_api_client-4.1.0/cr_api_client/topology/TopologyGenerator.py
--rw-r--r--   0        0        0     2635 2023-05-30 08:35:39.552785 cr_api_client-4.1.0/cr_api_client/topology/TopologyLinksGenerator.py
--rw-r--r--   0        0        0     3328 2023-05-30 08:35:39.552785 cr_api_client-4.1.0/cr_api_client/topology/TopologyNodeGenerator.py
--rw-r--r--   0        0        0     3821 2023-05-30 08:35:39.552785 cr_api_client-4.1.0/cr_api_client/topology/TopologyNodesGenerator.py
--rw-r--r--   0        0        0      346 2023-05-30 08:35:39.552785 cr_api_client-4.1.0/cr_api_client/topology/validator/__init__.py
--rw-r--r--   0        0        0     1429 2023-05-30 08:35:39.552785 cr_api_client-4.1.0/cr_api_client/topology/validator/common.py
--rw-r--r--   0        0        0     1730 2023-05-30 08:35:39.552785 cr_api_client-4.1.0/cr_api_client/topology/validator/link.py
--rw-r--r--   0        0        0     4063 2023-05-30 08:35:39.552785 cr_api_client-4.1.0/cr_api_client/topology/validator/node.py
--rw-r--r--   0        0        0     1360 2023-05-30 08:35:39.552785 cr_api_client-4.1.0/cr_api_client/topology/validator/topology.py
--rw-r--r--   0        0        0    10206 2023-05-30 08:35:39.552785 cr_api_client-4.1.0/cr_api_client/user_activity_api.py
--rw-r--r--   0        0        0     3279 2023-05-30 08:35:39.552785 cr_api_client-4.1.0/cr_api_client/yaml_helper.py
--rw-r--r--   0        0        0     1243 2023-05-30 08:35:39.552785 cr_api_client-4.1.0/pyproject.toml
--rw-r--r--   0        0        0    12658 1970-01-01 00:00:00.000000 cr_api_client-4.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-07-07 06:33:25.125693 cr_api_client-4.3.0/LICENSE
+-rw-r--r--   0        0        0    11574 2023-07-07 06:33:25.125693 cr_api_client-4.3.0/README.md
+-rw-r--r--   0        0        0      746 2023-07-07 06:33:25.125693 cr_api_client-4.3.0/cr_api_client/__init__.py
+-rw-r--r--   0        0        0     2161 2023-07-07 06:33:25.125693 cr_api_client-4.3.0/cr_api_client/config.py
+-rw-r--r--   0        0        0   104435 2023-07-07 06:33:25.125693 cr_api_client-4.3.0/cr_api_client/core_api.py
+-rwxr-xr-x   0        0        0   125124 2023-07-07 06:33:25.125693 cr_api_client-4.3.0/cr_api_client/cyber_range.py
+-rw-r--r--   0        0        0    20513 2023-07-07 06:33:25.125693 cr_api_client-4.3.0/cr_api_client/provisioning_api.py
+-rw-r--r--   0        0        0     7843 2023-07-07 06:33:25.125693 cr_api_client-4.3.0/cr_api_client/publish_api.py
+-rw-r--r--   0        0        0    23923 2023-07-07 06:33:25.125693 cr_api_client-4.3.0/cr_api_client/redteam_api.py
+-rw-r--r--   0        0        0     6861 2023-07-07 06:33:25.125693 cr_api_client-4.3.0/cr_api_client/topology/TopologyElements.py
+-rw-r--r--   0        0        0    14750 2023-07-07 06:33:25.125693 cr_api_client-4.3.0/cr_api_client/topology/TopologyGenerator.py
+-rw-r--r--   0        0        0     2635 2023-07-07 06:33:25.125693 cr_api_client-4.3.0/cr_api_client/topology/TopologyLinksGenerator.py
+-rw-r--r--   0        0        0     3328 2023-07-07 06:33:25.125693 cr_api_client-4.3.0/cr_api_client/topology/TopologyNodeGenerator.py
+-rw-r--r--   0        0        0     3821 2023-07-07 06:33:25.125693 cr_api_client-4.3.0/cr_api_client/topology/TopologyNodesGenerator.py
+-rw-r--r--   0        0        0      346 2023-07-07 06:33:25.125693 cr_api_client-4.3.0/cr_api_client/topology/validator/__init__.py
+-rw-r--r--   0        0        0     1429 2023-07-07 06:33:25.125693 cr_api_client-4.3.0/cr_api_client/topology/validator/common.py
+-rw-r--r--   0        0        0     1730 2023-07-07 06:33:25.125693 cr_api_client-4.3.0/cr_api_client/topology/validator/link.py
+-rw-r--r--   0        0        0     4063 2023-07-07 06:33:25.125693 cr_api_client-4.3.0/cr_api_client/topology/validator/node.py
+-rw-r--r--   0        0        0     1360 2023-07-07 06:33:25.125693 cr_api_client-4.3.0/cr_api_client/topology/validator/topology.py
+-rw-r--r--   0        0        0    10206 2023-07-07 06:33:25.125693 cr_api_client-4.3.0/cr_api_client/user_activity_api.py
+-rw-r--r--   0        0        0     3279 2023-07-07 06:33:25.125693 cr_api_client-4.3.0/cr_api_client/yaml_helper.py
+-rw-r--r--   0        0        0     1347 2023-07-07 06:33:25.125693 cr_api_client-4.3.0/pyproject.toml
+-rw-r--r--   0        0        0    12704 1970-01-01 00:00:00.000000 cr_api_client-4.3.0/PKG-INFO
```

### Comparing `cr_api_client-4.1.0/LICENSE` & `cr_api_client-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cr_api_client-4.1.0/README.md` & `cr_api_client-4.3.0/README.md`

 * *Files identical despite different names*

### Comparing `cr_api_client-4.1.0/cr_api_client/__init__.py` & `cr_api_client-4.3.0/cr_api_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import sys
 import threading
 from pathlib import Path
 
 from loguru import logger
 
 # Component version
-__version__ = "4.1.0"
+__version__ = "4.3.0"
 
 # Get component full version from file generated at build time
 current_file_dir = Path(__file__).resolve().parent
 fullversion_file = Path(current_file_dir, "fullversion.txt")
 if os.path.isfile(fullversion_file):
     __fullversion__ = open(fullversion_file, "r").read().strip()
 else:
```

### Comparing `cr_api_client-4.1.0/cr_api_client/config.py` & `cr_api_client-4.3.0/cr_api_client/config.py`

 * *Files identical despite different names*

### Comparing `cr_api_client-4.1.0/cr_api_client/core_api.py` & `cr_api_client-4.3.0/cr_api_client/core_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1190,4828 +1190,5339 @@
 00004a50: 736f 7572 6365 2066 696c 6573 2e0a 0a20  source files... 
 00004a60: 2020 203a 7265 7475 726e 3a20 4120 7475     :return: A tu
 00004a70: 706c 6520 636f 6e74 6169 6e69 6e67 2074  ple containing t
 00004a80: 6865 2049 4420 6f66 2074 6865 2063 7265  he ID of the cre
 00004a90: 6174 6564 2073 696d 756c 6174 696f 6e2c  ated simulation,
 00004aa0: 2061 6e64 2074 6865 206e 6577 206e 6f64   and the new nod
 00004ab0: 6573 206f 6620 7468 6520 7369 6d75 6c61  es of the simula
-00004ac0: 7469 6f6e 2e0a 2020 2020 3a72 7479 7065  tion..    :rtype
-00004ad0: 3a20 3a63 6c61 7373 3a60 5475 706c 655b  : :class:`Tuple[
-00004ae0: 696e 742c 204c 6973 745b 7374 725d 5d60  int, List[str]]`
-00004af0: 0a0a 2020 2020 3a70 6172 616d 2074 6f70  ..    :param top
-00004b00: 6f6c 6f67 795f 636f 6e74 656e 743a 2041  ology_content: A
-00004b10: 2064 6963 7420 636f 6e74 6169 6e69 6e67   dict containing
-00004b20: 2074 6865 206e 6f64 6573 2061 6e64 206e   the nodes and n
-00004b30: 6574 776f 726b 2074 6f70 6f6c 6f67 7920  etwork topology 
-00004b40: 746f 2063 7265 6174 652e 0a20 2020 203a  to create..    :
-00004b50: 7479 7065 2074 6f70 6f6c 6f67 795f 6669  type topology_fi
-00004b60: 6c65 3a20 3a63 6c61 7373 3a60 6469 6374  le: :class:`dict
-00004b70: 600a 2020 2020 3a70 6172 616d 2074 6f70  `.    :param top
-00004b80: 6f6c 6f67 795f 7265 736f 7572 6365 735f  ology_resources_
-00004b90: 7061 7468 733a 2054 6865 2070 6174 6820  paths: The path 
-00004ba0: 746f 2072 6573 6f75 7263 6573 2074 6861  to resources tha
-00004bb0: 7420 7769 6c6c 2062 6520 7075 7368 6564  t will be pushed
-00004bc0: 2069 6e74 6f20 636f 6d70 6174 6962 6c65   into compatible
-00004bd0: 206e 6f64 6573 2e0a 2020 2020 3a74 7970   nodes..    :typ
-00004be0: 6520 746f 706f 6c6f 6779 5f72 6573 6f75  e topology_resou
-00004bf0: 7263 6573 5f70 6174 6873 3a20 3a63 6c61  rces_paths: :cla
-00004c00: 7373 3a60 6c69 7374 602c 206f 7074 696f  ss:`list`, optio
-00004c10: 6e61 6c0a 0a20 2020 2022 2222 0a0a 2020  nal..    """..  
-00004c20: 2020 6966 2022 6e61 6d65 2220 6e6f 7420    if "name" not 
-00004c30: 696e 2074 6f70 6f6c 6f67 795f 636f 6e74  in topology_cont
-00004c40: 656e 743a 0a20 2020 2020 2020 206e 616d  ent:.        nam
-00004c50: 6520 3d20 2254 6f70 6f6c 6f67 7922 0a20  e = "Topology". 
-00004c60: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00004c70: 206e 616d 6520 3d20 746f 706f 6c6f 6779   name = topology
-00004c80: 5f63 6f6e 7465 6e74 5b22 6e61 6d65 225d  _content["name"]
-00004c90: 0a0a 2020 2020 6966 2022 6e6f 6465 7322  ..    if "nodes"
-00004ca0: 206e 6f74 2069 6e20 746f 706f 6c6f 6779   not in topology
-00004cb0: 5f63 6f6e 7465 6e74 3a0a 2020 2020 2020  _content:.      
-00004cc0: 2020 7261 6973 6520 4578 6365 7074 696f    raise Exceptio
-00004cd0: 6e28 0a20 2020 2020 2020 2020 2020 2022  n(.            "
-00004ce0: 5468 6572 6520 7368 6f75 6c64 2062 6520  There should be 
-00004cf0: 6120 276e 6f64 6573 2720 7374 7275 6374  a 'nodes' struct
-00004d00: 7572 6520 696e 2074 6865 2059 414d 4c20  ure in the YAML 
-00004d10: 636f 6e66 6967 7572 6174 696f 6e20 6669  configuration fi
-00004d20: 6c65 220a 2020 2020 2020 2020 290a 0a20  le".        ).. 
-00004d30: 2020 2069 6620 226c 696e 6b73 2220 6e6f     if "links" no
-00004d40: 7420 696e 2074 6f70 6f6c 6f67 795f 636f  t in topology_co
-00004d50: 6e74 656e 743a 0a20 2020 2020 2020 2072  ntent:.        r
-00004d60: 6169 7365 2045 7863 6570 7469 6f6e 280a  aise Exception(.
-00004d70: 2020 2020 2020 2020 2020 2020 2254 6865              "The
-00004d80: 7265 2073 686f 756c 6420 6265 2061 2027  re should be a '
-00004d90: 6c69 6e6b 7327 2073 7472 7563 7475 7265  links' structure
-00004da0: 2069 6e20 7468 6520 5941 4d4c 2063 6f6e   in the YAML con
-00004db0: 6669 6775 7261 7469 6f6e 2066 696c 6522  figuration file"
-00004dc0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-00004dd0: 7265 7175 6972 6564 203d 205b 2273 7769  required = ["swi
-00004de0: 7463 6822 2c20 226e 6f64 6522 2c20 2270  tch", "node", "p
-00004df0: 6172 616d 7322 5d0a 2020 2020 666f 7220  arams"].    for 
-00004e00: 6c69 6e6b 2069 6e20 746f 706f 6c6f 6779  link in topology
-00004e10: 5f63 6f6e 7465 6e74 5b22 6c69 6e6b 7322  _content["links"
-00004e20: 5d3a 0a20 2020 2020 2020 2066 6f72 2072  ]:.        for r
-00004e30: 6571 2069 6e20 7265 7175 6972 6564 3a0a  eq in required:.
-00004e40: 2020 2020 2020 2020 2020 2020 6966 2072              if r
-00004e50: 6571 206e 6f74 2069 6e20 6c69 6e6b 3a0a  eq not in link:.
-00004e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e70: 7261 6973 6520 4578 6365 7074 696f 6e28  raise Exception(
-00004e80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004e90: 2020 2020 2066 2254 6865 7265 2073 686f       f"There sho
-00004ea0: 756c 6420 6265 2061 2027 7b72 6571 7d27  uld be a '{req}'
-00004eb0: 2070 6172 616d 6574 6572 2066 6f72 2065   parameter for e
-00004ec0: 7665 7279 2069 7465 6d20 6f66 2027 6c69  very item of 'li
-00004ed0: 6e6b 7327 2069 6e20 7468 6520 5941 4d4c  nks' in the YAML
-00004ee0: 2063 6f6e 6669 6775 7261 7469 6f6e 2066   configuration f
-00004ef0: 696c 6522 0a20 2020 2020 2020 2020 2020  ile".           
-00004f00: 2020 2020 2029 0a0a 2020 2020 5f73 696d       )..    _sim
-00004f10: 755f 6372 6561 7465 5f61 6464 5f69 6d70  u_create_add_imp
-00004f20: 6c69 6369 745f 746f 706f 5f70 6172 616d  licit_topo_param
-00004f30: 6574 6572 7328 746f 706f 6c6f 6779 5f63  eters(topology_c
-00004f40: 6f6e 7465 6e74 290a 0a20 2020 2073 696d  ontent)..    sim
-00004f50: 756c 6174 696f 6e5f 6469 6374 203d 207b  ulation_dict = {
-00004f60: 226e 616d 6522 3a20 6e61 6d65 2c20 226e  "name": name, "n
-00004f70: 6574 776f 726b 223a 2074 6f70 6f6c 6f67  etwork": topolog
-00004f80: 795f 636f 6e74 656e 742c 2022 7265 736f  y_content, "reso
-00004f90: 7572 6365 735f 7061 7468 7322 3a20 5b5d  urces_paths": []
-00004fa0: 7d0a 0a20 2020 2023 204e 6f72 6d61 6c69  }..    # Normali
-00004fb0: 7a65 2074 6865 2072 6573 6f75 7263 6573  ze the resources
-00004fc0: 2070 6174 6873 0a20 2020 2074 6f70 6f6c   paths.    topol
-00004fd0: 6f67 795f 7265 736f 7572 6365 735f 7061  ogy_resources_pa
-00004fe0: 7468 7320 3d20 5f6e 6f72 6d61 6c69 7a65  ths = _normalize
-00004ff0: 5f73 696d 756c 6174 696f 6e5f 7265 736f  _simulation_reso
-00005000: 7572 6365 5f70 6174 6873 280a 2020 2020  urce_paths(.    
-00005010: 2020 2020 746f 706f 6c6f 6779 5f72 6573      topology_res
-00005020: 6f75 7263 6573 5f70 6174 6873 0a20 2020  ources_paths.   
-00005030: 2029 0a0a 2020 2020 2320 5665 7269 6679   )..    # Verify
-00005040: 2074 6861 7420 7765 2064 6f20 6e6f 7420   that we do not 
-00005050: 6861 7665 2074 6865 2073 616d 6520 7265  have the same re
-00005060: 736f 7572 6365 7320 7061 7468 2069 6e20  sources path in 
-00005070: 7468 6520 6c69 7374 0a20 2020 2069 6620  the list.    if 
-00005080: 6c65 6e28 7365 7428 746f 706f 6c6f 6779  len(set(topology
-00005090: 5f72 6573 6f75 7263 6573 5f70 6174 6873  _resources_paths
-000050a0: 2929 2021 3d20 6c65 6e28 746f 706f 6c6f  )) != len(topolo
-000050b0: 6779 5f72 6573 6f75 7263 6573 5f70 6174  gy_resources_pat
-000050c0: 6873 293a 0a20 2020 2020 2020 2072 6169  hs):.        rai
-000050d0: 7365 2045 7863 6570 7469 6f6e 2822 4964  se Exception("Id
-000050e0: 656e 7469 6361 6c20 7265 736f 7572 6365  entical resource
-000050f0: 7320 7061 7468 7320 6861 7665 2062 6565  s paths have bee
-00005100: 6e20 6769 7665 6e22 290a 0a20 2020 2066  n given")..    f
-00005110: 6f72 2072 6573 6f75 7263 6520 696e 2074  or resource in t
-00005120: 6f70 6f6c 6f67 795f 7265 736f 7572 6365  opology_resource
-00005130: 735f 7061 7468 733a 0a20 2020 2020 2020  s_paths:.       
-00005140: 2023 2056 616c 6964 6174 6520 7265 736f   # Validate reso
-00005150: 7572 6365 7320 7061 7468 0a20 2020 2020  urces path.     
-00005160: 2020 205f 5f76 616c 6964 6174 655f 7265     __validate_re
-00005170: 736f 7572 6365 735f 7061 7468 2872 6573  sources_path(res
-00005180: 6f75 7263 6529 2020 2320 7261 6973 6520  ource)  # raise 
-00005190: 616e 2065 7863 6570 7469 6f6e 2069 6620  an exception if 
-000051a0: 696e 7661 6c69 640a 2020 2020 2020 2020  invalid.        
-000051b0: 2320 7461 6b65 2074 6865 2061 6273 6f6c  # take the absol
-000051c0: 7574 6520 7061 7468 0a20 2020 2020 2020  ute path.       
-000051d0: 2073 696d 756c 6174 696f 6e5f 6469 6374   simulation_dict
-000051e0: 5b22 7265 736f 7572 6365 735f 7061 7468  ["resources_path
-000051f0: 7322 5d2e 6170 7065 6e64 286f 732e 7061  s"].append(os.pa
-00005200: 7468 2e61 6273 7061 7468 2872 6573 6f75  th.abspath(resou
-00005210: 7263 6529 290a 0a20 2020 2072 6574 7572  rce))..    retur
-00005220: 6e20 7369 6d75 6c61 7469 6f6e 5f64 6963  n simulation_dic
-00005230: 740a 0a0a 2320 2d2d 2d2d 2d2d 2d2d 2d2d  t...# ----------
-00005240: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005250: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005260: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005270: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005280: 2023 0a23 2041 5049 2068 656c 7065 7273   #.# API helpers
-00005290: 0a23 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .# -------------
-000052a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000052b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000052c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000052d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 230a  ------------- #.
-000052e0: 0a0a 2323 230a 2320 5369 6d75 6c61 7469  ..###.# Simulati
-000052f0: 6f6e 2068 656c 7065 7273 0a23 2323 0a0a  on helpers.###..
-00005300: 0a64 6566 2063 7265 6174 655f 7369 6d75  .def create_simu
-00005310: 6c61 7469 6f6e 280a 2020 2020 746f 706f  lation(.    topo
-00005320: 6c6f 6779 5f63 6f6e 7465 6e74 3a20 4469  logy_content: Di
-00005330: 6374 5b73 7472 2c20 416e 795d 203d 204e  ct[str, Any] = N
-00005340: 6f6e 652c 0a20 2020 2074 6f70 6f6c 6f67  one,.    topolog
-00005350: 795f 7265 736f 7572 6365 735f 7061 7468  y_resources_path
-00005360: 733a 204f 7074 696f 6e61 6c5b 4c69 7374  s: Optional[List
-00005370: 5b50 6174 685d 5d20 3d20 4e6f 6e65 2c0a  [Path]] = None,.
-00005380: 2020 2020 616c 6c6f 6361 7469 6f6e 5f73      allocation_s
-00005390: 7472 6174 6567 793a 204f 7074 696f 6e61  trategy: Optiona
-000053a0: 6c5b 7374 725d 203d 204e 6f6e 652c 0a29  l[str] = None,.)
-000053b0: 202d 3e20 5475 706c 655b 696e 742c 204c   -> Tuple[int, L
-000053c0: 6973 745b 7374 725d 5d3a 0a20 2020 2022  ist[str]]:.    "
-000053d0: 2222 4372 6561 7465 2061 206e 6577 2073  ""Create a new s
-000053e0: 696d 756c 6174 696f 6e20 6d6f 6465 6c20  imulation model 
-000053f0: 696e 2064 6174 6162 6173 6520 6261 7365  in database base
-00005400: 6420 6f6e 2074 6865 2070 726f 7669 6465  d on the provide
-00005410: 6420 746f 706f 6c6f 6779 2c20 616c 6f6e  d topology, alon
-00005420: 6720 7769 7468 206f 7074 696f 6e61 6c20  g with optional 
-00005430: 7265 736f 7572 6365 2066 696c 6573 2e0a  resource files..
-00005440: 0a20 2020 203a 7265 7475 726e 3a20 4120  .    :return: A 
-00005450: 7475 706c 6520 636f 6e74 6169 6e69 6e67  tuple containing
-00005460: 2074 6865 2049 4420 6f66 2074 6865 2063   the ID of the c
-00005470: 7265 6174 6564 2073 696d 756c 6174 696f  reated simulatio
-00005480: 6e2c 2061 6e64 2074 6865 206e 6577 206e  n, and the new n
-00005490: 6f64 6573 206f 6620 7468 6520 7369 6d75  odes of the simu
-000054a0: 6c61 7469 6f6e 2e0a 2020 2020 3a72 7479  lation..    :rty
-000054b0: 7065 3a20 3a63 6c61 7373 3a60 5475 706c  pe: :class:`Tupl
-000054c0: 655b 696e 742c 204c 6973 745b 7374 725d  e[int, List[str]
-000054d0: 5d60 0a0a 2020 2020 3a70 6172 616d 2074  ]`..    :param t
-000054e0: 6f70 6f6c 6f67 795f 636f 6e74 656e 743a  opology_content:
-000054f0: 2041 2064 6963 7420 636f 6e74 6169 6e69   A dict containi
-00005500: 6e67 2074 6865 206e 6f64 6573 2061 6e64  ng the nodes and
-00005510: 206e 6574 776f 726b 2074 6f70 6f6c 6f67   network topolog
-00005520: 7920 746f 2063 7265 6174 652e 0a20 2020  y to create..   
-00005530: 203a 7479 7065 2074 6f70 6f6c 6f67 795f   :type topology_
-00005540: 6669 6c65 3a20 3a63 6c61 7373 3a60 6469  file: :class:`di
-00005550: 6374 600a 2020 2020 3a70 6172 616d 2074  ct`.    :param t
-00005560: 6f70 6f6c 6f67 795f 7265 736f 7572 6365  opology_resource
-00005570: 735f 7061 7468 733a 2054 6865 2070 6174  s_paths: The pat
-00005580: 6820 746f 2072 6573 6f75 7263 6573 2074  h to resources t
-00005590: 6861 7420 7769 6c6c 2062 6520 7075 7368  hat will be push
-000055a0: 6564 2069 6e74 6f20 636f 6d70 6174 6962  ed into compatib
-000055b0: 6c65 206e 6f64 6573 2e0a 2020 2020 3a74  le nodes..    :t
-000055c0: 7970 6520 746f 706f 6c6f 6779 5f72 6573  ype topology_res
-000055d0: 6f75 7263 6573 5f70 6174 6873 3a20 3a63  ources_paths: :c
-000055e0: 6c61 7373 3a60 6c69 7374 602c 206f 7074  lass:`list`, opt
-000055f0: 696f 6e61 6c0a 2020 2020 3a70 6172 616d  ional.    :param
-00005600: 2061 6c6c 6f63 6174 696f 6e5f 7374 7261   allocation_stra
-00005610: 7465 6779 3a20 4e61 6d65 206f 6620 7468  tegy: Name of th
-00005620: 6520 616c 6c6f 6361 7469 6f6e 2073 7472  e allocation str
-00005630: 6174 6567 7920 746f 2075 7365 2074 6f20  ategy to use to 
-00005640: 616c 6c6f 6361 7465 206e 6f64 6573 2074  allocate nodes t
-00005650: 6f20 636f 6d70 7574 6520 7365 7276 6572  o compute server
-00005660: 732e 0a20 2020 203a 7479 7065 2061 6c6c  s..    :type all
-00005670: 6f63 6174 696f 6e5f 7374 7261 7465 6779  ocation_strategy
-00005680: 3a20 3a63 6c61 7373 3a60 7374 7260 2c20  : :class:`str`, 
-00005690: 6f70 7469 6f6e 616c 0a0a 2020 2020 2222  optional..    ""
-000056a0: 220a 2020 2020 7369 6d75 6c61 7469 6f6e  ".    simulation
-000056b0: 5f64 6963 7420 3d20 5f6e 6f72 6d61 6c69  _dict = _normali
-000056c0: 7a65 5f73 696d 756c 6174 696f 6e5f 7265  ze_simulation_re
-000056d0: 736f 7572 6365 7328 0a20 2020 2020 2020  sources(.       
-000056e0: 2074 6f70 6f6c 6f67 795f 636f 6e74 656e   topology_conten
-000056f0: 743d 746f 706f 6c6f 6779 5f63 6f6e 7465  t=topology_conte
-00005700: 6e74 2c0a 2020 2020 2020 2020 746f 706f  nt,.        topo
-00005710: 6c6f 6779 5f72 6573 6f75 7263 6573 5f70  logy_resources_p
-00005720: 6174 6873 3d74 6f70 6f6c 6f67 795f 7265  aths=topology_re
-00005730: 736f 7572 6365 735f 7061 7468 732c 0a20  sources_paths,. 
-00005740: 2020 2029 0a0a 2020 2020 7265 7475 726e     )..    return
-00005750: 205f 6372 6561 7465 5f6f 725f 6578 7465   _create_or_exte
-00005760: 6e64 5f73 696d 756c 6174 696f 6e28 0a20  nd_simulation(. 
-00005770: 2020 2020 2020 2073 696d 756c 6174 696f         simulatio
-00005780: 6e5f 6469 6374 3d73 696d 756c 6174 696f  n_dict=simulatio
-00005790: 6e5f 6469 6374 2c20 616c 6c6f 6361 7469  n_dict, allocati
-000057a0: 6f6e 5f73 7472 6174 6567 793d 616c 6c6f  on_strategy=allo
-000057b0: 6361 7469 6f6e 5f73 7472 6174 6567 790a  cation_strategy.
-000057c0: 2020 2020 290a 0a0a 6465 6620 6578 7465      )...def exte
-000057d0: 6e64 5f73 696d 756c 6174 696f 6e28 0a20  nd_simulation(. 
-000057e0: 2020 2074 6f70 6f6c 6f67 795f 636f 6e74     topology_cont
-000057f0: 656e 743a 2044 6963 745b 7374 722c 2041  ent: Dict[str, A
-00005800: 6e79 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ny] = None,.    
-00005810: 746f 706f 6c6f 6779 5f72 6573 6f75 7263  topology_resourc
-00005820: 6573 5f70 6174 6873 3a20 4f70 7469 6f6e  es_paths: Option
-00005830: 616c 5b4c 6973 745b 5061 7468 5d5d 203d  al[List[Path]] =
-00005840: 204e 6f6e 652c 0a20 2020 2061 6c6c 6f63   None,.    alloc
-00005850: 6174 696f 6e5f 7374 7261 7465 6779 3a20  ation_strategy: 
-00005860: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-00005870: 4e6f 6e65 2c0a 2020 2020 6964 5f73 696d  None,.    id_sim
-00005880: 756c 6174 696f 6e3a 2069 6e74 203d 204e  ulation: int = N
-00005890: 6f6e 652c 0a29 202d 3e20 5475 706c 655b  one,.) -> Tuple[
-000058a0: 696e 742c 204c 6973 745b 7374 725d 5d3a  int, List[str]]:
-000058b0: 0a20 2020 2022 2222 4578 7465 6e64 2061  .    """Extend a
-000058c0: 6e20 6578 6973 7469 6e67 2073 696d 756c  n existing simul
-000058d0: 6174 696f 6e20 6d6f 6465 6c20 696e 2064  ation model in d
-000058e0: 6174 6162 6173 6520 6261 7365 6420 6f6e  atabase based on
-000058f0: 2074 6865 2070 726f 7669 6465 6420 746f   the provided to
-00005900: 706f 6c6f 6779 2c20 616c 6f6e 6720 7769  pology, along wi
-00005910: 7468 206f 7074 696f 6e61 6c20 7265 736f  th optional reso
-00005920: 7572 6365 2066 696c 6573 2e0a 0a20 2020  urce files...   
-00005930: 203a 7265 7475 726e 3a20 4120 7475 706c   :return: A tupl
-00005940: 6520 636f 6e74 6169 6e69 6e67 2074 6865  e containing the
-00005950: 2049 4420 6f66 2074 6865 2063 7265 6174   ID of the creat
-00005960: 6564 2073 696d 756c 6174 696f 6e2c 2061  ed simulation, a
-00005970: 6e64 2074 6865 206e 6577 206e 6f64 6573  nd the new nodes
-00005980: 206f 6620 7468 6520 7369 6d75 6c61 7469   of the simulati
-00005990: 6f6e 2e0a 2020 2020 3a72 7479 7065 3a20  on..    :rtype: 
-000059a0: 3a63 6c61 7373 3a60 5475 706c 655b 696e  :class:`Tuple[in
-000059b0: 742c 204c 6973 745b 7374 725d 5d60 0a0a  t, List[str]]`..
-000059c0: 2020 2020 3a70 6172 616d 2074 6f70 6f6c      :param topol
-000059d0: 6f67 795f 636f 6e74 656e 743a 2041 2064  ogy_content: A d
-000059e0: 6963 7420 636f 6e74 6169 6e69 6e67 2074  ict containing t
-000059f0: 6865 206e 6f64 6573 2061 6e64 206e 6574  he nodes and net
-00005a00: 776f 726b 2074 6f70 6f6c 6f67 7920 746f  work topology to
-00005a10: 2063 7265 6174 652e 0a20 2020 203a 7479   create..    :ty
-00005a20: 7065 2074 6f70 6f6c 6f67 795f 6669 6c65  pe topology_file
-00005a30: 3a20 3a63 6c61 7373 3a60 6469 6374 600a  : :class:`dict`.
-00005a40: 2020 2020 3a70 6172 616d 2074 6f70 6f6c      :param topol
-00005a50: 6f67 795f 7265 736f 7572 6365 735f 7061  ogy_resources_pa
-00005a60: 7468 733a 2054 6865 2070 6174 6820 746f  ths: The path to
-00005a70: 2072 6573 6f75 7263 6573 2074 6861 7420   resources that 
-00005a80: 7769 6c6c 2062 6520 7075 7368 6564 2069  will be pushed i
-00005a90: 6e74 6f20 636f 6d70 6174 6962 6c65 206e  nto compatible n
-00005aa0: 6f64 6573 2e0a 2020 2020 3a74 7970 6520  odes..    :type 
-00005ab0: 746f 706f 6c6f 6779 5f72 6573 6f75 7263  topology_resourc
-00005ac0: 6573 5f70 6174 6873 3a20 3a63 6c61 7373  es_paths: :class
-00005ad0: 3a60 6c69 7374 602c 206f 7074 696f 6e61  :`list`, optiona
-00005ae0: 6c0a 2020 2020 3a70 6172 616d 2061 6c6c  l.    :param all
-00005af0: 6f63 6174 696f 6e5f 7374 7261 7465 6779  ocation_strategy
-00005b00: 3a20 4e61 6d65 206f 6620 7468 6520 616c  : Name of the al
-00005b10: 6c6f 6361 7469 6f6e 2073 7472 6174 6567  location strateg
-00005b20: 7920 746f 2075 7365 2074 6f20 616c 6c6f  y to use to allo
-00005b30: 6361 7465 206e 6f64 6573 2074 6f20 636f  cate nodes to co
-00005b40: 6d70 7574 6520 7365 7276 6572 732e 0a20  mpute servers.. 
-00005b50: 2020 203a 7479 7065 2061 6c6c 6f63 6174     :type allocat
-00005b60: 696f 6e5f 7374 7261 7465 6779 3a20 3a63  ion_strategy: :c
-00005b70: 6c61 7373 3a60 7374 7260 2c20 6f70 7469  lass:`str`, opti
-00005b80: 6f6e 616c 0a20 2020 203a 7061 7261 6d20  onal.    :param 
-00005b90: 6964 5f73 696d 756c 6174 696f 6e3a 2054  id_simulation: T
-00005ba0: 6865 2073 696d 756c 6174 696f 6e20 4944  he simulation ID
-00005bb0: 2c20 7768 656e 2065 7874 656e 6469 6e67  , when extending
-00005bc0: 2061 6e20 6578 6973 7469 6e67 2073 696d   an existing sim
-00005bd0: 756c 6174 696f 6e20 7769 7468 206e 6577  ulation with new
-00005be0: 206e 6f64 6573 2061 6e64 206c 696e 6b73   nodes and links
-00005bf0: 2e0a 2020 2020 3a74 7970 6520 6964 5f73  ..    :type id_s
-00005c00: 696d 756c 6174 696f 6e3a 203a 636c 6173  imulation: :clas
-00005c10: 733a 6069 6e74 602c 206f 7074 696f 6e61  s:`int`, optiona
-00005c20: 6c0a 0a20 2020 2022 2222 0a0a 2020 2020  l..    """..    
-00005c30: 7369 6d75 6c61 7469 6f6e 5f64 6963 7420  simulation_dict 
-00005c40: 3d20 5f6e 6f72 6d61 6c69 7a65 5f73 696d  = _normalize_sim
-00005c50: 756c 6174 696f 6e5f 7265 736f 7572 6365  ulation_resource
-00005c60: 7328 0a20 2020 2020 2020 2074 6f70 6f6c  s(.        topol
-00005c70: 6f67 795f 636f 6e74 656e 743d 746f 706f  ogy_content=topo
-00005c80: 6c6f 6779 5f63 6f6e 7465 6e74 2c0a 2020  logy_content,.  
-00005c90: 2020 2020 2020 746f 706f 6c6f 6779 5f72        topology_r
-00005ca0: 6573 6f75 7263 6573 5f70 6174 6873 3d74  esources_paths=t
-00005cb0: 6f70 6f6c 6f67 795f 7265 736f 7572 6365  opology_resource
-00005cc0: 735f 7061 7468 732c 0a20 2020 2029 0a0a  s_paths,.    )..
-00005cd0: 2020 2020 7265 7475 726e 205f 6372 6561      return _crea
-00005ce0: 7465 5f6f 725f 6578 7465 6e64 5f73 696d  te_or_extend_sim
-00005cf0: 756c 6174 696f 6e28 0a20 2020 2020 2020  ulation(.       
-00005d00: 2073 696d 756c 6174 696f 6e5f 6469 6374   simulation_dict
-00005d10: 3d73 696d 756c 6174 696f 6e5f 6469 6374  =simulation_dict
-00005d20: 2c0a 2020 2020 2020 2020 6964 5f73 696d  ,.        id_sim
-00005d30: 756c 6174 696f 6e3d 6964 5f73 696d 756c  ulation=id_simul
-00005d40: 6174 696f 6e2c 0a20 2020 2020 2020 2061  ation,.        a
-00005d50: 6c6c 6f63 6174 696f 6e5f 7374 7261 7465  llocation_strate
-00005d60: 6779 3d61 6c6c 6f63 6174 696f 6e5f 7374  gy=allocation_st
-00005d70: 7261 7465 6779 2c0a 2020 2020 290a 0a0a  rategy,.    )...
-00005d80: 6465 6620 6372 6561 7465 5f73 696d 756c  def create_simul
-00005d90: 6174 696f 6e5f 6672 6f6d 5f74 6f70 6f6c  ation_from_topol
-00005da0: 6f67 7928 0a20 2020 2074 6f70 6f6c 6f67  ogy(.    topolog
-00005db0: 795f 6669 6c65 3a20 7374 7220 3d20 4e6f  y_file: str = No
-00005dc0: 6e65 2c0a 2020 2020 746f 706f 6c6f 6779  ne,.    topology
-00005dd0: 5f72 6573 6f75 7263 6573 5f70 6174 6873  _resources_paths
-00005de0: 3a20 4f70 7469 6f6e 616c 5b4c 6973 745b  : Optional[List[
-00005df0: 5061 7468 5d5d 203d 204e 6f6e 652c 0a20  Path]] = None,. 
-00005e00: 2020 2061 6c6c 6f63 6174 696f 6e5f 7374     allocation_st
-00005e10: 7261 7465 6779 3a20 4f70 7469 6f6e 616c  rategy: Optional
-00005e20: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2920  [str] = None,.) 
-00005e30: 2d3e 2054 7570 6c65 5b69 6e74 2c20 4c69  -> Tuple[int, Li
-00005e40: 7374 5b73 7472 5d5d 3a0a 2020 2020 2222  st[str]]:.    ""
-00005e50: 2243 7265 6174 6520 6120 6e65 7720 7369  "Create a new si
-00005e60: 6d75 6c61 7469 6f6e 206d 6f64 656c 2069  mulation model i
-00005e70: 6e20 6461 7461 6261 7365 2062 6173 6564  n database based
-00005e80: 206f 6e20 7468 6520 7072 6f76 6964 6564   on the provided
-00005e90: 2074 6f70 6f6c 6f67 7920 6669 6c65 2c20   topology file, 
-00005ea0: 616c 6f6e 6720 7769 7468 206f 7074 696f  along with optio
-00005eb0: 6e61 6c20 7265 736f 7572 6365 2066 696c  nal resource fil
-00005ec0: 6573 2e0a 0a20 2020 203a 7265 7475 726e  es...    :return
-00005ed0: 3a20 4120 7475 706c 6520 636f 6e74 6169  : A tuple contai
-00005ee0: 6e69 6e67 2074 6865 2049 4420 6f66 2074  ning the ID of t
-00005ef0: 6865 2063 7265 6174 6564 2073 696d 756c  he created simul
-00005f00: 6174 696f 6e2c 2061 6e64 2074 6865 206e  ation, and the n
-00005f10: 6577 206e 6f64 6573 206f 6620 7468 6520  ew nodes of the 
-00005f20: 7369 6d75 6c61 7469 6f6e 2e0a 2020 2020  simulation..    
-00005f30: 3a72 7479 7065 3a20 3a63 6c61 7373 3a60  :rtype: :class:`
-00005f40: 5475 706c 655b 696e 742c 204c 6973 745b  Tuple[int, List[
-00005f50: 7374 725d 5d60 0a0a 2020 2020 3a70 6172  str]]`..    :par
-00005f60: 616d 2074 6f70 6f6c 6f67 795f 6669 6c65  am topology_file
-00005f70: 3a20 5468 6520 7061 7468 2074 6f20 6120  : The path to a 
-00005f80: 746f 706f 6c6f 6779 2066 696c 6520 636f  topology file co
-00005f90: 6e74 6169 6e69 6e67 2074 6865 206e 6f64  ntaining the nod
-00005fa0: 6573 2061 6e64 206e 6574 776f 726b 2074  es and network t
-00005fb0: 6f70 6f6c 6f67 7920 746f 2063 7265 6174  opology to creat
-00005fc0: 652e 0a20 2020 203a 7479 7065 2074 6f70  e..    :type top
-00005fd0: 6f6c 6f67 795f 6669 6c65 3a20 3a63 6c61  ology_file: :cla
-00005fe0: 7373 3a60 7374 7260 0a20 2020 203a 7061  ss:`str`.    :pa
-00005ff0: 7261 6d20 746f 706f 6c6f 6779 5f72 6573  ram topology_res
-00006000: 6f75 7263 6573 5f70 6174 6873 3a20 5468  ources_paths: Th
-00006010: 6520 7061 7468 2074 6f20 7265 736f 7572  e path to resour
-00006020: 6365 7320 7468 6174 2077 696c 6c20 6265  ces that will be
-00006030: 2070 7573 6865 6420 696e 746f 2063 6f6d   pushed into com
-00006040: 7061 7469 626c 6520 6e6f 6465 732e 0a20  patible nodes.. 
-00006050: 2020 203a 7479 7065 2074 6f70 6f6c 6f67     :type topolog
-00006060: 795f 7265 736f 7572 6365 735f 7061 7468  y_resources_path
-00006070: 733a 203a 636c 6173 733a 6073 7472 602c  s: :class:`str`,
-00006080: 206f 7074 696f 6e61 6c0a 2020 2020 3a70   optional.    :p
-00006090: 6172 616d 2061 6c6c 6f63 6174 696f 6e5f  aram allocation_
-000060a0: 7374 7261 7465 6779 3a20 4e61 6d65 206f  strategy: Name o
-000060b0: 6620 7468 6520 616c 6c6f 6361 7469 6f6e  f the allocation
-000060c0: 2073 7472 6174 6567 7920 746f 2075 7365   strategy to use
-000060d0: 2074 6f20 616c 6c6f 6361 7465 206e 6f64   to allocate nod
-000060e0: 6573 2074 6f20 636f 6d70 7574 6520 7365  es to compute se
-000060f0: 7276 6572 732e 0a20 2020 203a 7479 7065  rvers..    :type
-00006100: 2061 6c6c 6f63 6174 696f 6e5f 7374 7261   allocation_stra
-00006110: 7465 6779 3a20 3a63 6c61 7373 3a60 7374  tegy: :class:`st
-00006120: 7260 2c20 6f70 7469 6f6e 616c 0a0a 2020  r`, optional..  
-00006130: 2020 3e3e 3e20 6672 6f6d 2063 725f 6170    >>> from cr_ap
-00006140: 695f 636c 6965 6e74 2069 6d70 6f72 7420  i_client import 
-00006150: 636f 7265 5f61 7069 0a20 2020 203e 3e3e  core_api.    >>>
-00006160: 2063 6f72 655f 6170 692e 7265 7365 7428   core_api.reset(
-00006170: 290a 2020 2020 2743 6f6d 7075 7465 2069  ).    'Compute i
-00006180: 6e66 7261 7374 7275 6374 7572 6520 7375  nfrastructure su
-00006190: 6363 6573 7366 756c 6c79 2072 6573 6574  ccessfully reset
-000061a0: 270a 2020 2020 3e3e 3e20 636f 7265 5f61  '.    >>> core_a
-000061b0: 7069 2e63 7265 6174 655f 7369 6d75 6c61  pi.create_simula
-000061c0: 7469 6f6e 5f66 726f 6d5f 746f 706f 6c6f  tion_from_topolo
-000061d0: 6779 2822 6461 7461 2f74 6f70 6f6c 6f67  gy("data/topolog
-000061e0: 6965 732f 746f 706f 6c6f 6779 2d31 2d63  ies/topology-1-c
-000061f0: 6c69 656e 742e 7961 6d6c 2229 0a20 2020  lient.yaml").   
-00006200: 2028 312c 205b 2743 4c49 454e 5431 272c   (1, ['CLIENT1',
-00006210: 2027 526f 7574 6572 3127 2c20 2753 7769   'Router1', 'Swi
-00006220: 7463 6831 275d 290a 0a20 2020 2022 2222  tch1'])..    """
-00006230: 0a0a 2020 2020 6966 2074 6f70 6f6c 6f67  ..    if topolog
-00006240: 795f 7265 736f 7572 6365 735f 7061 7468  y_resources_path
-00006250: 7320 6973 204e 6f6e 653a 0a20 2020 2020  s is None:.     
-00006260: 2020 2074 6f70 6f6c 6f67 795f 7265 736f     topology_reso
-00006270: 7572 6365 735f 7061 7468 7320 3d20 5b5d  urces_paths = []
-00006280: 0a0a 2020 2020 2320 4372 6561 7465 2061  ..    # Create a
-00006290: 206e 6577 2073 696d 756c 6174 696f 6e20   new simulation 
-000062a0: 6d6f 6465 6c20 696e 2064 6174 6162 6173  model in databas
-000062b0: 6520 6261 7365 6420 6f6e 2074 6865 2070  e based on the p
-000062c0: 726f 7669 6465 6420 746f 706f 6c6f 6779  rovided topology
-000062d0: 2066 696c 6520 7061 7468 2e22 2222 0a20   file path.""". 
-000062e0: 2020 2069 6620 746f 706f 6c6f 6779 5f66     if topology_f
-000062f0: 696c 6520 6973 204e 6f6e 653a 0a20 2020  ile is None:.   
-00006300: 2020 2020 2072 6169 7365 2045 7863 6570       raise Excep
-00006310: 7469 6f6e 2822 416e 2074 6f70 6f6c 6f67  tion("An topolog
-00006320: 7920 6669 6c65 2069 7320 7265 7175 6972  y file is requir
-00006330: 6564 2229 0a0a 2020 2020 2320 5661 6c69  ed")..    # Vali
-00006340: 6461 7465 2059 414d 4c20 636f 6e66 6967  date YAML config
-00006350: 7572 6174 696f 6e20 6669 6c65 0a20 2020  uration file.   
-00006360: 205f 7661 6c69 6461 7465 5f79 616d 6c5f   _validate_yaml_
-00006370: 746f 706f 6c6f 6779 5f66 696c 6528 746f  topology_file(to
-00006380: 706f 6c6f 6779 5f66 696c 6529 0a0a 2020  pology_file)..  
-00006390: 2020 2320 4f70 656e 2061 6e64 2072 6561    # Open and rea
-000063a0: 6420 5941 4d4c 2063 6f6e 6669 6775 7261  d YAML configura
-000063b0: 7469 6f6e 2066 696c 650a 2020 2020 7961  tion file.    ya
-000063c0: 6d6c 5f63 6f6e 7465 6e74 203d 205f 7265  ml_content = _re
-000063d0: 6164 5f79 616d 6c5f 746f 706f 6c6f 6779  ad_yaml_topology
-000063e0: 5f66 696c 6528 746f 706f 6c6f 6779 5f66  _file(topology_f
-000063f0: 696c 6529 0a0a 2020 2020 2320 5061 7273  ile)..    # Pars
-00006400: 6520 5941 4d4c 2063 6f6e 6669 6775 7261  e YAML configura
-00006410: 7469 6f6e 0a20 2020 2023 2057 6520 7573  tion.    # We us
-00006420: 6520 7275 616d 656c 2e79 616d 6c20 6265  e ruamel.yaml be
-00006430: 6361 7573 6520 6974 206b 6565 7073 2061  cause it keeps a
-00006440: 6e63 686f 7273 2061 6e64 0a20 2020 2023  nchors and.    #
-00006450: 2061 6c69 6173 6573 2069 6e20 6d65 6d6f   aliases in memo
-00006460: 7279 2e20 4974 2069 7320 7665 7279 2063  ry. It is very c
-00006470: 6f6e 7665 6e69 656e 7420 7768 656e 2074  onvenient when t
-00006480: 6865 2073 696d 756c 6174 696f 6e0a 2020  he simulation.  
-00006490: 2020 2320 6973 2073 746f 7265 642f 6665    # is stored/fe
-000064a0: 7463 6865 6420 2872 6566 6572 656e 6365  tched (reference
-000064b0: 7320 6172 6520 6b65 7074 2129 0a20 2020  s are kept!).   
-000064c0: 206c 6f61 6465 7220 3d20 5941 4d4c 2874   loader = YAML(t
-000064d0: 7970 3d22 7274 2229 0a20 2020 2074 6f70  yp="rt").    top
-000064e0: 6f6c 6f67 795f 636f 6e74 656e 7420 3d20  ology_content = 
-000064f0: 6c6f 6164 6572 2e6c 6f61 6428 7961 6d6c  loader.load(yaml
-00006500: 5f63 6f6e 7465 6e74 290a 0a20 2020 205f  _content)..    _
-00006510: 7661 6c69 6461 7465 5f74 6f70 6f6c 6f67  validate_topolog
-00006520: 795f 7265 7175 6972 656d 656e 7473 2874  y_requirements(t
-00006530: 6f70 6f6c 6f67 795f 636f 6e74 656e 742c  opology_content,
-00006540: 2074 6f70 6f6c 6f67 795f 7265 736f 7572   topology_resour
-00006550: 6365 735f 7061 7468 7329 0a0a 2020 2020  ces_paths)..    
-00006560: 2320 4164 6420 6120 6465 6661 756c 7420  # Add a default 
-00006570: 7265 736f 7572 6365 7320 6469 7265 6374  resources direct
-00006580: 6f72 7920 6966 2069 7420 6578 6973 7473  ory if it exists
-00006590: 2e0a 2020 2020 2320 4966 2074 6865 2074  ..    # If the t
-000065a0: 6f70 6f6c 6f67 7920 6973 2022 7061 7468  opology is "path
-000065b0: 2f74 6f2f 746f 706f 2e79 616d 6c22 2c20  /to/topo.yaml", 
-000065c0: 7468 6520 6465 6661 756c 7420 7265 736f  the default reso
-000065d0: 7572 6365 7320 6469 7265 6374 6f72 7920  urces directory 
-000065e0: 6973 2022 7061 7468 2f74 6f2f 7265 736f  is "path/to/reso
-000065f0: 7572 6365 7322 2e0a 2020 2020 746f 706f  urces"..    topo
-00006600: 6c6f 6779 5f72 6573 6f75 7263 6573 5f70  logy_resources_p
-00006610: 6174 6873 203d 205f 6e6f 726d 616c 697a  aths = _normaliz
-00006620: 655f 7369 6d75 6c61 7469 6f6e 5f72 6573  e_simulation_res
-00006630: 6f75 7263 655f 7061 7468 7328 0a20 2020  ource_paths(.   
-00006640: 2020 2020 2074 6f70 6f6c 6f67 795f 7265       topology_re
-00006650: 736f 7572 6365 735f 7061 7468 730a 2020  sources_paths.  
-00006660: 2020 290a 2020 2020 6465 6661 756c 745f    ).    default_
-00006670: 7265 736f 7572 6365 735f 7061 7468 203d  resources_path =
-00006680: 206f 732e 7061 7468 2e6a 6f69 6e28 6f73   os.path.join(os
-00006690: 2e70 6174 682e 6469 726e 616d 6528 746f  .path.dirname(to
-000066a0: 706f 6c6f 6779 5f66 696c 6529 2c20 2272  pology_file), "r
-000066b0: 6573 6f75 7263 6573 2229 0a20 2020 2064  esources").    d
-000066c0: 6566 6175 6c74 5f72 6573 6f75 7263 6573  efault_resources
-000066d0: 5f70 6174 6820 3d20 6f73 2e70 6174 682e  _path = os.path.
-000066e0: 6e6f 726d 7061 7468 2864 6566 6175 6c74  normpath(default
-000066f0: 5f72 6573 6f75 7263 6573 5f70 6174 6829  _resources_path)
-00006700: 0a20 2020 2069 6620 5f5f 7661 6c69 6461  .    if __valida
-00006710: 7465 5f72 6573 6f75 7263 6573 5f70 6174  te_resources_pat
-00006720: 6828 6465 6661 756c 745f 7265 736f 7572  h(default_resour
-00006730: 6365 735f 7061 7468 2c20 4661 6c73 6529  ces_path, False)
-00006740: 3a0a 2020 2020 2020 2020 6966 2064 6566  :.        if def
-00006750: 6175 6c74 5f72 6573 6f75 7263 6573 5f70  ault_resources_p
-00006760: 6174 6820 6e6f 7420 696e 2074 6f70 6f6c  ath not in topol
-00006770: 6f67 795f 7265 736f 7572 6365 735f 7061  ogy_resources_pa
-00006780: 7468 733a 0a20 2020 2020 2020 2020 2020  ths:.           
-00006790: 2074 6f70 6f6c 6f67 795f 7265 736f 7572   topology_resour
-000067a0: 6365 735f 7061 7468 732e 6170 7065 6e64  ces_paths.append
-000067b0: 2864 6566 6175 6c74 5f72 6573 6f75 7263  (default_resourc
-000067c0: 6573 5f70 6174 6829 0a0a 2020 2020 7265  es_path)..    re
-000067d0: 7475 726e 2063 7265 6174 655f 7369 6d75  turn create_simu
-000067e0: 6c61 7469 6f6e 280a 2020 2020 2020 2020  lation(.        
-000067f0: 746f 706f 6c6f 6779 5f63 6f6e 7465 6e74  topology_content
-00006800: 3d74 6f70 6f6c 6f67 795f 636f 6e74 656e  =topology_conten
-00006810: 742c 0a20 2020 2020 2020 2074 6f70 6f6c  t,.        topol
-00006820: 6f67 795f 7265 736f 7572 6365 735f 7061  ogy_resources_pa
-00006830: 7468 733d 746f 706f 6c6f 6779 5f72 6573  ths=topology_res
-00006840: 6f75 7263 6573 5f70 6174 6873 2c0a 2020  ources_paths,.  
-00006850: 2020 2020 2020 616c 6c6f 6361 7469 6f6e        allocation
-00006860: 5f73 7472 6174 6567 793d 616c 6c6f 6361  _strategy=alloca
-00006870: 7469 6f6e 5f73 7472 6174 6567 792c 0a20  tion_strategy,. 
-00006880: 2020 2029 0a0a 0a64 6566 2065 7874 656e     )...def exten
-00006890: 645f 7369 6d75 6c61 7469 6f6e 5f66 726f  d_simulation_fro
-000068a0: 6d5f 746f 706f 6c6f 6779 280a 2020 2020  m_topology(.    
-000068b0: 746f 706f 6c6f 6779 5f66 696c 653a 2073  topology_file: s
-000068c0: 7472 203d 204e 6f6e 652c 0a20 2020 2074  tr = None,.    t
-000068d0: 6f70 6f6c 6f67 795f 7265 736f 7572 6365  opology_resource
-000068e0: 735f 7061 7468 733a 204f 7074 696f 6e61  s_paths: Optiona
-000068f0: 6c5b 4c69 7374 5b50 6174 685d 5d20 3d20  l[List[Path]] = 
-00006900: 4e6f 6e65 2c0a 2020 2020 616c 6c6f 6361  None,.    alloca
-00006910: 7469 6f6e 5f73 7472 6174 6567 793a 204f  tion_strategy: O
-00006920: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-00006930: 6f6e 652c 0a20 2020 2069 645f 7369 6d75  one,.    id_simu
-00006940: 6c61 7469 6f6e 3a20 696e 7420 3d20 4e6f  lation: int = No
-00006950: 6e65 2c0a 2920 2d3e 2054 7570 6c65 5b69  ne,.) -> Tuple[i
-00006960: 6e74 2c20 4c69 7374 5b73 7472 5d5d 3a0a  nt, List[str]]:.
-00006970: 2020 2020 2222 2245 7874 656e 6420 616e      """Extend an
-00006980: 2065 7869 7374 696e 6720 7369 6d75 6c61   existing simula
-00006990: 7469 6f6e 206d 6f64 656c 2069 6e20 6461  tion model in da
-000069a0: 7461 6261 7365 2062 6173 6564 206f 6e20  tabase based on 
-000069b0: 7468 6520 7072 6f76 6964 6564 2074 6f70  the provided top
-000069c0: 6f6c 6f67 7920 6669 6c65 2c20 616c 6f6e  ology file, alon
-000069d0: 6720 7769 7468 206f 7074 696f 6e61 6c20  g with optional 
-000069e0: 7265 736f 7572 6365 2066 696c 6573 2e0a  resource files..
-000069f0: 0a20 2020 203a 7265 7475 726e 3a20 4120  .    :return: A 
-00006a00: 7475 706c 6520 636f 6e74 6169 6e69 6e67  tuple containing
-00006a10: 2074 6865 2049 4420 6f66 2074 6865 2063   the ID of the c
-00006a20: 7265 6174 6564 2073 696d 756c 6174 696f  reated simulatio
-00006a30: 6e2c 2061 6e64 2074 6865 206e 6577 206e  n, and the new n
-00006a40: 6f64 6573 206f 6620 7468 6520 7369 6d75  odes of the simu
-00006a50: 6c61 7469 6f6e 2e0a 2020 2020 3a72 7479  lation..    :rty
-00006a60: 7065 3a20 3a63 6c61 7373 3a60 5475 706c  pe: :class:`Tupl
-00006a70: 655b 696e 742c 204c 6973 745b 7374 725d  e[int, List[str]
-00006a80: 5d60 0a0a 2020 2020 3a70 6172 616d 2074  ]`..    :param t
-00006a90: 6f70 6f6c 6f67 795f 6669 6c65 3a20 5468  opology_file: Th
-00006aa0: 6520 7061 7468 2074 6f20 6120 746f 706f  e path to a topo
-00006ab0: 6c6f 6779 2066 696c 6520 636f 6e74 6169  logy file contai
-00006ac0: 6e69 6e67 2074 6865 206e 6f64 6573 2061  ning the nodes a
-00006ad0: 6e64 206e 6574 776f 726b 2074 6f70 6f6c  nd network topol
-00006ae0: 6f67 7920 746f 2063 7265 6174 652e 0a20  ogy to create.. 
-00006af0: 2020 203a 7479 7065 2074 6f70 6f6c 6f67     :type topolog
-00006b00: 795f 6669 6c65 3a20 3a63 6c61 7373 3a60  y_file: :class:`
-00006b10: 7374 7260 0a20 2020 203a 7061 7261 6d20  str`.    :param 
-00006b20: 746f 706f 6c6f 6779 5f72 6573 6f75 7263  topology_resourc
-00006b30: 6573 5f70 6174 6873 3a20 5468 6520 7061  es_paths: The pa
-00006b40: 7468 2074 6f20 7265 736f 7572 6365 7320  th to resources 
-00006b50: 7468 6174 2077 696c 6c20 6265 2070 7573  that will be pus
-00006b60: 6865 6420 696e 746f 2063 6f6d 7061 7469  hed into compati
-00006b70: 626c 6520 6e6f 6465 732e 0a20 2020 203a  ble nodes..    :
-00006b80: 7479 7065 2074 6f70 6f6c 6f67 795f 7265  type topology_re
-00006b90: 736f 7572 6365 735f 7061 7468 733a 203a  sources_paths: :
-00006ba0: 636c 6173 733a 6073 7472 602c 206f 7074  class:`str`, opt
-00006bb0: 696f 6e61 6c0a 2020 2020 3a70 6172 616d  ional.    :param
-00006bc0: 2061 6c6c 6f63 6174 696f 6e5f 7374 7261   allocation_stra
-00006bd0: 7465 6779 3a20 4e61 6d65 206f 6620 7468  tegy: Name of th
-00006be0: 6520 616c 6c6f 6361 7469 6f6e 2073 7472  e allocation str
-00006bf0: 6174 6567 7920 746f 2075 7365 2074 6f20  ategy to use to 
-00006c00: 616c 6c6f 6361 7465 206e 6f64 6573 2074  allocate nodes t
-00006c10: 6f20 636f 6d70 7574 6520 7365 7276 6572  o compute server
-00006c20: 732e 0a20 2020 203a 7479 7065 2061 6c6c  s..    :type all
-00006c30: 6f63 6174 696f 6e5f 7374 7261 7465 6779  ocation_strategy
-00006c40: 3a20 3a63 6c61 7373 3a60 7374 7260 2c20  : :class:`str`, 
-00006c50: 6f70 7469 6f6e 616c 0a20 2020 203a 7061  optional.    :pa
-00006c60: 7261 6d20 6964 5f73 696d 756c 6174 696f  ram id_simulatio
-00006c70: 6e3a 2054 6865 2073 696d 756c 6174 696f  n: The simulatio
-00006c80: 6e20 4944 2c20 7768 656e 2065 7874 656e  n ID, when exten
-00006c90: 6469 6e67 2061 6e20 6578 6973 7469 6e67  ding an existing
-00006ca0: 2073 696d 756c 6174 696f 6e20 7769 7468   simulation with
-00006cb0: 206e 6577 206e 6f64 6573 2061 6e64 206c   new nodes and l
-00006cc0: 696e 6b73 2e0a 2020 2020 3a74 7970 6520  inks..    :type 
-00006cd0: 6964 5f73 696d 756c 6174 696f 6e3a 203a  id_simulation: :
-00006ce0: 636c 6173 733a 6069 6e74 602c 206f 7074  class:`int`, opt
-00006cf0: 696f 6e61 6c0a 2020 2020 2222 220a 2020  ional.    """.  
-00006d00: 2020 6966 2074 6f70 6f6c 6f67 795f 7265    if topology_re
-00006d10: 736f 7572 6365 735f 7061 7468 7320 6973  sources_paths is
-00006d20: 204e 6f6e 653a 0a20 2020 2020 2020 2074   None:.        t
-00006d30: 6f70 6f6c 6f67 795f 7265 736f 7572 6365  opology_resource
-00006d40: 735f 7061 7468 7320 3d20 5b5d 0a0a 2020  s_paths = []..  
-00006d50: 2020 2320 4372 6561 7465 2061 206e 6577    # Create a new
-00006d60: 2073 696d 756c 6174 696f 6e20 6d6f 6465   simulation mode
-00006d70: 6c20 696e 2064 6174 6162 6173 6520 6261  l in database ba
-00006d80: 7365 6420 6f6e 2074 6865 2070 726f 7669  sed on the provi
-00006d90: 6465 6420 746f 706f 6c6f 6779 2066 696c  ded topology fil
-00006da0: 6520 7061 7468 2e22 2222 0a20 2020 2069  e path.""".    i
-00006db0: 6620 746f 706f 6c6f 6779 5f66 696c 6520  f topology_file 
-00006dc0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00006dd0: 2072 6169 7365 2045 7863 6570 7469 6f6e   raise Exception
-00006de0: 2822 416e 2074 6f70 6f6c 6f67 7920 6669  ("An topology fi
-00006df0: 6c65 2069 7320 7265 7175 6972 6564 2229  le is required")
-00006e00: 0a0a 2020 2020 2320 5661 6c69 6461 7465  ..    # Validate
-00006e10: 2059 414d 4c20 636f 6e66 6967 7572 6174   YAML configurat
-00006e20: 696f 6e20 6669 6c65 0a20 2020 205f 7661  ion file.    _va
-00006e30: 6c69 6461 7465 5f79 616d 6c5f 746f 706f  lidate_yaml_topo
-00006e40: 6c6f 6779 5f66 696c 6528 746f 706f 6c6f  logy_file(topolo
-00006e50: 6779 5f66 696c 6529 0a0a 2020 2020 2320  gy_file)..    # 
-00006e60: 4f70 656e 2061 6e64 2072 6561 6420 5941  Open and read YA
-00006e70: 4d4c 2063 6f6e 6669 6775 7261 7469 6f6e  ML configuration
-00006e80: 2066 696c 650a 2020 2020 7961 6d6c 5f63   file.    yaml_c
-00006e90: 6f6e 7465 6e74 203d 205f 7265 6164 5f79  ontent = _read_y
-00006ea0: 616d 6c5f 746f 706f 6c6f 6779 5f66 696c  aml_topology_fil
-00006eb0: 6528 746f 706f 6c6f 6779 5f66 696c 6529  e(topology_file)
-00006ec0: 0a0a 2020 2020 2320 5061 7273 6520 5941  ..    # Parse YA
-00006ed0: 4d4c 2063 6f6e 6669 6775 7261 7469 6f6e  ML configuration
-00006ee0: 0a20 2020 2023 2057 6520 7573 6520 7275  .    # We use ru
-00006ef0: 616d 656c 2e79 616d 6c20 6265 6361 7573  amel.yaml becaus
-00006f00: 6520 6974 206b 6565 7073 2061 6e63 686f  e it keeps ancho
-00006f10: 7273 2061 6e64 0a20 2020 2023 2061 6c69  rs and.    # ali
-00006f20: 6173 6573 2069 6e20 6d65 6d6f 7279 2e20  ases in memory. 
-00006f30: 4974 2069 7320 7665 7279 2063 6f6e 7665  It is very conve
-00006f40: 6e69 656e 7420 7768 656e 2074 6865 2073  nient when the s
-00006f50: 696d 756c 6174 696f 6e0a 2020 2020 2320  imulation.    # 
-00006f60: 6973 2073 746f 7265 642f 6665 7463 6865  is stored/fetche
-00006f70: 6420 2872 6566 6572 656e 6365 7320 6172  d (references ar
-00006f80: 6520 6b65 7074 2129 0a20 2020 206c 6f61  e kept!).    loa
-00006f90: 6465 7220 3d20 5941 4d4c 2874 7970 3d22  der = YAML(typ="
-00006fa0: 7274 2229 0a20 2020 2074 6f70 6f6c 6f67  rt").    topolog
-00006fb0: 795f 636f 6e74 656e 7420 3d20 6c6f 6164  y_content = load
-00006fc0: 6572 2e6c 6f61 6428 7961 6d6c 5f63 6f6e  er.load(yaml_con
-00006fd0: 7465 6e74 290a 0a20 2020 2023 2041 6464  tent)..    # Add
-00006fe0: 2061 2064 6566 6175 6c74 2072 6573 6f75   a default resou
-00006ff0: 7263 6573 2064 6972 6563 746f 7279 2069  rces directory i
-00007000: 6620 6974 2065 7869 7374 732e 0a20 2020  f it exists..   
-00007010: 2023 2049 6620 7468 6520 746f 706f 6c6f   # If the topolo
-00007020: 6779 2069 7320 2270 6174 682f 746f 2f74  gy is "path/to/t
-00007030: 6f70 6f2e 7961 6d6c 222c 2074 6865 2064  opo.yaml", the d
-00007040: 6566 6175 6c74 2072 6573 6f75 7263 6573  efault resources
-00007050: 2064 6972 6563 746f 7279 2069 7320 2270   directory is "p
-00007060: 6174 682f 746f 2f72 6573 6f75 7263 6573  ath/to/resources
-00007070: 222e 0a20 2020 2064 6566 6175 6c74 5f72  "..    default_r
-00007080: 6573 6f75 7263 6573 5f70 6174 6820 3d20  esources_path = 
-00007090: 6f73 2e70 6174 682e 6a6f 696e 286f 732e  os.path.join(os.
-000070a0: 7061 7468 2e64 6972 6e61 6d65 2874 6f70  path.dirname(top
-000070b0: 6f6c 6f67 795f 6669 6c65 292c 2022 7265  ology_file), "re
-000070c0: 736f 7572 6365 7322 290a 2020 2020 6465  sources").    de
-000070d0: 6661 756c 745f 7265 736f 7572 6365 735f  fault_resources_
-000070e0: 7061 7468 203d 206f 732e 7061 7468 2e6e  path = os.path.n
-000070f0: 6f72 6d70 6174 6828 6465 6661 756c 745f  ormpath(default_
-00007100: 7265 736f 7572 6365 735f 7061 7468 290a  resources_path).
-00007110: 2020 2020 6966 205f 5f76 616c 6964 6174      if __validat
-00007120: 655f 7265 736f 7572 6365 735f 7061 7468  e_resources_path
-00007130: 2864 6566 6175 6c74 5f72 6573 6f75 7263  (default_resourc
-00007140: 6573 5f70 6174 682c 2046 616c 7365 293a  es_path, False):
-00007150: 0a20 2020 2020 2020 2069 6620 6465 6661  .        if defa
-00007160: 756c 745f 7265 736f 7572 6365 735f 7061  ult_resources_pa
-00007170: 7468 206e 6f74 2069 6e20 746f 706f 6c6f  th not in topolo
-00007180: 6779 5f72 6573 6f75 7263 6573 5f70 6174  gy_resources_pat
-00007190: 6873 3a0a 2020 2020 2020 2020 2020 2020  hs:.            
-000071a0: 746f 706f 6c6f 6779 5f72 6573 6f75 7263  topology_resourc
-000071b0: 6573 5f70 6174 6873 2e61 7070 656e 6428  es_paths.append(
-000071c0: 6465 6661 756c 745f 7265 736f 7572 6365  default_resource
-000071d0: 735f 7061 7468 290a 0a20 2020 2072 6574  s_path)..    ret
-000071e0: 7572 6e20 6578 7465 6e64 5f73 696d 756c  urn extend_simul
-000071f0: 6174 696f 6e28 0a20 2020 2020 2020 2074  ation(.        t
-00007200: 6f70 6f6c 6f67 795f 636f 6e74 656e 743d  opology_content=
-00007210: 746f 706f 6c6f 6779 5f63 6f6e 7465 6e74  topology_content
-00007220: 2c0a 2020 2020 2020 2020 746f 706f 6c6f  ,.        topolo
-00007230: 6779 5f72 6573 6f75 7263 6573 5f70 6174  gy_resources_pat
-00007240: 6873 3d74 6f70 6f6c 6f67 795f 7265 736f  hs=topology_reso
-00007250: 7572 6365 735f 7061 7468 732c 0a20 2020  urces_paths,.   
-00007260: 2020 2020 2061 6c6c 6f63 6174 696f 6e5f       allocation_
-00007270: 7374 7261 7465 6779 3d61 6c6c 6f63 6174  strategy=allocat
-00007280: 696f 6e5f 7374 7261 7465 6779 2c0a 2020  ion_strategy,.  
-00007290: 2020 2020 2020 6964 5f73 696d 756c 6174        id_simulat
-000072a0: 696f 6e3d 6964 5f73 696d 756c 6174 696f  ion=id_simulatio
-000072b0: 6e2c 0a20 2020 2029 0a0a 0a64 6566 2063  n,.    )...def c
-000072c0: 7265 6174 655f 7369 6d75 6c61 7469 6f6e  reate_simulation
-000072d0: 5f66 726f 6d5f 6261 7365 626f 7828 0a20  _from_basebox(. 
-000072e0: 2020 2062 6173 6562 6f78 5f69 643a 2073     basebox_id: s
-000072f0: 7472 2c0a 2020 2020 6164 645f 696e 7465  tr,.    add_inte
-00007300: 726e 6574 3a20 626f 6f6c 203d 2046 616c  rnet: bool = Fal
-00007310: 7365 2c0a 2020 2020 6164 645f 686f 7374  se,.    add_host
-00007320: 3a20 626f 6f6c 203d 2046 616c 7365 2c0a  : bool = False,.
-00007330: 2020 2020 616c 6c6f 6361 7469 6f6e 5f73      allocation_s
-00007340: 7472 6174 6567 793a 204f 7074 696f 6e61  trategy: Optiona
-00007350: 6c5b 7374 725d 203d 204e 6f6e 652c 0a29  l[str] = None,.)
-00007360: 202d 3e20 696e 743a 0a20 2020 2022 2222   -> int:.    """
-00007370: 4372 6561 7465 2061 206e 6577 2073 696d  Create a new sim
-00007380: 756c 6174 696f 6e20 6d6f 6465 6c20 696e  ulation model in
-00007390: 2064 6174 6162 6173 6520 6261 7365 6420   database based 
-000073a0: 6f6e 2074 6865 2070 726f 7669 6465 6420  on the provided 
-000073b0: 6261 7365 626f 7820 6964 2c20 7769 7468  basebox id, with
-000073c0: 0a20 2020 206f 7074 696f 6e61 6c20 696e  .    optional in
-000073d0: 7465 726e 6574 2061 6e64 2f6f 7220 686f  ternet and/or ho
-000073e0: 7374 2063 6f6e 6e65 6374 6976 6974 792e  st connectivity.
-000073f0: 0a0a 2020 2020 2222 220a 0a20 2020 2069  ..    """..    i
-00007400: 6620 6261 7365 626f 785f 6964 2069 7320  f basebox_id is 
-00007410: 4e6f 6e65 3a0a 2020 2020 2020 2020 7261  None:.        ra
-00007420: 6973 6520 4578 6365 7074 696f 6e28 2241  ise Exception("A
-00007430: 2062 6173 6562 6f78 2049 4420 6973 2072   basebox ID is r
-00007440: 6571 7569 7265 6422 290a 0a20 2020 2023  equired")..    #
-00007450: 2043 7265 6174 6520 616e 2074 6f70 6f6c   Create an topol
-00007460: 6f67 7920 7769 7468 2074 6865 2070 726f  ogy with the pro
-00007470: 7669 6465 6420 6261 7365 626f 7820 4944  vided basebox ID
-00007480: 0a20 2020 2074 7279 3a0a 2020 2020 2020  .    try:.      
-00007490: 2020 6261 7365 626f 7820 3d20 6665 7463    basebox = fetc
-000074a0: 685f 6261 7365 626f 7828 6261 7365 626f  h_basebox(basebo
-000074b0: 785f 6964 290a 2020 2020 6578 6365 7074  x_id).    except
-000074c0: 2045 7863 6570 7469 6f6e 3a0a 2020 2020   Exception:.    
-000074d0: 2020 2020 7261 6973 6520 4578 6365 7074      raise Except
-000074e0: 696f 6e28 0a20 2020 2020 2020 2020 2020  ion(.           
-000074f0: 2066 2243 616e 6e6f 7420 6669 6e64 2062   f"Cannot find b
-00007500: 6173 6562 6f78 2069 6e20 6461 7461 6261  asebox in databa
-00007510: 7365 2066 726f 6d20 6261 7365 626f 7820  se from basebox 
-00007520: 4944 2027 7b62 6173 6562 6f78 5f69 647d  ID '{basebox_id}
-00007530: 2722 0a20 2020 2020 2020 2029 0a0a 2020  '".        )..  
-00007540: 2020 6e6f 6465 5f6e 616d 6520 3d20 5f67    node_name = _g
-00007550: 6574 5f72 616e 646f 6d5f 7374 7269 6e67  et_random_string
-00007560: 2831 3029 0a20 2020 2072 6f6c 6520 3d20  (10).    role = 
-00007570: 6261 7365 626f 785b 2272 6f6c 6522 5d0a  basebox["role"].
-00007580: 2020 2020 6e62 5f70 726f 6320 3d20 6261      nb_proc = ba
-00007590: 7365 626f 785b 226e 625f 7072 6f63 225d  sebox["nb_proc"]
-000075a0: 0a20 2020 206d 656d 6f72 795f 7369 7a65  .    memory_size
-000075b0: 203d 2062 6173 6562 6f78 5b22 6d65 6d6f   = basebox["memo
-000075c0: 7279 5f73 697a 6522 5d0a 0a20 2020 2079  ry_size"]..    y
-000075d0: 616d 6c5f 636f 6e74 656e 7420 3d20 6622  aml_content = f"
-000075e0: 2222 2d2d 2d0a 6e61 6d65 3a20 227b 6261  ""---.name: "{ba
-000075f0: 7365 626f 785f 6964 7d22 0a6e 6f64 6573  sebox_id}".nodes
-00007600: 3a0a 0a20 202d 2026 7377 6974 6368 0a20  :..  - &switch. 
-00007610: 2020 2074 7970 653a 2073 7769 7463 680a     type: switch.
-00007620: 2020 2020 6e61 6d65 3a20 2273 7769 7463      name: "switc
-00007630: 6822 0a0a 2020 2d20 2663 6c69 656e 740a  h"..  - &client.
-00007640: 2020 2020 7479 7065 3a20 7669 7274 7561      type: virtua
-00007650: 6c5f 6d61 6368 696e 650a 2020 2020 6e61  l_machine.    na
-00007660: 6d65 3a20 227b 6e6f 6465 5f6e 616d 657d  me: "{node_name}
-00007670: 220a 2020 2020 6261 7365 626f 785f 6964  ".    basebox_id
-00007680: 3a20 227b 6261 7365 626f 785f 6964 7d22  : "{basebox_id}"
-00007690: 0a20 2020 206e 625f 7072 6f63 3a20 7b6e  .    nb_proc: {n
-000076a0: 625f 7072 6f63 7d0a 2020 2020 6d65 6d6f  b_proc}.    memo
-000076b0: 7279 5f73 697a 653a 207b 6d65 6d6f 7279  ry_size: {memory
-000076c0: 5f73 697a 657d 0a20 2020 2072 6f6c 6573  _size}.    roles
-000076d0: 3a20 5b22 7b72 6f6c 657d 225d 0a22 2222  : ["{role}"]."""
-000076e0: 0a0a 2020 2020 6966 2061 6464 5f68 6f73  ..    if add_hos
-000076f0: 743a 0a20 2020 2020 2020 2079 616d 6c5f  t:.        yaml_
-00007700: 636f 6e74 656e 7420 2b3d 2022 2222 0a20  content += """. 
-00007710: 202d 2026 686f 7374 5f6d 6163 6869 6e65   - &host_machine
-00007720: 0a20 2020 2074 7970 653a 2068 6f73 745f  .    type: host_
-00007730: 6d61 6368 696e 650a 2020 2020 6e61 6d65  machine.    name
-00007740: 3a20 2268 6f73 7422 0a22 2222 0a0a 2020  : "host"."""..  
-00007750: 2020 6966 2061 6464 5f69 6e74 6572 6e65    if add_interne
-00007760: 743a 0a20 2020 2020 2020 2023 2061 6464  t:.        # add
-00007770: 2064 6566 6175 6c74 2072 6f75 7465 2074   default route t
-00007780: 6f20 6761 7465 7761 792c 2061 2067 6174  o gateway, a gat
-00007790: 6577 6179 2061 6e64 2061 2073 7769 7463  eway and a switc
-000077a0: 6820 746f 2070 6c75 6720 7468 6520 6761  h to plug the ga
-000077b0: 7465 7761 7920 616e 6420 7468 6520 726f  teway and the ro
-000077c0: 7574 6572 0a20 2020 2020 2020 2079 616d  uter.        yam
-000077d0: 6c5f 636f 6e74 656e 7420 2b3d 2022 2222  l_content += """
-000077e0: 0a20 202d 2026 726f 7574 6572 0a20 2020  .  - &router.   
-000077f0: 2074 7970 653a 2072 6f75 7465 720a 2020   type: router.  
-00007800: 2020 6e61 6d65 3a20 2272 6f75 7465 7222    name: "router"
-00007810: 0a20 2020 2072 6f75 7465 733a 0a20 2020  .    routes:.   
-00007820: 2020 202d 2022 302e 302e 302e 302f 3020     - "0.0.0.0/0 
-00007830: 2d3e 2031 3932 2e31 3638 2e32 332e 3222  -> 192.168.23.2"
-00007840: 0a0a 2020 2d20 2673 7769 7463 685f 696e  ..  - &switch_in
-00007850: 7465 726e 6574 0a20 2020 2074 7970 653a  ternet.    type:
-00007860: 2073 7769 7463 680a 2020 2020 6e61 6d65   switch.    name
-00007870: 3a20 2273 7769 7463 6849 6e74 6572 6e65  : "switchInterne
-00007880: 7422 0a0a 2020 2d20 2670 6879 7369 6361  t"..  - &physica
-00007890: 6c5f 6761 7465 7761 790a 2020 2020 7479  l_gateway.    ty
-000078a0: 7065 3a20 7068 7973 6963 616c 5f67 6174  pe: physical_gat
-000078b0: 6577 6179 0a20 2020 206e 616d 653a 2022  eway.    name: "
-000078c0: 7068 7973 6963 616c 4761 7465 7761 7922  physicalGateway"
-000078d0: 0a22 2222 0a20 2020 2065 6c73 653a 0a20  .""".    else:. 
-000078e0: 2020 2020 2020 2079 616d 6c5f 636f 6e74         yaml_cont
-000078f0: 656e 7420 2b3d 2022 2222 0a20 202d 2026  ent += """.  - &
-00007900: 726f 7574 6572 0a20 2020 2074 7970 653a  router.    type:
-00007910: 2072 6f75 7465 720a 2020 2020 6e61 6d65   router.    name
-00007920: 3a20 2272 6f75 7465 7222 0a22 2222 0a0a  : "router"."""..
-00007930: 2020 2020 7961 6d6c 5f63 6f6e 7465 6e74      yaml_content
-00007940: 202b 3d20 2222 220a 6c69 6e6b 733a 0a0a   += """.links:..
-00007950: 2020 2d20 7377 6974 6368 3a20 2a73 7769    - switch: *swi
-00007960: 7463 680a 2020 2020 6e6f 6465 3a20 2a72  tch.    node: *r
-00007970: 6f75 7465 720a 2020 2020 7061 7261 6d73  outer.    params
-00007980: 3a0a 2020 2020 2020 6970 3a20 2231 3932  :.      ip: "192
-00007990: 2e31 3638 2e32 2e31 2f32 3422 0a20 2020  .168.2.1/24".   
-000079a0: 2020 2064 6863 705f 6e61 6d65 7365 7276     dhcp_nameserv
-000079b0: 6572 3a20 2238 2e38 2e38 2e38 220a 0a20  er: "8.8.8.8".. 
-000079c0: 202d 2073 7769 7463 683a 202a 7377 6974   - switch: *swit
-000079d0: 6368 0a20 2020 206e 6f64 653a 202a 636c  ch.    node: *cl
-000079e0: 6965 6e74 0a20 2020 2070 6172 616d 733a  ient.    params:
-000079f0: 0a20 2020 2020 2069 703a 2022 3139 322e  .      ip: "192.
-00007a00: 3136 382e 322e 322f 3234 220a 2222 220a  168.2.2/24".""".
-00007a10: 0a20 2020 2069 6620 6164 645f 686f 7374  .    if add_host
-00007a20: 3a0a 2020 2020 2020 2020 7961 6d6c 5f63  :.        yaml_c
-00007a30: 6f6e 7465 6e74 202b 3d20 2222 220a 2020  ontent += """.  
-00007a40: 2d20 7377 6974 6368 3a20 2a73 7769 7463  - switch: *switc
-00007a50: 680a 2020 2020 6e6f 6465 3a20 2a68 6f73  h.    node: *hos
-00007a60: 745f 6d61 6368 696e 650a 2020 2020 7061  t_machine.    pa
-00007a70: 7261 6d73 3a0a 2020 2020 2020 6970 3a20  rams:.      ip: 
-00007a80: 2231 3932 2e31 3638 2e32 2e33 2f32 3422  "192.168.2.3/24"
-00007a90: 0a22 2222 0a0a 2020 2020 6966 2061 6464  ."""..    if add
-00007aa0: 5f69 6e74 6572 6e65 743a 0a20 2020 2020  _internet:.     
-00007ab0: 2020 2079 616d 6c5f 636f 6e74 656e 7420     yaml_content 
-00007ac0: 2b3d 2022 2222 0a20 202d 2073 7769 7463  += """.  - switc
-00007ad0: 683a 202a 7377 6974 6368 5f69 6e74 6572  h: *switch_inter
-00007ae0: 6e65 740a 2020 2020 6e6f 6465 3a20 2a72  net.    node: *r
-00007af0: 6f75 7465 720a 2020 2020 7061 7261 6d73  outer.    params
-00007b00: 3a0a 2020 2020 2020 6970 3a20 2231 3932  :.      ip: "192
-00007b10: 2e31 3638 2e32 332e 312f 3234 220a 0a20  .168.23.1/24".. 
-00007b20: 202d 2073 7769 7463 683a 202a 7377 6974   - switch: *swit
-00007b30: 6368 5f69 6e74 6572 6e65 740a 2020 2020  ch_internet.    
-00007b40: 6e6f 6465 3a20 2a70 6879 7369 6361 6c5f  node: *physical_
-00007b50: 6761 7465 7761 790a 2020 2020 7061 7261  gateway.    para
-00007b60: 6d73 3a0a 2020 2020 2020 6970 3a20 2231  ms:.      ip: "1
-00007b70: 3932 2e31 3638 2e32 332e 322f 3234 220a  92.168.23.2/24".
-00007b80: 2222 220a 0a20 2020 206c 6f61 6465 7220  """..    loader 
-00007b90: 3d20 5941 4d4c 2874 7970 3d22 7274 2229  = YAML(typ="rt")
-00007ba0: 0a20 2020 2074 6f70 6f6c 6f67 795f 636f  .    topology_co
-00007bb0: 6e74 656e 7420 3d20 6c6f 6164 6572 2e6c  ntent = loader.l
-00007bc0: 6f61 6428 7961 6d6c 5f63 6f6e 7465 6e74  oad(yaml_content
-00007bd0: 290a 0a20 2020 2072 6574 7572 6e20 6372  )..    return cr
-00007be0: 6561 7465 5f73 696d 756c 6174 696f 6e28  eate_simulation(
-00007bf0: 0a20 2020 2020 2020 2074 6f70 6f6c 6f67  .        topolog
-00007c00: 795f 636f 6e74 656e 743d 746f 706f 6c6f  y_content=topolo
-00007c10: 6779 5f63 6f6e 7465 6e74 2c0a 2020 2020  gy_content,.    
-00007c20: 2020 2020 616c 6c6f 6361 7469 6f6e 5f73      allocation_s
-00007c30: 7472 6174 6567 793d 616c 6c6f 6361 7469  trategy=allocati
-00007c40: 6f6e 5f73 7472 6174 6567 792c 0a20 2020  on_strategy,.   
-00007c50: 2029 0a0a 0a64 6566 2065 7874 656e 645f   )...def extend_
-00007c60: 7369 6d75 6c61 7469 6f6e 5f66 726f 6d5f  simulation_from_
-00007c70: 6261 7365 626f 7828 0a20 2020 2062 6173  basebox(.    bas
-00007c80: 6562 6f78 5f69 643a 2073 7472 2c0a 2020  ebox_id: str,.  
-00007c90: 2020 7377 6974 6368 5f6e 616d 653a 2073    switch_name: s
-00007ca0: 7472 2c0a 2020 2020 616c 6c6f 6361 7469  tr,.    allocati
-00007cb0: 6f6e 5f73 7472 6174 6567 793a 204f 7074  on_strategy: Opt
-00007cc0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-00007cd0: 652c 0a20 2020 2069 645f 7369 6d75 6c61  e,.    id_simula
-00007ce0: 7469 6f6e 3a20 696e 7420 3d20 4e6f 6e65  tion: int = None
-00007cf0: 2c0a 2920 2d3e 2069 6e74 3a0a 2020 2020  ,.) -> int:.    
-00007d00: 2222 2245 7874 656e 6420 616e 2065 7869  """Extend an exi
-00007d10: 7374 696e 6720 7369 6d75 6c61 7469 6f6e  sting simulation
-00007d20: 206d 6f64 656c 2069 6e20 6461 7461 6261   model in databa
-00007d30: 7365 2062 6173 6564 206f 6e20 7468 650a  se based on the.
-00007d40: 2020 2020 7072 6f76 6964 6564 2062 6173      provided bas
-00007d50: 6562 6f78 2069 642c 2061 6e64 2070 6c75  ebox id, and plu
-00007d60: 6720 7468 6520 6e65 7720 6e6f 6465 206f  g the new node o
-00007d70: 6620 7468 6520 7370 6563 6966 6564 2073  f the specifed s
-00007d80: 7769 7463 682e 0a0a 2020 2020 2222 220a  witch...    """.
-00007d90: 0a20 2020 2069 6620 6261 7365 626f 785f  .    if basebox_
-00007da0: 6964 2069 7320 4e6f 6e65 3a0a 2020 2020  id is None:.    
-00007db0: 2020 2020 7261 6973 6520 4578 6365 7074      raise Except
-00007dc0: 696f 6e28 2241 2062 6173 6562 6f78 2049  ion("A basebox I
-00007dd0: 4420 6973 2072 6571 7569 7265 6422 290a  D is required").
-00007de0: 0a20 2020 2023 2043 7265 6174 6520 616e  .    # Create an
-00007df0: 2074 6f70 6f6c 6f67 7920 7769 7468 2074   topology with t
-00007e00: 6865 2070 726f 7669 6465 6420 6261 7365  he provided base
-00007e10: 626f 7820 4944 0a20 2020 2074 7279 3a0a  box ID.    try:.
-00007e20: 2020 2020 2020 2020 6261 7365 626f 7820          basebox 
-00007e30: 3d20 6665 7463 685f 6261 7365 626f 7828  = fetch_basebox(
-00007e40: 6261 7365 626f 785f 6964 290a 2020 2020  basebox_id).    
-00007e50: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-00007e60: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
-00007e70: 4578 6365 7074 696f 6e28 0a20 2020 2020  Exception(.     
-00007e80: 2020 2020 2020 2066 2243 616e 6e6f 7420         f"Cannot 
-00007e90: 6669 6e64 2062 6173 6562 6f78 2069 6e20  find basebox in 
-00007ea0: 6461 7461 6261 7365 2066 726f 6d20 6261  database from ba
-00007eb0: 7365 626f 7820 4944 2027 7b62 6173 6562  sebox ID '{baseb
-00007ec0: 6f78 5f69 647d 2722 0a20 2020 2020 2020  ox_id}'".       
-00007ed0: 2029 0a0a 2020 2020 6e6f 6465 5f6e 616d   )..    node_nam
-00007ee0: 6520 3d20 5f67 6574 5f72 616e 646f 6d5f  e = _get_random_
-00007ef0: 7374 7269 6e67 2831 3029 0a20 2020 2072  string(10).    r
-00007f00: 6f6c 6520 3d20 6261 7365 626f 785b 2272  ole = basebox["r
-00007f10: 6f6c 6522 5d0a 2020 2020 6e62 5f70 726f  ole"].    nb_pro
-00007f20: 6320 3d20 6261 7365 626f 785b 226e 625f  c = basebox["nb_
-00007f30: 7072 6f63 225d 0a20 2020 206d 656d 6f72  proc"].    memor
-00007f40: 795f 7369 7a65 203d 2062 6173 6562 6f78  y_size = basebox
-00007f50: 5b22 6d65 6d6f 7279 5f73 697a 6522 5d0a  ["memory_size"].
-00007f60: 0a20 2020 2074 6f70 6f6c 6f67 795f 636f  .    topology_co
-00007f70: 6e74 656e 7420 3d20 7b0a 2020 2020 2020  ntent = {.      
-00007f80: 2020 226e 6f64 6573 223a 205b 0a20 2020    "nodes": [.   
-00007f90: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
-00007fa0: 2020 2020 2020 2020 2020 2022 7479 7065             "type
-00007fb0: 223a 2022 7669 7274 7561 6c5f 6d61 6368  ": "virtual_mach
-00007fc0: 696e 6522 2c0a 2020 2020 2020 2020 2020  ine",.          
-00007fd0: 2020 2020 2020 226e 616d 6522 3a20 6e6f        "name": no
-00007fe0: 6465 5f6e 616d 652c 0a20 2020 2020 2020  de_name,.       
-00007ff0: 2020 2020 2020 2020 2022 6261 7365 626f           "basebo
-00008000: 785f 6964 223a 2062 6173 6562 6f78 5f69  x_id": basebox_i
-00008010: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
-00008020: 2020 2022 6e62 5f70 726f 6322 3a20 6e62     "nb_proc": nb
-00008030: 5f70 726f 632c 0a20 2020 2020 2020 2020  _proc,.         
-00008040: 2020 2020 2020 2022 6d65 6d6f 7279 5f73         "memory_s
-00008050: 697a 6522 3a20 6d65 6d6f 7279 5f73 697a  ize": memory_siz
-00008060: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00008070: 2020 2022 726f 6c65 7322 3a20 5b72 6f6c     "roles": [rol
-00008080: 655d 2c0a 2020 2020 2020 2020 2020 2020  e],.            
-00008090: 7d0a 2020 2020 2020 2020 5d2c 0a20 2020  }.        ],.   
-000080a0: 2020 2020 2022 6c69 6e6b 7322 3a20 5b0a       "links": [.
-000080b0: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
-000080c0: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-000080d0: 7769 7463 6822 3a20 7b22 7479 7065 223a  witch": {"type":
-000080e0: 2022 7377 6974 6368 222c 2022 6e61 6d65   "switch", "name
-000080f0: 223a 2073 7769 7463 685f 6e61 6d65 7d2c  ": switch_name},
-00008100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008110: 2022 6e6f 6465 223a 207b 0a20 2020 2020   "node": {.     
-00008120: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00008130: 7479 7065 223a 2022 7669 7274 7561 6c5f  type": "virtual_
-00008140: 6d61 6368 696e 6522 2c0a 2020 2020 2020  machine",.      
-00008150: 2020 2020 2020 2020 2020 2020 2020 226e                "n
-00008160: 616d 6522 3a20 6e6f 6465 5f6e 616d 652c  ame": node_name,
-00008170: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008180: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
-00008190: 2020 2020 2270 6172 616d 7322 3a20 7b7d      "params": {}
-000081a0: 2c20 2023 2044 796e 616d 6963 2049 5020  ,  # Dynamic IP 
-000081b0: 6164 6472 6573 730a 2020 2020 2020 2020  address.        
-000081c0: 2020 2020 7d0a 2020 2020 2020 2020 5d2c      }.        ],
-000081d0: 0a20 2020 207d 0a0a 2020 2020 7265 7475  .    }..    retu
-000081e0: 726e 2065 7874 656e 645f 7369 6d75 6c61  rn extend_simula
-000081f0: 7469 6f6e 280a 2020 2020 2020 2020 746f  tion(.        to
-00008200: 706f 6c6f 6779 5f63 6f6e 7465 6e74 3d74  pology_content=t
-00008210: 6f70 6f6c 6f67 795f 636f 6e74 656e 742c  opology_content,
-00008220: 0a20 2020 2020 2020 2061 6c6c 6f63 6174  .        allocat
-00008230: 696f 6e5f 7374 7261 7465 6779 3d61 6c6c  ion_strategy=all
-00008240: 6f63 6174 696f 6e5f 7374 7261 7465 6779  ocation_strategy
-00008250: 2c0a 2020 2020 2020 2020 6964 5f73 696d  ,.        id_sim
-00008260: 756c 6174 696f 6e3d 6964 5f73 696d 756c  ulation=id_simul
-00008270: 6174 696f 6e2c 0a20 2020 2029 0a0a 0a23  ation,.    )...#
-00008280: 2323 0a23 2054 6f70 6f6c 6f67 7920 6865  ##.# Topology he
-00008290: 6c70 6572 730a 2323 230a 0a0a 6465 6620  lpers.###...def 
-000082a0: 746f 706f 6c6f 6779 5f66 696c 655f 6164  topology_file_ad
-000082b0: 645f 7765 6273 6974 6573 280a 2020 2020  d_websites(.    
-000082c0: 746f 706f 6c6f 6779 5f66 696c 653a 2073  topology_file: s
-000082d0: 7472 2c20 7765 6273 6974 6573 3a20 4c69  tr, websites: Li
-000082e0: 7374 5b73 7472 5d2c 2073 7769 7463 685f  st[str], switch_
-000082f0: 6e61 6d65 3a20 7374 720a 2920 2d3e 2073  name: str.) -> s
-00008300: 7472 3a0a 2020 2020 2222 2241 6464 2064  tr:.    """Add d
-00008310: 6f63 6b65 7220 7765 6273 6974 6573 206e  ocker websites n
-00008320: 6f64 6520 746f 2061 2067 6976 656e 2074  ode to a given t
-00008330: 6f70 6f6c 6f67 792c 2061 6e64 2072 6574  opology, and ret
-00008340: 7572 6e20 7468 6520 7570 6461 7465 6420  urn the updated 
-00008350: 746f 706f 6c6f 6779 2e22 2222 0a0a 2020  topology."""..  
-00008360: 2020 2320 5661 6c69 6461 7465 2059 414d    # Validate YAM
-00008370: 4c20 746f 706f 6c6f 6779 2066 696c 650a  L topology file.
-00008380: 2020 2020 5f76 616c 6964 6174 655f 7961      _validate_ya
-00008390: 6d6c 5f74 6f70 6f6c 6f67 795f 6669 6c65  ml_topology_file
-000083a0: 2874 6f70 6f6c 6f67 795f 6669 6c65 290a  (topology_file).
-000083b0: 0a20 2020 2023 204f 7065 6e20 616e 6420  .    # Open and 
-000083c0: 7265 6164 2059 414d 4c20 746f 706f 6c6f  read YAML topolo
-000083d0: 6779 2066 696c 650a 2020 2020 746f 706f  gy file.    topo
-000083e0: 6c6f 6779 5f79 616d 6c20 3d20 5f72 6561  logy_yaml = _rea
-000083f0: 645f 7961 6d6c 5f74 6f70 6f6c 6f67 795f  d_yaml_topology_
-00008400: 6669 6c65 2874 6f70 6f6c 6f67 795f 6669  file(topology_fi
-00008410: 6c65 290a 0a20 2020 2023 2055 7064 6174  le)..    # Updat
-00008420: 6520 746f 706f 6c6f 6779 2077 6974 6820  e topology with 
-00008430: 7468 6520 4150 490a 2020 2020 746f 706f  the API.    topo
-00008440: 6c6f 6779 5f79 616d 6c20 3d20 746f 706f  logy_yaml = topo
-00008450: 6c6f 6779 5f61 6464 5f77 6562 7369 7465  logy_add_website
-00008460: 7328 746f 706f 6c6f 6779 5f79 616d 6c2c  s(topology_yaml,
-00008470: 2077 6562 7369 7465 732c 2073 7769 7463   websites, switc
-00008480: 685f 6e61 6d65 290a 0a20 2020 2072 6574  h_name)..    ret
-00008490: 7572 6e20 746f 706f 6c6f 6779 5f79 616d  urn topology_yam
-000084a0: 6c0a 0a0a 6465 6620 746f 706f 6c6f 6779  l...def topology
-000084b0: 5f66 696c 655f 6164 645f 6467 6128 0a20  _file_add_dga(. 
-000084c0: 2020 2074 6f70 6f6c 6f67 795f 6669 6c65     topology_file
-000084d0: 3a20 7374 722c 0a20 2020 2061 6c67 6f72  : str,.    algor
-000084e0: 6974 686d 3a20 7374 722c 0a20 2020 2073  ithm: str,.    s
-000084f0: 7769 7463 685f 6e61 6d65 3a20 7374 722c  witch_name: str,
-00008500: 0a20 2020 206e 756d 6265 723a 2069 6e74  .    number: int
-00008510: 2c0a 2020 2020 7265 736f 7572 6365 735f  ,.    resources_
-00008520: 6469 723a 2073 7472 2c0a 2920 2d3e 2028  dir: str,.) -> (
-00008530: 7374 722c 204c 6973 745b 7374 725d 293a  str, List[str]):
-00008540: 0a20 2020 2022 2222 4164 6420 646f 636b  .    """Add dock
-00008550: 6572 2065 6d70 7479 2077 6562 7369 7465  er empty website
-00008560: 7320 6e6f 6465 2077 6974 6820 4447 4120  s node with DGA 
-00008570: 746f 2061 2067 6976 656e 2074 6f70 6f6c  to a given topol
-00008580: 6f67 792c 2061 6e64 2072 6574 7572 6e20  ogy, and return 
-00008590: 7468 6520 7570 6461 7465 6420 746f 706f  the updated topo
-000085a0: 6c6f 6779 2e22 2222 0a0a 2020 2020 2320  logy."""..    # 
-000085b0: 5661 6c69 6461 7465 0a0a 2020 2020 2320  Validate..    # 
-000085c0: 5661 6c69 6461 7465 2059 414d 4c20 746f  Validate YAML to
-000085d0: 706f 6c6f 6779 2066 696c 650a 2020 2020  pology file.    
-000085e0: 5f76 616c 6964 6174 655f 7961 6d6c 5f74  _validate_yaml_t
-000085f0: 6f70 6f6c 6f67 795f 6669 6c65 2874 6f70  opology_file(top
-00008600: 6f6c 6f67 795f 6669 6c65 290a 0a20 2020  ology_file)..   
-00008610: 2023 204f 7065 6e20 616e 6420 7265 6164   # Open and read
-00008620: 2059 414d 4c20 746f 706f 6c6f 6779 2066   YAML topology f
-00008630: 696c 650a 2020 2020 746f 706f 6c6f 6779  ile.    topology
-00008640: 5f79 616d 6c20 3d20 5f72 6561 645f 7961  _yaml = _read_ya
-00008650: 6d6c 5f74 6f70 6f6c 6f67 795f 6669 6c65  ml_topology_file
-00008660: 2874 6f70 6f6c 6f67 795f 6669 6c65 290a  (topology_file).
-00008670: 0a20 2020 2023 2055 7064 6174 6520 746f  .    # Update to
-00008680: 706f 6c6f 6779 2077 6974 6820 7468 6520  pology with the 
-00008690: 4150 490a 2020 2020 2874 6f70 6f6c 6f67  API.    (topolog
-000086a0: 795f 7961 6d6c 2c20 646f 6d61 696e 7329  y_yaml, domains)
-000086b0: 203d 2074 6f70 6f6c 6f67 795f 6164 645f   = topology_add_
-000086c0: 6467 6128 0a20 2020 2020 2020 2074 6f70  dga(.        top
-000086d0: 6f6c 6f67 795f 7961 6d6c 2c20 616c 676f  ology_yaml, algo
-000086e0: 7269 7468 6d2c 2073 7769 7463 685f 6e61  rithm, switch_na
-000086f0: 6d65 2c20 6e75 6d62 6572 2c20 7265 736f  me, number, reso
-00008700: 7572 6365 735f 6469 720a 2020 2020 290a  urces_dir.    ).
-00008710: 0a20 2020 2072 6574 7572 6e20 746f 706f  .    return topo
-00008720: 6c6f 6779 5f79 616d 6c2c 2064 6f6d 6169  logy_yaml, domai
-00008730: 6e73 0a0a 0a64 6566 2074 6f70 6f6c 6f67  ns...def topolog
-00008740: 795f 6669 6c65 5f61 6464 5f64 6e73 5f73  y_file_add_dns_s
-00008750: 6572 7665 7228 0a20 2020 2074 6f70 6f6c  erver(.    topol
-00008760: 6f67 795f 6669 6c65 3a20 7374 722c 0a20  ogy_file: str,. 
-00008770: 2020 2073 7769 7463 685f 6e61 6d65 3a20     switch_name: 
-00008780: 7374 722c 0a20 2020 2072 6573 6f75 7263  str,.    resourc
-00008790: 6573 5f64 6972 3a20 7374 722c 0a29 202d  es_dir: str,.) -
-000087a0: 3e20 2873 7472 2c20 7374 7229 3a0a 2020  > (str, str):.  
-000087b0: 2020 2222 2241 6464 2061 2044 4e53 2073    """Add a DNS s
-000087c0: 6572 7665 7220 746f 2061 2059 414d 4c20  erver to a YAML 
-000087d0: 746f 706f 6c6f 6779 2e0a 2020 2020 5265  topology..    Re
-000087e0: 7475 726e 7320 7468 6520 7570 6461 7465  turns the update
-000087f0: 6420 746f 706f 6c6f 6779 2061 6e64 2074  d topology and t
-00008800: 6865 2063 6f6e 7465 6e74 206f 6620 7468  he content of th
-00008810: 6520 444e 5320 636f 6e66 6967 7572 6174  e DNS configurat
-00008820: 696f 6e20 6669 6c65 2e22 2222 0a0a 2020  ion file."""..  
-00008830: 2020 2320 5661 6c69 6461 7465 0a0a 2020    # Validate..  
-00008840: 2020 2320 5661 6c69 6461 7465 2059 414d    # Validate YAM
-00008850: 4c20 746f 706f 6c6f 6779 2066 696c 650a  L topology file.
-00008860: 2020 2020 5f76 616c 6964 6174 655f 7961      _validate_ya
-00008870: 6d6c 5f74 6f70 6f6c 6f67 795f 6669 6c65  ml_topology_file
-00008880: 2874 6f70 6f6c 6f67 795f 6669 6c65 290a  (topology_file).
-00008890: 0a20 2020 2023 204f 7065 6e20 616e 6420  .    # Open and 
-000088a0: 7265 6164 2059 414d 4c20 746f 706f 6c6f  read YAML topolo
-000088b0: 6779 2066 696c 650a 2020 2020 746f 706f  gy file.    topo
-000088c0: 6c6f 6779 5f79 616d 6c20 3d20 5f72 6561  logy_yaml = _rea
-000088d0: 645f 7961 6d6c 5f74 6f70 6f6c 6f67 795f  d_yaml_topology_
-000088e0: 6669 6c65 2874 6f70 6f6c 6f67 795f 6669  file(topology_fi
-000088f0: 6c65 290a 0a20 2020 2023 2055 7064 6174  le)..    # Updat
-00008900: 6520 746f 706f 6c6f 6779 2077 6974 6820  e topology with 
-00008910: 7468 6520 4150 490a 2020 2020 2874 6f70  the API.    (top
-00008920: 6f6c 6f67 795f 7961 6d6c 2c20 646e 735f  ology_yaml, dns_
-00008930: 636f 6e66 5f63 6f6e 7465 6e74 2920 3d20  conf_content) = 
-00008940: 746f 706f 6c6f 6779 5f61 6464 5f64 6e73  topology_add_dns
-00008950: 5f73 6572 7665 7228 0a20 2020 2020 2020  _server(.       
-00008960: 2074 6f70 6f6c 6f67 795f 7961 6d6c 2c20   topology_yaml, 
-00008970: 7377 6974 6368 5f6e 616d 652c 2072 6573  switch_name, res
-00008980: 6f75 7263 6573 5f64 6972 0a20 2020 2029  ources_dir.    )
-00008990: 0a0a 2020 2020 7265 7475 726e 2074 6f70  ..    return top
-000089a0: 6f6c 6f67 795f 7961 6d6c 2c20 646e 735f  ology_yaml, dns_
-000089b0: 636f 6e66 5f63 6f6e 7465 6e74 0a0a 0a23  conf_content...#
-000089c0: 2323 0a23 2042 6173 6562 6f78 2068 656c  ##.# Basebox hel
-000089d0: 7065 7273 0a23 2323 0a0a 0a64 6566 205f  pers.###...def _
-000089e0: 7261 6973 655f 6572 726f 725f 6d73 6728  raise_error_msg(
-000089f0: 7265 7375 6c74 3a20 6469 6374 2920 2d3e  result: dict) ->
-00008a00: 204e 6f6e 653a 0a20 2020 2022 2222 0a20   None:.    """. 
-00008a10: 2020 2052 6169 7365 2061 6e20 6572 726f     Raise an erro
-00008a20: 7220 6d65 7373 6167 6520 6966 2061 2074  r message if a t
-00008a30: 6173 6b20 2865 6720 7468 6520 6261 7365  ask (eg the base
-00008a40: 626f 7820 7665 7269 6669 6361 7469 6f6e  box verification
-00008a50: 2920 6661 696c 6564 0a20 2020 203a 7061  ) failed.    :pa
-00008a60: 7261 6d20 7265 7375 6c74 3a20 7468 6520  ram result: the 
-00008a70: 7265 7375 6c74 206f 6620 7468 6520 7461  result of the ta
-00008a80: 736b 0a20 2020 203a 7265 7475 726e 3a20  sk.    :return: 
-00008a90: 4e6f 6e65 0a20 2020 2022 2222 0a20 2020  None.    """.   
-00008aa0: 2065 7272 6f72 5f6d 7367 203d 2022 4e6f   error_msg = "No
-00008ab0: 2065 7272 6f72 206d 6573 7361 6765 2072   error message r
-00008ac0: 6574 7572 6e65 6422 0a20 2020 2069 6620  eturned".    if 
-00008ad0: 2272 6573 756c 7422 2069 6e20 7265 7375  "result" in resu
-00008ae0: 6c74 3a0a 2020 2020 2020 2020 6966 2022  lt:.        if "
-00008af0: 6572 726f 725f 6d73 6722 2069 6e20 7265  error_msg" in re
-00008b00: 7375 6c74 5b22 7265 7375 6c74 225d 3a0a  sult["result"]:.
-00008b10: 2020 2020 2020 2020 2020 2020 6572 726f              erro
-00008b20: 725f 6d73 6720 3d20 7265 7375 6c74 5b22  r_msg = result["
-00008b30: 7265 7375 6c74 225d 5b22 6572 726f 725f  result"]["error_
-00008b40: 6d73 6722 5d0a 2020 2020 2020 2020 7261  msg"].        ra
-00008b50: 6973 6520 4578 6365 7074 696f 6e28 6572  ise Exception(er
-00008b60: 726f 725f 6d73 6729 0a20 2020 2065 6c73  ror_msg).    els
-00008b70: 653a 0a20 2020 2020 2020 2072 6169 7365  e:.        raise
-00008b80: 2045 7863 6570 7469 6f6e 2866 224e 6f20   Exception(f"No 
-00008b90: 2772 6573 756c 7427 206b 6579 2069 6e20  'result' key in 
-00008ba0: 7265 7375 6c74 3a20 7b72 6573 756c 747d  result: {result}
-00008bb0: 2229 0a0a 0a64 6566 205f 5f62 6173 6562  ")...def __baseb
-00008bc0: 6f78 6573 5f76 6572 6966 6963 6174 696f  oxes_verificatio
-00008bd0: 6e5f 7761 6974 5f75 6e74 696c 5f63 6f6d  n_wait_until_com
-00008be0: 706c 6574 6528 0a20 2020 2074 6173 6b5f  plete(.    task_
-00008bf0: 6964 3a20 7374 722c 206c 6f67 5f73 7566  id: str, log_suf
-00008c00: 6669 783a 2073 7472 203d 204e 6f6e 652c  fix: str = None,
-00008c10: 2074 696d 656f 7574 3a20 696e 7420 3d20   timeout: int = 
-00008c20: 3336 3030 0a29 202d 3e20 6469 6374 3a0a  3600.) -> dict:.
-00008c30: 2020 2020 2222 220a 2020 2020 5761 6974      """.    Wait
-00008c40: 2075 6e74 696c 2074 6865 2076 6572 6966   until the verif
-00008c50: 6963 6174 696f 6e20 7461 736b 2072 6570  ication task rep
-00008c60: 7265 7365 6e74 696e 6720 6279 2069 7473  resenting by its
-00008c70: 2069 6420 6973 2063 6f6d 706c 6574 6564   id is completed
-00008c80: 0a20 2020 203a 7061 7261 6d20 7461 736b  .    :param task
-00008c90: 5f69 643a 2074 6865 2074 6173 6b20 6964  _id: the task id
-00008ca0: 0a20 2020 203a 7061 7261 6d20 6c6f 675f  .    :param log_
-00008cb0: 7375 6666 6978 3a20 7768 6174 2074 6f20  suffix: what to 
-00008cc0: 696e 7365 7274 2069 6e74 6f20 7468 6520  insert into the 
-00008cd0: 6c6f 670a 2020 2020 3a70 6172 616d 2074  log.    :param t
-00008ce0: 696d 656f 7574 3a20 7468 6520 7469 6d65  imeout: the time
-00008cf0: 6f75 7420 746f 2073 746f 7020 7468 6520  out to stop the 
-00008d00: 7461 736b 0a20 2020 203a 7265 7475 726e  task.    :return
-00008d10: 3a20 7468 6520 7265 7375 6c74 206f 6620  : the result of 
-00008d20: 7468 6520 6261 7365 626f 7820 7665 7269  the basebox veri
-00008d30: 6669 6361 7469 6f6e 0a20 2020 2022 2222  fication.    """
-00008d40: 0a0a 2020 2020 7374 6172 745f 7469 6d65  ..    start_time
-00008d50: 203d 2074 696d 652e 7469 6d65 2829 0a0a   = time.time()..
-00008d60: 2020 2020 6669 6e69 7368 6564 203d 2046      finished = F
-00008d70: 616c 7365 0a20 2020 2077 6869 6c65 206e  alse.    while n
-00008d80: 6f74 2028 6669 6e69 7368 6564 206f 7220  ot (finished or 
-00008d90: 2874 696d 652e 7469 6d65 2829 202d 2073  (time.time() - s
-00008da0: 7461 7274 5f74 696d 6529 203e 2074 696d  tart_time) > tim
-00008db0: 656f 7574 293a 0a20 2020 2020 2020 2074  eout):.        t
-00008dc0: 696d 652e 736c 6565 7028 3229 0a20 2020  ime.sleep(2).   
-00008dd0: 2020 2020 2063 7572 7265 6e74 5f74 696d       current_tim
-00008de0: 6520 3d20 7469 6d65 2e74 696d 6528 290a  e = time.time().
-00008df0: 2020 2020 2020 2020 656c 6170 7365 6420          elapsed 
-00008e00: 3d20 696e 7428 6375 7272 656e 745f 7469  = int(current_ti
-00008e10: 6d65 202d 2073 7461 7274 5f74 696d 6529  me - start_time)
-00008e20: 0a20 2020 2020 2020 2069 6620 6c6f 675f  .        if log_
-00008e30: 7375 6666 6978 2069 7320 6e6f 7420 4e6f  suffix is not No
-00008e40: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00008e50: 6c6f 6767 6572 2e69 6e66 6f28 0a20 2020  logger.info(.   
-00008e60: 2020 2020 2020 2020 2020 2020 2066 2220               f" 
-00008e70: 2020 5b2b 5d20 4375 7272 656e 746c 7920    [+] Currently 
-00008e80: 7665 7269 6679 696e 6720 7b6c 6f67 5f73  verifying {log_s
-00008e90: 7566 6669 787d 2066 6f72 207b 656c 6170  uffix} for {elap
-00008ea0: 7365 647d 2073 6563 6f6e 6473 2028 7469  sed} seconds (ti
-00008eb0: 6d65 6f75 7420 6174 207b 7469 6d65 6f75  meout at {timeou
-00008ec0: 747d 2073 6563 6f6e 6473 2922 0a20 2020  t} seconds)".   
-00008ed0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00008ee0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00008ef0: 2020 2020 206c 6f67 6765 722e 696e 666f       logger.info
-00008f00: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00008f10: 2020 6622 2020 205b 2b5d 2043 7572 7265    f"   [+] Curre
-00008f20: 6e74 6c79 2072 756e 6e69 6e67 2074 6865  ntly running the
-00008f30: 2076 6572 6966 6963 6174 696f 6e20 666f   verification fo
-00008f40: 7220 7b65 6c61 7073 6564 7d20 7365 636f  r {elapsed} seco
-00008f50: 6e64 7322 0a20 2020 2020 2020 2020 2020  nds".           
-00008f60: 2029 0a0a 2020 2020 2020 2020 7265 7375   )..        resu
-00008f70: 6c74 203d 205f 706f 7374 2822 2f62 6173  lt = _post("/bas
-00008f80: 6562 6f78 2f73 7461 7475 735f 7665 7269  ebox/status_veri
-00008f90: 6679 222c 2064 6174 613d 7b22 7461 736b  fy", data={"task
-00008fa0: 5f69 6422 3a20 7461 736b 5f69 647d 290a  _id": task_id}).
-00008fb0: 2020 2020 2020 2020 7265 7375 6c74 2e72          result.r
-00008fc0: 6169 7365 5f66 6f72 5f73 7461 7475 7328  aise_for_status(
-00008fd0: 290a 2020 2020 2020 2020 7265 7375 6c74  ).        result
-00008fe0: 203d 2072 6573 756c 742e 6a73 6f6e 2829   = result.json()
-00008ff0: 0a0a 2020 2020 2020 2020 6966 2022 7374  ..        if "st
-00009000: 6174 7573 2220 696e 2072 6573 756c 743a  atus" in result:
-00009010: 0a20 2020 2020 2020 2020 2020 2063 7572  .            cur
-00009020: 7265 6e74 5f73 7461 7475 7320 3d20 7265  rent_status = re
-00009030: 7375 6c74 5b22 7374 6174 7573 225d 0a0a  sult["status"]..
-00009040: 2020 2020 2020 2020 2020 2020 6966 2063              if c
-00009050: 7572 7265 6e74 5f73 7461 7475 7320 3d3d  urrent_status ==
-00009060: 2022 4552 524f 5222 3a0a 2020 2020 2020   "ERROR":.      
-00009070: 2020 2020 2020 2020 2020 6572 726f 725f            error_
-00009080: 6d65 7373 6167 6520 3d20 7265 7375 6c74  message = result
-00009090: 5b22 6572 726f 725f 6d73 6722 5d0a 2020  ["error_msg"].  
-000090a0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-000090b0: 6973 6520 4578 6365 7074 696f 6e28 0a20  ise Exception(. 
-000090c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000090d0: 2020 2066 2245 7272 6f72 2064 7572 696e     f"Error durin
-000090e0: 6720 7665 7269 6669 6361 7469 6f6e 206f  g verification o
-000090f0: 7065 7261 7469 6f6e 3a20 277b 6572 726f  peration: '{erro
-00009100: 725f 6d65 7373 6167 657d 2722 0a20 2020  r_message}'".   
-00009110: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00009120: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00009130: 6375 7272 656e 745f 7374 6174 7573 203d  current_status =
-00009140: 3d20 2246 494e 4953 4845 4422 3a0a 2020  = "FINISHED":.  
-00009150: 2020 2020 2020 2020 2020 2020 2020 6669                fi
-00009160: 6e69 7368 6564 203d 2054 7275 650a 0a20  nished = True.. 
-00009170: 2020 2069 6620 6e6f 7420 6669 6e69 7368     if not finish
-00009180: 6564 3a0a 2020 2020 2020 2020 6572 726f  ed:.        erro
-00009190: 725f 6d73 6720 3d20 6622 5b2d 5d20 556e  r_msg = f"[-] Un
-000091a0: 6162 6c65 2074 6f20 7465 726d 696e 6174  able to terminat
-000091b0: 6520 6f70 6572 6174 696f 6e20 6265 666f  e operation befo
-000091c0: 7265 2074 696d 656f 7574 206f 6620 7b74  re timeout of {t
-000091d0: 696d 656f 7574 7d20 7365 636f 6e64 732e  imeout} seconds.
-000091e0: 2053 746f 7070 696e 6720 6f70 6572 6174   Stopping operat
-000091f0: 696f 6e2e 220a 2020 2020 2020 2020 7265  ion.".        re
-00009200: 7375 6c74 203d 2076 6572 6966 795f 6261  sult = verify_ba
-00009210: 7365 626f 785f 7374 6f70 2874 6173 6b5f  sebox_stop(task_
-00009220: 6964 290a 2020 2020 2020 2020 7374 6f70  id).        stop
-00009230: 7065 6420 3d20 7265 7375 6c74 5b22 7374  ped = result["st
-00009240: 6174 7573 225d 203d 3d20 2253 544f 5050  atus"] == "STOPP
-00009250: 4544 220a 2020 2020 2020 2020 6966 2073  ED".        if s
-00009260: 746f 7070 6564 3a0a 2020 2020 2020 2020  topped:.        
-00009270: 2020 2020 7265 7375 6c74 5b22 7265 7375      result["resu
-00009280: 6c74 225d 203d 2064 6963 7428 290a 2020  lt"] = dict().  
-00009290: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-000092a0: 5b22 7265 7375 6c74 225d 5b22 6572 726f  ["result"]["erro
-000092b0: 725f 6d73 6722 5d20 3d20 6572 726f 725f  r_msg"] = error_
-000092c0: 6d73 670a 2020 2020 2020 2020 2020 2020  msg.            
-000092d0: 7265 7475 726e 2072 6573 756c 740a 2020  return result.  
-000092e0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-000092f0: 2020 2020 2020 2020 7261 6973 6520 4578          raise Ex
-00009300: 6365 7074 696f 6e28 2255 6e61 626c 6520  ception("Unable 
-00009310: 746f 2073 746f 7020 7665 7269 6669 6361  to stop verifica
-00009320: 7469 6f6e 2074 6173 6b22 290a 0a20 2020  tion task")..   
-00009330: 2072 6573 756c 7420 3d20 5f70 6f73 7428   result = _post(
-00009340: 222f 6261 7365 626f 782f 7265 7375 6c74  "/basebox/result
-00009350: 5f76 6572 6966 7922 2c20 6461 7461 3d7b  _verify", data={
-00009360: 2274 6173 6b5f 6964 223a 2074 6173 6b5f  "task_id": task_
-00009370: 6964 7d29 0a20 2020 2072 6573 756c 742e  id}).    result.
-00009380: 7261 6973 655f 666f 725f 7374 6174 7573  raise_for_status
-00009390: 2829 0a20 2020 2072 6573 756c 7420 3d20  ().    result = 
-000093a0: 7265 7375 6c74 2e6a 736f 6e28 290a 0a20  result.json().. 
-000093b0: 2020 2073 7563 6365 7373 203d 2072 6573     success = res
-000093c0: 756c 745b 2273 7461 7475 7322 5d20 3d3d  ult["status"] ==
-000093d0: 2022 4649 4e49 5348 4544 2220 616e 6420   "FINISHED" and 
-000093e0: 7265 7375 6c74 5b22 7265 7375 6c74 225d  result["result"]
-000093f0: 5b22 7375 6363 6573 7322 5d20 6973 2054  ["success"] is T
-00009400: 7275 650a 0a20 2020 2069 6620 6e6f 7420  rue..    if not 
-00009410: 7375 6363 6573 733a 0a20 2020 2020 2020  success:.       
-00009420: 2065 7272 6f72 5f6d 7367 203d 2072 6573   error_msg = res
-00009430: 756c 745b 2272 6573 756c 7422 5d5b 2265  ult["result"]["e
-00009440: 7272 6f72 5f6d 7367 225d 0a20 2020 2020  rror_msg"].     
-00009450: 2020 206c 6f67 6765 722e 6572 726f 7228     logger.error(
-00009460: 0a20 2020 2020 2020 2020 2020 2066 225b  .            f"[
-00009470: 2d5d 2054 6865 2062 6173 6562 6f78 2076  -] The basebox v
-00009480: 6572 6966 6963 6174 696f 6e20 7761 7320  erification was 
-00009490: 6578 6563 7574 6564 2077 6974 6820 6572  executed with er
-000094a0: 726f 723a 207b 6572 726f 725f 6d73 677d  ror: {error_msg}
-000094b0: 220a 2020 2020 2020 2020 290a 0a20 2020  ".        )..   
-000094c0: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
-000094d0: 0a64 6566 205f 5f77 6169 745f 666f 725f  .def __wait_for_
-000094e0: 7468 655f 6f70 6572 6174 696f 6e5f 746f  the_operation_to
-000094f0: 5f73 7461 7274 2874 6173 6b5f 6964 3a20  _start(task_id: 
-00009500: 7374 7229 202d 3e20 626f 6f6c 3a0a 2020  str) -> bool:.  
-00009510: 2020 2222 220a 2020 2020 5761 6974 2066    """.    Wait f
-00009520: 6f72 2061 2074 6173 6b20 746f 2073 7461  or a task to sta
-00009530: 7274 0a20 2020 203a 7061 7261 6d20 7461  rt.    :param ta
-00009540: 736b 5f69 643a 2074 6865 2074 6173 6b20  sk_id: the task 
-00009550: 6964 0a20 2020 203a 7265 7475 726e 3a20  id.    :return: 
-00009560: 4973 2074 6865 2074 6173 6b20 7275 6e6e  Is the task runn
-00009570: 696e 670a 2020 2020 2222 220a 0a20 2020  ing.    """..   
-00009580: 2072 756e 6e69 6e67 203d 2046 616c 7365   running = False
-00009590: 0a20 2020 2074 696d 656f 7574 203d 2031  .    timeout = 1
-000095a0: 300a 2020 2020 7374 6172 745f 7469 6d65  0.    start_time
-000095b0: 203d 2074 696d 652e 7469 6d65 2829 0a20   = time.time(). 
-000095c0: 2020 2077 6869 6c65 206e 6f74 2028 7275     while not (ru
-000095d0: 6e6e 696e 6720 6f72 2028 7469 6d65 2e74  nning or (time.t
-000095e0: 696d 6528 2920 2d20 7374 6172 745f 7469  ime() - start_ti
-000095f0: 6d65 2920 3e20 7469 6d65 6f75 7429 3a0a  me) > timeout):.
-00009600: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-00009610: 205f 706f 7374 2822 2f62 6173 6562 6f78   _post("/basebox
-00009620: 2f73 7461 7475 735f 7665 7269 6679 222c  /status_verify",
-00009630: 2064 6174 613d 7b22 7461 736b 5f69 6422   data={"task_id"
-00009640: 3a20 7461 736b 5f69 647d 290a 2020 2020  : task_id}).    
-00009650: 2020 2020 7265 7375 6c74 2e72 6169 7365      result.raise
-00009660: 5f66 6f72 5f73 7461 7475 7328 290a 2020  _for_status().  
-00009670: 2020 2020 2020 7265 7375 6c74 203d 2072        result = r
-00009680: 6573 756c 742e 6a73 6f6e 2829 0a20 2020  esult.json().   
-00009690: 2020 2020 2072 756e 6e69 6e67 203d 2072       running = r
-000096a0: 6573 756c 745b 2273 7461 7475 7322 5d20  esult["status"] 
-000096b0: 3d3d 2022 5255 4e4e 494e 4722 0a20 2020  == "RUNNING".   
-000096c0: 2020 2020 2074 696d 652e 736c 6565 7028       time.sleep(
-000096d0: 3129 0a0a 2020 2020 6966 206e 6f74 2072  1)..    if not r
-000096e0: 756e 6e69 6e67 3a0a 2020 2020 2020 2020  unning:.        
-000096f0: 6c6f 6767 6572 2e65 7272 6f72 280a 2020  logger.error(.  
-00009700: 2020 2020 2020 2020 2020 6622 5b2d 5d20            f"[-] 
-00009710: 556e 6162 6c65 2074 6f20 7374 6172 7420  Unable to start 
-00009720: 6f70 6572 6174 696f 6e20 6265 666f 7265  operation before
-00009730: 2074 696d 656f 7574 206f 6620 7b74 696d   timeout of {tim
-00009740: 656f 7574 7d20 7365 636f 6e64 7322 0a20  eout} seconds". 
-00009750: 2020 2020 2020 2029 0a0a 2020 2020 7265         )..    re
-00009760: 7475 726e 2072 756e 6e69 6e67 0a0a 0a64  turn running...d
-00009770: 6566 205f 5f68 616e 646c 655f 7761 6974  ef __handle_wait
-00009780: 280a 2020 2020 7761 6974 3a20 626f 6f6c  (.    wait: bool
-00009790: 2c20 7461 736b 5f69 643a 2073 7472 2c20  , task_id: str, 
-000097a0: 6c6f 675f 7375 6666 6978 3a20 7374 722c  log_suffix: str,
-000097b0: 2074 696d 656f 7574 3a20 696e 7420 3d20   timeout: int = 
-000097c0: 3336 3030 0a29 202d 3e20 626f 6f6c 3a0a  3600.) -> bool:.
-000097d0: 2020 2020 2222 220a 0a20 2020 203a 7061      """..    :pa
-000097e0: 7261 6d20 7761 6974 3a20 5761 6974 2066  ram wait: Wait f
-000097f0: 6f72 2074 6865 206f 7065 7261 7469 6f6e  or the operation
-00009800: 2074 6f20 6265 2063 6f6d 706c 6574 6564   to be completed
-00009810: 2069 6e20 6261 636b 656e 640a 2020 2020   in backend.    
-00009820: 3a70 6172 616d 2074 6173 6b5f 6964 3a20  :param task_id: 
-00009830: 7468 6520 7461 736b 2069 640a 2020 2020  the task id.    
-00009840: 3a70 6172 616d 206c 6f67 5f73 7566 6669  :param log_suffi
-00009850: 783a 2074 6865 2073 7472 696e 6720 746f  x: the string to
-00009860: 2062 6520 696e 7365 7274 6564 2069 6e20   be inserted in 
-00009870: 7468 6520 6c6f 670a 2020 2020 3a70 6172  the log.    :par
-00009880: 616d 2074 696d 656f 7574 3a20 7468 6520  am timeout: the 
-00009890: 7469 6d65 206c 696d 6974 2062 6566 6f72  time limit befor
-000098a0: 6520 7374 6f70 7069 6e67 2074 6865 2074  e stopping the t
-000098b0: 6173 6b0a 2020 2020 3a72 6574 7572 6e3a  ask.    :return:
-000098c0: 2074 6865 2072 6573 756c 7420 6f66 2074   the result of t
-000098d0: 6865 2076 6572 6966 6963 6174 696f 6e0a  he verification.
-000098e0: 2020 2020 2222 220a 2020 2020 7375 6363      """.    succ
-000098f0: 6573 7320 3d20 5472 7565 0a0a 2020 2020  ess = True..    
-00009900: 6966 2077 6169 743a 0a20 2020 2020 2020  if wait:.       
-00009910: 2023 2057 6169 7420 666f 7220 7468 6520   # Wait for the 
-00009920: 6f70 6572 6174 696f 6e20 746f 2062 6520  operation to be 
-00009930: 636f 6d70 6c65 7465 6420 696e 2062 6163  completed in bac
-00009940: 6b65 6e64 0a0a 2020 2020 2020 2020 7265  kend..        re
-00009950: 7375 6c74 203d 205f 5f62 6173 6562 6f78  sult = __basebox
-00009960: 6573 5f76 6572 6966 6963 6174 696f 6e5f  es_verification_
-00009970: 7761 6974 5f75 6e74 696c 5f63 6f6d 706c  wait_until_compl
-00009980: 6574 6528 0a20 2020 2020 2020 2020 2020  ete(.           
-00009990: 2074 6173 6b5f 6964 3d74 6173 6b5f 6964   task_id=task_id
-000099a0: 2c20 6c6f 675f 7375 6666 6978 3d6c 6f67  , log_suffix=log
-000099b0: 5f73 7566 6669 782c 2074 696d 656f 7574  _suffix, timeout
-000099c0: 3d74 696d 656f 7574 0a20 2020 2020 2020  =timeout.       
-000099d0: 2029 0a0a 2020 2020 2020 2020 6669 6e69   )..        fini
-000099e0: 7368 6564 203d 2022 7374 6174 7573 2220  shed = "status" 
-000099f0: 696e 2072 6573 756c 7420 616e 6420 7265  in result and re
-00009a00: 7375 6c74 5b22 7374 6174 7573 225d 203d  sult["status"] =
-00009a10: 3d20 2246 494e 4953 4845 4422 0a20 2020  = "FINISHED".   
-00009a20: 2020 2020 2073 7563 6365 7373 203d 2066       success = f
-00009a30: 696e 6973 6865 640a 0a20 2020 2020 2020  inished..       
-00009a40: 2069 6620 7375 6363 6573 733a 0a20 2020   if success:.   
-00009a50: 2020 2020 2020 2020 2069 6620 2272 6573           if "res
-00009a60: 756c 7422 2069 6e20 7265 7375 6c74 3a0a  ult" in result:.
-00009a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a80: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
-00009a90: 2020 2020 2020 2069 6620 6e6f 7420 7375         if not su
-00009aa0: 6363 6573 733a 0a20 2020 2020 2020 2020  ccess:.         
-00009ab0: 2020 205f 7261 6973 655f 6572 726f 725f     _raise_error_
-00009ac0: 6d73 6728 7265 7375 6c74 290a 0a20 2020  msg(result)..   
-00009ad0: 2065 6c73 653a 0a20 2020 2020 2020 2023   else:.        #
-00009ae0: 2077 6169 7420 666f 7220 7468 6520 6f70   wait for the op
-00009af0: 6572 6174 696f 6e20 746f 2073 7461 7274  eration to start
-00009b00: 0a20 2020 2020 2020 2072 756e 6e69 6e67  .        running
-00009b10: 203d 205f 5f77 6169 745f 666f 725f 7468   = __wait_for_th
-00009b20: 655f 6f70 6572 6174 696f 6e5f 746f 5f73  e_operation_to_s
-00009b30: 7461 7274 2874 6173 6b5f 6964 290a 0a20  tart(task_id).. 
-00009b40: 2020 2020 2020 2069 6620 6e6f 7420 7275         if not ru
-00009b50: 6e6e 696e 673a 0a20 2020 2020 2020 2020  nning:.         
-00009b60: 2020 2073 7563 6365 7373 203d 2046 616c     success = Fal
-00009b70: 7365 0a0a 2020 2020 7265 7475 726e 2073  se..    return s
-00009b80: 7563 6365 7373 0a0a 0a23 202d 2d2d 2d2d  uccess...# -----
-00009b90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009ba0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009bb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009bc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009bd0: 2d2d 2d2d 2d20 230a 2320 436f 7265 2041  ----- #.# Core A
-00009be0: 5049 0a23 202d 2d2d 2d2d 2d2d 2d2d 2d2d  PI.# -----------
-00009bf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009c00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009c10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009c20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d20  --------------- 
-00009c30: 230a 0a0a 6465 6620 6765 745f 7665 7273  #...def get_vers
-00009c40: 696f 6e28 2920 2d3e 2073 7472 3a0a 2020  ion() -> str:.  
-00009c50: 2020 2222 2252 6574 7572 6e20 436f 7265    """Return Core
-00009c60: 2041 5049 2076 6572 7369 6f6e 2e22 2222   API version."""
-00009c70: 0a0a 2020 2020 7265 7375 6c74 203d 205f  ..    result = _
-00009c80: 6765 7428 222f 7369 6d75 6c61 7469 6f6e  get("/simulation
-00009c90: 2f76 6572 7369 6f6e 2229 0a0a 2020 2020  /version")..    
-00009ca0: 6966 2072 6573 756c 742e 7374 6174 7573  if result.status
-00009cb0: 5f63 6f64 6520 213d 2032 3030 3a0a 2020  _code != 200:.  
-00009cc0: 2020 2020 2020 5f68 616e 646c 655f 6572        _handle_er
-00009cd0: 726f 7228 7265 7375 6c74 2c20 2243 616e  ror(result, "Can
-00009ce0: 6e6f 7420 7265 7472 6965 7665 2043 6f72  not retrieve Cor
-00009cf0: 6520 4150 4920 7665 7273 696f 6e22 290a  e API version").
-00009d00: 0a20 2020 2072 6574 7572 6e20 7265 7375  .    return resu
-00009d10: 6c74 2e6a 736f 6e28 290a 0a0a 6465 6620  lt.json()...def 
-00009d20: 7265 7365 7428 6465 6c65 7465 5f63 6f6d  reset(delete_com
-00009d30: 7075 7465 5f73 6572 7665 7273 3a20 626f  pute_servers: bo
-00009d40: 6f6c 203d 2046 616c 7365 2920 2d3e 2041  ol = False) -> A
-00009d50: 6e79 3a0a 2020 2020 2222 220a 2020 2020  ny:.    """.    
-00009d60: 5265 7365 7420 7468 6520 4954 2053 696d  Reset the IT Sim
-00009d70: 756c 6174 696f 6e20 696e 6672 6173 7472  ulation infrastr
-00009d80: 7563 7475 7265 0a0a 2020 2020 5468 6973  ucture..    This
-00009d90: 2068 6173 2074 6865 2066 6f6c 6c6f 7769   has the followi
-00009da0: 6e67 2065 6666 6563 743a 0a20 2020 202d  ng effect:.    -
-00009db0: 2063 6c65 616e 2074 6865 2064 6174 6162   clean the datab
-00009dc0: 6173 6520 616e 6420 7265 2d70 6f70 756c  ase and re-popul
-00009dd0: 6174 6520 6974 2077 6974 6820 7374 6174  ate it with stat
-00009de0: 6963 2069 6e66 6f20 2862 6173 6562 6f78  ic info (basebox
-00009df0: 6573 2c20 726f 6c65 732e 2e2e 290a 2020  es, roles...).  
-00009e00: 2020 2d20 6279 2064 6566 6175 742c 2074    - by defaut, t
-00009e10: 6865 2074 6162 6c65 206f 6620 636f 6d70  he table of comp
-00009e20: 7574 6520 7365 7276 6572 7320 6973 206b  ute servers is k
-00009e30: 6570 742c 2062 7574 2060 6465 6c65 7465  ept, but `delete
-00009e40: 5f63 6f6d 7075 7465 5f73 6572 7665 7273  _compute_servers
-00009e50: 3d54 7275 6560 2063 6861 6e67 6573 2074  =True` changes t
-00009e60: 6861 7420 6265 6861 7669 6f72 0a20 2020  hat behavior.   
-00009e70: 202d 2072 6573 6574 2074 6865 2073 696d   - reset the sim
-00009e80: 756c 6174 696f 6e20 6d61 6e61 6765 720a  ulation manager.
-00009e90: 2020 2020 2d20 7265 7365 7420 7468 6520      - reset the 
-00009ea0: 636f 6d70 7574 6520 7365 7276 6572 7320  compute servers 
-00009eb0: 2873 746f 7020 564d 7320 616e 6420 646f  (stop VMs and do
-00009ec0: 636b 6572 732c 2072 6573 6574 206e 6574  ckers, reset net
-00009ed0: 776f 726b 732c 202e 2e2e 290a 2020 2020  works, ...).    
-00009ee0: 2222 220a 2020 2020 7061 7261 6d73 203d  """.    params =
-00009ef0: 207b 7d0a 2020 2020 6966 2064 656c 6574   {}.    if delet
-00009f00: 655f 636f 6d70 7574 655f 7365 7276 6572  e_compute_server
-00009f10: 733a 0a20 2020 2020 2020 2070 6172 616d  s:.        param
-00009f20: 7320 3d20 7b22 6465 6c65 7465 5f63 6f6d  s = {"delete_com
-00009f30: 7075 7465 5f73 6572 7665 7273 5f66 726f  pute_servers_fro
-00009f40: 6d5f 6462 223a 2064 656c 6574 655f 636f  m_db": delete_co
-00009f50: 6d70 7574 655f 7365 7276 6572 737d 0a0a  mpute_servers}..
-00009f60: 2020 2020 7265 7375 6c74 203d 205f 6465      result = _de
-00009f70: 6c65 7465 2822 2f73 696d 756c 6174 696f  lete("/simulatio
-00009f80: 6e2f 636f 6d70 7574 655f 696e 6672 6173  n/compute_infras
-00009f90: 7472 7563 7475 7265 5f72 6573 6574 222c  tructure_reset",
-00009fa0: 2070 6172 616d 733d 7061 7261 6d73 290a   params=params).
-00009fb0: 0a20 2020 2069 6620 7265 7375 6c74 2e73  .    if result.s
-00009fc0: 7461 7475 735f 636f 6465 2021 3d20 3230  tatus_code != 20
-00009fd0: 303a 0a20 2020 2020 2020 205f 6861 6e64  0:.        _hand
-00009fe0: 6c65 5f65 7272 6f72 2872 6573 756c 742c  le_error(result,
-00009ff0: 2022 4361 6e6e 6f74 2072 6573 6574 2073   "Cannot reset s
-0000a000: 696d 756c 6174 696f 6e20 696e 6672 6173  imulation infras
-0000a010: 7472 7563 7475 7265 2229 0a0a 2020 2020  tructure")..    
-0000a020: 7265 7475 726e 2072 6573 756c 742e 6a73  return result.js
-0000a030: 6f6e 2829 0a0a 0a64 6566 205f 6372 6561  on()...def _crea
-0000a040: 7465 5f6f 725f 6578 7465 6e64 5f73 696d  te_or_extend_sim
-0000a050: 756c 6174 696f 6e28 0a20 2020 2073 696d  ulation(.    sim
-0000a060: 756c 6174 696f 6e5f 6469 6374 3a20 6469  ulation_dict: di
-0000a070: 6374 2c0a 2020 2020 6964 5f73 696d 756c  ct,.    id_simul
-0000a080: 6174 696f 6e3a 2069 6e74 203d 204e 6f6e  ation: int = Non
-0000a090: 652c 0a20 2020 2061 6c6c 6f63 6174 696f  e,.    allocatio
-0000a0a0: 6e5f 7374 7261 7465 6779 3a20 4f70 7469  n_strategy: Opti
-0000a0b0: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
-0000a0c0: 2c0a 2920 2d3e 2054 7570 6c65 5b69 6e74  ,.) -> Tuple[int
-0000a0d0: 2c20 4c69 7374 5b73 7472 5d5d 3a0a 2020  , List[str]]:.  
-0000a0e0: 2020 2222 2243 7265 6174 6520 6120 7369    """Create a si
-0000a0f0: 6d75 6c61 7469 6f6e 2c20 6f72 2065 7874  mulation, or ext
-0000a100: 656e 6420 616e 2065 7869 7374 696e 6720  end an existing 
-0000a110: 7369 6d75 6c61 7469 6f6e 2077 6974 6820  simulation with 
-0000a120: 6e65 770a 2020 2020 6e6f 6465 7320 616e  new.    nodes an
-0000a130: 6420 6c69 6e6b 732c 2061 6e64 2072 6574  d links, and ret
-0000a140: 7572 6e20 6120 7369 6d75 6c61 7469 6f6e  urn a simulation
-0000a150: 2049 442e 2222 220a 0a20 2020 2023 2047   ID."""..    # G
-0000a160: 6574 2074 6865 2070 6174 6873 2069 6620  et the paths if 
-0000a170: 736f 6d65 2068 6176 6520 6265 656e 2070  some have been p
-0000a180: 726f 7669 6465 640a 2020 2020 7265 736f  rovided.    reso
-0000a190: 7572 6365 735f 7061 7468 7320 3d20 7369  urces_paths = si
-0000a1a0: 6d75 6c61 7469 6f6e 5f64 6963 742e 706f  mulation_dict.po
-0000a1b0: 7028 2272 6573 6f75 7263 6573 5f70 6174  p("resources_pat
-0000a1c0: 6873 222c 205b 5d29 0a0a 2020 2020 6461  hs", [])..    da
-0000a1d0: 7461 203d 206a 736f 6e2e 6475 6d70 7328  ta = json.dumps(
-0000a1e0: 7369 6d75 6c61 7469 6f6e 5f64 6963 7429  simulation_dict)
-0000a1f0: 0a0a 2020 2020 2320 4372 6561 7469 6f6e  ..    # Creation
-0000a200: 206f 6620 6120 666f 6c64 6572 2063 6f6e   of a folder con
-0000a210: 7461 696e 696e 6720 616c 6c20 7468 6520  taining all the 
-0000a220: 7265 736f 7572 6365 732c 2074 6869 7320  resources, this 
-0000a230: 666f 6c64 6572 2077 696c 6c20 7468 656e  folder will then
-0000a240: 2062 6520 7a69 7070 6564 0a20 2020 2077   be zipped.    w
-0000a250: 6974 6820 5465 6d70 6f72 6172 7944 6972  ith TemporaryDir
-0000a260: 6563 746f 7279 2870 7265 6669 783d 2263  ectory(prefix="c
-0000a270: 7962 6572 5f72 616e 6765 5f63 725f 636f  yber_range_cr_co
-0000a280: 7265 5f72 6573 6f75 7263 6573 2229 2061  re_resources") a
-0000a290: 7320 6d61 696e 5f72 6573 6f75 7263 6573  s main_resources
-0000a2a0: 3a0a 2020 2020 2020 2020 2320 636f 7079  :.        # copy
-0000a2b0: 2061 6c6c 2072 6573 6f75 7263 6573 2069   all resources i
-0000a2c0: 6e20 7468 6520 6d61 696e 2074 656d 706f  n the main tempo
-0000a2d0: 7261 7279 2066 6f6c 6465 720a 2020 2020  rary folder.    
-0000a2e0: 2020 2020 666f 7220 7265 736f 7572 6365      for resource
-0000a2f0: 2069 6e20 7265 736f 7572 6365 735f 7061   in resources_pa
-0000a300: 7468 733a 0a20 2020 2020 2020 2020 2020  ths:.           
-0000a310: 2069 6620 6f73 2e70 6174 682e 6973 6469   if os.path.isdi
-0000a320: 7228 7265 736f 7572 6365 293a 0a20 2020  r(resource):.   
-0000a330: 2020 2020 2020 2020 2020 2020 2073 6875               shu
-0000a340: 7469 6c2e 636f 7079 7472 6565 280a 2020  til.copytree(.  
-0000a350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a360: 2020 7265 736f 7572 6365 2c0a 2020 2020    resource,.    
-0000a370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a380: 6f73 2e70 6174 682e 6a6f 696e 280a 2020  os.path.join(.  
-0000a390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a3a0: 2020 2020 2020 6d61 696e 5f72 6573 6f75        main_resou
-0000a3b0: 7263 6573 2c20 6f73 2e70 6174 682e 6261  rces, os.path.ba
-0000a3c0: 7365 6e61 6d65 286f 732e 7061 7468 2e6e  sename(os.path.n
-0000a3d0: 6f72 6d70 6174 6828 7265 736f 7572 6365  ormpath(resource
-0000a3e0: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-0000a3f0: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
-0000a400: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0000a410: 2020 2020 2020 2020 656c 6966 206f 732e          elif os.
-0000a420: 7061 7468 2e69 7366 696c 6528 7265 736f  path.isfile(reso
-0000a430: 7572 6365 293a 0a20 2020 2020 2020 2020  urce):.         
-0000a440: 2020 2020 2020 2073 6875 7469 6c2e 636f         shutil.co
-0000a450: 7079 6669 6c65 280a 2020 2020 2020 2020  pyfile(.        
-0000a460: 2020 2020 2020 2020 2020 2020 7265 736f              reso
-0000a470: 7572 6365 2c0a 2020 2020 2020 2020 2020  urce,.          
-0000a480: 2020 2020 2020 2020 2020 6f73 2e70 6174            os.pat
-0000a490: 682e 6a6f 696e 280a 2020 2020 2020 2020  h.join(.        
-0000a4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a4b0: 6d61 696e 5f72 6573 6f75 7263 6573 2c20  main_resources, 
-0000a4c0: 6f73 2e70 6174 682e 6261 7365 6e61 6d65  os.path.basename
-0000a4d0: 286f 732e 7061 7468 2e6e 6f72 6d70 6174  (os.path.normpat
-0000a4e0: 6828 7265 736f 7572 6365 2929 0a20 2020  h(resource)).   
-0000a4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a500: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
-0000a510: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-0000a520: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000a530: 2020 2020 2020 2020 7261 6973 6520 4578          raise Ex
-0000a540: 6365 7074 696f 6e28 6622 4361 6e20 6e6f  ception(f"Can no
-0000a550: 7420 636f 7079 207b 7265 736f 7572 6365  t copy {resource
-0000a560: 7d22 290a 0a20 2020 2020 2020 2023 2057  }")..        # W
-0000a570: 6520 6861 7665 2074 6f20 6372 6561 7465  e have to create
-0000a580: 2061 206e 6577 2074 656d 706f 7261 7279   a new temporary
-0000a590: 2066 6f6c 6465 7220 746f 2068 6f73 7420   folder to host 
-0000a5a0: 7468 6520 6172 6368 6976 650a 2020 2020  the archive.    
-0000a5b0: 2020 2020 7769 7468 2054 656d 706f 7261      with Tempora
-0000a5c0: 7279 4469 7265 6374 6f72 7928 7072 6566  ryDirectory(pref
-0000a5d0: 6978 3d22 6379 6265 725f 7261 6e67 655f  ix="cyber_range_
-0000a5e0: 6372 5f63 6f72 655f 6172 6368 6976 6522  cr_core_archive"
-0000a5f0: 2920 6173 2074 656d 705f 6469 723a 0a20  ) as temp_dir:. 
-0000a600: 2020 2020 2020 2020 2020 2069 6620 7265             if re
-0000a610: 736f 7572 6365 735f 7061 7468 733a 0a20  sources_paths:. 
-0000a620: 2020 2020 2020 2020 2020 2020 2020 207a                 z
-0000a630: 6970 5f66 696c 655f 6e61 6d65 203d 205f  ip_file_name = _
-0000a640: 7a69 705f 7265 736f 7572 6365 7328 6d61  zip_resources(ma
-0000a650: 696e 5f72 6573 6f75 7263 6573 2c20 7465  in_resources, te
-0000a660: 6d70 5f64 6972 290a 2020 2020 2020 2020  mp_dir).        
-0000a670: 2020 2020 2020 2020 7265 736f 7572 6365          resource
-0000a680: 735f 6669 6c65 203d 206f 7065 6e28 7a69  s_file = open(zi
-0000a690: 705f 6669 6c65 5f6e 616d 652c 2022 7262  p_file_name, "rb
-0000a6a0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-0000a6b0: 2020 2066 696c 6573 203d 207b 2272 6573     files = {"res
-0000a6c0: 6f75 7263 6573 5f66 696c 6522 3a20 7265  ources_file": re
-0000a6d0: 736f 7572 6365 735f 6669 6c65 2c20 2264  sources_file, "d
-0000a6e0: 6174 6122 3a20 6461 7461 7d0a 2020 2020  ata": data}.    
-0000a6f0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000a700: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0000a710: 736f 7572 6365 735f 6669 6c65 203d 204e  sources_file = N
-0000a720: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
-0000a730: 2020 2020 6669 6c65 7320 3d20 7b22 6461      files = {"da
-0000a740: 7461 223a 2064 6174 617d 0a0a 2020 2020  ta": data}..    
-0000a750: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-0000a760: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000a770: 6964 5f73 696d 756c 6174 696f 6e20 6973  id_simulation is
-0000a780: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000a790: 2020 2020 2020 2020 2020 2023 2043 7265             # Cre
-0000a7a0: 6174 6520 6e65 7720 7369 6d75 6c61 7469  ate new simulati
-0000a7b0: 6f6e 0a20 2020 2020 2020 2020 2020 2020  on.             
-0000a7c0: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-0000a7d0: 5f70 6f73 7428 0a20 2020 2020 2020 2020  _post(.         
-0000a7e0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000a7f0: 2f73 696d 756c 6174 696f 6e2f 222c 0a20  /simulation/",. 
-0000a800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a810: 2020 2020 2020 2066 696c 6573 3d66 696c         files=fil
-0000a820: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
-0000a830: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000a840: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-0000a850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a860: 2020 2020 2320 4578 7465 6e64 2061 6e20      # Extend an 
-0000a870: 6578 6973 7469 6e67 2073 696d 756c 6174  existing simulat
-0000a880: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
-0000a890: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-0000a8a0: 205f 706f 7374 280a 2020 2020 2020 2020   _post(.        
-0000a8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a8c0: 6622 2f73 696d 756c 6174 696f 6e2f 7b69  f"/simulation/{i
-0000a8d0: 645f 7369 6d75 6c61 7469 6f6e 7d2f 6578  d_simulation}/ex
-0000a8e0: 7465 6e64 222c 0a20 2020 2020 2020 2020  tend",.         
-0000a8f0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000a900: 696c 6573 3d66 696c 6573 2c0a 2020 2020  iles=files,.    
-0000a910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a920: 290a 2020 2020 2020 2020 2020 2020 6669  ).            fi
-0000a930: 6e61 6c6c 793a 0a20 2020 2020 2020 2020  nally:.         
-0000a940: 2020 2020 2020 2069 6620 7265 736f 7572         if resour
-0000a950: 6365 735f 6669 6c65 3a0a 2020 2020 2020  ces_file:.      
-0000a960: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0000a970: 736f 7572 6365 735f 6669 6c65 2e63 6c6f  sources_file.clo
-0000a980: 7365 2829 0a0a 2020 2020 6966 206e 6f74  se()..    if not
-0000a990: 206d 6169 6e5f 7265 736f 7572 6365 733a   main_resources:
-0000a9a0: 0a20 2020 2020 2020 2069 6620 6964 5f73  .        if id_s
-0000a9b0: 696d 756c 6174 696f 6e20 6973 204e 6f6e  imulation is Non
-0000a9c0: 653a 0a20 2020 2020 2020 2020 2020 2023  e:.            #
-0000a9d0: 2043 7265 6174 6520 6e65 7720 7369 6d75   Create new simu
-0000a9e0: 6c61 7469 6f6e 0a20 2020 2020 2020 2020  lation.         
-0000a9f0: 2020 2072 6573 756c 7420 3d20 5f70 6f73     result = _pos
-0000aa00: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
-0000aa10: 2020 2022 2f73 696d 756c 6174 696f 6e2f     "/simulation/
-0000aa20: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-0000aa30: 2020 2064 6174 613d 6461 7461 2c0a 2020     data=data,.  
-0000aa40: 2020 2020 2020 2020 2020 2020 2020 6865                he
-0000aa50: 6164 6572 733d 7b22 436f 6e74 656e 742d  aders={"Content-
-0000aa60: 5479 7065 223a 2022 6170 706c 6963 6174  Type": "applicat
-0000aa70: 696f 6e2f 6a73 6f6e 227d 2c0a 2020 2020  ion/json"},.    
-0000aa80: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000aa90: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000aaa0: 2020 2020 2320 4578 7465 6e64 2061 6e20      # Extend an 
-0000aab0: 6578 6973 7469 6e67 2073 696d 756c 6174  existing simulat
-0000aac0: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
-0000aad0: 7265 7375 6c74 203d 205f 706f 7374 280a  result = _post(.
-0000aae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aaf0: 6622 2f73 696d 756c 6174 696f 6e2f 7b69  f"/simulation/{i
-0000ab00: 645f 7369 6d75 6c61 7469 6f6e 7d2f 6578  d_simulation}/ex
-0000ab10: 7465 6e64 222c 0a20 2020 2020 2020 2020  tend",.         
-0000ab20: 2020 2020 2020 2064 6174 613d 6461 7461         data=data
-0000ab30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000ab40: 2020 6865 6164 6572 733d 7b22 436f 6e74    headers={"Cont
-0000ab50: 656e 742d 5479 7065 223a 2022 6170 706c  ent-Type": "appl
-0000ab60: 6963 6174 696f 6e2f 6a73 6f6e 227d 2c0a  ication/json"},.
-0000ab70: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-0000ab80: 2020 2069 6620 7265 7375 6c74 2e73 7461     if result.sta
-0000ab90: 7475 735f 636f 6465 2021 3d20 3230 303a  tus_code != 200:
-0000aba0: 0a20 2020 2020 2020 205f 6861 6e64 6c65  .        _handle
-0000abb0: 5f65 7272 6f72 2872 6573 756c 742c 2022  _error(result, "
-0000abc0: 4361 6e6e 6f74 2070 6f73 7420 7369 6d75  Cannot post simu
-0000abd0: 6c61 7469 6f6e 2069 6e66 6f72 6d61 7469  lation informati
-0000abe0: 6f6e 2074 6f20 636f 7265 2041 5049 2229  on to core API")
-0000abf0: 0a0a 2020 2020 6964 5f73 696d 756c 6174  ..    id_simulat
-0000ac00: 696f 6e20 3d20 7265 7375 6c74 2e6a 736f  ion = result.jso
-0000ac10: 6e28 295b 2269 6422 5d0a 2020 2020 6e65  n()["id"].    ne
-0000ac20: 775f 6e6f 6465 7320 3d20 7265 7375 6c74  w_nodes = result
-0000ac30: 2e6a 736f 6e28 295b 226e 6577 5f6e 6f64  .json()["new_nod
-0000ac40: 6573 225d 0a20 2020 206c 6f67 6765 722e  es"].    logger.
-0000ac50: 696e 666f 2866 225b 2b5d 204e 6577 206e  info(f"[+] New n
-0000ac60: 6f64 6573 2066 6f72 2073 696d 756c 6174  odes for simulat
-0000ac70: 696f 6e20 6964 2027 7b69 645f 7369 6d75  ion id '{id_simu
-0000ac80: 6c61 7469 6f6e 7d27 3a20 277b 6e65 775f  lation}': '{new_
-0000ac90: 6e6f 6465 737d 2722 290a 0a20 2020 2023  nodes}'")..    #
-0000aca0: 2050 7265 7061 7265 2064 6973 6b20 7265   Prepare disk re
-0000acb0: 736f 7572 6365 730a 2020 2020 706f 7374  sources.    post
-0000acc0: 5f64 6174 6120 3d20 7b22 6e6f 6465 7322  _data = {"nodes"
-0000acd0: 3a20 6e65 775f 6e6f 6465 737d 0a20 2020  : new_nodes}.   
-0000ace0: 205f 7369 6d75 6c61 7469 6f6e 5f65 7865   _simulation_exe
-0000acf0: 6375 7465 5f6f 7065 7261 7469 6f6e 280a  cute_operation(.
-0000ad00: 2020 2020 2020 2020 2270 6f73 7422 2c0a          "post",.
-0000ad10: 2020 2020 2020 2020 2270 7265 7061 7265          "prepare
-0000ad20: 222c 0a20 2020 2020 2020 2069 645f 7369  ",.        id_si
-0000ad30: 6d75 6c61 7469 6f6e 2c0a 2020 2020 2020  mulation,.      
-0000ad40: 2020 2250 5245 5041 5249 4e47 222c 0a20    "PREPARING",. 
-0000ad50: 2020 2020 2020 206f 7074 696f 6e61 6c5f         optional_
-0000ad60: 7061 7261 6d31 3d61 6c6c 6f63 6174 696f  param1=allocatio
-0000ad70: 6e5f 7374 7261 7465 6779 2c0a 2020 2020  n_strategy,.    
-0000ad80: 2020 2020 706f 7374 5f64 6174 613d 706f      post_data=po
-0000ad90: 7374 5f64 6174 612c 0a20 2020 2029 0a0a  st_data,.    )..
-0000ada0: 2020 2020 2320 544f 444f 3a20 4368 6563      # TODO: Chec
-0000adb0: 6b20 7468 6174 2074 6865 2064 6f63 6b65  k that the docke
-0000adc0: 7220 766f 6c75 6d65 7320 7468 6174 2077  r volumes that w
-0000add0: 696c 6c20 6265 206d 6f75 6e74 6564 2062  ill be mounted b
-0000ade0: 7920 7369 6d75 5f72 756e 2061 7265 2070  y simu_run are p
-0000adf0: 7265 7365 6e74 206f 6e20 7468 6520 6669  resent on the fi
-0000ae00: 6c65 7379 7374 656d 0a20 2020 2023 2066  lesystem.    # f
-0000ae10: 6f72 202e 2e2e 3a20 5f73 696d 755f 6372  or ...: _simu_cr
-0000ae20: 6561 7465 5f76 616c 6964 6174 655f 7265  eate_validate_re
-0000ae30: 736f 7572 6365 735f 6578 6973 7473 2829  sources_exists()
-0000ae40: 0a0a 2020 2020 7265 7475 726e 2028 6964  ..    return (id
-0000ae50: 5f73 696d 756c 6174 696f 6e2c 206e 6577  _simulation, new
-0000ae60: 5f6e 6f64 6573 290a 0a0a 6465 6620 7369  _nodes)...def si
-0000ae70: 6d75 6c61 7469 6f6e 5f73 7461 7475 7328  mulation_status(
-0000ae80: 6964 5f73 696d 756c 6174 696f 6e3a 2069  id_simulation: i
-0000ae90: 6e74 2920 2d3e 2073 7472 3a0a 2020 2020  nt) -> str:.    
-0000aea0: 2222 2252 6574 7572 6e20 6f6e 6c79 2074  """Return only t
-0000aeb0: 6865 2073 7461 7475 7320 6f66 2074 6865  he status of the
-0000aec0: 2073 696d 756c 6174 696f 6e22 2222 0a20   simulation""". 
-0000aed0: 2020 2072 6573 756c 7420 3d20 5f67 6574     result = _get
-0000aee0: 2866 222f 7369 6d75 6c61 7469 6f6e 2f7b  (f"/simulation/{
-0000aef0: 6964 5f73 696d 756c 6174 696f 6e7d 2f73  id_simulation}/s
-0000af00: 7461 7475 7322 290a 0a20 2020 2069 6620  tatus")..    if 
-0000af10: 7265 7375 6c74 2e73 7461 7475 735f 636f  result.status_co
-0000af20: 6465 2021 3d20 3230 303a 0a20 2020 2020  de != 200:.     
-0000af30: 2020 205f 6861 6e64 6c65 5f65 7272 6f72     _handle_error
-0000af40: 2872 6573 756c 742c 2022 4361 6e6e 6f74  (result, "Cannot
-0000af50: 2072 6574 7269 6576 6520 7369 6d75 6c61   retrieve simula
-0000af60: 7469 6f6e 2069 6e66 6f20 6672 6f6d 2049  tion info from I
-0000af70: 5420 5369 6d75 6c61 7469 6f6e 2041 5049  T Simulation API
-0000af80: 2229 0a0a 2020 2020 7265 7475 726e 2072  ")..    return r
-0000af90: 6573 756c 742e 6a73 6f6e 2829 0a0a 0a64  esult.json()...d
-0000afa0: 6566 2066 6574 6368 5f73 696d 756c 6174  ef fetch_simulat
-0000afb0: 696f 6e28 6964 5f73 696d 756c 6174 696f  ion(id_simulatio
-0000afc0: 6e3a 2069 6e74 2920 2d3e 2064 6963 743a  n: int) -> dict:
-0000afd0: 0a20 2020 2022 2222 5265 7475 726e 2061  .    """Return a
-0000afe0: 2073 696d 756c 6174 696f 6e20 6469 6374   simulation dict
-0000aff0: 2067 6976 656e 2061 2073 696d 756c 6174   given a simulat
-0000b000: 696f 6e20 6964 2e22 2222 0a20 2020 2072  ion id.""".    r
-0000b010: 6573 756c 7420 3d20 5f67 6574 2866 222f  esult = _get(f"/
-0000b020: 7369 6d75 6c61 7469 6f6e 2f7b 6964 5f73  simulation/{id_s
-0000b030: 696d 756c 6174 696f 6e7d 2229 0a0a 2020  imulation}")..  
-0000b040: 2020 6966 2072 6573 756c 742e 7374 6174    if result.stat
-0000b050: 7573 5f63 6f64 6520 213d 2032 3030 3a0a  us_code != 200:.
-0000b060: 2020 2020 2020 2020 5f68 616e 646c 655f          _handle_
-0000b070: 6572 726f 7228 7265 7375 6c74 2c20 2243  error(result, "C
-0000b080: 616e 6e6f 7420 7265 7472 6965 7665 2073  annot retrieve s
-0000b090: 696d 756c 6174 696f 6e20 696e 666f 2066  imulation info f
-0000b0a0: 726f 6d20 4954 2053 696d 756c 6174 696f  rom IT Simulatio
-0000b0b0: 6e20 4150 4922 290a 0a20 2020 2073 696d  n API")..    sim
-0000b0c0: 756c 6174 696f 6e5f 6469 6374 203d 2072  ulation_dict = r
-0000b0d0: 6573 756c 742e 6a73 6f6e 2829 0a0a 2020  esult.json()..  
-0000b0e0: 2020 7265 7475 726e 2073 696d 756c 6174    return simulat
-0000b0f0: 696f 6e5f 6469 6374 0a0a 0a64 6566 2066  ion_dict...def f
-0000b100: 6574 6368 5f73 696d 756c 6174 696f 6e73  etch_simulations
-0000b110: 2829 202d 3e20 4c69 7374 5b41 6e79 5d3a  () -> List[Any]:
-0000b120: 0a20 2020 2022 2222 4765 7420 7468 6520  .    """Get the 
-0000b130: 6c69 7374 206f 6620 7369 6d75 6c61 7469  list of simulati
-0000b140: 6f6e 732c 2069 6e63 6c75 6469 6e67 2074  ons, including t
-0000b150: 6865 2063 7572 7265 6e74 6c79 2072 756e  he currently run
-0000b160: 6e69 6e67 2073 696d 7561 6c74 696f 6e2c  ning simualtion,
-0000b170: 2061 6c6f 6e67 2077 6974 680a 2020 2020   along with.    
-0000b180: 696e 666f 726d 6174 696f 6e20 6f6e 206e  information on n
-0000b190: 6f64 6573 0a0a 2020 2020 2222 220a 2020  odes..    """.  
-0000b1a0: 2020 7265 7375 6c74 203d 205f 6765 7428    result = _get(
-0000b1b0: 222f 7369 6d75 6c61 7469 6f6e 2f22 290a  "/simulation/").
-0000b1c0: 0a20 2020 2069 6620 7265 7375 6c74 2e73  .    if result.s
-0000b1d0: 7461 7475 735f 636f 6465 2021 3d20 3230  tatus_code != 20
-0000b1e0: 303a 0a20 2020 2020 2020 205f 6861 6e64  0:.        _hand
-0000b1f0: 6c65 5f65 7272 6f72 2872 6573 756c 742c  le_error(result,
-0000b200: 2022 4361 6e6e 6f74 2072 6574 7269 6576   "Cannot retriev
-0000b210: 6520 7369 6d75 6c61 7469 6f6e 2069 6e66  e simulation inf
-0000b220: 6f20 6672 6f6d 2049 5420 5369 6d75 6c61  o from IT Simula
-0000b230: 7469 6f6e 2041 5049 2229 0a0a 2020 2020  tion API")..    
-0000b240: 7369 6d75 6c61 7469 6f6e 5f6c 6973 7420  simulation_list 
-0000b250: 3d20 7265 7375 6c74 2e6a 736f 6e28 290a  = result.json().
-0000b260: 2020 2020 7265 7475 726e 2073 696d 756c      return simul
-0000b270: 6174 696f 6e5f 6c69 7374 0a0a 0a64 6566  ation_list...def
-0000b280: 2064 656c 6574 655f 7369 6d75 6c61 7469   delete_simulati
-0000b290: 6f6e 2869 645f 7369 6d75 6c61 7469 6f6e  on(id_simulation
-0000b2a0: 3a20 696e 7429 202d 3e20 416e 793a 0a20  : int) -> Any:. 
-0000b2b0: 2020 2022 2222 4465 6c65 7465 2061 2073     """Delete a s
-0000b2c0: 696d 756c 6174 696f 6e20 696e 2064 6174  imulation in dat
-0000b2d0: 6162 6173 652e 2222 220a 0a20 2020 2023  abase."""..    #
-0000b2e0: 2044 6573 7472 6f79 2073 696d 756c 6174   Destroy simulat
-0000b2f0: 696f 6e20 6966 2069 7420 6973 2072 756e  ion if it is run
-0000b300: 6e69 6e67 0a20 2020 2069 6620 7369 6d75  ning.    if simu
-0000b310: 6c61 7469 6f6e 5f73 7461 7475 7328 6964  lation_status(id
-0000b320: 5f73 696d 756c 6174 696f 6e29 203d 3d20  _simulation) == 
-0000b330: 2252 554e 4e49 4e47 223a 0a20 2020 2020  "RUNNING":.     
-0000b340: 2020 206e 6f64 6573 3a20 4c69 7374 5b73     nodes: List[s
-0000b350: 7472 5d20 3d20 5b5d 0a20 2020 2020 2020  tr] = [].       
-0000b360: 2070 6f73 745f 6461 7461 203d 207b 226e   post_data = {"n
-0000b370: 6f64 6573 223a 206e 6f64 6573 7d0a 0a20  odes": nodes}.. 
-0000b380: 2020 2020 2020 205f 7369 6d75 6c61 7469         _simulati
-0000b390: 6f6e 5f65 7865 6375 7465 5f6f 7065 7261  on_execute_opera
-0000b3a0: 7469 6f6e 280a 2020 2020 2020 2020 2020  tion(.          
-0000b3b0: 2020 2270 6f73 7422 2c20 2264 6573 7472    "post", "destr
-0000b3c0: 6f79 222c 2069 645f 7369 6d75 6c61 7469  oy", id_simulati
-0000b3d0: 6f6e 2c20 2253 544f 5050 494e 4722 2c20  on, "STOPPING", 
-0000b3e0: 706f 7374 5f64 6174 613d 706f 7374 5f64  post_data=post_d
-0000b3f0: 6174 610a 2020 2020 2020 2020 290a 0a20  ata.        ).. 
-0000b400: 2020 205f 7369 6d75 6c61 7469 6f6e 5f65     _simulation_e
-0000b410: 7865 6375 7465 5f6f 7065 7261 7469 6f6e  xecute_operation
-0000b420: 2822 6765 7422 2c20 2264 656c 6574 655f  ("get", "delete_
-0000b430: 736e 6170 7368 6f74 7322 2c20 6964 5f73  snapshots", id_s
-0000b440: 696d 756c 6174 696f 6e2c 2022 5354 4f50  imulation, "STOP
-0000b450: 5049 4e47 2229 0a0a 2020 2020 2320 4465  PING")..    # De
-0000b460: 6c65 7465 2073 696d 756c 6174 696f 6e20  lete simulation 
-0000b470: 6e6f 6465 730a 2020 2020 6465 6c65 7465  nodes.    delete
-0000b480: 5f6e 6f64 6573 2869 645f 7369 6d75 6c61  _nodes(id_simula
-0000b490: 7469 6f6e 290a 0a20 2020 2023 2044 656c  tion)..    # Del
-0000b4a0: 6574 6520 7369 6d75 6c61 7469 6f6e 0a20  ete simulation. 
-0000b4b0: 2020 2072 6573 756c 7420 3d20 5f64 656c     result = _del
-0000b4c0: 6574 6528 6622 2f73 696d 756c 6174 696f  ete(f"/simulatio
-0000b4d0: 6e2f 7b69 645f 7369 6d75 6c61 7469 6f6e  n/{id_simulation
-0000b4e0: 7d22 290a 0a20 2020 2069 6620 7265 7375  }")..    if resu
-0000b4f0: 6c74 2e73 7461 7475 735f 636f 6465 2021  lt.status_code !
-0000b500: 3d20 3230 303a 0a20 2020 2020 2020 205f  = 200:.        _
-0000b510: 6861 6e64 6c65 5f65 7272 6f72 2872 6573  handle_error(res
-0000b520: 756c 742c 2022 4361 6e6e 6f74 2064 656c  ult, "Cannot del
-0000b530: 6574 6520 7369 6d75 6c61 7469 6f6e 2066  ete simulation f
-0000b540: 726f 6d20 4954 2053 696d 756c 6174 696f  rom IT Simulatio
-0000b550: 6e20 4150 4922 290a 0a20 2020 2072 6574  n API")..    ret
-0000b560: 7572 6e20 7265 7375 6c74 2e6a 736f 6e28  urn result.json(
-0000b570: 290a 0a0a 6465 6620 6e6f 6465 5f73 7461  )...def node_sta
-0000b580: 7475 7328 6964 5f6e 6f64 653a 2069 6e74  tus(id_node: int
-0000b590: 2920 2d3e 2073 7472 3a0a 2020 2020 2222  ) -> str:.    ""
-0000b5a0: 2252 6574 7269 6576 6520 6e6f 6465 2073  "Retrieve node s
-0000b5b0: 7461 7475 732e 2222 220a 0a20 2020 2072  tatus."""..    r
-0000b5c0: 6573 756c 7420 3d20 5f67 6574 2866 222f  esult = _get(f"/
-0000b5d0: 6e6f 6465 2f7b 6964 5f6e 6f64 657d 2f73  node/{id_node}/s
-0000b5e0: 7461 7475 7322 290a 0a20 2020 2069 6620  tatus")..    if 
-0000b5f0: 7265 7375 6c74 2e73 7461 7475 735f 636f  result.status_co
-0000b600: 6465 2021 3d20 3230 303a 0a20 2020 2020  de != 200:.     
-0000b610: 2020 205f 6861 6e64 6c65 5f65 7272 6f72     _handle_error
-0000b620: 2872 6573 756c 742c 2022 4361 6e6e 6f74  (result, "Cannot
-0000b630: 2072 6574 7269 6576 6520 6e6f 6465 2069   retrieve node i
-0000b640: 6e66 6f20 6672 6f6d 2049 5420 5369 6d75  nfo from IT Simu
-0000b650: 6c61 7469 6f6e 2041 5049 2229 0a0a 2020  lation API")..  
-0000b660: 2020 7265 7475 726e 2072 6573 756c 742e    return result.
-0000b670: 6a73 6f6e 2829 0a0a 0a64 6566 2073 746f  json()...def sto
-0000b680: 705f 6e6f 6465 5f62 795f 6e61 6d65 2869  p_node_by_name(i
-0000b690: 645f 7369 6d75 6c61 7469 6f6e 3a20 696e  d_simulation: in
-0000b6a0: 742c 206e 6f64 655f 6e61 6d65 3a20 7374  t, node_name: st
-0000b6b0: 7229 202d 3e20 4e6f 6e65 3a0a 2020 2020  r) -> None:.    
-0000b6c0: 2222 2253 746f 7020 6120 6e6f 6465 2069  """Stop a node i
-0000b6d0: 6620 6974 2069 7320 7275 6e6e 696e 672e  f it is running.
-0000b6e0: 2222 220a 0a20 2020 2023 2052 6574 7269  """..    # Retri
-0000b6f0: 6576 6520 6964 5f6e 6f64 650a 2020 2020  eve id_node.    
-0000b700: 6e6f 6465 203d 2066 6574 6368 5f6e 6f64  node = fetch_nod
-0000b710: 655f 6279 5f6e 616d 6528 6964 5f73 696d  e_by_name(id_sim
-0000b720: 756c 6174 696f 6e2c 206e 6f64 655f 6e61  ulation, node_na
-0000b730: 6d65 290a 2020 2020 6964 5f6e 6f64 6520  me).    id_node 
-0000b740: 3d20 6e6f 6465 5b22 6964 225d 0a0a 2020  = node["id"]..  
-0000b750: 2020 2320 4465 6c65 7465 206e 6f64 650a    # Delete node.
-0000b760: 2020 2020 7374 6f70 5f6e 6f64 6528 6964      stop_node(id
-0000b770: 5f73 696d 756c 6174 696f 6e2c 2069 645f  _simulation, id_
-0000b780: 6e6f 6465 290a 0a0a 6465 6620 7374 6f70  node)...def stop
-0000b790: 5f6e 6f64 6528 6964 5f73 696d 756c 6174  _node(id_simulat
-0000b7a0: 696f 6e3a 2069 6e74 2c20 6964 5f6e 6f64  ion: int, id_nod
-0000b7b0: 653a 2073 7472 2920 2d3e 204e 6f6e 653a  e: str) -> None:
-0000b7c0: 0a20 2020 2022 2222 5374 6f70 2061 206e  .    """Stop a n
-0000b7d0: 6f64 6520 6966 2069 7420 6973 2072 756e  ode if it is run
-0000b7e0: 6e69 6e67 2e22 2222 0a0a 2020 2020 2320  ning."""..    # 
-0000b7f0: 5265 7472 6965 7665 206e 6f64 6520 6163  Retrieve node ac
-0000b800: 636f 7264 696e 6720 746f 2069 7473 206e  cording to its n
-0000b810: 616d 650a 2020 2020 6e6f 6465 203d 2066  ame.    node = f
-0000b820: 6574 6368 5f6e 6f64 6528 6964 5f6e 6f64  etch_node(id_nod
-0000b830: 6529 0a0a 2020 2020 2320 5365 7420 6e6f  e)..    # Set no
-0000b840: 6465 206e 616d 6573 2074 6f20 6465 6c65  de names to dele
-0000b850: 7465 0a20 2020 206e 6f64 6573 5f74 6f5f  te.    nodes_to_
-0000b860: 6465 6c65 7465 203d 205b 6e6f 6465 5b22  delete = [node["
-0000b870: 6e61 6d65 225d 5d0a 2020 2020 706f 7374  name"]].    post
-0000b880: 5f64 6174 6120 3d20 7b22 6e6f 6465 7322  _data = {"nodes"
-0000b890: 3a20 6e6f 6465 735f 746f 5f64 656c 6574  : nodes_to_delet
-0000b8a0: 657d 0a0a 2020 2020 2320 5374 6f70 206e  e}..    # Stop n
-0000b8b0: 6f64 6520 6966 2069 7420 6973 2072 756e  ode if it is run
-0000b8c0: 6e69 6e67 0a20 2020 2069 6620 6e6f 6465  ning.    if node
-0000b8d0: 5f73 7461 7475 7328 6964 5f6e 6f64 6529  _status(id_node)
-0000b8e0: 203d 3d20 2252 554e 4e49 4e47 223a 0a20   == "RUNNING":. 
-0000b8f0: 2020 2020 2020 205f 7369 6d75 6c61 7469         _simulati
-0000b900: 6f6e 5f65 7865 6375 7465 5f6f 7065 7261  on_execute_opera
-0000b910: 7469 6f6e 280a 2020 2020 2020 2020 2020  tion(.          
-0000b920: 2020 2270 6f73 7422 2c0a 2020 2020 2020    "post",.      
-0000b930: 2020 2020 2020 2268 616c 7422 2c0a 2020        "halt",.  
-0000b940: 2020 2020 2020 2020 2020 6964 5f73 696d            id_sim
-0000b950: 756c 6174 696f 6e2c 0a20 2020 2020 2020  ulation,.       
-0000b960: 2020 2020 2022 5354 4f50 5049 4e47 222c       "STOPPING",
-0000b970: 0a20 2020 2020 2020 2020 2020 2070 6f73  .            pos
-0000b980: 745f 6461 7461 3d70 6f73 745f 6461 7461  t_data=post_data
-0000b990: 2c0a 2020 2020 2020 2020 290a 0a0a 6465  ,.        )...de
-0000b9a0: 6620 7570 6461 7465 5f73 696d 756c 6174  f update_simulat
-0000b9b0: 696f 6e28 6964 5f73 696d 756c 6174 696f  ion(id_simulatio
-0000b9c0: 6e3a 2069 6e74 2c20 7369 6d75 6c61 7469  n: int, simulati
-0000b9d0: 6f6e 5f64 6963 743a 2064 6963 7429 202d  on_dict: dict) -
-0000b9e0: 3e20 416e 793a 0a20 2020 2022 2222 5570  > Any:.    """Up
-0000b9f0: 6461 7465 2073 696d 756c 6174 696f 6e20  date simulation 
-0000ba00: 696e 666f 726d 6174 696f 6e20 696e 666f  information info
-0000ba10: 726d 6174 696f 6e20 6769 7665 6e20 6120  rmation given a 
-0000ba20: 7369 6d75 6c61 7469 6f6e 2069 640a 2020  simulation id.  
-0000ba30: 2020 616e 6420 6120 6469 6374 2063 6f6e    and a dict con
-0000ba40: 7461 696e 696e 6720 7369 6d75 6c61 7469  taining simulati
-0000ba50: 6f6e 2069 6e66 6f2e 0a20 2020 2022 2222  on info..    """
-0000ba60: 0a20 2020 2064 6174 6120 3d20 6a73 6f6e  .    data = json
-0000ba70: 2e64 756d 7073 2873 696d 756c 6174 696f  .dumps(simulatio
-0000ba80: 6e5f 6469 6374 290a 2020 2020 7265 7375  n_dict).    resu
-0000ba90: 6c74 203d 205f 7075 7428 0a20 2020 2020  lt = _put(.     
-0000baa0: 2020 2066 222f 7369 6d75 6c61 7469 6f6e     f"/simulation
-0000bab0: 2f7b 6964 5f73 696d 756c 6174 696f 6e7d  /{id_simulation}
-0000bac0: 222c 0a20 2020 2020 2020 2064 6174 613d  ",.        data=
-0000bad0: 6461 7461 2c0a 2020 2020 2020 2020 6865  data,.        he
-0000bae0: 6164 6572 733d 7b22 436f 6e74 656e 742d  aders={"Content-
-0000baf0: 5479 7065 223a 2022 6170 706c 6963 6174  Type": "applicat
-0000bb00: 696f 6e2f 6a73 6f6e 227d 2c0a 2020 2020  ion/json"},.    
-0000bb10: 290a 0a20 2020 2069 6620 7265 7375 6c74  )..    if result
-0000bb20: 2e73 7461 7475 735f 636f 6465 2021 3d20  .status_code != 
-0000bb30: 3230 303a 0a20 2020 2020 2020 205f 6861  200:.        _ha
-0000bb40: 6e64 6c65 5f65 7272 6f72 2872 6573 756c  ndle_error(resul
-0000bb50: 742c 2022 4361 6e6e 6f74 2075 7064 6174  t, "Cannot updat
-0000bb60: 6520 7369 6d75 6c61 7469 6f6e 2069 6e66  e simulation inf
-0000bb70: 6f72 6d61 7469 6f6e 2229 0a0a 2020 2020  ormation")..    
-0000bb80: 7265 7475 726e 2072 6573 756c 742e 6a73  return result.js
-0000bb90: 6f6e 2829 0a0a 0a64 6566 2066 6574 6368  on()...def fetch
-0000bba0: 5f73 696d 756c 6174 696f 6e5f 746f 706f  _simulation_topo
-0000bbb0: 6c6f 6779 2869 645f 7369 6d75 6c61 7469  logy(id_simulati
-0000bbc0: 6f6e 3a20 696e 7429 202d 3e20 416e 793a  on: int) -> Any:
-0000bbd0: 0a20 2020 2022 2222 5265 7475 726e 2074  .    """Return t
-0000bbe0: 6865 2074 6f70 6f6c 6f67 7920 6f66 2061  he topology of a
-0000bbf0: 2073 696d 756c 6174 696f 6e2e 2222 220a   simulation.""".
-0000bc00: 2020 2020 7265 7375 6c74 203d 205f 6765      result = _ge
-0000bc10: 7428 6622 2f73 696d 756c 6174 696f 6e2f  t(f"/simulation/
-0000bc20: 7b69 645f 7369 6d75 6c61 7469 6f6e 7d2f  {id_simulation}/
-0000bc30: 746f 706f 6c6f 6779 2229 0a0a 2020 2020  topology")..    
-0000bc40: 6966 2072 6573 756c 742e 7374 6174 7573  if result.status
-0000bc50: 5f63 6f64 6520 213d 2032 3030 3a0a 2020  _code != 200:.  
-0000bc60: 2020 2020 2020 5f68 616e 646c 655f 6572        _handle_er
-0000bc70: 726f 7228 7265 7375 6c74 2c20 2243 616e  ror(result, "Can
-0000bc80: 6e6f 7420 7265 7472 6965 7665 2073 696d  not retrieve sim
-0000bc90: 756c 6174 696f 6e20 746f 706f 6c6f 6779  ulation topology
-0000bca0: 2069 6e66 6f22 290a 0a20 2020 2072 6574   info")..    ret
-0000bcb0: 7572 6e20 7265 7375 6c74 2e6a 736f 6e28  urn result.json(
-0000bcc0: 290a 0a0a 6465 6620 6665 7463 685f 7369  )...def fetch_si
-0000bcd0: 6d75 6c61 7469 6f6e 5f74 6f70 6f6c 6f67  mulation_topolog
-0000bce0: 795f 7961 6d6c 2869 645f 7369 6d75 6c61  y_yaml(id_simula
-0000bcf0: 7469 6f6e 3a20 696e 7429 202d 3e20 416e  tion: int) -> An
-0000bd00: 793a 0a20 2020 2022 2222 5265 7475 726e  y:.    """Return
-0000bd10: 2074 6865 2059 414d 4c20 746f 706f 6c6f   the YAML topolo
-0000bd20: 6779 2063 6f6e 7465 6e74 206f 6620 6120  gy content of a 
-0000bd30: 7369 6d75 6c61 7469 6f6e 2e22 2222 0a20  simulation.""". 
-0000bd40: 2020 2072 6573 756c 7420 3d20 5f67 6574     result = _get
-0000bd50: 2866 222f 7369 6d75 6c61 7469 6f6e 2f7b  (f"/simulation/{
-0000bd60: 6964 5f73 696d 756c 6174 696f 6e7d 2f74  id_simulation}/t
-0000bd70: 6f70 6f6c 6f67 795f 7961 6d6c 2229 0a0a  opology_yaml")..
-0000bd80: 2020 2020 6966 2072 6573 756c 742e 7374      if result.st
-0000bd90: 6174 7573 5f63 6f64 6520 213d 2032 3030  atus_code != 200
-0000bda0: 3a0a 2020 2020 2020 2020 5f68 616e 646c  :.        _handl
-0000bdb0: 655f 6572 726f 7228 7265 7375 6c74 2c20  e_error(result, 
-0000bdc0: 2243 616e 6e6f 7420 7265 7472 6965 7665  "Cannot retrieve
-0000bdd0: 2073 696d 756c 6174 696f 6e20 746f 706f   simulation topo
-0000bde0: 6c6f 6779 2069 6e66 6f22 290a 0a20 2020  logy info")..   
-0000bdf0: 2072 6574 7572 6e20 7265 7375 6c74 2e6a   return result.j
-0000be00: 736f 6e28 290a 0a0a 6465 6620 6665 7463  son()...def fetc
-0000be10: 685f 6173 7365 7473 2869 645f 7369 6d75  h_assets(id_simu
-0000be20: 6c61 7469 6f6e 3a20 696e 7429 202d 3e20  lation: int) -> 
-0000be30: 416e 793a 0a20 2020 2022 2222 5265 7475  Any:.    """Retu
-0000be40: 726e 2074 6865 206c 6973 7420 6f66 2074  rn the list of t
-0000be50: 6865 2061 7373 6574 730a 2020 2020 6f66  he assets.    of
-0000be60: 2061 2067 6976 656e 2073 696d 756c 6174   a given simulat
-0000be70: 696f 6e2e 2049 7420 636f 7272 6573 706f  ion. It correspo
-0000be80: 6e64 7320 746f 0a20 2020 2074 6865 206c  nds to.    the l
-0000be90: 6973 7420 6f66 2074 6865 206e 6f64 6573  ist of the nodes
-0000bea0: 2077 6974 6820 736f 6d65 2061 6464 6974   with some addit
-0000beb0: 696f 6e61 6c0a 2020 2020 696e 666f 726d  ional.    inform
-0000bec0: 6174 696f 6e2e 0a20 2020 2022 2222 0a20  ation..    """. 
-0000bed0: 2020 2072 6573 756c 7420 3d20 5f67 6574     result = _get
-0000bee0: 2866 222f 7369 6d75 6c61 7469 6f6e 2f7b  (f"/simulation/{
-0000bef0: 6964 5f73 696d 756c 6174 696f 6e7d 2f61  id_simulation}/a
-0000bf00: 7373 6574 7322 290a 0a20 2020 2069 6620  ssets")..    if 
-0000bf10: 7265 7375 6c74 2e73 7461 7475 735f 636f  result.status_co
-0000bf20: 6465 2021 3d20 3230 303a 0a20 2020 2020  de != 200:.     
-0000bf30: 2020 205f 6861 6e64 6c65 5f65 7272 6f72     _handle_error
-0000bf40: 2872 6573 756c 742c 2022 4361 6e6e 6f74  (result, "Cannot
-0000bf50: 2072 6574 7269 6576 6520 6173 7365 7473   retrieve assets
-0000bf60: 2066 726f 6d20 636f 7265 2041 5049 2229   from core API")
-0000bf70: 0a0a 2020 2020 7265 7475 726e 2072 6573  ..    return res
-0000bf80: 756c 742e 6a73 6f6e 2829 0a0a 0a64 6566  ult.json()...def
-0000bf90: 2066 6574 6368 5f73 7769 7463 685f 6279   fetch_switch_by
-0000bfa0: 5f6e 6574 776f 726b 5f69 6428 6964 5f73  _network_id(id_s
-0000bfb0: 696d 756c 6174 696f 6e3a 2069 6e74 2c20  imulation: int, 
-0000bfc0: 6e65 7477 6f72 6b5f 6964 3a20 7374 7229  network_id: str)
-0000bfd0: 202d 3e20 416e 793a 0a20 2020 2022 2222   -> Any:.    """
-0000bfe0: 5265 7475 726e 2061 2073 7769 7463 6820  Return a switch 
-0000bff0: 6769 7665 6e20 6974 7320 6e65 7477 6f72  given its networ
-0000c000: 6b5f 6964 2222 220a 0a20 2020 2072 6573  k_id"""..    res
-0000c010: 756c 7420 3d20 5f67 6574 2866 222f 7369  ult = _get(f"/si
-0000c020: 6d75 6c61 7469 6f6e 2f7b 6964 5f73 696d  mulation/{id_sim
-0000c030: 756c 6174 696f 6e7d 2f73 7769 7463 682f  ulation}/switch/
-0000c040: 7b6e 6574 776f 726b 5f69 647d 2229 0a0a  {network_id}")..
-0000c050: 2020 2020 6966 2072 6573 756c 742e 7374      if result.st
-0000c060: 6174 7573 5f63 6f64 6520 213d 2032 3030  atus_code != 200
-0000c070: 3a0a 2020 2020 2020 2020 5f68 616e 646c  :.        _handl
-0000c080: 655f 6572 726f 7228 7265 7375 6c74 2c20  e_error(result, 
-0000c090: 2243 616e 6e6f 7420 7265 7472 6965 7665  "Cannot retrieve
-0000c0a0: 2073 696d 756c 6174 696f 6e20 7377 6974   simulation swit
-0000c0b0: 6368 2066 726f 6d20 636f 7265 2041 5049  ch from core API
-0000c0c0: 2229 0a0a 2020 2020 7265 7475 726e 2072  ")..    return r
-0000c0d0: 6573 756c 742e 6a73 6f6e 2829 0a0a 0a64  esult.json()...d
-0000c0e0: 6566 2066 6574 6368 5f6e 6f64 6528 6e6f  ef fetch_node(no
-0000c0f0: 6465 5f69 643a 2069 6e74 2920 2d3e 2041  de_id: int) -> A
-0000c100: 6e79 3a0a 2020 2020 2222 2252 6574 7572  ny:.    """Retur
-0000c110: 6e20 6120 6e6f 6465 2067 6976 656e 2069  n a node given i
-0000c120: 7473 2049 4422 2222 0a20 2020 2072 6573  ts ID""".    res
-0000c130: 756c 7420 3d20 5f67 6574 2866 222f 6e6f  ult = _get(f"/no
-0000c140: 6465 2f7b 6e6f 6465 5f69 647d 2229 0a0a  de/{node_id}")..
-0000c150: 2020 2020 6966 2072 6573 756c 742e 7374      if result.st
-0000c160: 6174 7573 5f63 6f64 6520 213d 2032 3030  atus_code != 200
-0000c170: 3a0a 2020 2020 2020 2020 5f68 616e 646c  :.        _handl
-0000c180: 655f 6572 726f 7228 7265 7375 6c74 2c20  e_error(result, 
-0000c190: 2243 616e 6e6f 7420 7265 7472 6965 7665  "Cannot retrieve
-0000c1a0: 206e 6f64 6520 6672 6f6d 2049 5420 5369   node from IT Si
-0000c1b0: 6d75 6c61 7469 6f6e 2041 5049 2229 0a0a  mulation API")..
-0000c1c0: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-0000c1d0: 742e 6a73 6f6e 2829 0a0a 0a64 6566 2066  t.json()...def f
-0000c1e0: 6574 6368 5f6e 6f64 655f 6279 5f6e 616d  etch_node_by_nam
-0000c1f0: 6528 6964 5f73 696d 756c 6174 696f 6e3a  e(id_simulation:
-0000c200: 2069 6e74 2c20 6e6f 6465 5f6e 616d 653a   int, node_name:
-0000c210: 2073 7472 2920 2d3e 2041 6e79 3a0a 2020   str) -> Any:.  
-0000c220: 2020 2222 2252 6574 7572 6e20 6120 6e6f    """Return a no
-0000c230: 6465 2067 6976 656e 2069 7473 206e 616d  de given its nam
-0000c240: 6522 2222 0a0a 2020 2020 7265 7375 6c74  e"""..    result
-0000c250: 203d 205f 6765 7428 6622 2f73 696d 756c   = _get(f"/simul
-0000c260: 6174 696f 6e2f 7b69 645f 7369 6d75 6c61  ation/{id_simula
-0000c270: 7469 6f6e 7d2f 6e6f 6465 2f7b 6e6f 6465  tion}/node/{node
-0000c280: 5f6e 616d 657d 2229 0a0a 2020 2020 6966  _name}")..    if
-0000c290: 2072 6573 756c 742e 7374 6174 7573 5f63   result.status_c
-0000c2a0: 6f64 6520 213d 2032 3030 3a0a 2020 2020  ode != 200:.    
-0000c2b0: 2020 2020 5f68 616e 646c 655f 6572 726f      _handle_erro
-0000c2c0: 7228 0a20 2020 2020 2020 2020 2020 2072  r(.            r
-0000c2d0: 6573 756c 742c 2022 4361 6e6e 6f74 2072  esult, "Cannot r
-0000c2e0: 6574 7269 6576 6520 6e6f 6465 2062 6173  etrieve node bas
-0000c2f0: 6564 206f 6e20 6974 7320 6e61 6d65 2066  ed on its name f
-0000c300: 726f 6d20 4954 2053 696d 756c 6174 696f  rom IT Simulatio
-0000c310: 6e20 4150 4922 0a20 2020 2020 2020 2029  n API".        )
-0000c320: 0a0a 2020 2020 7265 7475 726e 2072 6573  ..    return res
-0000c330: 756c 742e 6a73 6f6e 2829 0a0a 0a64 6566  ult.json()...def
-0000c340: 2066 6574 6368 5f6e 6f64 6573 5f62 795f   fetch_nodes_by_
-0000c350: 726f 6c65 7328 6964 5f73 696d 756c 6174  roles(id_simulat
-0000c360: 696f 6e3a 2069 6e74 2920 2d3e 2041 6e79  ion: int) -> Any
-0000c370: 3a0a 2020 2020 2222 2252 6574 7572 6e20  :.    """Return 
-0000c380: 6120 6469 6374 2077 6b65 7265 206b 6579  a dict wkere key
-0000c390: 7320 6172 6520 726f 6c65 7320 2873 7563  s are roles (suc
-0000c3a0: 6820 6173 2027 6164 272c 2027 6669 6c65  h as 'ad', 'file
-0000c3b0: 5f73 6572 7665 7227 2c20 2763 6c69 656e  _server', 'clien
-0000c3c0: 7427 2c20 2e2e 2e29 2061 6e64 0a20 2020  t', ...) and.   
-0000c3d0: 2076 616c 7565 7320 6172 6520 6e6f 6465   values are node
-0000c3e0: 732e 0a0a 2020 2020 2222 220a 2020 2020  s...    """.    
-0000c3f0: 7265 7375 6c74 203d 205f 6765 7428 6622  result = _get(f"
-0000c400: 2f73 696d 756c 6174 696f 6e2f 7b69 645f  /simulation/{id_
-0000c410: 7369 6d75 6c61 7469 6f6e 7d2f 6e6f 6465  simulation}/node
-0000c420: 735f 6279 5f72 6f6c 6573 2229 0a0a 2020  s_by_roles")..  
-0000c430: 2020 6966 2072 6573 756c 742e 7374 6174    if result.stat
-0000c440: 7573 5f63 6f64 6520 213d 2032 3030 3a0a  us_code != 200:.
-0000c450: 2020 2020 2020 2020 5f68 616e 646c 655f          _handle_
-0000c460: 6572 726f 7228 7265 7375 6c74 2c20 2243  error(result, "C
-0000c470: 616e 6e6f 7420 7265 7472 6965 7665 206e  annot retrieve n
-0000c480: 6f64 6573 2229 0a0a 2020 2020 726f 6c65  odes")..    role
-0000c490: 735f 6469 6374 203d 2072 6573 756c 742e  s_dict = result.
-0000c4a0: 6a73 6f6e 2829 0a20 2020 2072 6574 7572  json().    retur
-0000c4b0: 6e20 726f 6c65 735f 6469 6374 0a0a 0a64  n roles_dict...d
-0000c4c0: 6566 2064 656c 6574 655f 6e6f 6465 5f62  ef delete_node_b
-0000c4d0: 795f 6e61 6d65 2869 645f 7369 6d75 6c61  y_name(id_simula
-0000c4e0: 7469 6f6e 3a20 696e 742c 206e 6f64 655f  tion: int, node_
-0000c4f0: 6e61 6d65 3a20 7374 7229 202d 3e20 416e  name: str) -> An
-0000c500: 793a 0a20 2020 2023 2052 6574 7269 6576  y:.    # Retriev
-0000c510: 6520 6964 5f6e 6f64 650a 2020 2020 6e6f  e id_node.    no
-0000c520: 6465 203d 2066 6574 6368 5f6e 6f64 655f  de = fetch_node_
-0000c530: 6279 5f6e 616d 6528 6964 5f73 696d 756c  by_name(id_simul
-0000c540: 6174 696f 6e2c 206e 6f64 655f 6e61 6d65  ation, node_name
-0000c550: 290a 2020 2020 6964 5f6e 6f64 6520 3d20  ).    id_node = 
-0000c560: 6e6f 6465 5b22 6964 225d 0a0a 2020 2020  node["id"]..    
-0000c570: 2320 4465 6c65 7465 206e 6f64 650a 2020  # Delete node.  
-0000c580: 2020 6465 6c65 7465 5f6e 6f64 6528 6964    delete_node(id
-0000c590: 5f6e 6f64 6529 0a0a 0a64 6566 2064 656c  _node)...def del
-0000c5a0: 6574 655f 6e6f 6465 2869 645f 6e6f 6465  ete_node(id_node
-0000c5b0: 3a20 696e 7429 202d 3e20 416e 793a 0a20  : int) -> Any:. 
-0000c5c0: 2020 2022 2222 4465 6c65 7465 206e 6f64     """Delete nod
-0000c5d0: 6520 6672 6f6d 2064 6174 6162 6173 6520  e from database 
-0000c5e0: 6769 7665 6e20 6974 7320 4944 2e22 2222  given its ID."""
-0000c5f0: 0a0a 2020 2020 2320 4665 7463 6820 7669  ..    # Fetch vi
-0000c600: 7274 7561 6c20 6e6f 6465 206e 6574 776f  rtual node netwo
-0000c610: 726b 2069 6e74 6572 6661 6365 730a 2020  rk interfaces.  
-0000c620: 2020 6e65 7477 6f72 6b5f 696e 7465 7266    network_interf
-0000c630: 6163 6573 203d 2066 6574 6368 5f6e 6f64  aces = fetch_nod
-0000c640: 655f 6e65 7477 6f72 6b5f 696e 7465 7266  e_network_interf
-0000c650: 6163 6573 2869 645f 6e6f 6465 290a 0a20  aces(id_node).. 
-0000c660: 2020 2023 2044 656c 6574 6520 6561 6368     # Delete each
-0000c670: 206e 6574 776f 726b 2069 6e74 6572 6661   network interfa
-0000c680: 6365 730a 2020 2020 666f 7220 6e65 7477  ces.    for netw
-0000c690: 6f72 6b5f 696e 7465 7266 6163 6520 696e  ork_interface in
-0000c6a0: 206e 6574 776f 726b 5f69 6e74 6572 6661   network_interfa
-0000c6b0: 6365 733a 0a20 2020 2020 2020 2064 656c  ces:.        del
-0000c6c0: 6574 655f 6e65 7477 6f72 6b5f 696e 7465  ete_network_inte
-0000c6d0: 7266 6163 6528 6e65 7477 6f72 6b5f 696e  rface(network_in
-0000c6e0: 7465 7266 6163 655b 2269 6422 5d29 0a0a  terface["id"])..
-0000c6f0: 2020 2020 2320 4465 6c65 7465 206e 6f64      # Delete nod
-0000c700: 650a 2020 2020 7265 7375 6c74 203d 205f  e.    result = _
-0000c710: 6465 6c65 7465 2866 222f 6e6f 6465 2f7b  delete(f"/node/{
-0000c720: 6964 5f6e 6f64 657d 2229 0a0a 2020 2020  id_node}")..    
-0000c730: 6966 2072 6573 756c 742e 7374 6174 7573  if result.status
-0000c740: 5f63 6f64 6520 213d 2032 3030 3a0a 2020  _code != 200:.  
-0000c750: 2020 2020 2020 5f68 616e 646c 655f 6572        _handle_er
-0000c760: 726f 7228 7265 7375 6c74 2c20 2243 616e  ror(result, "Can
-0000c770: 6e6f 7420 6465 6c65 7465 206e 6f64 6522  not delete node"
-0000c780: 290a 0a20 2020 2072 6574 7572 6e20 7265  )..    return re
-0000c790: 7375 6c74 2e6a 736f 6e28 290a 0a0a 6465  sult.json()...de
-0000c7a0: 6620 6665 7463 685f 6e6f 6465 7328 6964  f fetch_nodes(id
-0000c7b0: 5f73 696d 756c 6174 696f 6e3a 2069 6e74  _simulation: int
-0000c7c0: 2920 2d3e 2041 6e79 3a0a 2020 2020 2222  ) -> Any:.    ""
-0000c7d0: 2252 6574 7572 6e20 7369 6d75 6c61 7469  "Return simulati
-0000c7e0: 6f6e 206e 6f64 6573 2064 6963 7420 6769  on nodes dict gi
-0000c7f0: 7665 6e0a 2020 2020 6120 7369 6d75 6c61  ven.    a simula
-0000c800: 7469 6f6e 2049 442c 2077 6865 7265 206b  tion ID, where k
-0000c810: 6579 7320 6172 6520 6e6f 6465 206e 616d  eys are node nam
-0000c820: 6573 2e0a 2020 2020 2222 220a 2020 2020  es..    """.    
-0000c830: 7265 7375 6c74 203d 205f 6765 7428 6622  result = _get(f"
-0000c840: 2f73 696d 756c 6174 696f 6e2f 7b69 645f  /simulation/{id_
-0000c850: 7369 6d75 6c61 7469 6f6e 7d2f 6e6f 6465  simulation}/node
-0000c860: 2229 0a0a 2020 2020 6966 2072 6573 756c  ")..    if resul
-0000c870: 742e 7374 6174 7573 5f63 6f64 6520 213d  t.status_code !=
-0000c880: 2032 3030 3a0a 2020 2020 2020 2020 5f68   200:.        _h
-0000c890: 616e 646c 655f 6572 726f 7228 7265 7375  andle_error(resu
-0000c8a0: 6c74 2c20 2243 616e 6e6f 7420 7265 7472  lt, "Cannot retr
-0000c8b0: 6965 7665 206e 6f64 6573 2066 726f 6d20  ieve nodes from 
-0000c8c0: 4954 2053 696d 756c 6174 696f 6e20 4150  IT Simulation AP
-0000c8d0: 4922 290a 0a20 2020 2072 6574 7572 6e20  I")..    return 
-0000c8e0: 7265 7375 6c74 2e6a 736f 6e28 290a 0a0a  result.json()...
-0000c8f0: 6465 6620 6665 7463 685f 7669 7274 7561  def fetch_virtua
-0000c900: 6c5f 6d61 6368 696e 6573 2869 645f 7369  l_machines(id_si
-0000c910: 6d75 6c61 7469 6f6e 3a20 696e 7429 202d  mulation: int) -
-0000c920: 3e20 4c69 7374 5b64 6963 745d 3a0a 2020  > List[dict]:.  
-0000c930: 2020 2222 2252 6574 7572 6e20 7369 6d75    """Return simu
-0000c940: 6c61 7469 6f6e 2076 6972 7475 616c 206d  lation virtual m
-0000c950: 6163 6869 6e65 7320 6469 6374 2067 6976  achines dict giv
-0000c960: 656e 2061 2073 696d 756c 6174 696f 6e20  en a simulation 
-0000c970: 4944 2c0a 2020 2020 7768 6572 6520 6b65  ID,.    where ke
-0000c980: 7973 2061 7265 2076 6972 7475 616c 206d  ys are virtual m
-0000c990: 6163 6869 6e65 206e 616d 6573 2e0a 2020  achine names..  
-0000c9a0: 2020 2222 220a 2020 2020 7265 7375 6c74    """.    result
-0000c9b0: 7320 3d20 6665 7463 685f 6e6f 6465 7328  s = fetch_nodes(
-0000c9c0: 6964 5f73 696d 756c 6174 696f 6e29 0a0a  id_simulation)..
-0000c9d0: 2020 2020 766d 5f6f 6e6c 7920 3d20 6669      vm_only = fi
-0000c9e0: 6c74 6572 286c 616d 6264 6120 6d3a 206d  lter(lambda m: m
-0000c9f0: 5b22 7479 7065 225d 203d 3d20 2276 6972  ["type"] == "vir
-0000ca00: 7475 616c 5f6d 6163 6869 6e65 222c 2072  tual_machine", r
-0000ca10: 6573 756c 7473 290a 2020 2020 7265 7475  esults).    retu
-0000ca20: 726e 206c 6973 7428 766d 5f6f 6e6c 7929  rn list(vm_only)
-0000ca30: 0a0a 0a64 6566 2064 656c 6574 655f 6e6f  ...def delete_no
-0000ca40: 6465 7328 6964 5f73 696d 756c 6174 696f  des(id_simulatio
-0000ca50: 6e3a 2069 6e74 2920 2d3e 2073 7472 3a0a  n: int) -> str:.
-0000ca60: 2020 2020 2222 2244 656c 6574 6520 7369      """Delete si
-0000ca70: 6d75 6c61 7469 6f6e 206e 6f64 6573 2067  mulation nodes g
-0000ca80: 6976 656e 2061 2073 696d 756c 6174 696f  iven a simulatio
-0000ca90: 6e20 4944 2e22 2222 0a0a 2020 2020 2320  n ID."""..    # 
-0000caa0: 4665 7463 6820 7369 6d75 6c61 7469 6f6e  Fetch simulation
-0000cab0: 206e 6f64 6573 0a20 2020 2072 6573 756c   nodes.    resul
-0000cac0: 7420 3d20 5f67 6574 2866 222f 7369 6d75  t = _get(f"/simu
-0000cad0: 6c61 7469 6f6e 2f7b 6964 5f73 696d 756c  lation/{id_simul
-0000cae0: 6174 696f 6e7d 2f6e 6f64 6522 290a 0a20  ation}/node").. 
-0000caf0: 2020 2069 6620 7265 7375 6c74 2e73 7461     if result.sta
-0000cb00: 7475 735f 636f 6465 2021 3d20 3230 303a  tus_code != 200:
-0000cb10: 0a20 2020 2020 2020 205f 6861 6e64 6c65  .        _handle
-0000cb20: 5f65 7272 6f72 2872 6573 756c 742c 2022  _error(result, "
-0000cb30: 4361 6e6e 6f74 2064 656c 6574 6520 7369  Cannot delete si
-0000cb40: 6d75 6c61 7469 6f6e 206e 6f64 6573 2229  mulation nodes")
-0000cb50: 0a0a 2020 2020 6e6f 6465 735f 6c69 7374  ..    nodes_list
-0000cb60: 203d 2072 6573 756c 742e 6a73 6f6e 2829   = result.json()
-0000cb70: 0a0a 2020 2020 2320 4465 6c65 7465 2065  ..    # Delete e
-0000cb80: 6163 6820 6e6f 6465 0a20 2020 2066 6f72  ach node.    for
-0000cb90: 206e 6f64 6520 696e 206e 6f64 6573 5f6c   node in nodes_l
-0000cba0: 6973 743a 0a20 2020 2020 2020 2064 656c  ist:.        del
-0000cbb0: 6574 655f 6e6f 6465 286e 6f64 655b 2269  ete_node(node["i
-0000cbc0: 6422 5d29 0a0a 2020 2020 7265 7375 6c74  d"])..    result
-0000cbd0: 5f6a 736f 6e20 3d20 227b 7d22 0a20 2020  _json = "{}".   
-0000cbe0: 2072 6574 7572 6e20 7265 7375 6c74 5f6a   return result_j
-0000cbf0: 736f 6e0a 0a0a 6465 6620 7570 6461 7465  son...def update
-0000cc00: 5f6e 6f64 6528 6e6f 6465 5f69 643a 2069  _node(node_id: i
-0000cc10: 6e74 2c20 6e6f 6465 5f64 6963 743a 2064  nt, node_dict: d
-0000cc20: 6963 7429 202d 3e20 416e 793a 0a20 2020  ict) -> Any:.   
-0000cc30: 2022 2222 5570 6461 7465 206e 6f64 6520   """Update node 
-0000cc40: 696e 666f 726d 6174 696f 6e20 6769 7665  information give
-0000cc50: 6e20 6120 6e6f 6465 2069 6420 616e 6420  n a node id and 
-0000cc60: 6120 6469 6374 2063 6f6e 7461 696e 696e  a dict containin
-0000cc70: 670a 2020 2020 6e6f 6465 2064 6174 612e  g.    node data.
-0000cc80: 0a20 2020 2022 2222 0a20 2020 2064 6174  .    """.    dat
-0000cc90: 6120 3d20 6a73 6f6e 2e64 756d 7073 286e  a = json.dumps(n
-0000cca0: 6f64 655f 6469 6374 290a 2020 2020 7265  ode_dict).    re
-0000ccb0: 7375 6c74 203d 205f 7075 7428 0a20 2020  sult = _put(.   
-0000ccc0: 2020 2020 2066 222f 6e6f 6465 2f7b 6e6f       f"/node/{no
-0000ccd0: 6465 5f69 647d 222c 0a20 2020 2020 2020  de_id}",.       
-0000cce0: 2064 6174 613d 6461 7461 2c0a 2020 2020   data=data,.    
-0000ccf0: 2020 2020 6865 6164 6572 733d 7b22 436f      headers={"Co
-0000cd00: 6e74 656e 742d 5479 7065 223a 2022 6170  ntent-Type": "ap
-0000cd10: 706c 6963 6174 696f 6e2f 6a73 6f6e 227d  plication/json"}
-0000cd20: 2c0a 2020 2020 290a 0a20 2020 2069 6620  ,.    )..    if 
-0000cd30: 7265 7375 6c74 2e73 7461 7475 735f 636f  result.status_co
-0000cd40: 6465 2021 3d20 3230 303a 0a20 2020 2020  de != 200:.     
-0000cd50: 2020 205f 6861 6e64 6c65 5f65 7272 6f72     _handle_error
-0000cd60: 2872 6573 756c 742c 2022 4361 6e6e 6f74  (result, "Cannot
-0000cd70: 2075 7064 6174 6520 6e6f 6465 2069 6e66   update node inf
-0000cd80: 6f72 6d61 7469 6f6e 2077 6974 6820 636f  ormation with co
-0000cd90: 7265 2041 5049 2229 0a0a 2020 2020 7265  re API")..    re
-0000cda0: 7475 726e 2072 6573 756c 742e 6a73 6f6e  turn result.json
-0000cdb0: 2829 0a0a 0a64 6566 2067 6574 5f6e 6f64  ()...def get_nod
-0000cdc0: 655f 6465 6661 756c 745f 6761 7465 7761  e_default_gatewa
-0000cdd0: 7928 6964 5f6e 6f64 653a 2069 6e74 2920  y(id_node: int) 
-0000cde0: 2d3e 204f 7074 696f 6e61 6c5b 7374 725d  -> Optional[str]
-0000cdf0: 3a0a 2020 2020 2222 2252 6574 7269 6576  :.    """Retriev
-0000ce00: 6520 6e6f 6465 2064 6566 6175 6c74 2067  e node default g
-0000ce10: 6174 6577 6179 2c20 7768 6963 6820 6361  ateway, which ca
-0000ce20: 6e20 6569 7468 6572 2062 6520 616e 2049  n either be an I
-0000ce30: 5020 6164 6472 6573 730a 2020 2020 6f66  P address.    of
-0000ce40: 2074 6865 2066 6f72 6d20 7878 2e78 782e   the form xx.xx.
-0000ce50: 7878 2e78 7820 6f72 204e 6f6e 6520 6966  xx.xx or None if
-0000ce60: 206e 6f20 6761 7465 7761 7920 6973 2073   no gateway is s
-0000ce70: 6574 2e0a 0a20 2020 2022 2222 0a0a 2020  et...    """..  
-0000ce80: 2020 7265 7375 6c74 203d 205f 6765 7428    result = _get(
-0000ce90: 6622 2f6e 6f64 652f 7b69 645f 6e6f 6465  f"/node/{id_node
-0000cea0: 7d2f 6465 6661 756c 745f 6761 7465 7761  }/default_gatewa
-0000ceb0: 7922 290a 0a20 2020 2069 6620 7265 7375  y")..    if resu
-0000cec0: 6c74 2e73 7461 7475 735f 636f 6465 2021  lt.status_code !
-0000ced0: 3d20 3230 303a 0a20 2020 2020 2020 205f  = 200:.        _
-0000cee0: 6861 6e64 6c65 5f65 7272 6f72 280a 2020  handle_error(.  
-0000cef0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0000cf00: 2c20 2243 616e 6e6f 7420 7265 7472 6965  , "Cannot retrie
-0000cf10: 7665 206e 6f64 6520 6465 6661 756c 7420  ve node default 
-0000cf20: 6761 7465 7761 7920 6672 6f6d 2049 5420  gateway from IT 
-0000cf30: 5369 6d75 6c61 7469 6f6e 2041 5049 220a  Simulation API".
-0000cf40: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
-0000cf50: 6566 6175 6c74 5f67 6174 6577 6179 203d  efault_gateway =
-0000cf60: 2072 6573 756c 742e 6a73 6f6e 2829 0a0a   result.json()..
-0000cf70: 2020 2020 7265 7475 726e 2064 6566 6175      return defau
-0000cf80: 6c74 5f67 6174 6577 6179 0a0a 0a64 6566  lt_gateway...def
-0000cf90: 2067 6574 5f6e 6f64 655f 7374 6174 6973   get_node_statis
-0000cfa0: 7469 6373 5f62 795f 6964 2869 645f 6e6f  tics_by_id(id_no
-0000cfb0: 6465 3a20 696e 7429 202d 3e20 416e 793a  de: int) -> Any:
-0000cfc0: 0a20 2020 2022 2222 0a20 2020 2052 6574  .    """.    Ret
-0000cfd0: 7572 6e20 6167 6772 6567 6174 6564 2073  urn aggregated s
-0000cfe0: 7461 7469 7374 6963 7320 6672 6f6d 2043  tatistics from C
-0000cff0: 5055 2c20 6d65 6d6f 7279 2c20 626c 6f63  PU, memory, bloc
-0000d000: 6b20 6465 7669 6365 7320 616e 6420 6e65  k devices and ne
-0000d010: 7477 6f72 6b20 696e 7465 7266 6163 6573  twork interfaces
-0000d020: 2e0a 2020 2020 4e6f 7465 3a20 796f 7520  ..    Note: you 
-0000d030: 6361 6e20 6765 7420 7468 6520 6e6f 6465  can get the node
-0000d040: 2049 4473 2075 7369 6e67 2074 6865 2073   IDs using the s
-0000d050: 696d 755f 7374 6174 7573 2063 6f6d 6d61  imu_status comma
-0000d060: 6e64 2028 6f72 2074 6865 2066 6574 6368  nd (or the fetch
-0000d070: 5f73 696d 756c 6174 696f 6e73 2829 2066  _simulations() f
-0000d080: 756e 6374 696f 6e29 2e0a 2020 2020 2222  unction)..    ""
-0000d090: 220a 2020 2020 7265 7375 6c74 203d 205f  ".    result = _
-0000d0a0: 6765 7428 6622 2f6e 6f64 652f 7b69 645f  get(f"/node/{id_
-0000d0b0: 6e6f 6465 7d2f 7374 6174 7322 290a 0a20  node}/stats").. 
-0000d0c0: 2020 2069 6620 7265 7375 6c74 2e73 7461     if result.sta
-0000d0d0: 7475 735f 636f 6465 2021 3d20 3230 303a  tus_code != 200:
-0000d0e0: 0a20 2020 2020 2020 205f 6861 6e64 6c65  .        _handle
-0000d0f0: 5f65 7272 6f72 2872 6573 756c 742c 2022  _error(result, "
-0000d100: 4361 6e6e 6f74 2072 6574 7269 6576 6520  Cannot retrieve 
-0000d110: 6e6f 6465 2073 7461 7469 7374 6963 7322  node statistics"
-0000d120: 290a 0a20 2020 2072 6574 7572 6e20 7265  )..    return re
-0000d130: 7375 6c74 2e6a 736f 6e28 290a 0a0a 6465  sult.json()...de
-0000d140: 6620 6e6f 6465 5f6c 6f67 7328 6964 5f6e  f node_logs(id_n
-0000d150: 6f64 653a 2069 6e74 2920 2d3e 2041 6e79  ode: int) -> Any
-0000d160: 3a0a 2020 2020 2222 220a 2020 2020 5265  :.    """.    Re
-0000d170: 7472 6965 7665 206c 6f67 7320 6672 6f6d  trieve logs from
-0000d180: 2073 7065 6369 6669 6564 206e 6f64 6520   specified node 
-0000d190: 286f 6e6c 7920 776f 726b 2066 6f72 2044  (only work for D
-0000d1a0: 6f63 6b65 7220 6e6f 6465 292e 0a0a 2020  ocker node)...  
-0000d1b0: 2020 5265 7475 726e 2074 6865 206c 6f67    Return the log
-0000d1c0: 7320 7374 7269 6e67 2e0a 2020 2020 2222  s string..    ""
-0000d1d0: 220a 0a20 2020 2023 2043 6865 636b 2074  "..    # Check t
-0000d1e0: 6861 7420 7468 6520 7461 7267 6574 206e  hat the target n
-0000d1f0: 6f64 6520 6973 2061 2064 6f63 6b65 7220  ode is a docker 
-0000d200: 6e6f 6465 2028 6e6f 6465 5f65 7865 6320  node (node_exec 
-0000d210: 6f6e 6c79 0a20 2020 2023 2077 6f72 6b73  only.    # works
-0000d220: 2066 6f72 2044 6f63 6b65 7220 6e6f 6465   for Docker node
-0000d230: 2066 6f72 206e 6f77 290a 2020 2020 6e6f   for now).    no
-0000d240: 6465 203d 2066 6574 6368 5f6e 6f64 6528  de = fetch_node(
-0000d250: 6964 5f6e 6f64 6529 0a20 2020 2069 6620  id_node).    if 
-0000d260: 6e6f 6465 5b22 7479 7065 225d 2021 3d20  node["type"] != 
-0000d270: 2264 6f63 6b65 7222 3a0a 2020 2020 2020  "docker":.      
-0000d280: 2020 7261 6973 6520 4578 6365 7074 696f    raise Exceptio
-0000d290: 6e28 2243 616e 6e6f 7420 6578 6563 7574  n("Cannot execut
-0000d2a0: 6520 636f 6d6d 616e 6420 666f 7220 6e6f  e command for no
-0000d2b0: 6465 7320 6469 6666 6572 656e 7420 6672  des different fr
-0000d2c0: 6f6d 2064 6f63 6b65 7220 6e6f 6465 7322  om docker nodes"
-0000d2d0: 290a 0a20 2020 2072 6573 756c 7420 3d20  )..    result = 
-0000d2e0: 5f67 6574 2866 222f 6e6f 6465 2f7b 6964  _get(f"/node/{id
-0000d2f0: 5f6e 6f64 657d 2f6c 6f67 7322 290a 0a20  _node}/logs").. 
-0000d300: 2020 2069 6620 7265 7375 6c74 2e73 7461     if result.sta
-0000d310: 7475 735f 636f 6465 2021 3d20 3230 303a  tus_code != 200:
-0000d320: 0a20 2020 2020 2020 205f 6861 6e64 6c65  .        _handle
-0000d330: 5f65 7272 6f72 2872 6573 756c 742c 2022  _error(result, "
-0000d340: 4361 6e6e 6f74 2072 6574 7269 6576 6520  Cannot retrieve 
-0000d350: 6c6f 6773 2066 726f 6d20 4954 2053 696d  logs from IT Sim
-0000d360: 756c 6174 696f 6e20 4150 4922 290a 0a20  ulation API").. 
-0000d370: 2020 206c 6f67 7320 3d20 7265 7375 6c74     logs = result
-0000d380: 2e6a 736f 6e28 290a 0a20 2020 2072 6574  .json()..    ret
-0000d390: 7572 6e20 6c6f 6773 0a0a 0a64 6566 206e  urn logs...def n
-0000d3a0: 6f64 655f 6578 6563 2869 645f 6e6f 6465  ode_exec(id_node
-0000d3b0: 3a20 696e 742c 2063 6f6d 6d61 6e64 3a20  : int, command: 
-0000d3c0: 7374 7229 202d 3e20 416e 793a 0a20 2020  str) -> Any:.   
-0000d3d0: 2022 2222 0a20 2020 2045 7865 6375 7465   """.    Execute
-0000d3e0: 2061 2063 6f6d 6d61 6e64 206f 6e20 7370   a command on sp
-0000d3f0: 6563 6966 6965 6420 6e6f 6465 2028 6f6e  ecified node (on
-0000d400: 6c79 2077 6f72 6b20 666f 7220 446f 636b  ly work for Dock
-0000d410: 6572 206e 6f64 6529 2e0a 0a20 2020 2052  er node)...    R
-0000d420: 6574 7572 6e20 6120 7475 706c 6520 2865  eturn a tuple (e
-0000d430: 7869 745f 636f 6465 3a20 696e 742c 2073  xit_code: int, s
-0000d440: 7464 6f75 743a 2073 7472 2c20 7374 6465  tdout: str, stde
-0000d450: 7272 3a20 7374 7229 206f 6620 7468 6520  rr: str) of the 
-0000d460: 6578 6563 7574 6564 2063 6f6d 6d61 6e64  executed command
-0000d470: 2e0a 2020 2020 2222 220a 0a20 2020 2023  ..    """..    #
-0000d480: 2043 6865 636b 2074 6861 7420 7468 6520   Check that the 
-0000d490: 7461 7267 6574 206e 6f64 6520 6973 2061  target node is a
-0000d4a0: 2064 6f63 6b65 7220 6e6f 6465 2028 6e6f   docker node (no
-0000d4b0: 6465 5f65 7865 6320 6f6e 6c79 0a20 2020  de_exec only.   
-0000d4c0: 2023 2077 6f72 6b73 2066 6f72 2044 6f63   # works for Doc
-0000d4d0: 6b65 7220 6e6f 6465 2066 6f72 206e 6f77  ker node for now
-0000d4e0: 290a 2020 2020 6e6f 6465 203d 2066 6574  ).    node = fet
-0000d4f0: 6368 5f6e 6f64 6528 6964 5f6e 6f64 6529  ch_node(id_node)
-0000d500: 0a20 2020 2069 6620 6e6f 6465 5b22 7479  .    if node["ty
-0000d510: 7065 225d 2021 3d20 2264 6f63 6b65 7222  pe"] != "docker"
-0000d520: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
-0000d530: 4578 6365 7074 696f 6e28 2243 616e 6e6f  Exception("Canno
-0000d540: 7420 6578 6563 7574 6520 636f 6d6d 616e  t execute comman
-0000d550: 6420 666f 7220 6e6f 6465 7320 6469 6666  d for nodes diff
-0000d560: 6572 656e 7420 6672 6f6d 2064 6f63 6b65  erent from docke
-0000d570: 7220 6e6f 6465 7322 290a 0a20 2020 2073  r nodes")..    s
-0000d580: 7461 7475 735f 6b65 7920 3d20 2273 7461  tatus_key = "sta
-0000d590: 7475 7322 0a20 2020 2065 7869 745f 636f  tus".    exit_co
-0000d5a0: 6465 203d 2022 6578 6974 5f63 6f64 6522  de = "exit_code"
-0000d5b0: 0a20 2020 2073 7464 6f75 7420 3d20 2273  .    stdout = "s
-0000d5c0: 7464 6f75 7422 0a20 2020 2073 7464 6572  tdout".    stder
-0000d5d0: 7220 3d20 2273 7464 6572 7222 0a0a 2020  r = "stderr"..  
-0000d5e0: 2020 706f 7374 5f64 6174 6120 3d20 7b22    post_data = {"
-0000d5f0: 636f 6d6d 616e 6422 3a20 636f 6d6d 616e  command": comman
-0000d600: 647d 0a20 2020 2064 6174 6120 3d20 6a73  d}.    data = js
-0000d610: 6f6e 2e64 756d 7073 2870 6f73 745f 6461  on.dumps(post_da
-0000d620: 7461 290a 2020 2020 7265 7375 6c74 203d  ta).    result =
-0000d630: 205f 706f 7374 280a 2020 2020 2020 2020   _post(.        
-0000d640: 6622 2f6e 6f64 652f 7b69 645f 6e6f 6465  f"/node/{id_node
-0000d650: 7d2f 6578 6563 222c 2064 6174 613d 6461  }/exec", data=da
-0000d660: 7461 2c20 6865 6164 6572 733d 7b22 436f  ta, headers={"Co
-0000d670: 6e74 656e 742d 5479 7065 223a 2022 6170  ntent-Type": "ap
-0000d680: 706c 6963 6174 696f 6e2f 6a73 6f6e 227d  plication/json"}
-0000d690: 0a20 2020 2029 0a0a 2020 2020 6966 2028  .    )..    if (
-0000d6a0: 0a20 2020 2020 2020 2072 6573 756c 742e  .        result.
-0000d6b0: 7374 6174 7573 5f63 6f64 6520 213d 2032  status_code != 2
-0000d6c0: 3030 0a20 2020 2020 2020 206f 7220 7374  00.        or st
-0000d6d0: 6174 7573 5f6b 6579 206e 6f74 2069 6e20  atus_key not in 
-0000d6e0: 7265 7375 6c74 2e6a 736f 6e28 290a 2020  result.json().  
-0000d6f0: 2020 2020 2020 6f72 2072 6573 756c 742e        or result.
-0000d700: 6a73 6f6e 2829 5b73 7461 7475 735f 6b65  json()[status_ke
-0000d710: 795d 2021 3d20 2253 5441 5254 4544 220a  y] != "STARTED".
-0000d720: 2020 2020 293a 0a20 2020 2020 2020 205f      ):.        _
-0000d730: 6861 6e64 6c65 5f65 7272 6f72 2872 6573  handle_error(res
-0000d740: 756c 742c 2022 4361 6e6e 6f74 2069 6e69  ult, "Cannot ini
-0000d750: 7469 6174 6520 6578 6563 2063 6f6d 6d61  tiate exec comma
-0000d760: 6e64 2066 726f 6d20 4954 2053 696d 756c  nd from IT Simul
-0000d770: 6174 696f 6e20 4150 4922 290a 0a20 2020  ation API")..   
-0000d780: 206c 6f67 6765 722e 696e 666f 2866 225b   logger.info(f"[
-0000d790: 2b5d 2045 7865 6375 7469 6e67 2063 6f6d  +] Executing com
-0000d7a0: 6d61 6e64 2027 7b63 6f6d 6d61 6e64 7d27  mand '{command}'
-0000d7b0: 2066 6f72 206e 6f64 6520 277b 6964 5f6e   for node '{id_n
-0000d7c0: 6f64 657d 272e 2e2e 2229 0a0a 2020 2020  ode}'...")..    
-0000d7d0: 2320 5761 6974 2066 6f72 2074 6865 206f  # Wait for the o
-0000d7e0: 7065 7261 7469 6f6e 2074 6f20 6265 2063  peration to be c
-0000d7f0: 6f6d 706c 6574 6564 2069 6e20 6261 636b  ompleted in back
-0000d800: 656e 640a 2020 2020 2320 4e6f 7465 203a  end.    # Note :
-0000d810: 206c 6f6f 7020 696e 7370 6972 6564 2066   loop inspired f
-0000d820: 726f 6d20 5f73 696d 756c 6174 696f 6e5f  rom _simulation_
-0000d830: 6578 6563 7574 655f 6f70 6572 6174 696f  execute_operatio
-0000d840: 6e0a 2020 2020 7768 696c 6520 5472 7565  n.    while True
-0000d850: 3a0a 2020 2020 2020 2020 2320 536c 6565  :.        # Slee
-0000d860: 7020 6265 666f 7265 206e 6578 7420 6974  p before next it
-0000d870: 6572 6174 696f 6e0a 2020 2020 2020 2020  eration.        
-0000d880: 7469 6d65 2e73 6c65 6570 2832 290a 0a20  time.sleep(2).. 
-0000d890: 2020 2020 2020 2023 2046 6574 6368 2074         # Fetch t
-0000d8a0: 6865 2063 7572 7265 6e74 2073 7461 7475  he current statu
-0000d8b0: 7320 6f66 2074 6865 206d 656d 6475 6d70  s of the memdump
-0000d8c0: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-0000d8d0: 3d20 5f67 6574 2866 222f 6e6f 6465 2f7b  = _get(f"/node/{
-0000d8e0: 6964 5f6e 6f64 657d 2f65 7865 635f 7374  id_node}/exec_st
-0000d8f0: 6174 7573 2229 0a0a 2020 2020 2020 2020  atus")..        
-0000d900: 6966 2072 6573 756c 742e 7374 6174 7573  if result.status
-0000d910: 5f63 6f64 6520 213d 2032 3030 3a0a 2020  _code != 200:.  
-0000d920: 2020 2020 2020 2020 2020 5f68 616e 646c            _handl
-0000d930: 655f 6572 726f 7228 0a20 2020 2020 2020  e_error(.       
-0000d940: 2020 2020 2020 2020 2072 6573 756c 742c           result,
-0000d950: 2022 4361 6e6e 6f74 2067 6574 2073 7461   "Cannot get sta
-0000d960: 7475 7320 6f66 2065 7865 6320 636f 6d6d  tus of exec comm
-0000d970: 616e 6420 6672 6f6d 2049 5420 5369 6d75  and from IT Simu
-0000d980: 6c61 7469 6f6e 2041 5049 220a 2020 2020  lation API".    
-0000d990: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-0000d9a0: 2020 2072 6573 756c 745f 6a73 6f6e 203d     result_json =
-0000d9b0: 2072 6573 756c 742e 6a73 6f6e 2829 0a20   result.json(). 
-0000d9c0: 2020 2020 2020 2069 6620 6e6f 7420 2861         if not (a
-0000d9d0: 6c6c 286b 2069 6e20 7265 7375 6c74 5f6a  ll(k in result_j
-0000d9e0: 736f 6e20 666f 7220 6b20 696e 2028 6578  son for k in (ex
-0000d9f0: 6974 5f63 6f64 652c 2073 7464 6f75 742c  it_code, stdout,
-0000da00: 2073 7464 6572 722c 2073 7461 7475 735f   stderr, status_
-0000da10: 6b65 7929 2929 3a0a 2020 2020 2020 2020  key))):.        
-0000da20: 2020 2020 7261 6973 6520 4578 6365 7074      raise Except
-0000da30: 696f 6e28 0a20 2020 2020 2020 2020 2020  ion(.           
-0000da40: 2020 2020 2066 2243 6f6e 7465 6e74 7320       f"Contents 
-0000da50: 6f66 2065 7865 6320 636f 6d6d 616e 6420  of exec command 
-0000da60: 7374 6174 7573 2075 7064 6174 6520 6973  status update is
-0000da70: 206e 6f74 2069 6e20 7468 6520 6578 7065   not in the expe
-0000da80: 6374 6564 2066 6f72 6d61 7420 2861 7474  cted format (att
-0000da90: 7269 6275 7465 7320 277b 6578 6974 5f63  ributes '{exit_c
-0000daa0: 6f64 657d 272c 2027 7b73 7464 6f75 747d  ode}', '{stdout}
-0000dab0: 272c 2027 7b73 7464 6572 727d 2720 616e  ', '{stderr}' an
-0000dac0: 6420 277b 7374 6174 7573 5f6b 6579 7d27  d '{status_key}'
-0000dad0: 2065 7870 6563 7465 6429 220a 2020 2020   expected)".    
-0000dae0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-0000daf0: 2020 2023 204c 6f67 2069 6e66 6f20 6f6e     # Log info on
-0000db00: 2070 726f 6772 6573 7369 6f6e 0a20 2020   progression.   
-0000db10: 2020 2020 2069 6620 7265 7375 6c74 5f6a       if result_j
-0000db20: 736f 6e5b 7374 6174 7573 5f6b 6579 5d20  son[status_key] 
-0000db30: 3d3d 2022 5354 4152 5445 4422 3a0a 2020  == "STARTED":.  
-0000db40: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-0000db50: 2e69 6e66 6f28 0a20 2020 2020 2020 2020  .info(.         
-0000db60: 2020 2020 2020 2066 2220 205b 2b5d 2043         f"  [+] C
-0000db70: 7572 7265 6e74 6c79 2077 6169 7469 6e67  urrently waiting
-0000db80: 2066 6f72 2065 7865 6320 636f 6d6d 616e   for exec comman
-0000db90: 6420 666f 7220 6e6f 6465 2027 7b69 645f  d for node '{id_
-0000dba0: 6e6f 6465 7d27 2920 746f 2073 7461 7274  node}') to start
-0000dbb0: 2e2e 2e22 0a20 2020 2020 2020 2020 2020  ...".           
-0000dbc0: 2029 0a20 2020 2020 2020 2065 6c69 6620   ).        elif 
-0000dbd0: 7265 7375 6c74 5f6a 736f 6e5b 7374 6174  result_json[stat
-0000dbe0: 7573 5f6b 6579 5d20 3d3d 2022 5052 4f47  us_key] == "PROG
-0000dbf0: 5245 5353 223a 0a20 2020 2020 2020 2020  RESS":.         
-0000dc00: 2020 206c 6f67 6765 722e 696e 666f 280a     logger.info(.
-0000dc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc20: 6622 2020 5b2b 5d20 4375 7272 656e 746c  f"  [+] Currentl
-0000dc30: 7920 7065 7266 6f72 6d69 6e67 2065 7865  y performing exe
-0000dc40: 6320 636f 6d6d 616e 6420 666f 7220 6e6f  c command for no
-0000dc50: 6465 2027 7b69 645f 6e6f 6465 7d27 292e  de '{id_node}').
-0000dc60: 2e2e 220a 2020 2020 2020 2020 2020 2020  ..".            
-0000dc70: 290a 2020 2020 2020 2020 656c 6966 2072  ).        elif r
-0000dc80: 6573 756c 745f 6a73 6f6e 5b73 7461 7475  esult_json[statu
-0000dc90: 735f 6b65 795d 203d 3d20 2253 5543 4345  s_key] == "SUCCE
-0000dca0: 5353 223a 0a20 2020 2020 2020 2020 2020  SS":.           
-0000dcb0: 2062 7265 616b 0a20 2020 2020 2020 2065   break.        e
-0000dcc0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000dcd0: 2072 6169 7365 2045 7863 6570 7469 6f6e   raise Exception
-0000dce0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000dcf0: 2020 2245 7272 6f72 2064 7572 696e 6720    "Error during 
-0000dd00: 6578 6563 2063 6f6d 6d61 6e64 2066 6f72  exec command for
-0000dd10: 206e 6f64 6520 7b7d 206f 7065 7261 7469   node {} operati
-0000dd20: 6f6e 3a20 277b 7d27 222e 666f 726d 6174  on: '{}'".format
-0000dd30: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000dd40: 2020 2020 2020 6964 5f6e 6f64 652c 2072        id_node, r
-0000dd50: 6573 756c 745f 6a73 6f6e 5b73 7461 7475  esult_json[statu
-0000dd60: 735f 6b65 795d 0a20 2020 2020 2020 2020  s_key].         
-0000dd70: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000dd80: 2020 2020 2029 0a0a 2020 2020 6c6f 6767       )..    logg
-0000dd90: 6572 2e69 6e66 6f28 225b 2b5d 204e 6f64  er.info("[+] Nod
-0000dda0: 6520 6578 6563 2063 6f6d 6d61 6e64 2066  e exec command f
-0000ddb0: 696e 6973 6865 6422 290a 0a20 2020 2072  inished")..    r
-0000ddc0: 6574 7572 6e20 2872 6573 756c 745f 6a73  eturn (result_js
-0000ddd0: 6f6e 5b65 7869 745f 636f 6465 5d2c 2072  on[exit_code], r
-0000dde0: 6573 756c 745f 6a73 6f6e 5b73 7464 6f75  esult_json[stdou
-0000ddf0: 745d 2c20 7265 7375 6c74 5f6a 736f 6e5b  t], result_json[
-0000de00: 7374 6465 7272 5d29 0a0a 0a64 6566 206e  stderr])...def n
-0000de10: 6f64 655f 6d65 6d6f 7279 6475 6d70 2869  ode_memorydump(i
-0000de20: 645f 6e6f 6465 3a20 696e 7429 202d 3e20  d_node: int) -> 
-0000de30: 416e 793a 0a20 2020 2022 2222 0a20 2020  Any:.    """.   
-0000de40: 2052 6574 7572 6e20 5241 4d20 6475 6d70   Return RAM dump
-0000de50: 206f 6620 6120 6e6f 6465 2069 6e20 6120   of a node in a 
-0000de60: 7275 6e6e 696e 6720 7369 6d75 6c61 7469  running simulati
-0000de70: 6f6e 0a20 2020 204e 6f74 653a 2079 6f75  on.    Note: you
-0000de80: 2063 616e 2067 6574 2074 6865 206e 6f64   can get the nod
-0000de90: 6520 4944 7320 7573 696e 6720 7468 6520  e IDs using the 
-0000dea0: 7369 6d75 5f73 7461 7475 7320 636f 6d6d  simu_status comm
-0000deb0: 616e 6420 286f 7220 7468 6520 6665 7463  and (or the fetc
-0000dec0: 685f 7369 6d75 6c61 7469 6f6e 7328 2920  h_simulations() 
-0000ded0: 6675 6e63 7469 6f6e 292e 0a20 2020 2022  function)..    "
-0000dee0: 2222 0a0a 2020 2020 2323 2054 4f44 4f3a  ""..    ## TODO:
-0000def0: 2069 6d70 6c65 6d65 6e74 2074 6869 7320   implement this 
-0000df00: 6f70 6572 6174 696f 6e20 696e 2041 5049  operation in API
-0000df10: 2062 6163 6b65 6e64 0a20 2020 2072 6169   backend.    rai
-0000df20: 7365 204e 6f74 496d 706c 656d 656e 7465  se NotImplemente
-0000df30: 6445 7272 6f72 2829 0a0a 2020 2020 2320  dError()..    # 
-0000df40: 6669 6c65 5f70 6174 685f 6b65 7920 3d20  file_path_key = 
-0000df50: 2266 696c 655f 7061 7468 220a 2020 2020  "file_path".    
-0000df60: 2320 6669 6c65 5f73 697a 655f 6b65 7920  # file_size_key 
-0000df70: 3d20 2266 696c 655f 7369 7a65 220a 2020  = "file_size".  
-0000df80: 2020 2320 7374 6174 7573 5f6b 6579 203d    # status_key =
-0000df90: 2022 7374 6174 7573 220a 0a20 2020 2023   "status"..    #
-0000dfa0: 2072 6573 756c 7420 3d20 5f67 6574 2866   result = _get(f
-0000dfb0: 222f 6e6f 6465 2f7b 6964 5f6e 6f64 657d  "/node/{id_node}
-0000dfc0: 2f6d 656d 6f72 7964 756d 7022 290a 0a20  /memorydump").. 
-0000dfd0: 2020 2023 2069 6620 280a 2020 2020 2320     # if (.    # 
-0000dfe0: 2020 2020 7265 7375 6c74 2e73 7461 7475      result.statu
-0000dff0: 735f 636f 6465 2021 3d20 3230 300a 2020  s_code != 200.  
-0000e000: 2020 2320 2020 2020 6f72 2073 7461 7475    #     or statu
-0000e010: 735f 6b65 7920 6e6f 7420 696e 2072 6573  s_key not in res
-0000e020: 756c 742e 6a73 6f6e 2829 0a20 2020 2023  ult.json().    #
-0000e030: 2020 2020 206f 7220 7265 7375 6c74 2e6a       or result.j
-0000e040: 736f 6e28 295b 7374 6174 7573 5f6b 6579  son()[status_key
-0000e050: 5d20 213d 2022 5354 4152 5445 4422 0a20  ] != "STARTED". 
-0000e060: 2020 2023 2029 3a0a 2020 2020 2320 2020     # ):.    #   
-0000e070: 2020 5f68 616e 646c 655f 6572 726f 7228    _handle_error(
-0000e080: 7265 7375 6c74 2c20 2243 616e 6e6f 7420  result, "Cannot 
-0000e090: 696e 6974 6961 7465 206e 6f64 6520 6d65  initiate node me
-0000e0a0: 6d6f 7279 2064 756d 7020 6672 6f6d 2063  mory dump from c
-0000e0b0: 6f72 6520 4150 4922 290a 0a20 2020 2023  ore API")..    #
-0000e0c0: 206c 6f67 6765 722e 696e 666f 2822 5b2b   logger.info("[+
-0000e0d0: 5d20 496e 6974 6961 6c69 7a65 6420 6d65  ] Initialized me
-0000e0e0: 6d6f 7279 2064 756d 7020 6f66 206e 6f64  mory dump of nod
-0000e0f0: 6520 277b 7d27 2e2e 2e22 2e66 6f72 6d61  e '{}'...".forma
-0000e100: 7428 6964 5f6e 6f64 6529 290a 0a20 2020  t(id_node))..   
-0000e110: 2023 2023 2057 6169 7420 666f 7220 7468   # # Wait for th
-0000e120: 6520 6f70 6572 6174 696f 6e20 746f 2062  e operation to b
-0000e130: 6520 636f 6d70 6c65 7465 6420 696e 2062  e completed in b
-0000e140: 6163 6b65 6e64 0a20 2020 2023 2023 204e  ackend.    # # N
-0000e150: 6f74 6520 3a20 6c6f 6f70 2069 6e73 7069  ote : loop inspi
-0000e160: 7265 6420 6672 6f6d 205f 7369 6d75 6c61  red from _simula
-0000e170: 7469 6f6e 5f65 7865 6375 7465 5f6f 7065  tion_execute_ope
-0000e180: 7261 7469 6f6e 0a20 2020 2023 2077 6869  ration.    # whi
-0000e190: 6c65 2054 7275 653a 0a20 2020 2023 2020  le True:.    #  
-0000e1a0: 2020 2023 2053 6c65 6570 2062 6566 6f72     # Sleep befor
-0000e1b0: 6520 6e65 7874 2069 7465 7261 7469 6f6e  e next iteration
-0000e1c0: 0a20 2020 2023 2020 2020 2074 696d 652e  .    #     time.
-0000e1d0: 736c 6565 7028 3229 0a0a 2020 2020 2320  sleep(2)..    # 
-0000e1e0: 2020 2020 2320 4665 7463 6820 7468 6520      # Fetch the 
-0000e1f0: 6375 7272 656e 7420 7374 6174 7573 206f  current status o
-0000e200: 6620 7468 6520 6d65 6d64 756d 700a 2020  f the memdump.  
-0000e210: 2020 2320 2020 2020 7265 7375 6c74 203d    #     result =
-0000e220: 205f 6765 7428 6622 2f6e 6f64 652f 7b69   _get(f"/node/{i
-0000e230: 645f 6e6f 6465 7d2f 6d65 6d6f 7279 6475  d_node}/memorydu
-0000e240: 6d70 5f73 7461 7475 7322 290a 0a20 2020  mp_status")..   
-0000e250: 2023 2020 2020 2069 6620 7265 7375 6c74   #     if result
-0000e260: 2e73 7461 7475 735f 636f 6465 2021 3d20  .status_code != 
-0000e270: 3230 303a 0a20 2020 2023 2020 2020 2020  200:.    #      
-0000e280: 2020 205f 6861 6e64 6c65 5f65 7272 6f72     _handle_error
-0000e290: 2872 6573 756c 742c 2022 4361 6e6e 6f74  (result, "Cannot
-0000e2a0: 2067 6574 2073 7461 7475 7320 6f66 206e   get status of n
-0000e2b0: 6f64 6520 6d65 6d6f 7279 2064 756d 7020  ode memory dump 
-0000e2c0: 6672 6f6d 2063 6f72 6520 4150 4922 290a  from core API").
-0000e2d0: 0a20 2020 2023 2020 2020 2072 6573 756c  .    #     resul
-0000e2e0: 745f 6a73 6f6e 203d 2072 6573 756c 742e  t_json = result.
-0000e2f0: 6a73 6f6e 2829 0a20 2020 2023 2020 2020  json().    #    
-0000e300: 2070 7269 6e74 2872 6573 756c 745f 6a73   print(result_js
-0000e310: 6f6e 290a 2020 2020 2320 2020 2020 6966  on).    #     if
-0000e320: 206e 6f74 2028 0a20 2020 2023 2020 2020   not (.    #    
-0000e330: 2020 2020 2061 6c6c 286b 2069 6e20 7265       all(k in re
-0000e340: 7375 6c74 5f6a 736f 6e20 666f 7220 6b20  sult_json for k 
-0000e350: 696e 2028 6669 6c65 5f70 6174 685f 6b65  in (file_path_ke
-0000e360: 792c 2066 696c 655f 7369 7a65 5f6b 6579  y, file_size_key
-0000e370: 2c20 7374 6174 7573 5f6b 6579 2929 0a20  , status_key)). 
-0000e380: 2020 2023 2020 2020 2029 3a0a 2020 2020     #     ):.    
-0000e390: 2320 2020 2020 2020 2020 7261 6973 6520  #         raise 
-0000e3a0: 4578 6365 7074 696f 6e28 0a20 2020 2023  Exception(.    #
-0000e3b0: 2020 2020 2020 2020 2020 2020 2066 2243               f"C
-0000e3c0: 6f6e 7465 6e74 7320 6f66 206d 656d 6f72  ontents of memor
-0000e3d0: 7920 6475 6d70 2073 7461 7475 7320 7570  y dump status up
-0000e3e0: 6461 7465 2069 7320 6e6f 7420 696e 2074  date is not in t
-0000e3f0: 6865 2065 7870 6563 7465 6420 666f 726d  he expected form
-0000e400: 6174 2028 6174 7472 6962 7574 6573 2027  at (attributes '
-0000e410: 7b66 696c 655f 7061 7468 5f6b 6579 7d27  {file_path_key}'
-0000e420: 2c20 277b 6669 6c65 5f73 697a 655f 6b65  , '{file_size_ke
-0000e430: 797d 2720 616e 6420 277b 7374 6174 7573  y}' and '{status
-0000e440: 5f6b 6579 7d27 2065 7870 6563 7465 6429  _key}' expected)
-0000e450: 220a 2020 2020 2320 2020 2020 2020 2020  ".    #         
-0000e460: 290a 0a20 2020 2023 2020 2020 2023 204c  )..    #     # L
-0000e470: 6f67 2069 6e66 6f20 6f6e 2070 726f 6772  og info on progr
-0000e480: 6573 7369 6f6e 0a20 2020 2023 2020 2020  ession.    #    
-0000e490: 2069 6620 7265 7375 6c74 5f6a 736f 6e5b   if result_json[
-0000e4a0: 7374 6174 7573 5f6b 6579 5d20 3d3d 2022  status_key] == "
-0000e4b0: 5354 4152 5445 4422 3a0a 2020 2020 2320  STARTED":.    # 
-0000e4c0: 2020 2020 2020 2020 7061 7373 0a20 2020          pass.   
-0000e4d0: 2023 2020 2020 2065 6c69 6620 7265 7375   #     elif resu
-0000e4e0: 6c74 5f6a 736f 6e5b 7374 6174 7573 5f6b  lt_json[status_k
-0000e4f0: 6579 5d20 3d3d 2022 5052 4f47 5245 5353  ey] == "PROGRESS
-0000e500: 223a 0a20 2020 2023 2020 2020 2020 2020  ":.    #        
-0000e510: 206c 6f67 6765 722e 696e 666f 280a 2020   logger.info(.  
-0000e520: 2020 2320 2020 2020 2020 2020 2020 2020    #             
-0000e530: 2220 205b 2b5d 2043 7572 7265 6e74 6c79  "  [+] Currently
-0000e540: 2070 6572 666f 726d 696e 6720 6d65 6d6f   performing memo
-0000e550: 7279 2064 756d 7020 6f66 206e 6f64 6520  ry dump of node 
-0000e560: 277b 7d27 2028 6375 7272 656e 7420 6475  '{}' (current du
-0000e570: 6d70 2066 696c 6520 7369 7a65 2069 7320  mp file size is 
-0000e580: 7b7d 292e 2e2e 222e 666f 726d 6174 280a  {})...".format(.
-0000e590: 2020 2020 2320 2020 2020 2020 2020 2020      #           
-0000e5a0: 2020 2020 2020 6964 5f6e 6f64 652c 206e        id_node, n
-0000e5b0: 6174 7572 616c 7369 7a65 2872 6573 756c  aturalsize(resul
-0000e5c0: 745f 6a73 6f6e 5b66 696c 655f 7369 7a65  t_json[file_size
-0000e5d0: 5f6b 6579 5d2c 2062 696e 6172 793d 5472  _key], binary=Tr
-0000e5e0: 7565 290a 2020 2020 2320 2020 2020 2020  ue).    #       
-0000e5f0: 2020 2020 2020 290a 2020 2020 2320 2020        ).    #   
-0000e600: 2020 2020 2020 290a 2020 2020 2320 2020        ).    #   
-0000e610: 2020 656c 6966 2072 6573 756c 745f 6a73    elif result_js
-0000e620: 6f6e 5b73 7461 7475 735f 6b65 795d 203d  on[status_key] =
-0000e630: 3d20 2253 5543 4345 5353 223a 0a20 2020  = "SUCCESS":.   
-0000e640: 2023 2020 2020 2020 2020 2062 7265 616b   #         break
-0000e650: 0a20 2020 2023 2020 2020 2065 6c73 653a  .    #     else:
-0000e660: 0a20 2020 2023 2020 2020 2020 2020 2072  .    #         r
-0000e670: 6169 7365 2045 7863 6570 7469 6f6e 280a  aise Exception(.
-0000e680: 2020 2020 2320 2020 2020 2020 2020 2020      #           
-0000e690: 2020 2245 7272 6f72 2064 7572 696e 6720    "Error during 
-0000e6a0: 6d65 6d6f 7279 2064 756d 7020 6f66 206e  memory dump of n
-0000e6b0: 6f64 6520 7b7d 206f 7065 7261 7469 6f6e  ode {} operation
-0000e6c0: 3a20 277b 7d27 222e 666f 726d 6174 280a  : '{}'".format(.
-0000e6d0: 2020 2020 2320 2020 2020 2020 2020 2020      #           
-0000e6e0: 2020 2020 2020 6964 5f6e 6f64 652c 2072        id_node, r
-0000e6f0: 6573 756c 745f 6a73 6f6e 5b73 7461 7475  esult_json[statu
-0000e700: 735f 6b65 795d 0a20 2020 2023 2020 2020  s_key].    #    
-0000e710: 2020 2020 2020 2020 2029 0a20 2020 2023           ).    #
-0000e720: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-0000e730: 2320 6c6f 6767 6572 2e69 6e66 6f28 0a20  # logger.info(. 
-0000e740: 2020 2023 2020 2020 2022 5b2b 5d20 4e6f     #     "[+] No
-0000e750: 6465 206d 656d 6f72 7920 6475 6d70 2028  de memory dump (
-0000e760: 7261 7720 6475 6d70 2077 6974 6820 6c69  raw dump with li
-0000e770: 6276 6972 7429 206f 6274 6169 6e65 642c  bvirt) obtained,
-0000e780: 2061 6e64 2070 6c61 6365 6420 696e 2066   and placed in f
-0000e790: 696c 6520 7b7d 2028 7b7d 2920 6f6e 2074  ile {} ({}) on t
-0000e7a0: 6865 2073 6572 7665 722e 222e 666f 726d  he server.".form
-0000e7b0: 6174 280a 2020 2020 2320 2020 2020 2020  at(.    #       
-0000e7c0: 2020 7265 7375 6c74 5f6a 736f 6e5b 6669    result_json[fi
-0000e7d0: 6c65 5f70 6174 685f 6b65 795d 2c0a 2020  le_path_key],.  
-0000e7e0: 2020 2320 2020 2020 2020 2020 6e61 7475    #         natu
-0000e7f0: 7261 6c73 697a 6528 7265 7375 6c74 5f6a  ralsize(result_j
-0000e800: 736f 6e5b 6669 6c65 5f73 697a 655f 6b65  son[file_size_ke
-0000e810: 795d 2c20 6269 6e61 7279 3d54 7275 6529  y], binary=True)
-0000e820: 2c0a 2020 2020 2320 2020 2020 290a 2020  ,.    #     ).  
-0000e830: 2020 2320 290a 0a20 2020 2023 2072 6574    # )..    # ret
-0000e840: 7572 6e20 7265 7375 6c74 5f6a 736f 6e5b  urn result_json[
-0000e850: 6669 6c65 5f70 6174 685f 6b65 795d 2c20  file_path_key], 
-0000e860: 7265 7375 6c74 5f6a 736f 6e5b 6669 6c65  result_json[file
-0000e870: 5f73 697a 655f 6b65 795d 0a0a 0a64 6566  _size_key]...def
-0000e880: 2066 6574 6368 5f6e 6f64 655f 6e65 7477   fetch_node_netw
-0000e890: 6f72 6b5f 696e 7465 7266 6163 6573 2869  ork_interfaces(i
-0000e8a0: 645f 6e6f 6465 3a20 696e 7429 202d 3e20  d_node: int) -> 
-0000e8b0: 416e 793a 0a20 2020 2022 2222 5265 7475  Any:.    """Retu
-0000e8c0: 726e 206e 6574 776f 726b 2069 6e74 6572  rn network inter
-0000e8d0: 6661 6365 7320 6c69 7374 2067 6976 656e  faces list given
-0000e8e0: 2061 206e 6f64 6520 4944 2e22 2222 0a20   a node ID.""". 
-0000e8f0: 2020 2072 6573 756c 7420 3d20 5f67 6574     result = _get
-0000e900: 2866 222f 6e6f 6465 2f7b 6964 5f6e 6f64  (f"/node/{id_nod
-0000e910: 657d 2f6e 6574 776f 726b 5f69 6e74 6572  e}/network_inter
-0000e920: 6661 6365 2229 0a0a 2020 2020 6966 2072  face")..    if r
-0000e930: 6573 756c 742e 7374 6174 7573 5f63 6f64  esult.status_cod
-0000e940: 6520 213d 2032 3030 3a0a 2020 2020 2020  e != 200:.      
-0000e950: 2020 5f68 616e 646c 655f 6572 726f 7228    _handle_error(
-0000e960: 7265 7375 6c74 2c20 2243 616e 6e6f 7420  result, "Cannot 
-0000e970: 7265 7472 6965 7665 206e 6f64 6520 6e65  retrieve node ne
-0000e980: 7477 6f72 6b20 696e 7465 7266 6163 6573  twork interfaces
-0000e990: 2229 0a0a 2020 2020 7265 7475 726e 2072  ")..    return r
-0000e9a0: 6573 756c 742e 6a73 6f6e 2829 0a0a 0a64  esult.json()...d
-0000e9b0: 6566 2066 6574 6368 5f73 696d 756c 6174  ef fetch_simulat
-0000e9c0: 696f 6e5f 6e65 7477 6f72 6b5f 696e 7465  ion_network_inte
-0000e9d0: 7266 6163 6573 2869 645f 7369 6d75 6c61  rfaces(id_simula
-0000e9e0: 7469 6f6e 3a20 696e 7429 202d 3e20 416e  tion: int) -> An
-0000e9f0: 793a 0a20 2020 2022 2222 5265 7475 726e  y:.    """Return
-0000ea00: 206e 6574 776f 726b 2069 6e74 6572 6661   network interfa
-0000ea10: 6365 7320 6c69 7374 2067 6976 656e 2061  ces list given a
-0000ea20: 2073 696d 756c 6174 696f 6e20 4944 2e22   simulation ID."
-0000ea30: 2222 0a20 2020 2072 6573 756c 7420 3d20  "".    result = 
-0000ea40: 5f67 6574 2866 222f 7369 6d75 6c61 7469  _get(f"/simulati
-0000ea50: 6f6e 2f7b 6964 5f73 696d 756c 6174 696f  on/{id_simulatio
-0000ea60: 6e7d 2f6e 6574 776f 726b 5f69 6e74 6572  n}/network_inter
-0000ea70: 6661 6365 2229 0a0a 2020 2020 6966 2072  face")..    if r
-0000ea80: 6573 756c 742e 7374 6174 7573 5f63 6f64  esult.status_cod
-0000ea90: 6520 213d 2032 3030 3a0a 2020 2020 2020  e != 200:.      
-0000eaa0: 2020 5f68 616e 646c 655f 6572 726f 7228    _handle_error(
-0000eab0: 7265 7375 6c74 2c20 2243 616e 6e6f 7420  result, "Cannot 
-0000eac0: 7265 7472 6965 7665 2073 696d 756c 6174  retrieve simulat
-0000ead0: 696f 6e20 6e65 7477 6f72 6b20 696e 7465  ion network inte
-0000eae0: 7266 6163 6573 2229 0a0a 2020 2020 7265  rfaces")..    re
-0000eaf0: 7475 726e 2072 6573 756c 742e 6a73 6f6e  turn result.json
-0000eb00: 2829 0a0a 0a64 6566 2066 6574 6368 5f6e  ()...def fetch_n
-0000eb10: 6574 776f 726b 5f69 6e74 6572 6661 6365  etwork_interface
-0000eb20: 5f62 795f 6d61 6328 6964 5f73 696d 756c  _by_mac(id_simul
-0000eb30: 6174 696f 6e3a 2069 6e74 2c20 6d61 635f  ation: int, mac_
-0000eb40: 6164 6472 6573 733a 2073 7472 2920 2d3e  address: str) ->
-0000eb50: 2041 6e79 3a0a 2020 2020 2222 2252 6574   Any:.    """Ret
-0000eb60: 7572 6e20 6e65 7477 6f72 6b20 696e 7465  urn network inte
-0000eb70: 7266 6163 6520 6c69 7374 2067 6976 656e  rface list given
-0000eb80: 2061 206d 6163 2061 6464 7265 7373 2e22   a mac address."
-0000eb90: 2222 0a20 2020 2023 2046 6574 6368 206e  "".    # Fetch n
-0000eba0: 6f64 6520 6e65 7477 6f72 6b20 696e 7465  ode network inte
-0000ebb0: 7266 6163 6573 0a20 2020 2072 6573 756c  rfaces.    resul
-0000ebc0: 7420 3d20 5f67 6574 2866 222f 7369 6d75  t = _get(f"/simu
-0000ebd0: 6c61 7469 6f6e 2f7b 6964 5f73 696d 756c  lation/{id_simul
-0000ebe0: 6174 696f 6e7d 2f6e 6574 776f 726b 5f69  ation}/network_i
-0000ebf0: 6e74 6572 6661 6365 2229 0a0a 2020 2020  nterface")..    
-0000ec00: 6966 2072 6573 756c 742e 7374 6174 7573  if result.status
-0000ec10: 5f63 6f64 6520 213d 2032 3030 3a0a 2020  _code != 200:.  
-0000ec20: 2020 2020 2020 5f68 616e 646c 655f 6572        _handle_er
-0000ec30: 726f 7228 7265 7375 6c74 2c20 2243 616e  ror(result, "Can
-0000ec40: 6e6f 7420 7265 7472 6965 7665 206e 6574  not retrieve net
-0000ec50: 776f 726b 2069 6e74 6572 6661 6365 7322  work interfaces"
-0000ec60: 290a 0a20 2020 206e 6574 776f 726b 5f69  )..    network_i
-0000ec70: 6e74 6572 6661 6365 7320 3d20 7265 7375  nterfaces = resu
-0000ec80: 6c74 2e6a 736f 6e28 290a 0a20 2020 2066  lt.json()..    f
-0000ec90: 6f72 206e 6574 776f 726b 5f69 6e74 6572  or network_inter
-0000eca0: 6661 6365 2069 6e20 6e65 7477 6f72 6b5f  face in network_
-0000ecb0: 696e 7465 7266 6163 6573 3a0a 2020 2020  interfaces:.    
-0000ecc0: 2020 2020 6966 206e 6574 776f 726b 5f69      if network_i
-0000ecd0: 6e74 6572 6661 6365 5b22 6d61 635f 6164  nterface["mac_ad
-0000ece0: 6472 6573 7322 5d20 3d3d 206d 6163 5f61  dress"] == mac_a
-0000ecf0: 6464 7265 7373 3a0a 2020 2020 2020 2020  ddress:.        
-0000ed00: 2020 2020 7265 7475 726e 206e 6574 776f      return netwo
-0000ed10: 726b 5f69 6e74 6572 6661 6365 0a20 2020  rk_interface.   
-0000ed20: 2065 6c73 653a 0a20 2020 2020 2020 2072   else:.        r
-0000ed30: 6574 7572 6e20 4e6f 6e65 0a0a 0a64 6566  eturn None...def
-0000ed40: 2064 656c 6574 655f 6e65 7477 6f72 6b5f   delete_network_
-0000ed50: 696e 7465 7266 6163 6528 6964 5f6e 6574  interface(id_net
-0000ed60: 776f 726b 5f69 6e74 6572 6661 6365 3a20  work_interface: 
-0000ed70: 696e 7429 202d 3e20 416e 793a 0a20 2020  int) -> Any:.   
-0000ed80: 2022 2222 4465 6c65 7465 206e 6574 776f   """Delete netwo
-0000ed90: 726b 2069 6e74 6572 6661 6365 2067 6976  rk interface giv
-0000eda0: 656e 2061 6e20 6964 2e22 2222 0a20 2020  en an id.""".   
-0000edb0: 2072 6573 756c 7420 3d20 5f64 656c 6574   result = _delet
-0000edc0: 6528 6622 2f6e 6574 776f 726b 5f69 6e74  e(f"/network_int
-0000edd0: 6572 6661 6365 2f7b 6964 5f6e 6574 776f  erface/{id_netwo
-0000ede0: 726b 5f69 6e74 6572 6661 6365 7d22 290a  rk_interface}").
-0000edf0: 0a20 2020 2069 6620 7265 7375 6c74 2e73  .    if result.s
-0000ee00: 7461 7475 735f 636f 6465 2021 3d20 3230  tatus_code != 20
-0000ee10: 303a 0a20 2020 2020 2020 205f 6861 6e64  0:.        _hand
-0000ee20: 6c65 5f65 7272 6f72 280a 2020 2020 2020  le_error(.      
-0000ee30: 2020 2020 2020 7265 7375 6c74 2c20 2243        result, "C
-0000ee40: 616e 6e6f 7420 7265 7472 6965 7665 206e  annot retrieve n
-0000ee50: 6f64 6520 6e65 7477 6f72 6b20 696e 7465  ode network inte
-0000ee60: 7266 6163 6573 2066 726f 6d20 4954 2053  rfaces from IT S
-0000ee70: 696d 756c 6174 696f 6e20 4150 4922 0a20  imulation API". 
-0000ee80: 2020 2020 2020 2029 0a0a 2020 2020 7265         )..    re
-0000ee90: 7475 726e 2072 6573 756c 742e 6a73 6f6e  turn result.json
-0000eea0: 2829 0a0a 0a64 6566 2075 7064 6174 655f  ()...def update_
-0000eeb0: 6e65 7477 6f72 6b5f 696e 7465 7266 6163  network_interfac
-0000eec0: 6528 0a20 2020 2069 645f 6e65 7477 6f72  e(.    id_networ
-0000eed0: 6b5f 696e 7465 7266 6163 653a 2069 6e74  k_interface: int
-0000eee0: 2c20 6e65 7477 6f72 6b5f 696e 7465 7266  , network_interf
-0000eef0: 6163 655f 6469 6374 3a20 6469 6374 0a29  ace_dict: dict.)
-0000ef00: 202d 3e20 416e 793a 0a20 2020 2022 2222   -> Any:.    """
-0000ef10: 5570 6461 7465 206e 6574 776f 726b 2069  Update network i
-0000ef20: 6e74 6572 6661 6365 2069 6e66 6f72 6d61  nterface informa
-0000ef30: 7469 6f6e 2069 6e66 6f72 6d61 7469 6f6e  tion information
-0000ef40: 2067 6976 656e 2061 206e 6574 776f 726b   given a network
-0000ef50: 2069 6e74 6572 6661 6365 2069 6420 616e   interface id an
-0000ef60: 6420 610a 2020 2020 6469 6374 2063 6f6e  d a.    dict con
-0000ef70: 7461 696e 696e 6720 6e65 7477 6f72 6b20  taining network 
-0000ef80: 696e 666f 2e0a 0a20 2020 2022 2222 0a20  info...    """. 
-0000ef90: 2020 2064 6174 6120 3d20 6a73 6f6e 2e64     data = json.d
-0000efa0: 756d 7073 286e 6574 776f 726b 5f69 6e74  umps(network_int
-0000efb0: 6572 6661 6365 5f64 6963 7429 0a20 2020  erface_dict).   
-0000efc0: 2072 6573 756c 7420 3d20 5f70 7574 280a   result = _put(.
-0000efd0: 2020 2020 2020 2020 6622 2f6e 6574 776f          f"/netwo
-0000efe0: 726b 5f69 6e74 6572 6661 6365 2f7b 6964  rk_interface/{id
-0000eff0: 5f6e 6574 776f 726b 5f69 6e74 6572 6661  _network_interfa
-0000f000: 6365 7d22 2c0a 2020 2020 2020 2020 6461  ce}",.        da
-0000f010: 7461 3d64 6174 612c 0a20 2020 2020 2020  ta=data,.       
-0000f020: 2068 6561 6465 7273 3d7b 2243 6f6e 7465   headers={"Conte
-0000f030: 6e74 2d54 7970 6522 3a20 2261 7070 6c69  nt-Type": "appli
-0000f040: 6361 7469 6f6e 2f6a 736f 6e22 7d2c 0a20  cation/json"},. 
-0000f050: 2020 2029 0a0a 2020 2020 6966 2072 6573     )..    if res
-0000f060: 756c 742e 7374 6174 7573 5f63 6f64 6520  ult.status_code 
-0000f070: 213d 2032 3030 3a0a 2020 2020 2020 2020  != 200:.        
-0000f080: 5f68 616e 646c 655f 6572 726f 7228 7265  _handle_error(re
-0000f090: 7375 6c74 2c20 2243 616e 6e6f 7420 7570  sult, "Cannot up
-0000f0a0: 6461 7465 206e 6574 776f 726b 2069 6e74  date network int
-0000f0b0: 6572 6661 6365 2069 6e66 6f72 6d61 7469  erface informati
-0000f0c0: 6f6e 2229 0a0a 2020 2020 7265 7475 726e  on")..    return
-0000f0d0: 2072 6573 756c 742e 6a73 6f6e 2829 0a0a   result.json()..
-0000f0e0: 0a64 6566 2066 6574 6368 5f70 726f 6265  .def fetch_probe
-0000f0f0: 2870 726f 6265 5f69 643a 2069 6e74 2920  (probe_id: int) 
-0000f100: 2d3e 2041 6e79 3a0a 2020 2020 2222 2252  -> Any:.    """R
-0000f110: 6574 7572 6e20 6120 7072 6f62 6520 6769  eturn a probe gi
-0000f120: 7665 6e20 6974 7320 4944 2222 220a 0a20  ven its ID""".. 
-0000f130: 2020 2072 6573 756c 7420 3d20 5f67 6574     result = _get
-0000f140: 2866 222f 7072 6f62 652f 7b70 726f 6265  (f"/probe/{probe
-0000f150: 5f69 647d 2229 0a0a 2020 2020 6966 2072  _id}")..    if r
-0000f160: 6573 756c 742e 7374 6174 7573 5f63 6f64  esult.status_cod
-0000f170: 6520 213d 2032 3030 3a0a 2020 2020 2020  e != 200:.      
-0000f180: 2020 5f68 616e 646c 655f 6572 726f 7228    _handle_error(
-0000f190: 7265 7375 6c74 2c20 2243 616e 6e6f 7420  result, "Cannot 
-0000f1a0: 7265 7472 6965 7665 2070 726f 6265 2066  retrieve probe f
-0000f1b0: 726f 6d20 636f 7265 2041 5049 2229 0a0a  rom core API")..
-0000f1c0: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-0000f1d0: 742e 6a73 6f6e 2829 0a0a 0a64 6566 2066  t.json()...def f
-0000f1e0: 6574 6368 5f70 726f 6265 7328 6964 5f73  etch_probes(id_s
-0000f1f0: 696d 756c 6174 696f 6e3a 2069 6e74 2920  imulation: int) 
-0000f200: 2d3e 2041 6e79 3a0a 2020 2020 2222 2252  -> Any:.    """R
-0000f210: 6574 7572 6e20 7369 6d75 6c61 7469 6f6e  eturn simulation
-0000f220: 2070 726f 6265 7320 6469 6374 2067 6976   probes dict giv
-0000f230: 656e 0a20 2020 2061 2073 696d 756c 6174  en.    a simulat
-0000f240: 696f 6e20 4944 2c20 7768 6572 6520 6b65  ion ID, where ke
-0000f250: 7973 2061 7265 2070 726f 6265 7320 6964  ys are probes id
-0000f260: 732e 0a20 2020 2022 2222 0a0a 2020 2020  s..    """..    
-0000f270: 7265 7375 6c74 203d 205f 6765 7428 6622  result = _get(f"
-0000f280: 2f73 696d 756c 6174 696f 6e2f 7b69 645f  /simulation/{id_
-0000f290: 7369 6d75 6c61 7469 6f6e 7d2f 7072 6f62  simulation}/prob
-0000f2a0: 6522 290a 0a20 2020 2069 6620 7265 7375  e")..    if resu
-0000f2b0: 6c74 2e73 7461 7475 735f 636f 6465 2021  lt.status_code !
-0000f2c0: 3d20 3230 303a 0a20 2020 2020 2020 205f  = 200:.        _
-0000f2d0: 6861 6e64 6c65 5f65 7272 6f72 2872 6573  handle_error(res
-0000f2e0: 756c 742c 2022 4361 6e6e 6f74 2072 6574  ult, "Cannot ret
-0000f2f0: 7269 6576 6520 7369 6d75 6c61 7469 6f6e  rieve simulation
-0000f300: 2070 726f 6265 7320 6672 6f6d 2063 6f72   probes from cor
-0000f310: 6520 4150 4922 290a 0a20 2020 2072 6574  e API")..    ret
-0000f320: 7572 6e20 7265 7375 6c74 2e6a 736f 6e28  urn result.json(
-0000f330: 290a 0a0a 6465 6620 6372 6561 7465 5f70  )...def create_p
-0000f340: 726f 6265 280a 2020 2020 6964 5f73 696d  robe(.    id_sim
-0000f350: 756c 6174 696f 6e3a 2069 6e74 2c0a 2020  ulation: int,.  
-0000f360: 2020 6e65 7477 6f72 6b5f 696e 7465 7266    network_interf
-0000f370: 6163 6573 3a20 4c69 7374 5b69 6e74 5d2c  aces: List[int],
-0000f380: 0a20 2020 2069 6661 6365 3a20 7374 722c  .    iface: str,
-0000f390: 0a20 2020 2070 6361 703a 2062 6f6f 6c2c  .    pcap: bool,
-0000f3a0: 0a20 2020 2066 696c 7465 723a 2073 7472  .    filter: str
-0000f3b0: 2c0a 2020 2020 6469 7265 6374 696f 6e3a  ,.    direction:
-0000f3c0: 2073 7472 2c0a 2920 2d3e 2069 6e74 3a0a   str,.) -> int:.
-0000f3d0: 2020 2020 2222 2243 7265 6174 6520 6120      """Create a 
-0000f3e0: 6e65 7720 7072 6f62 6520 666f 7220 7468  new probe for th
-0000f3f0: 6520 7369 6d75 6c61 7469 6f6e 2067 6976  e simulation giv
-0000f400: 656e 2061 2064 6963 7420 636f 6e74 6169  en a dict contai
-0000f410: 6e69 6e67 2070 726f 6265 2064 6174 6122  ning probe data"
-0000f420: 2222 0a0a 2020 2020 6461 7461 5f64 6963  ""..    data_dic
-0000f430: 7420 3d20 7b0a 2020 2020 2020 2020 2269  t = {.        "i
-0000f440: 6661 6365 223a 2069 6661 6365 2c0a 2020  face": iface,.  
-0000f450: 2020 2020 2020 2270 6361 7022 3a20 7063        "pcap": pc
-0000f460: 6170 2c0a 2020 2020 2020 2020 2266 696c  ap,.        "fil
-0000f470: 7465 7222 3a20 6669 6c74 6572 2c0a 2020  ter": filter,.  
-0000f480: 2020 2020 2020 226e 6574 776f 726b 5f69        "network_i
-0000f490: 6e74 6572 6661 6365 7322 3a20 6e65 7477  nterfaces": netw
-0000f4a0: 6f72 6b5f 696e 7465 7266 6163 6573 2c0a  ork_interfaces,.
-0000f4b0: 2020 2020 2020 2020 2264 6972 6563 7469          "directi
-0000f4c0: 6f6e 223a 2064 6972 6563 7469 6f6e 2c0a  on": direction,.
-0000f4d0: 2020 2020 7d0a 0a20 2020 2064 6174 6120      }..    data 
-0000f4e0: 3d20 6a73 6f6e 2e64 756d 7073 2864 6174  = json.dumps(dat
-0000f4f0: 615f 6469 6374 290a 2020 2020 7265 7375  a_dict).    resu
-0000f500: 6c74 203d 205f 706f 7374 280a 2020 2020  lt = _post(.    
-0000f510: 2020 2020 6622 2f73 696d 756c 6174 696f      f"/simulatio
-0000f520: 6e2f 7b69 645f 7369 6d75 6c61 7469 6f6e  n/{id_simulation
-0000f530: 7d2f 7072 6f62 6522 2c0a 2020 2020 2020  }/probe",.      
-0000f540: 2020 6461 7461 3d64 6174 612c 0a20 2020    data=data,.   
-0000f550: 2020 2020 2068 6561 6465 7273 3d7b 2243       headers={"C
-0000f560: 6f6e 7465 6e74 2d54 7970 6522 3a20 2261  ontent-Type": "a
-0000f570: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e22  pplication/json"
-0000f580: 7d2c 0a20 2020 2029 0a0a 2020 2020 6966  },.    )..    if
-0000f590: 2072 6573 756c 742e 7374 6174 7573 5f63   result.status_c
-0000f5a0: 6f64 6520 213d 2032 3030 3a0a 2020 2020  ode != 200:.    
-0000f5b0: 2020 2020 5f68 616e 646c 655f 6572 726f      _handle_erro
-0000f5c0: 7228 7265 7375 6c74 2c20 2243 616e 6e6f  r(result, "Canno
-0000f5d0: 7420 6372 6561 7465 2070 726f 6265 2077  t create probe w
-0000f5e0: 6974 6820 636f 7265 2041 5049 2229 0a0a  ith core API")..
-0000f5f0: 2020 2020 7072 6f62 655f 6964 203d 2072      probe_id = r
-0000f600: 6573 756c 742e 6a73 6f6e 2829 5b22 6964  esult.json()["id
-0000f610: 225d 0a0a 2020 2020 7265 7475 726e 2070  "]..    return p
-0000f620: 726f 6265 5f69 640a 0a0a 6465 6620 7570  robe_id...def up
-0000f630: 6461 7465 5f70 726f 6265 2870 726f 6265  date_probe(probe
-0000f640: 5f69 643a 2069 6e74 2c20 7072 6f62 655f  _id: int, probe_
-0000f650: 6469 6374 3a20 6469 6374 2920 2d3e 2041  dict: dict) -> A
-0000f660: 6e79 3a0a 2020 2020 2222 2255 7064 6174  ny:.    """Updat
-0000f670: 6520 7072 6f62 6520 696e 666f 726d 6174  e probe informat
-0000f680: 696f 6e20 6769 7665 6e20 6120 7072 6f62  ion given a prob
-0000f690: 6520 6964 2061 6e64 2061 2064 6963 7420  e id and a dict 
-0000f6a0: 636f 6e74 6169 6e69 6e67 0a20 2020 2070  containing.    p
-0000f6b0: 726f 6265 2064 6174 612e 0a20 2020 2022  robe data..    "
-0000f6c0: 2222 0a0a 2020 2020 6461 7461 203d 206a  ""..    data = j
-0000f6d0: 736f 6e2e 6475 6d70 7328 7072 6f62 655f  son.dumps(probe_
-0000f6e0: 6469 6374 290a 2020 2020 7265 7375 6c74  dict).    result
-0000f6f0: 203d 205f 7075 7428 0a20 2020 2020 2020   = _put(.       
-0000f700: 2066 222f 7072 6f62 652f 7b70 726f 6265   f"/probe/{probe
-0000f710: 5f69 647d 222c 0a20 2020 2020 2020 2064  _id}",.        d
-0000f720: 6174 613d 6461 7461 2c0a 2020 2020 2020  ata=data,.      
-0000f730: 2020 6865 6164 6572 733d 7b22 436f 6e74    headers={"Cont
-0000f740: 656e 742d 5479 7065 223a 2022 6170 706c  ent-Type": "appl
-0000f750: 6963 6174 696f 6e2f 6a73 6f6e 227d 2c0a  ication/json"},.
-0000f760: 2020 2020 290a 0a20 2020 2069 6620 7265      )..    if re
-0000f770: 7375 6c74 2e73 7461 7475 735f 636f 6465  sult.status_code
-0000f780: 2021 3d20 3230 303a 0a20 2020 2020 2020   != 200:.       
-0000f790: 205f 6861 6e64 6c65 5f65 7272 6f72 2872   _handle_error(r
-0000f7a0: 6573 756c 742c 2022 4361 6e6e 6f74 2075  esult, "Cannot u
-0000f7b0: 7064 6174 6520 7072 6f62 6520 696e 666f  pdate probe info
-0000f7c0: 726d 6174 696f 6e20 7769 7468 2063 6f72  rmation with cor
-0000f7d0: 6520 4150 4922 290a 0a20 2020 2072 6574  e API")..    ret
-0000f7e0: 7572 6e20 7265 7375 6c74 2e6a 736f 6e28  urn result.json(
-0000f7f0: 290a 0a0a 6465 6620 6465 6c65 7465 5f70  )...def delete_p
-0000f800: 726f 6265 2870 726f 6265 5f69 643a 2069  robe(probe_id: i
-0000f810: 6e74 2920 2d3e 2041 6e79 3a0a 2020 2020  nt) -> Any:.    
-0000f820: 2222 2244 656c 6574 6520 7369 6d75 6c61  """Delete simula
-0000f830: 7469 6f6e 2070 726f 6265 2067 6976 656e  tion probe given
-0000f840: 2069 7473 2049 442e 2222 220a 0a20 2020   its ID."""..   
-0000f850: 2023 2044 656c 6574 6520 7072 6f62 650a   # Delete probe.
-0000f860: 2020 2020 7265 7375 6c74 203d 205f 6465      result = _de
-0000f870: 6c65 7465 2866 222f 7072 6f62 652f 7b70  lete(f"/probe/{p
-0000f880: 726f 6265 5f69 647d 2229 0a0a 2020 2020  robe_id}")..    
-0000f890: 6966 2072 6573 756c 742e 7374 6174 7573  if result.status
-0000f8a0: 5f63 6f64 6520 213d 2032 3030 3a0a 2020  _code != 200:.  
-0000f8b0: 2020 2020 2020 5f68 616e 646c 655f 6572        _handle_er
-0000f8c0: 726f 7228 7265 7375 6c74 2c20 2243 616e  ror(result, "Can
-0000f8d0: 6e6f 7420 6465 6c65 7465 2070 726f 6265  not delete probe
-0000f8e0: 2229 0a0a 2020 2020 7265 7475 726e 2072  ")..    return r
-0000f8f0: 6573 756c 742e 6a73 6f6e 2829 0a0a 0a64  esult.json()...d
-0000f900: 6566 2066 6574 6368 5f62 6173 6562 6f78  ef fetch_basebox
-0000f910: 6573 2829 202d 3e20 416e 793a 0a20 2020  es() -> Any:.   
-0000f920: 2022 2222 5265 7475 726e 2062 6173 6562   """Return baseb
-0000f930: 6f78 6573 206c 6973 742e 2222 220a 2020  oxes list.""".  
-0000f940: 2020 7265 7375 6c74 203d 205f 6765 7428    result = _get(
-0000f950: 222f 6261 7365 626f 7822 290a 0a20 2020  "/basebox")..   
-0000f960: 2069 6620 7265 7375 6c74 2e73 7461 7475   if result.statu
-0000f970: 735f 636f 6465 2021 3d20 3230 303a 0a20  s_code != 200:. 
-0000f980: 2020 2020 2020 205f 6861 6e64 6c65 5f65         _handle_e
-0000f990: 7272 6f72 2872 6573 756c 742c 2022 4361  rror(result, "Ca
-0000f9a0: 6e6e 6f74 2072 6574 7269 6576 6520 6261  nnot retrieve ba
-0000f9b0: 7365 626f 7865 7320 6c69 7374 2066 726f  seboxes list fro
-0000f9c0: 6d20 4954 2053 696d 756c 6174 696f 6e20  m IT Simulation 
-0000f9d0: 4150 4922 290a 0a20 2020 2062 6173 6562  API")..    baseb
-0000f9e0: 6f78 6573 203d 2072 6573 756c 742e 6a73  oxes = result.js
-0000f9f0: 6f6e 2829 0a20 2020 2072 6574 7572 6e20  on().    return 
-0000fa00: 6261 7365 626f 7865 730a 0a0a 6465 6620  baseboxes...def 
-0000fa10: 6665 7463 685f 6261 7365 626f 7828 6964  fetch_basebox(id
-0000fa20: 5f62 6173 6562 6f78 3a20 7374 7229 202d  _basebox: str) -
-0000fa30: 3e20 416e 793a 0a20 2020 2022 2222 5265  > Any:.    """Re
-0000fa40: 7475 726e 2062 6173 6562 6f78 2067 6976  turn basebox giv
-0000fa50: 656e 2061 2062 6173 6562 6f78 2069 642e  en a basebox id.
-0000fa60: 2222 220a 2020 2020 7265 7375 6c74 203d  """.    result =
-0000fa70: 205f 6765 7428 6622 2f62 6173 6562 6f78   _get(f"/basebox
-0000fa80: 2f69 642f 7b69 645f 6261 7365 626f 787d  /id/{id_basebox}
-0000fa90: 2229 0a0a 2020 2020 6966 2072 6573 756c  ")..    if resul
-0000faa0: 742e 7374 6174 7573 5f63 6f64 6520 213d  t.status_code !=
-0000fab0: 2032 3030 3a0a 2020 2020 2020 2020 5f68   200:.        _h
-0000fac0: 616e 646c 655f 6572 726f 7228 7265 7375  andle_error(resu
-0000fad0: 6c74 2c20 2243 616e 6e6f 7420 7265 7472  lt, "Cannot retr
-0000fae0: 6965 7665 2062 6173 6562 6f78 2069 6e66  ieve basebox inf
-0000faf0: 6f20 6672 6f6d 2049 5420 5369 6d75 6c61  o from IT Simula
-0000fb00: 7469 6f6e 2041 5049 2229 0a0a 2020 2020  tion API")..    
-0000fb10: 6261 7365 626f 7820 3d20 7265 7375 6c74  basebox = result
-0000fb20: 2e6a 736f 6e28 290a 2020 2020 7265 7475  .json().    retu
-0000fb30: 726e 2062 6173 6562 6f78 0a0a 0a64 6566  rn basebox...def
-0000fb40: 2072 656c 6f61 645f 6261 7365 626f 7865   reload_baseboxe
-0000fb50: 7328 2920 2d3e 2041 6e79 3a0a 2020 2020  s() -> Any:.    
-0000fb60: 2222 220a 2020 2020 4361 6c6c 2074 6865  """.    Call the
-0000fb70: 2063 7962 6572 2072 616e 6765 2041 5049   cyber range API
-0000fb80: 2074 6f20 7265 6c6f 6164 2074 6865 206c   to reload the l
-0000fb90: 6973 7420 6f66 2061 7661 696c 6162 6c65  ist of available
-0000fba0: 2062 6173 6562 6f78 6573 2e0a 0a20 2020   baseboxes...   
-0000fbb0: 203a 7265 7475 726e 3a0a 2020 2020 2222   :return:.    ""
-0000fbc0: 220a 2020 2020 7265 7375 6c74 203d 205f  ".    result = _
-0000fbd0: 6765 7428 222f 6261 7365 626f 782f 7265  get("/basebox/re
-0000fbe0: 6c6f 6164 2229 0a0a 2020 2020 6966 2072  load")..    if r
-0000fbf0: 6573 756c 742e 7374 6174 7573 5f63 6f64  esult.status_cod
-0000fc00: 6520 213d 2032 3030 3a0a 2020 2020 2020  e != 200:.      
-0000fc10: 2020 5f68 616e 646c 655f 6572 726f 7228    _handle_error(
-0000fc20: 7265 7375 6c74 2c20 2243 616e 6e6f 7420  result, "Cannot 
-0000fc30: 7265 7472 6965 7665 2062 6173 6562 6f78  retrieve basebox
-0000fc40: 2069 6e66 6f20 6672 6f6d 2049 5420 5369   info from IT Si
-0000fc50: 6d75 6c61 7469 6f6e 2041 5049 2229 0a0a  mulation API")..
-0000fc60: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-0000fc70: 742e 6a73 6f6e 2829 0a0a 0a64 6566 2076  t.json()...def v
-0000fc80: 6572 6966 795f 6261 7365 626f 785f 7265  erify_basebox_re
-0000fc90: 7375 6c74 2874 6173 6b5f 6964 3a20 7374  sult(task_id: st
-0000fca0: 7229 202d 3e20 416e 793a 0a20 2020 2022  r) -> Any:.    "
-0000fcb0: 2222 0a20 2020 2020 4361 6c6c 2074 6865  "".     Call the
-0000fcc0: 2041 5049 2074 6f20 6765 7420 7468 6520   API to get the 
-0000fcd0: 7265 7375 6c74 2074 6865 2063 7572 7265  result the curre
-0000fce0: 6e74 2076 6572 6966 6963 6174 696f 6e2e  nt verification.
-0000fcf0: 0a0a 2020 2020 3a70 6172 616d 2074 6173  ..    :param tas
-0000fd00: 6b5f 6964 3a20 7468 6520 7461 736b 2069  k_id: the task i
-0000fd10: 640a 2020 2020 3a72 6574 7572 6e3a 2074  d.    :return: t
-0000fd20: 6865 2072 6573 756c 7420 6f66 2074 6865  he result of the
-0000fd30: 2076 6572 6966 6963 6174 696f 6e0a 0a20   verification.. 
-0000fd40: 2020 2022 2222 0a0a 2020 2020 6461 7461     """..    data
-0000fd50: 203d 207b 2274 6173 6b5f 6964 223a 2074   = {"task_id": t
-0000fd60: 6173 6b5f 6964 7d0a 0a20 2020 2074 7279  ask_id}..    try
-0000fd70: 3a0a 2020 2020 2020 2020 7265 7375 6c74  :.        result
-0000fd80: 203d 205f 706f 7374 280a 2020 2020 2020   = _post(.      
-0000fd90: 2020 2020 2020 222f 6261 7365 626f 782f        "/basebox/
-0000fda0: 7265 7375 6c74 5f76 6572 6966 7922 2c0a  result_verify",.
-0000fdb0: 2020 2020 2020 2020 2020 2020 6461 7461              data
-0000fdc0: 3d64 6174 612c 0a20 2020 2020 2020 2029  =data,.        )
-0000fdd0: 0a0a 2020 2020 2020 2020 6966 2072 6573  ..        if res
-0000fde0: 756c 742e 7374 6174 7573 5f63 6f64 6520  ult.status_code 
-0000fdf0: 213d 2032 3030 3a0a 2020 2020 2020 2020  != 200:.        
-0000fe00: 2020 2020 5f68 616e 646c 655f 6572 726f      _handle_erro
-0000fe10: 7228 7265 7375 6c74 2c20 2243 616e 6e6f  r(result, "Canno
-0000fe20: 7420 6765 7420 7665 7269 6669 6361 7469  t get verificati
-0000fe30: 6f6e 2072 6573 756c 7422 290a 0a20 2020  on result")..   
-0000fe40: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-0000fe50: 6c74 2e6a 736f 6e28 290a 0a20 2020 2065  lt.json()..    e
-0000fe60: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
-0000fe70: 6173 2065 3a0a 2020 2020 2020 2020 7261  as e:.        ra
-0000fe80: 6973 6520 4578 6365 7074 696f 6e28 2249  ise Exception("I
-0000fe90: 7373 7565 2077 6865 6e20 6765 7474 696e  ssue when gettin
-0000fea0: 6720 7665 7269 6669 6361 7469 6f6e 2072  g verification r
-0000feb0: 6573 756c 743a 2027 7b7d 2722 2e66 6f72  esult: '{}'".for
-0000fec0: 6d61 7428 6529 290a 0a0a 6465 6620 7665  mat(e))...def ve
-0000fed0: 7269 6679 5f62 6173 6562 6f78 5f73 746f  rify_basebox_sto
-0000fee0: 7028 7461 736b 5f69 643a 2073 7472 2920  p(task_id: str) 
-0000fef0: 2d3e 2041 6e79 3a0a 2020 2020 2222 220a  -> Any:.    """.
-0000ff00: 2020 2020 4361 6c6c 2074 6865 2041 5049      Call the API
-0000ff10: 2074 6f20 7374 6f70 2074 6865 2063 7572   to stop the cur
-0000ff20: 7265 6e74 2076 6572 6966 6963 6174 696f  rent verificatio
-0000ff30: 6e0a 2020 2020 3a72 6574 7572 6e3a 0a20  n.    :return:. 
-0000ff40: 2020 2022 2222 0a20 2020 2064 6174 6120     """.    data 
-0000ff50: 3d20 7b22 7461 736b 5f69 6422 3a20 7461  = {"task_id": ta
-0000ff60: 736b 5f69 647d 0a0a 2020 2020 7265 7375  sk_id}..    resu
-0000ff70: 6c74 203d 205f 706f 7374 2822 2f62 6173  lt = _post("/bas
-0000ff80: 6562 6f78 2f73 746f 705f 7665 7269 6679  ebox/stop_verify
-0000ff90: 222c 2064 6174 613d 6461 7461 290a 0a20  ", data=data).. 
-0000ffa0: 2020 2069 6620 7265 7375 6c74 2e73 7461     if result.sta
-0000ffb0: 7475 735f 636f 6465 2021 3d20 3230 303a  tus_code != 200:
-0000ffc0: 0a20 2020 2020 2020 205f 6861 6e64 6c65  .        _handle
-0000ffd0: 5f65 7272 6f72 2872 6573 756c 742c 2022  _error(result, "
-0000ffe0: 4361 6e6e 6f74 2073 746f 7020 7665 7269  Cannot stop veri
-0000fff0: 6669 6361 7469 6f6e 2074 6173 6b22 290a  fication task").
-00010000: 0a20 2020 2072 6574 7572 6e20 7265 7375  .    return resu
-00010010: 6c74 2e6a 736f 6e28 290a 0a0a 6465 6620  lt.json()...def 
-00010020: 7665 7269 6679 5f62 6173 6562 6f78 5f73  verify_basebox_s
-00010030: 7461 7475 7328 7461 736b 5f69 643a 2073  tatus(task_id: s
-00010040: 7472 2920 2d3e 2041 6e79 3a0a 2020 2020  tr) -> Any:.    
-00010050: 2222 220a 2020 2020 4361 6c6c 2074 6865  """.    Call the
-00010060: 2041 5049 2074 6f20 6765 7420 7468 6520   API to get the 
-00010070: 7374 6174 7573 206f 6620 6375 7272 656e  status of curren
-00010080: 7420 7665 7269 6669 6361 7469 6f6e 0a20  t verification. 
-00010090: 2020 203a 7265 7475 726e 3a0a 2020 2020     :return:.    
-000100a0: 2222 220a 2020 2020 6461 7461 203d 207b  """.    data = {
-000100b0: 2274 6173 6b5f 6964 223a 2074 6173 6b5f  "task_id": task_
-000100c0: 6964 7d0a 0a20 2020 2074 7279 3a0a 2020  id}..    try:.  
-000100d0: 2020 2020 2020 7265 7375 6c74 203d 205f        result = _
-000100e0: 706f 7374 2822 2f62 6173 6562 6f78 2f73  post("/basebox/s
-000100f0: 7461 7475 735f 7665 7269 6679 222c 2064  tatus_verify", d
-00010100: 6174 613d 6461 7461 290a 0a20 2020 2020  ata=data)..     
-00010110: 2020 2069 6620 7265 7375 6c74 2e73 7461     if result.sta
-00010120: 7475 735f 636f 6465 2021 3d20 3230 303a  tus_code != 200:
-00010130: 0a20 2020 2020 2020 2020 2020 205f 6861  .            _ha
-00010140: 6e64 6c65 5f65 7272 6f72 2872 6573 756c  ndle_error(resul
-00010150: 742c 2022 4361 6e6e 6f74 2067 6574 2076  t, "Cannot get v
-00010160: 6572 6966 7920 7374 6174 7573 2229 0a0a  erify status")..
-00010170: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-00010180: 6573 756c 742e 6a73 6f6e 2829 0a0a 2020  esult.json()..  
-00010190: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
-000101a0: 6f6e 2061 7320 653a 0a20 2020 2020 2020  on as e:.       
-000101b0: 2072 6169 7365 2045 7863 6570 7469 6f6e   raise Exception
-000101c0: 2822 4973 7375 6520 7768 656e 2067 6574  ("Issue when get
-000101d0: 7469 6e67 2076 6572 6966 7920 7374 6174  ting verify stat
-000101e0: 7573 3a20 277b 7d27 222e 666f 726d 6174  us: '{}'".format
-000101f0: 2865 2929 0a0a 0a64 6566 2076 6572 6966  (e))...def verif
-00010200: 795f 6261 7365 626f 7828 6964 5f62 6173  y_basebox(id_bas
-00010210: 6562 6f78 3a20 696e 7429 202d 3e20 416e  ebox: int) -> An
-00010220: 793a 0a20 2020 2022 2222 0a20 2020 2043  y:.    """.    C
-00010230: 616c 6c20 7468 6520 4150 4920 746f 2076  all the API to v
-00010240: 6572 6966 7920 7468 6520 6368 6563 6b73  erify the checks
-00010250: 756d 206f 6620 7468 6520 6769 7665 6e20  um of the given 
-00010260: 6261 7365 626f 780a 2020 2020 3a70 6172  basebox.    :par
-00010270: 616d 2069 645f 6261 7365 626f 783a 2074  am id_basebox: t
-00010280: 6865 2069 6420 6f66 2074 6865 2062 6173  he id of the bas
-00010290: 6562 6f78 2074 6f20 7665 7269 6679 0a20  ebox to verify. 
-000102a0: 2020 203a 7265 7475 726e 3a0a 2020 2020     :return:.    
-000102b0: 2222 220a 2020 2020 7265 7375 6c74 203d  """.    result =
-000102c0: 205f 6765 7428 6622 2f62 6173 6562 6f78   _get(f"/basebox
-000102d0: 2f76 6572 6966 792f 7b69 645f 6261 7365  /verify/{id_base
-000102e0: 626f 787d 2229 0a0a 2020 2020 6966 2072  box}")..    if r
-000102f0: 6573 756c 742e 7374 6174 7573 5f63 6f64  esult.status_cod
-00010300: 6520 213d 2032 3030 3a0a 2020 2020 2020  e != 200:.      
-00010310: 2020 5f68 616e 646c 655f 6572 726f 7228    _handle_error(
-00010320: 7265 7375 6c74 2c20 2243 616e 6e6f 7420  result, "Cannot 
-00010330: 7265 7472 6965 7665 2062 6173 6562 6f78  retrieve basebox
-00010340: 2069 6e66 6f20 6672 6f6d 2049 5420 5369   info from IT Si
-00010350: 6d75 6c61 7469 6f6e 2041 5049 2229 0a0a  mulation API")..
-00010360: 2020 2020 7265 7375 6c74 203d 2072 6573      result = res
-00010370: 756c 742e 6a73 6f6e 2829 0a20 2020 2074  ult.json().    t
-00010380: 6173 6b5f 6964 203d 2072 6573 756c 745b  ask_id = result[
-00010390: 2274 6173 6b5f 6964 225d 0a20 2020 2073  "task_id"].    s
-000103a0: 7563 6365 7373 203d 2072 6573 756c 745b  uccess = result[
-000103b0: 2272 6573 756c 7422 5d20 3d3d 2022 5354  "result"] == "ST
-000103c0: 4152 5445 4422 0a0a 2020 2020 6966 206e  ARTED"..    if n
-000103d0: 6f74 2073 7563 6365 7373 3a0a 2020 2020  ot success:.    
-000103e0: 2020 2020 5f72 6169 7365 5f65 7272 6f72      _raise_error
-000103f0: 5f6d 7367 2872 6573 756c 7429 0a0a 2020  _msg(result)..  
-00010400: 2020 6c6f 6767 6572 2e69 6e66 6f28 6622    logger.info(f"
-00010410: 5b2b 5d20 5665 7269 6669 6361 7469 6f6e  [+] Verification
-00010420: 2074 6173 6b20 4944 3a20 7b74 6173 6b5f   task ID: {task_
-00010430: 6964 7d22 290a 0a20 2020 2072 6573 756c  id}")..    resul
-00010440: 7420 3d20 5f5f 6861 6e64 6c65 5f77 6169  t = __handle_wai
-00010450: 7428 0a20 2020 2020 2020 2077 6169 743d  t(.        wait=
-00010460: 5472 7565 2c20 7461 736b 5f69 643d 7461  True, task_id=ta
-00010470: 736b 5f69 642c 206c 6f67 5f73 7566 6669  sk_id, log_suffi
-00010480: 783d 6964 5f62 6173 6562 6f78 2c20 7469  x=id_basebox, ti
-00010490: 6d65 6f75 743d 3336 3030 0a20 2020 2029  meout=3600.    )
-000104a0: 0a0a 2020 2020 7265 7475 726e 207b 0a20  ..    return {. 
-000104b0: 2020 2020 2020 2022 7375 6363 6573 7322         "success"
-000104c0: 3a20 7265 7375 6c74 5b22 7265 7375 6c74  : result["result
-000104d0: 225d 5b22 7375 6363 6573 7322 5d2c 0a20  "]["success"],. 
-000104e0: 2020 2020 2020 2022 7461 736b 5f69 6422         "task_id"
-000104f0: 3a20 7461 736b 5f69 642c 0a20 2020 2020  : task_id,.     
-00010500: 2020 2022 7661 6c69 645f 6368 6563 6b73     "valid_checks
-00010510: 756d 223a 2072 6573 756c 745b 2272 6573  um": result["res
-00010520: 756c 7422 5d5b 2276 616c 6964 5f63 6865  ult"]["valid_che
-00010530: 636b 7375 6d22 5d2c 0a20 2020 207d 0a0a  cksum"],.    }..
-00010540: 0a64 6566 2076 6572 6966 795f 6261 7365  .def verify_base
-00010550: 626f 7865 7328 2920 2d3e 2041 6e79 3a0a  boxes() -> Any:.
-00010560: 2020 2020 2222 220a 2020 2020 4361 6c6c      """.    Call
-00010570: 2074 6865 2041 5049 2074 6f20 7665 7269   the API to veri
-00010580: 6679 2074 6865 2063 6865 636b 7375 6d20  fy the checksum 
-00010590: 6f66 2061 6c6c 2062 6173 6562 6f78 6573  of all baseboxes
-000105a0: 0a20 2020 203a 7265 7475 726e 3a0a 2020  .    :return:.  
-000105b0: 2020 2222 220a 2020 2020 7265 7375 6c74    """.    result
-000105c0: 203d 205f 6765 7428 222f 6261 7365 626f   = _get("/basebo
-000105d0: 782f 7665 7269 6679 2f22 290a 0a20 2020  x/verify/")..   
-000105e0: 2069 6620 7265 7375 6c74 2e73 7461 7475   if result.statu
-000105f0: 735f 636f 6465 2021 3d20 3230 303a 0a20  s_code != 200:. 
-00010600: 2020 2020 2020 205f 6861 6e64 6c65 5f65         _handle_e
-00010610: 7272 6f72 2872 6573 756c 742c 2022 4361  rror(result, "Ca
-00010620: 6e6e 6f74 2072 6574 7269 6576 6520 6261  nnot retrieve ba
-00010630: 7365 626f 7820 696e 666f 2066 726f 6d20  sebox info from 
-00010640: 4954 2053 696d 756c 6174 696f 6e20 4150  IT Simulation AP
-00010650: 4922 290a 0a20 2020 2072 6573 756c 7420  I")..    result 
-00010660: 3d20 7265 7375 6c74 2e6a 736f 6e28 290a  = result.json().
-00010670: 2020 2020 7461 736b 5f69 6420 3d20 7265      task_id = re
-00010680: 7375 6c74 5b22 7461 736b 5f69 6422 5d0a  sult["task_id"].
-00010690: 2020 2020 7375 6363 6573 7320 3d20 7265      success = re
-000106a0: 7375 6c74 5b22 7265 7375 6c74 225d 203d  sult["result"] =
-000106b0: 3d20 2253 5441 5254 4544 220a 0a20 2020  = "STARTED"..   
-000106c0: 2069 6620 6e6f 7420 7375 6363 6573 733a   if not success:
-000106d0: 0a20 2020 2020 2020 205f 7261 6973 655f  .        _raise_
-000106e0: 6572 726f 725f 6d73 6728 7265 7375 6c74  error_msg(result
-000106f0: 290a 0a20 2020 206c 6f67 6765 722e 696e  )..    logger.in
-00010700: 666f 2866 225b 2b5d 2056 6572 6966 6963  fo(f"[+] Verific
-00010710: 6174 696f 6e20 7461 736b 2049 443a 207b  ation task ID: {
-00010720: 7461 736b 5f69 647d 2229 0a0a 2020 2020  task_id}")..    
-00010730: 7265 7375 6c74 203d 205f 5f68 616e 646c  result = __handl
-00010740: 655f 7761 6974 280a 2020 2020 2020 2020  e_wait(.        
-00010750: 7761 6974 3d54 7275 652c 2074 6173 6b5f  wait=True, task_
-00010760: 6964 3d74 6173 6b5f 6964 2c20 6c6f 675f  id=task_id, log_
-00010770: 7375 6666 6978 3d22 616c 6c20 6261 7365  suffix="all base
-00010780: 626f 7865 7322 2c20 7469 6d65 6f75 743d  boxes", timeout=
-00010790: 3336 3030 0a20 2020 2029 0a0a 2020 2020  3600.    )..    
-000107a0: 7265 7475 726e 207b 0a20 2020 2020 2020  return {.       
-000107b0: 2022 7375 6363 6573 7322 3a20 7265 7375   "success": resu
-000107c0: 6c74 5b22 7265 7375 6c74 225d 5b22 7375  lt["result"]["su
-000107d0: 6363 6573 7322 5d2c 0a20 2020 2020 2020  ccess"],.       
-000107e0: 2022 7461 736b 5f69 6422 3a20 7461 736b   "task_id": task
-000107f0: 5f69 642c 0a20 2020 2020 2020 2022 7265  _id,.        "re
-00010800: 7375 6c74 223a 2072 6573 756c 745b 2272  sult": result["r
-00010810: 6573 756c 7422 5d5b 2276 616c 6964 5f63  esult"]["valid_c
-00010820: 6865 636b 7375 6d22 5d2c 0a20 2020 207d  hecksum"],.    }
-00010830: 0a0a 0a64 6566 2066 6574 6368 5f64 6f6d  ...def fetch_dom
-00010840: 6169 6e73 2829 202d 3e20 4469 6374 5b73  ains() -> Dict[s
-00010850: 7472 2c20 7374 725d 3a0a 2020 2020 2222  tr, str]:.    ""
-00010860: 2252 6574 7572 6e73 2074 6865 206d 6170  "Returns the map
-00010870: 7069 6e67 2064 6f6d 6169 6e2d 3e49 5022  ping domain->IP"
-00010880: 2222 0a0a 2020 2020 2320 4649 584d 4528  ""..    # FIXME(
-00010890: 6d75 6c74 692d 7465 6e61 6e74 293a 2077  multi-tenant): w
-000108a0: 6520 7368 6f75 6c64 2072 6574 7269 6576  e should retriev
-000108b0: 6520 646f 6d61 696e 7320 6163 636f 7264  e domains accord
-000108c0: 696e 6720 746f 2061 2073 696d 756c 6174  ing to a simulat
-000108d0: 696f 6e20 6964 0a20 2020 2072 6573 756c  ion id.    resul
-000108e0: 7420 3d20 5f67 6574 2822 2f6e 6574 776f  t = _get("/netwo
-000108f0: 726b 5f69 6e74 6572 6661 6365 2f64 6f6d  rk_interface/dom
-00010900: 6169 6e73 2229 0a0a 2020 2020 6966 2072  ains")..    if r
-00010910: 6573 756c 742e 7374 6174 7573 5f63 6f64  esult.status_cod
-00010920: 6520 213d 2032 3030 3a0a 2020 2020 2020  e != 200:.      
-00010930: 2020 5f68 616e 646c 655f 6572 726f 7228    _handle_error(
-00010940: 7265 7375 6c74 2c20 2245 7272 6f72 2077  result, "Error w
-00010950: 6869 6c65 2066 6574 6368 696e 6720 646f  hile fetching do
-00010960: 6d61 696e 7322 290a 0a20 2020 2072 6574  mains")..    ret
-00010970: 7572 6e20 7265 7375 6c74 2e6a 736f 6e28  urn result.json(
-00010980: 290a 0a0a 6465 6620 6665 7463 685f 7765  )...def fetch_we
-00010990: 6273 6974 6573 2829 202d 3e20 416e 793a  bsites() -> Any:
-000109a0: 0a20 2020 2022 2222 5265 7475 726e 2077  .    """Return w
-000109b0: 6562 7369 7465 7320 6c69 7374 2e22 2222  ebsites list."""
-000109c0: 0a20 2020 2072 6573 756c 7420 3d20 5f67  .    result = _g
-000109d0: 6574 2822 2f77 6562 7369 7465 2229 0a0a  et("/website")..
-000109e0: 2020 2020 6966 2072 6573 756c 742e 7374      if result.st
-000109f0: 6174 7573 5f63 6f64 6520 213d 2032 3030  atus_code != 200
-00010a00: 3a0a 2020 2020 2020 2020 5f68 616e 646c  :.        _handl
-00010a10: 655f 6572 726f 7228 7265 7375 6c74 2c20  e_error(result, 
-00010a20: 2243 616e 6e6f 7420 7265 7472 6965 7665  "Cannot retrieve
-00010a30: 2077 6562 7369 7465 7320 6c69 7374 2066   websites list f
-00010a40: 726f 6d20 4954 2053 696d 756c 6174 696f  rom IT Simulatio
-00010a50: 6e20 4150 4922 290a 0a20 2020 2077 6562  n API")..    web
-00010a60: 7369 7465 7320 3d20 7265 7375 6c74 2e6a  sites = result.j
-00010a70: 736f 6e28 290a 2020 2020 7265 7475 726e  son().    return
-00010a80: 2077 6562 7369 7465 730a 0a0a 6465 6620   websites...def 
-00010a90: 746f 706f 6c6f 6779 5f61 6464 5f77 6562  topology_add_web
-00010aa0: 7369 7465 7328 0a20 2020 2074 6f70 6f6c  sites(.    topol
-00010ab0: 6f67 795f 7961 6d6c 3a20 7374 722c 2077  ogy_yaml: str, w
-00010ac0: 6562 7369 7465 733a 204c 6973 745b 7374  ebsites: List[st
-00010ad0: 725d 2c20 7377 6974 6368 5f6e 616d 653a  r], switch_name:
-00010ae0: 2073 7472 0a29 202d 3e20 7374 723a 0a20   str.) -> str:. 
-00010af0: 2020 2022 2222 4164 6420 646f 636b 6572     """Add docker
-00010b00: 2077 6562 7369 7465 7320 6e6f 6465 2074   websites node t
-00010b10: 6f20 6120 6769 7665 6e20 746f 706f 6c6f  o a given topolo
-00010b20: 6779 2c20 616e 6420 7265 7475 726e 2074  gy, and return t
-00010b30: 6865 2075 7064 6174 6564 2074 6f70 6f6c  he updated topol
-00010b40: 6f67 792e 2222 220a 0a20 2020 2064 6174  ogy."""..    dat
-00010b50: 615f 6469 6374 203d 207b 0a20 2020 2020  a_dict = {.     
-00010b60: 2020 2022 746f 706f 6c6f 6779 5f79 616d     "topology_yam
-00010b70: 6c22 3a20 746f 706f 6c6f 6779 5f79 616d  l": topology_yam
-00010b80: 6c2c 0a20 2020 2020 2020 2022 7765 6273  l,.        "webs
-00010b90: 6974 6573 223a 2077 6562 7369 7465 732c  ites": websites,
-00010ba0: 0a20 2020 2020 2020 2022 7377 6974 6368  .        "switch
-00010bb0: 5f6e 616d 6522 3a20 7377 6974 6368 5f6e  _name": switch_n
-00010bc0: 616d 652c 0a20 2020 207d 0a20 2020 2064  ame,.    }.    d
-00010bd0: 6174 6120 3d20 6a73 6f6e 2e64 756d 7073  ata = json.dumps
-00010be0: 2864 6174 615f 6469 6374 290a 2020 2020  (data_dict).    
-00010bf0: 7265 7375 6c74 203d 205f 706f 7374 280a  result = _post(.
-00010c00: 2020 2020 2020 2020 222f 746f 706f 6c6f          "/topolo
-00010c10: 6779 2f61 6464 5f77 6562 7369 7465 7322  gy/add_websites"
-00010c20: 2c0a 2020 2020 2020 2020 6461 7461 3d64  ,.        data=d
-00010c30: 6174 612c 0a20 2020 2020 2020 2068 6561  ata,.        hea
-00010c40: 6465 7273 3d7b 2243 6f6e 7465 6e74 2d54  ders={"Content-T
-00010c50: 7970 6522 3a20 2261 7070 6c69 6361 7469  ype": "applicati
-00010c60: 6f6e 2f6a 736f 6e22 7d2c 0a20 2020 2029  on/json"},.    )
-00010c70: 0a0a 2020 2020 6966 2072 6573 756c 742e  ..    if result.
-00010c80: 7374 6174 7573 5f63 6f64 6520 213d 2032  status_code != 2
-00010c90: 3030 3a0a 2020 2020 2020 2020 5f68 616e  00:.        _han
-00010ca0: 646c 655f 6572 726f 7228 7265 7375 6c74  dle_error(result
-00010cb0: 2c20 2245 7272 6f72 2077 6869 6c65 2061  , "Error while a
-00010cc0: 6464 696e 6720 7765 6273 6974 6573 2074  dding websites t
-00010cd0: 6f20 6120 746f 706f 6c6f 6779 2229 0a0a  o a topology")..
-00010ce0: 2020 2020 746f 706f 6c6f 6779 5f79 616d      topology_yam
-00010cf0: 6c20 3d20 7265 7375 6c74 2e6a 736f 6e28  l = result.json(
-00010d00: 295b 2274 6f70 6f6c 6f67 795f 7961 6d6c  )["topology_yaml
-00010d10: 225d 0a0a 2020 2020 7265 7475 726e 2074  "]..    return t
-00010d20: 6f70 6f6c 6f67 795f 7961 6d6c 0a0a 0a64  opology_yaml...d
-00010d30: 6566 2074 6f70 6f6c 6f67 795f 6164 645f  ef topology_add_
-00010d40: 6467 6128 0a20 2020 2074 6f70 6f6c 6f67  dga(.    topolog
-00010d50: 795f 7961 6d6c 3a20 7374 722c 0a20 2020  y_yaml: str,.   
-00010d60: 2061 6c67 6f72 6974 686d 3a20 7374 722c   algorithm: str,
-00010d70: 0a20 2020 2073 7769 7463 685f 6e61 6d65  .    switch_name
-00010d80: 3a20 7374 722c 0a20 2020 206e 756d 6265  : str,.    numbe
-00010d90: 723a 2069 6e74 2c0a 2020 2020 7265 736f  r: int,.    reso
-00010da0: 7572 6365 735f 6469 723a 2073 7472 2c0a  urces_dir: str,.
-00010db0: 2920 2d3e 2054 7570 6c65 5b73 7472 2c20  ) -> Tuple[str, 
-00010dc0: 4c69 7374 5b73 7472 5d5d 3a0a 2020 2020  List[str]]:.    
-00010dd0: 2222 2241 6464 2064 6f63 6b65 7220 656d  """Add docker em
-00010de0: 7074 7920 7765 6273 6974 6573 2077 6974  pty websites wit
-00010df0: 6820 4447 4120 6e6f 6465 2074 6f20 6120  h DGA node to a 
-00010e00: 6769 7665 6e20 746f 706f 6c6f 6779 2c20  given topology, 
-00010e10: 616e 6420 7265 7475 726e 2074 6865 2075  and return the u
-00010e20: 7064 6174 6564 2074 6f70 6f6c 6f67 790a  pdated topology.
-00010e30: 2020 2020 6173 736f 6369 6174 6564 2077      associated w
-00010e40: 6974 6820 7468 6520 646f 6d61 696e 732e  ith the domains.
-00010e50: 2222 220a 0a20 2020 2064 6174 615f 6469  """..    data_di
-00010e60: 6374 203d 207b 0a20 2020 2020 2020 2022  ct = {.        "
-00010e70: 746f 706f 6c6f 6779 5f79 616d 6c22 3a20  topology_yaml": 
-00010e80: 746f 706f 6c6f 6779 5f79 616d 6c2c 0a20  topology_yaml,. 
-00010e90: 2020 2020 2020 2022 616c 676f 7269 7468         "algorith
-00010ea0: 6d22 3a20 616c 676f 7269 7468 6d2c 0a20  m": algorithm,. 
-00010eb0: 2020 2020 2020 2022 7377 6974 6368 5f6e         "switch_n
-00010ec0: 616d 6522 3a20 7377 6974 6368 5f6e 616d  ame": switch_nam
-00010ed0: 652c 0a20 2020 2020 2020 2022 6e75 6d62  e,.        "numb
-00010ee0: 6572 223a 206e 756d 6265 722c 0a20 2020  er": number,.   
-00010ef0: 2020 2020 2022 7265 736f 7572 6365 735f       "resources_
-00010f00: 6469 7222 3a20 7265 736f 7572 6365 735f  dir": resources_
-00010f10: 6469 722c 0a20 2020 207d 0a20 2020 2064  dir,.    }.    d
-00010f20: 6174 6120 3d20 6a73 6f6e 2e64 756d 7073  ata = json.dumps
-00010f30: 2864 6174 615f 6469 6374 290a 2020 2020  (data_dict).    
-00010f40: 7265 7375 6c74 203d 205f 706f 7374 280a  result = _post(.
-00010f50: 2020 2020 2020 2020 222f 746f 706f 6c6f          "/topolo
-00010f60: 6779 2f61 6464 5f64 6761 222c 0a20 2020  gy/add_dga",.   
-00010f70: 2020 2020 2064 6174 613d 6461 7461 2c0a       data=data,.
-00010f80: 2020 2020 2020 2020 6865 6164 6572 733d          headers=
-00010f90: 7b22 436f 6e74 656e 742d 5479 7065 223a  {"Content-Type":
-00010fa0: 2022 6170 706c 6963 6174 696f 6e2f 6a73   "application/js
-00010fb0: 6f6e 227d 2c0a 2020 2020 290a 0a20 2020  on"},.    )..   
-00010fc0: 2069 6620 7265 7375 6c74 2e73 7461 7475   if result.statu
-00010fd0: 735f 636f 6465 2021 3d20 3230 303a 0a20  s_code != 200:. 
-00010fe0: 2020 2020 2020 205f 6861 6e64 6c65 5f65         _handle_e
-00010ff0: 7272 6f72 2872 6573 756c 742c 2022 4572  rror(result, "Er
-00011000: 726f 7220 7768 696c 6520 6164 6469 6e67  ror while adding
-00011010: 2077 6562 7369 7465 7320 746f 2061 2074   websites to a t
-00011020: 6f70 6f6c 6f67 7922 290a 0a20 2020 2074  opology")..    t
-00011030: 6f70 6f6c 6f67 795f 7961 6d6c 203d 2072  opology_yaml = r
-00011040: 6573 756c 742e 6a73 6f6e 2829 5b22 746f  esult.json()["to
-00011050: 706f 6c6f 6779 5f79 616d 6c22 5d0a 2020  pology_yaml"].  
-00011060: 2020 646f 6d61 696e 7320 3d20 7265 7375    domains = resu
-00011070: 6c74 2e6a 736f 6e28 295b 2264 6f6d 6169  lt.json()["domai
-00011080: 6e73 225d 0a0a 2020 2020 7265 7475 726e  ns"]..    return
-00011090: 2074 6f70 6f6c 6f67 795f 7961 6d6c 2c20   topology_yaml, 
-000110a0: 646f 6d61 696e 730a 0a0a 6465 6620 746f  domains...def to
-000110b0: 706f 6c6f 6779 5f61 6464 5f64 6e73 5f73  pology_add_dns_s
-000110c0: 6572 7665 7228 0a20 2020 2074 6f70 6f6c  erver(.    topol
-000110d0: 6f67 795f 7961 6d6c 3a20 7374 722c 0a20  ogy_yaml: str,. 
-000110e0: 2020 2073 7769 7463 685f 6e61 6d65 3a20     switch_name: 
-000110f0: 7374 722c 0a20 2020 2072 6573 6f75 7263  str,.    resourc
-00011100: 6573 5f64 6972 3a20 7374 722c 0a29 202d  es_dir: str,.) -
-00011110: 3e20 5475 706c 655b 7374 722c 2073 7472  > Tuple[str, str
-00011120: 5d3a 0a20 2020 2064 6174 615f 6469 6374  ]:.    data_dict
-00011130: 203d 207b 0a20 2020 2020 2020 2022 746f   = {.        "to
-00011140: 706f 6c6f 6779 5f79 616d 6c22 3a20 746f  pology_yaml": to
-00011150: 706f 6c6f 6779 5f79 616d 6c2c 0a20 2020  pology_yaml,.   
-00011160: 2020 2020 2022 7377 6974 6368 5f6e 616d       "switch_nam
-00011170: 6522 3a20 7377 6974 6368 5f6e 616d 652c  e": switch_name,
-00011180: 0a20 2020 2020 2020 2022 7265 736f 7572  .        "resour
-00011190: 6365 735f 6469 7222 3a20 7265 736f 7572  ces_dir": resour
-000111a0: 6365 735f 6469 722c 0a20 2020 207d 0a20  ces_dir,.    }. 
-000111b0: 2020 2064 6174 6120 3d20 6a73 6f6e 2e64     data = json.d
-000111c0: 756d 7073 2864 6174 615f 6469 6374 290a  umps(data_dict).
-000111d0: 2020 2020 7265 7375 6c74 203d 205f 706f      result = _po
-000111e0: 7374 280a 2020 2020 2020 2020 222f 746f  st(.        "/to
-000111f0: 706f 6c6f 6779 2f61 6464 5f64 6e73 5f73  pology/add_dns_s
-00011200: 6572 7665 7222 2c0a 2020 2020 2020 2020  erver",.        
-00011210: 6461 7461 3d64 6174 612c 0a20 2020 2020  data=data,.     
-00011220: 2020 2068 6561 6465 7273 3d7b 2243 6f6e     headers={"Con
-00011230: 7465 6e74 2d54 7970 6522 3a20 2261 7070  tent-Type": "app
-00011240: 6c69 6361 7469 6f6e 2f6a 736f 6e22 7d2c  lication/json"},
-00011250: 0a20 2020 2029 0a0a 2020 2020 6966 2072  .    )..    if r
-00011260: 6573 756c 742e 7374 6174 7573 5f63 6f64  esult.status_cod
-00011270: 6520 213d 2032 3030 3a0a 2020 2020 2020  e != 200:.      
-00011280: 2020 5f68 616e 646c 655f 6572 726f 7228    _handle_error(
-00011290: 7265 7375 6c74 2c20 2245 7272 6f72 2077  result, "Error w
-000112a0: 6869 6c65 2061 6464 696e 6720 6120 444e  hile adding a DN
-000112b0: 5320 7365 7276 6572 2074 6f20 6120 746f  S server to a to
-000112c0: 706f 6c6f 6779 2229 0a0a 2020 2020 746f  pology")..    to
-000112d0: 706f 6c6f 6779 5f79 616d 6c20 3d20 7265  pology_yaml = re
-000112e0: 7375 6c74 2e6a 736f 6e28 295b 2274 6f70  sult.json()["top
-000112f0: 6f6c 6f67 795f 7961 6d6c 225d 0a20 2020  ology_yaml"].   
-00011300: 2064 6e73 5f63 6f6e 6620 3d20 7265 7375   dns_conf = resu
-00011310: 6c74 2e6a 736f 6e28 295b 2264 6e73 5f63  lt.json()["dns_c
-00011320: 6f6e 6622 5d0a 0a20 2020 2072 6574 7572  onf"]..    retur
-00011330: 6e20 746f 706f 6c6f 6779 5f79 616d 6c2c  n topology_yaml,
-00011340: 2064 6e73 5f63 6f6e 660a 0a0a 6465 6620   dns_conf...def 
-00011350: 746f 6f6c 735f 6765 6e65 7261 7465 5f64  tools_generate_d
-00011360: 6f6d 6169 6e73 280a 2020 2020 616c 676f  omains(.    algo
-00011370: 7269 7468 6d3a 2073 7472 2c0a 2020 2020  rithm: str,.    
-00011380: 6e75 6d62 6572 3a20 696e 742c 0a29 202d  number: int,.) -
-00011390: 3e20 4c69 7374 5b73 7472 5d3a 0a20 2020  > List[str]:.   
-000113a0: 2022 2222 0a20 2020 2047 656e 6572 6174   """.    Generat
-000113b0: 6520 646f 6d61 696e 206e 616d 6573 2061  e domain names a
-000113c0: 6363 6f72 6469 6e67 2074 6f20 7468 6520  ccording to the 
-000113d0: 6769 7665 6e20 616c 676f 7269 7468 6d0a  given algorithm.
-000113e0: 2020 2020 3a70 6172 616d 2061 6c67 6f72      :param algor
-000113f0: 6974 686d 3a20 616c 676f 7269 7468 6d20  ithm: algorithm 
-00011400: 746f 2075 7365 0a20 2020 203a 7061 7261  to use.    :para
-00011410: 6d20 6e75 6d62 6572 3a20 6e75 6d62 6572  m number: number
-00011420: 206f 6620 646f 6d61 696e 7320 746f 2067   of domains to g
-00011430: 656e 6572 6174 650a 2020 2020 3a72 6574  enerate.    :ret
-00011440: 7572 6e3a 2041 206c 6973 7420 6f66 2064  urn: A list of d
-00011450: 6f6d 6169 6e73 0a20 2020 2022 2222 0a20  omains.    """. 
-00011460: 2020 2064 6174 615f 6469 6374 203d 207b     data_dict = {
-00011470: 0a20 2020 2020 2020 2022 616c 676f 7269  .        "algori
-00011480: 7468 6d22 3a20 616c 676f 7269 7468 6d2c  thm": algorithm,
-00011490: 0a20 2020 2020 2020 2022 6e75 6d62 6572  .        "number
-000114a0: 223a 206e 756d 6265 722c 0a20 2020 207d  ": number,.    }
-000114b0: 0a20 2020 2064 6174 6120 3d20 6a73 6f6e  .    data = json
-000114c0: 2e64 756d 7073 2864 6174 615f 6469 6374  .dumps(data_dict
-000114d0: 290a 2020 2020 7265 7375 6c74 203d 205f  ).    result = _
-000114e0: 706f 7374 280a 2020 2020 2020 2020 222f  post(.        "/
-000114f0: 646f 6d61 696e 2f67 656e 6572 6174 655f  domain/generate_
-00011500: 646f 6d61 696e 7322 2c0a 2020 2020 2020  domains",.      
-00011510: 2020 6461 7461 3d64 6174 612c 0a20 2020    data=data,.   
-00011520: 2020 2020 2068 6561 6465 7273 3d7b 2243       headers={"C
-00011530: 6f6e 7465 6e74 2d54 7970 6522 3a20 2261  ontent-Type": "a
-00011540: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e22  pplication/json"
-00011550: 7d2c 0a20 2020 2029 0a0a 2020 2020 6966  },.    )..    if
-00011560: 2072 6573 756c 742e 7374 6174 7573 5f63   result.status_c
-00011570: 6f64 6520 213d 2032 3030 3a0a 2020 2020  ode != 200:.    
-00011580: 2020 2020 5f68 616e 646c 655f 6572 726f      _handle_erro
-00011590: 7228 7265 7375 6c74 2c20 2245 7272 6f72  r(result, "Error
-000115a0: 2077 6869 6c65 2067 656e 6572 6174 696e   while generatin
-000115b0: 6720 646f 6d61 696e 7322 290a 0a20 2020  g domains")..   
-000115c0: 2064 6f6d 6169 6e73 203d 2072 6573 756c   domains = resul
-000115d0: 742e 6a73 6f6e 2829 5b22 646f 6d61 696e  t.json()["domain
-000115e0: 7322 5d0a 0a20 2020 2072 6574 7572 6e20  s"]..    return 
-000115f0: 646f 6d61 696e 730a 0a0a 6465 6620 6665  domains...def fe
-00011600: 7463 685f 746f 706f 6c6f 6769 6573 2829  tch_topologies()
-00011610: 202d 3e20 416e 793a 0a20 2020 2022 2222   -> Any:.    """
-00011620: 5265 7475 726e 2074 6f70 6f6c 6f67 6965  Return topologie
-00011630: 7320 6c69 7374 2e22 2222 0a20 2020 2072  s list.""".    r
-00011640: 6573 756c 7420 3d20 5f67 6574 2822 2f74  esult = _get("/t
-00011650: 6f70 6f6c 6f67 7922 290a 0a20 2020 2069  opology")..    i
-00011660: 6620 7265 7375 6c74 2e73 7461 7475 735f  f result.status_
-00011670: 636f 6465 2021 3d20 3230 303a 0a20 2020  code != 200:.   
-00011680: 2020 2020 205f 6861 6e64 6c65 5f65 7272       _handle_err
-00011690: 6f72 2872 6573 756c 742c 2022 4361 6e6e  or(result, "Cann
-000116a0: 6f74 2072 6574 7269 6576 6520 746f 706f  ot retrieve topo
-000116b0: 6c6f 6769 6573 206c 6973 7420 6672 6f6d  logies list from
-000116c0: 2049 5420 5369 6d75 6c61 7469 6f6e 2041   IT Simulation A
-000116d0: 5049 2229 0a0a 2020 2020 746f 706f 6c6f  PI")..    topolo
-000116e0: 6769 6573 203d 2072 6573 756c 742e 6a73  gies = result.js
-000116f0: 6f6e 2829 0a20 2020 2072 6574 7572 6e20  on().    return 
-00011700: 746f 706f 6c6f 6769 6573 0a0a 0a23 2323  topologies...###
-00011710: 0a23 2053 696d 756c 6174 696f 6e20 636f  .# Simulation co
-00011720: 6d6d 616e 6473 0a23 2323 0a0a 0a64 6566  mmands.###...def
-00011730: 2073 7461 7274 5f73 696d 756c 6174 696f   start_simulatio
-00011740: 6e28 0a20 2020 2069 645f 7369 6d75 6c61  n(.    id_simula
-00011750: 7469 6f6e 3a20 696e 742c 0a20 2020 2075  tion: int,.    u
-00011760: 7365 5f69 6e73 7461 6c6c 5f74 696d 653a  se_install_time:
-00011770: 2062 6f6f 6c20 3d20 4661 6c73 652c 0a20   bool = False,. 
-00011780: 2020 2074 696d 656f 7574 3a20 696e 7420     timeout: int 
-00011790: 3d20 3330 302c 0a20 2020 206e 6f64 6573  = 300,.    nodes
-000117a0: 3a20 4f70 7469 6f6e 616c 5b4c 6973 745b  : Optional[List[
-000117b0: 7374 725d 5d20 3d20 4e6f 6e65 2c0a 2920  str]] = None,.) 
-000117c0: 2d3e 204e 6f6e 653a 0a20 2020 2022 2222  -> None:.    """
-000117d0: 5374 6172 7420 7468 6520 7369 6d75 6c61  Start the simula
-000117e0: 7469 6f6e 2c20 7769 7468 2063 7572 7265  tion, with curre
-000117f0: 6e74 2074 696d 6520 2862 7920 6465 6661  nt time (by defa
-00011800: 756c 7429 206f 7220 7469 6d65 2077 6865  ult) or time whe
-00011810: 7265 0a20 2020 2074 6865 2056 4d20 7761  re.    the VM wa
-00011820: 7320 6372 6561 7465 6420 2875 7365 5f69  s created (use_i
-00011830: 6e73 7461 6c6c 5f74 696d 653d 5472 7565  nstall_time=True
-00011840: 292e 2049 7420 6973 2070 6f73 7369 626c  ). It is possibl
-00011850: 6520 746f 0a20 2020 2073 7065 6369 6679  e to.    specify
-00011860: 2074 6865 206e 6f64 6573 2074 6f20 7374   the nodes to st
-00011870: 6172 742e 2042 7920 6465 6661 756c 742c  art. By default,
-00011880: 2061 6c6c 206e 6f64 6573 2061 7265 2073   all nodes are s
-00011890: 7461 7274 6564 2e0a 0a20 2020 2022 2222  tarted...    """
-000118a0: 0a20 2020 2023 2043 6865 636b 2074 6861  .    # Check tha
-000118b0: 7420 6e6f 206f 7468 6572 2073 696d 756c  t no other simul
-000118c0: 6174 696f 6e20 6973 2072 756e 6e69 6e67  ation is running
-000118d0: 0a20 2020 2073 696d 756c 6174 696f 6e5f  .    simulation_
-000118e0: 6c69 7374 203d 2066 6574 6368 5f73 696d  list = fetch_sim
-000118f0: 756c 6174 696f 6e73 2829 0a20 2020 2066  ulations().    f
-00011900: 6f72 2073 696d 756c 6174 696f 6e20 696e  or simulation in
-00011910: 2073 696d 756c 6174 696f 6e5f 6c69 7374   simulation_list
-00011920: 3a0a 2020 2020 2020 2020 6966 2073 696d  :.        if sim
-00011930: 756c 6174 696f 6e5b 2269 6422 5d20 213d  ulation["id"] !=
-00011940: 2069 645f 7369 6d75 6c61 7469 6f6e 2061   id_simulation a
-00011950: 6e64 2073 696d 756c 6174 696f 6e5b 2273  nd simulation["s
-00011960: 7461 7475 7322 5d20 3d3d 2022 5255 4e4e  tatus"] == "RUNN
-00011970: 494e 4722 3a0a 2020 2020 2020 2020 2020  ING":.          
-00011980: 2020 7261 6973 6520 4578 6365 7074 696f    raise Exceptio
-00011990: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
-000119a0: 2020 2022 4361 6e6e 6f74 2073 7461 7274     "Cannot start
-000119b0: 2061 206e 6577 2073 696d 756c 6174 696f   a new simulatio
-000119c0: 6e2c 2061 7320 7468 6520 7369 6d75 6c61  n, as the simula
-000119d0: 7469 6f6e 2027 7b7d 2720 6973 2022 0a20  tion '{}' is ". 
-000119e0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000119f0: 616c 7265 6164 7920 7275 6e6e 696e 6722  already running"
-00011a00: 2e66 6f72 6d61 7428 7369 6d75 6c61 7469  .format(simulati
-00011a10: 6f6e 5b22 6964 225d 290a 2020 2020 2020  on["id"]).      
-00011a20: 2020 2020 2020 290a 0a20 2020 2023 2049        )..    # I
-00011a30: 6e69 7469 6174 6520 7468 6520 7369 6d75  nitiate the simu
-00011a40: 6c61 7469 6f6e 0a20 2020 2069 6620 6e6f  lation.    if no
-00011a50: 6465 7320 6973 204e 6f6e 653a 0a20 2020  des is None:.   
-00011a60: 2020 2020 206e 6f64 6573 203d 205b 5d0a       nodes = [].
-00011a70: 2020 2020 706f 7374 5f64 6174 6120 3d20      post_data = 
-00011a80: 7b22 6e6f 6465 7322 3a20 6e6f 6465 737d  {"nodes": nodes}
-00011a90: 0a0a 2020 2020 5f73 696d 756c 6174 696f  ..    _simulatio
-00011aa0: 6e5f 6578 6563 7574 655f 6f70 6572 6174  n_execute_operat
-00011ab0: 696f 6e28 0a20 2020 2020 2020 2022 706f  ion(.        "po
-00011ac0: 7374 222c 0a20 2020 2020 2020 2022 7374  st",.        "st
-00011ad0: 6172 7422 2c0a 2020 2020 2020 2020 6964  art",.        id
-00011ae0: 5f73 696d 756c 6174 696f 6e2c 0a20 2020  _simulation,.   
-00011af0: 2020 2020 2022 5354 4152 5449 4e47 222c       "STARTING",
-00011b00: 0a20 2020 2020 2020 206f 7074 696f 6e61  .        optiona
-00011b10: 6c5f 7061 7261 6d31 3d75 7365 5f69 6e73  l_param1=use_ins
-00011b20: 7461 6c6c 5f74 696d 652c 0a20 2020 2020  tall_time,.     
-00011b30: 2020 206f 7074 696f 6e61 6c5f 7061 7261     optional_para
-00011b40: 6d32 3d74 696d 656f 7574 2c0a 2020 2020  m2=timeout,.    
-00011b50: 2020 2020 706f 7374 5f64 6174 613d 706f      post_data=po
-00011b60: 7374 5f64 6174 612c 0a20 2020 2029 0a0a  st_data,.    )..
-00011b70: 0a64 6566 2070 6175 7365 5f73 696d 756c  .def pause_simul
-00011b80: 6174 696f 6e28 6964 5f73 696d 756c 6174  ation(id_simulat
-00011b90: 696f 6e3a 2069 6e74 2920 2d3e 204e 6f6e  ion: int) -> Non
-00011ba0: 653a 0a20 2020 2022 2222 5061 7573 6520  e:.    """Pause 
-00011bb0: 6120 7369 6d75 6c61 7469 6f6e 2028 6361  a simulation (ca
-00011bc0: 6c6c 7320 6c69 6276 6972 7420 7375 7370  lls libvirt susp
-00011bd0: 656e 6420 4150 4929 2e22 2222 0a20 2020  end API).""".   
-00011be0: 205f 7369 6d75 6c61 7469 6f6e 5f65 7865   _simulation_exe
-00011bf0: 6375 7465 5f6f 7065 7261 7469 6f6e 2822  cute_operation("
-00011c00: 6765 7422 2c20 2270 6175 7365 222c 2069  get", "pause", i
-00011c10: 645f 7369 6d75 6c61 7469 6f6e 2c20 2250  d_simulation, "P
-00011c20: 4155 5349 4e47 2229 0a0a 0a64 6566 2075  AUSING")...def u
-00011c30: 6e70 6175 7365 5f73 696d 756c 6174 696f  npause_simulatio
-00011c40: 6e28 6964 5f73 696d 756c 6174 696f 6e3a  n(id_simulation:
-00011c50: 2069 6e74 2920 2d3e 204e 6f6e 653a 0a20   int) -> None:. 
-00011c60: 2020 2022 2222 556e 7061 7573 6520 6120     """Unpause a 
-00011c70: 7369 6d75 6c61 7469 6f6e 2028 6361 6c6c  simulation (call
-00011c80: 7320 6c69 6276 6972 7420 7265 7375 6d65  s libvirt resume
-00011c90: 2041 5049 292e 2222 220a 2020 2020 5f73   API).""".    _s
-00011ca0: 696d 756c 6174 696f 6e5f 6578 6563 7574  imulation_execut
-00011cb0: 655f 6f70 6572 6174 696f 6e28 2267 6574  e_operation("get
-00011cc0: 222c 2022 756e 7061 7573 6522 2c20 6964  ", "unpause", id
-00011cd0: 5f73 696d 756c 6174 696f 6e2c 2022 554e  _simulation, "UN
-00011ce0: 5041 5553 494e 4722 290a 0a0a 6465 6620  PAUSING")...def 
-00011cf0: 6372 6561 7465 5f62 6163 6b75 705f 7369  create_backup_si
-00011d00: 6d75 6c61 7469 6f6e 280a 2020 2020 6964  mulation(.    id
-00011d10: 5f73 696d 756c 6174 696f 6e3a 2069 6e74  _simulation: int
-00011d20: 2c0a 2020 2020 6e6f 6465 733a 204f 7074  ,.    nodes: Opt
-00011d30: 696f 6e61 6c5b 4c69 7374 5b73 7472 5d5d  ional[List[str]]
-00011d40: 203d 204e 6f6e 652c 0a29 202d 3e20 4e6f   = None,.) -> No
-00011d50: 6e65 3a0a 2020 2020 2222 2243 7265 6174  ne:.    """Creat
-00011d60: 6520 6261 636b 7570 206f 6620 6120 7369  e backup of a si
-00011d70: 6d75 6c61 7469 6f6e 2e20 4974 2069 7320  mulation. It is 
-00011d80: 706f 7373 6962 6c65 2074 6f20 7370 6563  possible to spec
-00011d90: 6966 7920 7468 6520 6e6f 6465 730a 2020  ify the nodes.  
-00011da0: 2020 746f 2062 6163 6b75 702e 2042 7920    to backup. By 
-00011db0: 6465 6661 756c 742c 2061 6c6c 206e 6f64  default, all nod
-00011dc0: 6573 2061 7265 2062 6163 6b65 6420 7570  es are backed up
-00011dd0: 2e0a 0a20 2020 2022 2222 0a0a 2020 2020  ...    """..    
-00011de0: 6966 206e 6f64 6573 2069 7320 4e6f 6e65  if nodes is None
-00011df0: 3a0a 2020 2020 2020 2020 6e6f 6465 7320  :.        nodes 
-00011e00: 3d20 5b5d 0a20 2020 2070 6f73 745f 6461  = [].    post_da
-00011e10: 7461 203d 207b 226e 6f64 6573 223a 206e  ta = {"nodes": n
-00011e20: 6f64 6573 7d0a 0a20 2020 205f 7369 6d75  odes}..    _simu
-00011e30: 6c61 7469 6f6e 5f65 7865 6375 7465 5f6f  lation_execute_o
-00011e40: 7065 7261 7469 6f6e 280a 2020 2020 2020  peration(.      
-00011e50: 2020 2270 6f73 7422 2c20 2263 7265 6174    "post", "creat
-00011e60: 655f 6261 636b 7570 222c 2069 645f 7369  e_backup", id_si
-00011e70: 6d75 6c61 7469 6f6e 2c20 2250 5245 5041  mulation, "PREPA
-00011e80: 5249 4e47 222c 2070 6f73 745f 6461 7461  RING", post_data
-00011e90: 3d70 6f73 745f 6461 7461 0a20 2020 2029  =post_data.    )
-00011ea0: 0a0a 0a64 6566 2072 6573 746f 7265 5f62  ...def restore_b
-00011eb0: 6163 6b75 705f 7369 6d75 6c61 7469 6f6e  ackup_simulation
-00011ec0: 280a 2020 2020 6964 5f73 696d 756c 6174  (.    id_simulat
-00011ed0: 696f 6e3a 2069 6e74 2c0a 2020 2020 6e6f  ion: int,.    no
-00011ee0: 6465 733a 204f 7074 696f 6e61 6c5b 4c69  des: Optional[Li
-00011ef0: 7374 5b73 7472 5d5d 203d 204e 6f6e 652c  st[str]] = None,
-00011f00: 0a29 202d 3e20 4e6f 6e65 3a0a 2020 2020  .) -> None:.    
-00011f10: 2222 2252 6573 746f 7265 2062 6163 6b75  """Restore backu
-00011f20: 7020 6f66 2061 2073 696d 756c 6174 696f  p of a simulatio
-00011f30: 6e2e 2049 7420 6973 2070 6f73 7369 626c  n. It is possibl
-00011f40: 6520 746f 2073 7065 6369 6679 2074 6865  e to specify the
-00011f50: 206e 6f64 6573 0a20 2020 2074 6f20 7265   nodes.    to re
-00011f60: 7374 6f72 652e 2042 7920 6465 6661 756c  store. By defaul
-00011f70: 742c 2061 6c6c 206e 6f64 6573 2061 7265  t, all nodes are
-00011f80: 2072 6573 746f 7265 642e 0a0a 2020 2020   restored...    
-00011f90: 2222 220a 0a20 2020 2069 6620 6e6f 6465  """..    if node
-00011fa0: 7320 6973 204e 6f6e 653a 0a20 2020 2020  s is None:.     
-00011fb0: 2020 206e 6f64 6573 203d 205b 5d0a 2020     nodes = [].  
-00011fc0: 2020 706f 7374 5f64 6174 6120 3d20 7b22    post_data = {"
-00011fd0: 6e6f 6465 7322 3a20 6e6f 6465 737d 0a0a  nodes": nodes}..
-00011fe0: 2020 2020 5f73 696d 756c 6174 696f 6e5f      _simulation_
-00011ff0: 6578 6563 7574 655f 6f70 6572 6174 696f  execute_operatio
-00012000: 6e28 0a20 2020 2020 2020 2022 706f 7374  n(.        "post
-00012010: 222c 2022 7265 7374 6f72 655f 6261 636b  ", "restore_back
-00012020: 7570 222c 2069 645f 7369 6d75 6c61 7469  up", id_simulati
-00012030: 6f6e 2c20 2250 5245 5041 5249 4e47 222c  on, "PREPARING",
-00012040: 2070 6f73 745f 6461 7461 3d70 6f73 745f   post_data=post_
-00012050: 6461 7461 0a20 2020 2029 0a0a 0a64 6566  data.    )...def
-00012060: 2068 616c 745f 7369 6d75 6c61 7469 6f6e   halt_simulation
-00012070: 280a 2020 2020 6964 5f73 696d 756c 6174  (.    id_simulat
-00012080: 696f 6e3a 2069 6e74 2c20 6e6f 6465 733a  ion: int, nodes:
-00012090: 204f 7074 696f 6e61 6c5b 4c69 7374 5b73   Optional[List[s
-000120a0: 7472 5d5d 203d 204e 6f6e 650a 2920 2d3e  tr]] = None.) ->
-000120b0: 204f 7074 696f 6e61 6c5b 7575 6964 2e55   Optional[uuid.U
-000120c0: 5549 445d 3a0a 2020 2020 2222 2250 726f  UID]:.    """Pro
-000120d0: 7065 726c 7920 7374 6f70 2061 2073 696d  perly stop a sim
-000120e0: 756c 6174 696f 6e2c 2062 7920 7365 6e64  ulation, by send
-000120f0: 696e 6720 6120 7368 7574 646f 776e 2073  ing a shutdown s
-00012100: 6967 6e61 6c20 746f 2074 6865 0a20 2020  ignal to the.   
-00012110: 206f 7065 7261 7469 6e67 2073 7973 7465   operating syste
-00012120: 6d73 2e20 4974 2069 7320 706f 7373 6962  ms. It is possib
-00012130: 6c65 2074 6f20 7370 6563 6966 7920 7468  le to specify th
-00012140: 6520 6e6f 6465 7320 746f 0a20 2020 2073  e nodes to.    s
-00012150: 7461 7274 2e20 4279 2064 6566 6175 6c74  tart. By default
-00012160: 2c20 616c 6c20 6e6f 6465 7320 6172 6520  , all nodes are 
-00012170: 7374 6172 7465 642e 0a0a 2020 2020 2222  started...    ""
-00012180: 220a 2020 2020 6966 206e 6f64 6573 2069  ".    if nodes i
-00012190: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-000121a0: 6e6f 6465 7320 3d20 5b5d 0a20 2020 2070  nodes = [].    p
-000121b0: 6f73 745f 6461 7461 203d 207b 226e 6f64  ost_data = {"nod
-000121c0: 6573 223a 206e 6f64 6573 7d0a 0a20 2020  es": nodes}..   
-000121d0: 205f 7369 6d75 6c61 7469 6f6e 5f65 7865   _simulation_exe
-000121e0: 6375 7465 5f6f 7065 7261 7469 6f6e 280a  cute_operation(.
-000121f0: 2020 2020 2020 2020 2270 6f73 7422 2c0a          "post",.
-00012200: 2020 2020 2020 2020 2273 746f 7022 2c0a          "stop",.
-00012210: 2020 2020 2020 2020 6964 5f73 696d 756c          id_simul
-00012220: 6174 696f 6e2c 0a20 2020 2020 2020 2022  ation,.        "
-00012230: 5354 4f50 5049 4e47 222c 0a20 2020 2020  STOPPING",.     
-00012240: 2020 2070 6f73 745f 6461 7461 3d70 6f73     post_data=pos
-00012250: 745f 6461 7461 2c0a 2020 2020 290a 0a0a  t_data,.    )...
-00012260: 6465 6620 6465 7374 726f 795f 7369 6d75  def destroy_simu
-00012270: 6c61 7469 6f6e 2869 645f 7369 6d75 6c61  lation(id_simula
-00012280: 7469 6f6e 3a20 696e 742c 206e 6f64 6573  tion: int, nodes
-00012290: 3a20 4f70 7469 6f6e 616c 5b4c 6973 745b  : Optional[List[
-000122a0: 7374 725d 5d20 3d20 4e6f 6e65 2920 2d3e  str]] = None) ->
-000122b0: 204e 6f6e 653a 0a20 2020 2022 2222 5374   None:.    """St
-000122c0: 6f70 2061 2073 696d 756c 6174 696f 6e20  op a simulation 
-000122d0: 7468 726f 7567 6820 6120 6861 7264 2072  through a hard r
-000122e0: 6573 6574 2e22 2222 0a0a 2020 2020 6966  eset."""..    if
-000122f0: 206e 6f64 6573 2069 7320 4e6f 6e65 3a0a   nodes is None:.
-00012300: 2020 2020 2020 2020 6e6f 6465 7320 3d20          nodes = 
-00012310: 5b5d 0a20 2020 2070 6f73 745f 6461 7461  [].    post_data
-00012320: 203d 207b 226e 6f64 6573 223a 206e 6f64   = {"nodes": nod
-00012330: 6573 7d0a 0a20 2020 205f 7369 6d75 6c61  es}..    _simula
-00012340: 7469 6f6e 5f65 7865 6375 7465 5f6f 7065  tion_execute_ope
-00012350: 7261 7469 6f6e 280a 2020 2020 2020 2020  ration(.        
-00012360: 2270 6f73 7422 2c20 2264 6573 7472 6f79  "post", "destroy
-00012370: 222c 2069 645f 7369 6d75 6c61 7469 6f6e  ", id_simulation
-00012380: 2c20 2253 544f 5050 494e 4722 2c20 706f  , "STOPPING", po
-00012390: 7374 5f64 6174 613d 706f 7374 5f64 6174  st_data=post_dat
-000123a0: 610a 2020 2020 290a 0a0a 6465 6620 636c  a.    )...def cl
-000123b0: 6f6e 655f 7369 6d75 6c61 7469 6f6e 2869  one_simulation(i
-000123c0: 645f 7369 6d75 6c61 7469 6f6e 3a20 696e  d_simulation: in
-000123d0: 7429 202d 3e20 696e 743a 0a20 2020 2022  t) -> int:.    "
-000123e0: 2222 436c 6f6e 6520 6120 7369 6d75 6c61  ""Clone a simula
-000123f0: 7469 6f6e 2061 6e64 2063 7265 6174 6520  tion and create 
-00012400: 6120 6e65 7720 7369 6d75 6c61 7469 6f6e  a new simulation
-00012410: 2c20 616e 6420 7265 7475 726e 2074 6865  , and return the
-00012420: 206e 6577 2049 442e 2222 220a 2020 2020   new ID.""".    
-00012430: 6964 5f6e 6577 5f73 696d 756c 6174 696f  id_new_simulatio
-00012440: 6e20 3d20 5f73 696d 756c 6174 696f 6e5f  n = _simulation_
-00012450: 6578 6563 7574 655f 6f70 6572 6174 696f  execute_operatio
-00012460: 6e28 0a20 2020 2020 2020 2022 6765 7422  n(.        "get"
-00012470: 2c20 2263 6c6f 6e65 222c 2069 645f 7369  , "clone", id_si
-00012480: 6d75 6c61 7469 6f6e 2c20 2243 4c4f 4e49  mulation, "CLONI
-00012490: 4e47 220a 2020 2020 290a 2020 2020 7265  NG".    ).    re
-000124a0: 7475 726e 2069 645f 6e65 775f 7369 6d75  turn id_new_simu
-000124b0: 6c61 7469 6f6e 0a0a 0a64 6566 206e 6574  lation...def net
-000124c0: 5f63 7265 6174 655f 7072 6f62 6528 2020  _create_probe(  
-000124d0: 2320 6e6f 7161 3a20 4339 3031 0a20 2020  # noqa: C901.   
-000124e0: 2069 645f 7369 6d75 6c61 7469 6f6e 3a20   id_simulation: 
-000124f0: 696e 742c 0a20 2020 2073 696d 755f 6e6f  int,.    simu_no
-00012500: 6465 733a 2044 6963 742c 0a20 2020 2069  des: Dict,.    i
-00012510: 6661 6365 3a20 4f70 7469 6f6e 616c 5b73  face: Optional[s
-00012520: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
-00012530: 7063 6170 3a20 4f70 7469 6f6e 616c 5b62  pcap: Optional[b
-00012540: 6f6f 6c5d 203d 2046 616c 7365 2c0a 2020  ool] = False,.  
-00012550: 2020 6669 6c74 6572 3a20 4f70 7469 6f6e    filter: Option
-00012560: 616c 5b73 7472 5d20 3d20 2222 2c0a 2020  al[str] = "",.  
-00012570: 2020 6469 7265 6374 696f 6e3a 204f 7074    direction: Opt
-00012580: 696f 6e61 6c5b 7374 725d 203d 2022 626f  ional[str] = "bo
-00012590: 7468 222c 0a29 202d 3e20 696e 743a 0a20  th",.) -> int:. 
-000125a0: 2020 2022 2222 4372 6561 7465 2061 206e     """Create a n
-000125b0: 6577 2070 726f 6265 2061 6e64 2063 6f6e  ew probe and con
-000125c0: 6669 6775 7265 2068 6973 206e 6574 776f  figure his netwo
-000125d0: 726b 2063 6f6c 6c65 6374 696f 6e73 2070  rk collections p
-000125e0: 6f69 6e74 732e 0a0a 2020 2020 3a70 6172  oints...    :par
-000125f0: 616d 2069 645f 7369 6d75 6c61 7469 6f6e  am id_simulation
-00012600: 3a20 5468 6520 6964 206f 6620 7468 6520  : The id of the 
-00012610: 7369 6d75 6c61 7469 6f6e 2e0a 2020 2020  simulation..    
-00012620: 3a70 6172 616d 2073 696d 755f 6e6f 6465  :param simu_node
-00012630: 733a 2041 2064 6963 7469 6f6e 6172 7920  s: A dictionary 
-00012640: 7374 6f72 696e 6720 7468 6520 636f 6c6c  storing the coll
-00012650: 6563 7469 6f6e 2070 6f69 6e74 7320 746f  ection points to
-00012660: 2063 6170 7475 7265 2e0a 2020 2020 3a70   capture..    :p
-00012670: 6172 616d 2069 6661 6365 3a20 496e 7465  aram iface: Inte
-00012680: 7266 6163 6520 7768 6572 6520 7468 6520  rface where the 
-00012690: 7472 6166 6669 6320 6973 206d 6972 726f  traffic is mirro
-000126a0: 7265 6420 746f 2e0a 2020 2020 3a70 6172  red to..    :par
-000126b0: 616d 2070 6361 703a 2041 2062 6f6f 6c65  am pcap: A boole
-000126c0: 616e 2069 6e64 6963 6174 696e 6720 6966  an indicating if
-000126d0: 2074 6865 2063 6170 7475 7265 2073 686f   the capture sho
-000126e0: 756c 6420 6265 2073 6176 6564 206f 6e20  uld be saved on 
-000126f0: 6469 736b 2069 6e20 6120 7063 6170 2066  disk in a pcap f
-00012700: 696c 6520 2874 6f20 6265 2069 6e63 6c75  ile (to be inclu
-00012710: 6465 6420 696e 2064 6174 6173 6574 290a  ded in dataset).
-00012720: 2020 2020 3a70 6172 616d 2066 696c 7465      :param filte
-00012730: 723a 2053 7472 696e 6720 6669 6c74 6572  r: String filter
-00012740: 696e 6720 7463 7064 756d 7020 6361 7074  ing tcpdump capt
-00012750: 7572 650a 2020 2020 3a70 6172 616d 2064  ure.    :param d
-00012760: 6972 6563 7469 6f6e 3a20 5365 6c65 6374  irection: Select
-00012770: 2077 6869 6368 2074 7261 6666 6963 2074   which traffic t
-00012780: 6f20 6d6f 6e69 746f 7220 6f6e 2074 6865  o monitor on the
-00012790: 206d 6972 726f 7265 6420 696e 7465 7266   mirrored interf
-000127a0: 6163 6528 7329 3a20 6569 7468 6572 2027  ace(s): either '
-000127b0: 696e 6772 6573 7327 2c20 2765 6772 6573  ingress', 'egres
-000127c0: 7327 206f 7220 2762 6f74 6827 2e0a 0a20  s' or 'both'... 
-000127d0: 2020 203a 7479 7065 2069 645f 7369 6d75     :type id_simu
-000127e0: 6c61 7469 6f6e 3a20 3a63 6c61 7373 3a60  lation: :class:`
-000127f0: 696e 7460 2c20 6578 203a 2031 0a20 2020  int`, ex : 1.   
-00012800: 203a 7479 7065 2073 696d 755f 6e6f 6465   :type simu_node
-00012810: 733a 203a 636c 6173 733a 6044 6963 7460  s: :class:`Dict`
-00012820: 2c20 6578 203a 207b 2773 7769 7463 6873  , ex : {'switchs
-00012830: 273a 205b 5b27 7377 6974 6368 3127 2c20  ': [['switch1', 
-00012840: 2763 6c69 656e 7431 275d 5d2c 2027 6e6f  'client1']], 'no
-00012850: 6465 7327 3a20 5b27 636c 6965 6e74 3227  des': ['client2'
-00012860: 5d7d 0a20 2020 203a 7479 7065 2069 6661  ]}.    :type ifa
-00012870: 6365 3a20 3a63 6c61 7373 3a60 7374 7260  ce: :class:`str`
-00012880: 2c20 6578 203a 2064 756d 6d79 300a 2020  , ex : dummy0.  
-00012890: 2020 3a74 7970 6520 7063 6170 3a20 3a63    :type pcap: :c
-000128a0: 6c61 7373 3a60 626f 6f6c 602c 2065 7820  lass:`bool`, ex 
-000128b0: 3a20 7472 7565 0a20 2020 203a 7479 7065  : true.    :type
-000128c0: 2066 696c 7465 723a 203a 636c 6173 733a   filter: :class:
-000128d0: 6073 7472 602c 2065 7820 3a20 7463 7020  `str`, ex : tcp 
-000128e0: 706f 7274 2038 300a 2020 2020 3a74 7970  port 80.    :typ
-000128f0: 6520 6469 7265 6374 696f 6e3a 203a 636c  e direction: :cl
-00012900: 6173 733a 6073 7472 602c 2065 7820 3a20  ass:`str`, ex : 
-00012910: 696e 6772 6573 730a 2020 2020 2222 220a  ingress.    """.
-00012920: 0a20 2020 206e 6574 776f 726b 5f69 6e74  .    network_int
-00012930: 6572 6661 6365 7320 3d20 5b5d 0a0a 2020  erfaces = []..  
-00012940: 2020 6966 2073 696d 755f 6e6f 6465 735b    if simu_nodes[
-00012950: 2273 7769 7463 6873 225d 2069 7320 4e6f  "switchs"] is No
-00012960: 6e65 2061 6e64 2073 696d 755f 6e6f 6465  ne and simu_node
-00012970: 735b 226e 6f64 6573 225d 2069 7320 4e6f  s["nodes"] is No
-00012980: 6e65 3a0a 2020 2020 2020 2020 2320 436f  ne:.        # Co
-00012990: 6e73 6964 6572 2061 6c6c 206e 6f64 6520  nsider all node 
-000129a0: 6f66 2074 6865 2073 696d 756c 6174 696f  of the simulatio
-000129b0: 6e20 2865 7863 6570 7420 726f 7574 6572  n (except router
-000129c0: 7320 7468 6174 2061 7265 0a20 2020 2020  s that are.     
-000129d0: 2020 2023 204f 564e 2061 6273 7472 6163     # OVN abstrac
-000129e0: 7420 6f62 6a65 6374 7320 6f6e 2077 6869  t objects on whi
-000129f0: 6368 2069 7420 6973 206e 6f74 2070 6f73  ch it is not pos
-00012a00: 7369 626c 6520 746f 2063 6170 7475 7265  sible to capture
-00012a10: 0a20 2020 2020 2020 2023 2074 7261 6666  .        # traff
-00012a20: 6963 290a 2020 2020 2020 2020 666f 7220  ic).        for 
-00012a30: 6e6f 6465 2069 6e20 6665 7463 685f 6e6f  node in fetch_no
-00012a40: 6465 7328 6964 5f73 696d 756c 6174 696f  des(id_simulatio
-00012a50: 6e29 3a0a 2020 2020 2020 2020 2020 2020  n):.            
-00012a60: 6966 206e 6f64 655b 2274 7970 6522 5d20  if node["type"] 
-00012a70: 213d 2022 726f 7574 6572 223a 0a20 2020  != "router":.   
-00012a80: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00012a90: 206e 6574 776f 726b 5f69 6e74 6572 6661   network_interfa
-00012aa0: 6365 2069 6e20 6e6f 6465 5b22 6e65 7477  ce in node["netw
-00012ab0: 6f72 6b5f 696e 7465 7266 6163 6573 225d  ork_interfaces"]
-00012ac0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00012ad0: 2020 2020 2020 6e65 7477 6f72 6b5f 696e        network_in
-00012ae0: 7465 7266 6163 6573 2e61 7070 656e 6428  terfaces.append(
-00012af0: 6e65 7477 6f72 6b5f 696e 7465 7266 6163  network_interfac
-00012b00: 655b 226d 6163 5f61 6464 7265 7373 225d  e["mac_address"]
-00012b10: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
-00012b20: 2020 2020 6966 2073 696d 755f 6e6f 6465      if simu_node
-00012b30: 735b 2273 7769 7463 6873 225d 2069 7320  s["switchs"] is 
-00012b40: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00012b50: 2020 2020 2020 2320 4d69 7272 6f72 2074        # Mirror t
-00012b60: 7261 6666 6963 2066 726f 6d20 6e6f 6465  raffic from node
-00012b70: 2069 6e74 6572 6661 6365 7320 636f 6e6e   interfaces conn
-00012b80: 6563 7465 6420 746f 2074 6865 2073 7065  ected to the spe
-00012b90: 6369 6669 6564 2073 7769 7463 6873 0a20  cified switchs. 
-00012ba0: 2020 2020 2020 2020 2020 2066 6f72 2073             for s
-00012bb0: 7769 7463 685f 6e6f 6465 7320 696e 2073  witch_nodes in s
-00012bc0: 696d 755f 6e6f 6465 735b 2273 7769 7463  imu_nodes["switc
-00012bd0: 6873 225d 3a0a 2020 2020 2020 2020 2020  hs"]:.          
-00012be0: 2020 2020 2020 7377 6974 6368 203d 2066        switch = f
-00012bf0: 6574 6368 5f6e 6f64 655f 6279 5f6e 616d  etch_node_by_nam
-00012c00: 6528 6964 5f73 696d 756c 6174 696f 6e2c  e(id_simulation,
-00012c10: 2073 7769 7463 685f 6e6f 6465 735b 305d   switch_nodes[0]
-00012c20: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
-00012c30: 2020 2023 2043 6865 636b 2069 6620 7370     # Check if sp
-00012c40: 6563 6966 6963 206e 6f64 6573 2061 7265  ecific nodes are
-00012c50: 2064 6566 696e 6564 2c20 666f 7220 7468   defined, for th
-00012c60: 6973 2073 7769 7463 680a 2020 2020 2020  is switch.      
-00012c70: 2020 2020 2020 2020 2020 6966 2073 7769            if swi
-00012c80: 7463 685f 6e6f 6465 735b 313a 5d3a 0a20  tch_nodes[1:]:. 
-00012c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ca0: 2020 2066 6f72 206e 6f64 655f 6e61 6d65     for node_name
-00012cb0: 2069 6e20 7377 6974 6368 5f6e 6f64 6573   in switch_nodes
-00012cc0: 5b31 3a5d 3a0a 2020 2020 2020 2020 2020  [1:]:.          
-00012cd0: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
-00012ce0: 6465 203d 2066 6574 6368 5f6e 6f64 655f  de = fetch_node_
-00012cf0: 6279 5f6e 616d 6528 6964 5f73 696d 756c  by_name(id_simul
-00012d00: 6174 696f 6e2c 206e 6f64 655f 6e61 6d65  ation, node_name
-00012d10: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
-00012d20: 2020 2020 2020 2020 2020 2066 6f72 206e             for n
-00012d30: 6574 776f 726b 5f69 6e74 6572 6661 6365  etwork_interface
-00012d40: 2069 6e20 6e6f 6465 5b22 6e65 7477 6f72   in node["networ
-00012d50: 6b5f 696e 7465 7266 6163 6573 225d 3a0a  k_interfaces"]:.
-00012d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d70: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00012d80: 6574 776f 726b 5f69 6e74 6572 6661 6365  etwork_interface
-00012d90: 5b22 7377 6974 6368 5f6e 616d 6522 5d20  ["switch_name"] 
-00012da0: 3d3d 2073 7769 7463 685b 226e 616d 6522  == switch["name"
-00012db0: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
-00012dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012dd0: 2020 206e 6574 776f 726b 5f69 6e74 6572     network_inter
-00012de0: 6661 6365 732e 6170 7065 6e64 280a 2020  faces.append(.  
-00012df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e10: 2020 6e65 7477 6f72 6b5f 696e 7465 7266    network_interf
-00012e20: 6163 655b 226d 6163 5f61 6464 7265 7373  ace["mac_address
-00012e30: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
-00012e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e50: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00012e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e70: 2020 2020 2062 7265 616b 0a20 2020 2020       break.     
-00012e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e90: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00012ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012eb0: 2020 2020 2072 6169 7365 2045 7863 6570       raise Excep
-00012ec0: 7469 6f6e 280a 2020 2020 2020 2020 2020  tion(.          
-00012ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ee0: 2020 2020 2020 2254 6865 206e 6f64 6520        "The node 
-00012ef0: 277b 7d27 2069 736e 2774 206c 696e 6b65  '{}' isn't linke
-00012f00: 6420 7769 7468 2074 6865 2073 7769 7463  d with the switc
-00012f10: 6820 277b 7d27 222e 666f 726d 6174 280a  h '{}'".format(.
-00012f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f40: 2020 2020 6e6f 6465 5f6e 616d 652c 2073      node_name, s
-00012f50: 7769 7463 685b 226e 616d 6522 5d0a 2020  witch["name"].  
-00012f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f70: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00012f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f90: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00012fa0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00012fb0: 456c 7365 2c20 636f 6e73 6964 6572 2061  Else, consider a
-00012fc0: 6c6c 206e 6f64 6573 2063 6f6e 6e65 6374  ll nodes connect
-00012fd0: 6564 2074 6f20 7468 6520 7377 6974 6368  ed to the switch
-00012fe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012ff0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00013000: 2020 2020 2020 2020 2020 2066 6f72 206e             for n
-00013010: 6f64 6520 696e 2066 6574 6368 5f6e 6f64  ode in fetch_nod
-00013020: 6573 2869 645f 7369 6d75 6c61 7469 6f6e  es(id_simulation
-00013030: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00013040: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-00013050: 6465 5b22 7479 7065 225d 2021 3d20 2272  de["type"] != "r
-00013060: 6f75 7465 7222 3a0a 2020 2020 2020 2020  outer":.        
-00013070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013080: 2020 2020 666f 7220 6e65 7477 6f72 6b5f      for network_
-00013090: 696e 7465 7266 6163 6520 696e 206e 6f64  interface in nod
-000130a0: 655b 226e 6574 776f 726b 5f69 6e74 6572  e["network_inter
-000130b0: 6661 6365 7322 5d3a 0a20 2020 2020 2020  faces"]:.       
-000130c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000130d0: 2020 2020 2020 2020 2069 6620 6e65 7477           if netw
-000130e0: 6f72 6b5f 696e 7465 7266 6163 655b 2273  ork_interface["s
-000130f0: 7769 7463 685f 6e61 6d65 225d 203d 3d20  witch_name"] == 
-00013100: 7377 6974 6368 5b22 6e61 6d65 225d 3a0a  switch["name"]:.
-00013110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013130: 2020 2020 6e65 7477 6f72 6b5f 696e 7465      network_inte
-00013140: 7266 6163 6573 2e61 7070 656e 6428 0a20  rfaces.append(. 
-00013150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013170: 2020 2020 2020 206e 6574 776f 726b 5f69         network_i
-00013180: 6e74 6572 6661 6365 5b22 6d61 635f 6164  nterface["mac_ad
-00013190: 6472 6573 7322 5d0a 2020 2020 2020 2020  dress"].        
-000131a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000131b0: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-000131c0: 2020 2020 2020 2069 6620 7369 6d75 5f6e         if simu_n
-000131d0: 6f64 6573 5b22 6e6f 6465 7322 5d20 6973  odes["nodes"] is
-000131e0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000131f0: 2020 2020 2020 2023 204d 6972 726f 7220         # Mirror 
-00013200: 7472 6166 6669 6320 6f6e 2061 6c6c 2069  traffic on all i
-00013210: 6e74 6572 6661 6365 7320 6672 6f6d 2074  nterfaces from t
-00013220: 6865 2073 7065 6369 6669 6564 206e 6f64  he specified nod
-00013230: 6573 0a20 2020 2020 2020 2020 2020 2066  es.            f
-00013240: 6f72 206e 6f64 655f 6e61 6d65 2069 6e20  or node_name in 
-00013250: 7369 6d75 5f6e 6f64 6573 5b22 6e6f 6465  simu_nodes["node
-00013260: 7322 5d3a 0a20 2020 2020 2020 2020 2020  s"]:.           
-00013270: 2020 2020 2066 6f72 206e 6574 776f 726b       for network
-00013280: 5f69 6e74 6572 6661 6365 2069 6e20 6665  _interface in fe
-00013290: 7463 685f 6e6f 6465 5f62 795f 6e61 6d65  tch_node_by_name
-000132a0: 2869 645f 7369 6d75 6c61 7469 6f6e 2c20  (id_simulation, 
-000132b0: 6e6f 6465 5f6e 616d 6529 5b0a 2020 2020  node_name)[.    
-000132c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000132d0: 226e 6574 776f 726b 5f69 6e74 6572 6661  "network_interfa
-000132e0: 6365 7322 0a20 2020 2020 2020 2020 2020  ces".           
-000132f0: 2020 2020 205d 3a0a 2020 2020 2020 2020       ]:.        
-00013300: 2020 2020 2020 2020 2020 2020 6e65 7477              netw
-00013310: 6f72 6b5f 696e 7465 7266 6163 6573 2e61  ork_interfaces.a
-00013320: 7070 656e 6428 6e65 7477 6f72 6b5f 696e  ppend(network_in
-00013330: 7465 7266 6163 655b 226d 6163 5f61 6464  terface["mac_add
-00013340: 7265 7373 225d 290a 0a20 2020 2070 726f  ress"])..    pro
-00013350: 6265 5f69 6420 3d20 6372 6561 7465 5f70  be_id = create_p
-00013360: 726f 6265 280a 2020 2020 2020 2020 6964  robe(.        id
-00013370: 5f73 696d 756c 6174 696f 6e2c 206e 6574  _simulation, net
-00013380: 776f 726b 5f69 6e74 6572 6661 6365 732c  work_interfaces,
-00013390: 2069 6661 6365 2c20 7063 6170 2c20 6669   iface, pcap, fi
-000133a0: 6c74 6572 2c20 6469 7265 6374 696f 6e0a  lter, direction.
-000133b0: 2020 2020 290a 0a20 2020 2072 6574 7572      )..    retur
-000133c0: 6e20 7072 6f62 655f 6964 0a0a 0a64 6566  n probe_id...def
-000133d0: 206e 6574 5f73 7461 7274 5f70 726f 6265   net_start_probe
-000133e0: 2869 645f 7369 6d75 6c61 7469 6f6e 3a20  (id_simulation: 
-000133f0: 696e 742c 2070 726f 6265 5f69 643a 2069  int, probe_id: i
-00013400: 6e74 2920 2d3e 204e 6f6e 653a 0a20 2020  nt) -> None:.   
-00013410: 2022 2222 5265 6469 7265 6374 206e 6574   """Redirect net
-00013420: 776f 726b 2074 7261 6666 6963 2074 6f20  work traffic to 
-00013430: 7468 6520 7072 6f62 6520 696e 7465 7266  the probe interf
-00013440: 6163 652e 0a0a 2020 2020 3a70 6172 616d  ace...    :param
-00013450: 2069 645f 7369 6d75 6c61 7469 6f6e 3a20   id_simulation: 
-00013460: 5468 6520 6964 206f 6620 7468 6520 7369  The id of the si
-00013470: 6d75 6c61 7469 6f6e 2e0a 2020 2020 3a70  mulation..    :p
-00013480: 6172 616d 2070 726f 6265 5f69 643a 2054  aram probe_id: T
-00013490: 6865 2069 6420 6f66 2074 6865 2070 726f  he id of the pro
-000134a0: 6265 0a0a 2020 2020 3a74 7970 6520 6964  be..    :type id
-000134b0: 5f73 696d 756c 6174 696f 6e3a 203a 636c  _simulation: :cl
-000134c0: 6173 733a 6069 6e74 602c 2065 7820 3a20  ass:`int`, ex : 
-000134d0: 310a 2020 2020 3a74 7970 6520 7072 6f62  1.    :type prob
-000134e0: 655f 6964 3a20 3a63 6c61 7373 3a60 696e  e_id: :class:`in
-000134f0: 7460 2c20 6578 203a 2031 0a0a 2020 2020  t`, ex : 1..    
-00013500: 2222 220a 0a20 2020 2072 6573 756c 7420  """..    result 
-00013510: 3d20 5f67 6574 2866 222f 7369 6d75 6c61  = _get(f"/simula
-00013520: 7469 6f6e 2f7b 6964 5f73 696d 756c 6174  tion/{id_simulat
-00013530: 696f 6e7d 2f70 726f 6265 2f7b 7072 6f62  ion}/probe/{prob
-00013540: 655f 6964 7d22 290a 0a20 2020 2069 6620  e_id}")..    if 
-00013550: 7265 7375 6c74 2e73 7461 7475 735f 636f  result.status_co
-00013560: 6465 2021 3d20 3230 303a 0a20 2020 2020  de != 200:.     
-00013570: 2020 205f 6861 6e64 6c65 5f65 7272 6f72     _handle_error
-00013580: 280a 2020 2020 2020 2020 2020 2020 7265  (.            re
-00013590: 7375 6c74 2c20 2243 616e 6e6f 7420 6163  sult, "Cannot ac
-000135a0: 7469 7661 7465 206e 6574 776f 726b 2074  tivate network t
-000135b0: 7261 6666 6963 2072 6564 6972 6563 7469  raffic redirecti
-000135c0: 6f6e 2066 726f 6d20 4954 2053 696d 756c  on from IT Simul
-000135d0: 6174 696f 6e20 4150 4922 0a20 2020 2020  ation API".     
-000135e0: 2020 2029 0a0a 0a64 6566 206e 6574 5f73     )...def net_s
-000135f0: 746f 705f 7072 6f62 6528 6964 5f73 696d  top_probe(id_sim
-00013600: 756c 6174 696f 6e3a 2069 6e74 2c20 7072  ulation: int, pr
-00013610: 6f62 655f 6964 3a20 696e 7429 202d 3e20  obe_id: int) -> 
-00013620: 4e6f 6e65 3a0a 2020 2020 2222 2253 746f  None:.    """Sto
-00013630: 7020 7265 6469 7265 6374 696f 6e20 6f66  p redirection of
-00013640: 206e 6574 776f 726b 2074 7261 6666 6963   network traffic
-00013650: 2074 6f20 7468 6520 7072 6f62 6520 696e   to the probe in
-00013660: 7465 7266 6163 652e 0a0a 2020 2020 3a70  terface...    :p
-00013670: 6172 616d 2069 645f 7369 6d75 6c61 7469  aram id_simulati
-00013680: 6f6e 3a20 5468 6520 6964 206f 6620 7468  on: The id of th
-00013690: 6520 7369 6d75 6c61 7469 6f6e 2e0a 2020  e simulation..  
-000136a0: 2020 3a70 6172 616d 2070 726f 6265 5f69    :param probe_i
-000136b0: 643a 2054 6865 2069 6420 6f66 2074 6865  d: The id of the
-000136c0: 2070 726f 6265 0a0a 2020 2020 3a74 7970   probe..    :typ
-000136d0: 6520 6964 5f73 696d 756c 6174 696f 6e3a  e id_simulation:
-000136e0: 203a 636c 6173 733a 6069 6e74 602c 2065   :class:`int`, e
-000136f0: 7820 3a20 310a 2020 2020 3a74 7970 6520  x : 1.    :type 
-00013700: 7072 6f62 655f 6964 3a20 3a63 6c61 7373  probe_id: :class
-00013710: 3a60 696e 7460 2c20 6578 203a 2031 0a0a  :`int`, ex : 1..
-00013720: 2020 2020 2222 220a 0a20 2020 2072 6573      """..    res
-00013730: 756c 7420 3d20 5f67 6574 2866 222f 7369  ult = _get(f"/si
-00013740: 6d75 6c61 7469 6f6e 2f7b 6964 5f73 696d  mulation/{id_sim
-00013750: 756c 6174 696f 6e7d 2f73 746f 705f 7072  ulation}/stop_pr
-00013760: 6f62 652f 7b70 726f 6265 5f69 647d 2229  obe/{probe_id}")
-00013770: 0a0a 2020 2020 6966 2072 6573 756c 742e  ..    if result.
-00013780: 7374 6174 7573 5f63 6f64 6520 213d 2032  status_code != 2
-00013790: 3030 3a0a 2020 2020 2020 2020 5f68 616e  00:.        _han
-000137a0: 646c 655f 6572 726f 7228 0a20 2020 2020  dle_error(.     
-000137b0: 2020 2020 2020 2072 6573 756c 742c 2022         result, "
-000137c0: 4361 6e6e 6f74 2073 746f 7020 6e65 7477  Cannot stop netw
-000137d0: 6f72 6b20 7472 6166 6669 6320 7265 6469  ork traffic redi
-000137e0: 7265 6374 696f 6e20 6672 6f6d 2049 5420  rection from IT 
-000137f0: 5369 6d75 6c61 7469 6f6e 2041 5049 220a  Simulation API".
-00013800: 2020 2020 2020 2020 290a 0a0a 6465 6620          )...def 
-00013810: 6665 7463 685f 6c69 7374 5f70 726f 6265  fetch_list_probe
-00013820: 7328 6964 5f73 696d 756c 6174 696f 6e3a  s(id_simulation:
-00013830: 2069 6e74 2920 2d3e 2044 6963 743a 0a20   int) -> Dict:. 
-00013840: 2020 2022 2222 5265 7475 726e 2074 6865     """Return the
-00013850: 206c 6973 7420 6f66 2070 726f 6265 7320   list of probes 
-00013860: 7769 7468 2074 6865 6972 2064 6174 610a  with their data.
+00004ac0: 7469 6f6e 2e0a 0a20 2020 203a 7061 7261  tion...    :para
+00004ad0: 6d20 746f 706f 6c6f 6779 5f63 6f6e 7465  m topology_conte
+00004ae0: 6e74 3a20 4120 6469 6374 2063 6f6e 7461  nt: A dict conta
+00004af0: 696e 696e 6720 7468 6520 6e6f 6465 7320  ining the nodes 
+00004b00: 616e 6420 6e65 7477 6f72 6b20 746f 706f  and network topo
+00004b10: 6c6f 6779 2074 6f20 6372 6561 7465 2e0a  logy to create..
+00004b20: 2020 2020 3a70 6172 616d 2074 6f70 6f6c      :param topol
+00004b30: 6f67 795f 7265 736f 7572 6365 735f 7061  ogy_resources_pa
+00004b40: 7468 733a 2054 6865 2070 6174 6820 746f  ths: The path to
+00004b50: 2072 6573 6f75 7263 6573 2074 6861 7420   resources that 
+00004b60: 7769 6c6c 2062 6520 7075 7368 6564 2069  will be pushed i
+00004b70: 6e74 6f20 636f 6d70 6174 6962 6c65 206e  nto compatible n
+00004b80: 6f64 650a 2020 2020 2222 220a 0a20 2020  ode.    """..   
+00004b90: 2069 6620 226e 616d 6522 206e 6f74 2069   if "name" not i
+00004ba0: 6e20 746f 706f 6c6f 6779 5f63 6f6e 7465  n topology_conte
+00004bb0: 6e74 3a0a 2020 2020 2020 2020 6e61 6d65  nt:.        name
+00004bc0: 203d 2022 546f 706f 6c6f 6779 220a 2020   = "Topology".  
+00004bd0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00004be0: 6e61 6d65 203d 2074 6f70 6f6c 6f67 795f  name = topology_
+00004bf0: 636f 6e74 656e 745b 226e 616d 6522 5d0a  content["name"].
+00004c00: 0a20 2020 2069 6620 226e 6f64 6573 2220  .    if "nodes" 
+00004c10: 6e6f 7420 696e 2074 6f70 6f6c 6f67 795f  not in topology_
+00004c20: 636f 6e74 656e 743a 0a20 2020 2020 2020  content:.       
+00004c30: 2072 6169 7365 2045 7863 6570 7469 6f6e   raise Exception
+00004c40: 280a 2020 2020 2020 2020 2020 2020 2254  (.            "T
+00004c50: 6865 7265 2073 686f 756c 6420 6265 2061  here should be a
+00004c60: 2027 6e6f 6465 7327 2073 7472 7563 7475   'nodes' structu
+00004c70: 7265 2069 6e20 7468 6520 5941 4d4c 2063  re in the YAML c
+00004c80: 6f6e 6669 6775 7261 7469 6f6e 2066 696c  onfiguration fil
+00004c90: 6522 0a20 2020 2020 2020 2029 0a0a 2020  e".        )..  
+00004ca0: 2020 6966 2022 6c69 6e6b 7322 206e 6f74    if "links" not
+00004cb0: 2069 6e20 746f 706f 6c6f 6779 5f63 6f6e   in topology_con
+00004cc0: 7465 6e74 3a0a 2020 2020 2020 2020 7261  tent:.        ra
+00004cd0: 6973 6520 4578 6365 7074 696f 6e28 0a20  ise Exception(. 
+00004ce0: 2020 2020 2020 2020 2020 2022 5468 6572             "Ther
+00004cf0: 6520 7368 6f75 6c64 2062 6520 6120 276c  e should be a 'l
+00004d00: 696e 6b73 2720 7374 7275 6374 7572 6520  inks' structure 
+00004d10: 696e 2074 6865 2059 414d 4c20 636f 6e66  in the YAML conf
+00004d20: 6967 7572 6174 696f 6e20 6669 6c65 220a  iguration file".
+00004d30: 2020 2020 2020 2020 290a 0a20 2020 2072          )..    r
+00004d40: 6571 7569 7265 6420 3d20 5b22 7377 6974  equired = ["swit
+00004d50: 6368 222c 2022 6e6f 6465 222c 2022 7061  ch", "node", "pa
+00004d60: 7261 6d73 225d 0a20 2020 2066 6f72 206c  rams"].    for l
+00004d70: 696e 6b20 696e 2074 6f70 6f6c 6f67 795f  ink in topology_
+00004d80: 636f 6e74 656e 745b 226c 696e 6b73 225d  content["links"]
+00004d90: 3a0a 2020 2020 2020 2020 666f 7220 7265  :.        for re
+00004da0: 7120 696e 2072 6571 7569 7265 643a 0a20  q in required:. 
+00004db0: 2020 2020 2020 2020 2020 2069 6620 7265             if re
+00004dc0: 7120 6e6f 7420 696e 206c 696e 6b3a 0a20  q not in link:. 
+00004dd0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00004de0: 6169 7365 2045 7863 6570 7469 6f6e 280a  aise Exception(.
+00004df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e00: 2020 2020 6622 5468 6572 6520 7368 6f75      f"There shou
+00004e10: 6c64 2062 6520 6120 277b 7265 717d 2720  ld be a '{req}' 
+00004e20: 7061 7261 6d65 7465 7220 666f 7220 6576  parameter for ev
+00004e30: 6572 7920 6974 656d 206f 6620 276c 696e  ery item of 'lin
+00004e40: 6b73 2720 696e 2074 6865 2059 414d 4c20  ks' in the YAML 
+00004e50: 636f 6e66 6967 7572 6174 696f 6e20 6669  configuration fi
+00004e60: 6c65 220a 2020 2020 2020 2020 2020 2020  le".            
+00004e70: 2020 2020 290a 0a20 2020 205f 7369 6d75      )..    _simu
+00004e80: 5f63 7265 6174 655f 6164 645f 696d 706c  _create_add_impl
+00004e90: 6963 6974 5f74 6f70 6f5f 7061 7261 6d65  icit_topo_parame
+00004ea0: 7465 7273 2874 6f70 6f6c 6f67 795f 636f  ters(topology_co
+00004eb0: 6e74 656e 7429 0a0a 2020 2020 7369 6d75  ntent)..    simu
+00004ec0: 6c61 7469 6f6e 5f64 6963 7420 3d20 7b22  lation_dict = {"
+00004ed0: 6e61 6d65 223a 206e 616d 652c 2022 6e65  name": name, "ne
+00004ee0: 7477 6f72 6b22 3a20 746f 706f 6c6f 6779  twork": topology
+00004ef0: 5f63 6f6e 7465 6e74 2c20 2272 6573 6f75  _content, "resou
+00004f00: 7263 6573 5f70 6174 6873 223a 205b 5d7d  rces_paths": []}
+00004f10: 0a0a 2020 2020 2320 4e6f 726d 616c 697a  ..    # Normaliz
+00004f20: 6520 7468 6520 7265 736f 7572 6365 7320  e the resources 
+00004f30: 7061 7468 730a 2020 2020 746f 706f 6c6f  paths.    topolo
+00004f40: 6779 5f72 6573 6f75 7263 6573 5f70 6174  gy_resources_pat
+00004f50: 6873 203d 205f 6e6f 726d 616c 697a 655f  hs = _normalize_
+00004f60: 7369 6d75 6c61 7469 6f6e 5f72 6573 6f75  simulation_resou
+00004f70: 7263 655f 7061 7468 7328 0a20 2020 2020  rce_paths(.     
+00004f80: 2020 2074 6f70 6f6c 6f67 795f 7265 736f     topology_reso
+00004f90: 7572 6365 735f 7061 7468 730a 2020 2020  urces_paths.    
+00004fa0: 290a 0a20 2020 2023 2056 6572 6966 7920  )..    # Verify 
+00004fb0: 7468 6174 2077 6520 646f 206e 6f74 2068  that we do not h
+00004fc0: 6176 6520 7468 6520 7361 6d65 2072 6573  ave the same res
+00004fd0: 6f75 7263 6573 2070 6174 6820 696e 2074  ources path in t
+00004fe0: 6865 206c 6973 740a 2020 2020 6966 206c  he list.    if l
+00004ff0: 656e 2873 6574 2874 6f70 6f6c 6f67 795f  en(set(topology_
+00005000: 7265 736f 7572 6365 735f 7061 7468 7329  resources_paths)
+00005010: 2920 213d 206c 656e 2874 6f70 6f6c 6f67  ) != len(topolog
+00005020: 795f 7265 736f 7572 6365 735f 7061 7468  y_resources_path
+00005030: 7329 3a0a 2020 2020 2020 2020 7261 6973  s):.        rais
+00005040: 6520 4578 6365 7074 696f 6e28 2249 6465  e Exception("Ide
+00005050: 6e74 6963 616c 2072 6573 6f75 7263 6573  ntical resources
+00005060: 2070 6174 6873 2068 6176 6520 6265 656e   paths have been
+00005070: 2067 6976 656e 2229 0a0a 2020 2020 666f   given")..    fo
+00005080: 7220 7265 736f 7572 6365 2069 6e20 746f  r resource in to
+00005090: 706f 6c6f 6779 5f72 6573 6f75 7263 6573  pology_resources
+000050a0: 5f70 6174 6873 3a0a 2020 2020 2020 2020  _paths:.        
+000050b0: 2320 5661 6c69 6461 7465 2072 6573 6f75  # Validate resou
+000050c0: 7263 6573 2070 6174 680a 2020 2020 2020  rces path.      
+000050d0: 2020 5f5f 7661 6c69 6461 7465 5f72 6573    __validate_res
+000050e0: 6f75 7263 6573 5f70 6174 6828 7265 736f  ources_path(reso
+000050f0: 7572 6365 2920 2023 2072 6169 7365 2061  urce)  # raise a
+00005100: 6e20 6578 6365 7074 696f 6e20 6966 2069  n exception if i
+00005110: 6e76 616c 6964 0a20 2020 2020 2020 2023  nvalid.        #
+00005120: 2074 616b 6520 7468 6520 6162 736f 6c75   take the absolu
+00005130: 7465 2070 6174 680a 2020 2020 2020 2020  te path.        
+00005140: 7369 6d75 6c61 7469 6f6e 5f64 6963 745b  simulation_dict[
+00005150: 2272 6573 6f75 7263 6573 5f70 6174 6873  "resources_paths
+00005160: 225d 2e61 7070 656e 6428 6f73 2e70 6174  "].append(os.pat
+00005170: 682e 6162 7370 6174 6828 7265 736f 7572  h.abspath(resour
+00005180: 6365 2929 0a0a 2020 2020 7265 7475 726e  ce))..    return
+00005190: 2073 696d 756c 6174 696f 6e5f 6469 6374   simulation_dict
+000051a0: 0a0a 0a23 202d 2d2d 2d2d 2d2d 2d2d 2d2d  ...# -----------
+000051b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000051c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000051d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000051e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d20  --------------- 
+000051f0: 230a 2320 4150 4920 6865 6c70 6572 730a  #.# API helpers.
+00005200: 2320 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  # --------------
+00005210: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005220: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005230: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005240: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2023 0a0a  ------------ #..
+00005250: 0a23 2323 0a23 2053 696d 756c 6174 696f  .###.# Simulatio
+00005260: 6e20 6865 6c70 6572 730a 2323 230a 0a0a  n helpers.###...
+00005270: 6465 6620 6372 6561 7465 5f73 696d 756c  def create_simul
+00005280: 6174 696f 6e28 0a20 2020 2074 6f70 6f6c  ation(.    topol
+00005290: 6f67 795f 636f 6e74 656e 743a 2044 6963  ogy_content: Dic
+000052a0: 745b 7374 722c 2041 6e79 5d20 3d20 4e6f  t[str, Any] = No
+000052b0: 6e65 2c0a 2020 2020 746f 706f 6c6f 6779  ne,.    topology
+000052c0: 5f72 6573 6f75 7263 6573 5f70 6174 6873  _resources_paths
+000052d0: 3a20 4f70 7469 6f6e 616c 5b4c 6973 745b  : Optional[List[
+000052e0: 5061 7468 5d5d 203d 204e 6f6e 652c 0a20  Path]] = None,. 
+000052f0: 2020 2061 6c6c 6f63 6174 696f 6e5f 7374     allocation_st
+00005300: 7261 7465 6779 3a20 4f70 7469 6f6e 616c  rategy: Optional
+00005310: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2920  [str] = None,.) 
+00005320: 2d3e 2054 7570 6c65 5b69 6e74 2c20 4c69  -> Tuple[int, Li
+00005330: 7374 5b73 7472 5d5d 3a0a 2020 2020 2222  st[str]]:.    ""
+00005340: 2243 7265 6174 6520 6120 6e65 7720 7369  "Create a new si
+00005350: 6d75 6c61 7469 6f6e 206d 6f64 656c 2069  mulation model i
+00005360: 6e20 6461 7461 6261 7365 2062 6173 6564  n database based
+00005370: 206f 6e20 7468 6520 7072 6f76 6964 6564   on the provided
+00005380: 2074 6f70 6f6c 6f67 792c 2061 6c6f 6e67   topology, along
+00005390: 2077 6974 6820 6f70 7469 6f6e 616c 2072   with optional r
+000053a0: 6573 6f75 7263 6520 6669 6c65 732e 0a0a  esource files...
+000053b0: 2020 2020 3a72 6574 7572 6e3a 2041 2074      :return: A t
+000053c0: 7570 6c65 2063 6f6e 7461 696e 696e 6720  uple containing 
+000053d0: 7468 6520 4944 206f 6620 7468 6520 6372  the ID of the cr
+000053e0: 6561 7465 6420 7369 6d75 6c61 7469 6f6e  eated simulation
+000053f0: 2c20 616e 6420 7468 6520 6e65 7720 6e6f  , and the new no
+00005400: 6465 7320 6f66 2074 6865 2073 696d 756c  des of the simul
+00005410: 6174 696f 6e2e 0a0a 2020 2020 3a70 6172  ation...    :par
+00005420: 616d 2074 6f70 6f6c 6f67 795f 636f 6e74  am topology_cont
+00005430: 656e 743a 2041 2064 6963 7420 636f 6e74  ent: A dict cont
+00005440: 6169 6e69 6e67 2074 6865 206e 6f64 6573  aining the nodes
+00005450: 2061 6e64 206e 6574 776f 726b 2074 6f70   and network top
+00005460: 6f6c 6f67 7920 746f 2063 7265 6174 652e  ology to create.
+00005470: 0a20 2020 203a 7061 7261 6d20 746f 706f  .    :param topo
+00005480: 6c6f 6779 5f72 6573 6f75 7263 6573 5f70  logy_resources_p
+00005490: 6174 6873 3a20 5468 6520 7061 7468 2074  aths: The path t
+000054a0: 6f20 7265 736f 7572 6365 7320 7468 6174  o resources that
+000054b0: 2077 696c 6c20 6265 2070 7573 6865 6420   will be pushed 
+000054c0: 696e 746f 2063 6f6d 7061 7469 626c 6520  into compatible 
+000054d0: 6e6f 6465 732e 0a20 2020 203a 7061 7261  nodes..    :para
+000054e0: 6d20 616c 6c6f 6361 7469 6f6e 5f73 7472  m allocation_str
+000054f0: 6174 6567 793a 204e 616d 6520 6f66 2074  ategy: Name of t
+00005500: 6865 2061 6c6c 6f63 6174 696f 6e20 7374  he allocation st
+00005510: 7261 7465 6779 2074 6f20 7573 6520 746f  rategy to use to
+00005520: 2061 6c6c 6f63 6174 6520 6e6f 6465 7320   allocate nodes 
+00005530: 746f 2063 6f6d 7075 7465 2073 6572 7665  to compute serve
+00005540: 7273 2e0a 0a20 2020 2022 2222 0a20 2020  rs...    """.   
+00005550: 2073 696d 756c 6174 696f 6e5f 6469 6374   simulation_dict
+00005560: 203d 205f 6e6f 726d 616c 697a 655f 7369   = _normalize_si
+00005570: 6d75 6c61 7469 6f6e 5f72 6573 6f75 7263  mulation_resourc
+00005580: 6573 280a 2020 2020 2020 2020 746f 706f  es(.        topo
+00005590: 6c6f 6779 5f63 6f6e 7465 6e74 3d74 6f70  logy_content=top
+000055a0: 6f6c 6f67 795f 636f 6e74 656e 742c 0a20  ology_content,. 
+000055b0: 2020 2020 2020 2074 6f70 6f6c 6f67 795f         topology_
+000055c0: 7265 736f 7572 6365 735f 7061 7468 733d  resources_paths=
+000055d0: 746f 706f 6c6f 6779 5f72 6573 6f75 7263  topology_resourc
+000055e0: 6573 5f70 6174 6873 2c0a 2020 2020 290a  es_paths,.    ).
+000055f0: 0a20 2020 2072 6574 7572 6e20 5f63 7265  .    return _cre
+00005600: 6174 655f 6f72 5f65 7874 656e 645f 7369  ate_or_extend_si
+00005610: 6d75 6c61 7469 6f6e 280a 2020 2020 2020  mulation(.      
+00005620: 2020 7369 6d75 6c61 7469 6f6e 5f64 6963    simulation_dic
+00005630: 743d 7369 6d75 6c61 7469 6f6e 5f64 6963  t=simulation_dic
+00005640: 742c 2061 6c6c 6f63 6174 696f 6e5f 7374  t, allocation_st
+00005650: 7261 7465 6779 3d61 6c6c 6f63 6174 696f  rategy=allocatio
+00005660: 6e5f 7374 7261 7465 6779 0a20 2020 2029  n_strategy.    )
+00005670: 0a0a 0a64 6566 2065 7874 656e 645f 7369  ...def extend_si
+00005680: 6d75 6c61 7469 6f6e 280a 2020 2020 746f  mulation(.    to
+00005690: 706f 6c6f 6779 5f63 6f6e 7465 6e74 3a20  pology_content: 
+000056a0: 4469 6374 5b73 7472 2c20 416e 795d 203d  Dict[str, Any] =
+000056b0: 204e 6f6e 652c 0a20 2020 2074 6f70 6f6c   None,.    topol
+000056c0: 6f67 795f 7265 736f 7572 6365 735f 7061  ogy_resources_pa
+000056d0: 7468 733a 204f 7074 696f 6e61 6c5b 4c69  ths: Optional[Li
+000056e0: 7374 5b50 6174 685d 5d20 3d20 4e6f 6e65  st[Path]] = None
+000056f0: 2c0a 2020 2020 616c 6c6f 6361 7469 6f6e  ,.    allocation
+00005700: 5f73 7472 6174 6567 793a 204f 7074 696f  _strategy: Optio
+00005710: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
+00005720: 0a20 2020 2069 645f 7369 6d75 6c61 7469  .    id_simulati
+00005730: 6f6e 3a20 696e 7420 3d20 4e6f 6e65 2c0a  on: int = None,.
+00005740: 2920 2d3e 2054 7570 6c65 5b69 6e74 2c20  ) -> Tuple[int, 
+00005750: 4c69 7374 5b73 7472 5d5d 3a0a 2020 2020  List[str]]:.    
+00005760: 2222 2245 7874 656e 6420 616e 2065 7869  """Extend an exi
+00005770: 7374 696e 6720 7369 6d75 6c61 7469 6f6e  sting simulation
+00005780: 206d 6f64 656c 2069 6e20 6461 7461 6261   model in databa
+00005790: 7365 2062 6173 6564 206f 6e20 7468 6520  se based on the 
+000057a0: 7072 6f76 6964 6564 2074 6f70 6f6c 6f67  provided topolog
+000057b0: 792c 2061 6c6f 6e67 2077 6974 6820 6f70  y, along with op
+000057c0: 7469 6f6e 616c 2072 6573 6f75 7263 6520  tional resource 
+000057d0: 6669 6c65 732e 0a0a 2020 2020 3a72 6574  files...    :ret
+000057e0: 7572 6e3a 2041 2074 7570 6c65 2063 6f6e  urn: A tuple con
+000057f0: 7461 696e 696e 6720 7468 6520 4944 206f  taining the ID o
+00005800: 6620 7468 6520 6372 6561 7465 6420 7369  f the created si
+00005810: 6d75 6c61 7469 6f6e 2c20 616e 6420 7468  mulation, and th
+00005820: 6520 6e65 7720 6e6f 6465 7320 6f66 2074  e new nodes of t
+00005830: 6865 2073 696d 756c 6174 696f 6e2e 0a0a  he simulation...
+00005840: 2020 2020 3a70 6172 616d 2074 6f70 6f6c      :param topol
+00005850: 6f67 795f 636f 6e74 656e 743a 2041 2064  ogy_content: A d
+00005860: 6963 7420 636f 6e74 6169 6e69 6e67 2074  ict containing t
+00005870: 6865 206e 6f64 6573 2061 6e64 206e 6574  he nodes and net
+00005880: 776f 726b 2074 6f70 6f6c 6f67 7920 746f  work topology to
+00005890: 2063 7265 6174 652e 0a20 2020 203a 7061   create..    :pa
+000058a0: 7261 6d20 746f 706f 6c6f 6779 5f72 6573  ram topology_res
+000058b0: 6f75 7263 6573 5f70 6174 6873 3a20 5468  ources_paths: Th
+000058c0: 6520 7061 7468 2074 6f20 7265 736f 7572  e path to resour
+000058d0: 6365 7320 7468 6174 2077 696c 6c20 6265  ces that will be
+000058e0: 2070 7573 6865 6420 696e 746f 2063 6f6d   pushed into com
+000058f0: 7061 7469 626c 6520 6e6f 6465 732e 0a20  patible nodes.. 
+00005900: 2020 203a 7061 7261 6d20 616c 6c6f 6361     :param alloca
+00005910: 7469 6f6e 5f73 7472 6174 6567 793a 204e  tion_strategy: N
+00005920: 616d 6520 6f66 2074 6865 2061 6c6c 6f63  ame of the alloc
+00005930: 6174 696f 6e20 7374 7261 7465 6779 2074  ation strategy t
+00005940: 6f20 7573 6520 746f 2061 6c6c 6f63 6174  o use to allocat
+00005950: 6520 6e6f 6465 7320 746f 2063 6f6d 7075  e nodes to compu
+00005960: 7465 2073 6572 7665 7273 2e0a 2020 2020  te servers..    
+00005970: 3a70 6172 616d 2069 645f 7369 6d75 6c61  :param id_simula
+00005980: 7469 6f6e 3a20 5468 6520 7369 6d75 6c61  tion: The simula
+00005990: 7469 6f6e 2049 442c 2077 6865 6e20 6578  tion ID, when ex
+000059a0: 7465 6e64 696e 6720 616e 2065 7869 7374  tending an exist
+000059b0: 696e 6720 7369 6d75 6c61 7469 6f6e 2077  ing simulation w
+000059c0: 6974 6820 6e65 7720 6e6f 6465 7320 616e  ith new nodes an
+000059d0: 6420 6c69 6e6b 732e 0a0a 2020 2020 2222  d links...    ""
+000059e0: 220a 0a20 2020 2073 696d 756c 6174 696f  "..    simulatio
+000059f0: 6e5f 6469 6374 203d 205f 6e6f 726d 616c  n_dict = _normal
+00005a00: 697a 655f 7369 6d75 6c61 7469 6f6e 5f72  ize_simulation_r
+00005a10: 6573 6f75 7263 6573 280a 2020 2020 2020  esources(.      
+00005a20: 2020 746f 706f 6c6f 6779 5f63 6f6e 7465    topology_conte
+00005a30: 6e74 3d74 6f70 6f6c 6f67 795f 636f 6e74  nt=topology_cont
+00005a40: 656e 742c 0a20 2020 2020 2020 2074 6f70  ent,.        top
+00005a50: 6f6c 6f67 795f 7265 736f 7572 6365 735f  ology_resources_
+00005a60: 7061 7468 733d 746f 706f 6c6f 6779 5f72  paths=topology_r
+00005a70: 6573 6f75 7263 6573 5f70 6174 6873 2c0a  esources_paths,.
+00005a80: 2020 2020 290a 0a20 2020 2072 6574 7572      )..    retur
+00005a90: 6e20 5f63 7265 6174 655f 6f72 5f65 7874  n _create_or_ext
+00005aa0: 656e 645f 7369 6d75 6c61 7469 6f6e 280a  end_simulation(.
+00005ab0: 2020 2020 2020 2020 7369 6d75 6c61 7469          simulati
+00005ac0: 6f6e 5f64 6963 743d 7369 6d75 6c61 7469  on_dict=simulati
+00005ad0: 6f6e 5f64 6963 742c 0a20 2020 2020 2020  on_dict,.       
+00005ae0: 2069 645f 7369 6d75 6c61 7469 6f6e 3d69   id_simulation=i
+00005af0: 645f 7369 6d75 6c61 7469 6f6e 2c0a 2020  d_simulation,.  
+00005b00: 2020 2020 2020 616c 6c6f 6361 7469 6f6e        allocation
+00005b10: 5f73 7472 6174 6567 793d 616c 6c6f 6361  _strategy=alloca
+00005b20: 7469 6f6e 5f73 7472 6174 6567 792c 0a20  tion_strategy,. 
+00005b30: 2020 2029 0a0a 0a64 6566 2063 7265 6174     )...def creat
+00005b40: 655f 7369 6d75 6c61 7469 6f6e 5f66 726f  e_simulation_fro
+00005b50: 6d5f 746f 706f 6c6f 6779 280a 2020 2020  m_topology(.    
+00005b60: 746f 706f 6c6f 6779 5f66 696c 653a 2073  topology_file: s
+00005b70: 7472 203d 204e 6f6e 652c 0a20 2020 2074  tr = None,.    t
+00005b80: 6f70 6f6c 6f67 795f 7265 736f 7572 6365  opology_resource
+00005b90: 735f 7061 7468 733a 204f 7074 696f 6e61  s_paths: Optiona
+00005ba0: 6c5b 4c69 7374 5b50 6174 685d 5d20 3d20  l[List[Path]] = 
+00005bb0: 4e6f 6e65 2c0a 2020 2020 616c 6c6f 6361  None,.    alloca
+00005bc0: 7469 6f6e 5f73 7472 6174 6567 793a 204f  tion_strategy: O
+00005bd0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+00005be0: 6f6e 652c 0a29 202d 3e20 5475 706c 655b  one,.) -> Tuple[
+00005bf0: 696e 742c 204c 6973 745b 7374 725d 5d3a  int, List[str]]:
+00005c00: 0a20 2020 2022 2222 4372 6561 7465 2061  .    """Create a
+00005c10: 206e 6577 2073 696d 756c 6174 696f 6e20   new simulation 
+00005c20: 6d6f 6465 6c20 696e 2064 6174 6162 6173  model in databas
+00005c30: 6520 6261 7365 6420 6f6e 2074 6865 2070  e based on the p
+00005c40: 726f 7669 6465 6420 746f 706f 6c6f 6779  rovided topology
+00005c50: 2066 696c 652c 2061 6c6f 6e67 2077 6974   file, along wit
+00005c60: 6820 6f70 7469 6f6e 616c 2072 6573 6f75  h optional resou
+00005c70: 7263 6520 6669 6c65 732e 0a0a 2020 2020  rce files...    
+00005c80: 3a72 6574 7572 6e3a 2041 2074 7570 6c65  :return: A tuple
+00005c90: 2063 6f6e 7461 696e 696e 6720 7468 6520   containing the 
+00005ca0: 4944 206f 6620 7468 6520 6372 6561 7465  ID of the create
+00005cb0: 6420 7369 6d75 6c61 7469 6f6e 2c20 616e  d simulation, an
+00005cc0: 6420 7468 6520 6e65 7720 6e6f 6465 7320  d the new nodes 
+00005cd0: 6f66 2074 6865 2073 696d 756c 6174 696f  of the simulatio
+00005ce0: 6e2e 0a0a 2020 2020 3a70 6172 616d 2074  n...    :param t
+00005cf0: 6f70 6f6c 6f67 795f 6669 6c65 3a20 5468  opology_file: Th
+00005d00: 6520 7061 7468 2074 6f20 6120 746f 706f  e path to a topo
+00005d10: 6c6f 6779 2066 696c 6520 636f 6e74 6169  logy file contai
+00005d20: 6e69 6e67 2074 6865 206e 6f64 6573 2061  ning the nodes a
+00005d30: 6e64 206e 6574 776f 726b 2074 6f70 6f6c  nd network topol
+00005d40: 6f67 7920 746f 2063 7265 6174 652e 0a20  ogy to create.. 
+00005d50: 2020 203a 7061 7261 6d20 746f 706f 6c6f     :param topolo
+00005d60: 6779 5f72 6573 6f75 7263 6573 5f70 6174  gy_resources_pat
+00005d70: 6873 3a20 5468 6520 7061 7468 2074 6f20  hs: The path to 
+00005d80: 7265 736f 7572 6365 7320 7468 6174 2077  resources that w
+00005d90: 696c 6c20 6265 2070 7573 6865 6420 696e  ill be pushed in
+00005da0: 746f 2063 6f6d 7061 7469 626c 6520 6e6f  to compatible no
+00005db0: 6465 732e 0a20 2020 203a 7061 7261 6d20  des..    :param 
+00005dc0: 616c 6c6f 6361 7469 6f6e 5f73 7472 6174  allocation_strat
+00005dd0: 6567 793a 204e 616d 6520 6f66 2074 6865  egy: Name of the
+00005de0: 2061 6c6c 6f63 6174 696f 6e20 7374 7261   allocation stra
+00005df0: 7465 6779 2074 6f20 7573 6520 746f 2061  tegy to use to a
+00005e00: 6c6c 6f63 6174 6520 6e6f 6465 7320 746f  llocate nodes to
+00005e10: 2063 6f6d 7075 7465 2073 6572 7665 7273   compute servers
+00005e20: 2e0a 0a20 2020 203e 3e3e 2066 726f 6d20  ...    >>> from 
+00005e30: 6372 5f61 7069 5f63 6c69 656e 7420 696d  cr_api_client im
+00005e40: 706f 7274 2063 6f72 655f 6170 690a 2020  port core_api.  
+00005e50: 2020 3e3e 3e20 636f 7265 5f61 7069 2e72    >>> core_api.r
+00005e60: 6573 6574 2829 0a20 2020 2027 436f 6d70  eset().    'Comp
+00005e70: 7574 6520 696e 6672 6173 7472 7563 7475  ute infrastructu
+00005e80: 7265 2073 7563 6365 7373 6675 6c6c 7920  re successfully 
+00005e90: 7265 7365 7427 0a20 2020 203e 3e3e 2063  reset'.    >>> c
+00005ea0: 6f72 655f 6170 692e 6372 6561 7465 5f73  ore_api.create_s
+00005eb0: 696d 756c 6174 696f 6e5f 6672 6f6d 5f74  imulation_from_t
+00005ec0: 6f70 6f6c 6f67 7928 2264 6174 612f 746f  opology("data/to
+00005ed0: 706f 6c6f 6769 6573 2f74 6f70 6f6c 6f67  pologies/topolog
+00005ee0: 792d 312d 636c 6965 6e74 2e79 616d 6c22  y-1-client.yaml"
+00005ef0: 290a 2020 2020 2831 2c20 5b27 434c 4945  ).    (1, ['CLIE
+00005f00: 4e54 3127 2c20 2752 6f75 7465 7231 272c  NT1', 'Router1',
+00005f10: 2027 5377 6974 6368 3127 5d29 0a0a 2020   'Switch1'])..  
+00005f20: 2020 2222 220a 0a20 2020 2069 6620 746f    """..    if to
+00005f30: 706f 6c6f 6779 5f72 6573 6f75 7263 6573  pology_resources
+00005f40: 5f70 6174 6873 2069 7320 4e6f 6e65 3a0a  _paths is None:.
+00005f50: 2020 2020 2020 2020 746f 706f 6c6f 6779          topology
+00005f60: 5f72 6573 6f75 7263 6573 5f70 6174 6873  _resources_paths
+00005f70: 203d 205b 5d0a 0a20 2020 2023 2043 7265   = []..    # Cre
+00005f80: 6174 6520 6120 6e65 7720 7369 6d75 6c61  ate a new simula
+00005f90: 7469 6f6e 206d 6f64 656c 2069 6e20 6461  tion model in da
+00005fa0: 7461 6261 7365 2062 6173 6564 206f 6e20  tabase based on 
+00005fb0: 7468 6520 7072 6f76 6964 6564 2074 6f70  the provided top
+00005fc0: 6f6c 6f67 7920 6669 6c65 2070 6174 682e  ology file path.
+00005fd0: 2222 220a 2020 2020 6966 2074 6f70 6f6c  """.    if topol
+00005fe0: 6f67 795f 6669 6c65 2069 7320 4e6f 6e65  ogy_file is None
+00005ff0: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
+00006000: 4578 6365 7074 696f 6e28 2241 6e20 746f  Exception("An to
+00006010: 706f 6c6f 6779 2066 696c 6520 6973 2072  pology file is r
+00006020: 6571 7569 7265 6422 290a 0a20 2020 2023  equired")..    #
+00006030: 2056 616c 6964 6174 6520 5941 4d4c 2063   Validate YAML c
+00006040: 6f6e 6669 6775 7261 7469 6f6e 2066 696c  onfiguration fil
+00006050: 650a 2020 2020 5f76 616c 6964 6174 655f  e.    _validate_
+00006060: 7961 6d6c 5f74 6f70 6f6c 6f67 795f 6669  yaml_topology_fi
+00006070: 6c65 2874 6f70 6f6c 6f67 795f 6669 6c65  le(topology_file
+00006080: 290a 0a20 2020 2023 204f 7065 6e20 616e  )..    # Open an
+00006090: 6420 7265 6164 2059 414d 4c20 636f 6e66  d read YAML conf
+000060a0: 6967 7572 6174 696f 6e20 6669 6c65 0a20  iguration file. 
+000060b0: 2020 2079 616d 6c5f 636f 6e74 656e 7420     yaml_content 
+000060c0: 3d20 5f72 6561 645f 7961 6d6c 5f74 6f70  = _read_yaml_top
+000060d0: 6f6c 6f67 795f 6669 6c65 2874 6f70 6f6c  ology_file(topol
+000060e0: 6f67 795f 6669 6c65 290a 0a20 2020 2023  ogy_file)..    #
+000060f0: 2050 6172 7365 2059 414d 4c20 636f 6e66   Parse YAML conf
+00006100: 6967 7572 6174 696f 6e0a 2020 2020 2320  iguration.    # 
+00006110: 5765 2075 7365 2072 7561 6d65 6c2e 7961  We use ruamel.ya
+00006120: 6d6c 2062 6563 6175 7365 2069 7420 6b65  ml because it ke
+00006130: 6570 7320 616e 6368 6f72 7320 616e 640a  eps anchors and.
+00006140: 2020 2020 2320 616c 6961 7365 7320 696e      # aliases in
+00006150: 206d 656d 6f72 792e 2049 7420 6973 2076   memory. It is v
+00006160: 6572 7920 636f 6e76 656e 6965 6e74 2077  ery convenient w
+00006170: 6865 6e20 7468 6520 7369 6d75 6c61 7469  hen the simulati
+00006180: 6f6e 0a20 2020 2023 2069 7320 7374 6f72  on.    # is stor
+00006190: 6564 2f66 6574 6368 6564 2028 7265 6665  ed/fetched (refe
+000061a0: 7265 6e63 6573 2061 7265 206b 6570 7421  rences are kept!
+000061b0: 290a 2020 2020 6c6f 6164 6572 203d 2059  ).    loader = Y
+000061c0: 414d 4c28 7479 703d 2272 7422 290a 2020  AML(typ="rt").  
+000061d0: 2020 746f 706f 6c6f 6779 5f63 6f6e 7465    topology_conte
+000061e0: 6e74 203d 206c 6f61 6465 722e 6c6f 6164  nt = loader.load
+000061f0: 2879 616d 6c5f 636f 6e74 656e 7429 0a0a  (yaml_content)..
+00006200: 2020 2020 5f76 616c 6964 6174 655f 746f      _validate_to
+00006210: 706f 6c6f 6779 5f72 6571 7569 7265 6d65  pology_requireme
+00006220: 6e74 7328 746f 706f 6c6f 6779 5f63 6f6e  nts(topology_con
+00006230: 7465 6e74 2c20 746f 706f 6c6f 6779 5f72  tent, topology_r
+00006240: 6573 6f75 7263 6573 5f70 6174 6873 290a  esources_paths).
+00006250: 0a20 2020 2023 2041 6464 2061 2064 6566  .    # Add a def
+00006260: 6175 6c74 2072 6573 6f75 7263 6573 2064  ault resources d
+00006270: 6972 6563 746f 7279 2069 6620 6974 2065  irectory if it e
+00006280: 7869 7374 732e 0a20 2020 2023 2049 6620  xists..    # If 
+00006290: 7468 6520 746f 706f 6c6f 6779 2069 7320  the topology is 
+000062a0: 2270 6174 682f 746f 2f74 6f70 6f2e 7961  "path/to/topo.ya
+000062b0: 6d6c 222c 2074 6865 2064 6566 6175 6c74  ml", the default
+000062c0: 2072 6573 6f75 7263 6573 2064 6972 6563   resources direc
+000062d0: 746f 7279 2069 7320 2270 6174 682f 746f  tory is "path/to
+000062e0: 2f72 6573 6f75 7263 6573 222e 0a20 2020  /resources"..   
+000062f0: 2074 6f70 6f6c 6f67 795f 7265 736f 7572   topology_resour
+00006300: 6365 735f 7061 7468 7320 3d20 5f6e 6f72  ces_paths = _nor
+00006310: 6d61 6c69 7a65 5f73 696d 756c 6174 696f  malize_simulatio
+00006320: 6e5f 7265 736f 7572 6365 5f70 6174 6873  n_resource_paths
+00006330: 280a 2020 2020 2020 2020 746f 706f 6c6f  (.        topolo
+00006340: 6779 5f72 6573 6f75 7263 6573 5f70 6174  gy_resources_pat
+00006350: 6873 0a20 2020 2029 0a20 2020 2064 6566  hs.    ).    def
+00006360: 6175 6c74 5f72 6573 6f75 7263 6573 5f70  ault_resources_p
+00006370: 6174 6820 3d20 6f73 2e70 6174 682e 6a6f  ath = os.path.jo
+00006380: 696e 286f 732e 7061 7468 2e64 6972 6e61  in(os.path.dirna
+00006390: 6d65 2874 6f70 6f6c 6f67 795f 6669 6c65  me(topology_file
+000063a0: 292c 2022 7265 736f 7572 6365 7322 290a  ), "resources").
+000063b0: 2020 2020 6465 6661 756c 745f 7265 736f      default_reso
+000063c0: 7572 6365 735f 7061 7468 203d 206f 732e  urces_path = os.
+000063d0: 7061 7468 2e6e 6f72 6d70 6174 6828 6465  path.normpath(de
+000063e0: 6661 756c 745f 7265 736f 7572 6365 735f  fault_resources_
+000063f0: 7061 7468 290a 2020 2020 6966 205f 5f76  path).    if __v
+00006400: 616c 6964 6174 655f 7265 736f 7572 6365  alidate_resource
+00006410: 735f 7061 7468 2864 6566 6175 6c74 5f72  s_path(default_r
+00006420: 6573 6f75 7263 6573 5f70 6174 682c 2046  esources_path, F
+00006430: 616c 7365 293a 0a20 2020 2020 2020 2069  alse):.        i
+00006440: 6620 6465 6661 756c 745f 7265 736f 7572  f default_resour
+00006450: 6365 735f 7061 7468 206e 6f74 2069 6e20  ces_path not in 
+00006460: 746f 706f 6c6f 6779 5f72 6573 6f75 7263  topology_resourc
+00006470: 6573 5f70 6174 6873 3a0a 2020 2020 2020  es_paths:.      
+00006480: 2020 2020 2020 746f 706f 6c6f 6779 5f72        topology_r
+00006490: 6573 6f75 7263 6573 5f70 6174 6873 2e61  esources_paths.a
+000064a0: 7070 656e 6428 6465 6661 756c 745f 7265  ppend(default_re
+000064b0: 736f 7572 6365 735f 7061 7468 290a 0a20  sources_path).. 
+000064c0: 2020 2072 6574 7572 6e20 6372 6561 7465     return create
+000064d0: 5f73 696d 756c 6174 696f 6e28 0a20 2020  _simulation(.   
+000064e0: 2020 2020 2074 6f70 6f6c 6f67 795f 636f       topology_co
+000064f0: 6e74 656e 743d 746f 706f 6c6f 6779 5f63  ntent=topology_c
+00006500: 6f6e 7465 6e74 2c0a 2020 2020 2020 2020  ontent,.        
+00006510: 746f 706f 6c6f 6779 5f72 6573 6f75 7263  topology_resourc
+00006520: 6573 5f70 6174 6873 3d74 6f70 6f6c 6f67  es_paths=topolog
+00006530: 795f 7265 736f 7572 6365 735f 7061 7468  y_resources_path
+00006540: 732c 0a20 2020 2020 2020 2061 6c6c 6f63  s,.        alloc
+00006550: 6174 696f 6e5f 7374 7261 7465 6779 3d61  ation_strategy=a
+00006560: 6c6c 6f63 6174 696f 6e5f 7374 7261 7465  llocation_strate
+00006570: 6779 2c0a 2020 2020 290a 0a0a 6465 6620  gy,.    )...def 
+00006580: 6578 7465 6e64 5f73 696d 756c 6174 696f  extend_simulatio
+00006590: 6e5f 6672 6f6d 5f74 6f70 6f6c 6f67 7928  n_from_topology(
+000065a0: 0a20 2020 2074 6f70 6f6c 6f67 795f 6669  .    topology_fi
+000065b0: 6c65 3a20 7374 7220 3d20 4e6f 6e65 2c0a  le: str = None,.
+000065c0: 2020 2020 746f 706f 6c6f 6779 5f72 6573      topology_res
+000065d0: 6f75 7263 6573 5f70 6174 6873 3a20 4f70  ources_paths: Op
+000065e0: 7469 6f6e 616c 5b4c 6973 745b 5061 7468  tional[List[Path
+000065f0: 5d5d 203d 204e 6f6e 652c 0a20 2020 2061  ]] = None,.    a
+00006600: 6c6c 6f63 6174 696f 6e5f 7374 7261 7465  llocation_strate
+00006610: 6779 3a20 4f70 7469 6f6e 616c 5b73 7472  gy: Optional[str
+00006620: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 6964  ] = None,.    id
+00006630: 5f73 696d 756c 6174 696f 6e3a 2069 6e74  _simulation: int
+00006640: 203d 204e 6f6e 652c 0a29 202d 3e20 5475   = None,.) -> Tu
+00006650: 706c 655b 696e 742c 204c 6973 745b 7374  ple[int, List[st
+00006660: 725d 5d3a 0a20 2020 2022 2222 4578 7465  r]]:.    """Exte
+00006670: 6e64 2061 6e20 6578 6973 7469 6e67 2073  nd an existing s
+00006680: 696d 756c 6174 696f 6e20 6d6f 6465 6c20  imulation model 
+00006690: 696e 2064 6174 6162 6173 6520 6261 7365  in database base
+000066a0: 6420 6f6e 2074 6865 2070 726f 7669 6465  d on the provide
+000066b0: 6420 746f 706f 6c6f 6779 2066 696c 652c  d topology file,
+000066c0: 2061 6c6f 6e67 2077 6974 6820 6f70 7469   along with opti
+000066d0: 6f6e 616c 2072 6573 6f75 7263 6520 6669  onal resource fi
+000066e0: 6c65 732e 0a0a 2020 2020 3a72 6574 7572  les...    :retur
+000066f0: 6e3a 2041 2074 7570 6c65 2063 6f6e 7461  n: A tuple conta
+00006700: 696e 696e 6720 7468 6520 4944 206f 6620  ining the ID of 
+00006710: 7468 6520 6372 6561 7465 6420 7369 6d75  the created simu
+00006720: 6c61 7469 6f6e 2c20 616e 6420 7468 6520  lation, and the 
+00006730: 6e65 7720 6e6f 6465 7320 6f66 2074 6865  new nodes of the
+00006740: 2073 696d 756c 6174 696f 6e2e 0a0a 2020   simulation...  
+00006750: 2020 3a70 6172 616d 2074 6f70 6f6c 6f67    :param topolog
+00006760: 795f 6669 6c65 3a20 5468 6520 7061 7468  y_file: The path
+00006770: 2074 6f20 6120 746f 706f 6c6f 6779 2066   to a topology f
+00006780: 696c 6520 636f 6e74 6169 6e69 6e67 2074  ile containing t
+00006790: 6865 206e 6f64 6573 2061 6e64 206e 6574  he nodes and net
+000067a0: 776f 726b 2074 6f70 6f6c 6f67 7920 746f  work topology to
+000067b0: 2061 6464 2e0a 2020 2020 3a70 6172 616d   add..    :param
+000067c0: 2074 6f70 6f6c 6f67 795f 7265 736f 7572   topology_resour
+000067d0: 6365 735f 7061 7468 733a 2054 6865 2070  ces_paths: The p
+000067e0: 6174 6820 746f 2072 6573 6f75 7263 6573  ath to resources
+000067f0: 2074 6861 7420 7769 6c6c 2062 6520 7075   that will be pu
+00006800: 7368 6564 2069 6e74 6f20 636f 6d70 6174  shed into compat
+00006810: 6962 6c65 206e 6f64 6573 2e0a 2020 2020  ible nodes..    
+00006820: 3a70 6172 616d 2061 6c6c 6f63 6174 696f  :param allocatio
+00006830: 6e5f 7374 7261 7465 6779 3a20 4e61 6d65  n_strategy: Name
+00006840: 206f 6620 7468 6520 616c 6c6f 6361 7469   of the allocati
+00006850: 6f6e 2073 7472 6174 6567 7920 746f 2075  on strategy to u
+00006860: 7365 2074 6f20 616c 6c6f 6361 7465 206e  se to allocate n
+00006870: 6f64 6573 2074 6f20 636f 6d70 7574 6520  odes to compute 
+00006880: 7365 7276 6572 732e 0a20 2020 203a 7061  servers..    :pa
+00006890: 7261 6d20 6964 5f73 696d 756c 6174 696f  ram id_simulatio
+000068a0: 6e3a 2054 6865 2073 696d 756c 6174 696f  n: The simulatio
+000068b0: 6e20 4944 2c20 7768 656e 2065 7874 656e  n ID, when exten
+000068c0: 6469 6e67 2061 6e20 6578 6973 7469 6e67  ding an existing
+000068d0: 2073 696d 756c 6174 696f 6e20 7769 7468   simulation with
+000068e0: 206e 6577 206e 6f64 6573 2061 6e64 206c   new nodes and l
+000068f0: 696e 6b73 2e0a 0a20 2020 2022 2222 0a20  inks...    """. 
+00006900: 2020 2069 6620 746f 706f 6c6f 6779 5f72     if topology_r
+00006910: 6573 6f75 7263 6573 5f70 6174 6873 2069  esources_paths i
+00006920: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00006930: 746f 706f 6c6f 6779 5f72 6573 6f75 7263  topology_resourc
+00006940: 6573 5f70 6174 6873 203d 205b 5d0a 0a20  es_paths = [].. 
+00006950: 2020 2023 2043 7265 6174 6520 6120 6e65     # Create a ne
+00006960: 7720 7369 6d75 6c61 7469 6f6e 206d 6f64  w simulation mod
+00006970: 656c 2069 6e20 6461 7461 6261 7365 2062  el in database b
+00006980: 6173 6564 206f 6e20 7468 6520 7072 6f76  ased on the prov
+00006990: 6964 6564 2074 6f70 6f6c 6f67 7920 6669  ided topology fi
+000069a0: 6c65 2070 6174 682e 2222 220a 2020 2020  le path.""".    
+000069b0: 6966 2074 6f70 6f6c 6f67 795f 6669 6c65  if topology_file
+000069c0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+000069d0: 2020 7261 6973 6520 4578 6365 7074 696f    raise Exceptio
+000069e0: 6e28 2241 6e20 746f 706f 6c6f 6779 2066  n("An topology f
+000069f0: 696c 6520 6973 2072 6571 7569 7265 6422  ile is required"
+00006a00: 290a 0a20 2020 2023 2056 616c 6964 6174  )..    # Validat
+00006a10: 6520 5941 4d4c 2063 6f6e 6669 6775 7261  e YAML configura
+00006a20: 7469 6f6e 2066 696c 650a 2020 2020 5f76  tion file.    _v
+00006a30: 616c 6964 6174 655f 7961 6d6c 5f74 6f70  alidate_yaml_top
+00006a40: 6f6c 6f67 795f 6669 6c65 2874 6f70 6f6c  ology_file(topol
+00006a50: 6f67 795f 6669 6c65 290a 0a20 2020 2023  ogy_file)..    #
+00006a60: 204f 7065 6e20 616e 6420 7265 6164 2059   Open and read Y
+00006a70: 414d 4c20 636f 6e66 6967 7572 6174 696f  AML configuratio
+00006a80: 6e20 6669 6c65 0a20 2020 2079 616d 6c5f  n file.    yaml_
+00006a90: 636f 6e74 656e 7420 3d20 5f72 6561 645f  content = _read_
+00006aa0: 7961 6d6c 5f74 6f70 6f6c 6f67 795f 6669  yaml_topology_fi
+00006ab0: 6c65 2874 6f70 6f6c 6f67 795f 6669 6c65  le(topology_file
+00006ac0: 290a 0a20 2020 2023 2050 6172 7365 2059  )..    # Parse Y
+00006ad0: 414d 4c20 636f 6e66 6967 7572 6174 696f  AML configuratio
+00006ae0: 6e0a 2020 2020 2320 5765 2075 7365 2072  n.    # We use r
+00006af0: 7561 6d65 6c2e 7961 6d6c 2062 6563 6175  uamel.yaml becau
+00006b00: 7365 2069 7420 6b65 6570 7320 616e 6368  se it keeps anch
+00006b10: 6f72 7320 616e 640a 2020 2020 2320 616c  ors and.    # al
+00006b20: 6961 7365 7320 696e 206d 656d 6f72 792e  iases in memory.
+00006b30: 2049 7420 6973 2076 6572 7920 636f 6e76   It is very conv
+00006b40: 656e 6965 6e74 2077 6865 6e20 7468 6520  enient when the 
+00006b50: 7369 6d75 6c61 7469 6f6e 0a20 2020 2023  simulation.    #
+00006b60: 2069 7320 7374 6f72 6564 2f66 6574 6368   is stored/fetch
+00006b70: 6564 2028 7265 6665 7265 6e63 6573 2061  ed (references a
+00006b80: 7265 206b 6570 7421 290a 2020 2020 6c6f  re kept!).    lo
+00006b90: 6164 6572 203d 2059 414d 4c28 7479 703d  ader = YAML(typ=
+00006ba0: 2272 7422 290a 2020 2020 746f 706f 6c6f  "rt").    topolo
+00006bb0: 6779 5f63 6f6e 7465 6e74 203d 206c 6f61  gy_content = loa
+00006bc0: 6465 722e 6c6f 6164 2879 616d 6c5f 636f  der.load(yaml_co
+00006bd0: 6e74 656e 7429 0a0a 2020 2020 2320 4164  ntent)..    # Ad
+00006be0: 6420 6120 6465 6661 756c 7420 7265 736f  d a default reso
+00006bf0: 7572 6365 7320 6469 7265 6374 6f72 7920  urces directory 
+00006c00: 6966 2069 7420 6578 6973 7473 2e0a 2020  if it exists..  
+00006c10: 2020 2320 4966 2074 6865 2074 6f70 6f6c    # If the topol
+00006c20: 6f67 7920 6973 2022 7061 7468 2f74 6f2f  ogy is "path/to/
+00006c30: 746f 706f 2e79 616d 6c22 2c20 7468 6520  topo.yaml", the 
+00006c40: 6465 6661 756c 7420 7265 736f 7572 6365  default resource
+00006c50: 7320 6469 7265 6374 6f72 7920 6973 2022  s directory is "
+00006c60: 7061 7468 2f74 6f2f 7265 736f 7572 6365  path/to/resource
+00006c70: 7322 2e0a 2020 2020 6465 6661 756c 745f  s"..    default_
+00006c80: 7265 736f 7572 6365 735f 7061 7468 203d  resources_path =
+00006c90: 206f 732e 7061 7468 2e6a 6f69 6e28 6f73   os.path.join(os
+00006ca0: 2e70 6174 682e 6469 726e 616d 6528 746f  .path.dirname(to
+00006cb0: 706f 6c6f 6779 5f66 696c 6529 2c20 2272  pology_file), "r
+00006cc0: 6573 6f75 7263 6573 2229 0a20 2020 2064  esources").    d
+00006cd0: 6566 6175 6c74 5f72 6573 6f75 7263 6573  efault_resources
+00006ce0: 5f70 6174 6820 3d20 6f73 2e70 6174 682e  _path = os.path.
+00006cf0: 6e6f 726d 7061 7468 2864 6566 6175 6c74  normpath(default
+00006d00: 5f72 6573 6f75 7263 6573 5f70 6174 6829  _resources_path)
+00006d10: 0a20 2020 2069 6620 5f5f 7661 6c69 6461  .    if __valida
+00006d20: 7465 5f72 6573 6f75 7263 6573 5f70 6174  te_resources_pat
+00006d30: 6828 6465 6661 756c 745f 7265 736f 7572  h(default_resour
+00006d40: 6365 735f 7061 7468 2c20 4661 6c73 6529  ces_path, False)
+00006d50: 3a0a 2020 2020 2020 2020 6966 2064 6566  :.        if def
+00006d60: 6175 6c74 5f72 6573 6f75 7263 6573 5f70  ault_resources_p
+00006d70: 6174 6820 6e6f 7420 696e 2074 6f70 6f6c  ath not in topol
+00006d80: 6f67 795f 7265 736f 7572 6365 735f 7061  ogy_resources_pa
+00006d90: 7468 733a 0a20 2020 2020 2020 2020 2020  ths:.           
+00006da0: 2074 6f70 6f6c 6f67 795f 7265 736f 7572   topology_resour
+00006db0: 6365 735f 7061 7468 732e 6170 7065 6e64  ces_paths.append
+00006dc0: 2864 6566 6175 6c74 5f72 6573 6f75 7263  (default_resourc
+00006dd0: 6573 5f70 6174 6829 0a0a 2020 2020 7265  es_path)..    re
+00006de0: 7475 726e 2065 7874 656e 645f 7369 6d75  turn extend_simu
+00006df0: 6c61 7469 6f6e 280a 2020 2020 2020 2020  lation(.        
+00006e00: 746f 706f 6c6f 6779 5f63 6f6e 7465 6e74  topology_content
+00006e10: 3d74 6f70 6f6c 6f67 795f 636f 6e74 656e  =topology_conten
+00006e20: 742c 0a20 2020 2020 2020 2074 6f70 6f6c  t,.        topol
+00006e30: 6f67 795f 7265 736f 7572 6365 735f 7061  ogy_resources_pa
+00006e40: 7468 733d 746f 706f 6c6f 6779 5f72 6573  ths=topology_res
+00006e50: 6f75 7263 6573 5f70 6174 6873 2c0a 2020  ources_paths,.  
+00006e60: 2020 2020 2020 616c 6c6f 6361 7469 6f6e        allocation
+00006e70: 5f73 7472 6174 6567 793d 616c 6c6f 6361  _strategy=alloca
+00006e80: 7469 6f6e 5f73 7472 6174 6567 792c 0a20  tion_strategy,. 
+00006e90: 2020 2020 2020 2069 645f 7369 6d75 6c61         id_simula
+00006ea0: 7469 6f6e 3d69 645f 7369 6d75 6c61 7469  tion=id_simulati
+00006eb0: 6f6e 2c0a 2020 2020 290a 0a0a 6465 6620  on,.    )...def 
+00006ec0: 6372 6561 7465 5f73 696d 756c 6174 696f  create_simulatio
+00006ed0: 6e5f 6672 6f6d 5f62 6173 6562 6f78 280a  n_from_basebox(.
+00006ee0: 2020 2020 6261 7365 626f 785f 6964 3a20      basebox_id: 
+00006ef0: 7374 722c 0a20 2020 2061 6464 5f69 6e74  str,.    add_int
+00006f00: 6572 6e65 743a 2062 6f6f 6c20 3d20 4661  ernet: bool = Fa
+00006f10: 6c73 652c 0a20 2020 2061 6464 5f68 6f73  lse,.    add_hos
+00006f20: 743a 2062 6f6f 6c20 3d20 4661 6c73 652c  t: bool = False,
+00006f30: 0a20 2020 2061 6c6c 6f63 6174 696f 6e5f  .    allocation_
+00006f40: 7374 7261 7465 6779 3a20 4f70 7469 6f6e  strategy: Option
+00006f50: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
+00006f60: 2920 2d3e 2054 7570 6c65 5b69 6e74 2c20  ) -> Tuple[int, 
+00006f70: 4c69 7374 5b73 7472 5d5d 3a0a 2020 2020  List[str]]:.    
+00006f80: 2222 2243 7265 6174 6520 6120 6e65 7720  """Create a new 
+00006f90: 7369 6d75 6c61 7469 6f6e 206d 6f64 656c  simulation model
+00006fa0: 2069 6e20 6461 7461 6261 7365 2062 6173   in database bas
+00006fb0: 6564 206f 6e20 7468 6520 7072 6f76 6964  ed on the provid
+00006fc0: 6564 2062 6173 6562 6f78 2069 642c 2077  ed basebox id, w
+00006fd0: 6974 680a 2020 2020 6f70 7469 6f6e 616c  ith.    optional
+00006fe0: 2069 6e74 6572 6e65 7420 616e 642f 6f72   internet and/or
+00006ff0: 2068 6f73 7420 636f 6e6e 6563 7469 7669   host connectivi
+00007000: 7479 2e0a 0a20 2020 203a 7265 7475 726e  ty...    :return
+00007010: 3a20 4120 7475 706c 6520 636f 6e74 6169  : A tuple contai
+00007020: 6e69 6e67 2074 6865 2049 4420 6f66 2074  ning the ID of t
+00007030: 6865 2063 7265 6174 6564 2073 696d 756c  he created simul
+00007040: 6174 696f 6e2c 2061 6e64 2074 6865 206e  ation, and the n
+00007050: 6577 206e 6f64 6573 206f 6620 7468 6520  ew nodes of the 
+00007060: 7369 6d75 6c61 7469 6f6e 2e0a 0a20 2020  simulation...   
+00007070: 203a 7061 7261 6d20 6261 7365 626f 785f   :param basebox_
+00007080: 6964 3a20 5468 6520 6261 7365 626f 7820  id: The basebox 
+00007090: 4944 2074 6f20 6164 6420 746f 2074 6865  ID to add to the
+000070a0: 2073 696d 756c 6174 696f 6e2e 0a20 2020   simulation..   
+000070b0: 203a 7061 7261 6d20 6164 645f 696e 7465   :param add_inte
+000070c0: 726e 6574 3a20 4164 6420 636f 6e6e 6563  rnet: Add connec
+000070d0: 7469 7669 7479 2074 6f20 696e 7465 726e  tivity to intern
+000070e0: 6574 2028 6e6f 7420 6163 7469 7665 2062  et (not active b
+000070f0: 7920 6465 6661 756c 7429 2e0a 2020 2020  y default)..    
+00007100: 3a70 6172 616d 2061 6464 5f68 6f73 743a  :param add_host:
+00007110: 2041 6464 2063 6f6e 6e65 6374 6976 6974   Add connectivit
+00007120: 7920 746f 2068 6f73 7420 7379 7374 656d  y to host system
+00007130: 2028 6e6f 7420 6163 7469 7665 2062 7920   (not active by 
+00007140: 6465 6661 756c 7429 2e0a 2020 2020 3a70  default)..    :p
+00007150: 6172 616d 2061 6c6c 6f63 6174 696f 6e5f  aram allocation_
+00007160: 7374 7261 7465 6779 3a20 4e61 6d65 206f  strategy: Name o
+00007170: 6620 7468 6520 616c 6c6f 6361 7469 6f6e  f the allocation
+00007180: 2073 7472 6174 6567 7920 746f 2075 7365   strategy to use
+00007190: 2074 6f20 616c 6c6f 6361 7465 206e 6f64   to allocate nod
+000071a0: 6573 2074 6f20 636f 6d70 7574 6520 7365  es to compute se
+000071b0: 7276 6572 732e 0a0a 2020 2020 2222 220a  rvers...    """.
+000071c0: 0a20 2020 2069 6620 6261 7365 626f 785f  .    if basebox_
+000071d0: 6964 2069 7320 4e6f 6e65 3a0a 2020 2020  id is None:.    
+000071e0: 2020 2020 7261 6973 6520 4578 6365 7074      raise Except
+000071f0: 696f 6e28 2241 2062 6173 6562 6f78 2049  ion("A basebox I
+00007200: 4420 6973 2072 6571 7569 7265 6422 290a  D is required").
+00007210: 0a20 2020 2023 2043 7265 6174 6520 616e  .    # Create an
+00007220: 2074 6f70 6f6c 6f67 7920 7769 7468 2074   topology with t
+00007230: 6865 2070 726f 7669 6465 6420 6261 7365  he provided base
+00007240: 626f 7820 4944 0a20 2020 2074 7279 3a0a  box ID.    try:.
+00007250: 2020 2020 2020 2020 6261 7365 626f 7820          basebox 
+00007260: 3d20 6665 7463 685f 6261 7365 626f 7828  = fetch_basebox(
+00007270: 6261 7365 626f 785f 6964 290a 2020 2020  basebox_id).    
+00007280: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
+00007290: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
+000072a0: 4578 6365 7074 696f 6e28 0a20 2020 2020  Exception(.     
+000072b0: 2020 2020 2020 2066 2243 616e 6e6f 7420         f"Cannot 
+000072c0: 6669 6e64 2062 6173 6562 6f78 2069 6e20  find basebox in 
+000072d0: 6461 7461 6261 7365 2066 726f 6d20 6261  database from ba
+000072e0: 7365 626f 7820 4944 2027 7b62 6173 6562  sebox ID '{baseb
+000072f0: 6f78 5f69 647d 2722 0a20 2020 2020 2020  ox_id}'".       
+00007300: 2029 0a0a 2020 2020 6e6f 6465 5f6e 616d   )..    node_nam
+00007310: 6520 3d20 5f67 6574 5f72 616e 646f 6d5f  e = _get_random_
+00007320: 7374 7269 6e67 2831 3029 0a20 2020 2072  string(10).    r
+00007330: 6f6c 6520 3d20 6261 7365 626f 785b 2272  ole = basebox["r
+00007340: 6f6c 6522 5d0a 2020 2020 6e62 5f70 726f  ole"].    nb_pro
+00007350: 6320 3d20 6261 7365 626f 785b 226e 625f  c = basebox["nb_
+00007360: 7072 6f63 225d 0a20 2020 206d 656d 6f72  proc"].    memor
+00007370: 795f 7369 7a65 203d 2062 6173 6562 6f78  y_size = basebox
+00007380: 5b22 6d65 6d6f 7279 5f73 697a 6522 5d0a  ["memory_size"].
+00007390: 0a20 2020 2079 616d 6c5f 636f 6e74 656e  .    yaml_conten
+000073a0: 7420 3d20 6622 2222 2d2d 2d0a 6e61 6d65  t = f"""---.name
+000073b0: 3a20 227b 6261 7365 626f 785f 6964 7d22  : "{basebox_id}"
+000073c0: 0a6e 6f64 6573 3a0a 0a20 202d 2026 7377  .nodes:..  - &sw
+000073d0: 6974 6368 0a20 2020 2074 7970 653a 2073  itch.    type: s
+000073e0: 7769 7463 680a 2020 2020 6e61 6d65 3a20  witch.    name: 
+000073f0: 2273 7769 7463 6822 0a0a 2020 2d20 2663  "switch"..  - &c
+00007400: 6c69 656e 740a 2020 2020 7479 7065 3a20  lient.    type: 
+00007410: 7669 7274 7561 6c5f 6d61 6368 696e 650a  virtual_machine.
+00007420: 2020 2020 6e61 6d65 3a20 227b 6e6f 6465      name: "{node
+00007430: 5f6e 616d 657d 220a 2020 2020 6261 7365  _name}".    base
+00007440: 626f 785f 6964 3a20 227b 6261 7365 626f  box_id: "{basebo
+00007450: 785f 6964 7d22 0a20 2020 206e 625f 7072  x_id}".    nb_pr
+00007460: 6f63 3a20 7b6e 625f 7072 6f63 7d0a 2020  oc: {nb_proc}.  
+00007470: 2020 6d65 6d6f 7279 5f73 697a 653a 207b    memory_size: {
+00007480: 6d65 6d6f 7279 5f73 697a 657d 0a20 2020  memory_size}.   
+00007490: 2072 6f6c 6573 3a20 5b22 7b72 6f6c 657d   roles: ["{role}
+000074a0: 225d 0a22 2222 0a0a 2020 2020 6966 2061  "]."""..    if a
+000074b0: 6464 5f68 6f73 743a 0a20 2020 2020 2020  dd_host:.       
+000074c0: 2079 616d 6c5f 636f 6e74 656e 7420 2b3d   yaml_content +=
+000074d0: 2022 2222 0a20 202d 2026 686f 7374 5f6d   """.  - &host_m
+000074e0: 6163 6869 6e65 0a20 2020 2074 7970 653a  achine.    type:
+000074f0: 2068 6f73 745f 6d61 6368 696e 650a 2020   host_machine.  
+00007500: 2020 6e61 6d65 3a20 2268 6f73 7422 0a22    name: "host"."
+00007510: 2222 0a0a 2020 2020 6966 2061 6464 5f69  ""..    if add_i
+00007520: 6e74 6572 6e65 743a 0a20 2020 2020 2020  nternet:.       
+00007530: 2023 2061 6464 2064 6566 6175 6c74 2072   # add default r
+00007540: 6f75 7465 2074 6f20 6761 7465 7761 792c  oute to gateway,
+00007550: 2061 2067 6174 6577 6179 2061 6e64 2061   a gateway and a
+00007560: 2073 7769 7463 6820 746f 2070 6c75 6720   switch to plug 
+00007570: 7468 6520 6761 7465 7761 7920 616e 6420  the gateway and 
+00007580: 7468 6520 726f 7574 6572 0a20 2020 2020  the router.     
+00007590: 2020 2079 616d 6c5f 636f 6e74 656e 7420     yaml_content 
+000075a0: 2b3d 2022 2222 0a20 202d 2026 726f 7574  += """.  - &rout
+000075b0: 6572 0a20 2020 2074 7970 653a 2072 6f75  er.    type: rou
+000075c0: 7465 720a 2020 2020 6e61 6d65 3a20 2272  ter.    name: "r
+000075d0: 6f75 7465 7222 0a20 2020 2072 6f75 7465  outer".    route
+000075e0: 733a 0a20 2020 2020 202d 2022 302e 302e  s:.      - "0.0.
+000075f0: 302e 302f 3020 2d3e 2031 3932 2e31 3638  0.0/0 -> 192.168
+00007600: 2e32 332e 3222 0a0a 2020 2d20 2673 7769  .23.2"..  - &swi
+00007610: 7463 685f 696e 7465 726e 6574 0a20 2020  tch_internet.   
+00007620: 2074 7970 653a 2073 7769 7463 680a 2020   type: switch.  
+00007630: 2020 6e61 6d65 3a20 2273 7769 7463 6849    name: "switchI
+00007640: 6e74 6572 6e65 7422 0a0a 2020 2d20 2670  nternet"..  - &p
+00007650: 6879 7369 6361 6c5f 6761 7465 7761 790a  hysical_gateway.
+00007660: 2020 2020 7479 7065 3a20 7068 7973 6963      type: physic
+00007670: 616c 5f67 6174 6577 6179 0a20 2020 206e  al_gateway.    n
+00007680: 616d 653a 2022 7068 7973 6963 616c 4761  ame: "physicalGa
+00007690: 7465 7761 7922 0a22 2222 0a20 2020 2065  teway".""".    e
+000076a0: 6c73 653a 0a20 2020 2020 2020 2079 616d  lse:.        yam
+000076b0: 6c5f 636f 6e74 656e 7420 2b3d 2022 2222  l_content += """
+000076c0: 0a20 202d 2026 726f 7574 6572 0a20 2020  .  - &router.   
+000076d0: 2074 7970 653a 2072 6f75 7465 720a 2020   type: router.  
+000076e0: 2020 6e61 6d65 3a20 2272 6f75 7465 7222    name: "router"
+000076f0: 0a22 2222 0a0a 2020 2020 7961 6d6c 5f63  ."""..    yaml_c
+00007700: 6f6e 7465 6e74 202b 3d20 2222 220a 6c69  ontent += """.li
+00007710: 6e6b 733a 0a0a 2020 2d20 7377 6974 6368  nks:..  - switch
+00007720: 3a20 2a73 7769 7463 680a 2020 2020 6e6f  : *switch.    no
+00007730: 6465 3a20 2a72 6f75 7465 720a 2020 2020  de: *router.    
+00007740: 7061 7261 6d73 3a0a 2020 2020 2020 6970  params:.      ip
+00007750: 3a20 2231 3932 2e31 3638 2e32 2e31 2f32  : "192.168.2.1/2
+00007760: 3422 0a20 2020 2020 2064 6863 705f 6e61  4".      dhcp_na
+00007770: 6d65 7365 7276 6572 3a20 2238 2e38 2e38  meserver: "8.8.8
+00007780: 2e38 220a 0a20 202d 2073 7769 7463 683a  .8"..  - switch:
+00007790: 202a 7377 6974 6368 0a20 2020 206e 6f64   *switch.    nod
+000077a0: 653a 202a 636c 6965 6e74 0a20 2020 2070  e: *client.    p
+000077b0: 6172 616d 733a 0a20 2020 2020 2069 703a  arams:.      ip:
+000077c0: 2022 3139 322e 3136 382e 322e 322f 3234   "192.168.2.2/24
+000077d0: 220a 2222 220a 0a20 2020 2069 6620 6164  "."""..    if ad
+000077e0: 645f 686f 7374 3a0a 2020 2020 2020 2020  d_host:.        
+000077f0: 7961 6d6c 5f63 6f6e 7465 6e74 202b 3d20  yaml_content += 
+00007800: 2222 220a 2020 2d20 7377 6974 6368 3a20  """.  - switch: 
+00007810: 2a73 7769 7463 680a 2020 2020 6e6f 6465  *switch.    node
+00007820: 3a20 2a68 6f73 745f 6d61 6368 696e 650a  : *host_machine.
+00007830: 2020 2020 7061 7261 6d73 3a0a 2020 2020      params:.    
+00007840: 2020 6970 3a20 2231 3932 2e31 3638 2e32    ip: "192.168.2
+00007850: 2e33 2f32 3422 0a22 2222 0a0a 2020 2020  .3/24"."""..    
+00007860: 6966 2061 6464 5f69 6e74 6572 6e65 743a  if add_internet:
+00007870: 0a20 2020 2020 2020 2079 616d 6c5f 636f  .        yaml_co
+00007880: 6e74 656e 7420 2b3d 2022 2222 0a20 202d  ntent += """.  -
+00007890: 2073 7769 7463 683a 202a 7377 6974 6368   switch: *switch
+000078a0: 5f69 6e74 6572 6e65 740a 2020 2020 6e6f  _internet.    no
+000078b0: 6465 3a20 2a72 6f75 7465 720a 2020 2020  de: *router.    
+000078c0: 7061 7261 6d73 3a0a 2020 2020 2020 6970  params:.      ip
+000078d0: 3a20 2231 3932 2e31 3638 2e32 332e 312f  : "192.168.23.1/
+000078e0: 3234 220a 0a20 202d 2073 7769 7463 683a  24"..  - switch:
+000078f0: 202a 7377 6974 6368 5f69 6e74 6572 6e65   *switch_interne
+00007900: 740a 2020 2020 6e6f 6465 3a20 2a70 6879  t.    node: *phy
+00007910: 7369 6361 6c5f 6761 7465 7761 790a 2020  sical_gateway.  
+00007920: 2020 7061 7261 6d73 3a0a 2020 2020 2020    params:.      
+00007930: 6970 3a20 2231 3932 2e31 3638 2e32 332e  ip: "192.168.23.
+00007940: 322f 3234 220a 2222 220a 0a20 2020 206c  2/24"."""..    l
+00007950: 6f61 6465 7220 3d20 5941 4d4c 2874 7970  oader = YAML(typ
+00007960: 3d22 7274 2229 0a20 2020 2074 6f70 6f6c  ="rt").    topol
+00007970: 6f67 795f 636f 6e74 656e 7420 3d20 6c6f  ogy_content = lo
+00007980: 6164 6572 2e6c 6f61 6428 7961 6d6c 5f63  ader.load(yaml_c
+00007990: 6f6e 7465 6e74 290a 0a20 2020 2072 6574  ontent)..    ret
+000079a0: 7572 6e20 6372 6561 7465 5f73 696d 756c  urn create_simul
+000079b0: 6174 696f 6e28 0a20 2020 2020 2020 2074  ation(.        t
+000079c0: 6f70 6f6c 6f67 795f 636f 6e74 656e 743d  opology_content=
+000079d0: 746f 706f 6c6f 6779 5f63 6f6e 7465 6e74  topology_content
+000079e0: 2c0a 2020 2020 2020 2020 616c 6c6f 6361  ,.        alloca
+000079f0: 7469 6f6e 5f73 7472 6174 6567 793d 616c  tion_strategy=al
+00007a00: 6c6f 6361 7469 6f6e 5f73 7472 6174 6567  location_strateg
+00007a10: 792c 0a20 2020 2029 0a0a 0a64 6566 2065  y,.    )...def e
+00007a20: 7874 656e 645f 7369 6d75 6c61 7469 6f6e  xtend_simulation
+00007a30: 5f66 726f 6d5f 6261 7365 626f 7828 0a20  _from_basebox(. 
+00007a40: 2020 2062 6173 6562 6f78 5f69 643a 2073     basebox_id: s
+00007a50: 7472 2c0a 2020 2020 7377 6974 6368 5f6e  tr,.    switch_n
+00007a60: 616d 653a 2073 7472 2c0a 2020 2020 616c  ame: str,.    al
+00007a70: 6c6f 6361 7469 6f6e 5f73 7472 6174 6567  location_strateg
+00007a80: 793a 204f 7074 696f 6e61 6c5b 7374 725d  y: Optional[str]
+00007a90: 203d 204e 6f6e 652c 0a20 2020 2069 645f   = None,.    id_
+00007aa0: 7369 6d75 6c61 7469 6f6e 3a20 696e 7420  simulation: int 
+00007ab0: 3d20 4e6f 6e65 2c0a 2920 2d3e 2054 7570  = None,.) -> Tup
+00007ac0: 6c65 5b69 6e74 2c20 4c69 7374 5b73 7472  le[int, List[str
+00007ad0: 5d5d 3a0a 2020 2020 2222 2245 7874 656e  ]]:.    """Exten
+00007ae0: 6420 616e 2065 7869 7374 696e 6720 7369  d an existing si
+00007af0: 6d75 6c61 7469 6f6e 206d 6f64 656c 2069  mulation model i
+00007b00: 6e20 6461 7461 6261 7365 2062 6173 6564  n database based
+00007b10: 206f 6e20 7468 650a 2020 2020 7072 6f76   on the.    prov
+00007b20: 6964 6564 2062 6173 6562 6f78 2069 642c  ided basebox id,
+00007b30: 2061 6e64 2070 6c75 6720 7468 6520 6e65   and plug the ne
+00007b40: 7720 6e6f 6465 206f 6620 7468 6520 7370  w node of the sp
+00007b50: 6563 6966 6564 2073 7769 7463 682e 0a0a  ecifed switch...
+00007b60: 2020 2020 3a72 6574 7572 6e3a 2041 2074      :return: A t
+00007b70: 7570 6c65 2063 6f6e 7461 696e 696e 6720  uple containing 
+00007b80: 7468 6520 4944 206f 6620 7468 6520 7570  the ID of the up
+00007b90: 6461 7465 6420 7369 6d75 6c61 7469 6f6e  dated simulation
+00007ba0: 2c20 616e 6420 7468 6520 6e65 7720 6e6f  , and the new no
+00007bb0: 6465 7320 6f66 2074 6865 2073 696d 756c  des of the simul
+00007bc0: 6174 696f 6e2e 0a0a 2020 2020 3a70 6172  ation...    :par
+00007bd0: 616d 2062 6173 6562 6f78 5f69 643a 2054  am basebox_id: T
+00007be0: 6865 2062 6173 6562 6f78 2049 4420 746f  he basebox ID to
+00007bf0: 2061 6464 2074 6f20 7468 6520 7369 6d75   add to the simu
+00007c00: 6c61 7469 6f6e 2e0a 2020 2020 3a70 6172  lation..    :par
+00007c10: 616d 2073 7769 7463 685f 6e61 6d65 3a20  am switch_name: 
+00007c20: 5468 6520 7377 6974 6368 206e 616d 6520  The switch name 
+00007c30: 6f6e 2077 6869 6368 2074 6f20 636f 6e6e  on which to conn
+00007c40: 6563 7420 7468 6520 6e65 7720 6261 7365  ect the new base
+00007c50: 626f 782e 0a20 2020 203a 7061 7261 6d20  box..    :param 
+00007c60: 616c 6c6f 6361 7469 6f6e 5f73 7472 6174  allocation_strat
+00007c70: 6567 793a 204e 616d 6520 6f66 2074 6865  egy: Name of the
+00007c80: 2061 6c6c 6f63 6174 696f 6e20 7374 7261   allocation stra
+00007c90: 7465 6779 2074 6f20 7573 6520 746f 2061  tegy to use to a
+00007ca0: 6c6c 6f63 6174 6520 6e6f 6465 7320 746f  llocate nodes to
+00007cb0: 2063 6f6d 7075 7465 2073 6572 7665 7273   compute servers
+00007cc0: 2e0a 2020 2020 3a70 6172 616d 2069 645f  ..    :param id_
+00007cd0: 7369 6d75 6c61 7469 6f6e 3a20 5468 6520  simulation: The 
+00007ce0: 7369 6d75 6c61 7469 6f6e 2049 442c 2077  simulation ID, w
+00007cf0: 6865 6e20 6578 7465 6e64 696e 6720 616e  hen extending an
+00007d00: 2065 7869 7374 696e 6720 7369 6d75 6c61   existing simula
+00007d10: 7469 6f6e 2077 6974 6820 6e65 7720 6e6f  tion with new no
+00007d20: 6465 7320 616e 6420 6c69 6e6b 732e 0a0a  des and links...
+00007d30: 2020 2020 2222 220a 0a20 2020 2069 6620      """..    if 
+00007d40: 6261 7365 626f 785f 6964 2069 7320 4e6f  basebox_id is No
+00007d50: 6e65 3a0a 2020 2020 2020 2020 7261 6973  ne:.        rais
+00007d60: 6520 4578 6365 7074 696f 6e28 2241 2062  e Exception("A b
+00007d70: 6173 6562 6f78 2049 4420 6973 2072 6571  asebox ID is req
+00007d80: 7569 7265 6422 290a 0a20 2020 2023 2043  uired")..    # C
+00007d90: 7265 6174 6520 616e 2074 6f70 6f6c 6f67  reate an topolog
+00007da0: 7920 7769 7468 2074 6865 2070 726f 7669  y with the provi
+00007db0: 6465 6420 6261 7365 626f 7820 4944 0a20  ded basebox ID. 
+00007dc0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+00007dd0: 6261 7365 626f 7820 3d20 6665 7463 685f  basebox = fetch_
+00007de0: 6261 7365 626f 7828 6261 7365 626f 785f  basebox(basebox_
+00007df0: 6964 290a 2020 2020 6578 6365 7074 2045  id).    except E
+00007e00: 7863 6570 7469 6f6e 3a0a 2020 2020 2020  xception:.      
+00007e10: 2020 7261 6973 6520 4578 6365 7074 696f    raise Exceptio
+00007e20: 6e28 0a20 2020 2020 2020 2020 2020 2066  n(.            f
+00007e30: 2243 616e 6e6f 7420 6669 6e64 2062 6173  "Cannot find bas
+00007e40: 6562 6f78 2069 6e20 6461 7461 6261 7365  ebox in database
+00007e50: 2066 726f 6d20 6261 7365 626f 7820 4944   from basebox ID
+00007e60: 2027 7b62 6173 6562 6f78 5f69 647d 2722   '{basebox_id}'"
+00007e70: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+00007e80: 6e6f 6465 5f6e 616d 6520 3d20 5f67 6574  node_name = _get
+00007e90: 5f72 616e 646f 6d5f 7374 7269 6e67 2831  _random_string(1
+00007ea0: 3029 0a20 2020 2072 6f6c 6520 3d20 6261  0).    role = ba
+00007eb0: 7365 626f 785b 2272 6f6c 6522 5d0a 2020  sebox["role"].  
+00007ec0: 2020 6e62 5f70 726f 6320 3d20 6261 7365    nb_proc = base
+00007ed0: 626f 785b 226e 625f 7072 6f63 225d 0a20  box["nb_proc"]. 
+00007ee0: 2020 206d 656d 6f72 795f 7369 7a65 203d     memory_size =
+00007ef0: 2062 6173 6562 6f78 5b22 6d65 6d6f 7279   basebox["memory
+00007f00: 5f73 697a 6522 5d0a 0a20 2020 2074 6f70  _size"]..    top
+00007f10: 6f6c 6f67 795f 636f 6e74 656e 7420 3d20  ology_content = 
+00007f20: 7b0a 2020 2020 2020 2020 226e 6f64 6573  {.        "nodes
+00007f30: 223a 205b 0a20 2020 2020 2020 2020 2020  ": [.           
+00007f40: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00007f50: 2020 2022 7479 7065 223a 2022 7669 7274     "type": "virt
+00007f60: 7561 6c5f 6d61 6368 696e 6522 2c0a 2020  ual_machine",.  
+00007f70: 2020 2020 2020 2020 2020 2020 2020 226e                "n
+00007f80: 616d 6522 3a20 6e6f 6465 5f6e 616d 652c  ame": node_name,
+00007f90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007fa0: 2022 6261 7365 626f 785f 6964 223a 2062   "basebox_id": b
+00007fb0: 6173 6562 6f78 5f69 642c 0a20 2020 2020  asebox_id,.     
+00007fc0: 2020 2020 2020 2020 2020 2022 6e62 5f70             "nb_p
+00007fd0: 726f 6322 3a20 6e62 5f70 726f 632c 0a20  roc": nb_proc,. 
+00007fe0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00007ff0: 6d65 6d6f 7279 5f73 697a 6522 3a20 6d65  memory_size": me
+00008000: 6d6f 7279 5f73 697a 652c 0a20 2020 2020  mory_size,.     
+00008010: 2020 2020 2020 2020 2020 2022 726f 6c65             "role
+00008020: 7322 3a20 5b72 6f6c 655d 2c0a 2020 2020  s": [role],.    
+00008030: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00008040: 2020 5d2c 0a20 2020 2020 2020 2022 6c69    ],.        "li
+00008050: 6e6b 7322 3a20 5b0a 2020 2020 2020 2020  nks": [.        
+00008060: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+00008070: 2020 2020 2020 2273 7769 7463 6822 3a20        "switch": 
+00008080: 7b22 7479 7065 223a 2022 7377 6974 6368  {"type": "switch
+00008090: 222c 2022 6e61 6d65 223a 2073 7769 7463  ", "name": switc
+000080a0: 685f 6e61 6d65 7d2c 0a20 2020 2020 2020  h_name},.       
+000080b0: 2020 2020 2020 2020 2022 6e6f 6465 223a           "node":
+000080c0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+000080d0: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
+000080e0: 7669 7274 7561 6c5f 6d61 6368 696e 6522  virtual_machine"
+000080f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00008100: 2020 2020 2020 226e 616d 6522 3a20 6e6f        "name": no
+00008110: 6465 5f6e 616d 652c 0a20 2020 2020 2020  de_name,.       
+00008120: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+00008130: 2020 2020 2020 2020 2020 2020 2270 6172              "par
+00008140: 616d 7322 3a20 7b7d 2c20 2023 2044 796e  ams": {},  # Dyn
+00008150: 616d 6963 2049 5020 6164 6472 6573 730a  amic IP address.
+00008160: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00008170: 2020 2020 2020 5d2c 0a20 2020 207d 0a0a        ],.    }..
+00008180: 2020 2020 7265 7475 726e 2065 7874 656e      return exten
+00008190: 645f 7369 6d75 6c61 7469 6f6e 280a 2020  d_simulation(.  
+000081a0: 2020 2020 2020 746f 706f 6c6f 6779 5f63        topology_c
+000081b0: 6f6e 7465 6e74 3d74 6f70 6f6c 6f67 795f  ontent=topology_
+000081c0: 636f 6e74 656e 742c 0a20 2020 2020 2020  content,.       
+000081d0: 2061 6c6c 6f63 6174 696f 6e5f 7374 7261   allocation_stra
+000081e0: 7465 6779 3d61 6c6c 6f63 6174 696f 6e5f  tegy=allocation_
+000081f0: 7374 7261 7465 6779 2c0a 2020 2020 2020  strategy,.      
+00008200: 2020 6964 5f73 696d 756c 6174 696f 6e3d    id_simulation=
+00008210: 6964 5f73 696d 756c 6174 696f 6e2c 0a20  id_simulation,. 
+00008220: 2020 2029 0a0a 0a23 2323 0a23 2054 6f70     )...###.# Top
+00008230: 6f6c 6f67 7920 6865 6c70 6572 730a 2323  ology helpers.##
+00008240: 230a 0a0a 6465 6620 746f 706f 6c6f 6779  #...def topology
+00008250: 5f66 696c 655f 6164 645f 7765 6273 6974  _file_add_websit
+00008260: 6573 280a 2020 2020 746f 706f 6c6f 6779  es(.    topology
+00008270: 5f66 696c 653a 2073 7472 2c20 7765 6273  _file: str, webs
+00008280: 6974 6573 3a20 4c69 7374 5b73 7472 5d2c  ites: List[str],
+00008290: 2073 7769 7463 685f 6e61 6d65 3a20 7374   switch_name: st
+000082a0: 720a 2920 2d3e 2073 7472 3a0a 2020 2020  r.) -> str:.    
+000082b0: 2222 2241 6464 2064 6f63 6b65 7220 7765  """Add docker we
+000082c0: 6273 6974 6573 206e 6f64 6520 746f 2061  bsites node to a
+000082d0: 2067 6976 656e 2074 6f70 6f6c 6f67 792c   given topology,
+000082e0: 2061 6e64 2072 6574 7572 6e20 7468 6520   and return the 
+000082f0: 7570 6461 7465 6420 746f 706f 6c6f 6779  updated topology
+00008300: 2e0a 0a20 2020 203a 7265 7475 726e 3a20  ...    :return: 
+00008310: 5468 6520 7570 6461 7465 6420 746f 706f  The updated topo
+00008320: 6c6f 6779 2063 6f6e 7465 6e74 2061 7320  logy content as 
+00008330: 6120 7374 7269 6e67 2e0a 0a20 2020 203a  a string...    :
+00008340: 7061 7261 6d20 746f 706f 6c6f 6779 5f66  param topology_f
+00008350: 696c 653a 2054 6865 2070 6174 6820 746f  ile: The path to
+00008360: 2061 2074 6f70 6f6c 6f67 7920 6669 6c65   a topology file
+00008370: 2e0a 2020 2020 3a70 6172 616d 2077 6562  ..    :param web
+00008380: 7369 7465 733a 2054 6865 2077 6562 7369  sites: The websi
+00008390: 7465 206e 616d 6573 2074 6f20 6164 6420  te names to add 
+000083a0: 746f 2074 6865 2074 6f70 6f6c 6f67 792e  to the topology.
+000083b0: 0a20 2020 203a 7061 7261 6d20 7377 6974  .    :param swit
+000083c0: 6368 5f6e 616d 653a 2054 6865 2073 7769  ch_name: The swi
+000083d0: 7463 6820 6f6e 2077 6869 6368 2074 6f20  tch on which to 
+000083e0: 636f 6e6e 6563 7420 7468 6520 646f 636b  connect the dock
+000083f0: 6572 2077 6562 7369 7465 206e 6f64 6573  er website nodes
+00008400: 2e0a 0a20 2020 2022 2222 0a0a 2020 2020  ...    """..    
+00008410: 2320 5661 6c69 6461 7465 2059 414d 4c20  # Validate YAML 
+00008420: 746f 706f 6c6f 6779 2066 696c 650a 2020  topology file.  
+00008430: 2020 5f76 616c 6964 6174 655f 7961 6d6c    _validate_yaml
+00008440: 5f74 6f70 6f6c 6f67 795f 6669 6c65 2874  _topology_file(t
+00008450: 6f70 6f6c 6f67 795f 6669 6c65 290a 0a20  opology_file).. 
+00008460: 2020 2023 204f 7065 6e20 616e 6420 7265     # Open and re
+00008470: 6164 2059 414d 4c20 746f 706f 6c6f 6779  ad YAML topology
+00008480: 2066 696c 650a 2020 2020 746f 706f 6c6f   file.    topolo
+00008490: 6779 5f79 616d 6c20 3d20 5f72 6561 645f  gy_yaml = _read_
+000084a0: 7961 6d6c 5f74 6f70 6f6c 6f67 795f 6669  yaml_topology_fi
+000084b0: 6c65 2874 6f70 6f6c 6f67 795f 6669 6c65  le(topology_file
+000084c0: 290a 0a20 2020 2023 2055 7064 6174 6520  )..    # Update 
+000084d0: 746f 706f 6c6f 6779 2077 6974 6820 7468  topology with th
+000084e0: 6520 4150 490a 2020 2020 746f 706f 6c6f  e API.    topolo
+000084f0: 6779 5f79 616d 6c20 3d20 746f 706f 6c6f  gy_yaml = topolo
+00008500: 6779 5f61 6464 5f77 6562 7369 7465 7328  gy_add_websites(
+00008510: 746f 706f 6c6f 6779 5f79 616d 6c2c 2077  topology_yaml, w
+00008520: 6562 7369 7465 732c 2073 7769 7463 685f  ebsites, switch_
+00008530: 6e61 6d65 290a 0a20 2020 2072 6574 7572  name)..    retur
+00008540: 6e20 746f 706f 6c6f 6779 5f79 616d 6c0a  n topology_yaml.
+00008550: 0a0a 6465 6620 746f 706f 6c6f 6779 5f66  ..def topology_f
+00008560: 696c 655f 6164 645f 6467 6128 0a20 2020  ile_add_dga(.   
+00008570: 2074 6f70 6f6c 6f67 795f 6669 6c65 3a20   topology_file: 
+00008580: 7374 722c 0a20 2020 2061 6c67 6f72 6974  str,.    algorit
+00008590: 686d 3a20 7374 722c 0a20 2020 2073 7769  hm: str,.    swi
+000085a0: 7463 685f 6e61 6d65 3a20 7374 722c 0a20  tch_name: str,. 
+000085b0: 2020 206e 756d 6265 723a 2069 6e74 2c0a     number: int,.
+000085c0: 2020 2020 7265 736f 7572 6365 735f 6469      resources_di
+000085d0: 723a 2073 7472 2c0a 2920 2d3e 2054 7570  r: str,.) -> Tup
+000085e0: 6c65 5b73 7472 2c20 4c69 7374 5b73 7472  le[str, List[str
+000085f0: 5d5d 3a0a 2020 2020 2222 2241 6464 2064  ]]:.    """Add d
+00008600: 6f63 6b65 7220 656d 7074 7920 7765 6273  ocker empty webs
+00008610: 6974 6573 206e 6f64 6520 7769 7468 2044  ites node with D
+00008620: 4741 2064 6f6d 6169 6e73 2074 6f20 6120  GA domains to a 
+00008630: 6769 7665 6e20 746f 706f 6c6f 6779 2c20  given topology, 
+00008640: 616e 6420 7265 7475 726e 2074 6865 2075  and return the u
+00008650: 7064 6174 6564 2074 6f70 6f6c 6f67 792e  pdated topology.
+00008660: 0a0a 2020 2020 3a72 6574 7572 6e3a 2041  ..    :return: A
+00008670: 206e 6577 2074 6f70 6f6c 6f67 7920 636f   new topology co
+00008680: 6e74 656e 742c 2061 6c6f 6e67 2077 6974  ntent, along wit
+00008690: 6820 7468 6520 6c69 7374 206f 6620 6164  h the list of ad
+000086a0: 6465 6420 646f 6d61 696e 732e 0a0a 2020  ded domains...  
+000086b0: 2020 3a70 6172 616d 2074 6f70 6f6c 6f67    :param topolog
+000086c0: 795f 6669 6c65 3a20 5468 6520 7061 7468  y_file: The path
+000086d0: 2074 6f20 6120 746f 706f 6c6f 6779 2066   to a topology f
+000086e0: 696c 652e 0a20 2020 203a 7061 7261 6d20  ile..    :param 
+000086f0: 616c 676f 7269 7468 6d3a 2054 6865 2061  algorithm: The a
+00008700: 6c67 6f72 6974 686d 2075 7365 6420 746f  lgorithm used to
+00008710: 2067 656e 6572 6174 6520 7468 6520 6e65   generate the ne
+00008720: 7720 4447 4120 646f 6d61 696e 732e 0a20  w DGA domains.. 
+00008730: 2020 203a 7061 7261 6d20 7377 6974 6368     :param switch
+00008740: 5f6e 616d 653a 2054 6865 2073 7769 7463  _name: The switc
+00008750: 6820 6f6e 2077 6869 6368 2074 6f20 636f  h on which to co
+00008760: 6e6e 6563 7420 7468 6520 646f 636b 6572  nnect the docker
+00008770: 2077 6562 7369 7465 206e 6f64 6573 2e0a   website nodes..
+00008780: 2020 2020 3a70 6172 616d 206e 756d 6265      :param numbe
+00008790: 723a 2054 6865 206e 756d 6265 7220 6f66  r: The number of
+000087a0: 2044 4741 2064 6f6d 6169 6e73 2074 6f20   DGA domains to 
+000087b0: 6164 642e 0a20 2020 203a 7061 7261 6d20  add..    :param 
+000087c0: 746f 706f 6c6f 6779 5f64 6972 3a20 5468  topology_dir: Th
+000087d0: 6520 7061 7468 2074 6f20 7265 736f 7572  e path to resour
+000087e0: 6365 7320 7468 6174 2077 696c 6c20 6265  ces that will be
+000087f0: 2070 7573 6865 6420 696e 746f 2074 6865   pushed into the
+00008800: 206e 6577 2064 6f63 6b65 7220 6e6f 6465   new docker node
+00008810: 732e 0a0a 2020 2020 2222 220a 0a20 2020  s...    """..   
+00008820: 2023 2056 616c 6964 6174 650a 0a20 2020   # Validate..   
+00008830: 2023 2056 616c 6964 6174 6520 5941 4d4c   # Validate YAML
+00008840: 2074 6f70 6f6c 6f67 7920 6669 6c65 0a20   topology file. 
+00008850: 2020 205f 7661 6c69 6461 7465 5f79 616d     _validate_yam
+00008860: 6c5f 746f 706f 6c6f 6779 5f66 696c 6528  l_topology_file(
+00008870: 746f 706f 6c6f 6779 5f66 696c 6529 0a0a  topology_file)..
+00008880: 2020 2020 2320 4f70 656e 2061 6e64 2072      # Open and r
+00008890: 6561 6420 5941 4d4c 2074 6f70 6f6c 6f67  ead YAML topolog
+000088a0: 7920 6669 6c65 0a20 2020 2074 6f70 6f6c  y file.    topol
+000088b0: 6f67 795f 7961 6d6c 203d 205f 7265 6164  ogy_yaml = _read
+000088c0: 5f79 616d 6c5f 746f 706f 6c6f 6779 5f66  _yaml_topology_f
+000088d0: 696c 6528 746f 706f 6c6f 6779 5f66 696c  ile(topology_fil
+000088e0: 6529 0a0a 2020 2020 2320 5570 6461 7465  e)..    # Update
+000088f0: 2074 6f70 6f6c 6f67 7920 7769 7468 2074   topology with t
+00008900: 6865 2041 5049 0a20 2020 2028 746f 706f  he API.    (topo
+00008910: 6c6f 6779 5f79 616d 6c2c 2064 6f6d 6169  logy_yaml, domai
+00008920: 6e73 2920 3d20 746f 706f 6c6f 6779 5f61  ns) = topology_a
+00008930: 6464 5f64 6761 280a 2020 2020 2020 2020  dd_dga(.        
+00008940: 746f 706f 6c6f 6779 5f79 616d 6c2c 2061  topology_yaml, a
+00008950: 6c67 6f72 6974 686d 2c20 7377 6974 6368  lgorithm, switch
+00008960: 5f6e 616d 652c 206e 756d 6265 722c 2072  _name, number, r
+00008970: 6573 6f75 7263 6573 5f64 6972 0a20 2020  esources_dir.   
+00008980: 2029 0a0a 2020 2020 7265 7475 726e 2074   )..    return t
+00008990: 6f70 6f6c 6f67 795f 7961 6d6c 2c20 646f  opology_yaml, do
+000089a0: 6d61 696e 730a 0a0a 6465 6620 746f 706f  mains...def topo
+000089b0: 6c6f 6779 5f66 696c 655f 6164 645f 646e  logy_file_add_dn
+000089c0: 735f 7365 7276 6572 280a 2020 2020 746f  s_server(.    to
+000089d0: 706f 6c6f 6779 5f66 696c 653a 2073 7472  pology_file: str
+000089e0: 2c0a 2020 2020 7377 6974 6368 5f6e 616d  ,.    switch_nam
+000089f0: 653a 2073 7472 2c0a 2020 2020 7265 736f  e: str,.    reso
+00008a00: 7572 6365 735f 6469 723a 2073 7472 2c0a  urces_dir: str,.
+00008a10: 2920 2d3e 2054 7570 6c65 5b73 7472 2c20  ) -> Tuple[str, 
+00008a20: 7374 725d 3a0a 2020 2020 2222 2241 6464  str]:.    """Add
+00008a30: 2061 2044 4e53 2073 6572 7665 7220 746f   a DNS server to
+00008a40: 2061 2059 414d 4c20 746f 706f 6c6f 6779   a YAML topology
+00008a50: 2e0a 0a20 2020 203a 7265 7475 726e 3a20  ...    :return: 
+00008a60: 5468 6520 7570 6461 7465 6420 746f 706f  The updated topo
+00008a70: 6c6f 6779 2063 6f6e 7465 6e74 2061 6e64  logy content and
+00008a80: 2074 6865 2063 6f6e 7465 6e74 206f 6620   the content of 
+00008a90: 7468 6520 444e 5320 636f 6e66 6967 7572  the DNS configur
+00008aa0: 6174 696f 6e20 6669 6c65 2e0a 0a20 2020  ation file...   
+00008ab0: 203a 7061 7261 6d20 746f 706f 6c6f 6779   :param topology
+00008ac0: 5f66 696c 653a 2054 6865 2070 6174 6820  _file: The path 
+00008ad0: 746f 2061 2074 6f70 6f6c 6f67 7920 6669  to a topology fi
+00008ae0: 6c65 2e0a 2020 2020 3a70 6172 616d 2073  le..    :param s
+00008af0: 7769 7463 685f 6e61 6d65 3a20 5468 6520  witch_name: The 
+00008b00: 7377 6974 6368 206f 6e20 7768 6963 6820  switch on which 
+00008b10: 746f 2063 6f6e 6e65 6374 2074 6865 2064  to connect the d
+00008b20: 6f63 6b65 7220 444e 5320 7365 7276 6572  ocker DNS server
+00008b30: 206e 6f64 652e 0a20 2020 203a 7061 7261   node..    :para
+00008b40: 6d20 746f 706f 6c6f 6779 5f64 6972 3a20  m topology_dir: 
+00008b50: 5468 6520 7061 7468 2074 6f20 7265 736f  The path to reso
+00008b60: 7572 6365 7320 7468 6174 2077 696c 6c20  urces that will 
+00008b70: 6265 2070 7573 6865 6420 696e 746f 2074  be pushed into t
+00008b80: 6865 206e 6577 2064 6f63 6b65 7220 6e6f  he new docker no
+00008b90: 6465 2e0a 0a20 2020 2022 2222 0a0a 2020  de...    """..  
+00008ba0: 2020 2320 5661 6c69 6461 7465 0a0a 2020    # Validate..  
+00008bb0: 2020 2320 5661 6c69 6461 7465 2059 414d    # Validate YAM
+00008bc0: 4c20 746f 706f 6c6f 6779 2066 696c 650a  L topology file.
+00008bd0: 2020 2020 5f76 616c 6964 6174 655f 7961      _validate_ya
+00008be0: 6d6c 5f74 6f70 6f6c 6f67 795f 6669 6c65  ml_topology_file
+00008bf0: 2874 6f70 6f6c 6f67 795f 6669 6c65 290a  (topology_file).
+00008c00: 0a20 2020 2023 204f 7065 6e20 616e 6420  .    # Open and 
+00008c10: 7265 6164 2059 414d 4c20 746f 706f 6c6f  read YAML topolo
+00008c20: 6779 2066 696c 650a 2020 2020 746f 706f  gy file.    topo
+00008c30: 6c6f 6779 5f79 616d 6c20 3d20 5f72 6561  logy_yaml = _rea
+00008c40: 645f 7961 6d6c 5f74 6f70 6f6c 6f67 795f  d_yaml_topology_
+00008c50: 6669 6c65 2874 6f70 6f6c 6f67 795f 6669  file(topology_fi
+00008c60: 6c65 290a 0a20 2020 2023 2055 7064 6174  le)..    # Updat
+00008c70: 6520 746f 706f 6c6f 6779 2077 6974 6820  e topology with 
+00008c80: 7468 6520 4150 490a 2020 2020 2874 6f70  the API.    (top
+00008c90: 6f6c 6f67 795f 7961 6d6c 2c20 646e 735f  ology_yaml, dns_
+00008ca0: 636f 6e66 5f63 6f6e 7465 6e74 2920 3d20  conf_content) = 
+00008cb0: 746f 706f 6c6f 6779 5f61 6464 5f64 6e73  topology_add_dns
+00008cc0: 5f73 6572 7665 7228 0a20 2020 2020 2020  _server(.       
+00008cd0: 2074 6f70 6f6c 6f67 795f 7961 6d6c 2c20   topology_yaml, 
+00008ce0: 7377 6974 6368 5f6e 616d 652c 2072 6573  switch_name, res
+00008cf0: 6f75 7263 6573 5f64 6972 0a20 2020 2029  ources_dir.    )
+00008d00: 0a0a 2020 2020 7265 7475 726e 2074 6f70  ..    return top
+00008d10: 6f6c 6f67 795f 7961 6d6c 2c20 646e 735f  ology_yaml, dns_
+00008d20: 636f 6e66 5f63 6f6e 7465 6e74 0a0a 0a23  conf_content...#
+00008d30: 2323 0a23 2042 6173 6562 6f78 2068 656c  ##.# Basebox hel
+00008d40: 7065 7273 0a23 2323 0a0a 0a64 6566 205f  pers.###...def _
+00008d50: 6261 7365 626f 7865 735f 7665 7269 6679  baseboxes_verify
+00008d60: 5f72 6169 7365 5f65 7272 6f72 5f6d 7367  _raise_error_msg
+00008d70: 2872 6573 756c 743a 2064 6963 7429 202d  (result: dict) -
+00008d80: 3e20 4e6f 6e65 3a0a 2020 2020 2222 220a  > None:.    """.
+00008d90: 2020 2020 5261 6973 6520 616e 2065 7272      Raise an err
+00008da0: 6f72 206d 6573 7361 6765 2069 6620 6120  or message if a 
+00008db0: 7461 736b 2028 6567 2074 6865 2062 6173  task (eg the bas
+00008dc0: 6562 6f78 2076 6572 6966 6963 6174 696f  ebox verificatio
+00008dd0: 6e29 2066 6169 6c65 640a 0a20 2020 203a  n) failed..    :
+00008de0: 7061 7261 6d20 7265 7375 6c74 3a20 7468  param result: th
+00008df0: 6520 7265 7375 6c74 206f 6620 7468 6520  e result of the 
+00008e00: 7461 736b 0a0a 2020 2020 2222 220a 2020  task..    """.  
+00008e10: 2020 6572 726f 725f 6d73 6720 3d20 224e    error_msg = "N
+00008e20: 6f20 6572 726f 7220 6d65 7373 6167 6520  o error message 
+00008e30: 7265 7475 726e 6564 220a 0a20 2020 2069  returned"..    i
+00008e40: 6620 2265 7272 6f72 5f6d 7367 2220 696e  f "error_msg" in
+00008e50: 2072 6573 756c 743a 0a20 2020 2020 2020   result:.       
+00008e60: 2065 7272 6f72 5f6d 7367 203d 2072 6573   error_msg = res
+00008e70: 756c 745b 2265 7272 6f72 5f6d 7367 225d  ult["error_msg"]
+00008e80: 0a20 2020 2020 2020 2072 6169 7365 2045  .        raise E
+00008e90: 7863 6570 7469 6f6e 2865 7272 6f72 5f6d  xception(error_m
+00008ea0: 7367 290a 2020 2020 656c 7365 3a0a 2020  sg).    else:.  
+00008eb0: 2020 2020 2020 7261 6973 6520 4578 6365        raise Exce
+00008ec0: 7074 696f 6e28 6622 4e6f 2027 6572 726f  ption(f"No 'erro
+00008ed0: 725f 6d73 6727 206b 6579 2069 6e20 7265  r_msg' key in re
+00008ee0: 7375 6c74 3a20 7b72 6573 756c 747d 2229  sult: {result}")
+00008ef0: 0a0a 0a64 6566 205f 5f62 6173 6562 6f78  ...def __basebox
+00008f00: 6573 5f76 6572 6966 6963 6174 696f 6e5f  es_verification_
+00008f10: 7761 6974 5f75 6e74 696c 5f63 6f6d 706c  wait_until_compl
+00008f20: 6574 6528 0a20 2020 2074 6173 6b5f 6964  ete(.    task_id
+00008f30: 3a20 7374 722c 206c 6f67 5f73 7566 6669  : str, log_suffi
+00008f40: 783a 2073 7472 203d 204e 6f6e 652c 2074  x: str = None, t
+00008f50: 696d 656f 7574 3a20 696e 7420 3d20 3336  imeout: int = 36
+00008f60: 3030 0a29 202d 3e20 6469 6374 3a0a 2020  00.) -> dict:.  
+00008f70: 2020 2222 220a 2020 2020 5761 6974 2075    """.    Wait u
+00008f80: 6e74 696c 2074 6865 2076 6572 6966 6963  ntil the verific
+00008f90: 6174 696f 6e20 7461 736b 2072 6570 7265  ation task repre
+00008fa0: 7365 6e74 696e 6720 6279 2069 7473 2069  senting by its i
+00008fb0: 6420 6973 2063 6f6d 706c 6574 6564 0a0a  d is completed..
+00008fc0: 2020 2020 3a70 6172 616d 2074 6173 6b5f      :param task_
+00008fd0: 6964 3a20 7468 6520 7461 736b 2069 640a  id: the task id.
+00008fe0: 2020 2020 3a70 6172 616d 206c 6f67 5f73      :param log_s
+00008ff0: 7566 6669 783a 2077 6861 7420 746f 2069  uffix: what to i
+00009000: 6e73 6572 7420 696e 746f 2074 6865 206c  nsert into the l
+00009010: 6f67 0a20 2020 203a 7061 7261 6d20 7469  og.    :param ti
+00009020: 6d65 6f75 743a 2074 6865 2074 696d 656f  meout: the timeo
+00009030: 7574 2074 6f20 7374 6f70 2074 6865 2074  ut to stop the t
+00009040: 6173 6b0a 2020 2020 3a72 6574 7572 6e3a  ask.    :return:
+00009050: 2074 6865 2072 6573 756c 7420 6f66 2074   the result of t
+00009060: 6865 2062 6173 6562 6f78 2076 6572 6966  he basebox verif
+00009070: 6963 6174 696f 6e0a 0a20 2020 2022 2222  ication..    """
+00009080: 0a0a 2020 2020 7374 6172 745f 7469 6d65  ..    start_time
+00009090: 203d 2074 696d 652e 7469 6d65 2829 0a0a   = time.time()..
+000090a0: 2020 2020 6669 6e69 7368 6564 203d 2046      finished = F
+000090b0: 616c 7365 0a20 2020 2077 6869 6c65 206e  alse.    while n
+000090c0: 6f74 2028 6669 6e69 7368 6564 206f 7220  ot (finished or 
+000090d0: 2874 696d 652e 7469 6d65 2829 202d 2073  (time.time() - s
+000090e0: 7461 7274 5f74 696d 6529 203e 2074 696d  tart_time) > tim
+000090f0: 656f 7574 293a 0a20 2020 2020 2020 2074  eout):.        t
+00009100: 696d 652e 736c 6565 7028 3229 0a20 2020  ime.sleep(2).   
+00009110: 2020 2020 2063 7572 7265 6e74 5f74 696d       current_tim
+00009120: 6520 3d20 7469 6d65 2e74 696d 6528 290a  e = time.time().
+00009130: 2020 2020 2020 2020 656c 6170 7365 6420          elapsed 
+00009140: 3d20 696e 7428 6375 7272 656e 745f 7469  = int(current_ti
+00009150: 6d65 202d 2073 7461 7274 5f74 696d 6529  me - start_time)
+00009160: 0a20 2020 2020 2020 2069 6620 6c6f 675f  .        if log_
+00009170: 7375 6666 6978 2069 7320 6e6f 7420 4e6f  suffix is not No
+00009180: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00009190: 6c6f 6767 6572 2e69 6e66 6f28 0a20 2020  logger.info(.   
+000091a0: 2020 2020 2020 2020 2020 2020 2066 2220               f" 
+000091b0: 2020 5b2b 5d20 4375 7272 656e 746c 7920    [+] Currently 
+000091c0: 7665 7269 6679 696e 6720 7b6c 6f67 5f73  verifying {log_s
+000091d0: 7566 6669 787d 2066 6f72 207b 656c 6170  uffix} for {elap
+000091e0: 7365 647d 2073 6563 6f6e 6473 2028 7469  sed} seconds (ti
+000091f0: 6d65 6f75 7420 6174 207b 7469 6d65 6f75  meout at {timeou
+00009200: 747d 2073 6563 6f6e 6473 2922 0a20 2020  t} seconds)".   
+00009210: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00009220: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00009230: 2020 2020 206c 6f67 6765 722e 696e 666f       logger.info
+00009240: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00009250: 2020 6622 2020 205b 2b5d 2043 7572 7265    f"   [+] Curre
+00009260: 6e74 6c79 2072 756e 6e69 6e67 2074 6865  ntly running the
+00009270: 2076 6572 6966 6963 6174 696f 6e20 666f   verification fo
+00009280: 7220 7b65 6c61 7073 6564 7d20 7365 636f  r {elapsed} seco
+00009290: 6e64 7322 0a20 2020 2020 2020 2020 2020  nds".           
+000092a0: 2029 0a0a 2020 2020 2020 2020 7265 7375   )..        resu
+000092b0: 6c74 203d 205f 706f 7374 2822 2f62 6173  lt = _post("/bas
+000092c0: 6562 6f78 2f73 7461 7475 735f 7665 7269  ebox/status_veri
+000092d0: 6679 222c 2064 6174 613d 7b22 7461 736b  fy", data={"task
+000092e0: 5f69 6422 3a20 7461 736b 5f69 647d 290a  _id": task_id}).
+000092f0: 2020 2020 2020 2020 7265 7375 6c74 2e72          result.r
+00009300: 6169 7365 5f66 6f72 5f73 7461 7475 7328  aise_for_status(
+00009310: 290a 2020 2020 2020 2020 7265 7375 6c74  ).        result
+00009320: 203d 2072 6573 756c 742e 6a73 6f6e 2829   = result.json()
+00009330: 0a0a 2020 2020 2020 2020 6966 2022 7374  ..        if "st
+00009340: 6174 7573 2220 6e6f 7420 696e 2072 6573  atus" not in res
+00009350: 756c 743a 0a20 2020 2020 2020 2020 2020  ult:.           
+00009360: 2076 6572 6966 795f 6261 7365 626f 785f   verify_basebox_
+00009370: 7374 6f70 2874 6173 6b5f 6964 290a 2020  stop(task_id).  
+00009380: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00009390: 4578 6365 7074 696f 6e28 0a20 2020 2020  Exception(.     
+000093a0: 2020 2020 2020 2020 2020 2022 4572 726f             "Erro
+000093b0: 7220 6475 7269 6e67 2076 6572 6966 6963  r during verific
+000093c0: 6174 696f 6e20 6f70 6572 6174 696f 6e3a  ation operation:
+000093d0: 2075 6e65 7870 6563 7465 6420 7265 7370   unexpected resp
+000093e0: 6f6e 7365 2066 6f72 6d61 7420 6672 6f6d  onse format from
+000093f0: 2049 5420 5369 6d75 6c61 7469 6f6e 2041   IT Simulation A
+00009400: 5049 206f 6e20 2f62 6173 6562 6f78 6573  PI on /baseboxes
+00009410: 2f73 7461 7475 735f 7665 7269 6679 220a  /status_verify".
+00009420: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+00009430: 2020 2020 2020 2069 6620 7265 7375 6c74         if result
+00009440: 5b22 7374 6174 7573 225d 203d 3d20 2246  ["status"] == "F
+00009450: 494e 4953 4845 4422 3a0a 2020 2020 2020  INISHED":.      
+00009460: 2020 2020 2020 6669 6e69 7368 6564 203d        finished =
+00009470: 2054 7275 650a 0a20 2020 2069 6620 6e6f   True..    if no
+00009480: 7420 6669 6e69 7368 6564 3a0a 2020 2020  t finished:.    
+00009490: 2020 2020 6572 726f 725f 6d73 6720 3d20      error_msg = 
+000094a0: 6622 5b2d 5d20 556e 6162 6c65 2074 6f20  f"[-] Unable to 
+000094b0: 7465 726d 696e 6174 6520 6f70 6572 6174  terminate operat
+000094c0: 696f 6e20 6265 666f 7265 2074 696d 656f  ion before timeo
+000094d0: 7574 206f 6620 7b74 696d 656f 7574 7d20  ut of {timeout} 
+000094e0: 7365 636f 6e64 732e 2053 746f 7070 696e  seconds. Stoppin
+000094f0: 6720 6f70 6572 6174 696f 6e2e 220a 2020  g operation.".  
+00009500: 2020 2020 2020 7265 7375 6c74 203d 2076        result = v
+00009510: 6572 6966 795f 6261 7365 626f 785f 7374  erify_basebox_st
+00009520: 6f70 2874 6173 6b5f 6964 290a 2020 2020  op(task_id).    
+00009530: 2020 2020 7374 6f70 7065 6420 3d20 7265      stopped = re
+00009540: 7375 6c74 5b22 7374 6174 7573 225d 203d  sult["status"] =
+00009550: 3d20 2253 544f 5050 4544 220a 2020 2020  = "STOPPED".    
+00009560: 2020 2020 6966 2073 746f 7070 6564 3a0a      if stopped:.
+00009570: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00009580: 6c74 5b22 7265 7375 6c74 225d 203d 2064  lt["result"] = d
+00009590: 6963 7428 290a 2020 2020 2020 2020 2020  ict().          
+000095a0: 2020 7265 7375 6c74 5b22 7375 6363 6573    result["succes
+000095b0: 7322 5d20 3d20 4661 6c73 650a 2020 2020  s"] = False.    
+000095c0: 2020 2020 2020 2020 7265 7375 6c74 5b22          result["
+000095d0: 6572 726f 725f 6d73 6722 5d20 3d20 6572  error_msg"] = er
+000095e0: 726f 725f 6d73 670a 2020 2020 2020 2020  ror_msg.        
+000095f0: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+00009600: 740a 2020 2020 2020 2020 656c 7365 3a0a  t.        else:.
+00009610: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00009620: 6520 4578 6365 7074 696f 6e28 2255 6e61  e Exception("Una
+00009630: 626c 6520 746f 2073 746f 7020 7665 7269  ble to stop veri
+00009640: 6669 6361 7469 6f6e 2074 6173 6b20 6166  fication task af
+00009650: 7465 7220 7469 6d65 6f75 7422 290a 0a20  ter timeout").. 
+00009660: 2020 2072 6573 756c 7420 3d20 5f70 6f73     result = _pos
+00009670: 7428 222f 6261 7365 626f 782f 7265 7375  t("/basebox/resu
+00009680: 6c74 5f76 6572 6966 7922 2c20 6461 7461  lt_verify", data
+00009690: 3d7b 2274 6173 6b5f 6964 223a 2074 6173  ={"task_id": tas
+000096a0: 6b5f 6964 7d29 0a20 2020 2072 6573 756c  k_id}).    resul
+000096b0: 742e 7261 6973 655f 666f 725f 7374 6174  t.raise_for_stat
+000096c0: 7573 2829 0a20 2020 2072 6573 756c 7420  us().    result 
+000096d0: 3d20 7265 7375 6c74 2e6a 736f 6e28 290a  = result.json().
+000096e0: 0a20 2020 2073 7563 6365 7373 203d 2072  .    success = r
+000096f0: 6573 756c 745b 2273 7461 7475 7322 5d20  esult["status"] 
+00009700: 3d3d 2022 4649 4e49 5348 4544 2220 616e  == "FINISHED" an
+00009710: 6420 7265 7375 6c74 5b22 7375 6363 6573  d result["succes
+00009720: 7322 5d20 6973 2054 7275 650a 0a20 2020  s"] is True..   
+00009730: 2069 6620 6e6f 7420 7375 6363 6573 733a   if not success:
+00009740: 0a20 2020 2020 2020 2065 7272 6f72 5f6d  .        error_m
+00009750: 7367 203d 2072 6573 756c 745b 2265 7272  sg = result["err
+00009760: 6f72 5f6d 7367 225d 0a20 2020 2020 2020  or_msg"].       
+00009770: 206c 6f67 6765 722e 6572 726f 7228 0a20   logger.error(. 
+00009780: 2020 2020 2020 2020 2020 2066 225b 2d5d             f"[-]
+00009790: 2054 6865 2062 6173 6562 6f78 2076 6572   The basebox ver
+000097a0: 6966 6963 6174 696f 6e20 7761 7320 6578  ification was ex
+000097b0: 6563 7574 6564 2077 6974 6820 6572 726f  ecuted with erro
+000097c0: 7228 7329 3a20 7b65 7272 6f72 5f6d 7367  r(s): {error_msg
+000097d0: 7d22 0a20 2020 2020 2020 2029 0a0a 2020  }".        )..  
+000097e0: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
+000097f0: 0a0a 6465 6620 5f5f 7761 6974 5f66 6f72  ..def __wait_for
+00009800: 5f74 6865 5f6f 7065 7261 7469 6f6e 5f74  _the_operation_t
+00009810: 6f5f 7374 6172 7428 7461 736b 5f69 643a  o_start(task_id:
+00009820: 2073 7472 2920 2d3e 2062 6f6f 6c3a 0a20   str) -> bool:. 
+00009830: 2020 2022 2222 0a20 2020 2057 6169 7420     """.    Wait 
+00009840: 666f 7220 6120 7461 736b 2074 6f20 7374  for a task to st
+00009850: 6172 740a 2020 2020 3a70 6172 616d 2074  art.    :param t
+00009860: 6173 6b5f 6964 3a20 7468 6520 7461 736b  ask_id: the task
+00009870: 2069 640a 2020 2020 3a72 6574 7572 6e3a   id.    :return:
+00009880: 2049 7320 7468 6520 7461 736b 2072 756e   Is the task run
+00009890: 6e69 6e67 0a20 2020 2022 2222 0a0a 2020  ning.    """..  
+000098a0: 2020 7275 6e6e 696e 6720 3d20 4661 6c73    running = Fals
+000098b0: 650a 2020 2020 7469 6d65 6f75 7420 3d20  e.    timeout = 
+000098c0: 3130 0a20 2020 2073 7461 7274 5f74 696d  10.    start_tim
+000098d0: 6520 3d20 7469 6d65 2e74 696d 6528 290a  e = time.time().
+000098e0: 2020 2020 7768 696c 6520 6e6f 7420 2872      while not (r
+000098f0: 756e 6e69 6e67 206f 7220 2874 696d 652e  unning or (time.
+00009900: 7469 6d65 2829 202d 2073 7461 7274 5f74  time() - start_t
+00009910: 696d 6529 203e 2074 696d 656f 7574 293a  ime) > timeout):
+00009920: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+00009930: 3d20 5f70 6f73 7428 222f 6261 7365 626f  = _post("/basebo
+00009940: 782f 7374 6174 7573 5f76 6572 6966 7922  x/status_verify"
+00009950: 2c20 6461 7461 3d7b 2274 6173 6b5f 6964  , data={"task_id
+00009960: 223a 2074 6173 6b5f 6964 7d29 0a20 2020  ": task_id}).   
+00009970: 2020 2020 2072 6573 756c 742e 7261 6973       result.rais
+00009980: 655f 666f 725f 7374 6174 7573 2829 0a20  e_for_status(). 
+00009990: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+000099a0: 7265 7375 6c74 2e6a 736f 6e28 290a 2020  result.json().  
+000099b0: 2020 2020 2020 7275 6e6e 696e 6720 3d20        running = 
+000099c0: 7265 7375 6c74 5b22 7374 6174 7573 225d  result["status"]
+000099d0: 203d 3d20 2252 554e 4e49 4e47 220a 2020   == "RUNNING".  
+000099e0: 2020 2020 2020 7469 6d65 2e73 6c65 6570        time.sleep
+000099f0: 2831 290a 0a20 2020 2069 6620 6e6f 7420  (1)..    if not 
+00009a00: 7275 6e6e 696e 673a 0a20 2020 2020 2020  running:.       
+00009a10: 206c 6f67 6765 722e 6572 726f 7228 0a20   logger.error(. 
+00009a20: 2020 2020 2020 2020 2020 2066 225b 2d5d             f"[-]
+00009a30: 2055 6e61 626c 6520 746f 2073 7461 7274   Unable to start
+00009a40: 206f 7065 7261 7469 6f6e 2062 6566 6f72   operation befor
+00009a50: 6520 7469 6d65 6f75 7420 6f66 207b 7469  e timeout of {ti
+00009a60: 6d65 6f75 747d 2073 6563 6f6e 6473 220a  meout} seconds".
+00009a70: 2020 2020 2020 2020 290a 0a20 2020 2072          )..    r
+00009a80: 6574 7572 6e20 7275 6e6e 696e 670a 0a0a  eturn running...
+00009a90: 6465 6620 5f5f 6861 6e64 6c65 5f77 6169  def __handle_wai
+00009aa0: 745f 6261 7365 626f 785f 7665 7269 6679  t_basebox_verify
+00009ab0: 280a 2020 2020 7761 6974 3a20 626f 6f6c  (.    wait: bool
+00009ac0: 2c20 7461 736b 5f69 643a 2073 7472 2c20  , task_id: str, 
+00009ad0: 6c6f 675f 7375 6666 6978 3a20 7374 722c  log_suffix: str,
+00009ae0: 2074 696d 656f 7574 3a20 696e 7420 3d20   timeout: int = 
+00009af0: 3336 3030 0a29 202d 3e20 626f 6f6c 3a0a  3600.) -> bool:.
+00009b00: 2020 2020 2222 220a 0a20 2020 203a 7061      """..    :pa
+00009b10: 7261 6d20 7761 6974 3a20 5761 6974 2066  ram wait: Wait f
+00009b20: 6f72 2074 6865 206f 7065 7261 7469 6f6e  or the operation
+00009b30: 2074 6f20 6265 2063 6f6d 706c 6574 6564   to be completed
+00009b40: 2069 6e20 6261 636b 656e 640a 2020 2020   in backend.    
+00009b50: 3a70 6172 616d 2074 6173 6b5f 6964 3a20  :param task_id: 
+00009b60: 7468 6520 7461 736b 2069 640a 2020 2020  the task id.    
+00009b70: 3a70 6172 616d 206c 6f67 5f73 7566 6669  :param log_suffi
+00009b80: 783a 2074 6865 2073 7472 696e 6720 746f  x: the string to
+00009b90: 2062 6520 696e 7365 7274 6564 2069 6e20   be inserted in 
+00009ba0: 7468 6520 6c6f 670a 2020 2020 3a70 6172  the log.    :par
+00009bb0: 616d 2074 696d 656f 7574 3a20 7468 6520  am timeout: the 
+00009bc0: 7469 6d65 206c 696d 6974 2062 6566 6f72  time limit befor
+00009bd0: 6520 7374 6f70 7069 6e67 2074 6865 2074  e stopping the t
+00009be0: 6173 6b0a 2020 2020 3a72 6574 7572 6e3a  ask.    :return:
+00009bf0: 2074 6865 2072 6573 756c 7420 6f66 2074   the result of t
+00009c00: 6865 2076 6572 6966 6963 6174 696f 6e0a  he verification.
+00009c10: 2020 2020 2222 220a 2020 2020 7375 6363      """.    succ
+00009c20: 6573 7320 3d20 5472 7565 0a0a 2020 2020  ess = True..    
+00009c30: 6966 2077 6169 743a 0a20 2020 2020 2020  if wait:.       
+00009c40: 2023 2057 6169 7420 666f 7220 7468 6520   # Wait for the 
+00009c50: 6f70 6572 6174 696f 6e20 746f 2062 6520  operation to be 
+00009c60: 636f 6d70 6c65 7465 6420 696e 2062 6163  completed in bac
+00009c70: 6b65 6e64 0a0a 2020 2020 2020 2020 7265  kend..        re
+00009c80: 7375 6c74 203d 205f 5f62 6173 6562 6f78  sult = __basebox
+00009c90: 6573 5f76 6572 6966 6963 6174 696f 6e5f  es_verification_
+00009ca0: 7761 6974 5f75 6e74 696c 5f63 6f6d 706c  wait_until_compl
+00009cb0: 6574 6528 0a20 2020 2020 2020 2020 2020  ete(.           
+00009cc0: 2074 6173 6b5f 6964 3d74 6173 6b5f 6964   task_id=task_id
+00009cd0: 2c20 6c6f 675f 7375 6666 6978 3d6c 6f67  , log_suffix=log
+00009ce0: 5f73 7566 6669 782c 2074 696d 656f 7574  _suffix, timeout
+00009cf0: 3d74 696d 656f 7574 0a20 2020 2020 2020  =timeout.       
+00009d00: 2029 0a0a 2020 2020 2020 2020 6669 6e69   )..        fini
+00009d10: 7368 6564 203d 2022 7374 6174 7573 2220  shed = "status" 
+00009d20: 696e 2072 6573 756c 7420 616e 6420 7265  in result and re
+00009d30: 7375 6c74 5b22 7374 6174 7573 225d 203d  sult["status"] =
+00009d40: 3d20 2246 494e 4953 4845 4422 0a20 2020  = "FINISHED".   
+00009d50: 2020 2020 2073 7563 6365 7373 203d 2066       success = f
+00009d60: 696e 6973 6865 640a 0a20 2020 2020 2020  inished..       
+00009d70: 2069 6620 7375 6363 6573 733a 0a20 2020   if success:.   
+00009d80: 2020 2020 2020 2020 2069 6620 2272 6573           if "res
+00009d90: 756c 7422 2069 6e20 7265 7375 6c74 3a0a  ult" in result:.
+00009da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009db0: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
+00009dc0: 2020 2020 2020 2069 6620 6e6f 7420 7375         if not su
+00009dd0: 6363 6573 733a 0a20 2020 2020 2020 2020  ccess:.         
+00009de0: 2020 205f 6261 7365 626f 7865 735f 7665     _baseboxes_ve
+00009df0: 7269 6679 5f72 6169 7365 5f65 7272 6f72  rify_raise_error
+00009e00: 5f6d 7367 2872 6573 756c 7429 0a0a 2020  _msg(result)..  
+00009e10: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00009e20: 2320 7761 6974 2066 6f72 2074 6865 206f  # wait for the o
+00009e30: 7065 7261 7469 6f6e 2074 6f20 7374 6172  peration to star
+00009e40: 740a 2020 2020 2020 2020 7275 6e6e 696e  t.        runnin
+00009e50: 6720 3d20 5f5f 7761 6974 5f66 6f72 5f74  g = __wait_for_t
+00009e60: 6865 5f6f 7065 7261 7469 6f6e 5f74 6f5f  he_operation_to_
+00009e70: 7374 6172 7428 7461 736b 5f69 6429 0a0a  start(task_id)..
+00009e80: 2020 2020 2020 2020 6966 206e 6f74 2072          if not r
+00009e90: 756e 6e69 6e67 3a0a 2020 2020 2020 2020  unning:.        
+00009ea0: 2020 2020 7375 6363 6573 7320 3d20 4661      success = Fa
+00009eb0: 6c73 650a 0a20 2020 2072 6574 7572 6e20  lse..    return 
+00009ec0: 7375 6363 6573 730a 0a0a 2320 2d2d 2d2d  success...# ----
+00009ed0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00009ee0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00009ef0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00009f00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00009f10: 2d2d 2d2d 2d2d 2023 0a23 2043 6f72 6520  ------ #.# Core 
+00009f20: 4150 490a 2320 2d2d 2d2d 2d2d 2d2d 2d2d  API.# ----------
+00009f30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00009f40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00009f50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00009f60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00009f70: 2023 0a0a 0a64 6566 2067 6574 5f76 6572   #...def get_ver
+00009f80: 7369 6f6e 2829 202d 3e20 7374 723a 0a20  sion() -> str:. 
+00009f90: 2020 2022 2222 5265 7475 726e 2049 5420     """Return IT 
+00009fa0: 5369 6d75 6c61 7469 6f6e 2041 5049 2076  Simulation API v
+00009fb0: 6572 7369 6f6e 2e0a 0a20 2020 203a 7265  ersion...    :re
+00009fc0: 7475 726e 3a20 5265 7475 726e 2076 6572  turn: Return ver
+00009fd0: 7369 6f6e 2e0a 0a20 2020 2022 2222 0a0a  sion...    """..
+00009fe0: 2020 2020 7265 7375 6c74 203d 205f 6765      result = _ge
+00009ff0: 7428 222f 7369 6d75 6c61 7469 6f6e 2f76  t("/simulation/v
+0000a000: 6572 7369 6f6e 2229 0a0a 2020 2020 6966  ersion")..    if
+0000a010: 2072 6573 756c 742e 7374 6174 7573 5f63   result.status_c
+0000a020: 6f64 6520 213d 2032 3030 3a0a 2020 2020  ode != 200:.    
+0000a030: 2020 2020 5f68 616e 646c 655f 6572 726f      _handle_erro
+0000a040: 7228 7265 7375 6c74 2c20 2243 616e 6e6f  r(result, "Canno
+0000a050: 7420 7265 7472 6965 7665 2043 6f72 6520  t retrieve Core 
+0000a060: 4150 4920 7665 7273 696f 6e22 290a 0a20  API version").. 
+0000a070: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+0000a080: 2e6a 736f 6e28 290a 0a0a 6465 6620 7265  .json()...def re
+0000a090: 7365 7428 6465 6c65 7465 5f63 6f6d 7075  set(delete_compu
+0000a0a0: 7465 5f73 6572 7665 7273 3a20 626f 6f6c  te_servers: bool
+0000a0b0: 203d 2046 616c 7365 2920 2d3e 2041 6e79   = False) -> Any
+0000a0c0: 3a0a 2020 2020 2222 220a 2020 2020 5265  :.    """.    Re
+0000a0d0: 7365 7420 7468 6520 4954 2053 696d 756c  set the IT Simul
+0000a0e0: 6174 696f 6e20 696e 6672 6173 7472 7563  ation infrastruc
+0000a0f0: 7475 7265 0a0a 2020 2020 5468 6973 2068  ture..    This h
+0000a100: 6173 2074 6865 2066 6f6c 6c6f 7769 6e67  as the following
+0000a110: 2065 6666 6563 743a 0a20 2020 202d 2063   effect:.    - c
+0000a120: 6c65 616e 2074 6865 2064 6174 6162 6173  lean the databas
+0000a130: 6520 616e 6420 7265 2d70 6f70 756c 6174  e and re-populat
+0000a140: 6520 6974 2077 6974 6820 7374 6174 6963  e it with static
+0000a150: 2069 6e66 6f20 2862 6173 6562 6f78 6573   info (baseboxes
+0000a160: 2c20 726f 6c65 732e 2e2e 290a 2020 2020  , roles...).    
+0000a170: 2d20 6279 2064 6566 6175 742c 2074 6865  - by defaut, the
+0000a180: 2074 6162 6c65 206f 6620 636f 6d70 7574   table of comput
+0000a190: 6520 7365 7276 6572 7320 6973 206b 6570  e servers is kep
+0000a1a0: 742c 2062 7574 2060 6465 6c65 7465 5f63  t, but `delete_c
+0000a1b0: 6f6d 7075 7465 5f73 6572 7665 7273 3d54  ompute_servers=T
+0000a1c0: 7275 6560 2063 6861 6e67 6573 2074 6861  rue` changes tha
+0000a1d0: 7420 6265 6861 7669 6f72 0a20 2020 202d  t behavior.    -
+0000a1e0: 2072 6573 6574 2074 6865 2073 696d 756c   reset the simul
+0000a1f0: 6174 696f 6e20 6d61 6e61 6765 720a 2020  ation manager.  
+0000a200: 2020 2d20 7265 7365 7420 7468 6520 636f    - reset the co
+0000a210: 6d70 7574 6520 7365 7276 6572 7320 2873  mpute servers (s
+0000a220: 746f 7020 564d 7320 616e 6420 646f 636b  top VMs and dock
+0000a230: 6572 732c 2072 6573 6574 206e 6574 776f  ers, reset netwo
+0000a240: 726b 732c 202e 2e2e 290a 0a20 2020 203a  rks, ...)..    :
+0000a250: 7265 7475 726e 3a20 4120 6d65 7373 6167  return: A messag
+0000a260: 6520 7465 6c6c 696e 6720 686f 7720 7468  e telling how th
+0000a270: 6520 6f70 6572 6174 696f 6e20 6578 6563  e operation exec
+0000a280: 7574 6564 2e0a 0a20 2020 203a 7061 7261  uted...    :para
+0000a290: 6d20 6465 6c65 7465 5f63 6f6d 7075 7465  m delete_compute
+0000a2a0: 5f73 6572 7665 7273 3a20 4120 626f 6f6c  _servers: A bool
+0000a2b0: 6561 6e20 7465 6c6c 696e 6720 6966 2077  ean telling if w
+0000a2c0: 6520 6e65 6564 2074 6f20 6465 6c65 7465  e need to delete
+0000a2d0: 206b 6e6f 776e 2063 6f6d 7075 7465 2073   known compute s
+0000a2e0: 6572 7665 7273 2e0a 0a20 2020 2022 2222  ervers...    """
+0000a2f0: 0a20 2020 2070 6172 616d 7320 3d20 7b7d  .    params = {}
+0000a300: 0a20 2020 2069 6620 6465 6c65 7465 5f63  .    if delete_c
+0000a310: 6f6d 7075 7465 5f73 6572 7665 7273 3a0a  ompute_servers:.
+0000a320: 2020 2020 2020 2020 7061 7261 6d73 203d          params =
+0000a330: 207b 2264 656c 6574 655f 636f 6d70 7574   {"delete_comput
+0000a340: 655f 7365 7276 6572 735f 6672 6f6d 5f64  e_servers_from_d
+0000a350: 6222 3a20 6465 6c65 7465 5f63 6f6d 7075  b": delete_compu
+0000a360: 7465 5f73 6572 7665 7273 7d0a 0a20 2020  te_servers}..   
+0000a370: 2072 6573 756c 7420 3d20 5f64 656c 6574   result = _delet
+0000a380: 6528 222f 7369 6d75 6c61 7469 6f6e 2f63  e("/simulation/c
+0000a390: 6f6d 7075 7465 5f69 6e66 7261 7374 7275  ompute_infrastru
+0000a3a0: 6374 7572 655f 7265 7365 7422 2c20 7061  cture_reset", pa
+0000a3b0: 7261 6d73 3d70 6172 616d 7329 0a0a 2020  rams=params)..  
+0000a3c0: 2020 6966 2072 6573 756c 742e 7374 6174    if result.stat
+0000a3d0: 7573 5f63 6f64 6520 213d 2032 3030 3a0a  us_code != 200:.
+0000a3e0: 2020 2020 2020 2020 5f68 616e 646c 655f          _handle_
+0000a3f0: 6572 726f 7228 7265 7375 6c74 2c20 2243  error(result, "C
+0000a400: 616e 6e6f 7420 7265 7365 7420 7369 6d75  annot reset simu
+0000a410: 6c61 7469 6f6e 2069 6e66 7261 7374 7275  lation infrastru
+0000a420: 6374 7572 6522 290a 0a20 2020 2072 6574  cture")..    ret
+0000a430: 7572 6e20 7265 7375 6c74 2e6a 736f 6e28  urn result.json(
+0000a440: 290a 0a0a 6465 6620 5f63 7265 6174 655f  )...def _create_
+0000a450: 6f72 5f65 7874 656e 645f 7369 6d75 6c61  or_extend_simula
+0000a460: 7469 6f6e 280a 2020 2020 7369 6d75 6c61  tion(.    simula
+0000a470: 7469 6f6e 5f64 6963 743a 2064 6963 742c  tion_dict: dict,
+0000a480: 0a20 2020 2069 645f 7369 6d75 6c61 7469  .    id_simulati
+0000a490: 6f6e 3a20 696e 7420 3d20 4e6f 6e65 2c0a  on: int = None,.
+0000a4a0: 2020 2020 616c 6c6f 6361 7469 6f6e 5f73      allocation_s
+0000a4b0: 7472 6174 6567 793a 204f 7074 696f 6e61  trategy: Optiona
+0000a4c0: 6c5b 7374 725d 203d 204e 6f6e 652c 0a29  l[str] = None,.)
+0000a4d0: 202d 3e20 5475 706c 655b 696e 742c 204c   -> Tuple[int, L
+0000a4e0: 6973 745b 7374 725d 5d3a 0a20 2020 2022  ist[str]]:.    "
+0000a4f0: 2222 4372 6561 7465 2061 2073 696d 756c  ""Create a simul
+0000a500: 6174 696f 6e2c 206f 7220 6578 7465 6e64  ation, or extend
+0000a510: 2061 6e20 6578 6973 7469 6e67 2073 696d   an existing sim
+0000a520: 756c 6174 696f 6e20 7769 7468 206e 6577  ulation with new
+0000a530: 0a20 2020 206e 6f64 6573 2061 6e64 206c  .    nodes and l
+0000a540: 696e 6b73 2c20 616e 6420 7265 7475 726e  inks, and return
+0000a550: 2061 2073 696d 756c 6174 696f 6e20 4944   a simulation ID
+0000a560: 2e22 2222 0a0a 2020 2020 2320 4765 7420  ."""..    # Get 
+0000a570: 7468 6520 7061 7468 7320 6966 2073 6f6d  the paths if som
+0000a580: 6520 6861 7665 2062 6565 6e20 7072 6f76  e have been prov
+0000a590: 6964 6564 0a20 2020 2072 6573 6f75 7263  ided.    resourc
+0000a5a0: 6573 5f70 6174 6873 203d 2073 696d 756c  es_paths = simul
+0000a5b0: 6174 696f 6e5f 6469 6374 2e70 6f70 2822  ation_dict.pop("
+0000a5c0: 7265 736f 7572 6365 735f 7061 7468 7322  resources_paths"
+0000a5d0: 2c20 5b5d 290a 0a20 2020 2064 6174 6120  , [])..    data 
+0000a5e0: 3d20 6a73 6f6e 2e64 756d 7073 2873 696d  = json.dumps(sim
+0000a5f0: 756c 6174 696f 6e5f 6469 6374 290a 0a20  ulation_dict).. 
+0000a600: 2020 2023 2043 7265 6174 696f 6e20 6f66     # Creation of
+0000a610: 2061 2066 6f6c 6465 7220 636f 6e74 6169   a folder contai
+0000a620: 6e69 6e67 2061 6c6c 2074 6865 2072 6573  ning all the res
+0000a630: 6f75 7263 6573 2c20 7468 6973 2066 6f6c  ources, this fol
+0000a640: 6465 7220 7769 6c6c 2074 6865 6e20 6265  der will then be
+0000a650: 207a 6970 7065 640a 2020 2020 7769 7468   zipped.    with
+0000a660: 2054 656d 706f 7261 7279 4469 7265 6374   TemporaryDirect
+0000a670: 6f72 7928 7072 6566 6978 3d22 6379 6265  ory(prefix="cybe
+0000a680: 725f 7261 6e67 655f 6372 5f63 6f72 655f  r_range_cr_core_
+0000a690: 7265 736f 7572 6365 7322 2920 6173 206d  resources") as m
+0000a6a0: 6169 6e5f 7265 736f 7572 6365 733a 0a20  ain_resources:. 
+0000a6b0: 2020 2020 2020 2023 2063 6f70 7920 616c         # copy al
+0000a6c0: 6c20 7265 736f 7572 6365 7320 696e 2074  l resources in t
+0000a6d0: 6865 206d 6169 6e20 7465 6d70 6f72 6172  he main temporar
+0000a6e0: 7920 666f 6c64 6572 0a20 2020 2020 2020  y folder.       
+0000a6f0: 2066 6f72 2072 6573 6f75 7263 6520 696e   for resource in
+0000a700: 2072 6573 6f75 7263 6573 5f70 6174 6873   resources_paths
+0000a710: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+0000a720: 206f 732e 7061 7468 2e69 7364 6972 2872   os.path.isdir(r
+0000a730: 6573 6f75 7263 6529 3a0a 2020 2020 2020  esource):.      
+0000a740: 2020 2020 2020 2020 2020 7368 7574 696c            shutil
+0000a750: 2e63 6f70 7974 7265 6528 0a20 2020 2020  .copytree(.     
+0000a760: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000a770: 6573 6f75 7263 652c 0a20 2020 2020 2020  esource,.       
+0000a780: 2020 2020 2020 2020 2020 2020 206f 732e               os.
+0000a790: 7061 7468 2e6a 6f69 6e28 0a20 2020 2020  path.join(.     
+0000a7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a7b0: 2020 206d 6169 6e5f 7265 736f 7572 6365     main_resource
+0000a7c0: 732c 206f 732e 7061 7468 2e62 6173 656e  s, os.path.basen
+0000a7d0: 616d 6528 6f73 2e70 6174 682e 6e6f 726d  ame(os.path.norm
+0000a7e0: 7061 7468 2872 6573 6f75 7263 6529 290a  path(resource)).
+0000a7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a800: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
+0000a810: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000a820: 2020 2020 2065 6c69 6620 6f73 2e70 6174       elif os.pat
+0000a830: 682e 6973 6669 6c65 2872 6573 6f75 7263  h.isfile(resourc
+0000a840: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
+0000a850: 2020 2020 7368 7574 696c 2e63 6f70 7966      shutil.copyf
+0000a860: 696c 6528 0a20 2020 2020 2020 2020 2020  ile(.           
+0000a870: 2020 2020 2020 2020 2072 6573 6f75 7263           resourc
+0000a880: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+0000a890: 2020 2020 2020 206f 732e 7061 7468 2e6a         os.path.j
+0000a8a0: 6f69 6e28 0a20 2020 2020 2020 2020 2020  oin(.           
+0000a8b0: 2020 2020 2020 2020 2020 2020 206d 6169               mai
+0000a8c0: 6e5f 7265 736f 7572 6365 732c 206f 732e  n_resources, os.
+0000a8d0: 7061 7468 2e62 6173 656e 616d 6528 6f73  path.basename(os
+0000a8e0: 2e70 6174 682e 6e6f 726d 7061 7468 2872  .path.normpath(r
+0000a8f0: 6573 6f75 7263 6529 290a 2020 2020 2020  esource)).      
+0000a900: 2020 2020 2020 2020 2020 2020 2020 292c                ),
+0000a910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a920: 2029 0a20 2020 2020 2020 2020 2020 2065   ).            e
+0000a930: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000a940: 2020 2020 2072 6169 7365 2045 7863 6570       raise Excep
+0000a950: 7469 6f6e 2866 2243 616e 206e 6f74 2063  tion(f"Can not c
+0000a960: 6f70 7920 7b72 6573 6f75 7263 657d 2229  opy {resource}")
+0000a970: 0a0a 2020 2020 2020 2020 2320 5765 2068  ..        # We h
+0000a980: 6176 6520 746f 2063 7265 6174 6520 6120  ave to create a 
+0000a990: 6e65 7720 7465 6d70 6f72 6172 7920 666f  new temporary fo
+0000a9a0: 6c64 6572 2074 6f20 686f 7374 2074 6865  lder to host the
+0000a9b0: 2061 7263 6869 7665 0a20 2020 2020 2020   archive.       
+0000a9c0: 2077 6974 6820 5465 6d70 6f72 6172 7944   with TemporaryD
+0000a9d0: 6972 6563 746f 7279 2870 7265 6669 783d  irectory(prefix=
+0000a9e0: 2263 7962 6572 5f72 616e 6765 5f63 725f  "cyber_range_cr_
+0000a9f0: 636f 7265 5f61 7263 6869 7665 2229 2061  core_archive") a
+0000aa00: 7320 7465 6d70 5f64 6972 3a0a 2020 2020  s temp_dir:.    
+0000aa10: 2020 2020 2020 2020 6966 2072 6573 6f75          if resou
+0000aa20: 7263 6573 5f70 6174 6873 3a0a 2020 2020  rces_paths:.    
+0000aa30: 2020 2020 2020 2020 2020 2020 7a69 705f              zip_
+0000aa40: 6669 6c65 5f6e 616d 6520 3d20 5f7a 6970  file_name = _zip
+0000aa50: 5f72 6573 6f75 7263 6573 286d 6169 6e5f  _resources(main_
+0000aa60: 7265 736f 7572 6365 732c 2074 656d 705f  resources, temp_
+0000aa70: 6469 7229 0a20 2020 2020 2020 2020 2020  dir).           
+0000aa80: 2020 2020 2072 6573 6f75 7263 6573 5f66       resources_f
+0000aa90: 696c 6520 3d20 6f70 656e 287a 6970 5f66  ile = open(zip_f
+0000aaa0: 696c 655f 6e61 6d65 2c20 2272 6222 290a  ile_name, "rb").
+0000aab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aac0: 6669 6c65 7320 3d20 7b22 7265 736f 7572  files = {"resour
+0000aad0: 6365 735f 6669 6c65 223a 2072 6573 6f75  ces_file": resou
+0000aae0: 7263 6573 5f66 696c 652c 2022 6461 7461  rces_file, "data
+0000aaf0: 223a 2064 6174 617d 0a20 2020 2020 2020  ": data}.       
+0000ab00: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000ab10: 2020 2020 2020 2020 2020 2072 6573 6f75             resou
+0000ab20: 7263 6573 5f66 696c 6520 3d20 4e6f 6e65  rces_file = None
+0000ab30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ab40: 2066 696c 6573 203d 207b 2264 6174 6122   files = {"data"
+0000ab50: 3a20 6461 7461 7d0a 0a20 2020 2020 2020  : data}..       
+0000ab60: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+0000ab70: 2020 2020 2020 2020 2020 6966 2069 645f            if id_
+0000ab80: 7369 6d75 6c61 7469 6f6e 2069 7320 4e6f  simulation is No
+0000ab90: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000aba0: 2020 2020 2020 2020 2320 4372 6561 7465          # Create
+0000abb0: 206e 6577 2073 696d 756c 6174 696f 6e0a   new simulation.
+0000abc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000abd0: 2020 2020 7265 7375 6c74 203d 205f 706f      result = _po
+0000abe0: 7374 280a 2020 2020 2020 2020 2020 2020  st(.            
+0000abf0: 2020 2020 2020 2020 2020 2020 222f 7369              "/si
+0000ac00: 6d75 6c61 7469 6f6e 2f22 2c0a 2020 2020  mulation/",.    
+0000ac10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac20: 2020 2020 6669 6c65 733d 6669 6c65 732c      files=files,
+0000ac30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ac40: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+0000ac50: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000ac60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac70: 2023 2045 7874 656e 6420 616e 2065 7869   # Extend an exi
+0000ac80: 7374 696e 6720 7369 6d75 6c61 7469 6f6e  sting simulation
+0000ac90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000aca0: 2020 2020 2072 6573 756c 7420 3d20 5f70       result = _p
+0000acb0: 6f73 7428 0a20 2020 2020 2020 2020 2020  ost(.           
+0000acc0: 2020 2020 2020 2020 2020 2020 2066 222f               f"/
+0000acd0: 7369 6d75 6c61 7469 6f6e 2f7b 6964 5f73  simulation/{id_s
+0000ace0: 696d 756c 6174 696f 6e7d 2f65 7874 656e  imulation}/exten
+0000acf0: 6422 2c0a 2020 2020 2020 2020 2020 2020  d",.            
+0000ad00: 2020 2020 2020 2020 2020 2020 6669 6c65              file
+0000ad10: 733d 6669 6c65 732c 0a20 2020 2020 2020  s=files,.       
+0000ad20: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+0000ad30: 2020 2020 2020 2020 2020 2066 696e 616c             final
+0000ad40: 6c79 3a0a 2020 2020 2020 2020 2020 2020  ly:.            
+0000ad50: 2020 2020 6966 2072 6573 6f75 7263 6573      if resources
+0000ad60: 5f66 696c 653a 0a20 2020 2020 2020 2020  _file:.         
+0000ad70: 2020 2020 2020 2020 2020 2072 6573 6f75             resou
+0000ad80: 7263 6573 5f66 696c 652e 636c 6f73 6528  rces_file.close(
+0000ad90: 290a 0a20 2020 2069 6620 6e6f 7420 6d61  )..    if not ma
+0000ada0: 696e 5f72 6573 6f75 7263 6573 3a0a 2020  in_resources:.  
+0000adb0: 2020 2020 2020 6966 2069 645f 7369 6d75        if id_simu
+0000adc0: 6c61 7469 6f6e 2069 7320 4e6f 6e65 3a0a  lation is None:.
+0000add0: 2020 2020 2020 2020 2020 2020 2320 4372              # Cr
+0000ade0: 6561 7465 206e 6577 2073 696d 756c 6174  eate new simulat
+0000adf0: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
+0000ae00: 7265 7375 6c74 203d 205f 706f 7374 280a  result = _post(.
+0000ae10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae20: 222f 7369 6d75 6c61 7469 6f6e 2f22 2c0a  "/simulation/",.
+0000ae30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae40: 6461 7461 3d64 6174 612c 0a20 2020 2020  data=data,.     
+0000ae50: 2020 2020 2020 2020 2020 2068 6561 6465             heade
+0000ae60: 7273 3d7b 2243 6f6e 7465 6e74 2d54 7970  rs={"Content-Typ
+0000ae70: 6522 3a20 2261 7070 6c69 6361 7469 6f6e  e": "application
+0000ae80: 2f6a 736f 6e22 7d2c 0a20 2020 2020 2020  /json"},.       
+0000ae90: 2020 2020 2029 0a20 2020 2020 2020 2065       ).        e
+0000aea0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000aeb0: 2023 2045 7874 656e 6420 616e 2065 7869   # Extend an exi
+0000aec0: 7374 696e 6720 7369 6d75 6c61 7469 6f6e  sting simulation
+0000aed0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+0000aee0: 756c 7420 3d20 5f70 6f73 7428 0a20 2020  ult = _post(.   
+0000aef0: 2020 2020 2020 2020 2020 2020 2066 222f               f"/
+0000af00: 7369 6d75 6c61 7469 6f6e 2f7b 6964 5f73  simulation/{id_s
+0000af10: 696d 756c 6174 696f 6e7d 2f65 7874 656e  imulation}/exten
+0000af20: 6422 2c0a 2020 2020 2020 2020 2020 2020  d",.            
+0000af30: 2020 2020 6461 7461 3d64 6174 612c 0a20      data=data,. 
+0000af40: 2020 2020 2020 2020 2020 2020 2020 2068                 h
+0000af50: 6561 6465 7273 3d7b 2243 6f6e 7465 6e74  eaders={"Content
+0000af60: 2d54 7970 6522 3a20 2261 7070 6c69 6361  -Type": "applica
+0000af70: 7469 6f6e 2f6a 736f 6e22 7d2c 0a20 2020  tion/json"},.   
+0000af80: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+0000af90: 6966 2072 6573 756c 742e 7374 6174 7573  if result.status
+0000afa0: 5f63 6f64 6520 213d 2032 3030 3a0a 2020  _code != 200:.  
+0000afb0: 2020 2020 2020 5f68 616e 646c 655f 6572        _handle_er
+0000afc0: 726f 7228 7265 7375 6c74 2c20 2243 616e  ror(result, "Can
+0000afd0: 6e6f 7420 706f 7374 2073 696d 756c 6174  not post simulat
+0000afe0: 696f 6e20 696e 666f 726d 6174 696f 6e20  ion information 
+0000aff0: 746f 2063 6f72 6520 4150 4922 290a 0a20  to core API").. 
+0000b000: 2020 2069 645f 7369 6d75 6c61 7469 6f6e     id_simulation
+0000b010: 203d 2072 6573 756c 742e 6a73 6f6e 2829   = result.json()
+0000b020: 5b22 6964 225d 0a20 2020 206e 6577 5f6e  ["id"].    new_n
+0000b030: 6f64 6573 203d 2072 6573 756c 742e 6a73  odes = result.js
+0000b040: 6f6e 2829 5b22 6e65 775f 6e6f 6465 7322  on()["new_nodes"
+0000b050: 5d0a 2020 2020 6c6f 6767 6572 2e69 6e66  ].    logger.inf
+0000b060: 6f28 6622 5b2b 5d20 4e65 7720 6e6f 6465  o(f"[+] New node
+0000b070: 7320 666f 7220 7369 6d75 6c61 7469 6f6e  s for simulation
+0000b080: 2069 6420 277b 6964 5f73 696d 756c 6174   id '{id_simulat
+0000b090: 696f 6e7d 273a 2027 7b6e 6577 5f6e 6f64  ion}': '{new_nod
+0000b0a0: 6573 7d27 2229 0a0a 2020 2020 2320 5072  es}'")..    # Pr
+0000b0b0: 6570 6172 6520 6469 736b 2072 6573 6f75  epare disk resou
+0000b0c0: 7263 6573 0a20 2020 2070 6f73 745f 6461  rces.    post_da
+0000b0d0: 7461 203d 207b 226e 6f64 6573 223a 206e  ta = {"nodes": n
+0000b0e0: 6577 5f6e 6f64 6573 7d0a 2020 2020 5f73  ew_nodes}.    _s
+0000b0f0: 696d 756c 6174 696f 6e5f 6578 6563 7574  imulation_execut
+0000b100: 655f 6f70 6572 6174 696f 6e28 0a20 2020  e_operation(.   
+0000b110: 2020 2020 2022 706f 7374 222c 0a20 2020       "post",.   
+0000b120: 2020 2020 2022 7072 6570 6172 6522 2c0a       "prepare",.
+0000b130: 2020 2020 2020 2020 6964 5f73 696d 756c          id_simul
+0000b140: 6174 696f 6e2c 0a20 2020 2020 2020 2022  ation,.        "
+0000b150: 5052 4550 4152 494e 4722 2c0a 2020 2020  PREPARING",.    
+0000b160: 2020 2020 6f70 7469 6f6e 616c 5f70 6172      optional_par
+0000b170: 616d 313d 616c 6c6f 6361 7469 6f6e 5f73  am1=allocation_s
+0000b180: 7472 6174 6567 792c 0a20 2020 2020 2020  trategy,.       
+0000b190: 2070 6f73 745f 6461 7461 3d70 6f73 745f   post_data=post_
+0000b1a0: 6461 7461 2c0a 2020 2020 290a 0a20 2020  data,.    )..   
+0000b1b0: 2023 2054 4f44 4f3a 2043 6865 636b 2074   # TODO: Check t
+0000b1c0: 6861 7420 7468 6520 646f 636b 6572 2076  hat the docker v
+0000b1d0: 6f6c 756d 6573 2074 6861 7420 7769 6c6c  olumes that will
+0000b1e0: 2062 6520 6d6f 756e 7465 6420 6279 2073   be mounted by s
+0000b1f0: 696d 755f 7275 6e20 6172 6520 7072 6573  imu_run are pres
+0000b200: 656e 7420 6f6e 2074 6865 2066 696c 6573  ent on the files
+0000b210: 7973 7465 6d0a 2020 2020 2320 666f 7220  ystem.    # for 
+0000b220: 2e2e 2e3a 205f 7369 6d75 5f63 7265 6174  ...: _simu_creat
+0000b230: 655f 7661 6c69 6461 7465 5f72 6573 6f75  e_validate_resou
+0000b240: 7263 6573 5f65 7869 7374 7328 290a 0a20  rces_exists().. 
+0000b250: 2020 2072 6574 7572 6e20 2869 645f 7369     return (id_si
+0000b260: 6d75 6c61 7469 6f6e 2c20 6e65 775f 6e6f  mulation, new_no
+0000b270: 6465 7329 0a0a 0a64 6566 2073 696d 756c  des)...def simul
+0000b280: 6174 696f 6e5f 7374 6174 7573 2869 645f  ation_status(id_
+0000b290: 7369 6d75 6c61 7469 6f6e 3a20 696e 7429  simulation: int)
+0000b2a0: 202d 3e20 7374 723a 0a20 2020 2022 2222   -> str:.    """
+0000b2b0: 5265 7472 6965 7665 2074 6865 2073 696d  Retrieve the sim
+0000b2c0: 756c 6174 696f 6e20 7374 6174 7573 2e0a  ulation status..
+0000b2d0: 0a20 2020 203a 7265 7475 726e 3a20 5468  .    :return: Th
+0000b2e0: 6520 7374 6174 7573 206f 6620 7468 6520  e status of the 
+0000b2f0: 7369 6d75 6c61 7469 6f6e 2e0a 0a20 2020  simulation...   
+0000b300: 203a 7061 7261 6d20 6964 5f73 696d 756c   :param id_simul
+0000b310: 6174 696f 6e3a 2054 6865 2073 696d 756c  ation: The simul
+0000b320: 6174 696f 6e20 4944 2e0a 0a20 2020 2022  ation ID...    "
+0000b330: 2222 0a20 2020 2072 6573 756c 7420 3d20  "".    result = 
+0000b340: 5f67 6574 2866 222f 7369 6d75 6c61 7469  _get(f"/simulati
+0000b350: 6f6e 2f7b 6964 5f73 696d 756c 6174 696f  on/{id_simulatio
+0000b360: 6e7d 2f73 7461 7475 7322 290a 0a20 2020  n}/status")..   
+0000b370: 2069 6620 7265 7375 6c74 2e73 7461 7475   if result.statu
+0000b380: 735f 636f 6465 2021 3d20 3230 303a 0a20  s_code != 200:. 
+0000b390: 2020 2020 2020 205f 6861 6e64 6c65 5f65         _handle_e
+0000b3a0: 7272 6f72 2872 6573 756c 742c 2022 4361  rror(result, "Ca
+0000b3b0: 6e6e 6f74 2072 6574 7269 6576 6520 7369  nnot retrieve si
+0000b3c0: 6d75 6c61 7469 6f6e 2069 6e66 6f20 6672  mulation info fr
+0000b3d0: 6f6d 2049 5420 5369 6d75 6c61 7469 6f6e  om IT Simulation
+0000b3e0: 2041 5049 2229 0a0a 2020 2020 7265 7475   API")..    retu
+0000b3f0: 726e 2072 6573 756c 742e 6a73 6f6e 2829  rn result.json()
+0000b400: 0a0a 0a64 6566 2066 6574 6368 5f73 696d  ...def fetch_sim
+0000b410: 756c 6174 696f 6e28 6964 5f73 696d 756c  ulation(id_simul
+0000b420: 6174 696f 6e3a 2069 6e74 2920 2d3e 2064  ation: int) -> d
+0000b430: 6963 743a 0a20 2020 2022 2222 5265 7472  ict:.    """Retr
+0000b440: 6965 7665 2061 2073 7065 6369 6669 6320  ieve a specific 
+0000b450: 7369 6d75 6c61 7469 6f6e 2067 6976 656e  simulation given
+0000b460: 2061 2073 696d 756c 6174 696f 6e20 6964   a simulation id
+0000b470: 2e0a 0a20 2020 203a 7265 7475 726e 3a20  ...    :return: 
+0000b480: 4120 6469 6374 2063 6f6e 7461 696e 696e  A dict containin
+0000b490: 6720 6461 7461 2072 656c 6174 6564 2074  g data related t
+0000b4a0: 6f20 7468 6520 7461 7267 6574 6564 2073  o the targeted s
+0000b4b0: 696d 756c 6174 696f 6e2e 0a0a 2020 2020  imulation...    
+0000b4c0: 3a70 6172 616d 2069 645f 7369 6d75 6c61  :param id_simula
+0000b4d0: 7469 6f6e 3a20 5468 6520 7369 6d75 6c61  tion: The simula
+0000b4e0: 7469 6f6e 2049 442e 0a0a 2020 2020 2222  tion ID...    ""
+0000b4f0: 220a 2020 2020 7265 7375 6c74 203d 205f  ".    result = _
+0000b500: 6765 7428 6622 2f73 696d 756c 6174 696f  get(f"/simulatio
+0000b510: 6e2f 7b69 645f 7369 6d75 6c61 7469 6f6e  n/{id_simulation
+0000b520: 7d22 290a 0a20 2020 2069 6620 7265 7375  }")..    if resu
+0000b530: 6c74 2e73 7461 7475 735f 636f 6465 2021  lt.status_code !
+0000b540: 3d20 3230 303a 0a20 2020 2020 2020 205f  = 200:.        _
+0000b550: 6861 6e64 6c65 5f65 7272 6f72 2872 6573  handle_error(res
+0000b560: 756c 742c 2022 4361 6e6e 6f74 2072 6574  ult, "Cannot ret
+0000b570: 7269 6576 6520 7369 6d75 6c61 7469 6f6e  rieve simulation
+0000b580: 2069 6e66 6f20 6672 6f6d 2049 5420 5369   info from IT Si
+0000b590: 6d75 6c61 7469 6f6e 2041 5049 2229 0a0a  mulation API")..
+0000b5a0: 2020 2020 7369 6d75 6c61 7469 6f6e 5f64      simulation_d
+0000b5b0: 6963 7420 3d20 7265 7375 6c74 2e6a 736f  ict = result.jso
+0000b5c0: 6e28 290a 0a20 2020 2072 6574 7572 6e20  n()..    return 
+0000b5d0: 7369 6d75 6c61 7469 6f6e 5f64 6963 740a  simulation_dict.
+0000b5e0: 0a0a 6465 6620 6665 7463 685f 7369 6d75  ..def fetch_simu
+0000b5f0: 6c61 7469 6f6e 7328 2920 2d3e 204c 6973  lations() -> Lis
+0000b600: 745b 416e 795d 3a0a 2020 2020 2222 2247  t[Any]:.    """G
+0000b610: 6574 2074 6865 206c 6973 7420 6f66 2073  et the list of s
+0000b620: 696d 756c 6174 696f 6e73 2c20 696e 636c  imulations, incl
+0000b630: 7564 696e 6720 7468 6520 6375 7272 656e  uding the curren
+0000b640: 746c 7920 7275 6e6e 696e 6720 7369 6d75  tly running simu
+0000b650: 616c 7469 6f6e 2c20 616c 6f6e 6720 7769  altion, along wi
+0000b660: 7468 0a20 2020 2069 6e66 6f72 6d61 7469  th.    informati
+0000b670: 6f6e 206f 6e20 6e6f 6465 732e 0a0a 2020  on on nodes...  
+0000b680: 2020 3a72 6574 7572 6e3a 2054 6865 206c    :return: The l
+0000b690: 6973 7420 6f66 2073 696d 756c 6174 696f  ist of simulatio
+0000b6a0: 6e73 2e0a 0a20 2020 2022 2222 0a20 2020  ns...    """.   
+0000b6b0: 2072 6573 756c 7420 3d20 5f67 6574 2822   result = _get("
+0000b6c0: 2f73 696d 756c 6174 696f 6e2f 2229 0a0a  /simulation/")..
+0000b6d0: 2020 2020 6966 2072 6573 756c 742e 7374      if result.st
+0000b6e0: 6174 7573 5f63 6f64 6520 213d 2032 3030  atus_code != 200
+0000b6f0: 3a0a 2020 2020 2020 2020 5f68 616e 646c  :.        _handl
+0000b700: 655f 6572 726f 7228 7265 7375 6c74 2c20  e_error(result, 
+0000b710: 2243 616e 6e6f 7420 7265 7472 6965 7665  "Cannot retrieve
+0000b720: 2073 696d 756c 6174 696f 6e20 696e 666f   simulation info
+0000b730: 2066 726f 6d20 4954 2053 696d 756c 6174   from IT Simulat
+0000b740: 696f 6e20 4150 4922 290a 0a20 2020 2073  ion API")..    s
+0000b750: 696d 756c 6174 696f 6e5f 6c69 7374 203d  imulation_list =
+0000b760: 2072 6573 756c 742e 6a73 6f6e 2829 0a20   result.json(). 
+0000b770: 2020 2072 6574 7572 6e20 7369 6d75 6c61     return simula
+0000b780: 7469 6f6e 5f6c 6973 740a 0a0a 6465 6620  tion_list...def 
+0000b790: 6465 6c65 7465 5f73 696d 756c 6174 696f  delete_simulatio
+0000b7a0: 6e28 6964 5f73 696d 756c 6174 696f 6e3a  n(id_simulation:
+0000b7b0: 2069 6e74 2920 2d3e 2041 6e79 3a0a 2020   int) -> Any:.  
+0000b7c0: 2020 2222 2244 656c 6574 6520 6120 7369    """Delete a si
+0000b7d0: 6d75 6c61 7469 6f6e 2069 6e20 6461 7461  mulation in data
+0000b7e0: 6261 7365 2e0a 0a20 2020 203a 7265 7475  base...    :retu
+0000b7f0: 726e 3a20 4120 6d65 7373 6167 6520 7465  rn: A message te
+0000b800: 6c6c 696e 6720 686f 7720 7468 6520 6f70  lling how the op
+0000b810: 6572 6174 696f 6e20 6578 6563 7574 6564  eration executed
+0000b820: 2e0a 0a20 2020 203a 7061 7261 6d20 6964  ...    :param id
+0000b830: 5f73 696d 756c 6174 696f 6e3a 2054 6865  _simulation: The
+0000b840: 2073 696d 756c 6174 696f 6e20 4944 2e0a   simulation ID..
+0000b850: 0a20 2020 2022 2222 0a0a 2020 2020 2320  .    """..    # 
+0000b860: 4465 7374 726f 7920 7369 6d75 6c61 7469  Destroy simulati
+0000b870: 6f6e 2069 6620 6974 2069 7320 7275 6e6e  on if it is runn
+0000b880: 696e 670a 2020 2020 6966 2073 696d 756c  ing.    if simul
+0000b890: 6174 696f 6e5f 7374 6174 7573 2869 645f  ation_status(id_
+0000b8a0: 7369 6d75 6c61 7469 6f6e 2920 3d3d 2022  simulation) == "
+0000b8b0: 5255 4e4e 494e 4722 3a0a 2020 2020 2020  RUNNING":.      
+0000b8c0: 2020 6e6f 6465 733a 204c 6973 745b 7374    nodes: List[st
+0000b8d0: 725d 203d 205b 5d0a 2020 2020 2020 2020  r] = [].        
+0000b8e0: 706f 7374 5f64 6174 6120 3d20 7b22 6e6f  post_data = {"no
+0000b8f0: 6465 7322 3a20 6e6f 6465 737d 0a0a 2020  des": nodes}..  
+0000b900: 2020 2020 2020 5f73 696d 756c 6174 696f        _simulatio
+0000b910: 6e5f 6578 6563 7574 655f 6f70 6572 6174  n_execute_operat
+0000b920: 696f 6e28 0a20 2020 2020 2020 2020 2020  ion(.           
+0000b930: 2022 706f 7374 222c 2022 6465 7374 726f   "post", "destro
+0000b940: 7922 2c20 6964 5f73 696d 756c 6174 696f  y", id_simulatio
+0000b950: 6e2c 2022 5354 4f50 5049 4e47 222c 2070  n, "STOPPING", p
+0000b960: 6f73 745f 6461 7461 3d70 6f73 745f 6461  ost_data=post_da
+0000b970: 7461 0a20 2020 2020 2020 2029 0a0a 2020  ta.        )..  
+0000b980: 2020 5f73 696d 756c 6174 696f 6e5f 6578    _simulation_ex
+0000b990: 6563 7574 655f 6f70 6572 6174 696f 6e28  ecute_operation(
+0000b9a0: 2267 6574 222c 2022 6465 6c65 7465 5f73  "get", "delete_s
+0000b9b0: 6e61 7073 686f 7473 222c 2069 645f 7369  napshots", id_si
+0000b9c0: 6d75 6c61 7469 6f6e 2c20 2253 544f 5050  mulation, "STOPP
+0000b9d0: 494e 4722 290a 0a20 2020 2023 2044 656c  ING")..    # Del
+0000b9e0: 6574 6520 7369 6d75 6c61 7469 6f6e 206e  ete simulation n
+0000b9f0: 6f64 6573 0a20 2020 2064 656c 6574 655f  odes.    delete_
+0000ba00: 6e6f 6465 7328 6964 5f73 696d 756c 6174  nodes(id_simulat
+0000ba10: 696f 6e29 0a0a 2020 2020 2320 4465 6c65  ion)..    # Dele
+0000ba20: 7465 2073 696d 756c 6174 696f 6e0a 2020  te simulation.  
+0000ba30: 2020 7265 7375 6c74 203d 205f 6465 6c65    result = _dele
+0000ba40: 7465 2866 222f 7369 6d75 6c61 7469 6f6e  te(f"/simulation
+0000ba50: 2f7b 6964 5f73 696d 756c 6174 696f 6e7d  /{id_simulation}
+0000ba60: 2229 0a0a 2020 2020 6966 2072 6573 756c  ")..    if resul
+0000ba70: 742e 7374 6174 7573 5f63 6f64 6520 213d  t.status_code !=
+0000ba80: 2032 3030 3a0a 2020 2020 2020 2020 5f68   200:.        _h
+0000ba90: 616e 646c 655f 6572 726f 7228 7265 7375  andle_error(resu
+0000baa0: 6c74 2c20 2243 616e 6e6f 7420 6465 6c65  lt, "Cannot dele
+0000bab0: 7465 2073 696d 756c 6174 696f 6e20 6672  te simulation fr
+0000bac0: 6f6d 2049 5420 5369 6d75 6c61 7469 6f6e  om IT Simulation
+0000bad0: 2041 5049 2229 0a0a 2020 2020 7265 7475   API")..    retu
+0000bae0: 726e 2072 6573 756c 742e 6a73 6f6e 2829  rn result.json()
+0000baf0: 0a0a 0a64 6566 206e 6f64 655f 7374 6174  ...def node_stat
+0000bb00: 7573 2869 645f 6e6f 6465 3a20 696e 7429  us(id_node: int)
+0000bb10: 202d 3e20 7374 723a 0a20 2020 2022 2222   -> str:.    """
+0000bb20: 5265 7472 6965 7665 206e 6f64 6520 7374  Retrieve node st
+0000bb30: 6174 7573 2e0a 0a20 2020 203a 7265 7475  atus...    :retu
+0000bb40: 726e 3a20 5468 6520 7374 6174 7573 206f  rn: The status o
+0000bb50: 6620 7468 6520 6e6f 6465 2e0a 0a20 2020  f the node...   
+0000bb60: 203a 7061 7261 6d20 6964 5f6e 6f64 653a   :param id_node:
+0000bb70: 2054 6865 206e 6f64 6520 4944 2e0a 0a20   The node ID... 
+0000bb80: 2020 2022 2222 0a0a 2020 2020 7265 7375     """..    resu
+0000bb90: 6c74 203d 205f 6765 7428 6622 2f6e 6f64  lt = _get(f"/nod
+0000bba0: 652f 7b69 645f 6e6f 6465 7d2f 7374 6174  e/{id_node}/stat
+0000bbb0: 7573 2229 0a0a 2020 2020 6966 2072 6573  us")..    if res
+0000bbc0: 756c 742e 7374 6174 7573 5f63 6f64 6520  ult.status_code 
+0000bbd0: 213d 2032 3030 3a0a 2020 2020 2020 2020  != 200:.        
+0000bbe0: 5f68 616e 646c 655f 6572 726f 7228 7265  _handle_error(re
+0000bbf0: 7375 6c74 2c20 2243 616e 6e6f 7420 7265  sult, "Cannot re
+0000bc00: 7472 6965 7665 206e 6f64 6520 696e 666f  trieve node info
+0000bc10: 2066 726f 6d20 4954 2053 696d 756c 6174   from IT Simulat
+0000bc20: 696f 6e20 4150 4922 290a 0a20 2020 2072  ion API")..    r
+0000bc30: 6574 7572 6e20 7265 7375 6c74 2e6a 736f  eturn result.jso
+0000bc40: 6e28 290a 0a0a 6465 6620 7374 6f70 5f6e  n()...def stop_n
+0000bc50: 6f64 655f 6279 5f6e 616d 6528 6964 5f73  ode_by_name(id_s
+0000bc60: 696d 756c 6174 696f 6e3a 2069 6e74 2c20  imulation: int, 
+0000bc70: 6e6f 6465 5f6e 616d 653a 2073 7472 2920  node_name: str) 
+0000bc80: 2d3e 204e 6f6e 653a 0a20 2020 2022 2222  -> None:.    """
+0000bc90: 5374 6f70 2061 206e 6f64 6520 6966 2069  Stop a node if i
+0000bca0: 7420 6973 2072 756e 6e69 6e67 2e0a 0a20  t is running... 
+0000bcb0: 2020 203a 7061 7261 6d20 6964 5f73 696d     :param id_sim
+0000bcc0: 756c 6174 696f 6e3a 2054 6865 2073 696d  ulation: The sim
+0000bcd0: 756c 6174 696f 6e20 4944 2e0a 2020 2020  ulation ID..    
+0000bce0: 3a70 6172 616d 206e 6f64 655f 6e61 6d65  :param node_name
+0000bcf0: 3a20 5468 6520 6e6f 6465 206e 616d 6520  : The node name 
+0000bd00: 746f 2073 746f 702e 0a0a 2020 2020 2222  to stop...    ""
+0000bd10: 220a 0a20 2020 2023 2052 6574 7269 6576  "..    # Retriev
+0000bd20: 6520 6964 5f6e 6f64 650a 2020 2020 6e6f  e id_node.    no
+0000bd30: 6465 203d 2066 6574 6368 5f6e 6f64 655f  de = fetch_node_
+0000bd40: 6279 5f6e 616d 6528 6964 5f73 696d 756c  by_name(id_simul
+0000bd50: 6174 696f 6e2c 206e 6f64 655f 6e61 6d65  ation, node_name
+0000bd60: 290a 2020 2020 6964 5f6e 6f64 6520 3d20  ).    id_node = 
+0000bd70: 6e6f 6465 5b22 6964 225d 0a0a 2020 2020  node["id"]..    
+0000bd80: 2320 4465 6c65 7465 206e 6f64 650a 2020  # Delete node.  
+0000bd90: 2020 7374 6f70 5f6e 6f64 6528 6964 5f73    stop_node(id_s
+0000bda0: 696d 756c 6174 696f 6e2c 2069 645f 6e6f  imulation, id_no
+0000bdb0: 6465 290a 0a0a 6465 6620 7374 6f70 5f6e  de)...def stop_n
+0000bdc0: 6f64 6528 6964 5f73 696d 756c 6174 696f  ode(id_simulatio
+0000bdd0: 6e3a 2069 6e74 2c20 6964 5f6e 6f64 653a  n: int, id_node:
+0000bde0: 2069 6e74 2920 2d3e 204e 6f6e 653a 0a20   int) -> None:. 
+0000bdf0: 2020 2022 2222 5374 6f70 2061 206e 6f64     """Stop a nod
+0000be00: 6520 6966 2069 7420 6973 2072 756e 6e69  e if it is runni
+0000be10: 6e67 2e0a 0a20 2020 203a 7061 7261 6d20  ng...    :param 
+0000be20: 6964 5f73 696d 756c 6174 696f 6e3a 2054  id_simulation: T
+0000be30: 6865 2073 696d 756c 6174 696f 6e20 4944  he simulation ID
+0000be40: 2e0a 2020 2020 3a70 6172 616d 2069 645f  ..    :param id_
+0000be50: 6e6f 6465 3a20 5468 6520 6e6f 6465 2049  node: The node I
+0000be60: 442e 0a0a 2020 2020 2222 220a 0a20 2020  D...    """..   
+0000be70: 2023 2052 6574 7269 6576 6520 6e6f 6465   # Retrieve node
+0000be80: 2061 6363 6f72 6469 6e67 2074 6f20 6974   according to it
+0000be90: 7320 6e61 6d65 0a20 2020 206e 6f64 6520  s name.    node 
+0000bea0: 3d20 6665 7463 685f 6e6f 6465 2869 645f  = fetch_node(id_
+0000beb0: 6e6f 6465 290a 0a20 2020 2023 2053 6574  node)..    # Set
+0000bec0: 206e 6f64 6520 6e61 6d65 7320 746f 2064   node names to d
+0000bed0: 656c 6574 650a 2020 2020 6e6f 6465 735f  elete.    nodes_
+0000bee0: 746f 5f64 656c 6574 6520 3d20 5b6e 6f64  to_delete = [nod
+0000bef0: 655b 226e 616d 6522 5d5d 0a20 2020 2070  e["name"]].    p
+0000bf00: 6f73 745f 6461 7461 203d 207b 226e 6f64  ost_data = {"nod
+0000bf10: 6573 223a 206e 6f64 6573 5f74 6f5f 6465  es": nodes_to_de
+0000bf20: 6c65 7465 7d0a 0a20 2020 2023 2053 746f  lete}..    # Sto
+0000bf30: 7020 6e6f 6465 2069 6620 6974 2069 7320  p node if it is 
+0000bf40: 7275 6e6e 696e 670a 2020 2020 6966 206e  running.    if n
+0000bf50: 6f64 655f 7374 6174 7573 2869 645f 6e6f  ode_status(id_no
+0000bf60: 6465 2920 3d3d 2022 5255 4e4e 494e 4722  de) == "RUNNING"
+0000bf70: 3a0a 2020 2020 2020 2020 5f73 696d 756c  :.        _simul
+0000bf80: 6174 696f 6e5f 6578 6563 7574 655f 6f70  ation_execute_op
+0000bf90: 6572 6174 696f 6e28 0a20 2020 2020 2020  eration(.       
+0000bfa0: 2020 2020 2022 706f 7374 222c 0a20 2020       "post",.   
+0000bfb0: 2020 2020 2020 2020 2022 6861 6c74 222c           "halt",
+0000bfc0: 0a20 2020 2020 2020 2020 2020 2069 645f  .            id_
+0000bfd0: 7369 6d75 6c61 7469 6f6e 2c0a 2020 2020  simulation,.    
+0000bfe0: 2020 2020 2020 2020 2253 544f 5050 494e          "STOPPIN
+0000bff0: 4722 2c0a 2020 2020 2020 2020 2020 2020  G",.            
+0000c000: 706f 7374 5f64 6174 613d 706f 7374 5f64  post_data=post_d
+0000c010: 6174 612c 0a20 2020 2020 2020 2029 0a0a  ata,.        )..
+0000c020: 0a64 6566 2075 7064 6174 655f 7369 6d75  .def update_simu
+0000c030: 6c61 7469 6f6e 2869 645f 7369 6d75 6c61  lation(id_simula
+0000c040: 7469 6f6e 3a20 696e 742c 2073 696d 756c  tion: int, simul
+0000c050: 6174 696f 6e5f 6469 6374 3a20 6469 6374  ation_dict: dict
+0000c060: 2920 2d3e 2041 6e79 3a0a 2020 2020 2222  ) -> Any:.    ""
+0000c070: 2255 7064 6174 6520 7369 6d75 6c61 7469  "Update simulati
+0000c080: 6f6e 2069 6e66 6f72 6d61 7469 6f6e 2069  on information i
+0000c090: 6e66 6f72 6d61 7469 6f6e 2067 6976 656e  nformation given
+0000c0a0: 2061 2073 696d 756c 6174 696f 6e20 6964   a simulation id
+0000c0b0: 0a20 2020 2061 6e64 2061 2064 6963 7420  .    and a dict 
+0000c0c0: 636f 6e74 6169 6e69 6e67 2073 696d 756c  containing simul
+0000c0d0: 6174 696f 6e20 696e 666f 2e0a 0a20 2020  ation info...   
+0000c0e0: 203a 7265 7475 726e 3a20 4120 6d65 7373   :return: A mess
+0000c0f0: 6167 6520 7465 6c6c 696e 6720 686f 7720  age telling how 
+0000c100: 7468 6520 6f70 6572 6174 696f 6e20 6578  the operation ex
+0000c110: 6563 7574 6564 2e0a 0a20 2020 203a 7061  ecuted...    :pa
+0000c120: 7261 6d20 6964 5f73 696d 756c 6174 696f  ram id_simulatio
+0000c130: 6e3a 2054 6865 2073 696d 756c 6174 696f  n: The simulatio
+0000c140: 6e20 4944 2e0a 2020 2020 3a70 6172 616d  n ID..    :param
+0000c150: 2073 696d 756c 6174 696f 6e5f 6469 6374   simulation_dict
+0000c160: 3a20 5468 6520 6469 6374 2063 6f6e 7461  : The dict conta
+0000c170: 696e 696e 6720 7468 6520 656e 7472 6965  ining the entrie
+0000c180: 7320 746f 2075 7064 6174 652e 0a0a 2020  s to update...  
+0000c190: 2020 2222 220a 2020 2020 6461 7461 203d    """.    data =
+0000c1a0: 206a 736f 6e2e 6475 6d70 7328 7369 6d75   json.dumps(simu
+0000c1b0: 6c61 7469 6f6e 5f64 6963 7429 0a20 2020  lation_dict).   
+0000c1c0: 2072 6573 756c 7420 3d20 5f70 7574 280a   result = _put(.
+0000c1d0: 2020 2020 2020 2020 6622 2f73 696d 756c          f"/simul
+0000c1e0: 6174 696f 6e2f 7b69 645f 7369 6d75 6c61  ation/{id_simula
+0000c1f0: 7469 6f6e 7d22 2c0a 2020 2020 2020 2020  tion}",.        
+0000c200: 6461 7461 3d64 6174 612c 0a20 2020 2020  data=data,.     
+0000c210: 2020 2068 6561 6465 7273 3d7b 2243 6f6e     headers={"Con
+0000c220: 7465 6e74 2d54 7970 6522 3a20 2261 7070  tent-Type": "app
+0000c230: 6c69 6361 7469 6f6e 2f6a 736f 6e22 7d2c  lication/json"},
+0000c240: 0a20 2020 2029 0a0a 2020 2020 6966 2072  .    )..    if r
+0000c250: 6573 756c 742e 7374 6174 7573 5f63 6f64  esult.status_cod
+0000c260: 6520 213d 2032 3030 3a0a 2020 2020 2020  e != 200:.      
+0000c270: 2020 5f68 616e 646c 655f 6572 726f 7228    _handle_error(
+0000c280: 7265 7375 6c74 2c20 2243 616e 6e6f 7420  result, "Cannot 
+0000c290: 7570 6461 7465 2073 696d 756c 6174 696f  update simulatio
+0000c2a0: 6e20 696e 666f 726d 6174 696f 6e22 290a  n information").
+0000c2b0: 0a20 2020 2072 6574 7572 6e20 7265 7375  .    return resu
+0000c2c0: 6c74 2e6a 736f 6e28 290a 0a0a 6465 6620  lt.json()...def 
+0000c2d0: 6665 7463 685f 7369 6d75 6c61 7469 6f6e  fetch_simulation
+0000c2e0: 5f74 6f70 6f6c 6f67 7928 6964 5f73 696d  _topology(id_sim
+0000c2f0: 756c 6174 696f 6e3a 2069 6e74 2920 2d3e  ulation: int) ->
+0000c300: 2041 6e79 3a0a 2020 2020 2222 2252 6574   Any:.    """Ret
+0000c310: 7572 6e20 7468 6520 746f 706f 6c6f 6779  urn the topology
+0000c320: 206f 6620 6120 7369 6d75 6c61 7469 6f6e   of a simulation
+0000c330: 2e0a 0a20 2020 203a 7265 7475 726e 3a20  ...    :return: 
+0000c340: 5468 6520 7369 6d75 6c61 7469 6f6e 2074  The simulation t
+0000c350: 6f70 6f6c 6f67 792e 0a0a 2020 2020 3a70  opology...    :p
+0000c360: 6172 616d 2069 645f 7369 6d75 6c61 7469  aram id_simulati
+0000c370: 6f6e 3a20 5468 6520 7369 6d75 6c61 7469  on: The simulati
+0000c380: 6f6e 2049 442e 0a0a 2020 2020 2222 220a  on ID...    """.
+0000c390: 2020 2020 7265 7375 6c74 203d 205f 6765      result = _ge
+0000c3a0: 7428 6622 2f73 696d 756c 6174 696f 6e2f  t(f"/simulation/
+0000c3b0: 7b69 645f 7369 6d75 6c61 7469 6f6e 7d2f  {id_simulation}/
+0000c3c0: 746f 706f 6c6f 6779 2229 0a0a 2020 2020  topology")..    
+0000c3d0: 6966 2072 6573 756c 742e 7374 6174 7573  if result.status
+0000c3e0: 5f63 6f64 6520 213d 2032 3030 3a0a 2020  _code != 200:.  
+0000c3f0: 2020 2020 2020 5f68 616e 646c 655f 6572        _handle_er
+0000c400: 726f 7228 7265 7375 6c74 2c20 2243 616e  ror(result, "Can
+0000c410: 6e6f 7420 7265 7472 6965 7665 2073 696d  not retrieve sim
+0000c420: 756c 6174 696f 6e20 746f 706f 6c6f 6779  ulation topology
+0000c430: 2069 6e66 6f22 290a 0a20 2020 2072 6574   info")..    ret
+0000c440: 7572 6e20 7265 7375 6c74 2e6a 736f 6e28  urn result.json(
+0000c450: 290a 0a0a 6465 6620 6665 7463 685f 7369  )...def fetch_si
+0000c460: 6d75 6c61 7469 6f6e 5f74 6f70 6f6c 6f67  mulation_topolog
+0000c470: 795f 7961 6d6c 2869 645f 7369 6d75 6c61  y_yaml(id_simula
+0000c480: 7469 6f6e 3a20 696e 7429 202d 3e20 416e  tion: int) -> An
+0000c490: 793a 0a20 2020 2022 2222 5265 7475 726e  y:.    """Return
+0000c4a0: 2074 6865 2059 414d 4c20 746f 706f 6c6f   the YAML topolo
+0000c4b0: 6779 2063 6f6e 7465 6e74 206f 6620 6120  gy content of a 
+0000c4c0: 7369 6d75 6c61 7469 6f6e 2e0a 0a20 2020  simulation...   
+0000c4d0: 203a 7265 7475 726e 3a20 5468 6520 5941   :return: The YA
+0000c4e0: 4d4c 2073 696d 756c 6174 696f 6e20 746f  ML simulation to
+0000c4f0: 706f 6c6f 6779 2e0a 0a20 2020 203a 7061  pology...    :pa
+0000c500: 7261 6d20 6964 5f73 696d 756c 6174 696f  ram id_simulatio
+0000c510: 6e3a 2054 6865 2073 696d 756c 6174 696f  n: The simulatio
+0000c520: 6e20 4944 2e0a 0a20 2020 2022 2222 0a20  n ID...    """. 
+0000c530: 2020 2072 6573 756c 7420 3d20 5f67 6574     result = _get
+0000c540: 2866 222f 7369 6d75 6c61 7469 6f6e 2f7b  (f"/simulation/{
+0000c550: 6964 5f73 696d 756c 6174 696f 6e7d 2f74  id_simulation}/t
+0000c560: 6f70 6f6c 6f67 795f 7961 6d6c 2229 0a0a  opology_yaml")..
+0000c570: 2020 2020 6966 2072 6573 756c 742e 7374      if result.st
+0000c580: 6174 7573 5f63 6f64 6520 213d 2032 3030  atus_code != 200
+0000c590: 3a0a 2020 2020 2020 2020 5f68 616e 646c  :.        _handl
+0000c5a0: 655f 6572 726f 7228 7265 7375 6c74 2c20  e_error(result, 
+0000c5b0: 2243 616e 6e6f 7420 7265 7472 6965 7665  "Cannot retrieve
+0000c5c0: 2073 696d 756c 6174 696f 6e20 746f 706f   simulation topo
+0000c5d0: 6c6f 6779 2069 6e66 6f22 290a 0a20 2020  logy info")..   
+0000c5e0: 2072 6574 7572 6e20 7265 7375 6c74 2e6a   return result.j
+0000c5f0: 736f 6e28 290a 0a0a 6465 6620 6665 7463  son()...def fetc
+0000c600: 685f 6173 7365 7473 2869 645f 7369 6d75  h_assets(id_simu
+0000c610: 6c61 7469 6f6e 3a20 696e 7429 202d 3e20  lation: int) -> 
+0000c620: 416e 793a 0a20 2020 2022 2222 5265 7475  Any:.    """Retu
+0000c630: 726e 2074 6865 206c 6973 7420 6f66 2074  rn the list of t
+0000c640: 6865 2061 7373 6574 7320 6f66 2061 2067  he assets of a g
+0000c650: 6976 656e 2073 696d 756c 6174 696f 6e2e  iven simulation.
+0000c660: 2049 7420 636f 7272 6573 706f 6e64 730a   It corresponds.
+0000c670: 2020 2020 746f 2074 6865 206c 6973 7420      to the list 
+0000c680: 6f66 2074 6865 206e 6f64 6573 2077 6974  of the nodes wit
+0000c690: 6820 736f 6d65 2061 6464 6974 696f 6e61  h some additiona
+0000c6a0: 6c20 696e 666f 726d 6174 696f 6e2e 0a0a  l information...
+0000c6b0: 2020 2020 3a72 6574 7572 6e3a 2054 6865      :return: The
+0000c6c0: 2073 696d 756c 6174 696f 6e20 6173 7365   simulation asse
+0000c6d0: 7473 2e0a 0a20 2020 203a 7061 7261 6d20  ts...    :param 
+0000c6e0: 6964 5f73 696d 756c 6174 696f 6e3a 2054  id_simulation: T
+0000c6f0: 6865 2073 696d 756c 6174 696f 6e20 4944  he simulation ID
+0000c700: 2e0a 0a20 2020 2022 2222 0a20 2020 2072  ...    """.    r
+0000c710: 6573 756c 7420 3d20 5f67 6574 2866 222f  esult = _get(f"/
+0000c720: 7369 6d75 6c61 7469 6f6e 2f7b 6964 5f73  simulation/{id_s
+0000c730: 696d 756c 6174 696f 6e7d 2f61 7373 6574  imulation}/asset
+0000c740: 7322 290a 0a20 2020 2069 6620 7265 7375  s")..    if resu
+0000c750: 6c74 2e73 7461 7475 735f 636f 6465 2021  lt.status_code !
+0000c760: 3d20 3230 303a 0a20 2020 2020 2020 205f  = 200:.        _
+0000c770: 6861 6e64 6c65 5f65 7272 6f72 2872 6573  handle_error(res
+0000c780: 756c 742c 2022 4361 6e6e 6f74 2072 6574  ult, "Cannot ret
+0000c790: 7269 6576 6520 6173 7365 7473 2066 726f  rieve assets fro
+0000c7a0: 6d20 636f 7265 2041 5049 2229 0a0a 2020  m core API")..  
+0000c7b0: 2020 7265 7475 726e 2072 6573 756c 742e    return result.
+0000c7c0: 6a73 6f6e 2829 0a0a 0a64 6566 2066 6574  json()...def fet
+0000c7d0: 6368 5f73 7769 7463 685f 6279 5f6e 6574  ch_switch_by_net
+0000c7e0: 776f 726b 5f69 6428 6964 5f73 696d 756c  work_id(id_simul
+0000c7f0: 6174 696f 6e3a 2069 6e74 2c20 6e65 7477  ation: int, netw
+0000c800: 6f72 6b5f 6964 3a20 7374 7229 202d 3e20  ork_id: str) -> 
+0000c810: 416e 793a 0a20 2020 2022 2222 5265 7475  Any:.    """Retu
+0000c820: 726e 2061 2073 7769 7463 6820 6769 7665  rn a switch give
+0000c830: 6e20 6974 7320 6e65 7477 6f72 6b5f 6964  n its network_id
+0000c840: 2e0a 0a20 2020 203a 7265 7475 726e 3a20  ...    :return: 
+0000c850: 5468 6520 7377 6974 6368 2064 6963 742e  The switch dict.
+0000c860: 0a0a 2020 2020 3a70 6172 616d 2069 645f  ..    :param id_
+0000c870: 7369 6d75 6c61 7469 6f6e 3a20 5468 6520  simulation: The 
+0000c880: 7369 6d75 6c61 7469 6f6e 2049 442e 0a20  simulation ID.. 
+0000c890: 2020 203a 7061 7261 6d20 6e65 7477 6f72     :param networ
+0000c8a0: 6b5f 6964 3a20 5468 6520 6e65 7477 6f72  k_id: The networ
+0000c8b0: 6b20 4944 2e0a 0a20 2020 2022 2222 0a0a  k ID...    """..
+0000c8c0: 2020 2020 7265 7375 6c74 203d 205f 6765      result = _ge
+0000c8d0: 7428 6622 2f73 696d 756c 6174 696f 6e2f  t(f"/simulation/
+0000c8e0: 7b69 645f 7369 6d75 6c61 7469 6f6e 7d2f  {id_simulation}/
+0000c8f0: 7377 6974 6368 2f7b 6e65 7477 6f72 6b5f  switch/{network_
+0000c900: 6964 7d22 290a 0a20 2020 2069 6620 7265  id}")..    if re
+0000c910: 7375 6c74 2e73 7461 7475 735f 636f 6465  sult.status_code
+0000c920: 2021 3d20 3230 303a 0a20 2020 2020 2020   != 200:.       
+0000c930: 205f 6861 6e64 6c65 5f65 7272 6f72 2872   _handle_error(r
+0000c940: 6573 756c 742c 2022 4361 6e6e 6f74 2072  esult, "Cannot r
+0000c950: 6574 7269 6576 6520 7369 6d75 6c61 7469  etrieve simulati
+0000c960: 6f6e 2073 7769 7463 6820 6672 6f6d 2063  on switch from c
+0000c970: 6f72 6520 4150 4922 290a 0a20 2020 2072  ore API")..    r
+0000c980: 6574 7572 6e20 7265 7375 6c74 2e6a 736f  eturn result.jso
+0000c990: 6e28 290a 0a0a 6465 6620 6665 7463 685f  n()...def fetch_
+0000c9a0: 6e6f 6465 286e 6f64 655f 6964 3a20 696e  node(node_id: in
+0000c9b0: 7429 202d 3e20 416e 793a 0a20 2020 2022  t) -> Any:.    "
+0000c9c0: 2222 5265 7475 726e 2061 206e 6f64 6520  ""Return a node 
+0000c9d0: 6769 7665 6e20 6974 7320 4944 2e0a 0a20  given its ID... 
+0000c9e0: 2020 203a 7265 7475 726e 3a20 5468 6520     :return: The 
+0000c9f0: 6e6f 6465 2064 6963 742e 0a0a 2020 2020  node dict...    
+0000ca00: 3a70 6172 616d 206e 6f64 655f 6964 3a20  :param node_id: 
+0000ca10: 5468 6520 6e6f 6465 2049 442e 0a0a 2020  The node ID...  
+0000ca20: 2020 2222 220a 2020 2020 7265 7375 6c74    """.    result
+0000ca30: 203d 205f 6765 7428 6622 2f6e 6f64 652f   = _get(f"/node/
+0000ca40: 7b6e 6f64 655f 6964 7d22 290a 0a20 2020  {node_id}")..   
+0000ca50: 2069 6620 7265 7375 6c74 2e73 7461 7475   if result.statu
+0000ca60: 735f 636f 6465 2021 3d20 3230 303a 0a20  s_code != 200:. 
+0000ca70: 2020 2020 2020 205f 6861 6e64 6c65 5f65         _handle_e
+0000ca80: 7272 6f72 2872 6573 756c 742c 2022 4361  rror(result, "Ca
+0000ca90: 6e6e 6f74 2072 6574 7269 6576 6520 6e6f  nnot retrieve no
+0000caa0: 6465 2066 726f 6d20 4954 2053 696d 756c  de from IT Simul
+0000cab0: 6174 696f 6e20 4150 4922 290a 0a20 2020  ation API")..   
+0000cac0: 2072 6574 7572 6e20 7265 7375 6c74 2e6a   return result.j
+0000cad0: 736f 6e28 290a 0a0a 6465 6620 6665 7463  son()...def fetc
+0000cae0: 685f 6e6f 6465 5f62 795f 6e61 6d65 2869  h_node_by_name(i
+0000caf0: 645f 7369 6d75 6c61 7469 6f6e 3a20 696e  d_simulation: in
+0000cb00: 742c 206e 6f64 655f 6e61 6d65 3a20 7374  t, node_name: st
+0000cb10: 7229 202d 3e20 416e 793a 0a20 2020 2022  r) -> Any:.    "
+0000cb20: 2222 5265 7475 726e 2061 206e 6f64 6520  ""Return a node 
+0000cb30: 6769 7665 6e20 6974 7320 6e61 6d65 2e0a  given its name..
+0000cb40: 0a20 2020 203a 7265 7475 726e 3a20 5468  .    :return: Th
+0000cb50: 6520 6e6f 6465 2064 6963 742e 0a0a 2020  e node dict...  
+0000cb60: 2020 3a70 6172 616d 2069 645f 7369 6d75    :param id_simu
+0000cb70: 6c61 7469 6f6e 3a20 5468 6520 7369 6d75  lation: The simu
+0000cb80: 6c61 7469 6f6e 2049 442e 0a20 2020 203a  lation ID..    :
+0000cb90: 7061 7261 6d20 6e6f 6465 5f6e 616d 653a  param node_name:
+0000cba0: 2054 6865 206e 6f64 6520 6e61 6d65 2074   The node name t
+0000cbb0: 6f20 6665 7463 682e 0a0a 2020 2020 2222  o fetch...    ""
+0000cbc0: 220a 0a20 2020 2072 6573 756c 7420 3d20  "..    result = 
+0000cbd0: 5f67 6574 2866 222f 7369 6d75 6c61 7469  _get(f"/simulati
+0000cbe0: 6f6e 2f7b 6964 5f73 696d 756c 6174 696f  on/{id_simulatio
+0000cbf0: 6e7d 2f6e 6f64 652f 7b6e 6f64 655f 6e61  n}/node/{node_na
+0000cc00: 6d65 7d22 290a 0a20 2020 2069 6620 7265  me}")..    if re
+0000cc10: 7375 6c74 2e73 7461 7475 735f 636f 6465  sult.status_code
+0000cc20: 2021 3d20 3230 303a 0a20 2020 2020 2020   != 200:.       
+0000cc30: 205f 6861 6e64 6c65 5f65 7272 6f72 280a   _handle_error(.
+0000cc40: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0000cc50: 6c74 2c20 2243 616e 6e6f 7420 7265 7472  lt, "Cannot retr
+0000cc60: 6965 7665 206e 6f64 6520 6261 7365 6420  ieve node based 
+0000cc70: 6f6e 2069 7473 206e 616d 6520 6672 6f6d  on its name from
+0000cc80: 2049 5420 5369 6d75 6c61 7469 6f6e 2041   IT Simulation A
+0000cc90: 5049 220a 2020 2020 2020 2020 290a 0a20  PI".        ).. 
+0000cca0: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+0000ccb0: 2e6a 736f 6e28 290a 0a0a 6465 6620 6665  .json()...def fe
+0000ccc0: 7463 685f 6e6f 6465 735f 6279 5f72 6f6c  tch_nodes_by_rol
+0000ccd0: 6573 2869 645f 7369 6d75 6c61 7469 6f6e  es(id_simulation
+0000cce0: 3a20 696e 7429 202d 3e20 416e 793a 0a20  : int) -> Any:. 
+0000ccf0: 2020 2022 2222 5265 7472 6965 7665 206e     """Retrieve n
+0000cd00: 6f64 6573 2063 6f6e 7465 6e74 2062 7920  odes content by 
+0000cd10: 726f 6c65 732e 0a0a 2020 2020 3a72 6574  roles...    :ret
+0000cd20: 7572 6e3a 2052 6574 7572 6e20 6120 6469  urn: Return a di
+0000cd30: 6374 2077 6b65 7265 206b 6579 7320 6172  ct wkere keys ar
+0000cd40: 6520 726f 6c65 7320 2873 7563 6820 6173  e roles (such as
+0000cd50: 2027 6164 272c 2027 6669 6c65 5f73 6572   'ad', 'file_ser
+0000cd60: 7665 7227 2c20 2763 6c69 656e 7427 2c20  ver', 'client', 
+0000cd70: 2e2e 2e29 2061 6e64 2076 616c 7565 7320  ...) and values 
+0000cd80: 6172 6520 6e6f 6465 732e 0a0a 2020 2020  are nodes...    
+0000cd90: 3a70 6172 616d 2069 645f 7369 6d75 6c61  :param id_simula
+0000cda0: 7469 6f6e 3a20 5468 6520 7369 6d75 6c61  tion: The simula
+0000cdb0: 7469 6f6e 2049 442e 0a0a 2020 2020 2222  tion ID...    ""
+0000cdc0: 220a 2020 2020 7265 7375 6c74 203d 205f  ".    result = _
+0000cdd0: 6765 7428 6622 2f73 696d 756c 6174 696f  get(f"/simulatio
+0000cde0: 6e2f 7b69 645f 7369 6d75 6c61 7469 6f6e  n/{id_simulation
+0000cdf0: 7d2f 6e6f 6465 735f 6279 5f72 6f6c 6573  }/nodes_by_roles
+0000ce00: 2229 0a0a 2020 2020 6966 2072 6573 756c  ")..    if resul
+0000ce10: 742e 7374 6174 7573 5f63 6f64 6520 213d  t.status_code !=
+0000ce20: 2032 3030 3a0a 2020 2020 2020 2020 5f68   200:.        _h
+0000ce30: 616e 646c 655f 6572 726f 7228 7265 7375  andle_error(resu
+0000ce40: 6c74 2c20 2243 616e 6e6f 7420 7265 7472  lt, "Cannot retr
+0000ce50: 6965 7665 206e 6f64 6573 2229 0a0a 2020  ieve nodes")..  
+0000ce60: 2020 726f 6c65 735f 6469 6374 203d 2072    roles_dict = r
+0000ce70: 6573 756c 742e 6a73 6f6e 2829 0a20 2020  esult.json().   
+0000ce80: 2072 6574 7572 6e20 726f 6c65 735f 6469   return roles_di
+0000ce90: 6374 0a0a 0a64 6566 2064 656c 6574 655f  ct...def delete_
+0000cea0: 6e6f 6465 5f62 795f 6e61 6d65 2869 645f  node_by_name(id_
+0000ceb0: 7369 6d75 6c61 7469 6f6e 3a20 696e 742c  simulation: int,
+0000cec0: 206e 6f64 655f 6e61 6d65 3a20 7374 7229   node_name: str)
+0000ced0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2222   -> None:.    ""
+0000cee0: 220a 0a20 2020 203a 7061 7261 6d20 6964  "..    :param id
+0000cef0: 5f73 696d 756c 6174 696f 6e3a 2054 6865  _simulation: The
+0000cf00: 2073 696d 756c 6174 696f 6e20 4944 2e0a   simulation ID..
+0000cf10: 2020 2020 3a70 6172 616d 206e 6f64 655f      :param node_
+0000cf20: 6e61 6d65 3a20 5468 6520 6e6f 6465 206e  name: The node n
+0000cf30: 616d 6520 746f 2064 656c 6574 652e 0a0a  ame to delete...
+0000cf40: 2020 2020 2222 220a 2020 2020 2320 5265      """.    # Re
+0000cf50: 7472 6965 7665 2069 645f 6e6f 6465 0a20  trieve id_node. 
+0000cf60: 2020 206e 6f64 6520 3d20 6665 7463 685f     node = fetch_
+0000cf70: 6e6f 6465 5f62 795f 6e61 6d65 2869 645f  node_by_name(id_
+0000cf80: 7369 6d75 6c61 7469 6f6e 2c20 6e6f 6465  simulation, node
+0000cf90: 5f6e 616d 6529 0a20 2020 2069 645f 6e6f  _name).    id_no
+0000cfa0: 6465 203d 206e 6f64 655b 2269 6422 5d0a  de = node["id"].
+0000cfb0: 0a20 2020 2023 2044 656c 6574 6520 6e6f  .    # Delete no
+0000cfc0: 6465 0a20 2020 2064 656c 6574 655f 6e6f  de.    delete_no
+0000cfd0: 6465 2869 645f 6e6f 6465 290a 0a0a 6465  de(id_node)...de
+0000cfe0: 6620 6465 6c65 7465 5f6e 6f64 6528 6964  f delete_node(id
+0000cff0: 5f6e 6f64 653a 2069 6e74 2920 2d3e 2041  _node: int) -> A
+0000d000: 6e79 3a0a 2020 2020 2222 2244 656c 6574  ny:.    """Delet
+0000d010: 6520 6e6f 6465 2066 726f 6d20 6461 7461  e node from data
+0000d020: 6261 7365 2067 6976 656e 2069 7473 2049  base given its I
+0000d030: 442e 0a0a 2020 2020 3a72 6574 7572 6e3a  D...    :return:
+0000d040: 2041 206d 6573 7361 6765 2074 656c 6c69   A message telli
+0000d050: 6e67 2068 6f77 2074 6865 206f 7065 7261  ng how the opera
+0000d060: 7469 6f6e 2065 7865 6375 7465 642e 0a0a  tion executed...
+0000d070: 2020 2020 3a70 6172 616d 2069 645f 6e6f      :param id_no
+0000d080: 6465 3a20 5468 6520 6e6f 6465 2049 442e  de: The node ID.
+0000d090: 0a0a 2020 2020 2222 220a 0a20 2020 2023  ..    """..    #
+0000d0a0: 2046 6574 6368 2076 6972 7475 616c 206e   Fetch virtual n
+0000d0b0: 6f64 6520 6e65 7477 6f72 6b20 696e 7465  ode network inte
+0000d0c0: 7266 6163 6573 0a20 2020 206e 6574 776f  rfaces.    netwo
+0000d0d0: 726b 5f69 6e74 6572 6661 6365 7320 3d20  rk_interfaces = 
+0000d0e0: 6665 7463 685f 6e6f 6465 5f6e 6574 776f  fetch_node_netwo
+0000d0f0: 726b 5f69 6e74 6572 6661 6365 7328 6964  rk_interfaces(id
+0000d100: 5f6e 6f64 6529 0a0a 2020 2020 2320 4465  _node)..    # De
+0000d110: 6c65 7465 2065 6163 6820 6e65 7477 6f72  lete each networ
+0000d120: 6b20 696e 7465 7266 6163 6573 0a20 2020  k interfaces.   
+0000d130: 2066 6f72 206e 6574 776f 726b 5f69 6e74   for network_int
+0000d140: 6572 6661 6365 2069 6e20 6e65 7477 6f72  erface in networ
+0000d150: 6b5f 696e 7465 7266 6163 6573 3a0a 2020  k_interfaces:.  
+0000d160: 2020 2020 2020 6465 6c65 7465 5f6e 6574        delete_net
+0000d170: 776f 726b 5f69 6e74 6572 6661 6365 286e  work_interface(n
+0000d180: 6574 776f 726b 5f69 6e74 6572 6661 6365  etwork_interface
+0000d190: 5b22 6964 225d 290a 0a20 2020 2023 2044  ["id"])..    # D
+0000d1a0: 656c 6574 6520 6e6f 6465 0a20 2020 2072  elete node.    r
+0000d1b0: 6573 756c 7420 3d20 5f64 656c 6574 6528  esult = _delete(
+0000d1c0: 6622 2f6e 6f64 652f 7b69 645f 6e6f 6465  f"/node/{id_node
+0000d1d0: 7d22 290a 0a20 2020 2069 6620 7265 7375  }")..    if resu
+0000d1e0: 6c74 2e73 7461 7475 735f 636f 6465 2021  lt.status_code !
+0000d1f0: 3d20 3230 303a 0a20 2020 2020 2020 205f  = 200:.        _
+0000d200: 6861 6e64 6c65 5f65 7272 6f72 2872 6573  handle_error(res
+0000d210: 756c 742c 2022 4361 6e6e 6f74 2064 656c  ult, "Cannot del
+0000d220: 6574 6520 6e6f 6465 2229 0a0a 2020 2020  ete node")..    
+0000d230: 7265 7475 726e 2072 6573 756c 742e 6a73  return result.js
+0000d240: 6f6e 2829 0a0a 0a64 6566 2066 6574 6368  on()...def fetch
+0000d250: 5f6e 6f64 6573 2869 645f 7369 6d75 6c61  _nodes(id_simula
+0000d260: 7469 6f6e 3a20 696e 7429 202d 3e20 416e  tion: int) -> An
+0000d270: 793a 0a20 2020 2022 2222 5265 7475 726e  y:.    """Return
+0000d280: 2073 696d 756c 6174 696f 6e20 6e6f 6465   simulation node
+0000d290: 7320 6469 6374 2067 6976 656e 0a20 2020  s dict given.   
+0000d2a0: 2061 2073 696d 756c 6174 696f 6e20 4944   a simulation ID
+0000d2b0: 2c20 7768 6572 6520 6b65 7973 2061 7265  , where keys are
+0000d2c0: 206e 6f64 6520 6e61 6d65 732e 0a0a 2020   node names...  
+0000d2d0: 2020 3a72 6574 7572 6e3a 2054 6865 206e    :return: The n
+0000d2e0: 6f64 6520 6c69 7374 2e0a 0a20 2020 203a  ode list...    :
+0000d2f0: 7061 7261 6d20 6964 5f73 696d 756c 6174  param id_simulat
+0000d300: 696f 6e3a 2054 6865 2073 696d 756c 6174  ion: The simulat
+0000d310: 696f 6e20 4944 2e0a 0a20 2020 2022 2222  ion ID...    """
+0000d320: 0a20 2020 2072 6573 756c 7420 3d20 5f67  .    result = _g
+0000d330: 6574 2866 222f 7369 6d75 6c61 7469 6f6e  et(f"/simulation
+0000d340: 2f7b 6964 5f73 696d 756c 6174 696f 6e7d  /{id_simulation}
+0000d350: 2f6e 6f64 6522 290a 0a20 2020 2069 6620  /node")..    if 
+0000d360: 7265 7375 6c74 2e73 7461 7475 735f 636f  result.status_co
+0000d370: 6465 2021 3d20 3230 303a 0a20 2020 2020  de != 200:.     
+0000d380: 2020 205f 6861 6e64 6c65 5f65 7272 6f72     _handle_error
+0000d390: 2872 6573 756c 742c 2022 4361 6e6e 6f74  (result, "Cannot
+0000d3a0: 2072 6574 7269 6576 6520 6e6f 6465 7320   retrieve nodes 
+0000d3b0: 6672 6f6d 2049 5420 5369 6d75 6c61 7469  from IT Simulati
+0000d3c0: 6f6e 2041 5049 2229 0a0a 2020 2020 7265  on API")..    re
+0000d3d0: 7475 726e 2072 6573 756c 742e 6a73 6f6e  turn result.json
+0000d3e0: 2829 0a0a 0a64 6566 2066 6574 6368 5f76  ()...def fetch_v
+0000d3f0: 6972 7475 616c 5f6d 6163 6869 6e65 7328  irtual_machines(
+0000d400: 6964 5f73 696d 756c 6174 696f 6e3a 2069  id_simulation: i
+0000d410: 6e74 2920 2d3e 204c 6973 745b 6469 6374  nt) -> List[dict
+0000d420: 5d3a 0a20 2020 2022 2222 5265 7475 726e  ]:.    """Return
+0000d430: 2073 696d 756c 6174 696f 6e20 7669 7274   simulation virt
+0000d440: 7561 6c20 6d61 6368 696e 6573 2064 6963  ual machines dic
+0000d450: 7420 6769 7665 6e20 6120 7369 6d75 6c61  t given a simula
+0000d460: 7469 6f6e 2049 442c 0a20 2020 2077 6865  tion ID,.    whe
+0000d470: 7265 206b 6579 7320 6172 6520 7669 7274  re keys are virt
+0000d480: 7561 6c20 6d61 6368 696e 6520 6e61 6d65  ual machine name
+0000d490: 732e 0a0a 2020 2020 3a72 6574 7572 6e3a  s...    :return:
+0000d4a0: 2054 6865 206c 6973 7420 6f66 2076 6972   The list of vir
+0000d4b0: 7475 616c 206d 6163 6869 6e65 732e 0a0a  tual machines...
+0000d4c0: 2020 2020 3a70 6172 616d 2069 645f 7369      :param id_si
+0000d4d0: 6d75 6c61 7469 6f6e 3a20 5468 6520 7369  mulation: The si
+0000d4e0: 6d75 6c61 7469 6f6e 2049 442e 0a0a 2020  mulation ID...  
+0000d4f0: 2020 2222 220a 2020 2020 7265 7375 6c74    """.    result
+0000d500: 7320 3d20 6665 7463 685f 6e6f 6465 7328  s = fetch_nodes(
+0000d510: 6964 5f73 696d 756c 6174 696f 6e29 0a0a  id_simulation)..
+0000d520: 2020 2020 766d 5f6f 6e6c 7920 3d20 6669      vm_only = fi
+0000d530: 6c74 6572 286c 616d 6264 6120 6d3a 206d  lter(lambda m: m
+0000d540: 5b22 7479 7065 225d 203d 3d20 2276 6972  ["type"] == "vir
+0000d550: 7475 616c 5f6d 6163 6869 6e65 222c 2072  tual_machine", r
+0000d560: 6573 756c 7473 290a 2020 2020 7265 7475  esults).    retu
+0000d570: 726e 206c 6973 7428 766d 5f6f 6e6c 7929  rn list(vm_only)
+0000d580: 0a0a 0a64 6566 2064 656c 6574 655f 6e6f  ...def delete_no
+0000d590: 6465 7328 6964 5f73 696d 756c 6174 696f  des(id_simulatio
+0000d5a0: 6e3a 2069 6e74 2920 2d3e 2073 7472 3a0a  n: int) -> str:.
+0000d5b0: 2020 2020 2222 2244 656c 6574 6520 7369      """Delete si
+0000d5c0: 6d75 6c61 7469 6f6e 206e 6f64 6573 2067  mulation nodes g
+0000d5d0: 6976 656e 2061 2073 696d 756c 6174 696f  iven a simulatio
+0000d5e0: 6e20 4944 2e0a 0a20 2020 203a 7265 7475  n ID...    :retu
+0000d5f0: 726e 3a20 4120 6d65 7373 6167 6520 7465  rn: A message te
+0000d600: 6c6c 696e 6720 686f 7720 7468 6520 6f70  lling how the op
+0000d610: 6572 6174 696f 6e20 6578 6563 7574 6564  eration executed
+0000d620: 2e0a 0a20 2020 203a 7061 7261 6d20 6964  ...    :param id
+0000d630: 5f73 696d 756c 6174 696f 6e3a 2054 6865  _simulation: The
+0000d640: 2073 696d 756c 6174 696f 6e20 4944 2e0a   simulation ID..
+0000d650: 0a20 2020 2022 2222 0a0a 2020 2020 2320  .    """..    # 
+0000d660: 4665 7463 6820 7369 6d75 6c61 7469 6f6e  Fetch simulation
+0000d670: 206e 6f64 6573 0a20 2020 2072 6573 756c   nodes.    resul
+0000d680: 7420 3d20 5f67 6574 2866 222f 7369 6d75  t = _get(f"/simu
+0000d690: 6c61 7469 6f6e 2f7b 6964 5f73 696d 756c  lation/{id_simul
+0000d6a0: 6174 696f 6e7d 2f6e 6f64 6522 290a 0a20  ation}/node").. 
+0000d6b0: 2020 2069 6620 7265 7375 6c74 2e73 7461     if result.sta
+0000d6c0: 7475 735f 636f 6465 2021 3d20 3230 303a  tus_code != 200:
+0000d6d0: 0a20 2020 2020 2020 205f 6861 6e64 6c65  .        _handle
+0000d6e0: 5f65 7272 6f72 2872 6573 756c 742c 2022  _error(result, "
+0000d6f0: 4361 6e6e 6f74 2064 656c 6574 6520 7369  Cannot delete si
+0000d700: 6d75 6c61 7469 6f6e 206e 6f64 6573 2229  mulation nodes")
+0000d710: 0a0a 2020 2020 6e6f 6465 735f 6c69 7374  ..    nodes_list
+0000d720: 203d 2072 6573 756c 742e 6a73 6f6e 2829   = result.json()
+0000d730: 0a0a 2020 2020 2320 4465 6c65 7465 2065  ..    # Delete e
+0000d740: 6163 6820 6e6f 6465 0a20 2020 2066 6f72  ach node.    for
+0000d750: 206e 6f64 6520 696e 206e 6f64 6573 5f6c   node in nodes_l
+0000d760: 6973 743a 0a20 2020 2020 2020 2064 656c  ist:.        del
+0000d770: 6574 655f 6e6f 6465 286e 6f64 655b 2269  ete_node(node["i
+0000d780: 6422 5d29 0a0a 2020 2020 7265 7375 6c74  d"])..    result
+0000d790: 5f6a 736f 6e20 3d20 227b 7d22 0a20 2020  _json = "{}".   
+0000d7a0: 2072 6574 7572 6e20 7265 7375 6c74 5f6a   return result_j
+0000d7b0: 736f 6e0a 0a0a 6465 6620 7570 6461 7465  son...def update
+0000d7c0: 5f6e 6f64 6528 6e6f 6465 5f69 643a 2069  _node(node_id: i
+0000d7d0: 6e74 2c20 6e6f 6465 5f64 6963 743a 2064  nt, node_dict: d
+0000d7e0: 6963 7429 202d 3e20 416e 793a 0a20 2020  ict) -> Any:.   
+0000d7f0: 2022 2222 5570 6461 7465 206e 6f64 6520   """Update node 
+0000d800: 696e 666f 726d 6174 696f 6e20 6769 7665  information give
+0000d810: 6e20 6120 6e6f 6465 2069 6420 616e 6420  n a node id and 
+0000d820: 6120 6469 6374 2063 6f6e 7461 696e 696e  a dict containin
+0000d830: 670a 2020 2020 6e6f 6465 2064 6174 612e  g.    node data.
+0000d840: 0a0a 2020 2020 3a72 6574 7572 6e3a 2041  ..    :return: A
+0000d850: 206d 6573 7361 6765 2074 656c 6c69 6e67   message telling
+0000d860: 2068 6f77 2074 6865 206f 7065 7261 7469   how the operati
+0000d870: 6f6e 2065 7865 6375 7465 642e 0a0a 2020  on executed...  
+0000d880: 2020 3a70 6172 616d 206e 6f64 655f 6964    :param node_id
+0000d890: 3a20 5468 6520 6e6f 6465 2049 442e 0a20  : The node ID.. 
+0000d8a0: 2020 203a 7061 7261 6d20 6e6f 6465 5f64     :param node_d
+0000d8b0: 6963 743a 2054 6865 2064 6963 7420 636f  ict: The dict co
+0000d8c0: 6e74 6169 6e69 6e67 2074 6865 2065 6e74  ntaining the ent
+0000d8d0: 7269 6573 2074 6f20 7570 6461 7465 2e0a  ries to update..
+0000d8e0: 0a20 2020 2022 2222 0a20 2020 2064 6174  .    """.    dat
+0000d8f0: 6120 3d20 6a73 6f6e 2e64 756d 7073 286e  a = json.dumps(n
+0000d900: 6f64 655f 6469 6374 290a 2020 2020 7265  ode_dict).    re
+0000d910: 7375 6c74 203d 205f 7075 7428 0a20 2020  sult = _put(.   
+0000d920: 2020 2020 2066 222f 6e6f 6465 2f7b 6e6f       f"/node/{no
+0000d930: 6465 5f69 647d 222c 0a20 2020 2020 2020  de_id}",.       
+0000d940: 2064 6174 613d 6461 7461 2c0a 2020 2020   data=data,.    
+0000d950: 2020 2020 6865 6164 6572 733d 7b22 436f      headers={"Co
+0000d960: 6e74 656e 742d 5479 7065 223a 2022 6170  ntent-Type": "ap
+0000d970: 706c 6963 6174 696f 6e2f 6a73 6f6e 227d  plication/json"}
+0000d980: 2c0a 2020 2020 290a 0a20 2020 2069 6620  ,.    )..    if 
+0000d990: 7265 7375 6c74 2e73 7461 7475 735f 636f  result.status_co
+0000d9a0: 6465 2021 3d20 3230 303a 0a20 2020 2020  de != 200:.     
+0000d9b0: 2020 205f 6861 6e64 6c65 5f65 7272 6f72     _handle_error
+0000d9c0: 2872 6573 756c 742c 2022 4361 6e6e 6f74  (result, "Cannot
+0000d9d0: 2075 7064 6174 6520 6e6f 6465 2069 6e66   update node inf
+0000d9e0: 6f72 6d61 7469 6f6e 2077 6974 6820 636f  ormation with co
+0000d9f0: 7265 2041 5049 2229 0a0a 2020 2020 7265  re API")..    re
+0000da00: 7475 726e 2072 6573 756c 742e 6a73 6f6e  turn result.json
+0000da10: 2829 0a0a 0a64 6566 2067 6574 5f6e 6f64  ()...def get_nod
+0000da20: 655f 6465 6661 756c 745f 6761 7465 7761  e_default_gatewa
+0000da30: 7928 6964 5f6e 6f64 653a 2069 6e74 2920  y(id_node: int) 
+0000da40: 2d3e 204f 7074 696f 6e61 6c5b 7374 725d  -> Optional[str]
+0000da50: 3a0a 2020 2020 2222 2252 6574 7269 6576  :.    """Retriev
+0000da60: 6520 6e6f 6465 2064 6566 6175 6c74 2067  e node default g
+0000da70: 6174 6577 6179 2c20 7768 6963 6820 6361  ateway, which ca
+0000da80: 6e20 6569 7468 6572 2062 6520 616e 2049  n either be an I
+0000da90: 5020 6164 6472 6573 730a 2020 2020 6f66  P address.    of
+0000daa0: 2074 6865 2066 6f72 6d20 7878 2e78 782e   the form xx.xx.
+0000dab0: 7878 2e78 7820 6f72 204e 6f6e 6520 6966  xx.xx or None if
+0000dac0: 206e 6f20 6761 7465 7761 7920 6973 2073   no gateway is s
+0000dad0: 6574 2e0a 0a20 2020 203a 7265 7475 726e  et...    :return
+0000dae0: 3a20 5468 6520 6e6f 6465 2064 6566 6175  : The node defau
+0000daf0: 6c74 2067 6174 6577 6179 2e0a 0a20 2020  lt gateway...   
+0000db00: 203a 7061 7261 6d20 6964 5f6e 6f64 653a   :param id_node:
+0000db10: 2054 6865 206e 6f64 6520 4944 2e0a 0a20   The node ID... 
+0000db20: 2020 2022 2222 0a0a 2020 2020 7265 7375     """..    resu
+0000db30: 6c74 203d 205f 6765 7428 6622 2f6e 6f64  lt = _get(f"/nod
+0000db40: 652f 7b69 645f 6e6f 6465 7d2f 6465 6661  e/{id_node}/defa
+0000db50: 756c 745f 6761 7465 7761 7922 290a 0a20  ult_gateway").. 
+0000db60: 2020 2069 6620 7265 7375 6c74 2e73 7461     if result.sta
+0000db70: 7475 735f 636f 6465 2021 3d20 3230 303a  tus_code != 200:
+0000db80: 0a20 2020 2020 2020 205f 6861 6e64 6c65  .        _handle
+0000db90: 5f65 7272 6f72 280a 2020 2020 2020 2020  _error(.        
+0000dba0: 2020 2020 7265 7375 6c74 2c20 2243 616e      result, "Can
+0000dbb0: 6e6f 7420 7265 7472 6965 7665 206e 6f64  not retrieve nod
+0000dbc0: 6520 6465 6661 756c 7420 6761 7465 7761  e default gatewa
+0000dbd0: 7920 6672 6f6d 2049 5420 5369 6d75 6c61  y from IT Simula
+0000dbe0: 7469 6f6e 2041 5049 220a 2020 2020 2020  tion API".      
+0000dbf0: 2020 290a 0a20 2020 2064 6566 6175 6c74    )..    default
+0000dc00: 5f67 6174 6577 6179 203d 2072 6573 756c  _gateway = resul
+0000dc10: 742e 6a73 6f6e 2829 0a0a 2020 2020 7265  t.json()..    re
+0000dc20: 7475 726e 2064 6566 6175 6c74 5f67 6174  turn default_gat
+0000dc30: 6577 6179 0a0a 0a64 6566 2067 6574 5f6e  eway...def get_n
+0000dc40: 6f64 655f 7374 6174 6973 7469 6373 5f62  ode_statistics_b
+0000dc50: 795f 6964 2869 645f 6e6f 6465 3a20 696e  y_id(id_node: in
+0000dc60: 7429 202d 3e20 416e 793a 0a20 2020 2022  t) -> Any:.    "
+0000dc70: 2222 0a20 2020 2052 6574 7572 6e20 6167  "".    Return ag
+0000dc80: 6772 6567 6174 6564 2073 7461 7469 7374  gregated statist
+0000dc90: 6963 7320 6672 6f6d 2043 5055 2c20 6d65  ics from CPU, me
+0000dca0: 6d6f 7279 2c20 626c 6f63 6b20 6465 7669  mory, block devi
+0000dcb0: 6365 7320 616e 6420 6e65 7477 6f72 6b20  ces and network 
+0000dcc0: 696e 7465 7266 6163 6573 2e0a 2020 2020  interfaces..    
+0000dcd0: 4e6f 7465 3a20 796f 7520 6361 6e20 6765  Note: you can ge
+0000dce0: 7420 7468 6520 6e6f 6465 2049 4473 2075  t the node IDs u
+0000dcf0: 7369 6e67 2074 6865 2073 696d 755f 7374  sing the simu_st
+0000dd00: 6174 7573 2063 6f6d 6d61 6e64 2028 6f72  atus command (or
+0000dd10: 2074 6865 2066 6574 6368 5f73 696d 756c   the fetch_simul
+0000dd20: 6174 696f 6e73 2829 2066 756e 6374 696f  ations() functio
+0000dd30: 6e29 2e0a 0a20 2020 203a 7265 7475 726e  n)...    :return
+0000dd40: 3a20 5468 6520 6e6f 6465 2073 7461 7469  : The node stati
+0000dd50: 7374 6963 732e 0a0a 2020 2020 3a70 6172  stics...    :par
+0000dd60: 616d 2069 645f 6e6f 6465 3a20 5468 6520  am id_node: The 
+0000dd70: 6e6f 6465 2049 442e 0a0a 2020 2020 2222  node ID...    ""
+0000dd80: 220a 2020 2020 7265 7375 6c74 203d 205f  ".    result = _
+0000dd90: 6765 7428 6622 2f6e 6f64 652f 7b69 645f  get(f"/node/{id_
+0000dda0: 6e6f 6465 7d2f 7374 6174 7322 290a 0a20  node}/stats").. 
+0000ddb0: 2020 2069 6620 7265 7375 6c74 2e73 7461     if result.sta
+0000ddc0: 7475 735f 636f 6465 2021 3d20 3230 303a  tus_code != 200:
+0000ddd0: 0a20 2020 2020 2020 205f 6861 6e64 6c65  .        _handle
+0000dde0: 5f65 7272 6f72 2872 6573 756c 742c 2022  _error(result, "
+0000ddf0: 4361 6e6e 6f74 2072 6574 7269 6576 6520  Cannot retrieve 
+0000de00: 6e6f 6465 2073 7461 7469 7374 6963 7322  node statistics"
+0000de10: 290a 0a20 2020 2072 6574 7572 6e20 7265  )..    return re
+0000de20: 7375 6c74 2e6a 736f 6e28 290a 0a0a 6465  sult.json()...de
+0000de30: 6620 6e6f 6465 5f6c 6f67 7328 6964 5f6e  f node_logs(id_n
+0000de40: 6f64 653a 2069 6e74 2920 2d3e 2041 6e79  ode: int) -> Any
+0000de50: 3a0a 2020 2020 2222 220a 2020 2020 5265  :.    """.    Re
+0000de60: 7472 6965 7665 206c 6f67 7320 6672 6f6d  trieve logs from
+0000de70: 2073 7065 6369 6669 6564 206e 6f64 6520   specified node 
+0000de80: 286f 6e6c 7920 776f 726b 2066 6f72 2044  (only work for D
+0000de90: 6f63 6b65 7220 6e6f 6465 292e 0a0a 2020  ocker node)...  
+0000dea0: 2020 3a72 6574 7572 6e3a 2054 6865 206c    :return: The l
+0000deb0: 6f67 7320 6173 2061 2073 7472 696e 672e  ogs as a string.
+0000dec0: 0a0a 2020 2020 3a70 6172 616d 2069 645f  ..    :param id_
+0000ded0: 6e6f 6465 3a20 5468 6520 6e6f 6465 2049  node: The node I
+0000dee0: 442e 0a0a 2020 2020 2222 220a 0a20 2020  D...    """..   
+0000def0: 2023 2043 6865 636b 2074 6861 7420 7468   # Check that th
+0000df00: 6520 7461 7267 6574 206e 6f64 6520 6973  e target node is
+0000df10: 2061 2064 6f63 6b65 7220 6e6f 6465 2028   a docker node (
+0000df20: 6e6f 6465 5f65 7865 6320 6f6e 6c79 0a20  node_exec only. 
+0000df30: 2020 2023 2077 6f72 6b73 2066 6f72 2044     # works for D
+0000df40: 6f63 6b65 7220 6e6f 6465 2066 6f72 206e  ocker node for n
+0000df50: 6f77 290a 2020 2020 6e6f 6465 203d 2066  ow).    node = f
+0000df60: 6574 6368 5f6e 6f64 6528 6964 5f6e 6f64  etch_node(id_nod
+0000df70: 6529 0a20 2020 2069 6620 6e6f 6465 5b22  e).    if node["
+0000df80: 7479 7065 225d 2021 3d20 2264 6f63 6b65  type"] != "docke
+0000df90: 7222 3a0a 2020 2020 2020 2020 7261 6973  r":.        rais
+0000dfa0: 6520 4578 6365 7074 696f 6e28 2243 616e  e Exception("Can
+0000dfb0: 6e6f 7420 6578 6563 7574 6520 636f 6d6d  not execute comm
+0000dfc0: 616e 6420 666f 7220 6e6f 6465 7320 6469  and for nodes di
+0000dfd0: 6666 6572 656e 7420 6672 6f6d 2064 6f63  fferent from doc
+0000dfe0: 6b65 7220 6e6f 6465 7322 290a 0a20 2020  ker nodes")..   
+0000dff0: 2072 6573 756c 7420 3d20 5f67 6574 2866   result = _get(f
+0000e000: 222f 6e6f 6465 2f7b 6964 5f6e 6f64 657d  "/node/{id_node}
+0000e010: 2f6c 6f67 7322 290a 0a20 2020 2069 6620  /logs")..    if 
+0000e020: 7265 7375 6c74 2e73 7461 7475 735f 636f  result.status_co
+0000e030: 6465 2021 3d20 3230 303a 0a20 2020 2020  de != 200:.     
+0000e040: 2020 205f 6861 6e64 6c65 5f65 7272 6f72     _handle_error
+0000e050: 2872 6573 756c 742c 2022 4361 6e6e 6f74  (result, "Cannot
+0000e060: 2072 6574 7269 6576 6520 6c6f 6773 2066   retrieve logs f
+0000e070: 726f 6d20 4954 2053 696d 756c 6174 696f  rom IT Simulatio
+0000e080: 6e20 4150 4922 290a 0a20 2020 206c 6f67  n API")..    log
+0000e090: 7320 3d20 7265 7375 6c74 2e6a 736f 6e28  s = result.json(
+0000e0a0: 290a 0a20 2020 2072 6574 7572 6e20 6c6f  )..    return lo
+0000e0b0: 6773 0a0a 0a64 6566 206e 6f64 655f 6578  gs...def node_ex
+0000e0c0: 6563 2869 645f 6e6f 6465 3a20 696e 742c  ec(id_node: int,
+0000e0d0: 2063 6f6d 6d61 6e64 3a20 7374 7229 202d   command: str) -
+0000e0e0: 3e20 416e 793a 0a20 2020 2022 2222 0a20  > Any:.    """. 
+0000e0f0: 2020 2045 7865 6375 7465 2061 2063 6f6d     Execute a com
+0000e100: 6d61 6e64 206f 6e20 7370 6563 6966 6965  mand on specifie
+0000e110: 6420 6e6f 6465 2028 6f6e 6c79 2077 6f72  d node (only wor
+0000e120: 6b20 666f 7220 446f 636b 6572 206e 6f64  k for Docker nod
+0000e130: 6529 2e0a 0a20 2020 203a 7265 7475 726e  e)...    :return
+0000e140: 3a20 5265 7475 726e 2061 2074 7570 6c65  : Return a tuple
+0000e150: 2028 6578 6974 5f63 6f64 653a 2069 6e74   (exit_code: int
+0000e160: 2c20 7374 646f 7574 3a20 7374 722c 2073  , stdout: str, s
+0000e170: 7464 6572 723a 2073 7472 2920 6f66 2074  tderr: str) of t
+0000e180: 6865 2065 7865 6375 7465 6420 636f 6d6d  he executed comm
+0000e190: 616e 642e 0a0a 2020 2020 3a70 6172 616d  and...    :param
+0000e1a0: 2069 645f 6e6f 6465 3a20 5468 6520 6e6f   id_node: The no
+0000e1b0: 6465 2049 442e 0a20 2020 203a 7061 7261  de ID..    :para
+0000e1c0: 6d20 636f 6d6d 616e 643a 2054 6865 2063  m command: The c
+0000e1d0: 6f6d 6d61 6e64 2074 6f20 6578 6563 7574  ommand to execut
+0000e1e0: 6520 6f6e 2074 6865 206e 6f64 652e 0a0a  e on the node...
+0000e1f0: 2020 2020 2222 220a 0a20 2020 2023 2043      """..    # C
+0000e200: 6865 636b 2074 6861 7420 7468 6520 7461  heck that the ta
+0000e210: 7267 6574 206e 6f64 6520 6973 2061 2064  rget node is a d
+0000e220: 6f63 6b65 7220 6e6f 6465 2028 6e6f 6465  ocker node (node
+0000e230: 5f65 7865 6320 6f6e 6c79 0a20 2020 2023  _exec only.    #
+0000e240: 2077 6f72 6b73 2066 6f72 2044 6f63 6b65   works for Docke
+0000e250: 7220 6e6f 6465 2066 6f72 206e 6f77 290a  r node for now).
+0000e260: 2020 2020 6e6f 6465 203d 2066 6574 6368      node = fetch
+0000e270: 5f6e 6f64 6528 6964 5f6e 6f64 6529 0a20  _node(id_node). 
+0000e280: 2020 2069 6620 6e6f 6465 5b22 7479 7065     if node["type
+0000e290: 225d 2021 3d20 2264 6f63 6b65 7222 3a0a  "] != "docker":.
+0000e2a0: 2020 2020 2020 2020 7261 6973 6520 4578          raise Ex
+0000e2b0: 6365 7074 696f 6e28 2243 616e 6e6f 7420  ception("Cannot 
+0000e2c0: 6578 6563 7574 6520 636f 6d6d 616e 6420  execute command 
+0000e2d0: 666f 7220 6e6f 6465 7320 6469 6666 6572  for nodes differ
+0000e2e0: 656e 7420 6672 6f6d 2064 6f63 6b65 7220  ent from docker 
+0000e2f0: 6e6f 6465 7322 290a 0a20 2020 2073 7461  nodes")..    sta
+0000e300: 7475 735f 6b65 7920 3d20 2273 7461 7475  tus_key = "statu
+0000e310: 7322 0a20 2020 2065 7869 745f 636f 6465  s".    exit_code
+0000e320: 203d 2022 6578 6974 5f63 6f64 6522 0a20   = "exit_code". 
+0000e330: 2020 2073 7464 6f75 7420 3d20 2273 7464     stdout = "std
+0000e340: 6f75 7422 0a20 2020 2073 7464 6572 7220  out".    stderr 
+0000e350: 3d20 2273 7464 6572 7222 0a0a 2020 2020  = "stderr"..    
+0000e360: 706f 7374 5f64 6174 6120 3d20 7b22 636f  post_data = {"co
+0000e370: 6d6d 616e 6422 3a20 636f 6d6d 616e 647d  mmand": command}
+0000e380: 0a20 2020 2064 6174 6120 3d20 6a73 6f6e  .    data = json
+0000e390: 2e64 756d 7073 2870 6f73 745f 6461 7461  .dumps(post_data
+0000e3a0: 290a 2020 2020 7265 7375 6c74 203d 205f  ).    result = _
+0000e3b0: 706f 7374 280a 2020 2020 2020 2020 6622  post(.        f"
+0000e3c0: 2f6e 6f64 652f 7b69 645f 6e6f 6465 7d2f  /node/{id_node}/
+0000e3d0: 6578 6563 222c 2064 6174 613d 6461 7461  exec", data=data
+0000e3e0: 2c20 6865 6164 6572 733d 7b22 436f 6e74  , headers={"Cont
+0000e3f0: 656e 742d 5479 7065 223a 2022 6170 706c  ent-Type": "appl
+0000e400: 6963 6174 696f 6e2f 6a73 6f6e 227d 0a20  ication/json"}. 
+0000e410: 2020 2029 0a0a 2020 2020 6966 2028 0a20     )..    if (. 
+0000e420: 2020 2020 2020 2072 6573 756c 742e 7374         result.st
+0000e430: 6174 7573 5f63 6f64 6520 213d 2032 3030  atus_code != 200
+0000e440: 0a20 2020 2020 2020 206f 7220 7374 6174  .        or stat
+0000e450: 7573 5f6b 6579 206e 6f74 2069 6e20 7265  us_key not in re
+0000e460: 7375 6c74 2e6a 736f 6e28 290a 2020 2020  sult.json().    
+0000e470: 2020 2020 6f72 2072 6573 756c 742e 6a73      or result.js
+0000e480: 6f6e 2829 5b73 7461 7475 735f 6b65 795d  on()[status_key]
+0000e490: 2021 3d20 2253 5441 5254 4544 220a 2020   != "STARTED".  
+0000e4a0: 2020 293a 0a20 2020 2020 2020 205f 6861    ):.        _ha
+0000e4b0: 6e64 6c65 5f65 7272 6f72 2872 6573 756c  ndle_error(resul
+0000e4c0: 742c 2022 4361 6e6e 6f74 2069 6e69 7469  t, "Cannot initi
+0000e4d0: 6174 6520 6578 6563 2063 6f6d 6d61 6e64  ate exec command
+0000e4e0: 2066 726f 6d20 4954 2053 696d 756c 6174   from IT Simulat
+0000e4f0: 696f 6e20 4150 4922 290a 0a20 2020 206c  ion API")..    l
+0000e500: 6f67 6765 722e 696e 666f 2866 225b 2b5d  ogger.info(f"[+]
+0000e510: 2045 7865 6375 7469 6e67 2063 6f6d 6d61   Executing comma
+0000e520: 6e64 2027 7b63 6f6d 6d61 6e64 7d27 2066  nd '{command}' f
+0000e530: 6f72 206e 6f64 6520 277b 6964 5f6e 6f64  or node '{id_nod
+0000e540: 657d 272e 2e2e 2229 0a0a 2020 2020 2320  e}'...")..    # 
+0000e550: 5761 6974 2066 6f72 2074 6865 206f 7065  Wait for the ope
+0000e560: 7261 7469 6f6e 2074 6f20 6265 2063 6f6d  ration to be com
+0000e570: 706c 6574 6564 2069 6e20 6261 636b 656e  pleted in backen
+0000e580: 640a 2020 2020 2320 4e6f 7465 203a 206c  d.    # Note : l
+0000e590: 6f6f 7020 696e 7370 6972 6564 2066 726f  oop inspired fro
+0000e5a0: 6d20 5f73 696d 756c 6174 696f 6e5f 6578  m _simulation_ex
+0000e5b0: 6563 7574 655f 6f70 6572 6174 696f 6e0a  ecute_operation.
+0000e5c0: 2020 2020 7768 696c 6520 5472 7565 3a0a      while True:.
+0000e5d0: 2020 2020 2020 2020 2320 536c 6565 7020          # Sleep 
+0000e5e0: 6265 666f 7265 206e 6578 7420 6974 6572  before next iter
+0000e5f0: 6174 696f 6e0a 2020 2020 2020 2020 7469  ation.        ti
+0000e600: 6d65 2e73 6c65 6570 2832 290a 0a20 2020  me.sleep(2)..   
+0000e610: 2020 2020 2023 2046 6574 6368 2074 6865       # Fetch the
+0000e620: 2063 7572 7265 6e74 2073 7461 7475 7320   current status 
+0000e630: 6f66 2074 6865 206d 656d 6475 6d70 0a20  of the memdump. 
+0000e640: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+0000e650: 5f67 6574 2866 222f 6e6f 6465 2f7b 6964  _get(f"/node/{id
+0000e660: 5f6e 6f64 657d 2f65 7865 635f 7374 6174  _node}/exec_stat
+0000e670: 7573 2229 0a0a 2020 2020 2020 2020 6966  us")..        if
+0000e680: 2072 6573 756c 742e 7374 6174 7573 5f63   result.status_c
+0000e690: 6f64 6520 213d 2032 3030 3a0a 2020 2020  ode != 200:.    
+0000e6a0: 2020 2020 2020 2020 5f68 616e 646c 655f          _handle_
+0000e6b0: 6572 726f 7228 0a20 2020 2020 2020 2020  error(.         
+0000e6c0: 2020 2020 2020 2072 6573 756c 742c 2022         result, "
+0000e6d0: 4361 6e6e 6f74 2067 6574 2073 7461 7475  Cannot get statu
+0000e6e0: 7320 6f66 2065 7865 6320 636f 6d6d 616e  s of exec comman
+0000e6f0: 6420 6672 6f6d 2049 5420 5369 6d75 6c61  d from IT Simula
+0000e700: 7469 6f6e 2041 5049 220a 2020 2020 2020  tion API".      
+0000e710: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+0000e720: 2072 6573 756c 745f 6a73 6f6e 203d 2072   result_json = r
+0000e730: 6573 756c 742e 6a73 6f6e 2829 0a20 2020  esult.json().   
+0000e740: 2020 2020 2069 6620 6e6f 7420 2861 6c6c       if not (all
+0000e750: 286b 2069 6e20 7265 7375 6c74 5f6a 736f  (k in result_jso
+0000e760: 6e20 666f 7220 6b20 696e 2028 6578 6974  n for k in (exit
+0000e770: 5f63 6f64 652c 2073 7464 6f75 742c 2073  _code, stdout, s
+0000e780: 7464 6572 722c 2073 7461 7475 735f 6b65  tderr, status_ke
+0000e790: 7929 2929 3a0a 2020 2020 2020 2020 2020  y))):.          
+0000e7a0: 2020 7261 6973 6520 4578 6365 7074 696f    raise Exceptio
+0000e7b0: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
+0000e7c0: 2020 2066 2243 6f6e 7465 6e74 7320 6f66     f"Contents of
+0000e7d0: 2065 7865 6320 636f 6d6d 616e 6420 7374   exec command st
+0000e7e0: 6174 7573 2075 7064 6174 6520 6973 206e  atus update is n
+0000e7f0: 6f74 2069 6e20 7468 6520 6578 7065 6374  ot in the expect
+0000e800: 6564 2066 6f72 6d61 7420 2861 7474 7269  ed format (attri
+0000e810: 6275 7465 7320 277b 6578 6974 5f63 6f64  butes '{exit_cod
+0000e820: 657d 272c 2027 7b73 7464 6f75 747d 272c  e}', '{stdout}',
+0000e830: 2027 7b73 7464 6572 727d 2720 616e 6420   '{stderr}' and 
+0000e840: 277b 7374 6174 7573 5f6b 6579 7d27 2065  '{status_key}' e
+0000e850: 7870 6563 7465 6429 220a 2020 2020 2020  xpected)".      
+0000e860: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+0000e870: 2023 204c 6f67 2069 6e66 6f20 6f6e 2070   # Log info on p
+0000e880: 726f 6772 6573 7369 6f6e 0a20 2020 2020  rogression.     
+0000e890: 2020 2069 6620 7265 7375 6c74 5f6a 736f     if result_jso
+0000e8a0: 6e5b 7374 6174 7573 5f6b 6579 5d20 3d3d  n[status_key] ==
+0000e8b0: 2022 5354 4152 5445 4422 3a0a 2020 2020   "STARTED":.    
+0000e8c0: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
+0000e8d0: 6e66 6f28 0a20 2020 2020 2020 2020 2020  nfo(.           
+0000e8e0: 2020 2020 2066 2220 205b 2b5d 2043 7572       f"  [+] Cur
+0000e8f0: 7265 6e74 6c79 2077 6169 7469 6e67 2066  rently waiting f
+0000e900: 6f72 2065 7865 6320 636f 6d6d 616e 6420  or exec command 
+0000e910: 666f 7220 6e6f 6465 2027 7b69 645f 6e6f  for node '{id_no
+0000e920: 6465 7d27 2920 746f 2073 7461 7274 2e2e  de}') to start..
+0000e930: 2e22 0a20 2020 2020 2020 2020 2020 2029  .".            )
+0000e940: 0a20 2020 2020 2020 2065 6c69 6620 7265  .        elif re
+0000e950: 7375 6c74 5f6a 736f 6e5b 7374 6174 7573  sult_json[status
+0000e960: 5f6b 6579 5d20 3d3d 2022 5052 4f47 5245  _key] == "PROGRE
+0000e970: 5353 223a 0a20 2020 2020 2020 2020 2020  SS":.           
+0000e980: 206c 6f67 6765 722e 696e 666f 280a 2020   logger.info(.  
+0000e990: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+0000e9a0: 2020 5b2b 5d20 4375 7272 656e 746c 7920    [+] Currently 
+0000e9b0: 7065 7266 6f72 6d69 6e67 2065 7865 6320  performing exec 
+0000e9c0: 636f 6d6d 616e 6420 666f 7220 6e6f 6465  command for node
+0000e9d0: 2027 7b69 645f 6e6f 6465 7d27 292e 2e2e   '{id_node}')...
+0000e9e0: 220a 2020 2020 2020 2020 2020 2020 290a  ".            ).
+0000e9f0: 2020 2020 2020 2020 656c 6966 2072 6573          elif res
+0000ea00: 756c 745f 6a73 6f6e 5b73 7461 7475 735f  ult_json[status_
+0000ea10: 6b65 795d 203d 3d20 2253 5543 4345 5353  key] == "SUCCESS
+0000ea20: 223a 0a20 2020 2020 2020 2020 2020 2062  ":.            b
+0000ea30: 7265 616b 0a20 2020 2020 2020 2065 6c73  reak.        els
+0000ea40: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0000ea50: 6169 7365 2045 7863 6570 7469 6f6e 280a  aise Exception(.
+0000ea60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea70: 2245 7272 6f72 2064 7572 696e 6720 6578  "Error during ex
+0000ea80: 6563 2063 6f6d 6d61 6e64 2066 6f72 206e  ec command for n
+0000ea90: 6f64 6520 7b7d 206f 7065 7261 7469 6f6e  ode {} operation
+0000eaa0: 3a20 277b 7d27 222e 666f 726d 6174 280a  : '{}'".format(.
+0000eab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eac0: 2020 2020 6964 5f6e 6f64 652c 2072 6573      id_node, res
+0000ead0: 756c 745f 6a73 6f6e 5b73 7461 7475 735f  ult_json[status_
+0000eae0: 6b65 795d 0a20 2020 2020 2020 2020 2020  key].           
+0000eaf0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+0000eb00: 2020 2029 0a0a 2020 2020 6c6f 6767 6572     )..    logger
+0000eb10: 2e69 6e66 6f28 225b 2b5d 204e 6f64 6520  .info("[+] Node 
+0000eb20: 6578 6563 2063 6f6d 6d61 6e64 2066 696e  exec command fin
+0000eb30: 6973 6865 6422 290a 0a20 2020 2072 6574  ished")..    ret
+0000eb40: 7572 6e20 2872 6573 756c 745f 6a73 6f6e  urn (result_json
+0000eb50: 5b65 7869 745f 636f 6465 5d2c 2072 6573  [exit_code], res
+0000eb60: 756c 745f 6a73 6f6e 5b73 7464 6f75 745d  ult_json[stdout]
+0000eb70: 2c20 7265 7375 6c74 5f6a 736f 6e5b 7374  , result_json[st
+0000eb80: 6465 7272 5d29 0a0a 0a64 6566 206e 6f64  derr])...def nod
+0000eb90: 655f 6d65 6d6f 7279 6475 6d70 2869 645f  e_memorydump(id_
+0000eba0: 6e6f 6465 3a20 696e 7429 202d 3e20 416e  node: int) -> An
+0000ebb0: 793a 0a20 2020 2022 2222 0a20 2020 2052  y:.    """.    R
+0000ebc0: 6574 7572 6e20 5241 4d20 6475 6d70 206f  eturn RAM dump o
+0000ebd0: 6620 6120 6e6f 6465 2069 6e20 6120 7275  f a node in a ru
+0000ebe0: 6e6e 696e 6720 7369 6d75 6c61 7469 6f6e  nning simulation
+0000ebf0: 0a20 2020 204e 6f74 653a 2079 6f75 2063  .    Note: you c
+0000ec00: 616e 2067 6574 2074 6865 206e 6f64 6520  an get the node 
+0000ec10: 4944 7320 7573 696e 6720 7468 6520 7369  IDs using the si
+0000ec20: 6d75 5f73 7461 7475 7320 636f 6d6d 616e  mu_status comman
+0000ec30: 6420 286f 7220 7468 6520 6665 7463 685f  d (or the fetch_
+0000ec40: 7369 6d75 6c61 7469 6f6e 7328 2920 6675  simulations() fu
+0000ec50: 6e63 7469 6f6e 292e 0a0a 2020 2020 3a72  nction)...    :r
+0000ec60: 6574 7572 6e3a 2041 206d 6573 7361 6765  eturn: A message
+0000ec70: 2074 656c 6c69 6e67 2068 6f77 2074 6865   telling how the
+0000ec80: 206f 7065 7261 7469 6f6e 2065 7865 6375   operation execu
+0000ec90: 7465 642e 0a0a 2020 2020 3a70 6172 616d  ted...    :param
+0000eca0: 2069 645f 6e6f 6465 3a20 5468 6520 6e6f   id_node: The no
+0000ecb0: 6465 2049 442e 0a0a 2020 2020 2222 220a  de ID...    """.
+0000ecc0: 0a20 2020 2023 2320 544f 444f 3a20 696d  .    ## TODO: im
+0000ecd0: 706c 656d 656e 7420 7468 6973 206f 7065  plement this ope
+0000ece0: 7261 7469 6f6e 2069 6e20 4150 4920 6261  ration in API ba
+0000ecf0: 636b 656e 640a 2020 2020 7261 6973 6520  ckend.    raise 
+0000ed00: 4e6f 7449 6d70 6c65 6d65 6e74 6564 4572  NotImplementedEr
+0000ed10: 726f 7228 290a 0a20 2020 2023 2066 696c  ror()..    # fil
+0000ed20: 655f 7061 7468 5f6b 6579 203d 2022 6669  e_path_key = "fi
+0000ed30: 6c65 5f70 6174 6822 0a20 2020 2023 2066  le_path".    # f
+0000ed40: 696c 655f 7369 7a65 5f6b 6579 203d 2022  ile_size_key = "
+0000ed50: 6669 6c65 5f73 697a 6522 0a20 2020 2023  file_size".    #
+0000ed60: 2073 7461 7475 735f 6b65 7920 3d20 2273   status_key = "s
+0000ed70: 7461 7475 7322 0a0a 2020 2020 2320 7265  tatus"..    # re
+0000ed80: 7375 6c74 203d 205f 6765 7428 6622 2f6e  sult = _get(f"/n
+0000ed90: 6f64 652f 7b69 645f 6e6f 6465 7d2f 6d65  ode/{id_node}/me
+0000eda0: 6d6f 7279 6475 6d70 2229 0a0a 2020 2020  morydump")..    
+0000edb0: 2320 6966 2028 0a20 2020 2023 2020 2020  # if (.    #    
+0000edc0: 2072 6573 756c 742e 7374 6174 7573 5f63   result.status_c
+0000edd0: 6f64 6520 213d 2032 3030 0a20 2020 2023  ode != 200.    #
+0000ede0: 2020 2020 206f 7220 7374 6174 7573 5f6b       or status_k
+0000edf0: 6579 206e 6f74 2069 6e20 7265 7375 6c74  ey not in result
+0000ee00: 2e6a 736f 6e28 290a 2020 2020 2320 2020  .json().    #   
+0000ee10: 2020 6f72 2072 6573 756c 742e 6a73 6f6e    or result.json
+0000ee20: 2829 5b73 7461 7475 735f 6b65 795d 2021  ()[status_key] !
+0000ee30: 3d20 2253 5441 5254 4544 220a 2020 2020  = "STARTED".    
+0000ee40: 2320 293a 0a20 2020 2023 2020 2020 205f  # ):.    #     _
+0000ee50: 6861 6e64 6c65 5f65 7272 6f72 2872 6573  handle_error(res
+0000ee60: 756c 742c 2022 4361 6e6e 6f74 2069 6e69  ult, "Cannot ini
+0000ee70: 7469 6174 6520 6e6f 6465 206d 656d 6f72  tiate node memor
+0000ee80: 7920 6475 6d70 2066 726f 6d20 636f 7265  y dump from core
+0000ee90: 2041 5049 2229 0a0a 2020 2020 2320 6c6f   API")..    # lo
+0000eea0: 6767 6572 2e69 6e66 6f28 225b 2b5d 2049  gger.info("[+] I
+0000eeb0: 6e69 7469 616c 697a 6564 206d 656d 6f72  nitialized memor
+0000eec0: 7920 6475 6d70 206f 6620 6e6f 6465 2027  y dump of node '
+0000eed0: 7b7d 272e 2e2e 222e 666f 726d 6174 2869  {}'...".format(i
+0000eee0: 645f 6e6f 6465 2929 0a0a 2020 2020 2320  d_node))..    # 
+0000eef0: 2320 5761 6974 2066 6f72 2074 6865 206f  # Wait for the o
+0000ef00: 7065 7261 7469 6f6e 2074 6f20 6265 2063  peration to be c
+0000ef10: 6f6d 706c 6574 6564 2069 6e20 6261 636b  ompleted in back
+0000ef20: 656e 640a 2020 2020 2320 2320 4e6f 7465  end.    # # Note
+0000ef30: 203a 206c 6f6f 7020 696e 7370 6972 6564   : loop inspired
+0000ef40: 2066 726f 6d20 5f73 696d 756c 6174 696f   from _simulatio
+0000ef50: 6e5f 6578 6563 7574 655f 6f70 6572 6174  n_execute_operat
+0000ef60: 696f 6e0a 2020 2020 2320 7768 696c 6520  ion.    # while 
+0000ef70: 5472 7565 3a0a 2020 2020 2320 2020 2020  True:.    #     
+0000ef80: 2320 536c 6565 7020 6265 666f 7265 206e  # Sleep before n
+0000ef90: 6578 7420 6974 6572 6174 696f 6e0a 2020  ext iteration.  
+0000efa0: 2020 2320 2020 2020 7469 6d65 2e73 6c65    #     time.sle
+0000efb0: 6570 2832 290a 0a20 2020 2023 2020 2020  ep(2)..    #    
+0000efc0: 2023 2046 6574 6368 2074 6865 2063 7572   # Fetch the cur
+0000efd0: 7265 6e74 2073 7461 7475 7320 6f66 2074  rent status of t
+0000efe0: 6865 206d 656d 6475 6d70 0a20 2020 2023  he memdump.    #
+0000eff0: 2020 2020 2072 6573 756c 7420 3d20 5f67       result = _g
+0000f000: 6574 2866 222f 6e6f 6465 2f7b 6964 5f6e  et(f"/node/{id_n
+0000f010: 6f64 657d 2f6d 656d 6f72 7964 756d 705f  ode}/memorydump_
+0000f020: 7374 6174 7573 2229 0a0a 2020 2020 2320  status")..    # 
+0000f030: 2020 2020 6966 2072 6573 756c 742e 7374      if result.st
+0000f040: 6174 7573 5f63 6f64 6520 213d 2032 3030  atus_code != 200
+0000f050: 3a0a 2020 2020 2320 2020 2020 2020 2020  :.    #         
+0000f060: 5f68 616e 646c 655f 6572 726f 7228 7265  _handle_error(re
+0000f070: 7375 6c74 2c20 2243 616e 6e6f 7420 6765  sult, "Cannot ge
+0000f080: 7420 7374 6174 7573 206f 6620 6e6f 6465  t status of node
+0000f090: 206d 656d 6f72 7920 6475 6d70 2066 726f   memory dump fro
+0000f0a0: 6d20 636f 7265 2041 5049 2229 0a0a 2020  m core API")..  
+0000f0b0: 2020 2320 2020 2020 7265 7375 6c74 5f6a    #     result_j
+0000f0c0: 736f 6e20 3d20 7265 7375 6c74 2e6a 736f  son = result.jso
+0000f0d0: 6e28 290a 2020 2020 2320 2020 2020 7072  n().    #     pr
+0000f0e0: 696e 7428 7265 7375 6c74 5f6a 736f 6e29  int(result_json)
+0000f0f0: 0a20 2020 2023 2020 2020 2069 6620 6e6f  .    #     if no
+0000f100: 7420 280a 2020 2020 2320 2020 2020 2020  t (.    #       
+0000f110: 2020 616c 6c28 6b20 696e 2072 6573 756c    all(k in resul
+0000f120: 745f 6a73 6f6e 2066 6f72 206b 2069 6e20  t_json for k in 
+0000f130: 2866 696c 655f 7061 7468 5f6b 6579 2c20  (file_path_key, 
+0000f140: 6669 6c65 5f73 697a 655f 6b65 792c 2073  file_size_key, s
+0000f150: 7461 7475 735f 6b65 7929 290a 2020 2020  tatus_key)).    
+0000f160: 2320 2020 2020 293a 0a20 2020 2023 2020  #     ):.    #  
+0000f170: 2020 2020 2020 2072 6169 7365 2045 7863         raise Exc
+0000f180: 6570 7469 6f6e 280a 2020 2020 2320 2020  eption(.    #   
+0000f190: 2020 2020 2020 2020 2020 6622 436f 6e74            f"Cont
+0000f1a0: 656e 7473 206f 6620 6d65 6d6f 7279 2064  ents of memory d
+0000f1b0: 756d 7020 7374 6174 7573 2075 7064 6174  ump status updat
+0000f1c0: 6520 6973 206e 6f74 2069 6e20 7468 6520  e is not in the 
+0000f1d0: 6578 7065 6374 6564 2066 6f72 6d61 7420  expected format 
+0000f1e0: 2861 7474 7269 6275 7465 7320 277b 6669  (attributes '{fi
+0000f1f0: 6c65 5f70 6174 685f 6b65 797d 272c 2027  le_path_key}', '
+0000f200: 7b66 696c 655f 7369 7a65 5f6b 6579 7d27  {file_size_key}'
+0000f210: 2061 6e64 2027 7b73 7461 7475 735f 6b65   and '{status_ke
+0000f220: 797d 2720 6578 7065 6374 6564 2922 0a20  y}' expected)". 
+0000f230: 2020 2023 2020 2020 2020 2020 2029 0a0a     #         )..
+0000f240: 2020 2020 2320 2020 2020 2320 4c6f 6720      #     # Log 
+0000f250: 696e 666f 206f 6e20 7072 6f67 7265 7373  info on progress
+0000f260: 696f 6e0a 2020 2020 2320 2020 2020 6966  ion.    #     if
+0000f270: 2072 6573 756c 745f 6a73 6f6e 5b73 7461   result_json[sta
+0000f280: 7475 735f 6b65 795d 203d 3d20 2253 5441  tus_key] == "STA
+0000f290: 5254 4544 223a 0a20 2020 2023 2020 2020  RTED":.    #    
+0000f2a0: 2020 2020 2070 6173 730a 2020 2020 2320       pass.    # 
+0000f2b0: 2020 2020 656c 6966 2072 6573 756c 745f      elif result_
+0000f2c0: 6a73 6f6e 5b73 7461 7475 735f 6b65 795d  json[status_key]
+0000f2d0: 203d 3d20 2250 524f 4752 4553 5322 3a0a   == "PROGRESS":.
+0000f2e0: 2020 2020 2320 2020 2020 2020 2020 6c6f      #         lo
+0000f2f0: 6767 6572 2e69 6e66 6f28 0a20 2020 2023  gger.info(.    #
+0000f300: 2020 2020 2020 2020 2020 2020 2022 2020               "  
+0000f310: 5b2b 5d20 4375 7272 656e 746c 7920 7065  [+] Currently pe
+0000f320: 7266 6f72 6d69 6e67 206d 656d 6f72 7920  rforming memory 
+0000f330: 6475 6d70 206f 6620 6e6f 6465 2027 7b7d  dump of node '{}
+0000f340: 2720 2863 7572 7265 6e74 2064 756d 7020  ' (current dump 
+0000f350: 6669 6c65 2073 697a 6520 6973 207b 7d29  file size is {})
+0000f360: 2e2e 2e22 2e66 6f72 6d61 7428 0a20 2020  ...".format(.   
+0000f370: 2023 2020 2020 2020 2020 2020 2020 2020   #              
+0000f380: 2020 2069 645f 6e6f 6465 2c20 6e61 7475     id_node, natu
+0000f390: 7261 6c73 697a 6528 7265 7375 6c74 5f6a  ralsize(result_j
+0000f3a0: 736f 6e5b 6669 6c65 5f73 697a 655f 6b65  son[file_size_ke
+0000f3b0: 795d 2c20 6269 6e61 7279 3d54 7275 6529  y], binary=True)
+0000f3c0: 0a20 2020 2023 2020 2020 2020 2020 2020  .    #          
+0000f3d0: 2020 2029 0a20 2020 2023 2020 2020 2020     ).    #      
+0000f3e0: 2020 2029 0a20 2020 2023 2020 2020 2065     ).    #     e
+0000f3f0: 6c69 6620 7265 7375 6c74 5f6a 736f 6e5b  lif result_json[
+0000f400: 7374 6174 7573 5f6b 6579 5d20 3d3d 2022  status_key] == "
+0000f410: 5355 4343 4553 5322 3a0a 2020 2020 2320  SUCCESS":.    # 
+0000f420: 2020 2020 2020 2020 6272 6561 6b0a 2020          break.  
+0000f430: 2020 2320 2020 2020 656c 7365 3a0a 2020    #     else:.  
+0000f440: 2020 2320 2020 2020 2020 2020 7261 6973    #         rais
+0000f450: 6520 4578 6365 7074 696f 6e28 0a20 2020  e Exception(.   
+0000f460: 2023 2020 2020 2020 2020 2020 2020 2022   #             "
+0000f470: 4572 726f 7220 6475 7269 6e67 206d 656d  Error during mem
+0000f480: 6f72 7920 6475 6d70 206f 6620 6e6f 6465  ory dump of node
+0000f490: 207b 7d20 6f70 6572 6174 696f 6e3a 2027   {} operation: '
+0000f4a0: 7b7d 2722 2e66 6f72 6d61 7428 0a20 2020  {}'".format(.   
+0000f4b0: 2023 2020 2020 2020 2020 2020 2020 2020   #              
+0000f4c0: 2020 2069 645f 6e6f 6465 2c20 7265 7375     id_node, resu
+0000f4d0: 6c74 5f6a 736f 6e5b 7374 6174 7573 5f6b  lt_json[status_k
+0000f4e0: 6579 5d0a 2020 2020 2320 2020 2020 2020  ey].    #       
+0000f4f0: 2020 2020 2020 290a 2020 2020 2320 2020        ).    #   
+0000f500: 2020 2020 2020 290a 0a20 2020 2023 206c        )..    # l
+0000f510: 6f67 6765 722e 696e 666f 280a 2020 2020  ogger.info(.    
+0000f520: 2320 2020 2020 225b 2b5d 204e 6f64 6520  #     "[+] Node 
+0000f530: 6d65 6d6f 7279 2064 756d 7020 2872 6177  memory dump (raw
+0000f540: 2064 756d 7020 7769 7468 206c 6962 7669   dump with libvi
+0000f550: 7274 2920 6f62 7461 696e 6564 2c20 616e  rt) obtained, an
+0000f560: 6420 706c 6163 6564 2069 6e20 6669 6c65  d placed in file
+0000f570: 207b 7d20 287b 7d29 206f 6e20 7468 6520   {} ({}) on the 
+0000f580: 7365 7276 6572 2e22 2e66 6f72 6d61 7428  server.".format(
+0000f590: 0a20 2020 2023 2020 2020 2020 2020 2072  .    #         r
+0000f5a0: 6573 756c 745f 6a73 6f6e 5b66 696c 655f  esult_json[file_
+0000f5b0: 7061 7468 5f6b 6579 5d2c 0a20 2020 2023  path_key],.    #
+0000f5c0: 2020 2020 2020 2020 206e 6174 7572 616c           natural
+0000f5d0: 7369 7a65 2872 6573 756c 745f 6a73 6f6e  size(result_json
+0000f5e0: 5b66 696c 655f 7369 7a65 5f6b 6579 5d2c  [file_size_key],
+0000f5f0: 2062 696e 6172 793d 5472 7565 292c 0a20   binary=True),. 
+0000f600: 2020 2023 2020 2020 2029 0a20 2020 2023     #     ).    #
+0000f610: 2029 0a0a 2020 2020 2320 7265 7475 726e   )..    # return
+0000f620: 2072 6573 756c 745f 6a73 6f6e 5b66 696c   result_json[fil
+0000f630: 655f 7061 7468 5f6b 6579 5d2c 2072 6573  e_path_key], res
+0000f640: 756c 745f 6a73 6f6e 5b66 696c 655f 7369  ult_json[file_si
+0000f650: 7a65 5f6b 6579 5d0a 0a0a 6465 6620 6665  ze_key]...def fe
+0000f660: 7463 685f 6e6f 6465 5f6e 6574 776f 726b  tch_node_network
+0000f670: 5f69 6e74 6572 6661 6365 7328 6964 5f6e  _interfaces(id_n
+0000f680: 6f64 653a 2069 6e74 2920 2d3e 2041 6e79  ode: int) -> Any
+0000f690: 3a0a 2020 2020 2222 2252 6574 7572 6e20  :.    """Return 
+0000f6a0: 6e65 7477 6f72 6b20 696e 7465 7266 6163  network interfac
+0000f6b0: 6573 206c 6973 7420 6769 7665 6e20 6120  es list given a 
+0000f6c0: 6e6f 6465 2049 442e 0a0a 2020 2020 3a72  node ID...    :r
+0000f6d0: 6574 7572 6e3a 2054 6865 206c 6973 7420  eturn: The list 
+0000f6e0: 6f66 206e 6574 776f 726b 2069 6e74 6572  of network inter
+0000f6f0: 6661 6365 732e 0a0a 2020 2020 3a70 6172  faces...    :par
+0000f700: 616d 2069 645f 6e6f 6465 3a20 5468 6520  am id_node: The 
+0000f710: 6e6f 6465 2049 442e 0a0a 2020 2020 2222  node ID...    ""
+0000f720: 220a 2020 2020 7265 7375 6c74 203d 205f  ".    result = _
+0000f730: 6765 7428 6622 2f6e 6f64 652f 7b69 645f  get(f"/node/{id_
+0000f740: 6e6f 6465 7d2f 6e65 7477 6f72 6b5f 696e  node}/network_in
+0000f750: 7465 7266 6163 6522 290a 0a20 2020 2069  terface")..    i
+0000f760: 6620 7265 7375 6c74 2e73 7461 7475 735f  f result.status_
+0000f770: 636f 6465 2021 3d20 3230 303a 0a20 2020  code != 200:.   
+0000f780: 2020 2020 205f 6861 6e64 6c65 5f65 7272       _handle_err
+0000f790: 6f72 2872 6573 756c 742c 2022 4361 6e6e  or(result, "Cann
+0000f7a0: 6f74 2072 6574 7269 6576 6520 6e6f 6465  ot retrieve node
+0000f7b0: 206e 6574 776f 726b 2069 6e74 6572 6661   network interfa
+0000f7c0: 6365 7322 290a 0a20 2020 2072 6574 7572  ces")..    retur
+0000f7d0: 6e20 7265 7375 6c74 2e6a 736f 6e28 290a  n result.json().
+0000f7e0: 0a0a 6465 6620 6665 7463 685f 7369 6d75  ..def fetch_simu
+0000f7f0: 6c61 7469 6f6e 5f6e 6574 776f 726b 5f69  lation_network_i
+0000f800: 6e74 6572 6661 6365 7328 6964 5f73 696d  nterfaces(id_sim
+0000f810: 756c 6174 696f 6e3a 2069 6e74 2920 2d3e  ulation: int) ->
+0000f820: 2041 6e79 3a0a 2020 2020 2222 2252 6574   Any:.    """Ret
+0000f830: 7572 6e20 6e65 7477 6f72 6b20 696e 7465  urn network inte
+0000f840: 7266 6163 6573 206c 6973 7420 6769 7665  rfaces list give
+0000f850: 6e20 6120 7369 6d75 6c61 7469 6f6e 2049  n a simulation I
+0000f860: 442e 0a0a 2020 2020 3a72 6574 7572 6e3a  D...    :return:
+0000f870: 2054 6865 206c 6973 7420 6f66 206e 6574   The list of net
+0000f880: 776f 726b 2069 6e74 6572 6661 6365 732e  work interfaces.
+0000f890: 0a0a 2020 2020 3a70 6172 616d 2069 645f  ..    :param id_
+0000f8a0: 7369 6d75 6c61 7469 6f6e 3a20 5468 6520  simulation: The 
+0000f8b0: 7369 6d75 6c61 7469 6f6e 2049 442e 0a0a  simulation ID...
+0000f8c0: 2020 2020 2222 220a 2020 2020 7265 7375      """.    resu
+0000f8d0: 6c74 203d 205f 6765 7428 6622 2f73 696d  lt = _get(f"/sim
+0000f8e0: 756c 6174 696f 6e2f 7b69 645f 7369 6d75  ulation/{id_simu
+0000f8f0: 6c61 7469 6f6e 7d2f 6e65 7477 6f72 6b5f  lation}/network_
+0000f900: 696e 7465 7266 6163 6522 290a 0a20 2020  interface")..   
+0000f910: 2069 6620 7265 7375 6c74 2e73 7461 7475   if result.statu
+0000f920: 735f 636f 6465 2021 3d20 3230 303a 0a20  s_code != 200:. 
+0000f930: 2020 2020 2020 205f 6861 6e64 6c65 5f65         _handle_e
+0000f940: 7272 6f72 2872 6573 756c 742c 2022 4361  rror(result, "Ca
+0000f950: 6e6e 6f74 2072 6574 7269 6576 6520 7369  nnot retrieve si
+0000f960: 6d75 6c61 7469 6f6e 206e 6574 776f 726b  mulation network
+0000f970: 2069 6e74 6572 6661 6365 7322 290a 0a20   interfaces").. 
+0000f980: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+0000f990: 2e6a 736f 6e28 290a 0a0a 6465 6620 6665  .json()...def fe
+0000f9a0: 7463 685f 6e65 7477 6f72 6b5f 696e 7465  tch_network_inte
+0000f9b0: 7266 6163 655f 6279 5f6d 6163 2869 645f  rface_by_mac(id_
+0000f9c0: 7369 6d75 6c61 7469 6f6e 3a20 696e 742c  simulation: int,
+0000f9d0: 206d 6163 5f61 6464 7265 7373 3a20 7374   mac_address: st
+0000f9e0: 7229 202d 3e20 416e 793a 0a20 2020 2022  r) -> Any:.    "
+0000f9f0: 2222 5265 7475 726e 206e 6574 776f 726b  ""Return network
+0000fa00: 2069 6e74 6572 6661 6365 206c 6973 7420   interface list 
+0000fa10: 6769 7665 6e20 6120 6d61 6320 6164 6472  given a mac addr
+0000fa20: 6573 732e 0a0a 2020 2020 3a72 6574 7572  ess...    :retur
+0000fa30: 6e3a 2054 6865 206e 6574 776f 726b 2069  n: The network i
+0000fa40: 6e74 6572 6661 6365 2e0a 0a20 2020 203a  nterface...    :
+0000fa50: 7061 7261 6d20 6964 5f73 696d 756c 6174  param id_simulat
+0000fa60: 696f 6e3a 2054 6865 2073 696d 756c 6174  ion: The simulat
+0000fa70: 696f 6e20 4944 2e0a 2020 2020 3a70 6172  ion ID..    :par
+0000fa80: 616d 206d 6163 5f61 6464 7265 7373 3a20  am mac_address: 
+0000fa90: 5468 6520 6d61 635f 6164 6472 6573 7320  The mac_address 
+0000faa0: 746f 206c 6f6f 6b20 666f 722e 0a0a 2020  to look for...  
+0000fab0: 2020 2222 220a 2020 2020 2320 4665 7463    """.    # Fetc
+0000fac0: 6820 6e6f 6465 206e 6574 776f 726b 2069  h node network i
+0000fad0: 6e74 6572 6661 6365 730a 2020 2020 7265  nterfaces.    re
+0000fae0: 7375 6c74 203d 205f 6765 7428 6622 2f73  sult = _get(f"/s
+0000faf0: 696d 756c 6174 696f 6e2f 7b69 645f 7369  imulation/{id_si
+0000fb00: 6d75 6c61 7469 6f6e 7d2f 6e65 7477 6f72  mulation}/networ
+0000fb10: 6b5f 696e 7465 7266 6163 6522 290a 0a20  k_interface").. 
+0000fb20: 2020 2069 6620 7265 7375 6c74 2e73 7461     if result.sta
+0000fb30: 7475 735f 636f 6465 2021 3d20 3230 303a  tus_code != 200:
+0000fb40: 0a20 2020 2020 2020 205f 6861 6e64 6c65  .        _handle
+0000fb50: 5f65 7272 6f72 2872 6573 756c 742c 2022  _error(result, "
+0000fb60: 4361 6e6e 6f74 2072 6574 7269 6576 6520  Cannot retrieve 
+0000fb70: 6e65 7477 6f72 6b20 696e 7465 7266 6163  network interfac
+0000fb80: 6573 2229 0a0a 2020 2020 6e65 7477 6f72  es")..    networ
+0000fb90: 6b5f 696e 7465 7266 6163 6573 203d 2072  k_interfaces = r
+0000fba0: 6573 756c 742e 6a73 6f6e 2829 0a0a 2020  esult.json()..  
+0000fbb0: 2020 666f 7220 6e65 7477 6f72 6b5f 696e    for network_in
+0000fbc0: 7465 7266 6163 6520 696e 206e 6574 776f  terface in netwo
+0000fbd0: 726b 5f69 6e74 6572 6661 6365 733a 0a20  rk_interfaces:. 
+0000fbe0: 2020 2020 2020 2069 6620 6e65 7477 6f72         if networ
+0000fbf0: 6b5f 696e 7465 7266 6163 655b 226d 6163  k_interface["mac
+0000fc00: 5f61 6464 7265 7373 225d 203d 3d20 6d61  _address"] == ma
+0000fc10: 635f 6164 6472 6573 733a 0a20 2020 2020  c_address:.     
+0000fc20: 2020 2020 2020 2072 6574 7572 6e20 6e65         return ne
+0000fc30: 7477 6f72 6b5f 696e 7465 7266 6163 650a  twork_interface.
+0000fc40: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000fc50: 2020 7265 7475 726e 204e 6f6e 650a 0a0a    return None...
+0000fc60: 6465 6620 6465 6c65 7465 5f6e 6574 776f  def delete_netwo
+0000fc70: 726b 5f69 6e74 6572 6661 6365 2869 645f  rk_interface(id_
+0000fc80: 6e65 7477 6f72 6b5f 696e 7465 7266 6163  network_interfac
+0000fc90: 653a 2069 6e74 2920 2d3e 2041 6e79 3a0a  e: int) -> Any:.
+0000fca0: 2020 2020 2222 2244 656c 6574 6520 6e65      """Delete ne
+0000fcb0: 7477 6f72 6b20 696e 7465 7266 6163 6520  twork interface 
+0000fcc0: 6769 7665 6e20 616e 2069 642e 0a0a 2020  given an id...  
+0000fcd0: 2020 3a72 6574 7572 6e3a 2041 206d 6573    :return: A mes
+0000fce0: 7361 6765 2074 656c 6c69 6e67 2068 6f77  sage telling how
+0000fcf0: 2074 6865 206f 7065 7261 7469 6f6e 2065   the operation e
+0000fd00: 7865 6375 7465 642e 0a0a 2020 2020 3a70  xecuted...    :p
+0000fd10: 6172 616d 2069 645f 6e65 7477 6f72 6b5f  aram id_network_
+0000fd20: 696e 7465 7266 6163 653a 2054 6865 206e  interface: The n
+0000fd30: 6574 776f 726b 2069 6e74 6572 6661 6365  etwork interface
+0000fd40: 2049 442e 0a0a 2020 2020 2222 220a 2020   ID...    """.  
+0000fd50: 2020 7265 7375 6c74 203d 205f 6465 6c65    result = _dele
+0000fd60: 7465 2866 222f 6e65 7477 6f72 6b5f 696e  te(f"/network_in
+0000fd70: 7465 7266 6163 652f 7b69 645f 6e65 7477  terface/{id_netw
+0000fd80: 6f72 6b5f 696e 7465 7266 6163 657d 2229  ork_interface}")
+0000fd90: 0a0a 2020 2020 6966 2072 6573 756c 742e  ..    if result.
+0000fda0: 7374 6174 7573 5f63 6f64 6520 213d 2032  status_code != 2
+0000fdb0: 3030 3a0a 2020 2020 2020 2020 5f68 616e  00:.        _han
+0000fdc0: 646c 655f 6572 726f 7228 0a20 2020 2020  dle_error(.     
+0000fdd0: 2020 2020 2020 2072 6573 756c 742c 2022         result, "
+0000fde0: 4361 6e6e 6f74 2072 6574 7269 6576 6520  Cannot retrieve 
+0000fdf0: 6e6f 6465 206e 6574 776f 726b 2069 6e74  node network int
+0000fe00: 6572 6661 6365 7320 6672 6f6d 2049 5420  erfaces from IT 
+0000fe10: 5369 6d75 6c61 7469 6f6e 2041 5049 220a  Simulation API".
+0000fe20: 2020 2020 2020 2020 290a 0a20 2020 2072          )..    r
+0000fe30: 6574 7572 6e20 7265 7375 6c74 2e6a 736f  eturn result.jso
+0000fe40: 6e28 290a 0a0a 6465 6620 7570 6461 7465  n()...def update
+0000fe50: 5f6e 6574 776f 726b 5f69 6e74 6572 6661  _network_interfa
+0000fe60: 6365 280a 2020 2020 6964 5f6e 6574 776f  ce(.    id_netwo
+0000fe70: 726b 5f69 6e74 6572 6661 6365 3a20 696e  rk_interface: in
+0000fe80: 742c 206e 6574 776f 726b 5f69 6e74 6572  t, network_inter
+0000fe90: 6661 6365 5f64 6963 743a 2064 6963 740a  face_dict: dict.
+0000fea0: 2920 2d3e 2041 6e79 3a0a 2020 2020 2222  ) -> Any:.    ""
+0000feb0: 2255 7064 6174 6520 6e65 7477 6f72 6b20  "Update network 
+0000fec0: 696e 7465 7266 6163 6520 696e 666f 726d  interface inform
+0000fed0: 6174 696f 6e20 696e 666f 726d 6174 696f  ation informatio
+0000fee0: 6e20 6769 7665 6e20 6120 6e65 7477 6f72  n given a networ
+0000fef0: 6b20 696e 7465 7266 6163 6520 6964 2061  k interface id a
+0000ff00: 6e64 2061 0a20 2020 2064 6963 7420 636f  nd a.    dict co
+0000ff10: 6e74 6169 6e69 6e67 206e 6574 776f 726b  ntaining network
+0000ff20: 2069 6e66 6f2e 0a0a 2020 2020 3a72 6574   info...    :ret
+0000ff30: 7572 6e3a 2041 206d 6573 7361 6765 2074  urn: A message t
+0000ff40: 656c 6c69 6e67 2068 6f77 2074 6865 206f  elling how the o
+0000ff50: 7065 7261 7469 6f6e 2065 7865 6375 7465  peration execute
+0000ff60: 642e 0a0a 2020 2020 3a70 6172 616d 2069  d...    :param i
+0000ff70: 645f 6e65 7477 6f72 6b5f 696e 7465 7266  d_network_interf
+0000ff80: 6163 653a 2054 6865 206e 6574 776f 726b  ace: The network
+0000ff90: 2069 6e74 6572 6661 6365 2049 442e 0a20   interface ID.. 
+0000ffa0: 2020 203a 7061 7261 6d20 6e65 7477 6f72     :param networ
+0000ffb0: 6b5f 696e 7465 7266 6163 655f 6469 6374  k_interface_dict
+0000ffc0: 3a20 5468 6520 6469 6374 2063 6f6e 7461  : The dict conta
+0000ffd0: 696e 696e 6720 7468 6520 656e 7472 6965  ining the entrie
+0000ffe0: 7320 746f 2075 7064 6174 652e 0a0a 2020  s to update...  
+0000fff0: 2020 2222 220a 2020 2020 6461 7461 203d    """.    data =
+00010000: 206a 736f 6e2e 6475 6d70 7328 6e65 7477   json.dumps(netw
+00010010: 6f72 6b5f 696e 7465 7266 6163 655f 6469  ork_interface_di
+00010020: 6374 290a 2020 2020 7265 7375 6c74 203d  ct).    result =
+00010030: 205f 7075 7428 0a20 2020 2020 2020 2066   _put(.        f
+00010040: 222f 6e65 7477 6f72 6b5f 696e 7465 7266  "/network_interf
+00010050: 6163 652f 7b69 645f 6e65 7477 6f72 6b5f  ace/{id_network_
+00010060: 696e 7465 7266 6163 657d 222c 0a20 2020  interface}",.   
+00010070: 2020 2020 2064 6174 613d 6461 7461 2c0a       data=data,.
+00010080: 2020 2020 2020 2020 6865 6164 6572 733d          headers=
+00010090: 7b22 436f 6e74 656e 742d 5479 7065 223a  {"Content-Type":
+000100a0: 2022 6170 706c 6963 6174 696f 6e2f 6a73   "application/js
+000100b0: 6f6e 227d 2c0a 2020 2020 290a 0a20 2020  on"},.    )..   
+000100c0: 2069 6620 7265 7375 6c74 2e73 7461 7475   if result.statu
+000100d0: 735f 636f 6465 2021 3d20 3230 303a 0a20  s_code != 200:. 
+000100e0: 2020 2020 2020 205f 6861 6e64 6c65 5f65         _handle_e
+000100f0: 7272 6f72 2872 6573 756c 742c 2022 4361  rror(result, "Ca
+00010100: 6e6e 6f74 2075 7064 6174 6520 6e65 7477  nnot update netw
+00010110: 6f72 6b20 696e 7465 7266 6163 6520 696e  ork interface in
+00010120: 666f 726d 6174 696f 6e22 290a 0a20 2020  formation")..   
+00010130: 2072 6574 7572 6e20 7265 7375 6c74 2e6a   return result.j
+00010140: 736f 6e28 290a 0a0a 6465 6620 6665 7463  son()...def fetc
+00010150: 685f 7072 6f62 6528 7072 6f62 655f 6964  h_probe(probe_id
+00010160: 3a20 696e 7429 202d 3e20 416e 793a 0a20  : int) -> Any:. 
+00010170: 2020 2022 2222 5265 7475 726e 2061 2070     """Return a p
+00010180: 726f 6265 2067 6976 656e 2069 7473 2049  robe given its I
+00010190: 442e 0a0a 2020 2020 3a72 6574 7572 6e3a  D...    :return:
+000101a0: 2054 6865 2070 726f 6265 2064 6963 742e   The probe dict.
+000101b0: 0a0a 2020 2020 3a70 6172 616d 2070 726f  ..    :param pro
+000101c0: 6265 5f69 643a 2054 6865 2070 726f 6265  be_id: The probe
+000101d0: 2049 442e 0a0a 2020 2020 2222 220a 2020   ID...    """.  
+000101e0: 2020 7265 7375 6c74 203d 205f 6765 7428    result = _get(
+000101f0: 6622 2f70 726f 6265 2f7b 7072 6f62 655f  f"/probe/{probe_
+00010200: 6964 7d22 290a 0a20 2020 2069 6620 7265  id}")..    if re
+00010210: 7375 6c74 2e73 7461 7475 735f 636f 6465  sult.status_code
+00010220: 2021 3d20 3230 303a 0a20 2020 2020 2020   != 200:.       
+00010230: 205f 6861 6e64 6c65 5f65 7272 6f72 2872   _handle_error(r
+00010240: 6573 756c 742c 2022 4361 6e6e 6f74 2072  esult, "Cannot r
+00010250: 6574 7269 6576 6520 7072 6f62 6520 6672  etrieve probe fr
+00010260: 6f6d 2063 6f72 6520 4150 4922 290a 0a20  om core API").. 
+00010270: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+00010280: 2e6a 736f 6e28 290a 0a0a 6465 6620 6665  .json()...def fe
+00010290: 7463 685f 7072 6f62 6573 2869 645f 7369  tch_probes(id_si
+000102a0: 6d75 6c61 7469 6f6e 3a20 696e 7429 202d  mulation: int) -
+000102b0: 3e20 416e 793a 0a20 2020 2022 2222 5265  > Any:.    """Re
+000102c0: 7475 726e 2073 696d 756c 6174 696f 6e20  turn simulation 
+000102d0: 7072 6f62 6573 2064 6963 7420 6769 7665  probes dict give
+000102e0: 6e0a 2020 2020 6120 7369 6d75 6c61 7469  n.    a simulati
+000102f0: 6f6e 2049 442c 2077 6865 7265 206b 6579  on ID, where key
+00010300: 7320 6172 6520 7072 6f62 6573 2069 6473  s are probes ids
+00010310: 2e0a 0a20 2020 203a 7265 7475 726e 3a20  ...    :return: 
+00010320: 5468 6520 6c69 7374 206f 6620 7072 6f62  The list of prob
+00010330: 6520 6469 6374 732e 0a0a 2020 2020 3a70  e dicts...    :p
+00010340: 6172 616d 2069 645f 7369 6d75 6c61 7469  aram id_simulati
+00010350: 6f6e 3a20 5468 6520 7369 6d75 6c61 7469  on: The simulati
+00010360: 6f6e 2049 442e 0a0a 2020 2020 2222 220a  on ID...    """.
+00010370: 0a20 2020 2072 6573 756c 7420 3d20 5f67  .    result = _g
+00010380: 6574 2866 222f 7369 6d75 6c61 7469 6f6e  et(f"/simulation
+00010390: 2f7b 6964 5f73 696d 756c 6174 696f 6e7d  /{id_simulation}
+000103a0: 2f70 726f 6265 2229 0a0a 2020 2020 6966  /probe")..    if
+000103b0: 2072 6573 756c 742e 7374 6174 7573 5f63   result.status_c
+000103c0: 6f64 6520 213d 2032 3030 3a0a 2020 2020  ode != 200:.    
+000103d0: 2020 2020 5f68 616e 646c 655f 6572 726f      _handle_erro
+000103e0: 7228 7265 7375 6c74 2c20 2243 616e 6e6f  r(result, "Canno
+000103f0: 7420 7265 7472 6965 7665 2073 696d 756c  t retrieve simul
+00010400: 6174 696f 6e20 7072 6f62 6573 2066 726f  ation probes fro
+00010410: 6d20 636f 7265 2041 5049 2229 0a0a 2020  m core API")..  
+00010420: 2020 7265 7475 726e 2072 6573 756c 742e    return result.
+00010430: 6a73 6f6e 2829 0a0a 0a64 6566 2063 7265  json()...def cre
+00010440: 6174 655f 7072 6f62 6528 0a20 2020 2069  ate_probe(.    i
+00010450: 645f 7369 6d75 6c61 7469 6f6e 3a20 696e  d_simulation: in
+00010460: 742c 0a20 2020 206e 6574 776f 726b 5f69  t,.    network_i
+00010470: 6e74 6572 6661 6365 733a 204c 6973 745b  nterfaces: List[
+00010480: 696e 745d 2c0a 2020 2020 6966 6163 653a  int],.    iface:
+00010490: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+000104a0: 204e 6f6e 652c 0a20 2020 2070 6361 703a   None,.    pcap:
+000104b0: 204f 7074 696f 6e61 6c5b 626f 6f6c 5d20   Optional[bool] 
+000104c0: 3d20 4661 6c73 652c 0a20 2020 2066 696c  = False,.    fil
+000104d0: 7465 723a 204f 7074 696f 6e61 6c5b 7374  ter: Optional[st
+000104e0: 725d 203d 2022 222c 0a20 2020 2064 6972  r] = "",.    dir
+000104f0: 6563 7469 6f6e 3a20 4f70 7469 6f6e 616c  ection: Optional
+00010500: 5b73 7472 5d20 3d20 2262 6f74 6822 2c0a  [str] = "both",.
+00010510: 2920 2d3e 2069 6e74 3a0a 2020 2020 2222  ) -> int:.    ""
+00010520: 2243 7265 6174 6520 6120 6e65 7720 7072  "Create a new pr
+00010530: 6f62 6520 666f 7220 7468 6520 7369 6d75  obe for the simu
+00010540: 6c61 7469 6f6e 2067 6976 656e 2061 2064  lation given a d
+00010550: 6963 7420 636f 6e74 6169 6e69 6e67 2070  ict containing p
+00010560: 726f 6265 2064 6174 612e 0a0a 2020 2020  robe data...    
+00010570: 3a72 6574 7572 6e3a 2054 6865 206e 6577  :return: The new
+00010580: 2070 726f 6265 2049 442e 0a0a 2020 2020   probe ID...    
+00010590: 3a70 6172 616d 2069 645f 7369 6d75 6c61  :param id_simula
+000105a0: 7469 6f6e 3a20 5468 6520 7369 6d75 6c61  tion: The simula
+000105b0: 7469 6f6e 2049 442e 0a20 2020 203a 7061  tion ID..    :pa
+000105c0: 7261 6d20 6e65 7477 6f72 6b5f 696e 7465  ram network_inte
+000105d0: 7266 6163 6573 3a20 5468 6520 6c69 7374  rfaces: The list
+000105e0: 206f 6620 6e65 7477 6f72 6b20 696e 7465   of network inte
+000105f0: 7266 6163 6573 2074 6f20 6361 7074 7572  rfaces to captur
+00010600: 6520 7472 6166 6669 6320 6672 6f6d 2e0a  e traffic from..
+00010610: 2020 2020 3a70 6172 616d 2069 6661 6365      :param iface
+00010620: 3a20 496e 7465 7266 6163 6520 7768 6572  : Interface wher
+00010630: 6520 7468 6520 7472 6166 6669 6320 6973  e the traffic is
+00010640: 206d 6972 726f 7265 6420 746f 2e20 4578   mirrored to. Ex
+00010650: 3a20 2764 756d 6d79 3027 2e0a 2020 2020  : 'dummy0'..    
+00010660: 3a70 6172 616d 2070 6361 703a 2041 2062  :param pcap: A b
+00010670: 6f6f 6c65 616e 2069 6e64 6963 6174 696e  oolean indicatin
+00010680: 6720 6966 2074 6865 2063 6170 7475 7265  g if the capture
+00010690: 2073 686f 756c 6420 6265 2073 6176 6564   should be saved
+000106a0: 206f 6e20 6469 736b 2069 6e20 6120 7063   on disk in a pc
+000106b0: 6170 2066 696c 6520 2874 6f20 6265 2069  ap file (to be i
+000106c0: 6e63 6c75 6465 6420 696e 2064 6174 6173  ncluded in datas
+000106d0: 6574 290a 2020 2020 3a70 6172 616d 2066  et).    :param f
+000106e0: 696c 7465 723a 2053 7472 696e 6720 6669  ilter: String fi
+000106f0: 6c74 6572 696e 6720 7463 7064 756d 7020  ltering tcpdump 
+00010700: 6361 7074 7572 652e 2045 783a 2027 7463  capture. Ex: 'tc
+00010710: 7020 706f 7274 2038 3027 2e0a 2020 2020  p port 80'..    
+00010720: 3a70 6172 616d 2064 6972 6563 7469 6f6e  :param direction
+00010730: 3a20 5365 6c65 6374 2077 6869 6368 2074  : Select which t
+00010740: 7261 6666 6963 2074 6f20 6d6f 6e69 746f  raffic to monito
+00010750: 7220 6f6e 2074 6865 206d 6972 726f 7265  r on the mirrore
+00010760: 6420 696e 7465 7266 6163 6528 7329 3a20  d interface(s): 
+00010770: 6569 7468 6572 2027 696e 6772 6573 7327  either 'ingress'
+00010780: 2c20 2765 6772 6573 7327 206f 7220 2762  , 'egress' or 'b
+00010790: 6f74 6827 2e0a 0a20 2020 2022 2222 0a0a  oth'...    """..
+000107a0: 2020 2020 6461 7461 5f64 6963 7420 3d20      data_dict = 
+000107b0: 7b0a 2020 2020 2020 2020 2269 6661 6365  {.        "iface
+000107c0: 223a 2069 6661 6365 2c0a 2020 2020 2020  ": iface,.      
+000107d0: 2020 2270 6361 7022 3a20 7063 6170 2c0a    "pcap": pcap,.
+000107e0: 2020 2020 2020 2020 2266 696c 7465 7222          "filter"
+000107f0: 3a20 6669 6c74 6572 2c0a 2020 2020 2020  : filter,.      
+00010800: 2020 226e 6574 776f 726b 5f69 6e74 6572    "network_inter
+00010810: 6661 6365 7322 3a20 6e65 7477 6f72 6b5f  faces": network_
+00010820: 696e 7465 7266 6163 6573 2c0a 2020 2020  interfaces,.    
+00010830: 2020 2020 2264 6972 6563 7469 6f6e 223a      "direction":
+00010840: 2064 6972 6563 7469 6f6e 2c0a 2020 2020   direction,.    
+00010850: 7d0a 0a20 2020 2064 6174 6120 3d20 6a73  }..    data = js
+00010860: 6f6e 2e64 756d 7073 2864 6174 615f 6469  on.dumps(data_di
+00010870: 6374 290a 2020 2020 7265 7375 6c74 203d  ct).    result =
+00010880: 205f 706f 7374 280a 2020 2020 2020 2020   _post(.        
+00010890: 6622 2f73 696d 756c 6174 696f 6e2f 7b69  f"/simulation/{i
+000108a0: 645f 7369 6d75 6c61 7469 6f6e 7d2f 7072  d_simulation}/pr
+000108b0: 6f62 6522 2c0a 2020 2020 2020 2020 6461  obe",.        da
+000108c0: 7461 3d64 6174 612c 0a20 2020 2020 2020  ta=data,.       
+000108d0: 2068 6561 6465 7273 3d7b 2243 6f6e 7465   headers={"Conte
+000108e0: 6e74 2d54 7970 6522 3a20 2261 7070 6c69  nt-Type": "appli
+000108f0: 6361 7469 6f6e 2f6a 736f 6e22 7d2c 0a20  cation/json"},. 
+00010900: 2020 2029 0a0a 2020 2020 6966 2072 6573     )..    if res
+00010910: 756c 742e 7374 6174 7573 5f63 6f64 6520  ult.status_code 
+00010920: 213d 2032 3030 3a0a 2020 2020 2020 2020  != 200:.        
+00010930: 5f68 616e 646c 655f 6572 726f 7228 7265  _handle_error(re
+00010940: 7375 6c74 2c20 2243 616e 6e6f 7420 6372  sult, "Cannot cr
+00010950: 6561 7465 2070 726f 6265 2077 6974 6820  eate probe with 
+00010960: 636f 7265 2041 5049 2229 0a0a 2020 2020  core API")..    
+00010970: 7072 6f62 655f 6964 203d 2072 6573 756c  probe_id = resul
+00010980: 742e 6a73 6f6e 2829 5b22 6964 225d 0a0a  t.json()["id"]..
+00010990: 2020 2020 7265 7475 726e 2070 726f 6265      return probe
+000109a0: 5f69 640a 0a0a 6465 6620 7570 6461 7465  _id...def update
+000109b0: 5f70 726f 6265 2870 726f 6265 5f69 643a  _probe(probe_id:
+000109c0: 2069 6e74 2c20 7072 6f62 655f 6469 6374   int, probe_dict
+000109d0: 3a20 6469 6374 2920 2d3e 2041 6e79 3a0a  : dict) -> Any:.
+000109e0: 2020 2020 2222 2255 7064 6174 6520 7072      """Update pr
+000109f0: 6f62 6520 696e 666f 726d 6174 696f 6e20  obe information 
+00010a00: 6769 7665 6e20 6120 7072 6f62 6520 6964  given a probe id
+00010a10: 2061 6e64 2061 2064 6963 7420 636f 6e74   and a dict cont
+00010a20: 6169 6e69 6e67 0a20 2020 2070 726f 6265  aining.    probe
+00010a30: 2064 6174 612e 0a0a 2020 2020 3a72 6574   data...    :ret
+00010a40: 7572 6e3a 2041 206d 6573 7361 6765 2074  urn: A message t
+00010a50: 656c 6c69 6e67 2068 6f77 2074 6865 206f  elling how the o
+00010a60: 7065 7261 7469 6f6e 2065 7865 6375 7465  peration execute
+00010a70: 642e 0a0a 2020 2020 3a70 6172 616d 2070  d...    :param p
+00010a80: 726f 6265 5f69 643a 2054 6865 2070 726f  robe_id: The pro
+00010a90: 6265 2049 442e 0a20 2020 203a 7061 7261  be ID..    :para
+00010aa0: 6d20 7072 6f62 655f 6469 6374 3a20 5468  m probe_dict: Th
+00010ab0: 6520 6469 6374 2063 6f6e 7461 696e 696e  e dict containin
+00010ac0: 6720 7468 6520 656e 7472 6965 7320 746f  g the entries to
+00010ad0: 2075 7064 6174 652e 0a0a 2020 2020 2222   update...    ""
+00010ae0: 220a 0a20 2020 2064 6174 6120 3d20 6a73  "..    data = js
+00010af0: 6f6e 2e64 756d 7073 2870 726f 6265 5f64  on.dumps(probe_d
+00010b00: 6963 7429 0a20 2020 2072 6573 756c 7420  ict).    result 
+00010b10: 3d20 5f70 7574 280a 2020 2020 2020 2020  = _put(.        
+00010b20: 6622 2f70 726f 6265 2f7b 7072 6f62 655f  f"/probe/{probe_
+00010b30: 6964 7d22 2c0a 2020 2020 2020 2020 6461  id}",.        da
+00010b40: 7461 3d64 6174 612c 0a20 2020 2020 2020  ta=data,.       
+00010b50: 2068 6561 6465 7273 3d7b 2243 6f6e 7465   headers={"Conte
+00010b60: 6e74 2d54 7970 6522 3a20 2261 7070 6c69  nt-Type": "appli
+00010b70: 6361 7469 6f6e 2f6a 736f 6e22 7d2c 0a20  cation/json"},. 
+00010b80: 2020 2029 0a0a 2020 2020 6966 2072 6573     )..    if res
+00010b90: 756c 742e 7374 6174 7573 5f63 6f64 6520  ult.status_code 
+00010ba0: 213d 2032 3030 3a0a 2020 2020 2020 2020  != 200:.        
+00010bb0: 5f68 616e 646c 655f 6572 726f 7228 7265  _handle_error(re
+00010bc0: 7375 6c74 2c20 2243 616e 6e6f 7420 7570  sult, "Cannot up
+00010bd0: 6461 7465 2070 726f 6265 2069 6e66 6f72  date probe infor
+00010be0: 6d61 7469 6f6e 2077 6974 6820 636f 7265  mation with core
+00010bf0: 2041 5049 2229 0a0a 2020 2020 7265 7475   API")..    retu
+00010c00: 726e 2072 6573 756c 742e 6a73 6f6e 2829  rn result.json()
+00010c10: 0a0a 0a64 6566 2064 656c 6574 655f 7072  ...def delete_pr
+00010c20: 6f62 6528 7072 6f62 655f 6964 3a20 696e  obe(probe_id: in
+00010c30: 7429 202d 3e20 416e 793a 0a20 2020 2022  t) -> Any:.    "
+00010c40: 2222 4465 6c65 7465 2073 696d 756c 6174  ""Delete simulat
+00010c50: 696f 6e20 7072 6f62 6520 6769 7665 6e20  ion probe given 
+00010c60: 6974 7320 4944 2e0a 0a20 2020 203a 7265  its ID...    :re
+00010c70: 7475 726e 3a20 4120 6d65 7373 6167 6520  turn: A message 
+00010c80: 7465 6c6c 696e 6720 686f 7720 7468 6520  telling how the 
+00010c90: 6f70 6572 6174 696f 6e20 6578 6563 7574  operation execut
+00010ca0: 6564 2e0a 0a20 2020 203a 7061 7261 6d20  ed...    :param 
+00010cb0: 7072 6f62 655f 6964 3a20 5468 6520 7072  probe_id: The pr
+00010cc0: 6f62 6520 4944 2e0a 0a20 2020 2022 2222  obe ID...    """
+00010cd0: 0a0a 2020 2020 2320 4465 6c65 7465 2070  ..    # Delete p
+00010ce0: 726f 6265 0a20 2020 2072 6573 756c 7420  robe.    result 
+00010cf0: 3d20 5f64 656c 6574 6528 6622 2f70 726f  = _delete(f"/pro
+00010d00: 6265 2f7b 7072 6f62 655f 6964 7d22 290a  be/{probe_id}").
+00010d10: 0a20 2020 2069 6620 7265 7375 6c74 2e73  .    if result.s
+00010d20: 7461 7475 735f 636f 6465 2021 3d20 3230  tatus_code != 20
+00010d30: 303a 0a20 2020 2020 2020 205f 6861 6e64  0:.        _hand
+00010d40: 6c65 5f65 7272 6f72 2872 6573 756c 742c  le_error(result,
+00010d50: 2022 4361 6e6e 6f74 2064 656c 6574 6520   "Cannot delete 
+00010d60: 7072 6f62 6522 290a 0a20 2020 2072 6574  probe")..    ret
+00010d70: 7572 6e20 7265 7375 6c74 2e6a 736f 6e28  urn result.json(
+00010d80: 290a 0a0a 6465 6620 6665 7463 685f 6261  )...def fetch_ba
+00010d90: 7365 626f 7865 7328 2920 2d3e 2041 6e79  seboxes() -> Any
+00010da0: 3a0a 2020 2020 2222 2252 6574 7572 6e20  :.    """Return 
+00010db0: 6261 7365 626f 7865 7320 6c69 7374 2e0a  baseboxes list..
+00010dc0: 0a20 2020 203a 7265 7475 726e 3a20 5468  .    :return: Th
+00010dd0: 6520 6c69 7374 206f 6620 6261 7365 626f  e list of basebo
+00010de0: 7865 7320 6469 6374 2e0a 0a20 2020 2022  xes dict...    "
+00010df0: 2222 0a20 2020 2072 6573 756c 7420 3d20  "".    result = 
+00010e00: 5f67 6574 2822 2f62 6173 6562 6f78 2229  _get("/basebox")
+00010e10: 0a0a 2020 2020 6966 2072 6573 756c 742e  ..    if result.
+00010e20: 7374 6174 7573 5f63 6f64 6520 213d 2032  status_code != 2
+00010e30: 3030 3a0a 2020 2020 2020 2020 5f68 616e  00:.        _han
+00010e40: 646c 655f 6572 726f 7228 7265 7375 6c74  dle_error(result
+00010e50: 2c20 2243 616e 6e6f 7420 7265 7472 6965  , "Cannot retrie
+00010e60: 7665 2062 6173 6562 6f78 6573 206c 6973  ve baseboxes lis
+00010e70: 7420 6672 6f6d 2049 5420 5369 6d75 6c61  t from IT Simula
+00010e80: 7469 6f6e 2041 5049 2229 0a0a 2020 2020  tion API")..    
+00010e90: 6261 7365 626f 7865 7320 3d20 7265 7375  baseboxes = resu
+00010ea0: 6c74 2e6a 736f 6e28 290a 2020 2020 7265  lt.json().    re
+00010eb0: 7475 726e 2062 6173 6562 6f78 6573 0a0a  turn baseboxes..
+00010ec0: 0a64 6566 2066 6574 6368 5f62 6173 6562  .def fetch_baseb
+00010ed0: 6f78 2869 645f 6261 7365 626f 783a 2073  ox(id_basebox: s
+00010ee0: 7472 2920 2d3e 2041 6e79 3a0a 2020 2020  tr) -> Any:.    
+00010ef0: 2222 2252 6574 7572 6e20 6261 7365 626f  """Return basebo
+00010f00: 7820 6769 7665 6e20 6120 6261 7365 626f  x given a basebo
+00010f10: 7820 4944 2e0a 0a20 2020 203a 7265 7475  x ID...    :retu
+00010f20: 726e 3a20 5468 6520 6261 7365 626f 7820  rn: The basebox 
+00010f30: 6469 6374 2e0a 0a20 2020 203a 7061 7261  dict...    :para
+00010f40: 6d20 6964 5f62 6173 6562 6f78 3a20 5468  m id_basebox: Th
+00010f50: 6520 6261 7365 626f 7820 4944 2e0a 0a20  e basebox ID... 
+00010f60: 2020 2022 2222 0a20 2020 2072 6573 756c     """.    resul
+00010f70: 7420 3d20 5f67 6574 2866 222f 6261 7365  t = _get(f"/base
+00010f80: 626f 782f 6964 2f7b 6964 5f62 6173 6562  box/id/{id_baseb
+00010f90: 6f78 7d22 290a 0a20 2020 2069 6620 7265  ox}")..    if re
+00010fa0: 7375 6c74 2e73 7461 7475 735f 636f 6465  sult.status_code
+00010fb0: 2021 3d20 3230 303a 0a20 2020 2020 2020   != 200:.       
+00010fc0: 205f 6861 6e64 6c65 5f65 7272 6f72 2872   _handle_error(r
+00010fd0: 6573 756c 742c 2022 4361 6e6e 6f74 2072  esult, "Cannot r
+00010fe0: 6574 7269 6576 6520 6261 7365 626f 7820  etrieve basebox 
+00010ff0: 696e 666f 2066 726f 6d20 4954 2053 696d  info from IT Sim
+00011000: 756c 6174 696f 6e20 4150 4922 290a 0a20  ulation API").. 
+00011010: 2020 2062 6173 6562 6f78 203d 2072 6573     basebox = res
+00011020: 756c 742e 6a73 6f6e 2829 0a20 2020 2072  ult.json().    r
+00011030: 6574 7572 6e20 6261 7365 626f 780a 0a0a  eturn basebox...
+00011040: 6465 6620 7265 6c6f 6164 5f62 6173 6562  def reload_baseb
+00011050: 6f78 6573 2829 202d 3e20 416e 793a 0a20  oxes() -> Any:. 
+00011060: 2020 2022 2222 0a20 2020 2043 616c 6c20     """.    Call 
+00011070: 7468 6520 6379 6265 7220 7261 6e67 6520  the cyber range 
+00011080: 4150 4920 746f 2072 656c 6f61 6420 7468  API to reload th
+00011090: 6520 6c69 7374 206f 6620 6176 6169 6c61  e list of availa
+000110a0: 626c 6520 6261 7365 626f 7865 732e 0a0a  ble baseboxes...
+000110b0: 2020 2020 3a72 6574 7572 6e3a 2041 206d      :return: A m
+000110c0: 6573 7361 6765 2074 656c 6c69 6e67 2068  essage telling h
+000110d0: 6f77 2074 6865 206f 7065 7261 7469 6f6e  ow the operation
+000110e0: 2065 7865 6375 7465 642e 0a0a 2020 2020   executed...    
+000110f0: 2222 220a 2020 2020 7265 7375 6c74 203d  """.    result =
+00011100: 205f 6765 7428 222f 6261 7365 626f 782f   _get("/basebox/
+00011110: 7265 6c6f 6164 2229 0a0a 2020 2020 6966  reload")..    if
+00011120: 2072 6573 756c 742e 7374 6174 7573 5f63   result.status_c
+00011130: 6f64 6520 213d 2032 3030 3a0a 2020 2020  ode != 200:.    
+00011140: 2020 2020 5f68 616e 646c 655f 6572 726f      _handle_erro
+00011150: 7228 7265 7375 6c74 2c20 2243 616e 6e6f  r(result, "Canno
+00011160: 7420 7265 7472 6965 7665 2062 6173 6562  t retrieve baseb
+00011170: 6f78 2069 6e66 6f20 6672 6f6d 2049 5420  ox info from IT 
+00011180: 5369 6d75 6c61 7469 6f6e 2041 5049 2229  Simulation API")
+00011190: 0a0a 2020 2020 7265 7475 726e 2072 6573  ..    return res
+000111a0: 756c 742e 6a73 6f6e 2829 0a0a 0a64 6566  ult.json()...def
+000111b0: 2076 6572 6966 795f 6261 7365 626f 785f   verify_basebox_
+000111c0: 7265 7375 6c74 2874 6173 6b5f 6964 3a20  result(task_id: 
+000111d0: 7374 7229 202d 3e20 416e 793a 0a20 2020  str) -> Any:.   
+000111e0: 2022 2222 4361 6c6c 2074 6865 2041 5049   """Call the API
+000111f0: 2074 6f20 6765 7420 7468 6520 7265 7375   to get the resu
+00011200: 6c74 2074 6865 2063 7572 7265 6e74 2076  lt the current v
+00011210: 6572 6966 6963 6174 696f 6e2e 0a0a 2020  erification...  
+00011220: 2020 3a70 6172 616d 2074 6173 6b5f 6964    :param task_id
+00011230: 3a20 5468 6520 7461 736b 2049 442e 0a0a  : The task ID...
+00011240: 2020 2020 3a72 6574 7572 6e3a 2054 6865      :return: The
+00011250: 2072 6573 756c 7420 6f66 2074 6865 2076   result of the v
+00011260: 6572 6966 6963 6174 696f 6e2e 0a0a 2020  erification...  
+00011270: 2020 2222 220a 0a20 2020 2064 6174 6120    """..    data 
+00011280: 3d20 7b22 7461 736b 5f69 6422 3a20 7461  = {"task_id": ta
+00011290: 736b 5f69 647d 0a0a 2020 2020 7472 793a  sk_id}..    try:
+000112a0: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+000112b0: 3d20 5f70 6f73 7428 0a20 2020 2020 2020  = _post(.       
+000112c0: 2020 2020 2022 2f62 6173 6562 6f78 2f72       "/basebox/r
+000112d0: 6573 756c 745f 7665 7269 6679 222c 0a20  esult_verify",. 
+000112e0: 2020 2020 2020 2020 2020 2064 6174 613d             data=
+000112f0: 6461 7461 2c0a 2020 2020 2020 2020 290a  data,.        ).
+00011300: 0a20 2020 2020 2020 2069 6620 7265 7375  .        if resu
+00011310: 6c74 2e73 7461 7475 735f 636f 6465 2021  lt.status_code !
+00011320: 3d20 3230 303a 0a20 2020 2020 2020 2020  = 200:.         
+00011330: 2020 205f 6861 6e64 6c65 5f65 7272 6f72     _handle_error
+00011340: 2872 6573 756c 742c 2022 4361 6e6e 6f74  (result, "Cannot
+00011350: 2067 6574 2076 6572 6966 6963 6174 696f   get verificatio
+00011360: 6e20 7265 7375 6c74 2229 0a0a 2020 2020  n result")..    
+00011370: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+00011380: 742e 6a73 6f6e 2829 0a0a 2020 2020 6578  t.json()..    ex
+00011390: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
+000113a0: 7320 653a 0a20 2020 2020 2020 2072 6169  s e:.        rai
+000113b0: 7365 2045 7863 6570 7469 6f6e 2822 4973  se Exception("Is
+000113c0: 7375 6520 7768 656e 2067 6574 7469 6e67  sue when getting
+000113d0: 2076 6572 6966 6963 6174 696f 6e20 7265   verification re
+000113e0: 7375 6c74 3a20 277b 7d27 222e 666f 726d  sult: '{}'".form
+000113f0: 6174 2865 2929 0a0a 0a64 6566 2076 6572  at(e))...def ver
+00011400: 6966 795f 6261 7365 626f 785f 7374 6f70  ify_basebox_stop
+00011410: 2874 6173 6b5f 6964 3a20 7374 7229 202d  (task_id: str) -
+00011420: 3e20 416e 793a 0a20 2020 2022 2222 4361  > Any:.    """Ca
+00011430: 6c6c 2074 6865 2041 5049 2074 6f20 7374  ll the API to st
+00011440: 6f70 2074 6865 2063 7572 7265 6e74 2076  op the current v
+00011450: 6572 6966 6963 6174 696f 6e2e 0a0a 2020  erification...  
+00011460: 2020 3a72 6574 7572 6e3a 2041 206d 6573    :return: A mes
+00011470: 7361 6765 2074 656c 6c69 6e67 2068 6f77  sage telling how
+00011480: 2074 6865 206f 7065 7261 7469 6f6e 2065   the operation e
+00011490: 7865 6375 7465 642e 0a0a 2020 2020 3a70  xecuted...    :p
+000114a0: 6172 616d 2074 6173 6b5f 6964 3a20 5468  aram task_id: Th
+000114b0: 6520 7461 736b 2049 442e 0a0a 2020 2020  e task ID...    
+000114c0: 2222 220a 2020 2020 6461 7461 203d 207b  """.    data = {
+000114d0: 2274 6173 6b5f 6964 223a 2074 6173 6b5f  "task_id": task_
+000114e0: 6964 7d0a 0a20 2020 2072 6573 756c 7420  id}..    result 
+000114f0: 3d20 5f70 6f73 7428 222f 6261 7365 626f  = _post("/basebo
+00011500: 782f 7374 6f70 5f76 6572 6966 7922 2c20  x/stop_verify", 
+00011510: 6461 7461 3d64 6174 6129 0a0a 2020 2020  data=data)..    
+00011520: 6966 2072 6573 756c 742e 7374 6174 7573  if result.status
+00011530: 5f63 6f64 6520 213d 2032 3030 3a0a 2020  _code != 200:.  
+00011540: 2020 2020 2020 5f68 616e 646c 655f 6572        _handle_er
+00011550: 726f 7228 7265 7375 6c74 2c20 2243 616e  ror(result, "Can
+00011560: 6e6f 7420 7374 6f70 2076 6572 6966 6963  not stop verific
+00011570: 6174 696f 6e20 7461 736b 2229 0a0a 2020  ation task")..  
+00011580: 2020 7265 7475 726e 2072 6573 756c 742e    return result.
+00011590: 6a73 6f6e 2829 0a0a 0a64 6566 2076 6572  json()...def ver
+000115a0: 6966 795f 6261 7365 626f 785f 7374 6174  ify_basebox_stat
+000115b0: 7573 2874 6173 6b5f 6964 3a20 7374 7229  us(task_id: str)
+000115c0: 202d 3e20 416e 793a 0a20 2020 2022 2222   -> Any:.    """
+000115d0: 0a20 2020 2043 616c 6c20 7468 6520 4150  .    Call the AP
+000115e0: 4920 746f 2067 6574 2074 6865 2073 7461  I to get the sta
+000115f0: 7475 7320 6f66 2063 7572 7265 6e74 2076  tus of current v
+00011600: 6572 6966 6963 6174 696f 6e0a 0a20 2020  erification..   
+00011610: 203a 7265 7475 726e 3a20 4120 6d65 7373   :return: A mess
+00011620: 6167 6520 7465 6c6c 696e 6720 686f 7720  age telling how 
+00011630: 7468 6520 6f70 6572 6174 696f 6e20 6578  the operation ex
+00011640: 6563 7574 6564 2e0a 0a20 2020 203a 7061  ecuted...    :pa
+00011650: 7261 6d20 7461 736b 5f69 643a 2054 6865  ram task_id: The
+00011660: 2074 6173 6b20 4944 2e0a 0a20 2020 2022   task ID...    "
+00011670: 2222 0a20 2020 2064 6174 6120 3d20 7b22  "".    data = {"
+00011680: 7461 736b 5f69 6422 3a20 7461 736b 5f69  task_id": task_i
+00011690: 647d 0a0a 2020 2020 7472 793a 0a20 2020  d}..    try:.   
+000116a0: 2020 2020 2072 6573 756c 7420 3d20 5f70       result = _p
+000116b0: 6f73 7428 222f 6261 7365 626f 782f 7374  ost("/basebox/st
+000116c0: 6174 7573 5f76 6572 6966 7922 2c20 6461  atus_verify", da
+000116d0: 7461 3d64 6174 6129 0a0a 2020 2020 2020  ta=data)..      
+000116e0: 2020 6966 2072 6573 756c 742e 7374 6174    if result.stat
+000116f0: 7573 5f63 6f64 6520 213d 2032 3030 3a0a  us_code != 200:.
+00011700: 2020 2020 2020 2020 2020 2020 5f68 616e              _han
+00011710: 646c 655f 6572 726f 7228 7265 7375 6c74  dle_error(result
+00011720: 2c20 2243 616e 6e6f 7420 6765 7420 7665  , "Cannot get ve
+00011730: 7269 6679 2073 7461 7475 7322 290a 0a20  rify status").. 
+00011740: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+00011750: 7375 6c74 2e6a 736f 6e28 290a 0a20 2020  sult.json()..   
+00011760: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+00011770: 6e20 6173 2065 3a0a 2020 2020 2020 2020  n as e:.        
+00011780: 7261 6973 6520 4578 6365 7074 696f 6e28  raise Exception(
+00011790: 2249 7373 7565 2077 6865 6e20 6765 7474  "Issue when gett
+000117a0: 696e 6720 7665 7269 6679 2073 7461 7475  ing verify statu
+000117b0: 733a 2027 7b7d 2722 2e66 6f72 6d61 7428  s: '{}'".format(
+000117c0: 6529 290a 0a0a 6465 6620 7665 7269 6679  e))...def verify
+000117d0: 5f62 6173 6562 6f78 2862 6173 6562 6f78  _basebox(basebox
+000117e0: 5f69 643a 2069 6e74 2920 2d3e 2044 6963  _id: int) -> Dic
+000117f0: 743a 0a20 2020 2022 2222 4361 6c6c 2074  t:.    """Call t
+00011800: 6865 2041 5049 2074 6f20 7665 7269 6679  he API to verify
+00011810: 2074 6865 2069 6e74 6567 7269 7479 206f   the integrity o
+00011820: 6620 7468 6520 6769 7665 6e20 6261 7365  f the given base
+00011830: 626f 7820 6261 7365 6420 6f6e 2069 7473  box based on its
+00011840: 2049 442e 0a0a 2020 2020 3a70 6172 616d   ID...    :param
+00011850: 2069 645f 6261 7365 626f 783a 2054 6865   id_basebox: The
+00011860: 2062 6173 6562 6f78 2049 442e 0a0a 2020   basebox ID...  
+00011870: 2020 3a72 6574 7572 6e3a 2041 2064 6963    :return: A dic
+00011880: 7420 636f 6e74 6169 6e69 6e67 2076 6572  t containing ver
+00011890: 6966 6963 6174 696f 6e20 7265 7375 6c74  ification result
+000118a0: 732e 0a0a 2020 2020 2222 220a 2020 2020  s...    """.    
+000118b0: 7265 7375 6c74 203d 205f 6765 7428 6622  result = _get(f"
+000118c0: 2f62 6173 6562 6f78 2f76 6572 6966 792f  /basebox/verify/
+000118d0: 7b62 6173 6562 6f78 5f69 647d 2229 0a0a  {basebox_id}")..
+000118e0: 2020 2020 6966 2072 6573 756c 742e 7374      if result.st
+000118f0: 6174 7573 5f63 6f64 6520 213d 2032 3030  atus_code != 200
+00011900: 3a0a 2020 2020 2020 2020 5f68 616e 646c  :.        _handl
+00011910: 655f 6572 726f 7228 7265 7375 6c74 2c20  e_error(result, 
+00011920: 2243 616e 6e6f 7420 7265 7472 6965 7665  "Cannot retrieve
+00011930: 2062 6173 6562 6f78 2069 6e66 6f20 6672   basebox info fr
+00011940: 6f6d 2049 5420 5369 6d75 6c61 7469 6f6e  om IT Simulation
+00011950: 2041 5049 2229 0a0a 2020 2020 7265 7375   API")..    resu
+00011960: 6c74 203d 2072 6573 756c 742e 6a73 6f6e  lt = result.json
+00011970: 2829 0a20 2020 2074 6173 6b5f 6964 203d  ().    task_id =
+00011980: 2072 6573 756c 745b 2274 6173 6b5f 6964   result["task_id
+00011990: 225d 0a20 2020 2073 7563 6365 7373 203d  "].    success =
+000119a0: 2072 6573 756c 745b 2272 6573 756c 7422   result["result"
+000119b0: 5d20 3d3d 2022 5354 4152 5445 4422 0a0a  ] == "STARTED"..
+000119c0: 2020 2020 6966 206e 6f74 2073 7563 6365      if not succe
+000119d0: 7373 3a0a 2020 2020 2020 2020 5f62 6173  ss:.        _bas
+000119e0: 6562 6f78 6573 5f76 6572 6966 795f 7261  eboxes_verify_ra
+000119f0: 6973 655f 6572 726f 725f 6d73 6728 7265  ise_error_msg(re
+00011a00: 7375 6c74 290a 0a20 2020 206c 6f67 6765  sult)..    logge
+00011a10: 722e 696e 666f 2866 225b 2b5d 2056 6572  r.info(f"[+] Ver
+00011a20: 6966 6963 6174 696f 6e20 7461 736b 2049  ification task I
+00011a30: 443a 207b 7461 736b 5f69 647d 2229 0a0a  D: {task_id}")..
+00011a40: 2020 2020 7265 7375 6c74 203d 205f 5f68      result = __h
+00011a50: 616e 646c 655f 7761 6974 5f62 6173 6562  andle_wait_baseb
+00011a60: 6f78 5f76 6572 6966 7928 0a20 2020 2020  ox_verify(.     
+00011a70: 2020 2077 6169 743d 5472 7565 2c20 7461     wait=True, ta
+00011a80: 736b 5f69 643d 7461 736b 5f69 642c 206c  sk_id=task_id, l
+00011a90: 6f67 5f73 7566 6669 783d 7374 7228 6261  og_suffix=str(ba
+00011aa0: 7365 626f 785f 6964 292c 2074 696d 656f  sebox_id), timeo
+00011ab0: 7574 3d33 3630 300a 2020 2020 290a 0a20  ut=3600.    ).. 
+00011ac0: 2020 2072 6574 7572 6e20 7b0a 2020 2020     return {.    
+00011ad0: 2020 2020 2273 7563 6365 7373 223a 2072      "success": r
+00011ae0: 6573 756c 745b 2273 7563 6365 7373 225d  esult["success"]
+00011af0: 2c0a 2020 2020 2020 2020 2274 6173 6b5f  ,.        "task_
+00011b00: 6964 223a 2074 6173 6b5f 6964 2c0a 2020  id": task_id,.  
+00011b10: 2020 2020 2020 2272 6573 756c 7422 3a20        "result": 
+00011b20: 7265 7375 6c74 5b22 7265 7375 6c74 225d  result["result"]
+00011b30: 2c0a 2020 2020 7d0a 0a0a 6465 6620 7665  ,.    }...def ve
+00011b40: 7269 6679 5f62 6173 6562 6f78 6573 2829  rify_baseboxes()
+00011b50: 202d 3e20 4469 6374 3a0a 2020 2020 2222   -> Dict:.    ""
+00011b60: 2243 616c 6c20 7468 6520 4150 4920 746f  "Call the API to
+00011b70: 2076 6572 6966 7920 7468 6520 6368 6563   verify the chec
+00011b80: 6b73 756d 206f 6620 616c 6c20 6261 7365  ksum of all base
+00011b90: 626f 7865 732e 0a0a 2020 2020 3a72 6574  boxes...    :ret
+00011ba0: 7572 6e3a 2041 2064 6963 7420 636f 6e74  urn: A dict cont
+00011bb0: 6169 6e69 6e67 2076 6572 6966 6963 6174  aining verificat
+00011bc0: 696f 6e20 7265 7375 6c74 732e 0a20 2020  ion results..   
+00011bd0: 2022 2222 0a20 2020 2072 6573 756c 7420   """.    result 
+00011be0: 3d20 5f67 6574 2822 2f62 6173 6562 6f78  = _get("/basebox
+00011bf0: 2f76 6572 6966 792f 2229 0a0a 2020 2020  /verify/")..    
+00011c00: 6966 2072 6573 756c 742e 7374 6174 7573  if result.status
+00011c10: 5f63 6f64 6520 213d 2032 3030 3a0a 2020  _code != 200:.  
+00011c20: 2020 2020 2020 5f68 616e 646c 655f 6572        _handle_er
+00011c30: 726f 7228 7265 7375 6c74 2c20 2243 616e  ror(result, "Can
+00011c40: 6e6f 7420 7265 7472 6965 7665 2062 6173  not retrieve bas
+00011c50: 6562 6f78 2069 6e66 6f20 6672 6f6d 2049  ebox info from I
+00011c60: 5420 5369 6d75 6c61 7469 6f6e 2041 5049  T Simulation API
+00011c70: 2229 0a0a 2020 2020 7265 7375 6c74 203d  ")..    result =
+00011c80: 2072 6573 756c 742e 6a73 6f6e 2829 0a20   result.json(). 
+00011c90: 2020 2074 6173 6b5f 6964 203d 2072 6573     task_id = res
+00011ca0: 756c 745b 2274 6173 6b5f 6964 225d 0a20  ult["task_id"]. 
+00011cb0: 2020 2073 7563 6365 7373 203d 2072 6573     success = res
+00011cc0: 756c 745b 2272 6573 756c 7422 5d20 3d3d  ult["result"] ==
+00011cd0: 2022 5354 4152 5445 4422 0a0a 2020 2020   "STARTED"..    
+00011ce0: 6966 206e 6f74 2073 7563 6365 7373 3a0a  if not success:.
+00011cf0: 2020 2020 2020 2020 5f62 6173 6562 6f78          _basebox
+00011d00: 6573 5f76 6572 6966 795f 7261 6973 655f  es_verify_raise_
+00011d10: 6572 726f 725f 6d73 6728 7265 7375 6c74  error_msg(result
+00011d20: 290a 0a20 2020 206c 6f67 6765 722e 696e  )..    logger.in
+00011d30: 666f 2866 225b 2b5d 2056 6572 6966 6963  fo(f"[+] Verific
+00011d40: 6174 696f 6e20 7461 736b 2049 443a 207b  ation task ID: {
+00011d50: 7461 736b 5f69 647d 2229 0a0a 2020 2020  task_id}")..    
+00011d60: 7265 7375 6c74 203d 205f 5f68 616e 646c  result = __handl
+00011d70: 655f 7761 6974 5f62 6173 6562 6f78 5f76  e_wait_basebox_v
+00011d80: 6572 6966 7928 0a20 2020 2020 2020 2077  erify(.        w
+00011d90: 6169 743d 5472 7565 2c20 7461 736b 5f69  ait=True, task_i
+00011da0: 643d 7461 736b 5f69 642c 206c 6f67 5f73  d=task_id, log_s
+00011db0: 7566 6669 783d 2261 6c6c 2062 6173 6562  uffix="all baseb
+00011dc0: 6f78 6573 222c 2074 696d 656f 7574 3d33  oxes", timeout=3
+00011dd0: 3630 300a 2020 2020 290a 0a20 2020 2072  600.    )..    r
+00011de0: 6574 7572 6e20 7b0a 2020 2020 2020 2020  eturn {.        
+00011df0: 2273 7563 6365 7373 223a 2072 6573 756c  "success": resul
+00011e00: 745b 2273 7563 6365 7373 225d 2c0a 2020  t["success"],.  
+00011e10: 2020 2020 2020 2274 6173 6b5f 6964 223a        "task_id":
+00011e20: 2074 6173 6b5f 6964 2c0a 2020 2020 2020   task_id,.      
+00011e30: 2020 2272 6573 756c 7422 3a20 7265 7375    "result": resu
+00011e40: 6c74 5b22 7265 7375 6c74 225d 2c0a 2020  lt["result"],.  
+00011e50: 2020 7d0a 0a0a 6465 6620 6665 7463 685f    }...def fetch_
+00011e60: 646f 6d61 696e 7328 2920 2d3e 2044 6963  domains() -> Dic
+00011e70: 745b 7374 722c 2073 7472 5d3a 0a20 2020  t[str, str]:.   
+00011e80: 2022 2222 5265 7475 726e 7320 7468 6520   """Returns the 
+00011e90: 6d61 7070 696e 6720 646f 6d61 696e 2d3e  mapping domain->
+00011ea0: 4950 2e0a 0a20 2020 203a 7265 7475 726e  IP...    :return
+00011eb0: 3a20 5468 6520 6c69 7374 206f 6620 646f  : The list of do
+00011ec0: 6d61 696e 2064 6963 7473 2e0a 0a20 2020  main dicts...   
+00011ed0: 2022 2222 0a0a 2020 2020 2320 4649 584d   """..    # FIXM
+00011ee0: 4528 6d75 6c74 692d 7465 6e61 6e74 293a  E(multi-tenant):
+00011ef0: 2077 6520 7368 6f75 6c64 2072 6574 7269   we should retri
+00011f00: 6576 6520 646f 6d61 696e 7320 6163 636f  eve domains acco
+00011f10: 7264 696e 6720 746f 2061 2073 696d 756c  rding to a simul
+00011f20: 6174 696f 6e20 6964 0a20 2020 2072 6573  ation id.    res
+00011f30: 756c 7420 3d20 5f67 6574 2822 2f6e 6574  ult = _get("/net
+00011f40: 776f 726b 5f69 6e74 6572 6661 6365 2f64  work_interface/d
+00011f50: 6f6d 6169 6e73 2229 0a0a 2020 2020 6966  omains")..    if
+00011f60: 2072 6573 756c 742e 7374 6174 7573 5f63   result.status_c
+00011f70: 6f64 6520 213d 2032 3030 3a0a 2020 2020  ode != 200:.    
+00011f80: 2020 2020 5f68 616e 646c 655f 6572 726f      _handle_erro
+00011f90: 7228 7265 7375 6c74 2c20 2245 7272 6f72  r(result, "Error
+00011fa0: 2077 6869 6c65 2066 6574 6368 696e 6720   while fetching 
+00011fb0: 646f 6d61 696e 7322 290a 0a20 2020 2072  domains")..    r
+00011fc0: 6574 7572 6e20 7265 7375 6c74 2e6a 736f  eturn result.jso
+00011fd0: 6e28 290a 0a0a 6465 6620 6665 7463 685f  n()...def fetch_
+00011fe0: 7765 6273 6974 6573 2829 202d 3e20 416e  websites() -> An
+00011ff0: 793a 0a20 2020 2022 2222 5265 7475 726e  y:.    """Return
+00012000: 2074 6865 2077 6562 7369 7465 7320 6c69   the websites li
+00012010: 7374 2e0a 0a20 2020 203a 7265 7475 726e  st...    :return
+00012020: 3a20 5468 6520 6c69 7374 206f 6620 7765  : The list of we
+00012030: 6273 6974 6520 6469 6374 732e 0a0a 2020  bsite dicts...  
+00012040: 2020 2222 220a 2020 2020 7265 7375 6c74    """.    result
+00012050: 203d 205f 6765 7428 222f 7765 6273 6974   = _get("/websit
+00012060: 6522 290a 0a20 2020 2069 6620 7265 7375  e")..    if resu
+00012070: 6c74 2e73 7461 7475 735f 636f 6465 2021  lt.status_code !
+00012080: 3d20 3230 303a 0a20 2020 2020 2020 205f  = 200:.        _
+00012090: 6861 6e64 6c65 5f65 7272 6f72 2872 6573  handle_error(res
+000120a0: 756c 742c 2022 4361 6e6e 6f74 2072 6574  ult, "Cannot ret
+000120b0: 7269 6576 6520 7765 6273 6974 6573 206c  rieve websites l
+000120c0: 6973 7420 6672 6f6d 2049 5420 5369 6d75  ist from IT Simu
+000120d0: 6c61 7469 6f6e 2041 5049 2229 0a0a 2020  lation API")..  
+000120e0: 2020 7765 6273 6974 6573 203d 2072 6573    websites = res
+000120f0: 756c 742e 6a73 6f6e 2829 0a20 2020 2072  ult.json().    r
+00012100: 6574 7572 6e20 7765 6273 6974 6573 0a0a  eturn websites..
+00012110: 0a64 6566 2074 6f70 6f6c 6f67 795f 6164  .def topology_ad
+00012120: 645f 7765 6273 6974 6573 280a 2020 2020  d_websites(.    
+00012130: 746f 706f 6c6f 6779 5f79 616d 6c3a 2073  topology_yaml: s
+00012140: 7472 2c20 7765 6273 6974 6573 3a20 4c69  tr, websites: Li
+00012150: 7374 5b73 7472 5d2c 2073 7769 7463 685f  st[str], switch_
+00012160: 6e61 6d65 3a20 7374 720a 2920 2d3e 2073  name: str.) -> s
+00012170: 7472 3a0a 2020 2020 2222 2241 6464 2064  tr:.    """Add d
+00012180: 6f63 6b65 7220 7765 6273 6974 6573 206e  ocker websites n
+00012190: 6f64 6520 746f 2061 2067 6976 656e 2074  ode to a given t
+000121a0: 6f70 6f6c 6f67 792e 0a0a 2020 2020 3a72  opology...    :r
+000121b0: 6574 7572 6e3a 2054 6865 2075 7064 6174  eturn: The updat
+000121c0: 6564 2074 6f70 6f6c 6f67 7920 636f 6e74  ed topology cont
+000121d0: 656e 742e 0a0a 2020 2020 3a70 6172 616d  ent...    :param
+000121e0: 2074 6f70 6f6c 6f67 795f 7961 6d6c 3a20   topology_yaml: 
+000121f0: 5468 6520 696e 7075 7420 746f 706f 6c6f  The input topolo
+00012200: 6779 2063 6f6e 7465 6e74 2061 7320 6120  gy content as a 
+00012210: 7374 7269 6e67 2e0a 2020 2020 3a70 6172  string..    :par
+00012220: 616d 2077 6562 7369 7465 733a 2054 6865  am websites: The
+00012230: 206c 6973 7420 6f66 2077 6562 7369 7465   list of website
+00012240: 7320 746f 2061 6464 2e0a 2020 2020 3a70  s to add..    :p
+00012250: 6172 616d 2073 7769 7463 685f 6e61 6d65  aram switch_name
+00012260: 3a20 5468 6520 7377 6974 6368 206f 6e20  : The switch on 
+00012270: 7768 6963 6820 746f 2063 6f6e 6e65 6374  which to connect
+00012280: 2074 6865 2064 6f63 6b65 7220 7765 6273   the docker webs
+00012290: 6974 6520 6e6f 6465 732e 0a0a 2020 2020  ite nodes...    
+000122a0: 2222 220a 0a20 2020 2064 6174 615f 6469  """..    data_di
+000122b0: 6374 203d 207b 0a20 2020 2020 2020 2022  ct = {.        "
+000122c0: 746f 706f 6c6f 6779 5f79 616d 6c22 3a20  topology_yaml": 
+000122d0: 746f 706f 6c6f 6779 5f79 616d 6c2c 0a20  topology_yaml,. 
+000122e0: 2020 2020 2020 2022 7765 6273 6974 6573         "websites
+000122f0: 223a 2077 6562 7369 7465 732c 0a20 2020  ": websites,.   
+00012300: 2020 2020 2022 7377 6974 6368 5f6e 616d       "switch_nam
+00012310: 6522 3a20 7377 6974 6368 5f6e 616d 652c  e": switch_name,
+00012320: 0a20 2020 207d 0a20 2020 2064 6174 6120  .    }.    data 
+00012330: 3d20 6a73 6f6e 2e64 756d 7073 2864 6174  = json.dumps(dat
+00012340: 615f 6469 6374 290a 2020 2020 7265 7375  a_dict).    resu
+00012350: 6c74 203d 205f 706f 7374 280a 2020 2020  lt = _post(.    
+00012360: 2020 2020 222f 746f 706f 6c6f 6779 2f61      "/topology/a
+00012370: 6464 5f77 6562 7369 7465 7322 2c0a 2020  dd_websites",.  
+00012380: 2020 2020 2020 6461 7461 3d64 6174 612c        data=data,
+00012390: 0a20 2020 2020 2020 2068 6561 6465 7273  .        headers
+000123a0: 3d7b 2243 6f6e 7465 6e74 2d54 7970 6522  ={"Content-Type"
+000123b0: 3a20 2261 7070 6c69 6361 7469 6f6e 2f6a  : "application/j
+000123c0: 736f 6e22 7d2c 0a20 2020 2029 0a0a 2020  son"},.    )..  
+000123d0: 2020 6966 2072 6573 756c 742e 7374 6174    if result.stat
+000123e0: 7573 5f63 6f64 6520 213d 2032 3030 3a0a  us_code != 200:.
+000123f0: 2020 2020 2020 2020 5f68 616e 646c 655f          _handle_
+00012400: 6572 726f 7228 7265 7375 6c74 2c20 2245  error(result, "E
+00012410: 7272 6f72 2077 6869 6c65 2061 6464 696e  rror while addin
+00012420: 6720 7765 6273 6974 6573 2074 6f20 6120  g websites to a 
+00012430: 746f 706f 6c6f 6779 2229 0a0a 2020 2020  topology")..    
+00012440: 746f 706f 6c6f 6779 5f79 616d 6c20 3d20  topology_yaml = 
+00012450: 7265 7375 6c74 2e6a 736f 6e28 295b 2274  result.json()["t
+00012460: 6f70 6f6c 6f67 795f 7961 6d6c 225d 0a0a  opology_yaml"]..
+00012470: 2020 2020 7265 7475 726e 2074 6f70 6f6c      return topol
+00012480: 6f67 795f 7961 6d6c 0a0a 0a64 6566 2074  ogy_yaml...def t
+00012490: 6f70 6f6c 6f67 795f 6164 645f 6467 6128  opology_add_dga(
+000124a0: 0a20 2020 2074 6f70 6f6c 6f67 795f 7961  .    topology_ya
+000124b0: 6d6c 3a20 7374 722c 0a20 2020 2061 6c67  ml: str,.    alg
+000124c0: 6f72 6974 686d 3a20 7374 722c 0a20 2020  orithm: str,.   
+000124d0: 2073 7769 7463 685f 6e61 6d65 3a20 7374   switch_name: st
+000124e0: 722c 0a20 2020 206e 756d 6265 723a 2069  r,.    number: i
+000124f0: 6e74 2c0a 2020 2020 7265 736f 7572 6365  nt,.    resource
+00012500: 735f 6469 723a 2073 7472 2c0a 2920 2d3e  s_dir: str,.) ->
+00012510: 2054 7570 6c65 5b73 7472 2c20 4c69 7374   Tuple[str, List
+00012520: 5b73 7472 5d5d 3a0a 2020 2020 2222 2241  [str]]:.    """A
+00012530: 6464 2064 6f63 6b65 7220 656d 7074 7920  dd docker empty 
+00012540: 7765 6273 6974 6573 2077 6974 6820 4447  websites with DG
+00012550: 4120 6e6f 6465 2074 6f20 6120 6769 7665  A node to a give
+00012560: 6e20 746f 706f 6c6f 6779 2e0a 0a20 2020  n topology...   
+00012570: 203a 7265 7475 726e 3a20 5468 6520 7475   :return: The tu
+00012580: 706c 6520 636f 6e74 6169 6e65 696e 6720  ple containeing 
+00012590: 7468 6520 7570 6461 7465 6420 746f 706f  the updated topo
+000125a0: 6c6f 6779 2061 7373 6f63 6961 7465 6420  logy associated 
+000125b0: 7769 7468 2074 6865 2064 6f6d 6169 6e73  with the domains
+000125c0: 2e0a 0a20 2020 203a 7061 7261 6d20 746f  ...    :param to
+000125d0: 706f 6c6f 6779 5f79 616d 6c3a 2054 6865  pology_yaml: The
+000125e0: 2069 6e70 7574 2074 6f70 6f6c 6f67 7920   input topology 
+000125f0: 636f 6e74 656e 7420 6173 2061 2073 7472  content as a str
+00012600: 696e 672e 0a20 2020 203a 7061 7261 6d20  ing..    :param 
+00012610: 616c 676f 7269 7468 6d3a 2054 6865 2061  algorithm: The a
+00012620: 6c67 6f72 6974 686d 2075 7365 6420 746f  lgorithm used to
+00012630: 2067 656e 6572 6174 6520 7468 6520 6e65   generate the ne
+00012640: 7720 4447 4120 646f 6d61 696e 732e 0a20  w DGA domains.. 
+00012650: 2020 203a 7061 7261 6d20 7377 6974 6368     :param switch
+00012660: 5f6e 616d 653a 2054 6865 2073 7769 7463  _name: The switc
+00012670: 6820 6f6e 2077 6869 6368 2074 6f20 636f  h on which to co
+00012680: 6e6e 6563 7420 7468 6520 646f 636b 6572  nnect the docker
+00012690: 2077 6562 7369 7465 206e 6f64 6573 2e0a   website nodes..
+000126a0: 2020 2020 3a70 6172 616d 206e 756d 6265      :param numbe
+000126b0: 723a 2054 6865 206e 756d 6265 7220 6f66  r: The number of
+000126c0: 2044 4741 2064 6f6d 6169 6e73 2074 6f20   DGA domains to 
+000126d0: 6164 642e 0a20 2020 203a 7061 7261 6d20  add..    :param 
+000126e0: 746f 706f 6c6f 6779 5f64 6972 3a20 5468  topology_dir: Th
+000126f0: 6520 7061 7468 2074 6f20 7265 736f 7572  e path to resour
+00012700: 6365 7320 7468 6174 2077 696c 6c20 6265  ces that will be
+00012710: 2070 7573 6865 6420 696e 746f 2074 6865   pushed into the
+00012720: 206e 6577 2064 6f63 6b65 7220 6e6f 6465   new docker node
+00012730: 732e 0a0a 2020 2020 2222 220a 0a20 2020  s...    """..   
+00012740: 2064 6174 615f 6469 6374 203d 207b 0a20   data_dict = {. 
+00012750: 2020 2020 2020 2022 746f 706f 6c6f 6779         "topology
+00012760: 5f79 616d 6c22 3a20 746f 706f 6c6f 6779  _yaml": topology
+00012770: 5f79 616d 6c2c 0a20 2020 2020 2020 2022  _yaml,.        "
+00012780: 616c 676f 7269 7468 6d22 3a20 616c 676f  algorithm": algo
+00012790: 7269 7468 6d2c 0a20 2020 2020 2020 2022  rithm,.        "
+000127a0: 7377 6974 6368 5f6e 616d 6522 3a20 7377  switch_name": sw
+000127b0: 6974 6368 5f6e 616d 652c 0a20 2020 2020  itch_name,.     
+000127c0: 2020 2022 6e75 6d62 6572 223a 206e 756d     "number": num
+000127d0: 6265 722c 0a20 2020 2020 2020 2022 7265  ber,.        "re
+000127e0: 736f 7572 6365 735f 6469 7222 3a20 7265  sources_dir": re
+000127f0: 736f 7572 6365 735f 6469 722c 0a20 2020  sources_dir,.   
+00012800: 207d 0a20 2020 2064 6174 6120 3d20 6a73   }.    data = js
+00012810: 6f6e 2e64 756d 7073 2864 6174 615f 6469  on.dumps(data_di
+00012820: 6374 290a 2020 2020 7265 7375 6c74 203d  ct).    result =
+00012830: 205f 706f 7374 280a 2020 2020 2020 2020   _post(.        
+00012840: 222f 746f 706f 6c6f 6779 2f61 6464 5f64  "/topology/add_d
+00012850: 6761 222c 0a20 2020 2020 2020 2064 6174  ga",.        dat
+00012860: 613d 6461 7461 2c0a 2020 2020 2020 2020  a=data,.        
+00012870: 6865 6164 6572 733d 7b22 436f 6e74 656e  headers={"Conten
+00012880: 742d 5479 7065 223a 2022 6170 706c 6963  t-Type": "applic
+00012890: 6174 696f 6e2f 6a73 6f6e 227d 2c0a 2020  ation/json"},.  
+000128a0: 2020 290a 0a20 2020 2069 6620 7265 7375    )..    if resu
+000128b0: 6c74 2e73 7461 7475 735f 636f 6465 2021  lt.status_code !
+000128c0: 3d20 3230 303a 0a20 2020 2020 2020 205f  = 200:.        _
+000128d0: 6861 6e64 6c65 5f65 7272 6f72 2872 6573  handle_error(res
+000128e0: 756c 742c 2022 4572 726f 7220 7768 696c  ult, "Error whil
+000128f0: 6520 6164 6469 6e67 2077 6562 7369 7465  e adding website
+00012900: 7320 746f 2061 2074 6f70 6f6c 6f67 7922  s to a topology"
+00012910: 290a 0a20 2020 2074 6f70 6f6c 6f67 795f  )..    topology_
+00012920: 7961 6d6c 203d 2072 6573 756c 742e 6a73  yaml = result.js
+00012930: 6f6e 2829 5b22 746f 706f 6c6f 6779 5f79  on()["topology_y
+00012940: 616d 6c22 5d0a 2020 2020 646f 6d61 696e  aml"].    domain
+00012950: 7320 3d20 7265 7375 6c74 2e6a 736f 6e28  s = result.json(
+00012960: 295b 2264 6f6d 6169 6e73 225d 0a0a 2020  )["domains"]..  
+00012970: 2020 7265 7475 726e 2074 6f70 6f6c 6f67    return topolog
+00012980: 795f 7961 6d6c 2c20 646f 6d61 696e 730a  y_yaml, domains.
+00012990: 0a0a 6465 6620 746f 706f 6c6f 6779 5f61  ..def topology_a
+000129a0: 6464 5f64 6e73 5f73 6572 7665 7228 0a20  dd_dns_server(. 
+000129b0: 2020 2074 6f70 6f6c 6f67 795f 7961 6d6c     topology_yaml
+000129c0: 3a20 7374 722c 0a20 2020 2073 7769 7463  : str,.    switc
+000129d0: 685f 6e61 6d65 3a20 7374 722c 0a20 2020  h_name: str,.   
+000129e0: 2072 6573 6f75 7263 6573 5f64 6972 3a20   resources_dir: 
+000129f0: 7374 722c 0a29 202d 3e20 5475 706c 655b  str,.) -> Tuple[
+00012a00: 7374 722c 2073 7472 5d3a 0a20 2020 2022  str, str]:.    "
+00012a10: 2222 0a0a 2020 2020 3a72 6574 7572 6e3a  ""..    :return:
+00012a20: 2054 6865 2074 7570 6c65 2063 6f6e 7461   The tuple conta
+00012a30: 696e 696e 6720 7468 6520 7570 6461 7465  ining the update
+00012a40: 6420 746f 706f 6c6f 6779 2061 7373 6f63  d topology assoc
+00012a50: 6961 7465 6420 7769 7468 2074 6865 2044  iated with the D
+00012a60: 4e53 2063 6f6e 6669 6775 7261 7469 6f6e  NS configuration
+00012a70: 2067 656e 6572 6174 6564 2e0a 0a20 2020   generated...   
+00012a80: 203a 7061 7261 6d20 746f 706f 6c6f 6779   :param topology
+00012a90: 5f79 616d 6c3a 2054 6865 2069 6e70 7574  _yaml: The input
+00012aa0: 2074 6f70 6f6c 6f67 7920 636f 6e74 656e   topology conten
+00012ab0: 7420 6173 2061 2073 7472 696e 672e 0a20  t as a string.. 
+00012ac0: 2020 203a 7061 7261 6d20 7377 6974 6368     :param switch
+00012ad0: 5f6e 616d 653a 2054 6865 2073 7769 7463  _name: The switc
+00012ae0: 6820 6f6e 2077 6869 6368 2074 6f20 636f  h on which to co
+00012af0: 6e6e 6563 7420 7468 6520 646f 636b 6572  nnect the docker
+00012b00: 2044 4e53 2073 6572 7665 7220 6e6f 6465   DNS server node
+00012b10: 2e0a 2020 2020 3a70 6172 616d 2074 6f70  ..    :param top
+00012b20: 6f6c 6f67 795f 6469 723a 2054 6865 2070  ology_dir: The p
+00012b30: 6174 6820 746f 2072 6573 6f75 7263 6573  ath to resources
+00012b40: 2074 6861 7420 7769 6c6c 2062 6520 7075   that will be pu
+00012b50: 7368 6564 2069 6e74 6f20 7468 6520 6e65  shed into the ne
+00012b60: 7720 646f 636b 6572 206e 6f64 652e 0a0a  w docker node...
+00012b70: 2020 2020 2222 220a 2020 2020 6461 7461      """.    data
+00012b80: 5f64 6963 7420 3d20 7b0a 2020 2020 2020  _dict = {.      
+00012b90: 2020 2274 6f70 6f6c 6f67 795f 7961 6d6c    "topology_yaml
+00012ba0: 223a 2074 6f70 6f6c 6f67 795f 7961 6d6c  ": topology_yaml
+00012bb0: 2c0a 2020 2020 2020 2020 2273 7769 7463  ,.        "switc
+00012bc0: 685f 6e61 6d65 223a 2073 7769 7463 685f  h_name": switch_
+00012bd0: 6e61 6d65 2c0a 2020 2020 2020 2020 2272  name,.        "r
+00012be0: 6573 6f75 7263 6573 5f64 6972 223a 2072  esources_dir": r
+00012bf0: 6573 6f75 7263 6573 5f64 6972 2c0a 2020  esources_dir,.  
+00012c00: 2020 7d0a 2020 2020 6461 7461 203d 206a    }.    data = j
+00012c10: 736f 6e2e 6475 6d70 7328 6461 7461 5f64  son.dumps(data_d
+00012c20: 6963 7429 0a20 2020 2072 6573 756c 7420  ict).    result 
+00012c30: 3d20 5f70 6f73 7428 0a20 2020 2020 2020  = _post(.       
+00012c40: 2022 2f74 6f70 6f6c 6f67 792f 6164 645f   "/topology/add_
+00012c50: 646e 735f 7365 7276 6572 222c 0a20 2020  dns_server",.   
+00012c60: 2020 2020 2064 6174 613d 6461 7461 2c0a       data=data,.
+00012c70: 2020 2020 2020 2020 6865 6164 6572 733d          headers=
+00012c80: 7b22 436f 6e74 656e 742d 5479 7065 223a  {"Content-Type":
+00012c90: 2022 6170 706c 6963 6174 696f 6e2f 6a73   "application/js
+00012ca0: 6f6e 227d 2c0a 2020 2020 290a 0a20 2020  on"},.    )..   
+00012cb0: 2069 6620 7265 7375 6c74 2e73 7461 7475   if result.statu
+00012cc0: 735f 636f 6465 2021 3d20 3230 303a 0a20  s_code != 200:. 
+00012cd0: 2020 2020 2020 205f 6861 6e64 6c65 5f65         _handle_e
+00012ce0: 7272 6f72 2872 6573 756c 742c 2022 4572  rror(result, "Er
+00012cf0: 726f 7220 7768 696c 6520 6164 6469 6e67  ror while adding
+00012d00: 2061 2044 4e53 2073 6572 7665 7220 746f   a DNS server to
+00012d10: 2061 2074 6f70 6f6c 6f67 7922 290a 0a20   a topology").. 
+00012d20: 2020 2074 6f70 6f6c 6f67 795f 7961 6d6c     topology_yaml
+00012d30: 203d 2072 6573 756c 742e 6a73 6f6e 2829   = result.json()
+00012d40: 5b22 746f 706f 6c6f 6779 5f79 616d 6c22  ["topology_yaml"
+00012d50: 5d0a 2020 2020 646e 735f 636f 6e66 203d  ].    dns_conf =
+00012d60: 2072 6573 756c 742e 6a73 6f6e 2829 5b22   result.json()["
+00012d70: 646e 735f 636f 6e66 225d 0a0a 2020 2020  dns_conf"]..    
+00012d80: 7265 7475 726e 2074 6f70 6f6c 6f67 795f  return topology_
+00012d90: 7961 6d6c 2c20 646e 735f 636f 6e66 0a0a  yaml, dns_conf..
+00012da0: 0a64 6566 2074 6f6f 6c73 5f67 656e 6572  .def tools_gener
+00012db0: 6174 655f 646f 6d61 696e 7328 0a20 2020  ate_domains(.   
+00012dc0: 2061 6c67 6f72 6974 686d 3a20 7374 722c   algorithm: str,
+00012dd0: 0a20 2020 206e 756d 6265 723a 2069 6e74  .    number: int
+00012de0: 2c0a 2920 2d3e 204c 6973 745b 7374 725d  ,.) -> List[str]
+00012df0: 3a0a 2020 2020 2222 2247 656e 6572 6174  :.    """Generat
+00012e00: 6520 646f 6d61 696e 206e 616d 6573 2061  e domain names a
+00012e10: 6363 6f72 6469 6e67 2074 6f20 7468 6520  ccording to the 
+00012e20: 6769 7665 6e20 616c 676f 7269 7468 6d2e  given algorithm.
+00012e30: 0a0a 2020 2020 3a72 6574 7572 6e3a 2041  ..    :return: A
+00012e40: 206c 6973 7420 6f66 2064 6f6d 6169 6e73   list of domains
+00012e50: 2e0a 0a20 2020 203a 7061 7261 6d20 616c  ...    :param al
+00012e60: 676f 7269 7468 6d3a 2054 6865 2061 6c67  gorithm: The alg
+00012e70: 6f72 6974 686d 2075 7365 6420 746f 2067  orithm used to g
+00012e80: 656e 6572 6174 6520 7468 6520 6e65 7720  enerate the new 
+00012e90: 646f 6d61 696e 732e 0a20 2020 203a 7061  domains..    :pa
+00012ea0: 7261 6d20 6e75 6d62 6572 3a20 4e75 6d62  ram number: Numb
+00012eb0: 6572 206f 6620 646f 6d61 696e 7320 746f  er of domains to
+00012ec0: 2067 656e 6572 6174 652e 0a0a 2020 2020   generate...    
+00012ed0: 2222 220a 2020 2020 6461 7461 5f64 6963  """.    data_dic
+00012ee0: 7420 3d20 7b0a 2020 2020 2020 2020 2261  t = {.        "a
+00012ef0: 6c67 6f72 6974 686d 223a 2061 6c67 6f72  lgorithm": algor
+00012f00: 6974 686d 2c0a 2020 2020 2020 2020 226e  ithm,.        "n
+00012f10: 756d 6265 7222 3a20 6e75 6d62 6572 2c0a  umber": number,.
+00012f20: 2020 2020 7d0a 2020 2020 6461 7461 203d      }.    data =
+00012f30: 206a 736f 6e2e 6475 6d70 7328 6461 7461   json.dumps(data
+00012f40: 5f64 6963 7429 0a20 2020 2072 6573 756c  _dict).    resul
+00012f50: 7420 3d20 5f70 6f73 7428 0a20 2020 2020  t = _post(.     
+00012f60: 2020 2022 2f64 6f6d 6169 6e2f 6765 6e65     "/domain/gene
+00012f70: 7261 7465 5f64 6f6d 6169 6e73 222c 0a20  rate_domains",. 
+00012f80: 2020 2020 2020 2064 6174 613d 6461 7461         data=data
+00012f90: 2c0a 2020 2020 2020 2020 6865 6164 6572  ,.        header
+00012fa0: 733d 7b22 436f 6e74 656e 742d 5479 7065  s={"Content-Type
+00012fb0: 223a 2022 6170 706c 6963 6174 696f 6e2f  ": "application/
+00012fc0: 6a73 6f6e 227d 2c0a 2020 2020 290a 0a20  json"},.    ).. 
+00012fd0: 2020 2069 6620 7265 7375 6c74 2e73 7461     if result.sta
+00012fe0: 7475 735f 636f 6465 2021 3d20 3230 303a  tus_code != 200:
+00012ff0: 0a20 2020 2020 2020 205f 6861 6e64 6c65  .        _handle
+00013000: 5f65 7272 6f72 2872 6573 756c 742c 2022  _error(result, "
+00013010: 4572 726f 7220 7768 696c 6520 6765 6e65  Error while gene
+00013020: 7261 7469 6e67 2064 6f6d 6169 6e73 2229  rating domains")
+00013030: 0a0a 2020 2020 646f 6d61 696e 7320 3d20  ..    domains = 
+00013040: 7265 7375 6c74 2e6a 736f 6e28 295b 2264  result.json()["d
+00013050: 6f6d 6169 6e73 225d 0a0a 2020 2020 7265  omains"]..    re
+00013060: 7475 726e 2064 6f6d 6169 6e73 0a0a 0a64  turn domains...d
+00013070: 6566 2066 6574 6368 5f74 6f70 6f6c 6f67  ef fetch_topolog
+00013080: 6965 7328 2920 2d3e 2041 6e79 3a0a 2020  ies() -> Any:.  
+00013090: 2020 2222 2252 6574 7572 6e20 746f 706f    """Return topo
+000130a0: 6c6f 6769 6573 206c 6973 742e 0a0a 2020  logies list...  
+000130b0: 2020 3a72 6574 7572 6e3a 2054 6865 206c    :return: The l
+000130c0: 6973 7420 6f66 2061 7661 696c 6162 6c65  ist of available
+000130d0: 2074 6f70 6f6c 6f67 6965 732e 0a0a 2020   topologies...  
+000130e0: 2020 2222 220a 2020 2020 7265 7375 6c74    """.    result
+000130f0: 203d 205f 6765 7428 222f 746f 706f 6c6f   = _get("/topolo
+00013100: 6779 2229 0a0a 2020 2020 6966 2072 6573  gy")..    if res
+00013110: 756c 742e 7374 6174 7573 5f63 6f64 6520  ult.status_code 
+00013120: 213d 2032 3030 3a0a 2020 2020 2020 2020  != 200:.        
+00013130: 5f68 616e 646c 655f 6572 726f 7228 7265  _handle_error(re
+00013140: 7375 6c74 2c20 2243 616e 6e6f 7420 7265  sult, "Cannot re
+00013150: 7472 6965 7665 2074 6f70 6f6c 6f67 6965  trieve topologie
+00013160: 7320 6c69 7374 2066 726f 6d20 4954 2053  s list from IT S
+00013170: 696d 756c 6174 696f 6e20 4150 4922 290a  imulation API").
+00013180: 0a20 2020 2074 6f70 6f6c 6f67 6965 7320  .    topologies 
+00013190: 3d20 7265 7375 6c74 2e6a 736f 6e28 290a  = result.json().
+000131a0: 2020 2020 7265 7475 726e 2074 6f70 6f6c      return topol
+000131b0: 6f67 6965 730a 0a0a 2323 230a 2320 5369  ogies...###.# Si
+000131c0: 6d75 6c61 7469 6f6e 2063 6f6d 6d61 6e64  mulation command
+000131d0: 730a 2323 230a 0a0a 6465 6620 7374 6172  s.###...def star
+000131e0: 745f 7369 6d75 6c61 7469 6f6e 280a 2020  t_simulation(.  
+000131f0: 2020 6964 5f73 696d 756c 6174 696f 6e3a    id_simulation:
+00013200: 2069 6e74 2c0a 2020 2020 7573 655f 696e   int,.    use_in
+00013210: 7374 616c 6c5f 7469 6d65 3a20 626f 6f6c  stall_time: bool
+00013220: 203d 2046 616c 7365 2c0a 2020 2020 7469   = False,.    ti
+00013230: 6d65 6f75 743a 2069 6e74 203d 2033 3030  meout: int = 300
+00013240: 2c0a 2020 2020 6e6f 6465 733a 204f 7074  ,.    nodes: Opt
+00013250: 696f 6e61 6c5b 4c69 7374 5b73 7472 5d5d  ional[List[str]]
+00013260: 203d 204e 6f6e 652c 0a29 202d 3e20 4e6f   = None,.) -> No
+00013270: 6e65 3a0a 2020 2020 2222 2253 7461 7274  ne:.    """Start
+00013280: 2074 6865 2073 696d 756c 6174 696f 6e2c   the simulation,
+00013290: 2077 6974 6820 6375 7272 656e 7420 7469   with current ti
+000132a0: 6d65 2028 6279 2064 6566 6175 6c74 2920  me (by default) 
+000132b0: 6f72 2074 696d 6520 7768 6572 650a 2020  or time where.  
+000132c0: 2020 7468 6520 564d 2077 6173 2063 7265    the VM was cre
+000132d0: 6174 6564 2028 7573 655f 696e 7374 616c  ated (use_instal
+000132e0: 6c5f 7469 6d65 3d54 7275 6529 2e20 4974  l_time=True). It
+000132f0: 2069 7320 706f 7373 6962 6c65 2074 6f0a   is possible to.
+00013300: 2020 2020 7370 6563 6966 7920 7468 6520      specify the 
+00013310: 6e6f 6465 7320 746f 2073 7461 7274 2e20  nodes to start. 
+00013320: 4279 2064 6566 6175 6c74 2c20 616c 6c20  By default, all 
+00013330: 6e6f 6465 7320 6172 6520 7374 6172 7465  nodes are starte
+00013340: 642e 0a0a 2020 2020 3a70 6172 616d 2069  d...    :param i
+00013350: 645f 7369 6d75 6c61 7469 6f6e 3a20 5468  d_simulation: Th
+00013360: 6520 7369 6d75 6c61 7469 6f6e 2049 442e  e simulation ID.
+00013370: 0a20 2020 203a 7061 7261 6d20 7573 655f  .    :param use_
+00013380: 696e 7374 616c 6c5f 7469 6d65 3a20 5465  install_time: Te
+00013390: 6c6c 2074 6f20 7374 6172 7420 7468 6520  ll to start the 
+000133a0: 7669 7274 7561 6c20 6d61 6368 696e 6573  virtual machines
+000133b0: 2077 6974 6820 7468 6520 6375 7272 656e   with the curren
+000133c0: 7420 7469 6d65 206f 7220 746f 2075 7365  t time or to use
+000133d0: 2074 6865 2069 6e73 7461 6c6c 6174 696f   the installatio
+000133e0: 6e20 7469 6d65 206f 6620 7468 6520 6173  n time of the as
+000133f0: 736f 6369 6174 6564 2062 6173 6562 6f78  sociated basebox
+00013400: 6573 2e20 4279 2064 6566 6175 6c74 2028  es. By default (
+00013410: 5472 7565 292c 2074 6865 2063 7572 7265  True), the curre
+00013420: 6e74 2068 6f73 7420 7379 7374 656d 2074  nt host system t
+00013430: 696d 6520 6973 2075 7365 6420 666f 7220  ime is used for 
+00013440: 7468 6520 6375 7272 656e 7420 7469 6d65  the current time
+00013450: 2e0a 2020 2020 3a70 6172 616d 2074 696d  ..    :param tim
+00013460: 656f 7574 3a20 4279 2064 6566 6175 6c74  eout: By default
+00013470: 2c20 6120 3330 3020 7365 636f 6e64 7320  , a 300 seconds 
+00013480: 7469 6d65 6f75 7420 6973 2075 7365 6420  timeout is used 
+00013490: 746f 206c 696d 6974 2074 6865 2061 6d6f  to limit the amo
+000134a0: 756e 7420 6f66 2074 696d 6520 7765 2077  unt of time we w
+000134b0: 6169 7420 666f 7220 7468 6520 6e6f 6465  ait for the node
+000134c0: 7320 746f 2066 696e 6973 6820 746f 2073  s to finish to s
+000134d0: 7461 7274 2e20 5468 6973 2064 656c 6179  tart. This delay
+000134e0: 2063 616e 2062 6520 6368 616e 6765 642e   can be changed.
+000134f0: 0a20 2020 203a 7061 7261 6d20 6e6f 6465  .    :param node
+00013500: 733a 2054 6865 206e 6f64 6573 2074 6f20  s: The nodes to 
+00013510: 7374 6172 7420 2861 6c6c 206e 6f64 6573  start (all nodes
+00013520: 2062 7920 6465 6661 756c 7429 2e0a 0a20   by default)... 
+00013530: 2020 2022 2222 0a20 2020 2023 2043 6865     """.    # Che
+00013540: 636b 2074 6861 7420 6e6f 206f 7468 6572  ck that no other
+00013550: 2073 696d 756c 6174 696f 6e20 6973 2072   simulation is r
+00013560: 756e 6e69 6e67 0a20 2020 2073 696d 756c  unning.    simul
+00013570: 6174 696f 6e5f 6c69 7374 203d 2066 6574  ation_list = fet
+00013580: 6368 5f73 696d 756c 6174 696f 6e73 2829  ch_simulations()
+00013590: 0a20 2020 2066 6f72 2073 696d 756c 6174  .    for simulat
+000135a0: 696f 6e20 696e 2073 696d 756c 6174 696f  ion in simulatio
+000135b0: 6e5f 6c69 7374 3a0a 2020 2020 2020 2020  n_list:.        
+000135c0: 6966 2073 696d 756c 6174 696f 6e5b 2269  if simulation["i
+000135d0: 6422 5d20 213d 2069 645f 7369 6d75 6c61  d"] != id_simula
+000135e0: 7469 6f6e 2061 6e64 2073 696d 756c 6174  tion and simulat
+000135f0: 696f 6e5b 2273 7461 7475 7322 5d20 3d3d  ion["status"] ==
+00013600: 2022 5255 4e4e 494e 4722 3a0a 2020 2020   "RUNNING":.    
+00013610: 2020 2020 2020 2020 7261 6973 6520 4578          raise Ex
+00013620: 6365 7074 696f 6e28 0a20 2020 2020 2020  ception(.       
+00013630: 2020 2020 2020 2020 2022 4361 6e6e 6f74           "Cannot
+00013640: 2073 7461 7274 2061 206e 6577 2073 696d   start a new sim
+00013650: 756c 6174 696f 6e2c 2061 7320 7468 6520  ulation, as the 
+00013660: 7369 6d75 6c61 7469 6f6e 2027 7b7d 2720  simulation '{}' 
+00013670: 6973 2022 0a20 2020 2020 2020 2020 2020  is ".           
+00013680: 2020 2020 2022 616c 7265 6164 7920 7275       "already ru
+00013690: 6e6e 696e 6722 2e66 6f72 6d61 7428 7369  nning".format(si
+000136a0: 6d75 6c61 7469 6f6e 5b22 6964 225d 290a  mulation["id"]).
+000136b0: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+000136c0: 2020 2023 2049 6e69 7469 6174 6520 7468     # Initiate th
+000136d0: 6520 7369 6d75 6c61 7469 6f6e 0a20 2020  e simulation.   
+000136e0: 2069 6620 6e6f 6465 7320 6973 204e 6f6e   if nodes is Non
+000136f0: 653a 0a20 2020 2020 2020 206e 6f64 6573  e:.        nodes
+00013700: 203d 205b 5d0a 2020 2020 706f 7374 5f64   = [].    post_d
+00013710: 6174 6120 3d20 7b22 6e6f 6465 7322 3a20  ata = {"nodes": 
+00013720: 6e6f 6465 737d 0a0a 2020 2020 5f73 696d  nodes}..    _sim
+00013730: 756c 6174 696f 6e5f 6578 6563 7574 655f  ulation_execute_
+00013740: 6f70 6572 6174 696f 6e28 0a20 2020 2020  operation(.     
+00013750: 2020 2022 706f 7374 222c 0a20 2020 2020     "post",.     
+00013760: 2020 2022 7374 6172 7422 2c0a 2020 2020     "start",.    
+00013770: 2020 2020 6964 5f73 696d 756c 6174 696f      id_simulatio
+00013780: 6e2c 0a20 2020 2020 2020 2022 5354 4152  n,.        "STAR
+00013790: 5449 4e47 222c 0a20 2020 2020 2020 206f  TING",.        o
+000137a0: 7074 696f 6e61 6c5f 7061 7261 6d31 3d75  ptional_param1=u
+000137b0: 7365 5f69 6e73 7461 6c6c 5f74 696d 652c  se_install_time,
+000137c0: 0a20 2020 2020 2020 206f 7074 696f 6e61  .        optiona
+000137d0: 6c5f 7061 7261 6d32 3d74 696d 656f 7574  l_param2=timeout
+000137e0: 2c0a 2020 2020 2020 2020 706f 7374 5f64  ,.        post_d
+000137f0: 6174 613d 706f 7374 5f64 6174 612c 0a20  ata=post_data,. 
+00013800: 2020 2029 0a0a 0a64 6566 2070 6175 7365     )...def pause
+00013810: 5f73 696d 756c 6174 696f 6e28 6964 5f73  _simulation(id_s
+00013820: 696d 756c 6174 696f 6e3a 2069 6e74 2920  imulation: int) 
+00013830: 2d3e 204e 6f6e 653a 0a20 2020 2022 2222  -> None:.    """
+00013840: 5061 7573 6520 6120 7369 6d75 6c61 7469  Pause a simulati
+00013850: 6f6e 2028 6361 6c6c 7320 6c69 6276 6972  on (calls libvir
+00013860: 7420 7375 7370 656e 6420 4150 4929 2e0a  t suspend API)..
 00013870: 0a20 2020 203a 7061 7261 6d20 6964 5f73  .    :param id_s
-00013880: 696d 756c 6174 696f 6e3a 2054 6865 2069  imulation: The i
-00013890: 6420 6f66 2074 6865 2073 696d 756c 6174  d of the simulat
-000138a0: 696f 6e0a 0a20 2020 203a 7479 7065 2069  ion..    :type i
-000138b0: 645f 7369 6d75 6c61 7469 6f6e 3a20 3a63  d_simulation: :c
-000138c0: 6c61 7373 3a60 696e 7460 2c20 6578 203a  lass:`int`, ex :
-000138d0: 2031 0a0a 2020 2020 3a72 6574 7572 6e3a   1..    :return:
-000138e0: 2041 206c 6973 7420 6f66 2070 726f 6265   A list of probe
-000138f0: 7320 7769 7468 2074 6865 6972 2064 6174  s with their dat
-00013900: 610a 2020 2020 2222 220a 0a20 2020 2072  a.    """..    r
-00013910: 6573 756c 7420 3d20 7b7d 0a0a 2020 2020  esult = {}..    
-00013920: 7072 6f62 6573 203d 2066 6574 6368 5f70  probes = fetch_p
-00013930: 726f 6265 7328 6964 5f73 696d 756c 6174  robes(id_simulat
-00013940: 696f 6e29 0a20 2020 2066 6f72 2070 726f  ion).    for pro
-00013950: 6265 2069 6e20 7072 6f62 6573 3a0a 2020  be in probes:.  
-00013960: 2020 2020 2020 7265 7375 6c74 5b70 726f        result[pro
-00013970: 6265 5b22 6964 225d 5d20 3d20 7b0a 2020  be["id"]] = {.  
-00013980: 2020 2020 2020 2020 2020 2263 6f6c 6c65            "colle
-00013990: 6374 696e 675f 706f 696e 7473 223a 2066  cting_points": f
-000139a0: 6574 6368 5f70 726f 6265 5f63 6f6c 6c65  etch_probe_colle
-000139b0: 6374 696e 675f 706f 696e 7473 2869 645f  cting_points(id_
-000139c0: 7369 6d75 6c61 7469 6f6e 2c20 7072 6f62  simulation, prob
-000139d0: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
-000139e0: 2269 6661 6365 223a 2070 726f 6265 5b22  "iface": probe["
-000139f0: 6966 6163 6522 5d2c 0a20 2020 2020 2020  iface"],.       
-00013a00: 2020 2020 2022 7063 6170 223a 2070 726f       "pcap": pro
-00013a10: 6265 5b22 7063 6170 225d 2c0a 2020 2020  be["pcap"],.    
-00013a20: 2020 2020 2020 2020 2266 696c 7465 7222          "filter"
-00013a30: 3a20 7072 6f62 655b 2266 696c 7465 7222  : probe["filter"
-00013a40: 5d2c 0a20 2020 2020 2020 2020 2020 2022  ],.            "
-00013a50: 6361 7074 7572 655f 696e 5f70 726f 6772  capture_in_progr
-00013a60: 6573 7322 3a20 7072 6f62 655b 2263 6170  ess": probe["cap
-00013a70: 7475 7265 5f69 6e5f 7072 6f67 7265 7373  ture_in_progress
-00013a80: 225d 2c0a 2020 2020 2020 2020 2020 2020  "],.            
-00013a90: 2264 6972 6563 7469 6f6e 223a 2070 726f  "direction": pro
-00013aa0: 6265 5b22 6469 7265 6374 696f 6e22 5d2c  be["direction"],
-00013ab0: 0a20 2020 2020 2020 207d 0a0a 2020 2020  .        }..    
-00013ac0: 7265 7475 726e 2072 6573 756c 740a 0a0a  return result...
-00013ad0: 6465 6620 6665 7463 685f 7072 6f62 655f  def fetch_probe_
-00013ae0: 636f 6c6c 6563 7469 6e67 5f70 6f69 6e74  collecting_point
-00013af0: 7328 6964 5f73 696d 756c 6174 696f 6e3a  s(id_simulation:
-00013b00: 2069 6e74 2c20 7072 6f62 653a 2044 6963   int, probe: Dic
-00013b10: 7429 202d 3e20 416e 793a 0a20 2020 2022  t) -> Any:.    "
-00013b20: 2222 5265 7475 726e 2074 6865 206c 6973  ""Return the lis
-00013b30: 7420 6f66 2063 6f6c 6c65 6374 696e 6720  t of collecting 
-00013b40: 706f 696e 7473 2075 7365 6420 746f 2063  points used to c
-00013b50: 6170 7475 7265 2074 6865 206e 6574 776f  apture the netwo
-00013b60: 726b 2074 7261 6666 6963 2074 6f20 6120  rk traffic to a 
-00013b70: 6769 7665 6e20 7072 6f62 6520 6f66 2061  given probe of a
-00013b80: 2073 696d 756c 6174 696f 6e2e 0a0a 2020   simulation...  
-00013b90: 2020 3a70 6172 616d 2069 645f 7369 6d75    :param id_simu
-00013ba0: 6c61 7469 6f6e 3a20 5468 6520 6964 206f  lation: The id o
-00013bb0: 6620 7468 6520 7369 6d75 6c61 7469 6f6e  f the simulation
-00013bc0: 2e0a 2020 2020 3a70 6172 616d 2070 726f  ..    :param pro
-00013bd0: 6265 3a20 5468 6520 6769 7665 6e20 7072  be: The given pr
-00013be0: 6f62 6520 6f66 2074 6865 2073 696d 756c  obe of the simul
-00013bf0: 6174 696f 6e0a 0a20 2020 203a 7479 7065  ation..    :type
-00013c00: 2069 645f 7369 6d75 6c61 7469 6f6e 3a20   id_simulation: 
-00013c10: 3a63 6c61 7373 3a60 696e 7460 2c20 6578  :class:`int`, ex
-00013c20: 203a 2031 0a20 2020 203a 7479 7065 2070   : 1.    :type p
-00013c30: 726f 6265 3a20 3a63 6c61 7373 3a60 636c  robe: :class:`cl
-00013c40: 6173 7360 3a60 4469 6374 602c 2065 7820  ass`:`Dict`, ex 
-00013c50: 3a20 7b27 6966 6163 6527 3a20 2764 756d  : {'iface': 'dum
-00013c60: 6d79 3027 2c20 2769 6427 3a20 312c 2027  my0', 'id': 1, '
-00013c70: 7063 6170 273a 2054 7275 652c 2027 6361  pcap': True, 'ca
-00013c80: 7074 7572 655f 696e 5f70 726f 6772 6573  pture_in_progres
-00013c90: 7327 3a20 4661 6c73 652c 2027 6669 6c74  s': False, 'filt
-00013ca0: 6572 273a 2027 7463 7020 706f 7274 2038  er': 'tcp port 8
-00013cb0: 3027 2c20 2773 696d 756c 6174 696f 6e5f  0', 'simulation_
-00013cc0: 6964 273a 2031 2c20 276e 6574 776f 726b  id': 1, 'network
-00013cd0: 5f69 6e74 6572 6661 6365 7327 3a20 5b27  _interfaces': ['
-00013ce0: 3030 3a32 313a 6131 3a30 373a 3764 3a62  00:21:a1:07:7d:b
-00013cf0: 6527 5d2c 2027 6469 7265 6374 696f 6e27  e'], 'direction'
-00013d00: 3a20 2769 6e67 7265 7373 277d 0a0a 2020  : 'ingress'}..  
-00013d10: 2020 2222 220a 0a20 2020 2063 6f6c 6c65    """..    colle
-00013d20: 6374 696e 675f 706f 696e 7473 203d 207b  cting_points = {
-00013d30: 2273 7769 7463 6873 223a 207b 7d2c 2022  "switchs": {}, "
-00013d40: 6e6f 6465 7322 3a20 5b5d 7d0a 0a20 2020  nodes": []}..   
-00013d50: 206e 6574 776f 726b 5f69 6e74 6572 6661   network_interfa
-00013d60: 6365 7320 3d20 5b0a 2020 2020 2020 2020  ces = [.        
-00013d70: 6665 7463 685f 6e65 7477 6f72 6b5f 696e  fetch_network_in
-00013d80: 7465 7266 6163 655f 6279 5f6d 6163 2869  terface_by_mac(i
-00013d90: 645f 7369 6d75 6c61 7469 6f6e 2c20 6e29  d_simulation, n)
-00013da0: 0a20 2020 2020 2020 2066 6f72 206e 2069  .        for n i
-00013db0: 6e20 7072 6f62 655b 226e 6574 776f 726b  n probe["network
-00013dc0: 5f69 6e74 6572 6661 6365 7322 5d0a 2020  _interfaces"].  
-00013dd0: 2020 5d0a 0a20 2020 206e 6f64 6573 5f74    ]..    nodes_t
-00013de0: 6f5f 6361 7074 7572 6520 3d20 5b5d 0a20  o_capture = []. 
-00013df0: 2020 2066 6f72 206e 6574 776f 726b 5f69     for network_i
-00013e00: 6e74 6572 6661 6365 2069 6e20 6e65 7477  nterface in netw
-00013e10: 6f72 6b5f 696e 7465 7266 6163 6573 3a0a  ork_interfaces:.
-00013e20: 2020 2020 2020 2020 6e6f 6465 203d 2066          node = f
-00013e30: 6574 6368 5f6e 6f64 6528 6e65 7477 6f72  etch_node(networ
-00013e40: 6b5f 696e 7465 7266 6163 655b 226e 6f64  k_interface["nod
-00013e50: 655f 6964 225d 290a 2020 2020 2020 2020  e_id"]).        
-00013e60: 6966 206e 6f64 6520 6e6f 7420 696e 206e  if node not in n
-00013e70: 6f64 6573 5f74 6f5f 6361 7074 7572 653a  odes_to_capture:
-00013e80: 0a20 2020 2020 2020 2020 2020 206e 6f64  .            nod
-00013e90: 6573 5f74 6f5f 6361 7074 7572 652e 6170  es_to_capture.ap
-00013ea0: 7065 6e64 286e 6f64 6529 0a0a 2020 2020  pend(node)..    
-00013eb0: 2320 5265 7475 726e 204e 6f6e 6520 6966  # Return None if
-00013ec0: 2074 6865 7265 2069 7320 6e6f 7468 696e   there is nothin
-00013ed0: 6720 746f 2063 6170 7475 7265 0a20 2020  g to capture.   
-00013ee0: 2069 6620 6e6f 6465 735f 746f 5f63 6170   if nodes_to_cap
-00013ef0: 7475 7265 203d 3d20 5b5d 3a0a 2020 2020  ture == []:.    
-00013f00: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
-00013f10: 0a20 2020 2023 2052 6574 7572 6e20 7b7d  .    # Return {}
-00013f20: 2069 6620 6576 6572 7920 6e6f 6465 206d   if every node m
-00013f30: 7573 7420 6265 2063 6170 7475 7265 640a  ust be captured.
-00013f40: 2020 2020 6966 206c 656e 286e 6574 776f      if len(netwo
-00013f50: 726b 5f69 6e74 6572 6661 6365 7329 203d  rk_interfaces) =
-00013f60: 3d20 6c65 6e28 0a20 2020 2020 2020 2066  = len(.        f
-00013f70: 6574 6368 5f73 696d 756c 6174 696f 6e5f  etch_simulation_
-00013f80: 6e65 7477 6f72 6b5f 696e 7465 7266 6163  network_interfac
-00013f90: 6573 2869 645f 7369 6d75 6c61 7469 6f6e  es(id_simulation
-00013fa0: 290a 2020 2020 293a 0a20 2020 2020 2020  ).    ):.       
-00013fb0: 2072 6574 7572 6e20 7b7d 0a0a 2020 2020   return {}..    
-00013fc0: 666f 7220 6e6f 6465 2069 6e20 6e6f 6465  for node in node
-00013fd0: 735f 746f 5f63 6170 7475 7265 3a0a 2020  s_to_capture:.  
-00013fe0: 2020 2020 2020 2320 4966 2065 7665 7279        # If every
-00013ff0: 206e 6574 776f 726b 5f69 6e74 6572 6661   network_interfa
-00014000: 6365 2066 726f 6d20 6120 6e6f 6465 2069  ce from a node i
-00014010: 7320 6361 7074 7572 6564 2c20 6974 2067  s captured, it g
-00014020: 6f65 7320 746f 2074 6865 2022 6e6f 6465  oes to the "node
-00014030: 7322 2064 6963 740a 2020 2020 2020 2020  s" dict.        
-00014040: 6361 7074 7572 655f 616c 6c5f 6e65 7477  capture_all_netw
-00014050: 6f72 6b5f 696e 7465 7266 6163 6573 203d  ork_interfaces =
-00014060: 2054 7275 650a 2020 2020 2020 2020 666f   True.        fo
-00014070: 7220 6e6f 6465 5f6e 6574 776f 726b 5f69  r node_network_i
-00014080: 6e74 6572 6661 6365 2069 6e20 6e6f 6465  nterface in node
-00014090: 5b22 6e65 7477 6f72 6b5f 696e 7465 7266  ["network_interf
-000140a0: 6163 6573 225d 3a0a 2020 2020 2020 2020  aces"]:.        
-000140b0: 2020 2020 6361 7074 7572 655f 616c 6c5f      capture_all_
-000140c0: 6e65 7477 6f72 6b5f 696e 7465 7266 6163  network_interfac
-000140d0: 6573 203d 2063 6170 7475 7265 5f61 6c6c  es = capture_all
-000140e0: 5f6e 6574 776f 726b 5f69 6e74 6572 6661  _network_interfa
-000140f0: 6365 7320 616e 6420 280a 2020 2020 2020  ces and (.      
-00014100: 2020 2020 2020 2020 2020 6e6f 6465 5f6e            node_n
-00014110: 6574 776f 726b 5f69 6e74 6572 6661 6365  etwork_interface
-00014120: 2069 6e20 6e65 7477 6f72 6b5f 696e 7465   in network_inte
-00014130: 7266 6163 6573 0a20 2020 2020 2020 2020  rfaces.         
-00014140: 2020 2029 0a0a 2020 2020 2020 2020 6966     )..        if
-00014150: 2063 6170 7475 7265 5f61 6c6c 5f6e 6574   capture_all_net
-00014160: 776f 726b 5f69 6e74 6572 6661 6365 733a  work_interfaces:
-00014170: 0a20 2020 2020 2020 2020 2020 2063 6f6c  .            col
-00014180: 6c65 6374 696e 675f 706f 696e 7473 5b22  lecting_points["
-00014190: 6e6f 6465 7322 5d2e 6170 7065 6e64 286e  nodes"].append(n
-000141a0: 6f64 655b 226e 616d 6522 5d29 0a20 2020  ode["name"]).   
-000141b0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-000141c0: 2020 2020 2020 2023 2045 6c73 652c 2069         # Else, i
-000141d0: 7420 676f 6573 2074 6f20 7468 6520 2273  t goes to the "s
-000141e0: 7769 7463 6873 2220 6469 6374 0a20 2020  witchs" dict.   
-000141f0: 2020 2020 2020 2020 2066 6f72 206e 6f64           for nod
-00014200: 655f 6e65 7477 6f72 6b5f 696e 7465 7266  e_network_interf
-00014210: 6163 6520 696e 206e 6f64 655b 226e 6574  ace in node["net
-00014220: 776f 726b 5f69 6e74 6572 6661 6365 7322  work_interfaces"
-00014230: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
-00014240: 2020 2069 6620 6e6f 6465 5f6e 6574 776f     if node_netwo
-00014250: 726b 5f69 6e74 6572 6661 6365 2069 6e20  rk_interface in 
-00014260: 6e65 7477 6f72 6b5f 696e 7465 7266 6163  network_interfac
-00014270: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
-00014280: 2020 2020 2020 2020 7377 6974 6368 203d          switch =
-00014290: 207b 226e 616d 6522 3a20 6e6f 6465 5f6e   {"name": node_n
-000142a0: 6574 776f 726b 5f69 6e74 6572 6661 6365  etwork_interface
-000142b0: 5b22 7377 6974 6368 5f6e 616d 6522 5d7d  ["switch_name"]}
-000142c0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000142d0: 2020 2020 2020 6966 2073 7769 7463 685b        if switch[
-000142e0: 226e 616d 6522 5d20 6e6f 7420 696e 2063  "name"] not in c
-000142f0: 6f6c 6c65 6374 696e 675f 706f 696e 7473  ollecting_points
-00014300: 5b22 7377 6974 6368 7322 5d2e 6b65 7973  ["switchs"].keys
-00014310: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00014320: 2020 2020 2020 2020 2020 2020 636f 6c6c              coll
-00014330: 6563 7469 6e67 5f70 6f69 6e74 735b 2273  ecting_points["s
-00014340: 7769 7463 6873 225d 5b73 7769 7463 685b  witchs"][switch[
-00014350: 226e 616d 6522 5d5d 203d 205b 5d0a 2020  "name"]] = [].  
-00014360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014370: 2020 636f 6c6c 6563 7469 6e67 5f70 6f69    collecting_poi
-00014380: 6e74 735b 2273 7769 7463 6873 225d 5b73  nts["switchs"][s
-00014390: 7769 7463 685b 226e 616d 6522 5d5d 2e61  witch["name"]].a
-000143a0: 7070 656e 6428 6e6f 6465 5b22 6e61 6d65  ppend(node["name
-000143b0: 225d 290a 0a20 2020 2072 6574 7572 6e20  "])..    return 
-000143c0: 636f 6c6c 6563 7469 6e67 5f70 6f69 6e74  collecting_point
-000143d0: 730a 0a0a 6465 6620 736e 6170 7368 6f74  s...def snapshot
-000143e0: 5f73 696d 756c 6174 696f 6e28 6964 5f73  _simulation(id_s
-000143f0: 696d 756c 6174 696f 6e3a 2069 6e74 2920  imulation: int) 
-00014400: 2d3e 2073 7472 3a0a 2020 2020 2222 2243  -> str:.    """C
-00014410: 7265 6174 6520 6120 736e 6170 7368 6f74  reate a snapshot
-00014420: 206f 6620 6120 7369 6d75 6c61 7469 6f6e   of a simulation
-00014430: 2e0a 0a20 2020 2041 6c6c 2074 6865 2066  ...    All the f
-00014440: 696c 6573 2077 696c 6c20 6265 2073 746f  iles will be sto
-00014450: 7265 6420 746f 0a20 2020 202f 6379 6265  red to.    /cybe
-00014460: 722d 7261 6e67 652d 6361 7461 6c6f 672f  r-range-catalog/
-00014470: 7369 6d75 6c61 7469 6f6e 732f 3c68 6173  simulations/<has
-00014480: 6820 6361 6d70 6169 676e 3e2f 3c74 696d  h campaign>/<tim
-00014490: 6573 7461 6d70 3e2f 0a0a 2020 2020 5468  estamp>/..    Th
-000144a0: 6973 2041 5049 2063 616c 6c20 7265 7475  is API call retu
-000144b0: 726e 7320 7468 6520 7061 7468 2077 6865  rns the path whe
-000144c0: 7265 2074 6865 2074 6f70 6f6c 6f67 7920  re the topology 
-000144d0: 6669 6c65 2077 696c 6c20 6265 2073 746f  file will be sto
-000144e0: 7265 642e 0a0a 2020 2020 5061 7261 6d65  red...    Parame
-000144f0: 7465 7273 3a0a 0a20 2020 2069 645f 7369  ters:..    id_si
-00014500: 6d75 6c61 7469 6f6e 3a20 696e 740a 2020  mulation: int.  
-00014510: 2020 2020 2020 5369 6d75 6c61 7469 6f6e        Simulation
-00014520: 2074 6f20 736e 6170 7368 6f74 0a0a 2020   to snapshot..  
-00014530: 2020 2222 220a 0a20 2020 2023 2073 696d    """..    # sim
-00014540: 755f 736e 6170 2063 616e 206f 6e6c 7920  u_snap can only 
-00014550: 6265 2064 6f6e 6520 6f6e 2061 2052 554e  be done on a RUN
-00014560: 4e49 4e47 2073 696d 756c 6174 696f 6e0a  NING simulation.
-00014570: 2020 2020 6966 2073 696d 756c 6174 696f      if simulatio
-00014580: 6e5f 7374 6174 7573 2869 645f 7369 6d75  n_status(id_simu
-00014590: 6c61 7469 6f6e 2920 213d 2022 5255 4e4e  lation) != "RUNN
-000145a0: 494e 4722 3a0a 2020 2020 2020 2020 7261  ING":.        ra
-000145b0: 6973 6520 4578 6365 7074 696f 6e28 0a20  ise Exception(. 
-000145c0: 2020 2020 2020 2020 2020 2022 4361 6e6e             "Cann
-000145d0: 6f74 2063 7265 6174 6520 6120 736e 6170  ot create a snap
-000145e0: 7368 6f74 206f 6620 7468 6520 7369 6d75  shot of the simu
-000145f0: 6c61 7469 6f6e 2c20 6173 2074 6865 2073  lation, as the s
-00014600: 696d 756c 6174 696f 6e20 277b 7d27 2069  imulation '{}' i
-00014610: 7320 220a 2020 2020 2020 2020 2020 2020  s ".            
-00014620: 226e 6f74 2072 756e 6e69 6e67 222e 666f  "not running".fo
-00014630: 726d 6174 2869 645f 7369 6d75 6c61 7469  rmat(id_simulati
-00014640: 6f6e 290a 2020 2020 2020 2020 290a 0a20  on).        ).. 
-00014650: 2020 2023 2043 616c 6c20 736e 6170 7368     # Call snapsh
-00014660: 6f74 2041 5049 0a20 2020 2072 6573 756c  ot API.    resul
-00014670: 7420 3d20 5f70 6f73 7428 6622 2f73 696d  t = _post(f"/sim
-00014680: 756c 6174 696f 6e2f 7b69 645f 7369 6d75  ulation/{id_simu
-00014690: 6c61 7469 6f6e 7d2f 736e 6170 7368 6f74  lation}/snapshot
-000146a0: 2229 0a20 2020 2069 6620 7265 7375 6c74  ").    if result
-000146b0: 2e73 7461 7475 735f 636f 6465 2021 3d20  .status_code != 
-000146c0: 3230 303a 0a20 2020 2020 2020 205f 6861  200:.        _ha
-000146d0: 6e64 6c65 5f65 7272 6f72 2872 6573 756c  ndle_error(resul
-000146e0: 742c 2022 4572 726f 7220 7768 696c 6520  t, "Error while 
-000146f0: 6372 6561 7469 6e67 2073 6e61 7073 686f  creating snapsho
-00014700: 7422 290a 0a20 2020 2079 616d 6c3a 2073  t")..    yaml: s
-00014710: 7472 203d 2072 6573 756c 742e 6a73 6f6e  tr = result.json
-00014720: 2829 0a0a 2020 2020 6c6f 6767 6572 2e69  ()..    logger.i
-00014730: 6e66 6f28 6622 5b2b 5d20 5374 6172 7469  nfo(f"[+] Starti
-00014740: 6e67 2074 6865 2073 6e61 7073 686f 7420  ng the snapshot 
-00014750: 6f66 2073 696d 756c 6174 696f 6e20 7b69  of simulation {i
-00014760: 645f 7369 6d75 6c61 7469 6f6e 7d2e 2e2e  d_simulation}...
-00014770: 2229 0a20 2020 2077 6869 6c65 2073 696d  ").    while sim
-00014780: 756c 6174 696f 6e5f 7374 6174 7573 2869  ulation_status(i
-00014790: 645f 7369 6d75 6c61 7469 6f6e 2920 213d  d_simulation) !=
-000147a0: 2022 534e 4150 5348 4f54 223a 0a20 2020   "SNAPSHOT":.   
-000147b0: 2020 2020 2074 696d 652e 736c 6565 7028       time.sleep(
-000147c0: 3129 0a0a 2020 2020 2020 2020 7369 6d75  1)..        simu
-000147d0: 6c61 7469 6f6e 5f64 6963 7420 3d20 6665  lation_dict = fe
-000147e0: 7463 685f 7369 6d75 6c61 7469 6f6e 2869  tch_simulation(i
-000147f0: 645f 7369 6d75 6c61 7469 6f6e 290a 2020  d_simulation).  
-00014800: 2020 2020 2020 6375 7272 656e 745f 7374        current_st
-00014810: 6174 7573 203d 2073 696d 756c 6174 696f  atus = simulatio
-00014820: 6e5f 6469 6374 5b22 7374 6174 7573 225d  n_dict["status"]
-00014830: 0a20 2020 2020 2020 2069 6620 6375 7272  .        if curr
-00014840: 656e 745f 7374 6174 7573 203d 3d20 2245  ent_status == "E
-00014850: 5252 4f52 223a 0a20 2020 2020 2020 2020  RROR":.         
-00014860: 2020 2065 7272 6f72 5f6d 6573 7361 6765     error_message
-00014870: 203d 2073 696d 756c 6174 696f 6e5f 6469   = simulation_di
-00014880: 6374 5b22 6572 726f 725f 6d73 6722 5d0a  ct["error_msg"].
-00014890: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-000148a0: 6520 4578 6365 7074 696f 6e28 0a20 2020  e Exception(.   
-000148b0: 2020 2020 2020 2020 2020 2020 2022 4572               "Er
-000148c0: 726f 7220 6475 7269 6e67 2073 696d 756c  ror during simul
-000148d0: 6174 696f 6e20 736e 6170 7368 6f74 3a20  ation snapshot: 
-000148e0: 277b 7d27 222e 666f 726d 6174 2865 7272  '{}'".format(err
-000148f0: 6f72 5f6d 6573 7361 6765 290a 2020 2020  or_message).    
-00014900: 2020 2020 2020 2020 290a 0a20 2020 206c          )..    l
-00014910: 6f67 6765 722e 696e 666f 2822 5b2b 5d20  ogger.info("[+] 
-00014920: 536e 6170 7368 6f74 2070 726f 6365 7373  Snapshot process
-00014930: 2068 6173 2073 7461 7274 6564 2229 0a0a   has started")..
-00014940: 2020 2020 7768 696c 6520 7369 6d75 6c61      while simula
-00014950: 7469 6f6e 5f73 7461 7475 7328 6964 5f73  tion_status(id_s
-00014960: 696d 756c 6174 696f 6e29 2021 3d20 2252  imulation) != "R
-00014970: 4541 4459 223a 0a20 2020 2020 2020 206c  EADY":.        l
-00014980: 6f67 6765 722e 696e 666f 2822 2020 5b2b  ogger.info("  [+
-00014990: 5d20 536e 6170 7368 6f74 2069 6e20 7072  ] Snapshot in pr
-000149a0: 6f67 7265 7373 2e2e 2e22 290a 2020 2020  ogress...").    
-000149b0: 2020 2020 7469 6d65 2e73 6c65 6570 2831      time.sleep(1
-000149c0: 290a 0a20 2020 2020 2020 2073 696d 756c  )..        simul
-000149d0: 6174 696f 6e5f 6469 6374 203d 2066 6574  ation_dict = fet
-000149e0: 6368 5f73 696d 756c 6174 696f 6e28 6964  ch_simulation(id
-000149f0: 5f73 696d 756c 6174 696f 6e29 0a20 2020  _simulation).   
-00014a00: 2020 2020 2063 7572 7265 6e74 5f73 7461       current_sta
-00014a10: 7475 7320 3d20 7369 6d75 6c61 7469 6f6e  tus = simulation
-00014a20: 5f64 6963 745b 2273 7461 7475 7322 5d0a  _dict["status"].
-00014a30: 2020 2020 2020 2020 6966 2063 7572 7265          if curre
-00014a40: 6e74 5f73 7461 7475 7320 3d3d 2022 4552  nt_status == "ER
-00014a50: 524f 5222 3a0a 2020 2020 2020 2020 2020  ROR":.          
-00014a60: 2020 6572 726f 725f 6d65 7373 6167 6520    error_message 
-00014a70: 3d20 7369 6d75 6c61 7469 6f6e 5f64 6963  = simulation_dic
-00014a80: 745b 2265 7272 6f72 5f6d 7367 225d 0a20  t["error_msg"]. 
-00014a90: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00014aa0: 2045 7863 6570 7469 6f6e 280a 2020 2020   Exception(.    
-00014ab0: 2020 2020 2020 2020 2020 2020 2245 7272              "Err
-00014ac0: 6f72 2064 7572 696e 6720 7369 6d75 6c61  or during simula
-00014ad0: 7469 6f6e 2073 6e61 7073 686f 743a 2027  tion snapshot: '
-00014ae0: 7b7d 2722 2e66 6f72 6d61 7428 6572 726f  {}'".format(erro
-00014af0: 725f 6d65 7373 6167 6529 0a20 2020 2020  r_message).     
-00014b00: 2020 2020 2020 2029 0a0a 2020 2020 7265         )..    re
-00014b10: 7475 726e 2079 616d 6c0a 0a0a 6465 6620  turn yaml...def 
-00014b20: 636f 6d70 7574 655f 696e 6672 6173 7472  compute_infrastr
-00014b30: 7563 7475 7265 5f73 7461 7475 7328 2920  ucture_status() 
-00014b40: 2d3e 2041 6e79 3a0a 2020 2020 2222 2247  -> Any:.    """G
-00014b50: 6574 2076 6972 7463 6c69 656e 7420 7365  et virtclient se
-00014b60: 7276 6963 6520 7374 6174 7573 2e22 2222  rvice status."""
-00014b70: 0a20 2020 2072 6573 756c 7420 3d20 5f67  .    result = _g
-00014b80: 6574 2822 2f73 696d 756c 6174 696f 6e2f  et("/simulation/
-00014b90: 636f 6d70 7574 655f 696e 6672 6173 7472  compute_infrastr
-00014ba0: 7563 7475 7265 5f73 7461 7475 7322 290a  ucture_status").
-00014bb0: 0a20 2020 2069 6620 7265 7375 6c74 2e73  .    if result.s
-00014bc0: 7461 7475 735f 636f 6465 2021 3d20 3230  tatus_code != 20
-00014bd0: 303a 0a20 2020 2020 2020 205f 6861 6e64  0:.        _hand
-00014be0: 6c65 5f65 7272 6f72 2872 6573 756c 742c  le_error(result,
-00014bf0: 2022 4361 6e6e 6f74 2067 6574 2063 6f6d   "Cannot get com
-00014c00: 7075 7465 2069 6e66 7261 7374 7275 6374  pute infrastruct
-00014c10: 7572 6520 7374 6174 7573 2229 0a0a 2020  ure status")..  
-00014c20: 2020 7369 6d75 6c61 7469 6f6e 5f64 6963    simulation_dic
-00014c30: 7420 3d20 7265 7375 6c74 2e6a 736f 6e28  t = result.json(
-00014c40: 290a 2020 2020 7265 7475 726e 2073 696d  ).    return sim
-00014c50: 756c 6174 696f 6e5f 6469 6374 0a0a 0a64  ulation_dict...d
-00014c60: 6566 2061 6464 5f64 6e73 5f65 6e74 7269  ef add_dns_entri
-00014c70: 6573 2869 645f 7369 6d75 6c61 7469 6f6e  es(id_simulation
-00014c80: 3a20 696e 742c 2064 6e73 5f65 6e74 7269  : int, dns_entri
-00014c90: 6573 3a20 4469 6374 5b73 7472 2c20 7374  es: Dict[str, st
-00014ca0: 725d 2920 2d3e 2073 7472 3a0a 2020 2020  r]) -> str:.    
-00014cb0: 2222 2241 6464 2076 6f6c 6174 696c 6520  """Add volatile 
-00014cc0: 444e 5320 656e 7472 6965 7320 746f 2074  DNS entries to t
-00014cd0: 6865 2063 7572 7265 6e74 2073 696d 756c  he current simul
-00014ce0: 6174 696f 6e2e 2056 6f6c 6174 696c 6520  ation. Volatile 
-00014cf0: 6d65 616e 7320 7468 6174 2069 7420 6973  means that it is
-00014d00: 206e 6f74 0a20 2020 2073 746f 7265 6420   not.    stored 
-00014d10: 696e 2064 6174 6162 6173 652e 0a0a 2020  in database...  
-00014d20: 2020 2222 220a 0a20 2020 2064 6174 6120    """..    data 
-00014d30: 3d20 6a73 6f6e 2e64 756d 7073 2864 6e73  = json.dumps(dns
-00014d40: 5f65 6e74 7269 6573 290a 2020 2020 7265  _entries).    re
-00014d50: 7375 6c74 203d 205f 706f 7374 280a 2020  sult = _post(.  
-00014d60: 2020 2020 2020 6622 2f73 696d 756c 6174        f"/simulat
-00014d70: 696f 6e2f 7b69 645f 7369 6d75 6c61 7469  ion/{id_simulati
-00014d80: 6f6e 7d2f 6164 645f 646e 735f 656e 7472  on}/add_dns_entr
-00014d90: 6965 7322 2c0a 2020 2020 2020 2020 6461  ies",.        da
-00014da0: 7461 3d64 6174 612c 0a20 2020 2020 2020  ta=data,.       
-00014db0: 2068 6561 6465 7273 3d7b 2243 6f6e 7465   headers={"Conte
-00014dc0: 6e74 2d54 7970 6522 3a20 2261 7070 6c69  nt-Type": "appli
-00014dd0: 6361 7469 6f6e 2f6a 736f 6e22 7d2c 0a20  cation/json"},. 
-00014de0: 2020 2029 0a0a 2020 2020 6966 2072 6573     )..    if res
-00014df0: 756c 742e 7374 6174 7573 5f63 6f64 6520  ult.status_code 
-00014e00: 213d 2032 3030 3a0a 2020 2020 2020 2020  != 200:.        
-00014e10: 5f68 616e 646c 655f 6572 726f 7228 7265  _handle_error(re
-00014e20: 7375 6c74 2c20 2245 7272 6f72 2077 6869  sult, "Error whi
-00014e30: 6c65 2061 6464 696e 6720 444e 5320 656e  le adding DNS en
-00014e40: 7472 6965 7322 290a 0a0a 6465 6620 636f  tries")...def co
-00014e50: 6e6e 6563 745f 686f 7374 2869 645f 7369  nnect_host(id_si
-00014e60: 6d75 6c61 7469 6f6e 3a20 696e 7429 202d  mulation: int) -
-00014e70: 3e20 4e6f 6e65 3a0a 2020 2020 2222 2243  > None:.    """C
-00014e80: 6f6e 6e65 6374 2074 6865 2068 6f73 7420  onnect the host 
-00014e90: 696e 7465 7266 6163 6520 746f 2074 6865  interface to the
-00014ea0: 2063 7572 7265 6e74 2073 696d 756c 6174   current simulat
-00014eb0: 696f 6e2e 2222 220a 0a20 2020 2072 6573  ion."""..    res
-00014ec0: 756c 7420 3d20 5f67 6574 2866 222f 7369  ult = _get(f"/si
-00014ed0: 6d75 6c61 7469 6f6e 2f7b 6964 5f73 696d  mulation/{id_sim
-00014ee0: 756c 6174 696f 6e7d 2f63 6f6e 6e65 6374  ulation}/connect
-00014ef0: 5f68 6f73 7422 290a 0a20 2020 2069 6620  _host")..    if 
-00014f00: 7265 7375 6c74 2e73 7461 7475 735f 636f  result.status_co
-00014f10: 6465 2021 3d20 3230 303a 0a20 2020 2020  de != 200:.     
-00014f20: 2020 205f 6861 6e64 6c65 5f65 7272 6f72     _handle_error
-00014f30: 280a 2020 2020 2020 2020 2020 2020 7265  (.            re
-00014f40: 7375 6c74 2c0a 2020 2020 2020 2020 2020  sult,.          
-00014f50: 2020 6622 4361 6e6e 6f74 2065 7865 6375    f"Cannot execu
-00014f60: 7465 206f 7065 7261 7469 6f6e 2027 636f  te operation 'co
-00014f70: 6e6e 6563 745f 686f 7374 2720 6f6e 2073  nnect_host' on s
-00014f80: 696d 756c 6174 696f 6e20 277b 6964 5f73  imulation '{id_s
-00014f90: 696d 756c 6174 696f 6e7d 272e 222c 0a20  imulation}'.",. 
-00014fa0: 2020 2020 2020 2029 0a0a 0a64 6566 2064         )...def d
-00014fb0: 6973 636f 6e6e 6563 745f 686f 7374 2869  isconnect_host(i
-00014fc0: 645f 7369 6d75 6c61 7469 6f6e 3a20 696e  d_simulation: in
-00014fd0: 7429 202d 3e20 4e6f 6e65 3a0a 2020 2020  t) -> None:.    
-00014fe0: 2222 2244 6973 636f 6e6e 6563 7420 7468  """Disconnect th
-00014ff0: 6520 686f 7374 2069 6e74 6572 6661 6365  e host interface
-00015000: 2074 6f20 7468 6520 6375 7272 656e 7420   to the current 
-00015010: 7369 6d75 6c61 7469 6f6e 2e22 2222 0a0a  simulation."""..
-00015020: 2020 2020 7265 7375 6c74 203d 205f 6765      result = _ge
-00015030: 7428 6622 2f73 696d 756c 6174 696f 6e2f  t(f"/simulation/
-00015040: 7b69 645f 7369 6d75 6c61 7469 6f6e 7d2f  {id_simulation}/
-00015050: 6469 7363 6f6e 6e65 6374 5f68 6f73 7422  disconnect_host"
-00015060: 290a 0a20 2020 2069 6620 7265 7375 6c74  )..    if result
-00015070: 2e73 7461 7475 735f 636f 6465 2021 3d20  .status_code != 
-00015080: 3230 303a 0a20 2020 2020 2020 205f 6861  200:.        _ha
-00015090: 6e64 6c65 5f65 7272 6f72 280a 2020 2020  ndle_error(.    
-000150a0: 2020 2020 2020 2020 7265 7375 6c74 2c0a          result,.
-000150b0: 2020 2020 2020 2020 2020 2020 6622 4361              f"Ca
-000150c0: 6e6e 6f74 2065 7865 6375 7465 206f 7065  nnot execute ope
-000150d0: 7261 7469 6f6e 2027 6469 7363 6f6e 6e65  ration 'disconne
-000150e0: 6374 5f68 6f73 7427 206f 6e20 7369 6d75  ct_host' on simu
-000150f0: 6c61 7469 6f6e 2027 7b69 645f 7369 6d75  lation '{id_simu
-00015100: 6c61 7469 6f6e 7d27 2e22 2c0a 2020 2020  lation}'.",.    
-00015110: 2020 2020 290a 0a0a 6465 6620 6765 6e65      )...def gene
-00015120: 7261 7465 5f6d 616c 6963 696f 7573 5f64  rate_malicious_d
-00015130: 6f6d 6169 6e73 2861 6c67 6f72 6974 686d  omains(algorithm
-00015140: 3a20 7374 7220 3d20 4e6f 6e65 2c20 6e75  : str = None, nu
-00015150: 6d62 6572 3a20 696e 7420 3d20 3129 202d  mber: int = 1) -
-00015160: 3e20 4c69 7374 5b73 7472 5d3a 0a20 2020  > List[str]:.   
-00015170: 2022 2222 4765 6e65 7261 7465 2061 6e64   """Generate and
-00015180: 2072 6574 7572 6e20 6120 6c69 7374 206f   return a list o
-00015190: 6620 6d61 6c69 6369 6f75 7320 646f 6d61  f malicious doma
-000151a0: 696e 732e 2222 220a 0a20 2020 2064 6174  ins."""..    dat
-000151b0: 615f 6469 6374 203d 207b 0a20 2020 2020  a_dict = {.     
-000151c0: 2020 2022 616c 676f 7269 7468 6d22 3a20     "algorithm": 
-000151d0: 616c 676f 7269 7468 6d2c 0a20 2020 2020  algorithm,.     
-000151e0: 2020 2022 6e75 6d62 6572 223a 206e 756d     "number": num
-000151f0: 6265 722c 0a20 2020 207d 0a20 2020 2064  ber,.    }.    d
-00015200: 6174 6120 3d20 6a73 6f6e 2e64 756d 7073  ata = json.dumps
-00015210: 2864 6174 615f 6469 6374 290a 0a20 2020  (data_dict)..   
-00015220: 2072 6573 756c 7420 3d20 5f70 6f73 7428   result = _post(
-00015230: 0a20 2020 2020 2020 2022 2f74 6f70 6f6c  .        "/topol
-00015240: 6f67 792f 6765 6e65 7261 7465 5f6d 616c  ogy/generate_mal
-00015250: 6963 696f 7573 5f64 6f6d 6169 6e73 222c  icious_domains",
-00015260: 0a20 2020 2020 2020 2064 6174 613d 6461  .        data=da
-00015270: 7461 2c0a 2020 2020 2020 2020 6865 6164  ta,.        head
-00015280: 6572 733d 7b22 436f 6e74 656e 742d 5479  ers={"Content-Ty
-00015290: 7065 223a 2022 6170 706c 6963 6174 696f  pe": "applicatio
-000152a0: 6e2f 6a73 6f6e 227d 2c0a 2020 2020 290a  n/json"},.    ).
-000152b0: 0a20 2020 2069 6620 7265 7375 6c74 2e73  .    if result.s
-000152c0: 7461 7475 735f 636f 6465 2021 3d20 3230  tatus_code != 20
-000152d0: 303a 0a20 2020 2020 2020 205f 6861 6e64  0:.        _hand
-000152e0: 6c65 5f65 7272 6f72 2872 6573 756c 742c  le_error(result,
-000152f0: 2022 4572 726f 7220 7768 696c 6520 6164   "Error while ad
-00015300: 6469 6e67 2044 4e53 2065 6e74 7269 6573  ding DNS entries
-00015310: 2229 0a0a 2020 2020 646f 6d61 696e 7320  ")..    domains 
-00015320: 3d20 7265 7375 6c74 2e6a 736f 6e28 290a  = result.json().
-00015330: 2020 2020 7265 7475 726e 2064 6f6d 6169      return domai
-00015340: 6e73 5b22 646f 6d61 696e 7322 5d0a 0a0a  ns["domains"]...
-00015350: 6465 6620 6372 6561 7465 5f64 6174 6173  def create_datas
-00015360: 6574 280a 2020 2020 6964 5f73 696d 756c  et(.    id_simul
-00015370: 6174 696f 6e3a 2069 6e74 2c20 646f 6e74  ation: int, dont
-00015380: 5f63 6865 636b 5f6c 6f67 735f 7061 7468  _check_logs_path
-00015390: 3a20 626f 6f6c 203d 2046 616c 7365 0a29  : bool = False.)
-000153a0: 202d 3e20 4f70 7469 6f6e 616c 5b75 7569   -> Optional[uui
-000153b0: 642e 5555 4944 5d3a 0a20 2020 2022 2222  d.UUID]:.    """
-000153c0: 0a20 2020 2048 616e 646c 6573 2074 6865  .    Handles the
-000153d0: 2063 7265 6174 696f 6e20 6f66 2074 6865   creation of the
-000153e0: 2064 6174 6173 6574 2061 6674 6572 2074   dataset after t
-000153f0: 6865 2065 6e64 206f 6620 6120 7369 6d75  he end of a simu
-00015400: 6c61 7469 6f6e 0a0a 2020 2020 4d75 7374  lation..    Must
-00015410: 2062 6520 6361 6c6c 6564 2061 6674 6572   be called after
-00015420: 2061 2053 544f 5020 6f70 6572 6174 696f   a STOP operatio
-00015430: 6e2c 2061 6e64 206f 6e63 6520 616c 6c20  n, and once all 
-00015440: 636f 6d70 7574 6520 7365 7276 6572 730a  compute servers.
-00015450: 2020 2020 2876 6972 7463 6c69 656e 7429      (virtclient)
-00015460: 2068 6176 6520 6675 6c6c 7920 7374 6f70   have fully stop
-00015470: 7065 642e 0a0a 2020 2020 4261 7369 6361  ped...    Basica
-00015480: 6c6c 792c 2074 6869 7320 6675 6e63 7469  lly, this functi
-00015490: 6f6e 2063 6f6d 6d75 6e69 6361 7465 7320  on communicates 
-000154a0: 7769 7468 2074 6865 2074 6865 2063 6f72  with the the cor
-000154b0: 6520 4150 492c 2077 6869 6368 2069 7473  e API, which its
-000154c0: 656c 660a 2020 2020 636f 6d6d 756e 6963  elf.    communic
-000154d0: 6174 6573 2077 6974 6820 7468 6520 7075  ates with the pu
-000154e0: 626c 6973 6820 7365 7276 6572 2773 2022  blish server's "
-000154f0: 6261 636b 656e 6422 2041 5049 2e0a 0a20  backend" API... 
-00015500: 2020 203a 7061 7261 6d20 6964 5f73 696d     :param id_sim
-00015510: 756c 6174 696f 6e3a 2074 6865 2073 696d  ulation: the sim
-00015520: 756c 6174 696f 6e20 7768 6963 6820 7761  ulation which wa
-00015530: 7320 6a75 7374 2073 746f 7070 6564 2061  s just stopped a
-00015540: 6e64 2066 726f 6d20 7768 6963 6820 6f75  nd from which ou
-00015550: 7470 7574 2074 6865 2064 6174 6173 6574  tput the dataset
-00015560: 2073 686f 756c 6420 6265 2063 7265 6174   should be creat
-00015570: 6564 0a20 2020 203a 7265 7475 726e 3a20  ed.    :return: 
-00015580: 7468 6520 6e65 7720 6461 7461 7365 7420  the new dataset 
-00015590: 6964 0a20 2020 2022 2222 0a0a 2020 2020  id.    """..    
-000155a0: 6c6f 6767 6572 2e69 6e66 6f28 0a20 2020  logger.info(.   
-000155b0: 2020 2020 2022 5b2b 5d20 476f 696e 6720       "[+] Going 
-000155c0: 746f 2063 7265 6174 6520 6461 7461 7365  to create datase
-000155d0: 7420 6261 7365 6420 6f6e 2064 6174 6120  t based on data 
-000155e0: 7072 6f64 7563 6564 2062 7920 7369 6d75  produced by simu
-000155f0: 6c61 7469 6f6e 2049 4420 277b 7d27 222e  lation ID '{}'".
-00015600: 666f 726d 6174 280a 2020 2020 2020 2020  format(.        
-00015610: 2020 2020 6964 5f73 696d 756c 6174 696f      id_simulatio
-00015620: 6e0a 2020 2020 2020 2020 290a 2020 2020  n.        ).    
-00015630: 290a 0a20 2020 2069 6620 646f 6e74 5f63  )..    if dont_c
-00015640: 6865 636b 5f6c 6f67 735f 7061 7468 2069  heck_logs_path i
-00015650: 7320 4661 6c73 653a 0a20 2020 2020 2020  s False:.       
-00015660: 2069 6620 5f63 6865 636b 5f6c 6f67 735f   if _check_logs_
-00015670: 7061 7468 2869 645f 7369 6d75 6c61 7469  path(id_simulati
-00015680: 6f6e 293a 0a20 2020 2020 2020 2020 2020  on):.           
-00015690: 2072 6574 7572 6e20 4e6f 6e65 0a0a 2020   return None..  
-000156a0: 2020 2320 4173 6b20 7468 6520 636f 7265    # Ask the core
-000156b0: 2041 5049 2074 6f20 636f 6e74 6163 7420   API to contact 
-000156c0: 7468 6520 2f62 6163 6b65 6e64 2f20 7075  the /backend/ pu
-000156d0: 626c 6973 6820 7365 7276 6572 2041 5049  blish server API
-000156e0: 0a20 2020 2023 2069 6e20 6f72 6465 7220  .    # in order 
-000156f0: 746f 2073 7461 7274 2074 6865 2064 6174  to start the dat
-00015700: 6173 6574 2063 7265 6174 696f 6e20 7072  aset creation pr
-00015710: 6f63 6573 730a 2020 2020 7265 7375 6c74  ocess.    result
-00015720: 203d 205f 706f 7374 2866 222f 6372 6561   = _post(f"/crea
-00015730: 7465 5f64 6174 6173 6574 2f7b 6964 5f73  te_dataset/{id_s
-00015740: 696d 756c 6174 696f 6e7d 2229 0a20 2020  imulation}").   
-00015750: 2069 6620 7265 7375 6c74 2e73 7461 7475   if result.statu
-00015760: 735f 636f 6465 2021 3d20 3230 303a 0a20  s_code != 200:. 
-00015770: 2020 2020 2020 205f 6861 6e64 6c65 5f65         _handle_e
-00015780: 7272 6f72 2872 6573 756c 742c 2022 4361  rror(result, "Ca
-00015790: 6e6e 6f74 2069 6e69 7469 6174 6520 7468  nnot initiate th
-000157a0: 6520 6372 6561 7469 6f6e 206f 6620 7468  e creation of th
-000157b0: 6520 6461 7461 7365 7422 290a 0a20 2020  e dataset")..   
-000157c0: 2064 6174 6173 6574 5f69 6420 3d20 7265   dataset_id = re
-000157d0: 7375 6c74 2e6a 736f 6e28 295b 2264 6174  sult.json()["dat
-000157e0: 6173 6574 5f69 6422 5d0a 0a20 2020 206c  aset_id"]..    l
-000157f0: 6f67 6765 722e 696e 666f 2866 2220 205b  ogger.info(f"  [
-00015800: 2b5d 2044 6174 6173 6574 2070 7265 2d63  +] Dataset pre-c
-00015810: 7265 6174 6564 2077 6974 6820 6461 7461  reated with data
-00015820: 7365 7420 6964 207b 6461 7461 7365 745f  set id {dataset_
-00015830: 6964 7d22 290a 0a20 2020 2023 2053 7461  id}")..    # Sta
-00015840: 7274 2061 6e20 6163 7469 7665 2077 6169  rt an active wai
-00015850: 7469 6e67 206c 6f6f 7020 756e 7469 6c20  ting loop until 
-00015860: 7468 6520 6461 7461 7365 7420 6372 6561  the dataset crea
-00015870: 7469 6f6e 2069 6620 6675 6c6c 7920 636f  tion if fully co
-00015880: 6d70 6c65 7465 0a20 2020 2023 2049 6e64  mplete.    # Ind
-00015890: 6565 642c 2064 6174 6173 6574 2063 7265  eed, dataset cre
-000158a0: 6174 696f 6e20 696e 766f 6c76 6573 2074  ation involves t
-000158b0: 6865 2064 6f77 6e6c 6f61 6420 6f66 2070  he download of p
-000158c0: 6f74 656e 7469 616c 6c79 206c 6172 6765  otentially large
-000158d0: 0a20 2020 2023 2066 696c 6573 206f 7665  .    # files ove
-000158e0: 7273 2074 6865 206e 6574 776f 726b 2c20  rs the network, 
-000158f0: 7768 6963 6820 6361 6e20 7461 6b65 2073  which can take s
-00015900: 6f6d 6520 7469 6d65 210a 2020 2020 6d61  ome time!.    ma
-00015910: 785f 7265 7472 6965 7320 3d20 350a 2020  x_retries = 5.  
-00015920: 2020 7265 7472 6965 7320 3d20 6d61 785f    retries = max_
-00015930: 7265 7472 6965 730a 2020 2020 7768 696c  retries.    whil
-00015940: 6520 5472 7565 3a0a 2020 2020 2020 2020  e True:.        
-00015950: 7469 6d65 2e73 6c65 6570 2832 290a 0a20  time.sleep(2).. 
-00015960: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-00015970: 5f67 6574 2866 222f 6372 6561 7465 5f64  _get(f"/create_d
-00015980: 6174 6173 6574 2f73 7461 7475 732f 7b64  ataset/status/{d
-00015990: 6174 6173 6574 5f69 647d 2229 0a20 2020  ataset_id}").   
-000159a0: 2020 2020 2069 6620 7265 7375 6c74 2e73       if result.s
-000159b0: 7461 7475 735f 636f 6465 2021 3d20 3230  tatus_code != 20
-000159c0: 303a 0a20 2020 2020 2020 2020 2020 2069  0:.            i
-000159d0: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
-000159e0: 2020 2020 7265 7375 6c74 2e68 6561 6465      result.heade
-000159f0: 7273 2e67 6574 2822 636f 6e74 656e 742d  rs.get("content-
-00015a00: 7479 7065 2229 203d 3d20 2261 7070 6c69  type") == "appli
-00015a10: 6361 7469 6f6e 2f6a 736f 6e22 0a20 2020  cation/json".   
-00015a20: 2020 2020 2020 2020 2020 2020 2061 6e64               and
-00015a30: 2022 6d65 7373 6167 6522 2069 6e20 7265   "message" in re
-00015a40: 7375 6c74 2e6a 736f 6e28 290a 2020 2020  sult.json().    
-00015a50: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
-00015a60: 2020 2020 2020 2020 2020 2065 7272 6f72             error
-00015a70: 5f6d 7367 203d 2072 6573 756c 742e 6a73  _msg = result.js
-00015a80: 6f6e 2829 5b22 6d65 7373 6167 6522 5d0a  on()["message"].
-00015a90: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00015aa0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00015ab0: 2020 6572 726f 725f 6d73 6720 3d20 7265    error_msg = re
-00015ac0: 7375 6c74 2e74 6578 740a 0a20 2020 2020  sult.text..     
-00015ad0: 2020 2020 2020 2023 2052 6574 7279 2074         # Retry t
-00015ae0: 6f20 6765 7420 7468 6520 7374 6174 7573  o get the status
-00015af0: 2061 2063 6f75 706c 6520 6f66 2074 696d   a couple of tim
-00015b00: 6573 2062 6566 6f72 6520 7173 656e 6469  es before qsendi
-00015b10: 6e67 2062 6163 6b20 616e 2065 7272 6f72  ng back an error
-00015b20: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00015b30: 7265 7472 6965 7320 3d3d 2030 3a0a 2020  retries == 0:.  
-00015b40: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-00015b50: 6973 6520 4578 6365 7074 696f 6e28 0a20  ise Exception(. 
-00015b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015b70: 2020 2022 4572 726f 7220 6475 7269 6e67     "Error during
-00015b80: 2063 7265 6174 696f 6e20 6f66 2064 6174   creation of dat
-00015b90: 6173 6574 207b 7d3a 2063 6f75 6c64 206e  aset {}: could n
-00015ba0: 6f74 2067 6574 2073 7461 7475 7320 6f66  ot get status of
-00015bb0: 2074 6865 2064 6174 6173 6574 2063 7265   the dataset cre
-00015bc0: 6174 696f 6e20 6166 7465 7220 7b7d 2074  ation after {} t
-00015bd0: 7269 6573 2e20 436f 7265 2041 5049 2048  ries. Core API H
-00015be0: 5454 5020 7374 6174 7573 3a20 7b7d 2e20  TTP status: {}. 
-00015bf0: 5265 7370 6f6e 7365 3a20 7b7d 2022 2e66  Response: {} ".f
-00015c00: 6f72 6d61 7428 0a20 2020 2020 2020 2020  ormat(.         
-00015c10: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00015c20: 6174 6173 6574 5f69 642c 206d 6178 5f72  ataset_id, max_r
-00015c30: 6574 7269 6573 2c20 7265 7375 6c74 2e73  etries, result.s
-00015c40: 7461 7475 735f 636f 6465 2c20 6572 726f  tatus_code, erro
-00015c50: 725f 6d73 670a 2020 2020 2020 2020 2020  r_msg.          
-00015c60: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00015c70: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00015c80: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00015c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015ca0: 6c6f 6767 6572 2e77 6172 6e69 6e67 280a  logger.warning(.
-00015cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015cc0: 2020 2020 2220 205b 2b5d 2043 6f75 6c64      "  [+] Could
-00015cd0: 206e 6f74 2067 6574 2073 7461 7475 7320   not get status 
-00015ce0: 6f66 2064 6174 6173 6574 2063 7265 6174  of dataset creat
-00015cf0: 696f 6e20 2852 6574 7269 6573 206c 6566  ion (Retries lef
-00015d00: 743a 207b 7d2e 2043 6f72 6520 4150 4920  t: {}. Core API 
-00015d10: 4854 5450 2073 7461 7475 733a 207b 7d2e  HTTP status: {}.
-00015d20: 2052 6573 706f 6e73 653a 207b 7d29 222e   Response: {})".
-00015d30: 666f 726d 6174 280a 2020 2020 2020 2020  format(.        
-00015d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015d50: 7265 7472 6965 732c 2072 6573 756c 742e  retries, result.
-00015d60: 7374 6174 7573 5f63 6f64 652c 2065 7272  status_code, err
-00015d70: 6f72 5f6d 7367 0a20 2020 2020 2020 2020  or_msg.         
-00015d80: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00015d90: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00015da0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00015db0: 6574 7269 6573 202d 3d20 310a 2020 2020  etries -= 1.    
-00015dc0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00015dd0: 2020 2020 2020 2320 5265 7365 7420 7468        # Reset th
-00015de0: 6520 6e75 6d62 6572 206f 6620 7265 7472  e number of retr
-00015df0: 6965 730a 2020 2020 2020 2020 2020 2020  ies.            
-00015e00: 7265 7472 6965 7320 3d20 6d61 785f 7265  retries = max_re
-00015e10: 7472 6965 730a 0a20 2020 2020 2020 2020  tries..         
-00015e20: 2020 2023 2047 6574 2074 6865 2073 7461     # Get the sta
-00015e30: 7475 7320 616e 6420 6d65 7373 6167 650a  tus and message.
-00015e40: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00015e50: 7365 745f 6372 6561 7469 6f6e 5f73 7461  set_creation_sta
-00015e60: 7475 7320 3d20 7265 7375 6c74 2e6a 736f  tus = result.jso
-00015e70: 6e28 295b 2273 7461 7475 7322 5d0a 2020  n()["status"].  
-00015e80: 2020 2020 2020 2020 2020 6461 7461 7365            datase
-00015e90: 745f 6372 6561 7469 6f6e 5f6d 6573 7361  t_creation_messa
-00015ea0: 6765 203d 2072 6573 756c 742e 6a73 6f6e  ge = result.json
-00015eb0: 2829 5b22 6d65 7373 6167 6522 5d0a 0a20  ()["message"].. 
-00015ec0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-00015ed0: 722e 696e 666f 280a 2020 2020 2020 2020  r.info(.        
-00015ee0: 2020 2020 2020 2020 2220 205b 2b5d 2044          "  [+] D
-00015ef0: 6174 6173 6574 2063 7265 6174 696f 6e20  ataset creation 
-00015f00: 696e 2070 726f 6772 6573 7320 2853 7461  in progress (Sta
-00015f10: 7475 733a 207b 7d29 222e 666f 726d 6174  tus: {})".format
-00015f20: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00015f30: 2020 2020 2020 6461 7461 7365 745f 6372        dataset_cr
-00015f40: 6561 7469 6f6e 5f73 7461 7475 730a 2020  eation_status.  
-00015f50: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00015f60: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-00015f70: 2020 2020 2020 2020 2020 2069 6620 6461             if da
-00015f80: 7461 7365 745f 6372 6561 7469 6f6e 5f73  taset_creation_s
-00015f90: 7461 7475 7320 3d3d 2022 4649 4e49 5348  tatus == "FINISH
-00015fa0: 4544 223a 0a20 2020 2020 2020 2020 2020  ED":.           
-00015fb0: 2020 2020 2023 2041 6c6c 2077 656e 7420       # All went 
-00015fc0: 7765 6c6c 0a20 2020 2020 2020 2020 2020  well.           
-00015fd0: 2020 2020 2062 7265 616b 0a20 2020 2020       break.     
-00015fe0: 2020 2020 2020 2065 6c69 6620 6461 7461         elif data
-00015ff0: 7365 745f 6372 6561 7469 6f6e 5f73 7461  set_creation_sta
-00016000: 7475 7320 3d3d 2022 4649 4e49 5348 4544  tus == "FINISHED
-00016010: 5f45 5252 4f52 223a 0a20 2020 2020 2020  _ERROR":.       
-00016020: 2020 2020 2020 2020 2023 2054 6865 2064           # The d
-00016030: 6174 6173 6574 2063 7265 6174 696f 6e20  ataset creation 
-00016040: 656e 636f 756e 7465 7265 6420 6572 726f  encountered erro
-00016050: 7273 0a20 2020 2020 2020 2020 2020 2020  rs.             
-00016060: 2020 2072 6169 7365 2045 7863 6570 7469     raise Excepti
-00016070: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
-00016080: 2020 2020 2020 2020 2245 7272 6f72 2064          "Error d
-00016090: 7572 696e 6720 6372 6561 7469 6f6e 206f  uring creation o
-000160a0: 6620 6461 7461 7365 7420 7b7d 3a20 6461  f dataset {}: da
-000160b0: 7461 7365 7420 6372 6561 7469 6f6e 2065  taset creation e
-000160c0: 6e64 6564 2077 6974 6820 6572 726f 7273  nded with errors
-000160d0: 2028 277b 7d27 292e 222e 666f 726d 6174   ('{}').".format
-000160e0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000160f0: 2020 2020 2020 2020 2020 6461 7461 7365            datase
-00016100: 745f 6964 2c20 6461 7461 7365 745f 6372  t_id, dataset_cr
-00016110: 6561 7469 6f6e 5f6d 6573 7361 6765 0a20  eation_message. 
-00016120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016130: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00016140: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00016150: 2020 2023 204f 7468 6572 7769 7365 2c20     # Otherwise, 
-00016160: 6461 7461 7365 7420 6372 6561 7469 6f6e  dataset creation
-00016170: 2069 7320 6e6f 7420 6669 6e69 7368 6564   is not finished
-00016180: 2c20 6a75 7374 206c 6f6f 700a 0a20 2020  , just loop..   
-00016190: 206c 6f67 6765 722e 696e 666f 2822 5b2b   logger.info("[+
-000161a0: 5d20 4461 7461 7365 7420 6372 6561 7469  ] Dataset creati
-000161b0: 6f6e 2077 6173 2063 6f72 7265 6374 6c79  on was correctly
-000161c0: 2065 7865 6375 7465 6422 290a 0a20 2020   executed")..   
-000161d0: 2023 2053 6574 2074 6865 2073 696d 756c   # Set the simul
-000161e0: 6174 696f 6e20 7374 6174 7573 2074 6f20  ation status to 
-000161f0: 5245 4144 590a 2020 2020 7570 6461 7465  READY.    update
-00016200: 5f73 696d 756c 6174 696f 6e28 6964 5f73  _simulation(id_s
-00016210: 696d 756c 6174 696f 6e2c 207b 2273 7461  imulation, {"sta
-00016220: 7475 7322 3a20 2252 4541 4459 227d 290a  tus": "READY"}).
-00016230: 0a20 2020 2073 696d 756c 6174 696f 6e20  .    simulation 
-00016240: 3d20 6665 7463 685f 7369 6d75 6c61 7469  = fetch_simulati
-00016250: 6f6e 2869 645f 7369 6d75 6c61 7469 6f6e  on(id_simulation
-00016260: 290a 2020 2020 6c6f 6767 6572 2e69 6e66  ).    logger.inf
-00016270: 6f28 225b 2b5d 2043 7572 7265 6e74 2073  o("[+] Current s
-00016280: 696d 756c 6174 696f 6e20 7374 6174 7573  imulation status
-00016290: 3a20 277b 7d27 222e 666f 726d 6174 2873  : '{}'".format(s
-000162a0: 696d 756c 6174 696f 6e5b 2273 7461 7475  imulation["statu
-000162b0: 7322 5d29 290a 0a20 2020 2072 6574 7572  s"]))..    retur
-000162c0: 6e20 7575 6964 2e55 5549 4428 6461 7461  n uuid.UUID(data
-000162d0: 7365 745f 6964 290a 0a0a 6465 6620 5f63  set_id)...def _c
-000162e0: 6865 636b 5f6c 6f67 735f 7061 7468 2869  heck_logs_path(i
-000162f0: 645f 7369 6d75 6c61 7469 6f6e 3a20 696e  d_simulation: in
-00016300: 7429 202d 3e20 626f 6f6c 3a0a 2020 2020  t) -> bool:.    
-00016310: 2222 220a 2020 2020 5265 7475 726e 2074  """.    Return t
-00016320: 7275 6520 6966 2061 2062 6164 2070 6174  rue if a bad pat
-00016330: 6820 7761 7320 7365 7420 666f 7220 7468  h was set for th
-00016340: 6520 7273 7973 6c6f 6727 7320 6c6f 6720  e rsyslog's log 
-00016350: 766f 6c75 6d65 0a0a 2020 2020 446f 2061  volume..    Do a
-00016360: 2073 6d61 6c6c 2063 6865 636b 2066 6f72   small check for
-00016370: 2074 6865 2073 616b 6520 6f66 2068 656c   the sake of hel
-00016380: 7069 6e67 2074 6865 2075 7365 7220 616e  ping the user an
-00016390: 6420 6769 7669 6e67 2062 6574 7465 720a  d giving better.
-000163a0: 2020 2020 7573 6572 2065 7870 6572 6965      user experie
-000163b0: 6e63 653a 2063 6865 636b 2069 6620 7468  nce: check if th
-000163c0: 6520 7273 7973 6c6f 6720 646f 636b 6572  e rsyslog docker
-000163d0: 2028 7768 6963 6820 636f 6c6c 6563 7473   (which collects
-000163e0: 206c 6f67 7329 0a20 2020 2069 7320 696e   logs).    is in
-000163f0: 7369 6465 2074 6865 2074 6f70 6f6c 6f67  side the topolog
-00016400: 792c 2061 6e64 2069 6620 736f 2c20 6368  y, and if so, ch
-00016410: 6563 6b20 7468 6520 2268 6f73 745f 7061  eck the "host_pa
-00016420: 7468 2220 666f 7220 6c6f 6773 0a20 2020  th" for logs.   
-00016430: 2028 6120 7370 6563 6966 6963 2070 6174   (a specific pat
-00016440: 6820 6973 2065 7870 6563 7465 642c 2061  h is expected, a
-00016450: 6e64 2069 7320 6861 7264 636f 6465 6420  nd is hardcoded 
-00016460: 696e 2069 745f 7369 6d75 6c61 7469 6f6e  in it_simulation
-00016470: 290a 2020 2020 2222 220a 2020 2020 2320  ).    """.    # 
-00016480: 544f 444f 2843 5244 293a 2074 6869 7320  TODO(CRD): this 
-00016490: 6368 6563 6b20 7769 6c6c 2061 6c77 6179  check will alway
-000164a0: 7320 6661 696c 2077 6865 6e20 6372 5f61  s fail when cr_a
-000164b0: 7069 5f63 6c69 656e 742c 2074 6865 0a20  pi_client, the. 
-000164c0: 2020 2023 2069 745f 7369 6d75 6c61 7469     # it_simulati
-000164d0: 6f6e 2064 6f63 6b65 722c 2061 6e64 2074  on docker, and t
-000164e0: 6865 2072 7379 736c 6f67 2064 6f63 6b65  he rsyslog docke
-000164f0: 7220 6172 6520 6e6f 7420 6f6e 2074 6865  r are not on the
-00016500: 2073 616d 6520 6d61 6368 696e 650a 0a20   same machine.. 
-00016510: 2020 2074 6f70 6f6c 6f67 7920 3d20 5941     topology = YA
-00016520: 4d4c 2829 2e6c 6f61 6428 6665 7463 685f  ML().load(fetch_
-00016530: 7369 6d75 6c61 7469 6f6e 5f74 6f70 6f6c  simulation_topol
-00016540: 6f67 795f 7961 6d6c 2869 645f 7369 6d75  ogy_yaml(id_simu
-00016550: 6c61 7469 6f6e 2929 0a0a 2020 2020 2320  lation))..    # 
-00016560: 5468 6520 7061 7468 206f 6620 7468 6520  The path of the 
-00016570: 6c6f 6773 2c20 6f6e 2074 6865 2063 6f6d  logs, on the com
-00016580: 7075 7465 2073 6572 7665 7220 6669 6c65  pute server file
-00016590: 2073 7973 7465 6d20 7368 6f75 6c64 2041   system should A
-000165a0: 4c57 4159 5320 6265 2061 7320 666f 6c6c  LWAYS be as foll
-000165b0: 6f77 730a 2020 2020 7273 7973 6c6f 675f  ows.    rsyslog_
-000165c0: 646f 636b 6572 5f70 7265 7365 6e74 3a20  docker_present: 
-000165d0: 626f 6f6c 203d 2046 616c 7365 0a20 2020  bool = False.   
-000165e0: 2070 6f74 656e 7469 616c 5f6c 6f67 735f   potential_logs_
-000165f0: 6162 736f 6c75 7465 5f70 6174 683a 204c  absolute_path: L
-00016600: 6973 745b 5061 7468 5d20 3d20 5b5d 0a20  ist[Path] = []. 
-00016610: 2020 2066 6f72 206e 6f64 6520 696e 2074     for node in t
-00016620: 6f70 6f6c 6f67 795b 226e 6f64 6573 225d  opology["nodes"]
-00016630: 3a0a 2020 2020 2020 2020 6966 2028 0a20  :.        if (. 
-00016640: 2020 2020 2020 2020 2020 206e 6f64 655b             node[
-00016650: 2274 7970 6522 5d20 3d3d 2022 646f 636b  "type"] == "dock
-00016660: 6572 220a 2020 2020 2020 2020 2020 2020  er".            
-00016670: 616e 6420 2272 7379 736c 6f67 2220 696e  and "rsyslog" in
-00016680: 206e 6f64 655b 2262 6173 655f 696d 6167   node["base_imag
-00016690: 6522 5d0a 2020 2020 2020 2020 2020 2020  e"].            
-000166a0: 616e 6420 2276 6f6c 756d 6573 2220 696e  and "volumes" in
-000166b0: 206e 6f64 650a 2020 2020 2020 2020 293a   node.        ):
-000166c0: 0a20 2020 2020 2020 2020 2020 2072 7379  .            rsy
-000166d0: 736c 6f67 5f64 6f63 6b65 725f 7072 6573  slog_docker_pres
-000166e0: 656e 7420 3d20 5472 7565 0a20 2020 2020  ent = True.     
-000166f0: 2020 2020 2020 2066 6f72 2076 6f6c 756d         for volum
-00016700: 6520 696e 206e 6f64 655b 2276 6f6c 756d  e in node["volum
-00016710: 6573 225d 3a0a 2020 2020 2020 2020 2020  es"]:.          
-00016720: 2020 2020 2020 6966 2028 0a20 2020 2020        if (.     
-00016730: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00016740: 686f 7374 5f70 6174 6822 2069 6e20 766f  host_path" in vo
-00016750: 6c75 6d65 0a20 2020 2020 2020 2020 2020  lume.           
-00016760: 2020 2020 2020 2020 2061 6e64 2022 7772           and "wr
-00016770: 6974 6162 6c65 2220 696e 2076 6f6c 756d  itable" in volum
-00016780: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00016790: 2020 2020 2020 616e 6420 766f 6c75 6d65        and volume
-000167a0: 5b22 7772 6974 6162 6c65 225d 0a20 2020  ["writable"].   
-000167b0: 2020 2020 2020 2020 2020 2020 2029 3a0a               ):.
-000167c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000167d0: 2020 2020 706f 7465 6e74 6961 6c5f 6c6f      potential_lo
-000167e0: 6773 5f61 6273 6f6c 7574 655f 7061 7468  gs_absolute_path
-000167f0: 2e61 7070 656e 6428 5061 7468 2876 6f6c  .append(Path(vol
-00016800: 756d 655b 2268 6f73 745f 7061 7468 225d  ume["host_path"]
-00016810: 2929 0a0a 2020 2020 2320 4966 206e 6f20  ))..    # If no 
-00016820: 7273 7973 6c6f 6720 646f 636b 6572 2069  rsyslog docker i
-00016830: 7320 7072 6573 656e 742c 206a 7375 7420  s present, jsut 
-00016840: 6973 7375 6520 6120 6e6f 6e2d 626c 6f63  issue a non-bloc
-00016850: 6b69 6e67 2077 6172 6e69 6e67 0a20 2020  king warning.   
-00016860: 2069 6620 6e6f 7420 7273 7973 6c6f 675f   if not rsyslog_
-00016870: 646f 636b 6572 5f70 7265 7365 6e74 3a0a  docker_present:.
-00016880: 2020 2020 2020 2020 6c6f 6767 6572 2e77          logger.w
-00016890: 6172 6e69 6e67 280a 2020 2020 2020 2020  arning(.        
-000168a0: 2020 2020 2220 205b 2b5d 2054 6865 2063      "  [+] The c
-000168b0: 6f6c 6c65 6374 696f 6e20 6f66 206c 6f67  ollection of log
-000168c0: 7320 7761 7320 6e6f 7420 6163 7469 7661  s was not activa
-000168d0: 7465 6420 666f 7220 7468 6520 7369 6d75  ted for the simu
-000168e0: 6c61 7469 6f6e 2028 7468 6520 7273 7973  lation (the rsys
-000168f0: 6c6f 6720 646f 636b 6572 2069 7320 6e6f  log docker is no
-00016900: 7420 7072 6573 656e 7420 696e 2074 6865  t present in the
-00016910: 2074 6f70 6f6c 6f67 7929 2e20 4e6f 206c   topology). No l
-00016920: 6f67 2077 696c 6c20 6265 2069 6e63 6c75  og will be inclu
-00016930: 6465 6420 696e 2074 6865 2064 6174 6173  ded in the datas
-00016940: 6574 2e22 0a20 2020 2020 2020 2029 0a20  et.".        ). 
-00016950: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00016960: 2077 726f 6e67 5f68 6f73 745f 7061 7468   wrong_host_path
-00016970: 203d 2054 7275 650a 2020 2020 2020 2020   = True.        
-00016980: 666f 7220 7020 696e 2070 6f74 656e 7469  for p in potenti
-00016990: 616c 5f6c 6f67 735f 6162 736f 6c75 7465  al_logs_absolute
-000169a0: 5f70 6174 683a 0a20 2020 2020 2020 2020  _path:.         
-000169b0: 2020 2069 6620 6e6f 7420 702e 6973 5f61     if not p.is_a
-000169c0: 6273 6f6c 7574 6528 2920 616e 6420 7020  bsolute() and p 
-000169d0: 3d3d 2050 6174 6828 2273 6861 7265 645f  == Path("shared_
-000169e0: 7265 736f 7572 6365 732f 7273 7973 6c6f  resources/rsyslo
-000169f0: 672f 6c6f 6773 2229 3a0a 2020 2020 2020  g/logs"):.      
-00016a00: 2020 2020 2020 2020 2020 7772 6f6e 675f            wrong_
-00016a10: 686f 7374 5f70 6174 6820 3d20 4661 6c73  host_path = Fals
-00016a20: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00016a30: 2020 6272 6561 6b0a 2020 2020 2020 2020    break.        
-00016a40: 2020 2020 656c 6966 2070 2e69 735f 6162      elif p.is_ab
-00016a50: 736f 6c75 7465 2829 2061 6e64 2050 6174  solute() and Pat
-00016a60: 6828 7374 7228 7029 5b31 3a5d 2920 3d3d  h(str(p)[1:]) ==
-00016a70: 2050 6174 6828 0a20 2020 2020 2020 2020   Path(.         
-00016a80: 2020 2020 2020 2022 7368 6172 6564 5f72         "shared_r
-00016a90: 6573 6f75 7263 6573 2f72 7379 736c 6f67  esources/rsyslog
-00016aa0: 2f6c 6f67 7322 0a20 2020 2020 2020 2020  /logs".         
-00016ab0: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
-00016ac0: 2020 2020 2020 7772 6f6e 675f 686f 7374        wrong_host
-00016ad0: 5f70 6174 6820 3d20 4661 6c73 650a 2020  _path = False.  
-00016ae0: 2020 2020 2020 2020 2020 2020 2020 6272                br
-00016af0: 6561 6b0a 2020 2020 2020 2020 2020 2020  eak.            
-00016b00: 656c 6966 2070 2e69 735f 6162 736f 6c75  elif p.is_absolu
-00016b10: 7465 2829 2061 6e64 2070 203d 3d20 5061  te() and p == Pa
-00016b20: 7468 280a 2020 2020 2020 2020 2020 2020  th(.            
-00016b30: 2020 2020 222f 6379 6265 722d 7261 6e67      "/cyber-rang
-00016b40: 652d 6361 7461 6c6f 672f 7369 6d75 6c61  e-catalog/simula
-00016b50: 7469 6f6e 735f 7265 736f 7572 6365 732f  tions_resources/
-00016b60: 312f 7368 6172 6564 5f72 6573 6f75 7263  1/shared_resourc
-00016b70: 6573 2f72 7379 736c 6f67 2f6c 6f67 7322  es/rsyslog/logs"
-00016b80: 0a20 2020 2020 2020 2020 2020 2029 3a0a  .            ):.
-00016b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ba0: 7772 6f6e 675f 686f 7374 5f70 6174 6820  wrong_host_path 
-00016bb0: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
-00016bc0: 2020 2020 2020 2020 6272 6561 6b0a 0a20          break.. 
-00016bd0: 2020 2020 2020 2069 6620 7772 6f6e 675f         if wrong_
-00016be0: 686f 7374 5f70 6174 683a 0a20 2020 2020  host_path:.     
-00016bf0: 2020 2020 2020 206c 6f67 6765 722e 6572         logger.er
-00016c00: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
-00016c10: 2020 2020 2022 2020 5b2b 5d20 4974 2073       "  [+] It s
-00016c20: 6565 6d73 2074 6861 7420 7468 6520 7369  eems that the si
-00016c30: 6d75 6c61 7469 6f6e 2069 6e63 6c75 6465  mulation include
-00016c40: 7320 7468 6520 2772 7379 736c 6f67 2720  s the 'rsyslog' 
-00016c50: 646f 636b 6572 2074 6861 7420 636f 6c6c  docker that coll
-00016c60: 6563 7473 2074 6865 206c 6f67 732c 2062  ects the logs, b
-00016c70: 7574 2064 6f65 7320 6e6f 7420 7370 6563  ut does not spec
-00016c80: 6966 7920 7468 6520 6170 7072 6f70 7269  ify the appropri
-00016c90: 6174 6520 686f 7374 5f70 6174 6820 666f  ate host_path fo
-00016ca0: 7220 7468 6520 6c6f 6773 2e20 4974 2069  r the logs. It i
-00016cb0: 7320 6578 7065 6374 6564 2074 6861 7420  s expected that 
-00016cc0: 7468 6520 7273 7973 6c6f 6720 646f 636b  the rsyslog dock
-00016cd0: 6572 206e 6f64 6520 7370 6563 6966 6965  er node specifie
-00016ce0: 7320 6120 2877 7269 7461 626c 6529 2076  s a (writable) v
-00016cf0: 6f6c 756d 6520 7769 7468 2061 2068 6f73  olume with a hos
-00016d00: 745f 7061 7468 2065 7175 616c 2074 6f20  t_path equal to 
-00016d10: 272f 7368 6172 6564 5f72 6573 6f75 7263  '/shared_resourc
-00016d20: 6573 2f72 7379 736c 6f67 2f6c 6f67 7327  es/rsyslog/logs'
-00016d30: 2e20 4361 6e64 6964 6174 6573 2061 7265  . Candidates are
-00016d40: 2027 7b7d 2720 696e 7374 6561 642e 222e   '{}' instead.".
-00016d50: 666f 726d 6174 280a 2020 2020 2020 2020  format(.        
-00016d60: 2020 2020 2020 2020 2020 2020 5b73 7472              [str
-00016d70: 2870 2920 666f 7220 7020 696e 2070 6f74  (p) for p in pot
-00016d80: 656e 7469 616c 5f6c 6f67 735f 6162 736f  ential_logs_abso
-00016d90: 6c75 7465 5f70 6174 685d 2c0a 2020 2020  lute_path],.    
-00016da0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00016db0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00016dc0: 2020 2020 2020 2020 6c6f 6767 6572 2e65          logger.e
-00016dd0: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
-00016de0: 2020 2020 2020 2220 5b2b 5d20 4461 7461        " [+] Data
-00016df0: 7365 7420 6372 6561 7469 6f6e 2061 626f  set creation abo
-00016e00: 7274 6564 2e20 596f 7520 6d61 7920 7769  rted. You may wi
-00016e10: 7368 2074 6f20 6d6f 7665 2074 6865 206c  sh to move the l
-00016e20: 6f67 2066 696c 6573 2074 6f20 7468 6520  og files to the 
-00016e30: 6170 7072 6f70 7269 6174 6520 666f 6c64  appropriate fold
-00016e40: 6572 206f 6e20 7468 6520 636f 6d70 7574  er on the comput
-00016e50: 6520 7365 7276 6572 2873 292c 2061 6e64  e server(s), and
-00016e60: 2074 6865 6e20 7265 7472 792e 2041 6c74   then retry. Alt
-00016e70: 6572 6e61 7469 7665 6c79 2c20 796f 7520  ernatively, you 
-00016e80: 6361 6e20 6279 7061 7373 2074 6869 7320  can bypass this 
-00016e90: 6368 6563 6b20 7769 7468 2074 6865 2064  check with the d
-00016ea0: 6f6e 745f 6368 6563 6b5f 6c6f 675f 7061  ont_check_log_pa
-00016eb0: 7468 206f 7074 696f 6e2e 220a 2020 2020  th option.".    
-00016ec0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00016ed0: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
-00016ee0: 650a 0a0a 6465 6620 7374 6f70 5f64 6174  e...def stop_dat
-00016ef0: 6173 6574 5f63 7265 6174 696f 6e28 6461  aset_creation(da
-00016f00: 7461 7365 745f 6964 3a20 7575 6964 2e55  taset_id: uuid.U
-00016f10: 5549 4429 202d 3e20 416e 793a 0a20 2020  UID) -> Any:.   
-00016f20: 2022 2222 0a20 2020 2053 746f 7073 2f61   """.    Stops/a
-00016f30: 626f 7274 7320 7468 6520 6372 6561 7469  borts the creati
-00016f40: 6f6e 206f 6620 6120 6461 7461 7365 7420  on of a dataset 
-00016f50: 7468 6174 2069 7320 696e 2074 6865 2070  that is in the p
-00016f60: 726f 6365 7373 206f 6620 6265 696e 6720  rocess of being 
-00016f70: 6372 6561 7465 642e 0a0a 2020 2020 5468  created...    Th
-00016f80: 6973 2066 756e 6374 696f 6e20 7368 6f75  is function shou
-00016f90: 6c64 2062 6520 7573 6564 2c20 666f 7220  ld be used, for 
-00016fa0: 696e 7374 616e 6365 2c20 6966 2061 2064  instance, if a d
-00016fb0: 6174 6173 6574 2063 7265 6174 696f 6e20  ataset creation 
-00016fc0: 6861 7320 6265 656e 0a20 2020 2061 7574  has been.    aut
-00016fd0: 6f6d 6174 6963 616c 6c79 2073 7461 7274  omatically start
-00016fe0: 6564 2061 6c74 686f 7567 6820 7468 6520  ed although the 
-00016ff0: 7573 6572 2064 6f65 7320 6e6f 7420 7761  user does not wa
-00017000: 6e74 2061 2064 6174 6173 6574 2c20 616e  nt a dataset, an
-00017010: 6420 7468 6520 6461 7461 7365 740a 2020  d the dataset.  
-00017020: 2020 6372 6561 7469 6f6e 2070 726f 6365    creation proce
-00017030: 7373 2069 7320 7461 6b69 6e67 2074 6f6f  ss is taking too
-00017040: 206d 7563 6820 7469 6d65 2e0a 0a20 2020   much time...   
-00017050: 2057 4152 4e49 4e47 3a20 6166 7465 7220   WARNING: after 
-00017060: 7374 6f70 7069 6e67 2074 6865 2064 6174  stopping the dat
-00017070: 6173 6574 2063 7265 6174 696f 6e2c 2069  aset creation, i
-00017080: 7420 6973 2061 6476 6973 6564 2074 6f20  t is advised to 
-00017090: 6465 6c65 7465 206f 7220 6174 206c 6561  delete or at lea
-000170a0: 7374 0a20 2020 2072 6570 6169 7220 7468  st.    repair th
-000170b0: 6520 6461 7461 7365 742e 0a0a 2020 2020  e dataset...    
-000170c0: 3a70 6172 616d 2064 6174 6173 6574 5f69  :param dataset_i
-000170d0: 643a 2074 6865 2064 6174 6173 6574 2077  d: the dataset w
-000170e0: 6869 6368 2069 7320 696e 2074 6865 2070  hich is in the p
-000170f0: 726f 6365 7373 206f 6620 6265 696e 6720  rocess of being 
-00017100: 6372 6561 7465 6420 616e 6420 7468 6174  created and that
-00017110: 206d 7573 7420 6265 2061 626f 7274 6564   must be aborted
-00017120: 0a20 2020 203a 7265 7475 726e 3a20 7265  .    :return: re
-00017130: 7475 726e 2074 6865 206a 736f 6e20 626f  turn the json bo
-00017140: 6479 206f 6620 7468 6520 636f 7265 2041  dy of the core A
-00017150: 5049 2072 6573 706f 6e73 650a 2020 2020  PI response.    
-00017160: 2222 220a 2020 2020 2320 5369 6d70 6c79  """.    # Simply
-00017170: 2063 616c 6c73 2074 6865 2063 6f72 6520   calls the core 
-00017180: 4150 4920 7768 6963 6820 6974 7365 6c66  API which itself
-00017190: 2061 736b 7320 7468 6520 7075 626c 6973   asks the publis
-000171a0: 680a 2020 2020 2320 7365 7276 6572 2028  h.    # server (
-000171b0: 6261 636b 656e 6429 2074 6f20 7374 6f70  backend) to stop
-000171c0: 206f 6620 7468 6520 6461 7461 7365 7420   of the dataset 
-000171d0: 6372 6561 7469 6f6e 2070 726f 6365 7373  creation process
-000171e0: 2e0a 0a20 2020 2072 6573 756c 7420 3d20  ...    result = 
-000171f0: 5f70 7574 2822 2f63 7265 6174 655f 6461  _put("/create_da
-00017200: 7461 7365 742f 7374 6f70 2f7b 7d22 2e66  taset/stop/{}".f
-00017210: 6f72 6d61 7428 7374 7228 6461 7461 7365  ormat(str(datase
-00017220: 745f 6964 2929 290a 0a20 2020 2069 6620  t_id)))..    if 
-00017230: 7265 7375 6c74 2e73 7461 7475 735f 636f  result.status_co
-00017240: 6465 2021 3d20 3230 303a 0a20 2020 2020  de != 200:.     
-00017250: 2020 205f 6861 6e64 6c65 5f65 7272 6f72     _handle_error
-00017260: 2872 6573 756c 742c 2022 4361 6e6e 6f74  (result, "Cannot
-00017270: 2073 746f 7020 6461 7461 7365 7420 6372   stop dataset cr
-00017280: 6561 7469 6f6e 2074 6872 6f75 6768 2063  eation through c
-00017290: 6f72 6520 4150 4922 290a 0a20 2020 2072  ore API")..    r
-000172a0: 6574 7572 6e20 7265 7375 6c74 2e6a 736f  eturn result.jso
-000172b0: 6e28 290a 0a0a 6465 6620 6665 7463 685f  n()...def fetch_
-000172c0: 636f 6d70 7574 655f 7365 7276 6572 2863  compute_server(c
-000172d0: 6f6d 7075 7465 5f73 6572 7665 725f 6964  ompute_server_id
-000172e0: 3a20 696e 7429 202d 3e20 416e 793a 0a20  : int) -> Any:. 
-000172f0: 2020 2022 2222 5265 7475 726e 2061 2063     """Return a c
-00017300: 6f6d 7075 7465 2073 6572 7665 7220 6769  ompute server gi
-00017310: 7665 6e20 6974 7320 4944 2222 220a 2020  ven its ID""".  
-00017320: 2020 7265 7375 6c74 203d 205f 6765 7428    result = _get(
-00017330: 6622 2f63 6f6d 7075 7465 5f73 6572 7665  f"/compute_serve
-00017340: 7273 2f7b 636f 6d70 7574 655f 7365 7276  rs/{compute_serv
-00017350: 6572 5f69 647d 2229 0a0a 2020 2020 6966  er_id}")..    if
-00017360: 2072 6573 756c 742e 7374 6174 7573 5f63   result.status_c
-00017370: 6f64 6520 213d 2032 3030 3a0a 2020 2020  ode != 200:.    
-00017380: 2020 2020 5f68 616e 646c 655f 6572 726f      _handle_erro
-00017390: 7228 7265 7375 6c74 2c20 2243 616e 6e6f  r(result, "Canno
-000173a0: 7420 7265 7472 6965 7665 206e 6f64 6520  t retrieve node 
-000173b0: 6672 6f6d 2049 5420 5369 6d75 6c61 7469  from IT Simulati
-000173c0: 6f6e 2041 5049 2229 0a0a 2020 2020 7265  on API")..    re
-000173d0: 7475 726e 2072 6573 756c 742e 6a73 6f6e  turn result.json
-000173e0: 2829 0a0a 0a64 6566 2066 6574 6368 5f63  ()...def fetch_c
-000173f0: 6f6d 7075 7465 5f73 6572 7665 725f 6279  ompute_server_by
-00017400: 5f6e 6f64 655f 6964 286e 6f64 655f 6964  _node_id(node_id
-00017410: 3a20 696e 7429 202d 3e20 416e 793a 0a20  : int) -> Any:. 
-00017420: 2020 2022 2222 5265 7475 726e 2061 2063     """Return a c
-00017430: 6f6d 7075 7465 2073 6572 7665 7220 7768  ompute server wh
-00017440: 6572 6520 6120 6e6f 6465 2049 4420 6973  ere a node ID is
-00017450: 2072 756e 6e69 6e67 2222 220a 2020 2020   running""".    
-00017460: 7265 7375 6c74 203d 205f 6765 7428 6622  result = _get(f"
-00017470: 2f63 6f6d 7075 7465 5f73 6572 7665 7273  /compute_servers
-00017480: 2f6e 6f64 652f 7b6e 6f64 655f 6964 7d22  /node/{node_id}"
-00017490: 290a 0a20 2020 2069 6620 7265 7375 6c74  )..    if result
-000174a0: 2e73 7461 7475 735f 636f 6465 2021 3d20  .status_code != 
-000174b0: 3230 303a 0a20 2020 2020 2020 205f 6861  200:.        _ha
-000174c0: 6e64 6c65 5f65 7272 6f72 2872 6573 756c  ndle_error(resul
-000174d0: 742c 2022 4361 6e6e 6f74 2072 6574 7269  t, "Cannot retri
-000174e0: 6576 6520 6e6f 6465 2066 726f 6d20 4954  eve node from IT
-000174f0: 2053 696d 756c 6174 696f 6e20 4150 4922   Simulation API"
-00017500: 290a 0a20 2020 2072 6574 7572 6e20 7265  )..    return re
-00017510: 7375 6c74 2e6a 736f 6e28 290a 0a0a 6465  sult.json()...de
-00017520: 6620 6665 7463 685f 636f 6d70 7574 655f  f fetch_compute_
-00017530: 7365 7276 6572 7328 2920 2d3e 204c 6973  servers() -> Lis
-00017540: 745b 4469 6374 5b73 7472 2c20 416e 795d  t[Dict[str, Any]
-00017550: 5d3a 0a20 2020 2022 2222 0a20 2020 2052  ]:.    """.    R
-00017560: 6574 7572 6e20 7468 6520 6c69 7374 206f  eturn the list o
-00017570: 6620 636f 6d70 7574 6520 7365 7276 6572  f compute server
-00017580: 7320 6173 206b 6e6f 776e 2069 6e20 6461  s as known in da
-00017590: 7461 6261 7365 0a20 2020 2022 2222 0a20  tabase.    """. 
-000175a0: 2020 2072 6573 756c 7420 3d20 5f67 6574     result = _get
-000175b0: 2822 2f63 6f6d 7075 7465 5f73 6572 7665  ("/compute_serve
-000175c0: 7273 2f22 290a 0a20 2020 2069 6620 7265  rs/")..    if re
-000175d0: 7375 6c74 2e73 7461 7475 735f 636f 6465  sult.status_code
-000175e0: 2021 3d20 3230 303a 0a20 2020 2020 2020   != 200:.       
-000175f0: 205f 6861 6e64 6c65 5f65 7272 6f72 2872   _handle_error(r
-00017600: 6573 756c 742c 2022 4361 6e6e 6f74 2072  esult, "Cannot r
-00017610: 6574 7269 6576 6520 636f 6d70 7574 6520  etrieve compute 
-00017620: 7365 7276 6572 7320 6672 6f6d 2049 5420  servers from IT 
-00017630: 5369 6d75 6c61 7469 6f6e 2041 5049 2229  Simulation API")
-00017640: 0a0a 2020 2020 7265 7475 726e 2072 6573  ..    return res
-00017650: 756c 742e 6a73 6f6e 2829 0a0a 0a64 6566  ult.json()...def
-00017660: 2064 656c 6574 655f 636f 6d70 7574 655f   delete_compute_
-00017670: 7365 7276 6572 2863 6f6d 7075 7465 5f73  server(compute_s
-00017680: 6572 7665 725f 6964 3a20 696e 7429 202d  erver_id: int) -
-00017690: 3e20 4e6f 6e65 3a0a 2020 2020 2222 220a  > None:.    """.
-000176a0: 2020 2020 4465 6c65 7465 7320 6120 636f      Deletes a co
-000176b0: 6d70 7574 6520 7365 7276 6572 2069 6e20  mpute server in 
-000176c0: 6461 7461 6261 7365 2075 7369 6e67 2069  database using i
-000176d0: 7473 2069 640a 0a20 2020 2043 6f6d 7075  ts id..    Compu
-000176e0: 7465 2073 6572 7665 7273 2069 6473 2063  te servers ids c
-000176f0: 616e 2062 6520 6f62 7461 696e 6564 2074  an be obtained t
-00017700: 6872 6f75 6768 2060 6379 6265 725f 7261  hrough `cyber_ra
-00017710: 6e67 6520 7374 6174 7573 60c2 a06f 7220  nge status`..or 
-00017720: 3a66 756e 633a 6066 6574 6368 5f63 6f6d  :func:`fetch_com
-00017730: 7075 7465 5f73 6572 7665 7260 2e0a 2020  pute_server`..  
-00017740: 2020 2222 220a 2020 2020 7265 7375 6c74    """.    result
-00017750: 203d 205f 6465 6c65 7465 2866 222f 636f   = _delete(f"/co
-00017760: 6d70 7574 655f 7365 7276 6572 732f 7b63  mpute_servers/{c
-00017770: 6f6d 7075 7465 5f73 6572 7665 725f 6964  ompute_server_id
-00017780: 7d22 290a 0a20 2020 2069 6620 7265 7375  }")..    if resu
-00017790: 6c74 2e73 7461 7475 735f 636f 6465 2021  lt.status_code !
-000177a0: 3d20 3230 303a 0a20 2020 2020 2020 205f  = 200:.        _
-000177b0: 6861 6e64 6c65 5f65 7272 6f72 2872 6573  handle_error(res
-000177c0: 756c 742c 2022 4361 6e6e 6f74 2064 656c  ult, "Cannot del
-000177d0: 6574 6520 636f 6d70 7574 6520 7365 7276  ete compute serv
-000177e0: 6572 2069 6e20 636f 7265 2041 5049 2229  er in core API")
-000177f0: 0a0a 2020 2020 7265 7475 726e 2072 6573  ..    return res
-00017800: 756c 742e 6a73 6f6e 2829 0a              ult.json().
+00013880: 696d 756c 6174 696f 6e3a 2054 6865 2073  imulation: The s
+00013890: 696d 756c 6174 696f 6e20 4944 2e0a 0a20  imulation ID... 
+000138a0: 2020 2022 2222 0a20 2020 205f 7369 6d75     """.    _simu
+000138b0: 6c61 7469 6f6e 5f65 7865 6375 7465 5f6f  lation_execute_o
+000138c0: 7065 7261 7469 6f6e 2822 6765 7422 2c20  peration("get", 
+000138d0: 2270 6175 7365 222c 2069 645f 7369 6d75  "pause", id_simu
+000138e0: 6c61 7469 6f6e 2c20 2250 4155 5349 4e47  lation, "PAUSING
+000138f0: 2229 0a0a 0a64 6566 2075 6e70 6175 7365  ")...def unpause
+00013900: 5f73 696d 756c 6174 696f 6e28 6964 5f73  _simulation(id_s
+00013910: 696d 756c 6174 696f 6e3a 2069 6e74 2920  imulation: int) 
+00013920: 2d3e 204e 6f6e 653a 0a20 2020 2022 2222  -> None:.    """
+00013930: 556e 7061 7573 6520 6120 7369 6d75 6c61  Unpause a simula
+00013940: 7469 6f6e 2028 6361 6c6c 7320 6c69 6276  tion (calls libv
+00013950: 6972 7420 7265 7375 6d65 2041 5049 292e  irt resume API).
+00013960: 0a0a 2020 2020 3a70 6172 616d 2069 645f  ..    :param id_
+00013970: 7369 6d75 6c61 7469 6f6e 3a20 5468 6520  simulation: The 
+00013980: 7369 6d75 6c61 7469 6f6e 2049 442e 0a0a  simulation ID...
+00013990: 2020 2020 2222 220a 2020 2020 5f73 696d      """.    _sim
+000139a0: 756c 6174 696f 6e5f 6578 6563 7574 655f  ulation_execute_
+000139b0: 6f70 6572 6174 696f 6e28 2267 6574 222c  operation("get",
+000139c0: 2022 756e 7061 7573 6522 2c20 6964 5f73   "unpause", id_s
+000139d0: 696d 756c 6174 696f 6e2c 2022 554e 5041  imulation, "UNPA
+000139e0: 5553 494e 4722 290a 0a0a 6465 6620 6372  USING")...def cr
+000139f0: 6561 7465 5f62 6163 6b75 705f 7369 6d75  eate_backup_simu
+00013a00: 6c61 7469 6f6e 280a 2020 2020 6964 5f73  lation(.    id_s
+00013a10: 696d 756c 6174 696f 6e3a 2069 6e74 2c0a  imulation: int,.
+00013a20: 2020 2020 6e6f 6465 733a 204f 7074 696f      nodes: Optio
+00013a30: 6e61 6c5b 4c69 7374 5b73 7472 5d5d 203d  nal[List[str]] =
+00013a40: 204e 6f6e 652c 0a29 202d 3e20 4e6f 6e65   None,.) -> None
+00013a50: 3a0a 2020 2020 2222 2243 7265 6174 6520  :.    """Create 
+00013a60: 6261 636b 7570 206f 6620 6120 7369 6d75  backup of a simu
+00013a70: 6c61 7469 6f6e 2e20 4974 2069 7320 706f  lation. It is po
+00013a80: 7373 6962 6c65 2074 6f20 7370 6563 6966  ssible to specif
+00013a90: 7920 7468 6520 6e6f 6465 730a 2020 2020  y the nodes.    
+00013aa0: 746f 2062 6163 6b75 702e 2042 7920 6465  to backup. By de
+00013ab0: 6661 756c 742c 2061 6c6c 206e 6f64 6573  fault, all nodes
+00013ac0: 2061 7265 2062 6163 6b65 6420 7570 2e0a   are backed up..
+00013ad0: 0a20 2020 203a 7061 7261 6d20 6964 5f73  .    :param id_s
+00013ae0: 696d 756c 6174 696f 6e3a 2054 6865 2073  imulation: The s
+00013af0: 696d 756c 6174 696f 6e20 4944 2e0a 2020  imulation ID..  
+00013b00: 2020 3a70 6172 616d 206e 6f64 6573 3a20    :param nodes: 
+00013b10: 5468 6520 6e6f 6465 7320 666f 7220 7768  The nodes for wh
+00013b20: 6963 6820 746f 2063 7265 6174 6520 6261  ich to create ba
+00013b30: 636b 7570 2028 616c 6c20 6e6f 6465 7320  ckup (all nodes 
+00013b40: 6279 2064 6566 6175 6c74 292e 0a0a 2020  by default)...  
+00013b50: 2020 2222 220a 0a20 2020 2069 6620 6e6f    """..    if no
+00013b60: 6465 7320 6973 204e 6f6e 653a 0a20 2020  des is None:.   
+00013b70: 2020 2020 206e 6f64 6573 203d 205b 5d0a       nodes = [].
+00013b80: 2020 2020 706f 7374 5f64 6174 6120 3d20      post_data = 
+00013b90: 7b22 6e6f 6465 7322 3a20 6e6f 6465 737d  {"nodes": nodes}
+00013ba0: 0a0a 2020 2020 5f73 696d 756c 6174 696f  ..    _simulatio
+00013bb0: 6e5f 6578 6563 7574 655f 6f70 6572 6174  n_execute_operat
+00013bc0: 696f 6e28 0a20 2020 2020 2020 2022 706f  ion(.        "po
+00013bd0: 7374 222c 2022 6372 6561 7465 5f62 6163  st", "create_bac
+00013be0: 6b75 7022 2c20 6964 5f73 696d 756c 6174  kup", id_simulat
+00013bf0: 696f 6e2c 2022 5052 4550 4152 494e 4722  ion, "PREPARING"
+00013c00: 2c20 706f 7374 5f64 6174 613d 706f 7374  , post_data=post
+00013c10: 5f64 6174 610a 2020 2020 290a 0a0a 6465  _data.    )...de
+00013c20: 6620 7265 7374 6f72 655f 6261 636b 7570  f restore_backup
+00013c30: 5f73 696d 756c 6174 696f 6e28 0a20 2020  _simulation(.   
+00013c40: 2069 645f 7369 6d75 6c61 7469 6f6e 3a20   id_simulation: 
+00013c50: 696e 742c 0a20 2020 206e 6f64 6573 3a20  int,.    nodes: 
+00013c60: 4f70 7469 6f6e 616c 5b4c 6973 745b 7374  Optional[List[st
+00013c70: 725d 5d20 3d20 4e6f 6e65 2c0a 2920 2d3e  r]] = None,.) ->
+00013c80: 204e 6f6e 653a 0a20 2020 2022 2222 5265   None:.    """Re
+00013c90: 7374 6f72 6520 6261 636b 7570 206f 6620  store backup of 
+00013ca0: 6120 7369 6d75 6c61 7469 6f6e 2e20 4974  a simulation. It
+00013cb0: 2069 7320 706f 7373 6962 6c65 2074 6f20   is possible to 
+00013cc0: 7370 6563 6966 7920 7468 6520 6e6f 6465  specify the node
+00013cd0: 730a 2020 2020 746f 2072 6573 746f 7265  s.    to restore
+00013ce0: 2e20 4279 2064 6566 6175 6c74 2c20 616c  . By default, al
+00013cf0: 6c20 6e6f 6465 7320 6172 6520 7265 7374  l nodes are rest
+00013d00: 6f72 6564 2e0a 0a20 2020 203a 7061 7261  ored...    :para
+00013d10: 6d20 6964 5f73 696d 756c 6174 696f 6e3a  m id_simulation:
+00013d20: 2054 6865 2073 696d 756c 6174 696f 6e20   The simulation 
+00013d30: 4944 2e0a 2020 2020 3a70 6172 616d 206e  ID..    :param n
+00013d40: 6f64 6573 3a20 5468 6520 6e6f 6465 7320  odes: The nodes 
+00013d50: 666f 7220 7768 6963 6820 746f 2072 6573  for which to res
+00013d60: 746f 7265 2062 6163 6b75 7020 2861 6c6c  tore backup (all
+00013d70: 206e 6f64 6573 2062 7920 6465 6661 756c   nodes by defaul
+00013d80: 7429 2e0a 0a20 2020 2022 2222 0a0a 2020  t)...    """..  
+00013d90: 2020 6966 206e 6f64 6573 2069 7320 4e6f    if nodes is No
+00013da0: 6e65 3a0a 2020 2020 2020 2020 6e6f 6465  ne:.        node
+00013db0: 7320 3d20 5b5d 0a20 2020 2070 6f73 745f  s = [].    post_
+00013dc0: 6461 7461 203d 207b 226e 6f64 6573 223a  data = {"nodes":
+00013dd0: 206e 6f64 6573 7d0a 0a20 2020 205f 7369   nodes}..    _si
+00013de0: 6d75 6c61 7469 6f6e 5f65 7865 6375 7465  mulation_execute
+00013df0: 5f6f 7065 7261 7469 6f6e 280a 2020 2020  _operation(.    
+00013e00: 2020 2020 2270 6f73 7422 2c20 2272 6573      "post", "res
+00013e10: 746f 7265 5f62 6163 6b75 7022 2c20 6964  tore_backup", id
+00013e20: 5f73 696d 756c 6174 696f 6e2c 2022 5052  _simulation, "PR
+00013e30: 4550 4152 494e 4722 2c20 706f 7374 5f64  EPARING", post_d
+00013e40: 6174 613d 706f 7374 5f64 6174 610a 2020  ata=post_data.  
+00013e50: 2020 290a 0a0a 6465 6620 6861 6c74 5f73    )...def halt_s
+00013e60: 696d 756c 6174 696f 6e28 6964 5f73 696d  imulation(id_sim
+00013e70: 756c 6174 696f 6e3a 2069 6e74 2c20 6e6f  ulation: int, no
+00013e80: 6465 733a 204f 7074 696f 6e61 6c5b 4c69  des: Optional[Li
+00013e90: 7374 5b73 7472 5d5d 203d 204e 6f6e 6529  st[str]] = None)
+00013ea0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2222   -> None:.    ""
+00013eb0: 2250 726f 7065 726c 7920 7374 6f70 2061  "Properly stop a
+00013ec0: 2073 696d 756c 6174 696f 6e2c 2062 7920   simulation, by 
+00013ed0: 7365 6e64 696e 6720 6120 7368 7574 646f  sending a shutdo
+00013ee0: 776e 2073 6967 6e61 6c20 746f 2074 6865  wn signal to the
+00013ef0: 0a20 2020 206f 7065 7261 7469 6e67 2073  .    operating s
+00013f00: 7973 7465 6d73 2e20 4974 2069 7320 706f  ystems. It is po
+00013f10: 7373 6962 6c65 2074 6f20 7370 6563 6966  ssible to specif
+00013f20: 7920 7468 6520 6e6f 6465 7320 746f 0a20  y the nodes to. 
+00013f30: 2020 2073 7461 7274 2e20 4279 2064 6566     start. By def
+00013f40: 6175 6c74 2c20 616c 6c20 6e6f 6465 7320  ault, all nodes 
+00013f50: 6172 6520 7374 6172 7465 642e 0a0a 2020  are started...  
+00013f60: 2020 3a70 6172 616d 2069 645f 7369 6d75    :param id_simu
+00013f70: 6c61 7469 6f6e 3a20 5468 6520 7369 6d75  lation: The simu
+00013f80: 6c61 7469 6f6e 2049 442e 0a20 2020 203a  lation ID..    :
+00013f90: 7061 7261 6d20 6e6f 6465 733a 2054 6865  param nodes: The
+00013fa0: 206e 6f64 6573 2074 6f20 6861 6c74 2028   nodes to halt (
+00013fb0: 616c 6c20 6e6f 6465 7320 6279 2064 6566  all nodes by def
+00013fc0: 6175 6c74 292e 0a0a 2020 2020 2222 220a  ault)...    """.
+00013fd0: 2020 2020 6966 206e 6f64 6573 2069 7320      if nodes is 
+00013fe0: 4e6f 6e65 3a0a 2020 2020 2020 2020 6e6f  None:.        no
+00013ff0: 6465 7320 3d20 5b5d 0a20 2020 2070 6f73  des = [].    pos
+00014000: 745f 6461 7461 203d 207b 226e 6f64 6573  t_data = {"nodes
+00014010: 223a 206e 6f64 6573 7d0a 0a20 2020 205f  ": nodes}..    _
+00014020: 7369 6d75 6c61 7469 6f6e 5f65 7865 6375  simulation_execu
+00014030: 7465 5f6f 7065 7261 7469 6f6e 280a 2020  te_operation(.  
+00014040: 2020 2020 2020 2270 6f73 7422 2c0a 2020        "post",.  
+00014050: 2020 2020 2020 2273 746f 7022 2c0a 2020        "stop",.  
+00014060: 2020 2020 2020 6964 5f73 696d 756c 6174        id_simulat
+00014070: 696f 6e2c 0a20 2020 2020 2020 2022 5354  ion,.        "ST
+00014080: 4f50 5049 4e47 222c 0a20 2020 2020 2020  OPPING",.       
+00014090: 2070 6f73 745f 6461 7461 3d70 6f73 745f   post_data=post_
+000140a0: 6461 7461 2c0a 2020 2020 290a 0a0a 6465  data,.    )...de
+000140b0: 6620 6465 7374 726f 795f 7369 6d75 6c61  f destroy_simula
+000140c0: 7469 6f6e 2869 645f 7369 6d75 6c61 7469  tion(id_simulati
+000140d0: 6f6e 3a20 696e 742c 206e 6f64 6573 3a20  on: int, nodes: 
+000140e0: 4f70 7469 6f6e 616c 5b4c 6973 745b 7374  Optional[List[st
+000140f0: 725d 5d20 3d20 4e6f 6e65 2920 2d3e 204e  r]] = None) -> N
+00014100: 6f6e 653a 0a20 2020 2022 2222 5374 6f70  one:.    """Stop
+00014110: 2061 2073 696d 756c 6174 696f 6e20 7468   a simulation th
+00014120: 726f 7567 6820 6120 6861 7264 2072 6573  rough a hard res
+00014130: 6574 2e0a 0a20 2020 203a 7061 7261 6d20  et...    :param 
+00014140: 6964 5f73 696d 756c 6174 696f 6e3a 2054  id_simulation: T
+00014150: 6865 2073 696d 756c 6174 696f 6e20 4944  he simulation ID
+00014160: 2e0a 2020 2020 3a70 6172 616d 206e 6f64  ..    :param nod
+00014170: 6573 3a20 5468 6520 6e6f 6465 7320 746f  es: The nodes to
+00014180: 2064 6573 7472 6f79 2028 616c 6c20 6e6f   destroy (all no
+00014190: 6465 7320 6279 2064 6566 6175 6c74 292e  des by default).
+000141a0: 0a0a 2020 2020 2222 220a 0a20 2020 2069  ..    """..    i
+000141b0: 6620 6e6f 6465 7320 6973 204e 6f6e 653a  f nodes is None:
+000141c0: 0a20 2020 2020 2020 206e 6f64 6573 203d  .        nodes =
+000141d0: 205b 5d0a 2020 2020 706f 7374 5f64 6174   [].    post_dat
+000141e0: 6120 3d20 7b22 6e6f 6465 7322 3a20 6e6f  a = {"nodes": no
+000141f0: 6465 737d 0a0a 2020 2020 5f73 696d 756c  des}..    _simul
+00014200: 6174 696f 6e5f 6578 6563 7574 655f 6f70  ation_execute_op
+00014210: 6572 6174 696f 6e28 0a20 2020 2020 2020  eration(.       
+00014220: 2022 706f 7374 222c 2022 6465 7374 726f   "post", "destro
+00014230: 7922 2c20 6964 5f73 696d 756c 6174 696f  y", id_simulatio
+00014240: 6e2c 2022 5354 4f50 5049 4e47 222c 2070  n, "STOPPING", p
+00014250: 6f73 745f 6461 7461 3d70 6f73 745f 6461  ost_data=post_da
+00014260: 7461 0a20 2020 2029 0a0a 0a64 6566 2063  ta.    )...def c
+00014270: 6c6f 6e65 5f73 696d 756c 6174 696f 6e28  lone_simulation(
+00014280: 6964 5f73 696d 756c 6174 696f 6e3a 2069  id_simulation: i
+00014290: 6e74 2920 2d3e 2069 6e74 3a0a 2020 2020  nt) -> int:.    
+000142a0: 2222 2243 6c6f 6e65 2061 2073 696d 756c  """Clone a simul
+000142b0: 6174 696f 6e20 616e 6420 6372 6561 7465  ation and create
+000142c0: 2061 206e 6577 2073 696d 756c 6174 696f   a new simulatio
+000142d0: 6e2c 2061 6e64 2072 6574 7572 6e20 7468  n, and return th
+000142e0: 6520 6e65 7720 4944 2e0a 0a20 2020 203a  e new ID...    :
+000142f0: 7265 7475 726e 3a20 5468 6520 4944 206f  return: The ID o
+00014300: 6620 7468 6520 636c 6f6e 6564 2073 696d  f the cloned sim
+00014310: 756c 6174 696f 6e2e 0a0a 2020 2020 3a70  ulation...    :p
+00014320: 6172 616d 2069 645f 7369 6d75 6c61 7469  aram id_simulati
+00014330: 6f6e 3a20 5468 6520 7369 6d75 6c61 7469  on: The simulati
+00014340: 6f6e 2049 442e 0a0a 2020 2020 2222 220a  on ID...    """.
+00014350: 2020 2020 6964 5f6e 6577 5f73 696d 756c      id_new_simul
+00014360: 6174 696f 6e20 3d20 5f73 696d 756c 6174  ation = _simulat
+00014370: 696f 6e5f 6578 6563 7574 655f 6f70 6572  ion_execute_oper
+00014380: 6174 696f 6e28 0a20 2020 2020 2020 2022  ation(.        "
+00014390: 6765 7422 2c20 2263 6c6f 6e65 222c 2069  get", "clone", i
+000143a0: 645f 7369 6d75 6c61 7469 6f6e 2c20 2243  d_simulation, "C
+000143b0: 4c4f 4e49 4e47 220a 2020 2020 290a 2020  LONING".    ).  
+000143c0: 2020 7265 7475 726e 2069 645f 6e65 775f    return id_new_
+000143d0: 7369 6d75 6c61 7469 6f6e 0a0a 0a64 6566  simulation...def
+000143e0: 206e 6574 5f63 7265 6174 655f 7072 6f62   net_create_prob
+000143f0: 6528 2020 2320 6e6f 7161 3a20 4339 3031  e(  # noqa: C901
+00014400: 0a20 2020 2069 645f 7369 6d75 6c61 7469  .    id_simulati
+00014410: 6f6e 3a20 696e 742c 0a20 2020 2073 696d  on: int,.    sim
+00014420: 755f 6e6f 6465 733a 2044 6963 742c 0a20  u_nodes: Dict,. 
+00014430: 2020 2069 6661 6365 3a20 4f70 7469 6f6e     iface: Option
+00014440: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
+00014450: 2020 2020 7063 6170 3a20 4f70 7469 6f6e      pcap: Option
+00014460: 616c 5b62 6f6f 6c5d 203d 2046 616c 7365  al[bool] = False
+00014470: 2c0a 2020 2020 6669 6c74 6572 3a20 4f70  ,.    filter: Op
+00014480: 7469 6f6e 616c 5b73 7472 5d20 3d20 2222  tional[str] = ""
+00014490: 2c0a 2020 2020 6469 7265 6374 696f 6e3a  ,.    direction:
+000144a0: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+000144b0: 2022 626f 7468 222c 0a29 202d 3e20 696e   "both",.) -> in
+000144c0: 743a 0a20 2020 2022 2222 4372 6561 7465  t:.    """Create
+000144d0: 2061 206e 6577 2070 726f 6265 2061 6e64   a new probe and
+000144e0: 2063 6f6e 6669 6775 7265 2068 6973 206e   configure his n
+000144f0: 6574 776f 726b 2063 6f6c 6c65 6374 696f  etwork collectio
+00014500: 6e73 2070 6f69 6e74 732e 0a0a 2020 2020  ns points...    
+00014510: 3a70 6172 616d 2069 645f 7369 6d75 6c61  :param id_simula
+00014520: 7469 6f6e 3a20 5468 6520 7369 6d75 6c61  tion: The simula
+00014530: 7469 6f6e 2049 442e 0a20 2020 203a 7061  tion ID..    :pa
+00014540: 7261 6d20 7369 6d75 5f6e 6f64 6573 3a20  ram simu_nodes: 
+00014550: 4120 6469 6374 696f 6e61 7279 2073 746f  A dictionary sto
+00014560: 7269 6e67 2074 6865 2063 6f6c 6c65 6374  ring the collect
+00014570: 696f 6e20 706f 696e 7473 2074 6f20 6361  ion points to ca
+00014580: 7074 7572 652e 2045 783a 207b 2773 7769  pture. Ex: {'swi
+00014590: 7463 6873 273a 205b 5b27 7377 6974 6368  tchs': [['switch
+000145a0: 3127 2c20 2763 6c69 656e 7431 275d 5d2c  1', 'client1']],
+000145b0: 2027 6e6f 6465 7327 3a20 5b27 636c 6965   'nodes': ['clie
+000145c0: 6e74 3227 5d7d 2e0a 2020 2020 3a70 6172  nt2']}..    :par
+000145d0: 616d 2069 6661 6365 3a20 496e 7465 7266  am iface: Interf
+000145e0: 6163 6520 7768 6572 6520 7468 6520 7472  ace where the tr
+000145f0: 6166 6669 6320 6973 206d 6972 726f 7265  affic is mirrore
+00014600: 6420 746f 2e20 4578 3a20 2764 756d 6d79  d to. Ex: 'dummy
+00014610: 3027 2e0a 2020 2020 3a70 6172 616d 2070  0'..    :param p
+00014620: 6361 703a 2041 2062 6f6f 6c65 616e 2069  cap: A boolean i
+00014630: 6e64 6963 6174 696e 6720 6966 2074 6865  ndicating if the
+00014640: 2063 6170 7475 7265 2073 686f 756c 6420   capture should 
+00014650: 6265 2073 6176 6564 206f 6e20 6469 736b  be saved on disk
+00014660: 2069 6e20 6120 7063 6170 2066 696c 6520   in a pcap file 
+00014670: 2874 6f20 6265 2069 6e63 6c75 6465 6420  (to be included 
+00014680: 696e 2064 6174 6173 6574 290a 2020 2020  in dataset).    
+00014690: 3a70 6172 616d 2066 696c 7465 723a 2053  :param filter: S
+000146a0: 7472 696e 6720 6669 6c74 6572 696e 6720  tring filtering 
+000146b0: 7463 7064 756d 7020 6361 7074 7572 652e  tcpdump capture.
+000146c0: 2045 783a 2027 7463 7020 706f 7274 2038   Ex: 'tcp port 8
+000146d0: 3027 2e0a 2020 2020 3a70 6172 616d 2064  0'..    :param d
+000146e0: 6972 6563 7469 6f6e 3a20 5365 6c65 6374  irection: Select
+000146f0: 2077 6869 6368 2074 7261 6666 6963 2074   which traffic t
+00014700: 6f20 6d6f 6e69 746f 7220 6f6e 2074 6865  o monitor on the
+00014710: 206d 6972 726f 7265 6420 696e 7465 7266   mirrored interf
+00014720: 6163 6528 7329 3a20 6569 7468 6572 2027  ace(s): either '
+00014730: 696e 6772 6573 7327 2c20 2765 6772 6573  ingress', 'egres
+00014740: 7327 206f 7220 2762 6f74 6827 2e0a 0a20  s' or 'both'... 
+00014750: 2020 2022 2222 0a0a 2020 2020 6e65 7477     """..    netw
+00014760: 6f72 6b5f 696e 7465 7266 6163 6573 203d  ork_interfaces =
+00014770: 205b 5d0a 0a20 2020 2069 6620 7369 6d75   []..    if simu
+00014780: 5f6e 6f64 6573 5b22 7377 6974 6368 7322  _nodes["switchs"
+00014790: 5d20 6973 204e 6f6e 6520 616e 6420 7369  ] is None and si
+000147a0: 6d75 5f6e 6f64 6573 5b22 6e6f 6465 7322  mu_nodes["nodes"
+000147b0: 5d20 6973 204e 6f6e 653a 0a20 2020 2020  ] is None:.     
+000147c0: 2020 2023 2043 6f6e 7369 6465 7220 616c     # Consider al
+000147d0: 6c20 6e6f 6465 206f 6620 7468 6520 7369  l node of the si
+000147e0: 6d75 6c61 7469 6f6e 2028 6578 6365 7074  mulation (except
+000147f0: 2072 6f75 7465 7273 2074 6861 7420 6172   routers that ar
+00014800: 650a 2020 2020 2020 2020 2320 4f56 4e20  e.        # OVN 
+00014810: 6162 7374 7261 6374 206f 626a 6563 7473  abstract objects
+00014820: 206f 6e20 7768 6963 6820 6974 2069 7320   on which it is 
+00014830: 6e6f 7420 706f 7373 6962 6c65 2074 6f20  not possible to 
+00014840: 6361 7074 7572 650a 2020 2020 2020 2020  capture.        
+00014850: 2320 7472 6166 6669 6329 0a20 2020 2020  # traffic).     
+00014860: 2020 2066 6f72 206e 6f64 6520 696e 2066     for node in f
+00014870: 6574 6368 5f6e 6f64 6573 2869 645f 7369  etch_nodes(id_si
+00014880: 6d75 6c61 7469 6f6e 293a 0a20 2020 2020  mulation):.     
+00014890: 2020 2020 2020 2069 6620 6e6f 6465 5b22         if node["
+000148a0: 7479 7065 225d 2021 3d20 2272 6f75 7465  type"] != "route
+000148b0: 7222 3a0a 2020 2020 2020 2020 2020 2020  r":.            
+000148c0: 2020 2020 666f 7220 6e65 7477 6f72 6b5f      for network_
+000148d0: 696e 7465 7266 6163 6520 696e 206e 6f64  interface in nod
+000148e0: 655b 226e 6574 776f 726b 5f69 6e74 6572  e["network_inter
+000148f0: 6661 6365 7322 5d3a 0a20 2020 2020 2020  faces"]:.       
+00014900: 2020 2020 2020 2020 2020 2020 206e 6574               net
+00014910: 776f 726b 5f69 6e74 6572 6661 6365 732e  work_interfaces.
+00014920: 6170 7065 6e64 286e 6574 776f 726b 5f69  append(network_i
+00014930: 6e74 6572 6661 6365 5b22 6d61 635f 6164  nterface["mac_ad
+00014940: 6472 6573 7322 5d29 0a20 2020 2065 6c73  dress"]).    els
+00014950: 653a 0a20 2020 2020 2020 2069 6620 7369  e:.        if si
+00014960: 6d75 5f6e 6f64 6573 5b22 7377 6974 6368  mu_nodes["switch
+00014970: 7322 5d20 6973 206e 6f74 204e 6f6e 653a  s"] is not None:
+00014980: 0a20 2020 2020 2020 2020 2020 2023 204d  .            # M
+00014990: 6972 726f 7220 7472 6166 6669 6320 6672  irror traffic fr
+000149a0: 6f6d 206e 6f64 6520 696e 7465 7266 6163  om node interfac
+000149b0: 6573 2063 6f6e 6e65 6374 6564 2074 6f20  es connected to 
+000149c0: 7468 6520 7370 6563 6966 6965 6420 7377  the specified sw
+000149d0: 6974 6368 730a 2020 2020 2020 2020 2020  itchs.          
+000149e0: 2020 666f 7220 7377 6974 6368 5f6e 6f64    for switch_nod
+000149f0: 6573 2069 6e20 7369 6d75 5f6e 6f64 6573  es in simu_nodes
+00014a00: 5b22 7377 6974 6368 7322 5d3a 0a20 2020  ["switchs"]:.   
+00014a10: 2020 2020 2020 2020 2020 2020 2073 7769               swi
+00014a20: 7463 6820 3d20 6665 7463 685f 6e6f 6465  tch = fetch_node
+00014a30: 5f62 795f 6e61 6d65 2869 645f 7369 6d75  _by_name(id_simu
+00014a40: 6c61 7469 6f6e 2c20 7377 6974 6368 5f6e  lation, switch_n
+00014a50: 6f64 6573 5b30 5d29 0a0a 2020 2020 2020  odes[0])..      
+00014a60: 2020 2020 2020 2020 2020 2320 4368 6563            # Chec
+00014a70: 6b20 6966 2073 7065 6369 6669 6320 6e6f  k if specific no
+00014a80: 6465 7320 6172 6520 6465 6669 6e65 642c  des are defined,
+00014a90: 2066 6f72 2074 6869 7320 7377 6974 6368   for this switch
+00014aa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014ab0: 2069 6620 7377 6974 6368 5f6e 6f64 6573   if switch_nodes
+00014ac0: 5b31 3a5d 3a0a 2020 2020 2020 2020 2020  [1:]:.          
+00014ad0: 2020 2020 2020 2020 2020 666f 7220 6e6f            for no
+00014ae0: 6465 5f6e 616d 6520 696e 2073 7769 7463  de_name in switc
+00014af0: 685f 6e6f 6465 735b 313a 5d3a 0a20 2020  h_nodes[1:]:.   
+00014b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014b10: 2020 2020 206e 6f64 6520 3d20 6665 7463       node = fetc
+00014b20: 685f 6e6f 6465 5f62 795f 6e61 6d65 2869  h_node_by_name(i
+00014b30: 645f 7369 6d75 6c61 7469 6f6e 2c20 6e6f  d_simulation, no
+00014b40: 6465 5f6e 616d 6529 0a0a 2020 2020 2020  de_name)..      
+00014b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014b60: 2020 666f 7220 6e65 7477 6f72 6b5f 696e    for network_in
+00014b70: 7465 7266 6163 6520 696e 206e 6f64 655b  terface in node[
+00014b80: 226e 6574 776f 726b 5f69 6e74 6572 6661  "network_interfa
+00014b90: 6365 7322 5d3a 0a20 2020 2020 2020 2020  ces"]:.         
+00014ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014bb0: 2020 2069 6620 6e65 7477 6f72 6b5f 696e     if network_in
+00014bc0: 7465 7266 6163 655b 2273 7769 7463 685f  terface["switch_
+00014bd0: 6e61 6d65 225d 203d 3d20 7377 6974 6368  name"] == switch
+00014be0: 5b22 6e61 6d65 225d 3a0a 2020 2020 2020  ["name"]:.      
+00014bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014c00: 2020 2020 2020 2020 2020 6e65 7477 6f72            networ
+00014c10: 6b5f 696e 7465 7266 6163 6573 2e61 7070  k_interfaces.app
+00014c20: 656e 6428 0a20 2020 2020 2020 2020 2020  end(.           
+00014c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014c40: 2020 2020 2020 2020 206e 6574 776f 726b           network
+00014c50: 5f69 6e74 6572 6661 6365 5b22 6d61 635f  _interface["mac_
+00014c60: 6164 6472 6573 7322 5d0a 2020 2020 2020  address"].      
+00014c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014c80: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00014c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ca0: 2020 2020 2020 2020 2020 2020 6272 6561              brea
+00014cb0: 6b0a 2020 2020 2020 2020 2020 2020 2020  k.              
+00014cc0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00014cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ce0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00014cf0: 6520 4578 6365 7074 696f 6e28 0a20 2020  e Exception(.   
+00014d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014d10: 2020 2020 2020 2020 2020 2020 2022 5468               "Th
+00014d20: 6520 6e6f 6465 2027 7b7d 2720 6973 6e27  e node '{}' isn'
+00014d30: 7420 6c69 6e6b 6564 2077 6974 6820 7468  t linked with th
+00014d40: 6520 7377 6974 6368 2027 7b7d 2722 2e66  e switch '{}'".f
+00014d50: 6f72 6d61 7428 0a20 2020 2020 2020 2020  ormat(.         
+00014d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014d70: 2020 2020 2020 2020 2020 206e 6f64 655f             node_
+00014d80: 6e61 6d65 2c20 7377 6974 6368 5b22 6e61  name, switch["na
+00014d90: 6d65 225d 0a20 2020 2020 2020 2020 2020  me"].           
+00014da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014db0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00014dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014dd0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00014de0: 2020 2020 2023 2045 6c73 652c 2063 6f6e       # Else, con
+00014df0: 7369 6465 7220 616c 6c20 6e6f 6465 7320  sider all nodes 
+00014e00: 636f 6e6e 6563 7465 6420 746f 2074 6865  connected to the
+00014e10: 2073 7769 7463 680a 2020 2020 2020 2020   switch.        
+00014e20: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00014e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e40: 2020 666f 7220 6e6f 6465 2069 6e20 6665    for node in fe
+00014e50: 7463 685f 6e6f 6465 7328 6964 5f73 696d  tch_nodes(id_sim
+00014e60: 756c 6174 696f 6e29 3a0a 2020 2020 2020  ulation):.      
+00014e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e80: 2020 6966 206e 6f64 655b 2274 7970 6522    if node["type"
+00014e90: 5d20 213d 2022 726f 7574 6572 223a 0a20  ] != "router":. 
+00014ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014eb0: 2020 2020 2020 2020 2020 2066 6f72 206e             for n
+00014ec0: 6574 776f 726b 5f69 6e74 6572 6661 6365  etwork_interface
+00014ed0: 2069 6e20 6e6f 6465 5b22 6e65 7477 6f72   in node["networ
+00014ee0: 6b5f 696e 7465 7266 6163 6573 225d 3a0a  k_interfaces"]:.
+00014ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f10: 6966 206e 6574 776f 726b 5f69 6e74 6572  if network_inter
+00014f20: 6661 6365 5b22 7377 6974 6368 5f6e 616d  face["switch_nam
+00014f30: 6522 5d20 3d3d 2073 7769 7463 685b 226e  e"] == switch["n
+00014f40: 616d 6522 5d3a 0a20 2020 2020 2020 2020  ame"]:.         
+00014f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f60: 2020 2020 2020 2020 2020 206e 6574 776f             netwo
+00014f70: 726b 5f69 6e74 6572 6661 6365 732e 6170  rk_interfaces.ap
+00014f80: 7065 6e64 280a 2020 2020 2020 2020 2020  pend(.          
+00014f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014fa0: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
+00014fb0: 7477 6f72 6b5f 696e 7465 7266 6163 655b  twork_interface[
+00014fc0: 226d 6163 5f61 6464 7265 7373 225d 0a20  "mac_address"]. 
+00014fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ff0: 2020 2029 0a0a 2020 2020 2020 2020 6966     )..        if
+00015000: 2073 696d 755f 6e6f 6465 735b 226e 6f64   simu_nodes["nod
+00015010: 6573 225d 2069 7320 6e6f 7420 4e6f 6e65  es"] is not None
+00015020: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+00015030: 4d69 7272 6f72 2074 7261 6666 6963 206f  Mirror traffic o
+00015040: 6e20 616c 6c20 696e 7465 7266 6163 6573  n all interfaces
+00015050: 2066 726f 6d20 7468 6520 7370 6563 6966   from the specif
+00015060: 6965 6420 6e6f 6465 730a 2020 2020 2020  ied nodes.      
+00015070: 2020 2020 2020 666f 7220 6e6f 6465 5f6e        for node_n
+00015080: 616d 6520 696e 2073 696d 755f 6e6f 6465  ame in simu_node
+00015090: 735b 226e 6f64 6573 225d 3a0a 2020 2020  s["nodes"]:.    
+000150a0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000150b0: 6e65 7477 6f72 6b5f 696e 7465 7266 6163  network_interfac
+000150c0: 6520 696e 2066 6574 6368 5f6e 6f64 655f  e in fetch_node_
+000150d0: 6279 5f6e 616d 6528 6964 5f73 696d 756c  by_name(id_simul
+000150e0: 6174 696f 6e2c 206e 6f64 655f 6e61 6d65  ation, node_name
+000150f0: 295b 0a20 2020 2020 2020 2020 2020 2020  )[.             
+00015100: 2020 2020 2020 2022 6e65 7477 6f72 6b5f         "network_
+00015110: 696e 7465 7266 6163 6573 220a 2020 2020  interfaces".    
+00015120: 2020 2020 2020 2020 2020 2020 5d3a 0a20              ]:. 
+00015130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015140: 2020 206e 6574 776f 726b 5f69 6e74 6572     network_inter
+00015150: 6661 6365 732e 6170 7065 6e64 286e 6574  faces.append(net
+00015160: 776f 726b 5f69 6e74 6572 6661 6365 5b22  work_interface["
+00015170: 6d61 635f 6164 6472 6573 7322 5d29 0a0a  mac_address"])..
+00015180: 2020 2020 7072 6f62 655f 6964 203d 2063      probe_id = c
+00015190: 7265 6174 655f 7072 6f62 6528 0a20 2020  reate_probe(.   
+000151a0: 2020 2020 2069 645f 7369 6d75 6c61 7469       id_simulati
+000151b0: 6f6e 2c20 6e65 7477 6f72 6b5f 696e 7465  on, network_inte
+000151c0: 7266 6163 6573 2c20 6966 6163 652c 2070  rfaces, iface, p
+000151d0: 6361 702c 2066 696c 7465 722c 2064 6972  cap, filter, dir
+000151e0: 6563 7469 6f6e 0a20 2020 2029 0a0a 2020  ection.    )..  
+000151f0: 2020 7265 7475 726e 2070 726f 6265 5f69    return probe_i
+00015200: 640a 0a0a 6465 6620 6e65 745f 7374 6172  d...def net_star
+00015210: 745f 7072 6f62 6528 6964 5f73 696d 756c  t_probe(id_simul
+00015220: 6174 696f 6e3a 2069 6e74 2c20 7072 6f62  ation: int, prob
+00015230: 655f 6964 3a20 696e 7429 202d 3e20 4e6f  e_id: int) -> No
+00015240: 6e65 3a0a 2020 2020 2222 2252 6564 6972  ne:.    """Redir
+00015250: 6563 7420 6e65 7477 6f72 6b20 7472 6166  ect network traf
+00015260: 6669 6320 746f 2074 6865 2070 726f 6265  fic to the probe
+00015270: 2069 6e74 6572 6661 6365 2e0a 0a20 2020   interface...   
+00015280: 203a 7061 7261 6d20 6964 5f73 696d 756c   :param id_simul
+00015290: 6174 696f 6e3a 2054 6865 2073 696d 756c  ation: The simul
+000152a0: 6174 696f 6e20 4944 2e0a 2020 2020 3a70  ation ID..    :p
+000152b0: 6172 616d 2070 726f 6265 5f69 643a 2054  aram probe_id: T
+000152c0: 6865 2070 726f 6265 2049 442e 0a0a 2020  he probe ID...  
+000152d0: 2020 2222 220a 0a20 2020 2072 6573 756c    """..    resul
+000152e0: 7420 3d20 5f67 6574 2866 222f 7369 6d75  t = _get(f"/simu
+000152f0: 6c61 7469 6f6e 2f7b 6964 5f73 696d 756c  lation/{id_simul
+00015300: 6174 696f 6e7d 2f70 726f 6265 2f7b 7072  ation}/probe/{pr
+00015310: 6f62 655f 6964 7d22 290a 0a20 2020 2069  obe_id}")..    i
+00015320: 6620 7265 7375 6c74 2e73 7461 7475 735f  f result.status_
+00015330: 636f 6465 2021 3d20 3230 303a 0a20 2020  code != 200:.   
+00015340: 2020 2020 205f 6861 6e64 6c65 5f65 7272       _handle_err
+00015350: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
+00015360: 7265 7375 6c74 2c20 2243 616e 6e6f 7420  result, "Cannot 
+00015370: 6163 7469 7661 7465 206e 6574 776f 726b  activate network
+00015380: 2074 7261 6666 6963 2072 6564 6972 6563   traffic redirec
+00015390: 7469 6f6e 2066 726f 6d20 4954 2053 696d  tion from IT Sim
+000153a0: 756c 6174 696f 6e20 4150 4922 0a20 2020  ulation API".   
+000153b0: 2020 2020 2029 0a0a 0a64 6566 206e 6574       )...def net
+000153c0: 5f73 746f 705f 7072 6f62 6528 6964 5f73  _stop_probe(id_s
+000153d0: 696d 756c 6174 696f 6e3a 2069 6e74 2c20  imulation: int, 
+000153e0: 7072 6f62 655f 6964 3a20 696e 7429 202d  probe_id: int) -
+000153f0: 3e20 4e6f 6e65 3a0a 2020 2020 2222 2253  > None:.    """S
+00015400: 746f 7020 7265 6469 7265 6374 696f 6e20  top redirection 
+00015410: 6f66 206e 6574 776f 726b 2074 7261 6666  of network traff
+00015420: 6963 2074 6f20 7468 6520 7072 6f62 6520  ic to the probe 
+00015430: 696e 7465 7266 6163 652e 0a0a 2020 2020  interface...    
+00015440: 3a70 6172 616d 2069 645f 7369 6d75 6c61  :param id_simula
+00015450: 7469 6f6e 3a20 5468 6520 7369 6d75 6c61  tion: The simula
+00015460: 7469 6f6e 2049 442e 0a20 2020 203a 7061  tion ID..    :pa
+00015470: 7261 6d20 7072 6f62 655f 6964 3a20 5468  ram probe_id: Th
+00015480: 6520 7072 6f62 6520 4944 2e0a 0a20 2020  e probe ID...   
+00015490: 2022 2222 0a0a 2020 2020 7265 7375 6c74   """..    result
+000154a0: 203d 205f 6765 7428 6622 2f73 696d 756c   = _get(f"/simul
+000154b0: 6174 696f 6e2f 7b69 645f 7369 6d75 6c61  ation/{id_simula
+000154c0: 7469 6f6e 7d2f 7374 6f70 5f70 726f 6265  tion}/stop_probe
+000154d0: 2f7b 7072 6f62 655f 6964 7d22 290a 0a20  /{probe_id}").. 
+000154e0: 2020 2069 6620 7265 7375 6c74 2e73 7461     if result.sta
+000154f0: 7475 735f 636f 6465 2021 3d20 3230 303a  tus_code != 200:
+00015500: 0a20 2020 2020 2020 205f 6861 6e64 6c65  .        _handle
+00015510: 5f65 7272 6f72 280a 2020 2020 2020 2020  _error(.        
+00015520: 2020 2020 7265 7375 6c74 2c20 2243 616e      result, "Can
+00015530: 6e6f 7420 7374 6f70 206e 6574 776f 726b  not stop network
+00015540: 2074 7261 6666 6963 2072 6564 6972 6563   traffic redirec
+00015550: 7469 6f6e 2066 726f 6d20 4954 2053 696d  tion from IT Sim
+00015560: 756c 6174 696f 6e20 4150 4922 0a20 2020  ulation API".   
+00015570: 2020 2020 2029 0a0a 0a64 6566 2066 6574       )...def fet
+00015580: 6368 5f6c 6973 745f 7072 6f62 6573 2869  ch_list_probes(i
+00015590: 645f 7369 6d75 6c61 7469 6f6e 3a20 696e  d_simulation: in
+000155a0: 7429 202d 3e20 4469 6374 3a0a 2020 2020  t) -> Dict:.    
+000155b0: 2222 2252 6574 7572 6e20 7468 6520 6c69  """Return the li
+000155c0: 7374 206f 6620 7072 6f62 6573 2077 6974  st of probes wit
+000155d0: 6820 7468 6569 7220 6461 7461 0a0a 2020  h their data..  
+000155e0: 2020 3a70 6172 616d 2069 645f 7369 6d75    :param id_simu
+000155f0: 6c61 7469 6f6e 3a20 5468 6520 7369 6d75  lation: The simu
+00015600: 6c61 7469 6f6e 2049 442e 0a0a 2020 2020  lation ID...    
+00015610: 3a72 6574 7572 6e3a 2041 206c 6973 7420  :return: A list 
+00015620: 6f66 2070 726f 6265 7320 7769 7468 2074  of probes with t
+00015630: 6865 6972 2064 6174 612e 0a20 2020 2022  heir data..    "
+00015640: 2222 0a0a 2020 2020 7265 7375 6c74 203d  ""..    result =
+00015650: 207b 7d0a 0a20 2020 2070 726f 6265 7320   {}..    probes 
+00015660: 3d20 6665 7463 685f 7072 6f62 6573 2869  = fetch_probes(i
+00015670: 645f 7369 6d75 6c61 7469 6f6e 290a 2020  d_simulation).  
+00015680: 2020 666f 7220 7072 6f62 6520 696e 2070    for probe in p
+00015690: 726f 6265 733a 0a20 2020 2020 2020 2072  robes:.        r
+000156a0: 6573 756c 745b 7072 6f62 655b 2269 6422  esult[probe["id"
+000156b0: 5d5d 203d 207b 0a20 2020 2020 2020 2020  ]] = {.         
+000156c0: 2020 2022 636f 6c6c 6563 7469 6e67 5f70     "collecting_p
+000156d0: 6f69 6e74 7322 3a20 6665 7463 685f 7072  oints": fetch_pr
+000156e0: 6f62 655f 636f 6c6c 6563 7469 6e67 5f70  obe_collecting_p
+000156f0: 6f69 6e74 7328 6964 5f73 696d 756c 6174  oints(id_simulat
+00015700: 696f 6e2c 2070 726f 6265 292c 0a20 2020  ion, probe),.   
+00015710: 2020 2020 2020 2020 2022 6966 6163 6522           "iface"
+00015720: 3a20 7072 6f62 655b 2269 6661 6365 225d  : probe["iface"]
+00015730: 2c0a 2020 2020 2020 2020 2020 2020 2270  ,.            "p
+00015740: 6361 7022 3a20 7072 6f62 655b 2270 6361  cap": probe["pca
+00015750: 7022 5d2c 0a20 2020 2020 2020 2020 2020  p"],.           
+00015760: 2022 6669 6c74 6572 223a 2070 726f 6265   "filter": probe
+00015770: 5b22 6669 6c74 6572 225d 2c0a 2020 2020  ["filter"],.    
+00015780: 2020 2020 2020 2020 2263 6170 7475 7265          "capture
+00015790: 5f69 6e5f 7072 6f67 7265 7373 223a 2070  _in_progress": p
+000157a0: 726f 6265 5b22 6361 7074 7572 655f 696e  robe["capture_in
+000157b0: 5f70 726f 6772 6573 7322 5d2c 0a20 2020  _progress"],.   
+000157c0: 2020 2020 2020 2020 2022 6469 7265 6374           "direct
+000157d0: 696f 6e22 3a20 7072 6f62 655b 2264 6972  ion": probe["dir
+000157e0: 6563 7469 6f6e 225d 2c0a 2020 2020 2020  ection"],.      
+000157f0: 2020 7d0a 0a20 2020 2072 6574 7572 6e20    }..    return 
+00015800: 7265 7375 6c74 0a0a 0a64 6566 2066 6574  result...def fet
+00015810: 6368 5f70 726f 6265 5f63 6f6c 6c65 6374  ch_probe_collect
+00015820: 696e 675f 706f 696e 7473 2869 645f 7369  ing_points(id_si
+00015830: 6d75 6c61 7469 6f6e 3a20 696e 742c 2070  mulation: int, p
+00015840: 726f 6265 3a20 4469 6374 2920 2d3e 2041  robe: Dict) -> A
+00015850: 6e79 3a0a 2020 2020 2222 2252 6574 7572  ny:.    """Retur
+00015860: 6e20 7468 6520 6c69 7374 206f 6620 636f  n the list of co
+00015870: 6c6c 6563 7469 6e67 2070 6f69 6e74 7320  llecting points 
+00015880: 7573 6564 2074 6f20 6361 7074 7572 6520  used to capture 
+00015890: 7468 6520 6e65 7477 6f72 6b20 7472 6166  the network traf
+000158a0: 6669 6320 746f 2061 2067 6976 656e 2070  fic to a given p
+000158b0: 726f 6265 206f 6620 6120 7369 6d75 6c61  robe of a simula
+000158c0: 7469 6f6e 2e0a 0a20 2020 203a 7061 7261  tion...    :para
+000158d0: 6d20 6964 5f73 696d 756c 6174 696f 6e3a  m id_simulation:
+000158e0: 2054 6865 2073 696d 756c 6174 696f 6e20   The simulation 
+000158f0: 4944 2e0a 2020 2020 3a70 6172 616d 2070  ID..    :param p
+00015900: 726f 6265 3a20 5468 6520 6769 7665 6e20  robe: The given 
+00015910: 7072 6f62 6520 6f66 2074 6865 2073 696d  probe of the sim
+00015920: 756c 6174 696f 6e2e 0a0a 2020 2020 3a74  ulation...    :t
+00015930: 7970 6520 7072 6f62 653a 203a 636c 6173  ype probe: :clas
+00015940: 733a 6063 6c61 7373 603a 6044 6963 7460  s:`class`:`Dict`
+00015950: 2c20 6578 203a 207b 2769 6661 6365 273a  , ex : {'iface':
+00015960: 2027 6475 6d6d 7930 272c 2027 6964 273a   'dummy0', 'id':
+00015970: 2031 2c20 2770 6361 7027 3a20 5472 7565   1, 'pcap': True
+00015980: 2c20 2763 6170 7475 7265 5f69 6e5f 7072  , 'capture_in_pr
+00015990: 6f67 7265 7373 273a 2046 616c 7365 2c20  ogress': False, 
+000159a0: 2766 696c 7465 7227 3a20 2774 6370 2070  'filter': 'tcp p
+000159b0: 6f72 7420 3830 272c 2027 7369 6d75 6c61  ort 80', 'simula
+000159c0: 7469 6f6e 5f69 6427 3a20 312c 2027 6e65  tion_id': 1, 'ne
+000159d0: 7477 6f72 6b5f 696e 7465 7266 6163 6573  twork_interfaces
+000159e0: 273a 205b 2730 303a 3231 3a61 313a 3037  ': ['00:21:a1:07
+000159f0: 3a37 643a 6265 275d 2c20 2764 6972 6563  :7d:be'], 'direc
+00015a00: 7469 6f6e 273a 2027 696e 6772 6573 7327  tion': 'ingress'
+00015a10: 7d0a 0a20 2020 2022 2222 0a0a 2020 2020  }..    """..    
+00015a20: 636f 6c6c 6563 7469 6e67 5f70 6f69 6e74  collecting_point
+00015a30: 7320 3d20 7b22 7377 6974 6368 7322 3a20  s = {"switchs": 
+00015a40: 7b7d 2c20 226e 6f64 6573 223a 205b 5d7d  {}, "nodes": []}
+00015a50: 0a0a 2020 2020 6e65 7477 6f72 6b5f 696e  ..    network_in
+00015a60: 7465 7266 6163 6573 203d 205b 0a20 2020  terfaces = [.   
+00015a70: 2020 2020 2066 6574 6368 5f6e 6574 776f       fetch_netwo
+00015a80: 726b 5f69 6e74 6572 6661 6365 5f62 795f  rk_interface_by_
+00015a90: 6d61 6328 6964 5f73 696d 756c 6174 696f  mac(id_simulatio
+00015aa0: 6e2c 206e 290a 2020 2020 2020 2020 666f  n, n).        fo
+00015ab0: 7220 6e20 696e 2070 726f 6265 5b22 6e65  r n in probe["ne
+00015ac0: 7477 6f72 6b5f 696e 7465 7266 6163 6573  twork_interfaces
+00015ad0: 225d 0a20 2020 205d 0a0a 2020 2020 6e6f  "].    ]..    no
+00015ae0: 6465 735f 746f 5f63 6170 7475 7265 203d  des_to_capture =
+00015af0: 205b 5d0a 2020 2020 666f 7220 6e65 7477   [].    for netw
+00015b00: 6f72 6b5f 696e 7465 7266 6163 6520 696e  ork_interface in
+00015b10: 206e 6574 776f 726b 5f69 6e74 6572 6661   network_interfa
+00015b20: 6365 733a 0a20 2020 2020 2020 206e 6f64  ces:.        nod
+00015b30: 6520 3d20 6665 7463 685f 6e6f 6465 286e  e = fetch_node(n
+00015b40: 6574 776f 726b 5f69 6e74 6572 6661 6365  etwork_interface
+00015b50: 5b22 6e6f 6465 5f69 6422 5d29 0a20 2020  ["node_id"]).   
+00015b60: 2020 2020 2069 6620 6e6f 6465 206e 6f74       if node not
+00015b70: 2069 6e20 6e6f 6465 735f 746f 5f63 6170   in nodes_to_cap
+00015b80: 7475 7265 3a0a 2020 2020 2020 2020 2020  ture:.          
+00015b90: 2020 6e6f 6465 735f 746f 5f63 6170 7475    nodes_to_captu
+00015ba0: 7265 2e61 7070 656e 6428 6e6f 6465 290a  re.append(node).
+00015bb0: 0a20 2020 2023 2052 6574 7572 6e20 4e6f  .    # Return No
+00015bc0: 6e65 2069 6620 7468 6572 6520 6973 206e  ne if there is n
+00015bd0: 6f74 6869 6e67 2074 6f20 6361 7074 7572  othing to captur
+00015be0: 650a 2020 2020 6966 206e 6f64 6573 5f74  e.    if nodes_t
+00015bf0: 6f5f 6361 7074 7572 6520 3d3d 205b 5d3a  o_capture == []:
+00015c00: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00015c10: 4e6f 6e65 0a0a 2020 2020 2320 5265 7475  None..    # Retu
+00015c20: 726e 207b 7d20 6966 2065 7665 7279 206e  rn {} if every n
+00015c30: 6f64 6520 6d75 7374 2062 6520 6361 7074  ode must be capt
+00015c40: 7572 6564 0a20 2020 2069 6620 6c65 6e28  ured.    if len(
+00015c50: 6e65 7477 6f72 6b5f 696e 7465 7266 6163  network_interfac
+00015c60: 6573 2920 3d3d 206c 656e 280a 2020 2020  es) == len(.    
+00015c70: 2020 2020 6665 7463 685f 7369 6d75 6c61      fetch_simula
+00015c80: 7469 6f6e 5f6e 6574 776f 726b 5f69 6e74  tion_network_int
+00015c90: 6572 6661 6365 7328 6964 5f73 696d 756c  erfaces(id_simul
+00015ca0: 6174 696f 6e29 0a20 2020 2029 3a0a 2020  ation).    ):.  
+00015cb0: 2020 2020 2020 7265 7475 726e 207b 7d0a        return {}.
+00015cc0: 0a20 2020 2066 6f72 206e 6f64 6520 696e  .    for node in
+00015cd0: 206e 6f64 6573 5f74 6f5f 6361 7074 7572   nodes_to_captur
+00015ce0: 653a 0a20 2020 2020 2020 2023 2049 6620  e:.        # If 
+00015cf0: 6576 6572 7920 6e65 7477 6f72 6b5f 696e  every network_in
+00015d00: 7465 7266 6163 6520 6672 6f6d 2061 206e  terface from a n
+00015d10: 6f64 6520 6973 2063 6170 7475 7265 642c  ode is captured,
+00015d20: 2069 7420 676f 6573 2074 6f20 7468 6520   it goes to the 
+00015d30: 226e 6f64 6573 2220 6469 6374 0a20 2020  "nodes" dict.   
+00015d40: 2020 2020 2063 6170 7475 7265 5f61 6c6c       capture_all
+00015d50: 5f6e 6574 776f 726b 5f69 6e74 6572 6661  _network_interfa
+00015d60: 6365 7320 3d20 5472 7565 0a20 2020 2020  ces = True.     
+00015d70: 2020 2066 6f72 206e 6f64 655f 6e65 7477     for node_netw
+00015d80: 6f72 6b5f 696e 7465 7266 6163 6520 696e  ork_interface in
+00015d90: 206e 6f64 655b 226e 6574 776f 726b 5f69   node["network_i
+00015da0: 6e74 6572 6661 6365 7322 5d3a 0a20 2020  nterfaces"]:.   
+00015db0: 2020 2020 2020 2020 2063 6170 7475 7265           capture
+00015dc0: 5f61 6c6c 5f6e 6574 776f 726b 5f69 6e74  _all_network_int
+00015dd0: 6572 6661 6365 7320 3d20 6361 7074 7572  erfaces = captur
+00015de0: 655f 616c 6c5f 6e65 7477 6f72 6b5f 696e  e_all_network_in
+00015df0: 7465 7266 6163 6573 2061 6e64 2028 0a20  terfaces and (. 
+00015e00: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00015e10: 6f64 655f 6e65 7477 6f72 6b5f 696e 7465  ode_network_inte
+00015e20: 7266 6163 6520 696e 206e 6574 776f 726b  rface in network
+00015e30: 5f69 6e74 6572 6661 6365 730a 2020 2020  _interfaces.    
+00015e40: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00015e50: 2020 2069 6620 6361 7074 7572 655f 616c     if capture_al
+00015e60: 6c5f 6e65 7477 6f72 6b5f 696e 7465 7266  l_network_interf
+00015e70: 6163 6573 3a0a 2020 2020 2020 2020 2020  aces:.          
+00015e80: 2020 636f 6c6c 6563 7469 6e67 5f70 6f69    collecting_poi
+00015e90: 6e74 735b 226e 6f64 6573 225d 2e61 7070  nts["nodes"].app
+00015ea0: 656e 6428 6e6f 6465 5b22 6e61 6d65 225d  end(node["name"]
+00015eb0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+00015ec0: 2020 2020 2020 2020 2020 2020 2320 456c              # El
+00015ed0: 7365 2c20 6974 2067 6f65 7320 746f 2074  se, it goes to t
+00015ee0: 6865 2022 7377 6974 6368 7322 2064 6963  he "switchs" dic
+00015ef0: 740a 2020 2020 2020 2020 2020 2020 666f  t.            fo
+00015f00: 7220 6e6f 6465 5f6e 6574 776f 726b 5f69  r node_network_i
+00015f10: 6e74 6572 6661 6365 2069 6e20 6e6f 6465  nterface in node
+00015f20: 5b22 6e65 7477 6f72 6b5f 696e 7465 7266  ["network_interf
+00015f30: 6163 6573 225d 3a0a 2020 2020 2020 2020  aces"]:.        
+00015f40: 2020 2020 2020 2020 6966 206e 6f64 655f          if node_
+00015f50: 6e65 7477 6f72 6b5f 696e 7465 7266 6163  network_interfac
+00015f60: 6520 696e 206e 6574 776f 726b 5f69 6e74  e in network_int
+00015f70: 6572 6661 6365 733a 0a20 2020 2020 2020  erfaces:.       
+00015f80: 2020 2020 2020 2020 2020 2020 2073 7769               swi
+00015f90: 7463 6820 3d20 7b22 6e61 6d65 223a 206e  tch = {"name": n
+00015fa0: 6f64 655f 6e65 7477 6f72 6b5f 696e 7465  ode_network_inte
+00015fb0: 7266 6163 655b 2273 7769 7463 685f 6e61  rface["switch_na
+00015fc0: 6d65 225d 7d0a 0a20 2020 2020 2020 2020  me"]}..         
+00015fd0: 2020 2020 2020 2020 2020 2069 6620 7377             if sw
+00015fe0: 6974 6368 5b22 6e61 6d65 225d 206e 6f74  itch["name"] not
+00015ff0: 2069 6e20 636f 6c6c 6563 7469 6e67 5f70   in collecting_p
+00016000: 6f69 6e74 735b 2273 7769 7463 6873 225d  oints["switchs"]
+00016010: 2e6b 6579 7328 293a 0a20 2020 2020 2020  .keys():.       
+00016020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016030: 2063 6f6c 6c65 6374 696e 675f 706f 696e   collecting_poin
+00016040: 7473 5b22 7377 6974 6368 7322 5d5b 7377  ts["switchs"][sw
+00016050: 6974 6368 5b22 6e61 6d65 225d 5d20 3d20  itch["name"]] = 
+00016060: 5b5d 0a20 2020 2020 2020 2020 2020 2020  [].             
+00016070: 2020 2020 2020 2063 6f6c 6c65 6374 696e         collectin
+00016080: 675f 706f 696e 7473 5b22 7377 6974 6368  g_points["switch
+00016090: 7322 5d5b 7377 6974 6368 5b22 6e61 6d65  s"][switch["name
+000160a0: 225d 5d2e 6170 7065 6e64 286e 6f64 655b  "]].append(node[
+000160b0: 226e 616d 6522 5d29 0a0a 2020 2020 7265  "name"])..    re
+000160c0: 7475 726e 2063 6f6c 6c65 6374 696e 675f  turn collecting_
+000160d0: 706f 696e 7473 0a0a 0a64 6566 2073 6e61  points...def sna
+000160e0: 7073 686f 745f 7369 6d75 6c61 7469 6f6e  pshot_simulation
+000160f0: 2869 645f 7369 6d75 6c61 7469 6f6e 3a20  (id_simulation: 
+00016100: 696e 7429 202d 3e20 7374 723a 0a20 2020  int) -> str:.   
+00016110: 2022 2222 4372 6561 7465 2061 2073 6e61   """Create a sna
+00016120: 7073 686f 7420 6f66 2061 2073 696d 756c  pshot of a simul
+00016130: 6174 696f 6e2e 0a0a 2020 2020 416c 6c20  ation...    All 
+00016140: 7468 6520 6669 6c65 7320 7769 6c6c 2062  the files will b
+00016150: 6520 7374 6f72 6564 2074 6f0a 2020 2020  e stored to.    
+00016160: 2f63 7962 6572 2d72 616e 6765 2d63 6174  /cyber-range-cat
+00016170: 616c 6f67 2f73 696d 756c 6174 696f 6e73  alog/simulations
+00016180: 2f3c 6861 7368 2063 616d 7061 6967 6e3e  /<hash campaign>
+00016190: 2f3c 7469 6d65 7374 616d 703e 2f0a 0a20  /<timestamp>/.. 
+000161a0: 2020 203a 7265 7475 726e 3a20 5468 6520     :return: The 
+000161b0: 7061 7468 2077 6865 7265 2074 6865 2074  path where the t
+000161c0: 6f70 6f6c 6f67 7920 6669 6c65 2077 696c  opology file wil
+000161d0: 6c20 6265 2073 746f 7265 642e 0a0a 2020  l be stored...  
+000161e0: 2020 3a70 6172 616d 2069 645f 7369 6d75    :param id_simu
+000161f0: 6c61 7469 6f6e 3a20 5468 6520 7369 6d75  lation: The simu
+00016200: 6c61 7469 6f6e 2049 442e 0a0a 2020 2020  lation ID...    
+00016210: 2222 220a 0a20 2020 2023 2073 696d 755f  """..    # simu_
+00016220: 736e 6170 2063 616e 206f 6e6c 7920 6265  snap can only be
+00016230: 2064 6f6e 6520 6f6e 2061 2052 554e 4e49   done on a RUNNI
+00016240: 4e47 2073 696d 756c 6174 696f 6e0a 2020  NG simulation.  
+00016250: 2020 6966 2073 696d 756c 6174 696f 6e5f    if simulation_
+00016260: 7374 6174 7573 2869 645f 7369 6d75 6c61  status(id_simula
+00016270: 7469 6f6e 2920 213d 2022 5255 4e4e 494e  tion) != "RUNNIN
+00016280: 4722 3a0a 2020 2020 2020 2020 7261 6973  G":.        rais
+00016290: 6520 4578 6365 7074 696f 6e28 0a20 2020  e Exception(.   
+000162a0: 2020 2020 2020 2020 2022 4361 6e6e 6f74           "Cannot
+000162b0: 2063 7265 6174 6520 6120 736e 6170 7368   create a snapsh
+000162c0: 6f74 206f 6620 7468 6520 7369 6d75 6c61  ot of the simula
+000162d0: 7469 6f6e 2c20 6173 2074 6865 2073 696d  tion, as the sim
+000162e0: 756c 6174 696f 6e20 277b 7d27 2069 7320  ulation '{}' is 
+000162f0: 220a 2020 2020 2020 2020 2020 2020 226e  ".            "n
+00016300: 6f74 2072 756e 6e69 6e67 222e 666f 726d  ot running".form
+00016310: 6174 2869 645f 7369 6d75 6c61 7469 6f6e  at(id_simulation
+00016320: 290a 2020 2020 2020 2020 290a 0a20 2020  ).        )..   
+00016330: 2023 2043 616c 6c20 736e 6170 7368 6f74   # Call snapshot
+00016340: 2041 5049 0a20 2020 2072 6573 756c 7420   API.    result 
+00016350: 3d20 5f70 6f73 7428 6622 2f73 696d 756c  = _post(f"/simul
+00016360: 6174 696f 6e2f 7b69 645f 7369 6d75 6c61  ation/{id_simula
+00016370: 7469 6f6e 7d2f 736e 6170 7368 6f74 2229  tion}/snapshot")
+00016380: 0a20 2020 2069 6620 7265 7375 6c74 2e73  .    if result.s
+00016390: 7461 7475 735f 636f 6465 2021 3d20 3230  tatus_code != 20
+000163a0: 303a 0a20 2020 2020 2020 205f 6861 6e64  0:.        _hand
+000163b0: 6c65 5f65 7272 6f72 2872 6573 756c 742c  le_error(result,
+000163c0: 2022 4572 726f 7220 7768 696c 6520 6372   "Error while cr
+000163d0: 6561 7469 6e67 2073 6e61 7073 686f 7422  eating snapshot"
+000163e0: 290a 0a20 2020 2079 616d 6c3a 2073 7472  )..    yaml: str
+000163f0: 203d 2072 6573 756c 742e 6a73 6f6e 2829   = result.json()
+00016400: 0a0a 2020 2020 6c6f 6767 6572 2e69 6e66  ..    logger.inf
+00016410: 6f28 6622 5b2b 5d20 5374 6172 7469 6e67  o(f"[+] Starting
+00016420: 2074 6865 2073 6e61 7073 686f 7420 6f66   the snapshot of
+00016430: 2073 696d 756c 6174 696f 6e20 7b69 645f   simulation {id_
+00016440: 7369 6d75 6c61 7469 6f6e 7d2e 2e2e 2229  simulation}...")
+00016450: 0a20 2020 2077 6869 6c65 2073 696d 756c  .    while simul
+00016460: 6174 696f 6e5f 7374 6174 7573 2869 645f  ation_status(id_
+00016470: 7369 6d75 6c61 7469 6f6e 2920 213d 2022  simulation) != "
+00016480: 534e 4150 5348 4f54 223a 0a20 2020 2020  SNAPSHOT":.     
+00016490: 2020 2074 696d 652e 736c 6565 7028 3129     time.sleep(1)
+000164a0: 0a0a 2020 2020 2020 2020 7369 6d75 6c61  ..        simula
+000164b0: 7469 6f6e 5f64 6963 7420 3d20 6665 7463  tion_dict = fetc
+000164c0: 685f 7369 6d75 6c61 7469 6f6e 2869 645f  h_simulation(id_
+000164d0: 7369 6d75 6c61 7469 6f6e 290a 2020 2020  simulation).    
+000164e0: 2020 2020 6375 7272 656e 745f 7374 6174      current_stat
+000164f0: 7573 203d 2073 696d 756c 6174 696f 6e5f  us = simulation_
+00016500: 6469 6374 5b22 7374 6174 7573 225d 0a20  dict["status"]. 
+00016510: 2020 2020 2020 2069 6620 6375 7272 656e         if curren
+00016520: 745f 7374 6174 7573 203d 3d20 2245 5252  t_status == "ERR
+00016530: 4f52 223a 0a20 2020 2020 2020 2020 2020  OR":.           
+00016540: 2065 7272 6f72 5f6d 6573 7361 6765 203d   error_message =
+00016550: 2073 696d 756c 6174 696f 6e5f 6469 6374   simulation_dict
+00016560: 5b22 6572 726f 725f 6d73 6722 5d0a 2020  ["error_msg"].  
+00016570: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00016580: 4578 6365 7074 696f 6e28 0a20 2020 2020  Exception(.     
+00016590: 2020 2020 2020 2020 2020 2022 4572 726f             "Erro
+000165a0: 7220 6475 7269 6e67 2073 696d 756c 6174  r during simulat
+000165b0: 696f 6e20 736e 6170 7368 6f74 3a20 277b  ion snapshot: '{
+000165c0: 7d27 222e 666f 726d 6174 2865 7272 6f72  }'".format(error
+000165d0: 5f6d 6573 7361 6765 290a 2020 2020 2020  _message).      
+000165e0: 2020 2020 2020 290a 0a20 2020 206c 6f67        )..    log
+000165f0: 6765 722e 696e 666f 2822 5b2b 5d20 536e  ger.info("[+] Sn
+00016600: 6170 7368 6f74 2070 726f 6365 7373 2068  apshot process h
+00016610: 6173 2073 7461 7274 6564 2229 0a0a 2020  as started")..  
+00016620: 2020 7768 696c 6520 7369 6d75 6c61 7469    while simulati
+00016630: 6f6e 5f73 7461 7475 7328 6964 5f73 696d  on_status(id_sim
+00016640: 756c 6174 696f 6e29 2021 3d20 2252 4541  ulation) != "REA
+00016650: 4459 223a 0a20 2020 2020 2020 206c 6f67  DY":.        log
+00016660: 6765 722e 696e 666f 2822 2020 5b2b 5d20  ger.info("  [+] 
+00016670: 536e 6170 7368 6f74 2069 6e20 7072 6f67  Snapshot in prog
+00016680: 7265 7373 2e2e 2e22 290a 2020 2020 2020  ress...").      
+00016690: 2020 7469 6d65 2e73 6c65 6570 2831 290a    time.sleep(1).
+000166a0: 0a20 2020 2020 2020 2073 696d 756c 6174  .        simulat
+000166b0: 696f 6e5f 6469 6374 203d 2066 6574 6368  ion_dict = fetch
+000166c0: 5f73 696d 756c 6174 696f 6e28 6964 5f73  _simulation(id_s
+000166d0: 696d 756c 6174 696f 6e29 0a20 2020 2020  imulation).     
+000166e0: 2020 2063 7572 7265 6e74 5f73 7461 7475     current_statu
+000166f0: 7320 3d20 7369 6d75 6c61 7469 6f6e 5f64  s = simulation_d
+00016700: 6963 745b 2273 7461 7475 7322 5d0a 2020  ict["status"].  
+00016710: 2020 2020 2020 6966 2063 7572 7265 6e74        if current
+00016720: 5f73 7461 7475 7320 3d3d 2022 4552 524f  _status == "ERRO
+00016730: 5222 3a0a 2020 2020 2020 2020 2020 2020  R":.            
+00016740: 6572 726f 725f 6d65 7373 6167 6520 3d20  error_message = 
+00016750: 7369 6d75 6c61 7469 6f6e 5f64 6963 745b  simulation_dict[
+00016760: 2265 7272 6f72 5f6d 7367 225d 0a20 2020  "error_msg"].   
+00016770: 2020 2020 2020 2020 2072 6169 7365 2045           raise E
+00016780: 7863 6570 7469 6f6e 280a 2020 2020 2020  xception(.      
+00016790: 2020 2020 2020 2020 2020 2245 7272 6f72            "Error
+000167a0: 2064 7572 696e 6720 7369 6d75 6c61 7469   during simulati
+000167b0: 6f6e 2073 6e61 7073 686f 743a 2027 7b7d  on snapshot: '{}
+000167c0: 2722 2e66 6f72 6d61 7428 6572 726f 725f  '".format(error_
+000167d0: 6d65 7373 6167 6529 0a20 2020 2020 2020  message).       
+000167e0: 2020 2020 2029 0a0a 2020 2020 7265 7475       )..    retu
+000167f0: 726e 2079 616d 6c0a 0a0a 6465 6620 636f  rn yaml...def co
+00016800: 6d70 7574 655f 696e 6672 6173 7472 7563  mpute_infrastruc
+00016810: 7475 7265 5f73 7461 7475 7328 2920 2d3e  ture_status() ->
+00016820: 2041 6e79 3a0a 2020 2020 2222 2247 6574   Any:.    """Get
+00016830: 2063 6f6d 7074 6520 7365 7276 6572 2073   compte server s
+00016840: 6572 7669 6365 7320 7374 6174 7573 2e0a  ervices status..
+00016850: 0a20 2020 203a 7265 7475 726e 3a20 5468  .    :return: Th
+00016860: 6520 636f 6d70 7574 6520 7365 7276 6572  e compute server
+00016870: 2073 6572 7669 6365 7320 7374 6174 7573   services status
+00016880: 2e0a 0a20 2020 2022 2222 0a20 2020 2072  ...    """.    r
+00016890: 6573 756c 7420 3d20 5f67 6574 2822 2f73  esult = _get("/s
+000168a0: 696d 756c 6174 696f 6e2f 636f 6d70 7574  imulation/comput
+000168b0: 655f 696e 6672 6173 7472 7563 7475 7265  e_infrastructure
+000168c0: 5f73 7461 7475 7322 290a 0a20 2020 2069  _status")..    i
+000168d0: 6620 7265 7375 6c74 2e73 7461 7475 735f  f result.status_
+000168e0: 636f 6465 2021 3d20 3230 303a 0a20 2020  code != 200:.   
+000168f0: 2020 2020 205f 6861 6e64 6c65 5f65 7272       _handle_err
+00016900: 6f72 2872 6573 756c 742c 2022 4361 6e6e  or(result, "Cann
+00016910: 6f74 2067 6574 2063 6f6d 7075 7465 2069  ot get compute i
+00016920: 6e66 7261 7374 7275 6374 7572 6520 7374  nfrastructure st
+00016930: 6174 7573 2229 0a0a 2020 2020 7369 6d75  atus")..    simu
+00016940: 6c61 7469 6f6e 5f64 6963 7420 3d20 7265  lation_dict = re
+00016950: 7375 6c74 2e6a 736f 6e28 290a 2020 2020  sult.json().    
+00016960: 7265 7475 726e 2073 696d 756c 6174 696f  return simulatio
+00016970: 6e5f 6469 6374 0a0a 0a64 6566 2061 6464  n_dict...def add
+00016980: 5f64 6e73 5f65 6e74 7269 6573 2869 645f  _dns_entries(id_
+00016990: 7369 6d75 6c61 7469 6f6e 3a20 696e 742c  simulation: int,
+000169a0: 2064 6e73 5f65 6e74 7269 6573 3a20 4469   dns_entries: Di
+000169b0: 6374 5b73 7472 2c20 7374 725d 2920 2d3e  ct[str, str]) ->
+000169c0: 204e 6f6e 653a 0a20 2020 2022 2222 4164   None:.    """Ad
+000169d0: 6420 766f 6c61 7469 6c65 2044 4e53 2065  d volatile DNS e
+000169e0: 6e74 7269 6573 2074 6f20 7468 6520 6375  ntries to the cu
+000169f0: 7272 656e 7420 7369 6d75 6c61 7469 6f6e  rrent simulation
+00016a00: 2e20 566f 6c61 7469 6c65 206d 6561 6e73  . Volatile means
+00016a10: 2074 6861 7420 6974 2069 7320 6e6f 740a   that it is not.
+00016a20: 2020 2020 7374 6f72 6564 2069 6e20 6461      stored in da
+00016a30: 7461 6261 7365 2e0a 0a20 2020 203a 7061  tabase...    :pa
+00016a40: 7261 6d20 6964 5f73 696d 756c 6174 696f  ram id_simulatio
+00016a50: 6e3a 2054 6865 2073 696d 756c 6174 696f  n: The simulatio
+00016a60: 6e20 4944 2e0a 2020 2020 3a70 6172 616d  n ID..    :param
+00016a70: 2064 6e73 5f65 6e74 7269 6573 3a20 5468   dns_entries: Th
+00016a80: 6520 444e 5320 656e 7472 6965 7320 2861  e DNS entries (a
+00016a90: 2064 6963 7420 7769 7468 2064 6f6d 6169   dict with domai
+00016aa0: 6e73 2061 7320 6b65 7973 2061 6e64 2049  ns as keys and I
+00016ab0: 5020 6164 6472 6573 7365 7320 6173 2076  P addresses as v
+00016ac0: 616c 7565 7329 2e0a 0a20 2020 2022 2222  alues)...    """
+00016ad0: 0a0a 2020 2020 6461 7461 203d 206a 736f  ..    data = jso
+00016ae0: 6e2e 6475 6d70 7328 646e 735f 656e 7472  n.dumps(dns_entr
+00016af0: 6965 7329 0a20 2020 2072 6573 756c 7420  ies).    result 
+00016b00: 3d20 5f70 6f73 7428 0a20 2020 2020 2020  = _post(.       
+00016b10: 2066 222f 7369 6d75 6c61 7469 6f6e 2f7b   f"/simulation/{
+00016b20: 6964 5f73 696d 756c 6174 696f 6e7d 2f61  id_simulation}/a
+00016b30: 6464 5f64 6e73 5f65 6e74 7269 6573 222c  dd_dns_entries",
+00016b40: 0a20 2020 2020 2020 2064 6174 613d 6461  .        data=da
+00016b50: 7461 2c0a 2020 2020 2020 2020 6865 6164  ta,.        head
+00016b60: 6572 733d 7b22 436f 6e74 656e 742d 5479  ers={"Content-Ty
+00016b70: 7065 223a 2022 6170 706c 6963 6174 696f  pe": "applicatio
+00016b80: 6e2f 6a73 6f6e 227d 2c0a 2020 2020 290a  n/json"},.    ).
+00016b90: 0a20 2020 2069 6620 7265 7375 6c74 2e73  .    if result.s
+00016ba0: 7461 7475 735f 636f 6465 2021 3d20 3230  tatus_code != 20
+00016bb0: 303a 0a20 2020 2020 2020 205f 6861 6e64  0:.        _hand
+00016bc0: 6c65 5f65 7272 6f72 2872 6573 756c 742c  le_error(result,
+00016bd0: 2022 4572 726f 7220 7768 696c 6520 6164   "Error while ad
+00016be0: 6469 6e67 2044 4e53 2065 6e74 7269 6573  ding DNS entries
+00016bf0: 2229 0a0a 0a64 6566 2063 6f6e 6e65 6374  ")...def connect
+00016c00: 5f68 6f73 7428 6964 5f73 696d 756c 6174  _host(id_simulat
+00016c10: 696f 6e3a 2069 6e74 2920 2d3e 204e 6f6e  ion: int) -> Non
+00016c20: 653a 0a20 2020 2022 2222 436f 6e6e 6563  e:.    """Connec
+00016c30: 7420 7468 6520 686f 7374 2069 6e74 6572  t the host inter
+00016c40: 6661 6365 2074 6f20 7468 6520 6375 7272  face to the curr
+00016c50: 656e 7420 7369 6d75 6c61 7469 6f6e 2e0a  ent simulation..
+00016c60: 0a20 2020 203a 7061 7261 6d20 6964 5f73  .    :param id_s
+00016c70: 696d 756c 6174 696f 6e3a 2054 6865 2073  imulation: The s
+00016c80: 696d 756c 6174 696f 6e20 4944 2e0a 0a20  imulation ID... 
+00016c90: 2020 2022 2222 0a0a 2020 2020 7265 7375     """..    resu
+00016ca0: 6c74 203d 205f 6765 7428 6622 2f73 696d  lt = _get(f"/sim
+00016cb0: 756c 6174 696f 6e2f 7b69 645f 7369 6d75  ulation/{id_simu
+00016cc0: 6c61 7469 6f6e 7d2f 636f 6e6e 6563 745f  lation}/connect_
+00016cd0: 686f 7374 2229 0a0a 2020 2020 6966 2072  host")..    if r
+00016ce0: 6573 756c 742e 7374 6174 7573 5f63 6f64  esult.status_cod
+00016cf0: 6520 213d 2032 3030 3a0a 2020 2020 2020  e != 200:.      
+00016d00: 2020 5f68 616e 646c 655f 6572 726f 7228    _handle_error(
+00016d10: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00016d20: 756c 742c 0a20 2020 2020 2020 2020 2020  ult,.           
+00016d30: 2066 2243 616e 6e6f 7420 6578 6563 7574   f"Cannot execut
+00016d40: 6520 6f70 6572 6174 696f 6e20 2763 6f6e  e operation 'con
+00016d50: 6e65 6374 5f68 6f73 7427 206f 6e20 7369  nect_host' on si
+00016d60: 6d75 6c61 7469 6f6e 2027 7b69 645f 7369  mulation '{id_si
+00016d70: 6d75 6c61 7469 6f6e 7d27 2e22 2c0a 2020  mulation}'.",.  
+00016d80: 2020 2020 2020 290a 0a0a 6465 6620 6469        )...def di
+00016d90: 7363 6f6e 6e65 6374 5f68 6f73 7428 6964  sconnect_host(id
+00016da0: 5f73 696d 756c 6174 696f 6e3a 2069 6e74  _simulation: int
+00016db0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2022  ) -> None:.    "
+00016dc0: 2222 4469 7363 6f6e 6e65 6374 2074 6865  ""Disconnect the
+00016dd0: 2068 6f73 7420 696e 7465 7266 6163 6520   host interface 
+00016de0: 746f 2074 6865 2063 7572 7265 6e74 2073  to the current s
+00016df0: 696d 756c 6174 696f 6e2e 0a0a 2020 2020  imulation...    
+00016e00: 3a70 6172 616d 2069 645f 7369 6d75 6c61  :param id_simula
+00016e10: 7469 6f6e 3a20 5468 6520 7369 6d75 6c61  tion: The simula
+00016e20: 7469 6f6e 2049 442e 0a0a 2020 2020 2222  tion ID...    ""
+00016e30: 220a 0a20 2020 2072 6573 756c 7420 3d20  "..    result = 
+00016e40: 5f67 6574 2866 222f 7369 6d75 6c61 7469  _get(f"/simulati
+00016e50: 6f6e 2f7b 6964 5f73 696d 756c 6174 696f  on/{id_simulatio
+00016e60: 6e7d 2f64 6973 636f 6e6e 6563 745f 686f  n}/disconnect_ho
+00016e70: 7374 2229 0a0a 2020 2020 6966 2072 6573  st")..    if res
+00016e80: 756c 742e 7374 6174 7573 5f63 6f64 6520  ult.status_code 
+00016e90: 213d 2032 3030 3a0a 2020 2020 2020 2020  != 200:.        
+00016ea0: 5f68 616e 646c 655f 6572 726f 7228 0a20  _handle_error(. 
+00016eb0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00016ec0: 742c 0a20 2020 2020 2020 2020 2020 2066  t,.            f
+00016ed0: 2243 616e 6e6f 7420 6578 6563 7574 6520  "Cannot execute 
+00016ee0: 6f70 6572 6174 696f 6e20 2764 6973 636f  operation 'disco
+00016ef0: 6e6e 6563 745f 686f 7374 2720 6f6e 2073  nnect_host' on s
+00016f00: 696d 756c 6174 696f 6e20 277b 6964 5f73  imulation '{id_s
+00016f10: 696d 756c 6174 696f 6e7d 272e 222c 0a20  imulation}'.",. 
+00016f20: 2020 2020 2020 2029 0a0a 0a64 6566 2067         )...def g
+00016f30: 656e 6572 6174 655f 6d61 6c69 6369 6f75  enerate_maliciou
+00016f40: 735f 646f 6d61 696e 7328 616c 676f 7269  s_domains(algori
+00016f50: 7468 6d3a 2073 7472 203d 204e 6f6e 652c  thm: str = None,
+00016f60: 206e 756d 6265 723a 2069 6e74 203d 2031   number: int = 1
+00016f70: 2920 2d3e 204c 6973 745b 7374 725d 3a0a  ) -> List[str]:.
+00016f80: 2020 2020 2222 2247 656e 6572 6174 6520      """Generate 
+00016f90: 616e 6420 7265 7475 726e 2061 206c 6973  and return a lis
+00016fa0: 7420 6f66 206d 616c 6963 696f 7573 2064  t of malicious d
+00016fb0: 6f6d 6169 6e73 2e0a 0a20 2020 203a 7265  omains...    :re
+00016fc0: 7475 726e 3a20 5468 6520 6c69 7374 206f  turn: The list o
+00016fd0: 6620 6765 6e65 7261 7465 6420 646f 6d61  f generated doma
+00016fe0: 696e 732e 0a0a 2020 2020 3a70 6172 616d  ins...    :param
+00016ff0: 2061 6c67 6f72 6974 686d 3a20 5468 6520   algorithm: The 
+00017000: 616c 676f 7269 7468 6d20 7573 6564 2074  algorithm used t
+00017010: 6f20 6765 6e65 7261 7465 2074 6865 206e  o generate the n
+00017020: 6577 2064 6f6d 6169 6e73 2e0a 2020 2020  ew domains..    
+00017030: 3a70 6172 616d 206e 756d 6265 723a 204e  :param number: N
+00017040: 756d 6265 7220 6f66 2064 6f6d 6169 6e73  umber of domains
+00017050: 2074 6f20 6765 6e65 7261 7465 2e0a 0a20   to generate... 
+00017060: 2020 2022 2222 0a0a 2020 2020 6461 7461     """..    data
+00017070: 5f64 6963 7420 3d20 7b0a 2020 2020 2020  _dict = {.      
+00017080: 2020 2261 6c67 6f72 6974 686d 223a 2061    "algorithm": a
+00017090: 6c67 6f72 6974 686d 2c0a 2020 2020 2020  lgorithm,.      
+000170a0: 2020 226e 756d 6265 7222 3a20 6e75 6d62    "number": numb
+000170b0: 6572 2c0a 2020 2020 7d0a 2020 2020 6461  er,.    }.    da
+000170c0: 7461 203d 206a 736f 6e2e 6475 6d70 7328  ta = json.dumps(
+000170d0: 6461 7461 5f64 6963 7429 0a0a 2020 2020  data_dict)..    
+000170e0: 7265 7375 6c74 203d 205f 706f 7374 280a  result = _post(.
+000170f0: 2020 2020 2020 2020 222f 746f 706f 6c6f          "/topolo
+00017100: 6779 2f67 656e 6572 6174 655f 6d61 6c69  gy/generate_mali
+00017110: 6369 6f75 735f 646f 6d61 696e 7322 2c0a  cious_domains",.
+00017120: 2020 2020 2020 2020 6461 7461 3d64 6174          data=dat
+00017130: 612c 0a20 2020 2020 2020 2068 6561 6465  a,.        heade
+00017140: 7273 3d7b 2243 6f6e 7465 6e74 2d54 7970  rs={"Content-Typ
+00017150: 6522 3a20 2261 7070 6c69 6361 7469 6f6e  e": "application
+00017160: 2f6a 736f 6e22 7d2c 0a20 2020 2029 0a0a  /json"},.    )..
+00017170: 2020 2020 6966 2072 6573 756c 742e 7374      if result.st
+00017180: 6174 7573 5f63 6f64 6520 213d 2032 3030  atus_code != 200
+00017190: 3a0a 2020 2020 2020 2020 5f68 616e 646c  :.        _handl
+000171a0: 655f 6572 726f 7228 7265 7375 6c74 2c20  e_error(result, 
+000171b0: 2245 7272 6f72 2077 6869 6c65 2061 6464  "Error while add
+000171c0: 696e 6720 444e 5320 656e 7472 6965 7322  ing DNS entries"
+000171d0: 290a 0a20 2020 2064 6f6d 6169 6e73 203d  )..    domains =
+000171e0: 2072 6573 756c 742e 6a73 6f6e 2829 0a20   result.json(). 
+000171f0: 2020 2072 6574 7572 6e20 646f 6d61 696e     return domain
+00017200: 735b 2264 6f6d 6169 6e73 225d 0a0a 0a64  s["domains"]...d
+00017210: 6566 2063 7265 6174 655f 6461 7461 7365  ef create_datase
+00017220: 7428 0a20 2020 2069 645f 7369 6d75 6c61  t(.    id_simula
+00017230: 7469 6f6e 3a20 696e 742c 2064 6f6e 745f  tion: int, dont_
+00017240: 6368 6563 6b5f 6c6f 6773 5f70 6174 683a  check_logs_path:
+00017250: 2062 6f6f 6c20 3d20 4661 6c73 650a 2920   bool = False.) 
+00017260: 2d3e 204f 7074 696f 6e61 6c5b 7575 6964  -> Optional[uuid
+00017270: 2e55 5549 445d 3a0a 2020 2020 2222 2248  .UUID]:.    """H
+00017280: 616e 646c 6573 2074 6865 2063 7265 6174  andles the creat
+00017290: 696f 6e20 6f66 2074 6865 2064 6174 6173  ion of the datas
+000172a0: 6574 2061 6674 6572 2074 6865 2065 6e64  et after the end
+000172b0: 206f 6620 6120 7369 6d75 6c61 7469 6f6e   of a simulation
+000172c0: 0a0a 2020 2020 4d75 7374 2062 6520 6361  ..    Must be ca
+000172d0: 6c6c 6564 2061 6674 6572 2061 2053 544f  lled after a STO
+000172e0: 5020 6f70 6572 6174 696f 6e2c 2061 6e64  P operation, and
+000172f0: 206f 6e63 6520 616c 6c20 636f 6d70 7574   once all comput
+00017300: 650a 2020 2020 7365 7276 6572 7320 6861  e.    servers ha
+00017310: 7665 2066 756c 6c79 2073 746f 7070 6564  ve fully stopped
+00017320: 2e0a 0a20 2020 2042 6173 6963 616c 6c79  ...    Basically
+00017330: 2c20 7468 6973 2066 756e 6374 696f 6e20  , this function 
+00017340: 636f 6d6d 756e 6963 6174 6573 2077 6974  communicates wit
+00017350: 6820 7468 6520 636f 7265 2041 5049 2c20  h the core API, 
+00017360: 7768 6963 6820 6974 7365 6c66 0a20 2020  which itself.   
+00017370: 2063 6f6d 6d75 6e69 6361 7465 7320 7769   communicates wi
+00017380: 7468 2074 6865 2070 7562 6c69 7368 2073  th the publish s
+00017390: 6572 7665 7227 7320 2262 6163 6b65 6e64  erver's "backend
+000173a0: 2220 4150 492e 0a0a 2020 2020 3a72 6574  " API...    :ret
+000173b0: 7572 6e3a 2054 6865 206e 6577 2064 6174  urn: The new dat
+000173c0: 6173 6574 2055 5549 442e 0a0a 2020 2020  aset UUID...    
+000173d0: 3a70 6172 616d 2069 645f 7369 6d75 6c61  :param id_simula
+000173e0: 7469 6f6e 3a20 5468 6520 7369 6d75 6c61  tion: The simula
+000173f0: 7469 6f6e 2049 442e 0a20 2020 203a 7061  tion ID..    :pa
+00017400: 7261 6d20 646f 6e74 5f63 6865 636b 5f6c  ram dont_check_l
+00017410: 6f67 735f 7061 7468 3a20 5465 6c6c 2074  ogs_path: Tell t
+00017420: 6f20 6e6f 7420 656d 6974 2061 2077 6172  o not emit a war
+00017430: 6e69 6e67 2069 6620 6c6f 6773 2070 6174  ning if logs pat
+00017440: 6873 2061 7265 2069 6e63 6f72 7265 6374  hs are incorrect
+00017450: 2028 7761 726e 696e 6720 6172 6520 656d   (warning are em
+00017460: 6974 7465 6420 6279 2064 6566 6175 6c74  itted by default
+00017470: 292e 0a0a 2020 2020 2222 220a 0a20 2020  )...    """..   
+00017480: 206c 6f67 6765 722e 696e 666f 280a 2020   logger.info(.  
+00017490: 2020 2020 2020 225b 2b5d 2047 6f69 6e67        "[+] Going
+000174a0: 2074 6f20 6372 6561 7465 2064 6174 6173   to create datas
+000174b0: 6574 2062 6173 6564 206f 6e20 6461 7461  et based on data
+000174c0: 2070 726f 6475 6365 6420 6279 2073 696d   produced by sim
+000174d0: 756c 6174 696f 6e20 4944 2027 7b7d 2722  ulation ID '{}'"
+000174e0: 2e66 6f72 6d61 7428 0a20 2020 2020 2020  .format(.       
+000174f0: 2020 2020 2069 645f 7369 6d75 6c61 7469       id_simulati
+00017500: 6f6e 0a20 2020 2020 2020 2029 0a20 2020  on.        ).   
+00017510: 2029 0a0a 2020 2020 6966 2064 6f6e 745f   )..    if dont_
+00017520: 6368 6563 6b5f 6c6f 6773 5f70 6174 6820  check_logs_path 
+00017530: 6973 2046 616c 7365 3a0a 2020 2020 2020  is False:.      
+00017540: 2020 5f63 6865 636b 5f6c 6f67 735f 7061    _check_logs_pa
+00017550: 7468 2869 645f 7369 6d75 6c61 7469 6f6e  th(id_simulation
+00017560: 290a 0a20 2020 2023 2041 736b 2074 6865  )..    # Ask the
+00017570: 2063 6f72 6520 4150 4920 746f 2063 6f6e   core API to con
+00017580: 7461 6374 2074 6865 202f 6261 636b 656e  tact the /backen
+00017590: 642f 2070 7562 6c69 7368 2073 6572 7665  d/ publish serve
+000175a0: 7220 4150 490a 2020 2020 2320 696e 206f  r API.    # in o
+000175b0: 7264 6572 2074 6f20 7374 6172 7420 7468  rder to start th
+000175c0: 6520 6461 7461 7365 7420 6372 6561 7469  e dataset creati
+000175d0: 6f6e 2070 726f 6365 7373 0a20 2020 2072  on process.    r
+000175e0: 6573 756c 7420 3d20 5f70 6f73 7428 6622  esult = _post(f"
+000175f0: 2f63 7265 6174 655f 6461 7461 7365 742f  /create_dataset/
+00017600: 7b69 645f 7369 6d75 6c61 7469 6f6e 7d22  {id_simulation}"
+00017610: 290a 2020 2020 6966 2072 6573 756c 742e  ).    if result.
+00017620: 7374 6174 7573 5f63 6f64 6520 213d 2032  status_code != 2
+00017630: 3030 3a0a 2020 2020 2020 2020 5f68 616e  00:.        _han
+00017640: 646c 655f 6572 726f 7228 7265 7375 6c74  dle_error(result
+00017650: 2c20 2243 616e 6e6f 7420 696e 6974 6961  , "Cannot initia
+00017660: 7465 2074 6865 2063 7265 6174 696f 6e20  te the creation 
+00017670: 6f66 2074 6865 2064 6174 6173 6574 2229  of the dataset")
+00017680: 0a0a 2020 2020 6461 7461 7365 745f 6964  ..    dataset_id
+00017690: 203d 2072 6573 756c 742e 6a73 6f6e 2829   = result.json()
+000176a0: 5b22 6461 7461 7365 745f 6964 225d 0a0a  ["dataset_id"]..
+000176b0: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
+000176c0: 6622 2020 5b2b 5d20 4461 7461 7365 7420  f"  [+] Dataset 
+000176d0: 7072 652d 6372 6561 7465 6420 7769 7468  pre-created with
+000176e0: 2064 6174 6173 6574 2069 6420 7b64 6174   dataset id {dat
+000176f0: 6173 6574 5f69 647d 2229 0a0a 2020 2020  aset_id}")..    
+00017700: 2320 5374 6172 7420 616e 2061 6374 6976  # Start an activ
+00017710: 6520 7761 6974 696e 6720 6c6f 6f70 2075  e waiting loop u
+00017720: 6e74 696c 2074 6865 2064 6174 6173 6574  ntil the dataset
+00017730: 2063 7265 6174 696f 6e20 6966 2066 756c   creation if ful
+00017740: 6c79 2063 6f6d 706c 6574 650a 2020 2020  ly complete.    
+00017750: 2320 496e 6465 6564 2c20 6461 7461 7365  # Indeed, datase
+00017760: 7420 6372 6561 7469 6f6e 2069 6e76 6f6c  t creation invol
+00017770: 7665 7320 7468 6520 646f 776e 6c6f 6164  ves the download
+00017780: 206f 6620 706f 7465 6e74 6961 6c6c 7920   of potentially 
+00017790: 6c61 7267 650a 2020 2020 2320 6669 6c65  large.    # file
+000177a0: 7320 6f76 6572 7320 7468 6520 6e65 7477  s overs the netw
+000177b0: 6f72 6b2c 2077 6869 6368 2063 616e 2074  ork, which can t
+000177c0: 616b 6520 736f 6d65 2074 696d 6521 0a20  ake some time!. 
+000177d0: 2020 206d 6178 5f72 6574 7269 6573 203d     max_retries =
+000177e0: 2035 0a20 2020 2072 6574 7269 6573 203d   5.    retries =
+000177f0: 206d 6178 5f72 6574 7269 6573 0a20 2020   max_retries.   
+00017800: 2077 6869 6c65 2054 7275 653a 0a20 2020   while True:.   
+00017810: 2020 2020 2074 696d 652e 736c 6565 7028       time.sleep(
+00017820: 3229 0a0a 2020 2020 2020 2020 7265 7375  2)..        resu
+00017830: 6c74 203d 205f 6765 7428 6622 2f63 7265  lt = _get(f"/cre
+00017840: 6174 655f 6461 7461 7365 742f 7374 6174  ate_dataset/stat
+00017850: 7573 2f7b 6461 7461 7365 745f 6964 7d22  us/{dataset_id}"
+00017860: 290a 2020 2020 2020 2020 6966 2072 6573  ).        if res
+00017870: 756c 742e 7374 6174 7573 5f63 6f64 6520  ult.status_code 
+00017880: 213d 2032 3030 3a0a 2020 2020 2020 2020  != 200:.        
+00017890: 2020 2020 6966 2028 0a20 2020 2020 2020      if (.       
+000178a0: 2020 2020 2020 2020 2072 6573 756c 742e           result.
+000178b0: 6865 6164 6572 732e 6765 7428 2263 6f6e  headers.get("con
+000178c0: 7465 6e74 2d74 7970 6522 2920 3d3d 2022  tent-type") == "
+000178d0: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
+000178e0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+000178f0: 2020 616e 6420 226d 6573 7361 6765 2220    and "message" 
+00017900: 696e 2072 6573 756c 742e 6a73 6f6e 2829  in result.json()
+00017910: 0a20 2020 2020 2020 2020 2020 2029 3a0a  .            ):.
+00017920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017930: 6572 726f 725f 6d73 6720 3d20 7265 7375  error_msg = resu
+00017940: 6c74 2e6a 736f 6e28 295b 226d 6573 7361  lt.json()["messa
+00017950: 6765 225d 0a20 2020 2020 2020 2020 2020  ge"].           
+00017960: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00017970: 2020 2020 2020 2065 7272 6f72 5f6d 7367         error_msg
+00017980: 203d 2072 6573 756c 742e 7465 7874 0a0a   = result.text..
+00017990: 2020 2020 2020 2020 2020 2020 2320 5265              # Re
+000179a0: 7472 7920 746f 2067 6574 2074 6865 2073  try to get the s
+000179b0: 7461 7475 7320 6120 636f 7570 6c65 206f  tatus a couple o
+000179c0: 6620 7469 6d65 7320 6265 666f 7265 2071  f times before q
+000179d0: 7365 6e64 696e 6720 6261 636b 2061 6e20  sending back an 
+000179e0: 6572 726f 720a 2020 2020 2020 2020 2020  error.          
+000179f0: 2020 6966 2072 6574 7269 6573 203d 3d20    if retries == 
+00017a00: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
+00017a10: 2020 2072 6169 7365 2045 7863 6570 7469     raise Excepti
+00017a20: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
+00017a30: 2020 2020 2020 2020 2245 7272 6f72 2064          "Error d
+00017a40: 7572 696e 6720 6372 6561 7469 6f6e 206f  uring creation o
+00017a50: 6620 6461 7461 7365 7420 7b7d 3a20 636f  f dataset {}: co
+00017a60: 756c 6420 6e6f 7420 6765 7420 7374 6174  uld not get stat
+00017a70: 7573 206f 6620 7468 6520 6461 7461 7365  us of the datase
+00017a80: 7420 6372 6561 7469 6f6e 2061 6674 6572  t creation after
+00017a90: 207b 7d20 7472 6965 732e 2043 6f72 6520   {} tries. Core 
+00017aa0: 4150 4920 4854 5450 2073 7461 7475 733a  API HTTP status:
+00017ab0: 207b 7d2e 2052 6573 706f 6e73 653a 207b   {}. Response: {
+00017ac0: 7d20 222e 666f 726d 6174 280a 2020 2020  } ".format(.    
+00017ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017ae0: 2020 2020 6461 7461 7365 745f 6964 2c20      dataset_id, 
+00017af0: 6d61 785f 7265 7472 6965 732c 2072 6573  max_retries, res
+00017b00: 756c 742e 7374 6174 7573 5f63 6f64 652c  ult.status_code,
+00017b10: 2065 7272 6f72 5f6d 7367 0a20 2020 2020   error_msg.     
+00017b20: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00017b30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017b40: 2029 0a20 2020 2020 2020 2020 2020 2065   ).            e
+00017b50: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00017b60: 2020 2020 206c 6f67 6765 722e 7761 726e       logger.warn
+00017b70: 696e 6728 0a20 2020 2020 2020 2020 2020  ing(.           
+00017b80: 2020 2020 2020 2020 2022 2020 5b2b 5d20           "  [+] 
+00017b90: 436f 756c 6420 6e6f 7420 6765 7420 7374  Could not get st
+00017ba0: 6174 7573 206f 6620 6461 7461 7365 7420  atus of dataset 
+00017bb0: 6372 6561 7469 6f6e 2028 5265 7472 6965  creation (Retrie
+00017bc0: 7320 6c65 6674 3a20 7b7d 2e20 436f 7265  s left: {}. Core
+00017bd0: 2041 5049 2048 5454 5020 7374 6174 7573   API HTTP status
+00017be0: 3a20 7b7d 2e20 5265 7370 6f6e 7365 3a20  : {}. Response: 
+00017bf0: 7b7d 2922 2e66 6f72 6d61 7428 0a20 2020  {})".format(.   
+00017c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017c10: 2020 2020 2072 6574 7269 6573 2c20 7265       retries, re
+00017c20: 7375 6c74 2e73 7461 7475 735f 636f 6465  sult.status_code
+00017c30: 2c20 6572 726f 725f 6d73 670a 2020 2020  , error_msg.    
+00017c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017c50: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00017c60: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00017c70: 2020 2020 7265 7472 6965 7320 2d3d 2031      retries -= 1
+00017c80: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00017c90: 2020 2020 2020 2020 2020 2023 2052 6573             # Res
+00017ca0: 6574 2074 6865 206e 756d 6265 7220 6f66  et the number of
+00017cb0: 2072 6574 7269 6573 0a20 2020 2020 2020   retries.       
+00017cc0: 2020 2020 2072 6574 7269 6573 203d 206d       retries = m
+00017cd0: 6178 5f72 6574 7269 6573 0a0a 2020 2020  ax_retries..    
+00017ce0: 2020 2020 2020 2020 2320 4765 7420 7468          # Get th
+00017cf0: 6520 7374 6174 7573 2061 6e64 206d 6573  e status and mes
+00017d00: 7361 6765 0a20 2020 2020 2020 2020 2020  sage.           
+00017d10: 2064 6174 6173 6574 5f63 7265 6174 696f   dataset_creatio
+00017d20: 6e5f 7374 6174 7573 203d 2072 6573 756c  n_status = resul
+00017d30: 742e 6a73 6f6e 2829 5b22 7374 6174 7573  t.json()["status
+00017d40: 225d 0a20 2020 2020 2020 2020 2020 2064  "].            d
+00017d50: 6174 6173 6574 5f63 7265 6174 696f 6e5f  ataset_creation_
+00017d60: 6d65 7373 6167 6520 3d20 7265 7375 6c74  message = result
+00017d70: 2e6a 736f 6e28 295b 226d 6573 7361 6765  .json()["message
+00017d80: 225d 0a0a 2020 2020 2020 2020 2020 2020  "]..            
+00017d90: 6c6f 6767 6572 2e69 6e66 6f28 0a20 2020  logger.info(.   
+00017da0: 2020 2020 2020 2020 2020 2020 2022 2020               "  
+00017db0: 5b2b 5d20 4461 7461 7365 7420 6372 6561  [+] Dataset crea
+00017dc0: 7469 6f6e 2069 6e20 7072 6f67 7265 7373  tion in progress
+00017dd0: 2028 5374 6174 7573 3a20 7b7d 2922 2e66   (Status: {})".f
+00017de0: 6f72 6d61 7428 0a20 2020 2020 2020 2020  ormat(.         
+00017df0: 2020 2020 2020 2020 2020 2064 6174 6173             datas
+00017e00: 6574 5f63 7265 6174 696f 6e5f 7374 6174  et_creation_stat
+00017e10: 7573 0a20 2020 2020 2020 2020 2020 2020  us.             
+00017e20: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00017e30: 2029 0a0a 2020 2020 2020 2020 2020 2020   )..            
+00017e40: 6966 2064 6174 6173 6574 5f63 7265 6174  if dataset_creat
+00017e50: 696f 6e5f 7374 6174 7573 203d 3d20 2246  ion_status == "F
+00017e60: 494e 4953 4845 4422 3a0a 2020 2020 2020  INISHED":.      
+00017e70: 2020 2020 2020 2020 2020 2320 416c 6c20            # All 
+00017e80: 7765 6e74 2077 656c 6c0a 2020 2020 2020  went well.      
+00017e90: 2020 2020 2020 2020 2020 6272 6561 6b0a            break.
+00017ea0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00017eb0: 2064 6174 6173 6574 5f63 7265 6174 696f   dataset_creatio
+00017ec0: 6e5f 7374 6174 7573 203d 3d20 2246 494e  n_status == "FIN
+00017ed0: 4953 4845 445f 4552 524f 5222 3a0a 2020  ISHED_ERROR":.  
+00017ee0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00017ef0: 5468 6520 6461 7461 7365 7420 6372 6561  The dataset crea
+00017f00: 7469 6f6e 2065 6e63 6f75 6e74 6572 6564  tion encountered
+00017f10: 2065 7272 6f72 730a 2020 2020 2020 2020   errors.        
+00017f20: 2020 2020 2020 2020 7261 6973 6520 4578          raise Ex
+00017f30: 6365 7074 696f 6e28 0a20 2020 2020 2020  ception(.       
+00017f40: 2020 2020 2020 2020 2020 2020 2022 4572               "Er
+00017f50: 726f 7220 6475 7269 6e67 2063 7265 6174  ror during creat
+00017f60: 696f 6e20 6f66 2064 6174 6173 6574 207b  ion of dataset {
+00017f70: 7d3a 2064 6174 6173 6574 2063 7265 6174  }: dataset creat
+00017f80: 696f 6e20 656e 6465 6420 7769 7468 2065  ion ended with e
+00017f90: 7272 6f72 7320 2827 7b7d 2729 2e22 2e66  rrors ('{}').".f
+00017fa0: 6f72 6d61 7428 0a20 2020 2020 2020 2020  ormat(.         
+00017fb0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00017fc0: 6174 6173 6574 5f69 642c 2064 6174 6173  ataset_id, datas
+00017fd0: 6574 5f63 7265 6174 696f 6e5f 6d65 7373  et_creation_mess
+00017fe0: 6167 650a 2020 2020 2020 2020 2020 2020  age.            
+00017ff0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00018000: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00018010: 2020 2020 2020 2020 2320 4f74 6865 7277          # Otherw
+00018020: 6973 652c 2064 6174 6173 6574 2063 7265  ise, dataset cre
+00018030: 6174 696f 6e20 6973 206e 6f74 2066 696e  ation is not fin
+00018040: 6973 6865 642c 206a 7573 7420 6c6f 6f70  ished, just loop
+00018050: 0a0a 2020 2020 6c6f 6767 6572 2e69 6e66  ..    logger.inf
+00018060: 6f28 225b 2b5d 2044 6174 6173 6574 2063  o("[+] Dataset c
+00018070: 7265 6174 696f 6e20 7761 7320 636f 7272  reation was corr
+00018080: 6563 746c 7920 6578 6563 7574 6564 2229  ectly executed")
+00018090: 0a0a 2020 2020 2320 5365 7420 7468 6520  ..    # Set the 
+000180a0: 7369 6d75 6c61 7469 6f6e 2073 7461 7475  simulation statu
+000180b0: 7320 746f 2052 4541 4459 0a20 2020 2075  s to READY.    u
+000180c0: 7064 6174 655f 7369 6d75 6c61 7469 6f6e  pdate_simulation
+000180d0: 2869 645f 7369 6d75 6c61 7469 6f6e 2c20  (id_simulation, 
+000180e0: 7b22 7374 6174 7573 223a 2022 5245 4144  {"status": "READ
+000180f0: 5922 7d29 0a0a 2020 2020 7369 6d75 6c61  Y"})..    simula
+00018100: 7469 6f6e 203d 2066 6574 6368 5f73 696d  tion = fetch_sim
+00018110: 756c 6174 696f 6e28 6964 5f73 696d 756c  ulation(id_simul
+00018120: 6174 696f 6e29 0a20 2020 206c 6f67 6765  ation).    logge
+00018130: 722e 696e 666f 2822 5b2b 5d20 4375 7272  r.info("[+] Curr
+00018140: 656e 7420 7369 6d75 6c61 7469 6f6e 2073  ent simulation s
+00018150: 7461 7475 733a 2027 7b7d 2722 2e66 6f72  tatus: '{}'".for
+00018160: 6d61 7428 7369 6d75 6c61 7469 6f6e 5b22  mat(simulation["
+00018170: 7374 6174 7573 225d 2929 0a0a 2020 2020  status"]))..    
+00018180: 7265 7475 726e 2075 7569 642e 5555 4944  return uuid.UUID
+00018190: 2864 6174 6173 6574 5f69 6429 0a0a 0a64  (dataset_id)...d
+000181a0: 6566 205f 6368 6563 6b5f 6c6f 6773 5f70  ef _check_logs_p
+000181b0: 6174 6828 6964 5f73 696d 756c 6174 696f  ath(id_simulatio
+000181c0: 6e3a 2069 6e74 2920 2d3e 204e 6f6e 653a  n: int) -> None:
+000181d0: 0a20 2020 2022 2222 5072 6f64 7563 6573  .    """Produces
+000181e0: 2065 7272 6f72 206d 6573 7361 6765 2069   error message i
+000181f0: 6620 6120 6261 6420 7061 7468 2077 6173  f a bad path was
+00018200: 2073 6574 2066 6f72 2074 6865 2072 7379   set for the rsy
+00018210: 736c 6f67 2773 206c 6f67 0a20 2020 2076  slog's log.    v
+00018220: 6f6c 756d 652e 0a0a 2020 2020 446f 2061  olume...    Do a
+00018230: 2073 6d61 6c6c 2063 6865 636b 2066 6f72   small check for
+00018240: 2074 6865 2073 616b 6520 6f66 2068 656c   the sake of hel
+00018250: 7069 6e67 2074 6865 2075 7365 7220 616e  ping the user an
+00018260: 6420 6769 7669 6e67 2062 6574 7465 720a  d giving better.
+00018270: 2020 2020 7573 6572 2065 7870 6572 6965      user experie
+00018280: 6e63 653a 2063 6865 636b 2069 6620 7468  nce: check if th
+00018290: 6520 7273 7973 6c6f 6720 646f 636b 6572  e rsyslog docker
+000182a0: 2028 7768 6963 6820 636f 6c6c 6563 7473   (which collects
+000182b0: 206c 6f67 7329 0a20 2020 2069 7320 696e   logs).    is in
+000182c0: 7369 6465 2074 6865 2074 6f70 6f6c 6f67  side the topolog
+000182d0: 792c 2061 6e64 2069 6620 736f 2c20 6368  y, and if so, ch
+000182e0: 6563 6b20 7468 6520 2268 6f73 745f 7061  eck the "host_pa
+000182f0: 7468 2220 666f 7220 6c6f 6773 0a20 2020  th" for logs.   
+00018300: 2028 6120 7370 6563 6966 6963 2070 6174   (a specific pat
+00018310: 6820 6973 2065 7870 6563 7465 642c 2061  h is expected, a
+00018320: 6e64 2069 7320 6861 7264 636f 6465 6420  nd is hardcoded 
+00018330: 696e 2069 745f 7369 6d75 6c61 7469 6f6e  in it_simulation
+00018340: 290a 0a20 2020 2022 2222 0a20 2020 2023  )..    """.    #
+00018350: 2054 4f44 4f28 4352 4429 3a20 7468 6973   TODO(CRD): this
+00018360: 2063 6865 636b 2077 696c 6c20 616c 7761   check will alwa
+00018370: 7973 2066 6169 6c20 7768 656e 2063 725f  ys fail when cr_
+00018380: 6170 695f 636c 6965 6e74 2c20 7468 650a  api_client, the.
+00018390: 2020 2020 2320 6974 5f73 696d 756c 6174      # it_simulat
+000183a0: 696f 6e20 646f 636b 6572 2c20 616e 6420  ion docker, and 
+000183b0: 7468 6520 7273 7973 6c6f 6720 646f 636b  the rsyslog dock
+000183c0: 6572 2061 7265 206e 6f74 206f 6e20 7468  er are not on th
+000183d0: 6520 7361 6d65 206d 6163 6869 6e65 0a0a  e same machine..
+000183e0: 2020 2020 746f 706f 6c6f 6779 203d 2059      topology = Y
+000183f0: 414d 4c28 292e 6c6f 6164 2866 6574 6368  AML().load(fetch
+00018400: 5f73 696d 756c 6174 696f 6e5f 746f 706f  _simulation_topo
+00018410: 6c6f 6779 5f79 616d 6c28 6964 5f73 696d  logy_yaml(id_sim
+00018420: 756c 6174 696f 6e29 290a 0a20 2020 2023  ulation))..    #
+00018430: 2054 6865 2070 6174 6820 6f66 2074 6865   The path of the
+00018440: 206c 6f67 732c 206f 6e20 7468 6520 636f   logs, on the co
+00018450: 6d70 7574 6520 7365 7276 6572 2066 696c  mpute server fil
+00018460: 6520 7379 7374 656d 2073 686f 756c 6420  e system should 
+00018470: 414c 5741 5953 2062 6520 6173 2066 6f6c  ALWAYS be as fol
+00018480: 6c6f 7773 0a20 2020 2072 7379 736c 6f67  lows.    rsyslog
+00018490: 5f64 6f63 6b65 725f 7072 6573 656e 743a  _docker_present:
+000184a0: 2062 6f6f 6c20 3d20 4661 6c73 650a 2020   bool = False.  
+000184b0: 2020 706f 7465 6e74 6961 6c5f 6c6f 6773    potential_logs
+000184c0: 5f61 6273 6f6c 7574 655f 7061 7468 3a20  _absolute_path: 
+000184d0: 4c69 7374 5b50 6174 685d 203d 205b 5d0a  List[Path] = [].
+000184e0: 2020 2020 666f 7220 6e6f 6465 2069 6e20      for node in 
+000184f0: 746f 706f 6c6f 6779 5b22 6e6f 6465 7322  topology["nodes"
+00018500: 5d3a 0a20 2020 2020 2020 2069 6620 280a  ]:.        if (.
+00018510: 2020 2020 2020 2020 2020 2020 6e6f 6465              node
+00018520: 5b22 7479 7065 225d 203d 3d20 2264 6f63  ["type"] == "doc
+00018530: 6b65 7222 0a20 2020 2020 2020 2020 2020  ker".           
+00018540: 2061 6e64 2022 7273 7973 6c6f 6722 2069   and "rsyslog" i
+00018550: 6e20 6e6f 6465 5b22 6261 7365 5f69 6d61  n node["base_ima
+00018560: 6765 225d 0a20 2020 2020 2020 2020 2020  ge"].           
+00018570: 2061 6e64 2022 766f 6c75 6d65 7322 2069   and "volumes" i
+00018580: 6e20 6e6f 6465 0a20 2020 2020 2020 2029  n node.        )
+00018590: 3a0a 2020 2020 2020 2020 2020 2020 7273  :.            rs
+000185a0: 7973 6c6f 675f 646f 636b 6572 5f70 7265  yslog_docker_pre
+000185b0: 7365 6e74 203d 2054 7275 650a 2020 2020  sent = True.    
+000185c0: 2020 2020 2020 2020 666f 7220 766f 6c75          for volu
+000185d0: 6d65 2069 6e20 6e6f 6465 5b22 766f 6c75  me in node["volu
+000185e0: 6d65 7322 5d3a 0a20 2020 2020 2020 2020  mes"]:.         
+000185f0: 2020 2020 2020 2069 6620 280a 2020 2020         if (.    
+00018600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018610: 2268 6f73 745f 7061 7468 2220 696e 2076  "host_path" in v
+00018620: 6f6c 756d 650a 2020 2020 2020 2020 2020  olume.          
+00018630: 2020 2020 2020 2020 2020 616e 6420 2277            and "w
+00018640: 7269 7461 626c 6522 2069 6e20 766f 6c75  ritable" in volu
+00018650: 6d65 0a20 2020 2020 2020 2020 2020 2020  me.             
+00018660: 2020 2020 2020 2061 6e64 2076 6f6c 756d         and volum
+00018670: 655b 2277 7269 7461 626c 6522 5d0a 2020  e["writable"].  
+00018680: 2020 2020 2020 2020 2020 2020 2020 293a                ):
+00018690: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000186a0: 2020 2020 2070 6f74 656e 7469 616c 5f6c       potential_l
+000186b0: 6f67 735f 6162 736f 6c75 7465 5f70 6174  ogs_absolute_pat
+000186c0: 682e 6170 7065 6e64 2850 6174 6828 766f  h.append(Path(vo
+000186d0: 6c75 6d65 5b22 686f 7374 5f70 6174 6822  lume["host_path"
+000186e0: 5d29 290a 0a20 2020 2023 2049 6620 6e6f  ]))..    # If no
+000186f0: 2072 7379 736c 6f67 2064 6f63 6b65 7220   rsyslog docker 
+00018700: 6973 2070 7265 7365 6e74 2c20 6a73 7574  is present, jsut
+00018710: 2069 7373 7565 2061 206e 6f6e 2d62 6c6f   issue a non-blo
+00018720: 636b 696e 6720 7761 726e 696e 670a 2020  cking warning.  
+00018730: 2020 6966 206e 6f74 2072 7379 736c 6f67    if not rsyslog
+00018740: 5f64 6f63 6b65 725f 7072 6573 656e 743a  _docker_present:
+00018750: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
+00018760: 7761 726e 696e 6728 0a20 2020 2020 2020  warning(.       
+00018770: 2020 2020 2022 2020 5b2b 5d20 5468 6520       "  [+] The 
+00018780: 636f 6c6c 6563 7469 6f6e 206f 6620 6c6f  collection of lo
+00018790: 6773 2077 6173 206e 6f74 2061 6374 6976  gs was not activ
+000187a0: 6174 6564 2066 6f72 2074 6865 2073 696d  ated for the sim
+000187b0: 756c 6174 696f 6e20 2874 6865 2072 7379  ulation (the rsy
+000187c0: 736c 6f67 2064 6f63 6b65 7220 6973 206e  slog docker is n
+000187d0: 6f74 2070 7265 7365 6e74 2069 6e20 7468  ot present in th
+000187e0: 6520 746f 706f 6c6f 6779 292e 204e 6f20  e topology). No 
+000187f0: 6c6f 6720 7769 6c6c 2062 6520 696e 636c  log will be incl
+00018800: 7564 6564 2069 6e20 7468 6520 6461 7461  uded in the data
+00018810: 7365 742e 220a 2020 2020 2020 2020 290a  set.".        ).
+00018820: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00018830: 2020 7772 6f6e 675f 686f 7374 5f70 6174    wrong_host_pat
+00018840: 6820 3d20 5472 7565 0a20 2020 2020 2020  h = True.       
+00018850: 2066 6f72 2070 2069 6e20 706f 7465 6e74   for p in potent
+00018860: 6961 6c5f 6c6f 6773 5f61 6273 6f6c 7574  ial_logs_absolut
+00018870: 655f 7061 7468 3a0a 2020 2020 2020 2020  e_path:.        
+00018880: 2020 2020 6966 206e 6f74 2070 2e69 735f      if not p.is_
+00018890: 6162 736f 6c75 7465 2829 2061 6e64 2070  absolute() and p
+000188a0: 203d 3d20 5061 7468 2822 7368 6172 6564   == Path("shared
+000188b0: 5f72 6573 6f75 7263 6573 2f72 7379 736c  _resources/rsysl
+000188c0: 6f67 2f6c 6f67 7322 293a 0a20 2020 2020  og/logs"):.     
+000188d0: 2020 2020 2020 2020 2020 2077 726f 6e67             wrong
+000188e0: 5f68 6f73 745f 7061 7468 203d 2046 616c  _host_path = Fal
+000188f0: 7365 0a20 2020 2020 2020 2020 2020 2020  se.             
+00018900: 2020 2062 7265 616b 0a20 2020 2020 2020     break.       
+00018910: 2020 2020 2065 6c69 6620 702e 6973 5f61       elif p.is_a
+00018920: 6273 6f6c 7574 6528 2920 616e 6420 5061  bsolute() and Pa
+00018930: 7468 2873 7472 2870 295b 313a 5d29 203d  th(str(p)[1:]) =
+00018940: 3d20 5061 7468 280a 2020 2020 2020 2020  = Path(.        
+00018950: 2020 2020 2020 2020 2273 6861 7265 645f          "shared_
+00018960: 7265 736f 7572 6365 732f 7273 7973 6c6f  resources/rsyslo
+00018970: 672f 6c6f 6773 220a 2020 2020 2020 2020  g/logs".        
+00018980: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
+00018990: 2020 2020 2020 2077 726f 6e67 5f68 6f73         wrong_hos
+000189a0: 745f 7061 7468 203d 2046 616c 7365 0a20  t_path = False. 
+000189b0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+000189c0: 7265 616b 0a20 2020 2020 2020 2020 2020  reak.           
+000189d0: 2065 6c69 6620 702e 6973 5f61 6273 6f6c   elif p.is_absol
+000189e0: 7574 6528 2920 616e 6420 7020 3d3d 2050  ute() and p == P
+000189f0: 6174 6828 0a20 2020 2020 2020 2020 2020  ath(.           
+00018a00: 2020 2020 2022 2f63 7962 6572 2d72 616e       "/cyber-ran
+00018a10: 6765 2d63 6174 616c 6f67 2f73 696d 756c  ge-catalog/simul
+00018a20: 6174 696f 6e73 5f72 6573 6f75 7263 6573  ations_resources
+00018a30: 2f31 2f73 6861 7265 645f 7265 736f 7572  /1/shared_resour
+00018a40: 6365 732f 7273 7973 6c6f 672f 6c6f 6773  ces/rsyslog/logs
+00018a50: 220a 2020 2020 2020 2020 2020 2020 293a  ".            ):
+00018a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018a70: 2077 726f 6e67 5f68 6f73 745f 7061 7468   wrong_host_path
+00018a80: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
+00018a90: 2020 2020 2020 2020 2062 7265 616b 0a0a           break..
+00018aa0: 2020 2020 2020 2020 6966 2077 726f 6e67          if wrong
+00018ab0: 5f68 6f73 745f 7061 7468 3a0a 2020 2020  _host_path:.    
+00018ac0: 2020 2020 2020 2020 6c6f 6767 6572 2e65          logger.e
+00018ad0: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
+00018ae0: 2020 2020 2020 2220 205b 2b5d 2049 7420        "  [+] It 
+00018af0: 7365 656d 7320 7468 6174 2074 6865 2073  seems that the s
+00018b00: 696d 756c 6174 696f 6e20 696e 636c 7564  imulation includ
+00018b10: 6573 2074 6865 2027 7273 7973 6c6f 6727  es the 'rsyslog'
+00018b20: 2064 6f63 6b65 7220 7468 6174 2063 6f6c   docker that col
+00018b30: 6c65 6374 7320 7468 6520 6c6f 6773 2c20  lects the logs, 
+00018b40: 6275 7420 646f 6573 206e 6f74 2073 7065  but does not spe
+00018b50: 6369 6679 2074 6865 2061 7070 726f 7072  cify the appropr
+00018b60: 6961 7465 2068 6f73 745f 7061 7468 2066  iate host_path f
+00018b70: 6f72 2074 6865 206c 6f67 732e 2049 7420  or the logs. It 
+00018b80: 6973 2065 7870 6563 7465 6420 7468 6174  is expected that
+00018b90: 2074 6865 2072 7379 736c 6f67 2064 6f63   the rsyslog doc
+00018ba0: 6b65 7220 6e6f 6465 2073 7065 6369 6669  ker node specifi
+00018bb0: 6573 2061 2028 7772 6974 6162 6c65 2920  es a (writable) 
+00018bc0: 766f 6c75 6d65 2077 6974 6820 6120 686f  volume with a ho
+00018bd0: 7374 5f70 6174 6820 6571 7561 6c20 746f  st_path equal to
+00018be0: 2027 2f73 6861 7265 645f 7265 736f 7572   '/shared_resour
+00018bf0: 6365 732f 7273 7973 6c6f 672f 6c6f 6773  ces/rsyslog/logs
+00018c00: 272e 2043 616e 6469 6461 7465 7320 6172  '. Candidates ar
+00018c10: 6520 277b 7d27 2069 6e73 7465 6164 2e22  e '{}' instead."
+00018c20: 2e66 6f72 6d61 7428 0a20 2020 2020 2020  .format(.       
+00018c30: 2020 2020 2020 2020 2020 2020 205b 7374               [st
+00018c40: 7228 7029 2066 6f72 2070 2069 6e20 706f  r(p) for p in po
+00018c50: 7465 6e74 6961 6c5f 6c6f 6773 5f61 6273  tential_logs_abs
+00018c60: 6f6c 7574 655f 7061 7468 5d2c 0a20 2020  olute_path],.   
+00018c70: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+00018c80: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00018c90: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+00018ca0: 6572 726f 7228 0a20 2020 2020 2020 2020  error(.         
+00018cb0: 2020 2020 2020 2022 205b 2b5d 2044 6174         " [+] Dat
+00018cc0: 6173 6574 2063 7265 6174 696f 6e20 6162  aset creation ab
+00018cd0: 6f72 7465 642e 2059 6f75 206d 6179 2077  orted. You may w
+00018ce0: 6973 6820 746f 206d 6f76 6520 7468 6520  ish to move the 
+00018cf0: 6c6f 6720 6669 6c65 7320 746f 2074 6865  log files to the
+00018d00: 2061 7070 726f 7072 6961 7465 2066 6f6c   appropriate fol
+00018d10: 6465 7220 6f6e 2074 6865 2063 6f6d 7075  der on the compu
+00018d20: 7465 2073 6572 7665 7228 7329 2c20 616e  te server(s), an
+00018d30: 6420 7468 656e 2072 6574 7279 2e20 416c  d then retry. Al
+00018d40: 7465 726e 6174 6976 656c 792c 2079 6f75  ternatively, you
+00018d50: 2063 616e 2062 7970 6173 7320 7468 6973   can bypass this
+00018d60: 2063 6865 636b 2077 6974 6820 7468 6520   check with the 
+00018d70: 646f 6e74 5f63 6865 636b 5f6c 6f67 5f70  dont_check_log_p
+00018d80: 6174 6820 6f70 7469 6f6e 2e22 0a20 2020  ath option.".   
+00018d90: 2020 2020 2020 2020 2029 0a0a 0a64 6566           )...def
+00018da0: 2073 746f 705f 6461 7461 7365 745f 6372   stop_dataset_cr
+00018db0: 6561 7469 6f6e 2864 6174 6173 6574 5f69  eation(dataset_i
+00018dc0: 643a 2075 7569 642e 5555 4944 2920 2d3e  d: uuid.UUID) ->
+00018dd0: 2041 6e79 3a0a 2020 2020 2222 220a 2020   Any:.    """.  
+00018de0: 2020 5374 6f70 732f 6162 6f72 7473 2074    Stops/aborts t
+00018df0: 6865 2063 7265 6174 696f 6e20 6f66 2061  he creation of a
+00018e00: 2064 6174 6173 6574 2074 6861 7420 6973   dataset that is
+00018e10: 2069 6e20 7468 6520 7072 6f63 6573 7320   in the process 
+00018e20: 6f66 2062 6569 6e67 2063 7265 6174 6564  of being created
+00018e30: 2e0a 0a20 2020 2054 6869 7320 6675 6e63  ...    This func
+00018e40: 7469 6f6e 2073 686f 756c 6420 6265 2075  tion should be u
+00018e50: 7365 642c 2066 6f72 2069 6e73 7461 6e63  sed, for instanc
+00018e60: 652c 2069 6620 6120 6461 7461 7365 7420  e, if a dataset 
+00018e70: 6372 6561 7469 6f6e 2068 6173 2062 6565  creation has bee
+00018e80: 6e0a 2020 2020 6175 746f 6d61 7469 6361  n.    automatica
+00018e90: 6c6c 7920 7374 6172 7465 6420 616c 7468  lly started alth
+00018ea0: 6f75 6768 2074 6865 2075 7365 7220 646f  ough the user do
+00018eb0: 6573 206e 6f74 2077 616e 7420 6120 6461  es not want a da
+00018ec0: 7461 7365 742c 2061 6e64 2074 6865 2064  taset, and the d
+00018ed0: 6174 6173 6574 0a20 2020 2063 7265 6174  ataset.    creat
+00018ee0: 696f 6e20 7072 6f63 6573 7320 6973 2074  ion process is t
+00018ef0: 616b 696e 6720 746f 6f20 6d75 6368 2074  aking too much t
+00018f00: 696d 652e 0a0a 2020 2020 5741 524e 494e  ime...    WARNIN
+00018f10: 473a 2061 6674 6572 2073 746f 7070 696e  G: after stoppin
+00018f20: 6720 7468 6520 6461 7461 7365 7420 6372  g the dataset cr
+00018f30: 6561 7469 6f6e 2c20 6974 2069 7320 6164  eation, it is ad
+00018f40: 7669 7365 6420 746f 2064 656c 6574 6520  vised to delete 
+00018f50: 6f72 2061 7420 6c65 6173 740a 2020 2020  or at least.    
+00018f60: 7265 7061 6972 2074 6865 2064 6174 6173  repair the datas
+00018f70: 6574 2e0a 0a20 2020 203a 7061 7261 6d20  et...    :param 
+00018f80: 6461 7461 7365 745f 6964 3a20 5468 6520  dataset_id: The 
+00018f90: 6461 7461 7365 7420 4944 2077 6869 6368  dataset ID which
+00018fa0: 2069 7320 696e 2074 6865 2070 726f 6365   is in the proce
+00018fb0: 7373 206f 6620 6265 696e 6720 6372 6561  ss of being crea
+00018fc0: 7465 6420 616e 6420 7468 6174 206d 7573  ted and that mus
+00018fd0: 7420 6265 2061 626f 7274 6564 2e0a 2020  t be aborted..  
+00018fe0: 2020 3a72 6574 7572 6e3a 2052 6574 7572    :return: Retur
+00018ff0: 6e20 7468 6520 6a73 6f6e 2062 6f64 7920  n the json body 
+00019000: 6f66 2074 6865 2063 6f72 6520 4150 4920  of the core API 
+00019010: 7265 7370 6f6e 7365 2e0a 0a20 2020 2022  response...    "
+00019020: 2222 0a20 2020 2023 2053 696d 706c 7920  "".    # Simply 
+00019030: 6361 6c6c 7320 7468 6520 636f 7265 2041  calls the core A
+00019040: 5049 2077 6869 6368 2069 7473 656c 6620  PI which itself 
+00019050: 6173 6b73 2074 6865 2070 7562 6c69 7368  asks the publish
+00019060: 0a20 2020 2023 2073 6572 7665 7220 2862  .    # server (b
+00019070: 6163 6b65 6e64 2920 746f 2073 746f 7020  ackend) to stop 
+00019080: 6f66 2074 6865 2064 6174 6173 6574 2063  of the dataset c
+00019090: 7265 6174 696f 6e20 7072 6f63 6573 732e  reation process.
+000190a0: 0a0a 2020 2020 7265 7375 6c74 203d 205f  ..    result = _
+000190b0: 7075 7428 222f 6372 6561 7465 5f64 6174  put("/create_dat
+000190c0: 6173 6574 2f73 746f 702f 7b7d 222e 666f  aset/stop/{}".fo
+000190d0: 726d 6174 2873 7472 2864 6174 6173 6574  rmat(str(dataset
+000190e0: 5f69 6429 2929 0a0a 2020 2020 6966 2072  _id)))..    if r
+000190f0: 6573 756c 742e 7374 6174 7573 5f63 6f64  esult.status_cod
+00019100: 6520 213d 2032 3030 3a0a 2020 2020 2020  e != 200:.      
+00019110: 2020 5f68 616e 646c 655f 6572 726f 7228    _handle_error(
+00019120: 7265 7375 6c74 2c20 2243 616e 6e6f 7420  result, "Cannot 
+00019130: 7374 6f70 2064 6174 6173 6574 2063 7265  stop dataset cre
+00019140: 6174 696f 6e20 7468 726f 7567 6820 636f  ation through co
+00019150: 7265 2041 5049 2229 0a0a 2020 2020 7265  re API")..    re
+00019160: 7475 726e 2072 6573 756c 742e 6a73 6f6e  turn result.json
+00019170: 2829 0a0a 0a64 6566 2066 6574 6368 5f63  ()...def fetch_c
+00019180: 6f6d 7075 7465 5f73 6572 7665 7228 636f  ompute_server(co
+00019190: 6d70 7574 655f 7365 7276 6572 5f69 643a  mpute_server_id:
+000191a0: 2069 6e74 2920 2d3e 2041 6e79 3a0a 2020   int) -> Any:.  
+000191b0: 2020 2222 2252 6574 7572 6e20 6120 636f    """Return a co
+000191c0: 6d70 7574 6520 7365 7276 6572 2067 6976  mpute server giv
+000191d0: 656e 2069 7473 2049 442e 0a0a 2020 2020  en its ID...    
+000191e0: 3a72 6574 7572 6e3a 2054 6865 2063 6f6d  :return: The com
+000191f0: 7075 7465 2073 6572 7665 7220 6469 6374  pute server dict
+00019200: 2e0a 0a20 2020 203a 7061 7261 6d20 636f  ...    :param co
+00019210: 6d70 7574 655f 7365 7276 6572 5f69 643a  mpute_server_id:
+00019220: 2054 6865 2063 6f6d 7075 7465 2073 6572   The compute ser
+00019230: 7665 7220 4944 2e0a 0a20 2020 2022 2222  ver ID...    """
+00019240: 0a20 2020 2072 6573 756c 7420 3d20 5f67  .    result = _g
+00019250: 6574 2866 222f 636f 6d70 7574 655f 7365  et(f"/compute_se
+00019260: 7276 6572 732f 7b63 6f6d 7075 7465 5f73  rvers/{compute_s
+00019270: 6572 7665 725f 6964 7d22 290a 0a20 2020  erver_id}")..   
+00019280: 2069 6620 7265 7375 6c74 2e73 7461 7475   if result.statu
+00019290: 735f 636f 6465 2021 3d20 3230 303a 0a20  s_code != 200:. 
+000192a0: 2020 2020 2020 205f 6861 6e64 6c65 5f65         _handle_e
+000192b0: 7272 6f72 2872 6573 756c 742c 2022 4361  rror(result, "Ca
+000192c0: 6e6e 6f74 2072 6574 7269 6576 6520 6e6f  nnot retrieve no
+000192d0: 6465 2066 726f 6d20 4954 2053 696d 756c  de from IT Simul
+000192e0: 6174 696f 6e20 4150 4922 290a 0a20 2020  ation API")..   
+000192f0: 2072 6574 7572 6e20 7265 7375 6c74 2e6a   return result.j
+00019300: 736f 6e28 290a 0a0a 6465 6620 6665 7463  son()...def fetc
+00019310: 685f 636f 6d70 7574 655f 7365 7276 6572  h_compute_server
+00019320: 5f62 795f 6e6f 6465 5f69 6428 6e6f 6465  _by_node_id(node
+00019330: 5f69 643a 2069 6e74 2920 2d3e 2041 6e79  _id: int) -> Any
+00019340: 3a0a 2020 2020 2222 2252 6574 7572 6e20  :.    """Return 
+00019350: 6120 636f 6d70 7574 6520 7365 7276 6572  a compute server
+00019360: 2077 6865 7265 2061 206e 6f64 6520 4944   where a node ID
+00019370: 2069 7320 7275 6e6e 696e 672e 0a0a 2020   is running...  
+00019380: 2020 3a72 6574 7572 6e3a 2054 6865 2063    :return: The c
+00019390: 6f6d 7075 7465 2073 6572 7665 7220 6469  ompute server di
+000193a0: 6374 2e0a 0a20 2020 203a 7061 7261 6d20  ct...    :param 
+000193b0: 6e6f 6465 5f69 643a 2054 6865 206e 6f64  node_id: The nod
+000193c0: 6520 4944 2074 6f20 6c6f 6f6b 2066 6f72  e ID to look for
+000193d0: 2e0a 0a20 2020 2022 2222 0a20 2020 2072  ...    """.    r
+000193e0: 6573 756c 7420 3d20 5f67 6574 2866 222f  esult = _get(f"/
+000193f0: 636f 6d70 7574 655f 7365 7276 6572 732f  compute_servers/
+00019400: 6e6f 6465 2f7b 6e6f 6465 5f69 647d 2229  node/{node_id}")
+00019410: 0a0a 2020 2020 6966 2072 6573 756c 742e  ..    if result.
+00019420: 7374 6174 7573 5f63 6f64 6520 213d 2032  status_code != 2
+00019430: 3030 3a0a 2020 2020 2020 2020 5f68 616e  00:.        _han
+00019440: 646c 655f 6572 726f 7228 7265 7375 6c74  dle_error(result
+00019450: 2c20 2243 616e 6e6f 7420 7265 7472 6965  , "Cannot retrie
+00019460: 7665 206e 6f64 6520 6672 6f6d 2049 5420  ve node from IT 
+00019470: 5369 6d75 6c61 7469 6f6e 2041 5049 2229  Simulation API")
+00019480: 0a0a 2020 2020 7265 7475 726e 2072 6573  ..    return res
+00019490: 756c 742e 6a73 6f6e 2829 0a0a 0a64 6566  ult.json()...def
+000194a0: 2066 6574 6368 5f63 6f6d 7075 7465 5f73   fetch_compute_s
+000194b0: 6572 7665 7273 2829 202d 3e20 4c69 7374  ervers() -> List
+000194c0: 5b44 6963 745b 7374 722c 2041 6e79 5d5d  [Dict[str, Any]]
+000194d0: 3a0a 2020 2020 2222 220a 2020 2020 5265  :.    """.    Re
+000194e0: 7475 726e 2074 6865 206c 6973 7420 6f66  turn the list of
+000194f0: 2063 6f6d 7075 7465 2073 6572 7665 7273   compute servers
+00019500: 2061 7320 6b6e 6f77 6e20 696e 2064 6174   as known in dat
+00019510: 6162 6173 652e 0a0a 2020 2020 3a72 6574  abase...    :ret
+00019520: 7572 6e3a 2054 6865 206c 6973 7420 6f66  urn: The list of
+00019530: 2063 6f6d 7075 7465 2073 6572 7665 7220   compute server 
+00019540: 6469 6374 732e 0a0a 2020 2020 2222 220a  dicts...    """.
+00019550: 2020 2020 7265 7375 6c74 203d 205f 6765      result = _ge
+00019560: 7428 222f 636f 6d70 7574 655f 7365 7276  t("/compute_serv
+00019570: 6572 732f 2229 0a0a 2020 2020 6966 2072  ers/")..    if r
+00019580: 6573 756c 742e 7374 6174 7573 5f63 6f64  esult.status_cod
+00019590: 6520 213d 2032 3030 3a0a 2020 2020 2020  e != 200:.      
+000195a0: 2020 5f68 616e 646c 655f 6572 726f 7228    _handle_error(
+000195b0: 7265 7375 6c74 2c20 2243 616e 6e6f 7420  result, "Cannot 
+000195c0: 7265 7472 6965 7665 2063 6f6d 7075 7465  retrieve compute
+000195d0: 2073 6572 7665 7273 2066 726f 6d20 4954   servers from IT
+000195e0: 2053 696d 756c 6174 696f 6e20 4150 4922   Simulation API"
+000195f0: 290a 0a20 2020 2072 6574 7572 6e20 7265  )..    return re
+00019600: 7375 6c74 2e6a 736f 6e28 290a 0a0a 6465  sult.json()...de
+00019610: 6620 6465 6c65 7465 5f63 6f6d 7075 7465  f delete_compute
+00019620: 5f73 6572 7665 7228 636f 6d70 7574 655f  _server(compute_
+00019630: 7365 7276 6572 5f69 643a 2069 6e74 2920  server_id: int) 
+00019640: 2d3e 204e 6f6e 653a 0a20 2020 2022 2222  -> None:.    """
+00019650: 0a20 2020 2044 656c 6574 6573 2061 2063  .    Deletes a c
+00019660: 6f6d 7075 7465 2073 6572 7665 7220 696e  ompute server in
+00019670: 2064 6174 6162 6173 6520 7573 696e 6720   database using 
+00019680: 6974 7320 6964 2e0a 0a20 2020 2043 6f6d  its id...    Com
+00019690: 7075 7465 2073 6572 7665 7273 2069 6473  pute servers ids
+000196a0: 2063 616e 2062 6520 6f62 7461 696e 6564   can be obtained
+000196b0: 2074 6872 6f75 6768 2060 6379 6265 725f   through `cyber_
+000196c0: 7261 6e67 6520 7374 6174 7573 6020 6f72  range status` or
+000196d0: 203a 6675 6e63 3a60 6665 7463 685f 636f   :func:`fetch_co
+000196e0: 6d70 7574 655f 7365 7276 6572 602e 0a0a  mpute_server`...
+000196f0: 2020 2020 3a70 6172 616d 2063 6f6d 7075      :param compu
+00019700: 7465 5f73 6572 7665 725f 6964 3a20 5468  te_server_id: Th
+00019710: 6520 636f 6d70 7574 6520 7365 7276 6572  e compute server
+00019720: 2049 442e 0a0a 2020 2020 2222 220a 2020   ID...    """.  
+00019730: 2020 7265 7375 6c74 203d 205f 6465 6c65    result = _dele
+00019740: 7465 2866 222f 636f 6d70 7574 655f 7365  te(f"/compute_se
+00019750: 7276 6572 732f 7b63 6f6d 7075 7465 5f73  rvers/{compute_s
+00019760: 6572 7665 725f 6964 7d22 290a 0a20 2020  erver_id}")..   
+00019770: 2069 6620 7265 7375 6c74 2e73 7461 7475   if result.statu
+00019780: 735f 636f 6465 2021 3d20 3230 303a 0a20  s_code != 200:. 
+00019790: 2020 2020 2020 205f 6861 6e64 6c65 5f65         _handle_e
+000197a0: 7272 6f72 2872 6573 756c 742c 2022 4361  rror(result, "Ca
+000197b0: 6e6e 6f74 2064 656c 6574 6520 636f 6d70  nnot delete comp
+000197c0: 7574 6520 7365 7276 6572 2069 6e20 636f  ute server in co
+000197d0: 7265 2041 5049 2229 0a0a 2020 2020 7265  re API")..    re
+000197e0: 7475 726e 2072 6573 756c 742e 6a73 6f6e  turn result.json
+000197f0: 2829 0a                                  ().
```

### Comparing `cr_api_client-4.1.0/cr_api_client/cyber_range.py` & `cr_api_client-4.3.0/cr_api_client/cyber_range.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,17 @@
 import shutil
 import sys
 import time
 import uuid
 from collections import OrderedDict
 from pathlib import Path
 from typing import Any
+from typing import Dict
+from typing import List
+from typing import Set
 
 import argcomplete
 import requests
 from loguru import logger
 from omegaconf import OmegaConf
 
 try:
@@ -506,41 +509,114 @@
     :param args: args.basebox_id (optional)
     :return: None
     """
 
     requested_basebox_id = args.basebox_id
 
     if requested_basebox_id is None:
-        logger.info("[+] Verifying the checksums of available baseboxes")
-        result = core_api.verify_baseboxes()
-        for basebox_result in result["result"]:
-            if basebox_result["result"]:
-                logger.info(
-                    "[+] {} has the correct checksum.".format(
-                        basebox_result["basebox_id"]
+        _baseboxes_verify_all_handler()
+    else:
+        _baseboxes_verify_one_handler(requested_basebox_id)
+
+
+def _baseboxes_verify_all_handler() -> None:
+    """
+    Handler for the verification of all the baseboxes
+    :return: None
+    """
+    logger.info("[+] Verifying the checksums of available baseboxes")
+    result = core_api.verify_baseboxes()
+    if "result" not in result or not result["result"]:
+        logger.warning("[+] No result received...")
+    else:
+        compute_servers_with_valid_checksums: Dict[str, List[str]] = {}
+        compute_servers_with_nonmissing_result: Dict[str, List[str]] = {}
+        all_baseboxes: Set[str] = set()
+        for compute_server_name, baseboxes_checksums in result["result"].items():
+            for bb_id, verification_result in baseboxes_checksums.items():
+                all_baseboxes.add(bb_id)
+                if bb_id not in compute_servers_with_valid_checksums:
+                    compute_servers_with_valid_checksums[bb_id] = []
+                if bb_id not in compute_servers_with_nonmissing_result:
+                    compute_servers_with_nonmissing_result[bb_id] = []
+
+                if verification_result is not None:
+                    compute_servers_with_nonmissing_result[bb_id].append(
+                        compute_server_name
+                    )
+                if verification_result:
+                    compute_servers_with_valid_checksums[bb_id].append(
+                        compute_server_name
+                    )
+
+        for bb_id in all_baseboxes:
+            compute_servers_with_missing_result = [
+                cs_name
+                for cs_name in result["result"].keys()
+                if cs_name not in compute_servers_with_nonmissing_result[bb_id]
+            ]
+            compute_servers_with_invalid_checksums = [
+                cs_name
+                for cs_name in result["result"].keys()
+                if cs_name not in compute_servers_with_valid_checksums[bb_id]
+                and cs_name in compute_servers_with_nonmissing_result[bb_id]
+            ]
+            if (
+                compute_servers_with_invalid_checksums
+                or compute_servers_with_missing_result
+            ):
+                if compute_servers_with_invalid_checksums:
+                    logger.error(
+                        f"[+] {bb_id} has an incorrect checksum on {len(compute_servers_with_invalid_checksums)} (out of {len(result['result'])}) compute severs: {', '.join(compute_servers_with_invalid_checksums)}."
+                    )
+                if compute_servers_with_missing_result:
+                    logger.error(
+                        f"[+] No result for verification of {bb_id} on {len(compute_servers_with_missing_result)} (out of {len(result['result'])}) compute severs: {', '.join(compute_servers_with_missing_result)}."
                     )
-                )
             else:
-                logger.error(
-                    "[+] {} has not the correct checksum.".format(
-                        basebox_result["basebox_id"]
-                    )
+                logger.info(
+                    f"[+] {bb_id} has the correct checksum on all compute servers."
                 )
+    logger.info("[+] Done")
 
-    else:
-        logger.info(
-            "[+] Verifying the checksum of basebox {}".format(requested_basebox_id)
-        )
-        result = core_api.verify_basebox(requested_basebox_id)
-        if result["valid_checksum"]:
-            logger.info("[+] {} has the correct checksum.".format(requested_basebox_id))
+
+def _baseboxes_verify_one_handler(requested_basebox_id: str) -> None:
+    logger.info("[+] Verifying the checksum of basebox {}".format(requested_basebox_id))
+    result = core_api.verify_basebox(requested_basebox_id)
+    if "result" not in result or not result["result"]:
+        logger.warning("[+] No result received...")
+    else:
+        compute_servers_with_invalid_checksums: List[str] = []
+        compute_servers_with_missing_result: List[str] = []
+        for compute_server_name, baseboxes_checksums in result["result"].items():
+            if (
+                requested_basebox_id not in baseboxes_checksums
+                or baseboxes_checksums[requested_basebox_id] is None
+            ):
+                compute_servers_with_missing_result.append(compute_server_name)
+            elif not baseboxes_checksums[requested_basebox_id]:
+                compute_servers_with_invalid_checksums.append(compute_server_name)
+
+        if (
+            compute_servers_with_invalid_checksums
+            or compute_servers_with_missing_result
+        ):
+            if compute_servers_with_invalid_checksums:
+                logger.error(
+                    f"[+] {requested_basebox_id} has an incorrect checksum on {len(compute_servers_with_invalid_checksums)} (out of {len(result['result'])}) compute severs: {', '.join(compute_servers_with_invalid_checksums)}."
+                )
+            if compute_servers_with_missing_result:
+                logger.error(
+                    f"[+] No result for verification of {requested_basebox_id} on {len(compute_servers_with_missing_result)} (out of {len(result['result'])}) compute severs: {', '.join(compute_servers_with_missing_result)}."
+                )
         else:
-            logger.error(
-                "[+] {} has not the correct checksum.".format(requested_basebox_id)
+            logger.info(
+                f"[+] {requested_basebox_id} has the correct checksum on all compute servers."
             )
+
     logger.info("[+] Done")
 
 
 #
 # 'websites_list' related functions
 #
 def websites_list_handler(args: Any) -> None:
@@ -2348,91 +2424,64 @@
     logger.info("[+] Report from redteam API")
     report = redteam_api.scenario_result()
 
     pp = pprint.PrettyPrinter(width=160)
     pp.pprint(report)
 
 
-def main() -> None:
+def create_cyber_range_cli_parser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser()
 
     # Config file argument
     parser.add_argument("--config", help="Configuration file")
 
     # Common debug argument
     parser.add_argument(
         "-d",
         "--debug",
         action="store_true",
         dest="debug_mode",
         help="Activate debug mode (default: %(default)s)",
     )
 
-    # Common options to access remote API
-    options_by_dest = dict()
-
-    option_name = "--core-url"
-    dest_name = "core_api_url"
-    options_by_dest[dest_name] = option_name
     parser.add_argument(
         "--core-url",
         dest="core_api_url",
         help="Set core API URL (default: %(default)r)",
     )
 
-    option_name = "--user-activity-url"
-    dest_name = "user_activity_api_url"
-    options_by_dest[dest_name] = option_name
     parser.add_argument(
-        option_name,
-        dest=dest_name,
+        "--user-activity-url",
+        dest="user_activity_api_url",
         help="Set user_activity API URL (default: %(default)r)",
     )
 
-    option_name = "--provisioning-url"
-    dest_name = "provisioning_api_url"
-    options_by_dest[dest_name] = option_name
     parser.add_argument(
-        option_name,
-        dest=dest_name,
+        "--provisioning-url",
+        dest="provisioning_api_url",
         help="Set provisioning API URL (default: %(default)r)",
     )
 
-    option_name = "--redteam-url"
-    dest_name = "redteam_api_url"
-    options_by_dest[dest_name] = option_name
     parser.add_argument(
-        option_name,
-        dest=dest_name,
+        "--redteam-url",
+        dest="redteam_api_url",
         help="Set redteam API URL (default: %(default)r)",
     )
 
-    option_name = "--publish-url"
-    dest_name = "publish_api_url"
-    options_by_dest[dest_name] = option_name
     parser.add_argument(
-        option_name,
-        dest=dest_name,
+        "--publish-url",
+        dest="publish_api_url",
         help="Set publish API URL (default: %(default)r)",
     )
 
-    option_name = "--cacert"
-    dest_name = "cacert"
-    options_by_dest[dest_name] = option_name
-    parser.add_argument(option_name, dest=dest_name, help="Set path to CA certs")
-
-    option_name = "--cert"
-    dest_name = "cert"
-    options_by_dest[dest_name] = option_name
-    parser.add_argument(option_name, dest=dest_name, help="Set path to client cert")
-
-    option_name = "--key"
-    dest_name = "key"
-    options_by_dest[dest_name] = option_name
-    parser.add_argument(option_name, dest=dest_name, help="Set path to client key")
+    parser.add_argument("--cacert", dest="cacert", help="Set path to CA certs")
+
+    parser.add_argument("--cert", dest="cert", help="Set path to client cert")
+
+    parser.add_argument("--key", dest="key", help="Set path to client key")
 
     subparsers = parser.add_subparsers()
 
     # 'status' command
     parser_status = subparsers.add_parser("status", help="Get platform status")
     parser_status.set_defaults(func=status_handler)
 
@@ -2739,15 +2788,16 @@
     parser_simu_destroy.set_defaults(func=simu_destroy_handler)
     parser_simu_destroy.add_argument(
         "id_simulation", type=int, help="The simulation id"
     )
 
     # 'simu_snap' simulation command
     parser_simu_snap = subparsers.add_parser(
-        "simu_snap", help="Get status of a simulation or all simulations"
+        "simu_snap",
+        help="Create a snapshot of the entire simulation, that can be restored afterwards",
     )
     parser_simu_snap.set_defaults(func=simu_snap_handler)
     parser_simu_snap.add_argument("id_simulation", type=int, help="The simulation id")
     parser_simu_snap.add_argument(
         "-o",
         "--output",
         type=str,
@@ -3533,14 +3583,20 @@
     # 'redteam_report' command
     parser_redteam_report = subparsers.add_parser(
         "redteam_report",
         help="Get redteam scenario report",
     )
     parser_redteam_report.set_defaults(func=redteam_report_handler)
 
+    return parser
+
+
+def main() -> None:
+    parser = create_cyber_range_cli_parser()
+
     argcomplete.autocomplete(parser)
 
     parser_defaults = {
         k: cr_api_client_config[k]
         for k in cr_api_client_config
         if not OmegaConf.is_missing(cr_api_client_config, k)
     }
@@ -3560,26 +3616,37 @@
         logger.info(f"  [+] Using config file: {configfile_path}")
         if not os.path.exists(configfile_path):
             raise Exception(f"Path '{configfile_path}' does not exist.")
         config = configparser.SafeConfigParser()
         fp = open(configfile_path)
         config.readfp(fp)
 
+        # Common options to access remote API
+        options_by_dest = dict()
+        options_by_dest["core_api_url"] = "--core-url"
+        options_by_dest["user_activity_api_url"] = "--user-activity-url"
+        options_by_dest["provisioning_api_url"] = "--provisioning-url"
+        options_by_dest["redteam_api_url"] = "--redteam-url"
+        options_by_dest["publish_api_url"] = "--publish-url"
+        options_by_dest["cacert"] = "--cacert"
+        options_by_dest["cert"] = "--cert"
+        options_by_dest["key"] = "--key"
+
         # find options defined in command line
         args_in_command_line = list()
         args_as_dict = vars(args)
         for key, value in args_as_dict.items():
             if key in options_by_dest and value is not None:
                 args_in_command_line.append(options_by_dest[key])
 
         for k, v in config.items("DEFAULT"):
             # if the argument is also in the command line, it overwrites the one present in the config file
             if k in args_in_command_line:
                 logger.info(
-                    f"  [+] Skipping '{option_name}' option defined in config file (already defined in command line)"
+                    f"  [+] Skipping '{k}' option defined in config file (already defined in command line)"
                 )
             else:
                 parser.parse_args([str(k), str(v)], args)
 
         fp.close()
 
     # Parse remaining args from command line (overriding potential config file
```

### Comparing `cr_api_client-4.1.0/cr_api_client/provisioning_api.py` & `cr_api_client-4.3.0/cr_api_client/provisioning_api.py`

 * *Files identical despite different names*

### Comparing `cr_api_client-4.1.0/cr_api_client/publish_api.py` & `cr_api_client-4.3.0/cr_api_client/publish_api.py`

 * *Files identical despite different names*

### Comparing `cr_api_client-4.1.0/cr_api_client/redteam_api.py` & `cr_api_client-4.3.0/cr_api_client/redteam_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -597,15 +597,15 @@
 
     for elt in data:
         key = list(elt)[0]
         output[key] = elt[key]
 
     url = "/knowledge"
     headers = {"Content-type": "application/json"}
-    result = _post(url, headers=headers, data=json.dumps(output), timeout=10)
+    result = _post(url, headers=headers, data=json.dumps(output))
 
     if result.status_code != 200:
         _handle_error(result, "Cannot initialize knowledge database from redteam API")
     else:
         return True
```

### Comparing `cr_api_client-4.1.0/cr_api_client/topology/TopologyElements.py` & `cr_api_client-4.3.0/cr_api_client/topology/TopologyElements.py`

 * *Files identical despite different names*

### Comparing `cr_api_client-4.1.0/cr_api_client/topology/TopologyGenerator.py` & `cr_api_client-4.3.0/cr_api_client/topology/TopologyGenerator.py`

 * *Files identical despite different names*

### Comparing `cr_api_client-4.1.0/cr_api_client/topology/TopologyLinksGenerator.py` & `cr_api_client-4.3.0/cr_api_client/topology/TopologyLinksGenerator.py`

 * *Files identical despite different names*

### Comparing `cr_api_client-4.1.0/cr_api_client/topology/TopologyNodeGenerator.py` & `cr_api_client-4.3.0/cr_api_client/topology/TopologyNodeGenerator.py`

 * *Files identical despite different names*

### Comparing `cr_api_client-4.1.0/cr_api_client/topology/TopologyNodesGenerator.py` & `cr_api_client-4.3.0/cr_api_client/topology/TopologyNodesGenerator.py`

 * *Files identical despite different names*

### Comparing `cr_api_client-4.1.0/cr_api_client/topology/validator/common.py` & `cr_api_client-4.3.0/cr_api_client/topology/validator/common.py`

 * *Files identical despite different names*

### Comparing `cr_api_client-4.1.0/cr_api_client/topology/validator/link.py` & `cr_api_client-4.3.0/cr_api_client/topology/validator/link.py`

 * *Files identical despite different names*

### Comparing `cr_api_client-4.1.0/cr_api_client/topology/validator/node.py` & `cr_api_client-4.3.0/cr_api_client/topology/validator/node.py`

 * *Files identical despite different names*

### Comparing `cr_api_client-4.1.0/cr_api_client/topology/validator/topology.py` & `cr_api_client-4.3.0/cr_api_client/topology/validator/topology.py`

 * *Files identical despite different names*

### Comparing `cr_api_client-4.1.0/cr_api_client/user_activity_api.py` & `cr_api_client-4.3.0/cr_api_client/user_activity_api.py`

 * *Files identical despite different names*

### Comparing `cr_api_client-4.1.0/cr_api_client/yaml_helper.py` & `cr_api_client-4.3.0/cr_api_client/yaml_helper.py`

 * *Files identical despite different names*

### Comparing `cr_api_client-4.1.0/pyproject.toml` & `cr_api_client-4.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cr_api_client"
-version = "4.1.0"
+version = "4.3.0"
 description = "AMOSSYS Cyber Range client API"
 readme = "README.md"
 authors = ["AMOSSYS"]
 packages = [
     { include = "cr_api_client" },
 ]
 license = "MIT"
@@ -20,14 +20,15 @@
 argcomplete = "~1.12.1"
 setuptools = "44.0.0"  # Needed to fix pex issue related to ruamel.yaml dependency
 Jinja2 = "~2.11.3" # Needed to play ./data/scenarios*
 pypsrp = "~0.5.0" # Needed to play ./data/scenarios*
 pydantic = "~1.10.2" # Needed to play ./data/scenarios*
 markupsafe = "2.0.1" # Need to fix version to resolve 'soft_unicode' needed by jinja2
 omegaconf = "^2.2.2"
+types-jinja2 = "^2.11.9" # Needed for typing and mypy, remove when updating to Jinja2 version 3 or more
 
 [tool.poetry.group.dev.dependencies]
 cr_dataset_model = {path = "../libs/cr_dataset_model", develop = true}
 coverage = "7.2.5"
 pytest = "7.3.1"
 pytest-env = "0.8.1"
 pytest-mock = "3.10.0"
```

### Comparing `cr_api_client-4.1.0/PKG-INFO` & `cr_api_client-4.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cr-api-client
-Version: 4.1.0
+Version: 4.3.0
 Summary: AMOSSYS Cyber Range client API
 License: MIT
 Author: AMOSSYS
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -21,14 +21,15 @@
 Requires-Dist: omegaconf (>=2.2.2,<3.0.0)
 Requires-Dist: pydantic (>=1.10.2,<1.11.0)
 Requires-Dist: pypsrp (>=0.5.0,<0.6.0)
 Requires-Dist: requests (>=2.24.0,<3.0.0)
 Requires-Dist: ruamel.yaml (>=0.16.10,<0.17.0)
 Requires-Dist: setuptools (==44.0.0)
 Requires-Dist: termcolor (>=1.1.0,<1.2.0)
+Requires-Dist: types-jinja2 (>=2.11.9,<3.0.0)
 Description-Content-Type: text/markdown
 
 # AMOSSYS Cyber Range client API
 
 ## Installation
 
 Note: it is recommanded to install the package in a virtualenv in order to avoid conflicts with version dependencies of other packages.
```

