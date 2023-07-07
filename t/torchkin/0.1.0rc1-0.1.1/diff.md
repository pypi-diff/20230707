# Comparing `tmp/torchkin-0.1.0rc1.tar.gz` & `tmp/torchkin-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchkin-0.1.0rc1.tar", last modified: Mon Jun 26 20:48:03 2023, max compression
+gzip compressed data, was "torchkin-0.1.1.tar", last modified: Fri Jul  7 15:27:55 2023, max compression
```

## Comparing `torchkin-0.1.0rc1.tar` & `torchkin-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-06-26 20:48:03.626120 torchkin-0.1.0rc1/
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1088 2023-06-26 20:17:33.000000 torchkin-0.1.0rc1/LICENSE
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)       68 2023-06-26 20:47:55.000000 torchkin-0.1.0rc1/MANIFEST.in
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     2001 2023-06-26 20:48:03.624754 torchkin-0.1.0rc1/PKG-INFO
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1454 2023-06-26 19:49:48.000000 torchkin-0.1.0rc1/README.md
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)       31 2023-06-26 19:57:23.000000 torchkin-0.1.0rc1/requirements.txt
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)       38 2023-06-26 20:48:03.627099 torchkin-0.1.0rc1/setup.cfg
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1397 2023-06-26 20:47:04.000000 torchkin-0.1.0rc1/setup.py
-drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-06-26 20:48:03.600827 torchkin-0.1.0rc1/torchkin/
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      289 2023-06-26 20:26:45.000000 torchkin-0.1.0rc1/torchkin/__init__.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     6074 2023-06-26 19:42:33.000000 torchkin-0.1.0rc1/torchkin/forward_kinematics.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)    15460 2023-06-26 20:21:58.000000 torchkin-0.1.0rc1/torchkin/joint.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     8686 2023-06-26 20:21:58.000000 torchkin-0.1.0rc1/torchkin/robot.py
-drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-06-26 20:48:03.620464 torchkin-0.1.0rc1/torchkin.egg-info/
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     2001 2023-06-26 20:48:03.000000 torchkin-0.1.0rc1/torchkin.egg-info/PKG-INFO
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      302 2023-06-26 20:48:03.000000 torchkin-0.1.0rc1/torchkin.egg-info/SOURCES.txt
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)        1 2023-06-26 20:48:03.000000 torchkin-0.1.0rc1/torchkin.egg-info/dependency_links.txt
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)       31 2023-06-26 20:48:03.000000 torchkin-0.1.0rc1/torchkin.egg-info/requires.txt
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)        9 2023-06-26 20:48:03.000000 torchkin-0.1.0rc1/torchkin.egg-info/top_level.txt
+drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-07-07 15:27:55.354990 torchkin-0.1.1/
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1088 2023-06-27 18:16:27.000000 torchkin-0.1.1/LICENSE
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)       68 2023-06-27 18:16:27.000000 torchkin-0.1.1/MANIFEST.in
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     6018 2023-07-07 15:27:55.353648 torchkin-0.1.1/PKG-INFO
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     5474 2023-06-28 01:10:53.000000 torchkin-0.1.1/README.md
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)       31 2023-06-27 18:16:27.000000 torchkin-0.1.1/requirements.txt
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)       38 2023-07-07 15:27:55.356008 torchkin-0.1.1/setup.cfg
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1397 2023-06-27 18:16:27.000000 torchkin-0.1.1/setup.py
+drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-07-07 15:27:55.331038 torchkin-0.1.1/torchkin/
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      286 2023-07-07 15:27:26.000000 torchkin-0.1.1/torchkin/__init__.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     6108 2023-07-06 16:24:10.000000 torchkin-0.1.1/torchkin/forward_kinematics.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)    15466 2023-07-06 21:51:37.000000 torchkin-0.1.1/torchkin/joint.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     8686 2023-06-27 18:16:27.000000 torchkin-0.1.1/torchkin/robot.py
+drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-07-07 15:27:55.349838 torchkin-0.1.1/torchkin.egg-info/
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     6018 2023-07-07 15:27:55.000000 torchkin-0.1.1/torchkin.egg-info/PKG-INFO
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      302 2023-07-07 15:27:55.000000 torchkin-0.1.1/torchkin.egg-info/SOURCES.txt
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)        1 2023-07-07 15:27:55.000000 torchkin-0.1.1/torchkin.egg-info/dependency_links.txt
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)       31 2023-07-07 15:27:55.000000 torchkin-0.1.1/torchkin.egg-info/requires.txt
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)        9 2023-07-07 15:27:55.000000 torchkin-0.1.1/torchkin.egg-info/top_level.txt
```

### Comparing `torchkin-0.1.0rc1/LICENSE` & `torchkin-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `torchkin-0.1.0rc1/setup.py` & `torchkin-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `torchkin-0.1.0rc1/torchkin/forward_kinematics.py` & `torchkin-0.1.1/torchkin/forward_kinematics.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,18 +86,20 @@
         @staticmethod
         def backward(ctx, *grad_outputs):
             rets: tuple(torch.Tensor) = ctx.saved_tensors
             if not hasattr(ctx, "jposes"):
                 ctx.jposes: torch.Tensor = _forward_kinematics_backward_helper(
                     ctx.poses
                 )
-            grad_pose = grad_outputs[0].new_zeros(
-                grad_outputs[0].shape[0], 6, robot.dof
+            grad_pose = grad_outputs[-2].new_zeros(
+                grad_outputs[-2].shape[0], 6, robot.dof
+            )
+            grad_input = grad_outputs[-2].new_zeros(
+                grad_outputs[-2].shape[0], robot.dof
             )
-            grad_input = grad_outputs[0].new_zeros(grad_outputs[0].shape[0], robot.dof)
 
             for link_id, ret, grad_output in zip(link_ids, rets, grad_outputs):
                 ancestor_non_fixed_joint_ids = robot.links[
                     link_id
                 ].ancestor_non_fixed_joint_ids
                 temp = SE3.project(
                     torch.cat(
```

### Comparing `torchkin-0.1.0rc1/torchkin/joint.py` & `torchkin-0.1.1/torchkin/joint.py`

 * *Files 0% similar despite different names*

```diff
@@ -359,15 +359,15 @@
         if angle.ndim == 1:
             angle = angle.view(-1, 1)
         if angle.ndim != 2 or angle.shape[1] != 1:
             raise ValueError("The joint angle must be a vector.")
 
     def translation(self, angle: torch.Tensor) -> torch.Tensor:
         _PrismaticJointImpl._check_input(angle)
-        return self.translation(angle.view(-1, 1))
+        return self._translation_impl(angle.view(-1, 1))
 
     def _relative_pose_impl(self, angle: torch.Tensor) -> torch.Tensor:
         trans = self.translation(angle)
         ret = angle.new_empty(angle.shape[0], 3, 4)
         ret[:, :, :3] = self.origin[:, :, :3]
         ret[:, :, 3:] = (
             self.origin[:, :, :3] @ trans.view(-1, 3, 1) + self.origin[:, :, 3:]
```

### Comparing `torchkin-0.1.0rc1/torchkin/robot.py` & `torchkin-0.1.1/torchkin/robot.py`

 * *Files identical despite different names*

