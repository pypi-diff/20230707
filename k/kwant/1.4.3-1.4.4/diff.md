# Comparing `tmp/kwant-1.4.3.tar.gz` & `tmp/kwant-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kwant-1.4.3.tar", last modified: Wed Mar 30 20:16:23 2022, max compression
+gzip compressed data, was "kwant-1.4.4.tar", last modified: Mon Jul  3 13:46:37 2023, max compression
```

## Comparing `kwant-1.4.3.tar` & `kwant-1.4.4.tar`

### file list

```diff
@@ -1,238 +1,238 @@
-drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2022-03-30 20:16:23.431414 kwant-1.4.3/
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      240 2019-03-29 14:02:16.000000 kwant-1.4.3/.coveragerc
--rw-rw-r--   0 cwg       (1000) cwg       (1000)       37 2020-03-31 21:13:48.000000 kwant-1.4.3/.gitattributes
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      393 2022-03-30 20:14:08.000000 kwant-1.4.3/.gitignore
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     7850 2022-03-30 20:14:08.000000 kwant-1.4.3/.gitlab-ci.yml
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      593 2022-03-30 20:14:08.000000 kwant-1.4.3/.mailmap
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     1844 2022-03-30 20:14:08.000000 kwant-1.4.3/AUTHORS.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     1512 2022-03-30 20:14:08.000000 kwant-1.4.3/CITING.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      607 2020-03-31 22:06:32.000000 kwant-1.4.3/CONTRIBUTE.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    12540 2022-03-30 20:14:08.000000 kwant-1.4.3/INSTALL.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     1476 2017-11-14 12:25:06.000000 kwant-1.4.3/LICENSE.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     7219 2022-03-30 20:14:57.000000 kwant-1.4.3/MANIFEST.in
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     2655 2022-03-30 20:16:23.431414 kwant-1.4.3/PKG-INFO
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     1554 2022-03-30 20:14:08.000000 kwant-1.4.3/README.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      273 2016-09-19 15:27:17.000000 kwant-1.4.3/README_WINDOWS.txt
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    18611 2022-03-30 20:14:08.000000 kwant-1.4.3/RELEASE.rst
--rwxrwxr-x   0 cwg       (1000) cwg       (1000)      318 2019-03-29 14:02:16.000000 kwant-1.4.3/check_whitespace
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     1577 2022-03-30 20:14:08.000000 kwant-1.4.3/conftest.py
-drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2022-03-30 20:16:23.379414 kwant-1.4.3/doc/
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     7346 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/Makefile
-drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2022-03-30 20:16:23.379414 kwant-1.4.3/doc/kwantdoctheme/
-drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2022-03-30 20:16:23.379414 kwant-1.4.3/doc/kwantdoctheme/static/
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     3576 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/kwantdoctheme/static/kwantdoctheme.css
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      614 2016-09-19 15:27:17.000000 kwant-1.4.3/doc/kwantdoctheme/theme.conf
-drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2022-03-30 20:16:23.379414 kwant-1.4.3/doc/source/
-drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2022-03-30 20:16:23.379414 kwant-1.4.3/doc/source/_static/
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     1304 2017-04-25 20:06:33.000000 kwant-1.4.3/doc/source/_static/kwant.css
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     3017 2016-09-19 15:27:17.000000 kwant-1.4.3/doc/source/_static/kwant_logo.png
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      294 2019-03-29 14:02:16.000000 kwant-1.4.3/doc/source/_static/mathconf.js
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     4914 2019-03-29 14:02:16.000000 kwant-1.4.3/doc/source/_static/sidebar.js
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      293 2013-10-15 09:31:17.000000 kwant-1.4.3/doc/source/_static/togglediv.js
-drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2022-03-30 20:16:23.379414 kwant-1.4.3/doc/source/code/
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     1915 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/source/code/README
-drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2022-03-30 20:16:23.383414 kwant-1.4.3/doc/source/code/figure/
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     1099 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/source/code/figure/_defs.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     6557 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/source/code/figure/ab_ring.py.diff
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     6209 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/source/code/figure/ab_ring_sketch.svg
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    26078 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/source/code/figure/ab_ring_sketch2.svg
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     2075 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/source/code/figure/band_structure.py.diff
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     5598 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/source/code/figure/closed_system.py.diff
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     7291 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/source/code/figure/discretize.py.diff
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    12445 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/source/code/figure/faq.py.diff
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     7090 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/source/code/figure/graphene.py.diff
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    11405 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/source/code/figure/kernel_polynomial_method.py.diff
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     8218 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/source/code/figure/magnetic_texture.py.diff
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     4499 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/source/code/figure/plot_graphene.py.diff
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     2424 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/source/code/figure/plot_qahe.py.diff
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     2166 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/source/code/figure/plot_zincblende.py.diff
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     3067 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/source/code/figure/quantum_well.py.diff
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     3681 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/source/code/figure/quantum_wire.py.diff
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     3879 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/source/code/figure/spin_orbit.py.diff
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     5479 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/source/code/figure/superconductor.py.diff
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    33403 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/source/code/figure/superconductor_transport_sketch.svg
-drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2022-03-30 20:16:23.383414 kwant-1.4.3/doc/source/code/include/
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     2331 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/source/code/include/quantum_wire_revisited.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    11233 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/source/conf.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      206 2019-03-29 14:02:16.000000 kwant-1.4.3/doc/source/index.rst
-drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2022-03-30 20:16:23.387414 kwant-1.4.3/doc/source/pre/
--rw-rw-r--   0 cwg       (1000) cwg       (1000)       82 2017-05-24 08:50:37.000000 kwant-1.4.3/doc/source/pre/about.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)       34 2017-05-24 08:50:37.000000 kwant-1.4.3/doc/source/pre/authors.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)       33 2017-05-24 08:50:37.000000 kwant-1.4.3/doc/source/pre/citing.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)       37 2017-05-24 08:50:37.000000 kwant-1.4.3/doc/source/pre/contribute.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      143 2017-05-24 08:50:37.000000 kwant-1.4.3/doc/source/pre/index.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)       34 2017-05-24 08:50:37.000000 kwant-1.4.3/doc/source/pre/install.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)       34 2017-05-24 08:50:37.000000 kwant-1.4.3/doc/source/pre/license.rst
-drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2022-03-30 20:16:23.387414 kwant-1.4.3/doc/source/pre/whatsnew/
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     4308 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/source/pre/whatsnew/0.2.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     9173 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/source/pre/whatsnew/1.0.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     3872 2019-03-29 14:02:16.000000 kwant-1.4.3/doc/source/pre/whatsnew/1.1.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     1292 2017-11-14 12:25:06.000000 kwant-1.4.3/doc/source/pre/whatsnew/1.2.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     9845 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/source/pre/whatsnew/1.3.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    14682 2022-03-30 20:10:15.000000 kwant-1.4.3/doc/source/pre/whatsnew/1.4.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      102 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/source/pre/whatsnew/index.rst
-drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2022-03-30 20:16:23.391414 kwant-1.4.3/doc/source/reference/
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      729 2020-03-31 22:06:32.000000 kwant-1.4.3/doc/source/reference/index.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      455 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/source/reference/kwant.builder.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      369 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/source/reference/kwant.continuum.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      147 2017-06-22 10:27:41.000000 kwant-1.4.3/doc/source/reference/kwant.digest.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     3127 2020-03-31 22:06:32.000000 kwant-1.4.3/doc/source/reference/kwant.graph.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      194 2020-03-31 22:06:32.000000 kwant-1.4.3/doc/source/reference/kwant.kpm.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      379 2019-03-29 14:02:16.000000 kwant-1.4.3/doc/source/reference/kwant.lattice.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      599 2017-06-22 10:27:41.000000 kwant-1.4.3/doc/source/reference/kwant.linalg.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      267 2019-03-29 14:02:16.000000 kwant-1.4.3/doc/source/reference/kwant.operator.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      534 2020-03-31 22:06:32.000000 kwant-1.4.3/doc/source/reference/kwant.physics.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      507 2020-03-31 22:06:32.000000 kwant-1.4.3/doc/source/reference/kwant.plotter.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      280 2020-03-31 22:06:32.000000 kwant-1.4.3/doc/source/reference/kwant.qsymm.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      148 2017-06-22 10:27:41.000000 kwant-1.4.3/doc/source/reference/kwant.rmt.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     1597 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/source/reference/kwant.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      878 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/source/reference/kwant.solvers.mumps.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     2971 2017-06-22 10:27:41.000000 kwant-1.4.3/doc/source/reference/kwant.solvers.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      680 2019-03-29 14:02:16.000000 kwant-1.4.3/doc/source/reference/kwant.solvers.sparse.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     1042 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/source/reference/kwant.system.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      238 2019-03-29 14:02:16.000000 kwant-1.4.3/doc/source/reference/kwant.wraparound.rst
-drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2022-03-30 20:16:23.395414 kwant-1.4.3/doc/source/tutorial/
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    12120 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/source/tutorial/discretize.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    19888 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/source/tutorial/faq.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    20208 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/source/tutorial/first_steps.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     7023 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/source/tutorial/graphene.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      260 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/source/tutorial/index.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     4303 2019-03-29 14:02:16.000000 kwant-1.4.3/doc/source/tutorial/introduction.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    16914 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/source/tutorial/kpm.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    14857 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/source/tutorial/operators.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     9829 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/source/tutorial/plotting.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     5994 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/source/tutorial/spectrum.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    14806 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/source/tutorial/spin_potential_shape.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    10261 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/source/tutorial/superconductors.rst
-drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2022-03-30 20:16:23.395414 kwant-1.4.3/doc/sphinxext/
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     2498 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/sphinxext/kwantdoc.py
-drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2022-03-30 20:16:23.395414 kwant-1.4.3/doc/templates/
-drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2022-03-30 20:16:23.395414 kwant-1.4.3/doc/templates/autosummary/
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      550 2021-11-01 14:15:02.000000 kwant-1.4.3/doc/templates/autosummary/class.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      206 2019-03-29 14:02:16.000000 kwant-1.4.3/doc/templates/autosummary/functor.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     8834 2022-03-30 20:14:08.000000 kwant-1.4.3/doc/templates/layout.html
-drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2022-03-30 20:16:23.399414 kwant-1.4.3/docker/
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      633 2022-03-30 20:14:08.000000 kwant-1.4.3/docker/Dockerfile.conda
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     1180 2022-03-30 20:14:08.000000 kwant-1.4.3/docker/Dockerfile.debian
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     1005 2022-03-30 20:14:08.000000 kwant-1.4.3/docker/Dockerfile.ubuntu
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     2184 2020-03-31 22:06:32.000000 kwant-1.4.3/docker/README.rst
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      535 2022-03-30 20:14:08.000000 kwant-1.4.3/docker/kwant-latest.yml
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      576 2022-03-30 20:14:08.000000 kwant-1.4.3/docker/kwant-stable-no-extras.yml
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      619 2022-03-30 20:14:08.000000 kwant-1.4.3/docker/kwant-stable.yml
-drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2022-03-30 20:16:23.399414 kwant-1.4.3/examples/
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      713 2019-03-29 14:02:16.000000 kwant-1.4.3/examples/3d_plot.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     1267 2021-03-16 21:28:08.000000 kwant-1.4.3/examples/advanced_construction.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     3988 2020-03-31 22:06:32.000000 kwant-1.4.3/examples/square.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     1300 2019-03-29 14:02:16.000000 kwant-1.4.3/examples/test_square.py
-drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2022-03-30 20:16:23.431414 kwant-1.4.3/kwant/
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     2342 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/__init__.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    13420 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/_colormaps.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     6768 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/_common.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)       60 2022-03-30 20:16:23.431414 kwant-1.4.3/kwant/_kwant_version.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    13811 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/_plotter.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)  1530224 2022-03-30 20:14:46.000000 kwant-1.4.3/kwant/_system.c
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    13346 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/_system.pyx
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    88538 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/builder.py
-drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2022-03-30 20:16:23.407414 kwant-1.4.3/kwant/continuum/
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      913 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/continuum/__init__.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    10062 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/continuum/_common.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    26418 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/continuum/discretizer.py
-drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2022-03-30 20:16:23.407414 kwant-1.4.3/kwant/continuum/tests/
--rw-rw-r--   0 cwg       (1000) cwg       (1000)        0 2019-03-29 14:02:16.000000 kwant-1.4.3/kwant/continuum/tests/__init__.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     5953 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/continuum/tests/test_common.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    21647 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/continuum/tests/test_discretizer.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     3079 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/digest.py
-drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2022-03-30 20:16:23.415414 kwant-1.4.3/kwant/graph/
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      655 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/graph/__init__.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     8464 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/graph/c_scotch.pxd
--rw-rw-r--   0 cwg       (1000) cwg       (1000)   892233 2022-03-30 20:14:47.000000 kwant-1.4.3/kwant/graph/core.c
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     1684 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/graph/core.pxd
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    25352 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/graph/core.pyx
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      570 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/graph/defs.h
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      440 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/graph/defs.pxd
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      450 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/graph/defs.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)  1147239 2021-08-30 14:14:50.000000 kwant-1.4.3/kwant/graph/dijkstra.c
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    12933 2020-03-31 22:06:32.000000 kwant-1.4.3/kwant/graph/dijkstra.pyx
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     2366 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/graph/scotch.pyx
-drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2022-03-30 20:16:23.415414 kwant-1.4.3/kwant/graph/tests/
--rw-rw-r--   0 cwg       (1000) cwg       (1000)        0 2017-05-24 08:50:37.000000 kwant-1.4.3/kwant/graph/tests/__init__.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     6617 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/graph/tests/test_core.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     1864 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/graph/tests/test_scotch.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    46860 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/kpm.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    30002 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/lattice.py
-drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2022-03-30 20:16:23.423414 kwant-1.4.3/kwant/linalg/
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      685 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/linalg/__init__.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)   622040 2022-03-30 20:14:48.000000 kwant-1.4.3/kwant/linalg/_mumps.c
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     6431 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/linalg/_mumps.pyx
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     1576 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/linalg/cmumps.pxd
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      425 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/linalg/cmumps.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     2012 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/linalg/decomp_ev.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     4018 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/linalg/decomp_lu.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    24952 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/linalg/decomp_schur.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     4849 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/linalg/fortran_helpers.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)  3683037 2022-03-30 20:14:53.000000 kwant-1.4.3/kwant/linalg/lapack.c
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    45136 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/linalg/lapack.pyx
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    11857 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/linalg/lll.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    20232 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/linalg/mumps.py
-drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2022-03-30 20:16:23.423414 kwant-1.4.3/kwant/linalg/tests/
--rw-rw-r--   0 cwg       (1000) cwg       (1000)        0 2017-05-24 08:50:37.000000 kwant-1.4.3/kwant/linalg/tests/__init__.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     2682 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/linalg/tests/_test_utils.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    14143 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/linalg/tests/test_linalg.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     2713 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/linalg/tests/test_lll.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     2832 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/linalg/tests/test_mumps.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)  2402213 2022-03-30 20:14:57.000000 kwant-1.4.3/kwant/operator.c
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     1327 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/operator.pxd
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    46358 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/operator.pyx
-drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2022-03-30 20:16:23.427414 kwant-1.4.3/kwant/physics/
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      692 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/physics/__init__.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     6874 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/physics/dispersion.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    40281 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/physics/gauge.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    53379 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/physics/leads.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     1772 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/physics/noise.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     9896 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/physics/symmetry.py
-drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2022-03-30 20:16:23.427414 kwant-1.4.3/kwant/physics/tests/
--rw-rw-r--   0 cwg       (1000) cwg       (1000)        0 2017-05-24 08:50:37.000000 kwant-1.4.3/kwant/physics/tests/__init__.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     5265 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/physics/tests/test_dispersion.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    18141 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/physics/tests/test_gauge.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    51169 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/physics/tests/test_leads.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     1743 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/physics/tests/test_noise.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     9371 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/physics/tests/test_symmetry.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    89671 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/plotter.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    19219 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/qsymm.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     9966 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/rmt.py
-drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2022-03-30 20:16:23.427414 kwant-1.4.3/kwant/solvers/
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      608 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/solvers/__init__.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    41368 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/solvers/common.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     1006 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/solvers/default.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     4908 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/solvers/mumps.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     3814 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/solvers/sparse.py
-drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2022-03-30 20:16:23.427414 kwant-1.4.3/kwant/solvers/tests/
--rw-rw-r--   0 cwg       (1000) cwg       (1000)        0 2017-05-24 08:50:37.000000 kwant-1.4.3/kwant/solvers/tests/__init__.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    20724 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/solvers/tests/_test_sparse.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     3192 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/solvers/tests/test_mumps.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     1804 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/solvers/tests/test_sparse.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    17060 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/system.py
-drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2022-03-30 20:16:23.431414 kwant-1.4.3/kwant/tests/
--rw-rw-r--   0 cwg       (1000) cwg       (1000)        0 2017-05-24 08:50:37.000000 kwant-1.4.3/kwant/tests/__init__.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    50575 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/tests/test_builder.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     1841 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/tests/test_comprehensive.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    24671 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/tests/test_kpm.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    10693 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/tests/test_lattice.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    19293 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/tests/test_operator.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    19932 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/tests/test_plotter.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    21984 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/tests/test_qsymm.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     4383 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/tests/test_rmt.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     3827 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/tests/test_system.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    15297 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/tests/test_wraparound.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     4355 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/version.py
--rw-rw-r--   0 cwg       (1000) cwg       (1000)    18404 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant/wraparound.py
-drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2022-03-30 20:16:23.407414 kwant-1.4.3/kwant.egg-info/
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     2655 2022-03-30 20:14:57.000000 kwant-1.4.3/kwant.egg-info/PKG-INFO
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     5820 2022-03-30 20:14:57.000000 kwant-1.4.3/kwant.egg-info/SOURCES.txt
--rw-rw-r--   0 cwg       (1000) cwg       (1000)        1 2022-03-30 20:14:57.000000 kwant-1.4.3/kwant.egg-info/dependency_links.txt
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      121 2022-03-30 20:14:57.000000 kwant-1.4.3/kwant.egg-info/requires.txt
--rw-rw-r--   0 cwg       (1000) cwg       (1000)        6 2022-03-30 20:14:57.000000 kwant-1.4.3/kwant.egg-info/top_level.txt
--rw-rw-r--   0 cwg       (1000) cwg       (1000)     2614 2022-03-30 20:14:08.000000 kwant-1.4.3/kwant_red.jscm
--rw-rw-r--   0 cwg       (1000) cwg       (1000)      201 2022-03-30 20:14:08.000000 kwant-1.4.3/pytest.ini
--rw-rw-r--   0 cwg       (1000) cwg       (1000)       59 2022-03-30 20:16:23.431414 kwant-1.4.3/setup.cfg
--rwxrwxr-x   0 cwg       (1000) cwg       (1000)    20805 2022-03-30 20:14:08.000000 kwant-1.4.3/setup.py
+drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2023-07-03 13:46:37.704252 kwant-1.4.4/
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      240 2019-03-29 14:02:16.000000 kwant-1.4.4/.coveragerc
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)       37 2020-03-31 21:13:48.000000 kwant-1.4.4/.gitattributes
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      393 2023-06-30 16:40:53.000000 kwant-1.4.4/.gitignore
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     7850 2023-06-30 16:40:53.000000 kwant-1.4.4/.gitlab-ci.yml
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      593 2023-06-30 16:40:53.000000 kwant-1.4.4/.mailmap
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     1844 2023-06-30 16:40:53.000000 kwant-1.4.4/AUTHORS.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     1512 2023-06-30 16:40:53.000000 kwant-1.4.4/CITING.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      607 2020-03-31 22:06:32.000000 kwant-1.4.4/CONTRIBUTE.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    12540 2023-06-30 16:40:53.000000 kwant-1.4.4/INSTALL.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     1476 2017-11-14 12:25:06.000000 kwant-1.4.4/LICENSE.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     7219 2023-07-03 13:46:36.000000 kwant-1.4.4/MANIFEST.in
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     2655 2023-07-03 13:46:37.704252 kwant-1.4.4/PKG-INFO
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     1554 2023-06-30 16:40:53.000000 kwant-1.4.4/README.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      273 2016-09-19 15:27:17.000000 kwant-1.4.4/README_WINDOWS.txt
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    18611 2023-06-30 16:40:53.000000 kwant-1.4.4/RELEASE.rst
+-rwxrwxr-x   0 cwg       (1000) cwg       (1000)      318 2019-03-29 14:02:16.000000 kwant-1.4.4/check_whitespace
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     1577 2023-06-30 16:40:53.000000 kwant-1.4.4/conftest.py
+drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2023-07-03 13:46:37.572252 kwant-1.4.4/doc/
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     7346 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/Makefile
+drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2023-07-03 13:46:37.572252 kwant-1.4.4/doc/kwantdoctheme/
+drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2023-07-03 13:46:37.576252 kwant-1.4.4/doc/kwantdoctheme/static/
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     3576 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/kwantdoctheme/static/kwantdoctheme.css
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      614 2016-09-19 15:27:17.000000 kwant-1.4.4/doc/kwantdoctheme/theme.conf
+drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2023-07-03 13:46:37.576252 kwant-1.4.4/doc/source/
+drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2023-07-03 13:46:37.576252 kwant-1.4.4/doc/source/_static/
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     1304 2017-04-25 20:06:33.000000 kwant-1.4.4/doc/source/_static/kwant.css
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     3017 2016-09-19 15:27:17.000000 kwant-1.4.4/doc/source/_static/kwant_logo.png
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      294 2019-03-29 14:02:16.000000 kwant-1.4.4/doc/source/_static/mathconf.js
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     4914 2019-03-29 14:02:16.000000 kwant-1.4.4/doc/source/_static/sidebar.js
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      293 2013-10-15 09:31:17.000000 kwant-1.4.4/doc/source/_static/togglediv.js
+drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2023-07-03 13:46:37.576252 kwant-1.4.4/doc/source/code/
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     1915 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/source/code/README
+drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2023-07-03 13:46:37.588252 kwant-1.4.4/doc/source/code/figure/
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     1099 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/source/code/figure/_defs.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     6557 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/source/code/figure/ab_ring.py.diff
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     6209 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/source/code/figure/ab_ring_sketch.svg
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    26078 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/source/code/figure/ab_ring_sketch2.svg
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     2075 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/source/code/figure/band_structure.py.diff
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     5598 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/source/code/figure/closed_system.py.diff
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     7291 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/source/code/figure/discretize.py.diff
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    12445 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/source/code/figure/faq.py.diff
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     7090 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/source/code/figure/graphene.py.diff
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    11405 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/source/code/figure/kernel_polynomial_method.py.diff
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     8218 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/source/code/figure/magnetic_texture.py.diff
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     4499 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/source/code/figure/plot_graphene.py.diff
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     2424 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/source/code/figure/plot_qahe.py.diff
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     2166 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/source/code/figure/plot_zincblende.py.diff
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     3067 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/source/code/figure/quantum_well.py.diff
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     3681 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/source/code/figure/quantum_wire.py.diff
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     3879 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/source/code/figure/spin_orbit.py.diff
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     5479 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/source/code/figure/superconductor.py.diff
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    33403 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/source/code/figure/superconductor_transport_sketch.svg
+drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2023-07-03 13:46:37.588252 kwant-1.4.4/doc/source/code/include/
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     2331 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/source/code/include/quantum_wire_revisited.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    11247 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/source/conf.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      206 2019-03-29 14:02:16.000000 kwant-1.4.4/doc/source/index.rst
+drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2023-07-03 13:46:37.592252 kwant-1.4.4/doc/source/pre/
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)       82 2017-05-24 08:50:37.000000 kwant-1.4.4/doc/source/pre/about.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)       34 2017-05-24 08:50:37.000000 kwant-1.4.4/doc/source/pre/authors.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)       33 2017-05-24 08:50:37.000000 kwant-1.4.4/doc/source/pre/citing.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)       37 2017-05-24 08:50:37.000000 kwant-1.4.4/doc/source/pre/contribute.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      143 2017-05-24 08:50:37.000000 kwant-1.4.4/doc/source/pre/index.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)       34 2017-05-24 08:50:37.000000 kwant-1.4.4/doc/source/pre/install.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)       34 2017-05-24 08:50:37.000000 kwant-1.4.4/doc/source/pre/license.rst
+drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2023-07-03 13:46:37.592252 kwant-1.4.4/doc/source/pre/whatsnew/
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     4308 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/source/pre/whatsnew/0.2.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     9173 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/source/pre/whatsnew/1.0.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     3872 2019-03-29 14:02:16.000000 kwant-1.4.4/doc/source/pre/whatsnew/1.1.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     1292 2017-11-14 12:25:06.000000 kwant-1.4.4/doc/source/pre/whatsnew/1.2.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     9845 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/source/pre/whatsnew/1.3.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    14858 2023-07-03 13:22:48.000000 kwant-1.4.4/doc/source/pre/whatsnew/1.4.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      102 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/source/pre/whatsnew/index.rst
+drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2023-07-03 13:46:37.596252 kwant-1.4.4/doc/source/reference/
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      729 2020-03-31 22:06:32.000000 kwant-1.4.4/doc/source/reference/index.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      455 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/source/reference/kwant.builder.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      369 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/source/reference/kwant.continuum.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      147 2017-06-22 10:27:41.000000 kwant-1.4.4/doc/source/reference/kwant.digest.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     3127 2020-03-31 22:06:32.000000 kwant-1.4.4/doc/source/reference/kwant.graph.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      194 2020-03-31 22:06:32.000000 kwant-1.4.4/doc/source/reference/kwant.kpm.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      379 2019-03-29 14:02:16.000000 kwant-1.4.4/doc/source/reference/kwant.lattice.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      599 2017-06-22 10:27:41.000000 kwant-1.4.4/doc/source/reference/kwant.linalg.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      267 2019-03-29 14:02:16.000000 kwant-1.4.4/doc/source/reference/kwant.operator.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      534 2020-03-31 22:06:32.000000 kwant-1.4.4/doc/source/reference/kwant.physics.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      507 2020-03-31 22:06:32.000000 kwant-1.4.4/doc/source/reference/kwant.plotter.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      280 2020-03-31 22:06:32.000000 kwant-1.4.4/doc/source/reference/kwant.qsymm.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      148 2017-06-22 10:27:41.000000 kwant-1.4.4/doc/source/reference/kwant.rmt.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     1597 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/source/reference/kwant.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      878 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/source/reference/kwant.solvers.mumps.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     2971 2017-06-22 10:27:41.000000 kwant-1.4.4/doc/source/reference/kwant.solvers.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      680 2019-03-29 14:02:16.000000 kwant-1.4.4/doc/source/reference/kwant.solvers.sparse.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     1042 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/source/reference/kwant.system.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      238 2019-03-29 14:02:16.000000 kwant-1.4.4/doc/source/reference/kwant.wraparound.rst
+drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2023-07-03 13:46:37.604252 kwant-1.4.4/doc/source/tutorial/
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    12120 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/source/tutorial/discretize.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    19888 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/source/tutorial/faq.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    20208 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/source/tutorial/first_steps.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     7023 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/source/tutorial/graphene.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      260 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/source/tutorial/index.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     4303 2019-03-29 14:02:16.000000 kwant-1.4.4/doc/source/tutorial/introduction.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    16914 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/source/tutorial/kpm.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    14857 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/source/tutorial/operators.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     9829 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/source/tutorial/plotting.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     5994 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/source/tutorial/spectrum.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    14806 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/source/tutorial/spin_potential_shape.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    10261 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/source/tutorial/superconductors.rst
+drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2023-07-03 13:46:37.604252 kwant-1.4.4/doc/sphinxext/
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     2498 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/sphinxext/kwantdoc.py
+drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2023-07-03 13:46:37.604252 kwant-1.4.4/doc/templates/
+drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2023-07-03 13:46:37.604252 kwant-1.4.4/doc/templates/autosummary/
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      550 2021-11-01 14:15:02.000000 kwant-1.4.4/doc/templates/autosummary/class.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      206 2019-03-29 14:02:16.000000 kwant-1.4.4/doc/templates/autosummary/functor.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     8834 2023-06-30 16:40:53.000000 kwant-1.4.4/doc/templates/layout.html
+drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2023-07-03 13:46:37.608252 kwant-1.4.4/docker/
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      633 2023-06-30 16:40:53.000000 kwant-1.4.4/docker/Dockerfile.conda
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     1180 2023-06-30 16:40:53.000000 kwant-1.4.4/docker/Dockerfile.debian
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     1005 2023-06-30 16:40:53.000000 kwant-1.4.4/docker/Dockerfile.ubuntu
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     2184 2020-03-31 22:06:32.000000 kwant-1.4.4/docker/README.rst
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      535 2023-06-30 16:40:53.000000 kwant-1.4.4/docker/kwant-latest.yml
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      576 2023-06-30 16:40:53.000000 kwant-1.4.4/docker/kwant-stable-no-extras.yml
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      619 2023-06-30 16:40:53.000000 kwant-1.4.4/docker/kwant-stable.yml
+drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2023-07-03 13:46:37.608252 kwant-1.4.4/examples/
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      713 2019-03-29 14:02:16.000000 kwant-1.4.4/examples/3d_plot.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     1267 2021-03-16 21:28:08.000000 kwant-1.4.4/examples/advanced_construction.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     3988 2020-03-31 22:06:32.000000 kwant-1.4.4/examples/square.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     1300 2019-03-29 14:02:16.000000 kwant-1.4.4/examples/test_square.py
+drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2023-07-03 13:46:37.708252 kwant-1.4.4/kwant/
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     2342 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/__init__.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    13420 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/_colormaps.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     6768 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/_common.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)       60 2023-07-03 13:46:37.708252 kwant-1.4.4/kwant/_kwant_version.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    14211 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/_plotter.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)  1530224 2023-06-30 16:41:32.000000 kwant-1.4.4/kwant/_system.c
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    13346 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/_system.pyx
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    88604 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/builder.py
+drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2023-07-03 13:46:37.632252 kwant-1.4.4/kwant/continuum/
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      913 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/continuum/__init__.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     9883 2023-06-30 16:41:04.000000 kwant-1.4.4/kwant/continuum/_common.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    26428 2023-06-30 16:41:04.000000 kwant-1.4.4/kwant/continuum/discretizer.py
+drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2023-07-03 13:46:37.632252 kwant-1.4.4/kwant/continuum/tests/
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)        0 2019-03-29 14:02:16.000000 kwant-1.4.4/kwant/continuum/tests/__init__.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     5953 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/continuum/tests/test_common.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    21593 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/continuum/tests/test_discretizer.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     3079 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/digest.py
+drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2023-07-03 13:46:37.648252 kwant-1.4.4/kwant/graph/
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      655 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/graph/__init__.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     8464 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/graph/c_scotch.pxd
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)   892233 2023-06-30 16:41:32.000000 kwant-1.4.4/kwant/graph/core.c
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     1684 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/graph/core.pxd
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    25352 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/graph/core.pyx
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      570 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/graph/defs.h
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      440 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/graph/defs.pxd
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      450 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/graph/defs.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)  1147239 2022-09-07 12:44:55.000000 kwant-1.4.4/kwant/graph/dijkstra.c
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    12933 2022-09-07 12:44:17.000000 kwant-1.4.4/kwant/graph/dijkstra.pyx
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     2366 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/graph/scotch.pyx
+drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2023-07-03 13:46:37.648252 kwant-1.4.4/kwant/graph/tests/
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)        0 2017-05-24 08:50:37.000000 kwant-1.4.4/kwant/graph/tests/__init__.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     6617 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/graph/tests/test_core.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     1864 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/graph/tests/test_scotch.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    46860 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/kpm.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    30002 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/lattice.py
+drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2023-07-03 13:46:37.684252 kwant-1.4.4/kwant/linalg/
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      685 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/linalg/__init__.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)   622040 2023-06-30 16:41:33.000000 kwant-1.4.4/kwant/linalg/_mumps.c
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     6431 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/linalg/_mumps.pyx
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     1576 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/linalg/cmumps.pxd
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      425 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/linalg/cmumps.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     2012 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/linalg/decomp_ev.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     4018 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/linalg/decomp_lu.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    24952 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/linalg/decomp_schur.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     4849 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/linalg/fortran_helpers.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)  3683037 2023-06-30 16:41:38.000000 kwant-1.4.4/kwant/linalg/lapack.c
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    45136 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/linalg/lapack.pyx
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    11857 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/linalg/lll.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    20232 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/linalg/mumps.py
+drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2023-07-03 13:46:37.688252 kwant-1.4.4/kwant/linalg/tests/
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)        0 2017-05-24 08:50:37.000000 kwant-1.4.4/kwant/linalg/tests/__init__.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     2682 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/linalg/tests/_test_utils.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    14143 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/linalg/tests/test_linalg.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     2713 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/linalg/tests/test_lll.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     2832 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/linalg/tests/test_mumps.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)  2402213 2023-06-30 16:41:40.000000 kwant-1.4.4/kwant/operator.c
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     1327 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/operator.pxd
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    46358 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/operator.pyx
+drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2023-07-03 13:46:37.688252 kwant-1.4.4/kwant/physics/
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      692 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/physics/__init__.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     6874 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/physics/dispersion.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    40281 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/physics/gauge.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    53515 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/physics/leads.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     1772 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/physics/noise.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     9896 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/physics/symmetry.py
+drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2023-07-03 13:46:37.692252 kwant-1.4.4/kwant/physics/tests/
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)        0 2017-05-24 08:50:37.000000 kwant-1.4.4/kwant/physics/tests/__init__.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     5265 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/physics/tests/test_dispersion.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    18141 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/physics/tests/test_gauge.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    51169 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/physics/tests/test_leads.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     1743 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/physics/tests/test_noise.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     9371 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/physics/tests/test_symmetry.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    89709 2023-06-30 16:41:04.000000 kwant-1.4.4/kwant/plotter.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    19219 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/qsymm.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     9966 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/rmt.py
+drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2023-07-03 13:46:37.696252 kwant-1.4.4/kwant/solvers/
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      608 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/solvers/__init__.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    41368 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/solvers/common.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     1006 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/solvers/default.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     4908 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/solvers/mumps.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     3814 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/solvers/sparse.py
+drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2023-07-03 13:46:37.696252 kwant-1.4.4/kwant/solvers/tests/
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)        0 2017-05-24 08:50:37.000000 kwant-1.4.4/kwant/solvers/tests/__init__.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    20724 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/solvers/tests/_test_sparse.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     3192 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/solvers/tests/test_mumps.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     1804 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/solvers/tests/test_sparse.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    17528 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/system.py
+drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2023-07-03 13:46:37.704252 kwant-1.4.4/kwant/tests/
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)        0 2017-05-24 08:50:37.000000 kwant-1.4.4/kwant/tests/__init__.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    50575 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/tests/test_builder.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     1841 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/tests/test_comprehensive.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    24671 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/tests/test_kpm.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    10693 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/tests/test_lattice.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    19293 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/tests/test_operator.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    19932 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/tests/test_plotter.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    21984 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/tests/test_qsymm.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     4383 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/tests/test_rmt.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     3827 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/tests/test_system.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    15297 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/tests/test_wraparound.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     4355 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/version.py
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)    18404 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant/wraparound.py
+drwxrwxr-x   0 cwg       (1000) cwg       (1000)        0 2023-07-03 13:46:37.632252 kwant-1.4.4/kwant.egg-info/
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     2655 2023-07-03 13:46:36.000000 kwant-1.4.4/kwant.egg-info/PKG-INFO
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     5820 2023-07-03 13:46:37.000000 kwant-1.4.4/kwant.egg-info/SOURCES.txt
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)        1 2023-07-03 13:46:36.000000 kwant-1.4.4/kwant.egg-info/dependency_links.txt
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      121 2023-07-03 13:46:36.000000 kwant-1.4.4/kwant.egg-info/requires.txt
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)        6 2023-07-03 13:46:36.000000 kwant-1.4.4/kwant.egg-info/top_level.txt
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)     2614 2023-06-30 16:40:53.000000 kwant-1.4.4/kwant_red.jscm
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)      201 2023-06-30 16:40:53.000000 kwant-1.4.4/pytest.ini
+-rw-rw-r--   0 cwg       (1000) cwg       (1000)       59 2023-07-03 13:46:37.708252 kwant-1.4.4/setup.cfg
+-rwxrwxr-x   0 cwg       (1000) cwg       (1000)    20805 2023-06-30 16:40:53.000000 kwant-1.4.4/setup.py
```

### Comparing `kwant-1.4.3/.gitlab-ci.yml` & `kwant-1.4.4/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/.mailmap` & `kwant-1.4.4/.mailmap`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/AUTHORS.rst` & `kwant-1.4.4/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/CITING.rst` & `kwant-1.4.4/CITING.rst`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/CONTRIBUTE.rst` & `kwant-1.4.4/CONTRIBUTE.rst`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/INSTALL.rst` & `kwant-1.4.4/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/LICENSE.rst` & `kwant-1.4.4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/MANIFEST.in` & `kwant-1.4.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/PKG-INFO` & `kwant-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kwant
-Version: 1.4.3
+Version: 1.4.4
 Summary: Package for numerical quantum transport calculations (Python 3 version)
 Home-page: http://kwant-project.org/
 Author: C. W. Groth (CEA), M. Wimmer, A. R. Akhmerov, X. Waintal (CEA), and others
 Author-email: authors@kwant-project.org
 License: BSD
 Description: Kwant is a free (open source) Python package for numerical calculations on
         tight-binding models with a strong focus on quantum transport. It is designed to
```

