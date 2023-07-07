# Comparing `tmp/fenics-smart-2.1.2.tar.gz` & `tmp/fenics-smart-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenics-smart-2.1.2.tar", last modified: Thu Jun 29 08:58:48 2023, max compression
+gzip compressed data, was "fenics-smart-2.1.3.tar", last modified: Fri Jul  7 20:20:12 2023, max compression
```

## Comparing `fenics-smart-2.1.2.tar` & `fenics-smart-2.1.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:48.386085 fenics-smart-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-06-29 08:58:15.000000 fenics-smart-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16773 2023-06-29 08:58:48.386085 fenics-smart-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8248 2023-06-29 08:58:15.000000 fenics-smart-2.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:48.382085 fenics-smart-2.1.2/fenics_smart.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16773 2023-06-29 08:58:48.000000 fenics-smart-2.1.2/fenics_smart.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-29 08:58:48.000000 fenics-smart-2.1.2/fenics_smart.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 08:58:48.000000 fenics-smart-2.1.2/fenics_smart.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-29 08:58:48.000000 fenics-smart-2.1.2/fenics_smart.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 08:58:48.000000 fenics-smart-2.1.2/fenics_smart.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-06-29 08:58:15.000000 fenics-smart-2.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 08:58:48.386085 fenics-smart-2.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:48.382085 fenics-smart-2.1.2/smart/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-29 08:58:15.000000 fenics-smart-2.1.2/smart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-06-29 08:58:15.000000 fenics-smart-2.1.2/smart/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-06-29 08:58:15.000000 fenics-smart-2.1.2/smart/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-29 08:58:15.000000 fenics-smart-2.1.2/smart/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16272 2023-06-29 08:58:15.000000 fenics-smart-2.1.2/smart/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    27558 2023-06-29 08:58:15.000000 fenics-smart-2.1.2/smart/mesh_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    89606 2023-06-29 08:58:15.000000 fenics-smart-2.1.2/smart/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    63943 2023-06-29 08:58:15.000000 fenics-smart-2.1.2/smart/model_assembly.py
--rw-r--r--   0 runner    (1001) docker     (123)    20870 2023-06-29 08:58:15.000000 fenics-smart-2.1.2/smart/solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-29 08:58:15.000000 fenics-smart-2.1.2/smart/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-29 08:58:15.000000 fenics-smart-2.1.2/smart/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-06-29 08:58:15.000000 fenics-smart-2.1.2/smart/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:48.382085 fenics-smart-2.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-29 08:58:15.000000 fenics-smart-2.1.2/tests/test_compartment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-06-29 08:58:15.000000 fenics-smart-2.1.2/tests/test_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-06-29 08:58:15.000000 fenics-smart-2.1.2/tests/test_species.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:20:12.065427 fenics-smart-2.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-07-07 20:19:54.000000 fenics-smart-2.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16773 2023-07-07 20:20:12.065427 fenics-smart-2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8248 2023-07-07 20:19:54.000000 fenics-smart-2.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:20:12.061427 fenics-smart-2.1.3/fenics_smart.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16773 2023-07-07 20:20:12.000000 fenics-smart-2.1.3/fenics_smart.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-07 20:20:12.000000 fenics-smart-2.1.3/fenics_smart.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 20:20:12.000000 fenics-smart-2.1.3/fenics_smart.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-07 20:20:12.000000 fenics-smart-2.1.3/fenics_smart.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-07 20:20:12.000000 fenics-smart-2.1.3/fenics_smart.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-07-07 20:19:54.000000 fenics-smart-2.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 20:20:12.065427 fenics-smart-2.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:20:12.065427 fenics-smart-2.1.3/smart/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-07 20:19:54.000000 fenics-smart-2.1.3/smart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-07-07 20:19:54.000000 fenics-smart-2.1.3/smart/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11745 2023-07-07 20:19:54.000000 fenics-smart-2.1.3/smart/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-07 20:19:54.000000 fenics-smart-2.1.3/smart/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16278 2023-07-07 20:19:54.000000 fenics-smart-2.1.3/smart/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27643 2023-07-07 20:19:54.000000 fenics-smart-2.1.3/smart/mesh_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89606 2023-07-07 20:19:54.000000 fenics-smart-2.1.3/smart/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64165 2023-07-07 20:19:54.000000 fenics-smart-2.1.3/smart/model_assembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20870 2023-07-07 20:19:54.000000 fenics-smart-2.1.3/smart/solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-07 20:19:54.000000 fenics-smart-2.1.3/smart/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-07 20:19:54.000000 fenics-smart-2.1.3/smart/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11394 2023-07-07 20:19:54.000000 fenics-smart-2.1.3/smart/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:20:12.065427 fenics-smart-2.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-07 20:19:54.000000 fenics-smart-2.1.3/tests/test_compartment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-07-07 20:19:54.000000 fenics-smart-2.1.3/tests/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-07-07 20:19:54.000000 fenics-smart-2.1.3/tests/test_species.py
```

### Comparing `fenics-smart-2.1.2/LICENSE` & `fenics-smart-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fenics-smart-2.1.2/PKG-INFO` & `fenics-smart-2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenics-smart
-Version: 2.1.2
+Version: 2.1.3
 Summary: Spatial Modeling Algorithms for Reactions and Transport (SMART) is a high-performance finite-element-based simulation package for model specification and numerical simulation of spatially-varying reaction-transport processes in biological cells.
 Author-email: Justin Laughlin <justinglaughlin@gmail.com>
 License: GNU LESSER GENERAL PUBLIC LICENSE
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fenics-smart-2.1.2/README.md` & `fenics-smart-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `fenics-smart-2.1.2/fenics_smart.egg-info/PKG-INFO` & `fenics-smart-2.1.3/fenics_smart.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenics-smart
-Version: 2.1.2
+Version: 2.1.3
 Summary: Spatial Modeling Algorithms for Reactions and Transport (SMART) is a high-performance finite-element-based simulation package for model specification and numerical simulation of spatially-varying reaction-transport processes in biological cells.
 Author-email: Justin Laughlin <justinglaughlin@gmail.com>
 License: GNU LESSER GENERAL PUBLIC LICENSE
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fenics-smart-2.1.2/pyproject.toml` & `fenics-smart-2.1.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system] # Require setuptool version due to https://github.com/pypa/setuptools/issues/2938
 requires = ["setuptools>=61.0.0", "wheel"]
 
 [project]
 name = "fenics-smart"
-version = "2.1.2"
+version = "2.1.3"
 description = "Spatial Modeling Algorithms for Reactions and Transport (SMART) is a high-performance finite-element-based simulation package for model specification and numerical simulation of spatially-varying reaction-transport processes in biological cells."
 authors = [{name = "Justin Laughlin", email = "justinglaughlin@gmail.com"}]
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
     "numpy>=1.16.0",
@@ -49,19 +49,18 @@
 ]
 pyvista = [
     "pyvista==0.38.4",
     "panel"
 ]
 
 all = [
-   "smart[examples]",
-   "smart[test]",
-   "smart[docs]",
-   "smart[dev]",
-   "smart[pyvista]"
+   "fenics-smart[examples]",
+   "fenics-smart[test]",
+   "fenics-smart[docs]",
+   "fenics-smart[pyvista]"
 ]
 
 
 [tool.pytest.ini_options]
 addopts = [
    "--cov=smart",
    "--cov-report=html",
```

