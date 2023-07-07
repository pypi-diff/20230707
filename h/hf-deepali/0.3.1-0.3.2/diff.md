# Comparing `tmp/hf-deepali-0.3.1.tar.gz` & `tmp/hf-deepali-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hf-deepali-0.3.1.tar", last modified: Sun Jun 25 01:57:33 2023, max compression
+gzip compressed data, was "hf-deepali-0.3.2.tar", last modified: Fri Jul  7 02:10:15 2023, max compression
```

## Comparing `hf-deepali-0.3.1.tar` & `hf-deepali-0.3.2.tar`

### file list

```diff
@@ -1,246 +1,251 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.168572 hf-deepali-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.136572 hf-deepali-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.140571 hf-deepali-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.140571 hf-deepali-0.3.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10865 2023-06-25 01:57:33.168572 hf-deepali-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/TODO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.144572 hf-deepali-0.3.1/conda/
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/conda/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/conda/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   544972 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/conda/environment.conda-lock.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/conda/environment.devenv.yml
--rw-r--r--   0 runner    (1001) docker     (123)    53117 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/conda/environment.linux-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)    45139 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/conda/environment.osx-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)    47699 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/conda/environment.win-64.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.144572 hf-deepali-0.3.1/docker/
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/docker/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (123)     1252 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/docker/build
--rwxr-xr-x   0 runner    (1001) docker     (123)     7011 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/docker/run
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.144572 hf-deepali-0.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/docs/_citations.bib
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/docs/_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.144572 hf-deepali-0.3.1/docs/_images/
--rw-r--r--   0 runner    (1001) docker     (123)   390208 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/docs/_images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/docs/_toc.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.144572 hf-deepali-0.3.1/docs/basics/
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/docs/basics/example-page.md
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/docs/basics/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.136572 hf-deepali-0.3.1/docs/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.144572 hf-deepali-0.3.1/docs/reference/core/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/docs/reference/core/domain.md
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/docs/reference/core/flow.md
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/docs/reference/core/image.md
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/docs/reference/core/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/docs/reference/core/kernels.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.144572 hf-deepali-0.3.1/docs/reference/data/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/docs/reference/data/dataset.md
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/docs/reference/data/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/docs/reference/data/sampler.md
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/docs/reference/data/tensor.md
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/docs/reference/data/transforms.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.144572 hf-deepali-0.3.1/docs/reference/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/docs/reference/losses/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.144572 hf-deepali-0.3.1/docs/reference/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/docs/reference/modules/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.144572 hf-deepali-0.3.1/docs/reference/networks/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/docs/reference/networks/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.148572 hf-deepali-0.3.1/docs/reference/spatial/
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/docs/reference/spatial/common.md
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/docs/reference/spatial/composite.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/docs/reference/spatial/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/docs/reference/spatial/transformer.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.148572 hf-deepali-0.3.1/docs/reference/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/docs/reference/utils/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.148572 hf-deepali-0.3.1/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/docs/tutorials/example-myst-notebook.md
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/docs/tutorials/example-notebook.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.148572 hf-deepali-0.3.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.148572 hf-deepali-0.3.1/examples/ffd/
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/examples/ffd/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/examples/ffd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/examples/ffd/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/examples/ffd/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/examples/ffd/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    15655 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/examples/ffd/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/examples/ffd/optim.py
--rw-r--r--   0 runner    (1001) docker     (123)    32029 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/examples/ffd/pairwise.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/examples/ffd/params.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/examples/ffd/register.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.148572 hf-deepali-0.3.1/examples/istn/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/examples/istn/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/examples/istn/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.148572 hf-deepali-0.3.1/examples/istn/models/
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/examples/istn/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/examples/istn/models/itn.py
--rw-r--r--   0 runner    (1001) docker     (123)    23118 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/examples/istn/models/stn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/examples/istn/params.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/examples/istn/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    27864 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/examples/istn/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/pyrightconfig.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 01:57:33.168572 hf-deepali-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.140571 hf-deepali-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.140571 hf-deepali-0.3.1/src/deepali/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.152572 hf-deepali-0.3.1/src/deepali/core/
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19990 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/core/_kornia.py
--rw-r--r--   0 runner    (1001) docker     (123)    20523 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/core/affine.py
--rw-r--r--   0 runner    (1001) docker     (123)    23068 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/core/bspline.py
--rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    24560 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/core/cube.py
--rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/core/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)    20230 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/core/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     6600 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/core/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)    74085 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/core/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    78389 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/core/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/core/itertools.py
--rw-r--r--   0 runner    (1001) docker     (123)    11707 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/core/kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)    19590 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/core/linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/core/math.py
--rw-r--r--   0 runner    (1001) docker     (123)    16778 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/core/nnutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/core/path.py
--rw-r--r--   0 runner    (1001) docker     (123)    15209 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/core/pointset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/core/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/core/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/core/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.156572 hf-deepali-0.3.1/src/deepali/data/
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/data/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)    19020 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    25444 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/data/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    60218 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/data/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/data/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/data/prepare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/data/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/data/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/data/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.156572 hf-deepali-0.3.1/src/deepali/data/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/data/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16698 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/data/transforms/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    10220 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/data/transforms/item.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.156572 hf-deepali-0.3.1/src/deepali/losses/
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/losses/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/losses/bspline.py
--rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/losses/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    66444 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/losses/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)    13371 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/losses/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/losses/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/losses/pointset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.160572 hf-deepali-0.3.1/src/deepali/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/modules/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/modules/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/modules/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/modules/lambd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/modules/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/modules/output.py
--rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/modules/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/modules/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.160572 hf-deepali-0.3.1/src/deepali/networks/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/networks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.160572 hf-deepali-0.3.1/src/deepali/networks/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/networks/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15305 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/networks/blocks/residual.py
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/networks/blocks/skip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.160572 hf-deepali-0.3.1/src/deepali/networks/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/networks/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/networks/layers/acti.py
--rw-r--r--   0 runner    (1001) docker     (123)    15670 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/networks/layers/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/networks/layers/join.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/networks/layers/lambd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/networks/layers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/networks/layers/norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/networks/layers/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    18748 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/networks/layers/upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)    19757 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/networks/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    42873 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/networks/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/networks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.164572 hf-deepali-0.3.1/src/deepali/spatial/
--rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/spatial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22600 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/spatial/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13325 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/spatial/bspline.py
--rw-r--r--   0 runner    (1001) docker     (123)    14024 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/spatial/composite.py
--rw-r--r--   0 runner    (1001) docker     (123)    16517 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/spatial/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/spatial/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    29197 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/spatial/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    12595 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/spatial/nonrigid.py
--rw-r--r--   0 runner    (1001) docker     (123)    17025 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/spatial/parametric.py
--rw-r--r--   0 runner    (1001) docker     (123)    12162 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/spatial/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.164572 hf-deepali-0.3.1/src/deepali/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.164572 hf-deepali-0.3.1/src/deepali/utils/aws/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/utils/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12704 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/utils/aws/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.164572 hf-deepali-0.3.1/src/deepali/utils/aws/s3/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/utils/aws/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21551 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/utils/aws/s3/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/utils/aws/s3/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/utils/aws/s3/object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.164572 hf-deepali-0.3.1/src/deepali/utils/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/utils/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13233 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/utils/cli/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/utils/cli/environ.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/utils/cli/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/utils/cli/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.164572 hf-deepali-0.3.1/src/deepali/utils/ignite/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/utils/ignite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13542 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/utils/ignite/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.164572 hf-deepali-0.3.1/src/deepali/utils/ignite/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/utils/ignite/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/utils/ignite/metrics/average_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/utils/ignite/metrics/binary_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/utils/ignite/metrics/multilabel_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/utils/ignite/output_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/utils/ignite/score_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.168572 hf-deepali-0.3.1/src/deepali/utils/sitk/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/utils/sitk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11201 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/utils/sitk/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/utils/sitk/imageio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/utils/sitk/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/utils/sitk/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/utils/sitk/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/utils/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.168572 hf-deepali-0.3.1/src/deepali/utils/vtk/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/utils/vtk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/utils/vtk/idlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/utils/vtk/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/utils/vtk/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/utils/vtk/polydataio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/src/deepali/utils/vtk/simpleitk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.168572 hf-deepali-0.3.1/src/hf_deepali.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10865 2023-06-25 01:57:33.000000 hf-deepali-0.3.1/src/hf_deepali.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-06-25 01:57:33.000000 hf-deepali-0.3.1/src/hf_deepali.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 01:57:33.000000 hf-deepali-0.3.1/src/hf_deepali.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-25 01:57:33.000000 hf-deepali-0.3.1/src/hf_deepali.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-25 01:57:33.000000 hf-deepali-0.3.1/src/hf_deepali.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:33.168572 hf-deepali-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/tests/_test_core_bspline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/tests/test_core_bspline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/tests/test_core_cube.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/tests/test_core_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/tests/test_core_image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/tests/test_core_random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/tests/test_core_tensor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/tests/test_data_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    22317 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/tests/test_data_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/tests/test_network_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)    11278 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/tests/test_network_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/tests/test_network_resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-06-25 01:57:16.000000 hf-deepali-0.3.1/tests/test_network_unet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:15.017692 hf-deepali-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.969689 hf-deepali-0.3.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.977689 hf-deepali-0.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.977689 hf-deepali-0.3.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10941 2023-07-07 02:10:15.017692 hf-deepali-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/TODO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.981690 hf-deepali-0.3.2/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/conda/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/conda/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   546679 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/conda/environment.conda-lock.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/conda/environment.devenv.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    53215 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/conda/environment.linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    15437 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/conda/environment.linux-64.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    45237 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/conda/environment.osx-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/conda/environment.osx-64.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    47796 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/conda/environment.win-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    14101 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/conda/environment.win-64.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.981690 hf-deepali-0.3.2/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docker/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1666 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docker/build
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7011 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docker/run
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.981690 hf-deepali-0.3.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/_citations.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.981690 hf-deepali-0.3.2/docs/_images/
+-rw-r--r--   0 runner    (1001) docker     (123)   390208 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/_images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/_toc.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.981690 hf-deepali-0.3.2/docs/basics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/basics/example-page.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/basics/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.969689 hf-deepali-0.3.2/docs/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.981690 hf-deepali-0.3.2/docs/reference/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/reference/core/domain.md
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/reference/core/flow.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/reference/core/image.md
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/reference/core/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/reference/core/kernels.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.981690 hf-deepali-0.3.2/docs/reference/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/reference/data/dataset.md
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/reference/data/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/reference/data/sampler.md
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/reference/data/tensor.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/reference/data/transforms.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.981690 hf-deepali-0.3.2/docs/reference/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/reference/losses/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.981690 hf-deepali-0.3.2/docs/reference/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/reference/modules/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.981690 hf-deepali-0.3.2/docs/reference/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/reference/networks/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.985690 hf-deepali-0.3.2/docs/reference/spatial/
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/reference/spatial/common.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/reference/spatial/composite.md
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/reference/spatial/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/reference/spatial/transformer.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.985690 hf-deepali-0.3.2/docs/reference/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/reference/utils/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.985690 hf-deepali-0.3.2/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/tutorials/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/tutorials/example-myst-notebook.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/tutorials/example-notebook.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    45130 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/tutorials/pairwise-registration-intro.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.985690 hf-deepali-0.3.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.985690 hf-deepali-0.3.2/examples/ffd/
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/examples/ffd/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/examples/ffd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/examples/ffd/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/examples/ffd/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/examples/ffd/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15655 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/examples/ffd/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/examples/ffd/optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32029 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/examples/ffd/pairwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/examples/ffd/params.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/examples/ffd/register.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.989690 hf-deepali-0.3.2/examples/istn/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/examples/istn/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/examples/istn/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.989690 hf-deepali-0.3.2/examples/istn/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/examples/istn/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/examples/istn/models/itn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23118 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/examples/istn/models/stn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/examples/istn/params.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/examples/istn/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    27864 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/examples/istn/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/pyrightconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 02:10:15.017692 hf-deepali-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.973689 hf-deepali-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.973689 hf-deepali-0.3.2/src/deepali/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.993690 hf-deepali-0.3.2/src/deepali/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19990 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/core/_kornia.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20523 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/core/affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23068 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/core/bspline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24560 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/core/cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/core/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20230 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/core/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6600 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/core/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74085 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/core/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78527 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/core/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/core/itertools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11707 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/core/kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19590 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/core/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/core/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16778 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/core/nnutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/core/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15209 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/core/pointset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/core/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/core/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/core/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.997691 hf-deepali-0.3.2/src/deepali/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/data/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19020 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24026 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/data/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60823 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/data/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/data/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/data/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/data/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/data/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/data/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.997691 hf-deepali-0.3.2/src/deepali/data/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/data/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16698 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/data/transforms/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10220 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/data/transforms/item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.997691 hf-deepali-0.3.2/src/deepali/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/losses/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/losses/bspline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/losses/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66444 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/losses/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13371 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/losses/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/losses/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/losses/pointset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:15.001691 hf-deepali-0.3.2/src/deepali/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/modules/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/modules/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/modules/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/modules/lambd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/modules/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/modules/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/modules/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/modules/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:15.001691 hf-deepali-0.3.2/src/deepali/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/networks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:15.001691 hf-deepali-0.3.2/src/deepali/networks/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/networks/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15305 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/networks/blocks/residual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/networks/blocks/skip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:15.005691 hf-deepali-0.3.2/src/deepali/networks/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/networks/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/networks/layers/acti.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15670 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/networks/layers/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/networks/layers/join.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/networks/layers/lambd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/networks/layers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/networks/layers/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/networks/layers/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18748 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/networks/layers/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19757 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/networks/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42873 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/networks/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/networks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:15.005691 hf-deepali-0.3.2/src/deepali/spatial/
+-rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/spatial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22600 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/spatial/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13325 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/spatial/bspline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14024 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/spatial/composite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16517 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/spatial/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/spatial/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29197 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/spatial/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12595 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/spatial/nonrigid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17025 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/spatial/parametric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12248 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/spatial/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:15.005691 hf-deepali-0.3.2/src/deepali/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:15.009692 hf-deepali-0.3.2/src/deepali/utils/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15321 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/aws/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:15.009692 hf-deepali-0.3.2/src/deepali/utils/aws/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/aws/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21551 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/aws/s3/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/aws/s3/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/aws/s3/object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:15.009692 hf-deepali-0.3.2/src/deepali/utils/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13233 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/cli/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/cli/environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/cli/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/cli/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:15.009692 hf-deepali-0.3.2/src/deepali/utils/ignite/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/ignite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13542 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/ignite/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:15.009692 hf-deepali-0.3.2/src/deepali/utils/ignite/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/ignite/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/ignite/metrics/average_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/ignite/metrics/binary_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/ignite/metrics/multilabel_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/ignite/output_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/ignite/score_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:15.013692 hf-deepali-0.3.2/src/deepali/utils/sitk/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/sitk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11201 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/sitk/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/sitk/imageio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/sitk/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/sitk/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/sitk/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:15.013692 hf-deepali-0.3.2/src/deepali/utils/vtk/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/vtk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/vtk/idlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/vtk/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/vtk/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/vtk/polydataio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/vtk/simpleitk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:15.013692 hf-deepali-0.3.2/src/hf_deepali.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10941 2023-07-07 02:10:14.000000 hf-deepali-0.3.2/src/hf_deepali.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-07-07 02:10:14.000000 hf-deepali-0.3.2/src/hf_deepali.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 02:10:14.000000 hf-deepali-0.3.2/src/hf_deepali.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-07 02:10:14.000000 hf-deepali-0.3.2/src/hf_deepali.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 02:10:14.000000 hf-deepali-0.3.2/src/hf_deepali.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:15.017692 hf-deepali-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/tests/_test_core_bspline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/tests/test_core_bspline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/tests/test_core_cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/tests/test_core_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/tests/test_core_image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/tests/test_core_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/tests/test_core_tensor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/tests/test_data_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23869 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/tests/test_data_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/tests/test_network_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11278 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/tests/test_network_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/tests/test_network_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/tests/test_network_unet.py
```

### Comparing `hf-deepali-0.3.1/.github/workflows/docs.yml` & `hf-deepali-0.3.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/.github/workflows/release.yml` & `hf-deepali-0.3.2/.github/workflows/release.yml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -39,16 +39,16 @@
           echo version=$(python -m setuptools_scm | awk -F+ '{print $1}' | tail -1) >> $GITHUB_ENV
       - name: Build packages
         run: |
           python -m build
           twine check dist/*
         env:
           SETUPTOOLS_SCM_PRETEND_VERSION: ${{ env.version }}
-      - name: Publish packages to PyPI
-        if: github.event_name == 'release'
-        uses: pypa/gh-action-pypi-publish@release/v1
       - name: Publish packages to Test PyPI
         if: ${{ github.event_name == 'release' || (github.event_name == 'push' && (github.ref == 'refs/heads/main' || github.ref == 'refs/heads/pypi')) }}
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           repository-url: https://test.pypi.org/legacy/
           skip-existing: true
+      - name: Publish packages to PyPI
+        if: github.event_name == 'release'
+        uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `hf-deepali-0.3.1/.github/workflows/tests.yml` & `hf-deepali-0.3.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/.vscode/extensions.json` & `hf-deepali-0.3.2/.vscode/extensions.json`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 {
     "recommendations": [
         // Python
         "ms-python.python",
         "ms-python.vscode-pylance",
+        "ms-toolsai.jupyter",
         // Remote SSH
         "ms-vscode-remote.remote-ssh",
         "ms-vscode-remote.remote-ssh-edit",
         // Code completion
         "visualstudioexptteam.vscodeintellicode",
         // Docker
         "ms-azuretools.vscode-docker",
```

### Comparing `hf-deepali-0.3.1/.vscode/launch.json` & `hf-deepali-0.3.2/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/.vscode/settings.json` & `hf-deepali-0.3.2/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/CODE_OF_CONDUCT.md` & `hf-deepali-0.3.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/LICENSE` & `hf-deepali-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/PKG-INFO` & `hf-deepali-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hf-deepali
-Version: 0.3.1
+Version: 0.3.2
 Summary: Image, point set, and surface registration library for PyTorch.
 Maintainer-email: Andreas Schuh <andreas.schuh@imperial.ac.uk>
 License: Apache-2.0
 Project-URL: Homepage, https://biomedia.github.io/deepali
 Project-URL: Repository, https://github.com/BioMedIA/deepali.git
 Project-URL: Bug Tracker, https://github.com/BioMedIA/deepali/issues
 Keywords: medical-imaging,image-registration,spatial-transformer-networks
@@ -23,16 +23,16 @@
 Provides-Extra: all
 Provides-Extra: utils
 Provides-Extra: tests
 License-File: LICENSE
 
 # deepali
 
-![pypi](https://img.shields.io/pypi/v/hf-deepali)
 <!-- ![downloads](https://img.shields.io/pypi/dm/hf-deepali) -->
+![pypi](https://img.shields.io/pypi/v/hf-deepali)
 ![python](https://img.shields.io/pypi/pyversions/hf-deepali)
 [![docs](https://github.com/BioMedIA/deepali/actions/workflows/docs.yml/badge.svg)](https://github.com/BioMedIA/deepali/actions/workflows/docs.yml)
 [![tests](https://github.com/BioMedIA/deepali/actions/workflows/tests.yml/badge.svg)](https://github.com/BioMedIA/deepali/actions/workflows/tests.yml)
 [![release](https://github.com/BioMedIA/deepali/actions/workflows/release.yml/badge.svg)](https://github.com/BioMedIA/deepali/actions/workflows/release.yml)
 
 An [open source](https://github.com/BioMedIA/deepali/tree/main/LICENSE) research library for image, point set, and surface registration in [PyTorch], which is developed and maintained by the [HeartFlow-Imperial College London] research lab at the [Biomedical Image Analysis Group].
 
@@ -73,15 +73,15 @@
 - [PyTorch]: The automatic differentiation and deep learning framework powering this project.
 - [SimpleITK] (optional): Used by [deepali.data] to read and write images in file formats supported by ITK.
 - [NumPy] (optional): Used by [deepali.utils]. Other components use pure PyTorch.
 - [VTK] (optional): May be used to read and write point sets and surface meshes.
 
 ## Installation
 
-This Python package can be installed with [pip]:
+This library is available as [Python package on PyPI](https://pypi.org/project/hf-deepali/) and can be installed with [pip]:
 
 ```
 pip install hf-deepali
 ```
 
 The latest development version can be installed directly from the GitHub repository, i.e.,
```

### Comparing `hf-deepali-0.3.1/README.md` & `hf-deepali-0.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # deepali
 
-![pypi](https://img.shields.io/pypi/v/hf-deepali)
 <!-- ![downloads](https://img.shields.io/pypi/dm/hf-deepali) -->
+![pypi](https://img.shields.io/pypi/v/hf-deepali)
 ![python](https://img.shields.io/pypi/pyversions/hf-deepali)
 [![docs](https://github.com/BioMedIA/deepali/actions/workflows/docs.yml/badge.svg)](https://github.com/BioMedIA/deepali/actions/workflows/docs.yml)
 [![tests](https://github.com/BioMedIA/deepali/actions/workflows/tests.yml/badge.svg)](https://github.com/BioMedIA/deepali/actions/workflows/tests.yml)
 [![release](https://github.com/BioMedIA/deepali/actions/workflows/release.yml/badge.svg)](https://github.com/BioMedIA/deepali/actions/workflows/release.yml)
 
 An [open source](https://github.com/BioMedIA/deepali/tree/main/LICENSE) research library for image, point set, and surface registration in [PyTorch], which is developed and maintained by the [HeartFlow-Imperial College London] research lab at the [Biomedical Image Analysis Group].
 
@@ -46,15 +46,15 @@
 - [PyTorch]: The automatic differentiation and deep learning framework powering this project.
 - [SimpleITK] (optional): Used by [deepali.data] to read and write images in file formats supported by ITK.
 - [NumPy] (optional): Used by [deepali.utils]. Other components use pure PyTorch.
 - [VTK] (optional): May be used to read and write point sets and surface meshes.
 
 ## Installation
 
-This Python package can be installed with [pip]:
+This library is available as [Python package on PyPI](https://pypi.org/project/hf-deepali/) and can be installed with [pip]:
 
 ```
 pip install hf-deepali
 ```
 
 The latest development version can be installed directly from the GitHub repository, i.e.,
```

### Comparing `hf-deepali-0.3.1/TODO` & `hf-deepali-0.3.2/TODO`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/conda/Makefile` & `hf-deepali-0.3.2/conda/Makefile`

 * *Files 5% similar despite different names*

```diff
@@ -59,29 +59,30 @@
 
 osx: clear lock-osx render
 
 win: clear lock-win render
 
 clear:
 	@echo "Remove all generated files"
-	@rm -f $(LOCKFILE) environment.{linux-64,osx-64,win-64}.{lock,yml}
+	@rm -f $(LOCKFILE) environment.devenv.{linux-64,osx-64,win-64}.yml environment.{linux-64,osx-64,win-64}.{lock,yml}
 
 lock-linux:
-	@$(CONDA_DEVENV) --name $(NAME) --file $(DEVENV) --env-manager $(CONDA) --env-var PLATFORM=linux-64 --print > environment.linux-64.yml
-	@$(CONDA_LOCK) $(CONDA_LOCK_OPTS) --lockfile $(LOCKFILE) --platform linux-64 --file environment.linux-64.yml
+	@$(CONDA_DEVENV) --name $(NAME) --file $(DEVENV) --env-manager $(CONDA) --env-var PLATFORM=linux-64 --print > environment.devenv.linux-64.yml
+	@$(CONDA_LOCK) $(CONDA_LOCK_OPTS) --lockfile $(LOCKFILE) --platform linux-64 --file environment.devenv.linux-64.yml
 
 lock-osx:
-	@$(CONDA_DEVENV) --name $(NAME) --file $(DEVENV) --env-manager $(CONDA) --env-var PLATFORM=osx-64 --print > environment.osx-64.yml
-	@$(CONDA_LOCK) $(CONDA_LOCK_OPTS) --lockfile $(LOCKFILE) --platform osx-64 --file environment.osx-64.yml
+	@$(CONDA_DEVENV) --name $(NAME) --file $(DEVENV) --env-manager $(CONDA) --env-var PLATFORM=osx-64 --print > environment.devenv.osx-64.yml
+	@$(CONDA_LOCK) $(CONDA_LOCK_OPTS) --lockfile $(LOCKFILE) --platform osx-64 --file environment.devenv.osx-64.yml
 
 lock-win:
-	@$(CONDA_DEVENV) --name $(NAME) --file $(DEVENV) --env-manager $(CONDA) --env-var PLATFORM=win-64 --print > environment.win-64.yml
-	@$(CONDA_LOCK) $(CONDA_LOCK_OPTS) --lockfile $(LOCKFILE) --platform win-64 --file environment.win-64.yml
+	@$(CONDA_DEVENV) --name $(NAME) --file $(DEVENV) --env-manager $(CONDA) --env-var PLATFORM=win-64 --print > environment.devenv.win-64.yml
+	@$(CONDA_LOCK) $(CONDA_LOCK_OPTS) --lockfile $(LOCKFILE) --platform win-64 --file environment.devenv.win-64.yml
 
 render:
+	@$(CONDA_LOCK) render $(LOCKFILE) --kind env --filename-template environment.{platform}
 	@$(CONDA_LOCK) render $(LOCKFILE) --kind explicit --filename-template environment.{platform}.lock
 	@if ! grep -e 'pytorch.*cuda' environment.linux-64.lock > /dev/null 2> /dev/null; then \
 		echo "Expected PyTorch with CUDA support for PLATFORM=linux-64. Check conda configuration."; \
 	fi
 
 
 env: create-env install
```

### Comparing `hf-deepali-0.3.1/conda/README.md` & `hf-deepali-0.3.2/conda/README.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/conda/environment.conda-lock.yml` & `hf-deepali-0.3.2/conda/environment.conda-lock.yml`

 * *Files 1% similar despite different names*

```diff
@@ -5,37 +5,37 @@
 # available, unless you explicitly update the lock file.
 #
 # Install this environment as "YOURENV" with:
 #     conda-lock install -n YOURENV --file environment.conda-lock.yml
 # To update a single package to the latest version compatible with the version constraints in the source:
 #     conda-lock lock --lockfile environment.conda-lock.yml --update PACKAGE
 # To re-solve the entire environment, e.g. after changing a version constraint in the source file:
-#     conda-lock -f environment.linux-64.yml -f environment.osx-64.yml -f environment.win-64.yml --lockfile environment.conda-lock.yml
+#     conda-lock -f environment.devenv.linux-64.yml -f environment.devenv.osx-64.yml -f environment.devenv.win-64.yml --lockfile environment.conda-lock.yml
 metadata:
   channels:
   - url: conda-forge
     used_env_vars: []
   - url: pytorch
     used_env_vars: []
   - url: nvidia
     used_env_vars: []
   - url: nodefaults
     used_env_vars: []
   content_hash:
-    linux-64: 404e905e5633264d344750350dd433b9a664952c8bd3a8255d3f31d9eb8a74d7
-    osx-64: 358ba6fb20a9e7c56751c467f43592eee84f35e52b7599dfceb8f0df6af063bb
-    win-64: 814107e5f84db920765778d5de91d5b37fbb12ed6d18c265014da09ea659ff50
+    linux-64: 8bbc0023a299b67380a6493155cba6c46fd177739fbaea7c67b86663b42d8354
+    osx-64: 1664d2c199c9cddb402252a38f5527d218754e954cbb25a82da7fecc8cbae3f6
+    win-64: fe02ca598f6ebbae4e65d2a2d45af1db4913dae4b25d021473f905afc52e3198
   platforms:
   - linux-64
   - osx-64
   - win-64
   sources:
-  - environment.linux-64.yml
-  - environment.osx-64.yml
-  - environment.win-64.yml
+  - environment.devenv.linux-64.yml
+  - environment.devenv.osx-64.yml
+  - environment.devenv.win-64.yml
 package:
 - category: main
   dependencies: {}
   hash:
     md5: d7c89558ba9fa0495403155b64376d81
     sha256: fe51de6107f9edc7aa4f786a70f4a883943bc9d39b3bb7307c04c41410990726
   manager: conda
@@ -636,22 +636,22 @@
   url: https://conda.anaconda.org/conda-forge/linux-64/lerc-4.0.0-h27087fc_0.tar.bz2
   version: 4.0.0
 - category: main
   dependencies:
     libgcc-ng: '>=12'
     libstdcxx-ng: '>=12'
   hash:
-    md5: f67106643beadfc737b94ca0bfd6d8e3
-    sha256: 1778dc86603df24aaf6865f7f3e1ffc5c793a0f1fc4570add2a6ccb4c0a62785
+    md5: d1db1b8be7c3a8983dcbbbfe4f0765de
+    sha256: 3c6fab31ed4dc8428605588454596b307b1bd59d33b0c7073c407ab51408b011
   manager: conda
   name: libabseil
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/libabseil-20230125.2-cxx17_h59595ed_2.conda
-  version: '20230125.2'
+  url: https://conda.anaconda.org/conda-forge/linux-64/libabseil-20230125.3-cxx17_h59595ed_0.conda
+  version: '20230125.3'
 - category: main
   dependencies:
     libgcc-ng: '>=12'
     libstdcxx-ng: '>=12'
   hash:
     md5: 0f683578378cddb223e7fd24f785ab2a
     sha256: 4df6a29b71264fb25462065e8cddcf5bca60776b1801974af8cbd26b7425fcda
@@ -661,21 +661,21 @@
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/libaec-1.0.6-hcb278e6_1.conda
   version: 1.0.6
 - category: main
   dependencies:
     libgcc-ng: '>=12'
   hash:
-    md5: 9194c9bf9428035a05352d031462eae4
-    sha256: ddc961a36d498aaafd5b71078836ad5dd247cc6ba7924157f3801a2f09b77b14
+    md5: 61641e239f96eae2b8492dc7e755828c
+    sha256: fc57c0876695c5b4ab7173438580c1d7eaa7dccaf14cb6467ca9e0e97abe0cf0
   manager: conda
   name: libbrotlicommon
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/libbrotlicommon-1.0.9-h166bdaf_8.tar.bz2
+  url: https://conda.anaconda.org/conda-forge/linux-64/libbrotlicommon-1.0.9-h166bdaf_9.conda
   version: 1.0.9
 - category: main
   dependencies:
     __glibc: '>=2.17,<3.0.a0'
     cuda-version: '>=12.0,<12.1.0a0'
     libgcc-ng: '>=12'
     libstdcxx-ng: '>=12'
@@ -1279,37 +1279,37 @@
   name: jack
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/jack-1.9.22-h11f4161_0.conda
   version: 1.9.22
 - category: main
   dependencies:
-    libbrotlicommon: 1.0.9 h166bdaf_8
+    libbrotlicommon: 1.0.9 h166bdaf_9
     libgcc-ng: '>=12'
   hash:
-    md5: 4ae4d7795d33e02bd20f6b23d91caf82
-    sha256: d88ba07c3be27c89cb4975cc7edf63ee7b1c62d01f70d5c3f7efeb987c82b052
+    md5: 081aa22f4581c08e4372b0b6c2f8478e
+    sha256: 564f301430c3c61bc5e149e74157ec181ed2a758befc89f7c38466d515a0f614
   manager: conda
   name: libbrotlidec
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/libbrotlidec-1.0.9-h166bdaf_8.tar.bz2
+  url: https://conda.anaconda.org/conda-forge/linux-64/libbrotlidec-1.0.9-h166bdaf_9.conda
   version: 1.0.9
 - category: main
   dependencies:
-    libbrotlicommon: 1.0.9 h166bdaf_8
+    libbrotlicommon: 1.0.9 h166bdaf_9
     libgcc-ng: '>=12'
   hash:
-    md5: 04bac51ba35ea023dc48af73c1c88c25
-    sha256: a0468858b2f647f51509a32040e93512818a8f9980f20b3554cccac747bcc4be
+    md5: 1f0a03af852a9659ed2bf08f2f1704fd
+    sha256: d27bc2562ea3f3b2bfd777f074f1cac6bfa4a737233dad288cd87c4634a9bb3a
   manager: conda
   name: libbrotlienc
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/libbrotlienc-1.0.9-h166bdaf_8.tar.bz2
+  url: https://conda.anaconda.org/conda-forge/linux-64/libbrotlienc-1.0.9-h166bdaf_9.conda
   version: 1.0.9
 - category: main
   dependencies:
     attr: '>=2.5.1,<2.6.0a0'
     libgcc-ng: '>=12'
   hash:
     md5: d05556c80caffff164d17bdea0105a1a
@@ -1362,22 +1362,22 @@
 - category: main
   dependencies:
     gettext: '>=0.21.1,<1.0a0'
     libgcc-ng: '>=12'
     libogg: '>=1.3.4,<1.4.0a0'
     libstdcxx-ng: '>=12'
   hash:
-    md5: 7daf72d8e2a8e848e11d63ed6d1026e0
-    sha256: 095cfa4e2df8622b8f9eebec3c60710ea0f4732c64cd24769ccf9ed63fd45545
+    md5: ee48bf17cc83a00f59ca1494d5646869
+    sha256: 65908b75fa7003167b8a8f0001e11e58ed5b1ef5e98b96ab2ba66d7c1b822c7d
   manager: conda
   name: libflac
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/libflac-1.4.2-h27087fc_0.tar.bz2
-  version: 1.4.2
+  url: https://conda.anaconda.org/conda-forge/linux-64/libflac-1.4.3-h59595ed_0.conda
+  version: 1.4.3
 - category: main
   dependencies:
     gettext: '>=0.21.1,<1.0a0'
     libgcc-ng: '>=12'
     libstdcxx-ng: '>=12'
   hash:
     md5: c2097d0b46367996f09b4e8e4920384a
@@ -1435,22 +1435,22 @@
 - category: main
   dependencies:
     libabseil: '>=20230125.2,<20230126.0a0'
     libgcc-ng: '>=12'
     libstdcxx-ng: '>=12'
     libzlib: '>=1.2.13,<1.3.0a0'
   hash:
-    md5: 40e9b664b20732e651178d0ea29ae2a5
-    sha256: 5f5b16e2e535e6116d0f51f9a15587d76fbe6504e69351ac117a74d666965c01
+    md5: c8da7f04073ed0fabcb60885a4c1a722
+    sha256: b0255d3c46c71e184d0513566a770356abf2cede5e795c4944521c4f7b6a26d4
   manager: conda
   name: libprotobuf
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/libprotobuf-4.23.2-hd1fb520_5.conda
-  version: 4.23.2
+  url: https://conda.anaconda.org/conda-forge/linux-64/libprotobuf-4.23.3-hd1fb520_0.conda
+  version: 4.23.3
 - category: main
   dependencies:
     libgcc-ng: '>=12'
     libzlib: '>=1.2.13,<1.3.0a0'
   hash:
     md5: fdaae20a1cf7cd62130a0973190a31b7
     sha256: 72e958870f49174ebc0ddcd4129e9a9f48de815f20aa3b553f136b514f29bb3a
@@ -1549,21 +1549,21 @@
   version: 4.2.0
 - category: main
   dependencies:
     libgcc-ng: '>=12'
     libstdcxx-ng: '>=12'
     openssl: '>=3.1.1,<4.0a0'
   hash:
-    md5: aa8b86066614c4573f6db62c91978fa9
-    sha256: 4131cd3a3e35050053da45e4f10415a8e4d1acaf169c4f3ad6a2fae9caa53c06
+    md5: b241363e3b72bae6dfbd31e9fecf7d26
+    sha256: 0ec502aaee1b9cb82947a1f56ad599d2ac79c9c25ccf2f44224a69e1e16f537e
   manager: conda
   name: mysql-common
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/mysql-common-8.0.33-hf1915f5_0.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/mysql-common-8.0.33-hf1915f5_1.conda
   version: 8.0.33
 - category: main
   dependencies:
     libffi: '>=3.4.2,<3.5.0a0'
     libgcc-ng: '>=12'
     libtasn1: '>=4.18.0,<5.0a0'
   hash:
@@ -1681,25 +1681,25 @@
   name: zstd
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/zstd-1.5.2-h3eb15da_6.conda
   version: 1.5.2
 - category: main
   dependencies:
-    libbrotlidec: 1.0.9 h166bdaf_8
-    libbrotlienc: 1.0.9 h166bdaf_8
+    libbrotlidec: 1.0.9 h166bdaf_9
+    libbrotlienc: 1.0.9 h166bdaf_9
     libgcc-ng: '>=12'
   hash:
-    md5: e5613f2bc717e9945840ff474419b8e4
-    sha256: ab1994e03bdd88e4b27f9f802ac18e45ed29b92cce25e1fd86da43b89734950f
+    md5: d47dee1856d9cb955b8076eeff304a5b
+    sha256: 1c128f136a59ee2fa47d7fbd9b6fc8afa8460d340e4ae0e6f5419ebbd7539a10
   manager: conda
   name: brotli-bin
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/brotli-bin-1.0.9-h166bdaf_8.tar.bz2
+  url: https://conda.anaconda.org/conda-forge/linux-64/brotli-bin-1.0.9-h166bdaf_9.conda
   version: 1.0.9
 - category: main
   dependencies:
     cuda-libraries: '>=11.8.0'
   hash:
     md5: 3ca379d762f8d7bd727df9e2c9b30664
     sha256: 4ec90f237174c33514a898a363eb9e65edd93df0b571362ac0bda590d7d4ba29
@@ -1816,30 +1816,30 @@
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/libglib-2.76.3-hebfc3b9_0.conda
   version: 2.76.3
 - category: main
   dependencies:
     c-ares: '>=1.19.1,<2.0a0'
-    libabseil: '>=20230125.2,<20230126.0a0'
+    libabseil: '>=20230125.3,<20230126.0a0'
     libgcc-ng: '>=12'
-    libprotobuf: '>=4.23.2,<4.23.3.0a0'
+    libprotobuf: '>=4.23.3,<4.23.4.0a0'
     libstdcxx-ng: '>=12'
     libzlib: '>=1.2.13,<1.3.0a0'
     openssl: '>=3.1.1,<4.0a0'
     re2: '>=2023.3.2,<2023.3.3.0a0'
   hash:
-    md5: 5aed976a1e827d49bec1fb5a9819d032
-    sha256: 055ce98b292ef7dc143e04f38bcd1c265169301835ba8904d9bb9dff0bf7a0b5
+    md5: 6cf9ef21c7ef12df628bf46ad67189d3
+    sha256: f50ab3e6577d1ed3408b5f2a6352fc26bdab3b959dacf0ca93001cf33d35d5f0
   manager: conda
   name: libgrpc
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/libgrpc-1.55.1-h59456c1_1.conda
-  version: 1.55.1
+  url: https://conda.anaconda.org/conda-forge/linux-64/libgrpc-1.56.0-h3905398_2.conda
+  version: 1.56.0
 - category: main
   dependencies:
     libgcc-ng: '>=12'
     libstdcxx-ng: '>=12'
     libxml2: '>=2.10.3,<2.11.0a0'
   hash:
     md5: a3ede1b8e47f993ff1fe3908b23bb307
@@ -1979,25 +1979,25 @@
   url: https://conda.anaconda.org/conda-forge/linux-64/mpc-1.3.1-hfe3b2da_0.conda
   version: 1.3.1
 - category: main
   dependencies:
     libgcc-ng: '>=12'
     libstdcxx-ng: '>=12'
     libzlib: '>=1.2.13,<1.3.0a0'
-    mysql-common: 8.0.33 hf1915f5_0
+    mysql-common: 8.0.33 hf1915f5_1
     openssl: '>=3.1.1,<4.0a0'
     zstd: '>=1.5.2,<1.6.0a0'
   hash:
-    md5: 276339b0115d92c6e0793dcdc7afe308
-    sha256: 44ced085e8ccaef349bbc86f95b34595cf907abe56b6268551fe99b31d2dd007
+    md5: a04ac37f0659929f3ba0f33c7f3d750f
+    sha256: d10f737f835a90d441c5cc0c15e46b4d34594a080f67a1e6cd64ac76bf3e6269
   manager: conda
   name: mysql-libs
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/mysql-libs-8.0.33-hca2cd23_0.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/mysql-libs-8.0.33-hca2cd23_1.conda
   version: 8.0.33
 - category: main
   dependencies:
     __glibc: '>=2.17,<3.0.a0'
     libgcc-ng: '>=12'
     libsqlite: '>=3.40.0,<4.0a0'
     libstdcxx-ng: '>=12'
@@ -2029,32 +2029,32 @@
 - category: main
   dependencies:
     bzip2: '>=1.0.8,<2.0a0'
     ld_impl_linux-64: '>=2.36.1'
     libffi: '>=3.4,<4.0a0'
     libgcc-ng: '>=12'
     libnsl: '>=2.0.0,<2.1.0a0'
-    libsqlite: '>=3.41.2,<4.0a0'
+    libsqlite: '>=3.42.0,<4.0a0'
     libuuid: '>=2.38.1,<3.0a0'
     libzlib: '>=1.2.13,<1.3.0a0'
-    ncurses: '>=6.3,<7.0a0'
-    openssl: '>=3.1.0,<4.0a0'
+    ncurses: '>=6.4,<7.0a0'
+    openssl: '>=3.1.1,<4.0a0'
     readline: '>=8.2,<9.0a0'
     tk: '>=8.6.12,<8.7.0a0'
     tzdata: ''
     xz: '>=5.2.6,<6.0a0'
   hash:
-    md5: 7439c9d24378a82b73a7a53868dacdf1
-    sha256: 6682c75caf3456796fb76313a25475738d85729b43f8c0e904407c0ed8362ede
+    md5: eb6f1df105f37daedd6dca78523baa75
+    sha256: 05e2a7ce916d259f11979634f770f31027d0a5d18463b094e64a30500f900699
   manager: conda
   name: python
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/python-3.10.11-he550d4f_0_cpython.conda
-  version: 3.10.11
+  url: https://conda.anaconda.org/conda-forge/linux-64/python-3.10.12-hd12c33a_0_cpython.conda
+  version: 3.10.12
 - category: main
   dependencies:
     libgcc-ng: '>=12'
     libsqlite: 3.42.0 h2797004_0
     libzlib: '>=1.2.13,<1.3.0a0'
     ncurses: '>=6.3,<7.0a0'
     readline: '>=8.2,<9.0a0'
@@ -2219,39 +2219,39 @@
   name: blinker
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/blinker-1.6.2-pyhd8ed1ab_0.conda
   version: 1.6.2
 - category: main
   dependencies:
-    brotli-bin: 1.0.9 h166bdaf_8
-    libbrotlidec: 1.0.9 h166bdaf_8
-    libbrotlienc: 1.0.9 h166bdaf_8
+    brotli-bin: 1.0.9 h166bdaf_9
+    libbrotlidec: 1.0.9 h166bdaf_9
+    libbrotlienc: 1.0.9 h166bdaf_9
     libgcc-ng: '>=12'
   hash:
-    md5: 2ff08978892a3e8b954397c461f18418
-    sha256: 74c0fa22ea7c62d2c8f7a7aea03a3bd4919f7f3940ef5b027ce0dfb5feb38c06
+    md5: 4601544b4982ba1861fa9b9c607b2c06
+    sha256: 2357d205931912def55df0dc53573361156b27856f9bf359d464da162812ec1f
   manager: conda
   name: brotli
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/brotli-1.0.9-h166bdaf_8.tar.bz2
+  url: https://conda.anaconda.org/conda-forge/linux-64/brotli-1.0.9-h166bdaf_9.conda
   version: 1.0.9
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
-    md5: fd006afc4115740d8d52887ee813f262
-    sha256: d17f6b5ae744e64a337c9dbad21b8d501916eaf0e55564dc81c78c492783d73a
+    md5: 60b5eb16d9a7a5482ba37f67aa49db5b
+    sha256: 8d30a41a88900730c748f5b296730a0d48e5cfa2c8b260aab60fa9f26ffafcc0
   manager: conda
   name: cachetools
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/cachetools-5.3.0-pyhd8ed1ab_0.conda
-  version: 5.3.0
+  url: https://conda.anaconda.org/conda-forge/noarch/cachetools-5.3.1-pyhd8ed1ab_0.conda
+  version: 5.3.1
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
     md5: 5d1b71c942b8421285934dad1d891ebc
     sha256: f839a6e04d94069f90dd85337ea9108f058dc76771bb469a413f32bb1ba0b256
   manager: conda
@@ -2399,22 +2399,22 @@
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2
   version: '0.4'
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
-    md5: 7312299d7a0ea4993159229b7d2dceb2
-    sha256: f073c3ba993912f1c0027bc34a54975642885f0a4cd5f9dc42a17ca945df2c18
+    md5: de4cb3384374e1411f0454edcf546cdb
+    sha256: 7b23ea0169fa6e7c3a0867d96d9eacd312759f83e5d83ad0fcc93e85379c16ae
   manager: conda
   name: exceptiongroup
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda
-  version: 1.1.1
+  url: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda
+  version: 1.1.2
 - category: main
   dependencies:
     python: '>=2.7'
   hash:
     md5: 4c1bc140e2be5c8ba6e3acab99e25c50
     sha256: 9c03425cd58c474af20e179c9ba121a82984d6c4bfc896bbc992f5ed75dd7539
   manager: conda
@@ -2553,28 +2553,28 @@
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/greenlet-2.0.2-py310hc6cd4ac_1.conda
   version: 2.0.2
 - category: main
   dependencies:
     libgcc-ng: '>=12'
-    libgrpc: 1.55.1 h59456c1_1
+    libgrpc: 1.56.0 h3905398_2
     libstdcxx-ng: '>=12'
     libzlib: '>=1.2.13,<1.3.0a0'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
   hash:
-    md5: 5292eea84c56fccfebcd51bb0d81eff5
-    sha256: 147620fbc64cdc71023b594addc5d57ed7928c3b2caa4506e8aa61e49d285c25
+    md5: 78282ea7b261ed53a615faba16532e82
+    sha256: ecd0f91a9cf71fb9bd4790b9ddc7028e519dd36291afd5c2a763e9cfaf60dcb0
   manager: conda
   name: grpcio
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/grpcio-1.55.1-py310h1b8f574_1.conda
-  version: 1.55.1
+  url: https://conda.anaconda.org/conda-forge/linux-64/grpcio-1.56.0-py310h1b8f574_2.conda
+  version: 1.56.0
 - category: main
   dependencies:
     libgcc-ng: '>=12'
     libglib: '>=2.76.3,<3.0a0'
     libstdcxx-ng: '>=12'
   hash:
     md5: 4d8df0b0db060d33c9a702ada998a8fe
@@ -2645,22 +2645,22 @@
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/jmespath-1.0.1-pyhd8ed1ab_0.tar.bz2
   version: 1.0.1
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
-    md5: 0c0a54e16b764bafcae35913cc9d60ff
-    sha256: 13ffd45adc630670469860932b4c046a46248b9b96d5c8fa8b3a95cdd0618f78
+    md5: 2bc3ca2f7387af385dd06706b4fb2d35
+    sha256: 0781ed7a4f35ff1309e95381c40c8d8f96263ca4260a72baaafda87c975a972a
   manager: conda
   name: jupyterlab_widgets
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.7-pyhd8ed1ab_1.conda
-  version: 3.0.7
+  url: https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.8-pyhd8ed1ab_0.conda
+  version: 3.0.8
 - category: main
   dependencies:
     libgcc-ng: '>=12'
     libstdcxx-ng: '>=12'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
   hash:
@@ -3023,22 +3023,22 @@
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2
   version: 1.3.10
 - category: main
   dependencies:
     python: '>=3.8'
   hash:
-    md5: 7d301a0d25f424d96175f810935f0da9
-    sha256: c25e1757e4e90638bb1e778aba3ee5f3c01fae9752e3c3929f9be7d367f6c7f3
+    md5: 7263924c642d22e311d9e59b839f1b33
+    sha256: ff1f70e0bd50693be7e2bad0efb2539f5dcc5ec4d638e787e703f28098e72de4
   manager: conda
   name: pluggy
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.0.0-pyhd8ed1ab_5.tar.bz2
-  version: 1.0.0
+  url: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.2.0-pyhd8ed1ab_0.conda
+  version: 1.2.0
 - category: main
   dependencies:
     python: ''
   hash:
     md5: 7205635cd71531943440fbfe3b6b5727
     sha256: 2cd6fae8f9cbc806b7f828f006ae4a83c23fac917cacfd73c37ce322d4324e53
   manager: conda
@@ -3549,22 +3549,22 @@
   version: 5.9.0
 - category: main
   dependencies:
     libgcc-ng: '>=12'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
   hash:
-    md5: 309cb97f0a3a11a6481453c16e8c5be1
-    sha256: 8fcb2141ae2d3b5d198791118bf8fd2a5382e70596647983746fcaff5a93beed
+    md5: 48d1b46a82b8b4fb6057711dd213977f
+    sha256: 1c5fe69f7729a7cde3cf5c1d96ea5c56c3c07209bb48c6d8247e2fa279ba01ca
   manager: conda
   name: typed-ast
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/typed-ast-1.5.4-py310h5764c6d_1.tar.bz2
-  version: 1.5.4
+  url: https://conda.anaconda.org/conda-forge/linux-64/typed-ast-1.5.5-py310h2372a71_0.conda
+  version: 1.5.5
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
     md5: 4a3014a4d107d15475d106b751c4e352
     sha256: 90a8d56c8015af1575d504d5f77d95a806cd999fc178a06ab51a349f1f744672
   manager: conda
@@ -3635,22 +3635,22 @@
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2
   version: 0.5.1
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
-    md5: 1dd6387a73d84e16b6f73de676bb4c36
-    sha256: 713075726a3e1db115dfeb48c448e72a8eb7c378af3e2598094a021bc21ce0fd
+    md5: c34d9325a609381a0b0e8a5b4f325147
+    sha256: c71cb65ac49692adb33735f3114b99a96c0c5140db1d56cf4ccef4fe92ea9a4c
   manager: conda
   name: websocket-client
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.0-pyhd8ed1ab_0.conda
-  version: 1.6.0
+  url: https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda
+  version: 1.6.1
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
     md5: 49bb0d9e60ce1db25e151780331bb5f3
     sha256: 79b4d29b0c004014a2abd5fc2c9fcd35cc6256222b960c2a317a27c4b0d8884d
   manager: conda
@@ -3659,22 +3659,22 @@
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda
   version: 0.40.0
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
-    md5: bcc54b91a8ce88f60f538b87b409909e
-    sha256: c63d6e1a51593895dec44931fb2396cfb80e8454d3c7062311a6194032c9b47e
+    md5: 2e9ebddf0b93d0fb203d0906b8052c4f
+    sha256: a73d34f8169e206bccfb356c093ff5ced803b953bbcc1480ed27976f97598d68
   manager: conda
   name: widgetsnbextension
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda
-  version: 4.0.7
+  url: https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.8-pyhd8ed1ab_0.conda
+  version: 4.0.8
 - category: main
   dependencies:
     libgcc-ng: '>=12'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
   hash:
     md5: cbfdcc9c243ac7f080cf60833b482f97
@@ -3840,22 +3840,22 @@
   version: 2.12.1
 - category: main
   dependencies:
     backports: ''
     python: '>=3.6'
     setuptools: ''
   hash:
-    md5: c5b3edc62d6309088f4970b3eaaa65a6
-    sha256: fdea00d4b79990f3fe938e2716bc32bd895eb5c44b6c75b8261db095a1b33c16
+    md5: 6b1b907661838a75d067a22f87996b2e
+    sha256: 7027bb689dd4ca4a08e3b25805de9d04239be6b31125993558f21f102a9d2700
   manager: conda
   name: backports.functools_lru_cache
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.4-pyhd8ed1ab_0.tar.bz2
-  version: 1.6.4
+  url: https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda
+  version: 1.6.5
 - category: main
   dependencies:
     python: '>=3.6'
     soupsieve: '>=1.2'
   hash:
     md5: a362ff7d976217f8fa78c0f1c4f59717
     sha256: 52d3e6bcd442537e22699cd227d8fdcfd54b708eeb8ee5b4c671a6a9b9cd74da
@@ -4202,22 +4202,22 @@
   version: 2.18.0
 - category: main
   dependencies:
     packaging: '>=17.1'
     python: '>=3.8'
     typing_extensions: ''
   hash:
-    md5: ad16f58b64d3b41f4cbb75040b06c9cc
-    sha256: 8c1fff22ab86c85768e65dc8c4f4664787476a21f4d934c4e0261a1fa7523f9c
+    md5: c71f7ec8b80a536e58b979299b230251
+    sha256: 9c866f31ff7a02cc70b306f65b1a81eabf84826b0d32c1f51e0ece17cfcdaf79
   manager: conda
   name: lightning-utilities
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/lightning-utilities-0.8.0-pyhd8ed1ab_0.conda
-  version: 0.8.0
+  url: https://conda.anaconda.org/conda-forge/noarch/lightning-utilities-0.9.0-pyhd8ed1ab_0.conda
+  version: 0.9.0
 - category: main
   dependencies:
     python: '>=3.6'
     uc-micro-py: '>=1.0.1,<2.0.0'
   hash:
     md5: 25b93e66067eb496ac10da888e25cc33
     sha256: 0980092a2e0a4bd263c18fb0db701589fc10fc8542ce511f844a533490d5f14e
@@ -4346,30 +4346,30 @@
   name: proj
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/proj-9.1.0-h93bde94_0.tar.bz2
   version: 9.1.0
 - category: main
   dependencies:
-    libabseil: '>=20230125.2,<20230126.0a0'
+    libabseil: '>=20230125.3,<20230126.0a0'
     libgcc-ng: '>=12'
-    libprotobuf: '>=4.23.2,<4.23.3.0a0'
+    libprotobuf: '>=4.23.3,<4.23.4.0a0'
     libstdcxx-ng: '>=12'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     setuptools: ''
   hash:
-    md5: 20feaa8fb200e45f93746836ad96997e
-    sha256: f4ab978a01d7339f52c2cf281200c3971d3737395300244c5347f847e9a7fd92
+    md5: 27ce7010f8821add3b955ec88f663bb6
+    sha256: b92f2c7728f1625003a247721af5b22c8100a92714596ce8158a07790221c40e
   manager: conda
   name: protobuf
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/protobuf-4.23.2-py310hb875b13_1.conda
-  version: 4.23.2
+  url: https://conda.anaconda.org/conda-forge/linux-64/protobuf-4.23.3-py310hb875b13_0.conda
+  version: 4.23.3
 - category: main
   dependencies:
     dbus: '>=1.13.6,<2.0a0'
     libgcc-ng: '>=12'
     libglib: '>=2.74.1,<3.0a0'
     libsndfile: '>=1.2.0,<1.3.0a0'
     libsystemd0: '>=253'
@@ -4912,22 +4912,22 @@
   url: https://conda.anaconda.org/conda-forge/linux-64/mkl-devel-2022.1.0-ha770c72_916.tar.bz2
   version: 2022.1.0
 - category: main
   dependencies:
     python: '>=3.7'
     typing-extensions: '>=4.6.3'
   hash:
-    md5: 741384b21c1b512617f4ee4ea8457c5d
-    sha256: ba254f8e7bc01586779c40d040ee000627cddc57965ccbcdb155936c534520d6
+    md5: 3e4aca765371893ad848397794600632
+    sha256: 5f382d0d3509784152506e0e022bb5a30d254555e809804491207196f890af67
   manager: conda
   name: platformdirs
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.6.0-pyhd8ed1ab_0.conda
-  version: 3.6.0
+  url: https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.8.0-pyhd8ed1ab_0.conda
+  version: 3.8.0
 - category: main
   dependencies:
     alsa-lib: '>=1.2.8,<1.2.9.0a0'
     dbus: '>=1.13.6,<2.0a0'
     fftw: '>=3.3.10,<4.0a0'
     gstreamer-orc: '>=0.4.33,<0.5.0a0'
     jack: '>=1.9.22,<1.10.0a0'
@@ -5020,22 +5020,22 @@
   dependencies:
     greenlet: '!=0.4.17'
     libgcc-ng: '>=12'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     typing-extensions: '>=4.2.0'
   hash:
-    md5: 61d5ef9e6989a9235a2b449df5ad6df1
-    sha256: b3c90441346666bc0e044b904a012f6ef415037bccd76467be3eb54a3afb14ff
+    md5: 5addfcf598875b2e4febacbc98aa2d29
+    sha256: 146012656f7ecc7e56871407f3509a2e8c050054bced89428d702ec6adad18bd
   manager: conda
   name: sqlalchemy
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/sqlalchemy-2.0.16-py310h2372a71_0.conda
-  version: 2.0.16
+  url: https://conda.anaconda.org/conda-forge/linux-64/sqlalchemy-2.0.17-py310h2372a71_0.conda
+  version: 2.0.17
 - category: main
   dependencies:
     asttokens: ''
     executing: ''
     pure_eval: ''
     python: '>=3.5'
   hash:
@@ -5231,22 +5231,22 @@
   url: https://conda.anaconda.org/conda-forge/linux-64/pango-1.50.14-hd33c08f_0.conda
   version: 1.50.14
 - category: main
   dependencies:
     python: '>=3.7'
     wcwidth: ''
   hash:
-    md5: 59ba1bf8ea558751a0d391249a248765
-    sha256: 78c2f3c6195ec350d7d6e5fa3e43274ca8191c181c97a867e2920faaeec0e9bc
+    md5: a4986c6bb5b0d05a38855b0880a5f425
+    sha256: 10e7fdc75d4b85633be6b12a70b857053987127a808caa0f88b2cba4b3ce6359
   manager: conda
   name: prompt-toolkit
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda
-  version: 3.0.38
+  url: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda
+  version: 3.0.39
 - category: main
   dependencies:
     libgcc-ng: '>=12'
     pulseaudio-client: 16.1 h5195f5e_3
     pulseaudio-daemon: 16.1 ha8d29e2_3
   hash:
     md5: 8b452ab959166d91949af4c2d28f81db
@@ -5342,22 +5342,22 @@
     jupyter_core: '>=4.12,!=5.0.*'
     python: '>=3.8'
     python-dateutil: '>=2.8.2'
     pyzmq: '>=23.0'
     tornado: '>=6.2'
     traitlets: '>=5.3'
   hash:
-    md5: 58ca2d50c3b27b86fd7df62eaadbf9a9
-    sha256: c36c0e9da3a23e89fc30333760f9c9fdb1a14ca2862fa1e1257f7fe4d508fded
+    md5: 1d018ee4ab13217e2544f795eb0a6798
+    sha256: 7dc74a032daefbdcf4d6d661616dfdc8649e5cf9db58258afe91cc09ea0cf402
   manager: conda
   name: jupyter_client
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.2.0-pyhd8ed1ab_0.conda
-  version: 8.2.0
+  url: https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda
+  version: 8.3.0
 - category: main
   dependencies:
     libblas: 3.9.0 16_linux64_mkl
     libcblas: 3.9.0 16_linux64_mkl
     liblapack: 3.9.0 16_linux64_mkl
   hash:
     md5: 44ccc4d4dca6a8d57fa17442bc64b5a1
@@ -5418,24 +5418,24 @@
   name: numpy
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/numpy-1.25.0-py310ha4c1d20_0.conda
   version: 1.25.0
 - category: main
   dependencies:
-    prompt-toolkit: '>=3.0.38,<3.0.39.0a0'
+    prompt-toolkit: '>=3.0.39,<3.0.40.0a0'
   hash:
-    md5: 45b74f64d8808eda7e6f6e6b1d641fd2
-    sha256: c0f24a75d27918eb33f86902aa6024783d128a89eb3a169bcb22f24163a422b3
+    md5: 4bbbe67d5df19db30f04b8e344dc9976
+    sha256: 89f7fecc7355181dbc2ab851e668a2fce6aa4830b336a34c93b59bda93206270
   manager: conda
   name: prompt_toolkit
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda
-  version: 3.0.38
+  url: https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.39-hd8ed1ab_0.conda
+  version: 3.0.39
 - category: main
   dependencies:
     __glibc: '>=2.17,<3.0.a0'
     alsa-lib: '>=1.2.8,<1.2.9.0a0'
     dbus: '>=1.13.6,<2.0a0'
     expat: '>=2.5.0,<3.0a0'
     fontconfig: '>=2.14.2,<3.0a0'
@@ -5500,22 +5500,22 @@
   url: https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.15-pyhd8ed1ab_0.conda
   version: 1.26.15
 - category: main
   dependencies:
     aiohttp: <4
     python: '>=3.6'
   hash:
-    md5: 70f4b52c0e703936aa1812d8b14a5bb2
-    sha256: 11dd5e6c5062e788160167e2a64fcbbb2c7ec825e28d628a9e7771172e039de7
+    md5: 0d0113b67472cea3da288838ebc80acb
+    sha256: 656947c8457d5ac06f11dc1da904ac7ac8ac8edf81323ee9794a3d51ace79ff3
   manager: conda
   name: wslink
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/wslink-1.11.0-pyhd8ed1ab_0.conda
-  version: 1.11.0
+  url: https://conda.anaconda.org/conda-forge/noarch/wslink-1.11.1-pyhd8ed1ab_0.conda
+  version: 1.11.1
 - category: main
   dependencies:
     libblas: 3.9.0 16_linux64_mkl
     libcblas: 3.9.0 16_linux64_mkl
     liblapack: 3.9.0 16_linux64_mkl
     liblapacke: 3.9.0 16_linux64_mkl
     mkl: '>=2022.1.0,<2023.0a0'
@@ -5532,22 +5532,22 @@
 - category: main
   dependencies:
     jmespath: '>=0.7.1,<2.0.0'
     python: '>=3.7'
     python-dateutil: '>=2.1,<3.0.0'
     urllib3: '>=1.25.4,<1.27'
   hash:
-    md5: ccfde1c6ce8dbb4af5590c88a0482248
-    sha256: b818c4a738c58fcc1ca231f75bfbfdd516b44e437a460336bdbee70a9a4573ca
+    md5: 0f30016ea54215fdb883b8978340c9b7
+    sha256: ccbd3413915259825a678707b438e7ba25712d9c8c5748d2d82f24359237b3f9
   manager: conda
   name: botocore
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/botocore-1.29.158-pyhd8ed1ab_0.conda
-  version: 1.29.158
+  url: https://conda.anaconda.org/conda-forge/noarch/botocore-1.29.165-pyhd8ed1ab_0.conda
+  version: 1.29.165
 - category: main
   dependencies:
     libgcc-ng: '>=12'
     libstdcxx-ng: '>=12'
     numpy: '>=1.16'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
@@ -5759,22 +5759,22 @@
     python: '>=3.6'
     pyu2f: '>=0.1.5'
     requests: '>=2.20.0,<3.0.0dev'
     rsa: '>=3.1.4,<5'
     six: '>=1.9.0'
     urllib3: <2.0
   hash:
-    md5: 59f942ef9326d2519a7c953f1c24d5da
-    sha256: ba9136edf49c8aa53f45ddfe0c16387bf375f1e5e27f50e39cc1e41c6f5ad25d
+    md5: 8c5dd8609d314721d990c1d1fd607f81
+    sha256: 6b097ca9b31961d6a983f81dc295012e9c99c4c1a5a83a93ab2fcc6528af428f
   manager: conda
   name: google-auth
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/google-auth-2.20.0-pyh1a96a4e_0.conda
-  version: 2.20.0
+  url: https://conda.anaconda.org/conda-forge/noarch/google-auth-2.21.0-pyh1a96a4e_0.conda
+  version: 2.21.0
 - category: main
   dependencies:
     __linux: ''
     comm: '>=0.1.1'
     debugpy: '>=1.6.5'
     ipython: '>=7.23.1'
     jupyter_client: '>=6.1.12'
@@ -5784,22 +5784,22 @@
     packaging: ''
     psutil: ''
     python: '>=3.8'
     pyzmq: '>=20'
     tornado: '>=6.1'
     traitlets: '>=5.4.0'
   hash:
-    md5: c76d274e313a06f23de594848e12a75c
-    sha256: 53d002980c25f74399f11f750df89ad8f876a785605ab1c8198893713c5427a5
+    md5: 482f0176a89f14e10a7d15f9f1980e36
+    sha256: 324bf8a374472ac15d4663b97c36852c59872d59aa6c4962bda6a82674061804
   manager: conda
   name: ipykernel
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.2-pyh210e3f2_0.conda
-  version: 6.23.2
+  url: https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.3-pyh71e2992_0.conda
+  version: 6.23.3
 - category: main
   dependencies:
     attrs: ''
     click: ''
     importlib-metadata: ''
     nbclient: '>=0.2,<0.8'
     nbformat: ''
@@ -5940,59 +5940,59 @@
   name: sphinx
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/sphinx-4.5.0-pyh6c4a22f_0.tar.bz2
   version: 4.5.0
 - category: main
   dependencies:
-    botocore: '>=1.29.158,<1.30.0'
+    botocore: '>=1.29.165,<1.30.0'
     jmespath: '>=0.7.1,<2.0.0'
     python: '>=3.7'
     s3transfer: '>=0.6.0,<0.7.0'
   hash:
-    md5: 2e39307a3987518e49eb30ca51e3cfb5
-    sha256: b22c2838e528d03d670f1ecbc57f3d57b4a93d21f456b1248788d7be4e080e3a
+    md5: b9a6316db67d5f2c8dbac2aeb24c6803
+    sha256: 4ca4d8c481609dbf8ce755a8f115486e40be0f0d01c0961c696d6f995dadb2f5
   manager: conda
   name: boto3
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/boto3-1.26.158-pyhd8ed1ab_0.conda
-  version: 1.26.158
+  url: https://conda.anaconda.org/conda-forge/noarch/boto3-1.26.165-pyhd8ed1ab_0.conda
+  version: 1.26.165
 - category: main
   dependencies:
     click: '>=6.0.0'
-    google-auth: '>=1.0.0'
+    google-auth: '>=2.15.0'
     python: '>=3.6'
     requests-oauthlib: '>=0.7.0'
   hash:
-    md5: 5ba9d95acb9add67f468ecdee6595c0f
-    sha256: ef8edcbc8efe616d0f3686607f445a6a96f3549ce2faed1797ad35ca5cd42e81
+    md5: 569e62e95b01b53e4ec7d9abe83b7385
+    sha256: f89613643658a51a1ac0fb7c7950526fadc2a6ce1ae13755d786e14cfce1633c
   manager: conda
   name: google-auth-oauthlib
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/google-auth-oauthlib-1.0.0-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/google-auth-oauthlib-1.0.0-pyhd8ed1ab_1.conda
   version: 1.0.0
 - category: main
   dependencies:
     ipykernel: '>=4.5.1'
     ipython: '>=6.1.0'
-    jupyterlab_widgets: '>=3.0.7,<4.1.dev0'
+    jupyterlab_widgets: '>=3.0.7,<3.1.0'
     python: '>=3.7'
     traitlets: '>=4.3.1'
-    widgetsnbextension: '>=4.0.7,<4.1.dev0'
+    widgetsnbextension: '>=4.0.7,<4.1.0'
   hash:
-    md5: 68627a08556e4a273e4c7bfc84251457
-    sha256: a18f168f368cc8ba4d11a83bf57fcd664bd311a0fcc9b36c283715470f43c133
+    md5: 4b0f4e8fe2a303e472674eae0340bdad
+    sha256: 3b17ad90294f0684fca9191f1e696e9b4f03a652d5e588b6ff0feb5647fcf116
   manager: conda
   name: ipywidgets
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.6-pyhd8ed1ab_0.conda
-  version: 8.0.6
+  url: https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.7-pyhd8ed1ab_0.conda
+  version: 8.0.7
 - category: main
   dependencies:
     ipykernel: '>=6.14'
     ipython: ''
     jupyter_client: '>=7.0.0'
     jupyter_core: '>=4.12,!=5.0.*'
     prompt_toolkit: '>=3.0.30'
@@ -6027,22 +6027,22 @@
     pyzmq: '>=24'
     send2trash: ''
     terminado: '>=0.8.3'
     tornado: '>=6.2.0'
     traitlets: '>=5.6.0'
     websocket-client: ''
   hash:
-    md5: 39fd52b0fcb2fb52bac47a1419bf09bd
-    sha256: 0f0feb284f667964d1e4122a7690f6e3ace257732591a6151fdd1eb797911128
+    md5: 7488cd1f4d35a2af96faa765b7e5b2f0
+    sha256: 132bfa3eef62231e53b59d93358f818a97c5e7939670bfdd821b7146a0094e43
   manager: conda
   name: jupyter_server
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.6.0-pyhd8ed1ab_0.conda
-  version: 2.6.0
+  url: https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.7.0-pyhd8ed1ab_0.conda
+  version: 2.7.0
 - category: main
   dependencies:
     matplotlib-base: '>=3.7.1,<3.7.2.0a0'
     pyqt: '>=5.10'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     tornado: '>=5'
@@ -6633,34 +6633,55 @@
   name: torchtriton
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/pytorch/linux-64/torchtriton-2.0.0-py310.tar.bz2
   version: 2.0.0
 - category: main
   dependencies:
+    ffmpeg: '>=4.2'
+    jpeg: ''
+    libpng: ''
+    numpy: '>=1.11'
+    pillow: '>=5.3.0,!=8.3.*'
+    python: '>=3.10,<3.11.0a0'
+    pytorch: 2.0.1
+    pytorch-cuda: 11.8.*
+    pytorch-mutex: 1.0 cuda
+    requests: ''
+  hash:
+    md5: b38f7082cde2a86ca981194e9ef51028
+    sha256: a00cadd783b30355d847a6aaa3452c4f5da6638a15933c322c20a652ee731a24
+  manager: conda
+  name: torchvision
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/pytorch/linux-64/torchvision-0.15.2-py310_cu118.tar.bz2
+  version: 0.15.2
+- category: main
+  dependencies:
     fsspec: '>2021.06.0'
     lightning-utilities: '>=0.7.0'
     numpy: '>=1.17.2'
     packaging: '>=17.1'
     python: '>=3.8'
     pytorch: '>=1.11.0'
     pyyaml: '>=5.4'
     requests: ''
     torchmetrics: '>=0.7.0'
     tqdm: '>=4.57.0'
     typing_extensions: '>=4.0.0'
   hash:
-    md5: 97138eb8783fa54884216a6562413736
-    sha256: d2b5fbd636393c71dfc07ce5a15eb36285b01aaa34453b3fd8b9b26f0fa5b689
+    md5: ce9d626b181c6f8cceb5047f6a819f7d
+    sha256: a049296b4b33bceedf3bafd378e8a4112bca71b453734f1e0daaca2a72598593
   manager: conda
   name: pytorch-lightning
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pytorch-lightning-2.0.3-pyhd8ed1ab_0.conda
-  version: 2.0.3
+  url: https://conda.anaconda.org/conda-forge/noarch/pytorch-lightning-2.0.4-pyhd8ed1ab_0.conda
+  version: 2.0.4
 - category: main
   dependencies: {}
   hash:
     md5: 37edc4e6304ca87316e160f5ca0bd1b5
     sha256: 60ba4c64f5d0afca0d283c7addba577d3e2efc0db86002808dadb0498661b2f2
   manager: conda
   name: bzip2
@@ -6777,21 +6798,21 @@
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/lame-3.100-hb7f2c08_1003.tar.bz2
   version: '3.100'
 - category: main
   dependencies: {}
   hash:
-    md5: 37157d273eaf3bc7d6862104161d9ec9
-    sha256: c983101653f5bffea605c4423d84fd5ca28ee36b290cdb6207ec246e293f7d94
+    md5: ee1ee8c79c3426229ad03290573be552
+    sha256: 1718e037a7ea9a1730b9f5285898528676794e2aaf5590149d239febab9a9b36
   manager: conda
   name: libbrotlicommon
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/libbrotlicommon-1.0.9-hb7f2c08_8.tar.bz2
+  url: https://conda.anaconda.org/conda-forge/osx-64/libbrotlicommon-1.0.9-hb7f2c08_9.conda
   version: 1.0.9
 - category: main
   dependencies: {}
   hash:
     md5: 7d6972792161077908b62971802f289a
     sha256: 9063271847cf05f3a6cc6cae3e7f0ced032ab5f3a3c9d3f943f876f39c5c2549
   manager: conda
@@ -7255,57 +7276,57 @@
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/lerc-4.0.0-hb486fe8_0.tar.bz2
   version: 4.0.0
 - category: main
   dependencies:
     libcxx: '>=15.0.7'
   hash:
-    md5: 52adda30d725e5afd2b4a25331818bdc
-    sha256: a245267505766ad336022d9d3bd7a0cea967615ba888bc7e59850e2316be5165
+    md5: 1d883cd421a0b0af624c38fa8d043f98
+    sha256: 915e61c37e1b57a296bf075c7b7ccf3f08f7cb2e873edf69e3c1b39e895dc61e
   manager: conda
   name: libabseil
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/libabseil-20230125.2-cxx17_h000cb23_2.conda
-  version: '20230125.2'
+  url: https://conda.anaconda.org/conda-forge/osx-64/libabseil-20230125.3-cxx17_h000cb23_0.conda
+  version: '20230125.3'
 - category: main
   dependencies:
     libcxx: '>=14.0.6'
   hash:
     md5: 7c0f82f435ab4c48d65dc9b28db2ad9e
     sha256: 38d32f4c7efddc204e53f43cd910122d3e6a997de1a3cd15f263217b225a9cdf
   manager: conda
   name: libaec
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/libaec-1.0.6-hf0c8a7f_1.conda
   version: 1.0.6
 - category: main
   dependencies:
-    libbrotlicommon: 1.0.9 hb7f2c08_8
+    libbrotlicommon: 1.0.9 hb7f2c08_9
   hash:
-    md5: 7f952a036d9014b4dab96c6ea0f8c2a7
-    sha256: 52d8e8929b2476cf13fd397d88cefd911f805de00e77090fdc50b8fb11c372ca
+    md5: 4043ef9fe42e178785e0e1853b79bdf9
+    sha256: 3892d88f778ddcda5c2bb7d066082fc7b785dcc84ffe448c65f21cbadd856e2c
   manager: conda
   name: libbrotlidec
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/libbrotlidec-1.0.9-hb7f2c08_8.tar.bz2
+  url: https://conda.anaconda.org/conda-forge/osx-64/libbrotlidec-1.0.9-hb7f2c08_9.conda
   version: 1.0.9
 - category: main
   dependencies:
-    libbrotlicommon: 1.0.9 hb7f2c08_8
+    libbrotlicommon: 1.0.9 hb7f2c08_9
   hash:
-    md5: b36a3bfe866d9127f25f286506982166
-    sha256: be7e794c6208e7e12982872922df13fbf020ab594d516b7bc306a384ac7d3ac6
+    md5: b64d4dcc70aa141db7fccbf13bad81e1
+    sha256: c099c964277ee7ea98cf6ba1bfe07078e662b86ed999da3fcf9eaf7d7d242e86
   manager: conda
   name: libbrotlienc
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/libbrotlienc-1.0.9-hb7f2c08_8.tar.bz2
+  url: https://conda.anaconda.org/conda-forge/osx-64/libbrotlienc-1.0.9-hb7f2c08_9.conda
   version: 1.0.9
 - category: main
   dependencies:
     ncurses: '>=6.2,<7.0.0a0'
   hash:
     md5: 6016a8a1d0e63cac3de2c352cd40208b
     sha256: dbd3c3f2eca1d21c52e4c03b21930bbce414c4592f8ce805801575b9e9256095
@@ -7609,24 +7630,24 @@
   name: zstd
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/zstd-1.5.2-hbc0c0cd_6.conda
   version: 1.5.2
 - category: main
   dependencies:
-    libbrotlidec: 1.0.9 hb7f2c08_8
-    libbrotlienc: 1.0.9 hb7f2c08_8
+    libbrotlidec: 1.0.9 hb7f2c08_9
+    libbrotlienc: 1.0.9 hb7f2c08_9
   hash:
-    md5: aac5ad0d8f747ef7f871508146df75d9
-    sha256: 36f79eb26da032c5d1ddc11e0bcac5526f249bf60d332e4743c8d48bb7334db0
+    md5: 72c526f7ffa265473e6c75fd90605e52
+    sha256: 98c257aee9b60dc91a86fc486b19192eebfe9ec7929b4efff99b6fb643f85b05
   manager: conda
   name: brotli-bin
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/brotli-bin-1.0.9-hb7f2c08_8.tar.bz2
+  url: https://conda.anaconda.org/conda-forge/osx-64/brotli-bin-1.0.9-hb7f2c08_9.conda
   version: 1.0.9
 - category: main
   dependencies:
     fonts-conda-forge: ''
   hash:
     md5: fee5683a3f04bd15cbd8318b096a27ab
     sha256: a997f2f1921bb9c9d76e6fa2f6b408b7fa549edd349a77639c9fe7a23ea93e61
@@ -7764,22 +7785,22 @@
   version: 1.52.0
 - category: main
   dependencies:
     libabseil: '>=20230125.2,<20230126.0a0'
     libcxx: '>=15.0.7'
     libzlib: '>=1.2.13,<1.3.0a0'
   hash:
-    md5: ae92f79c6d9af43468d4109fe76b37b8
-    sha256: 956377fb504e6adff842f42bb5b1ecfee39862b1407897f91cadbb1f01bf5d1f
+    md5: b9e780ed0d0a365ff10b8e83c64471ce
+    sha256: c46a032cffd7db2becfae7305a2e7c5568f3a6ce5a70c6c4092c87f837a4c9e5
   manager: conda
   name: libprotobuf
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/libprotobuf-4.23.2-h5feb325_5.conda
-  version: 4.23.2
+  url: https://conda.anaconda.org/conda-forge/osx-64/libprotobuf-4.23.3-h5feb325_0.conda
+  version: 4.23.3
 - category: main
   dependencies:
     libzlib: '>=1.2.13,<1.3.0a0'
     openssl: '>=3.1.1,<4.0a0'
   hash:
     md5: ca3a72efba692c59a90d4b9fc0dfe774
     sha256: f3886763b88f4b24265db6036535ef77b7b77ce91b1cbe588c0fbdd861eec515
@@ -7878,21 +7899,21 @@
   url: https://conda.anaconda.org/conda-forge/osx-64/mpfr-4.2.0-h4f9bd69_0.conda
   version: 4.2.0
 - category: main
   dependencies:
     libcxx: '>=15.0.7'
     openssl: '>=3.1.1,<4.0a0'
   hash:
-    md5: a4cd3c3df486b393d71ad75dd8d7c11f
-    sha256: b5c5c3e4a4b3b5f11e3711c34d007c05e99bfbf9329f5ec3a2dcafab2a85cbb4
+    md5: bfbfd93ef846f67d53f40bcf28b91621
+    sha256: 72cc42ab185b275c888d15d06b28e4d81e48c32af782188aea37020c4329452c
   manager: conda
   name: mysql-common
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/mysql-common-8.0.33-hc6116ba_0.conda
+  url: https://conda.anaconda.org/conda-forge/osx-64/mysql-common-8.0.33-hc6116ba_1.conda
   version: 8.0.33
 - category: main
   dependencies:
     libcxx: '>=14.0.6'
     libsqlite: '>=3.40.0,<4.0a0'
     libzlib: '>=1.2.13,<1.3.0a0'
     nspr: '>=4.35,<5.0a0'
@@ -7905,31 +7926,31 @@
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/nss-3.89-h78b00b3_0.conda
   version: '3.89'
 - category: main
   dependencies:
     bzip2: '>=1.0.8,<2.0a0'
     libffi: '>=3.4,<4.0a0'
-    libsqlite: '>=3.41.2,<4.0a0'
+    libsqlite: '>=3.42.0,<4.0a0'
     libzlib: '>=1.2.13,<1.3.0a0'
-    ncurses: '>=6.3,<7.0a0'
-    openssl: '>=3.1.0,<4.0a0'
+    ncurses: '>=6.4,<7.0a0'
+    openssl: '>=3.1.1,<4.0a0'
     readline: '>=8.2,<9.0a0'
     tk: '>=8.6.12,<8.7.0a0'
     tzdata: ''
     xz: '>=5.2.6,<6.0a0'
   hash:
-    md5: ec1a9528837c5fcd34f387e317b30f1e
-    sha256: 6e5ed21b0d491e791cbdf0f1361d306173dcd0f25b65b5d2881d12a500d2e128
+    md5: 351b8aa0687f3510620cf06ad11229f4
+    sha256: cbf1b9cf9bdba639675a1431a053f3f2babb73ca6b4329cf72dcf9cd45a29cc8
   manager: conda
   name: python
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/python-3.10.11-he7542f4_0_cpython.conda
-  version: 3.10.11
+  url: https://conda.anaconda.org/conda-forge/osx-64/python-3.10.12-had23ca6_0_cpython.conda
+  version: 3.10.12
 - category: main
   dependencies:
     libsqlite: 3.42.0 h58db7d2_0
     libzlib: '>=1.2.13,<1.3.0a0'
     ncurses: '>=6.3,<7.0a0'
     readline: '>=8.2,<9.0a0'
   hash:
@@ -8049,38 +8070,38 @@
   name: blinker
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/blinker-1.6.2-pyhd8ed1ab_0.conda
   version: 1.6.2
 - category: main
   dependencies:
-    brotli-bin: 1.0.9 hb7f2c08_8
-    libbrotlidec: 1.0.9 hb7f2c08_8
-    libbrotlienc: 1.0.9 hb7f2c08_8
+    brotli-bin: 1.0.9 hb7f2c08_9
+    libbrotlidec: 1.0.9 hb7f2c08_9
+    libbrotlienc: 1.0.9 hb7f2c08_9
   hash:
-    md5: 55f612fe4a9b5f6ac76348b6de94aaeb
-    sha256: 1272426370f1e8db1a8b245a7b522afe27413b09eab169990512a7676b802e3b
+    md5: 53cff90f0cea22e13e5b791f0e5a8e7d
+    sha256: eb425d4075f90d90bf9de5c2e8f88fe783d70177fcdfd3d3da5ef48e444ca148
   manager: conda
   name: brotli
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/brotli-1.0.9-hb7f2c08_8.tar.bz2
+  url: https://conda.anaconda.org/conda-forge/osx-64/brotli-1.0.9-hb7f2c08_9.conda
   version: 1.0.9
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
-    md5: fd006afc4115740d8d52887ee813f262
-    sha256: d17f6b5ae744e64a337c9dbad21b8d501916eaf0e55564dc81c78c492783d73a
+    md5: 60b5eb16d9a7a5482ba37f67aa49db5b
+    sha256: 8d30a41a88900730c748f5b296730a0d48e5cfa2c8b260aab60fa9f26ffafcc0
   manager: conda
   name: cachetools
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/cachetools-5.3.0-pyhd8ed1ab_0.conda
-  version: 5.3.0
+  url: https://conda.anaconda.org/conda-forge/noarch/cachetools-5.3.1-pyhd8ed1ab_0.conda
+  version: 5.3.1
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
     md5: 5d1b71c942b8421285934dad1d891ebc
     sha256: f839a6e04d94069f90dd85337ea9108f058dc76771bb469a413f32bb1ba0b256
   manager: conda
@@ -8213,22 +8234,22 @@
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2
   version: '0.4'
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
-    md5: 7312299d7a0ea4993159229b7d2dceb2
-    sha256: f073c3ba993912f1c0027bc34a54975642885f0a4cd5f9dc42a17ca945df2c18
+    md5: de4cb3384374e1411f0454edcf546cdb
+    sha256: 7b23ea0169fa6e7c3a0867d96d9eacd312759f83e5d83ad0fcc93e85379c16ae
   manager: conda
   name: exceptiongroup
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda
-  version: 1.1.1
+  url: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda
+  version: 1.1.2
 - category: main
   dependencies:
     python: '>=2.7'
   hash:
     md5: 4c1bc140e2be5c8ba6e3acab99e25c50
     sha256: 9c03425cd58c474af20e179c9ba121a82984d6c4bfc896bbc992f5ed75dd7539
   manager: conda
@@ -8450,22 +8471,22 @@
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/jmespath-1.0.1-pyhd8ed1ab_0.tar.bz2
   version: 1.0.1
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
-    md5: 0c0a54e16b764bafcae35913cc9d60ff
-    sha256: 13ffd45adc630670469860932b4c046a46248b9b96d5c8fa8b3a95cdd0618f78
+    md5: 2bc3ca2f7387af385dd06706b4fb2d35
+    sha256: 0781ed7a4f35ff1309e95381c40c8d8f96263ca4260a72baaafda87c975a972a
   manager: conda
   name: jupyterlab_widgets
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.7-pyhd8ed1ab_1.conda
-  version: 3.0.7
+  url: https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.8-pyhd8ed1ab_0.conda
+  version: 3.0.8
 - category: main
   dependencies:
     libcxx: '>=14.0.4'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
   hash:
     md5: cc358fb878ac593c60cea08b28ac7423
@@ -8529,30 +8550,31 @@
   name: libcurl
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/libcurl-8.1.2-hbee3ae8_0.conda
   version: 8.1.2
 - category: main
   dependencies:
+    __osx: '>=10.13'
     c-ares: '>=1.19.1,<2.0a0'
-    libabseil: '>=20230125.2,<20230126.0a0'
+    libabseil: '>=20230125.3,<20230126.0a0'
     libcxx: '>=15.0.7'
-    libprotobuf: '>=4.23.2,<4.23.3.0a0'
+    libprotobuf: '>=4.23.3,<4.23.4.0a0'
     libzlib: '>=1.2.13,<1.3.0a0'
     openssl: '>=3.1.1,<4.0a0'
     re2: '>=2023.3.2,<2023.3.3.0a0'
   hash:
-    md5: bbeac6706560961d3eb7cb75c6cc5ab1
-    sha256: e9a1e028526906c1dba90ebcf0f9f9dfd365501546090791a13affffd09a9f2e
+    md5: 46a189776f694d37c24c5c1fc301bf50
+    sha256: 6eb1860ab843c2711e67e1d084efe3cbc74ef8785fa8d908e9ef57879b9ebeee
   manager: conda
   name: libgrpc
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/libgrpc-1.55.1-h73e6b18_1.conda
-  version: 1.55.1
+  url: https://conda.anaconda.org/conda-forge/osx-64/libgrpc-1.56.0-he6801ca_2.conda
+  version: 1.56.0
 - category: main
   dependencies:
     krb5: '>=1.20.1,<1.21.0a0'
     libzlib: '>=1.2.13,<1.3.0a0'
     openssl: '>=3.1.0,<4.0a0'
   hash:
     md5: 571aa9141d1a823202bb4cd794c939b0
@@ -8716,25 +8738,25 @@
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/mypy_extensions-1.0.0-pyha770c72_0.conda
   version: 1.0.0
 - category: main
   dependencies:
     libcxx: '>=15.0.7'
     libzlib: '>=1.2.13,<1.3.0a0'
-    mysql-common: 8.0.33 hc6116ba_0
+    mysql-common: 8.0.33 hc6116ba_1
     openssl: '>=3.1.1,<4.0a0'
     zstd: '>=1.5.2,<1.6.0a0'
   hash:
-    md5: 8e35f9a9a8965c8c29e9f678e290ac7f
-    sha256: 9665dc412d9b975b790c54c4e7c277e7c73de3b9846244c4094fce266ef7fad3
+    md5: b1ba5ec2e4a774e8e4887f0f7592b574
+    sha256: 4af3a969518d0558b13d458901018220c69207e82d2a2a945c563778541fb356
   manager: conda
   name: mysql-libs
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/mysql-libs-8.0.33-haa61052_0.conda
+  url: https://conda.anaconda.org/conda-forge/osx-64/mysql-libs-8.0.33-haa61052_1.conda
   version: 8.0.33
 - category: main
   dependencies:
     python: '>=3.5'
   hash:
     md5: 7b868f21adde0d9b8b38f9c16836589b
     sha256: 594d240d8be933b6e47b78b786269cc89ffa34874544d9dbed1c6afc9213869b
@@ -8843,22 +8865,22 @@
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2
   version: 1.3.10
 - category: main
   dependencies:
     python: '>=3.8'
   hash:
-    md5: 7d301a0d25f424d96175f810935f0da9
-    sha256: c25e1757e4e90638bb1e778aba3ee5f3c01fae9752e3c3929f9be7d367f6c7f3
+    md5: 7263924c642d22e311d9e59b839f1b33
+    sha256: ff1f70e0bd50693be7e2bad0efb2539f5dcc5ec4d638e787e703f28098e72de4
   manager: conda
   name: pluggy
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.0.0-pyhd8ed1ab_5.tar.bz2
-  version: 1.0.0
+  url: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.2.0-pyhd8ed1ab_0.conda
+  version: 1.2.0
 - category: main
   dependencies:
     python: ''
   hash:
     md5: 7205635cd71531943440fbfe3b6b5727
     sha256: 2cd6fae8f9cbc806b7f828f006ae4a83c23fac917cacfd73c37ce322d4324e53
   manager: conda
@@ -9397,22 +9419,22 @@
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2
   version: 0.5.1
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
-    md5: 1dd6387a73d84e16b6f73de676bb4c36
-    sha256: 713075726a3e1db115dfeb48c448e72a8eb7c378af3e2598094a021bc21ce0fd
+    md5: c34d9325a609381a0b0e8a5b4f325147
+    sha256: c71cb65ac49692adb33735f3114b99a96c0c5140db1d56cf4ccef4fe92ea9a4c
   manager: conda
   name: websocket-client
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.0-pyhd8ed1ab_0.conda
-  version: 1.6.0
+  url: https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda
+  version: 1.6.1
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
     md5: 49bb0d9e60ce1db25e151780331bb5f3
     sha256: 79b4d29b0c004014a2abd5fc2c9fcd35cc6256222b960c2a317a27c4b0d8884d
   manager: conda
@@ -9421,22 +9443,22 @@
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda
   version: 0.40.0
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
-    md5: bcc54b91a8ce88f60f538b87b409909e
-    sha256: c63d6e1a51593895dec44931fb2396cfb80e8454d3c7062311a6194032c9b47e
+    md5: 2e9ebddf0b93d0fb203d0906b8052c4f
+    sha256: a73d34f8169e206bccfb356c093ff5ced803b953bbcc1480ed27976f97598d68
   manager: conda
   name: widgetsnbextension
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda
-  version: 4.0.7
+  url: https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.8-pyhd8ed1ab_0.conda
+  version: 4.0.8
 - category: main
   dependencies:
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
   hash:
     md5: f91dbc3c63e137a27a4de2964d56e6e3
     sha256: 2dcfffd2ff0a62b41d97cabdbfb4bdf6f39a1792e4b0e8b55163ba72a6e1959e
@@ -9528,22 +9550,22 @@
   version: 2.12.1
 - category: main
   dependencies:
     backports: ''
     python: '>=3.6'
     setuptools: ''
   hash:
-    md5: c5b3edc62d6309088f4970b3eaaa65a6
-    sha256: fdea00d4b79990f3fe938e2716bc32bd895eb5c44b6c75b8261db095a1b33c16
+    md5: 6b1b907661838a75d067a22f87996b2e
+    sha256: 7027bb689dd4ca4a08e3b25805de9d04239be6b31125993558f21f102a9d2700
   manager: conda
   name: backports.functools_lru_cache
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.4-pyhd8ed1ab_0.tar.bz2
-  version: 1.6.4
+  url: https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda
+  version: 1.6.5
 - category: main
   dependencies:
     python: '>=3.6'
     soupsieve: '>=1.2'
   hash:
     md5: a362ff7d976217f8fa78c0f1c4f59717
     sha256: 52d3e6bcd442537e22699cd227d8fdcfd54b708eeb8ee5b4c671a6a9b9cd74da
@@ -9751,29 +9773,29 @@
   name: gmpy2
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/gmpy2-2.1.2-py310hb691cb2_1.tar.bz2
   version: 2.1.2
 - category: main
   dependencies:
-    __osx: '>=10.9'
+    __osx: '>=10.13'
     libcxx: '>=15.0.7'
-    libgrpc: 1.55.1 h73e6b18_1
+    libgrpc: 1.56.0 he6801ca_2
     libzlib: '>=1.2.13,<1.3.0a0'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
   hash:
-    md5: cabe22578d16cd6a36a22d215a8a0f53
-    sha256: 4ac1b1c7bd7e23b915301adc15eb2a1ebaba59c2d0b12c8ee2c72761b4533281
+    md5: 0ce1b3a5e4abf21c5a33e8d270ec2be2
+    sha256: 87bbaee723f135f6d58825206405e35e59af620cfff762ee8ba94c2194577396
   manager: conda
   name: grpcio
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/grpcio-1.55.1-py310hd8379ad_1.conda
-  version: 1.55.1
+  url: https://conda.anaconda.org/conda-forge/osx-64/grpcio-1.56.0-py310h0d4bf3c_2.conda
+  version: 1.56.0
 - category: main
   dependencies:
     libaec: '>=1.0.6,<2.0a0'
     libcurl: '>=7.87.0,<9.0a0'
     libcxx: '>=13.0.1'
     libgfortran: 5.*
     libgfortran5: '>=9.5.0'
@@ -9916,22 +9938,22 @@
   version: 3.9.0
 - category: main
   dependencies:
     packaging: '>=17.1'
     python: '>=3.8'
     typing_extensions: ''
   hash:
-    md5: ad16f58b64d3b41f4cbb75040b06c9cc
-    sha256: 8c1fff22ab86c85768e65dc8c4f4664787476a21f4d934c4e0261a1fa7523f9c
+    md5: c71f7ec8b80a536e58b979299b230251
+    sha256: 9c866f31ff7a02cc70b306f65b1a81eabf84826b0d32c1f51e0ece17cfcdaf79
   manager: conda
   name: lightning-utilities
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/lightning-utilities-0.8.0-pyhd8ed1ab_0.conda
-  version: 0.8.0
+  url: https://conda.anaconda.org/conda-forge/noarch/lightning-utilities-0.9.0-pyhd8ed1ab_0.conda
+  version: 0.9.0
 - category: main
   dependencies:
     python: '>=3.6'
     uc-micro-py: '>=1.0.1,<2.0.0'
   hash:
     md5: 25b93e66067eb496ac10da888e25cc33
     sha256: 0980092a2e0a4bd263c18fb0db701589fc10fc8542ce511f844a533490d5f14e
@@ -10044,29 +10066,29 @@
   name: proj
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/proj-9.1.0-hcbd9701_0.tar.bz2
   version: 9.1.0
 - category: main
   dependencies:
-    libabseil: '>=20230125.2,<20230126.0a0'
+    libabseil: '>=20230125.3,<20230126.0a0'
     libcxx: '>=15.0.7'
-    libprotobuf: '>=4.23.2,<4.23.3.0a0'
+    libprotobuf: '>=4.23.3,<4.23.4.0a0'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     setuptools: ''
   hash:
-    md5: 62b758907a0ff180ceccd17ed0024aad
-    sha256: 9d517d9984402442cea85df8a7ec3901a3ed0f62af2de699f04731ebd6a01ac3
+    md5: 8da9b5d52ebad6a80785fdf5f2c57ff9
+    sha256: 28801d92d3ea66ac6f1ad961af1974479f9499cf62940616bd269ab62ca08d44
   manager: conda
   name: protobuf
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/protobuf-4.23.2-py310h4e8a696_1.conda
-  version: 4.23.2
+  url: https://conda.anaconda.org/conda-forge/osx-64/protobuf-4.23.3-py310h4e8a696_0.conda
+  version: 4.23.3
 - category: main
   dependencies:
     pyasn1: '>=0.4.6,<0.5.0'
     python: ''
   hash:
     md5: ad1e886d09700b2304975335f714bd9c
     sha256: 21f5d8ebf36ad2841028b7358b6b316441493d923045156e9c0e07eb62780e44
@@ -10369,26 +10391,27 @@
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/ghp-import-2.1.0-pyhd8ed1ab_0.tar.bz2
   version: 2.1.0
 - category: main
   dependencies:
     gettext: '>=0.21.1,<1.0a0'
-    glib: '>=2.76.2,<3.0a0'
+    glib: '>=2.76.3,<3.0a0'
     libcxx: '>=15.0.7'
-    libglib: '>=2.76.2,<3.0a0'
+    libglib: '>=2.76.3,<3.0a0'
+    libiconv: '>=1.17,<2.0a0'
   hash:
-    md5: a680a8c0182d9dfbac6cac234306ab67
-    sha256: 23a4fa5776e48a3053e89a1d1cdfaa09bb0279880fa47ddafd64bc53a1428aa4
+    md5: a24d0265742fe6614ca8d1186c0d8a42
+    sha256: 20014fd8c3a42094b8127f1a06c57c9c47115343fa721baae245b984def4ff60
   manager: conda
   name: gstreamer
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/gstreamer-1.22.3-h53e17e3_1.conda
-  version: 1.22.3
+  url: https://conda.anaconda.org/conda-forge/osx-64/gstreamer-1.22.4-h840fbdc_0.conda
+  version: 1.22.4
 - category: main
   dependencies:
     cairo: '>=1.16.0,<2.0a0'
     freetype: '>=2.12.1,<3.0a0'
     graphite2: ''
     icu: '>=70.1,<71.0a0'
     libcxx: '>=14.0.6'
@@ -10545,22 +10568,22 @@
   url: https://conda.anaconda.org/conda-forge/osx-64/numpy-1.25.0-py310h7451ae0_0.conda
   version: 1.25.0
 - category: main
   dependencies:
     python: '>=3.7'
     typing-extensions: '>=4.6.3'
   hash:
-    md5: 741384b21c1b512617f4ee4ea8457c5d
-    sha256: ba254f8e7bc01586779c40d040ee000627cddc57965ccbcdb155936c534520d6
+    md5: 3e4aca765371893ad848397794600632
+    sha256: 5f382d0d3509784152506e0e022bb5a30d254555e809804491207196f890af67
   manager: conda
   name: platformdirs
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.6.0-pyhd8ed1ab_0.conda
-  version: 3.6.0
+  url: https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.8.0-pyhd8ed1ab_0.conda
+  version: 3.8.0
 - category: main
   dependencies:
     latexcodec: '>=1.0.4'
     python: '>=3.6'
     pyyaml: '>=3.01'
     setuptools: ''
     six: ''
@@ -10641,22 +10664,22 @@
 - category: main
   dependencies:
     greenlet: '!=0.4.17'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     typing-extensions: '>=4.2.0'
   hash:
-    md5: 2cb1231f747d33242f6ae506eb6e9b93
-    sha256: e9de52699f42a390e076b824b67eea0e867da25ecf3feb12e870f21151c04aa4
+    md5: 2f7579944d2f1b682ad79c1de277368f
+    sha256: 89026e4549fa599e7db91a68a53cfa16983327e52ea661f1aadb5adccf59f71b
   manager: conda
   name: sqlalchemy
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/sqlalchemy-2.0.16-py310h6729b98_0.conda
-  version: 2.0.16
+  url: https://conda.anaconda.org/conda-forge/osx-64/sqlalchemy-2.0.17-py310h6729b98_0.conda
+  version: 2.0.17
 - category: main
   dependencies:
     asttokens: ''
     executing: ''
     pure_eval: ''
     python: '>=3.5'
   hash:
@@ -10781,30 +10804,31 @@
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/contourpy-1.1.0-py310h88cfcbd_0.conda
   version: 1.1.0
 - category: main
   dependencies:
     gettext: '>=0.21.1,<1.0a0'
-    gstreamer: 1.22.3 h53e17e3_1
+    gstreamer: 1.22.4 h840fbdc_0
     libcxx: '>=15.0.7'
-    libglib: '>=2.76.2,<3.0a0'
+    libglib: '>=2.76.3,<3.0a0'
+    libogg: '>=1.3.4,<1.4.0a0'
     libopus: '>=1.3.1,<2.0a0'
     libpng: '>=1.6.39,<1.7.0a0'
     libvorbis: '>=1.3.7,<1.4.0a0'
     libzlib: '>=1.2.13,<1.3.0a0'
   hash:
-    md5: d01492c656e4a1b5fcd5600a3e745fd5
-    sha256: a3c2018dd8972c996cb74bedcc23f3c5cb5f5193d435fcc1cbed22689176f2bc
+    md5: 3ddc9bb14daecff3a86233f07e0d472a
+    sha256: ef79b53e2a69ffba4fd089d461502049c955ca8d677aa7d5452b3dd87723521a
   manager: conda
   name: gst-plugins-base
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/gst-plugins-base-1.22.3-hb5d3a86_1.conda
-  version: 1.22.3
+  url: https://conda.anaconda.org/conda-forge/osx-64/gst-plugins-base-1.22.4-hb5d3a86_0.conda
+  version: 1.22.4
 - category: main
   dependencies:
     platformdirs: '>=2.5'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     traitlets: '>=5.3'
   hash:
@@ -10886,22 +10910,22 @@
   url: https://conda.anaconda.org/conda-forge/osx-64/pango-1.50.14-hbd9bf65_0.conda
   version: 1.50.14
 - category: main
   dependencies:
     python: '>=3.7'
     wcwidth: ''
   hash:
-    md5: 59ba1bf8ea558751a0d391249a248765
-    sha256: 78c2f3c6195ec350d7d6e5fa3e43274ca8191c181c97a867e2920faaeec0e9bc
+    md5: a4986c6bb5b0d05a38855b0880a5f425
+    sha256: 10e7fdc75d4b85633be6b12a70b857053987127a808caa0f88b2cba4b3ce6359
   manager: conda
   name: prompt-toolkit
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda
-  version: 3.0.38
+  url: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda
+  version: 3.0.39
 - category: main
   dependencies:
     docutils: '>=0.8'
     pybtex: '>=0.16'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     setuptools: ''
@@ -11013,22 +11037,22 @@
     jupyter_core: '>=4.12,!=5.0.*'
     python: '>=3.8'
     python-dateutil: '>=2.8.2'
     pyzmq: '>=23.0'
     tornado: '>=6.2'
     traitlets: '>=5.3'
   hash:
-    md5: 58ca2d50c3b27b86fd7df62eaadbf9a9
-    sha256: c36c0e9da3a23e89fc30333760f9c9fdb1a14ca2862fa1e1257f7fe4d508fded
+    md5: 1d018ee4ab13217e2544f795eb0a6798
+    sha256: 7dc74a032daefbdcf4d6d661616dfdc8649e5cf9db58258afe91cc09ea0cf402
   manager: conda
   name: jupyter_client
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.2.0-pyhd8ed1ab_0.conda
-  version: 8.2.0
+  url: https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda
+  version: 8.3.0
 - category: main
   dependencies:
     cairo: '>=1.16.0,<2.0.0a0'
     gdk-pixbuf: '>=2.42.8,<3.0a0'
     gettext: '>=0.19.8.1,<1.0a0'
     libglib: '>=2.70.2,<3.0a0'
     libxml2: '>=2.9.14,<2.11.0a0'
@@ -11082,24 +11106,24 @@
   name: nbformat
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda
   version: 5.9.0
 - category: main
   dependencies:
-    prompt-toolkit: '>=3.0.38,<3.0.39.0a0'
+    prompt-toolkit: '>=3.0.39,<3.0.40.0a0'
   hash:
-    md5: 45b74f64d8808eda7e6f6e6b1d641fd2
-    sha256: c0f24a75d27918eb33f86902aa6024783d128a89eb3a169bcb22f24163a422b3
+    md5: 4bbbe67d5df19db30f04b8e344dc9976
+    sha256: 89f7fecc7355181dbc2ab851e668a2fce6aa4830b336a34c93b59bda93206270
   manager: conda
   name: prompt_toolkit
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda
-  version: 3.0.38
+  url: https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.39-hd8ed1ab_0.conda
+  version: 3.0.39
 - category: main
   dependencies:
     gst-plugins-base: '>=1.22.0,<1.23.0a0'
     gstreamer: '>=1.22.0,<1.23.0a0'
     icu: '>=70.1,<71.0a0'
     jpeg: '>=9e,<10a'
     krb5: '>=1.20.1,<1.21.0a0'
@@ -11142,37 +11166,37 @@
   url: https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.15-pyhd8ed1ab_0.conda
   version: 1.26.15
 - category: main
   dependencies:
     aiohttp: <4
     python: '>=3.6'
   hash:
-    md5: 70f4b52c0e703936aa1812d8b14a5bb2
-    sha256: 11dd5e6c5062e788160167e2a64fcbbb2c7ec825e28d628a9e7771172e039de7
+    md5: 0d0113b67472cea3da288838ebc80acb
+    sha256: 656947c8457d5ac06f11dc1da904ac7ac8ac8edf81323ee9794a3d51ace79ff3
   manager: conda
   name: wslink
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/wslink-1.11.0-pyhd8ed1ab_0.conda
-  version: 1.11.0
+  url: https://conda.anaconda.org/conda-forge/noarch/wslink-1.11.1-pyhd8ed1ab_0.conda
+  version: 1.11.1
 - category: main
   dependencies:
     jmespath: '>=0.7.1,<2.0.0'
     python: '>=3.7'
     python-dateutil: '>=2.1,<3.0.0'
     urllib3: '>=1.25.4,<1.27'
   hash:
-    md5: ccfde1c6ce8dbb4af5590c88a0482248
-    sha256: b818c4a738c58fcc1ca231f75bfbfdd516b44e437a460336bdbee70a9a4573ca
+    md5: 0f30016ea54215fdb883b8978340c9b7
+    sha256: ccbd3413915259825a678707b438e7ba25712d9c8c5748d2d82f24359237b3f9
   manager: conda
   name: botocore
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/botocore-1.29.158-pyhd8ed1ab_0.conda
-  version: 1.29.158
+  url: https://conda.anaconda.org/conda-forge/noarch/botocore-1.29.165-pyhd8ed1ab_0.conda
+  version: 1.29.165
 - category: main
   dependencies:
     cairo: '>=1.16.0,<2.0a0'
     expat: '>=2.5.0,<3.0a0'
     fontconfig: '>=2.14.1,<3.0a0'
     fonts-conda-ecosystem: ''
     freetype: '>=2.12.1,<3.0a0'
@@ -11360,22 +11384,22 @@
     python: '>=3.6'
     pyu2f: '>=0.1.5'
     requests: '>=2.20.0,<3.0.0dev'
     rsa: '>=3.1.4,<5'
     six: '>=1.9.0'
     urllib3: <2.0
   hash:
-    md5: 59f942ef9326d2519a7c953f1c24d5da
-    sha256: ba9136edf49c8aa53f45ddfe0c16387bf375f1e5e27f50e39cc1e41c6f5ad25d
+    md5: 8c5dd8609d314721d990c1d1fd607f81
+    sha256: 6b097ca9b31961d6a983f81dc295012e9c99c4c1a5a83a93ab2fcc6528af428f
   manager: conda
   name: google-auth
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/google-auth-2.20.0-pyh1a96a4e_0.conda
-  version: 2.20.0
+  url: https://conda.anaconda.org/conda-forge/noarch/google-auth-2.21.0-pyh1a96a4e_0.conda
+  version: 2.21.0
 - category: main
   dependencies:
     __osx: ''
     appnope: ''
     comm: '>=0.1.1'
     debugpy: '>=1.6.5'
     ipython: '>=7.23.1'
@@ -11386,22 +11410,22 @@
     packaging: ''
     psutil: ''
     python: '>=3.8'
     pyzmq: '>=20'
     tornado: '>=6.1'
     traitlets: '>=5.4.0'
   hash:
-    md5: c406de32f968636cd33f6017f5c3f121
-    sha256: 26aa3db86d56d104927a5f32e5ddee844dd360f490ba2976784999934fb11c04
+    md5: 00cfe411a8e07b8322185e573ae7c5a3
+    sha256: 41b8a6796308d01db5f80fe06392307e72dd5cf155f1914d9f973b2acaafa29b
   manager: conda
   name: ipykernel
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.2-pyh5fb750a_0.conda
-  version: 6.23.2
+  url: https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.3-pyh5fb750a_0.conda
+  version: 6.23.3
 - category: main
   dependencies:
     attrs: ''
     click: ''
     importlib-metadata: ''
     nbclient: '>=0.2,<0.8'
     nbformat: ''
@@ -11543,59 +11567,78 @@
   name: torchmetrics
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/torchmetrics-0.11.4-pyhd8ed1ab_0.conda
   version: 0.11.4
 - category: main
   dependencies:
-    botocore: '>=1.29.158,<1.30.0'
+    ffmpeg: '>=4.2'
+    jpeg: ''
+    libpng: ''
+    numpy: '>=1.11'
+    pillow: '>=5.3.0,!=8.3.*'
+    python: '>=3.10,<3.11.0a0'
+    pytorch: 2.0.1
+    requests: ''
+  hash:
+    md5: 5c3600915df5413045fc3335c7b66ece
+    sha256: 6d9ea50f1923baa41fc9b8fa23567fc0deee2fe4c2bf81f658d5f867dc8ded1d
+  manager: conda
+  name: torchvision
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/pytorch/osx-64/torchvision-0.15.2-py310_cpu.tar.bz2
+  version: 0.15.2
+- category: main
+  dependencies:
+    botocore: '>=1.29.165,<1.30.0'
     jmespath: '>=0.7.1,<2.0.0'
     python: '>=3.7'
     s3transfer: '>=0.6.0,<0.7.0'
   hash:
-    md5: 2e39307a3987518e49eb30ca51e3cfb5
-    sha256: b22c2838e528d03d670f1ecbc57f3d57b4a93d21f456b1248788d7be4e080e3a
+    md5: b9a6316db67d5f2c8dbac2aeb24c6803
+    sha256: 4ca4d8c481609dbf8ce755a8f115486e40be0f0d01c0961c696d6f995dadb2f5
   manager: conda
   name: boto3
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/boto3-1.26.158-pyhd8ed1ab_0.conda
-  version: 1.26.158
+  url: https://conda.anaconda.org/conda-forge/noarch/boto3-1.26.165-pyhd8ed1ab_0.conda
+  version: 1.26.165
 - category: main
   dependencies:
     click: '>=6.0.0'
-    google-auth: '>=1.0.0'
+    google-auth: '>=2.15.0'
     python: '>=3.6'
     requests-oauthlib: '>=0.7.0'
   hash:
-    md5: 5ba9d95acb9add67f468ecdee6595c0f
-    sha256: ef8edcbc8efe616d0f3686607f445a6a96f3549ce2faed1797ad35ca5cd42e81
+    md5: 569e62e95b01b53e4ec7d9abe83b7385
+    sha256: f89613643658a51a1ac0fb7c7950526fadc2a6ce1ae13755d786e14cfce1633c
   manager: conda
   name: google-auth-oauthlib
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/google-auth-oauthlib-1.0.0-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/google-auth-oauthlib-1.0.0-pyhd8ed1ab_1.conda
   version: 1.0.0
 - category: main
   dependencies:
     ipykernel: '>=4.5.1'
     ipython: '>=6.1.0'
-    jupyterlab_widgets: '>=3.0.7,<4.1.dev0'
+    jupyterlab_widgets: '>=3.0.7,<3.1.0'
     python: '>=3.7'
     traitlets: '>=4.3.1'
-    widgetsnbextension: '>=4.0.7,<4.1.dev0'
+    widgetsnbextension: '>=4.0.7,<4.1.0'
   hash:
-    md5: 68627a08556e4a273e4c7bfc84251457
-    sha256: a18f168f368cc8ba4d11a83bf57fcd664bd311a0fcc9b36c283715470f43c133
+    md5: 4b0f4e8fe2a303e472674eae0340bdad
+    sha256: 3b17ad90294f0684fca9191f1e696e9b4f03a652d5e588b6ff0feb5647fcf116
   manager: conda
   name: ipywidgets
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.6-pyhd8ed1ab_0.conda
-  version: 8.0.6
+  url: https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.7-pyhd8ed1ab_0.conda
+  version: 8.0.7
 - category: main
   dependencies:
     ipykernel: '>=6.14'
     ipython: ''
     jupyter_client: '>=7.0.0'
     jupyter_core: '>=4.12,!=5.0.*'
     prompt_toolkit: '>=3.0.30'
@@ -11630,22 +11673,22 @@
     pyzmq: '>=24'
     send2trash: ''
     terminado: '>=0.8.3'
     tornado: '>=6.2.0'
     traitlets: '>=5.6.0'
     websocket-client: ''
   hash:
-    md5: 39fd52b0fcb2fb52bac47a1419bf09bd
-    sha256: 0f0feb284f667964d1e4122a7690f6e3ace257732591a6151fdd1eb797911128
+    md5: 7488cd1f4d35a2af96faa765b7e5b2f0
+    sha256: 132bfa3eef62231e53b59d93358f818a97c5e7939670bfdd821b7146a0094e43
   manager: conda
   name: jupyter_server
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.6.0-pyhd8ed1ab_0.conda
-  version: 2.6.0
+  url: https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.7.0-pyhd8ed1ab_0.conda
+  version: 2.7.0
 - category: main
   dependencies:
     docutils: '>=0.15,<0.20'
     jinja2: ''
     markdown-it-py: '>=1.0.0,<3.0.0'
     mdit-py-plugins: '>=0.3.1,<1'
     python: '>=3.7'
@@ -11704,22 +11747,22 @@
     pytorch: '>=1.11.0'
     pyyaml: '>=5.4'
     requests: ''
     torchmetrics: '>=0.7.0'
     tqdm: '>=4.57.0'
     typing_extensions: '>=4.0.0'
   hash:
-    md5: 97138eb8783fa54884216a6562413736
-    sha256: d2b5fbd636393c71dfc07ce5a15eb36285b01aaa34453b3fd8b9b26f0fa5b689
+    md5: ce9d626b181c6f8cceb5047f6a819f7d
+    sha256: a049296b4b33bceedf3bafd378e8a4112bca71b453734f1e0daaca2a72598593
   manager: conda
   name: pytorch-lightning
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pytorch-lightning-2.0.3-pyhd8ed1ab_0.conda
-  version: 2.0.3
+  url: https://conda.anaconda.org/conda-forge/noarch/pytorch-lightning-2.0.4-pyhd8ed1ab_0.conda
+  version: 2.0.4
 - category: main
   dependencies:
     ipykernel: '>=4.1'
     ipython_genutils: ''
     jupyter_client: '>=4.1'
     jupyter_core: ''
     packaging: ''
@@ -12244,22 +12287,22 @@
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/nvidia/win-64/cuda-nvtx-11.8.86-0.tar.bz2
   version: 11.8.86
 - category: main
   dependencies: {}
   hash:
-    md5: fac1be557eb9ea49655c2d5bd10242d0
-    sha256: cb8968041d3f689467433908798255e09e274e91caf6d8ce4cc204cbba048559
+    md5: 93cb84c3524a1612cbce98ead299c735
+    sha256: 26ab725d6db651e09943f88cc94a90afe8147cabe0e444dccf10bc70420f62a8
   manager: conda
   name: cuda-profiler-api
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/nvidia/win-64/cuda-profiler-api-12.1.105-0.tar.bz2
-  version: 12.1.105
+  url: https://conda.anaconda.org/nvidia/win-64/cuda-profiler-api-12.2.53-0.tar.bz2
+  version: 12.2.53
 - category: main
   dependencies: {}
   hash:
     md5: c9f9d925118c389a1a3f4267b6272b98
     sha256: 1634892d2b95f7cc27bb1cfaa5ba0de6f2478582961a0fd2d309f3956e883640
   manager: conda
   name: cuda-version
@@ -12656,22 +12699,22 @@
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/m2w64-libwinpthread-git-5.0.0.4634.697f757-2.tar.bz2
   version: 5.0.0.4634.697f757
 - category: main
   dependencies:
     ucrt: '>=10.0.20348.0'
   hash:
-    md5: 22125178654c6a8a393f9743d585704b
-    sha256: 1161f4848e1c0663897a6324fbc4ff13dafd11650b42c9864428da73593dda95
+    md5: 91c1ecaf3996889532fc0456178b1058
+    sha256: e76986c555647347a0185e646ef65625dabed60da255f6b30367df8bd6dc6cd8
   manager: conda
   name: vc14_runtime
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.34.31931-h5081d32_16.conda
-  version: 14.34.31931
+  url: https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.36.32532-hfdfe4a8_17.conda
+  version: 14.36.32532
 - category: main
   dependencies:
     cuda-cccl-impl: 2.0.1
     cuda-cccl_win-64: 12.0.90
     cuda-version: '>=12.0.0,<12.1.0a0'
   hash:
     md5: f1ceeb722d224d7be3ea7cd33abe5e25
@@ -12706,36 +12749,36 @@
   name: m2w64-gcc-libs-core
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/m2w64-gcc-libs-core-5.3.0-7.tar.bz2
   version: 5.3.0
 - category: main
   dependencies:
-    vc14_runtime: '>=14.32.31332'
+    vc14_runtime: '>=14.36.32532'
   hash:
-    md5: ea326b37e3bd6d2616988e09f3a9396c
-    sha256: 29bc108d66150ca75cab937f844f4ac4a836beb6ea3ee167d03c611444bb2a82
+    md5: 67ff6791f235bb606659bf2a5c169191
+    sha256: 86ae94bf680980776aa761c2b0909a0ddbe1f817e7eeb8b16a1730f10f8891b6
   manager: conda
   name: vc
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/vc-14.3-hb25d44b_16.conda
+  url: https://conda.anaconda.org/conda-forge/win-64/vc-14.3-h64f974e_17.conda
   version: '14.3'
 - category: main
   dependencies:
-    vc14_runtime: '>=14.34.31931'
+    vc14_runtime: '>=14.36.32532'
   hash:
-    md5: 0374eae69b6dbfb27c3dc27167109eb4
-    sha256: 25d852887a501ca8cb6753a4f3dae1549fa49592d51aec1a230b1f0c85fe4297
+    md5: 4618046c39f7c81861e53ded842e738a
+    sha256: 5ecbd731dc7f13762d67be0eadc47eb7f14713005e430d9b5fc680e965ac0f81
   manager: conda
   name: vs2015_runtime
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.34.31931-hed1258a_16.conda
-  version: 14.34.31931
+  url: https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.36.32532-h05e6639_17.conda
+  version: 14.36.32532
 - category: main
   dependencies:
     vc: '>=14.2,<15'
     vs2015_runtime: '>=14.29.30139'
   hash:
     md5: 455524d2bf9625a42a1848c0d08ac063
     sha256: 76a2fc753c372facbb83bc9fc063cbc9c439ec0922d5c776a4d280fc42ff885c
@@ -12945,22 +12988,22 @@
   version: 4.0.0
 - category: main
   dependencies:
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
   hash:
-    md5: 828f6bb057da235a4703ed33192f81c5
-    sha256: 8c4e1cde02f7937b4b1f089a75e785f86241f55d1e5d0101a80e3fae0704c173
+    md5: 219d819db61ee021a82ecee3d69642cd
+    sha256: d788ab2062bcfa5ae997d36825a403f4aca2cab3e2bfac15158bd0933189736b
   manager: conda
   name: libabseil
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/libabseil-20230125.2-cxx17_h63175ca_2.conda
-  version: '20230125.2'
+  url: https://conda.anaconda.org/conda-forge/win-64/libabseil-20230125.3-cxx17_h63175ca_0.conda
+  version: '20230125.3'
 - category: main
   dependencies:
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vs2015_runtime: '>=14.29.30139'
   hash:
     md5: f98474a8245f55f4a273889dbe7bf193
@@ -12971,23 +13014,23 @@
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/libaec-1.0.6-h63175ca_1.conda
   version: 1.0.6
 - category: main
   dependencies:
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
-    vs2015_runtime: '>=14.29.30139'
+    vc14_runtime: '>=14.29.30139'
   hash:
-    md5: e8078e37208cd7d3e1eb5053f370ded8
-    sha256: 0e771d447108219f43de770f7ca9428b2e3b5a4fd08475a27ac442ad310cb684
+    md5: 5e0f7bd6f1d0747abd5da59cffb6f533
+    sha256: adef98f4013859c111da28ff1f66c2c65e90213fe8bac78b7fc83a15e26bc955
   manager: conda
   name: libbrotlicommon
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/libbrotlicommon-1.0.9-hcfcfb64_8.tar.bz2
+  url: https://conda.anaconda.org/conda-forge/win-64/libbrotlicommon-1.0.9-hcfcfb64_9.conda
   version: 1.0.9
 - category: main
   dependencies:
     cuda-version: '>=12.0.0,<12.1.0a0'
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vs2015_runtime: '>=14.29.30139'
@@ -13105,24 +13148,24 @@
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/libuv-1.44.2-h8ffe710_0.tar.bz2
   version: 1.44.2
 - category: main
   dependencies:
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
-    vs2015_runtime: '>=14.29.30139'
+    vc14_runtime: '>=14.29.30139'
   hash:
-    md5: 381a3645c51cbf478872899b16490318
-    sha256: 9355940270db76592a1cdbcb840740afb5f6b81d167ac4f2cb0fbb2c37397566
+    md5: f89e765213cac556a8ed72ba8c1b5071
+    sha256: 1652438917a14bf67c1dc5a94a431f45fece7837c016a7144979a50924faa1b7
   manager: conda
   name: libwebp-base
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/libwebp-base-1.3.0-hcfcfb64_0.conda
-  version: 1.3.0
+  url: https://conda.anaconda.org/conda-forge/win-64/libwebp-base-1.3.1-hcfcfb64_0.conda
+  version: 1.3.1
 - category: main
   dependencies:
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
   hash:
     md5: 5fdb9c6a113b6b6cb5e517fd972d5f41
@@ -13366,41 +13409,41 @@
   name: krb5
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/krb5-1.20.1-heb0366b_0.conda
   version: 1.20.1
 - category: main
   dependencies:
-    libbrotlicommon: 1.0.9 hcfcfb64_8
+    libbrotlicommon: 1.0.9 hcfcfb64_9
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
-    vs2015_runtime: '>=14.29.30139'
+    vc14_runtime: '>=14.29.30139'
   hash:
-    md5: 99839d9d81f33afa173c0fa82a702038
-    sha256: 66814b8c0235bcc9124d32cb4b99845bcb2af0eba1d2ba609a501a6d8194e9a0
+    md5: 4c502e4846bdc22b944ab9aa5a55a58f
+    sha256: 12880edf7865c7acb72c8501ef71874a65ee5c7960c19cf21883390bc02860bb
   manager: conda
   name: libbrotlidec
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/libbrotlidec-1.0.9-hcfcfb64_8.tar.bz2
+  url: https://conda.anaconda.org/conda-forge/win-64/libbrotlidec-1.0.9-hcfcfb64_9.conda
   version: 1.0.9
 - category: main
   dependencies:
-    libbrotlicommon: 1.0.9 hcfcfb64_8
+    libbrotlicommon: 1.0.9 hcfcfb64_9
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
-    vs2015_runtime: '>=14.29.30139'
+    vc14_runtime: '>=14.29.30139'
   hash:
-    md5: 88e62627120c20289bf8982b15e0a6a1
-    sha256: 3abf0f0b124d54ad892bd74fe77089a712d6dad81a04583331a58728c58a69e0
+    md5: 19029748649ae0d48871d7012918efef
+    sha256: d8b1ee384d368aa72f7806f771a470e9676149c57f0d12876aff6e45079745c1
   manager: conda
   name: libbrotlienc
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/libbrotlienc-1.0.9-hcfcfb64_8.tar.bz2
+  url: https://conda.anaconda.org/conda-forge/win-64/libbrotlienc-1.0.9-hcfcfb64_9.conda
   version: 1.0.9
 - category: main
   dependencies:
     libzlib: '>=1.2.13,<1.3.0a0'
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
@@ -13448,22 +13491,22 @@
   dependencies:
     libabseil: '>=20230125.2,<20230126.0a0'
     libzlib: '>=1.2.13,<1.3.0a0'
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
   hash:
-    md5: f37b557f68140eec8421e35698c36478
-    sha256: a5d3407de28ce218121f9eac26f0b6a9ecc5653a32d86a5cdcd3a409e751d0cf
+    md5: 6386184da6e9e58de0d8e0a9e9aeb736
+    sha256: 04388df7545ca21a2384e51b4bd66fbfc9e918e55f93876a9bee7998ac0d31b8
   manager: conda
   name: libprotobuf
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/libprotobuf-4.23.2-h1975477_5.conda
-  version: 4.23.2
+  url: https://conda.anaconda.org/conda-forge/win-64/libprotobuf-4.23.3-h1975477_0.conda
+  version: 4.23.3
 - category: main
   dependencies:
     libzlib: '>=1.2.13,<1.3.0a0'
     openssl: '>=3.1.1,<4.0a0'
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
@@ -13502,27 +13545,27 @@
   name: libvorbis
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/libvorbis-1.3.7-h0e60522_0.tar.bz2
   version: 1.3.7
 - category: main
   dependencies:
-    libwebp-base: '>=1.3.0,<2.0a0'
+    libwebp-base: '>=1.3.1,<2.0a0'
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
-    vs2015_runtime: '>=14.29.30139'
+    vc14_runtime: '>=14.29.30139'
   hash:
-    md5: 0c1f2c4b45406631c600ec22ca9523fc
-    sha256: 9100912fc7f8f9772299ca44801c3a44e129e01e9e7acf9210d01aa43e25f19e
+    md5: cc9d668f51da7f6506185ab1130bcd57
+    sha256: 79d42a947ab7b51a4cb64ce730410f2b84738de3bbc4fc718ab07d099c43ae42
   manager: conda
   name: libwebp
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/libwebp-1.3.0-hcfcfb64_0.conda
-  version: 1.3.0
+  url: https://conda.anaconda.org/conda-forge/win-64/libwebp-1.3.1-hcfcfb64_0.conda
+  version: 1.3.1
 - category: main
   dependencies:
     libiconv: '>=1.17,<2.0a0'
     libzlib: '>=1.2.13,<1.3.0a0'
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vs2015_runtime: '>=14.29.30139'
@@ -13583,31 +13626,31 @@
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/pcre2-10.40-h17e33f8_0.tar.bz2
   version: '10.40'
 - category: main
   dependencies:
     bzip2: '>=1.0.8,<2.0a0'
     libffi: '>=3.4,<4.0a0'
-    libsqlite: '>=3.41.2,<4.0a0'
+    libsqlite: '>=3.42.0,<4.0a0'
     libzlib: '>=1.2.13,<1.3.0a0'
-    openssl: '>=3.1.0,<4.0a0'
+    openssl: '>=3.1.1,<4.0a0'
     tk: '>=8.6.12,<8.7.0a0'
     tzdata: ''
     vc: '>=14.1,<15'
     vc14_runtime: '>=14.16.27033'
     xz: '>=5.2.6,<6.0a0'
   hash:
-    md5: db564a923e0197854756c727ad3e4b8f
-    sha256: 1a437ff15647fe8566e6ae2118945080b8cbaebe95bc50d3fb65c1cbefffc22f
+    md5: 14273454ca348a123ce09ab9d39c1a6e
+    sha256: 02ee08f3f27488b76155535e43fc99ef491ccc21f28001c3cde9b134e8aa0b94
   manager: conda
   name: python
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/python-3.10.11-h4de0772_0_cpython.conda
-  version: 3.10.11
+  url: https://conda.anaconda.org/conda-forge/win-64/python-3.10.12-h4de0772_0_cpython.conda
+  version: 3.10.12
 - category: main
   dependencies:
     libsqlite: 3.42.0 hcfcfb64_0
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
   hash:
@@ -13733,40 +13776,40 @@
   name: blinker
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/blinker-1.6.2-pyhd8ed1ab_0.conda
   version: 1.6.2
 - category: main
   dependencies:
-    libbrotlidec: 1.0.9 hcfcfb64_8
-    libbrotlienc: 1.0.9 hcfcfb64_8
+    libbrotlidec: 1.0.9 hcfcfb64_9
+    libbrotlienc: 1.0.9 hcfcfb64_9
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
-    vs2015_runtime: '>=14.29.30139'
+    vc14_runtime: '>=14.29.30139'
   hash:
-    md5: e18b70ed349d96086fd60a9c642b1b58
-    sha256: e8b55a51cb907f336c6f308d5d052483b0cad6a8b09040b811a7f12f4f199d67
+    md5: ba8ae6c24cf47da3fb73270e4f119f08
+    sha256: 08c1431f7b4946a568d8f44d452a9358a841eaa58dd64dee66d8ac7bf1092673
   manager: conda
   name: brotli-bin
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/brotli-bin-1.0.9-hcfcfb64_8.tar.bz2
+  url: https://conda.anaconda.org/conda-forge/win-64/brotli-bin-1.0.9-hcfcfb64_9.conda
   version: 1.0.9
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
-    md5: fd006afc4115740d8d52887ee813f262
-    sha256: d17f6b5ae744e64a337c9dbad21b8d501916eaf0e55564dc81c78c492783d73a
+    md5: 60b5eb16d9a7a5482ba37f67aa49db5b
+    sha256: 8d30a41a88900730c748f5b296730a0d48e5cfa2c8b260aab60fa9f26ffafcc0
   manager: conda
   name: cachetools
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/cachetools-5.3.0-pyhd8ed1ab_0.conda
-  version: 5.3.0
+  url: https://conda.anaconda.org/conda-forge/noarch/cachetools-5.3.1-pyhd8ed1ab_0.conda
+  version: 5.3.1
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
     md5: 5d1b71c942b8421285934dad1d891ebc
     sha256: f839a6e04d94069f90dd85337ea9108f058dc76771bb469a413f32bb1ba0b256
   manager: conda
@@ -13922,22 +13965,22 @@
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2
   version: '0.4'
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
-    md5: 7312299d7a0ea4993159229b7d2dceb2
-    sha256: f073c3ba993912f1c0027bc34a54975642885f0a4cd5f9dc42a17ca945df2c18
+    md5: de4cb3384374e1411f0454edcf546cdb
+    sha256: 7b23ea0169fa6e7c3a0867d96d9eacd312759f83e5d83ad0fcc93e85379c16ae
   manager: conda
   name: exceptiongroup
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda
-  version: 1.1.1
+  url: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda
+  version: 1.1.2
 - category: main
   dependencies:
     python: '>=2.7'
   hash:
     md5: 4c1bc140e2be5c8ba6e3acab99e25c50
     sha256: 9c03425cd58c474af20e179c9ba121a82984d6c4bfc896bbc992f5ed75dd7539
   manager: conda
@@ -14121,22 +14164,22 @@
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/jmespath-1.0.1-pyhd8ed1ab_0.tar.bz2
   version: 1.0.1
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
-    md5: 0c0a54e16b764bafcae35913cc9d60ff
-    sha256: 13ffd45adc630670469860932b4c046a46248b9b96d5c8fa8b3a95cdd0618f78
+    md5: 2bc3ca2f7387af385dd06706b4fb2d35
+    sha256: 0781ed7a4f35ff1309e95381c40c8d8f96263ca4260a72baaafda87c975a972a
   manager: conda
   name: jupyterlab_widgets
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.7-pyhd8ed1ab_1.conda
-  version: 3.0.7
+  url: https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.8-pyhd8ed1ab_0.conda
+  version: 3.0.8
 - category: main
   dependencies:
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vs2015_runtime: '>=14.29.30139'
@@ -14216,31 +14259,31 @@
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/libglib-2.76.3-he8f3873_0.conda
   version: 2.76.3
 - category: main
   dependencies:
     c-ares: '>=1.19.1,<2.0a0'
-    libabseil: '>=20230125.2,<20230126.0a0'
-    libprotobuf: '>=4.23.2,<4.23.3.0a0'
+    libabseil: '>=20230125.3,<20230126.0a0'
+    libprotobuf: '>=4.23.3,<4.23.4.0a0'
     libzlib: '>=1.2.13,<1.3.0a0'
     openssl: '>=3.1.1,<4.0a0'
     re2: '>=2023.3.2,<2023.3.3.0a0'
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
   hash:
-    md5: 5eb83620ff9214afd3cc3cf3d9d87a33
-    sha256: bd89b5b2b30d621b7305e65c157ce5c48f0d2982ea4af552a5b507a8dd26c8be
+    md5: 44b832412b9a71277e67ecc52ffec4f2
+    sha256: 6a6791a8e6e68c36805ed83f6ad0929c20fcd5f3249cff5242f09a39e7f136fd
   manager: conda
   name: libgrpc
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/libgrpc-1.55.1-h0c1e3fa_1.conda
-  version: 1.55.1
+  url: https://conda.anaconda.org/conda-forge/win-64/libgrpc-1.56.0-hea2d5f7_2.conda
+  version: 1.56.0
 - category: main
   dependencies:
     libxml2: '>=2.10.3,<2.11.0a0'
     pthreads-win32: ''
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vs2015_runtime: '>=14.29.30139'
@@ -14473,22 +14516,22 @@
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2
   version: 1.3.10
 - category: main
   dependencies:
     python: '>=3.8'
   hash:
-    md5: 7d301a0d25f424d96175f810935f0da9
-    sha256: c25e1757e4e90638bb1e778aba3ee5f3c01fae9752e3c3929f9be7d367f6c7f3
+    md5: 7263924c642d22e311d9e59b839f1b33
+    sha256: ff1f70e0bd50693be7e2bad0efb2539f5dcc5ec4d638e787e703f28098e72de4
   manager: conda
   name: pluggy
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.0.0-pyhd8ed1ab_5.tar.bz2
-  version: 1.0.0
+  url: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.2.0-pyhd8ed1ab_0.conda
+  version: 1.2.0
 - category: main
   dependencies:
     python: ''
   hash:
     md5: 7205635cd71531943440fbfe3b6b5727
     sha256: 2cd6fae8f9cbc806b7f828f006ae4a83c23fac917cacfd73c37ce322d4324e53
   manager: conda
@@ -14976,24 +15019,24 @@
   version: 5.9.0
 - category: main
   dependencies:
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
-    vs2015_runtime: '>=14.29.30139'
+    vc14_runtime: '>=14.29.30139'
   hash:
-    md5: 5cc75fe139b6fa921326677120d44893
-    sha256: 67170f00794c10ee3d346071a6afb003a585ce96251a0ec2dddc237a561aa97d
+    md5: a2ac0e6c5a06b35dea207c3d77f94f74
+    sha256: a43f39e35901b4c2378b6fb34fe98bd1b397190e56b9478bf766001334fab7b1
   manager: conda
   name: typed-ast
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/typed-ast-1.5.4-py310h8d17308_1.tar.bz2
-  version: 1.5.4
+  url: https://conda.anaconda.org/conda-forge/win-64/typed-ast-1.5.5-py310h8d17308_0.conda
+  version: 1.5.5
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
     md5: 4a3014a4d107d15475d106b751c4e352
     sha256: 90a8d56c8015af1575d504d5f77d95a806cd999fc178a06ab51a349f1f744672
   manager: conda
@@ -15066,22 +15109,22 @@
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2
   version: 0.5.1
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
-    md5: 1dd6387a73d84e16b6f73de676bb4c36
-    sha256: 713075726a3e1db115dfeb48c448e72a8eb7c378af3e2598094a021bc21ce0fd
+    md5: c34d9325a609381a0b0e8a5b4f325147
+    sha256: c71cb65ac49692adb33735f3114b99a96c0c5140db1d56cf4ccef4fe92ea9a4c
   manager: conda
   name: websocket-client
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.0-pyhd8ed1ab_0.conda
-  version: 1.6.0
+  url: https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda
+  version: 1.6.1
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
     md5: 49bb0d9e60ce1db25e151780331bb5f3
     sha256: 79b4d29b0c004014a2abd5fc2c9fcd35cc6256222b960c2a317a27c4b0d8884d
   manager: conda
@@ -15090,22 +15133,22 @@
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda
   version: 0.40.0
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
-    md5: bcc54b91a8ce88f60f538b87b409909e
-    sha256: c63d6e1a51593895dec44931fb2396cfb80e8454d3c7062311a6194032c9b47e
+    md5: 2e9ebddf0b93d0fb203d0906b8052c4f
+    sha256: a73d34f8169e206bccfb356c093ff5ced803b953bbcc1480ed27976f97598d68
   manager: conda
   name: widgetsnbextension
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda
-  version: 4.0.7
+  url: https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.8-pyhd8ed1ab_0.conda
+  version: 4.0.8
 - category: main
   dependencies:
     python: '>=3.5'
   hash:
     md5: dc80c0c2b01f7d6d6d5df4b63ef54f17
     sha256: b2c4dfa3dcf888b9449a4a2fd480b2db4e9167838d91df15fe745f9ba7adff95
   manager: conda
@@ -15298,22 +15341,22 @@
   version: 2.12.1
 - category: main
   dependencies:
     backports: ''
     python: '>=3.6'
     setuptools: ''
   hash:
-    md5: c5b3edc62d6309088f4970b3eaaa65a6
-    sha256: fdea00d4b79990f3fe938e2716bc32bd895eb5c44b6c75b8261db095a1b33c16
+    md5: 6b1b907661838a75d067a22f87996b2e
+    sha256: 7027bb689dd4ca4a08e3b25805de9d04239be6b31125993558f21f102a9d2700
   manager: conda
   name: backports.functools_lru_cache
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.4-pyhd8ed1ab_0.tar.bz2
-  version: 1.6.4
+  url: https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda
+  version: 1.6.5
 - category: main
   dependencies:
     python: '>=3.6'
     soupsieve: '>=1.2'
   hash:
     md5: a362ff7d976217f8fa78c0f1c4f59717
     sha256: 52d3e6bcd442537e22699cd227d8fdcfd54b708eeb8ee5b4c671a6a9b9cd74da
@@ -15337,28 +15380,28 @@
   name: bleach
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda
   version: 6.0.0
 - category: main
   dependencies:
-    brotli-bin: 1.0.9 hcfcfb64_8
-    libbrotlidec: 1.0.9 hcfcfb64_8
-    libbrotlienc: 1.0.9 hcfcfb64_8
+    brotli-bin: 1.0.9 hcfcfb64_9
+    libbrotlidec: 1.0.9 hcfcfb64_9
+    libbrotlienc: 1.0.9 hcfcfb64_9
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
-    vs2015_runtime: '>=14.29.30139'
+    vc14_runtime: '>=14.29.30139'
   hash:
-    md5: 2e661f21e1741c11506bdc7226e6b0bc
-    sha256: 6d2fc2f147c9fc6685124d984089683988729463193578ba1d62f80263bce3c5
+    md5: 5275e2634840f6d156934a16b7c0c813
+    sha256: 7bfc2b4002463dd69d140ab1b46bb36987581252d19af08b5eb9611e339cd7a3
   manager: conda
   name: brotli
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/brotli-1.0.9-hcfcfb64_8.tar.bz2
+  url: https://conda.anaconda.org/conda-forge/win-64/brotli-1.0.9-hcfcfb64_9.conda
   version: 1.0.9
 - category: main
   dependencies:
     pycparser: ''
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     ucrt: '>=10.0.20348.0'
@@ -15491,30 +15534,30 @@
   name: glib-tools
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/glib-tools-2.76.3-h12be248_0.conda
   version: 2.76.3
 - category: main
   dependencies:
-    libgrpc: 1.55.1 h0c1e3fa_1
+    libgrpc: 1.56.0 hea2d5f7_2
     libzlib: '>=1.2.13,<1.3.0a0'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
   hash:
-    md5: 30bee6092170c8b57d96b90baa25d176
-    sha256: 8a3e9e88558f5470cf02dc56b7806377c8a13d5a9c7beb80c6038e3be9e63f99
+    md5: c624ac3dd1ada404b8d8cc378bb60daf
+    sha256: b53354f228f80551ef7326cf108197c4a362334e5e1ef6695cd0532db87c99f0
   manager: conda
   name: grpcio
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/grpcio-1.55.1-py310hb84602e_1.conda
-  version: 1.55.1
+  url: https://conda.anaconda.org/conda-forge/win-64/grpcio-1.56.0-py310hb84602e_2.conda
+  version: 1.56.0
 - category: main
   dependencies:
     libglib: '>=2.76.3,<3.0a0'
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
   hash:
@@ -15654,22 +15697,22 @@
   version: '1.13'
 - category: main
   dependencies:
     packaging: '>=17.1'
     python: '>=3.8'
     typing_extensions: ''
   hash:
-    md5: ad16f58b64d3b41f4cbb75040b06c9cc
-    sha256: 8c1fff22ab86c85768e65dc8c4f4664787476a21f4d934c4e0261a1fa7523f9c
+    md5: c71f7ec8b80a536e58b979299b230251
+    sha256: 9c866f31ff7a02cc70b306f65b1a81eabf84826b0d32c1f51e0ece17cfcdaf79
   manager: conda
   name: lightning-utilities
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/lightning-utilities-0.8.0-pyhd8ed1ab_0.conda
-  version: 0.8.0
+  url: https://conda.anaconda.org/conda-forge/noarch/lightning-utilities-0.9.0-pyhd8ed1ab_0.conda
+  version: 0.9.0
 - category: main
   dependencies:
     python: '>=3.6'
     uc-micro-py: '>=1.0.1,<2.0.0'
   hash:
     md5: 25b93e66067eb496ac10da888e25cc33
     sha256: 0980092a2e0a4bd263c18fb0db701589fc10fc8542ce511f844a533490d5f14e
@@ -15779,31 +15822,31 @@
   name: proj
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/proj-9.1.0-h3863b3b_0.tar.bz2
   version: 9.1.0
 - category: main
   dependencies:
-    libabseil: '>=20230125.2,<20230126.0a0'
-    libprotobuf: '>=4.23.2,<4.23.3.0a0'
+    libabseil: '>=20230125.3,<20230126.0a0'
+    libprotobuf: '>=4.23.3,<4.23.4.0a0'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     setuptools: ''
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
   hash:
-    md5: e2a566087d11bbcf502aeaffdd37fe3d
-    sha256: cb7c97fd41e196d39357f7657d38a6e05f899d8615b515610c6c660024bad7d8
+    md5: a65f902a101c1ec7bedfe48b65756379
+    sha256: ebb697fed21b185a1b2a8611f869d517da86de007c7e814acc6d5838cd2d7b8e
   manager: conda
   name: protobuf
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/protobuf-4.23.2-py310ha3d488f_1.conda
-  version: 4.23.2
+  url: https://conda.anaconda.org/conda-forge/win-64/protobuf-4.23.3-py310ha3d488f_0.conda
+  version: 4.23.3
 - category: main
   dependencies:
     pyasn1: '>=0.4.6,<0.5.0'
     python: ''
   hash:
     md5: ad1e886d09700b2304975335f714bd9c
     sha256: 21f5d8ebf36ad2841028b7358b6b316441493d923045156e9c0e07eb62780e44
@@ -16444,22 +16487,22 @@
   url: https://conda.anaconda.org/conda-forge/win-64/pillow-9.2.0-py310hd4fb230_3.tar.bz2
   version: 9.2.0
 - category: main
   dependencies:
     python: '>=3.7'
     typing-extensions: '>=4.6.3'
   hash:
-    md5: 741384b21c1b512617f4ee4ea8457c5d
-    sha256: ba254f8e7bc01586779c40d040ee000627cddc57965ccbcdb155936c534520d6
+    md5: 3e4aca765371893ad848397794600632
+    sha256: 5f382d0d3509784152506e0e022bb5a30d254555e809804491207196f890af67
   manager: conda
   name: platformdirs
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.6.0-pyhd8ed1ab_0.conda
-  version: 3.6.0
+  url: https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.8.0-pyhd8ed1ab_0.conda
+  version: 3.8.0
 - category: main
   dependencies:
     latexcodec: '>=1.0.4'
     python: '>=3.6'
     pyyaml: '>=3.01'
     setuptools: ''
     six: ''
@@ -16530,22 +16573,22 @@
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     typing-extensions: '>=4.2.0'
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
   hash:
-    md5: 650d1be95b2cba2e37d0a0fe13f3c509
-    sha256: 89eefcf3696e962aa3e98b0ea8475f12b8e159922de5d9c01040237d7e53cbe1
+    md5: 1a7ef45ab2cbed2272dc7bed9ee6f98a
+    sha256: 97cac75adba50a7fe35ae1abf29d5900e92f06f1ed08fc18ae5bfb4ea78175f1
   manager: conda
   name: sqlalchemy
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/sqlalchemy-2.0.16-py310h8d17308_0.conda
-  version: 2.0.16
+  url: https://conda.anaconda.org/conda-forge/win-64/sqlalchemy-2.0.17-py310h8d17308_0.conda
+  version: 2.0.17
 - category: main
   dependencies:
     asttokens: ''
     executing: ''
     pure_eval: ''
     python: '>=3.5'
   hash:
@@ -16658,28 +16701,29 @@
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/black-22.3.0-pyhd8ed1ab_0.tar.bz2
   version: 22.3.0
 - category: main
   dependencies:
     gettext: '>=0.21.1,<1.0a0'
-    glib: '>=2.76.2,<3.0a0'
-    libglib: '>=2.76.2,<3.0a0'
+    glib: '>=2.76.3,<3.0a0'
+    libglib: '>=2.76.3,<3.0a0'
+    libiconv: '>=1.17,<2.0a0'
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
   hash:
-    md5: 00afb31665a8028ca2ff9af61fea64e1
-    sha256: 328c1ddd1328d7419d827cf18e05522011337739302f332847f2d9d731f68d14
+    md5: ead79af9af7587ca3f685fed4966a881
+    sha256: c8473fd20f328fcb1840ce402fc3876b004e14370cb9509ae0220ffad3fce14e
   manager: conda
   name: gstreamer
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/gstreamer-1.22.3-h6b5321d_1.conda
-  version: 1.22.3
+  url: https://conda.anaconda.org/conda-forge/win-64/gstreamer-1.22.4-hb4038d2_0.conda
+  version: 1.22.4
 - category: main
   dependencies:
     cairo: '>=1.16.0,<2.0a0'
     freetype: '>=2.12.1,<3.0a0'
     graphite2: ''
     icu: '>=70.1,<71.0a0'
     libglib: '>=2.74.1,<3.0a0'
@@ -16770,22 +16814,22 @@
   url: https://conda.anaconda.org/conda-forge/noarch/oauthlib-3.2.2-pyhd8ed1ab_0.tar.bz2
   version: 3.2.2
 - category: main
   dependencies:
     python: '>=3.7'
     wcwidth: ''
   hash:
-    md5: 59ba1bf8ea558751a0d391249a248765
-    sha256: 78c2f3c6195ec350d7d6e5fa3e43274ca8191c181c97a867e2920faaeec0e9bc
+    md5: a4986c6bb5b0d05a38855b0880a5f425
+    sha256: 10e7fdc75d4b85633be6b12a70b857053987127a808caa0f88b2cba4b3ce6359
   manager: conda
   name: prompt-toolkit
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda
-  version: 3.0.38
+  url: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda
+  version: 3.0.39
 - category: main
   dependencies:
     docutils: '>=0.8'
     pybtex: '>=0.16'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     setuptools: ''
@@ -16875,48 +16919,49 @@
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/flake8-black-0.3.6-pyhd8ed1ab_0.conda
   version: 0.3.6
 - category: main
   dependencies:
     gettext: '>=0.21.1,<1.0a0'
-    gstreamer: 1.22.3 h6b5321d_1
-    libglib: '>=2.76.2,<3.0a0'
+    gstreamer: 1.22.4 hb4038d2_0
+    libglib: '>=2.76.3,<3.0a0'
+    libogg: '>=1.3.4,<1.4.0a0'
     libvorbis: '>=1.3.7,<1.4.0a0'
     libzlib: '>=1.2.13,<1.3.0a0'
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
   hash:
-    md5: bd6347f397891bf4eb264c652221507c
-    sha256: 5a9c3032a033d1cacf313527e1f492e17492d121c07c3f8213ffede1fef60d09
+    md5: 2c402e044af28ad8eccf03031c5c34c4
+    sha256: e173661c30f46d2baac980320cc53ce5f86c2d48994d895d39cdec7af825b878
   manager: conda
   name: gst-plugins-base
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/gst-plugins-base-1.22.3-h001b923_1.conda
-  version: 1.22.3
+  url: https://conda.anaconda.org/conda-forge/win-64/gst-plugins-base-1.22.4-h001b923_0.conda
+  version: 1.22.4
 - category: main
   dependencies:
     importlib_metadata: '>=4.8.3'
     jupyter_core: '>=4.12,!=5.0.*'
     python: '>=3.8'
     python-dateutil: '>=2.8.2'
     pyzmq: '>=23.0'
     tornado: '>=6.2'
     traitlets: '>=5.3'
   hash:
-    md5: 58ca2d50c3b27b86fd7df62eaadbf9a9
-    sha256: c36c0e9da3a23e89fc30333760f9c9fdb1a14ca2862fa1e1257f7fe4d508fded
+    md5: 1d018ee4ab13217e2544f795eb0a6798
+    sha256: 7dc74a032daefbdcf4d6d661616dfdc8649e5cf9db58258afe91cc09ea0cf402
   manager: conda
   name: jupyter_client
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.2.0-pyhd8ed1ab_0.conda
-  version: 8.2.0
+  url: https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda
+  version: 8.3.0
 - category: main
   dependencies:
     libblas: 3.9.0 17_win64_mkl
   hash:
     md5: 768b2c3be666ecf9e62f939ea919f819
     sha256: 5b9914c3b95d947a613a9b6d3c1c1515257a61e7838a1f2484927f0c9fe23063
   manager: conda
@@ -16970,24 +17015,24 @@
   name: pango
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/pango-1.50.14-hdffb7b3_0.conda
   version: 1.50.14
 - category: main
   dependencies:
-    prompt-toolkit: '>=3.0.38,<3.0.39.0a0'
+    prompt-toolkit: '>=3.0.39,<3.0.40.0a0'
   hash:
-    md5: 45b74f64d8808eda7e6f6e6b1d641fd2
-    sha256: c0f24a75d27918eb33f86902aa6024783d128a89eb3a169bcb22f24163a422b3
+    md5: 4bbbe67d5df19db30f04b8e344dc9976
+    sha256: 89f7fecc7355181dbc2ab851e668a2fce6aa4830b336a34c93b59bda93206270
   manager: conda
   name: prompt_toolkit
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda
-  version: 3.0.38
+  url: https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.39-hd8ed1ab_0.conda
+  version: 3.0.39
 - category: main
   dependencies:
     brotlipy: '>=0.6.0'
     certifi: ''
     cryptography: '>=1.3.4'
     idna: '>=2.0.0'
     pyopenssl: '>=0.14'
@@ -17003,22 +17048,22 @@
   url: https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.15-pyhd8ed1ab_0.conda
   version: 1.26.15
 - category: main
   dependencies:
     aiohttp: <4
     python: '>=3.6'
   hash:
-    md5: 70f4b52c0e703936aa1812d8b14a5bb2
-    sha256: 11dd5e6c5062e788160167e2a64fcbbb2c7ec825e28d628a9e7771172e039de7
+    md5: 0d0113b67472cea3da288838ebc80acb
+    sha256: 656947c8457d5ac06f11dc1da904ac7ac8ac8edf81323ee9794a3d51ace79ff3
   manager: conda
   name: wslink
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/wslink-1.11.0-pyhd8ed1ab_0.conda
-  version: 1.11.0
+  url: https://conda.anaconda.org/conda-forge/noarch/wslink-1.11.1-pyhd8ed1ab_0.conda
+  version: 1.11.1
 - category: main
   dependencies:
     m2w64-gcc-libs: ''
     m2w64-gcc-libs-core: ''
     xorg-libx11: '>=1.8.4,<2.0a0'
     xorg-libxext: '>=1.3.4,<2.0a0'
     xorg-libxt: '>=1.2.1,<2.0a0'
@@ -17036,22 +17081,22 @@
 - category: main
   dependencies:
     jmespath: '>=0.7.1,<2.0.0'
     python: '>=3.7'
     python-dateutil: '>=2.1,<3.0.0'
     urllib3: '>=1.25.4,<1.27'
   hash:
-    md5: ccfde1c6ce8dbb4af5590c88a0482248
-    sha256: b818c4a738c58fcc1ca231f75bfbfdd516b44e437a460336bdbee70a9a4573ca
+    md5: 0f30016ea54215fdb883b8978340c9b7
+    sha256: ccbd3413915259825a678707b438e7ba25712d9c8c5748d2d82f24359237b3f9
   manager: conda
   name: botocore
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/botocore-1.29.158-pyhd8ed1ab_0.conda
-  version: 1.29.158
+  url: https://conda.anaconda.org/conda-forge/noarch/botocore-1.29.165-pyhd8ed1ab_0.conda
+  version: 1.29.165
 - category: main
   dependencies:
     __win: ''
     backcall: ''
     colorama: ''
     decorator: ''
     jedi: '>=0.16'
@@ -17233,44 +17278,44 @@
     python: '>=3.6'
     pyu2f: '>=0.1.5'
     requests: '>=2.20.0,<3.0.0dev'
     rsa: '>=3.1.4,<5'
     six: '>=1.9.0'
     urllib3: <2.0
   hash:
-    md5: 59f942ef9326d2519a7c953f1c24d5da
-    sha256: ba9136edf49c8aa53f45ddfe0c16387bf375f1e5e27f50e39cc1e41c6f5ad25d
+    md5: 8c5dd8609d314721d990c1d1fd607f81
+    sha256: 6b097ca9b31961d6a983f81dc295012e9c99c4c1a5a83a93ab2fcc6528af428f
   manager: conda
   name: google-auth
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/google-auth-2.20.0-pyh1a96a4e_0.conda
-  version: 2.20.0
+  url: https://conda.anaconda.org/conda-forge/noarch/google-auth-2.21.0-pyh1a96a4e_0.conda
+  version: 2.21.0
 - category: main
   dependencies:
     cairo: '>=1.16.0,<2.0a0'
+    expat: '>=2.5.0,<3.0a0'
     getopt-win32: '>=0.1,<0.2.0a0'
     gts: '>=0.7.6,<0.8.0a0'
-    libexpat: '>=2.5.0,<3.0a0'
     libgd: '>=2.3.3,<2.4.0a0'
-    libglib: '>=2.76.2,<3.0a0'
-    libwebp-base: '>=1.3.0,<2.0a0'
-    pango: '>=1.50.14,<2.0a0'
+    libglib: '>=2.74.1,<3.0a0'
+    libwebp-base: '>=1.2.4,<2.0a0'
+    pango: '>=1.50.12,<2.0a0'
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
-    vc14_runtime: '>=14.29.30139'
+    vs2015_runtime: '>=14.29.30139'
   hash:
-    md5: ddd4c41fe063b15f4b8e0632dce89ef6
-    sha256: d5cf66c5979bb970484157bd5b9131c4958f1ba572567080ee09f6bc229515dd
+    md5: 136eb298a1c96b07f935dd0525fbd11c
+    sha256: 692b542a527973652ae3b224758a02c668ee93f55519ae723d77d06f0e1dcead
   manager: conda
   name: graphviz
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/graphviz-8.0.5-h51cb2cd_0.conda
-  version: 8.0.5
+  url: https://conda.anaconda.org/conda-forge/win-64/graphviz-7.0.6-h51cb2cd_0.conda
+  version: 7.0.6
 - category: main
   dependencies:
     __win: ''
     comm: '>=0.1.1'
     debugpy: '>=1.6.5'
     ipython: '>=7.23.1'
     jupyter_client: '>=6.1.12'
@@ -17280,22 +17325,22 @@
     packaging: ''
     psutil: ''
     python: '>=3.8'
     pyzmq: '>=20'
     tornado: '>=6.1'
     traitlets: '>=5.4.0'
   hash:
-    md5: e67aced0f12f38ced65e9d428dd1cff1
-    sha256: 3623664dd253d51799f41772f318977e234a51298340911ec43b417d59ddc049
+    md5: b71d6766fc67ea676f75d121965da056
+    sha256: 4f9a2edf8b0e9d7e09c97487b9f10b87abc250b1b1524e67e02d82086b68691a
   manager: conda
   name: ipykernel
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.2-pyh6817e22_0.conda
-  version: 6.23.2
+  url: https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.3-pyh6817e22_0.conda
+  version: 6.23.3
 - category: main
   dependencies:
     attrs: ''
     click: ''
     importlib-metadata: ''
     nbclient: '>=0.2,<0.8'
     nbformat: ''
@@ -17512,59 +17557,59 @@
   name: blas
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/blas-2.117-mkl.conda
   version: '2.117'
 - category: main
   dependencies:
-    botocore: '>=1.29.158,<1.30.0'
+    botocore: '>=1.29.165,<1.30.0'
     jmespath: '>=0.7.1,<2.0.0'
     python: '>=3.7'
     s3transfer: '>=0.6.0,<0.7.0'
   hash:
-    md5: 2e39307a3987518e49eb30ca51e3cfb5
-    sha256: b22c2838e528d03d670f1ecbc57f3d57b4a93d21f456b1248788d7be4e080e3a
+    md5: b9a6316db67d5f2c8dbac2aeb24c6803
+    sha256: 4ca4d8c481609dbf8ce755a8f115486e40be0f0d01c0961c696d6f995dadb2f5
   manager: conda
   name: boto3
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/boto3-1.26.158-pyhd8ed1ab_0.conda
-  version: 1.26.158
+  url: https://conda.anaconda.org/conda-forge/noarch/boto3-1.26.165-pyhd8ed1ab_0.conda
+  version: 1.26.165
 - category: main
   dependencies:
     click: '>=6.0.0'
-    google-auth: '>=1.0.0'
+    google-auth: '>=2.15.0'
     python: '>=3.6'
     requests-oauthlib: '>=0.7.0'
   hash:
-    md5: 5ba9d95acb9add67f468ecdee6595c0f
-    sha256: ef8edcbc8efe616d0f3686607f445a6a96f3549ce2faed1797ad35ca5cd42e81
+    md5: 569e62e95b01b53e4ec7d9abe83b7385
+    sha256: f89613643658a51a1ac0fb7c7950526fadc2a6ce1ae13755d786e14cfce1633c
   manager: conda
   name: google-auth-oauthlib
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/google-auth-oauthlib-1.0.0-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/google-auth-oauthlib-1.0.0-pyhd8ed1ab_1.conda
   version: 1.0.0
 - category: main
   dependencies:
     ipykernel: '>=4.5.1'
     ipython: '>=6.1.0'
-    jupyterlab_widgets: '>=3.0.7,<4.1.dev0'
+    jupyterlab_widgets: '>=3.0.7,<3.1.0'
     python: '>=3.7'
     traitlets: '>=4.3.1'
-    widgetsnbextension: '>=4.0.7,<4.1.dev0'
+    widgetsnbextension: '>=4.0.7,<4.1.0'
   hash:
-    md5: 68627a08556e4a273e4c7bfc84251457
-    sha256: a18f168f368cc8ba4d11a83bf57fcd664bd311a0fcc9b36c283715470f43c133
+    md5: 4b0f4e8fe2a303e472674eae0340bdad
+    sha256: 3b17ad90294f0684fca9191f1e696e9b4f03a652d5e588b6ff0feb5647fcf116
   manager: conda
   name: ipywidgets
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.6-pyhd8ed1ab_0.conda
-  version: 8.0.6
+  url: https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.7-pyhd8ed1ab_0.conda
+  version: 8.0.7
 - category: main
   dependencies:
     ipykernel: '>=6.14'
     ipython: ''
     jupyter_client: '>=7.0.0'
     jupyter_core: '>=4.12,!=5.0.*'
     prompt_toolkit: '>=3.0.30'
@@ -17599,22 +17644,22 @@
     pyzmq: '>=24'
     send2trash: ''
     terminado: '>=0.8.3'
     tornado: '>=6.2.0'
     traitlets: '>=5.6.0'
     websocket-client: ''
   hash:
-    md5: 39fd52b0fcb2fb52bac47a1419bf09bd
-    sha256: 0f0feb284f667964d1e4122a7690f6e3ace257732591a6151fdd1eb797911128
+    md5: 7488cd1f4d35a2af96faa765b7e5b2f0
+    sha256: 132bfa3eef62231e53b59d93358f818a97c5e7939670bfdd821b7146a0094e43
   manager: conda
   name: jupyter_server
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.6.0-pyhd8ed1ab_0.conda
-  version: 2.6.0
+  url: https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.7.0-pyhd8ed1ab_0.conda
+  version: 2.7.0
 - category: main
   dependencies:
     certifi: '>=2020.06.20'
     contourpy: '>=1.0.1'
     cycler: '>=0.10'
     fonttools: '>=4.22.0'
     freetype: '>=2.12.1,<3.0a0'
@@ -18173,14 +18218,34 @@
   name: torchmetrics
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/torchmetrics-0.11.4-pyhd8ed1ab_0.conda
   version: 0.11.4
 - category: main
   dependencies:
+    jpeg: ''
+    libpng: ''
+    numpy: '>=1.11'
+    pillow: '>=5.3.0,!=8.3.*'
+    python: '>=3.10,<3.11.0a0'
+    pytorch: 2.0.1
+    pytorch-cuda: 11.8.*
+    pytorch-mutex: 1.0 cuda
+    requests: ''
+  hash:
+    md5: 140ec95434b375beaa3b12159b9f0caf
+    sha256: f47cbfe72f103ec58d46cb16f77a5b57be4706b6656560301ad64c4df5ef88a4
+  manager: conda
+  name: torchvision
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/pytorch/win-64/torchvision-0.15.2-py310_cu118.tar.bz2
+  version: 0.15.2
+- category: main
+  dependencies:
     argon2-cffi: ''
     ipykernel: ''
     ipython_genutils: ''
     jinja2: ''
     jupyter_client: '>=5.3.4'
     jupyter_core: '>=4.6.1'
     nbclassic: '>=0.4.7'
@@ -18213,22 +18278,22 @@
     pytorch: '>=1.11.0'
     pyyaml: '>=5.4'
     requests: ''
     torchmetrics: '>=0.7.0'
     tqdm: '>=4.57.0'
     typing_extensions: '>=4.0.0'
   hash:
-    md5: 97138eb8783fa54884216a6562413736
-    sha256: d2b5fbd636393c71dfc07ce5a15eb36285b01aaa34453b3fd8b9b26f0fa5b689
+    md5: ce9d626b181c6f8cceb5047f6a819f7d
+    sha256: a049296b4b33bceedf3bafd378e8a4112bca71b453734f1e0daaca2a72598593
   manager: conda
   name: pytorch-lightning
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pytorch-lightning-2.0.3-pyhd8ed1ab_0.conda
-  version: 2.0.3
+  url: https://conda.anaconda.org/conda-forge/noarch/pytorch-lightning-2.0.4-pyhd8ed1ab_0.conda
+  version: 2.0.4
 - category: main
   dependencies:
     ipykernel: ''
     ipywidgets: ''
     jupyter_console: ''
     nbconvert: ''
     notebook: ''
```

### Comparing `hf-deepali-0.3.1/conda/environment.devenv.yml` & `hf-deepali-0.3.2/conda/environment.devenv.yml`

 * *Files 8% similar despite different names*

```diff
@@ -45,10 +45,11 @@
   - boto3 =1.26
   - matplotlib =3.7
   - scipy =1.10
   - tensorboard =2.13
   - vtk =9.2
   # Examples / Tutorials
   - pytorch-lightning =2.0
+  - torchvision =0.15
   # Tests
   - torchinfo =1.8
 name: deepali
```

### Comparing `hf-deepali-0.3.1/conda/environment.linux-64.lock` & `hf-deepali-0.3.2/conda/environment.linux-64.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Generated by conda-lock.
 # platform: linux-64
-# input_hash: 404e905e5633264d344750350dd433b9a664952c8bd3a8255d3f31d9eb8a74d7
+# input_hash: 8bbc0023a299b67380a6493155cba6c46fd177739fbaea7c67b86663b42d8354
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2#d7c89558ba9fa0495403155b64376d81
 https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2023.5.7-hbcca054_0.conda#f5c65075fc34438d5b456c7f3f5ab695
 https://conda.anaconda.org/nvidia/linux-64/cuda-cudart-11.8.89-0.tar.bz2#b68c7ef3eda01e95d5903fb508c5e440
 https://conda.anaconda.org/nvidia/linux-64/cuda-cupti-11.8.87-0.tar.bz2#2f4b4933285400137cf029fef9a7daa6
 https://conda.anaconda.org/nvidia/linux-64/cuda-nvrtc-11.8.89-0.tar.bz2#f4af75ee32661708c979630cdb8f4987
 https://conda.anaconda.org/nvidia/linux-64/cuda-nvtx-11.8.86-0.tar.bz2#1825ffc3feb608f2752073935e90bb49
@@ -49,17 +49,17 @@
 https://conda.anaconda.org/conda-forge/linux-64/gstreamer-orc-0.4.34-hd590300_0.conda#7ea223fa114cc8134b8c4d398d3e5afe
 https://conda.anaconda.org/conda-forge/linux-64/icu-70.1-h27087fc_0.tar.bz2#87473a15119779e021c314249d4b4aed
 https://conda.anaconda.org/conda-forge/linux-64/jpeg-9e-h0b41bf4_3.conda#c7a069243e1fbe9a556ed2ec030e6407
 https://conda.anaconda.org/conda-forge/linux-64/jsoncpp-1.9.5-h4bd325d_1.tar.bz2#ae7f50dd1e78c7e78b5d2cf7062e559d
 https://conda.anaconda.org/conda-forge/linux-64/keyutils-1.6.1-h166bdaf_0.tar.bz2#30186d27e2c9fa62b45fb1476b7200e3
 https://conda.anaconda.org/conda-forge/linux-64/lame-3.100-h166bdaf_1003.tar.bz2#a8832b479f93521a9e7b5b743803be51
 https://conda.anaconda.org/conda-forge/linux-64/lerc-4.0.0-h27087fc_0.tar.bz2#76bbff344f0134279f225174e9064c8f
-https://conda.anaconda.org/conda-forge/linux-64/libabseil-20230125.2-cxx17_h59595ed_2.conda#f67106643beadfc737b94ca0bfd6d8e3
+https://conda.anaconda.org/conda-forge/linux-64/libabseil-20230125.3-cxx17_h59595ed_0.conda#d1db1b8be7c3a8983dcbbbfe4f0765de
 https://conda.anaconda.org/conda-forge/linux-64/libaec-1.0.6-hcb278e6_1.conda#0f683578378cddb223e7fd24f785ab2a
-https://conda.anaconda.org/conda-forge/linux-64/libbrotlicommon-1.0.9-h166bdaf_8.tar.bz2#9194c9bf9428035a05352d031462eae4
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlicommon-1.0.9-h166bdaf_9.conda#61641e239f96eae2b8492dc7e755828c
 https://conda.anaconda.org/conda-forge/linux-64/libcufile-1.5.0.59-hcb278e6_0.conda#73fe585c1d401a3dbb39473cce1b7cc2
 https://conda.anaconda.org/conda-forge/linux-64/libcurand-10.3.1.50-hcb278e6_0.conda#52cd5b96f2385d5f6b706fa96553af66
 https://conda.anaconda.org/conda-forge/linux-64/libdb-6.2.32-h9c3ff4c_0.tar.bz2#3f3258d8f841fbac63b36b75bdac1afd
 https://conda.anaconda.org/conda-forge/linux-64/libdeflate-1.14-h166bdaf_0.tar.bz2#fc84a0446e4e4fb882e78d786cfb9734
 https://conda.anaconda.org/conda-forge/linux-64/libev-4.33-h516909a_1.tar.bz2#6f8720dff19e17ce5d48cfe7f3d2f0a3
 https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.5.0-hcb278e6_1.conda#6305a3dd2752c76335295da4e581f2fd
 https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
@@ -100,112 +100,112 @@
 https://conda.anaconda.org/conda-forge/linux-64/xorg-xextproto-7.3.0-h0b41bf4_1003.conda#bce9f945da8ad2ae9b1d7165a64d0f87
 https://conda.anaconda.org/conda-forge/linux-64/xorg-xproto-7.0.31-h7f98852_1007.tar.bz2#b4a4381d54784606820704f7b5f05a15
 https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2#2161070d867d1b1204ea749c8eec4ef0
 https://conda.anaconda.org/conda-forge/linux-64/yaml-0.2.5-h7f98852_2.tar.bz2#4cb3ad778ec2d5a7acbdf254eb1c42ae
 https://conda.anaconda.org/nvidia/linux-64/cuda-libraries-11.8.0-0.tar.bz2#3a43d100104e52ac8209a834c82ab231
 https://conda.anaconda.org/conda-forge/linux-64/expat-2.5.0-hcb278e6_1.conda#8b9b5aca60558d02ddaa09d599e55920
 https://conda.anaconda.org/conda-forge/linux-64/jack-1.9.22-h11f4161_0.conda#504fa9e712b99494a9cf4630e3ca7d78
-https://conda.anaconda.org/conda-forge/linux-64/libbrotlidec-1.0.9-h166bdaf_8.tar.bz2#4ae4d7795d33e02bd20f6b23d91caf82
-https://conda.anaconda.org/conda-forge/linux-64/libbrotlienc-1.0.9-h166bdaf_8.tar.bz2#04bac51ba35ea023dc48af73c1c88c25
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlidec-1.0.9-h166bdaf_9.conda#081aa22f4581c08e4372b0b6c2f8478e
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlienc-1.0.9-h166bdaf_9.conda#1f0a03af852a9659ed2bf08f2f1704fd
 https://conda.anaconda.org/conda-forge/linux-64/libcap-2.67-he9d0100_0.conda#d05556c80caffff164d17bdea0105a1a
 https://conda.anaconda.org/conda-forge/linux-64/libdrm-2.4.114-h166bdaf_0.tar.bz2#efb58e80f5d0179a783c4e76c3df3b9c
 https://conda.anaconda.org/conda-forge/linux-64/libedit-3.1.20191231-he28a2e2_2.tar.bz2#4d331e44109e3f0e19b4cb8f9b82f3e1
 https://conda.anaconda.org/conda-forge/linux-64/libevent-2.1.10-h28343ad_4.tar.bz2#4a049fc560e00e43151dc51368915fdd
-https://conda.anaconda.org/conda-forge/linux-64/libflac-1.4.2-h27087fc_0.tar.bz2#7daf72d8e2a8e848e11d63ed6d1026e0
+https://conda.anaconda.org/conda-forge/linux-64/libflac-1.4.3-h59595ed_0.conda#ee48bf17cc83a00f59ca1494d5646869
 https://conda.anaconda.org/conda-forge/linux-64/libgpg-error-1.47-h71f35ed_0.conda#c2097d0b46367996f09b4e8e4920384a
 https://conda.anaconda.org/conda-forge/linux-64/libidn2-2.3.4-h166bdaf_0.tar.bz2#7440fbafd870b8bab68f83a064875d34
 https://conda.anaconda.org/conda-forge/linux-64/libnghttp2-1.52.0-h61bc06f_0.conda#613955a50485812985c059e7b269f42e
 https://conda.anaconda.org/conda-forge/linux-64/libpng-1.6.39-h753d276_0.conda#e1c890aebdebbfbf87e2c917187b4416
-https://conda.anaconda.org/conda-forge/linux-64/libprotobuf-4.23.2-hd1fb520_5.conda#40e9b664b20732e651178d0ea29ae2a5
+https://conda.anaconda.org/conda-forge/linux-64/libprotobuf-4.23.3-hd1fb520_0.conda#c8da7f04073ed0fabcb60885a4c1a722
 https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.42.0-h2797004_0.conda#fdaae20a1cf7cd62130a0973190a31b7
 https://conda.anaconda.org/conda-forge/linux-64/libssh2-1.11.0-h0841786_0.conda#1f5a58e686b13bcfde88b93f547d23fe
 https://conda.anaconda.org/conda-forge/linux-64/libvorbis-1.3.7-h9c3ff4c_0.tar.bz2#309dec04b70a3cc0f1e84a4013683bc0
 https://conda.anaconda.org/conda-forge/linux-64/libxcb-1.13-h7f98852_1004.tar.bz2#b3653fdc58d03face9724f602218a904
 https://conda.anaconda.org/conda-forge/linux-64/libxml2-2.10.3-hca2bb57_4.conda#bb808b654bdc3c783deaf107a2ffb503
 https://conda.anaconda.org/conda-forge/linux-64/libzip-1.9.2-hc929e4a_1.tar.bz2#5b122b50e738c4be5c3f2899f010d7cf
 https://conda.anaconda.org/conda-forge/linux-64/mpfr-4.2.0-hb012696_0.conda#14d87bdff2cbd3b1179a29fb316ed743
-https://conda.anaconda.org/conda-forge/linux-64/mysql-common-8.0.33-hf1915f5_0.conda#aa8b86066614c4573f6db62c91978fa9
+https://conda.anaconda.org/conda-forge/linux-64/mysql-common-8.0.33-hf1915f5_1.conda#b241363e3b72bae6dfbd31e9fecf7d26
 https://conda.anaconda.org/conda-forge/linux-64/p11-kit-0.24.1-hc5aa10d_0.tar.bz2#56ee94e34b71742bbdfa832c974e47a8
 https://conda.anaconda.org/conda-forge/linux-64/pcre2-10.40-hc3806b6_0.tar.bz2#69e2c796349cd9b273890bee0febfe1b
 https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda#47d31b792659ce70f470b5c82fdfb7a4
 https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.12-h27826a3_0.tar.bz2#5b8c42eb62e9fc961af70bdd6a26e168
 https://conda.anaconda.org/conda-forge/linux-64/xorg-fixesproto-5.0-h7f98852_1002.tar.bz2#65ad6e1eb4aed2b0611855aff05e04f6
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libsm-1.2.3-hd9c2040_1000.tar.bz2#9e856f78d5c80d5a78f61e72d1d473a3
 https://conda.anaconda.org/conda-forge/linux-64/zeromq-4.3.4-h9c3ff4c_1.tar.bz2#21743a8d2ea0c8cfbbf8fe489b0347df
 https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-hd590300_5.conda#68c34ec6149623be41a1933ab996a209
 https://conda.anaconda.org/conda-forge/linux-64/zstd-1.5.2-h3eb15da_6.conda#6b63daed8feeca47be78f323e793d555
-https://conda.anaconda.org/conda-forge/linux-64/brotli-bin-1.0.9-h166bdaf_8.tar.bz2#e5613f2bc717e9945840ff474419b8e4
+https://conda.anaconda.org/conda-forge/linux-64/brotli-bin-1.0.9-h166bdaf_9.conda#d47dee1856d9cb955b8076eeff304a5b
 https://conda.anaconda.org/nvidia/linux-64/cuda-runtime-11.8.0-0.tar.bz2#3ca379d762f8d7bd727df9e2c9b30664
 https://conda.anaconda.org/conda-forge/linux-64/freetype-2.12.1-hca18f0e_1.conda#e1232042de76d24539a436d37597eb06
 https://conda.anaconda.org/conda-forge/linux-64/gl2ps-1.4.2-h0708190_0.tar.bz2#438718bf8921ac70956d919d0e2cc487
 https://conda.anaconda.org/conda-forge/linux-64/gnutls-3.7.8-hf3e180e_0.tar.bz2#cbe8e27140d67c3f30e01cfb642a6e7c
 https://conda.anaconda.org/conda-forge/linux-64/hdf4-4.2.15-h9772cbc_5.tar.bz2#ee08782aff2ff9b3291c967fa6bc7336
 https://conda.anaconda.org/conda-forge/linux-64/krb5-1.20.1-h81ceb04_0.conda#89a41adce7106749573d883b2f657d78
 https://conda.anaconda.org/conda-forge/linux-64/libgcrypt-1.10.1-h166bdaf_0.tar.bz2#f967fc95089cd247ceed56eda31de3a9
 https://conda.anaconda.org/conda-forge/linux-64/libglib-2.76.3-hebfc3b9_0.conda#a64f11b244b2c112cd3fa1cbe9493999
-https://conda.anaconda.org/conda-forge/linux-64/libgrpc-1.55.1-h59456c1_1.conda#5aed976a1e827d49bec1fb5a9819d032
+https://conda.anaconda.org/conda-forge/linux-64/libgrpc-1.56.0-h3905398_2.conda#6cf9ef21c7ef12df628bf46ad67189d3
 https://conda.anaconda.org/conda-forge/linux-64/libhwloc-2.9.1-hd6dc26d_0.conda#a3ede1b8e47f993ff1fe3908b23bb307
 https://conda.anaconda.org/conda-forge/linux-64/libllvm15-15.0.7-hadd5161_1.conda#17d91085ccf5934ce652cb448d0cb65a
 https://conda.anaconda.org/conda-forge/linux-64/libsndfile-1.2.0-hb75c966_0.conda#c648d19cd9c8625898d5d370414de7c7
 https://conda.anaconda.org/conda-forge/linux-64/libtheora-1.1.1-h7f98852_1005.tar.bz2#1a7c35f56343b7e9e8db20b296c7566c
 https://conda.anaconda.org/conda-forge/linux-64/libtiff-4.4.0-h82bc61c_5.conda#e712a63a21f9db647982971dc121cdcf
 https://conda.anaconda.org/conda-forge/linux-64/libudev1-253-h0b41bf4_1.conda#bb38b19a41bb94e8a19dbfb062d499c7
 https://conda.anaconda.org/conda-forge/linux-64/libxkbcommon-1.5.0-h79f4944_1.conda#04a39cdd663f295653fc143851830563
 https://conda.anaconda.org/conda-forge/linux-64/llvm-openmp-16.0.6-h4dfa4b3_0.conda#b096c85c415519259e731d8fb719a3ef
 https://conda.anaconda.org/conda-forge/linux-64/mpc-1.3.1-hfe3b2da_0.conda#289c71e83dc0daa7d4c81f04180778ca
-https://conda.anaconda.org/conda-forge/linux-64/mysql-libs-8.0.33-hca2cd23_0.conda#276339b0115d92c6e0793dcdc7afe308
+https://conda.anaconda.org/conda-forge/linux-64/mysql-libs-8.0.33-hca2cd23_1.conda#a04ac37f0659929f3ba0f33c7f3d750f
 https://conda.anaconda.org/conda-forge/linux-64/nss-3.89-he45b914_0.conda#2745719a58eeaab6657256a3f142f099
 https://conda.anaconda.org/conda-forge/linux-64/pandoc-3.1.3-h32600fe_0.conda#8287aeb8462e2d4b235eff788e75919d
-https://conda.anaconda.org/conda-forge/linux-64/python-3.10.11-he550d4f_0_cpython.conda#7439c9d24378a82b73a7a53868dacdf1
+https://conda.anaconda.org/conda-forge/linux-64/python-3.10.12-hd12c33a_0_cpython.conda#eb6f1df105f37daedd6dca78523baa75
 https://conda.anaconda.org/conda-forge/linux-64/sqlite-3.42.0-h2c6b66d_0.conda#1192f6ec654a5bc4ee1d64bdc4a3e5cc
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-0.4.0-h516909a_0.tar.bz2#a88ab22508ba067b689dc12696157cee
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-keysyms-0.4.0-h516909a_0.tar.bz2#d04a6285315c4f03ebaf37355be272f9
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-renderutil-0.3.9-h166bdaf_0.tar.bz2#732e22f1741bccea861f5668cf7342a7
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-wm-0.4.1-h516909a_0.tar.bz2#847df113dba16f0079758cacf9024409
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libx11-1.8.4-h0b41bf4_0.conda#ea8fbfeb976ac49cbeb594e985393514
 https://conda.anaconda.org/conda-forge/noarch/absl-py-1.4.0-pyhd8ed1ab_0.conda#dd5eed01874c75bebef810a2faec673e
 https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.13-pyhd8ed1ab_0.conda#06006184e203b61d3525f90de394471e
 https://conda.anaconda.org/conda-forge/linux-64/atk-1.0-2.38.0-hd4edc92_1.tar.bz2#6c72ec3e660a51736913ef6ea68c454b
 https://conda.anaconda.org/conda-forge/noarch/attrs-21.4.0-pyhd8ed1ab_0.tar.bz2#f70280205d7044c8b8358c8de3190e5d
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
 https://conda.anaconda.org/conda-forge/noarch/blinker-1.6.2-pyhd8ed1ab_0.conda#2fb79ec81bad9492b6d59a06b3b647a4
-https://conda.anaconda.org/conda-forge/linux-64/brotli-1.0.9-h166bdaf_8.tar.bz2#2ff08978892a3e8b954397c461f18418
-https://conda.anaconda.org/conda-forge/noarch/cachetools-5.3.0-pyhd8ed1ab_0.conda#fd006afc4115740d8d52887ee813f262
+https://conda.anaconda.org/conda-forge/linux-64/brotli-1.0.9-h166bdaf_9.conda#4601544b4982ba1861fa9b9c607b2c06
+https://conda.anaconda.org/conda-forge/noarch/cachetools-5.3.1-pyhd8ed1ab_0.conda#60b5eb16d9a7a5482ba37f67aa49db5b
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2#20e4087407c7cb04a40817114b333dbf
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.11.0-pyhd8ed1ab_0.tar.bz2#a50559fad0affdbb33729a68669ca1cb
 https://conda.anaconda.org/conda-forge/noarch/dataclasses-0.8-pyhc8e2a94_3.tar.bz2#a362b2124b06aad102e2ee4581acee7d
 https://conda.anaconda.org/conda-forge/linux-64/dbus-1.13.6-h5008d03_3.tar.bz2#ecfff944ba3960ecb334b9a2663d708d
 https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.6.7-py310heca2aa9_0.conda#8ffb020d2b722c962f0b4f06a304f533
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
 https://conda.anaconda.org/conda-forge/linux-64/docutils-0.17.1-py310hff52083_3.tar.bz2#785160da087cf1d70e989afbb761f01c
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
-https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
 https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
 https://conda.anaconda.org/conda-forge/noarch/filelock-3.12.2-pyhd8ed1ab_0.conda#53522ec72e6adae42bd373ef58357230
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/linux-64/fontconfig-2.14.2-h14ed4e7_0.conda#0f69b688f52ff6da70bccb7ff7001d1d
 https://conda.anaconda.org/conda-forge/linux-64/frozenlist-1.3.3-py310h5764c6d_0.tar.bz2#25e1626333f9a0646579a162e7b174ee
 https://conda.anaconda.org/conda-forge/noarch/fsspec-2023.6.0-pyh1a96a4e_0.conda#50ea2067ec92dfcc38b4f07992d7e235
 https://conda.anaconda.org/conda-forge/linux-64/gdk-pixbuf-2.42.8-hff1cb4f_1.tar.bz2#a61c6312192e7c9de71548a6706a21e6
 https://conda.anaconda.org/conda-forge/linux-64/glib-tools-2.76.3-hfc55251_0.conda#8951eedf3cdf94dd733c1b5eee1f4880
 https://conda.anaconda.org/conda-forge/linux-64/gmpy2-2.1.2-py310h3ec546c_1.tar.bz2#73f6fa50c32ddd985cf5fba7b890a75c
 https://conda.anaconda.org/conda-forge/linux-64/greenlet-2.0.2-py310hc6cd4ac_1.conda#934c4eb3214284125eff6dd665e9568a
-https://conda.anaconda.org/conda-forge/linux-64/grpcio-1.55.1-py310h1b8f574_1.conda#5292eea84c56fccfebcd51bb0d81eff5
+https://conda.anaconda.org/conda-forge/linux-64/grpcio-1.56.0-py310h1b8f574_2.conda#78282ea7b261ed53a615faba16532e82
 https://conda.anaconda.org/conda-forge/linux-64/gts-0.7.6-h977cf35_4.conda#4d8df0b0db060d33c9a702ada998a8fe
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
 https://conda.anaconda.org/conda-forge/noarch/ipython_genutils-0.2.0-py_1.tar.bz2#5071c982548b3a20caf70462f04f5287
 https://conda.anaconda.org/conda-forge/noarch/jmespath-1.0.1-pyhd8ed1ab_0.tar.bz2#2cfa3e1cf3fb51bb9b17acc5b5e9ea11
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.7-pyhd8ed1ab_1.conda#0c0a54e16b764bafcae35913cc9d60ff
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.8-pyhd8ed1ab_0.conda#2bc3ca2f7387af385dd06706b4fb2d35
 https://conda.anaconda.org/conda-forge/linux-64/kiwisolver-1.4.4-py310hbf28c38_1.tar.bz2#ad5647e517ba68e2868ef2e6e6ff7723
 https://conda.anaconda.org/conda-forge/linux-64/lazy-object-proxy-1.9.0-py310h1fa729e_0.conda#8664f43451412071a7111211fe7e38f2
 https://conda.anaconda.org/conda-forge/linux-64/lcms2-2.14-h6ed2654_0.tar.bz2#dcc588839de1445d90995a0a2c4f3a39
 https://conda.anaconda.org/conda-forge/linux-64/libclang13-15.0.7-default_h9986a30_2.conda#907344cee64101d44d806bbe0fccb01d
 https://conda.anaconda.org/conda-forge/linux-64/libcups-2.3.3-h36d4200_3.conda#c9f4416a34bc91e0eb029f912c68f81f
 https://conda.anaconda.org/conda-forge/linux-64/libcurl-8.1.2-h409715c_0.conda#50c873c9660ed116707ae15b663928d8
 https://conda.anaconda.org/conda-forge/linux-64/libpq-15.3-hbcd7760_1.conda#8afb2a97d256ffde95b91a6283bc598c
@@ -225,15 +225,15 @@
 https://conda.anaconda.org/conda-forge/linux-64/openjpeg-2.5.0-h7d73246_1.tar.bz2#a11b4df9271a8d7917686725aa04c8f2
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
 https://conda.anaconda.org/conda-forge/noarch/pathspec-0.11.1-pyhd8ed1ab_0.conda#dbb80d1e8dc2dba5c8b106dc0768ad45
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
-https://conda.anaconda.org/conda-forge/noarch/pluggy-1.0.0-pyhd8ed1ab_5.tar.bz2#7d301a0d25f424d96175f810935f0da9
+https://conda.anaconda.org/conda-forge/noarch/pluggy-1.2.0-pyhd8ed1ab_0.conda#7263924c642d22e311d9e59b839f1b33
 https://conda.anaconda.org/conda-forge/noarch/ply-3.11-py_1.tar.bz2#7205635cd71531943440fbfe3b6b5727
 https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.0-pyhd8ed1ab_0.conda#95c5be3c7cbd872509d16c216617fdab
 https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.5-py310h1fa729e_0.conda#b0f0a014fc04012c05f39df15fe270ce
 https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
 https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
 https://conda.anaconda.org/conda-forge/noarch/pyasn1-0.4.8-py_0.tar.bz2#06d04c9f8f72ac77911db942eda24fb9
 https://conda.anaconda.org/conda-forge/noarch/pycodestyle-2.10.0-pyhd8ed1ab_0.conda#89843e4cc99c6a3fe5f4c86994cc8410
@@ -266,37 +266,37 @@
 https://conda.anaconda.org/conda-forge/noarch/tabulate-0.9.0-pyhd8ed1ab_1.tar.bz2#4759805cce2d914c38472f70bf4d8bcb
 https://conda.anaconda.org/conda-forge/linux-64/tbb-2021.9.0-hf52228f_0.conda#f495e42d3d2020b025705625edf35490
 https://conda.anaconda.org/conda-forge/linux-64/tensorboard-data-server-0.7.0-py310h34c0648_0.conda#350fb40a1b4820cf02f546dfe6764fe9
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/linux-64/tornado-6.3.2-py310h2372a71_0.conda#1c510e74c87dc9b8fe1f7f9e8dbcef96
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
-https://conda.anaconda.org/conda-forge/linux-64/typed-ast-1.5.4-py310h5764c6d_1.tar.bz2#309cb97f0a3a11a6481453c16e8c5be1
+https://conda.anaconda.org/conda-forge/linux-64/typed-ast-1.5.5-py310h2372a71_0.conda#48d1b46a82b8b4fb6057711dd213977f
 https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.3-pyha770c72_0.conda#4a3014a4d107d15475d106b751c4e352
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/noarch/uc-micro-py-1.0.1-pyhd8ed1ab_0.tar.bz2#3ddf6684d9b274a12c94e509ca45656c
 https://conda.anaconda.org/conda-forge/linux-64/unicodedata2-15.0.0-py310h5764c6d_0.tar.bz2#e972c5a1f472561cf4a91962cb01f4b4
 https://conda.anaconda.org/conda-forge/noarch/unidecode-1.3.6-pyhd8ed1ab_0.tar.bz2#e8f24401b17802df5f82f66a88cee29e
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
-https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.0-pyhd8ed1ab_0.conda#1dd6387a73d84e16b6f73de676bb4c36
+https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda#c34d9325a609381a0b0e8a5b4f325147
 https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
-https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
+https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.8-pyhd8ed1ab_0.conda#2e9ebddf0b93d0fb203d0906b8052c4f
 https://conda.anaconda.org/conda-forge/linux-64/wrapt-1.15.0-py310h1fa729e_0.conda#cbfdcc9c243ac7f080cf60833b482f97
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-image-0.4.0-h166bdaf_0.tar.bz2#c9b568bd804cb2903c6be6f5f68182e4
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxext-1.3.4-h0b41bf4_2.conda#82b6df12252e6f32402b96dacc656fec
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxfixes-5.0.3-h7f98852_1004.tar.bz2#e9a21aa4d5e3e5f1aed71e8cefd46b6a
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxrender-0.9.10-h7f98852_1003.tar.bz2#f59c1242cc1dd93e72c2ee2b360979eb
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxt-1.3.0-hd590300_0.conda#ab2044e8d87dda9f74652e8e084a5569
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
 https://conda.anaconda.org/conda-forge/noarch/accessible-pygments-0.0.4-pyhd8ed1ab_0.conda#46a2e6e3dfa718ce3492018d5a110dd6
 https://conda.anaconda.org/conda-forge/noarch/aiosignal-1.3.1-pyhd8ed1ab_0.tar.bz2#d1e1eb7e21a9e2c74279d87dafb68156
 https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.0-pyhd8ed1ab_1.conda#2b35a85d654a47aac8f34c1bb6de7142
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
-https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.4-pyhd8ed1ab_0.tar.bz2#c5b3edc62d6309088f4970b3eaaa65a6
+https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
 https://conda.anaconda.org/conda-forge/linux-64/cairo-1.16.0-ha61ee94_1014.tar.bz2#d1a88f3ed5b52e1024b80d4bcd26a7a0
 https://conda.anaconda.org/conda-forge/linux-64/cffi-1.15.1-py310h255011f_3.conda#800596144bb613cd7ac58b80900ce835
 https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda#168ae0f82cdf7505048e81054c7354e4
 https://conda.anaconda.org/conda-forge/linux-64/curl-8.1.2-h409715c_0.conda#9f88cfb15b7d08b25880b138f91e0eb4
 https://conda.anaconda.org/conda-forge/noarch/dacite-1.8.0-pyhd8ed1ab_0.conda#3696792ba70ab3374320fe6041a82286
@@ -311,25 +311,25 @@
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
 https://conda.anaconda.org/conda-forge/noarch/latexcodec-2.0.1-pyh9f0ad1d_0.tar.bz2#8d67904973263afd2985ba56aa2d6bb4
 https://conda.anaconda.org/conda-forge/linux-64/libclang-15.0.7-default_h7634d5b_2.conda#1a4fe5162abe4a19b5a9dedf158a0ff9
 https://conda.anaconda.org/conda-forge/linux-64/libgd-2.3.3-h18fbbfe_3.tar.bz2#ea9758cf553476ddf75c789fdd239dc5
 https://conda.anaconda.org/conda-forge/linux-64/libva-2.18.0-h0b41bf4_0.conda#56e049224de34bbe0478aad422227942
-https://conda.anaconda.org/conda-forge/noarch/lightning-utilities-0.8.0-pyhd8ed1ab_0.conda#ad16f58b64d3b41f4cbb75040b06c9cc
+https://conda.anaconda.org/conda-forge/noarch/lightning-utilities-0.9.0-pyhd8ed1ab_0.conda#c71f7ec8b80a536e58b979299b230251
 https://conda.anaconda.org/conda-forge/noarch/linkify-it-py-2.0.0-pyhd8ed1ab_0.tar.bz2#25b93e66067eb496ac10da888e25cc33
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-2.2.0-pyhd8ed1ab_0.conda#b2928a6c6d52d7e3562b4a59c3214e3a
 https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
 https://conda.anaconda.org/conda-forge/linux-64/mkl-2022.1.0-h84fe81f_915.tar.bz2#b9c8f925797a93dbff45e1626b025a6b
 https://conda.anaconda.org/conda-forge/noarch/overrides-7.3.1-pyhd8ed1ab_0.tar.bz2#a5745ced46e69aa9754053ba061974ab
 https://conda.anaconda.org/conda-forge/noarch/pexpect-4.8.0-pyh1a96a4e_2.tar.bz2#330448ce4403cc74990ac07c555942a1
 https://conda.anaconda.org/conda-forge/linux-64/pillow-9.2.0-py310h454ad03_3.tar.bz2#eb354ff791f505b1d6f13f776359d88e
 https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
 https://conda.anaconda.org/conda-forge/linux-64/proj-9.1.0-h93bde94_0.tar.bz2#255c7204dda39747c3ba380d28b026d7
-https://conda.anaconda.org/conda-forge/linux-64/protobuf-4.23.2-py310hb875b13_1.conda#20feaa8fb200e45f93746836ad96997e
+https://conda.anaconda.org/conda-forge/linux-64/protobuf-4.23.3-py310hb875b13_0.conda#27ce7010f8821add3b955ec88f663bb6
 https://conda.anaconda.org/conda-forge/linux-64/pulseaudio-client-16.1-h5195f5e_3.conda#caeb3302ef1dc8b342b20c710a86f8a9
 https://conda.anaconda.org/conda-forge/noarch/pyasn1-modules-0.2.7-py_0.tar.bz2#ad1e886d09700b2304975335f714bd9c
 https://conda.anaconda.org/conda-forge/noarch/pyproject_hooks-1.0.0-pyhd8ed1ab_0.conda#21de50391d584eb7f4441b9de1ad773f
 https://conda.anaconda.org/conda-forge/noarch/pytest-7.3.2-pyhd8ed1ab_1.conda#f2465696f4396245eca4613f6e924796
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
 https://conda.anaconda.org/conda-forge/noarch/pyu2f-0.1.5-pyhd8ed1ab_0.tar.bz2#caabbeaa83928d0c3e3949261daa18eb
 https://conda.anaconda.org/conda-forge/noarch/qtpy-2.3.1-pyhd8ed1ab_0.conda#10812eca3ec4ebaf3749e1960c208d43
@@ -358,74 +358,74 @@
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
 https://conda.anaconda.org/conda-forge/linux-64/libblas-3.9.0-16_linux64_mkl.tar.bz2#85f61af03fd291dae33150ffe89dc09a
 https://conda.anaconda.org/conda-forge/linux-64/libitk-5.3.0-hcedbc38_0.conda#85b4afd676357f69ab154096f1977884
 https://conda.anaconda.org/conda-forge/linux-64/libnetcdf-4.8.1-nompi_h261ec11_106.tar.bz2#9b25de670ce5753a33c18b1090d1d3bf
 https://conda.anaconda.org/conda-forge/noarch/markdown-3.4.3-pyhd8ed1ab_0.conda#89ed59ad509c05db6f5f2f573d499bfe
 https://conda.anaconda.org/conda-forge/noarch/mdit-py-plugins-0.4.0-pyhd8ed1ab_0.conda#6c5358a10873a15398b6f15f60cb5e1f
 https://conda.anaconda.org/conda-forge/linux-64/mkl-devel-2022.1.0-ha770c72_916.tar.bz2#69ba49e445f87aea2cba343a71a35ca2
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.6.0-pyhd8ed1ab_0.conda#741384b21c1b512617f4ee4ea8457c5d
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.8.0-pyhd8ed1ab_0.conda#3e4aca765371893ad848397794600632
 https://conda.anaconda.org/conda-forge/linux-64/pulseaudio-daemon-16.1-ha8d29e2_3.conda#34d9d75ca896f5919c372a34e25f23ea
 https://conda.anaconda.org/conda-forge/noarch/pybtex-0.24.0-pyhd8ed1ab_2.tar.bz2#2099b86a7399c44c0c61cdb6de6915ba
 https://conda.anaconda.org/conda-forge/linux-64/pyqt5-sip-12.11.0-py310heca2aa9_3.conda#3b1946b676534472ce65181dda0b9554
 https://conda.anaconda.org/conda-forge/noarch/python-build-0.10.0-pyhd8ed1ab_1.conda#0ab47ce574f6a8bcb9f2076436e7fedb
 https://conda.anaconda.org/conda-forge/noarch/setuptools-scm-7.1.0-pyhd8ed1ab_0.conda#6613dbb3b25cc648a107f33ca9f80fc1
-https://conda.anaconda.org/conda-forge/linux-64/sqlalchemy-2.0.16-py310h2372a71_0.conda#61d5ef9e6989a9235a2b449df5ad6df1
+https://conda.anaconda.org/conda-forge/linux-64/sqlalchemy-2.0.17-py310h2372a71_0.conda#5addfcf598875b2e4febacbc98aa2d29
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
 https://conda.anaconda.org/conda-forge/linux-64/aiohttp-3.8.4-py310h2372a71_1.conda#05d01d95b7838f86796b18a80fd42584
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
 https://conda.anaconda.org/conda-forge/noarch/black-22.3.0-pyhd8ed1ab_0.tar.bz2#7ecbfaae9a30b73c1a6e36e4a0debc03
 https://conda.anaconda.org/conda-forge/linux-64/gst-plugins-base-1.22.0-h4243ec0_2.conda#0d0c6604c8ac4ad5e51efa7bb58da05c
 https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-5.3.1-py310hff52083_0.conda#63264f5a6dd5483475968016b614f525
 https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
 https://conda.anaconda.org/conda-forge/linux-64/libcblas-3.9.0-16_linux64_mkl.tar.bz2#361bf757b95488de76c4f123805742d3
 https://conda.anaconda.org/conda-forge/linux-64/liblapack-3.9.0-16_linux64_mkl.tar.bz2#a2f166748917d6d6e4707841ca1f519e
 https://conda.anaconda.org/conda-forge/noarch/oauthlib-3.2.2-pyhd8ed1ab_0.tar.bz2#8f882b197fd9c4941a787926baea4868
 https://conda.anaconda.org/conda-forge/linux-64/pango-1.50.14-hd33c08f_0.conda#a8b9e35dd7be2c945b0de4fe19a7c3a9
-https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
+https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda#a4986c6bb5b0d05a38855b0880a5f425
 https://conda.anaconda.org/conda-forge/linux-64/pulseaudio-16.1-hcb278e6_3.conda#8b452ab959166d91949af4c2d28f81db
 https://conda.anaconda.org/conda-forge/linux-64/pybtex-docutils-1.0.2-py310hff52083_2.tar.bz2#dc929612cad7834bb4726a4de6575a3c
 https://conda.anaconda.org/conda-forge/noarch/pyopenssl-23.2.0-pyhd8ed1ab_1.conda#34f7d568bf59d18e3fef8c405cbece21
 https://conda.anaconda.org/conda-forge/linux-64/simpleitk-2.2.1-py310h2b9ea3a_1.conda#ec09bbee37ea5d3b6022bab2e9b4d5a4
 https://conda.anaconda.org/conda-forge/noarch/flake8-black-0.3.6-pyhd8ed1ab_0.conda#61649e6e9b39ac0c7d10938025f6fe4f
 https://conda.anaconda.org/conda-forge/linux-64/gtk2-2.24.33-h90689f9_2.tar.bz2#957a0255ab58aaf394a91725d73ab422
-https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.2.0-pyhd8ed1ab_0.conda#58ca2d50c3b27b86fd7df62eaadbf9a9
+https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
 https://conda.anaconda.org/conda-forge/linux-64/liblapacke-3.9.0-16_linux64_mkl.tar.bz2#44ccc4d4dca6a8d57fa17442bc64b5a1
 https://conda.anaconda.org/conda-forge/linux-64/librsvg-2.54.4-h7abd40a_0.tar.bz2#921e53675ed5ea352f022b79abab076a
 https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda#f525a01528c3eba1d381a232a6971c6a
 https://conda.anaconda.org/conda-forge/linux-64/numpy-1.25.0-py310ha4c1d20_0.conda#03319f78e5c9c8d90c0110e2c6ed24f6
-https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
+https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.39-hd8ed1ab_0.conda#4bbbe67d5df19db30f04b8e344dc9976
 https://conda.anaconda.org/conda-forge/linux-64/qt-main-5.15.8-h5d23da1_6.conda#59c73debd9405771690ddbbad6c57b69
 https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.15-pyhd8ed1ab_0.conda#27db656619a55d727eaf5a6ece3d2fd6
-https://conda.anaconda.org/conda-forge/noarch/wslink-1.11.0-pyhd8ed1ab_0.conda#70f4b52c0e703936aa1812d8b14a5bb2
+https://conda.anaconda.org/conda-forge/noarch/wslink-1.11.1-pyhd8ed1ab_0.conda#0d0113b67472cea3da288838ebc80acb
 https://conda.anaconda.org/conda-forge/linux-64/blas-devel-3.9.0-16_linux64_mkl.tar.bz2#3f92c1c9e1c0e183462c5071aa02cae1
-https://conda.anaconda.org/conda-forge/noarch/botocore-1.29.158-pyhd8ed1ab_0.conda#ccfde1c6ce8dbb4af5590c88a0482248
+https://conda.anaconda.org/conda-forge/noarch/botocore-1.29.165-pyhd8ed1ab_0.conda#0f30016ea54215fdb883b8978340c9b7
 https://conda.anaconda.org/conda-forge/linux-64/contourpy-1.1.0-py310hd41b1e2_0.conda#684399f9ddc0b9d6f3b6164f6107098e
 https://conda.anaconda.org/conda-forge/linux-64/graphviz-7.0.5-h2e5815a_0.conda#96bf06b24d74a5bf826485e9032c9312
 https://conda.anaconda.org/conda-forge/noarch/ipython-8.14.0-pyh41d4057_0.conda#0a0b0d8177c4a209017b356439292db8
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.7.4-pyhd8ed1ab_0.conda#f7aa15f77d29b11caa1df1eb15383c59
 https://conda.anaconda.org/conda-forge/linux-64/pandas-1.5.3-py310h9b08913_1.conda#331c9dd2560aeb308e26f821280f19d0
 https://conda.anaconda.org/conda-forge/linux-64/pyqt-5.15.7-py310hab646b1_3.conda#d049da3204bf5ecb54a852b622f2d7d2
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/linux-64/vtk-9.2.5-qt_py310hc895abb_200.conda#3462cb0fb18182f4203cdb6e73434a31
 https://conda.anaconda.org/conda-forge/linux-64/blas-2.116-mkl.tar.bz2#c196a26abf6b4f132c88828ab7c2231c
-https://conda.anaconda.org/conda-forge/noarch/google-auth-2.20.0-pyh1a96a4e_0.conda#59f942ef9326d2519a7c953f1c24d5da
-https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.2-pyh210e3f2_0.conda#c76d274e313a06f23de594848e12a75c
+https://conda.anaconda.org/conda-forge/noarch/google-auth-2.21.0-pyh1a96a4e_0.conda#8c5dd8609d314721d990c1d1fd607f81
+https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.3-pyh71e2992_0.conda#482f0176a89f14e10a7d15f9f1980e36
 https://conda.anaconda.org/conda-forge/noarch/jupyter-cache-0.6.1-pyhd8ed1ab_0.conda#2e360820ae68e3d28e1a5a9d2714ca5c
 https://conda.anaconda.org/conda-forge/linux-64/matplotlib-base-3.7.1-py310he60537e_0.conda#68b2dd34c69d08b05a9db5e3596fe3ee
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.6.0-pyhd8ed1ab_0.conda#879782bde4bbdb4c7b5d4054504a20d5
 https://conda.anaconda.org/conda-forge/noarch/pooch-1.7.0-pyha770c72_3.conda#5936894aade8240c867d292aa0d980c6
 https://conda.anaconda.org/conda-forge/noarch/requests-oauthlib-1.3.1-pyhd8ed1ab_0.tar.bz2#61b279f051eef9c89d58f4d813e75e04
 https://conda.anaconda.org/conda-forge/noarch/s3transfer-0.6.1-pyhd8ed1ab_0.conda#b19a857ac845097e9c823c9f4d35f80e
 https://conda.anaconda.org/conda-forge/noarch/sphinx-4.5.0-pyh6c4a22f_0.tar.bz2#46b38d88c4270ff9ba78a89c83c66345
-https://conda.anaconda.org/conda-forge/noarch/boto3-1.26.158-pyhd8ed1ab_0.conda#2e39307a3987518e49eb30ca51e3cfb5
-https://conda.anaconda.org/conda-forge/noarch/google-auth-oauthlib-1.0.0-pyhd8ed1ab_0.conda#5ba9d95acb9add67f468ecdee6595c0f
-https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.6-pyhd8ed1ab_0.conda#68627a08556e4a273e4c7bfc84251457
+https://conda.anaconda.org/conda-forge/noarch/boto3-1.26.165-pyhd8ed1ab_0.conda#b9a6316db67d5f2c8dbac2aeb24c6803
+https://conda.anaconda.org/conda-forge/noarch/google-auth-oauthlib-1.0.0-pyhd8ed1ab_1.conda#569e62e95b01b53e4ec7d9abe83b7385
+https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.7-pyhd8ed1ab_0.conda#4b0f4e8fe2a303e472674eae0340bdad
 https://conda.anaconda.org/conda-forge/noarch/jupyter_console-6.6.3-pyhd8ed1ab_0.conda#7cf6f52a66f8e3cd9d8b6c231262dcab
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.6.0-pyhd8ed1ab_0.conda#39fd52b0fcb2fb52bac47a1419bf09bd
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.7.0-pyhd8ed1ab_0.conda#7488cd1f4d35a2af96faa765b7e5b2f0
 https://conda.anaconda.org/conda-forge/linux-64/matplotlib-3.7.1-py310hff52083_0.conda#c2b60c44d38d32779006a15c2581f0d1
 https://conda.anaconda.org/conda-forge/noarch/myst-parser-0.18.1-pyhd8ed1ab_0.tar.bz2#bcfdf5c7d8bf5c6f6be7b4c66fff2eca
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.6.0-pyhd8ed1ab_0.conda#e8172ca42f2869bb90185c9356899e81
 https://conda.anaconda.org/conda-forge/noarch/pydata-sphinx-theme-0.13.3-pyhd8ed1ab_0.conda#07aca5f2dea315dcc16680d6891e9056
 https://conda.anaconda.org/conda-forge/noarch/qtconsole-base-5.4.3-pyha770c72_0.conda#e0f5e8a6f9ea248e5c2d23efffff08f7
 https://conda.anaconda.org/conda-forge/linux-64/scipy-1.10.1-py310ha4c1d20_3.conda#0414d57832172f3cdcf56b5f053e177d
 https://conda.anaconda.org/conda-forge/noarch/sphinx-comments-0.0.3-pyh9f0ad1d_0.tar.bz2#2ae3ce35de0c1cec45c94182694f8d1b
@@ -453,8 +453,9 @@
 https://conda.anaconda.org/conda-forge/noarch/nbclassic-1.0.0-pyhb4ecaf3_1.conda#a0be31e9bd84d6eae87cdbf74c56b90b
 https://conda.anaconda.org/conda-forge/noarch/notebook-6.5.4-pyha770c72_0.conda#ec4ce3ce0a55ce21b6f5b86049b97af9
 https://conda.anaconda.org/conda-forge/linux-64/jupyter-1.0.0-py310hff52083_8.conda#6ecb24d6906d5d2a6f091cf4b0045079
 https://conda.anaconda.org/pytorch/linux-64/pytorch-2.0.1-py3.10_cuda11.8_cudnn8.7.0_0.tar.bz2#e8dd4a234ce193267c4cbc981c042429
 https://conda.anaconda.org/conda-forge/noarch/torchinfo-1.8.0-pyhd8ed1ab_0.conda#fba98fc95a945e2a6b93a77b39dd52dc
 https://conda.anaconda.org/conda-forge/noarch/torchmetrics-0.11.4-pyhd8ed1ab_0.conda#480cb2b6d502003e937d9e4326bc398f
 https://conda.anaconda.org/pytorch/linux-64/torchtriton-2.0.0-py310.tar.bz2#e34aa90f6d7c20babf28fc9225b2a3eb
-https://conda.anaconda.org/conda-forge/noarch/pytorch-lightning-2.0.3-pyhd8ed1ab_0.conda#97138eb8783fa54884216a6562413736
+https://conda.anaconda.org/pytorch/linux-64/torchvision-0.15.2-py310_cu118.tar.bz2#b38f7082cde2a86ca981194e9ef51028
+https://conda.anaconda.org/conda-forge/noarch/pytorch-lightning-2.0.4-pyhd8ed1ab_0.conda#ce9d626b181c6f8cceb5047f6a819f7d
```

### Comparing `hf-deepali-0.3.1/conda/environment.osx-64.lock` & `hf-deepali-0.3.2/conda/environment.osx-64.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # Generated by conda-lock.
 # platform: osx-64
-# input_hash: 358ba6fb20a9e7c56751c467f43592eee84f35e52b7599dfceb8f0df6af063bb
+# input_hash: 1664d2c199c9cddb402252a38f5527d218754e954cbb25a82da7fecc8cbae3f6
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h0d85af4_4.tar.bz2#37edc4e6304ca87316e160f5ca0bd1b5
 https://conda.anaconda.org/conda-forge/osx-64/c-ares-1.19.1-h0dc2134_0.conda#b3e62631b4e1b9801477523ce1d6f355
 https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2023.5.7-h8857fd0_0.conda#b704e4b79ba0d887c4870b7b09d6a4df
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-dejavu-sans-mono-2.37-hab24e00_0.tar.bz2#0c96522c6bdaed4b1566d11387caaf45
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-inconsolata-3.000-h77eed37_0.tar.bz2#34893075a5c9e55cdafac56607368fc6
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-source-code-pro-2.038-h77eed37_0.tar.bz2#4d59c254e01d9cde7957100457e2d5fb
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-ubuntu-0.83-hab24e00_0.tar.bz2#19410c3df09dfb12d1206132a1d357c5
 https://conda.anaconda.org/conda-forge/osx-64/fribidi-1.0.10-hbcb3906_0.tar.bz2#f1c6b41e0f56998ecd9a3e210faa1dc0
 https://conda.anaconda.org/conda-forge/osx-64/giflib-5.2.1-hb7f2c08_3.conda#aca150b0186836f893ebac79019e5498
 https://conda.anaconda.org/conda-forge/osx-64/jpeg-9e-hb7f2c08_3.conda#6b55131ae9445ef38746dc6b080acda9
 https://conda.anaconda.org/conda-forge/osx-64/lame-3.100-hb7f2c08_1003.tar.bz2#3342b33c9a0921b22b767ed68ee25861
-https://conda.anaconda.org/conda-forge/osx-64/libbrotlicommon-1.0.9-hb7f2c08_8.tar.bz2#37157d273eaf3bc7d6862104161d9ec9
+https://conda.anaconda.org/conda-forge/osx-64/libbrotlicommon-1.0.9-hb7f2c08_9.conda#ee1ee8c79c3426229ad03290573be552
 https://conda.anaconda.org/conda-forge/osx-64/libcxx-16.0.6-hd57cbcb_0.conda#7d6972792161077908b62971802f289a
 https://conda.anaconda.org/conda-forge/osx-64/libdeflate-1.14-hb7f2c08_0.tar.bz2#ce2a6075114c9b64ad8cace52492feee
 https://conda.anaconda.org/conda-forge/osx-64/libev-4.33-haf1e3a3_1.tar.bz2#79dc2be110b2a3d1e97ec21f691c50ad
 https://conda.anaconda.org/conda-forge/osx-64/libexpat-2.5.0-hf0c8a7f_1.conda#6c81cb022780ee33435cca0127dd43c9
 https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2#ccb34fb14960ad8b125962d3d79b31a9
 https://conda.anaconda.org/conda-forge/osx-64/libiconv-1.17-hac89ed1_0.tar.bz2#691d103d11180486154af49c037b7ed9
 https://conda.anaconda.org/conda-forge/osx-64/libogg-1.3.4-h35c211d_1.tar.bz2#a7ab4b53ef18c598ffaa597230bc3ba1
@@ -51,18 +51,18 @@
 https://conda.anaconda.org/conda-forge/osx-64/gettext-0.21.1-h8a4c099_0.tar.bz2#1e3aff29ce703d421c43f371ad676cc5
 https://conda.anaconda.org/conda-forge/osx-64/glew-2.1.0-h046ec9c_2.tar.bz2#6b753c8c7e4c46a8eb17b6f1781f958a
 https://conda.anaconda.org/conda-forge/osx-64/gmp-6.2.1-h2e338ed_0.tar.bz2#dedc96914428dae572a39e69ee2a392f
 https://conda.anaconda.org/conda-forge/osx-64/graphite2-1.3.13-h2e338ed_1001.tar.bz2#5f6e7f98caddd0fc2d345b207531814c
 https://conda.anaconda.org/conda-forge/osx-64/icu-70.1-h96cf925_0.tar.bz2#376635049e9b9b0bb875efd39dcd7b3b
 https://conda.anaconda.org/conda-forge/osx-64/jsoncpp-1.9.5-h940c156_1.tar.bz2#45824afbfd843fe0584ae8df22f1d99a
 https://conda.anaconda.org/conda-forge/osx-64/lerc-4.0.0-hb486fe8_0.tar.bz2#f9d6a4c82889d5ecedec1d90eb673c55
-https://conda.anaconda.org/conda-forge/osx-64/libabseil-20230125.2-cxx17_h000cb23_2.conda#52adda30d725e5afd2b4a25331818bdc
+https://conda.anaconda.org/conda-forge/osx-64/libabseil-20230125.3-cxx17_h000cb23_0.conda#1d883cd421a0b0af624c38fa8d043f98
 https://conda.anaconda.org/conda-forge/osx-64/libaec-1.0.6-hf0c8a7f_1.conda#7c0f82f435ab4c48d65dc9b28db2ad9e
-https://conda.anaconda.org/conda-forge/osx-64/libbrotlidec-1.0.9-hb7f2c08_8.tar.bz2#7f952a036d9014b4dab96c6ea0f8c2a7
-https://conda.anaconda.org/conda-forge/osx-64/libbrotlienc-1.0.9-hb7f2c08_8.tar.bz2#b36a3bfe866d9127f25f286506982166
+https://conda.anaconda.org/conda-forge/osx-64/libbrotlidec-1.0.9-hb7f2c08_9.conda#4043ef9fe42e178785e0e1853b79bdf9
+https://conda.anaconda.org/conda-forge/osx-64/libbrotlienc-1.0.9-hb7f2c08_9.conda#b64d4dcc70aa141db7fccbf13bad81e1
 https://conda.anaconda.org/conda-forge/osx-64/libedit-3.1.20191231-h0678c8f_2.tar.bz2#6016a8a1d0e63cac3de2c352cd40208b
 https://conda.anaconda.org/conda-forge/osx-64/libgfortran5-12.2.0-he409387_31.conda#5a544130e584b1f204ac896ff071d5b3
 https://conda.anaconda.org/conda-forge/osx-64/libllvm13-13.0.1-h64f94b2_2.tar.bz2#bac1c6f12f44f40e19274e6e04e9bad5
 https://conda.anaconda.org/conda-forge/osx-64/libpng-1.6.39-ha978bb4_0.conda#35e4928794c5391aec14ffdf1deaaee5
 https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.42.0-h58db7d2_0.conda#a7d3b44b7b0c9901ac7813b7a0462893
 https://conda.anaconda.org/conda-forge/osx-64/libvorbis-1.3.7-h046ec9c_0.tar.bz2#fbbda1fede0aadaa252f6919148c4ce1
 https://conda.anaconda.org/conda-forge/osx-64/libvpx-1.11.0-he49afe7_3.tar.bz2#4ad2e740535a74d4ab65550b8a41f99f
@@ -80,60 +80,60 @@
 https://conda.anaconda.org/conda-forge/osx-64/svt-av1-1.4.1-hf0c8a7f_0.conda#86739428e1e1c8882fe14067a7ac371a
 https://conda.anaconda.org/conda-forge/osx-64/tbb-2021.9.0-hb8565cd_0.conda#6aedf8fdcdf5f2d7b4db21853a7d42ed
 https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.12-h5dbffcc_0.tar.bz2#8e9480d9c47061db2ed1b4ecce519a7f
 https://conda.anaconda.org/conda-forge/osx-64/x265-3.5-hbb4e6a2_3.tar.bz2#a3bf3e95b7795871a6734a784400fcea
 https://conda.anaconda.org/conda-forge/osx-64/zeromq-4.3.4-he49afe7_1.tar.bz2#1972d732b123ed04b60fd21e94f0b178
 https://conda.anaconda.org/conda-forge/osx-64/zlib-1.2.13-h8a1eda9_5.conda#75a8a98b1c4671c5d2897975731da42d
 https://conda.anaconda.org/conda-forge/osx-64/zstd-1.5.2-hbc0c0cd_6.conda#40a188783d3c425bdccc9ae9104acbb8
-https://conda.anaconda.org/conda-forge/osx-64/brotli-bin-1.0.9-hb7f2c08_8.tar.bz2#aac5ad0d8f747ef7f871508146df75d9
+https://conda.anaconda.org/conda-forge/osx-64/brotli-bin-1.0.9-hb7f2c08_9.conda#72c526f7ffa265473e6c75fd90605e52
 https://conda.anaconda.org/conda-forge/noarch/fonts-conda-ecosystem-1-0.tar.bz2#fee5683a3f04bd15cbd8318b096a27ab
 https://conda.anaconda.org/conda-forge/osx-64/freetype-2.12.1-h3f81eb7_1.conda#852224ea3e8991a8342228eab274840e
 https://conda.anaconda.org/conda-forge/osx-64/gl2ps-1.4.2-h4cff582_0.tar.bz2#a9e91533b95cd019d58f4b3ef9bbddf0
 https://conda.anaconda.org/conda-forge/osx-64/hdf4-4.2.15-h7aa5921_5.tar.bz2#a5e171d71c6b524409de40d81c098758
 https://conda.anaconda.org/conda-forge/osx-64/krb5-1.20.1-h049b76e_0.conda#db11fa2968ef0837288fe2d7f5b77a50
 https://conda.anaconda.org/conda-forge/osx-64/libclang-13.0.1-default_h255f2f3_1.conda#7ffe2879ebb140302889d22a1ec41d84
 https://conda.anaconda.org/conda-forge/osx-64/libgfortran-5.0.0-11_3_0_h97931a8_31.conda#97451338600bd9c5b535eb224ef6c471
 https://conda.anaconda.org/conda-forge/osx-64/libglib-2.76.3-hc62aa5d_0.conda#3687b3c1d257dec787418281cfc58358
 https://conda.anaconda.org/conda-forge/osx-64/libidn2-2.3.4-hb7f2c08_0.tar.bz2#bd109fd705b4ce40a62759129bc4ef5a
 https://conda.anaconda.org/conda-forge/osx-64/libnghttp2-1.52.0-he2ab024_0.conda#12ac7d100bf260263e30a019517f42a2
-https://conda.anaconda.org/conda-forge/osx-64/libprotobuf-4.23.2-h5feb325_5.conda#ae92f79c6d9af43468d4109fe76b37b8
+https://conda.anaconda.org/conda-forge/osx-64/libprotobuf-4.23.3-h5feb325_0.conda#b9e780ed0d0a365ff10b8e83c64471ce
 https://conda.anaconda.org/conda-forge/osx-64/libssh2-1.11.0-hd019ec5_0.conda#ca3a72efba692c59a90d4b9fc0dfe774
 https://conda.anaconda.org/conda-forge/osx-64/libtheora-1.1.1-h0d85af4_1005.tar.bz2#e63b84ed4c2d84901332de92a98a2f2b
 https://conda.anaconda.org/conda-forge/osx-64/libtiff-4.4.0-h6268bbc_5.conda#551fc78ba147767ea5905d0746e2fbb5
 https://conda.anaconda.org/conda-forge/osx-64/libxml2-2.10.3-h201ad9d_4.conda#2101dd548f0601be252e27e48fa532fa
 https://conda.anaconda.org/conda-forge/osx-64/libzip-1.9.2-h6db710c_1.tar.bz2#ce732d37e479919f3d22b1ccdeb858ac
 https://conda.anaconda.org/conda-forge/osx-64/mkl-2022.1.0-h860c996_928.tar.bz2#98a4d58de0ba6e61ce46620b775c19ce
 https://conda.anaconda.org/conda-forge/osx-64/mpfr-4.2.0-h4f9bd69_0.conda#f48a2f4515be334c5cfeed82517b96e0
-https://conda.anaconda.org/conda-forge/osx-64/mysql-common-8.0.33-hc6116ba_0.conda#a4cd3c3df486b393d71ad75dd8d7c11f
+https://conda.anaconda.org/conda-forge/osx-64/mysql-common-8.0.33-hc6116ba_1.conda#bfbfd93ef846f67d53f40bcf28b91621
 https://conda.anaconda.org/conda-forge/osx-64/nss-3.89-h78b00b3_0.conda#1eb1408ecae62d98a902636d46f5595c
-https://conda.anaconda.org/conda-forge/osx-64/python-3.10.11-he7542f4_0_cpython.conda#ec1a9528837c5fcd34f387e317b30f1e
+https://conda.anaconda.org/conda-forge/osx-64/python-3.10.12-had23ca6_0_cpython.conda#351b8aa0687f3510620cf06ad11229f4
 https://conda.anaconda.org/conda-forge/osx-64/sqlite-3.42.0-h2b0dec6_0.conda#6c22b83608a6e3bd324ab29d3092592f
 https://conda.anaconda.org/conda-forge/osx-64/tbb-devel-2021.9.0-hb8565cd_0.conda#23fd9e2cb5478ed8b6ba925a741af61b
 https://conda.anaconda.org/conda-forge/noarch/absl-py-1.4.0-pyhd8ed1ab_0.conda#dd5eed01874c75bebef810a2faec673e
 https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.13-pyhd8ed1ab_0.conda#06006184e203b61d3525f90de394471e
 https://conda.anaconda.org/conda-forge/noarch/appnope-0.1.3-pyhd8ed1ab_0.tar.bz2#54ac328d703bff191256ffa1183126d1
 https://conda.anaconda.org/conda-forge/osx-64/atk-1.0-2.38.0-h1d18e73_1.tar.bz2#5a538295f97a484ee332aacc131718b5
 https://conda.anaconda.org/conda-forge/noarch/attrs-21.4.0-pyhd8ed1ab_0.tar.bz2#f70280205d7044c8b8358c8de3190e5d
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
 https://conda.anaconda.org/conda-forge/noarch/blinker-1.6.2-pyhd8ed1ab_0.conda#2fb79ec81bad9492b6d59a06b3b647a4
-https://conda.anaconda.org/conda-forge/osx-64/brotli-1.0.9-hb7f2c08_8.tar.bz2#55f612fe4a9b5f6ac76348b6de94aaeb
-https://conda.anaconda.org/conda-forge/noarch/cachetools-5.3.0-pyhd8ed1ab_0.conda#fd006afc4115740d8d52887ee813f262
+https://conda.anaconda.org/conda-forge/osx-64/brotli-1.0.9-hb7f2c08_9.conda#53cff90f0cea22e13e5b791f0e5a8e7d
+https://conda.anaconda.org/conda-forge/noarch/cachetools-5.3.1-pyhd8ed1ab_0.conda#60b5eb16d9a7a5482ba37f67aa49db5b
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2#20e4087407c7cb04a40817114b333dbf
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.11.0-pyhd8ed1ab_0.tar.bz2#a50559fad0affdbb33729a68669ca1cb
 https://conda.anaconda.org/conda-forge/noarch/dataclasses-0.8-pyhc8e2a94_3.tar.bz2#a362b2124b06aad102e2ee4581acee7d
 https://conda.anaconda.org/conda-forge/osx-64/debugpy-1.6.7-py310h7a76584_0.conda#549f7722839c44ee8a859fc0b94a5884
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
 https://conda.anaconda.org/conda-forge/osx-64/docutils-0.17.1-py310h2ec42d9_3.tar.bz2#69b3569d320b0fc940449fcc25b01e31
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
-https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
 https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
 https://conda.anaconda.org/conda-forge/osx-64/fftw-3.3.10-nompi_h4fa670e_108.conda#39132ce6ed3180b42b54d40289cd4157
 https://conda.anaconda.org/conda-forge/noarch/filelock-3.12.2-pyhd8ed1ab_0.conda#53522ec72e6adae42bd373ef58357230
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/osx-64/fontconfig-2.14.2-h5bb23bf_0.conda#86cc5867dfbee4178118392bae4a3c89
 https://conda.anaconda.org/conda-forge/osx-64/frozenlist-1.3.3-py310h90acd4f_0.tar.bz2#a3236ddc60f49384eba9348391293038
 https://conda.anaconda.org/conda-forge/noarch/fsspec-2023.6.0-pyh1a96a4e_0.conda#50ea2067ec92dfcc38b4f07992d7e235
@@ -143,45 +143,45 @@
 https://conda.anaconda.org/conda-forge/osx-64/greenlet-2.0.2-py310h9e9d8ca_1.conda#699b3a96666340fe9349c3547f047e29
 https://conda.anaconda.org/conda-forge/osx-64/gts-0.7.6-h53e17e3_4.conda#848cc963fcfbd063c7a023024aa3bec0
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
 https://conda.anaconda.org/conda-forge/noarch/ipython_genutils-0.2.0-py_1.tar.bz2#5071c982548b3a20caf70462f04f5287
 https://conda.anaconda.org/conda-forge/noarch/jmespath-1.0.1-pyhd8ed1ab_0.tar.bz2#2cfa3e1cf3fb51bb9b17acc5b5e9ea11
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.7-pyhd8ed1ab_1.conda#0c0a54e16b764bafcae35913cc9d60ff
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.8-pyhd8ed1ab_0.conda#2bc3ca2f7387af385dd06706b4fb2d35
 https://conda.anaconda.org/conda-forge/osx-64/kiwisolver-1.4.4-py310ha23aa8a_1.tar.bz2#cc358fb878ac593c60cea08b28ac7423
 https://conda.anaconda.org/conda-forge/osx-64/lazy-object-proxy-1.9.0-py310h90acd4f_0.conda#b0b1dc46dd92f49877ea8eecd56f2d00
 https://conda.anaconda.org/conda-forge/osx-64/lcms2-2.14-h90f4b2a_0.tar.bz2#e56c432e9a78c63692fa6bd076a15713
 https://conda.anaconda.org/conda-forge/osx-64/libblas-3.9.0-17_osx64_mkl.conda#e5d4b69958f8eb30b932828880b847f3
 https://conda.anaconda.org/conda-forge/osx-64/libcurl-8.1.2-hbee3ae8_0.conda#d51e337da844262f9033c9a26452520f
-https://conda.anaconda.org/conda-forge/osx-64/libgrpc-1.55.1-h73e6b18_1.conda#bbeac6706560961d3eb7cb75c6cc5ab1
+https://conda.anaconda.org/conda-forge/osx-64/libgrpc-1.56.0-he6801ca_2.conda#46a189776f694d37c24c5c1fc301bf50
 https://conda.anaconda.org/conda-forge/osx-64/libpq-15.3-h9dc22bb_1.conda#571aa9141d1a823202bb4cd794c939b0
 https://conda.anaconda.org/conda-forge/osx-64/libwebp-1.2.4-hfa4350a_0.tar.bz2#d3b5a56369701e6a11bf300ba3394391
 https://conda.anaconda.org/conda-forge/osx-64/loguru-0.7.0-py310h2ec42d9_0.conda#632a71feccc9f651c844c402efe61884
 https://conda.anaconda.org/conda-forge/osx-64/markupsafe-2.1.3-py310h6729b98_0.conda#b23ce1495527802905791489c3b1f129
 https://conda.anaconda.org/conda-forge/noarch/mccabe-0.7.0-pyhd8ed1ab_0.tar.bz2#34fc335fc50eef0b5ea708f2b5f54e0c
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
 https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda#c7d0ea64c37752ecbe6da458aee662d2
 https://conda.anaconda.org/conda-forge/osx-64/mkl-devel-2022.1.0-h694c41f_929.tar.bz2#041ceef009fe6d29cbd2555907c23ab3
 https://conda.anaconda.org/conda-forge/osx-64/mpc-1.3.1-h81bd1dd_0.conda#c752c0eb6c250919559172c011e5f65b
 https://conda.anaconda.org/conda-forge/noarch/mpmath-1.3.0-pyhd8ed1ab_0.conda#dbf6e2d89137da32fa6670f3bffc024e
 https://conda.anaconda.org/conda-forge/osx-64/multidict-6.0.4-py310h90acd4f_0.conda#0324181c4442d94c865cf9ae3b6a7fea
 https://conda.anaconda.org/conda-forge/noarch/munkres-1.1.4-pyh9f0ad1d_0.tar.bz2#2ba8498c1018c1e9c61eb99b973dfe19
 https://conda.anaconda.org/conda-forge/noarch/mypy_extensions-1.0.0-pyha770c72_0.conda#4eccaeba205f0aed9ac3a9ea58568ca3
-https://conda.anaconda.org/conda-forge/osx-64/mysql-libs-8.0.33-haa61052_0.conda#8e35f9a9a8965c8c29e9f678e290ac7f
+https://conda.anaconda.org/conda-forge/osx-64/mysql-libs-8.0.33-haa61052_1.conda#b1ba5ec2e4a774e8e4887f0f7592b574
 https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.6-pyhd8ed1ab_0.tar.bz2#7b868f21adde0d9b8b38f9c16836589b
 https://conda.anaconda.org/conda-forge/noarch/networkx-3.1-pyhd8ed1ab_0.conda#254f787d5068bc89f578bf63893ce8b4
 https://conda.anaconda.org/conda-forge/osx-64/openjpeg-2.5.0-h5d0d7b0_1.tar.bz2#be533cc782981a0ec5eed28aa618470a
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
 https://conda.anaconda.org/conda-forge/noarch/pathspec-0.11.1-pyhd8ed1ab_0.conda#dbb80d1e8dc2dba5c8b106dc0768ad45
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
-https://conda.anaconda.org/conda-forge/noarch/pluggy-1.0.0-pyhd8ed1ab_5.tar.bz2#7d301a0d25f424d96175f810935f0da9
+https://conda.anaconda.org/conda-forge/noarch/pluggy-1.2.0-pyhd8ed1ab_0.conda#7263924c642d22e311d9e59b839f1b33
 https://conda.anaconda.org/conda-forge/noarch/ply-3.11-py_1.tar.bz2#7205635cd71531943440fbfe3b6b5727
 https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.0-pyhd8ed1ab_0.conda#95c5be3c7cbd872509d16c216617fdab
 https://conda.anaconda.org/conda-forge/osx-64/psutil-5.9.5-py310h90acd4f_0.conda#1111504c53989e065a98171156fc376a
 https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
 https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
 https://conda.anaconda.org/conda-forge/noarch/pyasn1-0.4.8-py_0.tar.bz2#06d04c9f8f72ac77911db942eda24fb9
 https://conda.anaconda.org/conda-forge/noarch/pycodestyle-2.10.0-pyhd8ed1ab_0.conda#89843e4cc99c6a3fe5f4c86994cc8410
@@ -218,59 +218,59 @@
 https://conda.anaconda.org/conda-forge/osx-64/typed-ast-1.5.4-py310h90acd4f_1.tar.bz2#189bf6e55cac449f8b34763502b18385
 https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.3-pyha770c72_0.conda#4a3014a4d107d15475d106b751c4e352
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/noarch/uc-micro-py-1.0.1-pyhd8ed1ab_0.tar.bz2#3ddf6684d9b274a12c94e509ca45656c
 https://conda.anaconda.org/conda-forge/osx-64/unicodedata2-15.0.0-py310h90acd4f_0.tar.bz2#b62adca3645b3bbc46940d5b1833d59b
 https://conda.anaconda.org/conda-forge/noarch/unidecode-1.3.6-pyhd8ed1ab_0.tar.bz2#e8f24401b17802df5f82f66a88cee29e
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
-https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.0-pyhd8ed1ab_0.conda#1dd6387a73d84e16b6f73de676bb4c36
+https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda#c34d9325a609381a0b0e8a5b4f325147
 https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
-https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
+https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.8-pyhd8ed1ab_0.conda#2e9ebddf0b93d0fb203d0906b8052c4f
 https://conda.anaconda.org/conda-forge/osx-64/wrapt-1.15.0-py310h90acd4f_0.conda#f91dbc3c63e137a27a4de2964d56e6e3
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
 https://conda.anaconda.org/conda-forge/noarch/accessible-pygments-0.0.4-pyhd8ed1ab_0.conda#46a2e6e3dfa718ce3492018d5a110dd6
 https://conda.anaconda.org/conda-forge/noarch/aiosignal-1.3.1-pyhd8ed1ab_0.tar.bz2#d1e1eb7e21a9e2c74279d87dafb68156
 https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.0-pyhd8ed1ab_1.conda#2b35a85d654a47aac8f34c1bb6de7142
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
-https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.4-pyhd8ed1ab_0.tar.bz2#c5b3edc62d6309088f4970b3eaaa65a6
+https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
 https://conda.anaconda.org/conda-forge/osx-64/cairo-1.16.0-h904041c_1014.tar.bz2#2e7b4350178ed52bb6fd2b1ecbeeed4f
 https://conda.anaconda.org/conda-forge/osx-64/cffi-1.15.1-py310ha78151a_3.conda#652082e4a6cf9d26e43d0d362590c276
 https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda#168ae0f82cdf7505048e81054c7354e4
 https://conda.anaconda.org/conda-forge/osx-64/curl-8.1.2-hbee3ae8_0.conda#6cc301a6c2ba26e29949818efdc133ca
 https://conda.anaconda.org/conda-forge/noarch/dacite-1.8.0-pyhd8ed1ab_0.conda#3696792ba70ab3374320fe6041a82286
 https://conda.anaconda.org/conda-forge/noarch/deprecation-2.1.0-pyh9f0ad1d_0.tar.bz2#7b6747d7cc2076341029cff659669e8b
 https://conda.anaconda.org/conda-forge/osx-64/ffmpeg-5.1.2-gpl_h8b4fe81_106.conda#3c62afa3457aeb6f058b40f1f41f772a
 https://conda.anaconda.org/conda-forge/noarch/flake8-6.0.0-pyhd8ed1ab_0.conda#e9345ba05d71742412b8aa6992ad9457
 https://conda.anaconda.org/conda-forge/osx-64/fonttools-4.40.0-py310h6729b98_0.conda#15dcc729f2102b4b64e0e6f53f2fb377
 https://conda.anaconda.org/conda-forge/osx-64/glib-2.76.3-h7d26f99_0.conda#a062952a59c0a26adb18899ac6472a7e
 https://conda.anaconda.org/conda-forge/osx-64/gmpy2-2.1.2-py310hb691cb2_1.tar.bz2#a495ede1fb673f39133b7c2628af7259
-https://conda.anaconda.org/conda-forge/osx-64/grpcio-1.55.1-py310hd8379ad_1.conda#cabe22578d16cd6a36a22d215a8a0f53
+https://conda.anaconda.org/conda-forge/osx-64/grpcio-1.56.0-py310h0d4bf3c_2.conda#0ce1b3a5e4abf21c5a33e8d270ec2be2
 https://conda.anaconda.org/conda-forge/osx-64/hdf5-1.12.2-nompi_h48135f9_101.conda#2ee4811ba5f72f7f12f69b3ec2d6cd96
 https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.7.0-pyha770c72_0.conda#ba3786c6846e46038fe60c785d46dc81
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
 https://conda.anaconda.org/conda-forge/noarch/latexcodec-2.0.1-pyh9f0ad1d_0.tar.bz2#8d67904973263afd2985ba56aa2d6bb4
 https://conda.anaconda.org/conda-forge/osx-64/libcblas-3.9.0-17_osx64_mkl.conda#5adcad22978f80fa101047022e79d9eb
 https://conda.anaconda.org/conda-forge/osx-64/libgd-2.3.3-h1e214de_3.tar.bz2#350af2b75c58dc16985fa97298469143
 https://conda.anaconda.org/conda-forge/osx-64/liblapack-3.9.0-17_osx64_mkl.conda#5557060dea295fcbb224be17b3947d16
-https://conda.anaconda.org/conda-forge/noarch/lightning-utilities-0.8.0-pyhd8ed1ab_0.conda#ad16f58b64d3b41f4cbb75040b06c9cc
+https://conda.anaconda.org/conda-forge/noarch/lightning-utilities-0.9.0-pyhd8ed1ab_0.conda#c71f7ec8b80a536e58b979299b230251
 https://conda.anaconda.org/conda-forge/noarch/linkify-it-py-2.0.0-pyhd8ed1ab_0.tar.bz2#25b93e66067eb496ac10da888e25cc33
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-2.2.0-pyhd8ed1ab_0.conda#b2928a6c6d52d7e3562b4a59c3214e3a
 https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
 https://conda.anaconda.org/conda-forge/noarch/overrides-7.3.1-pyhd8ed1ab_0.tar.bz2#a5745ced46e69aa9754053ba061974ab
 https://conda.anaconda.org/conda-forge/noarch/pexpect-4.8.0-pyh1a96a4e_2.tar.bz2#330448ce4403cc74990ac07c555942a1
 https://conda.anaconda.org/conda-forge/osx-64/pillow-9.2.0-py310hffcf78b_3.tar.bz2#a7b7035e6aeace50e0023839f3f5beaa
 https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
 https://conda.anaconda.org/conda-forge/osx-64/proj-9.1.0-hcbd9701_0.tar.bz2#78ee95e87e5143d0e4a17d4aeef56411
-https://conda.anaconda.org/conda-forge/osx-64/protobuf-4.23.2-py310h4e8a696_1.conda#62b758907a0ff180ceccd17ed0024aad
+https://conda.anaconda.org/conda-forge/osx-64/protobuf-4.23.3-py310h4e8a696_0.conda#8da9b5d52ebad6a80785fdf5f2c57ff9
 https://conda.anaconda.org/conda-forge/noarch/pyasn1-modules-0.2.7-py_0.tar.bz2#ad1e886d09700b2304975335f714bd9c
 https://conda.anaconda.org/conda-forge/osx-64/pyobjc-core-9.2-py310hef2d279_0.conda#e1ab355e10f9fc8995371072a2e0fa29
 https://conda.anaconda.org/conda-forge/noarch/pyproject_hooks-1.0.0-pyhd8ed1ab_0.conda#21de50391d584eb7f4441b9de1ad773f
 https://conda.anaconda.org/conda-forge/noarch/pytest-7.3.2-pyhd8ed1ab_1.conda#f2465696f4396245eca4613f6e924796
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
 https://conda.anaconda.org/conda-forge/noarch/pyu2f-0.1.5-pyhd8ed1ab_0.tar.bz2#caabbeaa83928d0c3e3949261daa18eb
 https://conda.anaconda.org/conda-forge/noarch/qtpy-2.3.1-pyhd8ed1ab_0.conda#10812eca3ec4ebaf3749e1960c208d43
@@ -285,90 +285,91 @@
 https://conda.anaconda.org/conda-forge/osx-64/yarl-1.9.2-py310h6729b98_0.conda#f8a1c7107b3b661accf1a7d86c8fd4e1
 https://conda.anaconda.org/conda-forge/osx-64/argon2-cffi-bindings-21.2.0-py310h90acd4f_3.tar.bz2#952166ee5ce75092167a7385a4e243e3
 https://conda.anaconda.org/conda-forge/osx-64/astroid-2.15.5-py310h2ec42d9_0.conda#6f8c825da6f4eedc532a6d102220d0e0
 https://conda.anaconda.org/conda-forge/noarch/async-timeout-4.0.2-pyhd8ed1ab_0.tar.bz2#25e79f9a1133556671becbd65a170c78
 https://conda.anaconda.org/conda-forge/osx-64/brotlipy-0.7.0-py310h90acd4f_1005.tar.bz2#63accc45f2b9ae1dad4db9cdfaa903b4
 https://conda.anaconda.org/conda-forge/osx-64/cryptography-41.0.1-py310ha1817de_0.conda#f66541237ec50c9d89228ded177b8d65
 https://conda.anaconda.org/conda-forge/noarch/ghp-import-2.1.0-pyhd8ed1ab_0.tar.bz2#6d8d61116031a3f5b1f32e7899785866
-https://conda.anaconda.org/conda-forge/osx-64/gstreamer-1.22.3-h53e17e3_1.conda#a680a8c0182d9dfbac6cac234306ab67
+https://conda.anaconda.org/conda-forge/osx-64/gstreamer-1.22.4-h840fbdc_0.conda#a24d0265742fe6614ca8d1186c0d8a42
 https://conda.anaconda.org/conda-forge/osx-64/harfbuzz-6.0.0-h08f8713_0.conda#3852d6ef7b77da3e81074a8e487e7df5
 https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.7.0-hd8ed1ab_0.conda#27a4cec373ec84d1c1aa02a1e37f8eaf
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
 https://conda.anaconda.org/conda-forge/osx-64/libitk-5.3.0-h10ab89a_0.conda#73b9bad009f8759bd1854cbc6deca726
 https://conda.anaconda.org/conda-forge/osx-64/liblapacke-3.9.0-17_osx64_mkl.conda#678af3918e54ac46249290a05e7e69b1
 https://conda.anaconda.org/conda-forge/osx-64/libnetcdf-4.8.1-nompi_hc61b76e_106.tar.bz2#502e31e4a400216854da4e9933fb21c2
 https://conda.anaconda.org/conda-forge/noarch/markdown-3.4.3-pyhd8ed1ab_0.conda#89ed59ad509c05db6f5f2f573d499bfe
 https://conda.anaconda.org/conda-forge/noarch/mdit-py-plugins-0.4.0-pyhd8ed1ab_0.conda#6c5358a10873a15398b6f15f60cb5e1f
 https://conda.anaconda.org/conda-forge/osx-64/numpy-1.25.0-py310h7451ae0_0.conda#9accbca17b11eed20ee32b57189e9e66
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.6.0-pyhd8ed1ab_0.conda#741384b21c1b512617f4ee4ea8457c5d
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.8.0-pyhd8ed1ab_0.conda#3e4aca765371893ad848397794600632
 https://conda.anaconda.org/conda-forge/noarch/pybtex-0.24.0-pyhd8ed1ab_2.tar.bz2#2099b86a7399c44c0c61cdb6de6915ba
 https://conda.anaconda.org/conda-forge/osx-64/pyobjc-framework-cocoa-9.2-py310hef2d279_0.conda#0874355241e82a01cd15c6e6b28c7187
 https://conda.anaconda.org/conda-forge/osx-64/pyqt5-sip-12.11.0-py310h415000c_3.conda#6c56916bf99c55b1f57a53ed689f2561
 https://conda.anaconda.org/conda-forge/noarch/python-build-0.10.0-pyhd8ed1ab_1.conda#0ab47ce574f6a8bcb9f2076436e7fedb
 https://conda.anaconda.org/conda-forge/noarch/setuptools-scm-7.1.0-pyhd8ed1ab_0.conda#6613dbb3b25cc648a107f33ca9f80fc1
-https://conda.anaconda.org/conda-forge/osx-64/sqlalchemy-2.0.16-py310h6729b98_0.conda#2cb1231f747d33242f6ae506eb6e9b93
+https://conda.anaconda.org/conda-forge/osx-64/sqlalchemy-2.0.17-py310h6729b98_0.conda#2f7579944d2f1b682ad79c1de277368f
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
 https://conda.anaconda.org/conda-forge/noarch/sympy-1.12-pypyh9d50eac_103.conda#2f7d6347d7acf6edf1ac7f2189f44c8f
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
 https://conda.anaconda.org/conda-forge/osx-64/aiohttp-3.8.4-py310h6729b98_1.conda#513a7cdaa184e2856c358a57205d3837
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
 https://conda.anaconda.org/conda-forge/noarch/black-22.3.0-pyhd8ed1ab_0.tar.bz2#7ecbfaae9a30b73c1a6e36e4a0debc03
 https://conda.anaconda.org/conda-forge/osx-64/blas-devel-3.9.0-17_osx64_mkl.conda#b40b415e2be4d0d2a8d05d0f805240b7
 https://conda.anaconda.org/conda-forge/osx-64/contourpy-1.1.0-py310h88cfcbd_0.conda#0cfd4a8d0f1d785675d5e41e17c8b122
-https://conda.anaconda.org/conda-forge/osx-64/gst-plugins-base-1.22.3-hb5d3a86_1.conda#d01492c656e4a1b5fcd5600a3e745fd5
+https://conda.anaconda.org/conda-forge/osx-64/gst-plugins-base-1.22.4-hb5d3a86_0.conda#3ddc9bb14daecff3a86233f07e0d472a
 https://conda.anaconda.org/conda-forge/osx-64/jupyter_core-5.3.1-py310h2ec42d9_0.conda#2df6b800f29e805b1453a5a32981b873
 https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
 https://conda.anaconda.org/conda-forge/noarch/oauthlib-3.2.2-pyhd8ed1ab_0.tar.bz2#8f882b197fd9c4941a787926baea4868
 https://conda.anaconda.org/conda-forge/osx-64/pandas-1.5.3-py310hecf8f37_1.conda#116e61ed90d0332d30310b2210eb1db4
 https://conda.anaconda.org/conda-forge/osx-64/pango-1.50.14-hbd9bf65_0.conda#7de54d83e9c685b742e0a4d81b271de0
-https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
+https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda#a4986c6bb5b0d05a38855b0880a5f425
 https://conda.anaconda.org/conda-forge/osx-64/pybtex-docutils-1.0.2-py310h2ec42d9_2.tar.bz2#7dac3c5087b676102bf38bd984499219
 https://conda.anaconda.org/conda-forge/noarch/pyopenssl-23.2.0-pyhd8ed1ab_1.conda#34f7d568bf59d18e3fef8c405cbece21
 https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyhd1c38e8_0.conda#2657c3de5371c571aef6678afb4aaadd
 https://conda.anaconda.org/conda-forge/osx-64/simpleitk-2.2.1-py310h4447650_1.conda#ca28f25ff59b4907686307195de35927
 https://conda.anaconda.org/conda-forge/osx-64/blas-2.117-mkl.conda#4c921079b5298ce08bb336fc025b96d7
 https://conda.anaconda.org/conda-forge/noarch/flake8-black-0.3.6-pyhd8ed1ab_0.conda#61649e6e9b39ac0c7d10938025f6fe4f
 https://conda.anaconda.org/conda-forge/osx-64/gtk2-2.24.33-h7c1209e_2.tar.bz2#307614630946527e302b7dd042a5cfa2
-https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.2.0-pyhd8ed1ab_0.conda#58ca2d50c3b27b86fd7df62eaadbf9a9
+https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
 https://conda.anaconda.org/conda-forge/osx-64/librsvg-2.54.4-h3d48ba6_0.tar.bz2#1a106d9119086f73b5f88c650f700210
 https://conda.anaconda.org/conda-forge/osx-64/matplotlib-base-3.7.1-py310he725631_0.conda#8b1caf6e250a7c8270711c301d8bcd2e
 https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda#f525a01528c3eba1d381a232a6971c6a
-https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
+https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.39-hd8ed1ab_0.conda#4bbbe67d5df19db30f04b8e344dc9976
 https://conda.anaconda.org/conda-forge/osx-64/qt-main-5.15.8-h1d3b3f8_6.conda#5d816352174169f7ab45fb54a0fba4ed
 https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.15-pyhd8ed1ab_0.conda#27db656619a55d727eaf5a6ece3d2fd6
-https://conda.anaconda.org/conda-forge/noarch/wslink-1.11.0-pyhd8ed1ab_0.conda#70f4b52c0e703936aa1812d8b14a5bb2
-https://conda.anaconda.org/conda-forge/noarch/botocore-1.29.158-pyhd8ed1ab_0.conda#ccfde1c6ce8dbb4af5590c88a0482248
+https://conda.anaconda.org/conda-forge/noarch/wslink-1.11.1-pyhd8ed1ab_0.conda#0d0113b67472cea3da288838ebc80acb
+https://conda.anaconda.org/conda-forge/noarch/botocore-1.29.165-pyhd8ed1ab_0.conda#0f30016ea54215fdb883b8978340c9b7
 https://conda.anaconda.org/conda-forge/osx-64/graphviz-7.0.5-hc51f7b9_0.conda#589501e7b16648c032a537b6a0870dbe
 https://conda.anaconda.org/conda-forge/noarch/ipython-8.14.0-pyhd1c38e8_0.conda#f56fab4cea853c2248105b6cd7d79bf0
 https://conda.anaconda.org/conda-forge/osx-64/matplotlib-3.7.1-py310h2ec42d9_0.conda#958029c1236746d27149fca648c41cab
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.7.4-pyhd8ed1ab_0.conda#f7aa15f77d29b11caa1df1eb15383c59
 https://conda.anaconda.org/conda-forge/osx-64/pyqt-5.15.7-py310hdd03f62_3.conda#c652959992036327b71a2d5ff593cf72
 https://conda.anaconda.org/pytorch/osx-64/pytorch-2.0.1-py3.10_0.tar.bz2#527aa8793c545ed93288d32bb45d009d
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/osx-64/vtk-9.2.5-qt_py310hea5b068_200.conda#8210705bd78317d38a376b01f6cfab46
-https://conda.anaconda.org/conda-forge/noarch/google-auth-2.20.0-pyh1a96a4e_0.conda#59f942ef9326d2519a7c953f1c24d5da
-https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.2-pyh5fb750a_0.conda#c406de32f968636cd33f6017f5c3f121
+https://conda.anaconda.org/conda-forge/noarch/google-auth-2.21.0-pyh1a96a4e_0.conda#8c5dd8609d314721d990c1d1fd607f81
+https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.3-pyh5fb750a_0.conda#00cfe411a8e07b8322185e573ae7c5a3
 https://conda.anaconda.org/conda-forge/noarch/jupyter-cache-0.6.1-pyhd8ed1ab_0.conda#2e360820ae68e3d28e1a5a9d2714ca5c
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.6.0-pyhd8ed1ab_0.conda#879782bde4bbdb4c7b5d4054504a20d5
 https://conda.anaconda.org/conda-forge/noarch/pooch-1.7.0-pyha770c72_3.conda#5936894aade8240c867d292aa0d980c6
 https://conda.anaconda.org/conda-forge/noarch/requests-oauthlib-1.3.1-pyhd8ed1ab_0.tar.bz2#61b279f051eef9c89d58f4d813e75e04
 https://conda.anaconda.org/conda-forge/noarch/s3transfer-0.6.1-pyhd8ed1ab_0.conda#b19a857ac845097e9c823c9f4d35f80e
 https://conda.anaconda.org/conda-forge/noarch/sphinx-4.5.0-pyh6c4a22f_0.tar.bz2#46b38d88c4270ff9ba78a89c83c66345
 https://conda.anaconda.org/conda-forge/noarch/torchinfo-1.8.0-pyhd8ed1ab_0.conda#fba98fc95a945e2a6b93a77b39dd52dc
 https://conda.anaconda.org/conda-forge/noarch/torchmetrics-0.11.4-pyhd8ed1ab_0.conda#480cb2b6d502003e937d9e4326bc398f
-https://conda.anaconda.org/conda-forge/noarch/boto3-1.26.158-pyhd8ed1ab_0.conda#2e39307a3987518e49eb30ca51e3cfb5
-https://conda.anaconda.org/conda-forge/noarch/google-auth-oauthlib-1.0.0-pyhd8ed1ab_0.conda#5ba9d95acb9add67f468ecdee6595c0f
-https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.6-pyhd8ed1ab_0.conda#68627a08556e4a273e4c7bfc84251457
+https://conda.anaconda.org/pytorch/osx-64/torchvision-0.15.2-py310_cpu.tar.bz2#5c3600915df5413045fc3335c7b66ece
+https://conda.anaconda.org/conda-forge/noarch/boto3-1.26.165-pyhd8ed1ab_0.conda#b9a6316db67d5f2c8dbac2aeb24c6803
+https://conda.anaconda.org/conda-forge/noarch/google-auth-oauthlib-1.0.0-pyhd8ed1ab_1.conda#569e62e95b01b53e4ec7d9abe83b7385
+https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.7-pyhd8ed1ab_0.conda#4b0f4e8fe2a303e472674eae0340bdad
 https://conda.anaconda.org/conda-forge/noarch/jupyter_console-6.6.3-pyhd8ed1ab_0.conda#7cf6f52a66f8e3cd9d8b6c231262dcab
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.6.0-pyhd8ed1ab_0.conda#39fd52b0fcb2fb52bac47a1419bf09bd
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.7.0-pyhd8ed1ab_0.conda#7488cd1f4d35a2af96faa765b7e5b2f0
 https://conda.anaconda.org/conda-forge/noarch/myst-parser-0.18.1-pyhd8ed1ab_0.tar.bz2#bcfdf5c7d8bf5c6f6be7b4c66fff2eca
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.6.0-pyhd8ed1ab_0.conda#e8172ca42f2869bb90185c9356899e81
 https://conda.anaconda.org/conda-forge/noarch/pydata-sphinx-theme-0.13.3-pyhd8ed1ab_0.conda#07aca5f2dea315dcc16680d6891e9056
-https://conda.anaconda.org/conda-forge/noarch/pytorch-lightning-2.0.3-pyhd8ed1ab_0.conda#97138eb8783fa54884216a6562413736
+https://conda.anaconda.org/conda-forge/noarch/pytorch-lightning-2.0.4-pyhd8ed1ab_0.conda#ce9d626b181c6f8cceb5047f6a819f7d
 https://conda.anaconda.org/conda-forge/noarch/qtconsole-base-5.4.3-pyha770c72_0.conda#e0f5e8a6f9ea248e5c2d23efffff08f7
 https://conda.anaconda.org/conda-forge/osx-64/scipy-1.10.1-py310h3900cf1_3.conda#02fb6b5a4f5a89fecae4a11d6bc4a0b1
 https://conda.anaconda.org/conda-forge/noarch/sphinx-comments-0.0.3-pyh9f0ad1d_0.tar.bz2#2ae3ce35de0c1cec45c94182694f8d1b
 https://conda.anaconda.org/conda-forge/noarch/sphinx-copybutton-0.5.2-pyhd8ed1ab_0.conda#ac832cc43adc79118cf6e23f1f9b8995
 https://conda.anaconda.org/conda-forge/noarch/sphinx-design-0.3.0-pyhd8ed1ab_0.tar.bz2#83d1a712e6d2bab6b298b1d2f42ad355
 https://conda.anaconda.org/conda-forge/noarch/sphinx-external-toc-0.3.1-pyhd8ed1ab_0.conda#561bdf7b598d38e2962c46557bd1da12
 https://conda.anaconda.org/conda-forge/noarch/sphinx-jupyterbook-latex-0.5.2-pyhd8ed1ab_0.tar.bz2#88fc7863c8675f297b03e0ca50500b7f
```

### Comparing `hf-deepali-0.3.1/conda/environment.win-64.lock` & `hf-deepali-0.3.2/conda/environment.win-64.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Generated by conda-lock.
 # platform: win-64
-# input_hash: 814107e5f84db920765778d5de91d5b37fbb12ed6d18c265014da09ea659ff50
+# input_hash: fe02ca598f6ebbae4e65d2a2d45af1db4913dae4b25d021473f905afc52e3198
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2023.5.7-h56e8100_0.conda#604212634bd8c4d6f20d44b946e8eedb
 https://conda.anaconda.org/conda-forge/win-64/cuda-cccl-impl-2.0.1-h57928b3_0.conda#6ddbe275ebb9ae875355baf8ade34b3f
 https://conda.anaconda.org/nvidia/win-64/cuda-cudart-11.8.89-0.tar.bz2#cd0f6ab42e0ccba5f6899c531ea193c1
 https://conda.anaconda.org/nvidia/win-64/cuda-cupti-11.8.87-0.tar.bz2#f18f6268a222d476c804d4adadd4926a
 https://conda.anaconda.org/nvidia/win-64/cuda-nvrtc-11.8.89-0.tar.bz2#d692bd090a4a9638ac15709cde2400da
 https://conda.anaconda.org/nvidia/win-64/cuda-nvtx-11.8.86-0.tar.bz2#7874207353c834d34217555785859dba
-https://conda.anaconda.org/nvidia/win-64/cuda-profiler-api-12.1.105-0.tar.bz2#fac1be557eb9ea49655c2d5bd10242d0
+https://conda.anaconda.org/nvidia/win-64/cuda-profiler-api-12.2.53-0.tar.bz2#93cb84c3524a1612cbce98ead299c735
 https://conda.anaconda.org/conda-forge/noarch/cuda-version-12.0-hffde075_2.conda#c9f9d925118c389a1a3f4267b6272b98
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-dejavu-sans-mono-2.37-hab24e00_0.tar.bz2#0c96522c6bdaed4b1566d11387caaf45
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-inconsolata-3.000-h77eed37_0.tar.bz2#34893075a5c9e55cdafac56607368fc6
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-source-code-pro-2.038-h77eed37_0.tar.bz2#4d59c254e01d9cde7957100457e2d5fb
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-ubuntu-0.83-hab24e00_0.tar.bz2#19410c3df09dfb12d1206132a1d357c5
 https://conda.anaconda.org/conda-forge/win-64/intel-openmp-2023.1.0-h57928b3_46319.conda#dbc4636f419722fbf3ab6501377228ba
 https://conda.anaconda.org/nvidia/win-64/libcublas-11.11.3.6-0.tar.bz2#750e01875ed59059ae043d09d262968d
@@ -40,20 +40,20 @@
 https://conda.anaconda.org/nvidia/win-64/libcufft-dev-10.9.0.58-0.tar.bz2#3324bab83e7415785abdcc80ebceda72
 https://conda.anaconda.org/nvidia/win-64/libcusolver-dev-11.4.1.48-0.tar.bz2#5be85962afcb4326fc6e80294d2b15e5
 https://conda.anaconda.org/nvidia/win-64/libcusparse-dev-11.7.5.86-0.tar.bz2#e2fe98ab4b1442f85024c2fe96bc7a61
 https://conda.anaconda.org/nvidia/win-64/libnpp-dev-11.8.0.86-0.tar.bz2#b7a4f974dec24d055e46217db1b263a6
 https://conda.anaconda.org/nvidia/win-64/libnvjpeg-dev-11.9.0.86-0.tar.bz2#f116753a5673e7b113f5e06081059f6d
 https://conda.anaconda.org/conda-forge/win-64/m2w64-gmp-6.1.0-2.tar.bz2#53a1c73e1e3d185516d7e3af177596d9
 https://conda.anaconda.org/conda-forge/win-64/m2w64-libwinpthread-git-5.0.0.4634.697f757-2.tar.bz2#774130a326dee16f1ceb05cc687ee4f0
-https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.34.31931-h5081d32_16.conda#22125178654c6a8a393f9743d585704b
+https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.36.32532-hfdfe4a8_17.conda#91c1ecaf3996889532fc0456178b1058
 https://conda.anaconda.org/conda-forge/win-64/cuda-cccl-12.0.90-h57928b3_1.conda#f1ceeb722d224d7be3ea7cd33abe5e25
 https://conda.anaconda.org/conda-forge/noarch/fonts-conda-ecosystem-1-0.tar.bz2#fee5683a3f04bd15cbd8318b096a27ab
 https://conda.anaconda.org/conda-forge/win-64/m2w64-gcc-libs-core-5.3.0-7.tar.bz2#4289d80fb4d272f1f3b56cfe87ac90bd
-https://conda.anaconda.org/conda-forge/win-64/vc-14.3-hb25d44b_16.conda#ea326b37e3bd6d2616988e09f3a9396c
-https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.34.31931-hed1258a_16.conda#0374eae69b6dbfb27c3dc27167109eb4
+https://conda.anaconda.org/conda-forge/win-64/vc-14.3-h64f974e_17.conda#67ff6791f235bb606659bf2a5c169191
+https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.36.32532-h05e6639_17.conda#4618046c39f7c81861e53ded842e738a
 https://conda.anaconda.org/conda-forge/win-64/aom-3.5.0-h63175ca_0.tar.bz2#455524d2bf9625a42a1848c0d08ac063
 https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-h8ffe710_4.tar.bz2#7c03c66026944073040cb19a4f3ec3c9
 https://conda.anaconda.org/conda-forge/win-64/c-ares-1.19.1-hcfcfb64_0.conda#8aa74d9a74ed3a31d9ed38a387a8ca50
 https://conda.anaconda.org/nvidia/win-64/cuda-cudart-dev-11.8.89-0.tar.bz2#a4b0b3a1b7aa79ff39f6d3b1e7c62de3
 https://conda.anaconda.org/conda-forge/win-64/dav1d-1.2.0-hcfcfb64_0.conda#0ce7020bd3aadfb999f987d2b1cc0e25
 https://conda.anaconda.org/conda-forge/win-64/double-conversion-3.2.0-h63175ca_1.tar.bz2#d1b86ea3cf6e902694a592e6440b1fa5
 https://conda.anaconda.org/conda-forge/win-64/eigen-3.4.0-h2d74725_0.tar.bz2#72fab4b0a033b718950cc5d930cbd1a6
@@ -62,27 +62,27 @@
 https://conda.anaconda.org/conda-forge/win-64/getopt-win32-0.1-h8ffe710_0.tar.bz2#9ac4874e2958f18e01c386649208fe40
 https://conda.anaconda.org/conda-forge/win-64/glew-2.1.0-h39d44d4_2.tar.bz2#840d21c1ee66b91af3d0211e7766393a
 https://conda.anaconda.org/conda-forge/win-64/graphite2-1.3.13-1000.tar.bz2#8fc0e04e5c852cadf2cad68b86a906ab
 https://conda.anaconda.org/conda-forge/win-64/icu-70.1-h0e60522_0.tar.bz2#64073396a905b6df895ab2489fae3847
 https://conda.anaconda.org/conda-forge/win-64/jpeg-9e-hcfcfb64_3.conda#824f1e030d224e9e376a4655032fdbc7
 https://conda.anaconda.org/conda-forge/win-64/jsoncpp-1.9.5-h2d74725_1.tar.bz2#733179d30b9132159d9db5ed85b6c841
 https://conda.anaconda.org/conda-forge/win-64/lerc-4.0.0-h63175ca_0.tar.bz2#1900cb3cab5055833cfddb0ba233b074
-https://conda.anaconda.org/conda-forge/win-64/libabseil-20230125.2-cxx17_h63175ca_2.conda#828f6bb057da235a4703ed33192f81c5
+https://conda.anaconda.org/conda-forge/win-64/libabseil-20230125.3-cxx17_h63175ca_0.conda#219d819db61ee021a82ecee3d69642cd
 https://conda.anaconda.org/conda-forge/win-64/libaec-1.0.6-h63175ca_1.conda#f98474a8245f55f4a273889dbe7bf193
-https://conda.anaconda.org/conda-forge/win-64/libbrotlicommon-1.0.9-hcfcfb64_8.tar.bz2#e8078e37208cd7d3e1eb5053f370ded8
+https://conda.anaconda.org/conda-forge/win-64/libbrotlicommon-1.0.9-hcfcfb64_9.conda#5e0f7bd6f1d0747abd5da59cffb6f533
 https://conda.anaconda.org/conda-forge/win-64/libcurand-10.3.1.50-h63175ca_0.conda#aebb58b22a91bb91886b1487e96e43d1
 https://conda.anaconda.org/conda-forge/win-64/libdeflate-1.14-hcfcfb64_0.tar.bz2#4366e00d3270eb229c026920474a6dda
 https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2#2c96d1b6915b408893f9472569dee135
 https://conda.anaconda.org/conda-forge/win-64/libiconv-1.17-h8ffe710_0.tar.bz2#050119977a86e4856f0416e2edcf81bb
 https://conda.anaconda.org/conda-forge/win-64/libogg-1.3.4-h8ffe710_1.tar.bz2#04286d905a0dcb7f7d4a12bdfe02516d
 https://conda.anaconda.org/conda-forge/win-64/libopus-1.3.1-h8ffe710_1.tar.bz2#e35a6bcfeb20ea83aab21dfc50ae62a4
 https://conda.anaconda.org/conda-forge/win-64/libsodium-1.0.18-h8d14728_1.tar.bz2#5c1fb45b5e2912c19098750ae8a32604
 https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.42.0-hcfcfb64_0.conda#9a71d93deb99cc09d8939d5235b5909a
 https://conda.anaconda.org/conda-forge/win-64/libuv-1.44.2-h8ffe710_0.tar.bz2#0d45ae978c33ff0b5f95ea24c717d5cf
-https://conda.anaconda.org/conda-forge/win-64/libwebp-base-1.3.0-hcfcfb64_0.conda#381a3645c51cbf478872899b16490318
+https://conda.anaconda.org/conda-forge/win-64/libwebp-base-1.3.1-hcfcfb64_0.conda#f89e765213cac556a8ed72ba8c1b5071
 https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_5.conda#5fdb9c6a113b6b6cb5e517fd972d5f41
 https://conda.anaconda.org/conda-forge/win-64/lz4-c-1.9.4-hcfcfb64_0.conda#e34720eb20a33fc3bfb8451dd837ab7a
 https://conda.anaconda.org/conda-forge/win-64/m2w64-gcc-libgfortran-5.3.0-6.tar.bz2#066552ac6b907ec6d72c0ddab29050dc
 https://conda.anaconda.org/conda-forge/win-64/openh264-2.3.1-h63175ca_2.conda#76e822d93cdc32b00b61810d3fa030e0
 https://conda.anaconda.org/conda-forge/win-64/openssl-3.1.1-hcfcfb64_1.conda#1d913a5de46c6b2f7e4cfbd26b106b8b
 https://conda.anaconda.org/conda-forge/win-64/pixman-0.40.0-h8ffe710_0.tar.bz2#32b45d3fcffddc84cc1a014a0b5f0d58
 https://conda.anaconda.org/conda-forge/win-64/pthreads-win32-2.9.1-hfa6e2cd_3.tar.bz2#e2da8758d7d51ff6aa78a14dfb9dbed4
@@ -93,75 +93,75 @@
 https://conda.anaconda.org/conda-forge/win-64/x264-1!164.3095-h8ffe710_2.tar.bz2#19e39905184459760ccb8cf5c75f148b
 https://conda.anaconda.org/conda-forge/win-64/x265-3.5-h2d74725_3.tar.bz2#ca7129a334198f08347fb19ac98a2de9
 https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2#515d77642eaa3639413c6b1bc3f94219
 https://conda.anaconda.org/conda-forge/win-64/yaml-0.2.5-h8ffe710_2.tar.bz2#adbfb9f45d1004a26763652246a33764
 https://conda.anaconda.org/nvidia/win-64/cuda-libraries-11.8.0-0.tar.bz2#4a0d16015f1480c6b6845a4d17b9563b
 https://conda.anaconda.org/conda-forge/win-64/gettext-0.21.1-h5728263_0.tar.bz2#299d4fd6798a45337042ff5a48219e5f
 https://conda.anaconda.org/conda-forge/win-64/krb5-1.20.1-heb0366b_0.conda#a07b05ee8f451ab15698397185efe989
-https://conda.anaconda.org/conda-forge/win-64/libbrotlidec-1.0.9-hcfcfb64_8.tar.bz2#99839d9d81f33afa173c0fa82a702038
-https://conda.anaconda.org/conda-forge/win-64/libbrotlienc-1.0.9-hcfcfb64_8.tar.bz2#88e62627120c20289bf8982b15e0a6a1
+https://conda.anaconda.org/conda-forge/win-64/libbrotlidec-1.0.9-hcfcfb64_9.conda#4c502e4846bdc22b944ab9aa5a55a58f
+https://conda.anaconda.org/conda-forge/win-64/libbrotlienc-1.0.9-hcfcfb64_9.conda#19029748649ae0d48871d7012918efef
 https://conda.anaconda.org/conda-forge/win-64/libclang13-15.0.7-default_h77d9078_2.conda#c2e1def32a19610ac26db453501760b6
 https://conda.anaconda.org/conda-forge/win-64/libcurand-dev-10.3.1.50-h63175ca_0.conda#e6c08a829cbd187b1b0e2eafa8f2712e
 https://conda.anaconda.org/conda-forge/win-64/libpng-1.6.39-h19919ed_0.conda#ab6febdb2dbd9c00803609079db4de71
-https://conda.anaconda.org/conda-forge/win-64/libprotobuf-4.23.2-h1975477_5.conda#f37b557f68140eec8421e35698c36478
+https://conda.anaconda.org/conda-forge/win-64/libprotobuf-4.23.3-h1975477_0.conda#6386184da6e9e58de0d8e0a9e9aeb736
 https://conda.anaconda.org/conda-forge/win-64/libssh2-1.11.0-h7dfc565_0.conda#dc262d03aae04fe26825062879141a41
 https://conda.anaconda.org/conda-forge/win-64/libtheora-1.1.1-h8d14728_1005.tar.bz2#8ad3f8ea1dbd5ac4fe1299a3250cbd1b
 https://conda.anaconda.org/conda-forge/win-64/libvorbis-1.3.7-h0e60522_0.tar.bz2#e1a22282de0169c93e4ffe6ce6acc212
-https://conda.anaconda.org/conda-forge/win-64/libwebp-1.3.0-hcfcfb64_0.conda#0c1f2c4b45406631c600ec22ca9523fc
+https://conda.anaconda.org/conda-forge/win-64/libwebp-1.3.1-hcfcfb64_0.conda#cc9d668f51da7f6506185ab1130bcd57
 https://conda.anaconda.org/conda-forge/win-64/libxml2-2.10.4-hc3477c8_0.conda#d9869d2d502cca6b6f73dd7030696b3c
 https://conda.anaconda.org/conda-forge/win-64/libzip-1.9.2-h519de47_1.tar.bz2#9c3138e53e36c0c161a23d20db91297b
 https://conda.anaconda.org/conda-forge/win-64/m2w64-gcc-libs-5.3.0-7.tar.bz2#fe759119b8b3bfa720b8762c6fdc35de
 https://conda.anaconda.org/conda-forge/win-64/pcre2-10.40-h17e33f8_0.tar.bz2#2519de0d9620dc2bc7e19caf6867136d
-https://conda.anaconda.org/conda-forge/win-64/python-3.10.11-h4de0772_0_cpython.conda#db564a923e0197854756c727ad3e4b8f
+https://conda.anaconda.org/conda-forge/win-64/python-3.10.12-h4de0772_0_cpython.conda#14273454ca348a123ce09ab9d39c1a6e
 https://conda.anaconda.org/conda-forge/win-64/sqlite-3.42.0-hcfcfb64_0.conda#c505cc64dba674d4c419c0de772c8579
 https://conda.anaconda.org/conda-forge/win-64/zeromq-4.3.4-h0e60522_1.tar.bz2#e1aff0583dda5fb917eb3d2c1025aa80
 https://conda.anaconda.org/conda-forge/win-64/zlib-1.2.13-hcfcfb64_5.conda#a318e8622e11663f645cc7fa3260f462
 https://conda.anaconda.org/conda-forge/win-64/zstd-1.5.2-h12be248_6.conda#62826565682d013b3e2346aaf7bded0e
 https://conda.anaconda.org/conda-forge/noarch/absl-py-1.4.0-pyhd8ed1ab_0.conda#dd5eed01874c75bebef810a2faec673e
 https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.13-pyhd8ed1ab_0.conda#06006184e203b61d3525f90de394471e
 https://conda.anaconda.org/conda-forge/noarch/attrs-21.4.0-pyhd8ed1ab_0.tar.bz2#f70280205d7044c8b8358c8de3190e5d
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
 https://conda.anaconda.org/conda-forge/noarch/blinker-1.6.2-pyhd8ed1ab_0.conda#2fb79ec81bad9492b6d59a06b3b647a4
-https://conda.anaconda.org/conda-forge/win-64/brotli-bin-1.0.9-hcfcfb64_8.tar.bz2#e18b70ed349d96086fd60a9c642b1b58
-https://conda.anaconda.org/conda-forge/noarch/cachetools-5.3.0-pyhd8ed1ab_0.conda#fd006afc4115740d8d52887ee813f262
+https://conda.anaconda.org/conda-forge/win-64/brotli-bin-1.0.9-hcfcfb64_9.conda#ba8ae6c24cf47da3fb73270e4f119f08
+https://conda.anaconda.org/conda-forge/noarch/cachetools-5.3.1-pyhd8ed1ab_0.conda#60b5eb16d9a7a5482ba37f67aa49db5b
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
 https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/nvidia/win-64/cuda-libraries-dev-11.8.0-0.tar.bz2#4dceddb905013e47bee99757d42dfdd4
 https://conda.anaconda.org/nvidia/win-64/cuda-runtime-11.8.0-0.tar.bz2#9782ebd2dc96d2fd463c0d4a99254da6
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.11.0-pyhd8ed1ab_0.tar.bz2#a50559fad0affdbb33729a68669ca1cb
 https://conda.anaconda.org/conda-forge/noarch/dataclasses-0.8-pyhc8e2a94_3.tar.bz2#a362b2124b06aad102e2ee4581acee7d
 https://conda.anaconda.org/conda-forge/win-64/debugpy-1.6.7-py310h00ffb61_0.conda#b7defb941402f3581384d16070ed1456
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
 https://conda.anaconda.org/conda-forge/win-64/docutils-0.17.1-py310h5588dad_3.tar.bz2#cdc0acfc953b7bd34229b7f229eae46a
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
-https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
 https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
 https://conda.anaconda.org/conda-forge/noarch/filelock-3.12.2-pyhd8ed1ab_0.conda#53522ec72e6adae42bd373ef58357230
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/win-64/freetype-2.12.1-h546665d_1.conda#1b513009cd012591f3fdc9e03a74ec0a
 https://conda.anaconda.org/conda-forge/win-64/frozenlist-1.3.3-py310h8d17308_0.tar.bz2#550271ca005a4c805cd7391cef008dc6
 https://conda.anaconda.org/conda-forge/noarch/fsspec-2023.6.0-pyh1a96a4e_0.conda#50ea2067ec92dfcc38b4f07992d7e235
 https://conda.anaconda.org/conda-forge/win-64/gl2ps-1.4.2-h0597ee9_0.tar.bz2#9f17f1b93f610b4bea2a256d528fe8f6
 https://conda.anaconda.org/conda-forge/win-64/greenlet-2.0.2-py310h00ffb61_1.conda#7535b10dbe0b5fbf63fede10a4f8666b
 https://conda.anaconda.org/conda-forge/win-64/hdf4-4.2.15-h1b1b6ef_5.tar.bz2#bfb6a2d82ef9a30455cc0900d89eed20
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
 https://conda.anaconda.org/conda-forge/noarch/ipython_genutils-0.2.0-py_1.tar.bz2#5071c982548b3a20caf70462f04f5287
 https://conda.anaconda.org/conda-forge/noarch/jmespath-1.0.1-pyhd8ed1ab_0.tar.bz2#2cfa3e1cf3fb51bb9b17acc5b5e9ea11
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.7-pyhd8ed1ab_1.conda#0c0a54e16b764bafcae35913cc9d60ff
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.8-pyhd8ed1ab_0.conda#2bc3ca2f7387af385dd06706b4fb2d35
 https://conda.anaconda.org/conda-forge/win-64/kiwisolver-1.4.4-py310h232114e_1.tar.bz2#c55fe943d5f212d49d27d08580f5a610
 https://conda.anaconda.org/conda-forge/win-64/lazy-object-proxy-1.9.0-py310h8d17308_0.conda#696baee03eafd09ed9c4ab6a095b620f
 https://conda.anaconda.org/conda-forge/win-64/libclang-15.0.7-default_h77d9078_2.conda#70188b1b3e0b1716405adab9050894d1
 https://conda.anaconda.org/conda-forge/win-64/libcurl-8.1.2-h68f0423_0.conda#94b9b7d0e882461fdb72d8d4e7441746
 https://conda.anaconda.org/conda-forge/win-64/libglib-2.76.3-he8f3873_0.conda#4695e6acaf4790170161048d56cb51fc
-https://conda.anaconda.org/conda-forge/win-64/libgrpc-1.55.1-h0c1e3fa_1.conda#5eb83620ff9214afd3cc3cf3d9d87a33
+https://conda.anaconda.org/conda-forge/win-64/libgrpc-1.56.0-hea2d5f7_2.conda#44b832412b9a71277e67ecc52ffec4f2
 https://conda.anaconda.org/conda-forge/win-64/libhwloc-2.9.1-h51c2c0f_0.conda#8ec5920f3ed67faa0264a36c0b533ed0
 https://conda.anaconda.org/conda-forge/win-64/libtiff-4.4.0-hc4f729c_5.conda#fe00c2f95c1215e355c34094b00480d7
 https://conda.anaconda.org/conda-forge/win-64/markupsafe-2.1.3-py310h8d17308_0.conda#e6deeae9d0dac4d17c6ef2fa62b3efff
 https://conda.anaconda.org/conda-forge/noarch/mccabe-0.7.0-pyhd8ed1ab_0.tar.bz2#34fc335fc50eef0b5ea708f2b5f54e0c
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
 https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda#c7d0ea64c37752ecbe6da458aee662d2
 https://conda.anaconda.org/conda-forge/noarch/mpmath-1.3.0-pyhd8ed1ab_0.conda#dbf6e2d89137da32fa6670f3bffc024e
@@ -172,15 +172,15 @@
 https://conda.anaconda.org/conda-forge/noarch/networkx-3.1-pyhd8ed1ab_0.conda#254f787d5068bc89f578bf63893ce8b4
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
 https://conda.anaconda.org/conda-forge/noarch/pathspec-0.11.1-pyhd8ed1ab_0.conda#dbb80d1e8dc2dba5c8b106dc0768ad45
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
-https://conda.anaconda.org/conda-forge/noarch/pluggy-1.0.0-pyhd8ed1ab_5.tar.bz2#7d301a0d25f424d96175f810935f0da9
+https://conda.anaconda.org/conda-forge/noarch/pluggy-1.2.0-pyhd8ed1ab_0.conda#7263924c642d22e311d9e59b839f1b33
 https://conda.anaconda.org/conda-forge/noarch/ply-3.11-py_1.tar.bz2#7205635cd71531943440fbfe3b6b5727
 https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.0-pyhd8ed1ab_0.conda#95c5be3c7cbd872509d16c216617fdab
 https://conda.anaconda.org/conda-forge/win-64/psutil-5.9.5-py310h8d17308_0.conda#9f98965e4f7dc2e4eb84abd50406d3a0
 https://conda.anaconda.org/conda-forge/win-64/pthread-stubs-0.4-hcd874cb_1001.tar.bz2#a1f820480193ea83582b13249a7e7bd9
 https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
 https://conda.anaconda.org/conda-forge/noarch/pyasn1-0.4.8-py_0.tar.bz2#06d04c9f8f72ac77911db942eda24fb9
 https://conda.anaconda.org/conda-forge/noarch/pycodestyle-2.10.0-pyhd8ed1ab_0.conda#89843e4cc99c6a3fe5f4c86994cc8410
@@ -211,24 +211,24 @@
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-serializinghtml-1.1.5-pyhd8ed1ab_2.tar.bz2#9ff55a0901cf952f05c654394de76bf7
 https://conda.anaconda.org/conda-forge/noarch/tabulate-0.9.0-pyhd8ed1ab_1.tar.bz2#4759805cce2d914c38472f70bf4d8bcb
 https://conda.anaconda.org/conda-forge/win-64/tensorboard-data-server-0.7.0-py310h5588dad_0.conda#1aa33e391e578ec1f6b23d10e005aa2e
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/win-64/tornado-6.3.2-py310h8d17308_0.conda#6cd035ff75b46eb8ae7403b3dded2def
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
-https://conda.anaconda.org/conda-forge/win-64/typed-ast-1.5.4-py310h8d17308_1.tar.bz2#5cc75fe139b6fa921326677120d44893
+https://conda.anaconda.org/conda-forge/win-64/typed-ast-1.5.5-py310h8d17308_0.conda#a2ac0e6c5a06b35dea207c3d77f94f74
 https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.3-pyha770c72_0.conda#4a3014a4d107d15475d106b751c4e352
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/noarch/uc-micro-py-1.0.1-pyhd8ed1ab_0.tar.bz2#3ddf6684d9b274a12c94e509ca45656c
 https://conda.anaconda.org/conda-forge/win-64/unicodedata2-15.0.0-py310h8d17308_0.tar.bz2#5d14ba562f7740b64be9c8059498cfbf
 https://conda.anaconda.org/conda-forge/noarch/unidecode-1.3.6-pyhd8ed1ab_0.tar.bz2#e8f24401b17802df5f82f66a88cee29e
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
-https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.0-pyhd8ed1ab_0.conda#1dd6387a73d84e16b6f73de676bb4c36
+https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda#c34d9325a609381a0b0e8a5b4f325147
 https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
-https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
+https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.8-pyhd8ed1ab_0.conda#2e9ebddf0b93d0fb203d0906b8052c4f
 https://conda.anaconda.org/conda-forge/noarch/win32_setctime-1.1.0-pyhd8ed1ab_0.tar.bz2#dc80c0c2b01f7d6d6d5df4b63ef54f17
 https://conda.anaconda.org/conda-forge/noarch/win_inet_pton-1.1.0-pyhd8ed1ab_6.tar.bz2#30878ecc4bd36e8deeea1e3c151b2e0b
 https://conda.anaconda.org/conda-forge/win-64/wrapt-1.15.0-py310h8d17308_0.conda#2ec4d850e6fbe1da9971a7bb801a1ebd
 https://conda.anaconda.org/conda-forge/win-64/xorg-kbproto-1.0.7-hcd874cb_1002.tar.bz2#8d11c1dac4756ca57e78c1bfe173bba4
 https://conda.anaconda.org/conda-forge/win-64/xorg-libice-1.0.10-hcd874cb_0.tar.bz2#8f45beee385cb67e42d6732bdb1b6a40
 https://conda.anaconda.org/conda-forge/win-64/xorg-libxau-1.0.11-hcd874cb_0.conda#c46ba8712093cb0114404ae8a7582e1a
 https://conda.anaconda.org/conda-forge/win-64/xorg-libxdmcp-1.1.3-hcd874cb_0.tar.bz2#46878ebb6b9cbd8afcf8088d7ef00ece
@@ -236,48 +236,48 @@
 https://conda.anaconda.org/conda-forge/win-64/xorg-xproto-7.0.31-hcd874cb_1007.tar.bz2#88f3c65d2ad13826a9e0b162063be023
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
 https://conda.anaconda.org/conda-forge/noarch/accessible-pygments-0.0.4-pyhd8ed1ab_0.conda#46a2e6e3dfa718ce3492018d5a110dd6
 https://conda.anaconda.org/conda-forge/noarch/aiosignal-1.3.1-pyhd8ed1ab_0.tar.bz2#d1e1eb7e21a9e2c74279d87dafb68156
 https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.0-pyhd8ed1ab_1.conda#2b35a85d654a47aac8f34c1bb6de7142
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
-https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.4-pyhd8ed1ab_0.tar.bz2#c5b3edc62d6309088f4970b3eaaa65a6
+https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
-https://conda.anaconda.org/conda-forge/win-64/brotli-1.0.9-hcfcfb64_8.tar.bz2#2e661f21e1741c11506bdc7226e6b0bc
+https://conda.anaconda.org/conda-forge/win-64/brotli-1.0.9-hcfcfb64_9.conda#5275e2634840f6d156934a16b7c0c813
 https://conda.anaconda.org/conda-forge/win-64/cffi-1.15.1-py310h628cb3f_3.conda#b7ca236d34501eb6a70691c1e29a0234
 https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-win_pyhd8ed1ab_2.tar.bz2#6b58680207b526c42dcff68b543803dd
 https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda#168ae0f82cdf7505048e81054c7354e4
 https://conda.anaconda.org/conda-forge/win-64/curl-8.1.2-h68f0423_0.conda#fc67d347f9eaa7922fd7bc26bfa5419b
 https://conda.anaconda.org/conda-forge/noarch/dacite-1.8.0-pyhd8ed1ab_0.conda#3696792ba70ab3374320fe6041a82286
 https://conda.anaconda.org/conda-forge/noarch/deprecation-2.1.0-pyh9f0ad1d_0.tar.bz2#7b6747d7cc2076341029cff659669e8b
 https://conda.anaconda.org/conda-forge/noarch/flake8-6.0.0-pyhd8ed1ab_0.conda#e9345ba05d71742412b8aa6992ad9457
 https://conda.anaconda.org/conda-forge/win-64/fontconfig-2.14.2-hbde0cde_0.conda#08767992f1a4f1336a257af1241034bd
 https://conda.anaconda.org/conda-forge/win-64/glib-tools-2.76.3-h12be248_0.conda#3015483cb3ffa200d51aac3c691fcda0
-https://conda.anaconda.org/conda-forge/win-64/grpcio-1.55.1-py310hb84602e_1.conda#30bee6092170c8b57d96b90baa25d176
+https://conda.anaconda.org/conda-forge/win-64/grpcio-1.56.0-py310hb84602e_2.conda#c624ac3dd1ada404b8d8cc378bb60daf
 https://conda.anaconda.org/conda-forge/win-64/gts-0.7.6-h6b5321d_4.conda#a41f14768d5e377426ad60c613f2923b
 https://conda.anaconda.org/conda-forge/win-64/hdf5-1.12.2-nompi_h57737ce_101.conda#3e2b84f2f7bcf6915d1baa21e5b1a862
 https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.7.0-pyha770c72_0.conda#ba3786c6846e46038fe60c785d46dc81
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
 https://conda.anaconda.org/conda-forge/noarch/latexcodec-2.0.1-pyh9f0ad1d_0.tar.bz2#8d67904973263afd2985ba56aa2d6bb4
 https://conda.anaconda.org/conda-forge/win-64/lcms2-2.14-h90d422f_0.tar.bz2#a0deec92aa16fca7bf5a6717d05f88ee
 https://conda.anaconda.org/conda-forge/win-64/libxcb-1.13-hcd874cb_1004.tar.bz2#a6d7fd030532378ecb6ba435cd9f8234
-https://conda.anaconda.org/conda-forge/noarch/lightning-utilities-0.8.0-pyhd8ed1ab_0.conda#ad16f58b64d3b41f4cbb75040b06c9cc
+https://conda.anaconda.org/conda-forge/noarch/lightning-utilities-0.9.0-pyhd8ed1ab_0.conda#c71f7ec8b80a536e58b979299b230251
 https://conda.anaconda.org/conda-forge/noarch/linkify-it-py-2.0.0-pyhd8ed1ab_0.tar.bz2#25b93e66067eb496ac10da888e25cc33
 https://conda.anaconda.org/conda-forge/win-64/loguru-0.7.0-py310h5588dad_0.conda#418204da701dc43d8992ba8131c17848
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-2.2.0-pyhd8ed1ab_0.conda#b2928a6c6d52d7e3562b4a59c3214e3a
 https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
 https://conda.anaconda.org/conda-forge/win-64/openjpeg-2.5.0-hc9384bd_1.tar.bz2#a6834096f8d834339eca7ef4d23bcc44
 https://conda.anaconda.org/conda-forge/noarch/overrides-7.3.1-pyhd8ed1ab_0.tar.bz2#a5745ced46e69aa9754053ba061974ab
 https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
 https://conda.anaconda.org/conda-forge/win-64/proj-9.1.0-h3863b3b_0.tar.bz2#40201019efe10a1373387506cffa8cb1
-https://conda.anaconda.org/conda-forge/win-64/protobuf-4.23.2-py310ha3d488f_1.conda#e2a566087d11bbcf502aeaffdd37fe3d
+https://conda.anaconda.org/conda-forge/win-64/protobuf-4.23.3-py310ha3d488f_0.conda#a65f902a101c1ec7bedfe48b65756379
 https://conda.anaconda.org/conda-forge/noarch/pyasn1-modules-0.2.7-py_0.tar.bz2#ad1e886d09700b2304975335f714bd9c
 https://conda.anaconda.org/conda-forge/noarch/pyproject_hooks-1.0.0-pyhd8ed1ab_0.conda#21de50391d584eb7f4441b9de1ad773f
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyh0701188_6.tar.bz2#56cd9fe388baac0e90c7149cfac95b60
 https://conda.anaconda.org/conda-forge/noarch/pytest-7.3.2-pyhd8ed1ab_1.conda#f2465696f4396245eca4613f6e924796
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
 https://conda.anaconda.org/pytorch/win-64/pytorch-cuda-11.8-h24eeafa_5.tar.bz2#6c31007cf6837eac42629e117ef1d947
 https://conda.anaconda.org/conda-forge/noarch/pyu2f-0.1.5-pyhd8ed1ab_0.tar.bz2#caabbeaa83928d0c3e3949261daa18eb
@@ -310,79 +310,79 @@
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
 https://conda.anaconda.org/conda-forge/win-64/libitk-5.3.0-h6e1890f_0.conda#705a9011eeac84184b34f157ca927ec0
 https://conda.anaconda.org/conda-forge/win-64/libnetcdf-4.8.1-nompi_h8c042bf_106.tar.bz2#90515eee0f7575b5fd296b6ba8d91dae
 https://conda.anaconda.org/conda-forge/noarch/markdown-3.4.3-pyhd8ed1ab_0.conda#89ed59ad509c05db6f5f2f573d499bfe
 https://conda.anaconda.org/conda-forge/noarch/mdit-py-plugins-0.4.0-pyhd8ed1ab_0.conda#6c5358a10873a15398b6f15f60cb5e1f
 https://conda.anaconda.org/conda-forge/win-64/mkl-2022.1.0-h6a75c08_874.tar.bz2#2ff89a7337a9636029b4db9466e9f8e3
 https://conda.anaconda.org/conda-forge/win-64/pillow-9.2.0-py310hd4fb230_3.tar.bz2#96a1ddd65392fb64636dd8311f862e14
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.6.0-pyhd8ed1ab_0.conda#741384b21c1b512617f4ee4ea8457c5d
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.8.0-pyhd8ed1ab_0.conda#3e4aca765371893ad848397794600632
 https://conda.anaconda.org/conda-forge/noarch/pybtex-0.24.0-pyhd8ed1ab_2.tar.bz2#2099b86a7399c44c0c61cdb6de6915ba
 https://conda.anaconda.org/conda-forge/win-64/pyqt5-sip-12.11.0-py310h00ffb61_3.conda#a4c757150f616bae079bc08cea956138
 https://conda.anaconda.org/conda-forge/noarch/python-build-0.10.0-pyhd8ed1ab_1.conda#0ab47ce574f6a8bcb9f2076436e7fedb
 https://conda.anaconda.org/conda-forge/noarch/setuptools-scm-7.1.0-pyhd8ed1ab_0.conda#6613dbb3b25cc648a107f33ca9f80fc1
-https://conda.anaconda.org/conda-forge/win-64/sqlalchemy-2.0.16-py310h8d17308_0.conda#650d1be95b2cba2e37d0a0fe13f3c509
+https://conda.anaconda.org/conda-forge/win-64/sqlalchemy-2.0.17-py310h8d17308_0.conda#1a7ef45ab2cbed2272dc7bed9ee6f98a
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
 https://conda.anaconda.org/conda-forge/win-64/tbb-devel-2021.9.0-h91493d7_0.conda#ece1b712d5d6c96f916ec0f11e52b391
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
 https://conda.anaconda.org/conda-forge/win-64/xorg-libx11-1.8.4-hcd874cb_0.conda#ebdb02b455647e13fa697da89d9bdf84
 https://conda.anaconda.org/conda-forge/win-64/aiohttp-3.8.4-py310h8d17308_1.conda#c759aad020f1363a27088e6c621f4db1
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
 https://conda.anaconda.org/conda-forge/noarch/black-22.3.0-pyhd8ed1ab_0.tar.bz2#7ecbfaae9a30b73c1a6e36e4a0debc03
-https://conda.anaconda.org/conda-forge/win-64/gstreamer-1.22.3-h6b5321d_1.conda#00afb31665a8028ca2ff9af61fea64e1
+https://conda.anaconda.org/conda-forge/win-64/gstreamer-1.22.4-hb4038d2_0.conda#ead79af9af7587ca3f685fed4966a881
 https://conda.anaconda.org/conda-forge/win-64/harfbuzz-6.0.0-he256f1b_0.conda#15422d4ff786ed835173cfb8e6735679
 https://conda.anaconda.org/conda-forge/win-64/jupyter_core-5.3.1-py310h5588dad_0.conda#39614170bdabdaa7531cb1dc2846c37c
 https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
 https://conda.anaconda.org/conda-forge/win-64/libblas-3.9.0-17_win64_mkl.conda#9e42ac6b256b96bfaa19f829c25940e8
 https://conda.anaconda.org/conda-forge/win-64/mkl-devel-2022.1.0-h57928b3_875.tar.bz2#6319a06307af296c1dfae93687c283b2
 https://conda.anaconda.org/conda-forge/noarch/oauthlib-3.2.2-pyhd8ed1ab_0.tar.bz2#8f882b197fd9c4941a787926baea4868
-https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
+https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda#a4986c6bb5b0d05a38855b0880a5f425
 https://conda.anaconda.org/conda-forge/win-64/pybtex-docutils-1.0.2-py310h5588dad_2.tar.bz2#a69da1e6eb6ce9a7794d379a54e06990
 https://conda.anaconda.org/conda-forge/noarch/pyopenssl-23.2.0-pyhd8ed1ab_1.conda#34f7d568bf59d18e3fef8c405cbece21
 https://conda.anaconda.org/conda-forge/win-64/simpleitk-2.2.1-py310hcf936e6_1.conda#39ff6e62452d8ccdbc0bdfe8566932f5
 https://conda.anaconda.org/conda-forge/win-64/xorg-libxext-1.3.4-hcd874cb_2.conda#2aa695ac3c56193fd8d526e3b511e021
 https://conda.anaconda.org/conda-forge/win-64/xorg-libxt-1.3.0-hcd874cb_0.conda#f7db1a67cd97a9bd0f59ee6997a77159
 https://conda.anaconda.org/conda-forge/noarch/flake8-black-0.3.6-pyhd8ed1ab_0.conda#61649e6e9b39ac0c7d10938025f6fe4f
-https://conda.anaconda.org/conda-forge/win-64/gst-plugins-base-1.22.3-h001b923_1.conda#bd6347f397891bf4eb264c652221507c
-https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.2.0-pyhd8ed1ab_0.conda#58ca2d50c3b27b86fd7df62eaadbf9a9
+https://conda.anaconda.org/conda-forge/win-64/gst-plugins-base-1.22.4-h001b923_0.conda#2c402e044af28ad8eccf03031c5c34c4
+https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
 https://conda.anaconda.org/conda-forge/win-64/libcblas-3.9.0-17_win64_mkl.conda#768b2c3be666ecf9e62f939ea919f819
 https://conda.anaconda.org/conda-forge/win-64/liblapack-3.9.0-17_win64_mkl.conda#278121fe8f0d65d496998aa290f36322
 https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda#f525a01528c3eba1d381a232a6971c6a
 https://conda.anaconda.org/conda-forge/win-64/pango-1.50.14-hdffb7b3_0.conda#a613f324e0f213238baec720d5c4ed00
-https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
+https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.39-hd8ed1ab_0.conda#4bbbe67d5df19db30f04b8e344dc9976
 https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.15-pyhd8ed1ab_0.conda#27db656619a55d727eaf5a6ece3d2fd6
-https://conda.anaconda.org/conda-forge/noarch/wslink-1.11.0-pyhd8ed1ab_0.conda#70f4b52c0e703936aa1812d8b14a5bb2
+https://conda.anaconda.org/conda-forge/noarch/wslink-1.11.1-pyhd8ed1ab_0.conda#0d0113b67472cea3da288838ebc80acb
 https://conda.anaconda.org/conda-forge/win-64/xorg-libxpm-3.5.16-hcd874cb_0.conda#e74445e2a4ad70fc358ae2bf87c20f41
-https://conda.anaconda.org/conda-forge/noarch/botocore-1.29.158-pyhd8ed1ab_0.conda#ccfde1c6ce8dbb4af5590c88a0482248
+https://conda.anaconda.org/conda-forge/noarch/botocore-1.29.165-pyhd8ed1ab_0.conda#0f30016ea54215fdb883b8978340c9b7
 https://conda.anaconda.org/conda-forge/noarch/ipython-8.14.0-pyh08f2357_0.conda#1fc684c1de5475383790ada5627c5430
 https://conda.anaconda.org/conda-forge/win-64/libgd-2.3.3-h891f43f_3.tar.bz2#0d66b24e1ba733a75df08e0af6f20be1
 https://conda.anaconda.org/conda-forge/win-64/liblapacke-3.9.0-17_win64_mkl.conda#6c98bb1c41479063f089459dcdedcecb
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.7.4-pyhd8ed1ab_0.conda#f7aa15f77d29b11caa1df1eb15383c59
 https://conda.anaconda.org/conda-forge/win-64/numpy-1.25.0-py310hd02465a_0.conda#63be5dd380067c6db32243e6ca56e8e8
 https://conda.anaconda.org/conda-forge/win-64/qt-main-5.15.8-h720456b_6.conda#3047b05190091b66cf60017b8968a562
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/win-64/blas-devel-3.9.0-17_win64_mkl.conda#bfcbcc96906ca944d944eb4ae340371a
 https://conda.anaconda.org/conda-forge/win-64/contourpy-1.1.0-py310h232114e_0.conda#4079a644cfc3b1fbd72571dc0a87ea33
-https://conda.anaconda.org/conda-forge/noarch/google-auth-2.20.0-pyh1a96a4e_0.conda#59f942ef9326d2519a7c953f1c24d5da
-https://conda.anaconda.org/conda-forge/win-64/graphviz-8.0.5-h51cb2cd_0.conda#ddd4c41fe063b15f4b8e0632dce89ef6
-https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.2-pyh6817e22_0.conda#e67aced0f12f38ced65e9d428dd1cff1
+https://conda.anaconda.org/conda-forge/noarch/google-auth-2.21.0-pyh1a96a4e_0.conda#8c5dd8609d314721d990c1d1fd607f81
+https://conda.anaconda.org/conda-forge/win-64/graphviz-7.0.6-h51cb2cd_0.conda#136eb298a1c96b07f935dd0525fbd11c
+https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.3-pyh6817e22_0.conda#b71d6766fc67ea676f75d121965da056
 https://conda.anaconda.org/conda-forge/noarch/jupyter-cache-0.6.1-pyhd8ed1ab_0.conda#2e360820ae68e3d28e1a5a9d2714ca5c
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.6.0-pyhd8ed1ab_0.conda#879782bde4bbdb4c7b5d4054504a20d5
 https://conda.anaconda.org/conda-forge/win-64/pandas-1.5.3-py310h1c4a608_1.conda#3e3b61b47b88cf649025e67223bee77f
 https://conda.anaconda.org/conda-forge/noarch/pooch-1.7.0-pyha770c72_3.conda#5936894aade8240c867d292aa0d980c6
 https://conda.anaconda.org/conda-forge/win-64/pyqt-5.15.7-py310h1fd54f2_3.conda#4012c5ed74c63b82c344e38cf3e68a26
 https://conda.anaconda.org/conda-forge/noarch/requests-oauthlib-1.3.1-pyhd8ed1ab_0.tar.bz2#61b279f051eef9c89d58f4d813e75e04
 https://conda.anaconda.org/conda-forge/noarch/s3transfer-0.6.1-pyhd8ed1ab_0.conda#b19a857ac845097e9c823c9f4d35f80e
 https://conda.anaconda.org/conda-forge/noarch/sphinx-4.5.0-pyh6c4a22f_0.tar.bz2#46b38d88c4270ff9ba78a89c83c66345
 https://conda.anaconda.org/conda-forge/win-64/vtk-9.2.5-qt_py310h2fd250f_200.conda#fccf10ecfe3ea51109abdd5354071823
 https://conda.anaconda.org/conda-forge/win-64/blas-2.117-mkl.conda#a6b489be6ddbc3259df7cc8a440b8950
-https://conda.anaconda.org/conda-forge/noarch/boto3-1.26.158-pyhd8ed1ab_0.conda#2e39307a3987518e49eb30ca51e3cfb5
-https://conda.anaconda.org/conda-forge/noarch/google-auth-oauthlib-1.0.0-pyhd8ed1ab_0.conda#5ba9d95acb9add67f468ecdee6595c0f
-https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.6-pyhd8ed1ab_0.conda#68627a08556e4a273e4c7bfc84251457
+https://conda.anaconda.org/conda-forge/noarch/boto3-1.26.165-pyhd8ed1ab_0.conda#b9a6316db67d5f2c8dbac2aeb24c6803
+https://conda.anaconda.org/conda-forge/noarch/google-auth-oauthlib-1.0.0-pyhd8ed1ab_1.conda#569e62e95b01b53e4ec7d9abe83b7385
+https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.7-pyhd8ed1ab_0.conda#4b0f4e8fe2a303e472674eae0340bdad
 https://conda.anaconda.org/conda-forge/noarch/jupyter_console-6.6.3-pyhd8ed1ab_0.conda#7cf6f52a66f8e3cd9d8b6c231262dcab
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.6.0-pyhd8ed1ab_0.conda#39fd52b0fcb2fb52bac47a1419bf09bd
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.7.0-pyhd8ed1ab_0.conda#7488cd1f4d35a2af96faa765b7e5b2f0
 https://conda.anaconda.org/conda-forge/win-64/matplotlib-base-3.7.1-py310h51140c5_0.conda#d8c42a72d04ad1b93ba7269e9949738e
 https://conda.anaconda.org/conda-forge/noarch/myst-parser-0.18.1-pyhd8ed1ab_0.tar.bz2#bcfdf5c7d8bf5c6f6be7b4c66fff2eca
 https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.6.0-pyhd8ed1ab_0.conda#e8172ca42f2869bb90185c9356899e81
 https://conda.anaconda.org/conda-forge/noarch/pydata-sphinx-theme-0.13.3-pyhd8ed1ab_0.conda#07aca5f2dea315dcc16680d6891e9056
 https://conda.anaconda.org/conda-forge/noarch/qtconsole-base-5.4.3-pyha770c72_0.conda#e0f5e8a6f9ea248e5c2d23efffff08f7
 https://conda.anaconda.org/conda-forge/win-64/scipy-1.10.1-py310h578b7cb_3.conda#d44c1bad75bb3e4d40066b3d3dd718ed
 https://conda.anaconda.org/conda-forge/noarch/sphinx-comments-0.0.3-pyh9f0ad1d_0.tar.bz2#2ae3ce35de0c1cec45c94182694f8d1b
@@ -408,10 +408,11 @@
 https://conda.anaconda.org/conda-forge/noarch/sphinx-book-theme-1.0.1-pyhd8ed1ab_0.conda#1ef419576de2c51b6e3a5a393eb35cda
 https://conda.anaconda.org/conda-forge/noarch/sphinx_rtd_theme-1.2.2-pyha770c72_0.conda#5ef6aaf2cfb3b656cdadb431daed6a9f
 https://conda.anaconda.org/conda-forge/noarch/tensorboard-2.13.0-pyhd8ed1ab_0.conda#321151b2405f11ec6681a9a6f30822b4
 https://conda.anaconda.org/conda-forge/noarch/jupyter-book-0.15.1-pyhd8ed1ab_0.conda#f10d556d3b3dc0aeae6aee37c412ea60
 https://conda.anaconda.org/conda-forge/noarch/nbclassic-1.0.0-pyhb4ecaf3_1.conda#a0be31e9bd84d6eae87cdbf74c56b90b
 https://conda.anaconda.org/conda-forge/noarch/torchinfo-1.8.0-pyhd8ed1ab_0.conda#fba98fc95a945e2a6b93a77b39dd52dc
 https://conda.anaconda.org/conda-forge/noarch/torchmetrics-0.11.4-pyhd8ed1ab_0.conda#480cb2b6d502003e937d9e4326bc398f
+https://conda.anaconda.org/pytorch/win-64/torchvision-0.15.2-py310_cu118.tar.bz2#140ec95434b375beaa3b12159b9f0caf
 https://conda.anaconda.org/conda-forge/noarch/notebook-6.5.4-pyha770c72_0.conda#ec4ce3ce0a55ce21b6f5b86049b97af9
-https://conda.anaconda.org/conda-forge/noarch/pytorch-lightning-2.0.3-pyhd8ed1ab_0.conda#97138eb8783fa54884216a6562413736
+https://conda.anaconda.org/conda-forge/noarch/pytorch-lightning-2.0.4-pyhd8ed1ab_0.conda#ce9d626b181c6f8cceb5047f6a819f7d
 https://conda.anaconda.org/conda-forge/win-64/jupyter-1.0.0-py310h5588dad_8.conda#5fe66001841554f8b30f7db775d9ba81
```

### Comparing `hf-deepali-0.3.1/docker/build` & `hf-deepali-0.3.2/docker/build`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,58 @@
 #!/bin/bash
 
 DOCKER_DIR="$(dirname "$BASH_SOURCE")"
 PROJECT_DIR="$(cd "$DOCKER_DIR/.." && pwd)"
 
 tag=
 base_image=
-conda_yaml=
+conda_version=
 python_version=
+version=
 
 user_name=$(id -u -n)
 user_id=$(id -u)
 group_name=$(id -g -n)
 group_id=$(id -g)
 
 while [ $# -gt 0 ]; do
   case "$1" in
     -t|--tag) tag="$2"; shift; ;;
     -b|--base|--base-image|--from) base_image="$2"; shift; ;;
-    -e|--env|--conda-yaml) conda_yaml="$2"; shift; ;;
     --user) user_name="$2"; shift; ;;
     --uid) user_id="$2"; shift; ;;
     --group) group_name="$2"; shift; ;;
     --gid) group_id="$2"; shift; ;;
+    --version) version="$2"; shift; ;;
     --python|--python-version) python_version="$2"; shift; ;;
+    --conda|--conda-version) conda_version="$2"; shift; ;;
     *) error "invalid argument $1"
   esac
   shift
 done
 
 [ -n "$tag" ] || tag="deepali:$USER"
-[ -n "$base_image" ] || base_image="pytorch/pytorch:1.9.0-cuda11.1-cudnn8-runtime"
-[ -n "$conda_yaml" ] || conda_yaml="conda.yaml"
-[ -n "$python_version" ] || python_version="3.7.10"
+[ -n "$base_image" ] || base_image="ubuntu:22.04"
+[ -n "$conda_version" ] || conda_version="22.9.0-3"
+[ -n "$python_version" ] || python_version="3.10.8"
+
+if [ -z "$version" ]; then
+  version=$(cd "$PROJECT_DIR" && python -m setuptools_scm)
+  if [ $? -ne 0 ]; then
+    echo "setuptools_scm must be installed in Python environment used to build this Docker image. Alternatively, use --version to specify a deepali version string." 1>&2
+    exit 1
+  fi
+fi
+
+export DOCKER_BUILDKIT=${DOCKER_BUILDKIT:-1}
 
 exec docker build "$PROJECT_DIR" \
   --file "$DOCKER_DIR/Dockerfile" \
   --tag "$tag" \
   --build-arg "BASE_IMAGE=$base_image" \
-  --build-arg "CONDA_YAML=$conda_yaml" \
+  --build-arg "CONDA_VERSION=$conda_version" \
   --build-arg "PYTHON_VERSION=$python_version" \
+  --build-arg "VERSION=$version" \
   --build-arg "USER=$user_name" \
   --build-arg "GROUP=$group_name" \
   --build-arg "UID=$user_id" \
   --build-arg "GID=$group_id" \
```

### Comparing `hf-deepali-0.3.1/docker/run` & `hf-deepali-0.3.2/docker/run`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/docs/_citations.bib` & `hf-deepali-0.3.2/docs/_citations.bib`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/docs/_config.yml` & `hf-deepali-0.3.2/docs/_config.yml`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,18 @@
 
 # Add GitHub buttons to your book
 # See https://jupyterbook.org/customize/config.html#add-a-link-to-your-repository
 html:
   use_issues_button: true
   use_repository_button: true
 
+# Add a Launch on Google Colab button
+launch_buttons:
+  colab_url: "https://colab.research.google.com"
+
 # By default MathJax version 2 is currently used. If you are using a lot of math,
 # you may want to try using version 3, which claims to improve load speeds by 60 - 80%.
 sphinx:
   config:
     add_module_names: false
     autoapi_dirs:
     - ../src/deepali
```

### Comparing `hf-deepali-0.3.1/docs/_images/logo.png` & `hf-deepali-0.3.2/docs/_images/logo.png`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/docs/_toc.yml` & `hf-deepali-0.3.2/docs/_toc.yml`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 parts:
 - caption: Basics
   chapters:
   - file: basics/installation
   - file: basics/example-page
 - caption: Tutorials
   chapters:
-  - file: tutorials/example-notebook
-  - file: tutorials/example-myst-notebook
+  - file: tutorials/pairwise-registration-intro
 - caption: Reference
   chapters:
   - file: reference/core/index
     sections:
     - file: reference/core/domain
     - file: reference/core/kernels
     - file: reference/core/image
@@ -41,7 +40,11 @@
   - file: reference/api/deepali/core/index
   - file: reference/api/deepali/data/index
   - file: reference/api/deepali/losses/index
   - file: reference/api/deepali/modules/index
   - file: reference/api/deepali/networks/index
   - file: reference/api/deepali/spatial/index
   - file: reference/api/deepali/utils/index
+- caption: Contributing
+  chapters:
+  - file: tutorials/example-notebook
+  - file: tutorials/example-myst-notebook
```

### Comparing `hf-deepali-0.3.1/docs/basics/example-page.md` & `hf-deepali-0.3.2/docs/basics/example-page.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/docs/basics/installation.md` & `hf-deepali-0.3.2/docs/basics/installation.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/docs/index.md` & `hf-deepali-0.3.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/docs/reference/core/flow.md` & `hf-deepali-0.3.2/docs/reference/core/flow.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/docs/reference/core/image.md` & `hf-deepali-0.3.2/docs/reference/core/image.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/docs/reference/data/transforms.md` & `hf-deepali-0.3.2/docs/reference/data/transforms.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/docs/reference/spatial/common.md` & `hf-deepali-0.3.2/docs/reference/spatial/common.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/docs/reference/spatial/composite.md` & `hf-deepali-0.3.2/docs/reference/spatial/composite.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/docs/reference/utils/index.md` & `hf-deepali-0.3.2/docs/reference/utils/index.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/docs/tutorials/example-myst-notebook.md` & `hf-deepali-0.3.2/docs/tutorials/example-myst-notebook.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/docs/tutorials/example-notebook.ipynb` & `hf-deepali-0.3.2/docs/tutorials/example-notebook.ipynb`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/examples/ffd/README.md` & `hf-deepali-0.3.2/examples/ffd/README.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/examples/ffd/engine.py` & `hf-deepali-0.3.2/examples/ffd/engine.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/examples/ffd/hooks.py` & `hf-deepali-0.3.2/examples/ffd/hooks.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/examples/ffd/losses.py` & `hf-deepali-0.3.2/examples/ffd/losses.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/examples/ffd/optim.py` & `hf-deepali-0.3.2/examples/ffd/optim.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/examples/ffd/pairwise.py` & `hf-deepali-0.3.2/examples/ffd/pairwise.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/examples/ffd/params.yaml` & `hf-deepali-0.3.2/examples/ffd/params.yaml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/examples/ffd/register.py` & `hf-deepali-0.3.2/examples/ffd/register.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/examples/istn/models/__init__.py` & `hf-deepali-0.3.2/examples/istn/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/examples/istn/models/itn.py` & `hf-deepali-0.3.2/examples/istn/models/itn.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/examples/istn/models/stn.py` & `hf-deepali-0.3.2/examples/istn/models/stn.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/examples/istn/params.yaml` & `hf-deepali-0.3.2/examples/istn/params.yaml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/examples/istn/train.py` & `hf-deepali-0.3.2/examples/istn/train.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/pyproject.toml` & `hf-deepali-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/core/__init__.py` & `hf-deepali-0.3.2/src/deepali/core/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/core/_kornia.py` & `hf-deepali-0.3.2/src/deepali/core/_kornia.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/core/affine.py` & `hf-deepali-0.3.2/src/deepali/core/affine.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/core/bspline.py` & `hf-deepali-0.3.2/src/deepali/core/bspline.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/core/config.py` & `hf-deepali-0.3.2/src/deepali/core/config.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/core/cube.py` & `hf-deepali-0.3.2/src/deepali/core/cube.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/core/enum.py` & `hf-deepali-0.3.2/src/deepali/core/enum.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/core/flow.py` & `hf-deepali-0.3.2/src/deepali/core/flow.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/core/functional.py` & `hf-deepali-0.3.2/src/deepali/core/functional.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/core/grid.py` & `hf-deepali-0.3.2/src/deepali/core/grid.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/core/image.py` & `hf-deepali-0.3.2/src/deepali/core/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -1777,14 +1777,17 @@
     Returns:
         Image tensor of shape ``(N, 1, Y, X)``.
 
     """
     size = _image_size("cshape_image", size, shape, ndim=2)
     if dtype is None:
         dtype = torch.uint8
+    if radius is None:
+        center = tuple(float(x) for x in center)
+        radius = max(0, (min(center) - 1) - math.ceil(2 * sigma))
     if width is None:
         width = radius // 2
     outer = circle_image(size, center=center, radius=radius, x_max=x_max, sigma=0)
     inner = circle_image(size, center=center, radius=radius - width, sigma=0)
     image = (outer - inner).type(torch.float32)
     if sigma > 0:
         kernel = gaussian1d(sigma, dtype=torch.float32, device=image.device)
```

### Comparing `hf-deepali-0.3.1/src/deepali/core/itertools.py` & `hf-deepali-0.3.2/src/deepali/core/itertools.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/core/kernels.py` & `hf-deepali-0.3.2/src/deepali/core/kernels.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/core/linalg.py` & `hf-deepali-0.3.2/src/deepali/core/linalg.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/core/math.py` & `hf-deepali-0.3.2/src/deepali/core/math.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/core/nnutils.py` & `hf-deepali-0.3.2/src/deepali/core/nnutils.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/core/path.py` & `hf-deepali-0.3.2/src/deepali/core/path.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/core/pointset.py` & `hf-deepali-0.3.2/src/deepali/core/pointset.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/core/random.py` & `hf-deepali-0.3.2/src/deepali/core/random.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/core/tensor.py` & `hf-deepali-0.3.2/src/deepali/core/tensor.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/core/types.py` & `hf-deepali-0.3.2/src/deepali/core/types.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/data/__init__.py` & `hf-deepali-0.3.2/src/deepali/data/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/data/collate.py` & `hf-deepali-0.3.2/src/deepali/data/collate.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/data/dataset.py` & `hf-deepali-0.3.2/src/deepali/data/dataset.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/data/flow.py` & `hf-deepali-0.3.2/src/deepali/data/flow.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,22 +84,26 @@
 
     def _make_instance(
         self: TFlowFields,
         data: Tensor,
         grid: Optional[Sequence[Grid]] = None,
         axes: Optional[Axes] = None,
         **kwargs,
-    ) -> TFlowFields:
+    ) -> Union[TFlowFields, ImageBatch]:
         r"""Create a new instance while preserving subclass meta-data."""
+        if data.shape[1] != data.ndim - 2:
+            return ImageBatch(data, grid)
         kwargs["axes"] = axes or self._axes
         return super()._make_instance(data, grid, **kwargs)
 
-    def _make_flowfield(self, data: Tensor, grid: Grid, axes: Axes) -> FlowField:
+    def _make_subitem(self, data: Tensor, grid: Grid) -> Union[FlowField, Image]:
         r"""Create FlowField in __getitem__. Can be overridden by subclasses to return a subtype."""
-        return FlowField(data, grid, axes)
+        if data.shape[0] == data.ndim - 1:
+            return FlowField(data, grid, self._axes)
+        return super()._make_subitem(data, grid)
 
     @staticmethod
     def _torch_function_axes(args) -> Optional[Axes]:
         r"""Get flow field Axes from args passed to __torch_function__."""
         if not args:
             return None
         if isinstance(args[0], (tuple, list)):
@@ -157,62 +161,27 @@
         return cls._torch_function_result(func, data, grid, axes)
 
     @overload
     def __getitem__(self: TFlowFields, index: int) -> FlowField:
         ...
 
     @overload
-    def __getitem__(self: TFlowFields, index: Union[EllipsisType, slice]) -> TFlowFields:
+    def __getitem__(self: TFlowFields, index: EllipsisType) -> TFlowFields:
+        ...
+
+    @overload
+    def __getitem__(self: TFlowFields, index: Union[list, slice, Tensor]) -> TFlowFields:
         ...
 
     def __getitem__(
         self: TFlowFields,
         index: Union[EllipsisType, int, slice, Sequence[Union[EllipsisType, int, slice]]],
-    ) -> Union[FlowField, TFlowFields, Tensor]:
+    ) -> Union[FlowField, Image, TFlowFields, ImageBatch, Tensor]:
         r"""Get flow field at specified batch index, get a sub-batch, or extract region of interest tensor."""
-        if index is ...:
-            return self._make_instance(self.tensor(), self._grid, self._axes)
-        if isinstance(index, Sequence):
-            # Resolve additional ellipses
-            index = [j for i, j in enumerate(index) if j is not ... or ... not in index[:i]]
-            # Discard trailing ellipsis
-            if index[-1] is ...:
-                index = index[:-1]
-            # Substitute remaining ellipsis with full slices
-            try:
-                i = index.index(...)
-                j = len(index) - i - 1
-                index = index[:i] + [slice(None)] * (self.ndim - i - j) + index[-j:]
-            except ValueError:
-                pass
-            # Channel dimension is always a slice
-            if len(index) > 1 and isinstance(index[1], int):
-                index[1] = slice(index[1], index[1] + 1)
-            index = tuple(index)
-        data = self.tensor()[index]
-        grid_index = index[0] if isinstance(index, Sequence) else index
-        grid = self._grid[grid_index]
-        if isinstance(index, Sequence) and len(index) > 2:
-            same_grid = True
-            for i, n in zip(index[2:], self.shape[2:]):
-                if isinstance(i, int) or not isinstance(i, slice):
-                    same_grid = False
-                    break
-                if i.start not in (None, 0) or i.stop not in (None, n) or i.step not in (None, 1):
-                    same_grid = False
-                    break
-            if not same_grid:
-                return data
-        if isinstance(grid, Grid):
-            if data.ndim < 3:
-                return data
-            return self._make_flowfield(data, grid, self._axes)
-        elif data.ndim < 4:
-            return data
-        return self._make_instance(data, grid, self._axes)
+        return super().__getitem__(index)
 
     @overload
     def axes(self: TFlowFields) -> Axes:
         r"""Get axes with respect to which flow vectors are defined."""
         ...
 
     @overload
```

### Comparing `hf-deepali-0.3.1/src/deepali/data/image.py` & `hf-deepali-0.3.2/src/deepali/data/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 r"""Image tensors."""
 
 from __future__ import annotations
 
 from typing import Any, Dict, Optional, Sequence, Tuple, Type, TypeVar, Union, overload
 
+import numpy as np
 import torch
 from torch import Tensor
 from torch.nn import functional as F
 
 try:
     import SimpleITK as sitk
     from ..utils.sitk.torch import image_from_tensor, tensor_from_image
@@ -80,15 +81,15 @@
         grid: Optional[Sequence[Grid]] = None,
         **kwargs,
     ) -> TImageBatch:
         r"""Create a new instance while preserving subclass (meta-)data."""
         kwargs["grid"] = self._grid if grid is None else grid
         return super()._make_instance(data, **kwargs)
 
-    def _make_image(self, data: Tensor, grid: Grid) -> Image:
+    def _make_subitem(self, data: Tensor, grid: Grid) -> Image:
         r"""Create Image in __getitem__. Can be overridden by subclasses to return a subtype."""
         return Image(data, grid)
 
     def __deepcopy__(self: TImageBatch, memo) -> TImageBatch:
         if id(self) in memo:
             return memo[id(self)]
         result = self._make_instance(
@@ -294,59 +295,75 @@
         return self.shape[0]
 
     @overload
     def __getitem__(self: TImageBatch, index: int) -> Image:
         ...
 
     @overload
-    def __getitem__(self: TImageBatch, index: Union[EllipsisType, slice]) -> TImageBatch:
+    def __getitem__(self: TImageBatch, index: EllipsisType) -> TImageBatch:
+        ...
+
+    @overload
+    def __getitem__(self: TImageBatch, index: Union[list, slice, Tensor]) -> TImageBatch:
         ...
 
     def __getitem__(
         self: TImageBatch,
         index: Union[EllipsisType, int, slice, Sequence[Union[EllipsisType, int, slice]]],
     ) -> Union[Image, TImageBatch, Tensor]:
         r"""Get image at specified batch index, get a sub-batch, or a region of interest tensor."""
         if index is ...:
             return self._make_instance(self.tensor(), self.grid())
-        if isinstance(index, Sequence):
+        if type(index) is tuple:
             # Resolve additional ellipses
             index = [j for i, j in enumerate(index) if j is not ... or ... not in index[:i]]
             # Discard trailing ellipsis
             if index[-1] is ...:
                 index = index[:-1]
             # Substitute remaining ellipsis with full slices
             try:
                 i = index.index(...)
                 j = len(index) - i - 1
                 index = index[:i] + [slice(None)] * (self.ndim - i - j) + index[-j:]
             except ValueError:
                 pass
-            # Channel dimension is always a slice
-            if len(index) > 1 and isinstance(index[1], int):
-                index[1] = slice(index[1], index[1] + 1)
             index = tuple(index)
+            is_multi_index = True
+        elif isinstance(index, (np.ndarray, slice, Sequence, Tensor)):
+            # - batch[[0, 2, 4]]
+            # - batch[np.array([0, 2, 4])]
+            # - batch[torch.tensor([0, 2, 4])]
+            index = (index,)
+            is_multi_index = True
+        else:
+            index = int(index)
+            is_multi_index = False
         data = self.tensor()[index]
-        grid_index = index[0] if isinstance(index, Sequence) else index
-        grid = self._grid[grid_index]
-        if isinstance(index, Sequence) and len(index) > 2:
+        if is_multi_index and len(index) > 1 and isinstance(index[1], int):
+            return data  # cannot be an ImageBatch or Image without a channel dimension
+        grid_index = index[0] if is_multi_index else index
+        if isinstance(grid_index, (np.ndarray, Sequence, Tensor)):
+            grid = tuple(self._grid[i] for i in grid_index)
+        else:
+            grid = self._grid[grid_index]
+        if is_multi_index and len(index) > 2:
             same_grid = True
             for i, n in zip(index[2:], self.shape[2:]):
                 if isinstance(i, int) or not isinstance(i, slice):
                     same_grid = False
                     break
                 if i.start not in (None, 0) or i.stop not in (None, n) or i.step not in (None, 1):
                     same_grid = False
                     break
             if not same_grid:
                 return data
         if isinstance(grid, Grid):
             if data.ndim < 3:
                 return data
-            return self._make_image(data, grid)
+            return self._make_subitem(data, grid)
         elif data.ndim < 4:
             return data
         return self._make_instance(data, grid)
 
     @property
     def sdim(self: TImageBatch) -> int:
         r"""Number of spatial dimensions."""
```

### Comparing `hf-deepali-0.3.1/src/deepali/data/partition.py` & `hf-deepali-0.3.2/src/deepali/data/partition.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/data/prepare.py` & `hf-deepali-0.3.2/src/deepali/data/prepare.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/data/sample.py` & `hf-deepali-0.3.2/src/deepali/data/sample.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/data/sampler.py` & `hf-deepali-0.3.2/src/deepali/data/sampler.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/data/tensor.py` & `hf-deepali-0.3.2/src/deepali/data/tensor.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/data/transforms/__init__.py` & `hf-deepali-0.3.2/src/deepali/data/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/data/transforms/image.py` & `hf-deepali-0.3.2/src/deepali/data/transforms/image.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/data/transforms/item.py` & `hf-deepali-0.3.2/src/deepali/data/transforms/item.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/losses/__init__.py` & `hf-deepali-0.3.2/src/deepali/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/losses/base.py` & `hf-deepali-0.3.2/src/deepali/losses/base.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/losses/flow.py` & `hf-deepali-0.3.2/src/deepali/losses/flow.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/losses/functional.py` & `hf-deepali-0.3.2/src/deepali/losses/functional.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/losses/image.py` & `hf-deepali-0.3.2/src/deepali/losses/image.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/losses/params.py` & `hf-deepali-0.3.2/src/deepali/losses/params.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/losses/pointset.py` & `hf-deepali-0.3.2/src/deepali/losses/pointset.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/modules/__init__.py` & `hf-deepali-0.3.2/src/deepali/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/modules/basic.py` & `hf-deepali-0.3.2/src/deepali/modules/basic.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/modules/flow.py` & `hf-deepali-0.3.2/src/deepali/modules/flow.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/modules/image.py` & `hf-deepali-0.3.2/src/deepali/modules/image.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/modules/lambd.py` & `hf-deepali-0.3.2/src/deepali/modules/lambd.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/modules/mixins.py` & `hf-deepali-0.3.2/src/deepali/modules/mixins.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/modules/output.py` & `hf-deepali-0.3.2/src/deepali/modules/output.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/modules/sample.py` & `hf-deepali-0.3.2/src/deepali/modules/sample.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/modules/utilities.py` & `hf-deepali-0.3.2/src/deepali/modules/utilities.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/networks/__init__.py` & `hf-deepali-0.3.2/src/deepali/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/networks/blocks/residual.py` & `hf-deepali-0.3.2/src/deepali/networks/blocks/residual.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/networks/blocks/skip.py` & `hf-deepali-0.3.2/src/deepali/networks/blocks/skip.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/networks/layers/__init__.py` & `hf-deepali-0.3.2/src/deepali/networks/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/networks/layers/acti.py` & `hf-deepali-0.3.2/src/deepali/networks/layers/acti.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/networks/layers/conv.py` & `hf-deepali-0.3.2/src/deepali/networks/layers/conv.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/networks/layers/join.py` & `hf-deepali-0.3.2/src/deepali/networks/layers/join.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/networks/layers/linear.py` & `hf-deepali-0.3.2/src/deepali/networks/layers/linear.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/networks/layers/norm.py` & `hf-deepali-0.3.2/src/deepali/networks/layers/norm.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/networks/layers/pool.py` & `hf-deepali-0.3.2/src/deepali/networks/layers/pool.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/networks/layers/upsample.py` & `hf-deepali-0.3.2/src/deepali/networks/layers/upsample.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/networks/resnet.py` & `hf-deepali-0.3.2/src/deepali/networks/resnet.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/networks/unet.py` & `hf-deepali-0.3.2/src/deepali/networks/unet.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/networks/utils.py` & `hf-deepali-0.3.2/src/deepali/networks/utils.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/spatial/__init__.py` & `hf-deepali-0.3.2/src/deepali/spatial/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/spatial/base.py` & `hf-deepali-0.3.2/src/deepali/spatial/base.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/spatial/bspline.py` & `hf-deepali-0.3.2/src/deepali/spatial/bspline.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/spatial/composite.py` & `hf-deepali-0.3.2/src/deepali/spatial/composite.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/spatial/generic.py` & `hf-deepali-0.3.2/src/deepali/spatial/generic.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/spatial/linear.py` & `hf-deepali-0.3.2/src/deepali/spatial/linear.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/spatial/nonrigid.py` & `hf-deepali-0.3.2/src/deepali/spatial/nonrigid.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/spatial/parametric.py` & `hf-deepali-0.3.2/src/deepali/spatial/parametric.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/spatial/transformer.py` & `hf-deepali-0.3.2/src/deepali/spatial/transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,22 +145,24 @@
             raise TypeError(f"{type(self).__name__}() 'target' must be of type Grid")
         if not isinstance(source, Grid):
             raise TypeError(f"{type(self).__name__}() 'source' must be of type Grid")
         if not transform.grid().same_domain_as(target):
             raise ValueError(
                 f"{type(self).__name__}() 'target' and 'transform' grid must define the same domain"
             )
-        self._sample = SampleImage(
+        device = transform.device
+        sampler = SampleImage(
             target=target,
             source=source,
             sampling=sampling,
             padding=padding,
             align_centers=align_centers,
         )
-        grid_coords = target.coords(flip=flip_coords).unsqueeze(0)
+        self._sample = sampler.to(device)
+        grid_coords = target.coords(flip=flip_coords, device=device).unsqueeze(0)
         self.register_buffer("grid_coords", grid_coords, persistent=False)
         self.flip_coords = bool(flip_coords)
 
     @property
     def sample(self) -> SampleImage:
         r"""Source image sampler."""
         return self._sample
```

### Comparing `hf-deepali-0.3.1/src/deepali/utils/aws/resource.py` & `hf-deepali-0.3.2/src/deepali/utils/aws/resource.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,60 +3,27 @@
 from __future__ import annotations
 
 from copy import deepcopy
 import os
 from pathlib import Path
 import re
 import shutil
-from typing import Generator, Optional, TypeVar, Union
+from typing import Any, Generator, Optional, TypeVar, Union
 from urllib.parse import urlsplit
 
 PathStr = Union[Path, str]
+PathUri = Union[Path, str]
 
 
 # See https://mypy.readthedocs.io/en/latest/generics.html#generic-methods-and-generic-self for the use
 # of `T` to annotate `self`. Many methods of `Resource` return `self` and we want those return values
 # to be the type of the subclass, not the looser type of `Resource`.
 T = TypeVar("T", bound="Resource")
 
 
-def to_uri(arg: PathStr) -> str:
-    r"""Create valid URI from resource path.
-
-    Args:
-        arg: Local path or a valid URI.
-
-    Returns:
-        Valid URI.
-
-    """
-    # Path
-    if isinstance(arg, Path):
-        return arg.absolute().as_uri()
-    # Windows path with drive letter
-    if os.name == "nt":
-        match = re.match(r"([a-zA-Z]):[/\\](.*)", arg)
-        if match:
-            return Path(match.group(1) + ":/" + match.group(2)).as_uri()
-    # URI with scheme prefix
-    match = re.match(r"([a-zA-Z0-9]+)://(.*)", arg)
-    if match:
-        scheme = match.group(1).lower()
-        # Local file URI
-        if scheme == "file":
-            return Path("/" + match.group(2)).absolute().as_uri()
-        # AWS S3 object URI
-        if scheme == "s3":
-            return "s3://" + re.sub("^/+", "", re.sub(r"[/\\]{1,}", "/", match.group(2)))
-        # Other URI
-        return urlsplit(arg, scheme="file").geturl()
-    # Unix path or relative path
-    return Path(arg).absolute().as_uri()
-
-
 class Resource(object):
     r"""Interface for storage objects.
 
     This base class can be used for storage objects that are only stored locally.
     The base implementations of the ``Resource`` interface functions reflect this use
     case, where ``Resource("/path/to/file")`` represents such local path object.
     The factory function ``Resource.from_uri`` is recommended for creating concrete
@@ -141,14 +108,28 @@
     def __exit__(self: T, *exc) -> None:
         r"""Release resource when leaving outermost context."""
         self._depth = max(0, self._depth - 1)
         if self._depth == 0:
             self.release()
 
     @staticmethod
+    def from_path(*args: Optional[PathStr]) -> Resource:
+        r"""Create storage object from path or URI.
+
+        Args:
+            args: Path or URI components. The last absolute path or URI is the base to which
+                subsequent arguments are appended. Any ``None`` value is ignored. See also ``to_uri()``.
+
+        Returns:
+            obj (Resource): Instance of concrete type representing the referenced storage object.
+
+        """
+        return Resource.from_uri(to_uri(args))
+
+    @staticmethod
     def from_uri(uri: str) -> Resource:
         r"""Create storage object from URI.
 
         Args:
             uri: URI of storage object.
 
         Returns:
@@ -363,7 +344,106 @@
     def __str__(self: T) -> str:
         r"""Get human-readable string representation of storage object reference."""
         return self.uri
 
     def __repr__(self: T) -> str:
         r"""Get human-readable string representation of storage object reference."""
         return type(self).__name__ + "(path='{}')".format(self.path)
+
+
+def is_absolute(path: Union[Path, str]) -> bool:
+    r"""Check whether given path string or URI is absolute."""
+    if is_uri(path):
+        return True
+    return Path(path).is_absolute()
+
+
+def is_uri(arg: Any) -> bool:
+    r"""Check whether a given argument is a URI."""
+    if isinstance(arg, Path):
+        return False
+    if isinstance(arg, str):
+        # Windows path with drive letter
+        if os.name == "nt" and re.match(r"([a-zA-Z]):[/\\](.*)", arg):
+            return False
+        return re.match(r"([a-zA-Z0-9]+)://(.*)", arg) is not None
+    return False
+
+
+def to_uri(*args: Optional[PathStr]) -> str:
+    r"""Create valid URI from resource paths.
+
+    Args:
+        args: Local path components or an already valid URI. The last absolute path or URI in this
+            list of arguments is the base path or URI prefix for subsequent relative paths which
+            are appended to this base to construct the URI. Any ``None`` values are ignored.
+
+    Returns:
+        Valid URI.
+
+    """
+    args = [arg for arg in args if arg is not None]
+    for i, arg in enumerate(reversed(args)):
+        if is_uri(arg):
+            base = str(arg)
+            args = args[len(args) - i :]
+            break
+        elif Path(arg).is_absolute():
+            base = Path(arg)
+            args = args[len(args) - i :]
+            break
+    else:
+        base = Path.cwd()
+    if isinstance(base, Path):
+        uri = local_path_uri(base.joinpath(*args))
+    else:
+        uri = norm_uri(f"{base}/{'/'.join(args)}" if args else base)
+    return uri
+
+
+def norm_uri(uri: str) -> str:
+    r"""Normalize URI.
+
+    Args:
+        uri: A valid URI string.
+
+    Returns:
+        Normalized URI string.
+
+    """
+    match = re.match(r"(?P<scheme>[a-zA-Z0-9]+)://(?P<path>.*)", uri)
+    if not match:
+        raise ValueError(f"norm_uri() 'uri' is not a valid URI: {uri}")
+    scheme = match["scheme"].lower()
+    path = re.sub("^/+", "", re.sub(r"[/\\]{1,}", "/", match["path"]))
+    # Local file URI
+    if scheme == "file":
+        if os.name != "nt" or re.match(r"(?P<drive>[a-zA-Z]):[/\\]", path) is None:
+            path = "/" + path
+        return "file://" + path
+    # AWS S3 object URI
+    if scheme == "s3":
+        return "s3://" + path
+    # Other URI
+    return urlsplit(uri, scheme="file").geturl()
+
+
+def local_path_uri(arg: PathStr) -> str:
+    r"""Create valid URI from local path.
+
+    Unlike Path.as_uri(), this function does not escape special characters as used in format template strings.
+
+    Args:
+        arg: Local path.
+
+    Returns:
+        Valid URI.
+
+    """
+    uri = norm_uri(f"file://{Path(arg).absolute()}")
+    if uri.endswith("/"):
+        # Trailing forward slashes are removed by Path already, but trailing backward slashes are
+        # only converted to a single forward slash by norm_uri(), not removed by Path. To produce
+        # a consistent result regardless of whether forward or backward slashes are used, remove
+        # any remaining trailing slash even if it could signify a directory.
+        uri = uri[:-1]
+    return uri
```

### Comparing `hf-deepali-0.3.1/src/deepali/utils/aws/s3/client.py` & `hf-deepali-0.3.2/src/deepali/utils/aws/s3/client.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/utils/aws/s3/object.py` & `hf-deepali-0.3.2/src/deepali/utils/aws/s3/object.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/utils/cli/__init__.py` & `hf-deepali-0.3.2/src/deepali/utils/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/utils/cli/argparse.py` & `hf-deepali-0.3.2/src/deepali/utils/cli/argparse.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/utils/cli/environ.py` & `hf-deepali-0.3.2/src/deepali/utils/cli/environ.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/utils/cli/logging.py` & `hf-deepali-0.3.2/src/deepali/utils/cli/logging.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/utils/ignite/handlers.py` & `hf-deepali-0.3.2/src/deepali/utils/ignite/handlers.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/utils/ignite/metrics/average_loss.py` & `hf-deepali-0.3.2/src/deepali/utils/ignite/metrics/average_loss.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/utils/ignite/metrics/binary_classification.py` & `hf-deepali-0.3.2/src/deepali/utils/ignite/metrics/binary_classification.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/utils/ignite/metrics/multilabel_classification.py` & `hf-deepali-0.3.2/src/deepali/utils/ignite/metrics/multilabel_classification.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/utils/ignite/output_transforms.py` & `hf-deepali-0.3.2/src/deepali/utils/ignite/output_transforms.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/utils/ignite/score_functions.py` & `hf-deepali-0.3.2/src/deepali/utils/ignite/score_functions.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/utils/sitk/grid.py` & `hf-deepali-0.3.2/src/deepali/utils/sitk/grid.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/utils/sitk/imageio.py` & `hf-deepali-0.3.2/src/deepali/utils/sitk/imageio.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/utils/sitk/numpy.py` & `hf-deepali-0.3.2/src/deepali/utils/sitk/numpy.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/utils/sitk/sample.py` & `hf-deepali-0.3.2/src/deepali/utils/sitk/sample.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/utils/sitk/torch.py` & `hf-deepali-0.3.2/src/deepali/utils/sitk/torch.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/utils/tensorboard.py` & `hf-deepali-0.3.2/src/deepali/utils/tensorboard.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/utils/vtk/idlist.py` & `hf-deepali-0.3.2/src/deepali/utils/vtk/idlist.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/utils/vtk/image.py` & `hf-deepali-0.3.2/src/deepali/utils/vtk/image.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/utils/vtk/numpy.py` & `hf-deepali-0.3.2/src/deepali/utils/vtk/numpy.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/utils/vtk/polydataio.py` & `hf-deepali-0.3.2/src/deepali/utils/vtk/polydataio.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/deepali/utils/vtk/simpleitk.py` & `hf-deepali-0.3.2/src/deepali/utils/vtk/simpleitk.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/src/hf_deepali.egg-info/PKG-INFO` & `hf-deepali-0.3.2/src/hf_deepali.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hf-deepali
-Version: 0.3.1
+Version: 0.3.2
 Summary: Image, point set, and surface registration library for PyTorch.
 Maintainer-email: Andreas Schuh <andreas.schuh@imperial.ac.uk>
 License: Apache-2.0
 Project-URL: Homepage, https://biomedia.github.io/deepali
 Project-URL: Repository, https://github.com/BioMedIA/deepali.git
 Project-URL: Bug Tracker, https://github.com/BioMedIA/deepali/issues
 Keywords: medical-imaging,image-registration,spatial-transformer-networks
@@ -23,16 +23,16 @@
 Provides-Extra: all
 Provides-Extra: utils
 Provides-Extra: tests
 License-File: LICENSE
 
 # deepali
 
-![pypi](https://img.shields.io/pypi/v/hf-deepali)
 <!-- ![downloads](https://img.shields.io/pypi/dm/hf-deepali) -->
+![pypi](https://img.shields.io/pypi/v/hf-deepali)
 ![python](https://img.shields.io/pypi/pyversions/hf-deepali)
 [![docs](https://github.com/BioMedIA/deepali/actions/workflows/docs.yml/badge.svg)](https://github.com/BioMedIA/deepali/actions/workflows/docs.yml)
 [![tests](https://github.com/BioMedIA/deepali/actions/workflows/tests.yml/badge.svg)](https://github.com/BioMedIA/deepali/actions/workflows/tests.yml)
 [![release](https://github.com/BioMedIA/deepali/actions/workflows/release.yml/badge.svg)](https://github.com/BioMedIA/deepali/actions/workflows/release.yml)
 
 An [open source](https://github.com/BioMedIA/deepali/tree/main/LICENSE) research library for image, point set, and surface registration in [PyTorch], which is developed and maintained by the [HeartFlow-Imperial College London] research lab at the [Biomedical Image Analysis Group].
 
@@ -73,15 +73,15 @@
 - [PyTorch]: The automatic differentiation and deep learning framework powering this project.
 - [SimpleITK] (optional): Used by [deepali.data] to read and write images in file formats supported by ITK.
 - [NumPy] (optional): Used by [deepali.utils]. Other components use pure PyTorch.
 - [VTK] (optional): May be used to read and write point sets and surface meshes.
 
 ## Installation
 
-This Python package can be installed with [pip]:
+This library is available as [Python package on PyPI](https://pypi.org/project/hf-deepali/) and can be installed with [pip]:
 
 ```
 pip install hf-deepali
 ```
 
 The latest development version can be installed directly from the GitHub repository, i.e.,
```

### Comparing `hf-deepali-0.3.1/src/hf_deepali.egg-info/SOURCES.txt` & `hf-deepali-0.3.2/src/hf_deepali.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,19 @@
 .vscode/launch.json
 .vscode/settings.json
 conda/Makefile
 conda/README.md
 conda/environment.conda-lock.yml
 conda/environment.devenv.yml
 conda/environment.linux-64.lock
+conda/environment.linux-64.yml
 conda/environment.osx-64.lock
+conda/environment.osx-64.yml
 conda/environment.win-64.lock
+conda/environment.win-64.yml
 docker/Dockerfile
 docker/build
 docker/run
 docs/_citations.bib
 docs/_config.yml
 docs/_toc.yml
 docs/index.md
@@ -45,16 +48,18 @@
 docs/reference/modules/index.md
 docs/reference/networks/index.md
 docs/reference/spatial/common.md
 docs/reference/spatial/composite.md
 docs/reference/spatial/index.md
 docs/reference/spatial/transformer.md
 docs/reference/utils/index.md
+docs/tutorials/.gitignore
 docs/tutorials/example-myst-notebook.md
 docs/tutorials/example-notebook.ipynb
+docs/tutorials/pairwise-registration-intro.ipynb
 examples/__init__.py
 examples/ffd/README.md
 examples/ffd/__init__.py
 examples/ffd/__main__.py
 examples/ffd/engine.py
 examples/ffd/hooks.py
 examples/ffd/losses.py
```

### Comparing `hf-deepali-0.3.1/tests/_test_core_bspline.py` & `hf-deepali-0.3.2/tests/_test_core_bspline.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/tests/test_core_bspline.py` & `hf-deepali-0.3.2/tests/test_core_bspline.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/tests/test_core_cube.py` & `hf-deepali-0.3.2/tests/test_core_cube.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/tests/test_core_grid.py` & `hf-deepali-0.3.2/tests/test_core_grid.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/tests/test_core_image_utils.py` & `hf-deepali-0.3.2/tests/test_core_image_utils.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/tests/test_core_random.py` & `hf-deepali-0.3.2/tests/test_core_random.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/tests/test_core_tensor_utils.py` & `hf-deepali-0.3.2/tests/test_core_tensor_utils.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/tests/test_data_image.py` & `hf-deepali-0.3.2/tests/test_data_image.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from copy import deepcopy
 from typing import Tuple
 
+import numpy as np
 import pytest
 import torch
 from torch import Tensor
 from torch.nn import functional as F
 
 from deepali.core import ALIGN_CORNERS, Grid, functional as U
 from deepali.data import Image, ImageBatch
@@ -288,61 +289,105 @@
     assert type(batch._grid) is tuple
     assert len(batch._grid) == 1
     assert batch.data_ptr() == image.data_ptr()
 
 
 @pytest.mark.parametrize("zeros,grid", [(d, d) for d in (2, 3)], indirect=True)
 def test_image_batch_getitem(zeros: Tensor, grid: Grid) -> None:
-    batch = ImageBatch(zeros.unsqueeze(0).expand((5,) + zeros.shape), grid, dtype=torch.uint8)
+    grids = [deepcopy(grid) for _ in range(5)]  # make grids distinguishable
+    batch = ImageBatch(zeros.unsqueeze(0).expand((5,) + zeros.shape), grids, dtype=torch.uint8)
     for i in range(len(batch)):
         batch.tensor()[i] = i
     for i in range(len(batch)):
         image = batch[i]
         assert isinstance(image, Image)
-        assert image.grid() is grid
+        assert image.grid() is batch.grid(i)
         assert torch.allclose(image, torch.tensor(i, dtype=batch.dtype))
 
     image = batch[-1]
     assert isinstance(image, Image)
-    assert image.grid() is grid
+    assert image.grid() is batch.grid(-1)
     assert torch.allclose(image, torch.tensor(len(batch) - 1, dtype=batch.dtype))
 
     with pytest.raises(IndexError):
         batch[len(batch)]
 
     other = batch[0:1]
-    assert isinstance(other, ImageBatch)
+    assert type(other) is ImageBatch
+    assert len(other.grids()) == len(other)
     assert len(other) == 1
-    assert other.grids() == batch.grids()[0:1]
+    assert other.grid(0) is batch.grid(0)
     assert torch.allclose(other, torch.tensor(0, dtype=batch.dtype))
 
     other = batch[1:-1, 0:1]
-    assert isinstance(other, ImageBatch)
+    assert type(other) is ImageBatch
+    assert len(other.grids()) == len(other)
     assert len(other) == len(batch) - 2
-    assert other.grids() == batch.grids()[1:-1]
     for i, j in enumerate(range(1, len(batch) - 1)):
+        assert other.grid(i) is batch.grid(j)
         assert torch.allclose(other.tensor()[i], torch.tensor(j, dtype=batch.dtype))
+    assert torch.allclose(other, batch.tensor()[1:-1, 0:1])
 
     image = batch[3, :]
     assert isinstance(image, Image)
     assert image.grid() == grid
     assert torch.allclose(image, torch.tensor(3, dtype=image.dtype))
 
-    image = batch[4, 0]
-    assert isinstance(image, Image)
-    assert image.nchannels == 1
-    assert image.grid() == grid
-    assert torch.allclose(image, torch.tensor(4, dtype=image.dtype))
+    other = batch[4, 0]
+    assert type(other) is Tensor
+    assert torch.allclose(other, torch.tensor(4, dtype=image.dtype))
+    assert torch.allclose(other, batch.tensor()[4, 0])
+
+    other = batch[(0, 0)]
+    assert type(other) is Tensor
+    assert torch.allclose(other, batch.tensor()[(0, 0)])
+
+    other = batch[[0, 2]]
+    assert type(other) is ImageBatch
+    assert other.grids()[0] is batch.grid(0)
+    assert other.grids()[1] is batch.grid(2)
+    assert torch.allclose(other.tensor(), batch.tensor()[[0, 2]])
+
+    index = np.array([3, 4, 1])
+    item = batch[index]
+    assert type(item) is ImageBatch
+    assert len(item) == 3
+    assert item.grid(0) is batch.grid(3)
+    assert item.grid(1) is batch.grid(4)
+    assert item.grid(2) is batch.grid(1)
+    assert torch.allclose(item.tensor(), batch.tensor()[index])
+
+    index = torch.tensor([1, 2])
+    item = batch[index]
+    assert type(item) is ImageBatch
+    assert len(item) == 2
+    assert item.grid(0) is batch.grid(1)
+    assert item.grid(1) is batch.grid(2)
+    assert torch.allclose(item.tensor(), batch.tensor()[index])
 
     image = batch[4, 0:1]
     assert isinstance(image, Image)
     assert image.nchannels == 1
     assert image.grid() == grid
     assert torch.allclose(image, torch.tensor(4, dtype=image.dtype))
 
+    other = batch[:]
+    assert type(other) is type(batch)
+    assert other.data_ptr() == batch.data_ptr()
+
+    index = slice(0, 5, 2)
+    other = batch[index]
+    assert type(other) is type(batch)
+    assert other.shape[0] == 3
+    assert other.shape[1:] == batch.shape[1:]
+    assert other.grid(0) is batch.grid(0)
+    assert other.grid(1) is batch.grid(2)
+    assert other.grid(2) is batch.grid(4)
+    assert torch.allclose(other.tensor(), batch.tensor()[index])
+
     other = batch[:, :, :, :]
     assert isinstance(other, ImageBatch)
     assert other.grid() == batch.grid()
     assert other.shape == batch.shape
     assert torch.allclose(other, batch)
 
     other = batch[...]
@@ -365,39 +410,34 @@
 
     other = batch[..., :]
     assert isinstance(other, ImageBatch)
     assert other.grid() == batch.grid()
     assert other.shape == batch.shape
     assert torch.allclose(other, batch)
 
-    other = batch[..., 2, 0, :, :]
     if batch.ndim == 4:
-        assert isinstance(other, Image)
-        assert other.grid() == batch.grid()
-        assert other.nchannels == 1
-        assert other.shape[1:] == batch.shape[2:]
-        assert torch.allclose(other, torch.tensor(2, dtype=image.dtype))
-        another = batch[2, ..., 0, ..., :, :, ...]
-        assert isinstance(another, Image)
-        assert another.grid() == other.grid()
-        assert torch.allclose(another, other)
-    else:
-        assert isinstance(other, Tensor)
-
-    another = batch[..., 2, ..., 0, ..., :, :, ...]
-    assert type(another) == type(other)
-    assert torch.allclose(another, other)
+        other = batch[..., 2, 0:1, :, :]
+        assert type(other) is Image
+        assert other.grid() is batch.grid(2)
+        assert torch.allclose(other, batch.tensor()[..., 2, 0:1, :, :])
+        another = batch[2, ..., 0:1, ..., :, :, ...]
+        assert type(another) is Image
+        assert another.grid() is batch.grid(2)
+        assert torch.allclose(another, batch.tensor()[2, ..., 0:1, ..., :, :, ...])
+        another = batch[..., 2, ..., 0:1, ..., :, :, ...]
+        assert type(another) is Image
+        assert torch.allclose(another, batch.tensor()[..., 2, ..., 0, ..., :, :, ...])
 
     other = batch[:, ..., 0]
-    assert isinstance(other, Tensor)
+    assert type(other) is Tensor
 
     image = batch[3, ...]
-    assert isinstance(image, Image)
-    assert image.grid() == grid
-    assert torch.allclose(image, torch.tensor(3, dtype=image.dtype))
+    assert type(image) is Image
+    assert image.grid() is batch.grid(3)
+    assert torch.allclose(image, batch.tensor()[3, ...])
 
 
 @pytest.mark.parametrize("zeros,grid", [(d, d) for d in (3,)], indirect=True)
 def test_image_grid(zeros: Tensor, grid: Grid) -> None:
     image = Image(zeros, grid)
     assert image.grid() is grid
```

### Comparing `hf-deepali-0.3.1/tests/test_network_blocks.py` & `hf-deepali-0.3.2/tests/test_network_blocks.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/tests/test_network_layers.py` & `hf-deepali-0.3.2/tests/test_network_layers.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.1/tests/test_network_unet.py` & `hf-deepali-0.3.2/tests/test_network_unet.py`

 * *Files identical despite different names*

