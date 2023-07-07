# Comparing `tmp/resomapper-0.2.1.tar.gz` & `tmp/resomapper-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resomapper-0.2.1.tar", max compression
+gzip compressed data, was "resomapper-0.3.0.tar", max compression
```

## Comparing `resomapper-0.2.1.tar` & `resomapper-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0     2817 2023-05-19 14:13:54.847958 resomapper-0.2.1/LICENSE
--rw-r--r--   0        0        0      857 2023-06-02 08:11:46.996757 resomapper-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2931 2023-05-24 10:04:14.557416 resomapper-0.2.1/README.md
--rw-r--r--   0        0        0      114 2023-05-05 11:04:10.117735 resomapper-0.2.1/resomapper/__init__.py
--rw-r--r--   0        0        0     5560 2023-06-02 07:25:26.661296 resomapper-0.2.1/resomapper/cli.py
--rw-r--r--   0        0        0    25261 2023-05-31 14:19:33.655191 resomapper-0.2.1/resomapper/file_system_functions.py
--rw-r--r--   0        0        0        2 2023-05-11 15:27:12.587903 resomapper-0.2.1/resomapper/myrelax/__init__.py
--rw-r--r--   0        0        0    29416 2023-04-18 15:08:27.862058 resomapper-0.2.1/resomapper/myrelax/getT1TR.py
--rw-r--r--   0        0        0    29826 2023-04-18 15:08:27.862058 resomapper-0.2.1/resomapper/myrelax/getT2T2star.py
--rw-r--r--   0        0        0     7534 2023-06-02 08:09:40.236010 resomapper-0.2.1/resomapper/preprocessing.py
--rw-r--r--   0        0        0    62382 2023-05-31 13:11:18.455517 resomapper-0.2.1/resomapper/processing.py
--rw-r--r--   0        0        0    19972 2023-05-31 10:55:56.176706 resomapper-0.2.1/resomapper/utils.py
--rw-r--r--   0        0        0     3978 1970-01-01 00:00:00.000000 resomapper-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     2817 2023-05-19 14:13:54.847958 resomapper-0.3.0/LICENSE
+-rw-r--r--   0        0        0      867 2023-07-07 08:48:52.387143 resomapper-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2931 2023-05-24 10:04:14.557416 resomapper-0.3.0/README.md
+-rw-r--r--   0        0        0      114 2023-05-05 11:04:10.117735 resomapper-0.3.0/resomapper/__init__.py
+-rw-r--r--   0        0        0     5560 2023-06-02 08:21:40.005388 resomapper-0.3.0/resomapper/cli.py
+-rw-r--r--   0        0        0        0 2023-06-30 10:25:59.647813 resomapper-0.3.0/resomapper/dwi/__init__.py
+-rw-r--r--   0        0        0    12887 2023-06-30 10:25:59.647813 resomapper-0.3.0/resomapper/dwi/adcm.py
+-rw-r--r--   0        0        0    25353 2023-06-30 10:25:59.647813 resomapper-0.3.0/resomapper/file_system_functions.py
+-rw-r--r--   0        0        0        2 2023-05-11 15:27:12.587903 resomapper-0.3.0/resomapper/myrelax/__init__.py
+-rw-r--r--   0        0        0    29416 2023-04-18 15:08:27.862058 resomapper-0.3.0/resomapper/myrelax/getT1TR.py
+-rw-r--r--   0        0        0    29826 2023-04-18 15:08:27.862058 resomapper-0.3.0/resomapper/myrelax/getT2T2star.py
+-rw-r--r--   0        0        0     7534 2023-06-02 08:21:40.021012 resomapper-0.3.0/resomapper/preprocessing.py
+-rw-r--r--   0        0        0    63576 2023-06-30 10:25:59.663437 resomapper-0.3.0/resomapper/processing.py
+-rw-r--r--   0        0        0    19972 2023-06-02 08:21:40.052261 resomapper-0.3.0/resomapper/utils.py
+-rw-r--r--   0        0        0     3979 1970-01-01 00:00:00.000000 resomapper-0.3.0/PKG-INFO
```

### Comparing `resomapper-0.2.1/LICENSE` & `resomapper-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `resomapper-0.2.1/pyproject.toml` & `resomapper-0.3.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "resomapper"
-version = "0.2.1"
+version = "0.3.0"
 description = "Pipeline for processing MR images and generating parametric maps."
 authors = ["Biomedical-MR"]
 license = "MIT"
 readme = "README.md"
 
 packages = [
     { include = "resomapper" }
@@ -17,15 +17,15 @@
 colorama = "^0.4.6"
 dipy = "1.5.0"
 matplotlib = "^3.5.3"
 nibabel = "^4.0.2"
 pandas = "^1.4.4"
 Pillow = "^9.2.0"
 seaborn = "^0.12.0"
-numpy = "^1.23.3"
+numpy = ">=1.23.3, <1.25.0"
 opencv-python = "^4.6.0.66"
 scikit-image = "^0.19.3"
 scikit-learn = "^1.1.2"
 scipy = "^1.9.1"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `resomapper-0.2.1/README.md` & `resomapper-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `resomapper-0.2.1/resomapper/cli.py` & `resomapper-0.3.0/resomapper/cli.py`

 * *Files identical despite different names*