### Comparing `kwant-1.4.3/README.rst` & `kwant-1.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/RELEASE.rst` & `kwant-1.4.4/RELEASE.rst`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/conftest.py` & `kwant-1.4.4/conftest.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/Makefile` & `kwant-1.4.4/doc/Makefile`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/kwantdoctheme/static/kwantdoctheme.css` & `kwant-1.4.4/doc/kwantdoctheme/static/kwantdoctheme.css`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/kwantdoctheme/theme.conf` & `kwant-1.4.4/doc/kwantdoctheme/theme.conf`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/_static/kwant.css` & `kwant-1.4.4/doc/source/_static/kwant.css`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/_static/kwant_logo.png` & `kwant-1.4.4/doc/source/_static/kwant_logo.png`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/_static/sidebar.js` & `kwant-1.4.4/doc/source/_static/sidebar.js`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/code/README` & `kwant-1.4.4/doc/source/code/README`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/code/figure/_defs.py` & `kwant-1.4.4/doc/source/code/figure/_defs.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/code/figure/ab_ring.py.diff` & `kwant-1.4.4/doc/source/code/figure/ab_ring.py.diff`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/code/figure/ab_ring_sketch.svg` & `kwant-1.4.4/doc/source/code/figure/ab_ring_sketch.svg`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/code/figure/ab_ring_sketch2.svg` & `kwant-1.4.4/doc/source/code/figure/ab_ring_sketch2.svg`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/code/figure/band_structure.py.diff` & `kwant-1.4.4/doc/source/code/figure/band_structure.py.diff`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/code/figure/closed_system.py.diff` & `kwant-1.4.4/doc/source/code/figure/closed_system.py.diff`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/code/figure/discretize.py.diff` & `kwant-1.4.4/doc/source/code/figure/discretize.py.diff`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/code/figure/faq.py.diff` & `kwant-1.4.4/doc/source/code/figure/faq.py.diff`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/code/figure/graphene.py.diff` & `kwant-1.4.4/doc/source/code/figure/graphene.py.diff`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/code/figure/kernel_polynomial_method.py.diff` & `kwant-1.4.4/doc/source/code/figure/kernel_polynomial_method.py.diff`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/code/figure/magnetic_texture.py.diff` & `kwant-1.4.4/doc/source/code/figure/magnetic_texture.py.diff`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/code/figure/plot_graphene.py.diff` & `kwant-1.4.4/doc/source/code/figure/plot_graphene.py.diff`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/code/figure/plot_qahe.py.diff` & `kwant-1.4.4/doc/source/code/figure/plot_qahe.py.diff`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/code/figure/plot_zincblende.py.diff` & `kwant-1.4.4/doc/source/code/figure/plot_zincblende.py.diff`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/code/figure/quantum_well.py.diff` & `kwant-1.4.4/doc/source/code/figure/quantum_well.py.diff`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/code/figure/quantum_wire.py.diff` & `kwant-1.4.4/doc/source/code/figure/quantum_wire.py.diff`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/code/figure/spin_orbit.py.diff` & `kwant-1.4.4/doc/source/code/figure/spin_orbit.py.diff`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/code/figure/superconductor.py.diff` & `kwant-1.4.4/doc/source/code/figure/superconductor.py.diff`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/code/figure/superconductor_transport_sketch.svg` & `kwant-1.4.4/doc/source/code/figure/superconductor_transport_sketch.svg`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/code/include/quantum_wire_revisited.py` & `kwant-1.4.4/doc/source/code/include/quantum_wire_revisited.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/conf.py` & `kwant-1.4.4/doc/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,16 +235,17 @@
 latex_domain_indices = False
 
 # -- Options for autodoc -------------------------------------------------------
 # Generate stub pages for autosummary directives.
 autosummary_generate = True
 
 autoclass_content = "both"
