# Comparing `tmp/skellyforge-2023.6.1002.tar.gz` & `tmp/skellyforge-2023.7.1003.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skellyforge-2023.6.1002.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "skellyforge-2023.7.1003.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `skellyforge-2023.6.1002.tar` & `skellyforge-2023.7.1003.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1087 2023-06-28 16:36:51.690631 skellyforge-2023.6.1002/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
--rw-r--r--   0        0        0        7 2023-06-28 16:36:51.690631 skellyforge-2023.6.1002/.gitignore
--rw-r--r--   0        0        0       47 2023-06-28 16:36:51.690631 skellyforge-2023.6.1002/.idea/.gitignore
--rw-r--r--   0        0        0      501 2023-06-28 16:36:51.690631 skellyforge-2023.6.1002/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2023-06-28 16:36:51.690631 skellyforge-2023.6.1002/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      185 2023-06-28 16:36:51.690631 skellyforge-2023.6.1002/.idea/misc.xml
--rw-r--r--   0        0        0      288 2023-06-28 16:36:51.690631 skellyforge-2023.6.1002/.idea/modules.xml
--rw-r--r--   0        0        0      284 2023-06-28 16:36:51.690631 skellyforge-2023.6.1002/.idea/postprocessing_gui.iml
--rw-r--r--   0        0        0      180 2023-06-28 16:36:51.690631 skellyforge-2023.6.1002/.idea/vcs.xml
--rw-r--r--   0        0        0      496 2023-06-28 16:36:51.690631 skellyforge-2023.6.1002/.vscode/launch.json
--rw-r--r--   0        0        0    34522 2023-06-28 16:36:51.694631 skellyforge-2023.6.1002/LICENSE
--rw-r--r--   0        0        0     1835 2023-06-28 16:36:51.694631 skellyforge-2023.6.1002/README.md
--rw-r--r--   0        0        0     1560 2023-06-28 16:36:51.694631 skellyforge-2023.6.1002/pyproject.toml
--rw-r--r--   0        0        0       62 2023-06-28 16:36:51.694631 skellyforge-2023.6.1002/requirements.txt
--rw-r--r--   0        0        0       38 2023-06-28 16:36:51.694631 skellyforge-2023.6.1002/setup.py
--rw-r--r--   0        0        0      770 2023-06-28 16:36:51.694631 skellyforge-2023.6.1002/skellyforge/__init__.py
--rw-r--r--   0        0        0      321 2023-06-28 16:36:51.694631 skellyforge-2023.6.1002/skellyforge/__main__.py
--rw-r--r--   0        0        0      657 2023-06-28 16:36:51.694631 skellyforge-2023.6.1002/skellyforge/freemocap_utils/config.py
--rw-r--r--   0        0        0      488 2023-06-28 16:36:51.694631 skellyforge-2023.6.1002/skellyforge/freemocap_utils/constants.py
--rw-r--r--   0        0        0     3385 2023-06-28 16:36:51.694631 skellyforge-2023.6.1002/skellyforge/freemocap_utils/postprocessing_widgets/led_widgets.py
--rw-r--r--   0        0        0     3558 2023-06-28 16:36:51.694631 skellyforge-2023.6.1002/skellyforge/freemocap_utils/postprocessing_widgets/menus/filtering_menu.py
--rw-r--r--   0        0        0     3598 2023-06-28 16:36:51.694631 skellyforge-2023.6.1002/skellyforge/freemocap_utils/postprocessing_widgets/menus/interpolation_menu.py
--rw-r--r--   0        0        0     8299 2023-06-28 16:36:51.694631 skellyforge-2023.6.1002/skellyforge/freemocap_utils/postprocessing_widgets/menus/main_menu.py
--rw-r--r--   0        0        0     2640 2023-06-28 16:36:51.694631 skellyforge-2023.6.1002/skellyforge/freemocap_utils/postprocessing_widgets/parameter_tree_builder.py
--rw-r--r--   0        0        0     3727 2023-06-28 16:36:51.694631 skellyforge-2023.6.1002/skellyforge/freemocap_utils/postprocessing_widgets/parameter_widgets.py
--rw-r--r--   0        0        0     1034 2023-06-28 16:36:51.694631 skellyforge-2023.6.1002/skellyforge/freemocap_utils/postprocessing_widgets/postprocessing_functions/filter_data.py
--rw-r--r--   0        0        0     4599 2023-06-28 16:36:51.694631 skellyforge-2023.6.1002/skellyforge/freemocap_utils/postprocessing_widgets/postprocessing_functions/good_frame_finder.py
--rw-r--r--   0        0        0     1325 2023-06-28 16:36:51.694631 skellyforge-2023.6.1002/skellyforge/freemocap_utils/postprocessing_widgets/postprocessing_functions/interpolate_data.py
--rw-r--r--   0        0        0     8553 2023-06-28 16:36:51.694631 skellyforge-2023.6.1002/skellyforge/freemocap_utils/postprocessing_widgets/postprocessing_functions/rotate_skeleton.py
--rw-r--r--   0        0        0      415 2023-06-28 16:36:51.694631 skellyforge-2023.6.1002/skellyforge/freemocap_utils/postprocessing_widgets/stylesheet.py
--rw-r--r--   0        0        0     5113 2023-06-28 16:36:51.694631 skellyforge-2023.6.1002/skellyforge/freemocap_utils/postprocessing_widgets/task_worker_thread.py
--rw-r--r--   0        0        0     1063 2023-06-28 16:36:51.694631 skellyforge-2023.6.1002/skellyforge/freemocap_utils/postprocessing_widgets/visualization_widgets/marker_selector_widget.py
--rw-r--r--   0        0        0     3779 2023-06-28 16:36:51.694631 skellyforge-2023.6.1002/skellyforge/freemocap_utils/postprocessing_widgets/visualization_widgets/mediapipe_skeleton_builder.py
--rw-r--r--   0        0        0     4222 2023-06-28 16:36:51.694631 skellyforge-2023.6.1002/skellyforge/freemocap_utils/postprocessing_widgets/visualization_widgets/skeleton_view_widget.py
--rw-r--r--   0        0        0     1129 2023-06-28 16:36:51.694631 skellyforge-2023.6.1002/skellyforge/freemocap_utils/postprocessing_widgets/visualization_widgets/skeleton_viewers_container.py
--rw-r--r--   0        0        0      816 2023-06-28 16:36:51.694631 skellyforge-2023.6.1002/skellyforge/freemocap_utils/postprocessing_widgets/visualization_widgets/slider_widget.py
--rw-r--r--   0        0        0     2871 2023-06-28 16:36:51.694631 skellyforge-2023.6.1002/skellyforge/freemocap_utils/postprocessing_widgets/visualization_widgets/timeseries_view_widget.py
--rw-r--r--   0        0        0      746 2023-06-28 16:36:51.694631 skellyforge-2023.6.1002/skellyforge/headless_task_worker_test.py
--rw-r--r--   0        0        0     3382 2023-06-28 16:36:51.694631 skellyforge-2023.6.1002/skellyforge/postprocess_GUI.py
--rw-r--r--   0        0        0     2684 1970-01-01 00:00:00.000000 skellyforge-2023.6.1002/PKG-INFO
+-rw-r--r--   0        0        0     1087 2023-07-07 19:45:33.051835 skellyforge-2023.7.1003/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
+-rw-r--r--   0        0        0        7 2023-07-07 19:45:33.051835 skellyforge-2023.7.1003/.gitignore
+-rw-r--r--   0        0        0       47 2023-07-07 19:45:33.051835 skellyforge-2023.7.1003/.idea/.gitignore
+-rw-r--r--   0        0        0      501 2023-07-07 19:45:33.051835 skellyforge-2023.7.1003/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2023-07-07 19:45:33.051835 skellyforge-2023.7.1003/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      185 2023-07-07 19:45:33.055835 skellyforge-2023.7.1003/.idea/misc.xml
+-rw-r--r--   0        0        0      288 2023-07-07 19:45:33.055835 skellyforge-2023.7.1003/.idea/modules.xml
+-rw-r--r--   0        0        0      284 2023-07-07 19:45:33.055835 skellyforge-2023.7.1003/.idea/postprocessing_gui.iml
+-rw-r--r--   0        0        0      180 2023-07-07 19:45:33.055835 skellyforge-2023.7.1003/.idea/vcs.xml
+-rw-r--r--   0        0        0      496 2023-07-07 19:45:33.055835 skellyforge-2023.7.1003/.vscode/launch.json
+-rw-r--r--   0        0        0    34522 2023-07-07 19:45:33.055835 skellyforge-2023.7.1003/LICENSE
+-rw-r--r--   0        0        0     1708 2023-07-07 19:45:33.055835 skellyforge-2023.7.1003/README.md
+-rw-r--r--   0        0        0     1553 2023-07-07 19:45:33.055835 skellyforge-2023.7.1003/pyproject.toml
+-rw-r--r--   0        0        0       62 2023-07-07 19:45:33.055835 skellyforge-2023.7.1003/requirements.txt
+-rw-r--r--   0        0        0       38 2023-07-07 19:45:33.055835 skellyforge-2023.7.1003/setup.py
+-rw-r--r--   0        0        0      770 2023-07-07 19:45:33.055835 skellyforge-2023.7.1003/skellyforge/__init__.py
+-rw-r--r--   0        0        0      321 2023-07-07 19:45:33.055835 skellyforge-2023.7.1003/skellyforge/__main__.py
+-rw-r--r--   0        0        0      657 2023-07-07 19:45:33.055835 skellyforge-2023.7.1003/skellyforge/freemocap_utils/config.py
+-rw-r--r--   0        0        0      488 2023-07-07 19:45:33.055835 skellyforge-2023.7.1003/skellyforge/freemocap_utils/constants.py
+-rw-r--r--   0        0        0     3385 2023-07-07 19:45:33.055835 skellyforge-2023.7.1003/skellyforge/freemocap_utils/postprocessing_widgets/led_widgets.py
+-rw-r--r--   0        0        0     3558 2023-07-07 19:45:33.055835 skellyforge-2023.7.1003/skellyforge/freemocap_utils/postprocessing_widgets/menus/filtering_menu.py
+-rw-r--r--   0        0        0     3598 2023-07-07 19:45:33.055835 skellyforge-2023.7.1003/skellyforge/freemocap_utils/postprocessing_widgets/menus/interpolation_menu.py
+-rw-r--r--   0        0        0     8299 2023-07-07 19:45:33.055835 skellyforge-2023.7.1003/skellyforge/freemocap_utils/postprocessing_widgets/menus/main_menu.py
+-rw-r--r--   0        0        0     2640 2023-07-07 19:45:33.055835 skellyforge-2023.7.1003/skellyforge/freemocap_utils/postprocessing_widgets/parameter_tree_builder.py
+-rw-r--r--   0        0        0     3727 2023-07-07 19:45:33.055835 skellyforge-2023.7.1003/skellyforge/freemocap_utils/postprocessing_widgets/parameter_widgets.py
+-rw-r--r--   0        0        0     1034 2023-07-07 19:45:33.055835 skellyforge-2023.7.1003/skellyforge/freemocap_utils/postprocessing_widgets/postprocessing_functions/filter_data.py
+-rw-r--r--   0        0        0     4599 2023-07-07 19:45:33.055835 skellyforge-2023.7.1003/skellyforge/freemocap_utils/postprocessing_widgets/postprocessing_functions/good_frame_finder.py
+-rw-r--r--   0        0        0     1325 2023-07-07 19:45:33.055835 skellyforge-2023.7.1003/skellyforge/freemocap_utils/postprocessing_widgets/postprocessing_functions/interpolate_data.py
+-rw-r--r--   0        0        0     8553 2023-07-07 19:45:33.055835 skellyforge-2023.7.1003/skellyforge/freemocap_utils/postprocessing_widgets/postprocessing_functions/rotate_skeleton.py
+-rw-r--r--   0        0        0      415 2023-07-07 19:45:33.055835 skellyforge-2023.7.1003/skellyforge/freemocap_utils/postprocessing_widgets/stylesheet.py
+-rw-r--r--   0        0        0     5113 2023-07-07 19:45:33.055835 skellyforge-2023.7.1003/skellyforge/freemocap_utils/postprocessing_widgets/task_worker_thread.py
+-rw-r--r--   0        0        0     1063 2023-07-07 19:45:33.055835 skellyforge-2023.7.1003/skellyforge/freemocap_utils/postprocessing_widgets/visualization_widgets/marker_selector_widget.py
+-rw-r--r--   0        0        0     3779 2023-07-07 19:45:33.055835 skellyforge-2023.7.1003/skellyforge/freemocap_utils/postprocessing_widgets/visualization_widgets/mediapipe_skeleton_builder.py
+-rw-r--r--   0        0        0     4217 2023-07-07 19:45:33.055835 skellyforge-2023.7.1003/skellyforge/freemocap_utils/postprocessing_widgets/visualization_widgets/skeleton_view_widget.py
+-rw-r--r--   0        0        0     1129 2023-07-07 19:45:33.055835 skellyforge-2023.7.1003/skellyforge/freemocap_utils/postprocessing_widgets/visualization_widgets/skeleton_viewers_container.py
+-rw-r--r--   0        0        0      816 2023-07-07 19:45:33.055835 skellyforge-2023.7.1003/skellyforge/freemocap_utils/postprocessing_widgets/visualization_widgets/slider_widget.py
+-rw-r--r--   0        0        0     2871 2023-07-07 19:45:33.055835 skellyforge-2023.7.1003/skellyforge/freemocap_utils/postprocessing_widgets/visualization_widgets/timeseries_view_widget.py
+-rw-r--r--   0        0        0      746 2023-07-07 19:45:33.055835 skellyforge-2023.7.1003/skellyforge/headless_task_worker_test.py
+-rw-r--r--   0        0        0     3382 2023-07-07 19:45:33.055835 skellyforge-2023.7.1003/skellyforge/postprocess_GUI.py
+-rw-r--r--   0        0        0     2550 1970-01-01 00:00:00.000000 skellyforge-2023.7.1003/PKG-INFO
```

### Comparing `skellyforge-2023.6.1002/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml` & `skellyforge-2023.7.1003/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml`

 * *Files identical despite different names*

### Comparing `skellyforge-2023.6.1002/LICENSE` & `skellyforge-2023.7.1003/LICENSE`

 * *Files identical despite different names*

### Comparing `skellyforge-2023.6.1002/README.md` & `skellyforge-2023.7.1003/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # postprocessing_gui
 
 # INSTALLING the GUI
  1. Create a 3.9 or 3.10 conda environment environment 
    -have tested this successfully on 3.9.16 (latest 3.9 version) and 3.10.11 (latest 3.10 version)
