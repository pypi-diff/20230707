# Comparing `tmp/posetree-1.0.0.tar.gz` & `tmp/posetree-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "posetree-1.0.0.tar", last modified: Wed Jun 21 20:45:02 2023, max compression
+gzip compressed data, was "posetree-1.1.0.tar", last modified: Fri Jun 30 12:57:43 2023, max compression
```

## Comparing `posetree-1.0.0.tar` & `posetree-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 holson    (1000) holson    (1000)        0 2023-06-21 20:45:02.473088 posetree-1.0.0/
--rw-r--r--   0 holson    (1000) holson    (1000)     1067 2023-06-21 14:01:50.000000 posetree-1.0.0/LICENSE
--rw-r--r--   0 holson    (1000) holson    (1000)     9848 2023-06-21 20:45:02.473088 posetree-1.0.0/PKG-INFO
--rw-r--r--   0 holson    (1000) holson    (1000)     9057 2023-06-21 19:15:21.000000 posetree-1.0.0/README.md
-drwxr-xr-x   0 holson    (1000) holson    (1000)        0 2023-06-21 20:45:02.473088 posetree-1.0.0/posetree/
--rw-r--r--   0 holson    (1000) holson    (1000)       64 2023-06-21 14:01:50.000000 posetree-1.0.0/posetree/__init__.py
--rw-r--r--   0 holson    (1000) holson    (1000)    38754 2023-06-21 18:04:31.000000 posetree-1.0.0/posetree/pose.py
-drwxr-xr-x   0 holson    (1000) holson    (1000)        0 2023-06-21 20:45:02.473088 posetree-1.0.0/posetree.egg-info/
--rw-r--r--   0 holson    (1000) holson    (1000)     9848 2023-06-21 20:45:02.000000 posetree-1.0.0/posetree.egg-info/PKG-INFO
--rw-r--r--   0 holson    (1000) holson    (1000)      229 2023-06-21 20:45:02.000000 posetree-1.0.0/posetree.egg-info/SOURCES.txt
--rw-r--r--   0 holson    (1000) holson    (1000)        1 2023-06-21 20:45:02.000000 posetree-1.0.0/posetree.egg-info/dependency_links.txt
--rw-r--r--   0 holson    (1000) holson    (1000)       27 2023-06-21 20:45:02.000000 posetree-1.0.0/posetree.egg-info/requires.txt
--rw-r--r--   0 holson    (1000) holson    (1000)        9 2023-06-21 20:45:02.000000 posetree-1.0.0/posetree.egg-info/top_level.txt
--rw-r--r--   0 holson    (1000) holson    (1000)      850 2023-06-21 20:44:51.000000 posetree-1.0.0/pyproject.toml
--rw-r--r--   0 holson    (1000) holson    (1000)       38 2023-06-21 20:45:02.473088 posetree-1.0.0/setup.cfg
+drwxr-xr-x   0 holson    (1000) holson    (1000)        0 2023-06-30 12:57:43.898714 posetree-1.1.0/
+-rw-r--r--   0 holson    (1000) holson    (1000)     1067 2023-06-21 14:01:50.000000 posetree-1.1.0/LICENSE
+-rw-r--r--   0 holson    (1000) holson    (1000)    11068 2023-06-30 12:57:43.898714 posetree-1.1.0/PKG-INFO
+-rw-r--r--   0 holson    (1000) holson    (1000)    10277 2023-06-29 17:52:38.000000 posetree-1.1.0/README.md
+drwxr-xr-x   0 holson    (1000) holson    (1000)        0 2023-06-30 12:57:43.898714 posetree-1.1.0/posetree/
+-rw-r--r--   0 holson    (1000) holson    (1000)       64 2023-06-21 14:01:50.000000 posetree-1.1.0/posetree/__init__.py
+-rw-r--r--   0 holson    (1000) holson    (1000)    35587 2023-06-30 12:41:10.000000 posetree-1.1.0/posetree/pose.py
+drwxr-xr-x   0 holson    (1000) holson    (1000)        0 2023-06-30 12:57:43.898714 posetree-1.1.0/posetree.egg-info/
+-rw-r--r--   0 holson    (1000) holson    (1000)    11068 2023-06-30 12:57:43.000000 posetree-1.1.0/posetree.egg-info/PKG-INFO
+-rw-r--r--   0 holson    (1000) holson    (1000)      229 2023-06-30 12:57:43.000000 posetree-1.1.0/posetree.egg-info/SOURCES.txt
+-rw-r--r--   0 holson    (1000) holson    (1000)        1 2023-06-30 12:57:43.000000 posetree-1.1.0/posetree.egg-info/dependency_links.txt
+-rw-r--r--   0 holson    (1000) holson    (1000)       27 2023-06-30 12:57:43.000000 posetree-1.1.0/posetree.egg-info/requires.txt
+-rw-r--r--   0 holson    (1000) holson    (1000)        9 2023-06-30 12:57:43.000000 posetree-1.1.0/posetree.egg-info/top_level.txt
+-rw-r--r--   0 holson    (1000) holson    (1000)      851 2023-06-30 12:56:23.000000 posetree-1.1.0/pyproject.toml
+-rw-r--r--   0 holson    (1000) holson    (1000)       38 2023-06-30 12:57:43.898714 posetree-1.1.0/setup.cfg
```

### Comparing `posetree-1.0.0/LICENSE` & `posetree-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `posetree-1.0.0/PKG-INFO` & `posetree-1.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,46 @@
-Metadata-Version: 2.1
-Name: posetree
-Version: 1.0.0
-Summary: A Python library doing pose math for robotics.
-Author-email: Benjie Holson <bmholson@gmail.com>
-Project-URL: homepage, https://github.com/robobenjie/posetree
-Project-URL: documentation, https://htmlpreview.github.io/?https://raw.githubusercontent.com/robobenjie/posetree/main/docs/posetree/pose.html
-Project-URL: repository, https://github.com/robobenjie/posetree
-Project-URL: changelog, https://github.com/robobenjie/posetree/releases
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Scientific/Engineering
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # posetree
 
-`posetree` is an object-oriented, thread-safe, programmer-first, Python library for dealing with transforms, poses and frames, designed especially for robotics.
+`posetree` is an object-oriented, thread-safe, programmer-first, Python library for dealing with transforms, poses and frames, designed especially for robotics. It is unique in that Poses know their parent frame and it's relationship to other frames which allows for powerful operations with simple code.
 
 ## Installation
 
 ```
 pip install posetree
 ```
 
 ## Features
 
-* All poses are aware of all the frames which allows for powerful operations with simple code.
 * Write pose math designed for humans to read.
 * Think about quaternions as little as possible.
 * Never wonder if you are supposed to pre-multiply or post-multiply, or if you forgot an inverse somewhere.
-* Standalone and easy to integrate into any robotics stack.
+* Standalone, and easy to integrate into any robotics stack (works with ROS but does not depend on it).
 
 ## Basic Usage
 
 ```python
 from scipy.spatial.transform import Rotation
 from posetree import Pose
 