-autodoc_default_flags = ['show-inheritance']
-
+autodoc_default_options = {
+    'show-inheritance': True,
+}
 
 # -- Teach Sphinx to document bound methods like functions ---------------------
 import types
 from sphinx.ext import autodoc
 
 class BoundMethodDocumenter(autodoc.FunctionDocumenter):
     objtype = "boundmethod"
```

### Comparing `kwant-1.4.3/doc/source/pre/whatsnew/0.2.rst` & `kwant-1.4.4/doc/source/pre/whatsnew/0.2.rst`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/pre/whatsnew/1.0.rst` & `kwant-1.4.4/doc/source/pre/whatsnew/1.0.rst`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/pre/whatsnew/1.1.rst` & `kwant-1.4.4/doc/source/pre/whatsnew/1.1.rst`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/pre/whatsnew/1.2.rst` & `kwant-1.4.4/doc/source/pre/whatsnew/1.2.rst`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/pre/whatsnew/1.3.rst` & `kwant-1.4.4/doc/source/pre/whatsnew/1.3.rst`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/pre/whatsnew/1.4.rst` & `kwant-1.4.4/doc/source/pre/whatsnew/1.4.rst`

 * *Files 2% similar despite different names*

```diff
@@ -350,7 +350,12 @@
 Changes in Kwant 1.4.3
 ----------------------
 - Builder properly handles Hermitian conjugation of array-like values.
   Before, if the value was provided not as a true array but, for example, as a
   list of lists, it was not conjugated, which could lead to generation of a
   non-Hermitian Hamiltonian matrix without emitting any error.
 - Various maintenance.
+
+Changes in Kwant 1.4.4
+----------------------
+- Ensure compatibility with recent versions of SymPy, matplotlib and Sphinx.
+- Fix current density plotting when sites coincide.
```

