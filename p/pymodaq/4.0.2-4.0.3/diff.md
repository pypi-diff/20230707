# Comparing `tmp/pymodaq-4.0.2.tar.gz` & `tmp/pymodaq-4.0.3.tar.gz`

## Comparing `pymodaq-4.0.2.tar` & `pymodaq-4.0.3.tar`

### file list

```diff
@@ -1,418 +1,418 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/__init__.py
--rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/__init__.py
--rw-r--r--   0        0        0     8738 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/daq_utils.py
--rw-r--r--   0        0        0    61748 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/dashboard.py
--rw-r--r--   0        0        0    74359 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/icon.ico
--rw-r--r--   0        0        0    53114 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/splash.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/control_modules/__init__.py
--rw-r--r--   0        0        0    41489 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/control_modules/daq_move.py
--rw-r--r--   0        0        0    12919 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/control_modules/daq_move_ui.py
--rw-r--r--   0        0        0    64322 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/control_modules/daq_viewer.py
--rw-r--r--   0        0        0    15462 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/control_modules/daq_viewer_ui.py
--rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/control_modules/mocks.py
--rw-r--r--   0        0        0    30500 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/control_modules/move_utility_classes.py
--rw-r--r--   0        0        0     8250 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/control_modules/utils.py
--rw-r--r--   0        0        0    26665 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/control_modules/viewer_utility_classes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/__init__.py
--rw-r--r--   0        0        0    11127 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/custom_app.py
--rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/custom_viewer.py
--rw-r--r--   0        0        0     6104 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/function_plotter.py
--rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/nonlinearscanner.py
--rw-r--r--   0        0        0     7187 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/parameter_ex.py
--rw-r--r--   0        0        0    15774 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/preset_MockCamera.xml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Client.aliases
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Client.lvlps
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Client.lvproj
--rw-r--r--   0        0        0    69358 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Client.vi
--rw-r--r--   0        0        0    21969 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Server_1Dgaussian.vi
--rw-r--r--   0        0        0    29785 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Server_2Dgaussian.vi
--rw-r--r--   0        0        0    18148 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_read_cmd.vi
--rw-r--r--   0        0        0    20622 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_read_float.vi
--rw-r--r--   0        0        0    11828 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_read_int.vi
--rw-r--r--   0        0        0    23025 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_data.vi
--rw-r--r--   0        0        0     9072 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_int.vi
--rw-r--r--   0        0        0    19039 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_scalar.vi
--rw-r--r--   0        0        0    19791 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_string.vi
--rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/client_state.ctl
--rw-r--r--   0        0        0     4618 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/cmd_types.ctl
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/extensions/__init__.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/extensions/console.py
--rw-r--r--   0        0        0    19346 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/extensions/daq_logger.py
--rw-r--r--   0        0        0    56107 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/extensions/daq_scan.py
--rw-r--r--   0        0        0    10123 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/extensions/daq_scan_ui.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/extensions/h5browser.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/extensions/utils.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/extensions/pid/__init__.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/extensions/pid/daq_move_PID.py
--rw-r--r--   0        0        0    29797 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/extensions/pid/pid_controller.py
--rw-r--r--   0        0        0     8074 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/extensions/pid/utils.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/post_treatment/__init__.py
--rw-r--r--   0        0        0     8247 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/post_treatment/load_and_plot.py
--rw-r--r--   0        0        0    11562 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/post_treatment/process_to_scalar.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/post_treatment/daq_analysis/__init__.py
--rw-r--r--   0        0        0    24346 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/post_treatment/daq_analysis/daq_analysis_main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/post_treatment/daq_measurement/__init__.py
--rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/post_treatment/daq_measurement/daq_measurement_GUI.py
--rw-r--r--   0        0        0     7037 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/post_treatment/daq_measurement/daq_measurement_GUI.ui
--rw-r--r--   0        0        0    17093 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/post_treatment/daq_measurement/daq_measurement_main.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/post_treatment/daq_measurement/process_from_QtDesigner_DAQ_Measurement_GUI.bat
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/VERSION
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/__init__.py
--rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/config_template.toml
--rw-r--r--   0        0        0    31231 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/preset_default.xml
--rw-r--r--   0        0        0     9320 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/triangulation_data.npy
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/QtDesigner_ressources.bat
--rw-r--r--   0        0        0     9800 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/QtDesigner_ressources.qrc
--rw-r--r--   0        0        0  8225442 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/QtDesigner_ressources_rc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/__init__.py
--rw-r--r--   0        0        0     5703 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/icons.svg
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/1d.png
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/2d.png
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/3d.png
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Add2.png
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Add_Step.png
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Approve.png
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Approve_All.png
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Browse_Dir_Path.png
--rw-r--r--   0        0        0    47401 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Calculator.png
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ChnGroup.png
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ChnNum.png
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ChnText.png
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ChnTime.png
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ChnWave.png
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Close3.png
--rw-r--r--   0        0        0    47830 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/CollapseAll.png
--rw-r--r--   0        0        0    48054 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/CollapseAll_32.png
--rw-r--r--   0        0        0    48959 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ColorPicker.png
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Contract.png
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Create.png
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/DeleteLayer.png
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EditOpen.png
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EditRedo.png
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EditUndo.png
--rw-r--r--   0        0        0    49034 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Ellipse.png
--rw-r--r--   0        0        0    48413 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EllipseFilled.png
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Error.png
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ErrorMessage.png
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Error_16.png
--rw-r--r--   0        0        0    48491 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Exit.png
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Expand.png
--rw-r--r--   0        0        0    47692 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ExpandAll.png
--rw-r--r--   0        0        0    48102 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ExpandAll_32.png
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/FFT.png
--rw-r--r--   0        0        0    89487 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/HLM.ico
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Help.png
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Help_32.png
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Histogram.png
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/LUT_LookUpTable.png
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MagnifyingGlass.png
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MagnifyingGlass_24.png
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Marker.png
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Math.png
--rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MeasurementStudio_32.png
--rw-r--r--   0        0        0    48221 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Move.png
--rw-r--r--   0        0        0    47229 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MoveDown.png
--rw-r--r--   0        0        0    47258 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MoveUp.png
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Multiply.png
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/NewFile.png
--rw-r--r--   0        0        0    48742 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/NewLayer.png
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/New_File.png
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/New_Folder.png
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open.png
--rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_1D.png
--rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_2D.png
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_File.png
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_File_32.png
--rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_sim.png
--rw-r--r--   0        0        0    48140 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Options.png
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Oscilloscope.png
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Oscilloscope_16.png
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Pass.png
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/RGB.png
--rw-r--r--   0        0        0    47228 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Rectangle.png
--rw-r--r--   0        0        0    47093 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/RectangleFilled.png
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Redo.png
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Refresh.png
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Refresh2.png
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Refresh_32.png
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Region.png
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Rendezvous.png
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SELECT.png
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Save.png
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SaveAll.png
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SaveAll_32.png
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SaveAs.png
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SaveAs_32.png
--rw-r--r--   0        0        0    49529 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Save_24.png
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Save_32.png
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Search.png
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SelectPolygon.png
--rw-r--r--   0        0        0    47940 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Select_24.png
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Settings.png
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snap&Save.png
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot.png
--rw-r--r--   0        0        0    49414 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot2.png
--rw-r--r--   0        0        0    49581 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot2_16.png
--rw-r--r--   0        0        0    52734 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot2_32.png
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Spreadsheet.png
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Statistics.png
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Statistics2.png
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Status.png
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Subtract.png
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Vision.png
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Volts.png
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Wait2.png
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Zoom_1_1.png
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Zoom_in.png
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Zoom_out.png
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Zoom_to_Selection.png
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/abort.png
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/advanced2.png
--rw-r--r--   0        0        0    47292 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/autoscale.png
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/b_icon.png
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/back.png
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/bg_icon.png
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/camera.png
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/camera_snap.png
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/cartesian.png
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/clear2.png
--rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/clear_ROI.png
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/close2.png
--rw-r--r--   0        0        0    47742 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/cluster2.png
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/color.png
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/color2.png
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/continuous.png
--rw-r--r--   0        0        0    47210 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/data.png
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/delay.png
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/download.png
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/download2.png
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/error2.png
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ethernet.png
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/exit2.png
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/fan.png
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/filter2.png
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/g_icon.png
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/gear2.png
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/go_to.png
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/go_to_1.png
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/go_to_2.png
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/grab.png
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/graph.png
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/greenLight2.png
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/greenLight2_32.png
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/green_light.png
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/grey_icon.png
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/greyscale.png
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/help1.png
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/help1_32.png
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/home2.png
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/information2.png
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ini.png
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/integrator.png
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/joystick.png
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_green.png
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_green_16.png
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_red.png
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_red_16.png
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_yellow.png
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_yellow_16.png
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/limiter.png
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/load_ROI.png
--rw-r--r--   0        0        0    50113 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meshPlot.png
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meter.png
--rw-r--r--   0        0        0    47361 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meter2.png
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meter_32.png
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/move_contour.png
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/move_straight_line.png
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/movie.png
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/multi_point.png
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/multiplexer.png
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/new.png
--rw-r--r--   0        0        0    48254 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/openArrow.png
--rw-r--r--   0        0        0    49028 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/oscilloscope2.png
--rw-r--r--   0        0        0    48669 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/oscilloscope3.png
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/overlay.png
--rw-r--r--   0        0        0    24121 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pass2.png
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pass2_16.png
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pass_32.png
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pause.png
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/permute.png
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/phase.png
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/play.png
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/polar.png
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pole_zero.png
--rw-r--r--   0        0        0    47612 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/powerMeter.png
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/powerSwitch.png
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/powerSwitch_16.png
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/print2.png
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/print2_32.png
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/properties.png
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/r_icon.png
--rw-r--r--   0        0        0    47081 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/radiocontrolbutton.png
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/read2.png
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/red_light.png
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/remove.png
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/reset.png
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/rgb_icon.png
--rw-r--r--   0        0        0    49951 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/robot.png
--rw-r--r--   0        0        0    47140 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/rotation2.png
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/run2.png
--rw-r--r--   0        0        0     7132 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/run_all.png
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/saturation.png
--rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/save_ROI.png
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/scale_horizontally.png
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/scale_vertically.png
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/search2.png
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/select2.png
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/select_all.png
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/select_all2.png
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/select_none.png
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/sequence.png
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/sequence2.png
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/snap.png
--rw-r--r--   0        0        0    47434 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/spectrumAnalyzer.png
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/start.png
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/status_cancelled.png
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/stop.png
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/stop2.png
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/stop3.png
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/stop_all.png
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/sum.png
--rw-r--r--   0        0        0    50597 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/surfacePlot.png
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/tree.png
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/utility2.png
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/utility_small.png
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/vector.png
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/verify.png
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/video.png
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/wait.png
--rw-r--r--   0        0        0    50127 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/waterfallPlot.png
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/watershed.png
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/yellow_light.png
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/zip_file.png
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/zoomAuto.png
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/zoomReset.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/__init__.py
--rw-r--r--   0        0        0    10415 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/array_manipulation.py
--rw-r--r--   0        0        0     8921 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/calibration_camera.py
--rw-r--r--   0        0        0     7244 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/chrono_timer.py
--rw-r--r--   0        0        0    15404 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/config.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/conftests.py
--rw-r--r--   0        0        0    26941 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/daq_utils.py
--rw-r--r--   0        0        0    69686 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/data.py
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/enums.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/exceptions.py
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/factory.py
--rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/logger.py
--rw-r--r--   0        0        0    17513 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/math_utils.py
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/messenger.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/qvariant.py
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/slicing.py
--rw-r--r--   0        0        0    39074 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/tcp_server_client.py
--rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/units.py
--rw-r--r--   0        0        0   418388 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/Tuto innosetup/Tuto innosetup.odt
--rw-r--r--   0        0        0   361273 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/Tuto innosetup/Tuto innosetup.pdf
--rw-r--r--   0        0        0    12343 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/Tuto innosetup/script_full_setup.iss
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/abstract/__init__.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/abstract/logger.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/db/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/db/db_logger/__init__.py
--rw-r--r--   0        0        0    12413 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/db/db_logger/db_logger.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/db/db_logger/db_logger_models.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/gui_utils/__init__.py
--rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/gui_utils/custom_app.py
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/gui_utils/dock.py
--rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/gui_utils/file_io.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/gui_utils/layout.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/gui_utils/list_picker.py
--rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/gui_utils/utils.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/gui_utils/widgets/__init__.py
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/gui_utils/widgets/label.py
--rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/gui_utils/widgets/lcd.py
--rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/gui_utils/widgets/push.py
--rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/gui_utils/widgets/qled.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/gui_utils/widgets/spinbox.py
--rw-r--r--   0        0        0     8614 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/gui_utils/widgets/table.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/h5modules/__init__.py
--rw-r--r--   0        0        0    32012 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/h5modules/backends.py
--rw-r--r--   0        0        0    22457 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/h5modules/browsing.py
--rw-r--r--   0        0        0    31654 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/h5modules/data_saving.py
--rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/h5modules/exporter.py
--rw-r--r--   0        0        0     5490 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/h5modules/h5logging.py
--rw-r--r--   0        0        0    13166 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/h5modules/module_saving.py
--rw-r--r--   0        0        0    36657 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/h5modules/saving.py
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/h5modules/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/h5modules/exporters/__init__.py
--rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/h5modules/exporters/base.py
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/h5modules/exporters/flimj.py
--rw-r--r--   0        0        0     6517 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/h5modules/exporters/hyperspy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/managers/__init__.py
--rw-r--r--   0        0        0    16788 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/managers/action_manager.py
--rw-r--r--   0        0        0    13905 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/managers/batchscan_manager.py
--rw-r--r--   0        0        0    20283 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/managers/modules_manager.py
--rw-r--r--   0        0        0     7158 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/managers/overshoot_manager.py
--rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/managers/parameter_manager.py
--rw-r--r--   0        0        0     8205 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/managers/preset_manager.py
--rw-r--r--   0        0        0     8172 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/managers/preset_manager_utils.py
--rw-r--r--   0        0        0    22216 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/managers/remote_manager.py
--rw-r--r--   0        0        0    28454 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/managers/roi_manager.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/parameter/__init__.py
--rw-r--r--   0        0        0    16536 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/parameter/ioxml.py
--rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/parameter/utils.py
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/__init__.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/bool.py
--rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/date.py
--rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/filedir.py
--rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/itemselect.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/led.py
--rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/list.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/numeric.py
--rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/pixmap.py
--rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/slide.py
--rw-r--r--   0        0        0     4819 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/table.py
--rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/tableview.py
--rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/text.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/__init__.py
--rw-r--r--   0        0        0     4097 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/gant_chart.py
--rw-r--r--   0        0        0     3450 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/image_viewer.py
--rw-r--r--   0        0        0    13882 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/navigator.py
--rw-r--r--   0        0        0    16602 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/scan_selector.py
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/widgets.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/data_viewers/__init__.py
--rw-r--r--   0        0        0    12480 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/data_viewers/viewer.py
--rw-r--r--   0        0        0     9028 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/data_viewers/viewer0D.py
--rw-r--r--   0        0        0    19969 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/data_viewers/viewer1D.py
--rw-r--r--   0        0        0     7407 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/data_viewers/viewer1Dbasic.py
--rw-r--r--   0        0        0    41922 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/data_viewers/viewer2D.py
--rw-r--r--   0        0        0     5567 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/data_viewers/viewer2D_basic.py
--rw-r--r--   0        0        0    34930 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/data_viewers/viewerND.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/items/__init__.py
--rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/items/axis_scaled.py
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/items/crosshair.py
--rw-r--r--   0        0        0    14600 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/items/image.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/utils/__init__.py
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/utils/axes_viewer.py
--rw-r--r--   0        0        0    21044 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/utils/filter.py
--rw-r--r--   0        0        0     7945 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/utils/lineout.py
--rw-r--r--   0        0        0    17131 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/utils/plot_utils.py
--rw-r--r--   0        0        0    44892 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/plotting/utils/signalND.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/scanner/__init__.py
--rw-r--r--   0        0        0     7019 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/scanner/scan_factory.py
--rw-r--r--   0        0        0     9905 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/scanner/scanner.py
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/scanner/utils.py
--rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/scanner/scanners/_1d_scanners.py
--rw-r--r--   0        0        0    12852 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/scanner/scanners/_2d_scanners.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/scanner/scanners/__init__.py
--rw-r--r--   0        0        0     7646 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/scanner/scanners/sequential.py
--rw-r--r--   0        0        0    12514 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/scanner/scanners/tabular.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/svg/__init__.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/svg/svg_renderer.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/svg/svg_view.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/svg/svg_viewer2D.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/tree_layout/__init__.py
--rw-r--r--   0        0        0     6625 2020-02-02 00:00:00.000000 pymodaq-4.0.2/src/pymodaq/utils/tree_layout/tree_layout_main.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 pymodaq-4.0.2/.gitignore
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 pymodaq-4.0.2/LICENSE
--rw-r--r--   0        0        0     4567 2020-02-02 00:00:00.000000 pymodaq-4.0.2/README.rst
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 pymodaq-4.0.2/pyproject.toml
--rw-r--r--   0        0        0     7603 2020-02-02 00:00:00.000000 pymodaq-4.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/__init__.py
+-rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/__init__.py
+-rw-r--r--   0        0        0     8738 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/daq_utils.py
+-rw-r--r--   0        0        0    61748 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/dashboard.py
+-rw-r--r--   0        0        0    74359 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/icon.ico
+-rw-r--r--   0        0        0    53114 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/splash.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/control_modules/__init__.py
+-rw-r--r--   0        0        0    35899 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/control_modules/daq_move.py
+-rw-r--r--   0        0        0    13301 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/control_modules/daq_move_ui.py
+-rw-r--r--   0        0        0    56573 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/control_modules/daq_viewer.py
+-rw-r--r--   0        0        0    15462 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/control_modules/daq_viewer_ui.py
+-rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/control_modules/mocks.py
+-rw-r--r--   0        0        0    30998 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/control_modules/move_utility_classes.py
+-rw-r--r--   0        0        0    13073 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/control_modules/utils.py
+-rw-r--r--   0        0        0    26816 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/control_modules/viewer_utility_classes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/examples/__init__.py
+-rw-r--r--   0        0        0    11127 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/examples/custom_app.py
+-rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/examples/custom_viewer.py
+-rw-r--r--   0        0        0     6104 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/examples/function_plotter.py
+-rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/examples/nonlinearscanner.py
+-rw-r--r--   0        0        0     7187 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/examples/parameter_ex.py
+-rw-r--r--   0        0        0    15774 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/examples/preset_MockCamera.xml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Client.aliases
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Client.lvlps
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Client.lvproj
+-rw-r--r--   0        0        0    69358 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Client.vi
+-rw-r--r--   0        0        0    21969 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Server_1Dgaussian.vi
+-rw-r--r--   0        0        0    29785 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Server_2Dgaussian.vi
+-rw-r--r--   0        0        0    18148 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_read_cmd.vi
+-rw-r--r--   0        0        0    20622 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_read_float.vi
+-rw-r--r--   0        0        0    11828 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_read_int.vi
+-rw-r--r--   0        0        0    23025 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_data.vi
+-rw-r--r--   0        0        0     9072 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_int.vi
+-rw-r--r--   0        0        0    19039 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_scalar.vi
+-rw-r--r--   0        0        0    19791 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_string.vi
+-rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/examples/Labview_TCP_Client/client_state.ctl
+-rw-r--r--   0        0        0     4618 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/examples/Labview_TCP_Client/cmd_types.ctl
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/extensions/__init__.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/extensions/console.py
+-rw-r--r--   0        0        0    19346 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/extensions/daq_logger.py
+-rw-r--r--   0        0        0    56505 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/extensions/daq_scan.py
+-rw-r--r--   0        0        0    10134 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/extensions/daq_scan_ui.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/extensions/h5browser.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/extensions/utils.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/extensions/pid/__init__.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/extensions/pid/daq_move_PID.py
+-rw-r--r--   0        0        0    29797 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/extensions/pid/pid_controller.py
+-rw-r--r--   0        0        0     8074 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/extensions/pid/utils.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/post_treatment/__init__.py
+-rw-r--r--   0        0        0    10077 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/post_treatment/load_and_plot.py
+-rw-r--r--   0        0        0    11562 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/post_treatment/process_to_scalar.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/post_treatment/daq_analysis/__init__.py
+-rw-r--r--   0        0        0    24346 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/post_treatment/daq_analysis/daq_analysis_main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/post_treatment/daq_measurement/__init__.py
+-rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/post_treatment/daq_measurement/daq_measurement_GUI.py
+-rw-r--r--   0        0        0     7037 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/post_treatment/daq_measurement/daq_measurement_GUI.ui
+-rw-r--r--   0        0        0    17093 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/post_treatment/daq_measurement/daq_measurement_main.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/post_treatment/daq_measurement/process_from_QtDesigner_DAQ_Measurement_GUI.bat
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/VERSION
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/__init__.py
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/config_template.toml
+-rw-r--r--   0        0        0    31882 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/preset_default.xml
+-rw-r--r--   0        0        0     9320 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/triangulation_data.npy
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/QtDesigner_ressources.bat
+-rw-r--r--   0        0        0     9800 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/QtDesigner_ressources.qrc
+-rw-r--r--   0        0        0  8225442 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/QtDesigner_ressources_rc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/__init__.py
+-rw-r--r--   0        0        0     5703 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/icons.svg
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/1d.png
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/2d.png
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/3d.png
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Add2.png
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Add_Step.png
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Approve.png
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Approve_All.png
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Browse_Dir_Path.png
+-rw-r--r--   0        0        0    47401 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Calculator.png
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ChnGroup.png
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ChnNum.png
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ChnText.png
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ChnTime.png
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ChnWave.png
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Close3.png
+-rw-r--r--   0        0        0    47830 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/CollapseAll.png
+-rw-r--r--   0        0        0    48054 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/CollapseAll_32.png
+-rw-r--r--   0        0        0    48959 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ColorPicker.png
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Contract.png
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Create.png
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/DeleteLayer.png
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EditOpen.png
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EditRedo.png
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EditUndo.png
+-rw-r--r--   0        0        0    49034 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Ellipse.png
+-rw-r--r--   0        0        0    48413 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EllipseFilled.png
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Error.png
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ErrorMessage.png
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Error_16.png
+-rw-r--r--   0        0        0    48491 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Exit.png
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Expand.png
+-rw-r--r--   0        0        0    47692 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ExpandAll.png
+-rw-r--r--   0        0        0    48102 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ExpandAll_32.png
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/FFT.png
+-rw-r--r--   0        0        0    89487 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/HLM.ico
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Help.png
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Help_32.png
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Histogram.png
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/LUT_LookUpTable.png
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MagnifyingGlass.png
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MagnifyingGlass_24.png
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Marker.png
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Math.png
+-rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MeasurementStudio_32.png
+-rw-r--r--   0        0        0    48221 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Move.png
+-rw-r--r--   0        0        0    47229 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MoveDown.png
+-rw-r--r--   0        0        0    47258 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MoveUp.png
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Multiply.png
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/NewFile.png
+-rw-r--r--   0        0        0    48742 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/NewLayer.png
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/New_File.png
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/New_Folder.png
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open.png
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_1D.png
+-rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_2D.png
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_File.png
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_File_32.png
+-rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_sim.png
+-rw-r--r--   0        0        0    48140 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Options.png
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Oscilloscope.png
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Oscilloscope_16.png
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Pass.png
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/RGB.png
+-rw-r--r--   0        0        0    47228 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Rectangle.png
+-rw-r--r--   0        0        0    47093 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/RectangleFilled.png
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Redo.png
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Refresh.png
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Refresh2.png
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Refresh_32.png
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Region.png
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Rendezvous.png
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SELECT.png
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Save.png
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SaveAll.png
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SaveAll_32.png
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SaveAs.png
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SaveAs_32.png
+-rw-r--r--   0        0        0    49529 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Save_24.png
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Save_32.png
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Search.png
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SelectPolygon.png
+-rw-r--r--   0        0        0    47940 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Select_24.png
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Settings.png
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snap&Save.png
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot.png
+-rw-r--r--   0        0        0    49414 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot2.png
+-rw-r--r--   0        0        0    49581 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot2_16.png
+-rw-r--r--   0        0        0    52734 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot2_32.png
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Spreadsheet.png
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Statistics.png
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Statistics2.png
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Status.png
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Subtract.png
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Vision.png
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Volts.png
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Wait2.png
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Zoom_1_1.png
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Zoom_in.png
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Zoom_out.png
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Zoom_to_Selection.png
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/abort.png
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/advanced2.png
+-rw-r--r--   0        0        0    47292 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/autoscale.png
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/b_icon.png
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/back.png
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/bg_icon.png
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/camera.png
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/camera_snap.png
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/cartesian.png
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/clear2.png
+-rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/clear_ROI.png
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/close2.png
+-rw-r--r--   0        0        0    47742 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/cluster2.png
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/color.png
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/color2.png
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/continuous.png
+-rw-r--r--   0        0        0    47210 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/data.png
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/delay.png
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/download.png
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/download2.png
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/error2.png
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ethernet.png
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/exit2.png
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/fan.png
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/filter2.png
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/g_icon.png
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/gear2.png
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/go_to.png
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/go_to_1.png
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/go_to_2.png
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/grab.png
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/graph.png
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/greenLight2.png
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/greenLight2_32.png
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/green_light.png
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/grey_icon.png
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/greyscale.png
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/help1.png
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/help1_32.png
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/home2.png
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/information2.png
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ini.png
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/integrator.png
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/joystick.png
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_green.png
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_green_16.png
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_red.png
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_red_16.png
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_yellow.png
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_yellow_16.png
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/limiter.png
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/load_ROI.png
+-rw-r--r--   0        0        0    50113 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meshPlot.png
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meter.png
+-rw-r--r--   0        0        0    47361 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meter2.png
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meter_32.png
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/move_contour.png
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/move_straight_line.png
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/movie.png
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/multi_point.png
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/multiplexer.png
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/new.png
+-rw-r--r--   0        0        0    48254 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/openArrow.png
+-rw-r--r--   0        0        0    49028 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/oscilloscope2.png
+-rw-r--r--   0        0        0    48669 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/oscilloscope3.png
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/overlay.png
+-rw-r--r--   0        0        0    24121 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pass2.png
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pass2_16.png
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pass_32.png
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pause.png
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/permute.png
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/phase.png
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/play.png
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/polar.png
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pole_zero.png
+-rw-r--r--   0        0        0    47612 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/powerMeter.png
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/powerSwitch.png
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/powerSwitch_16.png
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/print2.png
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/print2_32.png
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/properties.png
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/r_icon.png
+-rw-r--r--   0        0        0    47081 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/radiocontrolbutton.png
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/read2.png
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/red_light.png
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/remove.png
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/reset.png
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/rgb_icon.png
+-rw-r--r--   0        0        0    49951 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/robot.png
+-rw-r--r--   0        0        0    47140 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/rotation2.png
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/run2.png
+-rw-r--r--   0        0        0     7132 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/run_all.png
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/saturation.png
+-rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/save_ROI.png
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/scale_horizontally.png
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/scale_vertically.png
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/search2.png
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/select2.png
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/select_all.png
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/select_all2.png
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/select_none.png
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/sequence.png
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/sequence2.png
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/snap.png
+-rw-r--r--   0        0        0    47434 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/spectrumAnalyzer.png
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/start.png
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/status_cancelled.png
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/stop.png
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/stop2.png
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/stop3.png
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/stop_all.png
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/sum.png
+-rw-r--r--   0        0        0    50597 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/surfacePlot.png
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/tree.png
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/utility2.png
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/utility_small.png
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/vector.png
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/verify.png
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/video.png
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/wait.png
+-rw-r--r--   0        0        0    50127 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/waterfallPlot.png
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/watershed.png
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/yellow_light.png
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/zip_file.png
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/zoomAuto.png
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/zoomReset.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/__init__.py
+-rw-r--r--   0        0        0    10415 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/array_manipulation.py
+-rw-r--r--   0        0        0     8921 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/calibration_camera.py
+-rw-r--r--   0        0        0     7244 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/chrono_timer.py
+-rw-r--r--   0        0        0    15404 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/config.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/conftests.py
+-rw-r--r--   0        0        0    26941 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/daq_utils.py
+-rw-r--r--   0        0        0    71226 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/data.py
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/enums.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/exceptions.py
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/factory.py
+-rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/logger.py
+-rw-r--r--   0        0        0    17513 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/math_utils.py
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/messenger.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/qvariant.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/slicing.py
+-rw-r--r--   0        0        0    39074 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/tcp_server_client.py
+-rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/units.py
+-rw-r--r--   0        0        0   418388 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/Tuto innosetup/Tuto innosetup.odt
+-rw-r--r--   0        0        0   361273 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/Tuto innosetup/Tuto innosetup.pdf
+-rw-r--r--   0        0        0    12343 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/Tuto innosetup/script_full_setup.iss
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/abstract/__init__.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/abstract/logger.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/db/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/db/db_logger/__init__.py
+-rw-r--r--   0        0        0    12413 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/db/db_logger/db_logger.py
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/db/db_logger/db_logger_models.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/gui_utils/__init__.py
+-rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/gui_utils/custom_app.py
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/gui_utils/dock.py
+-rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/gui_utils/file_io.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/gui_utils/layout.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/gui_utils/list_picker.py
+-rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/gui_utils/utils.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/gui_utils/widgets/__init__.py
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/gui_utils/widgets/label.py
+-rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/gui_utils/widgets/lcd.py
+-rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/gui_utils/widgets/push.py
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/gui_utils/widgets/qled.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/gui_utils/widgets/spinbox.py
+-rw-r--r--   0        0        0     8614 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/gui_utils/widgets/table.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/h5modules/__init__.py
+-rw-r--r--   0        0        0    32012 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/h5modules/backends.py
+-rw-r--r--   0        0        0    23145 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/h5modules/browsing.py
+-rw-r--r--   0        0        0    31654 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/h5modules/data_saving.py
+-rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/h5modules/exporter.py
+-rw-r--r--   0        0        0     5490 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/h5modules/h5logging.py
+-rw-r--r--   0        0        0    13494 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/h5modules/module_saving.py
+-rw-r--r--   0        0        0    34592 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/h5modules/saving.py
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/h5modules/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/h5modules/exporters/__init__.py
+-rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/h5modules/exporters/base.py
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/h5modules/exporters/flimj.py
+-rw-r--r--   0        0        0     6517 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/h5modules/exporters/hyperspy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/managers/__init__.py
+-rw-r--r--   0        0        0    16788 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/managers/action_manager.py
+-rw-r--r--   0        0        0    13905 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/managers/batchscan_manager.py
+-rw-r--r--   0        0        0    20283 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/managers/modules_manager.py
+-rw-r--r--   0        0        0     7158 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/managers/overshoot_manager.py
+-rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/managers/parameter_manager.py
+-rw-r--r--   0        0        0     8205 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/managers/preset_manager.py
+-rw-r--r--   0        0        0     8172 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/managers/preset_manager_utils.py
+-rw-r--r--   0        0        0    22216 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/managers/remote_manager.py
+-rw-r--r--   0        0        0    28454 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/managers/roi_manager.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/parameter/__init__.py
+-rw-r--r--   0        0        0    16536 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/parameter/ioxml.py
+-rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/parameter/utils.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/parameter/pymodaq_ptypes/__init__.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/parameter/pymodaq_ptypes/bool.py
+-rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/parameter/pymodaq_ptypes/date.py
+-rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/parameter/pymodaq_ptypes/filedir.py
+-rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/parameter/pymodaq_ptypes/itemselect.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/parameter/pymodaq_ptypes/led.py
+-rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/parameter/pymodaq_ptypes/list.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/parameter/pymodaq_ptypes/numeric.py
+-rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/parameter/pymodaq_ptypes/pixmap.py
+-rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/parameter/pymodaq_ptypes/slide.py
+-rw-r--r--   0        0        0     4819 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/parameter/pymodaq_ptypes/table.py
+-rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/parameter/pymodaq_ptypes/tableview.py
+-rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/parameter/pymodaq_ptypes/text.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/plotting/__init__.py
+-rw-r--r--   0        0        0     4097 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/plotting/gant_chart.py
+-rw-r--r--   0        0        0     3450 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/plotting/image_viewer.py
+-rw-r--r--   0        0        0    13882 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/plotting/navigator.py
+-rw-r--r--   0        0        0    16602 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/plotting/scan_selector.py
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/plotting/widgets.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/plotting/data_viewers/__init__.py
+-rw-r--r--   0        0        0    12480 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/plotting/data_viewers/viewer.py
+-rw-r--r--   0        0        0     9028 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/plotting/data_viewers/viewer0D.py
+-rw-r--r--   0        0        0    19969 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/plotting/data_viewers/viewer1D.py
+-rw-r--r--   0        0        0     7407 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/plotting/data_viewers/viewer1Dbasic.py
+-rw-r--r--   0        0        0    41922 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/plotting/data_viewers/viewer2D.py
+-rw-r--r--   0        0        0     5567 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/plotting/data_viewers/viewer2D_basic.py
+-rw-r--r--   0        0        0    34930 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/plotting/data_viewers/viewerND.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/plotting/items/__init__.py
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/plotting/items/axis_scaled.py
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/plotting/items/crosshair.py
+-rw-r--r--   0        0        0    14600 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/plotting/items/image.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/plotting/utils/__init__.py
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/plotting/utils/axes_viewer.py
+-rw-r--r--   0        0        0    21044 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/plotting/utils/filter.py
+-rw-r--r--   0        0        0     7945 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/plotting/utils/lineout.py
+-rw-r--r--   0        0        0    17131 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/plotting/utils/plot_utils.py
+-rw-r--r--   0        0        0    44892 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/plotting/utils/signalND.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/scanner/__init__.py
+-rw-r--r--   0        0        0     7019 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/scanner/scan_factory.py
+-rw-r--r--   0        0        0     9905 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/scanner/scanner.py
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/scanner/utils.py
+-rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/scanner/scanners/_1d_scanners.py
+-rw-r--r--   0        0        0    12882 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/scanner/scanners/_2d_scanners.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/scanner/scanners/__init__.py
+-rw-r--r--   0        0        0     7646 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/scanner/scanners/sequential.py
+-rw-r--r--   0        0        0    12514 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/scanner/scanners/tabular.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/svg/__init__.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/svg/svg_renderer.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/svg/svg_view.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/svg/svg_viewer2D.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/tree_layout/__init__.py
+-rw-r--r--   0        0        0     6625 2020-02-02 00:00:00.000000 pymodaq-4.0.3/src/pymodaq/utils/tree_layout/tree_layout_main.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 pymodaq-4.0.3/.gitignore
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 pymodaq-4.0.3/LICENSE
+-rw-r--r--   0        0        0     4567 2020-02-02 00:00:00.000000 pymodaq-4.0.3/README.rst
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 pymodaq-4.0.3/pyproject.toml
+-rw-r--r--   0        0        0     7571 2020-02-02 00:00:00.000000 pymodaq-4.0.3/PKG-INFO
```

