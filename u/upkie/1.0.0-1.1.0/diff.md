# Comparing `tmp/upkie-1.0.0.tar.gz` & `tmp/upkie-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upkie-1.0.0.tar", last modified: Mon Jun 12 17:39:45 2023, max compression
+gzip compressed data, was "upkie-1.1.0.tar", last modified: Fri Jul  7 10:12:08 2023, max compression
```

## Comparing `upkie-1.0.0.tar` & `upkie-1.1.0.tar`

### file list

```diff
@@ -1,29 +1,32 @@
--rw-r--r--   0        0        0     6671 2023-06-12 17:39:45.135682 upkie-1.0.0/README.md
--rw-r--r--   0        0        0     1909 2023-06-12 17:39:45.135682 upkie-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      695 2023-06-12 17:39:45.131682 upkie-1.0.0/upkie/__init__.py
--rw-r--r--   0        0        0     1084 2023-06-12 17:39:45.123682 upkie-1.0.0/upkie/envs/BUILD
--rw-r--r--   0        0        0     1236 2023-06-12 17:39:45.123682 upkie-1.0.0/upkie/envs/__init__.py
--rw-r--r--   0        0        0     2809 2023-06-12 17:39:45.123682 upkie-1.0.0/upkie/envs/standing_reward.py
--rw-r--r--   0        0        0      549 2023-06-12 17:39:45.123682 upkie-1.0.0/upkie/envs/tests/BUILD
--rw-r--r--   0        0        0     2530 2023-06-12 17:39:45.123682 upkie-1.0.0/upkie/envs/tests/upkie_base_env_test.py
--rw-r--r--   0        0        0     2446 2023-06-12 17:39:45.123682 upkie-1.0.0/upkie/envs/tests/upkie_servos_env_test.py
--rw-r--r--   0        0        0     2330 2023-06-12 17:39:45.123682 upkie-1.0.0/upkie/envs/tests/upkie_wheels_env_test.py
--rw-r--r--   0        0        0     8063 2023-06-12 17:39:45.123682 upkie-1.0.0/upkie/envs/upkie_base_env.py
--rw-r--r--   0        0        0     7363 2023-06-12 17:39:45.123682 upkie-1.0.0/upkie/envs/upkie_servos_env.py
--rw-r--r--   0        0        0     6263 2023-06-12 17:39:45.123682 upkie-1.0.0/upkie/envs/upkie_wheels_env.py
--rw-r--r--   0        0        0      327 2023-06-12 17:39:45.127682 upkie-1.0.0/upkie/observers/base_pitch/BUILD
--rw-r--r--   0        0        0      822 2023-06-12 17:39:45.127682 upkie-1.0.0/upkie/observers/base_pitch/__init__.py
--rw-r--r--   0        0        0     4550 2023-06-12 17:39:45.127682 upkie-1.0.0/upkie/observers/base_pitch/base_pitch.py
--rw-r--r--   0        0        0      305 2023-06-12 17:39:45.127682 upkie-1.0.0/upkie/observers/base_pitch/tests/BUILD
--rw-r--r--   0        0        0     2483 2023-06-12 17:39:45.127682 upkie-1.0.0/upkie/observers/base_pitch/tests/base_pitch_test.py
--rw-r--r--   0        0        0      694 2023-06-12 17:39:45.131682 upkie-1.0.0/upkie/utils/BUILD
--rw-r--r--   0        0        0     1896 2023-06-12 17:39:45.131682 upkie-1.0.0/upkie/utils/clamp.py
--rw-r--r--   0        0        0      803 2023-06-12 17:39:45.131682 upkie-1.0.0/upkie/utils/exceptions.py
--rw-r--r--   0        0        0     2820 2023-06-12 17:39:45.131682 upkie-1.0.0/upkie/utils/filters.py
--rw-r--r--   0        0        0     2433 2023-06-12 17:39:45.131682 upkie-1.0.0/upkie/utils/pinocchio.py
--rw-r--r--   0        0        0     1231 2023-06-12 17:39:45.131682 upkie-1.0.0/upkie/utils/realtime.py
--rw-r--r--   0        0        0     1983 2023-06-12 17:39:45.131682 upkie-1.0.0/upkie/utils/spdlog.py
--rw-r--r--   0        0        0      453 2023-06-12 17:39:45.131682 upkie-1.0.0/upkie/utils/tests/BUILD
--rw-r--r--   0        0        0     1303 2023-06-12 17:39:45.131682 upkie-1.0.0/upkie/utils/tests/clamp_test.py
--rw-r--r--   0        0        0     2232 2023-06-12 17:39:45.131682 upkie-1.0.0/upkie/utils/tests/pinocchio_test.py
--rw-r--r--   0        0        0     8132 1970-01-01 00:00:00.000000 upkie-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     8466 2023-07-07 10:12:07.583809 upkie-1.1.0/README.md
+-rw-r--r--   0        0        0     1909 2023-07-07 10:12:07.579809 upkie-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      695 2023-07-07 10:12:07.579809 upkie-1.1.0/upkie/__init__.py
+-rw-r--r--   0        0        0     1084 2023-07-07 10:12:07.555810 upkie-1.1.0/upkie/envs/BUILD
+-rw-r--r--   0        0        0     1236 2023-07-07 10:12:07.555810 upkie-1.1.0/upkie/envs/__init__.py
+-rw-r--r--   0        0        0     2809 2023-07-07 10:12:07.555810 upkie-1.1.0/upkie/envs/standing_reward.py
+-rw-r--r--   0        0        0      549 2023-07-07 10:12:07.555810 upkie-1.1.0/upkie/envs/tests/BUILD
+-rw-r--r--   0        0        0     2530 2023-07-07 10:12:07.555810 upkie-1.1.0/upkie/envs/tests/upkie_base_env_test.py
+-rw-r--r--   0        0        0     2446 2023-07-07 10:12:07.555810 upkie-1.1.0/upkie/envs/tests/upkie_servos_env_test.py
+-rw-r--r--   0        0        0     2330 2023-07-07 10:12:07.555810 upkie-1.1.0/upkie/envs/tests/upkie_wheels_env_test.py
+-rw-r--r--   0        0        0     8703 2023-07-07 10:12:07.559810 upkie-1.1.0/upkie/envs/upkie_base_env.py
+-rw-r--r--   0        0        0     7363 2023-07-07 10:12:07.555810 upkie-1.1.0/upkie/envs/upkie_servos_env.py
+-rw-r--r--   0        0        0     6573 2023-07-07 10:12:07.555810 upkie-1.1.0/upkie/envs/upkie_wheels_env.py
+-rw-r--r--   0        0        0      327 2023-07-07 10:12:07.567809 upkie-1.1.0/upkie/observers/base_pitch/BUILD
+-rw-r--r--   0        0        0      822 2023-07-07 10:12:07.567809 upkie-1.1.0/upkie/observers/base_pitch/__init__.py
+-rw-r--r--   0        0        0     5477 2023-07-07 10:12:07.567809 upkie-1.1.0/upkie/observers/base_pitch/base_pitch.py
+-rw-r--r--   0        0        0      305 2023-07-07 10:12:07.567809 upkie-1.1.0/upkie/observers/base_pitch/tests/BUILD
+-rw-r--r--   0        0        0     3105 2023-07-07 10:12:07.567809 upkie-1.1.0/upkie/observers/base_pitch/tests/base_pitch_test.py
+-rw-r--r--   0        0        0     1081 2023-07-07 10:12:07.575809 upkie-1.1.0/upkie/utils/BUILD
+-rw-r--r--   0        0        0     1896 2023-07-07 10:12:07.575809 upkie-1.1.0/upkie/utils/clamp.py
+-rw-r--r--   0        0        0     1137 2023-07-07 10:12:07.575809 upkie-1.1.0/upkie/utils/datetime_now_string.h
+-rw-r--r--   0        0        0      803 2023-07-07 10:12:07.575809 upkie-1.1.0/upkie/utils/exceptions.py
+-rw-r--r--   0        0        0     2820 2023-07-07 10:12:07.575809 upkie-1.1.0/upkie/utils/filters.py
+-rw-r--r--   0        0        0     2433 2023-07-07 10:12:07.575809 upkie-1.1.0/upkie/utils/pinocchio.py
+-rw-r--r--   0        0        0     1231 2023-07-07 10:12:07.575809 upkie-1.1.0/upkie/utils/realtime.py
+-rw-r--r--   0        0        0     1983 2023-07-07 10:12:07.575809 upkie-1.1.0/upkie/utils/spdlog.py
+-rw-r--r--   0        0        0      634 2023-07-07 10:12:07.575809 upkie-1.1.0/upkie/utils/tests/BUILD
+-rw-r--r--   0        0        0     1303 2023-07-07 10:12:07.575809 upkie-1.1.0/upkie/utils/tests/clamp_test.py
+-rw-r--r--   0        0        0      986 2023-07-07 10:12:07.575809 upkie-1.1.0/upkie/utils/tests/datetime_now_string_test.cpp
+-rw-r--r--   0        0        0     2232 2023-07-07 10:12:07.575809 upkie-1.1.0/upkie/utils/tests/pinocchio_test.py
+-rw-r--r--   0        0        0      880 1970-01-01 00:00:00.000000 upkie-1.1.0/setup.py
+-rw-r--r--   0        0        0     9927 1970-01-01 00:00:00.000000 upkie-1.1.0/PKG-INFO
```

### Comparing `upkie-1.0.0/pyproject.toml` & `upkie-1.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Topic :: Scientific/Engineering",
 ]
 dependencies = [
     "gym >=0.21.0",
     "loop-rate-limiters >=0.4.0",
-    "mpacklog >=2.0.0",
+    "mpacklog >=3.0.0",
     "numpy >=1.22.0",
     "qpsolvers >=1.9.1",
     "upkie_description >=1.2.0",
     "vulp >=1.1.1",
 ]
 keywords = ["wheeled", "biped", "robot", "balance", "motion", "control", "robotics"]
