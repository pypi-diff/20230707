# Comparing `tmp/neuromorphic_drivers-0.2.2.tar.gz` & `tmp/neuromorphic_drivers-0.3.0.tar.gz`

## Comparing `neuromorphic_drivers-0.2.2.tar` & `neuromorphic_drivers-0.3.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
--rw-r--r--   0        0        0      474 1970-01-01 00:00:00.000000 neuromorphic_drivers-0.2.2/local_dependencies/reflect/Cargo.toml
--rw-r--r--   0     1001      123    18887 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/local_dependencies/reflect/src/de.rs
--rw-r--r--   0     1001      123     5021 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/local_dependencies/reflect/src/error.rs
--rw-r--r--   0     1001      123    25754 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/local_dependencies/reflect/src/format.rs
--rw-r--r--   0     1001      123    14340 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/local_dependencies/reflect/src/lib.rs
--rw-r--r--   0     1001      123    14435 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/local_dependencies/reflect/src/ser.rs
--rw-r--r--   0     1001      123    11374 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/local_dependencies/reflect/src/trace.rs
--rw-r--r--   0     1001      123    10825 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/local_dependencies/reflect/src/value.rs
--rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 neuromorphic_drivers-0.2.2/Cargo.toml
--rw-r--r--   0     1001      123       41 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/.gitignore
--rw-r--r--   0     1001      123     1102 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/LICENSE
--rw-r--r--   0     1001      123      115 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/README.md
--rw-r--r--   0     1001      123    35531 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/build.rs
--rw-r--r--   0     1001      123     1031 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/pyproject.toml
--rw-r--r--   0     1001      123     2765 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/__init__.py
--rw-r--r--   0     1001      123      802 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/device.py
--rw-r--r--   0     1001      123     5781 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/generated/devices/prophesee_evk3_hd.py
--rw-r--r--   0     1001      123     6143 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/generated/devices/prophesee_evk4.py
--rw-r--r--   0     1001      123     8269 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/generated/devices_types.py
--rw-r--r--   0     1001      123      400 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/generated/enums.py
--rw-r--r--   0     1001      123      701 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/generated/unions.py
--rw-r--r--   0     1001      123     4481 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/mask.py
--rw-r--r--   0     1001      123       91 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/serde/__init__.py
--rw-r--r--   0     1001      123    15358 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/serde/binary.py
--rw-r--r--   0     1001      123     2296 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/serde/bincode.py
--rw-r--r--   0     1001      123     1547 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/serde/type.py
--rw-r--r--   0     1001      123     1091 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/status.py
--rw-r--r--   0     1001      123     1858 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/udev.py
--rw-r--r--   0     1001      123     4497 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/src/adapters.rs
--rw-r--r--   0     1001      123     1675 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/src/bytes.rs
--rw-r--r--   0     1001      123    14237 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/src/lib.rs
--rw-r--r--   0     1001      123     4091 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/src/structured_array.rs
--rw-r--r--   0     1001      123     6177 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/tests/display.py
--rw-r--r--   0     1001      123     1961 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/tests/external_synchronization.py
--rw-r--r--   0     1001      123      608 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/tests/read_many.py
--rw-r--r--   0     1001      123      687 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/tests/record_raw.py
--rw-r--r--   0     1001      123      336 2023-07-03 07:27:52.000000 neuromorphic_drivers-0.2.2/tests/test.py
--rw-r--r--   0     1001      123    19206 2023-07-03 07:28:04.000000 neuromorphic_drivers-0.2.2/Cargo.lock
--rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 neuromorphic_drivers-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      474 1970-01-01 00:00:00.000000 neuromorphic_drivers-0.3.0/local_dependencies/reflect/Cargo.toml
+-rw-r--r--   0     1001      123    18887 2023-07-07 08:00:55.000000 neuromorphic_drivers-0.3.0/local_dependencies/reflect/src/de.rs
+-rw-r--r--   0     1001      123     5021 2023-07-07 08:00:55.000000 neuromorphic_drivers-0.3.0/local_dependencies/reflect/src/error.rs
+-rw-r--r--   0     1001      123    25754 2023-07-07 08:00:55.000000 neuromorphic_drivers-0.3.0/local_dependencies/reflect/src/format.rs
+-rw-r--r--   0     1001      123    14340 2023-07-07 08:00:55.000000 neuromorphic_drivers-0.3.0/local_dependencies/reflect/src/lib.rs
+-rw-r--r--   0     1001      123    14435 2023-07-07 08:00:55.000000 neuromorphic_drivers-0.3.0/local_dependencies/reflect/src/ser.rs
+-rw-r--r--   0     1001      123    11374 2023-07-07 08:00:55.000000 neuromorphic_drivers-0.3.0/local_dependencies/reflect/src/trace.rs
+-rw-r--r--   0     1001      123    10825 2023-07-07 08:00:55.000000 neuromorphic_drivers-0.3.0/local_dependencies/reflect/src/value.rs
+-rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 neuromorphic_drivers-0.3.0/Cargo.toml
+-rw-r--r--   0     1001      123       41 2023-07-07 08:00:55.000000 neuromorphic_drivers-0.3.0/.gitignore
+-rw-r--r--   0     1001      123     1102 2023-07-07 08:00:55.000000 neuromorphic_drivers-0.3.0/LICENSE
+-rw-r--r--   0     1001      123      115 2023-07-07 08:00:55.000000 neuromorphic_drivers-0.3.0/README.md
+-rw-r--r--   0     1001      123    36762 2023-07-07 08:00:55.000000 neuromorphic_drivers-0.3.0/build.rs
+-rw-r--r--   0     1001      123     1031 2023-07-07 08:00:55.000000 neuromorphic_drivers-0.3.0/pyproject.toml
+-rw-r--r--   0     1001      123     2765 2023-07-07 08:00:55.000000 neuromorphic_drivers-0.3.0/python/neuromorphic_drivers/__init__.py
+-rw-r--r--   0     1001      123     1015 2023-07-07 08:00:55.000000 neuromorphic_drivers-0.3.0/python/neuromorphic_drivers/device.py
+-rw-r--r--   0     1001      123     6097 2023-07-07 08:00:55.000000 neuromorphic_drivers-0.3.0/python/neuromorphic_drivers/generated/devices/prophesee_evk3_hd.py
+-rw-r--r--   0     1001      123     6459 2023-07-07 08:00:55.000000 neuromorphic_drivers-0.3.0/python/neuromorphic_drivers/generated/devices/prophesee_evk4.py
+-rw-r--r--   0     1001      123     8585 2023-07-07 08:00:55.000000 neuromorphic_drivers-0.3.0/python/neuromorphic_drivers/generated/devices_types.py
+-rw-r--r--   0     1001      123      400 2023-07-07 08:00:55.000000 neuromorphic_drivers-0.3.0/python/neuromorphic_drivers/generated/enums.py
+-rw-r--r--   0     1001      123      701 2023-07-07 08:00:55.000000 neuromorphic_drivers-0.3.0/python/neuromorphic_drivers/generated/unions.py
+-rw-r--r--   0     1001      123     4481 2023-07-07 08:00:55.000000 neuromorphic_drivers-0.3.0/python/neuromorphic_drivers/mask.py
+-rw-r--r--   0     1001      123       91 2023-07-07 08:00:55.000000 neuromorphic_drivers-0.3.0/python/neuromorphic_drivers/serde/__init__.py
+-rw-r--r--   0     1001      123    15358 2023-07-07 08:00:55.000000 neuromorphic_drivers-0.3.0/python/neuromorphic_drivers/serde/binary.py
+-rw-r--r--   0     1001      123     2296 2023-07-07 08:00:55.000000 neuromorphic_drivers-0.3.0/python/neuromorphic_drivers/serde/bincode.py
+-rw-r--r--   0     1001      123     1547 2023-07-07 08:00:55.000000 neuromorphic_drivers-0.3.0/python/neuromorphic_drivers/serde/type.py
+-rw-r--r--   0     1001      123     1091 2023-07-07 08:00:55.000000 neuromorphic_drivers-0.3.0/python/neuromorphic_drivers/status.py
+-rw-r--r--   0     1001      123     1858 2023-07-07 08:00:55.000000 neuromorphic_drivers-0.3.0/python/neuromorphic_drivers/udev.py
+-rw-r--r--   0     1001      123     4497 2023-07-07 08:00:55.000000 neuromorphic_drivers-0.3.0/src/adapters.rs
+-rw-r--r--   0     1001      123     1675 2023-07-07 08:00:55.000000 neuromorphic_drivers-0.3.0/src/bytes.rs
+-rw-r--r--   0     1001      123    13849 2023-07-07 08:00:55.000000 neuromorphic_drivers-0.3.0/src/lib.rs
+-rw-r--r--   0     1001      123     4091 2023-07-07 08:00:55.000000 neuromorphic_drivers-0.3.0/src/structured_array.rs
+-rw-r--r--   0     1001      123     6177 2023-07-07 08:00:55.000000 neuromorphic_drivers-0.3.0/tests/display.py
+-rw-r--r--   0     1001      123     1961 2023-07-07 08:00:55.000000 neuromorphic_drivers-0.3.0/tests/external_synchronization.py
+-rw-r--r--   0     1001      123      608 2023-07-07 08:00:55.000000 neuromorphic_drivers-0.3.0/tests/read_many.py
+-rw-r--r--   0     1001      123      687 2023-07-07 08:00:55.000000 neuromorphic_drivers-0.3.0/tests/record_raw.py
+-rw-r--r--   0     1001      123      336 2023-07-07 08:00:55.000000 neuromorphic_drivers-0.3.0/tests/test.py
+-rw-r--r--   0     1001      123      901 2023-07-07 08:00:55.000000 neuromorphic_drivers-0.3.0/tests/update_biases.py
+-rw-r--r--   0     1001      123    21258 2023-07-07 08:01:08.000000 neuromorphic_drivers-0.3.0/Cargo.lock
+-rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 neuromorphic_drivers-0.3.0/PKG-INFO
```

### Comparing `neuromorphic_drivers-0.2.2/local_dependencies/reflect/src/de.rs` & `neuromorphic_drivers-0.3.0/local_dependencies/reflect/src/de.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.2/local_dependencies/reflect/src/error.rs` & `neuromorphic_drivers-0.3.0/local_dependencies/reflect/src/error.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.2/local_dependencies/reflect/src/format.rs` & `neuromorphic_drivers-0.3.0/local_dependencies/reflect/src/format.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.2/local_dependencies/reflect/src/lib.rs` & `neuromorphic_drivers-0.3.0/local_dependencies/reflect/src/lib.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.2/local_dependencies/reflect/src/ser.rs` & `neuromorphic_drivers-0.3.0/local_dependencies/reflect/src/ser.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.2/local_dependencies/reflect/src/trace.rs` & `neuromorphic_drivers-0.3.0/local_dependencies/reflect/src/trace.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.2/local_dependencies/reflect/src/value.rs` & `neuromorphic_drivers-0.3.0/local_dependencies/reflect/src/value.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.2/LICENSE` & `neuromorphic_drivers-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.2/build.rs` & `neuromorphic_drivers-0.3.0/build.rs`

 * *Files 1% similar despite different names*

```diff
@@ -538,14 +538,17 @@
                                 "    def properties(self) -> Properties:\n",
                                 "        ...\n",
                                 "\n",
                                 "    def serial(self) -> str:\n",
                                 "        ...\n",
                                 "\n",
                                 "    def speed(self) -> enums.Speed:\n",
