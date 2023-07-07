# Comparing `tmp/hello_robot_stretch_factory-0.4.6.tar.gz` & `tmp/hello_robot_stretch_factory-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hello_robot_stretch_factory-0.4.6.tar", last modified: Fri Jun  9 20:05:37 2023, max compression
+gzip compressed data, was "hello_robot_stretch_factory-0.4.7.tar", last modified: Fri Jul  7 20:34:26 2023, max compression
```

## Comparing `hello_robot_stretch_factory-0.4.6.tar` & `hello_robot_stretch_factory-0.4.7.tar`

### file list

```diff
@@ -1,61 +1,60 @@
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-06-09 20:05:37.036178 hello_robot_stretch_factory-0.4.6/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      929 2022-08-24 21:41:11.000000 hello_robot_stretch_factory-0.4.6/LICENSE.md
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      816 2023-06-09 20:05:37.036178 hello_robot_stretch_factory-0.4.6/PKG-INFO
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      355 2022-09-08 01:34:28.000000 hello_robot_stretch_factory-0.4.6/README.md
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-06-09 20:05:37.032178 hello_robot_stretch_factory-0.4.6/hello_robot_stretch_factory.egg-info/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      816 2023-06-09 20:05:36.000000 hello_robot_stretch_factory-0.4.6/hello_robot_stretch_factory.egg-info/PKG-INFO
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1852 2023-06-09 20:05:36.000000 hello_robot_stretch_factory-0.4.6/hello_robot_stretch_factory.egg-info/SOURCES.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        1 2023-06-09 20:05:36.000000 hello_robot_stretch_factory-0.4.6/hello_robot_stretch_factory.egg-info/dependency_links.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       74 2023-06-09 20:05:36.000000 hello_robot_stretch_factory-0.4.6/hello_robot_stretch_factory.egg-info/requires.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       16 2023-06-09 20:05:36.000000 hello_robot_stretch_factory-0.4.6/hello_robot_stretch_factory.egg-info/top_level.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       38 2023-06-09 20:05:37.036178 hello_robot_stretch_factory-0.4.6/setup.cfg
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      995 2023-06-09 20:04:37.000000 hello_robot_stretch_factory-0.4.6/setup.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-06-09 20:05:37.036178 hello_robot_stretch_factory-0.4.6/stretch_factory/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        0 2022-08-24 21:41:11.000000 hello_robot_stretch_factory-0.4.6/stretch_factory/__init__.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6326 2022-12-27 02:18:42.000000 hello_robot_stretch_factory-0.4.6/stretch_factory/device_mgmt.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     4641 2023-06-09 20:03:58.000000 hello_robot_stretch_factory-0.4.6/stretch_factory/firmware_available.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     5248 2023-06-09 20:03:58.000000 hello_robot_stretch_factory-0.4.6/stretch_factory/firmware_installed.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3861 2023-06-09 20:03:58.000000 hello_robot_stretch_factory-0.4.6/stretch_factory/firmware_recommended.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    38099 2023-06-09 20:03:58.000000 hello_robot_stretch_factory-0.4.6/stretch_factory/firmware_updater.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     5254 2023-06-09 20:03:58.000000 hello_robot_stretch_factory-0.4.6/stretch_factory/firmware_utils.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2726 2023-06-09 20:03:58.000000 hello_robot_stretch_factory-0.4.6/stretch_factory/firmware_version.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    22204 2023-06-09 20:03:58.000000 hello_robot_stretch_factory-0.4.6/stretch_factory/hello_device_utils.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    12828 2022-09-08 01:34:28.000000 hello_robot_stretch_factory-0.4.6/stretch_factory/param_mgmt.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     9286 2023-06-09 20:03:58.000000 hello_robot_stretch_factory-0.4.6/stretch_factory/trace_mgmt.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-06-09 20:05:37.036178 hello_robot_stretch_factory-0.4.6/test/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      685 2022-08-24 21:41:11.000000 hello_robot_stretch_factory-0.4.6/test/test_firmware_updater.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      668 2022-08-24 21:41:11.000000 hello_robot_stretch_factory-0.4.6/test/test_usb_reset.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-06-09 20:05:37.032178 hello_robot_stretch_factory-0.4.6/tools/
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2456 2022-09-08 01:34:28.000000 hello_robot_stretch_factory-0.4.6/tools/RE1_migrate_contacts.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     6621 2022-08-24 21:41:11.000000 hello_robot_stretch_factory-0.4.6/tools/RE1_migrate_params.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    22012 2023-04-06 22:42:29.000000 hello_robot_stretch_factory-0.4.6/tools/REx_D435i_check.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5418 2022-09-08 01:34:28.000000 hello_robot_stretch_factory-0.4.6/tools/REx_base_calibrate_imu_collect.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    32027 2022-09-08 01:33:19.000000 hello_robot_stretch_factory-0.4.6/tools/REx_base_calibrate_imu_process.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5950 2022-09-08 01:33:19.000000 hello_robot_stretch_factory-0.4.6/tools/REx_base_calibrate_wheel_separation.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4771 2023-01-19 20:41:45.000000 hello_robot_stretch_factory-0.4.6/tools/REx_calibrate_gravity_comp.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     7456 2023-06-09 20:03:58.000000 hello_robot_stretch_factory-0.4.6/tools/REx_calibrate_guarded_contact.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3578 2022-12-27 02:18:42.000000 hello_robot_stretch_factory-0.4.6/tools/REx_calibrate_range.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1728 2022-09-08 01:33:19.000000 hello_robot_stretch_factory-0.4.6/tools/REx_cliff_sensor_calibrate.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5596 2023-06-09 20:03:58.000000 hello_robot_stretch_factory-0.4.6/tools/REx_comm_rates.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    18552 2023-01-20 00:09:05.000000 hello_robot_stretch_factory-0.4.6/tools/REx_discover_hello_devices.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1442 2022-09-08 01:33:19.000000 hello_robot_stretch_factory-0.4.6/tools/REx_dynamixel_id_change.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1354 2022-09-08 01:33:19.000000 hello_robot_stretch_factory-0.4.6/tools/REx_dynamixel_id_scan.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5045 2022-12-27 02:18:42.000000 hello_robot_stretch_factory-0.4.6/tools/REx_dynamixel_jog.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1374 2022-09-08 01:33:19.000000 hello_robot_stretch_factory-0.4.6/tools/REx_dynamixel_reboot.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1188 2022-09-08 01:33:19.000000 hello_robot_stretch_factory-0.4.6/tools/REx_dynamixel_set_baud.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2846 2023-06-09 20:03:58.000000 hello_robot_stretch_factory-0.4.6/tools/REx_firmware_flash.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5804 2023-06-09 20:03:58.000000 hello_robot_stretch_factory-0.4.6/tools/REx_firmware_updater.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1583 2022-09-08 01:33:19.000000 hello_robot_stretch_factory-0.4.6/tools/REx_gamepad_configure.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2338 2022-09-08 01:33:19.000000 hello_robot_stretch_factory-0.4.6/tools/REx_gripper_calibrate.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1947 2022-09-08 01:33:19.000000 hello_robot_stretch_factory-0.4.6/tools/REx_hello_dynamixel_jog.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      870 2022-09-08 01:34:28.000000 hello_robot_stretch_factory-0.4.6/tools/REx_stepper_calibration_YAML_to_flash.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      735 2023-06-09 20:03:58.000000 hello_robot_stretch_factory-0.4.6/tools/REx_stepper_calibration_flash_to_YAML.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1168 2022-09-08 01:34:28.000000 hello_robot_stretch_factory-0.4.6/tools/REx_stepper_calibration_run.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    18644 2022-09-08 01:33:19.000000 hello_robot_stretch_factory-0.4.6/tools/REx_stepper_ctrl_tuning.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1163 2022-09-08 01:33:19.000000 hello_robot_stretch_factory-0.4.6/tools/REx_stepper_gains.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4449 2023-06-09 20:03:58.000000 hello_robot_stretch_factory-0.4.6/tools/REx_stepper_jog.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      852 2022-09-08 01:33:19.000000 hello_robot_stretch_factory-0.4.6/tools/REx_stepper_mechaduino_menu.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1572 2023-06-09 20:03:58.000000 hello_robot_stretch_factory-0.4.6/tools/REx_trace_firmware.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     7819 2023-04-06 22:42:29.000000 hello_robot_stretch_factory-0.4.6/tools/REx_trace_robot.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2347 2022-09-08 01:33:19.000000 hello_robot_stretch_factory-0.4.6/tools/REx_usb_reset.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1379 2022-09-08 01:33:19.000000 hello_robot_stretch_factory-0.4.6/tools/REx_wacc_calibrate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:34:26.264521 hello_robot_stretch_factory-0.4.7/
+-rw-r--r--   0 root         (0) root         (0)      935 2023-07-07 20:34:26.264521 hello_robot_stretch_factory-0.4.7/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      355 2023-05-22 22:41:16.000000 hello_robot_stretch_factory-0.4.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:34:26.264521 hello_robot_stretch_factory-0.4.7/hello_robot_stretch_factory.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      935 2023-07-07 20:34:26.000000 hello_robot_stretch_factory-0.4.7/hello_robot_stretch_factory.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1841 2023-07-07 20:34:26.000000 hello_robot_stretch_factory-0.4.7/hello_robot_stretch_factory.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 20:34:26.000000 hello_robot_stretch_factory-0.4.7/hello_robot_stretch_factory.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       74 2023-07-07 20:34:26.000000 hello_robot_stretch_factory-0.4.7/hello_robot_stretch_factory.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-07 20:34:26.000000 hello_robot_stretch_factory-0.4.7/hello_robot_stretch_factory.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 20:34:26.264521 hello_robot_stretch_factory-0.4.7/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      995 2023-07-07 20:32:01.000000 hello_robot_stretch_factory-0.4.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:34:26.264521 hello_robot_stretch_factory-0.4.7/stretch_factory/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-22 22:41:16.000000 hello_robot_stretch_factory-0.4.7/stretch_factory/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6326 2023-05-22 22:41:16.000000 hello_robot_stretch_factory-0.4.7/stretch_factory/device_mgmt.py
+-rw-rw-r--   0 root         (0) root         (0)     4641 2023-05-22 22:41:16.000000 hello_robot_stretch_factory-0.4.7/stretch_factory/firmware_available.py
+-rw-rw-r--   0 root         (0) root         (0)     5248 2023-07-07 20:20:08.000000 hello_robot_stretch_factory-0.4.7/stretch_factory/firmware_installed.py
+-rw-rw-r--   0 root         (0) root         (0)     3861 2023-05-22 22:41:16.000000 hello_robot_stretch_factory-0.4.7/stretch_factory/firmware_recommended.py
+-rw-rw-r--   0 root         (0) root         (0)    38329 2023-07-07 20:32:01.000000 hello_robot_stretch_factory-0.4.7/stretch_factory/firmware_updater.py
+-rw-rw-r--   0 root         (0) root         (0)     5254 2023-05-22 22:41:16.000000 hello_robot_stretch_factory-0.4.7/stretch_factory/firmware_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     2726 2023-05-22 22:41:16.000000 hello_robot_stretch_factory-0.4.7/stretch_factory/firmware_version.py
+-rw-rw-r--   0 root         (0) root         (0)    22204 2023-05-22 22:41:16.000000 hello_robot_stretch_factory-0.4.7/stretch_factory/hello_device_utils.py
+-rw-rw-r--   0 root         (0) root         (0)    12828 2023-05-22 22:41:16.000000 hello_robot_stretch_factory-0.4.7/stretch_factory/param_mgmt.py
+-rwxrwxr-x   0 root         (0) root         (0)     9286 2023-05-24 00:26:56.000000 hello_robot_stretch_factory-0.4.7/stretch_factory/trace_mgmt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:34:26.264521 hello_robot_stretch_factory-0.4.7/test/
+-rw-rw-r--   0 root         (0) root         (0)      685 2023-05-22 22:41:16.000000 hello_robot_stretch_factory-0.4.7/test/test_firmware_updater.py
+-rw-rw-r--   0 root         (0) root         (0)      668 2023-05-22 22:41:16.000000 hello_robot_stretch_factory-0.4.7/test/test_usb_reset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:34:26.264521 hello_robot_stretch_factory-0.4.7/tools/
+-rwxrwxr-x   0 root         (0) root         (0)     2456 2023-05-22 22:41:16.000000 hello_robot_stretch_factory-0.4.7/tools/RE1_migrate_contacts.py
+-rwxrwxr-x   0 root         (0) root         (0)     6621 2023-05-22 22:41:16.000000 hello_robot_stretch_factory-0.4.7/tools/RE1_migrate_params.py
+-rwxrwxr-x   0 root         (0) root         (0)    22012 2023-05-22 22:41:16.000000 hello_robot_stretch_factory-0.4.7/tools/REx_D435i_check.py
+-rwxrwxr-x   0 root         (0) root         (0)     5418 2023-05-22 22:41:16.000000 hello_robot_stretch_factory-0.4.7/tools/REx_base_calibrate_imu_collect.py
+-rwxrwxr-x   0 root         (0) root         (0)    32027 2023-05-22 22:41:16.000000 hello_robot_stretch_factory-0.4.7/tools/REx_base_calibrate_imu_process.py
+-rwxrwxr-x   0 root         (0) root         (0)     5950 2023-05-22 22:41:16.000000 hello_robot_stretch_factory-0.4.7/tools/REx_base_calibrate_wheel_separation.py
+-rwxrwxr-x   0 root         (0) root         (0)     4771 2023-05-22 22:41:16.000000 hello_robot_stretch_factory-0.4.7/tools/REx_calibrate_gravity_comp.py
+-rwxrwxr-x   0 root         (0) root         (0)     7456 2023-05-22 22:41:16.000000 hello_robot_stretch_factory-0.4.7/tools/REx_calibrate_guarded_contact.py
+-rwxrwxr-x   0 root         (0) root         (0)     3578 2023-05-22 22:41:16.000000 hello_robot_stretch_factory-0.4.7/tools/REx_calibrate_range.py
+-rwxrwxr-x   0 root         (0) root         (0)     1728 2023-05-22 22:41:16.000000 hello_robot_stretch_factory-0.4.7/tools/REx_cliff_sensor_calibrate.py
+-rwxrwxr-x   0 root         (0) root         (0)     5596 2023-05-24 00:26:56.000000 hello_robot_stretch_factory-0.4.7/tools/REx_comm_rates.py
+-rwxrwxr-x   0 root         (0) root         (0)    18552 2023-05-22 22:41:16.000000 hello_robot_stretch_factory-0.4.7/tools/REx_discover_hello_devices.py
+-rwxrwxr-x   0 root         (0) root         (0)     1442 2023-05-22 22:41:16.000000 hello_robot_stretch_factory-0.4.7/tools/REx_dynamixel_id_change.py
+-rwxrwxr-x   0 root         (0) root         (0)     1354 2023-05-22 22:41:16.000000 hello_robot_stretch_factory-0.4.7/tools/REx_dynamixel_id_scan.py
+-rwxrwxr-x   0 root         (0) root         (0)     5045 2023-05-22 22:41:16.000000 hello_robot_stretch_factory-0.4.7/tools/REx_dynamixel_jog.py
+-rwxrwxr-x   0 root         (0) root         (0)     1374 2023-05-22 22:41:16.000000 hello_robot_stretch_factory-0.4.7/tools/REx_dynamixel_reboot.py
+-rwxrwxr-x   0 root         (0) root         (0)     1188 2023-05-22 22:41:16.000000 hello_robot_stretch_factory-0.4.7/tools/REx_dynamixel_set_baud.py
+-rwxrwxr-x   0 root         (0) root         (0)     2846 2023-05-22 22:41:16.000000 hello_robot_stretch_factory-0.4.7/tools/REx_firmware_flash.py
+-rwxrwxr-x   0 root         (0) root         (0)     5804 2023-05-22 22:41:16.000000 hello_robot_stretch_factory-0.4.7/tools/REx_firmware_updater.py
+-rwxrwxr-x   0 root         (0) root         (0)     1583 2023-05-22 22:41:16.000000 hello_robot_stretch_factory-0.4.7/tools/REx_gamepad_configure.py
+-rwxrwxr-x   0 root         (0) root         (0)     2338 2023-05-22 22:41:16.000000 hello_robot_stretch_factory-0.4.7/tools/REx_gripper_calibrate.py
+-rwxrwxr-x   0 root         (0) root         (0)     1947 2023-05-22 22:41:16.000000 hello_robot_stretch_factory-0.4.7/tools/REx_hello_dynamixel_jog.py
+-rwxrwxr-x   0 root         (0) root         (0)      870 2023-05-22 22:41:16.000000 hello_robot_stretch_factory-0.4.7/tools/REx_stepper_calibration_YAML_to_flash.py
+-rwxrwxr-x   0 root         (0) root         (0)      735 2023-05-22 22:41:16.000000 hello_robot_stretch_factory-0.4.7/tools/REx_stepper_calibration_flash_to_YAML.py
+-rwxrwxr-x   0 root         (0) root         (0)     1168 2023-05-22 22:41:16.000000 hello_robot_stretch_factory-0.4.7/tools/REx_stepper_calibration_run.py
+-rwxrwxr-x   0 root         (0) root         (0)    18644 2023-05-22 22:41:16.000000 hello_robot_stretch_factory-0.4.7/tools/REx_stepper_ctrl_tuning.py
+-rwxrwxr-x   0 root         (0) root         (0)     1163 2023-05-22 22:41:16.000000 hello_robot_stretch_factory-0.4.7/tools/REx_stepper_gains.py
+-rwxrwxr-x   0 root         (0) root         (0)     4449 2023-05-22 22:41:16.000000 hello_robot_stretch_factory-0.4.7/tools/REx_stepper_jog.py
+-rwxrwxr-x   0 root         (0) root         (0)      852 2023-05-22 22:41:16.000000 hello_robot_stretch_factory-0.4.7/tools/REx_stepper_mechaduino_menu.py
+-rwxrwxr-x   0 root         (0) root         (0)     1572 2023-05-24 00:26:56.000000 hello_robot_stretch_factory-0.4.7/tools/REx_trace_firmware.py
+-rwxrwxr-x   0 root         (0) root         (0)     7819 2023-05-22 22:41:16.000000 hello_robot_stretch_factory-0.4.7/tools/REx_trace_robot.py
+-rwxrwxr-x   0 root         (0) root         (0)     2347 2023-05-22 22:41:16.000000 hello_robot_stretch_factory-0.4.7/tools/REx_usb_reset.py
+-rwxrwxr-x   0 root         (0) root         (0)     1379 2023-05-22 22:41:16.000000 hello_robot_stretch_factory-0.4.7/tools/REx_wacc_calibrate.py
```

### Comparing `hello_robot_stretch_factory-0.4.6/PKG-INFO` & `hello_robot_stretch_factory-0.4.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: hello_robot_stretch_factory
-Version: 0.4.6
+Version: 0.4.7
 Summary: Stretch Factory Tools
 Home-page: https://github.com/hello-robot/stretch_factory
 Author: Hello Robot Inc.
 Author-email: support@hello-robot.com
