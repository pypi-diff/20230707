# Comparing `tmp/tablespoon-0.4.7.tar.gz` & `tmp/tablespoon-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tablespoon-0.4.7.tar", max compression
+gzip compressed data, was "tablespoon-0.4.8.tar", max compression
```

## Comparing `tablespoon-0.4.7.tar` & `tablespoon-0.4.8.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1068 2022-12-16 20:31:51.130983 tablespoon-0.4.7/LICENSE
--rw-r--r--   0        0        0     8862 2022-12-16 20:31:51.130983 tablespoon-0.4.7/README.md
--rw-r--r--   0        0        0      964 2022-12-16 20:33:03.288673 tablespoon-0.4.7/pyproject.toml
--rw-r--r--   0        0        0       61 2022-12-16 20:32:39.836175 tablespoon-0.4.7/tablespoon/__init__.py
--rw-r--r--   0        0        0   432508 2022-12-16 20:31:51.138984 tablespoon-0.4.7/tablespoon/data.py
--rw-r--r--   0        0        0    12065 2022-12-16 20:31:51.138984 tablespoon-0.4.7/tablespoon/forecasters.py
--rw-r--r--   0        0        0     3428 2022-12-16 20:31:51.138984 tablespoon-0.4.7/tablespoon/model_selection.py
--rw-r--r--   0        0        0     9850 1970-01-01 00:00:00.000000 tablespoon-0.4.7/setup.py
--rw-r--r--   0        0        0     9779 1970-01-01 00:00:00.000000 tablespoon-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-02-02 15:48:15.619144 tablespoon-0.4.8/LICENSE
+-rw-r--r--   0        0        0     8862 2023-02-02 15:48:15.619272 tablespoon-0.4.8/README.md
+-rw-r--r--   0        0        0      955 2023-07-07 19:51:34.922730 tablespoon-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0       84 2023-02-02 15:48:15.627496 tablespoon-0.4.8/tablespoon/__init__.py
+-rw-r--r--   0        0        0   432508 2023-02-02 15:48:15.628400 tablespoon-0.4.8/tablespoon/data.py
+-rw-r--r--   0        0        0    12065 2023-02-02 15:48:15.628579 tablespoon-0.4.8/tablespoon/forecasters.py
+-rw-r--r--   0        0        0     3428 2023-02-02 15:48:15.628691 tablespoon-0.4.8/tablespoon/model_selection.py
+-rw-r--r--   0        0        0     9815 1970-01-01 00:00:00.000000 tablespoon-0.4.8/PKG-INFO
```

### Comparing `tablespoon-0.4.7/LICENSE` & `tablespoon-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tablespoon-0.4.7/README.md` & `tablespoon-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `tablespoon-0.4.7/pyproject.toml` & `tablespoon-0.4.8/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -19,21 +19,21 @@
   "seasonal naive",
   "mean forecast",
 ]
 license = "MIT"
 name = "tablespoon"
 readme = "README.md"
 repository = "https://github.com/alexhallam/tablespoon"
-version = "0.4.7"
+version = "0.4.8"
 
 [tool.poetry.dependencies]
 numpy = "^1.21.2"
 pandas = "^1.3.2"
-pytest = "^6.2.5"
-python = ">=3.7.1,<3.11"
+pytest = "7.0.0"
+python = ">=3.8"
 scipy = "^1.7.3"
 statsmodels = "^0.13.2"
 
 [tool.poetry.dev-dependencies]
 numpy = "^1.21.2"
 pandas = "^1.3.2"
```

### Comparing `tablespoon-0.4.7/tablespoon/data.py` & `tablespoon-0.4.8/tablespoon/data.py`

 * *Files identical despite different names*

### Comparing `tablespoon-0.4.7/tablespoon/forecasters.py` & `tablespoon-0.4.8/tablespoon/forecasters.py`

 * *Files identical despite different names*

### Comparing `tablespoon-0.4.7/tablespoon/model_selection.py` & `tablespoon-0.4.8/tablespoon/model_selection.py`

 * *Files identical despite different names*

