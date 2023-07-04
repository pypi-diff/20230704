# Comparing `tmp/Simba-UW-tf-dev-1.64.1.tar.gz` & `tmp/Simba-UW-tf-dev-1.64.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.64.1.tar", last modified: Mon Jul  3 18:44:46 2023, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.64.2.tar", last modified: Tue Jul  4 15:18:31 2023, max compression
```

## Comparing `Simba-UW-tf-dev-1.64.1.tar` & `Simba-UW-tf-dev-1.64.2.tar`

### file list

```diff
@@ -1,583 +1,583 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/ui/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-07-03 15:11:10.000000 Simba-UW-tf-dev-1.64.1/simba/ui/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)     9015 2023-06-29 20:55:17.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/mutual_exclusivity_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/csv_2_parquet_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/quick_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/batch_preprocess_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/heatmap_location_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/clf_probability_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/movement_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/clf_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    15950 2023-05-20 12:10:35.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1150 2023-05-25 18:21:39.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/remove_roi_features_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5814 2023-06-15 20:06:37.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/roi_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5977 2023-05-31 12:58:14.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/outlier_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/gantt_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/clf_validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7721 2023-05-24 15:18:33.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/severity_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/fsttc_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/kleinberg_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7288 2023-05-29 20:14:50.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/pose_reorganizer_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/clf_by_timebins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/heatmap_clf_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/data_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/roi_features_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/pup_retrieval_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/about_simba_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3605 2023-05-25 18:54:56.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6353 2023-05-24 15:31:12.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    44112 2023-07-03 18:17:05.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/video_processing_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/clf_by_roi_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/make_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/archive_files_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/pose_bp_drop_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    10695 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/distance_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3601 2023-07-03 00:19:12.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    12869 2023-05-23 12:47:59.000000 Simba-UW-tf-dev-1.64.1/simba/ui/video_info_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.64.1/simba/ui/user_defined_pose_creator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/ui/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12879 2023-06-18 20:27:37.000000 Simba-UW-tf-dev-1.64.1/simba/ui/create_project_ui.py
--rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.64.1/simba/ui/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    35431 2023-06-13 17:24:57.000000 Simba-UW-tf-dev-1.64.1/simba/ui/machine_model_settings_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/blob_storage/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.64.1/simba/blob_storage/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/labelling/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.64.1/simba/labelling/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21667 2023-06-20 18:30:00.000000 Simba-UW-tf-dev-1.64.1/simba/labelling/labelling_interface_old.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/labelling/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    20914 2023-06-22 13:26:28.000000 Simba-UW-tf-dev-1.64.1/simba/labelling/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     3568 2023-05-19 11:18:49.000000 Simba-UW-tf-dev-1.64.1/simba/labelling/extract_labelled_frames.py
--rw-r--r--   0 simon      (501) staff       (20)    26943 2023-06-20 19:04:35.000000 Simba-UW-tf-dev-1.64.1/simba/labelling/labelling_advanced_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.64.1/simba/labelling/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.64.1/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.64.1/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-13 17:25:39.000000 Simba-UW-tf-dev-1.64.1/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.64.1/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.64.1/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.64.1/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     9846 2023-06-06 18:27:30.000000 Simba-UW-tf-dev-1.64.1/simba/unsupervised/ui.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/unsupervised/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.64.1/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.64.1/simba/unsupervised/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.64.1/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.64.1/simba/unsupervised/cluster_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.64.1/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)    10287 2023-06-06 17:50:12.000000 Simba-UW-tf-dev-1.64.1/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.64.1/simba/unsupervised/tsne.py
--rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.64.1/simba/unsupervised/cluster_visualizer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.1/simba/bounding_box_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/bounding_box_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.64.1/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.64.1/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.64.1/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.1/simba/bounding_box_tools/find_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.1/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    49156 2023-07-03 15:11:15.000000 Simba-UW-tf-dev-1.64.1/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7127 2023-05-28 19:41:35.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-07 20:28:11.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     8943 2023-06-05 18:15:28.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/shap_log_mp_2.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     8580 2023-05-31 20:02:32.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/shap_log_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)    30764 2023-06-13 17:23:34.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
--rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     4279 2023-06-01 12:49:14.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/read_files_mp_2.py
--rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:44:29.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-06-29 20:33:26.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3864 2023-05-19 19:41:40.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    18368 2023-07-03 18:44:03.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8244 2023-05-21 16:28:49.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/feature_extractor_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/feature_extractor_4bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/.idea/features_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/.idea/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/.idea/.name
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/feature_extractors/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    15434 2023-05-20 18:29:53.000000 Simba-UW-tf-dev-1.64.1/simba/requirements.txt
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-07-02 23:47:13.000000 Simba-UW-tf-dev-1.64.1/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43029 2023-06-05 17:40:09.000000 Simba-UW-tf-dev-1.64.1/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    38224 2023-06-15 15:41:52.000000 Simba-UW-tf-dev-1.64.1/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/mixins/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.64.1/simba/mixins/pose_importer_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     2938 2023-07-02 20:03:29.000000 Simba-UW-tf-dev-1.64.1/simba/mixins/video_processing_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/mixins/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.64.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.64.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.64.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    82442 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.64.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    51809 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.64.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    14391 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.64.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc
--rw-r--r--   0 simon      (501) staff       (20)    14188 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.64.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    37135 2023-06-02 12:12:15.000000 Simba-UW-tf-dev-1.64.1/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    61873 2023-05-19 21:14:46.000000 Simba-UW-tf-dev-1.64.1/simba/mixins/plotting_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     9145 2023-06-13 18:36:10.000000 Simba-UW-tf-dev-1.64.1/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    73291 2023-06-19 20:46:57.000000 Simba-UW-tf-dev-1.64.1/simba/mixins/train_model_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6094 2023-05-21 17:39:19.000000 Simba-UW-tf-dev-1.64.1/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    10759 2023-06-08 22:23:03.000000 Simba-UW-tf-dev-1.64.1/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.64.1/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.1/simba/third_party_label_appenders/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    18417 2023-06-18 19:01:16.000000 Simba-UW-tf-dev-1.64.1/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.64.1/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18934 2023-06-18 19:03:04.000000 Simba-UW-tf-dev-1.64.1/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8181 2023-05-21 17:19:25.000000 Simba-UW-tf-dev-1.64.1/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     6988 2023-05-21 17:31:04.000000 Simba-UW-tf-dev-1.64.1/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5239 2023-05-21 18:07:18.000000 Simba-UW-tf-dev-1.64.1/simba/third_party_label_appenders/solomon_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.1/simba/cue_light_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.1/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.1/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.1/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.1/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.64.1/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.1/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)    11876 2023-06-18 20:21:39.000000 Simba-UW-tf-dev-1.64.1/simba/utils/config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    21103 2023-06-20 12:58:32.000000 Simba-UW-tf-dev-1.64.1/simba/utils/enums.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.64.1/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7698 2023-07-03 16:08:55.000000 Simba-UW-tf-dev-1.64.1/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)     8807 2023-05-25 13:24:45.000000 Simba-UW-tf-dev-1.64.1/simba/utils/checks.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/utils/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    43313 2023-06-27 15:38:38.000000 Simba-UW-tf-dev-1.64.1/simba/utils/read_write.py
--rw-r--r--   0 simon      (501) staff       (20)     9841 2023-06-19 23:24:08.000000 Simba-UW-tf-dev-1.64.1/simba/utils/lookups.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/utils/cli/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/utils/cli/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6017 2023-05-28 13:41:20.000000 Simba-UW-tf-dev-1.64.1/simba/utils/cli/cli_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    14886 2023-07-03 16:08:55.000000 Simba-UW-tf-dev-1.64.1/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)    19250 2023-06-13 13:46:20.000000 Simba-UW-tf-dev-1.64.1/simba/utils/data.py
--rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.64.1/simba/utils/printing.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/st/
--rw-r--r--   0 simon      (501) staff       (20)      282 2023-06-16 17:26:25.000000 Simba-UW-tf-dev-1.64.1/simba/st/enums.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-16 13:55:39.000000 Simba-UW-tf-dev-1.64.1/simba/st/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2102 2023-06-19 19:54:19.000000 Simba-UW-tf-dev-1.64.1/simba/st/select_groups_pg.py
--rw-r--r--   0 simon      (501) staff       (20)     2325 2023-06-19 19:54:19.000000 Simba-UW-tf-dev-1.64.1/simba/st/aggregate_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     1485 2023-06-16 18:20:31.000000 Simba-UW-tf-dev-1.64.1/simba/st/app.py
--rw-r--r--   0 simon      (501) staff       (20)      249 2023-06-16 18:20:19.000000 Simba-UW-tf-dev-1.64.1/simba/st/welcome_page.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/pose_processors/
--rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.64.1/simba/pose_processors/reorganize_keypoint.py
--rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.64.1/simba/pose_processors/remove_keypoints.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.1/simba/pose_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/pose_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.64.1/simba/pose_processors/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)     5618 2023-06-13 18:36:10.000000 Simba-UW-tf-dev-1.64.1/simba/pose_processors/reverse_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.64.1/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.64.1/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    13008 2023-05-24 15:32:44.000000 Simba-UW-tf-dev-1.64.1/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.64.1/simba/plotting/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.64.1/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.64.1/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.64.1/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.64.1/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12484 2023-05-23 14:52:24.000000 Simba-UW-tf-dev-1.64.1/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    14056 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.64.1/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.64.1/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.64.1/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.64.1/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/plotting/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.64.1/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)    14029 2023-06-04 11:55:47.000000 Simba-UW-tf-dev-1.64.1/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)    13964 2023-07-03 17:17:59.000000 Simba-UW-tf-dev-1.64.1/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)     7660 2023-06-20 12:45:11.000000 Simba-UW-tf-dev-1.64.1/simba/plotting/pose_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     7891 2023-05-29 21:41:05.000000 Simba-UW-tf-dev-1.64.1/simba/plotting/Directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.64.1/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    15745 2023-05-20 12:16:06.000000 Simba-UW-tf-dev-1.64.1/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11203 2023-05-24 15:35:24.000000 Simba-UW-tf-dev-1.64.1/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.64.1/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13471 2023-05-20 12:15:46.000000 Simba-UW-tf-dev-1.64.1/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.64.1/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    11519 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.64.1/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.64.1/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.64.1/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     9385 2023-05-31 16:46:49.000000 Simba-UW-tf-dev-1.64.1/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     9526 2023-06-04 12:03:25.000000 Simba-UW-tf-dev-1.64.1/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10005 2023-05-29 21:36:37.000000 Simba-UW-tf-dev-1.64.1/simba/plotting/Directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.64.1/simba/plotting/heat_mapper_location_mp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/dash_app/
--rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/dash_app/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/dash_app/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/dash_app/dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-16 12:50:41.000000 Simba-UW-tf-dev-1.64.1/simba/dash_app/plotly_dash.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/data_processors/
--rw-r--r--   0 simon      (501) staff       (20)     7248 2023-05-25 19:01:00.000000 Simba-UW-tf-dev-1.64.1/simba/data_processors/agg_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.64.1/simba/data_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    11196 2023-05-28 19:50:35.000000 Simba-UW-tf-dev-1.64.1/simba/data_processors/severity_bout_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16285 2023-06-13 13:57:45.000000 Simba-UW-tf-dev-1.64.1/simba/data_processors/interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)     8127 2023-05-25 13:57:19.000000 Simba-UW-tf-dev-1.64.1/simba/data_processors/timebins_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    13451 2023-06-19 20:47:55.000000 Simba-UW-tf-dev-1.64.1/simba/data_processors/fsttc_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/data_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.64.1/simba/data_processors/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.64.1/simba/data_processors/directing_other_animals_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8624 2023-05-25 14:07:56.000000 Simba-UW-tf-dev-1.64.1/simba/data_processors/timebins_movement_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.64.1/simba/data_processors/severity_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.64.1/simba/data_processors/pup_retrieval_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.64.1/simba/data_processors/pybursts_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    11533 2023-05-28 19:50:34.000000 Simba-UW-tf-dev-1.64.1/simba/data_processors/severity_frame_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     6087 2023-06-28 20:32:32.000000 Simba-UW-tf-dev-1.64.1/simba/data_processors/mutual_exclusivity_corrector.py
--rw-r--r--   0 simon      (501) staff       (20)     9656 2023-05-25 13:32:25.000000 Simba-UW-tf-dev-1.64.1/simba/data_processors/kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8131 2023-05-25 14:37:36.000000 Simba-UW-tf-dev-1.64.1/simba/data_processors/movement_calculator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/model/
--rw-r--r--   0 simon      (501) staff       (20)    20086 2023-06-05 20:43:28.000000 Simba-UW-tf-dev-1.64.1/simba/model/train_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.1/simba/model/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3315 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.64.1/simba/model/inference_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    20849 2023-06-05 18:44:40.000000 Simba-UW-tf-dev-1.64.1/simba/model/grid_search_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3363 2023-05-19 11:12:45.000000 Simba-UW-tf-dev-1.64.1/simba/model/inference_validation.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.64.1/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.64.1/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.1/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43194 2023-06-22 13:51:00.000000 Simba-UW-tf-dev-1.64.1/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.64.1/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    20174 2023-06-12 15:28:58.000000 Simba-UW-tf-dev-1.64.1/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11608 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.64.1/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.64.1/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)     2290 2023-06-12 16:21:03.000000 Simba-UW-tf-dev-1.64.1/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    11474 2023-06-12 19:37:22.000000 Simba-UW-tf-dev-1.64.1/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5080 2023-06-22 13:37:25.000000 Simba-UW-tf-dev-1.64.1/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.64.1/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.64.1/simba/roi_tools/ROI_image.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.64.1/simba/pose_importers/sleap_csv_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/pose_importers/misc/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.64.1/simba/pose_importers/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.64.1/simba/pose_importers/misc/apt_trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.64.1/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.1/simba/pose_importers/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    12549 2023-05-17 20:32:56.000000 Simba-UW-tf-dev-1.64.1/simba/pose_importers/sleap_h5_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.64.1/simba/pose_importers/madlc_importer.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/pose_importers/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.64.1/simba/pose_importers/sleap_slp_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.64.1/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.1/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.64.1/simba/pose_importers/trk_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/pose_configurations/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/three_dimensions/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/three_dimensions/ui/
--rw-r--r--   0 simon      (501) staff       (20)     1747 2023-06-25 18:18:01.000000 Simba-UW-tf-dev-1.64.1/simba/three_dimensions/ui/define_px_to_mm_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/three_dimensions/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)     6777 2023-06-26 17:04:03.000000 Simba-UW-tf-dev-1.64.1/simba/three_dimensions/feature_extractors/generic_feature_extractor.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/three_dimensions/mixins/
--rw-r--r--   0 simon      (501) staff       (20)    38820 2023-06-23 01:28:48.000000 Simba-UW-tf-dev-1.64.1/simba/three_dimensions/mixins/config_reader.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/three_dimensions/mixins/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)    51001 2023-06-26 13:52:31.000000 Simba-UW-tf-dev-1.64.1/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    50997 2023-06-25 19:59:06.000000 Simba-UW-tf-dev-1.64.1/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1380 2023-06-26 13:52:31.000000 Simba-UW-tf-dev-1.64.1/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     1379 2023-06-25 19:59:06.000000 Simba-UW-tf-dev-1.64.1/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     3758 2023-06-26 13:45:44.000000 Simba-UW-tf-dev-1.64.1/simba/three_dimensions/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     3953 2023-06-25 18:18:01.000000 Simba-UW-tf-dev-1.64.1/simba/three_dimensions/mixins/plotting_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/three_dimensions/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     3192 2023-06-25 18:21:24.000000 Simba-UW-tf-dev-1.64.1/simba/three_dimensions/plotting/plot_pose_in_dir.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/three_dimensions/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     3445 2023-06-22 22:21:05.000000 Simba-UW-tf-dev-1.64.1/simba/three_dimensions/pose_importers/anipose_csv_import.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/three_dimensions/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     5832 2023-06-23 13:06:19.000000 Simba-UW-tf-dev-1.64.1/simba/three_dimensions/outlier_tools/outlier_corrector_movement.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/video_processors/
--rw-r--r--   0 simon      (501) staff       (20)    47592 2023-07-03 18:03:55.000000 Simba-UW-tf-dev-1.64.1/simba/video_processors/video_processing.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.64.1/simba/video_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.64.1/simba/video_processors/px_to_mm.py
--rw-r--r--   0 simon      (501) staff       (20)    24648 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.64.1/simba/video_processors/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     3748 2023-07-02 21:12:43.000000 Simba-UW-tf-dev-1.64.1/simba/video_processors/video_processing_new.py
--rw-r--r--   0 simon      (501) staff       (20)     7610 2023-07-03 18:21:05.000000 Simba-UW-tf-dev-1.64.1/simba/video_processors/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.64.1/simba/video_processors/extract_frames.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/video_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.64.1/simba/video_processors/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.64.1/simba/video_processors/extract_seqframes.py
--rw-r--r--   0 simon      (501) staff       (20)    11087 2023-05-14 16:24:59.000000 Simba-UW-tf-dev-1.64.1/simba/video_processors/batch_process_create_ffmpeg_commands.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6535 2023-05-25 14:24:01.000000 Simba-UW-tf-dev-1.64.1/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:37.000000 Simba-UW-tf-dev-1.64.1/simba/outlier_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8168 2023-06-01 12:38:34.000000 Simba-UW-tf-dev-1.64.1/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     2668 2023-05-25 14:26:49.000000 Simba-UW-tf-dev-1.64.1/simba/outlier_tools/skip_outlier_correction.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/outlier_tools/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/outlier_tools/.idea/outlier_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/outlier_tools/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/outlier_tools/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/outlier_tools/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/outlier_tools/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/outlier_tools/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/outlier_tools/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/outlier_tools/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    66374 2023-06-29 20:30:38.000000 Simba-UW-tf-dev-1.64.1/simba/SimBA.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/assets/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
--rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-06-15 21:18:05.000000 Simba-UW-tf-dev-1.64.1/simba/assets/shap/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    16388 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.64.1/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/assets/lookups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.64.1/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/assets/lookups/unsupervised_example_x.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.64.1/simba/assets/img/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.64.1/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.64.1/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.64.1/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/gif.png
--rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/pose.png
--rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/.DS_Store
--rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/stopwatch.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/dimensionality_reduction.png
--rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/restart.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/add_on.png
--rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/print.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/clean.png
--rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/clf_2.png
--rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/boris.png
--rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/clahe.png
--rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/about.png
--rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/reorganize.png
--rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.64.1/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.1/simba/assets/TheGoldenLab.PNG
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/Simba_UW_tf_dev.egg-info/
--rw-rw-r--   0 simon      (501) staff       (20)      579 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-rw-r--   0 simon      (501) staff       (20)    21675 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 simon      (501) staff       (20)       44 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-rw-r--   0 simon      (501) staff       (20)      639 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/Simba_UW_tf_dev.egg-info/requires.txt
--rw-rw-r--   0 simon      (501) staff       (20)       12 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-rw-r--   0 simon      (501) staff       (20)        1 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.64.1/LICENSE.md
--rw-r--r--   0 simon      (501) staff       (20)       89 2023-05-20 17:55:56.000000 Simba-UW-tf-dev-1.64.1/pyproject.toml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/tests/
--rw-r--r--   0 simon      (501) staff       (20)     5209 2023-05-28 14:15:24.000000 Simba-UW-tf-dev-1.64.1/tests/test_data_processors.py
--rw-r--r--   0 simon      (501) staff       (20)     5317 2023-05-31 19:40:16.000000 Simba-UW-tf-dev-1.64.1/tests/test_distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-13 13:57:45.000000 Simba-UW-tf-dev-1.64.1/tests/test_interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)    12374 2023-06-07 20:44:17.000000 Simba-UW-tf-dev-1.64.1/tests/test_train_model_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     2470 2023-06-12 20:51:29.000000 Simba-UW-tf-dev-1.64.1/tests/test_pose_importers.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.1/tests/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6757 2023-06-02 12:11:53.000000 Simba-UW-tf-dev-1.64.1/tests/test_feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-12 20:53:51.000000 Simba-UW-tf-dev-1.64.1/tests/test_pose_processors.py
--rw-r--r--   0 simon      (501) staff       (20)     1774 2023-06-13 19:27:04.000000 Simba-UW-tf-dev-1.64.1/tests/test_utils_data.py
--rw-r--r--   0 simon      (501) staff       (20)     8984 2023-06-07 20:11:11.000000 Simba-UW-tf-dev-1.64.1/tests/test_config_reader_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     1528 2023-05-25 14:26:19.000000 Simba-UW-tf-dev-1.64.1/tests/test_outlier_correctors.py
--rw-r--r--   0 simon      (501) staff       (20)     4356 2023-05-29 20:59:49.000000 Simba-UW-tf-dev-1.64.1/tests/test_visualize_directing_animals.py
--rw-r--r--   0 simon      (501) staff       (20)     1859 2023-05-21 16:40:19.000000 Simba-UW-tf-dev-1.64.1/tests/test_featurizers.py
--rw-r--r--   0 simon      (501) staff       (20)     8736 2023-06-13 13:49:50.000000 Simba-UW-tf-dev-1.64.1/tests/test_video_processors.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/tests/data/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.1/tests/data/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/tests/data/test_projects/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/tests/data/test_projects/two_c57/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/tests/data/test_projects/two_c57/video_processing/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.1/tests/data/test_projects/two_c57/video_processing/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/tests/data/test_projects/two_c57/video_processing/test_imgs/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.1/tests/data/test_projects/two_c57/video_processing/test_imgs/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.1/tests/data/test_projects/two_c57/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/tests/data/test_projects/two_c57/models/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.1/tests/data/test_projects/two_c57/models/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/tests/data/test_projects/two_c57/expected_animal_bp_dict/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.1/tests/data/test_projects/two_c57/expected_animal_bp_dict/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.1/tests/data/test_projects/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/tests/data/test_projects/mouse_open_field/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.1/tests/data/test_projects/mouse_open_field/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/tests/data/test_projects/zebrafish/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.1/tests/data/test_projects/zebrafish/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/tests/data/test_projects/zebrafish/models/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/tests/data/test_projects/zebrafish/models/generated_models/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.1/tests/data/test_projects/zebrafish/models/generated_models/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.1/tests/data/test_projects/zebrafish/models/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/tests/data/test_projects/zebrafish/models/validations/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.1/tests/data/test_projects/zebrafish/models/validations/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/tests/data/test_projects/zebrafish/project_folder/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.1/tests/data/test_projects/zebrafish/project_folder/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/tests/data/test_projects/zebrafish/project_folder/videos/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.1/tests/data/test_projects/zebrafish/project_folder/videos/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/tests/data/test_projects/zebrafish/project_folder/logs/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.1/tests/data/test_projects/zebrafish/project_folder/logs/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/tests/data/test_projects/zebrafish/project_folder/logs/measures/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.1/tests/data/test_projects/zebrafish/project_folder/logs/measures/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/tests/data/test_projects/zebrafish/feature_file/
--rw-rw-r--   0 simon      (501) staff       (20)        0 2020-08-11 16:11:18.000000 Simba-UW-tf-dev-1.64.1/tests/data/test_projects/zebrafish/feature_file/__init__.py
--rw-rw-r--   0 simon      (501) staff       (20)    14128 2022-04-11 08:07:36.000000 Simba-UW-tf-dev-1.64.1/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py
--rw-r--r--   0 simon      (501) staff       (20)     3971 2023-05-28 17:20:18.000000 Simba-UW-tf-dev-1.64.1/tests/test_thirdparty_appenders.py
--rw-r--r--   0 simon      (501) staff       (20)     3090 2023-05-31 15:49:24.000000 Simba-UW-tf-dev-1.64.1/tests/test_validation_clips.py
--rw-r--r--   0 simon      (501) staff       (20)     4463 2023-06-12 18:41:18.000000 Simba-UW-tf-dev-1.64.1/tests/test_roi_tools.py
--rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.64.1/MANIFEST.in
--rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.64.1/README.md
--rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-07-03 18:44:04.000000 Simba-UW-tf-dev-1.64.1/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-07-03 18:44:46.000000 Simba-UW-tf-dev-1.64.1/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:30.000000 Simba-UW-tf-dev-1.64.2/simba/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-07-03 15:11:10.000000 Simba-UW-tf-dev-1.64.2/simba/ui/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)     9015 2023-06-29 20:55:17.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/mutual_exclusivity_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/csv_2_parquet_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/quick_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/batch_preprocess_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/heatmap_location_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/clf_probability_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/movement_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/clf_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    15950 2023-05-20 12:10:35.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1150 2023-05-25 18:21:39.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/remove_roi_features_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5814 2023-06-15 20:06:37.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/roi_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5977 2023-05-31 12:58:14.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/outlier_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/gantt_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/clf_validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7721 2023-05-24 15:18:33.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/severity_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/fsttc_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/kleinberg_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7288 2023-05-29 20:14:50.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/pose_reorganizer_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/clf_by_timebins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/heatmap_clf_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/data_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/roi_features_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/pup_retrieval_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/about_simba_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3605 2023-05-25 18:54:56.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6353 2023-05-24 15:31:12.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    49706 2023-07-04 01:47:12.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/video_processing_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/clf_by_roi_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/make_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/archive_files_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/pose_bp_drop_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    10695 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/distance_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3601 2023-07-03 00:19:12.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    12869 2023-05-23 12:47:59.000000 Simba-UW-tf-dev-1.64.2/simba/ui/video_info_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.64.2/simba/ui/user_defined_pose_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/ui/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12879 2023-06-18 20:27:37.000000 Simba-UW-tf-dev-1.64.2/simba/ui/create_project_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.64.2/simba/ui/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    35431 2023-06-13 17:24:57.000000 Simba-UW-tf-dev-1.64.2/simba/ui/machine_model_settings_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/blob_storage/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.64.2/simba/blob_storage/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/labelling/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.64.2/simba/labelling/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21667 2023-06-20 18:30:00.000000 Simba-UW-tf-dev-1.64.2/simba/labelling/labelling_interface_old.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/labelling/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    20914 2023-06-22 13:26:28.000000 Simba-UW-tf-dev-1.64.2/simba/labelling/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     3568 2023-05-19 11:18:49.000000 Simba-UW-tf-dev-1.64.2/simba/labelling/extract_labelled_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)    26943 2023-06-20 19:04:35.000000 Simba-UW-tf-dev-1.64.2/simba/labelling/labelling_advanced_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.64.2/simba/labelling/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.64.2/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.64.2/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-13 17:25:39.000000 Simba-UW-tf-dev-1.64.2/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.64.2/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.64.2/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.64.2/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     9846 2023-06-06 18:27:30.000000 Simba-UW-tf-dev-1.64.2/simba/unsupervised/ui.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/unsupervised/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.64.2/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.64.2/simba/unsupervised/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.64.2/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.64.2/simba/unsupervised/cluster_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.64.2/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)    10287 2023-06-06 17:50:12.000000 Simba-UW-tf-dev-1.64.2/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.64.2/simba/unsupervised/tsne.py
+-rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.64.2/simba/unsupervised/cluster_visualizer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.2/simba/bounding_box_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/bounding_box_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.64.2/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.64.2/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.64.2/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.2/simba/bounding_box_tools/find_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.2/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    49156 2023-07-03 15:11:15.000000 Simba-UW-tf-dev-1.64.2/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7127 2023-05-28 19:41:35.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-07 20:28:11.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     8943 2023-06-05 18:15:28.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/shap_log_mp_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8580 2023-05-31 20:02:32.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/shap_log_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)    30764 2023-06-13 17:23:34.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     4279 2023-06-01 12:49:14.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/read_files_mp_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:44:29.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-06-29 20:33:26.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3864 2023-05-19 19:41:40.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    18368 2023-07-03 18:44:03.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8244 2023-05-21 16:28:49.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/feature_extractor_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/feature_extractor_4bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/.idea/features_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/.idea/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/.idea/.name
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/feature_extractors/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    15434 2023-05-20 18:29:53.000000 Simba-UW-tf-dev-1.64.2/simba/requirements.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-07-02 23:47:13.000000 Simba-UW-tf-dev-1.64.2/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43029 2023-06-05 17:40:09.000000 Simba-UW-tf-dev-1.64.2/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    38224 2023-06-15 15:41:52.000000 Simba-UW-tf-dev-1.64.2/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/mixins/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.64.2/simba/mixins/pose_importer_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     2938 2023-07-02 20:03:29.000000 Simba-UW-tf-dev-1.64.2/simba/mixins/video_processing_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/mixins/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.64.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.64.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.64.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    82442 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.64.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    51809 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.64.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    14391 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.64.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    14188 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.64.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    37135 2023-06-02 12:12:15.000000 Simba-UW-tf-dev-1.64.2/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    61873 2023-05-19 21:14:46.000000 Simba-UW-tf-dev-1.64.2/simba/mixins/plotting_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     9145 2023-06-13 18:36:10.000000 Simba-UW-tf-dev-1.64.2/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    73291 2023-06-19 20:46:57.000000 Simba-UW-tf-dev-1.64.2/simba/mixins/train_model_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6094 2023-05-21 17:39:19.000000 Simba-UW-tf-dev-1.64.2/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10759 2023-06-08 22:23:03.000000 Simba-UW-tf-dev-1.64.2/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.64.2/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.2/simba/third_party_label_appenders/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    18417 2023-06-18 19:01:16.000000 Simba-UW-tf-dev-1.64.2/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.64.2/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18934 2023-06-18 19:03:04.000000 Simba-UW-tf-dev-1.64.2/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8181 2023-05-21 17:19:25.000000 Simba-UW-tf-dev-1.64.2/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     6988 2023-05-21 17:31:04.000000 Simba-UW-tf-dev-1.64.2/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5239 2023-05-21 18:07:18.000000 Simba-UW-tf-dev-1.64.2/simba/third_party_label_appenders/solomon_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.2/simba/cue_light_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.2/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.2/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.2/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.2/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.64.2/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.2/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)    11876 2023-06-18 20:21:39.000000 Simba-UW-tf-dev-1.64.2/simba/utils/config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    21103 2023-06-20 12:58:32.000000 Simba-UW-tf-dev-1.64.2/simba/utils/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.64.2/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7698 2023-07-03 16:08:55.000000 Simba-UW-tf-dev-1.64.2/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)     9041 2023-07-04 00:56:52.000000 Simba-UW-tf-dev-1.64.2/simba/utils/checks.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/utils/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    43561 2023-07-03 19:45:27.000000 Simba-UW-tf-dev-1.64.2/simba/utils/read_write.py
+-rw-r--r--   0 simon      (501) staff       (20)     9841 2023-06-19 23:24:08.000000 Simba-UW-tf-dev-1.64.2/simba/utils/lookups.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/utils/cli/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/utils/cli/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6017 2023-05-28 13:41:20.000000 Simba-UW-tf-dev-1.64.2/simba/utils/cli/cli_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    14889 2023-07-04 00:56:52.000000 Simba-UW-tf-dev-1.64.2/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)    19250 2023-06-13 13:46:20.000000 Simba-UW-tf-dev-1.64.2/simba/utils/data.py
+-rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.64.2/simba/utils/printing.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/st/
+-rw-r--r--   0 simon      (501) staff       (20)      282 2023-06-16 17:26:25.000000 Simba-UW-tf-dev-1.64.2/simba/st/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-16 13:55:39.000000 Simba-UW-tf-dev-1.64.2/simba/st/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2102 2023-06-19 19:54:19.000000 Simba-UW-tf-dev-1.64.2/simba/st/select_groups_pg.py
+-rw-r--r--   0 simon      (501) staff       (20)     2325 2023-06-19 19:54:19.000000 Simba-UW-tf-dev-1.64.2/simba/st/aggregate_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     1485 2023-06-16 18:20:31.000000 Simba-UW-tf-dev-1.64.2/simba/st/app.py
+-rw-r--r--   0 simon      (501) staff       (20)      249 2023-06-16 18:20:19.000000 Simba-UW-tf-dev-1.64.2/simba/st/welcome_page.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/pose_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.64.2/simba/pose_processors/reorganize_keypoint.py
+-rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.64.2/simba/pose_processors/remove_keypoints.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.2/simba/pose_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/pose_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.64.2/simba/pose_processors/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)     5618 2023-06-13 18:36:10.000000 Simba-UW-tf-dev-1.64.2/simba/pose_processors/reverse_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.64.2/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.64.2/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    13008 2023-05-24 15:32:44.000000 Simba-UW-tf-dev-1.64.2/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.64.2/simba/plotting/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.64.2/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.64.2/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.64.2/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.64.2/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12484 2023-05-23 14:52:24.000000 Simba-UW-tf-dev-1.64.2/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    14056 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.64.2/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.64.2/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.64.2/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.64.2/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/plotting/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.64.2/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)    14029 2023-06-04 11:55:47.000000 Simba-UW-tf-dev-1.64.2/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)    13964 2023-07-03 17:17:59.000000 Simba-UW-tf-dev-1.64.2/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)     7660 2023-06-20 12:45:11.000000 Simba-UW-tf-dev-1.64.2/simba/plotting/pose_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     7891 2023-05-29 21:41:05.000000 Simba-UW-tf-dev-1.64.2/simba/plotting/Directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.64.2/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    15745 2023-05-20 12:16:06.000000 Simba-UW-tf-dev-1.64.2/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11203 2023-05-24 15:35:24.000000 Simba-UW-tf-dev-1.64.2/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.64.2/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13471 2023-05-20 12:15:46.000000 Simba-UW-tf-dev-1.64.2/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.64.2/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    11519 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.64.2/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.64.2/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.64.2/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     9385 2023-05-31 16:46:49.000000 Simba-UW-tf-dev-1.64.2/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     9526 2023-06-04 12:03:25.000000 Simba-UW-tf-dev-1.64.2/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10005 2023-05-29 21:36:37.000000 Simba-UW-tf-dev-1.64.2/simba/plotting/Directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.64.2/simba/plotting/heat_mapper_location_mp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/dash_app/
+-rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/dash_app/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/dash_app/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/dash_app/dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-16 12:50:41.000000 Simba-UW-tf-dev-1.64.2/simba/dash_app/plotly_dash.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/data_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     7248 2023-05-25 19:01:00.000000 Simba-UW-tf-dev-1.64.2/simba/data_processors/agg_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.64.2/simba/data_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    11196 2023-05-28 19:50:35.000000 Simba-UW-tf-dev-1.64.2/simba/data_processors/severity_bout_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16285 2023-06-13 13:57:45.000000 Simba-UW-tf-dev-1.64.2/simba/data_processors/interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8127 2023-05-25 13:57:19.000000 Simba-UW-tf-dev-1.64.2/simba/data_processors/timebins_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    13451 2023-06-19 20:47:55.000000 Simba-UW-tf-dev-1.64.2/simba/data_processors/fsttc_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/data_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.64.2/simba/data_processors/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.64.2/simba/data_processors/directing_other_animals_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8624 2023-05-25 14:07:56.000000 Simba-UW-tf-dev-1.64.2/simba/data_processors/timebins_movement_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.64.2/simba/data_processors/severity_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.64.2/simba/data_processors/pup_retrieval_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.64.2/simba/data_processors/pybursts_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    11533 2023-05-28 19:50:34.000000 Simba-UW-tf-dev-1.64.2/simba/data_processors/severity_frame_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     6087 2023-06-28 20:32:32.000000 Simba-UW-tf-dev-1.64.2/simba/data_processors/mutual_exclusivity_corrector.py
+-rw-r--r--   0 simon      (501) staff       (20)     9656 2023-05-25 13:32:25.000000 Simba-UW-tf-dev-1.64.2/simba/data_processors/kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8131 2023-05-25 14:37:36.000000 Simba-UW-tf-dev-1.64.2/simba/data_processors/movement_calculator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:30.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/model/
+-rw-r--r--   0 simon      (501) staff       (20)    20086 2023-06-05 20:43:28.000000 Simba-UW-tf-dev-1.64.2/simba/model/train_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.2/simba/model/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3315 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.64.2/simba/model/inference_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    20849 2023-06-05 18:44:40.000000 Simba-UW-tf-dev-1.64.2/simba/model/grid_search_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3363 2023-05-19 11:12:45.000000 Simba-UW-tf-dev-1.64.2/simba/model/inference_validation.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.64.2/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.64.2/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.2/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43194 2023-06-22 13:51:00.000000 Simba-UW-tf-dev-1.64.2/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.64.2/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    20174 2023-06-12 15:28:58.000000 Simba-UW-tf-dev-1.64.2/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11608 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.64.2/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.64.2/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)     2290 2023-06-12 16:21:03.000000 Simba-UW-tf-dev-1.64.2/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    11474 2023-06-12 19:37:22.000000 Simba-UW-tf-dev-1.64.2/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5080 2023-06-22 13:37:25.000000 Simba-UW-tf-dev-1.64.2/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.64.2/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.64.2/simba/roi_tools/ROI_image.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.64.2/simba/pose_importers/sleap_csv_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/pose_importers/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.64.2/simba/pose_importers/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.64.2/simba/pose_importers/misc/apt_trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.64.2/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.2/simba/pose_importers/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    12549 2023-05-17 20:32:56.000000 Simba-UW-tf-dev-1.64.2/simba/pose_importers/sleap_h5_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.64.2/simba/pose_importers/madlc_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/pose_importers/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.64.2/simba/pose_importers/sleap_slp_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.64.2/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.2/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.64.2/simba/pose_importers/trk_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/pose_configurations/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:30.000000 Simba-UW-tf-dev-1.64.2/simba/three_dimensions/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/three_dimensions/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     1747 2023-06-25 18:18:01.000000 Simba-UW-tf-dev-1.64.2/simba/three_dimensions/ui/define_px_to_mm_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/three_dimensions/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)     6777 2023-06-26 17:04:03.000000 Simba-UW-tf-dev-1.64.2/simba/three_dimensions/feature_extractors/generic_feature_extractor.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/three_dimensions/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)    38820 2023-06-23 01:28:48.000000 Simba-UW-tf-dev-1.64.2/simba/three_dimensions/mixins/config_reader.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/three_dimensions/mixins/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)    51001 2023-06-26 13:52:31.000000 Simba-UW-tf-dev-1.64.2/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    50997 2023-06-25 19:59:06.000000 Simba-UW-tf-dev-1.64.2/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1380 2023-06-26 13:52:31.000000 Simba-UW-tf-dev-1.64.2/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     1379 2023-06-25 19:59:06.000000 Simba-UW-tf-dev-1.64.2/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     3758 2023-06-26 13:45:44.000000 Simba-UW-tf-dev-1.64.2/simba/three_dimensions/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     3953 2023-06-25 18:18:01.000000 Simba-UW-tf-dev-1.64.2/simba/three_dimensions/mixins/plotting_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/three_dimensions/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     3192 2023-06-25 18:21:24.000000 Simba-UW-tf-dev-1.64.2/simba/three_dimensions/plotting/plot_pose_in_dir.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/three_dimensions/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     3445 2023-06-22 22:21:05.000000 Simba-UW-tf-dev-1.64.2/simba/three_dimensions/pose_importers/anipose_csv_import.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/three_dimensions/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5832 2023-06-23 13:06:19.000000 Simba-UW-tf-dev-1.64.2/simba/three_dimensions/outlier_tools/outlier_corrector_movement.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/video_processors/
+-rw-r--r--   0 simon      (501) staff       (20)    56116 2023-07-04 01:54:33.000000 Simba-UW-tf-dev-1.64.2/simba/video_processors/video_processing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.64.2/simba/video_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.64.2/simba/video_processors/px_to_mm.py
+-rw-r--r--   0 simon      (501) staff       (20)    24648 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.64.2/simba/video_processors/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     3748 2023-07-02 21:12:43.000000 Simba-UW-tf-dev-1.64.2/simba/video_processors/video_processing_new.py
+-rw-r--r--   0 simon      (501) staff       (20)     7610 2023-07-03 18:21:05.000000 Simba-UW-tf-dev-1.64.2/simba/video_processors/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.64.2/simba/video_processors/extract_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/video_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.64.2/simba/video_processors/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.64.2/simba/video_processors/extract_seqframes.py
+-rw-r--r--   0 simon      (501) staff       (20)    11087 2023-05-14 16:24:59.000000 Simba-UW-tf-dev-1.64.2/simba/video_processors/batch_process_create_ffmpeg_commands.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6535 2023-05-25 14:24:01.000000 Simba-UW-tf-dev-1.64.2/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:37.000000 Simba-UW-tf-dev-1.64.2/simba/outlier_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8168 2023-06-01 12:38:34.000000 Simba-UW-tf-dev-1.64.2/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     2668 2023-05-25 14:26:49.000000 Simba-UW-tf-dev-1.64.2/simba/outlier_tools/skip_outlier_correction.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/outlier_tools/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/outlier_tools/.idea/outlier_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/outlier_tools/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/outlier_tools/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/outlier_tools/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/outlier_tools/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/outlier_tools/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/outlier_tools/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/outlier_tools/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    66493 2023-07-04 00:43:21.000000 Simba-UW-tf-dev-1.64.2/simba/SimBA.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:30.000000 Simba-UW-tf-dev-1.64.2/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/assets/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-06-15 21:18:05.000000 Simba-UW-tf-dev-1.64.2/simba/assets/shap/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    16388 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.64.2/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/assets/lookups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.64.2/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/assets/lookups/unsupervised_example_x.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.64.2/simba/assets/img/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.64.2/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.64.2/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.64.2/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/gif.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/pose.png
+-rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/.DS_Store
+-rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/stopwatch.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/dimensionality_reduction.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/restart.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/add_on.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/print.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/clean.png
+-rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/clf_2.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/boris.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/clahe.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/about.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/reorganize.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.64.2/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.2/simba/assets/TheGoldenLab.PNG
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:30.000000 Simba-UW-tf-dev-1.64.2/Simba_UW_tf_dev.egg-info/
+-rw-rw-r--   0 simon      (501) staff       (20)      579 2023-07-04 15:18:30.000000 Simba-UW-tf-dev-1.64.2/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 simon      (501) staff       (20)    21675 2023-07-04 15:18:30.000000 Simba-UW-tf-dev-1.64.2/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       44 2023-07-04 15:18:30.000000 Simba-UW-tf-dev-1.64.2/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-rw-r--   0 simon      (501) staff       (20)      639 2023-07-04 15:18:30.000000 Simba-UW-tf-dev-1.64.2/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       12 2023-07-04 15:18:30.000000 Simba-UW-tf-dev-1.64.2/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        1 2023-07-04 15:18:30.000000 Simba-UW-tf-dev-1.64.2/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.64.2/LICENSE.md
+-rw-r--r--   0 simon      (501) staff       (20)       89 2023-05-20 17:55:56.000000 Simba-UW-tf-dev-1.64.2/pyproject.toml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/tests/
+-rw-r--r--   0 simon      (501) staff       (20)     5209 2023-05-28 14:15:24.000000 Simba-UW-tf-dev-1.64.2/tests/test_data_processors.py
+-rw-r--r--   0 simon      (501) staff       (20)     5317 2023-05-31 19:40:16.000000 Simba-UW-tf-dev-1.64.2/tests/test_distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-13 13:57:45.000000 Simba-UW-tf-dev-1.64.2/tests/test_interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)    12374 2023-06-07 20:44:17.000000 Simba-UW-tf-dev-1.64.2/tests/test_train_model_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     2470 2023-06-12 20:51:29.000000 Simba-UW-tf-dev-1.64.2/tests/test_pose_importers.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.2/tests/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6757 2023-06-02 12:11:53.000000 Simba-UW-tf-dev-1.64.2/tests/test_feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-12 20:53:51.000000 Simba-UW-tf-dev-1.64.2/tests/test_pose_processors.py
+-rw-r--r--   0 simon      (501) staff       (20)     1774 2023-06-13 19:27:04.000000 Simba-UW-tf-dev-1.64.2/tests/test_utils_data.py
+-rw-r--r--   0 simon      (501) staff       (20)     8984 2023-06-07 20:11:11.000000 Simba-UW-tf-dev-1.64.2/tests/test_config_reader_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     1528 2023-05-25 14:26:19.000000 Simba-UW-tf-dev-1.64.2/tests/test_outlier_correctors.py
+-rw-r--r--   0 simon      (501) staff       (20)     4356 2023-05-29 20:59:49.000000 Simba-UW-tf-dev-1.64.2/tests/test_visualize_directing_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)     1859 2023-05-21 16:40:19.000000 Simba-UW-tf-dev-1.64.2/tests/test_featurizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     8736 2023-06-13 13:49:50.000000 Simba-UW-tf-dev-1.64.2/tests/test_video_processors.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/tests/data/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.2/tests/data/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/tests/data/test_projects/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/tests/data/test_projects/two_c57/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/tests/data/test_projects/two_c57/video_processing/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.2/tests/data/test_projects/two_c57/video_processing/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/tests/data/test_projects/two_c57/video_processing/test_imgs/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.2/tests/data/test_projects/two_c57/video_processing/test_imgs/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.2/tests/data/test_projects/two_c57/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/tests/data/test_projects/two_c57/models/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.2/tests/data/test_projects/two_c57/models/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/tests/data/test_projects/two_c57/expected_animal_bp_dict/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.2/tests/data/test_projects/two_c57/expected_animal_bp_dict/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.2/tests/data/test_projects/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/tests/data/test_projects/mouse_open_field/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.2/tests/data/test_projects/mouse_open_field/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/tests/data/test_projects/zebrafish/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.2/tests/data/test_projects/zebrafish/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/tests/data/test_projects/zebrafish/models/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/tests/data/test_projects/zebrafish/models/generated_models/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.2/tests/data/test_projects/zebrafish/models/generated_models/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.2/tests/data/test_projects/zebrafish/models/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/tests/data/test_projects/zebrafish/models/validations/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.2/tests/data/test_projects/zebrafish/models/validations/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/tests/data/test_projects/zebrafish/project_folder/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.2/tests/data/test_projects/zebrafish/project_folder/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/tests/data/test_projects/zebrafish/project_folder/videos/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.2/tests/data/test_projects/zebrafish/project_folder/videos/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/tests/data/test_projects/zebrafish/project_folder/logs/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.2/tests/data/test_projects/zebrafish/project_folder/logs/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/tests/data/test_projects/zebrafish/project_folder/logs/measures/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.2/tests/data/test_projects/zebrafish/project_folder/logs/measures/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/tests/data/test_projects/zebrafish/feature_file/
+-rw-rw-r--   0 simon      (501) staff       (20)        0 2020-08-11 16:11:18.000000 Simba-UW-tf-dev-1.64.2/tests/data/test_projects/zebrafish/feature_file/__init__.py
+-rw-rw-r--   0 simon      (501) staff       (20)    14128 2022-04-11 08:07:36.000000 Simba-UW-tf-dev-1.64.2/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py
+-rw-r--r--   0 simon      (501) staff       (20)     3971 2023-05-28 17:20:18.000000 Simba-UW-tf-dev-1.64.2/tests/test_thirdparty_appenders.py
+-rw-r--r--   0 simon      (501) staff       (20)     3090 2023-05-31 15:49:24.000000 Simba-UW-tf-dev-1.64.2/tests/test_validation_clips.py
+-rw-r--r--   0 simon      (501) staff       (20)     4463 2023-06-12 18:41:18.000000 Simba-UW-tf-dev-1.64.2/tests/test_roi_tools.py
+-rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.64.2/MANIFEST.in
+-rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.64.2/README.md
+-rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-07-04 15:18:29.000000 Simba-UW-tf-dev-1.64.2/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-07-04 15:18:31.000000 Simba-UW-tf-dev-1.64.2/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.64.1/PKG-INFO` & `Simba-UW-tf-dev-1.64.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.64.1
+Version: 1.64.2
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/.DS_Store` & `Simba-UW-tf-dev-1.64.2/simba/ui/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/mutual_exclusivity_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/mutual_exclusivity_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/csv_2_parquet_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/csv_2_parquet_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/quick_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/quick_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/batch_preprocess_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/batch_preprocess_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/heatmap_location_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/heatmap_location_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/clf_probability_plot_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/clf_probability_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/.DS_Store` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/movement_analysis_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/movement_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/clf_plot_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/clf_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/path_plot_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/remove_roi_features_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/remove_roi_features_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/smoothing_interpolation_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/smoothing_interpolation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/roi_analysis_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/roi_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/outlier_settings_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/outlier_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/gantt_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/gantt_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/clf_validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/clf_validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/severity_analysis_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/severity_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/fsttc_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/fsttc_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/kleinberg_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/kleinberg_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/pose_reorganizer_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/pose_reorganizer_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/append_roi_features_animals_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/append_roi_features_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/clf_by_timebins_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/clf_by_timebins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/heatmap_clf_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/heatmap_clf_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/data_plot_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/data_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/roi_features_plot_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/roi_features_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/pup_retrieval_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/pup_retrieval_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/about_simba_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/about_simba_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/roi_tracking_plot_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/roi_tracking_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/clf_add_remove_print_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/clf_add_remove_print_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/video_processing_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/video_processing_pop_up.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,15 +39,17 @@
                                                      change_single_video_fps,
                                                      change_fps_of_multiple_videos,
                                                      frames_to_movie,
                                                      gif_creator,
                                                      video_concatenator,
                                                      VideoRotator,
                                                      copy_img_folder,
-                                                     downsample_video)
+                                                     downsample_video,
+                                                     video_to_greyscale,
+                                                     superimpose_frame_count)
 from simba.utils.enums import (Options,
                                Formats,
                                Paths,
                                Links,
                                Keys,
                                Dtypes)
 from simba.mixins.pop_up_mixin import PopUpMixin
@@ -74,60 +76,108 @@
         #self.main_frm.mainloop()
 
 #_ = CLAHEPopUp()
 
 class CropVideoPopUp(PopUpMixin):
     def __init__(self):
         super().__init__(title='CROP SINGLE VIDEO')
-        crop_video_lbl_frm = LabelFrame(self.main_frm, text='Crop Video',font='bold',padx=5,pady=5)
+        crop_video_lbl_frm = LabelFrame(self.main_frm, text='Crop Video', font=Formats.LABELFRAME_HEADER_FORMAT.value)
         selected_video = FileSelect(crop_video_lbl_frm,"Video path",title='Select a video file', lblwidth=20)
-        button_crop_video_single = Button(crop_video_lbl_frm, text='Crop Video',command=lambda: crop_single_video(file_path=selected_video.file_path))
+        use_gpu_var_single = BooleanVar(value=False)
+        use_gpu_cb_single = Checkbutton(crop_video_lbl_frm, text='Use GPU (potentially much faster)', variable=use_gpu_var_single)
+        button_crop_video_single = Button(crop_video_lbl_frm, text='Crop Video',command=lambda: crop_single_video(file_path=selected_video.file_path, gpu=use_gpu_var_single.get()))
 
         crop_video_lbl_frm_multiple = LabelFrame(self.main_frm, text='Fixed coordinates crop for multiple videos', font='bold',  padx=5, pady=5)
         input_folder = FolderSelect(crop_video_lbl_frm_multiple, 'Video directory:', title='Select Folder with videos', lblwidth=20)
         output_folder = FolderSelect(crop_video_lbl_frm_multiple, 'Output directory:', title='Select a folder for your output videos', lblwidth=20)
-        button_crop_video_multiple = Button(crop_video_lbl_frm_multiple, text='Confirm', command=lambda: crop_multiple_videos(directory_path=input_folder.folder_path, output_path=output_folder.folder_path))
-
+        use_gpu_var_multiple = BooleanVar(value=False)
+        use_gpu_cb_multiple = Checkbutton(crop_video_lbl_frm_multiple, text='Use GPU (potentially much faster)', variable=use_gpu_var_multiple)
+        button_crop_video_multiple = Button(crop_video_lbl_frm_multiple, text='Crop Videos', command=lambda: crop_multiple_videos(directory_path=input_folder.folder_path, output_path=output_folder.folder_path, gpu=use_gpu_var_multiple.get()))
         crop_video_lbl_frm.grid(row=0, sticky=NW)
         selected_video.grid(row=0, sticky=NW)
-        button_crop_video_single.grid(row=1, sticky=NW, pady=10)
-        crop_video_lbl_frm_multiple.grid(row=1, sticky=W, pady=10, padx=5)
-        input_folder.grid(row=0,sticky=W,pady=5)
-        output_folder.grid(row=1,sticky=W,pady=5)
-        button_crop_video_multiple.grid(row=2,sticky=W,pady=5)
-
-#_ = CropVideoPopUp()
+        use_gpu_cb_single.grid(row=1, column=0, sticky=NW)
+        button_crop_video_single.grid(row=2, sticky=NW)
+        crop_video_lbl_frm_multiple.grid(row=1, sticky=NW)
+        input_folder.grid(row=0,sticky=NW)
+        output_folder.grid(row=1,sticky=NW)
+        use_gpu_cb_multiple.grid(row=2,sticky=NW)
+        button_crop_video_multiple.grid(row=3,sticky=NW)
+#         self.main_frm.mainloop()
+#
+# _ = CropVideoPopUp()
 
 
 class ClipVideoPopUp(PopUpMixin):
     def __init__(self):
         super().__init__(title='CLIP VIDEO')
-        selected_video = CreateLabelFrameWithIcon(parent=self.main_frm, header='Video path', icon_name=Keys.DOCUMENTATION.value, icon_link=Links.VIDEO_TOOLS.value)
+        selected_video_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header='Video path', icon_name=Keys.DOCUMENTATION.value, icon_link=Links.VIDEO_TOOLS.value)
+        selected_video = FileSelect(selected_video_frm, 'FILE PATH: ')
+        selected_video.grid(row=0, column=0, sticky='NW')
+        use_gpu_frm = LabelFrame(self.main_frm, text='GPU', font='bold', padx=5, pady=5)
+        self.use_gpu_var = BooleanVar(value=False)
+        self.use_gpu_cb = Checkbutton(use_gpu_frm, text='Use GPU (potentially much faster)', variable=self.use_gpu_var)
+        self.use_gpu_cb.grid(row=0, column=0, sticky=NW)
         method_1_frm = LabelFrame(self.main_frm, text='Method 1', font='bold', padx=5, pady=5)
         label_set_time_1 = Label(method_1_frm, text='Please enter the time frame in hh:mm:ss format')
         start_time = Entry_Box(method_1_frm, 'Start at (s):', '8', validation='numeric')
         end_time = Entry_Box(method_1_frm, 'End at (s):', '8', validation='numeric')
         CreateToolTip(method_1_frm, 'Method 1 will retrieve the specified time input. (eg: input of Start at: 00:00:00, End at: 00:01:00, will create a new video from the chosen video from the very start till it reaches the first minute of the video)')
         method_2_frm = LabelFrame(self.main_frm, text='Method 2', font='bold', padx=5, pady=5)
         method_2_time = Entry_Box(method_2_frm, 'Seconds:', '8', validation='numeric')
         label_method_2 = Label(method_2_frm, text='Method 2 will retrieve from the end of the video (e.g.,: an input of 3 seconds will get rid of the first 3 seconds of the video).')
-        button_cutvideo_method_1 = Button(method_1_frm, text='Cut Video', command=lambda: clip_video_in_range(file_path=selected_video.file_path, start_time=start_time.entry_get, end_time=end_time.entry_get))
-        button_cutvideo_method_2 = Button(method_2_frm, text='Cut Video', command=lambda: remove_beginning_of_video( file_path=selected_video.file_path, time=method_2_time.entry_get))
-        selected_video.grid(row=0, sticky=W)
-        method_1_frm.grid(row=1, sticky=NW, pady=5)
+        button_cutvideo_method_1 = Button(method_1_frm, text='Cut Video', command=lambda: clip_video_in_range(file_path=selected_video.file_path, start_time=start_time.entry_get, end_time=end_time.entry_get, gpu=self.use_gpu_var.get()))
+        button_cutvideo_method_2 = Button(method_2_frm, text='Cut Video', command=lambda: remove_beginning_of_video( file_path=selected_video.file_path, time=method_2_time.entry_get, gpu=self.use_gpu_var.get()))
+        selected_video_frm.grid(row=0, sticky=NW)
+        use_gpu_frm.grid(row=1, column=0, sticky=NW)
+        method_1_frm.grid(row=2, sticky=NW, pady=5)
         label_set_time_1.grid(row=0, sticky=NW)
         start_time.grid(row=1, sticky=NW)
         end_time.grid(row=2, sticky=NW)
         button_cutvideo_method_1.grid(row=3, sticky=NW)
-        method_2_frm.grid(row=2, sticky=NW, pady=5)
+        method_2_frm.grid(row=3, sticky=NW, pady=5)
         label_method_2.grid(row=0, sticky=NW)
         method_2_time.grid(row=2, sticky=NW)
         button_cutvideo_method_2.grid(row=3, sticky=NW)
-        #self.main_frm.mainloop()
-#_ = ClipVideoPopUp()
+#       self.main_frm.mainloop()
+# _ = ClipVideoPopUp()
+
+
+class GreyscaleSingleVideoPopUp(PopUpMixin):
+    def __init__(self):
+        super().__init__(title='GREYSCALE SINGLE VIDEO')
+        settings_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header='GREYSCALE VIDEO', icon_name=Keys.DOCUMENTATION.value, icon_link=Links.VIDEO_TOOLS.value)
+        self.selected_video = FileSelect(settings_frm, "VIDEO PATH", title='Select a video file', lblwidth=10)
+        self.use_gpu_var = BooleanVar(value=False)
+        use_gpu_cb = Checkbutton(settings_frm, text='Use GPU (potentially faster)', variable=self.use_gpu_var)
+
+        settings_frm.grid(row=0, column=0, sticky='NW')
+        self.selected_video.grid(row=0, column=0, sticky='NW')
+        use_gpu_cb.grid(row=1, column=0, sticky='NW')
+        self.create_run_frm(run_function=self.run)
+
+    def run(self):
+        check_file_exist_and_readable(file_path=self.selected_video.file_path)
+        video_to_greyscale(file_path=self.selected_video.file_path, gpu=self.use_gpu_var.get())
+
+class SuperImposeFrameCountPopUp(PopUpMixin):
+    def __init__(self):
+        super().__init__(title='SUPERIMPOSE FRAME COUNT ON VIDEO')
+        settings_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header='SUPERIMPOSE FRAME COUNT ON VIDEO', icon_name=Keys.DOCUMENTATION.value, icon_link=Links.VIDEO_TOOLS.value)
+        self.selected_video = FileSelect(settings_frm, "VIDEO PATH", title='Select a video file', lblwidth=10)
+        self.use_gpu_var = BooleanVar(value=False)
+        use_gpu_cb = Checkbutton(settings_frm, text='Use GPU (potentially faster)', variable=self.use_gpu_var)
+
+        settings_frm.grid(row=0, column=0, sticky='NW')
+        self.selected_video.grid(row=0, column=0, sticky='NW')
+        use_gpu_cb.grid(row=1, column=0, sticky='NW')
+        self.create_run_frm(run_function=self.run)
+
+    def run(self):
+        check_file_exist_and_readable(file_path=self.selected_video.file_path)
+        superimpose_frame_count(file_path=self.selected_video.file_path, gpu=self.use_gpu_var.get())
 
 class MultiShortenPopUp(PopUpMixin):
     def __init__(self):
         super().__init__(title='CLIP VIDEO INTO MULTIPLE VIDEOS')
         settings_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header='Split videos into different parts', icon_name=Keys.DOCUMENTATION.value, icon_link=Links.VIDEO_TOOLS.value)
         self.selected_video = FileSelect(settings_frm, "Video path", title='Select a video file', lblwidth=10)
         self.clip_cnt = Entry_Box(settings_frm, '# of clips', '10', validation='numeric')
@@ -235,41 +285,49 @@
 
 
 class ConvertVideoPopUp(PopUpMixin):
     def __init__(self):
         PopUpMixin.__init__(self, title="CONVERT VIDEO FORMAT", size=(200, 200))
         convert_multiple_videos_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header='Convert multiple videos', icon_name=Keys.DOCUMENTATION.value, icon_link=Links.VIDEO_TOOLS.value)
         video_dir = FolderSelect(convert_multiple_videos_frm, 'Video directory', title='Select folder with videos', lblwidth=15)
-        original_format = Entry_Box(convert_multiple_videos_frm, 'Input format', '15')
-        output_format = Entry_Box(convert_multiple_videos_frm, 'Output format', '15')
-        convert_multiple_btn = Button(convert_multiple_videos_frm, text='Convert multiple videos', command=lambda: batch_convert_video_format(directory=video_dir.folder_path, input_format=original_format.entry_get, output_format=output_format.entry_get))
-
+        video_format_options = ['mp4', 'avi', 'mov', 'flv', 'm4v']
+        original_format_dropdown = DropDownMenu(convert_multiple_videos_frm, 'Input format', video_format_options, labelwidth=15)
+        output_format_dropdown = DropDownMenu(convert_multiple_videos_frm, 'Input format', video_format_options, labelwidth=15)
+        original_format_dropdown.setChoices('avi')
+        output_format_dropdown.setChoices('mp4')
+        gpu_multiple_var = BooleanVar(value=False)
+        gpu_multiple_cb = Checkbutton(convert_multiple_videos_frm, text='Use GPU (potentially faster)', variable=gpu_multiple_var)
+        convert_multiple_btn = Button(convert_multiple_videos_frm, text='Convert multiple videos', command=lambda: batch_convert_video_format(directory=video_dir.folder_path, input_format=original_format_dropdown.getChoices(), output_format=output_format_dropdown.getChoices(), gpu=gpu_multiple_var.get()))
         convert_single_video_frm = LabelFrame(self.main_frm,text='Convert single video',font=("Helvetica",12,'bold'),padx=5,pady=5)
         self.selected_video = FileSelect(convert_single_video_frm, "Video path", title='Select a video file')
         self.output_format = StringVar()
         checkbox_v1 = Radiobutton(convert_single_video_frm, text="Convert to .mp4", variable=self.output_format, value='mp4')
         checkbox_v2 = Radiobutton(convert_single_video_frm, text="Convert mp4 into PowerPoint supported format", variable=self.output_format, value='pptx')
+        self.gpu_single_var = BooleanVar(value=False)
+        gpu_single_cb = Checkbutton(convert_single_video_frm, text='Use GPU (potentially faster)', variable=self.gpu_single_var)
         convert_single_btn = Button(convert_single_video_frm, text='Convert video format', command= lambda: self.convert_single())
 
-        convert_multiple_videos_frm.grid(row=0,sticky=W)
-        video_dir.grid(row=0,sticky=W)
-        original_format.grid(row=1,sticky=W)
-        output_format.grid(row=2,sticky=W)
-        convert_multiple_btn.grid(row=3,pady=10)
-        convert_single_video_frm.grid(row=1,sticky=W)
-        self.selected_video.grid(row=0,sticky=W)
-        checkbox_v1.grid(row=1,column=0,sticky=W)
-        checkbox_v2.grid(row=2,column=0,sticky=W)
-        convert_single_btn.grid(row=3,column=0,pady=10)
+        convert_multiple_videos_frm.grid(row=0,sticky=NW)
+        video_dir.grid(row=0,sticky=NW)
+        original_format_dropdown.grid(row=1,sticky=NW)
+        output_format_dropdown.grid(row=2,sticky=NW)
+        gpu_multiple_cb.grid(row=3,sticky=NW)
+        convert_multiple_btn.grid(row=4,pady=10, sticky=NW)
+        convert_single_video_frm.grid(row=1,sticky=NW)
+        self.selected_video.grid(row=0,sticky=NW)
+        checkbox_v1.grid(row=1,column=0,sticky=NW)
+        checkbox_v2.grid(row=2,column=0,sticky=NW)
+        gpu_single_cb.grid(row=3,column=0,sticky=NW)
+        convert_single_btn.grid(row=4,column=0,pady=10, sticky=NW)
 
     def convert_single(self):
         if self.output_format.get() == 'mp4':
-            convert_to_mp4(file_path=self.selected_video.file_path)
+            convert_to_mp4(file_path=self.selected_video.file_path, gpu=self.gpu_single_var.get())
         if self.output_format.get() == 'pptx':
-            convert_video_powerpoint_compatible_format(file_path=self.selected_video.file_path)
+            convert_video_powerpoint_compatible_format(file_path=self.selected_video.file_path, gpu=self.gpu_single_var.get())
 
 
 class ExtractSpecificFramesPopUp(PopUpMixin):
     def __init__(self):
         PopUpMixin.__init__(self, title="EXTRACT DEFINED FRAMES", size=(200,200))
         self.video_file_selected = FileSelect(self.main_frm, "Video path", title='Select a video file')
         select_frames_frm = LabelFrame(self.main_frm, text='Frames to be extracted', padx=5, pady=5)
@@ -340,30 +398,36 @@
         crop_cnt_dropdown.grid(row=3,sticky=NW)
         use_gpu_cb.grid(row=4, sticky=NW)
         run_btn.grid(row=5, pady=10)
 
 class ChangeFpsSingleVideoPopUp(PopUpMixin):
     def __init__(self):
         PopUpMixin.__init__(self, title="CHANGE FRAME RATE: SINGLE VIDEO", size=(200, 200))
-        video_path = FileSelect(self.main_frm, "Video path", title='Select a video file')
+        video_path = FileSelect(self.main_frm, "Video path", title='Select a video file', lblwidth=10)
         fps_entry_box = Entry_Box(self.main_frm, 'Output FPS:', '10', validation='numeric')
-        run_btn = Button(self.main_frm, text='Convert', command=lambda: change_single_video_fps(file_path=video_path.file_path, fps=fps_entry_box.entry_get))
-        video_path.grid(row=0,sticky=W)
-        fps_entry_box.grid(row=1,sticky=W)
-        run_btn.grid(row=2)
+        gpu_var = BooleanVar(value=False)
+        gpu_cb = Checkbutton(self.main_frm, text='Use GPU (potentially faster runtime)', variable=gpu_var)
+        run_btn = Button(self.main_frm, text='Convert', command=lambda: change_single_video_fps(file_path=video_path.file_path, fps=fps_entry_box.entry_get, gpu=gpu_var.get()))
+        video_path.grid(row=0, sticky=NW)
+        fps_entry_box.grid(row=1, sticky=NW)
+        gpu_cb.grid(row=2, sticky=NW)
+        run_btn.grid(row=3, sticky=NW)
 
 class ChangeFpsMultipleVideosPopUp(PopUpMixin):
     def __init__(self):
         PopUpMixin.__init__(self, title="CHANGE FRAME RATE: MULTIPLE VIDEO", size=(400, 200))
-        folder_path = FolderSelect(self.main_frm, "Folder path", title='Select folder with videos: ')
+        folder_path = FolderSelect(self.main_frm, "Folder path", title='Select folder with videos: ', lblwidth='10')
         fps_entry = Entry_Box(self.main_frm, 'Output FPS: ', '10', validation='numeric')
-        run_btn = Button(self.main_frm, text='Convert', command=lambda: change_fps_of_multiple_videos(directory=folder_path.folder_path, fps=fps_entry.entry_get))
-        folder_path.grid(row=0, sticky=W)
-        fps_entry.grid(row=1, sticky=W)
-        run_btn.grid(row=2)
+        gpu_var = BooleanVar(value=False)
+        gpu_cb = Checkbutton(self.main_frm, text='Use GPU (potentially faster runtime)', variable=gpu_var)
+        run_btn = Button(self.main_frm, text='Convert', command=lambda: change_fps_of_multiple_videos(directory=folder_path.folder_path, fps=fps_entry.entry_get, gpu=gpu_var.get()))
+        folder_path.grid(row=0, sticky=NW)
+        fps_entry.grid(row=1, sticky=NW)
+        gpu_cb.grid(row=2, sticky=NW)
+        run_btn.grid(row=3, sticky=NW)
 
 class ExtractSEQFramesPopUp(PopUpMixin):
     def __init__(self):
         PopUpMixin.__init__(self, title="EXTRACT ALL FRAMES FROM SEQ FILE", size=(200, 200))
         video_path = FileSelect(self.main_frm, "Video Path", title='Select a video file: ')
         run_btn = Button(self.main_frm, text='Extract All Frames', command=lambda: extract_seq_frames(video_path.file_path))
         video_path.grid(row=0)
@@ -396,24 +460,27 @@
     def __init__(self):
         PopUpMixin.__init__(self, title="CREATE GIF FROM VIDEO", size=(250, 250))
         settings_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header='SETTINGS', icon_name=Keys.DOCUMENTATION.value, icon_link=Links.VIDEO_TOOLS.value)
         selected_video = FileSelect(settings_frm, 'Video path: ', title='Select a video file')
         start_time_entry_box = Entry_Box(settings_frm, 'Start time (s): ', '16', validation='numeric')
         duration_entry_box = Entry_Box(settings_frm, 'Duration (s): ', '16', validation='numeric')
         width_entry_box = Entry_Box(settings_frm, 'Width: ', '16', validation='numeric')
+        gpu_var = BooleanVar()
+        gpu_cb = Checkbutton(settings_frm, text='Use GPU (potential runtime improvement)', variable=gpu_var)
         width_instructions_1 = Label(settings_frm, text='example Width: 240, 360, 480, 720, 1080', font=("Times", 10, "italic"))
         width_instructions_2 = Label(settings_frm, text='Aspect ratio is kept (i.e., height is automatically computed)', font=("Times", 10, "italic"))
-        run_btn = Button(settings_frm,text='CREATE GIF', command=lambda:gif_creator(file_path=selected_video.file_path, start_time=start_time_entry_box.entry_get, duration=duration_entry_box.entry_get, width=width_entry_box.entry_get))
-        settings_frm.grid(row=0,sticky=W)
-        selected_video.grid(row=0,sticky=W,pady=5)
-        start_time_entry_box.grid(row=1,sticky=W)
-        duration_entry_box.grid(row=2,sticky=W)
-        width_entry_box.grid(row=3,sticky=W)
-        width_instructions_1.grid(row=4,sticky=W)
-        width_instructions_2.grid(row=5, sticky=W)
+        run_btn = Button(settings_frm,text='CREATE GIF', command=lambda:gif_creator(file_path=selected_video.file_path, start_time=start_time_entry_box.entry_get, duration=duration_entry_box.entry_get, width=width_entry_box.entry_get, gpu=gpu_var.get()))
+        settings_frm.grid(row=0,sticky=NW)
+        selected_video.grid(row=0,sticky=NW,pady=5)
+        start_time_entry_box.grid(row=1,sticky=NW)
+        duration_entry_box.grid(row=2,sticky=NW)
+        width_entry_box.grid(row=3,sticky=NW)
+        gpu_cb.grid(row=4, column=0, sticky=NW)
+        width_instructions_1.grid(row=4,sticky=NW)
+        width_instructions_2.grid(row=5, sticky=NW)
         run_btn.grid(row=6,sticky=NW, pady=10)
 
 class CalculatePixelsPerMMInVideoPopUp(PopUpMixin):
     def __init__(self):
         PopUpMixin.__init__(self, title='CALCULATE PIXELS PER MILLIMETER IN VIDEO', size=(200, 200))
         self.video_path = FileSelect(self.main_frm, "Select a video file: ", title='Select a video file')
         self.known_distance = Entry_Box(self.main_frm, 'Known length in real life (mm): ', '0', validation='numeric')
@@ -572,28 +639,32 @@
 
 class VideoTemporalJoinPopUp(PopUpMixin):
     def __init__(self):
         super().__init__(title='TEMPORAL JOIN VIDEOS')
         self.settings_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header='SETTINGS', icon_name=Keys.DOCUMENTATION.value, icon_link=Links.VIDEO_TOOLS.value)
         self.input_dir = FolderSelect(self.settings_frm, 'INPUT DIRECTORY:', lblwidth=20)
         self.file_format = DropDownMenu(self.settings_frm, 'INPUT FORMAT:', Options.VIDEO_FORMAT_OPTIONS.value, '20')
+        self.use_gpu_var = BooleanVar(value=False)
+        use_gpu_cb = Checkbutton(self.settings_frm, text='Use GPU (potentially much faster)', variable=self.use_gpu_var)
         self.file_format.setChoices(Options.VIDEO_FORMAT_OPTIONS.value[0])
         self.settings_frm.grid(row=0, column=0, sticky=NW)
         self.input_dir.grid(row=0, column=0, sticky=NW)
         self.file_format.grid(row=1, column=0, sticky=NW)
+        use_gpu_cb.grid(row=2, column=0, sticky='NW')
         self.create_run_frm(run_function=self.run)
 
     def run(self):
         check_if_dir_exists(in_dir=self.input_dir.folder_path)
         print(f'Concatenating videos in {self.input_dir.folder_path} directory...')
         save_path = os.path.join(self.input_dir.folder_path, f'concatenated.mp4')
         concatenate_videos_in_folder(in_folder=self.input_dir.folder_path,
                                      save_path=save_path,
                                      remove_splits=False,
-                                     video_format=self.file_format.getChoices())
+                                     video_format=self.file_format.getChoices(),
+                                     gpu=self.use_gpu_var.get())
 
 
 
 class ImportFrameDirectoryPopUp(PopUpMixin, ConfigReader):
     def __init__(self,
                  config_path: str):
 
@@ -643,14 +714,18 @@
 class DownsampleVideoPopUp(PopUpMixin):
     def __init__(self):
 
         super().__init__(title='DOWN-SAMPLE VIDEO RESOLUTION')
         instructions = Label(self.main_frm, text='Choose only one of the following method (Custom or Default)')
         choose_video_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header='SELECT VIDEO', icon_name=Keys.DOCUMENTATION.value, icon_link=Links.DOWNSAMPLE.value)
         self.video_path_selected = FileSelect(choose_video_frm, "Video path", title='Select a video file')
+        gpu_frm = LabelFrame(self.main_frm, text='GPU', font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black', padx=5, pady=5)
+        self.use_gpu_var = BooleanVar(value=False)
+        use_gpu_cb = Checkbutton(gpu_frm, text='Use GPU (potentially much faster)', variable=self.use_gpu_var)
+        use_gpu_cb.grid(row=0, column=0, sticky='NW')
         custom_frm = LabelFrame(self.main_frm, text='Custom resolution', font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black', padx=5, pady=5)
         self.entry_width = Entry_Box(custom_frm, 'Width', '10', validation='numeric')
         self.entry_height = Entry_Box(custom_frm, 'Height', '10', validation='numeric')
 
         self.custom_downsample_btn = Button(custom_frm, text='Downsample to custom resolution', font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black', command=lambda: self.custom_downsample())
         default_frm = LabelFrame(self.main_frm, text='Default resolution', font='bold', padx=5, pady=5)
         self.radio_btns = {}
@@ -658,32 +733,33 @@
         for custom_cnt, resolution_radiobtn in enumerate(self.resolutions):
             self.radio_btns[resolution_radiobtn] = Radiobutton(default_frm, text=resolution_radiobtn, variable=self.var, value=resolution_radiobtn)
             self.radio_btns[resolution_radiobtn].grid(row=custom_cnt, sticky=NW)
 
         self.default_downsample_btn = Button(default_frm, text='Downsample to default resolution',command=lambda: self.default_downsample())
         instructions.grid(row=0,sticky=NW,pady=10)
         choose_video_frm.grid(row=1, column=0,sticky=NW)
+        gpu_frm.grid(row=2, column=0, sticky=NW)
         self.video_path_selected.grid(row=0, column=0,sticky=NW)
-        custom_frm.grid(row=2, column=0,sticky=NW)
+        custom_frm.grid(row=3, column=0,sticky=NW)
         self.entry_width.grid(row=0, column=0,sticky=NW)
         self.entry_height.grid(row=1, column=0, sticky=NW)
         self.custom_downsample_btn.grid(row=3, column=0, sticky=NW)
-        default_frm.grid(row=4, column=0, sticky=NW)
+        default_frm.grid(row=5, column=0, sticky=NW)
         self.default_downsample_btn.grid(row=len(self.resolutions)+1, column=0, sticky=NW)
 
     def custom_downsample(self):
         width = self.entry_width.entry_get
         height = self.entry_height.entry_get
         check_int(name='Video width', value=width)
         check_int(name='Video height', value=height)
         check_file_exist_and_readable(self.video_path_selected.file_path)
-        downsample_video(file_path=self.video_path_selected.file_path, video_width=int(width), video_height=int(height))
+        downsample_video(file_path=self.video_path_selected.file_path, video_width=int(width), video_height=int(height), gpu=self.use_gpu_var.get())
 
     def default_downsample(self):
         resolution = self.var.get()
         width, height = resolution.split('×', 2)[0].strip(), resolution.split('×', 2)[1].strip()
         check_file_exist_and_readable(self.video_path_selected.file_path)
-        downsample_video(file_path=self.video_path_selected.file_path, video_width=int(width), video_height=int(height))
+        downsample_video(file_path=self.video_path_selected.file_path, video_width=int(width), video_height=int(height),  gpu=self.use_gpu_var.get())
 
 #_ = DownsampleVideoPopUp()
```

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/clf_by_roi_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/clf_by_roi_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/make_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/make_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/archive_files_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/archive_files_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/pose_bp_drop_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/pose_bp_drop_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/distance_plot_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/distance_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/subset_feature_extractor_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/subset_feature_extractor_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/video_info_ui.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/video_info_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/user_defined_pose_creator.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/user_defined_pose_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/create_project_ui.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/create_project_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/tkinter_functions.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/ui/machine_model_settings_ui.py` & `Simba-UW-tf-dev-1.64.2/simba/ui/machine_model_settings_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/blob_storage/.DS_Store` & `Simba-UW-tf-dev-1.64.2/simba/blob_storage/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/labelling/.DS_Store` & `Simba-UW-tf-dev-1.64.2/simba/labelling/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/labelling/labelling_interface_old.py` & `Simba-UW-tf-dev-1.64.2/simba/labelling/labelling_interface_old.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/labelling/labelling_interface.py` & `Simba-UW-tf-dev-1.64.2/simba/labelling/labelling_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/labelling/extract_labelled_frames.py` & `Simba-UW-tf-dev-1.64.2/simba/labelling/extract_labelled_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/labelling/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.64.2/simba/labelling/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/labelling/play_annotation_video.py` & `Simba-UW-tf-dev-1.64.2/simba/labelling/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.64.2/simba/unsupervised/dbcv_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.64.2/simba/unsupervised/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.64.2/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.64.2/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.64.2/simba/unsupervised/grid_search_visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.64.2/simba/unsupervised/data_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/unsupervised/ui.py` & `Simba-UW-tf-dev-1.64.2/simba/unsupervised/ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.64.2/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/unsupervised/pop_up_classes.py` & `Simba-UW-tf-dev-1.64.2/simba/unsupervised/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.64.2/simba/unsupervised/bout_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/unsupervised/cluster_statistics.py` & `Simba-UW-tf-dev-1.64.2/simba/unsupervised/cluster_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.64.2/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.64.2/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.64.2/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/unsupervised/cluster_visualizer.py` & `Simba-UW-tf-dev-1.64.2/simba/unsupervised/cluster_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/bounding_box_tools/.DS_Store` & `Simba-UW-tf-dev-1.64.2/simba/bounding_box_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.64.2/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.64.2/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.64.2/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/bounding_box_tools/find_boundaries.py` & `Simba-UW-tf-dev-1.64.2/simba/bounding_box_tools/find_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.64.2/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/.DS_Store` & `Simba-UW-tf-dev-1.64.2/simba/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.64.2/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.64.2/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/peaks.py` & `Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/.DS_Store` & `Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/shap_log_mp_2.py` & `Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/shap_log_mp_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/shap_log_mp.py` & `Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/shap_log_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py` & `Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/read_files_mp_2.py` & `Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/read_files_mp_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.64.2/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.64.2/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.64.2/simba/feature_extractors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.64.2/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.64.2/simba/feature_extractors/feature_subsets.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.64.2/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.64.2/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/feature_extractors/feature_extractor_9bp.py` & `Simba-UW-tf-dev-1.64.2/simba/feature_extractors/feature_extractor_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.64.2/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.64.2/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/feature_extractors/.idea/features_scripts.iml` & `Simba-UW-tf-dev-1.64.2/simba/feature_extractors/.idea/features_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.64.2/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/feature_extractors/.idea/workspace.xml` & `Simba-UW-tf-dev-1.64.2/simba/feature_extractors/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/requirements.txt` & `Simba-UW-tf-dev-1.64.2/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.64.2/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.64.2/simba/mixins/pop_up_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.64.2/simba/mixins/config_reader.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/mixins/pose_importer_mixin.py` & `Simba-UW-tf-dev-1.64.2/simba/mixins/pose_importer_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/mixins/video_processing_mixin.py` & `Simba-UW-tf-dev-1.64.2/simba/mixins/video_processing_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi` & `Simba-UW-tf-dev-1.64.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi` & `Simba-UW-tf-dev-1.64.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi` & `Simba-UW-tf-dev-1.64.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc` & `Simba-UW-tf-dev-1.64.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc` & `Simba-UW-tf-dev-1.64.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc` & `Simba-UW-tf-dev-1.64.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc` & `Simba-UW-tf-dev-1.64.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.64.2/simba/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.64.2/simba/mixins/plotting_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.64.2/simba/mixins/unsupervised_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/mixins/train_model_mixin.py` & `Simba-UW-tf-dev-1.64.2/simba/mixins/train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.64.2/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.64.2/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.64.2/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/third_party_label_appenders/.DS_Store` & `Simba-UW-tf-dev-1.64.2/simba/third_party_label_appenders/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.64.2/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.64.2/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.64.2/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.64.2/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.64.2/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/cue_light_tools/.DS_Store` & `Simba-UW-tf-dev-1.64.2/simba/cue_light_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.64.2/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.64.2/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.64.2/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.64.2/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.64.2/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.64.2/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/utils/config_creator.py` & `Simba-UW-tf-dev-1.64.2/simba/utils/config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/utils/enums.py` & `Simba-UW-tf-dev-1.64.2/simba/utils/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.64.2/simba/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.64.2/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/utils/checks.py` & `Simba-UW-tf-dev-1.64.2/simba/utils/checks.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 """
 @authors: Xiaoyu Tong, Jia Jie Choong, Simon Nilsson
 """
 import os
 import trafaret as t
 import pandas as pd
 from typing import Any, Optional, Tuple, List, Union