+License: UNKNOWN
+Description: # Overview
+        
+        The Stretch Factory package provides Python tools for testing and calibration of the Hello Robot Stretch RE1 and RE2. 
+        
+        **These tools are provided for reference only and are intended to be used by qualified Hello Robot production engineers.** 
+        
+        This package can be installed by:
+        
+        ```
+        python -m pip install  -U hello-robot-stretch-factory
+        ```
+        
+        
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
-# Overview
-
-The Stretch Factory package provides Python tools for testing and calibration of the Hello Robot Stretch RE1 and RE2. 
-
-**These tools are provided for reference only and are intended to be used by qualified Hello Robot production engineers.** 
-
-This package can be installed by:
-
-```
-python -m pip install  -U hello-robot-stretch-factory
-```
-
```

### Comparing `hello_robot_stretch_factory-0.4.6/hello_robot_stretch_factory.egg-info/PKG-INFO` & `hello_robot_stretch_factory-0.4.7/hello_robot_stretch_factory.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: hello-robot-stretch-factory
-Version: 0.4.6
+Version: 0.4.7
 Summary: Stretch Factory Tools
 Home-page: https://github.com/hello-robot/stretch_factory
 Author: Hello Robot Inc.
 Author-email: support@hello-robot.com
+License: UNKNOWN
+Description: # Overview
+        
+        The Stretch Factory package provides Python tools for testing and calibration of the Hello Robot Stretch RE1 and RE2. 
+        
+        **These tools are provided for reference only and are intended to be used by qualified Hello Robot production engineers.** 
+        
+        This package can be installed by:
+        
+        ```
+        python -m pip install  -U hello-robot-stretch-factory
+        ```
+        
+        
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
-# Overview
-
-The Stretch Factory package provides Python tools for testing and calibration of the Hello Robot Stretch RE1 and RE2. 
-
-**These tools are provided for reference only and are intended to be used by qualified Hello Robot production engineers.** 
-
-This package can be installed by:
-
-```
-python -m pip install  -U hello-robot-stretch-factory
-```
-
```

### Comparing `hello_robot_stretch_factory-0.4.6/hello_robot_stretch_factory.egg-info/SOURCES.txt` & `hello_robot_stretch_factory-0.4.7/hello_robot_stretch_factory.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE.md
 README.md
 setup.py
 ./tools/RE1_migrate_contacts.py
 ./tools/RE1_migrate_params.py
 ./tools/REx_D435i_check.py
 ./tools/REx_base_calibrate_imu_collect.py
 ./tools/REx_base_calibrate_imu_process.py
