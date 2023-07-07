# Comparing `tmp/Simba-UW-tf-dev-1.64.7.tar.gz` & `tmp/Simba-UW-tf-dev-1.64.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.64.7.tar", last modified: Thu Jul  6 16:46:40 2023, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.64.8.tar", last modified: Fri Jul  7 20:40:51 2023, max compression
```

## Comparing `Simba-UW-tf-dev-1.64.7.tar` & `Simba-UW-tf-dev-1.64.8.tar`

### file list

```diff
@@ -1,584 +1,584 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:39.000000 Simba-UW-tf-dev-1.64.7/simba/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/ui/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-07-06 15:33:05.000000 Simba-UW-tf-dev-1.64.7/simba/ui/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)     9015 2023-06-29 20:55:17.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/mutual_exclusivity_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/csv_2_parquet_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/quick_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/batch_preprocess_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/heatmap_location_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/clf_probability_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/movement_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/clf_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    15950 2023-05-20 12:10:35.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1150 2023-05-25 18:21:39.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/remove_roi_features_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5814 2023-06-15 20:06:37.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/roi_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5977 2023-05-31 12:58:14.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/outlier_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/gantt_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/clf_validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7721 2023-05-24 15:18:33.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/severity_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/fsttc_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/kleinberg_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7288 2023-05-29 20:14:50.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/pose_reorganizer_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/clf_by_timebins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/heatmap_clf_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/data_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/roi_features_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/pup_retrieval_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/about_simba_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3605 2023-05-25 18:54:56.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6353 2023-05-24 15:31:12.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    50444 2023-07-05 17:57:07.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/video_processing_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/clf_by_roi_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/make_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/archive_files_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/pose_bp_drop_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    10695 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/distance_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3601 2023-07-03 00:19:12.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    12869 2023-05-23 12:47:59.000000 Simba-UW-tf-dev-1.64.7/simba/ui/video_info_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.64.7/simba/ui/user_defined_pose_creator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/ui/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12879 2023-06-18 20:27:37.000000 Simba-UW-tf-dev-1.64.7/simba/ui/create_project_ui.py
--rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.64.7/simba/ui/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    35431 2023-06-13 17:24:57.000000 Simba-UW-tf-dev-1.64.7/simba/ui/machine_model_settings_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/blob_storage/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.64.7/simba/blob_storage/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/labelling/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.64.7/simba/labelling/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21667 2023-06-20 18:30:00.000000 Simba-UW-tf-dev-1.64.7/simba/labelling/labelling_interface_old.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/labelling/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    20914 2023-06-22 13:26:28.000000 Simba-UW-tf-dev-1.64.7/simba/labelling/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     3568 2023-05-19 11:18:49.000000 Simba-UW-tf-dev-1.64.7/simba/labelling/extract_labelled_frames.py
--rw-r--r--   0 simon      (501) staff       (20)    26943 2023-06-20 19:04:35.000000 Simba-UW-tf-dev-1.64.7/simba/labelling/labelling_advanced_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.64.7/simba/labelling/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.64.7/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.64.7/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-13 17:25:39.000000 Simba-UW-tf-dev-1.64.7/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.64.7/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.64.7/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.64.7/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     9846 2023-06-06 18:27:30.000000 Simba-UW-tf-dev-1.64.7/simba/unsupervised/ui.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/unsupervised/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.64.7/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.64.7/simba/unsupervised/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.64.7/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.64.7/simba/unsupervised/cluster_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.64.7/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)    10287 2023-06-06 17:50:12.000000 Simba-UW-tf-dev-1.64.7/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.64.7/simba/unsupervised/tsne.py
--rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.64.7/simba/unsupervised/cluster_visualizer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.7/simba/bounding_box_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/bounding_box_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.64.7/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.64.7/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.64.7/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.7/simba/bounding_box_tools/find_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.7/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    49156 2023-07-06 15:33:05.000000 Simba-UW-tf-dev-1.64.7/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7127 2023-05-28 19:41:35.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-07 20:28:11.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)      421 2023-07-05 19:50:18.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/shap_gpu.py
--rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     8943 2023-06-05 18:15:28.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/shap_log_mp_2.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     8580 2023-05-31 20:02:32.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/shap_log_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)    30764 2023-06-13 17:23:34.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
--rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     4279 2023-06-01 12:49:14.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/read_files_mp_2.py
--rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:44:29.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-07-06 15:33:05.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3864 2023-05-19 19:41:40.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    18368 2023-07-03 18:44:03.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8244 2023-05-21 16:28:49.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/feature_extractor_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/feature_extractor_4bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/.idea/features_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/.idea/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/.idea/.name
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    15434 2023-05-20 18:29:53.000000 Simba-UW-tf-dev-1.64.7/simba/requirements.txt
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-07-06 15:33:05.000000 Simba-UW-tf-dev-1.64.7/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43029 2023-06-05 17:40:09.000000 Simba-UW-tf-dev-1.64.7/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    38224 2023-06-15 15:41:52.000000 Simba-UW-tf-dev-1.64.7/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/mixins/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.64.7/simba/mixins/pose_importer_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     2938 2023-07-02 20:03:29.000000 Simba-UW-tf-dev-1.64.7/simba/mixins/video_processing_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/mixins/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.64.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.64.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.64.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    82442 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.64.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    51809 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.64.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    14391 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.64.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc
--rw-r--r--   0 simon      (501) staff       (20)    14188 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.64.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    37135 2023-06-02 12:12:15.000000 Simba-UW-tf-dev-1.64.7/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    61873 2023-05-19 21:14:46.000000 Simba-UW-tf-dev-1.64.7/simba/mixins/plotting_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     9145 2023-06-13 18:36:10.000000 Simba-UW-tf-dev-1.64.7/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    73291 2023-06-19 20:46:57.000000 Simba-UW-tf-dev-1.64.7/simba/mixins/train_model_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6094 2023-05-21 17:39:19.000000 Simba-UW-tf-dev-1.64.7/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    10759 2023-06-08 22:23:03.000000 Simba-UW-tf-dev-1.64.7/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.64.7/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.7/simba/third_party_label_appenders/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    18417 2023-06-18 19:01:16.000000 Simba-UW-tf-dev-1.64.7/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.64.7/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18934 2023-06-18 19:03:04.000000 Simba-UW-tf-dev-1.64.7/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8181 2023-05-21 17:19:25.000000 Simba-UW-tf-dev-1.64.7/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     6988 2023-05-21 17:31:04.000000 Simba-UW-tf-dev-1.64.7/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5239 2023-05-21 18:07:18.000000 Simba-UW-tf-dev-1.64.7/simba/third_party_label_appenders/solomon_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.7/simba/cue_light_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.7/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.7/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.7/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.7/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.64.7/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.7/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)    11876 2023-06-18 20:21:39.000000 Simba-UW-tf-dev-1.64.7/simba/utils/config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    21103 2023-06-20 12:58:32.000000 Simba-UW-tf-dev-1.64.7/simba/utils/enums.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-07-06 15:33:05.000000 Simba-UW-tf-dev-1.64.7/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7801 2023-07-05 17:33:58.000000 Simba-UW-tf-dev-1.64.7/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)     9292 2023-07-05 17:27:17.000000 Simba-UW-tf-dev-1.64.7/simba/utils/checks.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/utils/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    43615 2023-07-05 18:25:40.000000 Simba-UW-tf-dev-1.64.7/simba/utils/read_write.py
--rw-r--r--   0 simon      (501) staff       (20)     9841 2023-06-19 23:24:08.000000 Simba-UW-tf-dev-1.64.7/simba/utils/lookups.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/utils/cli/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/utils/cli/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6017 2023-05-28 13:41:20.000000 Simba-UW-tf-dev-1.64.7/simba/utils/cli/cli_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    15116 2023-07-05 17:33:58.000000 Simba-UW-tf-dev-1.64.7/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)    19250 2023-06-13 13:46:20.000000 Simba-UW-tf-dev-1.64.7/simba/utils/data.py
--rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.64.7/simba/utils/printing.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/st/
--rw-r--r--   0 simon      (501) staff       (20)      282 2023-06-16 17:26:25.000000 Simba-UW-tf-dev-1.64.7/simba/st/enums.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-16 13:55:39.000000 Simba-UW-tf-dev-1.64.7/simba/st/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2102 2023-06-19 19:54:19.000000 Simba-UW-tf-dev-1.64.7/simba/st/select_groups_pg.py
--rw-r--r--   0 simon      (501) staff       (20)     2325 2023-06-19 19:54:19.000000 Simba-UW-tf-dev-1.64.7/simba/st/aggregate_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     1485 2023-06-16 18:20:31.000000 Simba-UW-tf-dev-1.64.7/simba/st/app.py
--rw-r--r--   0 simon      (501) staff       (20)      249 2023-06-16 18:20:19.000000 Simba-UW-tf-dev-1.64.7/simba/st/welcome_page.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/pose_processors/
--rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.64.7/simba/pose_processors/reorganize_keypoint.py
--rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.64.7/simba/pose_processors/remove_keypoints.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.7/simba/pose_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/pose_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.64.7/simba/pose_processors/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)     5618 2023-06-13 18:36:10.000000 Simba-UW-tf-dev-1.64.7/simba/pose_processors/reverse_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    13008 2023-05-24 15:32:44.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12484 2023-05-23 14:52:24.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    14056 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)    14029 2023-06-04 11:55:47.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)    14824 2023-07-05 12:33:51.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)     7660 2023-06-20 12:45:11.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/pose_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     7891 2023-05-29 21:41:05.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/Directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    15745 2023-05-20 12:16:06.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11203 2023-05-24 15:35:24.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13471 2023-05-20 12:15:46.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    11519 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     9385 2023-05-31 16:46:49.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     9526 2023-06-04 12:03:25.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10005 2023-05-29 21:36:37.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/Directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/heat_mapper_location_mp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/dash_app/
--rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/dash_app/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/dash_app/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/dash_app/dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-16 12:50:41.000000 Simba-UW-tf-dev-1.64.7/simba/dash_app/plotly_dash.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/data_processors/
--rw-r--r--   0 simon      (501) staff       (20)     7248 2023-05-25 19:01:00.000000 Simba-UW-tf-dev-1.64.7/simba/data_processors/agg_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.64.7/simba/data_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    11196 2023-05-28 19:50:35.000000 Simba-UW-tf-dev-1.64.7/simba/data_processors/severity_bout_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16285 2023-06-13 13:57:45.000000 Simba-UW-tf-dev-1.64.7/simba/data_processors/interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)     8127 2023-05-25 13:57:19.000000 Simba-UW-tf-dev-1.64.7/simba/data_processors/timebins_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    13451 2023-06-19 20:47:55.000000 Simba-UW-tf-dev-1.64.7/simba/data_processors/fsttc_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/data_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.64.7/simba/data_processors/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.64.7/simba/data_processors/directing_other_animals_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8624 2023-05-25 14:07:56.000000 Simba-UW-tf-dev-1.64.7/simba/data_processors/timebins_movement_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.64.7/simba/data_processors/severity_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.64.7/simba/data_processors/pup_retrieval_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.64.7/simba/data_processors/pybursts_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    11533 2023-05-28 19:50:34.000000 Simba-UW-tf-dev-1.64.7/simba/data_processors/severity_frame_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     6087 2023-06-28 20:32:32.000000 Simba-UW-tf-dev-1.64.7/simba/data_processors/mutual_exclusivity_corrector.py
--rw-r--r--   0 simon      (501) staff       (20)     9656 2023-05-25 13:32:25.000000 Simba-UW-tf-dev-1.64.7/simba/data_processors/kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8131 2023-05-25 14:37:36.000000 Simba-UW-tf-dev-1.64.7/simba/data_processors/movement_calculator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:39.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/model/
--rw-r--r--   0 simon      (501) staff       (20)    20086 2023-06-05 20:43:28.000000 Simba-UW-tf-dev-1.64.7/simba/model/train_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.7/simba/model/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3315 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.64.7/simba/model/inference_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    20849 2023-06-05 18:44:40.000000 Simba-UW-tf-dev-1.64.7/simba/model/grid_search_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3363 2023-05-19 11:12:45.000000 Simba-UW-tf-dev-1.64.7/simba/model/inference_validation.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.7/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43194 2023-06-22 13:51:00.000000 Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    20174 2023-06-12 15:28:58.000000 Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11608 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)     2290 2023-06-12 16:21:03.000000 Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    11474 2023-06-12 19:37:22.000000 Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5080 2023-06-22 13:37:25.000000 Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_image.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.64.7/simba/pose_importers/sleap_csv_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/pose_importers/misc/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.64.7/simba/pose_importers/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.64.7/simba/pose_importers/misc/apt_trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.64.7/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.7/simba/pose_importers/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    12549 2023-05-17 20:32:56.000000 Simba-UW-tf-dev-1.64.7/simba/pose_importers/sleap_h5_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.64.7/simba/pose_importers/madlc_importer.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/pose_importers/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.64.7/simba/pose_importers/sleap_slp_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.64.7/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.7/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.64.7/simba/pose_importers/trk_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:39.000000 Simba-UW-tf-dev-1.64.7/simba/three_dimensions/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/three_dimensions/ui/
--rw-r--r--   0 simon      (501) staff       (20)     1747 2023-06-25 18:18:01.000000 Simba-UW-tf-dev-1.64.7/simba/three_dimensions/ui/define_px_to_mm_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/three_dimensions/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)     6777 2023-06-26 17:04:03.000000 Simba-UW-tf-dev-1.64.7/simba/three_dimensions/feature_extractors/generic_feature_extractor.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/three_dimensions/mixins/
--rw-r--r--   0 simon      (501) staff       (20)    38820 2023-06-23 01:28:48.000000 Simba-UW-tf-dev-1.64.7/simba/three_dimensions/mixins/config_reader.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/three_dimensions/mixins/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)    51001 2023-06-26 13:52:31.000000 Simba-UW-tf-dev-1.64.7/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    50997 2023-06-25 19:59:06.000000 Simba-UW-tf-dev-1.64.7/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1380 2023-06-26 13:52:31.000000 Simba-UW-tf-dev-1.64.7/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     1379 2023-06-25 19:59:06.000000 Simba-UW-tf-dev-1.64.7/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     3758 2023-06-26 13:45:44.000000 Simba-UW-tf-dev-1.64.7/simba/three_dimensions/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     3953 2023-06-25 18:18:01.000000 Simba-UW-tf-dev-1.64.7/simba/three_dimensions/mixins/plotting_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/three_dimensions/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     3192 2023-06-25 18:21:24.000000 Simba-UW-tf-dev-1.64.7/simba/three_dimensions/plotting/plot_pose_in_dir.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/three_dimensions/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     3445 2023-06-22 22:21:05.000000 Simba-UW-tf-dev-1.64.7/simba/three_dimensions/pose_importers/anipose_csv_import.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/three_dimensions/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     5832 2023-06-23 13:06:19.000000 Simba-UW-tf-dev-1.64.7/simba/three_dimensions/outlier_tools/outlier_corrector_movement.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/video_processors/
--rw-r--r--   0 simon      (501) staff       (20)    59883 2023-07-05 17:43:17.000000 Simba-UW-tf-dev-1.64.7/simba/video_processors/video_processing.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-07-06 15:33:05.000000 Simba-UW-tf-dev-1.64.7/simba/video_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.64.7/simba/video_processors/px_to_mm.py
--rw-r--r--   0 simon      (501) staff       (20)    25424 2023-07-05 13:32:03.000000 Simba-UW-tf-dev-1.64.7/simba/video_processors/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     3748 2023-07-02 21:12:43.000000 Simba-UW-tf-dev-1.64.7/simba/video_processors/video_processing_new.py
--rw-r--r--   0 simon      (501) staff       (20)     7610 2023-07-03 18:21:05.000000 Simba-UW-tf-dev-1.64.7/simba/video_processors/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.64.7/simba/video_processors/extract_frames.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/video_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.64.7/simba/video_processors/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.64.7/simba/video_processors/extract_seqframes.py
--rw-r--r--   0 simon      (501) staff       (20)    13078 2023-07-05 13:23:30.000000 Simba-UW-tf-dev-1.64.7/simba/video_processors/batch_process_create_ffmpeg_commands.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6535 2023-05-25 14:24:01.000000 Simba-UW-tf-dev-1.64.7/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:37.000000 Simba-UW-tf-dev-1.64.7/simba/outlier_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8168 2023-06-01 12:38:34.000000 Simba-UW-tf-dev-1.64.7/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     2668 2023-05-25 14:26:49.000000 Simba-UW-tf-dev-1.64.7/simba/outlier_tools/skip_outlier_correction.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/outlier_tools/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/outlier_tools/.idea/outlier_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/outlier_tools/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/outlier_tools/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/outlier_tools/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/outlier_tools/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/outlier_tools/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/outlier_tools/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/outlier_tools/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    66845 2023-07-06 16:27:17.000000 Simba-UW-tf-dev-1.64.7/simba/SimBA.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:39.000000 Simba-UW-tf-dev-1.64.7/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:39.000000 Simba-UW-tf-dev-1.64.7/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:39.000000 Simba-UW-tf-dev-1.64.7/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
--rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-06-15 21:18:05.000000 Simba-UW-tf-dev-1.64.7/simba/assets/shap/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    16388 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.64.7/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:39.000000 Simba-UW-tf-dev-1.64.7/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/lookups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.64.7/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/lookups/unsupervised_example_x.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:39.000000 Simba-UW-tf-dev-1.64.7/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.64.7/simba/assets/img/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.64.7/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.64.7/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.64.7/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:39.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/gif.png
--rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/pose.png
--rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/.DS_Store
--rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/stopwatch.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/dimensionality_reduction.png
--rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/restart.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/add_on.png
--rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/print.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:39.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/clean.png
--rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/clf_2.png
--rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/boris.png
--rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/clahe.png
--rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/about.png
--rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/reorganize.png
--rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/TheGoldenLab.PNG
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:39.000000 Simba-UW-tf-dev-1.64.7/Simba_UW_tf_dev.egg-info/
--rw-rw-r--   0 simon      (501) staff       (20)      579 2023-07-06 16:46:39.000000 Simba-UW-tf-dev-1.64.7/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-rw-r--   0 simon      (501) staff       (20)    21717 2023-07-06 16:46:39.000000 Simba-UW-tf-dev-1.64.7/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 simon      (501) staff       (20)       44 2023-07-06 16:46:39.000000 Simba-UW-tf-dev-1.64.7/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-rw-r--   0 simon      (501) staff       (20)      639 2023-07-06 16:46:39.000000 Simba-UW-tf-dev-1.64.7/Simba_UW_tf_dev.egg-info/requires.txt
--rw-rw-r--   0 simon      (501) staff       (20)       12 2023-07-06 16:46:39.000000 Simba-UW-tf-dev-1.64.7/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-rw-r--   0 simon      (501) staff       (20)        1 2023-07-06 16:46:39.000000 Simba-UW-tf-dev-1.64.7/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.64.7/LICENSE.md
--rw-r--r--   0 simon      (501) staff       (20)       89 2023-05-20 17:55:56.000000 Simba-UW-tf-dev-1.64.7/pyproject.toml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/tests/
--rw-r--r--   0 simon      (501) staff       (20)     5209 2023-05-28 14:15:24.000000 Simba-UW-tf-dev-1.64.7/tests/test_data_processors.py
--rw-r--r--   0 simon      (501) staff       (20)     5317 2023-05-31 19:40:16.000000 Simba-UW-tf-dev-1.64.7/tests/test_distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-13 13:57:45.000000 Simba-UW-tf-dev-1.64.7/tests/test_interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)    12374 2023-06-07 20:44:17.000000 Simba-UW-tf-dev-1.64.7/tests/test_train_model_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     2470 2023-06-12 20:51:29.000000 Simba-UW-tf-dev-1.64.7/tests/test_pose_importers.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.7/tests/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6757 2023-06-02 12:11:53.000000 Simba-UW-tf-dev-1.64.7/tests/test_feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-12 20:53:51.000000 Simba-UW-tf-dev-1.64.7/tests/test_pose_processors.py
--rw-r--r--   0 simon      (501) staff       (20)     1774 2023-06-13 19:27:04.000000 Simba-UW-tf-dev-1.64.7/tests/test_utils_data.py
--rw-r--r--   0 simon      (501) staff       (20)     8984 2023-06-07 20:11:11.000000 Simba-UW-tf-dev-1.64.7/tests/test_config_reader_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     1528 2023-05-25 14:26:19.000000 Simba-UW-tf-dev-1.64.7/tests/test_outlier_correctors.py
--rw-r--r--   0 simon      (501) staff       (20)     4356 2023-05-29 20:59:49.000000 Simba-UW-tf-dev-1.64.7/tests/test_visualize_directing_animals.py
--rw-r--r--   0 simon      (501) staff       (20)     1859 2023-05-21 16:40:19.000000 Simba-UW-tf-dev-1.64.7/tests/test_featurizers.py
--rw-r--r--   0 simon      (501) staff       (20)     8736 2023-06-13 13:49:50.000000 Simba-UW-tf-dev-1.64.7/tests/test_video_processors.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/tests/data/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.7/tests/data/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/two_c57/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/two_c57/video_processing/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/two_c57/video_processing/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/two_c57/video_processing/test_imgs/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/two_c57/video_processing/test_imgs/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/two_c57/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/two_c57/models/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/two_c57/models/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/two_c57/expected_animal_bp_dict/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/two_c57/expected_animal_bp_dict/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/mouse_open_field/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/mouse_open_field/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/zebrafish/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/zebrafish/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/zebrafish/models/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/zebrafish/models/generated_models/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/zebrafish/models/generated_models/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/zebrafish/models/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/zebrafish/models/validations/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/zebrafish/models/validations/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/zebrafish/project_folder/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/zebrafish/project_folder/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/zebrafish/project_folder/videos/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/zebrafish/project_folder/videos/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/zebrafish/project_folder/logs/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/zebrafish/project_folder/logs/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/zebrafish/project_folder/logs/measures/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/zebrafish/project_folder/logs/measures/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/zebrafish/feature_file/
--rw-rw-r--   0 simon      (501) staff       (20)        0 2020-08-11 16:11:18.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/zebrafish/feature_file/__init__.py
--rw-rw-r--   0 simon      (501) staff       (20)    14128 2022-04-11 08:07:36.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py
--rw-r--r--   0 simon      (501) staff       (20)     3971 2023-05-28 17:20:18.000000 Simba-UW-tf-dev-1.64.7/tests/test_thirdparty_appenders.py
--rw-r--r--   0 simon      (501) staff       (20)     3090 2023-05-31 15:49:24.000000 Simba-UW-tf-dev-1.64.7/tests/test_validation_clips.py
--rw-r--r--   0 simon      (501) staff       (20)     4463 2023-06-12 18:41:18.000000 Simba-UW-tf-dev-1.64.7/tests/test_roi_tools.py
--rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.64.7/MANIFEST.in
--rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.64.7/README.md
--rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-07-06 16:44:59.000000 Simba-UW-tf-dev-1.64.7/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:50.000000 Simba-UW-tf-dev-1.64.8/simba/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/simba/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-07-06 15:33:05.000000 Simba-UW-tf-dev-1.64.8/simba/ui/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)     9015 2023-06-29 20:55:17.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/mutual_exclusivity_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/csv_2_parquet_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/quick_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/batch_preprocess_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/heatmap_location_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/clf_probability_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/movement_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/clf_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    15950 2023-05-20 12:10:35.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1150 2023-05-25 18:21:39.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/remove_roi_features_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5814 2023-06-15 20:06:37.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/roi_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5977 2023-05-31 12:58:14.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/outlier_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/gantt_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/clf_validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7721 2023-05-24 15:18:33.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/severity_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/fsttc_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/kleinberg_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7288 2023-05-29 20:14:50.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/pose_reorganizer_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/clf_by_timebins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/heatmap_clf_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/data_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/roi_features_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/pup_retrieval_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/about_simba_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3605 2023-05-25 18:54:56.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6353 2023-05-24 15:31:12.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    50444 2023-07-05 17:57:07.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/video_processing_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/clf_by_roi_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/make_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/archive_files_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/pose_bp_drop_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    10695 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/distance_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4573 2023-07-07 20:33:35.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    12869 2023-05-23 12:47:59.000000 Simba-UW-tf-dev-1.64.8/simba/ui/video_info_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.64.8/simba/ui/user_defined_pose_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/ui/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12879 2023-06-18 20:27:37.000000 Simba-UW-tf-dev-1.64.8/simba/ui/create_project_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.64.8/simba/ui/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    35431 2023-06-13 17:24:57.000000 Simba-UW-tf-dev-1.64.8/simba/ui/machine_model_settings_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:50.000000 Simba-UW-tf-dev-1.64.8/simba/blob_storage/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.64.8/simba/blob_storage/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:50.000000 Simba-UW-tf-dev-1.64.8/simba/labelling/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.64.8/simba/labelling/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21667 2023-06-20 18:30:00.000000 Simba-UW-tf-dev-1.64.8/simba/labelling/labelling_interface_old.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/labelling/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    20914 2023-06-22 13:26:28.000000 Simba-UW-tf-dev-1.64.8/simba/labelling/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     3568 2023-05-19 11:18:49.000000 Simba-UW-tf-dev-1.64.8/simba/labelling/extract_labelled_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)    26943 2023-06-20 19:04:35.000000 Simba-UW-tf-dev-1.64.8/simba/labelling/labelling_advanced_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.64.8/simba/labelling/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.64.8/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.64.8/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-13 17:25:39.000000 Simba-UW-tf-dev-1.64.8/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.64.8/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.64.8/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.64.8/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     9846 2023-06-06 18:27:30.000000 Simba-UW-tf-dev-1.64.8/simba/unsupervised/ui.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/unsupervised/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.64.8/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.64.8/simba/unsupervised/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.64.8/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.64.8/simba/unsupervised/cluster_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.64.8/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)    10287 2023-06-06 17:50:12.000000 Simba-UW-tf-dev-1.64.8/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.64.8/simba/unsupervised/tsne.py
+-rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.64.8/simba/unsupervised/cluster_visualizer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:50.000000 Simba-UW-tf-dev-1.64.8/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.8/simba/bounding_box_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/bounding_box_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.64.8/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.64.8/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.64.8/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.8/simba/bounding_box_tools/find_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.8/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    49156 2023-07-06 15:33:05.000000 Simba-UW-tf-dev-1.64.8/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:50.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:50.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7127 2023-05-28 19:41:35.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-07 20:28:11.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)      421 2023-07-05 19:50:18.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/shap_gpu.py
+-rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     8943 2023-06-05 18:15:28.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/shap_log_mp_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8580 2023-05-31 20:02:32.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/shap_log_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)    30764 2023-06-13 17:23:34.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     4279 2023-06-01 12:49:14.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/read_files_mp_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:44:29.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-07-06 15:33:05.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3864 2023-05-19 19:41:40.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    22875 2023-07-07 20:39:37.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8244 2023-05-21 16:28:49.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/feature_extractor_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/feature_extractor_4bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:50.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/.idea/features_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:50.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:50.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/.idea/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/.idea/.name
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/feature_extractors/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    15434 2023-05-20 18:29:53.000000 Simba-UW-tf-dev-1.64.8/simba/requirements.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:50.000000 Simba-UW-tf-dev-1.64.8/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-07-06 15:33:05.000000 Simba-UW-tf-dev-1.64.8/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43029 2023-06-05 17:40:09.000000 Simba-UW-tf-dev-1.64.8/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    38471 2023-07-07 19:58:19.000000 Simba-UW-tf-dev-1.64.8/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/mixins/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.64.8/simba/mixins/pose_importer_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     2938 2023-07-02 20:03:29.000000 Simba-UW-tf-dev-1.64.8/simba/mixins/video_processing_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:50.000000 Simba-UW-tf-dev-1.64.8/simba/mixins/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.64.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.64.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.64.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    82442 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.64.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    51809 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.64.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    14391 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.64.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    14188 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.64.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    37135 2023-06-02 12:12:15.000000 Simba-UW-tf-dev-1.64.8/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    61873 2023-05-19 21:14:46.000000 Simba-UW-tf-dev-1.64.8/simba/mixins/plotting_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     9145 2023-06-13 18:36:10.000000 Simba-UW-tf-dev-1.64.8/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    73291 2023-06-19 20:46:57.000000 Simba-UW-tf-dev-1.64.8/simba/mixins/train_model_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6094 2023-05-21 17:39:19.000000 Simba-UW-tf-dev-1.64.8/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10759 2023-06-08 22:23:03.000000 Simba-UW-tf-dev-1.64.8/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.64.8/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.8/simba/third_party_label_appenders/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    18417 2023-06-18 19:01:16.000000 Simba-UW-tf-dev-1.64.8/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.64.8/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18934 2023-06-18 19:03:04.000000 Simba-UW-tf-dev-1.64.8/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8181 2023-05-21 17:19:25.000000 Simba-UW-tf-dev-1.64.8/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     6988 2023-05-21 17:31:04.000000 Simba-UW-tf-dev-1.64.8/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5239 2023-05-21 18:07:18.000000 Simba-UW-tf-dev-1.64.8/simba/third_party_label_appenders/solomon_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:50.000000 Simba-UW-tf-dev-1.64.8/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.8/simba/cue_light_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.8/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.8/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.8/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.8/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.64.8/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.8/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)    11876 2023-06-18 20:21:39.000000 Simba-UW-tf-dev-1.64.8/simba/utils/config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    21103 2023-06-20 12:58:32.000000 Simba-UW-tf-dev-1.64.8/simba/utils/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-07-06 15:33:05.000000 Simba-UW-tf-dev-1.64.8/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7801 2023-07-05 17:33:58.000000 Simba-UW-tf-dev-1.64.8/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)    10349 2023-07-07 20:04:33.000000 Simba-UW-tf-dev-1.64.8/simba/utils/checks.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/utils/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    43615 2023-07-05 18:25:40.000000 Simba-UW-tf-dev-1.64.8/simba/utils/read_write.py
+-rw-r--r--   0 simon      (501) staff       (20)     9841 2023-06-19 23:24:08.000000 Simba-UW-tf-dev-1.64.8/simba/utils/lookups.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/simba/utils/cli/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/utils/cli/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6017 2023-05-28 13:41:20.000000 Simba-UW-tf-dev-1.64.8/simba/utils/cli/cli_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    15116 2023-07-05 17:33:58.000000 Simba-UW-tf-dev-1.64.8/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)    19250 2023-06-13 13:46:20.000000 Simba-UW-tf-dev-1.64.8/simba/utils/data.py
+-rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.64.8/simba/utils/printing.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/simba/st/
+-rw-r--r--   0 simon      (501) staff       (20)      282 2023-06-16 17:26:25.000000 Simba-UW-tf-dev-1.64.8/simba/st/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-16 13:55:39.000000 Simba-UW-tf-dev-1.64.8/simba/st/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2102 2023-06-19 19:54:19.000000 Simba-UW-tf-dev-1.64.8/simba/st/select_groups_pg.py
+-rw-r--r--   0 simon      (501) staff       (20)     2325 2023-06-19 19:54:19.000000 Simba-UW-tf-dev-1.64.8/simba/st/aggregate_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     1485 2023-06-16 18:20:31.000000 Simba-UW-tf-dev-1.64.8/simba/st/app.py
+-rw-r--r--   0 simon      (501) staff       (20)      249 2023-06-16 18:20:19.000000 Simba-UW-tf-dev-1.64.8/simba/st/welcome_page.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/simba/pose_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.64.8/simba/pose_processors/reorganize_keypoint.py
+-rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.64.8/simba/pose_processors/remove_keypoints.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.8/simba/pose_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/pose_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.64.8/simba/pose_processors/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)     5618 2023-06-13 18:36:10.000000 Simba-UW-tf-dev-1.64.8/simba/pose_processors/reverse_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.64.8/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.64.8/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    13008 2023-05-24 15:32:44.000000 Simba-UW-tf-dev-1.64.8/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.64.8/simba/plotting/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.64.8/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.64.8/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.64.8/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.64.8/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12484 2023-05-23 14:52:24.000000 Simba-UW-tf-dev-1.64.8/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    14056 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.64.8/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.64.8/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.64.8/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.64.8/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/plotting/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.64.8/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)    14029 2023-06-04 11:55:47.000000 Simba-UW-tf-dev-1.64.8/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)    14824 2023-07-05 12:33:51.000000 Simba-UW-tf-dev-1.64.8/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)     7660 2023-06-20 12:45:11.000000 Simba-UW-tf-dev-1.64.8/simba/plotting/pose_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     7891 2023-05-29 21:41:05.000000 Simba-UW-tf-dev-1.64.8/simba/plotting/Directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.64.8/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    15745 2023-05-20 12:16:06.000000 Simba-UW-tf-dev-1.64.8/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11203 2023-05-24 15:35:24.000000 Simba-UW-tf-dev-1.64.8/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.64.8/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13471 2023-05-20 12:15:46.000000 Simba-UW-tf-dev-1.64.8/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.64.8/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    11519 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.64.8/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.64.8/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.64.8/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     9385 2023-05-31 16:46:49.000000 Simba-UW-tf-dev-1.64.8/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     9526 2023-06-04 12:03:25.000000 Simba-UW-tf-dev-1.64.8/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10005 2023-05-29 21:36:37.000000 Simba-UW-tf-dev-1.64.8/simba/plotting/Directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.64.8/simba/plotting/heat_mapper_location_mp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:50.000000 Simba-UW-tf-dev-1.64.8/simba/dash_app/
+-rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/dash_app/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/dash_app/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/dash_app/dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-16 12:50:41.000000 Simba-UW-tf-dev-1.64.8/simba/dash_app/plotly_dash.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:50.000000 Simba-UW-tf-dev-1.64.8/simba/data_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     7248 2023-05-25 19:01:00.000000 Simba-UW-tf-dev-1.64.8/simba/data_processors/agg_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.64.8/simba/data_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    11196 2023-05-28 19:50:35.000000 Simba-UW-tf-dev-1.64.8/simba/data_processors/severity_bout_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16285 2023-06-13 13:57:45.000000 Simba-UW-tf-dev-1.64.8/simba/data_processors/interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8127 2023-05-25 13:57:19.000000 Simba-UW-tf-dev-1.64.8/simba/data_processors/timebins_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    13451 2023-06-19 20:47:55.000000 Simba-UW-tf-dev-1.64.8/simba/data_processors/fsttc_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/data_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.64.8/simba/data_processors/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.64.8/simba/data_processors/directing_other_animals_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8624 2023-05-25 14:07:56.000000 Simba-UW-tf-dev-1.64.8/simba/data_processors/timebins_movement_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.64.8/simba/data_processors/severity_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.64.8/simba/data_processors/pup_retrieval_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.64.8/simba/data_processors/pybursts_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    11533 2023-05-28 19:50:34.000000 Simba-UW-tf-dev-1.64.8/simba/data_processors/severity_frame_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     6087 2023-06-28 20:32:32.000000 Simba-UW-tf-dev-1.64.8/simba/data_processors/mutual_exclusivity_corrector.py
+-rw-r--r--   0 simon      (501) staff       (20)     9656 2023-05-25 13:32:25.000000 Simba-UW-tf-dev-1.64.8/simba/data_processors/kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8131 2023-05-25 14:37:36.000000 Simba-UW-tf-dev-1.64.8/simba/data_processors/movement_calculator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:50.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:50.000000 Simba-UW-tf-dev-1.64.8/simba/model/
+-rw-r--r--   0 simon      (501) staff       (20)    20086 2023-06-05 20:43:28.000000 Simba-UW-tf-dev-1.64.8/simba/model/train_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.8/simba/model/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3315 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.64.8/simba/model/inference_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    20849 2023-06-05 18:44:40.000000 Simba-UW-tf-dev-1.64.8/simba/model/grid_search_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3363 2023-05-19 11:12:45.000000 Simba-UW-tf-dev-1.64.8/simba/model/inference_validation.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.64.8/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.64.8/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.8/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43194 2023-06-22 13:51:00.000000 Simba-UW-tf-dev-1.64.8/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.64.8/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    20174 2023-06-12 15:28:58.000000 Simba-UW-tf-dev-1.64.8/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11608 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.64.8/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.64.8/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)     2290 2023-06-12 16:21:03.000000 Simba-UW-tf-dev-1.64.8/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    11474 2023-06-12 19:37:22.000000 Simba-UW-tf-dev-1.64.8/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5080 2023-06-22 13:37:25.000000 Simba-UW-tf-dev-1.64.8/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.64.8/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.64.8/simba/roi_tools/ROI_image.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.64.8/simba/pose_importers/sleap_csv_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/simba/pose_importers/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.64.8/simba/pose_importers/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.64.8/simba/pose_importers/misc/apt_trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.64.8/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.8/simba/pose_importers/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    12549 2023-05-17 20:32:56.000000 Simba-UW-tf-dev-1.64.8/simba/pose_importers/sleap_h5_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.64.8/simba/pose_importers/madlc_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/pose_importers/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.64.8/simba/pose_importers/sleap_slp_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.64.8/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.8/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.64.8/simba/pose_importers/trk_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/pose_configurations/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:50.000000 Simba-UW-tf-dev-1.64.8/simba/three_dimensions/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/simba/three_dimensions/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     1747 2023-06-25 18:18:01.000000 Simba-UW-tf-dev-1.64.8/simba/three_dimensions/ui/define_px_to_mm_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/simba/three_dimensions/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)     6777 2023-06-26 17:04:03.000000 Simba-UW-tf-dev-1.64.8/simba/three_dimensions/feature_extractors/generic_feature_extractor.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/simba/three_dimensions/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)    38820 2023-06-23 01:28:48.000000 Simba-UW-tf-dev-1.64.8/simba/three_dimensions/mixins/config_reader.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/simba/three_dimensions/mixins/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)    51001 2023-06-26 13:52:31.000000 Simba-UW-tf-dev-1.64.8/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    50997 2023-06-25 19:59:06.000000 Simba-UW-tf-dev-1.64.8/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1380 2023-06-26 13:52:31.000000 Simba-UW-tf-dev-1.64.8/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     1379 2023-06-25 19:59:06.000000 Simba-UW-tf-dev-1.64.8/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     3758 2023-06-26 13:45:44.000000 Simba-UW-tf-dev-1.64.8/simba/three_dimensions/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     3953 2023-06-25 18:18:01.000000 Simba-UW-tf-dev-1.64.8/simba/three_dimensions/mixins/plotting_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/simba/three_dimensions/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     3192 2023-06-25 18:21:24.000000 Simba-UW-tf-dev-1.64.8/simba/three_dimensions/plotting/plot_pose_in_dir.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/simba/three_dimensions/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     3445 2023-06-22 22:21:05.000000 Simba-UW-tf-dev-1.64.8/simba/three_dimensions/pose_importers/anipose_csv_import.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/simba/three_dimensions/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5832 2023-06-23 13:06:19.000000 Simba-UW-tf-dev-1.64.8/simba/three_dimensions/outlier_tools/outlier_corrector_movement.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/simba/video_processors/
+-rw-r--r--   0 simon      (501) staff       (20)    59883 2023-07-05 17:43:17.000000 Simba-UW-tf-dev-1.64.8/simba/video_processors/video_processing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-07-06 15:33:05.000000 Simba-UW-tf-dev-1.64.8/simba/video_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.64.8/simba/video_processors/px_to_mm.py
+-rw-r--r--   0 simon      (501) staff       (20)    25424 2023-07-05 13:32:03.000000 Simba-UW-tf-dev-1.64.8/simba/video_processors/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     3748 2023-07-02 21:12:43.000000 Simba-UW-tf-dev-1.64.8/simba/video_processors/video_processing_new.py
+-rw-r--r--   0 simon      (501) staff       (20)     7610 2023-07-03 18:21:05.000000 Simba-UW-tf-dev-1.64.8/simba/video_processors/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.64.8/simba/video_processors/extract_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/video_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.64.8/simba/video_processors/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.64.8/simba/video_processors/extract_seqframes.py
+-rw-r--r--   0 simon      (501) staff       (20)    13078 2023-07-05 13:23:30.000000 Simba-UW-tf-dev-1.64.8/simba/video_processors/batch_process_create_ffmpeg_commands.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:50.000000 Simba-UW-tf-dev-1.64.8/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6535 2023-05-25 14:24:01.000000 Simba-UW-tf-dev-1.64.8/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:37.000000 Simba-UW-tf-dev-1.64.8/simba/outlier_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8168 2023-06-01 12:38:34.000000 Simba-UW-tf-dev-1.64.8/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     2668 2023-05-25 14:26:49.000000 Simba-UW-tf-dev-1.64.8/simba/outlier_tools/skip_outlier_correction.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:50.000000 Simba-UW-tf-dev-1.64.8/simba/outlier_tools/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/outlier_tools/.idea/outlier_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/outlier_tools/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:50.000000 Simba-UW-tf-dev-1.64.8/simba/outlier_tools/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:50.000000 Simba-UW-tf-dev-1.64.8/simba/outlier_tools/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/outlier_tools/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/outlier_tools/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/outlier_tools/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/outlier_tools/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    66845 2023-07-06 16:27:17.000000 Simba-UW-tf-dev-1.64.8/simba/SimBA.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:50.000000 Simba-UW-tf-dev-1.64.8/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:50.000000 Simba-UW-tf-dev-1.64.8/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/assets/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:50.000000 Simba-UW-tf-dev-1.64.8/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:50.000000 Simba-UW-tf-dev-1.64.8/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-06-15 21:18:05.000000 Simba-UW-tf-dev-1.64.8/simba/assets/shap/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    16388 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.64.8/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:50.000000 Simba-UW-tf-dev-1.64.8/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/assets/lookups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.64.8/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/assets/lookups/unsupervised_example_x.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:50.000000 Simba-UW-tf-dev-1.64.8/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:50.000000 Simba-UW-tf-dev-1.64.8/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.64.8/simba/assets/img/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.64.8/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.64.8/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.64.8/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:50.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/gif.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/pose.png
+-rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/.DS_Store
+-rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/stopwatch.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/dimensionality_reduction.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/restart.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/add_on.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/print.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:50.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/clean.png
+-rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/clf_2.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/boris.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/clahe.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/about.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/reorganize.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.64.8/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.8/simba/assets/TheGoldenLab.PNG
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:50.000000 Simba-UW-tf-dev-1.64.8/Simba_UW_tf_dev.egg-info/
+-rw-rw-r--   0 simon      (501) staff       (20)      579 2023-07-07 20:40:49.000000 Simba-UW-tf-dev-1.64.8/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 simon      (501) staff       (20)    21717 2023-07-07 20:40:50.000000 Simba-UW-tf-dev-1.64.8/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       44 2023-07-07 20:40:49.000000 Simba-UW-tf-dev-1.64.8/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-rw-r--   0 simon      (501) staff       (20)      639 2023-07-07 20:40:49.000000 Simba-UW-tf-dev-1.64.8/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       12 2023-07-07 20:40:49.000000 Simba-UW-tf-dev-1.64.8/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        1 2023-07-07 20:40:49.000000 Simba-UW-tf-dev-1.64.8/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.64.8/LICENSE.md
+-rw-r--r--   0 simon      (501) staff       (20)       89 2023-05-20 17:55:56.000000 Simba-UW-tf-dev-1.64.8/pyproject.toml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/tests/
+-rw-r--r--   0 simon      (501) staff       (20)     5209 2023-05-28 14:15:24.000000 Simba-UW-tf-dev-1.64.8/tests/test_data_processors.py
+-rw-r--r--   0 simon      (501) staff       (20)     5317 2023-05-31 19:40:16.000000 Simba-UW-tf-dev-1.64.8/tests/test_distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-13 13:57:45.000000 Simba-UW-tf-dev-1.64.8/tests/test_interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)    12374 2023-06-07 20:44:17.000000 Simba-UW-tf-dev-1.64.8/tests/test_train_model_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     2470 2023-06-12 20:51:29.000000 Simba-UW-tf-dev-1.64.8/tests/test_pose_importers.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.8/tests/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6757 2023-06-02 12:11:53.000000 Simba-UW-tf-dev-1.64.8/tests/test_feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-12 20:53:51.000000 Simba-UW-tf-dev-1.64.8/tests/test_pose_processors.py
+-rw-r--r--   0 simon      (501) staff       (20)     1774 2023-06-13 19:27:04.000000 Simba-UW-tf-dev-1.64.8/tests/test_utils_data.py
+-rw-r--r--   0 simon      (501) staff       (20)     8984 2023-06-07 20:11:11.000000 Simba-UW-tf-dev-1.64.8/tests/test_config_reader_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     1528 2023-05-25 14:26:19.000000 Simba-UW-tf-dev-1.64.8/tests/test_outlier_correctors.py
+-rw-r--r--   0 simon      (501) staff       (20)     4356 2023-05-29 20:59:49.000000 Simba-UW-tf-dev-1.64.8/tests/test_visualize_directing_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)     1859 2023-05-21 16:40:19.000000 Simba-UW-tf-dev-1.64.8/tests/test_featurizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     8736 2023-06-13 13:49:50.000000 Simba-UW-tf-dev-1.64.8/tests/test_video_processors.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/tests/data/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.8/tests/data/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/tests/data/test_projects/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/tests/data/test_projects/two_c57/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/tests/data/test_projects/two_c57/video_processing/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.8/tests/data/test_projects/two_c57/video_processing/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/tests/data/test_projects/two_c57/video_processing/test_imgs/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.8/tests/data/test_projects/two_c57/video_processing/test_imgs/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.8/tests/data/test_projects/two_c57/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/tests/data/test_projects/two_c57/models/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.8/tests/data/test_projects/two_c57/models/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/tests/data/test_projects/two_c57/expected_animal_bp_dict/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.8/tests/data/test_projects/two_c57/expected_animal_bp_dict/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.8/tests/data/test_projects/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/tests/data/test_projects/mouse_open_field/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.8/tests/data/test_projects/mouse_open_field/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/tests/data/test_projects/zebrafish/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.8/tests/data/test_projects/zebrafish/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/tests/data/test_projects/zebrafish/models/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/tests/data/test_projects/zebrafish/models/generated_models/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.8/tests/data/test_projects/zebrafish/models/generated_models/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.8/tests/data/test_projects/zebrafish/models/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/tests/data/test_projects/zebrafish/models/validations/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.8/tests/data/test_projects/zebrafish/models/validations/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/tests/data/test_projects/zebrafish/project_folder/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.8/tests/data/test_projects/zebrafish/project_folder/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/tests/data/test_projects/zebrafish/project_folder/videos/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.8/tests/data/test_projects/zebrafish/project_folder/videos/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/tests/data/test_projects/zebrafish/project_folder/logs/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.8/tests/data/test_projects/zebrafish/project_folder/logs/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/tests/data/test_projects/zebrafish/project_folder/logs/measures/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.8/tests/data/test_projects/zebrafish/project_folder/logs/measures/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/tests/data/test_projects/zebrafish/feature_file/
+-rw-rw-r--   0 simon      (501) staff       (20)        0 2020-08-11 16:11:18.000000 Simba-UW-tf-dev-1.64.8/tests/data/test_projects/zebrafish/feature_file/__init__.py
+-rw-rw-r--   0 simon      (501) staff       (20)    14128 2022-04-11 08:07:36.000000 Simba-UW-tf-dev-1.64.8/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py
+-rw-r--r--   0 simon      (501) staff       (20)     3971 2023-05-28 17:20:18.000000 Simba-UW-tf-dev-1.64.8/tests/test_thirdparty_appenders.py
+-rw-r--r--   0 simon      (501) staff       (20)     3090 2023-05-31 15:49:24.000000 Simba-UW-tf-dev-1.64.8/tests/test_validation_clips.py
+-rw-r--r--   0 simon      (501) staff       (20)     4463 2023-06-12 18:41:18.000000 Simba-UW-tf-dev-1.64.8/tests/test_roi_tools.py
+-rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.64.8/MANIFEST.in
+-rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.64.8/README.md
+-rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-07-07 20:40:04.000000 Simba-UW-tf-dev-1.64.8/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-07-07 20:40:51.000000 Simba-UW-tf-dev-1.64.8/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.64.7/PKG-INFO` & `Simba-UW-tf-dev-1.64.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.64.7
+Version: 1.64.8
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/.DS_Store` & `Simba-UW-tf-dev-1.64.8/simba/ui/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/mutual_exclusivity_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/mutual_exclusivity_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/csv_2_parquet_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/csv_2_parquet_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/quick_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/quick_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/batch_preprocess_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/batch_preprocess_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/heatmap_location_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/heatmap_location_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/clf_probability_plot_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/clf_probability_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/.DS_Store` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/movement_analysis_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/movement_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/clf_plot_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/clf_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/path_plot_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/remove_roi_features_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/remove_roi_features_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/smoothing_interpolation_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/smoothing_interpolation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/roi_analysis_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/roi_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/outlier_settings_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/outlier_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/gantt_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/gantt_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/clf_validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/clf_validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/severity_analysis_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/severity_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/fsttc_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/fsttc_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/kleinberg_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/kleinberg_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/pose_reorganizer_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/pose_reorganizer_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/append_roi_features_animals_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/append_roi_features_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/clf_by_timebins_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/clf_by_timebins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/heatmap_clf_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/heatmap_clf_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/data_plot_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/data_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/roi_features_plot_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/roi_features_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/pup_retrieval_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/pup_retrieval_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/about_simba_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/about_simba_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/roi_tracking_plot_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/roi_tracking_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/clf_add_remove_print_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/clf_add_remove_print_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/video_processing_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/video_processing_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/clf_by_roi_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/clf_by_roi_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/make_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/make_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/archive_files_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/archive_files_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/pose_bp_drop_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/pose_bp_drop_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/distance_plot_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/distance_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/subset_feature_extractor_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/subset_feature_extractor_pop_up.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,56 +1,73 @@
 __author__ = "Simon Nilsson"
 
+import os.path
 from tkinter import *
 
 from simba.mixins.pop_up_mixin import PopUpMixin
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.enums import Links
 from simba.ui.tkinter_functions import DropDownMenu, CreateLabelFrameWithIcon, FolderSelect
 from simba.utils.checks import check_if_dir_exists
 from simba.feature_extractors.feature_subsets import FeatureSubsetsCalculator
+from simba.utils.errors import InvalidInputError
 
 
 
 class FeatureSubsetExtractorPopUp(PopUpMixin, ConfigReader):
     def __init__(self,
                  config_path: str):
 
-        PopUpMixin.__init__(self, title='EXTRACT FEATURE SUBSETS', size=(500, 100))
+        PopUpMixin.__init__(self, title='EXTRACT FEATURE SUBSETS', size=(500, 500))
         ConfigReader.__init__(self, config_path=config_path)
         self.feature_subset_options = ['Two-point body-part distances (mm)',
                                        'Within-animal three-point body-part angles (degrees)',
                                        'Within-animal three-point convex hull perimeters (mm)',
                                        'Within-animal four-point convex hull perimeters (mm)',
                                        'Entire animal convex hull perimeters (mm)',
                                        'Entire animal convex hull area (mm2)',
                                        'Frame-by-frame body-part movements (mm)',
                                        'Frame-by-frame distance to ROI centers (mm)',
                                        'Frame-by-frame body-parts inside ROIs (Boolean)']
 
         self.settings_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header='SETTINGS', icon_name='documentation', icon_link=Links.FEATURE_SUBSETS.value)
-        self.feature_family_dropdown = DropDownMenu(self.settings_frm, 'FEATURE FAMILY:', self.feature_subset_options, '20')
-        self.feature_family_dropdown.setChoices(self.feature_subset_options[0])
         self.save_dir = FolderSelect(self.settings_frm, 'SAVE DIRECTORY:', lblwidth=20)
         self.append_to_features_extracted_var = BooleanVar(value=False)
         self.append_to_targets_inserted_var = BooleanVar(value=False)
+        self.include_file_checks = BooleanVar(value=False)
         self.append_to_features_cb = Checkbutton(self.settings_frm, text='APPEND RESULTS TO FEATURES EXTRACTED FILES', variable=self.append_to_features_extracted_var)
         self.append_to_targets_inserted_cb = Checkbutton(self.settings_frm, text='APPEND RESULTS TO TARGET INSERTED FILES', variable=self.append_to_targets_inserted_var)
-        self.create_run_frm(run_function=self.run)
+        self.include_file_checks_cb = Checkbutton(self.settings_frm, text='INCLUDE INTEGRITY CHECKS BEFORE APPENDING NEW DATA (RECOMMENDED)', variable=self.include_file_checks)
         self.settings_frm.grid(row=0, column=0, sticky=NW)
-        self.feature_family_dropdown.grid(row=0, column=0, sticky=NW)
         self.save_dir.grid(row=1, column=0, sticky=NW)
         self.append_to_features_cb.grid(row=2, column=0, sticky=NW)
         self.append_to_targets_inserted_cb.grid(row=3, column=0, sticky=NW)
+        self.include_file_checks_cb.grid(row=4, column=0, sticky=NW)
+        self.feature_subset_selections = self.create_cb_frame(main_frm=self.main_frm, cb_titles=self.feature_subset_options, frm_title='FEATURE SUB-SETS')
+        self.create_run_frm(run_function=self.run)
         #self.main_frm.mainloop()
 
     def run(self):
-        check_if_dir_exists(in_dir=self.save_dir.folder_path)
+
+        selected_features = []
+        for feature_name, feature_var in self.feature_subset_selections.items():
+            if feature_var.get():
+                selected_features.append(feature_name)
+        if len(selected_features) == 0:
+            raise InvalidInputError(msg='Please select at least ONE feature subset family.')
+        if not self.append_to_targets_inserted_var.get() and not self.append_to_features_extracted_var.get():
+            if not os.path.isdir(self.save_dir.folder_path):
+                raise InvalidInputError(msg='You must select a valid path where to save the results OR select to append the features to the targets_inserted and/or features_extracted files.')
+
+
+
+
         feature_extractor = FeatureSubsetsCalculator(config_path=self.config_path,
-                                                     feature_family=self.feature_family_dropdown.getChoices(),
+                                                     feature_families=selected_features,
                                                      save_dir=self.save_dir.folder_path,
+                                                     include_file_checks=self.include_file_checks.get(),
                                                      append_to_features_extracted=self.append_to_features_extracted_var.get(),
                                                      append_to_targets_inserted=self.append_to_targets_inserted_var.get())
         feature_extractor.run()
 
 
 #FeatureSubsetExtractorPopUp(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini')
```

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/video_info_ui.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/video_info_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/user_defined_pose_creator.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/user_defined_pose_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/create_project_ui.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/create_project_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/tkinter_functions.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/ui/machine_model_settings_ui.py` & `Simba-UW-tf-dev-1.64.8/simba/ui/machine_model_settings_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/blob_storage/.DS_Store` & `Simba-UW-tf-dev-1.64.8/simba/blob_storage/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/labelling/.DS_Store` & `Simba-UW-tf-dev-1.64.8/simba/labelling/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/labelling/labelling_interface_old.py` & `Simba-UW-tf-dev-1.64.8/simba/labelling/labelling_interface_old.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/labelling/labelling_interface.py` & `Simba-UW-tf-dev-1.64.8/simba/labelling/labelling_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/labelling/extract_labelled_frames.py` & `Simba-UW-tf-dev-1.64.8/simba/labelling/extract_labelled_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/labelling/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.64.8/simba/labelling/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/labelling/play_annotation_video.py` & `Simba-UW-tf-dev-1.64.8/simba/labelling/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.64.8/simba/unsupervised/dbcv_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.64.8/simba/unsupervised/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.64.8/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.64.8/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.64.8/simba/unsupervised/grid_search_visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.64.8/simba/unsupervised/data_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/unsupervised/ui.py` & `Simba-UW-tf-dev-1.64.8/simba/unsupervised/ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.64.8/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/unsupervised/pop_up_classes.py` & `Simba-UW-tf-dev-1.64.8/simba/unsupervised/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.64.8/simba/unsupervised/bout_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/unsupervised/cluster_statistics.py` & `Simba-UW-tf-dev-1.64.8/simba/unsupervised/cluster_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.64.8/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.64.8/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.64.8/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/unsupervised/cluster_visualizer.py` & `Simba-UW-tf-dev-1.64.8/simba/unsupervised/cluster_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/bounding_box_tools/.DS_Store` & `Simba-UW-tf-dev-1.64.8/simba/bounding_box_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.64.8/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.64.8/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.64.8/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/bounding_box_tools/find_boundaries.py` & `Simba-UW-tf-dev-1.64.8/simba/bounding_box_tools/find_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.64.8/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/.DS_Store` & `Simba-UW-tf-dev-1.64.8/simba/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.64.8/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.64.8/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/peaks.py` & `Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/.DS_Store` & `Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/shap_log_mp_2.py` & `Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/shap_log_mp_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/shap_log_mp.py` & `Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/shap_log_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py` & `Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/read_files_mp_2.py` & `Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/read_files_mp_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.64.8/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.64.8/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.64.8/simba/feature_extractors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.64.8/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.64.8/simba/data_processors/interpolation_smoothing.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,350 +1,270 @@
 __author__ = "Simon Nilsson"
 
