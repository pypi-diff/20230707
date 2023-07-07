# Comparing `tmp/nmrformd-0.1.0.tar.gz` & `tmp/nmrformd-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmrformd-0.1.0.tar", last modified: Sat Jul 23 15:31:46 2022, max compression
+gzip compressed data, was "nmrformd-0.1.1.tar", last modified: Fri Jul  7 13:58:08 2023, max compression
```

## Comparing `nmrformd-0.1.0.tar` & `nmrformd-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 sgravelle  (1198) icp      (10000)        0 2022-07-23 15:31:46.426149 nmrformd-0.1.0/
--rw-r--r--   0 sgravelle  (1198) icp      (10000)     4025 2022-07-23 15:31:46.427158 nmrformd-0.1.0/PKG-INFO
--rw-r--r--   0 sgravelle  (1198) icp      (10000)     2801 2022-07-23 15:25:06.000000 nmrformd-0.1.0/README.rst
-drwxr-xr-x   0 sgravelle  (1198) icp      (10000)        0 2022-07-23 15:31:46.388149 nmrformd-0.1.0/nmrformd/
--rw-r--r--   0 sgravelle  (1198) icp      (10000)    16728 2022-07-23 13:52:22.000000 nmrformd-0.1.0/nmrformd/NMR.py
--rw-r--r--   0 sgravelle  (1198) icp      (10000)      317 2022-07-09 15:54:50.000000 nmrformd-0.1.0/nmrformd/__init__.py
--rw-r--r--   0 sgravelle  (1198) icp      (10000)     1697 2022-07-11 06:39:34.000000 nmrformd-0.1.0/nmrformd/utilities.py
-drwxr-xr-x   0 sgravelle  (1198) icp      (10000)        0 2022-07-23 15:31:46.414157 nmrformd-0.1.0/nmrformd.egg-info/
--rw-r--r--   0 sgravelle  (1198) icp      (10000)     4025 2022-07-23 15:31:46.000000 nmrformd-0.1.0/nmrformd.egg-info/PKG-INFO
--rw-r--r--   0 sgravelle  (1198) icp      (10000)      278 2022-07-23 15:31:46.000000 nmrformd-0.1.0/nmrformd.egg-info/SOURCES.txt
--rw-r--r--   0 sgravelle  (1198) icp      (10000)        1 2022-07-23 15:31:46.000000 nmrformd-0.1.0/nmrformd.egg-info/dependency_links.txt
--rw-r--r--   0 sgravelle  (1198) icp      (10000)        1 2022-07-09 15:23:09.000000 nmrformd-0.1.0/nmrformd.egg-info/not-zip-safe
--rw-r--r--   0 sgravelle  (1198) icp      (10000)       30 2022-07-23 15:31:46.000000 nmrformd-0.1.0/nmrformd.egg-info/requires.txt
--rw-r--r--   0 sgravelle  (1198) icp      (10000)        9 2022-07-23 15:31:46.000000 nmrformd-0.1.0/nmrformd.egg-info/top_level.txt
--rw-r--r--   0 sgravelle  (1198) icp      (10000)       80 2022-07-23 15:31:46.430162 nmrformd-0.1.0/setup.cfg
--rw-r--r--   0 sgravelle  (1198) icp      (10000)     1043 2022-07-23 15:31:03.000000 nmrformd-0.1.0/setup.py
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-07-07 13:58:08.140949 nmrformd-0.1.1/
+-rw-rw-r--   0 simon     (1000) simon     (1000)    35149 2023-06-30 09:27:53.000000 nmrformd-0.1.1/LICENSE.txt
+-rw-rw-r--   0 simon     (1000) simon     (1000)      748 2023-07-07 13:58:08.140949 nmrformd-0.1.1/PKG-INFO
+-rw-rw-r--   0 simon     (1000) simon     (1000)     4805 2023-07-07 13:49:12.000000 nmrformd-0.1.1/README.rst
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-07-07 13:58:08.140949 nmrformd-0.1.1/nmrformd/
+-rw-rw-r--   0 simon     (1000) simon     (1000)    14272 2023-07-05 08:23:34.000000 nmrformd-0.1.1/nmrformd/NMR.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)      317 2023-06-30 09:27:53.000000 nmrformd-0.1.1/nmrformd/__init__.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     2969 2023-07-06 13:38:45.000000 nmrformd-0.1.1/nmrformd/utilities.py
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-07-07 13:58:08.140949 nmrformd-0.1.1/nmrformd.egg-info/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      748 2023-07-07 13:58:08.000000 nmrformd-0.1.1/nmrformd.egg-info/PKG-INFO
+-rw-rw-r--   0 simon     (1000) simon     (1000)      290 2023-07-07 13:58:08.000000 nmrformd-0.1.1/nmrformd.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon     (1000) simon     (1000)        1 2023-07-07 13:58:08.000000 nmrformd-0.1.1/nmrformd.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon     (1000) simon     (1000)        1 2023-06-30 09:46:37.000000 nmrformd-0.1.1/nmrformd.egg-info/not-zip-safe
+-rw-rw-r--   0 simon     (1000) simon     (1000)       30 2023-07-07 13:58:08.000000 nmrformd-0.1.1/nmrformd.egg-info/requires.txt
+-rw-rw-r--   0 simon     (1000) simon     (1000)        9 2023-07-07 13:58:08.000000 nmrformd-0.1.1/nmrformd.egg-info/top_level.txt
+-rw-rw-r--   0 simon     (1000) simon     (1000)       80 2023-07-07 13:58:08.140949 nmrformd-0.1.1/setup.cfg
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1059 2023-07-07 13:54:09.000000 nmrformd-0.1.1/setup.py
```

### Comparing `nmrformd-0.1.0/nmrformd/NMR.py` & `nmrformd-0.1.1/nmrformd/NMR.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,394 +1,341 @@
 #!/usr/bin/env python3
 """Main file for NMRforMD package."""
 # -*- Mode: python; tab-width: 4; indent-tabs-mode:nil; coding:utf-8 -*-
 #
