# Comparing `tmp/neurotechdevkit-0.1.1.tar.gz` & `tmp/neurotechdevkit-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurotechdevkit-0.1.1.tar", max compression
+gzip compressed data, was "neurotechdevkit-0.1.2.tar", max compression
```

## Comparing `neurotechdevkit-0.1.1.tar` & `neurotechdevkit-0.1.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0    11339 2023-05-27 00:58:36.941683 neurotechdevkit-0.1.1/LICENSE
--rw-r--r--   0        0        0     3304 2023-05-27 00:58:37.057684 neurotechdevkit-0.1.1/docs/index.md
--rw-r--r--   0        0        0     2146 2023-05-27 00:58:56.145862 neurotechdevkit-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2404 2023-05-27 00:58:37.057684 neurotechdevkit-0.1.1/src/neurotechdevkit/__init__.py
--rw-r--r--   0        0        0     1162 2023-05-27 00:58:37.057684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/__init__.py
--rw-r--r--   0        0        0     4747 2023-05-27 00:58:37.057684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/_animations.py
--rw-r--r--   0        0        0     2304 2023-05-27 00:58:37.057684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/_formatting.py
--rw-r--r--   0        0        0     8996 2023-05-27 00:58:37.057684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/_source.py
--rw-r--r--   0        0        0     3485 2023-05-27 00:58:37.057684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/_target.py
--rw-r--r--   0        0        0    49858 2023-05-27 00:58:37.061684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/colormaps.py
--rw-r--r--   0        0        0     2307 2023-05-27 00:58:37.061684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=10°.png
--rw-r--r--   0        0        0    30101 2023-05-27 00:58:37.061684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=120°.png
--rw-r--r--   0        0        0    50607 2023-05-27 00:58:37.061684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=150°.png
--rw-r--r--   0        0        0    61496 2023-05-27 00:58:37.061684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=180°.png
--rw-r--r--   0        0        0     4467 2023-05-27 00:58:37.061684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=20°.png
--rw-r--r--   0        0        0      715 2023-05-27 00:58:37.061684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=2°.png
--rw-r--r--   0        0        0     8691 2023-05-27 00:58:37.061684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=40°.png
--rw-r--r--   0        0        0     1147 2023-05-27 00:58:37.061684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=5°.png
--rw-r--r--   0        0        0    12673 2023-05-27 00:58:37.061684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=60°.png
--rw-r--r--   0        0        0    20015 2023-05-27 00:58:37.061684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=90°.png
--rw-r--r--   0        0        0     2753 2023-05-27 00:58:37.061684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=Flat.png
--rw-r--r--   0        0        0     3377 2023-05-27 00:58:37.061684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/target-dark.png
--rw-r--r--   0        0        0     3598 2023-05-27 00:58:37.061684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/target-light.png
--rw-r--r--   0        0        0      722 2023-05-27 00:58:37.061684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/font.py
--rw-r--r--   0        0        0    96364 2023-05-27 00:58:37.061684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/fonts/Manrope-Bold.ttf
--rw-r--r--   0        0        0    97116 2023-05-27 00:58:37.061684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/fonts/Manrope-ExtraBold.ttf
--rw-r--r--   0        0        0    96304 2023-05-27 00:58:37.061684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/fonts/Manrope-ExtraLight.ttf
--rw-r--r--   0        0        0    96312 2023-05-27 00:58:37.065684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/fonts/Manrope-Light.ttf
--rw-r--r--   0        0        0    96492 2023-05-27 00:58:37.065684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/fonts/Manrope-Medium.ttf
--rw-r--r--   0        0        0    96412 2023-05-27 00:58:37.065684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/fonts/Manrope-Regular.ttf
--rw-r--r--   0        0        0    96528 2023-05-27 00:58:37.065684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/fonts/Manrope-SemiBold.ttf
--rw-r--r--   0        0        0     4314 2023-05-27 00:58:37.065684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/layers.py
--rw-r--r--   0        0        0     5561 2023-05-27 00:58:37.065684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/layout.py
--rw-r--r--   0        0        0     6290 2023-05-27 00:58:37.065684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/legends.py
--rw-r--r--   0        0        0     7499 2023-05-27 00:58:37.065684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/napari.py
--rw-r--r--   0        0        0     8880 2023-05-27 00:58:37.065684 neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/simulations.py
--rw-r--r--   0        0        0      593 2023-05-27 00:58:37.065684 neurotechdevkit-0.1.1/src/neurotechdevkit/results/__init__.py
--rw-r--r--   0        0        0    53394 2023-05-27 00:58:37.065684 neurotechdevkit-0.1.1/src/neurotechdevkit/results/_results.py
--rw-r--r--   0        0        0      619 2023-05-27 00:58:37.065684 neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/__init__.py
--rw-r--r--   0        0        0    44605 2023-05-27 00:58:37.065684 neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/_base.py
--rw-r--r--   0        0        0    13024 2023-05-27 00:58:37.065684 neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/_metrics.py
--rw-r--r--   0        0        0     6053 2023-05-27 00:58:37.065684 neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/_resources.py
--rw-r--r--   0        0        0     4549 2023-05-27 00:58:37.065684 neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/_scenario_0.py
--rw-r--r--   0        0        0     8500 2023-05-27 00:58:37.065684 neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/_scenario_1.py
--rw-r--r--   0        0        0    11457 2023-05-27 00:58:37.065684 neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/_scenario_2.py
--rw-r--r--   0        0        0     7378 2023-05-27 00:58:37.065684 neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/_shots.py
--rw-r--r--   0        0        0     4559 2023-05-27 00:58:37.065684 neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/_time.py
--rw-r--r--   0        0        0    11913 2023-05-27 00:58:37.065684 neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/_utils.py
--rw-r--r--   0        0        0  2195183 2023-05-27 00:58:37.077684 neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/data/skull_mask_bm8_dx_0.5mm.mat
--rw-r--r--   0        0        0      936 2023-05-27 00:58:37.077684 neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/materials.py
--rw-r--r--   0        0        0    55819 2023-05-27 00:58:37.077684 neurotechdevkit-0.1.1/src/neurotechdevkit/sources.py
--rw-r--r--   0        0        0     4726 1970-01-01 00:00:00.000000 neurotechdevkit-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-07-07 14:59:39.884003 neurotechdevkit-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4034 2023-07-07 14:59:40.016007 neurotechdevkit-0.1.2/docs/index.md
+-rw-r--r--   0        0        0     2217 2023-07-07 14:59:56.776350 neurotechdevkit-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2404 2023-07-07 14:59:40.016007 neurotechdevkit-0.1.2/src/neurotechdevkit/__init__.py
+-rw-r--r--   0        0        0     1162 2023-07-07 14:59:40.016007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/__init__.py
+-rw-r--r--   0        0        0     4747 2023-07-07 14:59:40.016007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/_animations.py
+-rw-r--r--   0        0        0     2304 2023-07-07 14:59:40.016007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/_formatting.py
+-rw-r--r--   0        0        0     8996 2023-07-07 14:59:40.016007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/_source.py
+-rw-r--r--   0        0        0     3485 2023-07-07 14:59:40.016007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/_target.py
+-rw-r--r--   0        0        0    49858 2023-07-07 14:59:40.020007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/colormaps.py
+-rw-r--r--   0        0        0     2307 2023-07-07 14:59:40.020007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=10°.png
+-rw-r--r--   0        0        0    30101 2023-07-07 14:59:40.020007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=120°.png
+-rw-r--r--   0        0        0    50607 2023-07-07 14:59:40.020007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=150°.png
+-rw-r--r--   0        0        0    61496 2023-07-07 14:59:40.020007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=180°.png
+-rw-r--r--   0        0        0     4467 2023-07-07 14:59:40.020007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=20°.png
+-rw-r--r--   0        0        0      715 2023-07-07 14:59:40.020007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=2°.png
+-rw-r--r--   0        0        0     8691 2023-07-07 14:59:40.020007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=40°.png
+-rw-r--r--   0        0        0     1147 2023-07-07 14:59:40.020007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=5°.png
+-rw-r--r--   0        0        0    12673 2023-07-07 14:59:40.020007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=60°.png
+-rw-r--r--   0        0        0    20015 2023-07-07 14:59:40.020007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=90°.png
+-rw-r--r--   0        0        0     2753 2023-07-07 14:59:40.020007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=Flat.png
+-rw-r--r--   0        0        0     3377 2023-07-07 14:59:40.020007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/target-dark.png
+-rw-r--r--   0        0        0     3598 2023-07-07 14:59:40.020007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/target-light.png
+-rw-r--r--   0        0        0      722 2023-07-07 14:59:40.020007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/font.py
+-rw-r--r--   0        0        0    96364 2023-07-07 14:59:40.020007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/fonts/Manrope-Bold.ttf
+-rw-r--r--   0        0        0    97116 2023-07-07 14:59:40.020007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/fonts/Manrope-ExtraBold.ttf
+-rw-r--r--   0        0        0    96304 2023-07-07 14:59:40.024007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/fonts/Manrope-ExtraLight.ttf
+-rw-r--r--   0        0        0    96312 2023-07-07 14:59:40.024007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/fonts/Manrope-Light.ttf
+-rw-r--r--   0        0        0    96492 2023-07-07 14:59:40.024007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/fonts/Manrope-Medium.ttf
+-rw-r--r--   0        0        0    96412 2023-07-07 14:59:40.024007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/fonts/Manrope-Regular.ttf
+-rw-r--r--   0        0        0    96528 2023-07-07 14:59:40.024007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/fonts/Manrope-SemiBold.ttf
+-rw-r--r--   0        0        0     4314 2023-07-07 14:59:40.024007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/layers.py
+-rw-r--r--   0        0        0     5561 2023-07-07 14:59:40.024007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/layout.py
+-rw-r--r--   0        0        0     6290 2023-07-07 14:59:40.024007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/legends.py
+-rw-r--r--   0        0        0     7499 2023-07-07 14:59:40.024007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/napari.py
+-rw-r--r--   0        0        0     8880 2023-07-07 14:59:40.024007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/simulations.py
+-rw-r--r--   0        0        0      593 2023-07-07 14:59:40.024007 neurotechdevkit-0.1.2/src/neurotechdevkit/results/__init__.py
+-rw-r--r--   0        0        0    13016 2023-07-07 14:59:40.024007 neurotechdevkit-0.1.2/src/neurotechdevkit/results/_metrics.py
+-rw-r--r--   0        0        0    53384 2023-07-07 14:59:40.028007 neurotechdevkit-0.1.2/src/neurotechdevkit/results/_results.py
+-rw-r--r--   0        0        0      619 2023-07-07 14:59:40.028007 neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/__init__.py
+-rw-r--r--   0        0        0    44605 2023-07-07 14:59:40.028007 neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/_base.py
+-rw-r--r--   0        0        0     6053 2023-07-07 14:59:40.028007 neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/_resources.py
+-rw-r--r--   0        0        0     4549 2023-07-07 14:59:40.028007 neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/_scenario_0.py
+-rw-r--r--   0        0        0     8500 2023-07-07 14:59:40.028007 neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/_scenario_1.py
+-rw-r--r--   0        0        0    11457 2023-07-07 14:59:40.028007 neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/_scenario_2.py
+-rw-r--r--   0        0        0     7378 2023-07-07 14:59:40.028007 neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/_shots.py
+-rw-r--r--   0        0        0     4559 2023-07-07 14:59:40.028007 neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/_time.py
+-rw-r--r--   0        0        0    11913 2023-07-07 14:59:40.028007 neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/_utils.py
+-rw-r--r--   0        0        0  2195183 2023-07-07 14:59:40.040007 neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/data/skull_mask_bm8_dx_0.5mm.mat
+-rw-r--r--   0        0        0      936 2023-07-07 14:59:40.040007 neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/materials.py
+-rw-r--r--   0        0        0    55819 2023-07-07 14:59:40.040007 neurotechdevkit-0.1.2/src/neurotechdevkit/sources.py
+-rw-r--r--   0        0        0     5507 1970-01-01 00:00:00.000000 neurotechdevkit-0.1.2/PKG-INFO
```

### Comparing `neurotechdevkit-0.1.1/LICENSE` & `neurotechdevkit-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/pyproject.toml` & `neurotechdevkit-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neurotechdevkit"
-version = "v0.1.1"
+version = "v0.1.2"
 description = "Neurotech Development Kit: an open-source software library designed to enhance accessibility to cutting-edge neurotechnology"
 authors = ["AE Studio <bci@ae.studio>"]
 maintainers = ["AE Studio <bci@ae.studio>"]
 packages = [{include = "neurotechdevkit", from = "src" }]
 
 readme = "README.md"
 license = "Apache-2.0"