### Comparing `fenics-smart-2.1.2/smart/common.py` & `fenics-smart-2.1.3/smart/common.py`

 * *Files identical despite different names*

### Comparing `fenics-smart-2.1.2/smart/config.py` & `fenics-smart-2.1.3/smart/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -339,15 +339,15 @@
     Args:
         final_t: End time of simulation
         use_snes: Use PETScSNES solver if true, else use DOLFINs NewtonSolver
         snes_preassemble_linear_system: If True separate linear components during assembly
         initial_dt: Initial time-stepping
         adjust_dt: A tuple (t, dt) of floats indicating when to next adjust the
             time-stepping and to what value
-        dt: Number of digits for rounding `dt`
+        adjust_dt: Number of digits for rounding `dt`
         print_assembly: Print information during assembly process
         dt_decrease_factor:
         dt_increase_factor:
         attempt_timestep_restart_on_divergence: Restart snes solver if it diverges
         reset_timestep_for_negative_solution: Reduce solver timestep is solution is negative
     """
```

### Comparing `fenics-smart-2.1.2/smart/deprecation.py` & `fenics-smart-2.1.3/smart/deprecation.py`

 * *Files identical despite different names*

### Comparing `fenics-smart-2.1.2/smart/mesh.py` & `fenics-smart-2.1.3/smart/mesh.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,19 +138,19 @@
 
 class ParentMesh(_Mesh):
     """
     Mesh loaded in from data. Submeshes are extracted from the ParentMesh based
     on marker values from the .hdf5 or .xml file.
 
     Args:
-    * mesh_filename (str): Name of mesh file
-    * mesh_filetype (str): Extension of mesh, either 'xml' or 'hdf5'
-    * parent_mesh (str): Name of mesh
-    * use_partition (bool): If `hdf5` mesh file is loaded,
-            choose if mesh should be read in with its current partition
+        mesh_filename (str): Name of mesh file
+        mesh_filetype (str): Extension of mesh, either 'xml' or 'hdf5'
+        parent_mesh (str): Name of mesh
+        use_partition (bool): If `hdf5` mesh file is loaded,
+          choose if mesh should be read in with its current partition
     """
 
     mesh_filename: str
     mesh_filetype: str
     child_meshes: Dict[str, "ChildMesh"]
     parent_mesh: "ParentMesh"
     use_partition: bool
```

### Comparing `fenics-smart-2.1.2/smart/mesh_tools.py` & `fenics-smart-2.1.3/smart/mesh_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -652,17 +652,19 @@
 def write_mesh(
     mesh: d.Mesh,
     mf_facet: d.MeshFunction,
     mf_cell: d.MeshFunction,
     filename: pathlib.Path = pathlib.Path("DemoMesh.h5"),
 ):
     """
-    Write 3D mesh, with cell markers (mf3)
-    and facet markers (mf2) to hdf5 file and pvd files.
+    Write 3D mesh, with cell markers (mf_cell)
+    and facet markers (mf_facet) to hdf5 file and pvd files.
     """
+    if isinstance(filename, str):
+        filename = pathlib.Path(filename)
     comm = mesh.mpi_comm()
     # extract dimensionality for meshfunctions
     cell_dim = mf_cell.dim()
     facet_dim = mf_facet.dim()
     # Write mesh and meshfunctions to file
     hdf5 = d.HDF5File(comm, str(filename.with_suffix(".h5")), "w")
     hdf5.write(mesh, "/mesh")
```

### Comparing `fenics-smart-2.1.2/smart/model.py` & `fenics-smart-2.1.3/smart/model.py`

 * *Files identical despite different names*

### Comparing `fenics-smart-2.1.2/smart/model_assembly.py` & `fenics-smart-2.1.3/smart/model_assembly.py`

 * *Files 1% similar despite different names*

```diff
@@ -437,18 +437,18 @@
     """
     Parameter objects contain information for the various parameters involved in reactions,
     such as binding rates and dissociation constants.
     A Parameter object that is constant over time and space is initialized by calling
 
     .. code:: python
 
-    param_var = Parameter(
-        name, value, unit, group (opt), notes (opt),
-        use_preintegration (opt)
-        )
+        param_var = Parameter(
+            name, value, unit, group (opt), notes (opt),
+            use_preintegration (opt)
+            )
 
     Args:
         name: string naming the parameter
         value: value of the given parameter
         unit: units associated with given value
         group (optional): string placing this parameter in a designated group;
              for organizational purposes when there are multiple reaction modules
@@ -891,14 +891,20 @@
     @property
     def latex_name(self):
         # Change _ to - in name
         name = self.name.replace("_", "-")
         self._latex_name = sym.latex(Symbol(name))
         return self._latex_name
 
