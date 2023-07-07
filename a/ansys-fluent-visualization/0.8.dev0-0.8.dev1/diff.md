# Comparing `tmp/ansys_fluent_visualization-0.8.dev0.tar.gz` & `tmp/ansys_fluent_visualization-0.8.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_fluent_visualization-0.8.dev0.tar", max compression
+gzip compressed data, was "ansys_fluent_visualization-0.8.dev1.tar", max compression
```

## Comparing `ansys_fluent_visualization-0.8.dev0.tar` & `ansys_fluent_visualization-0.8.dev1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1089 2023-04-19 01:17:51.197746 ansys_fluent_visualization-0.8.dev0/LICENSE
--rw-r--r--   0        0        0     5469 2023-04-19 01:17:51.197746 ansys_fluent_visualization-0.8.dev0/README.rst
--rw-r--r--   0        0        0     1316 2023-04-19 01:17:51.201746 ansys_fluent_visualization-0.8.dev0/pyproject.toml
--rw-r--r--   0        0        0     3774 2023-04-19 01:17:51.485754 ansys_fluent_visualization-0.8.dev0/src/ansys/fluent/visualization/__init__.py
--rw-r--r--   0        0        0      913 2023-04-19 01:17:51.201746 ansys_fluent_visualization-0.8.dev0/src/ansys/fluent/visualization/_config.py
--rw-r--r--   0        0        0      274 2023-04-19 01:17:51.201746 ansys_fluent_visualization-0.8.dev0/src/ansys/fluent/visualization/matplotlib/__init__.py
--rw-r--r--   0        0        0     2495 2023-04-19 01:17:51.201746 ansys_fluent_visualization-0.8.dev0/src/ansys/fluent/visualization/matplotlib/matplot_objects.py
--rw-r--r--   0        0        0    13270 2023-04-19 01:17:51.201746 ansys_fluent_visualization-0.8.dev0/src/ansys/fluent/visualization/matplotlib/matplot_windows_manager.py
--rw-r--r--   0        0        0     6935 2023-04-19 01:17:51.201746 ansys_fluent_visualization-0.8.dev0/src/ansys/fluent/visualization/matplotlib/plotter_defns.py
--rw-r--r--   0        0        0    14981 2023-04-19 01:17:51.201746 ansys_fluent_visualization-0.8.dev0/src/ansys/fluent/visualization/post_data_extractor.py
--rw-r--r--   0        0        0     4337 2023-04-19 01:17:51.201746 ansys_fluent_visualization-0.8.dev0/src/ansys/fluent/visualization/post_windows_manager.py
--rw-r--r--   0        0        0      268 2023-04-19 01:17:51.201746 ansys_fluent_visualization-0.8.dev0/src/ansys/fluent/visualization/pyvista/__init__.py
--rw-r--r--   0        0        0     6391 2023-04-19 01:17:51.205747 ansys_fluent_visualization-0.8.dev0/src/ansys/fluent/visualization/pyvista/pyvista_objects.py
--rw-r--r--   0        0        0    30842 2023-04-19 01:17:51.205747 ansys_fluent_visualization-0.8.dev0/src/ansys/fluent/visualization/pyvista/pyvista_windows_manager.py
--rw-r--r--   0        0        0     6765 1970-01-01 00:00:00.000000 ansys_fluent_visualization-0.8.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-07-07 14:45:28.112412 ansys_fluent_visualization-0.8.dev1/LICENSE
+-rw-r--r--   0        0        0     5452 2023-07-07 14:45:28.112412 ansys_fluent_visualization-0.8.dev1/README.rst
+-rw-r--r--   0        0        0     1284 2023-07-07 14:45:28.116412 ansys_fluent_visualization-0.8.dev1/pyproject.toml
+-rw-r--r--   0        0        0      748 2023-07-07 14:45:28.400413 ansys_fluent_visualization-0.8.dev1/src/ansys/fluent/visualization/__init__.py
+-rw-r--r--   0        0        0      913 2023-07-07 14:45:28.116412 ansys_fluent_visualization-0.8.dev1/src/ansys/fluent/visualization/_config.py
+-rw-r--r--   0        0        0      274 2023-07-07 14:45:28.116412 ansys_fluent_visualization-0.8.dev1/src/ansys/fluent/visualization/matplotlib/__init__.py
+-rw-r--r--   0        0        0     2495 2023-07-07 14:45:28.116412 ansys_fluent_visualization-0.8.dev1/src/ansys/fluent/visualization/matplotlib/matplot_objects.py
+-rw-r--r--   0        0        0    13269 2023-07-07 14:45:28.116412 ansys_fluent_visualization-0.8.dev1/src/ansys/fluent/visualization/matplotlib/matplot_windows_manager.py
+-rw-r--r--   0        0        0     6956 2023-07-07 14:45:28.116412 ansys_fluent_visualization-0.8.dev1/src/ansys/fluent/visualization/matplotlib/plotter_defns.py
+-rw-r--r--   0        0        0    14980 2023-07-07 14:45:28.116412 ansys_fluent_visualization-0.8.dev1/src/ansys/fluent/visualization/post_data_extractor.py
+-rw-r--r--   0        0        0     4465 2023-07-07 14:45:28.116412 ansys_fluent_visualization-0.8.dev1/src/ansys/fluent/visualization/post_windows_manager.py
+-rw-r--r--   0        0        0      268 2023-07-07 14:45:28.116412 ansys_fluent_visualization-0.8.dev1/src/ansys/fluent/visualization/pyvista/__init__.py
+-rw-r--r--   0        0        0     6391 2023-07-07 14:45:28.116412 ansys_fluent_visualization-0.8.dev1/src/ansys/fluent/visualization/pyvista/pyvista_objects.py
+-rw-r--r--   0        0        0    30983 2023-07-07 14:45:28.116412 ansys_fluent_visualization-0.8.dev1/src/ansys/fluent/visualization/pyvista/pyvista_windows_manager.py
+-rw-r--r--   0        0        0     6613 1970-01-01 00:00:00.000000 ansys_fluent_visualization-0.8.dev1/PKG-INFO
```

### Comparing `ansys_fluent_visualization-0.8.dev0/LICENSE` & `ansys_fluent_visualization-0.8.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_fluent_visualization-0.8.dev0/README.rst` & `ansys_fluent_visualization-0.8.dev1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -6,82 +6,82 @@
    :target: https://docs.pyansys.com/
    :alt: PyAnsys
 
 .. |pypi| image:: https://img.shields.io/pypi/v/ansys-fluent-visualization.svg?logo=python&logoColor=white
    :target: https://pypi.org/project/ansys-fluent-visualization
    :alt: PyPI
 
