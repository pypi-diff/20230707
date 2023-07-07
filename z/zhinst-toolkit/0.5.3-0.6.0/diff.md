# Comparing `tmp/zhinst-toolkit-0.5.3.tar.gz` & `tmp/zhinst-toolkit-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhinst-toolkit-0.5.3.tar", last modified: Tue Apr  4 14:53:18 2023, max compression
+gzip compressed data, was "zhinst-toolkit-0.6.0.tar", last modified: Fri Jul  7 14:54:18 2023, max compression
```

## Comparing `zhinst-toolkit-0.5.3.tar` & `zhinst-toolkit-0.6.0.tar`

### file list

```diff
@@ -1,252 +1,251 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:53:18.007925 zhinst-toolkit-0.5.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:53:17.979925 zhinst-toolkit-0.5.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:53:17.979925 zhinst-toolkit-0.5.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/.github/ISSUE_TEMPLATE/feature-request.md
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:53:17.983925 zhinst-toolkit-0.5.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-04-04 14:53:18.007925 zhinst-toolkit-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:53:17.983925 zhinst-toolkit-0.5.3/build_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/build_tools/test_wheels.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:53:17.983925 zhinst-toolkit-0.5.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:53:17.983925 zhinst-toolkit-0.5.3/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:53:17.975925 zhinst-toolkit-0.5.3/docs/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:53:17.983925 zhinst-toolkit-0.5.3/docs/source/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/docs/source/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/docs/source/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/docs/source/_templates/autosummary/module.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:53:17.983925 zhinst-toolkit-0.5.3/docs/source/about/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/docs/source/about/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    52432 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/docs/source/about/zhinst_logo_sep_2019_u3_1000.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:53:17.983925 zhinst-toolkit-0.5.3/docs/source/changelog/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/docs/source/changelog/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:53:17.983925 zhinst-toolkit-0.5.3/docs/source/contributing/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/docs/source/contributing/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:53:17.987925 zhinst-toolkit-0.5.3/docs/source/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/docs/source/examples/awg.nblink
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/docs/source/examples/common_device.rst
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/docs/source/examples/daq_module.nblink
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/docs/source/examples/hdawg.rst
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/docs/source/examples/hdawg_precomp_curve_fit.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/docs/source/examples/hf2.nblink
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/docs/source/examples/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/docs/source/examples/pqsc.rst
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/docs/source/examples/scope_module.nblink
--rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/docs/source/examples/shfqa.rst
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/docs/source/examples/shfqa_multistate_discrimination.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/docs/source/examples/shfqa_qubit_readout_measurement.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/docs/source/examples/shfqa_qubit_readout_weights.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/docs/source/examples/shfqa_sweeper.nblink
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/docs/source/examples/shfsg.rst
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/docs/source/examples/shfsg_rabi.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/docs/source/examples/shfsg_sine.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/docs/source/examples/sweeper_module.nblink
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/docs/source/examples/uhf.rst
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/docs/source/examples/uhf_boxcar.nblink
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/docs/source/examples/uhfqa.rst
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/docs/source/examples/uhfqa_result_unit.nblink
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:53:17.987925 zhinst-toolkit-0.5.3/docs/source/first_steps/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/docs/source/first_steps/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/docs/source/first_steps/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/docs/source/first_steps/nodetree.nblink
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/docs/source/first_steps/quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:53:17.987925 zhinst-toolkit-0.5.3/docs/source/images/
--rw-r--r--   0 runner    (1001) docker     (123)    31045 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/docs/source/images/zhinst_logo_sep_horiz_2019_1000.png
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:53:17.987925 zhinst-toolkit-0.5.3/docs/source/license/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/docs/source/license/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/docs/source/package_documentation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/docs/source/spelling_wordlist.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:53:17.991925 zhinst-toolkit-0.5.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    23741 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/examples/active_qubit_reset.md
--rw-r--r--   0 runner    (1001) docker     (123)    23245 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/examples/awg.md
--rw-r--r--   0 runner    (1001) docker     (123)    23445 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/examples/bell_state_stabilization.md
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/examples/daq_module.md
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/examples/device_settings_module.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      194 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/examples/generate_notebooks.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/examples/hdawg_precomp_curve_fit.md
--rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/examples/hf2.md
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/examples/impedance_module.md
--rw-r--r--   0 runner    (1001) docker     (123)    11269 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/examples/nodetree.md
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/examples/pid_advisor_module.md
--rw-r--r--   0 runner    (1001) docker     (123)    25669 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/examples/repeat_until_success.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:53:17.991925 zhinst-toolkit-0.5.3/examples/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   884740 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/examples/resources/example_multistate_signals.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/examples/rtlogger_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/examples/scope_module.md
--rw-r--r--   0 runner    (1001) docker     (123)    25722 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/examples/shfqa_multistate_discrimination.md
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/examples/shfqa_qubit_readout_measurement.md
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/examples/shfqa_qubit_readout_weights.md
--rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/examples/shfqa_shfqc_power_spectral_density.md
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/examples/shfqa_sweeper.md
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/examples/shfqc_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/examples/shfqc_propagation_delay.md
--rw-r--r--   0 runner    (1001) docker     (123)     7195 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/examples/shfqc_qubit_spectroscopy.md
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/examples/shfqc_resonator_spectroscopy_cw.md
--rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/examples/shfqc_resonator_spectroscopy_cw_power.md
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/examples/shfsg_rabi.md
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/examples/shfsg_sine.md
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/examples/sweeper_module.md
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/examples/test.spec.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/examples/uhf_boxcar.md
--rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/examples/uhfqa_result_unit.md
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:53:17.991925 zhinst-toolkit-0.5.3/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/scripts/generate_notebooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:53:17.991925 zhinst-toolkit-0.5.3/scripts/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/scripts/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/scripts/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/scripts/tests/test_zhinst_toolkit_symlink.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/scripts/zhinst_toolkit_symlink.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-04 14:53:18.011925 zhinst-toolkit-0.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:53:17.979925 zhinst-toolkit-0.5.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:53:17.979925 zhinst-toolkit-0.5.3/src/zhinst/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:53:17.991925 zhinst-toolkit-0.5.3/src/zhinst/toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/_min_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-04 14:53:17.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16105 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/command_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:53:17.991925 zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:53:17.995925 zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/devices/
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12630 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/devices/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/devices/hdawg.py
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/devices/pqsc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10222 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/devices/shfqa.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/devices/shfqc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8730 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/devices/shfsg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/devices/uhfli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/devices/uhfqa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:53:17.995925 zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/modules/base_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/modules/daq_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/modules/device_settings_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/modules/impedance_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/modules/pid_advisor_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/modules/precompensation_advisor_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/modules/scope_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/modules/shfqa_sweeper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/modules/sweeper_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:53:17.995925 zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/nodes/awg.py
--rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/nodes/command_table_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/nodes/multistate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/nodes/readout.py
--rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/nodes/shfqa_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/nodes/spectroscopy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9327 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:53:17.995925 zhinst-toolkit-0.5.3/src/zhinst/toolkit/nodetree/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/nodetree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/nodetree/connection_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/nodetree/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    46542 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/nodetree/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    18969 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/nodetree/nodetree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:53:17.995925 zhinst-toolkit-0.5.3/src/zhinst/toolkit/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/resources/ct_schema_hdawg.json
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/resources/ct_schema_shfsg.json
--rw-r--r--   0 runner    (1001) docker     (123)    64509 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/resources/nodedoc_hf2.json
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/resources/nodedoc_hf2_data_server.json
--rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/resources/shfqa_sweeper_nodes.json
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)    36853 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/session.py
--rw-r--r--   0 runner    (1001) docker     (123)    19263 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/src/zhinst/toolkit/waveform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:53:17.999925 zhinst-toolkit-0.5.3/src/zhinst_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-04-04 14:53:17.000000 zhinst-toolkit-0.5.3/src/zhinst_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-04-04 14:53:17.000000 zhinst-toolkit-0.5.3/src/zhinst_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 14:53:17.000000 zhinst-toolkit-0.5.3/src/zhinst_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-04 14:53:17.000000 zhinst-toolkit-0.5.3/src/zhinst_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-04 14:53:17.000000 zhinst-toolkit-0.5.3/src/zhinst_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:53:18.003925 zhinst-toolkit-0.5.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:53:18.003925 zhinst-toolkit-0.5.3/tests/command_table/
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/command_table/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:53:18.003925 zhinst-toolkit-0.5.3/tests/command_table/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/command_table/data/command_table_completed.json
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/command_table/data/command_table_schema_22_02.json
--rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/command_table/data/command_table_schema_22_08.json
--rw-r--r--   0 runner    (1001) docker     (123)    12093 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/command_table/test_command_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:53:18.007925 zhinst-toolkit-0.5.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    12499 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/data/list_nodes_hf2_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/data/nodedoc_awg_test.json
--rw-r--r--   0 runner    (1001) docker     (123)    20187 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/data/nodedoc_daq_test.json
--rw-r--r--   0 runner    (1001) docker     (123)   343552 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/data/nodedoc_dev1234.json
--rw-r--r--   0 runner    (1001) docker     (123)   550683 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/data/nodedoc_dev1234_hdawg.json
--rw-r--r--   0 runner    (1001) docker     (123)   343552 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/data/nodedoc_dev1234_mfli.json
--rw-r--r--   0 runner    (1001) docker     (123)   152345 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/data/nodedoc_dev1234_pqsc.json
--rw-r--r--   0 runner    (1001) docker     (123)   863116 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/data/nodedoc_dev1234_shfqa.json
--rw-r--r--   0 runner    (1001) docker     (123)   425097 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/data/nodedoc_dev1234_shfqc.json
--rw-r--r--   0 runner    (1001) docker     (123)   440459 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/data/nodedoc_dev1234_shfsg.json
--rw-r--r--   0 runner    (1001) docker     (123)   175027 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/data/nodedoc_dev1234_uhfli.json
--rw-r--r--   0 runner    (1001) docker     (123)   291109 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/data/nodedoc_dev1234_uhfqa.json
--rw-r--r--   0 runner    (1001) docker     (123)   349624 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/data/nodedoc_dev1234_zi.json
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/data/nodedoc_device_settings_test.json
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/data/nodedoc_fake.json
--rw-r--r--   0 runner    (1001) docker     (123)     8015 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/data/nodedoc_impedance_test.json
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/data/nodedoc_pid_advisor_test.json
--rw-r--r--   0 runner    (1001) docker     (123)    12778 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/data/nodedoc_precomensation_advisor_test.json
--rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/data/nodedoc_scope_test.json
--rw-r--r--   0 runner    (1001) docker     (123)    12886 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/data/nodedoc_sweeper_test.json
--rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/data/nodedoc_zi.json
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/data/preloadable_nodetree.json
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/data/waveform_descriptors.json
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/data/waveform_descriptors_large.json
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/data/zi_devices.json
--rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/test_awg.py
--rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/test_base_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/test_command_table_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/test_daq_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    19908 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/test_data_server_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/test_device_settings_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/test_example_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/test_examples_regex_match.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/test_hdawg.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/test_impedance_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/test_multistate.py
--rw-r--r--   0 runner    (1001) docker     (123)    35073 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/test_nodetree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/test_pid_advisor_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/test_pqsc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/test_precompensation_advisor_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/test_readout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/test_scope_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/test_shfqa.py
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/test_shfqa_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     8231 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/test_shfqa_sweeper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/test_shfqc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/test_shfsg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/test_spectroscopy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/test_sweeper_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/test_uhfli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/test_uhfqa.py
--rw-r--r--   0 runner    (1001) docker     (123)    13151 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tests/test_waveforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-04 14:52:56.000000 zhinst-toolkit-0.5.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:18.541399 zhinst-toolkit-0.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:18.465397 zhinst-toolkit-0.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:18.465397 zhinst-toolkit-0.6.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:18.465397 zhinst-toolkit-0.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     9201 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-07-07 14:54:18.541399 zhinst-toolkit-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:18.465397 zhinst-toolkit-0.6.0/build_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/build_tools/test_wheels.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:18.469397 zhinst-toolkit-0.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:18.469397 zhinst-toolkit-0.6.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:18.453397 zhinst-toolkit-0.6.0/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:18.469397 zhinst-toolkit-0.6.0/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/docs/source/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/docs/source/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/docs/source/_templates/autosummary/module.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:18.469397 zhinst-toolkit-0.6.0/docs/source/about/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/docs/source/about/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    52432 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/docs/source/about/zhinst_logo_sep_2019_u3_1000.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:18.469397 zhinst-toolkit-0.6.0/docs/source/changelog/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/docs/source/changelog/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:18.469397 zhinst-toolkit-0.6.0/docs/source/contributing/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/docs/source/contributing/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:18.477397 zhinst-toolkit-0.6.0/docs/source/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/docs/source/examples/awg.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/docs/source/examples/common_device.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/docs/source/examples/daq_module.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/docs/source/examples/hdawg.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/docs/source/examples/hdawg_precomp_curve_fit.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/docs/source/examples/hf2.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/docs/source/examples/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/docs/source/examples/pqsc.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/docs/source/examples/scope_module.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/docs/source/examples/shfqa.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/docs/source/examples/shfqa_multistate_discrimination.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/docs/source/examples/shfqa_qubit_readout_measurement.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/docs/source/examples/shfqa_qubit_readout_weights.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/docs/source/examples/shfqa_sweeper.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/docs/source/examples/shfsg.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/docs/source/examples/shfsg_rabi.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/docs/source/examples/shfsg_sine.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/docs/source/examples/sweeper_module.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/docs/source/examples/uhf.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/docs/source/examples/uhf_boxcar.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/docs/source/examples/uhfqa.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/docs/source/examples/uhfqa_result_unit.nblink
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:18.481397 zhinst-toolkit-0.6.0/docs/source/first_steps/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/docs/source/first_steps/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/docs/source/first_steps/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/docs/source/first_steps/nodetree.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/docs/source/first_steps/quickstart.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:18.481397 zhinst-toolkit-0.6.0/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    31045 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/docs/source/images/zhinst_logo_sep_horiz_2019_1000.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:18.481397 zhinst-toolkit-0.6.0/docs/source/license/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/docs/source/license/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/docs/source/package_documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/docs/source/spelling_wordlist.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:18.493398 zhinst-toolkit-0.6.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    23741 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/examples/active_qubit_reset.md
+-rw-r--r--   0 runner    (1001) docker     (123)    23245 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/examples/awg.md
+-rw-r--r--   0 runner    (1001) docker     (123)    23446 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/examples/bell_state_stabilization.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/examples/daq_module.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/examples/device_settings_module.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      194 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/examples/generate_notebooks.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/examples/hdawg_precomp_curve_fit.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/examples/hf2.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/examples/impedance_module.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11269 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/examples/nodetree.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/examples/pid_advisor_module.md
+-rw-r--r--   0 runner    (1001) docker     (123)    25670 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/examples/repeat_until_success.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:18.493398 zhinst-toolkit-0.6.0/examples/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   884740 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/examples/resources/example_multistate_signals.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/examples/rtlogger_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/examples/scope_module.md
+-rw-r--r--   0 runner    (1001) docker     (123)    25722 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/examples/shfqa_multistate_discrimination.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/examples/shfqa_qubit_readout_measurement.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/examples/shfqa_qubit_readout_weights.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/examples/shfqa_shfqc_power_spectral_density.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/examples/shfqa_sweeper.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/examples/shfqc_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/examples/shfqc_propagation_delay.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7195 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/examples/shfqc_qubit_spectroscopy.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/examples/shfqc_resonator_spectroscopy_cw.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/examples/shfsg_rabi.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/examples/shfsg_sine.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/examples/sweeper_module.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/examples/test.spec.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/examples/uhf_boxcar.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/examples/uhfqa_result_unit.md
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:18.493398 zhinst-toolkit-0.6.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/scripts/generate_notebooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:18.493398 zhinst-toolkit-0.6.0/scripts/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/scripts/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/scripts/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/scripts/tests/test_zhinst_toolkit_symlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/scripts/zhinst_toolkit_symlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-07 14:54:18.541399 zhinst-toolkit-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:18.457397 zhinst-toolkit-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:18.457397 zhinst-toolkit-0.6.0/src/zhinst/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:18.497398 zhinst-toolkit-0.6.0/src/zhinst/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/_min_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-07 14:54:18.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16105 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/command_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:18.497398 zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:18.501398 zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13284 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/devices/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/devices/hdawg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/devices/pqsc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/devices/shfqa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/devices/shfqc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8219 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/devices/shfsg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/devices/uhfli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/devices/uhfqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:18.505398 zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/modules/base_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/modules/daq_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/modules/device_settings_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/modules/impedance_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/modules/pid_advisor_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/modules/precompensation_advisor_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/modules/scope_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11124 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/modules/shfqa_sweeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/modules/sweeper_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:18.509398 zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/nodes/awg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/nodes/command_table_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/nodes/multistate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7317 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/nodes/readout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/nodes/shfqa_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/nodes/spectroscopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:18.509398 zhinst-toolkit-0.6.0/src/zhinst/toolkit/nodetree/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/nodetree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/nodetree/connection_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/nodetree/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42740 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/nodetree/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19870 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/nodetree/nodetree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:18.513398 zhinst-toolkit-0.6.0/src/zhinst/toolkit/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/resources/ct_schema_hdawg.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/resources/ct_schema_shfsg.json
+-rw-r--r--   0 runner    (1001) docker     (123)    64509 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/resources/nodedoc_hf2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/resources/nodedoc_hf2_data_server.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/resources/shfqa_sweeper_nodes.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37016 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19263 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/src/zhinst/toolkit/waveform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:18.513398 zhinst-toolkit-0.6.0/src/zhinst_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-07-07 14:54:18.000000 zhinst-toolkit-0.6.0/src/zhinst_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7419 2023-07-07 14:54:18.000000 zhinst-toolkit-0.6.0/src/zhinst_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 14:54:18.000000 zhinst-toolkit-0.6.0/src/zhinst_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-07 14:54:18.000000 zhinst-toolkit-0.6.0/src/zhinst_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-07 14:54:18.000000 zhinst-toolkit-0.6.0/src/zhinst_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:18.525398 zhinst-toolkit-0.6.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:18.525398 zhinst-toolkit-0.6.0/tests/command_table/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/command_table/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:18.525398 zhinst-toolkit-0.6.0/tests/command_table/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/command_table/data/command_table_completed.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/command_table/data/command_table_schema_22_02.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/command_table/data/command_table_schema_22_08.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12093 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/command_table/test_command_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:54:18.537399 zhinst-toolkit-0.6.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    12499 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/data/list_nodes_hf2_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/data/nodedoc_awg_test.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20187 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/data/nodedoc_daq_test.json
+-rw-r--r--   0 runner    (1001) docker     (123)   343552 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/data/nodedoc_dev1234.json
+-rw-r--r--   0 runner    (1001) docker     (123)   550683 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/data/nodedoc_dev1234_hdawg.json
+-rw-r--r--   0 runner    (1001) docker     (123)   343552 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/data/nodedoc_dev1234_mfli.json
+-rw-r--r--   0 runner    (1001) docker     (123)   152345 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/data/nodedoc_dev1234_pqsc.json
+-rw-r--r--   0 runner    (1001) docker     (123)   863116 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/data/nodedoc_dev1234_shfqa.json
+-rw-r--r--   0 runner    (1001) docker     (123)   425097 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/data/nodedoc_dev1234_shfqc.json
+-rw-r--r--   0 runner    (1001) docker     (123)   440459 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/data/nodedoc_dev1234_shfsg.json
+-rw-r--r--   0 runner    (1001) docker     (123)   175027 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/data/nodedoc_dev1234_uhfli.json
+-rw-r--r--   0 runner    (1001) docker     (123)   291109 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/data/nodedoc_dev1234_uhfqa.json
+-rw-r--r--   0 runner    (1001) docker     (123)   349624 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/data/nodedoc_dev1234_zi.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/data/nodedoc_device_settings_test.json
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/data/nodedoc_fake.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8015 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/data/nodedoc_impedance_test.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/data/nodedoc_pid_advisor_test.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12778 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/data/nodedoc_precomensation_advisor_test.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/data/nodedoc_scope_test.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12886 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/data/nodedoc_sweeper_test.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/data/nodedoc_zi.json
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/data/preloadable_nodetree.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/data/waveform_descriptors.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/data/waveform_descriptors_large.json
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/data/zi_devices.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/test_awg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/test_base_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/test_command_table_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/test_daq_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19906 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/test_data_server_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/test_device_settings_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/test_example_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/test_examples_regex_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/test_hdawg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/test_impedance_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/test_multistate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39336 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/test_nodetree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/test_pid_advisor_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/test_pqsc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/test_precompensation_advisor_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/test_readout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/test_scope_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/test_shfqa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/test_shfqa_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8231 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/test_shfqa_sweeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/test_shfqc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/test_shfsg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/test_spectroscopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/test_sweeper_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/test_uhfli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/test_uhfqa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13151 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tests/test_waveforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-07 14:53:47.000000 zhinst-toolkit-0.6.0/tox.ini
```

### Comparing `zhinst-toolkit-0.5.3/.github/ISSUE_TEMPLATE/feature-request.md` & `zhinst-toolkit-0.6.0/.github/ISSUE_TEMPLATE/feature-request.md`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/.github/workflows/codeql.yml` & `zhinst-toolkit-0.6.0/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/.github/workflows/docs.yml` & `zhinst-toolkit-0.6.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/.github/workflows/publish.yml` & `zhinst-toolkit-0.6.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/.github/workflows/tests.yml` & `zhinst-toolkit-0.6.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/.gitignore` & `zhinst-toolkit-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/CHANGELOG.md` & `zhinst-toolkit-0.6.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,21 @@
 # zhinst-toolkit Changelog
 
+## Version 0.6.0
+* Revert full support of `fnmatch` wildcards and instead use the LabOne wildcard support.
+  This means only `*` symbols are supported. A `*` in the middle of the path matches
+  everything instead of a `/`. A `*` at the end of the path matches everything.
+* Fix problem of garbage collection daq sessions. The problem was caused due to using
+  lru caches for instance methods. The usage of lru cache has now been bypassed or 
+  replaced with the `functools.cached_property` decorator (which is currently copied
+  to ensure support for python 3.7).
+* `device.factory_reset` now raises an exception if the factory reset was not successful (`#243`).
+* Fixed issue where calling a `Node` with `dir()` returned duplicate values on some nodes.
+* Factory preset is now available for SHFSG, SHFQA, SHFQA devices (`#249`).
+
 ## Version 0.5.3
 * Add internal trigger to SHFQA sweeper class.
 
 ## Version 0.5.2
 * Add SHFQA / SHFQC Power Spectral Density (PSD) node and example
 
 ## Version 0.5.1
