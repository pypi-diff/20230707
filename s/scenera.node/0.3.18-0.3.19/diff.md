# Comparing `tmp/scenera.node-0.3.18.tar.gz` & `tmp/scenera.node-0.3.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scenera.node-0.3.18.tar", last modified: Fri Jun  2 18:26:48 2023, max compression
+gzip compressed data, was "scenera.node-0.3.19.tar", last modified: Fri Jul  7 20:21:14 2023, max compression
```

## Comparing `scenera.node-0.3.18.tar` & `scenera.node-0.3.19.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:26:48.419424 scenera.node-0.3.18/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-02 18:26:40.000000 scenera.node-0.3.18/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-06-02 18:26:48.415424 scenera.node-0.3.18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-02 18:26:40.000000 scenera.node-0.3.18/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:26:48.415424 scenera.node-0.3.18/scenera/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:26:48.415424 scenera.node-0.3.18/scenera/node/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-02 18:26:40.000000 scenera.node-0.3.18/scenera/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-02 18:26:40.000000 scenera.node-0.3.18/scenera/node/jwt_decode.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-02 18:26:40.000000 scenera.node-0.3.18/scenera/node/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-02 18:26:40.000000 scenera.node-0.3.18/scenera/node/nodesequencer_header_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    30254 2023-06-02 18:26:40.000000 scenera.node-0.3.18/scenera/node/scenemark.py
--rw-r--r--   0 runner    (1001) docker     (123)    38051 2023-06-02 18:26:40.000000 scenera.node-0.3.18/scenera/node/scenemark_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-02 18:26:40.000000 scenera.node-0.3.18/scenera/node/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-06-02 18:26:40.000000 scenera.node-0.3.18/scenera/node/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-02 18:26:40.000000 scenera.node-0.3.18/scenera/node/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:26:48.415424 scenera.node-0.3.18/scenera.node.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-06-02 18:26:48.000000 scenera.node-0.3.18/scenera.node.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-02 18:26:48.000000 scenera.node-0.3.18/scenera.node.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 18:26:48.000000 scenera.node-0.3.18/scenera.node.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-02 18:26:48.000000 scenera.node-0.3.18/scenera.node.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 18:26:48.000000 scenera.node-0.3.18/scenera.node.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 18:26:48.419424 scenera.node-0.3.18/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-02 18:26:40.000000 scenera.node-0.3.18/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:21:14.919943 scenera.node-0.3.19/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-07 20:21:04.000000 scenera.node-0.3.19/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-07-07 20:21:14.919943 scenera.node-0.3.19/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-07 20:21:04.000000 scenera.node-0.3.19/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:21:14.919943 scenera.node-0.3.19/scenera/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:21:14.919943 scenera.node-0.3.19/scenera/node/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-07 20:21:04.000000 scenera.node-0.3.19/scenera/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-07 20:21:04.000000 scenera.node-0.3.19/scenera/node/jwt_decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-07 20:21:04.000000 scenera.node-0.3.19/scenera/node/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-07 20:21:04.000000 scenera.node-0.3.19/scenera/node/nodesequencer_header_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32540 2023-07-07 20:21:04.000000 scenera.node-0.3.19/scenera/node/scenemark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38592 2023-07-07 20:21:04.000000 scenera.node-0.3.19/scenera/node/scenemark_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-07 20:21:04.000000 scenera.node-0.3.19/scenera/node/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-07-07 20:21:04.000000 scenera.node-0.3.19/scenera/node/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-07 20:21:04.000000 scenera.node-0.3.19/scenera/node/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:21:14.919943 scenera.node-0.3.19/scenera.node.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-07-07 20:21:14.000000 scenera.node-0.3.19/scenera.node.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-07 20:21:14.000000 scenera.node-0.3.19/scenera.node.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 20:21:14.000000 scenera.node-0.3.19/scenera.node.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-07 20:21:14.000000 scenera.node-0.3.19/scenera.node.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 20:21:14.000000 scenera.node-0.3.19/scenera.node.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 20:21:14.919943 scenera.node-0.3.19/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-07 20:21:04.000000 scenera.node-0.3.19/setup.py
```

### Comparing `scenera.node-0.3.18/LICENSE` & `scenera.node-0.3.19/LICENSE`

 * *Files identical despite different names*

### Comparing `scenera.node-0.3.18/PKG-INFO` & `scenera.node-0.3.19/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scenera.node
-Version: 0.3.18
+Version: 0.3.19
 Summary: Scenera Node SDK
 Home-page: https://docs.scenera.live/
 Author: Dirk Meulenbelt
 Author-email: dirkmeulenbelt@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `scenera.node-0.3.18/README.md` & `scenera.node-0.3.19/README.md`

 * *Files identical despite different names*

