# Comparing `tmp/spec2nii-0.6.8.tar.gz` & `tmp/spec2nii-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spec2nii-0.6.8.tar", last modified: Wed Mar 22 16:17:43 2023, max compression
+gzip compressed data, was "spec2nii-0.6.9.tar", last modified: Fri Jul  7 14:10:42 2023, max compression
```

## Comparing `spec2nii-0.6.8.tar` & `spec2nii-0.6.9.tar`

### file list

```diff
@@ -1,79 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:17:43.077588 spec2nii-0.6.8/
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-03-22 16:17:33.000000 spec2nii-0.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-22 16:17:33.000000 spec2nii-0.6.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11272 2023-03-22 16:17:43.077588 spec2nii-0.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10559 2023-03-22 16:17:33.000000 spec2nii-0.6.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-22 16:17:33.000000 spec2nii-0.6.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-03-22 16:17:33.000000 spec2nii-0.6.8/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-03-22 16:17:43.077588 spec2nii-0.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-03-22 16:17:33.000000 spec2nii-0.6.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:17:43.081588 spec2nii-0.6.8/spec2nii/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:17:43.073588 spec2nii-0.6.8/spec2nii/GE/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 16:17:33.000000 spec2nii-0.6.8/spec2nii/GE/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   161091 2023-03-22 16:17:33.000000 spec2nii-0.6.8/spec2nii/GE/ge_hdr_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    13720 2023-03-22 16:17:33.000000 spec2nii-0.6.8/spec2nii/GE/ge_pfile.py
--rw-r--r--   0 runner    (1001) docker     (123)    47723 2023-03-22 16:17:33.000000 spec2nii-0.6.8/spec2nii/GE/ge_read_pfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:17:43.073588 spec2nii-0.6.8/spec2nii/GSL/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 16:17:33.000000 spec2nii-0.6.8/spec2nii/GSL/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-03-22 16:17:33.000000 spec2nii-0.6.8/spec2nii/GSL/gslfunctions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:17:43.073588 spec2nii-0.6.8/spec2nii/Philips/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 16:17:33.000000 spec2nii-0.6.8/spec2nii/Philips/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14540 2023-03-22 16:17:33.000000 spec2nii-0.6.8/spec2nii/Philips/philips.py
--rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-03-22 16:17:33.000000 spec2nii-0.6.8/spec2nii/Philips/philips_data_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    23678 2023-03-22 16:17:33.000000 spec2nii-0.6.8/spec2nii/Philips/philips_dcm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:17:43.073588 spec2nii-0.6.8/spec2nii/Siemens/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 16:17:33.000000 spec2nii-0.6.8/spec2nii/Siemens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26487 2023-03-22 16:17:33.000000 spec2nii-0.6.8/spec2nii/Siemens/dicomfunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-03-22 16:17:33.000000 spec2nii-0.6.8/spec2nii/Siemens/rda.py
--rw-r--r--   0 runner    (1001) docker     (123)    11492 2023-03-22 16:17:33.000000 spec2nii-0.6.8/spec2nii/Siemens/twix_special_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    46754 2023-03-22 16:17:33.000000 spec2nii-0.6.8/spec2nii/Siemens/twixfunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-22 16:17:33.000000 spec2nii-0.6.8/spec2nii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-22 16:17:43.081588 spec2nii-0.6.8/spec2nii/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-03-22 16:17:33.000000 spec2nii-0.6.8/spec2nii/anonymise.py
--rw-r--r--   0 runner    (1001) docker     (123)    12076 2023-03-22 16:17:33.000000 spec2nii-0.6.8/spec2nii/bruker.py
--rw-r--r--   0 runner    (1001) docker     (123)    18669 2023-03-22 16:17:33.000000 spec2nii-0.6.8/spec2nii/bruker_fid_override.json
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-03-22 16:17:33.000000 spec2nii-0.6.8/spec2nii/bruker_properties.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:17:43.073588 spec2nii-0.6.8/spec2nii/dcm2niiOrientation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 16:17:33.000000 spec2nii-0.6.8/spec2nii/dcm2niiOrientation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-03-22 16:17:33.000000 spec2nii-0.6.8/spec2nii/dcm2niiOrientation/orientationFuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23333 2023-03-22 16:17:33.000000 spec2nii-0.6.8/spec2nii/fileiobase.py
--rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-03-22 16:17:33.000000 spec2nii-0.6.8/spec2nii/jmrui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-03-22 16:17:33.000000 spec2nii-0.6.8/spec2nii/nifti_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-03-22 16:17:33.000000 spec2nii-0.6.8/spec2nii/other.py
--rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-03-22 16:17:33.000000 spec2nii-0.6.8/spec2nii/other_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)    31584 2023-03-22 16:17:33.000000 spec2nii-0.6.8/spec2nii/spec2nii.py
--rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-03-22 16:17:33.000000 spec2nii-0.6.8/spec2nii/uih.py
--rw-r--r--   0 runner    (1001) docker     (123)    64346 2023-03-22 16:17:33.000000 spec2nii-0.6.8/spec2nii/varian.py
--rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-03-22 16:17:33.000000 spec2nii-0.6.8/spec2nii/varian_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:17:43.073588 spec2nii-0.6.8/spec2nii.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11272 2023-03-22 16:17:43.000000 spec2nii-0.6.8/spec2nii.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-03-22 16:17:43.000000 spec2nii-0.6.8/spec2nii.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 16:17:43.000000 spec2nii-0.6.8/spec2nii.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-22 16:17:43.000000 spec2nii-0.6.8/spec2nii.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-22 16:17:43.000000 spec2nii-0.6.8/spec2nii.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-22 16:17:43.000000 spec2nii-0.6.8/spec2nii.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:17:43.077588 spec2nii-0.6.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-03-22 16:17:33.000000 spec2nii-0.6.8/tests/test_anon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-03-22 16:17:33.000000 spec2nii-0.6.8/tests/test_auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-03-22 16:17:33.000000 spec2nii-0.6.8/tests/test_bruker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-03-22 16:17:33.000000 spec2nii-0.6.8/tests/test_ge_pfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-03-22 16:17:33.000000 spec2nii-0.6.8/tests/test_ge_pfile_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-03-22 16:17:33.000000 spec2nii-0.6.8/tests/test_jmrui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-03-22 16:17:33.000000 spec2nii-0.6.8/tests/test_nifti_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-03-22 16:17:33.000000 spec2nii-0.6.8/tests/test_other.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-03-22 16:17:33.000000 spec2nii-0.6.8/tests/test_other_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-03-22 16:17:33.000000 spec2nii-0.6.8/tests/test_philips_data_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-03-22 16:17:33.000000 spec2nii-0.6.8/tests/test_philips_dicom.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-03-22 16:17:33.000000 spec2nii-0.6.8/tests/test_philips_dicom_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-03-22 16:17:33.000000 spec2nii-0.6.8/tests/test_philips_sdat_spar.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-03-22 16:17:33.000000 spec2nii-0.6.8/tests/test_philips_sdat_spar_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-03-22 16:17:33.000000 spec2nii-0.6.8/tests/test_siemens_dicom.py
--rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-03-22 16:17:33.000000 spec2nii-0.6.8/tests/test_siemens_mrsi_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-03-22 16:17:33.000000 spec2nii-0.6.8/tests/test_siemens_rda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-03-22 16:17:33.000000 spec2nii-0.6.8/tests/test_siemens_special_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-03-22 16:17:33.000000 spec2nii-0.6.8/tests/test_siemens_svs_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-03-22 16:17:33.000000 spec2nii-0.6.8/tests/test_twix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-03-22 16:17:33.000000 spec2nii-0.6.8/tests/test_uih.py
--rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-03-22 16:17:33.000000 spec2nii-0.6.8/tests/test_uih_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-03-22 16:17:33.000000 spec2nii-0.6.8/tests/test_varian.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-03-22 16:17:33.000000 spec2nii-0.6.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:10:42.384826 spec2nii-0.6.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-07-07 14:10:30.000000 spec2nii-0.6.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-07-07 14:10:30.000000 spec2nii-0.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-07 14:10:30.000000 spec2nii-0.6.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11272 2023-07-07 14:10:42.384826 spec2nii-0.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10559 2023-07-07 14:10:30.000000 spec2nii-0.6.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-07 14:10:30.000000 spec2nii-0.6.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-07 14:10:30.000000 spec2nii-0.6.9/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-07 14:10:42.384826 spec2nii-0.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-07 14:10:30.000000 spec2nii-0.6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:10:42.384826 spec2nii-0.6.9/spec2nii/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:10:42.376826 spec2nii-0.6.9/spec2nii/GE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/GE/VESPA_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/GE/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   161091 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/GE/ge_hdr_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15740 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/GE/ge_pfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47855 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/GE/ge_read_pfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:10:42.376826 spec2nii-0.6.9/spec2nii/GSL/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/GSL/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/GSL/gslfunctions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:10:42.376826 spec2nii-0.6.9/spec2nii/Philips/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/Philips/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14530 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/Philips/philips.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12028 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/Philips/philips_data_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23678 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/Philips/philips_dcm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:10:42.376826 spec2nii-0.6.9/spec2nii/Siemens/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/Siemens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26487 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/Siemens/dicomfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/Siemens/rda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11472 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/Siemens/twix_special_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46734 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/Siemens/twixfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-07 14:10:42.384826 spec2nii-0.6.9/spec2nii/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/anonymise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12076 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/bruker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18669 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/bruker_fid_override.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/bruker_properties.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:10:42.380826 spec2nii-0.6.9/spec2nii/dcm2niiOrientation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/dcm2niiOrientation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/dcm2niiOrientation/orientationFuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23331 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/fileiobase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/jmrui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/nifti_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/other.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/other_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31584 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/spec2nii.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/uih.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64350 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/varian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-07-07 14:10:30.000000 spec2nii-0.6.9/spec2nii/varian_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:10:42.376826 spec2nii-0.6.9/spec2nii.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11272 2023-07-07 14:10:42.000000 spec2nii-0.6.9/spec2nii.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-07-07 14:10:42.000000 spec2nii-0.6.9/spec2nii.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 14:10:42.000000 spec2nii-0.6.9/spec2nii.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-07 14:10:42.000000 spec2nii-0.6.9/spec2nii.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-07 14:10:42.000000 spec2nii-0.6.9/spec2nii.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-07 14:10:42.000000 spec2nii-0.6.9/spec2nii.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:10:42.384826 spec2nii-0.6.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/io_for_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_anon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_bruker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_ge_pfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_ge_pfile_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_jmrui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_nifti_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_other.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_other_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_philips_data_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_philips_dicom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_philips_dicom_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_philips_sdat_spar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_philips_sdat_spar_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_siemens_dicom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_siemens_mrsi_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_siemens_rda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_siemens_special_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_siemens_svs_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_twix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_uih.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_uih_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-07 14:10:30.000000 spec2nii-0.6.9/tests/test_varian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-07-07 14:10:30.000000 spec2nii-0.6.9/versioneer.py
```

### Comparing `spec2nii-0.6.8/LICENSE` & `spec2nii-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.8/PKG-INFO` & `spec2nii-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spec2nii
-Version: 0.6.8
+Version: 0.6.9
 Summary: Multi-format in vivo MR spectroscopy conversion to NIFTI
 Home-page: https://github.com/wtclarke/spec2nii
 Author: Will Clarke
 Author-email: william.clarke@ndcn.ox.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `spec2nii-0.6.8/README.md` & `spec2nii-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.8/setup.cfg` & `spec2nii-0.6.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.8/setup.py` & `spec2nii-0.6.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 
-from setuptools import setup
+from setuptools import setup, find_packages
 import versioneer
 import yaml
 
 with open("requirements.yml", "r") as stream:
     try:
         requirements = yaml.safe_load(stream)
         install_requires = requirements['dependencies']
@@ -19,29 +19,25 @@
       cmdclass=versioneer.get_cmdclass(),
       description='Multi-format in vivo MR spectroscopy conversion to NIFTI',
       author='Will Clarke',
       author_email='william.clarke@ndcn.ox.ac.uk',
       url='https://github.com/wtclarke/spec2nii',
       long_description=long_description,
       long_description_content_type="text/markdown",
-      packages=['spec2nii',
-                'spec2nii.Siemens',
-                'spec2nii.GSL',
-                'spec2nii.dcm2niiOrientation',
-                'spec2nii.Philips',
-                'spec2nii.GE'],
+      packages=find_packages(),
       install_requires=install_requires,
       classifiers=[
           "Programming Language :: Python :: 3",
           "Programming Language :: Python :: 3.7",
           "Programming Language :: Python :: 3.8",
           "Programming Language :: Python :: 3.9",
           "Programming Language :: Python :: 3.10",
           "Programming Language :: Python :: 3.11",
           "License :: OSI Approved :: BSD License",
           "Operating System :: OS Independent"],
       python_requires='>=3.7',
       entry_points={"console_scripts": [
           "spec2nii = spec2nii.spec2nii:main"]},
       package_data={'spec2nii': ['bruker_properties.json',
-                                 'bruker_fid_override.json']}
+                                 'bruker_fid_override.json'],
+                    'spec2nii.GE': ['VESPA_LICENSE']}
       )
```