+import subprocess
 
 from simba.utils.errors import (NoFilesFoundError,
                                 CorruptedFileError,
                                 IntegerError,
                                 FloatError,
                                 StringError,
                                 NotDirectoryError,
@@ -246,8 +247,17 @@
 
     for win in range(len(roll_windows_values)):
         if minimum_fps < roll_windows_values[win]:
             roll_windows_values[win] = minimum_fps
         else:
             pass
     roll_windows_values = list(set(roll_windows_values))
-    return roll_windows_values
+    return roll_windows_values
+
+
+def check_nvidea_gpu_available() -> bool:
+    """ Helper to check of NVIDEA GPU is available"""
+    try:
+        subprocess.check_output('nvidia-smi')
+        return True
+    except Exception:
+        return False
```

### Comparing `Simba-UW-tf-dev-1.64.1/simba/utils/read_write.py` & `Simba-UW-tf-dev-1.64.2/simba/utils/read_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -336,15 +336,16 @@
 def remove_a_folder(folder_dir: Union[str, os.PathLike]) -> None:
     """Helper to remove a directory"""
     shutil.rmtree(folder_dir, ignore_errors=True)
 
 def concatenate_videos_in_folder(in_folder: str,
                                  save_path: str,
                                  video_format: Optional[str] = 'mp4',
-                                 remove_splits: Optional[bool] = True) -> None:
+                                 remove_splits: Optional[bool] = True,
+                                 gpu: Optional[bool] = False) -> None:
     """
     Concatenate (temporally) all video files in a folder into a
     single video.
 
     .. important::
        Input video parts have to have sequential numerical ordered file names, e.g., ``1.mp4``, ``2.mp4`` ...
 
@@ -361,16 +362,18 @@
                                         in_folder))
     files.sort(key=lambda f: int(re.sub('\D', '', f)))
     temp_txt_path = Path(in_folder, 'files.txt')
     with open(temp_txt_path, 'w') as f:
         for file in files:
             f.write("file '" + str(Path(file)) + "'\n")
     if os.path.exists(save_path): os.remove(save_path)
-    returned = os.system(
-        'ffmpeg -f concat -safe 0 -i "{}" "{}" -c copy -hide_banner -loglevel info'.format(temp_txt_path, save_path))
+    if gpu:
+        returned = os.system('ffmpeg -hwaccel auto -c:v h264_cuvid -f concat -safe 0 -i "{}" -c copy -hide_banner -loglevel info "{}"'.format(temp_txt_path, save_path))
+    else:
+        returned = os.system('ffmpeg -f concat -safe 0 -i "{}" "{}" -c copy -hide_banner -loglevel info'.format(temp_txt_path, save_path))
     while True:
         if returned != 0:
             pass
         else:
             if remove_splits:
                 remove_a_folder(folder_dir=in_folder)
             break
```

### Comparing `Simba-UW-tf-dev-1.64.1/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.64.2/simba/utils/lookups.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/utils/cli/cli_tools.py` & `Simba-UW-tf-dev-1.64.2/simba/utils/cli/cli_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/utils/errors.py` & `Simba-UW-tf-dev-1.64.2/simba/utils/errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -299,11 +299,11 @@
                 f'Please make sure you imported the same video as you annotated in BORIS into SimBA and the video is registered with the correct frame rate.')
         else:
             msg = f'SIMBA THIRD-PARTY ANNOTATION WARNING: The annotations for video {video_name} contain data for {str(annotation_frms)} frames. The pose-estimation features for the same video contain data for {str(frm_cnt)} frames.'
 
         super().__init__(msg=msg, show_window=show_window)
         self.print_msg(msg=msg)
 
-class FFMPEGCodecError(SimbaError):
+class FFMPEGCodecGPUError(SimbaError):
     def __init__(self, msg: str, show_window: bool = False):
         super().__init__(msg=msg, show_window=show_window)
         self.print_msg(msg=f'SIMBA FFMPEG CODEC ERROR: {msg}')
```

### Comparing `Simba-UW-tf-dev-1.64.1/simba/utils/data.py` & `Simba-UW-tf-dev-1.64.2/simba/utils/data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/utils/printing.py` & `Simba-UW-tf-dev-1.64.2/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/st/select_groups_pg.py` & `Simba-UW-tf-dev-1.64.2/simba/st/select_groups_pg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/st/aggregate_statistics.py` & `Simba-UW-tf-dev-1.64.2/simba/st/aggregate_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/st/app.py` & `Simba-UW-tf-dev-1.64.2/simba/st/app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_processors/reorganize_keypoint.py` & `Simba-UW-tf-dev-1.64.2/simba/pose_processors/reorganize_keypoint.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_processors/remove_keypoints.py` & `Simba-UW-tf-dev-1.64.2/simba/pose_processors/remove_keypoints.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_processors/.DS_Store` & `Simba-UW-tf-dev-1.64.2/simba/pose_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_processors/pose_reset.py` & `Simba-UW-tf-dev-1.64.2/simba/pose_processors/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_processors/reverse_pose.py` & `Simba-UW-tf-dev-1.64.2/simba/pose_processors/reverse_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.64.2/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.64.2/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.64.2/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/plotting/.DS_Store` & `Simba-UW-tf-dev-1.64.2/simba/plotting/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.64.2/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.64.2/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.64.2/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.64.2/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.64.2/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.64.2/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.64.2/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.64.2/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.64.2/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.64.2/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.64.2/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.64.2/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/plotting/pose_plotter_mp.py` & `Simba-UW-tf-dev-1.64.2/simba/plotting/pose_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/plotting/Directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.64.2/simba/plotting/Directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.64.2/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.64.2/simba/plotting/path_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.64.2/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.64.2/simba/plotting/data_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.64.2/simba/plotting/path_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.64.2/simba/plotting/ez_lineplot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.64.2/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.64.2/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.64.2/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.64.2/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.64.2/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/plotting/Directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.64.2/simba/plotting/Directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.64.2/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/dash_app/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.64.2/simba/dash_app/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/dash_app/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.64.2/simba/dash_app/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/dash_app/dash_app.py` & `Simba-UW-tf-dev-1.64.2/simba/dash_app/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/data_processors/agg_clf_calculator.py` & `Simba-UW-tf-dev-1.64.2/simba/data_processors/agg_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/data_processors/.DS_Store` & `Simba-UW-tf-dev-1.64.2/simba/data_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/data_processors/severity_bout_based_calculator.py` & `Simba-UW-tf-dev-1.64.2/simba/data_processors/severity_bout_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/data_processors/interpolation_smoothing.py` & `Simba-UW-tf-dev-1.64.2/simba/data_processors/interpolation_smoothing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/data_processors/timebins_clf_calculator.py` & `Simba-UW-tf-dev-1.64.2/simba/data_processors/timebins_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/data_processors/fsttc_calculator.py` & `Simba-UW-tf-dev-1.64.2/simba/data_processors/fsttc_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/data_processors/interpolate_pose.py` & `Simba-UW-tf-dev-1.64.2/simba/data_processors/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/data_processors/directing_other_animals_calculator.py` & `Simba-UW-tf-dev-1.64.2/simba/data_processors/directing_other_animals_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/data_processors/timebins_movement_calculator.py` & `Simba-UW-tf-dev-1.64.2/simba/data_processors/timebins_movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/data_processors/severity_calculator.py` & `Simba-UW-tf-dev-1.64.2/simba/data_processors/severity_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/data_processors/pup_retrieval_calculator.py` & `Simba-UW-tf-dev-1.64.2/simba/data_processors/pup_retrieval_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/data_processors/pybursts_calculator.py` & `Simba-UW-tf-dev-1.64.2/simba/data_processors/pybursts_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/data_processors/severity_frame_based_calculator.py` & `Simba-UW-tf-dev-1.64.2/simba/data_processors/severity_frame_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/data_processors/mutual_exclusivity_corrector.py` & `Simba-UW-tf-dev-1.64.2/simba/data_processors/mutual_exclusivity_corrector.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/data_processors/kleinberg_calculator.py` & `Simba-UW-tf-dev-1.64.2/simba/data_processors/kleinberg_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/data_processors/movement_calculator.py` & `Simba-UW-tf-dev-1.64.2/simba/data_processors/movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store` & `Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store` & `Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png` & `Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png` & `Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png` & `Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png` & `Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png` & `Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png` & `Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png` & `Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png` & `Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png` & `Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png` & `Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png` & `Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png` & `Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png` & `Simba-UW-tf-dev-1.64.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/model/train_rf.py` & `Simba-UW-tf-dev-1.64.2/simba/model/train_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/model/.DS_Store` & `Simba-UW-tf-dev-1.64.2/simba/model/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/model/inference_batch.py` & `Simba-UW-tf-dev-1.64.2/simba/model/inference_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/model/grid_search_rf.py` & `Simba-UW-tf-dev-1.64.2/simba/model/grid_search_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/model/inference_validation.py` & `Simba-UW-tf-dev-1.64.2/simba/model/inference_validation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.64.2/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.64.2/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.64.2/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.64.2/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.64.2/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.64.2/simba/roi_tools/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.64.2/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.64.2/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.64.2/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.64.2/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.64.2/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.64.2/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.64.2/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.64.2/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.64.2/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_importers/sleap_csv_importer.py` & `Simba-UW-tf-dev-1.64.2/simba/pose_importers/sleap_csv_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_importers/misc/.DS_Store` & `Simba-UW-tf-dev-1.64.2/simba/pose_importers/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_importers/misc/apt_trk_importer.py` & `Simba-UW-tf-dev-1.64.2/simba/pose_importers/misc/apt_trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.64.2/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_importers/.DS_Store` & `Simba-UW-tf-dev-1.64.2/simba/pose_importers/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_importers/sleap_h5_importer.py` & `Simba-UW-tf-dev-1.64.2/simba/pose_importers/sleap_h5_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_importers/madlc_importer.py` & `Simba-UW-tf-dev-1.64.2/simba/pose_importers/madlc_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_importers/sleap_slp_importer.py` & `Simba-UW-tf-dev-1.64.2/simba/pose_importers/sleap_slp_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.64.2/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.64.2/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.64.2/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.64.2/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_configurations/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.64.2/simba/pose_configurations/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.64.2/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_configurations/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.64.2/simba/pose_configurations/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_configurations/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.64.2/simba/pose_configurations/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.64.2/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.64.2/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.64.2/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.64.2/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.64.2/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.64.2/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.64.2/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.64.2/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.64.2/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.64.2/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.64.2/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.64.2/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/three_dimensions/ui/define_px_to_mm_ui.py` & `Simba-UW-tf-dev-1.64.2/simba/three_dimensions/ui/define_px_to_mm_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/three_dimensions/feature_extractors/generic_feature_extractor.py` & `Simba-UW-tf-dev-1.64.2/simba/three_dimensions/feature_extractors/generic_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/three_dimensions/mixins/config_reader.py` & `Simba-UW-tf-dev-1.64.2/simba/three_dimensions/mixins/config_reader.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.1.nbc` & `Simba-UW-tf-dev-1.64.2/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.1.nbc` & `Simba-UW-tf-dev-1.64.2/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.nbi` & `Simba-UW-tf-dev-1.64.2/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.nbi` & `Simba-UW-tf-dev-1.64.2/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/three_dimensions/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.64.2/simba/three_dimensions/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/three_dimensions/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.64.2/simba/three_dimensions/mixins/plotting_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/three_dimensions/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.64.2/simba/three_dimensions/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/three_dimensions/pose_importers/anipose_csv_import.py` & `Simba-UW-tf-dev-1.64.2/simba/three_dimensions/pose_importers/anipose_csv_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/three_dimensions/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.64.2/simba/three_dimensions/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/video_processors/video_processing.py` & `Simba-UW-tf-dev-1.64.2/simba/video_processors/video_processing.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,15 +12,18 @@
 from tkinter import *
 from datetime import datetime
 import time
 from PIL import Image, ImageTk
 import multiprocessing
 from typing import List, Union, Optional
 
-from simba.utils.checks import (check_file_exist_and_readable, check_int, check_if_filepath_list_is_empty)
+from simba.utils.checks import (check_file_exist_and_readable,
+                                check_int,
+                                check_if_filepath_list_is_empty,
+                                check_nvidea_gpu_available)
 from simba.utils.read_write import (get_fn_ext,
                                     get_video_meta_data,
                                     find_all_videos_in_directory,
                                     find_core_cnt,
                                     read_config_entry,
                                     read_config_file)
 from simba.utils.printing import stdout_success, SimbaTimer
@@ -29,15 +32,16 @@
 
 from simba.utils.errors import (NotDirectoryError,
                                 NoFilesFoundError,
                                 FileExistError,
                                 CountError,
                                 InvalidInputError,
                                 DirectoryExistError,
-                                FFMPEGCodecError)
+                                FFMPEGCodecGPUError,
+                                InvalidFileTypeError)
 from simba.utils.warnings import (SameInputAndOutputWarning,
                                   FileExistWarning)
 
 
 MAX_FRM_SIZE = 1080, 650
 
 def change_img_format(directory: Union[str, os.PathLike],
@@ -138,52 +142,62 @@
         frm_save_path = os.path.join(save_dir, '{}.{}'.format(str(frm_number), 'png'))
         cv2.imwrite(frm_save_path,frame)
         print('Frame {} saved (Frame {}/{})'.format(str(frm_number), str(frm_cnt), str(len(frame_range))))
     stdout_success(msg=f'{str(len(frame_range))} frames extracted for video {file_name}')
 
 
 def change_single_video_fps(file_path: Union[str, os.PathLike],
-                            fps: int) -> None:
+                            fps: int,
+                            gpu: Optional[bool] = False) -> None:
     """
     Change the fps of a single video file. Results are stored in the same directory as in the input file with
     the suffix ``_fps_new_fps``.
 
     :parameter Union[str, os.PathLike] file_path: Path to video file
     :parameter int fps: Fps of the new video file.
