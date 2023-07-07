# Comparing `tmp/vulp-1.2.0.tar.gz` & `tmp/vulp-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vulp-1.2.0.tar", last modified: Tue Jun  6 14:06:26 2023, max compression
+gzip compressed data, was "vulp-1.2.1.tar", last modified: Fri Jul  7 10:18:31 2023, max compression
```

## Comparing `vulp-1.2.0.tar` & `vulp-1.2.1.tar`

### file list

```diff
@@ -1,43 +1,41 @@
--rw-r--r--   0        0        0    10714 2023-06-06 14:06:26.335895 vulp-1.2.0/README.md
--rw-r--r--   0        0        0     1406 2023-06-06 14:06:26.331895 vulp-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      685 2023-06-06 14:06:26.331895 vulp-1.2.0/vulp/__init__.py
--rw-r--r--   0        0        0     3444 2023-06-06 14:06:26.323895 vulp-1.2.0/vulp/spine/AgentInterface.cpp
--rw-r--r--   0        0        0     2957 2023-06-06 14:06:26.323895 vulp-1.2.0/vulp/spine/AgentInterface.h
--rw-r--r--   0        0        0     1991 2023-06-06 14:06:26.323895 vulp-1.2.0/vulp/spine/BUILD
--rw-r--r--   0        0        0      862 2023-06-06 14:06:26.323895 vulp-1.2.0/vulp/spine/Request.h
--rw-r--r--   0        0        0     9017 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/spine/Spine.cpp
--rw-r--r--   0        0        0     6184 2023-06-06 14:06:26.323895 vulp-1.2.0/vulp/spine/Spine.h
--rw-r--r--   0        0        0     5110 2023-06-06 14:06:26.323895 vulp-1.2.0/vulp/spine/StateMachine.cpp
--rw-r--r--   0        0        0     3944 2023-06-06 14:06:26.323895 vulp-1.2.0/vulp/spine/StateMachine.h
--rw-r--r--   0        0        0      872 2023-06-06 14:06:26.323895 vulp-1.2.0/vulp/spine/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/spine/position_commands.h
--rw-r--r--   0        0        0     1011 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/spine/request.py
--rw-r--r--   0        0        0      783 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/spine/spine_error.py
--rw-r--r--   0        0        0     6305 2023-06-06 14:06:26.323895 vulp-1.2.0/vulp/spine/spine_interface.py
--rw-r--r--   0        0        0    20664 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/spine/tags
--rw-r--r--   0        0        0     1638 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/spine/tests/AgentInterfaceTest.cpp
--rw-r--r--   0        0        0      718 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/spine/tests/BUILD
--rw-r--r--   0        0        0    10158 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/spine/tests/SpineTest.cpp
--rw-r--r--   0        0        0     3799 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/spine/tests/StateMachineTest.cpp
--rw-r--r--   0        0        0     6602 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/spine/tests/spine_interface_test.py
--rw-r--r--   0        0        0     1574 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/utils/BUILD
--rw-r--r--   0        0        0     1716 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/utils/Spinlock.h
--rw-r--r--   0        0        0     2604 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/utils/SynchronousClock.cpp
--rw-r--r--   0        0        0     2987 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/utils/SynchronousClock.h
--rw-r--r--   0        0        0     1091 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/utils/datetime_now_string.h
--rw-r--r--   0        0        0     1193 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/utils/handle_interrupts.cpp
--rw-r--r--   0        0        0     1121 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/utils/handle_interrupts.h
--rw-r--r--   0        0        0     2025 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/utils/low_pass_filter.h
--rw-r--r--   0        0        0     1003 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/utils/math.h
--rw-r--r--   0        0        0     1302 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/utils/random_string.h
--rw-r--r--   0        0        0     2106 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/utils/realtime.h
--rw-r--r--   0        0        0     1416 2023-06-06 14:06:26.331895 vulp-1.2.0/vulp/utils/serialize.py
--rw-r--r--   0        0        0      351 2023-06-06 14:06:26.327895 vulp-1.2.0/vulp/utils/tests/BUILD
--rw-r--r--   0        0        0     1502 2023-06-06 14:06:26.331895 vulp-1.2.0/vulp/utils/tests/SpinlockTest.cpp
--rw-r--r--   0        0        0     1356 2023-06-06 14:06:26.331895 vulp-1.2.0/vulp/utils/tests/SynchronousClockTest.cpp
--rw-r--r--   0        0        0      930 2023-06-06 14:06:26.331895 vulp-1.2.0/vulp/utils/tests/datetime_now_string_test.cpp
--rw-r--r--   0        0        0     1234 2023-06-06 14:06:26.331895 vulp-1.2.0/vulp/utils/tests/low_pass_filter_test.cpp
--rw-r--r--   0        0        0      859 2023-06-06 14:06:26.331895 vulp-1.2.0/vulp/utils/tests/math_test.cpp
--rw-r--r--   0        0        0     1215 2023-06-06 14:06:26.331895 vulp-1.2.0/vulp/utils/tests/random_string_test.cpp
--rw-r--r--   0        0        0      920 2023-06-06 14:06:26.331895 vulp-1.2.0/vulp/utils/tests/realtime_test.cpp
--rw-r--r--   0        0        0    11972 1970-01-01 00:00:00.000000 vulp-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    10970 2023-07-07 10:18:31.435026 vulp-1.2.1/README.md
+-rw-r--r--   0        0        0     1406 2023-07-07 10:18:31.431026 vulp-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      685 2023-07-07 10:18:31.431026 vulp-1.2.1/vulp/__init__.py
+-rw-r--r--   0        0        0     3628 2023-07-07 10:18:31.419026 vulp-1.2.1/vulp/spine/AgentInterface.cpp
+-rw-r--r--   0        0        0     2957 2023-07-07 10:18:31.419026 vulp-1.2.1/vulp/spine/AgentInterface.h
+-rw-r--r--   0        0        0     1991 2023-07-07 10:18:31.419026 vulp-1.2.1/vulp/spine/BUILD
+-rw-r--r--   0        0        0      862 2023-07-07 10:18:31.419026 vulp-1.2.1/vulp/spine/Request.h
+-rw-r--r--   0        0        0     9017 2023-07-07 10:18:31.419026 vulp-1.2.1/vulp/spine/Spine.cpp
+-rw-r--r--   0        0        0     6184 2023-07-07 10:18:31.419026 vulp-1.2.1/vulp/spine/Spine.h
+-rw-r--r--   0        0        0     5110 2023-07-07 10:18:31.419026 vulp-1.2.1/vulp/spine/StateMachine.cpp
+-rw-r--r--   0        0        0     3944 2023-07-07 10:18:31.419026 vulp-1.2.1/vulp/spine/StateMachine.h
+-rw-r--r--   0        0        0      872 2023-07-07 10:18:31.419026 vulp-1.2.1/vulp/spine/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 10:18:31.419026 vulp-1.2.1/vulp/spine/position_commands.h
+-rw-r--r--   0        0        0     1011 2023-07-07 10:18:31.419026 vulp-1.2.1/vulp/spine/request.py
+-rw-r--r--   0        0        0      783 2023-07-07 10:18:31.419026 vulp-1.2.1/vulp/spine/spine_error.py
+-rw-r--r--   0        0        0     6305 2023-07-07 10:18:31.419026 vulp-1.2.1/vulp/spine/spine_interface.py
+-rw-r--r--   0        0        0     1638 2023-07-07 10:18:31.419026 vulp-1.2.1/vulp/spine/tests/AgentInterfaceTest.cpp
+-rw-r--r--   0        0        0      718 2023-07-07 10:18:31.419026 vulp-1.2.1/vulp/spine/tests/BUILD
+-rw-r--r--   0        0        0    10158 2023-07-07 10:18:31.419026 vulp-1.2.1/vulp/spine/tests/SpineTest.cpp
+-rw-r--r--   0        0        0     3799 2023-07-07 10:18:31.419026 vulp-1.2.1/vulp/spine/tests/StateMachineTest.cpp
+-rw-r--r--   0        0        0     6602 2023-07-07 10:18:31.419026 vulp-1.2.1/vulp/spine/tests/spine_interface_test.py
+-rw-r--r--   0        0        0     1420 2023-07-07 10:18:31.427026 vulp-1.2.1/vulp/utils/BUILD
+-rw-r--r--   0        0        0     1716 2023-07-07 10:18:31.427026 vulp-1.2.1/vulp/utils/Spinlock.h
+-rw-r--r--   0        0        0     2604 2023-07-07 10:18:31.427026 vulp-1.2.1/vulp/utils/SynchronousClock.cpp
+-rw-r--r--   0        0        0     2987 2023-07-07 10:18:31.427026 vulp-1.2.1/vulp/utils/SynchronousClock.h
+-rw-r--r--   0        0        0     1193 2023-07-07 10:18:31.427026 vulp-1.2.1/vulp/utils/handle_interrupts.cpp
+-rw-r--r--   0        0        0     1121 2023-07-07 10:18:31.427026 vulp-1.2.1/vulp/utils/handle_interrupts.h
+-rw-r--r--   0        0        0     2025 2023-07-07 10:18:31.427026 vulp-1.2.1/vulp/utils/low_pass_filter.h
+-rw-r--r--   0        0        0     1003 2023-07-07 10:18:31.427026 vulp-1.2.1/vulp/utils/math.h
+-rw-r--r--   0        0        0     1302 2023-07-07 10:18:31.427026 vulp-1.2.1/vulp/utils/random_string.h
+-rw-r--r--   0        0        0     2106 2023-07-07 10:18:31.427026 vulp-1.2.1/vulp/utils/realtime.h
+-rw-r--r--   0        0        0     1416 2023-07-07 10:18:31.427026 vulp-1.2.1/vulp/utils/serialize.py
+-rw-r--r--   0        0        0      351 2023-07-07 10:18:31.427026 vulp-1.2.1/vulp/utils/tests/BUILD
+-rw-r--r--   0        0        0     1502 2023-07-07 10:18:31.427026 vulp-1.2.1/vulp/utils/tests/SpinlockTest.cpp
+-rw-r--r--   0        0        0     1356 2023-07-07 10:18:31.427026 vulp-1.2.1/vulp/utils/tests/SynchronousClockTest.cpp
+-rw-r--r--   0        0        0     1234 2023-07-07 10:18:31.427026 vulp-1.2.1/vulp/utils/tests/low_pass_filter_test.cpp
+-rw-r--r--   0        0        0      859 2023-07-07 10:18:31.427026 vulp-1.2.1/vulp/utils/tests/math_test.cpp
+-rw-r--r--   0        0        0     1215 2023-07-07 10:18:31.427026 vulp-1.2.1/vulp/utils/tests/random_string_test.cpp
+-rw-r--r--   0        0        0      920 2023-07-07 10:18:31.427026 vulp-1.2.1/vulp/utils/tests/realtime_test.cpp
+-rw-r--r--   0        0        0      660 1970-01-01 00:00:00.000000 vulp-1.2.1/setup.py
+-rw-r--r--   0        0        0    12228 1970-01-01 00:00:00.000000 vulp-1.2.1/PKG-INFO
```

### Comparing `vulp-1.2.0/README.md` & `vulp-1.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -58,21 +58,22 @@
 - Soft, not hard real-time guarantee: the code is empirically reliable by a large margin, that's it
 - Weakly-typed IPC: typing is used within agents and spines, but the interface between them is only checked at runtime
 
 ### Alternatives
 
 If any of the non-features is a no-go to you, you may also want to check out these existing alternatives:
 
