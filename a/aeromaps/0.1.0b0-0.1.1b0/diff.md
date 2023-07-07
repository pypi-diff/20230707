# Comparing `tmp/aeromaps-0.1.0b0.tar.gz` & `tmp/aeromaps-0.1.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeromaps-0.1.0b0.tar", max compression
+gzip compressed data, was "aeromaps-0.1.1b0.tar", max compression
```

## Comparing `aeromaps-0.1.0b0.tar` & `aeromaps-0.1.1b0.tar`

### file list

```diff
@@ -1,93 +1,93 @@
--rw-r--r--   0        0        0     2063 2023-06-07 09:00:09.911705 aeromaps-0.1.0b0/README.rst
--rw-r--r--   0        0        0        0 2023-06-07 09:00:09.911705 aeromaps-0.1.0b0/aeromaps/__init__.py
--rw-r--r--   0        0        0     3419 2023-06-07 09:00:09.911705 aeromaps-0.1.0b0/aeromaps/app.ipynb
--rw-r--r--   0        0        0     2275 2023-06-07 09:00:09.911705 aeromaps-0.1.0b0/aeromaps/app.py
--rw-r--r--   0        0        0        0 2023-06-07 09:00:09.911705 aeromaps-0.1.0b0/aeromaps/core/__init__.py
--rw-r--r--   0        0        0    13545 2023-06-07 09:00:09.911705 aeromaps-0.1.0b0/aeromaps/core/gemseo.py
--rw-r--r--   0        0        0    17837 2023-06-07 09:00:09.911705 aeromaps-0.1.0b0/aeromaps/core/models.py
--rw-r--r--   0        0        0     9458 2023-06-07 09:00:09.911705 aeromaps-0.1.0b0/aeromaps/core/process.py
--rw-r--r--   0        0        0        0 2023-06-07 09:00:09.911705 aeromaps-0.1.0b0/aeromaps/gui/__init__.py
--rw-r--r--   0        0        0     3608 2023-06-07 09:00:09.911705 aeromaps-0.1.0b0/aeromaps/gui/fleet.py
--rw-r--r--   0        0        0    79143 2023-06-07 09:00:09.911705 aeromaps-0.1.0b0/aeromaps/gui/graphical_user_interface.py
--rw-r--r--   0        0        0     4224 2023-06-07 09:00:09.911705 aeromaps-0.1.0b0/aeromaps/gui/plots.py
--rw-r--r--   0        0        0     5206 2023-06-07 09:00:09.911705 aeromaps-0.1.0b0/aeromaps/gui/resources/Beta.png
--rw-r--r--   0        0        0     1285 2023-06-07 09:00:09.911705 aeromaps-0.1.0b0/aeromaps/gui/resources/aboutAeroMAPS_en.md
--rw-r--r--   0        0        0     1440 2023-06-07 09:00:09.911705 aeromaps-0.1.0b0/aeromaps/gui/resources/aboutAeroMAPS_fr.md
--rw-r--r--   0        0        0    18684 2023-06-07 09:00:09.911705 aeromaps-0.1.0b0/aeromaps/gui/resources/logo-ISAE_SUPAERO.png
--rw-r--r--   0        0        0        0 2023-06-07 09:00:09.911705 aeromaps-0.1.0b0/aeromaps/models/__init__.py
--rw-r--r--   0        0        0        0 2023-06-07 09:00:09.911705 aeromaps-0.1.0b0/aeromaps/models/air_transport/__init__.py
--rw-r--r--   0        0        0        0 2023-06-07 09:00:09.911705 aeromaps-0.1.0b0/aeromaps/models/air_transport/air_traffic/__init__.py
--rw-r--r--   0        0        0     1619 2023-06-07 09:00:09.911705 aeromaps-0.1.0b0/aeromaps/models/air_transport/air_traffic/ask.py
--rw-r--r--   0        0        0    16535 2023-06-07 09:00:09.911705 aeromaps-0.1.0b0/aeromaps/models/air_transport/air_traffic/rpk.py
--rw-r--r--   0        0        0     5255 2023-06-07 09:00:09.911705 aeromaps-0.1.0b0/aeromaps/models/air_transport/air_traffic/rtk.py
--rw-r--r--   0        0        0     7593 2023-06-07 09:00:09.911705 aeromaps-0.1.0b0/aeromaps/models/air_transport/air_traffic/short_range_distribution.py
--rw-r--r--   0        0        0     1104 2023-06-07 09:00:09.911705 aeromaps-0.1.0b0/aeromaps/models/air_transport/air_traffic/total_aircraft_distance.py
--rw-r--r--   0        0        0        0 2023-06-07 09:00:09.911705 aeromaps-0.1.0b0/aeromaps/models/air_transport/aircraft_energy/__init__.py
--rw-r--r--   0        0        0     5791 2023-06-07 09:00:09.911705 aeromaps-0.1.0b0/aeromaps/models/air_transport/aircraft_energy/efficiency.py
--rw-r--r--   0        0        0     2705 2023-06-07 09:00:09.911705 aeromaps-0.1.0b0/aeromaps/models/air_transport/aircraft_energy/fuel_distribution.py
--rw-r--r--   0        0        0    10193 2023-06-07 09:00:09.911705 aeromaps-0.1.0b0/aeromaps/models/air_transport/aircraft_energy/fuel_emissions.py
--rw-r--r--   0        0        0     8210 2023-06-07 09:00:09.911705 aeromaps-0.1.0b0/aeromaps/models/air_transport/aircraft_energy/production_choices.py
--rw-r--r--   0        0        0        0 2023-06-07 09:00:09.911705 aeromaps-0.1.0b0/aeromaps/models/air_transport/aircraft_fleet_and_operations/__init__.py
--rw-r--r--   0        0        0     4874 2023-06-07 09:00:09.911705 aeromaps-0.1.0b0/aeromaps/models/air_transport/aircraft_fleet_and_operations/aircraft_fleet_and_operations.py
--rw-r--r--   0        0        0        0 2023-06-07 09:00:09.911705 aeromaps-0.1.0b0/aeromaps/models/air_transport/aircraft_fleet_and_operations/fleet/__init__.py
--rw-r--r--   0        0        0    29009 2023-06-07 09:00:09.911705 aeromaps-0.1.0b0/aeromaps/models/air_transport/aircraft_fleet_and_operations/fleet/aircraft_efficiency.py
--rw-r--r--   0        0        0    57335 2023-06-07 09:00:09.915705 aeromaps-0.1.0b0/aeromaps/models/air_transport/aircraft_fleet_and_operations/fleet/fleet_model.py
--rw-r--r--   0        0        0        0 2023-06-07 09:00:09.915705 aeromaps-0.1.0b0/aeromaps/models/air_transport/aircraft_fleet_and_operations/load_factor/__init__.py
--rw-r--r--   0        0        0     1762 2023-06-07 09:00:09.915705 aeromaps-0.1.0b0/aeromaps/models/air_transport/aircraft_fleet_and_operations/load_factor/load_factor.py
--rw-r--r--   0        0        0        0 2023-06-07 09:00:09.915705 aeromaps-0.1.0b0/aeromaps/models/air_transport/aircraft_fleet_and_operations/non_co2/__init__.py
--rw-r--r--   0        0        0     2224 2023-06-07 09:00:09.915705 aeromaps-0.1.0b0/aeromaps/models/air_transport/aircraft_fleet_and_operations/non_co2/non_co2.py
--rw-r--r--   0        0        0        0 2023-06-07 09:00:09.915705 aeromaps-0.1.0b0/aeromaps/models/air_transport/aircraft_fleet_and_operations/operations/__init__.py
--rw-r--r--   0        0        0     1410 2023-06-07 09:00:09.915705 aeromaps-0.1.0b0/aeromaps/models/air_transport/aircraft_fleet_and_operations/operations/operations.py
--rw-r--r--   0        0        0      373 2023-06-07 09:00:09.915705 aeromaps-0.1.0b0/aeromaps/models/air_transport/constants.py
--rw-r--r--   0        0        0     9886 2023-06-07 09:00:09.915705 aeromaps-0.1.0b0/aeromaps/models/air_transport/parameters.py
--rw-r--r--   0        0        0     3686 2023-06-07 09:00:09.915705 aeromaps-0.1.0b0/aeromaps/models/base.py
--rw-r--r--   0        0        0      193 2023-06-07 09:00:09.915705 aeromaps-0.1.0b0/aeromaps/models/constants.py
--rw-r--r--   0        0        0        0 2023-06-07 09:00:09.915705 aeromaps-0.1.0b0/aeromaps/models/impacts/__init__.py
--rw-r--r--   0        0        0        0 2023-06-07 09:00:09.915705 aeromaps-0.1.0b0/aeromaps/models/impacts/climate/__init__.py
--rw-r--r--   0        0        0     1237 2023-06-07 09:00:09.915705 aeromaps-0.1.0b0/aeromaps/models/impacts/climate/climate.py
--rw-r--r--   0        0        0        0 2023-06-07 09:00:09.915705 aeromaps-0.1.0b0/aeromaps/models/impacts/effective_radiative_forcing/__init__.py
--rw-r--r--   0        0        0     4547 2023-06-07 09:00:09.915705 aeromaps-0.1.0b0/aeromaps/models/impacts/effective_radiative_forcing/effective_radiative_forcing.py
--rw-r--r--   0        0        0      868 2023-06-07 09:00:09.915705 aeromaps-0.1.0b0/aeromaps/models/impacts/effective_radiative_forcing/test.py
--rw-r--r--   0        0        0        0 2023-06-07 09:00:09.915705 aeromaps-0.1.0b0/aeromaps/models/impacts/emissions/__init__.py
--rw-r--r--   0        0        0    26676 2023-06-07 09:00:09.915705 aeromaps-0.1.0b0/aeromaps/models/impacts/emissions/co2_emissions.py
--rw-r--r--   0        0        0     6456 2023-06-07 09:00:09.915705 aeromaps-0.1.0b0/aeromaps/models/impacts/emissions/non_co2_emissions.py
--rw-r--r--   0        0        0        0 2023-06-07 09:00:09.915705 aeromaps-0.1.0b0/aeromaps/models/impacts/energy_resources/__init__.py
--rw-r--r--   0        0        0    38627 2023-06-07 09:00:09.915705 aeromaps-0.1.0b0/aeromaps/models/impacts/energy_resources/energy_consumption.py
--rw-r--r--   0        0        0     4999 2023-06-07 09:00:09.915705 aeromaps-0.1.0b0/aeromaps/models/impacts/energy_resources/resources_consumption.py
--rw-r--r--   0        0        0        0 2023-06-07 09:00:09.915705 aeromaps-0.1.0b0/aeromaps/models/impacts/equivalent_co2_emissions/__init__.py
--rw-r--r--   0        0        0     6643 2023-06-07 09:00:09.915705 aeromaps-0.1.0b0/aeromaps/models/impacts/equivalent_co2_emissions/equivalent_co2_emissions.py
--rw-r--r--   0        0        0        0 2023-06-07 09:00:09.915705 aeromaps-0.1.0b0/aeromaps/models/impacts/others/__init__.py
--rw-r--r--   0        0        0     2259 2023-06-07 09:00:09.915705 aeromaps-0.1.0b0/aeromaps/models/impacts/others/comparison.py
--rw-r--r--   0        0        0     1319 2023-06-07 09:00:09.915705 aeromaps-0.1.0b0/aeromaps/models/impacts/others/others.py
--rw-r--r--   0        0        0     2060 2023-06-07 09:00:09.915705 aeromaps-0.1.0b0/aeromaps/models/impacts/parameters.py
--rw-r--r--   0        0        0     1386 2023-06-07 09:00:09.915705 aeromaps-0.1.0b0/aeromaps/models/parameters.py
--rw-r--r--   0        0        0        0 2023-06-07 09:00:09.915705 aeromaps-0.1.0b0/aeromaps/models/sustainability_assessment/__init__.py
--rw-r--r--   0        0        0        0 2023-06-07 09:00:09.915705 aeromaps-0.1.0b0/aeromaps/models/sustainability_assessment/climate/__init__.py
--rw-r--r--   0        0        0     1836 2023-06-07 09:00:09.915705 aeromaps-0.1.0b0/aeromaps/models/sustainability_assessment/climate/carbon_budgets.py
--rw-r--r--   0        0        0     2180 2023-06-07 09:00:09.915705 aeromaps-0.1.0b0/aeromaps/models/sustainability_assessment/climate/equivalent_carbon_budgets.py
--rw-r--r--   0        0        0     1511 2023-06-07 09:00:09.915705 aeromaps-0.1.0b0/aeromaps/models/sustainability_assessment/climate/test.py
--rw-r--r--   0        0        0        0 2023-06-07 09:00:09.915705 aeromaps-0.1.0b0/aeromaps/models/sustainability_assessment/energy/__init__.py
--rw-r--r--   0        0        0     4001 2023-06-07 09:00:09.915705 aeromaps-0.1.0b0/aeromaps/models/sustainability_assessment/energy/resources_availability.py
--rw-r--r--   0        0        0     1015 2023-06-07 09:00:09.915705 aeromaps-0.1.0b0/aeromaps/models/sustainability_assessment/parameters.py
--rw-r--r--   0        0        0        0 2023-06-07 09:00:09.915705 aeromaps-0.1.0b0/aeromaps/notebooks/__init__.py
--rw-r--r--   0        0        0   841857 2023-06-07 09:00:09.923705 aeromaps-0.1.0b0/aeromaps/notebooks/basic_example.ipynb
--rw-r--r--   0        0        0  1043930 2023-06-07 09:00:09.927706 aeromaps-0.1.0b0/aeromaps/notebooks/fleet.ipynb
--rw-r--r--   0        0        0     3693 2023-06-07 09:00:09.927706 aeromaps-0.1.0b0/aeromaps/plots/__init__.py
--rw-r--r--   0        0        0     8263 2023-06-07 09:00:09.927706 aeromaps-0.1.0b0/aeromaps/plots/air_traffic.py
--rw-r--r--   0        0        0     7576 2023-06-07 09:00:09.927706 aeromaps-0.1.0b0/aeromaps/plots/aircraft_energy.py
--rw-r--r--   0        0        0     8951 2023-06-07 09:00:09.927706 aeromaps-0.1.0b0/aeromaps/plots/aircraft_fleet_and_operations.py
--rw-r--r--   0        0        0    15544 2023-06-07 09:00:09.927706 aeromaps-0.1.0b0/aeromaps/plots/climate.py
--rw-r--r--   0        0        0       99 2023-06-07 09:00:09.927706 aeromaps-0.1.0b0/aeromaps/plots/constants.py
--rw-r--r--   0        0        0    10736 2023-06-07 09:00:09.927706 aeromaps-0.1.0b0/aeromaps/plots/emissions.py
--rw-r--r--   0        0        0     4681 2023-06-07 09:00:09.927706 aeromaps-0.1.0b0/aeromaps/plots/energy_resources.py
--rw-r--r--   0        0        0    22929 2023-06-07 09:00:09.927706 aeromaps-0.1.0b0/aeromaps/plots/indicators.py
--rw-r--r--   0        0        0    12623 2023-06-07 09:00:09.927706 aeromaps-0.1.0b0/aeromaps/plots/main.py
--rw-r--r--   0        0        0    47327 2023-06-07 09:00:09.927706 aeromaps-0.1.0b0/aeromaps/plots/sustainability_assessment.py
--rw-r--r--   0        0        0   110757 2023-06-07 09:00:09.927706 aeromaps-0.1.0b0/aeromaps/resources/data/data.xlsx
--rw-r--r--   0        0        0    54376 2023-06-07 09:00:09.927706 aeromaps-0.1.0b0/aeromaps/resources/data/data_information.csv
--rw-r--r--   0        0        0   303716 2023-06-07 09:00:09.931706 aeromaps-0.1.0b0/aeromaps/resources/data/outputs.json
--rw-r--r--   0        0        0    15171 2023-06-07 09:00:09.931706 aeromaps-0.1.0b0/aeromaps/resources/data/parameters.json
--rw-r--r--   0        0        0        0 2023-06-07 09:00:09.931706 aeromaps-0.1.0b0/aeromaps/utils/__init__.py
--rw-r--r--   0        0        0      478 2023-06-07 09:00:09.931706 aeromaps-0.1.0b0/aeromaps/utils/functions.py
--rw-r--r--   0        0        0     1417 2023-06-07 09:00:22.084167 aeromaps-0.1.0b0/pyproject.toml
--rw-r--r--   0        0        0     3484 1970-01-01 00:00:00.000000 aeromaps-0.1.0b0/PKG-INFO
+-rw-r--r--   0        0        0     2183 2023-07-07 08:18:52.780115 aeromaps-0.1.1b0/README.md
+-rw-r--r--   0        0        0        0 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/__init__.py
+-rw-r--r--   0        0        0     3419 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/app.ipynb
+-rw-r--r--   0        0        0     2424 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/app.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/core/__init__.py
+-rw-r--r--   0        0        0    13545 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/core/gemseo.py
+-rw-r--r--   0        0        0    17791 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/core/models.py
+-rw-r--r--   0        0        0     9458 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/core/process.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/gui/__init__.py
+-rw-r--r--   0        0        0     3608 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/gui/fleet.py
+-rw-r--r--   0        0        0    79056 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/gui/graphical_user_interface.py
+-rw-r--r--   0        0        0     4224 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/gui/plots.py
+-rw-r--r--   0        0        0     5206 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/gui/resources/Beta.png
+-rw-r--r--   0        0        0     1285 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/gui/resources/aboutAeroMAPS_en.md
+-rw-r--r--   0        0        0     1440 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/gui/resources/aboutAeroMAPS_fr.md
+-rw-r--r--   0        0        0    18684 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/gui/resources/logo-ISAE_SUPAERO.png
+-rw-r--r--   0        0        0        0 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/air_transport/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/air_transport/air_traffic/__init__.py
+-rw-r--r--   0        0        0     1619 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/air_transport/air_traffic/ask.py
+-rw-r--r--   0        0        0    16535 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/air_transport/air_traffic/rpk.py
+-rw-r--r--   0        0        0     5255 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/air_transport/air_traffic/rtk.py
+-rw-r--r--   0        0        0     7593 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/air_transport/air_traffic/short_range_distribution.py
+-rw-r--r--   0        0        0     1104 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/air_transport/air_traffic/total_aircraft_distance.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/air_transport/aircraft_energy/__init__.py
+-rw-r--r--   0        0        0     5791 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/air_transport/aircraft_energy/efficiency.py
+-rw-r--r--   0        0        0     2705 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/air_transport/aircraft_energy/fuel_distribution.py
+-rw-r--r--   0        0        0    10193 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/air_transport/aircraft_energy/fuel_emissions.py
+-rw-r--r--   0        0        0     8210 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/air_transport/aircraft_energy/production_choices.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/air_transport/aircraft_fleet_and_operations/__init__.py
+-rw-r--r--   0        0        0     4874 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/air_transport/aircraft_fleet_and_operations/aircraft_fleet_and_operations.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/air_transport/aircraft_fleet_and_operations/fleet/__init__.py
+-rw-r--r--   0        0        0    31711 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/air_transport/aircraft_fleet_and_operations/fleet/aircraft_efficiency.py
+-rw-r--r--   0        0        0    57831 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/air_transport/aircraft_fleet_and_operations/fleet/fleet_model.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/air_transport/aircraft_fleet_and_operations/load_factor/__init__.py
+-rw-r--r--   0        0        0     1762 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/air_transport/aircraft_fleet_and_operations/load_factor/load_factor.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/air_transport/aircraft_fleet_and_operations/non_co2/__init__.py
+-rw-r--r--   0        0        0     2224 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/air_transport/aircraft_fleet_and_operations/non_co2/non_co2.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/air_transport/aircraft_fleet_and_operations/operations/__init__.py
+-rw-r--r--   0        0        0     1410 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/air_transport/aircraft_fleet_and_operations/operations/operations.py
+-rw-r--r--   0        0        0      373 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/air_transport/constants.py
+-rw-r--r--   0        0        0     9886 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/air_transport/parameters.py
+-rw-r--r--   0        0        0     3686 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/base.py
+-rw-r--r--   0        0        0      193 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/constants.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/impacts/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/impacts/climate/__init__.py
+-rw-r--r--   0        0        0     1237 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/impacts/climate/climate.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/impacts/effective_radiative_forcing/__init__.py
+-rw-r--r--   0        0        0     4547 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/impacts/effective_radiative_forcing/effective_radiative_forcing.py
+-rw-r--r--   0        0        0      868 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/impacts/effective_radiative_forcing/test.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/impacts/emissions/__init__.py
+-rw-r--r--   0        0        0    26676 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/impacts/emissions/co2_emissions.py
+-rw-r--r--   0        0        0     6456 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/impacts/emissions/non_co2_emissions.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/impacts/energy_resources/__init__.py
+-rw-r--r--   0        0        0    38627 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/impacts/energy_resources/energy_consumption.py
+-rw-r--r--   0        0        0     4999 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/impacts/energy_resources/resources_consumption.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/impacts/equivalent_co2_emissions/__init__.py
+-rw-r--r--   0        0        0     6643 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/impacts/equivalent_co2_emissions/equivalent_co2_emissions.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/impacts/others/__init__.py
+-rw-r--r--   0        0        0     2259 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/impacts/others/comparison.py
+-rw-r--r--   0        0        0     1319 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/impacts/others/others.py
+-rw-r--r--   0        0        0     2060 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/impacts/parameters.py
+-rw-r--r--   0        0        0     1386 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/parameters.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/sustainability_assessment/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:18:52.784115 aeromaps-0.1.1b0/aeromaps/models/sustainability_assessment/climate/__init__.py
+-rw-r--r--   0        0        0     1836 2023-07-07 08:18:52.788116 aeromaps-0.1.1b0/aeromaps/models/sustainability_assessment/climate/carbon_budgets.py
+-rw-r--r--   0        0        0     2180 2023-07-07 08:18:52.788116 aeromaps-0.1.1b0/aeromaps/models/sustainability_assessment/climate/equivalent_carbon_budgets.py
+-rw-r--r--   0        0        0     1511 2023-07-07 08:18:52.788116 aeromaps-0.1.1b0/aeromaps/models/sustainability_assessment/climate/test.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:18:52.788116 aeromaps-0.1.1b0/aeromaps/models/sustainability_assessment/energy/__init__.py
+-rw-r--r--   0        0        0     4001 2023-07-07 08:18:52.788116 aeromaps-0.1.1b0/aeromaps/models/sustainability_assessment/energy/resources_availability.py
+-rw-r--r--   0        0        0     1015 2023-07-07 08:18:52.788116 aeromaps-0.1.1b0/aeromaps/models/sustainability_assessment/parameters.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:18:52.788116 aeromaps-0.1.1b0/aeromaps/notebooks/__init__.py
+-rw-r--r--   0        0        0   841857 2023-07-07 08:18:52.796116 aeromaps-0.1.1b0/aeromaps/notebooks/basic_example.ipynb
+-rw-r--r--   0        0        0  1043930 2023-07-07 08:18:52.796116 aeromaps-0.1.1b0/aeromaps/notebooks/fleet.ipynb
+-rw-r--r--   0        0        0     3693 2023-07-07 08:18:52.796116 aeromaps-0.1.1b0/aeromaps/plots/__init__.py
+-rw-r--r--   0        0        0     8263 2023-07-07 08:18:52.796116 aeromaps-0.1.1b0/aeromaps/plots/air_traffic.py
+-rw-r--r--   0        0        0     7576 2023-07-07 08:18:52.796116 aeromaps-0.1.1b0/aeromaps/plots/aircraft_energy.py
+-rw-r--r--   0        0        0     8951 2023-07-07 08:18:52.796116 aeromaps-0.1.1b0/aeromaps/plots/aircraft_fleet_and_operations.py
+-rw-r--r--   0        0        0    15544 2023-07-07 08:18:52.800117 aeromaps-0.1.1b0/aeromaps/plots/climate.py
+-rw-r--r--   0        0        0       99 2023-07-07 08:18:52.800117 aeromaps-0.1.1b0/aeromaps/plots/constants.py
+-rw-r--r--   0        0        0    10736 2023-07-07 08:18:52.800117 aeromaps-0.1.1b0/aeromaps/plots/emissions.py
+-rw-r--r--   0        0        0     4681 2023-07-07 08:18:52.800117 aeromaps-0.1.1b0/aeromaps/plots/energy_resources.py
+-rw-r--r--   0        0        0    22929 2023-07-07 08:18:52.800117 aeromaps-0.1.1b0/aeromaps/plots/indicators.py
+-rw-r--r--   0        0        0    12623 2023-07-07 08:18:52.800117 aeromaps-0.1.1b0/aeromaps/plots/main.py
+-rw-r--r--   0        0        0    47327 2023-07-07 08:18:52.800117 aeromaps-0.1.1b0/aeromaps/plots/sustainability_assessment.py
+-rw-r--r--   0        0        0   110757 2023-07-07 08:18:52.800117 aeromaps-0.1.1b0/aeromaps/resources/data/data.xlsx
+-rw-r--r--   0        0        0    54376 2023-07-07 08:18:52.800117 aeromaps-0.1.1b0/aeromaps/resources/data/data_information.csv
+-rw-r--r--   0        0        0   303716 2023-07-07 08:18:52.800117 aeromaps-0.1.1b0/aeromaps/resources/data/outputs.json
+-rw-r--r--   0        0        0    15171 2023-07-07 08:18:52.800117 aeromaps-0.1.1b0/aeromaps/resources/data/parameters.json
+-rw-r--r--   0        0        0        0 2023-07-07 08:18:52.800117 aeromaps-0.1.1b0/aeromaps/utils/__init__.py
+-rw-r--r--   0        0        0      478 2023-07-07 08:18:52.800117 aeromaps-0.1.1b0/aeromaps/utils/functions.py
+-rw-r--r--   0        0        0     1413 2023-07-07 08:19:07.573371 aeromaps-0.1.1b0/pyproject.toml
+-rw-r--r--   0        0        0     3604 1970-01-01 00:00:00.000000 aeromaps-0.1.1b0/PKG-INFO
```

### Comparing `aeromaps-0.1.0b0/README.rst` & `aeromaps-0.1.1b0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,45 @@
-.. image:: https://mybinder.org/badge_logo.svg
- :target: https://mybinder.org/v2/gh/AeroMAPS/AeroMAPS/HEAD?urlpath=voila%2Frender%2Faeromaps%2Fapp.ipynb
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/AeroMAPS/AeroMAPS/HEAD)
 
 AeroMAPS: Multidisciplinary Assessment of Prospective Scenarios for air transport
 =================================================================================
 
 AeroMAPS is a framework for performing Multidisciplinary Assessment of Prospective Scenarios for air transport. For
 instance, it allows simulating and analyzing scenarios for reducing aviation climate impacts through various levers of
 action. It is intended to become a sectoral Integrated Assessment Model (IAM) taking into account technological,
 environmental, sociological, economic and other considerations. It aims to assess the sustainability of simulated air
 transport transition scenarios on multiple criteria.
 
