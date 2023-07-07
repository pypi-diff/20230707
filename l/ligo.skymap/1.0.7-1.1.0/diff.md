# Comparing `tmp/ligo.skymap-1.0.7.tar.gz` & `tmp/ligo.skymap-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ligo.skymap-1.0.7.tar", last modified: Mon Feb 27 14:24:40 2023, max compression
+gzip compressed data, was "ligo.skymap-1.1.0.tar", last modified: Fri Jul  7 17:47:37 2023, max compression
```

## Comparing `ligo.skymap-1.0.7.tar` & `ligo.skymap-1.1.0.tar`

### file list

```diff
@@ -1,291 +1,294 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.292123 ligo.skymap-1.0.7/
--rw-rw-rw-   0 root         (0) root         (0)      602 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.204120 ligo.skymap-1.0.7/.gitlab/
--rwxrwxrwx   0 root         (0) root         (0)     2033 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/.gitlab/combine-coverage.py
--rw-rw-rw-   0 root         (0) root         (0)    12458 2023-02-27 04:32:34.000000 ligo.skymap-1.0.7/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)    40623 2023-02-27 14:24:21.000000 ligo.skymap-1.0.7/CHANGES.rst
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/CONTRIBUTING.rst
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4219 2023-02-27 14:24:40.292123 ligo.skymap-1.0.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2777 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.197120 ligo.skymap-1.0.7/cextern/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.205120 ligo.skymap-1.0.7/cextern/chealpix/
--rw-rw-rw-   0 root         (0) root         (0)    30207 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/cextern/chealpix/chealpix.c
--rw-rw-rw-   0 root         (0) root         (0)     7407 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/cextern/chealpix/chealpix.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.210121 ligo.skymap-1.0.7/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4581 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.215121 ligo.skymap-1.0.7/docs/_static/
--rw-rw-rw-   0 root         (0) root         (0)    39163 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/_static/benchmark.svg
--rw-rw-rw-   0 root         (0) root         (0)   567737 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/_static/coinc.xml
--rw-rw-rw-   0 root         (0) root         (0)   260305 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/_static/localization.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.197120 ligo.skymap-1.0.7/docs/_templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.217121 ligo.skymap-1.0.7/docs/_templates/autosummary/
--rw-rw-rw-   0 root         (0) root         (0)      250 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/_templates/autosummary/base.rst
--rw-rw-rw-   0 root         (0) root         (0)      251 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/_templates/autosummary/class.rst
--rw-rw-rw-   0 root         (0) root         (0)      252 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/_templates/autosummary/module.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.220121 ligo.skymap-1.0.7/docs/bayestar/
--rw-rw-rw-   0 root         (0) root         (0)    56171 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/bayestar/eggbox.png
--rw-rw-rw-   0 root         (0) root         (0)      212 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/bayestar/ez_emcee.rst
--rw-rw-rw-   0 root         (0) root         (0)      182 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/bayestar/filter.rst
--rw-rw-rw-   0 root         (0) root         (0)      309 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/bayestar/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/bayestar/interpolation.rst
--rw-rw-rw-   0 root         (0) root         (0)    40623 2023-02-27 14:24:21.000000 ligo.skymap-1.0.7/docs/changes.rst
--rw-rw-rw-   0 root         (0) root         (0)     8638 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/contributing.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.220121 ligo.skymap-1.0.7/docs/coordinates/
--rw-rw-rw-   0 root         (0) root         (0)      191 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/coordinates/detector.rst
--rw-rw-rw-   0 root         (0) root         (0)      189 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/coordinates/eigenframe.rst
--rw-rw-rw-   0 root         (0) root         (0)     2304 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/develop.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.221121 ligo.skymap-1.0.7/docs/distance/
--rw-rw-rw-   0 root         (0) root         (0)     1243 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/distance/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.221121 ligo.skymap-1.0.7/docs/healpix_tree/
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/healpix_tree/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      595 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/help.rst
--rw-rw-rw-   0 root         (0) root         (0)     4518 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)    15650 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/interface.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.222121 ligo.skymap-1.0.7/docs/io/
--rw-rw-rw-   0 root         (0) root         (0)     3691 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/io/events.rst
--rw-rw-rw-   0 root         (0) root         (0)      146 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/io/fits.rst
--rw-rw-rw-   0 root         (0) root         (0)      166 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/io/hdf5.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.222121 ligo.skymap-1.0.7/docs/kde/
--rw-rw-rw-   0 root         (0) root         (0)      162 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/kde/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4549 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       13 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/matplotlibrc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.223121 ligo.skymap-1.0.7/docs/moc/
--rw-rw-rw-   0 root         (0) root         (0)      267 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/moc/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1282 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/performance.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.224121 ligo.skymap-1.0.7/docs/plot/
--rw-rw-rw-   0 root         (0) root         (0)      186 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/plot/allsky.rst
--rw-rw-rw-   0 root         (0) root         (0)      198 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/plot/backdrop.rst
--rw-rw-rw-   0 root         (0) root         (0)      205 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/plot/marker.rst
--rw-rw-rw-   0 root         (0) root         (0)      166 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/plot/poly.rst
--rw-rw-rw-   0 root         (0) root         (0)      182 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/plot/pp.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.226121 ligo.skymap-1.0.7/docs/postprocess/
--rw-rw-rw-   0 root         (0) root         (0)      180 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/postprocess/contour.rst
--rw-rw-rw-   0 root         (0) root         (0)      184 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/postprocess/cosmology.rst
--rw-rw-rw-   0 root         (0) root         (0)      253 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/postprocess/crossmatch.rst
--rw-rw-rw-   0 root         (0) root         (0)      200 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/postprocess/ellipse.rst
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/postprocess/util.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.226121 ligo.skymap-1.0.7/docs/quickstart/
--rw-rw-rw-   0 root         (0) root         (0)     6351 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/quickstart/bayestar-injections.rst
--rw-rw-rw-   0 root         (0) root         (0)     4156 2023-02-27 05:49:16.000000 ligo.skymap-1.0.7/docs/quickstart/install.rst
--rw-rw-rw-   0 root         (0) root         (0)     1585 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/testing.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.233121 ligo.skymap-1.0.7/docs/tool/
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/tool/bayestar_inject.rst
--rw-rw-rw-   0 root         (0) root         (0)      188 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/tool/bayestar_localize_coincs.rst
--rw-rw-rw-   0 root         (0) root         (0)      204 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/tool/bayestar_localize_lvalert.rst
--rw-rw-rw-   0 root         (0) root         (0)      189 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/tool/bayestar_mcmc.rst
--rw-rw-rw-   0 root         (0) root         (0)      179 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/tool/bayestar_realize_coincs.rst
--rw-rw-rw-   0 root         (0) root         (0)      175 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/tool/bayestar_sample_model_psd.rst
--rw-rw-rw-   0 root         (0) root         (0)      175 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/tool/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1400 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/tool/ligo_skymap_combine.rst
--rw-rw-rw-   0 root         (0) root         (0)     3709 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/tool/ligo_skymap_constellations.rst
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/tool/ligo_skymap_contour.rst
--rw-rw-rw-   0 root         (0) root         (0)      215 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/tool/ligo_skymap_contour_moc.rst
--rw-rw-rw-   0 root         (0) root         (0)      199 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/tool/ligo_skymap_flatten.rst
--rw-rw-rw-   0 root         (0) root         (0)     1387 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/tool/ligo_skymap_from_samples.rst
--rw-rw-rw-   0 root         (0) root         (0)      747 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/tool/ligo_skymap_plot.rst
--rw-rw-rw-   0 root         (0) root         (0)      795 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/tool/ligo_skymap_plot_airmass.rst
--rw-rw-rw-   0 root         (0) root         (0)     1121 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/tool/ligo_skymap_plot_observability.rst
--rw-rw-rw-   0 root         (0) root         (0)      188 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/tool/ligo_skymap_plot_stats.rst
--rw-rw-rw-   0 root         (0) root         (0)      700 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/tool/ligo_skymap_plot_volume.rst
--rw-rw-rw-   0 root         (0) root         (0)      177 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/tool/ligo_skymap_stats.rst
--rw-rw-rw-   0 root         (0) root         (0)      209 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/tool/ligo_skymap_unflatten.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.235121 ligo.skymap-1.0.7/docs/util/
--rw-rw-rw-   0 root         (0) root         (0)      158 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/util/file.rst
--rw-rw-rw-   0 root         (0) root         (0)      172 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/util/ilwd.rst
--rw-rw-rw-   0 root         (0) root         (0)      163 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/util/numpy.rst
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/docs/util/sqlite.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.237121 ligo.skymap-1.0.7/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     6360 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/licenses/CHEALPIX_LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)    37565 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)     1792 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/licenses/NUMPY_LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      372 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/licenses/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1659 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/licenses/TEMPLATE_LICENCE.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.199120 ligo.skymap-1.0.7/ligo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.241121 ligo.skymap-1.0.7/ligo/skymap/
--rw-rw-rw-   0 root         (0) root         (0)     1012 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      698 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/_astropy_init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.243121 ligo.skymap-1.0.7/ligo/skymap/bayestar/
--rw-rw-rw-   0 root         (0) root         (0)    20852 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/bayestar/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5864 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/bayestar/ez_emcee.py
--rw-rw-rw-   0 root         (0) root         (0)    19685 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/bayestar/filter.py
--rw-rw-rw-   0 root         (0) root         (0)    10348 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/bayestar/interpolation.py
--rw-rw-rw-   0 root         (0) root         (0)     2176 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/bayestar/ptemcee.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.244121 ligo.skymap-1.0.7/ligo/skymap/bayestar/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/bayestar/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1545 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/bayestar/tests/test_bayestar.py
--rw-rw-rw-   0 root         (0) root         (0)     4573 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/bayestar/tests/test_interpolation.py
--rw-rw-rw-   0 root         (0) root         (0)     4287 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/bayestar/tests/test_signal_amplitude_model.py
--rw-rw-rw-   0 root         (0) root         (0)     2321 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.246122 ligo.skymap-1.0.7/ligo/skymap/coordinates/
--rw-rw-rw-   0 root         (0) root         (0)      382 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/coordinates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3645 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/coordinates/detector.py
--rw-rw-rw-   0 root         (0) root         (0)     4132 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/coordinates/eigenframe.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.247122 ligo.skymap-1.0.7/ligo/skymap/coordinates/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/coordinates/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      996 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/coordinates/tests/test_detector.py
--rw-rw-rw-   0 root         (0) root         (0)    20879 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/distance.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.248122 ligo.skymap-1.0.7/ligo/skymap/extern/
--rw-rw-rw-   0 root         (0) root         (0)      460 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/extern/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.249122 ligo.skymap-1.0.7/ligo/skymap/extern/numpy/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/extern/numpy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13938 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/extern/numpy/quantile.py
--rw-rw-rw-   0 root         (0) root         (0)    15264 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/healpix_tree.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.251122 ligo.skymap-1.0.7/ligo/skymap/io/
--rw-rw-rw-   0 root         (0) root         (0)      382 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/io/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.255122 ligo.skymap-1.0.7/ligo/skymap/io/events/
--rw-rw-rw-   0 root         (0) root         (0)      382 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/io/events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3832 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/io/events/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2664 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/io/events/detector_disabled.py
--rw-rw-rw-   0 root         (0) root         (0)     2274 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/io/events/gracedb.py
--rw-rw-rw-   0 root         (0) root         (0)     7809 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/io/events/hdf.py
--rw-rw-rw-   0 root         (0) root         (0)    11345 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/io/events/ligolw.py
--rw-rw-rw-   0 root         (0) root         (0)     2563 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/io/events/magic.py
--rw-rw-rw-   0 root         (0) root         (0)     1700 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/io/events/sqlite.py
--rwxrwxrwx   0 root         (0) root         (0)    19227 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/io/fits.py
--rwxrwxrwx   0 root         (0) root         (0)    10598 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/io/hdf5.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.256122 ligo.skymap-1.0.7/ligo/skymap/io/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/io/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.262122 ligo.skymap-1.0.7/ligo/skymap/io/tests/data/
--rw-rw-rw-   0 root         (0) root         (0)   492938 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/io/tests/data/2016_subset.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)     1699 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/io/tests/data/G197392_coinc.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)      675 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/io/tests/data/G197392_psd.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)     2470 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/io/tests/data/G211117_coinc.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)     2355 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/io/tests/data/G211117_psd.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/io/tests/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.262122 ligo.skymap-1.0.7/ligo/skymap/io/tests/data/gstlal_reference_psd/
--rw-rw-rw-   0 root         (0) root         (0)      717 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/io/tests/data/gstlal_reference_psd/H1L1V1-REFERENCE_PSD-967234210-29963.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/io/tests/data/gstlal_reference_psd/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9120 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/io/tests/data/test.hdf5
--rw-rw-rw-   0 root         (0) root         (0)    12598 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/io/tests/test_io_events.py
--rw-rw-rw-   0 root         (0) root         (0)    18854 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/kde.py
--rw-rw-rw-   0 root         (0) root         (0)     4806 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/moc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.269122 ligo.skymap-1.0.7/ligo/skymap/plot/
--rw-rw-rw-   0 root         (0) root         (0)      382 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/plot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    29184 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/plot/allsky.py
--rw-rw-rw-   0 root         (0) root         (0)     1415 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/plot/angle.py
--rw-rw-rw-   0 root         (0) root         (0)     7291 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/plot/backdrop.py
--rw-rw-rw-   0 root         (0) root         (0)     1522 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/plot/cmap.py
--rw-rw-rw-   0 root         (0) root         (0)     8714 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/plot/cylon.csv
--rw-rw-rw-   0 root         (0) root         (0)     2125 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/plot/cylon.py
--rw-rw-rw-   0 root         (0) root         (0)     2933 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/plot/marker.py
--rw-rw-rw-   0 root         (0) root         (0)    63275 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/plot/ne_simplified_coastline.json
--rw-rw-rw-   0 root         (0) root         (0)     7394 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/plot/poly.py
--rw-rw-rw-   0 root         (0) root         (0)     9445 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/plot/pp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.269122 ligo.skymap-1.0.7/ligo/skymap/plot/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/plot/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.274122 ligo.skymap-1.0.7/ligo/skymap/plot/tests/baseline/
--rw-rw-rw-   0 root         (0) root         (0)    67690 2023-02-27 05:49:16.000000 ligo.skymap-1.0.7/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-degrees-aitoff.png
--rw-rw-rw-   0 root         (0) root         (0)    65830 2023-02-27 05:49:16.000000 ligo.skymap-1.0.7/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-degrees-mollweide.png
--rw-rw-rw-   0 root         (0) root         (0)    65829 2023-02-27 05:49:16.000000 ligo.skymap-1.0.7/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-hours-aitoff.png
--rw-rw-rw-   0 root         (0) root         (0)    63879 2023-02-27 05:49:16.000000 ligo.skymap-1.0.7/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-hours-mollweide.png
--rw-rw-rw-   0 root         (0) root         (0)    71762 2023-02-27 05:49:16.000000 ligo.skymap-1.0.7/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-degrees-aitoff.png
--rw-rw-rw-   0 root         (0) root         (0)    71509 2023-02-27 05:49:16.000000 ligo.skymap-1.0.7/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-degrees-mollweide.png
--rw-rw-rw-   0 root         (0) root         (0)    70497 2023-02-27 05:49:16.000000 ligo.skymap-1.0.7/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-hours-aitoff.png
--rw-rw-rw-   0 root         (0) root         (0)    69334 2023-02-27 05:49:16.000000 ligo.skymap-1.0.7/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-hours-mollweide.png
--rw-rw-rw-   0 root         (0) root         (0)    64896 2023-02-27 05:49:16.000000 ligo.skymap-1.0.7/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-degrees-aitoff.png
--rw-rw-rw-   0 root         (0) root         (0)    63732 2023-02-27 05:49:16.000000 ligo.skymap-1.0.7/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-degrees-mollweide.png
--rw-rw-rw-   0 root         (0) root         (0)    63470 2023-02-27 05:49:16.000000 ligo.skymap-1.0.7/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-hours-aitoff.png
--rw-rw-rw-   0 root         (0) root         (0)    61561 2023-02-27 05:49:16.000000 ligo.skymap-1.0.7/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-hours-mollweide.png
--rw-rw-rw-   0 root         (0) root         (0)    33964 2023-02-27 05:49:16.000000 ligo.skymap-1.0.7/ligo/skymap/plot/tests/baseline/test_allsky_obstime.png
--rw-rw-rw-   0 root         (0) root         (0)    20330 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/plot/tests/baseline/test_globe_axes.png
--rw-rw-rw-   0 root         (0) root         (0)    19092 2023-02-27 05:49:16.000000 ligo.skymap-1.0.7/ligo/skymap/plot/tests/baseline/test_pp_plot_default.png
--rw-rw-rw-   0 root         (0) root         (0)    39991 2023-02-27 05:49:16.000000 ligo.skymap-1.0.7/ligo/skymap/plot/tests/baseline/test_pp_plot_lines.png
--rw-rw-rw-   0 root         (0) root         (0)    19092 2023-02-27 05:49:16.000000 ligo.skymap-1.0.7/ligo/skymap/plot/tests/baseline/test_pp_plot_steps.png
--rw-rw-rw-   0 root         (0) root         (0)     8866 2023-02-27 05:49:16.000000 ligo.skymap-1.0.7/ligo/skymap/plot/tests/baseline/test_reticle.png
--rw-rw-rw-   0 root         (0) root         (0)    19815 2023-02-27 05:49:16.000000 ligo.skymap-1.0.7/ligo/skymap/plot/tests/baseline/test_zoom_axes.png
--rw-rw-rw-   0 root         (0) root         (0)     5202 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/plot/tests/test_plot.py
--rw-rw-rw-   0 root         (0) root         (0)     2400 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/plot/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.275123 ligo.skymap-1.0.7/ligo/skymap/postprocess/
--rw-rw-rw-   0 root         (0) root         (0)      382 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/postprocess/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6348 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/postprocess/contour.py
--rw-rw-rw-   0 root         (0) root         (0)     2698 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/postprocess/cosmology.py
--rw-rw-rw-   0 root         (0) root         (0)    18664 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/postprocess/crossmatch.py
--rw-rw-rw-   0 root         (0) root         (0)    14581 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/postprocess/ellipse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.276122 ligo.skymap-1.0.7/ligo/skymap/postprocess/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/postprocess/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      899 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/postprocess/tests/test_cosmology.py
--rw-rw-rw-   0 root         (0) root         (0)     4373 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/postprocess/tests/test_crossmatch.py
--rw-rw-rw-   0 root         (0) root         (0)     3219 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/postprocess/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.276122 ligo.skymap-1.0.7/ligo/skymap/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.277123 ligo.skymap-1.0.7/ligo/skymap/tests/plugins/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/tests/plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      578 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/tests/plugins/omp.py
--rw-rw-rw-   0 root         (0) root         (0)     4390 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/tests/test_moc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.282123 ligo.skymap-1.0.7/ligo/skymap/tool/
--rw-rw-rw-   0 root         (0) root         (0)    15427 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/tool/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21594 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/tool/bayestar_inject.py
--rw-rw-rw-   0 root         (0) root         (0)     7486 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/tool/bayestar_localize_coincs.py
--rwxrwxrwx   0 root         (0) root         (0)     6781 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/tool/bayestar_localize_lvalert.py
--rw-rw-rw-   0 root         (0) root         (0)     8058 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/tool/bayestar_mcmc.py
--rw-rw-rw-   0 root         (0) root         (0)    18751 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/tool/bayestar_realize_coincs.py
--rw-rw-rw-   0 root         (0) root         (0)     4600 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/tool/bayestar_sample_model_psd.py
--rw-rw-rw-   0 root         (0) root         (0)     5841 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/tool/ligo_skymap_combine.py
--rw-rw-rw-   0 root         (0) root         (0)     2011 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/tool/ligo_skymap_constellations.py
--rw-rw-rw-   0 root         (0) root         (0)     3341 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/tool/ligo_skymap_contour.py
--rw-rw-rw-   0 root         (0) root         (0)     2508 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/tool/ligo_skymap_contour_moc.py
--rw-rw-rw-   0 root         (0) root         (0)     2288 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/tool/ligo_skymap_flatten.py
--rw-rw-rw-   0 root         (0) root         (0)     7330 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/tool/ligo_skymap_from_samples.py
--rw-rw-rw-   0 root         (0) root         (0)     6722 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/tool/ligo_skymap_plot.py
--rw-rw-rw-   0 root         (0) root         (0)     8343 2023-02-27 04:32:34.000000 ligo.skymap-1.0.7/ligo/skymap/tool/ligo_skymap_plot_airmass.py
--rw-rw-rw-   0 root         (0) root         (0)     5701 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/tool/ligo_skymap_plot_observability.py
--rw-rw-rw-   0 root         (0) root         (0)     5148 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/tool/ligo_skymap_plot_pp_samples.py
--rw-rw-rw-   0 root         (0) root         (0)     8066 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/tool/ligo_skymap_plot_stats.py
--rwxrwxrwx   0 root         (0) root         (0)     9394 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/tool/ligo_skymap_plot_volume.py
--rw-rw-rw-   0 root         (0) root         (0)    11830 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/tool/ligo_skymap_stats.py
--rw-rw-rw-   0 root         (0) root         (0)     1739 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/tool/ligo_skymap_unflatten.py
--rw-rw-rw-   0 root         (0) root         (0)     4389 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/tool/matplotlib.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.285123 ligo.skymap-1.0.7/ligo/skymap/tool/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3125 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/tool/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5271 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/tool/tests/test_bayestar.py
--rw-rw-rw-   0 root         (0) root         (0)     4494 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/tool/tests/test_bayestar_inject.py
--rw-rw-rw-   0 root         (0) root         (0)     2400 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/tool/tests/test_combine.py
--rw-rw-rw-   0 root         (0) root         (0)     4015 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/tool/tests/test_flatten.py
--rw-rw-rw-   0 root         (0) root         (0)     2631 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/tool/tests/test_from_samples.py
--rw-rw-rw-   0 root         (0) root         (0)      529 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/tool/tests/test_help.py
--rw-rw-rw-   0 root         (0) root         (0)     1826 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/tool/tests/test_plot.py
--rw-rw-rw-   0 root         (0) root         (0)     2065 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/tool/tests/test_plot_stats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.287123 ligo.skymap-1.0.7/ligo/skymap/util/
--rw-rw-rw-   0 root         (0) root         (0)      382 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1794 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/util/file.py
--rw-rw-rw-   0 root         (0) root         (0)     5163 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/util/ilwd.py
--rw-rw-rw-   0 root         (0) root         (0)     1680 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/util/numpy.py
--rw-rw-rw-   0 root         (0) root         (0)     2854 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/util/progress.py
--rw-rw-rw-   0 root         (0) root         (0)     4451 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/util/sqlite.py
--rw-rw-rw-   0 root         (0) root         (0)     2694 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/util/stopwatch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.287123 ligo.skymap-1.0.7/ligo/skymap/util/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/util/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      363 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/ligo/skymap/util/tests/test_progress.py
--rw-r--r--   0 root         (0) root         (0)      337 2023-02-27 14:24:40.000000 ligo.skymap-1.0.7/ligo/skymap/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.238121 ligo.skymap-1.0.7/ligo.skymap.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4219 2023-02-27 14:24:40.000000 ligo.skymap-1.0.7/ligo.skymap.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8207 2023-02-27 14:24:40.000000 ligo.skymap-1.0.7/ligo.skymap.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-27 14:24:40.000000 ligo.skymap-1.0.7/ligo.skymap.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1472 2023-02-27 14:24:40.000000 ligo.skymap-1.0.7/ligo.skymap.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-02-27 14:24:40.000000 ligo.skymap-1.0.7/ligo.skymap.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-27 14:24:40.000000 ligo.skymap-1.0.7/ligo.skymap.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      432 2023-02-27 14:24:40.000000 ligo.skymap-1.0.7/ligo.skymap.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-02-27 14:24:40.000000 ligo.skymap-1.0.7/ligo.skymap.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      355 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     6379 2023-02-27 14:24:40.293123 ligo.skymap-1.0.7/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     3514 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 14:24:40.291123 ligo.skymap-1.0.7/src/
--rw-rw-rw-   0 root         (0) root         (0)    37062 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/src/bayestar_cosmology.h
--rw-rw-rw-   0 root         (0) root         (0)     4078 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/src/bayestar_cosmology.py
--rw-rw-rw-   0 root         (0) root         (0)    15859 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/src/bayestar_distance.c
--rw-rw-rw-   0 root         (0) root         (0)     2067 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/src/bayestar_distance.h
--rw-rw-rw-   0 root         (0) root         (0)     4025 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/src/bayestar_moc.c
--rw-rw-rw-   0 root         (0) root         (0)     1492 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/src/bayestar_moc.h
--rw-rw-rw-   0 root         (0) root         (0)    53672 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/src/bayestar_sky_map.c
--rw-rw-rw-   0 root         (0) root         (0)     7887 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/src/bayestar_sky_map.h
--rw-rw-rw-   0 root         (0) root         (0)      218 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/src/branch_prediction.h
--rw-rw-rw-   0 root         (0) root         (0)    40070 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/src/core.c
--rw-rw-rw-   0 root         (0) root         (0)     5818 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/src/cubic_interp.c
--rw-rw-rw-   0 root         (0) root         (0)     2069 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/src/cubic_interp.h
--rw-rw-rw-   0 root         (0) root         (0)    13016 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/src/cubic_interp_test.c
--rw-rw-rw-   0 root         (0) root         (0)     6370 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/src/omp_interruptible.h
--rw-rw-rw-   0 root         (0) root         (0)     2377 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/src/vmath.h
--rw-rw-rw-   0 root         (0) root         (0)     1869 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/src/warnings.h
--rw-rw-rw-   0 root         (0) root         (0)     2589 2023-02-24 14:50:44.000000 ligo.skymap-1.0.7/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.555839 ligo.skymap-1.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)      602 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.516839 ligo.skymap-1.1.0/.gitlab/
+-rwxrwxrwx   0 root         (0) root         (0)     2033 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/.gitlab/combine-coverage.py
+-rw-rw-rw-   0 root         (0) root         (0)    12513 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)    42221 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/CHANGES.rst
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4216 2023-07-07 17:47:37.556839 ligo.skymap-1.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2777 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.509839 ligo.skymap-1.1.0/cextern/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.516839 ligo.skymap-1.1.0/cextern/chealpix/
+-rw-rw-rw-   0 root         (0) root         (0)    30207 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/cextern/chealpix/chealpix.c
+-rw-rw-rw-   0 root         (0) root         (0)     7407 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/cextern/chealpix/chealpix.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.518839 ligo.skymap-1.1.0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4581 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.519839 ligo.skymap-1.1.0/docs/_static/
+-rw-rw-rw-   0 root         (0) root         (0)    39163 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/_static/benchmark.svg
+-rw-rw-rw-   0 root         (0) root         (0)   567737 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/_static/coinc.xml
+-rw-rw-rw-   0 root         (0) root         (0)   260305 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/_static/localization.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.509839 ligo.skymap-1.1.0/docs/_templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.520839 ligo.skymap-1.1.0/docs/_templates/autosummary/
+-rw-rw-rw-   0 root         (0) root         (0)      250 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/_templates/autosummary/base.rst
+-rw-rw-rw-   0 root         (0) root         (0)      251 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/_templates/autosummary/class.rst
+-rw-rw-rw-   0 root         (0) root         (0)      252 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/_templates/autosummary/module.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.520839 ligo.skymap-1.1.0/docs/bayestar/
+-rw-rw-rw-   0 root         (0) root         (0)    56171 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/bayestar/eggbox.png
+-rw-rw-rw-   0 root         (0) root         (0)      212 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/bayestar/ez_emcee.rst
+-rw-rw-rw-   0 root         (0) root         (0)      182 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/bayestar/filter.rst
+-rw-rw-rw-   0 root         (0) root         (0)      309 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/bayestar/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/bayestar/interpolation.rst
+-rw-rw-rw-   0 root         (0) root         (0)    42221 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/changes.rst
+-rw-rw-rw-   0 root         (0) root         (0)     8638 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/contributing.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.521839 ligo.skymap-1.1.0/docs/coordinates/
+-rw-rw-rw-   0 root         (0) root         (0)      191 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/coordinates/detector.rst
+-rw-rw-rw-   0 root         (0) root         (0)      189 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/coordinates/eigenframe.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2304 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/develop.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.521839 ligo.skymap-1.1.0/docs/distance/
+-rw-rw-rw-   0 root         (0) root         (0)     1243 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/distance/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.521839 ligo.skymap-1.1.0/docs/healpix_tree/
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/healpix_tree/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      595 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/help.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4574 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)    15650 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/interface.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.521839 ligo.skymap-1.1.0/docs/io/
+-rw-rw-rw-   0 root         (0) root         (0)     3691 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/io/events.rst
+-rw-rw-rw-   0 root         (0) root         (0)      146 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/io/fits.rst
+-rw-rw-rw-   0 root         (0) root         (0)      166 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/io/hdf5.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.522839 ligo.skymap-1.1.0/docs/kde/
+-rw-rw-rw-   0 root         (0) root         (0)      162 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/kde/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4549 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       13 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/matplotlibrc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.522839 ligo.skymap-1.1.0/docs/moc/
+-rw-rw-rw-   0 root         (0) root         (0)      267 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/moc/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1282 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/performance.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.523839 ligo.skymap-1.1.0/docs/plot/
+-rw-rw-rw-   0 root         (0) root         (0)      186 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/plot/allsky.rst
+-rw-rw-rw-   0 root         (0) root         (0)      198 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/plot/backdrop.rst
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/plot/bayes_factor.rst
+-rw-rw-rw-   0 root         (0) root         (0)      205 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/plot/marker.rst
+-rw-rw-rw-   0 root         (0) root         (0)      166 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/plot/poly.rst
+-rw-rw-rw-   0 root         (0) root         (0)      182 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/plot/pp.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.524839 ligo.skymap-1.1.0/docs/postprocess/
+-rw-rw-rw-   0 root         (0) root         (0)      180 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/postprocess/contour.rst
+-rw-rw-rw-   0 root         (0) root         (0)      184 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/postprocess/cosmology.rst
+-rw-rw-rw-   0 root         (0) root         (0)      253 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/postprocess/crossmatch.rst
+-rw-rw-rw-   0 root         (0) root         (0)      200 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/postprocess/ellipse.rst
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/postprocess/util.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.524839 ligo.skymap-1.1.0/docs/quickstart/
+-rw-rw-rw-   0 root         (0) root         (0)     6351 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/quickstart/bayestar-injections.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4156 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/quickstart/install.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/testing.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.527839 ligo.skymap-1.1.0/docs/tool/
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/tool/bayestar_inject.rst
+-rw-rw-rw-   0 root         (0) root         (0)      188 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/tool/bayestar_localize_coincs.rst
+-rw-rw-rw-   0 root         (0) root         (0)      204 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/tool/bayestar_localize_lvalert.rst
+-rw-rw-rw-   0 root         (0) root         (0)      189 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/tool/bayestar_mcmc.rst
+-rw-rw-rw-   0 root         (0) root         (0)      179 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/tool/bayestar_realize_coincs.rst
+-rw-rw-rw-   0 root         (0) root         (0)      175 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/tool/bayestar_sample_model_psd.rst
+-rw-rw-rw-   0 root         (0) root         (0)      175 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/tool/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1400 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/tool/ligo_skymap_combine.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3709 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/tool/ligo_skymap_constellations.rst
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/tool/ligo_skymap_contour.rst
+-rw-rw-rw-   0 root         (0) root         (0)      215 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/tool/ligo_skymap_contour_moc.rst
+-rw-rw-rw-   0 root         (0) root         (0)      199 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/tool/ligo_skymap_flatten.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1387 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/tool/ligo_skymap_from_samples.rst
+-rw-rw-rw-   0 root         (0) root         (0)      747 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/tool/ligo_skymap_plot.rst
+-rw-rw-rw-   0 root         (0) root         (0)      795 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/tool/ligo_skymap_plot_airmass.rst
+-rw-rw-rw-   0 root         (0) root         (0)      779 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/tool/ligo_skymap_plot_coherence.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/tool/ligo_skymap_plot_observability.rst
+-rw-rw-rw-   0 root         (0) root         (0)      188 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/tool/ligo_skymap_plot_stats.rst
+-rw-rw-rw-   0 root         (0) root         (0)      700 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/tool/ligo_skymap_plot_volume.rst
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/tool/ligo_skymap_stats.rst
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/tool/ligo_skymap_unflatten.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.528839 ligo.skymap-1.1.0/docs/util/
+-rw-rw-rw-   0 root         (0) root         (0)      158 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/util/file.rst
+-rw-rw-rw-   0 root         (0) root         (0)      172 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/util/ilwd.rst
+-rw-rw-rw-   0 root         (0) root         (0)      163 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/util/numpy.rst
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/docs/util/sqlite.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.529839 ligo.skymap-1.1.0/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     6360 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/licenses/CHEALPIX_LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)    37565 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1792 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/licenses/NUMPY_LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/licenses/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1659 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/licenses/TEMPLATE_LICENCE.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.511839 ligo.skymap-1.1.0/ligo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.531839 ligo.skymap-1.1.0/ligo/skymap/
+-rw-rw-rw-   0 root         (0) root         (0)     1012 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      698 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/_astropy_init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.532839 ligo.skymap-1.1.0/ligo/skymap/bayestar/
+-rw-rw-rw-   0 root         (0) root         (0)    20852 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/bayestar/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5864 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/bayestar/ez_emcee.py
+-rw-rw-rw-   0 root         (0) root         (0)    19685 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/bayestar/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)    10348 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/bayestar/interpolation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2176 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/bayestar/ptemcee.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.532839 ligo.skymap-1.1.0/ligo/skymap/bayestar/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/bayestar/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1545 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/bayestar/tests/test_bayestar.py
+-rw-rw-rw-   0 root         (0) root         (0)     4573 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/bayestar/tests/test_interpolation.py
+-rw-rw-rw-   0 root         (0) root         (0)     4287 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/bayestar/tests/test_signal_amplitude_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2321 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.533839 ligo.skymap-1.1.0/ligo/skymap/coordinates/
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/coordinates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3645 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/coordinates/detector.py
+-rw-rw-rw-   0 root         (0) root         (0)     4132 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/coordinates/eigenframe.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.533839 ligo.skymap-1.1.0/ligo/skymap/coordinates/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/coordinates/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      996 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/coordinates/tests/test_detector.py
+-rw-rw-rw-   0 root         (0) root         (0)    20879 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/distance.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.533839 ligo.skymap-1.1.0/ligo/skymap/extern/
+-rw-rw-rw-   0 root         (0) root         (0)      460 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/extern/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.534839 ligo.skymap-1.1.0/ligo/skymap/extern/numpy/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/extern/numpy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13938 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/extern/numpy/quantile.py
+-rw-rw-rw-   0 root         (0) root         (0)    15264 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/healpix_tree.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.534839 ligo.skymap-1.1.0/ligo/skymap/io/
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.536839 ligo.skymap-1.1.0/ligo/skymap/io/events/
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3832 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/events/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2664 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/events/detector_disabled.py
+-rw-rw-rw-   0 root         (0) root         (0)     2274 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/events/gracedb.py
+-rw-rw-rw-   0 root         (0) root         (0)     7809 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/events/hdf.py
+-rw-rw-rw-   0 root         (0) root         (0)    11345 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/events/ligolw.py
+-rw-rw-rw-   0 root         (0) root         (0)     2563 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/events/magic.py
+-rw-rw-rw-   0 root         (0) root         (0)     1700 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/events/sqlite.py
+-rwxrwxrwx   0 root         (0) root         (0)    19227 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/fits.py
+-rwxrwxrwx   0 root         (0) root         (0)    10598 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/hdf5.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.536839 ligo.skymap-1.1.0/ligo/skymap/io/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.537839 ligo.skymap-1.1.0/ligo/skymap/io/tests/data/
+-rw-rw-rw-   0 root         (0) root         (0)   492938 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/tests/data/2016_subset.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)     1699 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/tests/data/G197392_coinc.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)      675 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/tests/data/G197392_psd.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)     2470 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/tests/data/G211117_coinc.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)     2355 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/tests/data/G211117_psd.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/tests/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.538839 ligo.skymap-1.1.0/ligo/skymap/io/tests/data/gstlal_reference_psd/
+-rw-rw-rw-   0 root         (0) root         (0)      717 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/tests/data/gstlal_reference_psd/H1L1V1-REFERENCE_PSD-967234210-29963.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/tests/data/gstlal_reference_psd/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9120 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/tests/data/test.hdf5
+-rw-rw-rw-   0 root         (0) root         (0)    12598 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/io/tests/test_io_events.py
+-rw-rw-rw-   0 root         (0) root         (0)    17043 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/kde.py
+-rw-rw-rw-   0 root         (0) root         (0)     7533 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/moc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.540839 ligo.skymap-1.1.0/ligo/skymap/plot/
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    29184 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/allsky.py
+-rw-rw-rw-   0 root         (0) root         (0)     1415 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/angle.py
+-rw-rw-rw-   0 root         (0) root         (0)     7291 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/backdrop.py
+-rw-rw-rw-   0 root         (0) root         (0)     3910 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/bayes_factor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1522 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/cmap.py
+-rw-rw-rw-   0 root         (0) root         (0)     8714 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/cylon.csv
+-rw-rw-rw-   0 root         (0) root         (0)     2125 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/cylon.py
+-rw-rw-rw-   0 root         (0) root         (0)     2933 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/marker.py
+-rw-rw-rw-   0 root         (0) root         (0)    63275 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/ne_simplified_coastline.json
+-rw-rw-rw-   0 root         (0) root         (0)     7394 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/poly.py
+-rw-rw-rw-   0 root         (0) root         (0)     9445 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/pp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.540839 ligo.skymap-1.1.0/ligo/skymap/plot/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.544839 ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/
+-rw-rw-rw-   0 root         (0) root         (0)    67690 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-degrees-aitoff.png
+-rw-rw-rw-   0 root         (0) root         (0)    65830 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-degrees-mollweide.png
+-rw-rw-rw-   0 root         (0) root         (0)    65829 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-hours-aitoff.png
+-rw-rw-rw-   0 root         (0) root         (0)    63879 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-hours-mollweide.png
+-rw-rw-rw-   0 root         (0) root         (0)    71762 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-degrees-aitoff.png
+-rw-rw-rw-   0 root         (0) root         (0)    71509 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-degrees-mollweide.png
+-rw-rw-rw-   0 root         (0) root         (0)    70497 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-hours-aitoff.png
+-rw-rw-rw-   0 root         (0) root         (0)    69334 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-hours-mollweide.png
+-rw-rw-rw-   0 root         (0) root         (0)    64896 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-degrees-aitoff.png
+-rw-rw-rw-   0 root         (0) root         (0)    63732 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-degrees-mollweide.png
+-rw-rw-rw-   0 root         (0) root         (0)    63470 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-hours-aitoff.png
+-rw-rw-rw-   0 root         (0) root         (0)    61561 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-hours-mollweide.png
+-rw-rw-rw-   0 root         (0) root         (0)    33964 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_obstime.png
+-rw-rw-rw-   0 root         (0) root         (0)    20330 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_globe_axes.png
+-rw-rw-rw-   0 root         (0) root         (0)    19092 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_pp_plot_default.png
+-rw-rw-rw-   0 root         (0) root         (0)    39991 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_pp_plot_lines.png
+-rw-rw-rw-   0 root         (0) root         (0)    19092 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_pp_plot_steps.png
+-rw-rw-rw-   0 root         (0) root         (0)     8866 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_reticle.png
+-rw-rw-rw-   0 root         (0) root         (0)    19815 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_zoom_axes.png
+-rw-rw-rw-   0 root         (0) root         (0)     5202 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/tests/test_plot.py
+-rw-rw-rw-   0 root         (0) root         (0)     2400 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/plot/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.545839 ligo.skymap-1.1.0/ligo/skymap/postprocess/
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/postprocess/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6348 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/postprocess/contour.py
+-rw-rw-rw-   0 root         (0) root         (0)     2407 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/postprocess/cosmology.py
+-rw-rw-rw-   0 root         (0) root         (0)    18664 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/postprocess/crossmatch.py
+-rw-rw-rw-   0 root         (0) root         (0)    15257 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/postprocess/ellipse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.546839 ligo.skymap-1.1.0/ligo/skymap/postprocess/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/postprocess/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      899 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/postprocess/tests/test_cosmology.py
+-rw-rw-rw-   0 root         (0) root         (0)     4373 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/postprocess/tests/test_crossmatch.py
+-rw-rw-rw-   0 root         (0) root         (0)     3219 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/postprocess/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.546839 ligo.skymap-1.1.0/ligo/skymap/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.546839 ligo.skymap-1.1.0/ligo/skymap/tests/plugins/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tests/plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      578 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tests/plugins/omp.py
+-rw-rw-rw-   0 root         (0) root         (0)     4831 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tests/test_moc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.550839 ligo.skymap-1.1.0/ligo/skymap/tool/
+-rw-rw-rw-   0 root         (0) root         (0)    15669 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21608 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/bayestar_inject.py
+-rw-rw-rw-   0 root         (0) root         (0)     7538 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/bayestar_localize_coincs.py
+-rwxrwxrwx   0 root         (0) root         (0)     6821 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/bayestar_localize_lvalert.py
+-rw-rw-rw-   0 root         (0) root         (0)     8137 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/bayestar_mcmc.py
+-rw-rw-rw-   0 root         (0) root         (0)    18761 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/bayestar_realize_coincs.py
+-rw-rw-rw-   0 root         (0) root         (0)     4600 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/bayestar_sample_model_psd.py
+-rw-rw-rw-   0 root         (0) root         (0)     5841 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_combine.py
+-rw-rw-rw-   0 root         (0) root         (0)     2011 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_constellations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3341 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_contour.py
+-rw-rw-rw-   0 root         (0) root         (0)     2519 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_contour_moc.py
+-rw-rw-rw-   0 root         (0) root         (0)     2288 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_flatten.py
+-rw-rw-rw-   0 root         (0) root         (0)     7662 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_from_samples.py
+-rw-rw-rw-   0 root         (0) root         (0)     6732 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_plot.py
+-rw-rw-rw-   0 root         (0) root         (0)     8353 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_plot_airmass.py
+-rw-rw-rw-   0 root         (0) root         (0)     1713 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_plot_coherence.py
+-rw-rw-rw-   0 root         (0) root         (0)     5711 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_plot_observability.py
+-rw-rw-rw-   0 root         (0) root         (0)     5158 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_plot_pp_samples.py
+-rw-rw-rw-   0 root         (0) root         (0)     8048 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_plot_stats.py
+-rwxrwxrwx   0 root         (0) root         (0)     9404 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_plot_volume.py
+-rw-rw-rw-   0 root         (0) root         (0)    11830 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_stats.py
+-rw-rw-rw-   0 root         (0) root         (0)     1739 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_unflatten.py
+-rw-rw-rw-   0 root         (0) root         (0)     4508 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/matplotlib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.551839 ligo.skymap-1.1.0/ligo/skymap/tool/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3064 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5271 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/tests/test_bayestar.py
+-rw-rw-rw-   0 root         (0) root         (0)     4494 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/tests/test_bayestar_inject.py
+-rw-rw-rw-   0 root         (0) root         (0)     2400 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/tests/test_combine.py
+-rw-rw-rw-   0 root         (0) root         (0)     4015 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/tests/test_flatten.py
+-rw-rw-rw-   0 root         (0) root         (0)     2631 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/tests/test_from_samples.py
+-rw-rw-rw-   0 root         (0) root         (0)      529 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/tests/test_help.py
+-rw-rw-rw-   0 root         (0) root         (0)     1826 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/tests/test_plot.py
+-rw-rw-rw-   0 root         (0) root         (0)     2065 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/tool/tests/test_plot_stats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.552839 ligo.skymap-1.1.0/ligo/skymap/util/
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1794 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/util/file.py
+-rw-rw-rw-   0 root         (0) root         (0)     5163 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/util/ilwd.py
+-rw-rw-rw-   0 root         (0) root         (0)     1680 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/util/numpy.py
+-rw-rw-rw-   0 root         (0) root         (0)     2854 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/util/progress.py
+-rw-rw-rw-   0 root         (0) root         (0)     4451 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/util/sqlite.py
+-rw-rw-rw-   0 root         (0) root         (0)     2694 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/util/stopwatch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.553839 ligo.skymap-1.1.0/ligo/skymap/util/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/util/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      363 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/ligo/skymap/util/tests/test_progress.py
+-rw-r--r--   0 root         (0) root         (0)      337 2023-07-07 17:47:37.000000 ligo.skymap-1.1.0/ligo/skymap/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.530839 ligo.skymap-1.1.0/ligo.skymap.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4216 2023-07-07 17:47:37.000000 ligo.skymap-1.1.0/ligo.skymap.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8311 2023-07-07 17:47:37.000000 ligo.skymap-1.1.0/ligo.skymap.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 17:47:37.000000 ligo.skymap-1.1.0/ligo.skymap.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1550 2023-07-07 17:47:37.000000 ligo.skymap-1.1.0/ligo.skymap.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 17:47:37.000000 ligo.skymap-1.1.0/ligo.skymap.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      432 2023-07-07 17:47:37.000000 ligo.skymap-1.1.0/ligo.skymap.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-07 17:47:37.000000 ligo.skymap-1.1.0/ligo.skymap.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      355 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     6429 2023-07-07 17:47:37.557839 ligo.skymap-1.1.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     3574 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:47:37.555839 ligo.skymap-1.1.0/src/
+-rw-rw-rw-   0 root         (0) root         (0)    37062 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/src/bayestar_cosmology.h
+-rw-rw-rw-   0 root         (0) root         (0)     4078 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/src/bayestar_cosmology.py
+-rw-rw-rw-   0 root         (0) root         (0)    15859 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/src/bayestar_distance.c
+-rw-rw-rw-   0 root         (0) root         (0)     2067 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/src/bayestar_distance.h
+-rw-rw-rw-   0 root         (0) root         (0)     4025 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/src/bayestar_moc.c
+-rw-rw-rw-   0 root         (0) root         (0)     1492 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/src/bayestar_moc.h
+-rw-rw-rw-   0 root         (0) root         (0)    53672 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/src/bayestar_sky_map.c
+-rw-rw-rw-   0 root         (0) root         (0)     7887 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/src/bayestar_sky_map.h
+-rw-rw-rw-   0 root         (0) root         (0)      218 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/src/branch_prediction.h
+-rw-rw-rw-   0 root         (0) root         (0)    39503 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/src/core.c
+-rw-rw-rw-   0 root         (0) root         (0)     5818 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/src/cubic_interp.c
+-rw-rw-rw-   0 root         (0) root         (0)     2069 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/src/cubic_interp.h
+-rw-rw-rw-   0 root         (0) root         (0)    13016 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/src/cubic_interp_test.c
+-rw-rw-rw-   0 root         (0) root         (0)     6370 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/src/omp_interruptible.h
+-rw-rw-rw-   0 root         (0) root         (0)     2377 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/src/vmath.h
+-rw-rw-rw-   0 root         (0) root         (0)     1869 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/src/warnings.h
+-rw-rw-rw-   0 root         (0) root         (0)     2595 2023-07-07 17:47:25.000000 ligo.skymap-1.1.0/tox.ini
```

### Comparing `ligo.skymap-1.0.7/.gitignore` & `ligo.skymap-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/.gitlab/combine-coverage.py` & `ligo.skymap-1.1.0/.gitlab/combine-coverage.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/.gitlab-ci.yml` & `ligo.skymap-1.1.0/.gitlab-ci.yml`

 * *Files 10% similar despite different names*

```diff
@@ -48,54 +48,57 @@
       - '*.tar.*'
     expire_in: 1 day
 
 #
 # Build binary wheels for Linux and macOS.
 #
 