-import pandas as pd
-import os
+from scipy.signal import savgol_filter
+import glob, os
 import numpy as np
-from typing import Union, Optional
+import pandas as pd
+import shutil
 try:
     from typing import Literal
-except:
+except ImportError:
     from typing_extensions import Literal
 
-from itertools import combinations
-from simba.feature_extractors.perimeter_jit import jitted_hull
-from simba.utils.enums import Formats, Options
 from simba.mixins.config_reader import ConfigReader
-from simba.mixins.feature_extraction_mixin import FeatureExtractionMixin
-from simba.utils.checks import check_if_filepath_list_is_empty, check_file_exist_and_readable
 from simba.utils.printing import stdout_success, SimbaTimer
-from simba.utils.read_write import get_fn_ext, read_df, write_df
-from simba.utils.errors import CountError, DataHeaderError
+from simba.utils.read_write import read_df, write_df, get_video_meta_data, get_fn_ext, find_video_of_file
+from simba.utils.checks import check_if_filepath_list_is_empty
+from simba.utils.enums import Methods
+from simba.utils.errors import NoFilesFoundError
 
 
-class FeatureSubsetsCalculator(ConfigReader, FeatureExtractionMixin):
+class Interpolate(ConfigReader):
     """
-    Computes a subset of features from pose for non-ML downstream purposes.
-    E.g., returns the size of animal convex hull in each frame.
+    Interpolate missing body-parts in pose-estimation data. "Missing" is defined as either (i) when a single body-parts is None, or
+    when all body-parts belonging to an animal are identical (i.e., the same 2D coordinate or all None).
 
-    :parameter str config_path: path to SimBA project config file in Configparser format
-    :parameter str save_dir: directory where to store results.
-    :parameter str feature_family: Feature subtype to calculate. E.g., "Two-point body-part distances (mm)".
+    :parameter str input_path: Directory or file path to pose-estimation data in CSV or parquet format
+    :parameter str config_path: path to SimBA project config file in Configparser format.
+    :parameter Literal str: Type of interpolation. OPTIONS: 'Animal(s): Nearest', 'Animal(s): Linear', 'Animal(s): Quadratic','Body-parts: Nearest', 'Body-parts: Linear', 'Body-parts: Quadratic']
+                            See `tutorial for info/images of the different interpolation types <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario1.md#to-import-multiple-dlc-csv-files>`__.
+    :parameter bool initial_import_multi_index: If True, the incoming data is multi-index columns dataframes. Default: False.
+
+    .. image:: _static/img/interpolation_comparison.png
+       :width: 400
+       :align: center
 
     .. note::
-       `Tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/feature_subsets.md>_`
+       `Interpolation tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario1.md#to-import-multiple-dlc-csv-files>`__.
 
     Examples
-    ----------
-    >>> _ = FeatureSubsetsCalculator(config_path='project_folder/project_config.ini', feature_family='Frame-by-frame body-parts inside ROIs (Boolean)', save_dir='data').run()
+    -----
+    >>> _ = Interpolate(input_path=data_path, config_path=SimBaProjectConfigPath, method='Animal(s): Nearest')
     """
 