@@ -22,15 +34,15 @@
 
 ## Version 0.5.0
 * Added full support for the following LabOne modules (no need to fallback to zhinst.core):
   * Scope Module
   * Sweeper Module
   * DAQ Module
 * Renamed `zhinst.toolkit.nodetree.node.WildcardResult` to `zhinst.toolkit.nodetree.helpers.NodeDict`
-* Added `active_validation` argument to `CommandTable`. By disabling it, `CommandTable` does not actively 
+* Added `active_validation` argument to `CommandTable`. By disabling it, `CommandTable` does not actively
   validate the inputs and therefore it improves the speed for command table creation.
 * Adapt `awg.enable_sequencer` to check the acknowledged value instead of using `wait_for_state_change`. This makes it much more stable when used with short sequences.
 * Fix issue with downloading waveforms from the device. This issue prevented reading waveforms from any other than the base channel.
 * Normalize the `zhinst-core` dependency version.
 * Update SHFQA Sweeper to expose new properties through nodes (`predicted_cycle_time`, `actual_hold_off_time`, `actual_settling_time`)
 * Tested against Python 3.11
 
@@ -38,48 +50,48 @@
 * Fix issue that prevented correct compilation of sequences for AWG cores other than the first one.
 
 ## Version 0.4.2
 * Embed multistate utils for the SHFQA into the node tree
   * shfqa.qachannels[n].readout.multistate.qudits[m].configure(settings)
   * shfqa.qachannels[n].readout.multistate.get_qudits_results()
 * Added new example for the multistate discrimination (shfqa_multistate_discrimination) for the SHFQA
-* Fixed issue `#181` (Wrong _device_type of awg node of UHFQA/UHFLI) which prevented 
+* Fixed issue `#181` (Wrong _device_type of awg node of UHFQA/UHFLI) which prevented
   the compilation of sequences.
 * Waveform validation moved from the `write_to_waveform_memory` into `Waveforms.validate`
 * Command Table `$schema` key removed from the output of `CommandTable.as_dict` function
 * Command Table validation changed to disabled by default
 * Command Table upload check disabled when called within a transaction.
 * New dependency `pyelftools` for extracting waveform information from a complied
   sequencer code.
 * Interface auto detection adapted to support `none`, which was introduced with LabOne 22.08
 
 ## Version 0.4.1
 * For all LabOne modules forward the `execute` function from the zhinst-core in zhinst-toolkit
 
 ## Version 0.4.0
-* Add new class `zhinst.toolkit.Sequence` that allows a more flexible use of 
+* Add new class `zhinst.toolkit.Sequence` that allows a more flexible use of
   sequences in toolkit (`#141`).
-* Add support for session wide transactions that bundle set command from all 
+* Add support for session wide transactions that bundle set command from all
   devices connected to the data server. (`#134`)
 * Add `from_existing_connection()` to `zhinst.toolkit.Session` to help reusing the existing DataServer connection.
 * Bugfix: Nodes with nameless options don't raise an exception when their enum attribute is called (`#165`).
 * Bugfix: Values of enumerated nodes can now be pickled (`#129`).
 * Bugfix: `SHFScope` `run()`  and `stop()` shows specified timeout value when `TimeoutError` is raised.
 * Bugfix: Allow capital letters in node paths. (`#173`).
 * Adapt toolkit to use the offline awg compiler when uploading a sequencer code to
   a awg node. Improves the performance a lot and also enables the uploading of
   a sequencer code within a transaction (Works both for AWGs and Generators).
 * Add new function `compile_sequencer_code` to the awg node.
 
 ## Version 0.3.5
 * Adapt AWG Waveform upload (`write_to_waveform_memory`) to append to existing transactions.
 * Make consistency validate during waveform upload optional (new flag `validate` in `write_to_waveform_memory`).
-* Add `get_sequence_snippet` function to `zhinst.toolkit.Waveforms` class. 
+* Add `get_sequence_snippet` function to `zhinst.toolkit.Waveforms` class.
   The function is able to generated a sequence code snippet that defines and assigns
-  the waveforms for this object. Additional meta information like an optional name 
+  the waveforms for this object. Additional meta information like an optional name
   or the output configuration can be specified through a newly added `Wave` class from `zhinst.toolkit.Waveforms`.
 * Getting a value by calling a wildcard node now returns `zhinst.toolkit.nodetree.node.WildcardResult`
 
 
 ## Version 0.3.4
 
 * `Commandtable.load_validation_schema` can also get the command table