-.. |GH-CI| image:: https://github.com/pyansys/pyfluent-visualization/actions/workflows/ci_cd.yml/badge.svg
-   :target: https://github.com/pyansys/pyfluent-visualization/actions/workflows/ci_cd.yml
+.. |GH-CI| image:: https://github.com/ansys/pyfluent-visualization/actions/workflows/ci_cd.yml/badge.svg
+   :target: https://github.com/ansys/pyfluent-visualization/actions/workflows/ci_cd.yml
    :alt: GH-CI
 
 .. |MIT| image:: https://img.shields.io/badge/License-MIT-yellow.svg
    :target: https://opensource.org/licenses/MIT
    :alt: MIT
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=flat
    :target: https://github.com/psf/black
    :alt: Black
 
-.. |pre-commit| image:: https://results.pre-commit.ci/badge/github/pyansys/pyfluent-visualization/main.svg
-   :target: https://results.pre-commit.ci/latest/github/pyansys/pyfluent-visualization/main
+.. |pre-commit| image:: https://results.pre-commit.ci/badge/github/ansys/pyfluent-visualization/main.svg
+   :target: https://results.pre-commit.ci/latest/github/ansys/pyfluent-visualization/main
    :alt: pre-commit.ci status
 
 Overview
 --------
 PyFluent-Visualization provides postprocessing and visualization
-capabilities for `PyFluent <https://github.com/pyansys/pyfluent>`_
+capabilities for `PyFluent <https://github.com/ansys/pyfluent>`_
 using `PyVista <https://docs.pyvista.org/>`_ and
 `Matplotlib <https://matplotlib.org/>`_.
 
 Documentation and issues
 ------------------------
 For comprehensive information on PyFluent-Visualization, see the latest release
