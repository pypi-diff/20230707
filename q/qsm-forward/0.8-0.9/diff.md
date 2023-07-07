# Comparing `tmp/qsm-forward-0.8.tar.gz` & `tmp/qsm-forward-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qsm-forward-0.8.tar", last modified: Tue Jun 27 01:21:32 2023, max compression
+gzip compressed data, was "qsm-forward-0.9.tar", last modified: Tue Jun 27 01:59:16 2023, max compression
```

## Comparing `qsm-forward-0.8.tar` & `qsm-forward-0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-27 01:21:32.515067 qsm-forward-0.8/
--rw-r--r--   0 ashley    (1000) ashley    (1000)    35149 2023-06-12 05:17:28.000000 qsm-forward-0.8/LICENSE
--rw-r--r--   0 ashley    (1000) ashley    (1000)     9000 2023-06-27 01:21:32.515067 qsm-forward-0.8/PKG-INFO
--rw-r--r--   0 ashley    (1000) ashley    (1000)     8229 2023-06-27 01:16:59.000000 qsm-forward-0.8/README.md
--rw-r--r--   0 ashley    (1000) ashley    (1000)      750 2023-06-27 01:15:26.000000 qsm-forward-0.8/pyproject.toml
-drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-27 01:21:32.515067 qsm-forward-0.8/qsm_forward/
--rw-r--r--   0 ashley    (1000) ashley    (1000)      497 2023-06-16 01:20:38.000000 qsm-forward-0.8/qsm_forward/__init__.py
--rw-r--r--   0 ashley    (1000) ashley    (1000)    29159 2023-06-27 00:56:58.000000 qsm-forward-0.8/qsm_forward/qsm_forward.py
-drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-27 01:21:32.515067 qsm-forward-0.8/qsm_forward.egg-info/
--rw-r--r--   0 ashley    (1000) ashley    (1000)     9000 2023-06-27 01:21:32.000000 qsm-forward-0.8/qsm_forward.egg-info/PKG-INFO
--rw-r--r--   0 ashley    (1000) ashley    (1000)      292 2023-06-27 01:21:32.000000 qsm-forward-0.8/qsm_forward.egg-info/SOURCES.txt
--rw-r--r--   0 ashley    (1000) ashley    (1000)        1 2023-06-27 01:21:32.000000 qsm-forward-0.8/qsm_forward.egg-info/dependency_links.txt
--rw-r--r--   0 ashley    (1000) ashley    (1000)       19 2023-06-27 01:21:32.000000 qsm-forward-0.8/qsm_forward.egg-info/requires.txt
--rw-r--r--   0 ashley    (1000) ashley    (1000)       12 2023-06-27 01:21:32.000000 qsm-forward-0.8/qsm_forward.egg-info/top_level.txt
--rw-r--r--   0 ashley    (1000) ashley    (1000)       38 2023-06-27 01:21:32.515067 qsm-forward-0.8/setup.cfg
--rw-r--r--   0 ashley    (1000) ashley    (1000)      812 2023-06-27 01:15:36.000000 qsm-forward-0.8/setup.py
-drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-27 01:21:32.515067 qsm-forward-0.8/tests/
--rw-r--r--   0 ashley    (1000) ashley    (1000)        6 2023-06-12 05:17:28.000000 qsm-forward-0.8/tests/test_qsm_forward.py
+drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-27 01:59:16.121678 qsm-forward-0.9/
+-rw-r--r--   0 ashley    (1000) ashley    (1000)    35149 2023-06-12 05:17:28.000000 qsm-forward-0.9/LICENSE
+-rw-r--r--   0 ashley    (1000) ashley    (1000)     9000 2023-06-27 01:59:16.121678 qsm-forward-0.9/PKG-INFO
+-rw-r--r--   0 ashley    (1000) ashley    (1000)     8229 2023-06-27 01:16:59.000000 qsm-forward-0.9/README.md
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      750 2023-06-27 01:57:04.000000 qsm-forward-0.9/pyproject.toml
+drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-27 01:59:16.121678 qsm-forward-0.9/qsm_forward/
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      497 2023-06-16 01:20:38.000000 qsm-forward-0.9/qsm_forward/__init__.py
+-rw-r--r--   0 ashley    (1000) ashley    (1000)    28358 2023-06-27 01:58:07.000000 qsm-forward-0.9/qsm_forward/qsm_forward.py
+drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-27 01:59:16.121678 qsm-forward-0.9/qsm_forward.egg-info/
+-rw-r--r--   0 ashley    (1000) ashley    (1000)     9000 2023-06-27 01:59:16.000000 qsm-forward-0.9/qsm_forward.egg-info/PKG-INFO
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      292 2023-06-27 01:59:16.000000 qsm-forward-0.9/qsm_forward.egg-info/SOURCES.txt
+-rw-r--r--   0 ashley    (1000) ashley    (1000)        1 2023-06-27 01:59:16.000000 qsm-forward-0.9/qsm_forward.egg-info/dependency_links.txt
+-rw-r--r--   0 ashley    (1000) ashley    (1000)       19 2023-06-27 01:59:16.000000 qsm-forward-0.9/qsm_forward.egg-info/requires.txt
+-rw-r--r--   0 ashley    (1000) ashley    (1000)       12 2023-06-27 01:59:16.000000 qsm-forward-0.9/qsm_forward.egg-info/top_level.txt
+-rw-r--r--   0 ashley    (1000) ashley    (1000)       38 2023-06-27 01:59:16.121678 qsm-forward-0.9/setup.cfg
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      812 2023-06-27 01:57:01.000000 qsm-forward-0.9/setup.py
+drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-27 01:59:16.121678 qsm-forward-0.9/tests/
+-rw-r--r--   0 ashley    (1000) ashley    (1000)        6 2023-06-12 05:17:28.000000 qsm-forward-0.9/tests/test_qsm_forward.py
```

### Comparing `qsm-forward-0.8/LICENSE` & `qsm-forward-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qsm-forward-0.8/PKG-INFO` & `qsm-forward-0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsm-forward
-Version: 0.8
+Version: 0.9
 Summary: A forward-model simulation for Quantitative Susceptibility Mapping
 Home-page: https://github.com/astewartau/qsm-forward-model
 Author: Ashley Stewart
 Author-email: Ashley Stewart <a.stewart.au@gmail.com>
 Project-URL: Homepage, https://github.com/astewartau/qsm-forward-model
 Project-URL: Bug Tracker, https://github.com/astewartau/qsm-forward-model/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `qsm-forward-0.8/README.md` & `qsm-forward-0.9/README.md`

 * *Files identical despite different names*