```

### Comparing `hello_robot_stretch_factory-0.4.6/setup.py` & `hello_robot_stretch_factory-0.4.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 script_path='./tools'
 ex_scripts = glob.glob(script_path+'/*.py') + glob.glob(script_path+'/*.sh')
 stretch_scripts=[f for f in ex_scripts if isfile(f)]
 
 setuptools.setup(
     name="hello_robot_stretch_factory",
-    version="0.4.6",
+    version="0.4.7",
     author="Hello Robot Inc.",
     author_email="support@hello-robot.com",
     description="Stretch Factory Tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hello-robot/stretch_factory",
     scripts = stretch_scripts,
```

### Comparing `hello_robot_stretch_factory-0.4.6/stretch_factory/device_mgmt.py` & `hello_robot_stretch_factory-0.4.7/stretch_factory/device_mgmt.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/stretch_factory/firmware_available.py` & `hello_robot_stretch_factory-0.4.7/stretch_factory/firmware_available.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/stretch_factory/firmware_installed.py` & `hello_robot_stretch_factory-0.4.7/stretch_factory/firmware_installed.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/stretch_factory/firmware_recommended.py` & `hello_robot_stretch_factory-0.4.7/stretch_factory/firmware_recommended.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/stretch_factory/firmware_updater.py` & `hello_robot_stretch_factory-0.4.7/stretch_factory/firmware_updater.py`

 * *Files 2% similar despite different names*

```diff
@@ -466,14 +466,18 @@
         elif device_name == 'hello-pimu':
             dd = stretch_body.pimu.Pimu()
         else:
             dd = stretch_body.stepper.Stepper('/dev/' + device_name)
         if not dd.startup():
             click.secho('FAIL: Unable to establish comms with device %s' % device_name.upper(), fg="red")
             return False
+        else:
+            time.sleep(0.5)
+            dd.stop()
+            del dd
         click.secho('PASS: Established comms with device %s ' % device_name.upper(),fg="green")
         return True
 # ########################################################################################################3
     def flash_stepper_calibration(self, device_name):
         if device_name == 'hello-motor-arm' or device_name == 'hello-motor-lift' or device_name == 'hello-motor-right-wheel' or device_name == 'hello-motor-left-wheel':
             #click.secho(' Flashing Stepper Calibration: %s '.center(70, '#') % device_name, fg="cyan", bold=True)
             if not fwu.wait_on_device(device_name):
@@ -641,19 +645,24 @@
 #                 return all_success
 #         return True
 
 
 
 
     def create_arduino_config_file(self):
+        if  self.state['install_path']:
+            user_path = self.state['install_path']
+        else:
+            user_path = self.fw_available.repo_path + '/arduino'
+       
         arduino_config = {'board_manager': {'additional_urls': []},
                           'daemon': {'port': '50051'},
                           'directories': {'data': os.environ['HOME'] + '/.arduino15',
                                           'downloads': os.environ['HOME'] + '/.arduino15/staging',
-                                          'user': self.fw_available.repo_path + '/arduino'},
+                                          'user': user_path},
                           'library': {'enable_unsafe_install': False},
                           'logging': {'file': '', 'format': 'text', 'level': 'info'},
                           'metrics': {'addr': ':9090', 'enabled': True},
                           'sketch': {'always_export_binaries': False},
                           'telemetry': {'addr': ':9090', 'enabled': True}}
         with open(self.fw_available.repo_path + '/arduino-cli.yaml', 'w') as yaml_file:
             yaml.dump(arduino_config, yaml_file, default_flow_style=False)