### Comparing `kwant-1.4.3/doc/source/reference/index.rst` & `kwant-1.4.4/doc/source/reference/index.rst`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/reference/kwant.graph.rst` & `kwant-1.4.4/doc/source/reference/kwant.graph.rst`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/reference/kwant.linalg.rst` & `kwant-1.4.4/doc/source/reference/kwant.linalg.rst`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/reference/kwant.physics.rst` & `kwant-1.4.4/doc/source/reference/kwant.physics.rst`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/reference/kwant.rst` & `kwant-1.4.4/doc/source/reference/kwant.rst`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/reference/kwant.solvers.mumps.rst` & `kwant-1.4.4/doc/source/reference/kwant.solvers.mumps.rst`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/reference/kwant.solvers.rst` & `kwant-1.4.4/doc/source/reference/kwant.solvers.rst`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/reference/kwant.solvers.sparse.rst` & `kwant-1.4.4/doc/source/reference/kwant.solvers.sparse.rst`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/reference/kwant.system.rst` & `kwant-1.4.4/doc/source/reference/kwant.system.rst`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/tutorial/discretize.rst` & `kwant-1.4.4/doc/source/tutorial/discretize.rst`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/tutorial/faq.rst` & `kwant-1.4.4/doc/source/tutorial/faq.rst`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/tutorial/first_steps.rst` & `kwant-1.4.4/doc/source/tutorial/first_steps.rst`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/tutorial/graphene.rst` & `kwant-1.4.4/doc/source/tutorial/graphene.rst`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/tutorial/introduction.rst` & `kwant-1.4.4/doc/source/tutorial/introduction.rst`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/tutorial/kpm.rst` & `kwant-1.4.4/doc/source/tutorial/kpm.rst`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/tutorial/operators.rst` & `kwant-1.4.4/doc/source/tutorial/operators.rst`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/tutorial/plotting.rst` & `kwant-1.4.4/doc/source/tutorial/plotting.rst`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/tutorial/spectrum.rst` & `kwant-1.4.4/doc/source/tutorial/spectrum.rst`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/tutorial/spin_potential_shape.rst` & `kwant-1.4.4/doc/source/tutorial/spin_potential_shape.rst`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/source/tutorial/superconductors.rst` & `kwant-1.4.4/doc/source/tutorial/superconductors.rst`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/sphinxext/kwantdoc.py` & `kwant-1.4.4/doc/sphinxext/kwantdoc.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/templates/autosummary/class.rst` & `kwant-1.4.4/doc/templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/doc/templates/layout.html` & `kwant-1.4.4/doc/templates/layout.html`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/docker/Dockerfile.conda` & `kwant-1.4.4/docker/Dockerfile.conda`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/docker/Dockerfile.debian` & `kwant-1.4.4/docker/Dockerfile.debian`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/docker/Dockerfile.ubuntu` & `kwant-1.4.4/docker/Dockerfile.ubuntu`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/docker/README.rst` & `kwant-1.4.4/docker/README.rst`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/docker/kwant-latest.yml` & `kwant-1.4.4/docker/kwant-latest.yml`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/docker/kwant-stable-no-extras.yml` & `kwant-1.4.4/docker/kwant-stable-no-extras.yml`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/docker/kwant-stable.yml` & `kwant-1.4.4/docker/kwant-stable.yml`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/examples/3d_plot.py` & `kwant-1.4.4/examples/3d_plot.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/examples/advanced_construction.py` & `kwant-1.4.4/examples/advanced_construction.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/examples/square.py` & `kwant-1.4.4/examples/square.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/examples/test_square.py` & `kwant-1.4.4/examples/test_square.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/__init__.py` & `kwant-1.4.4/kwant/__init__.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/_colormaps.py` & `kwant-1.4.4/kwant/_colormaps.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/_common.py` & `kwant-1.4.4/kwant/_common.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/_plotter.py` & `kwant-1.4.4/kwant/_plotter.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,25 +18,32 @@
 import warnings
 from math import sqrt, pi
 import numpy as np
 
 try:
     import matplotlib
     import matplotlib.colors