### Comparing `qsm-forward-0.8/pyproject.toml` & `qsm-forward-0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qsm-forward"
-version = "0.8"
+version = "0.9"
 authors = [
   { name="Ashley Stewart", email="a.stewart.au@gmail.com" },
 ]
 description = "A forward-model simulation for Quantitative Susceptibility Mapping"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers=[
```

### Comparing `qsm-forward-0.8/qsm_forward/qsm_forward.py` & `qsm-forward-0.9/qsm_forward/qsm_forward.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             self,
             root_dir = "",
             chi = "ChiModelMIX_noCalc.nii.gz",
             M0 = "M0.nii.gz",
             R1 = "R1.nii.gz",
             R2star = "R2star.nii.gz",
             mask = "BrainMask.nii.gz",
-            seg = "SegmentedModel.nii.gz",
+            seg = "SegmentedModel.nii.gz"
     ):
         if isinstance(chi, str) and not os.path.exists(os.path.join(root_dir, chi)):
             raise ValueError(f"Path to chi is invalid! ({os.path.join(root_dir, chi)})")
         self._chi = os.path.join(root_dir, chi) if isinstance(chi, str) and os.path.exists(os.path.join(root_dir, chi)) else chi if not isinstance(chi, str) else None
         self._M0 = os.path.join(root_dir, M0) if isinstance(M0, str) and os.path.exists(os.path.join(root_dir, M0)) else M0 if not isinstance(M0, str) else None
         self._R1 = os.path.join(root_dir, R1) if isinstance(R1, str) and os.path.exists(os.path.join(root_dir, R1)) else R1 if not isinstance(R1, str) else None
         self._R2star = os.path.join(root_dir, R2star) if isinstance(R2star, str) and os.path.exists(os.path.join(root_dir, R2star)) else R2star if not isinstance(R2star, str) else None
