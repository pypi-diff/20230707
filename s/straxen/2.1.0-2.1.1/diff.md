# Comparing `tmp/straxen-2.1.0.tar.gz` & `tmp/straxen-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "straxen-2.1.0.tar", last modified: Thu Jun 22 19:23:06 2023, max compression
+gzip compressed data, was "straxen-2.1.1.tar", last modified: Fri Jul  7 03:53:00 2023, max compression
```

## Comparing `straxen-2.1.0.tar` & `straxen-2.1.1.tar`

### file list

```diff
@@ -1,242 +1,242 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.976051 straxen-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    40334 2023-06-22 19:23:01.000000 straxen-2.1.0/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-22 19:23:01.000000 straxen-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-22 19:23:01.000000 straxen-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    53024 2023-06-22 19:23:06.976051 straxen-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-22 19:23:01.000000 straxen-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.956050 straxen-2.1.0/bin/
--rw-r--r--   0 runner    (1001) docker     (123)    37235 2023-06-22 19:23:01.000000 straxen-2.1.0/bin/ajax
--rwxr-xr-x   0 runner    (1001) docker     (123)    67099 2023-06-22 19:23:01.000000 straxen-2.1.0/bin/bootstrax
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-06-22 19:23:01.000000 straxen-2.1.0/bin/fake_daq
--rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-06-22 19:23:01.000000 straxen-2.1.0/bin/microstrax
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-06-22 19:23:01.000000 straxen-2.1.0/bin/refresh_raw_records
--rw-r--r--   0 runner    (1001) docker     (123)    35964 2023-06-22 19:23:01.000000 straxen-2.1.0/bin/restrax
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-22 19:23:01.000000 straxen-2.1.0/bin/straxen-print_versions
--rw-r--r--   0 runner    (1001) docker     (123)    12241 2023-06-22 19:23:01.000000 straxen-2.1.0/bin/straxer
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.956050 straxen-2.1.0/extra_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-22 19:23:01.000000 straxen-2.1.0/extra_requirements/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-22 19:23:01.000000 straxen-2.1.0/extra_requirements/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-22 19:23:01.000000 straxen-2.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-22 19:23:06.976051 straxen-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-22 19:23:01.000000 straxen-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.960050 straxen-2.1.0/straxen/
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.960050 straxen-2.1.0/straxen/analyses/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/analyses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38941 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/analyses/bokeh_waveform_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/analyses/daq_waveforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    18579 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/analyses/event_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    17242 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/analyses/holoviews_waveform_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/analyses/posrec_comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/analyses/pulse_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/analyses/quick_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/analyses/records_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    10245 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/analyses/waveform_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/bokeh_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21032 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    22966 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)    18385 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/corrections_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/daq_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     8203 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/get_corrections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.960050 straxen-2.1.0/straxen/holoviews/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/holoviews/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/holoviews/holoviews_inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)    13244 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/holoviews/holoviews_peak_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/holoviews/holoviews_pmt_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    17711 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/holoviews/holoviews_tpc_event_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    21799 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/holoviews_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10806 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/itp_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.960050 straxen-2.1.0/straxen/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/legacy/contexts_1t.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/legacy/hitfinder_thresholds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.964051 straxen-2.1.0/straxen/legacy/plugins_1t/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/legacy/plugins_1t/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/legacy/plugins_1t/event_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/legacy/plugins_1t/pax_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/legacy/plugins_1t/peak_positions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10186 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/legacy/plugins_1t/x1t_cuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/legacy/xenon1t_url_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/matplotlib_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/mini_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/numbafied_scipy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.964051 straxen-2.1.0/straxen/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.964051 straxen-2.1.0/straxen/plugins/afterpulses/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/afterpulses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11243 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/afterpulses/afterpulse_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.964051 straxen-2.1.0/straxen/plugins/aqmon_hits/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/aqmon_hits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/aqmon_hits/aqmon_hits.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.964051 straxen-2.1.0/straxen/plugins/detector_time_offsets/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/detector_time_offsets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/detector_time_offsets/detector_time_offsets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.964051 straxen-2.1.0/straxen/plugins/events/
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/_event_s1_positions_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/_event_s2_positions_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/corrected_areas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/distinct_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/energy_estimates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/event_ambience.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/event_area_per_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)    16617 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/event_basics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/event_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/event_info_double.py
--rw-r--r--   0 runner    (1001) docker     (123)    25160 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/event_pattern_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/event_positions.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/event_s1_positions_cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/event_s2_positions_cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/event_s2_positions_gcn.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/event_s2_positions_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/event_shadow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/event_top_bottom_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/event_w_bayes_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/event_waveform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/local_minimum_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/multi_scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/s2_recon_pos_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/veto_proximity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.964051 straxen-2.1.0/straxen/plugins/events_mv/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events_mv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events_mv/events_mv.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events_mv/events_sync_mv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.968051 straxen-2.1.0/straxen/plugins/events_nv/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events_nv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events_nv/event_positions_nv.py
--rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events_nv/events_nv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events_nv/events_sync_nv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.968051 straxen-2.1.0/straxen/plugins/hitlets_mv/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/hitlets_mv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/hitlets_mv/hitlets_mv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.968051 straxen-2.1.0/straxen/plugins/hitlets_nv/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/hitlets_nv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/hitlets_nv/hitlets_nv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.968051 straxen-2.1.0/straxen/plugins/individual_peak_monitor/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/individual_peak_monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/individual_peak_monitor/individual_peak_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.968051 straxen-2.1.0/straxen/plugins/led_cal/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/led_cal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/led_cal/led_calibration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.968051 straxen-2.1.0/straxen/plugins/merged_s2s/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/merged_s2s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/merged_s2s/merged_s2s.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.968051 straxen-2.1.0/straxen/plugins/merged_s2s_he/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/merged_s2s_he/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/merged_s2s_he/merged_s2s_he.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.968051 straxen-2.1.0/straxen/plugins/online_monitor_mv/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/online_monitor_mv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/online_monitor_mv/online_monitor_mv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.968051 straxen-2.1.0/straxen/plugins/online_monitor_nv/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/online_monitor_nv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/online_monitor_nv/online_monitor_nv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.968051 straxen-2.1.0/straxen/plugins/online_peak_monitor/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/online_peak_monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/online_peak_monitor/online_peak_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.968051 straxen-2.1.0/straxen/plugins/peaklets/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaklets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaklets/peaklet_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    25757 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaklets/peaklets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.968051 straxen-2.1.0/straxen/plugins/peaklets_he/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaklets_he/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaklets_he/peaklet_classification_he.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaklets_he/peaklets_he.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.968051 straxen-2.1.0/straxen/plugins/peaks/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaks/_peak_positions_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaks/_peak_s1_positions_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaks/peak_ambience.py
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaks/peak_basics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaks/peak_classification_bayes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaks/peak_corrections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaks/peak_per_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaks/peak_positions.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaks/peak_positions_cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaks/peak_positions_gcn.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaks/peak_positions_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaks/peak_proximity.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaks/peak_s1_positions_cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaks/peak_shadow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaks/peak_top_bottom_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaks/peaks.py
--rw-r--r--   0 runner    (1001) docker     (123)    13029 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaks/peaks_subtyping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.972051 straxen-2.1.0/straxen/plugins/peaks_he/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaks_he/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaks_he/peak_basics_he.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaks_he/peaks_he.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.972051 straxen-2.1.0/straxen/plugins/raw_records/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/raw_records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16653 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/raw_records/daqreader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.972051 straxen-2.1.0/straxen/plugins/raw_records_coin_nv/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/raw_records_coin_nv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19659 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/raw_records_coin_nv/nveto_recorder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.972051 straxen-2.1.0/straxen/plugins/records/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17703 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/records/records.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.972051 straxen-2.1.0/straxen/plugins/records_he/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/records_he/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/records_he/records_he.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.972051 straxen-2.1.0/straxen/plugins/records_mv/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/records_mv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/records_mv/records_mv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.972051 straxen-2.1.0/straxen/plugins/records_nv/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/records_nv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/records_nv/records_nv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.972051 straxen-2.1.0/straxen/plugins/veto_intervals/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/veto_intervals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/veto_intervals/veto_intervals.py
--rw-r--r--   0 runner    (1001) docker     (123)    27943 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/scada.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.972051 straxen-2.1.0/straxen/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15115 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/storage/mongo_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/storage/online_monitor_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/storage/rucio_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/storage/rucio_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)    13251 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/storage/rundb.py
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/units.py
--rw-r--r--   0 runner    (1001) docker     (123)    25161 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/url_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.960050 straxen-2.1.0/straxen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    53024 2023-06-22 19:23:06.000000 straxen-2.1.0/straxen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-06-22 19:23:06.000000 straxen-2.1.0/straxen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 19:23:06.000000 straxen-2.1.0/straxen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 19:23:06.000000 straxen-2.1.0/straxen.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-22 19:23:06.000000 straxen-2.1.0/straxen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-22 19:23:06.000000 straxen-2.1.0/straxen.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.976051 straxen-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.976051 straxen-2.1.0/tests/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9751 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/storage/test_database_frontends.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/storage/test_mongo_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/storage/test_mongo_interactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/storage/test_rucio_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/storage/test_rucio_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_1T_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)    10536 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_aqmon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_channel_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_cmt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_count_pulses.py
--rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_daq_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_holoviews_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_itp_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_led_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)    17347 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_mini_analyses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9765 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_nveto_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_nveto_recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_patternfit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_peaklet_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_peaks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_scada.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_testing_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)    15506 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_url_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_veto_hitlets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.505946 straxen-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    40896 2023-07-07 03:52:57.000000 straxen-2.1.1/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-07 03:52:57.000000 straxen-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-07 03:52:57.000000 straxen-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    53674 2023-07-07 03:53:00.505946 straxen-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-07-07 03:52:57.000000 straxen-2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.485943 straxen-2.1.1/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)    37235 2023-07-07 03:52:57.000000 straxen-2.1.1/bin/ajax
+-rwxr-xr-x   0 runner    (1001) docker     (123)    67099 2023-07-07 03:52:57.000000 straxen-2.1.1/bin/bootstrax
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-07-07 03:52:57.000000 straxen-2.1.1/bin/fake_daq
+-rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-07-07 03:52:57.000000 straxen-2.1.1/bin/microstrax
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-07-07 03:52:57.000000 straxen-2.1.1/bin/refresh_raw_records
+-rw-r--r--   0 runner    (1001) docker     (123)    35964 2023-07-07 03:52:57.000000 straxen-2.1.1/bin/restrax
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-07 03:52:57.000000 straxen-2.1.1/bin/straxen-print_versions
+-rw-r--r--   0 runner    (1001) docker     (123)    12241 2023-07-07 03:52:57.000000 straxen-2.1.1/bin/straxer
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.485943 straxen-2.1.1/extra_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-07 03:52:57.000000 straxen-2.1.1/extra_requirements/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-07 03:52:57.000000 straxen-2.1.1/extra_requirements/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-07 03:52:57.000000 straxen-2.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-07 03:53:00.509946 straxen-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-07 03:52:57.000000 straxen-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.485943 straxen-2.1.1/straxen/
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.489944 straxen-2.1.1/straxen/analyses/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/analyses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38941 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/analyses/bokeh_waveform_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/analyses/daq_waveforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18579 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/analyses/event_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17242 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/analyses/holoviews_waveform_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/analyses/posrec_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/analyses/pulse_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/analyses/quick_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/analyses/records_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10245 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/analyses/waveform_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/bokeh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21032 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22966 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18385 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/corrections_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/daq_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8203 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/get_corrections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.489944 straxen-2.1.1/straxen/holoviews/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/holoviews/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/holoviews/holoviews_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13244 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/holoviews/holoviews_peak_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/holoviews/holoviews_pmt_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17711 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/holoviews/holoviews_tpc_event_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21799 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/holoviews_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10806 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/itp_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.489944 straxen-2.1.1/straxen/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/legacy/contexts_1t.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/legacy/hitfinder_thresholds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.489944 straxen-2.1.1/straxen/legacy/plugins_1t/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/legacy/plugins_1t/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/legacy/plugins_1t/event_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/legacy/plugins_1t/pax_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/legacy/plugins_1t/peak_positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10186 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/legacy/plugins_1t/x1t_cuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/legacy/xenon1t_url_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/matplotlib_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/mini_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/numbafied_scipy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.489944 straxen-2.1.1/straxen/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.489944 straxen-2.1.1/straxen/plugins/afterpulses/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/afterpulses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11243 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/afterpulses/afterpulse_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.493944 straxen-2.1.1/straxen/plugins/aqmon_hits/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/aqmon_hits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/aqmon_hits/aqmon_hits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.493944 straxen-2.1.1/straxen/plugins/detector_time_offsets/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/detector_time_offsets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/detector_time_offsets/detector_time_offsets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.493944 straxen-2.1.1/straxen/plugins/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/_event_s1_positions_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/_event_s2_positions_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/corrected_areas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/distinct_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/energy_estimates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/event_ambience.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/event_area_per_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16617 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/event_basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/event_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/event_info_double.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25160 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/event_pattern_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/event_positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/event_s1_positions_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/event_s2_positions_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/event_s2_positions_gcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/event_s2_positions_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/event_shadow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/event_top_bottom_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/event_w_bayes_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/event_waveform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/local_minimum_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/multi_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/s2_recon_pos_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events/veto_proximity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.493944 straxen-2.1.1/straxen/plugins/events_mv/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events_mv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events_mv/events_mv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events_mv/events_sync_mv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.497945 straxen-2.1.1/straxen/plugins/events_nv/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events_nv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events_nv/event_positions_nv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events_nv/events_nv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/events_nv/events_sync_nv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.497945 straxen-2.1.1/straxen/plugins/hitlets_mv/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/hitlets_mv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/hitlets_mv/hitlets_mv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.497945 straxen-2.1.1/straxen/plugins/hitlets_nv/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/hitlets_nv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/hitlets_nv/hitlets_nv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.497945 straxen-2.1.1/straxen/plugins/individual_peak_monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/individual_peak_monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/individual_peak_monitor/individual_peak_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.497945 straxen-2.1.1/straxen/plugins/led_cal/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/led_cal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/led_cal/led_calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.497945 straxen-2.1.1/straxen/plugins/merged_s2s/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/merged_s2s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/merged_s2s/merged_s2s.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.497945 straxen-2.1.1/straxen/plugins/merged_s2s_he/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/merged_s2s_he/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/merged_s2s_he/merged_s2s_he.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.497945 straxen-2.1.1/straxen/plugins/online_monitor_mv/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/online_monitor_mv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/online_monitor_mv/online_monitor_mv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.497945 straxen-2.1.1/straxen/plugins/online_monitor_nv/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/online_monitor_nv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/online_monitor_nv/online_monitor_nv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.497945 straxen-2.1.1/straxen/plugins/online_peak_monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/online_peak_monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/online_peak_monitor/online_peak_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.497945 straxen-2.1.1/straxen/plugins/peaklets/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaklets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaklets/peaklet_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25757 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaklets/peaklets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.497945 straxen-2.1.1/straxen/plugins/peaklets_he/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaklets_he/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaklets_he/peaklet_classification_he.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaklets_he/peaklets_he.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.501945 straxen-2.1.1/straxen/plugins/peaks/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaks/_peak_positions_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaks/_peak_s1_positions_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7904 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaks/peak_ambience.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaks/peak_basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaks/peak_classification_bayes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaks/peak_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaks/peak_per_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaks/peak_positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaks/peak_positions_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaks/peak_positions_gcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaks/peak_positions_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaks/peak_proximity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaks/peak_s1_positions_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9637 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaks/peak_shadow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaks/peak_top_bottom_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaks/peaks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13029 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaks/peaks_subtyping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.501945 straxen-2.1.1/straxen/plugins/peaks_he/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaks_he/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaks_he/peak_basics_he.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/peaks_he/peaks_he.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.501945 straxen-2.1.1/straxen/plugins/raw_records/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/raw_records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16653 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/raw_records/daqreader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.501945 straxen-2.1.1/straxen/plugins/raw_records_coin_nv/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/raw_records_coin_nv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19659 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/raw_records_coin_nv/nveto_recorder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.501945 straxen-2.1.1/straxen/plugins/records/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17703 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/records/records.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.501945 straxen-2.1.1/straxen/plugins/records_he/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/records_he/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/records_he/records_he.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.501945 straxen-2.1.1/straxen/plugins/records_mv/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/records_mv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/records_mv/records_mv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.501945 straxen-2.1.1/straxen/plugins/records_nv/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/records_nv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/records_nv/records_nv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.501945 straxen-2.1.1/straxen/plugins/veto_intervals/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/veto_intervals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/plugins/veto_intervals/veto_intervals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27943 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/scada.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.501945 straxen-2.1.1/straxen/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15115 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/storage/mongo_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/storage/online_monitor_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/storage/rucio_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/storage/rucio_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13251 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/storage/rundb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25282 2023-07-07 03:52:57.000000 straxen-2.1.1/straxen/url_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.489944 straxen-2.1.1/straxen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    53674 2023-07-07 03:53:00.000000 straxen-2.1.1/straxen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-07-07 03:53:00.000000 straxen-2.1.1/straxen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 03:53:00.000000 straxen-2.1.1/straxen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 03:53:00.000000 straxen-2.1.1/straxen.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-07 03:53:00.000000 straxen-2.1.1/straxen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-07 03:53:00.000000 straxen-2.1.1/straxen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.505946 straxen-2.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:53:00.505946 straxen-2.1.1/tests/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9751 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/storage/test_database_frontends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/storage/test_mongo_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/storage/test_mongo_interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/storage/test_rucio_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/storage/test_rucio_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_1T_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10536 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_aqmon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_channel_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_cmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_count_pulses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_daq_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_holoviews_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_itp_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_led_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17347 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_mini_analyses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9765 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_nveto_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_nveto_recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_patternfit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_peaklet_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_peaks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_scada.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_testing_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15506 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_url_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-07 03:52:57.000000 straxen-2.1.1/tests/test_veto_hitlets.py
```

### Comparing `straxen-2.1.0/HISTORY.md` & `straxen-2.1.1/HISTORY.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,19 @@
-v2.1.70 / 2023-06-22
+v2.1.1 / 2023-07-06
+-------------------
+* Fix timing of peaks when ordering in `center_time` by @dachengx in https://github.com/XENONnT/straxen/pull/1208
+* Move `get_window_size` factor of merged_s2s as untracked configuration by @dachengx in https://github.com/XENONnT/straxen/pull/1209
+* Sort `hitlets` in `nVETOHitlets` by @dachengx in https://github.com/XENONnT/straxen/pull/1210
+* Only print out warning once by @LuisSanchez25 in https://github.com/XENONnT/straxen/pull/1211
+
+
+**Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.1.0...v2.1.1
+
+
+v2.1.0 / 2023-06-22
 -------------------
 * Added peaks subtyping by @Jianyu010 in https://github.com/XENONnT/straxen/pull/1152
 * Fix ipython version by @dachengx in https://github.com/XENONnT/straxen/pull/1169
 * Fix bug in hitlets time ordering by @dachengx in https://github.com/XENONnT/straxen/pull/1173
 * Bump actions/setup-python from 4.5.0 to 4.6.0 by @dependabot in https://github.com/XENONnT/straxen/pull/1170
 * Save hits level information(hits height and time difference) in peak and event level by @dachengx in https://github.com/XENONnT/straxen/pull/1155
 * Fix argsort inside numba.jit using kind='mergesort' by @dachengx in https://github.com/XENONnT/straxen/pull/1176