```

### Comparing `upkie-1.0.0/upkie/__init__.py` & `upkie-1.1.0/upkie/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Python module to control Upkie wheeled bipeds."""
 
-__version__ = "1.0.0"
+__version__ = "1.1.0"
```

### Comparing `upkie-1.0.0/upkie/envs/BUILD` & `upkie-1.1.0/upkie/envs/BUILD`

 * *Files identical despite different names*

### Comparing `upkie-1.0.0/upkie/envs/__init__.py` & `upkie-1.1.0/upkie/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `upkie-1.0.0/upkie/envs/standing_reward.py` & `upkie-1.1.0/upkie/envs/standing_reward.py`

 * *Files identical despite different names*

### Comparing `upkie-1.0.0/upkie/envs/tests/BUILD` & `upkie-1.1.0/upkie/envs/tests/BUILD`

 * *Files identical despite different names*

### Comparing `upkie-1.0.0/upkie/envs/tests/upkie_base_env_test.py` & `upkie-1.1.0/upkie/envs/tests/upkie_base_env_test.py`

 * *Files identical despite different names*

### Comparing `upkie-1.0.0/upkie/envs/tests/upkie_servos_env_test.py` & `upkie-1.1.0/upkie/envs/tests/upkie_servos_env_test.py`

 * *Files identical despite different names*

### Comparing `upkie-1.0.0/upkie/envs/tests/upkie_wheels_env_test.py` & `upkie-1.1.0/upkie/envs/tests/upkie_wheels_env_test.py`

 * *Files identical despite different names*

### Comparing `upkie-1.0.0/upkie/envs/upkie_base_env.py` & `upkie-1.1.0/upkie/envs/upkie_base_env.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,15 +32,25 @@
         "follower_camera": False,
         "gui": True,
         "position_init_base_in_world": [0.0, 0.0, 0.6],
         "torque_control": {
             "kp": 20.0,
             "kd": 1.0,
         },
-    }
+    },
+    "floor_contact": {
+        "upper_leg_torque_threshold": 10.0,
+    },
+    "wheel_contact": {
+        "cutoff_period": 0.2,
+        "liftoff_inertia": 0.001,
+        "min_touchdown_acceleration": 2.0,
+        "min_touchdown_torque": 0.015,
+        "touchdown_inertia": 0.004,
+    },
 }
 
 
 class UpkieBaseEnv(abc.ABC, gym.Env):
 
     """!
     Base class for Upkie environments.
