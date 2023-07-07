# Comparing `tmp/edgepi-python-sdk-1.1.7.tar.gz` & `tmp/edgepi-python-sdk-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgepi-python-sdk-1.1.7.tar", last modified: Wed Dec 14 01:49:36 2022, max compression
+gzip compressed data, was "edgepi-python-sdk-1.2.1.tar", last modified: Fri Jul  7 00:25:38 2023, max compression
```

## Comparing `edgepi-python-sdk-1.1.7.tar` & `edgepi-python-sdk-1.2.1.tar`

### file list

```diff
@@ -1,125 +1,189 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:36.656289 edgepi-python-sdk-1.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2022-12-14 01:49:36.656289 edgepi-python-sdk-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-14 01:49:36.656289 edgepi-python-sdk-1.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      966 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:36.616288 edgepi-python-sdk-1.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:36.620288 edgepi-python-sdk-1.1.7/src/edgepi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:36.624288 edgepi-python-sdk-1.1.7/src/edgepi/adc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/adc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/adc/adc_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    13453 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/adc/adc_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8094 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/adc/adc_conv_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/adc/adc_crc_8_atm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/adc/adc_multiplexers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14421 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/adc/adc_query_lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/adc/adc_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/adc/adc_voltage.py
--rw-r--r--   0 runner    (1001) docker     (123)    38415 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/adc/edgepi_adc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:36.628288 edgepi-python-sdk-1.1.7/src/edgepi/calibration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/calibration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/calibration/calibration_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/calibration/edgepi_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     7386 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/calibration/edgepi_eeprom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/calibration/eeprom_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12701 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/calibration/eeprom_mapping_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:36.632288 edgepi-python-sdk-1.1.7/src/edgepi/dac/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/dac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6096 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/dac/dac_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/dac/dac_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9042 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/dac/edgepi_dac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:36.632288 edgepi-python-sdk-1.1.7/src/edgepi/digital_input/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/digital_input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/digital_input/edgepi_digital_input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:36.632288 edgepi-python-sdk-1.1.7/src/edgepi/digital_output/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/digital_output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/digital_output/edgepi_digital_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:36.632288 edgepi-python-sdk-1.1.7/src/edgepi/gpio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/gpio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/gpio/edgepi_gpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/gpio/edgepi_gpio_chip.py
--rw-r--r--   0 runner    (1001) docker     (123)     9253 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/gpio/edgepi_gpio_expander.py
--rw-r--r--   0 runner    (1001) docker     (123)    13625 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/gpio/gpio_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9309 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/gpio/gpio_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:36.636289 edgepi-python-sdk-1.1.7/src/edgepi/led/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/led/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/led/edgepi_leds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:36.636289 edgepi-python-sdk-1.1.7/src/edgepi/peripherals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/peripherals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/peripherals/gpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/peripherals/i2c.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/peripherals/spi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:36.636289 edgepi-python-sdk-1.1.7/src/edgepi/reg_helper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/reg_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8611 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/reg_helper/reg_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:36.640289 edgepi-python-sdk-1.1.7/src/edgepi/tc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/tc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18416 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/tc/edgepi_tc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11643 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/tc/tc_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    11369 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/tc/tc_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/tc/tc_conv_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/tc/tc_faults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:36.640289 edgepi-python-sdk-1.1.7/src/edgepi/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/edgepi/utilities/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:36.640289 edgepi-python-sdk-1.1.7/src/edgepi_python_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2022-12-14 01:49:36.000000 edgepi-python-sdk-1.1.7/src/edgepi_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2022-12-14 01:49:36.000000 edgepi-python-sdk-1.1.7/src/edgepi_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-14 01:49:36.000000 edgepi-python-sdk-1.1.7/src/edgepi_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2022-12-14 01:49:36.000000 edgepi-python-sdk-1.1.7/src/edgepi_python_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2022-12-14 01:49:36.000000 edgepi-python-sdk-1.1.7/src/edgepi_python_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:36.616288 edgepi-python-sdk-1.1.7/src/test_edgepi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:36.640289 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:36.644289 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_adc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_adc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_adc/test_adc_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    24211 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_adc/test_adc_conv_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_adc/test_adc_multiplexers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17668 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_adc/test_adc_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_adc/test_adc_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_adc/test_adc_voltage.py
--rw-r--r--   0 runner    (1001) docker     (123)    32211 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_adc/test_edgepi_adc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:36.648289 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_calibration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_calibration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_calibration/read_serialized.py
--rw-r--r--   0 runner    (1001) docker     (123)     5516 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_calibration/test_access_eeprom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_calibration/test_edgepi_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_calibration/test_eeprom_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:36.648289 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_dac/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_dac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7736 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_dac/test_dac_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    12009 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_dac/test_edgepi_dac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:36.648289 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_din/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_din/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_din/test_edgepi_din.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:36.648289 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_dout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_dout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4734 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_dout/test_edgepi_dout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:36.652289 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_gpio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_gpio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7405 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_gpio/test_edgepi_gpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     9169 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_gpio/test_edgepi_gpio_expander.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_gpio/test_edgpepi_gpio_chip.py
--rw-r--r--   0 runner    (1001) docker     (123)     7222 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_gpio/test_gpio_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_gpio/test_gpio_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:36.652289 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_peripherals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_peripherals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_peripherals/test_gpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5797 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_peripherals/test_i2c.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_peripherals/test_spi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:36.656289 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_reg_helper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_reg_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15302 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_reg_helper/test_reg_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:36.656289 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_tc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_tc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16845 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_tc/test_edgepi_tc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21079 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_tc/test_tc_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    39495 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_tc/test_tc_conv_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     6345 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_tc/test_tc_faults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:36.656289 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2022-12-14 01:49:16.000000 edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_utilities/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.701993 edgepi-python-sdk-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-07-07 00:25:38.701993 edgepi-python-sdk-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 00:25:38.701993 edgepi-python-sdk-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.677993 edgepi-python-sdk-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.681993 edgepi-python-sdk-1.2.1/src/edgepi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.681993 edgepi-python-sdk-1.2.1/src/edgepi/adc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/adc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/adc/adc_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14779 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/adc/adc_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/adc/adc_conv_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/adc/adc_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/adc/adc_multiplexers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/adc/adc_query_lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/adc/adc_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/adc/adc_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/adc/adc_voltage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38761 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/adc/edgepi_adc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.681993 edgepi-python-sdk-1.2.1/src/edgepi/calibration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/calibration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/calibration/calibration_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/calibration/edgepi_calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.681993 edgepi-python-sdk-1.2.1/src/edgepi/dac/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/dac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/dac/dac_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/dac/dac_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13470 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/dac/edgepi_dac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.681993 edgepi-python-sdk-1.2.1/src/edgepi/digital_input/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/digital_input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/digital_input/digital_input_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/digital_input/edgepi_digital_input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.685993 edgepi-python-sdk-1.2.1/src/edgepi/digital_output/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/digital_output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/digital_output/digital_output_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/digital_output/edgepi_digital_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.685993 edgepi-python-sdk-1.2.1/src/edgepi/eeprom/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/eeprom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16573 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/eeprom/edgepi_eeprom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/eeprom/edgepi_eeprom_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/eeprom/eeprom_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.685993 edgepi-python-sdk-1.2.1/src/edgepi/gpio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/gpio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/gpio/edgepi_gpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/gpio/edgepi_gpio_chip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/gpio/edgepi_gpio_expander.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16842 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/gpio/gpio_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/gpio/gpio_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.685993 edgepi-python-sdk-1.2.1/src/edgepi/led/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/led/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/led/edgepi_leds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/led/led_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.685993 edgepi-python-sdk-1.2.1/src/edgepi/peripherals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/peripherals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/peripherals/gpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/peripherals/i2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/peripherals/pwm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/peripherals/spi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.685993 edgepi-python-sdk-1.2.1/src/edgepi/pwm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/pwm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/pwm/edgepi_pwm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/pwm/pwm_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.685993 edgepi-python-sdk-1.2.1/src/edgepi/reg_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/reg_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/reg_helper/reg_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.685993 edgepi-python-sdk-1.2.1/src/edgepi/relay/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/relay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/relay/edgepi_relay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.689993 edgepi-python-sdk-1.2.1/src/edgepi/tc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/tc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21394 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/tc/edgepi_tc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11643 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/tc/tc_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12909 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/tc/tc_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/tc/tc_conv_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/tc/tc_faults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.689993 edgepi-python-sdk-1.2.1/src/edgepi/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/utilities/crc_8_atm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/edgepi/utilities/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.689993 edgepi-python-sdk-1.2.1/src/edgepi_python_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-07-07 00:25:38.000000 edgepi-python-sdk-1.2.1/src/edgepi_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-07-07 00:25:38.000000 edgepi-python-sdk-1.2.1/src/edgepi_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 00:25:38.000000 edgepi-python-sdk-1.2.1/src/edgepi_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-07 00:25:38.000000 edgepi-python-sdk-1.2.1/src/edgepi_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-07 00:25:38.000000 edgepi-python-sdk-1.2.1/src/edgepi_python_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.677993 edgepi-python-sdk-1.2.1/src/test_edgepi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.689993 edgepi-python-sdk-1.2.1/src/test_edgepi/integration_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/integration_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.689993 edgepi-python-sdk-1.2.1/src/test_edgepi/integration_tests/test_adc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/integration_tests/test_adc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21046 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/integration_tests/test_adc/test_adc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55717 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/integration_tests/test_adc/test_adc_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.689993 edgepi-python-sdk-1.2.1/src/test_edgepi/integration_tests/test_dac/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/integration_tests/test_dac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/integration_tests/test_dac/test_dac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.689993 edgepi-python-sdk-1.2.1/src/test_edgepi/integration_tests/test_digital_in/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/integration_tests/test_digital_in/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/integration_tests/test_digital_in/test_digital_in.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.689993 edgepi-python-sdk-1.2.1/src/test_edgepi/integration_tests/test_digital_out/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/integration_tests/test_digital_out/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/integration_tests/test_digital_out/test_digital_out.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.689993 edgepi-python-sdk-1.2.1/src/test_edgepi/integration_tests/test_eeprom/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/integration_tests/test_eeprom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/integration_tests/test_eeprom/test_eeprom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.689993 edgepi-python-sdk-1.2.1/src/test_edgepi/integration_tests/test_gpio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/integration_tests/test_gpio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/integration_tests/test_gpio/test_gpio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.693993 edgepi-python-sdk-1.2.1/src/test_edgepi/integration_tests/test_led/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/integration_tests/test_led/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/integration_tests/test_led/test_led.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.693993 edgepi-python-sdk-1.2.1/src/test_edgepi/integration_tests/test_peripherals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/integration_tests/test_peripherals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/integration_tests/test_peripherals/test_gpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/integration_tests/test_peripherals/test_i2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/integration_tests/test_peripherals/test_spi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.693993 edgepi-python-sdk-1.2.1/src/test_edgepi/integration_tests/test_pwm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/integration_tests/test_pwm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/integration_tests/test_pwm/test_edgepi_pwm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.693993 edgepi-python-sdk-1.2.1/src/test_edgepi/integration_tests/test_relay/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/integration_tests/test_relay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/integration_tests/test_relay/test_relay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.693993 edgepi-python-sdk-1.2.1/src/test_edgepi/integration_tests/test_tc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/integration_tests/test_tc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11257 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/integration_tests/test_tc/test_tc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.693993 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.693993 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_adc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_adc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_adc/test_adc_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24417 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_adc/test_adc_conv_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_adc/test_adc_multiplexers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29323 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_adc/test_adc_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_adc/test_adc_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_adc/test_adc_voltage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45764 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_adc/test_edgepi_adc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.693993 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_calibration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_calibration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_calibration/test_edgepi_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_calibration/test_protobuf_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.693993 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_dac/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_dac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9311 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_dac/test_dac_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19916 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_dac/test_edgepi_dac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.697993 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_din/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_din/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_din/test_edgepi_din.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.697993 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_dout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_dout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_dout/test_edgepi_dout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.697993 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_eeprom/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_eeprom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_eeprom/read_serialized.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14445 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_eeprom/test_access_eeprom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_eeprom/test_edgepi_eeprom_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.697993 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_gpio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_gpio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_gpio/test_edgepi_gpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9169 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_gpio/test_edgepi_gpio_expander.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_gpio/test_edgpepi_gpio_chip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_gpio/test_gpio_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_gpio/test_gpio_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.697993 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_peripherals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_peripherals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_peripherals/test_gpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_peripherals/test_i2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_peripherals/test_pwm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_peripherals/test_spi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.697993 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_pwm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_pwm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17768 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_pwm/test_edgepi_pwm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.697993 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_reg_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_reg_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15302 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_reg_helper/test_reg_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.697993 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_relay/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_relay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_relay/test_relay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.701993 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_tc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_tc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24741 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_tc/test_edgepi_tc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21079 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_tc/test_tc_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39495 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_tc/test_tc_conv_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_tc/test_tc_faults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:38.701993 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_utilities/test_crc_8_atm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-07 00:25:22.000000 edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_utilities/test_utilities.py
```

### Comparing `edgepi-python-sdk-1.1.7/LICENSE` & `edgepi-python-sdk-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.1.7/PKG-INFO` & `edgepi-python-sdk-1.2.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgepi-python-sdk
-Version: 1.1.7
+Version: 1.2.1
 Summary: EdgePi Python SDK package
 Home-page: https://github.com/EdgePi-Cloud/edgepi-python-sdk
 Author: S.Park
 Author-email: spark@osensa.com
 Project-URL: Bug Tracker, https://github.com/EdgePi-Cloud/edgepi-python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -30,56 +30,58 @@
 
 ```
 $ python3 -m pip install edgepi-python-sdk
 ```
 ## Example Code
 The EdgePi SDK provides a wide range of functionality to users, allowing interaction with the many modules onboard the EdgePi. One such module, the ADC, can be used to read voltage continuously from any of the eight EdgePi analog input pins:
 
-```
-from edgepi.adc.edgepi_adc import EdgePiADC
-from edgepi.adc.adc_constants import ADCChannel, ConvMode, ADCNum
+```python
+from edgepi.dac.edgepi_adc import EdgePiADC
+from edgepi.adc.adc_constants import ADCChannel, ConvMode
 
 # initialize ADC
 edgepi_adc = EdgePiADC()
 
-# configure ADC to sample analog input pin AIN3
+# configure ADC to sample input pin 4 (the input pins are 0-indexed)
 edgepi_adc.set_config(adc_1_analog_in=ADCChannel.AIN3, conversion_mode=ConvMode.CONTINUOUS)
 
-# send command to start continuous conversions
-edgepi_adc.start_conversions(ADCNum.ADC_1)
+# send command to start automatic conversions
+edgepi_adc.start_conversions()
 
 # perform 10 voltage reads
 for _ in range(10):
-  out = edgepi_adc.read_voltage(ADCNum.ADC_1)
+  out = edgepi_adc.read_voltage()
   print(out)
   
-# stop continuous conversions
-edgepi_adc.stop_conversions(ADCNum.ADC_1)
+# stop automatic conversions
+edgepi_adc.stop_conversions()
 ```
 For further details on this and other modules, please refer to each module's documentation by following the links provided in the `Implemented Modules` section below.
 # Implemented Modules
 The EdgePi SDK contains modules intended to represent each connected peripheral device onboard the EdgePi. Below is a directory of the currently available modules.
-* [Thermocouple](src/edgepi/tc)
-* [Digital to Analog Converter (DAC)](src/edgepi/dac)
-* [Analog to Digital Converter (ADC)](src/edgepi/adc)
-* [LED Array](src/edgepi/led)
-* [Digital In (DIN)](src/edgepi/din)
-* [Digital Out (DOUT)](src/edgepi/dout)
+* [Thermocouple](https://github.com/EdgePi-Cloud/edgepi-python-sdk/tree/main/src/edgepi/tc)
+* [Digital to Analog Converter (DAC)](https://github.com/EdgePi-Cloud/edgepi-python-sdk/tree/main/src/edgepi/dac)
+* [Analog to Digital Converter (ADC)](https://github.com/EdgePi-Cloud/edgepi-python-sdk/tree/main/src/edgepi/adc)
+* [LED Array](https://github.com/EdgePi-Cloud/edgepi-python-sdk/tree/main/src/edgepi/led)
+* [Digital Input (DIN)](https://github.com/EdgePi-Cloud/edgepi-python-sdk/tree/main/src/edgepi/digital_input)
+* [Digital Output (DOUT)](https://github.com/EdgePi-Cloud/edgepi-python-sdk/tree/main/src/edgepi/digital_output)
 # Development
 Active development SDK versions can be accessed from the following resources:
 ## Installing from TestPyPi
 To install the most recent active development SDK version via [TestPyPi](https://test.pypi.org/project/edgepi-python-sdk/):
 ```
-$ python3 -m pip install -i https://test.pypi.org/simple/ edgepi-python-sdk
+
+$ python3 -m pip install -i https://test.pypi.org/simple/edgepi-python-sdk
 ```
 Previous development SDK versions can also be installed by specifiying the version number:
 ```
-$ python3 -m pip install -i https://test.pypi.org/simple/ edgepi-python-sdk==<version-number>
+$ python3 -m pip install -i https://test.pypi.org/simple/edgepi-python-sdk==<version-number>
 ```
 Please refer to [TestPyPi](https://test.pypi.org/project/edgepi-python-sdk/) for available SDK versions.
+
 ## Installing from GitHub
 To install the SDK via HTTPS from GitHub:
 ```
 $ python3 -m pip install git+https://github.com/EdgePi-Cloud/edgepi-python-sdk.git@<branch-name>
 ```
 
 # Packaging
```

### Comparing `edgepi-python-sdk-1.1.7/README.md` & `edgepi-python-sdk-1.2.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -15,56 +15,58 @@
 
 ```
 $ python3 -m pip install edgepi-python-sdk
 ```
 ## Example Code
 The EdgePi SDK provides a wide range of functionality to users, allowing interaction with the many modules onboard the EdgePi. One such module, the ADC, can be used to read voltage continuously from any of the eight EdgePi analog input pins:
 
-```
-from edgepi.adc.edgepi_adc import EdgePiADC
-from edgepi.adc.adc_constants import ADCChannel, ConvMode, ADCNum
+```python
+from edgepi.dac.edgepi_adc import EdgePiADC
+from edgepi.adc.adc_constants import ADCChannel, ConvMode
 
 # initialize ADC
 edgepi_adc = EdgePiADC()
 
-# configure ADC to sample analog input pin AIN3
+# configure ADC to sample input pin 4 (the input pins are 0-indexed)
 edgepi_adc.set_config(adc_1_analog_in=ADCChannel.AIN3, conversion_mode=ConvMode.CONTINUOUS)
 
-# send command to start continuous conversions
-edgepi_adc.start_conversions(ADCNum.ADC_1)
+# send command to start automatic conversions
+edgepi_adc.start_conversions()
 
 # perform 10 voltage reads
 for _ in range(10):
-  out = edgepi_adc.read_voltage(ADCNum.ADC_1)
+  out = edgepi_adc.read_voltage()
   print(out)
   
-# stop continuous conversions
-edgepi_adc.stop_conversions(ADCNum.ADC_1)
+# stop automatic conversions
+edgepi_adc.stop_conversions()
 ```
 For further details on this and other modules, please refer to each module's documentation by following the links provided in the `Implemented Modules` section below.
 # Implemented Modules
 The EdgePi SDK contains modules intended to represent each connected peripheral device onboard the EdgePi. Below is a directory of the currently available modules.
-* [Thermocouple](src/edgepi/tc)
-* [Digital to Analog Converter (DAC)](src/edgepi/dac)
-* [Analog to Digital Converter (ADC)](src/edgepi/adc)
-* [LED Array](src/edgepi/led)
-* [Digital In (DIN)](src/edgepi/din)
-* [Digital Out (DOUT)](src/edgepi/dout)
+* [Thermocouple](https://github.com/EdgePi-Cloud/edgepi-python-sdk/tree/main/src/edgepi/tc)
+* [Digital to Analog Converter (DAC)](https://github.com/EdgePi-Cloud/edgepi-python-sdk/tree/main/src/edgepi/dac)
+* [Analog to Digital Converter (ADC)](https://github.com/EdgePi-Cloud/edgepi-python-sdk/tree/main/src/edgepi/adc)
+* [LED Array](https://github.com/EdgePi-Cloud/edgepi-python-sdk/tree/main/src/edgepi/led)
+* [Digital Input (DIN)](https://github.com/EdgePi-Cloud/edgepi-python-sdk/tree/main/src/edgepi/digital_input)
+* [Digital Output (DOUT)](https://github.com/EdgePi-Cloud/edgepi-python-sdk/tree/main/src/edgepi/digital_output)
 # Development
 Active development SDK versions can be accessed from the following resources:
 ## Installing from TestPyPi
 To install the most recent active development SDK version via [TestPyPi](https://test.pypi.org/project/edgepi-python-sdk/):
 ```
-$ python3 -m pip install -i https://test.pypi.org/simple/ edgepi-python-sdk
+
+$ python3 -m pip install -i https://test.pypi.org/simple/edgepi-python-sdk
 ```
 Previous development SDK versions can also be installed by specifiying the version number:
 ```
-$ python3 -m pip install -i https://test.pypi.org/simple/ edgepi-python-sdk==<version-number>
+$ python3 -m pip install -i https://test.pypi.org/simple/edgepi-python-sdk==<version-number>
 ```
 Please refer to [TestPyPi](https://test.pypi.org/project/edgepi-python-sdk/) for available SDK versions.
+
 ## Installing from GitHub
 To install the SDK via HTTPS from GitHub:
 ```
 $ python3 -m pip install git+https://github.com/EdgePi-Cloud/edgepi-python-sdk.git@<branch-name>
 ```
 
 # Packaging
```