### Comparing `resomapper-0.2.1/resomapper/file_system_functions.py` & `resomapper-0.3.0/resomapper/file_system_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -460,15 +460,15 @@
             return "MT"
         else:
             return "M0"
 
     def get_selected_studies(self):
         """Returns those studies that will be processed. Checks if a modality
         has alredy been processed. In that case gives two options:
-            - Remove it and processed again
+            - Remove it and process it again.
             - Do not process it again.
 
         Returns:
             subfolders_paths (list): Paths to modality subfolders to be processed.
             modals_to_process (list): Modalities present in the studies to process.
         """
 
@@ -482,57 +482,57 @@
             # check if a modality has to be processed
             processed_modal = self.get_modality(subfolder)
             for modal in self.modals_to_process:
                 if modal == processed_modal:
                     if (
                         (("ADC_map.nii" in os.listdir(subfolder)) and modal == "DT")
                         or (("mapas" in os.listdir(subfolder)) and fnmatch(modal, "T*"))
-                        or (
-                            ("MT_map" in str([f for f in os.walk(subfolder)]))
-                            and modal == "MT"
-                        )
+                        or ("MT_map" in str(list(os.walk(subfolder))) and modal == "MT")
                     ):
                         patient = "_".join(subfolder.parts[-2].split("_")[1:])
                         msg = (
                             f"La modalidad {processed_modal} del estudio {patient} ya "
                             "ha sido procesada.\n¿Desea volver a procesarla?"
                         )
-                        avoid_subfolder = ut.ask_user(msg)
-                        if avoid_subfolder:  # if process again
+                        process_again = ut.ask_user(msg)
+                        if process_again:  # if process again
                             ready = ""
                             while ready != "y":
                                 msg = (
                                     f"\n{hmg.warn}El resultado del procesamiento "
                                     f"anterior de {processed_modal} del estudio "
                                     f"{patient} no se conservará.\n"
                                     f"\n{hmg.ask}Si desea guardarlo debe hacerlo ahora."
                                     f' Pulse "y" para continuar.\n{hmg.pointer}'
                                 )
                                 ready = input(msg)
                                 ready = ready.lower()
+                    else:
+                        process_again = True
 
-                    # remove folder and files contained in it
-                    shutil.rmtree(str(subfolder))
-                    # create folder again
-                    # src_path = Path(
-                    #     str(subfolder)
-                    #     .replace("procesados", "convertidos")
-                    #     .replace("procesado", "convertido")
-                    # )
-                    files_to_transfer = self.get_converted_files([processed_modal])
-                    dst_paths = [
-                        Path(
-                            str(f)
-                            .replace("convertidos", "procesados")
-                            .replace("convertido", "procesado")
-                        )
-                        for f in files_to_transfer
-                    ]
-                    self.transfer_files(files_to_transfer, dst_paths)
-                    subfolders_paths.append(subfolder)
+                    if process_again:
+                        # remove folder and files contained in it
+                        shutil.rmtree(str(subfolder))
+                        # create folder again
+                        # src_path = Path(
+                        #     str(subfolder)
+                        #     .replace("procesados", "convertidos")
+                        #     .replace("procesado", "convertido")
+                        # )
+                        files_to_transfer = self.get_converted_files([processed_modal])
+                        dst_paths = [
+                            Path(
+                                str(f)
+                                .replace("convertidos", "procesados")
+                                .replace("convertido", "procesado")
+                            )
+                            for f in files_to_transfer
+                        ]
+                        self.transfer_files(files_to_transfer, dst_paths)
+                        subfolders_paths.append(subfolder)
 
         return subfolders_paths, self.modals_to_process
 
 
 ###############################################################################
 # From Bruker to Nifti format
 ###############################################################################
```

### Comparing `resomapper-0.2.1/resomapper/myrelax/getT1TR.py` & `resomapper-0.3.0/resomapper/myrelax/getT1TR.py`

 * *Files identical despite different names*

### Comparing `resomapper-0.2.1/resomapper/myrelax/getT2T2star.py` & `resomapper-0.3.0/resomapper/myrelax/getT2T2star.py`

 * *Files identical despite different names*

### Comparing `resomapper-0.2.1/resomapper/preprocessing.py` & `resomapper-0.3.0/resomapper/preprocessing.py`

 * *Files identical despite different names*

### Comparing `resomapper-0.2.1/resomapper/processing.py` & `resomapper-0.3.0/resomapper/processing.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 import numpy as np
 import seaborn as sns
 from dipy.core.gradients import gradient_table
 from dipy.core.sphere import Sphere
 from dipy.io.gradients import read_bvals_bvecs
 from dipy.io.image import load_nifti, save_nifti
 from dipy.reconst.dti import (
-    _nlls_err_func,
     apparent_diffusion_coef,
     fractional_anisotropy,
 )
 