+    @property
+    def sol(self):
+        if not hasattr(self, "u") or "u" not in self.u:
+            raise RuntimeError("Solution does not exist. Please run a simulation first")
+        return self.u["u"]
+
 
 class CompartmentContainer(ObjectContainer):
     def __init__(self):
         super().__init__(Compartment)
 
         self.properties_to_print = [
             "_mesh_id",
```

### Comparing `fenics-smart-2.1.2/smart/solvers.py` & `fenics-smart-2.1.3/smart/solvers.py`

 * *Files identical despite different names*

### Comparing `fenics-smart-2.1.2/smart/units.py` & `fenics-smart-2.1.3/smart/units.py`

 * *Files identical despite different names*

### Comparing `fenics-smart-2.1.2/smart/utils.py` & `fenics-smart-2.1.3/smart/utils.py`

 * *Files identical despite different names*

### Comparing `fenics-smart-2.1.2/smart/visualization.py` & `fenics-smart-2.1.3/smart/visualization.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 from typing import Tuple
 import numpy.typing as npt
 import numpy as np
 import functools
 import pathlib
 from typing import Optional
 import warnings
+import logging
+
+logger = logging.getLogger(__name__)
 
 __all__ = ["create_vtk_structures", "plot"]
 
 _vtk_perm = {
     dolfin.interval: {i: np.arange(i) for i in range(2, 10)},
     vertex: {1: 1},
     dolfin.triangle: {
@@ -110,26 +113,34 @@
 def plot(
     uh: dolfin.Function,
     filename: Optional[pathlib.Path] = None,
     show_edges: bool = True,
     glyph_factor: float = 1,
     off_screen: bool = True,
     view_xy: bool = False,
-):
+    clip_plane: Tuple[float, float, float] = (1, 0, 0),
+    clip_origin: Tuple[float, float, float] = (0, 0, 0),
+    clip_logic: bool = True,
+    clim: Tuple[float, float] = (0, 0),
+) -> Optional[np.ndarray]:
     """
     Plot a (discontinuous) Lagrange function with Pyvista
 
     Args:
         uh: The function
         filename: If set, writes the plot to file instead of displaying it interactively
         show_edges: Show mesh edges if ``True``
         glyph_factor: Scaling of glyphs if input function is a function from a
             ``dolfin.VectorFunctionSpace``.
         off_screen: If ``True`` generate plots with virtual frame buffer using ``xvfb``.
         view_xy: If ``True``, view xy plane
+        clip_plane: plane for clipping 3D object, specified as the normal vector
+        clip_origin: origin for clipping 3D object
+        clip_logic: If ``True``, clip 3D object
+        clim: Tuple specifying (lower_lim, upper_lim) for display of uh
     """
     Vh = uh.function_space()
 
     dofmap = Vh.dofmap()
     num_vertices_local = dofmap.index_map().size(dofmap.index_map().MapSize.ALL)
     bs = 1 if Vh.num_sub_spaces() == 0 else Vh.num_sub_spaces()
 
@@ -157,48 +168,71 @@
     degree = Vh.ufl_element().degree()
     if degree > 1 and show_edges:
         first_order_el = Vh.ufl_element().reconstruct(degree=1)
         P1 = dolfin.FunctionSpace(Vh.mesh(), first_order_el)
         t1, c1, x1 = create_vtk_structures(P1)
         p1_grid = pyvista.UnstructuredGrid(t1, c1, x1)
         if bs > 1:
-            plotter.add_mesh(p1_grid, show_edges=show_edges)
+            if not clim == (0, 0):
+                plotter.add_mesh(p1_grid, show_edges=show_edges, clim=clim)
+            else:
+                plotter.add_mesh(p1_grid, show_edges=show_edges)
         else:
-            plotter.add_mesh(grid)
-            plotter.add_mesh(p1_grid, style="wireframe")
+            if not clim == (0, 0):
+                plotter.add_mesh(grid, clim=clim)
+                plotter.add_mesh(p1_grid, style="wireframe", clim=clim)
+            else:
+                plotter.add_mesh(grid)
+                plotter.add_mesh(p1_grid, style="wireframe")
     else:
-        if uh.geometric_dimension() == 2 or view_xy:
-            plotter.add_mesh(grid, show_edges=show_edges)
+        if uh.geometric_dimension() == 2 or view_xy or not clip_logic:
+            if not clim == (0, 0):
+                plotter.add_mesh(grid, show_edges=show_edges, clim=clim)
+            else:
+                plotter.add_mesh(grid, show_edges=show_edges)
         else:
-            crinkled = grid.clip(normal=(1, 0, 0), crinkle=True)
-            plotter.add_mesh(crinkled, show_edges=show_edges)
+            try:
+                crinkled = grid.clip(normal=clip_plane, origin=clip_origin, crinkle=True)
+                if not clim == (0, 0):
+                    plotter.add_mesh(crinkled, show_edges=show_edges, clim=clim)
+                else:
+                    plotter.add_mesh(crinkled, show_edges=show_edges)
+            except KeyError:
+                raise RuntimeError(
+                    "Pyvista clipping removed the entire mesh, "
+                    "either change clip_origin accordingly "
+                    "or set clip_logic to False"
+                )
 
     if uh.geometric_dimension() == 2 or view_xy:
         plotter.view_xy()
 
     if bs > 1:
         glyphs = grid.glyph(orient=uh.name(), factor=glyph_factor)
         plotter.add_mesh(glyphs)
-    print(filename)
     if filename is None:
         plotter.show()
     else:
-        plotter.screenshot(filename)
+        logger.debug(f"Saving plot to {filename}")
+        return plotter.screenshot(filename, return_img=True)
 
 
 @require_pyvista
 def plot_dolfin_mesh(
     msh: dolfin.mesh,
     mf_cell: dolfin.MeshFunction,
     mf_facet: dolfin.MeshFunction = None,
     outer_marker: int = 10,
     filename: Optional[pathlib.Path] = None,
     show_edges: bool = True,
     off_screen: bool = True,
     view_xy: bool = False,
+    clip_plane: Tuple[float, float, float] = (1, 0, 0),
+    clip_origin: Tuple[float, float, float] = (0, 0, 0),
+    clip_logic: bool = True,
 ):
     """
     Construct P1 function space on current mesh,
     convert function space to vtk structures,
     and then plot mesh markers in mf (a dolfin MeshFunction)
 
     Args:
@@ -209,14 +243,17 @@
         outer_marker (optional): value marking the boundary facets in mf_facet.
             Number of nodes with this marker
             should match the number of nodes in dolfin.BoundaryMesh(msh, "exterior")
         filename: If set, writes the plot to file instead of displaying it interactively
         show_edges: Show mesh edges if ``True``
         off_screen: If ``True`` generate plots with virtual frame buffer using ``xvfb``.
         view_xy: If ``True``, view xy plane
+        clip_plane: plane for clipping 3D object, specified as the normal vector
+        clip_origin: origin for clipping 3D object
+        clip_logic: If ``True``, clip 3D object
     """
     Vh = dolfin.FunctionSpace(msh, "P", 1)
     u_out = mf_cell.array()
     topology, cell_types, x = create_vtk_structures(Vh)
 
     import pyvista
 
@@ -249,21 +286,30 @@
         first_order_el = Vh.ufl_element().reconstruct(degree=1)
         P1 = dolfin.FunctionSpace(Vh.mesh(), first_order_el)
         t1, c1, x1 = create_vtk_structures(P1)
         p1_grid = pyvista.UnstructuredGrid(t1, c1, x1)
         plotter.add_mesh(grid)
         plotter.add_mesh(p1_grid, style="wireframe")
     else:
-        if msh.topology().dim() == 3:
-            crinkled = grid.clip(normal=(1, 0, 0), crinkle=True)
-            plotter.add_mesh(crinkled, show_edges=show_edges)
-            if facets_loaded:
-                crinkled_facet = grid_facet.clip(normal=(1, 0, 0), crinkle=True)
-                plotter.add_mesh(crinkled_facet, show_edges=show_edges)
-        elif msh.topology().dim() == 2:
+        if msh.topology().dim() == 3 and clip_logic:
+            try:
+                crinkled = grid.clip(normal=clip_plane, origin=clip_origin, crinkle=True)
+                plotter.add_mesh(crinkled, show_edges=show_edges)
+                if facets_loaded:
+                    crinkled_facet = grid_facet.clip(
+                        normal=clip_plane, origin=clip_origin, crinkle=True
+                    )
+                    plotter.add_mesh(crinkled_facet, show_edges=show_edges)
+            except KeyError:
+                raise RuntimeError(
+                    "Pyvista clipping removed the entire mesh, "
+                    "either change clip_origin accordingly "
+                    "or set clip_logic to False"
+                )
+        else:
             plotter.add_mesh(grid, show_edges=show_edges)
             if facets_loaded:
                 plotter.add_mesh(grid_facet, show_edges=show_edges)
 
     if msh.geometric_dimension() == 2 or view_xy:
         plotter.view_xy()
```

### Comparing `fenics-smart-2.1.2/tests/test_compartment.py` & `fenics-smart-2.1.3/tests/test_compartment.py`

 * *Files identical despite different names*

### Comparing `fenics-smart-2.1.2/tests/test_parameter.py` & `fenics-smart-2.1.3/tests/test_parameter.py`

 * *Files identical despite different names*

### Comparing `fenics-smart-2.1.2/tests/test_species.py` & `fenics-smart-2.1.3/tests/test_species.py`

 * *Files identical despite different names*