### Comparing `edgepi-python-sdk-1.1.7/setup.py` & `edgepi-python-sdk-1.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as file:
     long_description = file.read()
 
 setuptools.setup(
     name="edgepi-python-sdk",
-    version="1.1.7",
+    version="1.2.1",
     author="S.Park",
     author_email="spark@osensa.com",
     description="EdgePi Python SDK package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/EdgePi-Cloud/edgepi-python-sdk",
     project_urls={
@@ -21,9 +21,9 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     packages=setuptools.find_packages(where="src", exclude=["test_edgepi"]),
     package_dir={"": "src"},
     python_requires=">=3.6",
-    install_requires=["python-periphery >= 2.3.0", "bitstring >= 3.1.9", "protobuf==3.20.*"],
+    install_requires=["python-periphery >= 2.3.0", "bitstring >= 3.1.9", "protobuf>=3.20"],
 )
```

### Comparing `edgepi-python-sdk-1.1.7/src/edgepi/adc/adc_commands.py` & `edgepi-python-sdk-1.2.1/src/edgepi/adc/adc_commands.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,24 +16,22 @@
     def __init__(self):
         _logger.info("Initializing ADC Methods")
 
     def read_register_command(self, address: int, num: int):
         """Trigger ADC register read"""
         self.check_for_int([address, num])
         command = [ADCComs.COM_RREG.value + address, num - 1]
-        _logger.debug("RREG command to send is %s", (command + [255] * num))
         return command + [255] * num
 
     def write_register_command(self, address, values):
         """Trigger ADC register write"""
         self.check_for_int([address])
         all(self.check_range(value, 0, 255) for value in values)
         self.check_for_int(values)
         command = [ADCComs.COM_WREG.value + address, len(values) - 1]
-        _logger.debug("WREG Command to send is %s", (command + values))
         return command + values
 
     def start_adc(self, adc_num: ADCNum):
         """Command to start ADC"""
         _logger.debug("Command to send is %s", ([adc_num.start_cmd]))
         return [adc_num.start_cmd]
```

### Comparing `edgepi-python-sdk-1.1.7/src/edgepi/adc/adc_constants.py` & `edgepi-python-sdk-1.2.1/src/edgepi/adc/adc_constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,14 +61,28 @@
     REG_ADC2CFG = 0x15
     REG_ADC2MUX = 0x16
     REG_ADC2OFC0 = 0x17
     REG_ADC2OFC1 = 0x18
     REG_ADC2FSC0 = 0x19
     REG_ADC2FSC1 = 0x1A
 
+@unique
+class AnalogIn(Enum):
+    """EdgePi Analog Input Number"""
+
+    AIN1 = 0
+    AIN2 = 1
+    AIN3 = 2
+    AIN4 = 3
+    AIN5 = 4
+    AIN6 = 5
+    AIN7 = 6
+    AIN8 = 7
+    AINCOM = 10
+    FLOAT = 0xF
 
 @unique
 class ADCChannel(Enum):
     """EdgePi ADC channels/channel modes"""
 
     AIN0 = 0
     AIN1 = 1
@@ -309,48 +323,76 @@
     POS_REF_INT_VAVDD = OpCode(0x20, ADCReg.REG_REFMUX.value, ADCMasks.RMUXP_BITS.value)
     NEG_REF_INT_2P5 = OpCode(0x0, ADCReg.REG_REFMUX.value, ADCMasks.RMUXN_BITS.value)
     NEG_REF_EXT_AIN1 = OpCode(0x1, ADCReg.REG_REFMUX.value, ADCMasks.RMUXN_BITS.value)
     NEG_REF_EXT_AIN3 = OpCode(0x2, ADCReg.REG_REFMUX.value, ADCMasks.RMUXN_BITS.value)
     NEG_REF_EXT_AIN5 = OpCode(0x3, ADCReg.REG_REFMUX.value, ADCMasks.RMUXN_BITS.value)
     NEG_REF_INT_VAVSS = OpCode(0x4, ADCReg.REG_REFMUX.value, ADCMasks.RMUXN_BITS.value)
 
+class ADC2REFMUX(Enum):
+    """Settings for ADC2 REFMUX register (ADC2 Configuration register 5:3 bits)"""
+    INTERNAL_2P5 = OpCode(0x00, ADCReg.REG_ADC2CFG.value, ADCMasks.RMUXP_BITS.value)
+    AIN0_AIN1 = OpCode(0x08, ADCReg.REG_ADC2CFG.value, ADCMasks.RMUXP_BITS.value)
+    AIN2_AIN3 = OpCode(0x10, ADCReg.REG_ADC2CFG.value, ADCMasks.RMUXP_BITS.value)
+    AIN4_AIN5 = OpCode(0x18, ADCReg.REG_ADC2CFG.value, ADCMasks.RMUXP_BITS.value )
+    INT_VAVDD_VAVSS = OpCode(0x20, ADCReg.REG_ADC2CFG.value, ADCMasks.RMUXP_BITS.value )
 
 class RTDModes(Enum):
     "ADC.__config args for for turning RTD mode on/off"
     RTD_ON = {
-        "adc_1_analog_in": ADCChannel.AIN5,
-        "adc_1_mux_n": ADCChannel.AIN6,
         "idac_1_mux": IDACMUX.IDAC1_AIN8,
         "idac_2_mux": IDACMUX.IDAC2_AIN9,
         "idac_1_mag": IDACMAG.IDAC1_500,
         "idac_2_mag": IDACMAG.IDAC2_500,
-        "pos_ref_inp": REFMUX.POS_REF_EXT_AIN4,
-        "neg_ref_inp": REFMUX.NEG_REF_INT_VAVSS,
     }
     RTD_OFF = {
-        "adc_1_analog_in": ADCChannel.FLOAT,
-        "adc_1_mux_n": ADCChannel.AINCOM,
         "idac_1_mux": IDACMUX.IDAC1_NO_CONNECT,
         "idac_2_mux": IDACMUX.IDAC2_NO_CONNECT,
         "idac_1_mag": IDACMAG.IDAC1_OFF,
         "idac_2_mag": IDACMAG.IDAC2_OFF,
         "pos_ref_inp": REFMUX.POS_REF_INT_2P5,
         "neg_ref_inp": REFMUX.NEG_REF_INT_2P5,
+        "adc2_ref_inp": ADC2REFMUX.INTERNAL_2P5,
     }
 
+class ADC1RtdConfig(Enum):
+    "ADC1.__config args for for turning RTD mode on/off"
+    ON = {
+        "adc_1_ch": ADCChannel.AIN7,
+        "adc_1_mux_n": ADCChannel.AIN6,
+        "pos_ref_inp": REFMUX.POS_REF_EXT_AIN4,
+        "neg_ref_inp": REFMUX.NEG_REF_EXT_AIN5,
+    }
+    OFF = {
+        "adc_1_ch": ADCChannel.FLOAT,
+        "adc_1_mux_n": ADCChannel.AINCOM,
+        "pos_ref_inp": REFMUX.POS_REF_INT_2P5,
+        "neg_ref_inp": REFMUX.NEG_REF_INT_2P5,
+    }
+
+class ADC2RtdConfig(Enum):
+    "ADC2.__config args for for turning RTD mode on/off"
+    ON = {
+        "adc_2_ch": ADCChannel.AIN7,
+        "adc_2_mux_n": ADCChannel.AIN6,
+        "adc2_ref_inp": ADC2REFMUX.AIN4_AIN5,
+    }
+    OFF = {
+        "adc_2_ch": ADCChannel.FLOAT,
+        "adc_2_mux_n": ADCChannel.AINCOM,
+        "adc2_ref_inp": ADC2REFMUX.INTERNAL_2P5,
+    }
 
 class AllowedChannels(Enum):
     """Available channels for reading depend on whether RTD is enabled or not"""
 
     RTD_ON = [
         ADCChannel.AIN0,
         ADCChannel.AIN1,
         ADCChannel.AIN2,
         ADCChannel.AIN3,
-        ADCChannel.AIN7,
         ADCChannel.AINCOM,
         ADCChannel.FLOAT,
     ]
     RTD_OFF = [
         ADCChannel.AIN0,
         ADCChannel.AIN1,
         ADCChannel.AIN2,
```

### Comparing `edgepi-python-sdk-1.1.7/src/edgepi/adc/adc_conv_time.py` & `edgepi-python-sdk-1.2.1/src/edgepi/adc/adc_conv_time.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,22 +179,29 @@
     ],
     DR1.SPS_38400.value.op_code: ADC1_INITIAL_DELAYS[DR1.SPS_38400.value.op_code][
         FILT.SINC1.value.op_code
     ],
 }
 
 