+
     def __init__(self,
-                 config_path: Union[str, os.PathLike],
-                 save_dir: Union[str, os.PathLike],
-                 feature_family: Literal[Options.FEATURE_SUBSET_OPTIONS],
-                 append_to_features_extracted: Optional[bool] = False,
-                 append_to_targets_inserted: Optional[bool] = False):
-
-        FeatureExtractionMixin.__init__(self, config_path=config_path)
-        ConfigReader.__init__(self, config_path=config_path)
-        check_if_filepath_list_is_empty(
-            filepaths=self.outlier_corrected_paths,
-            error_msg=f"SIMBA ERROR: Zero data files found in {self.outlier_corrected_paths} directory",
-        )
-        self.feature_family, self.save_dir = feature_family, save_dir
-        self.append_to_features, self.append_to_targets = append_to_features_extracted, append_to_targets_inserted
-
-    def __get_bp_combinations(self):
-        self.two_point_combs = np.array(list(combinations(self.project_bps, 2)))
-        self.within_animal_three_point_combs = {}
-        self.within_animal_four_point_combs = {}
-        self.animal_bps = {}
-        for animal, animal_data in self.animal_bp_dict.items():
-            animal_bps = [x[:-2] for x in animal_data["X_bps"]]
-            self.animal_bps[animal] = animal_bps
-            self.within_animal_three_point_combs[animal] = np.array(
-                list(combinations(animal_bps, 3))
-            )
-            self.within_animal_four_point_combs[animal] = np.array(
-                list(combinations(animal_bps, 4))
-            )
-
-    def run(self):
-        self.__get_bp_combinations()
-        for file_path in self.outlier_corrected_paths:
-            self.current_file_path = file_path
-            self.video_timer = SimbaTimer(start=True)
-            self.results = pd.DataFrame()
-            _, self.video_name, _ = get_fn_ext(filepath=file_path)
-            print(f"Analyzing {self.video_name} ({self.feature_family})...")
-            _, self.pixel_per_mm, self.fps = self.read_video_info(
-                video_name=self.video_name
-            )
-            self.df = read_df(file_path=file_path, file_type=self.file_type)
-            if self.feature_family == "Two-point body-part distances (mm)":
-                self.calc_distances()
-            elif (
-                self.feature_family
-                == "Within-animal three-point body-part angles (degrees)"
-            ):
-                self.calc_angles()
-            elif (
-                self.feature_family
-                == "Within-animal three-point convex hull perimeters (mm)"
-            ):
-                self.calc_three_point_hulls()
-            elif (
-                self.feature_family
-                == "Within-animal four-point convex hull perimeters (mm)"
-            ):
-                self.calc_four_point_hulls()
-            elif self.feature_family == "Entire animal convex hull perimeters (mm)":
-                self.animal_convex_hulls()
-            elif self.feature_family == "Entire animal convex hull area (mm2)":
-                self.calc_animal_convex_hulls_area()
-            elif self.feature_family == "Frame-by-frame body-part movements (mm)":
-                self.calc_movements()
-            elif (
-                self.feature_family
-                == "Frame-by-frame body-part distances to ROI centers (mm)"
-            ):
-                self.calc_roi_center_distances()
-            elif (
-                self.feature_family == "Frame-by-frame body-parts inside ROIs (Boolean)"
-            ):
-                self.calc_inside_roi()
-            self.__save()
-            self.video_timer.stop_timer()
-            print(
-                f"Video {self.video_name} complete (elapsed time {self.video_timer.elapsed_time_str}s)..."
-            )
+                 input_path: str,
+                 config_path: str,
+                 method: Literal['Animal(s): Nearest', 'Animal(s): Linear', 'Animal(s): Quadratic','Body-parts: Nearest', 'Body-parts: Linear', 'Body-parts: Quadratic'],
+                 initial_import_multi_index: bool = False) -> None:
+
+        super().__init__(config_path=config_path, read_video_info=False)
+        self.interpolation_type, self.interpolation_method = method.split(':')[0], method.split(':')[1].replace(" ", "").lower()
+        if os.path.isdir(input_path):
+            self.files_found = glob.glob(input_path + '/*' + self.file_type)
+            self.input_dir = input_path
+            check_if_filepath_list_is_empty(filepaths=self.files_found, error_msg=f"SIMBA ERROR: {self.input_dir} does not contain any {self.file_type} files.")
+        else:
+            self.files_found = [input_path]
+            self.input_dir = os.path.dirname(input_path)
+        if not initial_import_multi_index:
+            self.save_dir = os.path.join(self.input_dir, f'Pre_{self.interpolation_method}_{self.interpolation_type}_interpolation_{self.datetime}')
+            if not os.path.exists(self.save_dir): os.makedirs(self.save_dir)
+        self.initial_import_multi_index = initial_import_multi_index
+        if self.interpolation_type == 'Animal(s)':
+            self.animal_interpolator()
+        if self.interpolation_type == 'Body-parts':
+            self.body_part_interpolator()
         self.timer.stop_timer()