@@ -52,43 +62,48 @@
 
     @note This environment is made to run on a single CPU thread rather than on
     GPU/TPU. The downside for reinforcement learning is that computations are
     not massively parallel. The upside is that it simplifies deployment to the
     real robot, as it relies on the same spine interface that runs on Upkie.
     """
 
-    __frequency: float
+    __frequency: Optional[float]
     __async_rate: Optional[AsyncRateLimiter]
     __rate: Optional[RateLimiter]
     _spine: SpineInterface
     config: dict
     fall_pitch: float
 
     def __init__(
         self,
         config: Optional[dict],
         fall_pitch: float,
-        frequency: float,
+        frequency: Optional[float],
         shm_name: str,
     ) -> None:
         """!
         Initialize environment.
 
         @param config Configuration dictionary, also sent to the spine.
         @param fall_pitch Fall pitch angle, in radians.
-        @param frequency Regulated frequency of the control loop, in Hz.
+        @param frequency Regulated frequency of the control loop, in Hz. Set to
+            ``None`` to disable loop frequency regulation.
         @param shm_name Name of shared-memory file.
         """
         if config is None:
             config = DEFAULT_CONFIG
         self.__frequency = frequency
         self._spine = SpineInterface(shm_name)
         self.config = config
         self.fall_pitch = fall_pitch
 
+    @property
+    def frequency(self) -> Optional[float]:
+        return self.__frequency
+
     def close(self) -> None:
         """!
         Stop the spine properly.
         """
         self._spine.stop()
 
     def reset(
@@ -122,14 +137,16 @@
             return observation
         else:  # return_info
             return observation, observation_dict
 
     def __reset_rates(self):
         self.__async_rate = None
         self.__rate = None
+        if self.__frequency is None:  # no rate
+            return
         try:
             asyncio.get_running_loop()
             self.__async_rate = AsyncRateLimiter(self.__frequency)
         except RuntimeError:  # not asyncio
             self.__rate = RateLimiter(self.__frequency)
 
     def step(self, action: np.ndarray) -> Tuple[np.ndarray, float, bool, dict]:
@@ -145,15 +162,16 @@
             - ``done``: Whether the agent reaches the terminal state, which can
               be a good or a bad thing. If true, the user needs to call
               :func:`reset()`.
             - ``info``: Contains auxiliary diagnostic information (helpful for
               debugging, logging, and sometimes learning).
         """
         action_dict = self.dictionarize_action(action)
