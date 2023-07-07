# Comparing `tmp/oganesson-0.1.7.tar.gz` & `tmp/oganesson-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oganesson-0.1.7.tar", last modified: Mon Jun 26 06:15:22 2023, max compression
+gzip compressed data, was "oganesson-0.1.8.tar", last modified: Fri Jul  7 02:32:23 2023, max compression
```

## Comparing `oganesson-0.1.7.tar` & `oganesson-0.1.8.tar`

### file list

```diff
@@ -1,38 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 06:15:22.525228 oganesson-0.1.7/
--rw-rw-rw-   0        0        0      893 2023-06-26 06:11:57.000000 oganesson-0.1.7/CHANGELOG.md
--rw-rw-rw-   0        0        0     1574 2023-05-25 07:33:57.000000 oganesson-0.1.7/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1108 2023-05-25 07:33:57.000000 oganesson-0.1.7/LICENSE
--rw-rw-rw-   0        0        0      128 2023-05-25 07:33:57.000000 oganesson-0.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0     3322 2023-06-26 06:15:22.522228 oganesson-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     2938 2023-06-13 08:40:24.000000 oganesson-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 06:15:22.427229 oganesson-0.1.7/oganesson/
--rw-rw-rw-   0        0        0        5 2023-06-26 06:11:57.000000 oganesson-0.1.7/oganesson/VERSION
--rw-rw-rw-   0        0        0      901 2023-05-25 07:33:57.000000 oganesson-0.1.7/oganesson/__init__.py
--rw-rw-rw-   0        0        0       72 2023-05-25 07:33:57.000000 oganesson-0.1.7/oganesson/__main__.py
--rw-rw-rw-   0        0        0     1234 2023-05-25 07:33:57.000000 oganesson-0.1.7/oganesson/cli.py
-drwxrwxrwx   0        0        0        0 2023-06-26 06:15:22.492229 oganesson-0.1.7/oganesson/descriptors/
--rw-rw-rw-   0        0        0     1679 2023-06-08 01:20:18.000000 oganesson-0.1.7/oganesson/descriptors/__init__.py
--rw-rw-rw-   0        0        0     7939 2023-05-25 07:33:57.000000 oganesson-0.1.7/oganesson/descriptors/bacd.py
--rw-rw-rw-   0        0        0     1620 2023-06-08 01:20:18.000000 oganesson-0.1.7/oganesson/descriptors/descriptors.py
--rw-rw-rw-   0        0        0     5267 2023-05-25 07:33:57.000000 oganesson-0.1.7/oganesson/descriptors/dscribe.py
--rw-rw-rw-   0        0        0     3606 2023-05-25 07:33:57.000000 oganesson-0.1.7/oganesson/descriptors/rosa.py
--rw-rw-rw-   0        0        0     2805 2023-05-25 07:33:57.000000 oganesson-0.1.7/oganesson/descriptors/symmetry_functions.py
-drwxrwxrwx   0        0        0        0 2023-06-26 06:15:22.498230 oganesson-0.1.7/oganesson/genetic_algorithms/
--rw-rw-rw-   0        0        0    13177 2023-06-26 06:11:57.000000 oganesson-0.1.7/oganesson/genetic_algorithms/__init__.py
--rw-rw-rw-   0        0        0     6399 2023-06-08 01:20:18.000000 oganesson-0.1.7/oganesson/molecular_dynamics.py
--rw-rw-rw-   0        0        0       21 2023-05-25 07:33:57.000000 oganesson-0.1.7/oganesson/ogai.py
--rw-rw-rw-   0        0        0    16259 2023-06-26 06:11:57.000000 oganesson-0.1.7/oganesson/ogstructure.py
-drwxrwxrwx   0        0        0        0 2023-06-26 06:15:22.515231 oganesson-0.1.7/oganesson/utilities/
--rw-rw-rw-   0        0        0      633 2023-05-25 07:33:57.000000 oganesson-0.1.7/oganesson/utilities/__init__.py
--rw-rw-rw-   0        0        0     1571 2023-05-25 07:33:57.000000 oganesson-0.1.7/oganesson/utilities/atomic_data.py
--rw-rw-rw-   0        0        0   405452 2023-05-25 07:33:57.000000 oganesson-0.1.7/oganesson/utilities/bonds_dictionary.py
--rw-rw-rw-   0        0        0      136 2023-05-25 07:33:57.000000 oganesson-0.1.7/oganesson/version.py
-drwxrwxrwx   0        0        0        0 2023-06-26 06:15:22.459227 oganesson-0.1.7/oganesson.egg-info/
--rw-rw-rw-   0        0        0     3322 2023-06-26 06:15:22.000000 oganesson-0.1.7/oganesson.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      799 2023-06-26 06:15:22.000000 oganesson-0.1.7/oganesson.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 06:15:22.000000 oganesson-0.1.7/oganesson.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-06-26 06:15:22.000000 oganesson-0.1.7/oganesson.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       52 2023-06-26 06:15:22.000000 oganesson-0.1.7/oganesson.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-26 06:15:22.000000 oganesson-0.1.7/oganesson.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-26 06:15:22.526228 oganesson-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1182 2023-06-08 01:20:18.000000 oganesson-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 02:32:23.971620 oganesson-0.1.8/
+-rw-rw-rw-   0        0        0       66 2023-05-09 00:45:17.000000 oganesson-0.1.8/.gitattributes
+-rw-rw-rw-   0        0        0     3036 2023-06-08 01:29:47.000000 oganesson-0.1.8/.gitignore
+drwxrwxrwx   0        0        0        0 2023-07-07 02:32:23.904654 oganesson-0.1.8/.vscode/
+-rw-rw-rw-   0        0        0      128 2023-06-13 10:57:12.000000 oganesson-0.1.8/.vscode/settings.json
+-rw-rw-rw-   0        0        0      992 2023-07-07 02:29:42.000000 oganesson-0.1.8/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1574 2023-04-18 13:14:12.000000 oganesson-0.1.8/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1107 2023-05-09 00:45:17.000000 oganesson-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0      128 2023-05-09 01:01:12.000000 oganesson-0.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     3322 2023-07-07 02:32:23.970305 oganesson-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2938 2023-06-13 10:57:12.000000 oganesson-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 02:32:23.906780 oganesson-0.1.8/assets/
+-rw-rw-rw-   0        0        0     2080 2023-05-16 02:19:45.000000 oganesson-0.1.8/assets/logo.svg
+drwxrwxrwx   0        0        0        0 2023-07-07 02:32:23.908953 oganesson-0.1.8/examples/
+-rw-rw-rw-   0        0        0     1820 2023-06-08 01:28:19.000000 oganesson-0.1.8/examples/m3gnet_train.py
+drwxrwxrwx   0        0        0        0 2023-07-07 02:32:23.913957 oganesson-0.1.8/examples/structures/
+-rw-rw-rw-   0        0        0     4538 2023-06-08 01:28:19.000000 oganesson-0.1.8/examples/structures/LGPS_ChemMater_2018_30_4995_Opt.cif
+-rw-rw-rw-   0        0        0     1519 2023-05-17 14:10:37.000000 oganesson-0.1.8/examples/structures/Li3PO4_mp-13725.cif
+-rw-rw-rw-   0        0        0      398 2023-05-17 14:10:37.000000 oganesson-0.1.8/examples/structures/MoS2.vasp
+drwxrwxrwx   0        0        0        0 2023-07-07 02:32:23.927111 oganesson-0.1.8/oganesson/
+-rw-rw-rw-   0        0        0        5 2023-07-07 02:31:52.000000 oganesson-0.1.8/oganesson/VERSION
+-rw-rw-rw-   0        0        0      901 2023-05-17 14:10:37.000000 oganesson-0.1.8/oganesson/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-05-03 06:26:05.000000 oganesson-0.1.8/oganesson/__main__.py
+-rw-rw-rw-   0        0        0     1234 2023-05-09 00:53:11.000000 oganesson-0.1.8/oganesson/cli.py
+drwxrwxrwx   0        0        0        0 2023-07-07 02:32:23.959297 oganesson-0.1.8/oganesson/descriptors/
+-rw-rw-rw-   0        0        0     1679 2023-06-08 01:28:19.000000 oganesson-0.1.8/oganesson/descriptors/__init__.py
+-rw-rw-rw-   0        0        0     7939 2023-05-17 14:10:37.000000 oganesson-0.1.8/oganesson/descriptors/bacd.py
+-rw-rw-rw-   0        0        0     1620 2023-06-08 01:28:19.000000 oganesson-0.1.8/oganesson/descriptors/descriptors.py
+-rw-rw-rw-   0        0        0     5267 2023-05-18 08:13:51.000000 oganesson-0.1.8/oganesson/descriptors/dscribe.py
+-rw-rw-rw-   0        0        0     3606 2023-05-17 14:10:37.000000 oganesson-0.1.8/oganesson/descriptors/rosa.py
+-rw-rw-rw-   0        0        0     2805 2023-05-24 03:23:47.000000 oganesson-0.1.8/oganesson/descriptors/symmetry_functions.py
+drwxrwxrwx   0        0        0        0 2023-07-07 02:32:23.960303 oganesson-0.1.8/oganesson/genetic_algorithms/
+-rw-rw-rw-   0        0        0    13878 2023-07-07 02:29:42.000000 oganesson-0.1.8/oganesson/genetic_algorithms/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 02:32:23.962305 oganesson-0.1.8/oganesson/io/
+-rw-rw-rw-   0        0        0     3803 2023-07-07 02:29:42.000000 oganesson-0.1.8/oganesson/io/vasp.py
+-rw-rw-rw-   0        0        0     6399 2023-06-08 01:28:19.000000 oganesson-0.1.8/oganesson/molecular_dynamics.py
+-rw-rw-rw-   0        0        0       21 2023-05-09 00:51:37.000000 oganesson-0.1.8/oganesson/ogai.py
+-rw-rw-rw-   0        0        0    16259 2023-07-07 02:29:42.000000 oganesson-0.1.8/oganesson/ogstructure.py
+drwxrwxrwx   0        0        0        0 2023-07-07 02:32:23.963305 oganesson-0.1.8/oganesson/reinforcement_learning/
+-rw-rw-rw-   0        0        0        0 2023-05-16 14:41:36.000000 oganesson-0.1.8/oganesson/reinforcement_learning/m3gnet.py
+drwxrwxrwx   0        0        0        0 2023-07-07 02:32:23.967307 oganesson-0.1.8/oganesson/utilities/
+-rw-rw-rw-   0        0        0      633 2023-05-16 01:59:56.000000 oganesson-0.1.8/oganesson/utilities/__init__.py
+-rw-rw-rw-   0        0        0     1524 2023-05-16 06:10:06.000000 oganesson-0.1.8/oganesson/utilities/atomic_data.py
+-rw-rw-rw-   0        0        0   405452 2023-05-17 13:20:45.000000 oganesson-0.1.8/oganesson/utilities/bonds_dictionary.py
+-rw-rw-rw-   0        0        0      136 2023-05-03 11:28:20.000000 oganesson-0.1.8/oganesson/version.py
+drwxrwxrwx   0        0        0        0 2023-07-07 02:32:23.948587 oganesson-0.1.8/oganesson.egg-info/
+-rw-rw-rw-   0        0        0     3322 2023-07-07 02:32:23.000000 oganesson-0.1.8/oganesson.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1093 2023-07-07 02:32:23.000000 oganesson-0.1.8/oganesson.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 02:32:23.000000 oganesson-0.1.8/oganesson.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-07-07 02:32:23.000000 oganesson-0.1.8/oganesson.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       52 2023-07-07 02:32:23.000000 oganesson-0.1.8/oganesson.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-07 02:32:23.000000 oganesson-0.1.8/oganesson.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 02:32:23.972634 oganesson-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1182 2023-06-08 01:28:19.000000 oganesson-0.1.8/setup.py
+-rw-rw-rw-   0        0        0     8797 2023-07-07 02:29:42.000000 oganesson-0.1.8/tutorial.ipynb
```

### Comparing `oganesson-0.1.7/CHANGELOG.md` & `oganesson-0.1.8/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 ## Changelog
 
 
+### 0.1.8 - 2023-07-07
+
+* Added new GA operators
+* Critical fix for vasp.py
+* Several fixes
+
 ### 0.1.7 - 2023-06-13
 
 * Creating the GA object won't relax the initial population. The first call for evolve() will do
 * Initial GA structures can be written to CIF files
 
 ### 0.1.6 - 2023-06-13