-AeroMAPS is licensed under the `GPL-3.0 <https://www.gnu.org/licenses/gpl-3.0.en.html>`_ license.
+AeroMAPS is licensed under the [GPL-3.0](https://www.gnu.org/licenses/gpl-3.0.en.html) license.
 
-A `documentation <https://aeromaps.github.io/AeroMAPS/>`_ is available for more details on AeroMAPS.
+A [documentation](https://aeromaps.github.io/AeroMAPS/) is available for more details on AeroMAPS.
 
 
 Quick start
 -----------
 
 For a quick start in order to discover the different features of AeroMAPS,
 a graphical user interface has been developed for facilitating the first uses.
 It is available at the following address: https://aeromaps.isae-supaero.fr/
+Another solution is to use the [Binder-hosted graphical user interface](https://mybinder.org/v2/gh/AeroMAPS/AeroMAPS/HEAD?urlpath=voila%2Frender%2Faeromaps%2Fapp.ipynb).
 
 
 Quick installation
 ------------------
 
-The use of the Python Package Index (`PyPI <https://pypi.org/>`_) is the simplest method for installing AeroMAPS.
+The use of the Python Package Index ([PyPI](https://pypi.org/)) is the simplest method for installing AeroMAPS.
 More details and other solutions are provided in the documentation.
 
-**Prerequisite**: AeroMAPS needs at least **Python 3.8.0**.
+**Prerequisite**: AeroMAPS needs at least Python 3.8.0.
 
-You can install the latest version with this command::
+You can install the latest version with this command:
 
-    pip install --upgrade aeromaps
+``` {.bash}
+$ pip install --upgrade aeromaps
+```
 
 
 Citation
 --------
 
 If you use AeroMAPS in your work, please cite the following reference. Other references are available in the
 documentation.
```

### Comparing `aeromaps-0.1.0b0/aeromaps/app.ipynb` & `aeromaps-0.1.1b0/aeromaps/app.ipynb`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/app.py` & `aeromaps-0.1.1b0/aeromaps/app.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,24 +22,32 @@
 
     @staticmethod
     def _run(args):
         """Run AeroMAPS locally or with server configuration."""
         machine = "server" if args.server else "local"
         print(MAIN_NOTEBOOK_NAME)
         if machine == "server":
-            os.system(
-                """voila --port=8080 --no-browser --VoilaConfiguration.file_whitelist="['.*\.(png|jpg|gif|xlsx|ico|pdf)']" """
-                + str(MAIN_NOTEBOOK_NAME)
+            command = (
+                "voila "
+                "--port=8080 "
+                "--no-browser "
+                "--MappingKernelManager.cull_idle_timeout=7200 "
+                """--VoilaConfiguration.file_whitelist "="['.*\.(png|jpg|gif|xlsx|ico|pdf)']" """
             )
         else:
-            os.system(
-                """voila --VoilaConfiguration.file_whitelist="['.*\.(png|jpg|gif|xlsx|ico|pdf)']" """
-                + str(MAIN_NOTEBOOK_NAME)
+            command = (
+                "voila "
+                """--VoilaConfiguration.file_whitelist="['.*\.(png|jpg|gif|xlsx|ico|pdf)']" """
             )
 
+        os.system(
+            command
+            + str(MAIN_NOTEBOOK_NAME)
+        )
+
     # ENTRY POINT ==================================================================================
     def run(self):
         """Main function."""
         subparsers = self.parser.add_subparsers(title="sub-commands")
 
         # sub-command for running AeroMAPS -------------------------------------
         parser_run = subparsers.add_parser(
```

### Comparing `aeromaps-0.1.0b0/aeromaps/core/gemseo.py` & `aeromaps-0.1.1b0/aeromaps/core/gemseo.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/core/models.py` & `aeromaps-0.1.1b0/aeromaps/core/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
     OperationsSimple,
 )
 from aeromaps.models.air_transport.aircraft_fleet_and_operations.non_co2.non_co2 import (
     OperationsContrailsSimple,
 )
 from aeromaps.models.air_transport.aircraft_fleet_and_operations.fleet.aircraft_efficiency import (
     PassengerAircraftEfficiencySimple,
-    FreightAircraftEfficiencySimple,
     PassengerAircraftEfficiencyComplex,
+    FreightAircraftEfficiency,
 )
 from aeromaps.models.air_transport.aircraft_fleet_and_operations.aircraft_fleet_and_operations import (
     EnergyIntensity,
 )
 from aeromaps.models.air_transport.aircraft_energy.fuel_distribution import FuelDistribution
 from aeromaps.models.sustainability_assessment.climate.carbon_budgets import GrossCarbonBudget
 from aeromaps.models.sustainability_assessment.climate.equivalent_carbon_budgets import (
@@ -117,16 +117,16 @@
         "operations_contrails_simple", parameters=AllParameters(), year_parameters=year_parameters
     ),
     "passenger_aircraft_efficiency_simple": PassengerAircraftEfficiencySimple(
         "passenger_aircraft_efficiency_simple",
         year_parameters=year_parameters,
         parameters=AllParameters(),
     ),
-    "freight_aircraft_efficiency_simple": FreightAircraftEfficiencySimple(
-        "freight_aircraft_efficiency_simple",
+    "freight_aircraft_efficiency": FreightAircraftEfficiency(
+        "freight_aircraft_efficiency",
         year_parameters=year_parameters,
         parameters=AllParameters(),
     ),
     "energy_intensity": EnergyIntensity(
         "energy_intensity", parameters=AllParameters(), year_parameters=year_parameters
     ),
     "aircraft_energy": FuelDistribution(
@@ -274,16 +274,16 @@
         "operations_contrails_simple", parameters=AllParameters(), year_parameters=year_parameters
     ),
     "passenger_aircraft_efficiency_complex": PassengerAircraftEfficiencyComplex(
         "passenger_aircraft_efficiency_complex",
         year_parameters=year_parameters,
         parameters=AllParameters(),
     ),
-    "freight_aircraft_efficiency_simple": FreightAircraftEfficiencySimple(
-        "freight_aircraft_efficiency_simple",
+    "freight_aircraft_efficiency": FreightAircraftEfficiency(
+        "freight_aircraft_efficiency",
         year_parameters=year_parameters,
         parameters=AllParameters(),
     ),
     "energy_intensity": EnergyIntensity(
         "energy_intensity", parameters=AllParameters(), year_parameters=year_parameters
     ),
     "aircraft_energy": FuelDistribution(
```

### Comparing `aeromaps-0.1.0b0/aeromaps/core/process.py` & `aeromaps-0.1.1b0/aeromaps/core/process.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/gui/fleet.py` & `aeromaps-0.1.1b0/aeromaps/gui/fleet.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/gui/graphical_user_interface.py` & `aeromaps-0.1.1b0/aeromaps/gui/graphical_user_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -571,15 +571,15 @@
                     layout={"align_items": "center"},
                 ),
                 widgets.VBox(
                     [
                         self.w_aircraft_efficiency,
                         self.w_operations,
                         self.w_load_factor,
-                        #self.w_turboprop,
+                        # self.w_turboprop,
                         self.w_contrails_avoidance,
                     ]
                 ),
             ]
         )
 
         carbon_intensity = widgets.VBox(
@@ -1533,18 +1533,16 @@
         self.fig3.update(self.process.data)
 
     def _download_results(self, change=None):
         if self.download_output:
             self.download_output.clear_output(wait=True)
         else:
             self.download_output = widgets.Output()
-        # file_name = "data.xlsx"
-        file_name = "data.txt"
-        # file_path = "/resources/data/" + file_name
-        file_path = pth.join(DATA_FOLDER, file_name)
+        file_name = "data.xlsx"
+        file_path = "/resources/data/" + file_name
 
         self._trigger_download(file_path, file_name, self.download_output)
         # os.remove(filepath)
 
     def _trigger_download(self, filepath, filename, output):
         js_code = f"""
             var a = document.createElement('a');
```

### Comparing `aeromaps-0.1.0b0/aeromaps/gui/plots.py` & `aeromaps-0.1.1b0/aeromaps/gui/plots.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/gui/resources/Beta.png` & `aeromaps-0.1.1b0/aeromaps/gui/resources/Beta.png`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/gui/resources/aboutAeroMAPS_en.md` & `aeromaps-0.1.1b0/aeromaps/gui/resources/aboutAeroMAPS_en.md`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/gui/resources/aboutAeroMAPS_fr.md` & `aeromaps-0.1.1b0/aeromaps/gui/resources/aboutAeroMAPS_fr.md`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/gui/resources/logo-ISAE_SUPAERO.png` & `aeromaps-0.1.1b0/aeromaps/gui/resources/logo-ISAE_SUPAERO.png`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/models/air_transport/air_traffic/ask.py` & `aeromaps-0.1.1b0/aeromaps/models/air_transport/air_traffic/ask.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/models/air_transport/air_traffic/rpk.py` & `aeromaps-0.1.1b0/aeromaps/models/air_transport/air_traffic/rpk.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/models/air_transport/air_traffic/rtk.py` & `aeromaps-0.1.1b0/aeromaps/models/air_transport/air_traffic/rtk.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/models/air_transport/air_traffic/short_range_distribution.py` & `aeromaps-0.1.1b0/aeromaps/models/air_transport/air_traffic/short_range_distribution.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/models/air_transport/air_traffic/total_aircraft_distance.py` & `aeromaps-0.1.1b0/aeromaps/models/air_transport/air_traffic/total_aircraft_distance.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/models/air_transport/aircraft_energy/efficiency.py` & `aeromaps-0.1.1b0/aeromaps/models/air_transport/aircraft_energy/efficiency.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/models/air_transport/aircraft_energy/fuel_distribution.py` & `aeromaps-0.1.1b0/aeromaps/models/air_transport/aircraft_energy/fuel_distribution.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/models/air_transport/aircraft_energy/fuel_emissions.py` & `aeromaps-0.1.1b0/aeromaps/models/air_transport/aircraft_energy/fuel_emissions.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/models/air_transport/aircraft_energy/production_choices.py` & `aeromaps-0.1.1b0/aeromaps/models/air_transport/aircraft_energy/production_choices.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/models/air_transport/aircraft_fleet_and_operations/aircraft_fleet_and_operations.py` & `aeromaps-0.1.1b0/aeromaps/models/air_transport/aircraft_fleet_and_operations/aircraft_fleet_and_operations.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/models/air_transport/aircraft_fleet_and_operations/fleet/aircraft_efficiency.py` & `aeromaps-0.1.1b0/aeromaps/models/air_transport/aircraft_fleet_and_operations/fleet/aircraft_efficiency.py`

 * *Files 3% similar despite different names*

```diff
@@ -97,24 +97,24 @@
                 k, "energy_per_ask_without_operations_long_range_dropin_fuel"
             ] = self.df.loc[k - 1, "energy_per_ask_without_operations_long_range_dropin_fuel"] * (
                 1 - energy_per_ask_long_range_dropin_fuel_gain / 100
             )
 
         self.df.loc[
             2020, "energy_per_ask_without_operations_short_range_dropin_fuel"
-        ] = self.df.loc[2020, "energy_per_ask_without_operations_short_range_dropin_fuel"] * (
+        ] = self.df.loc[2019, "energy_per_ask_without_operations_short_range_dropin_fuel"] * (
             1 + covid_energy_intensity_per_ask_increase_2020 / 100
         )
         self.df.loc[
             2020, "energy_per_ask_without_operations_medium_range_dropin_fuel"
-        ] = self.df.loc[2020, "energy_per_ask_without_operations_medium_range_dropin_fuel"] * (
+        ] = self.df.loc[2019, "energy_per_ask_without_operations_medium_range_dropin_fuel"] * (
             1 + covid_energy_intensity_per_ask_increase_2020 / 100
         )
         self.df.loc[2020, "energy_per_ask_without_operations_long_range_dropin_fuel"] = self.df.loc[
-            2020, "energy_per_ask_without_operations_long_range_dropin_fuel"
+            2019, "energy_per_ask_without_operations_long_range_dropin_fuel"
         ] * (1 + covid_energy_intensity_per_ask_increase_2020 / 100)
 
         energy_per_ask_without_operations_short_range_dropin_fuel = self.df[
             "energy_per_ask_without_operations_short_range_dropin_fuel"
         ]
         energy_per_ask_without_operations_medium_range_dropin_fuel = self.df[
             "energy_per_ask_without_operations_medium_range_dropin_fuel"
@@ -247,111 +247,14 @@
             ask_long_range_dropin_fuel,
             ask_short_range_hydrogen,
             ask_medium_range_hydrogen,
             ask_long_range_hydrogen,
         )
 
 
-class FreightAircraftEfficiencySimple(AeromapsModel):
-    def __init__(self, name="freight_aircraft_efficiency_simple", *args, **kwargs):
-        super().__init__(name=name, *args, **kwargs)
-
-    def compute(
-        self,
-        energy_consumption_init: pd.Series = pd.Series(dtype="float64"),
-        rtk: pd.Series = pd.Series(dtype="float64"),
-        freight_energy_share_2019: float = 0.0,
-        energy_per_ask_short_range_dropin_fuel_gain: float = 0.0,
-        energy_per_ask_medium_range_dropin_fuel_gain: float = 0.0,
-        energy_per_ask_long_range_dropin_fuel_gain: float = 0.0,
-        ask_short_range: pd.Series = pd.Series(dtype="float64"),
-        ask_medium_range: pd.Series = pd.Series(dtype="float64"),
-        ask_long_range: pd.Series = pd.Series(dtype="float64"),
-        ask: pd.Series = pd.Series(dtype="float64"),
-        relative_energy_per_ask_hydrogen_wrt_dropin_short_range: float = 0.0,
-        relative_energy_per_ask_hydrogen_wrt_dropin_medium_range: float = 0.0,
-        relative_energy_per_ask_hydrogen_wrt_dropin_long_range: float = 0.0,
-        ask_short_range_hydrogen_share: pd.Series = pd.Series(dtype="float64"),
-        ask_medium_range_hydrogen_share: pd.Series = pd.Series(dtype="float64"),
-        ask_long_range_hydrogen_share: pd.Series = pd.Series(dtype="float64"),
-        covid_energy_intensity_per_ask_increase_2020: float = 0.0,
-    ) -> Tuple[pd.Series, pd.Series, pd.Series, pd.Series, pd.Series, pd.Series]:
-        """Energy consumption per RTK (without operations) calculation using simple models."""
-
-        # Initialization based on 2019 share: to correct to include load factor
-        for k in range(self.historic_start_year, self.prospection_start_year):
-            self.df.loc[k, "energy_per_rtk_without_operations_freight_dropin_fuel"] = (
-                energy_consumption_init.loc[k] / rtk.loc[k] * freight_energy_share_2019 / 100
-            )
-
-        # Projections
-        for k in range(self.prospection_start_year, self.end_year + 1):
-            self.df.loc[k, "energy_per_rtk_without_operations_freight_dropin_fuel"] = self.df.loc[
-                k - 1, "energy_per_rtk_without_operations_freight_dropin_fuel"
-            ] * (
-                1
-                - (
-                    energy_per_ask_short_range_dropin_fuel_gain
-                    / 100
-                    * (ask_short_range.loc[k] / ask.loc[k])
-                    + energy_per_ask_medium_range_dropin_fuel_gain
-                    / 100
-                    * (ask_medium_range.loc[k] / ask.loc[k])
-                    + energy_per_ask_long_range_dropin_fuel_gain
-                    / 100
-                    * (ask_long_range.loc[k] / ask.loc[k])
-                )
-            )
-
-        self.df.loc[2020, "energy_per_rtk_without_operations_freight_dropin_fuel"] = self.df.loc[
-            2020, "energy_per_rtk_without_operations_freight_dropin_fuel"
-        ] * (1 + covid_energy_intensity_per_ask_increase_2020 / 100)
-
-        energy_per_rtk_without_operations_freight_dropin_fuel = self.df[
-            "energy_per_rtk_without_operations_freight_dropin_fuel"
-        ]
-
-        energy_per_rtk_without_operations_freight_hydrogen = (
-            energy_per_rtk_without_operations_freight_dropin_fuel
-            * (
-                relative_energy_per_ask_hydrogen_wrt_dropin_short_range * (ask_short_range / ask)
-                + relative_energy_per_ask_hydrogen_wrt_dropin_medium_range
-                * (ask_medium_range / ask)
-                + relative_energy_per_ask_hydrogen_wrt_dropin_long_range * (ask_long_range / ask)
-            )
-        )
-
-        self.df.loc[
-            :, "energy_per_rtk_without_operations_freight_hydrogen"
-        ] = energy_per_rtk_without_operations_freight_hydrogen
-
-        rtk_hydrogen_share = (
-            ask_short_range_hydrogen_share * (ask_short_range / ask)
-            + ask_medium_range_hydrogen_share * (ask_medium_range / ask)
-            + ask_long_range_hydrogen_share * (ask_long_range / ask)
-        )
-        rtk_dropin_fuel_share = 100 - rtk_hydrogen_share
-        self.df.loc[:, "rtk_hydrogen_share"] = rtk_hydrogen_share
-        self.df.loc[:, "rtk_dropin_fuel_share"] = rtk_dropin_fuel_share
-
-        rtk_hydrogen = rtk * rtk_hydrogen_share / 100
-        rtk_dropin_fuel = rtk * rtk_dropin_fuel_share / 100
-        self.df.loc[:, "rtk_hydrogen"] = rtk_hydrogen
-        self.df.loc[:, "rtk_dropin_fuel"] = rtk_dropin_fuel
-
-        return (
-            energy_per_rtk_without_operations_freight_dropin_fuel,
-            energy_per_rtk_without_operations_freight_hydrogen,
-            rtk_dropin_fuel_share,
-            rtk_hydrogen_share,
-            rtk_dropin_fuel,
-            rtk_hydrogen,
-        )
-
-
 class PassengerAircraftEfficiencyComplex(AeromapsModel):
     def __init__(
         self, name="passenger_aircraft_efficiency_complex", fleet_model=None, *args, **kwargs
     ):
         super().__init__(name=name, *args, **kwargs)
         self.fleet_model = fleet_model
 
@@ -365,38 +268,14 @@
         short_range_rpk_share_2019: float = 0.0,
         medium_range_rpk_share_2019: float = 0.0,
         long_range_rpk_share_2019: float = 0.0,
         covid_energy_intensity_per_ask_increase_2020: float = 0.0,
         ask_short_range: pd.Series = pd.Series(dtype="float64"),
         ask_medium_range: pd.Series = pd.Series(dtype="float64"),
         ask_long_range: pd.Series = pd.Series(dtype="float64"),
-        # ask_short_range_dropin_fuel_share: pd.Series = pd.Series(dtype="float64"),
-        # ask_medium_range_dropin_fuel_share: pd.Series = pd.Series(dtype="float64"),
-        # ask_long_range_dropin_fuel_share: pd.Series = pd.Series(dtype="float64"),
-        # ask_short_range_hydrogen_share: pd.Series = pd.Series(dtype="float64"),
-        # ask_medium_range_hydrogen_share: pd.Series = pd.Series(dtype="float64"),
-        # ask_long_range_hydrogen_share: pd.Series = pd.Series(dtype="float64"),
-        # energy_per_ask_without_operations_short_range_dropin_fuel: pd.Series = pd.Series(
-        #     dtype="float64"
-        # ),
-        # energy_per_ask_without_operations_medium_range_dropin_fuel: pd.Series = pd.Series(
-        #     dtype="float64"
-        # ),
-        # energy_per_ask_without_operations_long_range_dropin_fuel: pd.Series = pd.Series(
-        #     dtype="float64"
-        # ),
-        # energy_per_ask_without_operations_short_range_hydrogen: pd.Series = pd.Series(
-        #     dtype="float64"
-        # ),
-        # energy_per_ask_without_operations_medium_range_hydrogen: pd.Series = pd.Series(
-        #     dtype="float64"
-        # ),
-        # energy_per_ask_without_operations_long_range_hydrogen: pd.Series = pd.Series(
-        #     dtype="float64"
-        # ),
     ) -> Tuple[
         pd.Series,
         pd.Series,
         pd.Series,
         pd.Series,
         pd.Series,
         pd.Series,
@@ -486,24 +365,24 @@
             ] = energy_per_ask_without_operations_medium_range_dropin_fuel.loc[k]
             self.df.loc[
                 k, "energy_per_ask_without_operations_long_range_dropin_fuel"
             ] = energy_per_ask_without_operations_long_range_dropin_fuel.loc[k]
 
         self.df.loc[
             2020, "energy_per_ask_without_operations_short_range_dropin_fuel"
-        ] = self.df.loc[2020, "energy_per_ask_without_operations_short_range_dropin_fuel"] * (
+        ] = self.df.loc[2019, "energy_per_ask_without_operations_short_range_dropin_fuel"] * (
             1 + covid_energy_intensity_per_ask_increase_2020 / 100
         )
         self.df.loc[
             2020, "energy_per_ask_without_operations_medium_range_dropin_fuel"
-        ] = self.df.loc[2020, "energy_per_ask_without_operations_medium_range_dropin_fuel"] * (
+        ] = self.df.loc[2019, "energy_per_ask_without_operations_medium_range_dropin_fuel"] * (
             1 + covid_energy_intensity_per_ask_increase_2020 / 100
         )
         self.df.loc[2020, "energy_per_ask_without_operations_long_range_dropin_fuel"] = self.df.loc[
-            2020, "energy_per_ask_without_operations_long_range_dropin_fuel"
+            2019, "energy_per_ask_without_operations_long_range_dropin_fuel"
         ] * (1 + covid_energy_intensity_per_ask_increase_2020 / 100)
 
         energy_per_ask_without_operations_short_range_dropin_fuel = self.df[
             "energy_per_ask_without_operations_short_range_dropin_fuel"
         ]
         energy_per_ask_without_operations_medium_range_dropin_fuel = self.df[
             "energy_per_ask_without_operations_medium_range_dropin_fuel"
@@ -593,7 +472,177 @@
             ask_short_range_dropin_fuel,
             ask_medium_range_dropin_fuel,
             ask_long_range_dropin_fuel,
             ask_short_range_hydrogen,
             ask_medium_range_hydrogen,
             ask_long_range_hydrogen,
         )
+
+
+class FreightAircraftEfficiency(AeromapsModel):
+    def __init__(self, name="freight_aircraft_efficiency", *args, **kwargs):
+        super().__init__(name=name, *args, **kwargs)
+
+    def compute(
+        self,
+        energy_consumption_init: pd.Series = pd.Series(dtype="float64"),
+        rtk: pd.Series = pd.Series(dtype="float64"),
+        freight_energy_share_2019: float = 0.0,
+        energy_per_ask_without_operations_short_range_dropin_fuel: pd.Series = pd.Series(
+            dtype="float64"
+        ),
+        energy_per_ask_without_operations_medium_range_dropin_fuel: pd.Series = pd.Series(
+            dtype="float64"
+        ),
+        energy_per_ask_without_operations_long_range_dropin_fuel: pd.Series = pd.Series(
+            dtype="float64"
+        ),
+        energy_per_ask_without_operations_short_range_hydrogen: pd.Series = pd.Series(
+            dtype="float64"
+        ),
+        energy_per_ask_without_operations_medium_range_hydrogen: pd.Series = pd.Series(
+            dtype="float64"
+        ),
+        energy_per_ask_without_operations_long_range_hydrogen: pd.Series = pd.Series(
+            dtype="float64"
+        ),
+        ask: pd.Series = pd.Series(dtype="float64"),
+        ask_short_range: pd.Series = pd.Series(dtype="float64"),
+        ask_medium_range: pd.Series = pd.Series(dtype="float64"),
+        ask_long_range: pd.Series = pd.Series(dtype="float64"),
+        ask_short_range_dropin_fuel: pd.Series = pd.Series(dtype="float64"),
+        ask_medium_range_dropin_fuel: pd.Series = pd.Series(dtype="float64"),
+        ask_long_range_dropin_fuel: pd.Series = pd.Series(dtype="float64"),
+        ask_short_range_hydrogen_share: pd.Series = pd.Series(dtype="float64"),
+        ask_medium_range_hydrogen_share: pd.Series = pd.Series(dtype="float64"),
+        ask_long_range_hydrogen_share: pd.Series = pd.Series(dtype="float64"),
+        covid_energy_intensity_per_ask_increase_2020: float = 0.0,
+    ) -> Tuple[pd.Series, pd.Series, pd.Series, pd.Series, pd.Series, pd.Series]:
+        """Energy consumption per RTK (without operations) calculation."""
+
+        # Initialization based on 2019 share: to correct to include load factor
+        for k in range(self.historic_start_year, self.prospection_start_year):
+            self.df.loc[k, "energy_per_rtk_without_operations_freight_dropin_fuel"] = (
+                energy_consumption_init.loc[k] / rtk.loc[k] * freight_energy_share_2019 / 100
+            )
+
+        # Projections
+        energy_per_rtk_without_operations_freight_dropin_fuel_short_range_k = self.df.loc[
+            2019, "energy_per_rtk_without_operations_freight_dropin_fuel"
+        ]
+        energy_per_rtk_without_operations_freight_dropin_fuel_medium_range_k = self.df.loc[
+            2019, "energy_per_rtk_without_operations_freight_dropin_fuel"
+        ]
+        energy_per_rtk_without_operations_freight_dropin_fuel_long_range_k = self.df.loc[
+            2019, "energy_per_rtk_without_operations_freight_dropin_fuel"
+        ]
+        for k in range(self.prospection_start_year, self.end_year + 1):
+            energy_per_rtk_without_operations_freight_dropin_fuel_short_range_k = (
+                energy_per_rtk_without_operations_freight_dropin_fuel_short_range_k
+                * energy_per_ask_without_operations_short_range_dropin_fuel.loc[k]
+                / energy_per_ask_without_operations_short_range_dropin_fuel.loc[k - 1]
+            )
+            energy_per_rtk_without_operations_freight_dropin_fuel_medium_range_k = (
+                energy_per_rtk_without_operations_freight_dropin_fuel_medium_range_k
+                * energy_per_ask_without_operations_medium_range_dropin_fuel.loc[k]
+                / energy_per_ask_without_operations_medium_range_dropin_fuel.loc[k - 1]
+            )
+            energy_per_rtk_without_operations_freight_dropin_fuel_long_range_k = (
+                energy_per_rtk_without_operations_freight_dropin_fuel_long_range_k
+                * energy_per_ask_without_operations_long_range_dropin_fuel.loc[k]
+                / energy_per_ask_without_operations_long_range_dropin_fuel.loc[k - 1]
+            )
+            self.df.loc[k, "energy_per_rtk_without_operations_freight_dropin_fuel"] = (
+                energy_per_rtk_without_operations_freight_dropin_fuel_short_range_k
+                * ask_short_range_dropin_fuel.loc[k]
+                / (
+                    ask_short_range_dropin_fuel.loc[k]
+                    + ask_medium_range_dropin_fuel.loc[k]
+                    + ask_long_range_dropin_fuel.loc[k]
+                )
+                + energy_per_rtk_without_operations_freight_dropin_fuel_medium_range_k
+                * ask_medium_range_dropin_fuel.loc[k]
+                / (
+                    ask_short_range_dropin_fuel.loc[k]
+                    + ask_medium_range_dropin_fuel.loc[k]
+                    + ask_long_range_dropin_fuel.loc[k]
+                )
+                + energy_per_rtk_without_operations_freight_dropin_fuel_long_range_k
+                * ask_long_range_dropin_fuel.loc[k]
+                / (
+                    ask_short_range_dropin_fuel.loc[k]
+                    + ask_medium_range_dropin_fuel.loc[k]
+                    + ask_long_range_dropin_fuel.loc[k]
+                )
+            )
+
+        # Covid
+        self.df.loc[2020, "energy_per_rtk_without_operations_freight_dropin_fuel"] = self.df.loc[
+            2019, "energy_per_rtk_without_operations_freight_dropin_fuel"
+        ] * (1 + covid_energy_intensity_per_ask_increase_2020 / 100)
+
+        energy_per_rtk_without_operations_freight_dropin_fuel = self.df[
+            "energy_per_rtk_without_operations_freight_dropin_fuel"
+        ]
+
+        rtk_hydrogen_share = (
+            ask_short_range_hydrogen_share * (ask_short_range / ask)
+            + ask_medium_range_hydrogen_share * (ask_medium_range / ask)
+            + ask_long_range_hydrogen_share * (ask_long_range / ask)
+        )
+        rtk_dropin_fuel_share = 100 - rtk_hydrogen_share
+        self.df.loc[:, "rtk_hydrogen_share"] = rtk_hydrogen_share
+        self.df.loc[:, "rtk_dropin_fuel_share"] = rtk_dropin_fuel_share
+
+        rtk_hydrogen = rtk * rtk_hydrogen_share / 100
+        rtk_dropin_fuel = rtk * rtk_dropin_fuel_share / 100
+        self.df.loc[:, "rtk_hydrogen"] = rtk_hydrogen
+        self.df.loc[:, "rtk_dropin_fuel"] = rtk_dropin_fuel
+
+        relative_energy_per_ask_hydrogen_wrt_dropin_short_range = (
+            energy_per_ask_without_operations_short_range_hydrogen
+            / energy_per_ask_without_operations_short_range_dropin_fuel
+        )
+        relative_energy_per_ask_hydrogen_wrt_dropin_medium_range = (
+            energy_per_ask_without_operations_medium_range_hydrogen
+            / energy_per_ask_without_operations_medium_range_dropin_fuel
+        )
+        relative_energy_per_ask_hydrogen_wrt_dropin_long_range = (
+            energy_per_ask_without_operations_long_range_hydrogen
+            / energy_per_ask_without_operations_long_range_dropin_fuel
+        )
+
+        for k in range(self.historic_start_year, self.end_year + 1):
+            if rtk_hydrogen_share.loc[k] == 0:
+                self.df.loc[k, "energy_per_rtk_without_operations_freight_hydrogen"] = self.df.loc[
+                    k, "energy_per_rtk_without_operations_freight_dropin_fuel"
+                ]
+            else:
+                self.df.loc[
+                    k, "energy_per_rtk_without_operations_freight_hydrogen"
+                ] = energy_per_rtk_without_operations_freight_dropin_fuel.loc[k] * (
+                    relative_energy_per_ask_hydrogen_wrt_dropin_short_range.loc[k]
+                    * ask_short_range_hydrogen_share.loc[k]
+                    * (ask_short_range.loc[k] / ask.loc[k])
+                    / rtk_hydrogen_share.loc[k]
+                    + relative_energy_per_ask_hydrogen_wrt_dropin_medium_range.loc[k]
+                    * ask_medium_range_hydrogen_share.loc[k]
+                    * (ask_medium_range.loc[k] / ask.loc[k])
+                    / rtk_hydrogen_share.loc[k]
+                    + relative_energy_per_ask_hydrogen_wrt_dropin_long_range.loc[k]
+                    * ask_long_range_hydrogen_share.loc[k]
+                    * (ask_long_range.loc[k] / ask.loc[k])
+                    / rtk_hydrogen_share.loc[k]
+                )
+
+        energy_per_rtk_without_operations_freight_hydrogen = self.df[
+            "energy_per_rtk_without_operations_freight_hydrogen"
+        ]
+
+        return (
+            energy_per_rtk_without_operations_freight_dropin_fuel,
+            energy_per_rtk_without_operations_freight_hydrogen,
+            rtk_dropin_fuel_share,
+            rtk_hydrogen_share,
+            rtk_dropin_fuel,
+            rtk_hydrogen,
+        )
```

### Comparing `aeromaps-0.1.0b0/aeromaps/models/air_transport/aircraft_fleet_and_operations/fleet/fleet_model.py` & `aeromaps-0.1.1b0/aeromaps/models/air_transport/aircraft_fleet_and_operations/fleet/fleet_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,16 @@
     def __init__(self, name="fleet_model", fleet=None, *args, **kwargs):
         super().__init__(name, *args, **kwargs)
         self.fleet = fleet
 
     def compute(
         self,
     ):
-
+        # Start from empty dataframe
+        self.df = self.df.filter([])
         # Single aircraft share computation (for obtaining the main plot on fleet renewal)
         for category in self.fleet.categories.values():
 
             limit = 2
             life_base = 25
             parameter_base = np.log(100 / limit - 1) / (life_base / 2)
             parameter_renewal = np.log(100 / limit - 1) / (category.parameters.life / 2)
@@ -715,15 +716,19 @@
         # Considering fixed category distribution in 2019
         # var_name = "global_fleet:energy_consumption"
         # self.df[var_name] = self.df["Short Range" + ":energy_consumption"] * 0.272
         # self.df[var_name] += self.df["Medium Range" + ":energy_consumption"] * 0.351
         # self.df[var_name] += self.df["Long Range" + ":energy_consumption"] * 0.377
 
     def plot(self):
-        x = np.linspace(self.prospection_start_year, self.end_year, len(self.df.index))
+        x = np.linspace(
+            self.prospection_start_year,
+            self.end_year,
+            self.end_year - self.prospection_start_year + 1,
+        )
 
         categories = list(self.fleet.categories.values())
 
         f, axs = plt.subplots(2, len(categories), figsize=(20, 10))
 
         for i, category in enumerate(categories):
             # Top plot
@@ -733,29 +738,29 @@
             subcategory = category.subcategories[0]
             # Old reference aircraft
             var_name = (
                 category.name + ":" + subcategory.name + ":" + "old_reference:single_aircraft_share"
             )
             ax.fill_between(
                 x,
-                self.df[var_name],
+                self.df.loc[self.prospection_start_year : self.end_year, var_name],
                 label=subcategory.name + " - Old reference aircraft",
             )
 
             # Recent reference aircraft
             var_name = (
                 category.name
                 + ":"
                 + subcategory.name
                 + ":"
                 + "recent_reference:single_aircraft_share"
             )
             ax.fill_between(
                 x,
-                self.df[var_name],
+                self.df.loc[self.prospection_start_year : self.end_year, var_name],
                 label=subcategory.name + " - Recent reference aircraft",
             )
 
             for j, subcategory in category.subcategories.items():
 
                 # New aircraft
                 for aircraft in subcategory.aircraft.values():
@@ -765,39 +770,47 @@
                         + subcategory.name
                         + ":"
                         + aircraft.name
                         + ":single_aircraft_share"
                     )
                     ax.fill_between(
                         x,
-                        self.df[var_name],
+                        self.df.loc[self.prospection_start_year : self.end_year, var_name],
                         label=subcategory.name + " - " + aircraft.name,
                     )
 
             ax.set_xlim(self.prospection_start_year, self.end_year)
             ax.set_ylim(0, 100)
             ax.legend(loc="upper left", prop={"size": 8})
             ax.set_xlabel("Year")
             ax.set_ylabel("Share in fleet [%]")
             ax.set_title(categories[i].name)
 
             # Bottom plot
             ax = axs[1, i]
-            ax.plot(x, self.df[category.name + ":energy_consumption"])
+            ax.plot(
+                x,
+                self.df.loc[
+                    self.prospection_start_year : self.end_year,
+                    category.name + ":energy_consumption",
+                ],
+            )
 
             ax.set_xlim(self.prospection_start_year, self.end_year)
             ax.set_xlabel("Year")
             ax.set_ylabel("Fleet mean energy consumption [MJ/ASK]")
             # ax.set_title(categories[i].name)
 
         plt.plot()
         # plt.savefig("fleet_renewal.pdf")
 
     def _compute(self, life, entry_into_service_year, share, recent=False):
-        x = np.linspace(self.prospection_start_year, self.end_year, len(self.df.index))
+        x = np.linspace(
+            self.historic_start_year, self.end_year, self.end_year - self.historic_start_year + 1
+        )
 
         # Intermediate variable for S-shaped function
         limit = 2
         growth_rate = np.log(100 / limit - 1) / (life / 2)
 
         if not recent:
             midpoint_year = entry_into_service_year + life / 2
```

### Comparing `aeromaps-0.1.0b0/aeromaps/models/air_transport/aircraft_fleet_and_operations/load_factor/load_factor.py` & `aeromaps-0.1.1b0/aeromaps/models/air_transport/aircraft_fleet_and_operations/load_factor/load_factor.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/models/air_transport/aircraft_fleet_and_operations/non_co2/non_co2.py` & `aeromaps-0.1.1b0/aeromaps/models/air_transport/aircraft_fleet_and_operations/non_co2/non_co2.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/models/air_transport/aircraft_fleet_and_operations/operations/operations.py` & `aeromaps-0.1.1b0/aeromaps/models/air_transport/aircraft_fleet_and_operations/operations/operations.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/models/air_transport/parameters.py` & `aeromaps-0.1.1b0/aeromaps/models/air_transport/parameters.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/models/base.py` & `aeromaps-0.1.1b0/aeromaps/models/base.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/models/impacts/climate/climate.py` & `aeromaps-0.1.1b0/aeromaps/models/impacts/climate/climate.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/models/impacts/effective_radiative_forcing/effective_radiative_forcing.py` & `aeromaps-0.1.1b0/aeromaps/models/impacts/effective_radiative_forcing/effective_radiative_forcing.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/models/impacts/effective_radiative_forcing/test.py` & `aeromaps-0.1.1b0/aeromaps/models/impacts/effective_radiative_forcing/test.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/models/impacts/emissions/co2_emissions.py` & `aeromaps-0.1.1b0/aeromaps/models/impacts/emissions/co2_emissions.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/models/impacts/emissions/non_co2_emissions.py` & `aeromaps-0.1.1b0/aeromaps/models/impacts/emissions/non_co2_emissions.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/models/impacts/energy_resources/energy_consumption.py` & `aeromaps-0.1.1b0/aeromaps/models/impacts/energy_resources/energy_consumption.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/models/impacts/energy_resources/resources_consumption.py` & `aeromaps-0.1.1b0/aeromaps/models/impacts/energy_resources/resources_consumption.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/models/impacts/equivalent_co2_emissions/equivalent_co2_emissions.py` & `aeromaps-0.1.1b0/aeromaps/models/impacts/equivalent_co2_emissions/equivalent_co2_emissions.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/models/impacts/others/comparison.py` & `aeromaps-0.1.1b0/aeromaps/models/impacts/others/comparison.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/models/impacts/others/others.py` & `aeromaps-0.1.1b0/aeromaps/models/impacts/others/others.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/models/impacts/parameters.py` & `aeromaps-0.1.1b0/aeromaps/models/impacts/parameters.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/models/parameters.py` & `aeromaps-0.1.1b0/aeromaps/models/parameters.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/models/sustainability_assessment/climate/carbon_budgets.py` & `aeromaps-0.1.1b0/aeromaps/models/sustainability_assessment/climate/carbon_budgets.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/models/sustainability_assessment/climate/equivalent_carbon_budgets.py` & `aeromaps-0.1.1b0/aeromaps/models/sustainability_assessment/climate/equivalent_carbon_budgets.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/models/sustainability_assessment/climate/test.py` & `aeromaps-0.1.1b0/aeromaps/models/sustainability_assessment/climate/test.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/models/sustainability_assessment/energy/resources_availability.py` & `aeromaps-0.1.1b0/aeromaps/models/sustainability_assessment/energy/resources_availability.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/models/sustainability_assessment/parameters.py` & `aeromaps-0.1.1b0/aeromaps/models/sustainability_assessment/parameters.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/notebooks/basic_example.ipynb` & `aeromaps-0.1.1b0/aeromaps/notebooks/basic_example.ipynb`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/notebooks/fleet.ipynb` & `aeromaps-0.1.1b0/aeromaps/notebooks/fleet.ipynb`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/plots/__init__.py` & `aeromaps-0.1.1b0/aeromaps/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/plots/air_traffic.py` & `aeromaps-0.1.1b0/aeromaps/plots/air_traffic.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/plots/aircraft_energy.py` & `aeromaps-0.1.1b0/aeromaps/plots/aircraft_energy.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/plots/aircraft_fleet_and_operations.py` & `aeromaps-0.1.1b0/aeromaps/plots/aircraft_fleet_and_operations.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/plots/climate.py` & `aeromaps-0.1.1b0/aeromaps/plots/climate.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/plots/emissions.py` & `aeromaps-0.1.1b0/aeromaps/plots/emissions.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/plots/energy_resources.py` & `aeromaps-0.1.1b0/aeromaps/plots/energy_resources.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/plots/indicators.py` & `aeromaps-0.1.1b0/aeromaps/plots/indicators.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/plots/main.py` & `aeromaps-0.1.1b0/aeromaps/plots/main.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/plots/sustainability_assessment.py` & `aeromaps-0.1.1b0/aeromaps/plots/sustainability_assessment.py`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/resources/data/data.xlsx` & `aeromaps-0.1.1b0/aeromaps/resources/data/data.xlsx`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/resources/data/data_information.csv` & `aeromaps-0.1.1b0/aeromaps/resources/data/data_information.csv`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/resources/data/outputs.json` & `aeromaps-0.1.1b0/aeromaps/resources/data/outputs.json`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/aeromaps/resources/data/parameters.json` & `aeromaps-0.1.1b0/aeromaps/resources/data/parameters.json`

 * *Files identical despite different names*

### Comparing `aeromaps-0.1.0b0/pyproject.toml` & `aeromaps-0.1.1b0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.black]
 line-length = 100
 
 [tool.poetry]
 name = "aeromaps"
-version = "v0.1.0-beta"
+version = "v0.1.1-beta"
 description = "AeroMAPS: Multidisciplinary Assessment of Prospective Scenarios for air transport"
-readme = "README.rst"
+readme = "README.md"
 authors = [
     "Thomas PLANES <thomas.planes@isae-supaero.fr>",
     "Scott DELBECQ <scott.delbecq@isae-supaero.fr>",
     "Antoine SALGAS <antoine.salgas@isae-supaero.fr>",
 ]
 keywords = [
     "air transport",
@@ -31,15 +31,15 @@
 jupyterlab = "^3.3.0"
 matplotlib = "^3.1.2, <3.7.0"
 ipywidgets = "^8.0.6"
 ipysheet = ">=0.5.0, <1"
 plotly = "^5.0.0"
 markdown = "^3.4.3"
 ipympl = "^0.9.3"
-gemseo = "^5.0.0rc0"
+gemseo = "^5.0.0"
 aenum = "^3.1.12"
 ipydatagrid = "^1.1.14"
 ipytree = "^0.2.2"
 docstring-inheritance = "^1.0.0"
 dacite = "^1.8.0"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `aeromaps-0.1.0b0/PKG-INFO` & `aeromaps-0.1.1b0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: aeromaps
-Version: 0.1.0b0
+Version: 0.1.1b0
 Summary: AeroMAPS: Multidisciplinary Assessment of Prospective Scenarios for air transport
 Home-page: https://github.com/AeroMAPS/AeroMAPS
 License: GPL-3.0-only
 Keywords: air transport,climate change,prospective scenarios,energy issues
 Author: Thomas PLANES
 Author-email: thomas.planes@isae-supaero.fr
 Requires-Python: >=3.8.0,<3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: aenum (>=3.1.12,<4.0.0)
 Requires-Dist: dacite (>=1.8.0,<2.0.0)
 Requires-Dist: docstring-inheritance (>=1.0.0,<2.0.0)
-Requires-Dist: gemseo (>=5.0.0rc0,<6.0.0)
+Requires-Dist: gemseo (>=5.0.0,<6.0.0)
 Requires-Dist: ipydatagrid (>=1.1.14,<2.0.0)
 Requires-Dist: ipympl (>=0.9.3,<0.10.0)
 Requires-Dist: ipysheet (>=0.5.0,<1)
 Requires-Dist: ipytree (>=0.2.2,<0.3.0)
 Requires-Dist: ipywidgets (>=8.0.6,<9.0.0)
 Requires-Dist: jupyterlab (>=3.3.0,<4.0.0)
 Requires-Dist: markdown (>=3.4.3,<4.0.0)
@@ -27,52 +27,54 @@
 Requires-Dist: numpy (>=1.20.3,<2.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=1.1.0,<2.0.0)
 Requires-Dist: plotly (>=5.0.0,<6.0.0)
 Requires-Dist: scipy (>=1.4.1,<2.0.0)
 Requires-Dist: voila (>=0.4.0,<0.5.0)
 Requires-Dist: xlrd (==1.2.0)
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 
-.. image:: https://mybinder.org/badge_logo.svg
- :target: https://mybinder.org/v2/gh/AeroMAPS/AeroMAPS/HEAD?urlpath=voila%2Frender%2Faeromaps%2Fapp.ipynb
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/AeroMAPS/AeroMAPS/HEAD)
 
 AeroMAPS: Multidisciplinary Assessment of Prospective Scenarios for air transport
 =================================================================================
 
 AeroMAPS is a framework for performing Multidisciplinary Assessment of Prospective Scenarios for air transport. For
 instance, it allows simulating and analyzing scenarios for reducing aviation climate impacts through various levers of
 action. It is intended to become a sectoral Integrated Assessment Model (IAM) taking into account technological,
 environmental, sociological, economic and other considerations. It aims to assess the sustainability of simulated air
 transport transition scenarios on multiple criteria.
 
-AeroMAPS is licensed under the `GPL-3.0 <https://www.gnu.org/licenses/gpl-3.0.en.html>`_ license.
+AeroMAPS is licensed under the [GPL-3.0](https://www.gnu.org/licenses/gpl-3.0.en.html) license.
 
-A `documentation <https://aeromaps.github.io/AeroMAPS/>`_ is available for more details on AeroMAPS.
+A [documentation](https://aeromaps.github.io/AeroMAPS/) is available for more details on AeroMAPS.
 
 
 Quick start
 -----------
 
 For a quick start in order to discover the different features of AeroMAPS,
 a graphical user interface has been developed for facilitating the first uses.
 It is available at the following address: https://aeromaps.isae-supaero.fr/
+Another solution is to use the [Binder-hosted graphical user interface](https://mybinder.org/v2/gh/AeroMAPS/AeroMAPS/HEAD?urlpath=voila%2Frender%2Faeromaps%2Fapp.ipynb).
 
 
 Quick installation
 ------------------
 
-The use of the Python Package Index (`PyPI <https://pypi.org/>`_) is the simplest method for installing AeroMAPS.
+The use of the Python Package Index ([PyPI](https://pypi.org/)) is the simplest method for installing AeroMAPS.
 More details and other solutions are provided in the documentation.
 
-**Prerequisite**: AeroMAPS needs at least **Python 3.8.0**.
+**Prerequisite**: AeroMAPS needs at least Python 3.8.0.
 
-You can install the latest version with this command::
+You can install the latest version with this command:
 
-    pip install --upgrade aeromaps
+``` {.bash}
+$ pip install --upgrade aeromaps
+```
 
 
 Citation
 --------
 
 If you use AeroMAPS in your work, please cite the following reference. Other references are available in the
 documentation.
```