+import resomapper.dwi.adcm as adcm
 from resomapper.myrelax import getT1TR, getT2T2star
 from resomapper.utils import Headermsg as hmg
-from resomapper.utils import ask_user, check_shapes
+from resomapper.utils import ask_user, ask_user_options, check_shapes
 
 warnings.filterwarnings("ignore")
 
 
 ###############################################################################
 # MT PROCESSING
 ###############################################################################
@@ -301,15 +301,15 @@
             valid_n_dirs = False
             while not valid_n_dirs:
                 if n_dirs > n_dirs_real:
                     while True:
                         try:
                             print(
                                 "\nPrueba otra vez. Debes intruducir un valor "
-                                f"menor o igual a {n_dirs_real}."
+                                f"menor o igual a {n_dirs_real}.\n"
                             )
                             n_dirs = int(
                                 input(
                                     f"{hmg.ask}¿Número de direcciones?\n{hmg.pointer}"
                                 )
                             )
                             break
@@ -427,43 +427,14 @@
             dirs = np.loadtxt(src_dirs)
             print(f"{hmg.info}Mostrado direcciones del archivo métodos.\n")
             print(dirs, "\n")
 
         dirs = dirs.T
         return [b_vals, dirs, n_b_val, n_basal, n_dirs, indexes_to_rm]
 
-    def get_residuals(self, design_matrix, data, weighting=None, sigma=None, jac=True):
-        """Computes non-liear least squares per each pixel and returns a map
-        of residual errors.  It uses ordinary least squares (OLS) as starting
-        point for optimization. The residual error is obtained per direction
-        and per b value, including basal images (b=0)."""
-
-        # preparing data
-        data[data == 0] = 1
-        r_data = data.reshape((-1, data.shape[-1]))  # vectorize data
-
-        # OLS parameters are used as the starting point for optimization
-        log_s = np.log(r_data)
-        inv_design = np.linalg.pinv(design_matrix)
-        ols_params = np.dot(inv_design, log_s.T).T
-
-        # iterate over each voxel and compute non linear least squares error function
-        residuals = np.empty((r_data.shape[0], data.shape[3]))
-        for vox in range(r_data.shape[0]):
-            start_params = ols_params[vox]  # 7 params per voxel
-            if jac:
-                # Error func for the non-linear least-squares fit of the tensor.
-                residuals[vox] = _nlls_err_func(
-                    start_params, design_matrix, r_data[vox], weighting, sigma
-                )
-        # reshape to the original shape
-        residuals.shape = data.shape[:]
-
-        return residuals
-
     def compute_map(self, map_type: str):
         unit_change = 1_000_000
 
         if map_type == "AD":
             pmap = self.tensor.ad * unit_change
             pmap[pmap < 0.00000001] = float("nan")
         elif map_type == "RD":
@@ -561,226 +532,287 @@
             data[:, :, :, i] = data[:, :, :, i] * mask
 
         # read b values (bvals) and gradient directions (bvecs)
         bval_path = str(self.study_path / "bvalues.bval")
         bvec_path = str(self.study_path / "Bdirs.bvec")
         bvals, bvecs = read_bvals_bvecs(bval_path, bvec_path)
 