### Comparing `scenera.node-0.3.18/scenera/node/jwt_decode.py` & `scenera.node-0.3.19/scenera/node/jwt_decode.py`

 * *Files identical despite different names*

### Comparing `scenera.node-0.3.18/scenera/node/logger.py` & `scenera.node-0.3.19/scenera/node/logger.py`

 * *Files identical despite different names*

### Comparing `scenera.node-0.3.18/scenera/node/nodesequencer_header_schema.py` & `scenera.node-0.3.19/scenera/node/nodesequencer_header_schema.py`

 * *Files identical despite different names*

### Comparing `scenera.node-0.3.18/scenera/node/scenemark.py` & `scenera.node-0.3.19/scenera/node/scenemark.py`

 * *Files 10% similar despite different names*

```diff
@@ -353,14 +353,44 @@
         bounding_box_item['XCoordinate'] = x_c
         bounding_box_item['YCoordinate'] = y_c
         bounding_box_item['Height'] = height
         bounding_box_item['Width'] = width
 
         return bounding_box_item
 
+    @staticmethod    
+    def generate_directional_movement_item(id : str, uri : str = None):
+        """
+        Generate a directional movement item dictionary with specified ID and URI.
+
+        This method creates a dictionary with keys 'ID' and 'URI' and assigns the 
+        provided values to these keys. This dictionary represents a directional 
+        movement item.
+
+        :param id: The ID to assign to the 'ID' key in the resulting dictionary
+        :type id: str
+        :param uri: The URI to assign to the 'URI' key in the resulting dictionary
+        :type uri: str
+
+        :return: The resulting dictionary representing a directional movement item.
+        :rtype: dict
+
+        Example
+        -------
+
+        >>> generate_directional_movement_item('123', 'http://example.com')
+        {'ID': '123', 'URI': 'http://example.com'}
+        """
+        dm_item = {}
+        dm_item['ID'] = id
+        dm_item['URI'] = uri
+        logger.info(f"DirectionalMovement of ID: {id} & URI: {uri} created")
+        
+        return dm_item
+
     def generate_attribute_item(
         self,
         attribute : str,
         value : str,
         probability_of_attribute : float = 1.0,
         ):
         """
@@ -392,23 +422,26 @@
         attribute_item['VersionNumber'] = self.my_version_number
         attribute_item['Attribute'] = attribute
         attribute_item['Value'] = value
         attribute_item['ProbabilityOfAttribute'] = probability_of_attribute
 
         logger.info(f"Attribute item of {attribute}:{value} created")
         return attribute_item
-
+    
     @staticmethod
     def generate_detected_object_item(
         nice_item_type : str,
-        related_scenedata_id : str,
+        related_scenedata_id : str = "None",
         custom_item_type : str = "",
         item_id : str = "",
         item_type_count : int = 1,
         probability : float = 1.0,
+        frame : int = 0, 
+        timestamp : str = "",
+        directional_movement : dict = None,
         attributes : list = [],
         bounding_box : dict = None,
         ):
         # pylint: disable=dangerous-default-value
         """
         Generates a detected object item
 
@@ -416,14 +449,24 @@
 
         {\n
             "NICEItemType": "Human",\n
             "CustomItemType": "",\n
             "ItemID": "Chris",\n
             "ItemTypeCount": 1,\n
             "Probability": 0.93,\n
+            "DirectionalMovement": {\n
+                "ID": "123-track1-123",\n
+                "URI": "mystorage.com/123-track-123?acessTOKEN"\n
+            },\n
+            "Frame": 10,
+            "TimeStamp": "",
+            "DirectionalMovement": {
+                "ID": "123",
+                "URI": "https://example.com"
+            },
             "Attributes": [\n
                 {\n
                     "VersionNumber": 1.0,\n
                     "Attribute": "Mood",\n
                     "Value": "Anger",\n
                     "ProbabilityOfAttribute": 0.8\n
                 }\n
@@ -444,36 +487,46 @@
         :param custom_item_type: Allows specifying of the custom NICEItemType,
             defaults to "". Optional.
         :type custom_item_type: string
         :param item_id: Indicating an ID on the object.
             E.g. Name of the person Defaults to "". Optional.
         :type item_id: string
         :param item_type_count: Counting the amount of the stated NICEItemType,
-            optional, defaults to 1,
+            optional, defaults to 1.
         :type item_type_count: int
         :param probability: Indicating the confidence on the item. Optional, defaults to 1.0.
         :type probability: float
+        :param directional_movement: Contains the track_id & track_uri
+        :type directional_movement: dictionary
+        :param frame: Frame number where the item is detected. Defaults to 0.
+        :type frame: int
+        :param timestamp: Timestamp when the item is detected. Defaults to "".
+        :type timestamp: str
+        :param directional_movement: Contains directional movement item, defaults to None
+        :type directional_movement: dict
         :param attributes: Contains attribute items, defaults to []
         :type attributes: list
         :param bounding_box: Contains the bounding box, defaults to None
-        :type bounding_box: dictionary
+        :type bounding_box: dict
         :return: dictionary containing a DetectedObject item, see example.
         :rtype: dict
         """
-
         assert nice_item_type in NICEItemType, \
             logger.exception("This Item Type is not part of the Spec.")
 
         detected_object = {}
         detected_object['NICEItemType'] = nice_item_type
         detected_object['RelatedSceneData'] = related_scenedata_id
         detected_object['CustomItemType'] = custom_item_type
         detected_object['ItemID'] = item_id
         detected_object['ItemTypeCount'] = item_type_count
         detected_object['Probability'] = probability
+        detected_object['Frame'] = frame
+        detected_object['TimeStamp'] = timestamp
+        detected_object['DirectionalMovement'] = directional_movement
         detected_object['Attributes'] = attributes
         detected_object['BoundingBox'] = bounding_box
 
         logger.info(f"DetectedObjects item of NICEItemType '{nice_item_type}' generated")
         return detected_object
 
     def add_analysis_list_item(
@@ -767,15 +820,19 @@
         # Call NodeSequencer with an updated SceneMark
         answer = requests.post(
             self.nodesequencer_header['Ingress'],
             data=scenemark,
             headers=ns_header,
             verify=verify,
             stream=False)
-        logger.info(f"Returned SceneMark to NodeSequencer: {answer}")
+        try:
+            logger.info(f"Returned SceneMark to NodeSequencer: {answer}")
+            print(json.dumps(answer.json(), indent = 3))
+        except:
+            logger.info(f"Returned SceneMark to NodeSequencer: {answer}")
 
     # Helper Functions
     @staticmethod
     def get_current_utc_timestamp():
         """
         Helper function to create a UTC timestamp in the required format.
```