```

### Comparing `hello_robot_stretch_factory-0.4.6/stretch_factory/firmware_utils.py` & `hello_robot_stretch_factory-0.4.7/stretch_factory/firmware_utils.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/stretch_factory/firmware_version.py` & `hello_robot_stretch_factory-0.4.7/stretch_factory/firmware_version.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/stretch_factory/hello_device_utils.py` & `hello_robot_stretch_factory-0.4.7/stretch_factory/hello_device_utils.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/stretch_factory/param_mgmt.py` & `hello_robot_stretch_factory-0.4.7/stretch_factory/param_mgmt.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/stretch_factory/trace_mgmt.py` & `hello_robot_stretch_factory-0.4.7/stretch_factory/trace_mgmt.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/test/test_firmware_updater.py` & `hello_robot_stretch_factory-0.4.7/test/test_firmware_updater.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/test/test_usb_reset.py` & `hello_robot_stretch_factory-0.4.7/test/test_usb_reset.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/tools/RE1_migrate_contacts.py` & `hello_robot_stretch_factory-0.4.7/tools/RE1_migrate_contacts.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/tools/RE1_migrate_params.py` & `hello_robot_stretch_factory-0.4.7/tools/RE1_migrate_params.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/tools/REx_D435i_check.py` & `hello_robot_stretch_factory-0.4.7/tools/REx_D435i_check.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/tools/REx_base_calibrate_imu_collect.py` & `hello_robot_stretch_factory-0.4.7/tools/REx_base_calibrate_imu_collect.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/tools/REx_base_calibrate_imu_process.py` & `hello_robot_stretch_factory-0.4.7/tools/REx_base_calibrate_imu_process.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/tools/REx_base_calibrate_wheel_separation.py` & `hello_robot_stretch_factory-0.4.7/tools/REx_base_calibrate_wheel_separation.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/tools/REx_calibrate_gravity_comp.py` & `hello_robot_stretch_factory-0.4.7/tools/REx_calibrate_gravity_comp.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/tools/REx_calibrate_guarded_contact.py` & `hello_robot_stretch_factory-0.4.7/tools/REx_calibrate_guarded_contact.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/tools/REx_calibrate_range.py` & `hello_robot_stretch_factory-0.4.7/tools/REx_calibrate_range.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/tools/REx_cliff_sensor_calibrate.py` & `hello_robot_stretch_factory-0.4.7/tools/REx_cliff_sensor_calibrate.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/tools/REx_comm_rates.py` & `hello_robot_stretch_factory-0.4.7/tools/REx_comm_rates.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/tools/REx_discover_hello_devices.py` & `hello_robot_stretch_factory-0.4.7/tools/REx_discover_hello_devices.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/tools/REx_dynamixel_id_change.py` & `hello_robot_stretch_factory-0.4.7/tools/REx_dynamixel_id_change.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/tools/REx_dynamixel_id_scan.py` & `hello_robot_stretch_factory-0.4.7/tools/REx_dynamixel_id_scan.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/tools/REx_dynamixel_jog.py` & `hello_robot_stretch_factory-0.4.7/tools/REx_dynamixel_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/tools/REx_dynamixel_reboot.py` & `hello_robot_stretch_factory-0.4.7/tools/REx_dynamixel_reboot.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/tools/REx_dynamixel_set_baud.py` & `hello_robot_stretch_factory-0.4.7/tools/REx_dynamixel_set_baud.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/tools/REx_firmware_flash.py` & `hello_robot_stretch_factory-0.4.7/tools/REx_firmware_flash.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/tools/REx_firmware_updater.py` & `hello_robot_stretch_factory-0.4.7/tools/REx_firmware_updater.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/tools/REx_gamepad_configure.py` & `hello_robot_stretch_factory-0.4.7/tools/REx_gamepad_configure.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/tools/REx_gripper_calibrate.py` & `hello_robot_stretch_factory-0.4.7/tools/REx_gripper_calibrate.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/tools/REx_hello_dynamixel_jog.py` & `hello_robot_stretch_factory-0.4.7/tools/REx_hello_dynamixel_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/tools/REx_stepper_calibration_YAML_to_flash.py` & `hello_robot_stretch_factory-0.4.7/tools/REx_stepper_calibration_YAML_to_flash.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/tools/REx_stepper_calibration_flash_to_YAML.py` & `hello_robot_stretch_factory-0.4.7/tools/REx_stepper_calibration_flash_to_YAML.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/tools/REx_stepper_calibration_run.py` & `hello_robot_stretch_factory-0.4.7/tools/REx_stepper_calibration_run.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/tools/REx_stepper_ctrl_tuning.py` & `hello_robot_stretch_factory-0.4.7/tools/REx_stepper_ctrl_tuning.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/tools/REx_stepper_gains.py` & `hello_robot_stretch_factory-0.4.7/tools/REx_stepper_gains.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/tools/REx_stepper_jog.py` & `hello_robot_stretch_factory-0.4.7/tools/REx_stepper_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/tools/REx_stepper_mechaduino_menu.py` & `hello_robot_stretch_factory-0.4.7/tools/REx_stepper_mechaduino_menu.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/tools/REx_trace_firmware.py` & `hello_robot_stretch_factory-0.4.7/tools/REx_trace_firmware.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/tools/REx_trace_robot.py` & `hello_robot_stretch_factory-0.4.7/tools/REx_trace_robot.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/tools/REx_usb_reset.py` & `hello_robot_stretch_factory-0.4.7/tools/REx_usb_reset.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.6/tools/REx_wacc_calibrate.py` & `hello_robot_stretch_factory-0.4.7/tools/REx_wacc_calibrate.py`

 * *Files identical despite different names*