+                                "        ...\n",
+                                "\n",
+                                "    def update_configuration(self, configuration: Configuration):\n",
                                 "        ...",
                             ),
                             class_name,
                             class_suffix,
                             class_name,
                             class_suffix,
                             class_name,
@@ -682,14 +685,17 @@
                             "    def properties(self) -> Properties:\n",
                             "        ...\n",
                             "\n",
                             "    def serial(self) -> str:\n",
                             "        ...\n",
                             "\n",
                             "    def speed(self) -> Speed:\n",
+                            "        ...\n",
+                            "\n",
+                            "    def update_configuration(self, configuration: Configuration):\n",
                             "        ...",
                         ),
                         class_name,
                         class_suffix,
                         class_name,
                         class_suffix,
                         class_name,
@@ -814,14 +820,41 @@
             }
         }
     }
     None
 }
 
 fn main() {
+    {
+        let cargo_toml = std::fs::read_to_string("Cargo.toml")
+            .unwrap()
+            .parse::<toml::Value>()
+            .unwrap();
+        let cargo_version = cargo_toml
+            .get("package")
+            .unwrap()
+            .get("version")
+            .unwrap()
+            .as_str()
+            .unwrap();
+        let pyproject_toml = std::fs::read_to_string("pyproject.toml")
+            .unwrap()
+            .parse::<toml::Value>()
+            .unwrap();
+        let pyproject_version = pyproject_toml
+            .get("project")
+            .unwrap()
+            .get("version")
+            .unwrap()
+            .as_str()
+            .unwrap();
+        if cargo_version != pyproject_version {
+            panic!("the cargo version ({cargo_version}) and the pyproject version ({pyproject_version}) are different");
+        }
+    }
     if std::env::var("TARGET").unwrap().contains("apple") {
         if let Some(path) = macos_link_search_path() {
             println!("cargo:rustc-link-lib=clang_rt.osx");
             println!("cargo:rustc-link-search={}", path);
         }
     }
     generate!(prophesee_evk3_hd, prophesee_evk4);
```

### Comparing `neuromorphic_drivers-0.2.2/pyproject.toml` & `neuromorphic_drivers-0.3.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description = "Neuromorphic devices drivers"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [
     {name = "International Centre for Neuromorphic Systems"},
     {name = "Alexandre Marcireau"},
 ]
-version = "0.2.2"
+version = "0.3.0"
 requires-python = ">=3.8"
 dependencies = ["numpy>=1.24"]
 
 [project.urls]
 homepage = "https://github.com/neuromorphicsystems/neuromorphic-rs/"
 repository = "https://github.com/neuromorphicsystems/neuromorphic-rs/"
 documentation = "https://github.com/neuromorphicsystems/neuromorphic-rs/"
```

### Comparing `neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/__init__.py` & `neuromorphic_drivers-0.3.0/python/neuromorphic_drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/device.py` & `neuromorphic_drivers-0.3.0/python/neuromorphic_drivers/device.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,7 +24,12 @@
         return (
             status.Status(
                 system_time=system_time,
                 ring=None if ring_status is None else status.RingStatus(*ring_status),
             ),
             packet,
         )
+
+    def update_configuration(self, configuration: unions.Configuration) -> None:
+        return ExtensionDevice.update_configuration(
+            self, (configuration.type(), configuration.serialize())
+        )
```

### Comparing `neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/generated/devices/prophesee_evk3_hd.py` & `neuromorphic_drivers-0.3.0/python/neuromorphic_drivers/generated/devices/prophesee_evk3_hd.py`

 * *Files 8% similar despite different names*

```diff
@@ -134,14 +134,17 @@
 
     def serial(self) -> str:
         ...
 
     def speed(self) -> enums.Speed:
         ...
 
+    def update_configuration(self, configuration: Configuration):
+        ...
+
 
 class DeviceOptional(typing.Protocol):
     def __enter__(self) -> "DeviceOptional":
         ...
 
     def __exit__(
         self,
@@ -168,14 +171,17 @@
 
     def serial(self) -> str:
         ...
 
     def speed(self) -> enums.Speed:
         ...
 
+    def update_configuration(self, configuration: Configuration):
+        ...
+
 
 class DeviceRaw(typing.Protocol):
     def __enter__(self) -> "DeviceRaw":
         ...
 
     def __exit__(
         self,
@@ -202,14 +208,17 @@
 
     def serial(self) -> str:
         ...
 
     def speed(self) -> enums.Speed:
         ...
 
+    def update_configuration(self, configuration: Configuration):
+        ...
+
 
 class DeviceRawOptional(typing.Protocol):
     def __enter__(self) -> "DeviceRawOptional":
         ...
 
     def __exit__(
         self,
@@ -235,7 +244,10 @@
         ...
 
     def serial(self) -> str:
         ...
 
     def speed(self) -> enums.Speed:
         ...
+
+    def update_configuration(self, configuration: Configuration):
+        ...
```

### Comparing `neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/generated/devices/prophesee_evk4.py` & `neuromorphic_drivers-0.3.0/python/neuromorphic_drivers/generated/devices/prophesee_evk4.py`

 * *Files 15% similar despite different names*

```diff
@@ -148,14 +148,17 @@
 
     def serial(self) -> str:
         ...
 
     def speed(self) -> enums.Speed:
         ...
 
+    def update_configuration(self, configuration: Configuration):
+        ...
+
 
 class DeviceOptional(typing.Protocol):
     def __enter__(self) -> "DeviceOptional":
         ...
 
     def __exit__(
         self,
@@ -182,14 +185,17 @@
 
     def serial(self) -> str:
         ...
 
     def speed(self) -> enums.Speed:
         ...
 
+    def update_configuration(self, configuration: Configuration):
+        ...
+
 
 class DeviceRaw(typing.Protocol):
     def __enter__(self) -> "DeviceRaw":
         ...
 
     def __exit__(
         self,
@@ -216,14 +222,17 @@
 
     def serial(self) -> str:
         ...
 
     def speed(self) -> enums.Speed:
         ...
 
+    def update_configuration(self, configuration: Configuration):
+        ...
+
 
 class DeviceRawOptional(typing.Protocol):
     def __enter__(self) -> "DeviceRawOptional":
         ...
 
     def __exit__(
         self,
@@ -249,7 +258,10 @@
         ...
 
     def serial(self) -> str:
         ...
 
     def speed(self) -> enums.Speed:
         ...
+
+    def update_configuration(self, configuration: Configuration):
+        ...
```

### Comparing `neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/generated/devices_types.py` & `neuromorphic_drivers-0.3.0/python/neuromorphic_drivers/generated/devices_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,17 @@
 
     def serial(self) -> str:
         ...
 
     def speed(self) -> Speed:
         ...
 
+    def update_configuration(self, configuration: Configuration):
+        ...
+
 
 class GenericDeviceOptional(typing.Protocol):
     def __enter__(self) -> "GenericDeviceOptional":
         ...
 
     def __exit__(
         self,
@@ -77,14 +80,17 @@
 
     def serial(self) -> str:
         ...
 
     def speed(self) -> Speed:
         ...
 
+    def update_configuration(self, configuration: Configuration):
+        ...
+
 
 class GenericDeviceRaw(typing.Protocol):
     def __enter__(self) -> "GenericDeviceRaw":
         ...
 
     def __exit__(
         self,
@@ -111,14 +117,17 @@
 
     def serial(self) -> str:
         ...
 
     def speed(self) -> Speed:
         ...
 
+    def update_configuration(self, configuration: Configuration):
+        ...
+
 
 class GenericDeviceRawOptional(typing.Protocol):
     def __enter__(self) -> "GenericDeviceRawOptional":
         ...
 
     def __exit__(
         self,
@@ -145,14 +154,17 @@
 
     def serial(self) -> str:
         ...
 
     def speed(self) -> Speed:
         ...
 
+    def update_configuration(self, configuration: Configuration):
+        ...
+
 
 @typing.overload
 def open(
     configuration: prophesee_evk3_hd.Configuration,
     iterator_timeout: typing.Literal[None] = None,
     raw: typing.Literal[False] = False,
     serial: typing.Optional[str] = None,
```

### Comparing `neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/generated/unions.py` & `neuromorphic_drivers-0.3.0/python/neuromorphic_drivers/generated/unions.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/mask.py` & `neuromorphic_drivers-0.3.0/python/neuromorphic_drivers/mask.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/serde/binary.py` & `neuromorphic_drivers-0.3.0/python/neuromorphic_drivers/serde/binary.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/serde/bincode.py` & `neuromorphic_drivers-0.3.0/python/neuromorphic_drivers/serde/bincode.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/serde/type.py` & `neuromorphic_drivers-0.3.0/python/neuromorphic_drivers/serde/type.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/status.py` & `neuromorphic_drivers-0.3.0/python/neuromorphic_drivers/status.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.2/python/neuromorphic_drivers/udev.py` & `neuromorphic_drivers-0.3.0/python/neuromorphic_drivers/udev.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.2/src/adapters.rs` & `neuromorphic_drivers-0.3.0/src/adapters.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.2/src/bytes.rs` & `neuromorphic_drivers-0.3.0/src/bytes.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.2/src/lib.rs` & `neuromorphic_drivers-0.3.0/src/lib.rs`

 * *Files 5% similar despite different names*

```diff
@@ -25,25 +25,26 @@
             )
         })
         .collect())
 }
 
 #[pyo3::pyclass(subclass)]
 struct Device {
-    device: Option<std::cell::RefCell<neuromorphic_drivers_rs::Device>>,
+    device: Option<neuromorphic_drivers_rs::Device>,
     adapter: Option<std::cell::RefCell<adapters::Adapter>>,
     iterator_timeout: Option<std::time::Duration>,
     iterator_maximum_raw_packets: usize,
     error_flag: neuromorphic_drivers_rs::error::Flag<neuromorphic_drivers_rs::Error>,
 }
 
 // unsafe workaround until auto traits are stabilized
 // see https://docs.rs/pyo3/0.19.0/pyo3/marker/index.html
-struct DeviceReference<'a>(pub &'a mut neuromorphic_drivers_rs::Device);
+struct DeviceReference<'a>(pub &'a neuromorphic_drivers_rs::Device);
 unsafe impl Send for DeviceReference<'_> {}
+unsafe impl Sync for DeviceReference<'_> {}
 enum Buffer<'a> {
     Adapter(&'a mut adapters::Adapter),
     Bytes(bytes::Bytes),
 }
 unsafe impl Send for Buffer<'_> {}
 
 struct Status {
@@ -107,15 +108,15 @@
         .map_err(|error| pyo3::exceptions::PyRuntimeError::new_err(format!("{error}")))?;
         let adapter = if raw {
             None
         } else {
             Some(std::cell::RefCell::new(device.adapter().into()))
         };
         Ok(Self {
-            device: Some(std::cell::RefCell::new(device)),
+            device: Some(device),
             adapter,
             iterator_timeout: match iterator_timeout {
                 Some(seconds) => {
                     if seconds < 0.0 {
                         return Err(pyo3::exceptions::PyValueError::new_err(
                             "iterator_timeout must larger than or equal to 0",
                         ));
@@ -151,27 +152,17 @@
         slf: pyo3::PyRef<Self>,
         python: pyo3::Python,
     ) -> pyo3::PyResult<Option<pyo3::PyObject>> {
         let start = std::time::Instant::now();
         let error_flag = slf.error_flag.clone();
         let iterator_timeout = slf.iterator_timeout;
         let iterator_maximum_raw_packets = slf.iterator_maximum_raw_packets;
-        let mut device_reference = slf
-            .device
-            .as_ref()
-            .ok_or(pyo3::exceptions::PyRuntimeError::new_err(
-                "__next__ called after __exit__",
-            ))?
-            .try_borrow_mut()
-            .map_err(|_| {
-                pyo3::exceptions::PyRuntimeError::new_err(
-                    "__next__ called while device is used by a different thread",
-                )
-            })?;
-        let device = DeviceReference(device_reference.deref_mut());
+        let device = DeviceReference(slf.device.as_ref().ok_or(
+            pyo3::exceptions::PyRuntimeError::new_err("__next__ called after __exit__"),
+        )?);
         let mut adapter_reference = match slf.adapter.as_ref() {
             Some(adapter) => Some(adapter.try_borrow_mut().map_err(|_| {
                 pyo3::exceptions::PyRuntimeError::new_err(
                     "__next__ called while device is used by a different thread",
                 )
             })?),
             None => None,
@@ -262,27 +253,17 @@
 
     fn clear_backlog(
         slf: pyo3::PyRef<Self>,
         python: pyo3::Python,
         until: usize,
     ) -> pyo3::PyResult<()> {
         let error_flag = slf.error_flag.clone();
-        let mut device_reference = slf
-            .device
-            .as_ref()
-            .ok_or(pyo3::exceptions::PyRuntimeError::new_err(
-                "__next__ called after __exit__",
-            ))?
-            .try_borrow_mut()
-            .map_err(|_| {
-                pyo3::exceptions::PyRuntimeError::new_err(
-                    "__next__ called while device is used by a different thread",
-                )
-            })?;
-        let device = DeviceReference(device_reference.deref_mut());
+        let device = DeviceReference(slf.device.as_ref().ok_or(
+            pyo3::exceptions::PyRuntimeError::new_err("__next__ called after __exit__"),
+        )?);
         let mut adapter_reference = match slf.adapter.as_ref() {
             Some(adapter) => Some(adapter.try_borrow_mut().map_err(|_| {
                 pyo3::exceptions::PyRuntimeError::new_err(
                     "__next__ called while device is used by a different thread",
                 )
             })?),
             None => None,
@@ -316,55 +297,62 @@
     fn name(slf: pyo3::PyRef<Self>) -> pyo3::PyResult<String> {
         Ok(slf
             .device
             .as_ref()
             .ok_or(pyo3::exceptions::PyRuntimeError::new_err(
                 "name called after __exit__",
             ))?
-            .try_borrow()
-            .map_err(|_| {
-                pyo3::exceptions::PyRuntimeError::new_err(
-                    "name called while device is used by a different thread",
-                )
-            })?
             .name()
             .to_owned())
     }
 
     fn serial(slf: pyo3::PyRef<Self>) -> pyo3::PyResult<String> {
         Ok(slf
             .device
             .as_ref()
             .ok_or(pyo3::exceptions::PyRuntimeError::new_err(
                 "serial called after __exit__",
             ))?
-            .try_borrow()
-            .map_err(|_| {
-                pyo3::exceptions::PyRuntimeError::new_err(
-                    "serial called while device is used by a different thread",
-                )
-            })?
             .serial())
     }
 
     fn speed(slf: pyo3::PyRef<Self>) -> pyo3::PyResult<String> {
         Ok(slf
             .device
             .as_ref()
             .ok_or(pyo3::exceptions::PyRuntimeError::new_err(
                 "speed called after __exit__",
             ))?
-            .try_borrow()
+            .speed()
+            .to_string())
+    }
+
+    fn update_configuration(
+        slf: pyo3::PyRef<Self>,
+        type_and_configuration: (&str, &[u8]),
+    ) -> pyo3::PyResult<()> {
+        let configuration = neuromorphic_drivers_rs::Configuration::deserialize_bincode(
+            type_and_configuration
+                .0
+                .parse()
+                .map_err(|error| pyo3::exceptions::PyRuntimeError::new_err(format!("{error}")))?,
+            type_and_configuration.1,
+        )
+        .map_err(|error| pyo3::exceptions::PyRuntimeError::new_err(format!("{error}")))?;
+        slf.device
+            .as_ref()
+            .ok_or(pyo3::exceptions::PyRuntimeError::new_err(
+                "__next__ called after __exit__",
+            ))?
+            .update_configuration(configuration)
             .map_err(|_| {
                 pyo3::exceptions::PyRuntimeError::new_err(
-                    "speed called while device is used by a different thread",
+                    "update_configuration called while device is used by a different thread",
                 )
-            })?
-            .speed()
-            .to_string())
+            })
     }
 }
 
 #[pyo3::pymodule]
 fn neuromorphic_drivers(
     _py: pyo3::Python<'_>,
     module: &pyo3::types::PyModule,
```

### Comparing `neuromorphic_drivers-0.2.2/src/structured_array.rs` & `neuromorphic_drivers-0.3.0/src/structured_array.rs`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.2/tests/display.py` & `neuromorphic_drivers-0.3.0/tests/display.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.2/tests/external_synchronization.py` & `neuromorphic_drivers-0.3.0/tests/external_synchronization.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.2/tests/read_many.py` & `neuromorphic_drivers-0.3.0/tests/read_many.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.2/tests/record_raw.py` & `neuromorphic_drivers-0.3.0/tests/record_raw.py`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.2.2/Cargo.lock` & `neuromorphic_drivers-0.3.0/Cargo.lock`

 * *Files 11% similar despite different names*

```diff
@@ -38,14 +38,20 @@
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
+name = "equivalent"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88bffebc5d80432c9b140ee17875ff173a8ab62faad5b257da912bd2f6c1c0a1"
+
+[[package]]
 name = "getrandom"
 version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
 dependencies = [
  "cfg-if",
  "libc",
@@ -55,14 +61,20 @@
 [[package]]
 name = "glob"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
 
 [[package]]
+name = "hashbrown"
+version = "0.14.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2c6201b9ff9fd90a5a3bac2e56a830d0caa509576f0e503818ee82c181b3437a"
+
+[[package]]
 name = "heck"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6d621efb26863f0e9924c6ac577e8275e5e6b77455db64ffa6c65c904e9e132c"
 dependencies = [
  "unicode-segmentation",
 ]
@@ -88,24 +100,34 @@
  "proc-macro-hack",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "indexmap"
+version = "2.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d5477fe2230a79769d8dc68e0eabf5437907c0457a5614a9e8dddb67f65eb65d"
+dependencies = [
+ "equivalent",
+ "hashbrown",
+]
+
+[[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "itoa"
-version = "1.0.7"
+version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c0aa48fab2893d8a49caa94082ae8488f4e1050d73b367881dcd2198f4199fd8"
+checksum = "62b02a5381cc465bd3041d84623d0fa3b66738b52b8e2fc3bab8ad63ab032f4a"
 
 [[package]]
 name = "libc"
 version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
@@ -138,14 +160,20 @@
 checksum = "090126dc04f95dc0d1c1c91f61bdd474b3930ca064c1edc8a849da2c6cbe1e77"
 dependencies = [
  "autocfg",
  "rawpointer",
 ]
 
 [[package]]
+name = "memchr"
+version = "2.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
+
+[[package]]
 name = "memoffset"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
@@ -161,31 +189,31 @@
  "num-integer",
  "num-traits",
  "rawpointer",
 ]
 
 [[package]]
 name = "neuromorphic-drivers"
-version = "0.4.0"
+version = "0.5.0"
 dependencies = [
  "bincode",
  "libc",
  "libusb1-sys",
  "neuromorphic-types 0.4.0 (registry+https://github.com/rust-lang/crates.io-index)",
  "paste",
  "rusb",
  "serde",
  "thiserror",
 ]
 
 [[package]]
 name = "neuromorphic-drivers"
-version = "0.4.0"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eb6ec4b708513230e570689d32109906cdb90ff1fa31d68cda24968b25ed0d5e"
+checksum = "bbe22381c4040a1ffcb9910a0e1eab6c389421b9ffd2eb786d8769550b02e739"
 dependencies = [
  "bincode",
  "libc",
  "libusb1-sys",
  "neuromorphic-types 0.4.0 (registry+https://github.com/rust-lang/crates.io-index)",
  "paste",
  "rusb",
@@ -273,17 +301,17 @@
  "redox_syscall",
  "smallvec",
  "windows-targets",
 ]
 
 [[package]]
 name = "paste"
-version = "1.0.12"
+version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9f746c4065a8fa3fe23974dd82f15431cc8d40779821001404d10d2e79ca7d79"
+checksum = "b4b27ab7be369122c218afc2079489cdcb4b517c0a3fc386ff11e1fedfcc2b35"
 
 [[package]]
 name = "phf"
 version = "0.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fabbf1ead8a5bcbc20f5f8b939ee3f5b0f6f281b6ad3468b84656b658b455259"
 dependencies = [
@@ -350,86 +378,87 @@
 checksum = "7b368fba921b0dce7e60f5e04ec15e565b3303972b42bcfde1d0713b881959eb"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cffef52f74ec3b1a1baf295d9b8fcc3070327aefc39a6d00656b13c1d0b8885c"
+checksum = "ffb88ae05f306b4bfcde40ac4a51dc0b05936a9207a4b75b798c7729c4258a59"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "713eccf888fb05f1a96eb78c0dbc51907fee42b3377272dc902eb38985f418d5"
+checksum = "554db24f0b3c180a9c0b1268f91287ab3f17c162e15b54caaae5a6b3773396b0"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b2ecbdcfb01cbbf56e179ce969a048fd7305a66d4cdf3303e0da09d69afe4c3"
+checksum = "922ede8759e8600ad4da3195ae41259654b9c55da4f7eec84a0ccc7d067a70a4"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b78fdc0899f2ea781c463679b20cb08af9247febc8d052de941951024cd8aea0"
+checksum = "8a5caec6a1dd355964a841fcbeeb1b89fe4146c87295573f94228911af3cc5a2"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "60da7b84f1227c3e2fe7593505de274dcf4c8928b4e0a1c23d551a14e4e80a0f"
+checksum = "e0b78ccbb160db1556cdb6fd96c50334c5d4ec44dc5e0a968d0a1208fa0efa8b"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "python"
-version = "0.2.2"
+version = "0.3.0"
 dependencies = [
  "bincode",
  "cc",
- "neuromorphic-drivers 0.4.0 (registry+https://github.com/rust-lang/crates.io-index)",
+ "neuromorphic-drivers 0.5.0 (registry+https://github.com/rust-lang/crates.io-index)",
  "numpy",
  "paste",
  "pyo3",
  "reflect",
  "serde",
  "serde-generate",
  "serde_json",
+ "toml",
 ]
 
 [[package]]
 name = "quote"
 version = "1.0.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "573015e8ab27661678357f27dc26460738fd2b6c86e46f386fde94cb5d913105"
@@ -505,29 +534,29 @@
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
 name = "ryu"
-version = "1.0.13"
+version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
+checksum = "fe232bdf6be8c8de797b22184ee71118d63780ea42ac85b61d1baa6d3b782ae9"
 
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "serde"
-version = "1.0.164"
+version = "1.0.167"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e8c8cf938e98f769bc164923b06dce91cea1751522f46f8466461af04c9027d"
+checksum = "7daf513456463b42aa1d94cff7e0c24d682b429f020b9afa4f5ba5c40a22b237"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde-generate"
 version = "0.25.1"
@@ -551,45 +580,54 @@
  "once_cell",
  "serde",
  "thiserror",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.164"
+version = "1.0.167"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d9735b638ccc51c28bf6914d90a2e9725b377144fc612c49a611fddd1b631d68"
+checksum = "b69b106b68bc8054f0e974e70d19984040f8a5cf9215ca82626ea4853f82c4b9"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.23",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.99"
+version = "1.0.100"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46266871c240a00b8f503b877622fe33430b3c7d963bdc0f2adc511e54a1eae3"
+checksum = "0f1e14e89be7aa4c4b78bdbdc9eb5bf8517829a600ae8eaa39a6e1d960b5185c"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
+name = "serde_spanned"
+version = "0.6.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "96426c9936fd7a0124915f9185ea1d20aa9445cc9821142f0a73bc9207a2e186"
+dependencies = [
+ "serde",
+]
+
+[[package]]
 name = "siphasher"
 version = "0.3.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7bd3e3206899af3f8b12af284fafc038cc1dc2b41d1b89dd17297221c5d225de"
 
 [[package]]
 name = "smallvec"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+checksum = "62bb4feee49fdd9f707ef802e22365a35de4b7b299de4763d44bfea899442ff9"
 
 [[package]]
 name = "smawk"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f67ad224767faa3c7d8b6d91985b78e70a1324408abcb1cfcc2be4c06bc06043"
 
@@ -629,37 +667,71 @@
 dependencies = [
  "smawk",
  "unicode-width",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.40"
+version = "1.0.43"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
+checksum = "a35fc5b8971143ca348fa6df4f024d4d55264f3468c71ad1c2f365b0a4d58c42"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.40"
+version = "1.0.43"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
+checksum = "463fe12d7993d3b327787537ce8dd4dfa058de32fc2b195ef3cde03dc4771e8f"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.23",
 ]
 
 [[package]]
+name = "toml"
+version = "0.7.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c17e963a819c331dcacd7ab957d80bc2b9a9c1e71c804826d2f283dd65306542"
+dependencies = [
+ "serde",
+ "serde_spanned",
+ "toml_datetime",
+ "toml_edit",
+]
+
+[[package]]
+name = "toml_datetime"
+version = "0.6.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7cda73e2f1397b1262d6dfdcef8aafae14d1de7748d66822d3bfeeb6d03e5e4b"
+dependencies = [
+ "serde",
+]
+
+[[package]]
+name = "toml_edit"
+version = "0.19.12"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c500344a19072298cd05a7224b3c0c629348b78692bf48466c5238656e315a78"
+dependencies = [
+ "indexmap",
+ "serde",
+ "serde_spanned",
+ "toml_datetime",
+ "winnow",
+]
+
+[[package]]
 name = "unicode-ident"
-version = "1.0.9"
+version = "1.0.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
+checksum = "22049a19f4a68748a168c0fc439f9516686aa045927ff767eca0a85101fb6e73"
 
 [[package]]
 name = "unicode-segmentation"
 version = "1.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1dd624098567895118886609431a7c3b8f516e41d30e0643f03d94592a147e36"
 
@@ -739,7 +811,16 @@
 checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
+
+[[package]]
+name = "winnow"
+version = "0.4.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a9482fe6ceabdf32f3966bfdd350ba69256a97c30253dc616fe0005af24f164e"
+dependencies = [
+ "memchr",
+]
```

### Comparing `neuromorphic_drivers-0.2.2/PKG-INFO` & `neuromorphic_drivers-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuromorphic_drivers
-Version: 0.2.2
+Version: 0.3.0
 Requires-Dist: numpy >=1.24
 License-File: LICENSE
 Summary: Neuromorphic devices drivers
 Author: International Centre for Neuromorphic Systems, Alexandre Marcireau
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: homepage, https://github.com/neuromorphicsystems/neuromorphic-rs/
```