### Comparing `spec2nii-0.6.8/spec2nii/GE/ge_hdr_fields.py` & `spec2nii-0.6.9/spec2nii/GE/ge_hdr_fields.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.8/spec2nii/GE/ge_pfile.py` & `spec2nii-0.6.9/spec2nii/GE/ge_pfile.py`

 * *Files 20% similar despite different names*

```diff
@@ -91,14 +91,16 @@
     '''
     psd = pfile.hdr.rhi_psdname.decode('utf-8').lower()
 
     if psd in ('probe-p', 'probe-s'):
         data, meta, dwelltime, fname_suffix = _process_probe_p(pfile)
     elif psd in ('oslaser', 'slaser_cni'):
         data, meta, dwelltime, fname_suffix = _process_oslaser(pfile)
+    elif psd in ('slaser'):
+        data, meta, dwelltime, fname_suffix = _process_slaser(pfile)
     elif psd == 'gaba':
         data, meta, dwelltime, fname_suffix = _process_gaba(pfile)
     elif 'jpress_ac' in psd:  # Bergen patch
         data, meta, dwelltime, fname_suffix = _process_gaba(pfile)
     elif psd == 'jpress':
         data, meta, dwelltime, fname_suffix = _process_gaba(pfile)
     else:
@@ -128,14 +130,20 @@
     water = np.transpose(water, [0, 1, 2, 5, 4, 3])     # swap to (1,1,1,npts,ncoil,navg)
 
     dwelltime = 1 / pfile.hdr.rhr_spectral_width
 
     meta = _populate_metadata(pfile, water_suppressed=True)
     meta_ref = _populate_metadata(pfile, water_suppressed=False)
 
+    meta.set_dim_info(0, 'DIM_COIL')
+    meta.set_dim_info(1, 'DIM_DYN')
+
+    meta_ref.set_dim_info(0, 'DIM_COIL')
+    meta_ref.set_dim_info(1, 'DIM_DYN')
+
     return [metab, water], [meta, meta_ref], dwelltime, ['', '_ref']
 
 
 def _process_oslaser(pfile):
     '''Extract metabolite and reference data from a oslaser format pfile
 
     I think this is like the CMRR sLASER sequence with 2 ecc and 2 water scaling
@@ -150,31 +158,54 @@
     metab = pfile.map.raw_suppressed
     metab = np.transpose(metab, [0, 1, 2, 5, 4, 3])     # swap to (1,1,1,npts,ncoil,navg)
     water = np.transpose(water, [0, 1, 2, 5, 4, 3])     # swap to (1,1,1,npts,ncoil,navg)
 
     data = []
     meta = []
     fname_suffix = []
-
     data.append(water[:, :, :, :, :, [0, 1, 4, 5]])
-    meta.append(_populate_metadata(pfile, water_suppressed=False))
+    meta.append(_populate_metadata(pfile, water_suppressed=False, data_dimensions=data[0].ndim))
     fname_suffix.append('_quant')
     data.append(water[:, :, :, :, :, [2, 3, 6, 7]])
-    meta.append(_populate_metadata(pfile, water_suppressed=False))
+    meta.append(_populate_metadata(pfile, water_suppressed=False, data_dimensions=data[1].ndim))
     fname_suffix.append('_ecc')
 
     data.append(metab)
-    meta.append(_populate_metadata(pfile, water_suppressed=True))
+    meta.append(_populate_metadata(pfile, water_suppressed=True, data_dimensions=metab.ndim))
     fname_suffix.append('')
 
     dwelltime = 1 / pfile.hdr.rhr_spectral_width
 
     return data, meta, dwelltime, fname_suffix
 
 
+def _process_slaser(pfile):
+    '''Extract metabolite and reference data from a slaser format pfile
+
+    This seems to be like a standard probe-p. Maybe slaser is the canonical vendor implementation.
+
+    :param Pfile pfile: Pfile object
+    :return: List numpy data arrays
+    :return: List of file name suffixes
+    '''
+
+    metab = pfile.map.raw_suppressed                    # typically (1,1,1,navg,ncoil,npts)
+    metab = np.transpose(metab, [0, 1, 2, 5, 4, 3])     # swap to (1,1,1,npts,ncoil,navg)
+
+    water = pfile.map.raw_unsuppressed                  # typically (1,1,1,navg,ncoil,npts)
+    water = np.transpose(water, [0, 1, 2, 5, 4, 3])     # swap to (1,1,1,npts,ncoil,navg)
+
+    dwelltime = 1 / pfile.hdr.rhr_spectral_width
+
+    meta = _populate_metadata(pfile, water_suppressed=True, data_dimensions=metab.ndim)
+    meta_ref = _populate_metadata(pfile, water_suppressed=False, data_dimensions=water.ndim)
+
+    return [metab, water], [meta, meta_ref], dwelltime, ['', '_ref']
+
+
 def _process_gaba(pfile):
     '''Extract metabolite and reference data from a gaba (MPRESS) format pfile
 
     :param Pfile pfile: Pfile object
     :return: List numpy data arrays
     :return: List of file name suffixes
     '''
@@ -227,14 +258,16 @@
 
     data = fft_and_shift(data, 0)
     data = fft_and_shift(data, 1)
     data = fft_and_shift(data, 2)
 
     dwelltime = 1 / pfile.hdr.rhr_spectral_width
     meta = _populate_metadata(pfile)
+    meta.set_dim_info(0, 'DIM_COIL')
+
     orientation = NIFTIOrient(_calculate_affine_mrsi(pfile))
 
     return [gen_nifti_mrs_hdr_ext(data, dwelltime, meta, orientation.Q44, no_conj=True), ], ['', ]
 
 
 def _calculate_affine_mrsi(pfile):
     '''Calculate the 4x4 affine matrix for mrsi'''
@@ -273,16 +306,30 @@
 
     affine[:3, 3] = voi_position
     affine[3, 3] = 1.0
 
     return affine
 
 
-def _populate_metadata(pfile, water_suppressed=True):
-    ''' Populate a nifti-mrs header extension with the requisite information'''
+def _populate_metadata(pfile, water_suppressed=True, data_dimensions=None):
+    """Populate a nifti-mrs header extension with metadata from the pfile
+
+    If (up to 7) data_dimensions are specified then default dimension tags
+    (coil, dyn, indirect) will be included. Otherwise manually specify
+    outside this function.
+
+    :param pfile: pfile object
+    :type pfile: pfile map object
+    :param water_suppressed: Set water suppression header field, defaults to True
+    :type water_suppressed: bool, optional
+    :param data_dimensions: If set to 5,6, or 7 will inlcude default dim tags for those diemnsions, defaults to None
+    :type data_dimensions: int, optional
+    :return: Header extension object
+    :rtype: nifti_mrs.hdr_ext
+    """
     hdr = pfile.hdr
     spec_frequency = float(pfile.hdr.rhr_rh_ps_mps_freq) / 1e7
 
     #  Use the mps freq and field strength to determine gamma and thus isotope
     try:
         gamma = (hdr.rhr_rh_ps_mps_freq * 1e-7) / (hdr.rhe_magstrength / 10000.0)
         if abs(gamma - 42.57) < 0.3:
@@ -300,15 +347,16 @@
         # E.g. the BIG GABA data.
         print('Warning: Magnetic field value set to zero, setting nucleus to 1H as default. '
               'Use the --override_nucleus option to specify a different nuclide.')
         nucleus = "1H"
 
     meta = Hdr_Ext(
         spec_frequency,
-        nucleus)
+        nucleus,
+        dimensions=data_dimensions)
 
     # Standard defined metadata
     # # 5.1 MRS specific Tags
     # 'EchoTime'
     meta.set_standard_def('EchoTime', float(hdr.rhi_te) / 1E6)
     # 'RepetitionTime'
     meta.set_standard_def('RepetitionTime', float(hdr.rhi_tr) / 1E6)
```