-# Copyright (c) 2022 Authors and contributors
+# Copyright (c) 2023 Authors and contributors
 # Simon Gravelle
 #
 # Released under the GNU Public Licence, v3 or any higher version
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import random
 
 import MDAnalysis.core.groups
 import numpy as np
 from scipy import constants as cst
 from scipy.interpolate import interp1d
 from scipy.special import sph_harm
-from MDAnalysis.analysis.distances import distance_array
 
-from .utilities import correlation_function, find_nearest, fourier_transform
+from .utilities import autocorrelation_function, find_nearest, fourier_transform
 
 
 class NMR:
     """Calculate NMR relaxation time from MDAnalysis universe.
 
     Parameters
     ----------
     u : MDAnalysis.Universe
         MDAnalysis universe containing all the information describing
         the molecular dynamics system.
-    atom_group : [MDAnalysis.AtomGroup, MDAnalysis.AtomGroup]
-        Target and Neighbor groups, respectively.
+    atom_group : MDAnalysis.AtomGroup
+        Target atom groups for NMR calculation.
+    neighbor_group : MDAnalysis.AtomGroup
+        Neighbor atom groups. If not specified, atom_group is used.
     type_analysis : str, default ``full``
         Type of analysis, which can be ``full``, ``intra_molecular``,
         or ``inter_molecular``.
     number_i : int, default 0
         Number of atom of the target group to consider for the calculation.
         If ``number_i = 0``, all atoms are considered.
-    order : str, default ``m0``
-        Order of the analysis, which can be ``m0`` or ``m012``.
-        With ``m0``, only the spherical harmonic of order 0 is considered, 
-        this is only valid for isotropic systems. For nonisotropic systems,
-        use ``m012``.
+    isotropic : bool, default ``True``
+        If isotropic is true, only the spherical harmonic of order 0 is considered, 
+        which is usually valid for bulk systems. For non-isotropic systems,
+        use ``False``.
     f0 : int, default ``None``
         Frequency at which ``T1`` and ``T2`` are calculated.
         If ``None``, ``f = 0`` is used.
     actual_dt : float, default ``None``
         Can be used to specify a different time interface between frames than the 
         one detected by MDAnalysis.
     hydrogen_per_atom : float, default 1.0
         Specify the number of hydrogen per atom, usefull for 
         coarse-grained simulations.
-    start : int, default 0
-        To specify the first frame to be considered for the analysis.
-    stop : int, default 0
-        To specify the last frame to be considered for the analysis.
-    step : int, default 1
-        To jump frame during the analysis.  
     pdb : bool, default True
         To turn off/on the periodic boundary condition treatment.            
     """
 
     def __init__(self,
                  u: MDAnalysis.Universe,
                  atom_group: MDAnalysis.AtomGroup,
+                 neighbor_group: MDAnalysis.AtomGroup = None,
                  type_analysis: str = "full",
-                 number_i: int =0,
-                 order: str ="m0",
-                 f0: float =None,
-                 actual_dt: float =None,
-                 hydrogen_per_atom: float =1.0,
-                 spin: float =1/2,
-                 start: int = 0,
-                 stop: int = 0,
-                 step: int = 1,
+                 number_i: int = 0,
+                 isotropic: bool = True,
+                 f0: float = None,
+                 actual_dt: float = None,
+                 hydrogen_per_atom: float = 1.0,
+                 spin: float = 1/2,
                  pbc: bool = True
                  ):