-        # create gradient table. You can access gradients with gtab.gradients
-        gtab = gradient_table(bvals, bvecs, atol=1e-0)
-        # gtab contains bvec and bvals, such as
-        # -0.066   0.9937   -0.089   421.46    Gradient direction and b_val_1
-        # -0.066   0.9937   -0.089   1827.43   Gradient direction and b_val_2
-        #   ...      ...      ...      ...
-
-        print(f"\n{hmg.info}Se está resolviendo el tensor. Puede tardar unos segundos.")
-        tensor_model = dti.TensorModel(gtab, fit_method="NLLS")
-
-        tensor_fit = tensor_model.fit(data)
-        self.tensor = tensor_fit
-        # Some documentation of tensor_model and tensor_fit
-        # tensor_model.design_matrix:
-        #   np.array with shape (n_basals + n_b_val*n_dirs, 6 + 1).
-        #   Matrix with bi[gxi^2, gyi^2, gzi^2, 2*gxi*gyi, 2*gxi*gzi, 2*gyi*gzi, -1],
-        #   with g values obtained from gtab.bvecs corresponding with gradient
-        #   directions and bi are the b values obtained from gtab.bvals
-        # tensor_model.gtab
-        #   gtab contains bvec and bvals
-        # tensor_fit.evals
-        #   np.array with shape (x_dim, y_dim, n_slices, 3) offers 3 eigenvalues
-        #   per pixel sorted from the biggest to the smallest.
-        # tensor_fit.evecs
-        #   np.array with shape (x_dim, y_dim, n_slices, 3, 3) offers 3
-        #   eigenvectors per pixel. Each eigenvector has x, y, z directions,
-        #   so we have a 3-by-3 matrix per pixel. First row corresponds with
-        #   the biggest eigenvalue, and so on.
-        # tensor_fit.directions
-        #   np.array with shape (x_dim, y_dim, n_slices, 1, 3) offers the main
-        #   direction of each pixel, according to the biggest eigenvalue
-        # tensor_fit.model
-        #   access to tensor_model
-        # tensor_fit.quadratic_form
-        #   returns np.array of shape (x_dim, y_dim, n_slices, 3, 3).
-        #   Calculates the 3-by-3 diffusion tensor for each voxel.
-
-        # get ADC maps
-        print(f"\n{hmg.info}Se está generando el mapa ADC.")
-        my_sphere = Sphere(xyz=gtab.bvecs[~gtab.b0s_mask])
-        ADC_maps = apparent_diffusion_coef(tensor_fit.quadratic_form, my_sphere)
-
-        # ADC matrix has an adc value per bval and direction. For example,
-        # for 2 bvals and 15 directions ADC matrix will have 2*15 adc values per
-        # pixel. Actually, an adc value is the same as the slope of the straight
-        # line that adjust to the ln(S/S0) values at different b values. Then,
-        # the adc is different per direction, not per b value. Considering an
-        # adc value per b value has no sense. Thus, we only need one adc per
-        # direction.
-        if n_b_val > 1:
-            leap = [*range(1, n_dirs * n_b_val, n_b_val)]
-            ADC_maps = ADC_maps[:, :, :, leap]
+        if n_dirs < 6:
+            print(
+                f"\n{hmg.warn}Para imágenes de menos de 6 direcciones no se puede "
+                "ajustar el modelo de DTI. Se va a realizar el ajuste monoexponencial "
+                "de ADC."
+            )
 
-        unit_change = 1_000_000
-        ADC_maps = ADC_maps * unit_change
-        ADC_maps[ADC_maps < 0.00000001] = float("nan")
-        save_nifti(
-            str(self.study_path / "ADC_map"), ADC_maps.astype(np.float32), affine
-        )
+            question = "Elige el modelo que deseas ajustar."
+            options = {
+                "m": "Ajuste monoexponencial.",
+                "l": "Ajuste lineal.",
+            }
+            selected_model = ask_user_options(question, options)
+
+            print(f"\n{hmg.info}Ajustando el modelo... Puede tardar unos segundos.")
+            adcm_map, s0_map, residuals, prediction = adcm.fit_volume(
+                bvals, n_basal, n_b_val, n_dirs, data, selected_model
+            )
+            adcm_map_scaled = adcm_map * 1_000_000
+            save_nifti(
+                str(self.study_path / "ADC_map"),
+                adcm_map_scaled.astype(np.float32),
+                affine,
+            )
+            # save_nifti(
+            #     str(self.study_path / "s0_map"), s0_map.astype(np.float32), affine
+            # )
+            # save_nifti(
+            #     str(self.study_path / "res_map"), residuals.astype(np.float32), affine
+            # )
+            # save_nifti(
+            #     str(self.study_path / "pred_signal"),
+            #     prediction.astype(np.float32),
+            #     affine,
+            # )
 
-        # compute R^2 error maps
-        # design matrix computed as:
-        #   bi[gxi^2, gyi^2, gzi^2, 2*gxi*gyi, 2*gxi*gzi, 2*gyi*gzi, -1],
-        # and -1 will be multiplied by ln(S0)
+            R2_maps = []
+            print(f"\n{hmg.info}Generando mapas de R\u00b2.")
 
-        # design_matrix = tensor_model.design_matrix
+            for d in range(n_dirs):
+                # compute R^2 maps
+                i_dir = n_basal + d * n_b_val
+                R2_map = R2MapGenerator().get_R2_map(
+                    data[:, :, :, i_dir : i_dir + n_b_val],
+                    residuals=residuals[:, :, :, d : d + n_b_val],
+                )
+                R2_dir_path = self.study_path / f"Dir_{str(d + 1)}"
+                R2_dir_path.mkdir(parents=True)
+                save_nifti(R2_dir_path / "R2_map", R2_map.astype(np.float32), affine)
+                R2_maps.append(R2_map)
 
-        # get errors between the real signal and the predicted signal per our model
+            R2_maps_ordered = np.moveaxis(np.array(R2_maps), 0, -1)
+            save_nifti(
+                self.study_path / "R2_map",
+                R2_maps_ordered,
+                affine,
+            )
 
-        # residuals = self.get_residuals(design_matrix, data)
+            if ask_user("¿Deseas ver los resultados de las curvas de ajuste?"):
+                adcm.show_fitting_adc(
+                    adcm_map,
+                    s0_map,
+                    data,
+                    bvals,
+                    selected_model,
+                    n_basal,
+                    n_b_val,
+                    R2_maps_ordered,
+                )
 
-        # get basal information
-        # basal_residuals = residuals[:, :, :, 0:n_basal]
-        # basal_data = data[:, :, :, 0:n_basal]
+            # ask if filtering is desired
+            apply_filter = ask_user("¿Quieres usar el filtro de ajuste?")
 
