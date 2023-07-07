# Comparing `tmp/ltsfit-5.0.20.tar.gz` & `tmp/ltsfit-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ltsfit-5.0.20.tar", last modified: Mon Oct  3 16:57:26 2022, max compression
+gzip compressed data, was "ltsfit-6.0.0.tar", last modified: Fri Jul  7 17:13:06 2023, max compression
```

## Comparing `ltsfit-5.0.20.tar` & `ltsfit-6.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2022-10-03 16:57:26.677032 ltsfit-5.0.20/
--rw-rw-rw-   0        0        0    12885 2022-10-03 16:57:26.675984 ltsfit-5.0.20/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-10-03 16:57:26.636550 ltsfit-5.0.20/ltsfit/
--rw-rw-rw-   0        0        0     3215 2022-10-03 16:26:15.000000 ltsfit-5.0.20/ltsfit/CHANGELOG.rst
--rw-rw-rw-   0        0        0      442 2022-10-03 15:42:50.000000 ltsfit-5.0.20/ltsfit/LICENSE.txt
--rw-rw-rw-   0        0        0     2654 2022-10-03 16:55:01.000000 ltsfit-5.0.20/ltsfit/README.rst
--rw-rw-rw-   0        0        0       24 2022-10-03 16:57:15.000000 ltsfit-5.0.20/ltsfit/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-03 16:57:26.673720 ltsfit-5.0.20/ltsfit/examples/
--rw-rw-rw-   0        0        0       36 2018-04-16 16:12:03.000000 ltsfit-5.0.20/ltsfit/examples/__init__.py
--rw-rw-rw-   0        0        0     2543 2020-02-17 19:17:41.000000 ltsfit-5.0.20/ltsfit/examples/lts_fits_python_reference_output.txt
--rw-rw-rw-   0        0        0     1980 2022-09-20 10:15:55.000000 ltsfit-5.0.20/ltsfit/examples/lts_linefit_example.py
--rw-rw-rw-   0        0        0     2131 2022-05-20 17:12:50.000000 ltsfit-5.0.20/ltsfit/examples/lts_planefit_example.py
--rw-rw-rw-   0        0        0    14472 2022-10-03 16:55:01.000000 ltsfit-5.0.20/ltsfit/lts_linefit.py
--rw-rw-rw-   0        0        0    17481 2022-10-03 16:55:01.000000 ltsfit-5.0.20/ltsfit/lts_planefit.py
-drwxrwxrwx   0        0        0        0 2022-10-03 16:57:26.664207 ltsfit-5.0.20/ltsfit.egg-info/
--rw-rw-rw-   0        0        0    12885 2022-10-03 16:57:26.000000 ltsfit-5.0.20/ltsfit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2022-10-03 16:57:26.000000 ltsfit-5.0.20/ltsfit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-03 16:57:26.000000 ltsfit-5.0.20/ltsfit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2022-10-03 16:57:26.000000 ltsfit-5.0.20/ltsfit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-10-03 16:57:26.000000 ltsfit-5.0.20/ltsfit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2022-10-03 16:57:26.000000 ltsfit-5.0.20/ltsfit.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2022-10-03 16:57:26.678455 ltsfit-5.0.20/setup.cfg
--rw-rw-rw-   0        0        0     1723 2022-10-03 16:48:21.000000 ltsfit-5.0.20/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 17:13:06.696685 ltsfit-6.0.0/
+-rw-rw-rw-   0        0        0    12301 2023-07-07 17:13:06.693165 ltsfit-6.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-07 17:13:06.668007 ltsfit-6.0.0/ltsfit/
+-rw-rw-rw-   0        0        0     3772 2023-07-07 15:55:48.000000 ltsfit-6.0.0/ltsfit/CHANGELOG.rst
+-rw-rw-rw-   0        0        0      398 2023-07-07 13:04:21.000000 ltsfit-6.0.0/ltsfit/LICENSE.txt
+-rw-rw-rw-   0        0        0     2751 2023-07-07 13:18:09.000000 ltsfit-6.0.0/ltsfit/README.rst
+-rw-rw-rw-   0        0        0       23 2023-07-07 17:11:17.000000 ltsfit-6.0.0/ltsfit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 17:13:06.688147 ltsfit-6.0.0/ltsfit/examples/
+-rw-rw-rw-   0        0        0       36 2018-04-16 16:12:03.000000 ltsfit-6.0.0/ltsfit/examples/__init__.py
+-rw-rw-rw-   0        0        0     5960 2023-07-07 15:41:49.000000 ltsfit-6.0.0/ltsfit/examples/ltsfit_examples.py
+-rw-rw-rw-   0        0        0     3903 2023-07-07 15:40:28.000000 ltsfit-6.0.0/ltsfit/examples/ltsfit_python_reference_output.txt
+-rw-rw-rw-   0        0        0    20516 2023-07-07 17:10:34.000000 ltsfit-6.0.0/ltsfit/lts_hyperfit.py
+-rw-rw-rw-   0        0        0      692 2023-07-07 15:59:09.000000 ltsfit-6.0.0/ltsfit/lts_linefit.py
+-rw-rw-rw-   0        0        0      813 2023-07-07 15:59:09.000000 ltsfit-6.0.0/ltsfit/lts_planefit.py
+drwxrwxrwx   0        0        0        0 2023-07-07 17:13:06.688147 ltsfit-6.0.0/ltsfit.egg-info/
+-rw-rw-rw-   0        0        0    12301 2023-07-07 17:13:06.000000 ltsfit-6.0.0/ltsfit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      441 2023-07-07 17:13:06.000000 ltsfit-6.0.0/ltsfit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 17:13:06.000000 ltsfit-6.0.0/ltsfit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-07-07 17:13:06.000000 ltsfit-6.0.0/ltsfit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-07 17:13:06.000000 ltsfit-6.0.0/ltsfit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-07-07 17:13:06.000000 ltsfit-6.0.0/ltsfit.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-07-07 17:13:06.698211 ltsfit-6.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1658 2023-07-07 14:54:02.000000 ltsfit-6.0.0/setup.py
```

### Comparing `ltsfit-5.0.20/PKG-INFO` & `ltsfit-6.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ltsfit
-Version: 5.0.20
+Version: 6.0.0
 Summary: LtsFit: Least Trimmed Squares Fitting
 Home-page: https://purl.org/cappellari/software
 Author: Michele Cappellari
 Author-email: michele.cappellari@physics.ox.ac.uk
 License: Other/Proprietary License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -12,38 +12,38 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
 
 The LtsFit Package
 ==================
 
-**Robust Linear Regression with Scatter in One or Two Dimensions**
+**Robust Least Squares Regression with Uncertainties and Scatter in Any Dimension**
 
 .. image:: https://img.shields.io/pypi/v/ltsfit.svg
     :target: https://pypi.org/project/ltsfit/
 .. image:: https://img.shields.io/badge/arXiv-1208.3522-orange.svg
     :target: https://arxiv.org/abs/1208.3522
 .. image:: https://img.shields.io/badge/DOI-10.1093/mnras/stt562-green.svg
     :target: https://doi.org/10.1093/mnras/stt562
 
-LtsFit is a Python implementation of the method described in Section 3.2 of
+LtsFit is a Python package for **very robust** hyperplane fitting in N dimensions,
+with uncertainties in all coordinates and intrinsic scatter. It implements the
+method described in Section 3.2 of
 `Cappellari et al. (2013a) <https://ui.adsabs.harvard.edu/abs/2013MNRAS.432.1709C>`_
-to perform **very robust** fits of lines or planes to data with errors in all
-coordinates, while allowing for possible intrinsic scatter.
-Outliers are iteratively clipped using the robust Least Trimmed Squares (LTS)
-technique by `Rousseeuw & van Driessen (2006) <http://doi.org/10.1007/s10618-005-0024-4>`_.
+and uses the Least Trimmed Squares (LTS) technique to iteratively clip outliers
+`(Rousseeuw & van Driessen 2006) <http://doi.org/10.1007/s10618-005-0024-4>`_.
 
 .. contents:: :depth: 2
 
 Attribution
 -----------
 