-        """Initialise class NMR.
-        """
-
+        
+        """Initialise class NMR."""
         self.u = u
-        if len(atom_group) == 0:
-            raise ValueError("Missing atom group")
-        elif len(atom_group) == 1:
-            self.target_i = atom_group[0]
-            self.neighbor_j = atom_group[0]
-        elif len(atom_group) == 2:
-            self.target_i = atom_group[0]
-            self.neighbor_j = atom_group[1]
-        elif len(atom_group) >= 3:
-            raise ValueError("More than 2 atom groups")
+        self.target_i = atom_group
+        if neighbor_group is None:
+            self.neighbor_j = atom_group
+        else:
+            self.neighbor_j = neighbor_group
         self.type_analysis = type_analysis
         self.number_i = number_i
-        self.order = order
+        self.f0 = f0
+        self.isotropic = isotropic
+        if self.isotropic:
+            self.dim = 1
+        else:
+            self.dim = 3
         self.actual_dt = actual_dt
         self.hydrogen_per_atom = hydrogen_per_atom
         self.spin = spin
-        self.start = start
-        if stop == 0:
-            self.stop = u.trajectory.n_frames
-        else:
-            self.stop = stop
-        self.step = step
         self.pbc = pbc
         self.data = None
         self.rij = None
         self.r = None
         self.theta = None
         self.phi = None
-        self.sh20 = None
-        self.sh21 = None
-        self.sh22 = None
         self.gij = None
         self.T1 = None
         self.T2 = None
-        self.tau = None
-        self.delta_omega = None
 
-        self._verify_entry()
-        self._define_constants()
-        self._read_universe()
-        self._select_target_i()
-
-        # Loop on all the atom of group i
-        for _cpt_i, _ in enumerate(self.index_i):
-            self._cpt_i = _cpt_i
-            #self.atom_index_i = atom_index_i # not used
-            self._select_atoms_group_i()
-            self._select_atoms_group_j()
-            if _cpt_i == 0:
-                self._initialise_data()
-            self._evaluate_correlation_ij()
-
-        self._calculate_fourier_transform()
-        self._calculate_spectrum()
-        self.f0 = f0
-        self._calculate_relaxationtime()
-        self._calculate_tau()
-        self._calculate_secondmoment()
-
-    def _verify_entry(self):
-        """Verify that entries are correct."""
-        _possible_analysis = ["inter_molecular", "intra_molecular", "full"]
-        if self.type_analysis not in _possible_analysis:
-            raise ValueError("type_analysis can only be inter_molecular, intra_molecular, and full.")
-        _possible_order = ["m0", "m012"]
-        if self.order not in _possible_order:
-            raise ValueError("order can only be m0 and m012.")
+        self.initialize()
+        self.collect_data()
+        self.finalize()
+
+    def initialize(self):
+        """Prepare the calculation"""
+        self.verify_entry()
+        self.define_constants()
+        self.select_target_i()
+
+    def verify_entry(self):
+        """Verify that entries are correct, and that groups are not empty."""
+        possible_analysis = ["inter_molecular", "intra_molecular", "full"]
+        if self.type_analysis not in possible_analysis:
+            raise ValueError("type_analysis can only be inter_molecular, intra_molecular, and full.")      
+        if self.target_i.n_atoms == 0:
+            raise ValueError("Empty atom group")
+        if self.neighbor_j.n_atoms == 0:
+            raise ValueError("Empty neighbor atom group")
 