-        self.__rate.sleep()  # wait until clock tick to send the action
+        if self.__rate is not None:
+            self.__rate.sleep()  # wait until clock tick to send the action
         return self.__step(action_dict)
 
     async def async_step(
         self, action: np.ndarray
     ) -> Tuple[np.ndarray, float, bool, dict]:
         """!
         Run one timestep of the environment's dynamics using asynchronous I/O.
@@ -167,15 +185,16 @@
             - ``done``: Whether the agent reaches the terminal state, which can
               be a good or a bad thing. If true, the user needs to call
               :func:`reset()`.
             - ``info``: Contains auxiliary diagnostic information (helpful for
               debugging, logging, and sometimes learning).
         """
         action_dict = self.dictionarize_action(action)
-        await self.__async_rate.sleep()  # send action at next clock tick
+        if self.__async_rate is not None:
+            await self.__async_rate.sleep()  # send action at next clock tick
         return self.__step(action_dict)
 
     def __step(
         self, action_dict: dict
     ) -> Tuple[np.ndarray, float, bool, dict]:
         self._spine.set_action(action_dict)
         observation_dict = self._spine.get_observation()
@@ -188,15 +207,15 @@
         }
         return observation, reward, done, info
 
     def detect_fall(self, observation_dict: dict) -> bool:
         """!
         Detect a fall based on the body-to-world pitch angle.
 
-        @param pitch Current pitch angle in [rad].
+        @param observation_dict Observation dictionary with an "imu" key.
         @returns True if and only if a fall is detected.
         """
         imu = observation_dict["imu"]
         pitch = compute_base_pitch_from_imu(imu["orientation"])
         return abs(pitch) > self.fall_pitch
 
     @abc.abstractmethod
```

### Comparing `upkie-1.0.0/upkie/envs/upkie_servos_env.py` & `upkie-1.1.0/upkie/envs/upkie_servos_env.py`

 * *Files identical despite different names*

### Comparing `upkie-1.0.0/upkie/envs/upkie_wheels_env.py` & `upkie-1.1.0/upkie/envs/upkie_wheels_env.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,14 +66,27 @@
         <tr>
             <td>3</td>
             <td>Body angular velocity of the IMU frame along its y-axis, in
             rad/s.</td>
         </tr>
     </table>
 
+    Vectorized actions have the following structure:
+
+    <table>
+        <tr>
+            <td><strong>Index</strong></td>
+            <td><strong>Description</strong></td>
+            </tr>
+        <tr>
+            <td>``0``</td>
+            <td>Ground velocity in [m] / [s].</td>
+        </tr>
+    </table>
+
     The reward function is defined in @ref
     envs.standing_reward.StandingReward "StandingReward".
 
     See also @ref envs.upkie_base_env.UpkieBaseEnv "UpkieBaseEnv" for notes on
     using this environment.
     """
```

### Comparing `upkie-1.0.0/upkie/observers/base_pitch/__init__.py` & `upkie-1.1.0/upkie/observers/base_pitch/__init__.py`

 * *Files identical despite different names*

### Comparing `upkie-1.0.0/upkie/observers/base_pitch/base_pitch.py` & `upkie-1.1.0/upkie/observers/base_pitch/base_pitch.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import Tuple
+from typing import Optional, Tuple
 
 import numpy as np
 
 from upkie.utils.clamp import clamp
 
 
 def compute_pitch_frame_in_parent(
@@ -91,52 +91,68 @@
     """
     if abs(np.dot(quat, quat) - 1.0) > 1e-5:
         raise ValueError(f"Quaternion {quat} is not normalized")
     qw, qx, qy, qz = quat
     return np.array(
         [
             [
-                1 - 2 * (qy**2 + qz**2),
+                1 - 2 * (qy ** 2 + qz ** 2),
                 2 * (qx * qy - qz * qw),
                 2 * (qw * qy + qx * qz),
             ],
             [
                 2 * (qx * qy + qz * qw),
-                1 - 2 * (qx**2 + qz**2),
+                1 - 2 * (qx ** 2 + qz ** 2),
                 2 * (qy * qz - qx * qw),
             ],
             [
                 2 * (qx * qz - qy * qw),
                 2 * (qy * qz + qx * qw),
-                1 - 2 * (qx**2 + qy**2),
+                1 - 2 * (qx ** 2 + qy ** 2),
             ],
         ]
     )
 
 
 def compute_base_pitch_from_imu(
-    quat_imu_in_world: Tuple[float, float, float, float]
+    quat_imu_in_ars: Tuple[float, float, float, float],
+    rotation_base_to_imu: Optional[np.ndarray] = None,
 ) -> float:
     """
-    Get pitch angle of the *base* relative to the world vertical.
+    Get pitch angle of the base frame relative to the world frame.
 
     Args:
-        quat_imu_in_world: Quaternion representing the rotation matrix from
-            the *IMU* frame to the world frame, in ``[w, x, y, z]`` format.
+        quat_imu_in_ars: Quaternion representing the rotation matrix from
+            the IMU frame to the  attitude reference system (ARS) frame, in
+            ``[w, x, y, z]`` format.
+        rotation_base_to_imu: Rotation matrix from the base frame to the IMU
+            frame. When not specified, the default Upkie mounting orientation
+            is used.
 
     Returns:
-        Angle from the world z-axis (gravity) to the base z-axis.
-        Equivalently, angle that the sagittal vector of the base frame makes
-        with the heading vector.
+        Angle from the world z-axis (unit vector opposite to gravity) to the
+        base z-axis. Equivalently, angle that the sagittal vector of the base
+        frame makes with the heading vector.
 
     Note:
         The output pitch angle is for the base (x-axis pointing forward), but
         the input orientation is that of the IMU. Keep in mind that the IMU
         frame is turned 180 degrees around the yaw axis of the base frame.
+
     """