@@ -18,15 +18,15 @@
 [tool.poetry.urls]
 "Homepage" = "https://github.com/agencyenterprise/neurotechdevkit"
 "Documentation" = "https://agencyenterprise.github.io/neurotechdevkit/"
 "Bug Tracker" = "https://github.com/agencyenterprise/neurotechdevkit/issues"
 
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.11"
+python = ">=3.9,<3.12"
 numpy = "^1.23.3"
 matplotlib = "^3.5.3"
 imageio = "^2.21.2"
 jupyterlab = "^3.4.6"
 devito = "4.7.1"
 scipy = "^1.9.1"
 hdf5storage = "^0.1.18"
@@ -45,14 +45,16 @@
 pytest-asyncio = "^0.20.2"
 mkdocs-material = "^9.1.6"
 mkdocs-gallery = "^0.7.6"
 mkdocstrings = {extras = ["python"], version = "^0.21.2"}
 codespell = "^2.2.4"
 pydocstyle = "^6.3.0"
 pyright = "^1.1.306"
+pooch = "^1.7.0"
+pylint = {extras = ["spelling"], version = "^2.17.4"}
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 88
```

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/__init__.py` & `neurotechdevkit-0.1.2/src/neurotechdevkit/__init__.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/__init__.py` & `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/__init__.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/_animations.py` & `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/_animations.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/_formatting.py` & `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/_formatting.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/_source.py` & `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/_source.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/_target.py` & `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/_target.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/colormaps.py` & `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/colormaps.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=10°.png` & `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=10°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=120°.png` & `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=120°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=150°.png` & `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=150°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=180°.png` & `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=180°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=20°.png` & `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=20°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=2°.png` & `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=2°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=40°.png` & `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=40°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=5°.png` & `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=5°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=60°.png` & `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=60°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=90°.png` & `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=90°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/Angle=Flat.png` & `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=Flat.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/target-dark.png` & `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/target-dark.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/components/target-light.png` & `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/target-light.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/font.py` & `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/font.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/fonts/Manrope-Bold.ttf` & `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/fonts/Manrope-Bold.ttf`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/fonts/Manrope-ExtraBold.ttf` & `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/fonts/Manrope-ExtraBold.ttf`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/fonts/Manrope-ExtraLight.ttf` & `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/fonts/Manrope-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/fonts/Manrope-Light.ttf` & `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/fonts/Manrope-Light.ttf`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/fonts/Manrope-Medium.ttf` & `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/fonts/Manrope-Medium.ttf`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/fonts/Manrope-Regular.ttf` & `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/fonts/Manrope-Regular.ttf`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/fonts/Manrope-SemiBold.ttf` & `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/fonts/Manrope-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/layers.py` & `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/layers.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/layout.py` & `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/layout.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/legends.py` & `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/legends.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/napari.py` & `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/napari.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/rendering/simulations.py` & `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/simulations.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/results/__init__.py` & `neurotechdevkit-0.1.2/src/neurotechdevkit/results/__init__.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/results/_results.py` & `neurotechdevkit-0.1.2/src/neurotechdevkit/results/_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 import numpy.typing as npt
 import stride
 from matplotlib.animation import FuncAnimation
 
 import neurotechdevkit
 
 from .. import rendering, scenarios