-    def _define_constants(self):
-        """Define the pre-factor K.
+    def define_constants(self):
+        """Define prefactors.
 
-        Gamma is the gyromagnetic constant in Hz/T, and
+        See this page for details : https://nmrformd.readthedocs.io
+        Gamma is the gyromagnetic constant of 1H in Hz/T or C/kg
         K has the units of m^6/s^2
-        # @tocheck the units
-        # @tofix do atoms have all the same gyromag ratio?
+        alpha_m are normalizing coefficient for harmonic function
         """
-        self._GAMMA = 2 * np.pi * 42.6e6
-        self._K = (3 / 2) * (cst.mu_0 / 4 / np.pi) ** 2 \
-            * cst.hbar ** 2 * self._GAMMA ** 4 * self.spin * (1 + self.spin)
-
-    def _read_universe(self):
-        """Create atom groups from chosen atom selections.
-
-        The created groups must not be empty.
+        self.GAMMA = 2 * np.pi * 42.6e6
+        self.K = (3 / 2) * (cst.mu_0 / 4 / np.pi) ** 2 \
+            * cst.hbar ** 2 * self.GAMMA ** 4 * self.spin * (1 + self.spin)
+        self.alpha_m = [np.sqrt(16 * np.pi / 5),
+                        np.sqrt(8 * np.pi / 15),
+                        np.sqrt(32 * np.pi / 15)]
+
+    def select_target_i(self):
+        """Select the target atoms i
+        
+        If number_i=0, select all atoms in target_i
+        If number_i > target_i.atoms.n_atoms, raise message
+        Else, if 0<number_i<target_i.atoms.n_atoms, select atoms randomly
         """
-        self.group_target_i = self.u.select_atoms(self.target_i)
-        self.group_neighbor_j = self.u.select_atoms(self.neighbor_j)
-        # Assert that both groups contain atoms
-        if self.group_target_i.atoms.n_atoms == 0:
-            raise ValueError("Empty atom groups i")
-        elif self.group_neighbor_j.atoms.n_atoms == 0:
-            raise ValueError("Empty atom groups j")
-
-    def _select_target_i(self):
         if self.number_i == 0:
-            self.index_i = np.array(self.group_target_i.atoms.indices)
-        elif self.number_i > self.group_target_i.atoms.n_atoms:
+            self.index_i = np.array(self.target_i.atoms.indices)
+        elif self.number_i > self.target_i.atoms.n_atoms:
             print('Note : number_i is larger than the number of atoms in group target i\n'
+                  '-> The number_i value will be ignored'
                   '-> All the atoms of the group i have been selected')
-            self.index_i = np.array(self.group_target_i.atoms.indices)
+            self.index_i = np.array(self.target_i.atoms.indices)
         else:
-            self.index_i = np.array(random.choices(self.group_target_i.atoms.indices, k=self.number_i))
-    def _select_atoms_group_i(self):
+            self.index_i = np.array(random.choices(self.target_i.atoms.indices, k=self.number_i))
+
+    def collect_data(self):
+        """Collect data by looping over atoms, time, and evaluate correlation"""
+        # Loop on all the atom of group i
+        for cpt_i, _ in enumerate(self.index_i):
+            self.cpt_i = cpt_i
+            #self.atom_index_i = atom_index_i # not used
+            self.select_atoms_group_i()
+            self.select_atoms_group_j()
+            if cpt_i == 0:
+                self.initialise_data()
+            self.loop_over_trajectory()
+            self.calculate_correlation_ij()
+
+    def select_atoms_group_i(self):
         """Select atoms of the group i for the calculation."""
-        self.group_i = self.u.select_atoms('index ' + str(self.index_i[self._cpt_i]))
-        self._resids_i = self.group_i.resids[self.group_i.atoms.indices == self.index_i[self._cpt_i]]
+        self.group_i = self.u.select_atoms('index ' + str(self.index_i[self.cpt_i]))
+        self.resids_i = self.group_i.resids[self.group_i.atoms.indices == self.index_i[self.cpt_i]]
 
-    def _select_atoms_group_j(self):
+    def select_atoms_group_j(self):
         """Select atoms of the group j for the calculation.
 
         For intra molecular analysis, group j are made of atoms of the
         same residue as group i.
         For inter molecular analysis, group j are made of atoms of
         different residues as group i.
         For full analysis, group j are made of atoms that are not in group i.
         """
         if self.type_analysis == "intra_molecular":