-    orientation_imu_in_world = rotation_matrix_from_quaternion(
-        quat_imu_in_world
-    )
-    pitch_imu_in_world = compute_pitch_frame_in_parent(
-        orientation_imu_in_world
+    if rotation_base_to_imu is None:
+        # Default Upkie mounting orientation: USB connectors of the raspi
+        # pointing to the left of the robot (XT-30 of the pi3hat to the right)
+        rotation_base_to_imu = np.diag([-1.0, 1.0, -1.0])
+
+    rotation_imu_to_ars = rotation_matrix_from_quaternion(quat_imu_in_ars)
+
+    # The attitude reference system frame has +x forward, +y right and +z down,
+    # whereas our world frame has +x forward, +y left and +z up:
+    # https://github.com/mjbots/pi3hat/blob/ab632c82bd501b9fcb6f8200df0551989292b7a1/docs/reference.md#orientation
+    rotation_ars_to_world = np.diag([1.0, -1.0, -1.0])
+
+    rotation_base_to_world = (
+        rotation_ars_to_world @ rotation_imu_to_ars @ rotation_base_to_imu
     )
-    return -pitch_imu_in_world  # 180 degrees yaw rotation
+    pitch_base_in_world = compute_pitch_frame_in_parent(rotation_base_to_world)
+    return pitch_base_in_world
```

### Comparing `upkie-1.0.0/upkie/observers/base_pitch/tests/base_pitch_test.py` & `upkie-1.1.0/upkie/observers/base_pitch/tests/base_pitch_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 """
 
 import unittest
 
 import numpy as np
 
 from observers.base_pitch import (
+    compute_base_pitch_from_imu,
     compute_pitch_frame_in_parent,
 )
 
 
 class TestBasePitch(unittest.TestCase):
     def test_zero_pitch(self, phi=0.42):
         """
@@ -69,10 +70,27 @@
                 [-np.sin(theta), 0.0, np.cos(theta)],
             ]
         )
         orientation_imu_in_world[:, 0] *= 1.0 - 1e-2
         imu_pitch = compute_pitch_frame_in_parent(orientation_imu_in_world)
         self.assertTrue(np.isclose(imu_pitch, theta))
 
+    def test_balancing_plane_lateral_in_imu_frame(self):
+        quat_imu_in_ars = np.array(
+            [
+                0.008472769239730098,
+                -0.9953038144146671,
+                -0.09639792825405252,
+                -0.002443076206500708,
+            ]
+        )
+        rotation_base_to_imu = np.array(
+            [[0.0, -1.0, 0.0], [1.0, 0.0, 0.0], [0.0, 0.0, 1.0]]
+        )
+        pitch_base_in_world = compute_base_pitch_from_imu(
+            quat_imu_in_ars, rotation_base_to_imu
+        )
+        self.assertAlmostEqual(pitch_base_in_world, -0.016, places=3)
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `upkie-1.0.0/upkie/utils/BUILD` & `upkie-1.1.0/upkie/utils/BUILD`

 * *Files 26% similar despite different names*

