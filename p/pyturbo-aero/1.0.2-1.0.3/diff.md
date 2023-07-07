# Comparing `tmp/pyturbo_aero-1.0.2.tar.gz` & `tmp/pyturbo_aero-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyturbo_aero-1.0.2.tar", max compression
+gzip compressed data, was "pyturbo_aero-1.0.3.tar", max compression
```

## Comparing `pyturbo_aero-1.0.2.tar` & `pyturbo_aero-1.0.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0      540 2023-03-30 19:04:19.258127 pyturbo_aero-1.0.2/pyproject.toml
--rw-r--r--   0        0        0       95 2023-03-30 19:03:29.687736 pyturbo_aero-1.0.2/pyturbo/__init__.py
--rw-r--r--   0        0        0      152 2023-03-30 19:03:29.687806 pyturbo_aero-1.0.2/pyturbo/aero/__init__.py
--rw-r--r--   0        0        0    45356 2023-03-30 19:03:29.688015 pyturbo_aero-1.0.2/pyturbo/aero/airfoil2D.py
--rw-r--r--   0        0        0    67047 2023-03-30 19:03:29.688272 pyturbo_aero-1.0.2/pyturbo/aero/airfoil3D.py
--rw-r--r--   0        0        0    34367 2023-03-30 19:03:29.688393 pyturbo_aero-1.0.2/pyturbo/aero/airfoil_wavy.py
--rw-r--r--   0        0        0    18449 2023-03-30 19:03:29.688491 pyturbo_aero-1.0.2/pyturbo/aero/passage2D.py
--rw-r--r--   0        0        0      742 2023-03-30 19:03:29.688583 pyturbo_aero-1.0.2/pyturbo/helper/__init__.py
--rw-r--r--   0        0        0     2520 2023-03-30 19:03:29.688656 pyturbo_aero-1.0.2/pyturbo/helper/arc.py
--rw-r--r--   0        0        0    11163 2023-03-30 19:03:29.688752 pyturbo_aero-1.0.2/pyturbo/helper/bezier.py
--rw-r--r--   0        0        0     1295 2023-03-30 19:03:29.688806 pyturbo_aero-1.0.2/pyturbo/helper/bisect.py
--rw-r--r--   0        0        0      107 2023-03-30 19:03:29.688856 pyturbo_aero-1.0.2/pyturbo/helper/centroid.py
--rw-r--r--   0        0        0      477 2023-03-30 19:03:29.688905 pyturbo_aero-1.0.2/pyturbo/helper/convert_to_ndarray.py
--rw-r--r--   0        0        0      490 2023-03-30 19:03:29.688959 pyturbo_aero-1.0.2/pyturbo/helper/csapi.py
--rw-r--r--   0        0        0      832 2023-03-30 19:03:29.689014 pyturbo_aero-1.0.2/pyturbo/helper/derivative.py
--rw-r--r--   0        0        0      239 2023-03-30 19:03:29.689065 pyturbo_aero-1.0.2/pyturbo/helper/dist.py
--rw-r--r--   0        0        0      527 2023-03-30 19:03:29.689111 pyturbo_aero-1.0.2/pyturbo/helper/exp_ratio.py
--rw-r--r--   0        0        0     9841 2023-03-30 19:03:29.689184 pyturbo_aero-1.0.2/pyturbo/helper/line2D.py
--rw-r--r--   0        0        0     1068 2023-03-30 19:03:29.689244 pyturbo_aero-1.0.2/pyturbo/helper/min_max_check.py
--rw-r--r--   0        0        0     9654 2023-03-30 19:03:29.689323 pyturbo_aero-1.0.2/pyturbo/helper/pspline.py
--rw-r--r--   0        0        0     1543 2023-03-30 19:03:29.689380 pyturbo_aero-1.0.2/pyturbo/helper/ray.py
--rw-r--r--   0        0        0      505 2023-03-30 19:03:29.689436 pyturbo_aero-1.0.2/pyturbo/helper/rotate_array_values.py
--rw-r--r--   0        0        0      368 2023-03-30 19:03:29.689492 pyturbo_aero-1.0.2/pyturbo/helper/unique_xy.py
--rw-r--r--   0        0        0     1873 2023-03-30 19:03:29.689551 pyturbo_aero-1.0.2/pyturbo/helper/wave.py
--rw-r--r--   0        0        0      500 2023-03-30 19:03:29.689634 pyturbo_aero-1.0.2/pyturbo/ml/gramian_angular_field.py
--rw-r--r--   0        0        0    37766 2023-03-30 19:03:29.689896 pyturbo_aero-1.0.2/pyturbo/wiki/2D_design/2D_airfoil.png
--rw-r--r--   0        0        0    23891 2023-03-30 19:03:29.690060 pyturbo_aero-1.0.2/pyturbo/wiki/2D_design/Deriv_2.png
--rw-r--r--   0        0        0    25329 2023-03-30 19:03:29.690227 pyturbo_aero-1.0.2/pyturbo/wiki/2D_design/camber_line.png
--rw-r--r--   0        0        0    28623 2023-03-30 19:03:29.690397 pyturbo_aero-1.0.2/pyturbo/wiki/2D_design/s_c.png
--rw-r--r--   0        0        0    61651 2023-03-30 19:03:29.690741 pyturbo_aero-1.0.2/pyturbo/wiki/3D_design/stator3D_shell.png
--rw-r--r--   0        0        0   213435 2023-03-30 19:03:29.691753 pyturbo_aero-1.0.2/pyturbo/wiki/3D_design/stator3D_wavy_const_te_radius.PNG
--rw-r--r--   0        0        0   160990 2023-03-30 19:03:29.692142 pyturbo_aero-1.0.2/pyturbo/wiki/3D_design/stator3D_wavy_variable_te_radius.PNG
--rw-r--r--   0        0        0   146610 2023-03-30 19:03:29.692855 pyturbo_aero-1.0.2/pyturbo/wiki/3D_design/stator3D_whisker.PNG
--rw-r--r--   0        0        0   420888 2023-03-30 19:03:29.694746 pyturbo_aero-1.0.2/pyturbo/wiki/3D_design/stator_3D.png
--rw-r--r--   0        0        0    16958 2023-03-30 19:03:29.694909 pyturbo_aero-1.0.2/pyturbo/wiki/HeatPipe/circle_cross_section.png
--rw-r--r--   0        0        0    11380 2023-03-30 19:03:29.695003 pyturbo_aero-1.0.2/pyturbo/wiki/HeatPipe/pathline_close_loop_no_return.png
--rw-r--r--   0        0        0    13018 2023-03-30 19:03:29.695111 pyturbo_aero-1.0.2/pyturbo/wiki/HeatPipe/pathline_close_loop_return.png
--rw-r--r--   0        0        0    11751 2023-03-30 19:03:29.695201 pyturbo_aero-1.0.2/pyturbo/wiki/HeatPipe/pathline_periodic_loop.png
--rw-r--r--   0        0        0   164008 2023-03-30 19:03:29.695945 pyturbo_aero-1.0.2/pyturbo/wiki/HeatPipe/pattern_close_loop_no_return.PNG
--rw-r--r--   0        0        0    63687 2023-03-30 19:03:29.696266 pyturbo_aero-1.0.2/pyturbo/wiki/HeatPipe/pattern_close_loop_return.PNG
--rw-r--r--   0        0        0    59183 2023-03-30 19:03:29.696567 pyturbo_aero-1.0.2/pyturbo/wiki/HeatPipe/periodic_loop.PNG
--rw-r--r--   0        0        0    17135 2023-03-30 19:03:29.696696 pyturbo_aero-1.0.2/pyturbo/wiki/HeatPipe/rectangle_cross_section.png
--rw-r--r--   0        0        0    17732 2023-03-30 19:03:29.696828 pyturbo_aero-1.0.2/pyturbo/wiki/HeatPipe/rectangle_cross_section_fillet.png
--rw-r--r--   0        0        0      894 1970-01-01 00:00:00.000000 pyturbo_aero-1.0.2/setup.py
--rw-r--r--   0        0        0      729 1970-01-01 00:00:00.000000 pyturbo_aero-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      557 2023-07-07 19:53:58.446323 pyturbo_aero-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0       95 2023-07-05 19:18:15.890587 pyturbo_aero-1.0.3/pyturbo/__init__.py
+-rw-r--r--   0        0        0      152 2023-07-05 19:18:15.890674 pyturbo_aero-1.0.3/pyturbo/aero/__init__.py
+-rw-r--r--   0        0        0    44984 2023-07-05 19:18:15.890863 pyturbo_aero-1.0.3/pyturbo/aero/airfoil2D.py
+-rw-r--r--   0        0        0    67047 2023-07-05 19:18:15.891147 pyturbo_aero-1.0.3/pyturbo/aero/airfoil3D.py
+-rw-r--r--   0        0        0    34367 2023-07-05 19:18:15.891285 pyturbo_aero-1.0.3/pyturbo/aero/airfoil_wavy.py
+-rw-r--r--   0        0        0    18449 2023-07-05 19:18:15.891395 pyturbo_aero-1.0.3/pyturbo/aero/passage2D.py
+-rw-r--r--   0        0        0      742 2023-07-05 19:18:15.891510 pyturbo_aero-1.0.3/pyturbo/helper/__init__.py
+-rw-r--r--   0        0        0     2520 2023-07-05 19:18:15.891580 pyturbo_aero-1.0.3/pyturbo/helper/arc.py
+-rw-r--r--   0        0        0    16030 2023-07-05 19:18:15.891686 pyturbo_aero-1.0.3/pyturbo/helper/bezier.py
+-rw-r--r--   0        0        0     1295 2023-07-05 19:18:15.891760 pyturbo_aero-1.0.3/pyturbo/helper/bisect.py
+-rw-r--r--   0        0        0      107 2023-07-05 19:18:15.891818 pyturbo_aero-1.0.3/pyturbo/helper/centroid.py
+-rw-r--r--   0        0        0      477 2023-07-05 19:18:15.891878 pyturbo_aero-1.0.3/pyturbo/helper/convert_to_ndarray.py
+-rw-r--r--   0        0        0      490 2023-07-05 19:18:15.891933 pyturbo_aero-1.0.3/pyturbo/helper/csapi.py
+-rw-r--r--   0        0        0      832 2023-07-05 19:18:15.891992 pyturbo_aero-1.0.3/pyturbo/helper/derivative.py
+-rw-r--r--   0        0        0      239 2023-07-05 19:18:15.892049 pyturbo_aero-1.0.3/pyturbo/helper/dist.py
+-rw-r--r--   0        0        0      527 2023-07-05 19:18:15.892110 pyturbo_aero-1.0.3/pyturbo/helper/exp_ratio.py
+-rw-r--r--   0        0        0     9841 2023-07-05 19:18:15.892197 pyturbo_aero-1.0.3/pyturbo/helper/line2D.py
+-rw-r--r--   0        0        0     1068 2023-07-05 19:18:15.892260 pyturbo_aero-1.0.3/pyturbo/helper/min_max_check.py
+-rw-r--r--   0        0        0     9654 2023-07-05 19:18:15.892355 pyturbo_aero-1.0.3/pyturbo/helper/pspline.py
+-rw-r--r--   0        0        0     1542 2023-07-05 19:18:15.892422 pyturbo_aero-1.0.3/pyturbo/helper/ray.py
+-rw-r--r--   0        0        0      505 2023-07-05 19:18:15.892489 pyturbo_aero-1.0.3/pyturbo/helper/rotate_array_values.py
+-rw-r--r--   0        0        0      368 2023-07-05 19:18:15.892555 pyturbo_aero-1.0.3/pyturbo/helper/unique_xy.py
+-rw-r--r--   0        0        0     1873 2023-07-05 19:18:15.892618 pyturbo_aero-1.0.3/pyturbo/helper/wave.py
+-rw-r--r--   0        0        0      500 2023-07-05 19:18:15.892721 pyturbo_aero-1.0.3/pyturbo/ml/gramian_angular_field.py
+-rw-r--r--   0        0        0    37766 2023-07-05 19:18:15.893024 pyturbo_aero-1.0.3/pyturbo/wiki/2D_design/2D_airfoil.png
+-rw-r--r--   0        0        0    23891 2023-07-05 19:18:15.893201 pyturbo_aero-1.0.3/pyturbo/wiki/2D_design/Deriv_2.png
+-rw-r--r--   0        0        0    25329 2023-07-05 19:18:15.893382 pyturbo_aero-1.0.3/pyturbo/wiki/2D_design/camber_line.png
+-rw-r--r--   0        0        0    28623 2023-07-05 19:18:15.893565 pyturbo_aero-1.0.3/pyturbo/wiki/2D_design/s_c.png
+-rw-r--r--   0        0        0    61651 2023-07-05 19:18:15.893934 pyturbo_aero-1.0.3/pyturbo/wiki/3D_design/stator3D_shell.png
+-rw-r--r--   0        0        0   213435 2023-07-05 19:18:15.894939 pyturbo_aero-1.0.3/pyturbo/wiki/3D_design/stator3D_wavy_const_te_radius.PNG
+-rw-r--r--   0        0        0   160990 2023-07-05 19:18:15.895327 pyturbo_aero-1.0.3/pyturbo/wiki/3D_design/stator3D_wavy_variable_te_radius.PNG
+-rw-r--r--   0        0        0   146610 2023-07-05 19:18:15.896025 pyturbo_aero-1.0.3/pyturbo/wiki/3D_design/stator3D_whisker.PNG
+-rw-r--r--   0        0        0   420888 2023-07-05 19:18:15.897914 pyturbo_aero-1.0.3/pyturbo/wiki/3D_design/stator_3D.png
+-rw-r--r--   0        0        0    16958 2023-07-05 19:18:15.898104 pyturbo_aero-1.0.3/pyturbo/wiki/HeatPipe/circle_cross_section.png
+-rw-r--r--   0        0        0    11380 2023-07-05 19:18:15.898209 pyturbo_aero-1.0.3/pyturbo/wiki/HeatPipe/pathline_close_loop_no_return.png
+-rw-r--r--   0        0        0    13018 2023-07-05 19:18:15.898311 pyturbo_aero-1.0.3/pyturbo/wiki/HeatPipe/pathline_close_loop_return.png
+-rw-r--r--   0        0        0    11751 2023-07-05 19:18:15.898407 pyturbo_aero-1.0.3/pyturbo/wiki/HeatPipe/pathline_periodic_loop.png
+-rw-r--r--   0        0        0   164008 2023-07-05 19:18:15.899158 pyturbo_aero-1.0.3/pyturbo/wiki/HeatPipe/pattern_close_loop_no_return.PNG
+-rw-r--r--   0        0        0    63687 2023-07-05 19:18:15.899487 pyturbo_aero-1.0.3/pyturbo/wiki/HeatPipe/pattern_close_loop_return.PNG
+-rw-r--r--   0        0        0    59183 2023-07-05 19:18:15.899796 pyturbo_aero-1.0.3/pyturbo/wiki/HeatPipe/periodic_loop.PNG
+-rw-r--r--   0        0        0    17135 2023-07-05 19:18:15.899938 pyturbo_aero-1.0.3/pyturbo/wiki/HeatPipe/rectangle_cross_section.png
+-rw-r--r--   0        0        0    17732 2023-07-05 19:18:15.900074 pyturbo_aero-1.0.3/pyturbo/wiki/HeatPipe/rectangle_cross_section_fillet.png
+-rw-r--r--   0        0        0      908 1970-01-01 00:00:00.000000 pyturbo_aero-1.0.3/setup.py
+-rw-r--r--   0        0        0      754 1970-01-01 00:00:00.000000 pyturbo_aero-1.0.3/PKG-INFO
```

### Comparing `pyturbo_aero-1.0.2/pyproject.toml` & `pyturbo_aero-1.0.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 [tool.poetry]
-name = "pyturbo_aero"
-version = "1.0.2"
+name = "pyturbo-aero"
+version = "1.0.3"
 description = "PyTurbo_Aero is a Turbomachinery blade design library that lets you create a full 3D blades and passages."
 authors = ["Paht Juangphanich <paht.juangphanich@nasa.gov>"]
 packages = [
     { include = "pyturbo" }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7"
 plotly = "*"
 tqdm = "*"
 scipy = ">1.8.0"
 pandas = ">=1.4"
 numpy = ">1.23.1"
 matplotlib = ">3.2.1"
+numpy-stl = "*"
+
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry>=1.1.2"]
 build-backend = "poetry.masonry.api"
```

### Comparing `pyturbo_aero-1.0.2/pyturbo/aero/airfoil2D.py` & `pyturbo_aero-1.0.3/pyturbo/aero/airfoil2D.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,16 +270,15 @@
         yo = y_wedge_ss-m*(x_wedge_ss-xo)
         # mc = (yo-y_wedge_ss)/(xo-x_wedge_ss) # Check
         self.ssBezierX[-2] = xo
         self.ssBezierY[-2] = yo
         self.ssBezierX[-1] = x_wedge_ss
         self.ssBezierY[-1] = y_wedge_ss
         b = bezier(self.ssBezierX,self.ssBezierY)
-        self.ssBezier = b
-        
+        self.ssBezier = b      
     
     def ss_thickness_add(self,thicknessArray:List[float],camberPercent:float=None,thickness_loc:List[float]=None,expansion_ratio:float=1.2):
         """Adds thickness to the suction side by specifying bezier control points 
 
         Args:
             thicknessArray (List[float]): thickness along the suction side. Example: [0.2400, 0.2000, 0.1600, 0.1400]
             camberPercent (float, optional): Percent camber where straightening of the suction side happens. Defaults to None.
@@ -394,15 +393,14 @@
                 xn = x+cos(radians(theta))*t_ray
                 yn = y+sin(radians(theta))*t_ray
                 self.psBezierX.append(xn)
                 self.psBezierY.append(yn)
             
         self.psBezier = bezier(self.psBezierX,self.psBezierY)
 
-
     def add_pitch(self,x_pitch:float):
         """Adds extra pitch by shifting the turbine blade over by a x direction
 
         Args:
             x_pitch (float): [description]
         """
         # Pitch_Add Adds pitch or shifts turbine by x direction
@@ -444,15 +442,14 @@
             self.ssBezier = bezier(self.ssBezierX,self.ssBezierY)
 
         self.TE_ps_arc.x = self.TE_ps_arc.x + x
         self.TE_ps_arc.y = self.TE_ps_arc.y + y
         self.TE_ss_arc.x = self.TE_ss_arc.x + x
         self.TE_ss_arc.y = self.TE_ss_arc.y + y
 
-
     def get_centroid(self):
         """Returns the centroid of the airfoil
 
         Returns:
             float,float: centroid x and y coordinates (x,y)
         """
         n = 100
@@ -638,15 +635,14 @@
         
         ## Initialize piecewise bezier
         self.ssBezierX = np.array([self.ssBezierX[1:indx_d-1], x]) # Modify the bezier points to include an intersection point
         self.ssBezierY = np.array([self.ssBezierY[1:indx_d-1], y])
         bs = bezier(self.ssBezierX,self.ssBezierY)
         self.ssBezier = pw_bezier2D([bs,bl])
     
-
     # FlowGuidance2
     # Use if SS is defined from 0 to a camber percent
     def flow_guidance2(self,n:int=8):
         """This function straightens out the suction side by specifying n bezier control points instead of a straight line. 
 
         Args:.
             n (int): number of control points, increase this to make straightening more aggressive. Defaults to 8.
@@ -668,15 +664,14 @@
         # ssBezierX,ssBezierY -> define new ssBezier
         [x, y] = bl.get_point(np.linspace(0,1,n))
         self.ssBezierX = np.append(self.ssBezierX[0:-2],x)
         self.ssBezierY = np.append(self.ssBezierY[0:-2],y)
 
         self.ssBezier = bezier(self.ssBezierX,self.ssBezierY)
 
- 
     def flow_guidance3(self,s_c:float,n:int):
         """Straightens out the suction side. Computes the intersection point of the throat and draws a line, adds bezier points along the line
 
         Args:
             s_c (float): pitch-to-chord ratio
             n (int): number of bezier control points
         """
@@ -915,16 +910,14 @@
         plt.ylim(ylim)
         handles, labels = plt.gca().get_legend_handles_labels()
         plt.legend(handles, ['d^2y/dx^2 suction side','d^2y/dx^2 pressure side'])
         plt.xlabel('s(x)/s')
         plt.ylabel('d^2y/dx^2')
         plt.show()
 
-
-
     def thickness(self):
         """Calculates the location and value of maximum thickness along with average thickness
 
         Returns:
             int: along camberline of max thickness
             float: max thickness
             float: average thickness
@@ -950,26 +943,14 @@
                         
         # Find max thickness
         [max_thickness,indx] = max(d) # gives value and index
         
         # Find avg thickness
         avg_thickness = np.mean(d)
         return indx, max_thickness, avg_thickness
-        # Find avg thickness
-        
-        # Debug plot
-    #             close all
-    #             self.Plot2D[0]
-    #             figure(1)
-    #             hold on
-    #             for i=1:len(t)
-    #                 plot([xss(i) xx_ps(i)],[yss(i) yy_ps(i)],'k')
-    #             end
-    #             hold off
-    #             [val indx] = max(d)
 
     def channel_get(self,s_c):        
         """Gets adjacent airfoil 
 
         Args:
             s_c (float): pitch to chord ratio
```

### Comparing `pyturbo_aero-1.0.2/pyturbo/aero/airfoil3D.py` & `pyturbo_aero-1.0.3/pyturbo/aero/airfoil3D.py`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.2/pyturbo/aero/airfoil_wavy.py` & `pyturbo_aero-1.0.3/pyturbo/aero/airfoil_wavy.py`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.2/pyturbo/aero/passage2D.py` & `pyturbo_aero-1.0.3/pyturbo/aero/passage2D.py`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.2/pyturbo/helper/__init__.py` & `pyturbo_aero-1.0.3/pyturbo/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.2/pyturbo/helper/arc.py` & `pyturbo_aero-1.0.3/pyturbo/helper/arc.py`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.2/pyturbo/helper/bezier.py` & `pyturbo_aero-1.0.3/pyturbo/helper/bezier.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List
+from typing import List, Optional, Union
 import numpy as np
 from scipy.special import comb
 import scipy.interpolate as sp_intp
 from scipy.optimize import minimize_scalar 
 import matplotlib.pyplot as plt
 import matplotlib as mpl
 import math 
@@ -11,22 +11,26 @@
 from .convert_to_ndarray import convert_to_ndarray
 
 # https://www.journaldev.com/14893/python-property-decorator
 # https://www.codementor.io/sheena/advanced-use-python-decorators-class-function-du107nxsv
 # https://stackabuse.com/pythons-classmethod-and-staticmethod-explained/
 
 class bezier():
+    n:int           # Number of control points
+    c:np.ndarray    # bezier coefficients
+    x:np.ndarray    # x-control points
+    y:np.ndarray    # y-control points
+
+
     def __init__(self, x,y):
         self.n = len(x)
         self.c = np.zeros(self.n) 
-        self.x = x
-        self.y = y
-        self.dx = x[-1]-x[0]
-        self.dy = y[-1]-y[0]
-        self.t = []
+        self.x = convert_to_ndarray(x)
+        self.y = convert_to_ndarray(y)
+
         for i in range(0,self.n):
             self.c[i] = comb(self.n-1, i, exact=False) # use floating point
 
     def flip(self):
         '''
             Reverses the direction of the bezier curve
             returns:
@@ -35,30 +39,27 @@
         return bezier(np.flip(self.x),np.flip(self.y))
 
     @property
     def get_x_y(self):
         return self.x,self.y
     
     def get_curve_length(self):
-        """
-            Get a point or points along a bezier curve
-            Inputs:
-                t - scalar, list, or numpy array
-                equal_space - try to space points equally 
-            Outputs: 
-                Bx, By - scalar or numpy array
+        """Gets the curve length
+
+        Returns:
+            float: curve length
         """
         [x,y] = self.get_point(np.linspace(0,1,100))
         d = np.zeros((len(x),1))
         for i in range(0,len(x)-1):
             d[i] = math.sqrt((x[i+1]-x[i])**2 + (y[i+1]-y[i])**2)
         
         return sum(d) # Linear approximation of curve length
 
-    def equal_space(self,t:np.ndarray,x,y):
+    def __equal_space__(self,t:np.ndarray,x,y):
         """
             Equally space points along a bezier curve using arc length
             Inputs 
         """
         arcL = arclen(x,y)
         mean_old = np.mean(arcL)
         mean_err = 1
@@ -96,24 +97,20 @@
             tempx,tempy = 0.0, 0.0
             for j in range(0,self.n):
                 u = self.c[j]*pow(1-t[i], self.n-j-1)*pow(t[i],j)
                 tempx += u*self.x[j]
                 tempy += u*self.y[j]
                 
             Bx[i],By[i] = tempx,tempy
-        self.t = t
 
         if (equal_space and len(Bx)>2):
             Bx,By = self.equal_space(t,Bx,By)
             return Bx,By
-        elif (len(Bx)==1):
-            return Bx[0], By[0] # if it's just one point return floats
         return Bx,By
 
-
     def plot2D(self,equal_space=False):
         """Creates a 2D Plot of a bezier curve 
 
         Args:            
             equal_space (bool, optional): Equally spaces the points using arc length. Defaults to False.
             figure_num (int, optional): if you want plots to be on the same figure. Defaults to None.
         """
@@ -124,16 +121,14 @@
         plt.plot(x, y,'-b')
         plt.plot(self.x, self.y,'or')
 
         plt.xlabel("x-label")
         plt.ylabel("y-label")
         plt.axis('scaled')
 
-        
-
     def get_point_dt(self,t):
         """
          Gets the derivative
         """
         if type(t) is not np.ndarray:
             t = np.array([t],dtype=float) # the brackets [] are really helpful. scalars have to be converted to array before passing
         tmin = np.min(t)
@@ -158,29 +153,86 @@
                 tempx = tempx*(self.n-1)
                 tempy = tempy*(self.n-1)
             
             Bx[i] = tempx
             By[i] = tempy
         return Bx,By
 
+    def rotate(self,angle:float):
+        """Rotate 
+
+        Args:
+            angle (float): _description_
+        """
+        angle = np.radians(angle)
+        rot_matrix = np.array([[math.cos(angle) -math.sin(angle)],[math.sin(angle), math.cos(angle)]])
+        ans = (rot_matrix*self.x.transpose()).transpose()
+        self.x = ans[:,0]
+        self.y = ans[:,1]
+
+
 class bezier3:
     def __init__(self,x,y,z):
         self.n = len(x)
-        self.x = x
-        self.y = y
-        self.z = z
+        self.x = convert_to_ndarray(x)
+        self.y = convert_to_ndarray(y)
+        self.z = convert_to_ndarray(z)
         self.c = np.zeros(self.n)
         for i in range(self.n):
             self.c[i] = comb(self.n-1, i, exact=False) # use floating point
     
-    def get_point(self,t,equal_space = True):
+    def __equal_space__(self,t:np.ndarray,x:np.ndarray,y:np.ndarray,z:np.ndarray):
+        """Equally space points along a bezier curve using arc length
+            
+        Args:
+            t (np.ndarray): position along bezier curve. Example: t = np.linspace(0,1,100)
+            x (np.ndarray): x-coordinate as numpy array
+            y (np.ndarray): y-coordinates as numpy array
+            z (np.ndarray): z-coordinates as numpy array
+
+        Returns:
+            (Tuple): containing
+                - *x* (np.ndarray): new values of x that are equally spaced 
+                - *y* (np.ndarray): new values of y that are equally spaced 
+
         """
-            Gets the x,y,z coordinate at a particular time instance 
-            Inputs:
-                t - 0 to 1
+        arcL = arclen3(x,y,z)
+        mean_old = np.mean(arcL)
+        mean_err = 1
+        while (mean_err>1.0E-3):
+            target_len = np.sum(arcL)/len(t) # we want equal length
+            csum = np.cumsum(arcL)
+            f = sp_intp.PchipInterpolator(t,csum)
+            t_start = np.min(t)   
+            t_end = np.max(t)
+            for i in range(0,t.size-2):
+                f2 = lambda x: abs(f(x)-f(t_start)-target_len)
+                temp = minimize_scalar(f2,bounds=(t_start,t_end),method="bounded",tol=1e-6)
+                t[i+1] = temp.x
+                t_start = t[i+1]
+
+            x,y,z = self.get_point(t,equal_space=False)
+            arcL = arclen3(x,y,z)
+            mean_new = np.mean(arcL)
+            mean_err = abs(mean_old-mean_new)/abs(mean_new)
+            mean_old = mean_new
+        return x,y,z
+    
+    def get_point(self,t,equal_space = True):
+        """Gets the point(s) at a certain percentage along the piecewise bezier curve
+
+        Args:
+            t (Union[List[float],float,np.ndarray]): percentage(s) along a bezier curve. You can specify a float, List[float], or a numpy array
+            equal_space (bool, optional): Equally space points using arc length. Defaults to False.
+
+        Returns:
+            (Tuple): containing
+                - *x* (np.ndarray): x-coordinates
+                - *y* (np.ndarray): y-coordinates
+                
         """
 
         t = convert_to_ndarray(t)
         Bx,By,Bz = np.zeros(t.size),np.zeros(t.size),np.zeros(t.size)
         for i in range(len(t)):
             tempx,tempy,tempz = 0.0, 0.0, 0.0
             for j in range(0,self.n):
@@ -189,23 +241,31 @@
                 tempy += u*self.y[j]
                 tempz += u*self.z[j]
 
             Bx[i],By[i],Bz[i] = tempx,tempy,tempz
         self.t = t
 
         if (equal_space and len(Bx)>2):
-            Bx,By,Bz = equal_space(t,Bx,By,Bz)
+            Bx,By,Bz = self.__equal_space__(t,Bx,By,Bz)
             return Bx,By,Bz
         elif (len(Bx)==1):
             return Bx[0], By[0],Bz[0] # if it's just one point return floats
         return Bx,By,Bz
     
-    def get_point_dt(self,t):
-        """
-         Gets the derivative
+    def get_point_dt(self,t:Union[float,List[float],np.ndarray]):
+        """Returns the derivative at a particular percentage 
+
+        Args:
+            t (Union[float,List[float],np.ndarray]): Percentage from 0 to 1
+
+        Returns:
+            (Tuple): containing
+                - *dx* (np.ndarray): dx_dt
+                - *dy* (np.ndarray): dy_dt
+                - *dz* (np.ndarray): dz_dt
         """
         t = convert_to_ndarray(t)
 
         tmin = np.min(t)
         tmax = np.max(t)
             
         Bx = np.zeros((len(t),1))
@@ -248,17 +308,20 @@
 @time_this
 def func_a(stuff):
     import time
     time.sleep(3)
 
 class pw_bezier2D:
     def __init__(self,array:List[bezier]):
-        '''
-            Initializes the piecewise bezier curve from an array of bezier curves
-        '''
+        """Initializes the piecewise bezier curve from an array of bezier curves
+
+        Args:
+            array (List[bezier]): Bezier curves as an array
+        """
+        
         self.bezierArray = array
     
         x = np.zeros(len(self.bezierArray)+1)
         y = np.zeros(len(self.bezierArray)+1)
         dist = np.zeros(len(self.bezierArray))
         tArray = np.zeros(len(self.bezierArray))
         x[0] = self.bezierArray[0].x[0]
@@ -273,34 +336,90 @@
         for i in range(len(dist)):
             tArray[i]=np.sum(dist[0:i])/dmax
         
         self.tArray =tArray
         self.dist=dist
         self.dmax = dmax
 
-    def get_point(self,t):
-        t = convert_to_ndarray(t)
+    def get_point(self,t:Union[List[float],float,np.ndarray],equal_space:bool=False):
+        """Gets the point(s) at a certain percentage along the piecewise bezier curve
 
-        t.sort();  
-        n = len(self.bezierArray); 
-        x = np.zeros(int(len(t)*n-n))
-        y = np.zeros(int(len(t)*n-n))
+        Args:
+            t (Union[List[float],float,np.ndarray]): percentage(s) along a bezier curve. You can specify a float, List[float], or a numpy array
+            equal_space (bool, optional): Equally space points using arc length. Defaults to False.
+
+        Returns:
+            (Tuple): containing
+                - *x* (np.ndarray): x-coordinates
+                - *y* (np.ndarray): y-coordinates
+
+        """
+        n = len(self.bezierArray)
+        t = convert_to_ndarray(t) 
+        x = np.zeros(len(t)+(n-1)*(len(t)-1))
+        y = np.zeros(len(t)+(n-1)*(len(t)-1))
         t_start=0; lenT = len(t)
-
         for i in range(0,n): # loop for each bezier curve
             [xx,yy] = self.bezierArray[i].get_point(t)
-            if (i<n):
-                x[t_start:t_start+lenT-1] = xx[0:-1]
-                y[t_start:t_start+lenT-1] = yy[0:-1]
-                t_start = t_start+lenT-1
+            if i == 0:
+                x[0:lenT] = xx
+                y[0:lenT] = yy
+                t_start += lenT
             else:
-                x[t_start:] = xx
-                y[t_start:] = yy
+                x[t_start:t_start+lenT-1] = xx[1:]
+                y[t_start:t_start+lenT-1] = yy[1:]
+                t_start += lenT-1
+            
+
+        if len(t)>0:
+            t = np.linspace(0,1,len(x))
+            x = sp_intp.interp1d(t,x)(np.linspace(0,1,lenT))
+            y = sp_intp.interp1d(t,y)(np.linspace(0,1,lenT))
+            return x,y
+
+        if (equal_space and len(x)>2):
+            x,y = self.__equal_space__(t,x,y)
         return x,y
 
+    def __equal_space__(self,t:np.ndarray,x:np.ndarray,y:np.ndarray):
+        """Equally space points along a bezier curve using arc length
+            
+        Args:
+            t (np.ndarray): position along bezier curve. Example: t = np.linspace(0,1,100)
+            x (np.ndarray): x-coordinate as numpy array
+            y (np.ndarray): y-coordinates as numpy array
+
+        Returns:
+            (Tuple): containing
+                - *x* (np.ndarray): new values of x that are equally spaced 
+                - *y* (np.ndarray): new values of y that are equally spaced 
+
+        """
+        arcL = arclen(x,y)
+        mean_old = np.mean(arcL)
+        mean_err = 1
+        while (mean_err>1.0E-3):
+            target_len = np.sum(arcL)/len(t) # we want equal length
+            csum = np.cumsum(arcL)
+            f = sp_intp.PchipInterpolator(t,csum)
+            t_start = np.min(t)   
+            t_end = np.max(t)
+            for i in range(0,t.size-2):
+                f2 = lambda x: abs(f(x)-f(t_start)-target_len)
+                temp = minimize_scalar(f2,bounds=(t_start,t_end),method="bounded",tol=1e-6)
+                t[i+1] = temp.x
+                t_start = t[i+1]
+
+            x,y = self.get_point(t,equal_space=False)
+            arcL = arclen(x,y)
+            mean_new = np.mean(arcL)
+            mean_err = abs(mean_old-mean_new)/abs(mean_new)
+            mean_old = mean_new
+        return x,y
+    
     def get_dt(self,t):
         t = convert_to_ndarray(t)
         t = t.sort(); js = 1; tadj = 0
         dx = np.zeros((len(t),1))
         dy = np.zeros((len(t),1))
         for i in range(0,len(t)):
             for j in range(js,len(self.tArray)):
```

### Comparing `pyturbo_aero-1.0.2/pyturbo/helper/bisect.py` & `pyturbo_aero-1.0.3/pyturbo/helper/bisect.py`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.2/pyturbo/helper/derivative.py` & `pyturbo_aero-1.0.3/pyturbo/helper/derivative.py`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.2/pyturbo/helper/exp_ratio.py` & `pyturbo_aero-1.0.3/pyturbo/helper/exp_ratio.py`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.2/pyturbo/helper/line2D.py` & `pyturbo_aero-1.0.3/pyturbo/helper/line2D.py`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.2/pyturbo/helper/min_max_check.py` & `pyturbo_aero-1.0.3/pyturbo/helper/min_max_check.py`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.2/pyturbo/helper/pspline.py` & `pyturbo_aero-1.0.3/pyturbo/helper/pspline.py`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.2/pyturbo/helper/ray.py` & `pyturbo_aero-1.0.3/pyturbo/helper/ray.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     def plot(self,t):
         fig = plt.figure()
         ax = plt.axes(projection='3d')
 
         [x,y] = self.get_point(t)
         plt.figure()
         plt.plot(x,y)
-        plot.draw()
+        plt.draw()
         plt.show()
 
 def ray2D_intersection(ray1,ray2):
     A =np.array([[ray1.dx, -ray2.dx],[ray1.dy, -ray2.dy]])
     b = np.array([[ray2.x-ray1.x], [ray2.y-ray1.y]])
 
     T = np.linalg.solve(A,b)
```

### Comparing `pyturbo_aero-1.0.2/pyturbo/helper/wave.py` & `pyturbo_aero-1.0.3/pyturbo/helper/wave.py`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.2/pyturbo/wiki/2D_design/2D_airfoil.png` & `pyturbo_aero-1.0.3/pyturbo/wiki/2D_design/2D_airfoil.png`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.2/pyturbo/wiki/2D_design/Deriv_2.png` & `pyturbo_aero-1.0.3/pyturbo/wiki/2D_design/Deriv_2.png`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.2/pyturbo/wiki/2D_design/camber_line.png` & `pyturbo_aero-1.0.3/pyturbo/wiki/2D_design/camber_line.png`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.2/pyturbo/wiki/2D_design/s_c.png` & `pyturbo_aero-1.0.3/pyturbo/wiki/2D_design/s_c.png`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.2/pyturbo/wiki/3D_design/stator3D_shell.png` & `pyturbo_aero-1.0.3/pyturbo/wiki/3D_design/stator3D_shell.png`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.2/pyturbo/wiki/3D_design/stator3D_wavy_const_te_radius.PNG` & `pyturbo_aero-1.0.3/pyturbo/wiki/3D_design/stator3D_wavy_const_te_radius.PNG`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.2/pyturbo/wiki/3D_design/stator3D_wavy_variable_te_radius.PNG` & `pyturbo_aero-1.0.3/pyturbo/wiki/3D_design/stator3D_wavy_variable_te_radius.PNG`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.2/pyturbo/wiki/3D_design/stator3D_whisker.PNG` & `pyturbo_aero-1.0.3/pyturbo/wiki/3D_design/stator3D_whisker.PNG`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.2/pyturbo/wiki/3D_design/stator_3D.png` & `pyturbo_aero-1.0.3/pyturbo/wiki/3D_design/stator_3D.png`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.2/pyturbo/wiki/HeatPipe/circle_cross_section.png` & `pyturbo_aero-1.0.3/pyturbo/wiki/HeatPipe/circle_cross_section.png`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.2/pyturbo/wiki/HeatPipe/pathline_close_loop_no_return.png` & `pyturbo_aero-1.0.3/pyturbo/wiki/HeatPipe/pathline_close_loop_no_return.png`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.2/pyturbo/wiki/HeatPipe/pathline_close_loop_return.png` & `pyturbo_aero-1.0.3/pyturbo/wiki/HeatPipe/pathline_close_loop_return.png`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.2/pyturbo/wiki/HeatPipe/pathline_periodic_loop.png` & `pyturbo_aero-1.0.3/pyturbo/wiki/HeatPipe/pathline_periodic_loop.png`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.2/pyturbo/wiki/HeatPipe/pattern_close_loop_no_return.PNG` & `pyturbo_aero-1.0.3/pyturbo/wiki/HeatPipe/pattern_close_loop_no_return.PNG`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.2/pyturbo/wiki/HeatPipe/pattern_close_loop_return.PNG` & `pyturbo_aero-1.0.3/pyturbo/wiki/HeatPipe/pattern_close_loop_return.PNG`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.2/pyturbo/wiki/HeatPipe/periodic_loop.PNG` & `pyturbo_aero-1.0.3/pyturbo/wiki/HeatPipe/periodic_loop.PNG`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.2/pyturbo/wiki/HeatPipe/rectangle_cross_section.png` & `pyturbo_aero-1.0.3/pyturbo/wiki/HeatPipe/rectangle_cross_section.png`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.2/pyturbo/wiki/HeatPipe/rectangle_cross_section_fillet.png` & `pyturbo_aero-1.0.3/pyturbo/wiki/HeatPipe/rectangle_cross_section_fillet.png`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.2/setup.py` & `pyturbo_aero-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,24 @@
 
 package_data = \
 {'': ['*'],
  'pyturbo': ['wiki/2D_design/*', 'wiki/3D_design/*', 'wiki/HeatPipe/*']}
 
 install_requires = \
 ['matplotlib>3.2.1',
+ 'numpy-stl',
  'numpy>1.23.1',
  'pandas>=1.4',
  'plotly',
  'scipy>1.8.0',
  'tqdm']
 
 setup_kwargs = {
     'name': 'pyturbo-aero',
-    'version': '1.0.2',
+    'version': '1.0.3',
     'description': 'PyTurbo_Aero is a Turbomachinery blade design library that lets you create a full 3D blades and passages.',
     'long_description': 'None',
     'author': 'Paht Juangphanich',
     'author_email': 'paht.juangphanich@nasa.gov',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pyturbo_aero-1.0.2/PKG-INFO` & `pyturbo_aero-1.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: pyturbo-aero
-Version: 1.0.2
+Version: 1.0.3
 Summary: PyTurbo_Aero is a Turbomachinery blade design library that lets you create a full 3D blades and passages.
 Author: Paht Juangphanich
 Author-email: paht.juangphanich@nasa.gov
 Requires-Python: >=3.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: matplotlib (>3.2.1)
 Requires-Dist: numpy (>1.23.1)
+Requires-Dist: numpy-stl
 Requires-Dist: pandas (>=1.4)
 Requires-Dist: plotly
 Requires-Dist: scipy (>1.8.0)
 Requires-Dist: tqdm
```