### Comparing `pymodaq-4.0.2/src/pymodaq/__init__.py` & `pymodaq-4.0.3/src/pymodaq/__init__.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/daq_utils.py` & `pymodaq-4.0.3/src/pymodaq/daq_utils.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/dashboard.py` & `pymodaq-4.0.3/src/pymodaq/dashboard.py`

 * *Files 0% similar despite different names*

```diff
@@ -1155,22 +1155,22 @@
     Slot(bool)
     def stop_moves(self, overshoot):
         """
             Foreach module of the move module object list, stop motion.
 
             See Also
             --------
-            stop_scan,  DAQ_Move_main.daq_move.stop_Motion
+            stop_scan,  DAQ_Move_main.daq_move.stop_motion
         """
         self.overshoot = overshoot
         if self.scan_module is not None:
             self.scan_module.stop_scan()
 
         for mod in self.actuators_modules:
-            mod.stop_Motion()
+            mod.stop_motion()
 
     def show_log(self):
         import webbrowser
         webbrowser.open(logging.getLogger('pymodaq').handlers[0].baseFilename)
 
     def show_config(self):
         config_tree = configmod.TreeFromToml()
```

### Comparing `pymodaq-4.0.2/src/pymodaq/icon.ico` & `pymodaq-4.0.3/src/pymodaq/icon.ico`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/splash.png` & `pymodaq-4.0.3/src/pymodaq/splash.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/control_modules/daq_move.py` & `pymodaq-4.0.3/src/pymodaq/control_modules/daq_move.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,36 +12,38 @@
 import numpy as np
 
 from qtpy.QtCore import QObject, Signal, QThread, Slot, Qt, QTimer
 from qtpy import QtWidgets
 
 from easydict import EasyDict as edict
 
-from pymodaq.utils.logger import set_logger, get_module_name, get_module_name
+from pymodaq.utils.logger import set_logger, get_module_name
 from pymodaq.control_modules.utils import ControlModule
 from pymodaq.utils.parameter import ioxml
 from pymodaq.control_modules.daq_move_ui import DAQ_Move_UI, ThreadCommand
 from pymodaq.utils.managers.parameter_manager import ParameterManager, Parameter
 from pymodaq.control_modules.move_utility_classes import MoveCommand
 from pymodaq.utils.tcp_server_client import TCPClient
 from pymodaq.control_modules.move_utility_classes import params as daq_move_params
 from pymodaq.utils import daq_utils as utils
 from pymodaq.utils.parameter import utils as putils
 from pymodaq.utils.gui_utils import get_splash_sc
-from pymodaq.utils import config
+from pymodaq.utils import config as config_mod
 from pymodaq.utils.exceptions import ActuatorError
 from pymodaq.utils.messenger import deprecation_msg
 from pymodaq.utils.h5modules import module_saving
-from pymodaq.utils.data import DataRaw, DataFromPlugins, DataToExport, Axis, DataDistribution
+from pymodaq.utils.data import DataRaw, DataToExport
 from pymodaq.utils.h5modules.backends import Node
 
 
-local_path = config.get_set_local_dir()
+local_path = config_mod.get_set_local_dir()
 sys.path.append(local_path)
 logger = set_logger(get_module_name(__file__))
+config = config_mod.Config()
+
 DAQ_Move_Actuators = utils.get_plugins('daq_move')
 ACTUATOR_TYPES = [mov['name'] for mov in DAQ_Move_Actuators]
 
 STATUS_WAIT_TIME = 1000
 
 
 class DAQ_Move(ParameterManager, ControlModule):
@@ -68,15 +70,14 @@
     move_done_signal = Signal(str, float)
     current_value_signal = Signal(str, float)
     # to be used in external program to make sure the move has been done,
     # export the current position. str refer to the unique title given to the module
     _update_settings_signal = Signal(edict)
     bounds_signal = Signal(bool)
 
-    
     params = daq_move_params
 
     def __init__(self, parent=None, title="DAQ Move"):
         """
 
         Parameters
         ----------
@@ -94,15 +95,15 @@
         ParameterManager.__init__(self)
         ControlModule.__init__(self)
 
         self.parent = parent
         if parent is not None:
             self.ui = DAQ_Move_UI(parent, title)
         else:
-            self.ui = None
+            self.ui: DAQ_Move_UI = None
 
         if self.ui is not None:
             self.ui.actuators = ACTUATOR_TYPES
             self.ui.set_settings_tree(self.settings_tree)
             self.ui.command_sig.connect(self.process_ui_cmds)
 
         self.splash_sc = get_splash_sc()
@@ -229,18 +230,14 @@
         if move_command.move_type == 'abs':
             self.move_abs(move_command.value)
         elif move_command.move_type == 'rel':
             self.move_rel(move_command.value)
         elif move_command.move_type == 'home':
             self.move_home(move_command.value)
 
-    def move_Abs(self, value, send_to_tcpip=False):
-        deprecation_msg(f'The method *move_Abs* should not be used anymore, use *move_abs*')
-        self.move_abs(value, send_to_tcpip=send_to_tcpip)
-
     def move_abs(self, value, send_to_tcpip=False):
         """Move the connected hardware to the absolute value
 
         Returns nothing but the move_done_signal will be send once the action is done
 
         Parameters
         ----------
@@ -259,18 +256,14 @@
                 self.update_status("Moving")
                 self.command_hardware.emit(ThreadCommand(command="reset_stop_motion"))
                 self.command_hardware.emit(ThreadCommand(command="move_abs", attribute=[value]))
 
         except Exception as e:
             self.logger.exception(str(e))
 
-    def move_Home(self, send_to_tcpip=False):
-        self.move_home(send_to_tcpip)
-        deprecation_msg(f'The method *move_Home* is deprecated, use *move_home*')
-
     def move_home(self, send_to_tcpip=False):
         """Move the connected actuator to its home value (if any)
 
         Parameters
         ----------
         send_to_tcpip: bool
             if True, this position is send through the TCP/IP communication canal
@@ -278,23 +271,19 @@
         self._send_to_tcpip = send_to_tcpip
         try:
             if self.ui is not None:
                 self.ui.move_done = False
             self._move_done_bool = False
             self.update_status("Moving")
             self.command_hardware.emit(ThreadCommand(command="reset_stop_motion"))
-            self.command_hardware.emit(ThreadCommand(command="move_Home"))
+            self.command_hardware.emit(ThreadCommand(command="move_home"))
 
         except Exception as e:
             self.logger.exception(str(e))
 
-    def move_Rel(self, rel_value, send_to_tcpip=False):
-        deprecation_msg(f'The method *move_Rel* should not be used anymore, use *move_rel*')
-        self.move_rel(rel_value, send_to_tcpip=send_to_tcpip)
-
     def move_rel(self, rel_value, send_to_tcpip=False):
         """Move the connected hardware to the relative value
 
         Returns nothing but the move_done_signal will be send once the action is done
 
         Parameters
         ----------
@@ -313,22 +302,14 @@
             self.update_status("Moving")
             self.command_hardware.emit(ThreadCommand(command="reset_stop_motion"))
             self.command_hardware.emit(ThreadCommand(command="move_rel", attribute=[rel_value]))
 
         except Exception as e:
             self.logger.exception(str(e))
 
-    def move_Rel_p(self):
-        deprecation_msg(f'The method *move_Rel_p* should not be used anymore, use *move_rel_p*')
-        self.move_rel_p()
-
-    def move_Rel_m(self):
-        deprecation_msg(f'The method *move_Rel_m* should not be used anymore, use *move_rel_m*')
-        self.move_rel_m()
-
     def move_rel_p(self):
         self.move_rel(self._relative_value)
 
     def move_rel_m(self):
         self.move_rel(-self._relative_value)
 
     def quit_fun(self):
@@ -340,33 +321,29 @@
 
         if self._initialized_state:
             self.init_hardware(False)
         if self.ui is not None:
             self.ui.get_action('quit').trigger()
         self.quit_signal.emit()
 
-    def ini_stage_fun(self):
-        deprecation_msg(f'The function *ini_stage_fun* is deprecated, use init_hardware')
-        self.init_hardware(True)
-
     def init_hardware_ui(self, do_init=True):
         """Programmatic actuator's Initialization
 
         Programmatic way to simulate a click on the init button of the UI to initialize the communication with the
         hardware
 
         Parameters
         ----------
         do_init: bool
             if the init or des-init should be performed
         """
         self.ui.do_init(do_init)
 
     def init_hardware(self, do_init=True):
-
+        """ Init or desinit the selected instrument plugin class """
         if not do_init:
             try:
                 self.command_hardware.emit(ThreadCommand(command="close"))
                 if self.ui is not None:
                     self.ui.actuator_init = False
             except Exception as e:
                 self.logger.exception(str(e))
@@ -391,18 +368,19 @@
     @property
     def initialized_state(self):
         """bool: status of the actuator's initialization (init or not)"""
         return self._initialized_state
 
     @property
     def move_done_bool(self):
-        """bool: status of the actuator's action (done or not)"""
+        """bool: status of the actuator's status (done or not)"""
         return self._move_done_bool
 
     def value_changed(self, param):
+        """ Apply changes of value in the settings"""
         if param.name() == 'connect_server':
             if param.value():
                 self.connect_tcp_ip()
             else:
                 self._command_tcpip.emit(ThreadCommand('quit', ))
 
         elif param.name() == 'ip_address' or param.name == 'port':
@@ -418,96 +396,70 @@
         if path is not None:
             if 'main_settings' not in path:
                 self._update_settings_signal.emit(edict(path=path, param=param, change='value'))
                 if self.settings.child('main_settings', 'tcpip', 'tcp_connected').value():
                     self._command_tcpip.emit(ThreadCommand('send_info', dict(path=path, param=param)))
 
     def param_deleted(self, param):
+        """ Apply deletion of settings """
         if param.name() not in putils.iter_children(self.settings.child('main_settings'), []):
             self._update_settings_signal.emit(edict(path=['move_settings'], param=param, change='parent'))
 
     def child_added(self, param, data):
+        """ Apply addition of settings """
         path = self.settings.childPath(param)
         if 'main_settings' not in path:
             self._update_settings_signal.emit(edict(path=path, param=data[0].saveState(), change='childAdded'))
 
-    @Slot()
     def raise_timeout(self):
-        """Update status with "Timeout occurred" statement and change the timeout flag.
+        """ Update status with "Timeout occurred" statement and change the timeout flag.
         """
         self.update_status("Timeout occurred")
         self.wait_position_flag = False
 
     @Slot(ThreadCommand)
-    def thread_status(self, status):  # general function to get datas/infos from all threads back to the main
-        """
-            | General function to get datas/infos from all threads back to the main0
-            |
-
-            Interpret a command from the command given by the ThreadCommand status :
-                * In case of **'Update_status'** command, call the update_status method with status attribute as parameters
-                * In case of **'ini_stage'** command, initialise a Stage from status attribute
-                * In case of **'close'** command, close the launched stage thread
-                * In case of **'check_position'** command, set the current_value value from status attribute
-                * In case of **'move_done'** command, set the current_value value, make profile of move_done and send the move done signal with status attribute
-                * In case of **'Move_Not_Done'** command, set the current position value from the status attribute, make profile of Not_move_done and send the Thread Command "move_abs"
-                * In case of **'update_settings'** command, create child "Move Settings" from  status attribute (if possible)
-
-            ================ ================= ======================================================
-            **Parameters**     **Type**         **Description**
+    def thread_status(self, status: ThreadCommand):  # general function to get datas/infos from all threads back to the main
+        """Get back info (using the ThreadCommand object) from the hardware
 
-            *status*          ThreadCommand()   instance of ThreadCommand containing two attribute :
+        And re-emit this ThreadCommand using the custom_sig signal if it should be used in a higher level module
 
-                                                 * *command*    str
-                                                 * *attribute* list
+        Commands valid for all control modules are defined in the parent class, here are described only the specific
+        ones
 
-            ================ ================= ======================================================
+        Parameters
+        ----------
+        status: ThreadCommand
+            Possible values are:
 
-            See Also
-            --------
-            update_status, set_enabled_move_buttons, get_actuator_value, DAQ_utils.ThreadCommand, parameter_tree_changed, raise_timeout
+            * **ini_stage**: obtains info from the initialization
+            * **get_actuator_value**: update the UI current value
+            * **move_done**: update the UI current value and emits the move_done signal
+            * **outofbounds**: emits the bounds_signal signal with a True argument
+            * **set_allowed_values**: used to change the behaviour of the spinbox controlling absolute values (see
+              :meth:`daq_move_ui.set_abs_spinbox_properties`
+            * stop: stop the motion
         """
 
-        if status.command == "Update_Status":
-            if len(status.attribute) > 2:
-                self.update_status(status.attribute[0], log=status.attribute[1])
-            else:
-                self.update_status(status.attribute[0])
+        super().thread_status(status, 'move')
 
-        elif status.command == "ini_stage":
+        if status.command == "ini_stage":
             # status.attribute[0]=edict(initialized=bool,info="", controller=)
             self.update_status("Stage initialized: {:} info: {:}".format(status.attribute[0]['initialized'],
                                                                          status.attribute[0]['info']))
             if status.attribute[0]['initialized']:
                 self.controller = status.attribute[0]['controller']
                 if self.ui is not None:
                     self.ui.actuator_init = True
                 self._initialized_state = True
             else:
                 self._initialized_state = False
             if self._initialized_state:
                 self.get_actuator_value()
             self.init_signal.emit(self._initialized_state)
 
-        elif status.command == "close":
-            try:
-                self.update_status(status.attribute[0])
-                self._hardware_thread.exit()
-                self._hardware_thread.wait()
-                finished = self._hardware_thread.isFinished()
-                if finished:
-                    pass
-                    delattr(self, 'hardware_thread')
-                else:
-                    self.update_status('thread is locked?!', STATUS_WAIT_TIME, 'log')
-            except Exception as e:
-                self.logger.exception(str(e))
-            self._initialized_state = False
-            self.init_signal.emit(self._initialized_state)
-
         elif status.command == "get_actuator_value" or status.command == 'check_position':
             if self.ui is not None:
                 self.ui.display_value(status.attribute[0])
             self._current_value = status.attribute[0]
             self.current_value_signal.emit(self.title, self._current_value)
             if self.settings.child('main_settings', 'tcpip', 'tcp_connected').value() and self._send_to_tcpip:
                 self._command_tcpip.emit(ThreadCommand('position_is', status.attribute))
@@ -518,82 +470,23 @@
                 self.ui.move_done = True
             self._current_value = status.attribute[0]
             self._move_done_bool = True
             self.move_done_signal.emit(self._title, status.attribute[0])
             if self.settings.child('main_settings', 'tcpip', 'tcp_connected').value() and self._send_to_tcpip:
                 self._command_tcpip.emit(ThreadCommand('move_done', status.attribute))
 
-        elif status.command == "Move_Not_Done":
-            if self.ui is not None:
-                self.ui.display_value(status.attribute[0])
-                self.ui.move_done = False
-
-            self._current_value = status.attribute[0]
-            self._move_done_bool = False
-            self.command_hardware.emit(ThreadCommand(command="move_abs", attribute=[self._target_value]))
-
-        elif status.command == 'update_main_settings':
-            # this is a way for the plugins to update main settings of the ui (solely values, limits and options)
-            try:
-                if status.attribute[2] == 'value':
-                    self.settings.child('main_settings', *status.attribute[0]).setValue(status.attribute[1])
-                elif status.attribute[2] == 'limits':
-                    self.settings.child('main_settings', *status.attribute[0]).setLimits(status.attribute[1])
-                elif status.attribute[2] == 'options':
-                    self.settings.child('main_settings', *status.attribute[0]).setOpts(**status.attribute[1])
-            except Exception as e:
-                self.logger.exception(str(e))
-
-        elif status.command == 'update_settings':
-            # ThreadCommand(command='update_settings',attribute=[path,data,change]))
-            try:
-                self.settings.sigTreeStateChanged.disconnect(
-                    self.parameter_tree_changed)  # any changes on the settings will update accordingly the detector
-            except Exception:
-                pass
-            try:
-                if status.attribute[2] == 'value':
-                    self.settings.child('move_settings', *status.attribute[0]).setValue(status.attribute[1])
-                elif status.attribute[2] == 'limits':
-                    self.settings.child('move_settings', *status.attribute[0]).setLimits(status.attribute[1])
-                elif status.attribute[2] == 'options':
-                    self.settings.child('move_settings', *status.attribute[0]).setOpts(**status.attribute[1])
-                elif status.attribute[2] == 'childAdded':
-                    child = Parameter.create(name='tmp')
-                    child.restoreState(status.attribute[1][0])
-                    self.settings.child('move_settings', *status.attribute[0]).addChild(status.attribute[1][0])
-
-            except Exception as e:
-                self.logger.exception(str(e))
-            self.settings.sigTreeStateChanged.connect(
-                self.parameter_tree_changed)  # any changes on the settings will update accordingly the detector
-
-        elif status.command == 'raise_timeout':
-            self.raise_timeout()
-
         elif status.command == 'outofbounds':
             self.bounds_signal.emit(True)
 
-        elif status.command == 'show_splash':
-            self.settings_tree.setEnabled(False)
-            self.splash_sc.show()
-            self.splash_sc.raise_()
-            self.splash_sc.showMessage(status.attribute[0], color=Qt.white)
-
-        elif status.command == 'close_splash':
-            self.splash_sc.close()
-            self.settings_tree.setEnabled(True)
-
         elif status.command == 'set_allowed_values':
             if self.ui is not None:
-                self.ui.set_spinbox_properties(**status.attribute)
+                self.ui.set_abs_spinbox_properties(**status.attribute)
 
-    def get_position(self):
-        deprecation_msg(f'This method is deprecated , please use `get_actuator_value`')
-        self.get_actuator_value()
+        elif status.command == 'stop':
+            self.stop_motion()
 
     def get_actuator_value(self):
         """Get the current actuator value via the "get_actuator_value" command send to the hardware
 
         Returns nothing but the  `move_done_signal` will be send once the action is done
         """
         try:
@@ -895,35 +788,35 @@
         """
         self._current_value = pos
         self.status_sig.emit(ThreadCommand(command="move_done", attribute=[pos]))
 
     @Slot(ThreadCommand)
     def queue_command(self, command: ThreadCommand):
         """Interpret command send by DAQ_Move class
-                * In case of **'ini_stage'** command, init a stage from command attribute.
-                * In case of **'close'** command, unitinalise the stage closing hardware and emitting the corresponding status signal
-                * In case of **'move_abs'** command, call the move_Abs method with position from command attribute
-                * In case of **'move_rel'** command, call the move_Rel method with the relative position from the command attribute.
-                * In case of **'move_home'** command, call the move_Home method
-                * In case of **'get_actuator_value'** command, get the current position from the check_position method
-                * In case of **'Stop_motion'** command, stop any motion via the stop_Motion method
-                * In case of **'reset_stop_motion'** command, set the motion_stopped attribute to false
+                * **ini_stage** command, init a stage from command attribute.
+                * **close** command, unitinalise the stage closing hardware and emitting the corresponding status signal
+                * **move_abs** command, call the move_Abs method with position from command attribute
+                * **move_rel** command, call the move_Rel method with the relative position from the command attribute.
+                * **move_home** command, call the move_home method
+                * **get_actuator_value** command, get the current position from the check_position method
+                * **Stop_motion** command, stop any motion via the stop_Motion method
+                * **reset_stop_motion** command, set the motion_stopped attribute to false
 
         Parameters
         ----------
         command: ThreadCommand
             Possible commands are:
-            * **'ini_stage'** command, init a stage from command attribute.
-            * **'close'** command, unitinalise the stage closing hardware and emitting the corresponding status signal
-            * **'move_abs'** command, call the move_abs method with position from command attribute
-            * **'move_rel'** command, call the move_rel method with the relative position from the command attribute.
-            * **'move_home'** command, call the move_home method
-            * **'get_actuator_value'** command, get the current position from the check_position method
-            * **'stop_motion'** command, stop any motion via the stop_Motion method
-            * **'reset_stop_motion'** command, set the motion_stopped attribute to false
+            * **ini_stage** command, init a stage from command attribute.
+            * **close** command, unitinalise the stage closing hardware and emitting the corresponding status signal
+            * **move_abs** command, call the move_abs method with position from command attribute
+            * **move_rel** command, call the move_rel method with the relative position from the command attribute.
+            * **move_home** command, call the move_home method
+            * **get_actuator_value** command, get the current position from the check_position method
+            * **stop_motion** command, stop any motion via the stop_Motion method
+            * **reset_stop_motion** command, set the motion_stopped attribute to false
         """
         try:
             if command.command == "ini_stage":
                 status = self.ini_stage(
                     *command.attribute)  # return edict(initialized=bool,info="", controller=, stage=)
                 self.status_sig.emit(ThreadCommand(command=command.command, attribute=[status, 'log']))
 
@@ -996,14 +889,17 @@
         elif path[0] == 'move_settings':
             self.hardware.update_settings(settings_parameter_dict)
 
 
 def main(init_qt=True):
     if init_qt:  # used for the test suite
         app = QtWidgets.QApplication(sys.argv)
+        if config('style', 'darkstyle'):
+            import qdarkstyle
+            app.setStyleSheet(qdarkstyle.load_stylesheet(qdarkstyle.DarkPalette))
 
     widget = QtWidgets.QWidget()
     prog = DAQ_Move(widget, title="test")
     widget.show()
 
     if init_qt:
         sys.exit(app.exec_())
```

### Comparing `pymodaq-4.0.2/src/pymodaq/control_modules/daq_move_ui.py` & `pymodaq-4.0.3/src/pymodaq/control_modules/daq_move_ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,28 @@
         self.abs_value_sb.setEnabled(status)
         self.abs_value_sb_2.setEnabled(status)
         self.control_ui.setEnabled(status)
 
         self.get_action('move_abs').setEnabled(status)
         self.get_action('move_abs_2').setEnabled(status)
 
-    def set_spinbox_properties(self, **properties):
+    def set_abs_spinbox_properties(self, **properties):
+        """ Change the Spinbox properties
+
+        Parameters
+        --------
+        properties: dict or named parameters
+            possible keys are :
+
+            * decimals: to set the number of displayed decimals
+            * 'minimum': to set the minimum value
+            * 'maximum': to set the maximum value
+            * 'step': to set the step value
+
+        """
         if 'decimals' in properties:
             self.abs_value_sb.setDecimals(properties['decimals'])
             self.abs_value_sb_2.setDecimals(properties['decimals'])
             self.abs_value_sb_bis.setDecimals(properties['decimals'])
         if 'minimum' in properties:
             self.abs_value_sb.setMinimum()
             self.abs_value_sb_2.setMinimum(properties['minimum'])
```

### Comparing `pymodaq-4.0.2/src/pymodaq/control_modules/daq_viewer.py` & `pymodaq-4.0.3/src/pymodaq/control_modules/daq_viewer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 # -*- coding: utf-8 -*-
 """
 Created on Wed Jan 10 16:54:14 2018
 
 @author: Weber Sébastien
 """
 from __future__ import annotations
+
 from collections import OrderedDict
 import copy
-import datetime
 import os
 from pathlib import Path
 import sys
 from typing import List, Tuple, Union
 import time
 
 from easydict import EasyDict as edict
 import numpy as np
 from qtpy import QtWidgets
 from qtpy.QtCore import Qt, QObject, Slot, QThread, Signal
 
-from pymodaq.utils.data import DataRaw, DataFromPlugins, DataToExport, Axis, DataDistribution
+from pymodaq.utils.data import DataFromPlugins, DataToExport, Axis, DataDistribution
 from pymodaq.utils.logger import set_logger, get_module_name
 from pymodaq.control_modules.utils import ControlModule
 from pymodaq.utils.gui_utils.file_io import select_file
-from pymodaq.utils.gui_utils.utils import widget_to_png_to_bytes
-import pymodaq.utils.scanner
 from pymodaq.utils.tcp_server_client import TCPClient
 from pymodaq.utils.gui_utils.widgets.lcd import LCD
 from pymodaq.utils.config import Config, get_set_local_dir
 from pymodaq.utils.h5modules.browsing import browse_data
 from pymodaq.utils.h5modules.saving import H5Saver
 from pymodaq.utils.h5modules import module_saving
 from pymodaq.utils.h5modules.backends import Node
@@ -40,15 +38,15 @@
 from pymodaq.utils.messenger import deprecation_msg
 from pymodaq.utils.gui_utils import DockArea, get_splash_sc, Dock
 from pymodaq.utils.managers.parameter_manager import ParameterManager, Parameter
 from pymodaq.control_modules.daq_viewer_ui import DAQ_Viewer_UI
 from pymodaq.control_modules.utils import DET_TYPES, get_viewer_plugins, DAQTypesEnum
 from pymodaq.utils.plotting.data_viewers.viewer import ViewerBase, ViewersEnum
 from pymodaq.utils.enums import enum_checker
-
+from pymodaq.control_modules.viewer_utility_classes import DAQ_Viewer_base
 
 logger = set_logger(get_module_name(__file__))
 config = Config()
 
 local_path = get_set_local_dir()
 
 
@@ -134,15 +132,17 @@
         self.splash_sc = get_splash_sc()
 
         self._title = title
 
         self.module_and_data_saver: Union[module_saving.DetectorSaver,
                                           module_saving.DetectorEnlargeableSaver,
                                           module_saving.DetectorExtendedSaver] = None
-        self.setup_saving_objects()
+        self._h5saver_continuous: H5Saver = None
+        self._ind_continuous_grab = 0
+        self.setup_continuous_saving()
 
         self._external_h5_data = None
 
         self.settings.child('main_settings', 'DAQ_type').setValue(self.daq_type.name)
         self._detectors: List[str] = [det_dict['name'] for det_dict in DET_TYPES[self.daq_type.name]]
         if len(self._detectors) > 0:  # will be 0 if no valid plugins are installed
             self._detector: str = self._detectors[0]
@@ -154,32 +154,32 @@
 
         self._grab_done: bool = False
         self._start_grab_time: float = 0.  # used for the refreshing rate
         self._received_data: int = 0
 
         self._lcd: LCD = None
 
-        self._bkg: List[DataFromPlugins] = None  # buffer to store background
+        self._bkg: DataToExport = None  # buffer to store background
 
         self._save_file_pathname: Path = None  # to store last active path, will be an Path object
         
         self._snapshot_pathname: Path = None
-        self._current_data: DataToExport = None
         self._data_to_save_export: DataToExport = None
 
         self._do_save_data: bool = False
 
         self._set_setting_tree()  # to activate parameters of default Mock detector
 
         self.grab_done_signal.connect(self._save_export_data)
 
     def __repr__(self):
         return f'{self.__class__.__name__}: {self.title} ({self.daq_type}/{self.detector}'
 
-    def setup_saving_objects(self):
+    def setup_continuous_saving(self):
+        """Configure the objects dealing with the continuous saving mode"""
         self.module_and_data_saver = module_saving.DetectorSaver(self)
         self._h5saver_continuous = H5Saver(save_type='detector')
         self._h5saver_continuous.show_settings(False)
         self._h5saver_continuous.settings.child('do_save').sigValueChanged.connect(self._init_continuous_save)
         if self.ui is not None:
             self.ui.add_setting_tree(self._h5saver_continuous.settings_tree)
 
@@ -234,33 +234,40 @@
         elif cmd.command == 'do_bkg':
             self.do_bkg = cmd.attribute
         elif cmd.command == 'viewers_changed':
             self._viewer_types: List[ViewersEnum] = cmd.attribute['viewer_types']
             self.viewers = cmd.attribute['viewers']
 
     @property
-    def bkg(self):
+    def bkg(self) -> DataToExport:
+        """Get the background data object"""
         return self._bkg
 
     @property
-    def viewer_docks(self):
-        """:obj:`list` of Viewer Docks from the UI"""
+    def viewer_docks(self) -> List[Dock]:
+        """list of Viewer Docks from the UI"""
         if self.ui is not None:
             return self.ui.viewer_docks
 
     def daq_type_changed_from_ui(self, daq_type: DAQTypesEnum):
+        """ Apply changes from the selection of a different DAQTypesEnum in the UI
+
+        Parameters
+        ----------
+        daq_type: DAQTypesEnum
+        """
         daq_type = enum_checker(DAQTypesEnum, daq_type)
         self._daq_type = daq_type
         self.settings.child('main_settings', 'DAQ_type').setValue(daq_type.name)
         self.detectors = [det_dict['name'] for det_dict in DET_TYPES[daq_type.name]]
         self.detector = self.detectors[0]
 
     @property
     def daq_type(self) -> DAQTypesEnum:
-        """:obj:`DAQTypesEnum`: Get/Set the daq_type
+        """Get/Set the daq_type as a DAQTypesEnum
 
         Update the detector property with the list of available detectors of a given daq_type
         """
         return self._daq_type
 
     @daq_type.setter
     def daq_type(self, daq_type: DAQTypesEnum):