### Comparing `spec2nii-0.6.8/spec2nii/GE/ge_read_pfile.py` & `spec2nii-0.6.9/spec2nii/GE/ge_read_pfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,15 @@
         if self.hdr is None:
             return None
 
         psd = self.hdr.rhi_psdname.decode('utf-8').lower()
 
         if psd in ('probe-p', 'probe-s'):
             mapper = PfileMapper
-        elif psd in ('oslaser', 'slaser_cni'):
+        elif psd in ('oslaser', 'slaser_cni', 'slaser'):
             mapper = PfileMapperSlaser
         elif psd == 'presscsi':
             mapper = PfileMapper
         elif psd == 'fidcsi':
             # bjs - added for Pom's fidcsi 13C data
             mapper = PfileMapper
         elif psd == 'ia/stable/fidcsi':
@@ -204,14 +204,17 @@
             mapper = PfileMapperProbeSL
         elif 'jpress_ac' in psd:
             # ARC : Added for Bergen jpress patch
             mapper = PfileMapperGaba
         elif psd == 'jpress':
             # wtc - Added for HURCULES data.
             mapper = PfileMapperGaba
+        elif psd == 'fidall':
+            # WTC - added for JG's Hyperpolarised 13C data
+            mapper = PfileMapper
         else:
             raise UnknownPfile("No Pfile mapper for pulse sequence = %s" % psd)
 
         return mapper
 
     def read_header(self):