-# continuous conversion delay times for ADC2 (ADC2 only uses continuous mode)
-ADC2_DELAYS = {
+# initial conversion delay times for ADC2 (ADC2 only uses initial mode)
+ADC2_INITIAL_DELAYS = {
     DR2.SPS_10.value.op_code: 121,
     DR2.SPS_100.value.op_code: 31.2,
     DR2.SPS_400.value.op_code: 8.71,
     DR2.SPS_800.value.op_code: 4.97,
 }
 
+ADC2_CONT_DELAYS = {
+    DR2.SPS_10.value.op_code: 100,
+    DR2.SPS_100.value.op_code: 10,
+    DR2.SPS_400.value.op_code: 2.5,
+    DR2.SPS_800.value.op_code: 1.25,
+}
+
 
 def expected_initial_time_delay(adc_num: ADCNum, data_rate: int, filter_mode: int):
     """
     Computes conversion latency (ms) based on ADC configuration
     for PULSE mode reads or initial read in CONTINUOUS mode.
 
     Args:
@@ -209,15 +216,16 @@
     """
     if adc_num == ADCNum.ADC_1:
         # this is the initial delay for both pulse and continuous modes
         return ADC1_INITIAL_DELAYS[data_rate][filter_mode]
 
     # no initial figures given in documentation, but estimate initial delay
     # is 3 times longer than subsequent conversion delays
-    return ADC2_DELAYS[data_rate] * 3
+    return ADC2_INITIAL_DELAYS[data_rate]
+
 
 
 def expected_continuous_time_delay(adc_num: ADCNum, data_rate: int):
     """
     Computes conversion latency (ms) based on ADC configuration
     for reads 2...n in continuous conversion mode.
 
@@ -228,8 +236,8 @@
 
     Returns:
         `float`: conversion delay in milliseconds (ms)
     """
     if adc_num == ADCNum.ADC_1:
         return ADC1_CONT_DELAYS[data_rate]
 
-    return ADC2_DELAYS[data_rate]
+    return ADC2_CONT_DELAYS[data_rate]
```

### Comparing `edgepi-python-sdk-1.1.7/src/edgepi/adc/adc_multiplexers.py` & `edgepi-python-sdk-1.2.1/src/edgepi/adc/adc_multiplexers.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         Note: both of the above must be dictionaries formatted as:
 
             mux_reg_addx (ADCReg): (mux_p_val, mux_n_val)
 
     Returns:
         `list`: OpCodes for updated multiplexer mapping
     """
-    _logger.debug(f"mux updates = {mux_updates}")
+    _logger.debug(f"generate_mux_opcodes: mux updates = {mux_updates}")
 
     mux_opcodes = []
     # generate OpCodes for mux updates
     for addx, byte in mux_updates.items():
         mux_p = byte[0]
         mux_n = byte[1]
```

### Comparing `edgepi-python-sdk-1.1.7/src/edgepi/adc/adc_query_lang.py` & `edgepi-python-sdk-1.2.1/src/edgepi/adc/adc_query_lang.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import Any
 from enum import Enum
 
 from edgepi.adc.adc_constants import (
     IDACMAG,
     IDACMUX,
     REFMUX,
+    ADC2REFMUX,
     ADC1DataRate,
     ADC2DataRate,
     ADCChannel,
     ADCMasks,
     ADCReg,
     CheckMode,
     ConvMode,
@@ -325,7 +326,26 @@
                 "channel 5 external", REFMUX.NEG_REF_EXT_AIN5
             ),
             REFMUX.NEG_REF_INT_VAVSS.value.op_code: PropertyValue(
                 "VAVSS", REFMUX.NEG_REF_INT_VAVSS
             ),
         },
     )
+    ADC2_REFMUX = Property(
+        "adc-2-ref-mux",
+        ADCReg.REG_ADC2CFG.value,
+        ADCMasks.RMUXP_BITS.value,
+        {
+            ADC2REFMUX.INTERNAL_2P5.value.op_code: PropertyValue(
+                "2.5 V internal", ADC2REFMUX.INTERNAL_2P5
+            ),
+            ADC2REFMUX.AIN0_AIN1.value.op_code: PropertyValue(
+                "Channel 0 and 1 pair", ADC2REFMUX.AIN0_AIN1
+                ),
+            ADC2REFMUX.AIN2_AIN3.value.op_code: PropertyValue(
+                "Channel 2 and 3 pair", ADC2REFMUX.AIN2_AIN3
+                ),
+            ADC2REFMUX.AIN4_AIN5.value.op_code: PropertyValue(
+                "Channel 4 and 5 pair", ADC2REFMUX.AIN4_AIN5
+                ),
+        },
+    )
```

### Comparing `edgepi-python-sdk-1.1.7/src/edgepi/adc/adc_status.py` & `edgepi-python-sdk-1.2.1/src/edgepi/adc/adc_status.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.1.7/src/edgepi/adc/adc_voltage.py` & `edgepi-python-sdk-1.2.1/src/edgepi/adc/adc_voltage.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """ADC voltage reading configuration and utility methods"""
 
 
 import logging
 
 from bitstring import BitArray
-from edgepi.adc.adc_constants import ADCReadInfo
+from edgepi.adc.adc_constants import ADCReadInfo, ADCNum
 from edgepi.calibration.calibration_constants import CalibParam
 from edgepi.utilities.utilities import bitstring_from_list
-from edgepi.adc.adc_crc_8_atm import CRC_8_ATM_LUT
 
 
 # TODO: retrieve these values from EEPROM once added
 STEP_DOWN_RESISTOR_1 = 19.1
 STEP_DOWN_RESISTOR_2 = 4.99
 REFERENCE_VOLTAGE = 2.5
 
@@ -36,24 +35,25 @@
         `code` (int): uint value of ADC voltage read bytes
 
         `v_ref` (float): ADC reference voltage in Volts
 
         `num_bits` (int): number of bits in ADC voltage read (24 or 32)
     """
     voltage_range = v_ref / 2 ** (num_bits - 1)
+    _logger.debug(f" _code_to_input_voltage: code {code}")
     return float(code) * voltage_range
 
 
 def _adc_voltage_to_input_voltage(v_in: float, gain: float, offset: float):
     """
     Converts ADC input voltage (i.e. voltage measured at ADC) to
     ADC output voltage (i.e. voltage measured at terminal block)
     """
     step_up_ratio = (STEP_DOWN_RESISTOR_1 + STEP_DOWN_RESISTOR_2) / STEP_DOWN_RESISTOR_2
-    return v_in * step_up_ratio * gain - offset
+    return v_in * step_up_ratio * gain + offset
 
 
 def code_to_voltage(code: list[int], adc_info: ADCReadInfo, calibs: CalibParam) -> float:
     """
     Converts ADC voltage read digital code to output voltage (voltage measured at terminal block)
 
     Args:
@@ -62,33 +62,60 @@
         `adc_info` (ADCReadInfo): data about this adc's voltage reading configuration
 
         `calibs` (CalibParam): voltage reading gain and offset calibration values
 
     Returns:
         `float`: voltage value (V) corresponding to `code`
     """
-    code_bits = bitstring_from_list(code)
+    code_bits = bitstring_from_list(code[:adc_info.num_data_bytes])
     num_bits = adc_info.num_data_bytes * 8
-
-    # code is given in 2's complement, remove leading 1
+    code_val = code_bits.uint
+    # handling negative number
     if _is_negative_voltage(code_bits):
-        code_bits[0] = 0
+        code_val = code_val - 2**num_bits
 
-    v_in = _code_to_input_voltage(code_bits.uint, REFERENCE_VOLTAGE, num_bits)
+    v_in = _code_to_input_voltage(code_val, REFERENCE_VOLTAGE, num_bits)
 
     v_out = _adc_voltage_to_input_voltage(v_in, calibs.gain, calibs.offset)
 
     return v_out
 
+def code_to_voltage_single_ended(code: list[int], adc_info: ADCReadInfo, calibs: CalibParam):
+    """
+    Converts ADC voltage read digital code to output voltage (voltage measured at terminal block)
+
+    Args:
+        `code` (list[int]): code bytes retrieved from ADC voltage read
+
+        `adc_info` (ADCReadInfo): data about this adc's voltage reading configuration
+
+        `calibs` (CalibParam): voltage reading gain and offset calibration values
+
+    Returns:
+        `float`: voltage value (V) corresponding to `code`
+    """
+    code_bits = bitstring_from_list(code[:adc_info.num_data_bytes])
+    num_bits = adc_info.num_data_bytes * 8
+    code_val = code_bits.uint
+    # handling negative number
+    if _is_negative_voltage(code_bits):
+        code_val = code_val - 2**num_bits
+
+    v_in = _code_to_input_voltage(code_val, REFERENCE_VOLTAGE, num_bits)
+    v_in = REFERENCE_VOLTAGE + v_in
+    v_out = _adc_voltage_to_input_voltage(v_in, calibs.gain, calibs.offset)
+
+    return v_out
 
 def code_to_temperature(
     code: list[int],
     ref_resistance: float,
     rtd_sensor_resistance: float,
-    rtd_sensor_resistance_variation: float
+    rtd_sensor_resistance_variation: float,
+    adc_num: ADCNum
     ) -> float:
     """
     Converts ADC voltage read digital code to temperature. Intended for use in RTD sampling.
 
     Args:
         `code` (list[int]): code bytes retrieved from ADC voltage read
 
@@ -99,82 +126,15 @@
        `rtd_sensor_resistance_variation` (float): RTD model-dependent resistance variation (Ohms/°C)
 
     Returns:
         `float`: temperature value (°C) corresponding to `code`
     """
     code_bits = bitstring_from_list(code)
 
-    # refer to https://github.com/osensa/edgepi-python-sdk/issues/159 for computation details
-    r_rtd = code_bits.uint / (2 ** 30) * ref_resistance
-
+    # refer to Three-Wire RTD Measurement, Low-Side Reference
+    # https://www.ti.com/lit/an/sbaa275a/sbaa275a.pdf?ts=1683111690519&ref_url=https%253A%252F%252Fduckduckgo.com%252F
+    number_of_bits = 30 if adc_num == ADCNum.ADC_1 else 22
+    r_rtd = code_bits.uint / (2 ** number_of_bits) * ref_resistance
     temperature = (r_rtd - rtd_sensor_resistance) / rtd_sensor_resistance_variation
     _logger.debug(f"computed rtd temperature = {temperature}, from code = {code_bits.uint}")
 
     return temperature
-
-
-class CRCCheckError(Exception):
-    """Raised if CRC check fails to match CRC code generated by ADS1263"""
-
-
-# use this with `generate_crc_8_table` below to get LUT for CRC-8-ATM polynomial
-CRC_8_ATM_GEN = 0x07
-
-
-def generate_crc_8_table(crc_polynomial: int):
-    """
-    Generates LUT containing CRC-8 values for all possible byte (8 bit) values, i.e.
-    every entry is the CRC-8 value for the ith byte value from 0,...,255.
-
-    Adapted from:
-    https://github.com/osensa/rtu-adc/blob/6fac17efb955c2e8bb40740dd46e48ae51e1d5ff/crc8atm.py
-
-    Args:
-        `crc_polynomial`: the CRC-8 polynomial used to generate this LUT
-
-    Returns:
-        `list`: the LUT corresponding to this CRC-8 polynomial
-    """
-    table = list(range(256))
-
-    # for every byte value from 0 to 255
-    for index, crc in enumerate(table):
-        for _ in range(8):
-            # scan bitwise through byte to align leading 1 with CRC polynomial
-            # perform divison (XOR) operation once aligned
-            crc = (crc << 1) ^ (crc_polynomial if (crc & 0x80) else 0)
-
-        # store only low byte of computed value to account for left shifting
-        table[index] = crc & 0xFF
-
-    return table
-
-
-def check_crc(voltage_bytes: list, crc_code: int):
-    """
-    Performs CRC-8 check on a list of data bytes. By default uses
-    CRC-8-ATM polynomial table
-
-    Adapted from:
-    https://github.com/osensa/rtu-adc/blob/6fac17efb955c2e8bb40740dd46e48ae51e1d5ff/crc8atm.py
-
-    Args:
-        `data_bytes` (list): a list of bytes ordered as
-            [data_1, data_2,..., data_n, crc_8]
-
-        `crc_table`: a previously generated LUT for the CRC-8-ATM
-            polynomial
-    """
-    crc = 0
-
-    data_bytes = voltage_bytes + [crc_code]
-
-    # compute CRC value of data bytes byte wise using LUT
-    # which holds CRC values for all possible byte values
-    for byte in data_bytes:
-        index = crc ^ byte
-        crc = CRC_8_ATM_LUT[index]
-
-    if crc != 0:
-        raise CRCCheckError(
-            f"CRC check failed with codes: computed={hex(crc)}, expected={hex(crc_code)}"
-        )
```

### Comparing `edgepi-python-sdk-1.1.7/src/edgepi/adc/edgepi_adc.py` & `edgepi-python-sdk-1.2.1/src/edgepi/adc/edgepi_adc.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,186 +1,73 @@
 """ User interface for EdgePi ADC """
 
-
-from dataclasses import dataclass
 from enum import Enum
 from operator import attrgetter
 import logging
 import time
 
-
-from bitstring import pack
-from edgepi.adc.adc_query_lang import PropertyValue, ADCProperties
+from edgepi.adc.adc_query_lang import PropertyValue
 from edgepi.calibration.calibration_constants import CalibParam
 from edgepi.peripherals.spi import SpiDevice as SPI
 from edgepi.adc.adc_commands import ADCCommands
 from edgepi.adc.adc_constants import (
     ADC1DataRate,
     ADC2DataRate,
     ADCChannel as CH,
-    ADCComs,
     ADCNum,
     ADCPower,
     ConvMode,
     ADCReg,
     DifferentialPair,
     FilterMode,
     ADCReferenceSwitching,
     ADC_NUM_REGS,
     ADC_VOLTAGE_READ_LEN,
     CheckMode,
     DiffMode,
     IDACMUX,
     IDACMAG,
     REFMUX,
+    ADC2REFMUX,
     RTDModes,
+    ADC1RtdConfig,
+    ADC2RtdConfig,
     AllowedChannels,
+    AnalogIn,
 )
-from edgepi.adc.adc_voltage import code_to_voltage, check_crc, code_to_temperature
+from edgepi.adc.adc_voltage import (
+    code_to_voltage,
+    code_to_temperature,
+    code_to_voltage_single_ended
+)
+from edgepi.utilities.crc_8_atm import check_crc
 from edgepi.gpio.edgepi_gpio import EdgePiGPIO
-from edgepi.gpio.gpio_configs import ADCPins
-from edgepi.utilities.utilities import filter_dict
+from edgepi.gpio.gpio_configs import ADCPins, RTDPins
+from edgepi.utilities.utilities import filter_dict, filter_dict_list_key_val
 from edgepi.reg_helper.reg_helper import OpCode, apply_opcodes
 from edgepi.adc.adc_multiplexers import (
     generate_mux_opcodes,
     validate_channels_allowed,
 )
 from edgepi.adc.adc_conv_time import expected_initial_time_delay, expected_continuous_time_delay
 from edgepi.adc.adc_status import get_adc_status
-from edgepi.calibration.edgepi_eeprom import EdgePiEEPROM
+from edgepi.eeprom.edgepi_eeprom import EdgePiEEPROM
+from edgepi.adc.adc_state import ADCState
+from edgepi.adc.adc_exceptions import (
+    ADCRegisterUpdateError,
+    VoltageReadError,
+    ContinuousModeError,
+    RTDEnabledError,
+    InvalidDifferentialPairError,
+    CalibKeyMissingError
+)
 
 _logger = logging.getLogger(__name__)
 
 
-@dataclass
-class ADCReadFields:
-    """
-    ADC state properties specific to each of ADC1 and ADC2
-    """
-
-    conversion_mode: PropertyValue
-    data_rate: PropertyValue
-    mux_p: PropertyValue
-    mux_n: PropertyValue
-
-
-class ADCState:
-    """ADC state intended for reading by users"""
-
-    def __init__(self, reg_map: dict):
-        self.__reg_map = reg_map
-        self.adc_1: ADCReadFields = ADCReadFields(
-            self.__get_state(ADCProperties.CONV_MODE),
-            self.__get_state(ADCProperties.DATA_RATE_1),
-            self.__get_state(ADCProperties.ADC1_MUXP),
-            self.__get_state(ADCProperties.ADC1_MUXN),
-        )
-        self.adc_2: ADCReadFields = ADCReadFields(
-            PropertyValue("continuous", ADCProperties.CONV_MODE),
-            self.__get_state(ADCProperties.DATA_RATE_2),
-            self.__get_state(ADCProperties.ADC2_MUXP),
-            self.__get_state(ADCProperties.ADC2_MUXN),
-        )
-        self.filter_mode: PropertyValue = self.__get_state(ADCProperties.FILTER_MODE)
-        self.status_byte: PropertyValue = self.__get_state(ADCProperties.STATUS_MODE)
-        self.checksum_mode: PropertyValue = self.__get_state(ADCProperties.CHECK_MODE)
-        self.rtd_on: bool = self.__get_rtd_state()
-
-    def __query_state(self, adc_property: ADCProperties) -> PropertyValue:
-        """
-        Read the current state of configurable ADC properties
-
-        Args:
-            `adc_property` (ADCProperties): ADC property whose state is to be read
-            `reg_map`: register map formatted as {addx (int): value (int)}
-
-        Returns:
-            `PropertyValue`: information about the current value of this property
-        """
-        # value of this adc_property's register
-        reg_value = self.__reg_map[adc_property.value.addx]
-
-        # get value of bits corresponding to this property by letting through only the bits
-        # that were "masked" when setting this property (clear all bits except the property bits)
-        adc_property_bits = (~adc_property.value.mask) & reg_value
-
-        # name of current value of this adc_property
-        adc_property_value = adc_property.value.values[adc_property_bits]
-        _logger.debug(
-            (
-                f"query_state: query_property='{adc_property}',"
-                " adc_property_bits={hex(adc_property_bits)},"
-                f" adc_property_value='{adc_property_value}'"
-            )
-        )
-
-        return adc_property_value
-
-    def __get_state(self, adc_property: ADCProperties) -> PropertyValue:
-        """
-        Read the current state of configurable ADC properties
-
-        Args:
-            `adc_property` (ADCProperties): ADC property whose state is to be read
-
-        Returns:
-            `PropertyValue`: information about the current value of this mode
-        """
-        return self.__query_state(adc_property)
-
-    def __get_current_rtd_state(self) -> dict[str, PropertyValue]:
-        return {
-            "adc_1_analog_in": self.adc_1.mux_p.code,
-            "adc_1_mux_n": self.adc_1.mux_n.code,
-            "idac_1_mux": self.__get_state(ADCProperties.IDAC1_MUX).code,
-            "idac_2_mux": self.__get_state(ADCProperties.IDAC2_MUX).code,
-            "idac_1_mag": self.__get_state(ADCProperties.IDAC1_MAG).code,
-            "idac_2_mag": self.__get_state(ADCProperties.IDAC2_MAG).code,
-            "pos_ref_inp": self.__get_state(ADCProperties.REFMUX_POS).code,
-            "neg_ref_inp": self.__get_state(ADCProperties.REFMUX_NEG).code,
-        }
-
-    def __get_rtd_state(self) -> bool:
-        """
-        Get on/off RTD state.
-        """
-        return self.__get_current_rtd_state() == RTDModes.RTD_ON.value
-
-
-class ADCStateMissingMap(Exception):
-    """ "Raised if ADCState.get_map() is called before ADCState has been assigned a cached state"""
-
-
-class ADCRegisterUpdateError(Exception):
-    """Raised when a register update fails to set register to expected value"""
-
-
-class VoltageReadError(Exception):
-    """Raised if a voltage read fails to return the expected number of bytes"""
-
-
-class ContinuousModeError(Exception):
-    """Raised when `read_voltage` is called and ADC is not in CONTINUOUS conversion mode"""
-
-
-class RTDEnabledError(Exception):
-    """Raised when user attempts to set ADC configuration that conflicts with RTD mode"""
-
-
-class InvalidDifferentialPairError(Exception):
-    """
-    Raised when calibration values are attempted to be retrieved for an invalid Differential
-    read pair
-    """
-
-
-class CalibKeyMissingError(Exception):
-    """Raised when calibration values are missing from EEPROM dictionary"""
-
-
 class EdgePiADC(SPI):
     """
     EdgePi ADC device
 
     Warning, when caching is enabled to track the ADC's internal state, EdgePiADC objects are
     safe to use only within a single dev environment. Using multiple EdgePiADC objects,
     each within a different environment, will lead to the cached ADC state being out of sync
@@ -192,17 +79,26 @@
     # keep track of ADC register map state for state caching
     __state: dict = {}
 
     # default RTD model-dependent hardware constants
     RTD_SENSOR_RESISTANCE = 100 # RTD sensor resistance value (Ohms)
     RTD_SENSOR_RESISTANCE_VARIATION = 0.385 # RTD sensor resistance variation (Ohms/°C)
 
-    # TODO: this should be part of eeprom_data. Retrieve from eeprom_data in calling
-    # functions when available
-    r_ref = 1326.20
+    __analog_in_to_adc_in_map = {
+        AnalogIn.AIN1: CH.AIN0,
+        AnalogIn.AIN2: CH.AIN1,
+        AnalogIn.AIN3: CH.AIN2,
+        AnalogIn.AIN4: CH.AIN3,
+        AnalogIn.AIN5: CH.AIN4,
+        AnalogIn.AIN6: CH.AIN5,
+        AnalogIn.AIN7: CH.AIN6,
+        AnalogIn.AIN8: CH.AIN7,
+        AnalogIn.AINCOM : CH.AINCOM,
+        AnalogIn.FLOAT : CH.FLOAT
+    }
 
     def __init__(
         self,
         enable_cache: bool = False,
         rtd_sensor_resistance: float = None,
         rtd_sensor_resistance_variation: float = None
         ):
@@ -218,26 +114,28 @@
 
         super().__init__(bus_num=6, dev_id=1)
         # declare instance vars before config call below
         self.enable_cache = enable_cache
 
         # Load eeprom data and generate dictionary of calibration dataclass
         eeprom = EdgePiEEPROM()
-        eeprom_data  = eeprom.get_edgepi_reserved_data()
-        self.adc_calib_params = eeprom_data.adc_calib_parms
+        eeprom_data  = eeprom.read_edgepi_data()
+        self.adc_calib_params = {ADCNum.ADC_1:eeprom_data.adc1_calib_params.extract_ch_dict(),
+                                 ADCNum.ADC_2:eeprom_data.adc2_calib_params.extract_ch_dict(),}
+        self.r_ref = eeprom_data.rtd_calib_params.rtd_resistor
 
         self.adc_ops = ADCCommands()
         self.gpio = EdgePiGPIO()
         # ADC always needs to be in CRC check mode. This also updates the internal __state.
         # If this call to __config is removed, replace with a call to get_register_map to
         # initialize __state.
         self.__config(checksum_mode=CheckMode.CHECK_BYTE_CRC)
         # TODO: adc reference should ba a config that customer passes depending on the range of
         # voltage they are measuring. To be changed later when range config is implemented
-        self.set_adc_reference(ADCReferenceSwitching.GND_SW1.value)
+        # self.set_adc_reference(ADCReferenceSwitching.GND_SW1.value)
 
         # user updated rtd hardware constants
         self.rtd_sensor_resistance = (
             rtd_sensor_resistance
             if rtd_sensor_resistance is not None
             else EdgePiADC.RTD_SENSOR_RESISTANCE
         )
@@ -249,18 +147,18 @@
         )
 
     def __reapply_config(self):
         """
         Restore ADC to custom EdgePi configuration
         """
         # turn RTD off to allow updates in case RTD is on
-        self.rtd_mode(enable=False)
+        self.set_rtd(set_rtd=False)
         self.__config(
-            adc_1_analog_in=CH.FLOAT,
-            adc_2_analog_in=CH.FLOAT,
+            adc_1_ch=CH.FLOAT,
+            adc_2_ch=CH.FLOAT,
             adc_1_mux_n=CH.AINCOM,
             adc_2_mux_n=CH.AINCOM,
             checksum_mode=CheckMode.CHECK_BYTE_CRC,
         )
 
     def __update_cache_map(self, reg_map: dict):
         """
@@ -309,20 +207,17 @@
 
         Returns:
             `list`: a list of ints representing bytes formatted as [reg_1_data, reg_2_data,...]
                 where reg_1_data is the data of the register at start_addx.
         """
         if num_regs < 1:
             raise ValueError("Number of registers to read must be at least 1")
-
         code = self.adc_ops.read_register_command(start_addx.value, num_regs)
-        _logger.debug(f"ADC __read_register -> data in: {code}")
         out = self.transfer(code)
-        _logger.debug(f"ADC __read_register -> data out: {out}")
-
+        _logger.debug(f"__read_register: received {out}")
         # first 2 entries are null bytes
         return out[2:]
 
     def __write_register(self, start_addx: ADCReg, data: list[int]):
         """
         Write data to ADC registers, either individually or as a block.
 
@@ -330,22 +225,32 @@
             `start_addx` (ADCReg): address of register to start writing data from.
 
             `data` (list): list of int values, where each value represents a byte of data
                 to write to a register.
         """
         if len(data) < 1:
             raise ValueError("Number of registers to write to must be at least 1")
-
         code = self.adc_ops.write_register_command(start_addx.value, data)
-        _logger.debug(f"ADC __write_register -> data in: {code}")
+        _logger.debug(f"__write_register: sending {code}")
         out = self.transfer(code)
-        _logger.debug(f"ADC __write_register -> data out: {out}")
-
         return out
 
+    def __set_rtd_pin(self, enable: bool = False):
+        """
+        Set or clear RTD_EN pin
+        Args:
+            enable (bool): RTD enable flag
+        Return:
+            None
+        """
+        # pylint: disable=expression-not-assigned
+        self.gpio.set_pin_state(RTDPins.RTD_EN.value) if enable else \
+        self.gpio.clear_pin_state(RTDPins.RTD_EN.value)
+
+# TODO: To be deleted
     def set_adc_reference(self, reference_config: ADCReferenceSwitching = None):
         """
         Setting ADC referene terminal state. pin 18 and 23 labeled IN GND on the enclosure. It can
         be configured as regular 0V GND or 12V GND.
 
         Args:
             reference_config: (ADCReferenceSwitching): selecting none, 1, 2, both
@@ -378,15 +283,14 @@
     def start_conversions(self, adc_num: ADCNum):
         """
         Start ADC voltage read conversions. If ADC is continuous conversion mode,
         this method must be called before performing reads. If ADC is in
         pulse conversion mode, this method does not need to be called before
         performing reads.
         """
-
         # get state for configs relevant to conversion delay
         state = self.get_state()
         conv_mode = state.adc_1.conversion_mode.code
         data_rate = (
             state.adc_1.data_rate.code if adc_num == ADCNum.ADC_1 else state.adc_2.data_rate.code
         )
         filter_mode = state.filter_mode.code
@@ -394,20 +298,19 @@
         conv_delay = expected_initial_time_delay(
             adc_num, data_rate.value.op_code, filter_mode.value.op_code
         )
         _logger.debug(
             (
                 f"\nComputed time delay = {conv_delay} (ms) with the following config opcodes:\n"
                 f"adc_num={adc_num}, conv_mode={hex(conv_mode.value.op_code)}, "
-                f"data_rate={hex(data_rate.value.op_code)}"
+                f"data_rate={hex(data_rate.value.op_code)}, "
                 f"filter_mode={hex(filter_mode.value.op_code)}\n"
             )
         )
         self.__send_start_command(adc_num)
-
         # apply delay for first conversion
         time.sleep(conv_delay / 1000)
 
     def clear_reset_bit(self):
         """
         Clear the ADC reset bit. This reset bits acts as a flag that is raised when the ADC
         resets, which automatically happens during power on, or when a reset command is passed.
@@ -426,28 +329,22 @@
         and check bytes
 
         Returns:
             int, list[int], int: uint values of representations of voltage read data ordered as
                 (status_byte, voltage_data_bytes, check_byte)
         """
         read_data = self.__read_data(adc_num, ADC_VOLTAGE_READ_LEN)
-
         if len(read_data) - 1 != ADC_VOLTAGE_READ_LEN:
             raise VoltageReadError(
                 f"Voltage read failed: incorrect number of bytes ({len(read_data)}) retrieved"
             )
-
         status_code = read_data[1]
-
         voltage_code = read_data[2 : (2 + adc_num.value.num_data_bytes)]
-
         check_code = read_data[6]
-
         check_crc(voltage_code, check_code)
-
         return status_code, voltage_code, check_code
 
     @staticmethod
     def __get_diff_id(mux_p: PropertyValue, mux_n: PropertyValue) -> int:
         """
         Get differential pair id number for retrieving differential pair calibration values
         """
@@ -483,43 +380,40 @@
         mux_n = attrgetter(f"adc_{adc_num.value.id_num}.mux_n")(state)
 
         # assert neither mux is set to float mode
         if CH.FLOAT in (mux_p.code, mux_n.code):
             raise ValueError("Cannot retrieve calibration values for channel in float mode")
 
         calib_key = mux_p.value if mux_n.code == CH.AINCOM else self.__get_diff_id(mux_p, mux_n)
-
-        calibs = adc_calibs.get(calib_key)
+        calibs = adc_calibs[calib_key]
 
         if calibs is None:
             _logger.error("Failed to find ADC calibration values")
             raise CalibKeyMissingError(
                 (
                     "Failed to retrieve calibration values from eeprom dictionary: "
                     f"dict is missing key = {calib_key}"
                     f"\neeprom_calibs = \n{adc_calibs}"
                 )
             )
 
         return calibs
 
-    def __continuous_time_delay(self, adc_num: ADCNum):
+    def __continuous_time_delay(self, adc_num: ADCNum, state: ADCState):
         """Compute and enforce continuous conversion time delay"""
-        state = self.get_state()
         # get continuous mode time delay and wait here (delay is needed between each conversion)
         data_rate = (
             state.adc_1.data_rate.code if adc_num == ADCNum.ADC_1 else state.adc_2.data_rate.code
         )
         delay = expected_continuous_time_delay(adc_num, data_rate.value.op_code)
 
         time.sleep(delay / 1000)
 
-    def __check_adc_1_conv_mode(self):
+    def __check_adc_1_conv_mode(self, state: ADCState):
         # assert adc is in continuous mode
-        state = self.get_state()
         if state.adc_1.conversion_mode.code != ConvMode.CONTINUOUS:
             raise ContinuousModeError(
                 "ADC1 must be in CONTINUOUS conversion mode in order to call this method."
             )
 
     def read_voltage(self, adc_num: ADCNum):
         """
@@ -529,161 +423,196 @@
 
         Args:
             `adc_num` (ADCNum): the ADC to be read
 
         Returns:
             `float`: input voltage (V) read from the indicated ADC
         """
+        single_ended = False
+        state = self.get_state()
         if adc_num == ADCNum.ADC_1:
-            self.__check_adc_1_conv_mode()
+            self.__check_adc_1_conv_mode(state)
+            # Check whether the ADC is either in single-ended or differential
+            if state.adc_1.mux_n.code == CH.AINCOM:
+                single_ended = True
+        else:
+            if state.adc_2.mux_n.code == CH.AINCOM:
+                single_ended = True
 
-        self.__continuous_time_delay(adc_num)
+        self.__continuous_time_delay(adc_num, state)
 
         status_code, voltage_code, _ = self.__voltage_read(adc_num)
 
         # log STATUS byte
         status = get_adc_status(status_code)
-        _logger.debug(f"Logging STATUS byte:\n{status}")
-
-        calibs = self.__get_calibration_values(self.adc_calib_params, adc_num)
+        _logger.debug(f" read_voltage: Logging STATUS byte:\n{status}")
 
+        calibs = self.__get_calibration_values(self.adc_calib_params[adc_num], adc_num)
+        _logger.debug(f" read_voltage: gain {calibs.gain}, offset {calibs.offset}")
         # convert from code to voltage
-        return code_to_voltage(voltage_code, adc_num.value, calibs)
+
+        return code_to_voltage_single_ended(voltage_code, adc_num.value, calibs) if single_ended\
+            else code_to_voltage(voltage_code, adc_num.value, calibs)
 
 
     def read_rtd_temperature(self):
         """
         Read RTD temperature continuously. Note, to obtain valid temperature values,
         RTD mode must first be enabled by calling `rtd_mode`. ADC1 must also be configured
         to `CONTINUOUS` conversion mode via `set_config`, before calling this method.
 
         Returns:
             `float`: RTD measured temperature (°C)
         """
-        self.__check_adc_1_conv_mode()
-
-        self.__continuous_time_delay(ADCNum.ADC_1)
+        state = self.get_state()
+        adc_num = state.rtd_adc
+        if adc_num == ADCNum.ADC_1:
+            self.__check_adc_1_conv_mode(state)
+        self.__continuous_time_delay(adc_num, state)
 
-        _, voltage_code, _ = self.__voltage_read(ADCNum.ADC_1)
+        _, voltage_code, _ = self.__voltage_read(adc_num)
 
-        # TODO: get RTD calibs from eeprom once added
         return code_to_temperature(
             voltage_code,
             self.r_ref,
             self.rtd_sensor_resistance,
-            self.rtd_sensor_resistance_variation
+            self.rtd_sensor_resistance_variation,
+            adc_num
         )
 
-    def __enforce_pulse_mode(self):
+    def __enforce_pulse_mode(self, state: ADCState):
         # assert adc is in PULSE mode (check ADCState) -> set to PULSE if not
-        state = self.get_state()
         if state.adc_1.conversion_mode.code != ConvMode.PULSE:
             self.__config(conversion_mode=ConvMode.PULSE)
 
     def single_sample(self):
         """
         Trigger a single ADC1 voltage sampling event, when performing single channel reading or
         differential reading. ADC1 must be in `PULSE` conversion mode before calling this method.
         Do not call this method for voltage reading if ADC is configured to `CONTINUOUS`
         conversion mode: use `read_voltage` instead.
 
         Returns:
             `float`: input voltage (V) read from ADC1
         """
-        self.__enforce_pulse_mode()
+        state = self.get_state()
+        single_ended = False
+        # Check whether the ADC is either in single-ended or differential
+        if state.adc_1.mux_n.code == CH.AINCOM:
+            single_ended = True
+
+        self.__enforce_pulse_mode(state)
 
         # send command to trigger conversion
         self.start_conversions(ADCNum.ADC_1)
 
         # send command to read conversion data.
         status_code, voltage_code, _ = self.__voltage_read(ADCNum.ADC_1)
 
         # log STATUS byte
         status = get_adc_status(status_code)
-        _logger.debug(f"Logging STATUS byte:\n{status}")
+        _logger.debug(f"single_sample: Logging STATUS byte:\n{status}")
 
-        calibs = self.__get_calibration_values(self.adc_calib_params, ADCNum.ADC_1)
+        calibs = self.__get_calibration_values(self.adc_calib_params[ADCNum.ADC_1], ADCNum.ADC_1)
 
         # convert from code to voltage
-        return code_to_voltage(voltage_code, ADCNum.ADC_1.value, calibs)
+        _logger.debug(f" read_voltage: code {voltage_code}")
+        _logger.debug(f" read_voltage: gain {calibs.gain}, offset {calibs.offset}")
+        return code_to_voltage_single_ended(voltage_code, ADCNum.ADC_1.value, calibs) if \
+            single_ended  else code_to_voltage(voltage_code, ADCNum.ADC_1.value, calibs)
 
     def single_sample_rtd(self):
         """
         Trigger a single RTD temperature sampling event. Note, to obtain valid temperature values,
         RTD mode must first be enabled by calling `rtd_mode`. ADC1 must also be configured
         to `PULSE` conversion mode via `set_config`, before calling this method.
 
         Returns:
             `float`: RTD measured temperature (°C)
         """
-        self.__enforce_pulse_mode()
+        state = self.get_state()
+        adc_num = state.rtd_adc
+        if adc_num == ADCNum.ADC_1:
+            self.__enforce_pulse_mode(state)
 
         # send command to trigger conversion
-        self.start_conversions(ADCNum.ADC_1)
+        self.start_conversions(adc_num)
 
         # send command to read conversion data.
-        _, voltage_code, _ = self.__voltage_read(ADCNum.ADC_1)
+        _, voltage_code, _ = self.__voltage_read(adc_num)
 
-        # TODO: get RTD calibs from eeprom once added
         return code_to_temperature(
             voltage_code,
             self.r_ref,
             self.rtd_sensor_resistance,
-            self.rtd_sensor_resistance_variation
+            self.rtd_sensor_resistance_variation,
+            adc_num
         )
 
     def reset(self):
         """
         Reset ADC register values to EdgePi ADC power-on state.
         Note this state differs from ADS1263 default power-on, due to
         application of custom power-on configurations required by EdgePi.
         """
         self.transfer(self.adc_ops.reset_adc())
         self.__reapply_config()
 
-    def __is_data_ready(self):
+    def __is_data_ready(self, adc_num: ADCNum):
         # pylint: disable=unused-private-member
         # required for integration testing in test_conversion_times.py
         """Utility for testing conversion times, returns True if ADC indicates new voltage data"""
-        read_data = self.transfer([ADCComs.COM_RDATA1.value] + [255] * 6)
-        return read_data[1] & 0b01000000
+        read_data = self.transfer([adc_num.value.read_cmd] + [255] * 6)
+        if adc_num is ADCNum.ADC_1:
+            ready = (read_data[1] & 0b01000000) == 0b01000000
+        if adc_num is ADCNum.ADC_2:
+            ready = (read_data[1] & 0b10000000) == 0b10000000
+        return ready
 
     def __read_registers_to_map(self):
         """
         Reads value of all ADC registers to a dictionary
 
         Returns:
             `dict`: contains {register addx (int): register_value (int)} pairs
         """
         # get register values
         reg_values = self.__read_register(ADCReg.REG_ID, ADC_NUM_REGS)
         addx = ADCReg.REG_ID.value
 
         # build dict with (register addx : register_value) pairs.
         reg_dict = {addx + i: reg_values[i] for i in range(ADC_NUM_REGS)}
-        _logger.debug(f"__read_registers_to_map: {reg_dict}")
+        # _logger.debug(f"__read_registers_to_map: {reg_dict}")
 
         return reg_dict
 
     def __is_rtd_on(self):
         """
-        Get state of RTD_EN pin (on/off), to use for deciding which
-        ADC channels are available for reading.
+        Check whether the RTD is enabled or disabled
+        Args:
+            N/A
+        Return:
+            rtd_pin_state (bool): True RTD enabled, False RTD disabled
+        """
+        pin_state = self.gpio.read_pin_state(RTDPins.RTD_EN.value)
+        pin_dir = self.gpio.get_pin_direction(RTDPins.RTD_EN.value)
+        if pin_state and not pin_dir:
+            return True
+        return False
 
+    def __get_rtd_state(self):
+        """
+        Get RTD state this includes the corrent mode (on/off) and the adc type being used
+        (adc1 or adc2).
         Returns:
-            `bool`: True if RTD_EN pin is on, False otherwise
+            rtd_mode (dictionary): RTD mode dictionary {"name of config": op_codes}
+            rtd_adc (ADCNum): None, no adc attached to RTD, ADCNum.ADC1 or ADCNum.ADC1
         """
-        # TODO: this should use self.get_state() instead
-        _logger.debug("Checking RTD status")
-        idac_reg = self.__get_register_map()
-        idac_mag = pack("uint:8", idac_reg.get(ADCReg.REG_IDACMAG.value))
-        idac_1 = idac_mag[4:].uint
-        status = idac_1 != 0x0
-        _logger.debug(f"RTD enabled: {status}")
-        return status
+        state = self.get_state()
+        return state.rtd_mode, state.rtd_adc
 
     # by default set mux_n's to AINCOM. For diff_mode and rtd_mode, pass in custom mapping.
     # Case 1: user sets to adc_x read ch_x -> mux_n auto mapped to AINCOM
     # Case 2: user sets RTD mode on or off -> mux_n passed in as arg
     # Case 3: user sets any differential mode -> mux_n pass in as arg
     def __get_channel_assign_opcodes(
         self,
@@ -713,17 +642,15 @@
         if adc_1_mux_p is None:
             adc_1_mux_n = None
 
         if adc_2_mux_p is None:
             adc_2_mux_n = None
 
         # no multiplexer config to update
-        # TODO: refactor filter_dict to take list arg
-        args = filter_dict(locals(), "self", None)
-        args = filter_dict(args, "override_rtd_validation")
+        args = filter_dict_list_key_val(locals(), ["self", "override_rtd_validation"], [None])
         if not args:
             return []
 
         # allowed channels depend on RTD_EN status
         if not override_rtd_validation:
             channels = list(args.values())
             rtd_enabled = self.__is_rtd_on()
@@ -750,71 +677,115 @@
         Raises:
             `KeyError`: if adc is not a valid ADCNum enum
         """
         mux_p = diff_mode.value.mux_p
         mux_n = diff_mode.value.mux_n
         mux_properties = {
             ADCNum.ADC_1: {
-                "adc_1_analog_in": mux_p,
+                "adc_1_ch": mux_p,
                 "adc_1_mux_n": mux_n,
             },
             ADCNum.ADC_2: {
-                "adc_2_analog_in": mux_p,
+                "adc_2_ch": mux_p,
                 "adc_2_mux_n": mux_n,
             },
         }
         diff_update = mux_properties[adc]
         self.__config(**diff_update)
 
-    def __validate_no_rtd_conflict(self, updates: dict):
+    def  __validate_no_rtd_conflict(self, updates: dict):
         """
         Checks no RTD related properties are being updated if RTD mode is enabled
 
         Args:
             `updates` (dict): updates formatted as {'property_name': update_value}
 
         Raises:
             `RTDEnabledError`: if RTD is enabled and an RTD related property is in updates
         """
-        # ADC2 channel setting conflicts with RTD handled during channel mapping
-        if not self.__is_rtd_on():
-            return
-
-        rtd_properties = RTDModes.RTD_ON.value.keys()
+        rtd_mode, rtd_adc = self.__get_rtd_state()
+        if rtd_mode is None or rtd_mode == RTDModes.RTD_OFF:
+            return None
+
+        # rtd_properties RTDModes.RTD1_ON or RTDModes.RTD2_ON
+        rtd_properties = rtd_mode.value | (ADC1RtdConfig.ON.value if rtd_adc == ADCNum.ADC_1 else\
+                                           ADC2RtdConfig.ON.value)
         for update in updates:
             if update in rtd_properties:
                 raise RTDEnabledError(
                     f"ADC property '{update}' cannot be updated while RTD is enabled"
                 )
+        return None
 
-    def rtd_mode(self, enable: bool):
+    def __check_adc_pins(self):
         """
-        Enable or disable RTD. Note, this will reconfigure ADC2 to read FLOAT input channel
-        if ADC2 is configured to read RTD pins AIN4-AIN7. To read RTD values aftering enabling
-        RTD mode here, call either `read_voltage` or `single_sample`, depending on which
-        conversion mode ADC1 is currently configured to.
-
-        Args:
-            `enable` (bool): True to enable RTD, False to disable
-        """
-        # TODO: enable RTD_EN switching pin
-        if enable:
-            # check if adc_2 is reading RTD pins, remap channels if needed
-            mux_reg = self.__get_register_map()
-            adc2_mux = pack("uint:8", mux_reg.get(ADCReg.REG_ADC2MUX.value))
-            muxs = [adc2_mux[:4].uint, adc2_mux[4:].uint]
-            if any(mux not in [x.value for x in AllowedChannels.RTD_ON.value] for mux in muxs):
-                updates = RTDModes.RTD_ON.value | {
-                    "adc_2_analog_in": CH.FLOAT,
-                    "adc_2_mux_n": CH.AINCOM,
-                }
-            else:
-                updates = RTDModes.RTD_ON.value
+        check pin mux of each adc
+        Args:
+            N/A
+        Return:
+            channels
+        """
+        state = self.get_state()
+        adc_1_muxs = [state.adc_1.mux_n.code.value, state.adc_1.mux_p.code.value]
+        adc_2_muxs = [state.adc_2.mux_n.code.value, state.adc_2.mux_p.code.value]
+        return adc_1_muxs, adc_2_muxs
+
+    def __get_rtd_on_update_config(self, muxs: list, adc_num: ADCNum):
+        """
+        generate a dictionary of config parameters to enable RTD using specified ADC
+        Args:
+            muxs (list): list of input multiplexer of other ADC [negative input, positive input]
+            adc_num (ADCNum): ADC to read RTD
+        Return:
+            updates (dictionary): configuration dictionary for enabling RTD
+                                    {name_of_config : op_codes}
+        """
+        if any(mux not in [x.value for x in AllowedChannels.RTD_ON.value] for mux in muxs):
+            updates = RTDModes.RTD_ON.value |\
+            (ADC2RtdConfig.OFF.value if adc_num == ADCNum.ADC_1 else ADC1RtdConfig.OFF.value) |\
+            (ADC1RtdConfig.ON.value if adc_num ==ADCNum.ADC_1 else ADC2RtdConfig.ON.value)
         else:
-            updates = RTDModes.RTD_OFF.value
+            updates = RTDModes.RTD_ON.value |\
+            (ADC1RtdConfig.ON.value if adc_num ==ADCNum.ADC_1 else ADC2RtdConfig.ON.value)
+        return updates
+
+
+    def __get_rtd_off_update_config(self, adc_num: ADCNum):
+        """
+        generate update config dictionary to send to the config method
+        Args:
+            adc_num (ADCNum): ADC number
+        Return:
+            updates (dictionary): configuration dictionary for disabling RTD
+        """
+        updates = RTDModes.RTD_OFF.value |\
+        (ADC1RtdConfig.OFF.value if adc_num == ADCNum.ADC_1  else ADC2RtdConfig.OFF.value)
+        return updates
+
+    def set_rtd(self, set_rtd: bool, adc_num: ADCNum = ADCNum.ADC_2):
+        """
+        Enable/Disable RTD with ADC type passed as arguments.
+
+        NOTE: This function enforces only one ADC to be attached to RTD circuit
+
+        Args:
+            `set_rtd` (bool): True to enable RTD, False to disable
+        """
+        if set_rtd:
+            # check inputs of both ADCs. Input 5~8 are only available for RTD reading
+            mux_1, mux_2 = self.__check_adc_pins()
+            # If inputs on another ADC are one of RTD only inputs, reconfigure the pins them to the
+            # default setting. And get RTD_ON configuration values
+            updates = self.__get_rtd_on_update_config(
+                           mux_2 if adc_num == ADCNum.ADC_1 else mux_1, adc_num)
+            # enable RTD pin to re-route internal circuit
+            self.__set_rtd_pin(set_rtd)
+        else:
+            updates = self.__get_rtd_off_update_config(adc_num)
+            self.__set_rtd_pin(set_rtd)
 
         self.__config(**updates, override_rtd_validation=True)
 
     @staticmethod
     def __extract_mux_args(args: dict) -> dict:
         """
         Checks args dictionary for input multiplexer settings
@@ -822,54 +793,55 @@
         Args:
             `args` (dict): args formatted as {'arg_name': value}
 
         Returns:
             `dict`: input multiplexer args formatted as {'mux_name': value}
         """
         mux_arg_names = {
-            "adc_1_analog_in": "adc_1_mux_p",
-            "adc_2_analog_in": "adc_2_mux_p",
+            "adc_1_ch": "adc_1_mux_p",
+            "adc_2_ch": "adc_2_mux_p",
             "adc_1_mux_n": "adc_1_mux_n",
             "adc_2_mux_n": "adc_2_mux_n",
         }
         only_mux_args = {}
         for arg, mux_name in mux_arg_names.items():
             if args.get(arg) is not None:
                 only_mux_args[mux_name] = args[arg]
         return only_mux_args
 
     def __config(
         self,
-        adc_1_analog_in: CH = None,
-        adc_2_analog_in: CH = None,
+        adc_1_ch: CH = None,
+        adc_2_ch: CH = None,
         adc_1_mux_n: CH = None,
         adc_2_mux_n: CH = None,
         adc_1_data_rate: ADC1DataRate = None,
         adc_2_data_rate: ADC2DataRate = None,
         filter_mode: FilterMode = None,
         conversion_mode: ConvMode = None,
         checksum_mode: CheckMode = None,
         reset_clear: ADCPower = None,
         idac_1_mux: IDACMUX = None,
         idac_2_mux: IDACMUX = None,
         idac_1_mag: IDACMAG = None,
         idac_2_mag: IDACMAG = None,
         pos_ref_inp: REFMUX = None,
         neg_ref_inp: REFMUX = None,
+        adc2_ref_inp: ADC2REFMUX = None,
         override_updates_validation: bool = False,
         override_rtd_validation: bool = False,
     ):
         """
         Configure all ADC settings, either collectively or individually.
         Warning: for internal EdgePi developer use only, users should use
         `set_config()` for modifying settings instead.
 
         Args:
-            `adc_1_analog_in` (ADCChannel): input voltage channel to map to ADC1 mux_p
-            `adc_2_analog_in` (ADCChannel): input voltage channel to map to ADC2 mux_p
+            `adc_1_ch` (ADCChannel): input voltage channel to map to ADC1 mux_p
+            `adc_2_ch` (ADCChannel): input voltage channel to map to ADC2 mux_p
             `adc_1_mux_n` (ADCChannel): input voltage channel to map to ADC1 mux_n
             `adc_2_mux_n` (ADCChannel): input voltage channel to map to ADC1 mux_n
             `adc_1_data_rate` (ADC1DataRate): ADC1 data rate in samples per second
             `adc_2_data_rate` (ADC2DataRate): ADC2 data rate in samples per second,
             `filter_mode` (FilterMode): filter mode for both ADC1 and ADC2.
                 Note this affects data rate. Please refer to module documentation
                 for more information.
@@ -883,18 +855,17 @@
             `idac_2_mag` (IDACMAG): set the current value for IDAC2
             `pos_ref_inp` (REFMUX): set the positive reference input
             `neg_ref_inp` (REFMUX): set the negative reference input
             `override_updates_validation` (bool): set to True to override post-update validation
             `override_rtd_validation` (bool): turn off RTD property validation for RTD mode updates
         """
         # pylint: disable=unused-argument
-
         # filter out self and None args
         args = filter_dict(locals(), "self", None)
-        _logger.debug(f"__config: args after filtering out None defaults:\n\n{args}\n\n")
+        _logger.debug(f"__config: args after filtering out None defaults:\n{args}")
 
         # permit updates by rtd_mode() to turn RTD off when it's on, validate other updates
         if not override_rtd_validation:
             self.__validate_no_rtd_conflict(args)
 
         # get opcodes for mapping multiplexers
         mux_args = self.__extract_mux_args(args)
@@ -908,20 +879,19 @@
             entry.value
             for entry in args
             if issubclass(entry.__class__, Enum) and isinstance(entry.value, OpCode)
         ]
 
         # get current register values
         reg_values = self.__get_register_map()
-        _logger.debug(f"__config: register values before updates:\n\n{reg_values}\n\n")
+        _logger.debug(f"__config: register values before updates:\n{reg_values}")
 
         # get codes to update register values
-        _logger.debug(f"opcodes = {ops_list}")
         updated_reg_values = apply_opcodes(dict(reg_values), ops_list)
-        _logger.debug(f"__config: register values after updates:\n\n{reg_values}\n\n")
+        _logger.debug(f"__config: register values after updates:\n{reg_values}")
 
         # write updated reg values to ADC using a single write.
         data = [entry["value"] for entry in updated_reg_values.values()]
         self.__write_register(ADCReg.REG_ID, data)
 
         # update ADC state (for state caching)
         self.__update_cache_map(updated_reg_values)
@@ -953,39 +923,49 @@
                     )
                 )
 
         return True
 
     def set_config(
         self,
-        adc_1_analog_in: CH = None,
+        adc_1_analog_in: AnalogIn = None,
         adc_1_data_rate: ADC1DataRate = None,
-        adc_2_analog_in: CH = None,
+        adc_2_analog_in: AnalogIn = None,
         adc_2_data_rate: ADC2DataRate = None,
         filter_mode: FilterMode = None,
         conversion_mode: ConvMode = None,
         override_updates_validation: bool = False,
     ):
         """
         Configure user accessible ADC settings, either collectively or individually.
 
         Args:
-            `adc_1_analog_in` (ADCChannel): the input voltage channel to measure via ADC1
+            `adc_1_analog_in` (AnalogIn): the input voltage channel to measure via ADC1
             `adc_1_data_rate` (ADC1DataRate): ADC1 data rate in samples per second
-            `adc_2_analog_in` (ADCChannel): the input voltage channel to measure via ADC2
+            `adc_2_analog_in` (AnalogIn): the input voltage channel to measure via ADC2
             `adc_2_data_rate` (ADC2DataRate): ADC2 data rate in samples per second
             `filter_mode` (FilterMode): filter mode for ADC1.
                 Note this affects data rate. Please refer to module documentation
                 for more information.
             `conversion_mode` (ConvMode): set conversion mode for ADC1.
             `override_updates_validation` (bool): set to True to skip update validation
         """