-looking_at = Pose.from_position_and_rotation([0, 0, 1], Rotation.identity(), "camera", pose_tree)
-
-height = looking_at.in_frame("robot").z
+# Create a pose from perception information
+pose_of_tea_bottle = Pose.from_position_and_rotation(
+    [-0.3, 0.4, 1.2], # Position of the bottle
+    Rotation.identity(), # Rotation of the bottle
+    parent_frame="camera", # Parent frame for position and rotation.
+    pose_tree=pose_tree) # PoseTree object to track frame relationships over time.
+
+# Calculate things based on other frames
+height_of_tea = pose_of_tea_bottle.in_frame("world").z
+distance_from_gripper = pose_of_tea_bottle.distance_to(gripper_pose)
 
+# Calculate some base motion targets relative to the current robot pose
 base_target = base_pose.translate([2, 0, 0]).rotate_about_z(np.pi/4)
-
 base_target2 = base_pose.point_x_at(human_pose).translate([1, 0, 0])
 
+# Get numbers out of a pose to send to a motion API
 x, y, _ = base_target.in_frame("map").position
 theta = base_target.angle_about_z_to(map_origin)
 navigate_to(x, y, theta)
 ```
 
 ## Philosophy of Transforms, Poses and Frames
 
@@ -66,23 +56,22 @@
 
 Notice we can take our example pose (standing at my front door facing the street) and transform it into another pose by using our transform instructions (take 10 steps forward and then turn 90 degrees to your left). If we do that we have a new pose that is a bit in front of my house and (in my case) facing our detached garage.
 
 - **Frame**: This is a pose that is so important we’ve decided to give it a name. 
     - Example: We could name “Standing at my front door facing the street” “journey_start” and then we could describe that other pose by saying, “from journey_start take 10 steps forward and turn 90 degrees to your left”
     - Example: We could name the left camera pose `"camera"`.
 
-You can sequence Transforms by multiplying them together, (as is traditional). This has a semantic meaning: "do this operation and then this other operation." However you cannot sequentially apply positions in 3D space so there is no multiply operator for Pose.
+You can sequence Transforms (by multiplying them together, as is traditional). This has a semantic meaning: i.e. "take 10 steps foreard and turn left THEN take 1 step backwards and turn around" which is equivalent to "take 10 steps forward and sidestep once right and then turn right". However you cannot sequentially apply positions in 3D space so there is intentionally no multiply operator for Pose. If this seems strange, I promise that as you use this library you will find that nearly every operation is easier and more clearly expressed via `in_frame`, `translate` or `rotate` operations instead of chains of `(world_t_robot * robot_t_camera * camera_t_object).inverse()` that you might be used to.
 
 ## Anchoring Poses in Frames.
 
 When constucting poses it is useful to think of what you expect the pose to be fixed relative to. For example, you might
-detect an apple on a table and get a pose from your perception system in the `camera` frame, but the apple is fixed relative to the table, so you will
-want to store your pose object with a the parent frame equal to `odometry/map/world`. Then, even if the robot moves, `apple_pose` will still refer to the
-best estimation of the apple's true location (with the usual caviats about localization drift and noise).
+detect an apple on a table and get a pose from your perception system in the `camera` frame, but the apple is actually sitting on the table, and we don't expect the apple to move if the camera moves. So you will want to store your pose object with a the parent frame equal to `odometry/map/world`. Then, even if the robot drives around, `apple_pose` will still refer to the best estimation of the apple's true location (with the usual caviats about localization drift and noise).
 
+Here's how to express that in `posetree`.
 ```python
 apple_pose = Pose(camera_t_apple, "camera", pose_tree).in_frame("world")
 ```
 
 Likewise if you have a bin on the back of a mobile robot and you want to define a drop-objects-into-bin pose right above it you can store
 that in the `robot` frame.
 
@@ -91,49 +80,47 @@
 ```
 
 When designing motion APIs with this library, you should be liberal in what frames you accept, and internally convert them to the frame you want to work in. 
 
 For example, in a function to move the arm to a pose:
 ```python
 def move_to_pose(self, target_pose: Pose):
-    # Convert the target to be relative to the base of the robot so we can execute the motion.
-    target_pose = target_pose.in_frame("robot")
-
     # Best Practice: turn Poses into Transforms at the last moment before acting on them.
-    arm_motion_primitives.move_arm_to_pose_relative_to_base(target_pose.transform)
+    arm_motion_primitives.move_arm_to_pose_relative_to_base(target_pose.in_frame("robot").transform)
 ```
 
 This formulation lets you combine the perception outputs and the motion methods for things like this:
 
 ```python
 def grasp_apple(self, apple_pose: Pose):
     # pregrasp is a pose 15 cm above the apple, with z pointing at it.
     pregrasp = apple_pose.translate([0, 0, 0.15], frame="world").point_z_at(apple_pose)
     self.move_to_pose(pregrasp)
 
     # Move down in the local 'z' of pregrasp until we touch the apple.
     self.move_to_pose_until_contact(pregrasp.translate([0, 0, 0.2]))
 
     # If we feel a contact too early, raise some reasonable error:
-    # We can check the distance using distance_to, even though the frames are different.
+    # We can check the distance using distance_to, even though the parent frames 
+    # of the two poses are different.
     if apple_pose.distance_to(get_tool_pose()) > 0.1:
         return "Whoops, we probably didn't get the apple."
 
     # Close the gripper and move up a bit from where ever we are, to lift the apple.
     self.close_gripper()
     self.move_to_pose(get_tool_pose().translate([0, 0, -0.1]))
 
     # Drop it in the bin.
     self.move_to_pose(drop_pose)
     self.open_gripper()
 ```
 
 ## Poses are Immutable
 