-        stdout_success(
-            msg=f"{self.feature_family} for {str(len(self.outlier_corrected_paths))} video(s) saved in {self.save_dir}",
-            elapsed_time=self.timer.elapsed_time_str,
-        )
-
-    def calc_distances(self):
-        for c in self.two_point_combs:
-            col_names = list(sum([(x + "_x", y + "_y") for (x, y) in zip(c, c)], ()))
-
-            self.results[f"Distance (mm) {c[0]}-{c[1]}"] = self.euclidean_distance(
-                self.df[col_names[0]].values,
-                self.df[col_names[2]].values,
-                self.df[col_names[1]].values,
-                self.df[col_names[3]].values,
-                self.pixel_per_mm,
-            )
-
-    def calc_angles(self):
-        for animal, points in self.within_animal_three_point_combs.items():
-            for point in points:
-                col_names = list(
-                    sum([(x + "_x", y + "_y") for (x, y) in zip(point, point)], ())
-                )
-                self.results[
-                    f"Angle (degrees) {point[0]}-{point[1]}-{point[2]}"
-                ] = self.angle3pt_serialized(data=self.df[col_names].values)
-
-    def calc_three_point_hulls(self):
-        for animal, points in self.within_animal_three_point_combs.items():
-            for point in points:
-                col_names = list(
-                    sum([(x + "_x", y + "_y") for (x, y) in zip(point, point)], ())
-                )
-                three_point_arr = np.reshape(
-                    self.df[col_names].values, (len(self.df / 2), -1, 2)
-                ).astype(np.float32)
-                self.results[
-                    f"{animal} three-point convex hull perimeter (mm) {point[0]}-{point[1]}-{point[2]}"
-                ] = (
-                    jitted_hull(points=three_point_arr, target=Formats.PERIMETER.value)
-                    / self.pixel_per_mm
-                )
-
-    def calc_four_point_hulls(self):
-        for animal, points in self.within_animal_four_point_combs.items():
-            for point in points:
-                col_names = list(
-                    sum([(x + "_x", y + "_y") for (x, y) in zip(point, point)], ())
-                )
-                four_point_arr = np.reshape(
-                    self.df[col_names].values, (len(self.df / 2), -1, 2)
-                ).astype(np.float32)
-                self.results[
-                    f"{animal} four-point convex perimeter (mm) {point[0]}-{point[1]}-{point[2]}-{point[3]}"
-                ] = (
-                    jitted_hull(points=four_point_arr, target=Formats.PERIMETER.value)
-                    / self.pixel_per_mm
-                )
-
-    def animal_convex_hulls(self):
-        for animal, point in self.animal_bps.items():
-            col_names = list(
-                sum([(x + "_x", y + "_y") for (x, y) in zip(point, point)], ())
-            )
-            animal_point_arr = np.reshape(
-                self.df[col_names].values, (len(self.df / 2), -1, 2)
-            ).astype(np.float32)
-            self.results[f"{animal} convex hull perimeter (mm)"] = (
-                jitted_hull(points=animal_point_arr, target=Formats.PERIMETER.value)
-                / self.pixel_per_mm
-            )
-
-    def calc_movements(self):
-        for animal, animal_bps in self.animal_bps.items():
-            for bp in animal_bps:
-                bp_df = self.df[[f"{bp}_x", f"{bp}_y"]]
-                shift = bp_df.shift(periods=1).add_suffix("_shift")
-                bp_df = pd.concat([bp_df, shift], axis=1, join="inner").reset_index(
-                    drop=True
-                )
-                for c in shift.columns:
-                    bp_df[c] = bp_df[c].fillna(bp_df[c[:-6]])
-                self.results[f"{animal} movement {bp} (mm)"] = self.euclidean_distance(
-                    bp_df[f"{bp}_x_shift"].values,
-                    bp_df[f"{bp}_x"].values,
-                    bp_df[f"{bp}_y_shift"].values,
-                    bp_df[f"{bp}_y"].values,
-                    self.pixel_per_mm,
-                )
-
-    def calc_animal_convex_hulls_area(self):
-        for animal, point in self.animal_bps.items():
-            col_names = list(
-                sum([(x + "_x", y + "_y") for (x, y) in zip(point, point)], ())
-            )
-            animal_point_arr = np.reshape(
-                self.df[col_names].values, (len(self.df / 2), -1, 2)
-            ).astype(np.float32)
-            self.results[f"{animal} convex hull area (mm2)"] = (
-                jitted_hull(points=animal_point_arr, target=Formats.AREA.value)
-                / self.pixel_per_mm
-            )
-
-    def calc_roi_center_distances(self):
-        self.read_roi_data()
-        for animal, animal_bps in self.animal_bps.items():
-            for bp in animal_bps:
-                bp_arr = self.df[[f"{bp}_x", f"{bp}_y"]].values.astype(float)
-                for shape_type, shape_data in self.roi_dict.items():
-                    for shape_name in shape_data["Name"].unique():
-                        center_point = (
-                            shape_data.loc[
-                                (shape_data["Video"] == self.video_name)
-                                & (shape_data["Name"] == shape_name)
-                            ][["Center_X", "Center_Y"]]
-                            .astype(float)
-                            .values[0]
-                        )
-                        self.results[
-                            f"{animal} {bp} to {shape_name} center distance (mm)"
-                        ] = self.framewise_euclidean_distance_roi(
-                            location_1=bp_arr,
-                            location_2=center_point,
-                            px_per_mm=self.pixel_per_mm,
-                        )
-
-    def calc_inside_roi(self):
-        self.read_roi_data()
-        for animal, animal_bps in self.animal_bps.items():
-            for bp in animal_bps:
-                bp_arr = self.df[[f"{bp}_x", f"{bp}_y"]].values.astype(float)
-                for shape_type, shape_data in self.roi_dict.items():
-                    for shape_name in shape_data["Name"].unique():
-                        if shape_type == "rectangles":
-                            shape_data = shape_data.loc[
-                                (shape_data["Video"] == self.video_name)
-                                & (shape_data["Name"] == shape_name)
-                            ][
-                                [
-                                    "topLeftX",
-                                    "topLeftY",
-                                    "Bottom_right_X",
-                                    "Bottom_right_Y",
-                                ]
-                            ].values.reshape(
-                                2, 2
-                            )
-                            self.results[
-                                f"{animal} {bp} inside rectangle {shape_name} (Boolean)"
-                            ] = self.framewise_inside_rectangle_roi(
-                                bp_location=bp_arr, roi_coords=shape_data
-                            )
-                        if shape_type == "polygons":
-                            shape_data = shape_data.loc[
-                                (shape_data["Video"] == self.video_name)
-                                & (shape_data["Name"] == shape_name)
-                            ][["vertices"]].values[0][0]
-                            self.results[
-                                f"{animal} {bp} inside polygon {shape_name} (Boolean)"
-                            ] = self.framewise_inside_polygon_roi(
-                                bp_location=bp_arr, roi_coords=shape_data
-                            )
-
-    def __save(self):
-        if self.append_to_features:
-            prior_appending_features_data_folder = os.path.join(self.features_dir, f'Prior_to_third_subset_features_{self.datetime}')
-            if not os.path.isdir(prior_appending_features_data_folder):
-                os.makedirs(prior_appending_features_data_folder)
-            file_path = os.path.join(self.features_dir, f"{self.video_name}.csv")
-            check_file_exist_and_readable(file_path=file_path)
-            features_df = read_df(file_path=file_path, file_type=self.file_type)
-            if len(features_df) != len(self.results):
-                raise CountError(f'Cannot append feature subsets to features file. The file used to create the feature subsets ({self.current_file_path}) contains data for {len(self.results)} frames, while the file representing the same video in features extracted folder ({file_path}) contains data for {len(features_df)} frames. Make sure the two files has an equal number of rows.')
-            new_features_df = pd.concat([features_df, self.results.round(2).set_index(features_df.index)], axis=1)
-            duplicate_cols = new_features_df.columns[new_features_df.columns.duplicated()]
-            if len(duplicate_cols) > 0:
-                raise DataHeaderError(msg=f'Attempted to append feature data to file {file_path}. However the new features (e.g., {duplicate_cols[0]}) already exist in the targets inserted file.')
-            write_df(df=features_df, file_type=self.file_type, save_path=os.path.join(prior_appending_features_data_folder, os.path.basename(file_path)))
-            write_df(df=new_features_df, file_type=self.file_type, save_path=file_path)
-            del new_features_df
-            print(f'New features for video {self.video_name} saved in project_folder/csv/features_extracted directory...')
-
-        if self.append_to_targets:
-            prior_appending_features_data_folder = os.path.join(self.targets_folder,f'Prior_to_third_subset_features_{self.datetime}')
-            if not os.path.isdir(prior_appending_features_data_folder):
-                os.makedirs(prior_appending_features_data_folder)
-            file_path = os.path.join(self.targets_folder, f"{self.video_name}.csv")
-            check_file_exist_and_readable(file_path=file_path)
-            targets_df = read_df(file_path=file_path, file_type=self.file_type)
-            targets_clf_df = pd.DataFrame()
-            if len(targets_df) != len(self.results):
-                raise CountError(f'Cannot append feature subsets to targets file. The file used to create the feature subsets ({self.current_file_path}) contains data for {len(self.results)} frames, while the file representing the same video in features extracted folder ({file_path}) contains data for {len(targets_df)} frames. Make sure the two files has an equal number of rows.')
-            for clf in self.clf_names:
-                if clf in targets_df.columns:
-                    targets_clf_df[clf] = targets_df[clf]
-                    targets_df.drop(clf, axis=1, inplace=True)
-
-            new_targets_df = pd.concat([targets_df, self.results.round(2).set_index(targets_df.index), targets_clf_df], axis=1)
-            duplicate_cols = new_targets_df.columns[new_targets_df.columns.duplicated()]
-            if len(duplicate_cols) > 0:
-                raise DataHeaderError(msg=f'Attempted to append feature data to file {file_path}. However the new features (e.g., {duplicate_cols[0]}) already exist in the file.')
-
-
-            write_df(df=targets_df, file_type=self.file_type, save_path=os.path.join(prior_appending_features_data_folder, os.path.basename(file_path)))
-            write_df(df=new_targets_df, file_type=self.file_type, save_path=file_path)
-            del new_targets_df; del targets_df
-            print(f'New targets file for video {self.video_name} saved in project_folder/csv/targets_inserted directory...')
-
-        save_path = os.path.join(self.save_dir, f"{self.video_name}.csv")
-        write_df(df=self.results.round(2), file_type=Formats.CSV.value, save_path=save_path)
-
-
-# test = FeatureSubsetsCalculator(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
-#                                 feature_family='Frame-by-frame body-parts inside ROIs (Boolean)',
-#                                 save_dir='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/data')
-# test.run()
-
-
-# test = FeatureSubsetsCalculator(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
-#                                 feature_family='Frame-by-frame body-part movements (mm)',
-#                                 save_dir='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/data')
-# test.run()
+        stdout_success(msg=f'{str(len(self.files_found))} data file(s) interpolated)', elapsed_time=self.timer.elapsed_time_str)
+
+    def animal_interpolator(self):
+        for file_path in self.files_found:
+            video_timer = SimbaTimer()
+            video_timer.start_timer()
+            _, video_name, _ = get_fn_ext(filepath=file_path)
+            df = read_df(file_path=file_path, file_type=self.file_type, check_multiindex=self.initial_import_multi_index)
+            df[df < 0] = 0
+            if self.initial_import_multi_index:
+                df.columns = self.bp_headers
+            for animal_name, animal_bps in self.animal_bp_dict.items():
+                animal_df = df[animal_bps['X_bps'] + animal_bps['Y_bps']].fillna(0).astype(int)
+                idx = list(animal_df[animal_df.eq(animal_df.iloc[:, 0], axis=0).all(axis='columns')].index)
+                print(f'Interpolating {len(idx)} body-parts for animal {animal_name} in video {video_name}...')
+                animal_df.loc[idx, :] = np.nan
+                animal_df = animal_df.interpolate(method=self.interpolation_method, axis=0).ffill().bfill()
+                animal_df[animal_df < 0] = 0
+                df.update(animal_df)
+            if not self.initial_import_multi_index:
+                shutil.move(src=file_path, dst=os.path.join(self.save_dir, os.path.basename(file_path)))
+            else:
+                multi_idx_header = []
+                for i in range(len(df.columns)): multi_idx_header.append(('IMPORTED_POSE', 'IMPORTED_POSE', list(df.columns)[i]))
+                df.columns = pd.MultiIndex.from_tuples(multi_idx_header)
+            write_df(df=df, file_type=self.file_type, save_path=file_path, multi_idx_header=self.initial_import_multi_index)
+            video_timer.stop_timer()
+            print(f'Video {video_name} interpolated (elapsed time {video_timer.elapsed_time_str})...')
+
+    def body_part_interpolator(self):
+        for file_path in self.files_found:
+            video_timer = SimbaTimer(start=True)
+            _, video_name, _ = get_fn_ext(filepath=file_path)
+            df = read_df(file_path=file_path, file_type=self.file_type, check_multiindex=True)
+            if self.initial_import_multi_index:
+                df.columns = self.bp_headers
+            df[df < 0] = 0
+            for animal in self.animal_bp_dict:
+                for x_bps_name, y_bps_name in zip(self.animal_bp_dict[animal]['X_bps'], self.animal_bp_dict[animal]['Y_bps']):
+                    df[x_bps_name] = df[x_bps_name].astype(int)
+                    df[y_bps_name] = df[y_bps_name].astype(int)
+                    idx = df.loc[(df[x_bps_name] <= 0.0) & (df[y_bps_name] <= 0.0)].index.tolist()
+                    print(f'Interpolating {len(idx)} {x_bps_name[:-2]} body-parts for animal {animal} in video {video_name}...')
+                    df.loc[idx, [x_bps_name, y_bps_name]] = np.nan
+                    df[x_bps_name] = df[x_bps_name].interpolate(method=self.interpolation_method, axis=0).ffill().bfill()
+                    df[x_bps_name][df[x_bps_name] < 0] = 0
+                    df[y_bps_name] = df[y_bps_name].interpolate(method=self.interpolation_method, axis=0).ffill().bfill()
+                    df[y_bps_name][df[y_bps_name] < 0] = 0
+            if not self.initial_import_multi_index:
+                shutil.move(src=file_path, dst=os.path.join(self.save_dir, os.path.basename(file_path)))
+            else:
+                multi_idx_header = []
+                for i in range(len(df.columns)): multi_idx_header.append(('IMPORTED_POSE', 'IMPORTED_POSE', list(df.columns)[i]))
+                df.columns = pd.MultiIndex.from_tuples(multi_idx_header)
+            write_df(df=df, file_type=self.file_type, save_path=file_path, multi_idx_header=self.initial_import_multi_index)
+            video_timer.stop_timer()
+            print(f'Video {video_name} interpolated (elapsed time {video_timer.elapsed_time_str}) ...')
+
+class Smooth(ConfigReader):
+    """
+    Smooth pose-estimation data according to user-defined method.
+
+    :parameter str input_path: path to pose-estimation data in CSV or parquet format
+    :parameter str config_path: path to SimBA project config file in Configparser format.
+    :parameter Literal str: Type of smoothing_method. OPTIONS: ``Gaussian``, ``Savitzky-Golay``.
+    :parameter int time_window: Rolling time window in millisecond to use when smoothing. Larger time-windows and greater smoothing.
+    :parameter bool initial_import_multi_index: If True, the incoming data is multi-index columns dataframes. Default: False.
+
+    .. note::
+        `Smoothing tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario1.md#to-import-multiple-dlc-csv-files>`__.
 
+    Examples
+    -----
+    >>> _ = Smooth(input_path=data_path, config_path=SimBaProjectConfigPath, smoothing_method='Savitzky-Golay', time_window=300)
+    """
+
+    def __init__(self,
+                 config_path: str,
+                 input_path: str,
+                 time_window: int,
+                 smoothing_method: Literal['Gaussian', 'Savitzky-Golay'],
+                 initial_import_multi_index: bool = False):
+
+        super().__init__(config_path=config_path, read_video_info=False)
+        if os.path.isdir(input_path):
+            self.files_found = glob.glob(input_path + '/*' + self.file_type)
+            self.input_dir = input_path
+            check_if_filepath_list_is_empty(filepaths=self.files_found, error_msg=f"SIMBA ERROR: {self.input_dir} does not contain any {self.file_type} files.")
+        else:
+            self.files_found = [input_path]
+            self.input_dir = os.path.dirname(input_path)
+        if not initial_import_multi_index:
+            self.save_dir = os.path.join(self.input_dir, f'Pre_{smoothing_method}_interpolation_{self.datetime}')
+            if not os.path.exists(self.save_dir): os.makedirs(self.save_dir)
+        self.time_window, self.initial_import_multi_index = int(time_window), initial_import_multi_index
+        if smoothing_method == Methods.SAVITZKY_GOLAY.value:
+            self.savgol_smoother()
+        elif smoothing_method == Methods.GAUSSIAN.value:
+            self.gaussian_smoother()
+        self.timer.stop_timer()
+        stdout_success(msg=f'{str(len(self.files_found))} data file(s) smoothened', elapsed_time=self.timer.elapsed_time_str)
+
+    def savgol_smoother(self):
+        for file_path in self.files_found:
+            video_timer = SimbaTimer(start=True)
+            _, video_name, _ = get_fn_ext(filepath=file_path)
+            df = read_df(file_path=file_path, file_type=self.file_type, check_multiindex=self.initial_import_multi_index)
+            video_path = find_video_of_file(video_dir=self.video_dir, filename=video_name)
+            if not video_path:
+                try:
+                    video_meta_data = {}
+                    self.video_info_df = self.read_video_info_csv(file_path=self.video_info_path)
+                    _, _, fps = self.read_video_info(video_name=video_name)
+                    video_meta_data['fps'] = fps
+                except:
+                    raise NoFilesFoundError(msg=f'No video for file {video_name} found in SimBA project. Import the video before doing smoothing. To perform smoothing, SimBA needs the video fps from the video itself or the logs/video_info.csv file in order to read the video FPS.')
+            else:
+                video_meta_data = get_video_meta_data(video_path=video_path)
+            frames_in_time_window = int(self.time_window / (1000 / int(video_meta_data['fps'])))
+            if (frames_in_time_window % 2) == 0:
+                frames_in_time_window = frames_in_time_window - 1
+            if (frames_in_time_window % 2) <= 3:
+                frames_in_time_window = 5
+            df[df < 0] = 0
+            for c in df.columns:
+                df[c] = savgol_filter(x=df[c].to_numpy(), window_length=frames_in_time_window, polyorder=3, mode='nearest')
+                df[c][df[c] < 0] = 0
+            if not self.initial_import_multi_index:
+                shutil.move(src=file_path, dst=os.path.join(self.save_dir, os.path.basename(file_path)))
+            else:
+                multi_idx_header = []
+                for i in range(len(df.columns)): multi_idx_header.append(('IMPORTED_POSE', 'IMPORTED_POSE', list(df.columns)[i]))
+                df.columns = pd.MultiIndex.from_tuples(multi_idx_header)
+            write_df(df=df, file_type=self.file_type, save_path=file_path, multi_idx_header=self.initial_import_multi_index)
+            video_timer.stop_timer()
+            print(f'Video {video_name} smoothed (Savitzky Golay: {str(self.time_window)}ms) (elapsed time {video_timer.elapsed_time_str})...')
+
+    def gaussian_smoother(self):
+        for file_path in self.files_found:
+            video_timer = SimbaTimer(start=True)
+            _, video_name, _ = get_fn_ext(filepath=file_path)
+            df = read_df(file_path=file_path, file_type=self.file_type, check_multiindex=self.initial_import_multi_index)
+            video_path = find_video_of_file(video_dir=self.video_dir, filename=video_name)
+            if not video_path:
+                raise NoFilesFoundError(msg=f'No video for file {video_name} found in SimBA project. Import the video before doing Gaussian smoothing. To perform smoothing, SimBA needs the video in order to read the video FPS.')
+            video_meta_data = get_video_meta_data(video_path=video_path)
+            frames_in_time_window = int(self.time_window / (1000 / video_meta_data['fps']))
+            for c in df.columns:
+                df[c] = df[c].rolling(window=int(frames_in_time_window), win_type='gaussian', center=True).mean(std=5).fillna(df[c]).abs()
+                df[c][df[c] < 0] = 0
+            if not self.initial_import_multi_index:
+                shutil.move(src=file_path, dst=os.path.join(self.save_dir, os.path.basename(file_path)))
+            else:
+                multi_idx_header = []
+                for i in range(len(df.columns)): multi_idx_header.append(('IMPORTED_POSE', 'IMPORTED_POSE', list(df.columns)[i]))
+                df.columns = pd.MultiIndex.from_tuples(multi_idx_header)
+            write_df(df=df, file_type=self.file_type, save_path=file_path, multi_idx_header=self.initial_import_multi_index)
+            video_timer.stop_timer()
+            print(f'Video {video_name} smoothed (Gaussian: {str(self.time_window)}ms) (elapsed time {video_timer.elapsed_time_str})...')
+
+
+# Interpolate(input_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/csv/outlier_corrected_movement_location',
+#             config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
+#             method='Body-parts: Nearest',
+#             initial_import_multi_index=False)
+
+# Interpolate(input_path='/Users/simon/Desktop/envs/troubleshooting/dorian_2/project_folder/csv/input_csv',
+#             config_path='/Users/simon/Desktop/envs/troubleshooting/dorian_2/project_folder/project_config.ini',
+#             method='Body-parts: Linear',
+#             initial_import_multi_index=True)
 #
