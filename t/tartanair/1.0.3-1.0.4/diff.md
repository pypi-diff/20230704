# Comparing `tmp/tartanair-1.0.3.tar.gz` & `tmp/tartanair-1.0.4.tar.gz`

## Comparing `tartanair-1.0.3.tar` & `tartanair-1.0.4.tar`

### file list

```diff
@@ -1,126 +1,127 @@
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 tartanair-1.0.3/.gitmodules
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 tartanair-1.0.3/__init__.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 tartanair-1.0.3/.github/workflows/documentation.yaml
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 tartanair-1.0.3/docs/CNAME
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 tartanair-1.0.3/docs/conf.py
--rw-r--r--   0        0        0     9378 2020-02-02 00:00:00.000000 tartanair-1.0.3/docs/examples.rst
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 tartanair-1.0.3/docs/index.rst
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 tartanair-1.0.3/docs/installation.rst
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 tartanair-1.0.3/docs/usage.rst
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 tartanair-1.0.3/examples/customization_example.py
--rw-r--r--   0        0        0     5833 2020-02-02 00:00:00.000000 tartanair-1.0.3/examples/dataloader_example.py
--rw-r--r--   0        0        0     4215 2020-02-02 00:00:00.000000 tartanair-1.0.3/examples/dataset_example.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 tartanair-1.0.3/examples/download_config.yaml
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 tartanair-1.0.3/examples/download_example.py
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 tartanair-1.0.3/examples/evaluator_example.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 tartanair-1.0.3/examples/get_traj_example.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 tartanair-1.0.3/examples/iterator_example.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 tartanair-1.0.3/examples/list_example.py
--rw-r--r--   0        0        0     6754 2020-02-02 00:00:00.000000 tartanair-1.0.3/examples/sanity_test.py
--rw-r--r--   0        0        0     6196 2020-02-02 00:00:00.000000 tartanair-1.0.3/examples/slowloader_example.py
--rw-r--r--   0        0        0     8836 2020-02-02 00:00:00.000000 tartanair-1.0.3/examples/trippy_video.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 tartanair-1.0.3/examples/visualization_example.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/__init__.py
--rw-r--r--   0        0        0    26194 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/customizer.py
--rw-r--r--   0        0        0    14773 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/dataloader.py
--rw-r--r--   0        0        0    40499 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/dataset.py
--rw-r--r--   0        0        0    11978 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/downloader.py
--rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/evaluator.py
--rw-r--r--   0        0        0    16084 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/iterator.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/lister.py
--rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/reader.py
--rw-r--r--   0        0        0    23789 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/tartanair.py
--rw-r--r--   0        0        0     4285 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/tartanair_module.py
--rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/visualizer.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/.git
--rw-r--r--   0        0        0     4962 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/CacherDataset.py
--rw-r--r--   0        0        0     4487 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/ConfigParser.py
--rw-r--r--   0        0        0     9452 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/DataCacher.py
--rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/DataSplitter.py
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/LICENSE
--rw-r--r--   0        0        0     9715 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/MultiDatasets.py
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/RAMBuffer.py
--rw-r--r--   0        0        0    10184 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/RAMDataset.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/README.md
--rw-r--r--   0        0        0     5346 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/TrajBuffer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/__init__.py
--rw-r--r--   0        0        0     9001 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/data_roots.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/input_parser.py
--rw-r--r--   0        0        0    43545 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/utils.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/dataspec/flowvo_train_local_v1.yaml
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/dataspec/flowvo_train_local_v2.yaml
--rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/modality_type/ModBase.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/modality_type/__init__.py
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/modality_type/ply_io.py
--rw-r--r--   0        0        0    22699 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/modality_type/tartanair_types.py
--rw-r--r--   0        0        0     9737 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/modality_type/tartanairv1_types.py
--rw-r--r--   0        0        0     7968 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/modality_type/tartandrive_types.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/data_cacher/modality_type/test_register.py
--rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/eval_utils/trajectory_evaluator_ate.py
--rw-r--r--   0        0        0     9795 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/eval_utils/trajectory_evaluator_base.py
--rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/eval_utils/trajectory_evaluator_rpe.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/image_sampler/.git
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/image_sampler/LICENSE
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/image_sampler/__init__.py
--rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/image_sampler/blend_function.py
--rw-r--r--   0        0        0     6911 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/image_sampler/camera_model_sampler.py
--rw-r--r--   0        0        0    11078 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/image_sampler/full_view_rotation.py
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/image_sampler/generic_camera_model_sampler.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/image_sampler/numba_support_check.py
--rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/image_sampler/ocv_torch.py
--rw-r--r--   0        0        0     9941 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/image_sampler/planar_as_base.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/image_sampler/register.py
--rw-r--r--   0        0        0     9238 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/image_sampler/six_images.py
--rw-r--r--   0        0        0     5297 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/image_sampler/six_images_common.py
--rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/image_sampler/six_images_cupy.cu
--rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/image_sampler/six_images_numba.py
--rw-r--r--   0        0        0     6475 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/image_sampler/six_images_py_numba.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/image_sampler/examples/README.md
--rw-r--r--   0        0        0     8745 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/image_sampler/examples/generic_sampler_optical_flow_sampling_example.py
--rw-r--r--   0        0        0   445601 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/image_sampler/examples/data/flow_img.pt
--rw-r--r--   0        0        0     9716 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/image_sampler/examples/examples_utils/visualization_utils.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/.git
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/.gitmodules
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/LICENSE
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/README.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/__init__.py
--rw-r--r--   0        0        0    74909 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/camera_models.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/compatible_torch.py
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/debug.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/file_sys.py
--rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/frame_io.py
--rw-r--r--   0        0        0     9602 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/kalibr_parser.py
--rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/metadata_reader.py
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/point_cloud_helper.py
--rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/pose.py
--rw-r--r--   0        0        0    14499 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/pretty_dict.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/shape_struct.py
--rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/simulated_lidar_pre_def_models.py
--rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/test_frame_io.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/test_inheritance.py
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/examples/README.md
--rw-r--r--   0        0        0     4941 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/examples/linear_fisheye_camera_model.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/ftensor/.git
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/ftensor/LICENSE
--rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/ftensor/README.md
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/ftensor/__init__.py
--rw-r--r--   0        0        0     8218 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/ftensor/_pytree.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/ftensor/compatible_pytree.py
--rw-r--r--   0        0        0     5422 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/ftensor/frame_graph.py
--rw-r--r--   0        0        0    18394 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/ftensor/ftensor.py
--rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/ftensor/test_frame_graph.py
--rw-r--r--   0        0        0    18694 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/ftensor/test_ftensor.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/image_io/__init__.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/image_io/float_type.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/image_io/image_read.py
--rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/image_io/image_write.py
--rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 tartanair-1.0.3/tartanair/image_resampling/mvs_utils/test_data/frame_graph.json
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 tartanair-1.0.3/tests/README.md
--rw-r--r--   0        0        0    14286 2020-02-02 00:00:00.000000 tartanair-1.0.3/tests/tartanairpy_test.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 tartanair-1.0.3/tests/sample_tartanair_v2_data_root/ArchVizTinyHouseDayExposure/Data_hard/P000/image_lcam_custom0_doublesphere/camera_model_params_lcam_image_custom0_doublesphere.json
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 tartanair-1.0.3/tests/sample_tartanair_v2_data_root/ArchVizTinyHouseDayExposure/Data_hard/P000/image_lcam_custom0_pinhole/camera_model_params_lcam_image_custom0_pinhole.json
--rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 tartanair-1.0.3/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 tartanair-1.0.3/LICENSE
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 tartanair-1.0.3/README.md
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 tartanair-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 tartanair-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 tartanair-1.0.4/.gitmodules
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 tartanair-1.0.4/__init__.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 tartanair-1.0.4/.github/workflows/documentation.yaml
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 tartanair-1.0.4/docs/CNAME
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 tartanair-1.0.4/docs/conf.py
+-rw-r--r--   0        0        0     9378 2020-02-02 00:00:00.000000 tartanair-1.0.4/docs/examples.rst
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 tartanair-1.0.4/docs/index.rst
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 tartanair-1.0.4/docs/installation.rst
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 tartanair-1.0.4/docs/troubleshooting.rst
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 tartanair-1.0.4/docs/usage.rst
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 tartanair-1.0.4/examples/customization_example.py
+-rw-r--r--   0        0        0     5278 2020-02-02 00:00:00.000000 tartanair-1.0.4/examples/dataloader_example.py
+-rw-r--r--   0        0        0     4215 2020-02-02 00:00:00.000000 tartanair-1.0.4/examples/dataset_example.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 tartanair-1.0.4/examples/download_config.yaml
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 tartanair-1.0.4/examples/download_example.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 tartanair-1.0.4/examples/evaluator_example.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 tartanair-1.0.4/examples/get_traj_example.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 tartanair-1.0.4/examples/iterator_example.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 tartanair-1.0.4/examples/list_example.py
+-rw-r--r--   0        0        0     6754 2020-02-02 00:00:00.000000 tartanair-1.0.4/examples/sanity_test.py
+-rw-r--r--   0        0        0     6196 2020-02-02 00:00:00.000000 tartanair-1.0.4/examples/slowloader_example.py
+-rw-r--r--   0        0        0     8836 2020-02-02 00:00:00.000000 tartanair-1.0.4/examples/trippy_video.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 tartanair-1.0.4/examples/visualization_example.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/__init__.py
+-rw-r--r--   0        0        0    26513 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/customizer.py
+-rw-r--r--   0        0        0    14978 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/dataloader.py
+-rw-r--r--   0        0        0    40499 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/dataset.py
+-rw-r--r--   0        0        0    11978 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/downloader.py
+-rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/evaluator.py
+-rw-r--r--   0        0        0    16084 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/iterator.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/lister.py
+-rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/reader.py
+-rw-r--r--   0        0        0    24353 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/tartanair.py
+-rw-r--r--   0        0        0     4285 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/tartanair_module.py
+-rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/visualizer.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/data_cacher/.git
+-rw-r--r--   0        0        0     4986 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/data_cacher/CacherDataset.py
+-rw-r--r--   0        0        0     4487 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/data_cacher/ConfigParser.py
+-rw-r--r--   0        0        0     9452 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/data_cacher/DataCacher.py
+-rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/data_cacher/DataSplitter.py
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/data_cacher/LICENSE
+-rw-r--r--   0        0        0     9715 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/data_cacher/MultiDatasets.py
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/data_cacher/RAMBuffer.py
+-rw-r--r--   0        0        0    10184 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/data_cacher/RAMDataset.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/data_cacher/README.md
+-rw-r--r--   0        0        0     5346 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/data_cacher/TrajBuffer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/data_cacher/__init__.py
+-rw-r--r--   0        0        0     9001 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/data_cacher/data_roots.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/data_cacher/input_parser.py
+-rw-r--r--   0        0        0    43545 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/data_cacher/utils.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/data_cacher/dataspec/flowvo_train_local_v1.yaml
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/data_cacher/dataspec/flowvo_train_local_v2.yaml
+-rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/data_cacher/modality_type/ModBase.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/data_cacher/modality_type/__init__.py
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/data_cacher/modality_type/ply_io.py
+-rw-r--r--   0        0        0    25345 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/data_cacher/modality_type/tartanair_types.py
+-rw-r--r--   0        0        0     9737 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/data_cacher/modality_type/tartanairv1_types.py
+-rw-r--r--   0        0        0     7968 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/data_cacher/modality_type/tartandrive_types.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/data_cacher/modality_type/test_register.py
+-rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/eval_utils/trajectory_evaluator_ate.py
+-rw-r--r--   0        0        0     9774 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/eval_utils/trajectory_evaluator_base.py
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/eval_utils/trajectory_evaluator_rpe.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/image_sampler/.git
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/image_sampler/LICENSE
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/image_sampler/__init__.py
+-rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/image_sampler/blend_function.py
+-rw-r--r--   0        0        0     6911 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/image_sampler/camera_model_sampler.py
+-rw-r--r--   0        0        0    11078 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/image_sampler/full_view_rotation.py
+-rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/image_sampler/generic_camera_model_sampler.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/image_sampler/numba_support_check.py
+-rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/image_sampler/ocv_torch.py
+-rw-r--r--   0        0        0     9941 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/image_sampler/planar_as_base.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/image_sampler/register.py
+-rw-r--r--   0        0        0     9238 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/image_sampler/six_images.py
+-rw-r--r--   0        0        0     5297 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/image_sampler/six_images_common.py
+-rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/image_sampler/six_images_cupy.cu
+-rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/image_sampler/six_images_numba.py
+-rw-r--r--   0        0        0     6475 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/image_sampler/six_images_py_numba.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/image_sampler/examples/README.md
+-rw-r--r--   0        0        0     8745 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/image_sampler/examples/generic_sampler_optical_flow_sampling_example.py
+-rw-r--r--   0        0        0   445601 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/image_sampler/examples/data/flow_img.pt
+-rw-r--r--   0        0        0     9716 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/image_sampler/examples/examples_utils/visualization_utils.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/mvs_utils/.git
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/mvs_utils/.gitmodules
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/mvs_utils/LICENSE
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/mvs_utils/README.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/mvs_utils/__init__.py
+-rw-r--r--   0        0        0    77327 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/mvs_utils/camera_models.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/mvs_utils/compatible_torch.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/mvs_utils/debug.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/mvs_utils/file_sys.py
+-rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/mvs_utils/frame_io.py
+-rw-r--r--   0        0        0     9602 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/mvs_utils/kalibr_parser.py
+-rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/mvs_utils/metadata_reader.py
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/mvs_utils/point_cloud_helper.py
+-rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/mvs_utils/pose.py
+-rw-r--r--   0        0        0    14499 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/mvs_utils/pretty_dict.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/mvs_utils/shape_struct.py
+-rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/mvs_utils/simulated_lidar_pre_def_models.py
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/mvs_utils/test_frame_io.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/mvs_utils/test_inheritance.py
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/mvs_utils/examples/README.md
+-rw-r--r--   0        0        0     4941 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/mvs_utils/examples/linear_fisheye_camera_model.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/mvs_utils/ftensor/.git
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/mvs_utils/ftensor/LICENSE
+-rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/mvs_utils/ftensor/README.md
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/mvs_utils/ftensor/__init__.py
+-rw-r--r--   0        0        0     8218 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/mvs_utils/ftensor/_pytree.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/mvs_utils/ftensor/compatible_pytree.py
+-rw-r--r--   0        0        0     5422 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/mvs_utils/ftensor/frame_graph.py
+-rw-r--r--   0        0        0    18394 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/mvs_utils/ftensor/ftensor.py
+-rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/mvs_utils/ftensor/test_frame_graph.py
+-rw-r--r--   0        0        0    18694 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/mvs_utils/ftensor/test_ftensor.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/mvs_utils/image_io/__init__.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/mvs_utils/image_io/float_type.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/mvs_utils/image_io/image_read.py
+-rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/mvs_utils/image_io/image_write.py
+-rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 tartanair-1.0.4/tartanair/image_resampling/mvs_utils/test_data/frame_graph.json
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 tartanair-1.0.4/tests/README.md
+-rw-r--r--   0        0        0    14286 2020-02-02 00:00:00.000000 tartanair-1.0.4/tests/tartanairpy_test.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 tartanair-1.0.4/tests/sample_tartanair_v2_data_root/ArchVizTinyHouseDayExposure/Data_hard/P000/image_lcam_custom0_doublesphere/camera_model_params_lcam_image_custom0_doublesphere.json
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 tartanair-1.0.4/tests/sample_tartanair_v2_data_root/ArchVizTinyHouseDayExposure/Data_hard/P000/image_lcam_custom0_pinhole/camera_model_params_lcam_image_custom0_pinhole.json
+-rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 tartanair-1.0.4/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 tartanair-1.0.4/LICENSE
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 tartanair-1.0.4/README.md
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 tartanair-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 tartanair-1.0.4/PKG-INFO
```