- 2. Navigate to this github repo and use the command `pip install -r requirements.txt` to install the dependencies
-   -Note: I pinned the matplotlib version at 3.6.3 for now because 3.7.0 and above were causing some errors to pop up with the 3D plot
+ 2. Navigate to this github repo and use the command `pip install -e.` to install the dependencies from the pyproject.toml
 
 # STARTING the GUI:
  1. Open up `postprocess_GUI.py`
  2. Scroll down to the `if __name__ == '__main__'` section at the bottom
  3. Change the `path_to_data_folder` variable to the path to your recording
    -NOTE: The GUI is set up to take file paths and file names corresponding to the 
           FreeMoCap 1.0 release. If you need to change these file paths, you can do so
```

### Comparing `skellyforge-2023.6.1002/pyproject.toml` & `skellyforge-2023.7.1003/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -28,27 +28,27 @@
 dependencies = [
 "numpy",
 "pyqt6",
 "pyqtgraph",
 "scipy",
 "rich",
 "pandas",
-"matplotlib==3.6.3",
+"matplotlib",
 "toml",
 ] #add additional dependencies here - try to pin versions as minimally as possible
 
 requires-python = ">=3.8"
 
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [tool.bumpver] #bump the version by entering `bumpver update` in the terminal
-current_version = "v2023.06.1002"
+current_version = "v2023.07.1003"
 version_pattern = "vYYYY.0M.BUILD[-TAG]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `skellyforge-2023.6.1002/skellyforge/__init__.py` & `skellyforge-2023.7.1003/skellyforge/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Top-level package for basic_template_repo."""
 
 __package_name__ = "skellyforge"