+        # pylint: disable=possibly-unused-variable
         # pylint: disable=unused-argument
+        adc_1_ch  = self.__analog_in_to_adc_in_map.get(adc_1_analog_in)
+        adc_2_ch  = self.__analog_in_to_adc_in_map.get(adc_2_analog_in)
 
-        args = filter_dict(locals(), "self", None)
+        if adc_1_ch is None and adc_1_analog_in is not None:
+            raise TypeError(f"set_config: wrong type passed for adc_1_analog_in: {adc_1_analog_in}")
+        if adc_2_ch is None and adc_2_analog_in is not None:
+            raise TypeError(f"set_config: wrong type passed for adc_2_analog_in: {adc_2_analog_in}")
+
+        args = filter_dict_list_key_val(locals(),
+                                        ["self", "adc_1_analog_in", "adc_2_analog_in"],
+                                        [None])
         self.__config(**args)
 
     def get_state(self, override_cache: bool = False) -> ADCState:
         """
         Read the current hardware state of configurable ADC properties
 
         Args:
```

### Comparing `edgepi-python-sdk-1.1.7/src/edgepi/calibration/calibration_constants.py` & `edgepi-python-sdk-1.2.1/src/edgepi/calibration/calibration_constants.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.1.7/src/edgepi/calibration/edgepi_calibration.py` & `edgepi-python-sdk-1.2.1/src/edgepi/calibration/edgepi_calibration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 Module for generating calibration parameter data structure for each module. This module should be
 able to generate new calibration parameters using measurements tools.
 '''
 
-from edgepi.calibration.eeprom_constants import ModuleNames
+from edgepi.eeprom.eeprom_constants import ModuleNames
 from edgepi.calibration.calibration_constants import NumOfCh
 
 
 class EdgePiCalibration():
     '''
     EdgePi Calibration Class handling the following functionality
     1. load calibration parameter
```

### Comparing `edgepi-python-sdk-1.1.7/src/edgepi/dac/dac_commands.py` & `edgepi-python-sdk-1.2.1/src/edgepi/dac/dac_commands.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,23 +19,25 @@
 
     def __init__(self, dict_calib_param):
         _logger.info("Initializing DAC Methods")
         self.dict_calib_param = dict_calib_param
 
     def generate_write_and_update_command(self, ch: int, data: int) -> list:
         """Construct a write and update command"""
-        self.check_range(ch, 0, len(CH))
+        self.check_range(ch, 0, NUM_PINS-1)
         self.check_range(data, 0, CALIB_CONSTS.RANGE.value)
         return self.combine_command(COMMAND.COM_WRITE_UPDATE.value, CH(ch).value, data)
 
     def __voltage_to_float_code(self, ch: int, expected: float, dac_gain: int = 1):
-        """Convert a voltage to full precision binary code value"""
-        float_code =((expected / dac_gain) - self.dict_calib_param[ch].offset) * \
-                    (CALIB_CONSTS.RANGE.value / \
-                    (CALIB_CONSTS.V_RANGE.value * self.dict_calib_param[ch].gain))
+        """
+        Convert a voltage to full precision binary code value
+        code = ((expected_v - offset)/gain) * (Code_range/V_range))/DAC_GAIN
+        """
+        float_code =(((expected-self.dict_calib_param[ch].offset)/self.dict_calib_param[ch].gain)*\
+                    (CALIB_CONSTS.RANGE.value/CALIB_CONSTS.V_RANGE.value))/dac_gain
         _logger.debug(f"Full code generated {float_code}")
         return float_code
 
     def voltage_to_code(self, ch: int, expected: float, dac_gain: int = 1) -> int:
         """
         Convert a voltage to binary code value
 
@@ -46,15 +48,15 @@
 
             dac_gain (int): dac gain state, x1 or x2, when x2 voltage range extened to 10V from 5V
 
         Returns:
             int: 16 bit binary code value for writing voltage value to DAC
         """
         # DAC channels are 0 indexed
-        self.check_range(ch, 0, NUM_PINS - 1)
+        self.check_range(ch, 0, NUM_PINS-1)
         float_code = self.__voltage_to_float_code(ch, expected, dac_gain)
         _logger.debug(f"Int code generated {int(float_code)}")
         # DAC only accepts int values, round to nearest int
         return round(float_code)
 
     @staticmethod
     def extract_read_data(read_code: list) -> int:
@@ -77,18 +79,20 @@
         bits = pack("uint:8, uint:8, uint:8", read_code[0], read_code[1], read_code[2])
 
         # B23 to DB20 contain undefined data, and the last 16 bits contain the
         # DB19 to DB4 DAC register contents. B23 (MSB) is index 0 here.
         return bits[-16:].uint
 
     def __code_to_float_voltage(self, ch: int, code: int, dac_gain: int = 1) -> float:
-        """Convert a voltage to float voltage"""
-        voltage = (CALIB_CONSTS.V_RANGE.value /
-                   CALIB_CONSTS.RANGE.value * self.dict_calib_param[ch].gain) *\
-                  (code*dac_gain) + self.dict_calib_param[ch].offset
+        """
+        Convert a voltage to float voltage
+        ((Code*DAC_GAIN)*(V_Range/CodeRange))*Calib_Gain + Calib_Offset
+        """
+        voltage = ((code*dac_gain)*(CALIB_CONSTS.V_RANGE.value/CALIB_CONSTS.RANGE.value))*\
+                  self.dict_calib_param[ch].gain + self.dict_calib_param[ch].offset
         return voltage
 
     def code_to_voltage(self, ch: int, code: int, dac_gain: int = 1) -> float:
         """
         Convert a 16 bit binary code value to voltage
 
         Args:
```

### Comparing `edgepi-python-sdk-1.1.7/src/edgepi/dac/dac_constants.py` & `edgepi-python-sdk-1.2.1/src/edgepi/dac/dac_constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from enum import Enum
 
 
 DAC_PRECISION = 3  # decimal place precision for voltage conversions
 SW_RESET = 0x1234  # software reset command data bits
 NULL_BITS = 0x0
 READ_WRITE_SIZE = 3  # size of DAC read/write in bytes
-UPPER_LIMIT = 5.0 # upper limit for voltage writes to DAC
+UPPER_LIMIT = 5.000 # upper limit for voltage writes to DAC
 
 
 class EdgePiDacCom(Enum):
     """Commands for EdgePi DAC"""
 
     COM_NOP = 0x0
     COM_WRITE_INPUT = 0x1  # LDAC pin is held low, so not used
@@ -30,22 +30,22 @@
     # update all channel of teh input register and DAC register simultaneously with the input data
     COM_UPDATE_ALL_DAC = 0x0B
 
 
 class DACChannel(Enum):
     """EdgePi DAC channel addresses"""
 
-    AOUT0 = 0x0
-    AOUT1 = 0x1
-    AOUT2 = 0x2
-    AOUT3 = 0x3
-    AOUT4 = 0x4
-    AOUT5 = 0x5
-    AOUT6 = 0x6
-    AOUT7 = 0x7
+    AOUT1 = 0x0
+    AOUT2 = 0x1
+    AOUT3 = 0x2
+    AOUT4 = 0x3
+    AOUT5 = 0x4
+    AOUT6 = 0x5
+    AOUT7 = 0x6
+    AOUT8 = 0x7
 
 
 NUM_PINS = len(DACChannel)
 
 
 class EdgePiDacCalibrationConstants(Enum):
     """EdgePi DAC calibration constants"""
@@ -82,10 +82,22 @@
     AO_EN3 = "AO_EN3"
     AO_EN4 = "AO_EN4"
     AO_EN5 = "AO_EN5"
     AO_EN6 = "AO_EN6"
     AO_EN7 = "AO_EN7"
     AO_EN8 = "AO_EN8"
 
+class DOPins(Enum):
+    """Analog/Digital out gpio pin names"""
+
+    DOUT1 = 'DOUT1'
+    DOUT2 = 'DOUT2'
+    DOUT3 = 'DOUT3'
+    DOUT4 = 'DOUT4'
+    DOUT5 = 'DOUT5'
+    DOUT6 = 'DOUT6'
+    DOUT7 = 'DOUT7'
+    DOUT8 = 'DOUT8'
+
 class GainPin(Enum):
     """DAC gain enable/disable pin"""
     DAC_GAIN = "DAC_GAIN"
```

### Comparing `edgepi-python-sdk-1.1.7/src/edgepi/dac/edgepi_dac.py` & `edgepi-python-sdk-1.2.1/src/edgepi/dac/edgepi_dac.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,93 +11,122 @@
     SW_RESET,
     UPPER_LIMIT,
     PowerMode,
     DACChannel,
     EdgePiDacCom as COM,
     EdgePiDacCalibrationConstants as CalibConst,
     AOPins,
+    DOPins,
     GainPin
 )
 from edgepi.peripherals.spi import SpiDevice as spi
+from edgepi.gpio.gpio_constants import GpioPins
 from edgepi.gpio.edgepi_gpio import EdgePiGPIO
-from edgepi.calibration.edgepi_eeprom import EdgePiEEPROM
+from edgepi.eeprom.edgepi_eeprom import EdgePiEEPROM
 
 class EdgePiDAC(spi):
     """A EdgePi DAC device"""
 
     # analog_out number to pin name
     __analog_out_pin_map = {
-        DACChannel.AOUT0.value: AOPins.AO_EN1,
-        DACChannel.AOUT1.value: AOPins.AO_EN2,
-        DACChannel.AOUT2.value: AOPins.AO_EN3,
-        DACChannel.AOUT3.value: AOPins.AO_EN4,
-        DACChannel.AOUT4.value: AOPins.AO_EN5,
-        DACChannel.AOUT5.value: AOPins.AO_EN6,
-        DACChannel.AOUT6.value: AOPins.AO_EN7,
-        DACChannel.AOUT7.value: AOPins.AO_EN8,
+        DACChannel.AOUT1.value: AOPins.AO_EN1,
+        DACChannel.AOUT2.value: AOPins.AO_EN2,
+        DACChannel.AOUT3.value: AOPins.AO_EN3,
+        DACChannel.AOUT4.value: AOPins.AO_EN4,
+        DACChannel.AOUT5.value: AOPins.AO_EN5,
+        DACChannel.AOUT6.value: AOPins.AO_EN6,
+        DACChannel.AOUT7.value: AOPins.AO_EN7,
+        DACChannel.AOUT8.value: AOPins.AO_EN8,
     }
 
+    # analog_out number to DOUT pin pair
+    __analog_to_digital_pin_map = {
+        DACChannel.AOUT1.value: DOPins.DOUT1,
+        DACChannel.AOUT2.value: DOPins.DOUT2,
+        DACChannel.AOUT3.value: DOPins.DOUT3,
+        DACChannel.AOUT4.value: DOPins.DOUT4,
+        DACChannel.AOUT5.value: DOPins.DOUT5,
+        DACChannel.AOUT6.value: DOPins.DOUT6,
+        DACChannel.AOUT7.value: DOPins.DOUT7,
+        DACChannel.AOUT8.value: DOPins.DOUT8,
+    }
+
+
+
     def __init__(self):
         self.log = logging.getLogger(__name__)
         self.log.info("Initializing DAC Bus")
         super().__init__(bus_num=6, dev_id=3, mode=1, max_speed=1000000)
 
         # Read edgepi reserved data and generate calibration parameter dictionary
         eeprom = EdgePiEEPROM()
-        eeprom_data  = eeprom.get_edgepi_reserved_data()
-        dac_calib_params = eeprom_data.dac_calib_parms
+        eeprom_data  = eeprom.read_edgepi_data()
+        dac_calib_params = eeprom_data.dac_calib_params.extract_ch_dict()
 
         self.dac_ops = DACCommands(dac_calib_params)
         self.gpio = EdgePiGPIO()
 
         self.__dac_power_state = {
+            DACChannel.AOUT8.value: PowerMode.NORMAL.value,
             DACChannel.AOUT7.value: PowerMode.NORMAL.value,
             DACChannel.AOUT6.value: PowerMode.NORMAL.value,
             DACChannel.AOUT5.value: PowerMode.NORMAL.value,
             DACChannel.AOUT4.value: PowerMode.NORMAL.value,
             DACChannel.AOUT3.value: PowerMode.NORMAL.value,
             DACChannel.AOUT2.value: PowerMode.NORMAL.value,
             DACChannel.AOUT1.value: PowerMode.NORMAL.value,
-            DACChannel.AOUT0.value: PowerMode.NORMAL.value,
         }
 
     def __send_to_gpio_pins(self, analog_out: int, voltage: float):
         ao_pin = self.__analog_out_pin_map[analog_out].value
-
+        do_pin = self.__analog_to_digital_pin_map[analog_out].value
         if voltage > 0:
             self.gpio.set_pin_state(ao_pin)
+            self.gpio.clear_pin_state(do_pin)
+            if analog_out in [DACChannel.AOUT1.value, DACChannel.AOUT2.value]:
+                self.__dac_switching_logic(analog_out)
         elif voltage == 0:
             self.gpio.clear_pin_state(ao_pin)
+            if analog_out in [DACChannel.AOUT2.value,DACChannel.AOUT1.value]:
+                self.__dac_switching_logic(analog_out)
         else:
             raise ValueError("voltage cannot be negative")
 
+    def __dac_switching_logic(self, analog_out: int):
+        """
+        In order to attach DAC output to the terminal block, proper swtiching of GPIO should happen.
+        AOUT1 and AOUT2 have special switching logic.
+
+        Args:
+            `analog_out` (DACChannel): A/D_OUT pin to write a voltage value to.
+        """
+        pwm_en = GpioPins.PWM1 if analog_out == DACChannel.AOUT1.value else GpioPins.PWM2
+        self.gpio.set_pin_direction_out(pwm_en.value)
+        self.gpio.set_pin_state(pwm_en.value)
+
     # TODO: Decimal instead of float for precision testing
     def write_voltage(self, analog_out: DACChannel, voltage: float):
         """
         Write a voltage value to an analog out pin. Voltage will be continuously
         transmitted to the analog out pin until a 0 V value is written to it.
 
         Args:
             `analog_out` (DACChannel): A/D_OUT pin to write a voltage value to.
 
             `voltage` (float): the voltage value to write, in volts.
 
         Raises:
             `ValueError`: if voltage has more decimal places than DAC accuracy limit
         """
-        self.dac_ops.check_range(analog_out.value, 0, NUM_PINS-1)
-        self.dac_ops.check_range(voltage, 0, UPPER_LIMIT)
         dac_gain = CalibConst.DAC_GAIN_FACTOR.value if self.__get_gain_state() else 1
+        self.dac_ops.check_range(analog_out.value, 0, NUM_PINS-1)
+        self.dac_ops.check_range(voltage, 0, (UPPER_LIMIT*dac_gain))
         code = self.dac_ops.voltage_to_code(analog_out.value, voltage, dac_gain)
         self.log.debug(f'Code: {code}')
 
-        if self.gpio.get_pin_direction(self.__analog_out_pin_map[analog_out.value].value):
-            self.gpio.clear_pin_state(self.__analog_out_pin_map[analog_out.value].value)
-            self.gpio.set_pin_direction_out(self.__analog_out_pin_map[analog_out.value].value)
-
         # update DAC register
         self.transfer(self.dac_ops.generate_write_and_update_command(analog_out.value, code))
         # send voltage to analog out pin
         self.__send_to_gpio_pins(analog_out.value, voltage)
         return code
 
     def set_power_mode(self, analog_out: DACChannel, power_mode: PowerMode):
@@ -163,37 +192,114 @@
             float: the computed voltage value of the DAC channel corresponding
                 to the selected analog out pin.
         """
         code = self.channel_readback(analog_out)
         dac_gain = CalibConst.DAC_GAIN_FACTOR.value if self.__get_gain_state() else 1
         return self.dac_ops.code_to_voltage(analog_out.value, code, dac_gain)
 
-    def enable_dac_gain(self, enable: bool = None):
+    def __compute_code_val(self, set_gain: bool, code: int = None):
         """
-        Enable/Disable internal DAC gain by toggling the DAC_GAIN pin
+        Modify code value depending on the enable flag
         Args:
-            enable (bool): enable boolean to set or clear the gpio pin
+            set_gain(bool): False: multiply the current code value by 2 if current code value is
+                               less than the half of maixmum code value.
+                               True: divide the current code value by 2
+            code (int): intial code value
+        Return:
+            code (int): modified code value
+        """
+        if set_gain:
+            return int(code/CalibConst.DAC_GAIN_FACTOR.value)
+
+        code = code*CalibConst.DAC_GAIN_FACTOR.value
+        if code > CalibConst.RANGE.value:
+            raise ValueError(f"Code Value: {code} is out of range")
+
+        return code
+
+    def __get_ch_codes(self, set_gain: bool):
+        """
+        Read and modify channel code value
+        Args:
+            set_gain (bool): False: multiply the current code value by 2
+                          True: divide the current code value by 2
+        Return:
+            code_vals (list): list of code values from ch1-ch8
+        """
+        code_vals = []
+        for ch in DACChannel:
+            code, _, _ = self.get_state(ch, True, False, False)
+            code_vals.append(self.__compute_code_val(set_gain, code))
+        return code_vals
+
+    def __auto_code_handler(self, set_gain: bool):
+        """
+        Compute and change code values of each channel when toggling DAC gain
+        Args:
+            set_gain (bool): enable boolean to set or clear the gpio pin
+        Return:
+            N/A
+        """
+        codes = self.__get_ch_codes(set_gain)
+        self.log.debug(f'Code: {codes}')
+
+        # When the DAC_GAIN is enabled/disabled, the output voltage is doubled/halved instantly.
+        # This may damage the circuit that the output is connected to. Therefore, enabling/disabling
+        # gain have different steps of sending code value and toggling the GPIO pin.
+
+        # gain being enabled, change code first than enable gain
+        if set_gain:
+            for ch, code in enumerate(codes):
+                # update DAC register
+                self.transfer(self.dac_ops.generate_write_and_update_command(ch, code))
+            self.gpio.set_pin_state(GainPin.DAC_GAIN.value)
+
+        # Disabling gain, change gain first than change codes
+        else:
+            self.gpio.clear_pin_state(GainPin.DAC_GAIN.value)
+            for ch, code in enumerate(codes):
+                # update DAC register
+                self.transfer(self.dac_ops.generate_write_and_update_command(ch, code))
+
+    def set_dac_gain(self, set_gain: bool, auto_code_change: bool = False):
+        """
+        Enable/Disable internal DAC gain.
+        Args:
+            set_gain (bool): True enable DAC gain, False disable DAC gain
+            auto_code_change (bool): flag to re-write code value of each channel to keep the same
+                                    output voltage
         Return:
             gain_state (bool): state of the gain pin
         """
         # pylint: disable=expression-not-assigned
-        self.gpio.set_pin_state(GainPin.DAC_GAIN.value) if enable else \
-        self.gpio.clear_pin_state(GainPin.DAC_GAIN.value)
+        # if current gain state is the same as toggle_gain flag, do nothing
+        if self.__get_gain_state() == set_gain:
+            return set_gain
+
+        if auto_code_change:
+            self.__auto_code_handler(set_gain)
+        else:
+            self.gpio.set_pin_state(GainPin.DAC_GAIN.value) if set_gain else \
+            self.gpio.clear_pin_state(GainPin.DAC_GAIN.value)
         return self.__get_gain_state()
 
     def __get_gain_state(self):
         """
         Retrieve the internal gain state by reading the expander pin
         Args:
             N/A
         Return:
             gain_state (bool): True - gain enalbed, False - gain disabled
         """
-        _, _, gain_state = self.get_state(gain=True)
-        return gain_state
+
+        pin_state = self.gpio.read_pin_state(GainPin.DAC_GAIN.value)
+        pin_dir = self.gpio.get_pin_direction(GainPin.DAC_GAIN.value)
+        if pin_state and not pin_dir:
+            return True
+        return False
 
     def get_state(self, analog_out: DACChannel = None,
                         code: bool = None,
                         voltage: bool = None,
                         gain: bool = None):
         """
         the method returns the state of requested parameters. It will either read the register of