-# test = FeatureSubsetsCalculator(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
-#                                 feature_family='Frame-by-frame body-parts inside ROIs (Boolean)',
-#                                 save_dir='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/data',
-#                                 append_to_features_extracted=False,
-#                                 append_to_targets_inserted=True)
-# test.run()
+
+
+# Interpolate(input_path='/Users/simon/Desktop/envs/troubleshooting/sleap_5_animals/project_folder/csv/outlier_corrected_movement_location',
+#             config_path='/Users/simon/Desktop/envs/troubleshooting/sleap_5_animals/project_folder/project_config.ini',
+#             method='Body-parts: Nearest',
+#             initial_import_multi_index=False)
+
+# PostHocInterpolate(config_path='/Users/simon/Desktop/envs/troubleshooting/ddddfff/project_folder/project_config.ini',
+#                    input_dir='/Users/simon/Desktop/envs/troubleshooting/ddddfff/project_folder/csv/outlier_corrected_movement_location',
+#                    method='Animal(s): Nearest')
+
+
+# Smooth(config_path='/Users/simon/Desktop/envs/troubleshooting/DLC_2_Black_animals/project_folder/project_config.ini',
+#               input_path='/Users/simon/Desktop/envs/troubleshooting/DLC_2_Black_animals/project_folder/csv/input_csv',
+#               time_window=100,
+#               smoothing_method=Methods.SAVITZKY_GOLAY.value,
+#               initial_import_multi_index=True)
+
+# Smooth(config_path='/Users/simon/Desktop/envs/troubleshooting/dorian_2/project_folder/project_config.ini',
+#               input_path='/Users/simon/Desktop/envs/troubleshooting/dorian_2/project_folder/csv/input_csv',
+#               time_window=400,
+#               smoothing_method=Methods.SAVITZKY_GOLAY.value,
+#               initial_import_multi_index=True)
+
+
+# class PostHocSmooth(ConfigReader):
+#     def __init__(self,
+#                  config_path: str,
+#                  input_dir: str,
+#                  time_window: int,
+#                  smoothing_method: str):
```

### Comparing `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.64.8/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.64.8/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/feature_extractor_9bp.py` & `Simba-UW-tf-dev-1.64.8/simba/feature_extractors/feature_extractor_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.64.8/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.64.8/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/.idea/features_scripts.iml` & `Simba-UW-tf-dev-1.64.8/simba/feature_extractors/.idea/features_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.64.8/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/.idea/workspace.xml` & `Simba-UW-tf-dev-1.64.8/simba/feature_extractors/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/requirements.txt` & `Simba-UW-tf-dev-1.64.8/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.64.8/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.64.8/simba/mixins/pop_up_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.64.8/simba/mixins/config_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,14 +278,20 @@
         return shape_df
 
     def remove_a_folder(self,
                         folder_dir: str) -> None:
         """Helper to remove a directory"""
         shutil.rmtree(folder_dir, ignore_errors=True)
 