```

### Comparing `zhinst-toolkit-0.5.3/CONTRIBUTING.rst` & `zhinst-toolkit-0.6.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/LICENSE` & `zhinst-toolkit-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/PKG-INFO` & `zhinst-toolkit-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhinst-toolkit
-Version: 0.5.3
+Version: 0.6.0
 Summary: Zurich Instruments Toolkit High Level API
 Home-page: https://github.com/zhinst/zhinst-toolkit
 Author: Zurich Instrument
 Author-email: info@zhinst.com
 Project-URL: Bug Tracker, https://github.com/zhinst/zhinst-toolkit/issues
 Project-URL: Documentation, https://docs.zhinst.com/zhinst-toolkit/en/latest/
 Project-URL: Release notes, https://docs.zhinst.com/zhinst-toolkit/en/latest/changelog/index.html
```

### Comparing `zhinst-toolkit-0.5.3/README.md` & `zhinst-toolkit-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/docs/Makefile` & `zhinst-toolkit-0.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/docs/make.bat` & `zhinst-toolkit-0.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/docs/source/_templates/autosummary/class.rst` & `zhinst-toolkit-0.6.0/docs/source/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/docs/source/_templates/autosummary/module.rst` & `zhinst-toolkit-0.6.0/docs/source/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/docs/source/about/zhinst_logo_sep_2019_u3_1000.png` & `zhinst-toolkit-0.6.0/docs/source/about/zhinst_logo_sep_2019_u3_1000.png`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/docs/source/conf.py` & `zhinst-toolkit-0.6.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/docs/source/examples/common_device.rst` & `zhinst-toolkit-0.6.0/docs/source/examples/common_device.rst`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/docs/source/examples/hdawg.rst` & `zhinst-toolkit-0.6.0/docs/source/examples/hdawg.rst`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/docs/source/examples/index.rst` & `zhinst-toolkit-0.6.0/docs/source/examples/index.rst`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/docs/source/examples/pqsc.rst` & `zhinst-toolkit-0.6.0/docs/source/examples/pqsc.rst`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/docs/source/examples/shfqa.rst` & `zhinst-toolkit-0.6.0/docs/source/examples/shfqa.rst`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/docs/source/examples/shfsg.rst` & `zhinst-toolkit-0.6.0/docs/source/examples/shfsg.rst`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/docs/source/examples/uhfqa.rst` & `zhinst-toolkit-0.6.0/docs/source/examples/uhfqa.rst`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/docs/source/first_steps/installation.rst` & `zhinst-toolkit-0.6.0/docs/source/first_steps/installation.rst`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/docs/source/first_steps/quickstart.rst` & `zhinst-toolkit-0.6.0/docs/source/first_steps/quickstart.rst`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/docs/source/images/zhinst_logo_sep_horiz_2019_1000.png` & `zhinst-toolkit-0.6.0/docs/source/images/zhinst_logo_sep_horiz_2019_1000.png`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/docs/source/index.rst` & `zhinst-toolkit-0.6.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/docs/source/package_documentation.rst` & `zhinst-toolkit-0.6.0/docs/source/package_documentation.rst`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/docs/source/spelling_wordlist.txt` & `zhinst-toolkit-0.6.0/docs/source/spelling_wordlist.txt`

 * *Files 10% similar despite different names*

```diff
@@ -128,8 +128,12 @@
 historylength
 demods
 natively
 subtree
 misconfiguration
 pre
 forwardwave
-backwardwave
+backwardwave
+labone
+LabOne
+lru
+func
```

### Comparing `zhinst-toolkit-0.5.3/examples/README.md` & `zhinst-toolkit-0.6.0/examples/README.md`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/examples/active_qubit_reset.md` & `zhinst-toolkit-0.6.0/examples/active_qubit_reset.md`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/examples/awg.md` & `zhinst-toolkit-0.6.0/examples/awg.md`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/examples/bell_state_stabilization.md` & `zhinst-toolkit-0.6.0/examples/bell_state_stabilization.md`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 shfsg = session.connect_device(shfsg_serial)
 pqsc = session.connect_device(pqsc_serial)
 ```
 
 ## Basic initial setup
 
 
-### Cocks and communications
+### Clocks and communications
 Configure clock resources such that the PQSC receives the reference clock by an external source, and then distributes it to the other devices via ZSync connections.
 
 ```python vscode={"languageId": "python"}
 # PQSC external reference clock
 pqsc.system.clocks.referenceclock.in_.source("external")
 pqsc.check_ref_clock()
```

### Comparing `zhinst-toolkit-0.5.3/examples/daq_module.md` & `zhinst-toolkit-0.6.0/examples/daq_module.md`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/examples/device_settings_module.md` & `zhinst-toolkit-0.6.0/examples/device_settings_module.md`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/examples/hdawg_precomp_curve_fit.md` & `zhinst-toolkit-0.6.0/examples/hdawg_precomp_curve_fit.md`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/examples/hf2.md` & `zhinst-toolkit-0.6.0/examples/hf2.md`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/examples/impedance_module.md` & `zhinst-toolkit-0.6.0/examples/impedance_module.md`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/examples/nodetree.md` & `zhinst-toolkit-0.6.0/examples/nodetree.md`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/examples/pid_advisor_module.md` & `zhinst-toolkit-0.6.0/examples/pid_advisor_module.md`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/examples/repeat_until_success.md` & `zhinst-toolkit-0.6.0/examples/repeat_until_success.md`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 shfsg = session.connect_device(shfsg_serial)
 pqsc = session.connect_device(pqsc_serial)
 ```
 
 ## Basic initial setup
 
 
-### Cocks and communications
+### Clocks and communications
 Configure clock resources such that the PQSC receives the reference clock by an external source, and then distributes it to the other devices via ZSync connections.
 
 ```python vscode={"languageId": "python"}
 # PQSC external reference clock
 pqsc.system.clocks.referenceclock.in_.source("external")
 pqsc.check_ref_clock()
```

### Comparing `zhinst-toolkit-0.5.3/examples/resources/example_multistate_signals.csv` & `zhinst-toolkit-0.6.0/examples/resources/example_multistate_signals.csv`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/examples/rtlogger_helpers.py` & `zhinst-toolkit-0.6.0/examples/rtlogger_helpers.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/examples/scope_module.md` & `zhinst-toolkit-0.6.0/examples/scope_module.md`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 
 ```python
 MIN_NUMBER_OF_RECORDS = 20
 
 scope_module = session.modules.scope
 scope_module.mode(1)
 scope_module.averager.weight(1)
-scope_module.historylength(20)
+scope_module.historylength(MIN_NUMBER_OF_RECORDS)
 scope_module.fft.window(0)
 ```
 
 ### Subscribing to the scope node data
 
 ```python
 wave_node = device.scopes[0].wave
```

### Comparing `zhinst-toolkit-0.5.3/examples/shfqa_multistate_discrimination.md` & `zhinst-toolkit-0.6.0/examples/shfqa_multistate_discrimination.md`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/examples/shfqa_qubit_readout_measurement.md` & `zhinst-toolkit-0.6.0/examples/shfqa_qubit_readout_measurement.md`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/examples/shfqa_qubit_readout_weights.md` & `zhinst-toolkit-0.6.0/examples/shfqa_qubit_readout_weights.md`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/examples/shfqa_shfqc_power_spectral_density.md` & `zhinst-toolkit-0.6.0/examples/shfqa_shfqc_power_spectral_density.md`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/examples/shfqa_sweeper.md` & `zhinst-toolkit-0.6.0/examples/shfqa_sweeper.md`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
 std_dev = rise_fall_len // 10
 gauss = gaussian(2 * rise_fall_len, std_dev)
 flat_top_gaussian = np.ones(int(envelope_duration * SHFQA_SAMPLING_FREQUENCY))
 flat_top_gaussian[0:rise_fall_len] = gauss[0:rise_fall_len]
 flat_top_gaussian[-rise_fall_len:] = gauss[-rise_fall_len:]
 ```
 
-#### Plot Envelope
+### Plot Envelope
 
 ```python
 import matplotlib.pyplot as plt
 plt.plot(flat_top_gaussian)
 plt.show()
 ```
```

### Comparing `zhinst-toolkit-0.5.3/examples/shfqc_helper.py` & `zhinst-toolkit-0.6.0/examples/shfqc_helper.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/examples/shfqc_propagation_delay.md` & `zhinst-toolkit-0.6.0/examples/shfqc_propagation_delay.md`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/examples/shfqc_qubit_spectroscopy.md` & `zhinst-toolkit-0.6.0/examples/shfqc_qubit_spectroscopy.md`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/examples/shfqc_resonator_spectroscopy_cw.md` & `zhinst-toolkit-0.6.0/examples/shfqc_resonator_spectroscopy_cw.md`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/examples/shfsg_rabi.md` & `zhinst-toolkit-0.6.0/examples/shfsg_rabi.md`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/examples/shfsg_sine.md` & `zhinst-toolkit-0.6.0/examples/shfsg_sine.md`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/examples/sweeper_module.md` & `zhinst-toolkit-0.6.0/examples/sweeper_module.md`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/examples/test.spec.yml` & `zhinst-toolkit-0.6.0/examples/test.spec.yml`

 * *Files 6% similar despite different names*

```diff
@@ -49,22 +49,20 @@
 shfqa_sweeper:
   device_type: "SHFQA2"
 
 shfqa_shfqc_power_spectral_density:
   device_type: "SHFQA2"
 
 shfqc_propagation_delay:
-  device_type: "SHFQC"
+  # device_type: "SHFQC"
+  skip: True
 
 shfqc_qubit_spectroscopy:
   device_type: "SHFQC"
 
-shfqc_resonator_spectroscopy_cw_power:
-  device_type: "SHFQC"
-
 shfqc_resonator_spectroscopy_cw:
   device_type: "SHFQC"
 
 shfsg_rabi:
   device_type: "SHFSG4"
 
 shfsg_sine:
@@ -74,8 +72,7 @@
   device_type: ["MFLI", "UHFLI"]
 
 uhf_boxcar:
   device_type: "UHFLI"
 
 uhfqa_result_unit:
   device_type: "UHFQA"
-
```

### Comparing `zhinst-toolkit-0.5.3/examples/uhf_boxcar.md` & `zhinst-toolkit-0.6.0/examples/uhf_boxcar.md`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/examples/uhfqa_result_unit.md` & `zhinst-toolkit-0.6.0/examples/uhfqa_result_unit.md`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/pyproject.toml` & `zhinst-toolkit-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/scripts/generate_notebooks.py` & `zhinst-toolkit-0.6.0/scripts/generate_notebooks.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/scripts/tests/test_zhinst_toolkit_symlink.py` & `zhinst-toolkit-0.6.0/scripts/tests/test_zhinst_toolkit_symlink.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/scripts/zhinst_toolkit_symlink.py` & `zhinst-toolkit-0.6.0/scripts/zhinst_toolkit_symlink.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/setup.cfg` & `zhinst-toolkit-0.6.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 package_dir = 
 	= src
 packages = find_namespace:
 python_requires = >=3.7
 use_scm_version = True
 install_requires = 
 	numpy>=1.13
-	zhinst-core>=23.02
+	zhinst-core>=23.06
 	zhinst-utils>=0.3.1
 	jsonschema>=3.2.0
 	jsonref>=0.2
 	typing_extensions>=4.1.1
 	pyelftools>=0.29
 include_package_data = True
```

### Comparing `zhinst-toolkit-0.5.3/src/zhinst/toolkit/__init__.py` & `zhinst-toolkit-0.6.0/src/zhinst/toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/src/zhinst/toolkit/command_table.py` & `zhinst-toolkit-0.6.0/src/zhinst/toolkit/command_table.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/devices/__init__.py` & `zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/devices/base.py` & `zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/devices/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 """
 import copy
 import json
 import logging
 import re
 import typing as t
 import warnings
-from functools import lru_cache
 from pathlib import Path
 
 from zhinst.utils._version import version as utils_version_str
 from zhinst.core import __version__ as zhinst_version_str
 
 from zhinst.toolkit._min_version import _MIN_DEVICE_UTILS_VERSION, _MIN_LABONE_VERSION
 from zhinst.toolkit.driver.parsers import node_parser
@@ -62,14 +61,16 @@
         # (the node of HF2 will not change any more so this is safe)
         preloaded_json = None
         if "HF2" in self._device_type:
             preloaded_json = self._load_preloaded_json(
                 Path(__file__).parent / "../../resources/nodedoc_hf2.json"
             )
 
+        self._streaming_nodes: t.Optional[t.List[Node]] = None
+
         nodetree = NodeTree(
             self._session.daq_server,
             prefix_hide=self._serial,
             list_nodes=[f"/{self._serial}/*"],
             preloaded_json=preloaded_json,
         )
         # Add predefined parseres (in node_parser) to nodetree nodes
@@ -82,23 +83,35 @@
     def __repr__(self):
         options = f"({self._options})" if self._options else ""
         options = options.replace("\n", ",")
         return str(
             f"{self.__class__.__name__}({self._device_type}" f"{options},{self.serial})"
         )
 
-    def factory_reset(self, *, deep: bool = True) -> None:
+    def factory_reset(self, *, deep: bool = True, timeout: int = 30) -> None:
         """Load the factory default settings.
 
         Args:
             deep: A flag that specifies if a synchronization
                 should be performed between the device and the data
                 server after loading the factory preset (default: True).