@@ -209,9 +315,11 @@
             code_val (int): code value read from the input register, None when not requested
             voltage_val (float): voltage calculated using the code value, None when not requested
             gain_state (bool): true if dac gain is enabled or False disabled, None when not
                                requested
         """
         code_val = self.channel_readback(analog_out) if code else None
         voltage_val = self.compute_expected_voltage(analog_out) if voltage else None
-        gain_state = self.gpio.get_pin_direction(GainPin.DAC_GAIN.value) if gain else None
+        gain_state = self.__get_gain_state() if gain else None
+        self.log.debug(f":get_state: state of {analog_out} code {code_val},"
+                       f"expected {voltage_val}, dac_gain {gain_state}")
         return code_val, voltage_val, gain_state
```

### Comparing `edgepi-python-sdk-1.1.7/src/edgepi/digital_input/edgepi_digital_input.py` & `edgepi-python-sdk-1.2.1/src/edgepi/digital_input/edgepi_digital_input.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 """Digital Input Module"""
 
-from edgepi.gpio.gpio_constants import GpioPins
-from edgepi.gpio.gpio_configs import DINPins
+from edgepi.digital_input.digital_input_constants import DinPins
 from edgepi.gpio.edgepi_gpio import EdgePiGPIO
 
 class InvalidPinName(Exception):
     """Raised invalid pin name"""
 
 class EdgePiDigitalInput():
     """handling reading of digital inputs"""
     def __init__(self):
         # To limit access to input functionality, using composition rather than inheritance
         self.gpio = EdgePiGPIO()
 
-    def digital_input_state(self, pin_name: GpioPins = None):
+    def digital_input_state(self, pin_name: DinPins = None):
         """
         Read selected GPIO pin
         Args:
-            pin_name (GpioPins): GpioPin enums
+            pin_name (DinPins): GpioPin enums
         Return:
             state (bool): corresponding pin state
         """
-        if pin_name is None or pin_name.value not in [pins.value for pins in DINPins]:
+        if pin_name is None or pin_name.value not in [pins.value for pins in DinPins]:
             raise InvalidPinName(f'Invalid pin name passed: {pin_name}')
         return self.gpio.read_pin_state(pin_name.value)
```

### Comparing `edgepi-python-sdk-1.1.7/src/edgepi/gpio/edgepi_gpio.py` & `edgepi-python-sdk-1.2.1/src/edgepi/gpio/edgepi_gpio.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.1.7/src/edgepi/gpio/edgepi_gpio_chip.py` & `edgepi-python-sdk-1.2.1/src/edgepi/gpio/edgepi_gpio_chip.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 '''
 Provides a class for interacting with the GPIO pins through GPIO peripheral
 '''
 
 import logging
 from edgepi.peripherals.gpio import GpioDevice
 from edgepi.gpio.gpio_constants import GpioDevPaths
-from edgepi.gpio.gpio_configs import DOUTPins, DINPins, generate_gpiochip_pin_info
+from edgepi.gpio.gpio_configs import DINPins, generate_gpiochip_pin_info
 
 _logger = logging.getLogger(__name__)
 
 class EdgePiGPIOChip(GpioDevice):
     """
     A class to represent the GPIO peripheral using gpiochip device. This class will be imported to
     each module that requires GPIO manipulation.
@@ -17,18 +17,17 @@
     # dictionary mapping pin name to CPU gpio pin number
     __pin_name_dict = {DINPins.DIN1.value : 26,
                        DINPins.DIN2.value : 6,
                        DINPins.DIN3.value : 11,
                        DINPins.DIN4.value : 9,
                        DINPins.DIN5.value : 22,
                        DINPins.DIN6.value : 27,
-                       DINPins.DIN7.value : 3,
-                       DINPins.DIN8.value : 2,
-                       DOUTPins.DOUT1.value : 13,
-                       DOUTPins.DOUT2.value : 12}
+                       DINPins.DIN7.value : 10,
+                       DINPins.DIN8.value : 7
+                    }
 
     def __init__(self):
         super().__init__(GpioDevPaths.GPIO_CIHP_DEV_PATH.value)
         self.gpiochip_pins_dict = generate_gpiochip_pin_info()
 
     def read_gpio_pin_state(self, pin_name: str = None):
         """
@@ -40,15 +39,15 @@
         Returns:
             `bool`: True if state is high, False if state is low
         """
         self.open_gpio(pin_num=self.__pin_name_dict[pin_name],
                        pin_dir=self.gpiochip_pins_dict[pin_name].dir,
                        pin_bias=self.gpiochip_pins_dict[pin_name].bias)
         state = self.read_state()
-        self.close()
+        self.close_gpio()
         return state
 
     def write_gpio_pin_state(self, pin_name: str = None, state: bool = None):
         """
         write pin state
         Args:
             pin_name (str): name of the pin to write state to
@@ -57,28 +56,28 @@
             N/A
         """
         self.open_gpio(pin_num=self.__pin_name_dict[pin_name],
                        pin_dir=self.gpiochip_pins_dict[pin_name].dir,
                        pin_bias=self.gpiochip_pins_dict[pin_name].bias)
         self.write_state(state)
         read_back = self.read_state()
-        self.close()
+        self.close_gpio()
         return read_back
 
     def set_gpio_pin_dir(self, pin_name: str = None, direction: bool = None):
         """
         Set gpio pin direction
         Args:
             pin_name (str): name of the pin
             direction (bool): direction to write, True = Input, False = Output
         """
         self.open_gpio(pin_num=self.__pin_name_dict[pin_name],
                        pin_dir="in" if direction else "out",
                        pin_bias=self.gpiochip_pins_dict[pin_name].bias)
-        self.close()
+        self.close_gpio()
 
     def toggle_gpio_pin_state(self, pin_name: str = None):
         """
         Toggle pin state
         Args:
             pin_name (str): name of the pin to write state to
         Return:
@@ -88,8 +87,8 @@
                        pin_dir=self.gpiochip_pins_dict[pin_name].dir,
                        pin_bias=self.gpiochip_pins_dict[pin_name].bias)
         state = self.read_state()
         if state:
             self.write_state(False)
         else:
             self.write_state(True)
-        self.close()
+        self.close_gpio()
```

### Comparing `edgepi-python-sdk-1.1.7/src/edgepi/gpio/edgepi_gpio_expander.py` & `edgepi-python-sdk-1.2.1/src/edgepi/gpio/edgepi_gpio_expander.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,19 +29,19 @@
         Args:
             `reg_address`: register/port address to read data from
             `dev_address`: expander address to read
         Returns:
             `int`: 8-bit uint value of port/register
         '''
         msg_read = self.set_read_msg(reg_address, [0xFF])
-        _logger.debug(f'Read Message: Register Address {msg_read[0].data}\
-                      , Msg Place Holder {msg_read[1].data}')
+        _logger.debug(f"Read Message: Register Address {msg_read[0].data}"
+                      f", Msg Place Holder {msg_read[1].data}")
         self.transfer(dev_address, msg_read)
-        _logger.debug(f'Message Read: Register Address {msg_read[0].data},\
-         Msg Place Holder {msg_read[1].data}')
+        _logger.debug(f"Message Read: Register Address {msg_read[0].data},"
+                      f"Msg Place Holder {msg_read[1].data}")
         return msg_read[1].data[0]
 
     def __write_changed_values(self, reg_dict: dict, dev_address: int):
         '''
         Function to write changed values to the specified register
         In:
             reg_dict (dict): register address to value and is_changed flag
@@ -110,17 +110,14 @@
         dev_address = self.expander_pin_dict[pin_name].address
         dir_out_code = self.expander_pin_dict[pin_name].dir_out_code
         reg_addx = dir_out_code.reg_address
 
         # get register value of port this pin belongs to
         reg_val = self.__read_register(reg_addx, dev_address)
 
-        # set pin to low before setting to output (hazard)
-        self.clear_expander_pin(pin_name)
-
         # set pin direction to out
         self.__apply_code_to_register(dev_address, reg_addx, reg_val, dir_out_code)
         _logger.debug(":set_expander_pin_direction_out: pin '%s' set to output", pin_name)
 
         self.expander_pin_dict[pin_name].is_out = True
 
     def set_expander_pin_direction_in(self, pin_name: str):
@@ -153,16 +150,17 @@
         dev_address = self.expander_pin_dict[pin_name].address
         set_code = self.expander_pin_dict[pin_name].set_code
         reg_addx = set_code.reg_address
 
         # get register value of port this pin belongs to
         reg_val = self.__read_register(reg_addx, dev_address)
 
-        # set pin direction to output (also sets to low)
-        self.set_expander_pin_direction_out(pin_name)
+        if self.get_expander_pin_direction(pin_name):
+            # set pin direction to output (also sets to low)
+            self.set_expander_pin_direction_out(pin_name)
 
         # set pin state to high
         self.__apply_code_to_register(dev_address, reg_addx, reg_val, set_code)
         _logger.debug(":set_expander_pin: pin '%s' = set to high", pin_name)
 
         self.expander_pin_dict[pin_name].is_high = True
 
@@ -198,17 +196,21 @@
         dev_address = self.expander_pin_dict[pin_name].address
         clear_code = self.expander_pin_dict[pin_name].clear_code
         reg_addx = clear_code.reg_address
 
         # get register value of port this pin belongs to
         reg_val = self.__read_register(reg_addx, dev_address)
 
+        if self.get_expander_pin_direction(pin_name):
+            # set pin direction to output (also sets to low)
+            self.set_expander_pin_direction_out(pin_name)
+
         # set pin state to low
         self.__apply_code_to_register(dev_address, reg_addx, reg_val, clear_code)
-        _logger.debug(":set_expander_pin: pin '%s' = set to low", pin_name)
+        _logger.debug(":clear_expander_pin: pin '%s' = set to low", pin_name)
 
         self.expander_pin_dict[pin_name].is_high = False
 
     def toggle_expander_pin(self, pin_name: str):
         '''
         Function toggle gpio pin state to opposite logic
```

### Comparing `edgepi-python-sdk-1.1.7/src/edgepi/gpio/gpio_configs.py` & `edgepi-python-sdk-1.2.1/src/edgepi/gpio/gpio_configs.py`

 * *Files 11% similar despite different names*

```diff
@@ -79,36 +79,46 @@
     RTD = GpioExpanderConfig(name = 'rtd',
                              device='i2c',
                              num_pins=1,
                              dir='out',
                              port='B',
                              address=GpioExpanderAddress.EXP_TWO.value,
                              dev_path='/dev/i2c-10')
+    RELAY = GpioExpanderConfig(name = 'relay',
+                             device='i2c',
+                             num_pins=1,
+                             dir='out',
+                             port='B',
+                             address=GpioExpanderAddress.EXP_TWO.value,
+                             dev_path='/dev/i2c-10')
     LED = GpioExpanderConfig(name = 'led',
                              device='i2c',
                              num_pins=8,
                              dir='in',
                              port='B',
                              address=GpioExpanderAddress.EXP_ONE.value,
                              dev_path='/dev/i2c-10')
     DIN = GpioChipConfig(name = 'din',
                          device = 'gpiochip0',
                          num_pins = 8,
                          dev_path = "/dev/gpiochip0")
-    DOUT1 = GpioChipConfig(name = 'dout1',
-                          device = 'gpiochip0',
-                          num_pins = 2,
-                          dev_path = "/dev/gpiochip0")
-    DOUT2 = GpioExpanderConfig(name = 'dout2',
+    DOUT = GpioExpanderConfig(name = 'dout',
                                device='i2c',
-                               num_pins=6,
+                               num_pins=8,
                                dir='out',
                                port='A',
                                address=GpioExpanderAddress.EXP_TWO.value,
                                dev_path='/dev/i2c-10')
+    PWM = GpioExpanderConfig(name = 'pwm',
+                               device='i2c',
+                               num_pins=2,
+                               dir='out',
+                               port='B',
+                               address=GpioExpanderAddress.EXP_TWO.value,
+                               dev_path='/dev/i2c-10')
 
 @dataclass
 class I2cPinInfo:
     '''
     Represents I2C pin information
 
         Attributes:
@@ -170,14 +180,19 @@
 class RTDPins(Enum):
     "RTD GPIO Pin Names"
     RTD_EN = 'RTD_EN'
 
 
 _list_of_RTD_gpios = [RTDPins.RTD_EN.value]
 
+class RELAYPins(Enum):
+    "RTD GPIO Pin Names"
+    RELAY_EN = 'RELAY_EN'
+_list_of_RELAY_gpios = [RELAYPins.RELAY_EN.value]
+
 
 class LEDPins(Enum):
     "LED GPIO Pin Names"
     LED_OVR1 = 'LED_OVR1'
     LED_OVR2 = 'LED_OVR2'
     LED_OVR3 = 'LED_OVR3'
     LED_OVR4 = 'LED_OVR4'
@@ -222,24 +237,24 @@
     DOUT3 = 'DOUT3'
     DOUT4 = 'DOUT4'
     DOUT5 = 'DOUT5'
     DOUT6 = 'DOUT6'
     DOUT7 = 'DOUT7'
     DOUT8 = 'DOUT8'
 
-
-_list_of_DOUT_cpu_gpios =  [
-    DOUTPins.DOUT1.value, DOUTPins.DOUT2.value
-]
-
 _list_of_DOUT_expander_gpios =[
+    None, None,
     DOUTPins.DOUT8.value, DOUTPins.DOUT7.value,
     DOUTPins.DOUT6.value, DOUTPins.DOUT5.value,
     DOUTPins.DOUT4.value, DOUTPins.DOUT3.value]
 
+class PWMPins(Enum):
+    "PWM Enable Pin Names"
+    PWM1 = "PWM1"
+    PWM2 = "PWM2"
 
 def _generate_DAC_pins(): #pylint: disable=C0103
     ''' Generates a list I2cPinInfo dataclasses for DAC pins
         Args:
             N/A
         Returns:
             a dictionary of dataclass with gpio information, {'pin_name' : pin_info_dataclass}
@@ -311,56 +326,91 @@
     pin_dict.update({_list_of_RTD_gpios[0] : I2cPinInfo(GpioBOutputSet.SET_OUTPUT_1.value,
                                                         GpioBOutputClear.CLEAR_OUTPUT_1.value,
                                                         GpioBPinDirOut.PIN1_DIR_OUT.value,
                                                         GpioBPinDirIn.PIN1_DIR_IN.value,
                                                         GpioExpanderAddress.EXP_TWO.value)})
     return pin_dict
 
-def _generate_DIN_pins(): #pylint: disable=C0103
-    """
+def _generate_RELAY_pins(): #pylint: disable=C0103
+    '''
         Args:
             N/A
         Returns:
         a dictionary of dataclass with gpio information, {'pin_name' : pin_info_dataclass}
-    """
+    '''
     pin_dict = {}
-    for pin in _list_of_DIN_gpios:
-        pin_dict[pin] = GpioChipPinInfo(dir = "in", bias = "pull_down")
+    pin_dict.update({_list_of_RELAY_gpios[0] : I2cPinInfo(GpioBOutputSet.SET_OUTPUT_8.value,
+                                                        GpioBOutputClear.CLEAR_OUTPUT_8.value,
+                                                        GpioBPinDirOut.PIN8_DIR_OUT.value,
+                                                        GpioBPinDirIn.PIN8_DIR_IN.value,
+                                                        GpioExpanderAddress.EXP_TWO.value)})
     return pin_dict
 
-def _generate_DOUT_cpu_pins(): #pylint: disable=C0103
+def _generate_DIN_pins(): #pylint: disable=C0103
     """
         Args:
             N/A
         Returns:
         a dictionary of dataclass with gpio information, {'pin_name' : pin_info_dataclass}
     """
     pin_dict = {}
-    for pin in _list_of_DOUT_cpu_gpios:
-        pin_dict[pin] = GpioChipPinInfo(dir = "out", bias = "pull_down")
+    for pin in _list_of_DIN_gpios:
+        pin_dict[pin] = GpioChipPinInfo(dir = "in", bias = "pull_down")
     return pin_dict
 
 def _generate_DOUT_expander_pins(): #pylint: disable=C0103
     """
         Args:
             N/A
         Returns:
         a dictionary of dataclass with gpio information, {'pin_name' : pin_info_dataclass}
     """
     pin_dict = {}
     for pin, set_code, clear_code, dir_out_code, dir_in_code in \
     zip(_list_of_DOUT_expander_gpios,GpioAOutputSet,GpioAOutputClear,GpioAPinDirOut,GpioAPinDirIn):
-
+        if pin is None:
+            continue
         pin_dict.update({pin : I2cPinInfo(set_code.value,
                                           clear_code.value,
                                           dir_out_code.value,
                                           dir_in_code.value,
                                           GpioExpanderAddress.EXP_TWO.value)})
+    pin_dict.update({DOUTPins.DOUT1.value : I2cPinInfo(GpioBOutputSet.SET_OUTPUT_4.value,
+                                                      GpioBOutputClear.CLEAR_OUTPUT_4.value,
+                                                      GpioBPinDirOut.PIN4_DIR_OUT.value,
+                                                      GpioBPinDirIn.PIN4_DIR_IN.value,
+                                                      GpioExpanderAddress.EXP_TWO.value)})
+
+    pin_dict.update({DOUTPins.DOUT2.value : I2cPinInfo(GpioBOutputSet.SET_OUTPUT_5.value,
+                                                      GpioBOutputClear.CLEAR_OUTPUT_5.value,
+                                                      GpioBPinDirOut.PIN5_DIR_OUT.value,
+                                                      GpioBPinDirIn.PIN5_DIR_IN.value,
+                                                      GpioExpanderAddress.EXP_TWO.value)})
     return pin_dict
 
+def _generate_PWM_expander_pins(): #pylint: disable=C0103
+    """
+        Args:
+            N/A
+        Returns:
+        a dictionary of dataclass with gpio information, {'pin_name' : pin_info_dataclass}
+    """
+    pin_dict = {}
+    pin_dict.update({PWMPins.PWM1.value : I2cPinInfo(GpioBOutputSet.SET_OUTPUT_6.value,
+                                                      GpioBOutputClear.CLEAR_OUTPUT_6.value,
+                                                      GpioBPinDirOut.PIN6_DIR_OUT.value,
+                                                      GpioBPinDirIn.PIN6_DIR_IN.value,
+                                                      GpioExpanderAddress.EXP_TWO.value)})
+
+    pin_dict.update({PWMPins.PWM2.value : I2cPinInfo(GpioBOutputSet.SET_OUTPUT_7.value,
+                                                      GpioBOutputClear.CLEAR_OUTPUT_7.value,
+                                                      GpioBPinDirOut.PIN7_DIR_OUT.value,
+                                                      GpioBPinDirIn.PIN7_DIR_IN.value,
+                                                      GpioExpanderAddress.EXP_TWO.value)})
+    return pin_dict
 
 # This function is used inside unit testing
 def generate_pin_info(config: Union[GpioExpanderConfig, GpioChipConfig] = None):
     ''' Generates a dictionary of pin info dataclasses
         Args:
             config (GpioExpanderConfig): name of the module to configure the gpio pins fors
         Returns:
@@ -371,41 +421,44 @@
         pin_dict =  _generate_DAC_pins()
     elif config.name == GpioConfigs.LED.value.name:
         pin_dict =  _generate_LED_pins()
     elif config.name == GpioConfigs.ADC.value.name:
         pin_dict =  _generate_ADC_pins()
     elif config.name == GpioConfigs.RTD.value.name:
         pin_dict =  _generate_RTD_pins()
+    elif config.name == GpioConfigs.RELAY.value.name:
+        pin_dict = _generate_RELAY_pins()
     elif config.name == GpioConfigs.DIN.value.name:
         pin_dict = _generate_DIN_pins()
-    elif config.name == GpioConfigs.DOUT1.value.name:
-        pin_dict = _generate_DOUT_cpu_pins()
-    elif config.name == GpioConfigs.DOUT2.value.name:
+    elif config.name == GpioConfigs.DOUT.value.name:
         pin_dict = _generate_DOUT_expander_pins()
+    elif config.name == GpioConfigs.PWM.value.name:
+        pin_dict = _generate_PWM_expander_pins()
     return pin_dict
 
 def generate_expander_pin_info():
     ''' Generates a dictionary of pin info dataclasses
         Args:
             N/A
         Returns:
             a dictionary of dataclass with gpio information, {'pin_name' : pin_info_dataclass}
     '''
     pin_dict = {}
     pin_dict.update(_generate_DAC_pins())
     pin_dict.update(_generate_ADC_pins())
     pin_dict.update(_generate_RTD_pins())
+    pin_dict.update(_generate_RELAY_pins())
     pin_dict.update(_generate_LED_pins())
     pin_dict.update(_generate_DOUT_expander_pins())
+    pin_dict.update(_generate_PWM_expander_pins())
     return pin_dict
 
 def generate_gpiochip_pin_info():
     ''' Generates a dictionary of pin info dataclasses
         Args:
             N/A
         Returns:
             a dictionary of dataclass with gpio information, {'pin_name' : pin_info_dataclass}
     '''
     pin_dict = {}
     pin_dict.update(_generate_DIN_pins())
-    pin_dict.update(_generate_DOUT_cpu_pins())
     return pin_dict
```

### Comparing `edgepi-python-sdk-1.1.7/src/edgepi/gpio/gpio_constants.py` & `edgepi-python-sdk-1.2.1/src/edgepi/gpio/gpio_constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,15 @@
     AO_EN6 = 'AO_EN6'
     AO_EN7 = 'AO_EN7'
     AO_EN8 = 'AO_EN8'
     DAC_GAIN = 'DAC_GAIN'
     GNDSW_IN1 = 'GNDSW_IN1'
     GNDSW_IN2 = 'GNDSW_IN2'
     RTD_EN = 'RTD_EN'
-    RELAY = 'RELAY'
+    RELAY = 'RELAY_EN'
     DOUT1 = 'DOUT1'
     DOUT2 = 'DOUT2'
     DOUT3 = 'DOUT3'
     DOUT4 = 'DOUT4'
     DOUT5 = 'DOUT5'
     DOUT6 = 'DOUT6'
     DOUT7 = 'DOUT7'
@@ -195,7 +195,9 @@
     DIN4 = 'DIN4'
     DIN5 = 'DIN5'
     DIN6 = 'DIN6'
     DIN7 = 'DIN7'
     DIN8 = 'DIN8'
     BUZZER = 'BUZZER'
     AUDIO = 'AUDIO'
+    PWM1 = 'PWM1'
+    PWM2 = 'PWM2'
```

### Comparing `edgepi-python-sdk-1.1.7/src/edgepi/led/edgepi_leds.py` & `edgepi-python-sdk-1.2.1/src/edgepi/led/edgepi_leds.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """EdgePi LED array"""
 
 
 import logging
 
 
-from edgepi.gpio.gpio_configs import LEDPins
+from edgepi.led.led_constants import LEDPins
 from edgepi.gpio.edgepi_gpio import EdgePiGPIO
 
 
 class InvalidLEDNameError(Exception):
     """
     Raised if a user attempts to pass an invalid LED name to
     an EdgePiLED method."""
```

### Comparing `edgepi-python-sdk-1.1.7/src/edgepi/peripherals/gpio.py` & `edgepi-python-sdk-1.2.1/src/edgepi/peripherals/gpio.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,10 +39,10 @@
         Args:
             state (bool): High if True else LOW
         Return:
             N/A
         """
         self.gpio.write(state)
 
-    def close(self):
+    def close_gpio(self):
         """Close GPIO connection"""
         self.gpio.close()
```

### Comparing `edgepi-python-sdk-1.1.7/src/edgepi/peripherals/i2c.py` & `edgepi-python-sdk-1.2.1/src/edgepi/peripherals/i2c.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 """
 Module for I2C devices
 
 Classes:
     I2CDevice
 """
+import logging
 
 from typing import Union
 from periphery import I2C
 
+_logger = logging.getLogger(__name__)
+
 class I2CDevice():
     '''
     I2C Device class
     '''
     def __init__(self, fd: str = None):
         self.fd = fd
-        self.i2cdev = I2C(fd)
+        _logger.debug(f"Initialized I2C device with path '{self.fd}'")
+        self.i2cdev = I2C(devpath=fd)
 
     def set_read_msg(self, addr:Union[int,list] = None, msg:list = None):
         '''
         set Read message to be sent through I2C.
         Attributes:
             addr(int or list): Register address to read from
             Msg: list of place holder bytes
```

### Comparing `edgepi-python-sdk-1.1.7/src/edgepi/peripherals/spi.py` & `edgepi-python-sdk-1.2.1/src/edgepi/peripherals/spi.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,15 +38,13 @@
             bit_order,
             bits_per_word,
             extra_flags,
         )
 
     def transfer(self, data: list) -> list:
         """Conduct an SPI data transfer"""
-        _logger.debug(f"Before SPI transfer: data={data}")
         out = self.spi.transfer(data)
-        _logger.debug(f"After SPI transfer: data={out}")
         return out
 
     def close(self):
         """Close SPI connection"""
         self.spi.close()
```

### Comparing `edgepi-python-sdk-1.1.7/src/edgepi/reg_helper/reg_helper.py` & `edgepi-python-sdk-1.2.1/src/edgepi/reg_helper/reg_helper.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.1.7/src/edgepi/tc/edgepi_tc.py` & `edgepi-python-sdk-1.2.1/src/edgepi/tc/edgepi_tc.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     CJLowMask,
     CJMode,
     ConvMode,
     DecBits4,
     DecBits6,
     FaultMode,
     NoiseFilterMode,
+    Masks,
     OpenCircuitMode,
     OpenMask,
     OvuvMask,
     TCAddresses,
     TCHighMask,
     TCLowMask,
     TCOps,
@@ -34,14 +35,87 @@
 from edgepi.tc.tc_faults import map_fault_status
 from edgepi.reg_helper.reg_helper import OpCode, apply_opcodes
 from edgepi.utilities.utilities import filter_dict
 from edgepi.tc.tc_conv_time import calc_conv_time
 
 _logger = logging.getLogger(__name__)
 