```diff
@@ -3,14 +3,27 @@
 # Copyright 2022 Stéphane Caron
 
 load("//tools/lint:lint.bzl", "add_lint_tests")
 load("@pip_upkie//:requirements.bzl", "requirement")
 
 package(default_visibility = ["//visibility:public"])
 
+cc_library(
+    name = "datetime_now_string",
+    hdrs = ["datetime_now_string.h"],
+    include_prefix = "upkie/utils",
+)
+
+cc_library(
+    name = "cpp",
+    deps = [
+        ":datetime_now_string",
+    ],
+)
+
 py_library(
     name = "clamp",
     srcs = ["clamp.py"],
     deps = [
         ":spdlog",
     ],
 )
@@ -39,8 +52,20 @@
 )
 
 py_library(
     name = "spdlog",
     srcs = ["spdlog.py"],
 )
 
+py_library(
+    name = "python",
+    deps = [
+        ":clamp",
+        ":exceptions",
+        ":filters",
+        ":pinocchio",
+        ":realtime",
+        ":spdlog",
+    ],
+)
+
 add_lint_tests()
```

### Comparing `upkie-1.0.0/upkie/utils/clamp.py` & `upkie-1.1.0/upkie/utils/clamp.py`

 * *Files identical despite different names*

### Comparing `upkie-1.0.0/upkie/utils/exceptions.py` & `upkie-1.1.0/upkie/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `upkie-1.0.0/upkie/utils/filters.py` & `upkie-1.1.0/upkie/utils/filters.py`

 * *Files identical despite different names*

### Comparing `upkie-1.0.0/upkie/utils/pinocchio.py` & `upkie-1.1.0/upkie/utils/pinocchio.py`

 * *Files identical despite different names*

### Comparing `upkie-1.0.0/upkie/utils/realtime.py` & `upkie-1.1.0/upkie/utils/realtime.py`

 * *Files identical despite different names*

### Comparing `upkie-1.0.0/upkie/utils/spdlog.py` & `upkie-1.1.0/upkie/utils/spdlog.py`

 * *Files identical despite different names*

### Comparing `upkie-1.0.0/upkie/utils/tests/clamp_test.py` & `upkie-1.1.0/upkie/utils/tests/clamp_test.py`

 * *Files identical despite different names*

### Comparing `upkie-1.0.0/upkie/utils/tests/pinocchio_test.py` & `upkie-1.1.0/upkie/utils/tests/pinocchio_test.py`

 * *Files identical despite different names*

### Comparing `upkie-1.0.0/PKG-INFO` & `upkie-1.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,67 +1,88 @@
-Metadata-Version: 2.1
-Name: upkie
-Version: 1.0.0
-Summary: Python module to control Upkie wheeled bipeds.
-Keywords: wheeled,biped,robot,balance,motion,control,robotics
-Author-email: Stéphane Caron <stephane.caron@normalesup.org>
-Maintainer-email: Stéphane Caron <stephane.caron@normalesup.org>
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Classifier: Development Status :: 4 - Beta
-Classifier: Framework :: Robot Framework :: Library
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering
-Requires-Dist: gym >=0.21.0
-Requires-Dist: loop-rate-limiters >=0.4.0
-Requires-Dist: mpacklog >=2.0.0
-Requires-Dist: numpy >=1.22.0
-Requires-Dist: qpsolvers >=1.9.1
-Requires-Dist: upkie_description >=1.2.0
-Requires-Dist: vulp >=1.1.1
-Project-URL: Changelog, https://github.com/tasts-robots/upkie/blob/main/CHANGELOG.md
-Project-URL: Documentation, https://tasts-robots.org/doc/upkie/
-Project-URL: Source, https://github.com/tasts-robots/upkie
-Project-URL: Tracker, https://github.com/tasts-robots/upkie/issues
-
 # Upkie wheeled biped
 