-If you use this software for your research, please also cite
-`Cappellari et al. (2013a) <https://ui.adsabs.harvard.edu/abs/2013MNRAS.432.1709C>`_
-where the implementation was described. The BibTeX entry for the paper is::
+Please also cite `Cappellari et al. (2013a) <https://ui.adsabs.harvard.edu/abs/2013MNRAS.432.1709C>`_
+if you use this software for your research. This is the paper where the
+implementation was described. The BibTeX entry for the paper is::
 
     @ARTICLE{Cappellari2013a,
         author = {{Cappellari}, M. and {Scott}, N. and {Alatalo}, K. and
             {Blitz}, L. and {Bois}, M. and {Bournaud}, F. and {Bureau}, M. and
             {Crocker}, A.~F. and {Davies}, R.~L. and {Davis}, T.~A. and {de Zeeuw},
             P.~T. and {Duc}, P.-A. and {Emsellem}, E. and {Khochfar}, S. and
             {Krajnovi{\'c}}, D. and {Kuntschner}, H. and {McDermid}, R.~M. and
@@ -67,241 +67,185 @@
 
     pip install ltsfit
 
 Without writing access to the global ``site-packages`` directory, use::
 
     pip install --user ltsfit
 
+To upgrade the package to the latest version use::
+
+    pip install --upgrade ltsfit
+
 Documentation
 -------------
 
 See ``ltsfit/examples`` and the files docstrings.
 They are copied by ``pip`` within the global folder
 `site-packages <https://stackoverflow.com/a/46071447>`_.
 
 ###########################################################################
 
-lts_linefit
-===========
+lts_hyperfit
+============ 
 
 Purpose
 -------
 
-Best straight-line *robust* fit to data with errors in
-both coordinates while fitting for the intrinsic scatter.
-See `Cappellari et al. (2013a, Sec.3.2)
-<https://ui.adsabs.harvard.edu/abs/2013MNRAS.432.1709C>`_
+Fit a linear function of the form::
 
-Explanation
------------
+    z = a + b1*x1 + b2*x2 +...+ bm*xm,
 
-Linear Least-squares approximation in one-dimension (y = a + b*x),
-when both x and y data have errors and allowing for intrinsic
-scatter in the relation.
-
-Outliers are iteratively clipped using the extremely robust
-FAST-LTS technique by
-`Rousseeuw & van Driessen (2006) <http://doi.org/10.1007/s10618-005-0024-4>`_
-See also `Rousseeuw (1987) <http://books.google.co.uk/books?id=woaH_73s-MwC&pg=PA15>`_
+to data with errors in all coordinates and intrinsic scatter, using a robust
+method that clips outliers. The function can handle lines in 2-dim, planes in
+3-dim, or hyperplanes in N-dim, where ``x1, x2,..., xm`` are the independent
+variables and ``z`` is the dependent variable. The method was introduced in
+Sec. 3.2 of `Cappellari et al. (2013a) <https://ui.adsabs.harvard.edu/abs/2013MNRAS.432.1709C>`_
+and the treatment of outliers is is based on the FAST-LTS technique by
+`Rousseeuw & van Driessen (2006) <http://doi.org/10.1007/s10618-005-0024-4>`_.
+See also `Rousseeuw (1987) <http://books.google.co.uk/books?id=woaH_73s-MwC&pg=PA15>`_.
 
 Calling Sequence
 ----------------
 
 .. code-block:: python
 
-    p = lts_linefit(x, y, sigx, sigy, clip=2.6, epsy=True, corr=True,
-                  frac=None, pivot=None, plot=True, text=True)
-
-The output values are stored as attributes of "p".
-See usage example at the bottom of this file.
-
-Input Parameters
-----------------
-
-x, y:
-    vectors of size N with the measured values.
-sigx, sigy:
-    vectors of size N with the 1sigma errors in x and y.
-clip:
-    values deviating more than clip*sigma from the best fit are
-    considered outliers and are excluded from the linear fit.
-epsy:
-    if True, the intrinsic scatter is printed on the plot.
-corr:
-    if True, the correlation coefficients are printed on the plot.
-frac:
-    fractions of values to include in the LTS stage.
-    Up to a fraction "frac" of the values can be outliers.
-    One must have 0.5 < frac < 1  (default frac=0.5).
-
-    NOTE: Set frac=1, to turn off outliers detection.
-label:
-    optional string label to create a legend outside the procedure.
-pivot:
-    if this is not None, then lts_linefit fits the relation::
-
-        y = a + b*(x - pivot)
-
-    pivot is called x_0 in eq.(6) of Cappellari et al. (2013)
-    Use of this keyword is *strongly* recommended and a suggested
-    value is pivot ~ np.mean(x). This keyword is important to
-    reduce the covariance between a and b.
-plot:
-    if True a plot of the fit is produced.
-text:
-    if True, the best fitting parameters are printed on the plot.
-
-Output Parameters
------------------
-
-The output values are stored as attributed of the lts_linefit class.
-
-p.ab:
-    best fitting parameters [a, b]
-p.ab_err:
-    1*sigma formal errors [a_err, b_err] on a and b.
-p.mask:
-    boolean vector with the same size of x and y.
-    It contains True  for the elements of (x, y) which were included in
-    the fit and False for the outliers which were automatically clipped.
-p.rms:
-    rms = np.std(fit - y) beteween the data and the fitted relation.
-p.sig_int:
-    intrinsic scatter around the linear relation.
-    sig_int is called epsilon_y in eq.(6) of Cappellari et al. (2013).
-p.sig_int_err:
-    1*sigma formal error on sig_int.
-
-###########################################################################
-
+    from ltsfit.lts_hyperfit import lts_hyperfit
 
-lts_planefit
-============
+    p = lts_hyperfit(x, z, sigx, sigz, clip=2.6, corr=True, epsz=True,
+             frac=None, label='Fitted', label_clip='Clipped', pivot=0,
+             plot=True, text=True)
 
-Purpose
--------
-
-Best plane *robust* fit to data with errors in all
-three coordinates and fitting for the intrinsic scatter.
-See `Cappellari et al. (2013a, Sec.3.2)
-<https://ui.adsabs.harvard.edu/abs/2013MNRAS.432.1709C>`_
-
-Explanation
------------
+The output values are stored as attributes of the ``p`` object.
 
-Linear Least-squares approximation in two-dimension (z = a + b*x + c*y),
-when x, y and z data have errors, and allowing for intrinsic
-scatter in the relation.
-
-Outliers are iteratively clipped using the extremely robust
-FAST-LTS technique by
-`Rousseeuw & van Driessen (2006) <http://doi.org/10.1007/s10618-005-0024-4>`_
-See also `Rousseeuw (1987) <http://books.google.co.uk/books?id=woaH_73s-MwC&pg=PA15>`_
-
-Calling Sequence
+Input Parameters
 ----------------
 
-.. code-block:: python
-
-    p = lts_planefit(x, y, z, sigx, sigy, sigz, clip=2.6, epsz=True,
-                    frac=None, pivotx=None, pivoty=None, plot=True, text=True)
+x: array_like with shape (n, m)
+    Array of ``n`` independent variables for ``m`` dimensions.
 
-The output values are stored as attributes of "p".
-See usage example at the bottom of this file.
+    EXAMPLE: To fit a line in 2-dim, one has a single vector ``xx`` of
+    length ``n`` with the independent variable and a corresponding vector of
+    dependent variable ``yy``. In this case, ``x = xx`` and ``z = yy``.
+
+    EXAMPLE: To fit a plane in 3-dim, one has two vectors of length ``n`` of
+    independent variables ``(xx, yy)``. In this case, ``x = np.column_stack([xx, yy])``.
+
+    EXAMPLE: To fit a hyperplane in 4-dim, one has three vectors of independent
+    variables ``(x1, x2, x3)``. In this case, ``x = np.column_stack([x1, x2, x3])``.
+z: array_like with shape (n,)
+    Vector of ``n`` measured values for each set of ``x`` variables.
+sigx: array_like with shape (n, m)
+    Array of ``n`` values of ``1sigma`` uncertainties for each ``x`` 
+    coordinate for ``m`` dimensions. This has the same shape as ``x``.
+sigz: array_like with shape (n,)
+    Vector of ``n`` values of ``1sigma`` uncertainties for each ``z`` value.
 
-Input Parameters
-----------------
+Optional Keywords
+-----------------
 
-x, y, z:
-    vectors of size N with the measured values.
-sigx, sigy, sigz:
-    vectors of size N with the 1sigma errors in x , y and z.
-clip:
-    values deviating more than clip*sigma from the best fit are
-    considered outliers and are excluded from the plane fit.
-epsz:
-    if True, the intrinsic scatter is printed on the plot.
-frac:
-    fractions of values to include in the LTS stage.
-    Up to a fraction "frac" of the values can be outliers.
-    One must have 0.5 <= frac <= 1  (default frac=0.5).
-
-    NOTE: Set frac=1, to turn off outliers detection.
-pivotx, pivoty:
-    if these are not None, then lts_planefit fits the plane::
-
-        z = a + b*(x - pivotx) + c*(y - pivoty)
-
-    pivotx, pivoty are called x_0, y_0 in eq.(7) of Cappellari et al. (2013)
-    Use of these keywords is *strongly* recommended, and suggested
-    values are ``pivotx=np.median(x), pivoty=np.median(y)``.
-    This keyword is important to reduce the covariance between a, b and c.
-plot:
-    if True a plot of the fit is produced.
-text:
-    if True, the best fitting parameters are printed on the plot.
+clip: float
+    Clipping threshold in ``sigma`` units. Values deviating more than
+    ``clip*sigma`` from the best fit are considered outliers and are
+    excluded from the fit. Default is ``2.6``, which would include 99% of
+    the values for a Gaussian distribution.
+corr:
+    if ``True``, the correlation coefficients are printed on the plot.
+epsz: bool
+    If ``True``, the intrinsic scatter is printed on the output plot.
+    Default is ``True``.
+frac: float
+    Fraction of values to include in the LTS stage.
+    Up to a fraction ``frac`` of the values can be outliers.
+    One must have ``0.5 <= frac <= 1``. Default is ``0.5``.
+
+    NOTE: Set ``frac=1`` to turn off outliers detection.
+pivot: array_like with shape (m,)
+    If nonzero, then ``lts_hyperfit`` fits the hyperplane::
+
+        z = a + b0*(x0 - pivot[0]) + b1*(x1 - pivot[1]) + ... + bm*(xm - pivot[m])
+
+    ``pivot`` are called ``x_0``, ``y_0`` in eq.(7) of `Cappellari et al. (2013a)`_.
+    Use of this parameter is strongly recommended, and suggested
+    values are ``pivot = np.median(x, 0)``. The fitted parameters are not
+    strongly dependent on the precise value of this parameter. For this
+    reason it is generally better to round the pivot values to nice numbers.
+    This parameter is important to reduce the covariance between the
+    coefficients. Default is ``0``.
+plot: bool
+    If ``True``, a plot of the fit is produced. Default is ``True``.
+text: bool
+    If ``True``, the best fitting parameters are printed on the plot.
+    Default is ``True``.
 
 Output Parameters
 -----------------
 
-The output values are stored as attributed of the lts_linefit class.
+The output values are stored as attributes of the ``lts_hyperfit`` class.
 
-p.abc:
-    best fitting parameters [a, b, c]
-p.abc_err:
-    1*sigma formal errors [a_err, b_err, c_err] on a, b and c.
-p.mask:
-    boolean vector with the same size of x, y and z.
-    It contains True for the elements of (x, y, z) which were included in
-    the fit and False for the outliers which were automatically clipped.
-p.rms:
-    rms = np.std(fit - z) beteween the data and the fitted relation.
-p.sig_int:
-    intrinsic scatter in the z direction around the plane.
-    sig_int is called epsilon_z in eq.(7) of Cappellari et al. (2013).
-p.sig_int_err:
-    1*sigma formal error on sig_int.
+p.abc: array_like with shape (m+1,)
+    Best fitting parameters ``[a, b1, b2,..., bm]``.
+p.abc_err: array_like with shape (m+1,)
+    ``1*sigma`` formal errors ``[a_err, b1_err, b2_err,..., bm_err]`` on
+    ``[a, b1, b2,..., bm]``.
+p.mask: array_like with shape (n,) and dtype bool
+    Boolean vector indicating which elements of ``z`` were included in
+    the fit (``True``) and which were clipped as outliers (``False``).
+p.rms: float
+    RMS deviation between the data and the fitted relation.
+p.sig_int: float
+    Intrinsic scatter in the ``z`` direction around the hyperplane.
+    ``sig_int`` is called ``epsilon_z`` in eq.(7) of `Cappellari et al. (2013a)`_.
+p.sig_int_err: float
+    ``1*sigma`` formal error on ``sig_int``.
 
 ###########################################################################
 
 
 
 License
 =======
 
 Other/Proprietary License
 
-Copyright (c) 2012-2022 Michele Cappellari
+Copyright (c) 2012-2023 Michele Cappellari
 
-This software is provided as is without any warranty whatsoever.
-Permission to use, for non-commercial purposes is granted.
-Permission to modify for personal or internal use is granted,
-provided this copyright and disclaimer are included in all 
-copies of the software. All other rights are reserved.
-In particular, redistribution of the code is not allowed.
+This software is provided as is with no warranty. You may use it for
+non-commercial purposes and modify it for personal or internal use, as long
+as you include this copyright and disclaimer in all copies. You may not
+redistribute the code.
+
+###########################################################################
 
 Changelog
 =========
 
-V2.0.20: MC, Oxford, 3 October 2022
+V6.0.0: MC, Oxford, 7 July 2023
+  - Added ``lts_hyperfit`` to fit hyperplanes in N-dim. This procedure
+    generalizes and replaces both ``lts_linefit`` and ``lts_planefit``, which
+    are now deprecated wrappers for ``lts_hyperfit``. This change was suggested
+    and motivated by Francesco D'Eugenio (cam.ac.uk), who shared his own 4-dim
+    ``lts_hyperfit`` and his paper on a useful application.
+  - Fixed inconsistency between the version number on PyPi and in the Changelog.
+
+V5.0.20: MC, Oxford, 3 October 2022
   - Fixed program stop due to Matplotlib change.
     Thanks to Hitesh Lala (Heidelberg) for the report.
   - Extract documentation from docstrings and show it on PyPi.
 
-V2.0.19: MC, Oxford, 22 January 2021
+V5.0.19: MC, Oxford, 22 January 2021
   - Fixed incorrect plot ranges due to a Matplotlib change.
     Thanks to Davide Bevacqua (unibo.it) for the report.
 
-V2.0.18: MC, Oxford, 17 February 2020
+V5.0.18: MC, Oxford, 17 February 2020
   - Properly print significant trailing zeros in results.
 
-V2.0.17: MC, Oxford, 22 January 2020
+V5.0.17: MC, Oxford, 22 January 2020
   - Formatted documentation as docstring.
   - Included p.rms output.
-
+  - Published on PyPi. Increased major version number by mistake.
 
 V2.0.16: MC, Oxford, 27 September 2018
   - Fixed clock DeprecationWarning in Python 3.7.
 
 V2.0.15: MC, Oxford, 12 May 2018
   - Dropped Python 2.7 support.
```

### Comparing `ltsfit-5.0.20/ltsfit/README.rst` & `ltsfit-6.0.0/ltsfit/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 The LtsFit Package
 ==================
 
-**Robust Linear Regression with Scatter in One or Two Dimensions**
+**Robust Least Squares Regression with Uncertainties and Scatter in Any Dimension**
 
 .. image:: https://img.shields.io/pypi/v/ltsfit.svg
     :target: https://pypi.org/project/ltsfit/
 .. image:: https://img.shields.io/badge/arXiv-1208.3522-orange.svg
     :target: https://arxiv.org/abs/1208.3522
 .. image:: https://img.shields.io/badge/DOI-10.1093/mnras/stt562-green.svg
     :target: https://doi.org/10.1093/mnras/stt562
 
-LtsFit is a Python implementation of the method described in Section 3.2 of
+LtsFit is a Python package for **very robust** hyperplane fitting in N dimensions,
+with uncertainties in all coordinates and intrinsic scatter. It implements the
+method described in Section 3.2 of
 `Cappellari et al. (2013a) <https://ui.adsabs.harvard.edu/abs/2013MNRAS.432.1709C>`_
-to perform **very robust** fits of lines or planes to data with errors in all
-coordinates, while allowing for possible intrinsic scatter.
-Outliers are iteratively clipped using the robust Least Trimmed Squares (LTS)
-technique by `Rousseeuw & van Driessen (2006) <http://doi.org/10.1007/s10618-005-0024-4>`_.
+and uses the Least Trimmed Squares (LTS) technique to iteratively clip outliers
+`(Rousseeuw & van Driessen 2006) <http://doi.org/10.1007/s10618-005-0024-4>`_.
 
 .. contents:: :depth: 2
 
 Attribution
 -----------
 
-If you use this software for your research, please also cite
-`Cappellari et al. (2013a) <https://ui.adsabs.harvard.edu/abs/2013MNRAS.432.1709C>`_
-where the implementation was described. The BibTeX entry for the paper is::
+Please also cite `Cappellari et al. (2013a) <https://ui.adsabs.harvard.edu/abs/2013MNRAS.432.1709C>`_
+if you use this software for your research. This is the paper where the
+implementation was described. The BibTeX entry for the paper is::
 
     @ARTICLE{Cappellari2013a,
         author = {{Cappellari}, M. and {Scott}, N. and {Alatalo}, K. and
             {Blitz}, L. and {Bois}, M. and {Bournaud}, F. and {Bureau}, M. and
             {Crocker}, A.~F. and {Davies}, R.~L. and {Davis}, T.~A. and {de Zeeuw},
             P.~T. and {Duc}, P.-A. and {Emsellem}, E. and {Khochfar}, S. and
             {Krajnovi{\'c}}, D. and {Kuntschner}, H. and {McDermid}, R.~M. and
@@ -52,14 +52,18 @@
 
     pip install ltsfit
 
 Without writing access to the global ``site-packages`` directory, use::
 
     pip install --user ltsfit
 
+To upgrade the package to the latest version use::
+
+    pip install --upgrade ltsfit
+
 Documentation
 -------------
 
 See ``ltsfit/examples`` and the files docstrings.
 They are copied by ``pip`` within the global folder
 `site-packages <https://stackoverflow.com/a/46071447>`_.
```

### Comparing `ltsfit-5.0.20/ltsfit/examples/lts_fits_python_reference_output.txt` & `ltsfit-6.0.0/ltsfit/examples/ltsfit_python_reference_output.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-# lts_linefit_example() and lts_planefit_example() reference 
-# output for the LtsFit package version 5.0.18.
-# Generated under Python 3.7 using NumPy 1.18, SciPy 1.3, Matplotlib 3.1
+# ltsfit_examples reference output for the LtsFit package version 6.0.0 (7 July 2023)
+# Generated under Python 3.11 using NumPy 1.24, SciPy 1.10, Matplotlib 3.7
 #
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
-Running lts_linefit_example.py
+runfile('ltsfit_examples.py')
+
+----------------------------------------------------------------------
+Running lts_linefit_example
 
 sig_int:     0.0000      2.5670
 Computing sig_int
 sig_int:     0.0000      2.5670
 sig_int:     0.4473     -0.3742
 sig_int:     0.3904     -0.2211
 sig_int:     0.3147      0.0725
@@ -21,28 +23,28 @@
 sig_int:     0.3612     -0.0243
 sig_int:     0.3552     -0.0016
 sig_int:     0.3547      0.0000
 sig_int:     0.3549     -0.0007
 Repeat at best fitting solution
 sig_int:     0.3306      0.0002
 ################# Values and formal errors ################
- intercept:  20.235 +/- 0.029
-     slope:  0.500 +/- 0.031
-   scatter:  0.331 +/- 0.024
-Observed rms scatter: 0.39 
-y = a + b*(x - pivot) with pivot = 20.4
+        a =  20.235 +/- 0.029
+      b_0 =  0.500 +/- 0.031
+  scatter =  0.331 +/- 0.024
+Observed rms scatter: 0.39
+z = a + (x_0 - p_0) b_0
+   p_0 = 20.40
 Spearman r=0.65 and p=5.3e-37
-Pearson r=0.5 and p=9.1e-21
+Pearson r=0.50 and p=9.1e-21
 ##########################################################
-seconds 10.75
-The best fitting parameters are: [ 20.23536506   0.49999518]
-
-+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
+seconds 10.56
+The best fitting parameters are: [20.23536506  0.49999517]
 
-Running lts_planefit_example.py
+----------------------------------------------------------------------
+Running lts_planefit_example
 
 sig_int:     0.0000      2.3049
 Computing sig_int
 sig_int:     0.0000      2.3049
 sig_int:     1.5083     -0.4527
 sig_int:     1.2607     -0.2690
 sig_int:     0.9359      0.1216
@@ -56,19 +58,60 @@
 sig_int:     1.1303     -0.0347
 sig_int:     1.1023     -0.0024
 sig_int:     1.1002      0.0000
 sig_int:     1.1007     -0.0006
 Repeat at best fitting solution
 sig_int:     1.0191      0.0000
 ################# Values and formal errors ################
- intercept:  60.743 +/- 0.090
-    slopeX:  1.959 +/- 0.061
-    slopeY:  0.958 +/- 0.027
-   scatter:  1.019 +/- 0.081
+        a =  60.743 +/- 0.090
+      b_0 =  1.959 +/- 0.061
+      b_1 =  0.958 +/- 0.027
+  scatter =  1.019 +/- 0.081
 Observed rms scatter: 1.2
-z = a + b*(x - pivotx) + c*(y - pivoty)
-with pivotx = 19.55 & pivoty = 11.74
+z = a + (x_0 - p_0) b_0 + (x_1 - p_1) b_1
+   p_0 = 19.55
+   p_1 = 11.74
 ##########################################################
-seconds 14.33
-The best fitting parameters are: [ 60.74285125   1.9590924    0.95786781]
+seconds 10.90
+The best fitting parameters are: [60.74285125  1.95909241  0.95786782]
 
-+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
+----------------------------------------------------------------------
+Running lts_hyperfit_example
+
+sig_int:     0.0000      0.7861
+Computing sig_int
+sig_int:     0.0000      0.7861
+sig_int:     2.1853     -0.5375
+sig_int:     1.2979     -0.1013
+sig_int:     1.1153      0.1087
+sig_int:     1.2098      0.0315
+sig_int:     1.2307      0.0151
+sig_int:     1.2474      0.0021
+sig_int:     1.2498      0.0002
+sig_int:     1.2505     -0.0003
+Computing sig_int error
+sig_int:     1.2498      0.0377
+sig_int:     2.1853     -0.4327
+sig_int:     1.3248     -0.0151
+sig_int:     1.3033      0.0636
+sig_int:     1.3207     -0.0123
+sig_int:     1.3120      0.0572
+sig_int:     1.3191      0.0519
+sig_int:     1.3200     -0.0118
+Repeat at best fitting solution
+sig_int:     1.2498     -0.0671
+################# Values and formal errors ################
+        a =  84.31 +/- 0.16
+      b_0 =  2.049 +/- 0.085
+      b_1 =  0.786 +/- 0.045
+      b_2 =  2.89 +/- 0.10
+  scatter =  1.250 +/- 0.070
+Observed rms scatter: 1.7
+z = a + (x_0 - p_0) b_0 + (x_1 - p_1) b_1 + (x_2 - p_2) b_2
+   p_0 = 19.80
+   p_1 = 11.67
+   p_2 = 7.787
+##########################################################
+seconds 20.41
+The best fitting parameters are: [84.30589223  2.04931942  0.78569159  2.88565599]
+
+----------------------------------------------------------------------
```

### Comparing `ltsfit-5.0.20/ltsfit/lts_planefit.py` & `ltsfit-6.0.0/ltsfit/lts_hyperfit.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # ###############################################################################
 #
-# Copyright (C) 2012-2021, Michele Cappellari
+# Copyright (C) 2012-2023, Michele Cappellari
 # E-mail: michele.cappellari_at_physics.ox.ac.uk
 #
 # Updated versions of the software are available from my web page
 # http://purl.org/cappellari/software
 #
 # If you have found this software useful for your research, I would
-# appreciate an acknowledgement to the use of the "LTS_PLANEFIT program
+# appreciate an acknowledgement to the use of the "LtsFit package
 # described in Cappellari et al. (2013, MNRAS, 432, 1709), which
 # combines the Least Trimmed Squares robust technique of Rousseeuw &
 # van Driessen (2006) into a least-squares fitting algorithm which
 # allows for errors in all variables and intrinsic scatter."
 #
 # This software is provided as is without any warranty whatsoever.
 # Permission to use, for non-commercial purposes is granted.
@@ -35,15 +35,15 @@
 #           MC, Baltimore, 8 June 2014
 #       V2.0.5: Text plotting changes. MC, Oxford, 26 June 2014
 #       V3.0.0: Converted from IDL into Python. MC, Oxford, 5 November 2014
 #       V3.0.1: Updated documentation. MC, Baltimore, 9 June 2015
 #       V3.0.2: Fixed potential program stop without outliers.
 #           Thanks to Masato Onodera for a clear report of the problem.
 #         - Output boolean mask instead of good/bad indices.
-#         - Removed lts_planefit_example from this file.
+#         - Removed lts_hyperfit_example from this file.
 #           MC, Oxford, 6 July 2015
 #       V3.0.3: Fixed potential program stop without outliers.
 #           MC, Oxford, 1 October 2015
 #       V3.0.4: Fixed potential program stop without outliers in Matplotlib 1.5.
 #           MC, Oxford, 9 December 2015
 #       V3.0.5: Use LimeGreen for outliers. MC, Oxford, 8 January 2016
 #       V3.0.6: Check for non finite values in input.
@@ -71,367 +71,428 @@
 #       Vx.x.x: Additional changes are documented in the CHANGELOG of the LtsFit package.
 #
 #------------------------------------------------------------------------------
 
 from time import perf_counter as clock
 import numpy as np
 import matplotlib.pyplot as plt
-from scipy import optimize
+from scipy import optimize, stats
 
 #----------------------------------------------------------------------------
 
-def _planefit(x, y, z, sigz=None, weights=None):
+def _hyperfit(x, z, sigz=None, weights=None):
     """
-    Fit a plane z = a + b*x + c*y to a set of points (x, y, z)
+    Fit a hyperplane zfit = a + b1*x1 + b2*x2 + ...
+    to a set of points (x1, x2,... , z)
     by minimizing chi2 = np.sum(((z - zfit)/sigz)**2)
 
     """
-    v1 = np.ones_like(x)
+    v1 = np.ones_like(z)
     if weights is None:
         if sigz is None:
             sw = v1
         else:
             sw = v1/sigz
     else:
         sw = np.sqrt(weights)
 
-    a = np.column_stack([v1, x, y])
+    a = np.column_stack([v1, x])
     abc = np.linalg.lstsq(a*sw[:, None], z*sw, rcond=None)[0]
 
     return abc
 
 #----------------------------------------------------------------------------
 
 def _display_errors(par, sig_par, epsz):
-    """
-    Print parameters rounded according to their errors
+    """ Print parameters rounded according to their uncertainties """
 
-    """
     prec = np.zeros_like(par)
     w = (sig_par != 0) & (par != 0)
     prec[w] = np.ceil(np.log10(np.abs(par[w]))) - np.floor(np.log10(sig_par[w])) + 1
     prec = prec.clip(0)  # negative precisions not allowed
     dg = list(map(str, prec.astype(int)))
 
-    # print on the terminal and save as string
+    # print on the terminal and save as LaTeX string
 
-    txt = ['intercept: ', 'slopeX: ', 'slopeY: ', 'scatter: ']
-    for t, d, p, s in zip(txt, dg, par, sig_par):
-        print(f"{t:>{12}} {p:#.{d}g} +/- {s:#.2g}")
+    txt = ['a = '] + [f'b_{j} = ' for j in range(len(par) - 2)]
+    txt1 = txt + ['scatter = ']
+    for t, d, p, s in zip(txt1, dg, par, sig_par):
+        print(f"{t:>12} {p:#.{d}g} +/- {s:#.2g}")
 
-    txt = ['a=', 'b=', 'c=', '\\varepsilon_z=']
-    if not epsz:
-        txt = txt[:-1]
+    if epsz:
+        txt += ['\\varepsilon_z=']
     string = ''
     for t, d, p, s in zip(txt, dg, par, sig_par):
         string += f"${t} {p:#.{d}g} \\pm {s:#.2g}$\n"
 
     return string
 
 #------------------------------------------------------------------------------
 
-def _residuals(abc, x, y, z, sigx, sigy, sigz):
-    """
-    See equation (7) of Cappellari et al. (2013, MNRAS, 432, 1709)
+def _residuals(abc, x, z, sigx, sigz):
+    """ See equation (7) of Cappellari et al. (2013, MNRAS, 432, 1709) """
 
-    """
-    res = (abc[0] + abc[1]*x + abc[2]*y - z) \
-        / np.sqrt((abc[1]*sigx)**2 + (abc[2]*sigy)**2 + sigz**2)
+    res = (abc[0] + x @ abc[1:] - z)/np.sqrt(sigx**2 @ abc[1:]**2 + sigz**2)
 
     return res
 
 #----------------------------------------------------------------------------
 
-def _fitting(x, y, z, sigx, sigy, sigz, abc):
+def _fitting(x, z, sigx, sigz, abc):
 
     abc, pcov, infodict, errmsg, success = optimize.leastsq(
-        _residuals, abc, args=(x, y, z, sigx, sigy, sigz), full_output=1)
+        _residuals, abc, args=(x, z, sigx, sigz), full_output=1)
 
     if pcov is None or np.any(np.diag(pcov) < 0):
-        sig_ABC = np.full(3, np.inf)
+        sig_abc = np.full(x.shape[1], np.inf)
         chi2 = np.inf
     else:
         chi2 = np.sum(infodict['fvec']**2)
-        sig_ABC = np.sqrt(np.diag(pcov))  # ignore covariance
+        sig_abc = np.sqrt(np.diag(pcov))  # ignore covariance
 
-    return abc, sig_ABC, chi2
+    return abc, sig_abc, chi2
 
 #----------------------------------------------------------------------------
 
-def _fast_algorithm(x, y, z, sigx, sigy, sigz, h):
+def _fast_algorithm(x, z, sigx, sigz, h):
 
     # Robust least trimmed squares regression.
     # Pg. 38 of Rousseeuw & van Driessen (2006)
     # http://dx.doi.org/10.1007/s10618-005-0024-4
     #
     m = 500 # Number of random starting points
-    abcv = np.empty((m, 3))
+    ndim = x.shape[1] + 1
+    abcv = np.empty((m, ndim))
     chi2v = np.empty(m)
     for j in range(m):  # Draw m random starting points
-        w = np.random.choice(x.size, 3, replace=False)
-        abc = _planefit(x[w], y[w], z[w])  # Find a plane going trough three random points
+        w = np.random.choice(z.size, ndim, replace=False)
+        abc = _hyperfit(x[w], z[w])  # Find a plane going trough three random points
         for k in range(3):  # Run C-steps up to H_3
-            res = _residuals(abc, x, y, z, sigx, sigy, sigz)
+            res = _residuals(abc, x, z, sigx, sigz)
             good = np.argsort(np.abs(res))[:h]  # Fit the h points with smallest errors
-            abc, sig_abc, chi_sq = _fitting(x[good], y[good], z[good], sigx[good], sigy[good], sigz[good], abc)
+            abc, sig_abc, chi_sq = _fitting(x[good], z[good], sigx[good], sigz[good], abc)
         abcv[j, :] = abc
         chi2v[j] = chi_sq
 
     # Perform full C-steps only for the 10 best results
     #
     w = np.argsort(chi2v)
     nbest = 10
     chi_sq = np.inf
     for j in range(nbest):
         abc1 = abcv[w[j], :]
         while True:  # Run C-steps to convergence
             abcOld = abc1
-            res = _residuals(abc1, x, y, z, sigx, sigy, sigz)
+            res = _residuals(abc1, x, z, sigx, sigz)
             good1 = np.argsort(np.abs(res))[:h]  # Fit the h points with smallest errors
-            abc1, sig_ab1, chi1_sq = _fitting(x[good1], y[good1], z[good1], sigx[good1], sigy[good1], sigz[good1], abc1)
+            abc1, sig_ab1, chi1_sq = _fitting(x[good1], z[good1], sigx[good1], sigz[good1], abc1)
             if np.allclose(abcOld, abc1):
                 break
         if chi_sq > chi1_sq:
             abc = abc1  # Save best solution
             good = good1
             chi_sq = chi1_sq
 
-    mask = np.zeros_like(x, dtype=bool)
+    mask = np.zeros_like(z, dtype=bool)
     mask[good] = True
 
     return abc, mask
 
 #------------------------------------------------------------------------------
 
-class lts_planefit:
+class lts_hyperfit:
     """
-    lts_planefit
-    ============
+    lts_hyperfit
+    ============ 
 
     Purpose
     -------
 
-    Best plane *robust* fit to data with errors in all
-    three coordinates and fitting for the intrinsic scatter.
-    See `Cappellari et al. (2013a, Sec.3.2)
-    <https://ui.adsabs.harvard.edu/abs/2013MNRAS.432.1709C>`_
-
-    Explanation
-    -----------
-
-    Linear Least-squares approximation in two-dimension (z = a + b*x + c*y),
-    when x, y and z data have errors, and allowing for intrinsic
-    scatter in the relation.
-
-    Outliers are iteratively clipped using the extremely robust
-    FAST-LTS technique by
-    `Rousseeuw & van Driessen (2006) <http://doi.org/10.1007/s10618-005-0024-4>`_
-    See also `Rousseeuw (1987) <http://books.google.co.uk/books?id=woaH_73s-MwC&pg=PA15>`_
+    Fit a linear function of the form::
 
+        z = a + b1*x1 + b2*x2 +...+ bm*xm,
+
+    to data with errors in all coordinates and intrinsic scatter, using a robust
+    method that clips outliers. The function can handle lines in 2-dim, planes in
+    3-dim, or hyperplanes in N-dim, where ``x1, x2,..., xm`` are the independent
+    variables and ``z`` is the dependent variable. The method was introduced in
+    Sec. 3.2 of `Cappellari et al. (2013a) <https://ui.adsabs.harvard.edu/abs/2013MNRAS.432.1709C>`_
+    and the treatment of outliers is is based on the FAST-LTS technique by
+    `Rousseeuw & van Driessen (2006) <http://doi.org/10.1007/s10618-005-0024-4>`_.
+    See also `Rousseeuw (1987) <http://books.google.co.uk/books?id=woaH_73s-MwC&pg=PA15>`_.
+    
     Calling Sequence
     ----------------
 
     .. code-block:: python
 
-        p = lts_planefit(x, y, z, sigx, sigy, sigz, clip=2.6, epsz=True,
-                        frac=None, pivotx=None, pivoty=None, plot=True, text=True)
+        from ltsfit.lts_hyperfit import lts_hyperfit
+
+        p = lts_hyperfit(x, z, sigx, sigz, clip=2.6, corr=True, epsz=True,
+                 frac=None, label='Fitted', label_clip='Clipped', pivot=0,
+                 plot=True, text=True)
 
-    The output values are stored as attributes of "p".
-    See usage example at the bottom of this file.
+    The output values are stored as attributes of the ``p`` object.
 
     Input Parameters
     ----------------
 
-    x, y, z:
-        vectors of size N with the measured values.
-    sigx, sigy, sigz:
-        vectors of size N with the 1sigma errors in x , y and z.
-    clip:
-        values deviating more than clip*sigma from the best fit are
-        considered outliers and are excluded from the plane fit.
-    epsz:
-        if True, the intrinsic scatter is printed on the plot.
-    frac:
-        fractions of values to include in the LTS stage.
-        Up to a fraction "frac" of the values can be outliers.
-        One must have 0.5 <= frac <= 1  (default frac=0.5).
-
-        NOTE: Set frac=1, to turn off outliers detection.
-    pivotx, pivoty:
-        if these are not None, then lts_planefit fits the plane::
-
-            z = a + b*(x - pivotx) + c*(y - pivoty)
-
-        pivotx, pivoty are called x_0, y_0 in eq.(7) of Cappellari et al. (2013)
-        Use of these keywords is *strongly* recommended, and suggested
-        values are ``pivotx=np.median(x), pivoty=np.median(y)``.
-        This keyword is important to reduce the covariance between a, b and c.
-    plot:
-        if True a plot of the fit is produced.
-    text:
-        if True, the best fitting parameters are printed on the plot.
+    x: array_like with shape (n, m)
+        Array of ``n`` independent variables for ``m`` dimensions.
+
+        EXAMPLE: To fit a line in 2-dim, one has a single vector ``xx`` of
+        length ``n`` with the independent variable and a corresponding vector of
+        dependent variable ``yy``. In this case, ``x = xx`` and ``z = yy``.
+
+        EXAMPLE: To fit a plane in 3-dim, one has two vectors of length ``n`` of
+        independent variables ``(xx, yy)``. In this case, ``x = np.column_stack([xx, yy])``.
+
+        EXAMPLE: To fit a hyperplane in 4-dim, one has three vectors of independent
+        variables ``(x1, x2, x3)``. In this case, ``x = np.column_stack([x1, x2, x3])``.
+    z: array_like with shape (n,)
+        Vector of ``n`` measured values for each set of ``x`` variables.
+    sigx: array_like with shape (n, m)
+        Array of ``n`` values of ``1sigma`` uncertainties for each ``x`` 
+        coordinate for ``m`` dimensions. This has the same shape as ``x``.
+    sigz: array_like with shape (n,)
+        Vector of ``n`` values of ``1sigma`` uncertainties for each ``z`` value.
+
+    Optional Keywords
+    -----------------
+
+    clip: float
+        Clipping threshold in ``sigma`` units. Values deviating more than
+        ``clip*sigma`` from the best fit are considered outliers and are
+        excluded from the fit. Default is ``2.6``, which would include 99% of
+        the values for a Gaussian distribution.
+    corr:
+        if ``True``, the correlation coefficients are printed on the plot.
+    epsz: bool
+        If ``True``, the intrinsic scatter is printed on the output plot.
+        Default is ``True``.
+    frac: float
+        Fraction of values to include in the LTS stage.
+        Up to a fraction ``frac`` of the values can be outliers.
+        One must have ``0.5 <= frac <= 1``. Default is ``0.5``.
+
+        NOTE: Set ``frac=1`` to turn off outliers detection.
+    pivot: array_like with shape (m,)
+        If nonzero, then ``lts_hyperfit`` fits the hyperplane::
+
+            z = a + b0*(x0 - pivot[0]) + b1*(x1 - pivot[1]) + ... + bm*(xm - pivot[m])
+
+        ``pivot`` are called ``x_0``, ``y_0`` in eq.(7) of `Cappellari et al. (2013a)`_.
+        Use of this parameter is strongly recommended, and suggested
+        values are ``pivot = np.median(x, 0)``. The fitted parameters are not
+        strongly dependent on the precise value of this parameter. For this
+        reason it is generally better to round the pivot values to nice numbers.
+        This parameter is important to reduce the covariance between the
+        coefficients. Default is ``0``.
+    plot: bool
+        If ``True``, a plot of the fit is produced. Default is ``True``.
+    text: bool
+        If ``True``, the best fitting parameters are printed on the plot.
+        Default is ``True``.
 
     Output Parameters
     -----------------
 
-    The output values are stored as attributed of the lts_linefit class.
+    The output values are stored as attributes of the ``lts_hyperfit`` class.
 
-    p.abc:
-        best fitting parameters [a, b, c]
-    p.abc_err:
-        1*sigma formal errors [a_err, b_err, c_err] on a, b and c.
-    p.mask:
-        boolean vector with the same size of x, y and z.
-        It contains True for the elements of (x, y, z) which were included in
-        the fit and False for the outliers which were automatically clipped.
-    p.rms:
-        rms = np.std(fit - z) beteween the data and the fitted relation.
-    p.sig_int:
-        intrinsic scatter in the z direction around the plane.
-        sig_int is called epsilon_z in eq.(7) of Cappellari et al. (2013).
-    p.sig_int_err:
-        1*sigma formal error on sig_int.
+    p.abc: array_like with shape (m+1,)
+        Best fitting parameters ``[a, b1, b2,..., bm]``.
+    p.abc_err: array_like with shape (m+1,)
+        ``1*sigma`` formal errors ``[a_err, b1_err, b2_err,..., bm_err]`` on
+        ``[a, b1, b2,..., bm]``.
+    p.mask: array_like with shape (n,) and dtype bool
+        Boolean vector indicating which elements of ``z`` were included in
+        the fit (``True``) and which were clipped as outliers (``False``).
+    p.rms: float
+        RMS deviation between the data and the fitted relation.
+    p.sig_int: float
+        Intrinsic scatter in the ``z`` direction around the hyperplane.
+        ``sig_int`` is called ``epsilon_z`` in eq.(7) of `Cappellari et al. (2013a)`_.
+    p.sig_int_err: float
+        ``1*sigma`` formal error on ``sig_int``.
 
     ###########################################################################
 
     """
 
-    def _find_outliers(self, sig_int, x, y, z, sigx, sigy, sigz1, h, offs, clip):
+    def __init__(self, x0, z, sigx, sigz, clip=2.6, corr=True, epsz=True,
+                 frac=None, label='Fitted', label_clip='Clipped', pivot=None,
+                 plot=True, text=True):
+
+        if x0.ndim == 1:
+            x0, sigx = x0[:, None], sigx[:, None]
+
+        n, ndim = x0.shape
+        assert x0.shape == sigx.shape, 'x and sigx must have the same shape'
+        assert n == z.size == sigz.size, 'z, sigz must have length x.shape[0]'
+
+        if pivot is None:
+            print(
+                'WARNING: Using a nonzero `pivot` keyword is always reccomended')
+            pivot = np.zeros(ndim)
+        else:
+            pivot = np.atleast_1d(pivot)
+
+        if not np.all(np.isfinite(np.column_stack([x0, z, sigx, sigz]))):
+            raise ValueError('Input contains non finite values')
+
+        t = clock()
+
+        p = ndim + 1  # space dimension
+        n = z.size
+        h = int((n + p + 1)/2) if frac is None else int(
+            max(round(frac*n), (n + p + 1)/2))
+
+        x = x0 - pivot
+        self._single_fit(x, z, sigx, sigz, h, clip)
+        self.rms = np.std(
+            self.abc[0] + x[self.mask]@self.abc[1:] - z[self.mask], ddof=p)
+
+        par = np.append(self.abc, self.sig_int)
+        sig_par = np.append(self.abc_err, self.sig_int_err)
+        print('################# Values and formal errors ################')
+        string = _display_errors(par, sig_par, epsz)
+        print(f'Observed rms scatter: {self.rms:#.2g}')
+
+        ylabel = 'a + ' + ' + '.join(
+            [f'(x_{j} - p_{j}) b_{j}' for j in range(ndim)])
+        print('z = ' + ylabel)
+        for j, piv in enumerate(pivot):
+            print(f'   p_{j} = {pivot[j]:#.4g}')
+        if p == 2:
+            x, x0, sigx = map(np.ravel, [x, x0, sigx])
+            print('Spearman r=%#.2g and p=%#.2g'%stats.spearmanr(x, z))
+            print('Pearson r=%#.2g and p=%#.2g'%stats.pearsonr(x, z))
+
+        print('##########################################################')
+
+        print('seconds %.2f'%(clock() - t))
+
+        if plot:
+
+            if p == 2:
+                xx = x0
+                zz = z
+                xerr = sigx
+                yerr = sigz
+                xlabel = '$x_0$'
+                ylabel = '$y,\quad y_{\\rm fit} = a + (x_0 - p_{0}) b_0$'
+            else:
+                xx = z
+                zz = par[0] + x@par[1:-1]
+                xerr = sigz
+                yerr = np.sqrt(sigx**2@par[1:-1]**2)
+                xlabel = 'z'
+                ylabel = '$' + ylabel + '$'
+
+            plt.errorbar(xx[self.mask], zz[self.mask], xerr=xerr[self.mask],
+                         yerr=yerr[self.mask], fmt='ob', capthick=0, capsize=0,
+                         label=label)
+            plt.errorbar(xx[~self.mask], zz[~self.mask], xerr=xerr[~self.mask],
+                         yerr=yerr[~self.mask], fmt='d', color='LimeGreen',
+                         capthick=0, capsize=0, label=label_clip)
+
+            xlim = np.array(plt.gca().get_xlim())
+            y1 = par[0] + par[1]*(xlim - pivot) if p == 2 else xlim
+
+            plt.plot(xlim, y1, '-k', xlim, y1 + self.rms, '--r', xlim,
+                     y1 - self.rms, '--r', xlim, y1 + 2.6*self.rms, ':r', xlim,
+                     y1 - 2.6*self.rms, ':r', linewidth=2, zorder=1)
+            plt.xlabel(xlabel)
+            plt.ylabel(ylabel)
+            plt.title('Best fit, 1$\sigma$ (68%) and 2.6$\sigma$ (99%)')
+
+            ax = plt.gca()
+            ax.minorticks_on()
+            if text:
+                string += f'$\Delta={self.rms:#.2g}$\n'
+                if np.any(pivot):
+                    for j, piv in enumerate(pivot):
+                        string += f'$(p_{j}={piv:#.4g})$\n'
+                ax.text(0.05, 0.95, string, horizontalalignment='left',
+                        verticalalignment='top', transform=ax.transAxes)
+
+            if (p == 2) and corr:
+                txt = '${\\rm Spearman/Pearson}$\n'
+                txt += '$r=%#.2g\, p=%#.2g$\n'%stats.spearmanr(x, z)
+                txt += '$r=%#.2g\, p=%#.2g$\n'%stats.pearsonr(x, z)
+                ax.text(0.95, 0.95, txt, horizontalalignment='right',
+                        verticalalignment='top', transform=ax.transAxes)
+
+    # ------------------------------------------------------------------------------
+    def _find_outliers(self, sig_int, x, z, sigx, sigz1, h, offs, clip):
 
         sigz = np.sqrt(sigz1**2 + sig_int**2) # Gaussian intrinsic scatter
 
-        if h == x.size: # No outliers detection
+        if h == len(x): # No outliers detection
 
-            abc = _planefit(x, y, z, sigz=sigz)  # quick initial guess
-            abc, sig_abc, chi_sq = _fitting(x, y, z, sigx, sigy, sigz, abc)
-            mask = np.ones_like(x, dtype=bool)  # No outliers
+            abc = _hyperfit(x, z, sigz=sigz)  # quick initial guess
+            abc, sig_abc, chi_sq = _fitting(x, z, sigx, sigz, abc)
+            mask = np.ones_like(z, dtype=bool)  # No outliers
 
         else: # Robust fit and outliers detection
 
             # Initial estimate using the maximum breakdown of
             # the method of 50% but minimum efficiency
             #
-            abc, mask = _fast_algorithm(x, y, z, sigx, sigy, sigz, h)
+            abc, mask = _fast_algorithm(x, z, sigx, sigz, h)
 
             # inside-out outliers removal
             #
             while True:
-                res = _residuals(abc, x, y, z, sigx, sigy, sigz)
-                sig = np.std(res[mask], ddof=3)
+                res = _residuals(abc, x, z, sigx, sigz)
+                sig = np.std(res[mask], ddof=abc.size)
                 maskOld = mask
                 mask = np.abs(res) < clip*sig
-                abc, sig_abc, chi_sq = _fitting(x[mask], y[mask], z[mask], sigx[mask], sigy[mask], sigz[mask], abc)
+                abc, sig_abc, chi_sq = _fitting(x[mask], z[mask], sigx[mask], sigz[mask], abc)
                 if np.array_equal(mask, maskOld):
                     break
 
         # To determine 1sigma error on the intrinsic scatter the chi2
         # is decreased by 1sigma=sqrt(2(h-3)) while optimizing (a,b,c)
         #
         h = mask.sum()
-        dchi = np.sqrt(2*(h - 3)) if offs else 0.
+        dchi = np.sqrt(2*(h - abc.size)) if offs else 0.
 
         self.abc = abc
         self.abc_err = sig_abc
         self.mask = mask
 
-        err = (chi_sq + dchi)/(h - 3.) - 1
+        err = (chi_sq + dchi)/(h - abc.size) - 1
         print('sig_int: %10.4f  %10.4f' % (sig_int, err))
 
         return err
 
 #------------------------------------------------------------------------------
 
-    def _single_fit(self, x, y, z, sigx, sigy, sigz, h, clip):
+    def _single_fit(self, x, z, sigx, sigz, h, clip):
 
-        if self._find_outliers(0, x, y, z, sigx, sigy, sigz, h, 0, clip) < 0:
+        if self._find_outliers(0, x, z, sigx, sigz, h, 0, clip) < 0:
             print('No intrinsic scatter or errors overestimated')
             sig_int = 0.
             sig_int_err = 0.
         else:
             sig1 = 0.
-            res = self.abc[0] + self.abc[1]*x + self.abc[2]*y - z  # Total residuals ignoring measurement errors
-            std = np.std(res[self.mask], ddof=3)
+            ndim = x.shape[1] + 1
+            res = self.abc[0] + x @ self.abc[1:] - z  # Total residuals ignoring measurement errors
+            std = np.std(res[self.mask], ddof=ndim)
             sig2 = std*(1 + 3/np.sqrt(2*self.mask.sum()))  # Observed scatter + 3sigma error
             print('Computing sig_int')
             sig_int = optimize.brentq(self._find_outliers, sig1, sig2,
-                                      args=(x, y, z, sigx, sigy, sigz, h, 0, clip), rtol=1e-3)
+                                      args=(x, z, sigx, sigz, h, 0, clip), rtol=1e-3)
             print('Computing sig_int error') # chi2 can always decrease
             sigMax_int = optimize.brentq(self._find_outliers, sig_int, sig2,
-                                         args=(x, y, z, sigx, sigy, sigz, h, 1, clip), rtol=1e-3)
+                                         args=(x, z, sigx, sigz, h, 1, clip), rtol=1e-3)
             sig_int_err = sigMax_int - sig_int
 
         self.sig_int = sig_int
         self.sig_int_err = sig_int_err
 
         print('Repeat at best fitting solution')
-        self._find_outliers(sig_int, x, y, z, sigx, sigy, sigz, h, 0, clip)
+        self._find_outliers(sig_int, x, z, sigx, sigz, h, 0, clip)
 
 #------------------------------------------------------------------------------
 
-    def __init__(self, x0, y0, z, sigx, sigy, sigz, clip=2.6, epsz=True,
-                  frac=None, pivotx=0, pivoty=0, plot=True, text=True):
-
-        assert x0.size == y0.size == z.size == sigx.size == sigy.size == sigz.size, '[X, Y, Z, SIGX, SIGY, SIGZ] must have the same size'
-
-        if not np.all(np.isfinite(np.hstack([x0, y0, z, sigx, sigy, sigz]))):
-            raise ValueError('Input contains non finite values')
-
-        t = clock()
-
-        x = x0 - pivotx
-        y = y0 - pivoty
-
-        p = 3  # three dimensions
-        n = x.size
-        h = int((n + p + 1)/2) if frac is None else int(max(round(frac*n), (n + p + 1)/2))
-
-        self._single_fit(x, y, z, sigx, sigy, sigz, h, clip)
-        self.rms = np.std(self.abc[0] + self.abc[1]*x[self.mask] + self.abc[2]*y[self.mask] - z[self.mask], ddof=3)
-
-        par = np.append(self.abc, self.sig_int)
-        sig_par = np.append(self.abc_err, self.sig_int_err)
-        print('################# Values and formal errors ################')
-        string = _display_errors(par, sig_par, epsz)
-        print(f'Observed rms scatter: {self.rms:#.2g}')
-        if pivotx or pivoty:
-            print('z = a + b*(x - pivotx) + c*(y - pivoty)')
-            print('with pivotx = %.4g & pivoty = %.4g' % (pivotx, pivoty))
-        else:
-            print('WARNING: pivotx=0 or pivoty=0. Using `pivotx` and `pivoty` keywords is always reccomended')
-
-        print('##########################################################')
-
-        print('seconds %.2f' % (clock() - t))
-
-        if plot:
-
-            z1 = par[0] + x*par[1] + y*par[2]
-            sigz1 = np.sqrt((sigx*par[1])**2 + (sigy*par[2])**2)
-
-            plt.errorbar(z[self.mask], z1[self.mask], xerr=sigz[self.mask], yerr=sigz1[self.mask],
-                         fmt='ob', capthick=0, capsize=0)
-            if not np.all(self.mask):
-                plt.errorbar(z[~self.mask], z1[~self.mask], xerr=sigz[~self.mask], yerr=sigz1[~self.mask],
-                             fmt='d', color='LimeGreen', capthick=0, capsize=0)
-            xlim = plt.gca().get_xlim()
-            plt.title('Best fit, 1$\sigma$ (68%) and 2.6$\sigma$ (99%)')
-
-            plt.plot(xlim, xlim, '-k',
-                     xlim, xlim + self.rms, '--r',
-                     xlim, xlim - self.rms, '--r',
-                     xlim, xlim + 2.6*self.rms, ':r',
-                     xlim, xlim - 2.6*self.rms, ':r', linewidth=2, zorder=1)
-
-            ax = plt.gca()
-            if text:
-                string += f'$\Delta={self.rms:#.2g}$\n'
-                if pivotx:
-                    string += '$(x_0=%.4g)$\n' % pivotx
-                if pivoty:
-                    string += '$(y_0=%.4g)$' % pivoty
-                ax.text(0.05, 0.95, string, horizontalalignment='left',
-                        verticalalignment='top', transform=ax.transAxes)
-
-            ax.minorticks_on()
-            plt.xlim(xlim)
-
-#------------------------------------------------------------------------------
```

### Comparing `ltsfit-5.0.20/ltsfit.egg-info/PKG-INFO` & `ltsfit-6.0.0/ltsfit.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ltsfit
-Version: 5.0.20
+Version: 6.0.0
 Summary: LtsFit: Least Trimmed Squares Fitting
 Home-page: https://purl.org/cappellari/software
 Author: Michele Cappellari
 Author-email: michele.cappellari@physics.ox.ac.uk
 License: Other/Proprietary License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -12,38 +12,38 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
 
 The LtsFit Package
 ==================
 
-**Robust Linear Regression with Scatter in One or Two Dimensions**
+**Robust Least Squares Regression with Uncertainties and Scatter in Any Dimension**
 
 .. image:: https://img.shields.io/pypi/v/ltsfit.svg
     :target: https://pypi.org/project/ltsfit/
 .. image:: https://img.shields.io/badge/arXiv-1208.3522-orange.svg
     :target: https://arxiv.org/abs/1208.3522
 .. image:: https://img.shields.io/badge/DOI-10.1093/mnras/stt562-green.svg
     :target: https://doi.org/10.1093/mnras/stt562
 
-LtsFit is a Python implementation of the method described in Section 3.2 of
+LtsFit is a Python package for **very robust** hyperplane fitting in N dimensions,
+with uncertainties in all coordinates and intrinsic scatter. It implements the
+method described in Section 3.2 of
 `Cappellari et al. (2013a) <https://ui.adsabs.harvard.edu/abs/2013MNRAS.432.1709C>`_
-to perform **very robust** fits of lines or planes to data with errors in all
-coordinates, while allowing for possible intrinsic scatter.
-Outliers are iteratively clipped using the robust Least Trimmed Squares (LTS)
-technique by `Rousseeuw & van Driessen (2006) <http://doi.org/10.1007/s10618-005-0024-4>`_.
+and uses the Least Trimmed Squares (LTS) technique to iteratively clip outliers
+`(Rousseeuw & van Driessen 2006) <http://doi.org/10.1007/s10618-005-0024-4>`_.
 
 .. contents:: :depth: 2
 
 Attribution
 -----------
 
-If you use this software for your research, please also cite
-`Cappellari et al. (2013a) <https://ui.adsabs.harvard.edu/abs/2013MNRAS.432.1709C>`_
-where the implementation was described. The BibTeX entry for the paper is::
+Please also cite `Cappellari et al. (2013a) <https://ui.adsabs.harvard.edu/abs/2013MNRAS.432.1709C>`_
+if you use this software for your research. This is the paper where the
+implementation was described. The BibTeX entry for the paper is::
 
     @ARTICLE{Cappellari2013a,
         author = {{Cappellari}, M. and {Scott}, N. and {Alatalo}, K. and
             {Blitz}, L. and {Bois}, M. and {Bournaud}, F. and {Bureau}, M. and
             {Crocker}, A.~F. and {Davies}, R.~L. and {Davis}, T.~A. and {de Zeeuw},
             P.~T. and {Duc}, P.-A. and {Emsellem}, E. and {Khochfar}, S. and
             {Krajnovi{\'c}}, D. and {Kuntschner}, H. and {McDermid}, R.~M. and
@@ -67,241 +67,185 @@
 
     pip install ltsfit
 
 Without writing access to the global ``site-packages`` directory, use::
 
     pip install --user ltsfit
 
+To upgrade the package to the latest version use::
+
+    pip install --upgrade ltsfit
+
 Documentation
 -------------
 
 See ``ltsfit/examples`` and the files docstrings.
 They are copied by ``pip`` within the global folder
 `site-packages <https://stackoverflow.com/a/46071447>`_.
 
 ###########################################################################
 
-lts_linefit
-===========
+lts_hyperfit
+============ 
 
 Purpose
 -------
 
-Best straight-line *robust* fit to data with errors in
-both coordinates while fitting for the intrinsic scatter.
-See `Cappellari et al. (2013a, Sec.3.2)
-<https://ui.adsabs.harvard.edu/abs/2013MNRAS.432.1709C>`_
+Fit a linear function of the form::
 
-Explanation
------------
+    z = a + b1*x1 + b2*x2 +...+ bm*xm,
 
-Linear Least-squares approximation in one-dimension (y = a + b*x),
-when both x and y data have errors and allowing for intrinsic
-scatter in the relation.
-
-Outliers are iteratively clipped using the extremely robust
-FAST-LTS technique by
-`Rousseeuw & van Driessen (2006) <http://doi.org/10.1007/s10618-005-0024-4>`_
-See also `Rousseeuw (1987) <http://books.google.co.uk/books?id=woaH_73s-MwC&pg=PA15>`_
+to data with errors in all coordinates and intrinsic scatter, using a robust
+method that clips outliers. The function can handle lines in 2-dim, planes in
+3-dim, or hyperplanes in N-dim, where ``x1, x2,..., xm`` are the independent
+variables and ``z`` is the dependent variable. The method was introduced in
+Sec. 3.2 of `Cappellari et al. (2013a) <https://ui.adsabs.harvard.edu/abs/2013MNRAS.432.1709C>`_
+and the treatment of outliers is is based on the FAST-LTS technique by
+`Rousseeuw & van Driessen (2006) <http://doi.org/10.1007/s10618-005-0024-4>`_.
+See also `Rousseeuw (1987) <http://books.google.co.uk/books?id=woaH_73s-MwC&pg=PA15>`_.
 
 Calling Sequence
 ----------------
 
 .. code-block:: python
 
-    p = lts_linefit(x, y, sigx, sigy, clip=2.6, epsy=True, corr=True,
-                  frac=None, pivot=None, plot=True, text=True)
-
-The output values are stored as attributes of "p".
-See usage example at the bottom of this file.
-
-Input Parameters
-----------------
-
-x, y:
-    vectors of size N with the measured values.
-sigx, sigy:
-    vectors of size N with the 1sigma errors in x and y.
-clip:
-    values deviating more than clip*sigma from the best fit are
-    considered outliers and are excluded from the linear fit.
-epsy:
-    if True, the intrinsic scatter is printed on the plot.
-corr:
-    if True, the correlation coefficients are printed on the plot.
-frac:
-    fractions of values to include in the LTS stage.
-    Up to a fraction "frac" of the values can be outliers.
-    One must have 0.5 < frac < 1  (default frac=0.5).
-
-    NOTE: Set frac=1, to turn off outliers detection.
-label:
-    optional string label to create a legend outside the procedure.
-pivot:
-    if this is not None, then lts_linefit fits the relation::
-
-        y = a + b*(x - pivot)
-
-    pivot is called x_0 in eq.(6) of Cappellari et al. (2013)
-    Use of this keyword is *strongly* recommended and a suggested
-    value is pivot ~ np.mean(x). This keyword is important to
-    reduce the covariance between a and b.
-plot:
-    if True a plot of the fit is produced.
-text:
-    if True, the best fitting parameters are printed on the plot.
-
-Output Parameters
------------------
-
-The output values are stored as attributed of the lts_linefit class.
-
-p.ab:
-    best fitting parameters [a, b]
-p.ab_err:
-    1*sigma formal errors [a_err, b_err] on a and b.
-p.mask:
-    boolean vector with the same size of x and y.
-    It contains True  for the elements of (x, y) which were included in
-    the fit and False for the outliers which were automatically clipped.
-p.rms:
-    rms = np.std(fit - y) beteween the data and the fitted relation.
-p.sig_int:
-    intrinsic scatter around the linear relation.
-    sig_int is called epsilon_y in eq.(6) of Cappellari et al. (2013).
-p.sig_int_err:
-    1*sigma formal error on sig_int.
-
-###########################################################################
-
+    from ltsfit.lts_hyperfit import lts_hyperfit
 
-lts_planefit
-============
+    p = lts_hyperfit(x, z, sigx, sigz, clip=2.6, corr=True, epsz=True,
+             frac=None, label='Fitted', label_clip='Clipped', pivot=0,
+             plot=True, text=True)
 
-Purpose
--------
-
-Best plane *robust* fit to data with errors in all
-three coordinates and fitting for the intrinsic scatter.
-See `Cappellari et al. (2013a, Sec.3.2)
-<https://ui.adsabs.harvard.edu/abs/2013MNRAS.432.1709C>`_
-
-Explanation
------------
+The output values are stored as attributes of the ``p`` object.
 
-Linear Least-squares approximation in two-dimension (z = a + b*x + c*y),
-when x, y and z data have errors, and allowing for intrinsic
-scatter in the relation.
-
-Outliers are iteratively clipped using the extremely robust
-FAST-LTS technique by
-`Rousseeuw & van Driessen (2006) <http://doi.org/10.1007/s10618-005-0024-4>`_
-See also `Rousseeuw (1987) <http://books.google.co.uk/books?id=woaH_73s-MwC&pg=PA15>`_
-
-Calling Sequence
+Input Parameters
 ----------------
 
-.. code-block:: python
-
-    p = lts_planefit(x, y, z, sigx, sigy, sigz, clip=2.6, epsz=True,
-                    frac=None, pivotx=None, pivoty=None, plot=True, text=True)
+x: array_like with shape (n, m)
+    Array of ``n`` independent variables for ``m`` dimensions.
 
-The output values are stored as attributes of "p".
-See usage example at the bottom of this file.
+    EXAMPLE: To fit a line in 2-dim, one has a single vector ``xx`` of
+    length ``n`` with the independent variable and a corresponding vector of
+    dependent variable ``yy``. In this case, ``x = xx`` and ``z = yy``.
+
+    EXAMPLE: To fit a plane in 3-dim, one has two vectors of length ``n`` of
+    independent variables ``(xx, yy)``. In this case, ``x = np.column_stack([xx, yy])``.
+
+    EXAMPLE: To fit a hyperplane in 4-dim, one has three vectors of independent
+    variables ``(x1, x2, x3)``. In this case, ``x = np.column_stack([x1, x2, x3])``.
+z: array_like with shape (n,)
+    Vector of ``n`` measured values for each set of ``x`` variables.
+sigx: array_like with shape (n, m)
+    Array of ``n`` values of ``1sigma`` uncertainties for each ``x`` 
+    coordinate for ``m`` dimensions. This has the same shape as ``x``.
+sigz: array_like with shape (n,)
+    Vector of ``n`` values of ``1sigma`` uncertainties for each ``z`` value.
 
-Input Parameters
-----------------
+Optional Keywords
+-----------------
 
-x, y, z:
-    vectors of size N with the measured values.
-sigx, sigy, sigz:
-    vectors of size N with the 1sigma errors in x , y and z.
-clip:
-    values deviating more than clip*sigma from the best fit are
-    considered outliers and are excluded from the plane fit.
-epsz:
-    if True, the intrinsic scatter is printed on the plot.
-frac:
-    fractions of values to include in the LTS stage.
-    Up to a fraction "frac" of the values can be outliers.
-    One must have 0.5 <= frac <= 1  (default frac=0.5).
-
-    NOTE: Set frac=1, to turn off outliers detection.
-pivotx, pivoty:
-    if these are not None, then lts_planefit fits the plane::
-
-        z = a + b*(x - pivotx) + c*(y - pivoty)
-
-    pivotx, pivoty are called x_0, y_0 in eq.(7) of Cappellari et al. (2013)
-    Use of these keywords is *strongly* recommended, and suggested
-    values are ``pivotx=np.median(x), pivoty=np.median(y)``.
-    This keyword is important to reduce the covariance between a, b and c.
-plot:
-    if True a plot of the fit is produced.
-text:
-    if True, the best fitting parameters are printed on the plot.
+clip: float
+    Clipping threshold in ``sigma`` units. Values deviating more than
+    ``clip*sigma`` from the best fit are considered outliers and are
+    excluded from the fit. Default is ``2.6``, which would include 99% of
+    the values for a Gaussian distribution.
+corr:
+    if ``True``, the correlation coefficients are printed on the plot.
+epsz: bool
+    If ``True``, the intrinsic scatter is printed on the output plot.
+    Default is ``True``.
+frac: float
+    Fraction of values to include in the LTS stage.
+    Up to a fraction ``frac`` of the values can be outliers.
+    One must have ``0.5 <= frac <= 1``. Default is ``0.5``.
+
+    NOTE: Set ``frac=1`` to turn off outliers detection.
+pivot: array_like with shape (m,)
+    If nonzero, then ``lts_hyperfit`` fits the hyperplane::
+
+        z = a + b0*(x0 - pivot[0]) + b1*(x1 - pivot[1]) + ... + bm*(xm - pivot[m])
+
+    ``pivot`` are called ``x_0``, ``y_0`` in eq.(7) of `Cappellari et al. (2013a)`_.
+    Use of this parameter is strongly recommended, and suggested
+    values are ``pivot = np.median(x, 0)``. The fitted parameters are not
+    strongly dependent on the precise value of this parameter. For this
+    reason it is generally better to round the pivot values to nice numbers.
+    This parameter is important to reduce the covariance between the
+    coefficients. Default is ``0``.
+plot: bool
+    If ``True``, a plot of the fit is produced. Default is ``True``.
+text: bool
+    If ``True``, the best fitting parameters are printed on the plot.
+    Default is ``True``.
 
 Output Parameters
 -----------------
 
-The output values are stored as attributed of the lts_linefit class.
+The output values are stored as attributes of the ``lts_hyperfit`` class.
 
-p.abc:
-    best fitting parameters [a, b, c]
-p.abc_err:
-    1*sigma formal errors [a_err, b_err, c_err] on a, b and c.
-p.mask:
-    boolean vector with the same size of x, y and z.
-    It contains True for the elements of (x, y, z) which were included in
-    the fit and False for the outliers which were automatically clipped.
-p.rms:
-    rms = np.std(fit - z) beteween the data and the fitted relation.
-p.sig_int:
-    intrinsic scatter in the z direction around the plane.
-    sig_int is called epsilon_z in eq.(7) of Cappellari et al. (2013).
-p.sig_int_err:
-    1*sigma formal error on sig_int.
+p.abc: array_like with shape (m+1,)
+    Best fitting parameters ``[a, b1, b2,..., bm]``.
+p.abc_err: array_like with shape (m+1,)
+    ``1*sigma`` formal errors ``[a_err, b1_err, b2_err,..., bm_err]`` on
+    ``[a, b1, b2,..., bm]``.
+p.mask: array_like with shape (n,) and dtype bool
+    Boolean vector indicating which elements of ``z`` were included in
+    the fit (``True``) and which were clipped as outliers (``False``).
+p.rms: float
+    RMS deviation between the data and the fitted relation.
+p.sig_int: float
+    Intrinsic scatter in the ``z`` direction around the hyperplane.
+    ``sig_int`` is called ``epsilon_z`` in eq.(7) of `Cappellari et al. (2013a)`_.
+p.sig_int_err: float
+    ``1*sigma`` formal error on ``sig_int``.
 
 ###########################################################################
 
 
 
 License
 =======
 
 Other/Proprietary License
 
-Copyright (c) 2012-2022 Michele Cappellari
+Copyright (c) 2012-2023 Michele Cappellari
 
-This software is provided as is without any warranty whatsoever.
-Permission to use, for non-commercial purposes is granted.
-Permission to modify for personal or internal use is granted,
-provided this copyright and disclaimer are included in all 
-copies of the software. All other rights are reserved.
-In particular, redistribution of the code is not allowed.
+This software is provided as is with no warranty. You may use it for
+non-commercial purposes and modify it for personal or internal use, as long
+as you include this copyright and disclaimer in all copies. You may not
+redistribute the code.
+
+###########################################################################
 
 Changelog
 =========
 
-V2.0.20: MC, Oxford, 3 October 2022
+V6.0.0: MC, Oxford, 7 July 2023
+  - Added ``lts_hyperfit`` to fit hyperplanes in N-dim. This procedure
+    generalizes and replaces both ``lts_linefit`` and ``lts_planefit``, which
+    are now deprecated wrappers for ``lts_hyperfit``. This change was suggested
+    and motivated by Francesco D'Eugenio (cam.ac.uk), who shared his own 4-dim
+    ``lts_hyperfit`` and his paper on a useful application.
+  - Fixed inconsistency between the version number on PyPi and in the Changelog.
+
+V5.0.20: MC, Oxford, 3 October 2022
   - Fixed program stop due to Matplotlib change.
     Thanks to Hitesh Lala (Heidelberg) for the report.
   - Extract documentation from docstrings and show it on PyPi.
 
-V2.0.19: MC, Oxford, 22 January 2021
+V5.0.19: MC, Oxford, 22 January 2021
   - Fixed incorrect plot ranges due to a Matplotlib change.
     Thanks to Davide Bevacqua (unibo.it) for the report.
 
-V2.0.18: MC, Oxford, 17 February 2020
+V5.0.18: MC, Oxford, 17 February 2020
   - Properly print significant trailing zeros in results.
 
-V2.0.17: MC, Oxford, 22 January 2020
+V5.0.17: MC, Oxford, 22 January 2020
   - Formatted documentation as docstring.
   - Included p.rms output.
-
+  - Published on PyPi. Increased major version number by mistake.
 
 V2.0.16: MC, Oxford, 27 September 2018
   - Fixed clock DeprecationWarning in Python 3.7.
 
 V2.0.15: MC, Oxford, 12 May 2018
   - Dropped Python 2.7 support.
```

### Comparing `ltsfit-5.0.20/setup.py` & `ltsfit-6.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,16 +14,15 @@
     docstring = re.search(rex, main_file).group(1)
     return docstring.replace("\n    ", "\n")
 
 setup(name=package,
       version=find_version(package),
       description='LtsFit: Least Trimmed Squares Fitting',
       long_description=open(package + "/README.rst").read()
-                       + read_docstring(package, "lts_linefit")
-                       + read_docstring(package, "lts_planefit")
+                       + read_docstring(package, "lts_hyperfit")
                        + "\n\nLicense\n=======\n\n"
                        + open(package + "/LICENSE.txt").read()
                        + open(package + "/CHANGELOG.rst").read(),
       long_description_content_type='text/x-rst',
       url="https://purl.org/cappellari/software",
       author="Michele Cappellari",
       author_email="michele.cappellari@physics.ox.ac.uk",
```