```

### Comparing `oganesson-0.1.7/CONTRIBUTING.rst` & `oganesson-0.1.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.7/LICENSE` & `oganesson-0.1.8/LICENSE`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `oganesson-0.1.7/PKG-INFO` & `oganesson-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oganesson
-Version: 0.1.7
+Version: 0.1.8
 Summary: oganesson enables rapid AI workflows for material science and chemistry
 Home-page: https://github.com/oganesson-ai/oganesson
 Author: Sherif Abdulkader Tawfik Abbas
 Author-email: sherif.tawfic@gmail.com
 License: mit
 Keywords: ai,machine learning
 Description-Content-Type: text/markdown
```

### Comparing `oganesson-0.1.7/README.md` & `oganesson-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.7/oganesson/__init__.py` & `oganesson-0.1.8/oganesson/__init__.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.7/oganesson/cli.py` & `oganesson-0.1.8/oganesson/cli.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.7/oganesson/descriptors/__init__.py` & `oganesson-0.1.8/oganesson/descriptors/__init__.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.7/oganesson/descriptors/bacd.py` & `oganesson-0.1.8/oganesson/descriptors/bacd.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.7/oganesson/descriptors/descriptors.py` & `oganesson-0.1.8/oganesson/descriptors/descriptors.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.7/oganesson/descriptors/dscribe.py` & `oganesson-0.1.8/oganesson/descriptors/dscribe.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.7/oganesson/descriptors/rosa.py` & `oganesson-0.1.8/oganesson/descriptors/rosa.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.7/oganesson/descriptors/symmetry_functions.py` & `oganesson-0.1.8/oganesson/descriptors/symmetry_functions.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.7/oganesson/genetic_algorithms/__init__.py` & `oganesson-0.1.8/oganesson/genetic_algorithms/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from ase.ga.population import Population
 from ase.ga.utilities import closest_distances_generator, CellBounds
 from ase.ga.ofp_comparator import OFPComparator
 from ase.ga.offspring_creator import OperationSelector
 from ase.ga.standardmutations import StrainMutation
 from ase.ga.soft_mutation import SoftMutation
 from ase.ga.cutandsplicepairing import CutAndSplicePairing