```

### Comparing `spec2nii-0.6.8/spec2nii/GSL/gslfunctions.py` & `spec2nii-0.6.9/spec2nii/GSL/gslfunctions.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.8/spec2nii/Philips/philips.py` & `spec2nii-0.6.9/spec2nii/Philips/philips.py`

 * *Files 0% similar despite different names*

```diff
@@ -321,15 +321,15 @@
     data_short_te = data[:, :, :, :, :32]
     data_edited = data[:, :, :, :, 32:]
 
     if data_edited.shape[-1] % 4 != 0:                                                      # Handle Incomplete Data
         old_num_avgs = data_edited.shape[-1]                                                # Old Number of Averages
         new_num_avgs = (data_edited.shape[-1] // 4) * 4                                     # Complete Sets of 4
         data_edited = data_edited[..., :new_num_avgs]                                       # Only Keep Complete Sets
-        print('Correcting - Incomplete Averages {} --> {}    Corrected**'.format(old_num_avgs, new_num_avgs))
+        print(f'Correcting - Incomplete Averages {old_num_avgs} --> {new_num_avgs}    Corrected**')
 
     data_edited = data_edited.T.reshape((-1, 4, data.shape[3], 1, 1, 1)).T
 
     meta_short_te = meta.copy()
     meta_short_te.set_standard_def("WaterSuppressed", True)
     meta_short_te.set_standard_def("EchoTime", 0.035)
```

### Comparing `spec2nii-0.6.8/spec2nii/Philips/philips_data_list.py` & `spec2nii-0.6.9/spec2nii/Philips/philips_data_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
                                   f' Dimensions are {kept_ind} with shape {out_data.shape[1:]}.'
                                   ' NIFTI-MRS can only handle three dynamic dimensions. Unsure how to proceed.')
 
         # Special cases
         if data_type == 'STD_0'\
                 and (special_case == 'hyper' or 'hyper' in meta['ProtocolName'].lower()):
             out_hyper, meta_hyper = _special_case_hyper(out_data, meta)
