# Comparing `tmp/ochsner_web2com-0.1.5.tar.gz` & `tmp/ochsner_web2com-0.1.6.tar.gz`

## Comparing `ochsner_web2com-0.1.5.tar` & `ochsner_web2com-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.5/.gitattributes
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.5/ochsner_web2com/__init__.py
--rw-r--r--   0        0        0     7961 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.5/ochsner_web2com/web2com.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.5/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.5/LICENSE
--rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.5/README.md
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.6/.gitattributes
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.6/ochsner_web2com/__init__.py
+-rw-r--r--   0        0        0     7963 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.6/ochsner_web2com/web2com.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.6/LICENSE
+-rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.6/README.md
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 ochsner_web2com-0.1.6/PKG-INFO
```

### Comparing `ochsner_web2com-0.1.5/ochsner_web2com/web2com.py` & `ochsner_web2com-0.1.6/ochsner_web2com/web2com.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,26 +167,26 @@
 
     def get(self, enum_id):
         try:
             if isinstance(enum_id, list):
                 id = self.get_chain_id(enum_id)
             else:
                 id = self.get_chain_id(enum_id.value)
-            result = w2c.get_value(id)
+            result = self.get_value(id)
             return (result)
         except:
             return (0, 0.0)
     
     def set(self, enum_id, command_value):
         try:
             if isinstance(enum_id, list):
                 id = self.get_chain_id(enum_id)
             else:
                 id = self.get_chain_id(enum_id.value)
-            result = w2c.set_value(id, command_value)
+            result = self.set_value(id, command_value)
             return (result)
         except:
             return (0, 0.0)
 
 
 if __name__ == '__main__':
```

### Comparing `ochsner_web2com-0.1.5/LICENSE` & `ochsner_web2com-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ochsner_web2com-0.1.5/README.md` & `ochsner_web2com-0.1.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -18,18 +18,18 @@
     result = w2c.get_value('/1/2/1/125/9')
     print(result)
     ## set value via chain id
     result = w2c.set_value('/1/2/4/99/6', 20.0)
     print(result)
 
     ## get value via predefined enum
-    result = w2c.get(HEAT_PUMP.Thermal_energy_kWh)
+    result = w2c.get(web2com.HEAT_PUMP.Thermal_energy_kWh)
     print(result)
     ## set value via predefined enum
-    result = w2c.set(HEATING_CIRCUIT.Normal_setpoint_room_temperature_heating, 20.0)
+    result = w2c.set(web2com.HEATING_CIRCUIT.Normal_setpoint_room_temperature_heating, 20.0)
     print(result)
 
     ## get values via list of id's (eBus and device will be added)
     result = w2c.get([1, 125, 9])
     print(result)
     ## set value via list of id's (eBus and device will be added)
     result = w2c.set([4, 99, 6], 20.0)
```

### Comparing `ochsner_web2com-0.1.5/pyproject.toml` & `ochsner_web2com-0.1.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ochsner_web2com"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Alexander Hackl", email="pypi@eccoz.de" },
 ]
 description = "Access to the ochsner web2com interface"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `ochsner_web2com-0.1.5/PKG-INFO` & `ochsner_web2com-0.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ochsner_web2com
-Version: 0.1.5
+Version: 0.1.6
 Summary: Access to the ochsner web2com interface
 Project-URL: Homepage, https://github.com/ahackl/pypi_ochsner_web2com
 Project-URL: Bug Tracker, https://github.com/ahackl/pypi_ochsner_web2com/issues
 Author-email: Alexander Hackl <pypi@eccoz.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -34,18 +34,18 @@
     result = w2c.get_value('/1/2/1/125/9')
     print(result)
     ## set value via chain id
     result = w2c.set_value('/1/2/4/99/6', 20.0)
     print(result)
 
     ## get value via predefined enum
-    result = w2c.get(HEAT_PUMP.Thermal_energy_kWh)
+    result = w2c.get(web2com.HEAT_PUMP.Thermal_energy_kWh)
     print(result)
     ## set value via predefined enum
-    result = w2c.set(HEATING_CIRCUIT.Normal_setpoint_room_temperature_heating, 20.0)
+    result = w2c.set(web2com.HEATING_CIRCUIT.Normal_setpoint_room_temperature_heating, 20.0)
     print(result)
 
     ## get values via list of id's (eBus and device will be added)
     result = w2c.get([1, 125, 9])
     print(result)
     ## set value via list of id's (eBus and device will be added)
     result = w2c.set([4, 99, 6], 20.0)
```