-            _same_residue : bool = self.group_neighbor_j.resids == self._resids_i
-            _different_atom : bool = self.group_neighbor_j.indices != self.index_i[self._cpt_i]
-            _index_j = self.group_neighbor_j.atoms.indices[_same_residue & _different_atom]
-            _str_j = ' '.join(str(e) for e in _index_j)
+            same_residue : bool = self.neighbor_j.resids == self.resids_i
+            different_atom : bool = self.neighbor_j.indices != self.index_i[self.cpt_i]
+            index_j = self.neighbor_j.atoms.indices[same_residue & different_atom]
+            str_j = ' '.join(str(e) for e in index_j)
         elif self.type_analysis == "inter_molecular":
-            _different_residue : bool = self.group_neighbor_j.resids != self._resids_i
-            _index_j = self.group_neighbor_j.atoms.indices[_different_residue]
-            _str_j = ' '.join(str(e) for e in _index_j)
+            different_residue : bool = self.neighbor_j.resids != self.resids_i
+            index_j = self.neighbor_j.atoms.indices[different_residue]
+            str_j = ' '.join(str(e) for e in index_j)
         elif self.type_analysis == "full":
-            _different_atom : bool = self.group_neighbor_j.indices != self.index_i[self._cpt_i]
-            _index_j = self.group_neighbor_j.atoms.indices[_different_atom]
-            _str_j = ' '.join(str(e) for e in _index_j)
-        if len(_str_j) == 0:
+            different_atom : bool = self.neighbor_j.indices != self.index_i[self.cpt_i]
+            index_j = self.neighbor_j.atoms.indices[different_atom]
+            str_j = ' '.join(str(e) for e in index_j)
+        if len(str_j) == 0:
             raise ValueError("Empty atom groups j \n"
                              "Wrong combination of type_analysis and group selection?")
         else:
-            self.group_j = self.u.select_atoms('index ' + _str_j)
+            self.group_j = self.u.select_atoms('index ' + str_j)
 
-    def _initialise_data(self):
-        """Initialise data arrays.
+    def initialise_data(self):
+        """Initialise arrays.
 
-        # @tofix if step>1, matrix will be too large
-        # either adapt or cut it before calculating correlation
-        """
-        if self.order == "m0":
-            self._data = np.zeros((1, self.u.trajectory.n_frames,
-                                  self.group_j.atoms.n_atoms),
-                                  dtype=np.float32)
-            self.gij = np.zeros((1,  self.u.trajectory.n_frames),
-                                 dtype=np.float32)
-        elif self.order == "m012":
-            self._data = np.zeros((3, self.u.trajectory.n_frames,
-                                  self.group_j.atoms.n_atoms),
-                                  dtype=np.complex64)
-            self.gij = np.zeros((3, self.u.trajectory.n_frames),
+        Create an array of zeros for the data and the correlation function.
+        If anisotropic, the spherical harmonic may be complex, so dtype=complex64
+        is used.
+        Create an array for of values separated by timestep for the time. 
+        """
+        if self.isotropic:
+            self.data = np.zeros((self.dim, self.u.trajectory.n_frames,
+                                    self.group_j.atoms.n_atoms),
+                                    dtype=np.float16)
+        else:
+            self.data = np.zeros((self.dim, self.u.trajectory.n_frames,
+                                    self.group_j.atoms.n_atoms),
+                                    dtype=np.complex64)
+        self.gij = np.zeros((self.dim,  self.u.trajectory.n_frames),
                                 dtype=np.float32)
         if self.actual_dt is None:
-            _timestep = np.round(self.u.trajectory.dt, 4)
+            self.timestep = np.round(self.u.trajectory.dt, 4)
         else:
-            _timestep = self.actual_dt
-        if self.step > 1:
-            _timestep *= self.step
-        self.t = np.arange(self.u.trajectory.n_frames) * _timestep
-
-    def _evaluate_correlation_ij(self):
-        """Evaluate the correlation function.
+            self.timestep = self.actual_dt
+        self.t = np.arange(self.u.trajectory.n_frames) * self.timestep
 
+    def loop_over_trajectory(self):
+        """Loop of the MDA trajectory and extract rij. 
+        
         Run over the MDA trajectory. If start, stop, or step are
         specified, only a sub-part of the trajectory is analysed.