+    :parameter Optional[bool] gpu: If True, use NVIDEA GPU codecs. Default False.
 
     :example:
     >>> _ = change_single_video_fps(file_path='project_folder/videos/Video_1.mp4', fps=15)
     """
 
+    if gpu and not check_nvidea_gpu_available():
+        raise FFMPEGCodecGPUError(msg='No GPU found (as evaluated by nvidea-smi returning None)')
     check_file_exist_and_readable(file_path=file_path)
     check_int(name='New fps', value=fps)
     video_meta_data = get_video_meta_data(video_path=file_path)
     dir_name, file_name, ext = get_fn_ext(filepath=file_path)
     if int(fps) == int(video_meta_data['fps']):
         SameInputAndOutputWarning(msg=f'The new fps is the same as the input fps for video {file_name} ({str(fps)})')
     save_path = os.path.join(dir_name, file_name + '_fps_{}{}'.format(str(fps), str(ext)))
     if os.path.isfile(save_path):
         FileExistWarning(msg=f'Overwriting existing file at {save_path}')
+    if gpu:
+        command = f'ffmpeg -hwaccel auto -c:v h264_cuvid -i "{file_path}" -vf "fps={fps}" -c:v h264_nvenc -c:a copy "{save_path}"'
+    else:
         command = str('ffmpeg -i ') + '"' + str(file_path) + '"' + ' -filter:v fps=fps=' + str(fps) + ' ' + '"' + save_path + '"'
     subprocess.call(command, shell=True)
     stdout_success(msg=f'SIMBA COMPLETE: FPS of video {file_name} changed from {str(video_meta_data["fps"])} to {str(fps)} and saved in directory {save_path}')
 
 def change_fps_of_multiple_videos(directory: Union[str, os.PathLike],
-                                  fps: int) -> None:
+                                  fps: int,
+                                  gpu: Optional[bool] = False) -> None:
     """
     Change the fps of all video files in a folder. Results are stored in the same directory as in the input files with
     the suffix ``_fps_new_fps``.
 
     :parameter Union[str, os.PathLike] directory: Path to video file directory
     :parameter int fps: Fps of the new video files.