-.wheel-manylinux: &wheel-manylinux
+.wheel-linux: &wheel-linux
   stage: dist
   script:
     # Build and install LALSuite
-    - PYPREFIX=/opt/python/cp38-cp38
+    - PYPREFIX=/opt/python/cp39-cp39
     - ${PYPREFIX}/bin/pip install build
     - ${PYPREFIX}/bin/python -m build -w
     - auditwheel repair dist/*.whl
     - rm dist/*
     - mv wheelhouse/* .
   needs: []
   artifacts:
     paths:
       - '*.whl'
     expire_in: 1 day
 
-wheel/manylinux/x86_64:
-  <<: *wheel-manylinux
+wheel/linux/x86_64:
+  <<: *wheel-linux
   # This container is derived from the official manylinux image provided by
   # python.org (see PEP 513), and includes all of the LALSuite
   # build-dependencies.
   image: containers.ligo.org/lscsoft/lalsuite-manylinux/manylinux_2_28_x86_64:icc
 
-wheel/manylinux/aarch64:
-  <<: *wheel-manylinux
+wheel/linux/aarch64:
+  <<: *wheel-linux
+  variables:
+    CFLAGS: -Ofast -fno-finite-math-only -flto
   # This container is derived from the official manylinux image provided by
   # python.org (see PEP 513), and includes all of the LALSuite
   # build-dependencies.
   image: containers.ligo.org/lscsoft/lalsuite-manylinux/manylinux_2_28_aarch64
   tags:
     - aarch64
 
 .wheel-macos: &wheel-macos
   variables:
     CC: gcc-mp-11
     CXX: g++-mp-11
+    CFLAGS: -Ofast -fno-finite-math-only -flto
   stage: dist
   script:
     - . /opt/local/share/macports/setupenv.bash
-    - PYVERS=3.8
+    - PYVERS=3.9
     # Enter virtualenv so that we have a controlled version of Numpy
     - python${PYVERS} -m venv env
     - source env/bin/activate
     - pip install build delocate
     # Build and audit wheel
     - python -m build -w .
     - delocate-wheel -v -w wheelhouse dist/*.whl
@@ -127,15 +130,15 @@
   before_script:
     - WORKING_DIRECTORY="$(mktemp -d)"
     - cd "${WORKING_DIRECTORY}"
   after_script:
     - cd "${CI_PROJECT_DIR}"
     - rm -rf "${WORKING_DIRECTORY}"
 
-.dependencies: &dependencies
+.deps: &deps
   stage: dist
   variables:
     IMAGE_TAG: $CI_REGISTRY_IMAGE/$CI_JOB_NAME:$CI_COMMIT_REF_SLUG
     GIT_STRATEGY: none
   script:
     - docker login -u gitlab-ci-token -p $CI_JOB_TOKEN $CI_REGISTRY
     - |
@@ -147,40 +150,42 @@
       RUN pip --no-cache-dir install -r requirements.txt && rm -f requirements.txt
       EOF
     - docker build -t $IMAGE_TAG .
     - docker push $IMAGE_TAG
   needs:
     - requirements
 
-dependencies/python3.8:
-  <<: *dependencies
+deps-aarch64/python3.9:
+  <<: *deps
+  tags:
+    - aarch64
 
-dependencies/python3.9:
-  <<: *dependencies
+deps-x86_64/python3.9:
+  <<: *deps
 
-dependencies/python3.10:
-  <<: *dependencies
+deps-x86_64/python3.10:
+  <<: *deps
 
-dependencies/python3.11:
-  <<: *dependencies
+deps-x86_64/python3.11:
+  <<: *deps
 
 #
 # Generate documentation.
 #
 
 docs:
-  image: $CI_REGISTRY_IMAGE/dependencies/python3.8:$CI_COMMIT_REF_SLUG
+  image: $CI_REGISTRY_IMAGE/deps-x86_64/python3.9:$CI_COMMIT_REF_SLUG
   stage: test
   <<: *in-tmpdir
   script:
     - tar --strip-components 1 -xf ${CI_PROJECT_DIR}/*.tar.*
     - tox -e build_docs
     - mv docs/_build/html ${CI_PROJECT_DIR}/
   needs:
-    - dependencies/python3.8
+    - deps-x86_64/python3.9
     - sdist
   artifacts:
     paths:
       - html/
     expire_in: 1 day
 
 #
@@ -190,48 +195,50 @@
 .test: &test
   <<: *in-tmpdir
   stage: test
   script:
     - pip install $(echo ${CI_PROJECT_DIR}/*.whl)[test]
     - python -c 'import sys; from ligo.skymap import test; sys.exit(test(args="--doctest-plus --doctest-ufunc --mpl --omp-get-num-threads --durations=10"))'
 
-test/linux/python3.8:
+test/linux/aarch64/python3.9:
   <<: *test
-  image: $CI_REGISTRY_IMAGE/dependencies/python3.8:$CI_COMMIT_REF_SLUG
+  image: $CI_REGISTRY_IMAGE/deps-aarch64/python3.9:$CI_COMMIT_REF_SLUG
   needs:
-    - dependencies/python3.8
-    - wheel/manylinux/x86_64
+    - deps-aarch64/python3.9
+    - wheel/linux/aarch64
+  tags:
+    - aarch64
 
-test/linux/python3.9:
+test/linux/x86_64/python3.9:
   <<: *test
-  image: $CI_REGISTRY_IMAGE/dependencies/python3.9:$CI_COMMIT_REF_SLUG
+  image: $CI_REGISTRY_IMAGE/deps-x86_64/python3.9:$CI_COMMIT_REF_SLUG
   needs:
-    - dependencies/python3.9
-    - wheel/manylinux/x86_64
+    - deps-x86_64/python3.9
+    - wheel/linux/x86_64
 
-test/linux/python3.10:
+test/linux/x86_64/python3.10:
   <<: *test
-  image: $CI_REGISTRY_IMAGE/dependencies/python3.10:$CI_COMMIT_REF_SLUG
+  image: $CI_REGISTRY_IMAGE/deps-x86_64/python3.10:$CI_COMMIT_REF_SLUG
   needs:
-    - dependencies/python3.10
-    - wheel/manylinux/x86_64
+    - deps-x86_64/python3.10
+    - wheel/linux/x86_64
 
-test/linux/python3.11:
+test/linux/x86_64/python3.11:
   <<: *test
-  image: $CI_REGISTRY_IMAGE/dependencies/python3.11:$CI_COMMIT_REF_SLUG
+  image: $CI_REGISTRY_IMAGE/deps-x86_64/python3.11:$CI_COMMIT_REF_SLUG
   needs:
-    - dependencies/python3.11
-    - wheel/manylinux/x86_64
+    - deps-x86_64/python3.11
+    - wheel/linux/x86_64
 
 .test/macos: &test-macos
   <<: *in-tmpdir
   stage: test
   script:
     - . /opt/local/share/macports/setupenv.bash
-    - PYVERS=3.8
+    - PYVERS=3.9
     # Enter virtualenv so that we have a controlled version of Numpy
     - python${PYVERS} -m venv env
     - source env/bin/activate
     - pip install $(echo ${CI_PROJECT_DIR}/*.whl)[test]
     - python -c 'import sys; from ligo.skymap import test; sys.exit(test(args="--doctest-plus --doctest-ufunc --mpl --omp-get-num-threads --durations=10"))'
 
 
@@ -247,30 +254,30 @@
   <<: *test-macos
   tags:
     - macos_monterey_arm64
   needs:
     - wheel/macos/arm64
 
 # Test against development versions of certain upstream dependencies.
-test/dev-dependencies:
+test/dev-deps:
   <<: *test
   image: python:3.9
   script:
     # Qhull is needed to build Matplotlib from source
     - apt-get update && apt-get -y install --no-install-recommends libqhull-dev
     - >
       pip install
       git+https://github.com/numpy/numpy
       git+https://github.com/matplotlib/matplotlib
       git+https://github.com/astropy/astropy
       git+https://git.ligo.org/kipp.cannon/python-ligo-lw
       $(echo ${CI_PROJECT_DIR}/*.whl)[test]
     - python -c 'import sys; from ligo.skymap import test; sys.exit(test(args="--doctest-plus --doctest-ufunc --mpl --omp-get-num-threads --durations=10"))'
   needs:
-    - wheel/manylinux/x86_64
+    - wheel/linux/x86_64
   rules:
     - if: '$CI_PIPELINE_SOURCE == "schedule"'
 
 #
 # Measure test coverage:
 # - coverage.py for Python code
 # - gcov/gcovr for C code
@@ -282,15 +289,15 @@
 # This would be a lot prettier if we could use coveralls or codecov.io,
 # which support multilingual test coverage. However, those products don't
 # integrate with git.ligo.org (or at least, they don't integrate for free).
 #
 
 test/coverage:
   stage: test
-  image: $CI_REGISTRY_IMAGE/dependencies/python3.8:$CI_COMMIT_REF_SLUG
+  image: $CI_REGISTRY_IMAGE/deps-x86_64/python3.9:$CI_COMMIT_REF_SLUG
   variables:
     # -UNDEBUG
     #     enable C assertions
     # -coverage
     #     instrument C code for coverage measurement
     # -fsanitize=undefined
     #     enable GCC UndefinedBehaviorSanitizer
@@ -307,25 +314,25 @@
     # Run tests.
     # FIXME: C coverage relies on in-tree build/ directory.
     # pip 21.3 uses an out-of-tree temporary directory.
     - pip install 'pip<21.3'
     - pip install -ve .[test]
     - pytest --capture=sys --doctest-plus --doctest-ufunc --mpl --mpl-results-path ${CI_PROJECT_DIR}/pytest-mpl-results --durations=10 --cov ligo/skymap --junit-xml=${CI_PROJECT_DIR}/junit.xml || FAILED=true
     # Write coverage reports in Cobertura format.
-    - gcovr build/temp*/src -r . -x -o c-coverage.xml
+    - gcovr --gcov-ignore-errors no_working_dir_found build/temp*/src -r . -x -o c-coverage.xml
     - coverage xml -o py-coverage.xml
     # Merge coverage reports.
     - ${CI_PROJECT_DIR}/.gitlab/combine-coverage.py py-coverage.xml c-coverage.xml coverage.xml
     # Write human-readable report.
     - pycobertura show coverage.xml -f html -o coverage.html
     - pycobertura show coverage.xml
     - cp coverage.html coverage.xml ${CI_PROJECT_DIR}
     - if [[ "$FAILED" ]]; then false; fi
   needs:
-    - dependencies/python3.8
+    - deps-x86_64/python3.9
     - sdist
   artifacts:
     paths:
       - coverage.html
       - pytest-mpl-results/
     reports:
       coverage_report:
@@ -339,29 +346,29 @@
 #
 # Run flake8 linter to enforce code style.
 #
 
 lint:
   extends:
     - .python:flake8
-  image: $CI_REGISTRY_IMAGE/dependencies/python3.8:$CI_COMMIT_REF_SLUG
+  image: $CI_REGISTRY_IMAGE/deps-x86_64/python3.9:$CI_COMMIT_REF_SLUG
   stage: test
   needs:
-    - dependencies/python3.8
+    - deps-x86_64/python3.9
 
 #
 # Acceptance tests.
 #
 
 tests/review:
   stage: test
   image: containers.ligo.org/emfollow/ssh-kerberos
   when: manual
   needs:
-    - wheel/manylinux/x86_64
+    - wheel/linux/x86_64
   variables:
     GIT_STRATEGY: none
     REMOTE_HOST: skymap.testing@ldas-grid.ligo.caltech.edu
   script:
     - echo -e "section_start:`date +%s`:remote_clone\r\e[0KCloning HTCondor workflow on cluster"
     - ssh -T $REMOTE_HOST "mkdir -p public_html && git clone --depth=1 --recurse-submodules --shallow-submodules https://git.ligo.org/leo-singer/ligo-skymap-acceptance-tests-public public_html/$CI_PIPELINE_ID"
     - echo -e "section_end:`date +%s`:remote_clone\r\e[0K"