```

### Comparing `straxen-2.1.0/LICENSE` & `straxen-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/PKG-INFO` & `straxen-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: straxen
-Version: 2.1.0
+Version: 2.1.1
 Summary: Streaming analysis for XENON
 Home-page: https://github.com/XENONnT/straxen
 Author: Straxen contributors, the XENON collaboration
 License: UNKNOWN
 Description: # straxen
         Streaming analysis for XENON(nT)
         
@@ -25,15 +25,26 @@
         [![Python Versions](https://img.shields.io/pypi/pyversions/straxen.svg)](https://pypi.python.org/pypi/straxen)
         [![PyPI downloads](https://img.shields.io/pypi/dm/straxen.svg)](https://pypistats.org/packages/straxen)
         
         [![Update context collection](https://github.com/XENONnT/straxen/workflows/Update%20context%20collection/badge.svg)](https://github.com/XENONnT/straxen/actions/workflows/contexts.yml)
         [![Python style](https://github.com/XENONnT/straxen/actions/workflows/code_style.yml/badge.svg)](https://github.com/XENONnT/straxen/actions/workflows/code_style.yml)
         
         
-        v2.1.70 / 2023-06-22
+        v2.1.1 / 2023-07-06
+        -------------------
+        * Fix timing of peaks when ordering in `center_time` by @dachengx in https://github.com/XENONnT/straxen/pull/1208
+        * Move `get_window_size` factor of merged_s2s as untracked configuration by @dachengx in https://github.com/XENONnT/straxen/pull/1209
+        * Sort `hitlets` in `nVETOHitlets` by @dachengx in https://github.com/XENONnT/straxen/pull/1210
+        * Only print out warning once by @LuisSanchez25 in https://github.com/XENONnT/straxen/pull/1211
+        
+        
+        **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.1.0...v2.1.1
+        
+        
+        v2.1.0 / 2023-06-22
         -------------------
         * Added peaks subtyping by @Jianyu010 in https://github.com/XENONnT/straxen/pull/1152
         * Fix ipython version by @dachengx in https://github.com/XENONnT/straxen/pull/1169
         * Fix bug in hitlets time ordering by @dachengx in https://github.com/XENONnT/straxen/pull/1173
         * Bump actions/setup-python from 4.5.0 to 4.6.0 by @dependabot in https://github.com/XENONnT/straxen/pull/1170
         * Save hits level information(hits height and time difference) in peak and event level by @dachengx in https://github.com/XENONnT/straxen/pull/1155
         * Fix argsort inside numba.jit using kind='mergesort' by @dachengx in https://github.com/XENONnT/straxen/pull/1176
```

### Comparing `straxen-2.1.0/README.md` & `straxen-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/bin/ajax` & `straxen-2.1.1/bin/ajax`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/bin/bootstrax` & `straxen-2.1.1/bin/bootstrax`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/bin/fake_daq` & `straxen-2.1.1/bin/fake_daq`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/bin/microstrax` & `straxen-2.1.1/bin/microstrax`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/bin/refresh_raw_records` & `straxen-2.1.1/bin/refresh_raw_records`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/bin/restrax` & `straxen-2.1.1/bin/restrax`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/bin/straxen-print_versions` & `straxen-2.1.1/bin/straxen-print_versions`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/bin/straxer` & `straxen-2.1.1/bin/straxer`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/setup.cfg` & `straxen-2.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/setup.py` & `straxen-2.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 with open('README.md') as file:
     readme = file.read()
 
 with open('HISTORY.md') as file:
     history = file.read()
 
 setuptools.setup(name='straxen',
-                 version='2.1.0',
+                 version='2.1.1',
                  description='Streaming analysis for XENON',
                  author='Straxen contributors, the XENON collaboration',
                  url='https://github.com/XENONnT/straxen',
                  long_description=readme + '\n\n' + history,
                  long_description_content_type="text/markdown",
                  setup_requires=['pytest-runner'],
                  install_requires=requires,
```

### Comparing `straxen-2.1.0/straxen/__init__.py` & `straxen-2.1.1/straxen/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '2.1.0'
+__version__ = '2.1.1'
 
 from utilix import uconfig
 from .common import *
 # contexts.py below
 from .corrections_services import *
 from .get_corrections import *
```

### Comparing `straxen-2.1.0/straxen/analyses/bokeh_waveform_plot.py` & `straxen-2.1.1/straxen/analyses/bokeh_waveform_plot.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/analyses/daq_waveforms.py` & `straxen-2.1.1/straxen/analyses/daq_waveforms.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/analyses/event_display.py` & `straxen-2.1.1/straxen/analyses/event_display.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/analyses/holoviews_waveform_display.py` & `straxen-2.1.1/straxen/analyses/holoviews_waveform_display.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/analyses/posrec_comparison.py` & `straxen-2.1.1/straxen/analyses/posrec_comparison.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/analyses/pulse_plots.py` & `straxen-2.1.1/straxen/analyses/pulse_plots.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/analyses/quick_checks.py` & `straxen-2.1.1/straxen/analyses/quick_checks.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/analyses/records_matrix.py` & `straxen-2.1.1/straxen/analyses/records_matrix.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/analyses/waveform_plot.py` & `straxen-2.1.1/straxen/analyses/waveform_plot.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/bokeh_utils.py` & `straxen-2.1.1/straxen/bokeh_utils.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/common.py` & `straxen-2.1.1/straxen/common.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/contexts.py` & `straxen-2.1.1/straxen/contexts.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/corrections_services.py` & `straxen-2.1.1/straxen/corrections_services.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/daq_core.py` & `straxen-2.1.1/straxen/daq_core.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/entry_points.py` & `straxen-2.1.1/straxen/entry_points.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/get_corrections.py` & `straxen-2.1.1/straxen/get_corrections.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/holoviews/holoviews_inspector.py` & `straxen-2.1.1/straxen/holoviews/holoviews_inspector.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/holoviews/holoviews_peak_data.py` & `straxen-2.1.1/straxen/holoviews/holoviews_peak_data.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/holoviews/holoviews_pmt_array.py` & `straxen-2.1.1/straxen/holoviews/holoviews_pmt_array.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/holoviews/holoviews_tpc_event_display.py` & `straxen-2.1.1/straxen/holoviews/holoviews_tpc_event_display.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/holoviews_utils.py` & `straxen-2.1.1/straxen/holoviews_utils.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/itp_map.py` & `straxen-2.1.1/straxen/itp_map.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/legacy/contexts_1t.py` & `straxen-2.1.1/straxen/legacy/contexts_1t.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/legacy/hitfinder_thresholds.py` & `straxen-2.1.1/straxen/legacy/hitfinder_thresholds.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/legacy/plugins_1t/event_info.py` & `straxen-2.1.1/straxen/legacy/plugins_1t/event_info.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/legacy/plugins_1t/pax_interface.py` & `straxen-2.1.1/straxen/legacy/plugins_1t/pax_interface.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/legacy/plugins_1t/peak_positions.py` & `straxen-2.1.1/straxen/legacy/plugins_1t/peak_positions.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/legacy/plugins_1t/x1t_cuts.py` & `straxen-2.1.1/straxen/legacy/plugins_1t/x1t_cuts.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/legacy/xenon1t_url_configs.py` & `straxen-2.1.1/straxen/legacy/xenon1t_url_configs.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/matplotlib_utils.py` & `straxen-2.1.1/straxen/matplotlib_utils.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/mini_analysis.py` & `straxen-2.1.1/straxen/mini_analysis.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/misc.py` & `straxen-2.1.1/straxen/misc.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/numbafied_scipy.py` & `straxen-2.1.1/straxen/numbafied_scipy.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/__init__.py` & `straxen-2.1.1/straxen/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/afterpulses/afterpulse_processing.py` & `straxen-2.1.1/straxen/plugins/afterpulses/afterpulse_processing.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/aqmon_hits/aqmon_hits.py` & `straxen-2.1.1/straxen/plugins/aqmon_hits/aqmon_hits.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/defaults.py` & `straxen-2.1.1/straxen/plugins/defaults.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/detector_time_offsets/detector_time_offsets.py` & `straxen-2.1.1/straxen/plugins/detector_time_offsets/detector_time_offsets.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/events/__init__.py` & `straxen-2.1.1/straxen/plugins/events/__init__.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/events/_event_s1_positions_base.py` & `straxen-2.1.1/straxen/plugins/events/_event_s1_positions_base.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/events/_event_s2_positions_base.py` & `straxen-2.1.1/straxen/plugins/events/_event_s2_positions_base.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/events/corrected_areas.py` & `straxen-2.1.1/straxen/plugins/events/corrected_areas.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/events/distinct_channels.py` & `straxen-2.1.1/straxen/plugins/events/distinct_channels.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/events/energy_estimates.py` & `straxen-2.1.1/straxen/plugins/events/energy_estimates.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/events/event_ambience.py` & `straxen-2.1.1/straxen/plugins/events/event_ambience.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/events/event_area_per_channel.py` & `straxen-2.1.1/straxen/plugins/events/event_area_per_channel.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/events/event_basics.py` & `straxen-2.1.1/straxen/plugins/events/event_basics.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/events/event_info.py` & `straxen-2.1.1/straxen/plugins/events/event_info.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/events/event_info_double.py` & `straxen-2.1.1/straxen/plugins/events/event_info_double.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/events/event_pattern_fit.py` & `straxen-2.1.1/straxen/plugins/events/event_pattern_fit.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/events/event_positions.py` & `straxen-2.1.1/straxen/plugins/events/event_positions.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/events/event_s1_positions_cnn.py` & `straxen-2.1.1/straxen/plugins/events/event_s1_positions_cnn.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/events/event_s2_positions_cnn.py` & `straxen-2.1.1/straxen/plugins/events/event_s2_positions_cnn.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/events/event_s2_positions_gcn.py` & `straxen-2.1.1/straxen/plugins/events/event_s2_positions_gcn.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/events/event_s2_positions_mlp.py` & `straxen-2.1.1/straxen/plugins/events/event_s2_positions_mlp.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/events/event_shadow.py` & `straxen-2.1.1/straxen/plugins/events/event_shadow.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/events/event_top_bottom_params.py` & `straxen-2.1.1/straxen/plugins/events/event_top_bottom_params.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/events/event_w_bayes_class.py` & `straxen-2.1.1/straxen/plugins/events/event_w_bayes_class.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/events/event_waveform.py` & `straxen-2.1.1/straxen/plugins/events/event_waveform.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/events/events.py` & `straxen-2.1.1/straxen/plugins/events/events.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/events/local_minimum_info.py` & `straxen-2.1.1/straxen/plugins/events/local_minimum_info.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/events/multi_scatter.py` & `straxen-2.1.1/straxen/plugins/events/multi_scatter.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/events/s2_recon_pos_diff.py` & `straxen-2.1.1/straxen/plugins/events/s2_recon_pos_diff.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/events/veto_proximity.py` & `straxen-2.1.1/straxen/plugins/events/veto_proximity.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/events_mv/events_mv.py` & `straxen-2.1.1/straxen/plugins/events_mv/events_mv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/events_mv/events_sync_mv.py` & `straxen-2.1.1/straxen/plugins/events_mv/events_sync_mv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/events_nv/event_positions_nv.py` & `straxen-2.1.1/straxen/plugins/events_nv/event_positions_nv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/events_nv/events_nv.py` & `straxen-2.1.1/straxen/plugins/events_nv/events_nv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/events_nv/events_sync_nv.py` & `straxen-2.1.1/straxen/plugins/events_nv/events_sync_nv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/hitlets_mv/hitlets_mv.py` & `straxen-2.1.1/straxen/plugins/hitlets_mv/hitlets_mv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/hitlets_nv/hitlets_nv.py` & `straxen-2.1.1/straxen/plugins/hitlets_nv/hitlets_nv.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,15 @@
         strax.hitlet_properties(temp_hitlets)
         entropy = strax.conditional_entropy(temp_hitlets, template='flat', square_data=False)
         temp_hitlets['entropy'][:] = entropy
 
         # Remove data field:
         hitlets = np.zeros(len(temp_hitlets), dtype=strax.hitlet_dtype())
         strax.copy_to_buffer(temp_hitlets, hitlets, '_copy_hitlets')
-        return hitlets
+        return strax.sort_by_time(hitlets)
 
 
 def remove_switched_off_channels(hits, to_pe):
     """Removes hits which were found in a channel without any gain.
     :param hits: Hits found in records.
     :param to_pe: conversion factor from ADC per sample.
     :return: Hits
```

### Comparing `straxen-2.1.0/straxen/plugins/individual_peak_monitor/individual_peak_monitor.py` & `straxen-2.1.1/straxen/plugins/individual_peak_monitor/individual_peak_monitor.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/led_cal/led_calibration.py` & `straxen-2.1.1/straxen/plugins/led_cal/led_calibration.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/merged_s2s/merged_s2s.py` & `straxen-2.1.1/straxen/plugins/merged_s2s/merged_s2s.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,23 +56,30 @@
 
     sum_waveform_top_array = straxen.URLConfig(
         default=True,
         type=bool,
         help='Digitize the sum waveform of the top array separately'
     )
 
+    merged_s2s_get_window_size_factor = straxen.URLConfig(
+        default=5,
+        type=int,
+        track=False,
+        help='Factor of the window size for the merged_s2s plugin'
+    )
+
     def setup(self):
         self.to_pe = self.gain_model
 
     def infer_dtype(self):
         return strax.unpack_dtype(self.deps['peaklets'].dtype_for('peaklets'))
 
     def get_window_size(self):
-        return 5 * (int(self.s2_merge_gap_thresholds[0][1])
-                    + self.s2_merge_max_duration)
+        return self.merged_s2s_get_window_size_factor * (
+            int(self.s2_merge_gap_thresholds[0][1]) + self.s2_merge_max_duration)
 
     def compute(self, peaklets, lone_hits):
         if self.merge_without_s1:
             peaklets = peaklets[peaklets['type'] != 1]
 
         if len(peaklets) <= 1:
             return np.zeros(0, dtype=self.dtype)
```

### Comparing `straxen-2.1.0/straxen/plugins/merged_s2s_he/merged_s2s_he.py` & `straxen-2.1.1/straxen/plugins/merged_s2s_he/merged_s2s_he.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/online_monitor_mv/online_monitor_mv.py` & `straxen-2.1.1/straxen/plugins/online_monitor_mv/online_monitor_mv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/online_monitor_nv/online_monitor_nv.py` & `straxen-2.1.1/straxen/plugins/online_monitor_nv/online_monitor_nv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/online_peak_monitor/online_peak_monitor.py` & `straxen-2.1.1/straxen/plugins/online_peak_monitor/online_peak_monitor.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/peaklets/peaklet_classification.py` & `straxen-2.1.1/straxen/plugins/peaklets/peaklet_classification.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/peaklets/peaklets.py` & `straxen-2.1.1/straxen/plugins/peaklets/peaklets.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/peaklets_he/peaklet_classification_he.py` & `straxen-2.1.1/straxen/plugins/peaklets_he/peaklet_classification_he.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/peaklets_he/peaklets_he.py` & `straxen-2.1.1/straxen/plugins/peaklets_he/peaklets_he.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/peaks/__init__.py` & `straxen-2.1.1/straxen/plugins/peaks/__init__.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/peaks/_peak_positions_base.py` & `straxen-2.1.1/straxen/plugins/peaks/_peak_positions_base.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/peaks/_peak_s1_positions_base.py` & `straxen-2.1.1/straxen/plugins/peaks/_peak_s1_positions_base.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/peaks/peak_ambience.py` & `straxen-2.1.1/straxen/plugins/peaks/peak_ambience.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     """
     Calculate Ambience of peaks.
     Features are the number of lonehits, small S0, S1, S2 in a time window before peaks,
     and the number of small S2 in circle near the S2 peak in a time window.
     References:
         * v0.0.7 reference: xenon:xenonnt:ac:prediction:shadow_ambience
     """
-    __version__ = '0.0.7'
+    __version__ = '0.0.8'
     depends_on = ('lone_hits', 'peak_basics', 'peak_positions')
     provides = 'peak_ambience'
     data_kind = 'peaks'
     save_when = strax.SaveWhen.EXPLICIT
 
     ambience_time_window_backward = straxen.URLConfig(
         default=int(2e6),
@@ -71,15 +71,19 @@
                         f'n_{ambience}'), np.int16),
                       ((f"Area sum of small {' '.join(ambience.split('_'))} a peak",
                         f's_{ambience}'), np.float32)]
         dtype += strax.time_fields
         return dtype
 
     def compute(self, lone_hits, peaks):
-        return self.compute_ambience(lone_hits, peaks, peaks)
+        argsort = np.argsort(peaks['center_time'], kind='mergesort')
+        _peaks = np.sort(peaks, order='center_time')
+        result = np.zeros(len(peaks), self.dtype)
+        _quick_assign(argsort, result, self.compute_ambience(lone_hits, peaks, _peaks))
+        return result
 
     def compute_ambience(self, lone_hits, peaks, current_peak):
         # 1. Initialization
         result = np.zeros(len(current_peak), self.dtype)
 
         # 2. Define time window for each peak, we will find small peaks & lone hits within these time windows
         roi = np.zeros(len(current_peak), dtype=strax.time_fields)
@@ -182,7 +186,13 @@
 
 
 @numba.njit
 def distance_in_xy(peak_a, peak_b):
     """Distance between S2s in (x,y)"""
     return np.sqrt((peak_a['x'] - peak_b['x']) ** 2 +
                    (peak_a['y'] - peak_b['y']) ** 2)
+
+
+@numba.njit
+def _quick_assign(indices, results, inputs):
+    for i, r in zip(indices, inputs):
+        results[i] = r
```

### Comparing `straxen-2.1.0/straxen/plugins/peaks/peak_basics.py` & `straxen-2.1.1/straxen/plugins/peaks/peak_basics.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/peaks/peak_classification_bayes.py` & `straxen-2.1.1/straxen/plugins/peaks/peak_classification_bayes.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/peaks/peak_corrections.py` & `straxen-2.1.1/straxen/plugins/peaks/peak_corrections.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/peaks/peak_per_event.py` & `straxen-2.1.1/straxen/plugins/peaks/peak_per_event.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/peaks/peak_positions.py` & `straxen-2.1.1/straxen/plugins/peaks/peak_positions.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/peaks/peak_positions_cnn.py` & `straxen-2.1.1/straxen/plugins/peaks/peak_positions_cnn.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/peaks/peak_positions_gcn.py` & `straxen-2.1.1/straxen/plugins/peaks/peak_positions_gcn.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/peaks/peak_positions_mlp.py` & `straxen-2.1.1/straxen/plugins/peaks/peak_positions_mlp.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/peaks/peak_proximity.py` & `straxen-2.1.1/straxen/plugins/peaks/peak_proximity.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/peaks/peak_s1_positions_cnn.py` & `straxen-2.1.1/straxen/plugins/peaks/peak_s1_positions_cnn.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/peaks/peak_shadow.py` & `straxen-2.1.1/straxen/plugins/peaks/peak_shadow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import numba
 from scipy.stats import halfcauchy
-from .peak_ambience import distance_in_xy
+from .peak_ambience import distance_in_xy, _quick_assign
 import strax
 import straxen
 
 export, __all__ = strax.exporter()
 
 
 @export
@@ -14,15 +14,15 @@
     This plugin can find and calculate the time & position shadow
     from previous peaks in time.
     It also gives the area and (x,y) of the previous peaks.
     References:
         * v0.1.5 reference: xenon:xenonnt:ac:prediction:shadow_ambience
     """
 
-    __version__ = '0.1.5'
+    __version__ = '0.1.6'
 
     depends_on = ('peak_basics', 'peak_positions')
     provides = 'peak_shadow'
     save_when = strax.SaveWhen.EXPLICIT
 
     shadow_time_window_backward = straxen.URLConfig(
         default=int(1e9),
@@ -94,15 +94,19 @@
         dtype = []
         dtype += [('shadow', np.float32), ('dt', np.int64)]
         dtype += [('x', np.float32), ('y', np.float32)]
         dtype += [('nearest_dt', np.int64)]
         return dtype
 
     def compute(self, peaks):
-        return self.compute_shadow(peaks, peaks)
+        argsort = np.argsort(peaks['center_time'], kind='mergesort')
+        _peaks = np.sort(peaks, order='center_time')
+        result = np.zeros(len(peaks), self.dtype)
+        _quick_assign(argsort, result, self.compute_shadow(peaks, _peaks))
+        return result
 
     def compute_shadow(self, peaks, current_peak):
         # 1. Define time window for each peak, we will find previous peaks within these time windows
         roi_shadow = np.zeros(len(current_peak), dtype=strax.time_fields)
         roi_shadow['time'] = current_peak['center_time'] - self.shadow_time_window_backward
         roi_shadow['endtime'] = current_peak['center_time']
```

### Comparing `straxen-2.1.0/straxen/plugins/peaks/peak_top_bottom_params.py` & `straxen-2.1.1/straxen/plugins/peaks/peak_top_bottom_params.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/peaks/peaks.py` & `straxen-2.1.1/straxen/plugins/peaks/peaks.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/peaks/peaks_subtyping.py` & `straxen-2.1.1/straxen/plugins/peaks/peaks_subtyping.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/peaks_he/peaks_he.py` & `straxen-2.1.1/straxen/plugins/peaks_he/peaks_he.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/raw_records/daqreader.py` & `straxen-2.1.1/straxen/plugins/raw_records/daqreader.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/raw_records_coin_nv/nveto_recorder.py` & `straxen-2.1.1/straxen/plugins/raw_records_coin_nv/nveto_recorder.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/records/records.py` & `straxen-2.1.1/straxen/plugins/records/records.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/records_he/records_he.py` & `straxen-2.1.1/straxen/plugins/records_he/records_he.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/records_mv/records_mv.py` & `straxen-2.1.1/straxen/plugins/records_mv/records_mv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/records_nv/records_nv.py` & `straxen-2.1.1/straxen/plugins/records_nv/records_nv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/plugins/veto_intervals/veto_intervals.py` & `straxen-2.1.1/straxen/plugins/veto_intervals/veto_intervals.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/scada.py` & `straxen-2.1.1/straxen/scada.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/storage/mongo_storage.py` & `straxen-2.1.1/straxen/storage/mongo_storage.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/storage/online_monitor_frontend.py` & `straxen-2.1.1/straxen/storage/online_monitor_frontend.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/storage/rucio_local.py` & `straxen-2.1.1/straxen/storage/rucio_local.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/storage/rucio_remote.py` & `straxen-2.1.1/straxen/storage/rucio_remote.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/storage/rundb.py` & `straxen-2.1.1/straxen/storage/rundb.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/test_utils.py` & `straxen-2.1.1/straxen/test_utils.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/units.py` & `straxen-2.1.1/straxen/units.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/straxen/url_config.py` & `straxen-2.1.1/straxen/url_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 from straxen.misc import filter_kwargs
 from typing import Container, Mapping, Union, Iterable
 
 export, __all__ = strax.exporter()
 
 _CACHES = {}
 
+WARN = True
+
 
 @export
 def clear_config_caches():
     for cache in _CACHES.values():
         cache.clear()
 
 
@@ -697,18 +699,25 @@
 
 
 @URLConfig.preprocessor
 def alphabetize_url_kwargs(url: str):
     """
     Reorders queries for urlconfigs to avoid hashing issues
     """
+    
+    global WARN
 
     if isinstance(url, str) and URLConfig.SCHEME_SEP in url:
-        if url != URLConfig.format_url_kwargs(url):
-            warnings.warn("From straxen version 2.1.0 onward, URLConfig parameters will be sorted alphabetically before being passed to the plugins, this will change the lineage hash for non-sorted URLs. To load data processed with non-sorted URLs, you will need to use an older version.", FutureWarning)
+        if url != URLConfig.format_url_kwargs(url) and WARN:
+            warnings.warn("From straxen version 2.1.0 onward, URLConfig parameters"
+              "will be sorted alphabetically before being passed to the plugins,"
+              " this will change the lineage hash for non-sorted URLs. To load"
+              " data processed with non-sorted URLs, you will need to use an"
+              " older version.")
+            WARN = False
         return URLConfig.format_url_kwargs(url)
     return url
 
 
 @URLConfig.register('run_doc')
 def read_rundoc(path, run_id=None, default=None):
     """Read a path from the rundoc.
@@ -726,7 +735,8 @@
         elif isinstance(rundoc, dict) and part in rundoc:
             rundoc = rundoc[part]
         elif default is not None:
             return default
         else:
             raise ValueError(f'No path {path} found in rundoc for run {run_id}')
     return rundoc
+
```

### Comparing `straxen-2.1.0/straxen.egg-info/PKG-INFO` & `straxen-2.1.1/straxen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: straxen
-Version: 2.1.0
+Version: 2.1.1
 Summary: Streaming analysis for XENON
 Home-page: https://github.com/XENONnT/straxen
 Author: Straxen contributors, the XENON collaboration
 License: UNKNOWN
 Description: # straxen
         Streaming analysis for XENON(nT)
         
@@ -25,15 +25,26 @@
         [![Python Versions](https://img.shields.io/pypi/pyversions/straxen.svg)](https://pypi.python.org/pypi/straxen)
         [![PyPI downloads](https://img.shields.io/pypi/dm/straxen.svg)](https://pypistats.org/packages/straxen)
         
         [![Update context collection](https://github.com/XENONnT/straxen/workflows/Update%20context%20collection/badge.svg)](https://github.com/XENONnT/straxen/actions/workflows/contexts.yml)
         [![Python style](https://github.com/XENONnT/straxen/actions/workflows/code_style.yml/badge.svg)](https://github.com/XENONnT/straxen/actions/workflows/code_style.yml)
         
         
-        v2.1.70 / 2023-06-22
+        v2.1.1 / 2023-07-06
+        -------------------
+        * Fix timing of peaks when ordering in `center_time` by @dachengx in https://github.com/XENONnT/straxen/pull/1208
+        * Move `get_window_size` factor of merged_s2s as untracked configuration by @dachengx in https://github.com/XENONnT/straxen/pull/1209
+        * Sort `hitlets` in `nVETOHitlets` by @dachengx in https://github.com/XENONnT/straxen/pull/1210
+        * Only print out warning once by @LuisSanchez25 in https://github.com/XENONnT/straxen/pull/1211
+        
+        
+        **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.1.0...v2.1.1
+        
+        
+        v2.1.0 / 2023-06-22
         -------------------
         * Added peaks subtyping by @Jianyu010 in https://github.com/XENONnT/straxen/pull/1152
         * Fix ipython version by @dachengx in https://github.com/XENONnT/straxen/pull/1169
         * Fix bug in hitlets time ordering by @dachengx in https://github.com/XENONnT/straxen/pull/1173
         * Bump actions/setup-python from 4.5.0 to 4.6.0 by @dependabot in https://github.com/XENONnT/straxen/pull/1170
         * Save hits level information(hits height and time difference) in peak and event level by @dachengx in https://github.com/XENONnT/straxen/pull/1155
         * Fix argsort inside numba.jit using kind='mergesort' by @dachengx in https://github.com/XENONnT/straxen/pull/1176
```

### Comparing `straxen-2.1.0/straxen.egg-info/SOURCES.txt` & `straxen-2.1.1/straxen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/tests/storage/test_database_frontends.py` & `straxen-2.1.1/tests/storage/test_database_frontends.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/tests/storage/test_mongo_downloader.py` & `straxen-2.1.1/tests/storage/test_mongo_downloader.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/tests/storage/test_mongo_interactions.py` & `straxen-2.1.1/tests/storage/test_mongo_interactions.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/tests/storage/test_rucio_local.py` & `straxen-2.1.1/tests/storage/test_rucio_local.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/tests/storage/test_rucio_remote.py` & `straxen-2.1.1/tests/storage/test_rucio_remote.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/tests/test_1T_plugins.py` & `straxen-2.1.1/tests/test_1T_plugins.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/tests/test_aqmon.py` & `straxen-2.1.1/tests/test_aqmon.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/tests/test_basics.py` & `straxen-2.1.1/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/tests/test_channel_split.py` & `straxen-2.1.1/tests/test_channel_split.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/tests/test_cmt.py` & `straxen-2.1.1/tests/test_cmt.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/tests/test_common.py` & `straxen-2.1.1/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/tests/test_contexts.py` & `straxen-2.1.1/tests/test_contexts.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/tests/test_count_pulses.py` & `straxen-2.1.1/tests/test_count_pulses.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/tests/test_daq_reader.py` & `straxen-2.1.1/tests/test_daq_reader.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/tests/test_holoviews_utils.py` & `straxen-2.1.1/tests/test_holoviews_utils.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/tests/test_itp_map.py` & `straxen-2.1.1/tests/test_itp_map.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/tests/test_led_calibration.py` & `straxen-2.1.1/tests/test_led_calibration.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/tests/test_mini_analyses.py` & `straxen-2.1.1/tests/test_mini_analyses.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/tests/test_misc.py` & `straxen-2.1.1/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/tests/test_nveto_events.py` & `straxen-2.1.1/tests/test_nveto_events.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/tests/test_nveto_recorder.py` & `straxen-2.1.1/tests/test_nveto_recorder.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/tests/test_patternfit.py` & `straxen-2.1.1/tests/test_patternfit.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/tests/test_peaklet_processing.py` & `straxen-2.1.1/tests/test_peaklet_processing.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/tests/test_peaks.py` & `straxen-2.1.1/tests/test_peaks.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/tests/test_scada.py` & `straxen-2.1.1/tests/test_scada.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/tests/test_url_config.py` & `straxen-2.1.1/tests/test_url_config.py`

 * *Files identical despite different names*

### Comparing `straxen-2.1.0/tests/test_veto_hitlets.py` & `straxen-2.1.1/tests/test_veto_hitlets.py`

 * *Files identical despite different names*