+    :parameter Optional[bool] gpu: If True, use NVIDEA GPU codecs. Default False.
 
     :example:
     >>> _ = change_fps_of_multiple_videos(directory='project_folder/videos/Video_1.mp4', fps=15)
     """
-
+    if gpu and not check_nvidea_gpu_available():
+        raise FFMPEGCodecGPUError(msg='No GPU found (as evaluated by nvidea-smi returning None)')
     if not os.path.isdir(directory):
         raise NotDirectoryError(msg='SIMBA ERROR: {} is not a valid directory'.format(directory))
     check_int(name='New fps', value=fps)
     video_paths = []
     file_paths_in_folder = [f for f in glob.glob(directory + '/*') if os.path.isfile(f)]
     for file_path in file_paths_in_folder:
         _, _, ext = get_fn_ext(filepath=file_path)
@@ -191,237 +205,316 @@
             video_paths.append(file_path)
     if len(video_paths) < 1:
         raise NoFilesFoundError(msg='SIMBA ERROR: No files with .mp4, .avi, .mov, .flv file ending found in the {} directory'.format(directory))
     for file_cnt, file_path in enumerate(video_paths):
         dir_name, file_name, ext = get_fn_ext(filepath=file_path)
         print('Converting FPS for {}...'.format(file_name))
         save_path = os.path.join(dir_name, file_name + '_fps_{}{}'.format(str(fps), str(ext)))
-        command = str('ffmpeg -i ') + str(file_path) + ' -filter:v fps=fps=' + str(fps) + ' ' + '"' + save_path + '"'
+        if gpu:
+            command = f'ffmpeg -hwaccel auto -c:v h264_cuvid -i "{file_path}" -vf "fps={fps}" -c:v h264_nvenc -c:a copy "{save_path}"'
+        else:
+            command = str('ffmpeg -i ') + str(file_path) + ' -filter:v fps=fps=' + str(fps) + ' ' + '"' + save_path + '"'
         subprocess.call(command, shell=True)
         print('Video {} complete...'.format(file_name))
     stdout_success(msg=f'SIMBA COMPLETE: FPS of {str(len(video_paths))} videos changed to { str(fps)}')
 
-def convert_video_powerpoint_compatible_format(file_path: Union[str, os.PathLike]) -> None:
+def convert_video_powerpoint_compatible_format(file_path: Union[str, os.PathLike],
+                                               gpu: Optional[bool] = False) -> None:
     """
     Create MS PowerPoint compatible copy of a video file. The result is stored in the same directory as the
     input file with the ``_powerpointready`` suffix.
 
     :parameter Union[str, os.PathLike] file_path: Path to video file.