+# pylint: disable=too-many-instance-attributes
+class TCState:
+    """
+    A Class to store TC state
+    """
+    def __init__(self):
+        # cmode = True = auto conv mode
+        self.cmode = None
+        # one_shot = True = single shot
+        self.one_shot = None
+        self.open_circuit_fault = None
+        # cj = True = disabled
+        self.cold_junction = None
+        # fault = True = interrupt mode
+        self.fault = None
+        self.fault_clr = None
+        # noise_rejection = true = 50Hz
+        self.noise_rejection = None
+        self.sampling_average = None
+        self.tc_type = None
+
+    def __tc_get_state_bool(self, cr_reg: int, mask:int):
+        """
+        Populate the state value using the cr_regs
+        Args:
+            cr_reg (int): value of one of configuration register either CR0 | CR1
+            bitmask (int): bit mask
+        Return:
+            Bool
+        """
+        return (cr_reg & mask) == mask
+
+    def __tc_get_state(self, cr_reg: int, mask: int):
+        """
+        Populate thes state value using the cr_regs
+        Args:
+            cr_reg (int): value of one of configuration register either CR0 | CR1
+            bitmask (int): bit mask
+        Return:
+            int
+        """
+        reg_val = cr_reg&mask
+        if mask == Masks.CR1_HIGH_MASK.value:
+            state = TCType.get_tc_type(reg_val=reg_val)
+        else:
+            state = AvgMode.get_avg_mode(reg_val=reg_val)
+        return state
+
+    def tc_update_state(self, cr_regs: list):
+        """
+        Update configurations using configuration registers
+        """
+        # cmode = True = auto conv mode
+        self.cmode = self.__tc_get_state_bool(cr_regs[0], ConvMode.AUTO.value.op_code)
+        # one_shot = True = single shot
+        self.one_shot = self.__tc_get_state_bool(cr_regs[0], TCOps.SINGLE_SHOT.value.op_code)
+        self.open_circuit_fault = None
+        # cj = True = disabled
+        self.cold_junction = self.__tc_get_state_bool(cr_regs[0], CJMode.DISABLE.value.op_code)
+        # fault = True = interrupt mode
+        self.fault = self.__tc_get_state_bool(cr_regs[0], FaultMode.INTERRUPT.value.op_code)
+        self.fault_clr = None
+        # noise_rejection = true = 50Hz
+        self.noise_rejection = self.__tc_get_state_bool(cr_regs[0],
+                                                        NoiseFilterMode.HZ_50.value.op_code)
+        # sampling_average = 0x00 =1sample,
+        #                    0x10 = 2 samples,
+        #                    0x20 = 4 samples,
+        #                    0x30 = 8 samples,
+        #                    0x40 = 16 samples
+        self.sampling_average = self.__tc_get_state(cr_regs[1], Masks.CR1_LOW_MASK.value)
+        #TC_TYPE = 0->7 = B->E->J->K->N->R->S->T
+        self.tc_type = self.__tc_get_state(cr_regs[1], Masks.CR1_HIGH_MASK.value)
 
 class EdgePiTC(SpiDevice):
     """
     A class used to represent the EdgePi Thermocouple as an SPI device.
     """
 
     # default MAX31856 register values for writeable registers
@@ -58,14 +132,15 @@
         TCAddresses.CJTO_W.value: 0x00,
         TCAddresses.CJTH_W.value: 0x00,
         TCAddresses.CJTL_W.value: 0x00,
     }
 
     def __init__(self):
         super().__init__(bus_num=6, dev_id=2)
+        self.tc_state = TCState()
 
     def read_temperatures(self):
         """Use to read cold junction and linearized thermocouple temperature measurements"""
         temp_bytes = self.__read_registers(TCAddresses.CJTH_R.value, 5)
         return code_to_temp(temp_bytes)
 
     def single_sample(self, safe_delay: bool = True):
@@ -175,15 +250,14 @@
             reg_addx (TCAddress.Enum.value): the register's address
 
         Returns:
             a list containing two entries:
             new_data[0] = register address, new_data[1] = register value
         """
         data = [reg_addx] + [0xFF]
-        _logger.debug(f"__read_register: addx = {reg_addx} => data before xfer = {data}")
         new_data = self.transfer(data)
         _logger.debug(f"__read_register: addx = {reg_addx} => data after xfer = {new_data}")
         return new_data
 
     def __read_registers(self, start_addx: int = 0, regs_to_read: int = 16):
         """read a variable number of registers sequentially
 
@@ -192,31 +266,29 @@
             regs_to_read (int): number of registers to read, including starting register.
 
         Returns:
             a list containing register values starting from start_addx. Note, first entry
             is the start address: register values begin from the second entry.
         """
         data = [start_addx] + [0xFF] * regs_to_read
-        _logger.debug(f"__read_registers: shifting in data => {data}")
         new_data = self.transfer(data)
         _logger.debug(f"__read_registers: shifted out data => {new_data}")
         return new_data
 
     def __write_to_register(self, reg_addx: int, value: int):
         """write a value to a register.
 
         Args:
             reg_addx (TCAddress.Enum.value): address of the register to write the value to.
 
             value (int): a values to be written to the register.
         """
         data = [reg_addx] + [value]
         _logger.debug(f"__write_to_registers: shifting in data => {data}")
-        new_data = self.transfer(data)
-        _logger.debug(f"__write_to_registers: shifted out data => {new_data}")
+        self.transfer(data)
 
     def __read_registers_to_map(self):
         """
         Builds a map of write register address to corresponding read register value.
         Note, each register has a read and write address, but only the read address
         contains the register's value. Write addresses are only for writing.
 
@@ -245,25 +317,24 @@
                                 entry is a dictionary holding 'value' and 'is_changed' keys.
         """
         for reg_addx, entry in reg_values.items():
             if entry["is_changed"]:
                 updated_value = entry["value"]
                 self.__write_to_register(reg_addx, updated_value)
                 _logger.debug(
-                    f"""register value at address ({hex(reg_addx)})
-                     has been updated to ({hex(updated_value)})"""
-                )
+                    f"register value at address ({hex(reg_addx)})"
+                    f" has been updated to ({hex(updated_value)})")
 
     def __get_tc_type(self):
         """Returns the currently configured thermocouple type"""
         cr1 = Bits(uint=self.__read_register(TCAddresses.CR1_R.value)[1], length=8)
         tc_bits = cr1[-4:].uint
-        for enum in TCType:
-            if enum.value.op_code == tc_bits:
-                return enum
+        for tc in TCType:
+            if not isinstance(tc.value, int) and tc.value.op_code == tc_bits:
+                return tc
         return None
 
     def __get_cj_status(self):
         "Returns the current cold-junction sensing status (on/off)"
         cr0 = Bits(uint=self.__read_register(TCAddresses.CR0_R.value)[1], length=8)
         return cr0[4]
 
@@ -433,15 +504,15 @@
 
                 cj_temp_decimals (DecBits6): set decimal value for cj_temp
         """
         # pylint: disable=unused-argument
 
         # filter out self from args
         args_dict = filter_dict(locals(), "self", None)
-        _logger.debug(f"set_config: args dict:\n\n {args_dict}\n\n")
+        _logger.debug(f"set_config: args dict:\n {args_dict}")
 
         # extract non-temperature setting opcodes from Enums
         ops_list = [
             entry.value
             for entry in args_dict.values()
             if issubclass(entry.__class__, Enum) and isinstance(entry.value, OpCode)
         ]
@@ -460,15 +531,29 @@
             tc_type,
             ops_list,
         )
 
         # read value of every write register into dict, starting from CR0_W.
         # Tuples are (write register addx : register_value) pairs.
         reg_values = self.__read_registers_to_map()
-        _logger.debug(f"set_config: register values before updates:\n\n{reg_values}\n\n")
+        _logger.debug(f"set_config: register values before updates:\n{reg_values}")
 
         # updated register values
         apply_opcodes(reg_values, ops_list)
-        _logger.debug(f"set_config: register values after updates:\n\n{reg_values}\n\n")
+        _logger.debug(f"set_config: register values after updates:\n\n{reg_values}")
 
         # only update registers whose values have been changed
         self.__update_registers_from_dict(reg_values)
+
+        # Update configuration state
+        self.get_state()
+
+    def get_state(self):
+        """
+        Read config registers and update state object
+        Args:
+            N/A
+        Retuern:
+            N/A
+        """
+        cr_regs = self.__read_registers(TCAddresses.CR0_R.value, 2)
+        self.tc_state.tc_update_state(cr_regs[1:])
```

### Comparing `edgepi-python-sdk-1.1.7/src/edgepi/tc/tc_commands.py` & `edgepi-python-sdk-1.2.1/src/edgepi/tc/tc_commands.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.1.7/src/edgepi/tc/tc_constants.py` & `edgepi-python-sdk-1.2.1/src/edgepi/tc/tc_constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -259,28 +259,78 @@
 
     AVG_1 = OpCode(0x00, TCAddresses.CR1_W.value, Masks.CR1_HIGH_MASK.value)  # single sample
     AVG_2 = OpCode(0x10, TCAddresses.CR1_W.value, Masks.CR1_HIGH_MASK.value)  # 2 samples averaged
     AVG_4 = OpCode(0x20, TCAddresses.CR1_W.value, Masks.CR1_HIGH_MASK.value)  # 4 samples averaged
     AVG_8 = OpCode(0x30, TCAddresses.CR1_W.value, Masks.CR1_HIGH_MASK.value)  # 8 samples averaged
     AVG_16 = OpCode(0x40, TCAddresses.CR1_W.value, Masks.CR1_HIGH_MASK.value)  # 16 samples averaged
 
+    @staticmethod
+    def get_avg_mode(reg_val: int):
+        """
+        get the sampling average mode config enum by checking register value passed
+        Args:
+            reg_val (int): masked register value passed
+        Return:
+            avg_mode (Eum): avg_mode Enum value
+        """
+        if reg_val == 0:
+            avg_mode = AvgMode.AVG_1
+        elif reg_val == 16:
+            avg_mode = AvgMode.AVG_2
+        elif reg_val == 32:
+            avg_mode = AvgMode.AVG_4
+        elif reg_val == 48:
+            avg_mode = AvgMode.AVG_8
+        elif reg_val == 64:
+            avg_mode = AvgMode.AVG_16
+        else:
+            avg_mode = None
+        return avg_mode
 
 @unique
 class TCType(Enum):
     """valid opcodes for setting thermocouple type"""
 
     TYPE_B = OpCode(0x00, TCAddresses.CR1_W.value, Masks.CR1_LOW_MASK.value)  # type B thermocouple
     TYPE_E = OpCode(0x01, TCAddresses.CR1_W.value, Masks.CR1_LOW_MASK.value)  # type E thermocouple
     TYPE_J = OpCode(0x02, TCAddresses.CR1_W.value, Masks.CR1_LOW_MASK.value)  # type J thermocouple
     TYPE_K = OpCode(0x03, TCAddresses.CR1_W.value, Masks.CR1_LOW_MASK.value)  # type K thermocouple
     TYPE_N = OpCode(0x04, TCAddresses.CR1_W.value, Masks.CR1_LOW_MASK.value)  # type N thermocouple
     TYPE_R = OpCode(0x05, TCAddresses.CR1_W.value, Masks.CR1_LOW_MASK.value)  # type R thermocouple
     TYPE_S = OpCode(0x06, TCAddresses.CR1_W.value, Masks.CR1_LOW_MASK.value)  # type S thermocouple
     TYPE_T = OpCode(0x07, TCAddresses.CR1_W.value, Masks.CR1_LOW_MASK.value)  # type T thermocouple
 
+    @staticmethod
+    def get_tc_type(reg_val: int):
+        """
+        get the thermocouple type config enum by checking register value passed
+        Args:
+            reg_val (int): masked register value passed
+        Return:
+            tc_type (Eum): TC_type Enum value
+        """
+        if reg_val == 0:
+            tc_type = TCType.TYPE_B
+        elif reg_val == 1:
+            tc_type = TCType.TYPE_E
+        elif reg_val == 2:
+            tc_type = TCType.TYPE_J
+        elif reg_val == 3:
+            tc_type = TCType.TYPE_K
+        elif reg_val == 4:
+            tc_type = TCType.TYPE_N
+        elif reg_val == 5:
+            tc_type = TCType.TYPE_R
+        elif reg_val == 6:
+            tc_type = TCType.TYPE_S
+        elif reg_val == 7:
+            tc_type = TCType.TYPE_T
+        else:
+            tc_type = None
+        return tc_type
 
 class VoltageMode(Enum):
     """
     valid opcodes for setting thermocouple voltage mode. Use to set
     thermocouple type other than those listed under TCType.
     Note, When voltage mode is selected, no linearization is
     performed on the conversion data. Use the voltage data
```

### Comparing `edgepi-python-sdk-1.1.7/src/edgepi/tc/tc_conv_time.py` & `edgepi-python-sdk-1.2.1/src/edgepi/tc/tc_conv_time.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.1.7/src/edgepi/tc/tc_faults.py` & `edgepi-python-sdk-1.2.1/src/edgepi/tc/tc_faults.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.1.7/src/edgepi/utilities/utilities.py` & `edgepi-python-sdk-1.2.1/src/edgepi/utilities/utilities.py`

 * *Files 17% similar despite different names*

```diff
@@ -24,14 +24,35 @@
         key or value matches either the entry_key or entry_val, respectively.
     """
     filtered_args = {
         key: value for (key, value) in dictionary.items() if key != entry_key and value != entry_val
     }
     return filtered_args
 