### Comparing `tartanair-1.0.3/.gitmodules` & `tartanair-1.0.4/.gitmodules`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/.github/workflows/documentation.yaml` & `tartanair-1.0.4/.github/workflows/documentation.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
       - uses: actions/setup-python@v3
       - name: Install dependencies
         run: |
           pip3 install sphinx sphinx_rtd_theme
       - name: Sphinx build
         run: |
           sphinx-build docs _build
+          echo "tartanair.org" > _build/CNAME
       - name: Deploy
         uses: peaceiris/actions-gh-pages@v3
         if: ${{ github.event_name == 'push' && github.ref == 'refs/heads/main' }}
         with:
           publish_branch: gh-pages
           github_token: ${{ secrets.GITHUB_TOKEN }}
           publish_dir: _build/
```

### Comparing `tartanair-1.0.3/docs/conf.py` & `tartanair-1.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/docs/examples.rst` & `tartanair-1.0.4/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/docs/index.rst` & `tartanair-1.0.4/docs/index.rst`

 * *Files 8% similar despite different names*

```diff
@@ -26,7 +26,8 @@
 .. toctree::
    :maxdepth: 2
    :caption: Getting Started:
 
    installation
    examples
    usage
+   troubleshooting
```

### Comparing `tartanair-1.0.3/docs/installation.rst` & `tartanair-1.0.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/docs/usage.rst` & `tartanair-1.0.4/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/examples/customization_example.py` & `tartanair-1.0.4/examples/customization_example.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,27 +36,25 @@
                         'fy':  250, 
                         'cx': 500, 
                         'cy': 500, 
                         'width': 1000, 
                         'height': 1000, 
                         'alpha': 0.6, 
                         'xi': -0.2, 