@@ -270,68 +277,67 @@
         if self.ui is not None:
             self.ui.daq_type = daq_type
         self.settings.child('main_settings', 'DAQ_type').setValue(daq_type.name)
         self.detectors = [det_dict['name'] for det_dict in DET_TYPES[daq_type.name]]
         self.detector = self.detectors[0]
 
     @property
-    def daq_types(self):
-        """:obj:`list` of :obj:`str`: List of available DAQ_TYPES"""
+    def daq_types(self) -> List[str]:
+        """List of available DAQ_TYPES as keys of the DAQTypesEnum"""
         return DAQTypesEnum.names()
 
-    def detector_changed_from_ui(self, detector):
+    def detector_changed_from_ui(self, detector: str):
         self._detector = detector
         self._set_setting_tree()
 
     @property
-    def detector(self):
-        """:obj:`str`: Get/Set the detector among detectors property"""
+    def detector(self) -> str:
+        """:obj:`str`: Get/Set the currently selected detector among available detectors"""
         return self._detector
 
     @detector.setter
-    def detector(self, det):
+    def detector(self, det: str):
         if det not in self.detectors:
             raise ValueError(f'{det} is not a valid Detector: {self.detectors}')
         self._detector = det
         if self.ui is not None:
             self.ui.detector = det
         self._set_setting_tree()
 
-    def detectors_changed_from_ui(self, detectors):
+    def detectors_changed_from_ui(self, detectors: List[str]):
         self._detectors = detectors
 
     @property
-    def detectors(self):
-        """:obj:`list` of :obj:`str`: List of available detectors of the current daq_type"""
+    def detectors(self) -> str:
+        """:obj:`list` of :obj:`str`: List of available detectors of the current daq_type (DAQTypesEnum)"""
         return self._detectors
 
     @detectors.setter
     def detectors(self, detectors):
         self._detectors = detectors
         if self.ui is not None:
             self.ui.detectors = detectors
 
     @property
     def grab_state(self):
         """:obj:`bool`: Get the current grabbing status"""
         return self._grabing
 
-
     @property
-    def do_bkg(self):
+    def do_bkg(self) -> bool:
         """:obj:`bool`: Get/Set if background subtraction should be done"""
         return self._do_bkg
 
     @do_bkg.setter
     def do_bkg(self, doit: bool):
         self._do_bkg = doit
 
     @property
     def viewers(self) -> List[ViewerBase]:
-        """:obj:`list` of Viewers from the UI"""
+        """:obj:`list`: Get/Set the Viewers (instances of real implementation of ViewerBase class) from the UI"""
         if self.ui is not None:
             return self._viewers
 
     @viewers.setter
     def viewers(self, viewers):
         for viewer in self._viewers:
             try:
@@ -341,22 +347,16 @@
         for viewer in viewers:
             viewer.data_to_export_signal.connect(self._get_data_from_viewer)
             if hasattr(viewer, 'ROI_select_signal'):
                 viewer.ROI_select_signal.connect(
                     lambda roi_pos_size: self.command_hardware.emit(ThreadCommand('ROISelect', roi_pos_size)))
         self._viewers = viewers
 
-    @property
-    def viewers_docks(self):
-        if self.ui is not None:
-            return self.ui.viewer_docks
-
     def quit_fun(self):
-        """Quit the application, closing the hardware and other modules
-        """
+        """ Quit the application, closing the hardware and other modules """
 
         # insert anything that needs to be closed before leaving
 
         if self._initialized_state:  # means  initialized
             self.init_hardware(False)
         self.quit_signal.emit()
 
@@ -380,24 +380,16 @@
     #  Methods for running the acquisition
 
     def init_hardware_ui(self, do_init=True):
         """Send a command to the underlying UI to click the init button"""
         if self.ui is not None:
             self.ui.do_init()
 
-    def init_det(self):
-        deprecation_msg(f'The function *init_det* is deprecated, use init_hardware_ui')
-        self.init_hardware_ui(True)
-
-    def ini_det_fun(self):
-        deprecation_msg(f'The function *ini_det_fun* is deprecated, use init_hardware')
-        self.init_hardware(True)
-
     def init_hardware(self, do_init=True):
-        """Init the selected detector
+        """ Init the selected detector
 
         Parameters
         ----------
         do_init: bool
             If True, create a DAQ_Detector instance and move it into a separated thread, connected its signals/slots
             to the DAQ_Viewer object (self)
             If False, force the instrument to close and kill the Thread (still not done properly in some cases)
@@ -416,16 +408,16 @@
 
                 hardware = DAQ_Detector(self._title, self.settings, self.detector)
                 self._hardware_thread = QThread()
                 if config('viewer', 'viewer_in_thread'):
                     hardware.moveToThread(self._hardware_thread)
 
                 self.command_hardware[ThreadCommand].connect(hardware.queue_command)