-
-        Note: if step>1 is given, the timestep is adapted.
         """
-        for _cpt, _ts in enumerate(self.u.trajectory[self.start:self.stop:self.step]):
-            self._position_i = self.group_i.atoms.positions
-            self._position_j = self.group_j.atoms.positions
-            self._box = _ts.dimensions
+        for cpt, ts in enumerate(self.u.trajectory):
+            self.position_i = self.group_i.atoms.positions
+            self.position_j = self.group_j.atoms.positions
+            self.box = ts.dimensions
             # ensure that the box is orthonormal
-            if not np.all(self._box[3:] == self._box[3:][0]) & np.all(self._box[3:][0] == 90.0):
+            if not np.all(self.box[3:] == self.box[3:][0]) & np.all(self.box[3:][0] == 90.0):
                 raise ValueError("NMRforMD does not accept non-orthogonal box"
-                                 "Use triclinic_to_orthorhombic from the package lipyphilic"
-                                 "to convert the trajectory file.")
-            self._vector_ij()
-            self._cartesian_to_spherical()
-            self._spherical_harmonic()
-            if self.order == 'm0':
-                self._data[:, _cpt] = self._sh20
-            elif self.order == 'm012':
-                self._data[:, _cpt] = self._sh20, self._sh21, self._sh22
-        self._calculate_correlation_ij()
-
-    def _calculate_correlation_ij(self):
-        """Calculate the correlation function from ."""
-        for _idx_j in range(self.group_j.atoms.n_atoms):
-            if self.order == 'm0':
-                self.gij += correlation_function(self._data[0, :, _idx_j])
-            elif self.order == 'm012':
-                for _m in range(3):
-                    self.gij[_m] += correlation_function(self._data[_m, :, _idx_j])
-        self.gij = np.real(self.gij)
-
-    def _calculate_fourier_transform(self):
-        # normalise gij by the number of iteration
-        self.gij /= self._cpt_i+1
-        # dimensionalize the correlation function
-        # from A-6 to s2/m6
-        # @tocheck units
-        self.gij *= self._K / cst.angstrom ** 6
-        # for coarse grained models, possibly more than 1 hydrogen per atom
-        self.gij *= np.float32(self.hydrogen_per_atom)
-        if self.order == 'm0':
-            fij = fourier_transform(np.vstack([self.t, self.gij]).T)
-            self.f = np.real(fij.T[0])
-            self.J = np.real(fij.T[1])
-        elif self.order == 'm012':
-            for _m in range(3):
-                fij = fourier_transform(np.vstack([self.t, self.gij[_m]]).T)
-                self.f = np.real(fij.T[0])
-                if _m == 0:
-                    _J_0 = np.real(fij.T[1])
-                elif _m == 1:
-                    _J_1 = np.real(fij.T[1])
-                elif _m == 2:
-                    _J_2 = np.real(fij.T[1])
-            self.J = np.array([_J_0, _J_1, _J_2])
+                                 "You can use triclinic_to_orthorhombic from the package"
+                                 "lipyphilic to convert the trajectory file.")
+            self.vector_rij()
+            self.cartesian_to_spherical()
+            self.evaluate_function_F()
+            self.data[:, cpt] = self.sph_val
 
 
-    def _vector_ij(self):
-        """Calculate distance between position_i and position_j."""
+    def vector_rij(self):
+        """Calculate distance between position_i and position_j.
+        
+        By defaults, periodic boundary conditions are assumed, but can also be turned off.
+        """
         if self.pbc:
-            self._rij = (np.remainder(self._position_i - self._position_j
-                         + self._box[:3]/2., self._box[:3]) - self._box[:3]/2.).T
+            self.rij = (np.remainder(self.position_i - self.position_j
+                         + self.box[:3]/2., self.box[:3]) - self.box[:3]/2.).T
         else:
-            self._rij = (self._position_i - self._position_j).T
+            self.rij = (self.position_i - self.position_j).T
 
-    def _cartesian_to_spherical(self):
+    def cartesian_to_spherical(self):
         """Convert cartesian coordinate to spherical."""
-        self._r = np.sqrt(self._rij[0]**2 + self._rij[1]**2 + self._rij[2]**2)
-        self._theta = np.arctan2(np.sqrt(self._rij[0]**2 + self._rij[1]**2), self._rij[2])
-        self._phi = np.arctan2(self._rij[1], self._rij[0])
-
-    def _spherical_harmonic(self):
-        """Evaluate spherical harmonic functions from rij vector.
-
+        self.r = np.sqrt(self.rij[0]**2 + self.rij[1]**2 + self.rij[2]**2)
+        self.theta = np.arctan2(np.sqrt(self.rij[0]**2 + self.rij[1]**2), self.rij[2])
+        self.phi = np.arctan2(self.rij[1], self.rij[0])
+
+    def evaluate_function_F(self):
+        """Evaluate the F functions.
+
+        F = alpha Y / r ** 3
+        Y : spherical harmonic
+        r : spin-spin distance
+        
         convention : theta = polar angle, phi = azimuthal angle
         note: scipy uses the opposite convention
         """