-__version__ = "v2023.06.1002"
+__version__ = "v2023.07.1003"
 
 __author__ = """Aaron Cherian"""
 __email__ = "info@freemocap.org"
 __repo_owner_github_user_name__ = "freemocap"
 __repo_url__ = (
     f"https://github.com/{__repo_owner_github_user_name__}/{__package_name__}/"
 )
```

### Comparing `skellyforge-2023.6.1002/skellyforge/freemocap_utils/config.py` & `skellyforge-2023.7.1003/skellyforge/freemocap_utils/config.py`

 * *Files identical despite different names*

### Comparing `skellyforge-2023.6.1002/skellyforge/freemocap_utils/postprocessing_widgets/led_widgets.py` & `skellyforge-2023.7.1003/skellyforge/freemocap_utils/postprocessing_widgets/led_widgets.py`

 * *Files identical despite different names*

### Comparing `skellyforge-2023.6.1002/skellyforge/freemocap_utils/postprocessing_widgets/menus/filtering_menu.py` & `skellyforge-2023.7.1003/skellyforge/freemocap_utils/postprocessing_widgets/menus/filtering_menu.py`

 * *Files identical despite different names*

### Comparing `skellyforge-2023.6.1002/skellyforge/freemocap_utils/postprocessing_widgets/menus/interpolation_menu.py` & `skellyforge-2023.7.1003/skellyforge/freemocap_utils/postprocessing_widgets/menus/interpolation_menu.py`

 * *Files identical despite different names*

### Comparing `skellyforge-2023.6.1002/skellyforge/freemocap_utils/postprocessing_widgets/menus/main_menu.py` & `skellyforge-2023.7.1003/skellyforge/freemocap_utils/postprocessing_widgets/menus/main_menu.py`

 * *Files identical despite different names*

### Comparing `skellyforge-2023.6.1002/skellyforge/freemocap_utils/postprocessing_widgets/parameter_tree_builder.py` & `skellyforge-2023.7.1003/skellyforge/freemocap_utils/postprocessing_widgets/parameter_tree_builder.py`

 * *Files identical despite different names*

### Comparing `skellyforge-2023.6.1002/skellyforge/freemocap_utils/postprocessing_widgets/parameter_widgets.py` & `skellyforge-2023.7.1003/skellyforge/freemocap_utils/postprocessing_widgets/parameter_widgets.py`

 * *Files identical despite different names*

### Comparing `skellyforge-2023.6.1002/skellyforge/freemocap_utils/postprocessing_widgets/postprocessing_functions/filter_data.py` & `skellyforge-2023.7.1003/skellyforge/freemocap_utils/postprocessing_widgets/postprocessing_functions/filter_data.py`

 * *Files identical despite different names*

### Comparing `skellyforge-2023.6.1002/skellyforge/freemocap_utils/postprocessing_widgets/postprocessing_functions/good_frame_finder.py` & `skellyforge-2023.7.1003/skellyforge/freemocap_utils/postprocessing_widgets/postprocessing_functions/good_frame_finder.py`

 * *Files identical despite different names*

### Comparing `skellyforge-2023.6.1002/skellyforge/freemocap_utils/postprocessing_widgets/postprocessing_functions/interpolate_data.py` & `skellyforge-2023.7.1003/skellyforge/freemocap_utils/postprocessing_widgets/postprocessing_functions/interpolate_data.py`

 * *Files identical despite different names*

### Comparing `skellyforge-2023.6.1002/skellyforge/freemocap_utils/postprocessing_widgets/postprocessing_functions/rotate_skeleton.py` & `skellyforge-2023.7.1003/skellyforge/freemocap_utils/postprocessing_widgets/postprocessing_functions/rotate_skeleton.py`

 * *Files identical despite different names*

### Comparing `skellyforge-2023.6.1002/skellyforge/freemocap_utils/postprocessing_widgets/task_worker_thread.py` & `skellyforge-2023.7.1003/skellyforge/freemocap_utils/postprocessing_widgets/task_worker_thread.py`

 * *Files identical despite different names*

### Comparing `skellyforge-2023.6.1002/skellyforge/freemocap_utils/postprocessing_widgets/visualization_widgets/marker_selector_widget.py` & `skellyforge-2023.7.1003/skellyforge/freemocap_utils/postprocessing_widgets/visualization_widgets/marker_selector_widget.py`

 * *Files identical despite different names*

### Comparing `skellyforge-2023.6.1002/skellyforge/freemocap_utils/postprocessing_widgets/visualization_widgets/mediapipe_skeleton_builder.py` & `skellyforge-2023.7.1003/skellyforge/freemocap_utils/postprocessing_widgets/visualization_widgets/mediapipe_skeleton_builder.py`

 * *Files identical despite different names*

### Comparing `skellyforge-2023.6.1002/skellyforge/freemocap_utils/postprocessing_widgets/visualization_widgets/skeleton_view_widget.py` & `skellyforge-2023.7.1003/skellyforge/freemocap_utils/postprocessing_widgets/visualization_widgets/skeleton_view_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
             self.ax.set_zlim([self.current_zlim[0],self.current_zlim[1]])
         else:
             self.ax.set_xlim([self.mx_skel-self.skel_3d_range, self.mx_skel+self.skel_3d_range])
             self.ax.set_ylim([self.my_skel-self.skel_3d_range, self.my_skel+self.skel_3d_range])
             self.ax.set_zlim([self.mz_skel-self.skel_3d_range, self.mz_skel+self.skel_3d_range])
         
         self.ax.set_title(self.plot_title)