@@ -68,66 +68,24 @@
     def chi(self): return nib.load(self._chi) if isinstance(self._chi, str) else nib.Nifti1Image(self._chi, affine=self.nii_affine, header=self.nii_header)
 
     @property
     def mask(self): return nib.load(self._mask) if isinstance(self._mask, str) else nib.Nifti1Image(self._mask or np.array(self._chi != 0), affine=self.nii_affine, header=self.nii_header)
 
     @property
     def M0(self): return nib.load(self._M0) if isinstance(self._M0, str) else nib.Nifti1Image(self._M0 or np.array(self.mask.get_fdata() * 1), affine=self.nii_affine, header=self.nii_header)
-    #def M0(self): return nib.load(self._M0) if isinstance(self._M0, str) else nib.Nifti1Image(self._estimate_M0(1, self.chi.get_fdata()), affine=self.nii_affine, header=self.nii_header)
 
     @property
     def R1(self): return nib.load(self._R1) if isinstance(self._R1, str) else nib.Nifti1Image(self._R1 or np.array(self.mask.get_fdata() * 1), affine=self.nii_affine, header=self.nii_header)
     
     @property
     def R2star(self): return nib.load(self._R2star) if isinstance(self._R2star, str) else nib.Nifti1Image(self._R2star or np.array(self.mask.get_fdata() * 50), affine=self.nii_affine, header=self.nii_header)
     
     @property
     def seg(self): return nib.load(self._seg) if isinstance(self._seg, str) else nib.Nifti1Image(self._seg or self.mask.get_fdata(), affine=self.nii_affine, header=self.nii_header)
     
-    def _estimate_M0(self, B0, chi):
-        """
-        Calculate the equilibrium magnetization M0 based on B0 field strength and magnetic susceptibility (chi).
-
-        Parameters
-        ----------
-        B0 : float
-            The main magnetic field strength (in T).
-        chi : numpy.ndarray
-            The magnetic susceptibility map.
-
-        Returns
-        -------
-        M0 : numpy.ndarray
-            The calculated equilibrium magnetization.
-        """
-        
-        # Constants
-        k = 1.38064852e-23  # Boltzmann constant (m^2 kg s^-2 K^-1)
-        h = 6.62607015e-34  # Planck's constant (m^2 kg s^-1)
-        gamma = 267.522190e3  # proton gyromagnetic ratio (kHz/T to Hz/T)
-        rho = 65  # proton density (mol/L)
-        T = 298.15  # absolute temperature (K)
-        
-        # Convert gamma from Hz/T to rad/(s*T)
-        gamma = gamma * 2 * np.pi * 1e3 
-
-        # Convert rho from mol/L to mol/m^3
-        rho = rho * 1e3
-
-        # Calculate B from B0 and chi
-        B = B0 * (1 + chi)
-
-        # Calculate M0
-        M0 = gamma * rho * h * B / (2 * k * T)
-
-        nib.save(nib.Nifti1Image(M0, affine=self.nii_affine, header=self.nii_header), "M0_TEST.nii")
-        nib.save(nib.Nifti1Image(B, affine=self.nii_affine, header=self.nii_header), "B_TEST.nii")
-
-        return M0
-
 
 class ReconParams:
     """
     A class used to represent reconstruction parameters.
 
     Attributes
     ----------
@@ -153,14 +111,16 @@
         Boolean to control phase offset generation.
     generate_shim_field : bool
         Boolean to control shim field generation.
     voxel_size : np.array
         Voxel size (in mm).
     peak_snr : float
         Peak signal-to-noise ratio.
+    random_seed : int
+        Random seed to use for noise.
     """
 
     def __init__(
             self,
             subject="1",
             session="1",
             run="1",
@@ -169,29 +129,31 @@
             flip_angle=15,
             B0=7,
             B0_dir=np.array([0, 0, 1]),
             phase_offset=0,
             generate_phase_offset=True,
             generate_shim_field=True,
             voxel_size=np.array([1.0, 1.0, 1.0]),
-            peak_snr=np.inf
+            peak_snr=np.inf,
+            random_seed=None
         ):
         self.subject = subject
         self.session = session
         self.run = run
         self.TR = TR
         self.TEs = TEs
         self.flip_angle = flip_angle
         self.B0 = B0
         self.B0_dir = B0_dir
         self.phase_offset = phase_offset
         self.generate_phase_offset = generate_phase_offset
         self.generate_shim_field = generate_shim_field
         self.voxel_size = voxel_size
         self.peak_snr = peak_snr