+    :parameter Optional[bool] gpu: If True, use NVIDEA GPU codecs. Default False.
 
     :example:
     >>> _ = convert_video_powerpoint_compatible_format(file_path='project_folder/videos/Video_1.mp4')
     """
-
+    if gpu and not check_nvidea_gpu_available():
+        raise FFMPEGCodecGPUError(msg='No GPU found (as evaluated by nvidea-smi returning None)')
+    timer = SimbaTimer(start=True)
     check_file_exist_and_readable(file_path=file_path)
     dir, file_name, ext = get_fn_ext(filepath=file_path)
     save_name = os.path.join(dir, file_name + '_powerpointready.mp4')
     if os.path.isfile(save_name):
         raise FileExistError(msg='SIMBA ERROR: The outfile file already exist: {}.'.format(save_name))
-    command = (str('ffmpeg -i ') + '"' + str(file_path) + '"' + ' -c:v libx264 -preset slow  -profile:v high -level:v 4.0 -pix_fmt yuv420p -crf 22 -codec:a aac ' + '"' + save_name + '"')
+    if gpu:
+        command = 'ffmpeg -hwaccel auto -c:v h264_cuvid -i "{}" -c:v h264_nvenc -preset slow -profile:v high -level:v 4.0 -pix_fmt yuv420p -crf 22 -c:a aac "{}"'.format(file_path, save_name)
+    else:
+        command = (str('ffmpeg -i ') + '"' + str(file_path) + '"' + ' -c:v libx264 -preset slow  -profile:v high -level:v 4.0 -pix_fmt yuv420p -crf 22 -codec:a aac ' + '"' + save_name + '"')
     print('Creating video in powerpoint compatible format... ')
     subprocess.call(command, shell=True, stdout=subprocess.PIPE)
-    stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!')
+    timer.stop_timer()
+    stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!', elapsed_time=timer.elapsed_time_str)
 
-def convert_to_mp4(file_path: Union[str, os.PathLike]) -> None:
+def convert_to_mp4(file_path: Union[str, os.PathLike],
+                   gpu: Optional[bool] = False) -> None:
     """
     Convert a video file to mp4 format. The result is stored in the same directory as the
     input file with the ``_converted.mp4`` suffix.
 
     :parameter Union[str, os.PathLike] file_path: Path to video file.