-    import matplotlib.cm
     from matplotlib.figure import Figure
     from matplotlib import collections
     from . import _colormaps
     mpl_available = True
     try:
         from mpl_toolkits import mplot3d
         has3d = True
     except ImportError:
         warnings.warn("3D plotting not available.", RuntimeWarning)
         has3d = False
+
+    # TODO: remove the try statement (leaving only the try clause)
+    # once we depend on matplotlib >= 3.5.0
+    try:
+        get_cmap = matplotlib.colormaps.get_cmap
+    except AttributeError:
+        from matplotlib.cm import get_cmap
+
 except ImportError:
     warnings.warn("matplotlib is not available, only iterator-providing "
                   "functions will work.", RuntimeWarning)
     mpl_available = False
 
 
 # Collections that allow for symbols and linewiths to be given in data space
@@ -153,15 +160,20 @@
                 self.reflen = reflen
                 self.zorder3d = zorder
 
             def set_linewidths(self, linewidths):
                 self.linewidths_orig = nparray_if_array(linewidths)
 
             def do_3d_projection(self, renderer=None):
-                super().do_3d_projection(renderer)
+                # TODO: remove the try once we depend on matplotlib >= 3.6.0
+                try:
+                    super().do_3d_projection(renderer)
+                except TypeError:
+                    super().do_3d_projection()
+
                 # The whole 3D ordering is flawed in mplot3d when several
                 # collections are added. We just use normal zorder. Note the
                 # "-" due to the different logic in the 3d plotting, we still
                 # want larger zorder values to be plotted on top of smaller
                 # ones.
                 return -self.zorder3d
```

### Comparing `kwant-1.4.3/kwant/_system.c` & `kwant-1.4.4/kwant/_system.c`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/_system.pyx` & `kwant-1.4.4/kwant/_system.pyx`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/builder.py` & `kwant-1.4.4/kwant/builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1813,23 +1813,24 @@
         else:
             raise ValueError('Currently, only builders without or with a 1D '
                              'translational symmetry can be finalized.')
 
     # Protect novice users from confusing error messages if they
     # forget to finalize their Builder.
 