+            timeout: Timeout in seconds to wait for the factory reset to
+                complete.
+
+        Raises:
+            ToolkitError: If the factory preset could not be loaded.
+            TimeoutError: If the factory reset did not complete within the
+                given timeout.
         """
         self.system.preset.load(1, deep=deep)
+        self.system.preset.busy.wait_for_state_change(0, timeout=timeout)
+        if self.system.preset.error(deep=True)[1]:
+            raise ToolkitError(
+                f"Failed to load factory preset to device {self.serial.upper()}."
+            )
         logger.info(f"Factory preset is loaded to device {self.serial.upper()}.")
 
     @staticmethod
     def _version_string_to_tuple(version: str) -> t.Tuple[int, int, int]:
         """Converts a version string into a version tuple.
 
         Args:
@@ -245,26 +258,26 @@
             labone_version_str + "." + labone_revision_str
         )
         self._check_labone_version(
             self._version_string_to_tuple(zhinst_version_str), labone_version
         )
         self._check_firmware_update_status()
 
-    @lru_cache()
     def get_streamingnodes(self) -> t.List[Node]:
         """Create a list with all streaming nodes available.
 
         Returns:
             Available streaming node.
         """
-        streaming_nodes = []
-        for node, info in self:
-            if "Stream" in info.get("Properties"):
-                streaming_nodes.append(node)
-        return streaming_nodes
+        if self._streaming_nodes is None:
+            self._streaming_nodes = []
+            for node, info in self:
+                if "Stream" in info.get("Properties"):
+                    self._streaming_nodes.append(node)
+        return self._streaming_nodes
 
     def _load_preloaded_json(self, filename: Path) -> t.Optional[dict]:
         """Load a preloaded json and match the existing nodes.
 
         Args:
             Filename for the preloaded json.
```

### Comparing `zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/devices/hdawg.py` & `zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/devices/hdawg.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/devices/pqsc.py` & `zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/devices/pqsc.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/devices/shfqa.py` & `zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/devices/shfqa.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """SHFQA Instrument Driver."""
 
 import logging
 import typing as t
-import warnings
 
 import zhinst.utils.shfqa as utils
 
 from zhinst.toolkit.driver.devices.base import BaseInstrument
 from zhinst.toolkit.driver.nodes.awg import AWG
 from zhinst.toolkit.driver.nodes.readout import Readout
 from zhinst.toolkit.driver.nodes.shfqa_scope import SHFScope
 from zhinst.toolkit.driver.nodes.spectroscopy import Spectroscopy
+from zhinst.toolkit.exceptions import ToolkitError
 from zhinst.toolkit.interface import SHFQAChannelMode
 from zhinst.toolkit.nodetree import Node, NodeTree
 from zhinst.toolkit.nodetree.helper import (
     lazy_property,
     create_or_append_set_transaction,
 )
 from zhinst.toolkit.nodetree.node import NodeList
@@ -70,17 +70,17 @@
             clear_existing: Flag whether to clear the waveform memory before the
                 present upload. (default = True)
         """
         if (
             len(pulses.keys()) > 0
             and max(pulses.keys()) >= self._max_qubits_per_channel
         ):