-        # get the signal predicted by the fitted DTI model
-        # the predicted signal is normalized, as it is divided by S0
-        predicted_signal = tensor_fit.predict(gtab)
+            # select threshold and create R^2 maps
+            if apply_filter:
+                # get R2 maps and apply threshold to them to get the masks/filters
+                R2_map_paths = list(self.study_path.glob("Dir_*/*"))
+                f_R2_maps = []
+
+                th = R2MapGenerator().select_threshold()
+                for R2_map_path in R2_map_paths:
+                    # f_R2_map shape: (x_dim, y_dim, n_slices)
+                    f_R2_map = R2MapGenerator().get_filtered_R2(R2_map_path, "DTI", th)
+                    f_R2_maps.append(
+                        f_R2_map
+                    )  # filtered R2 maps for all gradient directions
+            else:
+                f_R2_maps = np.ones(np.shape(R2_maps))
+                f_R2_maps_slc = None
 
-        # s0 is the average of the basal images (no diffusion gradient)
-        s0 = np.mean(data[:, :, :, :n_basal], axis=3)
+            # save adc filtered heatmaps
+            f_ADC_maps = np.rollaxis(adcm_map_scaled, axis=3) * np.array(f_R2_maps)
+            vmin, vmax, cmap = Heatmap().save_ADC_heatmap(f_ADC_maps, self.study_path)
 
-        # normalize our original image dividing by s0
-        norm_data = np.zeros(data.shape)
-        for i in range(data.shape[2]):
-            for j in range(data.shape[3]):
-                norm_data[:, :, i, j] += data[:, :, i, j] / s0[:, :, i]
+        else:
+            # create gradient table. You can access gradients with gtab.gradients
+            gtab = gradient_table(bvals, bvecs, atol=1e-0)
+            # gtab contains bvec and bvals, such as
+            # -0.066   0.9937   -0.089   421.46    Gradient direction and b_val_1
+            # -0.066   0.9937   -0.089   1827.43   Gradient direction and b_val_2
+            #   ...      ...      ...      ...
 
-        # get residuals: difference between real data and predicted data
-        residuals = norm_data - predicted_signal
+            print(
+                f"\n{hmg.info}Se está resolviendo el tensor. "
+                "Puede tardar unos segundos."
+            )
+            # Estimation of S0 needs to be returned for calculating r2 maps later
+            tensor_model = dti.TensorModel(gtab, fit_method="NLLS", return_S0_hat=True)
 
-        R2_maps = []
-        print(f"\n{hmg.info}Generando mapas de R\u00b2.")
-        if n_b_val > 1:
-            for d in range(n_dirs):
-                # residuals
-                # dir_res = residuals[
-                #     :, :, :, (leap[d] + 1) : ((leap[d]) + (1 + n_b_val))
-                # ]
-                # full_res = np.concatenate((basal_residuals, dir_res), axis=-1)
-
-                # # data
-                # dir_data = data[:, :, :, (leap[d] + 1) : ((leap[d]) + (1 + n_b_val))]
-                # # concatenates basals with directions
-                # full_data = np.concatenate((basal_data, dir_data), axis=-1)
+            tensor_fit = tensor_model.fit(data)
+            self.tensor = tensor_fit
+            # Some documentation of tensor_model and tensor_fit
+            # tensor_model.design_matrix:
+            #   np.array with shape (n_basals + n_b_val*n_dirs, 6 + 1).
+            #   Matrix with bi[gxi^2, gyi^2, gzi^2, 2*gxi*gyi, 2*gxi*gzi, 2*gyi*gzi, -1]
+            #   with g values obtained from gtab.bvecs corresponding with gradient
+            #   directions and bi are the b values obtained from gtab.bvals
+            # tensor_model.gtab
+            #   gtab contains bvec and bvals
+            # tensor_fit.evals
+            #   np.array with shape (x_dim, y_dim, n_slices, 3) offers 3 eigenvalues
+            #   per pixel sorted from the biggest to the smallest.
+            # tensor_fit.evecs
+            #   np.array with shape (x_dim, y_dim, n_slices, 3, 3) offers 3
+            #   eigenvectors per pixel. Each eigenvector has x, y, z directions,
+            #   so we have a 3-by-3 matrix per pixel. First row corresponds with
+            #   the biggest eigenvalue, and so on.
+            # tensor_fit.directions
+            #   np.array with shape (x_dim, y_dim, n_slices, 1, 3) offers the main
+            #   direction of each pixel, according to the biggest eigenvalue
+            # tensor_fit.model
+            #   access to tensor_model
+            # tensor_fit.quadratic_form
+            #   returns np.array of shape (x_dim, y_dim, n_slices, 3, 3).
+            #   Calculates the 3-by-3 diffusion tensor for each voxel.
+
+            # get ADC maps
+            print(f"\n{hmg.info}Se está generando el mapa ADC.")
+            my_sphere = Sphere(xyz=gtab.bvecs[~gtab.b0s_mask])
+            ADC_maps = apparent_diffusion_coef(tensor_fit.quadratic_form, my_sphere)
+
+            # ADC matrix has an adc value per bval and direction. For example,
+            # for 2 bvals and 15 directions ADC matrix will have 2*15 adc values per
+            # pixel. Actually, an adc value is the same as the slope of the straight
+            # line that adjust to the ln(S/S0) values at different b values. Then,
+            # the adc is different per direction, not per b value. Considering an
+            # adc value per b value has no sense. Thus, we only need one adc per
+            # direction.
+            if n_b_val > 1:
+                leap = [*range(1, n_dirs * n_b_val, n_b_val)]
+                ADC_maps = ADC_maps[:, :, :, leap]
+
+            unit_change = 1_000_000
+            ADC_maps = ADC_maps * unit_change
+            ADC_maps[ADC_maps < 0.00000001] = float("nan")
+            save_nifti(
+                str(self.study_path / "ADC_map"), ADC_maps.astype(np.float32), affine
+            )
 