-`documentation <https://fluentvisualization.docs.pyansys.com>`_.
+`documentation <https://visualization.fluent.docs.pyansys.com>`_.
 
 In the upper right corner of the documentation's title bar, there is an option
 for switching from viewing the documentation for the latest stable release
 to viewing the documentation for the development version or previously
 released versions.
 
 On the `PyFluent Visualization Issues
-<https://github.com/pyansys/pyfluent-visualization/issues>`_ page, you can create
+<https://github.com/ansys/pyfluent-visualization/issues>`_ page, you can create
 issues to submit questions, reports burgs, and request new features. To reach
 the project support team, email `pyansys.core@ansys.com <pyansys.core@ansys.com>`_.
 
 Installation
 ------------
-The ``ansys-fluent-visualization`` package supports Python 3.7 through Python
-3.10 on Windows and Linux.
+The ``ansys-fluent-visualization`` package supports Python 3.8 through Python
+3.11 on Windows and Linux.
 
 If you are using Python 3.10, download and install the wheel file for the ``vtk`` package from
 `here for Windows <https://github.com/pyvista/pyvista-wheels/raw/main/vtk-9.1.0.dev0-cp310-cp310-win_amd64.whl>`_
 or from `here for Linux <https://github.com/pyvista/pyvista-wheels/raw/main/vtk-9.1.0.dev0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl>`_.
 
 Install the latest release from `PyPI
 <https://pypi.org/project/ansys-fluent-visualization/>`_ with:
 
 .. code:: console
 
    pip install ansys-fluent-visualization
 
 Alternatively, install the latest release from `GitHub
-<https://github.com/pyansys/pyfluent-visualization>`_ with:
+<https://github.com/ansys/pyfluent-visualization>`_ with:
 
 .. code:: console
 
-   pip install git+https://github.com/pyansys/pyfluent-visualization.git
+   pip install git+https://github.com/ansys/pyfluent-visualization.git
 
 
 If you plan on doing local *development* of PyFluent-Visualization with Git,
 install with:
 
 .. code:: console
 
-   git clone https://github.com/pyansys/pyfluent-visualization.git
+   git clone https://github.com/ansys/pyfluent-visualization.git
    cd pyfluent-visualization
    pip install pip -U
    pip install -e .
 
 Dependencies
 ------------
 You must have a licensed copy of Ansys Fluent installed locally.
```

### Comparing `ansys_fluent_visualization-0.8.dev0/pyproject.toml` & `ansys_fluent_visualization-0.8.dev1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 # Check https://python-poetry.org/docs/pyproject/ for all available sections
 name = "ansys-fluent-visualization"
-version = "0.8.dev0"
+version = "0.8.dev1"
 description = "A python wrapper for ansys Fluent visualization"
 license = "MIT"
 authors = ["ANSYS, Inc. <ansys.support@ansys.com>"]
 maintainers = ["PyAnsys developers <pyansys.maintainers@ansys.com>"]
 readme = "README.rst"