-        self.fig.figure.canvas.draw_idle()
+        self.fig.figure.canvas.draw()
 
     def plot_skeleton_bones(self,frame_number):
             this_frame_skeleton_data = self.mediapipe_skeleton[frame_number]
             for connection in this_frame_skeleton_data.keys():
                 line_start_point = this_frame_skeleton_data[connection][0] 
                 line_end_point = this_frame_skeleton_data[connection][1]
```

### Comparing `skellyforge-2023.6.1002/skellyforge/freemocap_utils/postprocessing_widgets/visualization_widgets/skeleton_viewers_container.py` & `skellyforge-2023.7.1003/skellyforge/freemocap_utils/postprocessing_widgets/visualization_widgets/skeleton_viewers_container.py`

 * *Files identical despite different names*

### Comparing `skellyforge-2023.6.1002/skellyforge/freemocap_utils/postprocessing_widgets/visualization_widgets/slider_widget.py` & `skellyforge-2023.7.1003/skellyforge/freemocap_utils/postprocessing_widgets/visualization_widgets/slider_widget.py`

 * *Files identical despite different names*

### Comparing `skellyforge-2023.6.1002/skellyforge/freemocap_utils/postprocessing_widgets/visualization_widgets/timeseries_view_widget.py` & `skellyforge-2023.7.1003/skellyforge/freemocap_utils/postprocessing_widgets/visualization_widgets/timeseries_view_widget.py`

 * *Files identical despite different names*

### Comparing `skellyforge-2023.6.1002/skellyforge/headless_task_worker_test.py` & `skellyforge-2023.7.1003/skellyforge/headless_task_worker_test.py`

 * *Files identical despite different names*

### Comparing `skellyforge-2023.6.1002/skellyforge/postprocess_GUI.py` & `skellyforge-2023.7.1003/skellyforge/postprocess_GUI.py`

 * *Files identical despite different names*

### Comparing `skellyforge-2023.6.1002/PKG-INFO` & `skellyforge-2023.7.1003/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 Metadata-Version: 2.1
 Name: skellyforge