-        _a_0 = np.sqrt(16 * np.pi / 5)
-        _a_1 = np.sqrt(8 * np.pi / 15)
-        _a_2 = np.sqrt(32 * np.pi / 15)
-        self._sh20 = _a_0 * sph_harm(0, 2, self._phi, self._theta) / np.power(self._r, 3)
-        if self.order == "m0":
-            self._sh20 = self._sh20.real
-        if self.order == "m012":
-            self._sh21 = _a_1 * sph_harm(1, 2, self._phi, self._theta) / np.power(self._r, 3)
-            self._sh22 = _a_2 * sph_harm(2, 2, self._phi, self._theta) / np.power(self._r, 3)
+        F_val = []
+        for m in range(self.dim):
+            F_val.append(self.alpha_m[m] * sph_harm(m, 2, self.phi, self.theta) / np.power(self.r, 3))
+        if self.isotropic:
+            F_val[0] = F_val[0].real
+        self.sph_val = F_val
+
+    def calculate_correlation_ij(self):
+        """Calculate the correlation function."""
+        for idx_j in range(self.group_j.atoms.n_atoms):
+            for m in range(self.dim):
+                self.gij[m] += autocorrelation_function(self.data[m, :, idx_j])
 
-    def _calculate_spectrum(self):
-        """Calculate spectrums R1 and R2 from J."""
-        if self.order == "m0":
-            _inter1d = interp1d(self.f, self.J, fill_value="extrapolate")
-            self.R1 = (_inter1d(self.f)
-                       + 4 * _inter1d(2 * self.f))/6
-            self.R2 = (3/2*_inter1d(self.f[0])
-                       + 5/2*_inter1d(self.f)
-                       + _inter1d(2 * self.f))/6
-        elif self.order == "m012":
-            _inter1d_0 = interp1d(self.f, self.J[0], fill_value="extrapolate")
-            _inter1d_1 = interp1d(self.f, self.J[1], fill_value="extrapolate")
-            _inter1d_2 = interp1d(self.f, self.J[2], fill_value="extrapolate")
-            self.R1 = _inter1d_1(self.f) + _inter1d_2(2 * self.f)
-            self.R2 = (1/4)*(_inter1d_0(self.f[0])+ 10*_inter1d_1(self.f)
-                             + _inter1d_2(2 * self.f))
+        self.gij = np.real(self.gij)
 