+    :parameter Optional[bool] gpu: If True, use NVIDEA GPU codecs. Default False.
 
     :example:
     >>> _ = convert_to_mp4(file_path='project_folder/videos/Video_1.avi')
     """
 
+    timer = SimbaTimer(start=True)
+    if gpu and not check_nvidea_gpu_available():
+        raise FFMPEGCodecGPUError(msg='No GPU found (as evaluated by nvidea-smi returning None)')
     check_file_exist_and_readable(file_path=file_path)
     dir, file_name, ext = get_fn_ext(filepath=file_path)
     save_name = os.path.join(dir, file_name + '_converted.mp4')
     if os.path.isfile(save_name):
         raise FileExistError(msg='SIMBA ERROR: The outfile file already exist: {}.'.format(save_name))
-    command = (str('ffmpeg -i ') + '"' + str(file_path) + '"' + ' ' + '"' + save_name + '"')
+    if gpu:
+        command = 'ffmpeg -hwaccel auto -c:v h264_cuvid -i "{}" -c:v h264_nvenc "{}"'.format(file_path, save_name)
+    else:
+        command = (str('ffmpeg -i ') + '"' + str(file_path) + '"' + ' ' + '"' + save_name + '"')
     print('Converting to mp4... ')
     subprocess.call(command, shell=True, stdout=subprocess.PIPE)
-    stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!')
+    timer.stop_timer()
+    stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!', elapsed_time=timer.elapsed_time_str)
 
-def video_to_greyscale(file_path: Union[str, os.PathLike]) -> None:
+def video_to_greyscale(file_path: Union[str, os.PathLike],
+                       gpu: Optional[bool] = False) -> None:
     """
     Convert a video file to greyscale mp4 format. The result is stored in the same directory as the
     input file with the ``_grayscale.mp4`` suffix.
 
     :parameter Union[str, os.PathLike] file_path: Path to video file.
+    :parameter Optional[bool] gpu: If True, use NVIDEA GPU codecs. Default False.
 
     :example:
     >>> _ = video_to_greyscale(file_path='project_folder/videos/Video_1.avi')
     """
 
+    timer = SimbaTimer(start=True)
     check_file_exist_and_readable(file_path=file_path)
     dir, file_name, ext = get_fn_ext(filepath=file_path)
     save_name = os.path.join(dir, file_name + '_grayscale.mp4')
     if os.path.isfile(save_name):
         raise FileExistError(msg='SIMBA ERROR: The outfile file already exist: {}.'.format(save_name))
-    command = (str('ffmpeg -i ') + '"' + str(file_path) + '"' + ' -vf format=gray ' + '"' + save_name + '"')
+    if gpu:
+        if not check_nvidea_gpu_available():
+            raise FFMPEGCodecGPUError(msg='No GPU found (as evaluated by nvidea-smi returning None)')
+        command = f'ffmpeg -hwaccel auto -c:v h264_cuvid -i "{file_path}" -vf "hwdownload,format=nv12,format=gray" -c:v h264_nvenc -c:a copy "{save_name}"'
+    else:
+        command = (str('ffmpeg -i ') + '"' + str(file_path) + '"' + ' -vf format=gray ' + '"' + save_name + '"')
     print('Converting to greyscale... ')
     subprocess.call(command, shell=True, stdout=subprocess.PIPE)
-    stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!')
-
+    timer.stop_timer()
+    stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!', elapsed_time=timer.elapsed_time_str)
 
-def superimpose_frame_count(file_path: Union[str, os.PathLike]) -> None:
+def superimpose_frame_count(file_path: Union[str, os.PathLike],
+                            gpu: Optional[bool] = False) -> None:
     """
     Superimpose frame count on a video file. The result is stored in the same directory as the
     input file with the ``_frame_no.mp4`` suffix.
 
     :parameter Union[str, os.PathLike] file_path: Path to video file.