-    @staticmethod
-    def _require_system(*args, **kwargs):
-        """You need a finalized system; Use Builder.finalized() first."""
-        raise TypeError('You need a finalized system; '
-                        'use Builder.finalized() first.')
+    _system_methods = {
+        "hamiltonian", "hamiltonian_submatrix", "modes", "selfenergy",
+        "inter_cell_hopping", "cell_hamiltonian", "precalculated"}
 
-    hamiltonian = hamiltonian_submatrix = modes = selfenergy = \
-    inter_cell_hopping = cell_hamiltonian = precalculated = \
-    _require_system
+    def __getattr__(self, name):
+        msg = "'Builder' object has no attribute '{}'.".format(name)
+        if name in self._system_methods:
+            msg += ("\nIt looks like you need a finalized system; "
+                    "use Builder.finalized() first.")
+        raise AttributeError(msg)
 
 
 ################ Finalized systems
 
 def _raise_user_error(exc, func):
     msg = ('Error occurred in user-supplied value function "{0}".\n'
            'See the upper part of the above backtrace for more information.')
```

### Comparing `kwant-1.4.3/kwant/continuum/__init__.py` & `kwant-1.4.4/kwant/continuum/__init__.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/continuum/_common.py` & `kwant-1.4.4/kwant/continuum/_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,24 +12,21 @@
 import numpy as np
 
 import sympy
 import sympy.abc
 import sympy.physics.quantum
 from sympy.core.function import AppliedUndef
 from sympy.core.sympify import converter
-from sympy.core.core import all_classes as sympy_classes
+from sympy.core import Basic
 from sympy.physics.matrices import msigma as _msigma
 
 import warnings
 
 from .._common import reraise_warnings
 
-# TODO: remove when sympy correctly includes MutableDenseMatrix (lol).
-sympy_classes = set(sympy_classes) | {sympy.MutableDenseMatrix}
-
 momentum_operators = sympy.symbols('k_x k_y k_z', commutative=False)
 position_operators = sympy.symbols('x y z', commutative=False)
 
 pauli = [sympy.eye(2), _msigma(1), _msigma(2), _msigma(3)]
 
 extra_ns = sympy.abc._clash.copy()
 extra_ns.update({s.name: s for s in momentum_operators})