-Version: 2023.6.1002
+Version: 2023.7.1003
 Summary: Basic template of a python repository
 Keywords: basic,template,python,repository
 Author-email: skellyforge <info@freemocap.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: numpy
 Requires-Dist: pyqt6
 Requires-Dist: pyqtgraph
 Requires-Dist: scipy
 Requires-Dist: rich
 Requires-Dist: pandas
-Requires-Dist: matplotlib==3.6.3
+Requires-Dist: matplotlib
 Requires-Dist: toml
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: bumpver ; extra == "dev"
 Requires-Dist: isort ; extra == "dev"
 Requires-Dist: pip-tools ; extra == "dev"
 Requires-Dist: pytest ; extra == "dev"
 Provides-Extra: dev
 
 # postprocessing_gui
 
 # INSTALLING the GUI
  1. Create a 3.9 or 3.10 conda environment environment 
    -have tested this successfully on 3.9.16 (latest 3.9 version) and 3.10.11 (latest 3.10 version)
- 2. Navigate to this github repo and use the command `pip install -r requirements.txt` to install the dependencies
-   -Note: I pinned the matplotlib version at 3.6.3 for now because 3.7.0 and above were causing some errors to pop up with the 3D plot
+ 2. Navigate to this github repo and use the command `pip install -e.` to install the dependencies from the pyproject.toml
 
 # STARTING the GUI:
  1. Open up `postprocess_GUI.py`
  2. Scroll down to the `if __name__ == '__main__'` section at the bottom
  3. Change the `path_to_data_folder` variable to the path to your recording
    -NOTE: The GUI is set up to take file paths and file names corresponding to the 
           FreeMoCap 1.0 release. If you need to change these file paths, you can do so
```