+    def remove_multiple_folders(self,
+                                folders: List[str]) -> None:
+        """Helper to remove multiple directories"""
+        for folder_path in folders:
+            shutil.rmtree(folder_path, ignore_errors=True)
+
     def find_animal_name_from_body_part_name(self,
                                              bp_name: str,
                                              bp_dict: dict) -> str:
 
         """
         Given body-part name and animal body-part dict, returns the animal name
```

### Comparing `Simba-UW-tf-dev-1.64.7/simba/mixins/pose_importer_mixin.py` & `Simba-UW-tf-dev-1.64.8/simba/mixins/pose_importer_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/mixins/video_processing_mixin.py` & `Simba-UW-tf-dev-1.64.8/simba/mixins/video_processing_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi` & `Simba-UW-tf-dev-1.64.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi` & `Simba-UW-tf-dev-1.64.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi` & `Simba-UW-tf-dev-1.64.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc` & `Simba-UW-tf-dev-1.64.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc` & `Simba-UW-tf-dev-1.64.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc` & `Simba-UW-tf-dev-1.64.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc` & `Simba-UW-tf-dev-1.64.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.64.8/simba/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.64.8/simba/mixins/plotting_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.64.8/simba/mixins/unsupervised_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/mixins/train_model_mixin.py` & `Simba-UW-tf-dev-1.64.8/simba/mixins/train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.64.8/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.64.8/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.64.8/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/third_party_label_appenders/.DS_Store` & `Simba-UW-tf-dev-1.64.8/simba/third_party_label_appenders/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.64.8/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.64.8/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.64.8/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.64.8/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.64.8/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/cue_light_tools/.DS_Store` & `Simba-UW-tf-dev-1.64.8/simba/cue_light_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.64.8/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.64.8/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.64.8/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.64.8/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.64.8/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.64.8/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/utils/config_creator.py` & `Simba-UW-tf-dev-1.64.8/simba/utils/config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/utils/enums.py` & `Simba-UW-tf-dev-1.64.8/simba/utils/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.64.8/simba/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.64.8/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/utils/checks.py` & `Simba-UW-tf-dev-1.64.8/simba/utils/checks.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 from simba.utils.errors import (NoFilesFoundError,
                                 CorruptedFileError,
                                 IntegerError,
                                 FloatError,
                                 StringError,
                                 NotDirectoryError,
                                 ColumnNotFoundError,
-                                InvalidInputError)
+                                InvalidInputError,
+                                CountError)
 
 
 def check_file_exist_and_readable(file_path: Union[str, os.PathLike]) -> None:
     """
     Checks if a path points to a readable file.
 
     :param str file_path:
@@ -250,14 +251,46 @@
             roll_windows_values[win] = minimum_fps
         else:
             pass
     roll_windows_values = list(set(roll_windows_values))
     return roll_windows_values
 
 
+def check_same_number_of_rows_in_dfs(dfs: List[pd.DataFrame]) -> bool:
+    """
+    Helper to check if dataframes contains an equal number of rows
+
+    :param List[pd.DataFrame] dfs: List of dataframes.
+    :return bool: True if dataframes has an equal number of rows. Else False.
+    """
+    row_cnt = None
+    for df_cnt, df in enumerate(dfs):
+        if df_cnt == 0:
+            row_cnt = len(df)
+        else:
+            if len(df) != row_cnt:
+                return False
+    return True
+
+
+
+def check_if_headers_in_dfs_are_unique(dfs: List[pd.DataFrame]) -> List[str]:
+    """
+    Helper to check heaaders in multiple dataframes are unique.
+
+    :param List[pd.DataFrame] dfs: List of dataframes.
+    :return List[str]: List of columns headers seen in multiple dataframes. Empty if None.
+    """
+    seen_headers = []
+    for df_cnt, df in enumerate(dfs):
+        seen_headers.extend(list(df.columns))
+    duplicates = list(set([x for x in seen_headers if seen_headers.count(x) > 1]))
+    return duplicates
+
+
 def check_nvidea_gpu_available() -> bool:
     """ Helper to check of NVIDEA GPU is available"""
     try:
         subprocess.check_output('nvidia-smi')
         return True
     except Exception:
         return False