@@ -148,15 +145,15 @@
         >>> sympify('k_x * A(c) * k_x', locals={'c': sympy.Symbol('x')})
         A(x)*k_x**2
 
     """
     stored_value = None
 
     # if ``expr`` is already a ``sympy`` object we may terminate a code path
-    if isinstance(expr, tuple(sympy_classes)):
+    if isinstance(expr, Basic):
         if locals:
             warnings.warn('Input expression is already SymPy object: '
                           '"locals" will not be used.',
                           RuntimeWarning,
                           stacklevel=2)
 
         # We assume that all present functions, like "sin", "cos", will be
```

### Comparing `kwant-1.4.3/kwant/continuum/discretizer.py` & `kwant-1.4.4/kwant/continuum/discretizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -313,15 +313,15 @@
     # run sympifcation on hamiltonian values
     with reraise_warnings():
         for k, v in tb_hamiltonian.items():
             tb_hamiltonian[k] = sympify(v, locals)
 
     # generate grid if required, check constraints if provided
     random_element = next(iter(tb_hamiltonian.values()))
-    norbs = (1 if isinstance(random_element, sympy.Expr)
+    norbs = (1 if not isinstance(random_element, sympy.MatrixExpr)
              else random_element.shape[0])
 
     if np.isscalar(grid):
         lat = lattice.Monatomic(grid * np.eye(grid_dim), norbs=norbs)
     else:
         lat = grid
```

### Comparing `kwant-1.4.3/kwant/continuum/tests/test_common.py` & `kwant-1.4.4/kwant/continuum/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/continuum/tests/test_discretizer.py` & `kwant-1.4.4/kwant/continuum/tests/test_discretizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,47 +47,47 @@
 x, y, z = sympy.symbols('x y z', commutative=False)
 ax, ay, az = sympy.symbols('a_x a_y a_z')
 a = sympy.symbols('a')
 
 wf = _wf
 Psi = wf(x, y, z)
 A, B = sympy.symbols('A B', commutative=False)
-fA, fB = sympy.symbols('A B', cls=sympy.Function)
+F, G = sympy.symbols('F G', cls=sympy.Function)
 
 ns = {'A': A, 'B': B, 'a_x': ax, 'a_y': ay, 'az': az, 'x': x, 'y': y, 'z': z}
 
 
 @pytest.mark.parametrize('commutative', [True, False])
 def test_reading_coordinates(commutative):
     kx, ky, kz = sympy.symbols('k_x k_y k_z', commutative=commutative)
 
     test = {
         kx**2                         : ['x'],
         kx**2 + ky**2                 : ['x', 'y'],
         kx**2 + ky**2 + kz**2         : ['x', 'y', 'z'],
         ky**2 + kz**2                 : ['y', 'z'],
         kz**2                         : ['z'],
-        kx * fA(x, y) * kx              : ['x'],
-        kx**2 + kz * fB(y)             : ['x', 'z'],
+        kx * F(x, y) * kx              : ['x'],
+        kx**2 + kz * G(y)             : ['x', 'z'],
     }
     for inp, out in test.items():
         ham, got = discretize_symbolic(inp)
         assert got == out
 
 
 def test_reading_coordinates_matrix():
     test = [
         (sympy.Matrix([sympy.sympify('k_x**2')])      , ['x']),
         (sympy.Matrix([kx**2])                        , ['x']),
         (sympy.Matrix([kx**2 + ky**2])                , ['x', 'y']),
         (sympy.Matrix([kx**2 + ky**2 + kz**2])        , ['x', 'y', 'z']),
         (sympy.Matrix([ky**2 + kz**2])                , ['y', 'z']),
         (sympy.Matrix([kz**2])                        , ['z']),
-        (sympy.Matrix([kx * fA(x, y) * kx])            , ['x']),
-        (sympy.Matrix([kx**2 + kz * fB(y)])            , ['x', 'z']),
+        (sympy.Matrix([kx * F(x, y) * kx])            , ['x']),
+        (sympy.Matrix([kx**2 + kz * G(y)])            , ['x', 'z']),
     ]
     for inp, out in test:
         ham, got = discretize_symbolic(inp)
         assert got == out
 
 
 def test_reading_different_matrix_types():
@@ -118,24 +118,24 @@
                                    (0, 0, 0): 2/ax**2 + 2/ay**2 + 2/az**2,
                                    (0, 1, 0): -1/ay**2},
         ky**2 + kz**2           : {(0, 1): -1/az**2, (0, 0): 2/ay**2 + 2/az**2,
                                    (1, 0): -1/ay**2},
         kz**2                   : {(0,): 2/az**2, (1,): -1/az**2},
     }
     non_commutative_test = {
-        kx * fA(x, y) * kx       : {(1, ): -fA(ax/2 + x, y)/ax**2,
-                                  (0, ): fA(-ax/2 + x, y)/ax**2 + fA(ax/2 + x, y)/ax**2},
-        kx**2 + kz * fB(y)       : {(1, 0): -1/ax**2, (0, 1): -I*fB(y)/(2*az),
+        kx * F(x, y) * kx       : {(1, ): -F(ax/2 + x, y)/ax**2,
+                                  (0, ): F(-ax/2 + x, y)/ax**2 + F(ax/2 + x, y)/ax**2},
+        kx**2 + kz * G(y)       : {(1, 0): -1/ax**2, (0, 1): -I*G(y)/(2*az),
                                    (0, 0): 2/ax**2},
-        kx * fA(x)               : {(0,): 0, (1,): -I*fA(ax + x)/(2*ax)},
-        ky * fA(x)               : {(1,): -I*fA(x)/(2*ay), (0,): 0},
-        kx * fA(x) * B           : {(0,): 0, (1,): -I*fA(ax + x)*B/(2*ax)},
+        kx * F(x)               : {(0,): 0, (1,): -I*F(ax + x)/(2*ax)},
+        ky * F(x)               : {(1,): -I*F(x)/(2*ay), (0,): 0},
+        kx * F(x) * B           : {(0,): 0, (1,): -I*F(ax + x)*B/(2*ax)},
         5 * kx                  : {(0,): 0, (1,): -5*I/(2*ax)},
-        kx * (fA(x) + fB(x))      : {(0,): 0,
-                                   (1,): -I*fA(ax + x)/(2*ax) - I*fB(ax + x)/(2*ax)},
+        kx * (F(x) + G(x))      : {(0,): 0,
+                                   (1,): -I*F(ax + x)/(2*ax) - I*G(ax + x)/(2*ax)},
     }
 
     if not commutative:
         test.update(non_commutative_test)
 
     for inp, out in test.items():
         got, _ = discretize_symbolic(inp)
@@ -167,24 +167,24 @@
         kx**2 + ky**2 + kz**2   : {(1, 0, 0): -1/ax**2, (0, 0, 1): -1/az**2,
                                    (0, 0, 0): 2/ax**2 + 2/ay**2 + 2/az**2,
                                    (0, 1, 0): -1/ay**2},
         ky**2 + kz**2           : {(0, 1): -1/az**2, (0, 0): 2/ay**2 + 2/az**2,
                                    (1, 0): -1/ay**2},
         kz**2                   : {(0,): 2/az**2, (1,): -1/az**2},
 
-        kx * fA(x, y) * kx       : {(1, ): -fA(ax/2 + x, y)/ax**2,
-                                  (0, ): fA(-ax/2 + x, y)/ax**2 + fA(ax/2 + x, y)/ax**2},
-        kx**2 + kz * fB(y)       : {(1, 0): -1/ax**2, (0, 1): -I*fB(y)/(2*az),
+        kx * F(x, y) * kx       : {(1, ): -F(ax/2 + x, y)/ax**2,
+                                  (0, ): F(-ax/2 + x, y)/ax**2 + F(ax/2 + x, y)/ax**2},
+        kx**2 + kz * G(y)       : {(1, 0): -1/ax**2, (0, 1): -I*G(y)/(2*az),
                                    (0, 0): 2/ax**2},
-        kx * fA(x)               : {(0,): 0, (1,): -I*fA(ax + x)/(2*ax)},
-        ky * fA(x)               : {(1,): -I*fA(x)/(2*ay), (0,): 0},
-        kx * fA(x) * B           : {(0,): 0, (1,): -I*fA(ax + x)*B/(2*ax)},
+        kx * F(x)               : {(0,): 0, (1,): -I*F(ax + x)/(2*ax)},
+        ky * F(x)               : {(1,): -I*F(x)/(2*ay), (0,): 0},
+        kx * F(x) * B           : {(0,): 0, (1,): -I*F(ax + x)*B/(2*ax)},
         5 * kx                  : {(0,): 0, (1,): -5*I/(2*ax)},
-        kx * (fA(x) + fB(x))      : {(0,): 0,
-                                   (1,): -I*fA(ax + x)/(2*ax) - I*fB(ax + x)/(2*ax)},
+        kx * (F(x) + G(x))      : {(0,): 0,
+                                   (1,): -I*F(ax + x)/(2*ax) - I*G(ax + x)/(2*ax)},
    }
 
     new_test = []
     for inp, out in test.items():
         new_out = {}
         for k, v in out.items():
             new_out[k] = sympy.Matrix([v])
@@ -293,28 +293,28 @@
 
     for inp, out in new_test:
         got, _ = discretize_symbolic(sympy.Matrix([kx**2 + ky**2 + kz**2]), inp)
         assert got == out
 
 
 def test_non_expended_input():
-    symbolic, coords = discretize_symbolic(kx * (kx + fA(x)))
+    symbolic, coords = discretize_symbolic(kx * (kx + F(x)))
     desired = {
         (0,): 2/ax**2,
-        (1,): -I*fA(ax + x)/(2*ax) - 1/ax**2
+        (1,): -I*F(ax + x)/(2*ax) - 1/ax**2
     }
     assert symbolic == desired
 
 
 def test_matrix_with_zeros():
     Matrix = sympy.Matrix
-    symbolic, _ = discretize_symbolic("[[k_x*A(x)*k_x, 0], [0, k_x*A(x)*k_x]]")
+    symbolic, _ = discretize_symbolic("[[k_x*F(x)*k_x, 0], [0, k_x*F(x)*k_x]]")
     output = {
-        (0,):  Matrix([[fA(-ax/2 + x)/ax**2 + fA(ax/2 + x)/ax**2, 0], [0, fA(-ax/2 + x)/ax**2 + fA(ax/2 + x)/ax**2]]),
-        (1,):  Matrix([[-fA(ax/2 + x)/ax**2, 0], [0, -fA(ax/2 + x)/ax**2]]),
+        (0,):  Matrix([[F(-ax/2 + x)/ax**2 + F(ax/2 + x)/ax**2, 0], [0, F(-ax/2 + x)/ax**2 + F(ax/2 + x)/ax**2]]),
+        (1,):  Matrix([[-F(ax/2 + x)/ax**2, 0], [0, -F(ax/2 + x)/ax**2]]),
         }
     assert symbolic == output
 
 
 def test_numeric_functions_basic_symbolic():
     for i in [0, 1, 3, 5]:
         builder = discretize(i, 'x')
@@ -425,81 +425,81 @@
     assert 'def hopping' in template
 
 
 def test_numeric_functions_advance():
     hams = [
         kx**2,
         kx**2 + x,
-        fA(x),
-        kx*fA(x)*kx,
-        sympy.Matrix([[kx * fA(x) * kx, fA(x)*kx], [kx*fA(x), fA(x)+B]]),
+        F(x),
+        kx*F(x)*kx,
+        sympy.Matrix([[kx * F(x) * kx, F(x)*kx], [kx*F(x), F(x)+B]]),
         kx**2 + B * x,
         'k_x**2 + sin(x)',
         B ** 0.5 * kx**2,
         B ** (1/2) * kx**2,
         sympy.sqrt(B) * kx**2,
 
     ]
     for hamiltonian in hams:
         for a in [1, 2, 5]:
             for func in [lambda x: x, lambda x: x**2, lambda x: x**3]:
                 symbolic, coords = discretize_symbolic(hamiltonian, 'x')
                 builder = build_discretized(symbolic, coords, grid=a)
                 lat = next(iter(builder.sites()))[0]
 
-                p = dict(A=func, B=5, sin=np.sin)
+                p = dict(F=func, B=5, sin=np.sin)
 
                 # test onsite
                 v = symbolic.pop((0,)).subs({sympy.symbols('a_x'): a, B: p['B']})
-                f_sym = sympy.lambdify(['A', 'x'], v)
+                f_sym = sympy.lambdify(['F', 'x'], v)
                 f_num = builder[lat(0)]
 
                 if callable(f_num):
                     f_num = swallows_extra_kwargs(f_num)
                     for n in range(-100, 100, 10):
                         assert np.allclose(f_sym(func, a*n), f_num(lat(n), **p))
                 else:
                     for n in range(-100, 100, 10):
                         assert np.allclose(f_sym(func, a*n), f_num)
 
 
                 # test hoppings
                 for k, v in symbolic.items():
                     v = v.subs({sympy.symbols('a_x'): a, B: p['B']})
-                    f_sym = sympy.lambdify(['A', 'x'], v)
+                    f_sym = sympy.lambdify(['F', 'x'], v)
                     f_num = builder[lat(0), lat(k[0])]
 
                     if callable(f_num):
                         f_num = swallows_extra_kwargs(f_num)
                         for n in range(10):
                             lhs = f_sym(func, a * n)
                             rhs = f_num(lat(n), lat(n+k[0]), **p)
                             assert np.allclose(lhs, rhs)
                     else:
                         for n in range(10):
-                            lhs = f_sym(fA, a * n)
+                            lhs = f_sym(F, a * n)
                             rhs = f_num
                             assert np.allclose(lhs, rhs)
 
 
 def test_numeric_functions_with_parameter():
 
-    hamiltonian = kx**2 + fA(B, x)
+    hamiltonian = kx**2 + F(B, x)
 
     for a in [1, 2, 5]:
         for func in [lambda c, x: x+c, lambda c, x: x**2 + c]:
             symbolic, coords = discretize_symbolic(hamiltonian, 'x')
             builder = build_discretized(symbolic, coords, grid=a)
             lat = next(iter(builder.sites()))[0]
 
-            p = dict(A=func, B=5)
+            p = dict(F=func, B=5)
 
             # test onsite
             v = symbolic.pop((0,)).subs({sympy.symbols('a_x'): a, B: p['B']})
-            f_sym = sympy.lambdify(['A', 'x'], v)
+            f_sym = sympy.lambdify(['F', 'x'], v)
 
             f_num = builder[lat(0)]
             if callable(f_num):
                 f_num = swallows_extra_kwargs(f_num)
 
             for n in range(10):
                 s = lat(n)
```

### Comparing `kwant-1.4.3/kwant/digest.py` & `kwant-1.4.4/kwant/digest.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/graph/__init__.py` & `kwant-1.4.4/kwant/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/graph/c_scotch.pxd` & `kwant-1.4.4/kwant/graph/c_scotch.pxd`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/graph/core.c` & `kwant-1.4.4/kwant/graph/core.c`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/graph/core.pxd` & `kwant-1.4.4/kwant/graph/core.pxd`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/graph/core.pyx` & `kwant-1.4.4/kwant/graph/core.pyx`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/graph/defs.h` & `kwant-1.4.4/kwant/graph/defs.h`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/graph/dijkstra.c` & `kwant-1.4.4/kwant/graph/dijkstra.c`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/graph/dijkstra.pyx` & `kwant-1.4.4/kwant/graph/dijkstra.pyx`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/graph/scotch.pyx` & `kwant-1.4.4/kwant/graph/scotch.pyx`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/graph/tests/test_core.py` & `kwant-1.4.4/kwant/graph/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/graph/tests/test_scotch.py` & `kwant-1.4.4/kwant/graph/tests/test_scotch.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/kpm.py` & `kwant-1.4.4/kwant/kpm.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/lattice.py` & `kwant-1.4.4/kwant/lattice.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/linalg/__init__.py` & `kwant-1.4.4/kwant/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/linalg/_mumps.c` & `kwant-1.4.4/kwant/linalg/_mumps.c`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/linalg/_mumps.pyx` & `kwant-1.4.4/kwant/linalg/_mumps.pyx`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/linalg/cmumps.pxd` & `kwant-1.4.4/kwant/linalg/cmumps.pxd`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/linalg/decomp_ev.py` & `kwant-1.4.4/kwant/linalg/decomp_ev.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/linalg/decomp_lu.py` & `kwant-1.4.4/kwant/linalg/decomp_lu.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/linalg/decomp_schur.py` & `kwant-1.4.4/kwant/linalg/decomp_schur.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/linalg/fortran_helpers.py` & `kwant-1.4.4/kwant/linalg/fortran_helpers.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/linalg/lapack.c` & `kwant-1.4.4/kwant/linalg/lapack.c`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/linalg/lapack.pyx` & `kwant-1.4.4/kwant/linalg/lapack.pyx`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/linalg/lll.py` & `kwant-1.4.4/kwant/linalg/lll.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/linalg/mumps.py` & `kwant-1.4.4/kwant/linalg/mumps.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/linalg/tests/_test_utils.py` & `kwant-1.4.4/kwant/linalg/tests/_test_utils.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/linalg/tests/test_linalg.py` & `kwant-1.4.4/kwant/linalg/tests/test_linalg.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/linalg/tests/test_lll.py` & `kwant-1.4.4/kwant/linalg/tests/test_lll.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/linalg/tests/test_mumps.py` & `kwant-1.4.4/kwant/linalg/tests/test_mumps.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/operator.c` & `kwant-1.4.4/kwant/operator.c`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/operator.pxd` & `kwant-1.4.4/kwant/operator.pxd`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/operator.pyx` & `kwant-1.4.4/kwant/operator.pyx`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/physics/__init__.py` & `kwant-1.4.4/kwant/physics/__init__.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/physics/dispersion.py` & `kwant-1.4.4/kwant/physics/dispersion.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/physics/gauge.py` & `kwant-1.4.4/kwant/physics/gauge.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/physics/leads.py` & `kwant-1.4.4/kwant/physics/leads.py`

 * *Files 1% similar despite different names*

```diff
@@ -1011,23 +1011,25 @@
         anti-Hermitian term to the cell Hamiltonian before inverting. If it is
         set to `False`, the extra term will only be added if the cell
         Hamiltonian isn't invertible. The second element set to `True` forces
         Kwant to solve a generalized eigenvalue problem, and not to reduce it
         to the regular one.  If it is `False`, reduction to a regular problem
         is performed if possible.  Selecting the stabilization manually is
         mostly necessary for testing purposes.
-    particle_hole : sparse or dense square matrix
-        The unitary part of the particle-hole symmetry operator.
+    discrete_symmetry : `~kwant.physics.DiscreteSymmetry` or None
+        The discrete symmetry to use when performing the computation.
+    projectors : an iterable of sparse or dense matrices
+        Projectors that block diagonalize the Hamiltonian in accordance
+        with a conservation law.
     time_reversal : sparse or dense square matrix
         The unitary part of the time-reversal symmetry operator.
+    particle_hole : sparse or dense square matrix
+        The unitary part of the particle-hole symmetry operator.
     chiral : sparse or dense square matrix
         The chiral symmetry operator.
-    projectors : an iterable of sparse or dense matrices
-        Projectors that block diagonalize the Hamiltonian in accordance
-        with a conservation law.
 
     Returns
     -------
     propagating : `~kwant.physics.PropagatingModes`
         Contains the array of the wave functions of propagating modes, their
         momenta, and their velocities. It can be used to identify the gauge in
         which the scattering problem is solved.
```

### Comparing `kwant-1.4.3/kwant/physics/noise.py` & `kwant-1.4.4/kwant/physics/noise.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/physics/symmetry.py` & `kwant-1.4.4/kwant/physics/symmetry.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/physics/tests/test_dispersion.py` & `kwant-1.4.4/kwant/physics/tests/test_dispersion.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/physics/tests/test_gauge.py` & `kwant-1.4.4/kwant/physics/tests/test_gauge.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/physics/tests/test_leads.py` & `kwant-1.4.4/kwant/physics/tests/test_leads.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/physics/tests/test_noise.py` & `kwant-1.4.4/kwant/physics/tests/test_noise.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/physics/tests/test_symmetry.py` & `kwant-1.4.4/kwant/physics/tests/test_symmetry.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/plotter.py` & `kwant-1.4.4/kwant/plotter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1649,14 +1649,15 @@
     assert elements.shape[-1] == dim
     is_current = len(elements.shape) == 3
     if is_current:
         assert elements.shape[1] == 2
         dirs = elements[:, 1] - elements[:, 0]
         lens = np.sqrt(np.sum(dirs * dirs, axis=-1))
         dirs /= lens[:, None]
+        dirs = np.nan_to_num(dirs)
         lens = lens * scale
 
     if is_current:
         pos_offsets = elements[:, 0]  # first site in hopping
         kernel = current_kernel
     else:
         pos_offsets = elements  # sites themselves
@@ -1781,14 +1782,15 @@
     bbox_size = bbox_max - bbox_min
 
     # lens: scaled lengths of hoppings
     # dirs: normalized directions of hoppings
     dirs = hops[:, 1] - hops[:, 0]
     lens = np.sqrt(np.sum(dirs * dirs, -1))
     dirs /= lens[:, None]
+    dirs = np.nan_to_num(dirs)
     width = _optimal_width(lens, abswidth, relwidth, bbox_size)
 
 
     field, padding = _create_field(dim, bbox_size, width, n, is_current=True)
     boundaries = tuple((bbox_min[d] - padding, bbox_max[d] + padding)
                         for d in range(dim))
     _interpolate_field(dim, hops, current,
@@ -1994,15 +1996,15 @@
 
     if field.shape[-1] != 2 or field.ndim != 3:
         raise ValueError("Only 2D field can be plotted.")
 
     if bgcolor is None:
         if cmap is None:
             cmap = _p._colormaps.kwant_red
-        cmap = _p.matplotlib.cm.get_cmap(cmap)
+        cmap = _p.get_cmap(cmap)
         bgcolor = cmap(0)[:3]
     elif cmap is not None:
         raise ValueError("The parameters 'cmap' and 'bgcolor' are "
                          "mutually exclusive.")
 
     if ax is None:
         fig = _make_figure(dpi, fig_size, use_pyplot=(file is None))
@@ -2104,15 +2106,15 @@
     field = field.squeeze(axis=-1).transpose()
 
     if field.ndim != 2:
         raise ValueError("Only 2D field can be plotted.")
 
     if cmap is None:
         cmap = _p._colormaps.kwant_red
-    cmap = _p.matplotlib.cm.get_cmap(cmap)
+    cmap = _p.get_cmap(cmap)
 
     if ax is None:
         fig = _make_figure(dpi, fig_size, use_pyplot=(file is None))
         ax = fig.add_subplot(1, 1, 1, aspect='equal')
     else:
         fig = None
```

### Comparing `kwant-1.4.3/kwant/qsymm.py` & `kwant-1.4.4/kwant/qsymm.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/rmt.py` & `kwant-1.4.4/kwant/rmt.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/solvers/__init__.py` & `kwant-1.4.4/kwant/solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/solvers/common.py` & `kwant-1.4.4/kwant/solvers/common.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/solvers/default.py` & `kwant-1.4.4/kwant/solvers/default.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/solvers/mumps.py` & `kwant-1.4.4/kwant/solvers/mumps.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/solvers/sparse.py` & `kwant-1.4.4/kwant/solvers/sparse.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/solvers/tests/_test_sparse.py` & `kwant-1.4.4/kwant/solvers/tests/_test_sparse.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/solvers/tests/test_mumps.py` & `kwant-1.4.4/kwant/solvers/tests/test_mumps.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/solvers/tests/test_sparse.py` & `kwant-1.4.4/kwant/solvers/tests/test_sparse.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/system.py` & `kwant-1.4.4/kwant/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,17 @@
         """
         pass
 
     @deprecate_args
     def discrete_symmetry(self, args, *, params=None):
         """Return the discrete symmetry of the system.
 
+        The returned object is an instance of
+        `~kwant.physics.DiscreteSymmetry`.
+
         Providing positional arguments via 'args' is deprecated,
         instead, provide named parameters as a dictionary via 'params'.
         """
         # Avoid the circular import.
         from .physics import DiscreteSymmetry
         return DiscreteSymmetry()
 