-[![Build](https://img.shields.io/github/actions/workflow/status/tasts-robots/upkie/bazel.yml?branch=main)](https://github.com/tasts-robots/upkie/actions/workflows/bazel.yml)
-[![Documentation](https://img.shields.io/badge/docs-online-brightgreen?logo=read-the-docs&style=flat)](https://tasts-robots.org/doc/upkie/)
+[![Build instructions](https://img.shields.io/badge/build-instructions-brightgreen?logo=read-the-docs&style=flat)](https://github.com/tasts-robots/upkie/wiki)
+[![CI](https://github.com/tasts-robots/upkie/actions/workflows/bazel.yml/badge.svg)](https://github.com/tasts-robots/upkie/actions/workflows/bazel.yml)
 [![Coverage](https://coveralls.io/repos/github/tasts-robots/upkie/badge.svg?branch=main)](https://coveralls.io/github/tasts-robots/upkie?branch=main)
 [![Vulp](https://img.shields.io/badge/%F0%9F%A6%8A%20vulp-1.2.0-orange)](https://github.com/tasts-robots/vulp)
-[![Chat](https://img.shields.io/badge/matrix-joint%20chat-%234eb899)](https://app.element.io/#/room/#tasts-robots:matrix.org)
+[![Chat](https://img.shields.io/matrix/tasts-robots:matrix.org?color=4EB899)](https://app.element.io/#/room/#tasts-robots:matrix.org)
 
-Main repository to build and control **Upkie** wheeled bipeds. Made for Linux 🐧
+Build and control **Upkie** wheeled bipeds. Made for Linux 🐧
 
-Questions about using the code, contributing, or balancing robots in general are welcome in the [Discussions](https://github.com/tasts-robots/upkie/discussions) forum or on the [Chat](https://github.com/tasts-robots/upkie/discussions).
+Questions about building and using an Upkie, or balancing robots in general, are all welcome in the [Discussions](https://github.com/tasts-robots/upkie/discussions) forum or on the [Chat](https://app.element.io/#/room/#tasts-robots:matrix.org).
 
-## Quick test
+## Quick sim
 
-Run a simulated Upkie right away from the command line, no installation required:
+If you have Python and a C++ compiler (Ubuntu: ``sudo apt install curl g++ python3-dev``), you can run an Upkie simulation right from the command line. It won't install anything on your machine, everything will run locally from the repository:
 
 <img src="https://user-images.githubusercontent.com/1189580/170496331-e1293dd3-b50c-40ee-9c2e-f75f3096ebd8.png" height="100" align="right" />
 
 ```console
-$ git clone https://github.com/tasts-robots/upkie.git
-$ cd upkie
-$ ./start_test_balancer.sh
+git clone https://github.com/tasts-robots/upkie.git
+cd upkie
+./start_wheel_balancer.sh
 ```
 
 Connect a USB controller to move the robot around 🎮
 
-## Example
+## Running a spine
+
+The code of Upkie is organized into *spines*, which communicate with the simulation or mjbots actuators, and *agents*, the programs that implement robot behaviors. Check out [this introduction](https://github.com/tasts-robots/vulp#readme) for more details.
+
+### Simulation spine
+
+In the example above we ran an agent called "wheel balancer". We could also start the simulation spine independently, and let it run waiting for agents to connect:
+
+```console
+./start_simulation.sh
+```
+
+### Robot spine
+
+To run a spine on the robot, we first build it locally and upload it to the onboard Raspberry Pi:
+
+```console
+make build
+make upload ROBOT=your_upkie
+```
+
+Next, log into the Pi and run a pi3hat spine:
+
+```console
+$ ssh user@your_upkie
+user@your_upkie:~$ cd upkie
+user@your_upkie:upkie$ make run_pi3hat_spine
+```
+
+Once the spine is running, you can run any agent in a separate shell on the robot, for example the wheel balancer:
+
+```console
+user@robot:upkie$ make run_wheel_balancer
+```
+
+## Running an agent
+
+There are two ways we can develop and run agents: using the [PyPI](#pypi) distribution, or [Bazel](#bazel). PyPI is better to get started and prototype everything in Python, while Bazel is better to recompile things from source.
+
+### PyPI
+
+[![PyPI version](https://img.shields.io/pypi/v/upkie)](https://pypi.org/project/upkie/)
+[![PyPI downloads](https://pepy.tech/badge/upkie/month)](https://pepy.tech/project/upkie)
+
+The PyPI distribution is the recommended way to control Upkie in Python. It is already [fast enough](https://github.com/tasts-robots/vulp#performance) for real-time control.
+
+#### Installation
+
+```console
+pip install upkie
+```
+
+#### Example
+
+While [running a spine](#running-a-spine), you can execute the following code in a Python interpreter or as a standalone Python script:
 
 ```python
 import gym
 import upkie.envs
 
 upkie.envs.register()
 
@@ -72,42 +93,37 @@
         observation, reward, done, _ = env.step(action)
         if done:
             observation = env.reset()
         pitch = observation[0]
         action[0] = 10.0 * pitch
 ```
 
-## Installation
+With a simulation spine, this code will reset the robot's state and execute the policy continuously. In a pi3hat spine, this code will control the robot directly.
 
-### PyPI
+Check out the ``examples/`` directory for other examples.
 
-[![PyPI version](https://img.shields.io/pypi/v/upkie)](https://pypi.org/project/upkie/)
-[![PyPI downloads](https://pepy.tech/badge/upkie/month)](https://pepy.tech/project/upkie)
-
-```console
-$ pip install upkie
-```
-
-## Code overview
+### Bazel
 
-This repository uses [Bazel](https://bazel.build/) for building and testing. One benefit of this choice is that there is no dependency to install: Bazel builds everything locally in a local cache. Compilation will only take a while the first time.
+We use [Bazel](https://bazel.build/) to build C++ spines that can run on both your host computer and the Raspberry Pi. Everything you see in the ``agents/`` and ``spines/`` directories is built with Bazel, including for instance the wheel balancer and the PPO balancer. Bazel builds everything locally, does not install anything on your system, and makes sure that all versions of all dependencies are correct. It is therefore better for sharing code with other Upkie's (no need to worry about what each user did or did not ``pip install`).
 
-Locomotion code is organized into *spines*, which communicate with the simulator or actuators using [Vulp](https://github.com/tasts-robots/vulp), and *agents*, the main programs that implement behaviors in Python. In the example above we ran the test balancer. We could also start the Bullet spine independently, and let it run waiting for agents to connect:
+Use the following syntax to run an agent with Bazel:
 
 ```console
-$ ./tools/bazelisk run -c opt //spines:bullet -- --show
+./tools/bazelisk run -c opt //agents/wheel_balancer:agent
 ```
 
-The ``-c opt`` argument to Bazel makes sure we compile optimized code, while the ``--show`` argument to the spine displays the Bullet visualization.
+Here we added the ``-c opt`` to include optimization flags during compilation.
+
+## Code overview
 
 ### Agents
 
 <dl>
-  <dt>Test balancer</dt>
-  <dd>A baseline agent designed to check out Upkie's physical capabilities. It balances the robot using PD feedback from the head's pitch and wheel odometry to wheel velocities, plus a feedforward <a href="https://github.com/tasts-robots/upkie/blob/662d76180e03a855e8810d60eeb5b229c95b68fb/agents/test_balancer/wheel_balancer.py#L378-L400">non-minimum phase trick</a> for smoother transitions from standing to rolling.</dd>
+  <dt>Wheel balancer</dt>
+  <dd>A baseline agent designed to check out Upkie's physical capabilities. The robot balances with its wheels only, following PD feedback from the head pitch and wheel odometry to wheel velocities, plus a feedforward <a href="https://github.com/tasts-robots/upkie/blob/662d76180e03a855e8810d60eeb5b229c95b68fb/agents/wheel_balancer/wheel_balancer.py#L378-L400">non-minimum phase trick</a> for smoother transitions from standing to rolling.</dd>
 
   <dt>Pink balancer</dt>
   <dd>A more capable agent that combines wheeled balancing with inverse kinematics computed by <a href="https://github.com/tasts-robots/pink">Pink</a>. This is the controller that runs in the <a href="https://www.youtube.com/shorts/8b36XcCgh7s">first</a> <a href="https://www.youtube.com/watch?v=NO_TkHGS0wQ">two</a> videos of Upkie.</dd>
 
   <dt>PPO balancer</dt>
   <dd>An agent trained by reinforcement learning to balance with straight legs. Training uses the <code><a href="https://tasts-robots.org/doc/upkie/classenvs_1_1upkie__wheels__env_1_1UpkieWheelsEnv.html#details">UpkieWheelsEnv</a></code> gym environment and the PPO implementation from <a href="https://github.com/DLR-RM/stable-baselines3/">Stable Baselines3</a>.</dd>
 </dl>
@@ -125,15 +141,15 @@
 
 ### Observers
 
 <img src="https://tasts-robots.org/doc/upkie/observers.png" align="right">
 
 <dl>
   <dt><a href="https://tasts-robots.org/doc/upkie/classupkie__locomotion_1_1observers_1_1FloorContact.html#details">Floor contact</a></dt>
-  <dd>Detect contact between the wheels and the floor. The Pink and test balancers use contact as a reset flag for their integrators, to avoid over-spinning the wheels while the robot is in the air.</dd>
+  <dd>Detect contact between the wheels and the floor. The pink and wheel balancers use contact as a reset flag for their integrators, to avoid over-spinning the wheels while the robot is in the air.</dd>
 
   <dt><a href="https://tasts-robots.org/doc/upkie/classupkie__locomotion_1_1observers_1_1WheelContact.html#details">Wheel contact</a></dt>
   <dd>Detect contact between a given wheel and the floor.</dd>
 
   <dt><a href="https://tasts-robots.org/doc/upkie/classupkie__locomotion_1_1observers_1_1WheelOdometry.html#details">Wheel odometry</a></dt>
   <dd>Measure the relative motion of the floating base with respect to the floor. Wheel odometry is part of their secondary task (after keeping the head straight), which is to stay around the same spot on the floor.</dd>
 </dl>
@@ -142,12 +158,7 @@
 
 <dl>
   <dt>Bullet</dt>
   <dd>Spawn Upkie in a <a href="http://bulletphysics.org/">Bullet</a> simulation. Resetting this spine moves the robot back to its initial configuration in this world.</dd>
   <dt>pi3hat</dt>
   <dd>Spine is made to be called from a Raspberry Pi with an onboard mjbots <a href="https://mjbots.com/products/mjbots-pi3hat-r4-4b">pi3hat</a>. Servos are stopped when the spine is stopped, and switch to <a href="https://github.com/mjbots/moteus/blob/main/docs/reference.md#theory-of-operation">position mode</a> (which is a position-velocity-torque controller) when the spine idles. Check out the <a href="https://tasts-robots.org/doc/vulp/classvulp_1_1spine_1_1StateMachine.html#details">spine state machine</a> for details.</dd>
 </dl>
-
-## See also
-
-- [Project page on Hackaday](https://hackaday.io/project/185729-upkie-wheeled-biped-robot)
-
```