-                # compute R^2 maps
-                R2_map = R2MapGenerator().get_R2_map(norm_data, residuals)
-                R2_dir_path = self.study_path / ("Dir_" + str(d + 1))
-                R2_dir_path.mkdir(parents=True)
-                save_nifti(R2_dir_path / "R2_map", R2_map.astype(np.float32), affine)
-                R2_maps.append(R2_map)
+            # get the signal predicted by the fitted DTI model
+            predicted_signal = tensor_fit.predict(gtab)
+            # save_nifti(
+            #     str(self.study_path / "pred_signal"),
+            #     predicted_signal.astype(np.float32),
+            #     affine,
+            # )
 
-                # save_nifti(
-                #     R2_dir_path / "norm_data", norm_data.astype(np.float32), affine
-                # )
-                # save_nifti(R2_dir_path / "data", data.astype(np.float32), affine)
-                # save_nifti(R2_dir_path / "s0mean", s0.astype(np.float32), affine)
-                # save_nifti(
-                #     R2_dir_path / "residuals", residuals.astype(np.float32), affine
-                # )
-                # save_nifti(
-                #     R2_dir_path / "pred", predicted_signal.astype(np.float32), affine
-                # )
+            residuals = data - predicted_signal
 
-        else:
-            for d in range(ADC_maps.shape[3]):
-                # dir_res = residuals[:, :, :, (n_basal + d)]
-                # # add new axis to keep dimensions consistent
-                # dir_res = dir_res[:, :, :, np.newaxis]
-                # full_res = np.concatenate((basal_residuals, dir_res), axis=-1)
-
-                # dir_data = data[:, :, :, (n_basal + d)]
-                # dir_data = dir_data[:, :, :, np.newaxis]
-                # full_data = np.concatenate((basal_data, dir_data), axis=-1)
+            R2_maps = []
+            print(f"\n{hmg.info}Generando mapas de R\u00b2.")
 
-                R2_map = R2MapGenerator().get_R2_map(norm_data, residuals)
-                R2_dir_path = self.study_path / ("Dir_" + str(d + 1))
+            for d in range(n_dirs):
+                # compute R^2 maps
+                i_dir = n_basal + d * n_b_val
+                R2_map = R2MapGenerator().get_R2_map(
+                    data[:, :, :, i_dir : i_dir + n_b_val],
+                    residuals[:, :, :, i_dir : i_dir + n_b_val],
+                )
+                R2_map[mask == 0] = np.nan
+                R2_dir_path = self.study_path / f"Dir_{str(d + 1)}"
                 R2_dir_path.mkdir(parents=True)
                 save_nifti(R2_dir_path / "R2_map", R2_map.astype(np.float32), affine)
                 R2_maps.append(R2_map)
 
-        # ask if filtering is desired
-        apply_filter = ask_user("¿Quieres usar el filtro de ajuste?")
+            save_nifti(
+                self.study_path / "R2_map",
+                np.moveaxis(np.array(R2_maps), 0, -1),
+                affine,
+            )
 
-        # select threshold and create R^2 maps
-        if apply_filter:
-            # get R2 maps and apply threshold to them to get the masks/filters
-            R2_map_paths = list(self.study_path.glob("Dir_*/*"))
-            f_R2_maps = []
-
-            th = R2MapGenerator().select_threshold()
-            for R2_map_path in R2_map_paths:
-                # f_R2_map shape: (x_dim, y_dim, n_slices)
-                f_R2_map = R2MapGenerator().get_filtered_R2(R2_map_path, "DTI", th)
-                f_R2_maps.append(
-                    f_R2_map
-                )  # filtered R2 maps for all gradient directions
-        else:
-            f_R2_maps = np.ones(np.shape(R2_maps))
-            f_R2_maps_slc = None
+            # ask if filtering is desired
+            apply_filter = ask_user("¿Quieres usar el filtro de ajuste?")
 