+    :parameter Optional[bool] gpu: If True, use NVIDEA GPU codecs. Default False.
 
     :example:
     >>> _ = superimpose_frame_count(file_path='project_folder/videos/Video_1.avi')
     """
 
-
+    timer = SimbaTimer(start=True)
     check_file_exist_and_readable(file_path=file_path)
     dir, file_name, ext = get_fn_ext(filepath=file_path)
     save_name = os.path.join(dir, file_name + '_frame_no.mp4')
     print('Superimposing frame numbers...... ')
     try:
-        command = (str('ffmpeg -y -i ') + '"' + file_path + '"' + ' -vf "drawtext=fontfile=Arial.ttf: text=\'%{frame_num}\': start_number=0: x=(w-tw)/2: y=h-(2*lh): fontcolor=black: fontsize=20: box=1: boxcolor=white: boxborderw=5" -c:a copy ' + '"' + save_name + '"')
+        if gpu:
+            if not check_nvidea_gpu_available():
+                raise FFMPEGCodecGPUError(msg='No GPU found (as evaluated by nvidea-smi returning None)')
+            command = f'ffmpeg -hwaccel auto -c:v h264_cuvid -i "{file_path}" -vf "drawtext=fontfile=Arial.ttf:text=\'%%{{n}}\':x=(w-tw)/2:y=h-th-10*ph:fontcolor=white:fontsize=ih/20:box=1:boxcolor=black@0.5" -c:v h264_nvenc -c:a copy "{save_name}"'
+        else:
+            command = (str('ffmpeg -y -i ') + '"' + file_path + '"' + ' -vf "drawtext=fontfile=Arial.ttf: text=\'%{frame_num}\': start_number=0: x=(w-tw)/2: y=h-(2*lh): fontcolor=black: fontsize=20: box=1: boxcolor=white: boxborderw=5" -c:a copy ' + '"' + save_name + '"')
         subprocess.check_output(command, shell=True)
         subprocess.call(command, shell=True, stdout=subprocess.PIPE)
     except subprocess.CalledProcessError as e:
         simba_cw = os.path.dirname(simba.__file__)
         simba_font_path = Path(simba_cw, 'assets', 'UbuntuMono-Regular.ttf')
-        command = 'ffmpeg -y -i ' + file_path + ' -vf "drawtext=fontfile={}:'.format(simba_font_path) + "text='%{frame_num}': start_number=1: x=(w-tw)/2: y=h-(2*lh): fontcolor=black: fontsize=20: box=1: boxcolor=white: boxborderw=5" + '" ' + "-c:a copy " + save_name
+        if gpu:
+            if not check_nvidea_gpu_available():
+                raise FFMPEGCodecGPUError(msg='No GPU found (as evaluated by nvidea-smi returning None)')
+            command = f'ffmpeg -hwaccel auto -c:v h264_cuvid -i "{file_path}" -vf "drawtext=fontfile={simba_font_path}:text=\'%%{{n}}\':x=(w-tw)/2:y=h-th-10*ph:fontcolor=white:fontsize=ih/20:box=1:boxcolor=black@0.5" -c:v h264_nvenc -c:a copy "{save_name}"'
+        else:
+            command = 'ffmpeg -y -i ' + file_path + ' -vf "drawtext=fontfile={}:'.format(simba_font_path) + "text='%{frame_num}': start_number=1: x=(w-tw)/2: y=h-(2*lh): fontcolor=black: fontsize=20: box=1: boxcolor=white: boxborderw=5" + '" ' + "-c:a copy " + save_name
         subprocess.call(command, shell=True, stdout=subprocess.PIPE)
-    stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!')
+    timer.stop_timer()
+    stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!', elapsed_time=timer.elapsed_time_str)
 
 def remove_beginning_of_video(file_path: Union[str, os.PathLike],
-                              time: int) -> None:
+                              time: int,
+                              gpu: Optional[bool] = False) -> None:
     """
     Remove N seconds from the beginning of a video file. The result is stored in the same directory as the
     input file with the ``_shorten.mp4`` suffix.
 
     :parameter Union[str, os.PathLike] file_path: Path to video file
     :parameter int time: Number of seconds to remove from the beginning of the video.
+    :parameter Optional[bool] gpu: If True, use NVIDEA GPU codecs. Default False.
 
     :example:
     >>> _ = remove_beginning_of_video(file_path='project_folder/videos/Video_1.avi', time=10)
     """
 
+    timer = SimbaTimer(start=True)
     check_file_exist_and_readable(file_path=file_path)
     check_int(name='Cut time', value=time)
     dir, file_name, ext = get_fn_ext(filepath=file_path)
     save_name = os.path.join(dir, file_name + '_shorten.mp4')
     if os.path.isfile(save_name):
         raise FileExistError(msg='SIMBA ERROR: The outfile file already exist: {}.'.format(save_name))
-    command = (str('ffmpeg -ss ') + str(int(time)) + ' -i ' + '"' + str(file_path) + '"' + ' -c:v libx264 -c:a aac ' + '"' + save_name + '"')
+    if gpu:
+        if not check_nvidea_gpu_available():
+            raise FFMPEGCodecGPUError(msg='No GPU found (as evaluated by nvidea-smi returning None)')
+        command = 'ffmpeg -hwaccel cuvid -c:v h264_cuvid -ss {} -i "{}" -c:v h264_nvenc -c:a aac "{}"'.format(int(time), file_path, save_name)
+    else:
+        command = (str('ffmpeg -ss ') + str(int(time)) + ' -i ' + '"' + str(file_path) + '"' + ' -c:v libx264 -c:a aac ' + '"' + save_name + '"')
     print('Shortening video... ')
     subprocess.call(command, shell=True, stdout=subprocess.PIPE)
-    stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!')
+    timer.stop_timer()
+    stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!', elapsed_time=timer.elapsed_time_str)
 
 
 def clip_video_in_range(file_path: Union[str, os.PathLike],
                         start_time: str,
-                        end_time: str) -> None:
+                        end_time: str,
+                        gpu: Optional[bool] = False) -> None:
     """
     Clip video within a specific range. The result is stored in the same directory as the
     input file with the ``_clipped.mp4`` suffix.
 
     :parameter Union[str, os.PathLike] file_path: Path to video file
     :parameter str start_time: Start time in HH:MM:SS format.
     :parameter str end_time: End time in HH:MM:SS format.
+    :parameter Optional[bool] gpu: If True, use NVIDEA GPU codecs. Default False.
 
     :example:
     >>> _ = clip_video_in_range(file_path='project_folder/videos/Video_1.avi', start_time='00:00:05', end_time='00:00:10')
     """
 
+    timer = SimbaTimer(start=True)
     check_file_exist_and_readable(file_path=file_path)
     dir, file_name, ext = get_fn_ext(filepath=file_path)
     save_name = os.path.join(dir, file_name + '_clipped.mp4')
     if os.path.isfile(save_name):
         raise FileExistError(msg='SIMBA ERROR: The outfile file already exist: {}.'.format(save_name))
-    command = (str('ffmpeg -i ') + '"' + str(file_path) + '"' + ' -ss ' + str(start_time) + ' -to ' + str(end_time) + ' -async 1 ' + '"' + save_name + '"')
+    if gpu:
+        if not check_nvidea_gpu_available():
+            raise FFMPEGCodecGPUError(msg='No GPU found (as evaluated by nvidea-smi returning None)')
+        command = 'ffmpeg -hwaccel auto -c:v h264_cuvid -i "{}" -ss {} -to {} -async 1 "{}"'.format(file_path, start_time, end_time, save_name)
+    else:
+        command = (str('ffmpeg -i ') + '"' + str(file_path) + '"' + ' -ss ' + str(start_time) + ' -to ' + str(end_time) + ' -async 1 ' + '"' + save_name + '"')
     print('Clipping video... ')
     subprocess.call(command, shell=True, stdout=subprocess.PIPE)
-    stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!')
+    timer.stop_timer()
+    stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!', elapsed_time=timer.elapsed_time_str)
 
 def downsample_video(file_path: Union[str, os.PathLike],
                      video_height: int,
-                     video_width: int) -> None:
+                     video_width: int,
+                     gpu: Optional[bool] = False) -> None:
     """
     Down-sample a video file. The result is stored in the same directory as the
     input file with the ``_downsampled.mp4`` suffix.
 
     :parameter Union[str, os.PathLike] file_path: Path to video file.
     :parameter int video_height: height of new video.
     :parameter int video_width: width of new video.
+    :parameter Optional[bool] gpu: If True, use NVIDEA GPU codecs. Default False.
 
     :example:
     >>> _ = downsample_video(file_path='project_folder/videos/Video_1.avi', video_height=600, video_width=400)
     """
 
+    timer = SimbaTimer(start=True)
     check_int(name='Video height', value=video_height)
     check_int(name='Video width', value=video_width)
     check_file_exist_and_readable(file_path=file_path)
     dir, file_name, ext = get_fn_ext(filepath=file_path)
     save_name = os.path.join(dir, file_name + '_downsampled.mp4')
     if os.path.isfile(save_name):
         raise FileExistError('SIMBA ERROR: The outfile file already exist: {}.'.format(save_name))
-    command = (str('ffmpeg -i ') + '"' + str(file_path) + '"' + ' -vf scale=' + str(video_width) + ':' + str(video_height) + ' ' + '"' + save_name + '"' + ' -hide_banner')
+    if gpu:
+        if not check_nvidea_gpu_available():
+            raise FFMPEGCodecGPUError(msg='No GPU found (as evaluated by nvidea-smi returning None)')
+        command = f'ffmpeg -y -hwaccel auto -c:v h264_cuvid -i "{file_path}" -vf "scale=w={video_width}:h={video_height}:force_original_aspect_ratio=decrease:flags=bicubic" -c:v h264_nvenc "{save_name}"'
+    else:
+        command = (str('ffmpeg -i ') + '"' + str(file_path) + '"' + ' -vf scale=' + str(video_width) + ':' + str(video_height) + ' ' + '"' + save_name + '"' + ' -hide_banner')
     print('Down-sampling video... ')
     subprocess.call(command, shell=True, stdout=subprocess.PIPE)
-    stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!')
+    timer.stop_timer()
+    stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!', elapsed_time=timer.elapsed_time_str)
 
 def gif_creator(file_path: str,
                 start_time: int,
                 duration: int,
-                width: int) -> None:
+                width: int,
+                gpu: Optional[bool] = False) -> None:
     """
     Create a sample gif from a video file. The result is stored in the same directory as the
     input file with the ``.gif`` file-ending.
 
     .. note::
        The height is auto-computed to retain aspect ratio
 
     :parameter Union[str, os.PathLike] file_path: Path to video file.
     :parameter int start_time: Start time of the gif in relation to the video in seconds.
     :parameter int duration: Duration of the gif.
     :parameter int width: Width of the gif.
+    :parameter Optional[bool] gpu: If True, use NVIDEA GPU codecs. Default False.
 
     :example:
     >>> _ = gif_creator(file_path='project_folder/videos/Video_1.avi', start_time=5, duration=10, width=600)
     """
 
     check_file_exist_and_readable(file_path=file_path)
     check_int(name='Start time', value=start_time)
     check_int(name='Duration', value=duration)
     check_int(name='Width', value=width)
     _ = get_video_meta_data(file_path)
     dir, file_name, ext = get_fn_ext(filepath=file_path)
     save_name = os.path.join(dir, file_name + '.gif')
     if os.path.isfile(save_name):
         raise FileExistError('SIMBA ERROR: The outfile file already exist: {}.'.format(save_name))
-    command = 'ffmpeg -ss ' + str(start_time) + ' -t ' + str(duration) + ' -i ' + '"' + str(file_path) + '"' + ' -filter_complex "[0:v] fps=15,scale=w=' + str(width) + ':h=-1,split [a][b];[a] palettegen=stats_mode=single [p];[b][p] paletteuse=new=1" ' + '"' + str(save_name) + '"'
+    if gpu:
+        if not check_nvidea_gpu_available():
+            raise FFMPEGCodecGPUError(msg='NVIDEA GPU not available (as evaluated by nvidea-smi returning None')
+        command = f'ffmpeg -hwaccel auto -c:v h264_cuvid -ss {start_time} -i "{file_path}" -to {duration} -vf "fps=15,scale=width:-1" -c:v h264_nvenc -pix_fmt yuv420p "{save_name}"'
+    else:
+        command = 'ffmpeg -ss ' + str(start_time) + ' -t ' + str(duration) + ' -i ' + '"' + str(file_path) + '"' + ' -filter_complex "[0:v] fps=15,scale=w=' + str(width) + ':h=-1,split [a][b];[a] palettegen=stats_mode=single [p];[b][p] paletteuse=new=1" ' + '"' + str(save_name) + '"'
     print('Creating gif sample... ')
     subprocess.call(command, shell=True, stdout=subprocess.PIPE)
     stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!')
 
 
 def batch_convert_video_format(directory: Union[str, os.PathLike],
                                input_format: str,
-                               output_format: str) -> None:
+                               output_format: str,
+                               gpu: Optional[bool] = False) -> None:
     """
     Batch convert all videos in a folder of specific format into a different video format. The results are
     stored in the same directory as the input files.
 
     :parameter Union[str, os.PathLike] directory: Path to video file directory.
     :parameter str input_format: Format of the input files (e.g., avi).
     :parameter str output_format: Format of the output files (e.g., mp4).
+    :parameter Optional[bool] gpu: If True, use NVIDEA GPU codecs. Default False.
 
     :example:
     >>> _ = batch_convert_video_format(directory='project_folder/videos', input_format='avi', output_format='mp4')
     """
 
+    if input_format == output_format:
+        raise InvalidFileTypeError(msg=f'The input format ({input_format}) is the same as the output format ({output_format})')
     if not os.path.isdir(directory):
         raise NotDirectoryError(msg='SIMBA ERROR: {} is not a valid directory'.format(directory))
     video_paths = []
     file_paths_in_folder = [f for f in glob.glob(directory + '/*') if os.path.isfile(f)]
     for file_path in file_paths_in_folder:
         _, _, ext = get_fn_ext(filepath=file_path)
         if ext.lower() == '.{}'.format(input_format.lower()):
@@ -430,15 +523,20 @@
         raise NoFilesFoundError(msg='SIMBA ERROR: No files with .{} file ending found in the {} directory'.format(input_format, directory))
     for file_cnt, file_path in enumerate(video_paths):
         dir_name, file_name, ext = get_fn_ext(filepath=file_path)
         print('Processing video {}...'.format(file_name))
         save_path = os.path.join(dir_name, file_name + '.{}'.format(output_format.lower()))
         if os.path.isfile(save_path):
             raise FileExistError(msg='SIMBA ERROR: The outfile file already exist: {}.'.format(save_path))
-        command = 'ffmpeg -y -i ' + '"' + file_path + '"' + ' -c:v libx264 -crf 5 -preset medium -c:a libmp3lame -b:a 320k '+'"' + save_path + '"'
+        if gpu:
+            if not check_nvidea_gpu_available():
+                raise FFMPEGCodecGPUError(msg='NVIDEA GPU not available (as evaluated by nvidea-smi returning None')
+            command = 'ffmpeg -hwaccel auto -c:v h264_cuvid -i "{}" -c:v h264_nvenc -cq 23 -preset:v medium -c:a copy "{}"'.format(file_path, save_path)
+        else:
+            command = 'ffmpeg -y -i ' + '"' + file_path + '"' + ' -c:v libx264 -crf 5 -preset medium -c:a libmp3lame -b:a 320k '+'"' + save_path + '"'
         subprocess.call(command, shell=True, stdout=subprocess.PIPE)
         print('Video {} complete, (Video {}/{})...'.format(file_name, str(file_cnt+1), str(len(video_paths))))
 
     stdout_success(msg=f'SIMBA COMPLETE: {str(len(video_paths))} videos converted in {directory} directory!')
 
 def batch_create_frames(directory: Union[str, os.PathLike]) -> None:
     """
@@ -496,19 +594,21 @@
                       gpu: Optional[bool] = False) -> None:
     """
     Divide a video file into multiple video files from specified start and stop times.
 
     :parameter str file_path: Path to input video file.
     :parameter List[str] start_times: Start times in HH:MM:SS format.
     :parameter List[str] end_times: End times in HH:MM:SS format.
+    :parameter Optional[bool] gpu: If True, use NVIDEA GPU codecs. Default False.
 
     :example:
     >>> _ = multi_split_video(file_path='project_folder/videos/Video_1.mp4', start_times=['00:00:05', '00:00:20'], end_times=['00:00:10', '00:00:25'])
     """
 
+    timer = SimbaTimer(start=True)
     check_file_exist_and_readable(file_path=file_path)
     video_meta_data = get_video_meta_data(file_path)
     dir_name, file_name, ext = get_fn_ext(filepath=file_path)
     r = re.compile('.{2}:.{2}:.{2}')
     for start_time_cnt, start_time in enumerate(start_times):
         if (len(start_time) != 8) or (not r.match(start_time)) or (re.search('[a-zA-Z]', start_time)):
             raise InvalidInputError(msg=f'Start time for clip {str(start_time_cnt+1)} is should be in the format XX:XX:XX where X is an integer between 0-9')
@@ -526,27 +626,32 @@
             raise InvalidInputError(msg=f'Clip {str(clip_cnt+1)} has the same start time and end time.')
         if end_in_s > video_meta_data['video_length_s']:
             raise InvalidInputError(f'Clip {str(clip_cnt + 1)} has end time at {str(end_in_s)} seconds into the video, which is greater then the lenth of the video ({str(video_meta_data["video_length_s"])}s).')
         save_path = os.path.join(dir_name, file_name + '_{}'.format(str(clip_cnt+1)) + '.mp4')
         if os.path.isfile(save_path):
             raise FileExistError(msg=f'The outfile file already exist: {save_path}.')
         if gpu:
+            if not check_nvidea_gpu_available():
+                raise FFMPEGCodecGPUError(msg='NVIDEA GPU not available (as evaluated by nvidea-smi returning None')
             command = 'ffmpeg -hwaccel auto -i "{}" -ss {} -to {} -c:v h264_nvenc -async 1 "{}"'.format(file_path, start_time, end_time, save_path)
         else:
             command = (str('ffmpeg -i ') + '"' + file_path + '"' + ' -ss ' + start_time + ' -to ' + end_time + ' -async 1 ' + '"' + save_path + '"')
         print('Processing video clip {}...'.format(str(clip_cnt+1)))
         subprocess.call(command, shell=True, stdout=subprocess.PIPE)
-    stdout_success(msg=f'Video {file_name} converted into {str(len(start_times))} clips in directory {dir_name}!')
+    timer.stop_timer()
+    stdout_success(msg=f'Video {file_name} converted into {str(len(start_times))} clips in directory {dir_name}!', elapsed_time=timer.elapsed_time_str)
 