+from ase.ga.particle_mutations import Poor2richPermutation, Rich2poorPermutation
 from ase import Atoms
 from ase.data import atomic_numbers
 from ase.ga.startgenerator import StartGenerator
 from ase.ga.data import PrepareDB
 from ase.ga import set_raw_score
 from m3gnet.models import Relaxer
 from oganesson.ogstructure import OgStructure
@@ -56,15 +57,15 @@
         if not os.path.isdir(self.path):
             os.mkdir(self.path)
             
         self.path_relaxed = self.path + '/relaxed/'
         if not os.path.isdir(self.path_relaxed):
             os.mkdir(self.path_relaxed)
 
-        print('Starting structural optimization using genetic algorithms..')
+        print('og:Starting structural optimization using genetic algorithms..')
         if population is None:
             self.N = population_size
             self.volume = box_volume
             self.species = species
             self.Z = [atomic_numbers[x] for x in self.species]
 
             self.blmin = closest_distances_generator(atom_numbers=self.Z,
@@ -151,35 +152,50 @@
             
             self.database_connection = DataConnection(self.path+'/ga.db')
             self.slab = self.database_connection.get_slab()
             atom_numbers_to_optimize = self.database_connection.get_atom_numbers_to_optimize()
             self.n_top = len(atom_numbers_to_optimize)
         
         else:
-            raise Exception('Wrong input arguments!')
+            raise Exception('og:Wrong input arguments!')
+
+        print('og:Population size:', self.N)
+
 
-        print('Population size:', self.N)
         self.comp = OFPComparator(n_top=self.n_top, dE=1.0,
                                   cos_dist_max=1e-3, rcut=10., binwidth=0.05,
                                   pbc=[True, True, True], sigma=0.05, nsigma=4,
                                   recalculate=False)
+        
+
 
         self.pairing = CutAndSplicePairing(self.slab, self.n_top, self.blmin, p1=1., p2=0., minfrac=0.15,
                                            number_of_variable_cell_vectors=3,
                                            cellbounds=self.cellbounds, use_tags=False)
 
         self.strainmut = StrainMutation(self.blmin, stddev=0.7, cellbounds=self.cellbounds,
                                         number_of_variable_cell_vectors=3,
                                         use_tags=False)
         self.blmin_soft = closest_distances_generator(
             atom_numbers_to_optimize, 0.1)
         self.softmut = SoftMutation(self.blmin_soft, bounds=[
                                     2., 5.], use_tags=False)
-        self.operators = OperationSelector([4., 3., 3.],
-                                           [self.pairing, self.softmut, self.strainmut])
+        import numpy as np
+        cell = self.slab.get_cell()
+        vol = self.slab.cell.volume
+        axb = np.cross(cell[(i + 1) % 3, :], cell[(i + 2) % 3, :])
+        h = vol / np.linalg.norm(axb)
+        if h >= 20:
+            print('og:Including the Rich2poorPermutation in the list of GA operators')
+            self.rich2poor = Rich2poorPermutation(self.species)
+            self.operators = OperationSelector([3, 2, 1.5, 1.5],
+                                            [self.rich2poor, self.pairing, self.softmut, self.strainmut])
+        else:
+            self.operators = OperationSelector([4, 3, 3],
+                                            [self.pairing, self.softmut, self.strainmut])
         self.relaxed_population = False
         # Relax the initial candidates
     
     def evolve(self, num_offsprings=20):
         if not self.relaxed_population:
             while self.database_connection.get_number_of_unrelaxed_candidates() > 0:
                 a = self.database_connection.get_an_unrelaxed_candidate()
@@ -209,17 +225,17 @@
                                         logfile=self.path+'/log.txt',
                                         use_extinct=True)
 
             current_pop = self.population.get_current_population()
             self.strainmut.update_scaling_volume(
                 current_pop, w_adapt=0.5, n_adapt=4)
             self.pairing.update_scaling_volume(current_pop, w_adapt=0.5, n_adapt=4)