-        # save adc filtered heatmaps
-        f_ADC_maps = np.rollaxis(ADC_maps, axis=3) * np.array(f_R2_maps)
-        vmin, vmax, cmap = Heatmap().save_ADC_heatmap(f_ADC_maps, self.study_path)
-
-        # Getting a map per slice requires to have one R^2 map per slice
-        if apply_filter:
-            f_R2_maps_slc = np.multiply.reduce(f_R2_maps, axis=0)
-
-        self.f_R2_maps_slc = f_R2_maps_slc
-
-        # mean diffusivity
-        print(f"\n{hmg.info}Generando mapas de MD.")
-        MD_map = self.compute_map("MD")
-        md_saving_path = str(self.study_path / "MD")
-        os.makedirs(md_saving_path)
-        save_nifti(
-            os.path.join(md_saving_path, "MD_map"), MD_map.astype(np.float32), affine
-        )
-        Heatmap().save_heatmap(MD_map, "MD", md_saving_path, vmin, vmax, cmap)
+            # select threshold and create R^2 maps
+            if apply_filter:
+                # get R2 maps and apply threshold to them to get the masks/filters
+                R2_map_paths = list(self.study_path.glob("Dir_*/*"))
+                f_R2_maps = []
+
+                th = R2MapGenerator().select_threshold()
+                for R2_map_path in R2_map_paths:
+                    # f_R2_map shape: (x_dim, y_dim, n_slices)
+                    f_R2_map = R2MapGenerator().get_filtered_R2(R2_map_path, "DTI", th)
+                    f_R2_maps.append(
+                        f_R2_map
+                    )  # filtered R2 maps for all gradient directions
+            else:
+                f_R2_maps = np.ones(np.shape(R2_maps))
+                f_R2_maps_slc = None
 
-        # axial diffusivity
-        print(f"\n{hmg.info}Generando mapas de AD.")
-        AD_map = self.compute_map("AD")
-        AD_saving_path = str(self.study_path / "AD")
-        os.makedirs(AD_saving_path)
-        save_nifti(
-            os.path.join(AD_saving_path, "AD_map"), AD_map.astype(np.float32), affine
-        )
-        Heatmap().save_heatmap(AD_map, "AD", AD_saving_path, vmin, vmax, cmap)
+            # save adc filtered heatmaps
+            f_ADC_maps = np.rollaxis(ADC_maps, axis=3) * np.array(f_R2_maps)
+            vmin, vmax, cmap = Heatmap().save_ADC_heatmap(f_ADC_maps, self.study_path)
+
+            # Getting a map per slice requires to have one R^2 map per slice
+            if apply_filter:
+                f_R2_maps_slc = np.multiply.reduce(f_R2_maps, axis=0)
+
+            self.f_R2_maps_slc = f_R2_maps_slc
+
+            if n_dirs >= 6:
+                # mean diffusivity
+                print(f"\n{hmg.info}Generando mapas de MD.")
+                MD_map = self.compute_map("MD")
+                md_saving_path = str(self.study_path / "MD")
+                os.makedirs(md_saving_path)
+                save_nifti(
+                    os.path.join(md_saving_path, "MD_map"),
+                    MD_map.astype(np.float32),
+                    affine,
+                )
+                Heatmap().save_heatmap(MD_map, "MD", md_saving_path, vmin, vmax, cmap)
 
-        # radial diffusivity
-        print(f"\n{hmg.info}Generando mapas de RD.")
-        RD_map = self.compute_map("RD")
-        RD_saving_path = str(self.study_path / "RD")
-        os.makedirs(RD_saving_path)
-        save_nifti(
-            os.path.join(RD_saving_path, "RD_map"), RD_map.astype(np.float32), affine
-        )
-        Heatmap().save_heatmap(RD_map, "RD", RD_saving_path, vmin, vmax, cmap)
+                # axial diffusivity
+                print(f"\n{hmg.info}Generando mapas de AD.")
+                AD_map = self.compute_map("AD")
+                AD_saving_path = str(self.study_path / "AD")
+                os.makedirs(AD_saving_path)
+                save_nifti(
+                    os.path.join(AD_saving_path, "AD_map"),
+                    AD_map.astype(np.float32),
+                    affine,
+                )
+                Heatmap().save_heatmap(AD_map, "AD", AD_saving_path, vmin, vmax, cmap)
 