-def crop_single_video(file_path: Union[str, os.PathLike]) -> None:
+def crop_single_video(file_path: Union[str, os.PathLike],
+                      gpu: Optional[bool] = False) -> None:
     """
     Crop a single video using cv2.selectROI interface. Results is saved in the same directory as input video with the
     ``_cropped.mp4`` suffix`.
 
     :parameter str file_path: Path to video file.
+    :parameter Optional[bool] gpu: If True, use NVIDEA GPU codecs. Default False.
 
     :example:
     >>> _ = crop_single_video(file_path='project_folder/videos/Video_1.mp4')
     """
 
     check_file_exist_and_readable(file_path=file_path)
     _ = get_video_meta_data(video_path=file_path)
@@ -562,30 +667,41 @@
     cv2.waitKey(0)
     cv2.destroyAllWindows()
     if (width == 0 and height == 0) or (width + height + top_lext_x + top_left_y == 0):
         raise CountError(msg='CROP FAILED: Cropping height and width are both 0. Please try again.')
     save_path = os.path.join(dir_name, file_name + '_cropped.mp4')
     if os.path.isfile(save_path):
         raise FileExistError(msg='SIMBA ERROR: The out file file already exist: {}.'.format(save_path))
-    command = str('ffmpeg -y -i ') + '"' + str(file_path) + '"' + str(' -vf ') + str('"crop=') + str(width) + ':' + str(height) + ':' + str(top_lext_x) + ':' + str(top_left_y) + '" ' + str('-c:v libx264 -crf 21 -c:a copy ') + '"' + str(save_path) + '"'
+    timer = SimbaTimer(start=True)
+    if gpu:
+        if not check_nvidea_gpu_available():
+            raise FFMPEGCodecGPUError(msg='NVIDEA GPU not available (as evaluated by nvidea-smi returning None')
+        command = f'ffmpeg -hwaccel auto -c:v h264_cuvid -i "{file_path}" -vf "crop={width}:{height}:{top_lext_x}:{top_left_y}" -c:v h264_nvenc -c:a -crf 21 copy "{save_path}"'
+    else:
+        command = str('ffmpeg -y -i ') + '"' + str(file_path) + '"' + str(' -vf ') + str('"crop=') + str(width) + ':' + str(height) + ':' + str(top_lext_x) + ':' + str(top_left_y) + '" ' + str('-c:v libx264 -crf 21 -c:a copy ') + '"' + str(save_path) + '"'
+    timer.stop_timer()
     subprocess.call(command, shell=True)
-    stdout_success(f'Video {file_name} cropped and saved at {save_path}')
+    stdout_success(f'Video {file_name} cropped and saved at {save_path}', elapsed_time=timer.elapsed_time_str)
 
 def crop_multiple_videos(directory_path: Union[str, os.PathLike],
-                         output_path: Union[str, os.PathLike]) -> None:
+                         output_path: Union[str, os.PathLike],
+                         gpu: Optional[bool] = False) -> None:
     """
     Crop multiple videos in a folder according to crop-coordinates defines in the **first** video.
 
     :parameter str directory_path: Directory containing input videos.
     :parameter str output_path: Directory where to save the cropped videos.
+    :parameter Optional[bool] gpu: If True, use NVIDEA GPU codecs. Default False.
 
     :example:
     >>> _ = crop_multiple_videos(directory_path='project_folder/videos', output_path='project_folder/videos/my_new_folder')
     """
 
+    if gpu and not check_nvidea_gpu_available():
+        raise FFMPEGCodecGPUError(msg='NVIDEA GPU not available (as evaluated by nvidea-smi returning None')
     if not os.path.isdir(directory_path):
         raise NotDirectoryError(msg='SIMBA ERROR: {} is not a valid directory'.format(directory_path))
     video_paths = []
     file_paths_in_folder = [f for f in glob.glob(directory_path + '/*') if os.path.isfile(f)]
     for file_path in file_paths_in_folder:
         _, _, ext = get_fn_ext(filepath=file_path)
         if ext.lower() in ['.avi', '.mp4', '.mov', '.flv']:
@@ -600,23 +716,28 @@
     width = int(abs(ROI[0] - (ROI[2] + ROI[0])))
     height = int(abs(ROI[2] - (ROI[3] + ROI[2])))
     top_lext_x, top_left_y = int(ROI[0]), int(ROI[1])
     cv2.waitKey(0)
     cv2.destroyAllWindows()
     if (width == 0 and height == 0) or (width + height + top_lext_x + top_left_y == 0):
         raise CountError(msg='CROP FAILED: Cropping height and width are both 0. Please try again.')
+    timer = SimbaTimer(start=True)
     for file_cnt, file_path in enumerate(video_paths):
         dir_name, file_name, ext = get_fn_ext(filepath=file_path)
         print('Cropping video {}...'.format(file_name))
         _ = get_video_meta_data(file_path)
         save_path = os.path.join(output_path, file_name + '_cropped.mp4')
-        command = str('ffmpeg -i ') + '"' + file_path + '"' + str(' -vf ') + str('"crop=') + str(width) + ':' + str(height) + ':' + str(top_lext_x) + ':' + str(top_left_y) + '" ' + str('-c:v libx264 -crf 21 -c:a copy ') + '"' + str(save_path) + '"'
+        if gpu:
+            command = f'ffmpeg -hwaccel auto -c:v h264_cuvid -i "{file_path}" -vf "crop={width}:{height}:{top_lext_x}:{top_left_y}" -c:v h264_nvenc -c:a -crf 21 copy "{save_path}"'
+        else:
+            command = str('ffmpeg -i ') + '"' + file_path + '"' + str(' -vf ') + str('"crop=') + str(width) + ':' + str(height) + ':' + str(top_lext_x) + ':' + str(top_left_y) + '" ' + str('-c:v libx264 -crf 21 -c:a copy ') + '"' + str(save_path) + '"'
         subprocess.call(command, shell=True)
         print('Video {} cropped (Video {}/{})'.format(file_name, str(file_cnt+1), str(len(video_paths))))
-    stdout_success(msg=f'{str(len(video_paths))} videos cropped and saved in {directory_path} directory')
+    timer.stop_timer()
+    stdout_success(msg=f'{str(len(video_paths))} videos cropped and saved in {directory_path} directory', elapsed_time=timer.elapsed_time_str)
 
 def frames_to_movie(directory: Union[str, os.PathLike],
                     fps: int,
                     bitrate: int,
                     img_format: str) -> None:
 
     """
@@ -663,18 +784,22 @@
     """
     Concatenate two videos to a single video
 
     :param str video_one_path: Path to the first video in the concatenated video
     :param str video_two_path: Path to the second video in the concatenated video
     :param int or str resolution: If str, then the name of the video which resolution you want to retain. E.g., `Video_1`. Else int, representing the video width (if vertical concat) or height (if horizontal concat). Aspect raio will be retained.
     :param horizontal: If true, then horizontal concatenation. Else vertical concatenation.
+    :parameter Optional[bool] gpu: If True, use NVIDEA GPU codecs. Default False.
 
     :example:
     >>> video_concatenator(video_one_path='project_folder/videos/Video_1.mp4', video_two_path='project_folder/videos/Video_2.mp4', resolution=800, horizontal=True)
     """
+
+    if gpu and not check_nvidea_gpu_available():
+        raise FFMPEGCodecGPUError(msg='NVIDEA GPU not available (as evaluated by nvidea-smi returning None')
     timer = SimbaTimer(start=True)
     for file_path in [video_one_path, video_two_path]:
         check_file_exist_and_readable(file_path=file_path)
         _ = get_video_meta_data(file_path)
     if type(resolution) is int:
         video_meta_data = {}
         if horizontal:
@@ -701,17 +826,17 @@
             command = 'ffmpeg -y -i "{}" -i "{}" -filter_complex "[0:v]scale={}:-1[v0];[v0][1:v]vstack=inputs=2" "{}"'.format(video_one_path, video_two_path, video_meta_data['width'], save_path)
 
     if gpu:
         process = subprocess.Popen(command, shell=True)
         output, error = process.communicate()
         if process.returncode != 0:
             if 'Unknown decoder' in str(error.split(b'\n')[-2]):
-                raise FFMPEGCodecError(msg='GPU codec not found: reverting to CPU. Properly configure FFMpeg and ensure you have GPU available or use CPU.')
+                raise FFMPEGCodecGPUError(msg='GPU codec not found: reverting to CPU. Properly configure FFMpeg and ensure you have GPU available or use CPU.')
             else:
-                raise FFMPEGCodecError(msg='GPU error. Properly configure FFMpeg and ensure you have GPU available, or use CPU.')
+                raise FFMPEGCodecGPUError(msg='GPU error. Properly configure FFMpeg and ensure you have GPU available, or use CPU.')
         else:
             pass
     else:
        subprocess.call(command, shell=True, stdout=subprocess.PIPE)
     timer.stop_timer()
     stdout_success(msg=f'Videos concatenated and saved at {save_path}', elapsed_time=timer.elapsed_time_str)
 
@@ -859,15 +984,14 @@
         save_path = os.path.join(project_path, 'frames', 'input', video_name)
         if not os.path.exists(save_path): os.makedirs(save_path)
         else: print(f'Frames for video {video_name} already extracted. SimBA is overwriting prior frames...')
         video_to_frames(video_path, save_path, overwrite=True, every=1, chunk_size=1000)
     timer.stop_timer()
     stdout_success(f'Frames created for {str(len(video_paths))} videos', elapsed_time=timer.elapsed_time_str)
 
-
 def copy_img_folder(config_path: Union[str, os.PathLike], source: Union[str, os.PathLike]) -> None:
     """
     Copy directory of png files to the SimBA project. The directory is stored in the project_folder/frames/input folder of the SimBA project
 
     :parameter str config_path: path to SimBA project config file in Configparser format.
     :parameter str source: path to image folder outside SimBA project.
```

### Comparing `Simba-UW-tf-dev-1.64.1/simba/video_processors/.DS_Store` & `Simba-UW-tf-dev-1.64.2/simba/video_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/video_processors/px_to_mm.py` & `Simba-UW-tf-dev-1.64.2/simba/video_processors/px_to_mm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/video_processors/batch_process_menus.py` & `Simba-UW-tf-dev-1.64.2/simba/video_processors/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/video_processors/video_processing_new.py` & `Simba-UW-tf-dev-1.64.2/simba/video_processors/video_processing_new.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/video_processors/multi_cropper.py` & `Simba-UW-tf-dev-1.64.2/simba/video_processors/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/video_processors/extract_frames.py` & `Simba-UW-tf-dev-1.64.2/simba/video_processors/extract_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/video_processors/calculate_px_dist.py` & `Simba-UW-tf-dev-1.64.2/simba/video_processors/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/video_processors/extract_seqframes.py` & `Simba-UW-tf-dev-1.64.2/simba/video_processors/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/video_processors/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.64.2/simba/video_processors/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.64.2/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/outlier_tools/.DS_Store` & `Simba-UW-tf-dev-1.64.2/simba/outlier_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.64.2/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.64.2/simba/outlier_tools/skip_outlier_correction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/outlier_tools/.idea/outlier_scripts.iml` & `Simba-UW-tf-dev-1.64.2/simba/outlier_tools/.idea/outlier_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.64.2/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/outlier_tools/.idea/workspace.xml` & `Simba-UW-tf-dev-1.64.2/simba/outlier_tools/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/SimBA.py` & `Simba-UW-tf-dev-1.64.2/simba/SimBA.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,27 +93,29 @@
                                                       ClipVideoPopUp,
                                                       MultiShortenPopUp,
                                                       ChangeImageFormatPopUp,
                                                       ConvertVideoPopUp,
                                                       ExtractSpecificFramesPopUp,
                                                       ExtractAllFramesPopUp,
                                                       MultiCropPopUp,
+                                                      GreyscaleSingleVideoPopUp,
                                                       ChangeFpsSingleVideoPopUp,
                                                       ChangeFpsMultipleVideosPopUp,
                                                       ExtractSEQFramesPopUp,
                                                       MergeFrames2VideoPopUp,
                                                       CreateGIFPopUP,
                                                       CalculatePixelsPerMMInVideoPopUp,
                                                       ConcatenatingVideosPopUp,
                                                       ConcatenatorPopUp,
                                                       ImportFrameDirectoryPopUp,
                                                       VideoRotatorPopUp,
                                                       VideoTemporalJoinPopUp,
                                                       DownsampleVideoPopUp,
-                                                      ExtractAnnotationFramesPopUp)
+                                                      ExtractAnnotationFramesPopUp,
+                                                      SuperImposeFrameCountPopUp)
 
 from simba.bounding_box_tools.boundary_menus import BoundaryMenus
 from simba.labelling.labelling_interface import select_labelling_video
 from simba.labelling.labelling_advanced_interface import select_labelling_video_advanced
 from simba.utils.enums import (Formats,
                                OS,
                                Defaults,
@@ -772,16 +774,16 @@
 
         format_menu = Menu(video_process_menu)
         format_menu.add_command(label='Change image file formats',command=ChangeImageFormatPopUp)
         format_menu.add_command(label='Change video file formats',command=ConvertVideoPopUp)
         video_process_menu.add_cascade(label='Change formats...', compound='left', image=self.menu_icons['convert']['img'], menu=format_menu)
 
         video_process_menu.add_command(label='CLAHE enhance video', compound='left', image=self.menu_icons['clahe']['img'], command=CLAHEPopUp)
-        video_process_menu.add_command(label='Superimpose frame numbers on video', compound='left', image=self.menu_icons['trash']['img'], command=lambda:superimpose_frame_count(file_path=askopenfilename()))
-        video_process_menu.add_command(label='Convert to grayscale', compound='left', image=self.menu_icons['grey']['img'], command=lambda:video_to_greyscale(file_path=askopenfilename()))
+        video_process_menu.add_command(label='Superimpose frame numbers on video', compound='left', image=self.menu_icons['trash']['img'], command=lambda:SuperImposeFrameCountPopUp())
+        video_process_menu.add_command(label='Convert to grayscale', compound='left', image=self.menu_icons['grey']['img'], command=lambda:GreyscaleSingleVideoPopUp())
         video_process_menu.add_command(label='Merge frames to video', compound='left', image=self.menu_icons['merge']['img'], command=MergeFrames2VideoPopUp)
         video_process_menu.add_command(label='Generate gifs', compound='left', image=self.menu_icons['gif']['img'], command=CreateGIFPopUP)
         video_process_menu.add_command(label='Rotate videos', compound='left', image=self.menu_icons['rotate']['img'], command=VideoRotatorPopUp)
         video_process_menu.add_command(label='Temporal join videos', compound='left', image=self.menu_icons['stopwatch']['img'], command=VideoTemporalJoinPopUp)
         video_process_menu.add_command(label='Print classifier info...', compound='left', image=self.menu_icons['print']['img'], command=PrintModelInfoPopUp)
 
         extract_frames_menu = Menu(video_process_menu)
```

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.64.2/simba/assets/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.64.2/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.64.2/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.64.2/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.64.2/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.64.2/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/shap/.DS_Store` & `Simba-UW-tf-dev-1.64.2/simba/assets/shap/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.64.2/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.64.2/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.64.2/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.64.2/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.64.2/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.64.2/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.64.2/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.64.2/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.64.2/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.64.2/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.64.2/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.64.2/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.64.2/simba/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/lookups/.DS_Store` & `Simba-UW-tf-dev-1.64.2/simba/assets/lookups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.64.2/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.64.2/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.64.2/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.64.2/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.64.2/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.64.2/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.64.2/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.64.2/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/img/.DS_Store` & `Simba-UW-tf-dev-1.64.2/simba/assets/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.64.2/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.64.2/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.64.2/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/stopwatch.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/stopwatch.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.64.2/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.64.2/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.64.2/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.64.2/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.64.1
+Version: 1.64.2
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.64.1/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.64.2/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.64.2/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/LICENSE.md` & `Simba-UW-tf-dev-1.64.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/tests/test_data_processors.py` & `Simba-UW-tf-dev-1.64.2/tests/test_data_processors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/tests/test_distance_plotter.py` & `Simba-UW-tf-dev-1.64.2/tests/test_distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/tests/test_train_model_mixin.py` & `Simba-UW-tf-dev-1.64.2/tests/test_train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/tests/test_pose_importers.py` & `Simba-UW-tf-dev-1.64.2/tests/test_pose_importers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/tests/test_feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.64.2/tests/test_feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/tests/test_utils_data.py` & `Simba-UW-tf-dev-1.64.2/tests/test_utils_data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/tests/test_config_reader_mixin.py` & `Simba-UW-tf-dev-1.64.2/tests/test_config_reader_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/tests/test_outlier_correctors.py` & `Simba-UW-tf-dev-1.64.2/tests/test_outlier_correctors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/tests/test_visualize_directing_animals.py` & `Simba-UW-tf-dev-1.64.2/tests/test_visualize_directing_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/tests/test_featurizers.py` & `Simba-UW-tf-dev-1.64.2/tests/test_featurizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/tests/test_video_processors.py` & `Simba-UW-tf-dev-1.64.2/tests/test_video_processors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py` & `Simba-UW-tf-dev-1.64.2/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/tests/test_thirdparty_appenders.py` & `Simba-UW-tf-dev-1.64.2/tests/test_thirdparty_appenders.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/tests/test_validation_clips.py` & `Simba-UW-tf-dev-1.64.2/tests/test_validation_clips.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/tests/test_roi_tools.py` & `Simba-UW-tf-dev-1.64.2/tests/test_roi_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/README.md` & `Simba-UW-tf-dev-1.64.2/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.1/setup.py` & `Simba-UW-tf-dev-1.64.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under GNU Lesser General Public License v3.0
 """
 
 import setuptools
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.64.1",
+    version="1.64.2",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of complex social behaviors in experimental animals",
     url="https://github.com/sgoldenlab/simba",
     install_requires=['Pillow == 5.4.1', 'pyyaml == 5.3.1','shapely == 1.7','wxpython == 4.0.4',
               'dtreeviz == 0.8.1','eli5 == 0.10.1','graphviz == 0.11',
               'imblearn == 0.0','imgaug == 0.4.0','imutils == 0.5.2','matplotlib == 3.0.3', 'numpy == 1.18.1',
```