@@ -376,15 +383,15 @@
       pip install *.whl
       pip install -r requirements.txt
       EOF
     - echo -e "section_end:`date +%s`:remote_install\r\e[0K"
 
     - echo -e "section_start:`date +%s`:remote_submit\r\e[0KRunning HTCondor workflow on cluster"
     - |
-      containers.ligo.org/emfollow/ssh-kerberosssh -T $REMOTE_HOST "bash -e" <<EOF
+      ssh -T $REMOTE_HOST "bash -e" <<EOF
       cd public_html/$CI_PIPELINE_ID
       source env/bin/activate
       condor_submit_dag -append accounting_group_user=leo.singer -batch-name pipeline/$CI_PIPELINE_ID htcondor/acceptance-tests.dag
       tail --follow=descriptor --retry htcondor/acceptance-tests.dag.dagman.out &
       condor_wait htcondor/acceptance-tests.dag.dagman.log
       kill %
       EOF
@@ -434,13 +441,13 @@
   image: python:slim
   script:
     # TWINE_USERNAME and TWINE_PASSWORD are provided by CI secret variables
     - pip install twine
     - twine upload *.whl *.tar.*
   needs:
     - sdist
-    - wheel/manylinux/x86_64
-    - wheel/manylinux/aarch64
+    - wheel/linux/x86_64
+    - wheel/linux/aarch64
     - wheel/macos/x86_64
     - wheel/macos/arm64
   only:
     - tags
```

### Comparing `ligo.skymap-1.0.7/CHANGES.rst` & `ligo.skymap-1.1.0/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,55 @@
 #########
 Changelog
 #########
 
+1.1.0 (2023-07-07)
+==================
+
+- Add ``max_depth`` keyword argument to the call to
+  ``MOC.from_valued_healpix_cells`` in ``ligo-skymap-contour-moc``.
+  Contributed by `@parkma99 <https://github.com/parkma99>`_.
+
+- Improve handling of the ``--output`` command line argument for
+  ``ligo-skymap-contour-moc``:
+
+  - Add ``-o`` as a short form.
+
+  - Don't write to stdout by default; it does not make sense to write a binary
+    FITS file to stdout.
+
+  - Make the argument required.
+
+- Drop dependency on distutils to prepare for its removal in Python 3.12.
+  See `PEP 632 <https://peps.python.org/pep-0632/>`_.
+
+- Drop support for Python 3.8.
+
+- Vectorize ``find_ellipse`` over the ``cl`` argument.
+
+- Tune compiler settings used to build wheels for PyPI:
+
+  - Add the option ``-fvisibility=hidden`` to hide all symbols except for the
+    Python entry point. This improves the efficiency of link-time optimization.
+    On average, it speeds up BAYESTAR by about 5%.
+
+  - Add the options ``-Ofast -fno-finite-math-only -flto`` on Linux aarch64
+    and macOS, the targets on which we use gcc. These options approximate the
+    configuration that we use for icc on Linux x86_64. On average, this change
+    speeds up BAYESTAR on macOS by about 30%.
+
+- Factor out the Python implementation of the BAYESTAR adaptive mesh refinement
+  algorithm so that other libraries can use it. It is exposed as
+  ``ligo.skymap.moc.bayestar_adaptive_grid``.
+
+- Fix incorrectly rendered default values for some command line arguments in
+  the documentation.
+
+- Move coherence plots from GWCelery to ligo.skymap.
+
 1.0.7 (2023-02-27)
 ==================
 
 - Track an API change in Matplotlib 3.7.0. Update test baseline images.
 
 - Update Linux wheels from manylinux2014 to manylinux_2_28.
```

### Comparing `ligo.skymap-1.0.7/CONTRIBUTING.rst` & `ligo.skymap-1.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/PKG-INFO` & `ligo.skymap-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ligo.skymap
-Version: 1.0.7
+Version: 1.1.0
 Summary: Tools for reading, writing, manipulating, and making LIGO and Virgo sky maps
 Home-page: https://lscsoft.docs.ligo.org/ligo.skymap/
 Author: Leo Singer
 Author-email: leo.singer@ligo.org
 License: GNU GPL v3+
 Project-URL: Bug Tracker, https://git.ligo.org/lscsoft/ligo.skymap/issues
 Project-URL: Change Log, https://lscsoft.docs.ligo.org/ligo.skymap/changes.html
@@ -12,18 +12,18 @@
 Project-URL: GitHub, https://github.com/lpsinger/ligo.skymap
 Project-URL: Source Code, https://git.ligo.org/lscsoft/ligo.skymap
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
+Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Description-Content-Type: text/x-rst
 Provides-Extra: test
```

### Comparing `ligo.skymap-1.0.7/README.rst` & `ligo.skymap-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/cextern/chealpix/chealpix.c` & `ligo.skymap-1.1.0/cextern/chealpix/chealpix.c`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/cextern/chealpix/chealpix.h` & `ligo.skymap-1.1.0/cextern/chealpix/chealpix.h`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/docs/Makefile` & `ligo.skymap-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/docs/_static/benchmark.svg` & `ligo.skymap-1.1.0/docs/_static/benchmark.svg`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/docs/_static/coinc.xml` & `ligo.skymap-1.1.0/docs/_static/coinc.xml`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/docs/_static/localization.svg` & `ligo.skymap-1.1.0/docs/_static/localization.svg`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/docs/bayestar/eggbox.png` & `ligo.skymap-1.1.0/docs/bayestar/eggbox.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/docs/changes.rst` & `ligo.skymap-1.1.0/docs/changes.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,55 @@
 #########
 Changelog
 #########
 
+1.1.0 (2023-07-07)
+==================
+
+- Add ``max_depth`` keyword argument to the call to
+  ``MOC.from_valued_healpix_cells`` in ``ligo-skymap-contour-moc``.
+  Contributed by `@parkma99 <https://github.com/parkma99>`_.
+
+- Improve handling of the ``--output`` command line argument for
+  ``ligo-skymap-contour-moc``:
+
+  - Add ``-o`` as a short form.
+
+  - Don't write to stdout by default; it does not make sense to write a binary
+    FITS file to stdout.
+
+  - Make the argument required.
+
+- Drop dependency on distutils to prepare for its removal in Python 3.12.
+  See `PEP 632 <https://peps.python.org/pep-0632/>`_.
+
+- Drop support for Python 3.8.
+
+- Vectorize ``find_ellipse`` over the ``cl`` argument.
+
+- Tune compiler settings used to build wheels for PyPI:
+
+  - Add the option ``-fvisibility=hidden`` to hide all symbols except for the
+    Python entry point. This improves the efficiency of link-time optimization.
+    On average, it speeds up BAYESTAR by about 5%.
+
+  - Add the options ``-Ofast -fno-finite-math-only -flto`` on Linux aarch64
+    and macOS, the targets on which we use gcc. These options approximate the
+    configuration that we use for icc on Linux x86_64. On average, this change
+    speeds up BAYESTAR on macOS by about 30%.
+
+- Factor out the Python implementation of the BAYESTAR adaptive mesh refinement
+  algorithm so that other libraries can use it. It is exposed as
+  ``ligo.skymap.moc.bayestar_adaptive_grid``.
+
+- Fix incorrectly rendered default values for some command line arguments in
+  the documentation.
+
+- Move coherence plots from GWCelery to ligo.skymap.
+
 1.0.7 (2023-02-27)
 ==================
 
 - Track an API change in Matplotlib 3.7.0. Update test baseline images.
 
 - Update Linux wheels from manylinux2014 to manylinux_2_28.
```

### Comparing `ligo.skymap-1.0.7/docs/conf.py` & `ligo.skymap-1.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/docs/contributing.rst` & `ligo.skymap-1.1.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/docs/develop.rst` & `ligo.skymap-1.1.0/docs/develop.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/docs/distance/index.rst` & `ligo.skymap-1.1.0/docs/distance/index.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/docs/help.rst` & `ligo.skymap-1.1.0/docs/help.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/docs/index.rst` & `ligo.skymap-1.1.0/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,15 @@
 -----------------------------------------------
 
 .. toctree::
    :maxdepth: 1
 
    plot/allsky
    plot/backdrop
+   plot/bayes_factor
    plot/marker
    plot/poly
    plot/pp
 
 Sky Map Postprocessing (`ligo.skymap.postprocess`)
 --------------------------------------------------
 
@@ -140,14 +141,15 @@
 .. toctree::
    :maxdepth: 1
 
    tool/ligo_skymap_contour
    tool/ligo_skymap_contour_moc
    tool/ligo_skymap_plot
    tool/ligo_skymap_plot_airmass
+   tool/ligo_skymap_plot_coherence
    tool/ligo_skymap_plot_observability
    tool/ligo_skymap_plot_volume
 
 Postprocessing
 --------------
 
 .. toctree::
```

### Comparing `ligo.skymap-1.0.7/docs/interface.rst` & `ligo.skymap-1.1.0/docs/interface.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/docs/io/events.rst` & `ligo.skymap-1.1.0/docs/io/events.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/docs/make.bat` & `ligo.skymap-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/docs/performance.rst` & `ligo.skymap-1.1.0/docs/performance.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/docs/quickstart/bayestar-injections.rst` & `ligo.skymap-1.1.0/docs/quickstart/bayestar-injections.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/docs/quickstart/install.rst` & `ligo.skymap-1.1.0/docs/quickstart/install.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 .. highlight:: sh
 
 Installation
 ============
 
-.. important:: The `ligo.skymap` package requires `Python`_ 3.8 or later.
+.. important:: The `ligo.skymap` package requires `Python`_ 3.9 or later.
 
 On Linux or macOS x86_64 systems, we recommend installing `ligo.skymap` using
 `pip`_ or `conda`_, either of which will automatically install all of the
 additional :ref:`Python dependencies <python-dependencies>`.
 
 (On other operating systems and architectures, you can :doc:`install from
 source <../develop>`.)
@@ -15,15 +15,15 @@
 Option 1: pip
 -------------
 
 To install `ligo.skymap` using `pip`_, you will need pip 19.3 or later. You can
 check what version of pip you have by running this command::
 
     $ pip --version
-    pip 20.0.2 from /usr/local/lib/python3.8/site-packages/pip (python 3.8)
+    pip 20.0.2 from /usr/local/lib/python3.9/site-packages/pip (python 3.9)
 
 If your version of pip is too old, then you can update pip to the most recent
 version by running this command::
 
     $ pip install --upgrade pip
 
 Then, just run this command::
```

### Comparing `ligo.skymap-1.0.7/docs/testing.rst` & `ligo.skymap-1.1.0/docs/testing.rst`

 * *Files 12% similar despite different names*

```diff
@@ -35,8 +35,8 @@
 GW170814 and GW170817 as well as populations of simulated events.
 
 .. _`Astropy Testing Guidelines`: https://docs.astropy.org/en/latest/development/testguide.html
 .. _`GitLab Continuous Integration (CI)`: https://docs.gitlab.com/ee/ci/
 .. _`.gitlab-ci.yml`: https://git.ligo.org/lscsoft/ligo.skymap/blob/main/.gitlab-ci.yml
 .. _`Astropy's documentation on running-tests`: https://docs.astropy.org/en/latest/development/testguide.html#running-tests
 .. _`coverage report`: https://lscsoft.docs.ligo.org/ligo.skymap/coverage.html