-            # Handle the main acqusition of the HYPER (short TE + editing) sequence
+            # Handle the main acquisition of the HYPER (short TE + editing) sequence
 
             # Insert spatial dimensions
             out_shortte = out_hyper[0].reshape((1, 1, 1) + out_hyper[0].shape)
             out_edited = out_hyper[1].reshape((1, 1, 1) + out_hyper[1].shape)
 
             # Apply conjugate
             out_shortte = out_shortte.conj()
@@ -116,14 +116,18 @@
             continue
 
         elif data_type == 'STD_1'\
                 and (special_case == 'hyper' or 'hyper' in meta['ProtocolName'].lower()):
             # Handle the water ref acqusition of the HYPER sequence
 
             meta.set_dim_info(
+                0,
+                'DIM_COIL')
+
+            meta.set_dim_info(
                 1,
                 'DIM_USER_0',
                 info='HYPER water reference')
 
             name = 'hyper_water_ref'
 
         else:
@@ -274,33 +278,44 @@
     data_short_te = data[:, :, :32]
     data_edited = data[:, :, 32:]
 
     if data_edited.shape[-1] % 4 != 0:                                                      # Handle Incomplete Data
         old_num_avgs = data_edited.shape[-1]                                                # Old Number of Averages
         new_num_avgs = (data_edited.shape[-1] // 4) * 4                                     # Complete Sets of 4
         data_edited = data_edited[..., :new_num_avgs]                                       # Only Keep Complete Sets
-        print('Correcting - Incomplete Averages {} --> {}    Corrected**'.format(old_num_avgs, new_num_avgs))
+        print(f'Correcting - Incomplete Averages {old_num_avgs} --> {new_num_avgs}    Corrected**')
 
     data_edited = data_edited.T.reshape((-1, 4, data.shape[1], data.shape[0])).T
 
     meta_short_te = meta.copy()
     meta_edited = meta.copy()
 
+    meta_short_te.set_dim_info(
+        0,
+        'DIM_COIL')
+    meta_short_te.set_dim_info(
+        1,
+        'DIM_DYN')
+
     edit_pulse_1   = 1.9
     edit_pulse_2   = 4.58
     edit_pulse_off = 4.18
     dim_info       = "HERCULES j-difference editing, four conditions"
     dim_header     = {"EditCondition": ["A", "B", "C", "D"]}
     edit_pulse_val = {
         "A": {"PulseOffset": [edit_pulse_1, edit_pulse_2], "PulseDuration": 0.02},
         "B": {"PulseOffset": [edit_pulse_off, edit_pulse_2], "PulseDuration": 0.02},
         "C": {"PulseOffset": edit_pulse_1, "PulseDuration": 0.02},
         "D": {"PulseOffset": edit_pulse_off, "PulseDuration": 0.02}}
 
     meta_edited.set_dim_info(
+        0,
+        'DIM_COIL')
+
+    meta_edited.set_dim_info(
         1,
         'DIM_EDIT',
         dim_info,
         dim_header)
 
     meta_edited.set_dim_info(2, 'DIM_DYN')
     meta_edited.set_standard_def("EditPulse", edit_pulse_val)
```

### Comparing `spec2nii-0.6.8/spec2nii/Philips/philips_dcm.py` & `spec2nii-0.6.9/spec2nii/Philips/philips_dcm.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.8/spec2nii/Siemens/dicomfunctions.py` & `spec2nii-0.6.9/spec2nii/Siemens/dicomfunctions.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.8/spec2nii/Siemens/rda.py` & `spec2nii-0.6.9/spec2nii/Siemens/rda.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.8/spec2nii/Siemens/twix_special_case.py` & `spec2nii-0.6.9/spec2nii/Siemens/twix_special_case.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,25 +40,25 @@
         3 = HERCULES  (This is what should get chosen for HBCD)
         4 = HERMES GABA LAC
 
     Author : Aaron Gudmundson, Johns Hopkins University, 2023
     Contact: agudmun2@jhmi.edu
     """
 
-    print('{:3d} {:<20} - Starting   -'.format(subseq, subseq_name), end='\r')
+    print(f'{subseq:3d} {subseq_name:<20} - Starting   -', end='\r')
 
     short_TE        = twixObj['hdr']['Phoenix'][('sWipMemBlock', 'alFree', '6')] / 1E6          # Short TE's Echo Time
     pulse_length    = twixObj['hdr']['Phoenix'][('sWipMemBlock', 'alFree', '12')] / 1E6         # Pulse Duration
 
     edit_cases      = 4                                                                         # 4 Editing Conditions
     edit_pulse_1    = twixObj['hdr']['Phoenix'][('sWipMemBlock', 'adFree', '8')]                # 4.58 ppm
     edit_pulse_2    = twixObj['hdr']['Phoenix'][('sWipMemBlock', 'adFree', '9')]                # 1.90 ppm
     edit_pulse_4    = twixObj['hdr']['Phoenix'][('sWipMemBlock', 'adFree', '11')]               # 4.18 ppm
 
-    dim_info        = 'Hyper - {}'.format(subseq_name)                                          # Subscan Name
+    dim_info        = f'Hyper - {subseq_name}'                                                  # Subscan Name
 
     if subseq == 0:                                                                             # Short TE Water Ref
         reord_data = reord_data[:, :, 33::66]                                                   # Short TE Water Refs
         meta_obj.set_standard_def('EchoTime', short_TE)                                         # Echo Time
         meta_obj.set_standard_def('WaterSuppressed', False)                                     # Water Suppression
 
     elif subseq == 1:                                                                           # Long  TE Water Ref
@@ -80,18 +80,18 @@
 
         # Handle Incomplete
         if reord_data.shape[-1] % 4 != 0:
             old_num_avgs = reord_data.shape[-1]                                                 # Old Total Averages
             new_num_avgs = (reord_data.shape[-1] // 4) * 4                                      # New Total Averages
             reord_data   = reord_data[..., :new_num_avgs]                                       # Remove Incomplete
 
-            notestring   = '{:3d} {:<20}'.format(subseq, subseq_name)                           # Note Incomplete Data
-            notestring   = '{} - Correcting - Incomplete Averages'.format(notestring)           # Note Incomplete Data
-            notestring   = '{}  {} --> {}'.format(notestring, old_num_avgs, new_num_avgs)       # Note Incomplete Data
-            print('{} \t Corrected**'.format(notestring), end='\r')                             # Note Incomplete Data
+            notestring   = f'{subseq:3d} {subseq_name:<20}'                                     # Note Incomplete Data
+            notestring   = f'{notestring} - Correcting - Incomplete Averages'                   # Note Incomplete Data
+            notestring   = f'{notestring}  {old_num_avgs} --> {new_num_avgs}'                   # Note Incomplete Data
+            print(f'{notestring} \t Corrected**', end='\r')                                     # Note Incomplete Data
 
         dim_header       = {'EditCondition': ['A', 'B', 'C', 'D']}                              # 4 Subscans
         edit_pulse_val   = {'A': {'PulseOffset': [edit_pulse_1, edit_pulse_2], 'PulseDuration': pulse_length},
                             'B': {'PulseOffset': [edit_pulse_4, edit_pulse_2], 'PulseDuration': pulse_length},
                             'C': {'PulseOffset': edit_pulse_1, 'PulseDuration': pulse_length},
                             'D': {'PulseOffset': edit_pulse_4, 'PulseDuration': pulse_length}}
 
@@ -105,15 +105,15 @@
 
         for idx, dt in enumerate(dim_tags):                                                     # Iterate Dimensions
             if dt == 'DIM_EDIT':
                 meta_obj.set_dim_info(idx, dt, dim_info, dim_header)                            # Set Dimension
             else:
                 meta_obj.set_dim_info(idx, dt)                                                  # Set Dimension
 
-    print('{:3d} {:<20} - Completed  - Final Array Size: '.format(subseq, subseq_name), reord_data.shape)
+    print(f'{subseq:3d} {subseq_name:<20} - Completed  - Final Array Size: ', reord_data.shape)
 
     return reord_data, meta_obj, dim_tags
 
 
 def mgs_svs_ed_twix(twixObj, reord_data, meta_obj, dim_tags):
     """Special case handling for the mgs_svs_ed (VX) and smm_svs_herc (XA) sequence
```

### Comparing `spec2nii-0.6.8/spec2nii/Siemens/twixfunctions.py` & `spec2nii-0.6.9/spec2nii/Siemens/twixfunctions.py`

 * *Files 0% similar despite different names*

```diff
@@ -385,15 +385,15 @@
 
         reord_list = []                                                                     # List of Reord Data
         meta_list  = []                                                                     # List of Meta Objects
         dim_list   = []                                                                     # List of Dimensions
 
         # Reording the Data & Adjusting the Header Appropriately
         for ii in range(len(hyp_names)):                                                    # Iterate over Subscans
-            print('{:3d} {:<20}'.format(ii, hyp_names[ii]), end='\r')
+            print(f'{ii:3d} {hyp_names[ii]:<20}', end='\r')
             reord_data_, meta_obj_, dim_tags_ = smm_svs_herc_hyper(twixObj,
                                                                    reord_data,
                                                                    meta_obj,
                                                                    dim_tags,
                                                                    subseq=ii,
                                                                    subseq_name=hyp_names[ii])
 
@@ -404,15 +404,15 @@
         for ii in range(len(hyp_names)):
             if reord_list[ii].ndim <= 4:                                                    # 4 or less Dims
                 newshape  = (1, 1, 1) + reord_list[ii].shape                                # Pad 3 singleton dims
                 nifit_mrs_out.append(assemble_nifti_mrs(reord_list[ii].reshape(newshape),
                                                         dwellTime,
                                                         orientation,
                                                         meta_list[ii]))
-                filename_out.append('{}_{}'.format(mainStr, hyp_suffix[ii]))
+                filename_out.append(f'{mainStr}_{hyp_suffix[ii]}')
 
         return nifit_mrs_out, filename_out
 
     # HERCULES Data
     elif (xa_or_vx(twixObj['hdr']) == 'xa' and 'smm_svs_herc' in twixObj['hdr']['Meas'][('tSequenceFileName')]):
         from spec2nii.Siemens.twix_special_case import mgs_svs_ed_twix
         reord_data, meta_obj, dim_tags = mgs_svs_ed_twix(twixObj, reord_data, meta_obj, dim_tags)
```

### Comparing `spec2nii-0.6.8/spec2nii/anonymise.py` & `spec2nii-0.6.9/spec2nii/anonymise.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.8/spec2nii/bruker.py` & `spec2nii-0.6.9/spec2nii/bruker.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.8/spec2nii/bruker_fid_override.json` & `spec2nii-0.6.9/spec2nii/bruker_fid_override.json`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.8/spec2nii/bruker_properties.json` & `spec2nii-0.6.9/spec2nii/bruker_properties.json`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.8/spec2nii/dcm2niiOrientation/orientationFuncs.py` & `spec2nii-0.6.9/spec2nii/dcm2niiOrientation/orientationFuncs.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.8/spec2nii/fileiobase.py` & `spec2nii-0.6.9/spec2nii/fileiobase.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Originally part of NMR glue -- an open source module for working with NMR data
 in Python https://github.com/jjhelmus/nmrglue/
 
 If you find nmrglue useful in your research please cite the package as:
 
 J.J. Helmus, C.P. Jaroniec, Nmrglue: An open source Python package for the
 analysis of multidimensional NMR data, J. Biomol. NMR 2013, 55, 355-367,
-http://dx.doi.org/10.1007/s10858-013-9718-x.
+https://doi.org/10.1007/s10858-013-9718-x.
 ----------------
 
 Copyright Notice and Statement for the nmrglue Project
 
 
 Copyright (c) 2010-2015 Jonathan J. Helmus
 All rights reserved.
```

### Comparing `spec2nii-0.6.8/spec2nii/jmrui.py` & `spec2nii-0.6.9/spec2nii/jmrui.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.8/spec2nii/nifti_orientation.py` & `spec2nii-0.6.9/spec2nii/nifti_orientation.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.8/spec2nii/other.py` & `spec2nii-0.6.9/spec2nii/other.py`

 * *Files 7% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     except NotNIFTI_MRS:
         print(f'{args.file} is not compliant with the NIfTI-MRS standard, attempting to convert')
         from fsl.data.image import Image
         from nifti_mrs.create_nmrs import gen_nifti_mrs_hdr_ext
         from nifti_mrs.hdr_ext import Hdr_Ext
 
         nimg = Image(args.file)
-        hdr_ext = Hdr_Ext.from_header_ext(new_hdr, dimensions=nimg.ndim)
+        hdr_ext = Hdr_Ext.from_header_ext(new_hdr)
         nifti_mrs_img = gen_nifti_mrs_hdr_ext(
             nimg[:],
             nimg.header['pixdim'][4],
             hdr_ext,
             affine=nimg.getAffine('voxel', 'world'))
 
     if args.dwelltime is not None:
```

### Comparing `spec2nii-0.6.8/spec2nii/other_formats.py` & `spec2nii-0.6.9/spec2nii/other_formats.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.8/spec2nii/spec2nii.py` & `spec2nii-0.6.9/spec2nii/spec2nii.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.8/spec2nii/uih.py` & `spec2nii-0.6.9/spec2nii/uih.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.8/spec2nii/varian.py` & `spec2nii-0.6.9/spec2nii/varian.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Originally part of NMR glue -- an open source module for working with NMR data
 in Python https://github.com/jjhelmus/nmrglue/
 
 If you find nmrglue useful in your research please cite the package as:
 
 J.J. Helmus, C.P. Jaroniec, Nmrglue: An open source Python package for the
 analysis of multidimensional NMR data, J. Biomol. NMR 2013, 55, 355-367,
-http://dx.doi.org/10.1007/s10858-013-9718-x.
+https://doi.org/10.1007/s10858-013-9718-x.
 
 ------------
 Copyright Notice and Statement for the nmrglue Project
 
 
 Copyright (c) 2010-2015 Jonathan J. Helmus
 All rights reserved.
@@ -62,15 +62,15 @@
 Both the Agilent/Varian binary and parameter formats are documented in:
 
 * Varian MR News 2005-04-18 Importing Binary VnmrJ / VNMR FIDs into Third
     Party Software and VnmrJ / VNMR FID Data Format
 * VnmrJ User Programming - Chapter 5: Parameters and Data
 
 These are available (as of 04/2011) online from
-`Agilent <http://agilent.com>`_.
+`Agilent <https://www.agilent.com/>`_.
 
 """
 
 import os
 import struct
 import inspect
 from warnings import warn
```

### Comparing `spec2nii-0.6.8/spec2nii/varian_importer.py` & `spec2nii-0.6.9/spec2nii/varian_importer.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.8/spec2nii.egg-info/PKG-INFO` & `spec2nii-0.6.9/spec2nii.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spec2nii
-Version: 0.6.8
+Version: 0.6.9
 Summary: Multi-format in vivo MR spectroscopy conversion to NIFTI
 Home-page: https://github.com/wtclarke/spec2nii
 Author: Will Clarke
 Author-email: william.clarke@ndcn.ox.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `spec2nii-0.6.8/spec2nii.egg-info/SOURCES.txt` & `spec2nii-0.6.9/spec2nii.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.yml
 setup.cfg
 setup.py
@@ -23,14 +24,15 @@
 spec2nii/varian_importer.py
 spec2nii.egg-info/PKG-INFO
 spec2nii.egg-info/SOURCES.txt
 spec2nii.egg-info/dependency_links.txt
 spec2nii.egg-info/entry_points.txt
 spec2nii.egg-info/requires.txt
 spec2nii.egg-info/top_level.txt
+spec2nii/GE/VESPA_LICENSE
 spec2nii/GE/__init__.py
 spec2nii/GE/ge_hdr_fields.py
 spec2nii/GE/ge_pfile.py
 spec2nii/GE/ge_read_pfile.py
 spec2nii/GSL/__init__.py
 spec2nii/GSL/gslfunctions.py
 spec2nii/Philips/__init__.py
@@ -40,14 +42,16 @@
 spec2nii/Siemens/__init__.py
 spec2nii/Siemens/dicomfunctions.py
 spec2nii/Siemens/rda.py
 spec2nii/Siemens/twix_special_case.py
 spec2nii/Siemens/twixfunctions.py
 spec2nii/dcm2niiOrientation/__init__.py
 spec2nii/dcm2niiOrientation/orientationFuncs.py
+tests/__init__.py
+tests/io_for_tests.py
 tests/test_anon.py
 tests/test_auto.py
 tests/test_bruker.py
 tests/test_ge_pfile.py
 tests/test_ge_pfile_orientation.py
 tests/test_jmrui.py
 tests/test_nifti_options.py
```

### Comparing `spec2nii-0.6.8/tests/test_anon.py` & `spec2nii-0.6.9/tests/test_anon.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.8/tests/test_auto.py` & `spec2nii-0.6.9/tests/test_auto.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.8/tests/test_bruker.py` & `spec2nii-0.6.9/tests/test_bruker.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.8/tests/test_ge_pfile.py` & `spec2nii-0.6.9/tests/test_ge_pfile.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.8/tests/test_ge_pfile_orientation.py` & `spec2nii-0.6.9/tests/test_ge_pfile_orientation.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.8/tests/test_jmrui.py` & `spec2nii-0.6.9/tests/test_jmrui.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.8/tests/test_nifti_options.py` & `spec2nii-0.6.9/tests/test_nifti_options.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.8/tests/test_other.py` & `spec2nii-0.6.9/tests/test_other.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.8/tests/test_other_func.py` & `spec2nii-0.6.9/tests/test_other_func.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.8/tests/test_philips_data_list.py` & `spec2nii-0.6.9/tests/test_philips_data_list.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.8/tests/test_philips_dicom.py` & `spec2nii-0.6.9/tests/test_philips_dicom.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.8/tests/test_philips_dicom_orientation.py` & `spec2nii-0.6.9/tests/test_philips_dicom_orientation.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.8/tests/test_philips_sdat_spar.py` & `spec2nii-0.6.9/tests/test_philips_sdat_spar.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.8/tests/test_philips_sdat_spar_orientation.py` & `spec2nii-0.6.9/tests/test_philips_sdat_spar_orientation.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.8/tests/test_siemens_dicom.py` & `spec2nii-0.6.9/tests/test_siemens_dicom.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.8/tests/test_siemens_mrsi_orientation.py` & `spec2nii-0.6.9/tests/test_siemens_mrsi_orientation.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.8/tests/test_siemens_rda.py` & `spec2nii-0.6.9/tests/test_siemens_rda.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.8/tests/test_siemens_special_data.py` & `spec2nii-0.6.9/tests/test_siemens_special_data.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.8/tests/test_siemens_svs_orientation.py` & `spec2nii-0.6.9/tests/test_siemens_svs_orientation.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.8/tests/test_twix.py` & `spec2nii-0.6.9/tests/test_twix.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.8/tests/test_uih.py` & `spec2nii-0.6.9/tests/test_uih.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.8/tests/test_uih_orientation.py` & `spec2nii-0.6.9/tests/test_uih_orientation.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.8/tests/test_varian.py` & `spec2nii-0.6.9/tests/test_varian.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.6.8/versioneer.py` & `spec2nii-0.6.9/versioneer.py`

 * *Files identical despite different names*