-                hardware.data_detector_sig[list].connect(self.show_data)
-                hardware.data_detector_temp_sig[list].connect(self.show_temp_data)
+                hardware.data_detector_sig[DataToExport].connect(self.show_data)
+                hardware.data_detector_temp_sig[DataToExport].connect(self.show_temp_data)
                 hardware.status_sig[ThreadCommand].connect(self.thread_status)
                 self._update_settings_signal[edict].connect(hardware.update_settings)
 
                 self._hardware_thread.hardware = hardware
                 if config('viewer', 'viewer_in_thread'):
                     self._hardware_thread.start()
                 self.command_hardware.emit(ThreadCommand("ini_detector", attribute=[
@@ -434,54 +426,54 @@
                     for dock in self.ui.viewer_docks:
                         dock.setEnabled(True)
 
             except Exception as e:
                 self.logger.exception(str(e))
 
     def snap(self):
-        """Programmatic click on the UI snap button"""
+        """ Launch a single grab """
         self.grab_data(False, snap_state=True)
 
     def grab(self):
-        """Programmatic click on the UI grab button"""
+        """ Launch a continuous grab """
         if self.ui is not None:
             self.manage_ui_actions('grab', 'setChecked', not self._grabing)
             self.grab_data(not self._grabing, snap_state=False)
 
     def snapshot(self, pathname=None, dosave=False, send_to_tcpip=False):
         """Do one single grab (snap) and eventually save the data.
 
         Parameters
         ----------
         pathname: str or Path object
             The path where to save data
         dosave: bool
             Do save or just grab data
         send_to_tcpip: bool
-            If True, send the grabed data through the TCP/IP pipe
+            If True, send the grabbed data through the TCP/IP pipe
         """
         try:
             self._do_save_data = dosave
             if pathname is None:
                 raise (ValueError("filepathanme has not been defined in snapshot"))
 
             self._save_file_pathname = pathname
             self.grab_data(grab_state=False, send_to_tcpip=send_to_tcpip, snap_state=True)
         except Exception as e:
             self.logger.exception(str(e))
 
     def grab_data(self, grab_state=False, send_to_tcpip=False, snap_state=False):
-        """Generic method to grab or snap data from the selected (and initialized) detector
+        """ Generic method to grab or snap data from the selected (and initialized) detector
 
         Parameters
         ----------
         grab_state: bool
-            Defines the grab status: if True: do live grabing if False stops the grab
+            Defines the grab status: if True: do live grabbing if False stops the grab
         send_to_tcpip: bool
-            If True, send the grabed data through the TCP/IP pipe
+            If True, send the grabbed data through the TCP/IP pipe
         snap_state: bool
             if True performs a single grab
         """
         self._grabing = grab_state
         self._send_to_tcpip = send_to_tcpip
         self._grab_done = False
 
@@ -500,27 +492,34 @@
             else:
                 self.thread_status(ThreadCommand("update_channels", ))
                 self.update_status(f'{self._title}: Continuous Grab')
                 self.command_hardware.emit(
                     ThreadCommand("grab", [self.settings.child('main_settings', 'Naverage').value()]))
 
     def take_bkg(self):
-        """Do a snap and store data to be used as background into an attribute: `self._bkg`
+        """ Do a snap and store data to be used as background into an attribute: `self._bkg`
 
         The content of the bkg will be saved if data is further saved with do_bkg property set to True
         """
         self._take_bkg = True
         self.grab_data(snap_state=True)
 
     def stop_grab(self):
+        """ Stop the current continuous grabbing and unchecked the stop button of the UI
+
+        See Also
+        --------
+        :meth:`stop`
+        """
         if self.ui is not None:
             self.manage_ui_actions('grab', 'setChecked', False)
         self.stop()
 
     def stop(self):
+        """ Stop the current continuous grabbing """
         self.update_status(f'{self._title}: Stop Grab')
         self.command_hardware.emit(ThreadCommand("stop_all", ))
         self._grabing = False
 
     @Slot()
     def _raise_timeout(self):
         """  Print the "timeout occurred" error message in the status bar via the update_status method.
@@ -531,15 +530,14 @@
     def load_data():
         """Opens a H5 file in the H5Browser module
 
         Convenience static method.
         """
         browse_data()
 
-
     def save_current(self):
         """Save current data into a h5file"""
         self._do_save_data = True
         self._save_file_pathname = select_file(start_path=self._save_file_pathname, save=True,
                                                                                   ext='h5')  # see daq_utils
         self._save_export_data(self._data_to_save_export)
 
@@ -547,14 +545,18 @@
         """Snap data and save them into a h5file"""
         self._do_save_data = True
         self._save_file_pathname = select_file(start_path=self._save_file_pathname, save=True,
                                                                                   ext='h5')  # see daq_utils
         self.snapshot(pathname=self._save_file_pathname, dosave=True)
 
     def _init_continuous_save(self):
+        """ Initialize the continuous saving H5Saver object
+
+        Update the module_and_data_saver attribute as :class:`DetectorEnlargeableSaver` object
+        """
         if self._h5saver_continuous.settings.child('do_save').value():
 
             self._h5saver_continuous.settings.child('base_name').setValue('Data')
             self._h5saver_continuous.settings.child('N_saved').show()
             self._h5saver_continuous.settings.child('N_saved').setValue(0)
             self.module_and_data_saver.h5saver = self._h5saver_continuous
             self._h5saver_continuous.init_file(update_h5=True)
@@ -573,41 +575,43 @@
                 self._h5saver_continuous.close()
             except Exception as e:
                 self.logger.exception(str(e))
 
     def append_data(self, data: DataToExport = None, where: Union[Node, str] = None):
         """Appends current DataToExport to a DetectorEnlargeableSaver
 
+        Method to be used when performing continuous saving into a h5file (continuous mode or DAQ_Logger)
+
         Parameters
         ----------
         data: DataToExport
             not really used
         where: Node or str
         See Also
         --------
-        DetectorEnlargeableSaver
+        :class:`DetectorEnlargeableSaver`
         """
         if data is None:
             data = self._data_to_save_export
         self._add_data_to_saver(data, init_step=self._h5saver_continuous.settings['N_saved'] == 0,
                                 where=where)
         self._h5saver_continuous.settings.child('N_saved').setValue(self._h5saver_continuous.settings['N_saved'] + 1)
 
     def insert_data(self, indexes: Tuple[int], where: Union[Node, str] = None,
                     distribution=DataDistribution['uniform']):
         """Insert DataToExport to a DetectorExtendedSaver at specified indexes
 
+        Method to be used when saving into an already initialized array within a h5file (DAQ_Scan for instance)
+
         Parameters
         ----------
         indexes: tuple(int)
             The indexes within the extended array where to place these data
         where: Node or str
         distribution: DataDistribution enum
-        save_raw_only: bool
-            If True save only Raw data (no data processed from Roi)
 
         See Also
         --------
         DAQ_Scan, DetectorExtendedSaver
         """
         self._add_data_to_saver(self._data_to_save_export, init_step=np.all(np.array(indexes) == 0), where=where,
                                 indexes=indexes, distribution=distribution)
@@ -661,36 +665,32 @@
         if path is not None:
             path = Path(path)
         h5saver = H5Saver(save_type='detector')
         h5saver.init_file(update_h5=True, custom_naming=False, addhoc_file_path=path)
         self.module_and_data_saver = module_saving.DetectorSaver(self)
         self.module_and_data_saver.h5saver = h5saver
 
-        self._add_data_to_saver(data)
+        self._add_data_to_saver(data, init_step=True)
 
         if self.ui is not None:
             (root, filename) = os.path.split(str(path))
             filename, ext = os.path.splitext(filename)
             image_path = os.path.join(root, filename + '.png')
             self.dockarea.parent().grab().save(image_path)
 
         h5saver.close_file()
         self.data_saved.emit()
 
-    @Slot(OrderedDict)
+    @Slot(DataToExport)
     def _save_export_data(self, data: DataToExport):
         """Auxiliary method (Slot) to receive all data (raw and processed from rois) and save them
 
         Parameters
         ----------
         data: DataToExport
-            contains a timestamp and data (raw and extracted from roi in dataviewers) on the dorm:
-            `_data_to_save_export = OrderedDict(Ndatas=Ndatas, acq_time_s=acq_time, name=name,
-             control_module='DAQ_Viewer')`
-             with extra keys for data dimensionality such as Data0D=OrderedDict(...)
 
         See Also
         --------
         _save_data
         """
 
         if self._do_save_data:
@@ -720,32 +720,33 @@
 
             if self._received_data == len(self.viewers):
                 self._grab_done = True
                 self.grab_done_signal.emit(self._data_to_save_export)
 
     @property
     def current_data(self) -> DataToExport:
+        """ Get the current data stored internally"""
         return self._data_to_save_export
 
-    @Slot(list)
-    def show_temp_data(self, data: List[DataFromPlugins]):
+    @Slot(DataToExport)
+    def show_temp_data(self, data: DataToExport):
         """Send data to their dedicated viewers but those will not emit processed data signal
 
         Slot receiving data from plugins emitted with the `data_grabed_signal_temp`
 
         Parameters
         ----------
         data: list of DataFromPlugins
         """
         self._init_show_data(data)
         if self.ui is not None:
             self.set_data_to_viewers(data, temp=True)
 
-    @Slot(list)
-    def show_data(self, data: List[DataFromPlugins]):
+    @Slot(DataToExport)
+    def show_data(self, dte: DataToExport):
         """Send data to their dedicated viewers but those will not emit processed data signal
 
         Slot receiving data from plugins emitted with the `data_grabed_signal`
         Process the data as specified in the settings, display them into the dedicated data viewers depending on the
         settings:
             * create a container (OrderedDict `_data_to_save_export`) with info from this DAQ_Viewer (title), a timestamp...
             * call `_process_data`
@@ -753,41 +754,40 @@
             * check refresh time (if set in the settings) to send or not data to data viewers
             * either send to the data viewers (if refresh time is ok and/or show data option in settings is set)
             * either
                 * send grab_done_signal (to the slot _save_export_data ) to save the data
 
         Parameters
         ----------
-        data: list of DataFromPlugins
+        dte: DataToExport
 
         See Also
         --------
         _init_show_data, _process_data
         """
         try:
             if self.settings.child('main_settings', 'tcpip', 'tcp_connected').value() and self._send_to_tcpip:
-                self._command_tcpip.emit(ThreadCommand('data_ready', data))
+                self._command_tcpip.emit(ThreadCommand('data_ready', dte))
             if self.ui is not None:
                 self.ui.data_ready = True
-            self._init_show_data(data)
-
-            # store raw data for further processing
-            self._data_to_save_export = DataToExport(self._title, control_module='DAQ_Viewer', data=data)
+            self._init_show_data(dte)
 
             if self.settings['main_settings', 'live_averaging']:
                 self.settings.child('main_settings', 'N_live_averaging').setValue(self._ind_continuous_grab)
-                self._current_data = copy.deepcopy(self._data_to_save_export)
+                _current_data = dte.deepcopy()
 
                 self._ind_continuous_grab += 1
                 if self._ind_continuous_grab > 1:
                     self._data_to_save_export = \
-                        self._data_to_save_export.average(self._current_data, self._ind_continuous_grab)
+                        _current_data.average(self._data_to_save_export, self._ind_continuous_grab)
+            else:
+                self._data_to_save_export = DataToExport(self._title, control_module='DAQ_Viewer', data=dte.data)
 
             if self._take_bkg:
-                self._bkg = copy.deepcopy(self._data_to_save_export)
+                self._bkg = self._data_to_save_export.deepcopy()
                 self._take_bkg = False
 
             if self._grabing:  # if live
                 refresh_time = self.settings['main_settings', 'refresh_time']
                 refresh = time.perf_counter() - self._start_grab_time > refresh_time / 1000
                 if refresh:
                     self._start_grab_time = time.perf_counter()
@@ -803,23 +803,23 @@
             else:
                 self._grab_done = True
                 self.grab_done_signal.emit(self._data_to_save_export)
 
         except Exception as e:
             self.logger.exception(str(e))
 
-    def _init_show_data(self, data):
+    def _init_show_data(self, data: DataToExport):
         """Processing before showing data
 
         * process the data to check if they overshoot
         * check the data dimensionality to update the dedicated viewers
 
         Parameters
         ----------
-        data: list of DataFromPlugins
+        data: DataToExport
 
         See Also
         --------
         _process_overshoot
         """
         self._process_overshoot(data)
         self._viewer_types = [ViewersEnum(data.dim.name) for data in data]
@@ -845,15 +845,15 @@
             self.viewer_docks[ind].setTitle(self._title + ' ' + data.name)
 
             if temp:
                 self.viewers[ind].show_data_temp(data)
             else:
                 self.viewers[ind].show_data(data)
 
-    def value_changed(self, param):
+    def value_changed(self, param: Parameter):
         """ParameterManager subclassed method. Process events from value changed by user in the UI Settings
 
         Parameters
         ----------
         param: Parameter
             a given parameter whose value has been changed by user
         """
@@ -870,14 +870,15 @@
             self.settings.child('main_settings', 'show_averaging').setValue(False)
             if param.value():
                 self.settings.child('main_settings', 'N_live_averaging').show()
                 self._ind_continuous_grab = 0
                 self.settings.child('main_settings', 'N_live_averaging').setValue(0)
             else:
                 self.settings.child('main_settings', 'N_live_averaging').hide()
+            #self._update_settings_signal.emit(edict(path=path, param=param, change='value'))
 
         elif param.name() in putils.iter_children(self.settings.child('main_settings', 'axes'), []):
             if self.daq_type.name == "DAQ2D":
                 if param.name() == 'use_calib':
                     if param.value() != 'None':
                         params = ioxml.XML_file_to_parameter(
                             os.path.join(local_path, 'camera_calibrations', param.value() + '.xml'))
@@ -912,28 +913,29 @@
             if 'main_settings' not in path:
                 self._update_settings_signal.emit(edict(path=path, param=param, change='value'))
 
                 if self.settings.child('main_settings', 'tcpip', 'tcp_connected').value():
                     self._command_tcpip.emit(ThreadCommand('send_info', dict(path=path, param=param)))
 
     def child_added(self, param, data):
-        """Non-mandatory method to be subclassed for actions to perform when a param  has been added in self.settings
+        """ Adds a child in the settings attribute
 
         Parameters
         ----------
         param: Parameter
             the parameter where child will be added
         data: Parameter
             the child parameter
         """
         if param.name() not in putils.iter_children(self.settings.child('main_settings'), []):
-            self._update_settings_signal.emit(edict(path=putils.get_param_path(param)[1:], param=data[0], change='childAdded'))
+            self._update_settings_signal.emit(edict(path=putils.get_param_path(param)[1:], param=data[0],
+                                                    change='childAdded'))
 
     def param_deleted(self, param):
-        """ParameterManager subclassed method. Process events from parameter deleted by user in the UI Settings
+        """ Remove a child from the settings attribute
 
         Parameters
         ----------
         param: Parameter
             a given parameter whose value has been changed by user
         """
         if param.name() not in putils.iter_children(self.settings.child('main_settings'), []):
@@ -955,192 +957,101 @@
                     child.remove()
 
             det_params, _class = get_viewer_plugins(self.daq_type.name, self.detector)
             self.settings.child('detector_settings').addChildren(det_params.children())
         except Exception as e:
             self.logger.exception(str(e))
 
-    def _process_overshoot(self, data):
+    def _process_overshoot(self, dte: DataToExport):
         """Compare data value (0D) to the given overshoot setting
         """
         if self.settings.child('main_settings', 'overshoot', 'stop_overshoot').value():
-            for channels in data:
-                for channel in channels['data']:
-                    if any(channel >= self.settings.child('main_settings', 'overshoot', 'overshoot_value').value()):
+            for dwa in dte:
+                for data_array in dwa.data:
+                    if any(data_array >= self.settings.child('main_settings', 'overshoot', 'overshoot_value').value()):
                         self.overshoot_signal.emit(True)
 
     def get_scaling_options(self):
         """Create axes scaling options depending on the ('main_settings', 'axes') settings
 
         Returns
         -------
-        pymodaq.utils.data.ScalingOptions
+        Tuple[Axis]
         """
         scaled_xaxis = Axis(label=self.settings['main_settings', 'axes', 'xaxis', 'xlabel'],
                             units=self.settings['main_settings', 'axes', 'xaxis', 'xunits'],
                             offset=self.settings['main_settings', 'axes', 'xaxis', 'xoffset'],
                             scaling=self.settings['main_settings', 'axes', 'xaxis', 'xscaling'])
         scaled_yaxis = Axis(label=self.settings['main_settings', 'axes', 'yaxis', 'ylabel'],
                             units=self.settings['main_settings', 'axes', 'yaxis', 'yunits'],
                             offset=self.settings['main_settings', 'axes', 'yaxis', 'yoffset'],
                             scaling=self.settings['main_settings', 'axes', 'yaxis', 'yscaling'])
         return scaled_xaxis, scaled_yaxis
 
-    @Slot(ThreadCommand)
-    def thread_status(self, status):
+    def thread_status(self, status: ThreadCommand):
         """Get back info (using the ThreadCommand object) from the hardware
 
         And re-emit this ThreadCommand using the custom_sig signal if it should be used in a higher level module
 
+        Commands valid for all control modules are defined in the parent class, here are described only the specific
+        ones
+
         Parameters
         ----------
         status: ThreadCommand
             The info returned from the hardware, the command (str) can be either:
-                * Update_Status: display messages and log info
                 * ini_detector: update the status with "detector initialized" value and init state if attribute not null.
-                * close: close the current thread and delete corresponding attribute on cascade.
                 * grab : emit grab_status(True)
                 * grab_stopped: emit grab_status(False)
-                * x_axis: update x_axis from status attribute and User Interface viewer consequently. (Deprecated)
-                * y_axis: update y_axis from status attribute and User Interface viewer consequently. (Deprecated)
-                * update_channel: update the viewer channels in case of 0D DAQ_type (deprecated)
-                * update_settings: Update the "detector setting" node in the settings tree.
-                * update_main_settings: update the "main setting" node in the settings tree
-                * raise_timeout:
-                * show_splash: Display the splash screen with attribute as message
-                * close_splash
                 * init_lcd: display a LCD panel
                 * lcd: display on the LCD panel, the content of the attribute
                 * stop: stop the grab
         """
-        if status.command == "Update_Status":
-            if len(status.attribute) > 1:
-                self.update_status(status.attribute[0], log=status.attribute[1])
-            else:
-                self.update_status(status.attribute[0])
+        super().thread_status(status, 'detector')
 
-        elif status.command == "ini_detector":
+        if status.command == "ini_detector":
             self.update_status("detector initialized: " + str(status.attribute[0]['initialized']))
             if self.ui is not None:
                 self.ui.detector_init = status.attribute[0]['initialized']
             if status.attribute[0]['initialized']:
                 self.controller = status.attribute[0]['controller']
                 self._initialized_state = True
             else:
                 self._initialized_state = False
 
             self.init_signal.emit(self._initialized_state)
 
-        elif status.command == "close":
-            try:
-                self.update_status(status.attribute[0])
-                self._hardware_thread.quit()
-                self._hardware_thread.wait()
-                finished = self._hardware_thread.isFinished()
-                if finished:
-                    pass
-                else:
-                    print('Thread still running')
-                    self._hardware_thread.terminate()
-                    self.update_status('thread is locked?!', 'log')
-            except Exception as e:
-                self.logger.exception(str(e))
-
-            self._initialized_state = False
-            self.init_signal.emit(self._initialized_state)
-
         elif status.command == "grab":
             self.grab_status.emit(True)
 
         elif status.command == 'grab_stopped':
             self.grab_status.emit(False)
 
-        elif status.command == "x_axis":
-            deprecation_msg(f'using emit_x_axis in plugins is deprecated use data emission with correct axis to set it.'
-                            f'To send it only once, use the data_grabed_signal_temp')
-
-        elif status.command == "y_axis":
-            deprecation_msg(f'using emit_y_axis in plugins is deprecated use data emission with correct axis to set it.'
-                            f'To send it only once, use the data_grabed_signal_temp')
-
-        elif status.command == "update_channels":
-            pass
-
-        elif status.command == 'update_main_settings':
-            # this is a way for the plugins to update main settings of the ui (solely values, limits and options)
-            try:
-                if status.attribute[2] == 'value':
-                    self.settings.child('main_settings', *status.attribute[0]).setValue(status.attribute[1])
-                elif status.attribute[2] == 'limits':
-                    self.settings.child('main_settings', *status.attribute[0]).setLimits(status.attribute[1])
-                elif status.attribute[2] == 'options':
-                    self.settings.child('main_settings', *status.attribute[0]).setOpts(**status.attribute[1])
-            except Exception as e:
-                self.logger.exception(str(e))
-
-        elif status.command == 'update_settings':
-            # using this the settings shown in the UI for the plugin reflects the real plugin settings
-            try:
-                self.settings.sigTreeStateChanged.disconnect(
-                    self.parameter_tree_changed)  # any changes on the detcetor settings will update accordingly the gui
-            except Exception as e:
-                self.logger.exception(str(e))
-            try:
-                if status.attribute[2] == 'value':
-                    self.settings.child('detector_settings', *status.attribute[0]).setValue(status.attribute[1])
-                elif status.attribute[2] == 'limits':
-                    self.settings.child('detector_settings', *status.attribute[0]).setLimits(status.attribute[1])
-                elif status.attribute[2] == 'options':
-                    self.settings.child('detector_settings', *status.attribute[0]).setOpts(**status.attribute[1])
-                elif status.attribute[2] == 'childAdded':
-                    child = Parameter.create(name='tmp')
-                    child.restoreState(status.attribute[1][0])
-                    self.settings.child('detector_settings', *status.attribute[0]).addChild(status.attribute[1][0])
-
-            except Exception as e:
-                self.logger.exception(str(e))
-            self.settings.sigTreeStateChanged.connect(self.parameter_tree_changed)
-
-        elif status.command == 'raise_timeout':
-            self._raise_timeout()
-
-        elif status.command == 'show_splash':
-            self.ui.settings_tree.setEnabled(False)
-            self.splash_sc.show()
-            self.splash_sc.raise_()
-            self.splash_sc.showMessage(status.attribute[0], color=Qt.white)
-
-        elif status.command == 'close_splash':
-            self.splash_sc.close()
-            self.ui.settings_tree.setEnabled(True)
-
         elif status.command == 'init_lcd':
             if self._lcd is not None:
                 try:
                     self._lcd.parent.close()
                 except Exception as e:
                     self.logger.exception(str(e))
             # lcd module
             lcd = QtWidgets.QWidget()
-            self._lcd = LCD(lcd, **status.attribute[0])
+            self._lcd = LCD(lcd, **status.attribute)
             lcd.setVisible(True)
             QtWidgets.QApplication.processEvents()
 
         elif status.command == 'lcd':
-            self._lcd.setvalues(status.attribute[0])
+            self._lcd.setvalues(status.attribute)
 
         elif status.command == 'stop':
-            self.stop()
-
-        self.custom_sig.emit(status)  # to be used if needed in custom application connected to this module
+            self.stop_grab()
 
     def connect_tcp_ip(self):
         """Init a TCPClient in a separated thread to communicate with a distant TCp/IP Server
 
-        Use the settings: ip_adress and port to specify the connection
+        Use the settings: ip_address and port to specify the connection
 
         See Also
         --------
         TCPServer
         """
         if self.settings.child('main_settings', 'tcpip', 'connect_server').value():
             self._tcpclient_thread = QThread()
@@ -1198,89 +1109,71 @@
 
         elif status.command == 'get_axis':
             self.command_hardware.emit(
                 ThreadCommand('get_axis', ))  # tells the plugin to emit its axes so that the server will receive them
 
 
 class DAQ_Detector(QObject):
-    """
-        ========================= ==========================
-        **Attributes**              **Type**
-        *status_sig*                instance of pyqt Signal
-        *data_detector_sig*         instance of pyqt Signal
-        *data_detector_temp_sig*    instance of pyqt Signal
-
-        *waiting_for_data*          boolean
-        *controller*                ???
-        *detector_name*             string
-        *detector*                  ???
-        *controller_adress*         ???
-        *grab_state*                boolean
-        *single_grab*               boolean
-        *x_axis*                    1D numpy array
-        *y_axis*                    1D numpy array
-        *datas*                     dictionnary
-        *ind_average*               int
-        *Naverage*                  int
-        *average_done*              boolean
-        *hardware_averaging*        boolean
-        *show_averaging*            boolean
-        *wait_time*                 int
-        *daq_type*                  string
-        ========================= ==========================
+    """ Worker class to control the instrument plugin
+
+    Attributes
+    ----------
+    detector: real instance of the instrument plugin class
+    controller: DAQ_Viewer_base
+        wrapper object used to control a given instrument in the instrument plugin
+    controller_adress: int
+        unique integer used to identify a controller shared among multiple instrument plugins
+
     """
     status_sig = Signal(ThreadCommand)
-    data_detector_sig = Signal(list)
-    data_detector_temp_sig = Signal(list)
+    data_detector_sig = Signal(DataToExport)
+    data_detector_temp_sig = Signal(DataToExport)
 
     def __init__(self, title, settings_parameter, detector_name):
         super().__init__()
         self.waiting_for_data = False
         self.controller = None
         self.logger = set_logger(f'{logger.name}.{title}.detector')
         self.detector_name = detector_name
-        self.detector = None
-        self.controller_adress = None
+        self.detector: DAQ_Viewer_base = None
+        self.controller_adress: int = None
         self.grab_state = False
         self.single_grab = False
-        self.datas = None
+        self.datas: DataToExport = None
         self.ind_average = 0
-        self.Naverage = None
+        self.Naverage = 1
         self.average_done = False
         self.hardware_averaging = False
         self.show_averaging = False
         self.wait_time = settings_parameter['main_settings', 'wait_time']
         self.daq_type = DAQTypesEnum[settings_parameter['main_settings', 'DAQ_type']]
 
-    @Slot(edict)
     def update_settings(self, settings_parameter_dict):
-        """
-            | Set attribute values in case of "main_settings" path with corresponding parameter values.
-            | Recursively call the method on detector class attribute else.
+        """ Apply a Parameter serialized as a dict to the instrument plugin class or to self
+
+        Parameters
+        ----------
+        settings_parameter_dict: dict
+            dictionary serializing a Parameter object
 
-            ======================== ============== ======================================
-            **Parameters**             **Type**      **Description**
-            settings_parameter_dict    dictionnary   the (pathname,parameter) dictionnary
-            ======================== ============== ======================================
-
-            See Also
-            --------
-            update_settings
+        Examples
+        --------
+        If the parameter is of the form ('detector_settings', 'xxx') then the parameter is sent to the instrument
+        plugin class.
         """
 
         path = settings_parameter_dict['path']
         param = settings_parameter_dict['param']
         if path[0] == 'main_settings':
             if hasattr(self, path[-1]):
                 setattr(self, path[-1], param.value())
 
         elif path[0] == 'detector_settings':
             self.detector.update_settings(settings_parameter_dict)
 
-    @Slot(ThreadCommand)
     def queue_command(self, command: ThreadCommand):
         """Transfer command from the main module to the hardware module
 
         Parameters
         ----------
         command: ThreadCommand
             The specific (or generic) command (str) to pass to the hardware,  either:
@@ -1288,15 +1181,14 @@
             * close
             * grab
             * single
             * stop_grab
             * stop_all
             * update_scanner
             * move_at_navigator
-            * update_com
             * update_wait_time
             * get_axis
             * any string that the hardware is able to understand
         """
         if command.command == "ini_detector":
             status = self.ini_detector(*command.attribute)
             self.status_sig.emit(ThreadCommand(command.command, [status, 'log']))
@@ -1327,184 +1219,142 @@
 
         elif command.command == 'update_scanner':
             self.detector.update_scanner(command.attribute[0])
 
         elif command.command == 'move_at_navigator':
             self.detector.move_at_navigator(*command.attribute)
 
-        elif command.command == 'update_com':
-            self.detector.update_com()
-
         elif command.command == 'update_wait_time':
             self.wait_time = command.attribute[0]
 
         elif command.command == 'get_axis':
             self.detector.get_axis()
 
-        else:  # custom commands for particular plugins (see ROISelect in relation to a Viewer2D and the plugin
-            # Mock2D or the spectrometer module 'get_spectro_wl' for instance)
+        else:  # custom commands for particular plugins
             if hasattr(self.detector, command.command):
                 cmd = getattr(self.detector, command.command)
                 cmd(command.attribute)
 
     def ini_detector(self, params_state=None, controller=None):
-        """
-            Init the detector from params_state parameter and DAQ_type class attribute :
-                * in **0D** profile : update the local status and send the "x_axis" Thread command via a status signal
-                * in **1D** profile : update the local status and send the "x_axis" Thread command via a status signal
-                * in **2D** profile : update the local status and send the "x_axis" and the "y_axis" Thread command via a status signal
-
-            =============== =========== ==========================================
-            **Parameters**    **Type**    **Description**
-            *params_state*     ???         the parameter's state of initialization
-            =============== =========== ==========================================
-
-            See Also
-            --------
-            ini_detector, daq_utils.ThreadCommand
+        """ Initialize an instrument plugin class and tries to apply preset settings
+
+        When the instrument is initialized from the Dashboard using a Preset, tries to apply the preset
+        settings to the instrument instance
+
+        Parameters
+        ----------
+        params_state: dict
+        controller: wrapper
         """
         try:
             # status="Not initialized"
             status = edict(initialized=False, info="", x_axis=None, y_axis=None)
             det_params, class_ = get_viewer_plugins(self.daq_type.name, self.detector_name)
-            self.detector = class_(self, params_state)
+            self.detector: DAQ_Viewer_base = class_(self, params_state)
 
             try:
-                self.detector.data_grabed_signal.connect(self.data_ready)
-                self.detector.data_grabed_signal_temp.connect(self.emit_temp_data)
-                infos = self.detector.ini_detector(controller)  # return edict(info="", controller=, stage=)
+                self.detector.dte_signal.connect(self.data_ready)
+                self.detector.dte_signal_temp.connect(self.emit_temp_data)
+                infos = self.detector.ini_detector(controller)
                 status.controller = self.detector.controller
 
             except Exception as e:
                 logger.exception('Hardware couldn\'t be initialized' + str(e))
                 infos = str(e), False
                 status.controller = None
 
             if isinstance(infos, edict):
                 status.update(infos)
             else:
                 status.info = infos[0]
                 status.initialized = infos[1]
 
-
-            if status['x_axis'] is not None:
-                x_axis = status['x_axis']
-                self.status_sig.emit(ThreadCommand("x_axis", [x_axis]))
-            if status['y_axis'] is not None:
-                y_axis = status['y_axis']
-                self.status_sig.emit(ThreadCommand("y_axis", [y_axis]))
-
-            self.hardware_averaging = class_.hardware_averaging  # to check if averaging can be done directly by the hardware or done here software wise
+            self.hardware_averaging = class_.hardware_averaging  # to check if averaging can be done directly by
+            # the hardware or done here software wise
 
             return status
         except Exception as e:
             self.logger.exception(str(e))
             return status
 
-    @Slot(list)
-    def emit_temp_data(self, datas):
-        self.data_detector_temp_sig.emit(datas)
+    def emit_temp_data(self, data: DataToExport):
+        """ Convenience method to export temporary data using the data_detector_temp_sig Signal
 
-    @Slot(list)
-    def data_ready(self, datas):
+        Parameters
+        ----------
+        data: DataToExport
         """
-            | Update the local datas attribute from the given datas parameter if the averaging has to be done software wise.
-            |
-            | Else emit the data detector signals with datas parameter as an attribute.
-
-            =============== ===================== =========================
-            **Parameters**    **Type**             **Description**
-            *datas*           list                the datas to be emitted.
-            =============== ===================== =========================
+        self.data_detector_temp_sig.emit(data)
 
-            See Also
-            --------
-            daq_utils.ThreadCommand
-        """
+    def data_ready(self, data: DataToExport):
+        """ Process the data received from the instrument plugin class
 
-        # datas validation check for backcompatibility with plugins not exporting new DataFromPlugins list of objects
+        Processing here is eventual software averaging if it was not possible in the instrument plugin class
 
-        for dat in datas:
-            if not isinstance(dat, DataFromPlugins):
-                if 'type' in dat:
-                    dat['dim'] = dat['type']
-                    dat['type'] = 'raw'
+        Parameters
+        ----------
+        data: DataToExport
+        """
+        do_averaging = self.Naverage > 1 and not self.hardware_averaging
 
-        if not self.hardware_averaging:  # to execute if the averaging has to be done software wise
+        if do_averaging:  # to execute if the averaging has to be done software wise
             self.ind_average += 1
             if self.ind_average == 1:
-                self.datas = datas
+                self.datas = data.deepcopy()
             else:
-                try:
-                    for indpannel, dic in enumerate(datas):
-                        self.datas[indpannel]['data'] = \
-                            [((self.ind_average - 1) * self.datas[indpannel]['data'][ind] + datas[indpannel]['data'][
-                                ind]) / self.ind_average for ind in range(len(datas[indpannel]['data']))]
+                self.datas = data.average(self.datas, self.ind_average)
 
-                    if self.show_averaging:
-                        self.emit_temp_data(self.datas)
-
-                except Exception as e:
-                    self.logger.exception(str(e))
+            if self.show_averaging:
+                self.emit_temp_data(self.datas)
 
             if self.ind_average == self.Naverage:
                 self.average_done = True
                 self.data_detector_sig.emit(self.datas)
                 self.ind_average = 0
         else:
-            self.data_detector_sig.emit(datas)
+            self.average_done = True  # expected to make sure the single_grab stop by itself
+            self.data_detector_sig.emit(data)
         self.waiting_for_data = False
         if not self.grab_state:
-            # self.status_sig.emit(["Update_Status","Grabing braked"])
             self.detector.stop()
 
-    def single(self, Naverage=1, args_as_dict={}):
-        """
-            Call the grab method with Naverage parameter as an attribute.
+    def single(self, Naverage=1, **kwargs):
+        """ Convenience function to grab a single set of data
 
-            =============== =========== ==================
-            **Parameters**    **Type**    **Description**
-            *Naverage*        int
-            *savepath*           str        eventual savepath
-            =============== =========== ==================
-
-            See Also
-            --------
-            daq_utils.ThreadCommand, grab
+        Parameters
+        ----------
+        Naverage: int
+            The number of data to average before displaying
+        kwargs: optional named arguments
         """
-        try:
-            self.grab_data(Naverage, live=False, **args_as_dict)
-
-        except Exception as e:
-            self.logger.exception(str(e))
+        self.grab_data(Naverage, live=False, **kwargs)
 
     def grab_data(self, Naverage=1, live=True, **kwargs):
-        """
-            | Update status with 'Start Grabing' Update_status sub command of the Thread command.
-            | Process events and grab naverage is needed.
+        """ General method to grab data from the instrument plugin class
+
+        Will check if the plugin class can do hardware averaging (if NAverage > 1) and and live_mode, otherwise
+        do both software wise here
 
-            =============== =========== ==================
-            **Parameters**    **Type**    **Description**
-            *Naverage*        int
-            =============== =========== ==================
-
-            See Also
-            --------
-            daq_utils.ThreadCommand, grab
+        Parameters
+        ----------
+        Naverage: int
+            The number of data to average
+        live: bool
+            Try to run the instrument plugin class grabbing in live mode
+        kwargs: optional named arguments passed to the grab_data method of the instrument plugin class
         """
         try:
             self.ind_average = 0
             self.Naverage = Naverage
             if Naverage > 1:
                 self.average_done = False
-            # self.status_sig.emit(ThreadCommand("Update_Status", [f'Start Grabing']))
             self.waiting_for_data = False
 
             # for live mode:two possibilities: either snap one data and regrab softwarewise (while True) or if
-            # self.detector.live_mode_available is True all data is continuously emited from the plugin
+            # self.detector.live_mode_available is True all data is continuously emitted from the plugin
             if self.detector.live_mode_available:
                 kwargs['wait_time'] = self.wait_time
             else:
                 kwargs['wait_time'] = 0
             self.status_sig.emit(ThreadCommand('grab'))
             while True:
                 try:
@@ -1515,48 +1365,55 @@
                     if self.single_grab:
                         if self.hardware_averaging:
                             break
                         else:
                             if self.average_done:
                                 break
                     else:
-                        QThread.msleep(self.wait_time) #if in live mode apply a waiting time after acquisition
+                        QThread.msleep(self.wait_time)  # if in grab mode apply a waiting time after acquisition
                     if not self.grab_state:
-                        break
+                        break   # if not in grab mode  breaks the while loop
                     if self.detector.live_mode_available:
-                        break
+                        break  # if live can be done in the plugin breaks the while loop
                 except Exception as e:
                     self.logger.exception(str(e))
             self.status_sig.emit(ThreadCommand('grab_stopped'))
 
         except Exception as e:
             self.logger.exception(str(e))
 
     def close(self):
+        """ Call the close method of the instrument plugin class
         """
-            close the current instance of DAQ_Detector.
-        """
-        try:
-            self.detector.stop()
-            status = self.detector.close()
-        except Exception as e:
-            self.logger.exception(str(e))
-            status = str(e)
+        status = self.detector.close()
         return status
 
 
 def prepare_docks(area, title):
+    """ Static method to init docks to be used within a DAQ_Viewer
+
+    Parameters
+    ----------
+    area
+    title
+
+    Returns
+    -------
+
+    """
     dock_settings = Dock(title + " settings", size=(150, 250))
     dock_viewer = Dock(title + " viewer", size=(350, 350))
     area.addDock(dock_settings)
     area.addDock(dock_viewer, 'right', dock_settings)
     return dict(dock_settings=dock_settings, dock_viewer=dock_viewer)
 
 
 def main(init_qt=True, init_det=False):
+    """ Method called to start the DAQ_Viewer in standalone mode"""
+
     if init_qt:  # used for the test suite
         app = QtWidgets.QApplication(sys.argv)
         if config('style', 'darkstyle'):
             import qdarkstyle
             app.setStyleSheet(qdarkstyle.load_stylesheet(qdarkstyle.DarkPalette))
 
     win = QtWidgets.QMainWindow()
```

### Comparing `pymodaq-4.0.2/src/pymodaq/control_modules/daq_viewer_ui.py` & `pymodaq-4.0.3/src/pymodaq/control_modules/daq_viewer_ui.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/control_modules/mocks.py` & `pymodaq-4.0.3/src/pymodaq/control_modules/mocks.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/control_modules/move_utility_classes.py` & `pymodaq-4.0.3/src/pymodaq/control_modules/move_utility_classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,22 +69,28 @@
     is_multiaxes: bool
         If True, display the particular settings to define which axis the controller is driving
     axes_names: list of str
         The string identifier of every axis the controller can drive
     master: bool
         If True consider this plugin has to init the controller, otherwise use an already initialized instance
     """
-    params = [{'title': 'MultiAxes:', 'name': 'multiaxes', 'type': 'group', 'visible': is_multiaxes, 'children': [
-        {'title': 'is Multiaxes:', 'name': 'ismultiaxes', 'type': 'bool', 'value': is_multiaxes,
-         'default': False},
-        {'title': 'Status:', 'name': 'multi_status', 'type': 'list', 'value': 'Master' if master else 'Slave',
-         'limits': ['Master', 'Slave']},
-        {'title': 'Axis:', 'name': 'axis', 'type': 'list', 'limits': axes_names},
-
-    ]}] + comon_parameters(epsilon)
+    params = [
+                 {'title': 'MultiAxes:', 'name': 'multiaxes', 'type': 'group', 'visible': is_multiaxes, 'children': [
+                     {'title': 'is Multiaxes:', 'name': 'ismultiaxes', 'type': 'bool', 'value': is_multiaxes,
+                      'default': False},
+                     {'title': 'Status:', 'name': 'multi_status', 'type': 'list',
+                      'value': 'Master' if master else 'Slave', 'limits': ['Master', 'Slave']},
+                     {'title': 'Axis:', 'name': 'axis', 'type': 'list', 'limits': axes_names},
+                 ]},
+                 {'title': 'Grouping', 'name': 'grouping', 'type': 'group', 'visible': is_multiaxes, 'children': [
+                     {'title': 'Axes', 'name': 'grouped_axes', 'type': 'itemselect',
+                      'value': dict(all_items=axes_names, selected=[])},
+                     {'title': 'Do group', 'name': 'do_group', 'type': 'bool'},
+                 ]}
+             ] + comon_parameters(epsilon)
     return params
 
 
 params = [
     {'title': 'Main Settings:', 'name': 'main_settings', 'type': 'group', 'children': [
         {'title': 'Actuator type:', 'name': 'move_type', 'type': 'str', 'value': '', 'readonly': True},
         {'title': 'Actuator name:', 'name': 'module_name', 'type': 'str', 'value': '', 'readonly': True},
@@ -318,15 +324,15 @@
     def move_home(self, value):
         if hasattr(self, 'move_Home'):
             deprecation_msg('move_Home method in plugins is deprecated, use move_home', 3)
             self.move_Home()
         else:
             raise NotImplementedError
 
-    def emit_status(self, status):
+    def emit_status(self, status: ThreadCommand):
         """
             | Emit the statut signal from the given status parameter.
             |
             | The signal is sended to the gui to update the user interface.
 
             =============== ===================== ========================================================================================================================================
             **Parameters**   **Type**              **Description**
```

### Comparing `pymodaq-4.0.2/src/pymodaq/control_modules/utils.py` & `pymodaq-4.0.3/src/pymodaq/extensions/pid/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,265 +1,223 @@
-# -*- coding: utf-8 -*-
-"""
-Created the 03/10/2022
-
-@author: Sebastien Weber
-"""
-from easydict import EasyDict as edict
-
-from qtpy import QtCore
-from qtpy.QtCore import Signal, QObject
-from pymodaq.utils.gui_utils import CustomApp
-from pymodaq.utils.daq_utils import ThreadCommand, get_plugins, find_dict_in_list_from_key_val
-from pymodaq.utils.config import Config
-from pymodaq.utils.parameter import Parameter
-from pymodaq.utils.enums import BaseEnum, enum_checker
-from pymodaq.utils.plotting.data_viewers.viewer import ViewersEnum
-
-
-class DAQTypesEnum(BaseEnum):
-    """enum relating a given DAQType and a viewer type
-    See Also
-    --------
-    pymodaq.utils.plotting.data_viewers.viewer.ViewersEnum
-    """
-    DAQ0D = 'Viewer0D'
-    DAQ1D = 'Viewer1D'
-    DAQ2D = 'Viewer2D'
-    DAQND = 'ViewerND'
-
-    def to_data_type(self):
-        return ViewersEnum[self.value].value
-
-    def to_viewer_type(self):
-        return self.value
-
-    def to_daq_type(self):
-        return self.name
-
-    def increase_dim(self, ndim: int):
-        dim = self.get_dim()
-        if dim != 'N':
-            dim_as_int = int(dim) + ndim
-            if dim_as_int > 2:
-                dim = 'N'
-            else:
-                dim = str(dim_as_int)
-        else:
-            dim = 'N'
-        return DAQTypesEnum(f'Viewer{dim}D')
-
-    def get_dim(self):
-        return self.value.split('Viewer')[1].split('D')[0]
-
-DAQ_TYPES = DAQTypesEnum
-
-DET_TYPES = {'DAQ0D': get_plugins('daq_0Dviewer'),
-             'DAQ1D': get_plugins('daq_1Dviewer'),
-             'DAQ2D': get_plugins('daq_2Dviewer'),
-             'DAQND': get_plugins('daq_NDviewer'),}
-
-
-config = Config()
-
-
-class ViewerError(Exception):
-    pass
-
-
-def get_viewer_plugins(daq_type, det_name):
-    parent_module = find_dict_in_list_from_key_val(DET_TYPES[daq_type], 'name', det_name)
-    match_name = daq_type.lower()
-    match_name = f'{match_name[0:3]}_{match_name[3:].upper()}viewer_'
-    obj = getattr(getattr(parent_module['module'], match_name + det_name),
-                  f'{match_name[0:7].upper()}{match_name[7:]}{det_name}')
-    params = getattr(obj, 'params')
-    det_params = Parameter.create(name='Det Settings', type='group', children=params)
-    return det_params, obj
-
-
-class ControlModule(QObject):
-    """Abstract Base class common to both DAQ_Move and DAQ_Viewer control modules
-
-    Attributes
-    ----------
-    init_signal : Signal[bool]
-        This signal is emitted when the chosen hardware is correctly initialized
-    command_hardware : Signal[ThreadCommand]
-        This signal is used to communicate with the instrument plugin within a separate thread
-    command_tcpip : Signal[ThreadCommand]
-        This signal is used to communicate through the TCP/IP Network
-    quit_signal : Signal[]
-        This signal is emitted when the user requested to stop the module
-    """
-    init_signal = Signal(bool)
-    command_hardware = Signal(ThreadCommand)
-    _command_tcpip = Signal(ThreadCommand)
-    quit_signal = Signal()
-    _update_settings_signal = Signal(edict)
-    status_sig = Signal(str)
+import importlib
+import inspect
+import pkgutil
+from importlib import metadata
+from pathlib import Path
+
+from pymodaq.utils.gui_utils.dock import DockArea
+from pymodaq.utils.daq_utils import get_plugins
+from pymodaq.utils.logger import get_module_name, set_logger
+from pymodaq.utils.daq_utils import find_dict_in_list_from_key_val
+
+logger = set_logger(get_module_name(__file__))
+
+DAQ_Move_Stage_type = get_plugins('daq_move')
+DAQ_0DViewer_Det_types = get_plugins('daq_0Dviewer')
+DAQ_1DViewer_Det_types = get_plugins('daq_1Dviewer')
+DAQ_2DViewer_Det_types = get_plugins('daq_2Dviewer')
+DAQ_NDViewer_Det_types = get_plugins('daq_NDviewer')
+
 
-    def __init__(self):
+class InputFromDetector:
+    def __init__(self, values=[]):
         super().__init__()
-        self._title = ""
 
-        # the hardware controller instance set after initialization and to be used by other modules if they share the
-        # same controller
-        self.controller = None
-        self._initialized_state = False
-        self._send_to_tcpip = False
-        self._tcpclient_thread = None
-        self._hardware_thread = None
-        self.module_and_data_saver = None
+        self.values = values
 
     def __repr__(self):
-        return f'{self.__class__.__name__}: {self.title}'
+        return f'Inputs with current values: {self.values}'
 
-    @property
-    def module_type(self):
-        """str: Get the module type, either DAQ_Move or DAQ_viewer"""
-        return type(self).__name__
-
-    @property
-    def initialized_state(self):
-        """bool: Check if the module is initialized"""
-        return self._initialized_state
-
-    @property
-    def title(self):
-        """str: get the title of the module"""
-        return self._title
-
-    def grab(self):
-        """Programmatic entry to grab data from detectors or current value from actuator"""
-        raise NotImplementedError
 
-    def stop_grab(self):
-        """Programmatic entry to stop data grabbing from detectors or current value polling from actuator"""
-        raise NotImplementedError
+class OutputToActuator:
+    def __init__(self, mode='rel', values=[]):
+        super().__init__()
+        if mode not in ['abs', 'rel']:
+            raise ValueError(f'Incorrect mode for the OutputToActuator object: {mode}')
 
-    def _add_data_to_saver(self, *args, **kwargs):
-        raise NotImplementedError
+        self.mode = mode
+        self.values = values
 
-    def append_data(self, *args, **kwargs):
-        raise NotImplementedError
-
-    def insert_data(self, *args, **kwargs):
-        raise NotImplementedError
+    def __repr__(self):
+        return f'Output in {self.mode} mode with current values: {self.values}'
 
-    def quit_fun(self):
-        """Programmatic entry to quit the controle module"""
-        raise NotImplementedError
 
-    def init_hardware(self, do_init=True):
-        """Programmatic entry to initialize/deinitialize the control module
+class PIDModelGeneric:
+    limits = dict(max=dict(state=False, value=1),
+                  min=dict(state=False, value=0),)
+    konstants = dict(kp=1, ki=0.1, kd=0.001)
+    params = []
+
+    Nsetpoints = 1
+    setpoint_ini = [0. for ind in range(Nsetpoints)]
+    setpoints_names = ['' for ind in range(Nsetpoints)]
+
+    actuators_name = []
+    detectors_name = []
+
+    epsilon = 1
+
+    def __init__(self, pid_controller):
+        self.pid_controller = pid_controller  # instance of the pid_controller using this model
+        self.modules_manager = pid_controller.modules_manager
+
+        self.settings = self.pid_controller.settings.child('models', 'model_params')  # set of parameters
+        self.data_names = None
+        self.curr_output = [0. for ind in range(self.Nsetpoints)]
+        self.curr_input = None
+
+        self.check_modules(self.modules_manager)
+
+    def setpoint(self, values):
+        self.pid_controller.setpoints = values
+
+    def apply_constants(self):
+        for kxx in self.konstants:
+            self.pid_controller.settings.child('main_settings', 'pid_controls', 'pid_constants',
+                                               kxx).setValue(self.konstants[kxx])
+
+    def apply_limits(self):
+        for limit in self.limits:
+            self.pid_controller.settings.child('main_settings', 'pid_controls', 'output_limits',
+                                               f'output_limit_{limit}').setValue(self.limits[limit]['value'])
+            self.pid_controller.settings.child('main_settings', 'pid_controls', 'output_limits',
+                                               f'output_limit_{limit}_enabled').setValue(self.limits[limit]['state'])
+
+    def check_modules(self, modules_manager):
+        for act in self.actuators_name:
+            if act not in modules_manager.actuators_name:
+                logger.warning(f'The actuator {act} defined in the PID model is not present in the Dashboard')
+                return False
+        for det in self.detectors_name:
+            if det not in modules_manager.detectors_name:
+                logger.warning(f'The detector {det} defined in the PID model is not present in the Dashboard')
+
+    def update_detector_names(self):
+        names = self.pid_controller.settings.child('main_settings', 'detector_modules').value()['selected']
+        self.data_names = []
+        for name in names:
+            name = name.split('//')
+            self.data_names.append(name)
 
-        Parameters
-        ----------
-        do_init : bool
-            if True initialize the selected hardware else deinitialize it
 
-        See Also
-        --------
-        :meth:`init_hardware_ui`
+    def update_settings(self, param):
         """
-        raise NotImplementedError
+        Get a parameter instance whose value has been modified by a user on the UI
+        To be overwritten in child class
+        """
+        if param.name() == '':
+            pass
 
-    def init_hardware_ui(self, do_init=True):
-        """Programmatic entry to simulate a click on the user interface init button
+    def ini_model(self):
+        self.apply_limits()
+        self.setpoint(self.setpoint_ini)
+        self.apply_constants()
 
+    def convert_input(self, measurements):
+        """
+        Convert the measurements in the units to be fed to the PID (same dimensionality as the setpoint)
         Parameters
         ----------
-        do_init : bool
-            if True initialize the selected hardware else deinitialize it
+        measurements: (Ordereddict) Ordereded dict of object from which the model extract a value of the same units as the setpoint
+
+        Returns
+        -------
+        float: the converted input
 
-        Notes
-        -----
-        This method should be preferred to :meth:`init_hardware`
         """
         raise NotImplementedError
 
-    def show_log(self):
-        """Open the log file in the default text editor"""
-        import webbrowser
-        webbrowser.open(self.logger.parent.handlers[0].baseFilename)
-
-    def update_status(self, txt, log=True):
-        """Display a message in the ui status bar and eventually log the message
-
+    def convert_output(self, outputs, dt, stab=True):
+        """
+        Convert the output of the PID in units to be fed into the actuator
         Parameters
         ----------
-        txt : str
-            message to display
-        log : bool
-            if True, log the message in the logger
+        outputs: (list of float) output value from the PID from which the model extract a value of the same units as the actuator
+        dt: (float) elapsed time in seconds since last call
+        Returns
+        -------
+        OutputToActuator: the converted output as an OutputToActuator object
+
         """
-        if self.ui is not None:
-            self.ui.display_status(txt)
-        self.status_sig.emit(txt)
-        if log:
-            self.logger.info(txt)
+        self.curr_output = outputs
+        return OutputToActuator(mode='rel', values=outputs)
 
-    def manage_ui_actions(self, action_name: str, attribute: str, value):
-        """Method to manage actions for the UI (if any).
 
-        Will try to apply the given value to the given attribute of the corresponding action
+def main(xmlfile):
+    from pymodaq.dashboard import DashBoard
+    from pymodaq.utils.config import get_set_preset_path
+    from pathlib import Path
+    from qtpy import QtWidgets
+    from extensions.pid.pid_controller import DAQ_PID
+
+    import sys
+    app = QtWidgets.QApplication(sys.argv)
+    win = QtWidgets.QMainWindow()
+    area = DockArea()
+    win.setCentralWidget(area)
+    win.resize(1000, 500)
+    win.setWindowTitle('PyMoDAQ Dashboard')
+
+    dashboard = DashBoard(area)
+    file = Path(get_set_preset_path()).joinpath(xmlfile)
+    if file.exists():
+        dashboard.set_preset_mode(file)
+        # prog.load_scan_module()
+        pid_area = DockArea()
+        pid_window = QtWidgets.QMainWindow()
+        pid_window.setCentralWidget(pid_area)
+
+        prog = DAQ_PID(pid_area)
+        pid_window.show()
+        pid_window.setWindowTitle('PidController')
+        prog.set_module_manager(dashboard.detector_modules, dashboard.actuators_modules)
+        QtWidgets.QApplication.processEvents()
+
+
+    else:
+        msgBox = QtWidgets.QMessageBox()
+        msgBox.setText(f"The default file specified in the configuration file does not exists!\n"
+                       f"{file}\n"
+                       f"Impossible to load the DAQ_PID Module")
+        msgBox.setStandardButtons(msgBox.Ok)
+        ret = msgBox.exec()
 
-        Parameters
-        ----------
-        action_name: str
-        attribute: method signature or attribute
-        value: object
-            actual type and value depend on the triggered attribute
-
-        Examples
-        --------
-        >>>manage_ui_actions('quit', 'setEnabled', False)
-        # will disable the quit action (button) on the UI
-        """
-        if self.ui is not None:
-            if self.ui.has_action(action_name):
-                action = self.ui.get_action(action_name)
-                if hasattr(action, attribute):
-                    attr = getattr(action, attribute)
-                    if callable(attr):
-                        attr(value)
-                    else:
-                        attr = value
-
-
-class ControlModuleUI(CustomApp):
-    """ Base Class for ControlModules UIs
-
-    Attributes
-    ----------
-    command_sig: Signal[Threadcommand]
-        This signal is emitted whenever some actions done by the user has to be
-        applied on the main module. Possible commands are:
-        See specific implementation
-
-    See Also
-    --------
-    :class:`daq_move_ui.DAQ_Move_UI`, :class:`daq_viewer_ui.DAQ_Viewer_UI`
-    """
-    command_sig = QtCore.Signal(ThreadCommand)
+    sys.exit(app.exec_())
 
-    def __init__(self, parent):
-        super().__init__(parent)
 
-    def display_status(self, txt, wait_time=config('general', 'message_status_persistence')):
-        if self.statusbar is not None:
-            self.statusbar.showMessage(txt, wait_time)
-
-    def do_init(self, do_init=True):
-        """Programmatically press the Init button
-        API entry
-        Parameters
-        ----------
-        do_init: bool
-            will fire the Init button depending on the argument value and the button check state
-        """
-        raise NotImplementedError
+def get_models(model_name=None):
+    """
+    Get PID Models as a list to instantiate Control Actuators per degree of liberty in the model
 
-    def send_init(self):
-        """Shoudl be implemented to send to the main app the fact that someone pressed init"""
-        raise NotImplementedError
+    Returns
+    -------
+    list: list of disct containting the name and python module of the found models
+    """
+    from pymodaq.extensions.pid.utils import PIDModelGeneric
+    models_import = []
+    entry_points = metadata.entry_points()
+    if 'pymodaq.pid_models' in entry_points:
+        discovered_models = entry_points['pymodaq.pid_models']
+        for pkg in discovered_models:
+            try:
+                module = importlib.import_module(pkg.value)
+                module_name = pkg.value
+
+                for mod in pkgutil.iter_modules([str(Path(module.__file__).parent.joinpath('models'))]):
+                    try:
+                        model_module = importlib.import_module(f'{module_name}.models.{mod.name}', module)
+                        classes = inspect.getmembers(model_module, inspect.isclass)
+                        for name, klass in classes:
+                            if klass.__base__ is PIDModelGeneric:
+                                models_import.append({'name': mod.name, 'module': model_module, 'class': klass})
+                                break
+
+                    except Exception as e:  # pragma: no cover
+                        logger.warning(str(e))
+
+            except Exception as e:  # pragma: no cover
+                logger.warning(f'Impossible to import the {pkg.value} extension: {str(e)}')
+
+    if model_name is None:
+        return models_import
+    else:
+        return find_dict_in_list_from_key_val(models_import, 'name', model_name)
```

### Comparing `pymodaq-4.0.2/src/pymodaq/control_modules/viewer_utility_classes.py` & `pymodaq-4.0.3/src/pymodaq/control_modules/viewer_utility_classes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,24 @@
+from typing import Union
 from qtpy import QtWidgets
 from qtpy.QtCore import QObject, Slot, Signal
 
 from pymodaq.utils.parameter import ioxml
 from pymodaq.utils.parameter.utils import get_param_path, get_param_from_name, iter_children
 from pyqtgraph.parametertree import Parameter
 from easydict import EasyDict as edict
 
 import numpy as np
 from pymodaq.utils.math_utils import gauss1D, gauss2D
 from pymodaq.utils.daq_utils import ThreadCommand, getLineInfo
 from pymodaq.utils.config import Config, get_set_local_dir
-#from pymodaq.utils.scanner import ScanParameters
 from pymodaq.utils.tcp_server_client import TCPServer, tcp_parameters
+from pymodaq.utils.data import DataToExport
+from pymodaq.utils.messenger import deprecation_msg
+
 
 comon_parameters = [{'title': 'Controller Status:', 'name': 'controller_status', 'type': 'list', 'value': 'Master',
                      'limits': ['Master', 'Slave']}, ]
 
 local_path = get_set_local_dir()
 # look for eventual calibration files
 calibs = ['None']
@@ -29,15 +32,14 @@
 
 params = [
     {'title': 'Main Settings:', 'name': 'main_settings', 'expanded': False, 'type': 'group', 'children': [
         {'title': 'DAQ type:', 'name': 'DAQ_type', 'type': 'list', 'limits': ['DAQ0D', 'DAQ1D', 'DAQ2D', 'DAQND'],
          'readonly': True},
         {'title': 'Detector type:', 'name': 'detector_type', 'type': 'str', 'value': '', 'readonly': True},
         {'title': 'Detector Name:', 'name': 'module_name', 'type': 'str', 'value': '', 'readonly': True},
-        {'title': 'Nviewers:', 'name': 'Nviewers', 'type': 'int', 'value': 1, 'min': 1, 'default': 1, 'readonly': True},
         {'title': 'Controller ID:', 'name': 'controller_ID', 'type': 'int', 'value': 0, 'default': 0, 'readonly': False},
         {'title': 'Show data and process:', 'name': 'show_data', 'type': 'bool', 'value': True, },
         {'title': 'Refresh time (ms):', 'name': 'refresh_time', 'type': 'float', 'value': 50., 'min': 0.},
         {'title': 'Naverage', 'name': 'Naverage', 'type': 'int', 'default': 1, 'value': 1, 'min': 1},
         {'title': 'Show averaging:', 'name': 'show_averaging', 'type': 'bool', 'default': False, 'value': False},
         {'title': 'Live averaging:', 'name': 'live_averaging', 'type': 'bool', 'default': False, 'value': False},
         {'title': 'N Live aver.:', 'name': 'N_live_averaging', 'type': 'int', 'default': 0, 'value': 0,
@@ -107,15 +109,15 @@
         detector = Path(plugin_file).stem[13:]
         det_type = f'DAQ{Path(plugin_file).stem[4:6].upper()}'
     prog = DAQ_Viewer(area, title="Testing")
     win.show()
     prog.daq_type = det_type
     prog.detector = detector
     if init:
-        prog.init_det()
+        prog.init_hardware()
 
     sys.exit(app.exec_())
 
 
 class DAQ_Viewer_base(QObject):
     """
         ===================== ===================================
@@ -130,22 +132,26 @@
 
         See Also
         --------
         send_param_status
     """
     hardware_averaging = False
     live_mode_available = False
-    data_grabed_signal = Signal(list)
-    data_grabed_signal_temp = Signal(list)
+    data_grabed_signal = Signal(list)  # will be deprecated use dte_signal
+    data_grabed_signal_temp = Signal(list)  # will be deprecated use dte_signal_temp
+    dte_signal = Signal(DataToExport)
+    dte_signal_temp = Signal(DataToExport)
 
     params = []
 
     def __init__(self, parent=None, params_state=None):
-        QObject.__init__(self)
-        self.parent_parameters_path = []  # this is to be added in the send_param_status to take into account when the current class instance parameter list is a child of some other class
+        super().__init__()
+
+        self.parent_parameters_path = []  # this is to be added in the send_param_status to take into account when
+        # the current class instance parameter list is a child of some other class
         self.settings = Parameter.create(name='Settings', type='group', children=self.params)
         if params_state is not None:
             if isinstance(params_state, dict):
                 self.settings.restoreState(params_state)
             elif isinstance(params_state, Parameter):
                 self.settings.restoreState(params_state.saveState())
 
@@ -163,14 +169,33 @@
         self.scan_parameters = None
 
         self.x_axis = None
         self.y_axis = None
 
         self.ini_attributes()
 
+        self.data_grabed_signal.connect(self._emit_dte)
+        self.data_grabed_signal_temp.connect(self._emit_dte_temp)
+
+    def _emit_dte(self, dte: Union[DataToExport, list]):
+        if isinstance(dte, list):
+            deprecation_msg(f'Data emitted from the instrument plugins should be a DataToExport instance'
+                            f'See: http://pymodaq.cnrs.fr/en/latest/developer_folder/'
+                            f'instrument_plugins.html#emission-of-data')
+            dte = DataToExport('temp', dte)
+        self.dte_signal.emit(dte)
+
+    def _emit_dte_temp(self, dte: Union[DataToExport, list]):
+        if isinstance(dte, list):
+            deprecation_msg(f'Data emitted from the instrument plugins should be a DataToExport instance'
+                            f'See: http://pymodaq.cnrs.fr/en/latest/developer_folder/'
+                            f'instrument_plugins.html#emission-of-data')
+            dte = DataToExport('temp', dte)
+        self.dte_signal_temp.emit(dte)
+
     def ini_attributes(self):
         """
         To be reimplemented in subclass
         """
         pass
 
     def ini_detector_init(self, old_controller=None, new_controller=None):
@@ -232,31 +257,22 @@
 
     def commit_settings(self, param):
         """
         To be reimplemented in subclass
         """
         pass
 
-    def update_com(self):
-        """
-        If some communications settings have to be re init
-        To be reimplemented in subclass
-        -------
-
-        """
-        pass
-
     def get_axis(self):
         if self.plugin_type == '1D' or self.plugin_type == '2D':
             self.emit_x_axis()
 
         if self.plugin_type == '2D':
             self.emit_y_axis()
 
-    def emit_status(self, status):
+    def emit_status(self, status: ThreadCommand):
         """
             Emit the status signal from the given status.
 
             =============== ============ =====================================
             **Parameters**    **Type**     **Description**
             *status*                       the status information to transmit
             =============== ============ =====================================
@@ -345,36 +361,14 @@
                 self.emit_status(ThreadCommand('update_settings', [self.parent_parameters_path + path, data,
                                                                    change]))  # send parameters values/limits back to the GUI
             elif change == 'parent':
                 pass
 
             pass
 
-    def emit_x_axis(self, x_axis=None):
-        """
-            Convenience function
-            Emit the thread command "x_axis" with x_axis as an attribute.
-
-            See Also
-            --------
-            daq_utils.ThreadCommand
-        """
-        if x_axis is None:
-            x_axis = self.x_axis
-        self.emit_status(ThreadCommand("x_axis", [x_axis]))
-
-    def emit_y_axis(self):
-        """
-            Emit the thread command "y_axis" with y_axis as an attribute.
-
-            See Also
-            --------
-            daq_utils.ThreadCommand
-        """
-        self.emit_status(ThreadCommand("y_axis", [self.y_axis]))
 
 
 class DAQ_Viewer_TCP_server(DAQ_Viewer_base, TCPServer):
     """
         ================= ==============================
         **Attributes**      **Type**
         *command_server*    instance of Signal
@@ -522,17 +516,15 @@
             sock = self.find_socket_within_connected_clients(self.client_type)
             if sock is not None:  # if client self.client_type is connected then send it the command
                 data = self.read_data(sock)
             else:
                 data = self.data_mock
 
             if command_sock is None:
-                # self.data_grabed_signal.emit([OrderedDict(data=[data],name='TCP GRABBER', type='Data2D')]) #to be directly send to a viewer
                 self.data_ready(data)
-                # print(data)
             else:
                 self.send_data(command_sock, data)  # to be send to a client
 
         except Exception as e:
             self.emit_status(ThreadCommand("Update_Status", [str(e), 'log']))
 
     def commit_settings(self, param):
```

### Comparing `pymodaq-4.0.2/src/pymodaq/examples/custom_app.py` & `pymodaq-4.0.3/src/pymodaq/examples/custom_app.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/examples/custom_viewer.py` & `pymodaq-4.0.3/src/pymodaq/examples/custom_viewer.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/examples/function_plotter.py` & `pymodaq-4.0.3/src/pymodaq/examples/function_plotter.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/examples/nonlinearscanner.py` & `pymodaq-4.0.3/src/pymodaq/examples/nonlinearscanner.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/examples/parameter_ex.py` & `pymodaq-4.0.3/src/pymodaq/examples/parameter_ex.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/examples/preset_MockCamera.xml` & `pymodaq-4.0.3/src/pymodaq/examples/preset_MockCamera.xml`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Client.lvproj` & `pymodaq-4.0.3/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Client.lvproj`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Client.vi` & `pymodaq-4.0.3/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Client.vi`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Server_1Dgaussian.vi` & `pymodaq-4.0.3/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Server_1Dgaussian.vi`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Server_2Dgaussian.vi` & `pymodaq-4.0.3/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_Server_2Dgaussian.vi`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_read_cmd.vi` & `pymodaq-4.0.3/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_read_cmd.vi`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_read_float.vi` & `pymodaq-4.0.3/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_read_float.vi`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_read_int.vi` & `pymodaq-4.0.3/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_read_int.vi`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_data.vi` & `pymodaq-4.0.3/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_data.vi`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_int.vi` & `pymodaq-4.0.3/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_int.vi`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_scalar.vi` & `pymodaq-4.0.3/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_scalar.vi`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_string.vi` & `pymodaq-4.0.3/src/pymodaq/examples/Labview_TCP_Client/DAQ_TCP_send_string.vi`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/client_state.ctl` & `pymodaq-4.0.3/src/pymodaq/examples/Labview_TCP_Client/client_state.ctl`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/examples/Labview_TCP_Client/cmd_types.ctl` & `pymodaq-4.0.3/src/pymodaq/examples/Labview_TCP_Client/cmd_types.ctl`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/extensions/console.py` & `pymodaq-4.0.3/src/pymodaq/extensions/console.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/extensions/daq_logger.py` & `pymodaq-4.0.3/src/pymodaq/extensions/daq_logger.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/extensions/daq_scan.py` & `pymodaq-4.0.3/src/pymodaq/extensions/daq_scan.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,19 +75,19 @@
             {'title': 'Wait time between (ms)', 'name': 'wait_time_between', 'type': 'int',
              'value': 0,
              'tip': 'Wait time in ms between move and grab processes'},
             {'title': 'Timeout (ms)', 'name': 'timeout', 'type': 'int', 'value': 10000},
         ]},
         {'title': 'Scan options', 'name': 'scan_options', 'type': 'group', 'children': [
             {'title': 'Naverage:', 'name': 'scan_average', 'type': 'int', 'value': 1, 'min': 1},
-            {'title': 'Group 0D data:', 'name': 'group0D', 'type': 'bool', 'value': True},
             {'title': 'Sort 1D scan data:', 'name': 'sort_scan1D', 'type': 'bool', 'value': False},]},
 
         {'title': 'Plotting options', 'name': 'plot_options', 'type': 'group', 'children': [
-            {'title': 'Get Probe signals', 'name': 'plot_probe', 'type': 'bool_push'},
+            {'title': 'Get data', 'name': 'plot_probe', 'type': 'bool_push'},
+            {'title': 'Group 0D data:', 'name': 'group0D', 'type': 'bool', 'value': True},
             {'title': 'Plot 0Ds:', 'name': 'plot_0d', 'type': 'itemselect'},
             {'title': 'Plot 1Ds:', 'name': 'plot_1d', 'type': 'itemselect'},
             {'title': 'Prepare Viewers', 'name': 'prepare_viewers', 'type': 'bool_push'},
             {'title': 'Plot at each step?', 'name': 'plot_at_each_step', 'type': 'bool', 'value': True},
             {'title': 'Refresh Plots (ms)', 'name': 'refresh_live', 'type': 'int', 'value': 1000, 'visible': False},
             ]},
     ]
@@ -235,15 +235,15 @@
             # self.scanner.scan_selector.widget.setVisible(False)
             # self.scanner.scan_selector.show_scan_selector(visible=False)
             #
             # self.show_average_dock(False)
             #
             # self.ui.scan_dock.setEnabled(True)
             # self.file_menu.setEnabled(True)
-            # self.settings_menu.setEnabled(True)
+            # self._extensions_menu.setEnabled(True)
             # self.create_new_file(True)
 
         except Exception as e:
             logger.exception(str(e))
             # self.update_status(getLineInfo()+str(e), self.wait_time, log_type='log')
 
     def create_average_dock(self):
@@ -558,14 +558,15 @@
                     break
             settings_str += b'</All_settings>'
             attr['settings'] = settings_str
 
     def create_new_file(self, new_file):
         if new_file:
             self._metada_dataset_set = False
+            self.h5saver.close_file()
         self.h5saver.init_file(update_h5=new_file)
         self.module_and_data_saver.h5saver = self.h5saver
         res = self.update_file_settings()
         if new_file:
             self.ui.enable_start_stop()
         return res
 
@@ -650,22 +651,26 @@
         self.settings.child('plot_options', 'plot_0d').setValue(dict(all_items=[], selected=[]))
         self.settings.child('plot_options', 'plot_1d').setValue(dict(all_items=[], selected=[]))
 
     def prepare_viewers(self):
 
         viewers_enum = [ViewersEnum('Data0D').increase_dim(self.scanner.n_axes)
                         for _ in range(len(self.settings['plot_options', 'plot_0d']['selected']))]
-        data_names = self.settings['plot_options', 'plot_0d']['selected']
+        data_names = self.settings['plot_options', 'plot_0d']['selected'][:]
 
-        if self.settings['scan_options', 'group0D'] and len(viewers_enum) > 0 and ViewersEnum('Data1D') in viewers_enum:
+        if self.settings['plot_options', 'group0D'] and len(viewers_enum) > 0 and ViewersEnum('Data1D') in viewers_enum:
             viewers_enum = [ViewersEnum('Data1D')]
-            data_names = [self.live_plotter.grouped_data1D_fullname]
+            data_names = [self.live_plotter.grouped_data0D_fullname]
+        elif self.settings['plot_options', 'group0D'] and len(viewers_enum) > 0 and ViewersEnum('Data2D') in viewers_enum:
+            viewers_enum = [ViewersEnum('Data2D')]
+            data_names = [self.live_plotter.grouped_data0D_fullname]
+
         viewers_enum.extend([ViewersEnum('Data1D').increase_dim(self.scanner.n_axes)
                              for _ in range(len(self.settings['plot_options', 'plot_1d']['selected']))])
-        data_names.extend(self.settings['plot_options', 'plot_1d']['selected'])
+        data_names.extend(self.settings['plot_options', 'plot_1d']['selected'][:])
         self.live_plotter.prepare_viewers(viewers_enum, viewers_name=data_names)
 
     def update_status(self, txt, wait_time=0, log_type=None):
         """
             Show the txt message in the status bar with a delay of wait_time ms.
 
             =============== =========== =======================
@@ -709,15 +714,15 @@
             self.ind_average = status[1][1]
             self.ui.set_scan_step_average(status[1][1] + 1)
 
         elif status[0] == "Scan_done":
             self.modules_manager.reset_signals()
             self.live_timer.stop()
             self.ui.set_scan_done()
-            scan_node = self.module_and_data_saver.get_set_node()
+            scan_node = self.module_and_data_saver.get_last_node()
             scan_node.attrs['scan_done'] = True
             self.save_scan()
             if not self.batch_started:
                 if not self.dashboard.overshoot:
                     self.set_ini_positions()
                 self.ui.set_action_enabled('ini_positions', True)
                 self.ui.set_action_enabled('start', True)
@@ -757,15 +762,15 @@
     def update_live_plots(self):
 
         if self.settings['scan_options', 'scan_average'] > 1:
             average_axis = 0
         else:
             average_axis = None
         try:
-            self.live_plotter.load_plot_data(group_1D=self.settings['scan_options', 'group0D'],
+            self.live_plotter.load_plot_data(group_0D=self.settings['plot_options', 'group0D'],
                                              average_axis=average_axis, average_index=self.ind_average,
                                              target_at=self.scanner.positions[self.ind_scan])
         except Exception as e:
             logger.exception(str(e))
     #################
     #  SCAN FLOW
 
@@ -873,15 +878,15 @@
         if res:
             # deactivate module controls using remote_control
             if hasattr(self.dashboard, 'remote_manager'):
                 remote_manager = getattr(self.dashboard, 'remote_manager')
                 remote_manager.activate_all(False)
 
             self.module_and_data_saver.h5saver = self.h5saver
-            new_scan = self.module_and_data_saver.get_set_node(new=False).attrs['scan_done']
+            new_scan = self.module_and_data_saver.get_last_node().attrs['scan_done'] # get_last_node
             scan_node = self.module_and_data_saver.get_set_node(new=new_scan)
             self.save_metadata(scan_node, 'scan_info')
 
             self._init_live()
 
             # mandatory to deal with multithreads
             if self.scan_thread is not None:
@@ -952,14 +957,16 @@
 
             See Also
             --------
             set_ini_positions
         """
         self.ui.set_permanent_status('Stoping acquisition')
         self.command_daq_signal.emit(utils.ThreadCommand("stop_acquisition"))
+        scan_node = self.module_and_data_saver.get_last_node()
+        scan_node.attrs['scan_done'] = True
 
         if not self.dashboard.overshoot:
             self.set_ini_positions()  # do not set ini position again in case overshoot fired
             status = 'Data Acquisition has been stopped by user'
         else:
             status = 'Data Acquisition has been stopped due to overshoot'
```

### Comparing `pymodaq-4.0.2/src/pymodaq/extensions/daq_scan_ui.py` & `pymodaq-4.0.3/src/pymodaq/extensions/daq_scan_ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,16 @@
         self.add_action('log', 'Show Log file', 'information2', menu=self.file_menu)
 
         self.add_action('load', 'Load File', 'Open', menu=self.file_menu, auto_toolbar=False)
         self.file_menu.addSeparator()
         self.add_action('save', 'Save file as', 'SaveAs', menu=self.file_menu, auto_toolbar=False)
         self.add_action('show_file', 'Show file content', '', menu=self.file_menu, auto_toolbar=False)
 
-        self.add_action('navigator', 'Show Navigator', '', menu=self.settings_menu, auto_toolbar=False)
-        self.add_action('batch', 'Show Batch Scanner', '', menu=self.settings_menu, auto_toolbar=False)
+        self.add_action('navigator', 'Show Navigator', '', menu=self._extensions_menu, auto_toolbar=False)
+        self.add_action('batch', 'Show Batch Scanner', '', menu=self._extensions_menu, auto_toolbar=False)
         self.set_action_visible('start_batch', False)
 
     def enable_start_stop(self, enable=True):
         """If True enable main buttons to launch/stop scan"""
         self.set_action_enabled('start', enable)
         self.set_action_enabled('stop', enable)
 
@@ -81,15 +81,15 @@
         self.connect_action('batch', lambda: self.command_sig.emit(ThreadCommand('batch')))
 
     def setup_menu(self):
         self.menubar = QtWidgets.QMenuBar()
         self.menubar.setMaximumHeight(30)
         self.mainwindow.setMenuBar(self.menubar)
         self.file_menu = self.menubar.addMenu('File')
-        self.settings_menu = self.menubar.addMenu('Settings')
+        self._extensions_menu = self.menubar.addMenu('Extensions')
         self.action_menu = self.menubar.addMenu('Actions')
 
     def setup_docks(self):
         self.dock_command = Dock('Scan Command')
         self.dockarea.addDock(self.dock_command)
 
         widget_command = QtWidgets.QWidget()
```

### Comparing `pymodaq-4.0.2/src/pymodaq/extensions/h5browser.py` & `pymodaq-4.0.3/src/pymodaq/extensions/h5browser.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/extensions/utils.py` & `pymodaq-4.0.3/src/pymodaq/extensions/utils.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/extensions/pid/__init__.py` & `pymodaq-4.0.3/src/pymodaq/extensions/pid/__init__.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/extensions/pid/daq_move_PID.py` & `pymodaq-4.0.3/src/pymodaq/extensions/pid/daq_move_PID.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/extensions/pid/pid_controller.py` & `pymodaq-4.0.3/src/pymodaq/extensions/pid/pid_controller.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/extensions/pid/utils.py` & `pymodaq-4.0.3/src/pymodaq/utils/scanner/scan_factory.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,223 +1,204 @@
-import importlib
-import inspect
-import pkgutil
-from importlib import metadata
-from pathlib import Path
-
-from pymodaq.utils.gui_utils.dock import DockArea
-from pymodaq.utils.daq_utils import get_plugins
-from pymodaq.utils.logger import get_module_name, set_logger
-from pymodaq.utils.daq_utils import find_dict_in_list_from_key_val
+# -*- coding: utf-8 -*-
+"""
+Created the 05/12/2022
+
+@author: Sebastien Weber
+"""
+from __future__ import annotations
+
+from abc import ABCMeta, abstractmethod
+from typing import Callable, Union, List, Tuple, TYPE_CHECKING
+
+
+import numpy as np
+
+from pymodaq.utils.managers.parameter_manager import ParameterManager, Parameter
+from pymodaq.utils.factory import ObjectFactory
+from pymodaq.utils.logger import set_logger, get_module_name
+from pymodaq.utils.data import Axis, DataDistribution
+from pymodaq.utils.abstract import abstract_attribute
+from pymodaq.utils import math_utils as mutils
+from pymodaq.utils import config as configmod
+
+if TYPE_CHECKING:
+    from pymodaq.control_modules.daq_move import DAQ_Move
+    from pymodaq.utils.plotting.scan_selector import Selector
+
 
 logger = set_logger(get_module_name(__file__))
+config = configmod.Config()
 
-DAQ_Move_Stage_type = get_plugins('daq_move')
-DAQ_0DViewer_Det_types = get_plugins('daq_0Dviewer')
-DAQ_1DViewer_Det_types = get_plugins('daq_1Dviewer')
-DAQ_2DViewer_Det_types = get_plugins('daq_2Dviewer')
-DAQ_NDViewer_Det_types = get_plugins('daq_NDviewer')
 
+class ScanParameterManager(ParameterManager):
+    settings_name = 'scanner_settings'
 
-class InputFromDetector:
-    def __init__(self, values=[]):
+    def __init__(self):
         super().__init__()
+        self.settings_tree.header().setVisible(False)
+        self.settings_tree.setMinimumHeight(150)
 
-        self.values = values
 
-    def __repr__(self):
-        return f'Inputs with current values: {self.values}'
+class ScannerBase(ScanParameterManager, metaclass=ABCMeta):
+    """Abstract class for all Scanners
 
+    Attributes
+    ----------
+    params: List[dict]
+        list specifying the scanner set of parameters to properly configure all the scan steps
+    positions: np.ndarray
+        ndarray of all positions. First dimension is number of actuators, second is positions of a given actuator at
+        each step
+    axes_unique: List[np.ndarray]
+        list of ndarrays representing unique values of steps for each actuator in the scan
+    axes_indexes: np.ndarray
+        ndarray of indexes from axes_unique for each value in positions
+    n_steps: int
+        Number of scan steps. Equal to the second dimension of positions
+    n_axes: int
+        Number of actuators/scan axes. Equal to the first dimension of positions
+    """
+    params: List[dict] = abstract_attribute()
+    axes_unique: List[np.ndarray] = abstract_attribute()
+    axes_indexes: np.ndarray = abstract_attribute()
+    n_steps: int = abstract_attribute()
+    n_axes: int = abstract_attribute()
+    distribution: DataDistribution = abstract_attribute()
 
-class OutputToActuator:
-    def __init__(self, mode='rel', values=[]):
+    def __init__(self, actuators: List[DAQ_Move] = None):
         super().__init__()
-        if mode not in ['abs', 'rel']:
-            raise ValueError(f'Incorrect mode for the OutputToActuator object: {mode}')
-
-        self.mode = mode
-        self.values = values
-
-    def __repr__(self):
-        return f'Output in {self.mode} mode with current values: {self.values}'
-
-
-class PIDModelGeneric:
-    limits = dict(max=dict(state=False, value=1),
-                  min=dict(state=False, value=0),)
-    konstants = dict(kp=1, ki=0.1, kd=0.001)
-    params = []
-
-    Nsetpoints = 1
-    setpoint_ini = [0. for ind in range(Nsetpoints)]
-    setpoints_names = ['' for ind in range(Nsetpoints)]
-
-    actuators_name = []
-    detectors_name = []
-
-    epsilon = 1
-
-    def __init__(self, pid_controller):
-        self.pid_controller = pid_controller  # instance of the pid_controller using this model
-        self.modules_manager = pid_controller.modules_manager
-
-        self.settings = self.pid_controller.settings.child('models', 'model_params')  # set of parameters
-        self.data_names = None
-        self.curr_output = [0. for ind in range(self.Nsetpoints)]
-        self.curr_input = None
-
-        self.check_modules(self.modules_manager)
-
-    def setpoint(self, values):
-        self.pid_controller.setpoints = values
-
-    def apply_constants(self):
-        for kxx in self.konstants:
-            self.pid_controller.settings.child('main_settings', 'pid_controls', 'pid_constants',
-                                               kxx).setValue(self.konstants[kxx])
-
-    def apply_limits(self):
-        for limit in self.limits:
-            self.pid_controller.settings.child('main_settings', 'pid_controls', 'output_limits',
-                                               f'output_limit_{limit}').setValue(self.limits[limit]['value'])
-            self.pid_controller.settings.child('main_settings', 'pid_controls', 'output_limits',
-                                               f'output_limit_{limit}_enabled').setValue(self.limits[limit]['state'])
-
-    def check_modules(self, modules_manager):
-        for act in self.actuators_name:
-            if act not in modules_manager.actuators_name:
-                logger.warning(f'The actuator {act} defined in the PID model is not present in the Dashboard')
-                return False
-        for det in self.detectors_name:
-            if det not in modules_manager.detectors_name:
-                logger.warning(f'The detector {det} defined in the PID model is not present in the Dashboard')
-
-    def update_detector_names(self):
-        names = self.pid_controller.settings.child('main_settings', 'detector_modules').value()['selected']
-        self.data_names = []
-        for name in names:
-            name = name.split('//')
-            self.data_names.append(name)
-
-
-    def update_settings(self, param):
-        """
-        Get a parameter instance whose value has been modified by a user on the UI
-        To be overwritten in child class
-        """
-        if param.name() == '':
-            pass
-
-    def ini_model(self):
-        self.apply_limits()
-        self.setpoint(self.setpoint_ini)
-        self.apply_constants()
-
-    def convert_input(self, measurements):
-        """
-        Convert the measurements in the units to be fed to the PID (same dimensionality as the setpoint)
-        Parameters
-        ----------
-        measurements: (Ordereddict) Ordereded dict of object from which the model extract a value of the same units as the setpoint
-
-        Returns
-        -------
-        float: the converted input
+        self.positions: np.ndarray = None
+        self.n_steps = 1
+        self._actuators: List[DAQ_Move] = None
+
+        self.actuators = actuators
+
+        self.set_settings_titles()
+
+        if self.check_steps():
+            self.set_scan()
+
+    def set_settings_titles(self):
+        """Update the settings accordingly with the selected actuators"""
+        ...
+
+    @property
+    def actuators(self):
+        return self._actuators
+
+    @actuators.setter
+    def actuators(self, actuators_name: List[DAQ_Move]):
+        self._actuators = actuators_name
+
+    def check_steps(self):
+        steps_limit = config('scan', 'steps_limit')
+        n_steps = self.evaluate_steps()
+        return n_steps <= steps_limit
+
+    def __call__(self, **kwargs):
+        return self(**kwargs)
+
+    @abstractmethod
+    def set_scan(self):
+        """To be reimplemented. Calculations of all mandatory attributes from the settings"""
+        ...
+
+    @abstractmethod
+    def get_nav_axes(self) -> List[Axis]:
+        """To be reimplemented. Calculations of all navigation axes from attributes"""
+        ...
+
+    @abstractmethod
+    def get_scan_shape(self) -> Tuple[int]:
+        """To be reimplemented. Calculations of all the final shape of the scan"""
+        ...
+
+    @abstractmethod
+    def get_indexes_from_scan_index(self, scan_index: int) -> Tuple[int]:
+        """To be reimplemented. Calculations of indexes within the scan"""
+        ...
+
+    def get_info_from_positions(self, positions: np.ndarray):
+        """Set mandatory attributes from a ndarray of positions"""
+        if positions is not None:
+            if len(positions.shape) == 1:
+                positions = np.expand_dims(positions, 1)
+            axes_unique = []
+            for ax in positions.T:
+                axes_unique.append(np.unique(ax))
+            axes_indexes = np.zeros_like(positions, dtype=int)
+            for ind in range(positions.shape[0]):
+                for ind_pos, pos in enumerate(positions[ind]):
+                    axes_indexes[ind, ind_pos] = mutils.find_index(axes_unique[ind_pos], pos)[0][0]
+
+            self.n_axes = len(axes_unique)
+            self.axes_unique = axes_unique
+            self.axes_indexes = axes_indexes
+            self.positions = positions
+            self.n_steps = positions.shape[0]
+
+    @abstractmethod
+    def evaluate_steps(self):
+        """To be reimplemented. Quick evaluation of the current numbers of scan steps from the settings
+        """
+        ...
+
+    def update_model(self):
+        """Method to reimplement and use for scanners using table_view types Parameters to set and apply the underlying
+        model
+
+        See Also
+        --------
+        SequentialScanner, TabularScanner, pymodaq.utils.parameter.pymodaq_ptypes.tableview
+        """
+        ...
+
+    def value_changed(self, param):
+        self.evaluate_steps()
+
+    @abstractmethod
+    def update_from_scan_selector(self, scan_selector: Selector):
+        """To be reimplemented. Process the Selector object to set the Scanner settings
+
+        See Also
+        --------
+        Selector, ScanSelector
+        """
+        ...
+
+
+class ScannerFactory(ObjectFactory):
+    """Factory class registering and storing Scanners"""
+
+    @classmethod
+    def register(cls, key: str, sub_key: str = '') -> Callable:
+        def inner_wrapper(wrapped_class: Union[Callable]) -> Callable:
+            if cls.__name__ not in cls._builders:
+                cls._builders[cls.__name__] = {}
+            if key not in cls._builders[cls.__name__]:
+                cls._builders[cls.__name__][key] = {}
+            if sub_key not in cls._builders[cls.__name__][key]:
+                cls._builders[cls.__name__][key][sub_key] = wrapped_class
+            else:
+                logger.warning(f'The {cls.__name__}/{key}/{sub_key} builder is already registered. Replacing it')
+            return wrapped_class
+
+        return inner_wrapper
+
+    @classmethod
+    def create(cls, key, sub_key, **kwargs) -> ScannerBase:
+        builder = cls._builders[cls.__name__].get(key).get(sub_key)
+        if not builder:
+            raise ValueError(key)
+        return builder(**kwargs)
+
+    def get(self, scan_type, scan_sub_type, **kwargs):
+        return self.create(scan_type, scan_sub_type, **kwargs)
+
+    def scan_types(self) -> List[str]:
+        """Returns the list of scan types, main identifier of a given scanner"""
+        return sorted(list(self.builders[self.__class__.__name__].keys()))
+
+    def scan_sub_types(self, scan_type: str) -> List[str]:
+        """Returns the list of scan subtypes, second identifier of a given scanner of type scan_type"""
+        return list(self.builders[self.__class__.__name__][scan_type].keys())
 
-        """
-        raise NotImplementedError
-
-    def convert_output(self, outputs, dt, stab=True):
-        """
-        Convert the output of the PID in units to be fed into the actuator
-        Parameters
-        ----------
-        outputs: (list of float) output value from the PID from which the model extract a value of the same units as the actuator
-        dt: (float) elapsed time in seconds since last call
-        Returns
-        -------
-        OutputToActuator: the converted output as an OutputToActuator object
-
-        """
-        self.curr_output = outputs
-        return OutputToActuator(mode='rel', values=outputs)
-
-
-def main(xmlfile):
-    from pymodaq.dashboard import DashBoard
-    from pymodaq.utils.config import get_set_preset_path
-    from pathlib import Path
-    from qtpy import QtWidgets
-    from extensions.pid.pid_controller import DAQ_PID
-
-    import sys
-    app = QtWidgets.QApplication(sys.argv)
-    win = QtWidgets.QMainWindow()
-    area = DockArea()
-    win.setCentralWidget(area)
-    win.resize(1000, 500)
-    win.setWindowTitle('PyMoDAQ Dashboard')
-
-    dashboard = DashBoard(area)
-    file = Path(get_set_preset_path()).joinpath(xmlfile)
-    if file.exists():
-        dashboard.set_preset_mode(file)
-        # prog.load_scan_module()
-        pid_area = DockArea()
-        pid_window = QtWidgets.QMainWindow()
-        pid_window.setCentralWidget(pid_area)
-
-        prog = DAQ_PID(pid_area)
-        pid_window.show()
-        pid_window.setWindowTitle('PidController')
-        prog.set_module_manager(dashboard.detector_modules, dashboard.actuators_modules)
-        QtWidgets.QApplication.processEvents()
-
-
-    else:
-        msgBox = QtWidgets.QMessageBox()
-        msgBox.setText(f"The default file specified in the configuration file does not exists!\n"
-                       f"{file}\n"
-                       f"Impossible to load the DAQ_PID Module")
-        msgBox.setStandardButtons(msgBox.Ok)
-        ret = msgBox.exec()
-
-    sys.exit(app.exec_())
-
-
-def get_models(model_name=None):
-    """
-    Get PID Models as a list to instantiate Control Actuators per degree of liberty in the model
-
-    Returns
-    -------
-    list: list of disct containting the name and python module of the found models
-    """
-    from pymodaq.extensions.pid.utils import PIDModelGeneric
-    models_import = []
-    entry_points = metadata.entry_points()
-    if 'pymodaq.pid_models' in entry_points:
-        discovered_models = entry_points['pymodaq.pid_models']
-        for pkg in discovered_models:
-            try:
-                module = importlib.import_module(pkg.value)
-                module_name = pkg.value
-
-                for mod in pkgutil.iter_modules([str(Path(module.__file__).parent.joinpath('models'))]):
-                    try:
-                        model_module = importlib.import_module(f'{module_name}.models.{mod.name}', module)
-                        classes = inspect.getmembers(model_module, inspect.isclass)
-                        for name, klass in classes:
-                            if klass.__base__ is PIDModelGeneric:
-                                models_import.append({'name': mod.name, 'module': model_module, 'class': klass})
-                                break
-
-                    except Exception as e:  # pragma: no cover
-                        logger.warning(str(e))
-
-            except Exception as e:  # pragma: no cover
-                logger.warning(f'Impossible to import the {pkg.value} extension: {str(e)}')
-
-    if model_name is None:
-        return models_import
-    else:
-        return find_dict_in_list_from_key_val(models_import, 'name', model_name)
```

### Comparing `pymodaq-4.0.2/src/pymodaq/post_treatment/load_and_plot.py` & `pymodaq-4.0.3/src/pymodaq/post_treatment/load_and_plot.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from pymodaq.utils.h5modules.saving import H5Saver
 from pymodaq.utils.plotting.data_viewers.viewer import ViewerBase, ViewersEnum, ViewerDispatcher
 from pymodaq.utils.gui_utils import Dock, DockArea
 
 
 class LoaderPlotter:
 
-    grouped_data1D_fullname = 'Grouped/Data1D'
+    grouped_data0D_fullname = 'Grouped/Data0D'
 
     def __init__(self, dockarea):
         self.dockarea = dockarea
         self.dispatcher = ViewerDispatcher(dockarea, title='ViewerDispatcher')
         self._viewers: dict[str, ViewerBase] = None
         self._viewer_docks: dict[str, ViewerBase] = None
         self._viewer_types: List[ViewersEnum] = None
@@ -56,60 +56,111 @@
         self.dataloader = DataLoader(h5saver)
 
     @property
     def data(self) -> DataToExport:
         return self._data
 
     def load_data(self, filter_dims: List[Union[DataDim, str]] = None, filter_full_names: List[str] = None,
-                  remove_navigation: bool = True, group_1D=False, average_axis=None, average_index: int = 0):
+                  remove_navigation: bool = True, group_0D=False, average_axis: int=None, average_index: int = 0):
+        """Load Data from the h5 node of the dataloader and apply some filtering/manipulation before plotting
+
+        Parameters
+        ----------
+        filter_dims: List[Union[DataDim, str]]
+            load only data with correct dims
+        filter_full_names: List[str]
+            load only data matching these names
+        remove_navigation: bool
+            if True, make navigation axes as signal axes (means DataND could be plotted on Viewer1D or
+            Viewer2D by concatenation)
+        group_0D: bool
+            if True, group all (initial) Data0D into one DataFromPlugins
+        average_axis: int or None
+            which axis in the data shapes should be interpereted as the average (in general it is 0 or None)
+        average_index: int
+            which step in the averaging process are we in.
+
+        Returns
+        -------
+        DataToExport
+        """
+
         self._data = DataToExport('All')
         self.dataloader.load_all('/', self._data)
 
         if average_axis is not None:
-            for ind, data in enumerate(self._data):
-                current_data = data.inav[average_index, ...]
-                if average_index == 0:
-                    data_to_append = data.inav[0:average_index + 1, ...]
-                else:
-                    data_to_append = data.inav[0:average_index+1, ...].mean(axis=average_axis)
-                data_to_append.labels = [f'{label}_averaged' for label in data_to_append.labels]
-                current_data.append(data_to_append)
-                self._data[ind] = current_data
-
-        if remove_navigation:
-            for data in self._data:
-                data.nav_indexes = ()
-                data.transpose()  # because usual ND data should be plotted here as 2D with the nav axes as the minor
-                # (horizontal)
+            self.average_axis(average_axis, average_index)
 
         if filter_dims is not None:
             filter_dims[:] = [enum_checker(DataDim, dim) for dim in filter_dims]
             self._data.data[:] = [data for data in self._data if data.dim in filter_dims]
 
         if filter_full_names is not None:
             self._data.data[:] = [data for data in self._data if data.get_full_name() in filter_full_names]
 
-        if group_1D:
-            data = self._data.get_data_from_dim('Data1D')
-            if len(data) > 0:
-                data1D_arrays = []
-                labels = []
-                for dwa in data:
-                    data1D_arrays.extend(dwa.data)
-                    labels.extend([f'{dwa.get_full_name()}/{label}' for label in dwa.labels])
-                    self._data.remove(dwa)
-
-                data1D = DataFromPlugins(self.grouped_data1D_fullname.split('/')[1],
-                                         data=data1D_arrays, labels=labels,
-                                         origin=self.grouped_data1D_fullname.split('/')[0],
-                                         axes=dwa.axes)
-                self._data.append(data1D)
+        if group_0D:  # 0D initial data
+            self.group_0D_data()
+
+        if remove_navigation:
+            self.remove_navigation_axes()
 
         return self._data
 
+    def average_axis(self, average_axis, average_index) -> None:
+        """ Average the data along their average axis
+
+        Parameters
+        ----------
+        average_axis: int or None
+            which axis in the data shapes should be interpereted as the average (in general it is 0 or None)
+        average_index: int
+            which step in the averaging process are we in.
+        """
+        for ind, data in enumerate(self._data):
+            current_data = data.inav[average_index, ...]
+            if average_index == 0:
+                data_to_append = data.inav[0:average_index + 1, ...]
+            else:
+                data_to_append = data.inav[0:average_index + 1, ...].mean(axis=average_axis)
+            data_to_append.labels = [f'{label}_averaged' for label in data_to_append.labels]
+            current_data.append(data_to_append)
+            self._data[ind] = current_data
+
+    def remove_navigation_axes(self):
+        """Make the navigation axes as signal axes
+
+        transforms DataND into Data1D or Data2D or error... depending the exact shape of the data and the number of
+        navigation axes
+        """
+        for data in self._data:
+            data.nav_indexes = ()
+            data.transpose()  # because usual ND data should be plotted here as 2D with the nav axes as the minor
+            # (horizontal)
+
+    def group_0D_data(self):
+        """Group in a single DataFromPlugins all data that are initialy Data0D
+
+        """
+        data = self._data.get_data_from_sig_axes(0)
+        if len(data) > 0:
+            data0D_arrays = []
+            labels = []
+            for dwa in data:
+                data0D_arrays.extend(dwa.data)
+                labels.extend([f'{dwa.get_full_name()}/{label}' for label in dwa.labels])
+                self._data.remove(dwa)
+
+            data0D = DataFromPlugins(self.grouped_data0D_fullname.split('/')[1],
+                                     data=data0D_arrays, labels=labels,
+                                     dim='DataND',
+                                     origin=self.grouped_data0D_fullname.split('/')[0],
+                                     axes=dwa.axes, nav_indexes=dwa.nav_indexes,
+                                     )
+            self._data.append(data0D)
+
     def load_plot_data(self, **kwargs):
         """Load and plot all data from the current H5Saver
 
         See Also
         -----
         load_data
         """
```

### Comparing `pymodaq-4.0.2/src/pymodaq/post_treatment/process_to_scalar.py` & `pymodaq-4.0.3/src/pymodaq/post_treatment/process_to_scalar.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/post_treatment/daq_analysis/daq_analysis_main.py` & `pymodaq-4.0.3/src/pymodaq/post_treatment/daq_analysis/daq_analysis_main.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/post_treatment/daq_measurement/daq_measurement_GUI.py` & `pymodaq-4.0.3/src/pymodaq/post_treatment/daq_measurement/daq_measurement_GUI.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/post_treatment/daq_measurement/daq_measurement_GUI.ui` & `pymodaq-4.0.3/src/pymodaq/post_treatment/daq_measurement/daq_measurement_GUI.ui`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/post_treatment/daq_measurement/daq_measurement_main.py` & `pymodaq-4.0.3/src/pymodaq/post_treatment/daq_measurement/daq_measurement_main.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/config_template.toml` & `pymodaq-4.0.3/src/pymodaq/resources/config_template.toml`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/preset_default.xml` & `pymodaq-4.0.3/src/pymodaq/resources/preset_default.xml`

 * *Files 3% similar despite different names*

#### Comparing `pymodaq-4.0.2/src/pymodaq/resources/preset_default.xml` & `pymodaq-4.0.3/src/pymodaq/resources/preset_default.xml`

```diff
@@ -2,137 +2,146 @@
 <Preset type="group" title="Preset" visible="1" removable="0" readonly="0">
   <filename type="str" title="Filename:" visible="1" removable="0" readonly="0" show_pb="0">preset_default</filename>
   <use_pid type="bool" title="Use PID as actuator:" visible="1" removable="0" readonly="0" show_pb="0">0</use_pid>
   <pid_models type="list" title="PID models:" visible="0" removable="0" readonly="0" values="['PIDModelBeamSteeringReal', 'PIDModelBeamSteeringReal1D', 'PIDModelMichelsonDemo']" limits="['PIDModelBeamSteeringReal', 'PIDModelBeamSteeringReal1D', 'PIDModelMichelsonDemo']" show_pb="0">str('PIDModelBeamSteeringReal')</pid_models>
   <model_settings type="group" title="Model Settings:" visible="0" removable="0" readonly="0" show_pb="0">
     <threshold type="float" title="Threshold" visible="1" removable="0" readonly="0" show_pb="0">40.0</threshold>
   </model_settings>
-  <Moves type="groupmove" title="Moves:" visible="1" removable="0" readonly="0" addList="['Mock', 'TCPServer', 'PID']" show_pb="0">
-    <move00 type="group" title="Actuator 00" visible="1" removable="1" readonly="0" show_pb="0">
-      <name type="str" title="Name:" visible="1" removable="0" readonly="0" show_pb="0">Xaxis</name>
-      <init type="bool" title="Init?:" visible="1" removable="0" readonly="0" show_pb="0">1</init>
-      <params type="group" title="Settings:" visible="1" removable="0" readonly="0" show_pb="0">
-        <main_settings type="group" title="Main Settings:" visible="1" removable="0" readonly="0" show_pb="0">
-          <move_type type="str" title="Actuator type:" visible="1" removable="0" readonly="1" show_pb="0">MockTau</move_type>
-          <module_name type="str" title="Actuator name:" visible="1" removable="0" readonly="1" show_pb="0">Xaxis</module_name>
-          <controller_ID type="int" title="Controller ID:" visible="1" removable="0" readonly="0" show_pb="0">5606</controller_ID>
-          <refresh_timeout type="int" title="Refresh value (ms):" visible="1" removable="0" readonly="0" show_pb="0">500</refresh_timeout>
-          <tcpip type="group" title="TCP/IP options:" visible="1" removable="0" readonly="0" show_pb="0">
-            <connect_server type="bool_push" title="Connect to server:" visible="1" removable="0" readonly="0" show_pb="0">0</connect_server>
-            <tcp_connected type="led" title="Connected?:" visible="1" removable="0" readonly="0" show_pb="0">0</tcp_connected>
-            <ip_address type="str" title="IP address:" visible="1" removable="0" readonly="0" show_pb="0">localhost</ip_address>
-            <port type="int" title="Port:" visible="1" removable="0" readonly="0" show_pb="0">6341</port>
+  <Moves type="groupmove" title="Moves:" visible="1" removable="0" readonly="0" addList="['Mock', 'HoloeyeFile', 'HoloeyeFullScreen', 'HoloeyeSplitScreen', 'PRM1Z8_pylablib', 'MockCamera', 'MockTau', 'MockTauMulti', 'TCPServer', 'PID']" addText="Add" show_pb="0">
+    <move00 type="group" title="Actuator 00" visible="1" removable="1" readonly="0">
+      <name type="str" title="Name:" visible="1" removable="0" readonly="0">Xaxis</name>
+      <init type="bool" title="Init?:" visible="1" removable="0" readonly="0">1</init>
+      <params type="group" title="Settings:" visible="1" removable="0" readonly="0">
+        <main_settings type="group" title="Main Settings:" visible="1" removable="0" readonly="0">
+          <move_type type="str" title="Actuator type:" visible="1" removable="0" readonly="1">MockTau</move_type>
+          <module_name type="str" title="Actuator name:" visible="1" removable="0" readonly="1"/>
+          <controller_ID type="int" title="Controller ID:" visible="1" removable="0" readonly="0">8199</controller_ID>
+          <refresh_timeout type="int" title="Refresh value (ms):" visible="1" removable="0" readonly="0">500</refresh_timeout>
+          <tcpip type="group" title="TCP/IP options:" visible="1" removable="0" readonly="0">
+            <connect_server type="bool_push" title="Connect to server:" visible="1" removable="0" readonly="0">0</connect_server>
+            <tcp_connected type="led" title="Connected?:" visible="1" removable="0" readonly="0">0</tcp_connected>
+            <ip_address type="str" title="IP address:" visible="1" removable="0" readonly="0">10.47.0.39</ip_address>
+            <port type="int" title="Port:" visible="1" removable="0" readonly="0">6341</port>
           </tcpip>
         </main_settings>
-        <move_settings type="group" title="Actuator Settings:" visible="1" removable="0" readonly="0" show_pb="0">
-          <comport type="str" title="Com port:" visible="1" removable="0" readonly="0" show_pb="0">COM28</comport>
-          <tau type="int" title="Tau (ms):" visible="1" removable="0" readonly="0" show_pb="0">500</tau>
-          <multiaxes type="group" title="MultiAxes:" visible="0" removable="0" readonly="0" show_pb="0">
-            <ismultiaxes type="bool" title="is Multiaxes:" visible="1" removable="0" readonly="0" show_pb="0">0</ismultiaxes>
+        <move_settings type="group" title="Actuator Settings:" visible="1" removable="0" readonly="0">
+          <tau type="int" title="Tau (ms):" visible="1" removable="0" readonly="0">100</tau>
+          <multiaxes type="group" title="MultiAxes:" visible="1" removable="0" readonly="0">
+            <ismultiaxes type="bool" title="is Multiaxes:" visible="1" removable="0" readonly="0">1</ismultiaxes>
             <multi_status type="list" title="Status:" visible="1" removable="0" readonly="0" values="['Master', 'Slave']" limits="['Master', 'Slave']" show_pb="1">str('Master')</multi_status>
-            <axis type="list" title="Axis:" visible="1" removable="0" readonly="0" values="[]" limits="[]" show_pb="1">str('')</axis>
+            <axis type="list" title="Axis:" visible="1" removable="0" readonly="0" values="['X', 'Y', 'Z', '']" limits="['X', 'Y', 'Z', '']" show_pb="1">str('X')</axis>
           </multiaxes>
-          <units type="list" title="Units:" visible="1" removable="0" readonly="0" values="[]" limits="[]" show_pb="1">str('')</units>
-          <epsilon type="float" title="Epsilon:" visible="1" removable="0" readonly="0" show_pb="0">1.0</epsilon>
-          <timeout type="int" title="Timeout (s):" visible="1" removable="0" readonly="0" show_pb="0">10</timeout>
-          <bounds type="group" title="Bounds:" visible="1" removable="0" readonly="0" show_pb="0">
-            <is_bounds type="bool" title="Set Bounds:" visible="1" removable="0" readonly="0" show_pb="0">0</is_bounds>
-            <min_bound type="float" title="Min:" visible="1" removable="0" readonly="0" show_pb="0">0.0</min_bound>
-            <max_bound type="float" title="Max:" visible="1" removable="0" readonly="0" show_pb="0">1.0</max_bound>
+          <grouping type="group" title="Grouping" visible="1" removable="0" readonly="0">
+            <grouped_axes type="itemselect" title="Axes" visible="1" removable="0" readonly="0" show_pb="1" all_items="['X', 'Y', 'Z', '']">[]</grouped_axes>
+            <do_group type="bool" title="Do group" visible="1" removable="0" readonly="0">0</do_group>
+          </grouping>
+          <units type="str" title="Units:" visible="1" removable="0" readonly="1"/>
+          <epsilon type="float" title="Epsilon:" visible="1" removable="0" readonly="0">0.01</epsilon>
+          <timeout type="int" title="Timeout (s):" visible="1" removable="0" readonly="0">20</timeout>
+          <bounds type="group" title="Bounds:" visible="1" removable="0" readonly="0">
+            <is_bounds type="bool" title="Set Bounds:" visible="1" removable="0" readonly="0">0</is_bounds>
+            <min_bound type="float" title="Min:" visible="1" removable="0" readonly="0">0.0</min_bound>
+            <max_bound type="float" title="Max:" visible="1" removable="0" readonly="0">1.0</max_bound>
           </bounds>
-          <scaling type="group" title="Scaling:" visible="1" removable="0" readonly="0" show_pb="0">
-            <use_scaling type="bool" title="Use scaling:" visible="1" removable="0" readonly="0" show_pb="0">0</use_scaling>
-            <scaling type="float" title="Scaling factor:" visible="1" removable="0" readonly="0" show_pb="0">1.0</scaling>
-            <offset type="float" title="Offset factor:" visible="1" removable="0" readonly="0" show_pb="0">0.0</offset>
+          <scaling type="group" title="Scaling:" visible="1" removable="0" readonly="0">
+            <use_scaling type="bool" title="Use scaling:" visible="1" removable="0" readonly="0">0</use_scaling>
+            <scaling type="float" title="Scaling factor:" visible="1" removable="0" readonly="0">1.0</scaling>
+            <offset type="float" title="Offset factor:" visible="1" removable="0" readonly="0">0.0</offset>
           </scaling>
         </move_settings>
       </params>
     </move00>
-    <move01 type="group" title="Actuator 01" visible="1" removable="1" readonly="0" show_pb="0">
-      <name type="str" title="Name:" visible="1" removable="0" readonly="0" show_pb="0">Yaxis</name>
-      <init type="bool" title="Init?:" visible="1" removable="0" readonly="0" show_pb="0">1</init>
-      <params type="group" title="Settings:" visible="1" removable="0" readonly="0" show_pb="0">
-        <main_settings type="group" title="Main Settings:" visible="1" removable="0" readonly="0" show_pb="0">
-          <move_type type="str" title="Actuator type:" visible="1" removable="0" readonly="1" show_pb="0">MockTau</move_type>
-          <module_name type="str" title="Actuator name:" visible="1" removable="0" readonly="1" show_pb="0">Yaxis</module_name>
-          <controller_ID type="int" title="Controller ID:" visible="1" removable="0" readonly="0" show_pb="0">8101</controller_ID>
-          <refresh_timeout type="int" title="Refresh value (ms):" visible="1" removable="0" readonly="0" show_pb="0">500</refresh_timeout>
-          <tcpip type="group" title="TCP/IP options:" visible="1" removable="0" readonly="0" show_pb="0">
-            <connect_server type="bool_push" title="Connect to server:" visible="1" removable="0" readonly="0" show_pb="0">0</connect_server>
-            <tcp_connected type="led" title="Connected?:" visible="1" removable="0" readonly="0" show_pb="0">0</tcp_connected>
-            <ip_address type="str" title="IP address:" visible="1" removable="0" readonly="0" show_pb="0">localhost</ip_address>
-            <port type="int" title="Port:" visible="1" removable="0" readonly="0" show_pb="0">6341</port>
+    <move01 type="group" title="Actuator 01" visible="1" removable="1" readonly="0">
+      <name type="str" title="Name:" visible="1" removable="0" readonly="0">Yaxis</name>
+      <init type="bool" title="Init?:" visible="1" removable="0" readonly="0">1</init>
+      <params type="group" title="Settings:" visible="1" removable="0" readonly="0">
+        <main_settings type="group" title="Main Settings:" visible="1" removable="0" readonly="0">
+          <move_type type="str" title="Actuator type:" visible="1" removable="0" readonly="1">MockTau</move_type>
+          <module_name type="str" title="Actuator name:" visible="1" removable="0" readonly="1"/>
+          <controller_ID type="int" title="Controller ID:" visible="1" removable="0" readonly="0">4142</controller_ID>
+          <refresh_timeout type="int" title="Refresh value (ms):" visible="1" removable="0" readonly="0">500</refresh_timeout>
+          <tcpip type="group" title="TCP/IP options:" visible="1" removable="0" readonly="0">
+            <connect_server type="bool_push" title="Connect to server:" visible="1" removable="0" readonly="0">0</connect_server>
+            <tcp_connected type="led" title="Connected?:" visible="1" removable="0" readonly="0">0</tcp_connected>
+            <ip_address type="str" title="IP address:" visible="1" removable="0" readonly="0">10.47.0.39</ip_address>
+            <port type="int" title="Port:" visible="1" removable="0" readonly="0">6341</port>
           </tcpip>
         </main_settings>
-        <move_settings type="group" title="Actuator Settings:" visible="1" removable="0" readonly="0" show_pb="0">
-          <comport type="str" title="Com port:" visible="1" removable="0" readonly="0" show_pb="0">COM28</comport>
-          <tau type="int" title="Tau (ms):" visible="1" removable="0" readonly="0" show_pb="0">500</tau>
-          <multiaxes type="group" title="MultiAxes:" visible="0" removable="0" readonly="0" show_pb="0">
-            <ismultiaxes type="bool" title="is Multiaxes:" visible="1" removable="0" readonly="0" show_pb="0">0</ismultiaxes>
+        <move_settings type="group" title="Actuator Settings:" visible="1" removable="0" readonly="0">
+          <tau type="int" title="Tau (ms):" visible="1" removable="0" readonly="0">100</tau>
+          <multiaxes type="group" title="MultiAxes:" visible="1" removable="0" readonly="0">
+            <ismultiaxes type="bool" title="is Multiaxes:" visible="1" removable="0" readonly="0">1</ismultiaxes>
             <multi_status type="list" title="Status:" visible="1" removable="0" readonly="0" values="['Master', 'Slave']" limits="['Master', 'Slave']" show_pb="1">str('Master')</multi_status>
-            <axis type="list" title="Axis:" visible="1" removable="0" readonly="0" values="[]" limits="[]" show_pb="1">str('')</axis>
+            <axis type="list" title="Axis:" visible="1" removable="0" readonly="0" values="['X', 'Y', 'Z', '']" limits="['X', 'Y', 'Z', '']" show_pb="1">str('X')</axis>
           </multiaxes>
-          <units type="list" title="Units:" visible="1" removable="0" readonly="0" values="[]" limits="[]" show_pb="1">str('')</units>
-          <epsilon type="float" title="Epsilon:" visible="1" removable="0" readonly="0" show_pb="0">1.0</epsilon>
-          <timeout type="int" title="Timeout (s):" visible="1" removable="0" readonly="0" show_pb="0">10</timeout>
-          <bounds type="group" title="Bounds:" visible="1" removable="0" readonly="0" show_pb="0">
-            <is_bounds type="bool" title="Set Bounds:" visible="1" removable="0" readonly="0" show_pb="0">0</is_bounds>
-            <min_bound type="float" title="Min:" visible="1" removable="0" readonly="0" show_pb="0">0.0</min_bound>
-            <max_bound type="float" title="Max:" visible="1" removable="0" readonly="0" show_pb="0">1.0</max_bound>
+          <grouping type="group" title="Grouping" visible="1" removable="0" readonly="0">
+            <grouped_axes type="itemselect" title="Axes" visible="1" removable="0" readonly="0" show_pb="1" all_items="['X', 'Y', 'Z', '']">[]</grouped_axes>
+            <do_group type="bool" title="Do group" visible="1" removable="0" readonly="0">0</do_group>
+          </grouping>
+          <units type="str" title="Units:" visible="1" removable="0" readonly="1"/>
+          <epsilon type="float" title="Epsilon:" visible="1" removable="0" readonly="0">0.01</epsilon>
+          <timeout type="int" title="Timeout (s):" visible="1" removable="0" readonly="0">20</timeout>
+          <bounds type="group" title="Bounds:" visible="1" removable="0" readonly="0">
+            <is_bounds type="bool" title="Set Bounds:" visible="1" removable="0" readonly="0">0</is_bounds>
+            <min_bound type="float" title="Min:" visible="1" removable="0" readonly="0">0.0</min_bound>
+            <max_bound type="float" title="Max:" visible="1" removable="0" readonly="0">1.0</max_bound>
           </bounds>
-          <scaling type="group" title="Scaling:" visible="1" removable="0" readonly="0" show_pb="0">
-            <use_scaling type="bool" title="Use scaling:" visible="1" removable="0" readonly="0" show_pb="0">0</use_scaling>
-            <scaling type="float" title="Scaling factor:" visible="1" removable="0" readonly="0" show_pb="0">1.0</scaling>
-            <offset type="float" title="Offset factor:" visible="1" removable="0" readonly="0" show_pb="0">0.0</offset>
+          <scaling type="group" title="Scaling:" visible="1" removable="0" readonly="0">
+            <use_scaling type="bool" title="Use scaling:" visible="1" removable="0" readonly="0">0</use_scaling>
+            <scaling type="float" title="Scaling factor:" visible="1" removable="0" readonly="0">1.0</scaling>
+            <offset type="float" title="Offset factor:" visible="1" removable="0" readonly="0">0.0</offset>
           </scaling>
         </move_settings>
       </params>
     </move01>
-    <move02 type="group" title="Actuator 02" visible="1" removable="1" readonly="0" show_pb="0">
-      <name type="str" title="Name:" visible="1" removable="0" readonly="0" show_pb="0">Theta</name>
-      <init type="bool" title="Init?:" visible="1" removable="0" readonly="0" show_pb="0">1</init>
-      <params type="group" title="Settings:" visible="1" removable="0" readonly="0" show_pb="0">
-        <main_settings type="group" title="Main Settings:" visible="1" removable="0" readonly="0" show_pb="0">
-          <move_type type="str" title="Actuator type:" visible="1" removable="0" readonly="1" show_pb="0">MockTau</move_type>
-          <module_name type="str" title="Actuator name:" visible="1" removable="0" readonly="1" show_pb="0">Theta</module_name>
-          <controller_ID type="int" title="Controller ID:" visible="1" removable="0" readonly="0" show_pb="0">6356</controller_ID>
-          <refresh_timeout type="int" title="Refresh value (ms):" visible="1" removable="0" readonly="0" show_pb="0">500</refresh_timeout>
-          <tcpip type="group" title="TCP/IP options:" visible="1" removable="0" readonly="0" show_pb="0">
-            <connect_server type="bool_push" title="Connect to server:" visible="1" removable="0" readonly="0" show_pb="0">0</connect_server>
-            <tcp_connected type="led" title="Connected?:" visible="1" removable="0" readonly="0" show_pb="0">0</tcp_connected>
-            <ip_address type="str" title="IP address:" visible="1" removable="0" readonly="0" show_pb="0">localhost</ip_address>
-            <port type="int" title="Port:" visible="1" removable="0" readonly="0" show_pb="0">6341</port>
+    <move02 type="group" title="Actuator 02" visible="1" removable="1" readonly="0">
+      <name type="str" title="Name:" visible="1" removable="0" readonly="0">Theta</name>
+      <init type="bool" title="Init?:" visible="1" removable="0" readonly="0">1</init>
+      <params type="group" title="Settings:" visible="1" removable="0" readonly="0">
+        <main_settings type="group" title="Main Settings:" visible="1" removable="0" readonly="0">
+          <move_type type="str" title="Actuator type:" visible="1" removable="0" readonly="1">MockTau</move_type>
+          <module_name type="str" title="Actuator name:" visible="1" removable="0" readonly="1"/>
+          <controller_ID type="int" title="Controller ID:" visible="1" removable="0" readonly="0">1911</controller_ID>
+          <refresh_timeout type="int" title="Refresh value (ms):" visible="1" removable="0" readonly="0">500</refresh_timeout>
+          <tcpip type="group" title="TCP/IP options:" visible="1" removable="0" readonly="0">
+            <connect_server type="bool_push" title="Connect to server:" visible="1" removable="0" readonly="0">0</connect_server>
+            <tcp_connected type="led" title="Connected?:" visible="1" removable="0" readonly="0">0</tcp_connected>
+            <ip_address type="str" title="IP address:" visible="1" removable="0" readonly="0">10.47.0.39</ip_address>
+            <port type="int" title="Port:" visible="1" removable="0" readonly="0">6341</port>
           </tcpip>
         </main_settings>
-        <move_settings type="group" title="Actuator Settings:" visible="1" removable="0" readonly="0" show_pb="0">
-          <comport type="str" title="Com port:" visible="1" removable="0" readonly="0" show_pb="0">COM28</comport>
-          <tau type="int" title="Tau (ms):" visible="1" removable="0" readonly="0" show_pb="0">2000</tau>
-          <multiaxes type="group" title="MultiAxes:" visible="0" removable="0" readonly="0" show_pb="0">
-            <ismultiaxes type="bool" title="is Multiaxes:" visible="1" removable="0" readonly="0" show_pb="0">0</ismultiaxes>
+        <move_settings type="group" title="Actuator Settings:" visible="1" removable="0" readonly="0">
+          <tau type="int" title="Tau (ms):" visible="1" removable="0" readonly="0">200</tau>
+          <multiaxes type="group" title="MultiAxes:" visible="1" removable="0" readonly="0">
+            <ismultiaxes type="bool" title="is Multiaxes:" visible="1" removable="0" readonly="0">1</ismultiaxes>
             <multi_status type="list" title="Status:" visible="1" removable="0" readonly="0" values="['Master', 'Slave']" limits="['Master', 'Slave']" show_pb="1">str('Master')</multi_status>
-            <axis type="list" title="Axis:" visible="1" removable="0" readonly="0" values="[]" limits="[]" show_pb="1">str('')</axis>
+            <axis type="list" title="Axis:" visible="1" removable="0" readonly="0" values="['X', 'Y', 'Z', '']" limits="['X', 'Y', 'Z', '']" show_pb="1">str('X')</axis>
           </multiaxes>
-          <units type="list" title="Units:" visible="1" removable="0" readonly="0" values="[]" limits="[]" show_pb="1">str('')</units>
-          <epsilon type="float" title="Epsilon:" visible="1" removable="0" readonly="0" show_pb="0">1.0</epsilon>
-          <timeout type="int" title="Timeout (s):" visible="1" removable="0" readonly="0" show_pb="0">10</timeout>
-          <bounds type="group" title="Bounds:" visible="1" removable="0" readonly="0" show_pb="0">
-            <is_bounds type="bool" title="Set Bounds:" visible="1" removable="0" readonly="0" show_pb="0">0</is_bounds>
-            <min_bound type="float" title="Min:" visible="1" removable="0" readonly="0" show_pb="0">0.0</min_bound>
-            <max_bound type="float" title="Max:" visible="1" removable="0" readonly="0" show_pb="0">1.0</max_bound>
+          <grouping type="group" title="Grouping" visible="1" removable="0" readonly="0">
+            <grouped_axes type="itemselect" title="Axes" visible="1" removable="0" readonly="0" show_pb="1" all_items="['X', 'Y', 'Z', '']">[]</grouped_axes>
+            <do_group type="bool" title="Do group" visible="1" removable="0" readonly="0">0</do_group>
+          </grouping>
+          <units type="str" title="Units:" visible="1" removable="0" readonly="1"/>
+          <epsilon type="float" title="Epsilon:" visible="1" removable="0" readonly="0">0.01</epsilon>
+          <timeout type="int" title="Timeout (s):" visible="1" removable="0" readonly="0">20</timeout>
+          <bounds type="group" title="Bounds:" visible="1" removable="0" readonly="0">
+            <is_bounds type="bool" title="Set Bounds:" visible="1" removable="0" readonly="0">0</is_bounds>
+            <min_bound type="float" title="Min:" visible="1" removable="0" readonly="0">0.0</min_bound>
+            <max_bound type="float" title="Max:" visible="1" removable="0" readonly="0">1.0</max_bound>
           </bounds>
-          <scaling type="group" title="Scaling:" visible="1" removable="0" readonly="0" show_pb="0">
-            <use_scaling type="bool" title="Use scaling:" visible="1" removable="0" readonly="0" show_pb="0">0</use_scaling>
-            <scaling type="float" title="Scaling factor:" visible="1" removable="0" readonly="0" show_pb="0">1.0</scaling>
-            <offset type="float" title="Offset factor:" visible="1" removable="0" readonly="0" show_pb="0">0.0</offset>
+          <scaling type="group" title="Scaling:" visible="1" removable="0" readonly="0">
+            <use_scaling type="bool" title="Use scaling:" visible="1" removable="0" readonly="0">0</use_scaling>
+            <scaling type="float" title="Scaling factor:" visible="1" removable="0" readonly="0">1.0</scaling>
+            <offset type="float" title="Offset factor:" visible="1" removable="0" readonly="0">0.0</offset>
           </scaling>
         </move_settings>
       </params>
     </move02>
   </Moves>
-  <Detectors type="groupdet" title="Detectors:" visible="1" removable="0" readonly="0" addList="['DAQ0D/Mock', 'DAQ0D/TCPServer', 'DAQ1D/Mock', 'DAQ1D/Mock_spectro', 'DAQ1D/TCPServer', 'DAQ2D/Mock', 'DAQ2D/TCPServer', 'DAQND/Mock']" show_pb="0">
+  <Detectors type="groupdet" title="Detectors:" visible="1" removable="0" readonly="0" addList="['DAQ0D/Mock', 'DAQ0D/Kinesis_KPA101', 'DAQ0D/TLPMPowermeter', 'DAQ0D/TLPMPowermeterInst', 'DAQ0D/BeamSteering', 'DAQ0D/Boiler', 'DAQ0D/TCPServer', 'DAQ1D/Mock', 'DAQ1D/BeamSteering', 'DAQ1D/Mock_spectro', 'DAQ1D/TCPServer', 'DAQ1D/Omnidriver', 'DAQ1D/Seabreeze', 'DAQ2D/Mock', 'DAQ2D/Thorlabs_DCx', 'DAQ2D/Thorlabs_TSI', 'DAQ2D/BeamSteering', 'DAQ2D/BeamSteeringAll', 'DAQ2D/BeamSteeringFocused', 'DAQ2D/MockCamera', 'DAQ2D/TCPServer', 'DAQND/Mock']" addText="Add" show_pb="0">
     <det00 type="group" title="Det 00" visible="1" removable="1" readonly="0" show_pb="0">
       <name type="str" title="Name:" visible="1" removable="0" readonly="0" show_pb="0">Det0D</name>
       <init type="bool" title="Init?:" visible="1" removable="0" readonly="0" show_pb="0">1</init>
       <params type="group" title="Settings:" visible="1" removable="0" readonly="0" show_pb="0">
         <main_settings type="group" title="Main Settings:" visible="1" removable="0" readonly="0" show_pb="0">
           <DAQ_type type="list" title="DAQ type:" visible="1" removable="0" readonly="1" values="['DAQ0D', 'DAQ1D', 'DAQ2D', 'DAQND']" limits="['DAQ0D', 'DAQ1D', 'DAQ2D', 'DAQND']" show_pb="1">str('DAQ0D')</DAQ_type>
           <detector_type type="str" title="Detector type:" visible="1" removable="0" readonly="1" show_pb="0">Mock</detector_type>
@@ -279,73 +288,73 @@
             <dx type="float" title="dx:" visible="1" removable="0" readonly="0" show_pb="0">0.1</dx>
           </x_axis>
           <laser_wl type="list" title="Laser Wavelength" visible="1" removable="0" readonly="0" values="[405, 515, 632.8]" limits="[405, 515, 632.8]" show_pb="1">int(515)</laser_wl>
           <exposure_ms type="int" title="Exposure (ms)" visible="1" removable="0" readonly="0" show_pb="0">100</exposure_ms>
         </detector_settings>
       </params>
     </det01>
-    <det02 type="group" title="Det 02" visible="1" removable="1" readonly="0">
-      <name type="str" title="Name:" visible="1" removable="0" readonly="0">Det 02</name>
-      <init type="bool" title="Init?:" visible="1" removable="0" readonly="0">1</init>
-      <params type="group" title="Settings:" visible="1" removable="0" readonly="0">
-        <main_settings type="group" title="Main Settings:" visible="1" removable="0" readonly="0">
+    <det02 type="group" title="Det 02" visible="1" removable="1" readonly="0" show_pb="0">
+      <name type="str" title="Name:" visible="1" removable="0" readonly="0" show_pb="0">Det 2D</name>
+      <init type="bool" title="Init?:" visible="1" removable="0" readonly="0" show_pb="0">1</init>
+      <params type="group" title="Settings:" visible="1" removable="0" readonly="0" show_pb="0">
+        <main_settings type="group" title="Main Settings:" visible="1" removable="0" readonly="0" show_pb="0">
           <DAQ_type type="list" title="DAQ type:" visible="1" removable="0" readonly="1" values="['DAQ0D', 'DAQ1D', 'DAQ2D', 'DAQND']" limits="['DAQ0D', 'DAQ1D', 'DAQ2D', 'DAQND']" show_pb="1">str('DAQ2D')</DAQ_type>
-          <detector_type type="str" title="Detector type:" visible="1" removable="0" readonly="1">Mock</detector_type>
-          <module_name type="str" title="Detector Name:" visible="1" removable="0" readonly="1"/>
-          <Nviewers type="int" title="Nviewers:" visible="1" removable="0" readonly="1">1</Nviewers>
-          <controller_ID type="int" title="Controller ID:" visible="1" removable="0" readonly="0">4944</controller_ID>
-          <show_data type="bool" title="Show data and process:" visible="1" removable="0" readonly="0">1</show_data>
-          <refresh_time type="float" title="Refresh time (ms):" visible="1" removable="0" readonly="0">50.0</refresh_time>
-          <Naverage type="int" title="Naverage" visible="1" removable="0" readonly="0">1</Naverage>
-          <show_averaging type="bool" title="Show averaging:" visible="1" removable="0" readonly="0">0</show_averaging>
-          <live_averaging type="bool" title="Live averaging:" visible="1" removable="0" readonly="0">0</live_averaging>
-          <N_live_averaging type="int" title="N Live aver.:" visible="0" removable="0" readonly="0">0</N_live_averaging>
-          <wait_time type="int" title="Wait time (ms):" visible="1" removable="0" readonly="0">0</wait_time>
-          <continuous_saving_opt type="bool" title="Continuous saving:" visible="1" removable="0" readonly="0">0</continuous_saving_opt>
-          <tcpip type="group" title="TCP/IP options:" visible="1" removable="0" readonly="0">
-            <connect_server type="bool_push" title="Connect to server:" visible="1" removable="0" readonly="0">0</connect_server>
-            <tcp_connected type="led" title="Connected?:" visible="1" removable="0" readonly="0">0</tcp_connected>
-            <ip_address type="str" title="IP address:" visible="1" removable="0" readonly="0">10.47.0.39</ip_address>
-            <port type="int" title="Port:" visible="1" removable="0" readonly="0">6341</port>
+          <detector_type type="str" title="Detector type:" visible="1" removable="0" readonly="1" show_pb="0">Mock</detector_type>
+          <module_name type="str" title="Detector Name:" visible="1" removable="0" readonly="1" show_pb="0"/>
+          <Nviewers type="int" title="Nviewers:" visible="1" removable="0" readonly="1" show_pb="0">1</Nviewers>
+          <controller_ID type="int" title="Controller ID:" visible="1" removable="0" readonly="0" show_pb="0">4944</controller_ID>
+          <show_data type="bool" title="Show data and process:" visible="1" removable="0" readonly="0" show_pb="0">1</show_data>
+          <refresh_time type="float" title="Refresh time (ms):" visible="1" removable="0" readonly="0" show_pb="0">50.0</refresh_time>
+          <Naverage type="int" title="Naverage" visible="1" removable="0" readonly="0" show_pb="0">1</Naverage>
+          <show_averaging type="bool" title="Show averaging:" visible="1" removable="0" readonly="0" show_pb="0">0</show_averaging>
+          <live_averaging type="bool" title="Live averaging:" visible="1" removable="0" readonly="0" show_pb="0">0</live_averaging>
+          <N_live_averaging type="int" title="N Live aver.:" visible="0" removable="0" readonly="0" show_pb="0">0</N_live_averaging>
+          <wait_time type="int" title="Wait time (ms):" visible="1" removable="0" readonly="0" show_pb="0">0</wait_time>
+          <continuous_saving_opt type="bool" title="Continuous saving:" visible="1" removable="0" readonly="0" show_pb="0">0</continuous_saving_opt>
+          <tcpip type="group" title="TCP/IP options:" visible="1" removable="0" readonly="0" show_pb="0">
+            <connect_server type="bool_push" title="Connect to server:" visible="1" removable="0" readonly="0" show_pb="0">0</connect_server>
+            <tcp_connected type="led" title="Connected?:" visible="1" removable="0" readonly="0" show_pb="0">0</tcp_connected>
+            <ip_address type="str" title="IP address:" visible="1" removable="0" readonly="0" show_pb="0">10.47.0.39</ip_address>
+            <port type="int" title="Port:" visible="1" removable="0" readonly="0" show_pb="0">6341</port>
           </tcpip>
-          <overshoot type="group" title="Overshoot options:" visible="1" removable="0" readonly="0">
-            <stop_overshoot type="bool" title="Overshoot:" visible="1" removable="0" readonly="0">0</stop_overshoot>
-            <overshoot_value type="float" title="Overshoot value:" visible="1" removable="0" readonly="0">0.0</overshoot_value>
+          <overshoot type="group" title="Overshoot options:" visible="1" removable="0" readonly="0" show_pb="0">
+            <stop_overshoot type="bool" title="Overshoot:" visible="1" removable="0" readonly="0" show_pb="0">0</stop_overshoot>
+            <overshoot_value type="float" title="Overshoot value:" visible="1" removable="0" readonly="0" show_pb="0">0.0</overshoot_value>
           </overshoot>
-          <axes type="group" title="Axis options:" visible="1" removable="0" readonly="0">
+          <axes type="group" title="Axis options:" visible="1" removable="0" readonly="0" show_pb="0">
             <use_calib type="list" title="Use calibration?:" visible="1" removable="0" readonly="0" values="['None']" limits="['None']" show_pb="1">str('None')</use_calib>
-            <xaxis type="group" title="X axis:" visible="1" removable="0" readonly="0">
-              <xlabel type="str" title="Label:" visible="1" removable="0" readonly="0">x axis</xlabel>
-              <xunits type="str" title="Units:" visible="1" removable="0" readonly="0">pxls</xunits>
-              <xoffset type="float" title="Offset:" visible="1" removable="0" readonly="0">0.0</xoffset>
-              <xscaling type="float" title="Scaling" visible="1" removable="0" readonly="0">1.0</xscaling>
+            <xaxis type="group" title="X axis:" visible="1" removable="0" readonly="0" show_pb="0">
+              <xlabel type="str" title="Label:" visible="1" removable="0" readonly="0" show_pb="0">x axis</xlabel>
+              <xunits type="str" title="Units:" visible="1" removable="0" readonly="0" show_pb="0">pxls</xunits>
+              <xoffset type="float" title="Offset:" visible="1" removable="0" readonly="0" show_pb="0">0.0</xoffset>
+              <xscaling type="float" title="Scaling" visible="1" removable="0" readonly="0" show_pb="0">1.0</xscaling>
             </xaxis>
-            <yaxis type="group" title="Y axis:" visible="1" removable="0" readonly="0">
-              <ylabel type="str" title="Label:" visible="1" removable="0" readonly="0">y axis</ylabel>
-              <yunits type="str" title="Units:" visible="1" removable="0" readonly="0">pxls</yunits>
-              <yoffset type="float" title="Offset:" visible="1" removable="0" readonly="0">0.0</yoffset>
-              <yscaling type="float" title="Scaling" visible="1" removable="0" readonly="0">1.0</yscaling>
+            <yaxis type="group" title="Y axis:" visible="1" removable="0" readonly="0" show_pb="0">
+              <ylabel type="str" title="Label:" visible="1" removable="0" readonly="0" show_pb="0">y axis</ylabel>
+              <yunits type="str" title="Units:" visible="1" removable="0" readonly="0" show_pb="0">pxls</yunits>
+              <yoffset type="float" title="Offset:" visible="1" removable="0" readonly="0" show_pb="0">0.0</yoffset>
+              <yscaling type="float" title="Scaling" visible="1" removable="0" readonly="0" show_pb="0">1.0</yscaling>
             </yaxis>
           </axes>
         </main_settings>
-        <detector_settings type="group" title="Detector Settings" visible="1" removable="0" readonly="0">
+        <detector_settings type="group" title="Detector Settings" visible="1" removable="0" readonly="0" show_pb="0">
           <controller_status type="list" title="Controller Status:" visible="1" removable="0" readonly="0" values="['Master', 'Slave']" limits="['Master', 'Slave']" show_pb="1">str('Master')</controller_status>
-          <Nimagescolor type="int" title="Nimages colors:" visible="1" removable="0" readonly="0">1</Nimagescolor>
-          <Nimagespannel type="int" title="Nimages pannels:" visible="1" removable="0" readonly="0">1</Nimagespannel>
-          <use_roi_select type="bool" title="Use ROISelect" visible="1" removable="0" readonly="0">0</use_roi_select>
-          <threshold type="int" title="Threshold" visible="1" removable="0" readonly="0">1</threshold>
-          <rolling type="int" title="rolling" visible="1" removable="0" readonly="0">1</rolling>
-          <Nx type="int" title="Nx" visible="1" removable="0" readonly="0">100</Nx>
-          <Ny type="int" title="Ny" visible="1" removable="0" readonly="0">200</Ny>
-          <Amp type="int" title="Amp" visible="1" removable="0" readonly="0">20</Amp>
-          <x0 type="slide" title="x0" visible="1" removable="0" readonly="0">50</x0>
-          <y0 type="float" title="y0" visible="1" removable="0" readonly="0">100.0</y0>
-          <dx type="float" title="dx" visible="1" removable="0" readonly="0">20.0</dx>
-          <dy type="float" title="dy" visible="1" removable="0" readonly="0">40.0</dy>
-          <n type="int" title="n" visible="1" removable="0" readonly="0">1</n>
-          <amp_noise type="float" title="amp_noise" visible="1" removable="0" readonly="0">4.0</amp_noise>
-          <cam_settings type="group" title="Cam. Prop.:" visible="1" removable="0" readonly="0"/>
+          <Nimagescolor type="int" title="Nimages colors:" visible="1" removable="0" readonly="0" show_pb="0">1</Nimagescolor>
+          <Nimagespannel type="int" title="Nimages pannels:" visible="1" removable="0" readonly="0" show_pb="0">1</Nimagespannel>
+          <use_roi_select type="bool" title="Use ROISelect" visible="1" removable="0" readonly="0" show_pb="0">0</use_roi_select>
+          <threshold type="int" title="Threshold" visible="1" removable="0" readonly="0" show_pb="0">1</threshold>
+          <rolling type="int" title="rolling" visible="1" removable="0" readonly="0" show_pb="0">1</rolling>
+          <Nx type="int" title="Nx" visible="1" removable="0" readonly="0" show_pb="0">100</Nx>
+          <Ny type="int" title="Ny" visible="1" removable="0" readonly="0" show_pb="0">200</Ny>
+          <Amp type="int" title="Amp" visible="1" removable="0" readonly="0" show_pb="0">20</Amp>
+          <x0 type="slide" title="x0" visible="1" removable="0" readonly="0" show_pb="0">50.0</x0>
+          <y0 type="float" title="y0" visible="1" removable="0" readonly="0" show_pb="0">100.0</y0>
+          <dx type="float" title="dx" visible="1" removable="0" readonly="0" show_pb="0">20.0</dx>
+          <dy type="float" title="dy" visible="1" removable="0" readonly="0" show_pb="0">40.0</dy>
+          <n type="int" title="n" visible="1" removable="0" readonly="0" show_pb="0">1</n>
+          <amp_noise type="float" title="amp_noise" visible="1" removable="0" readonly="0" show_pb="0">4.0</amp_noise>
+          <cam_settings type="group" title="Cam. Prop.:" visible="1" removable="0" readonly="0" show_pb="0"/>
         </detector_settings>
       </params>
     </det02>
   </Detectors>
 </Preset>
```

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/triangulation_data.npy` & `pymodaq-4.0.3/src/pymodaq/resources/triangulation_data.npy`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/QtDesigner_ressources.qrc` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/QtDesigner_ressources.qrc`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/QtDesigner_ressources_rc.py` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/QtDesigner_ressources_rc.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/icons.svg` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/icons.svg`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Add_Step.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Add_Step.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Browse_Dir_Path.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Browse_Dir_Path.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Calculator.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Calculator.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/CollapseAll.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/CollapseAll.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/CollapseAll_32.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/CollapseAll_32.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ColorPicker.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ColorPicker.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/DeleteLayer.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/DeleteLayer.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EditOpen.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EditOpen.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EditRedo.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EditRedo.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EditUndo.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EditUndo.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Ellipse.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Ellipse.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EllipseFilled.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/EllipseFilled.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Error.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Error.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Error_16.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Error_16.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Exit.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Exit.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ExpandAll.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ExpandAll.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ExpandAll_32.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ExpandAll_32.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/HLM.ico` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/HLM.ico`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Help_32.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Help_32.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MagnifyingGlass.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MagnifyingGlass.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MagnifyingGlass_24.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MagnifyingGlass_24.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MeasurementStudio_32.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MeasurementStudio_32.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Move.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Move.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MoveDown.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MoveDown.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MoveUp.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/MoveUp.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/NewFile.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/NewFile.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/NewLayer.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/NewLayer.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_1D.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_1D.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_2D.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_2D.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_File_32.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_File_32.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_sim.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Open_sim.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Options.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Options.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Rectangle.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Rectangle.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/RectangleFilled.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/RectangleFilled.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Redo.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Redo.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Refresh.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Refresh.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Refresh_32.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Refresh_32.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SaveAll_32.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SaveAll_32.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SaveAs.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SaveAs.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SaveAs_32.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SaveAs_32.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Save_24.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Save_24.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Save_32.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Save_32.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SelectPolygon.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/SelectPolygon.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Select_24.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Select_24.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Settings.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Settings.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snap&Save.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snap&Save.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot2.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot2_16.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot2_16.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot2_32.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/Snapshot2_32.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/autoscale.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/autoscale.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/camera_snap.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/camera_snap.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/clear2.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/clear2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/clear_ROI.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/clear_ROI.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/cluster2.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/cluster2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/data.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/data.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/delay.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/delay.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/exit2.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/exit2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/gear2.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/gear2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/go_to_1.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/go_to_1.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/go_to_2.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/go_to_2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/greenLight2.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/greenLight2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/greenLight2_32.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/greenLight2_32.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/green_light.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/green_light.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/information2.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/information2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ini.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/ini.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_green.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_green.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_green_16.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_green_16.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_red.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_red.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_red_16.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_red_16.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_yellow.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_yellow.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_yellow_16.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/light_yellow_16.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/load_ROI.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/load_ROI.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meshPlot.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meshPlot.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meter.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meter.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meter2.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meter2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meter_32.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/meter_32.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/move_contour.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/move_contour.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/openArrow.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/openArrow.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/oscilloscope2.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/oscilloscope2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/oscilloscope3.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/oscilloscope3.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pass2.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pass2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pass2_16.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pass2_16.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pass_32.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/pass_32.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/powerMeter.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/powerMeter.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/powerSwitch.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/powerSwitch.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/powerSwitch_16.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/powerSwitch_16.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/print2.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/print2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/print2_32.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/print2_32.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/radiocontrolbutton.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/radiocontrolbutton.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/red_light.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/red_light.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/robot.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/robot.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/rotation2.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/rotation2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/run_all.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/run_all.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/save_ROI.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/save_ROI.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/select_all2.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/select_all2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/spectrumAnalyzer.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/spectrumAnalyzer.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/stop2.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/stop2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/stop_all.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/stop_all.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/surfacePlot.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/surfacePlot.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/utility2.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/utility2.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/utility_small.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/utility_small.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/waterfallPlot.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/waterfallPlot.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/yellow_light.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/yellow_light.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/zip_file.png` & `pymodaq-4.0.3/src/pymodaq/resources/QtDesigner_Ressources/Icon_Library/zip_file.png`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/array_manipulation.py` & `pymodaq-4.0.3/src/pymodaq/utils/array_manipulation.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/calibration_camera.py` & `pymodaq-4.0.3/src/pymodaq/utils/calibration_camera.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/chrono_timer.py` & `pymodaq-4.0.3/src/pymodaq/utils/chrono_timer.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/config.py` & `pymodaq-4.0.3/src/pymodaq/utils/config.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/daq_utils.py` & `pymodaq-4.0.3/src/pymodaq/utils/daq_utils.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/data.py` & `pymodaq-4.0.3/src/pymodaq/utils/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,14 +118,18 @@
     scaling: float
         The scaling to apply to a linspace version in order to obtain the proper scaling
     offset: float
         The offset to apply to a linspace/scaled version in order to obtain the proper axis
     spread_order: int
         An integer needed in the case where data has a spread DataDistribution. It refers to the index along the data's
         spread_index dimension
+
+    Examples
+    --------
+    >>> axis = Axis('myaxis', units='seconds', data=np.array([1,2,3,4,5]), index=0)
     """
 
     def __init__(self, label: str = '', units: str = '', data: np.ndarray = None, index: int = 0, scaling=None,
                  offset=None, spread_order: int = None):
         super().__init__()
 
         self.iaxis: Axis = SpecialSlicersData(self, False)
@@ -461,14 +465,32 @@
     extra_attributes: List[str]
         list of string giving identifiers of the attributes added dynamically at the initialization (for instance
         to save extra metadata using the DataSaverLoader
 
     See Also
     --------
     DataWithAxes, DataFromPlugins, DataRaw, DataSaverLoader
+
+    Examples
+    --------
+    >>> import numpy as np
+    >>> from pymodaq.utils.data import DataBase, DataSource, DataDim, DataDistribution
+    >>> data = DataBase('mydata', source=DataSource['raw'], dim=DataDim['Data1D'], \
+distribution=DataDistribution['uniform'], data=[np.array([1.,2.,3.]), np.array([4.,5.,6.])],\
+labels=['channel1', 'channel2'], origin='docutils code')
+    >>> data.dim
+    <DataDim.Data1D: 1>
+    >>> data.source
+    <DataSource.raw: 0>
+    >>> data.shape
+    (3,)
+    >>> data.length
+    2
+    >>> data.size
+    3
     """
 
     def __init__(self, name: str, source: DataSource = None, dim: DataDim = None,
                  distribution: DataDistribution = DataDistribution['uniform'], data: List[np.ndarray] = None,
                  labels: List[str] = [], origin: str = None, **kwargs):
 
         super().__init__(name=name)
@@ -1470,16 +1492,14 @@
     def _am(self) -> AxesManagerBase:
         return self.axes_manager
 
     def get_data_dimension(self) -> str:
         return str(self._am)
 
 
-
-
 class DataRaw(DataWithAxes):
     """Specialized DataWithAxes set with source as 'raw'. To be used for raw data"""
     def __init__(self, *args,  **kwargs):
         if 'source' in kwargs:
             kwargs.pop('source')
         super().__init__(*args, source=DataSource['raw'], **kwargs)
 
@@ -1731,17 +1751,43 @@
         DataToExport: filtered with data matching the dimensionality
         """
         data = DataToExport(name=self.name)
         for dim in dims:
             data.append(self.get_data_from_dim(dim, deepcopy=deepcopy))
         return data
 
+    def get_data_from_sig_axes(self, Naxes: int, deepcopy: bool = False) -> DataToExport:
+        """Get the data matching the given number of signal axes
+
+        Parameters
+        ----------
+        Naxes: int
+            Number of signal axes in the DataWithAxes objects
+
+        Returns
+        -------
+        DataToExport: filtered with data matching the number of signal axes
+        """
+        data = DataToExport(name=self.name)
+        for _data in self:
+            if len(_data.sig_indexes) == Naxes:
+                if deepcopy:
+                    data.append(_data.deepcopy())
+                else:
+                    data.append(_data)
+        return data
+
     def get_data_from_Naxes(self, Naxes: int, deepcopy: bool = False) -> DataToExport:
         """Get the data matching the given number of axes
 
+        Parameters
+        ----------
+        Naxes: int
+            Number of axes in the DataWithAxes objects
+
         Returns
         -------
         DataToExport: filtered with data matching the number of axes
         """
         data = DataToExport(name=self.name)
         for _data in self:
             if len(_data.shape) == Naxes:
@@ -1815,14 +1861,17 @@
 
     @staticmethod
     def _check_data_type(data: DataWithAxes):
         """Make sure data is a DataWithAxes object or inherited"""
         if not isinstance(data, DataWithAxes):
             raise TypeError('Data stored in a DataToExport object should be objects inherited from DataWithAxis')
 
+    def deepcopy(self):
+        return DataToExport('Copy', data=[data.deepcopy() for data in self])
+
     @dispatch(list)
     def append(self, data: List[DataWithAxes]):
         for dat in data:
             self.append(dat)
 
     @dispatch(DataWithAxes)
     def append(self, data: DataWithAxes):
```

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/enums.py` & `pymodaq-4.0.3/src/pymodaq/utils/enums.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/exceptions.py` & `pymodaq-4.0.3/src/pymodaq/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/factory.py` & `pymodaq-4.0.3/src/pymodaq/utils/factory.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/logger.py` & `pymodaq-4.0.3/src/pymodaq/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/math_utils.py` & `pymodaq-4.0.3/src/pymodaq/utils/math_utils.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/messenger.py` & `pymodaq-4.0.3/src/pymodaq/utils/messenger.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/slicing.py` & `pymodaq-4.0.3/src/pymodaq/utils/slicing.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/tcp_server_client.py` & `pymodaq-4.0.3/src/pymodaq/utils/tcp_server_client.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/units.py` & `pymodaq-4.0.3/src/pymodaq/utils/units.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/Tuto innosetup/Tuto innosetup.odt` & `pymodaq-4.0.3/src/pymodaq/utils/Tuto innosetup/Tuto innosetup.odt`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/Tuto innosetup/Tuto innosetup.pdf` & `pymodaq-4.0.3/src/pymodaq/utils/Tuto innosetup/Tuto innosetup.pdf`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/Tuto innosetup/script_full_setup.iss` & `pymodaq-4.0.3/src/pymodaq/utils/Tuto innosetup/script_full_setup.iss`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/abstract/__init__.py` & `pymodaq-4.0.3/src/pymodaq/utils/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/abstract/logger.py` & `pymodaq-4.0.3/src/pymodaq/utils/abstract/logger.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/db/db_logger/db_logger.py` & `pymodaq-4.0.3/src/pymodaq/utils/db/db_logger/db_logger.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/db/db_logger/db_logger_models.py` & `pymodaq-4.0.3/src/pymodaq/utils/db/db_logger/db_logger_models.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/gui_utils/custom_app.py` & `pymodaq-4.0.3/src/pymodaq/utils/gui_utils/custom_app.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/gui_utils/dock.py` & `pymodaq-4.0.3/src/pymodaq/utils/gui_utils/dock.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/gui_utils/file_io.py` & `pymodaq-4.0.3/src/pymodaq/utils/gui_utils/file_io.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/gui_utils/layout.py` & `pymodaq-4.0.3/src/pymodaq/utils/gui_utils/layout.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/gui_utils/list_picker.py` & `pymodaq-4.0.3/src/pymodaq/utils/gui_utils/list_picker.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/gui_utils/utils.py` & `pymodaq-4.0.3/src/pymodaq/utils/gui_utils/utils.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/gui_utils/widgets/label.py` & `pymodaq-4.0.3/src/pymodaq/utils/gui_utils/widgets/label.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/gui_utils/widgets/lcd.py` & `pymodaq-4.0.3/src/pymodaq/utils/gui_utils/widgets/lcd.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/gui_utils/widgets/push.py` & `pymodaq-4.0.3/src/pymodaq/utils/gui_utils/widgets/push.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/gui_utils/widgets/qled.py` & `pymodaq-4.0.3/src/pymodaq/utils/gui_utils/widgets/qled.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/gui_utils/widgets/spinbox.py` & `pymodaq-4.0.3/src/pymodaq/utils/gui_utils/widgets/spinbox.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/gui_utils/widgets/table.py` & `pymodaq-4.0.3/src/pymodaq/utils/gui_utils/widgets/table.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/h5modules/backends.py` & `pymodaq-4.0.3/src/pymodaq/utils/h5modules/backends.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/h5modules/browsing.py` & `pymodaq-4.0.3/src/pymodaq/utils/h5modules/browsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 from pymodaq.utils import daq_utils as utils
 from pymodaq.utils.managers.action_manager import ActionManager
 from pymodaq.utils.managers.parameter_manager import ParameterManager
 from pymodaq.utils.messenger import messagebox
 from .backends import H5Backend
 from .saving import H5Saver
 from . import data_saving
-from .utils import find_scan_node, get_h5_attributes
 from .exporter import ExporterFactory
 
 config = Config()
 logger = set_logger(get_module_name(__file__))
 
 
 class H5BrowserUtil(H5Backend):
@@ -89,17 +88,40 @@
             if 'pixmap2D' in node.attrs:
                 scan_list.append(
                     dict(scan_name='{:s}_{:s}'.format(node.parent_node.name, node.name), path=node.path,
                          data=node.attrs['pixmap2D']))
 
         return scan_list
 
-    @staticmethod
-    def get_h5_attributes(node_path):
-        return get_h5_attributes(node_path)
+    def get_h5_attributes(self, node_path):
+        """
+        """
+        node = self.get_node(node_path)
+        attrs_names = node.attrs.attrs_name
+        attr_dict = OrderedDict([])
+        for attr in attrs_names:
+            # if attr!='settings':
+            attr_dict[attr] = node.attrs[attr]
+
+        settings = None
+        scan_settings = None
+        if 'settings' in attrs_names:
+            if node.attrs['settings'] != '':
+                settings = node.attrs['settings']
+
+        if 'scan_settings' in attrs_names:
+            if node.attrs['scan_settings'] != '':
+                scan_settings = node.attrs['scan_settings']
+        pixmaps = []
+        for attr in attrs_names:
+            if 'pixmap' in attr:
+                pixmaps.append(node.attrs[attr])
+
+        return attr_dict, settings, scan_settings, pixmaps
+
 
 class View(QObject):
     item_clicked_sig = Signal(object)
     item_double_clicked_sig = Signal(object)
     
     def __init__(self, widget: QtWidgets.QWidget, settings_tree, settings_attributes_tree):
         super().__init__()
```

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/h5modules/data_saving.py` & `pymodaq-4.0.3/src/pymodaq/utils/h5modules/data_saving.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/h5modules/exporter.py` & `pymodaq-4.0.3/src/pymodaq/utils/h5modules/exporter.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/h5modules/h5logging.py` & `pymodaq-4.0.3/src/pymodaq/utils/h5modules/h5logging.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/h5modules/module_saving.py` & `pymodaq-4.0.3/src/pymodaq/utils/h5modules/module_saving.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     group_type: GroupType = abstract_attribute()
     _module = abstract_attribute()
     _h5saver: H5SaverLowLevel = abstract_attribute()
     _module_group: GROUP = abstract_attribute()
     main_module = True
 
     def get_set_node(self, where: Union[Node, str] = None, name: str = None) -> GROUP:
-        """Get the node corresponding to this particular Module instance
+        """Get or create the node corresponding to this particular Module instance
 
         Parameters
         ----------
         where: Union[Node, str]
             the path of a given node or the node itself
         new: bool
             if True force the creation of a new indexed node of this class type
@@ -168,14 +168,27 @@
         return self._h5saver.add_det_group(where, title=self._module.title, settings_as_xml=ET.tostring(settings_xml),
                                            metadata=metadata)
 
     def add_data(self, where: Union[Node, str], data: DataToExport):
         self._datatoexport_saver.add_data(where, data)
 
     def add_bkg(self, where: Union[Node, str], data_bkg: DataToExport):
+        """ Adds a DataToExport as a background node in the h5file
+
+        Parameters
+        ----------
+        where: Union[Node, str]
+            the path of a given node or the node itself
+        data_bkg: DataToExport
+            The data to be saved as background
+
+        Returns
+        -------
+
+        """
         self._datatoexport_saver.add_bkg(where, data_bkg)
 
     def add_external_h5(self, other_h5data: H5SaverLowLevel):
         if other_h5data is not None:
             external_group = self._h5saver.add_group('external_data', 'external_h5', self.module_group)
             try:
                 if not other_h5data.isopen:
```

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/h5modules/saving.py` & `pymodaq-4.0.3/src/pymodaq/utils/h5modules/saving.py`

 * *Files 4% similar despite different names*

```diff
@@ -800,51 +800,14 @@
 
     def save_file(self, filename=None):
         if filename is None:
             filename = select_file(None, save=True, ext='h5')
         if filename != '':
             super().save_file_as(filename)
 
-
-    # def add_data_live_scan(self, channel_group, data_dict, scan_type='scan1D', title='', scan_subtype=''):
-    #     isadaptive = scan_subtype == 'Adaptive'
-    #     if not isadaptive:
-    #         shape, dimension, size = utils.get_data_dimension(data_dict['data'], scan_type=scan_type,
-    #                                                           remove_scan_dimension=True)
-    #     else:
-    #         shape, dimension, size = data_dict['data'].shape, '0D', 1
-    #     data_array = self.add_array(channel_group, 'Data', 'data', array_type=np.float,
-    #                                 title=title,
-    #                                 data_shape=shape,
-    #                                 data_dimension=dimension, scan_type=scan_type,
-    #                                 scan_subtype=scan_subtype,
-    #                                 array_to_save=data_dict['data'])
-    #     if 'x_axis' in data_dict:
-    #         if not isinstance(data_dict['x_axis'], dict):
-    #             array_to_save = data_dict['x_axis']
-    #             tmp_dict = dict(label='', units='')
-    #         else:
-    #             tmp_dict = copy.deepcopy(data_dict['x_axis'])
-    #             array_to_save = tmp_dict.pop('data')
-    #         self.add_array(channel_group, 'x_axis', 'axis',
-    #                        array_type=np.float, array_to_save=array_to_save,
-    #                        enlargeable=False, data_dimension='1D', metadata=tmp_dict)
-    #     if 'y_axis' in data_dict:
-    #         if not isinstance(data_dict['y_axis'], dict):
-    #             array_to_save = data_dict['y_axis']
-    #             tmp_dict = dict(label='', units='')
-    #         else:
-    #             tmp_dict = copy.deepcopy(data_dict['y_axis'])
-    #             array_to_save = tmp_dict.pop('data')
-    #         self.add_array(channel_group, 'y_axis', 'axis',
-    #                        array_type=np.float, array_to_save=array_to_save,
-    #                        enlargeable=False, data_dimension='1D', metadata=tmp_dict)
-    #     return data_array
-
-
     def value_changed(self, param):
         if param.name() == 'show_file':
             param.setValue(False)
             self.show_file_content()
 
         elif param.name() == 'base_path':
             try:
```

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/h5modules/utils.py` & `pymodaq-4.0.3/src/pymodaq/utils/h5modules/utils.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/h5modules/exporters/base.py` & `pymodaq-4.0.3/src/pymodaq/utils/h5modules/exporters/base.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/h5modules/exporters/flimj.py` & `pymodaq-4.0.3/src/pymodaq/utils/h5modules/exporters/flimj.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/h5modules/exporters/hyperspy.py` & `pymodaq-4.0.3/src/pymodaq/utils/h5modules/exporters/hyperspy.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/managers/action_manager.py` & `pymodaq-4.0.3/src/pymodaq/utils/managers/action_manager.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/managers/batchscan_manager.py` & `pymodaq-4.0.3/src/pymodaq/utils/managers/batchscan_manager.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/managers/modules_manager.py` & `pymodaq-4.0.3/src/pymodaq/utils/managers/modules_manager.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/managers/overshoot_manager.py` & `pymodaq-4.0.3/src/pymodaq/utils/managers/overshoot_manager.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/managers/parameter_manager.py` & `pymodaq-4.0.3/src/pymodaq/utils/managers/parameter_manager.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/managers/preset_manager.py` & `pymodaq-4.0.3/src/pymodaq/utils/managers/preset_manager.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/managers/preset_manager_utils.py` & `pymodaq-4.0.3/src/pymodaq/utils/managers/preset_manager_utils.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/managers/remote_manager.py` & `pymodaq-4.0.3/src/pymodaq/utils/managers/remote_manager.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/managers/roi_manager.py` & `pymodaq-4.0.3/src/pymodaq/utils/managers/roi_manager.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/parameter/ioxml.py` & `pymodaq-4.0.3/src/pymodaq/utils/parameter/ioxml.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/parameter/utils.py` & `pymodaq-4.0.3/src/pymodaq/utils/parameter/utils.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/__init__.py` & `pymodaq-4.0.3/src/pymodaq/utils/parameter/pymodaq_ptypes/__init__.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/bool.py` & `pymodaq-4.0.3/src/pymodaq/utils/parameter/pymodaq_ptypes/bool.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/date.py` & `pymodaq-4.0.3/src/pymodaq/utils/parameter/pymodaq_ptypes/date.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/filedir.py` & `pymodaq-4.0.3/src/pymodaq/utils/parameter/pymodaq_ptypes/filedir.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/itemselect.py` & `pymodaq-4.0.3/src/pymodaq/utils/parameter/pymodaq_ptypes/itemselect.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/led.py` & `pymodaq-4.0.3/src/pymodaq/utils/parameter/pymodaq_ptypes/led.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/list.py` & `pymodaq-4.0.3/src/pymodaq/utils/parameter/pymodaq_ptypes/list.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/numeric.py` & `pymodaq-4.0.3/src/pymodaq/utils/parameter/pymodaq_ptypes/numeric.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/pixmap.py` & `pymodaq-4.0.3/src/pymodaq/utils/parameter/pymodaq_ptypes/pixmap.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/slide.py` & `pymodaq-4.0.3/src/pymodaq/utils/parameter/pymodaq_ptypes/slide.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/table.py` & `pymodaq-4.0.3/src/pymodaq/utils/parameter/pymodaq_ptypes/table.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/tableview.py` & `pymodaq-4.0.3/src/pymodaq/utils/parameter/pymodaq_ptypes/tableview.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/parameter/pymodaq_ptypes/text.py` & `pymodaq-4.0.3/src/pymodaq/utils/parameter/pymodaq_ptypes/text.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/plotting/gant_chart.py` & `pymodaq-4.0.3/src/pymodaq/utils/plotting/gant_chart.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/plotting/image_viewer.py` & `pymodaq-4.0.3/src/pymodaq/utils/plotting/image_viewer.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/plotting/navigator.py` & `pymodaq-4.0.3/src/pymodaq/utils/plotting/navigator.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/plotting/scan_selector.py` & `pymodaq-4.0.3/src/pymodaq/utils/plotting/scan_selector.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/plotting/widgets.py` & `pymodaq-4.0.3/src/pymodaq/utils/plotting/widgets.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/plotting/data_viewers/viewer.py` & `pymodaq-4.0.3/src/pymodaq/utils/plotting/data_viewers/viewer.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/plotting/data_viewers/viewer0D.py` & `pymodaq-4.0.3/src/pymodaq/utils/plotting/data_viewers/viewer0D.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/plotting/data_viewers/viewer1D.py` & `pymodaq-4.0.3/src/pymodaq/utils/plotting/data_viewers/viewer1D.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/plotting/data_viewers/viewer1Dbasic.py` & `pymodaq-4.0.3/src/pymodaq/utils/plotting/data_viewers/viewer1Dbasic.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/plotting/data_viewers/viewer2D.py` & `pymodaq-4.0.3/src/pymodaq/utils/plotting/data_viewers/viewer2D.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/plotting/data_viewers/viewer2D_basic.py` & `pymodaq-4.0.3/src/pymodaq/utils/plotting/data_viewers/viewer2D_basic.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/plotting/data_viewers/viewerND.py` & `pymodaq-4.0.3/src/pymodaq/utils/plotting/data_viewers/viewerND.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/plotting/items/axis_scaled.py` & `pymodaq-4.0.3/src/pymodaq/utils/plotting/items/axis_scaled.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/plotting/items/crosshair.py` & `pymodaq-4.0.3/src/pymodaq/utils/plotting/items/crosshair.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/plotting/items/image.py` & `pymodaq-4.0.3/src/pymodaq/utils/plotting/items/image.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/plotting/utils/axes_viewer.py` & `pymodaq-4.0.3/src/pymodaq/utils/plotting/utils/axes_viewer.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/plotting/utils/filter.py` & `pymodaq-4.0.3/src/pymodaq/utils/plotting/utils/filter.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/plotting/utils/lineout.py` & `pymodaq-4.0.3/src/pymodaq/utils/plotting/utils/lineout.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/plotting/utils/plot_utils.py` & `pymodaq-4.0.3/src/pymodaq/utils/plotting/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/plotting/utils/signalND.py` & `pymodaq-4.0.3/src/pymodaq/utils/plotting/utils/signalND.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/scanner/scanner.py` & `pymodaq-4.0.3/src/pymodaq/utils/scanner/scanner.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/scanner/utils.py` & `pymodaq-4.0.3/src/pymodaq/utils/scanner/utils.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/scanner/scanners/_1d_scanners.py` & `pymodaq-4.0.3/src/pymodaq/utils/scanner/scanners/_1d_scanners.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/scanner/scanners/_2d_scanners.py` & `pymodaq-4.0.3/src/pymodaq/utils/scanner/scanners/_2d_scanners.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
                'value': config('scan', 'scan2D', 'linear', 'stop2')},
               ]
     n_axes = 2
     distribution = DataDistribution['uniform']
 
     def __init__(self, actuators: List = None, **_ignored):
         super().__init__(actuators=actuators)
+        self.axes_unique = []
 
     def get_pos(self):
         starts = np.array([self.settings['start_axis1'], self.settings['start_axis2']])
         stops = np.array([self.settings['stop_axis1'], self.settings['stop_axis2']])
         steps = np.array([self.settings['step_axis1'], self.settings['step_axis2']])
         return starts, stops, steps
```

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/scanner/scanners/sequential.py` & `pymodaq-4.0.3/src/pymodaq/utils/scanner/scanners/sequential.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/scanner/scanners/tabular.py` & `pymodaq-4.0.3/src/pymodaq/utils/scanner/scanners/tabular.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/svg/svg_view.py` & `pymodaq-4.0.3/src/pymodaq/utils/svg/svg_view.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/svg/svg_viewer2D.py` & `pymodaq-4.0.3/src/pymodaq/utils/svg/svg_viewer2D.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/src/pymodaq/utils/tree_layout/tree_layout_main.py` & `pymodaq-4.0.3/src/pymodaq/utils/tree_layout/tree_layout_main.py`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/.gitignore` & `pymodaq-4.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/LICENSE` & `pymodaq-4.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/README.rst` & `pymodaq-4.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `pymodaq-4.0.2/pyproject.toml` & `pymodaq-4.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering :: Human Machine Interfaces",
     "Topic :: Scientific/Engineering :: Visualization",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: User Interfaces",
 ]
 dependencies = [
-    "docutils==0.17.1",
+    #"docutils==0.17.1",
     "easydict",
     "importlib_metadata; python_version<\"3.8\"",
     "multipledispatch",
     "numpy",
     "packaging",
     "pint",
     "pymodaq_plugin_manager>=0.0.17",
```

### Comparing `pymodaq-4.0.2/PKG-INFO` & `pymodaq-4.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodaq
-Version: 4.0.2
+Version: 4.0.3
 Summary: Modular Data Acquisition with Python
 Project-URL: Homepage, http://pymodaq.cnrs.fr
 Project-URL: Source, https://github.com/PyMoDAQ/PyMoDAQ
 Project-URL: Tracker, https://github.com/PyMoDAQ/PyMoDAQ/issues
 Author-email: Sébastien Weber <sebastien.weber@cemes.fr>
 License: The MIT License (MIT)
         
@@ -40,15 +40,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: User Interfaces
 Requires-Python: >=3.7
-Requires-Dist: docutils==0.17.1
 Requires-Dist: easydict
 Requires-Dist: importlib-metadata; python_version < '3.8'
 Requires-Dist: multipledispatch
 Requires-Dist: numpy
 Requires-Dist: packaging
 Requires-Dist: pint
 Requires-Dist: pymodaq-plugin-manager>=0.0.17
```