### Comparing `tablespoon-0.4.7/setup.py` & `tablespoon-0.4.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,219 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: tablespoon
+Version: 0.4.8
+Summary: Simple probabilistic time series benchmark models
+Home-page: https://alexhallam.github.io/tablespoon/
+License: MIT
+Keywords: forecasting,forecast,probabilistic,naive,benchmark,seasonal naive,mean forecast
+Author: Alex Hallam
+Author-email: alexhallam6.28@gmail.com
+Requires-Python: >=3.8
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: numpy (>=1.21.2,<2.0.0)
+Requires-Dist: pandas (>=1.3.2,<2.0.0)
+Requires-Dist: pytest (==7.0.0)
+Requires-Dist: scipy (>=1.7.3,<2.0.0)
+Requires-Dist: statsmodels (>=0.13.2,<0.14.0)
+Project-URL: Repository, https://github.com/alexhallam/tablespoon
+Description-Content-Type: text/markdown
+
+[![Python application](https://github.com/alexhallam/tablespoon/actions/workflows/python-app.yml/badge.svg)](https://github.com/alexhallam/tablespoon/actions/workflows/python-app.yml)
+
+<h1 align="center">tablespoon</h1>
+<p align="center"><b>T</b>ime-series <b>B</b>enchmark methods that are <b>S</b>imple and <b>P</b>robabilistic</p>
+
+<p align="center"><img align="center" src="assets/tbsp.png" width="100" /></p>
+
+
+# Documentation and quick links
+- [Documentation and quick links](#documentation-and-quick-links)
+- [Introduction](#introduction)
+- [Why Run Simple Methods](#why-run-simple-methods)
+- [Quick Example](#quick-example)
+    - [Seasonal Example](#seasonal-example)
+    - [Stock Prediction](#stock-prediction)
+- [Goals of this package](#goals-of-this-package)
+- [Non-Goals](#non-goals)
+- [Installation](#installation)
+    - [Python](#python)
+- [Citation](#citation)
+- [References](#references)
+- [Recommended probabilistic forecasting packages](#recommended-probabilistic-forecasting-packages)
+- [Learn more about forecasting](#learn-more-about-forecasting)
+- [Built with poetry and pushed to pypi](#built-with-poetry-and-pushed-to-pypi)
+
+# Introduction
+
+Many methods exist for probabilistic forecasting. If you are looking for an
+impressive probabilistic forecasting package see the list of recommendation at
+the bottom of this README. This package is <b>exceptionally ordinary</b>. It is
+expected that this package may be used as a compliment to what is already out
+there.
+
+# Why Run Simple Methods
+
+We have found, by experience, many good uses for the methods in this package.
+To often we see that forecast methods go in production without a naive method to
+accompany it. This is a missed opportunity.
+
+1. **Naive May Be Good Enough**: How good is good enough? I have almost never started a project where the firm receiving the forecast knew the answer to this question, but it is important to get to it early. I think all of us would agree that a forecast error of 0 is best, but in reality how much time should be spent spinning our wheels to get there. Further, many business applications can’t be improved upon even with significant forecast error reduction. I remember hearing a story of a firm which ordered units on pallets. The firm paid by the pallet, not the unit. The forecast team was able to reduce the forecast error, but in the end this did not change the outcome. This is the ‘pallet problem’. As data scientists it is easy to think of error reduction as a continuous function, but this need not map the same way to business value. In this example the continuous error reduction mapped to a discrete pallet. This is a long way of saying, “A naive forecast may be good enough”. What is a naive forecasting method? I typically think of two methods. The mean forecast and the naive forecast. I will go over these in more detail below. There are also some applications where naive methods have been shown to be hard to beat.
+2. **Get A Denominator for Relative Metrics**: Though naive methods can usually
+   be beat it is good to know the relative improvement over the benchmark. This
+   can allow a forecasting team to market their alternative forecast when the
+   'skill score' is impressive.
+3. **Easy to productionize and get expectations**: Get a sense for *how good is
+   good enough*. In many applications a forecast team is asked to forecast, but
+   stakeholders provide no line-in-the-sand for when the forecasting work needs
+   to stop. One reasonable approach is to run the benchmarks found in this
+   package then beat the best performing benchmark by a margin that is
+   statistically significant.
+4. **Resilience in Production - Why not have many models?**: Sometimes, despite
+   best efforts the production model does something unexpected. In this
+   case it is nice to have a simple backup that is cheap to generate and good
+   enough to fall back on. In this way a production forecast pipeline gains
+   strength from a diversity of models.
+5. **Easy Uncertainty Quantification**: Recently we see that applications
+   are not about forecast accuracy, but instead about forecasting uncertainty.
+   Capturing the full distribution helps firms set "service levels" aka
+   percentiles of the distribution for which they are prepared to serve. Even
+   if you have the worlds most accurate unbiased forecast the median point is
+   , by definition, an underforecast half the time. For this reason it is best to provide a
+   distribution of simulated future values and the firm may decide for
+   themselves what risks they are or are not willing to take.
+
+# Quick Example
+
+We show a quick example below. 
+
+For more examples see [Simple Example](https://alexhallam.github.io/tablespoon/section/plotting/), [Extended Example](https://alexhallam.github.io/tablespoon/section/extended/)
+
+There are also some Notebook examples
+1. [Intro](https://github.com/alexhallam/tablespoon/blob/main/examples/tablespoon.ipynb)
+2. [Time Series Cross Validation & Skill Score](https://github.com/alexhallam/tablespoon/blob/main/examples/time_series_cv.ipynb)
+### Seasonal Example
+
+```python
+import tablespoon as tbsp
+from tablespoon.data import SEAS
+
+sn = tbsp.Snaive()
+df_sn = sn.predict(
+    SEAS, horizon=7 * 4, frequency="D", lag=7, uncertainty_samples=8000
+).assign(model="snaive")
+
+print(df_sn.head(10))
+```
+
+### Stock Prediction
+
+```python
+import tablespoon as tbsp
+from tablespoon.data import APPL
+
+n = tbsp.Naive()
+df_n = n.predict(
+    APPL, horizon=7 * 4, frequency="D", lag=1, uncertainty_samples=8000
+).assign(model="naive")
+
+print(df_n.head(10))
+```
+
+```sh
+          ds  rep    y_sim  model
+0 2022-01-02    0  5.20006  naive
+1 2022-01-02    1  5.16789  naive
+2 2022-01-02    2  5.17641  naive
+3 2022-01-02    3  5.19340  naive
+4 2022-01-02    4  5.20075  naive
+5 2022-01-02    5  5.17681  naive
+6 2022-01-02    6  5.20302  naive
+7 2022-01-02    7  5.18896  naive
+8 2022-01-02    8  5.19622  naive
+9 2022-01-02    9  5.17469  naive
+```
+<p align="center"><img align="center" src="assets/forecasts_n.jpg" width="800" /></p>
+
+
+
+
+# Goals of this package
+
+1. ♙**Simple**: Not just in the forecasts themselves, but also from the
+   users perspective.
+2. ♝**Documented**: It should be very clear exactly how forecasts are getting
+   generated. We document the parameterization of the models to make this as
+   obvious and uninteresting as possible. See [Forecast Method Math Documentation](https://alexhallam.github.io/tablespoon/section/math/)
+3. ♜**Stable**: We want this package to feel rock solid. For this to happen
+   we keep the feature set relatively small. We believe that after the initial 
+   development of this package we should spend out time maintaining the code as
+   oppose to thinking of new features.
+4. ♞**Distributional**: Quantification of uncertainty is the name of
+   the game.
+
+# Non-Goals
+
+1. 🔥**Circut Melting Focus on Speed**: Not to say this is a slow package. In fact, it is very fast! 
+   We just don't put any extra effort to make it faster than `numpy`.
+2. 🤖**New/Complex Forecast Models**: Again, this is out of scope. If you are
+   looking for recommendations please see the bottom of the page.
+
+# Installation
+
+### Python
+
+```
+pip3 install tablespoon
+```
+
+# Citation
+
+If you would like to cite `tablespoon`, please cite it as follows:
+
+Alex Hallam. **tablespoon: Time-series Benchmark methods that are Simple and Probabilistic** https://github.com/alexhallam/tablespoon, 2022. Version 0.4.6.
+
+```
+@misc{tablespoon,
+  author={Alex Hallam},
+  title={{tablespoon}: {Time-series Benchmark methods that are Simple and Probabilistic},
+  howpublished={https://github.com/alexhallam/tablespoon},
+  note={Version 0.4.6,
+  year={2022}
+}
+```
 
-packages = \
-['tablespoon']
+# References
 
-package_data = \
-{'': ['*']}
+1. Hyndman, R.J., & Athanasopoulos, G. (2021) Forecasting: principles and practice, 3rd edition, OTexts: Melbourne, Australia. OTexts.com/fpp3. Accessed on 2021-09-26.
 
-install_requires = \
-['numpy>=1.21.2,<2.0.0',
- 'pandas>=1.3.2,<2.0.0',
- 'pytest>=6.2.5,<7.0.0',
- 'scipy>=1.7.3,<2.0.0',
- 'statsmodels>=0.13.2,<0.14.0']
-
-setup_kwargs = {
-    'name': 'tablespoon',
-    'version': '0.4.7',
-    'description': 'Simple probabilistic time series benchmark models',
-    'long_description': '[![Python application](https://github.com/alexhallam/tablespoon/actions/workflows/python-app.yml/badge.svg)](https://github.com/alexhallam/tablespoon/actions/workflows/python-app.yml)\n\n<h1 align="center">tablespoon</h1>\n<p align="center"><b>T</b>ime-series <b>B</b>enchmark methods that are <b>S</b>imple and <b>P</b>robabilistic</p>\n\n<p align="center"><img align="center" src="assets/tbsp.png" width="100" /></p>\n\n\n# Documentation and quick links\n- [Documentation and quick links](#documentation-and-quick-links)\n- [Introduction](#introduction)\n- [Why Run Simple Methods](#why-run-simple-methods)\n- [Quick Example](#quick-example)\n    - [Seasonal Example](#seasonal-example)\n    - [Stock Prediction](#stock-prediction)\n- [Goals of this package](#goals-of-this-package)\n- [Non-Goals](#non-goals)\n- [Installation](#installation)\n    - [Python](#python)\n- [Citation](#citation)\n- [References](#references)\n- [Recommended probabilistic forecasting packages](#recommended-probabilistic-forecasting-packages)\n- [Learn more about forecasting](#learn-more-about-forecasting)\n- [Built with poetry and pushed to pypi](#built-with-poetry-and-pushed-to-pypi)\n\n# Introduction\n\nMany methods exist for probabilistic forecasting. If you are looking for an\nimpressive probabilistic forecasting package see the list of recommendation at\nthe bottom of this README. This package is <b>exceptionally ordinary</b>. It is\nexpected that this package may be used as a compliment to what is already out\nthere.\n\n# Why Run Simple Methods\n\nWe have found, by experience, many good uses for the methods in this package.\nTo often we see that forecast methods go in production without a naive method to\naccompany it. This is a missed opportunity.\n\n1. **Naive May Be Good Enough**: How good is good enough? I have almost never started a project where the firm receiving the forecast knew the answer to this question, but it is important to get to it early. I think all of us would agree that a forecast error of 0 is best, but in reality how much time should be spent spinning our wheels to get there. Further, many business applications can’t be improved upon even with significant forecast error reduction. I remember hearing a story of a firm which ordered units on pallets. The firm paid by the pallet, not the unit. The forecast team was able to reduce the forecast error, but in the end this did not change the outcome. This is the ‘pallet problem’. As data scientists it is easy to think of error reduction as a continuous function, but this need not map the same way to business value. In this example the continuous error reduction mapped to a discrete pallet. This is a long way of saying, “A naive forecast may be good enough”. What is a naive forecasting method? I typically think of two methods. The mean forecast and the naive forecast. I will go over these in more detail below. There are also some applications where naive methods have been shown to be hard to beat.\n2. **Get A Denominator for Relative Metrics**: Though naive methods can usually\n   be beat it is good to know the relative improvement over the benchmark. This\n   can allow a forecasting team to market their alternative forecast when the\n   \'skill score\' is impressive.\n3. **Easy to productionize and get expectations**: Get a sense for *how good is\n   good enough*. In many applications a forecast team is asked to forecast, but\n   stakeholders provide no line-in-the-sand for when the forecasting work needs\n   to stop. One reasonable approach is to run the benchmarks found in this\n   package then beat the best performing benchmark by a margin that is\n   statistically significant.\n4. **Resilience in Production - Why not have many models?**: Sometimes, despite\n   best efforts the production model does something unexpected. In this\n   case it is nice to have a simple backup that is cheap to generate and good\n   enough to fall back on. In this way a production forecast pipeline gains\n   strength from a diversity of models.\n5. **Easy Uncertainty Quantification**: Recently we see that applications\n   are not about forecast accuracy, but instead about forecasting uncertainty.\n   Capturing the full distribution helps firms set "service levels" aka\n   percentiles of the distribution for which they are prepared to serve. Even\n   if you have the worlds most accurate unbiased forecast the median point is\n   , by definition, an underforecast half the time. For this reason it is best to provide a\n   distribution of simulated future values and the firm may decide for\n   themselves what risks they are or are not willing to take.\n\n# Quick Example\n\nWe show a quick example below. \n\nFor more examples see [Simple Example](https://alexhallam.github.io/tablespoon/section/plotting/), [Extended Example](https://alexhallam.github.io/tablespoon/section/extended/)\n\nThere are also some Notebook examples\n1. [Intro](https://github.com/alexhallam/tablespoon/blob/main/examples/tablespoon.ipynb)\n2. [Time Series Cross Validation & Skill Score](https://github.com/alexhallam/tablespoon/blob/main/examples/time_series_cv.ipynb)\n### Seasonal Example\n\n```python\nimport tablespoon as tbsp\nfrom tablespoon.data import SEAS\n\nsn = tbsp.Snaive()\ndf_sn = sn.predict(\n    SEAS, horizon=7 * 4, frequency="D", lag=7, uncertainty_samples=8000\n).assign(model="snaive")\n\nprint(df_sn.head(10))\n```\n\n### Stock Prediction\n\n```python\nimport tablespoon as tbsp\nfrom tablespoon.data import APPL\n\nn = tbsp.Naive()\ndf_n = n.predict(\n    APPL, horizon=7 * 4, frequency="D", lag=1, uncertainty_samples=8000\n).assign(model="naive")\n\nprint(df_n.head(10))\n```\n\n```sh\n          ds  rep    y_sim  model\n0 2022-01-02    0  5.20006  naive\n1 2022-01-02    1  5.16789  naive\n2 2022-01-02    2  5.17641  naive\n3 2022-01-02    3  5.19340  naive\n4 2022-01-02    4  5.20075  naive\n5 2022-01-02    5  5.17681  naive\n6 2022-01-02    6  5.20302  naive\n7 2022-01-02    7  5.18896  naive\n8 2022-01-02    8  5.19622  naive\n9 2022-01-02    9  5.17469  naive\n```\n<p align="center"><img align="center" src="assets/forecasts_n.jpg" width="800" /></p>\n\n\n\n\n# Goals of this package\n\n1. ♙**Simple**: Not just in the forecasts themselves, but also from the\n   users perspective.\n2. ♝**Documented**: It should be very clear exactly how forecasts are getting\n   generated. We document the parameterization of the models to make this as\n   obvious and uninteresting as possible. See [Forecast Method Math Documentation](https://alexhallam.github.io/tablespoon/section/math/)\n3. ♜**Stable**: We want this package to feel rock solid. For this to happen\n   we keep the feature set relatively small. We believe that after the initial \n   development of this package we should spend out time maintaining the code as\n   oppose to thinking of new features.\n4. ♞**Distributional**: Quantification of uncertainty is the name of\n   the game.\n\n# Non-Goals\n\n1. 🔥**Circut Melting Focus on Speed**: Not to say this is a slow package. In fact, it is very fast! \n   We just don\'t put any extra effort to make it faster than `numpy`.\n2. 🤖**New/Complex Forecast Models**: Again, this is out of scope. If you are\n   looking for recommendations please see the bottom of the page.\n\n# Installation\n\n### Python\n\n```\npip3 install tablespoon\n```\n\n# Citation\n\nIf you would like to cite `tablespoon`, please cite it as follows:\n\nAlex Hallam. **tablespoon: Time-series Benchmark methods that are Simple and Probabilistic** https://github.com/alexhallam/tablespoon, 2022. Version 0.4.6.\n\n```\n@misc{tablespoon,\n  author={Alex Hallam},\n  title={{tablespoon}: {Time-series Benchmark methods that are Simple and Probabilistic},\n  howpublished={https://github.com/alexhallam/tablespoon},\n  note={Version 0.4.6,\n  year={2022}\n}\n```\n\n# References\n\n1. Hyndman, R.J., & Athanasopoulos, G. (2021) Forecasting: principles and practice, 3rd edition, OTexts: Melbourne, Australia. OTexts.com/fpp3. Accessed on 2021-09-26.\n\n# Recommended probabilistic forecasting packages\n\nThere are many packages that can compliment `tablespoon`\n\n[forecast](https://github.com/robjhyndman/forecast): The king of forecasting\npackages. Rob Hyndman is a professor of forecasting and has served as editor of\nthe journal "International Journal of Forecasting". If you are new to\nforecasting please read his free ebook [fpp3](https://otexts.com/fpp3/).\n\n[prophet](https://facebook.github.io/prophet/): A very capable and reliable\nforecasting package. I have never seen a bad forecast come out of prophet.\n\n[gluonts](https://ts.gluon.ai/). If you are itching to use neural nets for\nforecasting this is a good one to pick.\n\n# Learn more about forecasting\n\n1. Read [fpp3](https://otexts.com/fpp3/)\n2. Join the [International Institute of Forecasting](https://forecasters.org/)\n   and read their publications.\n   \n# Built with poetry and pushed to pypi\n\n```sh\npoetry publish -u <username> -p <password> --build\n```\n',
-    'author': 'Alex Hallam',
-    'author_email': 'alexhallam6.28@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://alexhallam.github.io/tablespoon/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7.1,<3.11',
-}
+# Recommended probabilistic forecasting packages
+
+There are many packages that can compliment `tablespoon`
+
+[forecast](https://github.com/robjhyndman/forecast): The king of forecasting
+packages. Rob Hyndman is a professor of forecasting and has served as editor of
+the journal "International Journal of Forecasting". If you are new to
+forecasting please read his free ebook [fpp3](https://otexts.com/fpp3/).
+
+[prophet](https://facebook.github.io/prophet/): A very capable and reliable
+forecasting package. I have never seen a bad forecast come out of prophet.
+
+[gluonts](https://ts.gluon.ai/). If you are itching to use neural nets for
+forecasting this is a good one to pick.
+
+# Learn more about forecasting
+
+1. Read [fpp3](https://otexts.com/fpp3/)
+2. Join the [International Institute of Forecasting](https://forecasters.org/)
+   and read their publications.
+   
+# Built with poetry and pushed to pypi
 
+```sh
+poetry publish -u <username> -p <password> --build
+```
 
-setup(**setup_kwargs)
```