-                        'fov_degree': 195},
+                        'fov_degree': 295},
                 'R_raw_new': np.eye(3).tolist()}
 
-cam_model_2 = {'name': 'radtan', # TUM Fisheye parameters for cam0.
+cam_model_1 = {'name': 'eucm',
                 'raw_side': 'left',
                 'params':
-                        {
-                        'fx': 190.9227077601815,
-                        'fy': 190.89761005621563,
-                        'cx': 254.9135474328476,
-                        'cy': 256.8281792099312,
-                        'width': 1000,
-                        'height': 1000,
-                        'k1': 0.6288947328627524,
-                        'k2': 1.0441360489134845,
-                        'p1': 0.1,
-                        'p2': 0.1},
+                        {'fx': 320, 
+                        'fy':  320, 
+                        'cx': 320, 
+                        'cy': 320, 
+                        'width': 640, 
+                        'height': 640, 
+                        'alpha': 0.99, 
+                        'beta': 1.0, 
+                        'fov_degree': 295},
                 'R_raw_new': np.eye(3).tolist()}
 
-ta.customize(env = 'MiddleEastExposure', difficulty = 'easy', trajectory_id = ['P000'], modality = ['image'], new_camera_models_params=[cam_model_1], num_workers = 12, device='cuda') # Or cpu.
+ta.customize(env = ['MiddleEastExposure', 'ShoreCavesExposure', 'AbandonedCableExposure'], difficulty = 'easy', trajectory_id = [], modality = ['image'], new_camera_models_params=[cam_model_1], num_workers = 12, device='cuda') # Or cpu.
```

### Comparing `tartanair-1.0.3/examples/dataloader_example.py` & `tartanair-1.0.4/examples/dataloader_example.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,47 +18,36 @@
 # tartanair_data_root = './data/tartanair-v2'
 tartanair_data_root = '/media/yoraish/overflow/data/tartanair-v2'
 ta.init(tartanair_data_root)
 
 
 # Specify the environments, difficulties, and trajectory ids to load.
 envs = [
-"AbandonedCableExposure",
-"AbandonedFactoryExposure",
-"AbandonedSchoolExposure",
-"AmericanDinerExposure",
-"ArchVizTinyHouseDayExposure",
-"CarweldingExposure",
-"HQWesternSaloonExposure",
-"JapaneseCityExposure",
-"MiddleEastExposure",
-"ModularNeighborhoodIntExt",
-"OldScandinaviaExposure",
-"ShoreCavesExposure",
+    "AmericanDinerExposure",
 ]
-difficulties = []
-trajectory_ids = ['P000']
+difficulties = ['hard']
+trajectory_ids = ['P005']
 
 # Specify the modalities to load.
-modalities = ['image', 'depth', 'pose']
+modalities = ['image', 'pose', 'imu_gyro', 'imu_time', 'imu_pos']
 camnames = ['lcam_front', 'lcam_left', 'lcam_right', 'lcam_back', 'lcam_top', 'lcam_bottom']
 
 # Specify dataloader configuration. The dataloader operates in the following way:
 # 1. It loads a subset of the dataset to RAM.
 # 2. It serves mini-batches from this subset. The mini-batches are of data-sequences. So for example, if the sequence length is 2, then the mini-batch will have samples of 2 frames each. A batch size of 16 means that the mini-batch will contain 16 pairs of images, for the example of images. The samples do not have to be consecutive, and the 'skip' between the samples can be specified. The sequences also do not have to start from consecutive indices, and the stride between the sequences can be specified.
 # 3. The dataloader will load a new subset of the dataset to RAM while the mini-batches are loaded from the first subset, and switch the subsets when the first subset is exhausted. If the first subset is exhausted before the mini-batches are loaded, then the dataloader will keep loading mini-batches from the first subset until the second subset is loaded.
 
 new_image_shape_hw = [640, 640] # If None, no resizing is performed. If a value is passed, then the image is resized to this shape.
 subset_framenum = 200 # This is the number of frames in a subset. Notice that this is an upper bound on the batch size. Ideally, make this number large to utilize your RAM efficiently. Information about the allocated memory will be provided in the console.
 frame_skip = 0 # This is the number of frames to skip between each frame. For example, if the frame skip is 2 and the sequence length is 3, then the dataloader will load frames [0, 3, 6], [1, 4, 7], [2, 5, 8], etc.
-seq_length = {'image': 2, 'depth': 1, 'pose': 2} # This is the length of the data-sequences. For example, if the sequence length is 2, then the dataloader will load pairs of images.
+seq_length = {'image': 2, 'pose': 2, 'imu_gyro': 10, 'imu_time': 10, 'imu_pos': 10} # This is the length of the data-sequences. For example, if the sequence length is 2, then the dataloader will load pairs of images.
 seq_stride = 1 # This is the stride between the data-sequences. For example, if the sequence length is 2 and the stride is 1, then the dataloader will load pairs of images [0,1], [1,2], [2,3], etc. If the stride is 2, then the dataloader will load pairs of images [0,1], [2,3], [4,5], etc.
-batch_size = 16 # This is the number of data-sequences in a mini-batch.
+batch_size = 4 # This is the number of data-sequences in a mini-batch.
 num_workers = 8 # This is the number of workers to use for loading the data.
-shuffle = True # Whether to shuffle the data. Let's set this to False for now, so that we can see the data loading in a nice video. Yes it is nice don't argue with me please. Just look at it! So nice. :)\
+shuffle = False # Whether to shuffle the data. Let's set this to False for now, so that we can see the data loading in a nice video. Yes it is nice don't argue with me please. Just look at it! So nice. :)\
 
 # Create a dataloader object.
 dataloader = ta.dataloader(env = envs, 
             difficulty = difficulties, 
             trajectory_id = trajectory_ids, 
             modality = modalities, 
             camera_name = camnames, 
@@ -98,23 +87,12 @@
     cross = np.concatenate([cross_top, cross_mid, cross_bottom], axis=0)
 
     # Resize.
     cross = cv2.resize(cross, (cross.shape[1]//4, cross.shape[0]//4))
 
     # Show the image cross.
     cv2.imshow('cross', cross)
-    cv2.imwrite('cross.png', cross)
-    cv2.waitKey(0)
+    cv2.waitKey(1)
 
+    import ipdb; ipdb.set_trace()
 
-    images = []
-    for b in range(batch['rgb_lcam_front'].shape[0]):
-        images.append(batch['rgb_lcam_front'][b][0])
-    # Visualize the images.
-    outimg = np.concatenate(images, axis=1)
-    outimg = cv2.resize(outimg, (outimg.shape[1]//4, outimg.shape[0]//4))
-    cv2.imshow('outimg', outimg)
-    cv2.waitKey(1)
-    
-    
-        
 dataloader.stop_cachers()
```

### Comparing `tartanair-1.0.3/examples/dataset_example.py` & `tartanair-1.0.4/examples/dataset_example.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/examples/evaluator_example.py` & `tartanair-1.0.4/examples/evaluator_example.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/examples/get_traj_example.py` & `tartanair-1.0.4/examples/get_traj_example.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/examples/iterator_example.py` & `tartanair-1.0.4/examples/iterator_example.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/examples/list_example.py` & `tartanair-1.0.4/examples/list_example.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/examples/sanity_test.py` & `tartanair-1.0.4/examples/sanity_test.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/examples/slowloader_example.py` & `tartanair-1.0.4/examples/slowloader_example.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/examples/trippy_video.py` & `tartanair-1.0.4/examples/trippy_video.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/examples/visualization_example.py` & `tartanair-1.0.4/examples/visualization_example.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/customizer.py` & `tartanair-1.0.4/tartanair/customizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,30 @@
 '''
 # General imports.
 import json
 from multiprocessing import Pool
 import multiprocessing
 import os
 import time
+from colorama import Fore, Style
 import cv2
 import numpy as np
 from scipy.spatial.transform import Rotation
 
 # PyTorch imports.
 import torch
 import torch.multiprocessing as mp
 
 # Local imports.
 from .tartanair_module import TartanAirModule
 
 # Image resampling.
 from .image_resampling.image_sampler import SixPlanarNumba
 
-from .image_resampling.mvs_utils.camera_models import Pinhole, DoubleSphere, LinearSphere, Equirectangular, PinholeRadTanFast
+from .image_resampling.mvs_utils.camera_models import Pinhole, DoubleSphere, LinearSphere, Equirectangular, PinholeRadTanFast, EUCM
 from .image_resampling.mvs_utils.shape_struct import ShapeStruct
 from .image_resampling.image_sampler.blend_function import BlendBy2ndOrderGradTorch
 
 class TartanAirCustomizer(TartanAirModule):
     def __init__(self, tartanair_data_root):
         super().__init__(tartanair_data_root)
 
@@ -37,15 +38,16 @@
         self.data_root = tartanair_data_root
 
         # Available camera models.
         self.camera_model_name_to_class = {'pinhole': Pinhole, 
                                            'doublesphere': DoubleSphere, 
                                            'linearsphere': LinearSphere, 
                                            'equirect': Equirectangular,
-                                           'radtan': PinholeRadTanFast}
+                                           'radtan': PinholeRadTanFast,
+                                           'eucm': EUCM}
 
     def customize(self, env, difficulty = [], trajectory_id = [], modality = [], new_camera_models_params = [], R_raw_new = np.eye(4), num_workers = 1, device = 'cpu'):
         ###############################
         # Check the input arguments.
         ###############################
 
         print("Customizing the TartanAir dataset... With {} workers.".format(num_workers))
@@ -146,14 +148,18 @@
         tartanair_path = self.data_root
         envs_to_trajs = self.enumerate_trajs(self.data_folders)
 
         for env_name, env_trajs  in envs_to_trajs.items():
             if self.env_folders and env_name not in self.env_folders:
                 continue
             for rel_traj_path in env_trajs: 
+                # Proceed only if the trajectory is in the list of trajectories to be processed.
+                if trajectory_id and rel_traj_path.split("/")[-1] not in trajectory_id:
+                    continue
+
                 traj_path = os.path.join(tartanair_path, env_name, rel_traj_path)
 
                 # For this trajectory folder, create the appropriate folders for each new data input and populate those with resampled images.
                 for modality in self.modalities:
                     for cam_name in required_cam_sides: # Could be either of lcam or rcam.
                         for new_cam_model_name, (new_cam_model_object, R_raw_new, params_dict) in new_cam_model_name_to_cam_model_object_R_dict.items():
                             
@@ -377,16 +383,16 @@
                 env_path = os.path.join(self.data_root, env_folder)
                 difficulty = os.listdir(env_path)
             for difficulty_folder in difficulty:
 
                 # Iterate trajectory.
                 if not trajectory_id:
                     diff_path = os.path.join(self.data_root, env_folder, difficulty_folder)
-                    trajectory_id = os.listdir(diff_path)                
-                for traj_id_folder in trajectory_id:
+                    env_trajectory_id = os.listdir(diff_path)                
+                for traj_id_folder in env_trajectory_id:
 
                     # Iterate modality.
                     if not modality:
                         raise ValueError("modality must be specified.")
                     
                     # Keep a list of the file-count in each modality folder. We expect those to all be the same.
                     modality_num_files = []
```

### Comparing `tartanair-1.0.3/tartanair/dataloader.py` & `tartanair-1.0.4/tartanair/dataloader.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 This class provides an interface to the Data-Cacher module. The data cacher is an efficient two-stage loader that allows for continuous training: parallelizing loading data and serving mini-batches.
 
 Output batches will be of the form:
 
 '''
 
 # TODO(yoraish): there is a notation discrepancy between 'rgb' and 'image'. Should fix this and probably stick with 'image' as this is the name used in the dataset. 
-# TODO(yoraish): support naming between 'imu_acc' and 'imu_gyro' etc. Currently only 'imu' is supported and is mapped to 'imu_acc'.
 
 # General imports.
 import os
 from colorama import Fore, Back, Style
 
 
 # Local imports.
@@ -30,39 +29,50 @@
 
         # Remap some modality names to support naming inconsistencies.
         self.modality_name_remaps = {
             'rgb': 'rgb',
             'image': 'rgb',
             'imu': 'imu_acc',
             'imu_acc': 'imu_acc',
+            'imu_gyro': 'imu_gyro',
+            'imu_time': 'imu_time',
             'depth': 'depth',
             'lidar': 'lidar',
             'pose': 'pose',
             'seg': 'seg',
-            'flow': 'flow'
+            'flow': 'flow',
+            'cam_time': 'cam_time',
+            'imu_pos': 'imu_pos'
         }
 
 
         self.modality_default_seq_length = {
             'rgb': 1,
             'depth': 1,
             'seg': 1,
             'flow': 1,
             'pose': 1,
             'imu_acc': 10,
+            'imu_gyro': 10,
+            'imu_time': 10,
             'lidar': 1,
+            'cam_time': 1,
+            'imu_pos': 10
         }
 
         self.modality_default_cacher_size = {
             'rgb': [640, 640],
             'depth': [640, 640],
             'seg': [640, 640],
             'flow': [640, 640],
             'pose': [7],
             'imu_acc': [3],
+            'imu_gyro': [3],
+            'imu_time': [1],
+            'imu_pos': [3],
             'lidar': [3],
         }
 
     def get_data_cacher(self, 
                         env, 
                         difficulty = None, 
                         trajectory_id = None,
```

### Comparing `tartanair-1.0.3/tartanair/dataset.py` & `tartanair-1.0.4/tartanair/dataset.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/downloader.py` & `tartanair-1.0.4/tartanair/downloader.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/evaluator.py` & `tartanair-1.0.4/tartanair/evaluator.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/iterator.py` & `tartanair-1.0.4/tartanair/iterator.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/lister.py` & `tartanair-1.0.4/tartanair/lister.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/reader.py` & `tartanair-1.0.4/tartanair/reader.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/tartanair.py` & `tartanair-1.0.4/tartanair/tartanair.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
     :param env: The environment to download. Can be a list of environments.
     :type env: str or list
     :param difficulty: The difficulty of the trajectory. Can be a list of difficulties. Valid difficulties are: easy, hard.
     :type difficulty: str or list
     :param trajectory_id: The id of the trajectory to download. Can be a list of trajectory ids of form P000, P001, etc.
     :type trajectory_id: str or list
-    :param modality: The modality to download. Can be a list of modalities. Valid modalities are: image, depth, seg, imu{_acc, _gyro...}, lidar. Default will include all.
+    :param modality: The modality to download. Can be a list of modalities. Valid modalities are: image, depth, seg, imu{_acc, _gyro, _time, ...}, lidar. Default will include all.
     :type modality: str or list
     :param camera_name: The camera name to download. Can be a list of camera names. Default will include all. Choices are `lcam_front`, `lcam_right`, `lcam_back`, `lcam_left`, `lcam_top`, `lcam_bottom`, `rcam_front`, `rcam_right`, `rcam_back`, `rcam_left`, `rcam_top`, `rcam_bottom`, `lcam_fish`, `rcam_fish`, `lcam_equirect`, `rcam_equirect`.
      Modalities IMU and LIDAR do not need camera names specified.
     :type camera_name: str or list
     :param config: Optional. Path to a yaml file containing the download configuration. If a config file is provided, the other arguments will be ignored.
     :type config: str
     """
@@ -101,35 +101,38 @@
 
 def customize(env, difficulty, trajectory_id, modality, new_camera_models_params = [{}], num_workers = 1, device = "cpu"):
     """
     Synthesizes raw data into new camera-models. A few camera models are provided, although you can also provide your own camera models. The currently available camera models are:
 
     * 'pinhole': A pinhole camera model.
     * 'doublesphere': A wide-angle camera model with a double sphere distortion model. Source: https://arxiv.org/abs/1807.08957
-    * 'linearsphere': A wide-angle camera model with a custom "linear sphere" distortion model.
+    * 'linearsphere': A wide-angle camera model with a custom "linear sphere" distortion model. There is a constant azimuth/elevation delta between vertical/horizontal lines.
     * 'equirect': An equirectangular camera model.
+    * 'eucm': Enhanced Unified Camera Model. Source: https://ieeexplore.ieee.org/document/7342909
     
     :param env: The environment to customize. Can be a list of environments.
     :type env: str or list
     :param difficulty: The difficulty of the trajectory. Can be a list of difficulties. Valid difficulties are: `easy`, `hard`.
     :type difficulty: str or list
     :param trajectory_id: The id of the trajectory to customize. Can be a list of trajectory ids of form `P000`, `P001`, etc.
     :type trajectory_id: str or list
     :param modality: The modality to be customized. Can be a list of modalities. Valid modalities are: `image`, `depth`, `seg`.
     :type modality: str or list
     :param new_camera_models_params: A list of dictionaries containing the parameters for the new camera models. Each dictionary should contain the following keys:
             
-        * `name`: The name of the camera model. Valid camera models are: `pinhole`, `doublesphere`, `linearsphere`, `equirect`.
+        * `name`: The name of the camera model. Valid camera models are: `pinhole`, `doublesphere`, `linearsphere`, `equirect`, `eucm`.
         * `raw_side`: The raw camera side. Can be one of `left`, `right`.
         * `R_raw_new`: The rotation matrix from the raw camera frame, with z pointing out of the image frame, x right, y down, to the new camera frame.
         * `params`: A dictionary containing the parameters for the new camera model. The parameters for each camera model are:
             * `pinhole`: `fx`, `fy`, `cx`, `cy`, `height`, `width`.
             * `doublesphere`: `fx`, `fy`, `cx`, `cy`, `height`, `width`, `xi`, `alpha`, `fov_degree`.
             * `linearsphere`: `fx`, `fy`, `cx`, `cy`, `height`, `width`, `fov_degree`.
             * `equirect`: `height`, `width`.
+            * `eucm`: `fx`, `fy`, `cx`, `cy`, `height`, `width`, `alpha`, `beta`, `fov_degree`.
+            
     :type new_camera_models_params: list
     :param num_workers: The number of workers to use for the customizer. Default is 1.
     :type num_workers: int
     """
     global customizer
     check_init()
     customizer.customize(env, difficulty, trajectory_id, modality, new_camera_models_params, num_workers=num_workers, device=device)
@@ -158,15 +161,15 @@
 
     :param env: The environments to load. Can be a list of environments or a single environment.
     :type env: str or list
     :param difficulty: The difficulty of the trajectory. Can be a list of difficulties or a single difficulty. Valid difficulties are: easy, hard. If empty, all difficulties will be loaded.
     :type difficulty: str or list
     :param trajectory_id: The id of the trajectory to load. Can be a list of trajectory ids of form P000, P001, etc.
     :type trajectory_id: str or list
-    :param modality: The modality to load. Can be a list of modalities or a single modality. Valid modalities are: image, depth, seg, flow, imu{_acc, _gyro, ...}, lidar. If empty, a sample of a few modalities will be loaded. Please specify your requested modalities explicitly or be pleasantly surprised by the data you get.
+    :param modality: The modality to load. Can be a list of modalities or a single modality. Valid modalities are: image, depth, seg, flow, imu{_acc, _gyro, _time, _pos}, lidar. The `imu_time` is the timestamp of the imu measurements, and the `imu_pos` are the global translation values of the imu, which should be identical to `lcam` with an orientation similar to `lcam_front`. Both in a higher frequency than the images though. If empty, a sample of a few modalities will be loaded. Please specify your requested modalities explicitly or be pleasantly surprised by the data you get.
     :type modality: str or list
     :param camera_name: The camera name to load. Can be a list of camera names or a single camera name. Valid camera names are: lcam_front, lcam_rear, lcam_left, lcam_right, lcam_fish, lcam_equirect, rcam_front, rcam_rear, rcam_left, rcam_right, rcam_fish, rcam_equirect. If empty, all cameras will be loaded.
     :type camera_name: str or list
     :param new_image_shape_hw: The new image shape to resize the images to [height, width]. If empty, the original image shape [640, 640] will be used.
     :type new_image_shape_hw: list
     :param subset_framenum: The number of frames to load in a single subset on the RAM, per modality type. If empty, 360 frames will be loaded. Notice that this is an upper bound on the bath size as well, as batches are harvested from the subset that has been loaded to RAM, so they can be at most as large as the subset.
     :type subset_framenum: int
```

### Comparing `tartanair-1.0.3/tartanair/tartanair_module.py` & `tartanair-1.0.4/tartanair/tartanair_module.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/visualizer.py` & `tartanair-1.0.4/tartanair/visualizer.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/data_cacher/CacherDataset.py` & `tartanair-1.0.4/tartanair/data_cacher/CacherDataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         # load numpy file for each trajectory and concate them together
         assert trajidx<self.trajnum, "Traj {} exceeds the total number of trajectories {}".format(trajidx, self.trajnum)
         trajstr = self.trajlist[trajidx]
         trajdir = join(self.dataroot, trajstr)
         data = self.modality.load_data(trajdir, self.framelist[trajidx])
         assert data.shape[0] == self.trajlenlist[trajidx]*self.modality.freq_mult, \
             "Traj {} mod {} data loaded size {} different from the required size {}".format(trajdir, 
-            self.modality.name, data.shape[0], self.trajlenlist[trajidx])
+            self.modality.name, data.shape[0], self.trajlenlist[trajidx]*self.modality.freq_mult)
         return data
 
 if __name__=="__main__":
     from .modality_type.tartanair_types import rgb_lcam_front, depth_lcam_front, flow_lcam_front
     from .input_parser import parse_inputfile
     from .utils import visdepth, visflow
     import cv2
```

### Comparing `tartanair-1.0.3/tartanair/data_cacher/ConfigParser.py` & `tartanair-1.0.4/tartanair/data_cacher/ConfigParser.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/data_cacher/DataCacher.py` & `tartanair-1.0.4/tartanair/data_cacher/DataCacher.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/data_cacher/DataSplitter.py` & `tartanair-1.0.4/tartanair/data_cacher/DataSplitter.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/data_cacher/LICENSE` & `tartanair-1.0.4/tartanair/data_cacher/LICENSE`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/data_cacher/MultiDatasets.py` & `tartanair-1.0.4/tartanair/data_cacher/MultiDatasets.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/data_cacher/RAMBuffer.py` & `tartanair-1.0.4/tartanair/data_cacher/RAMBuffer.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/data_cacher/RAMDataset.py` & `tartanair-1.0.4/tartanair/data_cacher/RAMDataset.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/data_cacher/TrajBuffer.py` & `tartanair-1.0.4/tartanair/data_cacher/TrajBuffer.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/data_cacher/data_roots.py` & `tartanair-1.0.4/tartanair/data_cacher/data_roots.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/data_cacher/input_parser.py` & `tartanair-1.0.4/tartanair/data_cacher/input_parser.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/data_cacher/utils.py` & `tartanair-1.0.4/tartanair/data_cacher/utils.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/data_cacher/dataspec/flowvo_train_local_v1.yaml` & `tartanair-1.0.4/tartanair/data_cacher/dataspec/flowvo_train_local_v1.yaml`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/data_cacher/dataspec/flowvo_train_local_v2.yaml` & `tartanair-1.0.4/tartanair/data_cacher/dataspec/flowvo_train_local_v2.yaml`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/data_cacher/modality_type/ModBase.py` & `tartanair-1.0.4/tartanair/data_cacher/modality_type/ModBase.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/data_cacher/modality_type/ply_io.py` & `tartanair-1.0.4/tartanair/data_cacher/modality_type/ply_io.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/data_cacher/modality_type/tartanair_types.py` & `tartanair-1.0.4/tartanair/data_cacher/modality_type/tartanair_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,64 @@
     def data_padding(self):
         '''
         In TartanAir, the lengh of IMU seq is (N-1)*10
         We would like the data be aligned, which means the nominal lengh should be N*10
         That's why we pad the data with 10 frames
         '''
         return np.zeros((10,3), dtype=np.float32)
+    
+class IMUTimeBase(SimpleModBase):
+    '''
+    This defines modality that is light-weight
+    such as IMU, pose, wheel_encoder
+    '''
+    def __init__(self, datashape):
+        super().__init__(datashape)
+        self.data_shape = (1,)
+
+        self.freq_mult = 10
+        self.drop_last = 10
+
+        self.folder_name = 'imu'
+
+    def crop_trajectory(self, data, framestrlist):
+        startind = int(framestrlist[0]) * self.freq_mult
+        endind = int(framestrlist[-1]) * self.freq_mult # IMU len = (N-1)*10, where N is the number of images
+        datalen = data.shape[0]
+        assert startind < datalen and endind <= datalen, "Error in loading IMU, startind {}, endind {}, datalen {}".format(startind, endind, datalen)
+        return data[startind: endind]
+
+    def data_padding(self):
+        '''
+        In TartanAir, the length of IMU seq is (N-1)*10
+        We would like the data be aligned, which means the nominal lengh should be N*10
+        That's why we pad the data with 10 frames
+        '''
+        return np.zeros((10,1), dtype=np.float32)
+    
+    def load_data(self, trajdir, framestrlist):
+            '''
+            The startingframe indicates the starting frame of this modality
+            It is used in the case that the trajectory is cropped into pieces and the current trajectory is not start from the first frame
+            '''
+            filename = self.get_filename()
+            if filename.endswith('.npy'):
+                data = np.load(join(trajdir, filename)) # this assume the data is stored as np file, this can be changed in the future
+            elif filename.endswith('.txt'):
+                data = np.loadtxt(join(trajdir, filename))
+            else:
+                assert False, "File format is not supported {}".format(filename)
+            # crop the trajectory based on the starting and ending frames
+            data = self.crop_trajectory(data, framestrlist)
+            data = data.reshape(-1,1)
+            padding = self.data_padding()
+            if padding is not None:
+                data = np.concatenate((data, padding), axis=0)
+            return data
+
 
 class LiDARBase(FrameModBase):
     def __init__(self, datashape):
         super().__init__(datashape) # point dimention, e.g. 3 for tartanvo, 6 if rgb is included
         self.data_shape = (57600, 3) # 57600 is the maximun points for Velodyn 16 where there are 16x3600 points
         self.data_type = np.float32
 
@@ -462,15 +512,38 @@
 class imu_gyro(IMUBase):
     '''
     This defines modality that is light-weight
     such as IMU, pose, wheel_encoder
     '''
     def get_filename(self):
         return join(self.folder_name, 'gyro.npy')
+    
+@register(TYPEDICT)
+class imu_time(IMUTimeBase):
+    '''
+    This defines modality that is light-weight
+    such as IMU, pose, wheel_encoder
+    '''
+    def get_filename(self):
+        return join(self.folder_name, 'imu_time.npy')
 
+
+@register(TYPEDICT)
+class imu_pos(IMUBase):
+    '''
+    The pose of the left front camera in 100Hz.
+    '''
+    def __init__(self, datashape):
+        super().__init__(datashape)
+        self.data_shape = (3,)
+
+    def get_filename(self):
+        return 'imu/pos_global.txt'
+
+    
 @register(TYPEDICT)
 class pose_lcam_front(SimpleModBase):
     '''
     The pose of the left front camera.
     '''
     def __init__(self, datashape):
         super().__init__(datashape)
```

### Comparing `tartanair-1.0.3/tartanair/data_cacher/modality_type/tartanairv1_types.py` & `tartanair-1.0.4/tartanair/data_cacher/modality_type/tartanairv1_types.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/data_cacher/modality_type/tartandrive_types.py` & `tartanair-1.0.4/tartanair/data_cacher/modality_type/tartandrive_types.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/data_cacher/modality_type/test_register.py` & `tartanair-1.0.4/tartanair/data_cacher/modality_type/test_register.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/eval_utils/trajectory_evaluator_ate.py` & `tartanair-1.0.4/tartanair/eval_utils/trajectory_evaluator_ate.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/eval_utils/trajectory_evaluator_base.py` & `tartanair-1.0.4/tartanair/eval_utils/trajectory_evaluator_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         #####################
 
         # Set up the plot flag.
         self.plot = plot
 
         # Set up the plot directory.
         if not plot_gfp :
-            self.plot_gfp  = os.path.dirname(est_traj)
+            self.plot_gfp  = "./"
         else:
             self.plot_gfp  = plot_gfp
 
         # Set up the scale flag.
         self.do_scale = do_scale
 
         # Read the trajectories, if those files were provided.
```

### Comparing `tartanair-1.0.3/tartanair/eval_utils/trajectory_evaluator_rpe.py` & `tartanair-1.0.4/tartanair/eval_utils/trajectory_evaluator_rpe.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/image_sampler/LICENSE` & `tartanair-1.0.4/tartanair/image_resampling/image_sampler/LICENSE`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/image_sampler/__init__.py` & `tartanair-1.0.4/tartanair/image_resampling/image_sampler/__init__.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/image_sampler/blend_function.py` & `tartanair-1.0.4/tartanair/image_resampling/image_sampler/blend_function.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/image_sampler/camera_model_sampler.py` & `tartanair-1.0.4/tartanair/image_resampling/image_sampler/camera_model_sampler.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/image_sampler/full_view_rotation.py` & `tartanair-1.0.4/tartanair/image_resampling/image_sampler/full_view_rotation.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/image_sampler/generic_camera_model_sampler.py` & `tartanair-1.0.4/tartanair/image_resampling/image_sampler/generic_camera_model_sampler.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/image_sampler/numba_support_check.py` & `tartanair-1.0.4/tartanair/image_resampling/image_sampler/numba_support_check.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/image_sampler/ocv_torch.py` & `tartanair-1.0.4/tartanair/image_resampling/image_sampler/ocv_torch.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/image_sampler/planar_as_base.py` & `tartanair-1.0.4/tartanair/image_resampling/image_sampler/planar_as_base.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/image_sampler/register.py` & `tartanair-1.0.4/tartanair/image_resampling/image_sampler/register.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/image_sampler/six_images.py` & `tartanair-1.0.4/tartanair/image_resampling/image_sampler/six_images.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/image_sampler/six_images_common.py` & `tartanair-1.0.4/tartanair/image_resampling/image_sampler/six_images_common.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/image_sampler/six_images_cupy.cu` & `tartanair-1.0.4/tartanair/image_resampling/image_sampler/six_images_cupy.cu`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/image_sampler/six_images_numba.py` & `tartanair-1.0.4/tartanair/image_resampling/image_sampler/six_images_numba.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/image_sampler/six_images_py_numba.py` & `tartanair-1.0.4/tartanair/image_resampling/image_sampler/six_images_py_numba.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/image_sampler/examples/README.md` & `tartanair-1.0.4/tartanair/image_resampling/image_sampler/examples/README.md`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/image_sampler/examples/generic_sampler_optical_flow_sampling_example.py` & `tartanair-1.0.4/tartanair/image_resampling/image_sampler/examples/generic_sampler_optical_flow_sampling_example.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/image_sampler/examples/data/flow_img.pt` & `tartanair-1.0.4/tartanair/image_resampling/image_sampler/examples/data/flow_img.pt`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/image_sampler/examples/examples_utils/visualization_utils.py` & `tartanair-1.0.4/tartanair/image_resampling/image_sampler/examples/examples_utils/visualization_utils.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/LICENSE` & `tartanair-1.0.4/tartanair/image_resampling/mvs_utils/LICENSE`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/camera_models.py` & `tartanair-1.0.4/tartanair/image_resampling/mvs_utils/camera_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -501,14 +501,136 @@
     "fov_degree": {self.fov_degree},
     "shape_struct": {self.ss},
     "in_to_tensor": {self.in_to_tensor},
     "out_to_numpy": {self.out_to_numpy}
 }}'''
 
 @register(CAMERA_MODELS)
+class EUCM(CameraModel):
+    def __init__(self, alpha, beta, fx, fy, cx, cy, fov_degree, shape_struct, in_to_tensor=False, out_to_numpy=False):
+        '''
+        Enhanced Unified Camera Model (EUCM).
+    
+        '''
+        super(EUCM, self).__init__(
+            'eucm', fx, fy, cx, cy, fov_degree, shape_struct, in_to_tensor=in_to_tensor, out_to_numpy=out_to_numpy)
+
+        self.alpha = alpha
+        self.beta = beta
+    
+    @CameraModel.device.setter
+    def device(self, d):
+        CameraModel.device.fset(self, d)
+        # Do nothing.
+
+    def pixel_2_ray(self, pixel_coor):
+        '''
+        The definition of the pixel projection according to the Enhanced Unified Camera Model (EUCM). Code is adapted from the original implementation in OmniCV: https://kaustubh-sadekar.github.io/OmniCV-Lib/index.html .
+
+        Arguments:
+        pixel_coor (Tensor): A 2xN Tensor contains the pixel coordinates.
+        
+        NOTE: pixel_coor can also have a dimension of Bx2xN, where B is the 
+        batch number. 
+        
+        Returns:
+        ray: A 3xN Tensor representing the 3D rays. Bx3xN if batched.
+        valid_mask: A (N,) Tensor representing the valid mask. BxN if batched.
+        '''
+        pixel_coor = self.in_wrap(pixel_coor)
+        
+        # mx and my becomes float64 if pixel_coor.dtype is integer type.
+        mx = ( pixel_coor[..., 0, :] - self.cx ) / self.fx
+        my = ( pixel_coor[..., 1, :] - self.cy ) / self.fy
+
+        r_2 = mx ** 2 + my ** 2
+
+        mz = torch.real(
+            (1 - self.beta * self.alpha * self.alpha * r_2)
+            / (
+                self.alpha * torch.sqrt(1 - (2 * self.alpha - 1) *
+                                              self.beta * r_2)
+                + (1 - self.alpha)
+            )
+        )
+
+        coef = 1 / torch.sqrt(mx ** 2 + my ** 2 + mz ** 2)
+
+        x = mx * coef
+        y = my * coef
+        z = mz * coef
+
+        ray = torch.stack((x, y, z), dim=-2)
+        norm_ray = torch.linalg.norm( ray, ord=2, dim=-2, keepdim=True )
+        zero_mask = norm_ray == 0
+        norm_ray[zero_mask] = 1
+
+        # Normalize ray.
+        ray = ray / norm_ray
+
+        # Filter by FOV.
+        valid_mask = torch.logical_not(torch.isnan(z))
+
+
+        # Ray nans to zeros. # TODO(yoraish): This is probably wrong. Handle this more gracefully.
+        ray[torch.isnan(ray)] = 0.0001
+
+        return self.out_wrap(ray), self.out_wrap(valid_mask)
+
+    def point_3d_2_pixel(self, point_3d, normalized=False):
+        '''
+        Arguments:
+        point_3d (Tensor): A 3xN Tensor contains 3D point coordinates. 
+        normalized (bool): If True, then the returned coordinates are normalized to [-1, 1]
+        
+        NOTE: point_3d can also have a dimension of Bx3xN, where B is the 
+        batch number. 
+        
+        Returns: 
+        pixel_coor: A 2xN Tensor representing the 2D pixels. Bx2xN if batched.
+        valid_mask: A (N,) Tensor representing the valid mask. BXN if batched.
+        '''
+
+        point_3d = self.in_wrap(point_3d)
+
+        # torch.split results in Bx1XN.
+        x, y, z = torch.split( point_3d, 1, dim=-2 )
+
+        # If Ftensor convert to Tensor.
+        if isinstance(x, FTensor):
+            x = x.tensor()
+            y = y.tensor()
+            z = z.tensor()
+
+        x2 = x**2.0 # Note: this may promote x2 to torch.float64 if point_3d.dtype=torch.int. 
+        y2 = y**2.0
+        z2 = z**2.0
+
+        raise NotImplementedError()
+
+        return self.out_wrap(pixel_coor), self.out_wrap(valid_mask)
+    
+    
+    def __str__(self) -> str:
+        return \
+f'''{{
+    "type": "{self.__class__.__name__}",
+    "alpha": {self.alpha},
+    "beta": {self.beta},
+    "fx": {self.fx},
+    "fy": {self.fy},
+    "cx": {self.cx},
+    "cy": {self.cy},
+    "fov_degree": {self.fov_degree},
+    "shape_struct": {self.ss},
+    "in_to_tensor": {self.in_to_tensor},
+    "out_to_numpy": {self.out_to_numpy}
+}}'''
+
+@register(CAMERA_MODELS)
 class Equirectangular(CameraModel):
     # def __init__(self, cx, cy, shape_struct, lon_shift=0, open_span=False, in_to_tensor=False, out_to_numpy=False):
     def __init__(self, shape_struct, longitude_span=(-LOCAL_PI, LOCAL_PI), latitude_span=(-LOCAL_PI/2, LOCAL_PI/2), open_span=False, in_to_tensor=False, out_to_numpy=False):
         '''
         Used primarily for generating a panorama image from six pinhole images or ratating a
         panorama image for training.
         
@@ -1241,33 +1363,14 @@
         print("Started calculations for pinhole-radtan.. Might take a couple minutes.")
         for start_batch_idx in tqdm(torch.arange(0,N,batch_size)):
             end_batch = min(start_batch_idx+batch_size,N)
 
             xyz[:,start_batch_idx:end_batch] = self.undistort(self.normalize_points(uv[:,start_batch_idx:end_batch]),homogeneous=True,debug=False)
 
         print("Elapsed time: {0}, for {1} images.".format(time.time()-time_start,N))
-        # xyz = torch.zeros((3,N)).to(dtype=torch.float32, device=self._device)
-        # for i in range(N):
-        #     debug = False
-        #     if i == 0:
-        #         debug = True
-
-        #     xyz[:,i] = self.undistort_single(self.normalize_point(uv[:,i]),homogeneous=True,debug=debug)
-        
-
-        # print("Single")
-        # print(xyz[:,:4])
-
-
-        # Convert to honmogeneous coordinates.
-        # uv1 = F.pad(uv, (0, 0, 0, 1), value=1)
-
-        # Convert to camera-frame (metric).
-
-        # xyz = self.inv_intrinsics @ uv1
 
         # Normalize rays to be unit length.
         xyz = xyz / torch.linalg.norm(xyz, dim = -2, keepdims= True)
 
         # Mask points that are out of field of view.
         # Currently returning a mask of only ones as all pixels are assumed to be with valid values, and the projection out of the image frame of all pixels is valid.
         # The following if-statements match the dimensionality of batched inputs.
@@ -1299,29 +1402,14 @@
         # can we remove the for loop? Not sure, this is how Kalibr does it
         N = point_3d.shape[1]
         # for i in range(N):
         point_3d = torch.div(point_3d,point_3d[-1,:])
         
         point_3d = self.unnormalize_points(self.distort(point_3d,jacobian=False)[0],homogeneous=True)
 
-        # _, Js_parallel = self.distort(point_3d,jacobian=True)
-
-
-        # for i in range(N):
-        #     point_tmp, J = self.distort(torch.tensor([point_3d[0,i],point_3d[1,i]]),jacobian=True)
-        #     point_3d[:,i] = self.unnormalize_point(point_tmp,homogeneous=True)
-
-        # print(point_3d.shape)
-        uv = point_3d
-        # Pixel coordinates projected from the world points. 
-        # uv_unnormalized = self.intrinsics @ point_3d
-
-        # Normalize the homogenous coordinate-points such that their z-value is 1. The expression uv_unnormalized[..., -1:, :] keeps the dimension of the tensor, which is required by the division operation since PyTorch has trouble to broadcast the operation. 
-        # uv = torch.div(uv_unnormalized, uv_unnormalized[..., -1:, :])
-
         # Warp to desired datatype.
         uv = self.in_wrap(uv).to(dtype=torch.float32)
 
         # Do torch.split results in Bx1XN.
         px, py, _ = torch.split( uv, 1, dim=-2 )
 
         if normalized:
@@ -1572,21 +1660,14 @@
         # can we remove the for loop? Not sure, this is how Kalibr does it
         N = point_3d.shape[1]
         # for i in range(N):
         point_3d = torch.div(point_3d,point_3d[-1,:])
         
         point_3d = self.unnormalize_points(self.distort(point_3d),homogeneous=True)
 
-        # _, Js_parallel = self.distort(point_3d,jacobian=True)
-
-
-        # for i in range(N):
-        #     point_tmp, J = self.distort(torch.tensor([point_3d[0,i],point_3d[1,i]]),jacobian=True)
-        #     point_3d[:,i] = self.unnormalize_point(point_tmp,homogeneous=True)
-
         # print(point_3d.shape)
         uv = point_3d
         # Pixel coordinates projected from the world points. 
         # uv_unnormalized = self.intrinsics @ point_3d
 
         # Normalize the homogenous coordinate-points such that their z-value is 1. The expression uv_unnormalized[..., -1:, :] keeps the dimension of the tensor, which is required by the division operation since PyTorch has trouble to broadcast the operation. 
         # uv = torch.div(uv_unnormalized, uv_unnormalized[..., -1:, :])
```

### Comparing `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/compatible_torch.py` & `tartanair-1.0.4/tartanair/image_resampling/mvs_utils/compatible_torch.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/debug.py` & `tartanair-1.0.4/tartanair/image_resampling/mvs_utils/debug.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/frame_io.py` & `tartanair-1.0.4/tartanair/image_resampling/mvs_utils/frame_io.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/kalibr_parser.py` & `tartanair-1.0.4/tartanair/image_resampling/mvs_utils/kalibr_parser.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/metadata_reader.py` & `tartanair-1.0.4/tartanair/image_resampling/mvs_utils/metadata_reader.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/point_cloud_helper.py` & `tartanair-1.0.4/tartanair/image_resampling/mvs_utils/point_cloud_helper.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/pose.py` & `tartanair-1.0.4/tartanair/image_resampling/mvs_utils/pose.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/pretty_dict.py` & `tartanair-1.0.4/tartanair/image_resampling/mvs_utils/pretty_dict.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/shape_struct.py` & `tartanair-1.0.4/tartanair/image_resampling/mvs_utils/shape_struct.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/simulated_lidar_pre_def_models.py` & `tartanair-1.0.4/tartanair/image_resampling/mvs_utils/simulated_lidar_pre_def_models.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/test_frame_io.py` & `tartanair-1.0.4/tartanair/image_resampling/mvs_utils/test_frame_io.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/test_inheritance.py` & `tartanair-1.0.4/tartanair/image_resampling/mvs_utils/test_inheritance.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/examples/README.md` & `tartanair-1.0.4/tartanair/image_resampling/mvs_utils/examples/README.md`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/examples/linear_fisheye_camera_model.py` & `tartanair-1.0.4/tartanair/image_resampling/mvs_utils/examples/linear_fisheye_camera_model.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/ftensor/LICENSE` & `tartanair-1.0.4/tartanair/image_resampling/mvs_utils/ftensor/LICENSE`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/ftensor/README.md` & `tartanair-1.0.4/tartanair/image_resampling/mvs_utils/ftensor/README.md`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/ftensor/_pytree.py` & `tartanair-1.0.4/tartanair/image_resampling/mvs_utils/ftensor/_pytree.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/ftensor/frame_graph.py` & `tartanair-1.0.4/tartanair/image_resampling/mvs_utils/ftensor/frame_graph.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/ftensor/ftensor.py` & `tartanair-1.0.4/tartanair/image_resampling/mvs_utils/ftensor/ftensor.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/ftensor/test_frame_graph.py` & `tartanair-1.0.4/tartanair/image_resampling/mvs_utils/ftensor/test_frame_graph.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/ftensor/test_ftensor.py` & `tartanair-1.0.4/tartanair/image_resampling/mvs_utils/ftensor/test_ftensor.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/image_io/float_type.py` & `tartanair-1.0.4/tartanair/image_resampling/mvs_utils/image_io/float_type.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/image_io/image_read.py` & `tartanair-1.0.4/tartanair/image_resampling/mvs_utils/image_io/image_read.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/image_io/image_write.py` & `tartanair-1.0.4/tartanair/image_resampling/mvs_utils/image_io/image_write.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tartanair/image_resampling/mvs_utils/test_data/frame_graph.json` & `tartanair-1.0.4/tartanair/image_resampling/mvs_utils/test_data/frame_graph.json`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tests/README.md` & `tartanair-1.0.4/tests/README.md`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tests/tartanairpy_test.py` & `tartanair-1.0.4/tests/tartanairpy_test.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/tests/sample_tartanair_v2_data_root/ArchVizTinyHouseDayExposure/Data_hard/P000/image_lcam_custom0_doublesphere/camera_model_params_lcam_image_custom0_doublesphere.json` & `tartanair-1.0.4/tests/sample_tartanair_v2_data_root/ArchVizTinyHouseDayExposure/Data_hard/P000/image_lcam_custom0_doublesphere/camera_model_params_lcam_image_custom0_doublesphere.json`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/.gitignore` & `tartanair-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/LICENSE` & `tartanair-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.3/pyproject.toml` & `tartanair-1.0.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tartanair"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Yorai Shaoul", email="yorai@cmu.edu" },
   { name="Wenshan Wang", email="wenshanw@cs.cmu.edu " } 
 ]
 description = "TartanAir"
 readme = "README.md"
 requires-python = ">=3.7"
@@ -29,12 +29,15 @@
     "Pillow",
     "plyfile",
     "pyquaternion",
     "pytransform3d",
     "PyYAML",
     "scipy",
     "pyyaml",
-    "pandas"
+    "pandas",
+    "imageio",
+    "einops",
+    "tqdm"
     ]
 
 [project.urls]
 "Homepage" = "https://tartanair.org"
```

### Comparing `tartanair-1.0.3/PKG-INFO` & `tartanair-1.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Metadata-Version: 2.1
 Name: tartanair
-Version: 1.0.3
+Version: 1.0.4
 Summary: TartanAir
 Project-URL: Homepage, https://tartanair.org
 Author-email: Yorai Shaoul <yorai@cmu.edu>, Wenshan Wang <wenshanw@cs.cmu.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: colorama>=0.4.0
+Requires-Dist: einops
+Requires-Dist: imageio
 Requires-Dist: kornia
 Requires-Dist: matplotlib>=3.1.2
 Requires-Dist: networkx>=2.4
 Requires-Dist: numba>=0.56
 Requires-Dist: numpy
 Requires-Dist: opencv-contrib-python
 Requires-Dist: pandas
 Requires-Dist: pillow
 Requires-Dist: plyfile
 Requires-Dist: pyquaternion
 Requires-Dist: pytransform3d
 Requires-Dist: pyyaml
 Requires-Dist: scipy
+Requires-Dist: tqdm
 Description-Content-Type: text/markdown
 
 # TartanAir
 
 Hello and welcome to the official TartanAir repository. This repository includes a set of tools that complement the [TartanAir Dataset](https://www.tartanair.org/)).
```