+        self.random_seed = random_seed
 
 def generate_bids(tissue_params: TissueParams, recon_params: ReconParams, bids_dir):
     """
     Simulate T2*-weighted magnitude and phase images and save the outputs in the BIDS-compliant format.
 
     This function simulates a T2*-weighted MRI signal based on a ground truth susceptibility map,
     and saves the outputs (images, JSON headers) in the BIDS-compliant format in the specified
@@ -219,26 +181,29 @@
     
     # recon name
     recon_name = f"sub-{recon_params.subject}_ses-{recon_params.session}_run-{recon_params.run}"
     session_dir = os.path.join(bids_dir, f"sub-{recon_params.subject}", f"ses-{recon_params.session}")
     os.makedirs(os.path.join(session_dir, 'anat'), exist_ok=True)
     os.makedirs(os.path.join(session_dir, 'extra_data'), exist_ok=True)
 
+    # random number generator for noise etc.
+    rng = np.random.default_rng(recon_params.random_seed)
+
     # image-space resizing
     print("Image-space resizing of chi...")
     chi_downsampled_nii = resize(tissue_params.chi, recon_params.voxel_size)
     nib.save(chi_downsampled_nii, filename=os.path.join(session_dir, "extra_data", f"{recon_name}_chi.nii"))
     print("Image-space cropping of mask...")
     nib.save(resize(tissue_params.mask, recon_params.voxel_size, 'nearest'), filename=os.path.join(session_dir, "extra_data", f"{recon_name}_mask.nii"))
     print("Image-space cropping of segmentation...")
     nib.save(resize(tissue_params.seg, recon_params.voxel_size, 'nearest'), filename=os.path.join(session_dir, "extra_data", f"{recon_name}_segmentation.nii"))
 
     # calculate field
     print("Computing field model...")
-    field = generate_field(tissue_params.chi.get_fdata())
+    field = generate_field(tissue_params.chi.get_fdata(), voxel_size=recon_params.voxel_size, B0_dir=recon_params.B0_dir)
 
     # simulate shim field
     if recon_params.generate_shim_field:
         print("Computing shim fields...")
         _, field, _ = generate_shimmed_field(field, tissue_params.mask.get_fdata(), order=2)
 
     # phase offset
@@ -268,15 +233,15 @@
         print(f"k-space cropping of MR signal for echo {i+1}...")
         resolution = np.array(np.round((np.array(tissue_params.chi.header.get_zooms()) / recon_params.voxel_size) * np.array(tissue_params.chi.header.get_data_shape())), dtype=int)
         sigHR_cropped = crop_kspace(sigHR, resolution)
         del sigHR
 
         # noise
         print(f"Simulating noise for echo {i+1}...")
-        sigHR_cropped_noisy = add_noise(sigHR_cropped, peak_snr=recon_params.peak_snr)
+        sigHR_cropped_noisy = add_noise(sigHR_cropped, peak_snr=recon_params.peak_snr, rng=rng)
         del sigHR_cropped
 
         # save nifti images
         mag_filename = f"{recon_name_i}_part-mag" + ("_MEGRE" if multiecho else "_T2starw")
         phs_filename = f"{recon_name_i}_part-phase" + ("_MEGRE" if multiecho else "_T2starw")
         nib.save(nib.Nifti1Image(dataobj=np.abs(sigHR_cropped_noisy)*500, affine=chi_downsampled_nii.affine, header=chi_downsampled_nii.header), filename=os.path.join(session_dir, "anat", f"{mag_filename}.nii"))
         nib.save(nib.Nifti1Image(dataobj=np.angle(sigHR_cropped_noisy), affine=chi_downsampled_nii.affine, header=chi_downsampled_nii.header), filename=os.path.join(session_dir, "anat", f"{phs_filename}.nii"))
@@ -456,32 +421,38 @@
 
     sigHR = M0 * np.exp(1j * (2 * np.pi * field * B0 * 42.58 * TE + phase_offset)) * np.exp(-TE * R2star) \
         * (1 - np.exp(-TR * R1)) * np.sin(np.deg2rad(flip_angle)) / (1 - np.cos(np.deg2rad(flip_angle)) * np.exp(-TR * R1))
     sigHR[np.isnan(sigHR)]
 
     return sigHR
 
-def add_noise(sig, peak_snr=np.inf):
+def add_noise(sig, peak_snr=np.inf, rng=None):
     """
     Add complex Gaussian noise to a signal.
 
     Parameters
     ----------
     sig : numpy.ndarray
         The input signal to which noise will be added.
     peak_snr : float, optional
         The peak signal-to-noise ratio, by default np.inf