-from ..scenarios import _metrics as metrics
 from ..scenarios._utils import drop_element, slice_field
+from . import _metrics as metrics
 
 DATA_FILENAME = "data.gz"
 
 
 def _get_ndk_version() -> str:
     """Get the version of the neurotechdevkit package.
```

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/__init__.py` & `neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/__init__.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/_base.py` & `neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/_base.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/_metrics.py` & `neurotechdevkit-0.1.2/src/neurotechdevkit/results/_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import numpy as np
 import numpy.typing as npt
 
-from ..results import _results as results
+from . import _results as results
 
 
 def calculate_all_metrics(
     result: results.SteadyStateResult,
 ) -> dict[str, dict[str, float | str]]:
     """Calculate all metrics for the steady-state result and return as a dictionary.
```

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/_resources.py` & `neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/_resources.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/_scenario_0.py` & `neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/_scenario_0.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/_scenario_1.py` & `neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/_scenario_1.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/_scenario_2.py` & `neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/_scenario_2.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/_shots.py` & `neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/_shots.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/_time.py` & `neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/_time.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/_utils.py` & `neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/_utils.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/data/skull_mask_bm8_dx_0.5mm.mat` & `neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/data/skull_mask_bm8_dx_0.5mm.mat`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/scenarios/materials.py` & `neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/materials.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.1/src/neurotechdevkit/sources.py` & `neurotechdevkit-0.1.2/src/neurotechdevkit/sources.py`

 * *Files 0% similar despite different names*

```diff
@@ -1321,15 +1321,15 @@
 
         The first and last element centers are calculated and the direction vector from
         the first element to the last element is computed.
 
         The current alignment is rotated to match the `self.unit_center_line` alignment.
 
         Args:
-            coords: Aa array containing the 3D coordinates to be aligned.
+            coords: An array containing the 3D coordinates to be aligned.
 
         Returns:
             An array of shape containing the aligned 3D coordinates.
 
         """
         v2 = self.unit_center_line
         point_mapping = self.point_mapping
```

### Comparing `neurotechdevkit-0.1.1/PKG-INFO` & `neurotechdevkit-0.1.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: neurotechdevkit
-Version: 0.1.1
+Version: 0.1.2
 Summary: Neurotech Development Kit: an open-source software library designed to enhance accessibility to cutting-edge neurotechnology
 License: Apache-2.0
 Author: AE Studio
 Author-email: bci@ae.studio
 Maintainer: AE Studio
 Maintainer-email: bci@ae.studio
-Requires-Python: >=3.9,<3.11
+Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: devito (==4.7.1)
 Requires-Dist: frozenlist (>=1.3.3,<2.0.0)
 Requires-Dist: hdf5storage (>=0.1.18,<0.2.0)
 Requires-Dist: imageio (>=2.21.2,<3.0.0)
 Requires-Dist: jupyterlab (>=3.4.6,<4.0.0)
 Requires-Dist: matplotlib (>=3.5.3,<4.0.0)
 Requires-Dist: mkdocs-gallery (==0.7.6)
@@ -29,45 +30,57 @@
 Project-URL: Bug Tracker, https://github.com/agencyenterprise/neurotechdevkit/issues
 Project-URL: Documentation, https://agencyenterprise.github.io/neurotechdevkit/
 Project-URL: Homepage, https://github.com/agencyenterprise/neurotechdevkit
 Description-Content-Type: text/markdown
 
 # Welcome to Neurotech Development Kit
 
-The [_Neurotech Development Kit_ (NDK)](https://agencyenterprise.github.io/neurotechdevkit/) is an open-source software library designed to enhance accessibility to cutting-edge neurotechnology.
-Featuring an easy-to-use API and pre-built examples, the NDK provides a seamless starting point for users.
-Moreover, the NDK offers educational resources, such as interactive simulations and notebook-based tutorials, catering to a diverse audience including researchers, educators, engineers, and trainees.
-By lowering the barrier of entry for newcomers and accelerating the progress of researchers, the NDK aims to be a versatile and invaluable tool for the neurotech community.
-
-The initial set of target users for the NDK are ultrasound simulation trainees – individuals with backgrounds in technical or neuroscience-related fields who are learning to perform ultrasound simulations.
-Our goal is to help users familiarize themselves with ultrasound simulation, understand the importance of input parameters, and streamline the process of running and visualizing simulations.
-In the future, we plan to expand the NDK's features to incorporate additional functionality and modalities, catering to a broader range of users, including ultrasound researchers, product developers, machine learning engineers, and many more.
+[![Linting](https://github.com/agencyenterprise/neurotechdevkit/actions/workflows/lint.yml/badge.svg)](https://github.com/agencyenterprise/neurotechdevkit/actions/workflows/lint.yml)
+[![Tests](https://github.com/agencyenterprise/neurotechdevkit/actions/workflows/test.yml/badge.svg)](https://github.com/agencyenterprise/neurotechdevkit/actions/workflows/test.yml)
+[![Gallery examples](https://circleci.com/gh/agencyenterprise/neurotechdevkit.png?style=shield)](https://circleci.com/gh/agencyenterprise/neurotechdevkit)
 
-The initial release of NDK provides support for transcranial functional ultrasound stimulation, with a focus on providing comprehensive documentation, API flexibility, and visualizations.
-The Neurotech Development Kit is actively developed and we welcome feedback and contributions.
+The [_Neurotech Development Kit_ (NDK)](https://agencyenterprise.github.io/neurotechdevkit/) is an open-source, community-driven software library designed to lower the barrier of entry to the next generation of neurotechnology for current researchers and companies. It also enables software developers without access to hardware and human subjects to solve open problems in the field. The initial release of NDK provides support for transcranial focused ultrasound stimulation, along with comprehensive documentation, API flexibility, and 2D/3D visualizations. Future areas of interest may include photoacoustic and optical whole-brain imaging.
+
+As a community-driven project, we encourage you to contribute code, feedback, and features to help accelerate the development of transformative neurotechnology.
 
 ![Simulation](https://raw.githubusercontent.com/agencyenterprise/neurotechdevkit/main/docs/images/ndk_example.gif)
 
 Check out the [NDK documentation page](https://agencyenterprise.github.io/neurotechdevkit/).
 
 ## Running
 
 ### Docker
 
-You can run `NDK` inside a docker container with a couple of steps:
+You can run `neurotechdevkit` inside a docker container with just a couple of steps:
 
 1. Install [docker](https://docs.docker.com/engine/install/#desktop)
 
-1. Execute `docker run -p 8888:8888 ghcr.io/agencyenterprise/neurotechdevkit:latest`
+1. Run the following command:
 
-The output of the command above contains the URL of a jupyter notebook server, you can open the URL in your browser or connect to it using your IDE.
+    ```
+    docker run -p 8888:8888 -it ghcr.io/agencyenterprise/neurotechdevkit:latest
+    ```
+
+    The command above will start a [Jupyter notebook](https://jupyterlab.readthedocs.io/en/stable/getting_started/overview.html) server with example notebooks you can use to explore `neurotechdevkit`. Use the printed URL to open it in your browser or connect to it using your IDE.
+
+    All changes you make to these files will be lost once you stop the docker container.
+
+> **Note**:
+>
+>    You can have persisting [Jupyter notebooks](https://jupyterlab.readthedocs.io/en/stable/getting_started/overview.html) by running
+>    ```
+>    docker run -p 8888:8888  -v $(pwd)/notebooks:/ndk/notebooks -it ghcr.io/agencyenterprise/neurotechdevkit:latest
+>    ```
+>    The command above will create a folder `notebooks` in your current directory where you can put your jupyter notebooks.
+>
+>    We recommend downloading the `.zip` file with example notebooks from this [link](https://agencyenterprise.github.io/neurotechdevkit/generated/gallery/gallery_jupyter.zip), and extracting it into your local `notebooks` folder so you can access them from the docker.
 
 ### Local installation
 
-To install and run **neurotechdevkit** locally check the [installation](usage/installation.md) page.
+To install and run **neurotechdevkit** locally check the [installation](https://agencyenterprise.github.io/neurotechdevkit/installation/) page.
 
 ## Usage
 
 ```python
 import neurotechdevkit as ndk
 
 scenario = ndk.make('scenario-0-v0')
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