+def filter_dict_list_key_val(dictionary: dict, entry_key: list, entry_val:list) -> dict:
+    """use for filtering an entry from a dictionary by key or value
+
+    Args:
+        dictionary (dict): any dictionary whose entries are to be filtered
+
+        entry_key (list): list of the key of the entry to filter out
+
+        entry_val (list): list of the value of the entry or entries to filter out
+
+    Returns:
+        a dictionary of entries from the original dictionary, after filtering out entries whose
+        key or value matches either the entry_key or entry_val, respectively.
+    """
+    filtered_args = {
+        key: value for (key, value) in dictionary.items() \
+        if key not in entry_key and value not in entry_val
+    }
+    return filtered_args
+
+
 
 def bitstring_from_list(data: list) -> BitArray:
     """
     Builds a bitstring from a list of uint byte values
 
     Args:
         data (List[int]): a list of uint byte values
```

### Comparing `edgepi-python-sdk-1.1.7/src/edgepi_python_sdk.egg-info/PKG-INFO` & `edgepi-python-sdk-1.2.1/src/edgepi_python_sdk.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgepi-python-sdk
-Version: 1.1.7
+Version: 1.2.1
 Summary: EdgePi Python SDK package
 Home-page: https://github.com/EdgePi-Cloud/edgepi-python-sdk
 Author: S.Park
 Author-email: spark@osensa.com
 Project-URL: Bug Tracker, https://github.com/EdgePi-Cloud/edgepi-python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -30,56 +30,58 @@
 
 ```
 $ python3 -m pip install edgepi-python-sdk
 ```
 ## Example Code
 The EdgePi SDK provides a wide range of functionality to users, allowing interaction with the many modules onboard the EdgePi. One such module, the ADC, can be used to read voltage continuously from any of the eight EdgePi analog input pins:
 
-```
-from edgepi.adc.edgepi_adc import EdgePiADC
-from edgepi.adc.adc_constants import ADCChannel, ConvMode, ADCNum
+```python
+from edgepi.dac.edgepi_adc import EdgePiADC
+from edgepi.adc.adc_constants import ADCChannel, ConvMode
 
 # initialize ADC
 edgepi_adc = EdgePiADC()
 
-# configure ADC to sample analog input pin AIN3
+# configure ADC to sample input pin 4 (the input pins are 0-indexed)
 edgepi_adc.set_config(adc_1_analog_in=ADCChannel.AIN3, conversion_mode=ConvMode.CONTINUOUS)
 
-# send command to start continuous conversions
-edgepi_adc.start_conversions(ADCNum.ADC_1)
+# send command to start automatic conversions
+edgepi_adc.start_conversions()
 
 # perform 10 voltage reads
 for _ in range(10):
-  out = edgepi_adc.read_voltage(ADCNum.ADC_1)
+  out = edgepi_adc.read_voltage()
   print(out)
   
-# stop continuous conversions
-edgepi_adc.stop_conversions(ADCNum.ADC_1)
+# stop automatic conversions
+edgepi_adc.stop_conversions()
 ```
 For further details on this and other modules, please refer to each module's documentation by following the links provided in the `Implemented Modules` section below.
 # Implemented Modules
 The EdgePi SDK contains modules intended to represent each connected peripheral device onboard the EdgePi. Below is a directory of the currently available modules.
-* [Thermocouple](src/edgepi/tc)
-* [Digital to Analog Converter (DAC)](src/edgepi/dac)
-* [Analog to Digital Converter (ADC)](src/edgepi/adc)
-* [LED Array](src/edgepi/led)
-* [Digital In (DIN)](src/edgepi/din)
-* [Digital Out (DOUT)](src/edgepi/dout)
+* [Thermocouple](https://github.com/EdgePi-Cloud/edgepi-python-sdk/tree/main/src/edgepi/tc)
+* [Digital to Analog Converter (DAC)](https://github.com/EdgePi-Cloud/edgepi-python-sdk/tree/main/src/edgepi/dac)
+* [Analog to Digital Converter (ADC)](https://github.com/EdgePi-Cloud/edgepi-python-sdk/tree/main/src/edgepi/adc)
+* [LED Array](https://github.com/EdgePi-Cloud/edgepi-python-sdk/tree/main/src/edgepi/led)
+* [Digital Input (DIN)](https://github.com/EdgePi-Cloud/edgepi-python-sdk/tree/main/src/edgepi/digital_input)
+* [Digital Output (DOUT)](https://github.com/EdgePi-Cloud/edgepi-python-sdk/tree/main/src/edgepi/digital_output)
 # Development
 Active development SDK versions can be accessed from the following resources:
 ## Installing from TestPyPi
 To install the most recent active development SDK version via [TestPyPi](https://test.pypi.org/project/edgepi-python-sdk/):
 ```
-$ python3 -m pip install -i https://test.pypi.org/simple/ edgepi-python-sdk
+
+$ python3 -m pip install -i https://test.pypi.org/simple/edgepi-python-sdk
 ```
 Previous development SDK versions can also be installed by specifiying the version number:
 ```
-$ python3 -m pip install -i https://test.pypi.org/simple/ edgepi-python-sdk==<version-number>
+$ python3 -m pip install -i https://test.pypi.org/simple/edgepi-python-sdk==<version-number>
 ```
 Please refer to [TestPyPi](https://test.pypi.org/project/edgepi-python-sdk/) for available SDK versions.
+
 ## Installing from GitHub
 To install the SDK via HTTPS from GitHub:
 ```
 $ python3 -m pip install git+https://github.com/EdgePi-Cloud/edgepi-python-sdk.git@<branch-name>
 ```
 
 # Packaging
```

### Comparing `edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_adc/test_adc_commands.py` & `edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_adc/test_adc_commands.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_adc/test_adc_conv_time.py` & `edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_adc/test_adc_conv_time.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 import pytest
 from edgepi.adc.adc_conv_time import (
     expected_initial_time_delay,
     expected_continuous_time_delay,
     ADC1_CONT_DELAYS,
     ADC1_INITIAL_DELAYS,
-    ADC2_DELAYS,
+    ADC2_CONT_DELAYS,
+    ADC2_INITIAL_DELAYS,
 )
 from edgepi.adc.adc_constants import (
     FilterMode as FILT,
     ADC1DataRate as DR1,
     ADC2DataRate as DR2,
     ADCNum,
 )
@@ -501,137 +502,137 @@
             ADC1_INITIAL_DELAYS[DR1.SPS_38400.value.op_code][FILT.FIR.value.op_code],
         ),
         # ADC2
         (
             ADCNum.ADC_2,
             DR2.SPS_10.value.op_code,
             FILT.SINC1.value.op_code,
-            ADC2_DELAYS[DR2.SPS_10.value.op_code],
+            ADC2_INITIAL_DELAYS[DR2.SPS_10.value.op_code],
         ),
         (
             ADCNum.ADC_2,
             DR2.SPS_10.value.op_code,
             FILT.SINC2.value.op_code,
-            ADC2_DELAYS[DR2.SPS_10.value.op_code],
+            ADC2_INITIAL_DELAYS[DR2.SPS_10.value.op_code],
         ),
         (
             ADCNum.ADC_2,
             DR2.SPS_10.value.op_code,
             FILT.SINC3.value.op_code,
-            ADC2_DELAYS[DR2.SPS_10.value.op_code],
+            ADC2_INITIAL_DELAYS[DR2.SPS_10.value.op_code],
         ),
         (
             ADCNum.ADC_2,
             DR2.SPS_10.value.op_code,
             FILT.SINC4.value.op_code,
-            ADC2_DELAYS[DR2.SPS_10.value.op_code],
+            ADC2_INITIAL_DELAYS[DR2.SPS_10.value.op_code],
         ),
         (
             ADCNum.ADC_2,
             DR2.SPS_10.value.op_code,
             FILT.FIR.value.op_code,
-            ADC2_DELAYS[DR2.SPS_10.value.op_code],
+            ADC2_INITIAL_DELAYS[DR2.SPS_10.value.op_code],
         ),
         (
             ADCNum.ADC_2,
             DR2.SPS_100.value.op_code,
             FILT.SINC1.value.op_code,
-            ADC2_DELAYS[DR2.SPS_100.value.op_code],
+            ADC2_INITIAL_DELAYS[DR2.SPS_100.value.op_code],
         ),
         (
             ADCNum.ADC_2,
             DR2.SPS_100.value.op_code,
             FILT.SINC2.value.op_code,
-            ADC2_DELAYS[DR2.SPS_100.value.op_code],
+            ADC2_INITIAL_DELAYS[DR2.SPS_100.value.op_code],
         ),
         (
             ADCNum.ADC_2,
             DR2.SPS_100.value.op_code,
             FILT.SINC3.value.op_code,
-            ADC2_DELAYS[DR2.SPS_100.value.op_code],
+            ADC2_INITIAL_DELAYS[DR2.SPS_100.value.op_code],
         ),
         (
             ADCNum.ADC_2,
             DR2.SPS_100.value.op_code,
             FILT.SINC4.value.op_code,
-            ADC2_DELAYS[DR2.SPS_100.value.op_code],
+            ADC2_INITIAL_DELAYS[DR2.SPS_100.value.op_code],
         ),
         (
             ADCNum.ADC_2,
             DR2.SPS_100.value.op_code,
             FILT.FIR.value.op_code,
-            ADC2_DELAYS[DR2.SPS_100.value.op_code],
+            ADC2_INITIAL_DELAYS[DR2.SPS_100.value.op_code],
         ),
         (
             ADCNum.ADC_2,
             DR2.SPS_400.value.op_code,
             FILT.SINC1.value.op_code,
-            ADC2_DELAYS[DR2.SPS_400.value.op_code],
+            ADC2_INITIAL_DELAYS[DR2.SPS_400.value.op_code],
         ),
         (
             ADCNum.ADC_2,
             DR2.SPS_400.value.op_code,
             FILT.SINC2.value.op_code,
-            ADC2_DELAYS[DR2.SPS_400.value.op_code],
+            ADC2_INITIAL_DELAYS[DR2.SPS_400.value.op_code],
         ),
         (
             ADCNum.ADC_2,
             DR2.SPS_400.value.op_code,
             FILT.SINC3.value.op_code,
-            ADC2_DELAYS[DR2.SPS_400.value.op_code],
+            ADC2_INITIAL_DELAYS[DR2.SPS_400.value.op_code],
         ),
         (
             ADCNum.ADC_2,
             DR2.SPS_400.value.op_code,
             FILT.SINC4.value.op_code,
-            ADC2_DELAYS[DR2.SPS_400.value.op_code],
+            ADC2_INITIAL_DELAYS[DR2.SPS_400.value.op_code],
         ),
         (
             ADCNum.ADC_2,
             DR2.SPS_400.value.op_code,
             FILT.FIR.value.op_code,
-            ADC2_DELAYS[DR2.SPS_400.value.op_code],
+            ADC2_INITIAL_DELAYS[DR2.SPS_400.value.op_code],
         ),
         (
             ADCNum.ADC_2,
             DR2.SPS_800.value.op_code,
             FILT.SINC1.value.op_code,
-            ADC2_DELAYS[DR2.SPS_800.value.op_code],
+            ADC2_INITIAL_DELAYS[DR2.SPS_800.value.op_code],
         ),
         (
             ADCNum.ADC_2,
             DR2.SPS_800.value.op_code,
             FILT.SINC2.value.op_code,
-            ADC2_DELAYS[DR2.SPS_800.value.op_code],
+            ADC2_INITIAL_DELAYS[DR2.SPS_800.value.op_code],
         ),
         (
             ADCNum.ADC_2,
             DR2.SPS_800.value.op_code,
             FILT.SINC3.value.op_code,
-            ADC2_DELAYS[DR2.SPS_800.value.op_code],
+            ADC2_INITIAL_DELAYS[DR2.SPS_800.value.op_code],
         ),
         (
             ADCNum.ADC_2,
             DR2.SPS_800.value.op_code,
             FILT.SINC4.value.op_code,
-            ADC2_DELAYS[DR2.SPS_800.value.op_code],
+            ADC2_INITIAL_DELAYS[DR2.SPS_800.value.op_code],
         ),
         (
             ADCNum.ADC_2,
             DR2.SPS_800.value.op_code,
             FILT.FIR.value.op_code,
-            ADC2_DELAYS[DR2.SPS_800.value.op_code],
+            ADC2_INITIAL_DELAYS[DR2.SPS_800.value.op_code],
         ),
     ],
 )
 def test_compute_initial_time_delay(adc_num, data_rate, filter_mode, expected):
     if adc_num == ADCNum.ADC_1:
         assert expected_initial_time_delay(adc_num, data_rate, filter_mode) == expected
     else:
-        assert expected_initial_time_delay(adc_num, data_rate, filter_mode) == expected * 3
+        assert expected_initial_time_delay(adc_num, data_rate, filter_mode) == expected
 
 
 @pytest.mark.parametrize(
     "adc_num, data_rate, expected",
     [
         # ADC1 CONTINUOUS MODE
         (
@@ -714,28 +715,28 @@
             DR1.SPS_38400.value.op_code,
             ADC1_CONT_DELAYS[DR1.SPS_38400.value.op_code],
         ),
         # ADC2
         (
             ADCNum.ADC_2,
             DR2.SPS_10.value.op_code,
-            ADC2_DELAYS[DR2.SPS_10.value.op_code],
+            ADC2_CONT_DELAYS[DR2.SPS_10.value.op_code],
         ),
         (
             ADCNum.ADC_2,
             DR2.SPS_100.value.op_code,
-            ADC2_DELAYS[DR2.SPS_100.value.op_code],
+            ADC2_CONT_DELAYS[DR2.SPS_100.value.op_code],
         ),
         (
             ADCNum.ADC_2,
             DR2.SPS_400.value.op_code,
-            ADC2_DELAYS[DR2.SPS_400.value.op_code],
+            ADC2_CONT_DELAYS[DR2.SPS_400.value.op_code],
         ),
         (
             ADCNum.ADC_2,
             DR2.SPS_800.value.op_code,
-            ADC2_DELAYS[DR2.SPS_800.value.op_code],
+            ADC2_CONT_DELAYS[DR2.SPS_800.value.op_code],
         ),
     ],
 )
 def test_compute_continuous_time_delay_adc_1(adc_num, data_rate, expected):
     assert expected_continuous_time_delay(adc_num, data_rate) == expected
```

### Comparing `edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_adc/test_adc_multiplexers.py` & `edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_adc/test_adc_multiplexers.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_adc/test_adc_state.py` & `edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_adc/test_adc_state.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,27 +5,28 @@
 import sys
 import pytest
 
 sys.modules['periphery'] = mock.MagicMock()
 
 # pylint: disable=wrong-import-position
 # mocked periphery module needs to be placed above
-from edgepi.adc.edgepi_adc import ADCState
+from edgepi.adc.adc_state import ADCState
 from edgepi.adc.adc_query_lang import ADCProperties
 from edgepi.adc.adc_constants import (
     ADC1DataRate,
     ADC2DataRate,
     ADCChannel,
     ADCReg,
     CheckMode,
     ConvMode,
     FilterMode,
     StatusByte,
+    ADCNum,
+    RTDModes
 )
-
 # mock default register values
 ADC_REGS = {
     ADCReg.REG_ID.value: 0x0,
     ADCReg.REG_POWER.value: 0x0,
     ADCReg.REG_INTERFACE.value: 0x0,
     ADCReg.REG_MODE0.value: 0x0,
     ADCReg.REG_MODE1.value: 0x0,
@@ -366,47 +367,445 @@
             ADCProperties.FILTER_MODE.value.values[FilterMode.SINC4.value.op_code],
         ),
         (
             {ADCReg.REG_MODE1.value: 0b10000000},
             "state.filter_mode",
             ADCProperties.FILTER_MODE.value.values[FilterMode.FIR.value.op_code],
         ),
-        # RTD on
+        # RTD OFF
+        (
+            {
+                ADCReg.REG_IDACMUX.value: 0xBB,
+                ADCReg.REG_IDACMAG.value: 0x0,
+                ADCReg.REG_REFMUX.value: 0x0,
+                ADCReg.REG_ADC2CFG.value: 0x0,
+            },
+            "state.rtd_mode",
+            RTDModes.RTD_OFF
+        ),
+        (
+            {
+                ADCReg.REG_IDACMUX.value: 0xBB,
+                ADCReg.REG_IDACMAG.value: 0x0,
+                ADCReg.REG_REFMUX.value: 0x0,
+                ADCReg.REG_ADC2CFG.value: 0x01,
+            },
+            "state.rtd_mode",
+            RTDModes.RTD_OFF
+        ),
+        (
+            {
+                ADCReg.REG_IDACMUX.value: 0xBB,
+                ADCReg.REG_IDACMAG.value: 0x0,
+                ADCReg.REG_REFMUX.value: 0x0,
+                ADCReg.REG_ADC2CFG.value: 0x02,
+            },
+            "state.rtd_mode",
+            RTDModes.RTD_OFF
+        ),
+        (
+            {
+                ADCReg.REG_IDACMUX.value: 0xBB,
+                ADCReg.REG_IDACMAG.value: 0x0,
+                ADCReg.REG_REFMUX.value: 0x0,
+                ADCReg.REG_ADC2CFG.value: 0x03,
+            },
+            "state.rtd_mode",
+            RTDModes.RTD_OFF
+        ),
+        (
+            {
+                ADCReg.REG_IDACMUX.value: 0xBB,
+                ADCReg.REG_IDACMAG.value: 0x0,
+                ADCReg.REG_REFMUX.value: 0x0,
+                ADCReg.REG_ADC2CFG.value: 0x05,
+            },
+            "state.rtd_mode",
+            RTDModes.RTD_OFF
+        ),
+        (
+            {
+                ADCReg.REG_IDACMUX.value: 0xBB,
+                ADCReg.REG_IDACMAG.value: 0x0,
+                ADCReg.REG_REFMUX.value: 0x0,
+                ADCReg.REG_ADC2CFG.value: 0x06,
+            },
+            "state.rtd_mode",
+            RTDModes.RTD_OFF
+        ),
+        (
+            {
+                ADCReg.REG_IDACMUX.value: 0xBB,
+                ADCReg.REG_IDACMAG.value: 0x0,
+                ADCReg.REG_REFMUX.value: 0x0,
+                ADCReg.REG_ADC2CFG.value: 0x07,
+            },
+            "state.rtd_mode",
+            RTDModes.RTD_OFF
+        ),
+        (
+            {
+                ADCReg.REG_IDACMUX.value: 0xBB,
+                ADCReg.REG_IDACMAG.value: 0x0,
+                ADCReg.REG_REFMUX.value: 0x0,
+                ADCReg.REG_ADC2CFG.value: 0x40,
+            },
+            "state.rtd_mode",
+            RTDModes.RTD_OFF
+        ),
+        (
+            {
+                ADCReg.REG_IDACMUX.value: 0xBB,
+                ADCReg.REG_IDACMAG.value: 0x0,
+                ADCReg.REG_REFMUX.value: 0x0,
+                ADCReg.REG_ADC2CFG.value: 0x80,
+            },
+            "state.rtd_mode",
+            RTDModes.RTD_OFF
+        ),
+        # RTD State None
+        (
+            {
+                ADCReg.REG_INPMUX.value: 0x0,
+                ADCReg.REG_IDACMUX.value: 0x98,
+                ADCReg.REG_IDACMAG.value: 0x44,
+                ADCReg.REG_REFMUX.value: 27,
+            },
+            "state.rtd_mode",
+            None
+        ),
+        # RTD ADC1 ON
+        (
+            {
+                ADCReg.REG_INPMUX.value: 0x76,
+                ADCReg.REG_IDACMUX.value: 0x98,
+                ADCReg.REG_IDACMAG.value: 0x44,
+                ADCReg.REG_REFMUX.value: 27,
+            },
+            "state.rtd_mode",
+            RTDModes.RTD_ON
+        ),
+        # RTD ADC2 ON
+        (
+            {
+                ADCReg.REG_ADC2MUX.value: 0x76,
+                ADCReg.REG_IDACMUX.value: 0x98,
+                ADCReg.REG_IDACMAG.value: 0x44,
+                ADCReg.REG_ADC2CFG.value: 24,
+            },
+            "state.rtd_mode",
+            RTDModes.RTD_ON
+        ),
+        (
+            {
+                ADCReg.REG_ADC2MUX.value: 0x76,
+                ADCReg.REG_IDACMUX.value: 0x98,
+                ADCReg.REG_IDACMAG.value: 0x44,
+                ADCReg.REG_ADC2CFG.value: 24+1,
+            },
+            "state.rtd_mode",
+            RTDModes.RTD_ON
+        ),
+        (
+            {
+                ADCReg.REG_ADC2MUX.value: 0x76,
+                ADCReg.REG_IDACMUX.value: 0x98,
+                ADCReg.REG_IDACMAG.value: 0x44,
+                ADCReg.REG_ADC2CFG.value: 24+2,
+            },
+            "state.rtd_mode",
+            RTDModes.RTD_ON
+        ),
+        (
+            {
+                ADCReg.REG_ADC2MUX.value: 0x76,
+                ADCReg.REG_IDACMUX.value: 0x98,
+                ADCReg.REG_IDACMAG.value: 0x44,
+                ADCReg.REG_ADC2CFG.value: 24+3,
+            },
+            "state.rtd_mode",
+            RTDModes.RTD_ON
+        ),
+        (
+            {
+                ADCReg.REG_ADC2MUX.value: 0x76,
+                ADCReg.REG_IDACMUX.value: 0x98,
+                ADCReg.REG_IDACMAG.value: 0x44,
+                ADCReg.REG_ADC2CFG.value: 24+4,
+            },
+            "state.rtd_mode",
+            RTDModes.RTD_ON
+        ),
+        (
+            {
+                ADCReg.REG_ADC2MUX.value: 0x76,
+                ADCReg.REG_IDACMUX.value: 0x98,
+                ADCReg.REG_IDACMAG.value: 0x44,
+                ADCReg.REG_ADC2CFG.value: 24+5,
+            },
+            "state.rtd_mode",
+            RTDModes.RTD_ON
+        ),
+        (
+            {
+                ADCReg.REG_ADC2MUX.value: 0x76,
+                ADCReg.REG_IDACMUX.value: 0x98,
+                ADCReg.REG_IDACMAG.value: 0x44,
+                ADCReg.REG_ADC2CFG.value: 24+6,
+            },
+            "state.rtd_mode",
+            RTDModes.RTD_ON
+        ),
+        (
+            {
+                ADCReg.REG_ADC2MUX.value: 0x76,
+                ADCReg.REG_IDACMUX.value: 0x98,
+                ADCReg.REG_IDACMAG.value: 0x44,
+                ADCReg.REG_ADC2CFG.value: 24+7,
+            },
+            "state.rtd_mode",
+            RTDModes.RTD_ON
+        ),
         (
             {
-                ADCReg.REG_INPMUX.value: 0x56,
+                ADCReg.REG_ADC2MUX.value: 0x76,
                 ADCReg.REG_IDACMUX.value: 0x98,
                 ADCReg.REG_IDACMAG.value: 0x44,
-                ADCReg.REG_REFMUX.value: 0b00011100,
+                ADCReg.REG_ADC2CFG.value: 24+64,
             },
-            "state.rtd_on",
-            True
+            "state.rtd_mode",
+            RTDModes.RTD_ON
+        ),
+        (
+            {
+                ADCReg.REG_ADC2MUX.value: 0x76,
+                ADCReg.REG_IDACMUX.value: 0x98,
+                ADCReg.REG_IDACMAG.value: 0x44,
+                ADCReg.REG_ADC2CFG.value: 24+128,
+            },
+            "state.rtd_mode",
+            RTDModes.RTD_ON
+        ),
+
+
+        # Check ADC number for RTD None
+        (
+            {
+                ADCReg.REG_IDACMUX.value: 0xBB,
+                ADCReg.REG_IDACMAG.value: 0x0,
+                ADCReg.REG_REFMUX.value: 0x0,
+                ADCReg.REG_ADC2CFG.value: 0x0,
+            },
+            "state.rtd_adc",
+            None
+        ),
+        (
+            {
+                ADCReg.REG_IDACMUX.value: 0xBB,
+                ADCReg.REG_IDACMAG.value: 0x0,
+                ADCReg.REG_REFMUX.value: 0x0,
+                ADCReg.REG_ADC2CFG.value: 0x01,
+            },
+            "state.rtd_adc",
+            None
+        ),
+        (
+            {
+                ADCReg.REG_IDACMUX.value: 0xBB,
+                ADCReg.REG_IDACMAG.value: 0x0,
+                ADCReg.REG_REFMUX.value: 0x0,
+                ADCReg.REG_ADC2CFG.value: 0x02,
+            },
+            "state.rtd_adc",
+            None
+        ),
+        (
+            {
+                ADCReg.REG_IDACMUX.value: 0xBB,
+                ADCReg.REG_IDACMAG.value: 0x0,
+                ADCReg.REG_REFMUX.value: 0x0,
+                ADCReg.REG_ADC2CFG.value: 0x03,
+            },
+            "state.rtd_adc",
+            None
+        ),
+        (
+            {
+                ADCReg.REG_IDACMUX.value: 0xBB,
+                ADCReg.REG_IDACMAG.value: 0x0,
+                ADCReg.REG_REFMUX.value: 0x0,
+                ADCReg.REG_ADC2CFG.value: 0x05,
+            },
+            "state.rtd_adc",
+            None
+        ),
+        (
+            {
+                ADCReg.REG_IDACMUX.value: 0xBB,
+                ADCReg.REG_IDACMAG.value: 0x0,
+                ADCReg.REG_REFMUX.value: 0x0,
+                ADCReg.REG_ADC2CFG.value: 0x06,
+            },
+            "state.rtd_adc",
+            None
+        ),
+        (
+            {
+                ADCReg.REG_IDACMUX.value: 0xBB,
+                ADCReg.REG_IDACMAG.value: 0x0,
+                ADCReg.REG_REFMUX.value: 0x0,
+                ADCReg.REG_ADC2CFG.value: 0x07,
+            },
+            "state.rtd_adc",
+            None
+        ),
+        (
+            {
+                ADCReg.REG_IDACMUX.value: 0xBB,
+                ADCReg.REG_IDACMAG.value: 0x0,
+                ADCReg.REG_REFMUX.value: 0x0,
+                ADCReg.REG_ADC2CFG.value: 0x40,
+            },
+            "state.rtd_adc",
+            None
         ),
-        # RTD off
         (
             {
-                ADCReg.REG_INPMUX.value: 0xFA,
                 ADCReg.REG_IDACMUX.value: 0xBB,
-                ADCReg.REG_IDACMAG.value: 0x00,
-                ADCReg.REG_REFMUX.value: 0x00,
+                ADCReg.REG_IDACMAG.value: 0x0,
+                ADCReg.REG_REFMUX.value: 0x0,
+                ADCReg.REG_ADC2CFG.value: 0x80,
             },
-            "state.rtd_on",
-            False
+            "state.rtd_adc",
+            None
         ),
-        # RTD improperly configured
         (
             {
-                ADCReg.REG_INPMUX.value: 0x56,
+                ADCReg.REG_INPMUX.value: 0x0,
                 ADCReg.REG_IDACMUX.value: 0x98,
-                ADCReg.REG_IDACMAG.value: 0x48,
-                ADCReg.REG_REFMUX.value: 0b00011100,
+                ADCReg.REG_IDACMAG.value: 0x44,
+                ADCReg.REG_REFMUX.value: 27,
+            },
+            "state.rtd_adc",
+            None
+        ),
+        # Check ADC number for RTD ADC1
+        (
+            {
+                ADCReg.REG_INPMUX.value: 0x76,
+                ADCReg.REG_IDACMUX.value: 0x98,
+                ADCReg.REG_IDACMAG.value: 0x44,
+                ADCReg.REG_REFMUX.value: 27,
             },
-            "state.rtd_on",
-            False
+            "state.rtd_adc",
+            ADCNum.ADC_1
         ),
+        # Check ADC number for RTD ADC2
+        (
+            {
+                ADCReg.REG_ADC2MUX.value: 0x76,
+                ADCReg.REG_IDACMUX.value: 0x98,
+                ADCReg.REG_IDACMAG.value: 0x44,
+                ADCReg.REG_ADC2CFG.value: 24,
+            },
+            "state.rtd_adc",
+            ADCNum.ADC_2
+        ),
+        (
+            {
+                ADCReg.REG_ADC2MUX.value: 0x76,
+                ADCReg.REG_IDACMUX.value: 0x98,
+                ADCReg.REG_IDACMAG.value: 0x44,
+                ADCReg.REG_ADC2CFG.value: 24+1,
+            },
+            "state.rtd_adc",
+            ADCNum.ADC_2
+        ),
+        (
+            {
+                ADCReg.REG_ADC2MUX.value: 0x76,
+                ADCReg.REG_IDACMUX.value: 0x98,
+                ADCReg.REG_IDACMAG.value: 0x44,
+                ADCReg.REG_ADC2CFG.value: 24+2,
+            },
+            "state.rtd_adc",
+            ADCNum.ADC_2
+        ),
+        (
+            {
+                ADCReg.REG_ADC2MUX.value: 0x76,
+                ADCReg.REG_IDACMUX.value: 0x98,
+                ADCReg.REG_IDACMAG.value: 0x44,
+                ADCReg.REG_ADC2CFG.value: 24+3,
+            },
+            "state.rtd_adc",
+            ADCNum.ADC_2
+        ),
+        (
+            {
+                ADCReg.REG_ADC2MUX.value: 0x76,
+                ADCReg.REG_IDACMUX.value: 0x98,
+                ADCReg.REG_IDACMAG.value: 0x44,
+                ADCReg.REG_ADC2CFG.value: 24+4,
+            },
+            "state.rtd_adc",
+            ADCNum.ADC_2
+        ),
+        (
+            {
+                ADCReg.REG_ADC2MUX.value: 0x76,
+                ADCReg.REG_IDACMUX.value: 0x98,
+                ADCReg.REG_IDACMAG.value: 0x44,
+                ADCReg.REG_ADC2CFG.value: 24+5,
+            },
+            "state.rtd_adc",
+            ADCNum.ADC_2
+        ),
+        (
+            {
+                ADCReg.REG_ADC2MUX.value: 0x76,
+                ADCReg.REG_IDACMUX.value: 0x98,
+                ADCReg.REG_IDACMAG.value: 0x44,
+                ADCReg.REG_ADC2CFG.value: 24+6,
+            },
+            "state.rtd_adc",
+            ADCNum.ADC_2
+        ),
+        (
+            {
+                ADCReg.REG_ADC2MUX.value: 0x76,
+                ADCReg.REG_IDACMUX.value: 0x98,
+                ADCReg.REG_IDACMAG.value: 0x44,
+                ADCReg.REG_ADC2CFG.value: 24+7,
+            },
+            "state.rtd_adc",
+            ADCNum.ADC_2
+        ),
+        (
+            {
+                ADCReg.REG_ADC2MUX.value: 0x76,
+                ADCReg.REG_IDACMUX.value: 0x98,
+                ADCReg.REG_IDACMAG.value: 0x44,
+                ADCReg.REG_ADC2CFG.value: 24+64,
+            },
+            "state.rtd_adc",
+            ADCNum.ADC_2
+        ),
+        (
+            {
+                ADCReg.REG_ADC2MUX.value: 0x76,
+                ADCReg.REG_IDACMUX.value: 0x98,
+                ADCReg.REG_IDACMAG.value: 0x44,
+                ADCReg.REG_ADC2CFG.value: 24+128,
+            },
+            "state.rtd_adc",
+            ADCNum.ADC_2
+        ),
+
+
         # ADC1 Data Rate
         (
             {ADCReg.REG_MODE2.value: 0x00},
             "state.adc_1.data_rate",
             ADCProperties.DATA_RATE_1.value.values[ADC1DataRate.SPS_2P5.value.op_code],
         ),
         (
@@ -501,15 +900,15 @@
             ADCProperties.DATA_RATE_2.value.values[ADC2DataRate.SPS_400.value.op_code],
         ),
         (
             {ADCReg.REG_ADC2CFG.value: 0xC0},
             "state.adc_2.data_rate",
             ADCProperties.DATA_RATE_2.value.values[ADC2DataRate.SPS_800.value.op_code],
         ),
-    ],
+    ]
 )
 def test_adc_state_init(updates, state_property, expected):
     reg_map = deepcopy(ADC_REGS)
     _apply_register_updates(reg_map, updates)
     # pylint: disable=eval-used, unused-variable
     # using eval to access nested attributes of state with dot notation
     state = ADCState(reg_map)
```

### Comparing `edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_adc/test_adc_status.py` & `edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_adc/test_adc_status.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_adc/test_adc_voltage.py` & `edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_utilities/test_crc_8_atm.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,53 +1,21 @@
-"""Unit tests for adc_voltage.py module"""
-
+"""Unit tests for crc_8_atm.py"""
 
 from contextlib import nullcontext as does_not_raise
 
 import pytest
-from edgepi.adc.adc_constants import ADCNum
-from edgepi.adc.adc_voltage import (
+
+from edgepi.utilities.crc_8_atm import (
+    generate_crc_8_table,
     check_crc,
+    get_crc,
     CRCCheckError,
-    _code_to_input_voltage,
-    generate_crc_8_table,
-    code_to_temperature,
-    CRC_8_ATM_GEN
+    CRC_8_ATM_GEN,
+    CRC_8_ATM_LUT,
 )
-from edgepi.adc.adc_crc_8_atm import CRC_8_ATM_LUT
-
-# pylint: disable=too-many-lines
-
-# mock calib values
-V_REF = 2.5
-GAIN = 1
-OFFSET = 0
-
-
-@pytest.mark.parametrize(
-    "code, voltage, num_bytes",
-    [
-        (0x00000000, 0, ADCNum.ADC_1.value.num_data_bytes),
-        (0x00000000, 0, ADCNum.ADC_2.value.num_data_bytes),
-        # based on a reference voltage of 2.5 V
-        (
-            0xFFFFFFFF,
-            5.0,
-            ADCNum.ADC_1.value.num_data_bytes,
-        ),
-        (
-            0xFFFFFF,
-            5.0,
-            ADCNum.ADC_2.value.num_data_bytes,
-        ),
-    ],
-)
-def test_code_to_voltage(code, voltage, num_bytes):
-    assert pytest.approx(_code_to_input_voltage(code, V_REF, num_bytes * 8)) == voltage
-
 
 @pytest.mark.parametrize(
     "voltage_bytes, crc_code, err",
     [
         ([51, 16, 126, 166], 62, does_not_raise()),
         ([51, 14, 170, 195], 98, does_not_raise()),
         ([51, 16, 133, 237], 75, does_not_raise()),
@@ -68,17 +36,26 @@
 
 
 def test_generate_crc_8_table():
     assert generate_crc_8_table(CRC_8_ATM_GEN) == CRC_8_ATM_LUT
 
 
 @pytest.mark.parametrize(
-    "code, ref_resistance, temp_offset, rtd_conv_constant",
+    "data, expected, err",
     [
-        ([51, 16, 126, 166], 1326.20, 100, 0.385),
-        ([0x8, 0x43, 0x1C, 0x45], 1326.20, 100, 0.385),
-    ]
+        ([51, 16, 126, 166], 62, does_not_raise()),
+        ([51, 14, 170, 195], 98, does_not_raise()),
+        ([51, 16, 133, 237], 75, does_not_raise()),
+        ([51, 17, 166, 166], 71, does_not_raise()),
+        ([51, 16, 148, 157], 94, does_not_raise()),
+        ([51, 14, 144, 155], 150, does_not_raise()),
+        ([51, 14, 166, 18], 167, does_not_raise()),
+        ([51, 16, 5, 109], 116, does_not_raise()),
+        ([51, 15, 16, 130], 4, does_not_raise())
+    ],
 )
-def test_code_to_temperature(code, ref_resistance, temp_offset, rtd_conv_constant):
-    # TODO: add check for expected value later if any values are known. No errors raised
-    # is good enough for now.
-    code_to_temperature(code, ref_resistance, temp_offset, rtd_conv_constant)
+def test_get_crc(data, expected, err):
+    data_crc = get_crc(data)
+    assert len(data)+1 == len(data_crc)
+    assert data_crc[-1] == expected
+    with err:
+        check_crc(data, data_crc[-1])
```

### Comparing `edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_calibration/test_edgepi_calibration.py` & `edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_calibration/test_edgepi_calibration.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 PATH = os.path.dirname(os.path.abspath(__file__))
 import sys
 sys.modules['periphery'] = mock.MagicMock()
 
 import pytest
 from edgepi.calibration.edgepi_calibration import EdgePiCalibration
-from edgepi.calibration.eeprom_constants import ModuleNames
+from edgepi.eeprom.eeprom_constants import ModuleNames
 
 def read_binfile():
     """Read the dummy serializedFile and return byte string"""
     with open(PATH+"/serializedFile","rb") as fd:
         b_string = fd.read()
     return b_string
```

### Comparing `edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_dac/test_dac_commands.py` & `edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_dac/test_dac_commands.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,25 +5,29 @@
 import sys
 sys.modules['periphery'] = mock.MagicMock()
 
 import pytest
 from edgepi.dac.dac_constants import DACChannel as CH
 from edgepi.dac.dac_commands import DACCommands
 from edgepi.dac.dac_constants import EdgePiDacCalibrationConstants as CALIB_CONSTS, PowerMode
-from edgepi.calibration.edgepi_eeprom import EdgePiEEPROM
-from test_edgepi.unit_tests.test_calibration.read_serialized import read_binfile
+from edgepi.calibration.calibration_constants import CalibParam
+
+dummy_calib_param_dict = {0:CalibParam(gain=1,offset=0),
+                          1:CalibParam(gain=1,offset=0),
+                          2:CalibParam(gain=1,offset=0),
+                          3:CalibParam(gain=1,offset=0),
+                          4:CalibParam(gain=1,offset=0),
+                          5:CalibParam(gain=1,offset=0),
+                          6:CalibParam(gain=1,offset=0),
+                          7:CalibParam(gain=1,offset=0)}
 
 @pytest.fixture(name="dac_ops")
 def fixture_test_dac_ops(mocker):
     mocker.patch("edgepi.peripherals.i2c.I2C")
-    mocker.patch("edgepi.dac.edgepi_dac.EdgePiEEPROM._EdgePiEEPROM__read_edgepi_reserved_memory",
-                  return_value = read_binfile())
-    eeprom = EdgePiEEPROM()
-    eeprom_data  = eeprom.get_edgepi_reserved_data()
-    dac_calib_params = eeprom_data.dac_calib_parms
+    dac_calib_params = dummy_calib_param_dict
     dac_ops = DACCommands(dac_calib_params)
     return dac_ops
 
 
 # Combine command needs check for interger numbers for op-code, channel and value
 # It also needs to check the range of each value.
 
@@ -55,27 +59,29 @@
     with pytest.raises(Exception) as err:
         dac_ops.check_for_int(sample)
     assert err.type is error
 
 
 @pytest.mark.parametrize(
     "range_min, target, range_max, result",
-    [(0, 0, 10, True), (0, 10, 10, True), (0, 5, 10, True), (0.5, 1, 1.1, True)],
+    [(0, 0, 10, True),
+     (0, 5, 10, True),
+     (0.5, 1, 1.1, True)],
 )
 def test_dac_check_range(range_min, target, range_max, result, dac_ops):
     assert dac_ops.check_range(target, range_min, range_max) == result
 
 
 @pytest.mark.parametrize(
     "range_min, target, range_max, error",
     [
         (0, -1, len(CH), ValueError),
         (0, 11, len(CH), ValueError),
         (0, -5, CALIB_CONSTS.RANGE.value, ValueError),
-        (0, 65536, CALIB_CONSTS.RANGE.value, ValueError),
+        (0, 65536, (CALIB_CONSTS.RANGE.value)-1, ValueError),
     ],
 )
 def test_dac_check_range_raises(range_min, target, range_max, error, dac_ops):
     with pytest.raises(Exception) as err:
         dac_ops.check_range(target, range_min, range_max)
     assert err.type is error
 
@@ -105,25 +111,79 @@
 # voltage to code conversion
 # voltage = positive floating number 0~5V ideally
 # code = positive integer number 0~65535
 # rounding up/down during conversion ?
 
 
 @pytest.mark.parametrize("ch, expected, dac_gain, result",
-                        [(1, 2.345, 1, 30282), (0, 2.345, 2, 15285), (3, 2.345, 1, 30341)])
+                        [
+(0, 0.5 , 1, 6553.5),
+(1, 1 , 1, 13107),
+(2, 1.5 , 1, 19660.5),
+(3, 2 , 1, 26214),
+(4, 2.5 , 1, 32767.5),
+(5, 3 , 1, 39321),
+(6, 3.5 , 1, 45874.5),
+(7, 4 , 1, 52428),
+(0, 4.5 , 1, 58981.5),
+(1, 5 , 1, 65535),
+(2, 0.5 ,2,3276.75),
+(3, 1	 ,2,6553.5),
+(4, 1.5 ,2,9830.25),
+(5, 2	 ,2,13107),
+(6, 2.5 ,2,16383.75),
+(7, 3	 ,2,19660.5),
+(0, 3.5 ,2,22937.25),
+(1, 4	 ,2,26214),
+(2, 4.5 ,2,29490.75),
+(3, 5	 ,2,32767.5),
+(4, 5.5 ,2,36044.25),
+(5, 6	 ,2,39321),
+(6, 6.5 ,2,42597.75),
+(7, 7	 ,2,45874.5),
+(0, 7.5 ,2,49151.25),
+(2, 8	 ,2,52428),
+(3, 8.5 ,2,55704.75),
+(4, 9	 ,2,58981.5),
+(5, 9.5 ,2,62258.25),
+(6, 10  ,2,65535),
+                         ])
 def test_dac_voltage_to_code(ch, expected, dac_gain, result, dac_ops):
-    assert dac_ops.voltage_to_code(ch, expected, dac_gain) == result
+    assert dac_ops.voltage_to_code(ch, expected, dac_gain) == round(result)
 
 
 @pytest.mark.parametrize(
     "ch, code, dac_gain, result",
     [
-        (1, 33798, 1, 2.619),
-        (0, 33798, 2, 5.239),
-        (3, 33798, 1, 2.614),
+        (1, 5000, 1, 0.3814755474),
+        (2, 10000, 1, 0.7629510948),
+        (3, 15000, 1, 1.144426642),
+        (4, 20000, 1, 1.52590219),
+        (5, 25000, 1, 1.907377737),
+        (6, 30000, 1, 2.288853285),
+        (7, 35000, 1, 2.670328832),
+        (0, 40000, 1, 3.051804379),
+        (1, 45000, 1, 3.433279927),
+        (2, 50000, 1, 3.814755474),
+        (3, 55000, 1, 4.196231022),
+        (4, 60000, 1, 4.577706569),
+        (5, 65000, 1, 4.959182116),
+        (6, 5000, 2, 0.7629510948),
+        (7, 10000, 2, 1.52590219),
+        (0, 15000, 2, 2.288853285),
+        (1, 20000, 2, 3.051804379),
+        (2, 25000, 2, 3.814755474),
+        (3, 30000, 2, 4.577706569),
+        (4, 35000, 2, 5.340657664),
+        (5, 40000, 2, 6.103608759),
+        (6, 45000, 2, 6.866559854),
+        (7, 50000, 2, 7.629510948),
+        (0, 55000, 2, 8.392462043),
+        (1, 60000, 2, 9.155413138),
+        (2, 65000, 2, 9.918364233),
     ],
 )
 def test_dac_code_to_voltage(ch, code, dac_gain, result, dac_ops):
     assert pytest.approx(dac_ops.code_to_voltage(ch, code, dac_gain), 0.001) == result
 
 
 @pytest.mark.parametrize(
```

### Comparing `edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_din/test_edgepi_din.py` & `edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_din/test_edgepi_din.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,39 +5,40 @@
 from unittest import mock
 import sys
 if sys.platform != 'linux':
     sys.modules['periphery'] = mock.MagicMock()
 
 from contextlib import nullcontext as does_not_raise
 import pytest
+from edgepi.digital_input.digital_input_constants import DinPins
 from edgepi.gpio.gpio_constants import GpioPins
 from edgepi.digital_input.edgepi_digital_input import EdgePiDigitalInput, InvalidPinName
 
 @pytest.fixture(name="din")
 def fixture_test_dac(mocker):
     mocker.patch('edgepi.gpio.edgepi_gpio.EdgePiGPIO')
     yield EdgePiDigitalInput()
 
 @pytest.mark.parametrize("pin_name, mock_value, result, error",
-                        [(GpioPins.DIN1, True, True, does_not_raise()),
-                         (GpioPins.DIN2, True, True, does_not_raise()),
-                         (GpioPins.DIN3, True, True, does_not_raise()),
-                         (GpioPins.DIN4, True, True, does_not_raise()),
-                         (GpioPins.DIN5, True, True, does_not_raise()),
-                         (GpioPins.DIN6, True, True, does_not_raise()),
-                         (GpioPins.DIN7, True, True, does_not_raise()),
-                         (GpioPins.DIN8, True, True, does_not_raise()),
-                         (GpioPins.DIN1, False, False, does_not_raise()),
-                         (GpioPins.DIN2, False, False, does_not_raise()),
-                         (GpioPins.DIN3, False, False, does_not_raise()),
-                         (GpioPins.DIN4, False, False, does_not_raise()),
-                         (GpioPins.DIN5, False, False, does_not_raise()),
-                         (GpioPins.DIN6, False, False, does_not_raise()),
-                         (GpioPins.DIN7, False, False, does_not_raise()),
-                         (GpioPins.DIN8, False, False, does_not_raise()),
+                        [(DinPins.DIN1, True, True, does_not_raise()),
+                         (DinPins.DIN2, True, True, does_not_raise()),
+                         (DinPins.DIN3, True, True, does_not_raise()),
+                         (DinPins.DIN4, True, True, does_not_raise()),
+                         (DinPins.DIN5, True, True, does_not_raise()),
+                         (DinPins.DIN6, True, True, does_not_raise()),
+                         (DinPins.DIN7, True, True, does_not_raise()),
+                         (DinPins.DIN8, True, True, does_not_raise()),
+                         (DinPins.DIN1, False, False, does_not_raise()),
+                         (DinPins.DIN2, False, False, does_not_raise()),
+                         (DinPins.DIN3, False, False, does_not_raise()),
+                         (DinPins.DIN4, False, False, does_not_raise()),
+                         (DinPins.DIN5, False, False, does_not_raise()),
+                         (DinPins.DIN6, False, False, does_not_raise()),
+                         (DinPins.DIN7, False, False, does_not_raise()),
+                         (DinPins.DIN8, False, False, does_not_raise()),
                          (GpioPins.DOUT2, False, False, pytest.raises(InvalidPinName)),
                          (None, False, False, pytest.raises(InvalidPinName))])
 def test_edgepi_digital_input_state(mocker, pin_name, mock_value, result, error, din):
     mocker.patch("edgepi.gpio.edgepi_gpio.EdgePiGPIOChip.read_gpio_pin_state",
                  return_value = mock_value)
     with error:
         state = din.digital_input_state(pin_name)
```

### Comparing `edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_dout/test_edgepi_dout.py` & `edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_dout/test_edgepi_dout.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,79 +6,78 @@
 import sys
 if sys.platform != 'linux':
     sys.modules['periphery'] = mock.MagicMock()
 
 from contextlib import nullcontext as does_not_raise
 import pytest
 from edgepi.gpio.gpio_constants import GpioPins
-from edgepi.gpio.gpio_configs import DOUTPins
+from edgepi.digital_output.digital_output_constants import DoutPins, DoutTriState
 from edgepi.digital_output.edgepi_digital_output import EdgePiDigitalOutput, InvalidPinName
 
-@pytest.mark.parametrize("pin_name, state, error",
-                        [(GpioPins.DOUT1, True, does_not_raise()),
-                         (GpioPins.DOUT2, True, does_not_raise()),
-                         (GpioPins.DOUT3, True, does_not_raise()),
-                         (GpioPins.DOUT4, True, does_not_raise()),
-                         (GpioPins.DOUT5, True, does_not_raise()),
-                         (GpioPins.DOUT6, True, does_not_raise()),
-                         (GpioPins.DOUT7, True, does_not_raise()),
-                         (GpioPins.DOUT8, True, does_not_raise()),
-                         (GpioPins.DOUT1, False, does_not_raise()),
-                         (GpioPins.DOUT2, False, does_not_raise()),
-                         (GpioPins.DOUT3, False, does_not_raise()),
-                         (GpioPins.DOUT4, False, does_not_raise()),
-                         (GpioPins.DOUT5, False, does_not_raise()),
-                         (GpioPins.DOUT6, False, does_not_raise()),
-                         (GpioPins.DOUT7, False, does_not_raise()),
-                         (GpioPins.DOUT8, False, does_not_raise()),
-                         (GpioPins.DOUT8, None, pytest.raises(ValueError)),
-                         (None, False, pytest.raises(InvalidPinName)),
-                         (GpioPins.DIN1, False, pytest.raises(InvalidPinName))])
-def test_edgepi_digital_output_state(mocker, pin_name, state, error):
-    gpio_chip=mocker.patch("edgepi.gpio.edgepi_gpio.EdgePiGPIO.write_gpio_pin_state")
+@pytest.mark.parametrize("pin_name, state, error, aout_clear",
+                        [(DoutPins.DOUT1, DoutTriState.HIGH, does_not_raise(), GpioPins.AO_EN1),
+                         (DoutPins.DOUT2, DoutTriState.HIGH, does_not_raise(), GpioPins.AO_EN2),
+                         (DoutPins.DOUT3, DoutTriState.HIGH, does_not_raise(), GpioPins.AO_EN3),
+                         (DoutPins.DOUT4, DoutTriState.HIGH, does_not_raise(), GpioPins.AO_EN4),
+                         (DoutPins.DOUT5, DoutTriState.HIGH, does_not_raise(), GpioPins.AO_EN5),
+                         (DoutPins.DOUT6, DoutTriState.HIGH, does_not_raise(), GpioPins.AO_EN6),
+                         (DoutPins.DOUT7, DoutTriState.HIGH, does_not_raise(), GpioPins.AO_EN7),
+                         (DoutPins.DOUT8, DoutTriState.HIGH, does_not_raise(), GpioPins.AO_EN8),
+                         (DoutPins.DOUT1, DoutTriState.LOW, does_not_raise(), GpioPins.AO_EN1),
+                         (DoutPins.DOUT2, DoutTriState.LOW, does_not_raise(), GpioPins.AO_EN2),
+                         (DoutPins.DOUT3, DoutTriState.LOW, does_not_raise(), GpioPins.AO_EN3),
+                         (DoutPins.DOUT4, DoutTriState.LOW, does_not_raise(), GpioPins.AO_EN4),
+                         (DoutPins.DOUT5, DoutTriState.LOW, does_not_raise(), GpioPins.AO_EN5),
+                         (DoutPins.DOUT6, DoutTriState.LOW, does_not_raise(), GpioPins.AO_EN6),
+                         (DoutPins.DOUT7, DoutTriState.LOW, does_not_raise(), GpioPins.AO_EN7),
+                         (DoutPins.DOUT8, DoutTriState.LOW, does_not_raise(), GpioPins.AO_EN8),
+                         (DoutPins.DOUT1, DoutTriState.HI_Z, does_not_raise(), GpioPins.AO_EN1),
+                         (DoutPins.DOUT2, DoutTriState.HI_Z, does_not_raise(), GpioPins.AO_EN2),
+                         (DoutPins.DOUT3, DoutTriState.HI_Z, does_not_raise(), GpioPins.AO_EN3),
+                         (DoutPins.DOUT4, DoutTriState.HI_Z, does_not_raise(), GpioPins.AO_EN4),
+                         (DoutPins.DOUT5, DoutTriState.HI_Z, does_not_raise(), GpioPins.AO_EN5),
+                         (DoutPins.DOUT6, DoutTriState.HI_Z, does_not_raise(), GpioPins.AO_EN6),
+                         (DoutPins.DOUT7, DoutTriState.HI_Z, does_not_raise(), GpioPins.AO_EN7),
+                         (DoutPins.DOUT8, DoutTriState.HI_Z, does_not_raise(), GpioPins.AO_EN8),
+                         (DoutPins.DOUT8, None, pytest.raises(ValueError), None),
+                         (None, False, pytest.raises(InvalidPinName), None),
+                         (GpioPins.AO_EN8, False, pytest.raises(InvalidPinName), None)])
+def test_set_dout_state(mocker, pin_name, state, error, aout_clear):
     expander_set = mocker.patch("edgepi.gpio.edgepi_gpio.EdgePiGPIO.set_expander_pin")
     expander_clear = mocker.patch("edgepi.gpio.edgepi_gpio.EdgePiGPIO.clear_expander_pin")
-    dout = EdgePiDigitalOutput()
-    with error:
-        dout.digital_output_state(pin_name, state)
-        if pin_name.value in [DOUTPins.DOUT1.value,DOUTPins.DOUT2.value]:
-            gpio_chip.assert_called_once_with(pin_name.value, state)
-        else:
-            if state:
-                expander_set.assert_called_once_with(pin_name.value)
-            else:
-                expander_clear.assert_called_once_with(pin_name.value)
-
-@pytest.mark.parametrize("pin_name, direction, error",
-                        [(GpioPins.DOUT1, True, does_not_raise()),
-                         (GpioPins.DOUT2, True, does_not_raise()),
-                         (GpioPins.DOUT3, True, does_not_raise()),
-                         (GpioPins.DOUT4, True, does_not_raise()),
-                         (GpioPins.DOUT5, True, does_not_raise()),
-                         (GpioPins.DOUT6, True, does_not_raise()),
-                         (GpioPins.DOUT7, True, does_not_raise()),
-                         (GpioPins.DOUT8, True, does_not_raise()),
-                         (GpioPins.DOUT1, False, does_not_raise()),
-                         (GpioPins.DOUT2, False, does_not_raise()),
-                         (GpioPins.DOUT3, False, does_not_raise()),
-                         (GpioPins.DOUT4, False, does_not_raise()),
-                         (GpioPins.DOUT5, False, does_not_raise()),
-                         (GpioPins.DOUT6, False, does_not_raise()),
-                         (GpioPins.DOUT7, False, does_not_raise()),
-                         (GpioPins.DOUT8, False, does_not_raise()),
-                         (GpioPins.DOUT8, None, pytest.raises(ValueError)),
-                         (None, False, pytest.raises(InvalidPinName)),
-                         (GpioPins.DIN1, False, pytest.raises(InvalidPinName))])
-def test_edgepi_digital_output_direction(mocker, pin_name, direction, error):
-    gpio_chip=mocker.patch("edgepi.gpio.edgepi_gpio.EdgePiGPIO.set_gpio_pin_dir")
     exp_dir_in = mocker.patch("edgepi.gpio.edgepi_gpio.EdgePiGPIO.set_expander_pin_direction_in")
-    exp_dir_out = mocker.patch("edgepi.gpio.edgepi_gpio.EdgePiGPIO.set_expander_pin_direction_out")
+    mock_eeprom = mocker.patch("edgepi.dac.edgepi_dac.EdgePiEEPROM")
     dout = EdgePiDigitalOutput()
+    dout.dac=mock_eeprom
     with error:
-        dout.digital_output_direction(pin_name, direction)
-        if pin_name.value in [DOUTPins.DOUT1.value,DOUTPins.DOUT2.value]:
-            gpio_chip.assert_called_once_with(pin_name.value, direction)
+        dout.set_dout_state(pin_name, state)
+        if state == DoutTriState.HIGH:
+            expander_set.assert_called_once_with(pin_name.value)
+        elif state == DoutTriState.LOW:
+            expander_set.assert_called_once_with(aout_clear.value)
+            expander_clear.assert_has_calls([mocker.call(pin_name.value),
+                                             mocker.call(aout_clear.value)])
         else:
-            if direction:
-                exp_dir_in.assert_called_once_with(pin_name.value)
-            else:
-                exp_dir_out.assert_called_once_with(pin_name.value)
+            expander_set.assert_called_once_with(aout_clear.value)
+            expander_clear.assert_called_once_with(pin_name.value)
+            exp_dir_in.assert_called_once_with(pin_name.value)
+            dout.dac.write_voltage.assert_called_once()
+
+@pytest.mark.parametrize("pin_name, mock_vals, result",
+                        [(DoutPins.DOUT1,[True, False], DoutTriState.HIGH),
+                         (DoutPins.DOUT3,[False, False], DoutTriState.LOW),
+                         (DoutPins.DOUT2,[True, True], DoutTriState.HI_Z),
+                         (DoutPins.DOUT4,[False, True], DoutTriState.HI_Z),
+                         (DoutPins.DOUT5,[True, False], DoutTriState.HIGH),
+                         (DoutPins.DOUT7,[False, False], DoutTriState.LOW),
+                         (DoutPins.DOUT6,[True, True], DoutTriState.HI_Z),
+                         (DoutPins.DOUT8,[False, True], DoutTriState.HI_Z),
+                         ])
+def test_get_state(mocker, pin_name, mock_vals, result):
+    mocker.patch("edgepi.gpio.edgepi_gpio.EdgePiGPIO.read_pin_state",
+                               return_value = mock_vals[0])
+    mocker.patch("edgepi.gpio.edgepi_gpio.EdgePiGPIO.get_pin_direction",
+                                   return_value = mock_vals[1])
+    mocker.patch("edgepi.dac.edgepi_dac.EdgePiEEPROM")
+    dout= EdgePiDigitalOutput()
+    gpio_state = dout.get_state(pin_name)
+    assert gpio_state == result
```

### Comparing `edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_gpio/test_edgepi_gpio.py` & `edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_gpio/test_edgepi_gpio.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
                   return_value = mock_value[0])
     edgepi_gpio = EdgePiGPIO()
     with error:
         edgepi_gpio.set_pin_state(pin_name)
 
 @pytest.mark.parametrize("pin_name, mock_value, result, error",
                         [(GpioPins.DIN1.value,[None, None], True, does_not_raise()),
-                         (GpioPins.DOUT1.value,[None, None], False, does_not_raise()),
+                         (GpioPins.DOUT1.value,[None, False], False, does_not_raise()),
                          (GpioPins.AO_EN1.value,[None, False], False, does_not_raise()),
                          (None, [None, None], None, pytest.raises(PinNameNoneError)),
                          ("Does not exits",[None, None], None, pytest.raises(PinNameNotFound))])
 def test_edgepi_gpio_get_pin_direction(mocker, pin_name, mock_value, result, error):
     mocker.patch('edgepi.gpio.edgepi_gpio.EdgePiGPIOExpander.get_expander_pin_direction',
                   return_value = mock_value[1])
     edgepi_gpio = EdgePiGPIO()
```

### Comparing `edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_gpio/test_edgepi_gpio_expander.py` & `edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_gpio/test_edgepi_gpio_expander.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_gpio/test_edgpepi_gpio_chip.py` & `edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_gpio/test_edgpepi_gpio_chip.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,21 +20,21 @@
 def test_edgepi_gpio_init():
     gpio = EdgePiGPIOChip()
     assert gpio.gpiochip_pins_dict == generate_gpiochip_pin_info()
 
 @pytest.mark.parametrize("pin_name, mock_value, result", [("DIN1",[True], True)])
 def test_read_gpio_pin_state(mocker, pin_name, mock_value, result):
     mocker.patch("edgepi.peripherals.gpio.GpioDevice.open_gpio")
-    mocker.patch("edgepi.peripherals.gpio.GpioDevice.close")
+    mocker.patch("edgepi.peripherals.gpio.GpioDevice.close_gpio")
     mocker.patch("edgepi.peripherals.gpio.GpioDevice.read_state", return_value = mock_value[0])
     gpio = EdgePiGPIOChip()
     assert gpio.read_gpio_pin_state(pin_name) == result
 
 @pytest.mark.parametrize("pin_name, mock_value, result", [("DIN1",[True], True),
                                                           ("DIN1",[False], False)])
 def test_write_gpio_pin_state(mocker, pin_name, mock_value, result):
     mocker.patch("edgepi.peripherals.gpio.GpioDevice.open_gpio")
-    mocker.patch("edgepi.peripherals.gpio.GpioDevice.close")
+    mocker.patch("edgepi.peripherals.gpio.GpioDevice.close_gpio")
     mocker.patch("edgepi.peripherals.gpio.GpioDevice.write_state")
     mocker.patch("edgepi.peripherals.gpio.GpioDevice.read_state", return_value = mock_value[0])
     gpio = EdgePiGPIOChip()
     assert gpio.write_gpio_pin_state(pin_name, mock_value[0]) == result
```

### Comparing `edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_gpio/test_gpio_config.py` & `edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_gpio/test_gpio_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,14 +120,22 @@
     zip(pin_list.items(), GpioBOutputSet, GpioBOutputClear, GpioBPinDirOut):
 
         assert pin[1].set_code == output_set.value
         assert pin[1].clear_code == output_clear.value
         assert pin[1].dir_out_code == output_dir.value
         assert pin[1].address == GpioExpanderAddress.EXP_TWO.value
 
+def test_generate_pin_info_relay(config = GpioConfigs.RELAY.value):
+    pin_list = generate_pin_info(config)
+    pin_keys = list(pin_list.keys())
+    assert pin_list[pin_keys[0]].set_code == GpioBOutputSet.SET_OUTPUT_8.value
+    assert pin_list[pin_keys[0]].clear_code == GpioBOutputClear.CLEAR_OUTPUT_8.value
+    assert pin_list[pin_keys[0]].dir_out_code == GpioBPinDirOut.PIN8_DIR_OUT.value
+    assert pin_list[pin_keys[0]].address == GpioExpanderAddress.EXP_TWO.value
+
 def test_generate_pin_info_adc(config = GpioConfigs.ADC.value):
     pin_list = generate_pin_info(config)
     pin_keys = list(pin_list.keys())
     assert pin_list[pin_keys[0]].set_code == GpioBOutputSet.SET_OUTPUT_2.value
     assert pin_list[pin_keys[0]].clear_code == GpioBOutputClear.CLEAR_OUTPUT_2.value
     assert pin_list[pin_keys[0]].dir_out_code == GpioBPinDirOut.PIN2_DIR_OUT.value
     assert pin_list[pin_keys[0]].address == GpioExpanderAddress.EXP_TWO.value
@@ -146,17 +154,18 @@
 
 def test_generate_expander_pin_info():
     pin_dict = generate_expander_pin_info()
     result_dict = {}
     result_dict.update(generate_pin_info(GpioConfigs.DAC.value))
     result_dict.update(generate_pin_info(GpioConfigs.ADC.value))
     result_dict.update(generate_pin_info(GpioConfigs.RTD.value))
+    result_dict.update(generate_pin_info(GpioConfigs.RELAY.value))
     result_dict.update(generate_pin_info(GpioConfigs.LED.value))
-    result_dict.update(generate_pin_info(GpioConfigs.DOUT2.value))
+    result_dict.update(generate_pin_info(GpioConfigs.DOUT.value))
+    result_dict.update(generate_pin_info(GpioConfigs.PWM.value))
     assert pin_dict == result_dict
 
 def test_generate_gpiochip_pin_info():
     pin_dict = generate_gpiochip_pin_info()
     result_dict = {}
     result_dict.update(generate_pin_info(GpioConfigs.DIN.value))
-    result_dict.update(generate_pin_info(GpioConfigs.DOUT1.value))
     assert pin_dict == result_dict
```

### Comparing `edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_gpio/test_gpio_constants.py` & `edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_gpio/test_gpio_constants.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_peripherals/test_gpio.py` & `edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_peripherals/test_gpio.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_peripherals/test_i2c.py` & `edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_peripherals/test_i2c.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_reg_helper/test_reg_helper.py` & `edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_reg_helper/test_reg_helper.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_tc/test_tc_commands.py` & `edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_tc/test_tc_commands.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_tc/test_tc_conv_time.py` & `edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_tc/test_tc_conv_time.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.1.7/src/test_edgepi/unit_tests/test_tc/test_tc_faults.py` & `edgepi-python-sdk-1.2.1/src/test_edgepi/unit_tests/test_tc/test_tc_faults.py`

 * *Files identical despite different names*

