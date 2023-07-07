# Comparing `tmp/osl-dynamics-1.2.4.tar.gz` & `tmp/osl-dynamics-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osl-dynamics-1.2.4.tar", last modified: Wed Jun 28 11:56:25 2023, max compression
+gzip compressed data, was "osl-dynamics-1.2.5.tar", last modified: Fri Jul  7 12:52:56 2023, max compression
```

## Comparing `osl-dynamics-1.2.4.tar` & `osl-dynamics-1.2.5.tar`

### file list

```diff
@@ -1,194 +1,191 @@
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-06-28 11:56:25.024306 osl-dynamics-1.2.4/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     4561 2023-06-28 11:56:25.024640 osl-dynamics-1.2.4/PKG-INFO
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     4248 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/README.rst
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-06-28 11:56:23.710602 osl-dynamics-1.2.4/osl_dynamics/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      643 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/__init__.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-06-28 11:56:23.844957 osl-dynamics-1.2.4/osl_dynamics/analysis/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      250 2023-05-09 14:36:05.000000 osl-dynamics-1.2.4/osl_dynamics/analysis/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    27101 2023-06-22 11:45:55.000000 osl-dynamics-1.2.4/osl_dynamics/analysis/connectivity.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6437 2023-05-09 14:35:55.000000 osl-dynamics-1.2.4/osl_dynamics/analysis/fisher_kernel.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6165 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/analysis/gmm.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    25514 2023-06-22 15:05:16.000000 osl-dynamics-1.2.4/osl_dynamics/analysis/modes.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    20303 2023-06-26 18:57:47.000000 osl-dynamics-1.2.4/osl_dynamics/analysis/power.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     3268 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/analysis/regression.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    46846 2023-06-22 08:42:10.000000 osl-dynamics-1.2.4/osl_dynamics/analysis/spectral.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     7487 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/analysis/static.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     8486 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/analysis/statistics.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    29690 2023-06-08 09:36:36.000000 osl-dynamics-1.2.4/osl_dynamics/analysis/tinda.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5688 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/analysis/workbench.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    10899 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/array_ops.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-06-28 11:56:23.876316 osl-dynamics-1.2.4/osl_dynamics/config_api/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      895 2023-06-19 18:50:42.000000 osl-dynamics-1.2.4/osl_dynamics/config_api/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5896 2023-06-19 18:50:42.000000 osl-dynamics-1.2.4/osl_dynamics/config_api/pipeline.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    56168 2023-06-22 15:05:16.000000 osl-dynamics-1.2.4/osl_dynamics/config_api/wrappers.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-06-28 11:56:23.952554 osl-dynamics-1.2.4/osl_dynamics/data/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      112 2023-06-28 08:10:13.000000 osl-dynamics-1.2.4/osl_dynamics/data/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    37114 2023-06-26 18:57:47.000000 osl-dynamics-1.2.4/osl_dynamics/data/base.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6757 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/data/processing.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     8574 2023-05-10 09:37:57.000000 osl-dynamics-1.2.4/osl_dynamics/data/rw.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2809 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/data/spm.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2447 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/data/task.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     4726 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/data/tf.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-06-28 11:56:23.970040 osl-dynamics-1.2.4/osl_dynamics/files/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      883 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      434 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/functions.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-06-28 11:56:24.092386 osl-dynamics-1.2.4/osl_dynamics/files/mask/
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)     7241 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/mask/MNI152_T1_8mm_brain.nii.gz
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   724726 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/mask/ParcellationPilot.L.inflated.32k_fs_LR.surf.gii
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   723434 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/mask/ParcellationPilot.L.midthickness.32k_fs_LR.surf.gii
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   723505 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/mask/ParcellationPilot.L.very_inflated.32k_fs_LR.surf.gii
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   713031 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/mask/ParcellationPilot.R.inflated.32k_fs_LR.surf.gii
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   710727 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/mask/ParcellationPilot.R.midthickness.32k_fs_LR.surf.gii
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   712178 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/mask/ParcellationPilot.R.very_inflated.32k_fs_LR.surf.gii
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     1649 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/mask/__init__.py
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)      971 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/mask/ft_8mm_brain_mask.nii.gz
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-06-28 11:56:24.186442 osl-dynamics-1.2.4/osl_dynamics/files/parcellation/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    41373 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/parcellation/Glasser50_space-MNI152NLin6_res-8x8x8.nii.gz
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     9131 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/parcellation/Glasser52_binary_space-MNI152NLin6_res-8x8x8.nii.gz
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      669 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/parcellation/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    36166 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/parcellation/aal_cortical_merged_8mm_stacked.nii.gz
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)    23705 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/parcellation/fMRI_parcellation_ds8mm.nii.gz
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    24111 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_3PCC_ips_reduced_2mm_ss5mm_ds8mm.nii.gz
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    33885 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_3PCC_ips_reduced_2mm_ss5mm_ds8mm_adj.nii.gz
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)    23705 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_reduced_2mm_ss5mm_ds8mm.nii.gz
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)    63185 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_tighterMay15_v2_6mm_exclusive.nii.gz
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)    63835 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_tighterMay15_v2_8mm.nii.gz
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)     5233 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/parcellation/giles_39_binary.nii.gz
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-06-28 11:56:24.210483 osl-dynamics-1.2.4/osl_dynamics/files/scanner/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      268 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5568 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/ctf275_channel_names.npy
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-06-28 11:56:24.684585 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6679 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/4D148.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    11272 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/4D248.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    22296 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/4D248_helmet.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    42102 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/4D248_helmet.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     7077 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/CTF151.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    13813 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/CTF151_helmet.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    46654 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/CTF151_helmet.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    12927 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/CTF275.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    25461 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/CTF275_helmet.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    46654 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/CTF275_helmet.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    15330 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/EEG1005.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     3827 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/EEG1010.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      985 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/EEG1020.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     7134 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/QuikCap_NSL_128.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5164 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/QuikCap_NSL_128.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5813 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/acticap-64ch-standard2.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/acticap-64ch-standard2.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5697 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/biosemi128.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      770 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/biosemi16.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     7128 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/biosemi160.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    11414 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/biosemi256.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     1470 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/biosemi32.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2860 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/biosemi64.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5110 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/dccn_customized_acticap64.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6161 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/dccn_customized_acticap64.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6696 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM1.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM1.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5581 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM10.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6361 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM10.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5833 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM11.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6367 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM11.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    11302 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM14.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6361 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM14.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    11794 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM15.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6361 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM15.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     7800 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM16.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6362 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM16.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2643 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM17.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM17.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6873 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM20.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM20.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2547 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM22.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM22.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2985 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM23.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM23.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     3165 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM24.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM24.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2016 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM25.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM25.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2906 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM3.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM3.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2989 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM7.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6361 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM7.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    15330 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/elec1005.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     3827 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/elec1010.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      985 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/elec1020.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5269 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/mpi_customized_acticap64.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6161 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/mpi_customized_acticap64.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6127 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/natmeg_customized_eeg1005.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     3249 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/neuromag122cmb.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5961 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/neuromag122planar.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    14973 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/neuromag306all.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2643 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/neuromag306all_helmet.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/neuromag306all_helmet.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5489 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/neuromag306cmb.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6873 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/neuromag306cmb_helmet.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/neuromag306cmb_helmet.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     4979 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/neuromag306mag.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2547 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/neuromag306mag_helmet.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/neuromag306mag_helmet.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     9969 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/neuromag306planar.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2985 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/neuromag306planar_helmet.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/neuromag306planar_helmet.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5691 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/quickcap64.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6366 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/quickcap64.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    20670 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/yokogawa440.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    19775 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/yokogawa440_old.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    14079 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/yokogawa440ag.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    20655 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/yokogawa440all.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6565 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/yokogawa440pg.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     8696 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scanner/neuromag306_channel_names.npy
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-06-28 11:56:24.686856 osl-dynamics-1.2.4/osl_dynamics/files/scene/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)       82 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scene/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)  1511998 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/files/scene/mode_scene.scene
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-06-28 11:56:24.801735 osl-dynamics-1.2.4/osl_dynamics/inference/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      160 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/inference/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     7118 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/inference/callbacks.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     7382 2023-06-27 10:28:22.000000 osl-dynamics-1.2.4/osl_dynamics/inference/initializers.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    43495 2023-06-08 10:40:24.000000 osl-dynamics-1.2.4/osl_dynamics/inference/layers.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    11394 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/inference/metrics.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    20066 2023-06-22 15:05:16.000000 osl-dynamics-1.2.4/osl_dynamics/inference/modes.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6797 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/inference/regularizers.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     1647 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/inference/tf_ops.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-06-28 11:56:24.922124 osl-dynamics-1.2.4/osl_dynamics/models/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     1426 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/models/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    17504 2023-06-26 18:57:47.000000 osl-dynamics-1.2.4/osl_dynamics/models/dynemo.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    11105 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/models/dynemo_obs.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    44792 2023-06-27 10:28:22.000000 osl-dynamics-1.2.4/osl_dynamics/models/hmm.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    24034 2023-06-27 14:18:42.000000 osl-dynamics-1.2.4/osl_dynamics/models/inf_mod_base.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    23641 2023-06-26 18:57:47.000000 osl-dynamics-1.2.4/osl_dynamics/models/mage.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    21074 2023-06-26 18:57:47.000000 osl-dynamics-1.2.4/osl_dynamics/models/mdynemo.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    11366 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/models/mdynemo_obs.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    16837 2023-06-27 14:18:42.000000 osl-dynamics-1.2.4/osl_dynamics/models/mod_base.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    19196 2023-06-26 18:57:47.000000 osl-dynamics-1.2.4/osl_dynamics/models/sage.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    31151 2023-06-26 18:57:47.000000 osl-dynamics-1.2.4/osl_dynamics/models/sedynemo.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    32160 2023-06-08 09:36:36.000000 osl-dynamics-1.2.4/osl_dynamics/models/sedynemo_obs.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    38592 2023-06-26 19:15:14.000000 osl-dynamics-1.2.4/osl_dynamics/models/sehmm.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    13448 2023-06-08 10:40:24.000000 osl-dynamics-1.2.4/osl_dynamics/models/state_dynemo.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-06-28 11:56:25.009595 osl-dynamics-1.2.4/osl_dynamics/simulation/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      566 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/simulation/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      974 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/simulation/base.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    30162 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/simulation/hmm.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    12958 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/simulation/hsmm.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2710 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/simulation/mar.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    26028 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/simulation/mvn.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     4809 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/simulation/sin.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    10563 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/simulation/sm.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-06-28 11:56:25.023256 osl-dynamics-1.2.4/osl_dynamics/utils/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      287 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/utils/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5701 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/utils/decorators.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    13545 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/utils/misc.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6997 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/utils/model.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2206 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/utils/parcellation.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    63282 2023-06-26 18:57:47.000000 osl-dynamics-1.2.4/osl_dynamics/utils/plotting.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     9063 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/osl_dynamics/utils/topoplots.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-06-28 11:56:23.728532 osl-dynamics-1.2.4/osl_dynamics.egg-info/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     4561 2023-06-28 11:56:23.726351 osl-dynamics-1.2.4/osl_dynamics.egg-info/PKG-INFO
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     8283 2023-06-28 11:56:23.726956 osl-dynamics-1.2.4/osl_dynamics.egg-info/SOURCES.txt
--rw-r--r--   0 wlo995   (37469) woolrich (37107)        1 2023-06-28 11:56:23.727411 osl-dynamics-1.2.4/osl_dynamics.egg-info/dependency_links.txt
--rw-r--r--   0 wlo995   (37469) woolrich (37107)       83 2023-06-28 11:56:23.727759 osl-dynamics-1.2.4/osl_dynamics.egg-info/entry_points.txt
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      141 2023-06-28 11:56:23.728179 osl-dynamics-1.2.4/osl_dynamics.egg-info/requires.txt
--rw-r--r--   0 wlo995   (37469) woolrich (37107)       13 2023-06-28 11:56:23.728653 osl-dynamics-1.2.4/osl_dynamics.egg-info/top_level.txt
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)     1173 2023-06-28 11:56:25.025452 osl-dynamics-1.2.4/setup.cfg
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)      189 2023-05-09 14:22:26.000000 osl-dynamics-1.2.4/setup.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-07-07 12:52:56.730379 osl-dynamics-1.2.5/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     4561 2023-07-07 12:52:56.730581 osl-dynamics-1.2.5/PKG-INFO
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     4248 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/README.rst
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-07-07 12:52:55.097422 osl-dynamics-1.2.5/osl_dynamics/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      643 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/__init__.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-07-07 12:52:55.249943 osl-dynamics-1.2.5/osl_dynamics/analysis/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      250 2023-05-09 14:36:05.000000 osl-dynamics-1.2.5/osl_dynamics/analysis/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    27101 2023-06-22 11:45:55.000000 osl-dynamics-1.2.5/osl_dynamics/analysis/connectivity.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6437 2023-05-09 14:35:55.000000 osl-dynamics-1.2.5/osl_dynamics/analysis/fisher_kernel.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6165 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/analysis/gmm.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    25751 2023-07-07 10:59:21.000000 osl-dynamics-1.2.5/osl_dynamics/analysis/modes.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    20303 2023-06-26 18:57:47.000000 osl-dynamics-1.2.5/osl_dynamics/analysis/power.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     3268 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/analysis/regression.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    47241 2023-07-07 10:59:21.000000 osl-dynamics-1.2.5/osl_dynamics/analysis/spectral.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     7487 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/analysis/static.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     8644 2023-07-04 16:42:28.000000 osl-dynamics-1.2.5/osl_dynamics/analysis/statistics.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    29690 2023-06-08 09:36:36.000000 osl-dynamics-1.2.5/osl_dynamics/analysis/tinda.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5688 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/analysis/workbench.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    10899 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/array_ops.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-07-07 12:52:55.275228 osl-dynamics-1.2.5/osl_dynamics/config_api/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      895 2023-06-19 18:50:42.000000 osl-dynamics-1.2.5/osl_dynamics/config_api/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5832 2023-06-30 15:13:42.000000 osl-dynamics-1.2.5/osl_dynamics/config_api/pipeline.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    57245 2023-07-05 13:35:45.000000 osl-dynamics-1.2.5/osl_dynamics/config_api/wrappers.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-07-07 12:52:55.316383 osl-dynamics-1.2.5/osl_dynamics/data/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      112 2023-06-28 08:10:13.000000 osl-dynamics-1.2.5/osl_dynamics/data/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    41414 2023-07-07 10:59:21.000000 osl-dynamics-1.2.5/osl_dynamics/data/base.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     4770 2023-07-07 10:59:21.000000 osl-dynamics-1.2.5/osl_dynamics/data/processing.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     8142 2023-06-30 15:13:42.000000 osl-dynamics-1.2.5/osl_dynamics/data/rw.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2447 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/data/task.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     4473 2023-07-05 13:12:41.000000 osl-dynamics-1.2.5/osl_dynamics/data/tf.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-07-07 12:52:55.328138 osl-dynamics-1.2.5/osl_dynamics/files/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      883 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      434 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/functions.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-07-07 12:52:55.540552 osl-dynamics-1.2.5/osl_dynamics/files/mask/
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)     7241 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/mask/MNI152_T1_8mm_brain.nii.gz
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   724726 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/mask/ParcellationPilot.L.inflated.32k_fs_LR.surf.gii
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   723434 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/mask/ParcellationPilot.L.midthickness.32k_fs_LR.surf.gii
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   723505 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/mask/ParcellationPilot.L.very_inflated.32k_fs_LR.surf.gii
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   713031 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/mask/ParcellationPilot.R.inflated.32k_fs_LR.surf.gii
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   710727 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/mask/ParcellationPilot.R.midthickness.32k_fs_LR.surf.gii
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   712178 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/mask/ParcellationPilot.R.very_inflated.32k_fs_LR.surf.gii
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     1649 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/mask/__init__.py
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)      971 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/mask/ft_8mm_brain_mask.nii.gz
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-07-07 12:52:55.635136 osl-dynamics-1.2.5/osl_dynamics/files/parcellation/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    41373 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/parcellation/Glasser50_space-MNI152NLin6_res-8x8x8.nii.gz
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     9131 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/parcellation/Glasser52_binary_space-MNI152NLin6_res-8x8x8.nii.gz
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      669 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/parcellation/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    36166 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/parcellation/aal_cortical_merged_8mm_stacked.nii.gz
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)    23705 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/parcellation/fMRI_parcellation_ds8mm.nii.gz
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    24111 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_3PCC_ips_reduced_2mm_ss5mm_ds8mm.nii.gz
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    33885 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_3PCC_ips_reduced_2mm_ss5mm_ds8mm_adj.nii.gz
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)    23705 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_reduced_2mm_ss5mm_ds8mm.nii.gz
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)    63185 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_tighterMay15_v2_6mm_exclusive.nii.gz
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)    63835 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_tighterMay15_v2_8mm.nii.gz
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)     5233 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/parcellation/giles_39_binary.nii.gz
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-07-07 12:52:55.663618 osl-dynamics-1.2.5/osl_dynamics/files/scanner/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      268 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5568 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/ctf275_channel_names.npy
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-07-07 12:52:56.397175 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6679 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/4D148.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    11272 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/4D248.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    22296 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/4D248_helmet.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    42102 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/4D248_helmet.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     7077 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/CTF151.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    13813 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/CTF151_helmet.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    46654 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/CTF151_helmet.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    12927 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/CTF275.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    25461 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/CTF275_helmet.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    46654 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/CTF275_helmet.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    15330 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/EEG1005.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     3827 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/EEG1010.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      985 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/EEG1020.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     7134 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/QuikCap_NSL_128.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5164 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/QuikCap_NSL_128.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5813 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/acticap-64ch-standard2.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/acticap-64ch-standard2.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5697 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/biosemi128.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      770 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/biosemi16.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     7128 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/biosemi160.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    11414 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/biosemi256.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     1470 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/biosemi32.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2860 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/biosemi64.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5110 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/dccn_customized_acticap64.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6161 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/dccn_customized_acticap64.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6696 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM1.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM1.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5581 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM10.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6361 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM10.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5833 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM11.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6367 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM11.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    11302 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM14.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6361 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM14.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    11794 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM15.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6361 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM15.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     7800 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM16.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6362 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM16.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2643 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM17.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM17.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6873 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM20.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM20.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2547 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM22.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM22.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2985 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM23.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM23.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     3165 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM24.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM24.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2016 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM25.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM25.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2906 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM3.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM3.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2989 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM7.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6361 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM7.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    15330 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/elec1005.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     3827 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/elec1010.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      985 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/elec1020.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5269 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/mpi_customized_acticap64.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6161 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/mpi_customized_acticap64.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6127 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/natmeg_customized_eeg1005.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     3249 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/neuromag122cmb.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5961 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/neuromag122planar.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    14973 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/neuromag306all.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2643 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/neuromag306all_helmet.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/neuromag306all_helmet.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5489 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/neuromag306cmb.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6873 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/neuromag306cmb_helmet.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/neuromag306cmb_helmet.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     4979 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/neuromag306mag.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2547 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/neuromag306mag_helmet.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/neuromag306mag_helmet.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     9969 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/neuromag306planar.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2985 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/neuromag306planar_helmet.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/neuromag306planar_helmet.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5691 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/quickcap64.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6366 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/quickcap64.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    20670 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/yokogawa440.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    19775 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/yokogawa440_old.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    14079 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/yokogawa440ag.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    20655 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/yokogawa440all.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6565 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/yokogawa440pg.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     8696 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scanner/neuromag306_channel_names.npy
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-07-07 12:52:56.399180 osl-dynamics-1.2.5/osl_dynamics/files/scene/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)       82 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scene/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)  1511998 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/files/scene/mode_scene.scene
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-07-07 12:52:56.500783 osl-dynamics-1.2.5/osl_dynamics/inference/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      160 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/inference/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     7118 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/inference/callbacks.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     7382 2023-06-27 10:28:22.000000 osl-dynamics-1.2.5/osl_dynamics/inference/initializers.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    43495 2023-06-08 10:40:24.000000 osl-dynamics-1.2.5/osl_dynamics/inference/layers.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    11394 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/inference/metrics.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    20066 2023-06-22 15:05:16.000000 osl-dynamics-1.2.5/osl_dynamics/inference/modes.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6797 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/inference/regularizers.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     1647 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/inference/tf_ops.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-07-07 12:52:56.602397 osl-dynamics-1.2.5/osl_dynamics/models/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     1259 2023-06-29 15:07:07.000000 osl-dynamics-1.2.5/osl_dynamics/models/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    24157 2023-07-04 16:37:06.000000 osl-dynamics-1.2.5/osl_dynamics/models/dynemo.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    52499 2023-07-04 16:37:06.000000 osl-dynamics-1.2.5/osl_dynamics/models/hmm.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    24197 2023-06-30 12:57:28.000000 osl-dynamics-1.2.5/osl_dynamics/models/inf_mod_base.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    26522 2023-06-29 15:07:07.000000 osl-dynamics-1.2.5/osl_dynamics/models/mage.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    23271 2023-06-29 15:07:07.000000 osl-dynamics-1.2.5/osl_dynamics/models/mdynemo.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    18390 2023-06-28 14:04:34.000000 osl-dynamics-1.2.5/osl_dynamics/models/mod_base.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    22072 2023-06-29 15:07:07.000000 osl-dynamics-1.2.5/osl_dynamics/models/obs_mod.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    20816 2023-06-29 15:07:07.000000 osl-dynamics-1.2.5/osl_dynamics/models/sage.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    31720 2023-06-29 15:07:07.000000 osl-dynamics-1.2.5/osl_dynamics/models/sedynemo.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    41297 2023-06-29 15:07:07.000000 osl-dynamics-1.2.5/osl_dynamics/models/sehmm.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    13448 2023-06-08 10:40:24.000000 osl-dynamics-1.2.5/osl_dynamics/models/state_dynemo.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-07-07 12:52:56.684855 osl-dynamics-1.2.5/osl_dynamics/simulation/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      566 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/simulation/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      974 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/simulation/base.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    30162 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/simulation/hmm.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    12970 2023-07-07 10:59:21.000000 osl-dynamics-1.2.5/osl_dynamics/simulation/hsmm.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2710 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/simulation/mar.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    26028 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/simulation/mvn.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     4809 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/simulation/sin.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    10563 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/simulation/sm.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-07-07 12:52:56.729420 osl-dynamics-1.2.5/osl_dynamics/utils/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      287 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/utils/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5701 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/utils/decorators.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    13792 2023-06-30 18:25:18.000000 osl-dynamics-1.2.5/osl_dynamics/utils/misc.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6997 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/utils/model.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2206 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/utils/parcellation.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    63282 2023-06-26 18:57:47.000000 osl-dynamics-1.2.5/osl_dynamics/utils/plotting.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     9063 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/osl_dynamics/utils/topoplots.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-07-07 12:52:55.143016 osl-dynamics-1.2.5/osl_dynamics.egg-info/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     4561 2023-07-07 12:52:55.140905 osl-dynamics-1.2.5/osl_dynamics.egg-info/PKG-INFO
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     8184 2023-07-07 12:52:55.141357 osl-dynamics-1.2.5/osl_dynamics.egg-info/SOURCES.txt
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)        1 2023-07-07 12:52:55.141805 osl-dynamics-1.2.5/osl_dynamics.egg-info/dependency_links.txt
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)       83 2023-07-07 12:52:55.142205 osl-dynamics-1.2.5/osl_dynamics.egg-info/entry_points.txt
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      141 2023-07-07 12:52:55.142707 osl-dynamics-1.2.5/osl_dynamics.egg-info/requires.txt
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)       13 2023-07-07 12:52:55.143123 osl-dynamics-1.2.5/osl_dynamics.egg-info/top_level.txt
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)     1173 2023-07-07 12:52:56.731358 osl-dynamics-1.2.5/setup.cfg
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)      189 2023-05-09 14:22:26.000000 osl-dynamics-1.2.5/setup.py
```

### Comparing `osl-dynamics-1.2.4/PKG-INFO` & `osl-dynamics-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osl-dynamics
-Version: 1.2.4
+Version: 1.2.5
 Summary: Models for infering dynamics in neuroimaging data
 Home-page: https://github.com/OHBA-analysis/osl-dynamics
 License: MIT
 Project-URL: Documentation, https://osl-dynamics.readthedocs.io/en/latest/
 Description-Content-Type: text/x-rst; charset=UTF-8
 
 ============
```

### Comparing `osl-dynamics-1.2.4/README.rst` & `osl-dynamics-1.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/__init__.py` & `osl-dynamics-1.2.5/osl_dynamics/__init__.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/analysis/connectivity.py` & `osl-dynamics-1.2.5/osl_dynamics/analysis/connectivity.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/analysis/fisher_kernel.py` & `osl-dynamics-1.2.5/osl_dynamics/analysis/fisher_kernel.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/analysis/gmm.py` & `osl-dynamics-1.2.5/osl_dynamics/analysis/gmm.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/analysis/modes.py` & `osl-dynamics-1.2.5/osl_dynamics/analysis/modes.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,50 +9,52 @@
 from scipy import signal
 
 from osl_dynamics import array_ops, inference
 
 _logger = logging.getLogger("osl-dynamics")
 
 
-def autocorrelation_functions(
-    mode_covariances,
-    n_embeddings,
-    pca_components,
-):
+def autocorr_from_tde_cov(covs, n_embeddings, pca_components=None):
     """Auto/cross-correlation function from the mode covariance matrices.
 
     Parameters
     ----------
-    mode_covariances : np.ndarray
-        Mode covariance matrices.
+    covs : np.ndarray
+        Covariance matrix of time-delay embedded data. Shape must be
+        (n_channels, n_channels) or (n_modes, n_channels, n_channels).
     n_embeddings : int
-        Number of embeddings applied to the training data.
+        Number of embeddings.
     pca_components : np.ndarray
-        PCA components used for dimensionality reduction.
+        PCA components used for dimensionality reduction. Only needs to be passed
+        if PCA was performed on the time embedded data.
 
     Returns
     -------
     acfs : np.ndarray
-        Auto/cross-correlation functions.
+        Auto/cross-correlation functions. Shape is (n_channels, n_channels, n_acf)
+        or (n_modes, n_channels, n_channels, n_acf).
     """
     # Validation
     error_message = (
-        "mode_covariances must be of shape (n_channels, n_channels) or "
+        "covs must be of shape (n_channels, n_channels) or "
         + "(n_modes, n_channels, n_channels) or "
         + "(n_subjects, n_modes, n_channels, n_channels)."
     )