-.. _`acceptance tests`: https://git.ligo.org/lscsoft/ligo-skymap-acceptance-tests
+.. _`acceptance tests`: https://git.ligo.org/leo-singer/ligo-skymap-acceptance-tests-public
```

### Comparing `ligo.skymap-1.0.7/docs/tool/ligo_skymap_combine.rst` & `ligo.skymap-1.1.0/docs/tool/ligo_skymap_combine.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/docs/tool/ligo_skymap_constellations.rst` & `ligo.skymap-1.1.0/docs/tool/ligo_skymap_constellations.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/docs/tool/ligo_skymap_from_samples.rst` & `ligo.skymap-1.1.0/docs/tool/ligo_skymap_from_samples.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/docs/tool/ligo_skymap_plot.rst` & `ligo.skymap-1.1.0/docs/tool/ligo_skymap_plot.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/docs/tool/ligo_skymap_plot_airmass.rst` & `ligo.skymap-1.1.0/docs/tool/ligo_skymap_plot_airmass.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/docs/tool/ligo_skymap_plot_observability.rst` & `ligo.skymap-1.1.0/docs/tool/ligo_skymap_plot_observability.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/docs/tool/ligo_skymap_plot_volume.rst` & `ligo.skymap-1.1.0/docs/tool/ligo_skymap_plot_volume.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/licenses/CHEALPIX_LICENSE.rst` & `ligo.skymap-1.1.0/licenses/CHEALPIX_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/licenses/LICENSE.rst` & `ligo.skymap-1.1.0/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/licenses/NUMPY_LICENSE.rst` & `ligo.skymap-1.1.0/licenses/NUMPY_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/licenses/TEMPLATE_LICENCE.rst` & `ligo.skymap-1.1.0/licenses/TEMPLATE_LICENCE.rst`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/__init__.py` & `ligo.skymap-1.1.0/ligo/skymap/__init__.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/_astropy_init.py` & `ligo.skymap-1.1.0/ligo/skymap/_astropy_init.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/bayestar/__init__.py` & `ligo.skymap-1.1.0/ligo/skymap/bayestar/__init__.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/bayestar/ez_emcee.py` & `ligo.skymap-1.1.0/ligo/skymap/bayestar/ez_emcee.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/bayestar/filter.py` & `ligo.skymap-1.1.0/ligo/skymap/bayestar/filter.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/bayestar/interpolation.py` & `ligo.skymap-1.1.0/ligo/skymap/bayestar/interpolation.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/bayestar/ptemcee.py` & `ligo.skymap-1.1.0/ligo/skymap/bayestar/ptemcee.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/bayestar/tests/test_bayestar.py` & `ligo.skymap-1.1.0/ligo/skymap/bayestar/tests/test_bayestar.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/bayestar/tests/test_interpolation.py` & `ligo.skymap-1.1.0/ligo/skymap/bayestar/tests/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/bayestar/tests/test_signal_amplitude_model.py` & `ligo.skymap-1.1.0/ligo/skymap/bayestar/tests/test_signal_amplitude_model.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/conftest.py` & `ligo.skymap-1.1.0/ligo/skymap/conftest.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/coordinates/detector.py` & `ligo.skymap-1.1.0/ligo/skymap/coordinates/detector.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/coordinates/eigenframe.py` & `ligo.skymap-1.1.0/ligo/skymap/coordinates/eigenframe.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/coordinates/tests/test_detector.py` & `ligo.skymap-1.1.0/ligo/skymap/coordinates/tests/test_detector.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/distance.py` & `ligo.skymap-1.1.0/ligo/skymap/distance.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/extern/numpy/quantile.py` & `ligo.skymap-1.1.0/ligo/skymap/extern/numpy/quantile.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/healpix_tree.py` & `ligo.skymap-1.1.0/ligo/skymap/healpix_tree.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/io/events/base.py` & `ligo.skymap-1.1.0/ligo/skymap/io/events/base.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/io/events/detector_disabled.py` & `ligo.skymap-1.1.0/ligo/skymap/io/events/detector_disabled.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/io/events/gracedb.py` & `ligo.skymap-1.1.0/ligo/skymap/io/events/gracedb.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/io/events/hdf.py` & `ligo.skymap-1.1.0/ligo/skymap/io/events/hdf.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/io/events/ligolw.py` & `ligo.skymap-1.1.0/ligo/skymap/io/events/ligolw.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/io/events/magic.py` & `ligo.skymap-1.1.0/ligo/skymap/io/events/magic.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/io/events/sqlite.py` & `ligo.skymap-1.1.0/ligo/skymap/io/events/sqlite.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/io/fits.py` & `ligo.skymap-1.1.0/ligo/skymap/io/fits.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/io/hdf5.py` & `ligo.skymap-1.1.0/ligo/skymap/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/io/tests/data/2016_subset.xml.gz` & `ligo.skymap-1.1.0/ligo/skymap/io/tests/data/2016_subset.xml.gz`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/io/tests/data/G197392_coinc.xml.gz` & `ligo.skymap-1.1.0/ligo/skymap/io/tests/data/G197392_coinc.xml.gz`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/io/tests/data/G197392_psd.xml.gz` & `ligo.skymap-1.1.0/ligo/skymap/io/tests/data/G197392_psd.xml.gz`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/io/tests/data/G211117_coinc.xml.gz` & `ligo.skymap-1.1.0/ligo/skymap/io/tests/data/G211117_coinc.xml.gz`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/io/tests/data/G211117_psd.xml.gz` & `ligo.skymap-1.1.0/ligo/skymap/io/tests/data/G211117_psd.xml.gz`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/io/tests/data/gstlal_reference_psd/H1L1V1-REFERENCE_PSD-967234210-29963.xml.gz` & `ligo.skymap-1.1.0/ligo/skymap/io/tests/data/gstlal_reference_psd/H1L1V1-REFERENCE_PSD-967234210-29963.xml.gz`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/io/tests/data/test.hdf5` & `ligo.skymap-1.1.0/ligo/skymap/io/tests/data/test.hdf5`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/io/tests/test_io_events.py` & `ligo.skymap-1.1.0/ligo/skymap/io/tests/test_io_events.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/kde.py` & `ligo.skymap-1.1.0/ligo/skymap/kde.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,18 +15,15 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 
 import copyreg
 from functools import partial
 
-import astropy_healpix as ah
 from astropy.coordinates import SkyCoord
-from astropy.table import Table
-from astropy import units as u
 from astropy.utils.misc import NumpyRNGContext
 import healpy as hp
 import logging
 import numpy as np
 from scipy.stats import gaussian_kde
 
 from . import distance
@@ -318,56 +315,17 @@
             pts = self.transform(pts)
         super().__init__(
             pts, max_k=max_k, trials=trials, assign=assign, jobs=jobs)
 
     def __call__(self, pts):
         return super().__call__(self.transform(pts))
 