+    rng : numpy.random.Generator, optional
+        A random number Generator. If None, a new Generator will be created.
 
     Returns
     -------
     numpy.ndarray
         The input signal with added noise.
     """
 
-    noise = np.random.randn(*sig.shape) + 1j * np.random.randn(*sig.shape)
+    # Create a new RNG if one was not provided
+    if rng is None:
+        rng = np.random.default_rng()
+
+    noise = rng.standard_normal(sig.shape) + 1j * rng.standard_normal(sig.shape)
     sig_noisy = sig + (noise * np.max(np.abs(sig))) / peak_snr
     return sig_noisy
 
 
 def resize(nii, voxel_size, interpolation='continuous'):
     """
     Resize a Nifti image to a voxel size.
@@ -704,14 +675,15 @@
 def simulate_susceptibility_sources(
     simulation_dim=160,
     rectangles_total=50,
     spheres_total=50,
     sus_std=1,
     shape_size_min_factor=0.01,
     shape_size_max_factor=0.5,
+    seed=None
 ):
     """
     This function simulates susceptibility sources by generating a three-dimensional numpy array, 
     and populating it with a certain number of randomly generated and positioned rectangular prisms and spheres.
     
     Parameters
     ----------
@@ -730,42 +702,48 @@
     shape_size_min_factor : float
         A factor to determine the minimum size of the shapes (both rectangular prisms and spheres). 
         The actual minimum size in each dimension is calculated as simulation_dim * shape_size_min_factor.
         
     shape_size_max_factor : float
         A factor to determine the maximum size of the shapes (both rectangular prisms and spheres). 
         The actual maximum size in each dimension is calculated as simulation_dim * shape_size_max_factor.
+
+    seed : int, optional
+        A seed for the random number generator. If None, a random seed will be used.
         
     Returns
     -------
     temp_sources : ndarray
         A three-dimensional numpy array of size (simulation_dim, simulation_dim, simulation_dim) 
         that contains the simulated susceptibility sources. Rectangular prisms and spheres have susceptibility 
         values drawn from a Gaussian distribution, while all other points are set to zero.
     """
 
     temp_sources = np.zeros((simulation_dim, simulation_dim, simulation_dim))
 