-repository = "https://github.com/pyansys/pyfluent-visualization"
+repository = "https://github.com/ansys/pyfluent-visualization"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 packages = [
     { include = "ansys", from = "src" },
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.7,<4.0"
+python = ">=3.8,<4.0"
 importlib-metadata = {version = "^4.0", python = "<3.8"}
-ansys-fluent-core = "~=0.13.dev0"
-vtk = {version = ">=9.0.3", python = "<=3.9"}
-pyvista = ">=0.33.2"
+ansys-fluent-core = "~=0.14.dev0"
+vtk = ">=9.2.6"
+pyvista = ">=0.39.0"
 pyvistaqt = ">=0.7.0"
 pyside6 = ">=6.2.3"
 matplotlib = ">=3.5.1"
 
 [tool.black]
 line-length = 88
```

### Comparing `ansys_fluent_visualization-0.8.dev0/src/ansys/fluent/visualization/_config.py` & `ansys_fluent_visualization-0.8.dev1/src/ansys/fluent/visualization/_config.py`

 * *Files identical despite different names*

### Comparing `ansys_fluent_visualization-0.8.dev0/src/ansys/fluent/visualization/matplotlib/matplot_objects.py` & `ansys_fluent_visualization-0.8.dev1/src/ansys/fluent/visualization/matplotlib/matplot_objects.py`

 * *Files identical despite different names*

### Comparing `ansys_fluent_visualization-0.8.dev0/src/ansys/fluent/visualization/matplotlib/matplot_windows_manager.py` & `ansys_fluent_visualization-0.8.dev1/src/ansys/fluent/visualization/matplotlib/matplot_windows_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -389,15 +389,14 @@
         return window
 
     def _get_windows_id(
         self,
         session_id: Optional[str] = "",
         windows_id: Optional[List[str]] = [],
     ) -> List[str]:
-
         return [
             window_id
             for window_id in [
                 window_id
                 for window_id, window in self._post_windows.items()
                 if not window.plotter.is_closed()
                 and (
```

### Comparing `ansys_fluent_visualization-0.8.dev0/src/ansys/fluent/visualization/matplotlib/plotter_defns.py` & `ansys_fluent_visualization-0.8.dev1/src/ansys/fluent/visualization/matplotlib/plotter_defns.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
             self._data[curve_name]["xvalues"] = []
             self._data[curve_name]["yvalues"] = []
             self.ax.plot([], [], label=curve_name)
         self.fig.canvas.manager.set_window_title("PyFluent [" + self._window_id + "]")
         plt.title(self._title)
         plt.xlabel(self._xlabel)
         plt.ylabel(self._ylabel)
-        plt.legend(loc="upper right")
+        plt.legend(labels=self._curves, loc="upper right")
 
 
 class ProcessPlotter(Plotter):
     """Class for matplotlib process plotter.
 
     Opens matplotlib window in a separate process.
     """
```

### Comparing `ansys_fluent_visualization-0.8.dev0/src/ansys/fluent/visualization/post_data_extractor.py` & `ansys_fluent_visualization-0.8.dev1/src/ansys/fluent/visualization/post_data_extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,14 @@
         except Exception as e:
             raise RuntimeError("Error while requesting data from server." + str(e))
         finally:
             obj._post_display()
         return pathlines_data
 
     def _fetch_vector_data(self, obj, *args, **kwargs):
-
         if not obj.surfaces_list():
             raise RuntimeError("Vector definition is incomplete.")
 
         obj._pre_display()
         field = obj.field()
         if not field:
             field = obj.field = "velocity-magnitude"
```

### Comparing `ansys_fluent_visualization-0.8.dev0/src/ansys/fluent/visualization/post_windows_manager.py` & `ansys_fluent_visualization-0.8.dev1/src/ansys/fluent/visualization/post_windows_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,27 +106,31 @@
         pass
 
     @abstractmethod
     def refresh_windows(
         self,
         session_id: Optional[str] = "",
         windows_id: Optional[List[str]] = [],
+        overlay: Optional[bool] = False,
     ) -> None:
         """Refresh windows.
 
         Parameters
         ----------
         session_id : str, optional
            Session id to refresh. If specified, all windows which belong to
            specified session will be refreshed. Otherwise windows for all
            sessions will be refreshed.
 
         windows_id : List[str], optional
             Windows id to refresh. If not specified, all windows will be
             refreshed.
+
+        overlay : bool, Optional
+            Overlay graphics over existing graphics.
         """
         pass
 
     @abstractmethod
     def animate_windows(
         self,
         session_id: Optional[str] = "",
```

### Comparing `ansys_fluent_visualization-0.8.dev0/src/ansys/fluent/visualization/pyvista/pyvista_objects.py` & `ansys_fluent_visualization-0.8.dev1/src/ansys/fluent/visualization/pyvista/pyvista_objects.py`

 * *Files identical despite different names*

### Comparing `ansys_fluent_visualization-0.8.dev0/src/ansys/fluent/visualization/pyvista/pyvista_windows_manager.py` & `ansys_fluent_visualization-0.8.dev1/src/ansys/fluent/visualization/pyvista/pyvista_windows_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,15 +209,15 @@
                         velocity_magnitude,
                         auto_range_off.minimum(),
                         auto_range_off.maximum(),
                     ).filled(fill_value=0)
             else:
                 auto_range_on = obj.range.auto_range_on
                 if auto_range_on.global_range():
-                    range = field_info.get_scalar_fields_range(obj.field(), False)
+                    range = field_info.get_scalar_field_range(obj.field(), False)
                 else:
                     range = [np.min(scalar_field), np.max(scalar_field)]
 
             if obj.skip():
                 vmag = np.zeros(velocity_magnitude.size)
                 vmag[:: obj.skip() + 1] = velocity_magnitude[:: obj.skip() + 1]
                 velocity_magnitude = vmag
@@ -356,15 +356,15 @@
             else:
                 auto_range_on = obj.range.auto_range_on
                 if auto_range_on.global_range():
                     if filled:
                         field_info = obj._api_helper.field_info()
                         plotter.add_mesh(
                             mesh,
-                            clim=field_info.get_scalar_fields_range(obj.field(), False),
+                            clim=field_info.get_scalar_field_range(obj.field(), False),
                             scalars=field,
                             show_edges=obj.show_edges(),
                             scalar_bar_args=scalar_bar_args,
                         )
                     if (not filled or contour_lines) and (
                         np.min(mesh[field]) != np.max(mesh[field])
                     ):
@@ -452,15 +452,14 @@
                 )
             color_size = len(self._colors.values())
             color = list(self._colors.values())[surface_id % color_size]
             plotter.add_mesh(mesh, show_edges=obj.show_edges(), color=color)
 
     def _get_refresh_for_plotter(self, window: "PyVistaWindow"):
         def refresh():
-
             with PyVistaWindowsManager._condition:
                 plotter = window.plotter
                 if window.close:
                     window.animate = False
                     plotter.close()
                     return
                 if not window.update:
@@ -625,34 +624,37 @@
             if window:
                 window.plotter.save_graphic(f"{window_id}.{format}")
 
     def refresh_windows(
         self,
         session_id: Optional[str] = "",
         windows_id: Optional[List[str]] = [],
+        overlay: Optional[bool] = False,
     ) -> None:
         """Refresh windows.
 
         Parameters
         ----------
         session_id : str, optional
            Session ID for refreshing the windows that belong only to this
            session. The default is ``""``, in which case the windows in all
            sessions are refreshed.
         windows_id : List[str], optional
             IDs of the windows to refresh. The default is ``[]``, in which case
             all windows are refreshed.
+        overlay : bool, Optional
+            Overlay graphics over existing graphics.
         """
         with self._condition:
             windows_id = self._get_windows_id(session_id, windows_id)
             for window_id in windows_id:
                 window = self._post_windows.get(window_id)
                 if window:
                     window.refresh = True
-                    self.plot(window.post_object, window.id)
+                    self.plot(window.post_object, window.id, overlay=overlay)
 
     def animate_windows(
         self,
         session_id: Optional[str] = "",
         windows_id: Optional[List[str]] = [],
     ) -> None:
         """Animate windows.
```

### Comparing `ansys_fluent_visualization-0.8.dev0/PKG-INFO` & `ansys_fluent_visualization-0.8.dev1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,118 +1,116 @@
 Metadata-Version: 2.1
 Name: ansys-fluent-visualization
-Version: 0.8.dev0
+Version: 0.8.dev1
 Summary: A python wrapper for ansys Fluent visualization
-Home-page: https://github.com/pyansys/pyfluent-visualization
+Home-page: https://github.com/ansys/pyfluent-visualization
 License: MIT
 Author: ANSYS, Inc.
 Author-email: ansys.support@ansys.com
 Maintainer: PyAnsys developers
 Maintainer-email: pyansys.maintainers@ansys.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Requires-Dist: ansys-fluent-core (>=0.13.dev0,<1.0)
+Requires-Dist: ansys-fluent-core (>=0.14.dev0,<1.0)
 Requires-Dist: importlib-metadata (>=4.0,<5.0) ; python_version < "3.8"
 Requires-Dist: matplotlib (>=3.5.1)
 Requires-Dist: pyside6 (>=6.2.3)
-Requires-Dist: pyvista (>=0.33.2)
+Requires-Dist: pyvista (>=0.39.0)
 Requires-Dist: pyvistaqt (>=0.7.0)
-Requires-Dist: vtk (>=9.0.3) ; python_full_version <= "3.9.0"
-Project-URL: Repository, https://github.com/pyansys/pyfluent-visualization
+Requires-Dist: vtk (>=9.2.6)
+Project-URL: Repository, https://github.com/ansys/pyfluent-visualization
 Description-Content-Type: text/x-rst
 
 PyFluent-Visualization
 ======================
 |pyansys| |pypi| |GH-CI| |MIT| |black| |pre-commit|
 
 .. |pyansys| image:: https://img.shields.io/badge/Py-Ansys-ffc107.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC
    :target: https://docs.pyansys.com/
    :alt: PyAnsys
 
 .. |pypi| image:: https://img.shields.io/pypi/v/ansys-fluent-visualization.svg?logo=python&logoColor=white
    :target: https://pypi.org/project/ansys-fluent-visualization
    :alt: PyPI
 
-.. |GH-CI| image:: https://github.com/pyansys/pyfluent-visualization/actions/workflows/ci_cd.yml/badge.svg
-   :target: https://github.com/pyansys/pyfluent-visualization/actions/workflows/ci_cd.yml
+.. |GH-CI| image:: https://github.com/ansys/pyfluent-visualization/actions/workflows/ci_cd.yml/badge.svg
+   :target: https://github.com/ansys/pyfluent-visualization/actions/workflows/ci_cd.yml
    :alt: GH-CI
 
 .. |MIT| image:: https://img.shields.io/badge/License-MIT-yellow.svg
    :target: https://opensource.org/licenses/MIT
    :alt: MIT
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=flat
    :target: https://github.com/psf/black
    :alt: Black
 
-.. |pre-commit| image:: https://results.pre-commit.ci/badge/github/pyansys/pyfluent-visualization/main.svg
-   :target: https://results.pre-commit.ci/latest/github/pyansys/pyfluent-visualization/main
+.. |pre-commit| image:: https://results.pre-commit.ci/badge/github/ansys/pyfluent-visualization/main.svg
+   :target: https://results.pre-commit.ci/latest/github/ansys/pyfluent-visualization/main
    :alt: pre-commit.ci status
 
 Overview
 --------
 PyFluent-Visualization provides postprocessing and visualization
-capabilities for `PyFluent <https://github.com/pyansys/pyfluent>`_
+capabilities for `PyFluent <https://github.com/ansys/pyfluent>`_
 using `PyVista <https://docs.pyvista.org/>`_ and
 `Matplotlib <https://matplotlib.org/>`_.
 
 Documentation and issues
 ------------------------
 For comprehensive information on PyFluent-Visualization, see the latest release
-`documentation <https://fluentvisualization.docs.pyansys.com>`_.
+`documentation <https://visualization.fluent.docs.pyansys.com>`_.
 
 In the upper right corner of the documentation's title bar, there is an option
 for switching from viewing the documentation for the latest stable release
 to viewing the documentation for the development version or previously
 released versions.
 
 On the `PyFluent Visualization Issues
-<https://github.com/pyansys/pyfluent-visualization/issues>`_ page, you can create
+<https://github.com/ansys/pyfluent-visualization/issues>`_ page, you can create
 issues to submit questions, reports burgs, and request new features. To reach
 the project support team, email `pyansys.core@ansys.com <pyansys.core@ansys.com>`_.
 
 Installation
 ------------
-The ``ansys-fluent-visualization`` package supports Python 3.7 through Python
-3.10 on Windows and Linux.
+The ``ansys-fluent-visualization`` package supports Python 3.8 through Python
+3.11 on Windows and Linux.
 
 If you are using Python 3.10, download and install the wheel file for the ``vtk`` package from
 `here for Windows <https://github.com/pyvista/pyvista-wheels/raw/main/vtk-9.1.0.dev0-cp310-cp310-win_amd64.whl>`_
 or from `here for Linux <https://github.com/pyvista/pyvista-wheels/raw/main/vtk-9.1.0.dev0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl>`_.
 
 Install the latest release from `PyPI
 <https://pypi.org/project/ansys-fluent-visualization/>`_ with:
 
 .. code:: console
 
    pip install ansys-fluent-visualization
 
 Alternatively, install the latest release from `GitHub
-<https://github.com/pyansys/pyfluent-visualization>`_ with:
+<https://github.com/ansys/pyfluent-visualization>`_ with:
 
 .. code:: console
 
-   pip install git+https://github.com/pyansys/pyfluent-visualization.git
+   pip install git+https://github.com/ansys/pyfluent-visualization.git
 
 
 If you plan on doing local *development* of PyFluent-Visualization with Git,
 install with:
 
 .. code:: console
 
-   git clone https://github.com/pyansys/pyfluent-visualization.git
+   git clone https://github.com/ansys/pyfluent-visualization.git
    cd pyfluent-visualization
    pip install pip -U
    pip install -e .
 
 Dependencies
 ------------
 You must have a licensed copy of Ansys Fluent installed locally.
```