-    def _bayestar_adaptive_grid(self, top_nside=16, rounds=8):
-        """Implement of the BAYESTAR adaptive mesh refinement scheme as
-        described in Section VI of Singer & Price 2016, PRD, 93, 024013
-        :doi:`10.1103/PhysRevD.93.024013`.
-
-        FIXME: Consider refactoring BAYESTAR itself to perform the adaptation
-        step in Python.
-        """
-        top_npix = ah.nside_to_npix(top_nside)
-        nrefine = top_npix // 4
-        cells = zip([0] * nrefine, [top_nside // 2] * nrefine, range(nrefine))
-        for iround in range(rounds - 1):
-            print('adaptive refinement round {} of {} ...'.format(
-                  iround + 1, rounds - 1))
-            cells = sorted(cells, key=lambda p_n_i: p_n_i[0] / p_n_i[1]**2)
-            new_nside, new_ipix = np.transpose([
-                (nside * 2, ipix * 4 + i)
-                for _, nside, ipix in cells[-nrefine:] for i in range(4)])
-            theta, phi = hp.pix2ang(new_nside, new_ipix, nest=True)
-            ra = phi
-            dec = 0.5 * np.pi - theta
-            p = self(np.column_stack((ra, dec)))
-            cells[-nrefine:] = zip(p, new_nside, new_ipix)
-        return cells
-
-    def as_healpix(self, top_nside=16):
-        """Return a HEALPix multi-order map of the posterior density."""
-        post, nside, ipix = zip(*self._bayestar_adaptive_grid(
-            top_nside=top_nside))
-        post = np.asarray(list(post))
-        nside = np.asarray(list(nside))
-        ipix = np.asarray(list(ipix))
-
-        # Make sure that sky map is normalized (it should be already)
-        post /= np.sum(post * ah.nside_to_pixel_area(nside).to_value(u.sr))
-
-        # Convert from NESTED to UNIQ pixel indices
-        order = np.log2(nside).astype(int)
-        uniq = moc.nest2uniq(order.astype(np.int8), ipix)
-
-        # Done!
-        return Table([uniq, post], names=['UNIQ', 'PROBDENSITY'], copy=False)
+    def as_healpix(self, top_nside=16, rounds=8):
+        return moc.bayestar_adaptive_grid(self, top_nside=top_nside,
+                                          rounds=rounds)
 
 
 # We have to put in some hooks to make instances of Clustered2DSkyKDE picklable
 # because we dynamically create subclasses with different values of the 'frame'
 # class variable. This gets even trickier because we need both the class and
 # instance objects to be picklable.
```

### Comparing `ligo.skymap-1.0.7/ligo/skymap/moc.py` & `ligo.skymap-1.1.0/ligo/skymap/moc.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2017-2020  Leo Singer
+# Copyright (C) 2017-2023  Leo Singer
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -24,23 +24,25 @@
        grids." AA 580, A132. :doi:`10.1051/0004-6361/201526549`
 .. [2] Boch et al., 2014. "MOC - HEALPix Multi-Order Coverage map." IVOA
        Recommendation <http://ivoa.net/documents/MOC/>.
 
 """
 
 from astropy import table
+from astropy import units as u
+import astropy_healpix as ah
 import numpy as np
 from numpy.lib.recfunctions import repack_fields
 
 from .core import nest2uniq, uniq2nest, uniq2order, uniq2pixarea, uniq2ang
 from .core import rasterize as _rasterize
 from .util.numpy import add_newdoc_ufunc, require_contiguous_aligned
 
 __all__ = ('nest2uniq', 'uniq2nest', 'uniq2order', 'uniq2pixarea',
-           'uniq2ang', 'rasterize')
+           'uniq2ang', 'rasterize', 'bayestar_adaptive_grid')
 
 
 add_newdoc_ufunc(nest2uniq, """\
 Convert a pixel index from NESTED to NUNIQ ordering.
 
 Parameters
 ----------
@@ -157,8 +159,70 @@
     # Ensure that moc_data has appropriate padding for each of its columns to
     # be properly aligned in order to avoid undefined behavior.
     moc_data = repack_fields(np.asarray(moc_data), align=True)
 
     return _rasterize(moc_data, order=order)
 
 
+def bayestar_adaptive_grid(probdensity, *args, top_nside=16, rounds=8,
+                           **kwargs):
+    """Create a sky map by evaluating a function on an adaptive grid.
+
+    Perform the BAYESTAR adaptive mesh refinement scheme as described in
+    Section VI of Singer & Price 2016, PRD, 93, 024013
+    :doi:`10.1103/PhysRevD.93.024013`. This computes the sky map
+    using a provided analytic function and refines the grid, dividing the
+    highest 25% into subpixels and then recalculating their values. The extra
+    given args and kwargs will be passed to the given probdensity function.
+
+    Parameters
+    ----------
+    probdensity : callable
+        Probability density function. The first argument consists of
+        column-stacked array of right ascension and declination in radians.
+        The return value must be a 1D array of the probability density in
+        inverse steradians with the same length as the argument.
+    top_nside : int
+        HEALPix NSIDE resolution of initial evaluation of the sky map
+    rounds : int
+        Number of refinement rounds, including the initial sky map evaluation
+
+    Returns
+    -------
+    skymap : astropy.table.Table
+        An astropy Table with UNIQ and PROBDENSITY columns, representing
+        a multi-ordered sky map
+    """
+    top_npix = ah.nside_to_npix(top_nside)
+    nrefine = top_npix // 4
+    cells = zip([0] * nrefine, [top_nside // 2] * nrefine, range(nrefine))
+    for iround in range(rounds + 1):
+        print('adaptive refinement round {} of {} ...'.format(
+            iround, rounds))
+        cells = sorted(cells, key=lambda p_n_i: p_n_i[0] / p_n_i[1]**2)
+        new_nside, new_ipix = np.transpose([
+            (nside * 2, ipix * 4 + i)
+            for _, nside, ipix in cells[-nrefine:] for i in range(4)])
+        ra, dec = ah.healpix_to_lonlat(new_ipix, new_nside, order='nested')
+        p = probdensity(np.column_stack((ra.value, dec.value)),
+                        *args, **kwargs)
+        cells[-nrefine:] = zip(p, new_nside, new_ipix)
+
+    """Return a HEALPix multi-order map of the posterior density."""
+    post, nside, ipix = zip(*cells)
+    post = np.asarray(list(post))
+    nside = np.asarray(list(nside))
+    ipix = np.asarray(list(ipix))
+
+    # Make sure that sky map is normalized (it should be already)
+    post /= np.sum(post * ah.nside_to_pixel_area(nside).to_value(u.sr))
+
+    # Convert from NESTED to UNIQ pixel indices
+    order = np.log2(nside).astype(int)
+    uniq = nest2uniq(order.astype(np.int8), ipix)
+
+    # Done!
+    return table.Table([uniq, post], names=['UNIQ', 'PROBDENSITY'],
+                       copy=False)
+
+
 del add_newdoc_ufunc, require_contiguous_aligned
```

### Comparing `ligo.skymap-1.0.7/ligo/skymap/plot/allsky.py` & `ligo.skymap-1.1.0/ligo/skymap/plot/allsky.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/plot/angle.py` & `ligo.skymap-1.1.0/ligo/skymap/plot/angle.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/plot/backdrop.py` & `ligo.skymap-1.1.0/ligo/skymap/plot/backdrop.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/plot/cmap.py` & `ligo.skymap-1.1.0/ligo/skymap/plot/cmap.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/plot/cylon.csv` & `ligo.skymap-1.1.0/ligo/skymap/plot/cylon.csv`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/plot/cylon.py` & `ligo.skymap-1.1.0/ligo/skymap/plot/cylon.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/plot/marker.py` & `ligo.skymap-1.1.0/ligo/skymap/plot/marker.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/plot/ne_simplified_coastline.json` & `ligo.skymap-1.1.0/ligo/skymap/plot/ne_simplified_coastline.json`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/plot/poly.py` & `ligo.skymap-1.1.0/ligo/skymap/plot/poly.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/plot/pp.py` & `ligo.skymap-1.1.0/ligo/skymap/plot/pp.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-degrees-aitoff.png` & `ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-degrees-aitoff.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-degrees-mollweide.png` & `ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-degrees-mollweide.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-hours-aitoff.png` & `ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-hours-aitoff.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-hours-mollweide.png` & `ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-hours-mollweide.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-degrees-aitoff.png` & `ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-degrees-aitoff.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-degrees-mollweide.png` & `ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-degrees-mollweide.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-hours-aitoff.png` & `ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-hours-aitoff.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-hours-mollweide.png` & `ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-hours-mollweide.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-degrees-aitoff.png` & `ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-degrees-aitoff.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-degrees-mollweide.png` & `ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-degrees-mollweide.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-hours-aitoff.png` & `ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-hours-aitoff.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-hours-mollweide.png` & `ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-hours-mollweide.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/plot/tests/baseline/test_allsky_obstime.png` & `ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_allsky_obstime.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/plot/tests/baseline/test_globe_axes.png` & `ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_globe_axes.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/plot/tests/baseline/test_pp_plot_default.png` & `ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_pp_plot_default.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/plot/tests/baseline/test_pp_plot_lines.png` & `ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_pp_plot_lines.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/plot/tests/baseline/test_pp_plot_steps.png` & `ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_pp_plot_steps.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/plot/tests/baseline/test_reticle.png` & `ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_reticle.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/plot/tests/baseline/test_zoom_axes.png` & `ligo.skymap-1.1.0/ligo/skymap/plot/tests/baseline/test_zoom_axes.png`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/plot/tests/test_plot.py` & `ligo.skymap-1.1.0/ligo/skymap/plot/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/plot/util.py` & `ligo.skymap-1.1.0/ligo/skymap/plot/util.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/postprocess/contour.py` & `ligo.skymap-1.1.0/ligo/skymap/postprocess/contour.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/postprocess/cosmology.py` & `ligo.skymap-1.1.0/ligo/skymap/postprocess/cosmology.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2013-2021  Leo Singer, Rainer Corley
+# Copyright (C) 2013-2023  Leo Singer, Rainer Corley
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -58,21 +58,16 @@
     ret *= np.square(zplus1)
     return 1.0 / ret
 
 
 @np.vectorize
 def z_for_DL(DL):
     """Redshift as a function of luminosity distance in Mpc."""
-    # FIXME: In Astropy 4, `z_at_value` returns a float,
-    # but in Astropy 5, returns a quantity with dimensionless redshift units.
-    # Make sure it is a quantity before we convert it to a float.
-    # Remove the u.Quantity() call once we drop support for astropy < 5.
-    return u.Quantity(
-        z_at_value(cosmo.luminosity_distance, DL * u.Mpc)
-    ).to_value(u.dimensionless_unscaled)
+    return z_at_value(cosmo.luminosity_distance, DL * u.Mpc).to_value(
+        u.dimensionless_unscaled)
 
 
 def dVC_dVL_for_DL(DL):
     """Same as :meth:`dVC_dVL_for_z`, but as a function of luminosity
     distance.
     """
     return dVC_dVL_for_z(z_for_DL(DL))
```

### Comparing `ligo.skymap-1.0.7/ligo/skymap/postprocess/crossmatch.py` & `ligo.skymap-1.1.0/ligo/skymap/postprocess/crossmatch.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/postprocess/ellipse.py` & `ligo.skymap-1.1.0/ligo/skymap/postprocess/ellipse.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2013-2020  Leo Singer
+# Copyright (C) 2013-2023  Leo Singer
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -40,35 +40,35 @@
     Aladin drawing commands [2]_.
 
     Parameters
     ----------
     prob : np.ndarray, astropy.table.Table
         The HEALPix probability map, either as a full rank explicit array
         or as a multi-order map.
-    cl : float
-        The desired credible level (default: 90).
+    cl : float, np.ndarray
+        The desired credible level or levels (default: 90).
     projection : str, optional
         The WCS projection (default: 'ARC', or zenithal equidistant).
         For a list of possible values, see the Astropy documentation [3]_.
     nest : bool
         HEALPix pixel ordering (default: False, or ring ordering).
 
     Returns
     -------
     ra : float
         The ellipse center right ascension in degrees.
     dec : float
         The ellipse center right ascension in degrees.
-    a : float
+    a : float, np.ndarray
         The lenth of the semimajor axis in degrees.
-    b : float
+    b : float, np.ndarray
         The length of the semiminor axis in degrees.
     pa : float
         The orientation of the ellipse axis on the plane of the sky in degrees.
-    area : float
+    area : float, np.ndarray
         The area of the ellipse in square degrees.
 
     Notes
     -----
     The center of the ellipse is the median a posteriori sky position. The
     length and orientation of the semi-major and semi-minor axes are measured
     as follows:
@@ -83,14 +83,18 @@
     3. The 1-sigma ellipse is inflated until it encloses an integrated
        probability of ``cl`` (default: 90%).
 
     The function returns a tuple of the right ascension, declination,
     semi-major distance, semi-minor distance, and orientation angle, all in
     degrees.
 
+    If no ellipse can be found that contains integrated probability greater
+    than or equal to the desired credible level ``cl``, then the return values
+    ``a``, ``b``, and ``area`` will be set to nan.
+
     References
     ----------
     .. [1] http://ds9.si.edu/doc/ref/region.html
     .. [2] http://aladin.u-strasbg.fr/java/AladinScriptManual.gml#draw
     .. [3] http://docs.astropy.org/en/stable/wcs/index.html#supported-projections
 
     Examples
@@ -301,14 +305,23 @@
     ...     [[0.1, 0, 0],
     ...      [0, 1, -0.15],
     ...      [0, -0.15, 0.1]])
     ...
     >>> find_ellipse(prob)  # doctest: +FLOAT_CMP
     (0.0, 0.0, 64.77564486039148, 33.50986301851987, 9.217477126726322, 6372.42573159241)
 
+    ***Example 5***
+
+    You can ask for other credible levels:
+    >>> find_ellipse(prob, cl=50)  # doctest: +FLOAT_CMP
+    (0.0, 0.0, 37.054207653285076, 19.168955020015982, 9.217477126726322, 2182.5580135410632)
+
+    Or even for multiple credible levels:
+    >>> find_ellipse(prob, cl=[50, 90])  # doctest: +FLOAT_CMP
+    (0.0, 0.0, array([37.05420765, 64.77564486]), array([19.16895502, 33.50986302]), 9.217477126726322, array([2182.55801354, 6372.42573159]))
     """  # noqa: E501
     try:
         prob['UNIQ']
     except (IndexError, KeyError, ValueError):
         npix = len(prob)
         nside = ah.npix_to_nside(npix)
         ipix = range(npix)
@@ -329,15 +342,15 @@
 
     # Construct WCS with the specified projection
     # and centered on mean direction.
     w = WCS()
     w.wcs.crval = [ra, dec]
     w.wcs.ctype = ['RA---' + projection, 'DEC--' + projection]
 
-    # Transform HEALPix to zenithal equidistant coordinates.
+    # Transform HEALPix to the specified projection.
     xy = w.wcs_world2pix(
         np.transpose(
             hp.pix2ang(
                 nside, ipix, nest=nest, lonlat=True)), 1)
 
     # Keep only values that were inside the projection.
     keep = np.logical_and.reduce(np.isfinite(xy), axis=1)
@@ -358,27 +371,24 @@
     i = np.argsort(nsigmas)
     nsigmas = nsigmas[i]
     cls = np.cumsum(prob[i])
     if np.isscalar(area):
         careas = np.arange(1, len(i) + 1) * area
     else:
         careas = np.cumsum(area[i])
-    nsigma = np.interp(1e-2 * cl, cls, nsigmas)
-    area = np.interp(1e-2 * cl, cls, careas)
-
-    # If the credible level is not within the projection,
-    # then stop here and return all nans.
-    if 1e-2 * cl > cls[-1]:
-        return np.nan, np.nan, np.nan, np.nan, np.nan, np.nan
+    # np.multiply rather than * to automatically convert to ndarray if needed
+    cl = np.multiply(cl, 1e-2)
+    nsigma = np.interp(cl, cls, nsigmas, right=np.nan)
+    area = np.interp(cl, cls, careas, right=np.nan)
 
     # Find the eigendecomposition of the covariance matrix.
     w, v = np.linalg.eigh(c)
 
     # Find the semi-minor and semi-major axes.
-    b, a = nsigma * np.sqrt(w)
+    b, a = (nsigma * root_w for root_w in np.sqrt(w))
 
     # Find the position angle.
     pa = np.rad2deg(np.arctan2(*v[0]))
 
     # An ellipse is symmetric under rotations of 180°.
     # Return the smallest possible positive position angle.
     pa %= 180
```

### Comparing `ligo.skymap-1.0.7/ligo/skymap/postprocess/tests/test_cosmology.py` & `ligo.skymap-1.1.0/ligo/skymap/postprocess/tests/test_cosmology.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/postprocess/tests/test_crossmatch.py` & `ligo.skymap-1.1.0/ligo/skymap/postprocess/tests/test_crossmatch.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/postprocess/util.py` & `ligo.skymap-1.1.0/ligo/skymap/postprocess/util.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/tests/plugins/omp.py` & `ligo.skymap-1.1.0/ligo/skymap/tests/plugins/omp.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/tests/test_moc.py` & `ligo.skymap-1.1.0/ligo/skymap/tests/test_moc.py`

 * *Files 7% similar despite different names*

```diff
@@ -126,7 +126,23 @@
 
 @pytest.mark.parametrize('order', range(3))
 def test_rasterize_default(order):
     npix = ah.nside_to_npix(ah.level_to_nside(order))
     skymap_in = input_skymap(order, 0, 0)
     skymap_out = moc.rasterize(skymap_in)
     assert len(skymap_out) == npix
+
+
+def prob_test(pts):
+    ras, decs = np.hsplit(pts, 2)
+    return ras + decs
+
+
+@pytest.mark.parametrize('order', range(1, 4))
+@pytest.mark.parametrize('round', range(3))
+def test_bayestar_adaptive_grid(order, round):
+    nside = ah.level_to_nside(order)
+    npix = ah.nside_to_npix(nside) * (1 + .75 * round)
+
+    skymap_out = moc.bayestar_adaptive_grid(
+        prob_test, top_nside=nside, rounds=round)
+    assert len(skymap_out) == npix
```

### Comparing `ligo.skymap-1.0.7/ligo/skymap/tool/__init__.py` & `ligo.skymap-1.1.0/ligo/skymap/tool/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2013-2022  Leo Singer
+# Copyright (C) 2013-2023  Leo Singer
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -13,16 +13,14 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 """Functions that support the command line interface."""
 
 import argparse
-from distutils.dir_util import mkpath
-from distutils.errors import DistutilsFileError
 import glob
 import inspect
 import itertools
 import logging
 import os
 import sys
 
@@ -111,73 +109,76 @@
             msg += ', but found '
             msg += '{} file'.format(nvalues)
             if nvalues != 1:
                 msg += 's'
             raise argparse.ArgumentError(self, msg)
 
 
-waveform_parser = argparse.ArgumentParser(add_help=False)
-group = waveform_parser.add_argument_group(
-    'waveform options', 'Options that affect template waveform generation')
-# FIXME: The O1 uberbank high-mass template, SEOBNRv2_ROM_DoubleSpin, does
-# not support frequencies less than 30 Hz.
-group.add_argument(
-    '--f-low', type=float, metavar='Hz', default=30,
-    help='Low frequency cutoff')
-group.add_argument(
-    '--f-high-truncate', type=float, default=0.95,
-    help='Truncate waveform at this fraction of the maximum frequency of the '
-    'PSD')
-group.add_argument(
-    '--waveform', default='o2-uberbank',
-    help='Template waveform approximant: e.g., TaylorF2threePointFivePN')
-del group
-
-
-posterior_parser = argparse.ArgumentParser(add_help=False)
-group = posterior_parser.add_argument_group(
-    'posterior options', 'Options that affect the BAYESTAR posterior')
-group.add_argument(
-    '--min-inclination', type=float, metavar='deg', default=0.0,
-    help='Minimum inclination in degrees')
-group.add_argument(
-    '--max-inclination', type=float, metavar='deg', default=90.0,
-    help='Maximum inclination in degrees')
-group.add_argument(
-    '--min-distance', type=float, metavar='Mpc',
-    help='Minimum distance of prior in megaparsecs')
-group.add_argument(
-    '--max-distance', type=float, metavar='Mpc',
-    help='Maximum distance of prior in megaparsecs')
-group.add_argument(
-    '--prior-distance-power', type=int, metavar='-1|2', default=2,
-    help='Distance prior: -1 for uniform in log, 2 for uniform in volume')
-group.add_argument(
-    '--cosmology', action='store_true',
-    help='Use cosmological comoving volume prior')
-group.add_argument(
-    '--enable-snr-series', action=EnableAction,
-    help='Enable input of SNR time series')
-group.add_argument(
-    '--rescale-loglikelihood', type=float, default=0.83,
-    help='Rescale log likelihood by the square of this factor to account for '
-    'excess technical noise from search pipeline')
-del group
-
-
-mcmc_parser = argparse.ArgumentParser(add_help=False)
-group = mcmc_parser.add_argument_group(
-    'BAYESTAR MCMC options', 'BAYESTAR options for MCMC sampling')
-group.add_argument(
-    '--mcmc', action='store_true',
-    help='Use MCMC sampling instead of Gaussian quadrature')
-group.add_argument(
-    '--chain-dump', action='store_true',
-    help='For MCMC methods, dump the sample chain to disk')
-del group
+def get_waveform_parser():
+    parser = argparse.ArgumentParser(add_help=False)
+    group = parser.add_argument_group(
+        'waveform options', 'Options that affect template waveform generation')
+    # FIXME: The O1 uberbank high-mass template, SEOBNRv2_ROM_DoubleSpin, does
+    # not support frequencies less than 30 Hz.
+    group.add_argument(
+        '--f-low', type=float, metavar='Hz', default=30,
+        help='Low frequency cutoff')
+    group.add_argument(
+        '--f-high-truncate', type=float, default=0.95,
+        help='Truncate waveform at this fraction of the maximum frequency of '
+        'the PSD')
+    group.add_argument(
+        '--waveform', default='o2-uberbank',
+        help='Template waveform approximant: e.g., TaylorF2threePointFivePN')
+    return parser
+
+
+def get_posterior_parser():
+    parser = argparse.ArgumentParser(add_help=False)
+    group = parser.add_argument_group(
+        'posterior options', 'Options that affect the BAYESTAR posterior')
+    group.add_argument(
+        '--min-inclination', type=float, metavar='deg', default=0.0,
+        help='Minimum inclination in degrees')
+    group.add_argument(
+        '--max-inclination', type=float, metavar='deg', default=90.0,
+        help='Maximum inclination in degrees')
+    group.add_argument(
+        '--min-distance', type=float, metavar='Mpc',
+        help='Minimum distance of prior in megaparsecs')
+    group.add_argument(
+        '--max-distance', type=float, metavar='Mpc',
+        help='Maximum distance of prior in megaparsecs')
+    group.add_argument(
+        '--prior-distance-power', type=int, metavar='-1|2', default=2,
+        help='Distance prior: -1 for uniform in log, 2 for uniform in volume')
+    group.add_argument(
+        '--cosmology', action='store_true',
+        help='Use cosmological comoving volume prior')
+    group.add_argument(
+        '--enable-snr-series', action=EnableAction,
+        help='Enable input of SNR time series')
+    group.add_argument(
+        '--rescale-loglikelihood', type=float, default=0.83,
+        help='Rescale log likelihood by the square of this factor to account '
+        'for excess technical noise from search pipeline')
+    return parser
+
+
+def get_mcmc_parser():
+    parser = argparse.ArgumentParser(add_help=False)
+    group = parser.add_argument_group(
+        'BAYESTAR MCMC options', 'BAYESTAR options for MCMC sampling')
+    group.add_argument(
+        '--mcmc', action='store_true',
+        help='Use MCMC sampling instead of Gaussian quadrature')
+    group.add_argument(
+        '--chain-dump', action='store_true',
+        help='For MCMC methods, dump the sample chain to disk')
+    return parser
 
 
 class HelpChoicesAction(argparse.Action):
 
     def __init__(self,
                  option_strings,
                  choices=(),
@@ -234,21 +235,23 @@
 
 
 @type_with_sideeffect(int)
 def seed(value):
     np.random.seed(value)
 
 
-random_parser = argparse.ArgumentParser(add_help=False)
-group = random_parser.add_argument_group(
-    'random number generator options',
-    'Options that affect the Numpy pseudo-random number genrator')
-group.add_argument(
-    '--seed', type=seed, help='Pseudo-random number generator seed '
-    '[default: initialized from /dev/urandom or clock]')
+def get_random_parser():
+    parser = argparse.ArgumentParser(add_help=False)
+    group = parser.add_argument_group(
+        'random number generator options',
+        'Options that affect the Numpy pseudo-random number genrator')
+    group.add_argument(
+        '--seed', type=seed, help='Pseudo-random number generator seed '
+        '[default: initialized from /dev/urandom or clock]')
+    return parser
 
 
 class HelpFormatter(argparse.RawDescriptionHelpFormatter,
                     argparse.ArgumentDefaultsHelpFormatter):
     pass
 
 
@@ -310,16 +313,16 @@
 
     def __init__(self, create=False):
         self._create = create
 
     def __call__(self, string):
         if self._create:
             try:
-                mkpath(string)
-            except DistutilsFileError as e:
+                os.makedirs(string, exist_ok=True)
+            except OSError as e:
                 raise argparse.ArgumentTypeError(e.message)
         else:
             try:
                 os.listdir(string)
             except OSError as e:
                 raise argparse.ArgumentTypeError(e)
         return string
```

### Comparing `ligo.skymap-1.0.7/ligo/skymap/tool/bayestar_inject.py` & `ligo.skymap-1.1.0/ligo/skymap/tool/bayestar_inject.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2019-2022  Leo Singer
+# Copyright (C) 2019-2023  Leo Singer
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -39,15 +39,16 @@
 from scipy.interpolate import interp1d
 from scipy.optimize import root_scalar
 from scipy.ndimage import maximum_filter
 
 from ..util import progress_map
 from ..bayestar.filter import sngl_inspiral_psd
 from . import (
-    ArgumentParser, FileType, random_parser, register_to_xmldoc, write_fileobj)
+    ArgumentParser, FileType, get_random_parser, register_to_xmldoc,
+    write_fileobj)
 
 try:
     from astropy.cosmology import available as available_cosmologies
 except ImportError:
     # FIXME: Remove once we drop support for Astropy < 5.1
     from astropy.cosmology.parameters import available as available_cosmologies
 
@@ -228,15 +229,15 @@
 
 
 def assert_not_reached():  # pragma: no cover
     raise AssertionError('This line should not be reached.')
 
 
 def parser():
-    parser = ArgumentParser(parents=[random_parser])
+    parser = ArgumentParser(parents=[get_random_parser()])
     parser.add_argument(
         '--cosmology', choices=available_cosmologies,
         default='Planck15', help='Cosmological model')
 
     group = parser.add_mutually_exclusive_group(required=True)
     group.add_argument(
         '--distribution', help='Use a preset distribution', choices=(
```

### Comparing `ligo.skymap-1.0.7/ligo/skymap/tool/bayestar_localize_coincs.py` & `ligo.skymap-1.1.0/ligo/skymap/tool/bayestar_localize_coincs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2013-2020  Leo Singer
+# Copyright (C) 2013-2023  Leo Singer
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -28,29 +28,29 @@
 
 A FITS file is created for each sky map, having a filename of the form
 ``X.fits`` where X is the integer LIGO-LW row ID of the coinc. The ``OBJECT``
 card in the FITS header is also set to the integer row ID.
 """
 
 from . import (
-    ArgumentParser, FileType, mkpath,
-    waveform_parser, posterior_parser, mcmc_parser, random_parser)
+    ArgumentParser, FileType, get_waveform_parser, get_posterior_parser,
+    get_mcmc_parser, get_random_parser)
 
 
 ROW_ID_COMMENT = [
     '',
     'The integer value in the OBJECT card in this FITS header is a row ID',
     'that refers to a coinc_event table row in the input LIGO-LW document.',
     '']
 
 
 def parser():
     parser = ArgumentParser(
-        parents=[waveform_parser, posterior_parser, mcmc_parser,
-                 random_parser])
+        parents=[get_waveform_parser(), get_posterior_parser(),
+                 get_mcmc_parser(), get_random_parser()])
     parser.add_argument(
         '-d', '--disable-detector', metavar='X1', type=str, nargs='+',
         help='disable certain detectors')
     parser.add_argument(
         '--keep-going', '-k', default=False, action='store_true',
         help='Keep processing events if a sky map fails to converge')
     parser.add_argument(
@@ -106,15 +106,15 @@
         '%s:reading input files', ','.join(file.name for file in opts.input))
     event_source = events.open(*opts.input, sample=opts.pycbc_sample)
 
     if opts.disable_detector:
         event_source = events.detector_disabled.open(
             event_source, opts.disable_detector)
 
-    mkpath(opts.output)
+    os.makedirs(opts.output, exist_ok=True)
 
     if opts.condor_submit:
         if opts.seed is not None:
             raise NotImplementedError(
                 '--seed does not yet work with --condor-submit')
         if opts.coinc_event_id:
             raise ValueError(
```

### Comparing `ligo.skymap-1.0.7/ligo/skymap/tool/bayestar_localize_lvalert.py` & `ligo.skymap-1.1.0/ligo/skymap/tool/bayestar_localize_lvalert.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2013-2020  Leo Singer
+# Copyright (C) 2013-2023  Leo Singer
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -27,22 +27,22 @@
 
     $ mkfifo /var/run/bayestar
     $ tail -F /var/run/bayestar | bayestar_localize_lvalert &
     $ echo T90713 > /var/run/bayestar
 """
 
 from . import (
-    ArgumentParser, EnableAction, waveform_parser, posterior_parser,
-    mcmc_parser, random_parser, iterlines)
+    ArgumentParser, EnableAction, get_waveform_parser, get_posterior_parser,
+    get_mcmc_parser, get_random_parser, iterlines)
 
 
 def parser():
     parser = ArgumentParser(
-        parents=[waveform_parser, posterior_parser, mcmc_parser,
-                 random_parser])
+        parents=[get_waveform_parser(), get_posterior_parser(),
+                 get_mcmc_parser(), get_random_parser()])
     parser.add_argument(
         '-d', '--disable-detector', metavar='X1', type=str, nargs='+',
         help='disable certain detectors')
     parser.add_argument(
         '-N', '--dry-run', action='store_true',
         help='Dry run; do not update GraceDB entry')
     parser.add_argument(
```

### Comparing `ligo.skymap-1.0.7/ligo/skymap/tool/bayestar_mcmc.py` & `ligo.skymap-1.1.0/ligo/skymap/tool/bayestar_mcmc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2013-2020  Leo Singer
+# Copyright (C) 2013-2023  Leo Singer
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -13,21 +13,22 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 """Markov-Chain Monte Carlo sky localization."""
 
 from . import (
-    ArgumentParser, FileType, waveform_parser,
-    posterior_parser, random_parser, mkpath)
+    ArgumentParser, FileType, get_waveform_parser,
+    get_posterior_parser, get_random_parser)
 
 
 def parser():
-    parser = ArgumentParser(parents=[waveform_parser, posterior_parser,
-                                     random_parser])
+    parser = ArgumentParser(parents=[get_waveform_parser(),
+                                     get_posterior_parser(),
+                                     get_random_parser()])
     parser.add_argument(
         'input', metavar='INPUT.{hdf,xml,xml.gz,sqlite}', default='-',
         nargs='+', type=FileType('rb'),
         help='Input LIGO-LW XML file, SQLite file, or PyCBC HDF5 files. '
              'For PyCBC, you must supply the coincidence file '
              '(e.g. "H1L1-HDFINJFIND.hdf" or "H1L1-STATMAP.hdf"), '
              'the template bank file (e.g. H1L1-BANK2HDF.hdf), '
@@ -88,15 +89,15 @@
     import lal
 
     # Read coinc file.
     log.info(
         '%s:reading input files', ','.join(file.name for file in opts.input))
     event_source = events.open(*opts.input, sample=opts.pycbc_sample)
 
-    mkpath(opts.output)
+    os.makedirs(opts.output, exist_ok=True)
 
     if opts.condor_submit:
         if opts.seed is not None:
             raise NotImplementedError(
                 '--seed does not yet work with --condor-submit')
         if opts.coinc_event_id:
             raise ValueError(
```

### Comparing `ligo.skymap-1.0.7/ligo/skymap/tool/bayestar_realize_coincs.py` & `ligo.skymap-1.1.0/ligo/skymap/tool/bayestar_realize_coincs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2013-2022  Leo Singer
+# Copyright (C) 2013-2023  Leo Singer
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -31,24 +31,24 @@
 import copy
 import functools
 
 import lal
 import numpy as np
 
 from . import (
-    ArgumentParser, EnableAction, FileType, random_parser, register_to_xmldoc,
-    write_fileobj)
+    ArgumentParser, EnableAction, FileType, get_random_parser,
+    register_to_xmldoc, write_fileobj)
 
 
 def parser():
     # Determine list of known detectors for command line arguments.
     available_ifos = sorted(det.frDetector.prefix
                             for det in lal.CachedDetectors)
 
-    parser = ArgumentParser(parents=[random_parser])
+    parser = ArgumentParser(parents=[get_random_parser()])
     parser.add_argument(
         'input', metavar='IN.xml[.gz]', type=FileType('rb'),
         default='-', help='Name of input file')
     parser.add_argument(
         '-o', '--output', metavar='OUT.xml[.gz]', type=FileType('wb'),
         default='-', help='Name of output file')
     parser.add_argument(
```

### Comparing `ligo.skymap-1.0.7/ligo/skymap/tool/bayestar_sample_model_psd.py` & `ligo.skymap-1.1.0/ligo/skymap/tool/bayestar_sample_model_psd.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/tool/ligo_skymap_combine.py` & `ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_combine.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/tool/ligo_skymap_constellations.py` & `ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_constellations.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/tool/ligo_skymap_contour.py` & `ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_contour.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/tool/ligo_skymap_contour_moc.py` & `ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_contour_moc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2013-2020 Giuseppe Greco, Leo Singer, and CDS team.
+# Copyright (C) 2013-2023 Giuseppe Greco, Leo Singer, and CDS team.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -22,16 +22,16 @@
 from . import ArgumentParser, FileType
 
 
 def parser():
     parser = ArgumentParser()
 
     parser.add_argument(
-        '--output', metavar='FILE.fits',
-        default='-', type=str, help='output file [default: stdout]')
+        '-o', '--output', metavar='FILE.fits', required=True,
+        help='output file')
     parser.add_argument(
         '-c', '--contour', metavar='PERCENT', type=float, required=True,
         help='MOC region enclosing this percentage of probability \
               [range is 0-100]')
     parser.add_argument(
         'input', metavar='INPUT.fits[.gz]', type=FileType('rb'),
         default='-', nargs='?', help='Input multi-order or flatten \
@@ -66,11 +66,12 @@
         ah.level_to_nside(level)).to_value(u.steradian)
 
     prob = probdensity * area
 
     # Create MOC
     contour_decimal = opts.contour / 100
     moc = MOC.from_valued_healpix_cells(
-        uniq, prob, cumul_from=0.0, cumul_to=contour_decimal)
+        uniq, prob, max_depth=level.max(),
+        cumul_from=0.0, cumul_to=contour_decimal)
 
     # Write MOC
     moc.write(opts.output, format='fits', overwrite=True)
```

### Comparing `ligo.skymap-1.0.7/ligo/skymap/tool/ligo_skymap_flatten.py` & `ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_flatten.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/tool/ligo_skymap_from_samples.py` & `ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_from_samples.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2011-2020  Will M. Farr <will.farr@ligo.org>
+# Copyright (C) 2011-2023  Will M. Farr <will.farr@ligo.org>
 #                          Leo P. Singer <leo.singer@ligo.org>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
@@ -15,29 +15,38 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 """
 Generate a FITS sky map file from posterior samples using clustering and
 kernel density estimation.
 
+The input file should be an HDF5 file with the following columns:
+
+*  ``ra``, ``rightascension``, or ``right_ascension``: J2000 right ascension in
+    radians
+*  ``dec`` or ``declination``: J200 declination in radians
+*  ``dist``, ``distance``, or ``luminosity_distance``: luminosity distance in
+   Mpc (optional)
+
 The output consist of two files:
 
 *  ``skypost.obj``, a :mod:`pickle` representation of the kernel density
    estimator
 *  ``skymap.fits.gz``, a 3D localization in HEALPix/FITS format
 """
 
 from argparse import SUPPRESS
 
-from . import ArgumentParser, DirType, EnableAction, FileType, random_parser
+from . import (
+    ArgumentParser, DirType, EnableAction, FileType, get_random_parser)
 
 
 def parser():
     # Command line interface.
-    parser = ArgumentParser(parents=[random_parser])
+    parser = ArgumentParser(parents=[get_random_parser()])
     parser.add_argument('samples', type=FileType('rb'), metavar='SAMPLES.hdf5',
                         help='posterior samples file')
     # Only present for backward compatibility with --samples syntax
     parser.add_argument('--samples', action='store_false', dest='_ignored',
                         help=SUPPRESS)
     parser.add_argument('--outdir', '-o', default='.',
                         type=DirType(create=True), help='output directory')
```

### Comparing `ligo.skymap-1.0.7/ligo/skymap/tool/ligo_skymap_plot.py` & `ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,19 +23,19 @@
 
 Public-domain cartographic data is courtesy of `Natural Earth
 <http://www.naturalearthdata.com>`_ and processed with `MapShaper
 <http://www.mapshaper.org>`_.
 """
 
 from . import ArgumentParser, FileType, SQLiteType
-from .matplotlib import figure_parser
+from .matplotlib import get_figure_parser
 
 
 def parser():
-    parser = ArgumentParser(parents=[figure_parser])
+    parser = ArgumentParser(parents=[get_figure_parser()])
     parser.add_argument(
         '--annotate', default=False, action='store_true',
         help='annotate plot with information about the event')
     parser.add_argument(
         '--contour', metavar='PERCENT', type=float, nargs='+',
         help='plot contour enclosing this percentage of'
         ' probability mass [may be specified multiple times, default: none]')
```

### Comparing `ligo.skymap-1.0.7/ligo/skymap/tool/ligo_skymap_plot_airmass.py` & `ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_plot_airmass.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2018-2020  Leo Singer
+# Copyright (C) 2018-2023  Leo Singer
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -15,21 +15,21 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 """Make an airmass chart for a LIGO/Virgo/KAGRA probability sky map."""
 
 import numpy as np
 
 from . import ArgumentParser, FileType, HelpChoicesAction
-from .matplotlib import figure_parser
+from .matplotlib import get_figure_parser
 
 
 def parser():
     from astropy.coordinates import EarthLocation
     site_names = EarthLocation.get_site_names()
-    parser = ArgumentParser(parents=[figure_parser])
+    parser = ArgumentParser(parents=[get_figure_parser()])
     parser.add_argument(
         '-v', '--verbose', action='store_true',
         help='Print airmass table to stdout')
     parser.add_argument(
         'input', metavar='INPUT.fits[.gz]', type=FileType('rb'),
         default='-', nargs='?', help='Input FITS file')
     parser.add_argument(
```

### Comparing `ligo.skymap-1.0.7/ligo/skymap/tool/ligo_skymap_plot_observability.py` & `ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_plot_observability.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,21 +15,21 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 """Make an observability chart for a LIGO/Virgo/KAGRA probability sky map."""
 
 import numpy as np
 
 from . import ArgumentParser, FileType, HelpChoicesAction
-from .matplotlib import figure_parser
+from .matplotlib import get_figure_parser
 
 
 def parser():
     from astropy.coordinates import EarthLocation
     site_names = EarthLocation.get_site_names()
-    parser = ArgumentParser(parents=[figure_parser])
+    parser = ArgumentParser(parents=[get_figure_parser()])
     parser.add_argument(
         '-v', '--verbose', action='store_true',
         help='Print airmass table to stdout')
     parser.add_argument(
         'input', metavar='INPUT.fits[.gz]', type=FileType('rb'),
         default='-', nargs='?', help='Input FITS file')
     parser.add_argument(
```

### Comparing `ligo.skymap-1.0.7/ligo/skymap/tool/ligo_skymap_plot_pp_samples.py` & `ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_plot_pp_samples.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,30 +17,30 @@
 """Create a P-P plot to compare a posterior sample chain with a sky map."""
 
 import re
 
 import numpy as np
 
 from . import ArgumentParser, FileType
-from .matplotlib import figure_parser
+from .matplotlib import get_figure_parser
 
 
 def fmt(x, sigfigs, force_scientific=False):
     """Round and format a number in scientific notation."""
     places = sigfigs - int(np.floor(np.log10(x)))
     x_rounded = np.around(x, places)
     if places <= 0 and not force_scientific:
         return '{:d}'.format(int(x_rounded))
     else:
         s = ('{:.' + str(sigfigs) + 'e}').format(x_rounded)
         return re.sub(r'^(.*)e\+?(-?)0*(\d+)$', r'$\1 \\times 10^{\2\3}$', s)
 
 
 def parser():
-    parser = ArgumentParser(parents=[figure_parser])
+    parser = ArgumentParser(parents=[get_figure_parser()])
     parser.add_argument(
         'skymap', metavar='SKYMAP.fits[.gz]', type=FileType('rb'),
         help='FITS sky map file')
     parser.add_argument(
         'samples', metavar='SAMPLES.hdf5', type=FileType('rb'),
         help='HDF5 posterior sample chain file')
     parser.add_argument(
```

### Comparing `ligo.skymap-1.0.7/ligo/skymap/tool/ligo_skymap_plot_stats.py` & `ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_plot_stats.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2013-2020  Leo Singer
+# Copyright (C) 2013-2023  Leo Singer
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -14,15 +14,14 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 """Create summary plots for sky maps of found injections, optionally binned
 cumulatively by false alarm rate or SNR.
 """
 
-from distutils.dir_util import mkpath
 import os
 
 from . import ArgumentParser, FileType
 from .matplotlib import MatplotlibFigureType
 
 
 def parser():
@@ -161,15 +160,15 @@
             if len(nsamples) == 1:
                 nsamples, = nsamples
                 title += ' ({} events)'.format(nsamples)
             else:
                 nsamples = None
 
             subdir = os.path.join(opts.output, key_to_dir(key))
-            mkpath(subdir)
+            os.makedirs(subdir, exist_ok=True)
 
             # Make several different kinds of P-P plots
             for suffix, xlabel in pp_plot_settings:
                 colname = 'searched_prob' + suffix
                 fig = plt.figure(figsize=(6, 6))
                 ax = fig.add_subplot(111, projection='pp_plot')
                 fig.subplots_adjust(bottom=0.15)
```

### Comparing `ligo.skymap-1.0.7/ligo/skymap/tool/ligo_skymap_plot_volume.py` & `ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_plot_volume.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 """Plot a volumetric posterior in three-projection view."""
 
 
 from . import ArgumentParser, FileType
-from .matplotlib import figure_parser
+from .matplotlib import get_figure_parser
 
 
 def parser():
-    parser = ArgumentParser(parents=[figure_parser])
+    parser = ArgumentParser(parents=[get_figure_parser()])
     parser.add_argument(
         '--annotate', default=False, action='store_true',
         help='annotate plot with information about the event')
     parser.add_argument(
         '--max-distance', metavar='Mpc', type=float,
         help='maximum distance of plot in Mpc')
     parser.add_argument(
```

### Comparing `ligo.skymap-1.0.7/ligo/skymap/tool/ligo_skymap_stats.py` & `ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_stats.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/tool/ligo_skymap_unflatten.py` & `ligo.skymap-1.1.0/ligo/skymap/tool/ligo_skymap_unflatten.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/tool/matplotlib.py` & `ligo.skymap-1.1.0/ligo/skymap/tool/matplotlib.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2013-2020  Leo Singer
+# Copyright (C) 2013-2023  Leo Singer
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -31,15 +31,15 @@
 if 'matplotlib.pyplot' in sys.modules:
     from matplotlib import pyplot as plt
     plt.switch_backend('Template')
 else:
     matplotlib.use('Template', warn=False, force=True)
     from matplotlib import pyplot as plt
 
-__all__ = ('figure_parser',)
+__all__ = ('get_figure_parser',)
 
 
 class MatplotlibFigureType(FileType):
 
     def __init__(self):
         super().__init__('wb')
 
@@ -105,32 +105,33 @@
 
 @type_with_sideeffect(int)
 def transparent(value):
     from matplotlib import rcParams
     rcParams['savefig.transparent'] = bool(value)
 
 
-figure_parser = argparse.ArgumentParser(add_help=False)
-group = figure_parser.add_argument_group(
-    'figure options', 'Options that affect figure output format')
-group.add_argument(
-    '-o', '--output', metavar='FILE.{pdf,png}',
-    default='-', type=MatplotlibFigureType(),
-    help='output file, or - to plot to screen')
-group.add_argument(
-    '--colormap', default='cylon', choices=plt.colormaps(), type=colormap,
-    metavar='CMAP', help='matplotlib colormap')
-group.add_argument(
-    '--help-colormap', action=HelpChoicesAction, choices=plt.colormaps())
-group.add_argument(
-    '--figure-width', metavar='INCHES', type=figwidth, default='8',
-    help='width of figure in inches')
-group.add_argument(
-    '--figure-height', metavar='INCHES', type=figheight, default='6',
-    help='height of figure in inches')
-group.add_argument(
-    '--dpi', metavar='PIXELS', type=dpi, default=300,
-    help='resolution of figure in dots per inch')
-group.add_argument(
-    '--transparent', const='1', default='0', nargs='?', type=transparent,
-    help='Save image with transparent background')
-del group
+def get_figure_parser():
+    parser = argparse.ArgumentParser(add_help=False)
+    group = parser.add_argument_group(
+        'figure options', 'Options that affect figure output format')
+    group.add_argument(
+        '-o', '--output', metavar='FILE.{pdf,png}',
+        default='-', type=MatplotlibFigureType(),
+        help='output file, or - to plot to screen')
+    group.add_argument(
+        '--colormap', default='cylon', choices=plt.colormaps(), type=colormap,
+        metavar='CMAP', help='matplotlib colormap')
+    group.add_argument(
+        '--help-colormap', action=HelpChoicesAction, choices=plt.colormaps())
+    group.add_argument(
+        '--figure-width', metavar='INCHES', type=figwidth, default='8',
+        help='width of figure in inches')
+    group.add_argument(
+        '--figure-height', metavar='INCHES', type=figheight, default='6',
+        help='height of figure in inches')
+    group.add_argument(
+        '--dpi', metavar='PIXELS', type=dpi, default=300,
+        help='resolution of figure in dots per inch')
+    group.add_argument(
+        '--transparent', const='1', default='0', nargs='?', type=transparent,
+        help='Save image with transparent background')
+    return parser
```

### Comparing `ligo.skymap-1.0.7/ligo/skymap/tool/tests/__init__.py` & `ligo.skymap-1.1.0/ligo/skymap/tool/tests/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import distutils.spawn
 from importlib import metadata
 from importlib import resources
 import multiprocessing
 import os
 import shutil
 import stat
 import subprocess
@@ -39,15 +38,15 @@
 def run_ligolw(name, *args):
     """Run an external tool that is provided by python-ligo-lw.
 
     This is trivial if python-ligo-lw has actually been installed and LALSuite
     is in the PATH. If python-ligo-lw is not installed and is only present as
     an egg, then things get more complicated.
     """
-    path = distutils.spawn.find_executable(name)
+    path = shutil.which(name)
     if path:
         # The tool has been installed, so we can just call it.
         subprocess.check_call([path, *args])
     else:
         # The tool has not been installed, so we have to try to run it using
         # importlib.metadata.
         process = multiprocessing.Process(
@@ -63,15 +62,15 @@
     """Run an external tool that is provided by LALSuite.
 
     This is trivial if lalsuite has actually been installed it is in the PATH.
     If LALSuite is not installed and is only present as an egg, then things get
     more complicated because of how the LALSuite wheel packs binaries as
     package data.
     """
-    path = distutils.spawn.find_executable(name)
+    path = shutil.which(name)
     if path:
         # The tool has been installed, so we can just call it.
         subprocess.check_call([path, *args])
     else:
         # The tool has not been installed, so we have to find the underlying
         # binary inside the lalapps module.
         with resources.path('lalapps.bin', name) as path:
```

### Comparing `ligo.skymap-1.0.7/ligo/skymap/tool/tests/test_bayestar.py` & `ligo.skymap-1.1.0/ligo/skymap/tool/tests/test_bayestar.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/tool/tests/test_bayestar_inject.py` & `ligo.skymap-1.1.0/ligo/skymap/tool/tests/test_bayestar_inject.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/tool/tests/test_combine.py` & `ligo.skymap-1.1.0/ligo/skymap/tool/tests/test_combine.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/tool/tests/test_flatten.py` & `ligo.skymap-1.1.0/ligo/skymap/tool/tests/test_flatten.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/tool/tests/test_from_samples.py` & `ligo.skymap-1.1.0/ligo/skymap/tool/tests/test_from_samples.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/tool/tests/test_help.py` & `ligo.skymap-1.1.0/ligo/skymap/tool/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/tool/tests/test_plot.py` & `ligo.skymap-1.1.0/ligo/skymap/tool/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/tool/tests/test_plot_stats.py` & `ligo.skymap-1.1.0/ligo/skymap/tool/tests/test_plot_stats.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/util/file.py` & `ligo.skymap-1.1.0/ligo/skymap/util/file.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/util/ilwd.py` & `ligo.skymap-1.1.0/ligo/skymap/util/ilwd.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/util/numpy.py` & `ligo.skymap-1.1.0/ligo/skymap/util/numpy.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/util/progress.py` & `ligo.skymap-1.1.0/ligo/skymap/util/progress.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/util/sqlite.py` & `ligo.skymap-1.1.0/ligo/skymap/util/sqlite.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo/skymap/util/stopwatch.py` & `ligo.skymap-1.1.0/ligo/skymap/util/stopwatch.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/ligo.skymap.egg-info/PKG-INFO` & `ligo.skymap-1.1.0/ligo.skymap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ligo.skymap
-Version: 1.0.7
+Version: 1.1.0
 Summary: Tools for reading, writing, manipulating, and making LIGO and Virgo sky maps
 Home-page: https://lscsoft.docs.ligo.org/ligo.skymap/
 Author: Leo Singer
 Author-email: leo.singer@ligo.org
 License: GNU GPL v3+
 Project-URL: Bug Tracker, https://git.ligo.org/lscsoft/ligo.skymap/issues
 Project-URL: Change Log, https://lscsoft.docs.ligo.org/ligo.skymap/changes.html
@@ -12,18 +12,18 @@
 Project-URL: GitHub, https://github.com/lpsinger/ligo.skymap
 Project-URL: Source Code, https://git.ligo.org/lscsoft/ligo.skymap
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
+Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Description-Content-Type: text/x-rst
 Provides-Extra: test
```

### Comparing `ligo.skymap-1.0.7/ligo.skymap.egg-info/SOURCES.txt` & `ligo.skymap-1.1.0/ligo.skymap.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 docs/io/events.rst
 docs/io/fits.rst
 docs/io/hdf5.rst
 docs/kde/index.rst
 docs/moc/index.rst
 docs/plot/allsky.rst
 docs/plot/backdrop.rst
+docs/plot/bayes_factor.rst
 docs/plot/marker.rst
 docs/plot/poly.rst
 docs/plot/pp.rst
 docs/postprocess/contour.rst
 docs/postprocess/cosmology.rst
 docs/postprocess/crossmatch.rst
 docs/postprocess/ellipse.rst
@@ -66,14 +67,15 @@
 docs/tool/ligo_skymap_constellations.rst
 docs/tool/ligo_skymap_contour.rst
 docs/tool/ligo_skymap_contour_moc.rst
 docs/tool/ligo_skymap_flatten.rst
 docs/tool/ligo_skymap_from_samples.rst
 docs/tool/ligo_skymap_plot.rst
 docs/tool/ligo_skymap_plot_airmass.rst
+docs/tool/ligo_skymap_plot_coherence.rst
 docs/tool/ligo_skymap_plot_observability.rst
 docs/tool/ligo_skymap_plot_stats.rst
 docs/tool/ligo_skymap_plot_volume.rst
 docs/tool/ligo_skymap_stats.rst
 docs/tool/ligo_skymap_unflatten.rst
 docs/util/file.rst
 docs/util/ilwd.rst
@@ -84,15 +86,14 @@
 licenses/NUMPY_LICENSE.rst
 licenses/README.rst
 licenses/TEMPLATE_LICENCE.rst
 ligo.skymap.egg-info/PKG-INFO
 ligo.skymap.egg-info/SOURCES.txt
 ligo.skymap.egg-info/dependency_links.txt
 ligo.skymap.egg-info/entry_points.txt
-ligo.skymap.egg-info/namespace_packages.txt
 ligo.skymap.egg-info/not-zip-safe
 ligo.skymap.egg-info/requires.txt
 ligo.skymap.egg-info/top_level.txt
 ligo/skymap/__init__.py
 ligo/skymap/_astropy_init.py
 ligo/skymap/conftest.py
 ligo/skymap/distance.py
@@ -139,14 +140,15 @@
 ligo/skymap/io/tests/data/test.hdf5
 ligo/skymap/io/tests/data/gstlal_reference_psd/H1L1V1-REFERENCE_PSD-967234210-29963.xml.gz
 ligo/skymap/io/tests/data/gstlal_reference_psd/__init__.py
 ligo/skymap/plot/__init__.py
 ligo/skymap/plot/allsky.py
 ligo/skymap/plot/angle.py
 ligo/skymap/plot/backdrop.py
+ligo/skymap/plot/bayes_factor.py
 ligo/skymap/plot/cmap.py
 ligo/skymap/plot/cylon.csv
 ligo/skymap/plot/cylon.py
 ligo/skymap/plot/marker.py
 ligo/skymap/plot/ne_simplified_coastline.json
 ligo/skymap/plot/poly.py
 ligo/skymap/plot/pp.py
@@ -196,14 +198,15 @@
 ligo/skymap/tool/ligo_skymap_constellations.py
 ligo/skymap/tool/ligo_skymap_contour.py
 ligo/skymap/tool/ligo_skymap_contour_moc.py
 ligo/skymap/tool/ligo_skymap_flatten.py
 ligo/skymap/tool/ligo_skymap_from_samples.py
 ligo/skymap/tool/ligo_skymap_plot.py
 ligo/skymap/tool/ligo_skymap_plot_airmass.py
+ligo/skymap/tool/ligo_skymap_plot_coherence.py
 ligo/skymap/tool/ligo_skymap_plot_observability.py
 ligo/skymap/tool/ligo_skymap_plot_pp_samples.py
 ligo/skymap/tool/ligo_skymap_plot_stats.py
 ligo/skymap/tool/ligo_skymap_plot_volume.py
 ligo/skymap/tool/ligo_skymap_stats.py
 ligo/skymap/tool/ligo_skymap_unflatten.py
 ligo/skymap/tool/matplotlib.py
```

### Comparing `ligo.skymap-1.0.7/ligo.skymap.egg-info/entry_points.txt` & `ligo.skymap-1.1.0/ligo.skymap.egg-info/entry_points.txt`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 ligo-skymap-constellations = ligo.skymap.tool.ligo_skymap_constellations:main
 ligo-skymap-contour = ligo.skymap.tool.ligo_skymap_contour:main
 ligo-skymap-contour-moc = ligo.skymap.tool.ligo_skymap_contour_moc:main
 ligo-skymap-flatten = ligo.skymap.tool.ligo_skymap_flatten:main
 ligo-skymap-from-samples = ligo.skymap.tool.ligo_skymap_from_samples:main
 ligo-skymap-plot = ligo.skymap.tool.ligo_skymap_plot:main
 ligo-skymap-plot-airmass = ligo.skymap.tool.ligo_skymap_plot_airmass:main
+ligo-skymap-plot-coherence = ligo.skymap.tool.ligo_skymap_plot_coherence:main
 ligo-skymap-plot-observability = ligo.skymap.tool.ligo_skymap_plot_observability:main
 ligo-skymap-plot-pp-samples = ligo.skymap.tool.ligo_skymap_plot_pp_samples:main
 ligo-skymap-plot-stats = ligo.skymap.tool.ligo_skymap_plot_stats:main
 ligo-skymap-plot-volume = ligo.skymap.tool.ligo_skymap_plot_volume:main
 ligo-skymap-stats = ligo.skymap.tool.ligo_skymap_stats:main
 ligo-skymap-unflatten = ligo.skymap.tool.ligo_skymap_unflatten:main
```

### Comparing `ligo.skymap-1.0.7/setup.cfg` & `ligo.skymap-1.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 github_project = lpsinger/ligo.skymap
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 	Operating System :: MacOS
 	Operating System :: POSIX
+	Operating System :: POSIX :: Linux
 	Operating System :: Unix
 	Programming Language :: C
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: Scientific/Engineering :: Astronomy
 	Topic :: Scientific/Engineering :: Physics
 project_urls = 
 	Bug Tracker = https://git.ligo.org/lscsoft/ligo.skymap/issues
@@ -31,16 +31,15 @@
 	Documentation = https://lscsoft.docs.ligo.org/ligo.skymap
 	GitHub = https://github.com/lpsinger/ligo.skymap
 	Source Code = https://git.ligo.org/lscsoft/ligo.skymap
 
 [options]
 zip_safe = False
 packages = find_namespace:
-namespace_packages = ligo
-python_version = >=3.8
+python_version = >=3.9
 setup_requires = setuptools_scm
 install_requires = 
 	astroplan>=0.7  # https://github.com/astropy/astroplan/issues/479
 	astropy>=5.0  # https://github.com/astropy/astropy/pull/12176
 	astropy-healpix>=0.3  # https://github.com/astropy/astropy-healpix/pull/106
 	healpy
 	h5py
@@ -71,14 +70,15 @@
 	ligo-skymap-contour-moc = ligo.skymap.tool.ligo_skymap_contour_moc:main
 	ligo-skymap-flatten = ligo.skymap.tool.ligo_skymap_flatten:main
 	ligo-skymap-unflatten = ligo.skymap.tool.ligo_skymap_unflatten:main
 	ligo-skymap-from-samples = ligo.skymap.tool.ligo_skymap_from_samples:main
 	ligo-skymap-constellations = ligo.skymap.tool.ligo_skymap_constellations:main
 	ligo-skymap-plot = ligo.skymap.tool.ligo_skymap_plot:main
 	ligo-skymap-plot-airmass = ligo.skymap.tool.ligo_skymap_plot_airmass:main
+	ligo-skymap-plot-coherence = ligo.skymap.tool.ligo_skymap_plot_coherence:main
 	ligo-skymap-plot-observability = ligo.skymap.tool.ligo_skymap_plot_observability:main
 	ligo-skymap-plot-pp-samples = ligo.skymap.tool.ligo_skymap_plot_pp_samples:main
 	ligo-skymap-plot-stats = ligo.skymap.tool.ligo_skymap_plot_stats:main
 	ligo-skymap-plot-volume = ligo.skymap.tool.ligo_skymap_plot_volume:main
 	ligo-skymap-stats = ligo.skymap.tool.ligo_skymap_stats:main
 pytest11 = 
 	omp-get-num-threads = ligo.skymap.tests.plugins.omp
@@ -163,13 +163,13 @@
 	ligo/skymap/tool/bayestar_inject.py:E731,N803,N806
 	ligo/skymap/tool/bayestar_realize_coincs.py:N803,N806
 	ligo/skymap/tool/tests/test_bayestar_inject.py:N803,N806
 	ligo/skymap/util/ilwd.py:N802,N803
 	src/bayestar_cosmology.py:N802,N803,N806,N816
 
 [bdist_wheel]
-py_limited_api = cp38
+py_limited_api = cp39
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `ligo.skymap-1.0.7/setup.py` & `ligo.skymap-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import sys
 
 from setuptools import setup
 
 
 def get_extensions():
-    from distutils.core import Extension
+    from setuptools import Extension
     import os
 
     from extension_helpers import add_openmp_flags_if_available, pkg_config
     import numpy as np
 
     pkg_config_packages = ['gsl']
 
@@ -38,14 +38,15 @@
 
     if os.environ.get('LIGO_SKYMAP_USE_ITTNOTIFY'):
         pkg_config_packages.append('ittnotify')
 
     kwargs = pkg_config(pkg_config_packages, [])
     kwargs['include_dirs'].extend(include_dirs)
     kwargs['extra_compile_args'].extend(['-std=gnu11',
+                                         '-fvisibility=hidden',
                                          '-DGSL_RANGE_CHECK_OFF',
                                          '-DHAVE_INLINE'])
 
     if os.environ.get('LIGO_SKYMAP_USE_ITTNOTIFY'):
         kwargs.setdefault('define_macros', []).append(('WITH_ITTNOTIFY', 1))
 
     extension = Extension(name='ligo.skymap.core', language='c',
```

### Comparing `ligo.skymap-1.0.7/src/bayestar_cosmology.h` & `ligo.skymap-1.1.0/src/bayestar_cosmology.h`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/src/bayestar_cosmology.py` & `ligo.skymap-1.1.0/src/bayestar_cosmology.py`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/src/bayestar_distance.c` & `ligo.skymap-1.1.0/src/bayestar_distance.c`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/src/bayestar_distance.h` & `ligo.skymap-1.1.0/src/bayestar_distance.h`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/src/bayestar_moc.c` & `ligo.skymap-1.1.0/src/bayestar_moc.c`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/src/bayestar_moc.h` & `ligo.skymap-1.1.0/src/bayestar_moc.h`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/src/bayestar_sky_map.c` & `ligo.skymap-1.1.0/src/bayestar_sky_map.c`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 **************  / __  / /| |\  / __/  \__ \ / / / /| | / /_/ /  ****************
 *************  / /_/ / ___ |/ / /___ ___/ // / / ___ |/ _, _/  *****************
 ************  /_____/_/  |_/_/_____//____//_/ /_/  |_/_/ |_|  ******************
 */
 
 
 /*
- * Copyright (C) 2013-2020  Leo Singer
+ * Copyright (C) 2013-2023  Leo Singer
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
  *
  * This program is distributed in the hope that it will be useful,
@@ -1364,15 +1364,15 @@
     bayestar_distance_parameters_to_moments(
         mu, sigma, &mean2, &std2, &norm2);
 
     if (gsl_finite(mean_std) && mean_std >= min_mean_std)
     {
         /* Precision degrades as we approach the singularity at
          * mean/std=sqrt(3). Relax the tolerance of the test near there. */
-        const double rtol = mean_std >= min_mean_std + 0.1 ? 1e-9 : 4e-5;
+        const double rtol = mean_std >= min_mean_std + 0.1 ? 1e-9 : 6e-5;
         gsl_test_rel(norm2, norm, rtol,
             "testing round-trip conversion of normalization for mean=%g, std=%g",
             mean, std);
         gsl_test_rel(mean2, mean, rtol,
             "testing round-trip conversion of mean for mean=%g, std=%g",
             mean, std);
         gsl_test_rel(std2, std, rtol,
```

### Comparing `ligo.skymap-1.0.7/src/bayestar_sky_map.h` & `ligo.skymap-1.1.0/src/bayestar_sky_map.h`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/src/core.c` & `ligo.skymap-1.1.0/src/core.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /*
- * Copyright (C) 2013-2022  Leo Singer
+ * Copyright (C) 2013-2023  Leo Singer
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
  *
  * This program is distributed in the hope that it will be useful,
@@ -11,16 +11,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#define NPY_NO_DEPRECATED_API NPY_1_7_API_VERSION
-#define Py_LIMITED_API 0x03080000
+#define NPY_NO_DEPRECATED_API NPY_1_19_API_VERSION
+#define Py_LIMITED_API 0x03090000
 
 /* FIXME:
  * The Numpy C-API defines PyArrayDescr_Type as:
  *
  *   #define PyArrayDescr_Type (*(PyTypeObject *)PyArray_API[3])
  *
  * and then in some places we need to take its address, &PyArrayDescr_Type.
@@ -1026,35 +1026,32 @@
     return PyLong_FromLong(ret);
 }
 
 
 /*****************************************************************************/
 
 
-/* FIXME: (PyUFuncGenericFunction) casts below work around possible mismatched
- * const-ness of the dimensions and steps arguments, which became const in
- * Numpy 1.19.0. Remove casts once we drop support for Numpy < 1.19.0. */
 static const PyUFuncGenericFunction
-    conditional_pdf_loops[] = {(PyUFuncGenericFunction) conditional_pdf_loop},
-    conditional_cdf_loops[] = {(PyUFuncGenericFunction) conditional_cdf_loop},
-    conditional_ppf_loops[] = {(PyUFuncGenericFunction) conditional_ppf_loop},
-    moments_to_parameters_loops[] = {(PyUFuncGenericFunction) moments_to_parameters_loop},
-    parameters_to_moments_loops[] = {(PyUFuncGenericFunction) parameters_to_moments_loop},
-    volume_render_loops[] = {(PyUFuncGenericFunction) volume_render_loop},
-    marginal_pdf_loops[] = {(PyUFuncGenericFunction) marginal_pdf_loop},
-    marginal_cdf_loops[] = {(PyUFuncGenericFunction) marginal_cdf_loop},
-    marginal_ppf_loops[] = {(PyUFuncGenericFunction) marginal_ppf_loop},
-    nest2uniq_loops[] = {(PyUFuncGenericFunction) nest2uniq_loop},
-    uniq2nest_loops[] = {(PyUFuncGenericFunction) uniq2nest_loop},
-    uniq2order_loops[] = {(PyUFuncGenericFunction) uniq2order_loop},
-    uniq2pixarea_loops[] = {(PyUFuncGenericFunction) uniq2pixarea_loop},
-    uniq2ang_loops[] = {(PyUFuncGenericFunction) uniq2ang_loop},
-    log_posterior_toa_phoa_snr_loops[] = {(PyUFuncGenericFunction) log_posterior_toa_phoa_snr_loop},
-    antenna_factor_loops[] = {(PyUFuncGenericFunction) antenna_factor_loop},
-    signal_amplitude_model_loops[] = {(PyUFuncGenericFunction) signal_amplitude_model_loop};
+    conditional_pdf_loops[] = {conditional_pdf_loop},
+    conditional_cdf_loops[] = {conditional_cdf_loop},
+    conditional_ppf_loops[] = {conditional_ppf_loop},
+    moments_to_parameters_loops[] = {moments_to_parameters_loop},
+    parameters_to_moments_loops[] = {parameters_to_moments_loop},
+    volume_render_loops[] = {volume_render_loop},
+    marginal_pdf_loops[] = {marginal_pdf_loop},
+    marginal_cdf_loops[] = {marginal_cdf_loop},
+    marginal_ppf_loops[] = {marginal_ppf_loop},
+    nest2uniq_loops[] = {nest2uniq_loop},
+    uniq2nest_loops[] = {uniq2nest_loop},
+    uniq2order_loops[] = {uniq2order_loop},
+    uniq2pixarea_loops[] = {uniq2pixarea_loop},
+    uniq2ang_loops[] = {uniq2ang_loop},
+    log_posterior_toa_phoa_snr_loops[] = {log_posterior_toa_phoa_snr_loop},
+    antenna_factor_loops[] = {antenna_factor_loop},
+    signal_amplitude_model_loops[] = {signal_amplitude_model_loop};
 
 static const char log_posterior_toa_phoa_snr_types[] = {
     NPY_DOUBLE, NPY_DOUBLE, NPY_DOUBLE, NPY_DOUBLE, NPY_DOUBLE, NPY_DOUBLE,
     NPY_DOUBLE, NPY_DOUBLE, NPY_INT, NPY_BOOL, NPY_DOUBLE, NPY_DOUBLE,
     NPY_DOUBLE, NPY_FLOAT, NPY_FLOAT, NPY_DOUBLE, NPY_DOUBLE, NPY_FLOAT,
     NPY_DOUBLE};
 
@@ -1122,15 +1119,17 @@
     import_array();
     import_umath();
 
     module = PyModule_Create(&moduledef);
     if (!module)
         return NULL;
 
-    /* Ignore warnings in Numpy API */
+    /* Ignore warnings in Numpy API.
+     * FIXME: remove once https://github.com/numpy/numpy/pull/23847 is merged.
+     */
     WARNINGS_PUSH
     WARNINGS_IGNORE_DISCARDED_QUALIFIERS
 
     MODULE_ADD_OBJECT(
         "sky_map_descr", (PyObject *) sky_map_create_descr());
 
     MODULE_ADD_OBJECT(
```

### Comparing `ligo.skymap-1.0.7/src/cubic_interp.c` & `ligo.skymap-1.1.0/src/cubic_interp.c`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/src/cubic_interp.h` & `ligo.skymap-1.1.0/src/cubic_interp.h`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/src/cubic_interp_test.c` & `ligo.skymap-1.1.0/src/cubic_interp_test.c`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/src/omp_interruptible.h` & `ligo.skymap-1.1.0/src/omp_interruptible.h`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/src/vmath.h` & `ligo.skymap-1.1.0/src/vmath.h`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/src/warnings.h` & `ligo.skymap-1.1.0/src/warnings.h`

 * *Files identical despite different names*

### Comparing `ligo.skymap-1.0.7/tox.ini` & `ligo.skymap-1.1.0/tox.ini`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tox]
 envlist =
-    py{36,37,38}-test{,-alldeps,-devdeps}{,-cov}
-    py{36,37,38}-test-numpy{116,117,118}
-    py{36,37,38}-test-astropy{30,40,lts}
+    py{39,310,311}-test{,-alldeps,-devdeps}{,-cov}
+    py{39,310,311}-test-numpy{116,117,118}
+    py{39,310,311}-test-astropy{30,40,lts}
     build_docs
     linkcheck
     codestyle
 requires =
     setuptools >= 30.3.0
     pip >= 19.3.1
 isolated_build = true
```