### Comparing `scenera.node-0.3.18/scenera/node/scenemark_schema.py` & `scenera.node-0.3.19/scenera/node/scenemark_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,15 +264,15 @@
             },
             "required": ["VersionNumber", "NodeID"]
           }
         }
       }
     },
     "ThumbnailList": {
-      "type": "array",
+      "type": ["array", "null"],
       "items": {
         "type": "object",
         "properties": {
           "VersionNumber": {
             "type": "number"
           },
           "SceneDataID": {
@@ -360,14 +360,31 @@
                   "type": ["string", "null"],
                   "description": "Unique ID that is associated with this instance of object. This is an optional field that may be used to track objects across different scenemarks."
                 },
                 "Probability": {
                   "type": ["number", "null"],
                   "description": "Certainty of the Attribute According to the Algorithm"
                 },
+                "Frame": {
+                  "type": ["integer", "null"],
+                },
+                "TimeStamp": {
+                  "type": ["string", "null"],
+                },
+                "DirectionalMovement": {
+                  "type": ["object", "null"],
+                  "properties": {
+                  "ID": {
+                    "type": "string"
+                    },
+                  "URI": {
+                    "type": ["string", "null"]
+                    }
+                  }
+                },
                 "Attributes": {
                   "type": ["array", "null"],
                   "description": "Different AI algorithms are capable of identifying different attribute of objects that have been identified. For example if a face is detected the attribute may be \"smiling\". These attributes depend on the AI algorithm used and are not specified.",
                   "uniqueItems": True,
                   "items": {
                     "type": "object",
                     "properties": {
```

### Comparing `scenera.node-0.3.18/scenera/node/spec.py` & `scenera.node-0.3.19/scenera/node/spec.py`

 * *Files identical despite different names*

### Comparing `scenera.node-0.3.18/scenera/node/utils.py` & `scenera.node-0.3.19/scenera/node/utils.py`

 * *Files identical despite different names*

### Comparing `scenera.node-0.3.18/scenera/node/validators.py` & `scenera.node-0.3.19/scenera/node/validators.py`

 * *Files identical despite different names*

### Comparing `scenera.node-0.3.18/scenera.node.egg-info/PKG-INFO` & `scenera.node-0.3.19/scenera.node.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scenera.node
-Version: 0.3.18
+Version: 0.3.19
 Summary: Scenera Node SDK
 Home-page: https://docs.scenera.live/
 Author: Dirk Meulenbelt
 Author-email: dirkmeulenbelt@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `scenera.node-0.3.18/setup.py` & `scenera.node-0.3.19/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="scenera.node",
-    version="0.3.18",
+    version="0.3.19",
     description="Scenera Node SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://docs.scenera.live/",
     author="Dirk Meulenbelt",
     author_email="dirkmeulenbelt@gmail.com",
     license="MIT",
```