-    def _calculate_relaxationtime(self):
+    def finalize(self):
+        # calculate spectrums
+        self.normalize_Gij()
+        self.calculate_fourier_transform()
+        self.calculate_spectrum()
+        self.calculate_relaxationtime()
+
+    def normalize_Gij(self):
+        """Divide Gij by the number of spin pairs.
+        
+        Optional, for coarse grained model, apply a coefficient "hydrogen_per_atom" != 1
+        """
+        # normalise gij by the number of iteration (or number of pair spin)
+        self.gij /= self.cpt_i+1
+        if self.hydrogen_per_atom != 1:
+            self.gij *= np.float32(self.hydrogen_per_atom)
+
+    def calculate_fourier_transform(self):
+        """Calculate spectral density J.
+        
+        Calculate the spectral density J from the 
+        Fourier transform of the correlation function.
+        """
+        # for coarse grained models, possibly more than 1 hydrogen per atom
+        self.J = []
+        for m in range(self.dim):
+            fij = fourier_transform(np.vstack([self.t, self.gij[m]]).T)
+            self.J.append(np.real(fij.T[1]))
+        self.J = np.array(self.J)
+        self.f = np.real(fij.T[0])
+
+    def calculate_spectrum(self):
+        """Calculate spectrums R1 and R2 from J."""
+        inter1d_0 = interp1d(self.f, self.J[0], fill_value="extrapolate")
+        if self.isotropic:
+            self.R1 = self.K/cst.angstrom ** 6 * (inter1d_0(self.f)
+                                                  + 4 * inter1d_0(2 * self.f) )/6
+            self.R2 = self.K/cst.angstrom ** 6 * (3/2*inter1d_0(self.f[0])
+                                                  + 5/2*inter1d_0(self.f)
+                                                  + inter1d_0(2 * self.f) )/6
+        elif self.isotropic is False:
+            inter1d_1 = interp1d(self.f, self.J[1], fill_value="extrapolate")
+            inter1d_2 = interp1d(self.f, self.J[2], fill_value="extrapolate")
+            self.R1 = self.K/cst.angstrom ** 6 * (inter1d_1(self.f)
+                                                  + inter1d_2(2 * self.f))
+            self.R2 = self.K/cst.angstrom ** 6 * ((1/4)*(inter1d_0(self.f[0])
+                                                         + 10*inter1d_1(self.f)
+                                                         + inter1d_2(2 * self.f)))
+        
+    def calculate_relaxationtime(self):
         """Calculate the relaxation time at a given frequency f0 (default is 0)"""
         if self.f0 is None:
             self.T1 = 1/self.R1[0]
             self.T2 = 1/self.R2[0]
         else:
             idx = find_nearest(self.f, self.f0)
             self.T1 = 1 / self.R1[idx]
             self.T2 = 1 / self.R2[idx]
-
-    def _calculate_tau(self):
-        """
-        Calculate correlation time using tau = 0.5 J(0) / G(0).
-
-        The unit are in picosecond. If only the 0th m order is used,
-        one value for tau is returned, if all three m orders are used,
-        three values for tau are returned.
-        """
-        if self.order == "m0":
-            self.tau = 0.5 * (self.J[0] / self.gij[0][0])
-        elif self.order == "m012":
-            self.tau = np.array([0.5*(self.J[0][0] / self.gij.T[0][0]),
-                                 0.5*(self.J[1][0] / self.gij.T[0][1]),
-                                 0.5*(self.J[2][0] / self.gij.T[0][2])])
-        self.tau /= cst.pico
-
-    def _calculate_secondmoment(self):
-        """
-        Calculate second moment Delta omega.
-
-        The unit of Delta omega are kHz /2 pi. The formula is G(0) = (1/3)
-        (Delta omega)**2 where G(0) is the correlation function
-        at time 0. If only the 0th m order is used, one value for Delta omega
-        is returned, if all three m orders are used, three values for Delta
-        omega are returned.
-        """
-        if self.order == "m0":
-            self.delta_omega = np.sqrt(3*self.gij[0][0])
-        elif self.order == "m012":
-            self.delta_omega = np.array([np.sqrt(3*self.gij[0][0]),
-                                         np.sqrt(3*self.gij[0][1]),
-                                         np.sqrt(3*self.gij[0][2])])
-        self.delta_omega /= 1000*2*np.pi
```

### Comparing `nmrformd-0.1.0/setup.py` & `nmrformd-0.1.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 #
 # Released under the GNU Public Licence, v3 or any higher version
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 from setuptools import setup
 
 setup(name='nmrformd',
-      version='v0.1.0',
-      description='Calculate NMR relaxation time from \
+      version='0.1.1',
+      description='Calculate dipolar NMR relaxation time from \
                    molecular dynamics trajectory file',
-      long_description=open('README.rst').read(),
+      long_description=open('LONG_DESCRIPTION.rst').read(),
       long_description_content_type='text/x-rst',
       url='https://github.com/simongravelle/nmrformd',
-      download_url='https://github.com/simongravelle/nmrformd/archive/refs/tags/v0.0.9.tar.gz',  # noqa
+      download_url='https://github.com/simongravelle/nmrformd/archive/refs/tags/0.1.1.tar.gz',  # noqa
       author='Simon Gravelle',
       author_email='simon.gravelle@live.fr',
       license='GNU GENERAL PUBLIC LICENSE',
       packages=['nmrformd'],
       zip_safe=False,
       install_requires=[
        "mdanalysis",
```