+* [kodlab_mjbots_sdk](https://github.com/KodlabPenn/kodlab_mjbots_sdk) - C++-only framework integrated with [LCM](https://lcm-proj.github.io/lcm/) for logging and remote I/O. Still a work in progress, only supports torque commands as of writing this note.
 * [mc\_rtc](https://github.com/jrl-umi3218/mc_rtc/) - C++ real-time control framework from which Vulp inherited, among others, the idea of running the same code on simulated and real robots. The choice of a weakly-typed dictionary-based IPC was also inspired by mc\_rtc's data store. C++ controllers are bigger cathedrals to build but they can run at higher frequencies.
 * [robot\_interfaces](https://github.com/open-dynamic-robot-initiative/robot_interfaces) - Similar IPC between non-realtime Python and real-time C++ processes. The main difference lies in the use of Python bindings and action/observation types (more overhead, more safeguards) where Vulp goes structureless (faster changes, faster blunders). Also, robot\_interfaces enforces process synchronization with a [time-series API](https://people.tuebingen.mpg.de/mpi-is-software/robotfingers/docs/robot_interfaces/doc/timeseries.html) while in Vulp this is up to the agent (most agents act greedily on the latest observation).
 * [ros2_control](https://github.com/ros-controls/ros2_control) - A C++ framework for real-time control using ROS2 (still a work in progress). Its barrier of entry is steeper than the other alternatives, making it a fit for production rather than prototyping, as it aims for compatibility with other ROS frameworks like [MoveIt](https://moveit.ros.org/). A Vulp C++ spine is equivalent to a ROS ``ControllerInterface`` implementing the dictionary-based IPC protocol.
 
-If your robot is built with some of the following open hardware components, you can also use their corresponding bindings directly:
+If your robot is built with some of the following open hardware components, you can also use their corresponding Python bindings directly:
 
-* [moteus](https://pypi.org/project/moteus/) - Python bindings for moteus brushless controllers also [run well up to 200 Hz](https://github.com/tasts-robots/vulp/blob/main/doc/loop_cycles.md#moteus-python-api).
+* [moteus](https://pypi.org/project/moteus/) - bindings for moteus brushless controllers also [run well up to 200 Hz](https://github.com/tasts-robots/vulp/blob/main/doc/loop_cycles.md#moteus-python-api).
 * [odri_control_interface](https://github.com/open-dynamic-robot-initiative/odri_control_interface) - interface to control robots built with the [ODRI](https://github.com/open-dynamic-robot-initiative) Master Board.
 
 Using control bindings directly is a simpler alternative if you don't need the action-observation loop and simulation/real-robot switch from Vulp.
 
 ## Q and A
 
 ### Performance
```

### Comparing `vulp-1.2.0/pyproject.toml` & `vulp-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vulp-1.2.0/vulp/__init__.py` & `vulp-1.2.1/vulp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Real-time motion control for Python."""
 
-__version__ = "1.2.0"
+__version__ = "1.2.1"
```

### Comparing `vulp-1.2.0/vulp/spine/AgentInterface.cpp` & `vulp-1.2.1/vulp/spine/AgentInterface.cpp`

 * *Files 11% similar despite different names*

```diff
@@ -24,19 +24,25 @@
 /*! Allocate file with some error handling.
  *
  * \param[in] file_descriptor File descriptor.
  * \param[in] bytes Number of bytes to allocate.
  */
 void allocate_file(int file_descriptor, int bytes) {
   struct ::stat file_stats;
-  ::ftruncate(file_descriptor, bytes);
+
+  if (::ftruncate(file_descriptor, bytes) < 0) {
+    throw std::runtime_error("Error truncating file, errno is " +
+                             std::to_string(errno));
+  }
+
   ::fstat(file_descriptor, &file_stats);
   if (file_stats.st_size < bytes) {
-    throw std::runtime_error("Error allocating " + std::to_string(bytes) +
-                             " bytes in shared memory");
+    throw std::runtime_error(
+        "Error allocating " + std::to_string(bytes) +
+        " bytes in shared memory. Errno is : " + std::to_string(errno));
   }
 }
 
 AgentInterface::AgentInterface(const std::string& name, size_t size)
     : name_(name), size_(size) {
   // Allocate shared memory
   // About umask: see https://stackoverflow.com/a/11909753
@@ -47,15 +53,16 @@
   if (file_descriptor < 0) {
     if (errno == EINVAL) {
       spdlog::error("Cannot open shared memory \"{}\": file name is invalid.",
                     name);
     } else if (errno == EEXIST) {
       spdlog::error(
           "Cannot open shared memory \"{}\": file already exists. Is the spine "
-          "already running? Did it not exit properly? If not, run ``bazel run "
+          "already running? Did it not exit properly? If not, run "
+          "``./tools/bazelisk run "
           "@vulp//tools/shm:clean -- {}``",
           name, name);
     } else {
       spdlog::error("Cannot open shared memory file: errno is {}", errno);
     }
     throw std::runtime_error("Error opening file");
   }
```

### Comparing `vulp-1.2.0/vulp/spine/AgentInterface.h` & `vulp-1.2.1/vulp/spine/AgentInterface.h`

 * *Files identical despite different names*

### Comparing `vulp-1.2.0/vulp/spine/BUILD` & `vulp-1.2.1/vulp/spine/BUILD`

 * *Files identical despite different names*

### Comparing `vulp-1.2.0/vulp/spine/Request.h` & `vulp-1.2.1/vulp/spine/Request.h`

 * *Files identical despite different names*

### Comparing `vulp-1.2.0/vulp/spine/Spine.cpp` & `vulp-1.2.1/vulp/spine/Spine.cpp`

 * *Files identical despite different names*

### Comparing `vulp-1.2.0/vulp/spine/Spine.h` & `vulp-1.2.1/vulp/spine/Spine.h`

 * *Files identical despite different names*

### Comparing `vulp-1.2.0/vulp/spine/StateMachine.cpp` & `vulp-1.2.1/vulp/spine/StateMachine.cpp`

 * *Files identical despite different names*

### Comparing `vulp-1.2.0/vulp/spine/StateMachine.h` & `vulp-1.2.1/vulp/spine/StateMachine.h`

 * *Files identical despite different names*

### Comparing `vulp-1.2.0/vulp/spine/__init__.py` & `vulp-1.2.1/vulp/spine/__init__.py`

 * *Files identical despite different names*

### Comparing `vulp-1.2.0/vulp/spine/request.py` & `vulp-1.2.1/vulp/spine/request.py`

 * *Files identical despite different names*

### Comparing `vulp-1.2.0/vulp/spine/spine_error.py` & `vulp-1.2.1/vulp/spine/spine_error.py`

 * *Files identical despite different names*

### Comparing `vulp-1.2.0/vulp/spine/spine_interface.py` & `vulp-1.2.1/vulp/spine/spine_interface.py`

 * *Files identical despite different names*

### Comparing `vulp-1.2.0/vulp/spine/tests/AgentInterfaceTest.cpp` & `vulp-1.2.1/vulp/spine/tests/AgentInterfaceTest.cpp`

 * *Files identical despite different names*

### Comparing `vulp-1.2.0/vulp/spine/tests/BUILD` & `vulp-1.2.1/vulp/spine/tests/BUILD`

 * *Files identical despite different names*

### Comparing `vulp-1.2.0/vulp/spine/tests/SpineTest.cpp` & `vulp-1.2.1/vulp/spine/tests/SpineTest.cpp`

 * *Files identical despite different names*

### Comparing `vulp-1.2.0/vulp/spine/tests/StateMachineTest.cpp` & `vulp-1.2.1/vulp/spine/tests/StateMachineTest.cpp`

 * *Files identical despite different names*

### Comparing `vulp-1.2.0/vulp/spine/tests/spine_interface_test.py` & `vulp-1.2.1/vulp/spine/tests/spine_interface_test.py`

 * *Files identical despite different names*

### Comparing `vulp-1.2.0/vulp/utils/BUILD` & `vulp-1.2.1/vulp/utils/BUILD`

 * *Files 6% similar despite different names*

```diff
@@ -3,20 +3,14 @@
 # Copyright 2022 Stéphane Caron
 
 load("//tools/lint:lint.bzl", "add_lint_tests")
 
 package(default_visibility = ["//visibility:public"])
 
 cc_library(
-    name = "datetime_now_string",
-    hdrs = ["datetime_now_string.h"],
-    include_prefix = "vulp/utils",
-)
-
-cc_library(
     name = "handle_interrupts",
     hdrs = ["handle_interrupts.h"],
     srcs = ["handle_interrupts.cpp"],
     include_prefix = "vulp/utils",
 )
 
 cc_library(
@@ -64,15 +58,14 @@
     ],
     include_prefix = "vulp/utils",
 )
 
 cc_library(
     name = "utils",
     deps = [
-        ":datetime_now_string",
         ":handle_interrupts",
         ":low_pass_filter",
         ":math",
         ":random_string",
         ":realtime",
         ":spinlock",
         ":synchronous_clock",
```

### Comparing `vulp-1.2.0/vulp/utils/Spinlock.h` & `vulp-1.2.1/vulp/utils/Spinlock.h`

 * *Files identical despite different names*

### Comparing `vulp-1.2.0/vulp/utils/SynchronousClock.cpp` & `vulp-1.2.1/vulp/utils/SynchronousClock.cpp`

 * *Files identical despite different names*

### Comparing `vulp-1.2.0/vulp/utils/SynchronousClock.h` & `vulp-1.2.1/vulp/utils/SynchronousClock.h`

 * *Files identical despite different names*

### Comparing `vulp-1.2.0/vulp/utils/datetime_now_string.h` & `vulp-1.2.1/vulp/utils/tests/math_test.cpp`

 * *Files 18% similar despite different names*

```diff
@@ -10,29 +10,20 @@
  * Unless required by applicable law or agreed to in writing, software
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  */
 
-#pragma once
+#include "vulp/utils/math.h"
 
-#include <ctime>
-#include <iomanip>
-#include <sstream>
-#include <string>
+#include "gtest/gtest.h"
 
-namespace vulp::utils {
+namespace vulp::utils::math {
 
-/*! Generate a date-time string for time of call.
- *
- * \return Date-time string at the time the function is called.
- */
-inline std::string datetime_now_string() {
-  auto time = std::time(nullptr);
-  auto datetime = *std::localtime(&time);
-  std::ostringstream output;
-  output << std::put_time(&datetime, "%Y%m%d-%H%M%S");
-  return output.str();
+TEST(Math, Divides) {
+  ASSERT_FALSE(divides(1000000u, 0u));
+  ASSERT_FALSE(divides(100000u, 42u));
+  ASSERT_TRUE(divides(100u, 20u));
 }
 
-}  // namespace vulp::utils
+}  // namespace vulp::utils::math
```

### Comparing `vulp-1.2.0/vulp/utils/handle_interrupts.cpp` & `vulp-1.2.1/vulp/utils/handle_interrupts.cpp`

 * *Files identical despite different names*

### Comparing `vulp-1.2.0/vulp/utils/handle_interrupts.h` & `vulp-1.2.1/vulp/utils/handle_interrupts.h`

 * *Files identical despite different names*

### Comparing `vulp-1.2.0/vulp/utils/low_pass_filter.h` & `vulp-1.2.1/vulp/utils/low_pass_filter.h`

 * *Files identical despite different names*

### Comparing `vulp-1.2.0/vulp/utils/math.h` & `vulp-1.2.1/vulp/utils/math.h`

 * *Files identical despite different names*

### Comparing `vulp-1.2.0/vulp/utils/random_string.h` & `vulp-1.2.1/vulp/utils/random_string.h`

 * *Files identical despite different names*

### Comparing `vulp-1.2.0/vulp/utils/realtime.h` & `vulp-1.2.1/vulp/utils/realtime.h`

 * *Files identical despite different names*

### Comparing `vulp-1.2.0/vulp/utils/serialize.py` & `vulp-1.2.1/vulp/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `vulp-1.2.0/vulp/utils/tests/SpinlockTest.cpp` & `vulp-1.2.1/vulp/utils/tests/SpinlockTest.cpp`

 * *Files identical despite different names*

### Comparing `vulp-1.2.0/vulp/utils/tests/SynchronousClockTest.cpp` & `vulp-1.2.1/vulp/utils/tests/SynchronousClockTest.cpp`

 * *Files identical despite different names*

### Comparing `vulp-1.2.0/vulp/utils/tests/low_pass_filter_test.cpp` & `vulp-1.2.1/vulp/utils/tests/low_pass_filter_test.cpp`

 * *Files identical despite different names*

### Comparing `vulp-1.2.0/vulp/utils/tests/math_test.cpp` & `vulp-1.2.1/vulp/utils/tests/realtime_test.cpp`

 * *Files 22% similar despite different names*

```diff
@@ -10,20 +10,21 @@
  * Unless required by applicable law or agreed to in writing, software
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  */
 
-#include "vulp/utils/math.h"
+#include "vulp/utils/realtime.h"
 
 #include "gtest/gtest.h"
 
-namespace vulp::utils::math {
+namespace vulp::utils {
 
-TEST(Math, Divides) {
-  ASSERT_FALSE(divides(1000000u, 0u));
-  ASSERT_FALSE(divides(100000u, 42u));
-  ASSERT_TRUE(divides(100u, 20u));
+TEST(Realtime, ConfigureCPU) { ASSERT_NO_THROW(configure_cpu(0)); }
+
+TEST(Realtime, ConfigureScheduler) {
+  constexpr int priority = 10;
+  ASSERT_THROW(configure_scheduler(priority), std::runtime_error);
 }
 
-}  // namespace vulp::utils::math
+}  // namespace vulp::utils
```

### Comparing `vulp-1.2.0/vulp/utils/tests/random_string_test.cpp` & `vulp-1.2.1/vulp/utils/tests/random_string_test.cpp`

 * *Files identical despite different names*

### Comparing `vulp-1.2.0/PKG-INFO` & `vulp-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulp
-Version: 1.2.0
+Version: 1.2.1
 Summary: Real-time motion control for Python.
 Keywords: motion control,real time,robotics
 Author-email: Stéphane Caron <stephane.caron@normalesup.org>
 Maintainer-email: Stéphane Caron <stephane.caron@normalesup.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
@@ -86,21 +86,22 @@
 - Soft, not hard real-time guarantee: the code is empirically reliable by a large margin, that's it
 - Weakly-typed IPC: typing is used within agents and spines, but the interface between them is only checked at runtime
 
 ### Alternatives
 
 If any of the non-features is a no-go to you, you may also want to check out these existing alternatives:
 
+* [kodlab_mjbots_sdk](https://github.com/KodlabPenn/kodlab_mjbots_sdk) - C++-only framework integrated with [LCM](https://lcm-proj.github.io/lcm/) for logging and remote I/O. Still a work in progress, only supports torque commands as of writing this note.
 * [mc\_rtc](https://github.com/jrl-umi3218/mc_rtc/) - C++ real-time control framework from which Vulp inherited, among others, the idea of running the same code on simulated and real robots. The choice of a weakly-typed dictionary-based IPC was also inspired by mc\_rtc's data store. C++ controllers are bigger cathedrals to build but they can run at higher frequencies.
 * [robot\_interfaces](https://github.com/open-dynamic-robot-initiative/robot_interfaces) - Similar IPC between non-realtime Python and real-time C++ processes. The main difference lies in the use of Python bindings and action/observation types (more overhead, more safeguards) where Vulp goes structureless (faster changes, faster blunders). Also, robot\_interfaces enforces process synchronization with a [time-series API](https://people.tuebingen.mpg.de/mpi-is-software/robotfingers/docs/robot_interfaces/doc/timeseries.html) while in Vulp this is up to the agent (most agents act greedily on the latest observation).
 * [ros2_control](https://github.com/ros-controls/ros2_control) - A C++ framework for real-time control using ROS2 (still a work in progress). Its barrier of entry is steeper than the other alternatives, making it a fit for production rather than prototyping, as it aims for compatibility with other ROS frameworks like [MoveIt](https://moveit.ros.org/). A Vulp C++ spine is equivalent to a ROS ``ControllerInterface`` implementing the dictionary-based IPC protocol.
 
-If your robot is built with some of the following open hardware components, you can also use their corresponding bindings directly:
+If your robot is built with some of the following open hardware components, you can also use their corresponding Python bindings directly:
 
-* [moteus](https://pypi.org/project/moteus/) - Python bindings for moteus brushless controllers also [run well up to 200 Hz](https://github.com/tasts-robots/vulp/blob/main/doc/loop_cycles.md#moteus-python-api).
+* [moteus](https://pypi.org/project/moteus/) - bindings for moteus brushless controllers also [run well up to 200 Hz](https://github.com/tasts-robots/vulp/blob/main/doc/loop_cycles.md#moteus-python-api).
 * [odri_control_interface](https://github.com/open-dynamic-robot-initiative/odri_control_interface) - interface to control robots built with the [ODRI](https://github.com/open-dynamic-robot-initiative) Master Board.
 
 Using control bindings directly is a simpler alternative if you don't need the action-observation loop and simulation/real-robot switch from Vulp.
 
 ## Q and A
 
 ### Performance
```