-        # fractional anisotropy
-        # formula: https://dipy.org/documentation/1.0.0./examples_built/reconst_dti/
-        print(f"\n{hmg.info}Generando mapas de FA.")
-        FA_map = self.compute_map("FA")
-        FA_saving_path = str(self.study_path / "FA")
-        os.makedirs(FA_saving_path)
-        save_nifti(
-            os.path.join(FA_saving_path, "FA_map"), FA_map.astype(np.float32), affine
-        )
-        Heatmap().save_heatmap(FA_map, "FA", FA_saving_path)
+                # radial diffusivity
+                print(f"\n{hmg.info}Generando mapas de RD.")
+                RD_map = self.compute_map("RD")
+                RD_saving_path = str(self.study_path / "RD")
+                os.makedirs(RD_saving_path)
+                save_nifti(
+                    os.path.join(RD_saving_path, "RD_map"),
+                    RD_map.astype(np.float32),
+                    affine,
+                )
+                Heatmap().save_heatmap(RD_map, "RD", RD_saving_path, vmin, vmax, cmap)
+
+                # fractional anisotropy
+                # formula: https://dipy.org/documentation/1.0.0./examples_built/reconst_dti/
+                print(f"\n{hmg.info}Generando mapas de FA.")
+                FA_map = self.compute_map("FA")
+
+                FA_map[mask == 0] = np.nan
+
+                FA_saving_path = str(self.study_path / "FA")
+                os.makedirs(FA_saving_path)
+                save_nifti(
+                    os.path.join(FA_saving_path, "FA_map"),
+                    FA_map.astype(np.float32),
+                    affine,
+                )
+                Heatmap().save_heatmap(FA_map, "FA", FA_saving_path)
 
 
 ###############################################################################
 # T1/T2/T2E PROCESSING
 ###############################################################################
 class TimeCollector:
     def __init__(
@@ -824,28 +856,27 @@
             print(f"{hmg.error}El directorio no existe.")
 
     def write_times(self, times: list, file_name: str, subfolder: str):
         """Write times, overwritting if file alredy exists."""
 
         file_path = self.root_path / subfolder / file_name
         with open(file_path, "w") as f:
-            f.write(" ".join([t for t in times]))
+            f.write(" ".join(list(times)))
 
         return file_path
 
     def get_times_auto(self):
         """Read times (TR, TE, TEs) automatically from method.txt files
         located in T1, T2, T2* subfolders.
 
-        Returns
-        -------
-        times_paths: list
-            Contains TR in position 0, TE in position 1, and TEs in position 2.
-            It has to be in this way as other functions expect a varible with
-            times in this particular structure."""
+        Returns:
+            list: times_paths. Contains TR in position 0, TE in position 1, and TEs in
+            position 2. It has to be in this way as other functions expect a varible
+            with times in this particular structure.
+        """
 
         times_paths = {}  # empty dictionary that will store times
         for subfolder in self.studies_to_process:
             study_name = subfolder.parts[-1]
             if (
                 study_name.startswith("T1_")
                 and "T1" in self.modals_to_process
@@ -1306,21 +1337,25 @@
             plt.close()
         else:
             fig.show()
 
     def save_ADC_heatmap(self, f_ADC_maps: np.array, study_path: str):
         """Save ADC heatmap. Opens a window to show the heatmaps per slice
         and allows to change color range and color map.
-        Parameters
-        ----------
-        f_ADC_maps : np.array
-            Includes filtered ADC directions.
-        study_path : Path
-            Path to study folder.
+
+        Args:
+            f_ADC_maps (np.array): Includes filtered ADC directions.
+            study_path (str): Path to study folder.
+
+        Returns:
+            float: vmin. Minimum value for the color scale.
+            float: vmax. Maximum value for the color scale.
+            str: cmap. Color scale name.
         """
+
         f_ADC_maps[f_ADC_maps == 0.0] = np.nan
 
         cmap = plt.cm.turbo  # select default cmap
         # cmap.set_bad("black", 1)  # paints NaN values in black
         vmin = 0.1 * np.nanmax(f_ADC_maps) + np.nanmin(f_ADC_maps)
         vmax = 0.9 * np.nanmax(f_ADC_maps)
```

### Comparing `resomapper-0.2.1/resomapper/utils.py` & `resomapper-0.3.0/resomapper/utils.py`

 * *Files identical despite different names*

### Comparing `resomapper-0.2.1/PKG-INFO` & `resomapper-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resomapper
-Version: 0.2.1
+Version: 0.3.0
 Summary: Pipeline for processing MR images and generating parametric maps.
 License: MIT
 Author: Biomedical-MR
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -14,15 +14,15 @@
 Requires-Dist: Pillow (>=9.2.0,<10.0.0)
 Requires-Dist: bruker2nifti (==1.0.4)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: dipy (==1.5.0)
 Requires-Dist: matplotlib (>=3.5.3,<4.0.0)
 Requires-Dist: nibabel (>=4.0.2,<5.0.0)
-Requires-Dist: numpy (>=1.23.3,<2.0.0)
+Requires-Dist: numpy (>=1.23.3,<1.25.0)
 Requires-Dist: opencv-python (>=4.6.0.66,<5.0.0.0)
 Requires-Dist: pandas (>=1.4.4,<2.0.0)
 Requires-Dist: scikit-image (>=0.19.3,<0.20.0)
 Requires-Dist: scikit-learn (>=1.1.2,<2.0.0)
 Requires-Dist: scipy (>=1.9.1,<2.0.0)
 Requires-Dist: seaborn (>=0.12.0,<0.13.0)
 Description-Content-Type: text/markdown
```