-
+            
             for step in range(num_offsprings):
-                print('Now starting configuration number {0}'.format(step))
+                print('og:Now starting configuration number {0}'.format(step))
 
                 a3 = None
                 while a3 is None:
                     a1, a2 = self.population.get_two_candidates()
                     a3, desc = self.operators.get_new_individual([a1, a2])
 
                 # Save the unrelaxed candidate
@@ -255,16 +271,16 @@
                     current_pop = self.population.get_current_population()
                     self.strainmut.update_scaling_volume(current_pop, w_adapt=0.5,
                                                         n_adapt=4)
                     self.pairing.update_scaling_volume(
                         current_pop, w_adapt=0.5, n_adapt=4)
                     write(self.path+'/current_population.traj', current_pop)
 
-            print('GA finished after step %d' % step)
+            print('og:GA finished after step %d' % step)
             hiscore = get_raw_score(current_pop[0])
-            print('Highest raw score = -%8.4f eV' % hiscore)
+            print('og:Highest raw score = -%8.4f eV' % hiscore)
 
             all_candidates = self.database_connection.get_all_relaxed_candidates()
             write(self.path+'/all_candidates.traj', all_candidates)
 
             current_pop = self.population.get_current_population()
             write(self.path+'/current_population.traj', current_pop)
```

### Comparing `oganesson-0.1.7/oganesson/molecular_dynamics.py` & `oganesson-0.1.8/oganesson/molecular_dynamics.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.7/oganesson/ogstructure.py` & `oganesson-0.1.8/oganesson/ogstructure.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.7/oganesson/utilities/__init__.py` & `oganesson-0.1.8/oganesson/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.7/oganesson/utilities/atomic_data.py` & `oganesson-0.1.8/oganesson/utilities/atomic_data.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,99 +1,96 @@
-00000000: 0d0a 735f 6772 6f75 7073 203d 205b 5b0d  ..s_groups = [[.
-00000010: 0a20 2020 2034 2c20 3132 2c20 3230 2c20  .    4, 12, 20, 
-00000020: 3338 2c20 3536 0d0a 5d2c 0d0a 2020 2020  38, 56..],..    
-00000030: 5b33 2c20 3131 2c20 3139 2c20 3337 2c20  [3, 11, 19, 37, 
-00000040: 3535 5d0d 0a5d 0d0a 0d0a 7261 7265 5f65  55]..]....rare_e
-00000050: 6172 7468 7320 3d20 5b78 2066 6f72 2078  arths = [x for x
-00000060: 2069 6e20 7261 6e67 6528 3537 2c20 3732   in range(57, 72
-00000070: 295d 202b 205b 7820 666f 7220 7820 696e  )] + [x for x in
-00000080: 2072 616e 6765 2838 392c 2039 3529 5d0d   range(89, 95)].
-00000090: 0a0d 0a64 5f67 726f 7570 7320 3d20 5b0d  ...d_groups = [.
-000000a0: 0a20 2020 205b 3231 2c20 3339 5d20 2b20  .    [21, 39] + 
-000000b0: 7261 7265 5f65 6172 7468 730d 0a5d 0d0a  rare_earths..]..
-000000c0: 0d0a 645f 6772 6f75 7073 202b 3d20 5b5b  ..d_groups += [[
-000000d0: 782c 2078 2b31 382c 2078 2b35 305d 2066  x, x+18, x+50] f
-000000e0: 6f72 2078 2069 6e20 7261 6e67 6528 3232  or x in range(22
-000000f0: 2c20 3331 295d 0d0a 0d0a 0d0a 645f 6772  , 31)]......d_gr
-00000100: 6f75 7073 5f6e 6f5f 5245 4173 203d 205b  oups_no_REAs = [
-00000110: 0d0a 2020 2020 5b32 312c 2033 395d 0d0a  ..    [21, 39]..
-00000120: 5d0d 0a0d 0a64 5f67 726f 7570 735f 6e6f  ]....d_groups_no
-00000130: 5f52 4541 7320 2b3d 205b 5b78 2c20 782b  _REAs += [[x, x+
-00000140: 3138 2c20 782b 3530 5d20 666f 7220 7820  18, x+50] for x 
-00000150: 696e 2072 616e 6765 2832 322c 2033 3129  in range(22, 31)
-00000160: 5d0d 0a0d 0a70 5f67 726f 7570 7320 3d20  ]....p_groups = 
-00000170: 5b5b 782c 2078 2b38 2c20 782b 3236 2c20  [[x, x+8, x+26, 
-00000180: 782b 3434 2c20 782b 3736 5d20 666f 7220  x+44, x+76] for 
-00000190: 7820 696e 2072 616e 6765 2835 2c20 3829  x in range(5, 8)
-000001a0: 5d0d 0a70 5f67 726f 7570 7320 2b3d 205b  ]..p_groups += [
-000001b0: 5b78 2c20 782b 382c 2078 2b32 362c 2078  [x, x+8, x+26, x
-000001c0: 2b34 345d 2066 6f72 2078 2069 6e20 7261  +44] for x in ra
-000001d0: 6e67 6528 382c 2031 3129 5d0d 0a0d 0a61  nge(8, 11)]....a
-000001e0: 6c6c 5f67 726f 7570 7320 3d20 645f 6772  ll_groups = d_gr
-000001f0: 6f75 7073 202b 2070 5f67 726f 7570 7320  oups + p_groups 
-00000200: 2b20 735f 6772 6f75 7073 0d0a 616c 6c5f  + s_groups..all_
-00000210: 6772 6f75 7073 5f6e 6f5f 5245 4173 203d  groups_no_REAs =
-00000220: 2064 5f67 726f 7570 735f 6e6f 5f52 4541   d_groups_no_REA
-00000230: 7320 2b20 705f 6772 6f75 7073 202b 2073  s + p_groups + s
-00000240: 5f67 726f 7570 730d 0a0d 0a6c 6162 656c  _groups....label
-00000250: 7320 3d5c 0d0a 2020 2020 5b22 6522 2c20  s =\..    ["e", 
-00000260: 2248 222c 2022 4865 222c 0d0a 2020 2020  "H", "He",..    
-00000270: 2022 4c69 222c 2022 4265 222c 2022 4222   "Li", "Be", "B"
-00000280: 2c20 2243 222c 2022 4e22 2c20 224f 222c  , "C", "N", "O",
-00000290: 2022 4622 2c20 224e 6522 2c0d 0a20 2020   "F", "Ne",..   
-000002a0: 2020 224e 6122 2c20 224d 6722 2c20 2241    "Na", "Mg", "A
-000002b0: 6c22 2c20 2253 6922 2c20 2250 222c 2022  l", "Si", "P", "
-000002c0: 5322 2c20 2243 6c22 2c20 2241 7222 2c0d  S", "Cl", "Ar",.
-000002d0: 0a20 2020 2020 224b 222c 2022 4361 222c  .     "K", "Ca",
-000002e0: 2022 5363 222c 2022 5469 222c 2022 5622   "Sc", "Ti", "V"
-000002f0: 2c20 2243 7222 2c20 224d 6e22 2c20 2246  , "Cr", "Mn", "F
-00000300: 6522 2c20 2243 6f22 2c20 224e 6922 2c20  e", "Co", "Ni", 
-00000310: 2243 7522 2c20 225a 6e22 2c20 2247 6122  "Cu", "Zn", "Ga"
-00000320: 2c20 2247 6522 2c20 2241 7322 2c20 2253  , "Ge", "As", "S
-00000330: 6522 2c20 2242 7222 2c20 224b 7222 2c0d  e", "Br", "Kr",.
-00000340: 0a20 2020 2020 2252 6222 2c20 2253 7222  .     "Rb", "Sr"
-00000350: 2c20 2259 222c 2022 5a72 222c 2022 4e62  , "Y", "Zr", "Nb
-00000360: 222c 2022 4d6f 222c 2022 5463 222c 2022  ", "Mo", "Tc", "
-00000370: 5275 222c 2022 5268 222c 2022 5064 222c  Ru", "Rh", "Pd",
-00000380: 2022 4167 222c 2022 4364 222c 2022 496e   "Ag", "Cd", "In
-00000390: 222c 2022 536e 222c 2022 5362 222c 2022  ", "Sn", "Sb", "
-000003a0: 5465 222c 2022 4922 2c20 2258 6522 2c0d  Te", "I", "Xe",.
-000003b0: 0a20 2020 2020 2243 7322 2c20 2242 6122  .     "Cs", "Ba"
-000003c0: 2c20 224c 6122 2c20 2243 6522 2c20 2250  , "La", "Ce", "P
-000003d0: 7222 2c20 224e 6422 2c20 2250 6d22 2c20  r", "Nd", "Pm", 
-000003e0: 2253 6d22 2c20 2245 7522 2c20 2247 6422  "Sm", "Eu", "Gd"
-000003f0: 2c20 2254 6222 2c20 2244 7922 2c20 2248  , "Tb", "Dy", "H
-00000400: 6f22 2c20 2245 7222 2c20 2254 6d22 2c20  o", "Er", "Tm", 
-00000410: 2259 6222 2c20 224c 7522 2c20 2248 6622  "Yb", "Lu", "Hf"
-00000420: 2c20 2254 6122 2c20 2257 222c 2022 5265  , "Ta", "W", "Re
-00000430: 222c 2022 4f73 222c 2022 4972 222c 2022  ", "Os", "Ir", "
-00000440: 5074 222c 2022 4175 222c 2022 4867 222c  Pt", "Au", "Hg",
-00000450: 2022 546c 222c 2022 5062 222c 2022 4269   "Tl", "Pb", "Bi
-00000460: 222c 2022 506f 222c 2022 4174 222c 2022  ", "Po", "At", "
-00000470: 526e 222c 0d0a 2020 2020 2022 4672 222c  Rn",..     "Fr",
-00000480: 2022 5261 222c 2022 4163 222c 2022 5468   "Ra", "Ac", "Th
-00000490: 222c 2022 5061 222c 2022 5522 2c20 224e  ", "Pa", "U", "N
-000004a0: 7022 2c20 2250 7522 2c20 2241 6d22 2c20  p", "Pu", "Am", 
-000004b0: 2243 6d22 2c20 2242 6b22 2c20 2243 6622  "Cm", "Bk", "Cf"
-000004c0: 2c20 2245 7322 2c20 2246 6d22 2c20 224d  , "Es", "Fm", "M
-000004d0: 6422 2c20 224e 6f22 2c20 224c 7222 2c20  d", "No", "Lr", 
-000004e0: 2252 6622 2c20 2244 6222 2c20 2253 6722  "Rf", "Db", "Sg"
-000004f0: 2c20 2242 6822 2c20 2248 7322 2c20 224d  , "Bh", "Hs", "M
-00000500: 7422 2c20 2244 7322 2c20 2252 6722 2c20  t", "Ds", "Rg", 
-00000510: 2243 6e22 2c20 224e 6822 2c20 2246 6c22  "Cn", "Nh", "Fl"
-00000520: 2c20 224d 6322 2c20 224c 7622 2c20 2254  , "Mc", "Lv", "T
-00000530: 7322 2c20 224f 6722 0d0a 2020 2020 205d  s", "Og"..     ]
-00000540: 0d0a 0d0a 746f 7869 635f 656c 656d 656e  ....toxic_elemen
-00000550: 7473 203d 205b 3333 2c34 382c 3234 2c38  ts = [33,48,24,8
-00000560: 322c 3830 5d0d 0a0d 0a64 6566 2065 6e76  2,80]....def env
-00000570: 5f66 7269 656e 646c 7928 7229 3a0d 0a20  _friendly(r):.. 
-00000580: 2020 2073 3120 3d20 7365 7428 722e 6e75     s1 = set(r.nu
-00000590: 6d62 6572 7329 0d0a 2020 2020 7332 203d  mbers)..    s2 =
-000005a0: 2073 6574 2872 6172 655f 6561 7274 6873   set(rare_earths
-000005b0: 202b 2074 6f78 6963 5f65 6c65 6d65 6e74   + toxic_element
-000005c0: 7329 0d0a 2020 2020 6966 206c 656e 2873  s)..    if len(s
-000005d0: 312e 696e 7465 7273 6563 7469 6f6e 2873  1.intersection(s
-000005e0: 3229 2920 3d3d 2030 3a0d 0a20 2020 2020  2)) == 0:..     
-000005f0: 2020 2072 6574 7572 6e20 5472 7565 0d0a     return True..
-00000600: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00000610: 2020 2072 6574 7572 6e20 4661 6c73 650d     return False.
-00000620: 0a20 20                                  .  
+00000000: 0a73 5f67 726f 7570 7320 3d20 5b5b 0a20  .s_groups = [[. 
+00000010: 2020 2034 2c20 3132 2c20 3230 2c20 3338     4, 12, 20, 38
+00000020: 2c20 3536 0a5d 2c0a 2020 2020 5b33 2c20  , 56.],.    [3, 
+00000030: 3131 2c20 3139 2c20 3337 2c20 3535 5d0a  11, 19, 37, 55].
+00000040: 5d0a 0a72 6172 655f 6561 7274 6873 203d  ]..rare_earths =
+00000050: 205b 7820 666f 7220 7820 696e 2072 616e   [x for x in ran
+00000060: 6765 2835 372c 2037 3229 5d20 2b20 5b78  ge(57, 72)] + [x
+00000070: 2066 6f72 2078 2069 6e20 7261 6e67 6528   for x in range(
+00000080: 3839 2c20 3935 295d 0a0a 645f 6772 6f75  89, 95)]..d_grou
+00000090: 7073 203d 205b 0a20 2020 205b 3231 2c20  ps = [.    [21, 
+000000a0: 3339 5d20 2b20 7261 7265 5f65 6172 7468  39] + rare_earth
+000000b0: 730a 5d0a 0a64 5f67 726f 7570 7320 2b3d  s.]..d_groups +=
+000000c0: 205b 5b78 2c20 782b 3138 2c20 782b 3530   [[x, x+18, x+50
+000000d0: 5d20 666f 7220 7820 696e 2072 616e 6765  ] for x in range
+000000e0: 2832 322c 2033 3129 5d0a 0a0a 645f 6772  (22, 31)]...d_gr
+000000f0: 6f75 7073 5f6e 6f5f 5245 4173 203d 205b  oups_no_REAs = [
+00000100: 0a20 2020 205b 3231 2c20 3339 5d0a 5d0a  .    [21, 39].].
+00000110: 0a64 5f67 726f 7570 735f 6e6f 5f52 4541  .d_groups_no_REA
+00000120: 7320 2b3d 205b 5b78 2c20 782b 3138 2c20  s += [[x, x+18, 
+00000130: 782b 3530 5d20 666f 7220 7820 696e 2072  x+50] for x in r
+00000140: 616e 6765 2832 322c 2033 3129 5d0a 0a70  ange(22, 31)]..p
+00000150: 5f67 726f 7570 7320 3d20 5b5b 782c 2078  _groups = [[x, x
+00000160: 2b38 2c20 782b 3236 2c20 782b 3434 2c20  +8, x+26, x+44, 
+00000170: 782b 3736 5d20 666f 7220 7820 696e 2072  x+76] for x in r
+00000180: 616e 6765 2835 2c20 3829 5d0a 705f 6772  ange(5, 8)].p_gr
+00000190: 6f75 7073 202b 3d20 5b5b 782c 2078 2b38  oups += [[x, x+8
+000001a0: 2c20 782b 3236 2c20 782b 3434 5d20 666f  , x+26, x+44] fo
+000001b0: 7220 7820 696e 2072 616e 6765 2838 2c20  r x in range(8, 
+000001c0: 3131 295d 0a0a 616c 6c5f 6772 6f75 7073  11)]..all_groups
+000001d0: 203d 2064 5f67 726f 7570 7320 2b20 705f   = d_groups + p_
+000001e0: 6772 6f75 7073 202b 2073 5f67 726f 7570  groups + s_group
+000001f0: 730a 616c 6c5f 6772 6f75 7073 5f6e 6f5f  s.all_groups_no_
+00000200: 5245 4173 203d 2064 5f67 726f 7570 735f  REAs = d_groups_
+00000210: 6e6f 5f52 4541 7320 2b20 705f 6772 6f75  no_REAs + p_grou
+00000220: 7073 202b 2073 5f67 726f 7570 730a 0a6c  ps + s_groups..l
+00000230: 6162 656c 7320 3d5c 0a20 2020 205b 2265  abels =\.    ["e
+00000240: 222c 2022 4822 2c20 2248 6522 2c0a 2020  ", "H", "He",.  
+00000250: 2020 2022 4c69 222c 2022 4265 222c 2022     "Li", "Be", "
+00000260: 4222 2c20 2243 222c 2022 4e22 2c20 224f  B", "C", "N", "O
+00000270: 222c 2022 4622 2c20 224e 6522 2c0a 2020  ", "F", "Ne",.  
+00000280: 2020 2022 4e61 222c 2022 4d67 222c 2022     "Na", "Mg", "
+00000290: 416c 222c 2022 5369 222c 2022 5022 2c20  Al", "Si", "P", 
+000002a0: 2253 222c 2022 436c 222c 2022 4172 222c  "S", "Cl", "Ar",
+000002b0: 0a20 2020 2020 224b 222c 2022 4361 222c  .     "K", "Ca",
+000002c0: 2022 5363 222c 2022 5469 222c 2022 5622   "Sc", "Ti", "V"
+000002d0: 2c20 2243 7222 2c20 224d 6e22 2c20 2246  , "Cr", "Mn", "F
+000002e0: 6522 2c20 2243 6f22 2c20 224e 6922 2c20  e", "Co", "Ni", 
+000002f0: 2243 7522 2c20 225a 6e22 2c20 2247 6122  "Cu", "Zn", "Ga"
+00000300: 2c20 2247 6522 2c20 2241 7322 2c20 2253  , "Ge", "As", "S
+00000310: 6522 2c20 2242 7222 2c20 224b 7222 2c0a  e", "Br", "Kr",.
+00000320: 2020 2020 2022 5262 222c 2022 5372 222c       "Rb", "Sr",
+00000330: 2022 5922 2c20 225a 7222 2c20 224e 6222   "Y", "Zr", "Nb"
+00000340: 2c20 224d 6f22 2c20 2254 6322 2c20 2252  , "Mo", "Tc", "R
+00000350: 7522 2c20 2252 6822 2c20 2250 6422 2c20  u", "Rh", "Pd", 
+00000360: 2241 6722 2c20 2243 6422 2c20 2249 6e22  "Ag", "Cd", "In"
+00000370: 2c20 2253 6e22 2c20 2253 6222 2c20 2254  , "Sn", "Sb", "T
+00000380: 6522 2c20 2249 222c 2022 5865 222c 0a20  e", "I", "Xe",. 
+00000390: 2020 2020 2243 7322 2c20 2242 6122 2c20      "Cs", "Ba", 
+000003a0: 224c 6122 2c20 2243 6522 2c20 2250 7222  "La", "Ce", "Pr"
+000003b0: 2c20 224e 6422 2c20 2250 6d22 2c20 2253  , "Nd", "Pm", "S
+000003c0: 6d22 2c20 2245 7522 2c20 2247 6422 2c20  m", "Eu", "Gd", 
+000003d0: 2254 6222 2c20 2244 7922 2c20 2248 6f22  "Tb", "Dy", "Ho"
+000003e0: 2c20 2245 7222 2c20 2254 6d22 2c20 2259  , "Er", "Tm", "Y
+000003f0: 6222 2c20 224c 7522 2c20 2248 6622 2c20  b", "Lu", "Hf", 
+00000400: 2254 6122 2c20 2257 222c 2022 5265 222c  "Ta", "W", "Re",
+00000410: 2022 4f73 222c 2022 4972 222c 2022 5074   "Os", "Ir", "Pt
+00000420: 222c 2022 4175 222c 2022 4867 222c 2022  ", "Au", "Hg", "
+00000430: 546c 222c 2022 5062 222c 2022 4269 222c  Tl", "Pb", "Bi",
+00000440: 2022 506f 222c 2022 4174 222c 2022 526e   "Po", "At", "Rn
+00000450: 222c 0a20 2020 2020 2246 7222 2c20 2252  ",.     "Fr", "R
+00000460: 6122 2c20 2241 6322 2c20 2254 6822 2c20  a", "Ac", "Th", 
+00000470: 2250 6122 2c20 2255 222c 2022 4e70 222c  "Pa", "U", "Np",
+00000480: 2022 5075 222c 2022 416d 222c 2022 436d   "Pu", "Am", "Cm
+00000490: 222c 2022 426b 222c 2022 4366 222c 2022  ", "Bk", "Cf", "
+000004a0: 4573 222c 2022 466d 222c 2022 4d64 222c  Es", "Fm", "Md",
+000004b0: 2022 4e6f 222c 2022 4c72 222c 2022 5266   "No", "Lr", "Rf
+000004c0: 222c 2022 4462 222c 2022 5367 222c 2022  ", "Db", "Sg", "
+000004d0: 4268 222c 2022 4873 222c 2022 4d74 222c  Bh", "Hs", "Mt",
+000004e0: 2022 4473 222c 2022 5267 222c 2022 436e   "Ds", "Rg", "Cn
+000004f0: 222c 2022 4e68 222c 2022 466c 222c 2022  ", "Nh", "Fl", "
+00000500: 4d63 222c 2022 4c76 222c 2022 5473 222c  Mc", "Lv", "Ts",
+00000510: 2022 4f67 220a 2020 2020 205d 0a0a 746f   "Og".     ]..to
+00000520: 7869 635f 656c 656d 656e 7473 203d 205b  xic_elements = [
+00000530: 3333 2c34 382c 3234 2c38 322c 3830 5d0a  33,48,24,82,80].
+00000540: 0a64 6566 2065 6e76 5f66 7269 656e 646c  .def env_friendl
+00000550: 7928 7229 3a0a 2020 2020 7331 203d 2073  y(r):.    s1 = s
+00000560: 6574 2872 2e6e 756d 6265 7273 290a 2020  et(r.numbers).  
+00000570: 2020 7332 203d 2073 6574 2872 6172 655f    s2 = set(rare_
+00000580: 6561 7274 6873 202b 2074 6f78 6963 5f65  earths + toxic_e
+00000590: 6c65 6d65 6e74 7329 0a20 2020 2069 6620  lements).    if 
+000005a0: 6c65 6e28 7331 2e69 6e74 6572 7365 6374  len(s1.intersect
+000005b0: 696f 6e28 7332 2929 203d 3d20 303a 0a20  ion(s2)) == 0:. 
+000005c0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
+000005d0: 7565 0a20 2020 2065 6c73 653a 0a20 2020  ue.    else:.   
+000005e0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+000005f0: 650a 2020                                e.
```

### Comparing `oganesson-0.1.7/oganesson/utilities/bonds_dictionary.py` & `oganesson-0.1.8/oganesson/utilities/bonds_dictionary.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.7/oganesson.egg-info/PKG-INFO` & `oganesson-0.1.8/oganesson.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oganesson
-Version: 0.1.7
+Version: 0.1.8
 Summary: oganesson enables rapid AI workflows for material science and chemistry
 Home-page: https://github.com/oganesson-ai/oganesson
 Author: Sherif Abdulkader Tawfik Abbas
 Author-email: sherif.tawfic@gmail.com
 License: mit
 Keywords: ai,machine learning
 Description-Content-Type: text/markdown
```

### Comparing `oganesson-0.1.7/setup.py` & `oganesson-0.1.8/setup.py`

 * *Files identical despite different names*