-            raise RuntimeError(
+            raise ToolkitError(
                 f"The device only has {self._max_qubits_per_channel} qubits per channel"
-                f", but {max(pulses.keys())} where specified"
+                f", but {max(pulses.keys())} were specified."
             )
         with create_or_append_set_transaction(self._root):
             if clear_existing:
                 self.clearwave(1)
             if isinstance(pulses, Waveforms):
                 for slot in pulses.keys():
                     self.waveforms[slot].wave(
@@ -227,25 +227,14 @@
             self._index,
         )
 
 
 class SHFQA(BaseInstrument):
     """High-level driver for the Zurich Instruments SHFQA."""
 
-    def factory_reset(self, *, deep: bool = True) -> None:
-        """Load the factory default settings.
-
-        Args:
-            deep: A flag that specifies if a synchronization
-                should be performed between the device and the data
-                server after loading the factory preset (default: True).
-        """
-        warnings.warn("Factory preset is not yet supported for SHFQA.", RuntimeWarning)
-        logger.warning("Factory preset is not yet supported in SHFQA.")
-
     def start_continuous_sw_trigger(
         self, *, num_triggers: int, wait_time: float
     ) -> None:
         """Issues a specified number of software triggers.
 
         Issues a specified number of software triggers with a certain wait time
         in between. The function guarantees reception and proper processing of
```

### Comparing `zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/devices/shfsg.py` & `zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/devices/shfsg.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """SHFSG Instrument Driver."""
 
 import logging
 import typing as t
-import warnings
 
 import zhinst.utils.shfsg as utils
 
 from zhinst.toolkit.driver.devices.base import BaseInstrument
 from zhinst.toolkit.driver.nodes.awg import AWG
 from zhinst.toolkit.nodetree import Node
 from zhinst.toolkit.nodetree.helper import lazy_property
@@ -232,25 +231,14 @@
             self._device.device_options,
         )
 
 
 class SHFSG(BaseInstrument):
     """High-level driver for the Zurich Instruments SHFSG."""
 
-    def factory_reset(self, *, deep: bool = True) -> None:
-        """Load the factory default settings.
-
-        Args:
-            deep: A flag that specifies if a synchronization
-                should be performed between the device and the data
-                server after loading the factory preset (default: True).
-        """
-        warnings.warn("Factory preset is not yet supported for SHFSG.", RuntimeWarning)
-        logger.warning("Factory preset is not yet supported in SHFSG.")
-
     @lazy_property
     def sgchannels(self) -> t.Sequence[SGChannel]:
         """A Sequence of SG Channels."""
         return NodeList(
             [
                 SGChannel(self, self._session, self._tree + ("sgchannels", str(i)))
                 for i in range(len(self["sgchannels"]))
```

### Comparing `zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/devices/uhfli.py` & `zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/devices/uhfli.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/devices/uhfqa.py` & `zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/devices/uhfqa.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/modules/__init__.py` & `zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/modules/base_module.py` & `zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/modules/base_module.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/modules/daq_module.py` & `zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/modules/daq_module.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/modules/device_settings_module.py` & `zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/modules/device_settings_module.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/modules/impedance_module.py` & `zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/modules/impedance_module.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/modules/pid_advisor_module.py` & `zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/modules/pid_advisor_module.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/modules/precompensation_advisor_module.py` & `zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/modules/precompensation_advisor_module.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/modules/scope_module.py` & `zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/modules/scope_module.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/modules/shfqa_sweeper.py` & `zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/modules/shfqa_sweeper.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,21 @@
 import typing as t
 from collections import OrderedDict
 from dataclasses import asdict
 from enum import IntEnum
 from pathlib import Path
 
 import numpy as np
+from zhinst.core import ziDAQServer
 from zhinst.utils.shf_sweeper import AvgConfig, EnvelopeConfig, RfConfig
 from zhinst.utils.shf_sweeper import ShfSweeper as CoreSweeper
 from zhinst.utils.shf_sweeper import SweepConfig, TriggerConfig
-from zhinst.core import ziDAQServer
 
 from zhinst.toolkit.driver.parsers import Parse
+from zhinst.toolkit.exceptions import ToolkitError
 from zhinst.toolkit.nodetree import Node, NodeTree
 from zhinst.toolkit.nodetree.connection_dict import ConnectionDict
 from zhinst.toolkit.nodetree.helper import NodeDoc
 
 if t.TYPE_CHECKING:  # pragma: no cover
     from zhinst.toolkit.driver.devices import DeviceType
     from zhinst.toolkit.session import Session
@@ -191,15 +192,15 @@
 
     def _update_settings(self) -> None:
         """Update the ShfSweeper settings from the node tree.
 
         Converts the nodetree into a valid configuration for the SHFSweeper.
         """
         if not self.device():
-            raise RuntimeError(
+            raise ToolkitError(
                 "The device serial needs to be set before using the module."
             )
         data = OrderedDict()
         for config_class, parent_name in self._config_classes.items():
             config = OrderedDict()
             for parameter in asdict(config_class()):
                 value = self[parent_name[0]][
```

### Comparing `zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/modules/sweeper_module.py` & `zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/modules/sweeper_module.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/nodes/awg.py` & `zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/nodes/awg.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/nodes/command_table_node.py` & `zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/nodes/command_table_node.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Command Table Node adaptions."""
 import json
 import string
 import typing as t
-from functools import lru_cache
 from pathlib import Path
 
 from zhinst.toolkit.command_table import CommandTable
 from zhinst.toolkit.nodetree import Node, NodeTree
 
 _CT_RESOURCE_PATH = Path(__file__).parent.parent.parent / "resources"
 _CT_FILES = {
@@ -34,14 +33,15 @@
     """
 
     def __init__(
         self, root: NodeTree, tree: t.Tuple[str, ...], device_type: str
     ) -> None:
         Node.__init__(self, root, tree)
         self._device_type = device_type
+        self._schema: t.Optional[t.Dict[str, t.Any]] = None
 
     def check_status(self) -> bool:
         """Check status of the command table.
 
         Returns:
             Flag if a valid command table is loaded into the device.
 
@@ -52,27 +52,28 @@
         if ct_status >> 3:
             raise RuntimeError(
                 "Uploading of data to the command table failed "
                 "due to a JSON parsing error."
             )
         return ct_status == 1
 
-    @lru_cache()
     def load_validation_schema(self) -> t.Dict[str, t.Any]:
         """Load device command table validation schema.
 
         Returns:
             JSON validation schema for the device command tables.
         """
-        try:
-            return json.loads(self.schema())
-        except KeyError:
-            device_type_striped = self._device_type.lower().rstrip(string.digits)
-            with open(_CT_FILES[device_type_striped], encoding="utf-8") as file_:
-                return json.load(file_)
+        if self._schema is None:
+            try:
+                self._schema = json.loads(self.schema())
+            except KeyError:
+                device_type_striped = self._device_type.lower().rstrip(string.digits)
+                with open(_CT_FILES[device_type_striped], encoding="utf-8") as file_:
+                    self._schema = json.load(file_)
+        return self._schema  # type: ignore
 
     def upload_to_device(
         self,
         ct: t.Union[CommandTable, str, dict],
         *,
         validate: bool = False,
         check_upload: bool = True,
```

### Comparing `zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/nodes/multistate.py` & `zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/nodes/multistate.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/nodes/readout.py` & `zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/nodes/readout.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """zhinst-toolkit readout node adaptions."""
 import logging
 import typing as t
 
 import numpy as np
 import zhinst.utils.shfqa as utils
+from zhinst.toolkit.exceptions import ToolkitError
 
 from zhinst.toolkit.interface import AveragingMode
 from zhinst.toolkit.nodetree import Node, NodeTree
 from zhinst.toolkit.nodetree.helper import lazy_property
 from zhinst.toolkit.waveform import Waveforms
 from zhinst.toolkit.driver.nodes.multistate import MultiState
 
@@ -151,25 +152,24 @@
         """Configures the weighted integration.
 
         Args:
             weights: Dictionary containing the complex weight vectors, where
                 keys correspond to the indices of the integration units to be
                 configured.
             integration_delay: Delay in seconds before starting the readout.
-                (default = 0.0)
             clear_existing: Flag whether to clear the waveform memory before
-                the present upload. (default = True)
+                the present upload.
         """
         if (
             len(weights.keys()) > 0
             and max(weights.keys()) >= self._max_qubits_per_channel
         ):
-            raise RuntimeError(
+            raise ToolkitError(
                 f"The device only has {self._max_qubits_per_channel} qubits per channel"
-                f", but {max(weights.keys())} where specified"
+                f", but {max(weights.keys())} were specified."
             )
         waveform_dict = {}
         if isinstance(weights, Waveforms):
             for slot in weights.keys():
                 waveform_dict[slot] = weights.get_raw_vector(slot, complex_output=True)
         else:
             waveform_dict = weights
```

### Comparing `zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/nodes/shfqa_scope.py` & `zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/nodes/shfqa_scope.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/nodes/spectroscopy.py` & `zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/nodes/spectroscopy.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/src/zhinst/toolkit/driver/parsers.py` & `zhinst-toolkit-0.6.0/src/zhinst/toolkit/driver/parsers.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,14 +94,18 @@
         Args:
             value: Input value.
             factor: Factor that the value needs to be multiple of.
             rounding: Method of rounding (nearest, down).
 
         Returns:
             Rounded value.
+
+        .. versionchanged:: 0.5.3
+
+            Invalid `rounding` value raises `ValueError` instead of `RuntimeError`.
         """
         if abs(round(value / factor) * factor - value) < 1e-12:
             return value
         elif rounding == "nearest":
             v_rounded = round(value / factor) * factor
             logger.warning(
                 f"The value {value:.3e} is not a multiple of "
@@ -113,15 +117,15 @@
             v_rounded = round(value // factor) * factor
             logger.warning(
                 f"The value {value:.3e} is not a multiple of "
                 f"{factor:.3e} and will be rounded down to greatest "
                 f"multiple: {v_rounded:.3e}",
             )
             return v_rounded
-        raise RuntimeError(
+        raise ValueError(
             f"Invalid rounding type {rounding} only the "
             "following values are allowed: [nearest,down]"
         )
 
 
 node_parser = {
     "SHFQA": {
```

### Comparing `zhinst-toolkit-0.5.3/src/zhinst/toolkit/interface.py` & `zhinst-toolkit-0.6.0/src/zhinst/toolkit/interface.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/src/zhinst/toolkit/nodetree/connection_dict.py` & `zhinst-toolkit-0.6.0/src/zhinst/toolkit/nodetree/connection_dict.py`

 * *Files 15% similar despite different names*

```diff
@@ -41,23 +41,35 @@
             The value of the given path.
         """
         value = self._values[path]
         if callable(value):
             return value()
         return value
 
+    def _resolve_wildcards(self, path: str) -> t.List[str]:
+        path_raw = path.replace("/\\*/", "/[^/]*/")
+        path_raw_regex = re.compile(path_raw)
+        return list(filter(path_raw_regex.match, self._values.keys()))
+
     def _set_value(self, path: str, value: t.Any) -> None:
         """Set the value for a given path.
 
         If the value is callable it is called with the new value.
 
         Args:
             path: Key in the internal values dictionary.
             value: New value of the path.
         """
+        paths = self._resolve_wildcards(path)
+        if not paths:
+            raise KeyError(path)
+        for path in paths:
+            self._do_set_value(path, value)
+
+    def _do_set_value(self, path: str, value: t.Any) -> None:
         if callable(self._values[path]):
             self._values[path](value)
         else:
             self._values[path] = value
 
     def listNodesJSON(self, path: str, *args, **kwargs) -> str:
         """Returns a list of nodes with description found at the specified path."""
```

### Comparing `zhinst-toolkit-0.5.3/src/zhinst/toolkit/nodetree/node.py` & `zhinst-toolkit-0.6.0/src/zhinst/toolkit/nodetree/node.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,24 +5,21 @@
 import numbers
 import re
 import time
 import typing as t
 from collections import namedtuple
 from collections.abc import Sequence
 from enum import IntEnum
-from functools import lru_cache
 
 from zhinst.toolkit.nodetree.helper import (
-    create_or_append_set_transaction,
-    lazy_property,
     NodeDict,
+    lazy_property,
+    resolve_wildcards_labone,
 )
 
-from zhinst.core.errors import CoreError
-
 if t.TYPE_CHECKING:  # pragma: no cover
     from zhinst.toolkit.nodetree import NodeTree
 
 
 class NodeEnumMeta:
     """Custom Metaclass for NodeEnum.
 
@@ -112,15 +109,15 @@
         self._is_wildcard = False
         self._is_partial = False
         if any(wildcard in "".join(node.raw_tree) for wildcard in ["*", "?", "["]):
             self._info = {"Node": node.root.node_to_raw_path(node)}
             self._is_wildcard = True
         else:
             try:
-                self._info = next(iter(node.root.get_node_info(node).values()))
+                self._info = next(iter(node.root.get_node_info_raw(node).values()))
                 self._info["Node"] = self._info.get(
                     "Node", node.root.node_to_raw_path(node)
                 ).lower()
             except KeyError as error:
                 self._info = {"Node": error.args[0]}
                 if "sample" in node.raw_tree and "sample" != node.raw_tree[-1]:
                     path, signal = self._info["Node"].split("/sample/")
@@ -437,14 +434,15 @@
         root: Root of the nodetree.
         tree: Tree (node path as tuple) of the current node.
     """
 
     def __init__(self, root: "NodeTree", tree: tuple):
         self._root = root
         self._tree = tree
+        self._is_valid: t.Optional[bool] = None
 
     def __getattr__(self, name) -> "Node":
         return Node(self._root, self._tree + (name,))
 
     def __getitem__(self, name) -> "Node":
         name = str(name).lower()
         if "/" in name:
@@ -464,15 +462,19 @@
 
     def __repr__(self):
         return self.node_info.path
 
     def __dir__(self):
         dir_info = list(self._next_layer)
         for var, value in vars(self.__class__).items():
-            if isinstance(value, property) and not var.startswith("_"):
+            if (
+                isinstance(value, property)
+                and not var.startswith("_")
+                and var not in dir_info
+            ):
                 dir_info.append(var)
         return dir_info
 
     def __eq__(self, other):
         # buildin keywords are escaped with a tailing underscore
         # (https://pep8.org/#descriptive-naming-styles)
         own_node_list = tuple(node.rstrip("_") for node in self._tree)
@@ -555,16 +557,16 @@
         """Resolves potential wildcards.
 
         Also will resolve partial nodes to its leaf nodes.
 
         Returns:
             List of matched nodes in the raw path format
         """
-        return fnmatch.filter(
-            self._root.raw_dict.keys(), self._root.node_to_raw_path(self) + "*"
+        return resolve_wildcards_labone(
+            self._root.node_to_raw_path(self), self._root.raw_dict.keys()
         )
 
     def _parse_get_value(
         self, value: t.Any, enum: bool = True, parse: bool = True
     ) -> t.Any:
         """Parse the raw value from the data server.
 
@@ -703,24 +705,15 @@
         # a try catch block to avoid unnecessary comparisons
         kwargs.setdefault("settingsonly", False)
         kwargs.setdefault("flat", True)
         try:
             result_raw = self._root.connection.get(self.node_info.path, **kwargs)
         except TypeError:
             del kwargs["settingsonly"]
-            try:
-                result_raw = self._root.connection.get(self.node_info.path, **kwargs)
-            except (RuntimeError, TypeError):
-                # resolve wildecard and get the value of the resulting leaf nodes
-                nodes_raw = self._resolve_wildcards()
-                result_raw = self._root.connection.get(",".join(nodes_raw), **kwargs)
-        except RuntimeError:
-            # resolve wildecard and get the value of the resulting leaf nodes
-            nodes_raw = self._resolve_wildcards()
-            result_raw = self._root.connection.get(",".join(nodes_raw), **kwargs)
+            result_raw = self._root.connection.get(self.node_info.path, **kwargs)
         if not result_raw:
             raise KeyError(self.node_info.path)
         if not kwargs["flat"]:
             return result_raw
         result = {}
         for sub_node_raw, node_value in result_raw.items():
             sub_node = self._root.raw_path_to_node(sub_node_raw)
@@ -823,15 +816,15 @@
             AttributeError: If the connection does not support the necessary
                 function the set the value.
             KeyError: if the wildcard does not resolve to a valid node
             RuntimeError: if deep set is not possible
             TypeError: Connection does not support deep set
         """
         writable = self.node_info.writable
-        if writable:
+        if writable or self.node_info.contains_wildcards:
             if parse:
                 value = self.node_info.set_parser(value)
             if self._root.transaction.in_progress():
                 self._root.transaction.add(self, value)
             elif deep:
                 return self._parse_get_value(
                     self._set_deep(value, **kwargs), enum=enum, parse=parse
@@ -844,43 +837,20 @@
                     if self.node_info.type == "ZIVectorData":
                         self._root.connection.setVector(
                             self.node_info.path, value, **kwargs
                         )
                     else:
                         raise
             return None
-        if writable is None and (
-            self.node_info.contains_wildcards or self.node_info.is_partial
-        ):
-            self._set_wildcard(value, parse=parse, **kwargs)
-            return None
+        if self.node_info.is_partial:
+            return self["*"](value, deep=deep, enum=enum, parse=parse, **kwargs)
         if writable is False:
             raise AttributeError(f"{self.node_info.path} is read-only.")
         raise KeyError(self.node_info.path)
 
-    def _set_wildcard(self, value: t.Any, parse: bool = True, **kwargs) -> None:
-        """Performs a transactional set on all nodes that match the wildcard.
-
-        The kwargs will be forwarded to the mapped zhinst.core function call.
-
-        Args:
-            value: value
-            parse: Flag if the SetParser, if present, should be applied or not.
-                (default=True)
-
-        Raises:
-            KeyError: if the wildcard does not resolve to a valid node
-        """
-        nodes_raw = self._resolve_wildcards()
-        if not nodes_raw:
-            raise KeyError(self._root.node_to_raw_path(self))
-        with create_or_append_set_transaction(self._root):
-            for node_raw in nodes_raw:
-                self._root.raw_path_to_node(node_raw)(value, parse=parse, **kwargs)
-
     def _set_deep(self, value: t.Any, **kwargs) -> t.Any:
         """Set the node value from device.
 
         The kwargs will be forwarded to the mapped zhinst.core function call.
 
         Args:
             value: value
@@ -996,61 +966,48 @@
 
         In order to avoid fetching old data that is still in the buffer execute
         a sync command before subscribing to new data streams.
         """
         try:
             self._root.connection.subscribe(self.node_info.path)
         except RuntimeError as error:
-            nodes_raw = self._resolve_wildcards()
-            if not nodes_raw:
-                raise KeyError(self.node_info.path) from error
-            for node_raw in nodes_raw:
-                self._root.connection.subscribe(node_raw)
+            raise KeyError(self.node_info.path) from error
 
     def unsubscribe(self) -> None:
         """Unsubscribe this node (its child lead nodes).
 
         Use this command after recording to avoid buffer overflows that may
         increase the latency of subsequent commands.
         """
         try:
             self._root.connection.unsubscribe(self.node_info.path)
         except RuntimeError as error:
-            nodes_raw = self._resolve_wildcards()
-            if not nodes_raw:
-                raise KeyError(self.node_info.path) from error
-            for node_raw in nodes_raw:
-                self._root.connection.unsubscribe(node_raw)
+            raise KeyError(self.node_info.path) from error
 
     def get_as_event(self) -> None:
         """Trigger an event for that node (its child lead nodes).
 
         The node data is returned by a subsequent poll command.
         """
         try:
             self._root.connection.getAsEvent(self.node_info.path)
         except RuntimeError as error:
-            nodes_raw = self._resolve_wildcards()
-            if not nodes_raw:
-                raise KeyError(self.node_info.path) from error
-            for node_raw in nodes_raw:
-                self._root.connection.getAsEvent(node_raw)
+            raise KeyError(self.node_info.path) from error
 
     def child_nodes(
         self,
         *,
         recursive: bool = False,
         leavesonly: bool = False,
         settingsonly: bool = False,
         streamingonly: bool = False,
         subscribedonly: bool = False,
         basechannelonly: bool = False,
         excludestreaming: bool = False,
         excludevectors: bool = False,
-        full_wildcard: bool = False,
     ) -> t.Generator["Node", None, None]:
         """Generator for all child nodes that matches the filters.
 
         If the nodes does not contain any child nodes the generator will only
         contain the node itself (if it matches the filters).
 
         Warning:
@@ -1078,89 +1035,52 @@
             streamingonly: Returns only streaming nodes (default: False).
             subscribedonly: Returns only subscribed nodes
                 (default: False).
             basechannelonly: Return only one instance of a node in case
                 of multiple channels (default: False).
             excludestreaming: Exclude streaming nodes (default: False).
             excludevectors: Exclude vector nodes (default: False).
-            full_wildcard: Enables full wildcard support. Per default
-                only the asterisk wildcard is supported. (Automatically sets
-                recursive and leavesonly) (default = False)
 
         Returns:
             Generator of all child nodes that match the filters
         """
         raw_path = self._root.node_to_raw_path(self)
-        try:
-            raw_result = self._root.connection.listNodes(
-                raw_path,
-                recursive=recursive,
-                leavesonly=leavesonly,
-                settingsonly=settingsonly,
-                streamingonly=streamingonly,
-                subscribedonly=subscribedonly,
-                basechannelonly=basechannelonly,
-                excludestreaming=excludestreaming,
-                excludevectors=excludevectors,
-            )
-            for node_raw in raw_result:
-                yield self._root.raw_path_to_node(node_raw)
-        except CoreError as error:
-            if error.code != 32768:  # Replace with correct error in 23.02
-                raise
-            if not full_wildcard:
-                raise RuntimeError(
-                    "The node contains wildcards that the DataServer can not resolve. "
-                    "Use the `full_wildcard` flag to search for child nodes manually."
-                ) from error
-            nodes_raw = self._resolve_wildcards()
-            for node_raw in nodes_raw:
-                node = self._root.raw_path_to_node(node_raw)
-                if not (
-                    (settingsonly and not node.node_info.is_setting)
-                    or (excludevectors and node.node_info.is_vector)
-                    or (
-                        basechannelonly
-                        and any(number != 0 for number in re.findall(r"\d+", node_raw))
-                    )
-                    or (
-                        (excludestreaming or subscribedonly or streamingonly)
-                        and not self._root.connection.listNodes(
-                            node_raw[:-1] + "*",  # TODO remove once listNodes is fixed
-                            recursive=recursive,
-                            leavesonly=leavesonly,
-                            settingsonly=settingsonly,
-                            streamingonly=streamingonly,
-                            subscribedonly=subscribedonly,
-                            basechannelonly=basechannelonly,
-                            excludestreaming=excludestreaming,
-                            excludevectors=excludevectors,
-                        )
-                    )
-                ):
-                    yield node
+        raw_result = self._root.connection.listNodes(
+            raw_path,
+            recursive=recursive,
+            leavesonly=leavesonly,
+            settingsonly=settingsonly,
+            streamingonly=streamingonly,
+            subscribedonly=subscribedonly,
+            basechannelonly=basechannelonly,
+            excludestreaming=excludestreaming,
+            excludevectors=excludevectors,
+        )
+        for node_raw in raw_result:
+            yield self._root.raw_path_to_node(node_raw)
 
-    @lru_cache()
     def is_valid(self) -> bool:
         """Check if the node is a valid node.
 
         Valid node means it resolves to at least one existing node in the node
         tree. Meaning not only leaf nodes are valid nodes but also partial nodes
         and nodes containing wildcards.
 
         Returns:
             Flag if the node is a valid node
         """
-        keys = self._resolve_wildcards()
-        return len(keys) > 0
+        if self._is_valid is None:
+            keys = self._resolve_wildcards()
+            self._is_valid = len(keys) > 0
+        return self._is_valid
 
-    @lazy_property
+    @property
     def node_info(self) -> NodeInfo:
         """Additional information about the node."""
-        return NodeInfo(self)
+        return self.root.get_node_info(self)
 
     @property
     def raw_tree(self) -> t.Tuple[str, ...]:
         """Internal representation of the node."""
         return self._tree
 
     @property
```

### Comparing `zhinst-toolkit-0.5.3/src/zhinst/toolkit/nodetree/nodetree.py` & `zhinst-toolkit-0.6.0/src/zhinst/toolkit/nodetree/nodetree.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Protocol is available in the typing module since 3.8
 # Ift we only support 3.8 we should switch to t.Protocol
 from typing_extensions import Protocol
 
 from contextlib import contextmanager
 
 from zhinst.toolkit.nodetree.helper import NodeDoc, _NodeInfo
-from zhinst.toolkit.nodetree.node import Node
+from zhinst.toolkit.nodetree.node import Node, NodeInfo
 from zhinst.toolkit.exceptions import ToolkitError
 
 
 class Connection(Protocol):
     """Protocol class for the connection used in the nodetree.
 
     Every connection object used in the Nodetree is expected to have at least
@@ -198,14 +198,15 @@
                 self._flat_dict = {**self._flat_dict, **json.loads(nodes_json)}
         self._flat_dict = {key.lower(): value for key, value in self._flat_dict.items()}
         self._transaction = Transaction(self)
         # First Layer must be generate during initialization to calculate the
         # prefixes to keep
         self._first_layer: t.List[str] = []
         self._prefixes_keep: t.List[str] = []
+        self._node_infos: t.Dict[Node, NodeInfo] = {}
         self._generate_first_layer()
 
     def __getattr__(self, name):
         if not name.startswith("_"):
             return Node(self, (name.lower(),))
         return None
 
@@ -249,15 +250,42 @@
                 if node_split[2] not in self._first_layer:
                     self._first_layer.append(node_split[2])
             else:
                 if node_split[1] not in self._prefixes_keep:
                     self._prefixes_keep.append(node_split[1])
         self._first_layer.extend(self._prefixes_keep)
 
-    def get_node_info(
+    def get_node_info(self, node: Node):
+        """Get the node information for a node.
+
+        The nodetree caches the node information for each node.
+        This enables lazy created nodes to access its information
+        fast without additional cost.
+
+        Please note that this function returns a valid object for all
+        node objects. Even if the node does not exist on the device.
+
+        The cache (dict) lifetime is bound to the nodetree object and
+        each session/nodetree instance must have its own cache.
+
+        Args:
+            node: Node object
+
+        Returns:
+            Node information
+
+        .. versionadded:: 0.6.0
+        """
+        try:
+            return self._node_infos[node]
+        except KeyError:
+            self._node_infos[node] = NodeInfo(node)
+            return self._node_infos[node]
+
+    def get_node_info_raw(
         self, node: t.Union[Node, str]
     ) -> t.Dict[Node, t.Optional[t.Dict]]:
         """Get the information/data for a node.
 
         Unix shell-style wildcards are supported.
 
         Args:
@@ -319,15 +347,15 @@
             first_node = potential_key.split("/")[1]
             if not self._prefix_hide == first_node:
                 self._prefixes_keep.append(first_node)
                 self._first_layer.append(first_node)
         else:
             for single_key in keys:
                 self._flat_dict[single_key].update(updates)
-        Node.node_info.fget.cache_clear()
+        self._node_infos = {}
 
     def update_nodes(
         self,
         update_dict: t.Dict[t.Union[Node, str], t.Dict[str, t.Any]],
         *,
         add: bool = False,
         raise_for_invalid_node: bool = True,
```

### Comparing `zhinst-toolkit-0.5.3/src/zhinst/toolkit/resources/ct_schema_hdawg.json` & `zhinst-toolkit-0.6.0/src/zhinst/toolkit/resources/ct_schema_hdawg.json`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/src/zhinst/toolkit/resources/ct_schema_shfsg.json` & `zhinst-toolkit-0.6.0/src/zhinst/toolkit/resources/ct_schema_shfsg.json`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/src/zhinst/toolkit/resources/nodedoc_hf2.json` & `zhinst-toolkit-0.6.0/src/zhinst/toolkit/resources/nodedoc_hf2.json`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/src/zhinst/toolkit/resources/nodedoc_hf2_data_server.json` & `zhinst-toolkit-0.6.0/src/zhinst/toolkit/resources/nodedoc_hf2_data_server.json`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/src/zhinst/toolkit/resources/shfqa_sweeper_nodes.json` & `zhinst-toolkit-0.6.0/src/zhinst/toolkit/resources/shfqa_sweeper_nodes.json`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/src/zhinst/toolkit/sequence.py` & `zhinst-toolkit-0.6.0/src/zhinst/toolkit/sequence.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/src/zhinst/toolkit/session.py` & `zhinst-toolkit-0.6.0/src/zhinst/toolkit/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -877,33 +877,38 @@
         Args:
             raw_path: Raw node path (e.g. /dev1234/relative/path/to/node).
 
         Returns:
             Corresponding toolkit node object.
 
         Raises:
-            RuntimeError: If the node does not belong to the optional module or
+            ValueError: If the `raw_path` does not start with a leading dash.
+            ToolkitError: If the node does not belong to the optional module or
                 to a connected device.
+
+        .. versionchanged:: 0.5.3
+
+            Changed `RuntimeError` to `ValueError`.
         """
         if not raw_path.startswith("/"):
-            raise RuntimeError(
+            raise ValueError(
                 f"{raw_path} does not seem to be an absolute path. "
-                "(it must start with a leading slash)"
+                "It must start with a leading slash."
             )
         if module is not None:
             node = module.root.raw_path_to_node(raw_path)
             if node.raw_tree[0] in module.root:
                 return node
         try:
             serial = raw_path.split("/")[1]
             if serial == "zi":
                 return self.root.raw_path_to_node(raw_path)
             return self.devices[serial].root.raw_path_to_node(raw_path)
         except KeyError as error:
-            raise RuntimeError(
+            raise ToolkitError(
                 f"Node belongs to a device({raw_path.split('/')[1]}) not connected to "
                 "the Data Server."
             ) from error
 
     @contextmanager
     def set_transaction(self) -> t.Generator[None, None, None]:
         """Context manager for a transactional set.
```

### Comparing `zhinst-toolkit-0.5.3/src/zhinst/toolkit/waveform.py` & `zhinst-toolkit-0.6.0/src/zhinst/toolkit/waveform.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/src/zhinst_toolkit.egg-info/PKG-INFO` & `zhinst-toolkit-0.6.0/src/zhinst_toolkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhinst-toolkit
-Version: 0.5.3
+Version: 0.6.0
 Summary: Zurich Instruments Toolkit High Level API
 Home-page: https://github.com/zhinst/zhinst-toolkit
 Author: Zurich Instrument
 Author-email: info@zhinst.com
 Project-URL: Bug Tracker, https://github.com/zhinst/zhinst-toolkit/issues
 Project-URL: Documentation, https://docs.zhinst.com/zhinst-toolkit/en/latest/
 Project-URL: Release notes, https://docs.zhinst.com/zhinst-toolkit/en/latest/changelog/index.html
```

### Comparing `zhinst-toolkit-0.5.3/src/zhinst_toolkit.egg-info/SOURCES.txt` & `zhinst-toolkit-0.6.0/src/zhinst_toolkit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,14 @@
 examples/shfqa_qubit_readout_weights.md
 examples/shfqa_shfqc_power_spectral_density.md
 examples/shfqa_sweeper.md
 examples/shfqc_helper.py
 examples/shfqc_propagation_delay.md
 examples/shfqc_qubit_spectroscopy.md
 examples/shfqc_resonator_spectroscopy_cw.md
-examples/shfqc_resonator_spectroscopy_cw_power.md
 examples/shfsg_rabi.md
 examples/shfsg_sine.md
 examples/sweeper_module.md
 examples/test.spec.yml
 examples/uhf_boxcar.md
 examples/uhfqa_result_unit.md
 examples/resources/example_multistate_signals.csv
```

### Comparing `zhinst-toolkit-0.5.3/tests/command_table/conftest.py` & `zhinst-toolkit-0.6.0/tests/command_table/conftest.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/command_table/data/command_table_completed.json` & `zhinst-toolkit-0.6.0/tests/command_table/data/command_table_completed.json`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/command_table/data/command_table_schema_22_02.json` & `zhinst-toolkit-0.6.0/tests/command_table/data/command_table_schema_22_02.json`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/command_table/data/command_table_schema_22_08.json` & `zhinst-toolkit-0.6.0/tests/command_table/data/command_table_schema_22_08.json`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/command_table/test_command_table.py` & `zhinst-toolkit-0.6.0/tests/command_table/test_command_table.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/conftest.py` & `zhinst-toolkit-0.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/data/list_nodes_hf2_dev.txt` & `zhinst-toolkit-0.6.0/tests/data/list_nodes_hf2_dev.txt`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/data/nodedoc_awg_test.json` & `zhinst-toolkit-0.6.0/tests/data/nodedoc_awg_test.json`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/data/nodedoc_daq_test.json` & `zhinst-toolkit-0.6.0/tests/data/nodedoc_daq_test.json`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/data/nodedoc_dev1234.json` & `zhinst-toolkit-0.6.0/tests/data/nodedoc_dev1234.json`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/data/nodedoc_dev1234_hdawg.json` & `zhinst-toolkit-0.6.0/tests/data/nodedoc_dev1234_hdawg.json`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/data/nodedoc_dev1234_mfli.json` & `zhinst-toolkit-0.6.0/tests/data/nodedoc_dev1234_mfli.json`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/data/nodedoc_dev1234_pqsc.json` & `zhinst-toolkit-0.6.0/tests/data/nodedoc_dev1234_pqsc.json`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/data/nodedoc_dev1234_shfqa.json` & `zhinst-toolkit-0.6.0/tests/data/nodedoc_dev1234_shfqa.json`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/data/nodedoc_dev1234_shfqc.json` & `zhinst-toolkit-0.6.0/tests/data/nodedoc_dev1234_shfqc.json`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/data/nodedoc_dev1234_shfsg.json` & `zhinst-toolkit-0.6.0/tests/data/nodedoc_dev1234_shfsg.json`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/data/nodedoc_dev1234_uhfli.json` & `zhinst-toolkit-0.6.0/tests/data/nodedoc_dev1234_uhfli.json`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/data/nodedoc_dev1234_uhfqa.json` & `zhinst-toolkit-0.6.0/tests/data/nodedoc_dev1234_uhfqa.json`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/data/nodedoc_dev1234_zi.json` & `zhinst-toolkit-0.6.0/tests/data/nodedoc_dev1234_zi.json`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/data/nodedoc_device_settings_test.json` & `zhinst-toolkit-0.6.0/tests/data/nodedoc_device_settings_test.json`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/data/nodedoc_fake.json` & `zhinst-toolkit-0.6.0/tests/data/nodedoc_fake.json`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/data/nodedoc_impedance_test.json` & `zhinst-toolkit-0.6.0/tests/data/nodedoc_impedance_test.json`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/data/nodedoc_pid_advisor_test.json` & `zhinst-toolkit-0.6.0/tests/data/nodedoc_pid_advisor_test.json`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/data/nodedoc_precomensation_advisor_test.json` & `zhinst-toolkit-0.6.0/tests/data/nodedoc_precomensation_advisor_test.json`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/data/nodedoc_scope_test.json` & `zhinst-toolkit-0.6.0/tests/data/nodedoc_scope_test.json`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/data/nodedoc_sweeper_test.json` & `zhinst-toolkit-0.6.0/tests/data/nodedoc_sweeper_test.json`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/data/nodedoc_zi.json` & `zhinst-toolkit-0.6.0/tests/data/nodedoc_zi.json`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/data/waveform_descriptors.json` & `zhinst-toolkit-0.6.0/tests/data/waveform_descriptors.json`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/data/waveform_descriptors_large.json` & `zhinst-toolkit-0.6.0/tests/data/waveform_descriptors_large.json`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/test_awg.py` & `zhinst-toolkit-0.6.0/tests/test_awg.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/test_base.py` & `zhinst-toolkit-0.6.0/tests/test_base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import operator
+from collections import OrderedDict
 from contextlib import _GeneratorContextManager
 from unittest.mock import MagicMock, Mock, patch
 
 import pytest
 
 from zhinst.toolkit._min_version import _MIN_DEVICE_UTILS_VERSION, _MIN_LABONE_VERSION
 from zhinst.toolkit.driver.devices.base import BaseInstrument
@@ -42,22 +43,52 @@
     instrument = BaseInstrument("DEV1234", "HF2LI", hf2_session)
 
     assert instrument.device_type == "HF2LI"
     assert instrument.serial == "DEV1234"
     assert repr(instrument) == "BaseInstrument(HF2LI(OptionA),DEV1234)"
 
 
-def test_factory_reset(base_instrument, mock_connection):
-    base_instrument.factory_reset()
+def test_factory_reset_ok(base_instrument, mock_connection):
     dev_id = base_instrument.serial.lower()
+    mock_connection.return_value.getInt.return_value = 0
+    mock_connection.return_value.get.return_value = OrderedDict(
+        [
+            (
+                f"/{dev_id}/system/preset/error",
+                {"timestamp": [0], "value": [0]},
+            )
+        ]
+    )
+    base_instrument.factory_reset()
     mock_connection.return_value.syncSetInt.assert_called_once_with(
         f"/{dev_id}/system/preset/load", 1
     )
 
 
+def test_factory_reset_timeout(base_instrument, mock_connection):
+    mock_connection.return_value.getInt.return_value = 1
+    with pytest.raises(TimeoutError):
+        base_instrument.factory_reset(timeout=0.00001)
+
+
+def test_factory_reset_failure(base_instrument, mock_connection):
+    dev_id = base_instrument.serial.lower()
+    mock_connection.return_value.getInt.return_value = 0
+    mock_connection.return_value.get.return_value = OrderedDict(
+        [
+            (
+                f"/{dev_id}/system/preset/error",
+                {"timestamp": [0], "value": [1]},
+            )
+        ]
+    )
+    with pytest.raises(ToolkitError):
+        base_instrument.factory_reset()
+
+
 def test_get_streamingnodes(base_instrument):
     nodes = base_instrument.get_streamingnodes()
 
     assert base_instrument.dios[0].input in nodes
     assert base_instrument.scopes[0].wave in nodes
     assert base_instrument.demods[0].sample in nodes
```

### Comparing `zhinst-toolkit-0.5.3/tests/test_base_module.py` & `zhinst-toolkit-0.6.0/tests/test_base_module.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/test_command_table_node.py` & `zhinst-toolkit-0.6.0/tests/test_command_table_node.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/test_daq_module.py` & `zhinst-toolkit-0.6.0/tests/test_daq_module.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/test_data_server_session.py` & `zhinst-toolkit-0.6.0/tests/test_data_server_session.py`

 * *Files 0% similar despite different names*

```diff
@@ -308,15 +308,15 @@
 
     mock_connection.return_value.getString.side_effect = get_string_side_effect
     result = session.raw_path_to_node("/dev1234/test/a/b/c")
     assert result.raw_tree == ("test", "a", "b", "c")
     assert result.root.prefix_hide == "dev1234"
 
     # Only absolut paths are supported
-    with pytest.raises(RuntimeError) as e_info:
+    with pytest.raises(ValueError) as e_info:
         session.raw_path_to_node("dev1234/test/a/b/c")
 
     # Not connected device
     with pytest.raises(RuntimeError) as e_info:
         session.raw_path_to_node("/dev1235/test/a/b/c")
 
     # with optional module
```

### Comparing `zhinst-toolkit-0.5.3/tests/test_device_settings_module.py` & `zhinst-toolkit-0.6.0/tests/test_device_settings_module.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/test_example_config.py` & `zhinst-toolkit-0.6.0/tests/test_example_config.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/test_examples_regex_match.py` & `zhinst-toolkit-0.6.0/tests/test_examples_regex_match.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/test_generator.py` & `zhinst-toolkit-0.6.0/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/test_hdawg.py` & `zhinst-toolkit-0.6.0/tests/test_hdawg.py`

 * *Files 24% similar despite different names*

```diff
@@ -32,41 +32,29 @@
     hdawg.enable_qccs_mode()
     mock_connection.return_value.set.assert_called_with(
         [
             ("/dev1234/system/clocks/referenceclock/source", "zsync"),
             ("/dev1234/dios/0/interface", 0),
             ("/dev1234/dios/0/mode", "qccs"),
             ("/dev1234/dios/0/drive", 12),
-            ("/dev1234/awgs/0/dio/strobe/slope", "off"),
-            ("/dev1234/awgs/1/dio/strobe/slope", "off"),
-            ("/dev1234/awgs/2/dio/strobe/slope", "off"),
-            ("/dev1234/awgs/3/dio/strobe/slope", "off"),
-            ("/dev1234/awgs/0/dio/valid/polarity", "none"),
-            ("/dev1234/awgs/1/dio/valid/polarity", "none"),
-            ("/dev1234/awgs/2/dio/valid/polarity", "none"),
-            ("/dev1234/awgs/3/dio/valid/polarity", "none"),
+            ("/dev1234/awgs/*/dio/strobe/slope", "off"),
+            ("/dev1234/awgs/*/dio/valid/polarity", "none"),
         ]
     )
     mock_connection.reset_mock()
     with hdawg.set_transaction():
         hdawg.enable_qccs_mode()
     mock_connection.return_value.set.assert_called_with(
         [
             ("/dev1234/system/clocks/referenceclock/source", "zsync"),
             ("/dev1234/dios/0/interface", 0),
             ("/dev1234/dios/0/mode", "qccs"),
             ("/dev1234/dios/0/drive", 12),
-            ("/dev1234/awgs/0/dio/strobe/slope", "off"),
-            ("/dev1234/awgs/1/dio/strobe/slope", "off"),
-            ("/dev1234/awgs/2/dio/strobe/slope", "off"),
-            ("/dev1234/awgs/3/dio/strobe/slope", "off"),
-            ("/dev1234/awgs/0/dio/valid/polarity", "none"),
-            ("/dev1234/awgs/1/dio/valid/polarity", "none"),
-            ("/dev1234/awgs/2/dio/valid/polarity", "none"),
-            ("/dev1234/awgs/3/dio/valid/polarity", "none"),
+            ("/dev1234/awgs/*/dio/strobe/slope", "off"),
+            ("/dev1234/awgs/*/dio/valid/polarity", "none"),
         ]
     )
 
 
 def test_awg(hdawg):
     assert len(hdawg.awgs) == 4
     assert isinstance(hdawg.awgs[0], AWG)
```

### Comparing `zhinst-toolkit-0.5.3/tests/test_impedance_module.py` & `zhinst-toolkit-0.6.0/tests/test_impedance_module.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/test_multistate.py` & `zhinst-toolkit-0.6.0/tests/test_multistate.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/test_nodetree.py` & `zhinst-toolkit-0.6.0/tests/test_nodetree.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 from array import array
 from collections import OrderedDict
 from pathlib import Path
 from types import GeneratorType
 from unittest.mock import MagicMock, Mock
 from copy import deepcopy
 import pickle
+import gc
 
 import pytest
 from numpy import array as nparray
 
 from zhinst.toolkit.driver.devices import HDAWG
 from zhinst.toolkit.nodetree import Node, NodeTree
 from zhinst.toolkit.nodetree.connection_dict import ConnectionDict
 from zhinst.toolkit.nodetree.node import NodeList
+from zhinst.toolkit.nodetree.helper import resolve_wildcards_labone
 
 from zhinst.core.errors import CoreError
 
 
 @pytest.fixture()
 def data_dir(request):
     yield Path(request.fspath).parent / "data"
@@ -238,14 +240,30 @@
     assert tree.test.path[0].node_info.set_parser(5) == 7
 
     # dynamic node
     with pytest.raises(KeyError):
         tree.demods.waves[0].node_info.unit
 
 
+def test_node_dir_property_not_duplicated(connection):
+    class MockNode(Node):
+        def __init__(self, root: "NodeTree", tree: tuple):
+            self._root = root
+            self._tree = tree
+
+        @property
+        def features(self):
+            pass
+
+    tree = NodeTree(connection, "DEV1234")
+    assert "features" in dir(tree)
+    node = MockNode(tree, ())
+    assert len(dir(node)) == len(set(dir(node)))
+
+
 def test_wildcard_node(connection):
     tree = NodeTree(connection, "DEV1234")
     wildcard_node = tree.demods["*"].rate
     assert wildcard_node.node_info.path == "/dev1234/demods/*/rate"
     with pytest.raises(KeyError) as e_info:
         wildcard_node.node_info.description
 
@@ -254,14 +272,15 @@
     wildcard_node(1)
     with tree.set_transaction():
         tree.demods["*"].rate(1)
 
     connection.get.return_value = None
     with pytest.raises(KeyError) as e_info:
         tree.hello["*"].rate()
+    connection.set.side_effect = RuntimeError("test")
     with pytest.raises(KeyError) as e_info:
         tree.hello["*"].rate(1)
 
 
 def test_get_cached(connection):
     tree = NodeTree(connection, "DEV1234")
 
@@ -447,20 +466,14 @@
                 },
             )
         ]
     )
     connection.get.side_effect = [TypeError(), return_value]
     assert tree.demods()[tree.demods[0].impedance] == 123
 
-    connection.get.side_effect = [TypeError(), RuntimeError(), return_value]
-    assert tree.demods()[tree.demods[0].impedance] == 123
-
-    connection.get.side_effect = [RuntimeError(), return_value]
-    assert tree.demods()[tree.demods[0].impedance] == 123
-
 
 def test_set(connection):
     tree = NodeTree(connection, "DEV1234")
     tree.demods[0].rate(22.0)
     connection.set.assert_called_with(tree.demods[0].rate.node_info.path, 22.0)
     tree.demods[0].rate(22.0, test=True)
     connection.set.assert_called_with(
@@ -486,14 +499,20 @@
     with pytest.raises(TypeError):
         tree.demods[0].rate("test", deep=True)
 
     with pytest.raises(KeyError):
         tree.demods.test("test")
 
 
+def test_set_partial(connection):
+    tree = NodeTree(connection, "DEV1234")
+    tree.demods[0](22.0)
+    connection.set.assert_called_with(tree.demods[0]["*"].node_info.path, 22.0)
+
+
 def test_runtimerror_set_set_vector(connection):
     # tree.system.impedance.calib.user.data does work with set, but for
     # testing purposes call it
     tree = NodeTree(connection, "DEV1234")
     connection.set = Mock(side_effect=RuntimeError)
     tree.system.impedance.calib.user.data(b"Test Binary Data")
     connection.setVector.assert_called_with(
@@ -541,70 +560,74 @@
 
     with pytest.raises(RuntimeError) as e_info:
         with tree.set_transaction():
             with tree.set_transaction():
                 pass
 
 
-def test_get_node_info(connection):
+def test_get_node_info_raw(connection):
     tree = NodeTree(connection, "DEV1234")
     # raw get
-    assert tree.get_node_info("demods/0/rate") == tree.get_node_info(
+    assert tree.get_node_info_raw("demods/0/rate") == tree.get_node_info_raw(
         tree.demods[0].rate
     )
-    assert tree.get_node_info("/dev1234/demods/0/rate") == tree.get_node_info(
+    assert tree.get_node_info_raw("/dev1234/demods/0/rate") == tree.get_node_info_raw(
         tree.demods[0].rate
     )
     with pytest.raises(KeyError) as e_info:
-        tree.get_node_info("zi/config/open")
-    assert tree.get_node_info("/zi/config/open") == tree.get_node_info(
+        tree.get_node_info_raw("zi/config/open")
+    assert tree.get_node_info_raw("/zi/config/open") == tree.get_node_info_raw(
         tree.zi.config.open
     )
     with pytest.raises(KeyError) as e_info:
-        tree.get_node_info("/demods/0/rate")
+        tree.get_node_info_raw("/demods/0/rate")
     assert e_info.value.args[0] == "/demods/0/rate"
     with pytest.raises(KeyError):
-        tree.get_node_info("dev1234/demods/0/rate")
+        tree.get_node_info_raw("dev1234/demods/0/rate")
     with pytest.raises(KeyError) as e_info:
-        tree.get_node_info("no/real/element")
+        tree.get_node_info_raw("no/real/element")
     assert e_info.value.args[0] == "/dev1234/no/real/element"
 
     # raw get wildcards
-    assert tree.get_node_info("demods/*/rate") == tree.get_node_info("demods/?/rate")
-    assert len(tree.get_node_info("demods/0/*")) > 1
+    assert tree.get_node_info_raw("demods/*/rate") == tree.get_node_info_raw(
+        "demods/?/rate"
+    )
+    assert len(tree.get_node_info_raw("demods/0/*")) > 1
     with pytest.raises(KeyError) as e_info:
-        tree.get_node_info("demods/0/real/*")
+        tree.get_node_info_raw("demods/0/real/*")
     assert e_info.value.args[0] == "/dev1234/demods/0/real/*"
     with pytest.raises(KeyError) as e_info:
-        tree.get_node_info("demod/0/*")
+        tree.get_node_info_raw("demod/0/*")
     assert e_info.value.args[0] == "/dev1234/demod/0/*"
 
 
 def test_update_node(connection):
     tree = NodeTree(connection, "DEV1234")
 
     tree.update_node("demods/0/rate", {"Unit": "test"})
     assert tree.demods[0].rate.node_info.unit == "test"
     tree.update_node("demods/0/rate", {"Test": "test"})
     assert (
-        next(iter(tree.get_node_info("demods/0/rate").values())).get("Test", None)
+        next(iter(tree.get_node_info_raw("demods/0/rate").values())).get("Test", None)
         == "test"
     )
     tree.update_node("demods/0/rate", {"Unit": "test2", "Test2": True})
     assert tree.demods[0].rate.node_info.unit == "test2"
-    assert next(iter(tree.get_node_info("demods/0/rate").values())).get("Test2", None)
+    assert next(iter(tree.get_node_info_raw("demods/0/rate").values())).get(
+        "Test2", None
+    )
 
     # new Node
     with pytest.raises(KeyError) as e_info:
         tree.update_node("/test", {"Node": "test"})
     assert e_info.value.args[0] == "/test"
 
     assert str(tree.test) == "/dev1234/test"
     tree.update_node("/test", {"Node": "test"}, add=True)
-    tree.get_node_info(tree.test)
+    tree.get_node_info_raw(tree.test)
     assert tree.test.node_info["Node"] == "test"
 
     assert str(tree.demods[0].test) == "/dev1234/demods/0/test"
     tree.update_node("demods/0/test", {"Node": "test"}, add=True)
     assert str(tree.demods[0].test) == "test"
 
     tree.update_node("demods/0/rate", {"Properties": "Write"})
@@ -695,19 +718,14 @@
 
 def test_get_as_event(connection):
     tree = NodeTree(connection, "DEV1234")
 
     tree.demods[0].sample.get_as_event()
     connection.getAsEvent.assert_called_once_with(tree.demods[0].sample.node_info.path)
 
-    connection.getAsEvent.side_effect = [RuntimeError(), None, None]
-    tree.demods["[1,2]"].sample.get_as_event()
-    connection.getAsEvent.assert_any_call(tree.demods[1].sample.node_info.path)
-    connection.getAsEvent.assert_any_call(tree.demods[2].sample.node_info.path)
-
     connection.getAsEvent.side_effect = RuntimeError()
     with pytest.raises(KeyError):
         tree.demods["*"].test.get_as_event()
 
 
 def test_child_nodes(connection):
     tree = NodeTree(connection, "DEV1234")
@@ -787,21 +805,14 @@
         list(tree.demods["*"].child_nodes())
     assert e_info.value.args[0] == "Weird fail"
     connection.listNodes.side_effect = CoreError("Unrelated Error", 1111)
     with pytest.raises(CoreError) as e_info:
         list(tree.demods["*"].child_nodes())
     assert e_info.value.args[0] == "Unrelated Error"
 
-    connection.listNodes.side_effect = CoreError("Path format invalid", 32768)
-    with pytest.raises(RuntimeError) as e_info:
-        list(tree.demods["[0,1]"].child_nodes())
-    assert "full_wildcard" in e_info.value.args[0]
-
-    assert list(tree.demods["*"].child_nodes(full_wildcard=True))
-
 
 def test_subscribe(connection):
     tree = NodeTree(connection, "DEV1234")
 
     tree.demods[0].sample.subscribe()
     connection.subscribe.assert_called_once_with(tree.demods[0].sample.node_info.path)
 
@@ -879,14 +890,29 @@
 
     test_dict = {tree.demods[0].rate: 0, tree.demods[0].trigger: 1}
 
     assert test_dict[tree.demods[0].rate] == 0
     assert test_dict[tree.demods[0].trigger] == 1
 
 
+def test_hash_node_info(connection):
+    tree = NodeTree(connection, "DEV1234")
+
+    test_dict = {tree.demods[0].rate.node_info: 0, tree.demods[0].trigger.node_info: 1}
+
+    assert test_dict[tree.demods[0].rate.node_info] == 0
+    assert test_dict[tree.demods[0].trigger.node_info] == 1
+
+
+def test_eq_node_info(connection):
+    tree = NodeTree(connection, "DEV1234")
+
+    assert tree.demods[0].rate.node_info == tree["demods/0"].rate.node_info
+
+
 def test_connection_dict(data_dir):
     data = {"/car/seat": 4, "/car/color": "blue", "/street/length": 110.4}
     json_path = data_dir / "nodedoc_fake.json"
     with json_path.open("r", encoding="UTF-8") as file:
         nodes_json = json.loads(file.read())
     connection = ConnectionDict(data, nodes_json)
 
@@ -903,17 +929,17 @@
     assert tree.street.length(deep=True) == (None, 1.0)
 
     tree.car["*"](1)
     assert tree.car.seat() == 1
     assert tree.car.color() == "1"
 
     # subscribe and unsubscribe is not supported
-    with pytest.raises(RuntimeError) as e_info:
+    with pytest.raises(KeyError) as e_info:
         tree.car.seat.subscribe()
-    with pytest.raises(RuntimeError) as e_info:
+    with pytest.raises(KeyError) as e_info:
         tree.car.seat.unsubscribe()
 
     tree = NodeTree(connection, list_nodes=["/car/*"])
     assert tree.car.seat() == 1
     assert tree.car.color() == "1"
     with pytest.raises(KeyError):
         tree.street.length()
@@ -928,14 +954,34 @@
     with pytest.raises(TypeError):
         tree.car.seat()
     assert tree.car.color() == "{'blue'}"
     with pytest.raises(TypeError):
         tree.street.length()
 
 
+def test_connection_dict_set_list(data_dir):
+    data = {"/car/seat": 4, "/car/color": "blue", "/street/length": 110.4}
+    json_path = data_dir / "nodedoc_fake.json"
+    with json_path.open("r", encoding="UTF-8") as file:
+        nodes_json = json.loads(file.read())
+    connection = ConnectionDict(data, nodes_json)
+    connection.set([("/car/seat", 1), ("/car/color", "red")])
+    assert {"/car/seat": 1, "/car/color": "red", "/street/length": 110.4} == data
+
+
+def test_connection_dict_missing_node(data_dir):
+    data = {"/car/seat": 4, "/car/color": "blue", "/street/length": 110.4}
+    json_path = data_dir / "nodedoc_fake.json"
+    with json_path.open("r", encoding="UTF-8") as file:
+        nodes_json = json.loads(file.read())
+    connection = ConnectionDict(data, nodes_json)
+    with pytest.raises(KeyError):
+        connection.set("/car/test", 5)
+
+
 def test_connection_dict_callable_nodes(data_dir):
     global seat
     seat = 6
 
     def update_seat(value=None):
         global seat
         if value is None:
@@ -983,14 +1029,115 @@
 
 def test_nodelist_hash(connection, hdawg):
     nt = NodeTree(connection, "DEV1234")
     bar = NodeList([hdawg], nt, ("foobar",))
     hash(bar) == hash(Node(nt, ("foobar",)))
 
 
+def test_resolve_wildcards_labone_single_ok():
+    paths = ["test/hello/world", "test/hello/there", "test/hi/there"]
+    assert resolve_wildcards_labone("test/hello/world", paths) == ["test/hello/world"]
+
+
+def test_resolve_wildcards_labone_single_fail():
+    paths = ["test/hello/world", "test/hello/there", "test/hi/there"]
+    assert resolve_wildcards_labone("test/hello/a", paths) == []
+
+
+def test_resolve_wildcards_labone_wildcard_middle_ok():
+    paths = ["test/hello/world", "test/hello/there", "test/hi/there"]
+    assert resolve_wildcards_labone("test/*/there", paths) == [
+        "test/hello/there",
+        "test/hi/there",
+    ]
+
+
+def test_resolve_wildcards_labone_wildcard_middle_fail():
+    paths = ["test/hello/world", "test/hello/there", "test/hi/there"]
+    assert resolve_wildcards_labone("test/*/you", paths) == []
+
+
+def test_resolve_wildcards_labone_wildcard_partial_ok():
+    paths = ["test/hello/world", "test/hello/there", "test/hi/there"]
+    assert resolve_wildcards_labone("test", paths) == [
+        "test/hello/world",
+        "test/hello/there",
+        "test/hi/there",
+    ]
+
+
+def test_resolve_wildcards_labone_wildcard_partial_fail():
+    paths = ["test/hello/world", "test/hello/there", "test/hi/there"]
+    assert resolve_wildcards_labone("tes", paths) == []
+
+
+def test_resolve_wildcards_labone_wildcard_partial_subset():
+    paths = [
+        "/awgs/0/outputs/0/enables/0",
+        "/awgs/1/outputs/0/enables/0",
+        "/awgs/0/outputs/1/enables/0",
+        "/awgs/0/enable",
+        "/awgs/1/enable",
+    ]
+    assert resolve_wildcards_labone("/awgs/*/enable", paths) == [
+        "/awgs/0/enable",
+        "/awgs/1/enable",
+    ]
+
+
+def test_resolve_wildcards_labone_wildcard_end_ok():
+    paths = ["test/hello/world", "test/hello/there", "test/hi/there"]
+    assert resolve_wildcards_labone("test/hello/*", paths) == [
+        "test/hello/world",
+        "test/hello/there",
+    ]
+
+
+def test_resolve_wildcards_labone_wildcard_end_fail():
+    paths = ["test/hello/world", "test/hello/there", "test/hi/there"]
+    assert resolve_wildcards_labone("new/hello/*", paths) == []
+
+
+def test_garbage_collection_of_session(connection):
+
+    gc.collect()
+
+    def tester():
+        tree = NodeTree(connection, "DEV1234")
+        assert tree.demods[0].freq.is_valid()
+
+    tester()
+    gc.collect()
+    for obj in gc.get_objects():
+        assert not isinstance(obj, NodeTree)
+
+
+def test_garbage_collection_of_session_node_info(connection):
+
+    gc.collect()
+
+    def tester():
+        tree = NodeTree(connection, "DEV1234")
+        assert not tree.demods[0].freq.node_info.is_setting
+
+    tester()
+    gc.collect()
+    for obj in gc.get_objects():
+        assert not isinstance(obj, NodeTree)
+
+
+def test_node_info_caching(connection):
+    tree = NodeTree(connection, "DEV1234")
+    assert tree._node_infos == {}
+
+    assert not tree.demods[0].freq.node_info.is_setting
+
+    assert tree.demods[0].freq in tree._node_infos
+
+
 class TestWildCardResult:
     @pytest.fixture()
     def node_tree(self, connection):
         tree = NodeTree(connection, "DEV1234")
         connection.get.return_value = OrderedDict(
             [
                 (
```

### Comparing `zhinst-toolkit-0.5.3/tests/test_parsers.py` & `zhinst-toolkit-0.6.0/tests/test_parsers.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,9 +36,9 @@
     def test_multiple_of(self, caplog):
         assert Parse.multiple_of(10, 6, "nearest") == 12
         assert len(caplog.records) == 1
         assert Parse.multiple_of(10, 6, "down") == 6
         assert len(caplog.records) == 2
         assert Parse.multiple_of(12, 6, "down") == 12
         assert len(caplog.records) == 2
-        with pytest.raises(RuntimeError):
+        with pytest.raises(ValueError):
             Parse.multiple_of(100, 6, "up")
```

### Comparing `zhinst-toolkit-0.5.3/tests/test_pid_advisor_module.py` & `zhinst-toolkit-0.6.0/tests/test_pid_advisor_module.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/test_pqsc.py` & `zhinst-toolkit-0.6.0/tests/test_pqsc.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/test_precompensation_advisor_module.py` & `zhinst-toolkit-0.6.0/tests/test_precompensation_advisor_module.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/test_readout.py` & `zhinst-toolkit-0.6.0/tests/test_readout.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/test_scope_module.py` & `zhinst-toolkit-0.6.0/tests/test_scope_module.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/test_sequence.py` & `zhinst-toolkit-0.6.0/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/test_shfqa.py` & `zhinst-toolkit-0.6.0/tests/test_shfqa.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,20 +6,14 @@
 from zhinst.toolkit.driver.devices.shfqa import Generator, QAChannel, Readout, SHFScope
 
 
 def test_repr(shfqa):
     assert repr(shfqa) == "SHFQA(SHFQA4,DEV1234)"
 
 
-def test_factory_reset(shfqa):
-    # factory reset not yet implemented
-    with pytest.warns(RuntimeWarning) as record:
-        shfqa.factory_reset()
-
-
 def test_start_continuous_sw_trigger(mock_connection, shfqa):
     with patch("zhinst.toolkit.driver.devices.shfqa.utils", autospec=True) as utils:
         shfqa.start_continuous_sw_trigger(num_triggers=10, wait_time=20.0)
         utils.start_continuous_sw_trigger.assert_called_once_with(
             mock_connection.return_value, "DEV1234", num_triggers=10, wait_time=20.0
         )
```

### Comparing `zhinst-toolkit-0.5.3/tests/test_shfqa_scope.py` & `zhinst-toolkit-0.6.0/tests/test_shfqa_scope.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/test_shfqa_sweeper.py` & `zhinst-toolkit-0.6.0/tests/test_shfqa_sweeper.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/test_shfqc.py` & `zhinst-toolkit-0.6.0/tests/test_shfqc.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,20 +7,14 @@
 from zhinst.toolkit.driver.devices.shfsg import AWG, Node, SGChannel
 
 
 def test_repr(shfqc):
     assert repr(shfqc) == "SHFQC(SHFQC,DEV1234)"
 
 
-def test_factory_reset(shfqc):
-    # factory reset not yet implemented
-    with pytest.warns(RuntimeWarning) as record:
-        shfqc.factory_reset()
-
-
 def test_start_continuous_sw_trigger(mock_connection, shfqc):
     with patch("zhinst.toolkit.driver.devices.shfqa.utils", autospec=True) as utils:
         shfqc.start_continuous_sw_trigger(num_triggers=10, wait_time=20.0)
         utils.start_continuous_sw_trigger.assert_called_once_with(
             mock_connection.return_value, "DEV1234", num_triggers=10, wait_time=20.0
         )
```

### Comparing `zhinst-toolkit-0.5.3/tests/test_shfsg.py` & `zhinst-toolkit-0.6.0/tests/test_shfsg.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,14 @@
 
 
 def test_repr(shfsg):
     shfsg.sgchannels["*"].configure_channel()
     assert repr(shfsg) == "SHFSG(SHFSG8,DEV1234)"
 
 
-def test_factory_reset(shfsg):
-    # factory reset not yet implemented
-    with pytest.warns(RuntimeWarning) as record:
-        shfsg.factory_reset()
-
-
 def test_sgchannels(shfsg, mock_connection):
     assert len(shfsg.sgchannels) == 8
     assert isinstance(shfsg.sgchannels[0], SGChannel)
     # Wildcards nodes will be converted into normal Nodes
     assert not isinstance(shfsg.sgchannels["*"], SGChannel)
     assert isinstance(shfsg.sgchannels["*"], Node)
```

### Comparing `zhinst-toolkit-0.5.3/tests/test_spectroscopy.py` & `zhinst-toolkit-0.6.0/tests/test_spectroscopy.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/test_sweeper_module.py` & `zhinst-toolkit-0.6.0/tests/test_sweeper_module.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/test_uhfli.py` & `zhinst-toolkit-0.6.0/tests/test_uhfli.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/test_uhfqa.py` & `zhinst-toolkit-0.6.0/tests/test_uhfqa.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tests/test_waveforms.py` & `zhinst-toolkit-0.6.0/tests/test_waveforms.py`

 * *Files identical despite different names*

### Comparing `zhinst-toolkit-0.5.3/tox.ini` & `zhinst-toolkit-0.6.0/tox.ini`

 * *Files identical despite different names*