+    # Create a new generator instance with the provided seed if one was given
+    rng = np.random.default_rng(seed)
+
     # Generate rectangles
     for shapes in range(rectangles_total):
         shrink_factor = 1 / ((shapes / rectangles_total + 1))
         shape_size_min = np.floor(
             simulation_dim * shrink_factor * shape_size_min_factor
         )
         shape_size_max = np.floor(
             simulation_dim * shrink_factor * shape_size_max_factor
         )
 
-        susceptibility_value = np.random.normal(loc=0.0, scale=sus_std)
-        random_sizex = np.random.randint(low=shape_size_min, high=shape_size_max)
-        random_sizey = np.random.randint(low=shape_size_min, high=shape_size_max)
-        random_sizez = np.random.randint(low=shape_size_min, high=shape_size_max)
-        x_pos = np.random.randint(simulation_dim)
-        y_pos = np.random.randint(simulation_dim)
-        z_pos = np.random.randint(simulation_dim)
+        susceptibility_value = rng.normal(loc=0.0, scale=sus_std)
+        random_sizex = rng.integers(low=shape_size_min, high=shape_size_max)
+        random_sizey = rng.integers(low=shape_size_min, high=shape_size_max)
+        random_sizez = rng.integers(low=shape_size_min, high=shape_size_max)
+        x_pos = rng.integers(simulation_dim)
+        y_pos = rng.integers(simulation_dim)
+        z_pos = rng.integers(simulation_dim)
 
         x_pos_max = x_pos + random_sizex
         if x_pos_max >= simulation_dim:
             x_pos_max = simulation_dim
 
         y_pos_max = y_pos + random_sizey
         if y_pos_max >= simulation_dim:
@@ -777,19 +755,19 @@
 
         temp_sources[
             x_pos:x_pos_max, y_pos:y_pos_max, z_pos:z_pos_max
         ] = susceptibility_value
 
     # Generate spheres
     for sphere in range(spheres_total):
-        susceptibility_value = np.random.normal(loc=0.0, scale=sus_std)
-        sphere_radius = np.random.randint(low=shape_size_min//2, high=shape_size_max//2)
-        x_center = np.random.randint(simulation_dim)
-        y_center = np.random.randint(simulation_dim)
-        z_center = np.random.randint(simulation_dim)
+        susceptibility_value = rng.normal(loc=0.0, scale=sus_std)
+        sphere_radius = rng.integers(low=shape_size_min//2, high=shape_size_max//2)
+        x_center = rng.integers(simulation_dim)
+        y_center = rng.integers(simulation_dim)
+        z_center = rng.integers(simulation_dim)
 
         # Iterate over the 3D array
         for x in range(max(0, x_center-sphere_radius), min(simulation_dim, x_center+sphere_radius)):
             for y in range(max(0, y_center-sphere_radius), min(simulation_dim, y_center+sphere_radius)):
                 for z in range(max(0, z_center-sphere_radius), min(simulation_dim, z_center+sphere_radius)):
                     # Determine if this point is inside the sphere
                     if (x - x_center) ** 2 + (y - y_center) ** 2 + (z - z_center) ** 2 <= sphere_radius ** 2:
```

### Comparing `qsm-forward-0.8/qsm_forward.egg-info/PKG-INFO` & `qsm-forward-0.9/qsm_forward.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsm-forward
-Version: 0.8
+Version: 0.9
 Summary: A forward-model simulation for Quantitative Susceptibility Mapping
 Home-page: https://github.com/astewartau/qsm-forward-model
 Author: Ashley Stewart
 Author-email: Ashley Stewart <a.stewart.au@gmail.com>
 Project-URL: Homepage, https://github.com/astewartau/qsm-forward-model
 Project-URL: Bug Tracker, https://github.com/astewartau/qsm-forward-model/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `qsm-forward-0.8/setup.py` & `qsm-forward-0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='qsm-forward',
-    version='0.8',
+    version='0.9',
     packages=find_packages(),
     url='https://github.com/astewartau/qsm-forward-model',
     author='Ashley Stewart',
     author_email='a.stewart.au@gmail.com',
     description='A forward-model simulation for Quantitative Susceptibility Mapping',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