-    mode_covariances = array_ops.validate(
-        mode_covariances,
+    covs = array_ops.validate(
+        covs,
         correct_dimensionality=4,
         allow_dimensions=[2, 3],
         error_message=error_message,
     )
 
     # Get covariance of time embedded data
-    te_covs = reverse_pca(mode_covariances, pca_components)
+    if pca_components is not None:
+        te_covs = reverse_pca(covs, pca_components)
+    else:
+        te_covs = covs
 
     # Dimensions
     n_subjects = te_covs.shape[0]
     n_modes = te_covs.shape[1]
     n_parcels = te_covs.shape[-1] // n_embeddings
     n_acf = 2 * n_embeddings - 1
```

### Comparing `osl-dynamics-1.2.4/osl_dynamics/analysis/power.py` & `osl-dynamics-1.2.5/osl_dynamics/analysis/power.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/analysis/regression.py` & `osl-dynamics-1.2.5/osl_dynamics/analysis/regression.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/analysis/spectral.py` & `osl-dynamics-1.2.5/osl_dynamics/analysis/spectral.py`

 * *Files 0% similar despite different names*

```diff
@@ -382,30 +382,30 @@
 
     # Cross PSDs
     P = H @ covs[np.newaxis, ...] @ np.transpose(np.conj(H), axes=[0, 1, 3, 2])
 
     return f, np.squeeze(P)
 
 
-def mode_covariance_spectra(
-    autocorrelation_function,
+def autocorr_to_spectra(
+    autocorr_func,
     sampling_frequency,
     nfft=64,
     frequency_range=None,
 ):
     """Calculates spectra from the autocorrelation function.
 
     The power spectrum of each mode is calculated as the Fourier transform of
     the auto-correlation function. Coherences are calculated from the power spectra.
 
     Parameters
     ----------
-    autocorrelation_function : np.ndarray
-        Mode autocorrelation functions.
-        Shape must be (n_modes, n_channels, n_channels, n_acf).
+    autocorr_func : np.ndarray
+        Autocorrelation functions. Shape must be (n_channels, n_channels, n_acf) or
+        (n_modes, n_channels, n_channels, n_acf).
     sampling_frequency : float
         Frequency at which the data was sampled (Hz).
     nfft : int
         Number of data points in the FFT. The auto-correlation function will only
         have 2 * (n_embeddings + 2) - 1 data points. We pad the auto-correlation
         function with zeros to have nfft data points if the number of data points
         in the auto-correlation function is less than nfft. Default is 64.
@@ -413,38 +413,48 @@
         Minimum and maximum frequency to keep (Hz).
 
     Returns
     -------
     frequencies : np.ndarray
         Frequencies of the power spectra and coherences. Shape is (n_freq,).
     power_spectra : np.ndarray
-        Power (or cross) spectra calculated for each mode. Shape is (n_modes,
-        n_channels, n_channels, n_freq).
+        Power (or cross) spectra calculated for each mode. Shape is
+        (n_channels, n_channels, n_freq) or (n_modes, n_channels, n_channels, n_freq).
     coherences : np.ndarray
-        Coherences calculated for each mode. Shape is (n_modes, n_channels,
-        n_channels, n_freq).
+        Coherences calculated for each mode. Shape is (n_channels, n_channels, n_freq)
+        or (n_modes, n_channels, n_channels, n_freq).
     """
-    _logger.info("Calculating power spectra")
-
     # Validation
+    error_message = (
+        "autocorrelation_functions must be of shape (n_channels, n_channels, n_acf) "
+        + "or (n_modes, n_channels, n_channels, n_acf)."
+    )
+    autocorr_func = array_ops.validate(
+        autocorr_func,
+        correct_dimensionality=4,
+        allow_dimensions=[3],
+        error_message=error_message,
+    )
     if frequency_range is None:
         frequency_range = [0, sampling_frequency / 2]
 
+    _logger.info("Calculating power spectra")
+
     # Number of data points in the autocorrelation function and FFT
-    n_acf = autocorrelation_function.shape[-1]
+    n_acf = autocorr_func.shape[-1]
     nfft = max(nfft, 2 ** nextpow2(n_acf))
 
     # Calculate the argments to keep for the given frequency range
     frequencies = np.arange(0, sampling_frequency / 2, sampling_frequency / nfft)
     args_range = get_frequency_args_range(frequencies, frequency_range)
     frequencies = frequencies[args_range[0] : args_range[1]]
 
     # Calculate cross power spectra as the Fourier transform of the
     # auto/cross-correlation function
-    power_spectra = abs(fourier_transform(autocorrelation_function, nfft, args_range))
+    power_spectra = abs(fourier_transform(autocorr_func, nfft, args_range))
 
     # Normalise the power spectra
     power_spectra /= nfft**2
 
     # Coherences for each mode
     coherences = coherence_spectra(power_spectra)
```

### Comparing `osl-dynamics-1.2.4/osl_dynamics/analysis/static.py` & `osl-dynamics-1.2.5/osl_dynamics/analysis/static.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/analysis/statistics.py` & `osl-dynamics-1.2.5/osl_dynamics/analysis/statistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,66 +71,72 @@
     and performs a sign flip permutations test with the maximum statistic to
     determine a p-value for evoked responses.
 
     Parameters
     ----------
     data : np.ndarray
         Baseline corrected evoked responses. This will be the target data for the GLM.
-        Must be shape (n_subjects, n_samples, n_modes).
+        Must be shape (n_subjects, n_samples, ...).
     n_perm : int
         Number of permutations.
     covariates : dict
         Covariates (extra regressors) to add to the GLM fit. These will be z-transformed.
+        Must be of shape (n_subjects,).
     metric : str
         Metric to use to build the null distribution. Can be 'tstats' or 'copes'.
     n_jobs : int
         Number of processes to run in parallel.
 
     Returns
     -------
     pvalues : np.ndarray
-        P-values for the evoked response. Shape is (n_subjects, n_samples, n_modes).
+        P-values for the evoked response. Shape is (n_subjects, n_samples, ...).
     """
-    if metric not in ["tstats", "copes"]:
-        raise ValueError("metric must be 'tstats' or 'copes'.")
-
     if not isinstance(data, np.ndarray):
         raise ValueError("data must be a numpy array.")
-    if data.ndim != 3:
-        raise ValueError("data must be (n_subjects, n_samples, n_modes).")
+
+    ndim = data.ndim
+    if ndim < 3:
+        raise ValueError("data must be 3D or greater.")
+
+    if metric not in ["tstats", "copes"]:
+        raise ValueError("metric must be 'tstats' or 'copes'.")
 
     data, covariates = _check_glm_data(data, covariates)
 
     # Create GLM Dataset
     data = glm.data.TrialGLMData(
         data=data,
         **covariates,
-        dim_labels=["subjects", "samples", "channels"],
+        dim_labels=["subjects", "time"] + [f"features {i}" for i in range(1, ndim - 1)],
     )
 
     # Create design matrix
     DC = glm.design.DesignConfig()
     for name in covariates:
         DC.add_regressor(name=name, rtype="Parametric", datainfo=name, preproc="z")
     DC.add_regressor(name="Mean", rtype="Constant")
     DC.add_contrast(name="Mean", values=[1] + [0] * len(covariates))
     design = DC.design_from_datainfo(data.info)
 
     # Fit model and get t-statistics
     model = glm.fit.OLSModel(design, data)
 
+    # Pool over all dimensions over than subjects
+    pooled_dims = tuple(range(1, ndim))
+
     # Run permutations and get null distribution
     perm = glm.permutations.MaxStatPermutation(
         design,
         data,
         contrast_idx=0,  # selects the Mean contrast
         nperms=n_perm,
         metric=metric,
         tail=0,  # two-sided test
-        pooled_dims=(1, 2),  # pool over samples and modes dimension
+        pooled_dims=pooled_dims,
         nprocesses=n_jobs,
     )
     null_dist = perm.nulls
 
     # Get p-values
     if metric == "tstats":
         print("Using tstats as metric")
@@ -169,28 +175,30 @@
         1D numpy array containing group assignments. A value of 1 indicates
         Group1 and a value of 2 indicates Group2. Note, we test the contrast
         abs(Group1 - Group2) > 0.
     n_perm : int
         Number of permutations.
     covariates : dict
         Covariates (extra regressors) to add to the GLM fit. These will be z-transformed.
+        Must be of shape (n_subjects,).
     metric : str
         Metric to use to build the null distribution. Can be 'tstats' or 'copes'.
     n_jobs : int
         Number of processes to run in parallel.
 
     Returns
     -------
     group_diff : np.ndarray
         Group difference: Group1 - Group2. Shape is (features1, features2, ...).
     pvalues : np.ndarray
         P-values for the features. Shape is (features1, features2, ...).
     """
     if not isinstance(data, np.ndarray):
         raise ValueError("data must be a numpy array.")
+
     ndim = data.ndim
     if ndim == 1:
         raise ValueError("data must be 2D or greater.")
 
     if metric not in ["tstats", "copes"]:
         raise ValueError("metric must be 'tstats' or 'copes'.")
```

### Comparing `osl-dynamics-1.2.4/osl_dynamics/analysis/tinda.py` & `osl-dynamics-1.2.5/osl_dynamics/analysis/tinda.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/analysis/workbench.py` & `osl-dynamics-1.2.5/osl_dynamics/analysis/workbench.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/array_ops.py` & `osl-dynamics-1.2.5/osl_dynamics/array_ops.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/config_api/__init__.py` & `osl-dynamics-1.2.5/osl_dynamics/config_api/__init__.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/config_api/pipeline.py` & `osl-dynamics-1.2.5/osl_dynamics/config_api/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,14 @@
 
 Remember you need to activate the :code:`osld` conda environment to use the
 command line interface.
 """
 
 import argparse
 import logging
-import os
-import pickle
 import pprint
 from pathlib import Path
 
 import numpy as np
 import yaml
 
 from osl_dynamics.config_api import wrappers
@@ -130,18 +128,18 @@
         )
     )
 
     # Load data via the config
     load_data_kwargs = config.pop("load_data", None)
     if load_data_kwargs is not None:
         # Make sure the Data class uses a unique temporary directory
-        data_kwargs = load_data_kwargs.pop("data_kwargs", {})
-        default_data_kwargs = {"store_dir": f"tmp_{config_id}"}
-        data_kwargs = override_dict_defaults(default_data_kwargs, data_kwargs)
-        load_data_kwargs["data_kwargs"] = data_kwargs
+        kwargs = load_data_kwargs.pop("kwargs", {})
+        default_kwargs = {"store_dir": f"tmp_{config_id}"}
+        kwargs = override_dict_defaults(default_kwargs, kwargs)
+        load_data_kwargs["kwargs"] = kwargs
 
         # Load data
         _logger.info(f"load_data: {load_data_kwargs}")
         data = wrappers.load_data(**load_data_kwargs)
 
     # Loop through each item in the config
     for name, kwargs in config.items():
@@ -173,16 +171,16 @@
         Path to the output directory.
     restrict : int or str
         GPU to use. If a str is passed it will be cast to an int. Optional.
     """
     if restrict is not None:
         from osl_dynamics.inference import tf_ops
 
-        tp_ops.select_gpu(int(restrict))
-        tp_ops.gpu_growth()
+        tf_ops.select_gpu(int(restrict))
+        tf_ops.gpu_growth()
     config_path = Path(config_file)
     config = config_path.read_text()
 
     run_pipeline(config, output_directory)
 
 
 def osl_dynamics_cli():
```

### Comparing `osl-dynamics-1.2.4/osl_dynamics/config_api/wrappers.py` & `osl-dynamics-1.2.5/osl_dynamics/config_api/wrappers.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,56 +15,57 @@
 """
 
 import os
 import logging
 from pathlib import Path
 
 import numpy as np
-import pandas as pd
-import seaborn as sns
-import matplotlib.pyplot as plt
 
 from osl_dynamics import array_ops
 from osl_dynamics.utils.misc import load, override_dict_defaults, save
 
 _logger = logging.getLogger("osl-dynamics")
 
 
-def load_data(data_dir, data_kwargs={}, prepare_kwargs={}):
+def load_data(inputs, kwargs=None, prepare=None):
     """Load and prepare data.
 
     Parameters
     ----------
-    data_dir : str
+    inputs : str
         Path to directory containing npy files.
-    data_kwargs: dict
+    kwargs: dict
         Keyword arguments to pass to the Data class.
         Useful keyword arguments to pass are the :code:`sampling_frequency`,
         :code:`mask_file` and :code:`parcellation_file`.
-    prepare_kwargs : dict
-        Keyword arguments to pass to the prepare method.
+    prepare : dict
+        Methods dict to pass to the prepare method. See docstring for
+        osl_dynamics.data.Data.prepare.
 
     Returns
     -------
     data : osl_dynamics.data.Data
         Data object.
     """
     from osl_dynamics.data import Data
 
-    data = Data(data_dir, **data_kwargs)
-    data.prepare(**prepare_kwargs)
+    kwargs = {} if kwargs is None else kwargs
+    prepare = {} if prepare is None else prepare
+
+    data = Data(inputs, **kwargs)
+    data.prepare(prepare)
     return data
 
 
 def train_hmm(
     data,
     output_dir,
     config_kwargs,
-    init_kwargs={},
-    fit_kwargs={},
+    init_kwargs=None,
+    fit_kwargs=None,
     save_inf_params=True,
 ):
     """Train a Hidden Markov Model.
 
     This function will:
 
     1. Build an :code:`hmm.Model` object.
@@ -103,14 +104,17 @@
         Should we save the inferred parameters? Optional, defaults to :code:`True`.
     """
     if data is None:
         raise ValueError("data must be passed.")
 
     from osl_dynamics.models import hmm
 
+    init_kwargs = {} if init_kwargs is None else init_kwargs
+    fit_kwargs = {} if fit_kwargs is None else fit_kwargs
+
     # Directories
     model_dir = output_dir + "/model"
     inf_params_dir = output_dir + "/inf_params"
     os.makedirs(inf_params_dir, exist_ok=True)
 
     # Create the model object
     _logger.info("Building model")
@@ -156,16 +160,16 @@
         save(f"{inf_params_dir}/covs.npy", covs)
 
 
 def train_dynemo(
     data,
     output_dir,
     config_kwargs,
-    init_kwargs={},
-    fit_kwargs={},
+    init_kwargs=None,
+    fit_kwargs=None,
     save_inf_params=True,
 ):
     """Train DyNeMo.
 
     This function will:
 
     1. Build a :code:`dynemo.Model` object.
@@ -211,14 +215,18 @@
 
             {'n_init': 5, 'n_epochs': 1, 'take': 0.25}.
     fit_kwargs : dict
         Keyword arguments to pass to the :code:`Model.fit`. Optional, no defaults.
     save_inf_params : bool
         Should we save the inferred parameters? Optional, defaults to :code:`True`.
     """
+
+    init_kwargs = {} if init_kwargs is None else init_kwargs
+    fit_kwargs = {} if fit_kwargs is None else fit_kwargs
+
     if data is None:
         raise ValueError("data must be passed.")
 
     from osl_dynamics.models import dynemo
 
     # Directories
     model_dir = output_dir + "/model"
@@ -302,15 +310,15 @@
 
     covs = load(f"{inf_params_dir}/covs.npy")
 
     if hasattr(data, "pca_components"):
         if data.pca_components is not None:
             from osl_dynamics.analysis import modes
 
-            covs = modes.reverse_pca(covs, pca_components)
+            covs = modes.reverse_pca(covs, data.pca_components)
 
     from osl_dynamics.utils import plotting
 
     plotting.plot_matrices(covs, filename=f"{inf_params_dir}/tde_covs.png")
 
 
 def plot_state_psds(data, output_dir):
@@ -496,14 +504,17 @@
     data : osl_dynamics.data.Data
         Data object.
     output_dir : str
         Path to output directory.
     n_components : int
         Number of components to fit.
     """
+    from osl_dynamics.analysis import spectral
+
+    spectra_dir = output_dir + "/spectra"
     coh = load(f"{spectra_dir}/coh.npy")
     nnmf = spectral.decompose_spectra(coh, n_components=n_components)
     save(f"{spectra_dir}/nnmf_{n_components}.npy", nnmf)
 
 
 def regression_spectra(data, output_dir, kwargs):
     """Calculate regression spectra.
@@ -595,16 +606,16 @@
 
 def plot_group_ae_networks(
     data,
     output_dir,
     mask_file=None,
     parcellation_file=None,
     aec_abs=True,
-    power_save_kwargs={},
-    conn_save_kwargs={},
+    power_save_kwargs=None,
+    conn_save_kwargs=None,
 ):
     """Plot group-level amplitude envelope networks.
 
     This function expects a model has been trained and the following directory to exist:
 
     - :code:`<output_dir>/inf_params`, which contains the inferred parameters.
 
@@ -640,14 +651,17 @@
         <https://osl-dynamics.readthedocs.io/en/latest/autoapi/osl_dynamics/analysis/connectivity/index.html#osl_dynamics.analysis.connectivity.save>`_.
         Defaults to::
 
             {'parcellation_file': parcellation_file,
              'filename': '<output_dir>/networks/aec_.png',
              'threshold': 0.97}
     """
+    power_save_kwargs = {} if power_save_kwargs is None else power_save_kwargs
+    conn_save_kwargs = {} if conn_save_kwargs is None else conn_save_kwargs
+
     # Validation
     if mask_file is None:
         if data is None or data.mask_file is None:
             raise ValueError(
                 "mask_file must be passed or specified in the Data object."
             )
         else:
@@ -705,16 +719,16 @@
 def plot_group_tde_hmm_networks(
     data,
     output_dir,
     mask_file=None,
     parcellation_file=None,
     frequency_range=None,
     percentile=97,
-    power_save_kwargs={},
-    conn_save_kwargs={},
+    power_save_kwargs=None,
+    conn_save_kwargs=None,
 ):
     """Plot group-level TDE-HMM networks for a specified frequency band.
 
     This function will:
 
     1. Plot state PSDs.
     2. Plot the power maps.
@@ -742,15 +756,15 @@
         :code:`None`, we use :code:`data.parcellation_file`.
     frequency_range : list
         List of length 2 containing the minimum and maximum frequency to integrate
         spectra over. Optional, defaults to the full frequency range.
     percentile : float
         Percentile for thresholding the coherence networks. Default is 97, which
         corresponds to the top 3% of edges (relative to the mean across states).
-    plot_save_kwargs : dict
+    power_save_kwargs : dict
         Keyword arguments to pass to `analysis.power.save
         <https://osl-dynamics.readthedocs.io/en/latest/autoapi/osl_dynamics/analysis/power/index.html#osl_dynamics.analysis.power.save>`_.
         Defaults to::
 
             {'mask_file': mask_file,
              'parcellation_file': parcellation_file,
              'filename': '<output_dir>/networks/pow_.png',
@@ -760,14 +774,17 @@
         <https://osl-dynamics.readthedocs.io/en/latest/autoapi/osl_dynamics/analysis/connectivity/index.html#osl_dynamics.analysis.connectivity.save>`_.
         Defaults to::
 
             {'parcellation_file': parcellation_file,
              'filename': '<output_dir>/networks/coh_.png',
              'plot_kwargs': {'edge_cmap': 'Reds'}}
     """
+    power_save_kwargs = {} if power_save_kwargs is None else power_save_kwargs
+    conn_save_kwargs = {} if conn_save_kwargs is None else conn_save_kwargs
+
     # Validation
     if mask_file is None:
         if data is None or data.mask_file is None:
             raise ValueError(
                 "mask_file must be passed or specified in the Data object."
             )
         else:
@@ -867,16 +884,16 @@
     data,
     output_dir,
     nnmf_file,
     mask_file=None,
     parcellation_file=None,
     component=0,
     percentile=97,
-    power_save_kwargs={},
-    conn_save_kwargs={},
+    power_save_kwargs=None,
+    conn_save_kwargs=None,
 ):
     """Plot group-level TDE-HMM networks using a NNMF component to integrate
     the spectra.
 
     This function will:
 
     1. Plot state PSDs.
@@ -909,15 +926,15 @@
         Parcellation file used to parcellate the training data. Optional. If
         :code:`None`, we use :code:`data.parcellation_file`.
     component : int
         NNMF component to plot. Defaults to the first component.
     percentile : float
         Percentile for thresholding the coherence networks. Default is 97, which
         corresponds to the top 3% of edges (relative to the mean across states).
-    plot_save_kwargs : dict
+    power_save_kwargs : dict
         Keyword arguments to pass to `analysis.power.save
         <https://osl-dynamics.readthedocs.io/en/latest/autoapi/osl_dynamics/analysis/power/index.html#osl_dynamics.analysis.power.save>`_.
         Defaults to::
 
             {'mask_file': mask_file,
              'parcellation_file': parcellation_file,
              'component': component,
@@ -929,14 +946,17 @@
         Defaults to::
 
             {'parcellation_file': parcellation_file,
              'component': component,
              'filename': '<output_dir>/networks/coh_.png',
              'plot_kwargs': {'edge_cmap': 'Reds'}}
     """
+    power_save_kwargs = {} if power_save_kwargs is None else power_save_kwargs
+    conn_save_kwargs = {} if conn_save_kwargs is None else conn_save_kwargs
+
     # Validation
     if mask_file is None:
         if data is None or data.mask_file is None:
             raise ValueError(
                 "mask_file must be passed or specified in the Data object."
             )
         else:
@@ -1051,16 +1071,16 @@
 def plot_group_tde_dynemo_networks(
     data,
     output_dir,
     mask_file=None,
     parcellation_file=None,
     frequency_range=None,
     percentile=97,
-    power_save_kwargs={},
-    conn_save_kwargs={},
+    power_save_kwargs=None,
+    conn_save_kwargs=None,
 ):
     """Plot group-level TDE-DyNeMo networks for a specified frequency band.
 
     This function will:
 
     1. Plot mode PSDs.
     2. Plot the power maps.
@@ -1106,14 +1126,17 @@
         <https://osl-dynamics.readthedocs.io/en/latest/autoapi/osl_dynamics/analysis/connectivity/index.html#osl_dynamics.analysis.connectivity.save>`_.
         Defaults to::
 
             {'parcellation_file': parcellation_file,
              'filename': '<output_dir>/networks/coh_.png',
              'plot_kwargs': {'edge_cmap': 'Reds'}}
     """
+    power_save_kwargs = {} if power_save_kwargs is None else power_save_kwargs
+    conn_save_kwargs = {} if conn_save_kwargs is None else conn_save_kwargs
+
     # Validation
     if mask_file is None:
         if data is None or data.mask_file is None:
             raise ValueError(
                 "mask_file must be passed or specified in the Data object."
             )
         else:
@@ -1209,15 +1232,15 @@
         default_conn_save_kwargs, conn_save_kwargs
     )
     _logger.info(f"Using conn_save_kwargs: {conn_save_kwargs}")
     connectivity.save(gc, **conn_save_kwargs)
 
 
 def plot_alpha(
-    data, output_dir, subject=0, normalize=False, sampling_frequency=None, kwargs={}
+    data, output_dir, subject=0, normalize=False, sampling_frequency=None, kwargs=None
 ):
     """Plot inferred alphas.
 
     This is a wrapper for `utils.plotting.plot_alpha
     <https://osl-dynamics.readthedocs.io/en/latest/autoapi/osl_dynamics/utils/plotting/index.html#osl_dynamics.utils.plotting.plot_alpha>`_.
 
     This function expects a model has been trained and the following directory to exist:
@@ -1284,27 +1307,27 @@
         plotting.plot_alpha(alp[subject], **kwargs)
 
     if normalize:
         from osl_dynamics.inference import modes
 
         # Calculate normalised alphas
         covs = load(f"{inf_params_dir}/covs.npy")
-        norm_alp = modes.reweight_alphas(alp)
+        norm_alp = modes.reweight_alphas(alp, covs)
 
         # Plot
         if subject == "all":
             for i in range(len(alp)):
                 kwargs["filename"] = f"{alphas_dir}/norm_alpha_{i}.png"
                 plotting.plot_alpha(norm_alp[i], **kwargs)
         else:
             kwargs["filename"] = f"{alphas_dir}/norm_alpha_{subject}.png"
             plotting.plot_alpha(norm_alp[subject], **kwargs)
 
 
-def calc_gmm_alpha(data, output_dir, kwargs={}):
+def calc_gmm_alpha(data, output_dir, kwargs=None):
     """Binarize inferred alphas using a two-component GMM.
 
     This function expects a model has been trained and the following directory to exist:
 
     - :code:`<output_dir>/inf_params`, which contains the inferred parameters.
 
     This function will create the following file:
@@ -1317,14 +1340,15 @@
         Data object.
     output_dir : str
         Path to output directory.
     kwargs : dict
         Keyword arguments to pass to `inference.modes.gmm_time_courses
         <https://osl-dynamics.readthedocs.io/en/latest/autoapi/osl_dynamics/inference/modes/index.html#osl_dynamics.inference.modes.gmm_time_courses>`_.
     """
+    kwargs = {} if kwargs is None else kwargs
     inf_params_dir = output_dir + "/inf_params"
 
     # Load inferred alphas
     alp_file = f"{inf_params_dir}/alp.pkl"
     if not Path(alp_file).exists():
         raise ValueError(f"{alp_file} missing.")
     alp = load(alp_file)
```

### Comparing `osl-dynamics-1.2.4/osl_dynamics/data/base.py` & `osl-dynamics-1.2.5/osl_dynamics/data/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 """Base class for handling data.
 
 """
 
 import logging
 import pathlib
 import pickle
-import warnings
-from functools import partial
-from os import path
+from contextlib import contextmanager
 from shutil import rmtree
+from os import path
 
 import numpy as np
 from pqdm.threads import pqdm
-from scipy import signal
 from tqdm.auto import tqdm
 
 from osl_dynamics.data import processing, rw, tf
 from osl_dynamics.utils import misc
 
 _logger = logging.getLogger("osl-dynamics")
 
@@ -67,33 +65,26 @@
         Path to parcellation file used to source reconstruct the data. This argument
         is optional.
     store_dir : str
         We don't read all the data into memory. Instead we create store them on
         disk and create memmaps (unless load_memmaps=False is passed).
         This is the directory to save memmaps to. Default is ./tmp.
         This argument is optional.
-    n_embeddings : int
-        Number of time-delay embeddings that have already been appleid to the data.
-        This argument is optional. It is useful to pass this argument if the data has
-        already been prepared.
-    n_window : int
-        Length of sliding window that has already been applied to the data. This
-        argument is optional. It is useful to pass this argument if the data has
-        already been prepared.
-    amplitude_envelope : bool
-        Is the data we're loading amplitude envelope data? This argument is optional.
-        It is useful to pass this argument if the data has already been prepared.
     time_axis_first : bool
         Is the input data of shape (n_samples, n_channels)? Default is True.
         If your data is in format (n_channels, n_samples), use
         time_axis_first=False. This argument is optional.
-    load_memmaps: bool
+    load_memmaps : bool
         Should we load the data as memory maps (memmaps)? If False, we will load data
         into memory rather than storing it on disk. By default we will keep the data
         on disk and use memmaps. This argument is optional.
+    buffer_size : int
+        Buffer size for shuffling a TensorFlow Dataset. Smaller values will lead
+        to less random shuffling but will be quicker. This argument is optional.
+        Default is 100000.
     n_jobs : int
         Number of processes to load the data in parallel. This argument is optional.
         Default is 1, which loads data in serial.
     """
 
     def __init__(
         self,
@@ -101,161 +92,175 @@
         data_field="X",
         picks=None,
         reject_by_annotation=None,
         sampling_frequency=None,
         mask_file=None,
         parcellation_file=None,
         store_dir="tmp",
-        n_embeddings=None,
-        n_window=None,
-        amplitude_envelope=None,
         time_axis_first=True,
         load_memmaps=True,
+        buffer_size=100000,
         n_jobs=1,
     ):
         self._identifier = id(self)
         self.data_field = data_field
         self.picks = picks
         self.reject_by_annotation = reject_by_annotation
         self.sampling_frequency = sampling_frequency
         self.mask_file = mask_file
         self.parcellation_file = parcellation_file
-        self.n_embeddings = n_embeddings
-        self.n_window = n_window
-        self.amplitude_envelope = amplitude_envelope
         self.time_axis_first = time_axis_first
         self.load_memmaps = load_memmaps
+        self.buffer_size = buffer_size
         self.n_jobs = n_jobs
-        self.prepared = False
-        self.prepared_data_filenames = []
 
         # Validate inputs
         self.inputs = rw.validate_inputs(inputs)
 
         if len(self.inputs) == 0:
             raise ValueError("No valid inputs were passed.")
 
         # Directory to store memory maps created by this class
         self.store_dir = pathlib.Path(store_dir)
         self.store_dir.mkdir(parents=True, exist_ok=True)
 
         # Load and validate the raw data
-        self.raw_data_memmaps, self.raw_data_filenames = self.load_raw_data()
+        self.raw_data_arrays, self.raw_data_filenames = self.load_raw_data()
         self.validate_data()
 
-        # Get data prepration attributes if the raw data has been prepared
+        self.n_raw_data_channels = self.raw_data_arrays[0].shape[-1]
+
+        # Get data preparation attributes if there's a pickle file in the
+        # input directory
         if not isinstance(inputs, list):
             self.load_preparation(inputs)
 
-        self.n_raw_data_channels = self.raw_data_memmaps[0].shape[-1]
+        # Store raw data in the arrays attribute
+        self.arrays = self.raw_data_arrays
 
-        # Use raw data for the subject data
-        self.subjects = self.raw_data_memmaps
+        # Create filenames for prepared data memmaps
+        prepared_data_pattern = "prepared_data_{{i:0{width}d}}_{identifier}.npy".format(
+            width=len(str(self.n_arrays)), identifier=self._identifier
+        )
+        self.prepared_data_filenames = [
+            str(self.store_dir / prepared_data_pattern.format(i=i))
+            for i in range(self.n_arrays)
+        ]
+
+        # Arrays to keep when making TensorFlow Datasets
+        self.keep = list(range(self.n_arrays))
 
     def __iter__(self):
-        return iter(self.subjects)
+        return iter(self.arrays)
 
     def __getitem__(self, item):
-        return self.subjects[item]
+        return self.arrays[item]
 
     def __str__(self):
         info = [
             f"{self.__class__.__name__}",
             f"id: {self._identifier}",
-            f"n_subjects: {self.n_subjects}",
+            f"n_arrays: {self.n_arrays}",
             f"n_samples: {self.n_samples}",
             f"n_channels: {self.n_channels}",
         ]
         return "\n ".join(info)
 
     @property
     def raw_data(self):
         """Return raw data as a list of arrays."""
-        return self.raw_data_memmaps
+        return self.raw_data_arrays
 
     @property
     def n_channels(self):
         """Number of channels in the data files."""
-        return self.subjects[0].shape[-1]
+        return self.arrays[0].shape[-1]
 
     @property
     def n_samples(self):
-        """Number of samples for each subject."""
-        return sum([subject.shape[-2] for subject in self.subjects])
+        """Number of samples for each array."""
+        return sum([array.shape[-2] for array in self.arrays])
 
     @property
-    def n_subjects(self):
-        """Number of subjects."""
-        return len(self.subjects)
+    def n_arrays(self):
+        """Number of arrays."""
+        return len(self.arrays)
+
+    @contextmanager
+    def set_keep(self, keep):
+        """Context manager to temporarily set the kept arrays.
+
+        Parameters
+        ----------
+        keep : int or list of int
+            Indices to keep in the Data.arrays list.
+        """
+        # Store the current kept arrays
+        current_keep = self.keep
+        try:
+            # validation
+            if isinstance(keep, int):
+                keep = [keep]
+            if not isinstance(keep, list):
+                raise ValueError("keep must be a list of indices or a single index.")
+
+            # Set the new kept arrays
+            self.keep = keep
+            yield
+        finally:
+            self.keep = current_keep
 
     def set_sampling_frequency(self, sampling_frequency):
         """Sets the sampling_frequency attribute.
 
         Parameters
         ----------
         sampling_frequency : float
             Sampling frequency in Hz.
         """
         self.sampling_frequency = sampling_frequency
 
+    def set_buffer_size(self, buffer_size):
+        """Set the buffer_size attribute.
+
+        Parameters
+        ----------
+        buffer_size : int
+            Buffer size for shuffling a TensorFlow Dataset. Smaller values will lead
+            to less random shuffling but will be quicker.
+        """
+        self.buffer_size = buffer_size
+
     def time_series(self, prepared=True, concatenate=False):
-        """Time series data for all subjects.
+        """Time series data for all arrays.
 
         Parameters
         ----------
         prepared : bool
             Should we return the latest data after we have prepared it or
             the original data we loaded into the Data object?
         concatenate : bool
-            Should we return the time series for each subject concatenated?
+            Should we return the time series for each array concatenated?
 
         Returns
         -------
         ts : list or np.ndarray
-            Time series data for each subject.
+            Time series data for each array.
         """
         # What data should we return?
         if prepared:
-            memmaps = self.subjects
+            arrays = self.arrays
         else:
-            memmaps = self.raw_data_memmaps
+            arrays = self.raw_data_arrays
 
         # Should we return one long time series?
-        if concatenate or self.n_subjects == 1:
-            return np.concatenate(memmaps)
+        if concatenate or self.n_arrays == 1:
+            return np.concatenate(arrays)
         else:
-            return memmaps
-
-    def delete_dir(self):
-        """Deletes store_dir."""
-        if self.store_dir.exists():
-            rmtree(self.store_dir)
-
-    def load_preparation(self, inputs):
-        """Loads a pickle file containing preparation settings.
-
-        Parameters
-        ----------
-        inputs : str
-            Path to directory containing the pickle file with preparation settings.
-        """
-        if path.isdir(inputs):
-            for file in rw.list_dir(inputs):
-                if "preparation.pkl" in file:
-                    preparation = pickle.load(open(inputs + "/preparation.pkl", "rb"))
-                    self.amplitude_envelope = preparation["amplitude_envelope"]
-                    self.low_freq = preparation["low_freq"]
-                    self.high_freq = preparation["high_freq"]
-                    self.n_window = preparation["n_window"]
-                    self.n_embeddings = preparation["n_embeddings"]
-                    self.n_te_channels = preparation["n_te_channels"]
-                    self.n_pca_components = preparation["n_pca_components"]
-                    self.pca_components = preparation["pca_components"]
-                    self.whiten = preparation["whiten"]
-                    self.prepared = True
+            return arrays
 
     def load_raw_data(self):
         """Import data into a list of memory maps.
 
         Returns
         -------
         memmaps : list of np.memmap
@@ -270,19 +275,17 @@
             str(self.store_dir / raw_data_pattern.format(i=i))
             for i in range(len(self.inputs))
         ]
         # self.raw_data_filenames is not used if self.inputs is a list of strings,
         # where the strings are paths to .npy files
 
         # Load data
-        partial_make_memmap = partial(self.make_memmap)
-        args = zip(self.inputs, raw_data_filenames)
         memmaps = pqdm(
-            args,
-            partial_make_memmap,
+            array=zip(self.inputs, raw_data_filenames),
+            function=self.make_memmap,
             n_jobs=self.n_jobs,
             desc="Loading files",
             argument_type="args",
             total=len(self.inputs),
         )
 
         return memmaps, raw_data_filenames
@@ -312,429 +315,534 @@
             mmap_location,
             mmap_mode="r",
         )
         if not self.time_axis_first:
             raw_data_mmap = raw_data_mmap.T
         return raw_data_mmap
 
-    def save(self, output_dir="."):
-        """Saves data to numpy files.
-
-        Parameters
-        ----------
-        output_dir : str
-            Path to save data files to. Default is the current working directory.
-        """
-        output_dir = pathlib.Path(output_dir)
-        output_dir.mkdir(parents=True, exist_ok=True)
-
-        # Save time series data
-        for i, subject_data in enumerate(tqdm(self.subjects, desc="Saving data")):
-            padded_number = misc.leading_zeros(i, self.n_subjects)
-            np.save(f"{output_dir}/subject{padded_number}.npy", subject_data)
-
-        # Save preparation info if .prepared has been called
-        if self.prepared:
-            preparation = {
-                "amplitude_envelope": self.amplitude_envelope,
-                "low_freq": self.low_freq,
-                "high_freq": self.high_freq,
-                "n_window": self.n_window,
-                "n_embeddings": self.n_embeddings,
-                "n_te_channels": self.n_te_channels,
-                "n_pca_components": self.n_pca_components,
-                "pca_components": self.pca_components,
-                "whiten": self.whiten,
-            }
-            pickle.dump(preparation, open(f"{output_dir}/preparation.pkl", "wb"))
-
     def validate_data(self):
         """Validate data files."""
-        n_channels = [memmap.shape[-1] for memmap in self.raw_data_memmaps]
+        n_channels = [array.shape[-1] for array in self.raw_data_arrays]
         if not np.equal(n_channels, n_channels[0]).all():
             raise ValueError("All inputs should have the same number of channels.")
 
-    def filter(self, low_freq=None, high_freq=None):
-        """Filter the raw data.
+    def filter(self, low_freq=None, high_freq=None, use_raw=False):
+        """Filter the data.
+
+        This is an in-place operation.
 
         Parameters
         ----------
         low_freq : float
             Frequency in Hz for a high pass filter.
         high_freq : float
             Frequency in Hz for a low pass filter.
+        use_raw : bool
+            Should we prepare the original 'raw' data that we loaded?
+
+        Returns
+        -------
+        data : osl_dynamics.data.Data
+            The modified Data object.
         """
-        if (
-            low_freq is not None or high_freq is not None
-        ) and self.sampling_frequency is None:
+        if low_freq is None and high_freq is None:
+            _logger.warning("No filtering applied.")
+            return
+
+        if self.sampling_frequency is None:
             raise ValueError(
                 "Data.sampling_frequency must be set if we are filtering the data. "
                 + "Use Data.set_sampling_frequency() or pass "
                 + "Data(..., sampling_frequency=...) when creating the Data object."
             )
 
-        # Save settings
-        self.amplitude_envelope = False
         self.low_freq = low_freq
         self.high_freq = high_freq
-        self.n_window = 1
-        self.n_embeddings = 1
-        self.n_te_channels = self.n_raw_data_channels
-        self.n_pca_components = None
-        self.pca_components = None
-        self.whiten = None
-
-        # Create filenames for memmaps (i.e. self.prepared_data_filenames)
-        self.prepare_memmap_filenames()
-
-        # Prepare the data
-        for raw_data_memmap, prepared_data_file in zip(
-            tqdm(self.raw_data_memmaps, desc="Filtering data"),
-            self.prepared_data_filenames,
-        ):
-            # Filtering
-            prepared_data = processing.temporal_filter(
-                raw_data_memmap, low_freq, high_freq, self.sampling_frequency
-            )
 
+        # Function to apply filtering to a single array
+        def _apply(array, prepared_data_file):
+            array = processing.temporal_filter(
+                array, low_freq, high_freq, self.sampling_frequency
+            )
             if self.load_memmaps:
-                # Save the prepared data as a memmap
-                prepared_data_memmap = misc.array_to_memmap(
-                    prepared_data_file, prepared_data
-                )
-            else:
-                prepared_data_memmap = prepared_data
-            self.prepared_data_memmaps.append(prepared_data_memmap)
+                array = misc.array_to_memmap(prepared_data_file, array)
+            return array
 
-        # Update subjects to return the prepared data
-        self.subjects = self.prepared_data_memmaps
+        # Prepare the data in parallel
+        arrays = self.raw_data_arrays if use_raw else self.arrays
+        args = zip(arrays, self.prepared_data_filenames)
+        self.arrays = pqdm(
+            args,
+            function=_apply,
+            desc="Filtering",
+            n_jobs=self.n_jobs,
+            argument_type="args",
+            total=self.n_arrays,
+        )
+        if any([isinstance(e, Exception) for e in self.arrays]):
+            for i, e in enumerate(self.arrays):
+                if isinstance(e, Exception):
+                    e.args = (f"array {i}: {e}",)
+                    _logger.exception(e, exc_info=False)
+            raise e
 
-        self.prepared = True
+        return self
 
-    def prepare(
-        self,
-        amplitude_envelope=False,
-        low_freq=None,
-        high_freq=None,
-        n_window=1,
-        n_embeddings=1,
-        n_pca_components=None,
-        pca_components=None,
-        whiten=False,
-    ):
-        """Prepares data to train the model with.
+    def downsample(self, freq, use_raw=False):
+        """Downsample the data.
 
-        If amplitude_envelope=True, first we filter the data then
-        calculate a Hilbert transform and take the absolute value.
-        We then apply a sliding window moving average. Finally, we
-        standardize the data.
+        This is an in-place operation.
 
-        Otherwise, we standardize the data, perform time-delay embedding,
-        then PCA, then whiten. Finally, the data is standardized again.
+        Parameters
+        ----------
+        freq : float
+            Frequency in Hz to downsample to.
+        use_raw : bool
+            Should we prepare the original 'raw' data that we loaded?
 
-        If no arguments are passed, the data is just standardized.
+        Returns
+        -------
+        data : osl_dynamics.data.Data
+            The modified Data object.
+        """
+        if self.sampling_frequency is None:
+            raise ValueError(
+                "Data.sampling_frequency must be set if we are downsampling the data. "
+                + "Use Data.set_sampling_frequency() or pass "
+                + "Data(..., sampling_frequency=...) when creating the Data object."
+            )
+
+        if use_raw and hasattr(self, "original_sampling_frequency"):
+            sampling_frequency = self.original_sampling_frequency
+        else:
+            sampling_frequency = self.sampling_frequency
+
+        # Function to apply downsampling to a single array
+        def _apply(array, prepared_data_file):
+            array = processing.downsample(array, freq, sampling_frequency)
+            if self.load_memmaps:
+                array = misc.array_to_memmap(prepared_data_file, array)
+            return array
+
+        # Prepare the data in parallel
+        arrays = self.raw_data_arrays if use_raw else self.arrays
+        args = zip(arrays, self.prepared_data_filenames)
+        self.arrays = pqdm(
+            args,
+            function=_apply,
+            desc="Downsampling",
+            n_jobs=self.n_jobs,
+            argument_type="args",
+            total=self.n_arrays,
+        )
+        if any([isinstance(e, Exception) for e in self.arrays]):
+            for i, e in enumerate(self.arrays):
+                if isinstance(e, Exception):
+                    e.args = (f"array {i}: {e}",)
+                    _logger.exception(e, exc_info=False)
+            raise e
+
+        # Update sampling_frequency attributes
+        self.original_sampling_frequency = self.sampling_frequency
+        self.sampling_frequency = freq
+
+        return self
+
+    def pca(
+        self, n_pca_components=None, pca_components=None, whiten=False, use_raw=False
+    ):
+        """Principal component analysis (PCA).
+
+        This function will first standardize the data then perform PCA.
+        This is an in-place operation.
 
         Parameters
         ----------
-        amplitude_envelope : bool
-            Should we prepare amplitude envelope data?
-        low_freq : float
-            Frequency in Hz for a high pass filter.
-            Only used if amplitude_envelope=True.
-        high_freq : float
-            Frequency in Hz for a low pass filter.
-            Only used if amplitude_envelope=True.
-        n_window : int
-            Number of data points in a sliding window to apply to the amplitude
-            envelope data. Only used if amplitude_envelope=True.
-        n_embeddings : int
-            Number of data points to embed the data.
-            Only used if amplitude_envelope=False.
         n_pca_components : int
-            Number of PCA components to keep. Default is no PCA.
-            Only used if amplitude_envelope=False.
+            Number of PCA components to keep.
         pca_components : np.ndarray
             PCA components to apply if they have already been calculated.
-            Only used if amplitude_envelope=False.
         whiten : bool
             Should we whiten the PCA'ed data?
-            Only used if amplitude_envelope=False.
+        use_raw : bool
+            Should we prepare the original 'raw' data that we loaded?
+
+        Returns
+        -------
+        data : osl_dynamics.data.Data
+            The modified Data object.
         """
-        if self.prepared:
-            warnings.warn(
-                "Previously prepared data will be overwritten.", RuntimeWarning
-            )
+        if (n_pca_components is None and pca_components is None) or (
+            n_pca_components is not None and pca_components is not None
+        ):
+            raise ValueError("Please pass either n_pca_components or pca_components.")
 
-        # Prepare data (either amplitude envelope or time-delay embedded)
-        if amplitude_envelope:
-            self.prepare_amp_env(low_freq, high_freq, n_window)
-        else:
-            self.prepare_tde(n_embeddings, n_pca_components, pca_components, whiten)
+        if pca_components is not None and not isinstance(pca_components, np.ndarray):
+            raise ValueError("pca_components must be a numpy array.")
 
-    def prepare_amp_env(self, low_freq=None, high_freq=None, n_window=1):
-        """Prepare amplitude envelope data.
+        self.n_pca_components = n_pca_components
+        self.pca_components = pca_components
+        self.whiten = whiten
 
-        Parameters
-        ----------
-        low_freq : float
-            Frequency in Hz for a high pass filter.
-        high_freq : float
-            Frequency in Hz for a low pass filter.
-        n_window : int
-            Number of data points in a sliding window to apply to the amplitude
-            envelope data.
-        """
+        # What data should we apply PCA to?
+        arrays = self.raw_data_arrays if use_raw else self.arrays
 
-        # Validation
-        if (
-            low_freq is not None or high_freq is not None
-        ) and self.sampling_frequency is None:
-            raise ValueError(
-                "Data.sampling_frequency must be set if we are filtering the data. "
-                + "Use Data.set_sampling_frequency() or pass "
-                + "Data(..., sampling_frequency=...) when creating the Data object."
-            )
+        # Calculate PCA
+        if n_pca_components is not None:
+            # Calculate covariance of the data
+            n_channels = arrays[0].shape[-1]
+            covariance = np.zeros([n_channels, n_channels])
+            for array in tqdm(arrays, desc="Calculating PCA components"):
+                std_data = processing.standardize(array)
+                covariance += np.transpose(std_data) @ std_data
 
-        if n_window % 2 == 0:
-            raise ValueError("n_window must be an odd number.")
+            # Use SVD on the covariance to calculate PCA components
+            u, s, vh = np.linalg.svd(covariance)
+            u = u[:, :n_pca_components].astype(np.float32)
+            explained_variance = np.sum(s[:n_pca_components]) / np.sum(s)
+            _logger.info(f"Explained variance: {100 * explained_variance:.1f}%")
+            s = s[:n_pca_components].astype(np.float32)
+            if whiten:
+                u = u @ np.diag(1.0 / np.sqrt(s))
+            self.pca_components = u
 
-        # Save settings
-        self.amplitude_envelope = True
-        self.low_freq = low_freq
-        self.high_freq = high_freq
-        self.n_window = n_window
-        self.n_embeddings = 1
-        self.n_te_channels = self.n_raw_data_channels
-        self.n_pca_components = None
-        self.pca_components = None
-        self.whiten = None
-
-        # Create filenames for memmaps (i.e. self.prepared_data_filenames)
-        self.prepare_memmap_filenames()
-
-        # Prepare the data
-        prepare_args = zip(
-            self.raw_data_memmaps,
-            self.prepared_data_filenames,
-        )
-
-        prepared_data_memmaps = pqdm(
-            prepare_args,
-            self.apply_amp_env,
-            desc="Preparing data",
+        # Function to apply PCA to a single array
+        def _apply(array, prepared_data_file):
+            array = processing.standardize(array)
+            array = array @ self.pca_components
+            if self.load_memmaps:
+                array = misc.array_to_memmap(prepared_data_file, array)
+            return array
+
+        # Apply PCA in parallel
+        args = zip(arrays, self.prepared_data_filenames)
+        self.arrays = pqdm(
+            args,
+            function=_apply,
+            desc="PCA",
             n_jobs=self.n_jobs,
             argument_type="args",
-            total=len(self.raw_data_memmaps),
+            total=self.n_arrays,
         )
-        self.prepared_data_memmaps.extend(prepared_data_memmaps)
+        if any([isinstance(e, Exception) for e in self.arrays]):
+            for i, e in enumerate(self.arrays):
+                if isinstance(e, Exception):
+                    e.args = (f"array {i}: {e}",)
+                    _logger.exception(e, exc_info=False)
+            raise e
 
-        # Update subjects to return the prepared data
-        self.subjects = self.prepared_data_memmaps
+        return self
 
-        self.prepared = True
+    def tde(self, n_embeddings, use_raw=False):
+        """Time-delay embedding (TDE).
 
-    def apply_amp_env(self, raw_data_memmap, prepared_data_file):
-        """Applies filtering, a Hilbert transform and standardization to raw data.
+        This is an in-place operation.
 
         Parameters
         ----------
-        raw_data_memmap : np.memmap or np.ndarray
-            Raw data.
-        prepared_data_file : str
-            Name of memory map file to save prepared data to.
-            Can be None if we are not using memory maps.
+        n_embeddings : int
+            Number of data points to embed the data.
+        use_raw : bool
+            Should we prepare the original 'raw' data that we loaded?
 
         Returns
         -------
-        prepared_data_memmap : np.memmap or np.ndarray
-            Prepared data.
+        data : osl_dynamics.data.Data
+            The modified Data object.
         """
-        # Filtering
-        prepared_data = processing.temporal_filter(
-            raw_data_memmap, self.low_freq, self.high_freq, self.sampling_frequency
-        )
+        self.n_embeddings = n_embeddings
+        self.n_te_channels = self.n_raw_data_channels * n_embeddings
 
-        # Hilbert transform
-        prepared_data = np.abs(signal.hilbert(prepared_data, axis=0))
+        # Function to apply TDE to a single array
+        def _apply(array, prepared_data_file):
+            array = processing.time_embed(array, n_embeddings)
+            if self.load_memmaps:
+                array = misc.array_to_memmap(prepared_data_file, array)
+            return array
 
-        # Moving average filter
-        prepared_data = np.array(
-            [
-                np.convolve(
-                    prepared_data[:, i],
-                    np.ones(self.n_window) / self.n_window,
-                    mode="valid",
-                )
-                for i in range(prepared_data.shape[1])
-            ],
-        ).T
-
-        # Finally, we standardise
-        prepared_data = processing.standardize(prepared_data, create_copy=False)
-
-        # Make sure data is float32
-        prepared_data = prepared_data.astype(np.float32)
-
-        if self.load_memmaps:
-            # Save the prepared data as a memmap
-            prepared_data_memmap = misc.array_to_memmap(
-                prepared_data_file, prepared_data
-            )
-        else:
-            prepared_data_memmap = prepared_data
-        return prepared_data_memmap
+        # Apply TDE in parallel
+        arrays = self.raw_data_arrays if use_raw else self.arrays
+        args = zip(arrays, self.prepared_data_filenames)
+        self.arrays = pqdm(
+            args,
+            function=_apply,
+            desc="TDE",
+            n_jobs=self.n_jobs,
+            argument_type="args",
+            total=self.n_arrays,
+        )
+        if any([isinstance(e, Exception) for e in self.arrays]):
+            for i, e in enumerate(self.arrays):
+                if isinstance(e, Exception):
+                    e.args = (f"array {i}: {e}",)
+                    _logger.exception(e, exc_info=False)
+            raise e
+
+        return self
 
-    def prepare_tde(
+    def tde_pca(
         self,
-        n_embeddings=1,
+        n_embeddings,
         n_pca_components=None,
         pca_components=None,
         whiten=False,
+        use_raw=False,
     ):
-        """Prepares time-delay embedded data to train the model with.
+        """Time-delay embedding (TDE) and principal component analysis (PCA).
+
+        This function will first standardize the data, then perform TDE then PCA.
+        It is useful to do both operations in a single methods because it avoids
+        having to save the time-embedded data. This is an in-place operation.
 
         Parameters
         ----------
         n_embeddings : int
             Number of data points to embed the data.
         n_pca_components : int
-            Number of PCA components to keep. Default is no PCA.
+            Number of PCA components to keep.
         pca_components : np.ndarray
             PCA components to apply if they have already been calculated.
         whiten : bool
             Should we whiten the PCA'ed data?
-        """
+        use_raw : bool
+            Should we prepare the original 'raw' data that we loaded?
 
-        if n_pca_components is not None and pca_components is not None:
-            raise ValueError("Please only pass n_pca_components or pca_components.")
+        Returns
+        -------
+        data : osl_dynamics.data.Data
+            The modified Data object.
+        """
+        if (n_pca_components is None and pca_components is None) or (
+            n_pca_components is not None and pca_components is not None
+        ):
+            raise ValueError("Please pass either n_pca_components or pca_components.")
 
         if pca_components is not None and not isinstance(pca_components, np.ndarray):
             raise ValueError("pca_components must be a numpy array.")
 
-        # Save settings
-        self.amplitude_envelope = False
-        self.low_freq = None
-        self.high_freq = None
-        self.n_window = 1
         self.n_embeddings = n_embeddings
-        self.n_te_channels = self.n_raw_data_channels * n_embeddings
         self.n_pca_components = n_pca_components
         self.pca_components = pca_components
         self.whiten = whiten
 
-        # Create filenames for memmaps (i.e. self.prepared_data_filenames)
-        self.prepare_memmap_filenames()
+        # What data should we use?
+        arrays = self.raw_data_arrays if use_raw else self.arrays
+        self.n_te_channels = arrays[0].shape[-1] * n_embeddings
 
-        # Principle component analysis (PCA)
-        # NOTE: the approach used here only works for zero mean data
+        # Calculate PCA on TDE data
         if n_pca_components is not None:
-            # Calculate the PCA components by performing SVD on the covariance
-            # of the data
+            # Calculate covariance of the data
             covariance = np.zeros([self.n_te_channels, self.n_te_channels])
-            for raw_data_memmap in tqdm(
-                self.raw_data_memmaps, desc="Calculating PCA components"
-            ):
-                # Standardise and time embed the data
-                std_data = processing.standardize(raw_data_memmap)
+            for array in tqdm(arrays, desc="Calculating PCA components"):
+                std_data = processing.standardize(array)
                 te_std_data = processing.time_embed(std_data, n_embeddings)
-
-                # Calculate the covariance of the entire dataset
                 covariance += np.transpose(te_std_data) @ te_std_data
 
-            # Use SVD to calculate PCA components
+            # Use SVD on the covariance to calculate PCA components
             u, s, vh = np.linalg.svd(covariance)
             u = u[:, :n_pca_components].astype(np.float32)
             explained_variance = np.sum(s[:n_pca_components]) / np.sum(s)
             _logger.info(f"Explained variance: {100 * explained_variance:.1f}%")
             s = s[:n_pca_components].astype(np.float32)
             if whiten:
                 u = u @ np.diag(1.0 / np.sqrt(s))
             self.pca_components = u
 
-        prepare_args = zip(
-            self.raw_data_memmaps,
-            self.prepared_data_filenames,
+        # Function to apply TDE-PCA to a single array
+        def _apply(array, prepared_data_file):
+            array = processing.standardize(array)
+            array = processing.time_embed(array, n_embeddings)
+            array = array @ self.pca_components
+            if self.load_memmaps:
+                array = misc.array_to_memmap(prepared_data_file, array)
+            return array
+
+        # Apply TDE and PCA in parallel
+        args = zip(arrays, self.prepared_data_filenames)
+        self.arrays = pqdm(
+            args,
+            function=_apply,
+            desc="TDE-PCA",
+            n_jobs=self.n_jobs,
+            argument_type="args",
+            total=self.n_arrays,
         )
+        if any([isinstance(e, Exception) for e in self.arrays]):
+            for i, e in enumerate(self.arrays):
+                if isinstance(e, Exception):
+                    e.args = (f"array {i}: {e}",)
+                    _logger.exception(e, exc_info=False)
+            raise e
+
+        return self
+
+    def amplitude_envelope(self):
+        """Calculate the amplitude envelope.
 
-        prepared_data_memmaps = pqdm(
-            prepare_args,
-            self.apply_tde_pca,
-            desc="Preparing data",
+        This is an in-place operation.
+
+        Returns
+        -------
+        data : osl_dynamics.data.Data
+            The modified Data object.
+        """
+
+        # Function to calculate amplitude envelope for a single array
+        def _apply(array, prepared_data_file):
+            array = processing.amplitude_envelope(array)
+            if self.load_memmaps:
+                array = misc.array_to_memmap(prepared_data_file, array)
+            return array
+
+        # Prepare the data in parallel
+        args = zip(self.arrays, self.prepared_data_filenames)
+        self.arrays = pqdm(
+            args,
+            function=_apply,
+            desc="Amplitude envelope",
             n_jobs=self.n_jobs,
             argument_type="args",
-            total=len(self.raw_data_memmaps),
+            total=self.n_arrays,
         )
-        self.prepared_data_memmaps.extend(prepared_data_memmaps)
+        if any([isinstance(e, Exception) for e in self.arrays]):
+            for i, e in enumerate(self.arrays):
+                if isinstance(e, Exception):
+                    e.args = (f"array {i}: {e}",)
+                    _logger.exception(e, exc_info=False)
+            raise e
 
-        # Update subjects to return the prepared data
-        self.subjects = self.prepared_data_memmaps
+        return self
 
-        self.prepared = True
+    def moving_average(self, n_window, use_raw=False):
+        """Calculate a moving average.
 
-    def apply_tde_pca(self, raw_data_memmap, prepared_data_file):
-        """Applies time-delay embeddings, principal component analysis and
-        standardization to raw data.
+        This is an in-place operation.
 
         Parameters
         ----------
-        raw_data_memmap : np.memmap or np.ndarray
-            Raw data.
-        prepared_data_file : str
-            Name of memory map file to save prepared data to.
-            Can be None if we are not using memory maps.
+        n_window : int
+            Number of data points in the sliding window. Must be odd.
+        use_raw : bool
+            Should we prepare the original 'raw' data that we loaded?
 
         Returns
         -------
-        prepared_data_memmap : np.memmap or np.ndarray
-            Prepared data.
+        data : osl_dynamics.data.Data
+            The modified Data object.
         """
+        self.n_window = n_window
 
-        # Standardise and time embed the data
-        std_data = processing.standardize(raw_data_memmap)
-        te_std_data = processing.time_embed(std_data, self.n_embeddings)
+        # Function to apply sliding window to a single array
+        def _apply(array, prepared_data_file):
+            array = processing.moving_average(array, n_window)
+            if self.load_memmaps:
+                array = misc.array_to_memmap(prepared_data_file, array)
+            return array
 
-        # Apply PCA to get the prepared data
-        if self.pca_components is not None:
-            prepared_data = te_std_data @ self.pca_components
+        # Prepare the data in parallel
+        arrays = self.raw_data_arrays if use_raw else self.arrays
+        args = zip(arrays, self.prepared_data_filenames)
+        self.arrays = pqdm(
+            args,
+            function=_apply,
+            desc="Sliding window",
+            n_jobs=self.n_jobs,
+            argument_type="args",
+            total=self.n_arrays,
+        )
+        if any([isinstance(e, Exception) for e in self.arrays]):
+            for i, e in enumerate(self.arrays):
+                if isinstance(e, Exception):
+                    e.args = (f"array {i}: {e}",)
+                    _logger.exception(e, exc_info=False)
+            raise e
 
-        # Otherwise, the time embedded data is the prepared data
-        else:
-            prepared_data = te_std_data
+        return self
 
-        # Finally, we standardise
-        prepared_data = processing.standardize(prepared_data, create_copy=False)
+    def standardize(self):
+        """Standardize (z-transform) the data.
 
-        if self.load_memmaps:
-            # Save the prepared data as a memmap
-            prepared_data_memmap = misc.array_to_memmap(
-                prepared_data_file, prepared_data
-            )
-        else:
-            prepared_data_memmap = prepared_data
+        This is an in-place operation.
 
-        return prepared_data_memmap
+        Returns
+        -------
+        data : osl_dynamics.data.Data
+            The modified Data object.
+        """
 
-    def prepare_memmap_filenames(self):
-        prepared_data_pattern = "prepared_data_{{i:0{width}d}}_{identifier}.npy".format(
-            width=len(str(self.n_subjects)), identifier=self._identifier
+        # Function to apply standardisation to a single array
+        def _apply(array):
+            return processing.standardize(array, create_copy=False)
+
+        # Apply standardisation to each array in parallel
+        self.arrays = pqdm(
+            array=zip(self.arrays),
+            function=_apply,
+            desc="Standardize",
+            n_jobs=self.n_jobs,
+            argument_type="args",
+            total=self.n_arrays,
         )
-        self.prepared_data_filenames = [
-            str(self.store_dir / prepared_data_pattern.format(i=i))
-            for i in range(self.n_subjects)
-        ]
+        if any([isinstance(e, Exception) for e in self.arrays]):
+            for i, e in enumerate(self.arrays):
+                if isinstance(e, Exception):
+                    e.args = (f"array {i}: {e}",)
+                    _logger.exception(e, exc_info=False)
+            raise e
+
+        return self
 
-        self.prepared_data_memmaps = []
+    def prepare(self, methods):
+        """Prepare data.
+
+        Wrapper for calling a series of data preparation methods. Any method in
+        Data can be called.
+
+        Parameters
+        ----------
+        methods : dict
+            Each key is the name of a method to call. Each value is a dict
+            containing keyword arguments to pass to the method. Example use
+            for TDE-PCA data preparation::
+
+                methods = {
+                    "tde_pca": {"n_embeddings": 15, "n_pca_components": 80},
+                    "standardize": {},
+                }
+                data.prepare(methods)
+
+            Or for amplitude envelope data preparation::
+
+                methods = {
+                    "filter": {"low_freq": 1, "high_freq": 45},
+                    "amplitude_envelope": {},
+                    "moving_average": {"n_window": 5},
+                    "standardize": {},
+                }
+                data.prepare(methods)
+
+        Returns
+        -------
+        data : osl_dynamics.data.Data
+            The modified Data object.
+        """
+        for method_name, kwargs in methods.items():
+            method = getattr(self, method_name)
+            method(**kwargs)
+
+        return self
 
     def trim_time_series(
         self,
         sequence_length=None,
-        n_embeddings=1,
-        n_window=1,
+        n_embeddings=None,
+        n_window=None,
         prepared=True,
         concatenate=False,
+        verbose=False,
     ):
         """Trims the data time series.
 
         Removes the data points that are lost when the data is prepared,
         i.e. due to time embedding and separating into sequences, but does not
         perform time embedding or batching into sequences on the time series.
 
@@ -745,207 +853,181 @@
         n_embeddings : int
             Number of data points used to embed the data.
         n_window : int
             Number of data points the sliding window applied to the data.
         prepared : bool
             Should we return the prepared data? If not we return the raw data.
         concatenate : bool
-            Should we concatenate the data for each subject?
+            Should we concatenate the data for each array?
+        verbose : bool
+            Should we print the number of data points we're removing?
 
         Returns
         -------
         list of np.ndarray
-            Trimed time series for each subject.
+            Trimed time series for each array.
         """
-        if self.n_embeddings is None and self.n_window is None:
-            # Data has not been prepared so we can't trim the prepared data
-            prepared = False
-
-        if not prepared:
-            # We're trimming the raw data, how many data points do we
-            # need to remove due to time embedding or moving average?
-            if self.amplitude_envelope:
-                n_remove = self.n_window or n_window
-            else:
-                n_remove = self.n_embeddings or n_embeddings
+        # How many time points from the start/end of the time series should
+        # we remove?
+        n_remove = 0
+        if n_embeddings is None:
+            if hasattr(self, "n_embeddings"):
+                n_remove += self.n_embeddings // 2
+        else:
+            n_remove += n_embeddings // 2
+        if n_window is None:
+            if hasattr(self, "n_window"):
+                n_remove += self.n_window // 2
         else:
-            n_remove = 1
+            n_remove += n_window // 2
+        if verbose:
+            _logger.info(
+                f"Removing {n_remove} data points from the start and end"
+                + " of each array due to time embedding/sliding window."
+            )
 
         # What data should we trim?
         if prepared:
-            memmaps = self.subjects
+            arrays = self.arrays
         else:
-            memmaps = self.raw_data_memmaps
+            arrays = self.raw_data_arrays
 
         trimmed_time_series = []
-        for memmap in memmaps:
-            # Remove data points lost to time embedding
-            if n_remove != 1:
-                memmap = memmap[n_remove // 2 : -(n_remove // 2)]
+        for i, array in enumerate(arrays):
+            # Remove data points lost to time embedding or sliding window
+            if n_remove != 0:
+                array = array[n_remove:-n_remove]
 
             # Remove data points lost to separating into sequences
             if sequence_length is not None:
-                n_sequences = memmap.shape[0] // sequence_length
-                memmap = memmap[: n_sequences * sequence_length]
+                n_sequences = array.shape[0] // sequence_length
+                n_keep = n_sequences * sequence_length
+                if verbose:
+                    _logger.info(
+                        f"Removing {array.shape[0] - n_keep} data points"
+                        + f" from the end of array {i} due to sequencing."
+                    )
+                array = array[:n_keep]
 
-            trimmed_time_series.append(memmap)
+            trimmed_time_series.append(array)
 
         if concatenate or len(trimmed_time_series) == 1:
             trimmed_time_series = np.concatenate(trimmed_time_series)
 
         return trimmed_time_series
 
-    def count_batches(self, sequence_length):
-        """Count batches.
+    def count_sequences(self, sequence_length, step_size):
+        """Count sequences.
 
         Parameters
         ----------
         sequence_length : int
             Length of the segement of data to feed into the model.
+        step_size : int
+            The number of samples by which to move the sliding window between sequences.
 
         Returns
         -------
         n : np.ndarray
-            Number of batches for each subject's data.
+            Number of sequences for each array's data.
         """
         return np.array(
-            [tf.n_batches(memmap, sequence_length) for memmap in self.subjects]
+            [
+                tf.get_n_sequences(array, sequence_length, step_size)
+                for array in self.arrays
+            ]
         )
 
     def dataset(
         self,
         sequence_length,
         batch_size,
         shuffle=True,
         validation_split=None,
-        alpha=None,
-        gamma=None,
-        n_alpha_embeddings=1,
         concatenate=True,
         subj_id=False,
         step_size=None,
     ):
-        """Create a tensorflow dataset for training or evaluation.
+        """Create a Tensorflow Dataset for training or evaluation.
 
         Parameters
         ----------
         sequence_length : int
             Length of the segement of data to feed into the model.
         batch_size : int
             Number sequences in each mini-batch which is used to train the model.
         shuffle : bool
             Should we shuffle sequences (within a batch) and batches.
         validation_split : float
             Ratio to split the dataset into a training and validation set.
-        alpha : list of np.ndarray
-            List of mode mixing factors for each subject.
-            If passed, we create a dataset that includes alpha at each time point.
-            Optional. Such a dataset is used to train an observation model.
-        gamma : list of np.ndarray
-            List of mode mixing factors for the functional connectivity.
-            Optional. Used with a multi-dynamic model when training the observation
-            model only.
-        n_alpha_embeddings : int
-            Number of embeddings used when inferring alpha. Optional. Only should be
-            used if passing alpha (or gamma).
         concatenate : bool
-            Should we concatenate the datasets for each subject? Optional, default
+            Should we concatenate the datasets for each array? Optional, default
             is True.
         subj_id : bool
             Should we include the subject id in the dataset? Optional, default is
             False. This argument can be used to prepare datasets for subject-specific
             models.
         step_size : int
             Number of samples to slide the sequence across the dataset. Optional.
             Default is no overlap.
 
         Returns
         -------
-        tensorflow.data.Dataset or Tuple
+        dataset : tensorflow.data.Dataset or tuple
             Dataset for training or evaluating the model along with the validation
             set if validation_split was passed.
         """
-        self.n_batches = self.count_batches(sequence_length)
         self.sequence_length = sequence_length
         self.batch_size = batch_size
         self.step_size = step_size or sequence_length
-        n_embeddings = self.n_embeddings or 1
 
-        # Dataset for learning alpha and the observation model
-        if alpha is None:
-            subject_datasets = []
-            for i in range(self.n_subjects):
-                subject = self.subjects[i]
-                if subj_id:
-                    subject_tracker = np.zeros(subject.shape[0], dtype=np.float32) + i
-                    dataset = tf.create_dataset(
-                        {"data": subject, "subj_id": subject_tracker},
-                        self.sequence_length,
-                        self.step_size,
-                    )
-                else:
-                    dataset = tf.create_dataset(
-                        {"data": subject}, self.sequence_length, self.step_size
-                    )
-                subject_datasets.append(dataset)
-
-        # Dataset for learning the observation model
-        else:
-            if not isinstance(alpha, list):
-                raise ValueError("alpha must be a list of numpy arrays.")
+        n_sequences = self.count_sequences(self.sequence_length, self.step_size)
 
-            subject_datasets = []
-            for i in range(self.n_subjects):
-                if n_embeddings > n_alpha_embeddings:
-                    # We remove data points in alpha that are not in the new time
-                    # embedded data
-                    alp = alpha[i][(n_embeddings - n_alpha_embeddings) // 2 :]
-                    if gamma is not None:
-                        gam = gamma[i][(n_embeddings - n_alpha_embeddings) // 2 :]
-                    subject = self.subjects[i][: alp.shape[0]]
-
-                else:
-                    # We remove the data points that are not in alpha
-                    alp = alpha[i]
-                    if gamma is not None:
-                        gam = gamma[i]
-                    subject = self.subjects[i][
-                        (n_alpha_embeddings - n_embeddings) // 2 : alp.shape[0]
-                    ]
-
-                # Create dataset
-                input_data = {"data": subject, "alpha": alp}
-                if gamma is not None:
-                    input_data["gamma"] = gam
-                if subj_id:
-                    input_data["subj_id"] = (
-                        np.zeros(subject.shape[0], dtype=np.float32) + i
-                    )
+        datasets = []
+        for i in range(self.n_arrays):
+            if i not in self.keep:
+                # We don't want to include this file in the dataset
+                continue
+
+            # Get time series data and ensure an integer multiple of sequence length
+            array = self.arrays[i][: n_sequences[i] * sequence_length]
+
+            if subj_id:
+                # Create a dataset with the time series data and ID
+                array_tracker = np.zeros(array.shape[0], dtype=np.float32) + i
                 dataset = tf.create_dataset(
-                    input_data, self.sequence_length, self.step_size
+                    {"data": array, "subj_id": array_tracker},
+                    self.sequence_length,
+                    self.step_size,
                 )
-                subject_datasets.append(dataset)
+            else:
+                # Createa a dataset with just the time series data
+                dataset = tf.create_dataset(
+                    {"data": array}, self.sequence_length, self.step_size
+                )
+
+            datasets.append(dataset)
 
-        # Create a dataset from all the subjects concatenated
+        # Create a dataset from all the arrays concatenated
         if concatenate:
-            full_dataset = tf.concatenate_datasets(subject_datasets, shuffle=False)
+            full_dataset = tf.concatenate_datasets(datasets)
 
             if shuffle:
                 # Shuffle sequences
-                full_dataset = full_dataset.shuffle(100000)
+                full_dataset = full_dataset.shuffle(self.buffer_size)
 
                 # Group into mini-batches
-                full_dataset = full_dataset.batch(batch_size)
+                full_dataset = full_dataset.batch(self.batch_size)
 
                 # Shuffle mini-batches
-                full_dataset = full_dataset.shuffle(100000)
+                full_dataset = full_dataset.shuffle(self.buffer_size)
 
             else:
                 # Group into mini-batches
-                full_dataset = full_dataset.batch(batch_size)
+                full_dataset = full_dataset.batch(self.batch_size)
 
             if validation_split is None:
                 # Return the full dataset
                 return full_dataset.prefetch(-1)
 
             else:
                 # Calculate how many batches should be in the training dataset
@@ -958,52 +1040,140 @@
                 _logger.info(
                     f"{len(training_dataset)} batches in training dataset, "
                     + f"{len(validation_dataset)} batches in the validation dataset."
                 )
 
                 return training_dataset.prefetch(-1), validation_dataset.prefetch(-1)
 
-        # Otherwise create a dataset for each subject separately
+        # Otherwise create a dataset for each array separately
         else:
             full_datasets = []
-            for ds in subject_datasets:
+            for ds in datasets:
                 if shuffle:
                     # Shuffle sequences
-                    ds = ds.shuffle(100000)
+                    ds = ds.shuffle(self.buffer_size)
 
                 # Group into batches
-                ds = ds.batch(batch_size)
+                ds = ds.batch(self.batch_size)
 
                 if shuffle:
                     # Shuffle batches
-                    ds = ds.shuffle(100000)
+                    ds = ds.shuffle(self.buffer_size)
 
                 full_datasets.append(ds.prefetch(-1))
 
             if validation_split is None:
-                # Return the full dataset for each subject
+                # Return the full dataset for each array
                 return full_datasets
 
             else:
-                # Split the dataset for each subject separately
+                # Split the dataset for each array separately
                 training_datasets = []
                 validation_datasets = []
                 for i in range(len(full_datasets)):
                     # Calculate the number of batches in the training dataset
                     dataset_size = len(full_datasets[i])
                     training_dataset_size = round(
                         (1.0 - validation_split) * dataset_size
                     )
 
-                    # Split this subject's dataset
+                    # Split this array's dataset
                     training_datasets.append(
                         full_datasets[i].take(training_dataset_size)
                     )
                     validation_datasets.append(
                         full_datasets[i].skip(training_dataset_size)
                     )
                     _logger.info(
                         f"Subject {i}: "
                         + f"{len(training_datasets[i])} batches in training dataset, "
-                        + f"{len(validation_datasets[i])} batches in the validation dataset."
+                        + f"{len(validation_datasets[i])} batches in the validation "
+                        + "dataset."
                     )
                 return training_datasets, validation_datasets
+
+    def save_preparation(self, output_dir="."):
+        """Save a pickle file containing preparation settings.
+
+        Parameters
+        ----------
+        output_dir : str
+            Path to save data files to. Default is the current working directory.
+        """
+        attributes = list(self.__dict__.keys())
+        dont_keep = [
+            "_identifier",
+            "data_field",
+            "picks",
+            "reject_by_annotation",
+            "sampling_frequency",
+            "mask_file",
+            "parcellation_file",
+            "time_axis_first",
+            "load_memmaps",
+            "buffer_size",
+            "n_jobs",
+            "prepared_data_filenames",
+            "inputs",
+            "store_dir",
+            "raw_data_arrays",
+            "raw_data_filenames",
+            "n_raw_data_channels",
+            "arrays",
+            "keep",
+        ]
+        for item in dont_keep:
+            if item in attributes:
+                attributes.remove(item)
+        preparation = {a: getattr(self, a) for a in attributes}
+        pickle.dump(preparation, open(f"{output_dir}/preparation.pkl", "wb"))
+
+    def load_preparation(self, inputs):
+        """Loads a pickle file containing preparation settings.
+
+        Parameters
+        ----------
+        inputs : str
+            Path to directory containing the pickle file with preparation settings.
+        """
+        if path.isdir(inputs):
+            for file in rw.list_dir(inputs):
+                if "preparation.pkl" in file:
+                    preparation = pickle.load(open(f"{inputs}/preparation.pkl", "rb"))
+                    for attr, value in preparation.items():
+                        setattr(self, attr, value)
+                    break
+
+    def save(self, output_dir="."):
+        """Saves (prepared) data to numpy files.
+
+        Parameters
+        ----------
+        output_dir : str
+            Path to save data files to. Default is the current working directory.
+        """
+        # Create output directory
+        output_dir = pathlib.Path(output_dir)
+        output_dir.mkdir(parents=True, exist_ok=True)
+
+        # Function to save a single array
+        def _save(i, arr):
+            padded_number = misc.leading_zeros(i, self.n_arrays)
+            np.save(f"{output_dir}/array{padded_number}.npy", arr)
+
+        # Save arrays in parallel
+        pqdm(
+            enumerate(self.arrays),
+            _save,
+            desc="Saving data",
+            n_jobs=self.n_jobs,
+            argument_type="args",
+            total=self.n_arrays,
+        )
+
+        # Save preparation settings
+        self.save_preparation(output_dir)
+
+    def delete_dir(self):
+        """Deletes store_dir."""
+        if self.store_dir.exists():
+            rmtree(self.store_dir)
```

### Comparing `osl-dynamics-1.2.4/osl_dynamics/data/rw.py` & `osl-dynamics-1.2.5/osl_dynamics/data/rw.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 """Functions for reading and writing data.
 
 """
 
 import logging
-import warnings
 from os import listdir, path
 
 import mne
 import mat73
 import numpy as np
 import scipy.io
 
-from osl_dynamics.data import spm
-
 _logger = logging.getLogger("osl-dynamics")
 _allowed_ext = [".npy", ".mat", ".txt", ".fif"]
 
 
 def validate_inputs(inputs):
     """Validates inputs.
 
@@ -235,52 +232,37 @@
             verbose=False,
         ).T
     elif "epo.fif" in filename:
         epochs = mne.read_epochs(filename, verbose=False)
         data = epochs.get_data(picks=picks)
         data = np.swapaxes(data, 1, 2).reshape(-1, data.shape[1])
     else:
-        raise ValueError(f"a fif file must end with 'raw.fif' or 'epo.fif'.")
+        raise ValueError("a fif file must end with 'raw.fif' or 'epo.fif'.")
     return data
 
 
-def load_matlab(filename, field, ignored_keys=None):
-    """Loads a MATLAB or SPM file.
+def load_matlab(filename, field):
+    """Loads a MATLAB file.
 
     Parameters
     ----------
     filename : str
         Filename of MATLAB file to read.
     field : str
         Field that corresponds to the data.
-    ignored_keys :  list of str
-        Keys in the MATLAB file to ignore.
 
     Returns
     -------
     data : np.ndarray
-        Data in the MATLAB/SPM file.
+        Data in the MATLAB file.
     """
-    # Load file
     mat = loadmat(filename, return_dict=True)
-
-    # Get data
-    if "D" in mat:
-        warnings.warn(
-            "Assuming that key 'D' corresponds to an SPM MEEG object.", RuntimeWarning
-        )
-        D = spm.SPM(filename)
-        data = D.data
-    else:
-        try:
-            data = mat[field]
-        except KeyError:
-            raise KeyError(f"field '{field}' missing from MATLAB file.")
-
-    return data
+    if field not in mat:
+        raise KeyError(f"field '{field}' missing from MATLAB file.")
+    return mat[field]
 
 
 def loadmat(filename, return_dict=False):
     """Wrapper for scipy.io.loadmat or mat73.loadmat.
 
     Parameters
     ----------
```

### Comparing `osl-dynamics-1.2.4/osl_dynamics/data/task.py` & `osl-dynamics-1.2.5/osl_dynamics/data/task.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/data/tf.py` & `osl-dynamics-1.2.5/osl_dynamics/data/tf.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,70 +1,56 @@
 """Function related to TensorFlow datasets.
 
 """
 
 import numpy as np
 
 
-def n_batches(arr, sequence_length, step_size=None):
-    """Calculate the number of batches an array will be split into.
+def get_n_sequences(arr, sequence_length, step_size=None):
+    """Calculate the number of sequences an array will be split into.
 
     Parameters
     ----------
     arr : numpy.ndarray
         Time series data.
     sequence_length : int
         Length of sequences which the data will be segmented in to.
     step_size : int
         The number of samples by which to move the sliding window between sequences.
 
     Returns
     -------
     n : int
-        Number of batches.
+        Number of sequences.
     """
     step_size = step_size or sequence_length
-    final_slice_start = arr.shape[0] - sequence_length + 1
-    index = np.arange(0, final_slice_start, step_size)[:, None] + np.arange(
-        sequence_length
-    )
-    return len(index)
+    n_samples = (arr.shape[0] // sequence_length) * sequence_length
+    return n_samples // step_size
 
 
-def concatenate_datasets(datasets, shuffle=True):
+def concatenate_datasets(datasets):
     """Concatenates a list of TensorFlow datasets.
 
     Parameters
     ----------
     datasets : list
         List of TensorFlow datasets.
-    Shuffle : bool
-        Should we shuffle the final concatenated dataset?
 
     Returns
     -------
     full_dataset : tensorflow.data.Dataset
         Concatenated dataset.
     """
-
     full_dataset = datasets[0]
     for ds in datasets[1:]:
         full_dataset = full_dataset.concatenate(ds)
-
-    if shuffle:
-        full_dataset = full_dataset.shuffle(100000)
-
     return full_dataset
 
 
-def create_dataset(
-    data,
-    sequence_length,
-    step_size,
-):
+def create_dataset(data, sequence_length, step_size):
     """Creates a TensorFlow dataset of batched time series data.
 
     Parameters
     ----------
     data : dict
         Dictionary containing data to batch. Keys correspond to the input name
         for the model and the value is the data.
```

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/__init__.py` & `osl-dynamics-1.2.5/osl_dynamics/files/__init__.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/mask/MNI152_T1_8mm_brain.nii.gz` & `osl-dynamics-1.2.5/osl_dynamics/files/mask/MNI152_T1_8mm_brain.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/mask/ParcellationPilot.L.inflated.32k_fs_LR.surf.gii` & `osl-dynamics-1.2.5/osl_dynamics/files/mask/ParcellationPilot.L.inflated.32k_fs_LR.surf.gii`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/mask/ParcellationPilot.L.midthickness.32k_fs_LR.surf.gii` & `osl-dynamics-1.2.5/osl_dynamics/files/mask/ParcellationPilot.L.midthickness.32k_fs_LR.surf.gii`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/mask/ParcellationPilot.L.very_inflated.32k_fs_LR.surf.gii` & `osl-dynamics-1.2.5/osl_dynamics/files/mask/ParcellationPilot.L.very_inflated.32k_fs_LR.surf.gii`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/mask/ParcellationPilot.R.inflated.32k_fs_LR.surf.gii` & `osl-dynamics-1.2.5/osl_dynamics/files/mask/ParcellationPilot.R.inflated.32k_fs_LR.surf.gii`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/mask/ParcellationPilot.R.midthickness.32k_fs_LR.surf.gii` & `osl-dynamics-1.2.5/osl_dynamics/files/mask/ParcellationPilot.R.midthickness.32k_fs_LR.surf.gii`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/mask/ParcellationPilot.R.very_inflated.32k_fs_LR.surf.gii` & `osl-dynamics-1.2.5/osl_dynamics/files/mask/ParcellationPilot.R.very_inflated.32k_fs_LR.surf.gii`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/mask/__init__.py` & `osl-dynamics-1.2.5/osl_dynamics/files/mask/__init__.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/mask/ft_8mm_brain_mask.nii.gz` & `osl-dynamics-1.2.5/osl_dynamics/files/mask/ft_8mm_brain_mask.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/parcellation/Glasser50_space-MNI152NLin6_res-8x8x8.nii.gz` & `osl-dynamics-1.2.5/osl_dynamics/files/parcellation/Glasser50_space-MNI152NLin6_res-8x8x8.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/parcellation/Glasser52_binary_space-MNI152NLin6_res-8x8x8.nii.gz` & `osl-dynamics-1.2.5/osl_dynamics/files/parcellation/Glasser52_binary_space-MNI152NLin6_res-8x8x8.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/parcellation/__init__.py` & `osl-dynamics-1.2.5/osl_dynamics/files/parcellation/__init__.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/parcellation/aal_cortical_merged_8mm_stacked.nii.gz` & `osl-dynamics-1.2.5/osl_dynamics/files/parcellation/aal_cortical_merged_8mm_stacked.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/parcellation/fMRI_parcellation_ds8mm.nii.gz` & `osl-dynamics-1.2.5/osl_dynamics/files/parcellation/fMRI_parcellation_ds8mm.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_3PCC_ips_reduced_2mm_ss5mm_ds8mm.nii.gz` & `osl-dynamics-1.2.5/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_3PCC_ips_reduced_2mm_ss5mm_ds8mm.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_3PCC_ips_reduced_2mm_ss5mm_ds8mm_adj.nii.gz` & `osl-dynamics-1.2.5/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_3PCC_ips_reduced_2mm_ss5mm_ds8mm_adj.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_reduced_2mm_ss5mm_ds8mm.nii.gz` & `osl-dynamics-1.2.5/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_reduced_2mm_ss5mm_ds8mm.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_tighterMay15_v2_6mm_exclusive.nii.gz` & `osl-dynamics-1.2.5/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_tighterMay15_v2_6mm_exclusive.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_tighterMay15_v2_8mm.nii.gz` & `osl-dynamics-1.2.5/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_tighterMay15_v2_8mm.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/parcellation/giles_39_binary.nii.gz` & `osl-dynamics-1.2.5/osl_dynamics/files/parcellation/giles_39_binary.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/ctf275_channel_names.npy` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/ctf275_channel_names.npy`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/4D148.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/4D148.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/4D248.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/4D248.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/4D248_helmet.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/4D248_helmet.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/4D248_helmet.outline` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/4D248_helmet.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/CTF151.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/CTF151.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/CTF151_helmet.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/CTF151_helmet.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/CTF151_helmet.outline` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/CTF151_helmet.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/CTF275.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/CTF275.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/CTF275_helmet.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/CTF275_helmet.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/CTF275_helmet.outline` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/CTF275_helmet.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/EEG1005.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/EEG1005.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/EEG1010.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/EEG1010.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/EEG1020.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/EEG1020.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/QuikCap_NSL_128.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/QuikCap_NSL_128.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/QuikCap_NSL_128.outline` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/QuikCap_NSL_128.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/acticap-64ch-standard2.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/acticap-64ch-standard2.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/acticap-64ch-standard2.outline` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/acticap-64ch-standard2.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/biosemi128.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/biosemi128.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/biosemi16.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/biosemi16.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/biosemi160.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/biosemi160.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/biosemi256.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/biosemi256.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/biosemi32.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/biosemi32.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/biosemi64.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/biosemi64.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/dccn_customized_acticap64.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/dccn_customized_acticap64.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/dccn_customized_acticap64.outline` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/dccn_customized_acticap64.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM1.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM1.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM1.outline` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM1.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM10.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM10.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM10.outline` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM10.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM11.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM11.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM11.outline` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM11.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM14.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM14.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM14.outline` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM14.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM15.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM15.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM15.outline` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM15.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM16.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM16.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM16.outline` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM16.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM17.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM17.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM17.outline` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM17.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM20.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM20.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM20.outline` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM20.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM22.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM22.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM22.outline` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM22.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM23.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM23.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM23.outline` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM23.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM24.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM24.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM24.outline` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM24.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM25.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM25.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM25.outline` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM25.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM3.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM3.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM3.outline` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM3.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM7.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM7.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/easycapM7.outline` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/easycapM7.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/elec1005.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/elec1005.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/elec1010.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/elec1010.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/elec1020.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/elec1020.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/mpi_customized_acticap64.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/mpi_customized_acticap64.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/mpi_customized_acticap64.outline` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/mpi_customized_acticap64.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/natmeg_customized_eeg1005.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/natmeg_customized_eeg1005.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/neuromag122cmb.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/neuromag122cmb.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/neuromag122planar.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/neuromag122planar.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/neuromag306all.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/neuromag306all.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/neuromag306all_helmet.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/neuromag306all_helmet.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/neuromag306all_helmet.outline` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/neuromag306all_helmet.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/neuromag306cmb.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/neuromag306cmb.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/neuromag306cmb_helmet.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/neuromag306cmb_helmet.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/neuromag306cmb_helmet.outline` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/neuromag306cmb_helmet.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/neuromag306mag.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/neuromag306mag.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/neuromag306mag_helmet.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/neuromag306mag_helmet.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/neuromag306mag_helmet.outline` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/neuromag306mag_helmet.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/neuromag306planar.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/neuromag306planar.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/neuromag306planar_helmet.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/neuromag306planar_helmet.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/neuromag306planar_helmet.outline` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/neuromag306planar_helmet.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/quickcap64.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/quickcap64.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/quickcap64.outline` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/quickcap64.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/yokogawa440.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/yokogawa440.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/yokogawa440_old.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/yokogawa440_old.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/yokogawa440ag.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/yokogawa440ag.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/yokogawa440all.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/yokogawa440all.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/layouts/yokogawa440pg.lay` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/layouts/yokogawa440pg.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scanner/neuromag306_channel_names.npy` & `osl-dynamics-1.2.5/osl_dynamics/files/scanner/neuromag306_channel_names.npy`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/files/scene/mode_scene.scene` & `osl-dynamics-1.2.5/osl_dynamics/files/scene/mode_scene.scene`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/inference/callbacks.py` & `osl-dynamics-1.2.5/osl_dynamics/inference/callbacks.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/inference/initializers.py` & `osl-dynamics-1.2.5/osl_dynamics/inference/initializers.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/inference/layers.py` & `osl-dynamics-1.2.5/osl_dynamics/inference/layers.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/inference/metrics.py` & `osl-dynamics-1.2.5/osl_dynamics/inference/metrics.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/inference/modes.py` & `osl-dynamics-1.2.5/osl_dynamics/inference/modes.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/inference/regularizers.py` & `osl-dynamics-1.2.5/osl_dynamics/inference/regularizers.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/inference/tf_ops.py` & `osl-dynamics-1.2.5/osl_dynamics/inference/tf_ops.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/models/__init__.py` & `osl-dynamics-1.2.5/osl_dynamics/models/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,29 @@
 """Implemented models.
 
 """
 import yaml
 
 from osl_dynamics.models import (
     dynemo,
-    dynemo_obs,
     mage,
     sage,
     mdynemo,
-    mdynemo_obs,
     sedynemo,
-    sedynemo_obs,
     state_dynemo,
     hmm,
 )
 from osl_dynamics.utils.misc import NumpyLoader
 
 models = {
     "DyNeMo": dynemo.Model,
-    "DyNeMo-Obs": dynemo_obs.Model,
     "MAGE": mage.Model,
     "SAGE": sage.Model,
     "M-DyNeMo": mdynemo.Model,
-    "M-DyNeMo-Obs": mdynemo_obs.Model,
     "SE-DyNeMo": sedynemo.Model,
-    "SE-DyNeMo-Obs": sedynemo_obs.Model,
     "State-DyNeMo": state_dynemo.Model,
     "HMM": hmm.Model,
 }
 
 
 def load(dirname):
     """Load model from dirname.
```

### Comparing `osl-dynamics-1.2.4/osl_dynamics/models/dynemo.py` & `osl-dynamics-1.2.5/osl_dynamics/models/sage.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,57 +1,50 @@
-"""Dynamic Network Modes (DyNeMo).
+"""Single-dynamic Adversarial Generator Encoder (SAGE).
 
 """
 
+import logging
+import time
 from dataclasses import dataclass
 from typing import Literal
 
 import numpy as np
-import tensorflow as tf
-from tensorflow.keras import layers
+from tensorflow.keras import layers, models, optimizers, utils
 from tqdm.auto import trange
 
 from osl_dynamics.inference.layers import (
+    AdversarialLogLikelihoodLossLayer,
+    ConcatVectorsMatricesLayer,
     CovarianceMatricesLayer,
-    DiagonalMatricesLayer,
     InferenceRNNLayer,
-    KLDivergenceLayer,
-    KLLossLayer,
-    LogLikelihoodLossLayer,
     MixMatricesLayer,
     MixVectorsLayer,
     ModelRNNLayer,
-    NormalizationLayer,
-    SampleNormalDistributionLayer,
-    SoftmaxLayer,
     VectorsLayer,
 )
-from osl_dynamics.models import dynemo_obs
-from osl_dynamics.models.inf_mod_base import (
-    VariationalInferenceModelBase,
-    VariationalInferenceModelConfig,
-)
-from osl_dynamics.models.mod_base import BaseModelConfig
+from osl_dynamics.models import obs_mod
+from osl_dynamics.models.mod_base import BaseModelConfig, ModelBase
+
+_logger = logging.getLogger("osl-dynamics")
 
 
 @dataclass
-class Config(BaseModelConfig, VariationalInferenceModelConfig):
-    """Settings for DyNeMo.
+class Config(BaseModelConfig):
+    """Settings for SAGE.
 
     Parameters
     ----------
     model_name : str
         Model name.
     n_modes : int
         Number of modes.
     n_channels : int
         Number of channels.
     sequence_length : int
-        Length of sequence passed to the inference network and generative model.
-
+        Length of sequence passed to the inference, generative and discriminator network.
     inference_rnn : str
         RNN to use, either 'gru' or 'lstm'.
     inference_n_layers : int
         Number of layers.
     inference_n_units : int
         Number of units.
     inference_normalization : str
@@ -76,443 +69,549 @@
         Type of activation to use after normalization and before dropout.
         E.g. 'relu', 'elu', etc.
     model_dropout : float
         Dropout rate.
     model_regularizer : str
         Regularizer.
 
-    theta_normalization : str
-        Type of normalization to apply to the posterior samples, theta.
-        Either 'layer', 'batch' or None.
-    learn_alpha_temperature : bool
-        Should we learn the alpha temperature?
-    initial_alpha_temperature : float
-        Initial value for the alpha temperature.
+    discriminator_rnn : str
+        RNN to use, either 'gru' or 'lstm'.
+    discriminator_n_layers : int
+        Number of layers.
+    discriminator_n_units : int
+        Number of units.
+    discriminator_normalization : str
+        Type of normalization to use. Either None, 'batch' or 'layer'.
+    discriminator_activation : str
+        Type of activation to use after normalization and before dropout.
+        E.g. 'relu', 'elu', etc.
+    discriminator_dropout : float
+        Dropout rate.
+    discriminator_regularizer : str
+        Regularizer.
 
     learn_means : bool
         Should we make the mean vectors for each mode trainable?
     learn_covariances : bool
         Should we make the covariance matrix for each mode trainable?
     initial_means : np.ndarray
         Initialisation for mean vectors.
     initial_covariances : np.ndarray
-        Initialisation for state covariances. If diagonal_covariances=True
-        and full matrices are passed, the diagonal is extracted.
+        Initialisation for mode covariances.
     covariances_epsilon : float
         Error added to mode covariances for numerical stability.
-    diagonal_covariances : bool
-        Should we learn diagonal mode covariances?
-    means_regularizer : tf.keras.regularizers.Regularizer
-        Regularizer for mean vectors.
-    covariances_regularizer : tf.keras.regularizers.Regularizer
-        Regularizer for covariance matrices.
-
-    do_kl_annealing : bool
-        Should we use KL annealing during training?
-    kl_annealing_curve : str
-        Type of KL annealing curve. Either 'linear' or 'tanh'.
-    kl_annealing_sharpness : float
-        Parameter to control the shape of the annealing curve if
-        kl_annealing_curve='tanh'.
-    n_kl_annealing_epochs : int
-        Number of epochs to perform KL annealing.
 
     batch_size : int
         Mini-batch size.
     learning_rate : float
         Learning rate.
-    gradient_clip : float
-        Value to clip gradients by. This is the clipnorm argument passed to
-        the Keras optimizer. Cannot be used if multi_gpu=True.
     n_epochs : int
         Number of training epochs.
     optimizer : str or tensorflow.keras.optimizers.Optimizer
         Optimizer to use. 'adam' is recommended.
     multi_gpu : bool
         Should be use multiple GPUs for training?
     strategy : str
         Strategy for distributed learning.
     """
 
-    model_name: str = "DyNeMo"
+    model_name: str = "SAGE"
 
     # Inference network parameters
     inference_rnn: Literal["gru", "lstm"] = "lstm"
     inference_n_layers: int = 1
     inference_n_units: int = None
     inference_normalization: Literal[None, "batch", "layer"] = None
-    inference_activation: str = None
+    inference_activation: str = "elu"
     inference_dropout: float = 0.0
     inference_regularizer: str = None
 
     # Model network parameters
     model_rnn: Literal["gru", "lstm"] = "lstm"
     model_n_layers: int = 1
     model_n_units: int = None
     model_normalization: Literal[None, "batch", "layer"] = None
-    model_activation: str = None
+    model_activation: str = "elu"
     model_dropout: float = 0.0
     model_regularizer: str = None
 
+    # Descriminator network parameters
+    discriminator_rnn: Literal["gru", "lstm"] = "lstm"
+    discriminator_n_layers: int = 1
+    discriminator_n_units: int = None
+    discriminator_normalization: Literal[None, "batch", "layer"] = None
+    discriminator_activation: str = "elu"
+    discriminator_dropout: float = 0.0
+    discriminator_regularizer: str = None
+
     # Observation model parameters
     learn_means: bool = None
     learn_covariances: bool = None
     initial_means: np.ndarray = None
     initial_covariances: np.ndarray = None
-    diagonal_covariances: bool = False
     covariances_epsilon: float = None
-    means_regularizer: tf.keras.regularizers.Regularizer = None
-    covariances_regularizer: tf.keras.regularizers.Regularizer = None
 
     def __post_init__(self):
-        self.validate_rnn_parameters()
-        self.validate_observation_model_parameters()
-        self.validate_alpha_parameters()
-        self.validate_kl_annealing_parameters()
         self.validate_dimension_parameters()
         self.validate_training_parameters()
-
-    def validate_rnn_parameters(self):
-        if self.inference_n_units is None:
-            raise ValueError("Please pass inference_n_units.")
-
-        if self.model_n_units is None:
-            raise ValueError("Please pass model_n_units.")
+        self.validate_observation_model_parameters()
 
     def validate_observation_model_parameters(self):
         if self.learn_means is None or self.learn_covariances is None:
             raise ValueError("learn_means and learn_covariances must be passed.")
 
         if self.covariances_epsilon is None:
             if self.learn_covariances:
                 self.covariances_epsilon = 1e-6
             else:
                 self.covariances_epsilon = 0.0
 
 
-class Model(VariationalInferenceModelBase):
-    """DyNeMo model class.
+class Model(ModelBase):
+    """SAGE model class.
 
     Parameters
     ----------
-    config : osl_dynamics.models.dynemo.Config
+    config : osl_dynamics.models.sage.Config
     """
 
     config_type = Config
 
     def build_model(self):
-        """Builds a keras model."""
-        self.model = _model_structure(self.config)
+        """Builds a keras model for the inference, generator and discriminator model
+        and the full SAGE model.
+        """
+        _logger.info("Build models")
+        self.inference_model = _build_inference_model(self.config)
+        self.inference_model.summary()
+        print()
+        self.generator_model = _build_generator_model(self.config)
+        self.generator_model.summary()
+        print()
+        self.discriminator_model = _build_discriminator_model(self.config)
+        self.discriminator_model.summary()
+        print()
+
+        data = layers.Input(
+            shape=(self.config.sequence_length, self.config.n_channels), name="data"
+        )
+        C_m, alpha_posterior = self.inference_model(data)
+        alpha_prior = self.generator_model(alpha_posterior)
+        discriminator_output_prior = self.discriminator_model(alpha_prior)
+        self.model = models.Model(data, [C_m, discriminator_output_prior], name="SAGE")
+        self.model.summary()
+        print()
+
+    def compile(self):
+        """Compile the model."""
+
+        self.discriminator_model.compile(
+            loss="binary_crossentropy",
+            optimizer=self.config.optimizer.lower(),
+            metrics=["accuracy"],
+        )
+        self.discriminator_model.trainable = False
+
+        # Reconstruction (Likelihood) loss:
+        # The first loss corresponds to the likelihood - this tells us how well we
+        # are explaining our data according to the current estimate of the
+        # generative model, and is given by:
+        # L = \sum_{t=1}^{T} log p(Y_t | \theta_t^m = \mu^{m,\theta}_t,
+        #                                \theta_t^c = \mu^{c,\theta}_t)
+        ll_loss = AdversarialLogLikelihoodLossLayer(
+            self.config.n_channels, name="ll_loss"
+        )
+
+        # Regularization (Prior) Loss:
+        # The second loss regularises the estimate of the latent, time-varying
+        # parameters [$\theta^m$, $\theta^c$] using an adaptive prior - this penalises
+        # when the posterior estimates of [$\theta^m$, $\theta^c$] deviate from the
+        # prior:
+        # R = \sum_{t=1}^{T} [
+        #     CrossEntropy(\mu^{m,\theta}_t|| \hat{\mu}^{m,\theta}_{t})
+        #     + CrossEntropy(\mu^{c,\theta}_t || \hat{\mu}^{c,\theta}_{t})
+        # ]
+
+        # Compile the full model
+        optimizer = optimizers.get(
+            {
+                "class_name": self.config.optimizer.lower(),
+                "config": {"learning_rate": self.config.learning_rate},
+            }
+        )
+        self.model.compile(
+            loss=[ll_loss, "binary_crossentropy"],
+            loss_weights=[0.995, 0.005],
+            optimizer=optimizer,
+        )
+
+    def fit(self, training_data, epochs=None, verbose=1):
+        """Train the model.
+
+        Parameters
+        ----------
+        training_data : tensorflow.data.Dataset or osl_dynamics.data.Data
+            Training dataset.
+        epochs : int
+            Number of epochs to train. Defaults to value in config if not passed.
+        verbose : int
+            Should we print a progress bar?
+
+        Returns
+        -------
+        history : history
+            History of discriminator_loss and generator_loss.
+        """
+        if epochs is None:
+            epochs = self.config.n_epochs
+
+        # Make sure training data is a TensorFlow Dataset
+        training_data = self.make_dataset(training_data, shuffle=True, concatenate=True)
+
+        # Path to save the best model weights
+        timestr = time.strftime("%Y%m%d-%H%M%S")  # current date-time
+        filepath = "tmp/"
+        save_filepath = filepath + str(timestr) + "_best_model.h5"
+
+        history = []
+        best_val_loss = np.Inf
+        for epoch in range(epochs):
+            if verbose:
+                print("Epoch {}/{}".format(epoch + 1, epochs))
+                pb_i = utils.Progbar(len(training_data), stateful_metrics=["D", "G"])
+
+            for idx, batch in enumerate(training_data):
+                # Generate real/fake input for the discriminator
+                real = np.ones((len(batch["data"]), self.config.sequence_length, 1))
+                fake = np.zeros((len(batch["data"]), self.config.sequence_length, 1))
+                train_discriminator = self._train_discriminator(real, fake)
+
+                C_m, alpha_posterior = self.inference_model.predict_on_batch(batch)
+                alpha_prior = self.generator_model.predict_on_batch(alpha_posterior)
+
+                # Train discriminator, inference and generator model
+                discriminator_loss = train_discriminator(alpha_posterior, alpha_prior)
+                generator_loss = self.model.train_on_batch(batch, [batch, real])
+
+                if verbose:
+                    pb_i.add(
+                        1,
+                        values=[("D", discriminator_loss[1]), ("G", generator_loss[0])],
+                    )
+
+            if generator_loss[0] < best_val_loss:
+                self.save_weights(save_filepath)
+                _logger.info(
+                    "Best model w/ val loss (generator) {} saved to {}".format(
+                        generator_loss[0], save_filepath
+                    )
+                )
+                best_val_loss = generator_loss[0]
+            val_loss = self.model.test_on_batch([batch], [batch, real])
+
+            history.append({"D": discriminator_loss[1], "G": generator_loss[0]})
+
+        # Load the weights for the best model
+        _logger.info(f"Loading best model: {save_filepath}")
+        self.load_weights(save_filepath)
+
+        return history
+
+    def _train_discriminator(self, real, fake):
+        def train(real_samples, fake_samples):
+            self.discriminator_model.trainable = True
+            loss_real = self.discriminator_model.train_on_batch(real_samples, real)
+            loss_fake = self.discriminator_model.train_on_batch(fake_samples, fake)
+            loss = np.add(loss_real, loss_fake) * 0.5
+            self.discriminator_model.trainable = False
+            return loss
+
+        return train
+
+    def get_alpha(self, inputs, concatenate=False):
+        """Mode mixing factors, alpha.
+
+        Parameters
+        ----------
+        inputs : tensorflow.data.Dataset or osl_dynamics.data.Data
+            Prediction data.
+
+        Returns
+        -------
+        alpha : list or np.ndarray
+            Mode mixing factors with shape (n_subjects, n_samples, n_modes) or
+            (n_samples, n_modes).
+        """
+        inputs = self.make_dataset(inputs, concatenate=concatenate)
+
+        _logger.info("Getting alpha:")
+        outputs = []
+        for dataset in inputs:
+            alpha = self.inference_model.predict(dataset)[1]
+            alpha = np.concatenate(alpha)
+            outputs.append(alpha)
+
+        if concatenate or len(outputs) == 1:
+            outputs = np.concatenate(outputs)
+
+        return outputs
+
+    def get_means(self):
+        """Get the mode means.
+
+        Returns
+        -------
+        means : np.ndarray
+            Mode means. Shape (n_modes, n_channels).
+        """
+        return obs_mod.get_observation_model_parameter(self.inference_model, "means")
 
     def get_covariances(self):
-        """Get the covariances of each mode.
+        """Get the mode covariances.
 
         Returns
         -------
         covariances : np.ndarary
-            Mode covariances.
+            Mode covariances. Shape (n_modes, n_channels, n_channels).
         """
-        return dynemo_obs.get_covariances(self.model)
+        return obs_mod.get_observation_model_parameter(self.inference_model, "covs")
 
     def get_means_covariances(self):
-        """Get the means and covariances of each mode.
+        """Get the mode means and covariances.
+        This is a wrapper for get_means and get_covariances.
 
         Returns
         -------
         means : np.ndarary
-            Mode means.
+            Mode means. Shape (n_modes, n_channels).
         covariances : np.ndarray
-            Mode covariances.
+            Mode covariances. Shape (n_modes, n_channels, n_channels).
         """
-        return dynemo_obs.get_means_covariances(self.model)
+        return self.get_means(), self.get_covariances()
 
     def get_observation_model_parameters(self):
         """Wrapper for get_means_covariances."""
         return self.get_means_covariances()
 
     def set_means(self, means, update_initializer=True):
-        """Set the means of each mode.
+        """Set the mode means.
 
         Parameters
         ----------
         means : np.ndarray
-            Mode covariances.
+            Mode means. Shape is (n_modes, n_channels).
         update_initializer : bool
             Do we want to use the passed means when we re-initialize
             the model?
         """
-        dynemo_obs.set_means(self.model, means, update_initializer)
+        obs_mod.set_observation_model_parameter(
+            self.inference_model,
+            means,
+            layer_name="means",
+            update_initializer=update_initializer,
+        )
 
     def set_covariances(self, covariances, update_initializer=True):
-        """Set the covariances of each mode.
+        """Set the mode covariances.
 
         Parameters
         ----------
         covariances : np.ndarray
-            Mode covariances.
+            Mode covariances. Shape is (n_modes, n_channels, n_channels).
         update_initializer : bool
             Do we want to use the passed covariances when we re-initialize
             the model?
         """
-        dynemo_obs.set_covariances(
-            self.model,
+        obs_mod.set_observation_model_parameter(
+            self.inference_model,
             covariances,
-            self.config.diagonal_covariances,
-            update_initializer,
+            layer_name="covs",
+            update_initializer=update_initializer,
+            diagonal_covariances=self.config.diagonal_covariances,
         )
 
-    def set_observation_model_parameters(
-        self, observation_model_parameters, update_initializer=True
-    ):
-        """Wrapper for set_means and set_covariances."""
+    def set_means_covariances(self, means, covariances, update_initializer=True):
+        """This is a wrapper for set_means and set_covariances."""
         self.set_means(
-            observation_model_parameters[0],
+            means,
             update_initializer=update_initializer,
         )
         self.set_covariances(
-            observation_model_parameters[1],
+            covariances,
             update_initializer=update_initializer,
         )
 
-    def set_regularizers(self, training_dataset):
-        """Set the means and covariances regularizer based on the training data.
-
-        A multivariate normal prior is applied to the mean vectors with mu = 0,
-        sigma=diag((range / 2)**2). If config.diagonal_covariances is True, a log
-        normal prior is applied to the diagonal of the covariances matrices with mu=0,
-        sigma=sqrt(log(2 * (range))), otherwise an inverse Wishart prior is applied
-        to the covariances matrices with nu=n_channels - 1 + 0.1 and psi=diag(1 / range).
-
-        Parameters
-        ----------
-        training_dataset : tensorflow.data.Dataset or osl_dynamics.data.Data
-            Training dataset.
-        """
-        training_dataset = self.make_dataset(training_dataset, concatenate=True)
-
-        if self.config.learn_means:
-            dynemo_obs.set_means_regularizer(self.model, training_dataset)
-
-        if self.config.learn_covariances:
-            dynemo_obs.set_covariances_regularizer(
-                self.model,
-                training_dataset,
-                self.config.covariances_epsilon,
-                self.config.diagonal_covariances,
-            )
+    def set_observation_model_parameters(
+        self, observation_model_parameters, update_initializer=True
+    ):
+        """Wrapper for set_means_covariances."""
+        self.set_means_covariances(
+            observation_model_parameters[0],
+            observation_model_parameters[1],
+            update_initializer=update_initializer,
+        )
 
-    def sample_alpha(self, n_samples, theta_norm=None):
-        """Uses the model RNN to sample mode mixing factors, alpha.
+    def sample_alpha(self, alpha=None):
+        """Uses the generator to predict the prior alphas.
 
         Parameters
         ----------
-        n_samples : int
-            Number of samples to take.
-        theta_norm : np.ndarray
-            Normalized logits to initialise the sampling with. Shape must be
-            (sequence_length, n_modes).
+        alpha : np.ndarray
+            Shape must be (n_samples, n_modes).
 
         Returns
         -------
         alpha : np.ndarray
-            Sampled alpha.
+            Predicted alpha.
         """
-        # Get layers
-        model_rnn_layer = self.model.get_layer("mod_rnn")
-        mod_mu_layer = self.model.get_layer("mod_mu")
-        mod_sigma_layer = self.model.get_layer("mod_sigma")
-        theta_norm_layer = self.model.get_layer("theta_norm")
-        alpha_layer = self.model.get_layer("alpha")
-
-        # Normally distributed random numbers used to sample the logits theta
-        epsilon = np.random.normal(0, 1, [n_samples + 1, self.config.n_modes]).astype(
-            np.float32
-        )
-
-        if theta_norm is None:
-            # Sequence of the underlying logits theta
-            theta_norm = np.zeros(
-                [self.config.sequence_length, self.config.n_modes],
-                dtype=np.float32,
-            )
-
-            # Randomly sample the first time step
-            theta_norm[-1] = np.random.normal(size=self.config.n_modes)
-
-        # Sample the mode fixing factors
-        alpha = np.empty([n_samples, self.config.n_modes], dtype=np.float32)
-        for i in trange(n_samples, desc="Sampling mode time course"):
-            # If there are leading zeros we trim theta so that we don't pass the zeros
-            trimmed_theta = theta_norm[~np.all(theta_norm == 0, axis=1)][
-                np.newaxis, :, :
-            ]
-
-            # Predict the probability distribution function for theta one time step
-            # in the future,
-            # p(theta|theta_<t) ~ N(mod_mu, sigma_theta_jt)
-            model_rnn = model_rnn_layer(trimmed_theta)
-            mod_mu = mod_mu_layer(model_rnn)[0, -1]
-            mod_sigma = mod_sigma_layer(model_rnn)[0, -1]
-
-            # Shift theta one time step to the left
-            theta_norm = np.roll(theta_norm, -1, axis=0)
-
-            # Sample from the probability distribution function
-            theta = mod_mu + mod_sigma * epsilon[i]
-            theta_norm[-1] = theta_norm_layer(theta[np.newaxis, np.newaxis, :])[0]
-
-            # Calculate the mode mixing factors
-            alpha[i] = alpha_layer(mod_mu[np.newaxis, np.newaxis, :])[0, 0]
-
-        return alpha
+        n_samples = np.shape(alpha)[0]
+        alpha_sampled = np.empty([n_samples, self.config.n_modes], dtype=np.float32)
 
-    def get_n_params_generative_model(self):
-        """Get the number of trainable parameters in the generative model.
+        for i in trange(
+            n_samples - self.config.sequence_length,
+            desc="Predicting mode time course",
+        ):
+            # Extract the sequence
+            alpha_input = alpha[i : i + self.config.sequence_length]
+            alpha_input = alpha_input[np.newaxis, :, :]
 
-        This includes the model RNN weights and biases, mixing coefficients, mode
-        means and covariances.
-
-        Returns
-        -------
-        n_params : int
-            Number of parameters in the generative model.
-        """
-        n_params = 0
+            # Predict the point estimates for theta one time step in the future
+            alpha_sampled[i] = self.generator_model.predict_on_batch(alpha_input)[0, 0]
 
-        for var in self.trainable_weights:
-            var_name = var.name
-            if (
-                "mod_" in var_name
-                or "alpha" in var_name
-                or "means" in var_name
-                or "covs" in var_name
-            ):
-                n_params += np.prod(var.shape)
+        return alpha_sampled
 
-        return int(n_params)
 
+def _build_inference_model(config):
+    # Inference RNN:
+    #   alpha_t = zeta(theta^m_t) where
+    #   mu^{m,theta}_t = f(BLSTM(Y,omega^m_e),lambda_e^m)
+    #   mu^{c,theta}_t = f(BLSTM(Y,omega^c_e),lambda_e^c)
 
-def _model_structure(config):
-    # Layer for input
+    # Definition of layers
     inputs = layers.Input(
         shape=(config.sequence_length, config.n_channels), name="data"
     )
-
-    # Inference RNN:
-    # - Learns q(theta) ~ N(theta | inf_mu, inf_sigma), where
-    #     - inf_mu    ~ affine(RNN(inputs_<=t))
-    #     - inf_sigma ~ softplus(RNN(inputs_<=t))
-
-    # Definition of layers
-    data_drop_layer = layers.Dropout(config.inference_dropout, name="data_drop")
+    data_drop_layer = layers.TimeDistributed(
+        layers.Dropout(config.inference_dropout, name="inf_data_drop")
+    )
     inf_rnn_layer = InferenceRNNLayer(
         config.inference_rnn,
         config.inference_normalization,
         config.inference_activation,
         config.inference_n_layers,
         config.inference_n_units,
         config.inference_dropout,
         config.inference_regularizer,
         name="inf_rnn",
     )
-    inf_mu_layer = layers.Dense(config.n_modes, name="inf_mu")
-    inf_sigma_layer = layers.Dense(
-        config.n_modes, activation="softplus", name="inf_sigma"
-    )
-    theta_layer = SampleNormalDistributionLayer(config.theta_std_epsilon, name="theta")
-    theta_norm_layer = NormalizationLayer(config.theta_normalization, name="theta_norm")
-    alpha_layer = SoftmaxLayer(
-        config.initial_alpha_temperature,
-        config.learn_alpha_temperature,
-        name="alpha",
+
+    alpha_layer = layers.TimeDistributed(
+        layers.Dense(config.n_modes, activation="softmax"), name="inf_alpha"
     )
 
     # Data flow
     data_drop = data_drop_layer(inputs)
-    inf_rnn = inf_rnn_layer(data_drop)
-    inf_mu = inf_mu_layer(inf_rnn)
-    inf_sigma = inf_sigma_layer(inf_rnn)
-    theta = theta_layer([inf_mu, inf_sigma])
-    theta_norm = theta_norm_layer(theta)
-    alpha = alpha_layer(theta_norm)
+    theta = inf_rnn_layer(data_drop)
+    alpha = alpha_layer(theta)
 
     # Observation model:
     # - We use a multivariate normal with a mean vector and covariance matrix for
     #   each mode as the observation model.
     # - We calculate the likelihood of generating the training data with alpha
     #   and the observation model.
 
     # Definition of layers
     means_layer = VectorsLayer(
         config.n_modes,
         config.n_channels,
         config.learn_means,
         config.initial_means,
-        config.means_regularizer,
         name="means",
     )
-    if config.diagonal_covariances:
-        covs_layer = DiagonalMatricesLayer(
-            config.n_modes,
-            config.n_channels,
-            config.learn_covariances,
-            config.initial_covariances,
-            config.covariances_epsilon,
-            config.covariances_regularizer,
-            name="covs",
-        )
-    else:
-        covs_layer = CovarianceMatricesLayer(
-            config.n_modes,
-            config.n_channels,
-            config.learn_covariances,
-            config.initial_covariances,
-            config.covariances_epsilon,
-            config.covariances_regularizer,
-            name="covs",
-        )
+    covs_layer = CovarianceMatricesLayer(
+        config.n_modes,
+        config.n_channels,
+        config.learn_covariances,
+        config.initial_covariances,
+        config.covariances_epsilon,
+        name="covs",
+    )
     mix_means_layer = MixVectorsLayer(name="mix_means")
     mix_covs_layer = MixMatricesLayer(name="mix_covs")
-    ll_loss_layer = LogLikelihoodLossLayer(config.covariances_epsilon, name="ll_loss")
+    concat_means_covs_layer = ConcatVectorsMatricesLayer(name="concat_means_covs")
 
     # Data flow
     mu = means_layer(inputs)  # inputs not used
     D = covs_layer(inputs)  # inputs not used
     m = mix_means_layer([alpha, mu])
     C = mix_covs_layer([alpha, D])
-    ll_loss = ll_loss_layer([inputs, m, C])
+    C_m = concat_means_covs_layer([m, C])
 
+    return models.Model(inputs, [C_m, alpha], name="inference")
+
+
+def _build_generator_model(config):
     # Model RNN:
-    # - Learns p(theta_t |theta_<t) ~ N(theta_t | mod_mu, mod_sigma), where
-    #     - mod_mu    ~ affine(RNN(theta_<t))
-    #     - mod_sigma ~ softplus(RNN(theta_<t))
+    #   alpha_{t} = zeta(theta^m_t}) where
+    #   hat{mu}^{m,theta}_t = f(LSTM(theta^m_<t,omega^m_g), lambda_g^m)
+    #   hat{mu}^{c,theta}_t = f(LSTM(theta^c_<t,omega^c_g), lambda_g^c)
 
     # Definition of layers
-    theta_norm_drop_layer = layers.Dropout(config.model_dropout, name="theta_norm_drop")
+    inputs = layers.Input(
+        shape=(config.sequence_length, config.n_modes),
+        name="gen_inp",
+    )
+    drop_layer = layers.TimeDistributed(
+        layers.Dropout(config.model_dropout, name="gen_data_drop")
+    )
     mod_rnn_layer = ModelRNNLayer(
         config.model_rnn,
         config.model_normalization,
         config.model_activation,
         config.model_n_layers,
         config.model_n_units,
         config.model_dropout,
         config.model_regularizer,
-        name="mod_rnn",
+        name="gen_rnn",
     )
-    mod_mu_layer = layers.Dense(config.n_modes, name="mod_mu")
-    mod_sigma_layer = layers.Dense(
-        config.n_modes, activation="softplus", name="mod_sigma"
+    prior_layer = layers.TimeDistributed(
+        layers.Dense(config.n_modes, activation="softmax"), name="gen_softmax_alpha"
     )
-    kl_div_layer = KLDivergenceLayer(config.theta_std_epsilon, name="kl_div")
-    kl_loss_layer = KLLossLayer(config.do_kl_annealing, name="kl_loss")
 
     # Data flow
-    theta_norm_drop = theta_norm_drop_layer(theta_norm)
-    mod_rnn = mod_rnn_layer(theta_norm_drop)
-    mod_mu = mod_mu_layer(mod_rnn)
-    mod_sigma = mod_sigma_layer(mod_rnn)
-    kl_div = kl_div_layer([inf_mu, inf_sigma, mod_mu, mod_sigma])
-    kl_loss = kl_loss_layer(kl_div)
+    theta_drop = drop_layer(inputs)
+    mod_rnn = mod_rnn_layer(theta_drop)
+    prior = prior_layer(mod_rnn)
+
+    return models.Model(inputs, prior, name="generator")
+
 
-    return tf.keras.Model(
-        inputs=inputs, outputs=[ll_loss, kl_loss, theta_norm], name="DyNeMo"
+def _build_discriminator_model(config):
+    # Descriminator RNN:
+    #   D_theta^m_t = sigma(f(BLSTM([zeta(hat{mu}^{m,theta}_t), zeta(mu^{m,theta}_t)],omega^m_d), \lambda_d^m))
+    #   D_theta^c_t = sigma(f(BLSTM([zeta(hat{mu}^{c,theta}_t), zeta(mu^{c,theta}_t)],omega^c_d), \lambda_d^c))
+
+    # Definition of layers
+    inputs = layers.Input(shape=(config.sequence_length, config.n_modes), name="data")
+    drop_layer = layers.TimeDistributed(
+        layers.Dropout(config.model_dropout, name="dis_data_drop")
+    )
+    dis_rnn_layer = ModelRNNLayer(
+        config.discriminator_rnn,
+        config.discriminator_normalization,
+        config.discriminator_activation,
+        config.discriminator_n_layers,
+        config.discriminator_n_units,
+        config.discriminator_dropout,
+        config.discriminator_regularizer,
+        name="dis_rnn",
+    )
+    sigmoid_layer = layers.TimeDistributed(
+        layers.Dense(1, activation="sigmoid"), name="dis_sigmoid"
     )
+
+    # Data flow
+    theta_norm_drop = drop_layer(inputs)
+    dis_rnn = dis_rnn_layer(theta_norm_drop)
+    output = sigmoid_layer(dis_rnn)
+
+    return models.Model(inputs, output, name="discriminator")
```

### Comparing `osl-dynamics-1.2.4/osl_dynamics/models/hmm.py` & `osl-dynamics-1.2.5/osl_dynamics/models/hmm.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Hidden Markov Model (HMM).
 
 """
 
 import logging
+import os
 import os.path as op
 import sys
 import warnings
 from dataclasses import dataclass
 from pathlib import Path
 
 import numba
@@ -22,17 +23,18 @@
 from osl_dynamics.inference import initializers
 from osl_dynamics.inference.layers import (
     CategoricalLogLikelihoodLossLayer,
     CovarianceMatricesLayer,
     DiagonalMatricesLayer,
     VectorsLayer,
 )
-from osl_dynamics.models import dynemo_obs
+from osl_dynamics.models import obs_mod
 from osl_dynamics.models.mod_base import BaseModelConfig, ModelBase
 from osl_dynamics.simulation import HMM
+from osl_dynamics.utils.misc import set_logging_level
 
 _logger = logging.getLogger("osl-dynamics")
 
 warnings.filterwarnings("ignore", category=NumbaWarning)
 
 EPS = sys.float_info.epsilon
 
@@ -149,29 +151,33 @@
         """Builds a keras model."""
         self.model = _model_structure(self.config)
 
         self.rho = 1
         self.set_trans_prob(self.config.initial_trans_prob)
         self.set_state_probs_t0(self.config.state_probs_t0)
 
-    def fit(self, dataset, epochs=None, use_tqdm=False, **kwargs):
+    def fit(self, dataset, epochs=None, use_tqdm=False, verbose=1, **kwargs):
         """Fit model to a dataset.
 
         Iterates between:
 
         - Baum-Welch updates of latent variable time courses and transition
           probability matrix.
         - TensorFlow updates of observation model parameters.
 
         Parameters
         ----------
         dataset : tensorflow.data.Dataset or osl_dynamics.data.Data
             Training dataset.
         epochs : int
             Number of epochs.
+        use_tqdm : bool
+            Should we use tqdm to display a progress bar?
+        verbose : int
+            Verbosity level. 0 = silent.
         kwargs : keyword arguments
             Keyword arguments for the TensorFlow observation model training.
             These keywords arguments will be passed to self.model.fit().
 
         Returns
         -------
         history : dict
@@ -189,15 +195,15 @@
         # Loop through epochs
         if use_tqdm:
             _range = trange(epochs)
         else:
             _range = range(epochs)
         for n in _range:
             # Setup a progress bar for this epoch
-            if not use_tqdm:
+            if verbose > 0 and not use_tqdm:
                 print("Epoch {}/{}".format(n + 1, epochs))
                 pb_i = utils.Progbar(len(dataset))
 
             # Update rho
             self._update_rho(n)
 
             # Set learning rate for the observation model
@@ -229,19 +235,20 @@
                 # Get new loss
                 l = h.history["loss"][0]
                 if np.isnan(l):
                     _logger.error("Training failed!")
                     return
                 loss.append(l)
 
-                # Update progress bar
-                if use_tqdm:
-                    _range.set_postfix(rho=self.rho, lr=lr, loss=l)
-                else:
-                    pb_i.add(1, values=[("rho", self.rho), ("lr", lr), ("loss", l)])
+                if verbose > 0:
+                    # Update progress bar
+                    if use_tqdm:
+                        _range.set_postfix(rho=self.rho, lr=lr, loss=l)
+                    else:
+                        pb_i.add(1, values=[("rho", self.rho), ("lr", lr), ("loss", l)])
 
             history["loss"].append(np.mean(loss))
             history["rho"].append(self.rho)
             history["lr"].append(lr)
 
         if use_tqdm:
             _range.close()
@@ -800,65 +807,98 @@
         Returns
         -------
         trans_prob : np.ndarray
             Transition probability matrix. Shape is (n_states, n_states).
         """
         return self.trans_prob
 
+    def get_means(self):
+        """Get the state means.
+
+        Returns
+        -------
+        means : np.ndarray
+            State means. Shape is (n_states, n_channels).
+        """
+        return obs_mod.get_observation_model_parameter(self.model, "means")
+
     def get_covariances(self):
-        """Get the covariances of each state.
+        """Get the state covariances.
 
         Returns
         -------
         covariances : np.ndarray
             State covariances. Shape is (n_states, n_channels, n_channels).
         """
-        return dynemo_obs.get_covariances(self.model)
+        return obs_mod.get_observation_model_parameter(self.model, "covs")
 
     def get_means_covariances(self):
-        """Get the means and covariances of each state.
+        """Get the state means and covariances.
+        This is a wrapper for get_means and get_covariances.
 
         Returns
         -------
         means : np.ndarary
             State means.
         covariances : np.ndarray
             State covariances.
         """
-        return dynemo_obs.get_means_covariances(self.model)
+        return self.get_means(), self.get_covariances()
+
+    def get_observation_model_parameters(self):
+        """Wrapper for get_means_covariances."""
+        return self.get_means_covariances()
 
     def set_means(self, means, update_initializer=True):
-        """Set the means of each state.
+        """Set the state means.
 
         Parameters
         ----------
         means : np.ndarray
-            State covariances.
+            State means. Shape is (n_states, n_channels).
         update_initializer : bool
             Do we want to use the passed means when we re-initialize
             the model?
         """
-        dynemo_obs.set_means(self.model, means, update_initializer)
+        obs_mod.set_observation_model_parameter(
+            self.model, means, layer_name="means", update_initializer=update_initializer
+        )
 
     def set_covariances(self, covariances, update_initializer=True):
-        """Set the covariances of each state.
+        """Set the state covariances.
 
         Parameters
         ----------
         covariances : np.ndarray
-            State covariances.
+            State covariances. Shape is (n_states, n_channels, n_channels).
         update_initializer : bool
             Do we want to use the passed covariances when we re-initialize
             the model?
         """
-        dynemo_obs.set_covariances(
+        obs_mod.set_observation_model_parameter(
             self.model,
             covariances,
-            self.config.diagonal_covariances,
-            update_initializer,
+            layer_name="covs",
+            update_initializer=update_initializer,
+            diagonal_covariances=self.config.diagonal_covariances,
+        )
+
+    def set_means_covariances(self, means, covariances, update_initializer=True):
+        """This is a wrapper for set_means and set_covariances."""
+        self.set_means(means, update_initializer=update_initializer)
+        self.set_covariances(covariances, update_initializer=update_initializer)
+
+    def set_observation_model_parameters(
+        self, observation_model_parameters, update_initializer=True
+    ):
+        """Wrapper for set_means_covariances."""
+        self.set_means_covariances(
+            observation_model_parameters[0],
+            observation_model_parameters[1],
+            update_initializer=update_initializer,
         )
 
     def set_trans_prob(self, trans_prob):
         """Sets the transition probability matrix.
 
         Parameters
         ----------
@@ -955,18 +995,18 @@
         ----------
         training_dataset : tensorflow.data.Dataset or osl_dynamics.data.Data
             Training dataset.
         """
         training_dataset = self.make_dataset(training_dataset, concatenate=True)
 
         if self.config.learn_means:
-            dynemo_obs.set_means_regularizer(self.model, training_dataset)
+            obs_mod.set_means_regularizer(self.model, training_dataset)
 
         if self.config.learn_covariances:
-            dynemo_obs.set_covariances_regularizer(
+            obs_mod.set_covariances_regularizer(
                 self.model,
                 training_dataset,
                 self.config.covariances_epsilon,
                 self.config.diagonal_covariances,
             )
 
     def free_energy(self, dataset):
@@ -1156,14 +1196,170 @@
             2 * loss
             + (np.log(self.config.sequence_length) + np.log(n_sequences))
             * n_params
             / n_sequences
         )
         return bic
 
+    def subject_fine_tuning(
+        self, training_data, n_epochs=None, learning_rate=None, store_dir="tmp"
+    ):
+        """Fine tuning the model for each subject.
+
+        Here, we estimate the posterior distribution (state probabilities)
+        and observation model using the data from a single subject with the
+        group-level transition probability matrix held fixed.
+
+        Parameters
+        ----------
+        training_data : osl_dynamics.data.Data
+            Training dataset.
+        n_epochs : int
+            Number of epochs to train for. Defaults to the value in the config
+            used to create the model.
+        learning_rate : float
+            Learning rate. Defaults to the value in the config used to create
+            the model.
+        store_dir : str
+            Directory to temporarily store the model in.
+
+        Returns
+        -------
+        alpha : list of np.ndarray
+            Subject specific mixing coefficients.
+            Each element has shape (n_samples, n_modes).
+        means : np.ndarray
+            Subject specific means. Shape is (n_subjects, n_modes, n_channels).
+        covariances : np.ndarray
+            Subject specific covariances.
+            Shape is (n_subjects, n_modes, n_channels, n_channels).
+        """
+        # Save group-level model parameters
+        os.makedirs(store_dir, exist_ok=True)
+        self.save_weights(f"{store_dir}/weights.h5")
+
+        # Temporarily change hyperparameters
+        original_n_epochs = self.config.n_epochs
+        original_learning_rate = self.config.learning_rate
+        original_learn_trans_prob = self.config.learn_trans_prob
+        self.config.n_epochs = n_epochs or self.config.n_epochs
+        self.config.learning_rate = learning_rate or self.config.learning_rate
+        self.config.learn_trans_prob = False
+
+        # Reset the optimiser
+        self.compile()
+
+        # Fine tune the model for each subject
+        alpha = []
+        means = []
+        covariances = []
+        with set_logging_level(_logger, logging.WARNING):
+            for subject in trange(training_data.n_arrays, desc="Subject fine tuning"):
+                # Train on this subject
+                with training_data.set_keep(subject):
+                    self.fit(training_data, verbose=0)
+                    a = self.get_alpha(training_data, concatenate=True)
+
+                # Get the inferred parameters
+                m, c = self.get_means_covariances()
+                alpha.append(a)
+                means.append(m)
+                covariances.append(c)
+
+                # Reset back to group-level model parameters
+                self.load_weights(f"{store_dir}/weights.h5")
+                self.compile()
+
+        # Reset hyperparameters
+        self.config.n_epochs = original_n_epochs
+        self.config.learning_rate = original_learning_rate
+        self.config.learn_trans_prob = original_learn_trans_prob
+
+        return alpha, np.array(means), np.array(covariances)
+
+    def dual_estimation(
+        self, training_data, n_epochs=None, learning_rate=None, store_dir="tmp"
+    ):
+        """Dual estimation to get subject-specific observation model parameters.
+
+        Here, we estimate the state means and covariances for individual subjects
+        with the rest of the model held fixed at the best parameters (posterior
+        distribution and transition probability) estimated at the group-level.
+
+        Parameters
+        ----------
+        training_data : osl_dynamics.data.Data
+            Training data.
+        n_epochs : int
+            Number of epochs to train for. Defaults to the value in the config
+            used to create the model.
+        learning_rate : float
+            Learning rate. Defaults to the value in the config used to create
+            the model.
+        store_dir : str
+            Directory to temporarily store the model in.
+
+        Returns
+        -------
+        means : np.ndarray
+            Subject specific means. Shape is (n_subjects, n_states, n_channels).
+        covariances : np.ndarray
+            Subject specific covariances.
+            Shape is (n_subjects, n_states, n_channels, n_channels).
+        """
+        # Save group-level model parameters
+        os.makedirs(store_dir, exist_ok=True)
+        self.save_weights(f"{store_dir}/weights.h5")
+
+        # Temporarily change hyperparameters
+        original_n_epochs = self.config.n_epochs
+        original_learning_rate = self.config.learning_rate
+        self.config.n_epochs = n_epochs or self.config.n_epochs
+        self.config.learning_rate = learning_rate or self.config.learning_rate
+
+        # Reset the optimiser
+        self.compile()
+
+        # Create a TensorFlow Dataset
+        dataset = self.make_dataset(training_data, shuffle=True, concatenate=False)
+
+        # Perform dual estimation
+        means = []
+        covariances = []
+        for subject in trange(training_data.n_arrays, desc="Dual estimation"):
+            # Train on this subject's data
+            ds = dataset[subject]
+            for _ in range(self.config.n_epochs):
+                # Loop over batches
+                for data in ds:
+                    x = data["data"]
+
+                    # Get the inferred alpha for each subject
+                    gamma, _ = self._get_state_probs(x)
+                    gamma = gamma.reshape(x.shape[0], x.shape[1], -1)
+                    x_and_gamma = np.concatenate([x, gamma], axis=2)
+
+                    # Train observation model
+                    self.model.fit(x_and_gamma, epochs=1, verbose=0)
+
+            # Get the means and covariances estimated for this subject
+            m, c = self.get_means_covariances()
+            means.append(m)
+            covariances.append(c)
+
+            # Reset back to group-level model parameters
+            self.load_weights(f"{store_dir}/weights.h5")
+            self.compile()
+
+        # Reset hyperparameters
+        self.config.n_epochs = original_n_epochs
+        self.config.learning_rate = original_learning_rate
+
+        return np.array(means), np.array(covariances)
+
     def get_training_time_series(self, training_data, prepared=True, concatenate=False):
         """Get the time series used for training from a Data object.
 
         Parameters
         ----------
         training_data : osl_dynamics.data.Data
             Data object.
@@ -1276,8 +1472,8 @@
     )
 
     # Data flow
     mu = means_layer(data)  # data not used
     D = covs_layer(data)  # data not used
     ll_loss = ll_loss_layer([data, mu, D, gamma, None])
 
-    return tf.keras.Model(inputs=inputs, outputs=[ll_loss], name="HMM-Obs")
+    return tf.keras.Model(inputs=inputs, outputs=[ll_loss], name="HMM")
```

### Comparing `osl-dynamics-1.2.4/osl_dynamics/models/inf_mod_base.py` & `osl-dynamics-1.2.5/osl_dynamics/models/inf_mod_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -348,24 +348,26 @@
         """Wrapper for the standard keras predict method.
 
         Returns
         -------
         predictions : dict
             Dictionary with labels for each prediction.
         """
-        predictions = self.model.predict(*args, *kwargs)
+        predictions = self.model.predict(*args, **kwargs)
         if not self.config.multiple_dynamics:
             return_names = ["ll_loss", "kl_loss", "theta"]
         else:
             return_names = ["ll_loss", "kl_loss", "mean_theta", "fc_theta"]
         predictions_dict = dict(zip(return_names, predictions))
 
         return predictions_dict
 
-    def get_theta(self, dataset, concatenate=False, remove_edge_effects=False):
+    def get_theta(
+        self, dataset, concatenate=False, remove_edge_effects=False, **kwargs
+    ):
         """Mode mixing logits, theta.
 
         Parameters
         ----------
         dataset : tensorflow.data.Dataset or osl_dynamics.data.Data
             Prediction dataset. This can be a list of datasets, one for each subject.
         concatenate : bool
@@ -394,15 +396,15 @@
             step_size = None
 
         dataset = self.make_dataset(dataset, step_size=step_size)
 
         _logger.info("Getting theta")
         theta = []
         for ds in dataset:
-            predictions = self.predict(ds)
+            predictions = self.predict(ds, **kwargs)
             theta_ = predictions["theta"]
             if remove_edge_effects:
                 trim = step_size // 2  # throw away 25%
                 theta_ = (
                     [theta_[0, :-trim]]
                     + list(theta_[1:-1, trim:-trim])
                     + [theta_[-1, trim:]]
@@ -410,15 +412,17 @@
             theta.append(np.concatenate(theta_))
 
         if concatenate or len(theta) == 1:
             theta = np.concatenate(theta)
 
         return theta
 
-    def get_mode_logits(self, dataset, concatenate=False, remove_edge_effects=False):
+    def get_mode_logits(
+        self, dataset, concatenate=False, remove_edge_effects=False, **kwargs
+    ):
         """Get logits (theta) for a multi-time-scale model.
 
         Parameters
         ----------
         dataset : tensorflow.data.Dataset or osl_dynamics.data.Data
             Prediction dataset. This can be a list of datasets, one for each subject.
         concatenate : bool
@@ -448,15 +452,15 @@
 
         dataset = self.make_dataset(dataset, step_size=step_size)
 
         _logger.info("Getting mode logits")
         mean_theta = []
         fc_theta = []
         for ds in dataset:
-            predictions = self.predict(ds)
+            predictions = self.predict(ds, **kwargs)
             mean_theta_ = predictions["mean_theta"]
             fc_theta_ = predictions["fc_theta"]
             if remove_edge_effects:
                 trim = step_size // 2  # throw away 25%
                 mean_theta_ = (
                     [mean_theta_[0, :-trim]]
                     + list(mean_theta_[1:-1, trim:-trim])
@@ -472,15 +476,17 @@
 
         if concatenate or len(mean_theta) == 1:
             mean_theta = np.concatenate(mean_theta)
             fc_theta = np.concatenate(fc_theta)
 
         return mean_theta, fc_theta
 
-    def get_alpha(self, dataset, concatenate=False, remove_edge_effects=False):
+    def get_alpha(
+        self, dataset, concatenate=False, remove_edge_effects=False, **kwargs
+    ):
         """Get mode mixing coefficients, alpha.
 
         Parameters
         ----------
         dataset : tensorflow.data.Dataset or osl_dynamics.data.Data
             Prediction dataset. This can be a list of datasets, one for each subject.
         concatenate : bool
@@ -507,15 +513,15 @@
 
         dataset = self.make_dataset(dataset, step_size=step_size)
         alpha_layer = self.model.get_layer("alpha")
 
         _logger.info("Getting alpha")
         alpha = []
         for ds in dataset:
-            predictions = self.predict(ds)
+            predictions = self.predict(ds, **kwargs)
             theta = predictions["theta"]
             alpha_ = alpha_layer(theta)
             if remove_edge_effects:
                 trim = step_size // 2  # throw away 25%
                 alpha_ = (
                     [alpha_[0, :-trim]]
                     + list(alpha_[1:-1, trim:-trim])
@@ -525,15 +531,15 @@
 
         if concatenate or len(alpha) == 1:
             alpha = np.concatenate(alpha)
 
         return alpha
 
     def get_mode_time_courses(
-        self, dataset, concatenate=False, remove_edge_effects=False
+        self, dataset, concatenate=False, remove_edge_effects=False, **kwargs
     ):
         """Get mode time courses (alpha) for a multi-time-scale model.
 
         Parameters
         ----------
         dataset : tensorflow.data.Dataset or osl_dynamics.data.Data
             Prediction data. This can be a list of datasets, one for each subject.
@@ -567,15 +573,15 @@
         alpha_layer = self.model.get_layer("alpha")
         gamma_layer = self.model.get_layer("gamma")
 
         _logger.info("Getting mode time courses")
         alpha = []
         gamma = []
         for ds in dataset:
-            predictions = self.predict(ds)
+            predictions = self.predict(ds, **kwargs)
             mean_theta = predictions["mean_theta"]
             fc_theta = predictions["fc_theta"]
             alpha_ = alpha_layer(mean_theta)
             gamma_ = gamma_layer(fc_theta)
             if remove_edge_effects:
                 trim = step_size // 2  # throw away 25%
                 alpha_ = (
@@ -593,15 +599,15 @@
 
         if concatenate or len(alpha) == 1:
             alpha = np.concatenate(alpha)
             gamma = np.concatenate(gamma)
 
         return alpha, gamma
 
-    def losses(self, dataset):
+    def losses(self, dataset, **kwargs):
         """Calculates the log-likelihood and KL loss for a dataset.
 
         Parameters
         ----------
         dataset : tensorflow.data.Dataset or osl_dynamics.data.Data
             Dataset to calculate losses for.
 
@@ -610,20 +616,20 @@
         ll_loss : float
             Negative log-likelihood loss.
         kl_loss : float
             KL divergence loss.
         """
         dataset = self.make_dataset(dataset, concatenate=True)
         _logger.info("Getting losses")
-        predictions = self.predict(dataset)
+        predictions = self.predict(dataset, **kwargs)
         ll_loss = np.mean(predictions["ll_loss"])
         kl_loss = np.mean(predictions["kl_loss"])
         return ll_loss, kl_loss
 
-    def free_energy(self, dataset):
+    def free_energy(self, dataset, **kwargs):
         """Calculates the variational free energy of a dataset.
 
         Note, this method returns a free energy which may have a significantly
         smaller KL loss. This is because during training we sample from the
         posterior, however, when we're evaluating the model, we take the maximum
         a posteriori estimate (posterior mean). This has the effect of giving a
         lower KL loss for a given dataset.
@@ -635,15 +641,15 @@
 
         Returns
         -------
         free_energy : float
             Variational free energy for the dataset.
         """
         dataset = self.make_dataset(dataset, concatenate=True)
-        ll_loss, kl_loss = self.losses(dataset)
+        ll_loss, kl_loss = self.losses(dataset, **kwargs)
         free_energy = ll_loss + kl_loss
         return free_energy
 
     def bayesian_information_criterion(self, dataset):
         """Calculate the Bayesian Information Criterion (BIC) of the model
         for a given dataset.
```

### Comparing `osl-dynamics-1.2.4/osl_dynamics/models/mage.py` & `osl-dynamics-1.2.5/osl_dynamics/models/mage.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     InferenceRNNLayer,
     MatMulLayer,
     MixMatricesLayer,
     MixVectorsLayer,
     ModelRNNLayer,
     VectorsLayer,
 )
-from osl_dynamics.models import mdynemo_obs
+from osl_dynamics.models import obs_mod
 from osl_dynamics.models.mod_base import BaseModelConfig, ModelBase
 
 _logger = logging.getLogger("osl-dynamics")
 
 
 @dataclass
 class Config(BaseModelConfig):
@@ -498,46 +498,133 @@
             ]
             gamma_sampled[i] = self.generator_model_cov.predict_on_batch(gamma_input)[
                 0, 0
             ]
 
         return alpha_sampled, gamma_sampled
 
+    def get_means(self):
+        """Get the mode means.
+
+        Returns
+        -------
+        means : np.ndarray
+            Mode means. Shape (n_modes, n_channels).
+        """
+        return obs_mod.get_observation_model_parameter(self.inference_model, "means")
+
+    def get_stds(self):
+        """Get the mode standard deviations.
+
+        Returns
+        -------
+        stds : np.ndarray
+            Mode standard deviations. Shape (n_modes, n_channels, n_channels).
+        """
+        return obs_mod.get_observation_model_parameter(self.inference_model, "stds")
+
+    def get_fcs(self):
+        """Get the mode functional connectivities.
+
+        Returns
+        -------
+        fcs : np.ndarray
+            Mode functional connectivities. Shape (n_modes, n_channels, n_channels).
+        """
+        return obs_mod.get_observation_model_parameter(self.inference_model, "fcs")
+
     def get_means_stds_fcs(self):
-        """Get the mean, standard devation and functional connectivity of each mode.
+        """Get the mode means, standard deviations, functional connectivities.
+        This is a wrapper for get_means, get_stds, get_fcs.
 
         Returns
         -------
         means : np.ndarray
-            Mode means.
+            Mode means. Shape is (n_modes, n_channels).
         stds : np.ndarray
-            Mode standard deviations.
+            Mode standard deviations. Shape is (n_modes, n_channels, n_channels).
         fcs : np.ndarray
-            Mode functional connectivities.
+            Mode functional connectivities. Shape is (n_modes, n_channels, n_channels).
         """
-        return mdynemo_obs.get_means_stds_fcs(self.inference_model)
+        return self.get_means(), self.get_stds(), self.get_fcs()
 
-    def set_means_stds_fcs(self, means, stds, fcs, update_initializer=True):
-        """Set the means, standard deviations, functional connectivities of each mode.
+    def get_observation_model_parameters(self):
+        """Wrapper for get_means_stds_fcs."""
+        return self.get_means_stds_fcs()
+
+    def set_means(self, means, update_initializer=True):
+        """Set the mode means.
+
+        Parameters
+        ----------
+        means : np.ndarray
+            Mode means. Shape is (n_modes, n_channels).
+        update_initializer : bool
+            Do we want to use the passed parameters when we re_initialize
+            the model?
+        """
+        obs_mod.set_observation_model_parameter(
+            self.inference_model,
+            means,
+            layer_name="means",
+            update_initializer=update_initializer,
+        )
+
+    def set_stds(self, stds, update_initializer=True):
+        """Set the mode standard deviations.
 
         Parameters
         ----------
-        means: np.ndarray
-            Mode means with shape (n_modes, n_channels).
-        stds: np.ndarray
-            Mode standard deviations with shape (n_modes, n_channels) or
-            (n_modes, n_channels, n_channels).
-        fcs: np.ndarray
-            Mode functional connectivities with shape (n_modes, n_channels, n_channels).
-        update_initializer: bool
+        stds : np.ndarray
+            Mode standard deviations.
+            Shape is (n_modes, n_channels, n_channels) or (n_modes, n_channels).
+        update_initializer : bool
             Do we want to use the passed parameters when we re_initialize
             the model?
         """
-        mdynemo_obs.set_means_stds_fcs(
-            self.inference_model, means, stds, fcs, update_initializer
+        obs_mod.set_observation_model_parameter(
+            self.inference_model,
+            stds,
+            layer_name="stds",
+            update_initializer=update_initializer,
+        )
+
+    def set_fcs(self, fcs, update_initializer=True):
+        """Set the mode functional connectivities.
+
+        Parameters
+        ----------
+        fcs : np.ndarray
+            Mode functional connectivities. Shape is (n_modes, n_channels, n_channels).
+        update_initializer : bool
+            Do we want to use the passed parameters when we re_initialize
+            the model?
+        """
+        obs_mod.set_observation_model_parameter(
+            self.inference_model,
+            fcs,
+            layer_name="fcs",
+            update_initializer=update_initializer,
+        )
+
+    def set_means_stds_fcs(self, means, stds, fcs, update_initializer=True):
+        """This is a wrapper for set_means, set_stds, set_fcs."""
+        self.set_means(means, update_initializer=update_initializer)
+        self.set_stds(stds, update_initializer=update_initializer)
+        self.set_fcs(fcs, update_initializer=update_initializer)
+
+    def set_observation_model_parameters(
+        self, observation_model_parameters, update_initializer=True
+    ):
+        """Wrapper for set_means_stds_fcs."""
+        self.set_means_stds_fcs(
+            observation_model_parameters[0],
+            observation_model_parameters[1],
+            observation_model_parameters[2],
+            update_initializer=update_initializer,
         )
 
 
 def _build_inference_model(config):
     # Inference RNN:
     #   alpha_t = zeta(theta^m_t}) where
     #   mu^{m,theta}_t = f(BLSTM(Y,omega^m_e),lambda_e^m)
```

### Comparing `osl-dynamics-1.2.4/osl_dynamics/models/mdynemo.py` & `osl-dynamics-1.2.5/osl_dynamics/models/mdynemo.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     MixVectorsLayer,
     ModelRNNLayer,
     NormalizationLayer,
     SampleNormalDistributionLayer,
     SoftmaxLayer,
     VectorsLayer,
 )
-from osl_dynamics.models import dynemo_obs, mdynemo_obs
+from osl_dynamics.models import obs_mod
 from osl_dynamics.models.inf_mod_base import (
     VariationalInferenceModelBase,
     VariationalInferenceModelConfig,
 )
 from osl_dynamics.models.mod_base import BaseModelConfig
 
 _logger = logging.getLogger("osl-dynamics")
@@ -235,49 +235,114 @@
 
     config_type = Config
 
     def build_model(self):
         """Builds a keras model."""
         self.model = _model_structure(self.config)
 
+    def get_means(self):
+        """Get the mode means.
+
+        Returns
+        -------
+        means : np.ndarray
+            Mode means. Shape (n_modes, n_channels).
+        """
+        return obs_mod.get_observation_model_parameter(self.model, "means")
+
+    def get_stds(self):
+        """Get the mode standard deviations.
+
+        Returns
+        -------
+        stds : np.ndarray
+            Mode standard deviations. Shape (n_modes, n_channels, n_channels).
+        """
+        return obs_mod.get_observation_model_parameter(self.model, "stds")
+
+    def get_fcs(self):
+        """Get the mode functional connectivities.
+
+        Returns
+        -------
+        fcs : np.ndarray
+            Mode functional connectivities. Shape (n_modes, n_channels, n_channels).
+        """
+        return obs_mod.get_observation_model_parameter(self.model, "fcs")
+
     def get_means_stds_fcs(self):
-        """Get the mean, standard devation and functional connectivity of each mode.
+        """Get the mode means, standard deviations, functional connectivities.
+        This is a wrapper for get_means, get_stds, get_fcs.
 
         Returns
         -------
         means : np.ndarray
-            Mode means.
+            Mode means. Shape is (n_modes, n_channels).
         stds : np.ndarray
-            Mode standard deviations.
+            Mode standard deviations. Shape is (n_modes, n_channels, n_channels).
         fcs : np.ndarray
-            Mode functional connectivities.
+            Mode functional connectivities. Shape is (n_modes, n_channels, n_channels).
         """
-        return mdynemo_obs.get_means_stds_fcs(self.model)
+        return self.get_means(), self.get_stds(), self.get_fcs()
 
     def get_observation_model_parameters(self):
         """Wrapper for get_means_stds_fcs."""
         return self.get_means_stds_fcs()
 
-    def set_means_stds_fcs(self, means, stds, fcs, update_initializer=True):
-        """Set the means, standard deviations, functional connectivities of each mode.
+    def set_means(self, means, update_initializer=True):
+        """Set the mode means.
 
         Parameters
         ----------
-        means: np.ndarray
-            Mode means with shape (n_modes, n_channels).
-        stds: np.ndarray
-            Mode standard deviations with shape (n_modes, n_channels) or
-            (n_modes, n_channels, n_channels).
-        fcs: np.ndarray
-            Mode functional connectivities with shape (n_fc_modes, n_channels, n_channels).
-        update_initializer: bool
+        means : np.ndarray
+            Mode means. Shape is (n_modes, n_channels).
+        update_initializer : bool
             Do we want to use the passed parameters when we re_initialize
             the model?
         """
-        mdynemo_obs.set_means_stds_fcs(self.model, means, stds, fcs, update_initializer)
+        obs_mod.set_observation_model_parameter(
+            self.model, means, layer_name="means", update_initializer=update_initializer
+        )
+
+    def set_stds(self, stds, update_initializer=True):
+        """Set the mode standard deviations.
+
+        Parameters
+        ----------
+        stds : np.ndarray
+            Mode standard deviations.
+            Shape is (n_modes, n_channels, n_channels) or (n_modes, n_channels).
+        update_initializer : bool
+            Do we want to use the passed parameters when we re_initialize
+            the model?
+        """
+        obs_mod.set_observation_model_parameter(
+            self.model, stds, layer_name="stds", update_initializer=update_initializer
+        )
+
+    def set_fcs(self, fcs, update_initializer=True):
+        """Set the mode functional connectivities.
+
+        Parameters
+        ----------
+        fcs : np.ndarray
+            Mode functional connectivities. Shape is (n_modes, n_channels, n_channels).
+        update_initializer : bool
+            Do we want to use the passed parameters when we re_initialize
+            the model?
+        """
+        obs_mod.set_observation_model_parameter(
+            self.model, fcs, layer_name="fcs", update_initializer=update_initializer
+        )
+
+    def set_means_stds_fcs(self, means, stds, fcs, update_initializer=True):
+        """This is a wrapper for set_means, set_stds, set_fcs."""
+        self.set_means(means, update_initializer=update_initializer)
+        self.set_stds(stds, update_initializer=update_initializer)
+        self.set_fcs(fcs, update_initializer=update_initializer)
 
     def set_observation_model_parameters(
         self, observation_model_parameters, update_initializer=True
     ):
         """Wrapper for set_means_stds_fcs."""
         self.set_means_stds_fcs(
             observation_model_parameters[0],
@@ -298,23 +363,23 @@
         ----------
         training_dataset : tensorflow.data.Dataset or osl_dynamics.data.Data
             Training dataset.
         """
         training_dataset = self.make_dataset(training_dataset, concatenate=True)
 
         if self.config.learn_means:
-            dynemo_obs.set_means_regularizer(self.model, training_dataset)
+            obs_mod.set_means_regularizer(self.model, training_dataset)
 
         if self.config.learn_stds:
-            mdynemo_obs.set_stds_regularizer(
+            obs_mod.set_stds_regularizer(
                 self.model, training_dataset, self.config.stds_epsilon
             )
 
         if self.config.learn_fcs:
-            mdynemo_obs.set_fcs_regularizer(
+            obs_mod.set_fcs_regularizer(
                 self.model, training_dataset, self.config.fcs_epsilon
             )
 
     def sample_time_courses(self, n_samples: int):
         """Uses the model RNN to sample mode mixing factors, alpha and gamma.
 
         Parameters
```

### Comparing `osl-dynamics-1.2.4/osl_dynamics/models/mdynemo_obs.py` & `osl-dynamics-1.2.5/osl_dynamics/models/state_dynemo.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,76 +1,113 @@
-"""Multi-Dynamic Network Modes (M-DyNeMo) observation model.
+"""State-Dynamic Network Modelling (State-DyNeMo).
 
 """
 
 import logging
 from dataclasses import dataclass
+from typing import Literal
 
 import numpy as np
 import tensorflow as tf
 from tensorflow.keras import layers
 
 import osl_dynamics.data.tf as dtf
-from osl_dynamics.inference import regularizers
-from osl_dynamics.inference.initializers import WeightInitializer
 from osl_dynamics.inference.layers import (
-    CorrelationMatricesLayer,
+    CategoricalKLDivergenceLayer,
+    CategoricalLogLikelihoodLossLayer,
+    CovarianceMatricesLayer,
     DiagonalMatricesLayer,
-    LogLikelihoodLossLayer,
-    MatMulLayer,
-    MixMatricesLayer,
-    MixVectorsLayer,
+    InferenceRNNLayer,
+    KLLossLayer,
+    ModelRNNLayer,
+    SampleOneHotCategoricalDistributionLayer,
+    SoftmaxLayer,
     VectorsLayer,
-    add_epsilon,
 )
-from osl_dynamics.models import dynemo_obs
-from osl_dynamics.models.mod_base import BaseModelConfig, ModelBase
+from osl_dynamics.models.dynemo import Model as DyNeMo
+from osl_dynamics.models.inf_mod_base import VariationalInferenceModelConfig
+from osl_dynamics.models.mod_base import BaseModelConfig
+from osl_dynamics.simulation import HMM
 
 _logger = logging.getLogger("osl-dynamics")
 
 
 @dataclass
-class Config(BaseModelConfig):
-    """Settings for M-DyNeMo observation model.
+class Config(BaseModelConfig, VariationalInferenceModelConfig):
+    """Settings for State-DyNeMo.
 
     Parameters
     ----------
     model_name : str
         Model name.
-    n_modes : int
-        Number of modes for both power.
-    n_fc_modes : int
-        Number of modes for FC. If none, set to n_modes.
+    n_states : int
+        Number of states.
     n_channels : int
         Number of channels.
     sequence_length : int
-        Length of sequence passed to the generative model.
+        Length of sequence passed to the inference network and generative model.
+
+    inference_rnn : str
+        RNN to use, either 'gru' or 'lstm'.
+    inference_n_layers : int
+        Number of layers.
+    inference_n_units : int
+        Number of units.
+    inference_normalization : str
+        Type of normalization to use. Either None, 'batch' or 'layer'.
+    inference_activation : str
+        Type of activation to use after normalization and before dropout.
+        E.g. 'relu', 'elu', etc.
+    inference_dropout : float
+        Dropout rate.
+    inference_regularizer : str
+        Regularizer.
+
+    model_rnn : str
+        RNN to use, either 'gru' or 'lstm'.
+    model_n_layers : int
+        Number of layers.
+    model_n_units : int
+        Number of units.
+    model_normalization : str
+        Type of normalization to use. Either None, 'batch' or 'layer'.
+    model_activation : str
+        Type of activation to use after normalization and before dropout.
+        E.g. 'relu', 'elu', etc.
+    model_dropout : float
+        Dropout rate.
+    model_regularizer : str
+        Regularizer.
 
     learn_means : bool
-        Should we make the mean for each mode trainable?
-    learn_stds : bool
-        Should we make the standard deviation for each mode trainable?
-    learn_fcs : bool
-        Should we make the functional connectivity for each mode trainable?
+        Should we make the mean vectors for each mode trainable?
+    learn_covariances : bool
+        Should we make the covariance matrix for each mode trainable?
     initial_means : np.ndarray
-        Initialisation for the mode means.
-    initial_stds : np.ndarray
-        Initialisation for mode standard deviations.
-    initial_fcs : np.ndarray
-        Initialisation for mode functional connectivity matrices.
-    stds_epsilon : float
-        Error added to mode stds for numerical stability.
-    fcs_epsilon : float
-        Error added to mode fcs for numerical stability.
+        Initialisation for mean vectors.
+    initial_covariances : np.ndarray
+        Initialisation for mode covariances.
+    covariances_epsilon : float
+        Error added to standard deviations for numerical stability.
+    diagonal_covariances : bool
+        Should we learn diagonal mode covariances?
     means_regularizer : tf.keras.regularizers.Regularizer
-        Regularizer for the mean vectors.
-    stds_regularizer : tf.keras.regularizers.Regularizer
-        Regularizer for the standard deviation vectors.
-    fcs_regularizer : tf.keras.regularizers.Regularizer
-        Regularizer for the correlation matrices.
+        Regularizer for mean vectors.
+    covariances_regularizer : tf.keras.regularizers.Regularizer
+        Regularizer for covariance matrices.
+
+    do_kl_annealing : bool
+        Should we use KL annealing during training?
+    kl_annealing_curve : str
+        Type of KL annealing curve. Either 'linear' or 'tanh'.
+    kl_annealing_sharpness : float
+        Parameter to control the shape of the annealing curve if
+        kl_annealing_curve='tanh'.
+    n_kl_annealing_epochs : int
+        Number of epochs to perform KL annealing.
 
     batch_size : int
         Mini-batch size.
     learning_rate : float
         Learning rate.
     gradient_clip : float
         Value to clip gradients by. This is the clipnorm argument passed to
@@ -81,271 +118,284 @@
         Optimizer to use. 'adam' is recommended.
     multi_gpu : bool
         Should be use multiple GPUs for training?
     strategy : str
         Strategy for distributed learning.
     """
 
-    model_name: str = "M-DyNeMo-Obs"
+    model_name: str = "State-DyNeMo"
+
+    # Inference network parameters
+    inference_rnn: Literal["gru", "lstm"] = "lstm"
+    inference_n_layers: int = 1
+    inference_n_units: int = None
+    inference_normalization: Literal[None, "batch", "layer"] = None
+    inference_activation: str = None
+    inference_dropout: float = 0.0
+    inference_regularizer: str = None
+
+    # Model network parameters
+    model_rnn: Literal["gru", "lstm"] = "lstm"
+    model_n_layers: int = 1
+    model_n_units: int = None
+    model_normalization: Literal[None, "batch", "layer"] = None
+    model_activation: str = None
+    model_dropout: float = 0.0
+    model_regularizer: str = None
 
     # Observation model parameters
-    n_fc_modes: int = None
     learn_means: bool = None
-    learn_stds: bool = None
-    learn_fcs: bool = None
+    learn_covariances: bool = None
     initial_means: np.ndarray = None
-    initial_stds: np.ndarray = None
-    initial_fcs: np.ndarray = None
-    stds_epsilon: float = None
-    fcs_epsilon: float = None
+    initial_covariances: np.ndarray = None
+    diagonal_covariances: bool = False
+    covariances_epsilon: float = 1e-6
     means_regularizer: tf.keras.regularizers.Regularizer = None
-    stds_regularizer: tf.keras.regularizers.Regularizer = None
-    fcs_regularizer: tf.keras.regularizers.Regularizer = None
-    multiple_dynamics: bool = True
+    covariances_regularizer: tf.keras.regularizers.Regularizer = None
 
     def __post_init__(self):
+        self.validate_rnn_parameters()
         self.validate_observation_model_parameters()
+        self.validate_kl_annealing_parameters()
         self.validate_dimension_parameters()
         self.validate_training_parameters()
 
+    def validate_rnn_parameters(self):
+        if self.inference_n_units is None:
+            raise ValueError("Please pass inference_n_units.")
+
+        if self.model_n_units is None:
+            raise ValueError("Please pass model_n_units.")
+
     def validate_observation_model_parameters(self):
-        if (
-            self.learn_means is None
-            or self.learn_stds is None
-            or self.learn_fcs is None
-        ):
-            raise ValueError("learn_means, learn_stds and learn_fcs must be passed.")
-
-        if self.stds_epsilon is None:
-            if self.learn_stds:
-                self.stds_epsilon = 1e-6
-            else:
-                self.stds_epsilon = 0.0
-
-        if self.fcs_epsilon is None:
-            if self.learn_fcs:
-                self.fcs_epsilon = 1e-6
-            else:
-                self.fcs_epsilon = 0.0
-
-    def validate_dimension_parameters(self):
-        super().validate_dimension_parameters()
-        if self.n_fc_modes is None:
-            self.n_fc_modes = self.n_modes
-            _logger.warning("n_fc_modes is None, set to n_modes.")
+        if self.learn_means is None or self.learn_covariances is None:
+            raise ValueError("learn_means and learn_covariances must be passed.")
 
 
-class Model(ModelBase):
-    """M-DyNeMo observation model class.
+class Model(DyNeMo):
+    """State-DyNeMo model class.
 
     Parameters
     ----------
-    config : osl_dynamics.models.mdynemo_obs.Config
+    config : osl_dynamics.models.state_dynemo.Config
     """
 
     config_type = Config
 
     def build_model(self):
         """Builds a keras model."""
         self.model = _model_structure(self.config)
 
-    def get_means_stds_fcs(self):
-        """Get the mean, standard devation and functional connectivity of each mode.
+    def sample_alpha(self, n_samples):
+        """Uses the model RNN to sample a state time course, alpha."""
+        raise NotImplementedError("This method hasn't been coded yet.")
+
+    def random_state_time_course_initialization(
+        self, training_data, n_epochs, n_init, take=1, **kwargs
+    ):
+        """Random state time course initialization.
 
-        Returns
-        -------
-        means : np.ndarray
-            Mode means.
-        stds : np.ndarray
-            Mode standard deviations.
-        fcs : np.ndarray
-            Mode functional connectivities.
-        """
-        return get_means_stds_fcs(self.model)
-
-    def set_means_stds_fcs(self, means, stds, fcs, update_initializer=True):
-        """Set the means, standard deviations, functional connectivities of each mode.
+        The model is trained for a few epochs with a sampled state time course
+        initialization. The model with the best free energy is kept.
 
         Parameters
         ----------
-        means: np.ndarray
-            Mode means with shape (n_modes, n_channels).
-        stds: np.ndarray
-            Mode standard deviations with shape (n_modes, n_channels) or
-            (n_modes, n_channels, n_channels).
-        fcs: np.ndarray
-            Mode functional connectivities with shape (n_fc_modes, n_channels, n_channels).
-        update_initializer: bool
-            Do we want to use the passed parameters when we re_initialize
-            the model?
+        training_data : tensorflow.data.Dataset or osl_dynamics.data.Data
+            Dataset to use for training.
+        n_epochs : int
+            Number of epochs to train the model.
+        n_init : int
+            Number of initializations.
+        take : float
+            Fraction of total batches to take.
+        kwargs : keyword arguments
+            Keyword arguments for the fit method.
+
+        Returns
+        -------
+        history : history
+            The training history of the best initialization.
         """
-        set_means_stds_fcs(self.model, means, stds, fcs, update_initializer)
+        if n_init is None or n_init == 0:
+            _logger.warning(
+                "Number of initializations was set to zero. "
+                + "Skipping initialization."
+            )
+            return
+
+        _logger.info("Random state time course initialization:")
+
+        # Make a TensorFlow Dataset
+        training_dataset = self.make_dataset(
+            training_data, shuffle=True, concatenate=True
+        )
+
+        # Calculate the number of batches to use
+        n_total_batches = dtf.get_n_batches(training_dataset)
+        n_batches = max(round(n_total_batches * take), 1)
+        _logger.info(f"Using {n_batches} out of {n_total_batches} batches")
+
+        # Pick the initialization with the lowest free energy
+        best_loss = np.Inf
+        for n in range(n_init):
+            _logger.info(f"Initialization {n}")
+            self.reset()
+            self.set_random_state_time_course_initialization(training_data)
+            training_dataset.shuffle(100000)
+            training_data_subset = training_dataset.take(n_batches)
+            history = self.fit(training_data_subset, epochs=n_epochs, **kwargs)
+            loss = history["loss"][-1]
+            if loss < best_loss:
+                best_initialization = n
+                best_loss = loss
+                best_history = history
+                best_weights = self.get_weights()
+
+        if best_loss == np.Inf:
+            _logger.error("Initialization failed")
+            return
+
+        _logger.info(f"Using initialization {best_initialization}")
+        self.reset()
+        self.set_weights(best_weights)
 
-    def set_regularizers(self, training_dataset):
-        """Set the regularizers of means, stds and fcs based on the training data.
+        return best_history
 
-        A multivariate normal prior is applied to the mean vectors with mu=0,
-        sigma=diag((range / 2)**2), a log normal prior is applied to the standard
-        deviations with mu=0, sigma=sqrt(log(2 * (range))) and a marginal inverse
-        Wishart prior is applied to the fcs matrices with nu = n_channels - 1 + 0.1.
+    def set_random_state_time_course_initialization(self, training_data):
+        """Sets the initial means/covariances based on a random state time course.
 
         Parameters
         ----------
-        training_dataset : tensorflow.data.Dataset
-            Training dataset.
+        training_data : osl_dynamics.data.Data
+            Training data object.
         """
-        if self.config.learn_means:
-            dynemo_obs.set_means_regularizer(self.model, training_dataset)
 
-        if self.config.learn_stds:
-            set_stds_regularizer(self.model, training_dataset, self.config.stds_epsilon)
+        # Loop over subjects
+        subject_means = []
+        subject_covariances = []
+        for data in training_data.subjects:
+            # Sample a state time course from an HMM
+            trans_prob = (
+                np.ones((self.config.n_states, self.config.n_states))
+                * 0.1
+                / (self.config.n_states - 1)
+            )
+            np.fill_diagonal(trans_prob, 0.9)
+            stc = HMM(trans_prob).generate_states(data.shape[0])
+
+            # Calculate the mean/covariance for each state for this subject
+            m = []
+            C = []
+            for j in range(self.config.n_states):
+                x = data[stc[:, j] == 1]
+                mu_j = np.mean(x, axis=0)
+                sigma_j = np.cov(x, rowvar=False)
+                m.append(mu_j)
+                C.append(sigma_j)
+
+            subject_means.append(m)
+            subject_covariances.append(C)
+
+        # Average over subjects
+        initial_means = np.mean(subject_means, axis=0)
+        initial_covariances = np.mean(subject_covariances, axis=0)
+
+        if self.config.learn_means:
+            # Set initial means
+            self.set_means(initial_means, update_initializer=True)
 
-        if self.config.learn_fcs:
-            set_fcs_regularizer(self.model, training_dataset, self.config.fcs_epsilon)
+        if self.config.learn_covariances:
+            # Set initial covariances
+            self.set_covariances(initial_covariances, update_initializer=True)
 
 
 def _model_structure(config):
-    # Layers for inputs
+    # Layer for input
     data = layers.Input(shape=(config.sequence_length, config.n_channels), name="data")
-    alpha = layers.Input(shape=(config.sequence_length, config.n_modes), name="alpha")
-    gamma = layers.Input(
-        shape=(config.sequence_length, config.n_fc_modes), name="gamma"
+
+    # Inference RNN:
+    # - q(state_t) = softmax(theta_t), where theta_t is a set of logits
+    inf_rnn_layer = InferenceRNNLayer(
+        config.inference_rnn,
+        config.inference_normalization,
+        config.inference_activation,
+        config.inference_n_layers,
+        config.inference_n_units,
+        config.inference_dropout,
+        config.inference_regularizer,
+        name="inf_rnn",
+    )
+    inf_theta_layer = layers.Dense(config.n_states, name="inf_theta")
+    alpha_layer = SoftmaxLayer(
+        initial_temperature=1.0, learn_temperature=False, name="alpha"
     )
+    states_layer = SampleOneHotCategoricalDistributionLayer(name="states")
 
-    # Observation model:
-    # - We use a multivariate normal with a mean vector and covariance matrix for
-    #   each mode as the observation model.
-    # - We calculate the likelihood of generating the training data with alpha
-    #   and the observation model.
+    inf_rnn = inf_rnn_layer(data)
+    inf_theta = inf_theta_layer(inf_rnn)
+    alpha = alpha_layer(inf_theta)
+    states = states_layer(inf_theta)
 
-    # Layers
+    # Observation model:
+    # - p(x_t) = N(m_t, C_t), where m_t and C_t are state dependent
+    #   means/covariances
     means_layer = VectorsLayer(
-        config.n_modes,
+        config.n_states,
         config.n_channels,
         config.learn_means,
         config.initial_means,
         config.means_regularizer,
         name="means",
     )
-    stds_layer = DiagonalMatricesLayer(
-        config.n_modes,
-        config.n_channels,
-        config.learn_stds,
-        config.initial_stds,
-        config.stds_epsilon,
-        config.stds_regularizer,
-        name="stds",
-    )
-    fcs_layer = CorrelationMatricesLayer(
-        config.n_fc_modes,
-        config.n_channels,
-        config.learn_fcs,
-        config.initial_fcs,
-        config.fcs_epsilon,
-        config.fcs_regularizer,
-        name="fcs",
-    )
-    mix_means_layer = MixVectorsLayer(name="mix_means")
-    mix_stds_layer = MixMatricesLayer(name="mix_stds")
-    mix_fcs_layer = MixMatricesLayer(name="mix_fcs")
-    matmul_layer = MatMulLayer(name="cov")
-    ll_loss_layer = LogLikelihoodLossLayer(
-        np.maximum(config.stds_epsilon, config.fcs_epsilon), name="ll_loss"
+    if config.diagonal_covariances:
+        covs_layer = DiagonalMatricesLayer(
+            config.n_states,
+            config.n_channels,
+            config.learn_covariances,
+            config.initial_covariances,
+            config.covariances_epsilon,
+            config.covariances_regularizer,
+            name="covs",
+        )
+    else:
+        covs_layer = CovarianceMatricesLayer(
+            config.n_states,
+            config.n_channels,
+            config.learn_covariances,
+            config.initial_covariances,
+            config.covariances_epsilon,
+            config.covariances_regularizer,
+            name="covs",
+        )
+    ll_loss_layer = CategoricalLogLikelihoodLossLayer(
+        config.n_states, config.covariances_epsilon, name="ll_loss"
     )
 
-    # Data flow
     mu = means_layer(data)  # data not used
-    E = stds_layer(data)  # data not used
-    D = fcs_layer(data)  # data not used
-
-    m = mix_means_layer([alpha, mu])
-    G = mix_stds_layer([alpha, E])
-    F = mix_fcs_layer([gamma, D])
-    C = matmul_layer([G, F, G])
-
-    ll_loss = ll_loss_layer([data, m, C])
-
-    return tf.keras.Model(
-        inputs=[data, alpha, gamma], outputs=[ll_loss], name="M-DyNeMo-Obs"
-    )
+    D = covs_layer(data)  # data not used
+    ll_loss = ll_loss_layer([data, mu, D, alpha, None])
 
-
-def get_means_stds_fcs(model):
-    means_layer = model.get_layer("means")
-    stds_layer = model.get_layer("stds")
-    fcs_layer = model.get_layer("fcs")
-
-    means = means_layer(1)
-    stds = add_epsilon(
-        stds_layer(1),
-        stds_layer.epsilon,
-        diag=True,
-    )
-    fcs = add_epsilon(
-        fcs_layer(1),
-        fcs_layer.epsilon,
-        diag=True,
-    )
-    return means.numpy(), stds.numpy(), fcs.numpy()
-
-
-def set_means_stds_fcs(model, means, stds, fcs, update_initializer=True):
-    if stds.ndim == 3:
-        # Only keep the diagonal as a vector
-        stds = np.diagonal(stds, axis1=1, axis2=2)
-
-    means = means.astype(np.float32)
-    stds = stds.astype(np.float32)
-    fcs = fcs.astype(np.float32)
-
-    # Get layers
-    means_layer = model.get_layer("means")
-    stds_layer = model.get_layer("stds")
-    fcs_layer = model.get_layer("fcs")
-
-    # Transform the matrices to layer weights
-    diagonals = stds_layer.bijector.inverse(stds)
-    flattened_cholesky_factors = fcs_layer.bijector.inverse(fcs)
-
-    # Set values
-    means_layer.vectors_layer.tensor.assign(means)
-    stds_layer.diagonals_layer.tensor.assign(diagonals)
-    fcs_layer.flattened_cholesky_factors_layer.tensor.assign(flattened_cholesky_factors)
-
-    # Update initialisers
-    if update_initializer:
-        means_layer.vectors_layer.tensor_initializer = WeightInitializer(means)
-        stds_layer.diagonals_layer.tensor_initializer = WeightInitializer(diagonals)
-        fcs_layer.flattened_cholesky_factors_layer.tensor_initializer = (
-            WeightInitializer(flattened_cholesky_factors)
-        )
-
-
-def set_stds_regularizer(model, training_dataset, epsilon):
-    n_batches = dtf.get_n_batches(training_dataset)
-    n_channels = dtf.get_n_channels(training_dataset)
-    range_ = dtf.get_range(training_dataset)
-
-    mu = np.zeros([n_channels], dtype=np.float32)
-    sigma = np.sqrt(np.log(2 * range_))
-
-    stds_layer = model.get_layer("stds")
-    learnable_tensor_layer = stds_layer.layers[0]
-    learnable_tensor_layer.regularizer = regularizers.LogNormal(
-        mu, sigma, epsilon, n_batches
+    # Model RNN:
+    # - p(theta_t | state_<t), predicts logits for the next state based
+    #   on a history of states.
+    mod_rnn_layer = ModelRNNLayer(
+        config.model_rnn,
+        config.model_normalization,
+        config.model_activation,
+        config.model_n_layers,
+        config.model_n_units,
+        config.model_dropout,
+        config.model_regularizer,
+        name="mod_rnn",
     )
+    mod_theta_layer = layers.Dense(config.n_states, name="mod_theta")
+    kl_div_layer = CategoricalKLDivergenceLayer(name="kl_div")
+    kl_loss_layer = KLLossLayer(config.do_kl_annealing, name="kl_loss")
+
+    mod_rnn = mod_rnn_layer(states)
+    mod_theta = mod_theta_layer(mod_rnn)
+    kl_div = kl_div_layer([inf_theta, mod_theta])
+    kl_loss = kl_loss_layer(kl_div)
 
-
-def set_fcs_regularizer(model, training_dataset, epsilon):
-    n_batches = dtf.get_n_batches(training_dataset)
-    n_channels = dtf.get_n_channels(training_dataset)
-
-    nu = n_channels - 1 + 0.1
-
-    fcs_layer = model.get_layer("fcs")
-    learnable_tensor_layer = fcs_layer.layers[0]
-    learnable_tensor_layer.regularizer = regularizers.MarginalInverseWishart(
-        nu,
-        epsilon,
-        n_channels,
-        n_batches,
+    return tf.keras.Model(
+        inputs=data, outputs=[ll_loss, kl_loss, inf_theta], name="State-DyNeMo"
     )
```

### Comparing `osl-dynamics-1.2.4/osl_dynamics/models/mod_base.py` & `osl-dynamics-1.2.5/osl_dynamics/models/mod_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import logging
 import os
 import re
 from abc import abstractmethod
 from dataclasses import dataclass
 from io import StringIO
+from contextlib import contextmanager
 
 import numpy as np
 import tensorflow
 import yaml
 from tensorflow.data import Dataset
 from tensorflow.keras import optimizers
 from tensorflow.python.distribute.distribution_strategy_context import get_strategy
@@ -431,14 +432,56 @@
             Directory to save the config object and weights of the model.
         """
         self.save_config(dirname)
         self.save_weights(
             f"{dirname}/weights"
         )  # will use the keras method: self.model.save_weights()
 
+    @contextmanager
+    def set_trainable(self, layers, values):
+        """Context manager to temporarily set the trainable attribute of layers.
+
+        Parameters
+        ----------
+        layers : str or list of str
+            List of layers to set the trainable attribute of.
+        values : bool or list of bool
+            Value to set the trainable attribute of the layers to.
+        """
+        # Validation
+        if isinstance(layers, str):
+            layers = [layers]
+        if isinstance(values, bool):
+            values = [values] * len(layers)
+        if len(layers) != len(values):
+            raise ValueError(
+                f"layers and trainable must be the same length, "
+                + f"but got {len(layers)} and {len(values)}."
+            )
+
+        available_layers = [layer.name for layer in self.layers]
+        for layer in layers:
+            if layer not in available_layers:
+                raise ValueError(
+                    f"No such layer: {layer}. "
+                    + f"Available layers are: {available_layers}."
+                )
+
+        original_values = [self.get_layer(layer).trainable for layer in layers]
+
+        try:
+            for layer, trainable in zip(layers, values):
+                self.get_layer(layer).trainable = trainable
+            self.compile()
+            yield
+        finally:
+            for layer, trainable in zip(layers, original_values):
+                self.get_layer(layer).trainable = trainable
+            self.compile()
+
     @staticmethod
     def load_config(dirname):
         """Load a config object from a .yml file.
 
         Parameters
         ----------
         dirname : str
```

### Comparing `osl-dynamics-1.2.4/osl_dynamics/models/sedynemo.py` & `osl-dynamics-1.2.5/osl_dynamics/models/sedynemo.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Literal
 
 import numpy as np
 import tensorflow as tf
 from tensorflow.keras import layers, initializers
 
 import osl_dynamics.data.tf as dtf
-from osl_dynamics.models import dynemo_obs, sedynemo_obs
+from osl_dynamics.models import obs_mod
 from osl_dynamics.models.mod_base import BaseModelConfig
 from osl_dynamics.models.inf_mod_base import (
     VariationalInferenceModelConfig,
     VariationalInferenceModelBase,
 )
 from osl_dynamics.inference.layers import (
     InferenceRNNLayer,
@@ -253,70 +253,71 @@
 
     config_type = Config
 
     def build_model(self):
         """Builds a keras model."""
         self.model = _model_structure(self.config)
 
-    def make_dataset(self, inputs, shuffle=False, concatenate=False, subj_id=True):
+    def make_dataset(self, inputs, **kwargs):
         """SE-DyNeMo requires subject id to be included in the dataset."""
-        return super().make_dataset(inputs, shuffle, concatenate, subj_id)
+        return super().make_dataset(inputs, subj_id=True, **kwargs)
 
     def fit(self, training_data, *args, **kwargs):
         # Set the scalings
         self.set_dev_mlp_reg_scaling(training_data)
         self.set_bayesian_kl_scaling(training_data)
         return super().fit(training_data, *args, **kwargs)
 
     def get_group_means(self):
-        """Get the group means.
+        """Get the group level mode means.
 
         Returns
         -------
         means : np.ndarray
             Group means. Shape is (n_modes, n_channels).
         """
-        return dynemo_obs.get_means(self.model, "group_means")
+        return obs_mod.get_observation_model_parameter(self.model, "group_means")
 
     def get_group_covariances(self):
-        """Get the group covariances.
+        """Get the group level mode covariances.
 
         Returns
         -------
         covariances : np.ndarray
             Group covariances. Shape is (n_modes, n_channels, n_channels).
         """
-        return dynemo_obs.get_covariances(self.model, "group_covs")
+        return obs_mod.get_observation_model_parameter(self.model, "group_covs")
 
     def get_group_means_covariances(self):
-        """Get the group means and covariances of each mode
+        """Get the group level mode means and covariances.
+        This is a wrapper for get_group_means and get_group_covariances.
 
         Returns
         -------
         means : np.ndarray
-            Mode means for the group. Shape is (n_modes, n_channels).
+            Group means. Shape is (n_modes, n_channels).
         covariances : np.ndarray
-            Mode covariances for the group. Shape is (n_modes, n_channels, n_channels).
+            Group covariances. Shape is (n_modes, n_channels, n_channels).
         """
-        return sedynemo_obs.get_group_means_covariances(self.model)
+        return self.get_group_means(), self.get_group_covariances()
 
-    def get_observation_model_parameters(self):
+    def get_group_observation_model_parameters(self):
         """Wrapper for get_group_means_covariances."""
         return self.get_group_means_covariances()
 
     def get_subject_embeddings(self):
         """Get the subject embedding vectors
 
         Returns
         -------
         subject_embeddings : np.ndarray
             Embedding vectors for subjects.
             Shape is (n_subjects, subject_embedding_dim).
         """
-        return sedynemo_obs.get_subject_embeddings(self.model)
+        return obs_mod.get_subject_embeddings(self.model)
 
     def get_subject_means_covariances(self, subject_embeddings=None, n_neighbours=2):
         """Get the means and covariances for each subject.
 
         Parameters
         ----------
         subject_embeddings : np.ndarray
@@ -328,15 +329,15 @@
         -------
         subject_means : np.ndarray
             Mode means for each subject. Shape is (n_subjects, n_modes, n_channels).
         subject_covs : np.ndarray
             Mode covariances for each subject.
             Shape is (n_subjects, n_modes, n_channels, n_channels).
         """
-        return sedynemo_obs.get_subject_means_covariances(
+        return obs_mod.get_subject_means_covariances(
             self.model,
             self.config.learn_means,
             self.config.learn_covariances,
             subject_embeddings,
             n_neighbours,
         )
 
@@ -351,68 +352,81 @@
         ----------
         training_dataset : tensorflow.data.Dataset or osl_dynamics.data.Data
             Training dataset.
         """
         training_dataset = self.make_dataset(training_dataset, concatenate=True)
 
         if self.config.learn_means:
-            dynemo_obs.set_means_regularizer(
+            obs_mod.set_means_regularizer(
                 self.model, training_dataset, layer_name="group_means"
             )
 
         if self.config.learn_covariances:
-            dynemo_obs.set_covariances_regularizer(
+            obs_mod.set_covariances_regularizer(
                 self.model,
                 training_dataset,
                 self.config.covariances_epsilon,
                 layer_name="group_covs",
             )
 
     def set_group_means(self, group_means, update_initializer=True):
         """Set the group means of each mode.
 
         Parameters
         ----------
         group_means : np.ndarray
-            Mode means.
+            Group level mode means. Shape is (n_modes, n_channels).
         update_initializer : bool
             Do we want to use the passed group means when we re-initialize the model?
         """
-        dynemo_obs.set_means(
-            self.model, group_means, update_initializer, layer_name="group_means"
+        obs_mod.set_observation_model_parameter(
+            self.model,
+            group_means,
+            layer_name="group_means",
+            update_initializer=update_initializer,
         )
 
     def set_group_covariances(self, group_covariances, update_initializer=True):
         """Set the group covariances of each mode.
 
         Parameters
         ----------
         group_covariances : np.ndarray
-            Mode covariances.
+            Group level mode covariances. Shape is (n_modes, n_channels, n_channels).
         update_initializer : bool
             Do we want to use the passed group covariances when we re-initialize
             the model?
         """
-        dynemo_obs.set_covariances(
+        obs_mod.set_observation_model_parameter(
             self.model,
             group_covariances,
-            update_initializer=update_initializer,
             layer_name="group_covs",
+            update_initializer=update_initializer,
         )
 
-    def set_observation_model_parameters(
-        self, observation_model_parameters, update_initializer=True
+    def set_group_means_covariances(
+        self, group_means, group_covariances, update_initializer=True
     ):
-        """Wrapper for set_group_means and set_group_covariances."""
+        """This is a wrapper for set_group_means and set_group_covariances."""
         self.set_group_means(
-            observation_model_parameters[0],
+            group_means,
             update_initializer=update_initializer,
         )
         self.set_group_covariances(
-            observation_model_parameters[1],
+            group_covariances,
+            update_initializer=update_initializer,
+        )
+
+    def set_group_observation_model_parameters(
+        self, group_observation_model_parameters, update_initializer=True
+    ):
+        """Wrapper for set_group_means_covariances."""
+        self.set_group_means_covariances(
+            group_observation_model_parameters[0],
+            group_observation_model_parameters[1],
             update_initializer=update_initializer,
         )
 
     def set_bayesian_kl_scaling(self, training_dataset):
         """Set the correct scaling for KL loss between deviation posterior and prior.
 
         Parameters
@@ -420,15 +434,15 @@
         training_dataset : tensorflow.data.Dataset or osl_dynamics.data.Data
             Training dataset.
         """
         training_dataset = self.make_dataset(training_dataset, concatenate=True)
         n_batches = dtf.get_n_batches(training_dataset)
         learn_means = self.config.learn_means
         learn_covariances = self.config.learn_covariances
-        sedynemo_obs.set_bayesian_kl_scaling(
+        obs_mod.set_bayesian_kl_scaling(
             self.model, n_batches, learn_means, learn_covariances
         )
 
     def set_dev_mlp_reg_scaling(self, training_dataset):
         """Set the correct scaling for the deviation MLP regularization.
 
         Parameters
@@ -436,15 +450,15 @@
         training_dataset : tensorflow.data.Dataset or osl_dynamics.data.Data
             Training dataset.
         """
         training_dataset = self.make_dataset(training_dataset, concatenate=True)
         n_batches = dtf.get_n_batches(training_dataset)
         learn_means = self.config.learn_means
         learn_covariances = self.config.learn_covariances
-        sedynemo_obs.set_dev_mlp_reg_scaling(
+        obs_mod.set_dev_mlp_reg_scaling(
             self.model, n_batches, learn_means, learn_covariances
         )
 
     def random_subject_initialization(self, **kwargs):
         """random subject initialisation not compatible with SE-DyNeMo."""
         raise AttributeError(
             " 'Model' object has no attribute 'random_subject_initialization'."
```

### Comparing `osl-dynamics-1.2.4/osl_dynamics/models/sedynemo_obs.py` & `osl-dynamics-1.2.5/osl_dynamics/models/obs_mod.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,731 +1,454 @@
-"""Subject Embedding Dynamic Network Modes (Se-DyNeMo) observation model.
+"""Helpful functions related to observation models.
 
 """
 
-from dataclasses import dataclass
 
 import numpy as np
 import tensorflow as tf
 from tensorflow_probability import bijectors as tfb
-from tensorflow.keras import layers, initializers
 
 import osl_dynamics.data.tf as dtf
-from osl_dynamics.models import dynemo_obs
-from osl_dynamics.models.mod_base import BaseModelConfig, ModelBase
-from osl_dynamics.inference.layers import (
-    LogLikelihoodLossLayer,
-    LearnableTensorLayer,
-    VectorsLayer,
-    CovarianceMatricesLayer,
-    ConcatEmbeddingsLayer,
-    SubjectMapLayer,
-    MixSubjectSpecificParametersLayer,
-    TFRangeLayer,
-    ZeroLayer,
-    InverseCholeskyLayer,
-    SampleGammaDistributionLayer,
-    StaticKLDivergenceLayer,
-    KLLossLayer,
-    MultiLayerPerceptronLayer,
-)
-
-
-@dataclass
-class Config(BaseModelConfig):
-    """Settings for DyNeMo observation model.
+from osl_dynamics.inference import regularizers
+from osl_dynamics.inference.initializers import WeightInitializer
 
-    Parameters
-    ----------
-    model_name : str
-        Model name.
-    n_modes : int
-        Number of modes.
-    n_channels : int
-        Number of channels.
-    sequence_length : int
-        Length of sequence passed to the generative model.
-    learn_means : bool
-        Should we make the mean vectors for each mode trainable?
-    learn_covariances : bool
-        Should we make the covariance matrix for each mode trainable?
-    initial_means : np.ndarray
-        Initialisation for mean vectors.
-    initial_covariances : np.ndarray
-        Initialisation for mode covariances.
-    covariances_epsilon : float
-        Error added to mode covariances for numerical stability.
-    means_regularizer : tf.keras.regularizers.Regularizer
-        Regularizer for group mean vectors.
-    covariances_regularizer : tf.keras.regularizers.Regularizer
-        Regularizer for group covariance matrices.
-
-    n_subjects : int
-        Number of subjects.
-    subject_embeddings_dim : int
-        Number of dimensions for the subject embeddings.
-    mode_embeddings_dim : int
-        Number of dimensions for the mode embeddings in the spatial maps encoder.
-
-    dev_n_layers : int
-        Number of layers for the MLP for deviations.
-    dev_n_units : int
-        Number of units for the MLP for deviations.
-    dev_normalization : str
-        Type of normalization for the MLP for deviations.
-        Either None, 'batch' or 'layer'.
-    dev_activation : str
-        Type of activation to use for the MLP for deviations.
-        E.g. 'relu', 'sigmoid', 'tanh', etc.
-    dev_dropout : float
-        Dropout rate for the MLP for deviations.
-    dev_regularizer : str
-        Regularizer for the MLP for deviations.
-    dev_regularizer_factor : float
-        Regularizer factor for the MLP for deviations.
-        This will be scaled by the amount of data.
-
-    batch_size : int
-        Mini-batch size.
-    learning_rate : float
-        Learning rate.
-    gradient_clip : float
-        Value to clip gradients by. This is the clipnorm argument passed to
-        the Keras optimizer. Cannot be used if multi_gpu=True.
-    n_epochs : int
-        Number of training epochs.
-    optimizer : str or tensorflow.keras.optimizers.Optimizer
-        Optimizer to use. 'adam' is recommended.
-    multi_gpu : bool
-        Should be use multiple GPUs for training?
-    strategy : str
-        Strategy for distributed learning.
-    """
-
-    model_name: str = "SE-DyNeMo-Obs"
-
-    # Observation model parameters
-    learn_means: bool = None
-    learn_covariances: bool = None
-    initial_means: np.ndarray = None
-    initial_covariances: np.ndarray = None
-    covariances_epsilon: float = None
-    means_regularizer: tf.keras.regularizers.Regularizer = None
-    covariances_regularizer: tf.keras.regularizers.Regularizer = None
-
-    # Parameters specific to subject embedding model
-    n_subjects: int = None
-    subject_embeddings_dim: int = None
-    mode_embeddings_dim: int = None
-
-    dev_n_layers: int = 0
-    dev_n_units: int = None
-    dev_normalization: str = None
-    dev_activation: str = None
-    dev_dropout: float = 0.0
-    dev_regularizer: str = None
-    dev_regularizer_factor: float = 0.0
-
-    def __post_init__(self):
-        self.validate_observation_model_parameters()
-        self.validate_dimension_parameters()
-        self.validate_training_parameters()
-        self.validate_subject_embedding_parameters()
-
-    def validate_observation_model_parameters(self):
-        if self.learn_means is None or self.learn_covariances is None:
-            raise ValueError("learn_means and learn_covariances must be passed.")
-
-        if self.covariances_epsilon is None:
-            if self.learn_covariances:
-                self.covariances_epsilon = 1e-6
-            else:
-                self.covariances_epsilon = 0.0
-
-    def validate_subject_embedding_parameters(self):
-        if (
-            self.n_subjects is None
-            or self.subject_embeddings_dim is None
-            or self.mode_embeddings_dim is None
-        ):
-            raise ValueError(
-                "n_subjects, subject_embeddings_dim and mode_embeddings_dim must be passed."
-            )
-
-        if self.dev_n_layers != 0 and self.dev_n_units is None:
-            raise ValueError("Please pass dev_inf_n_units.")
 
+def get_observation_model_parameter(model, layer_name):
+    """Get the parameter of an observation model layer.
 
-class Model(ModelBase):
-    """Observation model for directional SE-DyNeMo
+    Parameters
+    ----------
+    model : osl_dynamics.models.*.Model.model
+        The model.
+    layer_name : str
+        Name of the layer of the observation model parameter.
+
+    Returns
+    -------
+    obs_parameter : np.ndarray
+        The observation model parameter.
+    """
+    available_layers = ["means", "covs", "stds", "fcs", "group_means", "group_covs"]
+    if layer_name not in available_layers:
+        raise ValueError(
+            f"Layer name {layer_name} not in available layers {available_layers}."
+        )
+    obs_layer = model.get_layer(layer_name)
+    obs_parameter = obs_layer(1)
+    return obs_parameter.numpy()
+
+
+def set_observation_model_parameter(
+    model,
+    obs_parameter,
+    layer_name,
+    update_initializer=True,
+    diagonal_covariances=False,
+):
+    """Set the value of an observation model parameter.
 
     Parameters
     ----------
-    config : osl_dynamics.models.sedynemo_obs.Config
-    """
-
-    config_type = Config
-
-    def build_model(self):
-        """Builds a keras model."""
-        self.model = _model_structure(self.config)
-
-    def fit(self, training_data, *args, **kwargs):
-        # Set the scalings
-        self.set_dev_mlp_reg_scaling(training_data)
-        self.set_bayesian_kl_scaling(training_data)
-        return super().fit(training_data, *args, **kwargs)
-
-    def get_group_means(self):
-        """Get the group means.
-
-        Returns
-        -------
-        means : np.ndarray
-            Group means. Shape is (n_modes, n_channels).
-        """
-        return dynemo_obs.get_means(self.model, "group_means")
-
-    def get_group_covariances(self):
-        """Get the group covariances.
-
-        Returns
-        -------
-        covariances : np.ndarray
-            Group covariances. Shape is (n_modes, n_channels, n_channels).
-        """
-        return dynemo_obs.get_covariances(self.model, "group_covs")
-
-    def get_group_means_covariances(self):
-        """Get the group means and covariances of each mode.
-
-        Returns
-        -------
-        means : np.ndarray
-            Mode means for the group. Shape is (n_modes, n_channels).
-        covariances : np.ndarray
-            Mode covariances for the group. Shape is (n_modes, n_channels, n_channels).
-        """
-        return get_group_means_covariances(self.model)
-
-    def get_subject_embeddings(self):
-        """Get the subject embedding vectors.
-
-        Returns
-        -------
-        subject_embeddings : np.ndarray
-            Embedding vectors for subjects. Shape is (n_subjects, subject_embeddings_dim).
-        """
-        return get_subject_embeddings(self.model)
-
-    def get_subject_means_covariances(self, subject_embeddings=None, n_neighbours=2):
-        """Get the means and covariances for each subject.
-
-        Parameters
-        ----------
-        subject_embeddings : np.ndarray
-            Input embedding vectors for subjects. Shape is (n_subjects, subject_embeddings_dim).
-        n_neighbours : int
-            Number of nearest neighbours. Ignored if subject_embedding=None.
-
-        Returns
-        -------
-        subject_means : np.ndarray
-            Mode means for each subject. Shape is (n_subjects, n_modes, n_channels).
-        subject_covs : np.ndarray
-            Mode covariances for each subject. Shape is (n_subjects, n_modes, n_channels, n_channels).
-        """
-        return get_subject_means_covariances(
-            self.model,
-            self.config.learn_means,
-            self.config.learn_covariances,
-            subject_embeddings,
-            n_neighbours,
+    model : osl_dynamics.models.*.Model.model
+        The model.
+    obs_parameter : np.ndarray
+        The value of the observation model parameter to set.
+    layer_name : str
+        Layer name of the observation model parameter.
+    update_initializer : bool
+        Whether to update the initializer of the layer.
+    diagonal_covariances : bool
+        Whether the covariances are diagonal. Ignored if layer_name is not "covs".
+    """
+    available_layers = ["means", "covs", "stds", "fcs", "group_means", "group_covs"]
+    if layer_name not in available_layers:
+        raise ValueError(
+            f"Layer name {layer_name} not in available layers {available_layers}."
         )
 
-    def set_regularizers(self, training_dataset):
-        """Set the means and covariances regularizer based on the training data.
+    obs_parameter = obs_parameter.astype(np.float32)
 
-        A multivariate normal prior is applied to the mean vectors with mu = 0,
-        sigma=diag((range / 2)**2) and an inverse Wishart prior is applied to the
-        covariances matrices with nu=n_channels - 1 + 0.1 and psi=diag(range).
-
-        Parameters
-        ----------
-        training_data : tensorflow.data.Dataset
-            Training dataset.
-        """
-        training_dataset = self.make_dataset(training_dataset, concatenate=True)
-
-        if self.config.learn_means:
-            dynemo_obs.set_means_regularizer(
-                self.model, training_dataset, layer_name="group_means"
-            )
+    if layer_name == "stds" or (layer_name == "covs" and diagonal_covariances):
+        if obs_parameter.ndim == 3:
+            # Only keep the diagonal as a vector
+            obs_parameter = np.diagonal(obs_parameter, axis1=1, axis2=2)
 
-        if self.config.learn_covariances:
-            dynemo_obs.set_covariances_regularizer(
-                self.model,
-                training_dataset,
-                self.config.covariances_epsilon,
-                layer_name="group_covs",
-            )
+    obs_layer = model.get_layer(layer_name)
+    learnable_tensor_layer = obs_layer.layers[0]
 
-    def set_bayesian_kl_scaling(self, training_dataset):
-        """Set the correct scaling for KL loss between deviation posterior and prior."""
-        n_batches = dtf.get_n_batches(training_dataset)
-        learn_means = self.config.learn_means
-        learn_covariances = self.config.learn_covariances
-        set_bayesian_kl_scaling(self.model, n_batches, learn_means, learn_covariances)
-
-    def set_dev_mlp_reg_scaling(self, training_dataset):
-        """Set the correct scaling for the dev mlp regularization."""
-        n_batches = dtf.get_n_batches(training_dataset)
-        learn_means = self.config.learn_means
-        learn_covariances = self.config.learn_covariances
-        set_dev_mlp_reg_scaling(self.model, n_batches, learn_means, learn_covariances)
-
-    def set_group_means(self, group_means, update_initializer=True):
-        """Set the group means of each mode.
-
-        Parameters
-        ----------
-        group_means : np.ndarray
-            Mode means.
-        update_initializer : bool
-            Do we want to use the passed group means when we re-initialize the model?
-        """
-        dynemo_obs.set_means(
-            self.model, group_means, update_initializer, layer_name="group_means"
-        )
+    if layer_name not in ["means", "group_means"]:
+        obs_parameter = obs_layer.bijector.inverse(obs_parameter)
 
-    def set_group_covariances(self, group_covariances, update_initializer=True):
-        """Set the group covariances of each mode.
+    learnable_tensor_layer.tensor.assign(obs_parameter)
 
-        Parameters
-        ----------
-        group_covariances : np.ndarray
-            Mode covariances.
-        update_initializer : bool
-            Do we want to use the passed group covariances when we re-initialize
-            the model?
-        """
-        dynemo_obs.set_covariances(
-            self.model,
-            group_covariances,
-            update_initializer=update_initializer,
-            layer_name="group_covs",
-        )
+    if update_initializer:
+        learnable_tensor_layer.tensor_initializer = WeightInitializer(obs_parameter)
 
 
-def _model_structure(config):
-    # Layers for inputs
-    data = layers.Input(shape=(config.sequence_length, config.n_channels), name="data")
-    alpha = layers.Input(shape=(config.sequence_length, config.n_modes), name="alpha")
-    subj_id = layers.Input(shape=(config.sequence_length,), name="subj_id")
-
-    # Subject embedding layers
-    subjects_layer = TFRangeLayer(config.n_subjects, name="subjects")
-    subject_embeddings_layer = layers.Embedding(
-        config.n_subjects, config.subject_embeddings_dim, name="subject_embeddings"
-    )
+def set_means_regularizer(model, training_dataset, layer_name="means"):
+    """Set the means regularizer based on training data.
 
-    # Group level observation model parameters
-    group_means_layer = VectorsLayer(
-        config.n_modes,
-        config.n_channels,
-        config.learn_means,
-        config.initial_means,
-        config.means_regularizer,
-        name="group_means",
-    )
-    group_covs_layer = CovarianceMatricesLayer(
-        config.n_modes,
-        config.n_channels,
-        config.learn_covariances,
-        config.initial_covariances,
-        config.covariances_epsilon,
-        config.covariances_regularizer,
-        name="group_covs",
+    A multivariate normal prior is applied to the mean vectors with mu = 0,
+    sigma=diag((range / 2)**2).
+
+    Parameters
+    ----------
+    model : osl_dynamics.models.*.Model.model
+        The model.
+    training_dataset : osl_dynamics.data.Data
+        The training dataset.
+    layer_name : str
+        Layer name of the means. Can be "means" or "group_means".
+    """
+    n_batches = dtf.get_n_batches(training_dataset)
+    n_channels = dtf.get_n_channels(training_dataset)
+    range_ = dtf.get_range(training_dataset)
+
+    mu = np.zeros(n_channels, dtype=np.float32)
+    sigma = np.diag((range_ / 2) ** 2)
+
+    means_layer = model.get_layer(layer_name)
+    learnable_tensor_layer = means_layer.layers[0]
+    learnable_tensor_layer.regularizer = regularizers.MultivariateNormal(
+        mu, sigma, n_batches
     )
 
-    subjects = subjects_layer(data)
-    subject_embeddings = subject_embeddings_layer(subjects)
 
-    group_mu = group_means_layer(data)
-    group_D = group_covs_layer(data)
+def set_covariances_regularizer(
+    model,
+    training_dataset,
+    epsilon,
+    diagonal=False,
+    layer_name="covs",
+):
+    """Set the covariances regularizer based on training data.
 
-    # ---------------
-    # Mean deviations
+    If config.diagonal_covariances is True, a log-normal prior is applied to the
+    diagonal of the covariance matrices with mu = 0, sigma=sqrt(log(2 * range)).
+    Otherwise, an inverse Wishart prior is applied to the covariance matrices with
+    nu = n_channels - 1 + 0.1, psi=diag(1 / range).
 
-    # Layer definitions
-    if config.learn_means:
-        means_mode_embeddings_layer = layers.Dense(
-            config.mode_embeddings_dim,
-            name="means_mode_embeddings",
-        )
-        means_concat_embeddings_layer = ConcatEmbeddingsLayer(
-            name="means_concat_embeddings",
-        )
+    Parameters
+    ----------
+    model : osl_dynamics.models.*.Model.model
+        The model.
+    training_dataset : osl_dynamics.data.Data
+        The training dataset.
+    epsilon : float
+        Error added to the covariance matrices.
+    diagonal : bool
+        Whether the covariances are diagonal.
+    layer_name : str
+        Layer name of the covariances. Can be "covs" or "group_covs".
+    """
+    n_batches = dtf.get_n_batches(training_dataset)
+    n_channels = dtf.get_n_channels(training_dataset)
+    range_ = dtf.get_range(training_dataset)
 
-        means_dev_map_input_layer = MultiLayerPerceptronLayer(
-            config.dev_n_layers,
-            config.dev_n_units,
-            config.dev_normalization,
-            config.dev_activation,
-            config.dev_dropout,
-            config.dev_regularizer,
-            config.dev_regularizer_factor,
-            name="means_dev_map_input",
-        )
-        means_dev_map_layer = layers.Dense(config.n_channels, name="means_dev_map")
-        norm_means_dev_map_layer = layers.LayerNormalization(
-            axis=-1, name="norm_means_dev_map"
+    covs_layer = model.get_layer(layer_name)
+    if diagonal:
+        mu = np.zeros([n_channels], dtype=np.float32)
+        sigma = np.sqrt(np.log(2 * range_))
+        learnable_tensor_layer = covs_layer.layers[0]
+        learnable_tensor_layer.regularizer = regularizers.LogNormal(
+            mu, sigma, epsilon, n_batches
         )
 
-        means_dev_mag_inf_alpha_input_layer = LearnableTensorLayer(
-            shape=(config.n_subjects, config.n_modes, 1),
-            learn=config.learn_means,
-            initializer=initializers.TruncatedNormal(mean=0, stddev=0.02),
-            name="means_dev_mag_inf_alpha_input",
-        )
-        means_dev_mag_inf_alpha_layer = layers.Activation(
-            "softplus", name="means_dev_mag_inf_alpha"
-        )
-        means_dev_mag_inf_beta_input_layer = LearnableTensorLayer(
-            shape=(config.n_subjects, config.n_modes, 1),
-            learn=config.learn_means,
-            initializer=initializers.TruncatedNormal(mean=0, stddev=0.02),
-            name="means_dev_mag_inf_beta_input",
-        )
-        means_dev_mag_inf_beta_layer = layers.Activation(
-            "softplus", name="means_dev_mag_inf_beta"
-        )
-        means_dev_mag_layer = SampleGammaDistributionLayer(
-            config.covariances_epsilon, name="means_dev_mag"
+    else:
+        nu = n_channels - 1 + 0.1
+        psi = np.diag(range_)
+        learnable_tensor_layer = covs_layer.layers[0]
+        learnable_tensor_layer.regularizer = regularizers.InverseWishart(
+            nu, psi, epsilon, n_batches
         )
 
-        means_dev_layer = layers.Multiply(name="means_dev")
 
-        # Data flow to get the subject specific deviations of means
+def set_stds_regularizer(model, training_dataset, epsilon):
+    """Set the standard deviations regularizer based on training data.
 
-        # Get the concatenated embeddings
-        means_mode_embeddings = means_mode_embeddings_layer(group_mu)
-        means_concat_embeddings = means_concat_embeddings_layer(
-            [subject_embeddings, means_mode_embeddings]
-        )
+    A log-normal prior is applied to the standard deviations with mu = 0,
+    sigma=sqrt(log(2 * range)).
 
-        # Get the mean deviation maps (no global magnitude information)
-        means_dev_map_input = means_dev_map_input_layer([data, means_concat_embeddings])
-        means_dev_map = means_dev_map_layer(means_dev_map_input)
-        norm_means_dev_map = norm_means_dev_map_layer(means_dev_map)
-
-        # Get the deviation magnitudes (scale deviation maps globally)
-
-        means_dev_mag_inf_alpha_input = means_dev_mag_inf_alpha_input_layer(data)
-        means_dev_mag_inf_alpha = means_dev_mag_inf_alpha_layer(
-            means_dev_mag_inf_alpha_input
-        )
-        means_dev_mag_inf_beta_input = means_dev_mag_inf_beta_input_layer(data)
-        means_dev_mag_inf_beta = means_dev_mag_inf_beta_layer(
-            means_dev_mag_inf_beta_input
-        )
-        means_dev_mag = means_dev_mag_layer(
-            [means_dev_mag_inf_alpha, means_dev_mag_inf_beta]
-        )
-        means_dev = means_dev_layer([means_dev_mag, norm_means_dev_map])
-    else:
-        means_dev_layer = ZeroLayer(
-            shape=(config.n_subjects, config.n_modes, config.n_channels),
-            name="means_dev",
-        )
-        means_dev = means_dev_layer(data)
+    Parameters
+    ----------
+    model : osl_dynamics.models.*.Model.model
+        The model.
+    training_dataset : osl_dynamics.data.Data
+        The training dataset.
+    epsilon : float
+        Error added to the standard deviations.
+    """
+    n_batches = dtf.get_n_batches(training_dataset)
+    n_channels = dtf.get_n_channels(training_dataset)
+    range_ = dtf.get_range(training_dataset)
 
-    # ----------------------
-    # Covariances deviations
+    mu = np.zeros([n_channels], dtype=np.float32)
+    sigma = np.sqrt(np.log(2 * range_))
 
-    # Layer definitions
-    if config.learn_covariances:
-        covs_mode_embeddings_layer = layers.Dense(
-            config.mode_embeddings_dim,
-            name="covs_mode_embeddings",
-        )
-        covs_concat_embeddings_layer = ConcatEmbeddingsLayer(
-            name="covs_concat_embeddings",
-        )
-
-        covs_dev_map_input_layer = MultiLayerPerceptronLayer(
-            config.dev_n_layers,
-            config.dev_n_units,
-            config.dev_normalization,
-            config.dev_activation,
-            config.dev_dropout,
-            config.dev_regularizer,
-            config.dev_regularizer_factor,
-            name="covs_dev_map_input",
-        )
-        covs_dev_map_layer = layers.Dense(
-            config.n_channels * (config.n_channels + 1) // 2, name="covs_dev_map"
-        )
-        norm_covs_dev_map_layer = layers.LayerNormalization(
-            axis=-1, name="norm_covs_dev_map"
-        )
+    stds_layer = model.get_layer("stds")
+    learnable_tensor_layer = stds_layer.layers[0]
+    learnable_tensor_layer.regularizer = regularizers.LogNormal(
+        mu, sigma, epsilon, n_batches
+    )
 
-        covs_dev_mag_inf_alpha_input_layer = LearnableTensorLayer(
-            shape=(config.n_subjects, config.n_modes, 1),
-            learn=config.learn_covariances,
-            initializer=initializers.TruncatedNormal(mean=0, stddev=0.02),
-            name="covs_dev_mag_inf_alpha_input",
-        )
-        covs_dev_mag_inf_alpha_layer = layers.Activation(
-            "softplus", name="covs_dev_mag_inf_alpha"
-        )
-        covs_dev_mag_inf_beta_input_layer = LearnableTensorLayer(
-            shape=(config.n_subjects, config.n_modes, 1),
-            learn=config.learn_covariances,
-            initializer=initializers.TruncatedNormal(mean=0, stddev=0.02),
-            name="covs_dev_mag_inf_beta_input",
-        )
-        covs_dev_mag_inf_beta_layer = layers.Activation(
-            "softplus", name="covs_dev_mag_inf_beta"
-        )
-        covs_dev_mag_layer = SampleGammaDistributionLayer(
-            config.covariances_epsilon, name="covs_dev_mag"
-        )
-        covs_dev_layer = layers.Multiply(name="covs_dev")
 
-        # Data flow to get subject specific deviations of covariances
+def set_fcs_regularizer(model, training_dataset, epsilon):
+    """Set the FCS regularizer based on training data.
 
-        # Get the concatenated embeddings
-        covs_mode_embeddings = covs_mode_embeddings_layer(
-            InverseCholeskyLayer(config.covariances_epsilon)(group_D)
-        )
-        covs_concat_embeddings = covs_concat_embeddings_layer(
-            [subject_embeddings, covs_mode_embeddings]
-        )
+    A marginal inverse Wishart prior is applied to the FCS
+    with nu = n_channels - 1 + 0.1.
 
-        # Get the covariance deviation maps (no global magnitude information)
-        covs_dev_map_input = covs_dev_map_input_layer([data, covs_concat_embeddings])
-        covs_dev_map = covs_dev_map_layer(covs_dev_map_input)
-        norm_covs_dev_map = norm_covs_dev_map_layer(covs_dev_map)
-
-        # Get the deviation magnitudes (scale deviation maps globally)
-        covs_dev_mag_inf_alpha_input = covs_dev_mag_inf_alpha_input_layer(data)
-        covs_dev_mag_inf_alpha = covs_dev_mag_inf_alpha_layer(
-            covs_dev_mag_inf_alpha_input
-        )
-        covs_dev_mag_inf_beta_input = covs_dev_mag_inf_beta_input_layer(data)
-        covs_dev_mag_inf_beta = covs_dev_mag_inf_beta_layer(covs_dev_mag_inf_beta_input)
-        covs_dev_mag = covs_dev_mag_layer(
-            [covs_dev_mag_inf_alpha, covs_dev_mag_inf_beta]
-        )
-        covs_dev = covs_dev_layer([covs_dev_mag, norm_covs_dev_map])
-    else:
-        covs_dev_layer = ZeroLayer(
-            shape=(
-                config.n_subjects,
-                config.n_modes,
-                config.n_channels * (config.n_channels + 1) // 2,
-            ),
-            name="covs_dev",
-        )
-        covs_dev = covs_dev_layer(data)
+    Parameters
+    ----------
+    model : osl_dynamics.models.*.Model.model
+        The model.
+    training_dataset : osl_dynamics.data.Data
+        The training dataset.
+    epsilon : float
+        Error added to the FCS.
+    """
+    n_batches = dtf.get_n_batches(training_dataset)
+    n_channels = dtf.get_n_channels(training_dataset)
 
-    # ----------------------------------------
-    # Add deviations to group level parameters
+    nu = n_channels - 1 + 0.1
 
-    # Layer definitions
-    subject_means_layer = SubjectMapLayer(
-        "means", config.covariances_epsilon, name="subject_means"
-    )
-    subject_covs_layer = SubjectMapLayer(
-        "covariances", config.covariances_epsilon, name="subject_covs"
+    fcs_layer = model.get_layer("fcs")
+    learnable_tensor_layer = fcs_layer.layers[0]
+    learnable_tensor_layer.regularizer = regularizers.MarginalInverseWishart(
+        nu,
+        epsilon,
+        n_channels,
+        n_batches,
     )
 
-    # Data flow
-    mu = subject_means_layer([group_mu, means_dev])
-    D = subject_covs_layer([group_D, covs_dev])
-
-    # -----------------------------------
-    # Mix the subject specific paraemters
-    # and get the conditional likelihood
-
-    # Layer definitions
-    mix_subject_means_covs_layer = MixSubjectSpecificParametersLayer(
-        name="mix_subject_means_covs"
-    )
-    ll_loss_layer = LogLikelihoodLossLayer(config.covariances_epsilon, name="ll_loss")
 
-    # Data flow
-    m, C = mix_subject_means_covs_layer([alpha, mu, D, subj_id])
-    ll_loss = ll_loss_layer([data, m, C])
-
-    # ---------
-    # KL losses
-
-    # For the observation model (static KL loss)
-    if config.learn_means:
-        # Layer definitions
-        means_dev_mag_mod_beta_input_layer = MultiLayerPerceptronLayer(
-            config.dev_n_layers,
-            config.dev_n_units,
-            config.dev_normalization,
-            config.dev_activation,
-            config.dev_dropout,
-            config.dev_regularizer,
-            config.dev_regularizer_factor,
-            name="means_dev_mag_mod_beta_input",
-        )
-        means_dev_mag_mod_beta_layer = layers.Dense(
-            1,
-            activation="softplus",
-            name="means_dev_mag_mod_beta",
-        )
+def get_subject_embeddings(model):
+    """Get the subject embeddings.
 
-        means_dev_mag_kl_loss_layer = StaticKLDivergenceLayer(
-            config.covariances_epsilon, name="means_dev_mag_kl_loss"
-        )
+    Parameters
+    ----------
+    model : osl_dynamics.models.*.Model.model
+        The model. * must be sehmm or sedynemo.
 
-        # Data flow
-        means_dev_mag_mod_beta_input = means_dev_mag_mod_beta_input_layer(
-            [data, means_concat_embeddings]
-        )
-        means_dev_mag_mod_beta = means_dev_mag_mod_beta_layer(
-            means_dev_mag_mod_beta_input
-        )
-        means_dev_mag_kl_loss = means_dev_mag_kl_loss_layer(
-            [
-                data,
-                means_dev_mag_inf_alpha,
-                means_dev_mag_inf_beta,
-                means_dev_mag_mod_beta,
-            ]
-        )
-    else:
-        means_dev_mag_kl_loss_layer = ZeroLayer((), name="means_dev_mag_kl_loss")
-        means_dev_mag_kl_loss = means_dev_mag_kl_loss_layer(data)
+    Returns
+    -------
+    subject_embeddings : np.ndarray
+        The subject embeddings. Shape is (n_subjects, subject_embeddings_dim).
+    """
+    subject_embeddings_layer = model.get_layer("subject_embeddings")
+    n_subjects = subject_embeddings_layer.input_dim
+    return subject_embeddings_layer(np.arange(n_subjects)).numpy()
 
-    if config.learn_covariances:
-        # Layer definitions
-        covs_dev_mag_mod_beta_input_layer = MultiLayerPerceptronLayer(
-            config.dev_n_layers,
-            config.dev_n_units,
-            config.dev_normalization,
-            config.dev_activation,
-            config.dev_dropout,
-            config.dev_regularizer,
-            config.dev_regularizer_factor,
-            name="covs_dev_mag_mod_beta_input",
-        )
-        covs_dev_mag_mod_beta_layer = layers.Dense(
-            1,
-            activation="softplus",
-            name="covs_dev_mag_mod_beta",
-        )
 
-        covs_dev_mag_kl_loss_layer = StaticKLDivergenceLayer(
-            config.covariances_epsilon, name="covs_dev_mag_kl_loss"
-        )
+def get_means_mode_embeddings(model):
+    """Get the means mode embeddings.
 
-        # Data flow
-        covs_dev_mag_mod_beta_input = covs_dev_mag_mod_beta_input_layer(
-            [data, covs_concat_embeddings]
-        )
-        covs_dev_mag_mod_beta = covs_dev_mag_mod_beta_layer(covs_dev_mag_mod_beta_input)
-        covs_dev_mag_kl_loss = covs_dev_mag_kl_loss_layer(
-            [
-                data,
-                covs_dev_mag_inf_alpha,
-                covs_dev_mag_inf_beta,
-                covs_dev_mag_mod_beta,
-            ]
-        )
-    else:
-        covs_dev_mag_kl_loss_layer = ZeroLayer((), name="covs_dev_mag_kl_loss")
-        covs_dev_mag_kl_loss = covs_dev_mag_kl_loss_layer(data)
+    Parameters
+    ----------
+    model : osl_dynamics.models.*.Model.model
+        The model. * must be sehmm or sedynemo.
 
-    # Total KL loss
-    # Layer definitions
-    kl_loss_layer = KLLossLayer(False, name="kl_loss")
-
-    # Data flow
-    kl_loss = kl_loss_layer([means_dev_mag_kl_loss, covs_dev_mag_kl_loss])
-
-    return tf.keras.Model(
-        inputs=[data, alpha, subj_id],
-        outputs=[ll_loss, kl_loss],
-        name="Se_DyNeMo-Obs",
-    )
+    Returns
+    -------
+    means_mode_embeddings : np.ndarray
+        The means mode embeddings. Shape is (n_modes, mode_embeddings_dim).
+    """
+    group_means = get_observation_model_parameter(model, "group_means")
+    means_mode_embeddings_layer = model.get_layer("means_mode_embeddings")
+    means_mode_embeddings = means_mode_embeddings_layer(group_means)
+    return means_mode_embeddings.numpy()
 
 
-def get_group_means_covariances(model):
-    """Wrapper for getting the group level means and covariances."""
-    group_means = dynemo_obs.get_means(model, "group_means")
-    group_covariances = dynemo_obs.get_covariances(model, "group_covs")
-    return group_means, group_covariances
+def get_covs_mode_embeddings(model):
+    """Get the covariances mode embeddings.
 
+    Parameters
+    ----------
+    model : osl_dynamics.models.*.Model.model
+        The model. * must be sehmm or sedynemo.
 
-def get_subject_embeddings(model):
-    subject_embeddings_layer = model.get_layer("subject_embeddings")
-    n_subjects = subject_embeddings_layer.input_dim
-    return subject_embeddings_layer(np.arange(n_subjects)).numpy()
+    Returns
+    -------
+    covs_mode_embeddings : np.ndarray
+        The covariances mode embeddings. Shape is (n_modes, mode_embeddings_dim).
+    """
+    cholesky_bijector = tfb.Chain([tfb.CholeskyOuterProduct(), tfb.FillScaleTriL()])
+    group_covs = get_observation_model_parameter(model, "group_covs")
+    covs_mode_embeddings_layer = model.get_layer("covs_mode_embeddings")
+    covs_mode_embeddings = covs_mode_embeddings_layer(
+        cholesky_bijector.inverse(group_covs)
+    )
+    return covs_mode_embeddings.numpy()
 
 
 def get_mode_embeddings(model, map):
     """Wrapper for getting the mode embeddings for the means and covariances."""
     if map == "means":
-        return _get_means_mode_embeddings(model)
+        return get_means_mode_embeddings(model)
     elif map == "covs":
-        return _get_covs_mode_embeddings(model)
+        return get_covs_mode_embeddings(model)
     else:
         raise ValueError("map must be either 'means' or 'covs'")
 
 
 def get_concatenated_embeddings(model, map, subject_embeddings=None):
-    """Getting the concatenated embeddings for the means and covariances."""
+    """Get the concatenated embeddings.
+
+    Parameters
+    ----------
+    model : osl_dynamics.models.*.Model.model
+        The model. * must be sehmm or sedynemo.
+    map : str
+        The map to use. Either "means" or "covs".
+    subject_embeddings : np.ndarray
+        Input subject embeddings. If None, they are retrieved from the model.
+        Shape is (n_subjects, subject_embeddings_dim).
+
+    Returns
+    -------
+    concat_embeddings : np.ndarray
+        The concatenated embeddings.
+        Shape is (n_subjects, n_modes, subject_embeddings_dim + mode_embeddings_dim).
+    """
     if subject_embeddings is None:
         subject_embeddings = get_subject_embeddings(model)
     if map == "means":
-        mode_embeddings = _get_means_mode_embeddings(model)
+        mode_embeddings = get_means_mode_embeddings(model)
         concat_embeddings_layer = model.get_layer("means_concat_embeddings")
     elif map == "covs":
-        mode_embeddings = _get_covs_mode_embeddings(model)
+        mode_embeddings = get_covs_mode_embeddings(model)
         concat_embeddings_layer = model.get_layer("covs_concat_embeddings")
     else:
         raise ValueError("map must be either 'means' or 'covs'")
     concat_embeddings = concat_embeddings_layer([subject_embeddings, mode_embeddings])
     return concat_embeddings.numpy()
 
 
+def get_means_dev_mag_parameters(model):
+    """Get the means deviation magnitude parameters.
+
+    Parameters
+    ----------
+    model : osl_dynamics.models.*.Model.model
+        The model. * must be sehmm or sedynemo.
+
+    Returns
+    -------
+    means_dev_mag_inf_alpha : np.ndarray
+        The means deviation magnitude alpha parameters.
+        Shape is (n_subjects, n_modes, 1).
+    means_dev_mag_inf_beta : np.ndarray
+        The means deviation magnitude beta parameters.
+        Shape is (n_subjects, n_modes, 1).
+    """
+    means_dev_mag_inf_alpha_input_layer = model.get_layer(
+        "means_dev_mag_inf_alpha_input"
+    )
+    means_dev_mag_inf_alpha_layer = model.get_layer("means_dev_mag_inf_alpha")
+    means_dev_mag_inf_beta_input_layer = model.get_layer("means_dev_mag_inf_beta_input")
+    means_dev_mag_inf_beta_layer = model.get_layer("means_dev_mag_inf_beta")
+
+    means_dev_mag_inf_alpha_input = means_dev_mag_inf_alpha_input_layer(1)
+    means_dev_mag_inf_alpha = means_dev_mag_inf_alpha_layer(
+        means_dev_mag_inf_alpha_input
+    )
+
+    means_dev_mag_inf_beta_input = means_dev_mag_inf_beta_input_layer(1)
+    means_dev_mag_inf_beta = means_dev_mag_inf_beta_layer(means_dev_mag_inf_beta_input)
+    return means_dev_mag_inf_alpha.numpy(), means_dev_mag_inf_beta.numpy()
+
+
+def get_covs_dev_mag_parameters(model):
+    """Get the covariances deviation magnitude parameters.
+
+    Parameters
+    ----------
+    model : osl_dynamics.models.*.Model.model
+        The model. * must be sehmm or sedynemo.
+
+    Returns
+    -------
+    covs_dev_mag_inf_alpha : np.ndarray
+        The covariances deviation magnitude alpha parameters.
+        Shape is (n_subjects, n_modes, 1).
+    covs_dev_mag_inf_beta : np.ndarray
+        The covariances deviation magnitude beta parameters.
+        Shape is (n_subjects, n_modes, 1).
+    """
+    covs_dev_mag_inf_alpha_input_layer = model.get_layer("covs_dev_mag_inf_alpha_input")
+    covs_dev_mag_inf_alpha_layer = model.get_layer("covs_dev_mag_inf_alpha")
+    covs_dev_mag_inf_beta_input_layer = model.get_layer("covs_dev_mag_inf_beta_input")
+    covs_dev_mag_inf_beta_layer = model.get_layer("covs_dev_mag_inf_beta")
+
+    covs_dev_mag_inf_alpha_input = covs_dev_mag_inf_alpha_input_layer(1)
+    covs_dev_mag_inf_alpha = covs_dev_mag_inf_alpha_layer(covs_dev_mag_inf_alpha_input)
+
+    covs_dev_mag_inf_beta_input = covs_dev_mag_inf_beta_input_layer(1)
+    covs_dev_mag_inf_beta = covs_dev_mag_inf_beta_layer(covs_dev_mag_inf_beta_input)
+    return covs_dev_mag_inf_alpha.numpy(), covs_dev_mag_inf_beta.numpy()
+
+
 def get_dev_mag_parameters(model, map):
     """Wrapper for getting the deviance magnitude parameters
     for the means and covariances."""
     if map == "means":
-        return _get_means_dev_mag_parameters(model)
+        return get_means_dev_mag_parameters(model)
     elif map == "covs":
-        return _get_covs_dev_mag_parameters(model)
+        return get_covs_dev_mag_parameters(model)
     else:
         raise ValueError("map must be either 'means' or 'covs'")
 
 
 def get_dev_mag(model, map):
-    """Getting the deviance magnitude for the means and covariances."""
+    """Getting the deviance magnitude.
+
+    Parameters
+    ----------
+    model : osl_dynamics.models.*.Model.model
+        The model. * must be sehmm or sedynemo.
+    map : str
+        The map. Must be either 'means' or 'covs'.
+
+    Returns
+    -------
+    dev_mag : np.ndarray
+        The deviance magnitude. Shape is (n_subjects, n_modes, 1).
+    """
     if map == "means":
-        alpha, beta = _get_means_dev_mag_parameters(model)
+        alpha, beta = get_means_dev_mag_parameters(model)
         dev_mag_layer = model.get_layer("means_dev_mag")
     elif map == "covs":
-        alpha, beta = _get_covs_dev_mag_parameters(model)
+        alpha, beta = get_covs_dev_mag_parameters(model)
         dev_mag_layer = model.get_layer("covs_dev_mag")
     else:
         raise ValueError("map must be either 'means' or 'covs'")
     dev_mag = dev_mag_layer([alpha, beta])
     return dev_mag.numpy()
 
 
 def get_dev_map(model, map, subject_embeddings=None):
-    """Getting the deviance map for the means and covariances."""
+    """Get the deviance map.
+
+    Parameters
+    ----------
+    model : osl_dynamics.models.*.Model.model
+        The model. * must be sehmm or sedynemo.
+    map : str
+        The map to use. Either "means" or "covs".
+    subject_embeddings : np.ndarray
+        Input subject embeddings. If None, they are retrieved from the model.
+        Shape is (n_subjects, subject_embeddings_dim).
+
+    Returns
+    -------
+    dev_map : np.ndarray
+        The deviance map.
+        If map == "means", shape is (n_subjects, n_modes, n_channels).
+        If map == "covs", shape is (n_subjects, n_modes, n_channels * (n_channels + 1) // 2).
+    """
     concat_embeddings = get_concatenated_embeddings(model, map, subject_embeddings)
     if map == "means":
         dev_map_input_layer = model.get_layer("means_dev_map_input")
         dev_map_layer = model.get_layer("means_dev_map")
         norm_dev_map_layer = model.get_layer("norm_means_dev_map")
     elif map == "covs":
         dev_map_input_layer = model.get_layer("covs_dev_map_input")
@@ -738,14 +461,38 @@
     norm_dev_map = norm_dev_map_layer(dev_map)
     return norm_dev_map.numpy()
 
 
 def get_subject_dev(
     model, learn_means, learn_covariances, subject_embeddings=None, n_neighbours=2
 ):
+    """Get the subject deviation.
+
+    Parameters
+    ----------
+    model : osl_dynamics.models.*.Model.model
+        The model. * must be sehmm or sedynemo.
+    learn_means : bool
+        Whether the mean is learnt.
+    learn_covariances : bool
+        Whether the covariances are learnt.
+    subject_embeddings : np.ndarray
+        Input subject embeddings. Shape is (n_subjects, subject_embeddings_dim).
+        If None, then the subject embeddings are retrieved from the model.
+    n_neighbours : int
+        The number of nearest neighbours if subject_embedding is not None.
+
+    Returns
+    -------
+    means_dev : np.ndarray
+        The means deviation. Shape is (n_subjects, n_modes, n_channels).
+    covs_dev : np.ndarray
+        The covariances deviation.
+        Shape is (n_subjects, n_modes, n_channels * (n_channels + 1) // 2).
+    """
     means_dev_layer = model.get_layer("means_dev")
     covs_dev_layer = model.get_layer("covs_dev")
 
     if subject_embeddings is not None:
         nearest_neighbours = get_nearest_neighbours(
             model, subject_embeddings, n_neighbours
         )
@@ -753,124 +500,145 @@
     if learn_means:
         means_dev_mag = get_dev_mag(model, "means")
         if subject_embeddings is not None:
             means_dev_mag = np.mean(
                 tf.gather(means_dev_mag, nearest_neighbours, axis=0),
                 axis=1,
             )
-        means_dev_map = get_dev_map(model, "means", subject_embeddings)
+        means_dev_map = get_dev_map(
+            model=model, map="means", subject_embeddings=subject_embeddings
+        )
         means_dev = means_dev_layer([means_dev_mag, means_dev_map])
     else:
         means_dev = means_dev_layer(1)
 
     if learn_covariances:
         covs_dev_mag = get_dev_mag(model, "covs")
         if subject_embeddings is not None:
             covs_dev_mag = np.mean(
                 tf.gather(covs_dev_mag, nearest_neighbours, axis=0),
                 axis=1,
             )
-        covs_dev_map = get_dev_map(model, "covs", subject_embeddings)
+        covs_dev_map = get_dev_map(
+            model=model, map="covs", subject_embeddings=subject_embeddings
+        )
         covs_dev = covs_dev_layer([covs_dev_mag, covs_dev_map])
     else:
         covs_dev = covs_dev_layer(1)
 
     return means_dev.numpy(), covs_dev.numpy()
 
 
 def get_subject_means_covariances(
     model, learn_means, learn_covariances, subject_embeddings=None, n_neighbours=2
 ):
-    group_means, group_covs = get_group_means_covariances(model)
+    """Get the subject means and covariances.
+
+    Parameters
+    ----------
+    model : osl_dynamics.models.*.Model.model
+        The model. * must be sehmm or sedynemo.
+    learn_means : bool
+        Whether the mean is learnt.
+    learn_covariances : bool
+        Whether the covariances are learnt.
+    subject_embeddings : np.ndarray
+        Input subject embeddings. Shape is (n_subjects, subject_embeddings_dim).
+        If None, then the subject embeddings are retrieved from the model.
+    n_neighbours : int
+        The number of nearest neighbours if subject_embedding is not None.
+
+    Returns
+    -------
+    mu : np.ndarray
+        The subject_means. Shape is (n_subjects, n_modes, n_channels).
+    D : np.ndarray
+        The subject_covariances.
+        Shape is (n_subjects, n_modes, n_channels, n_channels).
+    """
+    group_means = get_observation_model_parameter(model, "group_means")
+    group_covs = get_observation_model_parameter(model, "group_covs")
     means_dev, covs_dev = get_subject_dev(
         model, learn_means, learn_covariances, subject_embeddings, n_neighbours
     )
 
     subject_means_layer = model.get_layer("subject_means")
     subject_covs_layer = model.get_layer("subject_covs")
 
     mu = subject_means_layer([group_means, means_dev])
     D = subject_covs_layer([group_covs, covs_dev])
     return mu.numpy(), D.numpy()
 
 
-def _get_means_mode_embeddings(model):
-    group_means, _ = get_group_means_covariances(model)
-    means_mode_embeddings_layer = model.get_layer("means_mode_embeddings")
-    means_mode_embeddings = means_mode_embeddings_layer(group_means)
-    return means_mode_embeddings.numpy()
-
-
-def _get_covs_mode_embeddings(model):
-    cholesky_bijector = tfb.Chain([tfb.CholeskyOuterProduct(), tfb.FillScaleTriL()])
-    _, group_covs = get_group_means_covariances(model)
-    covs_mode_embeddings_layer = model.get_layer("covs_mode_embeddings")
-    covs_mode_embeddings = covs_mode_embeddings_layer(
-        cholesky_bijector.inverse(group_covs)
-    )
-    return covs_mode_embeddings.numpy()
-
-
-def _get_means_dev_mag_parameters(model):
-    means_dev_mag_inf_alpha_input_layer = model.get_layer(
-        "means_dev_mag_inf_alpha_input"
-    )
-    means_dev_mag_inf_alpha_layer = model.get_layer("means_dev_mag_inf_alpha")
-    means_dev_mag_inf_beta_input_layer = model.get_layer("means_dev_mag_inf_beta_input")
-    means_dev_mag_inf_beta_layer = model.get_layer("means_dev_mag_inf_beta")
-
-    means_dev_mag_inf_alpha_input = means_dev_mag_inf_alpha_input_layer(1)
-    means_dev_mag_inf_alpha = means_dev_mag_inf_alpha_layer(
-        means_dev_mag_inf_alpha_input
-    )
-
-    means_dev_mag_inf_beta_input = means_dev_mag_inf_beta_input_layer(1)
-    means_dev_mag_inf_beta = means_dev_mag_inf_beta_layer(means_dev_mag_inf_beta_input)
-    return means_dev_mag_inf_alpha.numpy(), means_dev_mag_inf_beta.numpy()
-
-
-def _get_covs_dev_mag_parameters(model):
-    covs_dev_mag_inf_alpha_input_layer = model.get_layer("covs_dev_mag_inf_alpha_input")
-    covs_dev_mag_inf_alpha_layer = model.get_layer("covs_dev_mag_inf_alpha")
-    covs_dev_mag_inf_beta_input_layer = model.get_layer("covs_dev_mag_inf_beta_input")
-    covs_dev_mag_inf_beta_layer = model.get_layer("covs_dev_mag_inf_beta")
-
-    covs_dev_mag_inf_alpha_input = covs_dev_mag_inf_alpha_input_layer(1)
-    covs_dev_mag_inf_alpha = covs_dev_mag_inf_alpha_layer(covs_dev_mag_inf_alpha_input)
-
-    covs_dev_mag_inf_beta_input = covs_dev_mag_inf_beta_input_layer(1)
-    covs_dev_mag_inf_beta = covs_dev_mag_inf_beta_layer(covs_dev_mag_inf_beta_input)
-    return covs_dev_mag_inf_alpha.numpy(), covs_dev_mag_inf_beta.numpy()
-
-
 def set_bayesian_kl_scaling(model, n_batches, learn_means, learn_covariances):
+    """Set the scaling of the KL loss of deviation magnitude.
+
+    Parameters
+    ----------
+    model : osl_dynamics.models.*.Model.model
+        The model. * must be sehmm or sedynemo.
+    n_batches : int
+        The number of batches in the dataset.
+    learn_means : bool
+        Whether the mean is learnt.
+    learn_covariances : bool
+        Whether the covariances are learnt.
+    """
     if learn_means:
         means_dev_mag_kl_loss_layer = model.get_layer("means_dev_mag_kl_loss")
         means_dev_mag_kl_loss_layer.n_batches = n_batches
 
     if learn_covariances:
         covs_dev_mag_kl_loss_layer = model.get_layer("covs_dev_mag_kl_loss")
         covs_dev_mag_kl_loss_layer.n_batches = n_batches
 
 
 def get_nearest_neighbours(model, subject_embeddings, n_neighbours):
-    """Get nearest neighbours for each subject in the embedding space."""
+    """Get the indices of the nearest neighours in the subject embedding space.
+
+    Parameters
+    ----------
+    model : osl_dynamics.models.*.Model.model
+        The model. * must be sehmm or sedynemo.
+    subject_embeddings : np.ndarray
+        Input subject embeddings. Shape is (n_subjects, subject_embeddings_dim).
+    n_neighbours : int
+        The number of nearest neighbours.
+
+    Returns
+    -------
+    nearest_neighbours : np.ndarray
+        The indices of the nearest neighbours. Shape is (n_subjects, n_neighbours).
+    """
     model_subject_embeddings = get_subject_embeddings(model)
     distances = np.linalg.norm(
         np.expand_dims(subject_embeddings, axis=1)
         - np.expand_dims(model_subject_embeddings, axis=0),
         axis=-1,
     )
 
     # Sort distances and get indices of nearest neighbours
     sorted_distances = np.argsort(distances, axis=1)
     nearest_neighbours = sorted_distances[:, :n_neighbours]
     return nearest_neighbours
 
 
 def set_dev_mlp_reg_scaling(model, n_batches, learn_means, learn_covariances):
+    """Set the scaling of the MLP regularisation.
+
+    Parameters
+    ----------
+    model : osl_dynamics.models.*.Model.model
+        The model. * must be sehmm or sedynemo.
+    n_batches : int
+        The number of batches in the dataset.
+    learn_means : bool
+        Whether the mean is learnt.
+    learn_covariances : bool
+        Whether the covariances are learnt.
+    """
     if learn_means:
         model.get_layer("means_dev_map_input").n_batches = n_batches
         model.get_layer("means_dev_mag_mod_beta_input").n_batches = n_batches
     if learn_covariances:
         model.get_layer("covs_dev_map_input").n_batches = n_batches
         model.get_layer("covs_dev_mag_mod_beta_input").n_batches = n_batches
```

### Comparing `osl-dynamics-1.2.4/osl_dynamics/models/sehmm.py` & `osl-dynamics-1.2.5/osl_dynamics/models/sehmm.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     InverseCholeskyLayer,
     SampleGammaDistributionLayer,
     StaticKLDivergenceLayer,
     KLLossLayer,
     MultiLayerPerceptronLayer,
 )
 from osl_dynamics.models.hmm import Config as HMMConfig, Model as HMMModel
-from osl_dynamics.models import dynemo_obs, sedynemo_obs
+from osl_dynamics.models import obs_mod
 
 _logger = logging.getLogger("osl-dynamics")
 
 warnings.filterwarnings("ignore", category=NumbaWarning)
 
 
 @dataclass
@@ -419,35 +419,66 @@
             training_data, concatenate=True, subj_id=True
         )
 
         return super().random_state_time_course_initialization(
             training_dataset, n_epochs, n_init, take, **kwargs
         )
 
+    def get_group_means(self):
+        """Get the group level mode means.
+
+        Returns
+        -------
+        means : np.ndarray
+            Group means. Shape is (n_modes, n_channels).
+        """
+        return obs_mod.get_observation_model_parameter(self.model, "group_means")
+
+    def get_means(self):
+        """Overwrite get_means method of the HMM."""
+        return self.get_group_means()
+
     def get_group_covariances(self):
-        """Get the covariances of each state.
+        """Get the group level mode covariances.
 
         Returns
         -------
         covariances : np.ndarray
-            State covariances. Shape is (n_states, n_channels, n_channels).
+            Group covariances. Shape is (n_modes, n_channels, n_channels).
         """
-        return sedynemo_obs.get_group_means_covariances(self.model)[1]
+        return obs_mod.get_observation_model_parameter(self.model, "group_covs")
+
+    def get_covariances(self):
+        """Overwrite get_covariances method of the HMM."""
+        return self.get_group_covariances()
 
     def get_group_means_covariances(self):
-        """Get the means and covariances of each state.
+        """Get the group level mode means and covariances.
+        This is a wrapper for get_group_means and get_group_covariances.
 
         Returns
         -------
-        means : np.ndarary
-            Group level state means.
+        means : np.ndarray
+            Group means. Shape is (n_modes, n_channels).
         covariances : np.ndarray
-            Group level state covariances.
+            Group covariances. Shape is (n_modes, n_channels, n_channels).
         """
-        return sedynemo_obs.get_group_means_covariances(self.model)
+        return self.get_group_means(), self.get_group_covariances()
+
+    def get_means_covariances(self):
+        """Overwrite get_means_covariances method of the HMM."""
+        return self.get_group_means_covariances()
+
+    def get_group_observation_model_parameters(self):
+        """Wrapper for get_group_means_covariances."""
+        return self.get_group_means_covariances()
+
+    def get_observation_model_parameters(self):
+        """Overwrite get_observation_model_parameters method of the HMM."""
+        return self.get_group_observation_model_parameters()
 
     def get_subject_means_covariances(self, subject_embeddings=None, n_neighbours=2):
         """Get the subject means and covariances.
 
         Parameters
         ----------
         subject_embeddings : np.ndarray
@@ -458,15 +489,15 @@
         Returns
         -------
         means : np.ndarray
             Subject means. Shape is (n_subjects, n_states, n_channels).
         covs : np.ndarray
             Subject covariances. Shape is (n_subjects, n_states, n_channels, n_channels).
         """
-        return sedynemo_obs.get_subject_means_covariances(
+        return obs_mod.get_subject_means_covariances(
             self.model,
             self.config.learn_means,
             self.config.learn_covariances,
             subject_embeddings,
             n_neighbours,
         )
 
@@ -475,57 +506,94 @@
 
         Returns
         -------
         subject_embeddings : np.ndarray
             Embedding vectors for subjects.
             Shape is (n_subjects, subject_embedding_dim).
         """
-        return sedynemo_obs.get_subject_embeddings(self.model)
+        return obs_mod.get_subject_embeddings(self.model)
 
     def set_group_means(self, group_means, update_initializer=True):
-        """Set the group means of each state.
+        """Set the group means of each mode.
 
         Parameters
         ----------
         group_means : np.ndarray
-            State covariances.
+            Group level mode means. Shape is (n_modes, n_channels).
         update_initializer : bool
-            Do we want to use the passed means when we re-initialize
-            the model?
+            Do we want to use the passed group means when we re-initialize the model?
         """
-        dynemo_obs.set_means(
-            self.model, group_means, update_initializer, layer_name="group_means"
+        obs_mod.set_observation_model_parameter(
+            self.model,
+            group_means,
+            layer_name="group_means",
+            update_initializer=update_initializer,
         )
 
     def set_group_covariances(self, group_covariances, update_initializer=True):
-        """Set the group covariances of each state.
+        """Set the group covariances of each mode.
 
         Parameters
         ----------
         group_covariances : np.ndarray
-            State covariances.
+            Group level mode covariances. Shape is (n_modes, n_channels, n_channels).
         update_initializer : bool
-            Do we want to use the passed covariances when we re-initialize
+            Do we want to use the passed group covariances when we re-initialize
             the model?
         """
-        dynemo_obs.set_covariances(
+        obs_mod.set_observation_model_parameter(
             self.model,
             group_covariances,
-            update_initializer=update_initializer,
             layer_name="group_covs",
+            update_initializer=update_initializer,
+        )
+
+    def set_group_means_covariances(
+        self, group_means, group_covariances, update_initializer=True
+    ):
+        """This is a wrapper for set_group_means and set_group_covariances."""
+        self.set_group_means(
+            group_means,
+            update_initializer=update_initializer,
+        )
+        self.set_group_covariances(
+            group_covariances,
+            update_initializer=update_initializer,
+        )
+
+    def set_group_observation_model_parameters(
+        self, group_observation_model_parameters, update_initializer=True
+    ):
+        """Wrapper for set_group_means_covariances."""
+        self.set_group_means_covariances(
+            group_observation_model_parameters[0],
+            group_observation_model_parameters[1],
+            update_initializer=update_initializer,
         )
 
     def set_means(self, means, update_initializer=True):
-        """Wrapper of set_group_means."""
+        """Overwrite set_means method of the HMM."""
         self.set_group_means(means, update_initializer)
 
     def set_covariances(self, covariances, update_initializer=True):
-        """Wrapper of set_group_covariances."""
+        """Overwrite set_covariances method of the HMM."""
         self.set_group_covariances(covariances, update_initializer)
 
+    def set_means_covariances(self, means, covariances, update_initializer=True):
+        """Overwrite set_means_covariances method of the HMM."""
+        self.set_group_means_covariances(means, covariances, update_initializer)
+
+    def set_observation_model_parameters(
+        self, observation_model_parameters, update_initializer=True
+    ):
+        """Overwrite set_observation_model_parameters method of the HMM."""
+        self.set_group_observation_model_parameters(
+            observation_model_parameters, update_initializer
+        )
+
     def set_regularizers(self, training_dataset):
         """Set the means and covariances regularizer based on the training data.
 
         A multivariate normal prior is applied to the mean vectors with mu = 0,
         sigma=diag((range / 2)**2). If config.diagonal_covariances is True, a log
         normal prior is applied to the diagonal of the covariances matrices with mu=0,
         sigma=sqrt(log(2 * (range))), otherwise an inverse Wishart prior is applied
@@ -535,20 +603,20 @@
         ----------
         training_dataset : tensorflow.data.Dataset or osl_dynamics.data.Data
             Training dataset.
         """
         training_dataset = self.make_dataset(training_dataset, concatenate=True)
 
         if self.config.learn_means:
-            dynemo_obs.set_means_regularizer(
+            obs_mod.set_means_regularizer(
                 self.model, training_dataset, layer_name="group_means"
             )
 
         if self.config.learn_covariances:
-            dynemo_obs.set_covariances_regularizer(
+            obs_mod.set_covariances_regularizer(
                 self.model,
                 training_dataset,
                 self.config.covariances_epsilon,
                 layer_name="group_covs",
             )
 
     def set_bayesian_kl_scaling(self, training_dataset):
@@ -559,15 +627,15 @@
         training_dataset : tensorflow.data.Dataset or osl_dynamics.data.Data
             Training dataset.
         """
         training_dataset = self.make_dataset(training_dataset, concatenate=True)
         n_batches = dtf.get_n_batches(training_dataset)
         learn_means = self.config.learn_means
         learn_covariances = self.config.learn_covariances
-        sedynemo_obs.set_bayesian_kl_scaling(
+        obs_mod.set_bayesian_kl_scaling(
             self.model, n_batches, learn_means, learn_covariances
         )
 
     def set_dev_mlp_reg_scaling(self, training_dataset):
         """Set the correct scaling for the deviation MLP regularization.
 
         Parameters
@@ -575,15 +643,15 @@
         training_dataset : tensorflow.data.Dataset or osl_dynamics.data.Data
             Training dataset.
         """
         training_dataset = self.make_dataset(training_dataset, concatenate=True)
         n_batches = dtf.get_n_batches(training_dataset)
         learn_means = self.config.learn_means
         learn_covariances = self.config.learn_covariances
-        sedynemo_obs.set_dev_mlp_reg_scaling(
+        obs_mod.set_dev_mlp_reg_scaling(
             self.model, n_batches, learn_means, learn_covariances
         )
 
     def free_energy(self, dataset):
         """Get the variational free energy.
 
         This calculates:
@@ -1086,8 +1154,8 @@
     # Total KL loss
     # Layer definitions
     kl_loss_layer = KLLossLayer(do_annealing=True, name="kl_loss")
 
     # Data flow
     kl_loss = kl_loss_layer([means_dev_mag_kl_loss, covs_dev_mag_kl_loss])
 
-    return tf.keras.Model(inputs=inputs, outputs=[ll_loss, kl_loss], name="SE-HMM-Obs")
+    return tf.keras.Model(inputs=inputs, outputs=[ll_loss, kl_loss], name="SE-HMM")
```

### Comparing `osl-dynamics-1.2.4/osl_dynamics/simulation/__init__.py` & `osl-dynamics-1.2.5/osl_dynamics/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/simulation/base.py` & `osl-dynamics-1.2.5/osl_dynamics/simulation/base.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/simulation/hmm.py` & `osl-dynamics-1.2.5/osl_dynamics/simulation/hmm.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/simulation/hsmm.py` & `osl-dynamics-1.2.5/osl_dynamics/simulation/hsmm.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
 
             rand = random_sample()
             current_state = np.argmin(
                 cumsum_off_diagonal_trans_prob[current_state] < rand
             )
             current_position += state_lifetime
 
-        return alpha
+        return alpha.astype(int)
 
 
 class HSMM_MVN(Simulation):
     """Hidden Semi-Markov Model Simulation.
 
     We sample the state using a transition probability matrix with zero
     probability for self-transitions. The lifetime of each state is sampled
```

### Comparing `osl-dynamics-1.2.4/osl_dynamics/simulation/mar.py` & `osl-dynamics-1.2.5/osl_dynamics/simulation/mar.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/simulation/mvn.py` & `osl-dynamics-1.2.5/osl_dynamics/simulation/mvn.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/simulation/sin.py` & `osl-dynamics-1.2.5/osl_dynamics/simulation/sin.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/simulation/sm.py` & `osl-dynamics-1.2.5/osl_dynamics/simulation/sm.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/utils/decorators.py` & `osl-dynamics-1.2.5/osl_dynamics/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/utils/misc.py` & `osl-dynamics-1.2.5/osl_dynamics/utils/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import inspect
 import logging
 import pickle
 import sys
 from copy import copy
 from pathlib import Path
+from contextlib import contextmanager
 
 import numpy as np
 import yaml
 from yaml.constructor import ConstructorError
 
 _logger = logging.getLogger("osl-dynamics")
 
@@ -498,7 +499,17 @@
     _logger.info(f"Loading {filename}")
     if ext == ".pkl":
         array = pickle.load(open(filename, "rb"))
     else:
         array = np.load(filename)
 
     return array
+
+
+@contextmanager
+def set_logging_level(logger, level):
+    current_level = logger.getEffectiveLevel()
+    try:
+        logger.setLevel(level)
+        yield
+    finally:
+        logger.setLevel(current_level)
```

### Comparing `osl-dynamics-1.2.4/osl_dynamics/utils/model.py` & `osl-dynamics-1.2.5/osl_dynamics/utils/model.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/utils/parcellation.py` & `osl-dynamics-1.2.5/osl_dynamics/utils/parcellation.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/utils/plotting.py` & `osl-dynamics-1.2.5/osl_dynamics/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics/utils/topoplots.py` & `osl-dynamics-1.2.5/osl_dynamics/utils/topoplots.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.4/osl_dynamics.egg-info/PKG-INFO` & `osl-dynamics-1.2.5/osl_dynamics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osl-dynamics
-Version: 1.2.4
+Version: 1.2.5
 Summary: Models for infering dynamics in neuroimaging data
 Home-page: https://github.com/OHBA-analysis/osl-dynamics
 License: MIT
 Project-URL: Documentation, https://osl-dynamics.readthedocs.io/en/latest/
 Description-Content-Type: text/x-rst; charset=UTF-8
 
 ============
```

### Comparing `osl-dynamics-1.2.4/osl_dynamics.egg-info/SOURCES.txt` & `osl-dynamics-1.2.5/osl_dynamics.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 osl_dynamics/config_api/__init__.py
 osl_dynamics/config_api/pipeline.py
 osl_dynamics/config_api/wrappers.py
 osl_dynamics/data/__init__.py
 osl_dynamics/data/base.py
 osl_dynamics/data/processing.py
 osl_dynamics/data/rw.py
-osl_dynamics/data/spm.py
 osl_dynamics/data/task.py
 osl_dynamics/data/tf.py
 osl_dynamics/files/__init__.py
 osl_dynamics/files/functions.py
 osl_dynamics/files/mask/MNI152_T1_8mm_brain.nii.gz
 osl_dynamics/files/mask/ParcellationPilot.L.inflated.32k_fs_LR.surf.gii
 osl_dynamics/files/mask/ParcellationPilot.L.midthickness.32k_fs_LR.surf.gii
@@ -144,24 +143,22 @@
 osl_dynamics/inference/layers.py
 osl_dynamics/inference/metrics.py
 osl_dynamics/inference/modes.py
 osl_dynamics/inference/regularizers.py
 osl_dynamics/inference/tf_ops.py
 osl_dynamics/models/__init__.py
 osl_dynamics/models/dynemo.py
-osl_dynamics/models/dynemo_obs.py
 osl_dynamics/models/hmm.py
 osl_dynamics/models/inf_mod_base.py
 osl_dynamics/models/mage.py
 osl_dynamics/models/mdynemo.py
-osl_dynamics/models/mdynemo_obs.py
 osl_dynamics/models/mod_base.py
+osl_dynamics/models/obs_mod.py
 osl_dynamics/models/sage.py
 osl_dynamics/models/sedynemo.py
-osl_dynamics/models/sedynemo_obs.py
 osl_dynamics/models/sehmm.py
 osl_dynamics/models/state_dynemo.py
 osl_dynamics/simulation/__init__.py
 osl_dynamics/simulation/base.py
 osl_dynamics/simulation/hmm.py
 osl_dynamics/simulation/hsmm.py
 osl_dynamics/simulation/mar.py
```

### Comparing `osl-dynamics-1.2.4/setup.cfg` & `osl-dynamics-1.2.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = osl-dynamics
-version = 1.2.4
+version = 1.2.5
 description = Models for infering dynamics in neuroimaging data
 license = MIT
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 url = https://github.com/OHBA-analysis/osl-dynamics
 project_urls = 
 	Documentation = https://osl-dynamics.readthedocs.io/en/latest/
```