@@ -265,8 +298,8 @@
 
 def check_ffmpeg_available() -> bool:
     """ Helper to check of FFMpeg is available"""
     try:
         subprocess.call('ffmpeg', stderr=subprocess.DEVNULL, stdout=subprocess.DEVNULL)
         return True
     except Exception:
-        return False
+        return False
```

### Comparing `Simba-UW-tf-dev-1.64.7/simba/utils/read_write.py` & `Simba-UW-tf-dev-1.64.8/simba/utils/read_write.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.64.8/simba/utils/lookups.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/utils/cli/cli_tools.py` & `Simba-UW-tf-dev-1.64.8/simba/utils/cli/cli_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/utils/errors.py` & `Simba-UW-tf-dev-1.64.8/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/utils/data.py` & `Simba-UW-tf-dev-1.64.8/simba/utils/data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/utils/printing.py` & `Simba-UW-tf-dev-1.64.8/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/st/select_groups_pg.py` & `Simba-UW-tf-dev-1.64.8/simba/st/select_groups_pg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/st/aggregate_statistics.py` & `Simba-UW-tf-dev-1.64.8/simba/st/aggregate_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/st/app.py` & `Simba-UW-tf-dev-1.64.8/simba/st/app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_processors/reorganize_keypoint.py` & `Simba-UW-tf-dev-1.64.8/simba/pose_processors/reorganize_keypoint.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_processors/remove_keypoints.py` & `Simba-UW-tf-dev-1.64.8/simba/pose_processors/remove_keypoints.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_processors/.DS_Store` & `Simba-UW-tf-dev-1.64.8/simba/pose_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_processors/pose_reset.py` & `Simba-UW-tf-dev-1.64.8/simba/pose_processors/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_processors/reverse_pose.py` & `Simba-UW-tf-dev-1.64.8/simba/pose_processors/reverse_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.64.8/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.64.8/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.64.8/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/plotting/.DS_Store` & `Simba-UW-tf-dev-1.64.8/simba/plotting/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.64.8/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.64.8/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.64.8/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.64.8/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.64.8/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.64.8/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.64.8/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.64.8/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.64.8/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.64.8/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.64.8/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.64.8/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/plotting/pose_plotter_mp.py` & `Simba-UW-tf-dev-1.64.8/simba/plotting/pose_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/plotting/Directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.64.8/simba/plotting/Directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.64.8/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.64.8/simba/plotting/path_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.64.8/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.64.8/simba/plotting/data_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.64.8/simba/plotting/path_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.64.8/simba/plotting/ez_lineplot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.64.8/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.64.8/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.64.8/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.64.8/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.64.8/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/plotting/Directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.64.8/simba/plotting/Directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.64.8/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/dash_app/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.64.8/simba/dash_app/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/dash_app/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.64.8/simba/dash_app/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/dash_app/dash_app.py` & `Simba-UW-tf-dev-1.64.8/simba/dash_app/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/data_processors/agg_clf_calculator.py` & `Simba-UW-tf-dev-1.64.8/simba/data_processors/agg_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/data_processors/.DS_Store` & `Simba-UW-tf-dev-1.64.8/simba/data_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/data_processors/severity_bout_based_calculator.py` & `Simba-UW-tf-dev-1.64.8/simba/data_processors/severity_bout_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/data_processors/timebins_clf_calculator.py` & `Simba-UW-tf-dev-1.64.8/simba/data_processors/timebins_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/data_processors/fsttc_calculator.py` & `Simba-UW-tf-dev-1.64.8/simba/data_processors/fsttc_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/data_processors/interpolate_pose.py` & `Simba-UW-tf-dev-1.64.8/simba/data_processors/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/data_processors/directing_other_animals_calculator.py` & `Simba-UW-tf-dev-1.64.8/simba/data_processors/directing_other_animals_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/data_processors/timebins_movement_calculator.py` & `Simba-UW-tf-dev-1.64.8/simba/data_processors/timebins_movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/data_processors/severity_calculator.py` & `Simba-UW-tf-dev-1.64.8/simba/data_processors/severity_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/data_processors/pup_retrieval_calculator.py` & `Simba-UW-tf-dev-1.64.8/simba/data_processors/pup_retrieval_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/data_processors/pybursts_calculator.py` & `Simba-UW-tf-dev-1.64.8/simba/data_processors/pybursts_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/data_processors/severity_frame_based_calculator.py` & `Simba-UW-tf-dev-1.64.8/simba/data_processors/severity_frame_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/data_processors/mutual_exclusivity_corrector.py` & `Simba-UW-tf-dev-1.64.8/simba/data_processors/mutual_exclusivity_corrector.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/data_processors/kleinberg_calculator.py` & `Simba-UW-tf-dev-1.64.8/simba/data_processors/kleinberg_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/data_processors/movement_calculator.py` & `Simba-UW-tf-dev-1.64.8/simba/data_processors/movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store` & `Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store` & `Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png` & `Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png` & `Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png` & `Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png` & `Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png` & `Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png` & `Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png` & `Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png` & `Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png` & `Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png` & `Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png` & `Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png` & `Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png` & `Simba-UW-tf-dev-1.64.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/model/train_rf.py` & `Simba-UW-tf-dev-1.64.8/simba/model/train_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/model/.DS_Store` & `Simba-UW-tf-dev-1.64.8/simba/model/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/model/inference_batch.py` & `Simba-UW-tf-dev-1.64.8/simba/model/inference_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/model/grid_search_rf.py` & `Simba-UW-tf-dev-1.64.8/simba/model/grid_search_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/model/inference_validation.py` & `Simba-UW-tf-dev-1.64.8/simba/model/inference_validation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.64.8/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.64.8/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.64.8/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.64.8/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.64.8/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.64.8/simba/roi_tools/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.64.8/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.64.8/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.64.8/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.64.8/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.64.8/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.64.8/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.64.8/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.64.8/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.64.8/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_importers/sleap_csv_importer.py` & `Simba-UW-tf-dev-1.64.8/simba/pose_importers/sleap_csv_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_importers/misc/.DS_Store` & `Simba-UW-tf-dev-1.64.8/simba/pose_importers/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_importers/misc/apt_trk_importer.py` & `Simba-UW-tf-dev-1.64.8/simba/pose_importers/misc/apt_trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.64.8/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_importers/.DS_Store` & `Simba-UW-tf-dev-1.64.8/simba/pose_importers/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_importers/sleap_h5_importer.py` & `Simba-UW-tf-dev-1.64.8/simba/pose_importers/sleap_h5_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_importers/madlc_importer.py` & `Simba-UW-tf-dev-1.64.8/simba/pose_importers/madlc_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_importers/sleap_slp_importer.py` & `Simba-UW-tf-dev-1.64.8/simba/pose_importers/sleap_slp_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.64.8/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.64.8/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.64.8/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.64.8/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_configurations/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.64.8/simba/pose_configurations/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.64.8/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_configurations/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.64.8/simba/pose_configurations/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_configurations/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.64.8/simba/pose_configurations/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.64.8/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.64.8/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.64.8/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.64.8/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.64.8/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.64.8/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.64.8/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.64.8/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.64.8/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.64.8/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.64.8/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.64.8/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/three_dimensions/ui/define_px_to_mm_ui.py` & `Simba-UW-tf-dev-1.64.8/simba/three_dimensions/ui/define_px_to_mm_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/three_dimensions/feature_extractors/generic_feature_extractor.py` & `Simba-UW-tf-dev-1.64.8/simba/three_dimensions/feature_extractors/generic_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/three_dimensions/mixins/config_reader.py` & `Simba-UW-tf-dev-1.64.8/simba/three_dimensions/mixins/config_reader.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.1.nbc` & `Simba-UW-tf-dev-1.64.8/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.1.nbc` & `Simba-UW-tf-dev-1.64.8/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.nbi` & `Simba-UW-tf-dev-1.64.8/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.nbi` & `Simba-UW-tf-dev-1.64.8/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/three_dimensions/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.64.8/simba/three_dimensions/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/three_dimensions/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.64.8/simba/three_dimensions/mixins/plotting_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/three_dimensions/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.64.8/simba/three_dimensions/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/three_dimensions/pose_importers/anipose_csv_import.py` & `Simba-UW-tf-dev-1.64.8/simba/three_dimensions/pose_importers/anipose_csv_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/three_dimensions/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.64.8/simba/three_dimensions/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/video_processors/video_processing.py` & `Simba-UW-tf-dev-1.64.8/simba/video_processors/video_processing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/video_processors/.DS_Store` & `Simba-UW-tf-dev-1.64.8/simba/video_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/video_processors/px_to_mm.py` & `Simba-UW-tf-dev-1.64.8/simba/video_processors/px_to_mm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/video_processors/batch_process_menus.py` & `Simba-UW-tf-dev-1.64.8/simba/video_processors/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/video_processors/video_processing_new.py` & `Simba-UW-tf-dev-1.64.8/simba/video_processors/video_processing_new.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/video_processors/multi_cropper.py` & `Simba-UW-tf-dev-1.64.8/simba/video_processors/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/video_processors/extract_frames.py` & `Simba-UW-tf-dev-1.64.8/simba/video_processors/extract_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/video_processors/calculate_px_dist.py` & `Simba-UW-tf-dev-1.64.8/simba/video_processors/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/video_processors/extract_seqframes.py` & `Simba-UW-tf-dev-1.64.8/simba/video_processors/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/video_processors/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.64.8/simba/video_processors/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.64.8/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/outlier_tools/.DS_Store` & `Simba-UW-tf-dev-1.64.8/simba/outlier_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.64.8/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.64.8/simba/outlier_tools/skip_outlier_correction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/outlier_tools/.idea/outlier_scripts.iml` & `Simba-UW-tf-dev-1.64.8/simba/outlier_tools/.idea/outlier_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.64.8/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/outlier_tools/.idea/workspace.xml` & `Simba-UW-tf-dev-1.64.8/simba/outlier_tools/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/SimBA.py` & `Simba-UW-tf-dev-1.64.8/simba/SimBA.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.64.8/simba/assets/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.64.8/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.64.8/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.64.8/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.64.8/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.64.8/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/shap/.DS_Store` & `Simba-UW-tf-dev-1.64.8/simba/assets/shap/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.64.8/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.64.8/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.64.8/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.64.8/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.64.8/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.64.8/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.64.8/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.64.8/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.64.8/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.64.8/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.64.8/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.64.8/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.64.8/simba/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/lookups/.DS_Store` & `Simba-UW-tf-dev-1.64.8/simba/assets/lookups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.64.8/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.64.8/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.64.8/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.64.8/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.64.8/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.64.8/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.64.8/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.64.8/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/img/.DS_Store` & `Simba-UW-tf-dev-1.64.8/simba/assets/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.64.8/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.64.8/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.64.8/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/stopwatch.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/stopwatch.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.64.8/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.64.8/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.64.8/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.64.8/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.64.7
+Version: 1.64.8
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.64.7/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.64.8/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.64.8/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/LICENSE.md` & `Simba-UW-tf-dev-1.64.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/tests/test_data_processors.py` & `Simba-UW-tf-dev-1.64.8/tests/test_data_processors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/tests/test_distance_plotter.py` & `Simba-UW-tf-dev-1.64.8/tests/test_distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/tests/test_train_model_mixin.py` & `Simba-UW-tf-dev-1.64.8/tests/test_train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/tests/test_pose_importers.py` & `Simba-UW-tf-dev-1.64.8/tests/test_pose_importers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/tests/test_feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.64.8/tests/test_feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/tests/test_utils_data.py` & `Simba-UW-tf-dev-1.64.8/tests/test_utils_data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/tests/test_config_reader_mixin.py` & `Simba-UW-tf-dev-1.64.8/tests/test_config_reader_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/tests/test_outlier_correctors.py` & `Simba-UW-tf-dev-1.64.8/tests/test_outlier_correctors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/tests/test_visualize_directing_animals.py` & `Simba-UW-tf-dev-1.64.8/tests/test_visualize_directing_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/tests/test_featurizers.py` & `Simba-UW-tf-dev-1.64.8/tests/test_featurizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/tests/test_video_processors.py` & `Simba-UW-tf-dev-1.64.8/tests/test_video_processors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py` & `Simba-UW-tf-dev-1.64.8/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/tests/test_thirdparty_appenders.py` & `Simba-UW-tf-dev-1.64.8/tests/test_thirdparty_appenders.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/tests/test_validation_clips.py` & `Simba-UW-tf-dev-1.64.8/tests/test_validation_clips.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/tests/test_roi_tools.py` & `Simba-UW-tf-dev-1.64.8/tests/test_roi_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/README.md` & `Simba-UW-tf-dev-1.64.8/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.7/setup.py` & `Simba-UW-tf-dev-1.64.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under GNU Lesser General Public License v3.0
 """
 
 import setuptools
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.64.7",
+    version="1.64.8",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of complex social behaviors in experimental animals",
     url="https://github.com/sgoldenlab/simba",
     install_requires=['Pillow == 5.4.1', 'pyyaml == 5.3.1','shapely == 1.7','wxpython == 4.0.4',
               'dtreeviz == 0.8.1','eli5 == 0.10.1','graphviz == 0.11',
               'imblearn == 0.0','imgaug == 0.4.0','imutils == 0.5.2','matplotlib == 3.0.3', 'numpy == 1.18.1',
```