-Poses are immutable, and methods like `translate` return a new pose object. Immutability is nice because it makes them safe to pass into methods and also thread safe, but there is a gotcha to watch out for:
+Poses are immutable, and methods like `translate` return a new pose object. Immutability is nice because it makes them safe to pass into methods and also makes them thread safe, but there is a gotcha to watch out for:
 
 ```python
 # BAD!!! Do Not Do!
 p1.translate([1,0,0])
 p1.rotate_about_z(np.rad2deg(90))
 p1.with_position_x(5)
 # Surprise! p1 has not changed!
@@ -147,47 +134,50 @@
 # My favorite
 p2 = p1.translate([1,0,0]).rotate_about_z(np.rad2deg(90)).with_position_x(5)
 ```
 
 ## Immutability and Moving Frames
 
 While a Pose is immutable, the parent frame can (and does!) change over time relative to other frames, meaning that an individual pose can move relative
-to other frames. (For example a pose defined in the "robot" frame will conceptually move as the robot moves relative to a 'world'
+to other frames. (For example a pose defined in the `robot` frame will conceptually move as the robot moves relative to a `world`
 frame, even though its position and orientation remain immutably constant.)
 
 To make this very concrete, say the robot starts out at the world origin:
 
 ```python
-pose_in_robot_frame = pose.from_position_and_rotation([1,2,3], Rotation.identity(), "robot", pose_tree)
-pose_in_world_frame = pose_in_robot_frame.in_frame("world")
+pose_in_robot_frame = pose.from_position_and_rotation([1,2,3], Rotation.identity(), "robot", pose_tree) # fixed to robot
+pose_in_world_frame = pose_in_robot_frame.in_frame("world") # fixed to world
 
 pose_in_robot_frame.position # [1,2,3]
 pose_in_world_frame.position # [1,2,3]
 
 # Now the robot moves 1 meter forward in the world frame.
 robot.drive_forward_in_x(1)
 
-# Poses are immutable so this has not changed. One pose is [1,2,3] from the robot frame origin, one is [1,2,3] from the world origin.
+# Poses are immutable so they have not changed. One pose is [1,2,3] from the robot
+# frame origin, one is [1,2,3] from the world origin.
 pose_in_robot_frame.position # [1,2,3]
-pose_in_world_frame.position # [2,2,3]
+pose_in_world_frame.position # [1,2,3]
 
-# But if we express the one in robot frame in the world frame, we see that it is now 1 meter forward in x.
+# But if we express the one in robot frame in the world frame, we see that it 
+# is now 1 meter farther forward in x (because it was glued to the robot as 
+# it moved relative to the world.)
 pose_in_robot_frame.in_frame("world").position # [2,2,3]
 ```
 
 ## Connecting it to the rest of your stack.
 
-To connect a pose_tree instance you need to subclass PoseTree. Lets say you have an (fictional) object called `MyTransformManager` in your stack that subscribes to pose messages and implements `get_transform`. You would write something like:
+To connect a pose_tree instance you need to subclass PoseTree. Lets say your stack uses a (fictional) object called `MyTransformManager` that subscribes to pose messages and implements `get_transform` that returns some flavor of transform struct. You would write something like:
 
 ```python
 class MyPoseTree(CustomFramePoseTree):
     """My implementation of PoseTree to integrate with MyTransformManager"""
 
     def __init__(self, transform_manager: MyTransfrormManager):
-        self._tfm = transformManager
+        self._tfm = transform_manager
 
     def _get_transform(self, parent_frame: str, child_frame: str, timestamp: Optional[float] = None) -> Transform:
         transform_data = self._tfm.get_transform(parent_frame, child_frame, timestamp)
         return Transform.from_position_and_quaternion(
             [transform_data.tx, transform_data.ty, transform_data.tz],
             [transform_data.qx, transform_data.qy, transform_data.qz, transform_data.qw]
         )
@@ -209,8 +199,8 @@
 
 ## Contributing
 
 We welcome contributions! This is my first open source project so I don't know what I'm doing, but I'd especially like it if folks wanted to create PoseTree object implementations to wrap tf2 nicely for ROS and ROS2.
 
 ## License
 
-PoseTree is licensed under the [MIT license](https://github.com/robobenjie/posetree/blob/main/LICENSE).
+posetree is licensed under the [MIT license](https://github.com/robobenjie/posetree/blob/main/LICENSE).
```

### Comparing `posetree-1.0.0/README.md` & `posetree-1.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,63 @@
+Metadata-Version: 2.1
+Name: posetree
+Version: 1.1.0
+Summary: A Python library doing pose math for robotics.
+Author-email: Benjie Holson <bmholson@gmail.com>
+Project-URL: homepage, https://github.com/robobenjie/posetree
+Project-URL: documentation, https://htmlpreview.github.io/?https://raw.githubusercontent.com/robobenjie/posetree/main/docs/posetree/pose.html
+Project-URL: repository, https://github.com/robobenjie/posetree
+Project-URL: changelog, https://github.com/robobenjie/posetree/releases
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Scientific/Engineering
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # posetree
 
-`posetree` is an object-oriented, thread-safe, programmer-first, Python library for dealing with transforms, poses and frames, designed especially for robotics.
+`posetree` is an object-oriented, thread-safe, programmer-first, Python library for dealing with transforms, poses and frames, designed especially for robotics. It is unique in that Poses know their parent frame and it's relationship to other frames which allows for powerful operations with simple code.
 
 ## Installation
 
 ```
 pip install posetree
 ```
 
 ## Features
 
-* All poses are aware of all the frames which allows for powerful operations with simple code.
 * Write pose math designed for humans to read.
 * Think about quaternions as little as possible.
 * Never wonder if you are supposed to pre-multiply or post-multiply, or if you forgot an inverse somewhere.
-* Standalone and easy to integrate into any robotics stack.
+* Standalone, and easy to integrate into any robotics stack (works with ROS but does not depend on it).
 
 ## Basic Usage
 
 ```python
 from scipy.spatial.transform import Rotation
 from posetree import Pose
 
-looking_at = Pose.from_position_and_rotation([0, 0, 1], Rotation.identity(), "camera", pose_tree)
-
-height = looking_at.in_frame("robot").z
+# Create a pose from perception information
+pose_of_tea_bottle = Pose.from_position_and_rotation(
+    [-0.3, 0.4, 1.2], # Position of the bottle
+    Rotation.identity(), # Rotation of the bottle
+    parent_frame="camera", # Parent frame for position and rotation.
+    pose_tree=pose_tree) # PoseTree object to track frame relationships over time.
+
+# Calculate things based on other frames
+height_of_tea = pose_of_tea_bottle.in_frame("world").z
+distance_from_gripper = pose_of_tea_bottle.distance_to(gripper_pose)
 
+# Calculate some base motion targets relative to the current robot pose
 base_target = base_pose.translate([2, 0, 0]).rotate_about_z(np.pi/4)
-
 base_target2 = base_pose.point_x_at(human_pose).translate([1, 0, 0])
 
+# Get numbers out of a pose to send to a motion API
 x, y, _ = base_target.in_frame("map").position
 theta = base_target.angle_about_z_to(map_origin)
 navigate_to(x, y, theta)
 ```
 
 ## Philosophy of Transforms, Poses and Frames
 
@@ -49,23 +73,22 @@
 
 Notice we can take our example pose (standing at my front door facing the street) and transform it into another pose by using our transform instructions (take 10 steps forward and then turn 90 degrees to your left). If we do that we have a new pose that is a bit in front of my house and (in my case) facing our detached garage.
 
 - **Frame**: This is a pose that is so important we’ve decided to give it a name. 
     - Example: We could name “Standing at my front door facing the street” “journey_start” and then we could describe that other pose by saying, “from journey_start take 10 steps forward and turn 90 degrees to your left”
     - Example: We could name the left camera pose `"camera"`.
 
-You can sequence Transforms by multiplying them together, (as is traditional). This has a semantic meaning: "do this operation and then this other operation." However you cannot sequentially apply positions in 3D space so there is no multiply operator for Pose.
+You can sequence Transforms (by multiplying them together, as is traditional). This has a semantic meaning: i.e. "take 10 steps foreard and turn left THEN take 1 step backwards and turn around" which is equivalent to "take 10 steps forward and sidestep once right and then turn right". However you cannot sequentially apply positions in 3D space so there is intentionally no multiply operator for Pose. If this seems strange, I promise that as you use this library you will find that nearly every operation is easier and more clearly expressed via `in_frame`, `translate` or `rotate` operations instead of chains of `(world_t_robot * robot_t_camera * camera_t_object).inverse()` that you might be used to.
 
 ## Anchoring Poses in Frames.
 
 When constucting poses it is useful to think of what you expect the pose to be fixed relative to. For example, you might
-detect an apple on a table and get a pose from your perception system in the `camera` frame, but the apple is fixed relative to the table, so you will
-want to store your pose object with a the parent frame equal to `odometry/map/world`. Then, even if the robot moves, `apple_pose` will still refer to the
-best estimation of the apple's true location (with the usual caviats about localization drift and noise).
+detect an apple on a table and get a pose from your perception system in the `camera` frame, but the apple is actually sitting on the table, and we don't expect the apple to move if the camera moves. So you will want to store your pose object with a the parent frame equal to `odometry/map/world`. Then, even if the robot drives around, `apple_pose` will still refer to the best estimation of the apple's true location (with the usual caviats about localization drift and noise).
 
+Here's how to express that in `posetree`.
 ```python
 apple_pose = Pose(camera_t_apple, "camera", pose_tree).in_frame("world")
 ```
 
 Likewise if you have a bin on the back of a mobile robot and you want to define a drop-objects-into-bin pose right above it you can store
 that in the `robot` frame.
 
@@ -74,49 +97,47 @@
 ```
 
 When designing motion APIs with this library, you should be liberal in what frames you accept, and internally convert them to the frame you want to work in. 
 
 For example, in a function to move the arm to a pose:
 ```python
 def move_to_pose(self, target_pose: Pose):
-    # Convert the target to be relative to the base of the robot so we can execute the motion.
-    target_pose = target_pose.in_frame("robot")
-
     # Best Practice: turn Poses into Transforms at the last moment before acting on them.
-    arm_motion_primitives.move_arm_to_pose_relative_to_base(target_pose.transform)
+    arm_motion_primitives.move_arm_to_pose_relative_to_base(target_pose.in_frame("robot").transform)
 ```
 
 This formulation lets you combine the perception outputs and the motion methods for things like this:
 
 ```python
 def grasp_apple(self, apple_pose: Pose):
     # pregrasp is a pose 15 cm above the apple, with z pointing at it.
     pregrasp = apple_pose.translate([0, 0, 0.15], frame="world").point_z_at(apple_pose)
     self.move_to_pose(pregrasp)
 
     # Move down in the local 'z' of pregrasp until we touch the apple.
     self.move_to_pose_until_contact(pregrasp.translate([0, 0, 0.2]))
 
     # If we feel a contact too early, raise some reasonable error:
-    # We can check the distance using distance_to, even though the frames are different.
+    # We can check the distance using distance_to, even though the parent frames 
+    # of the two poses are different.
     if apple_pose.distance_to(get_tool_pose()) > 0.1:
         return "Whoops, we probably didn't get the apple."
 
     # Close the gripper and move up a bit from where ever we are, to lift the apple.
     self.close_gripper()
     self.move_to_pose(get_tool_pose().translate([0, 0, -0.1]))
 
     # Drop it in the bin.
     self.move_to_pose(drop_pose)
     self.open_gripper()
 ```
 
 ## Poses are Immutable
 
-Poses are immutable, and methods like `translate` return a new pose object. Immutability is nice because it makes them safe to pass into methods and also thread safe, but there is a gotcha to watch out for:
+Poses are immutable, and methods like `translate` return a new pose object. Immutability is nice because it makes them safe to pass into methods and also makes them thread safe, but there is a gotcha to watch out for:
 
 ```python
 # BAD!!! Do Not Do!
 p1.translate([1,0,0])
 p1.rotate_about_z(np.rad2deg(90))
 p1.with_position_x(5)
 # Surprise! p1 has not changed!
@@ -130,47 +151,50 @@
 # My favorite
 p2 = p1.translate([1,0,0]).rotate_about_z(np.rad2deg(90)).with_position_x(5)
 ```
 
 ## Immutability and Moving Frames
 
 While a Pose is immutable, the parent frame can (and does!) change over time relative to other frames, meaning that an individual pose can move relative
-to other frames. (For example a pose defined in the "robot" frame will conceptually move as the robot moves relative to a 'world'
+to other frames. (For example a pose defined in the `robot` frame will conceptually move as the robot moves relative to a `world`
 frame, even though its position and orientation remain immutably constant.)
 
 To make this very concrete, say the robot starts out at the world origin:
 
 ```python
-pose_in_robot_frame = pose.from_position_and_rotation([1,2,3], Rotation.identity(), "robot", pose_tree)
-pose_in_world_frame = pose_in_robot_frame.in_frame("world")
+pose_in_robot_frame = pose.from_position_and_rotation([1,2,3], Rotation.identity(), "robot", pose_tree) # fixed to robot
+pose_in_world_frame = pose_in_robot_frame.in_frame("world") # fixed to world
 
 pose_in_robot_frame.position # [1,2,3]
 pose_in_world_frame.position # [1,2,3]
 
 # Now the robot moves 1 meter forward in the world frame.
 robot.drive_forward_in_x(1)
 
-# Poses are immutable so this has not changed. One pose is [1,2,3] from the robot frame origin, one is [1,2,3] from the world origin.
+# Poses are immutable so they have not changed. One pose is [1,2,3] from the robot
+# frame origin, one is [1,2,3] from the world origin.
 pose_in_robot_frame.position # [1,2,3]
-pose_in_world_frame.position # [2,2,3]
+pose_in_world_frame.position # [1,2,3]
 
-# But if we express the one in robot frame in the world frame, we see that it is now 1 meter forward in x.
+# But if we express the one in robot frame in the world frame, we see that it 
+# is now 1 meter farther forward in x (because it was glued to the robot as 
+# it moved relative to the world.)
 pose_in_robot_frame.in_frame("world").position # [2,2,3]
 ```
 
 ## Connecting it to the rest of your stack.
 
-To connect a pose_tree instance you need to subclass PoseTree. Lets say you have an (fictional) object called `MyTransformManager` in your stack that subscribes to pose messages and implements `get_transform`. You would write something like:
+To connect a pose_tree instance you need to subclass PoseTree. Lets say your stack uses a (fictional) object called `MyTransformManager` that subscribes to pose messages and implements `get_transform` that returns some flavor of transform struct. You would write something like:
 
 ```python
 class MyPoseTree(CustomFramePoseTree):
     """My implementation of PoseTree to integrate with MyTransformManager"""
 
     def __init__(self, transform_manager: MyTransfrormManager):
-        self._tfm = transformManager
+        self._tfm = transform_manager
 
     def _get_transform(self, parent_frame: str, child_frame: str, timestamp: Optional[float] = None) -> Transform:
         transform_data = self._tfm.get_transform(parent_frame, child_frame, timestamp)
         return Transform.from_position_and_quaternion(
             [transform_data.tx, transform_data.ty, transform_data.tz],
             [transform_data.qx, transform_data.qy, transform_data.qz, transform_data.qw]
         )
@@ -192,8 +216,8 @@
 
 ## Contributing
 
 We welcome contributions! This is my first open source project so I don't know what I'm doing, but I'd especially like it if folks wanted to create PoseTree object implementations to wrap tf2 nicely for ROS and ROS2.
 
 ## License
 
-PoseTree is licensed under the [MIT license](https://github.com/robobenjie/posetree/blob/main/LICENSE).
+posetree is licensed under the [MIT license](https://github.com/robobenjie/posetree/blob/main/LICENSE).
```

### Comparing `posetree-1.0.0/posetree/pose.py` & `posetree-1.1.0/posetree/pose.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,90 +23,14 @@
     A Pose is an immutable location and orientation in 3D space.
     A pose is defined with a `parent_frame` (where to start) and a transform (how to get to the pose from the parent frame).
 
     Note: While a Pose is immutable, the parent frame can (and does!) change over time relative to other frames, meaning that an individual pose can move relative
     to other frames. (For example a pose defined in the "robot" frame will conceptually move as the robot moves relative to a 'world'
     frame, even though its position and orientation remain immutably constant.)
 
-    To make this very concrete, say the robot starts out at the world origin:
-
-    ```python
-    pose_in_robot_frame = pose.from_position_and_rotation([1,2,3], Rotation.identity(), "robot", pose_tree)
-    pose_in_world_frame = pose_in_robot_frame.in_frame("world")
-
-    pose_in_robot_frame.position # [1,2,3]
-    pose_in_world_frame.position # [1,2,3]
-
-    # Now the robot moves 1 meter forward in the world frame.
-    robot.drive_forward_in_x(1)
-
-    # Poses are immutable so this has not changed. One pose is [1,2,3] from the robot frame origin, one is [1,2,3] from the world origin.
-    pose_in_robot_frame.position # [1,2,3]
-    pose_in_world_frame.position # [2,2,3]
-
-    # But if we express the one in robot frame in the world frame, we see that it is now 1 meter forward in x.
-    pose_in_robot_frame.in_frame("world").position # [2,2,3]
-
-    ```
-    Of course, the above example assumes that the `pose_tree` is correctly hooked up to the robot odometry system, so the poses know that the frames 
-    have moved.
-
-    When constucting poses it is useful to think of what you expect the pose to be fixed relative to. For example, you might
-    detect an apple on a table and get a pose from your perception system in the `camera` frame, but the apple is fixed relative to the table, so you will
-    want to store your pose object with a the parent frame equal to `odometry/map/world`. Then, even if the robot moves, apple_pose will still refer to the
-    best estimation of the apple's true location (with the usual caviats about localization drift and noise).
-
-    ```
-    apple_pose = Pose(camera_t_apple, "camera", pose_tree).in_frame("world")
-    ```
-
-    Likewise if you have a bin on the back of a mobile robot and you want to define a drop-objects-into-bin pose right above it you can store
-    that in the `robot` frame.
-
-    ```
-    drop_pose = Pose.from_position_and_quaternion([-.3, 0.1, 0.25], [0, 0, 0, 1]), "robot", pose_tree)
-    ```
-
-    When designing motion APIs with this library, you should be liberal in what frames you accept, and internally convert them to the frame you want to work in. 
-
-    For example, in a function to move the arm to a pose:
-    ```
-    def move_to_pose(self, target_pose: Pose):
-        # Convert the target to be relative to the base of the robot so we can execute the motion.
-        target_pose = target_pose.in_frame("robot")
-
-        # Best Practice: turn Poses into Transforms at the last moment before acting on them.
-        arm_motion_primitives.move_arm_to_pose_relative_to_base(target_pose.transform)
-    ```
-
-    This formulation lets you combine the perception outputs and the motion methods for things like this:
-
-    ```
-    def grasp_apple(self, apple_pose: Pose):
-        # pregrasp is a pose 15 cm above the apple, with z pointing at it.
-        pregrasp = apple_pose.translate([0, 0, 0.15], frame="world").point_z_at(apple_pose)
-        self.move_to_pose(pregrasp)
-
-        # Move down in the local 'z' of pregrasp until we touch the apple.
-        self.move_to_pose_until_contact(pregrasp.translate([0, 0, 0.2]))
-
-        # If we feel a contact too early, raise some reasonable error:
-        # We can check the distance using distance_to, even though the frames are different.
-        if apple_pose.distance_to(get_tool_pose()) > 0.1:
-            return "Whoops, we probably didn't get the apple."
-
-        # Close the gripper and move up a bit from where ever we are, to lift the apple.
-        self.close_gripper()
-        self.move_to_pose(get_tool_pose().translate([0, 0, -0.1]))
-
-        # Drop it in the bin.
-        self.move_to_pose(drop_pose)
-        self.open_gripper()
-    ```
-
     """
     def __init__(self, transform: "Transform", parent_frame: str, pose_tree: "PoseTree") -> None:
         """Create a pose from a transform, frame, and pose tree.
         
         Args:
             transform: The transform from the frame to the pose.
             parent_frame: The frame that the transform is relative to.
@@ -337,75 +261,81 @@
         """
         if frame is None:
             return Pose(Transform(self.position + self.rotation.apply(translation), self.rotation), self.frame, self.pose_tree)
         else:
             self_frame_t_frame = self.pose_tree.get_transform(self.frame, frame)
             return Pose(Transform(self.position + self_frame_t_frame.rotation.apply(translation), self.rotation), self.frame, self.pose_tree)
     
-    def rotate_about_axis(self, axis: Sequence[float], angle: float, *, frame: Optional[str]=None) -> "Pose":
+    def rotate_about_axis(self, axis: Sequence[float], angle: float, *, degrees: bool = False, frame: Optional[str]=None) -> "Pose":
         """Return a new pose rotated about an axis.
 
         This is rotated in the basis of the pose being rotated (i.e body-fixed) rather than the parent frame, and it only
         rotates the orientation. This is *not* a rotation about the origin, but a change of the orientation of the pose.
 
         If you pass a frame, the axis will be interpreted as being expressed in that frame.
         
         Args:
             axis: The axis to rotate about.
-            angle: The angle to rotate by, in radians.
+            angle: The angle to rotate by, in radians unless degrees=True.
+            degrees: Whether the angle is in degrees.
             frame: The frame that the axis is relative to. If None, the axis is interpreted in the basis vectors of the pose (not the parent frame).
         
         Returns:
             A new pose with the same location but rotated about an axis.
         """
+        if degrees:
+            angle = np.deg2rad(angle)
         axis = np.array(axis)
         if (np.inner(axis, axis) - 1) > 1e-6:
             raise ValueError("Axis must be a unit vector.")
         if frame is None:
             new_rotation = self.rotation * Rotation.from_rotvec(axis * angle)
         else:
             frame_t_self_frame = self.pose_tree.get_transform(frame, self.frame)
             new_rotation = Rotation.from_rotvec(frame_t_self_frame.rotation.apply(axis) * angle) * self.rotation
         return Pose(Transform(self.position, new_rotation), self.frame, self.pose_tree)
     
-    def rotate_about_x(self, angle: float, *, frame: Optional[str]=None) -> "Pose":
+    def rotate_about_x(self, angle: float, *, degrees: bool = False, frame: Optional[str]=None) -> "Pose":
         """Return a new pose rotated about the x axis.
         
         Args:
-            angle: The angle to rotate by, in radians.
+            angle: The angle to rotate by, in radians unless degrees=True.
+            degrees: Whether the angle is in degrees.
             frame: The frame that the axis is relative to. If not provided, it will rotate about the x-unit-vector of the pose being rotated.
         
         Returns:
             A new pose with the same location but rotated about the x axis.
         """
-        return self.rotate_about_axis([1, 0, 0], angle, frame=frame)
+        return self.rotate_about_axis([1, 0, 0], angle, degrees=degrees, frame=frame)
     
-    def rotate_about_y(self, angle: float, *, frame: Optional[str]=None) -> "Pose":
+    def rotate_about_y(self, angle: float, *, degrees: bool = False, frame: Optional[str]=None) -> "Pose":
         """Return a new pose rotated about the y axis.
         
         Args:
-            angle: The angle to rotate by, in radians.
+            angle: The angle to rotate by, in radians unless degrees=True.
+            degrees: Whether the angle is in degrees.
             frame: The frame that the axis is relative to. If not provided, it will rotate about the y-unit-vector of the pose being rotated.
         
         Returns:
             A new pose with the same location but rotated about the y axis.
         """
-        return self.rotate_about_axis([0, 1, 0], angle, frame=frame)
+        return self.rotate_about_axis([0, 1, 0], angle, degrees=degrees, frame=frame)
     
-    def rotate_about_z(self, angle: float, *, frame: Optional[str]=None) -> "Pose":
+    def rotate_about_z(self, angle: float, *, degrees: bool = False, frame: Optional[str]=None) -> "Pose":
         """Return a new pose rotated about the z axis.
         
         Args:
-            angle: The angle to rotate by, in radians.
+            angle: The angle to rotate by, in radians unless degrees=True.
+            degrees: Whether the angle is in degrees.
             frame: The frame that the axis is relative to. If not provided, it will rotate about the z-unit-vector of the pose being rotated.
         
         Returns:
             A new pose with the same location but rotated about the z axis.
         """
-        return self.rotate_about_axis([0, 0, 1], angle, frame=frame)
+        return self.rotate_about_axis([0, 0, 1], angle, degrees=degrees, frame=frame)
     
     def point_x_at(self, target: "Pose", fixed_axis: str = None) -> "Pose":
         """Return a new pose rotated to point the x axis at a target pose.
         
         Args:
             target: The target pose to point at.
             fixed_axis: An optional axis ('x', 'y' or 'z') to keep fixed. If not provided,
@@ -539,15 +469,15 @@
 
         Raises:
             ValueError: If the rotation is more than 20% out of the expected axis.
         """
         return self._angle_about_axis_to(target, [0, 0, 1])
 
 
-    def _point_at(self, target: "Pose", axis: Sequence[float], fixed_axis: str=None)  -> "Pose":
+    def _point_at(self, target: "Pose", axis: Sequence[float], fixed_axis: str=None) -> "Pose":
         """Return a new pose rotated to point at a target pose.
         
         Args:
             target: The target pose to point at.
             axis: The axis to rotate about.
             fixed_axis: An optional axis ('x', 'y' or 'z') to keep fixed. If not provided,
                 the pose will be rotated the minimum rotation to have the axis point at the target pose..
```

### Comparing `posetree-1.0.0/posetree.egg-info/PKG-INFO` & `posetree-1.1.0/posetree.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: posetree
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Python library doing pose math for robotics.
 Author-email: Benjie Holson <bmholson@gmail.com>
 Project-URL: homepage, https://github.com/robobenjie/posetree
 Project-URL: documentation, https://htmlpreview.github.io/?https://raw.githubusercontent.com/robobenjie/posetree/main/docs/posetree/pose.html
 Project-URL: repository, https://github.com/robobenjie/posetree
 Project-URL: changelog, https://github.com/robobenjie/posetree/releases
 Classifier: Development Status :: 4 - Beta
@@ -13,44 +13,51 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # posetree
 
-`posetree` is an object-oriented, thread-safe, programmer-first, Python library for dealing with transforms, poses and frames, designed especially for robotics.
+`posetree` is an object-oriented, thread-safe, programmer-first, Python library for dealing with transforms, poses and frames, designed especially for robotics. It is unique in that Poses know their parent frame and it's relationship to other frames which allows for powerful operations with simple code.
 
 ## Installation
 
 ```
 pip install posetree
 ```
 
 ## Features
 
-* All poses are aware of all the frames which allows for powerful operations with simple code.
 * Write pose math designed for humans to read.
 * Think about quaternions as little as possible.
 * Never wonder if you are supposed to pre-multiply or post-multiply, or if you forgot an inverse somewhere.
-* Standalone and easy to integrate into any robotics stack.
+* Standalone, and easy to integrate into any robotics stack (works with ROS but does not depend on it).
 
 ## Basic Usage
 
 ```python
 from scipy.spatial.transform import Rotation
 from posetree import Pose
 
-looking_at = Pose.from_position_and_rotation([0, 0, 1], Rotation.identity(), "camera", pose_tree)
-
-height = looking_at.in_frame("robot").z
+# Create a pose from perception information
+pose_of_tea_bottle = Pose.from_position_and_rotation(
+    [-0.3, 0.4, 1.2], # Position of the bottle
+    Rotation.identity(), # Rotation of the bottle
+    parent_frame="camera", # Parent frame for position and rotation.
+    pose_tree=pose_tree) # PoseTree object to track frame relationships over time.
+
+# Calculate things based on other frames
+height_of_tea = pose_of_tea_bottle.in_frame("world").z
+distance_from_gripper = pose_of_tea_bottle.distance_to(gripper_pose)
 
+# Calculate some base motion targets relative to the current robot pose
 base_target = base_pose.translate([2, 0, 0]).rotate_about_z(np.pi/4)
-
 base_target2 = base_pose.point_x_at(human_pose).translate([1, 0, 0])
 
+# Get numbers out of a pose to send to a motion API
 x, y, _ = base_target.in_frame("map").position
 theta = base_target.angle_about_z_to(map_origin)
 navigate_to(x, y, theta)
 ```
 
 ## Philosophy of Transforms, Poses and Frames
 
@@ -66,23 +73,22 @@
 
 Notice we can take our example pose (standing at my front door facing the street) and transform it into another pose by using our transform instructions (take 10 steps forward and then turn 90 degrees to your left). If we do that we have a new pose that is a bit in front of my house and (in my case) facing our detached garage.
 
 - **Frame**: This is a pose that is so important we’ve decided to give it a name. 
     - Example: We could name “Standing at my front door facing the street” “journey_start” and then we could describe that other pose by saying, “from journey_start take 10 steps forward and turn 90 degrees to your left”
     - Example: We could name the left camera pose `"camera"`.
 
-You can sequence Transforms by multiplying them together, (as is traditional). This has a semantic meaning: "do this operation and then this other operation." However you cannot sequentially apply positions in 3D space so there is no multiply operator for Pose.
+You can sequence Transforms (by multiplying them together, as is traditional). This has a semantic meaning: i.e. "take 10 steps foreard and turn left THEN take 1 step backwards and turn around" which is equivalent to "take 10 steps forward and sidestep once right and then turn right". However you cannot sequentially apply positions in 3D space so there is intentionally no multiply operator for Pose. If this seems strange, I promise that as you use this library you will find that nearly every operation is easier and more clearly expressed via `in_frame`, `translate` or `rotate` operations instead of chains of `(world_t_robot * robot_t_camera * camera_t_object).inverse()` that you might be used to.
 
 ## Anchoring Poses in Frames.
 
 When constucting poses it is useful to think of what you expect the pose to be fixed relative to. For example, you might
-detect an apple on a table and get a pose from your perception system in the `camera` frame, but the apple is fixed relative to the table, so you will
-want to store your pose object with a the parent frame equal to `odometry/map/world`. Then, even if the robot moves, `apple_pose` will still refer to the
-best estimation of the apple's true location (with the usual caviats about localization drift and noise).
+detect an apple on a table and get a pose from your perception system in the `camera` frame, but the apple is actually sitting on the table, and we don't expect the apple to move if the camera moves. So you will want to store your pose object with a the parent frame equal to `odometry/map/world`. Then, even if the robot drives around, `apple_pose` will still refer to the best estimation of the apple's true location (with the usual caviats about localization drift and noise).
 
+Here's how to express that in `posetree`.
 ```python
 apple_pose = Pose(camera_t_apple, "camera", pose_tree).in_frame("world")
 ```
 
 Likewise if you have a bin on the back of a mobile robot and you want to define a drop-objects-into-bin pose right above it you can store
 that in the `robot` frame.
 
@@ -91,49 +97,47 @@
 ```
 
 When designing motion APIs with this library, you should be liberal in what frames you accept, and internally convert them to the frame you want to work in. 
 
 For example, in a function to move the arm to a pose:
 ```python
 def move_to_pose(self, target_pose: Pose):
-    # Convert the target to be relative to the base of the robot so we can execute the motion.
-    target_pose = target_pose.in_frame("robot")
-
     # Best Practice: turn Poses into Transforms at the last moment before acting on them.
-    arm_motion_primitives.move_arm_to_pose_relative_to_base(target_pose.transform)
+    arm_motion_primitives.move_arm_to_pose_relative_to_base(target_pose.in_frame("robot").transform)
 ```
 
 This formulation lets you combine the perception outputs and the motion methods for things like this:
 
 ```python
 def grasp_apple(self, apple_pose: Pose):
     # pregrasp is a pose 15 cm above the apple, with z pointing at it.
     pregrasp = apple_pose.translate([0, 0, 0.15], frame="world").point_z_at(apple_pose)
     self.move_to_pose(pregrasp)
 
     # Move down in the local 'z' of pregrasp until we touch the apple.
     self.move_to_pose_until_contact(pregrasp.translate([0, 0, 0.2]))
 
     # If we feel a contact too early, raise some reasonable error:
-    # We can check the distance using distance_to, even though the frames are different.
+    # We can check the distance using distance_to, even though the parent frames 
+    # of the two poses are different.
     if apple_pose.distance_to(get_tool_pose()) > 0.1:
         return "Whoops, we probably didn't get the apple."
 
     # Close the gripper and move up a bit from where ever we are, to lift the apple.
     self.close_gripper()
     self.move_to_pose(get_tool_pose().translate([0, 0, -0.1]))
 
     # Drop it in the bin.
     self.move_to_pose(drop_pose)
     self.open_gripper()
 ```
 
 ## Poses are Immutable
 
-Poses are immutable, and methods like `translate` return a new pose object. Immutability is nice because it makes them safe to pass into methods and also thread safe, but there is a gotcha to watch out for:
+Poses are immutable, and methods like `translate` return a new pose object. Immutability is nice because it makes them safe to pass into methods and also makes them thread safe, but there is a gotcha to watch out for:
 
 ```python
 # BAD!!! Do Not Do!
 p1.translate([1,0,0])
 p1.rotate_about_z(np.rad2deg(90))
 p1.with_position_x(5)
 # Surprise! p1 has not changed!
@@ -147,47 +151,50 @@
 # My favorite
 p2 = p1.translate([1,0,0]).rotate_about_z(np.rad2deg(90)).with_position_x(5)
 ```
 
 ## Immutability and Moving Frames
 
 While a Pose is immutable, the parent frame can (and does!) change over time relative to other frames, meaning that an individual pose can move relative
-to other frames. (For example a pose defined in the "robot" frame will conceptually move as the robot moves relative to a 'world'
+to other frames. (For example a pose defined in the `robot` frame will conceptually move as the robot moves relative to a `world`
 frame, even though its position and orientation remain immutably constant.)
 
 To make this very concrete, say the robot starts out at the world origin:
 
 ```python
-pose_in_robot_frame = pose.from_position_and_rotation([1,2,3], Rotation.identity(), "robot", pose_tree)
-pose_in_world_frame = pose_in_robot_frame.in_frame("world")
+pose_in_robot_frame = pose.from_position_and_rotation([1,2,3], Rotation.identity(), "robot", pose_tree) # fixed to robot
+pose_in_world_frame = pose_in_robot_frame.in_frame("world") # fixed to world
 
 pose_in_robot_frame.position # [1,2,3]
 pose_in_world_frame.position # [1,2,3]
 
 # Now the robot moves 1 meter forward in the world frame.
 robot.drive_forward_in_x(1)
 
-# Poses are immutable so this has not changed. One pose is [1,2,3] from the robot frame origin, one is [1,2,3] from the world origin.
+# Poses are immutable so they have not changed. One pose is [1,2,3] from the robot
+# frame origin, one is [1,2,3] from the world origin.
 pose_in_robot_frame.position # [1,2,3]
-pose_in_world_frame.position # [2,2,3]
+pose_in_world_frame.position # [1,2,3]
 
-# But if we express the one in robot frame in the world frame, we see that it is now 1 meter forward in x.
+# But if we express the one in robot frame in the world frame, we see that it 
+# is now 1 meter farther forward in x (because it was glued to the robot as 
+# it moved relative to the world.)
 pose_in_robot_frame.in_frame("world").position # [2,2,3]
 ```
 
 ## Connecting it to the rest of your stack.
 
-To connect a pose_tree instance you need to subclass PoseTree. Lets say you have an (fictional) object called `MyTransformManager` in your stack that subscribes to pose messages and implements `get_transform`. You would write something like:
+To connect a pose_tree instance you need to subclass PoseTree. Lets say your stack uses a (fictional) object called `MyTransformManager` that subscribes to pose messages and implements `get_transform` that returns some flavor of transform struct. You would write something like:
 
 ```python
 class MyPoseTree(CustomFramePoseTree):
     """My implementation of PoseTree to integrate with MyTransformManager"""
 
     def __init__(self, transform_manager: MyTransfrormManager):
-        self._tfm = transformManager
+        self._tfm = transform_manager
 
     def _get_transform(self, parent_frame: str, child_frame: str, timestamp: Optional[float] = None) -> Transform:
         transform_data = self._tfm.get_transform(parent_frame, child_frame, timestamp)
         return Transform.from_position_and_quaternion(
             [transform_data.tx, transform_data.ty, transform_data.tz],
             [transform_data.qx, transform_data.qy, transform_data.qz, transform_data.qw]
         )
@@ -209,8 +216,8 @@
 
 ## Contributing
 
 We welcome contributions! This is my first open source project so I don't know what I'm doing, but I'd especially like it if folks wanted to create PoseTree object implementations to wrap tf2 nicely for ROS and ROS2.
 
 ## License
 
-PoseTree is licensed under the [MIT license](https://github.com/robobenjie/posetree/blob/main/LICENSE).
+posetree is licensed under the [MIT license](https://github.com/robobenjie/posetree/blob/main/LICENSE).
```

### Comparing `posetree-1.0.0/pyproject.toml` & `posetree-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "posetree"
-version = "1.0.0"
+version = "1.1.0"
 description = "A Python library doing pose math for robotics."
 readme = "README.md"
 authors = [{name = "Benjie Holson", email = "bmholson@gmail.com"}]
 
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
@@ -17,13 +17,13 @@
 ]   
 
 dependencies = [
     "numpy>=1.21.2",
     "scipy>=1.7.1"
 ]
 
-
 [project.urls]
 homepage = "https://github.com/robobenjie/posetree"
 documentation = "https://htmlpreview.github.io/?https://raw.githubusercontent.com/robobenjie/posetree/main/docs/posetree/pose.html"
 repository = "https://github.com/robobenjie/posetree"
-changelog = "https://github.com/robobenjie/posetree/releases"
+changelog = "https://github.com/robobenjie/posetree/releases"
+
```