@@ -285,16 +288,23 @@
         return self.hamiltonian_submatrix(args, cell_sites, interface_sites,
                                           sparse=sparse, params=params)
 
     @deprecate_args
     def modes(self, energy=0, args=(), *, params=None):
         """Return mode decomposition of the lead
 
-        See documentation of `~kwant.physics.PropagatingModes` and
-        `~kwant.physics.StabilizedModes` for the return format details.
+        This is a wrapper around `kwant.physics.modes`.  The said
+        function is applied to the infinite system at hand.  Any
+        discrete symmetries that are declared for the system are
+        validated, and, if present, passed on as well.  (Warnings are
+        emitted for declared symmetries that are broken.)
+
+        The result of the wrapped function (an instance of
+        `~kwant.physics.PropagatingModes` along with an instance of
+        `~kwant.physics.StabilizedModes`) is returned unchanged.
 
         The wave functions of the returned modes are defined over the
         *unit cell* of the system, which corresponds to the degrees of
         freedom on the first ``cell_sites`` sites of the system
         (recall that infinite systems store first the sites in the unit
         cell, then connected sites in the neighboring unit cell).
```

### Comparing `kwant-1.4.3/kwant/tests/test_builder.py` & `kwant-1.4.4/kwant/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/tests/test_comprehensive.py` & `kwant-1.4.4/kwant/tests/test_comprehensive.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/tests/test_kpm.py` & `kwant-1.4.4/kwant/tests/test_kpm.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/tests/test_lattice.py` & `kwant-1.4.4/kwant/tests/test_lattice.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/tests/test_operator.py` & `kwant-1.4.4/kwant/tests/test_operator.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/tests/test_plotter.py` & `kwant-1.4.4/kwant/tests/test_plotter.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/tests/test_qsymm.py` & `kwant-1.4.4/kwant/tests/test_qsymm.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/tests/test_rmt.py` & `kwant-1.4.4/kwant/tests/test_rmt.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/tests/test_system.py` & `kwant-1.4.4/kwant/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/tests/test_wraparound.py` & `kwant-1.4.4/kwant/tests/test_wraparound.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/version.py` & `kwant-1.4.4/kwant/version.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant/wraparound.py` & `kwant-1.4.4/kwant/wraparound.py`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant.egg-info/PKG-INFO` & `kwant-1.4.4/kwant.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kwant
-Version: 1.4.3
+Version: 1.4.4
 Summary: Package for numerical quantum transport calculations (Python 3 version)
 Home-page: http://kwant-project.org/
 Author: C. W. Groth (CEA), M. Wimmer, A. R. Akhmerov, X. Waintal (CEA), and others
 Author-email: authors@kwant-project.org
 License: BSD
 Description: Kwant is a free (open source) Python package for numerical calculations on
         tight-binding models with a strong focus on quantum transport. It is designed to
```

### Comparing `kwant-1.4.3/kwant.egg-info/SOURCES.txt` & `kwant-1.4.4/kwant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/kwant_red.jscm` & `kwant-1.4.4/kwant_red.jscm`

 * *Files identical despite different names*

### Comparing `kwant-1.4.3/setup.py` & `kwant-1.4.4/setup.py`

 * *Files identical despite different names*

