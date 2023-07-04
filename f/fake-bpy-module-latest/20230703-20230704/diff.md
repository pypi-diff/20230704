# Comparing `tmp/fake-bpy-module-latest-20230703.tar.gz` & `tmp/fake-bpy-module-latest-20230704.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fake-bpy-module-latest-20230703.tar", last modified: Mon Jul  3 06:23:33 2023, max compression
+gzip compressed data, was "dist/fake-bpy-module-latest-20230704.tar", last modified: Tue Jul  4 06:27:34 2023, max compression
```

## Comparing `fake-bpy-module-latest-20230703.tar` & `fake-bpy-module-latest-20230704.tar`

### file list

```diff
@@ -1,357 +1,357 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 06:23:33.000000 fake-bpy-module-latest-20230703/
--rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-07-03 06:23:33.000000 fake-bpy-module-latest-20230703/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-07-03 06:23:32.000000 fake-bpy-module-latest-20230703/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-03 06:21:37.000000 fake-bpy-module-latest-20230703/addon_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-03 06:23:31.000000 fake-bpy-module-latest-20230703/animsys_refactor.py
--rw-r--r--   0 runner    (1001) docker     (123)    30417 2023-07-03 06:21:33.000000 fake-bpy-module-latest-20230703/aud.py
--rw-r--r--   0 runner    (1001) docker     (123)   116266 2023-07-03 06:21:30.000000 fake-bpy-module-latest-20230703/bgl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 06:23:33.000000 fake-bpy-module-latest-20230703/bl_app_override/
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-03 06:21:36.000000 fake-bpy-module-latest-20230703/bl_app_override/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-03 06:21:36.000000 fake-bpy-module-latest-20230703/bl_app_override/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 06:14:33.000000 fake-bpy-module-latest-20230703/bl_app_override/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-03 06:21:37.000000 fake-bpy-module-latest-20230703/bl_app_template_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 06:23:33.000000 fake-bpy-module-latest-20230703/bl_console_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-03 06:21:37.000000 fake-bpy-module-latest-20230703/bl_console_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 06:23:33.000000 fake-bpy-module-latest-20230703/bl_console_utils/autocomplete/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-03 06:21:37.000000 fake-bpy-module-latest-20230703/bl_console_utils/autocomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-03 06:21:37.000000 fake-bpy-module-latest-20230703/bl_console_utils/autocomplete/complete_calltip.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-03 06:21:37.000000 fake-bpy-module-latest-20230703/bl_console_utils/autocomplete/complete_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-03 06:21:37.000000 fake-bpy-module-latest-20230703/bl_console_utils/autocomplete/complete_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-03 06:21:37.000000 fake-bpy-module-latest-20230703/bl_console_utils/autocomplete/intellisense.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 06:14:33.000000 fake-bpy-module-latest-20230703/bl_console_utils/autocomplete/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 06:14:33.000000 fake-bpy-module-latest-20230703/bl_console_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 06:23:33.000000 fake-bpy-module-latest-20230703/bl_i18n_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-03 06:21:36.000000 fake-bpy-module-latest-20230703/bl_i18n_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-03 06:21:36.000000 fake-bpy-module-latest-20230703/bl_i18n_utils/bl_extract_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-03 06:21:36.000000 fake-bpy-module-latest-20230703/bl_i18n_utils/merge_po.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 06:14:33.000000 fake-bpy-module-latest-20230703/bl_i18n_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-03 06:21:36.000000 fake-bpy-module-latest-20230703/bl_i18n_utils/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-07-03 06:21:36.000000 fake-bpy-module-latest-20230703/bl_i18n_utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-03 06:21:36.000000 fake-bpy-module-latest-20230703/bl_i18n_utils/utils_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-03 06:21:36.000000 fake-bpy-module-latest-20230703/bl_i18n_utils/utils_languages_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-03 06:21:36.000000 fake-bpy-module-latest-20230703/bl_i18n_utils/utils_rtl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 06:23:33.000000 fake-bpy-module-latest-20230703/bl_keymap_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-03 06:21:36.000000 fake-bpy-module-latest-20230703/bl_keymap_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-03 06:21:36.000000 fake-bpy-module-latest-20230703/bl_keymap_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-03 06:21:36.000000 fake-bpy-module-latest-20230703/bl_keymap_utils/keymap_from_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-03 06:21:36.000000 fake-bpy-module-latest-20230703/bl_keymap_utils/keymap_hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-03 06:21:36.000000 fake-bpy-module-latest-20230703/bl_keymap_utils/platform_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 06:14:33.000000 fake-bpy-module-latest-20230703/bl_keymap_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-03 06:21:36.000000 fake-bpy-module-latest-20230703/bl_keymap_utils/versioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-03 06:21:36.000000 fake-bpy-module-latest-20230703/bl_math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 06:23:33.000000 fake-bpy-module-latest-20230703/bl_operators/
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-03 06:23:25.000000 fake-bpy-module-latest-20230703/bl_operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-03 06:23:26.000000 fake-bpy-module-latest-20230703/bl_operators/add_mesh_torus.py
--rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-07-03 06:23:26.000000 fake-bpy-module-latest-20230703/bl_operators/anim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-03 06:23:28.000000 fake-bpy-module-latest-20230703/bl_operators/assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 06:23:33.000000 fake-bpy-module-latest-20230703/bl_operators/bmesh/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-03 06:23:26.000000 fake-bpy-module-latest-20230703/bl_operators/bmesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-03 06:23:26.000000 fake-bpy-module-latest-20230703/bl_operators/bmesh/find_adjacent.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 06:14:33.000000 fake-bpy-module-latest-20230703/bl_operators/bmesh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22556 2023-07-03 06:23:30.000000 fake-bpy-module-latest-20230703/bl_operators/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-07-03 06:23:28.000000 fake-bpy-module-latest-20230703/bl_operators/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-07-03 06:23:30.000000 fake-bpy-module-latest-20230703/bl_operators/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-07-03 06:23:26.000000 fake-bpy-module-latest-20230703/bl_operators/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-07-03 06:23:28.000000 fake-bpy-module-latest-20230703/bl_operators/freestyle.py
--rw-r--r--   0 runner    (1001) docker     (123)    15010 2023-07-03 06:23:26.000000 fake-bpy-module-latest-20230703/bl_operators/geometry_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-07-03 06:23:28.000000 fake-bpy-module-latest-20230703/bl_operators/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-07-03 06:23:30.000000 fake-bpy-module-latest-20230703/bl_operators/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    18689 2023-07-03 06:23:26.000000 fake-bpy-module-latest-20230703/bl_operators/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    38122 2023-07-03 06:23:27.000000 fake-bpy-module-latest-20230703/bl_operators/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-07-03 06:23:28.000000 fake-bpy-module-latest-20230703/bl_operators/object_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-07-03 06:23:26.000000 fake-bpy-module-latest-20230703/bl_operators/object_quick_effects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-03 06:23:26.000000 fake-bpy-module-latest-20230703/bl_operators/object_randomize_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    45483 2023-07-03 06:23:28.000000 fake-bpy-module-latest-20230703/bl_operators/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 06:14:33.000000 fake-bpy-module-latest-20230703/bl_operators/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-07-03 06:23:31.000000 fake-bpy-module-latest-20230703/bl_operators/rigidbody.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-03 06:23:26.000000 fake-bpy-module-latest-20230703/bl_operators/screen_play_rendered_anim.py
--rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-07-03 06:23:26.000000 fake-bpy-module-latest-20230703/bl_operators/sequencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-07-03 06:23:28.000000 fake-bpy-module-latest-20230703/bl_operators/spreadsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-03 06:23:28.000000 fake-bpy-module-latest-20230703/bl_operators/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    56119 2023-07-03 06:23:31.000000 fake-bpy-module-latest-20230703/bl_operators/userpref.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-07-03 06:23:30.000000 fake-bpy-module-latest-20230703/bl_operators/uvcalc_follow_active.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-07-03 06:23:26.000000 fake-bpy-module-latest-20230703/bl_operators/uvcalc_lightmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-07-03 06:23:30.000000 fake-bpy-module-latest-20230703/bl_operators/uvcalc_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-07-03 06:23:30.000000 fake-bpy-module-latest-20230703/bl_operators/vertexpaint_dirt.py
--rw-r--r--   0 runner    (1001) docker     (123)    11529 2023-07-03 06:23:26.000000 fake-bpy-module-latest-20230703/bl_operators/view3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    97916 2023-07-03 06:23:30.000000 fake-bpy-module-latest-20230703/bl_operators/wm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 06:23:33.000000 fake-bpy-module-latest-20230703/bl_previews_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-03 06:23:25.000000 fake-bpy-module-latest-20230703/bl_previews_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-03 06:23:25.000000 fake-bpy-module-latest-20230703/bl_previews_utils/bl_previews_render.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 06:14:33.000000 fake-bpy-module-latest-20230703/bl_previews_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 06:23:33.000000 fake-bpy-module-latest-20230703/bl_rna_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-03 06:21:36.000000 fake-bpy-module-latest-20230703/bl_rna_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-03 06:21:36.000000 fake-bpy-module-latest-20230703/bl_rna_utils/data_path.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 06:14:33.000000 fake-bpy-module-latest-20230703/bl_rna_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 06:23:33.000000 fake-bpy-module-latest-20230703/bl_ui/
--rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-07-03 06:21:38.000000 fake-bpy-module-latest-20230703/bl_ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-07-03 06:23:24.000000 fake-bpy-module-latest-20230703/bl_ui/generic_ui_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-03 06:22:34.000000 fake-bpy-module-latest-20230703/bl_ui/node_add_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)   110864 2023-07-03 06:22:25.000000 fake-bpy-module-latest-20230703/bl_ui/node_add_menu_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-03 06:23:24.000000 fake-bpy-module-latest-20230703/bl_ui/properties_animviz.py
--rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-07-03 06:22:49.000000 fake-bpy-module-latest-20230703/bl_ui/properties_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)   385296 2023-07-03 06:22:45.000000 fake-bpy-module-latest-20230703/bl_ui/properties_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    25330 2023-07-03 06:22:51.000000 fake-bpy-module-latest-20230703/bl_ui/properties_data_armature.py
--rw-r--r--   0 runner    (1001) docker     (123)    22602 2023-07-03 06:23:22.000000 fake-bpy-module-latest-20230703/bl_ui/properties_data_bone.py
--rw-r--r--   0 runner    (1001) docker     (123)    36945 2023-07-03 06:22:34.000000 fake-bpy-module-latest-20230703/bl_ui/properties_data_camera.py
--rw-r--r--   0 runner    (1001) docker     (123)    38857 2023-07-03 06:23:18.000000 fake-bpy-module-latest-20230703/bl_ui/properties_data_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)    15423 2023-07-03 06:23:22.000000 fake-bpy-module-latest-20230703/bl_ui/properties_data_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-07-03 06:22:46.000000 fake-bpy-module-latest-20230703/bl_ui/properties_data_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)    46403 2023-07-03 06:22:32.000000 fake-bpy-module-latest-20230703/bl_ui/properties_data_gpencil.py
--rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-07-03 06:23:01.000000 fake-bpy-module-latest-20230703/bl_ui/properties_data_grease_pencil.py
--rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-07-03 06:22:55.000000 fake-bpy-module-latest-20230703/bl_ui/properties_data_lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-07-03 06:23:24.000000 fake-bpy-module-latest-20230703/bl_ui/properties_data_light.py
--rw-r--r--   0 runner    (1001) docker     (123)    15425 2023-07-03 06:22:25.000000 fake-bpy-module-latest-20230703/bl_ui/properties_data_lightprobe.py
--rw-r--r--   0 runner    (1001) docker     (123)    52746 2023-07-03 06:22:56.000000 fake-bpy-module-latest-20230703/bl_ui/properties_data_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-07-03 06:22:51.000000 fake-bpy-module-latest-20230703/bl_ui/properties_data_metaball.py
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-07-03 06:23:22.000000 fake-bpy-module-latest-20230703/bl_ui/properties_data_modifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-07-03 06:22:56.000000 fake-bpy-module-latest-20230703/bl_ui/properties_data_pointcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-03 06:23:24.000000 fake-bpy-module-latest-20230703/bl_ui/properties_data_shaderfx.py
--rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-07-03 06:23:22.000000 fake-bpy-module-latest-20230703/bl_ui/properties_data_speaker.py
--rw-r--r--   0 runner    (1001) docker     (123)    20178 2023-07-03 06:22:23.000000 fake-bpy-module-latest-20230703/bl_ui/properties_data_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    66640 2023-07-03 06:22:32.000000 fake-bpy-module-latest-20230703/bl_ui/properties_freestyle.py
--rw-r--r--   0 runner    (1001) docker     (123)    32219 2023-07-03 06:23:16.000000 fake-bpy-module-latest-20230703/bl_ui/properties_grease_pencil_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-07-03 06:22:27.000000 fake-bpy-module-latest-20230703/bl_ui/properties_mask_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    30514 2023-07-03 06:23:16.000000 fake-bpy-module-latest-20230703/bl_ui/properties_material.py
--rw-r--r--   0 runner    (1001) docker     (123)    25892 2023-07-03 06:22:26.000000 fake-bpy-module-latest-20230703/bl_ui/properties_material_gpencil.py
--rw-r--r--   0 runner    (1001) docker     (123)    35174 2023-07-03 06:23:19.000000 fake-bpy-module-latest-20230703/bl_ui/properties_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    46745 2023-07-03 06:21:38.000000 fake-bpy-module-latest-20230703/bl_ui/properties_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-07-03 06:23:06.000000 fake-bpy-module-latest-20230703/bl_ui/properties_paint_common.py
--rw-r--r--   0 runner    (1001) docker     (123)   133597 2023-07-03 06:23:22.000000 fake-bpy-module-latest-20230703/bl_ui/properties_particle.py
--rw-r--r--   0 runner    (1001) docker     (123)    36563 2023-07-03 06:23:23.000000 fake-bpy-module-latest-20230703/bl_ui/properties_physics_cloth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-07-03 06:23:05.000000 fake-bpy-module-latest-20230703/bl_ui/properties_physics_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    67584 2023-07-03 06:23:18.000000 fake-bpy-module-latest-20230703/bl_ui/properties_physics_dynamicpaint.py
--rw-r--r--   0 runner    (1001) docker     (123)    27217 2023-07-03 06:22:56.000000 fake-bpy-module-latest-20230703/bl_ui/properties_physics_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    91307 2023-07-03 06:23:08.000000 fake-bpy-module-latest-20230703/bl_ui/properties_physics_fluid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-07-03 06:23:05.000000 fake-bpy-module-latest-20230703/bl_ui/properties_physics_geometry_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-07-03 06:22:55.000000 fake-bpy-module-latest-20230703/bl_ui/properties_physics_rigidbody.py
--rw-r--r--   0 runner    (1001) docker     (123)    33547 2023-07-03 06:23:08.000000 fake-bpy-module-latest-20230703/bl_ui/properties_physics_rigidbody_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    39030 2023-07-03 06:23:06.000000 fake-bpy-module-latest-20230703/bl_ui/properties_physics_softbody.py
--rw-r--r--   0 runner    (1001) docker     (123)    97011 2023-07-03 06:23:04.000000 fake-bpy-module-latest-20230703/bl_ui/properties_render.py
--rw-r--r--   0 runner    (1001) docker     (123)    32886 2023-07-03 06:23:23.000000 fake-bpy-module-latest-20230703/bl_ui/properties_scene.py
--rw-r--r--   0 runner    (1001) docker     (123)    66952 2023-07-03 06:22:34.000000 fake-bpy-module-latest-20230703/bl_ui/properties_texture.py
--rw-r--r--   0 runner    (1001) docker     (123)    37695 2023-07-03 06:23:23.000000 fake-bpy-module-latest-20230703/bl_ui/properties_view_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-07-03 06:22:32.000000 fake-bpy-module-latest-20230703/bl_ui/properties_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-07-03 06:23:06.000000 fake-bpy-module-latest-20230703/bl_ui/properties_world.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 06:14:33.000000 fake-bpy-module-latest-20230703/bl_ui/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   176850 2023-07-03 06:23:01.000000 fake-bpy-module-latest-20230703/bl_ui/space_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    15218 2023-07-03 06:23:01.000000 fake-bpy-module-latest-20230703/bl_ui/space_console.py
--rw-r--r--   0 runner    (1001) docker     (123)    64929 2023-07-03 06:23:05.000000 fake-bpy-module-latest-20230703/bl_ui/space_dopesheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    71853 2023-07-03 06:23:02.000000 fake-bpy-module-latest-20230703/bl_ui/space_filebrowser.py
--rw-r--r--   0 runner    (1001) docker     (123)    50899 2023-07-03 06:23:25.000000 fake-bpy-module-latest-20230703/bl_ui/space_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)   187053 2023-07-03 06:22:49.000000 fake-bpy-module-latest-20230703/bl_ui/space_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    15172 2023-07-03 06:22:33.000000 fake-bpy-module-latest-20230703/bl_ui/space_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    38361 2023-07-03 06:22:46.000000 fake-bpy-module-latest-20230703/bl_ui/space_nla.py
--rw-r--r--   0 runner    (1001) docker     (123)    75065 2023-07-03 06:22:51.000000 fake-bpy-module-latest-20230703/bl_ui/space_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    35830 2023-07-03 06:23:25.000000 fake-bpy-module-latest-20230703/bl_ui/space_outliner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-07-03 06:22:33.000000 fake-bpy-module-latest-20230703/bl_ui/space_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)   182398 2023-07-03 06:22:55.000000 fake-bpy-module-latest-20230703/bl_ui/space_sequencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-03 06:23:23.000000 fake-bpy-module-latest-20230703/bl_ui/space_spreadsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-07-03 06:23:06.000000 fake-bpy-module-latest-20230703/bl_ui/space_statusbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    40008 2023-07-03 06:23:16.000000 fake-bpy-module-latest-20230703/bl_ui/space_text.py
--rw-r--r--   0 runner    (1001) docker     (123)    18254 2023-07-03 06:22:35.000000 fake-bpy-module-latest-20230703/bl_ui/space_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-07-03 06:22:55.000000 fake-bpy-module-latest-20230703/bl_ui/space_toolsystem_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    21636 2023-07-03 06:21:38.000000 fake-bpy-module-latest-20230703/bl_ui/space_toolsystem_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    65863 2023-07-03 06:22:58.000000 fake-bpy-module-latest-20230703/bl_ui/space_topbar.py
--rw-r--r--   0 runner    (1001) docker     (123)   215185 2023-07-03 06:22:31.000000 fake-bpy-module-latest-20230703/bl_ui/space_userpref.py
--rw-r--r--   0 runner    (1001) docker     (123)   624121 2023-07-03 06:22:23.000000 fake-bpy-module-latest-20230703/bl_ui/space_view3d.py
--rw-r--r--   0 runner    (1001) docker     (123)   239548 2023-07-03 06:23:15.000000 fake-bpy-module-latest-20230703/bl_ui/space_view3d_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-03 06:22:26.000000 fake-bpy-module-latest-20230703/bl_ui/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 06:23:33.000000 fake-bpy-module-latest-20230703/bl_ui_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-03 06:21:36.000000 fake-bpy-module-latest-20230703/bl_ui_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-03 06:21:36.000000 fake-bpy-module-latest-20230703/bl_ui_utils/bug_report_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-03 06:21:36.000000 fake-bpy-module-latest-20230703/bl_ui_utils/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 06:14:33.000000 fake-bpy-module-latest-20230703/bl_ui_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-03 06:21:36.000000 fake-bpy-module-latest-20230703/blend_render_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-07-03 06:21:30.000000 fake-bpy-module-latest-20230703/blf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 06:23:33.000000 fake-bpy-module-latest-20230703/bmesh/
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-03 06:21:33.000000 fake-bpy-module-latest-20230703/bmesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-03 06:21:36.000000 fake-bpy-module-latest-20230703/bmesh/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    77492 2023-07-03 06:21:36.000000 fake-bpy-module-latest-20230703/bmesh/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 06:14:33.000000 fake-bpy-module-latest-20230703/bmesh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    36665 2023-07-03 06:21:33.000000 fake-bpy-module-latest-20230703/bmesh/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-07-03 06:21:33.000000 fake-bpy-module-latest-20230703/bmesh/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 06:23:33.000000 fake-bpy-module-latest-20230703/bpy/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-03 06:14:33.000000 fake-bpy-module-latest-20230703/bpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 06:23:33.000000 fake-bpy-module-latest-20230703/bpy/app/
--rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-07-03 06:20:48.000000 fake-bpy-module-latest-20230703/bpy/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-07-03 06:20:48.000000 fake-bpy-module-latest-20230703/bpy/app/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-03 06:20:48.000000 fake-bpy-module-latest-20230703/bpy/app/icons.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 06:14:33.000000 fake-bpy-module-latest-20230703/bpy/app/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-03 06:20:48.000000 fake-bpy-module-latest-20230703/bpy/app/timers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-07-03 06:20:48.000000 fake-bpy-module-latest-20230703/bpy/app/translations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-03 06:21:28.000000 fake-bpy-module-latest-20230703/bpy/msgbus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 06:23:33.000000 fake-bpy-module-latest-20230703/bpy/ops/
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-03 06:20:48.000000 fake-bpy-module-latest-20230703/bpy/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27608 2023-07-03 06:20:57.000000 fake-bpy-module-latest-20230703/bpy/ops/action.py
--rw-r--r--   0 runner    (1001) docker     (123)    35886 2023-07-03 06:21:19.000000 fake-bpy-module-latest-20230703/bpy/ops/anim.py
--rw-r--r--   0 runner    (1001) docker     (123)    25486 2023-07-03 06:21:25.000000 fake-bpy-module-latest-20230703/bpy/ops/armature.py
--rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-07-03 06:20:56.000000 fake-bpy-module-latest-20230703/bpy/ops/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-07-03 06:21:10.000000 fake-bpy-module-latest-20230703/bpy/ops/boid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-07-03 06:20:55.000000 fake-bpy-module-latest-20230703/bpy/ops/brush.py
--rw-r--r--   0 runner    (1001) docker     (123)    12217 2023-07-03 06:21:18.000000 fake-bpy-module-latest-20230703/bpy/ops/buttons.py
--rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-07-03 06:20:55.000000 fake-bpy-module-latest-20230703/bpy/ops/cachefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-03 06:20:52.000000 fake-bpy-module-latest-20230703/bpy/ops/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)    70588 2023-07-03 06:21:11.000000 fake-bpy-module-latest-20230703/bpy/ops/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-03 06:20:56.000000 fake-bpy-module-latest-20230703/bpy/ops/cloth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-07-03 06:21:28.000000 fake-bpy-module-latest-20230703/bpy/ops/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-07-03 06:21:15.000000 fake-bpy-module-latest-20230703/bpy/ops/console.py
--rw-r--r--   0 runner    (1001) docker     (123)    17809 2023-07-03 06:20:56.000000 fake-bpy-module-latest-20230703/bpy/ops/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    40670 2023-07-03 06:21:07.000000 fake-bpy-module-latest-20230703/bpy/ops/curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-07-03 06:21:04.000000 fake-bpy-module-latest-20230703/bpy/ops/curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-07-03 06:21:09.000000 fake-bpy-module-latest-20230703/bpy/ops/cycles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-03 06:21:17.000000 fake-bpy-module-latest-20230703/bpy/ops/dpaint.py
--rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-07-03 06:20:49.000000 fake-bpy-module-latest-20230703/bpy/ops/ed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-07-03 06:21:07.000000 fake-bpy-module-latest-20230703/bpy/ops/export_anim.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-03 06:21:12.000000 fake-bpy-module-latest-20230703/bpy/ops/export_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    35992 2023-07-03 06:20:52.000000 fake-bpy-module-latest-20230703/bpy/ops/export_scene.py
--rw-r--r--   0 runner    (1001) docker     (123)    30339 2023-07-03 06:20:52.000000 fake-bpy-module-latest-20230703/bpy/ops/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-07-03 06:20:56.000000 fake-bpy-module-latest-20230703/bpy/ops/fluid.py
--rw-r--r--   0 runner    (1001) docker     (123)    21051 2023-07-03 06:21:27.000000 fake-bpy-module-latest-20230703/bpy/ops/font.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-07-03 06:21:17.000000 fake-bpy-module-latest-20230703/bpy/ops/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-03 06:21:28.000000 fake-bpy-module-latest-20230703/bpy/ops/gizmogroup.py
--rw-r--r--   0 runner    (1001) docker     (123)   132520 2023-07-03 06:20:54.000000 fake-bpy-module-latest-20230703/bpy/ops/gpencil.py
--rw-r--r--   0 runner    (1001) docker     (123)    50492 2023-07-03 06:21:04.000000 fake-bpy-module-latest-20230703/bpy/ops/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-07-03 06:21:28.000000 fake-bpy-module-latest-20230703/bpy/ops/grease_pencil.py
--rw-r--r--   0 runner    (1001) docker     (123)    53280 2023-07-03 06:21:10.000000 fake-bpy-module-latest-20230703/bpy/ops/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-07-03 06:21:09.000000 fake-bpy-module-latest-20230703/bpy/ops/import_anim.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-03 06:21:19.000000 fake-bpy-module-latest-20230703/bpy/ops/import_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-03 06:20:59.000000 fake-bpy-module-latest-20230703/bpy/ops/import_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    11561 2023-07-03 06:21:16.000000 fake-bpy-module-latest-20230703/bpy/ops/import_scene.py
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-07-03 06:21:09.000000 fake-bpy-module-latest-20230703/bpy/ops/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-07-03 06:20:56.000000 fake-bpy-module-latest-20230703/bpy/ops/lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-07-03 06:21:12.000000 fake-bpy-module-latest-20230703/bpy/ops/marker.py
--rw-r--r--   0 runner    (1001) docker     (123)    27162 2023-07-03 06:21:15.000000 fake-bpy-module-latest-20230703/bpy/ops/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-03 06:21:28.000000 fake-bpy-module-latest-20230703/bpy/ops/material.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-07-03 06:21:26.000000 fake-bpy-module-latest-20230703/bpy/ops/mball.py
--rw-r--r--   0 runner    (1001) docker     (123)   179170 2023-07-03 06:21:15.000000 fake-bpy-module-latest-20230703/bpy/ops/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    28694 2023-07-03 06:20:56.000000 fake-bpy-module-latest-20230703/bpy/ops/nla.py
--rw-r--r--   0 runner    (1001) docker     (123)    72286 2023-07-03 06:21:05.000000 fake-bpy-module-latest-20230703/bpy/ops/node.py
--rw-r--r--   0 runner    (1001) docker     (123)   226228 2023-07-03 06:21:04.000000 fake-bpy-module-latest-20230703/bpy/ops/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    44201 2023-07-03 06:21:17.000000 fake-bpy-module-latest-20230703/bpy/ops/outliner.py
--rw-r--r--   0 runner    (1001) docker     (123)    44093 2023-07-03 06:21:16.000000 fake-bpy-module-latest-20230703/bpy/ops/paint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-07-03 06:21:05.000000 fake-bpy-module-latest-20230703/bpy/ops/paintcurve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-07-03 06:21:26.000000 fake-bpy-module-latest-20230703/bpy/ops/palette.py
--rw-r--r--   0 runner    (1001) docker     (123)    22863 2023-07-03 06:20:48.000000 fake-bpy-module-latest-20230703/bpy/ops/particle.py
--rw-r--r--   0 runner    (1001) docker     (123)    39854 2023-07-03 06:21:27.000000 fake-bpy-module-latest-20230703/bpy/ops/pose.py
--rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-07-03 06:21:09.000000 fake-bpy-module-latest-20230703/bpy/ops/poselib.py
--rw-r--r--   0 runner    (1001) docker     (123)    32889 2023-07-03 06:21:12.000000 fake-bpy-module-latest-20230703/bpy/ops/preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-03 06:21:00.000000 fake-bpy-module-latest-20230703/bpy/ops/ptcache.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 06:14:33.000000 fake-bpy-module-latest-20230703/bpy/ops/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-07-03 06:21:00.000000 fake-bpy-module-latest-20230703/bpy/ops/render.py
--rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-07-03 06:21:01.000000 fake-bpy-module-latest-20230703/bpy/ops/rigidbody.py
--rw-r--r--   0 runner    (1001) docker     (123)    25220 2023-07-03 06:21:26.000000 fake-bpy-module-latest-20230703/bpy/ops/scene.py
--rw-r--r--   0 runner    (1001) docker     (123)    31884 2023-07-03 06:21:26.000000 fake-bpy-module-latest-20230703/bpy/ops/screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-03 06:21:28.000000 fake-bpy-module-latest-20230703/bpy/ops/script.py
--rw-r--r--   0 runner    (1001) docker     (123)    46889 2023-07-03 06:21:18.000000 fake-bpy-module-latest-20230703/bpy/ops/sculpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-03 06:20:59.000000 fake-bpy-module-latest-20230703/bpy/ops/sculpt_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)    94657 2023-07-03 06:21:09.000000 fake-bpy-module-latest-20230703/bpy/ops/sequencer.py
--rw-r--r--   0 runner    (1001) docker     (123)    19928 2023-07-03 06:20:55.000000 fake-bpy-module-latest-20230703/bpy/ops/sound.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-03 06:21:09.000000 fake-bpy-module-latest-20230703/bpy/ops/spreadsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-07-03 06:20:55.000000 fake-bpy-module-latest-20230703/bpy/ops/surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    32954 2023-07-03 06:20:59.000000 fake-bpy-module-latest-20230703/bpy/ops/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-03 06:21:04.000000 fake-bpy-module-latest-20230703/bpy/ops/text_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-03 06:20:54.000000 fake-bpy-module-latest-20230703/bpy/ops/texture.py
--rw-r--r--   0 runner    (1001) docker     (123)    70745 2023-07-03 06:20:58.000000 fake-bpy-module-latest-20230703/bpy/ops/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    19753 2023-07-03 06:21:18.000000 fake-bpy-module-latest-20230703/bpy/ops/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-07-03 06:21:26.000000 fake-bpy-module-latest-20230703/bpy/ops/uilist.py
--rw-r--r--   0 runner    (1001) docker     (123)    57277 2023-07-03 06:21:00.000000 fake-bpy-module-latest-20230703/bpy/ops/uv.py
--rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-07-03 06:21:27.000000 fake-bpy-module-latest-20230703/bpy/ops/view2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    54854 2023-07-03 06:21:07.000000 fake-bpy-module-latest-20230703/bpy/ops/view3d.py
--rw-r--r--   0 runner    (1001) docker     (123)   246250 2023-07-03 06:21:25.000000 fake-bpy-module-latest-20230703/bpy/ops/wm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-07-03 06:21:15.000000 fake-bpy-module-latest-20230703/bpy/ops/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-03 06:21:28.000000 fake-bpy-module-latest-20230703/bpy/ops/world.py
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-07-03 06:21:28.000000 fake-bpy-module-latest-20230703/bpy/path.py
--rw-r--r--   0 runner    (1001) docker     (123)    29417 2023-07-03 06:21:28.000000 fake-bpy-module-latest-20230703/bpy/props.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 06:14:33.000000 fake-bpy-module-latest-20230703/bpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)  3497859 2023-07-03 06:20:48.000000 fake-bpy-module-latest-20230703/bpy/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 06:23:33.000000 fake-bpy-module-latest-20230703/bpy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-07-03 06:21:28.000000 fake-bpy-module-latest-20230703/bpy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-07-03 06:21:28.000000 fake-bpy-module-latest-20230703/bpy/utils/previews.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 06:14:33.000000 fake-bpy-module-latest-20230703/bpy/utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-07-03 06:21:28.000000 fake-bpy-module-latest-20230703/bpy/utils/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 06:23:33.000000 fake-bpy-module-latest-20230703/bpy_extras/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-03 06:21:33.000000 fake-bpy-module-latest-20230703/bpy_extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-07-03 06:21:33.000000 fake-bpy-module-latest-20230703/bpy_extras/anim_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-03 06:21:33.000000 fake-bpy-module-latest-20230703/bpy_extras/asset_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-03 06:21:33.000000 fake-bpy-module-latest-20230703/bpy_extras/bmesh_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-03 06:21:33.000000 fake-bpy-module-latest-20230703/bpy_extras/id_map_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-07-03 06:21:33.000000 fake-bpy-module-latest-20230703/bpy_extras/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-07-03 06:21:33.000000 fake-bpy-module-latest-20230703/bpy_extras/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-03 06:21:33.000000 fake-bpy-module-latest-20230703/bpy_extras/keyconfig_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-07-03 06:21:33.000000 fake-bpy-module-latest-20230703/bpy_extras/mesh_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-07-03 06:21:33.000000 fake-bpy-module-latest-20230703/bpy_extras/node_shader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-03 06:21:33.000000 fake-bpy-module-latest-20230703/bpy_extras/node_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-03 06:21:33.000000 fake-bpy-module-latest-20230703/bpy_extras/object_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 06:14:33.000000 fake-bpy-module-latest-20230703/bpy_extras/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-07-03 06:21:33.000000 fake-bpy-module-latest-20230703/bpy_extras/view3d_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 06:23:33.000000 fake-bpy-module-latest-20230703/bpy_extras/wm_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-03 06:21:33.000000 fake-bpy-module-latest-20230703/bpy_extras/wm_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-03 06:21:33.000000 fake-bpy-module-latest-20230703/bpy_extras/wm_utils/progress_report.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 06:14:33.000000 fake-bpy-module-latest-20230703/bpy_extras/wm_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-03 06:21:36.000000 fake-bpy-module-latest-20230703/bpy_restrict_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    54167 2023-07-03 06:21:37.000000 fake-bpy-module-latest-20230703/bpy_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-03 06:21:36.000000 fake-bpy-module-latest-20230703/console_python.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-03 06:23:31.000000 fake-bpy-module-latest-20230703/console_shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 06:23:33.000000 fake-bpy-module-latest-20230703/fake_bpy_module_latest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-07-03 06:23:33.000000 fake-bpy-module-latest-20230703/fake_bpy_module_latest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-07-03 06:23:33.000000 fake-bpy-module-latest-20230703/fake_bpy_module_latest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 06:23:33.000000 fake-bpy-module-latest-20230703/fake_bpy_module_latest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 06:23:33.000000 fake-bpy-module-latest-20230703/fake_bpy_module_latest.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-03 06:23:33.000000 fake-bpy-module-latest-20230703/fake_bpy_module_latest.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 06:23:33.000000 fake-bpy-module-latest-20230703/freestyle/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-03 06:21:32.000000 fake-bpy-module-latest-20230703/freestyle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-07-03 06:21:33.000000 fake-bpy-module-latest-20230703/freestyle/chainingiterators.py
--rw-r--r--   0 runner    (1001) docker     (123)    47908 2023-07-03 06:21:32.000000 fake-bpy-module-latest-20230703/freestyle/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13232 2023-07-03 06:21:32.000000 fake-bpy-module-latest-20230703/freestyle/predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 06:14:33.000000 fake-bpy-module-latest-20230703/freestyle/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23737 2023-07-03 06:21:33.000000 fake-bpy-module-latest-20230703/freestyle/shaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    86403 2023-07-03 06:21:32.000000 fake-bpy-module-latest-20230703/freestyle/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 06:23:33.000000 fake-bpy-module-latest-20230703/freestyle/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-03 06:21:32.000000 fake-bpy-module-latest-20230703/freestyle/utils/ContextFunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-07-03 06:21:32.000000 fake-bpy-module-latest-20230703/freestyle/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 06:14:33.000000 fake-bpy-module-latest-20230703/freestyle/utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 06:23:33.000000 fake-bpy-module-latest-20230703/gpu/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-03 06:21:32.000000 fake-bpy-module-latest-20230703/gpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-07-03 06:21:32.000000 fake-bpy-module-latest-20230703/gpu/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-03 06:21:32.000000 fake-bpy-module-latest-20230703/gpu/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-03 06:21:32.000000 fake-bpy-module-latest-20230703/gpu/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 06:14:33.000000 fake-bpy-module-latest-20230703/gpu/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-03 06:21:32.000000 fake-bpy-module-latest-20230703/gpu/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-03 06:21:32.000000 fake-bpy-module-latest-20230703/gpu/shader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-07-03 06:21:32.000000 fake-bpy-module-latest-20230703/gpu/state.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-03 06:21:32.000000 fake-bpy-module-latest-20230703/gpu/texture.py
--rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-07-03 06:21:32.000000 fake-bpy-module-latest-20230703/gpu/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 06:23:33.000000 fake-bpy-module-latest-20230703/gpu_extras/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-03 06:21:32.000000 fake-bpy-module-latest-20230703/gpu_extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-03 06:21:32.000000 fake-bpy-module-latest-20230703/gpu_extras/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-03 06:21:32.000000 fake-bpy-module-latest-20230703/gpu_extras/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 06:14:33.000000 fake-bpy-module-latest-20230703/gpu_extras/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-03 06:23:31.000000 fake-bpy-module-latest-20230703/graphviz_export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 06:23:33.000000 fake-bpy-module-latest-20230703/idprop/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-03 06:21:36.000000 fake-bpy-module-latest-20230703/idprop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 06:14:33.000000 fake-bpy-module-latest-20230703/idprop/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-03 06:21:36.000000 fake-bpy-module-latest-20230703/idprop/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 06:23:33.000000 fake-bpy-module-latest-20230703/imbuf/
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-03 06:21:36.000000 fake-bpy-module-latest-20230703/imbuf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 06:14:33.000000 fake-bpy-module-latest-20230703/imbuf/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-03 06:21:36.000000 fake-bpy-module-latest-20230703/imbuf/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    48637 2023-07-03 06:21:37.000000 fake-bpy-module-latest-20230703/keyingsets_builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-03 06:23:31.000000 fake-bpy-module-latest-20230703/keyingsets_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 06:23:33.000000 fake-bpy-module-latest-20230703/mathutils/
--rw-r--r--   0 runner    (1001) docker     (123)    86215 2023-07-03 06:21:31.000000 fake-bpy-module-latest-20230703/mathutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-07-03 06:21:31.000000 fake-bpy-module-latest-20230703/mathutils/bvhtree.py
--rw-r--r--   0 runner    (1001) docker     (123)    22187 2023-07-03 06:21:32.000000 fake-bpy-module-latest-20230703/mathutils/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-03 06:21:31.000000 fake-bpy-module-latest-20230703/mathutils/interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-07-03 06:21:31.000000 fake-bpy-module-latest-20230703/mathutils/kdtree.py
--rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-07-03 06:21:31.000000 fake-bpy-module-latest-20230703/mathutils/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 06:14:33.000000 fake-bpy-module-latest-20230703/mathutils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-03 06:23:25.000000 fake-bpy-module-latest-20230703/nodeitems_builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-03 06:23:31.000000 fake-bpy-module-latest-20230703/nodeitems_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-07-03 06:21:36.000000 fake-bpy-module-latest-20230703/rna_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-03 06:21:36.000000 fake-bpy-module-latest-20230703/rna_keymap_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-03 06:21:36.000000 fake-bpy-module-latest-20230703/rna_prop_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-03 06:23:31.000000 fake-bpy-module-latest-20230703/rna_xml.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 06:23:33.000000 fake-bpy-module-latest-20230703/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-03 06:23:32.000000 fake-bpy-module-latest-20230703/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-03 06:21:36.000000 fake-bpy-module-latest-20230703/sys_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:27:34.000000 fake-bpy-module-latest-20230704/
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-07-04 06:27:34.000000 fake-bpy-module-latest-20230704/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-07-04 06:27:33.000000 fake-bpy-module-latest-20230704/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-04 06:27:23.000000 fake-bpy-module-latest-20230704/addon_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-04 06:27:23.000000 fake-bpy-module-latest-20230704/animsys_refactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30417 2023-07-04 06:24:50.000000 fake-bpy-module-latest-20230704/aud.py
+-rw-r--r--   0 runner    (1001) docker     (123)   116266 2023-07-04 06:24:47.000000 fake-bpy-module-latest-20230704/bgl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:27:34.000000 fake-bpy-module-latest-20230704/bl_app_override/
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-04 06:27:23.000000 fake-bpy-module-latest-20230704/bl_app_override/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-04 06:27:23.000000 fake-bpy-module-latest-20230704/bl_app_override/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:15:22.000000 fake-bpy-module-latest-20230704/bl_app_override/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-04 06:27:24.000000 fake-bpy-module-latest-20230704/bl_app_template_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:27:34.000000 fake-bpy-module-latest-20230704/bl_console_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-04 06:24:53.000000 fake-bpy-module-latest-20230704/bl_console_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:27:34.000000 fake-bpy-module-latest-20230704/bl_console_utils/autocomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-04 06:24:53.000000 fake-bpy-module-latest-20230704/bl_console_utils/autocomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-04 06:24:53.000000 fake-bpy-module-latest-20230704/bl_console_utils/autocomplete/complete_calltip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-04 06:24:53.000000 fake-bpy-module-latest-20230704/bl_console_utils/autocomplete/complete_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-04 06:24:53.000000 fake-bpy-module-latest-20230704/bl_console_utils/autocomplete/complete_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-04 06:24:54.000000 fake-bpy-module-latest-20230704/bl_console_utils/autocomplete/intellisense.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:15:22.000000 fake-bpy-module-latest-20230704/bl_console_utils/autocomplete/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:15:22.000000 fake-bpy-module-latest-20230704/bl_console_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:27:34.000000 fake-bpy-module-latest-20230704/bl_i18n_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-04 06:27:33.000000 fake-bpy-module-latest-20230704/bl_i18n_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-04 06:27:33.000000 fake-bpy-module-latest-20230704/bl_i18n_utils/bl_extract_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-04 06:27:33.000000 fake-bpy-module-latest-20230704/bl_i18n_utils/merge_po.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:15:22.000000 fake-bpy-module-latest-20230704/bl_i18n_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-04 06:27:33.000000 fake-bpy-module-latest-20230704/bl_i18n_utils/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-07-04 06:27:33.000000 fake-bpy-module-latest-20230704/bl_i18n_utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-04 06:27:33.000000 fake-bpy-module-latest-20230704/bl_i18n_utils/utils_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 06:27:33.000000 fake-bpy-module-latest-20230704/bl_i18n_utils/utils_languages_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-04 06:27:33.000000 fake-bpy-module-latest-20230704/bl_i18n_utils/utils_rtl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:27:34.000000 fake-bpy-module-latest-20230704/bl_keymap_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-04 06:27:24.000000 fake-bpy-module-latest-20230704/bl_keymap_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-04 06:27:24.000000 fake-bpy-module-latest-20230704/bl_keymap_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-04 06:27:24.000000 fake-bpy-module-latest-20230704/bl_keymap_utils/keymap_from_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-04 06:27:24.000000 fake-bpy-module-latest-20230704/bl_keymap_utils/keymap_hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-04 06:27:24.000000 fake-bpy-module-latest-20230704/bl_keymap_utils/platform_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:15:22.000000 fake-bpy-module-latest-20230704/bl_keymap_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-04 06:27:24.000000 fake-bpy-module-latest-20230704/bl_keymap_utils/versioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-04 06:24:53.000000 fake-bpy-module-latest-20230704/bl_math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:27:34.000000 fake-bpy-module-latest-20230704/bl_operators/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-04 06:27:24.000000 fake-bpy-module-latest-20230704/bl_operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-04 06:27:29.000000 fake-bpy-module-latest-20230704/bl_operators/add_mesh_torus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-07-04 06:27:30.000000 fake-bpy-module-latest-20230704/bl_operators/anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-04 06:27:27.000000 fake-bpy-module-latest-20230704/bl_operators/assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:27:34.000000 fake-bpy-module-latest-20230704/bl_operators/bmesh/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-04 06:27:28.000000 fake-bpy-module-latest-20230704/bl_operators/bmesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-04 06:27:28.000000 fake-bpy-module-latest-20230704/bl_operators/bmesh/find_adjacent.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:15:22.000000 fake-bpy-module-latest-20230704/bl_operators/bmesh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22556 2023-07-04 06:27:29.000000 fake-bpy-module-latest-20230704/bl_operators/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-07-04 06:27:29.000000 fake-bpy-module-latest-20230704/bl_operators/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-07-04 06:27:27.000000 fake-bpy-module-latest-20230704/bl_operators/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-07-04 06:27:31.000000 fake-bpy-module-latest-20230704/bl_operators/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-07-04 06:27:29.000000 fake-bpy-module-latest-20230704/bl_operators/freestyle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15010 2023-07-04 06:27:30.000000 fake-bpy-module-latest-20230704/bl_operators/geometry_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-07-04 06:27:32.000000 fake-bpy-module-latest-20230704/bl_operators/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-07-04 06:27:29.000000 fake-bpy-module-latest-20230704/bl_operators/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18689 2023-07-04 06:27:31.000000 fake-bpy-module-latest-20230704/bl_operators/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38122 2023-07-04 06:27:31.000000 fake-bpy-module-latest-20230704/bl_operators/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-07-04 06:27:31.000000 fake-bpy-module-latest-20230704/bl_operators/object_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-07-04 06:27:28.000000 fake-bpy-module-latest-20230704/bl_operators/object_quick_effects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-04 06:27:30.000000 fake-bpy-module-latest-20230704/bl_operators/object_randomize_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45483 2023-07-04 06:27:27.000000 fake-bpy-module-latest-20230704/bl_operators/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:15:22.000000 fake-bpy-module-latest-20230704/bl_operators/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-07-04 06:27:32.000000 fake-bpy-module-latest-20230704/bl_operators/rigidbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-04 06:27:27.000000 fake-bpy-module-latest-20230704/bl_operators/screen_play_rendered_anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-07-04 06:27:30.000000 fake-bpy-module-latest-20230704/bl_operators/sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-07-04 06:27:28.000000 fake-bpy-module-latest-20230704/bl_operators/spreadsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-04 06:27:31.000000 fake-bpy-module-latest-20230704/bl_operators/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56119 2023-07-04 06:27:28.000000 fake-bpy-module-latest-20230704/bl_operators/userpref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-07-04 06:27:28.000000 fake-bpy-module-latest-20230704/bl_operators/uvcalc_follow_active.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-07-04 06:27:29.000000 fake-bpy-module-latest-20230704/bl_operators/uvcalc_lightmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-07-04 06:27:30.000000 fake-bpy-module-latest-20230704/bl_operators/uvcalc_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-07-04 06:27:29.000000 fake-bpy-module-latest-20230704/bl_operators/vertexpaint_dirt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11529 2023-07-04 06:27:32.000000 fake-bpy-module-latest-20230704/bl_operators/view3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97916 2023-07-04 06:27:27.000000 fake-bpy-module-latest-20230704/bl_operators/wm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:27:34.000000 fake-bpy-module-latest-20230704/bl_previews_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-04 06:27:24.000000 fake-bpy-module-latest-20230704/bl_previews_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-04 06:27:24.000000 fake-bpy-module-latest-20230704/bl_previews_utils/bl_previews_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:15:22.000000 fake-bpy-module-latest-20230704/bl_previews_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:27:34.000000 fake-bpy-module-latest-20230704/bl_rna_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-04 06:27:24.000000 fake-bpy-module-latest-20230704/bl_rna_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-04 06:27:24.000000 fake-bpy-module-latest-20230704/bl_rna_utils/data_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:15:22.000000 fake-bpy-module-latest-20230704/bl_rna_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:27:34.000000 fake-bpy-module-latest-20230704/bl_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-07-04 06:24:54.000000 fake-bpy-module-latest-20230704/bl_ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-07-04 06:27:00.000000 fake-bpy-module-latest-20230704/bl_ui/generic_ui_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-04 06:26:59.000000 fake-bpy-module-latest-20230704/bl_ui/node_add_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110864 2023-07-04 06:26:37.000000 fake-bpy-module-latest-20230704/bl_ui/node_add_menu_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-04 06:26:29.000000 fake-bpy-module-latest-20230704/bl_ui/properties_animviz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-07-04 06:27:09.000000 fake-bpy-module-latest-20230704/bl_ui/properties_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)   385296 2023-07-04 06:26:20.000000 fake-bpy-module-latest-20230704/bl_ui/properties_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25330 2023-07-04 06:26:55.000000 fake-bpy-module-latest-20230704/bl_ui/properties_data_armature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22602 2023-07-04 06:24:56.000000 fake-bpy-module-latest-20230704/bl_ui/properties_data_bone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36945 2023-07-04 06:26:26.000000 fake-bpy-module-latest-20230704/bl_ui/properties_data_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38857 2023-07-04 06:25:00.000000 fake-bpy-module-latest-20230704/bl_ui/properties_data_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15423 2023-07-04 06:26:25.000000 fake-bpy-module-latest-20230704/bl_ui/properties_data_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-07-04 06:27:15.000000 fake-bpy-module-latest-20230704/bl_ui/properties_data_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46403 2023-07-04 06:26:56.000000 fake-bpy-module-latest-20230704/bl_ui/properties_data_gpencil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-07-04 06:27:00.000000 fake-bpy-module-latest-20230704/bl_ui/properties_data_grease_pencil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-07-04 06:24:54.000000 fake-bpy-module-latest-20230704/bl_ui/properties_data_lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-07-04 06:26:29.000000 fake-bpy-module-latest-20230704/bl_ui/properties_data_light.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15425 2023-07-04 06:26:21.000000 fake-bpy-module-latest-20230704/bl_ui/properties_data_lightprobe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52746 2023-07-04 06:27:02.000000 fake-bpy-module-latest-20230704/bl_ui/properties_data_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-07-04 06:27:15.000000 fake-bpy-module-latest-20230704/bl_ui/properties_data_metaball.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-07-04 06:27:21.000000 fake-bpy-module-latest-20230704/bl_ui/properties_data_modifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-07-04 06:27:05.000000 fake-bpy-module-latest-20230704/bl_ui/properties_data_pointcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-04 06:26:25.000000 fake-bpy-module-latest-20230704/bl_ui/properties_data_shaderfx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-07-04 06:27:05.000000 fake-bpy-module-latest-20230704/bl_ui/properties_data_speaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20178 2023-07-04 06:26:27.000000 fake-bpy-module-latest-20230704/bl_ui/properties_data_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66640 2023-07-04 06:26:28.000000 fake-bpy-module-latest-20230704/bl_ui/properties_freestyle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32219 2023-07-04 06:25:00.000000 fake-bpy-module-latest-20230704/bl_ui/properties_grease_pencil_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-07-04 06:26:27.000000 fake-bpy-module-latest-20230704/bl_ui/properties_mask_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30514 2023-07-04 06:24:55.000000 fake-bpy-module-latest-20230704/bl_ui/properties_material.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25892 2023-07-04 06:27:01.000000 fake-bpy-module-latest-20230704/bl_ui/properties_material_gpencil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35174 2023-07-04 06:26:25.000000 fake-bpy-module-latest-20230704/bl_ui/properties_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46745 2023-07-04 06:27:01.000000 fake-bpy-module-latest-20230704/bl_ui/properties_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-07-04 06:26:24.000000 fake-bpy-module-latest-20230704/bl_ui/properties_paint_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)   133597 2023-07-04 06:24:59.000000 fake-bpy-module-latest-20230704/bl_ui/properties_particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36563 2023-07-04 06:26:57.000000 fake-bpy-module-latest-20230704/bl_ui/properties_physics_cloth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-07-04 06:26:59.000000 fake-bpy-module-latest-20230704/bl_ui/properties_physics_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67584 2023-07-04 06:27:08.000000 fake-bpy-module-latest-20230704/bl_ui/properties_physics_dynamicpaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27217 2023-07-04 06:27:05.000000 fake-bpy-module-latest-20230704/bl_ui/properties_physics_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91307 2023-07-04 06:27:04.000000 fake-bpy-module-latest-20230704/bl_ui/properties_physics_fluid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-07-04 06:27:21.000000 fake-bpy-module-latest-20230704/bl_ui/properties_physics_geometry_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-07-04 06:26:34.000000 fake-bpy-module-latest-20230704/bl_ui/properties_physics_rigidbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33547 2023-07-04 06:26:58.000000 fake-bpy-module-latest-20230704/bl_ui/properties_physics_rigidbody_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39030 2023-07-04 06:27:00.000000 fake-bpy-module-latest-20230704/bl_ui/properties_physics_softbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97011 2023-07-04 06:27:23.000000 fake-bpy-module-latest-20230704/bl_ui/properties_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32886 2023-07-04 06:24:55.000000 fake-bpy-module-latest-20230704/bl_ui/properties_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66952 2023-07-04 06:27:09.000000 fake-bpy-module-latest-20230704/bl_ui/properties_texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37695 2023-07-04 06:26:25.000000 fake-bpy-module-latest-20230704/bl_ui/properties_view_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-07-04 06:27:05.000000 fake-bpy-module-latest-20230704/bl_ui/properties_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-07-04 06:26:57.000000 fake-bpy-module-latest-20230704/bl_ui/properties_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:15:22.000000 fake-bpy-module-latest-20230704/bl_ui/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   176850 2023-07-04 06:27:14.000000 fake-bpy-module-latest-20230704/bl_ui/space_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15218 2023-07-04 06:24:54.000000 fake-bpy-module-latest-20230704/bl_ui/space_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64929 2023-07-04 06:26:22.000000 fake-bpy-module-latest-20230704/bl_ui/space_dopesheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71853 2023-07-04 06:26:59.000000 fake-bpy-module-latest-20230704/bl_ui/space_filebrowser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50899 2023-07-04 06:26:05.000000 fake-bpy-module-latest-20230704/bl_ui/space_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)   187053 2023-07-04 06:26:34.000000 fake-bpy-module-latest-20230704/bl_ui/space_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15172 2023-07-04 06:27:15.000000 fake-bpy-module-latest-20230704/bl_ui/space_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38361 2023-07-04 06:26:24.000000 fake-bpy-module-latest-20230704/bl_ui/space_nla.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75065 2023-07-04 06:27:07.000000 fake-bpy-module-latest-20230704/bl_ui/space_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35830 2023-07-04 06:26:38.000000 fake-bpy-module-latest-20230704/bl_ui/space_outliner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-07-04 06:26:29.000000 fake-bpy-module-latest-20230704/bl_ui/space_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)   182398 2023-07-04 06:27:21.000000 fake-bpy-module-latest-20230704/bl_ui/space_sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-04 06:27:02.000000 fake-bpy-module-latest-20230704/bl_ui/space_spreadsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-07-04 06:27:09.000000 fake-bpy-module-latest-20230704/bl_ui/space_statusbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40008 2023-07-04 06:26:23.000000 fake-bpy-module-latest-20230704/bl_ui/space_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18254 2023-07-04 06:26:54.000000 fake-bpy-module-latest-20230704/bl_ui/space_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-07-04 06:24:54.000000 fake-bpy-module-latest-20230704/bl_ui/space_toolsystem_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21699 2023-07-04 06:27:15.000000 fake-bpy-module-latest-20230704/bl_ui/space_toolsystem_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65863 2023-07-04 06:26:38.000000 fake-bpy-module-latest-20230704/bl_ui/space_topbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)   215185 2023-07-04 06:26:44.000000 fake-bpy-module-latest-20230704/bl_ui/space_userpref.py
+-rw-r--r--   0 runner    (1001) docker     (123)   626694 2023-07-04 06:26:04.000000 fake-bpy-module-latest-20230704/bl_ui/space_view3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)   239548 2023-07-04 06:26:54.000000 fake-bpy-module-latest-20230704/bl_ui/space_view3d_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-04 06:26:58.000000 fake-bpy-module-latest-20230704/bl_ui/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:27:34.000000 fake-bpy-module-latest-20230704/bl_ui_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-04 06:24:53.000000 fake-bpy-module-latest-20230704/bl_ui_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-04 06:24:53.000000 fake-bpy-module-latest-20230704/bl_ui_utils/bug_report_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-04 06:24:53.000000 fake-bpy-module-latest-20230704/bl_ui_utils/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:15:22.000000 fake-bpy-module-latest-20230704/bl_ui_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-04 06:27:24.000000 fake-bpy-module-latest-20230704/blend_render_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-07-04 06:24:47.000000 fake-bpy-module-latest-20230704/blf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:27:34.000000 fake-bpy-module-latest-20230704/bmesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-04 06:24:50.000000 fake-bpy-module-latest-20230704/bmesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-04 06:24:53.000000 fake-bpy-module-latest-20230704/bmesh/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77492 2023-07-04 06:24:53.000000 fake-bpy-module-latest-20230704/bmesh/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:15:22.000000 fake-bpy-module-latest-20230704/bmesh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    36665 2023-07-04 06:24:51.000000 fake-bpy-module-latest-20230704/bmesh/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-07-04 06:24:51.000000 fake-bpy-module-latest-20230704/bmesh/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:27:34.000000 fake-bpy-module-latest-20230704/bpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-04 06:15:22.000000 fake-bpy-module-latest-20230704/bpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:27:34.000000 fake-bpy-module-latest-20230704/bpy/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-07-04 06:24:44.000000 fake-bpy-module-latest-20230704/bpy/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-07-04 06:24:44.000000 fake-bpy-module-latest-20230704/bpy/app/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-04 06:24:44.000000 fake-bpy-module-latest-20230704/bpy/app/icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:15:22.000000 fake-bpy-module-latest-20230704/bpy/app/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-04 06:24:44.000000 fake-bpy-module-latest-20230704/bpy/app/timers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-07-04 06:24:44.000000 fake-bpy-module-latest-20230704/bpy/app/translations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-04 06:24:44.000000 fake-bpy-module-latest-20230704/bpy/msgbus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:27:34.000000 fake-bpy-module-latest-20230704/bpy/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-04 06:23:53.000000 fake-bpy-module-latest-20230704/bpy/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27608 2023-07-04 06:24:30.000000 fake-bpy-module-latest-20230704/bpy/ops/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35886 2023-07-04 06:24:11.000000 fake-bpy-module-latest-20230704/bpy/ops/anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25486 2023-07-04 06:24:05.000000 fake-bpy-module-latest-20230704/bpy/ops/armature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-07-04 06:23:58.000000 fake-bpy-module-latest-20230704/bpy/ops/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-07-04 06:24:29.000000 fake-bpy-module-latest-20230704/bpy/ops/boid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-07-04 06:23:58.000000 fake-bpy-module-latest-20230704/bpy/ops/brush.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12217 2023-07-04 06:24:06.000000 fake-bpy-module-latest-20230704/bpy/ops/buttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-07-04 06:24:43.000000 fake-bpy-module-latest-20230704/bpy/ops/cachefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-04 06:24:29.000000 fake-bpy-module-latest-20230704/bpy/ops/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70588 2023-07-04 06:24:20.000000 fake-bpy-module-latest-20230704/bpy/ops/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-04 06:23:59.000000 fake-bpy-module-latest-20230704/bpy/ops/cloth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-07-04 06:24:30.000000 fake-bpy-module-latest-20230704/bpy/ops/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-07-04 06:24:42.000000 fake-bpy-module-latest-20230704/bpy/ops/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17809 2023-07-04 06:24:33.000000 fake-bpy-module-latest-20230704/bpy/ops/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40670 2023-07-04 06:24:19.000000 fake-bpy-module-latest-20230704/bpy/ops/curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-07-04 06:23:58.000000 fake-bpy-module-latest-20230704/bpy/ops/curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-07-04 06:24:34.000000 fake-bpy-module-latest-20230704/bpy/ops/cycles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-04 06:24:10.000000 fake-bpy-module-latest-20230704/bpy/ops/dpaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-07-04 06:24:29.000000 fake-bpy-module-latest-20230704/bpy/ops/ed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-07-04 06:24:05.000000 fake-bpy-module-latest-20230704/bpy/ops/export_anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-04 06:24:05.000000 fake-bpy-module-latest-20230704/bpy/ops/export_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35992 2023-07-04 06:24:09.000000 fake-bpy-module-latest-20230704/bpy/ops/export_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30339 2023-07-04 06:24:35.000000 fake-bpy-module-latest-20230704/bpy/ops/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-07-04 06:23:59.000000 fake-bpy-module-latest-20230704/bpy/ops/fluid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21051 2023-07-04 06:24:21.000000 fake-bpy-module-latest-20230704/bpy/ops/font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-07-04 06:24:30.000000 fake-bpy-module-latest-20230704/bpy/ops/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-04 06:24:15.000000 fake-bpy-module-latest-20230704/bpy/ops/gizmogroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)   132520 2023-07-04 06:24:01.000000 fake-bpy-module-latest-20230704/bpy/ops/gpencil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50492 2023-07-04 06:24:34.000000 fake-bpy-module-latest-20230704/bpy/ops/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-07-04 06:24:05.000000 fake-bpy-module-latest-20230704/bpy/ops/grease_pencil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53280 2023-07-04 06:24:10.000000 fake-bpy-module-latest-20230704/bpy/ops/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-07-04 06:24:29.000000 fake-bpy-module-latest-20230704/bpy/ops/import_anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-04 06:24:41.000000 fake-bpy-module-latest-20230704/bpy/ops/import_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-04 06:24:16.000000 fake-bpy-module-latest-20230704/bpy/ops/import_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11561 2023-07-04 06:24:16.000000 fake-bpy-module-latest-20230704/bpy/ops/import_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-07-04 06:24:43.000000 fake-bpy-module-latest-20230704/bpy/ops/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-07-04 06:23:59.000000 fake-bpy-module-latest-20230704/bpy/ops/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-07-04 06:24:39.000000 fake-bpy-module-latest-20230704/bpy/ops/marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27162 2023-07-04 06:24:13.000000 fake-bpy-module-latest-20230704/bpy/ops/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-04 06:24:21.000000 fake-bpy-module-latest-20230704/bpy/ops/material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-07-04 06:24:33.000000 fake-bpy-module-latest-20230704/bpy/ops/mball.py
+-rw-r--r--   0 runner    (1001) docker     (123)   179170 2023-07-04 06:24:38.000000 fake-bpy-module-latest-20230704/bpy/ops/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28694 2023-07-04 06:24:33.000000 fake-bpy-module-latest-20230704/bpy/ops/nla.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72286 2023-07-04 06:24:18.000000 fake-bpy-module-latest-20230704/bpy/ops/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)   226228 2023-07-04 06:23:58.000000 fake-bpy-module-latest-20230704/bpy/ops/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44201 2023-07-04 06:24:06.000000 fake-bpy-module-latest-20230704/bpy/ops/outliner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44093 2023-07-04 06:24:14.000000 fake-bpy-module-latest-20230704/bpy/ops/paint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-07-04 06:24:32.000000 fake-bpy-module-latest-20230704/bpy/ops/paintcurve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-07-04 06:24:33.000000 fake-bpy-module-latest-20230704/bpy/ops/palette.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22863 2023-07-04 06:24:05.000000 fake-bpy-module-latest-20230704/bpy/ops/particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39854 2023-07-04 06:24:39.000000 fake-bpy-module-latest-20230704/bpy/ops/pose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-07-04 06:24:29.000000 fake-bpy-module-latest-20230704/bpy/ops/poselib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32889 2023-07-04 06:24:42.000000 fake-bpy-module-latest-20230704/bpy/ops/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-04 06:24:32.000000 fake-bpy-module-latest-20230704/bpy/ops/ptcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:15:22.000000 fake-bpy-module-latest-20230704/bpy/ops/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-07-04 06:24:15.000000 fake-bpy-module-latest-20230704/bpy/ops/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-07-04 06:23:58.000000 fake-bpy-module-latest-20230704/bpy/ops/rigidbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25220 2023-07-04 06:24:28.000000 fake-bpy-module-latest-20230704/bpy/ops/scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31884 2023-07-04 06:24:01.000000 fake-bpy-module-latest-20230704/bpy/ops/screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-04 06:23:58.000000 fake-bpy-module-latest-20230704/bpy/ops/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46889 2023-07-04 06:24:12.000000 fake-bpy-module-latest-20230704/bpy/ops/sculpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-04 06:24:42.000000 fake-bpy-module-latest-20230704/bpy/ops/sculpt_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94657 2023-07-04 06:24:41.000000 fake-bpy-module-latest-20230704/bpy/ops/sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19928 2023-07-04 06:24:29.000000 fake-bpy-module-latest-20230704/bpy/ops/sound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-04 06:24:06.000000 fake-bpy-module-latest-20230704/bpy/ops/spreadsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-07-04 06:24:30.000000 fake-bpy-module-latest-20230704/bpy/ops/surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32954 2023-07-04 06:24:11.000000 fake-bpy-module-latest-20230704/bpy/ops/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-04 06:24:29.000000 fake-bpy-module-latest-20230704/bpy/ops/text_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-04 06:24:41.000000 fake-bpy-module-latest-20230704/bpy/ops/texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70745 2023-07-04 06:24:32.000000 fake-bpy-module-latest-20230704/bpy/ops/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19753 2023-07-04 06:24:42.000000 fake-bpy-module-latest-20230704/bpy/ops/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-07-04 06:24:15.000000 fake-bpy-module-latest-20230704/bpy/ops/uilist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57464 2023-07-04 06:24:15.000000 fake-bpy-module-latest-20230704/bpy/ops/uv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-07-04 06:24:16.000000 fake-bpy-module-latest-20230704/bpy/ops/view2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54854 2023-07-04 06:24:44.000000 fake-bpy-module-latest-20230704/bpy/ops/view3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)   246250 2023-07-04 06:24:28.000000 fake-bpy-module-latest-20230704/bpy/ops/wm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-07-04 06:24:11.000000 fake-bpy-module-latest-20230704/bpy/ops/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-04 06:24:14.000000 fake-bpy-module-latest-20230704/bpy/ops/world.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-07-04 06:24:44.000000 fake-bpy-module-latest-20230704/bpy/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29417 2023-07-04 06:24:45.000000 fake-bpy-module-latest-20230704/bpy/props.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:15:22.000000 fake-bpy-module-latest-20230704/bpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)  3497949 2023-07-04 06:23:53.000000 fake-bpy-module-latest-20230704/bpy/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:27:34.000000 fake-bpy-module-latest-20230704/bpy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-07-04 06:24:44.000000 fake-bpy-module-latest-20230704/bpy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-07-04 06:24:44.000000 fake-bpy-module-latest-20230704/bpy/utils/previews.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:15:22.000000 fake-bpy-module-latest-20230704/bpy/utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-07-04 06:24:44.000000 fake-bpy-module-latest-20230704/bpy/utils/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:27:34.000000 fake-bpy-module-latest-20230704/bpy_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-04 06:24:50.000000 fake-bpy-module-latest-20230704/bpy_extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-07-04 06:24:50.000000 fake-bpy-module-latest-20230704/bpy_extras/anim_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-04 06:24:50.000000 fake-bpy-module-latest-20230704/bpy_extras/asset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-04 06:24:50.000000 fake-bpy-module-latest-20230704/bpy_extras/bmesh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-04 06:24:50.000000 fake-bpy-module-latest-20230704/bpy_extras/id_map_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-07-04 06:24:50.000000 fake-bpy-module-latest-20230704/bpy_extras/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-07-04 06:24:50.000000 fake-bpy-module-latest-20230704/bpy_extras/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-04 06:24:50.000000 fake-bpy-module-latest-20230704/bpy_extras/keyconfig_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-07-04 06:24:50.000000 fake-bpy-module-latest-20230704/bpy_extras/mesh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-07-04 06:24:50.000000 fake-bpy-module-latest-20230704/bpy_extras/node_shader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-04 06:24:50.000000 fake-bpy-module-latest-20230704/bpy_extras/node_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-04 06:24:50.000000 fake-bpy-module-latest-20230704/bpy_extras/object_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:15:22.000000 fake-bpy-module-latest-20230704/bpy_extras/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-07-04 06:24:50.000000 fake-bpy-module-latest-20230704/bpy_extras/view3d_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:27:34.000000 fake-bpy-module-latest-20230704/bpy_extras/wm_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-04 06:24:50.000000 fake-bpy-module-latest-20230704/bpy_extras/wm_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-04 06:24:50.000000 fake-bpy-module-latest-20230704/bpy_extras/wm_utils/progress_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:15:22.000000 fake-bpy-module-latest-20230704/bpy_extras/wm_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-04 06:27:23.000000 fake-bpy-module-latest-20230704/bpy_restrict_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54167 2023-07-04 06:27:33.000000 fake-bpy-module-latest-20230704/bpy_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-04 06:24:53.000000 fake-bpy-module-latest-20230704/console_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-04 06:27:23.000000 fake-bpy-module-latest-20230704/console_shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:27:34.000000 fake-bpy-module-latest-20230704/fake_bpy_module_latest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-07-04 06:27:34.000000 fake-bpy-module-latest-20230704/fake_bpy_module_latest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-07-04 06:27:34.000000 fake-bpy-module-latest-20230704/fake_bpy_module_latest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 06:27:34.000000 fake-bpy-module-latest-20230704/fake_bpy_module_latest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 06:27:34.000000 fake-bpy-module-latest-20230704/fake_bpy_module_latest.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-04 06:27:34.000000 fake-bpy-module-latest-20230704/fake_bpy_module_latest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:27:34.000000 fake-bpy-module-latest-20230704/freestyle/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-04 06:24:49.000000 fake-bpy-module-latest-20230704/freestyle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-07-04 06:24:50.000000 fake-bpy-module-latest-20230704/freestyle/chainingiterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47908 2023-07-04 06:24:49.000000 fake-bpy-module-latest-20230704/freestyle/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13232 2023-07-04 06:24:49.000000 fake-bpy-module-latest-20230704/freestyle/predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:15:22.000000 fake-bpy-module-latest-20230704/freestyle/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23737 2023-07-04 06:24:50.000000 fake-bpy-module-latest-20230704/freestyle/shaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86403 2023-07-04 06:24:50.000000 fake-bpy-module-latest-20230704/freestyle/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:27:34.000000 fake-bpy-module-latest-20230704/freestyle/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-04 06:24:49.000000 fake-bpy-module-latest-20230704/freestyle/utils/ContextFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-07-04 06:24:49.000000 fake-bpy-module-latest-20230704/freestyle/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:15:22.000000 fake-bpy-module-latest-20230704/freestyle/utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:27:34.000000 fake-bpy-module-latest-20230704/gpu/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-04 06:24:49.000000 fake-bpy-module-latest-20230704/gpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-07-04 06:24:49.000000 fake-bpy-module-latest-20230704/gpu/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-04 06:24:49.000000 fake-bpy-module-latest-20230704/gpu/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-04 06:24:49.000000 fake-bpy-module-latest-20230704/gpu/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:15:22.000000 fake-bpy-module-latest-20230704/gpu/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-04 06:24:49.000000 fake-bpy-module-latest-20230704/gpu/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-04 06:24:49.000000 fake-bpy-module-latest-20230704/gpu/shader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-07-04 06:24:49.000000 fake-bpy-module-latest-20230704/gpu/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-04 06:24:49.000000 fake-bpy-module-latest-20230704/gpu/texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-07-04 06:24:49.000000 fake-bpy-module-latest-20230704/gpu/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:27:34.000000 fake-bpy-module-latest-20230704/gpu_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-04 06:24:49.000000 fake-bpy-module-latest-20230704/gpu_extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-04 06:24:49.000000 fake-bpy-module-latest-20230704/gpu_extras/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-04 06:24:49.000000 fake-bpy-module-latest-20230704/gpu_extras/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:15:22.000000 fake-bpy-module-latest-20230704/gpu_extras/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-04 06:27:24.000000 fake-bpy-module-latest-20230704/graphviz_export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:27:34.000000 fake-bpy-module-latest-20230704/idprop/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-04 06:24:53.000000 fake-bpy-module-latest-20230704/idprop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:15:22.000000 fake-bpy-module-latest-20230704/idprop/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-04 06:24:53.000000 fake-bpy-module-latest-20230704/idprop/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:27:34.000000 fake-bpy-module-latest-20230704/imbuf/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-04 06:24:53.000000 fake-bpy-module-latest-20230704/imbuf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:15:22.000000 fake-bpy-module-latest-20230704/imbuf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-04 06:24:53.000000 fake-bpy-module-latest-20230704/imbuf/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48637 2023-07-04 06:27:24.000000 fake-bpy-module-latest-20230704/keyingsets_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-04 06:27:33.000000 fake-bpy-module-latest-20230704/keyingsets_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:27:34.000000 fake-bpy-module-latest-20230704/mathutils/
+-rw-r--r--   0 runner    (1001) docker     (123)    86215 2023-07-04 06:24:48.000000 fake-bpy-module-latest-20230704/mathutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-07-04 06:24:48.000000 fake-bpy-module-latest-20230704/mathutils/bvhtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22187 2023-07-04 06:24:49.000000 fake-bpy-module-latest-20230704/mathutils/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-04 06:24:48.000000 fake-bpy-module-latest-20230704/mathutils/interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-07-04 06:24:48.000000 fake-bpy-module-latest-20230704/mathutils/kdtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-07-04 06:24:48.000000 fake-bpy-module-latest-20230704/mathutils/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:15:22.000000 fake-bpy-module-latest-20230704/mathutils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-04 06:27:33.000000 fake-bpy-module-latest-20230704/nodeitems_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-04 06:24:53.000000 fake-bpy-module-latest-20230704/nodeitems_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-07-04 06:27:23.000000 fake-bpy-module-latest-20230704/rna_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-04 06:27:24.000000 fake-bpy-module-latest-20230704/rna_keymap_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-04 06:27:24.000000 fake-bpy-module-latest-20230704/rna_prop_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-04 06:27:23.000000 fake-bpy-module-latest-20230704/rna_xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 06:27:34.000000 fake-bpy-module-latest-20230704/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-04 06:27:33.000000 fake-bpy-module-latest-20230704/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-04 06:27:24.000000 fake-bpy-module-latest-20230704/sys_info.py
```

### Comparing `fake-bpy-module-latest-20230703/PKG-INFO` & `fake-bpy-module-latest-20230704/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: fake-bpy-module-latest
-Version: 20230703
+Version: 20230704
 Summary: Collection of the fake Blender Python API module for the code completion.
 Home-page: https://github.com/nutti/fake-bpy-module
 Author: nutti
 Author-email: nutti.metro@gmail.com
 Maintainer: nutti
 Maintainer-email: nutti.metro@gmail.com
 License: MIT
```

### Comparing `fake-bpy-module-latest-20230703/README.rst` & `fake-bpy-module-latest-20230704/README.rst`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/addon_utils.py` & `fake-bpy-module-latest-20230704/addon_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/animsys_refactor.py` & `fake-bpy-module-latest-20230704/animsys_refactor.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/aud.py` & `fake-bpy-module-latest-20230704/aud.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bgl.py` & `fake-bpy-module-latest-20230704/bgl.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_app_override/helpers.py` & `fake-bpy-module-latest-20230704/bl_app_override/helpers.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_i18n_utils/bl_extract_messages.py` & `fake-bpy-module-latest-20230704/bl_i18n_utils/bl_extract_messages.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_i18n_utils/settings.py` & `fake-bpy-module-latest-20230704/bl_i18n_utils/settings.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_i18n_utils/utils.py` & `fake-bpy-module-latest-20230704/bl_i18n_utils/utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_keymap_utils/io.py` & `fake-bpy-module-latest-20230704/bl_keymap_utils/io.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_math.py` & `fake-bpy-module-latest-20230704/bl_math.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_operators/__init__.py` & `fake-bpy-module-latest-20230704/bl_operators/__init__.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 import sys
 import typing
+from . import wm
+from . import constraint
+from . import presets
+from . import assets
 from . import screen_play_rendered_anim
-from . import file
-from . import sequencer
-from . import add_mesh_torus
-from . import node
-from . import object_randomize_transform
+from . import userpref
 from . import object_quick_effects
-from . import geometry_nodes
 from . import bmesh
-from . import anim
+from . import spreadsheet
+from . import uvcalc_follow_active
 from . import uvcalc_lightmap
-from . import view3d
+from . import add_mesh_torus
+from . import clip
+from . import mesh
+from . import freestyle
+from . import console
+from . import vertexpaint_dirt
+from . import geometry_nodes
+from . import sequencer
+from . import object_randomize_transform
+from . import uvcalc_transform
+from . import anim
+from . import node
 from . import object
-from . import presets
 from . import text
 from . import object_align
-from . import assets
-from . import spreadsheet
+from . import file
+from . import view3d
 from . import image
-from . import console
-from . import freestyle
-from . import wm
-from . import vertexpaint_dirt
-from . import mesh
-from . import clip
-from . import uvcalc_transform
-from . import constraint
-from . import uvcalc_follow_active
 from . import rigidbody
-from . import userpref
 
 GenericType = typing.TypeVar("GenericType")
 
 
 def register():
     '''
```

### Comparing `fake-bpy-module-latest-20230703/bl_operators/add_mesh_torus.py` & `fake-bpy-module-latest-20230704/bl_operators/add_mesh_torus.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_operators/anim.py` & `fake-bpy-module-latest-20230704/bl_operators/anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_operators/assets.py` & `fake-bpy-module-latest-20230704/bl_operators/assets.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_operators/bmesh/find_adjacent.py` & `fake-bpy-module-latest-20230704/bl_operators/bmesh/find_adjacent.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_operators/clip.py` & `fake-bpy-module-latest-20230704/bl_operators/clip.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_operators/console.py` & `fake-bpy-module-latest-20230704/bl_operators/console.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_operators/constraint.py` & `fake-bpy-module-latest-20230704/bl_operators/constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_operators/file.py` & `fake-bpy-module-latest-20230704/bl_operators/file.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_operators/freestyle.py` & `fake-bpy-module-latest-20230704/bl_operators/freestyle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_operators/geometry_nodes.py` & `fake-bpy-module-latest-20230704/bl_operators/geometry_nodes.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_operators/image.py` & `fake-bpy-module-latest-20230704/bl_operators/image.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_operators/mesh.py` & `fake-bpy-module-latest-20230704/bl_operators/mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_operators/node.py` & `fake-bpy-module-latest-20230704/bl_operators/node.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_operators/object.py` & `fake-bpy-module-latest-20230704/bl_operators/object.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_operators/object_align.py` & `fake-bpy-module-latest-20230704/bl_operators/object_align.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_operators/object_quick_effects.py` & `fake-bpy-module-latest-20230704/bl_operators/object_quick_effects.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_operators/object_randomize_transform.py` & `fake-bpy-module-latest-20230704/bl_operators/object_randomize_transform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_operators/presets.py` & `fake-bpy-module-latest-20230704/bl_operators/presets.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_operators/rigidbody.py` & `fake-bpy-module-latest-20230704/bl_operators/rigidbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_operators/screen_play_rendered_anim.py` & `fake-bpy-module-latest-20230704/bl_operators/screen_play_rendered_anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_operators/sequencer.py` & `fake-bpy-module-latest-20230704/bl_operators/sequencer.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_operators/spreadsheet.py` & `fake-bpy-module-latest-20230704/bl_operators/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_operators/text.py` & `fake-bpy-module-latest-20230704/bl_operators/text.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_operators/userpref.py` & `fake-bpy-module-latest-20230704/bl_operators/userpref.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_operators/uvcalc_follow_active.py` & `fake-bpy-module-latest-20230704/bl_operators/uvcalc_follow_active.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_operators/uvcalc_lightmap.py` & `fake-bpy-module-latest-20230704/bl_operators/uvcalc_lightmap.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_operators/uvcalc_transform.py` & `fake-bpy-module-latest-20230704/bl_operators/uvcalc_transform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_operators/vertexpaint_dirt.py` & `fake-bpy-module-latest-20230704/bl_operators/vertexpaint_dirt.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_operators/view3d.py` & `fake-bpy-module-latest-20230704/bl_operators/view3d.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_operators/wm.py` & `fake-bpy-module-latest-20230704/bl_operators/wm.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_previews_utils/bl_previews_render.py` & `fake-bpy-module-latest-20230704/bl_previews_utils/bl_previews_render.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/__init__.py` & `fake-bpy-module-latest-20230704/bl_ui/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,82 +1,82 @@
 import sys
 import typing
 import bpy_types
 
-from . import space_toolsystem_toolbar
-from . import properties_output
+from . import space_console
+from . import space_toolsystem_common
+from . import properties_data_lattice
+from . import properties_material
+from . import properties_scene
+from . import properties_data_bone
+from . import properties_particle
+from . import properties_grease_pencil_common
+from . import properties_data_curve
 from . import space_view3d
-from . import properties_data_volume
-from . import node_add_menu_geometry
+from . import space_graph
+from . import properties_constraint
 from . import properties_data_lightprobe
-from . import properties_material_gpencil
-from . import utils
+from . import space_dopesheet
+from . import space_text
+from . import space_nla
+from . import properties_paint_common
+from . import properties_object
+from . import properties_view_layer
+from . import properties_data_curves
+from . import properties_data_shaderfx
+from . import properties_data_camera
 from . import properties_mask_common
-from . import space_userpref
+from . import properties_data_volume
 from . import properties_freestyle
-from . import properties_workspace
-from . import properties_data_gpencil
-from . import space_info
+from . import properties_data_light
 from . import space_properties
-from . import properties_texture
-from . import node_add_menu
-from . import properties_data_camera
-from . import space_time
-from . import properties_constraint
-from . import space_nla
-from . import properties_data_empty
+from . import properties_animviz
 from . import space_image
-from . import properties_collection
-from . import space_node
-from . import properties_data_armature
-from . import properties_data_metaball
-from . import space_sequencer
-from . import properties_data_lattice
 from . import properties_physics_rigidbody
-from . import space_toolsystem_common
-from . import properties_data_mesh
-from . import properties_physics_field
-from . import properties_data_pointcloud
+from . import node_add_menu_geometry
 from . import space_topbar
-from . import space_clip
-from . import properties_data_grease_pencil
-from . import space_console
+from . import space_outliner
+from . import space_userpref
+from . import space_view3d_toolbar
+from . import space_time
+from . import properties_data_armature
+from . import properties_data_gpencil
+from . import properties_world
+from . import properties_physics_cloth
+from . import properties_physics_rigidbody_constraint
+from . import utils
 from . import space_filebrowser
-from . import properties_render
-from . import space_dopesheet
-from . import properties_physics_geometry_nodes
 from . import properties_physics_common
+from . import node_add_menu
+from . import properties_data_grease_pencil
 from . import properties_physics_softbody
-from . import properties_world
-from . import space_statusbar
-from . import properties_paint_common
+from . import generic_ui_list
+from . import properties_output
+from . import properties_material_gpencil
+from . import properties_data_mesh
+from . import space_spreadsheet
 from . import properties_physics_fluid
-from . import properties_physics_rigidbody_constraint
-from . import space_view3d_toolbar
-from . import properties_material
-from . import space_text
-from . import properties_grease_pencil_common
-from . import properties_data_curve
-from . import properties_physics_dynamicpaint
-from . import properties_object
-from . import properties_particle
+from . import properties_data_pointcloud
 from . import properties_data_speaker
-from . import properties_data_curves
+from . import properties_workspace
+from . import properties_physics_field
+from . import space_node
+from . import properties_physics_dynamicpaint
+from . import properties_texture
+from . import properties_collection
+from . import space_statusbar
+from . import space_clip
+from . import space_info
+from . import properties_data_metaball
+from . import properties_data_empty
+from . import space_toolsystem_toolbar
+from . import space_sequencer
 from . import properties_data_modifier
-from . import properties_data_bone
-from . import properties_view_layer
-from . import properties_scene
-from . import properties_physics_cloth
-from . import space_spreadsheet
-from . import properties_data_shaderfx
-from . import properties_data_light
-from . import properties_animviz
-from . import generic_ui_list
-from . import space_graph
-from . import space_outliner
+from . import properties_physics_geometry_nodes
+from . import properties_render
 
 GenericType = typing.TypeVar("GenericType")
 
 
 class UI_MT_button_context_menu(bpy_types.Menu, bpy_types._GenericUI):
     bl_idname = None
     ''' '''
```

### Comparing `fake-bpy-module-latest-20230703/bl_ui/generic_ui_list.py` & `fake-bpy-module-latest-20230704/bl_ui/generic_ui_list.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/node_add_menu_geometry.py` & `fake-bpy-module-latest-20230704/bl_ui/node_add_menu_geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_animviz.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_animviz.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_collection.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_collection.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_constraint.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_data_armature.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_data_armature.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_data_bone.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_data_bone.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_data_camera.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_data_camera.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_data_curve.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_data_curve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_data_curves.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_data_curves.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_data_empty.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_data_empty.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_data_gpencil.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_data_gpencil.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_data_grease_pencil.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_data_grease_pencil.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_data_lattice.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_data_lattice.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_data_light.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_data_light.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_data_lightprobe.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_data_lightprobe.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_data_mesh.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_data_mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_data_metaball.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_data_metaball.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_data_modifier.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_data_modifier.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_data_pointcloud.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_data_pointcloud.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_data_shaderfx.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_data_shaderfx.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_data_speaker.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_data_speaker.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_data_volume.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_data_volume.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_freestyle.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_freestyle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_grease_pencil_common.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_grease_pencil_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_mask_common.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_mask_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_material.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_material.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_material_gpencil.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_material_gpencil.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_object.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_object.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_output.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_output.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_paint_common.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_paint_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_particle.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_particle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_physics_cloth.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_physics_cloth.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_physics_common.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_physics_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_physics_dynamicpaint.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_physics_dynamicpaint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_physics_field.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_physics_field.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_physics_fluid.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_physics_fluid.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_physics_geometry_nodes.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_physics_geometry_nodes.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_physics_rigidbody.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_physics_rigidbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_physics_rigidbody_constraint.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_physics_rigidbody_constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_physics_softbody.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_physics_softbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_render.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_render.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_scene.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_scene.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_texture.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_texture.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_view_layer.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_view_layer.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_workspace.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_workspace.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/properties_world.py` & `fake-bpy-module-latest-20230704/bl_ui/properties_world.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/space_clip.py` & `fake-bpy-module-latest-20230704/bl_ui/space_clip.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/space_console.py` & `fake-bpy-module-latest-20230704/bl_ui/space_console.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/space_dopesheet.py` & `fake-bpy-module-latest-20230704/bl_ui/space_dopesheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/space_filebrowser.py` & `fake-bpy-module-latest-20230704/bl_ui/space_filebrowser.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/space_graph.py` & `fake-bpy-module-latest-20230704/bl_ui/space_graph.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/space_image.py` & `fake-bpy-module-latest-20230704/bl_ui/space_image.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/space_info.py` & `fake-bpy-module-latest-20230704/bl_ui/space_info.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/space_nla.py` & `fake-bpy-module-latest-20230704/bl_ui/space_nla.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/space_node.py` & `fake-bpy-module-latest-20230704/bl_ui/space_node.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/space_outliner.py` & `fake-bpy-module-latest-20230704/bl_ui/space_outliner.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/space_properties.py` & `fake-bpy-module-latest-20230704/bl_ui/space_properties.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/space_sequencer.py` & `fake-bpy-module-latest-20230704/bl_ui/space_sequencer.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/space_spreadsheet.py` & `fake-bpy-module-latest-20230704/bl_ui/space_spreadsheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/space_statusbar.py` & `fake-bpy-module-latest-20230704/bl_ui/space_statusbar.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/space_text.py` & `fake-bpy-module-latest-20230704/bl_ui/space_text.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/space_time.py` & `fake-bpy-module-latest-20230704/bl_ui/space_time.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/space_toolsystem_common.py` & `fake-bpy-module-latest-20230704/bl_ui/space_toolsystem_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/space_toolsystem_toolbar.py` & `fake-bpy-module-latest-20230704/bl_ui/space_toolsystem_toolbar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1393,14 +1393,19 @@
     lasso = None
     ''' '''
 
     select = None
     ''' '''
 
 
+class _defs_paint_grease_pencil:
+    draw = None
+    ''' '''
+
+
 class _defs_particle:
     def generate_from_brushes(self, context):
         ''' 
 
         '''
         pass
```

### Comparing `fake-bpy-module-latest-20230703/bl_ui/space_topbar.py` & `fake-bpy-module-latest-20230704/bl_ui/space_topbar.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/space_userpref.py` & `fake-bpy-module-latest-20230704/bl_ui/space_userpref.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/space_view3d.py` & `fake-bpy-module-latest-20230704/bl_ui/space_view3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -22508,14 +22508,218 @@
     def values(self):
         ''' 
 
         '''
         pass
 
 
+class VIEW3D_MT_paint_grease_pencil(bpy_types.Menu, bpy_types._GenericUI):
+    bl_label = None
+    ''' '''
+
+    bl_rna = None
+    ''' '''
+
+    id_data = None
+    ''' '''
+
+    def append(self, draw_func):
+        ''' 
+
+        '''
+        pass
+
+    def as_pointer(self):
+        ''' 
+
+        '''
+        pass
+
+    def bl_rna_get_subclass(self):
+        ''' 
+
+        '''
+        pass
+
+    def bl_rna_get_subclass_py(self):
+        ''' 
+
+        '''
+        pass
+
+    def draw(self, _context):
+        ''' 
+
+        '''
+        pass
+
+    def draw_collapsible(self, context, layout):
+        ''' 
+
+        '''
+        pass
+
+    def draw_preset(self, _context):
+        ''' 
+
+        '''
+        pass
+
+    def driver_add(self):
+        ''' 
+
+        '''
+        pass
+
+    def driver_remove(self):
+        ''' 
+
+        '''
+        pass
+
+    def get(self):
+        ''' 
+
+        '''
+        pass
+
+    def id_properties_clear(self):
+        ''' 
+
+        '''
+        pass
+
+    def id_properties_ensure(self):
+        ''' 
+
+        '''
+        pass
+
+    def id_properties_ui(self):
+        ''' 
+
+        '''
+        pass
+
+    def is_extended(self):
+        ''' 
+
+        '''
+        pass
+
+    def is_property_hidden(self):
+        ''' 
+
+        '''
+        pass
+
+    def is_property_overridable_library(self):
+        ''' 
+
+        '''
+        pass
+
+    def is_property_readonly(self):
+        ''' 
+
+        '''
+        pass
+
+    def is_property_set(self):
+        ''' 
+
+        '''
+        pass
+
+    def items(self):
+        ''' 
+
+        '''
+        pass
+
+    def keyframe_delete(self):
+        ''' 
+
+        '''
+        pass
+
+    def keyframe_insert(self):
+        ''' 
+
+        '''
+        pass
+
+    def keys(self):
+        ''' 
+
+        '''
+        pass
+
+    def path_from_id(self):
+        ''' 
+
+        '''
+        pass
+
+    def path_menu(self, searchpaths, operator, props_default, prop_filepath,
+                  filter_ext, filter_path, display_name, add_operator):
+        ''' 
+
+        '''
+        pass
+
+    def path_resolve(self):
+        ''' 
+
+        '''
+        pass
+
+    def pop(self):
+        ''' 
+
+        '''
+        pass
+
+    def prepend(self, draw_func):
+        ''' 
+
+        '''
+        pass
+
+    def property_overridable_library_set(self):
+        ''' 
+
+        '''
+        pass
+
+    def property_unset(self):
+        ''' 
+
+        '''
+        pass
+
+    def remove(self, draw_func):
+        ''' 
+
+        '''
+        pass
+
+    def type_recast(self):
+        ''' 
+
+        '''
+        pass
+
+    def values(self):
+        ''' 
+
+        '''
+        pass
+
+
 class VIEW3D_MT_paint_vertex(bpy_types.Menu, bpy_types._GenericUI):
     bl_label = None
     ''' '''
 
     bl_rna = None
     ''' '''
```

### Comparing `fake-bpy-module-latest-20230703/bl_ui/space_view3d_toolbar.py` & `fake-bpy-module-latest-20230704/bl_ui/space_view3d_toolbar.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bl_ui/utils.py` & `fake-bpy-module-latest-20230704/bl_ui/utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/blf.py` & `fake-bpy-module-latest-20230704/blf.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bmesh/__init__.py` & `fake-bpy-module-latest-20230704/bmesh/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bmesh/geometry.py` & `fake-bpy-module-latest-20230704/bmesh/geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bmesh/ops.py` & `fake-bpy-module-latest-20230704/bmesh/ops.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bmesh/types.py` & `fake-bpy-module-latest-20230704/bmesh/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bmesh/utils.py` & `fake-bpy-module-latest-20230704/bmesh/utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/app/__init__.py` & `fake-bpy-module-latest-20230704/bpy/app/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 import typing
 from . import translations
-from . import icons
 from . import timers
 from . import handlers
+from . import icons
 
 GenericType = typing.TypeVar("GenericType")
 
 
 def help_text(all: typing.Optional[bool] = False):
     ''' Return the help text as a string.
```

### Comparing `fake-bpy-module-latest-20230703/bpy/app/handlers.py` & `fake-bpy-module-latest-20230704/bpy/app/handlers.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/app/icons.py` & `fake-bpy-module-latest-20230704/bpy/app/icons.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/app/timers.py` & `fake-bpy-module-latest-20230704/bpy/app/timers.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/app/translations.py` & `fake-bpy-module-latest-20230704/bpy/app/translations.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/msgbus.py` & `fake-bpy-module-latest-20230704/bpy/msgbus.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/__init__.py` & `fake-bpy-module-latest-20230704/bpy/ops/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,81 +1,81 @@
 import sys
 import typing
-from . import particle
-from . import ed
-from . import export_scene
-from . import camera
-from . import file
-from . import gpencil
-from . import texture
-from . import cachefile
+from . import object
 from . import brush
-from . import sound
-from . import surface
+from . import curves
+from . import rigidbody
+from . import script
 from . import asset
+from . import lattice
 from . import fluid
-from . import constraint
 from . import cloth
-from . import lattice
-from . import nla
-from . import action
-from . import transform
-from . import text
-from . import import_mesh
-from . import sculpt_curves
-from . import uv
-from . import ptcache
-from . import render
-from . import rigidbody
-from . import object
-from . import graph
-from . import text_editor
-from . import curves
-from . import node
-from . import paintcurve
-from . import view3d
-from . import curve
+from . import gpencil
+from . import screen
+from . import armature
+from . import export_mesh
+from . import grease_pencil
 from . import export_anim
-from . import sequencer
+from . import particle
+from . import outliner
+from . import buttons
 from . import spreadsheet
-from . import poselib
-from . import import_anim
-from . import info
-from . import cycles
+from . import export_scene
 from . import image
-from . import boid
-from . import clip
-from . import preferences
-from . import export_mesh
-from . import marker
-from . import mesh
-from . import console
-from . import mask
+from . import dpaint
+from . import text
 from . import workspace
+from . import anim
+from . import sculpt
+from . import mask
 from . import paint
+from . import world
+from . import uv
+from . import render
+from . import uilist
+from . import gizmogroup
 from . import import_scene
-from . import outliner
-from . import geometry
-from . import dpaint
-from . import sculpt
-from . import ui
-from . import buttons
-from . import anim
-from . import import_curve
+from . import import_mesh
+from . import view2d
+from . import node
+from . import curve
+from . import clip
+from . import font
+from . import material
 from . import wm
-from . import armature
 from . import scene
-from . import uilist
+from . import poselib
+from . import boid
+from . import camera
+from . import import_anim
+from . import ed
+from . import sound
+from . import text_editor
+from . import surface
+from . import collection
+from . import geometry
+from . import action
+from . import transform
+from . import paintcurve
+from . import ptcache
+from . import constraint
 from . import mball
+from . import nla
 from . import palette
-from . import screen
-from . import font
-from . import view2d
+from . import graph
+from . import cycles
+from . import file
+from . import mesh
+from . import marker
 from . import pose
-from . import collection
-from . import material
-from . import world
-from . import script
-from . import grease_pencil
-from . import gizmogroup
+from . import sequencer
+from . import texture
+from . import import_curve
+from . import sculpt_curves
+from . import ui
+from . import console
+from . import preferences
+from . import info
+from . import cachefile
+from . import view3d
 
 GenericType = typing.TypeVar("GenericType")
```

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/action.py` & `fake-bpy-module-latest-20230704/bpy/ops/action.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/anim.py` & `fake-bpy-module-latest-20230704/bpy/ops/anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/armature.py` & `fake-bpy-module-latest-20230704/bpy/ops/armature.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/asset.py` & `fake-bpy-module-latest-20230704/bpy/ops/asset.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/boid.py` & `fake-bpy-module-latest-20230704/bpy/ops/boid.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/brush.py` & `fake-bpy-module-latest-20230704/bpy/ops/brush.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/buttons.py` & `fake-bpy-module-latest-20230704/bpy/ops/buttons.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/cachefile.py` & `fake-bpy-module-latest-20230704/bpy/ops/cachefile.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/camera.py` & `fake-bpy-module-latest-20230704/bpy/ops/camera.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/clip.py` & `fake-bpy-module-latest-20230704/bpy/ops/clip.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/cloth.py` & `fake-bpy-module-latest-20230704/bpy/ops/cloth.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/collection.py` & `fake-bpy-module-latest-20230704/bpy/ops/collection.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/console.py` & `fake-bpy-module-latest-20230704/bpy/ops/console.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/constraint.py` & `fake-bpy-module-latest-20230704/bpy/ops/constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/curve.py` & `fake-bpy-module-latest-20230704/bpy/ops/curve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/curves.py` & `fake-bpy-module-latest-20230704/bpy/ops/curves.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/cycles.py` & `fake-bpy-module-latest-20230704/bpy/ops/cycles.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/dpaint.py` & `fake-bpy-module-latest-20230704/bpy/ops/dpaint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/ed.py` & `fake-bpy-module-latest-20230704/bpy/ops/ed.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/export_anim.py` & `fake-bpy-module-latest-20230704/bpy/ops/export_anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/export_mesh.py` & `fake-bpy-module-latest-20230704/bpy/ops/export_mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/export_scene.py` & `fake-bpy-module-latest-20230704/bpy/ops/export_scene.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/file.py` & `fake-bpy-module-latest-20230704/bpy/ops/file.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/fluid.py` & `fake-bpy-module-latest-20230704/bpy/ops/fluid.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/font.py` & `fake-bpy-module-latest-20230704/bpy/ops/font.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/geometry.py` & `fake-bpy-module-latest-20230704/bpy/ops/geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/gizmogroup.py` & `fake-bpy-module-latest-20230704/bpy/ops/gizmogroup.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/gpencil.py` & `fake-bpy-module-latest-20230704/bpy/ops/gpencil.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/graph.py` & `fake-bpy-module-latest-20230704/bpy/ops/graph.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/grease_pencil.py` & `fake-bpy-module-latest-20230704/bpy/ops/grease_pencil.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/image.py` & `fake-bpy-module-latest-20230704/bpy/ops/image.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/import_anim.py` & `fake-bpy-module-latest-20230704/bpy/ops/import_anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/import_curve.py` & `fake-bpy-module-latest-20230704/bpy/ops/import_curve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/import_mesh.py` & `fake-bpy-module-latest-20230704/bpy/ops/import_mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/import_scene.py` & `fake-bpy-module-latest-20230704/bpy/ops/import_scene.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/info.py` & `fake-bpy-module-latest-20230704/bpy/ops/info.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/lattice.py` & `fake-bpy-module-latest-20230704/bpy/ops/lattice.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/marker.py` & `fake-bpy-module-latest-20230704/bpy/ops/marker.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/mask.py` & `fake-bpy-module-latest-20230704/bpy/ops/mask.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/material.py` & `fake-bpy-module-latest-20230704/bpy/ops/material.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/mball.py` & `fake-bpy-module-latest-20230704/bpy/ops/mball.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/mesh.py` & `fake-bpy-module-latest-20230704/bpy/ops/mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/nla.py` & `fake-bpy-module-latest-20230704/bpy/ops/nla.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/node.py` & `fake-bpy-module-latest-20230704/bpy/ops/node.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/object.py` & `fake-bpy-module-latest-20230704/bpy/ops/object.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/outliner.py` & `fake-bpy-module-latest-20230704/bpy/ops/outliner.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/paint.py` & `fake-bpy-module-latest-20230704/bpy/ops/paint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/paintcurve.py` & `fake-bpy-module-latest-20230704/bpy/ops/paintcurve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/palette.py` & `fake-bpy-module-latest-20230704/bpy/ops/palette.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/particle.py` & `fake-bpy-module-latest-20230704/bpy/ops/particle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/pose.py` & `fake-bpy-module-latest-20230704/bpy/ops/pose.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/poselib.py` & `fake-bpy-module-latest-20230704/bpy/ops/poselib.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/preferences.py` & `fake-bpy-module-latest-20230704/bpy/ops/preferences.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/ptcache.py` & `fake-bpy-module-latest-20230704/bpy/ops/ptcache.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/render.py` & `fake-bpy-module-latest-20230704/bpy/ops/render.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/rigidbody.py` & `fake-bpy-module-latest-20230704/bpy/ops/rigidbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/scene.py` & `fake-bpy-module-latest-20230704/bpy/ops/scene.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/screen.py` & `fake-bpy-module-latest-20230704/bpy/ops/screen.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/script.py` & `fake-bpy-module-latest-20230704/bpy/ops/script.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/sculpt.py` & `fake-bpy-module-latest-20230704/bpy/ops/sculpt.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/sculpt_curves.py` & `fake-bpy-module-latest-20230704/bpy/ops/sculpt_curves.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/sequencer.py` & `fake-bpy-module-latest-20230704/bpy/ops/sequencer.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/sound.py` & `fake-bpy-module-latest-20230704/bpy/ops/sound.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/spreadsheet.py` & `fake-bpy-module-latest-20230704/bpy/ops/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/surface.py` & `fake-bpy-module-latest-20230704/bpy/ops/surface.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/text.py` & `fake-bpy-module-latest-20230704/bpy/ops/text.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/text_editor.py` & `fake-bpy-module-latest-20230704/bpy/ops/text_editor.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/texture.py` & `fake-bpy-module-latest-20230704/bpy/ops/texture.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/transform.py` & `fake-bpy-module-latest-20230704/bpy/ops/transform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/ui.py` & `fake-bpy-module-latest-20230704/bpy/ops/ui.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/uilist.py` & `fake-bpy-module-latest-20230704/bpy/ops/uilist.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/uv.py` & `fake-bpy-module-latest-20230704/bpy/ops/uv.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,22 +369,25 @@
 
 
 def pin(override_context: typing.Union[typing.
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None,
         *,
-        clear: typing.Union[bool, typing.Any] = False):
+        clear: typing.Union[bool, typing.Any] = False,
+        invert: typing.Union[bool, typing.Any] = False):
     ''' Set/clear selected UV vertices as anchored between multiple unwrap operations
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param clear: Clear, Clear pinning for the selection instead of setting it
     :type clear: typing.Union[bool, typing.Any]
+    :param invert: Invert, Invert pinning for the selection instead of setting it
+    :type invert: typing.Union[bool, typing.Any]
     '''
 
     pass
 
 
 def project_from_view(override_context: typing.
                       Union[typing.Dict, 'bpy.types.Context'] = None,
```

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/view2d.py` & `fake-bpy-module-latest-20230704/bpy/ops/view2d.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/view3d.py` & `fake-bpy-module-latest-20230704/bpy/ops/view3d.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/wm.py` & `fake-bpy-module-latest-20230704/bpy/ops/wm.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/workspace.py` & `fake-bpy-module-latest-20230704/bpy/ops/workspace.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/ops/world.py` & `fake-bpy-module-latest-20230704/bpy/ops/world.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/path.py` & `fake-bpy-module-latest-20230704/bpy/path.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/props.py` & `fake-bpy-module-latest-20230704/bpy/props.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/types.py` & `fake-bpy-module-latest-20230704/bpy/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,180 +1,180 @@
 00000000: 696d 706f 7274 2073 7973 0a69 6d70 6f72  import sys.impor
 00000010: 7420 7479 7069 6e67 0a69 6d70 6f72 7420  t typing.import 
 00000020: 6d61 7468 7574 696c 730a 696d 706f 7274  mathutils.import
 00000030: 2062 7079 0a69 6d70 6f72 7420 626c 5f75   bpy.import bl_u
-00000040: 692e 7370 6163 655f 746f 6f6c 7379 7374  i.space_toolsyst
-00000050: 656d 5f74 6f6f 6c62 6172 0a69 6d70 6f72  em_toolbar.impor
-00000060: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
-00000070: 6573 5f6f 7574 7075 740a 696d 706f 7274  es_output.import
-00000080: 2062 6c5f 7569 2e73 7061 6365 5f76 6965   bl_ui.space_vie
-00000090: 7733 640a 696d 706f 7274 2062 6c5f 7569  w3d.import bl_ui
-000000a0: 2e70 726f 7065 7274 6965 735f 6461 7461  .properties_data
-000000b0: 5f76 6f6c 756d 650a 696d 706f 7274 2062  _volume.import b
-000000c0: 6c5f 7569 2e6e 6f64 655f 6164 645f 6d65  l_ui.node_add_me
-000000d0: 6e75 5f67 656f 6d65 7472 790a 696d 706f  nu_geometry.impo
-000000e0: 7274 2062 6c5f 6f70 6572 6174 6f72 732e  rt bl_operators.
-000000f0: 6669 6c65 0a69 6d70 6f72 7420 626c 5f75  file.import bl_u
-00000100: 692e 7072 6f70 6572 7469 6573 5f64 6174  i.properties_dat
-00000110: 615f 6c69 6768 7470 726f 6265 0a69 6d70  a_lightprobe.imp
-00000120: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
-00000130: 7469 6573 5f6d 6174 6572 6961 6c5f 6770  ties_material_gp
-00000140: 656e 6369 6c0a 696d 706f 7274 2062 6c5f  encil.import bl_
-00000150: 7569 2e70 726f 7065 7274 6965 735f 6d61  ui.properties_ma
-00000160: 736b 5f63 6f6d 6d6f 6e0a 696d 706f 7274  sk_common.import
-00000170: 2062 6c5f 7569 2e73 7061 6365 5f75 7365   bl_ui.space_use
-00000180: 7270 7265 660a 696d 706f 7274 2062 6c5f  rpref.import bl_
-00000190: 7569 2e70 726f 7065 7274 6965 735f 6672  ui.properties_fr
-000001a0: 6565 7374 796c 650a 696d 706f 7274 2062  eestyle.import b
-000001b0: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
-000001c0: 776f 726b 7370 6163 650a 696d 706f 7274  workspace.import
-000001d0: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
-000001e0: 735f 6461 7461 5f67 7065 6e63 696c 0a69  s_data_gpencil.i
-000001f0: 6d70 6f72 7420 626c 5f75 692e 7370 6163  mport bl_ui.spac
-00000200: 655f 696e 666f 0a69 6d70 6f72 7420 626c  e_info.import bl
-00000210: 5f6f 7065 7261 746f 7273 2e6e 6f64 650a  _operators.node.
-00000220: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
-00000230: 6365 5f70 726f 7065 7274 6965 730a 696d  ce_properties.im
-00000240: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
-00000250: 7274 6965 735f 7465 7874 7572 650a 696d  rties_texture.im
-00000260: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
-00000270: 7274 6965 735f 6461 7461 5f63 616d 6572  rties_data_camer
-00000280: 610a 696d 706f 7274 2062 6c5f 7569 2e73  a.import bl_ui.s
-00000290: 7061 6365 5f74 696d 650a 696d 706f 7274  pace_time.import
-000002a0: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
-000002b0: 735f 636f 6e73 7472 6169 6e74 0a69 6d70  s_constraint.imp
-000002c0: 6f72 7420 626c 5f75 692e 7370 6163 655f  ort bl_ui.space_
-000002d0: 6e6c 610a 696d 706f 7274 2062 6c5f 7569  nla.import bl_ui
-000002e0: 2e70 726f 7065 7274 6965 735f 6461 7461  .properties_data
-000002f0: 5f65 6d70 7479 0a69 6d70 6f72 7420 626c  _empty.import bl
-00000300: 5f75 692e 7370 6163 655f 696d 6167 650a  _ui.space_image.
-00000310: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
-00000320: 7065 7274 6965 735f 636f 6c6c 6563 7469  perties_collecti
-00000330: 6f6e 0a69 6d70 6f72 7420 626c 5f75 692e  on.import bl_ui.
-00000340: 7370 6163 655f 6e6f 6465 0a69 6d70 6f72  space_node.impor
-00000350: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
-00000360: 6573 5f64 6174 615f 6172 6d61 7475 7265  es_data_armature
-00000370: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
-00000380: 6f70 6572 7469 6573 5f64 6174 615f 6d65  operties_data_me
-00000390: 7461 6261 6c6c 0a69 6d70 6f72 7420 626c  taball.import bl
-000003a0: 5f6f 7065 7261 746f 7273 2e61 6e69 6d0a  _operators.anim.
-000003b0: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
-000003c0: 6365 5f73 6571 7565 6e63 6572 0a69 6d70  ce_sequencer.imp
-000003d0: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
-000003e0: 7469 6573 5f64 6174 615f 6c61 7474 6963  ties_data_lattic
-000003f0: 650a 696d 706f 7274 2062 6c5f 7569 2e70  e.import bl_ui.p
-00000400: 726f 7065 7274 6965 735f 7068 7973 6963  roperties_physic
-00000410: 735f 7269 6769 6462 6f64 790a 696d 706f  s_rigidbody.impo
-00000420: 7274 2062 6c5f 7569 0a69 6d70 6f72 7420  rt bl_ui.import 
-00000430: 626c 5f75 692e 7370 6163 655f 746f 6f6c  bl_ui.space_tool
-00000440: 7379 7374 656d 5f63 6f6d 6d6f 6e0a 696d  system_common.im
-00000450: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
-00000460: 7274 6965 735f 6461 7461 5f6d 6573 680a  rties_data_mesh.
-00000470: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
-00000480: 7065 7274 6965 735f 7068 7973 6963 735f  perties_physics_
-00000490: 6669 656c 640a 696d 706f 7274 2062 6c5f  field.import bl_
-000004a0: 7569 2e70 726f 7065 7274 6965 735f 6461  ui.properties_da
-000004b0: 7461 5f70 6f69 6e74 636c 6f75 640a 696d  ta_pointcloud.im
-000004c0: 706f 7274 2062 6c5f 7569 2e73 7061 6365  port bl_ui.space
-000004d0: 5f74 6f70 6261 720a 696d 706f 7274 2062  _topbar.import b
-000004e0: 6c5f 7569 2e73 7061 6365 5f63 6c69 700a  l_ui.space_clip.
-000004f0: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
-00000500: 7065 7274 6965 735f 6461 7461 5f67 7265  perties_data_gre
-00000510: 6173 655f 7065 6e63 696c 0a69 6d70 6f72  ase_pencil.impor
-00000520: 7420 626c 5f75 692e 7370 6163 655f 636f  t bl_ui.space_co
-00000530: 6e73 6f6c 650a 696d 706f 7274 2062 6c5f  nsole.import bl_
-00000540: 7569 2e73 7061 6365 5f66 696c 6562 726f  ui.space_filebro
-00000550: 7773 6572 0a69 6d70 6f72 7420 626c 5f75  wser.import bl_u
-00000560: 692e 7072 6f70 6572 7469 6573 5f72 656e  i.properties_ren
-00000570: 6465 720a 696d 706f 7274 2062 6c5f 7569  der.import bl_ui
-00000580: 2e73 7061 6365 5f64 6f70 6573 6865 6574  .space_dopesheet
-00000590: 0a69 6d70 6f72 7420 626c 5f6f 7065 7261  .import bl_opera
-000005a0: 746f 7273 2e76 6965 7733 640a 696d 706f  tors.view3d.impo
-000005b0: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
-000005c0: 6965 735f 7068 7973 6963 735f 6765 6f6d  ies_physics_geom
-000005d0: 6574 7279 5f6e 6f64 6573 0a69 6d70 6f72  etry_nodes.impor
-000005e0: 7420 626c 5f6f 7065 7261 746f 7273 2e6f  t bl_operators.o
-000005f0: 626a 6563 740a 696d 706f 7274 2062 6c5f  bject.import bl_
-00000600: 6f70 6572 6174 6f72 732e 7072 6573 6574  operators.preset
-00000610: 730a 696d 706f 7274 2062 6c5f 7569 2e70  s.import bl_ui.p
-00000620: 726f 7065 7274 6965 735f 7068 7973 6963  roperties_physic
-00000630: 735f 636f 6d6d 6f6e 0a69 6d70 6f72 7420  s_common.import 
-00000640: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-00000650: 5f70 6879 7369 6373 5f73 6f66 7462 6f64  _physics_softbod
-00000660: 790a 696d 706f 7274 2062 6c5f 7569 2e70  y.import bl_ui.p
-00000670: 726f 7065 7274 6965 735f 776f 726c 640a  roperties_world.
-00000680: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
-00000690: 6365 5f73 7461 7475 7362 6172 0a69 6d70  ce_statusbar.imp
-000006a0: 6f72 7420 626c 5f6f 7065 7261 746f 7273  ort bl_operators
-000006b0: 2e74 6578 740a 696d 706f 7274 2062 6c5f  .text.import bl_
-000006c0: 7569 2e70 726f 7065 7274 6965 735f 7061  ui.properties_pa
-000006d0: 696e 745f 636f 6d6d 6f6e 0a69 6d70 6f72  int_common.impor
-000006e0: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
-000006f0: 6573 5f70 6879 7369 6373 5f66 6c75 6964  es_physics_fluid
-00000700: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
-00000710: 6f70 6572 7469 6573 5f70 6879 7369 6373  operties_physics
-00000720: 5f72 6967 6964 626f 6479 5f63 6f6e 7374  _rigidbody_const
-00000730: 7261 696e 740a 696d 706f 7274 2062 6c5f  raint.import bl_
-00000740: 6f70 6572 6174 6f72 732e 6173 7365 7473  operators.assets
-00000750: 0a69 6d70 6f72 7420 626c 5f6f 7065 7261  .import bl_opera
-00000760: 746f 7273 2e73 7072 6561 6473 6865 6574  tors.spreadsheet
-00000770: 0a69 6d70 6f72 7420 626c 5f75 692e 7370  .import bl_ui.sp
-00000780: 6163 655f 7669 6577 3364 5f74 6f6f 6c62  ace_view3d_toolb
-00000790: 6172 0a69 6d70 6f72 7420 626c 5f75 692e  ar.import bl_ui.
-000007a0: 7072 6f70 6572 7469 6573 5f6d 6174 6572  properties_mater
-000007b0: 6961 6c0a 696d 706f 7274 2062 6c5f 7569  ial.import bl_ui
-000007c0: 2e73 7061 6365 5f74 6578 740a 696d 706f  .space_text.impo
-000007d0: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
-000007e0: 6965 735f 6772 6561 7365 5f70 656e 6369  ies_grease_penci
-000007f0: 6c5f 636f 6d6d 6f6e 0a69 6d70 6f72 7420  l_common.import 
-00000800: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-00000810: 5f64 6174 615f 6375 7276 650a 696d 706f  _data_curve.impo
-00000820: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
-00000830: 6965 735f 7068 7973 6963 735f 6479 6e61  ies_physics_dyna
-00000840: 6d69 6370 6169 6e74 0a69 6d70 6f72 7420  micpaint.import 
-00000850: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-00000860: 5f6f 626a 6563 740a 696d 706f 7274 2062  _object.import b
-00000870: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
-00000880: 7061 7274 6963 6c65 0a69 6d70 6f72 7420  particle.import 
-00000890: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-000008a0: 5f64 6174 615f 7370 6561 6b65 720a 696d  _data_speaker.im
-000008b0: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
-000008c0: 7274 6965 735f 6461 7461 5f63 7572 7665  rties_data_curve
-000008d0: 730a 696d 706f 7274 2062 6c5f 7569 2e70  s.import bl_ui.p
-000008e0: 726f 7065 7274 6965 735f 6461 7461 5f6d  roperties_data_m
-000008f0: 6f64 6966 6965 720a 696d 706f 7274 2062  odifier.import b
-00000900: 6c5f 6f70 6572 6174 6f72 732e 6672 6565  l_operators.free
-00000910: 7374 796c 650a 696d 706f 7274 2062 6c5f  style.import bl_
-00000920: 6f70 6572 6174 6f72 732e 776d 0a69 6d70  operators.wm.imp
-00000930: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
-00000940: 7469 6573 5f64 6174 615f 626f 6e65 0a69  ties_data_bone.i
-00000950: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
-00000960: 6572 7469 6573 5f76 6965 775f 6c61 7965  erties_view_laye
-00000970: 720a 696d 706f 7274 2062 6c5f 7569 2e70  r.import bl_ui.p
-00000980: 726f 7065 7274 6965 735f 7363 656e 650a  roperties_scene.
-00000990: 696d 706f 7274 2062 6c5f 6f70 6572 6174  import bl_operat
-000009a0: 6f72 732e 636c 6970 0a69 6d70 6f72 7420  ors.clip.import 
-000009b0: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-000009c0: 5f70 6879 7369 6373 5f63 6c6f 7468 0a69  _physics_cloth.i
-000009d0: 6d70 6f72 7420 626c 5f75 692e 7370 6163  mport bl_ui.spac
-000009e0: 655f 7370 7265 6164 7368 6565 740a 696d  e_spreadsheet.im
-000009f0: 706f 7274 2062 6c5f 6f70 6572 6174 6f72  port bl_operator
-00000a00: 732e 636f 6e73 7472 6169 6e74 0a69 6d70  s.constraint.imp
-00000a10: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
-00000a20: 7469 6573 5f64 6174 615f 7368 6164 6572  ties_data_shader
-00000a30: 6678 0a69 6d70 6f72 7420 626c 5f75 692e  fx.import bl_ui.
-00000a40: 7072 6f70 6572 7469 6573 5f64 6174 615f  properties_data_
-00000a50: 6c69 6768 740a 696d 706f 7274 2062 6c5f  light.import bl_
-00000a60: 7569 2e67 656e 6572 6963 5f75 695f 6c69  ui.generic_ui_li
-00000a70: 7374 0a69 6d70 6f72 7420 626c 5f75 692e  st.import bl_ui.
-00000a80: 7370 6163 655f 6772 6170 680a 696d 706f  space_graph.impo
-00000a90: 7274 2062 6c5f 7569 2e73 7061 6365 5f6f  rt bl_ui.space_o
-00000aa0: 7574 6c69 6e65 720a 696d 706f 7274 2062  utliner.import b
-00000ab0: 6c5f 6f70 6572 6174 6f72 732e 7573 6572  l_operators.user
-00000ac0: 7072 6566 0a0a 4765 6e65 7269 6354 7970  pref..GenericTyp
+00000040: 692e 7370 6163 655f 636f 6e73 6f6c 650a  i.space_console.
+00000050: 696d 706f 7274 2062 6c5f 6f70 6572 6174  import bl_operat
+00000060: 6f72 732e 776d 0a69 6d70 6f72 7420 626c  ors.wm.import bl
+00000070: 5f75 692e 7370 6163 655f 746f 6f6c 7379  _ui.space_toolsy
+00000080: 7374 656d 5f63 6f6d 6d6f 6e0a 696d 706f  stem_common.impo
+00000090: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
+000000a0: 6965 735f 6461 7461 5f6c 6174 7469 6365  ies_data_lattice
+000000b0: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
+000000c0: 6f70 6572 7469 6573 5f6d 6174 6572 6961  operties_materia
+000000d0: 6c0a 696d 706f 7274 2062 6c5f 6f70 6572  l.import bl_oper
+000000e0: 6174 6f72 732e 636f 6e73 7472 6169 6e74  ators.constraint
+000000f0: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
+00000100: 6f70 6572 7469 6573 5f73 6365 6e65 0a69  operties_scene.i
+00000110: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
+00000120: 6572 7469 6573 5f64 6174 615f 626f 6e65  erties_data_bone
+00000130: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
+00000140: 6f70 6572 7469 6573 5f70 6172 7469 636c  operties_particl
+00000150: 650a 696d 706f 7274 2062 6c5f 6f70 6572  e.import bl_oper
+00000160: 6174 6f72 732e 7072 6573 6574 730a 696d  ators.presets.im
+00000170: 706f 7274 2062 6c5f 6f70 6572 6174 6f72  port bl_operator
+00000180: 732e 6173 7365 7473 0a69 6d70 6f72 7420  s.assets.import 
+00000190: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+000001a0: 5f67 7265 6173 655f 7065 6e63 696c 5f63  _grease_pencil_c
+000001b0: 6f6d 6d6f 6e0a 696d 706f 7274 2062 6c5f  ommon.import bl_
+000001c0: 7569 2e70 726f 7065 7274 6965 735f 6461  ui.properties_da
+000001d0: 7461 5f63 7572 7665 0a69 6d70 6f72 7420  ta_curve.import 
+000001e0: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
+000001f0: 3364 0a69 6d70 6f72 7420 626c 5f75 692e  3d.import bl_ui.
+00000200: 7370 6163 655f 6772 6170 680a 696d 706f  space_graph.impo
+00000210: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
+00000220: 6965 735f 636f 6e73 7472 6169 6e74 0a69  ies_constraint.i
+00000230: 6d70 6f72 7420 626c 5f6f 7065 7261 746f  mport bl_operato
+00000240: 7273 2e75 7365 7270 7265 660a 696d 706f  rs.userpref.impo
+00000250: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
+00000260: 6965 735f 6461 7461 5f6c 6967 6874 7072  ies_data_lightpr
+00000270: 6f62 650a 696d 706f 7274 2062 6c5f 7569  obe.import bl_ui
+00000280: 2e73 7061 6365 5f64 6f70 6573 6865 6574  .space_dopesheet
+00000290: 0a69 6d70 6f72 7420 626c 5f75 692e 7370  .import bl_ui.sp
+000002a0: 6163 655f 7465 7874 0a69 6d70 6f72 7420  ace_text.import 
+000002b0: 626c 5f6f 7065 7261 746f 7273 2e73 7072  bl_operators.spr
+000002c0: 6561 6473 6865 6574 0a69 6d70 6f72 7420  eadsheet.import 
+000002d0: 626c 5f75 692e 7370 6163 655f 6e6c 610a  bl_ui.space_nla.
+000002e0: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
+000002f0: 7065 7274 6965 735f 7061 696e 745f 636f  perties_paint_co
+00000300: 6d6d 6f6e 0a69 6d70 6f72 7420 626c 5f75  mmon.import bl_u
+00000310: 690a 696d 706f 7274 2062 6c5f 7569 2e70  i.import bl_ui.p
+00000320: 726f 7065 7274 6965 735f 6f62 6a65 6374  roperties_object
+00000330: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
+00000340: 6f70 6572 7469 6573 5f76 6965 775f 6c61  operties_view_la
+00000350: 7965 720a 696d 706f 7274 2062 6c5f 7569  yer.import bl_ui
+00000360: 2e70 726f 7065 7274 6965 735f 6461 7461  .properties_data
+00000370: 5f63 7572 7665 730a 696d 706f 7274 2062  _curves.import b
+00000380: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
+00000390: 6461 7461 5f73 6861 6465 7266 780a 696d  data_shaderfx.im
+000003a0: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
+000003b0: 7274 6965 735f 6461 7461 5f63 616d 6572  rties_data_camer
+000003c0: 610a 696d 706f 7274 2062 6c5f 7569 2e70  a.import bl_ui.p
+000003d0: 726f 7065 7274 6965 735f 6d61 736b 5f63  roperties_mask_c
+000003e0: 6f6d 6d6f 6e0a 696d 706f 7274 2062 6c5f  ommon.import bl_
+000003f0: 7569 2e70 726f 7065 7274 6965 735f 6461  ui.properties_da
+00000400: 7461 5f76 6f6c 756d 650a 696d 706f 7274  ta_volume.import
+00000410: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
+00000420: 735f 6672 6565 7374 796c 650a 696d 706f  s_freestyle.impo
+00000430: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
+00000440: 6965 735f 6461 7461 5f6c 6967 6874 0a69  ies_data_light.i
+00000450: 6d70 6f72 7420 626c 5f6f 7065 7261 746f  mport bl_operato
+00000460: 7273 2e63 6c69 700a 696d 706f 7274 2062  rs.clip.import b
+00000470: 6c5f 7569 2e73 7061 6365 5f70 726f 7065  l_ui.space_prope
+00000480: 7274 6965 730a 696d 706f 7274 2062 6c5f  rties.import bl_
+00000490: 7569 2e73 7061 6365 5f69 6d61 6765 0a69  ui.space_image.i
+000004a0: 6d70 6f72 7420 626c 5f6f 7065 7261 746f  mport bl_operato
+000004b0: 7273 2e66 7265 6573 7479 6c65 0a69 6d70  rs.freestyle.imp
+000004c0: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
+000004d0: 7469 6573 5f70 6879 7369 6373 5f72 6967  ties_physics_rig
+000004e0: 6964 626f 6479 0a69 6d70 6f72 7420 626c  idbody.import bl
+000004f0: 5f75 692e 6e6f 6465 5f61 6464 5f6d 656e  _ui.node_add_men
+00000500: 755f 6765 6f6d 6574 7279 0a69 6d70 6f72  u_geometry.impor
+00000510: 7420 626c 5f75 692e 7370 6163 655f 746f  t bl_ui.space_to
+00000520: 7062 6172 0a69 6d70 6f72 7420 626c 5f75  pbar.import bl_u
+00000530: 692e 7370 6163 655f 6f75 746c 696e 6572  i.space_outliner
+00000540: 0a69 6d70 6f72 7420 626c 5f75 692e 7370  .import bl_ui.sp
+00000550: 6163 655f 7573 6572 7072 6566 0a69 6d70  ace_userpref.imp
+00000560: 6f72 7420 626c 5f75 692e 7370 6163 655f  ort bl_ui.space_
+00000570: 7669 6577 3364 5f74 6f6f 6c62 6172 0a69  view3d_toolbar.i
+00000580: 6d70 6f72 7420 626c 5f75 692e 7370 6163  mport bl_ui.spac
+00000590: 655f 7469 6d65 0a69 6d70 6f72 7420 626c  e_time.import bl
+000005a0: 5f75 692e 7072 6f70 6572 7469 6573 5f64  _ui.properties_d
+000005b0: 6174 615f 6172 6d61 7475 7265 0a69 6d70  ata_armature.imp
+000005c0: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
+000005d0: 7469 6573 5f64 6174 615f 6770 656e 6369  ties_data_gpenci
+000005e0: 6c0a 696d 706f 7274 2062 6c5f 7569 2e70  l.import bl_ui.p
+000005f0: 726f 7065 7274 6965 735f 776f 726c 640a  roperties_world.
+00000600: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
+00000610: 7065 7274 6965 735f 7068 7973 6963 735f  perties_physics_
+00000620: 636c 6f74 680a 696d 706f 7274 2062 6c5f  cloth.import bl_
+00000630: 7569 2e70 726f 7065 7274 6965 735f 7068  ui.properties_ph
+00000640: 7973 6963 735f 7269 6769 6462 6f64 795f  ysics_rigidbody_
+00000650: 636f 6e73 7472 6169 6e74 0a69 6d70 6f72  constraint.impor
+00000660: 7420 626c 5f6f 7065 7261 746f 7273 2e61  t bl_operators.a
+00000670: 6e69 6d0a 696d 706f 7274 2062 6c5f 6f70  nim.import bl_op
+00000680: 6572 6174 6f72 732e 6e6f 6465 0a69 6d70  erators.node.imp
+00000690: 6f72 7420 626c 5f75 692e 7370 6163 655f  ort bl_ui.space_
+000006a0: 6669 6c65 6272 6f77 7365 720a 696d 706f  filebrowser.impo
+000006b0: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
+000006c0: 6965 735f 7068 7973 6963 735f 636f 6d6d  ies_physics_comm
+000006d0: 6f6e 0a69 6d70 6f72 7420 626c 5f75 692e  on.import bl_ui.
+000006e0: 7072 6f70 6572 7469 6573 5f64 6174 615f  properties_data_
+000006f0: 6772 6561 7365 5f70 656e 6369 6c0a 696d  grease_pencil.im
+00000700: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
+00000710: 7274 6965 735f 7068 7973 6963 735f 736f  rties_physics_so
+00000720: 6674 626f 6479 0a69 6d70 6f72 7420 626c  ftbody.import bl
+00000730: 5f75 692e 6765 6e65 7269 635f 7569 5f6c  _ui.generic_ui_l
+00000740: 6973 740a 696d 706f 7274 2062 6c5f 7569  ist.import bl_ui
+00000750: 2e70 726f 7065 7274 6965 735f 6f75 7470  .properties_outp
+00000760: 7574 0a69 6d70 6f72 7420 626c 5f75 692e  ut.import bl_ui.
+00000770: 7072 6f70 6572 7469 6573 5f6d 6174 6572  properties_mater
+00000780: 6961 6c5f 6770 656e 6369 6c0a 696d 706f  ial_gpencil.impo
+00000790: 7274 2062 6c5f 6f70 6572 6174 6f72 732e  rt bl_operators.
+000007a0: 6f62 6a65 6374 0a69 6d70 6f72 7420 626c  object.import bl
+000007b0: 5f75 692e 7072 6f70 6572 7469 6573 5f64  _ui.properties_d
+000007c0: 6174 615f 6d65 7368 0a69 6d70 6f72 7420  ata_mesh.import 
+000007d0: 626c 5f75 692e 7370 6163 655f 7370 7265  bl_ui.space_spre
+000007e0: 6164 7368 6565 740a 696d 706f 7274 2062  adsheet.import b
+000007f0: 6c5f 6f70 6572 6174 6f72 732e 7465 7874  l_operators.text
+00000800: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
+00000810: 6f70 6572 7469 6573 5f70 6879 7369 6373  operties_physics
+00000820: 5f66 6c75 6964 0a69 6d70 6f72 7420 626c  _fluid.import bl
+00000830: 5f75 692e 7072 6f70 6572 7469 6573 5f64  _ui.properties_d
+00000840: 6174 615f 706f 696e 7463 6c6f 7564 0a69  ata_pointcloud.i
+00000850: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
+00000860: 6572 7469 6573 5f64 6174 615f 7370 6561  erties_data_spea
+00000870: 6b65 720a 696d 706f 7274 2062 6c5f 7569  ker.import bl_ui
+00000880: 2e70 726f 7065 7274 6965 735f 776f 726b  .properties_work
+00000890: 7370 6163 650a 696d 706f 7274 2062 6c5f  space.import bl_
+000008a0: 7569 2e70 726f 7065 7274 6965 735f 7068  ui.properties_ph
+000008b0: 7973 6963 735f 6669 656c 640a 696d 706f  ysics_field.impo
+000008c0: 7274 2062 6c5f 7569 2e73 7061 6365 5f6e  rt bl_ui.space_n
+000008d0: 6f64 650a 696d 706f 7274 2062 6c5f 7569  ode.import bl_ui
+000008e0: 2e70 726f 7065 7274 6965 735f 7068 7973  .properties_phys
+000008f0: 6963 735f 6479 6e61 6d69 6370 6169 6e74  ics_dynamicpaint
+00000900: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
+00000910: 6f70 6572 7469 6573 5f74 6578 7475 7265  operties_texture
+00000920: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
+00000930: 6f70 6572 7469 6573 5f63 6f6c 6c65 6374  operties_collect
+00000940: 696f 6e0a 696d 706f 7274 2062 6c5f 7569  ion.import bl_ui
+00000950: 2e73 7061 6365 5f73 7461 7475 7362 6172  .space_statusbar
+00000960: 0a69 6d70 6f72 7420 626c 5f6f 7065 7261  .import bl_opera
+00000970: 746f 7273 2e66 696c 650a 696d 706f 7274  tors.file.import
+00000980: 2062 6c5f 7569 2e73 7061 6365 5f63 6c69   bl_ui.space_cli
+00000990: 700a 696d 706f 7274 2062 6c5f 7569 2e73  p.import bl_ui.s
+000009a0: 7061 6365 5f69 6e66 6f0a 696d 706f 7274  pace_info.import
+000009b0: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
+000009c0: 735f 6461 7461 5f6d 6574 6162 616c 6c0a  s_data_metaball.
+000009d0: 696d 706f 7274 2062 6c5f 6f70 6572 6174  import bl_operat
+000009e0: 6f72 732e 7669 6577 3364 0a69 6d70 6f72  ors.view3d.impor
+000009f0: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
+00000a00: 6573 5f64 6174 615f 656d 7074 790a 696d  es_data_empty.im
+00000a10: 706f 7274 2062 6c5f 7569 2e73 7061 6365  port bl_ui.space
+00000a20: 5f74 6f6f 6c73 7973 7465 6d5f 746f 6f6c  _toolsystem_tool
+00000a30: 6261 720a 696d 706f 7274 2062 6c5f 7569  bar.import bl_ui
+00000a40: 2e73 7061 6365 5f73 6571 7565 6e63 6572  .space_sequencer
+00000a50: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
+00000a60: 6f70 6572 7469 6573 5f64 6174 615f 6d6f  operties_data_mo
+00000a70: 6469 6669 6572 0a69 6d70 6f72 7420 626c  difier.import bl
+00000a80: 5f75 692e 7072 6f70 6572 7469 6573 5f70  _ui.properties_p
+00000a90: 6879 7369 6373 5f67 656f 6d65 7472 795f  hysics_geometry_
+00000aa0: 6e6f 6465 730a 696d 706f 7274 2062 6c5f  nodes.import bl_
+00000ab0: 7569 2e70 726f 7065 7274 6965 735f 7265  ui.properties_re
+00000ac0: 6e64 6572 0a0a 4765 6e65 7269 6354 7970  nder..GenericTyp
 00000ad0: 6520 3d20 7479 7069 6e67 2e54 7970 6556  e = typing.TypeV
 00000ae0: 6172 2822 4765 6e65 7269 6354 7970 6522  ar("GenericType"
 00000af0: 290a 0a0a 636c 6173 7320 6270 795f 7072  )...class bpy_pr
 00000b00: 6f70 5f63 6f6c 6c65 6374 696f 6e28 7479  op_collection(ty
 00000b10: 7069 6e67 2e47 656e 6572 6963 5b47 656e  ping.Generic[Gen
 00000b20: 6572 6963 5479 7065 5d29 3a0a 2020 2020  ericType]):.    
 00000b30: 2727 2720 6275 696c 742d 696e 2063 6c61  ''' built-in cla
@@ -216803,1815 +216803,1820 @@
 0034ee20: 656e 7461 7469 6f6e 735f 7069 6527 203d  entations_pie' =
 0034ee30: 204e 6f6e 650a 0a56 4945 5733 445f 4d54   None..VIEW3D_MT
 0034ee40: 5f70 6169 6e74 5f67 7065 6e63 696c 3a20  _paint_gpencil: 
 0034ee50: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
 0034ee60: 7733 642e 5649 4557 3344 5f4d 545f 7061  w3d.VIEW3D_MT_pa
 0034ee70: 696e 745f 6770 656e 6369 6c27 203d 204e  int_gpencil' = N
 0034ee80: 6f6e 650a 0a56 4945 5733 445f 4d54 5f70  one..VIEW3D_MT_p
-0034ee90: 6169 6e74 5f76 6572 7465 783a 2027 626c  aint_vertex: 'bl
-0034eea0: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
-0034eeb0: 2e56 4945 5733 445f 4d54 5f70 6169 6e74  .VIEW3D_MT_paint
-0034eec0: 5f76 6572 7465 7827 203d 204e 6f6e 650a  _vertex' = None.
-0034eed0: 0a56 4945 5733 445f 4d54 5f70 6169 6e74  .VIEW3D_MT_paint
-0034eee0: 5f77 6569 6768 743a 2027 626c 5f75 692e  _weight: 'bl_ui.
-0034eef0: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
-0034ef00: 5733 445f 4d54 5f70 6169 6e74 5f77 6569  W3D_MT_paint_wei
-0034ef10: 6768 7427 203d 204e 6f6e 650a 0a56 4945  ght' = None..VIE
-0034ef20: 5733 445f 4d54 5f70 6169 6e74 5f77 6569  W3D_MT_paint_wei
-0034ef30: 6768 745f 6c6f 636b 3a20 2762 6c5f 7569  ght_lock: 'bl_ui
-0034ef40: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
-0034ef50: 4557 3344 5f4d 545f 7061 696e 745f 7765  EW3D_MT_paint_we
-0034ef60: 6967 6874 5f6c 6f63 6b27 203d 204e 6f6e  ight_lock' = Non
-0034ef70: 650a 0a56 4945 5733 445f 4d54 5f70 6172  e..VIEW3D_MT_par
-0034ef80: 7469 636c 653a 2027 626c 5f75 692e 7370  ticle: 'bl_ui.sp
-0034ef90: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
-0034efa0: 445f 4d54 5f70 6172 7469 636c 6527 203d  D_MT_particle' =
-0034efb0: 204e 6f6e 650a 0a56 4945 5733 445f 4d54   None..VIEW3D_MT
-0034efc0: 5f70 6172 7469 636c 655f 636f 6e74 6578  _particle_contex
-0034efd0: 745f 6d65 6e75 3a20 2762 6c5f 7569 2e73  t_menu: 'bl_ui.s
-0034efe0: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
-0034eff0: 3344 5f4d 545f 7061 7274 6963 6c65 5f63  3D_MT_particle_c
-0034f000: 6f6e 7465 7874 5f6d 656e 7527 203d 204e  ontext_menu' = N
-0034f010: 6f6e 650a 0a56 4945 5733 445f 4d54 5f70  one..VIEW3D_MT_p
-0034f020: 6172 7469 636c 655f 7368 6f77 6869 6465  article_showhide
+0034ee90: 6169 6e74 5f67 7265 6173 655f 7065 6e63  aint_grease_penc
+0034eea0: 696c 3a20 2762 6c5f 7569 2e73 7061 6365  il: 'bl_ui.space
+0034eeb0: 5f76 6965 7733 642e 5649 4557 3344 5f4d  _view3d.VIEW3D_M
+0034eec0: 545f 7061 696e 745f 6772 6561 7365 5f70  T_paint_grease_p
+0034eed0: 656e 6369 6c27 203d 204e 6f6e 650a 0a56  encil' = None..V
+0034eee0: 4945 5733 445f 4d54 5f70 6169 6e74 5f76  IEW3D_MT_paint_v
+0034eef0: 6572 7465 783a 2027 626c 5f75 692e 7370  ertex: 'bl_ui.sp
+0034ef00: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
+0034ef10: 445f 4d54 5f70 6169 6e74 5f76 6572 7465  D_MT_paint_verte
+0034ef20: 7827 203d 204e 6f6e 650a 0a56 4945 5733  x' = None..VIEW3
+0034ef30: 445f 4d54 5f70 6169 6e74 5f77 6569 6768  D_MT_paint_weigh
+0034ef40: 743a 2027 626c 5f75 692e 7370 6163 655f  t: 'bl_ui.space_
+0034ef50: 7669 6577 3364 2e56 4945 5733 445f 4d54  view3d.VIEW3D_MT
+0034ef60: 5f70 6169 6e74 5f77 6569 6768 7427 203d  _paint_weight' =
+0034ef70: 204e 6f6e 650a 0a56 4945 5733 445f 4d54   None..VIEW3D_MT
+0034ef80: 5f70 6169 6e74 5f77 6569 6768 745f 6c6f  _paint_weight_lo
+0034ef90: 636b 3a20 2762 6c5f 7569 2e73 7061 6365  ck: 'bl_ui.space
+0034efa0: 5f76 6965 7733 642e 5649 4557 3344 5f4d  _view3d.VIEW3D_M
+0034efb0: 545f 7061 696e 745f 7765 6967 6874 5f6c  T_paint_weight_l
+0034efc0: 6f63 6b27 203d 204e 6f6e 650a 0a56 4945  ock' = None..VIE
+0034efd0: 5733 445f 4d54 5f70 6172 7469 636c 653a  W3D_MT_particle:
+0034efe0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+0034eff0: 6577 3364 2e56 4945 5733 445f 4d54 5f70  ew3d.VIEW3D_MT_p
+0034f000: 6172 7469 636c 6527 203d 204e 6f6e 650a  article' = None.
+0034f010: 0a56 4945 5733 445f 4d54 5f70 6172 7469  .VIEW3D_MT_parti
+0034f020: 636c 655f 636f 6e74 6578 745f 6d65 6e75  cle_context_menu
 0034f030: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
 0034f040: 6965 7733 642e 5649 4557 3344 5f4d 545f  iew3d.VIEW3D_MT_
-0034f050: 7061 7274 6963 6c65 5f73 686f 7768 6964  particle_showhid
-0034f060: 6527 203d 204e 6f6e 650a 0a56 4945 5733  e' = None..VIEW3
-0034f070: 445f 4d54 5f70 6976 6f74 5f70 6965 3a20  D_MT_pivot_pie: 
-0034f080: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-0034f090: 7733 642e 5649 4557 3344 5f4d 545f 7069  w3d.VIEW3D_MT_pi
-0034f0a0: 766f 745f 7069 6527 203d 204e 6f6e 650a  vot_pie' = None.
-0034f0b0: 0a56 4945 5733 445f 4d54 5f70 6f73 653a  .VIEW3D_MT_pose:
-0034f0c0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-0034f0d0: 6577 3364 2e56 4945 5733 445f 4d54 5f70  ew3d.VIEW3D_MT_p
-0034f0e0: 6f73 6527 203d 204e 6f6e 650a 0a56 4945  ose' = None..VIE
-0034f0f0: 5733 445f 4d54 5f70 6f73 655f 6170 706c  W3D_MT_pose_appl
-0034f100: 793a 2027 626c 5f75 692e 7370 6163 655f  y: 'bl_ui.space_
-0034f110: 7669 6577 3364 2e56 4945 5733 445f 4d54  view3d.VIEW3D_MT
-0034f120: 5f70 6f73 655f 6170 706c 7927 203d 204e  _pose_apply' = N
-0034f130: 6f6e 650a 0a56 4945 5733 445f 4d54 5f70  one..VIEW3D_MT_p
-0034f140: 6f73 655f 636f 6e73 7472 6169 6e74 733a  ose_constraints:
-0034f150: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-0034f160: 6577 3364 2e56 4945 5733 445f 4d54 5f70  ew3d.VIEW3D_MT_p
-0034f170: 6f73 655f 636f 6e73 7472 6169 6e74 7327  ose_constraints'
-0034f180: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
-0034f190: 4d54 5f70 6f73 655f 636f 6e74 6578 745f  MT_pose_context_
-0034f1a0: 6d65 6e75 3a20 2762 6c5f 7569 2e73 7061  menu: 'bl_ui.spa
-0034f1b0: 6365 5f76 6965 7733 642e 5649 4557 3344  ce_view3d.VIEW3D
-0034f1c0: 5f4d 545f 706f 7365 5f63 6f6e 7465 7874  _MT_pose_context
-0034f1d0: 5f6d 656e 7527 203d 204e 6f6e 650a 0a56  _menu' = None..V
-0034f1e0: 4945 5733 445f 4d54 5f70 6f73 655f 6772  IEW3D_MT_pose_gr
-0034f1f0: 6f75 703a 2027 626c 5f75 692e 7370 6163  oup: 'bl_ui.spac
-0034f200: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
-0034f210: 4d54 5f70 6f73 655f 6772 6f75 7027 203d  MT_pose_group' =
-0034f220: 204e 6f6e 650a 0a56 4945 5733 445f 4d54   None..VIEW3D_MT
-0034f230: 5f70 6f73 655f 696b 3a20 2762 6c5f 7569  _pose_ik: 'bl_ui
-0034f240: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
-0034f250: 4557 3344 5f4d 545f 706f 7365 5f69 6b27  EW3D_MT_pose_ik'
-0034f260: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
-0034f270: 4d54 5f70 6f73 655f 6d6f 7469 6f6e 3a20  MT_pose_motion: 
-0034f280: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-0034f290: 7733 642e 5649 4557 3344 5f4d 545f 706f  w3d.VIEW3D_MT_po
-0034f2a0: 7365 5f6d 6f74 696f 6e27 203d 204e 6f6e  se_motion' = Non
-0034f2b0: 650a 0a56 4945 5733 445f 4d54 5f70 6f73  e..VIEW3D_MT_pos
-0034f2c0: 655f 6e61 6d65 733a 2027 626c 5f75 692e  e_names: 'bl_ui.
-0034f2d0: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
-0034f2e0: 5733 445f 4d54 5f70 6f73 655f 6e61 6d65  W3D_MT_pose_name
-0034f2f0: 7327 203d 204e 6f6e 650a 0a56 4945 5733  s' = None..VIEW3
-0034f300: 445f 4d54 5f70 6f73 655f 7072 6f70 6167  D_MT_pose_propag
-0034f310: 6174 653a 2027 626c 5f75 692e 7370 6163  ate: 'bl_ui.spac
-0034f320: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
-0034f330: 4d54 5f70 6f73 655f 7072 6f70 6167 6174  MT_pose_propagat
-0034f340: 6527 203d 204e 6f6e 650a 0a56 4945 5733  e' = None..VIEW3
-0034f350: 445f 4d54 5f70 6f73 655f 7368 6f77 6869  D_MT_pose_showhi
-0034f360: 6465 3a20 2762 6c5f 7569 2e73 7061 6365  de: 'bl_ui.space
-0034f370: 5f76 6965 7733 642e 5649 4557 3344 5f4d  _view3d.VIEW3D_M
-0034f380: 545f 706f 7365 5f73 686f 7768 6964 6527  T_pose_showhide'
-0034f390: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
-0034f3a0: 4d54 5f70 6f73 655f 736c 6964 653a 2027  MT_pose_slide: '
-0034f3b0: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
-0034f3c0: 3364 2e56 4945 5733 445f 4d54 5f70 6f73  3d.VIEW3D_MT_pos
-0034f3d0: 655f 736c 6964 6527 203d 204e 6f6e 650a  e_slide' = None.
-0034f3e0: 0a56 4945 5733 445f 4d54 5f70 6f73 655f  .VIEW3D_MT_pose_
-0034f3f0: 7472 616e 7366 6f72 6d3a 2027 626c 5f75  transform: 'bl_u
-0034f400: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
-0034f410: 4945 5733 445f 4d54 5f70 6f73 655f 7472  IEW3D_MT_pose_tr
-0034f420: 616e 7366 6f72 6d27 203d 204e 6f6e 650a  ansform' = None.
-0034f430: 0a56 4945 5733 445f 4d54 5f70 726f 706f  .VIEW3D_MT_propo
-0034f440: 7274 696f 6e61 6c5f 6564 6974 696e 675f  rtional_editing_
-0034f450: 6661 6c6c 6f66 665f 7069 653a 2027 626c  falloff_pie: 'bl
-0034f460: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
-0034f470: 2e56 4945 5733 445f 4d54 5f70 726f 706f  .VIEW3D_MT_propo
-0034f480: 7274 696f 6e61 6c5f 6564 6974 696e 675f  rtional_editing_
-0034f490: 6661 6c6c 6f66 665f 7069 6527 203d 204e  falloff_pie' = N
-0034f4a0: 6f6e 650a 0a56 4945 5733 445f 4d54 5f72  one..VIEW3D_MT_r
-0034f4b0: 616e 646f 6d5f 6d61 736b 3a20 2762 6c5f  andom_mask: 'bl_
-0034f4c0: 7569 2e73 7061 6365 5f76 6965 7733 642e  ui.space_view3d.
-0034f4d0: 5649 4557 3344 5f4d 545f 7261 6e64 6f6d  VIEW3D_MT_random
-0034f4e0: 5f6d 6173 6b27 203d 204e 6f6e 650a 0a56  _mask' = None..V
-0034f4f0: 4945 5733 445f 4d54 5f73 6375 6c70 743a  IEW3D_MT_sculpt:
-0034f500: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-0034f510: 6577 3364 2e56 4945 5733 445f 4d54 5f73  ew3d.VIEW3D_MT_s
-0034f520: 6375 6c70 7427 203d 204e 6f6e 650a 0a56  culpt' = None..V
-0034f530: 4945 5733 445f 4d54 5f73 6375 6c70 745f  IEW3D_MT_sculpt_
-0034f540: 6175 746f 6d61 736b 696e 675f 7069 653a  automasking_pie:
-0034f550: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-0034f560: 6577 3364 2e56 4945 5733 445f 4d54 5f73  ew3d.VIEW3D_MT_s
-0034f570: 6375 6c70 745f 6175 746f 6d61 736b 696e  culpt_automaskin
-0034f580: 675f 7069 6527 203d 204e 6f6e 650a 0a56  g_pie' = None..V
-0034f590: 4945 5733 445f 4d54 5f73 6375 6c70 745f  IEW3D_MT_sculpt_
-0034f5a0: 6375 7276 6573 3a20 2762 6c5f 7569 2e73  curves: 'bl_ui.s
-0034f5b0: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
-0034f5c0: 3344 5f4d 545f 7363 756c 7074 5f63 7572  3D_MT_sculpt_cur
-0034f5d0: 7665 7327 203d 204e 6f6e 650a 0a56 4945  ves' = None..VIE
-0034f5e0: 5733 445f 4d54 5f73 6375 6c70 745f 6661  W3D_MT_sculpt_fa
-0034f5f0: 6365 5f73 6574 735f 6564 6974 5f70 6965  ce_sets_edit_pie
+0034f050: 7061 7274 6963 6c65 5f63 6f6e 7465 7874  particle_context
+0034f060: 5f6d 656e 7527 203d 204e 6f6e 650a 0a56  _menu' = None..V
+0034f070: 4945 5733 445f 4d54 5f70 6172 7469 636c  IEW3D_MT_particl
+0034f080: 655f 7368 6f77 6869 6465 3a20 2762 6c5f  e_showhide: 'bl_
+0034f090: 7569 2e73 7061 6365 5f76 6965 7733 642e  ui.space_view3d.
+0034f0a0: 5649 4557 3344 5f4d 545f 7061 7274 6963  VIEW3D_MT_partic
+0034f0b0: 6c65 5f73 686f 7768 6964 6527 203d 204e  le_showhide' = N
+0034f0c0: 6f6e 650a 0a56 4945 5733 445f 4d54 5f70  one..VIEW3D_MT_p
+0034f0d0: 6976 6f74 5f70 6965 3a20 2762 6c5f 7569  ivot_pie: 'bl_ui
+0034f0e0: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
+0034f0f0: 4557 3344 5f4d 545f 7069 766f 745f 7069  EW3D_MT_pivot_pi
+0034f100: 6527 203d 204e 6f6e 650a 0a56 4945 5733  e' = None..VIEW3
+0034f110: 445f 4d54 5f70 6f73 653a 2027 626c 5f75  D_MT_pose: 'bl_u
+0034f120: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
+0034f130: 4945 5733 445f 4d54 5f70 6f73 6527 203d  IEW3D_MT_pose' =
+0034f140: 204e 6f6e 650a 0a56 4945 5733 445f 4d54   None..VIEW3D_MT
+0034f150: 5f70 6f73 655f 6170 706c 793a 2027 626c  _pose_apply: 'bl
+0034f160: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+0034f170: 2e56 4945 5733 445f 4d54 5f70 6f73 655f  .VIEW3D_MT_pose_
+0034f180: 6170 706c 7927 203d 204e 6f6e 650a 0a56  apply' = None..V
+0034f190: 4945 5733 445f 4d54 5f70 6f73 655f 636f  IEW3D_MT_pose_co
+0034f1a0: 6e73 7472 6169 6e74 733a 2027 626c 5f75  nstraints: 'bl_u
+0034f1b0: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
+0034f1c0: 4945 5733 445f 4d54 5f70 6f73 655f 636f  IEW3D_MT_pose_co
+0034f1d0: 6e73 7472 6169 6e74 7327 203d 204e 6f6e  nstraints' = Non
+0034f1e0: 650a 0a56 4945 5733 445f 4d54 5f70 6f73  e..VIEW3D_MT_pos
+0034f1f0: 655f 636f 6e74 6578 745f 6d65 6e75 3a20  e_context_menu: 
+0034f200: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
+0034f210: 7733 642e 5649 4557 3344 5f4d 545f 706f  w3d.VIEW3D_MT_po
+0034f220: 7365 5f63 6f6e 7465 7874 5f6d 656e 7527  se_context_menu'
+0034f230: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
+0034f240: 4d54 5f70 6f73 655f 6772 6f75 703a 2027  MT_pose_group: '
+0034f250: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
+0034f260: 3364 2e56 4945 5733 445f 4d54 5f70 6f73  3d.VIEW3D_MT_pos
+0034f270: 655f 6772 6f75 7027 203d 204e 6f6e 650a  e_group' = None.
+0034f280: 0a56 4945 5733 445f 4d54 5f70 6f73 655f  .VIEW3D_MT_pose_
+0034f290: 696b 3a20 2762 6c5f 7569 2e73 7061 6365  ik: 'bl_ui.space
+0034f2a0: 5f76 6965 7733 642e 5649 4557 3344 5f4d  _view3d.VIEW3D_M
+0034f2b0: 545f 706f 7365 5f69 6b27 203d 204e 6f6e  T_pose_ik' = Non
+0034f2c0: 650a 0a56 4945 5733 445f 4d54 5f70 6f73  e..VIEW3D_MT_pos
+0034f2d0: 655f 6d6f 7469 6f6e 3a20 2762 6c5f 7569  e_motion: 'bl_ui
+0034f2e0: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
+0034f2f0: 4557 3344 5f4d 545f 706f 7365 5f6d 6f74  EW3D_MT_pose_mot
+0034f300: 696f 6e27 203d 204e 6f6e 650a 0a56 4945  ion' = None..VIE
+0034f310: 5733 445f 4d54 5f70 6f73 655f 6e61 6d65  W3D_MT_pose_name
+0034f320: 733a 2027 626c 5f75 692e 7370 6163 655f  s: 'bl_ui.space_
+0034f330: 7669 6577 3364 2e56 4945 5733 445f 4d54  view3d.VIEW3D_MT
+0034f340: 5f70 6f73 655f 6e61 6d65 7327 203d 204e  _pose_names' = N
+0034f350: 6f6e 650a 0a56 4945 5733 445f 4d54 5f70  one..VIEW3D_MT_p
+0034f360: 6f73 655f 7072 6f70 6167 6174 653a 2027  ose_propagate: '
+0034f370: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
+0034f380: 3364 2e56 4945 5733 445f 4d54 5f70 6f73  3d.VIEW3D_MT_pos
+0034f390: 655f 7072 6f70 6167 6174 6527 203d 204e  e_propagate' = N
+0034f3a0: 6f6e 650a 0a56 4945 5733 445f 4d54 5f70  one..VIEW3D_MT_p
+0034f3b0: 6f73 655f 7368 6f77 6869 6465 3a20 2762  ose_showhide: 'b
+0034f3c0: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+0034f3d0: 642e 5649 4557 3344 5f4d 545f 706f 7365  d.VIEW3D_MT_pose
+0034f3e0: 5f73 686f 7768 6964 6527 203d 204e 6f6e  _showhide' = Non
+0034f3f0: 650a 0a56 4945 5733 445f 4d54 5f70 6f73  e..VIEW3D_MT_pos
+0034f400: 655f 736c 6964 653a 2027 626c 5f75 692e  e_slide: 'bl_ui.
+0034f410: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
+0034f420: 5733 445f 4d54 5f70 6f73 655f 736c 6964  W3D_MT_pose_slid
+0034f430: 6527 203d 204e 6f6e 650a 0a56 4945 5733  e' = None..VIEW3
+0034f440: 445f 4d54 5f70 6f73 655f 7472 616e 7366  D_MT_pose_transf
+0034f450: 6f72 6d3a 2027 626c 5f75 692e 7370 6163  orm: 'bl_ui.spac
+0034f460: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
+0034f470: 4d54 5f70 6f73 655f 7472 616e 7366 6f72  MT_pose_transfor
+0034f480: 6d27 203d 204e 6f6e 650a 0a56 4945 5733  m' = None..VIEW3
+0034f490: 445f 4d54 5f70 726f 706f 7274 696f 6e61  D_MT_proportiona
+0034f4a0: 6c5f 6564 6974 696e 675f 6661 6c6c 6f66  l_editing_fallof
+0034f4b0: 665f 7069 653a 2027 626c 5f75 692e 7370  f_pie: 'bl_ui.sp
+0034f4c0: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
+0034f4d0: 445f 4d54 5f70 726f 706f 7274 696f 6e61  D_MT_proportiona
+0034f4e0: 6c5f 6564 6974 696e 675f 6661 6c6c 6f66  l_editing_fallof
+0034f4f0: 665f 7069 6527 203d 204e 6f6e 650a 0a56  f_pie' = None..V
+0034f500: 4945 5733 445f 4d54 5f72 616e 646f 6d5f  IEW3D_MT_random_
+0034f510: 6d61 736b 3a20 2762 6c5f 7569 2e73 7061  mask: 'bl_ui.spa
+0034f520: 6365 5f76 6965 7733 642e 5649 4557 3344  ce_view3d.VIEW3D
+0034f530: 5f4d 545f 7261 6e64 6f6d 5f6d 6173 6b27  _MT_random_mask'
+0034f540: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
+0034f550: 4d54 5f73 6375 6c70 743a 2027 626c 5f75  MT_sculpt: 'bl_u
+0034f560: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
+0034f570: 4945 5733 445f 4d54 5f73 6375 6c70 7427  IEW3D_MT_sculpt'
+0034f580: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
+0034f590: 4d54 5f73 6375 6c70 745f 6175 746f 6d61  MT_sculpt_automa
+0034f5a0: 736b 696e 675f 7069 653a 2027 626c 5f75  sking_pie: 'bl_u
+0034f5b0: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
+0034f5c0: 4945 5733 445f 4d54 5f73 6375 6c70 745f  IEW3D_MT_sculpt_
+0034f5d0: 6175 746f 6d61 736b 696e 675f 7069 6527  automasking_pie'
+0034f5e0: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
+0034f5f0: 4d54 5f73 6375 6c70 745f 6375 7276 6573  MT_sculpt_curves
 0034f600: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
 0034f610: 6965 7733 642e 5649 4557 3344 5f4d 545f  iew3d.VIEW3D_MT_
-0034f620: 7363 756c 7074 5f66 6163 655f 7365 7473  sculpt_face_sets
-0034f630: 5f65 6469 745f 7069 6527 203d 204e 6f6e  _edit_pie' = Non
-0034f640: 650a 0a56 4945 5733 445f 4d54 5f73 6375  e..VIEW3D_MT_scu
-0034f650: 6c70 745f 6770 656e 6369 6c5f 6175 746f  lpt_gpencil_auto
-0034f660: 6d61 736b 696e 675f 7069 653a 2027 626c  masking_pie: 'bl
-0034f670: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
-0034f680: 2e56 4945 5733 445f 4d54 5f73 6375 6c70  .VIEW3D_MT_sculp
-0034f690: 745f 6770 656e 6369 6c5f 6175 746f 6d61  t_gpencil_automa
-0034f6a0: 736b 696e 675f 7069 6527 203d 204e 6f6e  sking_pie' = Non
-0034f6b0: 650a 0a56 4945 5733 445f 4d54 5f73 6375  e..VIEW3D_MT_scu
-0034f6c0: 6c70 745f 6d61 736b 5f65 6469 745f 7069  lpt_mask_edit_pi
-0034f6d0: 653a 2027 626c 5f75 692e 7370 6163 655f  e: 'bl_ui.space_
-0034f6e0: 7669 6577 3364 2e56 4945 5733 445f 4d54  view3d.VIEW3D_MT
-0034f6f0: 5f73 6375 6c70 745f 6d61 736b 5f65 6469  _sculpt_mask_edi
-0034f700: 745f 7069 6527 203d 204e 6f6e 650a 0a56  t_pie' = None..V
-0034f710: 4945 5733 445f 4d54 5f73 6375 6c70 745f  IEW3D_MT_sculpt_
-0034f720: 7365 745f 7069 766f 743a 2027 626c 5f75  set_pivot: 'bl_u
-0034f730: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
-0034f740: 4945 5733 445f 4d54 5f73 6375 6c70 745f  IEW3D_MT_sculpt_
-0034f750: 7365 745f 7069 766f 7427 203d 204e 6f6e  set_pivot' = Non
-0034f760: 650a 0a56 4945 5733 445f 4d54 5f73 656c  e..VIEW3D_MT_sel
-0034f770: 6563 745f 6564 6974 5f61 726d 6174 7572  ect_edit_armatur
-0034f780: 653a 2027 626c 5f75 692e 7370 6163 655f  e: 'bl_ui.space_
-0034f790: 7669 6577 3364 2e56 4945 5733 445f 4d54  view3d.VIEW3D_MT
-0034f7a0: 5f73 656c 6563 745f 6564 6974 5f61 726d  _select_edit_arm
-0034f7b0: 6174 7572 6527 203d 204e 6f6e 650a 0a56  ature' = None..V
-0034f7c0: 4945 5733 445f 4d54 5f73 656c 6563 745f  IEW3D_MT_select_
-0034f7d0: 6564 6974 5f63 7572 7665 3a20 2762 6c5f  edit_curve: 'bl_
-0034f7e0: 7569 2e73 7061 6365 5f76 6965 7733 642e  ui.space_view3d.
-0034f7f0: 5649 4557 3344 5f4d 545f 7365 6c65 6374  VIEW3D_MT_select
-0034f800: 5f65 6469 745f 6375 7276 6527 203d 204e  _edit_curve' = N
-0034f810: 6f6e 650a 0a56 4945 5733 445f 4d54 5f73  one..VIEW3D_MT_s
-0034f820: 656c 6563 745f 6564 6974 5f63 7572 7665  elect_edit_curve
-0034f830: 733a 2027 626c 5f75 692e 7370 6163 655f  s: 'bl_ui.space_
-0034f840: 7669 6577 3364 2e56 4945 5733 445f 4d54  view3d.VIEW3D_MT
-0034f850: 5f73 656c 6563 745f 6564 6974 5f63 7572  _select_edit_cur
-0034f860: 7665 7327 203d 204e 6f6e 650a 0a56 4945  ves' = None..VIE
-0034f870: 5733 445f 4d54 5f73 656c 6563 745f 6564  W3D_MT_select_ed
-0034f880: 6974 5f67 7065 6e63 696c 3a20 2762 6c5f  it_gpencil: 'bl_
-0034f890: 7569 2e73 7061 6365 5f76 6965 7733 642e  ui.space_view3d.
-0034f8a0: 5649 4557 3344 5f4d 545f 7365 6c65 6374  VIEW3D_MT_select
-0034f8b0: 5f65 6469 745f 6770 656e 6369 6c27 203d  _edit_gpencil' =
+0034f620: 7363 756c 7074 5f63 7572 7665 7327 203d  sculpt_curves' =
+0034f630: 204e 6f6e 650a 0a56 4945 5733 445f 4d54   None..VIEW3D_MT
+0034f640: 5f73 6375 6c70 745f 6661 6365 5f73 6574  _sculpt_face_set
+0034f650: 735f 6564 6974 5f70 6965 3a20 2762 6c5f  s_edit_pie: 'bl_
+0034f660: 7569 2e73 7061 6365 5f76 6965 7733 642e  ui.space_view3d.
+0034f670: 5649 4557 3344 5f4d 545f 7363 756c 7074  VIEW3D_MT_sculpt
+0034f680: 5f66 6163 655f 7365 7473 5f65 6469 745f  _face_sets_edit_
+0034f690: 7069 6527 203d 204e 6f6e 650a 0a56 4945  pie' = None..VIE
+0034f6a0: 5733 445f 4d54 5f73 6375 6c70 745f 6770  W3D_MT_sculpt_gp
+0034f6b0: 656e 6369 6c5f 6175 746f 6d61 736b 696e  encil_automaskin
+0034f6c0: 675f 7069 653a 2027 626c 5f75 692e 7370  g_pie: 'bl_ui.sp
+0034f6d0: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
+0034f6e0: 445f 4d54 5f73 6375 6c70 745f 6770 656e  D_MT_sculpt_gpen
+0034f6f0: 6369 6c5f 6175 746f 6d61 736b 696e 675f  cil_automasking_
+0034f700: 7069 6527 203d 204e 6f6e 650a 0a56 4945  pie' = None..VIE
+0034f710: 5733 445f 4d54 5f73 6375 6c70 745f 6d61  W3D_MT_sculpt_ma
+0034f720: 736b 5f65 6469 745f 7069 653a 2027 626c  sk_edit_pie: 'bl
+0034f730: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+0034f740: 2e56 4945 5733 445f 4d54 5f73 6375 6c70  .VIEW3D_MT_sculp
+0034f750: 745f 6d61 736b 5f65 6469 745f 7069 6527  t_mask_edit_pie'
+0034f760: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
+0034f770: 4d54 5f73 6375 6c70 745f 7365 745f 7069  MT_sculpt_set_pi
+0034f780: 766f 743a 2027 626c 5f75 692e 7370 6163  vot: 'bl_ui.spac
+0034f790: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
+0034f7a0: 4d54 5f73 6375 6c70 745f 7365 745f 7069  MT_sculpt_set_pi
+0034f7b0: 766f 7427 203d 204e 6f6e 650a 0a56 4945  vot' = None..VIE
+0034f7c0: 5733 445f 4d54 5f73 656c 6563 745f 6564  W3D_MT_select_ed
+0034f7d0: 6974 5f61 726d 6174 7572 653a 2027 626c  it_armature: 'bl
+0034f7e0: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+0034f7f0: 2e56 4945 5733 445f 4d54 5f73 656c 6563  .VIEW3D_MT_selec
+0034f800: 745f 6564 6974 5f61 726d 6174 7572 6527  t_edit_armature'
+0034f810: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
+0034f820: 4d54 5f73 656c 6563 745f 6564 6974 5f63  MT_select_edit_c
+0034f830: 7572 7665 3a20 2762 6c5f 7569 2e73 7061  urve: 'bl_ui.spa
+0034f840: 6365 5f76 6965 7733 642e 5649 4557 3344  ce_view3d.VIEW3D
+0034f850: 5f4d 545f 7365 6c65 6374 5f65 6469 745f  _MT_select_edit_
+0034f860: 6375 7276 6527 203d 204e 6f6e 650a 0a56  curve' = None..V
+0034f870: 4945 5733 445f 4d54 5f73 656c 6563 745f  IEW3D_MT_select_
+0034f880: 6564 6974 5f63 7572 7665 733a 2027 626c  edit_curves: 'bl
+0034f890: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+0034f8a0: 2e56 4945 5733 445f 4d54 5f73 656c 6563  .VIEW3D_MT_selec
+0034f8b0: 745f 6564 6974 5f63 7572 7665 7327 203d  t_edit_curves' =
 0034f8c0: 204e 6f6e 650a 0a56 4945 5733 445f 4d54   None..VIEW3D_MT
-0034f8d0: 5f73 656c 6563 745f 6564 6974 5f67 7265  _select_edit_gre
-0034f8e0: 6173 655f 7065 6e63 696c 3a20 2762 6c5f  ase_pencil: 'bl_
-0034f8f0: 7569 2e73 7061 6365 5f76 6965 7733 642e  ui.space_view3d.
-0034f900: 5649 4557 3344 5f4d 545f 7365 6c65 6374  VIEW3D_MT_select
-0034f910: 5f65 6469 745f 6772 6561 7365 5f70 656e  _edit_grease_pen
-0034f920: 6369 6c27 203d 204e 6f6e 650a 0a56 4945  cil' = None..VIE
-0034f930: 5733 445f 4d54 5f73 656c 6563 745f 6564  W3D_MT_select_ed
-0034f940: 6974 5f6c 6174 7469 6365 3a20 2762 6c5f  it_lattice: 'bl_
-0034f950: 7569 2e73 7061 6365 5f76 6965 7733 642e  ui.space_view3d.
-0034f960: 5649 4557 3344 5f4d 545f 7365 6c65 6374  VIEW3D_MT_select
-0034f970: 5f65 6469 745f 6c61 7474 6963 6527 203d  _edit_lattice' =
+0034f8d0: 5f73 656c 6563 745f 6564 6974 5f67 7065  _select_edit_gpe
+0034f8e0: 6e63 696c 3a20 2762 6c5f 7569 2e73 7061  ncil: 'bl_ui.spa
+0034f8f0: 6365 5f76 6965 7733 642e 5649 4557 3344  ce_view3d.VIEW3D
+0034f900: 5f4d 545f 7365 6c65 6374 5f65 6469 745f  _MT_select_edit_
+0034f910: 6770 656e 6369 6c27 203d 204e 6f6e 650a  gpencil' = None.
+0034f920: 0a56 4945 5733 445f 4d54 5f73 656c 6563  .VIEW3D_MT_selec
+0034f930: 745f 6564 6974 5f67 7265 6173 655f 7065  t_edit_grease_pe
+0034f940: 6e63 696c 3a20 2762 6c5f 7569 2e73 7061  ncil: 'bl_ui.spa
+0034f950: 6365 5f76 6965 7733 642e 5649 4557 3344  ce_view3d.VIEW3D
+0034f960: 5f4d 545f 7365 6c65 6374 5f65 6469 745f  _MT_select_edit_
+0034f970: 6772 6561 7365 5f70 656e 6369 6c27 203d  grease_pencil' =
 0034f980: 204e 6f6e 650a 0a56 4945 5733 445f 4d54   None..VIEW3D_MT
-0034f990: 5f73 656c 6563 745f 6564 6974 5f6d 6573  _select_edit_mes
-0034f9a0: 683a 2027 626c 5f75 692e 7370 6163 655f  h: 'bl_ui.space_
-0034f9b0: 7669 6577 3364 2e56 4945 5733 445f 4d54  view3d.VIEW3D_MT
-0034f9c0: 5f73 656c 6563 745f 6564 6974 5f6d 6573  _select_edit_mes
-0034f9d0: 6827 203d 204e 6f6e 650a 0a56 4945 5733  h' = None..VIEW3
-0034f9e0: 445f 4d54 5f73 656c 6563 745f 6564 6974  D_MT_select_edit
-0034f9f0: 5f6d 6574 6162 616c 6c3a 2027 626c 5f75  _metaball: 'bl_u
-0034fa00: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
-0034fa10: 4945 5733 445f 4d54 5f73 656c 6563 745f  IEW3D_MT_select_
-0034fa20: 6564 6974 5f6d 6574 6162 616c 6c27 203d  edit_metaball' =
-0034fa30: 204e 6f6e 650a 0a56 4945 5733 445f 4d54   None..VIEW3D_MT
-0034fa40: 5f73 656c 6563 745f 6564 6974 5f70 6f69  _select_edit_poi
-0034fa50: 6e74 5f63 6c6f 7564 3a20 2762 6c5f 7569  nt_cloud: 'bl_ui
-0034fa60: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
-0034fa70: 4557 3344 5f4d 545f 7365 6c65 6374 5f65  EW3D_MT_select_e
-0034fa80: 6469 745f 706f 696e 745f 636c 6f75 6427  dit_point_cloud'
-0034fa90: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
-0034faa0: 4d54 5f73 656c 6563 745f 6564 6974 5f73  MT_select_edit_s
-0034fab0: 7572 6661 6365 3a20 2762 6c5f 7569 2e73  urface: 'bl_ui.s
-0034fac0: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
-0034fad0: 3344 5f4d 545f 7365 6c65 6374 5f65 6469  3D_MT_select_edi
-0034fae0: 745f 7375 7266 6163 6527 203d 204e 6f6e  t_surface' = Non
+0034f990: 5f73 656c 6563 745f 6564 6974 5f6c 6174  _select_edit_lat
+0034f9a0: 7469 6365 3a20 2762 6c5f 7569 2e73 7061  tice: 'bl_ui.spa
+0034f9b0: 6365 5f76 6965 7733 642e 5649 4557 3344  ce_view3d.VIEW3D
+0034f9c0: 5f4d 545f 7365 6c65 6374 5f65 6469 745f  _MT_select_edit_
+0034f9d0: 6c61 7474 6963 6527 203d 204e 6f6e 650a  lattice' = None.
+0034f9e0: 0a56 4945 5733 445f 4d54 5f73 656c 6563  .VIEW3D_MT_selec
+0034f9f0: 745f 6564 6974 5f6d 6573 683a 2027 626c  t_edit_mesh: 'bl
+0034fa00: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+0034fa10: 2e56 4945 5733 445f 4d54 5f73 656c 6563  .VIEW3D_MT_selec
+0034fa20: 745f 6564 6974 5f6d 6573 6827 203d 204e  t_edit_mesh' = N
+0034fa30: 6f6e 650a 0a56 4945 5733 445f 4d54 5f73  one..VIEW3D_MT_s
+0034fa40: 656c 6563 745f 6564 6974 5f6d 6574 6162  elect_edit_metab
+0034fa50: 616c 6c3a 2027 626c 5f75 692e 7370 6163  all: 'bl_ui.spac
+0034fa60: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
+0034fa70: 4d54 5f73 656c 6563 745f 6564 6974 5f6d  MT_select_edit_m
+0034fa80: 6574 6162 616c 6c27 203d 204e 6f6e 650a  etaball' = None.
+0034fa90: 0a56 4945 5733 445f 4d54 5f73 656c 6563  .VIEW3D_MT_selec
+0034faa0: 745f 6564 6974 5f70 6f69 6e74 5f63 6c6f  t_edit_point_clo
+0034fab0: 7564 3a20 2762 6c5f 7569 2e73 7061 6365  ud: 'bl_ui.space
+0034fac0: 5f76 6965 7733 642e 5649 4557 3344 5f4d  _view3d.VIEW3D_M
+0034fad0: 545f 7365 6c65 6374 5f65 6469 745f 706f  T_select_edit_po
+0034fae0: 696e 745f 636c 6f75 6427 203d 204e 6f6e  int_cloud' = Non
 0034faf0: 650a 0a56 4945 5733 445f 4d54 5f73 656c  e..VIEW3D_MT_sel
-0034fb00: 6563 745f 6564 6974 5f74 6578 743a 2027  ect_edit_text: '
-0034fb10: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
-0034fb20: 3364 2e56 4945 5733 445f 4d54 5f73 656c  3d.VIEW3D_MT_sel
-0034fb30: 6563 745f 6564 6974 5f74 6578 7427 203d  ect_edit_text' =
-0034fb40: 204e 6f6e 650a 0a56 4945 5733 445f 4d54   None..VIEW3D_MT
-0034fb50: 5f73 656c 6563 745f 6f62 6a65 6374 3a20  _select_object: 
-0034fb60: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-0034fb70: 7733 642e 5649 4557 3344 5f4d 545f 7365  w3d.VIEW3D_MT_se
-0034fb80: 6c65 6374 5f6f 626a 6563 7427 203d 204e  lect_object' = N
-0034fb90: 6f6e 650a 0a56 4945 5733 445f 4d54 5f73  one..VIEW3D_MT_s
-0034fba0: 656c 6563 745f 6f62 6a65 6374 5f6d 6f72  elect_object_mor
-0034fbb0: 655f 6c65 7373 3a20 2762 6c5f 7569 2e73  e_less: 'bl_ui.s
-0034fbc0: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
-0034fbd0: 3344 5f4d 545f 7365 6c65 6374 5f6f 626a  3D_MT_select_obj
-0034fbe0: 6563 745f 6d6f 7265 5f6c 6573 7327 203d  ect_more_less' =
-0034fbf0: 204e 6f6e 650a 0a56 4945 5733 445f 4d54   None..VIEW3D_MT
-0034fc00: 5f73 656c 6563 745f 7061 696e 745f 6d61  _select_paint_ma
-0034fc10: 736b 3a20 2762 6c5f 7569 2e73 7061 6365  sk: 'bl_ui.space
-0034fc20: 5f76 6965 7733 642e 5649 4557 3344 5f4d  _view3d.VIEW3D_M
-0034fc30: 545f 7365 6c65 6374 5f70 6169 6e74 5f6d  T_select_paint_m
-0034fc40: 6173 6b27 203d 204e 6f6e 650a 0a56 4945  ask' = None..VIE
-0034fc50: 5733 445f 4d54 5f73 656c 6563 745f 7061  W3D_MT_select_pa
-0034fc60: 696e 745f 6d61 736b 5f76 6572 7465 783a  int_mask_vertex:
-0034fc70: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-0034fc80: 6577 3364 2e56 4945 5733 445f 4d54 5f73  ew3d.VIEW3D_MT_s
-0034fc90: 656c 6563 745f 7061 696e 745f 6d61 736b  elect_paint_mask
-0034fca0: 5f76 6572 7465 7827 203d 204e 6f6e 650a  _vertex' = None.
-0034fcb0: 0a56 4945 5733 445f 4d54 5f73 656c 6563  .VIEW3D_MT_selec
-0034fcc0: 745f 7061 7274 6963 6c65 3a20 2762 6c5f  t_particle: 'bl_
-0034fcd0: 7569 2e73 7061 6365 5f76 6965 7733 642e  ui.space_view3d.
-0034fce0: 5649 4557 3344 5f4d 545f 7365 6c65 6374  VIEW3D_MT_select
-0034fcf0: 5f70 6172 7469 636c 6527 203d 204e 6f6e  _particle' = Non
-0034fd00: 650a 0a56 4945 5733 445f 4d54 5f73 656c  e..VIEW3D_MT_sel
-0034fd10: 6563 745f 706f 7365 3a20 2762 6c5f 7569  ect_pose: 'bl_ui
-0034fd20: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
-0034fd30: 4557 3344 5f4d 545f 7365 6c65 6374 5f70  EW3D_MT_select_p
-0034fd40: 6f73 6527 203d 204e 6f6e 650a 0a56 4945  ose' = None..VIE
-0034fd50: 5733 445f 4d54 5f73 656c 6563 745f 706f  W3D_MT_select_po
-0034fd60: 7365 5f6d 6f72 655f 6c65 7373 3a20 2762  se_more_less: 'b
-0034fd70: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-0034fd80: 642e 5649 4557 3344 5f4d 545f 7365 6c65  d.VIEW3D_MT_sele
-0034fd90: 6374 5f70 6f73 655f 6d6f 7265 5f6c 6573  ct_pose_more_les
-0034fda0: 7327 203d 204e 6f6e 650a 0a56 4945 5733  s' = None..VIEW3
-0034fdb0: 445f 4d54 5f73 656c 6563 745f 7363 756c  D_MT_select_scul
-0034fdc0: 7074 5f63 7572 7665 733a 2027 626c 5f75  pt_curves: 'bl_u
-0034fdd0: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
-0034fde0: 4945 5733 445f 4d54 5f73 656c 6563 745f  IEW3D_MT_select_
-0034fdf0: 7363 756c 7074 5f63 7572 7665 7327 203d  sculpt_curves' =
-0034fe00: 204e 6f6e 650a 0a56 4945 5733 445f 4d54   None..VIEW3D_MT
-0034fe10: 5f73 6861 6469 6e67 5f65 785f 7069 653a  _shading_ex_pie:
-0034fe20: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-0034fe30: 6577 3364 2e56 4945 5733 445f 4d54 5f73  ew3d.VIEW3D_MT_s
-0034fe40: 6861 6469 6e67 5f65 785f 7069 6527 203d  hading_ex_pie' =
-0034fe50: 204e 6f6e 650a 0a56 4945 5733 445f 4d54   None..VIEW3D_MT
-0034fe60: 5f73 6861 6469 6e67 5f70 6965 3a20 2762  _shading_pie: 'b
-0034fe70: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-0034fe80: 642e 5649 4557 3344 5f4d 545f 7368 6164  d.VIEW3D_MT_shad
-0034fe90: 696e 675f 7069 6527 203d 204e 6f6e 650a  ing_pie' = None.
-0034fea0: 0a56 4945 5733 445f 4d54 5f73 6e61 703a  .VIEW3D_MT_snap:
-0034feb0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-0034fec0: 6577 3364 2e56 4945 5733 445f 4d54 5f73  ew3d.VIEW3D_MT_s
-0034fed0: 6e61 7027 203d 204e 6f6e 650a 0a56 4945  nap' = None..VIE
-0034fee0: 5733 445f 4d54 5f73 6e61 705f 7069 653a  W3D_MT_snap_pie:
-0034fef0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-0034ff00: 6577 3364 2e56 4945 5733 445f 4d54 5f73  ew3d.VIEW3D_MT_s
-0034ff10: 6e61 705f 7069 6527 203d 204e 6f6e 650a  nap_pie' = None.
-0034ff20: 0a56 4945 5733 445f 4d54 5f73 7572 6661  .VIEW3D_MT_surfa
-0034ff30: 6365 5f61 6464 3a20 2762 6c5f 7569 2e73  ce_add: 'bl_ui.s
-0034ff40: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
-0034ff50: 3344 5f4d 545f 7375 7266 6163 655f 6164  3D_MT_surface_ad
-0034ff60: 6427 203d 204e 6f6e 650a 0a56 4945 5733  d' = None..VIEW3
-0034ff70: 445f 4d54 5f74 6f6f 6c73 5f70 726f 6a65  D_MT_tools_proje
-0034ff80: 6374 7061 696e 745f 636c 6f6e 653a 2027  ctpaint_clone: '
-0034ff90: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-0034ffa0: 5f70 6169 6e74 5f63 6f6d 6d6f 6e2e 5649  _paint_common.VI
-0034ffb0: 4557 3344 5f4d 545f 746f 6f6c 735f 7072  EW3D_MT_tools_pr
-0034ffc0: 6f6a 6563 7470 6169 6e74 5f63 6c6f 6e65  ojectpaint_clone
-0034ffd0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-0034ffe0: 5f4d 545f 746f 6f6c 735f 7072 6f6a 6563  _MT_tools_projec
-0034fff0: 7470 6169 6e74 5f73 7465 6e63 696c 3a20  tpaint_stencil: 
-00350000: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-00350010: 7733 645f 746f 6f6c 6261 722e 5649 4557  w3d_toolbar.VIEW
-00350020: 3344 5f4d 545f 746f 6f6c 735f 7072 6f6a  3D_MT_tools_proj
-00350030: 6563 7470 6169 6e74 5f73 7465 6e63 696c  ectpaint_stencil
-00350040: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-00350050: 5f4d 545f 746f 6f6c 735f 7072 6f6a 6563  _MT_tools_projec
-00350060: 7470 6169 6e74 5f75 766c 6179 6572 3a20  tpaint_uvlayer: 
-00350070: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-00350080: 7733 645f 746f 6f6c 6261 722e 5649 4557  w3d_toolbar.VIEW
-00350090: 3344 5f4d 545f 746f 6f6c 735f 7072 6f6a  3D_MT_tools_proj
-003500a0: 6563 7470 6169 6e74 5f75 766c 6179 6572  ectpaint_uvlayer
-003500b0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-003500c0: 5f4d 545f 7472 616e 7366 6f72 6d3a 2027  _MT_transform: '
-003500d0: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
-003500e0: 3364 2e56 4945 5733 445f 4d54 5f74 7261  3d.VIEW3D_MT_tra
-003500f0: 6e73 666f 726d 2720 3d20 4e6f 6e65 0a0a  nsform' = None..
-00350100: 5649 4557 3344 5f4d 545f 7472 616e 7366  VIEW3D_MT_transf
-00350110: 6f72 6d5f 6172 6d61 7475 7265 3a20 2762  orm_armature: 'b
-00350120: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-00350130: 642e 5649 4557 3344 5f4d 545f 7472 616e  d.VIEW3D_MT_tran
-00350140: 7366 6f72 6d5f 6172 6d61 7475 7265 2720  sform_armature' 
-00350150: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f4d  = None..VIEW3D_M
-00350160: 545f 7472 616e 7366 6f72 6d5f 6769 7a6d  T_transform_gizm
-00350170: 6f5f 7069 653a 2027 626c 5f75 692e 7370  o_pie: 'bl_ui.sp
-00350180: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
-00350190: 445f 4d54 5f74 7261 6e73 666f 726d 5f67  D_MT_transform_g
-003501a0: 697a 6d6f 5f70 6965 2720 3d20 4e6f 6e65  izmo_pie' = None
+0034fb00: 6563 745f 6564 6974 5f73 7572 6661 6365  ect_edit_surface
+0034fb10: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+0034fb20: 6965 7733 642e 5649 4557 3344 5f4d 545f  iew3d.VIEW3D_MT_
+0034fb30: 7365 6c65 6374 5f65 6469 745f 7375 7266  select_edit_surf
+0034fb40: 6163 6527 203d 204e 6f6e 650a 0a56 4945  ace' = None..VIE
+0034fb50: 5733 445f 4d54 5f73 656c 6563 745f 6564  W3D_MT_select_ed
+0034fb60: 6974 5f74 6578 743a 2027 626c 5f75 692e  it_text: 'bl_ui.
+0034fb70: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
+0034fb80: 5733 445f 4d54 5f73 656c 6563 745f 6564  W3D_MT_select_ed
+0034fb90: 6974 5f74 6578 7427 203d 204e 6f6e 650a  it_text' = None.
+0034fba0: 0a56 4945 5733 445f 4d54 5f73 656c 6563  .VIEW3D_MT_selec
+0034fbb0: 745f 6f62 6a65 6374 3a20 2762 6c5f 7569  t_object: 'bl_ui
+0034fbc0: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
+0034fbd0: 4557 3344 5f4d 545f 7365 6c65 6374 5f6f  EW3D_MT_select_o
+0034fbe0: 626a 6563 7427 203d 204e 6f6e 650a 0a56  bject' = None..V
+0034fbf0: 4945 5733 445f 4d54 5f73 656c 6563 745f  IEW3D_MT_select_
+0034fc00: 6f62 6a65 6374 5f6d 6f72 655f 6c65 7373  object_more_less
+0034fc10: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+0034fc20: 6965 7733 642e 5649 4557 3344 5f4d 545f  iew3d.VIEW3D_MT_
+0034fc30: 7365 6c65 6374 5f6f 626a 6563 745f 6d6f  select_object_mo
+0034fc40: 7265 5f6c 6573 7327 203d 204e 6f6e 650a  re_less' = None.
+0034fc50: 0a56 4945 5733 445f 4d54 5f73 656c 6563  .VIEW3D_MT_selec
+0034fc60: 745f 7061 696e 745f 6d61 736b 3a20 2762  t_paint_mask: 'b
+0034fc70: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+0034fc80: 642e 5649 4557 3344 5f4d 545f 7365 6c65  d.VIEW3D_MT_sele
+0034fc90: 6374 5f70 6169 6e74 5f6d 6173 6b27 203d  ct_paint_mask' =
+0034fca0: 204e 6f6e 650a 0a56 4945 5733 445f 4d54   None..VIEW3D_MT
+0034fcb0: 5f73 656c 6563 745f 7061 696e 745f 6d61  _select_paint_ma
+0034fcc0: 736b 5f76 6572 7465 783a 2027 626c 5f75  sk_vertex: 'bl_u
+0034fcd0: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
+0034fce0: 4945 5733 445f 4d54 5f73 656c 6563 745f  IEW3D_MT_select_
+0034fcf0: 7061 696e 745f 6d61 736b 5f76 6572 7465  paint_mask_verte
+0034fd00: 7827 203d 204e 6f6e 650a 0a56 4945 5733  x' = None..VIEW3
+0034fd10: 445f 4d54 5f73 656c 6563 745f 7061 7274  D_MT_select_part
+0034fd20: 6963 6c65 3a20 2762 6c5f 7569 2e73 7061  icle: 'bl_ui.spa
+0034fd30: 6365 5f76 6965 7733 642e 5649 4557 3344  ce_view3d.VIEW3D
+0034fd40: 5f4d 545f 7365 6c65 6374 5f70 6172 7469  _MT_select_parti
+0034fd50: 636c 6527 203d 204e 6f6e 650a 0a56 4945  cle' = None..VIE
+0034fd60: 5733 445f 4d54 5f73 656c 6563 745f 706f  W3D_MT_select_po
+0034fd70: 7365 3a20 2762 6c5f 7569 2e73 7061 6365  se: 'bl_ui.space
+0034fd80: 5f76 6965 7733 642e 5649 4557 3344 5f4d  _view3d.VIEW3D_M
+0034fd90: 545f 7365 6c65 6374 5f70 6f73 6527 203d  T_select_pose' =
+0034fda0: 204e 6f6e 650a 0a56 4945 5733 445f 4d54   None..VIEW3D_MT
+0034fdb0: 5f73 656c 6563 745f 706f 7365 5f6d 6f72  _select_pose_mor
+0034fdc0: 655f 6c65 7373 3a20 2762 6c5f 7569 2e73  e_less: 'bl_ui.s
+0034fdd0: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
+0034fde0: 3344 5f4d 545f 7365 6c65 6374 5f70 6f73  3D_MT_select_pos
+0034fdf0: 655f 6d6f 7265 5f6c 6573 7327 203d 204e  e_more_less' = N
+0034fe00: 6f6e 650a 0a56 4945 5733 445f 4d54 5f73  one..VIEW3D_MT_s
+0034fe10: 656c 6563 745f 7363 756c 7074 5f63 7572  elect_sculpt_cur
+0034fe20: 7665 733a 2027 626c 5f75 692e 7370 6163  ves: 'bl_ui.spac
+0034fe30: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
+0034fe40: 4d54 5f73 656c 6563 745f 7363 756c 7074  MT_select_sculpt
+0034fe50: 5f63 7572 7665 7327 203d 204e 6f6e 650a  _curves' = None.
+0034fe60: 0a56 4945 5733 445f 4d54 5f73 6861 6469  .VIEW3D_MT_shadi
+0034fe70: 6e67 5f65 785f 7069 653a 2027 626c 5f75  ng_ex_pie: 'bl_u
+0034fe80: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
+0034fe90: 4945 5733 445f 4d54 5f73 6861 6469 6e67  IEW3D_MT_shading
+0034fea0: 5f65 785f 7069 6527 203d 204e 6f6e 650a  _ex_pie' = None.
+0034feb0: 0a56 4945 5733 445f 4d54 5f73 6861 6469  .VIEW3D_MT_shadi
+0034fec0: 6e67 5f70 6965 3a20 2762 6c5f 7569 2e73  ng_pie: 'bl_ui.s
+0034fed0: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
+0034fee0: 3344 5f4d 545f 7368 6164 696e 675f 7069  3D_MT_shading_pi
+0034fef0: 6527 203d 204e 6f6e 650a 0a56 4945 5733  e' = None..VIEW3
+0034ff00: 445f 4d54 5f73 6e61 703a 2027 626c 5f75  D_MT_snap: 'bl_u
+0034ff10: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
+0034ff20: 4945 5733 445f 4d54 5f73 6e61 7027 203d  IEW3D_MT_snap' =
+0034ff30: 204e 6f6e 650a 0a56 4945 5733 445f 4d54   None..VIEW3D_MT
+0034ff40: 5f73 6e61 705f 7069 653a 2027 626c 5f75  _snap_pie: 'bl_u
+0034ff50: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
+0034ff60: 4945 5733 445f 4d54 5f73 6e61 705f 7069  IEW3D_MT_snap_pi
+0034ff70: 6527 203d 204e 6f6e 650a 0a56 4945 5733  e' = None..VIEW3
+0034ff80: 445f 4d54 5f73 7572 6661 6365 5f61 6464  D_MT_surface_add
+0034ff90: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+0034ffa0: 6965 7733 642e 5649 4557 3344 5f4d 545f  iew3d.VIEW3D_MT_
+0034ffb0: 7375 7266 6163 655f 6164 6427 203d 204e  surface_add' = N
+0034ffc0: 6f6e 650a 0a56 4945 5733 445f 4d54 5f74  one..VIEW3D_MT_t
+0034ffd0: 6f6f 6c73 5f70 726f 6a65 6374 7061 696e  ools_projectpain
+0034ffe0: 745f 636c 6f6e 653a 2027 626c 5f75 692e  t_clone: 'bl_ui.
+0034fff0: 7072 6f70 6572 7469 6573 5f70 6169 6e74  properties_paint
+00350000: 5f63 6f6d 6d6f 6e2e 5649 4557 3344 5f4d  _common.VIEW3D_M
+00350010: 545f 746f 6f6c 735f 7072 6f6a 6563 7470  T_tools_projectp
+00350020: 6169 6e74 5f63 6c6f 6e65 2720 3d20 4e6f  aint_clone' = No
+00350030: 6e65 0a0a 5649 4557 3344 5f4d 545f 746f  ne..VIEW3D_MT_to
+00350040: 6f6c 735f 7072 6f6a 6563 7470 6169 6e74  ols_projectpaint
+00350050: 5f73 7465 6e63 696c 3a20 2762 6c5f 7569  _stencil: 'bl_ui
+00350060: 2e73 7061 6365 5f76 6965 7733 645f 746f  .space_view3d_to
+00350070: 6f6c 6261 722e 5649 4557 3344 5f4d 545f  olbar.VIEW3D_MT_
+00350080: 746f 6f6c 735f 7072 6f6a 6563 7470 6169  tools_projectpai
+00350090: 6e74 5f73 7465 6e63 696c 2720 3d20 4e6f  nt_stencil' = No
+003500a0: 6e65 0a0a 5649 4557 3344 5f4d 545f 746f  ne..VIEW3D_MT_to
+003500b0: 6f6c 735f 7072 6f6a 6563 7470 6169 6e74  ols_projectpaint
+003500c0: 5f75 766c 6179 6572 3a20 2762 6c5f 7569  _uvlayer: 'bl_ui
+003500d0: 2e73 7061 6365 5f76 6965 7733 645f 746f  .space_view3d_to
+003500e0: 6f6c 6261 722e 5649 4557 3344 5f4d 545f  olbar.VIEW3D_MT_
+003500f0: 746f 6f6c 735f 7072 6f6a 6563 7470 6169  tools_projectpai
+00350100: 6e74 5f75 766c 6179 6572 2720 3d20 4e6f  nt_uvlayer' = No
+00350110: 6e65 0a0a 5649 4557 3344 5f4d 545f 7472  ne..VIEW3D_MT_tr
+00350120: 616e 7366 6f72 6d3a 2027 626c 5f75 692e  ansform: 'bl_ui.
+00350130: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
+00350140: 5733 445f 4d54 5f74 7261 6e73 666f 726d  W3D_MT_transform
+00350150: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+00350160: 5f4d 545f 7472 616e 7366 6f72 6d5f 6172  _MT_transform_ar
+00350170: 6d61 7475 7265 3a20 2762 6c5f 7569 2e73  mature: 'bl_ui.s
+00350180: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
+00350190: 3344 5f4d 545f 7472 616e 7366 6f72 6d5f  3D_MT_transform_
+003501a0: 6172 6d61 7475 7265 2720 3d20 4e6f 6e65  armature' = None
 003501b0: 0a0a 5649 4557 3344 5f4d 545f 7472 616e  ..VIEW3D_MT_tran
-003501c0: 7366 6f72 6d5f 6f62 6a65 6374 3a20 2762  sform_object: 'b
-003501d0: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-003501e0: 642e 5649 4557 3344 5f4d 545f 7472 616e  d.VIEW3D_MT_tran
-003501f0: 7366 6f72 6d5f 6f62 6a65 6374 2720 3d20  sform_object' = 
-00350200: 4e6f 6e65 0a0a 5649 4557 3344 5f4d 545f  None..VIEW3D_MT_
-00350210: 7576 5f6d 6170 3a20 2762 6c5f 7569 2e73  uv_map: 'bl_ui.s
-00350220: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
-00350230: 3344 5f4d 545f 7576 5f6d 6170 2720 3d20  3D_MT_uv_map' = 
-00350240: 4e6f 6e65 0a0a 5649 4557 3344 5f4d 545f  None..VIEW3D_MT_
-00350250: 7665 7274 6578 5f67 726f 7570 3a20 2762  vertex_group: 'b
-00350260: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-00350270: 642e 5649 4557 3344 5f4d 545f 7665 7274  d.VIEW3D_MT_vert
-00350280: 6578 5f67 726f 7570 2720 3d20 4e6f 6e65  ex_group' = None
-00350290: 0a0a 5649 4557 3344 5f4d 545f 7669 6577  ..VIEW3D_MT_view
-003502a0: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
-003502b0: 6965 7733 642e 5649 4557 3344 5f4d 545f  iew3d.VIEW3D_MT_
-003502c0: 7669 6577 2720 3d20 4e6f 6e65 0a0a 5649  view' = None..VI
-003502d0: 4557 3344 5f4d 545f 7669 6577 5f61 6c69  EW3D_MT_view_ali
-003502e0: 676e 3a20 2762 6c5f 7569 2e73 7061 6365  gn: 'bl_ui.space
-003502f0: 5f76 6965 7733 642e 5649 4557 3344 5f4d  _view3d.VIEW3D_M
-00350300: 545f 7669 6577 5f61 6c69 676e 2720 3d20  T_view_align' = 
-00350310: 4e6f 6e65 0a0a 5649 4557 3344 5f4d 545f  None..VIEW3D_MT_
-00350320: 7669 6577 5f61 6c69 676e 5f73 656c 6563  view_align_selec
-00350330: 7465 643a 2027 626c 5f75 692e 7370 6163  ted: 'bl_ui.spac
-00350340: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
-00350350: 4d54 5f76 6965 775f 616c 6967 6e5f 7365  MT_view_align_se
-00350360: 6c65 6374 6564 2720 3d20 4e6f 6e65 0a0a  lected' = None..
-00350370: 5649 4557 3344 5f4d 545f 7669 6577 5f63  VIEW3D_MT_view_c
-00350380: 616d 6572 6173 3a20 2762 6c5f 7569 2e73  ameras: 'bl_ui.s
-00350390: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
-003503a0: 3344 5f4d 545f 7669 6577 5f63 616d 6572  3D_MT_view_camer
-003503b0: 6173 2720 3d20 4e6f 6e65 0a0a 5649 4557  as' = None..VIEW
-003503c0: 3344 5f4d 545f 7669 6577 5f6c 6f63 616c  3D_MT_view_local
-003503d0: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
-003503e0: 6965 7733 642e 5649 4557 3344 5f4d 545f  iew3d.VIEW3D_MT_
-003503f0: 7669 6577 5f6c 6f63 616c 2720 3d20 4e6f  view_local' = No
-00350400: 6e65 0a0a 5649 4557 3344 5f4d 545f 7669  ne..VIEW3D_MT_vi
-00350410: 6577 5f6e 6176 6967 6174 696f 6e3a 2027  ew_navigation: '
-00350420: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
-00350430: 3364 2e56 4945 5733 445f 4d54 5f76 6965  3d.VIEW3D_MT_vie
-00350440: 775f 6e61 7669 6761 7469 6f6e 2720 3d20  w_navigation' = 
-00350450: 4e6f 6e65 0a0a 5649 4557 3344 5f4d 545f  None..VIEW3D_MT_
-00350460: 7669 6577 5f70 6965 3a20 2762 6c5f 7569  view_pie: 'bl_ui
-00350470: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
-00350480: 4557 3344 5f4d 545f 7669 6577 5f70 6965  EW3D_MT_view_pie
-00350490: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-003504a0: 5f4d 545f 7669 6577 5f72 6567 696f 6e73  _MT_view_regions
-003504b0: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
-003504c0: 6965 7733 642e 5649 4557 3344 5f4d 545f  iew3d.VIEW3D_MT_
-003504d0: 7669 6577 5f72 6567 696f 6e73 2720 3d20  view_regions' = 
-003504e0: 4e6f 6e65 0a0a 5649 4557 3344 5f4d 545f  None..VIEW3D_MT_
-003504f0: 7669 6577 5f76 6965 7770 6f69 6e74 3a20  view_viewpoint: 
-00350500: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-00350510: 7733 642e 5649 4557 3344 5f4d 545f 7669  w3d.VIEW3D_MT_vi
-00350520: 6577 5f76 6965 7770 6f69 6e74 2720 3d20  ew_viewpoint' = 
-00350530: 4e6f 6e65 0a0a 5649 4557 3344 5f4d 545f  None..VIEW3D_MT_
-00350540: 766f 6c75 6d65 5f61 6464 3a20 2762 6c5f  volume_add: 'bl_
-00350550: 7569 2e73 7061 6365 5f76 6965 7733 642e  ui.space_view3d.
-00350560: 5649 4557 3344 5f4d 545f 766f 6c75 6d65  VIEW3D_MT_volume
-00350570: 5f61 6464 2720 3d20 4e6f 6e65 0a0a 5649  _add' = None..VI
-00350580: 4557 3344 5f4d 545f 7765 6967 6874 5f67  EW3D_MT_weight_g
-00350590: 7065 6e63 696c 3a20 2762 6c5f 7569 2e73  pencil: 'bl_ui.s
-003505a0: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
-003505b0: 3344 5f4d 545f 7765 6967 6874 5f67 7065  3D_MT_weight_gpe
-003505c0: 6e63 696c 2720 3d20 4e6f 6e65 0a0a 5649  ncil' = None..VI
-003505d0: 4557 3344 5f4d 545f 7770 6169 6e74 5f76  EW3D_MT_wpaint_v
-003505e0: 6772 6f75 705f 6c6f 636b 5f70 6965 3a20  group_lock_pie: 
-003505f0: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-00350600: 7733 642e 5649 4557 3344 5f4d 545f 7770  w3d.VIEW3D_MT_wp
-00350610: 6169 6e74 5f76 6772 6f75 705f 6c6f 636b  aint_vgroup_lock
-00350620: 5f70 6965 2720 3d20 4e6f 6e65 0a0a 5649  _pie' = None..VI
-00350630: 4557 3344 5f4f 545f 6564 6974 5f6d 6573  EW3D_OT_edit_mes
-00350640: 685f 6578 7472 7564 655f 696e 6469 7669  h_extrude_indivi
-00350650: 6475 616c 5f6d 6f76 653a 2027 626c 5f6f  dual_move: 'bl_o
-00350660: 7065 7261 746f 7273 2e76 6965 7733 642e  perators.view3d.
-00350670: 5649 4557 3344 5f4f 545f 6564 6974 5f6d  VIEW3D_OT_edit_m
-00350680: 6573 685f 6578 7472 7564 655f 696e 6469  esh_extrude_indi
-00350690: 7669 6475 616c 5f6d 6f76 6527 203d 204e  vidual_move' = N
-003506a0: 6f6e 650a 0a56 4945 5733 445f 4f54 5f65  one..VIEW3D_OT_e
-003506b0: 6469 745f 6d65 7368 5f65 7874 7275 6465  dit_mesh_extrude
-003506c0: 5f6d 616e 6966 6f6c 645f 6e6f 726d 616c  _manifold_normal
-003506d0: 3a20 2762 6c5f 6f70 6572 6174 6f72 732e  : 'bl_operators.
-003506e0: 7669 6577 3364 2e56 4945 5733 445f 4f54  view3d.VIEW3D_OT
-003506f0: 5f65 6469 745f 6d65 7368 5f65 7874 7275  _edit_mesh_extru
-00350700: 6465 5f6d 616e 6966 6f6c 645f 6e6f 726d  de_manifold_norm
-00350710: 616c 2720 3d20 4e6f 6e65 0a0a 5649 4557  al' = None..VIEW
-00350720: 3344 5f4f 545f 7472 616e 7366 6f72 6d5f  3D_OT_transform_
-00350730: 6769 7a6d 6f5f 7365 743a 2027 626c 5f6f  gizmo_set: 'bl_o
-00350740: 7065 7261 746f 7273 2e76 6965 7733 642e  perators.view3d.
-00350750: 5649 4557 3344 5f4f 545f 7472 616e 7366  VIEW3D_OT_transf
-00350760: 6f72 6d5f 6769 7a6d 6f5f 7365 7427 203d  orm_gizmo_set' =
-00350770: 204e 6f6e 650a 0a56 4945 5733 445f 5054   None..VIEW3D_PT
-00350780: 5f61 6374 6976 655f 746f 6f6c 3a20 2762  _active_tool: 'b
-00350790: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-003507a0: 642e 5649 4557 3344 5f50 545f 6163 7469  d.VIEW3D_PT_acti
-003507b0: 7665 5f74 6f6f 6c27 203d 204e 6f6e 650a  ve_tool' = None.
-003507c0: 0a56 4945 5733 445f 5054 5f61 6374 6976  .VIEW3D_PT_activ
-003507d0: 655f 746f 6f6c 5f64 7570 6c69 6361 7465  e_tool_duplicate
-003507e0: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
-003507f0: 6965 7733 642e 5649 4557 3344 5f50 545f  iew3d.VIEW3D_PT_
-00350800: 6163 7469 7665 5f74 6f6f 6c5f 6475 706c  active_tool_dupl
-00350810: 6963 6174 6527 203d 204e 6f6e 650a 0a56  icate' = None..V
-00350820: 4945 5733 445f 5054 5f61 6e6e 6f74 6174  IEW3D_PT_annotat
-00350830: 696f 6e5f 6f6e 696f 6e3a 2027 626c 5f75  ion_onion: 'bl_u
-00350840: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
-00350850: 4945 5733 445f 5054 5f61 6e6e 6f74 6174  IEW3D_PT_annotat
-00350860: 696f 6e5f 6f6e 696f 6e27 203d 204e 6f6e  ion_onion' = Non
-00350870: 650a 0a56 4945 5733 445f 5054 5f63 6f6c  e..VIEW3D_PT_col
-00350880: 6c65 6374 696f 6e73 3a20 2762 6c5f 7569  lections: 'bl_ui
-00350890: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
-003508a0: 4557 3344 5f50 545f 636f 6c6c 6563 7469  EW3D_PT_collecti
-003508b0: 6f6e 7327 203d 204e 6f6e 650a 0a56 4945  ons' = None..VIE
-003508c0: 5733 445f 5054 5f63 6f6e 7465 7874 5f70  W3D_PT_context_p
-003508d0: 726f 7065 7274 6965 733a 2027 626c 5f75  roperties: 'bl_u
-003508e0: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
-003508f0: 4945 5733 445f 5054 5f63 6f6e 7465 7874  IEW3D_PT_context
-00350900: 5f70 726f 7065 7274 6965 7327 203d 204e  _properties' = N
-00350910: 6f6e 650a 0a56 4945 5733 445f 5054 5f63  one..VIEW3D_PT_c
-00350920: 7572 7665 735f 7363 756c 7074 5f61 6464  urves_sculpt_add
-00350930: 5f73 6861 7065 3a20 2762 6c5f 7569 2e73  _shape: 'bl_ui.s
-00350940: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
-00350950: 3344 5f50 545f 6375 7276 6573 5f73 6375  3D_PT_curves_scu
-00350960: 6c70 745f 6164 645f 7368 6170 6527 203d  lpt_add_shape' =
-00350970: 204e 6f6e 650a 0a56 4945 5733 445f 5054   None..VIEW3D_PT
-00350980: 5f63 7572 7665 735f 7363 756c 7074 5f67  _curves_sculpt_g
-00350990: 726f 775f 7368 7269 6e6b 5f73 6361 6c69  row_shrink_scali
-003509a0: 6e67 3a20 2762 6c5f 7569 2e73 7061 6365  ng: 'bl_ui.space
-003509b0: 5f76 6965 7733 642e 5649 4557 3344 5f50  _view3d.VIEW3D_P
-003509c0: 545f 6375 7276 6573 5f73 6375 6c70 745f  T_curves_sculpt_
-003509d0: 6772 6f77 5f73 6872 696e 6b5f 7363 616c  grow_shrink_scal
-003509e0: 696e 6727 203d 204e 6f6e 650a 0a56 4945  ing' = None..VIE
-003509f0: 5733 445f 5054 5f63 7572 7665 735f 7363  W3D_PT_curves_sc
-00350a00: 756c 7074 5f70 6172 616d 6574 6572 5f66  ulpt_parameter_f
-00350a10: 616c 6c6f 6666 3a20 2762 6c5f 7569 2e73  alloff: 'bl_ui.s
-00350a20: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
-00350a30: 3344 5f50 545f 6375 7276 6573 5f73 6375  3D_PT_curves_scu
-00350a40: 6c70 745f 7061 7261 6d65 7465 725f 6661  lpt_parameter_fa
-00350a50: 6c6c 6f66 6627 203d 204e 6f6e 650a 0a56  lloff' = None..V
-00350a60: 4945 5733 445f 5054 5f63 7572 7665 735f  IEW3D_PT_curves_
-00350a70: 7363 756c 7074 5f73 796d 6d65 7472 793a  sculpt_symmetry:
-00350a80: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-00350a90: 6577 3364 5f74 6f6f 6c62 6172 2e56 4945  ew3d_toolbar.VIE
-00350aa0: 5733 445f 5054 5f63 7572 7665 735f 7363  W3D_PT_curves_sc
-00350ab0: 756c 7074 5f73 796d 6d65 7472 7927 203d  ulpt_symmetry' =
-00350ac0: 204e 6f6e 650a 0a56 4945 5733 445f 5054   None..VIEW3D_PT
-00350ad0: 5f63 7572 7665 735f 7363 756c 7074 5f73  _curves_sculpt_s
-00350ae0: 796d 6d65 7472 795f 666f 725f 746f 7062  ymmetry_for_topb
-00350af0: 6172 3a20 2762 6c5f 7569 2e73 7061 6365  ar: 'bl_ui.space
-00350b00: 5f76 6965 7733 645f 746f 6f6c 6261 722e  _view3d_toolbar.
-00350b10: 5649 4557 3344 5f50 545f 6375 7276 6573  VIEW3D_PT_curves
-00350b20: 5f73 6375 6c70 745f 7379 6d6d 6574 7279  _sculpt_symmetry
-00350b30: 5f66 6f72 5f74 6f70 6261 7227 203d 204e  _for_topbar' = N
-00350b40: 6f6e 650a 0a56 4945 5733 445f 5054 5f67  one..VIEW3D_PT_g
-00350b50: 697a 6d6f 5f64 6973 706c 6179 3a20 2762  izmo_display: 'b
-00350b60: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-00350b70: 642e 5649 4557 3344 5f50 545f 6769 7a6d  d.VIEW3D_PT_gizm
-00350b80: 6f5f 6469 7370 6c61 7927 203d 204e 6f6e  o_display' = Non
-00350b90: 650a 0a56 4945 5733 445f 5054 5f67 7065  e..VIEW3D_PT_gpe
-00350ba0: 6e63 696c 5f62 7275 7368 5f70 7265 7365  ncil_brush_prese
-00350bb0: 7473 3a20 2762 6c5f 7569 2e73 7061 6365  ts: 'bl_ui.space
-00350bc0: 5f76 6965 7733 645f 746f 6f6c 6261 722e  _view3d_toolbar.
-00350bd0: 5649 4557 3344 5f50 545f 6770 656e 6369  VIEW3D_PT_gpenci
-00350be0: 6c5f 6272 7573 685f 7072 6573 6574 7327  l_brush_presets'
-00350bf0: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
-00350c00: 5054 5f67 7065 6e63 696c 5f63 7572 7665  PT_gpencil_curve
-00350c10: 5f65 6469 743a 2027 626c 5f75 692e 7370  _edit: 'bl_ui.sp
-00350c20: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
-00350c30: 445f 5054 5f67 7065 6e63 696c 5f63 7572  D_PT_gpencil_cur
-00350c40: 7665 5f65 6469 7427 203d 204e 6f6e 650a  ve_edit' = None.
-00350c50: 0a56 4945 5733 445f 5054 5f67 7065 6e63  .VIEW3D_PT_gpenc
-00350c60: 696c 5f64 7261 775f 636f 6e74 6578 745f  il_draw_context_
-00350c70: 6d65 6e75 3a20 2762 6c5f 7569 2e73 7061  menu: 'bl_ui.spa
-00350c80: 6365 5f76 6965 7733 642e 5649 4557 3344  ce_view3d.VIEW3D
-00350c90: 5f50 545f 6770 656e 6369 6c5f 6472 6177  _PT_gpencil_draw
-00350ca0: 5f63 6f6e 7465 7874 5f6d 656e 7527 203d  _context_menu' =
-00350cb0: 204e 6f6e 650a 0a56 4945 5733 445f 5054   None..VIEW3D_PT
-00350cc0: 5f67 7065 6e63 696c 5f67 7569 6465 3a20  _gpencil_guide: 
+003501c0: 7366 6f72 6d5f 6769 7a6d 6f5f 7069 653a  sform_gizmo_pie:
+003501d0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+003501e0: 6577 3364 2e56 4945 5733 445f 4d54 5f74  ew3d.VIEW3D_MT_t
+003501f0: 7261 6e73 666f 726d 5f67 697a 6d6f 5f70  ransform_gizmo_p
+00350200: 6965 2720 3d20 4e6f 6e65 0a0a 5649 4557  ie' = None..VIEW
+00350210: 3344 5f4d 545f 7472 616e 7366 6f72 6d5f  3D_MT_transform_
+00350220: 6f62 6a65 6374 3a20 2762 6c5f 7569 2e73  object: 'bl_ui.s
+00350230: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
+00350240: 3344 5f4d 545f 7472 616e 7366 6f72 6d5f  3D_MT_transform_
+00350250: 6f62 6a65 6374 2720 3d20 4e6f 6e65 0a0a  object' = None..
+00350260: 5649 4557 3344 5f4d 545f 7576 5f6d 6170  VIEW3D_MT_uv_map
+00350270: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+00350280: 6965 7733 642e 5649 4557 3344 5f4d 545f  iew3d.VIEW3D_MT_
+00350290: 7576 5f6d 6170 2720 3d20 4e6f 6e65 0a0a  uv_map' = None..
+003502a0: 5649 4557 3344 5f4d 545f 7665 7274 6578  VIEW3D_MT_vertex
+003502b0: 5f67 726f 7570 3a20 2762 6c5f 7569 2e73  _group: 'bl_ui.s
+003502c0: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
+003502d0: 3344 5f4d 545f 7665 7274 6578 5f67 726f  3D_MT_vertex_gro
+003502e0: 7570 2720 3d20 4e6f 6e65 0a0a 5649 4557  up' = None..VIEW
+003502f0: 3344 5f4d 545f 7669 6577 3a20 2762 6c5f  3D_MT_view: 'bl_
+00350300: 7569 2e73 7061 6365 5f76 6965 7733 642e  ui.space_view3d.
+00350310: 5649 4557 3344 5f4d 545f 7669 6577 2720  VIEW3D_MT_view' 
+00350320: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f4d  = None..VIEW3D_M
+00350330: 545f 7669 6577 5f61 6c69 676e 3a20 2762  T_view_align: 'b
+00350340: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+00350350: 642e 5649 4557 3344 5f4d 545f 7669 6577  d.VIEW3D_MT_view
+00350360: 5f61 6c69 676e 2720 3d20 4e6f 6e65 0a0a  _align' = None..
+00350370: 5649 4557 3344 5f4d 545f 7669 6577 5f61  VIEW3D_MT_view_a
+00350380: 6c69 676e 5f73 656c 6563 7465 643a 2027  lign_selected: '
+00350390: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
+003503a0: 3364 2e56 4945 5733 445f 4d54 5f76 6965  3d.VIEW3D_MT_vie
+003503b0: 775f 616c 6967 6e5f 7365 6c65 6374 6564  w_align_selected
+003503c0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+003503d0: 5f4d 545f 7669 6577 5f63 616d 6572 6173  _MT_view_cameras
+003503e0: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+003503f0: 6965 7733 642e 5649 4557 3344 5f4d 545f  iew3d.VIEW3D_MT_
+00350400: 7669 6577 5f63 616d 6572 6173 2720 3d20  view_cameras' = 
+00350410: 4e6f 6e65 0a0a 5649 4557 3344 5f4d 545f  None..VIEW3D_MT_
+00350420: 7669 6577 5f6c 6f63 616c 3a20 2762 6c5f  view_local: 'bl_
+00350430: 7569 2e73 7061 6365 5f76 6965 7733 642e  ui.space_view3d.
+00350440: 5649 4557 3344 5f4d 545f 7669 6577 5f6c  VIEW3D_MT_view_l
+00350450: 6f63 616c 2720 3d20 4e6f 6e65 0a0a 5649  ocal' = None..VI
+00350460: 4557 3344 5f4d 545f 7669 6577 5f6e 6176  EW3D_MT_view_nav
+00350470: 6967 6174 696f 6e3a 2027 626c 5f75 692e  igation: 'bl_ui.
+00350480: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
+00350490: 5733 445f 4d54 5f76 6965 775f 6e61 7669  W3D_MT_view_navi
+003504a0: 6761 7469 6f6e 2720 3d20 4e6f 6e65 0a0a  gation' = None..
+003504b0: 5649 4557 3344 5f4d 545f 7669 6577 5f70  VIEW3D_MT_view_p
+003504c0: 6965 3a20 2762 6c5f 7569 2e73 7061 6365  ie: 'bl_ui.space
+003504d0: 5f76 6965 7733 642e 5649 4557 3344 5f4d  _view3d.VIEW3D_M
+003504e0: 545f 7669 6577 5f70 6965 2720 3d20 4e6f  T_view_pie' = No
+003504f0: 6e65 0a0a 5649 4557 3344 5f4d 545f 7669  ne..VIEW3D_MT_vi
+00350500: 6577 5f72 6567 696f 6e73 3a20 2762 6c5f  ew_regions: 'bl_
+00350510: 7569 2e73 7061 6365 5f76 6965 7733 642e  ui.space_view3d.
+00350520: 5649 4557 3344 5f4d 545f 7669 6577 5f72  VIEW3D_MT_view_r
+00350530: 6567 696f 6e73 2720 3d20 4e6f 6e65 0a0a  egions' = None..
+00350540: 5649 4557 3344 5f4d 545f 7669 6577 5f76  VIEW3D_MT_view_v
+00350550: 6965 7770 6f69 6e74 3a20 2762 6c5f 7569  iewpoint: 'bl_ui
+00350560: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
+00350570: 4557 3344 5f4d 545f 7669 6577 5f76 6965  EW3D_MT_view_vie
+00350580: 7770 6f69 6e74 2720 3d20 4e6f 6e65 0a0a  wpoint' = None..
+00350590: 5649 4557 3344 5f4d 545f 766f 6c75 6d65  VIEW3D_MT_volume
+003505a0: 5f61 6464 3a20 2762 6c5f 7569 2e73 7061  _add: 'bl_ui.spa
+003505b0: 6365 5f76 6965 7733 642e 5649 4557 3344  ce_view3d.VIEW3D
+003505c0: 5f4d 545f 766f 6c75 6d65 5f61 6464 2720  _MT_volume_add' 
+003505d0: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f4d  = None..VIEW3D_M
+003505e0: 545f 7765 6967 6874 5f67 7065 6e63 696c  T_weight_gpencil
+003505f0: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+00350600: 6965 7733 642e 5649 4557 3344 5f4d 545f  iew3d.VIEW3D_MT_
+00350610: 7765 6967 6874 5f67 7065 6e63 696c 2720  weight_gpencil' 
+00350620: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f4d  = None..VIEW3D_M
+00350630: 545f 7770 6169 6e74 5f76 6772 6f75 705f  T_wpaint_vgroup_
+00350640: 6c6f 636b 5f70 6965 3a20 2762 6c5f 7569  lock_pie: 'bl_ui
+00350650: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
+00350660: 4557 3344 5f4d 545f 7770 6169 6e74 5f76  EW3D_MT_wpaint_v
+00350670: 6772 6f75 705f 6c6f 636b 5f70 6965 2720  group_lock_pie' 
+00350680: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f4f  = None..VIEW3D_O
+00350690: 545f 6564 6974 5f6d 6573 685f 6578 7472  T_edit_mesh_extr
+003506a0: 7564 655f 696e 6469 7669 6475 616c 5f6d  ude_individual_m
+003506b0: 6f76 653a 2027 626c 5f6f 7065 7261 746f  ove: 'bl_operato
+003506c0: 7273 2e76 6965 7733 642e 5649 4557 3344  rs.view3d.VIEW3D
+003506d0: 5f4f 545f 6564 6974 5f6d 6573 685f 6578  _OT_edit_mesh_ex
+003506e0: 7472 7564 655f 696e 6469 7669 6475 616c  trude_individual
+003506f0: 5f6d 6f76 6527 203d 204e 6f6e 650a 0a56  _move' = None..V
+00350700: 4945 5733 445f 4f54 5f65 6469 745f 6d65  IEW3D_OT_edit_me
+00350710: 7368 5f65 7874 7275 6465 5f6d 616e 6966  sh_extrude_manif
+00350720: 6f6c 645f 6e6f 726d 616c 3a20 2762 6c5f  old_normal: 'bl_
+00350730: 6f70 6572 6174 6f72 732e 7669 6577 3364  operators.view3d
+00350740: 2e56 4945 5733 445f 4f54 5f65 6469 745f  .VIEW3D_OT_edit_
+00350750: 6d65 7368 5f65 7874 7275 6465 5f6d 616e  mesh_extrude_man
+00350760: 6966 6f6c 645f 6e6f 726d 616c 2720 3d20  ifold_normal' = 
+00350770: 4e6f 6e65 0a0a 5649 4557 3344 5f4f 545f  None..VIEW3D_OT_
+00350780: 7472 616e 7366 6f72 6d5f 6769 7a6d 6f5f  transform_gizmo_
+00350790: 7365 743a 2027 626c 5f6f 7065 7261 746f  set: 'bl_operato
+003507a0: 7273 2e76 6965 7733 642e 5649 4557 3344  rs.view3d.VIEW3D
+003507b0: 5f4f 545f 7472 616e 7366 6f72 6d5f 6769  _OT_transform_gi
+003507c0: 7a6d 6f5f 7365 7427 203d 204e 6f6e 650a  zmo_set' = None.
+003507d0: 0a56 4945 5733 445f 5054 5f61 6374 6976  .VIEW3D_PT_activ
+003507e0: 655f 746f 6f6c 3a20 2762 6c5f 7569 2e73  e_tool: 'bl_ui.s
+003507f0: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
+00350800: 3344 5f50 545f 6163 7469 7665 5f74 6f6f  3D_PT_active_too
+00350810: 6c27 203d 204e 6f6e 650a 0a56 4945 5733  l' = None..VIEW3
+00350820: 445f 5054 5f61 6374 6976 655f 746f 6f6c  D_PT_active_tool
+00350830: 5f64 7570 6c69 6361 7465 3a20 2762 6c5f  _duplicate: 'bl_
+00350840: 7569 2e73 7061 6365 5f76 6965 7733 642e  ui.space_view3d.
+00350850: 5649 4557 3344 5f50 545f 6163 7469 7665  VIEW3D_PT_active
+00350860: 5f74 6f6f 6c5f 6475 706c 6963 6174 6527  _tool_duplicate'
+00350870: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
+00350880: 5054 5f61 6e6e 6f74 6174 696f 6e5f 6f6e  PT_annotation_on
+00350890: 696f 6e3a 2027 626c 5f75 692e 7370 6163  ion: 'bl_ui.spac
+003508a0: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
+003508b0: 5054 5f61 6e6e 6f74 6174 696f 6e5f 6f6e  PT_annotation_on
+003508c0: 696f 6e27 203d 204e 6f6e 650a 0a56 4945  ion' = None..VIE
+003508d0: 5733 445f 5054 5f63 6f6c 6c65 6374 696f  W3D_PT_collectio
+003508e0: 6e73 3a20 2762 6c5f 7569 2e73 7061 6365  ns: 'bl_ui.space
+003508f0: 5f76 6965 7733 642e 5649 4557 3344 5f50  _view3d.VIEW3D_P
+00350900: 545f 636f 6c6c 6563 7469 6f6e 7327 203d  T_collections' =
+00350910: 204e 6f6e 650a 0a56 4945 5733 445f 5054   None..VIEW3D_PT
+00350920: 5f63 6f6e 7465 7874 5f70 726f 7065 7274  _context_propert
+00350930: 6965 733a 2027 626c 5f75 692e 7370 6163  ies: 'bl_ui.spac
+00350940: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
+00350950: 5054 5f63 6f6e 7465 7874 5f70 726f 7065  PT_context_prope
+00350960: 7274 6965 7327 203d 204e 6f6e 650a 0a56  rties' = None..V
+00350970: 4945 5733 445f 5054 5f63 7572 7665 735f  IEW3D_PT_curves_
+00350980: 7363 756c 7074 5f61 6464 5f73 6861 7065  sculpt_add_shape
+00350990: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+003509a0: 6965 7733 642e 5649 4557 3344 5f50 545f  iew3d.VIEW3D_PT_
+003509b0: 6375 7276 6573 5f73 6375 6c70 745f 6164  curves_sculpt_ad
+003509c0: 645f 7368 6170 6527 203d 204e 6f6e 650a  d_shape' = None.
+003509d0: 0a56 4945 5733 445f 5054 5f63 7572 7665  .VIEW3D_PT_curve
+003509e0: 735f 7363 756c 7074 5f67 726f 775f 7368  s_sculpt_grow_sh
+003509f0: 7269 6e6b 5f73 6361 6c69 6e67 3a20 2762  rink_scaling: 'b
+00350a00: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+00350a10: 642e 5649 4557 3344 5f50 545f 6375 7276  d.VIEW3D_PT_curv
+00350a20: 6573 5f73 6375 6c70 745f 6772 6f77 5f73  es_sculpt_grow_s
+00350a30: 6872 696e 6b5f 7363 616c 696e 6727 203d  hrink_scaling' =
+00350a40: 204e 6f6e 650a 0a56 4945 5733 445f 5054   None..VIEW3D_PT
+00350a50: 5f63 7572 7665 735f 7363 756c 7074 5f70  _curves_sculpt_p
+00350a60: 6172 616d 6574 6572 5f66 616c 6c6f 6666  arameter_falloff
+00350a70: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+00350a80: 6965 7733 642e 5649 4557 3344 5f50 545f  iew3d.VIEW3D_PT_
+00350a90: 6375 7276 6573 5f73 6375 6c70 745f 7061  curves_sculpt_pa
+00350aa0: 7261 6d65 7465 725f 6661 6c6c 6f66 6627  rameter_falloff'
+00350ab0: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
+00350ac0: 5054 5f63 7572 7665 735f 7363 756c 7074  PT_curves_sculpt
+00350ad0: 5f73 796d 6d65 7472 793a 2027 626c 5f75  _symmetry: 'bl_u
+00350ae0: 692e 7370 6163 655f 7669 6577 3364 5f74  i.space_view3d_t
+00350af0: 6f6f 6c62 6172 2e56 4945 5733 445f 5054  oolbar.VIEW3D_PT
+00350b00: 5f63 7572 7665 735f 7363 756c 7074 5f73  _curves_sculpt_s
+00350b10: 796d 6d65 7472 7927 203d 204e 6f6e 650a  ymmetry' = None.
+00350b20: 0a56 4945 5733 445f 5054 5f63 7572 7665  .VIEW3D_PT_curve
+00350b30: 735f 7363 756c 7074 5f73 796d 6d65 7472  s_sculpt_symmetr
+00350b40: 795f 666f 725f 746f 7062 6172 3a20 2762  y_for_topbar: 'b
+00350b50: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+00350b60: 645f 746f 6f6c 6261 722e 5649 4557 3344  d_toolbar.VIEW3D
+00350b70: 5f50 545f 6375 7276 6573 5f73 6375 6c70  _PT_curves_sculp
+00350b80: 745f 7379 6d6d 6574 7279 5f66 6f72 5f74  t_symmetry_for_t
+00350b90: 6f70 6261 7227 203d 204e 6f6e 650a 0a56  opbar' = None..V
+00350ba0: 4945 5733 445f 5054 5f67 697a 6d6f 5f64  IEW3D_PT_gizmo_d
+00350bb0: 6973 706c 6179 3a20 2762 6c5f 7569 2e73  isplay: 'bl_ui.s
+00350bc0: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
+00350bd0: 3344 5f50 545f 6769 7a6d 6f5f 6469 7370  3D_PT_gizmo_disp
+00350be0: 6c61 7927 203d 204e 6f6e 650a 0a56 4945  lay' = None..VIE
+00350bf0: 5733 445f 5054 5f67 7065 6e63 696c 5f62  W3D_PT_gpencil_b
+00350c00: 7275 7368 5f70 7265 7365 7473 3a20 2762  rush_presets: 'b
+00350c10: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+00350c20: 645f 746f 6f6c 6261 722e 5649 4557 3344  d_toolbar.VIEW3D
+00350c30: 5f50 545f 6770 656e 6369 6c5f 6272 7573  _PT_gpencil_brus
+00350c40: 685f 7072 6573 6574 7327 203d 204e 6f6e  h_presets' = Non
+00350c50: 650a 0a56 4945 5733 445f 5054 5f67 7065  e..VIEW3D_PT_gpe
+00350c60: 6e63 696c 5f63 7572 7665 5f65 6469 743a  ncil_curve_edit:
+00350c70: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+00350c80: 6577 3364 2e56 4945 5733 445f 5054 5f67  ew3d.VIEW3D_PT_g
+00350c90: 7065 6e63 696c 5f63 7572 7665 5f65 6469  pencil_curve_edi
+00350ca0: 7427 203d 204e 6f6e 650a 0a56 4945 5733  t' = None..VIEW3
+00350cb0: 445f 5054 5f67 7065 6e63 696c 5f64 7261  D_PT_gpencil_dra
+00350cc0: 775f 636f 6e74 6578 745f 6d65 6e75 3a20  w_context_menu: 
 00350cd0: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
 00350ce0: 7733 642e 5649 4557 3344 5f50 545f 6770  w3d.VIEW3D_PT_gp
-00350cf0: 656e 6369 6c5f 6775 6964 6527 203d 204e  encil_guide' = N
-00350d00: 6f6e 650a 0a56 4945 5733 445f 5054 5f67  one..VIEW3D_PT_g
-00350d10: 7065 6e63 696c 5f6c 6f63 6b3a 2027 626c  pencil_lock: 'bl
-00350d20: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
-00350d30: 2e56 4945 5733 445f 5054 5f67 7065 6e63  .VIEW3D_PT_gpenc
-00350d40: 696c 5f6c 6f63 6b27 203d 204e 6f6e 650a  il_lock' = None.
-00350d50: 0a56 4945 5733 445f 5054 5f67 7065 6e63  .VIEW3D_PT_gpenc
-00350d60: 696c 5f6d 756c 7469 5f66 7261 6d65 3a20  il_multi_frame: 
-00350d70: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-00350d80: 7733 642e 5649 4557 3344 5f50 545f 6770  w3d.VIEW3D_PT_gp
-00350d90: 656e 6369 6c5f 6d75 6c74 695f 6672 616d  encil_multi_fram
-00350da0: 6527 203d 204e 6f6e 650a 0a56 4945 5733  e' = None..VIEW3
-00350db0: 445f 5054 5f67 7065 6e63 696c 5f6f 7269  D_PT_gpencil_ori
-00350dc0: 6769 6e3a 2027 626c 5f75 692e 7370 6163  gin: 'bl_ui.spac
-00350dd0: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
-00350de0: 5054 5f67 7065 6e63 696c 5f6f 7269 6769  PT_gpencil_origi
-00350df0: 6e27 203d 204e 6f6e 650a 0a56 4945 5733  n' = None..VIEW3
-00350e00: 445f 5054 5f67 7065 6e63 696c 5f73 6375  D_PT_gpencil_scu
-00350e10: 6c70 745f 6175 746f 6d61 736b 696e 673a  lpt_automasking:
-00350e20: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-00350e30: 6577 3364 2e56 4945 5733 445f 5054 5f67  ew3d.VIEW3D_PT_g
-00350e40: 7065 6e63 696c 5f73 6375 6c70 745f 6175  pencil_sculpt_au
-00350e50: 746f 6d61 736b 696e 6727 203d 204e 6f6e  tomasking' = Non
-00350e60: 650a 0a56 4945 5733 445f 5054 5f67 7065  e..VIEW3D_PT_gpe
-00350e70: 6e63 696c 5f73 6375 6c70 745f 636f 6e74  ncil_sculpt_cont
-00350e80: 6578 745f 6d65 6e75 3a20 2762 6c5f 7569  ext_menu: 'bl_ui
-00350e90: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
-00350ea0: 4557 3344 5f50 545f 6770 656e 6369 6c5f  EW3D_PT_gpencil_
-00350eb0: 7363 756c 7074 5f63 6f6e 7465 7874 5f6d  sculpt_context_m
-00350ec0: 656e 7527 203d 204e 6f6e 650a 0a56 4945  enu' = None..VIE
-00350ed0: 5733 445f 5054 5f67 7065 6e63 696c 5f76  W3D_PT_gpencil_v
-00350ee0: 6572 7465 785f 636f 6e74 6578 745f 6d65  ertex_context_me
-00350ef0: 6e75 3a20 2762 6c5f 7569 2e73 7061 6365  nu: 'bl_ui.space
-00350f00: 5f76 6965 7733 642e 5649 4557 3344 5f50  _view3d.VIEW3D_P
-00350f10: 545f 6770 656e 6369 6c5f 7665 7274 6578  T_gpencil_vertex
-00350f20: 5f63 6f6e 7465 7874 5f6d 656e 7527 203d  _context_menu' =
-00350f30: 204e 6f6e 650a 0a56 4945 5733 445f 5054   None..VIEW3D_PT
-00350f40: 5f67 7065 6e63 696c 5f77 6569 6768 745f  _gpencil_weight_
-00350f50: 636f 6e74 6578 745f 6d65 6e75 3a20 2762  context_menu: 'b
-00350f60: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-00350f70: 642e 5649 4557 3344 5f50 545f 6770 656e  d.VIEW3D_PT_gpen
-00350f80: 6369 6c5f 7765 6967 6874 5f63 6f6e 7465  cil_weight_conte
-00350f90: 7874 5f6d 656e 7527 203d 204e 6f6e 650a  xt_menu' = None.
-00350fa0: 0a56 4945 5733 445f 5054 5f67 7265 6173  .VIEW3D_PT_greas
-00350fb0: 655f 7065 6e63 696c 3a20 2762 6c5f 7569  e_pencil: 'bl_ui
-00350fc0: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
-00350fd0: 4557 3344 5f50 545f 6772 6561 7365 5f70  EW3D_PT_grease_p
-00350fe0: 656e 6369 6c27 203d 204e 6f6e 650a 0a56  encil' = None..V
-00350ff0: 4945 5733 445f 5054 5f6d 6173 6b3a 2027  IEW3D_PT_mask: '
-00351000: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
-00351010: 3364 5f74 6f6f 6c62 6172 2e56 4945 5733  3d_toolbar.VIEW3
-00351020: 445f 5054 5f6d 6173 6b27 203d 204e 6f6e  D_PT_mask' = Non
-00351030: 650a 0a56 4945 5733 445f 5054 5f6f 626a  e..VIEW3D_PT_obj
-00351040: 6563 745f 7479 7065 5f76 6973 6962 696c  ect_type_visibil
-00351050: 6974 793a 2027 626c 5f75 692e 7370 6163  ity: 'bl_ui.spac
-00351060: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
-00351070: 5054 5f6f 626a 6563 745f 7479 7065 5f76  PT_object_type_v
-00351080: 6973 6962 696c 6974 7927 203d 204e 6f6e  isibility' = Non
-00351090: 650a 0a56 4945 5733 445f 5054 5f6f 7665  e..VIEW3D_PT_ove
-003510a0: 726c 6179 3a20 2762 6c5f 7569 2e73 7061  rlay: 'bl_ui.spa
-003510b0: 6365 5f76 6965 7733 642e 5649 4557 3344  ce_view3d.VIEW3D
-003510c0: 5f50 545f 6f76 6572 6c61 7927 203d 204e  _PT_overlay' = N
-003510d0: 6f6e 650a 0a56 4945 5733 445f 5054 5f6f  one..VIEW3D_PT_o
-003510e0: 7665 726c 6179 5f62 6f6e 6573 3a20 2762  verlay_bones: 'b
-003510f0: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-00351100: 642e 5649 4557 3344 5f50 545f 6f76 6572  d.VIEW3D_PT_over
-00351110: 6c61 795f 626f 6e65 7327 203d 204e 6f6e  lay_bones' = Non
-00351120: 650a 0a56 4945 5733 445f 5054 5f6f 7665  e..VIEW3D_PT_ove
-00351130: 726c 6179 5f65 6469 745f 6375 7276 653a  rlay_edit_curve:
-00351140: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-00351150: 6577 3364 2e56 4945 5733 445f 5054 5f6f  ew3d.VIEW3D_PT_o
-00351160: 7665 726c 6179 5f65 6469 745f 6375 7276  verlay_edit_curv
-00351170: 6527 203d 204e 6f6e 650a 0a56 4945 5733  e' = None..VIEW3
-00351180: 445f 5054 5f6f 7665 726c 6179 5f65 6469  D_PT_overlay_edi
-00351190: 745f 6d65 7368 3a20 2762 6c5f 7569 2e73  t_mesh: 'bl_ui.s
-003511a0: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
-003511b0: 3344 5f50 545f 6f76 6572 6c61 795f 6564  3D_PT_overlay_ed
-003511c0: 6974 5f6d 6573 6827 203d 204e 6f6e 650a  it_mesh' = None.
-003511d0: 0a56 4945 5733 445f 5054 5f6f 7665 726c  .VIEW3D_PT_overl
-003511e0: 6179 5f65 6469 745f 6d65 7368 5f66 7265  ay_edit_mesh_fre
-003511f0: 6573 7479 6c65 3a20 2762 6c5f 7569 2e73  estyle: 'bl_ui.s
-00351200: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
-00351210: 3344 5f50 545f 6f76 6572 6c61 795f 6564  3D_PT_overlay_ed
-00351220: 6974 5f6d 6573 685f 6672 6565 7374 796c  it_mesh_freestyl
-00351230: 6527 203d 204e 6f6e 650a 0a56 4945 5733  e' = None..VIEW3
-00351240: 445f 5054 5f6f 7665 726c 6179 5f65 6469  D_PT_overlay_edi
-00351250: 745f 6d65 7368 5f6d 6561 7375 7265 6d65  t_mesh_measureme
-00351260: 6e74 3a20 2762 6c5f 7569 2e73 7061 6365  nt: 'bl_ui.space
-00351270: 5f76 6965 7733 642e 5649 4557 3344 5f50  _view3d.VIEW3D_P
-00351280: 545f 6f76 6572 6c61 795f 6564 6974 5f6d  T_overlay_edit_m
-00351290: 6573 685f 6d65 6173 7572 656d 656e 7427  esh_measurement'
-003512a0: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
-003512b0: 5054 5f6f 7665 726c 6179 5f65 6469 745f  PT_overlay_edit_
-003512c0: 6d65 7368 5f6e 6f72 6d61 6c73 3a20 2762  mesh_normals: 'b
-003512d0: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-003512e0: 642e 5649 4557 3344 5f50 545f 6f76 6572  d.VIEW3D_PT_over
-003512f0: 6c61 795f 6564 6974 5f6d 6573 685f 6e6f  lay_edit_mesh_no
-00351300: 726d 616c 7327 203d 204e 6f6e 650a 0a56  rmals' = None..V
-00351310: 4945 5733 445f 5054 5f6f 7665 726c 6179  IEW3D_PT_overlay
-00351320: 5f65 6469 745f 6d65 7368 5f73 6861 6469  _edit_mesh_shadi
-00351330: 6e67 3a20 2762 6c5f 7569 2e73 7061 6365  ng: 'bl_ui.space
-00351340: 5f76 6965 7733 642e 5649 4557 3344 5f50  _view3d.VIEW3D_P
-00351350: 545f 6f76 6572 6c61 795f 6564 6974 5f6d  T_overlay_edit_m
-00351360: 6573 685f 7368 6164 696e 6727 203d 204e  esh_shading' = N
-00351370: 6f6e 650a 0a56 4945 5733 445f 5054 5f6f  one..VIEW3D_PT_o
-00351380: 7665 726c 6179 5f67 656f 6d65 7472 793a  verlay_geometry:
-00351390: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-003513a0: 6577 3364 2e56 4945 5733 445f 5054 5f6f  ew3d.VIEW3D_PT_o
-003513b0: 7665 726c 6179 5f67 656f 6d65 7472 7927  verlay_geometry'
-003513c0: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
-003513d0: 5054 5f6f 7665 726c 6179 5f67 7065 6e63  PT_overlay_gpenc
-003513e0: 696c 5f6f 7074 696f 6e73 3a20 2762 6c5f  il_options: 'bl_
-003513f0: 7569 2e73 7061 6365 5f76 6965 7733 642e  ui.space_view3d.
-00351400: 5649 4557 3344 5f50 545f 6f76 6572 6c61  VIEW3D_PT_overla
-00351410: 795f 6770 656e 6369 6c5f 6f70 7469 6f6e  y_gpencil_option
-00351420: 7327 203d 204e 6f6e 650a 0a56 4945 5733  s' = None..VIEW3
-00351430: 445f 5054 5f6f 7665 726c 6179 5f67 7569  D_PT_overlay_gui
-00351440: 6465 733a 2027 626c 5f75 692e 7370 6163  des: 'bl_ui.spac
-00351450: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
-00351460: 5054 5f6f 7665 726c 6179 5f67 7569 6465  PT_overlay_guide
-00351470: 7327 203d 204e 6f6e 650a 0a56 4945 5733  s' = None..VIEW3
-00351480: 445f 5054 5f6f 7665 726c 6179 5f6d 6f74  D_PT_overlay_mot
-00351490: 696f 6e5f 7472 6163 6b69 6e67 3a20 2762  ion_tracking: 'b
-003514a0: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-003514b0: 642e 5649 4557 3344 5f50 545f 6f76 6572  d.VIEW3D_PT_over
-003514c0: 6c61 795f 6d6f 7469 6f6e 5f74 7261 636b  lay_motion_track
-003514d0: 696e 6727 203d 204e 6f6e 650a 0a56 4945  ing' = None..VIE
-003514e0: 5733 445f 5054 5f6f 7665 726c 6179 5f6f  W3D_PT_overlay_o
-003514f0: 626a 6563 743a 2027 626c 5f75 692e 7370  bject: 'bl_ui.sp
-00351500: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
-00351510: 445f 5054 5f6f 7665 726c 6179 5f6f 626a  D_PT_overlay_obj
-00351520: 6563 7427 203d 204e 6f6e 650a 0a56 4945  ect' = None..VIE
-00351530: 5733 445f 5054 5f6f 7665 726c 6179 5f73  W3D_PT_overlay_s
-00351540: 6375 6c70 743a 2027 626c 5f75 692e 7370  culpt: 'bl_ui.sp
-00351550: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
-00351560: 445f 5054 5f6f 7665 726c 6179 5f73 6375  D_PT_overlay_scu
-00351570: 6c70 7427 203d 204e 6f6e 650a 0a56 4945  lpt' = None..VIE
-00351580: 5733 445f 5054 5f6f 7665 726c 6179 5f73  W3D_PT_overlay_s
-00351590: 6375 6c70 745f 6375 7276 6573 3a20 2762  culpt_curves: 'b
-003515a0: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-003515b0: 642e 5649 4557 3344 5f50 545f 6f76 6572  d.VIEW3D_PT_over
-003515c0: 6c61 795f 7363 756c 7074 5f63 7572 7665  lay_sculpt_curve
-003515d0: 7327 203d 204e 6f6e 650a 0a56 4945 5733  s' = None..VIEW3
-003515e0: 445f 5054 5f6f 7665 726c 6179 5f74 6578  D_PT_overlay_tex
-003515f0: 7475 7265 5f70 6169 6e74 3a20 2762 6c5f  ture_paint: 'bl_
-00351600: 7569 2e73 7061 6365 5f76 6965 7733 642e  ui.space_view3d.
-00351610: 5649 4557 3344 5f50 545f 6f76 6572 6c61  VIEW3D_PT_overla
-00351620: 795f 7465 7874 7572 655f 7061 696e 7427  y_texture_paint'
-00351630: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
-00351640: 5054 5f6f 7665 726c 6179 5f76 6572 7465  PT_overlay_verte
-00351650: 785f 7061 696e 743a 2027 626c 5f75 692e  x_paint: 'bl_ui.
-00351660: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
-00351670: 5733 445f 5054 5f6f 7665 726c 6179 5f76  W3D_PT_overlay_v
-00351680: 6572 7465 785f 7061 696e 7427 203d 204e  ertex_paint' = N
-00351690: 6f6e 650a 0a56 4945 5733 445f 5054 5f6f  one..VIEW3D_PT_o
-003516a0: 7665 726c 6179 5f77 6569 6768 745f 7061  verlay_weight_pa
-003516b0: 696e 743a 2027 626c 5f75 692e 7370 6163  int: 'bl_ui.spac
-003516c0: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
-003516d0: 5054 5f6f 7665 726c 6179 5f77 6569 6768  PT_overlay_weigh
-003516e0: 745f 7061 696e 7427 203d 204e 6f6e 650a  t_paint' = None.
-003516f0: 0a56 4945 5733 445f 5054 5f70 6169 6e74  .VIEW3D_PT_paint
-00351700: 5f74 6578 7475 7265 5f63 6f6e 7465 7874  _texture_context
-00351710: 5f6d 656e 753a 2027 626c 5f75 692e 7370  _menu: 'bl_ui.sp
-00351720: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
-00351730: 445f 5054 5f70 6169 6e74 5f74 6578 7475  D_PT_paint_textu
-00351740: 7265 5f63 6f6e 7465 7874 5f6d 656e 7527  re_context_menu'
-00351750: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
-00351760: 5054 5f70 6169 6e74 5f76 6572 7465 785f  PT_paint_vertex_
-00351770: 636f 6e74 6578 745f 6d65 6e75 3a20 2762  context_menu: 'b
-00351780: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-00351790: 642e 5649 4557 3344 5f50 545f 7061 696e  d.VIEW3D_PT_pain
-003517a0: 745f 7665 7274 6578 5f63 6f6e 7465 7874  t_vertex_context
-003517b0: 5f6d 656e 7527 203d 204e 6f6e 650a 0a56  _menu' = None..V
-003517c0: 4945 5733 445f 5054 5f70 6169 6e74 5f77  IEW3D_PT_paint_w
-003517d0: 6569 6768 745f 636f 6e74 6578 745f 6d65  eight_context_me
-003517e0: 6e75 3a20 2762 6c5f 7569 2e73 7061 6365  nu: 'bl_ui.space
-003517f0: 5f76 6965 7733 642e 5649 4557 3344 5f50  _view3d.VIEW3D_P
-00351800: 545f 7061 696e 745f 7765 6967 6874 5f63  T_paint_weight_c
-00351810: 6f6e 7465 7874 5f6d 656e 7527 203d 204e  ontext_menu' = N
-00351820: 6f6e 650a 0a56 4945 5733 445f 5054 5f70  one..VIEW3D_PT_p
-00351830: 726f 706f 7274 696f 6e61 6c5f 6564 6974  roportional_edit
-00351840: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
-00351850: 6965 7733 642e 5649 4557 3344 5f50 545f  iew3d.VIEW3D_PT_
-00351860: 7072 6f70 6f72 7469 6f6e 616c 5f65 6469  proportional_edi
-00351870: 7427 203d 204e 6f6e 650a 0a56 4945 5733  t' = None..VIEW3
-00351880: 445f 5054 5f71 7561 645f 7669 6577 3a20  D_PT_quad_view: 
-00351890: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-003518a0: 7733 642e 5649 4557 3344 5f50 545f 7175  w3d.VIEW3D_PT_qu
-003518b0: 6164 5f76 6965 7727 203d 204e 6f6e 650a  ad_view' = None.
-003518c0: 0a56 4945 5733 445f 5054 5f73 6375 6c70  .VIEW3D_PT_sculp
-003518d0: 745f 6175 746f 6d61 736b 696e 673a 2027  t_automasking: '
-003518e0: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
-003518f0: 3364 2e56 4945 5733 445f 5054 5f73 6375  3d.VIEW3D_PT_scu
-00351900: 6c70 745f 6175 746f 6d61 736b 696e 6727  lpt_automasking'
-00351910: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
-00351920: 5054 5f73 6375 6c70 745f 636f 6e74 6578  PT_sculpt_contex
-00351930: 745f 6d65 6e75 3a20 2762 6c5f 7569 2e73  t_menu: 'bl_ui.s
-00351940: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
-00351950: 3344 5f50 545f 7363 756c 7074 5f63 6f6e  3D_PT_sculpt_con
-00351960: 7465 7874 5f6d 656e 7527 203d 204e 6f6e  text_menu' = Non
+00350cf0: 656e 6369 6c5f 6472 6177 5f63 6f6e 7465  encil_draw_conte
+00350d00: 7874 5f6d 656e 7527 203d 204e 6f6e 650a  xt_menu' = None.
+00350d10: 0a56 4945 5733 445f 5054 5f67 7065 6e63  .VIEW3D_PT_gpenc
+00350d20: 696c 5f67 7569 6465 3a20 2762 6c5f 7569  il_guide: 'bl_ui
+00350d30: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
+00350d40: 4557 3344 5f50 545f 6770 656e 6369 6c5f  EW3D_PT_gpencil_
+00350d50: 6775 6964 6527 203d 204e 6f6e 650a 0a56  guide' = None..V
+00350d60: 4945 5733 445f 5054 5f67 7065 6e63 696c  IEW3D_PT_gpencil
+00350d70: 5f6c 6f63 6b3a 2027 626c 5f75 692e 7370  _lock: 'bl_ui.sp
+00350d80: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
+00350d90: 445f 5054 5f67 7065 6e63 696c 5f6c 6f63  D_PT_gpencil_loc
+00350da0: 6b27 203d 204e 6f6e 650a 0a56 4945 5733  k' = None..VIEW3
+00350db0: 445f 5054 5f67 7065 6e63 696c 5f6d 756c  D_PT_gpencil_mul
+00350dc0: 7469 5f66 7261 6d65 3a20 2762 6c5f 7569  ti_frame: 'bl_ui
+00350dd0: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
+00350de0: 4557 3344 5f50 545f 6770 656e 6369 6c5f  EW3D_PT_gpencil_
+00350df0: 6d75 6c74 695f 6672 616d 6527 203d 204e  multi_frame' = N
+00350e00: 6f6e 650a 0a56 4945 5733 445f 5054 5f67  one..VIEW3D_PT_g
+00350e10: 7065 6e63 696c 5f6f 7269 6769 6e3a 2027  pencil_origin: '
+00350e20: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
+00350e30: 3364 2e56 4945 5733 445f 5054 5f67 7065  3d.VIEW3D_PT_gpe
+00350e40: 6e63 696c 5f6f 7269 6769 6e27 203d 204e  ncil_origin' = N
+00350e50: 6f6e 650a 0a56 4945 5733 445f 5054 5f67  one..VIEW3D_PT_g
+00350e60: 7065 6e63 696c 5f73 6375 6c70 745f 6175  pencil_sculpt_au
+00350e70: 746f 6d61 736b 696e 673a 2027 626c 5f75  tomasking: 'bl_u
+00350e80: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
+00350e90: 4945 5733 445f 5054 5f67 7065 6e63 696c  IEW3D_PT_gpencil
+00350ea0: 5f73 6375 6c70 745f 6175 746f 6d61 736b  _sculpt_automask
+00350eb0: 696e 6727 203d 204e 6f6e 650a 0a56 4945  ing' = None..VIE
+00350ec0: 5733 445f 5054 5f67 7065 6e63 696c 5f73  W3D_PT_gpencil_s
+00350ed0: 6375 6c70 745f 636f 6e74 6578 745f 6d65  culpt_context_me
+00350ee0: 6e75 3a20 2762 6c5f 7569 2e73 7061 6365  nu: 'bl_ui.space
+00350ef0: 5f76 6965 7733 642e 5649 4557 3344 5f50  _view3d.VIEW3D_P
+00350f00: 545f 6770 656e 6369 6c5f 7363 756c 7074  T_gpencil_sculpt
+00350f10: 5f63 6f6e 7465 7874 5f6d 656e 7527 203d  _context_menu' =
+00350f20: 204e 6f6e 650a 0a56 4945 5733 445f 5054   None..VIEW3D_PT
+00350f30: 5f67 7065 6e63 696c 5f76 6572 7465 785f  _gpencil_vertex_
+00350f40: 636f 6e74 6578 745f 6d65 6e75 3a20 2762  context_menu: 'b
+00350f50: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+00350f60: 642e 5649 4557 3344 5f50 545f 6770 656e  d.VIEW3D_PT_gpen
+00350f70: 6369 6c5f 7665 7274 6578 5f63 6f6e 7465  cil_vertex_conte
+00350f80: 7874 5f6d 656e 7527 203d 204e 6f6e 650a  xt_menu' = None.
+00350f90: 0a56 4945 5733 445f 5054 5f67 7065 6e63  .VIEW3D_PT_gpenc
+00350fa0: 696c 5f77 6569 6768 745f 636f 6e74 6578  il_weight_contex
+00350fb0: 745f 6d65 6e75 3a20 2762 6c5f 7569 2e73  t_menu: 'bl_ui.s
+00350fc0: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
+00350fd0: 3344 5f50 545f 6770 656e 6369 6c5f 7765  3D_PT_gpencil_we
+00350fe0: 6967 6874 5f63 6f6e 7465 7874 5f6d 656e  ight_context_men
+00350ff0: 7527 203d 204e 6f6e 650a 0a56 4945 5733  u' = None..VIEW3
+00351000: 445f 5054 5f67 7265 6173 655f 7065 6e63  D_PT_grease_penc
+00351010: 696c 3a20 2762 6c5f 7569 2e73 7061 6365  il: 'bl_ui.space
+00351020: 5f76 6965 7733 642e 5649 4557 3344 5f50  _view3d.VIEW3D_P
+00351030: 545f 6772 6561 7365 5f70 656e 6369 6c27  T_grease_pencil'
+00351040: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
+00351050: 5054 5f6d 6173 6b3a 2027 626c 5f75 692e  PT_mask: 'bl_ui.
+00351060: 7370 6163 655f 7669 6577 3364 5f74 6f6f  space_view3d_too
+00351070: 6c62 6172 2e56 4945 5733 445f 5054 5f6d  lbar.VIEW3D_PT_m
+00351080: 6173 6b27 203d 204e 6f6e 650a 0a56 4945  ask' = None..VIE
+00351090: 5733 445f 5054 5f6f 626a 6563 745f 7479  W3D_PT_object_ty
+003510a0: 7065 5f76 6973 6962 696c 6974 793a 2027  pe_visibility: '
+003510b0: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
+003510c0: 3364 2e56 4945 5733 445f 5054 5f6f 626a  3d.VIEW3D_PT_obj
+003510d0: 6563 745f 7479 7065 5f76 6973 6962 696c  ect_type_visibil
+003510e0: 6974 7927 203d 204e 6f6e 650a 0a56 4945  ity' = None..VIE
+003510f0: 5733 445f 5054 5f6f 7665 726c 6179 3a20  W3D_PT_overlay: 
+00351100: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
+00351110: 7733 642e 5649 4557 3344 5f50 545f 6f76  w3d.VIEW3D_PT_ov
+00351120: 6572 6c61 7927 203d 204e 6f6e 650a 0a56  erlay' = None..V
+00351130: 4945 5733 445f 5054 5f6f 7665 726c 6179  IEW3D_PT_overlay
+00351140: 5f62 6f6e 6573 3a20 2762 6c5f 7569 2e73  _bones: 'bl_ui.s
+00351150: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
+00351160: 3344 5f50 545f 6f76 6572 6c61 795f 626f  3D_PT_overlay_bo
+00351170: 6e65 7327 203d 204e 6f6e 650a 0a56 4945  nes' = None..VIE
+00351180: 5733 445f 5054 5f6f 7665 726c 6179 5f65  W3D_PT_overlay_e
+00351190: 6469 745f 6375 7276 653a 2027 626c 5f75  dit_curve: 'bl_u
+003511a0: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
+003511b0: 4945 5733 445f 5054 5f6f 7665 726c 6179  IEW3D_PT_overlay
+003511c0: 5f65 6469 745f 6375 7276 6527 203d 204e  _edit_curve' = N
+003511d0: 6f6e 650a 0a56 4945 5733 445f 5054 5f6f  one..VIEW3D_PT_o
+003511e0: 7665 726c 6179 5f65 6469 745f 6d65 7368  verlay_edit_mesh
+003511f0: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+00351200: 6965 7733 642e 5649 4557 3344 5f50 545f  iew3d.VIEW3D_PT_
+00351210: 6f76 6572 6c61 795f 6564 6974 5f6d 6573  overlay_edit_mes
+00351220: 6827 203d 204e 6f6e 650a 0a56 4945 5733  h' = None..VIEW3
+00351230: 445f 5054 5f6f 7665 726c 6179 5f65 6469  D_PT_overlay_edi
+00351240: 745f 6d65 7368 5f66 7265 6573 7479 6c65  t_mesh_freestyle
+00351250: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+00351260: 6965 7733 642e 5649 4557 3344 5f50 545f  iew3d.VIEW3D_PT_
+00351270: 6f76 6572 6c61 795f 6564 6974 5f6d 6573  overlay_edit_mes
+00351280: 685f 6672 6565 7374 796c 6527 203d 204e  h_freestyle' = N
+00351290: 6f6e 650a 0a56 4945 5733 445f 5054 5f6f  one..VIEW3D_PT_o
+003512a0: 7665 726c 6179 5f65 6469 745f 6d65 7368  verlay_edit_mesh
+003512b0: 5f6d 6561 7375 7265 6d65 6e74 3a20 2762  _measurement: 'b
+003512c0: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+003512d0: 642e 5649 4557 3344 5f50 545f 6f76 6572  d.VIEW3D_PT_over
+003512e0: 6c61 795f 6564 6974 5f6d 6573 685f 6d65  lay_edit_mesh_me
+003512f0: 6173 7572 656d 656e 7427 203d 204e 6f6e  asurement' = Non
+00351300: 650a 0a56 4945 5733 445f 5054 5f6f 7665  e..VIEW3D_PT_ove
+00351310: 726c 6179 5f65 6469 745f 6d65 7368 5f6e  rlay_edit_mesh_n
+00351320: 6f72 6d61 6c73 3a20 2762 6c5f 7569 2e73  ormals: 'bl_ui.s
+00351330: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
+00351340: 3344 5f50 545f 6f76 6572 6c61 795f 6564  3D_PT_overlay_ed
+00351350: 6974 5f6d 6573 685f 6e6f 726d 616c 7327  it_mesh_normals'
+00351360: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
+00351370: 5054 5f6f 7665 726c 6179 5f65 6469 745f  PT_overlay_edit_
+00351380: 6d65 7368 5f73 6861 6469 6e67 3a20 2762  mesh_shading: 'b
+00351390: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+003513a0: 642e 5649 4557 3344 5f50 545f 6f76 6572  d.VIEW3D_PT_over
+003513b0: 6c61 795f 6564 6974 5f6d 6573 685f 7368  lay_edit_mesh_sh
+003513c0: 6164 696e 6727 203d 204e 6f6e 650a 0a56  ading' = None..V
+003513d0: 4945 5733 445f 5054 5f6f 7665 726c 6179  IEW3D_PT_overlay
+003513e0: 5f67 656f 6d65 7472 793a 2027 626c 5f75  _geometry: 'bl_u
+003513f0: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
+00351400: 4945 5733 445f 5054 5f6f 7665 726c 6179  IEW3D_PT_overlay
+00351410: 5f67 656f 6d65 7472 7927 203d 204e 6f6e  _geometry' = Non
+00351420: 650a 0a56 4945 5733 445f 5054 5f6f 7665  e..VIEW3D_PT_ove
+00351430: 726c 6179 5f67 7065 6e63 696c 5f6f 7074  rlay_gpencil_opt
+00351440: 696f 6e73 3a20 2762 6c5f 7569 2e73 7061  ions: 'bl_ui.spa
+00351450: 6365 5f76 6965 7733 642e 5649 4557 3344  ce_view3d.VIEW3D
+00351460: 5f50 545f 6f76 6572 6c61 795f 6770 656e  _PT_overlay_gpen
+00351470: 6369 6c5f 6f70 7469 6f6e 7327 203d 204e  cil_options' = N
+00351480: 6f6e 650a 0a56 4945 5733 445f 5054 5f6f  one..VIEW3D_PT_o
+00351490: 7665 726c 6179 5f67 7569 6465 733a 2027  verlay_guides: '
+003514a0: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
+003514b0: 3364 2e56 4945 5733 445f 5054 5f6f 7665  3d.VIEW3D_PT_ove
+003514c0: 726c 6179 5f67 7569 6465 7327 203d 204e  rlay_guides' = N
+003514d0: 6f6e 650a 0a56 4945 5733 445f 5054 5f6f  one..VIEW3D_PT_o
+003514e0: 7665 726c 6179 5f6d 6f74 696f 6e5f 7472  verlay_motion_tr
+003514f0: 6163 6b69 6e67 3a20 2762 6c5f 7569 2e73  acking: 'bl_ui.s
+00351500: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
+00351510: 3344 5f50 545f 6f76 6572 6c61 795f 6d6f  3D_PT_overlay_mo
+00351520: 7469 6f6e 5f74 7261 636b 696e 6727 203d  tion_tracking' =
+00351530: 204e 6f6e 650a 0a56 4945 5733 445f 5054   None..VIEW3D_PT
+00351540: 5f6f 7665 726c 6179 5f6f 626a 6563 743a  _overlay_object:
+00351550: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+00351560: 6577 3364 2e56 4945 5733 445f 5054 5f6f  ew3d.VIEW3D_PT_o
+00351570: 7665 726c 6179 5f6f 626a 6563 7427 203d  verlay_object' =
+00351580: 204e 6f6e 650a 0a56 4945 5733 445f 5054   None..VIEW3D_PT
+00351590: 5f6f 7665 726c 6179 5f73 6375 6c70 743a  _overlay_sculpt:
+003515a0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+003515b0: 6577 3364 2e56 4945 5733 445f 5054 5f6f  ew3d.VIEW3D_PT_o
+003515c0: 7665 726c 6179 5f73 6375 6c70 7427 203d  verlay_sculpt' =
+003515d0: 204e 6f6e 650a 0a56 4945 5733 445f 5054   None..VIEW3D_PT
+003515e0: 5f6f 7665 726c 6179 5f73 6375 6c70 745f  _overlay_sculpt_
+003515f0: 6375 7276 6573 3a20 2762 6c5f 7569 2e73  curves: 'bl_ui.s
+00351600: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
+00351610: 3344 5f50 545f 6f76 6572 6c61 795f 7363  3D_PT_overlay_sc
+00351620: 756c 7074 5f63 7572 7665 7327 203d 204e  ulpt_curves' = N
+00351630: 6f6e 650a 0a56 4945 5733 445f 5054 5f6f  one..VIEW3D_PT_o
+00351640: 7665 726c 6179 5f74 6578 7475 7265 5f70  verlay_texture_p
+00351650: 6169 6e74 3a20 2762 6c5f 7569 2e73 7061  aint: 'bl_ui.spa
+00351660: 6365 5f76 6965 7733 642e 5649 4557 3344  ce_view3d.VIEW3D
+00351670: 5f50 545f 6f76 6572 6c61 795f 7465 7874  _PT_overlay_text
+00351680: 7572 655f 7061 696e 7427 203d 204e 6f6e  ure_paint' = Non
+00351690: 650a 0a56 4945 5733 445f 5054 5f6f 7665  e..VIEW3D_PT_ove
+003516a0: 726c 6179 5f76 6572 7465 785f 7061 696e  rlay_vertex_pain
+003516b0: 743a 2027 626c 5f75 692e 7370 6163 655f  t: 'bl_ui.space_
+003516c0: 7669 6577 3364 2e56 4945 5733 445f 5054  view3d.VIEW3D_PT
+003516d0: 5f6f 7665 726c 6179 5f76 6572 7465 785f  _overlay_vertex_
+003516e0: 7061 696e 7427 203d 204e 6f6e 650a 0a56  paint' = None..V
+003516f0: 4945 5733 445f 5054 5f6f 7665 726c 6179  IEW3D_PT_overlay
+00351700: 5f77 6569 6768 745f 7061 696e 743a 2027  _weight_paint: '
+00351710: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
+00351720: 3364 2e56 4945 5733 445f 5054 5f6f 7665  3d.VIEW3D_PT_ove
+00351730: 726c 6179 5f77 6569 6768 745f 7061 696e  rlay_weight_pain
+00351740: 7427 203d 204e 6f6e 650a 0a56 4945 5733  t' = None..VIEW3
+00351750: 445f 5054 5f70 6169 6e74 5f74 6578 7475  D_PT_paint_textu
+00351760: 7265 5f63 6f6e 7465 7874 5f6d 656e 753a  re_context_menu:
+00351770: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+00351780: 6577 3364 2e56 4945 5733 445f 5054 5f70  ew3d.VIEW3D_PT_p
+00351790: 6169 6e74 5f74 6578 7475 7265 5f63 6f6e  aint_texture_con
+003517a0: 7465 7874 5f6d 656e 7527 203d 204e 6f6e  text_menu' = Non
+003517b0: 650a 0a56 4945 5733 445f 5054 5f70 6169  e..VIEW3D_PT_pai
+003517c0: 6e74 5f76 6572 7465 785f 636f 6e74 6578  nt_vertex_contex
+003517d0: 745f 6d65 6e75 3a20 2762 6c5f 7569 2e73  t_menu: 'bl_ui.s
+003517e0: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
+003517f0: 3344 5f50 545f 7061 696e 745f 7665 7274  3D_PT_paint_vert
+00351800: 6578 5f63 6f6e 7465 7874 5f6d 656e 7527  ex_context_menu'
+00351810: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
+00351820: 5054 5f70 6169 6e74 5f77 6569 6768 745f  PT_paint_weight_
+00351830: 636f 6e74 6578 745f 6d65 6e75 3a20 2762  context_menu: 'b
+00351840: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+00351850: 642e 5649 4557 3344 5f50 545f 7061 696e  d.VIEW3D_PT_pain
+00351860: 745f 7765 6967 6874 5f63 6f6e 7465 7874  t_weight_context
+00351870: 5f6d 656e 7527 203d 204e 6f6e 650a 0a56  _menu' = None..V
+00351880: 4945 5733 445f 5054 5f70 726f 706f 7274  IEW3D_PT_proport
+00351890: 696f 6e61 6c5f 6564 6974 3a20 2762 6c5f  ional_edit: 'bl_
+003518a0: 7569 2e73 7061 6365 5f76 6965 7733 642e  ui.space_view3d.
+003518b0: 5649 4557 3344 5f50 545f 7072 6f70 6f72  VIEW3D_PT_propor
+003518c0: 7469 6f6e 616c 5f65 6469 7427 203d 204e  tional_edit' = N
+003518d0: 6f6e 650a 0a56 4945 5733 445f 5054 5f71  one..VIEW3D_PT_q
+003518e0: 7561 645f 7669 6577 3a20 2762 6c5f 7569  uad_view: 'bl_ui
+003518f0: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
+00351900: 4557 3344 5f50 545f 7175 6164 5f76 6965  EW3D_PT_quad_vie
+00351910: 7727 203d 204e 6f6e 650a 0a56 4945 5733  w' = None..VIEW3
+00351920: 445f 5054 5f73 6375 6c70 745f 6175 746f  D_PT_sculpt_auto
+00351930: 6d61 736b 696e 673a 2027 626c 5f75 692e  masking: 'bl_ui.
+00351940: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
+00351950: 5733 445f 5054 5f73 6375 6c70 745f 6175  W3D_PT_sculpt_au
+00351960: 746f 6d61 736b 696e 6727 203d 204e 6f6e  tomasking' = Non
 00351970: 650a 0a56 4945 5733 445f 5054 5f73 6375  e..VIEW3D_PT_scu
-00351980: 6c70 745f 6479 6e74 6f70 6f3a 2027 626c  lpt_dyntopo: 'bl
-00351990: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
-003519a0: 5f74 6f6f 6c62 6172 2e56 4945 5733 445f  _toolbar.VIEW3D_
-003519b0: 5054 5f73 6375 6c70 745f 6479 6e74 6f70  PT_sculpt_dyntop
-003519c0: 6f27 203d 204e 6f6e 650a 0a56 4945 5733  o' = None..VIEW3
-003519d0: 445f 5054 5f73 6375 6c70 745f 6f70 7469  D_PT_sculpt_opti
-003519e0: 6f6e 733a 2027 626c 5f75 692e 7370 6163  ons: 'bl_ui.spac
-003519f0: 655f 7669 6577 3364 5f74 6f6f 6c62 6172  e_view3d_toolbar
-00351a00: 2e56 4945 5733 445f 5054 5f73 6375 6c70  .VIEW3D_PT_sculp
-00351a10: 745f 6f70 7469 6f6e 7327 203d 204e 6f6e  t_options' = Non
-00351a20: 650a 0a56 4945 5733 445f 5054 5f73 6375  e..VIEW3D_PT_scu
-00351a30: 6c70 745f 6f70 7469 6f6e 735f 6772 6176  lpt_options_grav
-00351a40: 6974 793a 2027 626c 5f75 692e 7370 6163  ity: 'bl_ui.spac
-00351a50: 655f 7669 6577 3364 5f74 6f6f 6c62 6172  e_view3d_toolbar
-00351a60: 2e56 4945 5733 445f 5054 5f73 6375 6c70  .VIEW3D_PT_sculp
-00351a70: 745f 6f70 7469 6f6e 735f 6772 6176 6974  t_options_gravit
-00351a80: 7927 203d 204e 6f6e 650a 0a56 4945 5733  y' = None..VIEW3
-00351a90: 445f 5054 5f73 6375 6c70 745f 7379 6d6d  D_PT_sculpt_symm
-00351aa0: 6574 7279 3a20 2762 6c5f 7569 2e73 7061  etry: 'bl_ui.spa
-00351ab0: 6365 5f76 6965 7733 645f 746f 6f6c 6261  ce_view3d_toolba
-00351ac0: 722e 5649 4557 3344 5f50 545f 7363 756c  r.VIEW3D_PT_scul
-00351ad0: 7074 5f73 796d 6d65 7472 7927 203d 204e  pt_symmetry' = N
+00351980: 6c70 745f 636f 6e74 6578 745f 6d65 6e75  lpt_context_menu
+00351990: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+003519a0: 6965 7733 642e 5649 4557 3344 5f50 545f  iew3d.VIEW3D_PT_
+003519b0: 7363 756c 7074 5f63 6f6e 7465 7874 5f6d  sculpt_context_m
+003519c0: 656e 7527 203d 204e 6f6e 650a 0a56 4945  enu' = None..VIE
+003519d0: 5733 445f 5054 5f73 6375 6c70 745f 6479  W3D_PT_sculpt_dy
+003519e0: 6e74 6f70 6f3a 2027 626c 5f75 692e 7370  ntopo: 'bl_ui.sp
+003519f0: 6163 655f 7669 6577 3364 5f74 6f6f 6c62  ace_view3d_toolb
+00351a00: 6172 2e56 4945 5733 445f 5054 5f73 6375  ar.VIEW3D_PT_scu
+00351a10: 6c70 745f 6479 6e74 6f70 6f27 203d 204e  lpt_dyntopo' = N
+00351a20: 6f6e 650a 0a56 4945 5733 445f 5054 5f73  one..VIEW3D_PT_s
+00351a30: 6375 6c70 745f 6f70 7469 6f6e 733a 2027  culpt_options: '
+00351a40: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
+00351a50: 3364 5f74 6f6f 6c62 6172 2e56 4945 5733  3d_toolbar.VIEW3
+00351a60: 445f 5054 5f73 6375 6c70 745f 6f70 7469  D_PT_sculpt_opti
+00351a70: 6f6e 7327 203d 204e 6f6e 650a 0a56 4945  ons' = None..VIE
+00351a80: 5733 445f 5054 5f73 6375 6c70 745f 6f70  W3D_PT_sculpt_op
+00351a90: 7469 6f6e 735f 6772 6176 6974 793a 2027  tions_gravity: '
+00351aa0: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
+00351ab0: 3364 5f74 6f6f 6c62 6172 2e56 4945 5733  3d_toolbar.VIEW3
+00351ac0: 445f 5054 5f73 6375 6c70 745f 6f70 7469  D_PT_sculpt_opti
+00351ad0: 6f6e 735f 6772 6176 6974 7927 203d 204e  ons_gravity' = N
 00351ae0: 6f6e 650a 0a56 4945 5733 445f 5054 5f73  one..VIEW3D_PT_s
-00351af0: 6375 6c70 745f 7379 6d6d 6574 7279 5f66  culpt_symmetry_f
-00351b00: 6f72 5f74 6f70 6261 723a 2027 626c 5f75  or_topbar: 'bl_u
-00351b10: 692e 7370 6163 655f 7669 6577 3364 5f74  i.space_view3d_t
-00351b20: 6f6f 6c62 6172 2e56 4945 5733 445f 5054  oolbar.VIEW3D_PT
-00351b30: 5f73 6375 6c70 745f 7379 6d6d 6574 7279  _sculpt_symmetry
-00351b40: 5f66 6f72 5f74 6f70 6261 7227 203d 204e  _for_topbar' = N
-00351b50: 6f6e 650a 0a56 4945 5733 445f 5054 5f73  one..VIEW3D_PT_s
-00351b60: 6375 6c70 745f 766f 7865 6c5f 7265 6d65  culpt_voxel_reme
-00351b70: 7368 3a20 2762 6c5f 7569 2e73 7061 6365  sh: 'bl_ui.space
-00351b80: 5f76 6965 7733 645f 746f 6f6c 6261 722e  _view3d_toolbar.
-00351b90: 5649 4557 3344 5f50 545f 7363 756c 7074  VIEW3D_PT_sculpt
-00351ba0: 5f76 6f78 656c 5f72 656d 6573 6827 203d  _voxel_remesh' =
-00351bb0: 204e 6f6e 650a 0a56 4945 5733 445f 5054   None..VIEW3D_PT
-00351bc0: 5f73 6861 6469 6e67 3a20 2762 6c5f 7569  _shading: 'bl_ui
-00351bd0: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
-00351be0: 4557 3344 5f50 545f 7368 6164 696e 6727  EW3D_PT_shading'
-00351bf0: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
-00351c00: 5054 5f73 6861 6469 6e67 5f63 6f6c 6f72  PT_shading_color
-00351c10: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
-00351c20: 6965 7733 642e 5649 4557 3344 5f50 545f  iew3d.VIEW3D_PT_
-00351c30: 7368 6164 696e 675f 636f 6c6f 7227 203d  shading_color' =
-00351c40: 204e 6f6e 650a 0a56 4945 5733 445f 5054   None..VIEW3D_PT
-00351c50: 5f73 6861 6469 6e67 5f63 6f6d 706f 7369  _shading_composi
-00351c60: 746f 723a 2027 626c 5f75 692e 7370 6163  tor: 'bl_ui.spac
-00351c70: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
-00351c80: 5054 5f73 6861 6469 6e67 5f63 6f6d 706f  PT_shading_compo
-00351c90: 7369 746f 7227 203d 204e 6f6e 650a 0a56  sitor' = None..V
-00351ca0: 4945 5733 445f 5054 5f73 6861 6469 6e67  IEW3D_PT_shading
-00351cb0: 5f6c 6967 6874 696e 673a 2027 626c 5f75  _lighting: 'bl_u
-00351cc0: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
-00351cd0: 4945 5733 445f 5054 5f73 6861 6469 6e67  IEW3D_PT_shading
-00351ce0: 5f6c 6967 6874 696e 6727 203d 204e 6f6e  _lighting' = Non
-00351cf0: 650a 0a56 4945 5733 445f 5054 5f73 6861  e..VIEW3D_PT_sha
-00351d00: 6469 6e67 5f6f 7074 696f 6e73 3a20 2762  ding_options: 'b
-00351d10: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-00351d20: 642e 5649 4557 3344 5f50 545f 7368 6164  d.VIEW3D_PT_shad
-00351d30: 696e 675f 6f70 7469 6f6e 7327 203d 204e  ing_options' = N
-00351d40: 6f6e 650a 0a56 4945 5733 445f 5054 5f73  one..VIEW3D_PT_s
-00351d50: 6861 6469 6e67 5f6f 7074 696f 6e73 5f73  hading_options_s
-00351d60: 6861 646f 773a 2027 626c 5f75 692e 7370  hadow: 'bl_ui.sp
-00351d70: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
-00351d80: 445f 5054 5f73 6861 6469 6e67 5f6f 7074  D_PT_shading_opt
-00351d90: 696f 6e73 5f73 6861 646f 7727 203d 204e  ions_shadow' = N
-00351da0: 6f6e 650a 0a56 4945 5733 445f 5054 5f73  one..VIEW3D_PT_s
-00351db0: 6861 6469 6e67 5f6f 7074 696f 6e73 5f73  hading_options_s
-00351dc0: 7361 6f3a 2027 626c 5f75 692e 7370 6163  sao: 'bl_ui.spac
-00351dd0: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
-00351de0: 5054 5f73 6861 6469 6e67 5f6f 7074 696f  PT_shading_optio
-00351df0: 6e73 5f73 7361 6f27 203d 204e 6f6e 650a  ns_ssao' = None.
-00351e00: 0a56 4945 5733 445f 5054 5f73 6861 6469  .VIEW3D_PT_shadi
-00351e10: 6e67 5f72 656e 6465 725f 7061 7373 3a20  ng_render_pass: 
-00351e20: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-00351e30: 7733 642e 5649 4557 3344 5f50 545f 7368  w3d.VIEW3D_PT_sh
-00351e40: 6164 696e 675f 7265 6e64 6572 5f70 6173  ading_render_pas
-00351e50: 7327 203d 204e 6f6e 650a 0a56 4945 5733  s' = None..VIEW3
-00351e60: 445f 5054 5f73 6c6f 7473 5f70 6169 6e74  D_PT_slots_paint
-00351e70: 5f63 616e 7661 733a 2027 626c 5f75 692e  _canvas: 'bl_ui.
-00351e80: 7370 6163 655f 7669 6577 3364 5f74 6f6f  space_view3d_too
-00351e90: 6c62 6172 2e56 4945 5733 445f 5054 5f73  lbar.VIEW3D_PT_s
-00351ea0: 6c6f 7473 5f70 6169 6e74 5f63 616e 7661  lots_paint_canva
-00351eb0: 7327 203d 204e 6f6e 650a 0a56 4945 5733  s' = None..VIEW3
-00351ec0: 445f 5054 5f73 6c6f 7473 5f70 726f 6a65  D_PT_slots_proje
-00351ed0: 6374 7061 696e 743a 2027 626c 5f75 692e  ctpaint: 'bl_ui.
-00351ee0: 7370 6163 655f 7669 6577 3364 5f74 6f6f  space_view3d_too
-00351ef0: 6c62 6172 2e56 4945 5733 445f 5054 5f73  lbar.VIEW3D_PT_s
-00351f00: 6c6f 7473 5f70 726f 6a65 6374 7061 696e  lots_projectpain
-00351f10: 7427 203d 204e 6f6e 650a 0a56 4945 5733  t' = None..VIEW3
-00351f20: 445f 5054 5f73 6e61 7070 696e 673a 2027  D_PT_snapping: '
-00351f30: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
-00351f40: 3364 2e56 4945 5733 445f 5054 5f73 6e61  3d.VIEW3D_PT_sna
-00351f50: 7070 696e 6727 203d 204e 6f6e 650a 0a56  pping' = None..V
-00351f60: 4945 5733 445f 5054 5f73 7465 6e63 696c  IEW3D_PT_stencil
-00351f70: 5f70 726f 6a65 6374 7061 696e 743a 2027  _projectpaint: '
-00351f80: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
-00351f90: 3364 5f74 6f6f 6c62 6172 2e56 4945 5733  3d_toolbar.VIEW3
-00351fa0: 445f 5054 5f73 7465 6e63 696c 5f70 726f  D_PT_stencil_pro
-00351fb0: 6a65 6374 7061 696e 7427 203d 204e 6f6e  jectpaint' = Non
-00351fc0: 650a 0a56 4945 5733 445f 5054 5f74 6f6f  e..VIEW3D_PT_too
-00351fd0: 6c73 5f61 6374 6976 653a 2027 626c 5f75  ls_active: 'bl_u
-00351fe0: 692e 7370 6163 655f 746f 6f6c 7379 7374  i.space_toolsyst
-00351ff0: 656d 5f74 6f6f 6c62 6172 2e56 4945 5733  em_toolbar.VIEW3
-00352000: 445f 5054 5f74 6f6f 6c73 5f61 6374 6976  D_PT_tools_activ
-00352010: 6527 203d 204e 6f6e 650a 0a56 4945 5733  e' = None..VIEW3
-00352020: 445f 5054 5f74 6f6f 6c73 5f61 726d 6174  D_PT_tools_armat
-00352030: 7572 6565 6469 745f 6f70 7469 6f6e 733a  ureedit_options:
-00352040: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-00352050: 6577 3364 5f74 6f6f 6c62 6172 2e56 4945  ew3d_toolbar.VIE
-00352060: 5733 445f 5054 5f74 6f6f 6c73 5f61 726d  W3D_PT_tools_arm
-00352070: 6174 7572 6565 6469 745f 6f70 7469 6f6e  atureedit_option
-00352080: 7327 203d 204e 6f6e 650a 0a56 4945 5733  s' = None..VIEW3
-00352090: 445f 5054 5f74 6f6f 6c73 5f62 7275 7368  D_PT_tools_brush
-003520a0: 5f63 6c6f 6e65 3a20 2762 6c5f 7569 2e73  _clone: 'bl_ui.s
-003520b0: 7061 6365 5f76 6965 7733 645f 746f 6f6c  pace_view3d_tool
-003520c0: 6261 722e 5649 4557 3344 5f50 545f 746f  bar.VIEW3D_PT_to
-003520d0: 6f6c 735f 6272 7573 685f 636c 6f6e 6527  ols_brush_clone'
-003520e0: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
-003520f0: 5054 5f74 6f6f 6c73 5f62 7275 7368 5f63  PT_tools_brush_c
-00352100: 6f6c 6f72 3a20 2762 6c5f 7569 2e73 7061  olor: 'bl_ui.spa
-00352110: 6365 5f76 6965 7733 645f 746f 6f6c 6261  ce_view3d_toolba
-00352120: 722e 5649 4557 3344 5f50 545f 746f 6f6c  r.VIEW3D_PT_tool
-00352130: 735f 6272 7573 685f 636f 6c6f 7227 203d  s_brush_color' =
-00352140: 204e 6f6e 650a 0a56 4945 5733 445f 5054   None..VIEW3D_PT
-00352150: 5f74 6f6f 6c73 5f62 7275 7368 5f64 6973  _tools_brush_dis
-00352160: 706c 6179 3a20 2762 6c5f 7569 2e73 7061  play: 'bl_ui.spa
-00352170: 6365 5f76 6965 7733 645f 746f 6f6c 6261  ce_view3d_toolba
-00352180: 722e 5649 4557 3344 5f50 545f 746f 6f6c  r.VIEW3D_PT_tool
-00352190: 735f 6272 7573 685f 6469 7370 6c61 7927  s_brush_display'
-003521a0: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
-003521b0: 5054 5f74 6f6f 6c73 5f62 7275 7368 5f66  PT_tools_brush_f
-003521c0: 616c 6c6f 6666 3a20 2762 6c5f 7569 2e73  alloff: 'bl_ui.s
-003521d0: 7061 6365 5f76 6965 7733 645f 746f 6f6c  pace_view3d_tool
-003521e0: 6261 722e 5649 4557 3344 5f50 545f 746f  bar.VIEW3D_PT_to
-003521f0: 6f6c 735f 6272 7573 685f 6661 6c6c 6f66  ols_brush_fallof
-00352200: 6627 203d 204e 6f6e 650a 0a56 4945 5733  f' = None..VIEW3
-00352210: 445f 5054 5f74 6f6f 6c73 5f62 7275 7368  D_PT_tools_brush
-00352220: 5f66 616c 6c6f 6666 5f66 726f 6e74 6661  _falloff_frontfa
-00352230: 6365 3a20 2762 6c5f 7569 2e73 7061 6365  ce: 'bl_ui.space
-00352240: 5f76 6965 7733 645f 746f 6f6c 6261 722e  _view3d_toolbar.
-00352250: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
-00352260: 6272 7573 685f 6661 6c6c 6f66 665f 6672  brush_falloff_fr
-00352270: 6f6e 7466 6163 6527 203d 204e 6f6e 650a  ontface' = None.
-00352280: 0a56 4945 5733 445f 5054 5f74 6f6f 6c73  .VIEW3D_PT_tools
-00352290: 5f62 7275 7368 5f66 616c 6c6f 6666 5f6e  _brush_falloff_n
-003522a0: 6f72 6d61 6c3a 2027 626c 5f75 692e 7370  ormal: 'bl_ui.sp
-003522b0: 6163 655f 7669 6577 3364 5f74 6f6f 6c62  ace_view3d_toolb
-003522c0: 6172 2e56 4945 5733 445f 5054 5f74 6f6f  ar.VIEW3D_PT_too
-003522d0: 6c73 5f62 7275 7368 5f66 616c 6c6f 6666  ls_brush_falloff
-003522e0: 5f6e 6f72 6d61 6c27 203d 204e 6f6e 650a  _normal' = None.
-003522f0: 0a56 4945 5733 445f 5054 5f74 6f6f 6c73  .VIEW3D_PT_tools
-00352300: 5f62 7275 7368 5f73 656c 6563 743a 2027  _brush_select: '
-00352310: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
-00352320: 3364 5f74 6f6f 6c62 6172 2e56 4945 5733  3d_toolbar.VIEW3
-00352330: 445f 5054 5f74 6f6f 6c73 5f62 7275 7368  D_PT_tools_brush
-00352340: 5f73 656c 6563 7427 203d 204e 6f6e 650a  _select' = None.
-00352350: 0a56 4945 5733 445f 5054 5f74 6f6f 6c73  .VIEW3D_PT_tools
-00352360: 5f62 7275 7368 5f73 6574 7469 6e67 733a  _brush_settings:
-00352370: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-00352380: 6577 3364 5f74 6f6f 6c62 6172 2e56 4945  ew3d_toolbar.VIE
-00352390: 5733 445f 5054 5f74 6f6f 6c73 5f62 7275  W3D_PT_tools_bru
-003523a0: 7368 5f73 6574 7469 6e67 7327 203d 204e  sh_settings' = N
-003523b0: 6f6e 650a 0a56 4945 5733 445f 5054 5f74  one..VIEW3D_PT_t
-003523c0: 6f6f 6c73 5f62 7275 7368 5f73 6574 7469  ools_brush_setti
-003523d0: 6e67 735f 6164 7661 6e63 6564 3a20 2762  ngs_advanced: 'b
-003523e0: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-003523f0: 645f 746f 6f6c 6261 722e 5649 4557 3344  d_toolbar.VIEW3D
-00352400: 5f50 545f 746f 6f6c 735f 6272 7573 685f  _PT_tools_brush_
-00352410: 7365 7474 696e 6773 5f61 6476 616e 6365  settings_advance
-00352420: 6427 203d 204e 6f6e 650a 0a56 4945 5733  d' = None..VIEW3
-00352430: 445f 5054 5f74 6f6f 6c73 5f62 7275 7368  D_PT_tools_brush
-00352440: 5f73 7472 6f6b 653a 2027 626c 5f75 692e  _stroke: 'bl_ui.
-00352450: 7370 6163 655f 7669 6577 3364 5f74 6f6f  space_view3d_too
-00352460: 6c62 6172 2e56 4945 5733 445f 5054 5f74  lbar.VIEW3D_PT_t
-00352470: 6f6f 6c73 5f62 7275 7368 5f73 7472 6f6b  ools_brush_strok
-00352480: 6527 203d 204e 6f6e 650a 0a56 4945 5733  e' = None..VIEW3
-00352490: 445f 5054 5f74 6f6f 6c73 5f62 7275 7368  D_PT_tools_brush
-003524a0: 5f73 7472 6f6b 655f 736d 6f6f 7468 5f73  _stroke_smooth_s
-003524b0: 7472 6f6b 653a 2027 626c 5f75 692e 7370  troke: 'bl_ui.sp
-003524c0: 6163 655f 7669 6577 3364 5f74 6f6f 6c62  ace_view3d_toolb
-003524d0: 6172 2e56 4945 5733 445f 5054 5f74 6f6f  ar.VIEW3D_PT_too
-003524e0: 6c73 5f62 7275 7368 5f73 7472 6f6b 655f  ls_brush_stroke_
-003524f0: 736d 6f6f 7468 5f73 7472 6f6b 6527 203d  smooth_stroke' =
-00352500: 204e 6f6e 650a 0a56 4945 5733 445f 5054   None..VIEW3D_PT
-00352510: 5f74 6f6f 6c73 5f62 7275 7368 5f73 7761  _tools_brush_swa
-00352520: 7463 6865 733a 2027 626c 5f75 692e 7370  tches: 'bl_ui.sp
-00352530: 6163 655f 7669 6577 3364 5f74 6f6f 6c62  ace_view3d_toolb
-00352540: 6172 2e56 4945 5733 445f 5054 5f74 6f6f  ar.VIEW3D_PT_too
-00352550: 6c73 5f62 7275 7368 5f73 7761 7463 6865  ls_brush_swatche
-00352560: 7327 203d 204e 6f6e 650a 0a56 4945 5733  s' = None..VIEW3
-00352570: 445f 5054 5f74 6f6f 6c73 5f62 7275 7368  D_PT_tools_brush
-00352580: 5f74 6578 7475 7265 3a20 2762 6c5f 7569  _texture: 'bl_ui
-00352590: 2e73 7061 6365 5f76 6965 7733 645f 746f  .space_view3d_to
-003525a0: 6f6c 6261 722e 5649 4557 3344 5f50 545f  olbar.VIEW3D_PT_
-003525b0: 746f 6f6c 735f 6272 7573 685f 7465 7874  tools_brush_text
-003525c0: 7572 6527 203d 204e 6f6e 650a 0a56 4945  ure' = None..VIE
-003525d0: 5733 445f 5054 5f74 6f6f 6c73 5f67 7265  W3D_PT_tools_gre
-003525e0: 6173 655f 7065 6e63 696c 5f62 7275 7368  ase_pencil_brush
-003525f0: 5f61 6476 616e 6365 643a 2027 626c 5f75  _advanced: 'bl_u
-00352600: 692e 7370 6163 655f 7669 6577 3364 5f74  i.space_view3d_t
-00352610: 6f6f 6c62 6172 2e56 4945 5733 445f 5054  oolbar.VIEW3D_PT
-00352620: 5f74 6f6f 6c73 5f67 7265 6173 655f 7065  _tools_grease_pe
-00352630: 6e63 696c 5f62 7275 7368 5f61 6476 616e  ncil_brush_advan
-00352640: 6365 6427 203d 204e 6f6e 650a 0a56 4945  ced' = None..VIE
-00352650: 5733 445f 5054 5f74 6f6f 6c73 5f67 7265  W3D_PT_tools_gre
-00352660: 6173 655f 7065 6e63 696c 5f62 7275 7368  ase_pencil_brush
-00352670: 5f67 6170 5f63 6c6f 7375 7265 3a20 2762  _gap_closure: 'b
-00352680: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-00352690: 645f 746f 6f6c 6261 722e 5649 4557 3344  d_toolbar.VIEW3D
-003526a0: 5f50 545f 746f 6f6c 735f 6772 6561 7365  _PT_tools_grease
-003526b0: 5f70 656e 6369 6c5f 6272 7573 685f 6761  _pencil_brush_ga
-003526c0: 705f 636c 6f73 7572 6527 203d 204e 6f6e  p_closure' = Non
-003526d0: 650a 0a56 4945 5733 445f 5054 5f74 6f6f  e..VIEW3D_PT_too
-003526e0: 6c73 5f67 7265 6173 655f 7065 6e63 696c  ls_grease_pencil
-003526f0: 5f62 7275 7368 5f6d 6978 5f70 616c 6574  _brush_mix_palet
-00352700: 7465 3a20 2762 6c5f 7569 2e73 7061 6365  te: 'bl_ui.space
-00352710: 5f76 6965 7733 645f 746f 6f6c 6261 722e  _view3d_toolbar.
-00352720: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
-00352730: 6772 6561 7365 5f70 656e 6369 6c5f 6272  grease_pencil_br
-00352740: 7573 685f 6d69 785f 7061 6c65 7474 6527  ush_mix_palette'
-00352750: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
-00352760: 5054 5f74 6f6f 6c73 5f67 7265 6173 655f  PT_tools_grease_
-00352770: 7065 6e63 696c 5f62 7275 7368 5f6d 6978  pencil_brush_mix
-00352780: 636f 6c6f 723a 2027 626c 5f75 692e 7370  color: 'bl_ui.sp
-00352790: 6163 655f 7669 6577 3364 5f74 6f6f 6c62  ace_view3d_toolb
-003527a0: 6172 2e56 4945 5733 445f 5054 5f74 6f6f  ar.VIEW3D_PT_too
-003527b0: 6c73 5f67 7265 6173 655f 7065 6e63 696c  ls_grease_pencil
-003527c0: 5f62 7275 7368 5f6d 6978 636f 6c6f 7227  _brush_mixcolor'
-003527d0: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
-003527e0: 5054 5f74 6f6f 6c73 5f67 7265 6173 655f  PT_tools_grease_
-003527f0: 7065 6e63 696c 5f62 7275 7368 5f70 6169  pencil_brush_pai
-00352800: 6e74 5f66 616c 6c6f 6666 3a20 2762 6c5f  nt_falloff: 'bl_
-00352810: 7569 2e73 7061 6365 5f76 6965 7733 645f  ui.space_view3d_
-00352820: 746f 6f6c 6261 722e 5649 4557 3344 5f50  toolbar.VIEW3D_P
-00352830: 545f 746f 6f6c 735f 6772 6561 7365 5f70  T_tools_grease_p
-00352840: 656e 6369 6c5f 6272 7573 685f 7061 696e  encil_brush_pain
-00352850: 745f 6661 6c6c 6f66 6627 203d 204e 6f6e  t_falloff' = Non
-00352860: 650a 0a56 4945 5733 445f 5054 5f74 6f6f  e..VIEW3D_PT_too
-00352870: 6c73 5f67 7265 6173 655f 7065 6e63 696c  ls_grease_pencil
-00352880: 5f62 7275 7368 5f70 6f73 745f 7072 6f63  _brush_post_proc
-00352890: 6573 7369 6e67 3a20 2762 6c5f 7569 2e73  essing: 'bl_ui.s
-003528a0: 7061 6365 5f76 6965 7733 645f 746f 6f6c  pace_view3d_tool
-003528b0: 6261 722e 5649 4557 3344 5f50 545f 746f  bar.VIEW3D_PT_to
-003528c0: 6f6c 735f 6772 6561 7365 5f70 656e 6369  ols_grease_penci
-003528d0: 6c5f 6272 7573 685f 706f 7374 5f70 726f  l_brush_post_pro
-003528e0: 6365 7373 696e 6727 203d 204e 6f6e 650a  cessing' = None.
-003528f0: 0a56 4945 5733 445f 5054 5f74 6f6f 6c73  .VIEW3D_PT_tools
-00352900: 5f67 7265 6173 655f 7065 6e63 696c 5f62  _grease_pencil_b
-00352910: 7275 7368 5f72 616e 646f 6d3a 2027 626c  rush_random: 'bl
-00352920: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
-00352930: 5f74 6f6f 6c62 6172 2e56 4945 5733 445f  _toolbar.VIEW3D_
-00352940: 5054 5f74 6f6f 6c73 5f67 7265 6173 655f  PT_tools_grease_
-00352950: 7065 6e63 696c 5f62 7275 7368 5f72 616e  pencil_brush_ran
-00352960: 646f 6d27 203d 204e 6f6e 650a 0a56 4945  dom' = None..VIE
-00352970: 5733 445f 5054 5f74 6f6f 6c73 5f67 7265  W3D_PT_tools_gre
-00352980: 6173 655f 7065 6e63 696c 5f62 7275 7368  ase_pencil_brush
-00352990: 5f73 6375 6c70 745f 6661 6c6c 6f66 663a  _sculpt_falloff:
-003529a0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-003529b0: 6577 3364 5f74 6f6f 6c62 6172 2e56 4945  ew3d_toolbar.VIE
-003529c0: 5733 445f 5054 5f74 6f6f 6c73 5f67 7265  W3D_PT_tools_gre
-003529d0: 6173 655f 7065 6e63 696c 5f62 7275 7368  ase_pencil_brush
-003529e0: 5f73 6375 6c70 745f 6661 6c6c 6f66 6627  _sculpt_falloff'
-003529f0: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
-00352a00: 5054 5f74 6f6f 6c73 5f67 7265 6173 655f  PT_tools_grease_
-00352a10: 7065 6e63 696c 5f62 7275 7368 5f73 656c  pencil_brush_sel
-00352a20: 6563 743a 2027 626c 5f75 692e 7370 6163  ect: 'bl_ui.spac
-00352a30: 655f 7669 6577 3364 5f74 6f6f 6c62 6172  e_view3d_toolbar
-00352a40: 2e56 4945 5733 445f 5054 5f74 6f6f 6c73  .VIEW3D_PT_tools
-00352a50: 5f67 7265 6173 655f 7065 6e63 696c 5f62  _grease_pencil_b
-00352a60: 7275 7368 5f73 656c 6563 7427 203d 204e  rush_select' = N
-00352a70: 6f6e 650a 0a56 4945 5733 445f 5054 5f74  one..VIEW3D_PT_t
-00352a80: 6f6f 6c73 5f67 7265 6173 655f 7065 6e63  ools_grease_penc
-00352a90: 696c 5f62 7275 7368 5f73 6574 7469 6e67  il_brush_setting
-00352aa0: 733a 2027 626c 5f75 692e 7370 6163 655f  s: 'bl_ui.space_
-00352ab0: 7669 6577 3364 5f74 6f6f 6c62 6172 2e56  view3d_toolbar.V
-00352ac0: 4945 5733 445f 5054 5f74 6f6f 6c73 5f67  IEW3D_PT_tools_g
-00352ad0: 7265 6173 655f 7065 6e63 696c 5f62 7275  rease_pencil_bru
-00352ae0: 7368 5f73 6574 7469 6e67 7327 203d 204e  sh_settings' = N
-00352af0: 6f6e 650a 0a56 4945 5733 445f 5054 5f74  one..VIEW3D_PT_t
-00352b00: 6f6f 6c73 5f67 7265 6173 655f 7065 6e63  ools_grease_penc
-00352b10: 696c 5f62 7275 7368 5f73 7461 6269 6c69  il_brush_stabili
-00352b20: 7a65 723a 2027 626c 5f75 692e 7370 6163  zer: 'bl_ui.spac
-00352b30: 655f 7669 6577 3364 5f74 6f6f 6c62 6172  e_view3d_toolbar
-00352b40: 2e56 4945 5733 445f 5054 5f74 6f6f 6c73  .VIEW3D_PT_tools
-00352b50: 5f67 7265 6173 655f 7065 6e63 696c 5f62  _grease_pencil_b
-00352b60: 7275 7368 5f73 7461 6269 6c69 7a65 7227  rush_stabilizer'
-00352b70: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
-00352b80: 5054 5f74 6f6f 6c73 5f67 7265 6173 655f  PT_tools_grease_
-00352b90: 7065 6e63 696c 5f62 7275 7368 5f73 7472  pencil_brush_str
-00352ba0: 6f6b 653a 2027 626c 5f75 692e 7370 6163  oke: 'bl_ui.spac
-00352bb0: 655f 7669 6577 3364 5f74 6f6f 6c62 6172  e_view3d_toolbar
-00352bc0: 2e56 4945 5733 445f 5054 5f74 6f6f 6c73  .VIEW3D_PT_tools
-00352bd0: 5f67 7265 6173 655f 7065 6e63 696c 5f62  _grease_pencil_b
-00352be0: 7275 7368 5f73 7472 6f6b 6527 203d 204e  rush_stroke' = N
-00352bf0: 6f6e 650a 0a56 4945 5733 445f 5054 5f74  one..VIEW3D_PT_t
-00352c00: 6f6f 6c73 5f67 7265 6173 655f 7065 6e63  ools_grease_penc
-00352c10: 696c 5f62 7275 7368 5f76 6572 7465 785f  il_brush_vertex_
-00352c20: 636f 6c6f 723a 2027 626c 5f75 692e 7370  color: 'bl_ui.sp
-00352c30: 6163 655f 7669 6577 3364 5f74 6f6f 6c62  ace_view3d_toolb
-00352c40: 6172 2e56 4945 5733 445f 5054 5f74 6f6f  ar.VIEW3D_PT_too
-00352c50: 6c73 5f67 7265 6173 655f 7065 6e63 696c  ls_grease_pencil
-00352c60: 5f62 7275 7368 5f76 6572 7465 785f 636f  _brush_vertex_co
-00352c70: 6c6f 7227 203d 204e 6f6e 650a 0a56 4945  lor' = None..VIE
-00352c80: 5733 445f 5054 5f74 6f6f 6c73 5f67 7265  W3D_PT_tools_gre
-00352c90: 6173 655f 7065 6e63 696c 5f62 7275 7368  ase_pencil_brush
-00352ca0: 5f76 6572 7465 785f 6661 6c6c 6f66 663a  _vertex_falloff:
-00352cb0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-00352cc0: 6577 3364 5f74 6f6f 6c62 6172 2e56 4945  ew3d_toolbar.VIE
-00352cd0: 5733 445f 5054 5f74 6f6f 6c73 5f67 7265  W3D_PT_tools_gre
-00352ce0: 6173 655f 7065 6e63 696c 5f62 7275 7368  ase_pencil_brush
-00352cf0: 5f76 6572 7465 785f 6661 6c6c 6f66 6627  _vertex_falloff'
-00352d00: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
-00352d10: 5054 5f74 6f6f 6c73 5f67 7265 6173 655f  PT_tools_grease_
-00352d20: 7065 6e63 696c 5f62 7275 7368 5f76 6572  pencil_brush_ver
-00352d30: 7465 785f 7061 6c65 7474 653a 2027 626c  tex_palette: 'bl
-00352d40: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
-00352d50: 5f74 6f6f 6c62 6172 2e56 4945 5733 445f  _toolbar.VIEW3D_
-00352d60: 5054 5f74 6f6f 6c73 5f67 7265 6173 655f  PT_tools_grease_
-00352d70: 7065 6e63 696c 5f62 7275 7368 5f76 6572  pencil_brush_ver
-00352d80: 7465 785f 7061 6c65 7474 6527 203d 204e  tex_palette' = N
-00352d90: 6f6e 650a 0a56 4945 5733 445f 5054 5f74  one..VIEW3D_PT_t
-00352da0: 6f6f 6c73 5f67 7265 6173 655f 7065 6e63  ools_grease_penc
-00352db0: 696c 5f62 7275 7368 5f77 6569 6768 745f  il_brush_weight_
-00352dc0: 6661 6c6c 6f66 663a 2027 626c 5f75 692e  falloff: 'bl_ui.
-00352dd0: 7370 6163 655f 7669 6577 3364 5f74 6f6f  space_view3d_too
-00352de0: 6c62 6172 2e56 4945 5733 445f 5054 5f74  lbar.VIEW3D_PT_t
-00352df0: 6f6f 6c73 5f67 7265 6173 655f 7065 6e63  ools_grease_penc
-00352e00: 696c 5f62 7275 7368 5f77 6569 6768 745f  il_brush_weight_
-00352e10: 6661 6c6c 6f66 6627 203d 204e 6f6e 650a  falloff' = None.
-00352e20: 0a56 4945 5733 445f 5054 5f74 6f6f 6c73  .VIEW3D_PT_tools
-00352e30: 5f67 7265 6173 655f 7065 6e63 696c 5f70  _grease_pencil_p
-00352e40: 6169 6e74 5f61 7070 6561 7261 6e63 653a  aint_appearance:
-00352e50: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-00352e60: 6577 3364 5f74 6f6f 6c62 6172 2e56 4945  ew3d_toolbar.VIE
-00352e70: 5733 445f 5054 5f74 6f6f 6c73 5f67 7265  W3D_PT_tools_gre
-00352e80: 6173 655f 7065 6e63 696c 5f70 6169 6e74  ase_pencil_paint
-00352e90: 5f61 7070 6561 7261 6e63 6527 203d 204e  _appearance' = N
-00352ea0: 6f6e 650a 0a56 4945 5733 445f 5054 5f74  one..VIEW3D_PT_t
-00352eb0: 6f6f 6c73 5f67 7265 6173 655f 7065 6e63  ools_grease_penc
-00352ec0: 696c 5f73 6375 6c70 745f 6170 7065 6172  il_sculpt_appear
-00352ed0: 616e 6365 3a20 2762 6c5f 7569 2e73 7061  ance: 'bl_ui.spa
-00352ee0: 6365 5f76 6965 7733 645f 746f 6f6c 6261  ce_view3d_toolba
-00352ef0: 722e 5649 4557 3344 5f50 545f 746f 6f6c  r.VIEW3D_PT_tool
-00352f00: 735f 6772 6561 7365 5f70 656e 6369 6c5f  s_grease_pencil_
-00352f10: 7363 756c 7074 5f61 7070 6561 7261 6e63  sculpt_appearanc
-00352f20: 6527 203d 204e 6f6e 650a 0a56 4945 5733  e' = None..VIEW3
-00352f30: 445f 5054 5f74 6f6f 6c73 5f67 7265 6173  D_PT_tools_greas
-00352f40: 655f 7065 6e63 696c 5f73 6375 6c70 745f  e_pencil_sculpt_
-00352f50: 6272 7573 685f 6164 7661 6e63 6564 3a20  brush_advanced: 
-00352f60: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-00352f70: 7733 645f 746f 6f6c 6261 722e 5649 4557  w3d_toolbar.VIEW
-00352f80: 3344 5f50 545f 746f 6f6c 735f 6772 6561  3D_PT_tools_grea
-00352f90: 7365 5f70 656e 6369 6c5f 7363 756c 7074  se_pencil_sculpt
-00352fa0: 5f62 7275 7368 5f61 6476 616e 6365 6427  _brush_advanced'
-00352fb0: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
-00352fc0: 5054 5f74 6f6f 6c73 5f67 7265 6173 655f  PT_tools_grease_
-00352fd0: 7065 6e63 696c 5f73 6375 6c70 745f 6272  pencil_sculpt_br
-00352fe0: 7573 685f 706f 706f 7665 723a 2027 626c  ush_popover: 'bl
-00352ff0: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
-00353000: 5f74 6f6f 6c62 6172 2e56 4945 5733 445f  _toolbar.VIEW3D_
-00353010: 5054 5f74 6f6f 6c73 5f67 7265 6173 655f  PT_tools_grease_
-00353020: 7065 6e63 696c 5f73 6375 6c70 745f 6272  pencil_sculpt_br
-00353030: 7573 685f 706f 706f 7665 7227 203d 204e  ush_popover' = N
-00353040: 6f6e 650a 0a56 4945 5733 445f 5054 5f74  one..VIEW3D_PT_t
-00353050: 6f6f 6c73 5f67 7265 6173 655f 7065 6e63  ools_grease_penc
-00353060: 696c 5f73 6375 6c70 745f 7365 6c65 6374  il_sculpt_select
-00353070: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
-00353080: 6965 7733 645f 746f 6f6c 6261 722e 5649  iew3d_toolbar.VI
-00353090: 4557 3344 5f50 545f 746f 6f6c 735f 6772  EW3D_PT_tools_gr
-003530a0: 6561 7365 5f70 656e 6369 6c5f 7363 756c  ease_pencil_scul
-003530b0: 7074 5f73 656c 6563 7427 203d 204e 6f6e  pt_select' = Non
-003530c0: 650a 0a56 4945 5733 445f 5054 5f74 6f6f  e..VIEW3D_PT_too
-003530d0: 6c73 5f67 7265 6173 655f 7065 6e63 696c  ls_grease_pencil
-003530e0: 5f73 6375 6c70 745f 7365 7474 696e 6773  _sculpt_settings
-003530f0: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
-00353100: 6965 7733 645f 746f 6f6c 6261 722e 5649  iew3d_toolbar.VI
-00353110: 4557 3344 5f50 545f 746f 6f6c 735f 6772  EW3D_PT_tools_gr
-00353120: 6561 7365 5f70 656e 6369 6c5f 7363 756c  ease_pencil_scul
-00353130: 7074 5f73 6574 7469 6e67 7327 203d 204e  pt_settings' = N
-00353140: 6f6e 650a 0a56 4945 5733 445f 5054 5f74  one..VIEW3D_PT_t
-00353150: 6f6f 6c73 5f67 7265 6173 655f 7065 6e63  ools_grease_penc
-00353160: 696c 5f76 6572 7465 785f 6170 7065 6172  il_vertex_appear
-00353170: 616e 6365 3a20 2762 6c5f 7569 2e73 7061  ance: 'bl_ui.spa
-00353180: 6365 5f76 6965 7733 645f 746f 6f6c 6261  ce_view3d_toolba
-00353190: 722e 5649 4557 3344 5f50 545f 746f 6f6c  r.VIEW3D_PT_tool
-003531a0: 735f 6772 6561 7365 5f70 656e 6369 6c5f  s_grease_pencil_
-003531b0: 7665 7274 6578 5f61 7070 6561 7261 6e63  vertex_appearanc
-003531c0: 6527 203d 204e 6f6e 650a 0a56 4945 5733  e' = None..VIEW3
-003531d0: 445f 5054 5f74 6f6f 6c73 5f67 7265 6173  D_PT_tools_greas
-003531e0: 655f 7065 6e63 696c 5f76 6572 7465 785f  e_pencil_vertex_
-003531f0: 7061 696e 745f 7365 6c65 6374 3a20 2762  paint_select: 'b
-00353200: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-00353210: 645f 746f 6f6c 6261 722e 5649 4557 3344  d_toolbar.VIEW3D
-00353220: 5f50 545f 746f 6f6c 735f 6772 6561 7365  _PT_tools_grease
-00353230: 5f70 656e 6369 6c5f 7665 7274 6578 5f70  _pencil_vertex_p
-00353240: 6169 6e74 5f73 656c 6563 7427 203d 204e  aint_select' = N
-00353250: 6f6e 650a 0a56 4945 5733 445f 5054 5f74  one..VIEW3D_PT_t
-00353260: 6f6f 6c73 5f67 7265 6173 655f 7065 6e63  ools_grease_penc
-00353270: 696c 5f76 6572 7465 785f 7061 696e 745f  il_vertex_paint_
-00353280: 7365 7474 696e 6773 3a20 2762 6c5f 7569  settings: 'bl_ui
-00353290: 2e73 7061 6365 5f76 6965 7733 645f 746f  .space_view3d_to
-003532a0: 6f6c 6261 722e 5649 4557 3344 5f50 545f  olbar.VIEW3D_PT_
-003532b0: 746f 6f6c 735f 6772 6561 7365 5f70 656e  tools_grease_pen
-003532c0: 6369 6c5f 7665 7274 6578 5f70 6169 6e74  cil_vertex_paint
-003532d0: 5f73 6574 7469 6e67 7327 203d 204e 6f6e  _settings' = Non
-003532e0: 650a 0a56 4945 5733 445f 5054 5f74 6f6f  e..VIEW3D_PT_too
-003532f0: 6c73 5f67 7265 6173 655f 7065 6e63 696c  ls_grease_pencil
-00353300: 5f77 6569 6768 745f 6170 7065 6172 616e  _weight_appearan
-00353310: 6365 3a20 2762 6c5f 7569 2e73 7061 6365  ce: 'bl_ui.space
-00353320: 5f76 6965 7733 645f 746f 6f6c 6261 722e  _view3d_toolbar.
-00353330: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
-00353340: 6772 6561 7365 5f70 656e 6369 6c5f 7765  grease_pencil_we
-00353350: 6967 6874 5f61 7070 6561 7261 6e63 6527  ight_appearance'
-00353360: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
-00353370: 5054 5f74 6f6f 6c73 5f67 7265 6173 655f  PT_tools_grease_
-00353380: 7065 6e63 696c 5f77 6569 6768 745f 6f70  pencil_weight_op
-00353390: 7469 6f6e 733a 2027 626c 5f75 692e 7370  tions: 'bl_ui.sp
-003533a0: 6163 655f 7669 6577 3364 5f74 6f6f 6c62  ace_view3d_toolb
-003533b0: 6172 2e56 4945 5733 445f 5054 5f74 6f6f  ar.VIEW3D_PT_too
-003533c0: 6c73 5f67 7265 6173 655f 7065 6e63 696c  ls_grease_pencil
-003533d0: 5f77 6569 6768 745f 6f70 7469 6f6e 7327  _weight_options'
-003533e0: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
-003533f0: 5054 5f74 6f6f 6c73 5f67 7265 6173 655f  PT_tools_grease_
-00353400: 7065 6e63 696c 5f77 6569 6768 745f 7061  pencil_weight_pa
-00353410: 696e 745f 7365 6c65 6374 3a20 2762 6c5f  int_select: 'bl_
-00353420: 7569 2e73 7061 6365 5f76 6965 7733 645f  ui.space_view3d_
-00353430: 746f 6f6c 6261 722e 5649 4557 3344 5f50  toolbar.VIEW3D_P
-00353440: 545f 746f 6f6c 735f 6772 6561 7365 5f70  T_tools_grease_p
-00353450: 656e 6369 6c5f 7765 6967 6874 5f70 6169  encil_weight_pai
-00353460: 6e74 5f73 656c 6563 7427 203d 204e 6f6e  nt_select' = Non
-00353470: 650a 0a56 4945 5733 445f 5054 5f74 6f6f  e..VIEW3D_PT_too
-00353480: 6c73 5f67 7265 6173 655f 7065 6e63 696c  ls_grease_pencil
-00353490: 5f77 6569 6768 745f 7061 696e 745f 7365  _weight_paint_se
-003534a0: 7474 696e 6773 3a20 2762 6c5f 7569 2e73  ttings: 'bl_ui.s
-003534b0: 7061 6365 5f76 6965 7733 645f 746f 6f6c  pace_view3d_tool
-003534c0: 6261 722e 5649 4557 3344 5f50 545f 746f  bar.VIEW3D_PT_to
-003534d0: 6f6c 735f 6772 6561 7365 5f70 656e 6369  ols_grease_penci
-003534e0: 6c5f 7765 6967 6874 5f70 6169 6e74 5f73  l_weight_paint_s
-003534f0: 6574 7469 6e67 7327 203d 204e 6f6e 650a  ettings' = None.
-00353500: 0a56 4945 5733 445f 5054 5f74 6f6f 6c73  .VIEW3D_PT_tools
-00353510: 5f69 6d61 6765 7061 696e 745f 6f70 7469  _imagepaint_opti
-00353520: 6f6e 733a 2027 626c 5f75 692e 7370 6163  ons: 'bl_ui.spac
-00353530: 655f 7669 6577 3364 5f74 6f6f 6c62 6172  e_view3d_toolbar
-00353540: 2e56 4945 5733 445f 5054 5f74 6f6f 6c73  .VIEW3D_PT_tools
-00353550: 5f69 6d61 6765 7061 696e 745f 6f70 7469  _imagepaint_opti
-00353560: 6f6e 7327 203d 204e 6f6e 650a 0a56 4945  ons' = None..VIE
-00353570: 5733 445f 5054 5f74 6f6f 6c73 5f69 6d61  W3D_PT_tools_ima
-00353580: 6765 7061 696e 745f 6f70 7469 6f6e 735f  gepaint_options_
-00353590: 6361 7669 7479 3a20 2762 6c5f 7569 2e73  cavity: 'bl_ui.s
-003535a0: 7061 6365 5f76 6965 7733 645f 746f 6f6c  pace_view3d_tool
-003535b0: 6261 722e 5649 4557 3344 5f50 545f 746f  bar.VIEW3D_PT_to
-003535c0: 6f6c 735f 696d 6167 6570 6169 6e74 5f6f  ols_imagepaint_o
-003535d0: 7074 696f 6e73 5f63 6176 6974 7927 203d  ptions_cavity' =
-003535e0: 204e 6f6e 650a 0a56 4945 5733 445f 5054   None..VIEW3D_PT
-003535f0: 5f74 6f6f 6c73 5f69 6d61 6765 7061 696e  _tools_imagepain
-00353600: 745f 6f70 7469 6f6e 735f 6578 7465 726e  t_options_extern
-00353610: 616c 3a20 2762 6c5f 7569 2e73 7061 6365  al: 'bl_ui.space
-00353620: 5f76 6965 7733 645f 746f 6f6c 6261 722e  _view3d_toolbar.
-00353630: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
-00353640: 696d 6167 6570 6169 6e74 5f6f 7074 696f  imagepaint_optio
-00353650: 6e73 5f65 7874 6572 6e61 6c27 203d 204e  ns_external' = N
-00353660: 6f6e 650a 0a56 4945 5733 445f 5054 5f74  one..VIEW3D_PT_t
-00353670: 6f6f 6c73 5f69 6d61 6765 7061 696e 745f  ools_imagepaint_
-00353680: 7379 6d6d 6574 7279 3a20 2762 6c5f 7569  symmetry: 'bl_ui
-00353690: 2e73 7061 6365 5f76 6965 7733 645f 746f  .space_view3d_to
-003536a0: 6f6c 6261 722e 5649 4557 3344 5f50 545f  olbar.VIEW3D_PT_
-003536b0: 746f 6f6c 735f 696d 6167 6570 6169 6e74  tools_imagepaint
-003536c0: 5f73 796d 6d65 7472 7927 203d 204e 6f6e  _symmetry' = Non
-003536d0: 650a 0a56 4945 5733 445f 5054 5f74 6f6f  e..VIEW3D_PT_too
-003536e0: 6c73 5f6d 6173 6b5f 7465 7874 7572 653a  ls_mask_texture:
-003536f0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-00353700: 6577 3364 5f74 6f6f 6c62 6172 2e56 4945  ew3d_toolbar.VIE
-00353710: 5733 445f 5054 5f74 6f6f 6c73 5f6d 6173  W3D_PT_tools_mas
-00353720: 6b5f 7465 7874 7572 6527 203d 204e 6f6e  k_texture' = Non
-00353730: 650a 0a56 4945 5733 445f 5054 5f74 6f6f  e..VIEW3D_PT_too
-00353740: 6c73 5f6d 6573 6865 6469 745f 6f70 7469  ls_meshedit_opti
-00353750: 6f6e 733a 2027 626c 5f75 692e 7370 6163  ons: 'bl_ui.spac
-00353760: 655f 7669 6577 3364 5f74 6f6f 6c62 6172  e_view3d_toolbar
-00353770: 2e56 4945 5733 445f 5054 5f74 6f6f 6c73  .VIEW3D_PT_tools
-00353780: 5f6d 6573 6865 6469 745f 6f70 7469 6f6e  _meshedit_option
-00353790: 7327 203d 204e 6f6e 650a 0a56 4945 5733  s' = None..VIEW3
-003537a0: 445f 5054 5f74 6f6f 6c73 5f6d 6573 6865  D_PT_tools_meshe
-003537b0: 6469 745f 6f70 7469 6f6e 735f 7472 616e  dit_options_tran
-003537c0: 7366 6f72 6d3a 2027 626c 5f75 692e 7370  sform: 'bl_ui.sp
-003537d0: 6163 655f 7669 6577 3364 5f74 6f6f 6c62  ace_view3d_toolb
-003537e0: 6172 2e56 4945 5733 445f 5054 5f74 6f6f  ar.VIEW3D_PT_too
-003537f0: 6c73 5f6d 6573 6865 6469 745f 6f70 7469  ls_meshedit_opti
-00353800: 6f6e 735f 7472 616e 7366 6f72 6d27 203d  ons_transform' =
-00353810: 204e 6f6e 650a 0a56 4945 5733 445f 5054   None..VIEW3D_PT
-00353820: 5f74 6f6f 6c73 5f6d 6573 6865 6469 745f  _tools_meshedit_
-00353830: 6f70 7469 6f6e 735f 7576 733a 2027 626c  options_uvs: 'bl
-00353840: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
-00353850: 5f74 6f6f 6c62 6172 2e56 4945 5733 445f  _toolbar.VIEW3D_
-00353860: 5054 5f74 6f6f 6c73 5f6d 6573 6865 6469  PT_tools_meshedi
-00353870: 745f 6f70 7469 6f6e 735f 7576 7327 203d  t_options_uvs' =
-00353880: 204e 6f6e 650a 0a56 4945 5733 445f 5054   None..VIEW3D_PT
-00353890: 5f74 6f6f 6c73 5f6f 626a 6563 745f 6f70  _tools_object_op
-003538a0: 7469 6f6e 733a 2027 626c 5f75 692e 7370  tions: 'bl_ui.sp
-003538b0: 6163 655f 7669 6577 3364 5f74 6f6f 6c62  ace_view3d_toolb
-003538c0: 6172 2e56 4945 5733 445f 5054 5f74 6f6f  ar.VIEW3D_PT_too
-003538d0: 6c73 5f6f 626a 6563 745f 6f70 7469 6f6e  ls_object_option
-003538e0: 7327 203d 204e 6f6e 650a 0a56 4945 5733  s' = None..VIEW3
-003538f0: 445f 5054 5f74 6f6f 6c73 5f6f 626a 6563  D_PT_tools_objec
-00353900: 745f 6f70 7469 6f6e 735f 7472 616e 7366  t_options_transf
-00353910: 6f72 6d3a 2027 626c 5f75 692e 7370 6163  orm: 'bl_ui.spac
-00353920: 655f 7669 6577 3364 5f74 6f6f 6c62 6172  e_view3d_toolbar
-00353930: 2e56 4945 5733 445f 5054 5f74 6f6f 6c73  .VIEW3D_PT_tools
-00353940: 5f6f 626a 6563 745f 6f70 7469 6f6e 735f  _object_options_
-00353950: 7472 616e 7366 6f72 6d27 203d 204e 6f6e  transform' = Non
-00353960: 650a 0a56 4945 5733 445f 5054 5f74 6f6f  e..VIEW3D_PT_too
-00353970: 6c73 5f70 6172 7469 636c 656d 6f64 653a  ls_particlemode:
-00353980: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-00353990: 6577 3364 5f74 6f6f 6c62 6172 2e56 4945  ew3d_toolbar.VIE
-003539a0: 5733 445f 5054 5f74 6f6f 6c73 5f70 6172  W3D_PT_tools_par
-003539b0: 7469 636c 656d 6f64 6527 203d 204e 6f6e  ticlemode' = Non
-003539c0: 650a 0a56 4945 5733 445f 5054 5f74 6f6f  e..VIEW3D_PT_too
-003539d0: 6c73 5f70 6172 7469 636c 656d 6f64 655f  ls_particlemode_
-003539e0: 6f70 7469 6f6e 733a 2027 626c 5f75 692e  options: 'bl_ui.
-003539f0: 7370 6163 655f 7669 6577 3364 5f74 6f6f  space_view3d_too
-00353a00: 6c62 6172 2e56 4945 5733 445f 5054 5f74  lbar.VIEW3D_PT_t
-00353a10: 6f6f 6c73 5f70 6172 7469 636c 656d 6f64  ools_particlemod
-00353a20: 655f 6f70 7469 6f6e 7327 203d 204e 6f6e  e_options' = Non
-00353a30: 650a 0a56 4945 5733 445f 5054 5f74 6f6f  e..VIEW3D_PT_too
-00353a40: 6c73 5f70 6172 7469 636c 656d 6f64 655f  ls_particlemode_
-00353a50: 6f70 7469 6f6e 735f 6469 7370 6c61 793a  options_display:
-00353a60: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-00353a70: 6577 3364 5f74 6f6f 6c62 6172 2e56 4945  ew3d_toolbar.VIE
-00353a80: 5733 445f 5054 5f74 6f6f 6c73 5f70 6172  W3D_PT_tools_par
-00353a90: 7469 636c 656d 6f64 655f 6f70 7469 6f6e  ticlemode_option
-00353aa0: 735f 6469 7370 6c61 7927 203d 204e 6f6e  s_display' = Non
-00353ab0: 650a 0a56 4945 5733 445f 5054 5f74 6f6f  e..VIEW3D_PT_too
-00353ac0: 6c73 5f70 6172 7469 636c 656d 6f64 655f  ls_particlemode_
-00353ad0: 6f70 7469 6f6e 735f 7368 6170 6563 7574  options_shapecut
-00353ae0: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
-00353af0: 6965 7733 645f 746f 6f6c 6261 722e 5649  iew3d_toolbar.VI
-00353b00: 4557 3344 5f50 545f 746f 6f6c 735f 7061  EW3D_PT_tools_pa
-00353b10: 7274 6963 6c65 6d6f 6465 5f6f 7074 696f  rticlemode_optio
-00353b20: 6e73 5f73 6861 7065 6375 7427 203d 204e  ns_shapecut' = N
-00353b30: 6f6e 650a 0a56 4945 5733 445f 5054 5f74  one..VIEW3D_PT_t
-00353b40: 6f6f 6c73 5f70 6f73 656d 6f64 655f 6f70  ools_posemode_op
-00353b50: 7469 6f6e 733a 2027 626c 5f75 692e 7370  tions: 'bl_ui.sp
-00353b60: 6163 655f 7669 6577 3364 5f74 6f6f 6c62  ace_view3d_toolb
-00353b70: 6172 2e56 4945 5733 445f 5054 5f74 6f6f  ar.VIEW3D_PT_too
-00353b80: 6c73 5f70 6f73 656d 6f64 655f 6f70 7469  ls_posemode_opti
-00353b90: 6f6e 7327 203d 204e 6f6e 650a 0a56 4945  ons' = None..VIE
-00353ba0: 5733 445f 5054 5f74 6f6f 6c73 5f76 6572  W3D_PT_tools_ver
-00353bb0: 7465 7870 6169 6e74 5f6f 7074 696f 6e73  texpaint_options
-00353bc0: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
-00353bd0: 6965 7733 645f 746f 6f6c 6261 722e 5649  iew3d_toolbar.VI
-00353be0: 4557 3344 5f50 545f 746f 6f6c 735f 7665  EW3D_PT_tools_ve
-00353bf0: 7274 6578 7061 696e 745f 6f70 7469 6f6e  rtexpaint_option
-00353c00: 7327 203d 204e 6f6e 650a 0a56 4945 5733  s' = None..VIEW3
-00353c10: 445f 5054 5f74 6f6f 6c73 5f76 6572 7465  D_PT_tools_verte
-00353c20: 7870 6169 6e74 5f73 796d 6d65 7472 793a  xpaint_symmetry:
-00353c30: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-00353c40: 6577 3364 5f74 6f6f 6c62 6172 2e56 4945  ew3d_toolbar.VIE
-00353c50: 5733 445f 5054 5f74 6f6f 6c73 5f76 6572  W3D_PT_tools_ver
-00353c60: 7465 7870 6169 6e74 5f73 796d 6d65 7472  texpaint_symmetr
-00353c70: 7927 203d 204e 6f6e 650a 0a56 4945 5733  y' = None..VIEW3
-00353c80: 445f 5054 5f74 6f6f 6c73 5f76 6572 7465  D_PT_tools_verte
-00353c90: 7870 6169 6e74 5f73 796d 6d65 7472 795f  xpaint_symmetry_
-00353ca0: 666f 725f 746f 7062 6172 3a20 2762 6c5f  for_topbar: 'bl_
-00353cb0: 7569 2e73 7061 6365 5f76 6965 7733 645f  ui.space_view3d_
-00353cc0: 746f 6f6c 6261 722e 5649 4557 3344 5f50  toolbar.VIEW3D_P
-00353cd0: 545f 746f 6f6c 735f 7665 7274 6578 7061  T_tools_vertexpa
-00353ce0: 696e 745f 7379 6d6d 6574 7279 5f66 6f72  int_symmetry_for
-00353cf0: 5f74 6f70 6261 7227 203d 204e 6f6e 650a  _topbar' = None.
-00353d00: 0a56 4945 5733 445f 5054 5f74 6f6f 6c73  .VIEW3D_PT_tools
-00353d10: 5f77 6569 6768 745f 6772 6164 6965 6e74  _weight_gradient
-00353d20: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
-00353d30: 6965 7733 645f 746f 6f6c 6261 722e 5649  iew3d_toolbar.VI
-00353d40: 4557 3344 5f50 545f 746f 6f6c 735f 7765  EW3D_PT_tools_we
-00353d50: 6967 6874 5f67 7261 6469 656e 7427 203d  ight_gradient' =
-00353d60: 204e 6f6e 650a 0a56 4945 5733 445f 5054   None..VIEW3D_PT
-00353d70: 5f74 6f6f 6c73 5f77 6569 6768 7470 6169  _tools_weightpai
-00353d80: 6e74 5f6f 7074 696f 6e73 3a20 2762 6c5f  nt_options: 'bl_
-00353d90: 7569 2e73 7061 6365 5f76 6965 7733 645f  ui.space_view3d_
-00353da0: 746f 6f6c 6261 722e 5649 4557 3344 5f50  toolbar.VIEW3D_P
-00353db0: 545f 746f 6f6c 735f 7765 6967 6874 7061  T_tools_weightpa
-00353dc0: 696e 745f 6f70 7469 6f6e 7327 203d 204e  int_options' = N
-00353dd0: 6f6e 650a 0a56 4945 5733 445f 5054 5f74  one..VIEW3D_PT_t
-00353de0: 6f6f 6c73 5f77 6569 6768 7470 6169 6e74  ools_weightpaint
-00353df0: 5f73 796d 6d65 7472 793a 2027 626c 5f75  _symmetry: 'bl_u
-00353e00: 692e 7370 6163 655f 7669 6577 3364 5f74  i.space_view3d_t
-00353e10: 6f6f 6c62 6172 2e56 4945 5733 445f 5054  oolbar.VIEW3D_PT
-00353e20: 5f74 6f6f 6c73 5f77 6569 6768 7470 6169  _tools_weightpai
-00353e30: 6e74 5f73 796d 6d65 7472 7927 203d 204e  nt_symmetry' = N
-00353e40: 6f6e 650a 0a56 4945 5733 445f 5054 5f74  one..VIEW3D_PT_t
-00353e50: 6f6f 6c73 5f77 6569 6768 7470 6169 6e74  ools_weightpaint
-00353e60: 5f73 796d 6d65 7472 795f 666f 725f 746f  _symmetry_for_to
-00353e70: 7062 6172 3a20 2762 6c5f 7569 2e73 7061  pbar: 'bl_ui.spa
-00353e80: 6365 5f76 6965 7733 645f 746f 6f6c 6261  ce_view3d_toolba
-00353e90: 722e 5649 4557 3344 5f50 545f 746f 6f6c  r.VIEW3D_PT_tool
-00353ea0: 735f 7765 6967 6874 7061 696e 745f 7379  s_weightpaint_sy
-00353eb0: 6d6d 6574 7279 5f66 6f72 5f74 6f70 6261  mmetry_for_topba
-00353ec0: 7227 203d 204e 6f6e 650a 0a56 4945 5733  r' = None..VIEW3
-00353ed0: 445f 5054 5f74 7261 6e73 666f 726d 5f6f  D_PT_transform_o
-00353ee0: 7269 656e 7461 7469 6f6e 733a 2027 626c  rientations: 'bl
-00353ef0: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
-00353f00: 2e56 4945 5733 445f 5054 5f74 7261 6e73  .VIEW3D_PT_trans
-00353f10: 666f 726d 5f6f 7269 656e 7461 7469 6f6e  form_orientation
-00353f20: 7327 203d 204e 6f6e 650a 0a56 4945 5733  s' = None..VIEW3
-00353f30: 445f 5054 5f76 6965 7733 645f 6375 7273  D_PT_view3d_curs
-00353f40: 6f72 3a20 2762 6c5f 7569 2e73 7061 6365  or: 'bl_ui.space
-00353f50: 5f76 6965 7733 642e 5649 4557 3344 5f50  _view3d.VIEW3D_P
-00353f60: 545f 7669 6577 3364 5f63 7572 736f 7227  T_view3d_cursor'
-00353f70: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
-00353f80: 5054 5f76 6965 7733 645f 6c6f 636b 3a20  PT_view3d_lock: 
-00353f90: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-00353fa0: 7733 642e 5649 4557 3344 5f50 545f 7669  w3d.VIEW3D_PT_vi
-00353fb0: 6577 3364 5f6c 6f63 6b27 203d 204e 6f6e  ew3d_lock' = Non
-00353fc0: 650a 0a56 4945 5733 445f 5054 5f76 6965  e..VIEW3D_PT_vie
-00353fd0: 7733 645f 7072 6f70 6572 7469 6573 3a20  w3d_properties: 
-00353fe0: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-00353ff0: 7733 642e 5649 4557 3344 5f50 545f 7669  w3d.VIEW3D_PT_vi
-00354000: 6577 3364 5f70 726f 7065 7274 6965 7327  ew3d_properties'
-00354010: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
-00354020: 5054 5f76 6965 7733 645f 7374 6572 656f  PT_view3d_stereo
-00354030: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
-00354040: 6965 7733 642e 5649 4557 3344 5f50 545f  iew3d.VIEW3D_PT_
-00354050: 7669 6577 3364 5f73 7465 7265 6f27 203d  view3d_stereo' =
-00354060: 204e 6f6e 650a 0a56 4945 5733 445f 5054   None..VIEW3D_PT
-00354070: 5f76 6965 7770 6f72 745f 6465 6275 673a  _viewport_debug:
-00354080: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-00354090: 6577 3364 2e56 4945 5733 445f 5054 5f76  ew3d.VIEW3D_PT_v
-003540a0: 6965 7770 6f72 745f 6465 6275 6727 203d  iewport_debug' =
-003540b0: 204e 6f6e 650a 0a56 4945 574c 4159 4552   None..VIEWLAYER
-003540c0: 5f4d 545f 6c69 6768 7467 726f 7570 5f73  _MT_lightgroup_s
-003540d0: 796e 633a 2027 626c 5f75 692e 7072 6f70  ync: 'bl_ui.prop
-003540e0: 6572 7469 6573 5f76 6965 775f 6c61 7965  erties_view_laye
-003540f0: 722e 5649 4557 4c41 5945 525f 4d54 5f6c  r.VIEWLAYER_MT_l
-00354100: 6967 6874 6772 6f75 705f 7379 6e63 2720  ightgroup_sync' 
-00354110: 3d20 4e6f 6e65 0a0a 5649 4557 4c41 5945  = None..VIEWLAYE
-00354120: 525f 5054 5f65 6576 6565 5f6c 6179 6572  R_PT_eevee_layer
-00354130: 5f70 6173 7365 735f 6461 7461 3a20 2762  _passes_data: 'b
-00354140: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
-00354150: 7669 6577 5f6c 6179 6572 2e56 4945 574c  view_layer.VIEWL
-00354160: 4159 4552 5f50 545f 6565 7665 655f 6c61  AYER_PT_eevee_la
-00354170: 7965 725f 7061 7373 6573 5f64 6174 6127  yer_passes_data'
-00354180: 203d 204e 6f6e 650a 0a56 4945 574c 4159   = None..VIEWLAY
-00354190: 4552 5f50 545f 6565 7665 655f 6c61 7965  ER_PT_eevee_laye
-003541a0: 725f 7061 7373 6573 5f65 6666 6563 7473  r_passes_effects
-003541b0: 3a20 2762 6c5f 7569 2e70 726f 7065 7274  : 'bl_ui.propert
-003541c0: 6965 735f 7669 6577 5f6c 6179 6572 2e56  ies_view_layer.V
-003541d0: 4945 574c 4159 4552 5f50 545f 6565 7665  IEWLAYER_PT_eeve
-003541e0: 655f 6c61 7965 725f 7061 7373 6573 5f65  e_layer_passes_e
-003541f0: 6666 6563 7473 2720 3d20 4e6f 6e65 0a0a  ffects' = None..
-00354200: 5649 4557 4c41 5945 525f 5054 5f65 6576  VIEWLAYER_PT_eev
-00354210: 6565 5f6c 6179 6572 5f70 6173 7365 735f  ee_layer_passes_
-00354220: 6c69 6768 743a 2027 626c 5f75 692e 7072  light: 'bl_ui.pr
-00354230: 6f70 6572 7469 6573 5f76 6965 775f 6c61  operties_view_la
-00354240: 7965 722e 5649 4557 4c41 5945 525f 5054  yer.VIEWLAYER_PT
-00354250: 5f65 6576 6565 5f6c 6179 6572 5f70 6173  _eevee_layer_pas
-00354260: 7365 735f 6c69 6768 7427 203d 204e 6f6e  ses_light' = Non
-00354270: 650a 0a56 4945 574c 4159 4552 5f50 545f  e..VIEWLAYER_PT_
-00354280: 6565 7665 655f 6e65 7874 5f6c 6179 6572  eevee_next_layer
-00354290: 5f70 6173 7365 735f 6461 7461 3a20 2762  _passes_data: 'b
-003542a0: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
-003542b0: 7669 6577 5f6c 6179 6572 2e56 4945 574c  view_layer.VIEWL
-003542c0: 4159 4552 5f50 545f 6565 7665 655f 6e65  AYER_PT_eevee_ne
-003542d0: 7874 5f6c 6179 6572 5f70 6173 7365 735f  xt_layer_passes_
-003542e0: 6461 7461 2720 3d20 4e6f 6e65 0a0a 5649  data' = None..VI
-003542f0: 4557 4c41 5945 525f 5054 5f66 7265 6573  EWLAYER_PT_frees
-00354300: 7479 6c65 3a20 2762 6c5f 7569 2e70 726f  tyle: 'bl_ui.pro
-00354310: 7065 7274 6965 735f 6672 6565 7374 796c  perties_freestyl
-00354320: 652e 5649 4557 4c41 5945 525f 5054 5f66  e.VIEWLAYER_PT_f
-00354330: 7265 6573 7479 6c65 2720 3d20 4e6f 6e65  reestyle' = None
-00354340: 0a0a 5649 4557 4c41 5945 525f 5054 5f66  ..VIEWLAYER_PT_f
-00354350: 7265 6573 7479 6c65 5f65 6467 655f 6465  reestyle_edge_de
-00354360: 7465 6374 696f 6e3a 2027 626c 5f75 692e  tection: 'bl_ui.
-00354370: 7072 6f70 6572 7469 6573 5f66 7265 6573  properties_frees
-00354380: 7479 6c65 2e56 4945 574c 4159 4552 5f50  tyle.VIEWLAYER_P
-00354390: 545f 6672 6565 7374 796c 655f 6564 6765  T_freestyle_edge
-003543a0: 5f64 6574 6563 7469 6f6e 2720 3d20 4e6f  _detection' = No
-003543b0: 6e65 0a0a 5649 4557 4c41 5945 525f 5054  ne..VIEWLAYER_PT
-003543c0: 5f66 7265 6573 7479 6c65 5f6c 696e 6573  _freestyle_lines
-003543d0: 6574 3a20 2762 6c5f 7569 2e70 726f 7065  et: 'bl_ui.prope
-003543e0: 7274 6965 735f 6672 6565 7374 796c 652e  rties_freestyle.
-003543f0: 5649 4557 4c41 5945 525f 5054 5f66 7265  VIEWLAYER_PT_fre
-00354400: 6573 7479 6c65 5f6c 696e 6573 6574 2720  estyle_lineset' 
-00354410: 3d20 4e6f 6e65 0a0a 5649 4557 4c41 5945  = None..VIEWLAYE
-00354420: 525f 5054 5f66 7265 6573 7479 6c65 5f6c  R_PT_freestyle_l
-00354430: 696e 6573 6574 5f63 6f6c 6c65 6374 696f  ineset_collectio
-00354440: 6e3a 2027 626c 5f75 692e 7072 6f70 6572  n: 'bl_ui.proper
-00354450: 7469 6573 5f66 7265 6573 7479 6c65 2e56  ties_freestyle.V
-00354460: 4945 574c 4159 4552 5f50 545f 6672 6565  IEWLAYER_PT_free
-00354470: 7374 796c 655f 6c69 6e65 7365 745f 636f  style_lineset_co
-00354480: 6c6c 6563 7469 6f6e 2720 3d20 4e6f 6e65  llection' = None
-00354490: 0a0a 5649 4557 4c41 5945 525f 5054 5f66  ..VIEWLAYER_PT_f
-003544a0: 7265 6573 7479 6c65 5f6c 696e 6573 6574  reestyle_lineset
-003544b0: 5f65 6467 6574 7970 653a 2027 626c 5f75  _edgetype: 'bl_u
-003544c0: 692e 7072 6f70 6572 7469 6573 5f66 7265  i.properties_fre
-003544d0: 6573 7479 6c65 2e56 4945 574c 4159 4552  estyle.VIEWLAYER
-003544e0: 5f50 545f 6672 6565 7374 796c 655f 6c69  _PT_freestyle_li
-003544f0: 6e65 7365 745f 6564 6765 7479 7065 2720  neset_edgetype' 
-00354500: 3d20 4e6f 6e65 0a0a 5649 4557 4c41 5945  = None..VIEWLAYE
-00354510: 525f 5054 5f66 7265 6573 7479 6c65 5f6c  R_PT_freestyle_l
-00354520: 696e 6573 6574 5f66 6163 656d 6172 6b73  ineset_facemarks
-00354530: 3a20 2762 6c5f 7569 2e70 726f 7065 7274  : 'bl_ui.propert
-00354540: 6965 735f 6672 6565 7374 796c 652e 5649  ies_freestyle.VI
-00354550: 4557 4c41 5945 525f 5054 5f66 7265 6573  EWLAYER_PT_frees
-00354560: 7479 6c65 5f6c 696e 6573 6574 5f66 6163  tyle_lineset_fac
-00354570: 656d 6172 6b73 2720 3d20 4e6f 6e65 0a0a  emarks' = None..
-00354580: 5649 4557 4c41 5945 525f 5054 5f66 7265  VIEWLAYER_PT_fre
-00354590: 6573 7479 6c65 5f6c 696e 6573 6574 5f76  estyle_lineset_v
-003545a0: 6973 6962 696c 7479 3a20 2762 6c5f 7569  isibilty: 'bl_ui
-003545b0: 2e70 726f 7065 7274 6965 735f 6672 6565  .properties_free
-003545c0: 7374 796c 652e 5649 4557 4c41 5945 525f  style.VIEWLAYER_
-003545d0: 5054 5f66 7265 6573 7479 6c65 5f6c 696e  PT_freestyle_lin
-003545e0: 6573 6574 5f76 6973 6962 696c 7479 2720  eset_visibilty' 
-003545f0: 3d20 4e6f 6e65 0a0a 5649 4557 4c41 5945  = None..VIEWLAYE
-00354600: 525f 5054 5f66 7265 6573 7479 6c65 5f6c  R_PT_freestyle_l
-00354610: 696e 6573 7479 6c65 5f61 6c70 6861 3a20  inestyle_alpha: 
-00354620: 2762 6c5f 7569 2e70 726f 7065 7274 6965  'bl_ui.propertie
-00354630: 735f 6672 6565 7374 796c 652e 5649 4557  s_freestyle.VIEW
-00354640: 4c41 5945 525f 5054 5f66 7265 6573 7479  LAYER_PT_freesty
-00354650: 6c65 5f6c 696e 6573 7479 6c65 5f61 6c70  le_linestyle_alp
-00354660: 6861 2720 3d20 4e6f 6e65 0a0a 5649 4557  ha' = None..VIEW
-00354670: 4c41 5945 525f 5054 5f66 7265 6573 7479  LAYER_PT_freesty
-00354680: 6c65 5f6c 696e 6573 7479 6c65 5f63 6f6c  le_linestyle_col
-00354690: 6f72 3a20 2762 6c5f 7569 2e70 726f 7065  or: 'bl_ui.prope
-003546a0: 7274 6965 735f 6672 6565 7374 796c 652e  rties_freestyle.
-003546b0: 5649 4557 4c41 5945 525f 5054 5f66 7265  VIEWLAYER_PT_fre
-003546c0: 6573 7479 6c65 5f6c 696e 6573 7479 6c65  estyle_linestyle
-003546d0: 5f63 6f6c 6f72 2720 3d20 4e6f 6e65 0a0a  _color' = None..
-003546e0: 5649 4557 4c41 5945 525f 5054 5f66 7265  VIEWLAYER_PT_fre
-003546f0: 6573 7479 6c65 5f6c 696e 6573 7479 6c65  estyle_linestyle
-00354700: 5f67 656f 6d65 7472 793a 2027 626c 5f75  _geometry: 'bl_u
-00354710: 692e 7072 6f70 6572 7469 6573 5f66 7265  i.properties_fre
-00354720: 6573 7479 6c65 2e56 4945 574c 4159 4552  estyle.VIEWLAYER
-00354730: 5f50 545f 6672 6565 7374 796c 655f 6c69  _PT_freestyle_li
-00354740: 6e65 7374 796c 655f 6765 6f6d 6574 7279  nestyle_geometry
-00354750: 2720 3d20 4e6f 6e65 0a0a 5649 4557 4c41  ' = None..VIEWLA
-00354760: 5945 525f 5054 5f66 7265 6573 7479 6c65  YER_PT_freestyle
-00354770: 5f6c 696e 6573 7479 6c65 5f73 7472 6f6b  _linestyle_strok
-00354780: 6573 3a20 2762 6c5f 7569 2e70 726f 7065  es: 'bl_ui.prope
-00354790: 7274 6965 735f 6672 6565 7374 796c 652e  rties_freestyle.
-003547a0: 5649 4557 4c41 5945 525f 5054 5f66 7265  VIEWLAYER_PT_fre
-003547b0: 6573 7479 6c65 5f6c 696e 6573 7479 6c65  estyle_linestyle
-003547c0: 5f73 7472 6f6b 6573 2720 3d20 4e6f 6e65  _strokes' = None
-003547d0: 0a0a 5649 4557 4c41 5945 525f 5054 5f66  ..VIEWLAYER_PT_f
-003547e0: 7265 6573 7479 6c65 5f6c 696e 6573 7479  reestyle_linesty
-003547f0: 6c65 5f73 7472 6f6b 6573 5f63 6861 696e  le_strokes_chain
-00354800: 696e 673a 2027 626c 5f75 692e 7072 6f70  ing: 'bl_ui.prop
-00354810: 6572 7469 6573 5f66 7265 6573 7479 6c65  erties_freestyle
-00354820: 2e56 4945 574c 4159 4552 5f50 545f 6672  .VIEWLAYER_PT_fr
-00354830: 6565 7374 796c 655f 6c69 6e65 7374 796c  eestyle_linestyl
-00354840: 655f 7374 726f 6b65 735f 6368 6169 6e69  e_strokes_chaini
-00354850: 6e67 2720 3d20 4e6f 6e65 0a0a 5649 4557  ng' = None..VIEW
-00354860: 4c41 5945 525f 5054 5f66 7265 6573 7479  LAYER_PT_freesty
-00354870: 6c65 5f6c 696e 6573 7479 6c65 5f73 7472  le_linestyle_str
-00354880: 6f6b 6573 5f64 6173 6865 646c 696e 653a  okes_dashedline:
-00354890: 2027 626c 5f75 692e 7072 6f70 6572 7469   'bl_ui.properti
-003548a0: 6573 5f66 7265 6573 7479 6c65 2e56 4945  es_freestyle.VIE
-003548b0: 574c 4159 4552 5f50 545f 6672 6565 7374  WLAYER_PT_freest
-003548c0: 796c 655f 6c69 6e65 7374 796c 655f 7374  yle_linestyle_st
-003548d0: 726f 6b65 735f 6461 7368 6564 6c69 6e65  rokes_dashedline
-003548e0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 4c41  ' = None..VIEWLA
-003548f0: 5945 525f 5054 5f66 7265 6573 7479 6c65  YER_PT_freestyle
-00354900: 5f6c 696e 6573 7479 6c65 5f73 7472 6f6b  _linestyle_strok
-00354910: 6573 5f73 656c 6563 7469 6f6e 3a20 2762  es_selection: 'b
-00354920: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
-00354930: 6672 6565 7374 796c 652e 5649 4557 4c41  freestyle.VIEWLA
-00354940: 5945 525f 5054 5f66 7265 6573 7479 6c65  YER_PT_freestyle
-00354950: 5f6c 696e 6573 7479 6c65 5f73 7472 6f6b  _linestyle_strok
-00354960: 6573 5f73 656c 6563 7469 6f6e 2720 3d20  es_selection' = 
-00354970: 4e6f 6e65 0a0a 5649 4557 4c41 5945 525f  None..VIEWLAYER_
-00354980: 5054 5f66 7265 6573 7479 6c65 5f6c 696e  PT_freestyle_lin
-00354990: 6573 7479 6c65 5f73 7472 6f6b 6573 5f73  estyle_strokes_s
-003549a0: 6f72 7469 6e67 3a20 2762 6c5f 7569 2e70  orting: 'bl_ui.p
-003549b0: 726f 7065 7274 6965 735f 6672 6565 7374  roperties_freest
-003549c0: 796c 652e 5649 4557 4c41 5945 525f 5054  yle.VIEWLAYER_PT
-003549d0: 5f66 7265 6573 7479 6c65 5f6c 696e 6573  _freestyle_lines
-003549e0: 7479 6c65 5f73 7472 6f6b 6573 5f73 6f72  tyle_strokes_sor
-003549f0: 7469 6e67 2720 3d20 4e6f 6e65 0a0a 5649  ting' = None..VI
-00354a00: 4557 4c41 5945 525f 5054 5f66 7265 6573  EWLAYER_PT_frees
-00354a10: 7479 6c65 5f6c 696e 6573 7479 6c65 5f73  tyle_linestyle_s
-00354a20: 7472 6f6b 6573 5f73 706c 6974 7469 6e67  trokes_splitting
-00354a30: 3a20 2762 6c5f 7569 2e70 726f 7065 7274  : 'bl_ui.propert
-00354a40: 6965 735f 6672 6565 7374 796c 652e 5649  ies_freestyle.VI
-00354a50: 4557 4c41 5945 525f 5054 5f66 7265 6573  EWLAYER_PT_frees
-00354a60: 7479 6c65 5f6c 696e 6573 7479 6c65 5f73  tyle_linestyle_s
-00354a70: 7472 6f6b 6573 5f73 706c 6974 7469 6e67  trokes_splitting
-00354a80: 2720 3d20 4e6f 6e65 0a0a 5649 4557 4c41  ' = None..VIEWLA
-00354a90: 5945 525f 5054 5f66 7265 6573 7479 6c65  YER_PT_freestyle
-00354aa0: 5f6c 696e 6573 7479 6c65 5f73 7472 6f6b  _linestyle_strok
-00354ab0: 6573 5f73 706c 6974 7469 6e67 5f70 6174  es_splitting_pat
-00354ac0: 7465 726e 3a20 2762 6c5f 7569 2e70 726f  tern: 'bl_ui.pro
-00354ad0: 7065 7274 6965 735f 6672 6565 7374 796c  perties_freestyl
-00354ae0: 652e 5649 4557 4c41 5945 525f 5054 5f66  e.VIEWLAYER_PT_f
-00354af0: 7265 6573 7479 6c65 5f6c 696e 6573 7479  reestyle_linesty
-00354b00: 6c65 5f73 7472 6f6b 6573 5f73 706c 6974  le_strokes_split
-00354b10: 7469 6e67 5f70 6174 7465 726e 2720 3d20  ting_pattern' = 
-00354b20: 4e6f 6e65 0a0a 5649 4557 4c41 5945 525f  None..VIEWLAYER_
-00354b30: 5054 5f66 7265 6573 7479 6c65 5f6c 696e  PT_freestyle_lin
-00354b40: 6573 7479 6c65 5f74 6578 7475 7265 3a20  estyle_texture: 
-00354b50: 2762 6c5f 7569 2e70 726f 7065 7274 6965  'bl_ui.propertie
-00354b60: 735f 6672 6565 7374 796c 652e 5649 4557  s_freestyle.VIEW
-00354b70: 4c41 5945 525f 5054 5f66 7265 6573 7479  LAYER_PT_freesty
-00354b80: 6c65 5f6c 696e 6573 7479 6c65 5f74 6578  le_linestyle_tex
-00354b90: 7475 7265 2720 3d20 4e6f 6e65 0a0a 5649  ture' = None..VI
-00354ba0: 4557 4c41 5945 525f 5054 5f66 7265 6573  EWLAYER_PT_frees
-00354bb0: 7479 6c65 5f6c 696e 6573 7479 6c65 5f74  tyle_linestyle_t
-00354bc0: 6869 636b 6e65 7373 3a20 2762 6c5f 7569  hickness: 'bl_ui
-00354bd0: 2e70 726f 7065 7274 6965 735f 6672 6565  .properties_free
-00354be0: 7374 796c 652e 5649 4557 4c41 5945 525f  style.VIEWLAYER_
-00354bf0: 5054 5f66 7265 6573 7479 6c65 5f6c 696e  PT_freestyle_lin
-00354c00: 6573 7479 6c65 5f74 6869 636b 6e65 7373  estyle_thickness
-00354c10: 2720 3d20 4e6f 6e65 0a0a 5649 4557 4c41  ' = None..VIEWLA
-00354c20: 5945 525f 5054 5f66 7265 6573 7479 6c65  YER_PT_freestyle
-00354c30: 5f73 7479 6c65 5f6d 6f64 756c 6573 3a20  _style_modules: 
-00354c40: 2762 6c5f 7569 2e70 726f 7065 7274 6965  'bl_ui.propertie
-00354c50: 735f 6672 6565 7374 796c 652e 5649 4557  s_freestyle.VIEW
-00354c60: 4c41 5945 525f 5054 5f66 7265 6573 7479  LAYER_PT_freesty
-00354c70: 6c65 5f73 7479 6c65 5f6d 6f64 756c 6573  le_style_modules
-00354c80: 2720 3d20 4e6f 6e65 0a0a 5649 4557 4c41  ' = None..VIEWLA
-00354c90: 5945 525f 5054 5f6c 6179 6572 3a20 2762  YER_PT_layer: 'b
-00354ca0: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
-00354cb0: 7669 6577 5f6c 6179 6572 2e56 4945 574c  view_layer.VIEWL
-00354cc0: 4159 4552 5f50 545f 6c61 7965 7227 203d  AYER_PT_layer' =
-00354cd0: 204e 6f6e 650a 0a56 4945 574c 4159 4552   None..VIEWLAYER
-00354ce0: 5f50 545f 6c61 7965 725f 6375 7374 6f6d  _PT_layer_custom
-00354cf0: 5f70 726f 7073 3a20 2762 6c5f 7569 2e70  _props: 'bl_ui.p
+00351af0: 6375 6c70 745f 7379 6d6d 6574 7279 3a20  culpt_symmetry: 
+00351b00: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
+00351b10: 7733 645f 746f 6f6c 6261 722e 5649 4557  w3d_toolbar.VIEW
+00351b20: 3344 5f50 545f 7363 756c 7074 5f73 796d  3D_PT_sculpt_sym
+00351b30: 6d65 7472 7927 203d 204e 6f6e 650a 0a56  metry' = None..V
+00351b40: 4945 5733 445f 5054 5f73 6375 6c70 745f  IEW3D_PT_sculpt_
+00351b50: 7379 6d6d 6574 7279 5f66 6f72 5f74 6f70  symmetry_for_top
+00351b60: 6261 723a 2027 626c 5f75 692e 7370 6163  bar: 'bl_ui.spac
+00351b70: 655f 7669 6577 3364 5f74 6f6f 6c62 6172  e_view3d_toolbar
+00351b80: 2e56 4945 5733 445f 5054 5f73 6375 6c70  .VIEW3D_PT_sculp
+00351b90: 745f 7379 6d6d 6574 7279 5f66 6f72 5f74  t_symmetry_for_t
+00351ba0: 6f70 6261 7227 203d 204e 6f6e 650a 0a56  opbar' = None..V
+00351bb0: 4945 5733 445f 5054 5f73 6375 6c70 745f  IEW3D_PT_sculpt_
+00351bc0: 766f 7865 6c5f 7265 6d65 7368 3a20 2762  voxel_remesh: 'b
+00351bd0: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+00351be0: 645f 746f 6f6c 6261 722e 5649 4557 3344  d_toolbar.VIEW3D
+00351bf0: 5f50 545f 7363 756c 7074 5f76 6f78 656c  _PT_sculpt_voxel
+00351c00: 5f72 656d 6573 6827 203d 204e 6f6e 650a  _remesh' = None.
+00351c10: 0a56 4945 5733 445f 5054 5f73 6861 6469  .VIEW3D_PT_shadi
+00351c20: 6e67 3a20 2762 6c5f 7569 2e73 7061 6365  ng: 'bl_ui.space
+00351c30: 5f76 6965 7733 642e 5649 4557 3344 5f50  _view3d.VIEW3D_P
+00351c40: 545f 7368 6164 696e 6727 203d 204e 6f6e  T_shading' = Non
+00351c50: 650a 0a56 4945 5733 445f 5054 5f73 6861  e..VIEW3D_PT_sha
+00351c60: 6469 6e67 5f63 6f6c 6f72 3a20 2762 6c5f  ding_color: 'bl_
+00351c70: 7569 2e73 7061 6365 5f76 6965 7733 642e  ui.space_view3d.
+00351c80: 5649 4557 3344 5f50 545f 7368 6164 696e  VIEW3D_PT_shadin
+00351c90: 675f 636f 6c6f 7227 203d 204e 6f6e 650a  g_color' = None.
+00351ca0: 0a56 4945 5733 445f 5054 5f73 6861 6469  .VIEW3D_PT_shadi
+00351cb0: 6e67 5f63 6f6d 706f 7369 746f 723a 2027  ng_compositor: '
+00351cc0: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
+00351cd0: 3364 2e56 4945 5733 445f 5054 5f73 6861  3d.VIEW3D_PT_sha
+00351ce0: 6469 6e67 5f63 6f6d 706f 7369 746f 7227  ding_compositor'
+00351cf0: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
+00351d00: 5054 5f73 6861 6469 6e67 5f6c 6967 6874  PT_shading_light
+00351d10: 696e 673a 2027 626c 5f75 692e 7370 6163  ing: 'bl_ui.spac
+00351d20: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
+00351d30: 5054 5f73 6861 6469 6e67 5f6c 6967 6874  PT_shading_light
+00351d40: 696e 6727 203d 204e 6f6e 650a 0a56 4945  ing' = None..VIE
+00351d50: 5733 445f 5054 5f73 6861 6469 6e67 5f6f  W3D_PT_shading_o
+00351d60: 7074 696f 6e73 3a20 2762 6c5f 7569 2e73  ptions: 'bl_ui.s
+00351d70: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
+00351d80: 3344 5f50 545f 7368 6164 696e 675f 6f70  3D_PT_shading_op
+00351d90: 7469 6f6e 7327 203d 204e 6f6e 650a 0a56  tions' = None..V
+00351da0: 4945 5733 445f 5054 5f73 6861 6469 6e67  IEW3D_PT_shading
+00351db0: 5f6f 7074 696f 6e73 5f73 6861 646f 773a  _options_shadow:
+00351dc0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+00351dd0: 6577 3364 2e56 4945 5733 445f 5054 5f73  ew3d.VIEW3D_PT_s
+00351de0: 6861 6469 6e67 5f6f 7074 696f 6e73 5f73  hading_options_s
+00351df0: 6861 646f 7727 203d 204e 6f6e 650a 0a56  hadow' = None..V
+00351e00: 4945 5733 445f 5054 5f73 6861 6469 6e67  IEW3D_PT_shading
+00351e10: 5f6f 7074 696f 6e73 5f73 7361 6f3a 2027  _options_ssao: '
+00351e20: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
+00351e30: 3364 2e56 4945 5733 445f 5054 5f73 6861  3d.VIEW3D_PT_sha
+00351e40: 6469 6e67 5f6f 7074 696f 6e73 5f73 7361  ding_options_ssa
+00351e50: 6f27 203d 204e 6f6e 650a 0a56 4945 5733  o' = None..VIEW3
+00351e60: 445f 5054 5f73 6861 6469 6e67 5f72 656e  D_PT_shading_ren
+00351e70: 6465 725f 7061 7373 3a20 2762 6c5f 7569  der_pass: 'bl_ui
+00351e80: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
+00351e90: 4557 3344 5f50 545f 7368 6164 696e 675f  EW3D_PT_shading_
+00351ea0: 7265 6e64 6572 5f70 6173 7327 203d 204e  render_pass' = N
+00351eb0: 6f6e 650a 0a56 4945 5733 445f 5054 5f73  one..VIEW3D_PT_s
+00351ec0: 6c6f 7473 5f70 6169 6e74 5f63 616e 7661  lots_paint_canva
+00351ed0: 733a 2027 626c 5f75 692e 7370 6163 655f  s: 'bl_ui.space_
+00351ee0: 7669 6577 3364 5f74 6f6f 6c62 6172 2e56  view3d_toolbar.V
+00351ef0: 4945 5733 445f 5054 5f73 6c6f 7473 5f70  IEW3D_PT_slots_p
+00351f00: 6169 6e74 5f63 616e 7661 7327 203d 204e  aint_canvas' = N
+00351f10: 6f6e 650a 0a56 4945 5733 445f 5054 5f73  one..VIEW3D_PT_s
+00351f20: 6c6f 7473 5f70 726f 6a65 6374 7061 696e  lots_projectpain
+00351f30: 743a 2027 626c 5f75 692e 7370 6163 655f  t: 'bl_ui.space_
+00351f40: 7669 6577 3364 5f74 6f6f 6c62 6172 2e56  view3d_toolbar.V
+00351f50: 4945 5733 445f 5054 5f73 6c6f 7473 5f70  IEW3D_PT_slots_p
+00351f60: 726f 6a65 6374 7061 696e 7427 203d 204e  rojectpaint' = N
+00351f70: 6f6e 650a 0a56 4945 5733 445f 5054 5f73  one..VIEW3D_PT_s
+00351f80: 6e61 7070 696e 673a 2027 626c 5f75 692e  napping: 'bl_ui.
+00351f90: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
+00351fa0: 5733 445f 5054 5f73 6e61 7070 696e 6727  W3D_PT_snapping'
+00351fb0: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
+00351fc0: 5054 5f73 7465 6e63 696c 5f70 726f 6a65  PT_stencil_proje
+00351fd0: 6374 7061 696e 743a 2027 626c 5f75 692e  ctpaint: 'bl_ui.
+00351fe0: 7370 6163 655f 7669 6577 3364 5f74 6f6f  space_view3d_too
+00351ff0: 6c62 6172 2e56 4945 5733 445f 5054 5f73  lbar.VIEW3D_PT_s
+00352000: 7465 6e63 696c 5f70 726f 6a65 6374 7061  tencil_projectpa
+00352010: 696e 7427 203d 204e 6f6e 650a 0a56 4945  int' = None..VIE
+00352020: 5733 445f 5054 5f74 6f6f 6c73 5f61 6374  W3D_PT_tools_act
+00352030: 6976 653a 2027 626c 5f75 692e 7370 6163  ive: 'bl_ui.spac
+00352040: 655f 746f 6f6c 7379 7374 656d 5f74 6f6f  e_toolsystem_too
+00352050: 6c62 6172 2e56 4945 5733 445f 5054 5f74  lbar.VIEW3D_PT_t
+00352060: 6f6f 6c73 5f61 6374 6976 6527 203d 204e  ools_active' = N
+00352070: 6f6e 650a 0a56 4945 5733 445f 5054 5f74  one..VIEW3D_PT_t
+00352080: 6f6f 6c73 5f61 726d 6174 7572 6565 6469  ools_armatureedi
+00352090: 745f 6f70 7469 6f6e 733a 2027 626c 5f75  t_options: 'bl_u
+003520a0: 692e 7370 6163 655f 7669 6577 3364 5f74  i.space_view3d_t
+003520b0: 6f6f 6c62 6172 2e56 4945 5733 445f 5054  oolbar.VIEW3D_PT
+003520c0: 5f74 6f6f 6c73 5f61 726d 6174 7572 6565  _tools_armaturee
+003520d0: 6469 745f 6f70 7469 6f6e 7327 203d 204e  dit_options' = N
+003520e0: 6f6e 650a 0a56 4945 5733 445f 5054 5f74  one..VIEW3D_PT_t
+003520f0: 6f6f 6c73 5f62 7275 7368 5f63 6c6f 6e65  ools_brush_clone
+00352100: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+00352110: 6965 7733 645f 746f 6f6c 6261 722e 5649  iew3d_toolbar.VI
+00352120: 4557 3344 5f50 545f 746f 6f6c 735f 6272  EW3D_PT_tools_br
+00352130: 7573 685f 636c 6f6e 6527 203d 204e 6f6e  ush_clone' = Non
+00352140: 650a 0a56 4945 5733 445f 5054 5f74 6f6f  e..VIEW3D_PT_too
+00352150: 6c73 5f62 7275 7368 5f63 6f6c 6f72 3a20  ls_brush_color: 
+00352160: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
+00352170: 7733 645f 746f 6f6c 6261 722e 5649 4557  w3d_toolbar.VIEW
+00352180: 3344 5f50 545f 746f 6f6c 735f 6272 7573  3D_PT_tools_brus
+00352190: 685f 636f 6c6f 7227 203d 204e 6f6e 650a  h_color' = None.
+003521a0: 0a56 4945 5733 445f 5054 5f74 6f6f 6c73  .VIEW3D_PT_tools
+003521b0: 5f62 7275 7368 5f64 6973 706c 6179 3a20  _brush_display: 
+003521c0: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
+003521d0: 7733 645f 746f 6f6c 6261 722e 5649 4557  w3d_toolbar.VIEW
+003521e0: 3344 5f50 545f 746f 6f6c 735f 6272 7573  3D_PT_tools_brus
+003521f0: 685f 6469 7370 6c61 7927 203d 204e 6f6e  h_display' = Non
+00352200: 650a 0a56 4945 5733 445f 5054 5f74 6f6f  e..VIEW3D_PT_too
+00352210: 6c73 5f62 7275 7368 5f66 616c 6c6f 6666  ls_brush_falloff
+00352220: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+00352230: 6965 7733 645f 746f 6f6c 6261 722e 5649  iew3d_toolbar.VI
+00352240: 4557 3344 5f50 545f 746f 6f6c 735f 6272  EW3D_PT_tools_br
+00352250: 7573 685f 6661 6c6c 6f66 6627 203d 204e  ush_falloff' = N
+00352260: 6f6e 650a 0a56 4945 5733 445f 5054 5f74  one..VIEW3D_PT_t
+00352270: 6f6f 6c73 5f62 7275 7368 5f66 616c 6c6f  ools_brush_fallo
+00352280: 6666 5f66 726f 6e74 6661 6365 3a20 2762  ff_frontface: 'b
+00352290: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+003522a0: 645f 746f 6f6c 6261 722e 5649 4557 3344  d_toolbar.VIEW3D
+003522b0: 5f50 545f 746f 6f6c 735f 6272 7573 685f  _PT_tools_brush_
+003522c0: 6661 6c6c 6f66 665f 6672 6f6e 7466 6163  falloff_frontfac
+003522d0: 6527 203d 204e 6f6e 650a 0a56 4945 5733  e' = None..VIEW3
+003522e0: 445f 5054 5f74 6f6f 6c73 5f62 7275 7368  D_PT_tools_brush
+003522f0: 5f66 616c 6c6f 6666 5f6e 6f72 6d61 6c3a  _falloff_normal:
+00352300: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+00352310: 6577 3364 5f74 6f6f 6c62 6172 2e56 4945  ew3d_toolbar.VIE
+00352320: 5733 445f 5054 5f74 6f6f 6c73 5f62 7275  W3D_PT_tools_bru
+00352330: 7368 5f66 616c 6c6f 6666 5f6e 6f72 6d61  sh_falloff_norma
+00352340: 6c27 203d 204e 6f6e 650a 0a56 4945 5733  l' = None..VIEW3
+00352350: 445f 5054 5f74 6f6f 6c73 5f62 7275 7368  D_PT_tools_brush
+00352360: 5f73 656c 6563 743a 2027 626c 5f75 692e  _select: 'bl_ui.
+00352370: 7370 6163 655f 7669 6577 3364 5f74 6f6f  space_view3d_too
+00352380: 6c62 6172 2e56 4945 5733 445f 5054 5f74  lbar.VIEW3D_PT_t
+00352390: 6f6f 6c73 5f62 7275 7368 5f73 656c 6563  ools_brush_selec
+003523a0: 7427 203d 204e 6f6e 650a 0a56 4945 5733  t' = None..VIEW3
+003523b0: 445f 5054 5f74 6f6f 6c73 5f62 7275 7368  D_PT_tools_brush
+003523c0: 5f73 6574 7469 6e67 733a 2027 626c 5f75  _settings: 'bl_u
+003523d0: 692e 7370 6163 655f 7669 6577 3364 5f74  i.space_view3d_t
+003523e0: 6f6f 6c62 6172 2e56 4945 5733 445f 5054  oolbar.VIEW3D_PT
+003523f0: 5f74 6f6f 6c73 5f62 7275 7368 5f73 6574  _tools_brush_set
+00352400: 7469 6e67 7327 203d 204e 6f6e 650a 0a56  tings' = None..V
+00352410: 4945 5733 445f 5054 5f74 6f6f 6c73 5f62  IEW3D_PT_tools_b
+00352420: 7275 7368 5f73 6574 7469 6e67 735f 6164  rush_settings_ad
+00352430: 7661 6e63 6564 3a20 2762 6c5f 7569 2e73  vanced: 'bl_ui.s
+00352440: 7061 6365 5f76 6965 7733 645f 746f 6f6c  pace_view3d_tool
+00352450: 6261 722e 5649 4557 3344 5f50 545f 746f  bar.VIEW3D_PT_to
+00352460: 6f6c 735f 6272 7573 685f 7365 7474 696e  ols_brush_settin
+00352470: 6773 5f61 6476 616e 6365 6427 203d 204e  gs_advanced' = N
+00352480: 6f6e 650a 0a56 4945 5733 445f 5054 5f74  one..VIEW3D_PT_t
+00352490: 6f6f 6c73 5f62 7275 7368 5f73 7472 6f6b  ools_brush_strok
+003524a0: 653a 2027 626c 5f75 692e 7370 6163 655f  e: 'bl_ui.space_
+003524b0: 7669 6577 3364 5f74 6f6f 6c62 6172 2e56  view3d_toolbar.V
+003524c0: 4945 5733 445f 5054 5f74 6f6f 6c73 5f62  IEW3D_PT_tools_b
+003524d0: 7275 7368 5f73 7472 6f6b 6527 203d 204e  rush_stroke' = N
+003524e0: 6f6e 650a 0a56 4945 5733 445f 5054 5f74  one..VIEW3D_PT_t
+003524f0: 6f6f 6c73 5f62 7275 7368 5f73 7472 6f6b  ools_brush_strok
+00352500: 655f 736d 6f6f 7468 5f73 7472 6f6b 653a  e_smooth_stroke:
+00352510: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+00352520: 6577 3364 5f74 6f6f 6c62 6172 2e56 4945  ew3d_toolbar.VIE
+00352530: 5733 445f 5054 5f74 6f6f 6c73 5f62 7275  W3D_PT_tools_bru
+00352540: 7368 5f73 7472 6f6b 655f 736d 6f6f 7468  sh_stroke_smooth
+00352550: 5f73 7472 6f6b 6527 203d 204e 6f6e 650a  _stroke' = None.
+00352560: 0a56 4945 5733 445f 5054 5f74 6f6f 6c73  .VIEW3D_PT_tools
+00352570: 5f62 7275 7368 5f73 7761 7463 6865 733a  _brush_swatches:
+00352580: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+00352590: 6577 3364 5f74 6f6f 6c62 6172 2e56 4945  ew3d_toolbar.VIE
+003525a0: 5733 445f 5054 5f74 6f6f 6c73 5f62 7275  W3D_PT_tools_bru
+003525b0: 7368 5f73 7761 7463 6865 7327 203d 204e  sh_swatches' = N
+003525c0: 6f6e 650a 0a56 4945 5733 445f 5054 5f74  one..VIEW3D_PT_t
+003525d0: 6f6f 6c73 5f62 7275 7368 5f74 6578 7475  ools_brush_textu
+003525e0: 7265 3a20 2762 6c5f 7569 2e73 7061 6365  re: 'bl_ui.space
+003525f0: 5f76 6965 7733 645f 746f 6f6c 6261 722e  _view3d_toolbar.
+00352600: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
+00352610: 6272 7573 685f 7465 7874 7572 6527 203d  brush_texture' =
+00352620: 204e 6f6e 650a 0a56 4945 5733 445f 5054   None..VIEW3D_PT
+00352630: 5f74 6f6f 6c73 5f67 7265 6173 655f 7065  _tools_grease_pe
+00352640: 6e63 696c 5f62 7275 7368 5f61 6476 616e  ncil_brush_advan
+00352650: 6365 643a 2027 626c 5f75 692e 7370 6163  ced: 'bl_ui.spac
+00352660: 655f 7669 6577 3364 5f74 6f6f 6c62 6172  e_view3d_toolbar
+00352670: 2e56 4945 5733 445f 5054 5f74 6f6f 6c73  .VIEW3D_PT_tools
+00352680: 5f67 7265 6173 655f 7065 6e63 696c 5f62  _grease_pencil_b
+00352690: 7275 7368 5f61 6476 616e 6365 6427 203d  rush_advanced' =
+003526a0: 204e 6f6e 650a 0a56 4945 5733 445f 5054   None..VIEW3D_PT
+003526b0: 5f74 6f6f 6c73 5f67 7265 6173 655f 7065  _tools_grease_pe
+003526c0: 6e63 696c 5f62 7275 7368 5f67 6170 5f63  ncil_brush_gap_c
+003526d0: 6c6f 7375 7265 3a20 2762 6c5f 7569 2e73  losure: 'bl_ui.s
+003526e0: 7061 6365 5f76 6965 7733 645f 746f 6f6c  pace_view3d_tool
+003526f0: 6261 722e 5649 4557 3344 5f50 545f 746f  bar.VIEW3D_PT_to
+00352700: 6f6c 735f 6772 6561 7365 5f70 656e 6369  ols_grease_penci
+00352710: 6c5f 6272 7573 685f 6761 705f 636c 6f73  l_brush_gap_clos
+00352720: 7572 6527 203d 204e 6f6e 650a 0a56 4945  ure' = None..VIE
+00352730: 5733 445f 5054 5f74 6f6f 6c73 5f67 7265  W3D_PT_tools_gre
+00352740: 6173 655f 7065 6e63 696c 5f62 7275 7368  ase_pencil_brush
+00352750: 5f6d 6978 5f70 616c 6574 7465 3a20 2762  _mix_palette: 'b
+00352760: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+00352770: 645f 746f 6f6c 6261 722e 5649 4557 3344  d_toolbar.VIEW3D
+00352780: 5f50 545f 746f 6f6c 735f 6772 6561 7365  _PT_tools_grease
+00352790: 5f70 656e 6369 6c5f 6272 7573 685f 6d69  _pencil_brush_mi
+003527a0: 785f 7061 6c65 7474 6527 203d 204e 6f6e  x_palette' = Non
+003527b0: 650a 0a56 4945 5733 445f 5054 5f74 6f6f  e..VIEW3D_PT_too
+003527c0: 6c73 5f67 7265 6173 655f 7065 6e63 696c  ls_grease_pencil
+003527d0: 5f62 7275 7368 5f6d 6978 636f 6c6f 723a  _brush_mixcolor:
+003527e0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+003527f0: 6577 3364 5f74 6f6f 6c62 6172 2e56 4945  ew3d_toolbar.VIE
+00352800: 5733 445f 5054 5f74 6f6f 6c73 5f67 7265  W3D_PT_tools_gre
+00352810: 6173 655f 7065 6e63 696c 5f62 7275 7368  ase_pencil_brush
+00352820: 5f6d 6978 636f 6c6f 7227 203d 204e 6f6e  _mixcolor' = Non
+00352830: 650a 0a56 4945 5733 445f 5054 5f74 6f6f  e..VIEW3D_PT_too
+00352840: 6c73 5f67 7265 6173 655f 7065 6e63 696c  ls_grease_pencil
+00352850: 5f62 7275 7368 5f70 6169 6e74 5f66 616c  _brush_paint_fal
+00352860: 6c6f 6666 3a20 2762 6c5f 7569 2e73 7061  loff: 'bl_ui.spa
+00352870: 6365 5f76 6965 7733 645f 746f 6f6c 6261  ce_view3d_toolba
+00352880: 722e 5649 4557 3344 5f50 545f 746f 6f6c  r.VIEW3D_PT_tool
+00352890: 735f 6772 6561 7365 5f70 656e 6369 6c5f  s_grease_pencil_
+003528a0: 6272 7573 685f 7061 696e 745f 6661 6c6c  brush_paint_fall
+003528b0: 6f66 6627 203d 204e 6f6e 650a 0a56 4945  off' = None..VIE
+003528c0: 5733 445f 5054 5f74 6f6f 6c73 5f67 7265  W3D_PT_tools_gre
+003528d0: 6173 655f 7065 6e63 696c 5f62 7275 7368  ase_pencil_brush
+003528e0: 5f70 6f73 745f 7072 6f63 6573 7369 6e67  _post_processing
+003528f0: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+00352900: 6965 7733 645f 746f 6f6c 6261 722e 5649  iew3d_toolbar.VI
+00352910: 4557 3344 5f50 545f 746f 6f6c 735f 6772  EW3D_PT_tools_gr
+00352920: 6561 7365 5f70 656e 6369 6c5f 6272 7573  ease_pencil_brus
+00352930: 685f 706f 7374 5f70 726f 6365 7373 696e  h_post_processin
+00352940: 6727 203d 204e 6f6e 650a 0a56 4945 5733  g' = None..VIEW3
+00352950: 445f 5054 5f74 6f6f 6c73 5f67 7265 6173  D_PT_tools_greas
+00352960: 655f 7065 6e63 696c 5f62 7275 7368 5f72  e_pencil_brush_r
+00352970: 616e 646f 6d3a 2027 626c 5f75 692e 7370  andom: 'bl_ui.sp
+00352980: 6163 655f 7669 6577 3364 5f74 6f6f 6c62  ace_view3d_toolb
+00352990: 6172 2e56 4945 5733 445f 5054 5f74 6f6f  ar.VIEW3D_PT_too
+003529a0: 6c73 5f67 7265 6173 655f 7065 6e63 696c  ls_grease_pencil
+003529b0: 5f62 7275 7368 5f72 616e 646f 6d27 203d  _brush_random' =
+003529c0: 204e 6f6e 650a 0a56 4945 5733 445f 5054   None..VIEW3D_PT
+003529d0: 5f74 6f6f 6c73 5f67 7265 6173 655f 7065  _tools_grease_pe
+003529e0: 6e63 696c 5f62 7275 7368 5f73 6375 6c70  ncil_brush_sculp
+003529f0: 745f 6661 6c6c 6f66 663a 2027 626c 5f75  t_falloff: 'bl_u
+00352a00: 692e 7370 6163 655f 7669 6577 3364 5f74  i.space_view3d_t
+00352a10: 6f6f 6c62 6172 2e56 4945 5733 445f 5054  oolbar.VIEW3D_PT
+00352a20: 5f74 6f6f 6c73 5f67 7265 6173 655f 7065  _tools_grease_pe
+00352a30: 6e63 696c 5f62 7275 7368 5f73 6375 6c70  ncil_brush_sculp
+00352a40: 745f 6661 6c6c 6f66 6627 203d 204e 6f6e  t_falloff' = Non
+00352a50: 650a 0a56 4945 5733 445f 5054 5f74 6f6f  e..VIEW3D_PT_too
+00352a60: 6c73 5f67 7265 6173 655f 7065 6e63 696c  ls_grease_pencil
+00352a70: 5f62 7275 7368 5f73 656c 6563 743a 2027  _brush_select: '
+00352a80: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
+00352a90: 3364 5f74 6f6f 6c62 6172 2e56 4945 5733  3d_toolbar.VIEW3
+00352aa0: 445f 5054 5f74 6f6f 6c73 5f67 7265 6173  D_PT_tools_greas
+00352ab0: 655f 7065 6e63 696c 5f62 7275 7368 5f73  e_pencil_brush_s
+00352ac0: 656c 6563 7427 203d 204e 6f6e 650a 0a56  elect' = None..V
+00352ad0: 4945 5733 445f 5054 5f74 6f6f 6c73 5f67  IEW3D_PT_tools_g
+00352ae0: 7265 6173 655f 7065 6e63 696c 5f62 7275  rease_pencil_bru
+00352af0: 7368 5f73 6574 7469 6e67 733a 2027 626c  sh_settings: 'bl
+00352b00: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+00352b10: 5f74 6f6f 6c62 6172 2e56 4945 5733 445f  _toolbar.VIEW3D_
+00352b20: 5054 5f74 6f6f 6c73 5f67 7265 6173 655f  PT_tools_grease_
+00352b30: 7065 6e63 696c 5f62 7275 7368 5f73 6574  pencil_brush_set
+00352b40: 7469 6e67 7327 203d 204e 6f6e 650a 0a56  tings' = None..V
+00352b50: 4945 5733 445f 5054 5f74 6f6f 6c73 5f67  IEW3D_PT_tools_g
+00352b60: 7265 6173 655f 7065 6e63 696c 5f62 7275  rease_pencil_bru
+00352b70: 7368 5f73 7461 6269 6c69 7a65 723a 2027  sh_stabilizer: '
+00352b80: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
+00352b90: 3364 5f74 6f6f 6c62 6172 2e56 4945 5733  3d_toolbar.VIEW3
+00352ba0: 445f 5054 5f74 6f6f 6c73 5f67 7265 6173  D_PT_tools_greas
+00352bb0: 655f 7065 6e63 696c 5f62 7275 7368 5f73  e_pencil_brush_s
+00352bc0: 7461 6269 6c69 7a65 7227 203d 204e 6f6e  tabilizer' = Non
+00352bd0: 650a 0a56 4945 5733 445f 5054 5f74 6f6f  e..VIEW3D_PT_too
+00352be0: 6c73 5f67 7265 6173 655f 7065 6e63 696c  ls_grease_pencil
+00352bf0: 5f62 7275 7368 5f73 7472 6f6b 653a 2027  _brush_stroke: '
+00352c00: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
+00352c10: 3364 5f74 6f6f 6c62 6172 2e56 4945 5733  3d_toolbar.VIEW3
+00352c20: 445f 5054 5f74 6f6f 6c73 5f67 7265 6173  D_PT_tools_greas
+00352c30: 655f 7065 6e63 696c 5f62 7275 7368 5f73  e_pencil_brush_s
+00352c40: 7472 6f6b 6527 203d 204e 6f6e 650a 0a56  troke' = None..V
+00352c50: 4945 5733 445f 5054 5f74 6f6f 6c73 5f67  IEW3D_PT_tools_g
+00352c60: 7265 6173 655f 7065 6e63 696c 5f62 7275  rease_pencil_bru
+00352c70: 7368 5f76 6572 7465 785f 636f 6c6f 723a  sh_vertex_color:
+00352c80: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+00352c90: 6577 3364 5f74 6f6f 6c62 6172 2e56 4945  ew3d_toolbar.VIE
+00352ca0: 5733 445f 5054 5f74 6f6f 6c73 5f67 7265  W3D_PT_tools_gre
+00352cb0: 6173 655f 7065 6e63 696c 5f62 7275 7368  ase_pencil_brush
+00352cc0: 5f76 6572 7465 785f 636f 6c6f 7227 203d  _vertex_color' =
+00352cd0: 204e 6f6e 650a 0a56 4945 5733 445f 5054   None..VIEW3D_PT
+00352ce0: 5f74 6f6f 6c73 5f67 7265 6173 655f 7065  _tools_grease_pe
+00352cf0: 6e63 696c 5f62 7275 7368 5f76 6572 7465  ncil_brush_verte
+00352d00: 785f 6661 6c6c 6f66 663a 2027 626c 5f75  x_falloff: 'bl_u
+00352d10: 692e 7370 6163 655f 7669 6577 3364 5f74  i.space_view3d_t
+00352d20: 6f6f 6c62 6172 2e56 4945 5733 445f 5054  oolbar.VIEW3D_PT
+00352d30: 5f74 6f6f 6c73 5f67 7265 6173 655f 7065  _tools_grease_pe
+00352d40: 6e63 696c 5f62 7275 7368 5f76 6572 7465  ncil_brush_verte
+00352d50: 785f 6661 6c6c 6f66 6627 203d 204e 6f6e  x_falloff' = Non
+00352d60: 650a 0a56 4945 5733 445f 5054 5f74 6f6f  e..VIEW3D_PT_too
+00352d70: 6c73 5f67 7265 6173 655f 7065 6e63 696c  ls_grease_pencil
+00352d80: 5f62 7275 7368 5f76 6572 7465 785f 7061  _brush_vertex_pa
+00352d90: 6c65 7474 653a 2027 626c 5f75 692e 7370  lette: 'bl_ui.sp
+00352da0: 6163 655f 7669 6577 3364 5f74 6f6f 6c62  ace_view3d_toolb
+00352db0: 6172 2e56 4945 5733 445f 5054 5f74 6f6f  ar.VIEW3D_PT_too
+00352dc0: 6c73 5f67 7265 6173 655f 7065 6e63 696c  ls_grease_pencil
+00352dd0: 5f62 7275 7368 5f76 6572 7465 785f 7061  _brush_vertex_pa
+00352de0: 6c65 7474 6527 203d 204e 6f6e 650a 0a56  lette' = None..V
+00352df0: 4945 5733 445f 5054 5f74 6f6f 6c73 5f67  IEW3D_PT_tools_g
+00352e00: 7265 6173 655f 7065 6e63 696c 5f62 7275  rease_pencil_bru
+00352e10: 7368 5f77 6569 6768 745f 6661 6c6c 6f66  sh_weight_fallof
+00352e20: 663a 2027 626c 5f75 692e 7370 6163 655f  f: 'bl_ui.space_
+00352e30: 7669 6577 3364 5f74 6f6f 6c62 6172 2e56  view3d_toolbar.V
+00352e40: 4945 5733 445f 5054 5f74 6f6f 6c73 5f67  IEW3D_PT_tools_g
+00352e50: 7265 6173 655f 7065 6e63 696c 5f62 7275  rease_pencil_bru
+00352e60: 7368 5f77 6569 6768 745f 6661 6c6c 6f66  sh_weight_fallof
+00352e70: 6627 203d 204e 6f6e 650a 0a56 4945 5733  f' = None..VIEW3
+00352e80: 445f 5054 5f74 6f6f 6c73 5f67 7265 6173  D_PT_tools_greas
+00352e90: 655f 7065 6e63 696c 5f70 6169 6e74 5f61  e_pencil_paint_a
+00352ea0: 7070 6561 7261 6e63 653a 2027 626c 5f75  ppearance: 'bl_u
+00352eb0: 692e 7370 6163 655f 7669 6577 3364 5f74  i.space_view3d_t
+00352ec0: 6f6f 6c62 6172 2e56 4945 5733 445f 5054  oolbar.VIEW3D_PT
+00352ed0: 5f74 6f6f 6c73 5f67 7265 6173 655f 7065  _tools_grease_pe
+00352ee0: 6e63 696c 5f70 6169 6e74 5f61 7070 6561  ncil_paint_appea
+00352ef0: 7261 6e63 6527 203d 204e 6f6e 650a 0a56  rance' = None..V
+00352f00: 4945 5733 445f 5054 5f74 6f6f 6c73 5f67  IEW3D_PT_tools_g
+00352f10: 7265 6173 655f 7065 6e63 696c 5f73 6375  rease_pencil_scu
+00352f20: 6c70 745f 6170 7065 6172 616e 6365 3a20  lpt_appearance: 
+00352f30: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
+00352f40: 7733 645f 746f 6f6c 6261 722e 5649 4557  w3d_toolbar.VIEW
+00352f50: 3344 5f50 545f 746f 6f6c 735f 6772 6561  3D_PT_tools_grea
+00352f60: 7365 5f70 656e 6369 6c5f 7363 756c 7074  se_pencil_sculpt
+00352f70: 5f61 7070 6561 7261 6e63 6527 203d 204e  _appearance' = N
+00352f80: 6f6e 650a 0a56 4945 5733 445f 5054 5f74  one..VIEW3D_PT_t
+00352f90: 6f6f 6c73 5f67 7265 6173 655f 7065 6e63  ools_grease_penc
+00352fa0: 696c 5f73 6375 6c70 745f 6272 7573 685f  il_sculpt_brush_
+00352fb0: 6164 7661 6e63 6564 3a20 2762 6c5f 7569  advanced: 'bl_ui
+00352fc0: 2e73 7061 6365 5f76 6965 7733 645f 746f  .space_view3d_to
+00352fd0: 6f6c 6261 722e 5649 4557 3344 5f50 545f  olbar.VIEW3D_PT_
+00352fe0: 746f 6f6c 735f 6772 6561 7365 5f70 656e  tools_grease_pen
+00352ff0: 6369 6c5f 7363 756c 7074 5f62 7275 7368  cil_sculpt_brush
+00353000: 5f61 6476 616e 6365 6427 203d 204e 6f6e  _advanced' = Non
+00353010: 650a 0a56 4945 5733 445f 5054 5f74 6f6f  e..VIEW3D_PT_too
+00353020: 6c73 5f67 7265 6173 655f 7065 6e63 696c  ls_grease_pencil
+00353030: 5f73 6375 6c70 745f 6272 7573 685f 706f  _sculpt_brush_po
+00353040: 706f 7665 723a 2027 626c 5f75 692e 7370  pover: 'bl_ui.sp
+00353050: 6163 655f 7669 6577 3364 5f74 6f6f 6c62  ace_view3d_toolb
+00353060: 6172 2e56 4945 5733 445f 5054 5f74 6f6f  ar.VIEW3D_PT_too
+00353070: 6c73 5f67 7265 6173 655f 7065 6e63 696c  ls_grease_pencil
+00353080: 5f73 6375 6c70 745f 6272 7573 685f 706f  _sculpt_brush_po
+00353090: 706f 7665 7227 203d 204e 6f6e 650a 0a56  pover' = None..V
+003530a0: 4945 5733 445f 5054 5f74 6f6f 6c73 5f67  IEW3D_PT_tools_g
+003530b0: 7265 6173 655f 7065 6e63 696c 5f73 6375  rease_pencil_scu
+003530c0: 6c70 745f 7365 6c65 6374 3a20 2762 6c5f  lpt_select: 'bl_
+003530d0: 7569 2e73 7061 6365 5f76 6965 7733 645f  ui.space_view3d_
+003530e0: 746f 6f6c 6261 722e 5649 4557 3344 5f50  toolbar.VIEW3D_P
+003530f0: 545f 746f 6f6c 735f 6772 6561 7365 5f70  T_tools_grease_p
+00353100: 656e 6369 6c5f 7363 756c 7074 5f73 656c  encil_sculpt_sel
+00353110: 6563 7427 203d 204e 6f6e 650a 0a56 4945  ect' = None..VIE
+00353120: 5733 445f 5054 5f74 6f6f 6c73 5f67 7265  W3D_PT_tools_gre
+00353130: 6173 655f 7065 6e63 696c 5f73 6375 6c70  ase_pencil_sculp
+00353140: 745f 7365 7474 696e 6773 3a20 2762 6c5f  t_settings: 'bl_
+00353150: 7569 2e73 7061 6365 5f76 6965 7733 645f  ui.space_view3d_
+00353160: 746f 6f6c 6261 722e 5649 4557 3344 5f50  toolbar.VIEW3D_P
+00353170: 545f 746f 6f6c 735f 6772 6561 7365 5f70  T_tools_grease_p
+00353180: 656e 6369 6c5f 7363 756c 7074 5f73 6574  encil_sculpt_set
+00353190: 7469 6e67 7327 203d 204e 6f6e 650a 0a56  tings' = None..V
+003531a0: 4945 5733 445f 5054 5f74 6f6f 6c73 5f67  IEW3D_PT_tools_g
+003531b0: 7265 6173 655f 7065 6e63 696c 5f76 6572  rease_pencil_ver
+003531c0: 7465 785f 6170 7065 6172 616e 6365 3a20  tex_appearance: 
+003531d0: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
+003531e0: 7733 645f 746f 6f6c 6261 722e 5649 4557  w3d_toolbar.VIEW
+003531f0: 3344 5f50 545f 746f 6f6c 735f 6772 6561  3D_PT_tools_grea
+00353200: 7365 5f70 656e 6369 6c5f 7665 7274 6578  se_pencil_vertex
+00353210: 5f61 7070 6561 7261 6e63 6527 203d 204e  _appearance' = N
+00353220: 6f6e 650a 0a56 4945 5733 445f 5054 5f74  one..VIEW3D_PT_t
+00353230: 6f6f 6c73 5f67 7265 6173 655f 7065 6e63  ools_grease_penc
+00353240: 696c 5f76 6572 7465 785f 7061 696e 745f  il_vertex_paint_
+00353250: 7365 6c65 6374 3a20 2762 6c5f 7569 2e73  select: 'bl_ui.s
+00353260: 7061 6365 5f76 6965 7733 645f 746f 6f6c  pace_view3d_tool
+00353270: 6261 722e 5649 4557 3344 5f50 545f 746f  bar.VIEW3D_PT_to
+00353280: 6f6c 735f 6772 6561 7365 5f70 656e 6369  ols_grease_penci
+00353290: 6c5f 7665 7274 6578 5f70 6169 6e74 5f73  l_vertex_paint_s
+003532a0: 656c 6563 7427 203d 204e 6f6e 650a 0a56  elect' = None..V
+003532b0: 4945 5733 445f 5054 5f74 6f6f 6c73 5f67  IEW3D_PT_tools_g
+003532c0: 7265 6173 655f 7065 6e63 696c 5f76 6572  rease_pencil_ver
+003532d0: 7465 785f 7061 696e 745f 7365 7474 696e  tex_paint_settin
+003532e0: 6773 3a20 2762 6c5f 7569 2e73 7061 6365  gs: 'bl_ui.space
+003532f0: 5f76 6965 7733 645f 746f 6f6c 6261 722e  _view3d_toolbar.
+00353300: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
+00353310: 6772 6561 7365 5f70 656e 6369 6c5f 7665  grease_pencil_ve
+00353320: 7274 6578 5f70 6169 6e74 5f73 6574 7469  rtex_paint_setti
+00353330: 6e67 7327 203d 204e 6f6e 650a 0a56 4945  ngs' = None..VIE
+00353340: 5733 445f 5054 5f74 6f6f 6c73 5f67 7265  W3D_PT_tools_gre
+00353350: 6173 655f 7065 6e63 696c 5f77 6569 6768  ase_pencil_weigh
+00353360: 745f 6170 7065 6172 616e 6365 3a20 2762  t_appearance: 'b
+00353370: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+00353380: 645f 746f 6f6c 6261 722e 5649 4557 3344  d_toolbar.VIEW3D
+00353390: 5f50 545f 746f 6f6c 735f 6772 6561 7365  _PT_tools_grease
+003533a0: 5f70 656e 6369 6c5f 7765 6967 6874 5f61  _pencil_weight_a
+003533b0: 7070 6561 7261 6e63 6527 203d 204e 6f6e  ppearance' = Non
+003533c0: 650a 0a56 4945 5733 445f 5054 5f74 6f6f  e..VIEW3D_PT_too
+003533d0: 6c73 5f67 7265 6173 655f 7065 6e63 696c  ls_grease_pencil
+003533e0: 5f77 6569 6768 745f 6f70 7469 6f6e 733a  _weight_options:
+003533f0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+00353400: 6577 3364 5f74 6f6f 6c62 6172 2e56 4945  ew3d_toolbar.VIE
+00353410: 5733 445f 5054 5f74 6f6f 6c73 5f67 7265  W3D_PT_tools_gre
+00353420: 6173 655f 7065 6e63 696c 5f77 6569 6768  ase_pencil_weigh
+00353430: 745f 6f70 7469 6f6e 7327 203d 204e 6f6e  t_options' = Non
+00353440: 650a 0a56 4945 5733 445f 5054 5f74 6f6f  e..VIEW3D_PT_too
+00353450: 6c73 5f67 7265 6173 655f 7065 6e63 696c  ls_grease_pencil
+00353460: 5f77 6569 6768 745f 7061 696e 745f 7365  _weight_paint_se
+00353470: 6c65 6374 3a20 2762 6c5f 7569 2e73 7061  lect: 'bl_ui.spa
+00353480: 6365 5f76 6965 7733 645f 746f 6f6c 6261  ce_view3d_toolba
+00353490: 722e 5649 4557 3344 5f50 545f 746f 6f6c  r.VIEW3D_PT_tool
+003534a0: 735f 6772 6561 7365 5f70 656e 6369 6c5f  s_grease_pencil_
+003534b0: 7765 6967 6874 5f70 6169 6e74 5f73 656c  weight_paint_sel
+003534c0: 6563 7427 203d 204e 6f6e 650a 0a56 4945  ect' = None..VIE
+003534d0: 5733 445f 5054 5f74 6f6f 6c73 5f67 7265  W3D_PT_tools_gre
+003534e0: 6173 655f 7065 6e63 696c 5f77 6569 6768  ase_pencil_weigh
+003534f0: 745f 7061 696e 745f 7365 7474 696e 6773  t_paint_settings
+00353500: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+00353510: 6965 7733 645f 746f 6f6c 6261 722e 5649  iew3d_toolbar.VI
+00353520: 4557 3344 5f50 545f 746f 6f6c 735f 6772  EW3D_PT_tools_gr
+00353530: 6561 7365 5f70 656e 6369 6c5f 7765 6967  ease_pencil_weig
+00353540: 6874 5f70 6169 6e74 5f73 6574 7469 6e67  ht_paint_setting
+00353550: 7327 203d 204e 6f6e 650a 0a56 4945 5733  s' = None..VIEW3
+00353560: 445f 5054 5f74 6f6f 6c73 5f69 6d61 6765  D_PT_tools_image
+00353570: 7061 696e 745f 6f70 7469 6f6e 733a 2027  paint_options: '
+00353580: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
+00353590: 3364 5f74 6f6f 6c62 6172 2e56 4945 5733  3d_toolbar.VIEW3
+003535a0: 445f 5054 5f74 6f6f 6c73 5f69 6d61 6765  D_PT_tools_image
+003535b0: 7061 696e 745f 6f70 7469 6f6e 7327 203d  paint_options' =
+003535c0: 204e 6f6e 650a 0a56 4945 5733 445f 5054   None..VIEW3D_PT
+003535d0: 5f74 6f6f 6c73 5f69 6d61 6765 7061 696e  _tools_imagepain
+003535e0: 745f 6f70 7469 6f6e 735f 6361 7669 7479  t_options_cavity
+003535f0: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+00353600: 6965 7733 645f 746f 6f6c 6261 722e 5649  iew3d_toolbar.VI
+00353610: 4557 3344 5f50 545f 746f 6f6c 735f 696d  EW3D_PT_tools_im
+00353620: 6167 6570 6169 6e74 5f6f 7074 696f 6e73  agepaint_options
+00353630: 5f63 6176 6974 7927 203d 204e 6f6e 650a  _cavity' = None.
+00353640: 0a56 4945 5733 445f 5054 5f74 6f6f 6c73  .VIEW3D_PT_tools
+00353650: 5f69 6d61 6765 7061 696e 745f 6f70 7469  _imagepaint_opti
+00353660: 6f6e 735f 6578 7465 726e 616c 3a20 2762  ons_external: 'b
+00353670: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+00353680: 645f 746f 6f6c 6261 722e 5649 4557 3344  d_toolbar.VIEW3D
+00353690: 5f50 545f 746f 6f6c 735f 696d 6167 6570  _PT_tools_imagep
+003536a0: 6169 6e74 5f6f 7074 696f 6e73 5f65 7874  aint_options_ext
+003536b0: 6572 6e61 6c27 203d 204e 6f6e 650a 0a56  ernal' = None..V
+003536c0: 4945 5733 445f 5054 5f74 6f6f 6c73 5f69  IEW3D_PT_tools_i
+003536d0: 6d61 6765 7061 696e 745f 7379 6d6d 6574  magepaint_symmet
+003536e0: 7279 3a20 2762 6c5f 7569 2e73 7061 6365  ry: 'bl_ui.space
+003536f0: 5f76 6965 7733 645f 746f 6f6c 6261 722e  _view3d_toolbar.
+00353700: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
+00353710: 696d 6167 6570 6169 6e74 5f73 796d 6d65  imagepaint_symme
+00353720: 7472 7927 203d 204e 6f6e 650a 0a56 4945  try' = None..VIE
+00353730: 5733 445f 5054 5f74 6f6f 6c73 5f6d 6173  W3D_PT_tools_mas
+00353740: 6b5f 7465 7874 7572 653a 2027 626c 5f75  k_texture: 'bl_u
+00353750: 692e 7370 6163 655f 7669 6577 3364 5f74  i.space_view3d_t
+00353760: 6f6f 6c62 6172 2e56 4945 5733 445f 5054  oolbar.VIEW3D_PT
+00353770: 5f74 6f6f 6c73 5f6d 6173 6b5f 7465 7874  _tools_mask_text
+00353780: 7572 6527 203d 204e 6f6e 650a 0a56 4945  ure' = None..VIE
+00353790: 5733 445f 5054 5f74 6f6f 6c73 5f6d 6573  W3D_PT_tools_mes
+003537a0: 6865 6469 745f 6f70 7469 6f6e 733a 2027  hedit_options: '
+003537b0: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
+003537c0: 3364 5f74 6f6f 6c62 6172 2e56 4945 5733  3d_toolbar.VIEW3
+003537d0: 445f 5054 5f74 6f6f 6c73 5f6d 6573 6865  D_PT_tools_meshe
+003537e0: 6469 745f 6f70 7469 6f6e 7327 203d 204e  dit_options' = N
+003537f0: 6f6e 650a 0a56 4945 5733 445f 5054 5f74  one..VIEW3D_PT_t
+00353800: 6f6f 6c73 5f6d 6573 6865 6469 745f 6f70  ools_meshedit_op
+00353810: 7469 6f6e 735f 7472 616e 7366 6f72 6d3a  tions_transform:
+00353820: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+00353830: 6577 3364 5f74 6f6f 6c62 6172 2e56 4945  ew3d_toolbar.VIE
+00353840: 5733 445f 5054 5f74 6f6f 6c73 5f6d 6573  W3D_PT_tools_mes
+00353850: 6865 6469 745f 6f70 7469 6f6e 735f 7472  hedit_options_tr
+00353860: 616e 7366 6f72 6d27 203d 204e 6f6e 650a  ansform' = None.
+00353870: 0a56 4945 5733 445f 5054 5f74 6f6f 6c73  .VIEW3D_PT_tools
+00353880: 5f6d 6573 6865 6469 745f 6f70 7469 6f6e  _meshedit_option
+00353890: 735f 7576 733a 2027 626c 5f75 692e 7370  s_uvs: 'bl_ui.sp
+003538a0: 6163 655f 7669 6577 3364 5f74 6f6f 6c62  ace_view3d_toolb
+003538b0: 6172 2e56 4945 5733 445f 5054 5f74 6f6f  ar.VIEW3D_PT_too
+003538c0: 6c73 5f6d 6573 6865 6469 745f 6f70 7469  ls_meshedit_opti
+003538d0: 6f6e 735f 7576 7327 203d 204e 6f6e 650a  ons_uvs' = None.
+003538e0: 0a56 4945 5733 445f 5054 5f74 6f6f 6c73  .VIEW3D_PT_tools
+003538f0: 5f6f 626a 6563 745f 6f70 7469 6f6e 733a  _object_options:
+00353900: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+00353910: 6577 3364 5f74 6f6f 6c62 6172 2e56 4945  ew3d_toolbar.VIE
+00353920: 5733 445f 5054 5f74 6f6f 6c73 5f6f 626a  W3D_PT_tools_obj
+00353930: 6563 745f 6f70 7469 6f6e 7327 203d 204e  ect_options' = N
+00353940: 6f6e 650a 0a56 4945 5733 445f 5054 5f74  one..VIEW3D_PT_t
+00353950: 6f6f 6c73 5f6f 626a 6563 745f 6f70 7469  ools_object_opti
+00353960: 6f6e 735f 7472 616e 7366 6f72 6d3a 2027  ons_transform: '
+00353970: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
+00353980: 3364 5f74 6f6f 6c62 6172 2e56 4945 5733  3d_toolbar.VIEW3
+00353990: 445f 5054 5f74 6f6f 6c73 5f6f 626a 6563  D_PT_tools_objec
+003539a0: 745f 6f70 7469 6f6e 735f 7472 616e 7366  t_options_transf
+003539b0: 6f72 6d27 203d 204e 6f6e 650a 0a56 4945  orm' = None..VIE
+003539c0: 5733 445f 5054 5f74 6f6f 6c73 5f70 6172  W3D_PT_tools_par
+003539d0: 7469 636c 656d 6f64 653a 2027 626c 5f75  ticlemode: 'bl_u
+003539e0: 692e 7370 6163 655f 7669 6577 3364 5f74  i.space_view3d_t
+003539f0: 6f6f 6c62 6172 2e56 4945 5733 445f 5054  oolbar.VIEW3D_PT
+00353a00: 5f74 6f6f 6c73 5f70 6172 7469 636c 656d  _tools_particlem
+00353a10: 6f64 6527 203d 204e 6f6e 650a 0a56 4945  ode' = None..VIE
+00353a20: 5733 445f 5054 5f74 6f6f 6c73 5f70 6172  W3D_PT_tools_par
+00353a30: 7469 636c 656d 6f64 655f 6f70 7469 6f6e  ticlemode_option
+00353a40: 733a 2027 626c 5f75 692e 7370 6163 655f  s: 'bl_ui.space_
+00353a50: 7669 6577 3364 5f74 6f6f 6c62 6172 2e56  view3d_toolbar.V
+00353a60: 4945 5733 445f 5054 5f74 6f6f 6c73 5f70  IEW3D_PT_tools_p
+00353a70: 6172 7469 636c 656d 6f64 655f 6f70 7469  articlemode_opti
+00353a80: 6f6e 7327 203d 204e 6f6e 650a 0a56 4945  ons' = None..VIE
+00353a90: 5733 445f 5054 5f74 6f6f 6c73 5f70 6172  W3D_PT_tools_par
+00353aa0: 7469 636c 656d 6f64 655f 6f70 7469 6f6e  ticlemode_option
+00353ab0: 735f 6469 7370 6c61 793a 2027 626c 5f75  s_display: 'bl_u
+00353ac0: 692e 7370 6163 655f 7669 6577 3364 5f74  i.space_view3d_t
+00353ad0: 6f6f 6c62 6172 2e56 4945 5733 445f 5054  oolbar.VIEW3D_PT
+00353ae0: 5f74 6f6f 6c73 5f70 6172 7469 636c 656d  _tools_particlem
+00353af0: 6f64 655f 6f70 7469 6f6e 735f 6469 7370  ode_options_disp
+00353b00: 6c61 7927 203d 204e 6f6e 650a 0a56 4945  lay' = None..VIE
+00353b10: 5733 445f 5054 5f74 6f6f 6c73 5f70 6172  W3D_PT_tools_par
+00353b20: 7469 636c 656d 6f64 655f 6f70 7469 6f6e  ticlemode_option
+00353b30: 735f 7368 6170 6563 7574 3a20 2762 6c5f  s_shapecut: 'bl_
+00353b40: 7569 2e73 7061 6365 5f76 6965 7733 645f  ui.space_view3d_
+00353b50: 746f 6f6c 6261 722e 5649 4557 3344 5f50  toolbar.VIEW3D_P
+00353b60: 545f 746f 6f6c 735f 7061 7274 6963 6c65  T_tools_particle
+00353b70: 6d6f 6465 5f6f 7074 696f 6e73 5f73 6861  mode_options_sha
+00353b80: 7065 6375 7427 203d 204e 6f6e 650a 0a56  pecut' = None..V
+00353b90: 4945 5733 445f 5054 5f74 6f6f 6c73 5f70  IEW3D_PT_tools_p
+00353ba0: 6f73 656d 6f64 655f 6f70 7469 6f6e 733a  osemode_options:
+00353bb0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+00353bc0: 6577 3364 5f74 6f6f 6c62 6172 2e56 4945  ew3d_toolbar.VIE
+00353bd0: 5733 445f 5054 5f74 6f6f 6c73 5f70 6f73  W3D_PT_tools_pos
+00353be0: 656d 6f64 655f 6f70 7469 6f6e 7327 203d  emode_options' =
+00353bf0: 204e 6f6e 650a 0a56 4945 5733 445f 5054   None..VIEW3D_PT
+00353c00: 5f74 6f6f 6c73 5f76 6572 7465 7870 6169  _tools_vertexpai
+00353c10: 6e74 5f6f 7074 696f 6e73 3a20 2762 6c5f  nt_options: 'bl_
+00353c20: 7569 2e73 7061 6365 5f76 6965 7733 645f  ui.space_view3d_
+00353c30: 746f 6f6c 6261 722e 5649 4557 3344 5f50  toolbar.VIEW3D_P
+00353c40: 545f 746f 6f6c 735f 7665 7274 6578 7061  T_tools_vertexpa
+00353c50: 696e 745f 6f70 7469 6f6e 7327 203d 204e  int_options' = N
+00353c60: 6f6e 650a 0a56 4945 5733 445f 5054 5f74  one..VIEW3D_PT_t
+00353c70: 6f6f 6c73 5f76 6572 7465 7870 6169 6e74  ools_vertexpaint
+00353c80: 5f73 796d 6d65 7472 793a 2027 626c 5f75  _symmetry: 'bl_u
+00353c90: 692e 7370 6163 655f 7669 6577 3364 5f74  i.space_view3d_t
+00353ca0: 6f6f 6c62 6172 2e56 4945 5733 445f 5054  oolbar.VIEW3D_PT
+00353cb0: 5f74 6f6f 6c73 5f76 6572 7465 7870 6169  _tools_vertexpai
+00353cc0: 6e74 5f73 796d 6d65 7472 7927 203d 204e  nt_symmetry' = N
+00353cd0: 6f6e 650a 0a56 4945 5733 445f 5054 5f74  one..VIEW3D_PT_t
+00353ce0: 6f6f 6c73 5f76 6572 7465 7870 6169 6e74  ools_vertexpaint
+00353cf0: 5f73 796d 6d65 7472 795f 666f 725f 746f  _symmetry_for_to
+00353d00: 7062 6172 3a20 2762 6c5f 7569 2e73 7061  pbar: 'bl_ui.spa
+00353d10: 6365 5f76 6965 7733 645f 746f 6f6c 6261  ce_view3d_toolba
+00353d20: 722e 5649 4557 3344 5f50 545f 746f 6f6c  r.VIEW3D_PT_tool
+00353d30: 735f 7665 7274 6578 7061 696e 745f 7379  s_vertexpaint_sy
+00353d40: 6d6d 6574 7279 5f66 6f72 5f74 6f70 6261  mmetry_for_topba
+00353d50: 7227 203d 204e 6f6e 650a 0a56 4945 5733  r' = None..VIEW3
+00353d60: 445f 5054 5f74 6f6f 6c73 5f77 6569 6768  D_PT_tools_weigh
+00353d70: 745f 6772 6164 6965 6e74 3a20 2762 6c5f  t_gradient: 'bl_
+00353d80: 7569 2e73 7061 6365 5f76 6965 7733 645f  ui.space_view3d_
+00353d90: 746f 6f6c 6261 722e 5649 4557 3344 5f50  toolbar.VIEW3D_P
+00353da0: 545f 746f 6f6c 735f 7765 6967 6874 5f67  T_tools_weight_g
+00353db0: 7261 6469 656e 7427 203d 204e 6f6e 650a  radient' = None.
+00353dc0: 0a56 4945 5733 445f 5054 5f74 6f6f 6c73  .VIEW3D_PT_tools
+00353dd0: 5f77 6569 6768 7470 6169 6e74 5f6f 7074  _weightpaint_opt
+00353de0: 696f 6e73 3a20 2762 6c5f 7569 2e73 7061  ions: 'bl_ui.spa
+00353df0: 6365 5f76 6965 7733 645f 746f 6f6c 6261  ce_view3d_toolba
+00353e00: 722e 5649 4557 3344 5f50 545f 746f 6f6c  r.VIEW3D_PT_tool
+00353e10: 735f 7765 6967 6874 7061 696e 745f 6f70  s_weightpaint_op
+00353e20: 7469 6f6e 7327 203d 204e 6f6e 650a 0a56  tions' = None..V
+00353e30: 4945 5733 445f 5054 5f74 6f6f 6c73 5f77  IEW3D_PT_tools_w
+00353e40: 6569 6768 7470 6169 6e74 5f73 796d 6d65  eightpaint_symme
+00353e50: 7472 793a 2027 626c 5f75 692e 7370 6163  try: 'bl_ui.spac
+00353e60: 655f 7669 6577 3364 5f74 6f6f 6c62 6172  e_view3d_toolbar
+00353e70: 2e56 4945 5733 445f 5054 5f74 6f6f 6c73  .VIEW3D_PT_tools
+00353e80: 5f77 6569 6768 7470 6169 6e74 5f73 796d  _weightpaint_sym
+00353e90: 6d65 7472 7927 203d 204e 6f6e 650a 0a56  metry' = None..V
+00353ea0: 4945 5733 445f 5054 5f74 6f6f 6c73 5f77  IEW3D_PT_tools_w
+00353eb0: 6569 6768 7470 6169 6e74 5f73 796d 6d65  eightpaint_symme
+00353ec0: 7472 795f 666f 725f 746f 7062 6172 3a20  try_for_topbar: 
+00353ed0: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
+00353ee0: 7733 645f 746f 6f6c 6261 722e 5649 4557  w3d_toolbar.VIEW
+00353ef0: 3344 5f50 545f 746f 6f6c 735f 7765 6967  3D_PT_tools_weig
+00353f00: 6874 7061 696e 745f 7379 6d6d 6574 7279  htpaint_symmetry
+00353f10: 5f66 6f72 5f74 6f70 6261 7227 203d 204e  _for_topbar' = N
+00353f20: 6f6e 650a 0a56 4945 5733 445f 5054 5f74  one..VIEW3D_PT_t
+00353f30: 7261 6e73 666f 726d 5f6f 7269 656e 7461  ransform_orienta
+00353f40: 7469 6f6e 733a 2027 626c 5f75 692e 7370  tions: 'bl_ui.sp
+00353f50: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
+00353f60: 445f 5054 5f74 7261 6e73 666f 726d 5f6f  D_PT_transform_o
+00353f70: 7269 656e 7461 7469 6f6e 7327 203d 204e  rientations' = N
+00353f80: 6f6e 650a 0a56 4945 5733 445f 5054 5f76  one..VIEW3D_PT_v
+00353f90: 6965 7733 645f 6375 7273 6f72 3a20 2762  iew3d_cursor: 'b
+00353fa0: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+00353fb0: 642e 5649 4557 3344 5f50 545f 7669 6577  d.VIEW3D_PT_view
+00353fc0: 3364 5f63 7572 736f 7227 203d 204e 6f6e  3d_cursor' = Non
+00353fd0: 650a 0a56 4945 5733 445f 5054 5f76 6965  e..VIEW3D_PT_vie
+00353fe0: 7733 645f 6c6f 636b 3a20 2762 6c5f 7569  w3d_lock: 'bl_ui
+00353ff0: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
+00354000: 4557 3344 5f50 545f 7669 6577 3364 5f6c  EW3D_PT_view3d_l
+00354010: 6f63 6b27 203d 204e 6f6e 650a 0a56 4945  ock' = None..VIE
+00354020: 5733 445f 5054 5f76 6965 7733 645f 7072  W3D_PT_view3d_pr
+00354030: 6f70 6572 7469 6573 3a20 2762 6c5f 7569  operties: 'bl_ui
+00354040: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
+00354050: 4557 3344 5f50 545f 7669 6577 3364 5f70  EW3D_PT_view3d_p
+00354060: 726f 7065 7274 6965 7327 203d 204e 6f6e  roperties' = Non
+00354070: 650a 0a56 4945 5733 445f 5054 5f76 6965  e..VIEW3D_PT_vie
+00354080: 7733 645f 7374 6572 656f 3a20 2762 6c5f  w3d_stereo: 'bl_
+00354090: 7569 2e73 7061 6365 5f76 6965 7733 642e  ui.space_view3d.
+003540a0: 5649 4557 3344 5f50 545f 7669 6577 3364  VIEW3D_PT_view3d
+003540b0: 5f73 7465 7265 6f27 203d 204e 6f6e 650a  _stereo' = None.
+003540c0: 0a56 4945 5733 445f 5054 5f76 6965 7770  .VIEW3D_PT_viewp
+003540d0: 6f72 745f 6465 6275 673a 2027 626c 5f75  ort_debug: 'bl_u
+003540e0: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
+003540f0: 4945 5733 445f 5054 5f76 6965 7770 6f72  IEW3D_PT_viewpor
+00354100: 745f 6465 6275 6727 203d 204e 6f6e 650a  t_debug' = None.
+00354110: 0a56 4945 574c 4159 4552 5f4d 545f 6c69  .VIEWLAYER_MT_li
+00354120: 6768 7467 726f 7570 5f73 796e 633a 2027  ghtgroup_sync: '
+00354130: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+00354140: 5f76 6965 775f 6c61 7965 722e 5649 4557  _view_layer.VIEW
+00354150: 4c41 5945 525f 4d54 5f6c 6967 6874 6772  LAYER_MT_lightgr
+00354160: 6f75 705f 7379 6e63 2720 3d20 4e6f 6e65  oup_sync' = None
+00354170: 0a0a 5649 4557 4c41 5945 525f 5054 5f65  ..VIEWLAYER_PT_e
+00354180: 6576 6565 5f6c 6179 6572 5f70 6173 7365  evee_layer_passe
+00354190: 735f 6461 7461 3a20 2762 6c5f 7569 2e70  s_data: 'bl_ui.p
+003541a0: 726f 7065 7274 6965 735f 7669 6577 5f6c  roperties_view_l
+003541b0: 6179 6572 2e56 4945 574c 4159 4552 5f50  ayer.VIEWLAYER_P
+003541c0: 545f 6565 7665 655f 6c61 7965 725f 7061  T_eevee_layer_pa
+003541d0: 7373 6573 5f64 6174 6127 203d 204e 6f6e  sses_data' = Non
+003541e0: 650a 0a56 4945 574c 4159 4552 5f50 545f  e..VIEWLAYER_PT_
+003541f0: 6565 7665 655f 6c61 7965 725f 7061 7373  eevee_layer_pass
+00354200: 6573 5f65 6666 6563 7473 3a20 2762 6c5f  es_effects: 'bl_
+00354210: 7569 2e70 726f 7065 7274 6965 735f 7669  ui.properties_vi
+00354220: 6577 5f6c 6179 6572 2e56 4945 574c 4159  ew_layer.VIEWLAY
+00354230: 4552 5f50 545f 6565 7665 655f 6c61 7965  ER_PT_eevee_laye
+00354240: 725f 7061 7373 6573 5f65 6666 6563 7473  r_passes_effects
+00354250: 2720 3d20 4e6f 6e65 0a0a 5649 4557 4c41  ' = None..VIEWLA
+00354260: 5945 525f 5054 5f65 6576 6565 5f6c 6179  YER_PT_eevee_lay
+00354270: 6572 5f70 6173 7365 735f 6c69 6768 743a  er_passes_light:
+00354280: 2027 626c 5f75 692e 7072 6f70 6572 7469   'bl_ui.properti
+00354290: 6573 5f76 6965 775f 6c61 7965 722e 5649  es_view_layer.VI
+003542a0: 4557 4c41 5945 525f 5054 5f65 6576 6565  EWLAYER_PT_eevee
+003542b0: 5f6c 6179 6572 5f70 6173 7365 735f 6c69  _layer_passes_li
+003542c0: 6768 7427 203d 204e 6f6e 650a 0a56 4945  ght' = None..VIE
+003542d0: 574c 4159 4552 5f50 545f 6565 7665 655f  WLAYER_PT_eevee_
+003542e0: 6e65 7874 5f6c 6179 6572 5f70 6173 7365  next_layer_passe
+003542f0: 735f 6461 7461 3a20 2762 6c5f 7569 2e70  s_data: 'bl_ui.p
+00354300: 726f 7065 7274 6965 735f 7669 6577 5f6c  roperties_view_l
+00354310: 6179 6572 2e56 4945 574c 4159 4552 5f50  ayer.VIEWLAYER_P
+00354320: 545f 6565 7665 655f 6e65 7874 5f6c 6179  T_eevee_next_lay
+00354330: 6572 5f70 6173 7365 735f 6461 7461 2720  er_passes_data' 
+00354340: 3d20 4e6f 6e65 0a0a 5649 4557 4c41 5945  = None..VIEWLAYE
+00354350: 525f 5054 5f66 7265 6573 7479 6c65 3a20  R_PT_freestyle: 
+00354360: 2762 6c5f 7569 2e70 726f 7065 7274 6965  'bl_ui.propertie
+00354370: 735f 6672 6565 7374 796c 652e 5649 4557  s_freestyle.VIEW
+00354380: 4c41 5945 525f 5054 5f66 7265 6573 7479  LAYER_PT_freesty
+00354390: 6c65 2720 3d20 4e6f 6e65 0a0a 5649 4557  le' = None..VIEW
+003543a0: 4c41 5945 525f 5054 5f66 7265 6573 7479  LAYER_PT_freesty
+003543b0: 6c65 5f65 6467 655f 6465 7465 6374 696f  le_edge_detectio
+003543c0: 6e3a 2027 626c 5f75 692e 7072 6f70 6572  n: 'bl_ui.proper
+003543d0: 7469 6573 5f66 7265 6573 7479 6c65 2e56  ties_freestyle.V
+003543e0: 4945 574c 4159 4552 5f50 545f 6672 6565  IEWLAYER_PT_free
+003543f0: 7374 796c 655f 6564 6765 5f64 6574 6563  style_edge_detec
+00354400: 7469 6f6e 2720 3d20 4e6f 6e65 0a0a 5649  tion' = None..VI
+00354410: 4557 4c41 5945 525f 5054 5f66 7265 6573  EWLAYER_PT_frees
+00354420: 7479 6c65 5f6c 696e 6573 6574 3a20 2762  tyle_lineset: 'b
+00354430: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
+00354440: 6672 6565 7374 796c 652e 5649 4557 4c41  freestyle.VIEWLA
+00354450: 5945 525f 5054 5f66 7265 6573 7479 6c65  YER_PT_freestyle
+00354460: 5f6c 696e 6573 6574 2720 3d20 4e6f 6e65  _lineset' = None
+00354470: 0a0a 5649 4557 4c41 5945 525f 5054 5f66  ..VIEWLAYER_PT_f
+00354480: 7265 6573 7479 6c65 5f6c 696e 6573 6574  reestyle_lineset
+00354490: 5f63 6f6c 6c65 6374 696f 6e3a 2027 626c  _collection: 'bl
+003544a0: 5f75 692e 7072 6f70 6572 7469 6573 5f66  _ui.properties_f
+003544b0: 7265 6573 7479 6c65 2e56 4945 574c 4159  reestyle.VIEWLAY
+003544c0: 4552 5f50 545f 6672 6565 7374 796c 655f  ER_PT_freestyle_
+003544d0: 6c69 6e65 7365 745f 636f 6c6c 6563 7469  lineset_collecti
+003544e0: 6f6e 2720 3d20 4e6f 6e65 0a0a 5649 4557  on' = None..VIEW
+003544f0: 4c41 5945 525f 5054 5f66 7265 6573 7479  LAYER_PT_freesty
+00354500: 6c65 5f6c 696e 6573 6574 5f65 6467 6574  le_lineset_edget
+00354510: 7970 653a 2027 626c 5f75 692e 7072 6f70  ype: 'bl_ui.prop
+00354520: 6572 7469 6573 5f66 7265 6573 7479 6c65  erties_freestyle
+00354530: 2e56 4945 574c 4159 4552 5f50 545f 6672  .VIEWLAYER_PT_fr
+00354540: 6565 7374 796c 655f 6c69 6e65 7365 745f  eestyle_lineset_
+00354550: 6564 6765 7479 7065 2720 3d20 4e6f 6e65  edgetype' = None
+00354560: 0a0a 5649 4557 4c41 5945 525f 5054 5f66  ..VIEWLAYER_PT_f
+00354570: 7265 6573 7479 6c65 5f6c 696e 6573 6574  reestyle_lineset
+00354580: 5f66 6163 656d 6172 6b73 3a20 2762 6c5f  _facemarks: 'bl_
+00354590: 7569 2e70 726f 7065 7274 6965 735f 6672  ui.properties_fr
+003545a0: 6565 7374 796c 652e 5649 4557 4c41 5945  eestyle.VIEWLAYE
+003545b0: 525f 5054 5f66 7265 6573 7479 6c65 5f6c  R_PT_freestyle_l
+003545c0: 696e 6573 6574 5f66 6163 656d 6172 6b73  ineset_facemarks
+003545d0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 4c41  ' = None..VIEWLA
+003545e0: 5945 525f 5054 5f66 7265 6573 7479 6c65  YER_PT_freestyle
+003545f0: 5f6c 696e 6573 6574 5f76 6973 6962 696c  _lineset_visibil
+00354600: 7479 3a20 2762 6c5f 7569 2e70 726f 7065  ty: 'bl_ui.prope
+00354610: 7274 6965 735f 6672 6565 7374 796c 652e  rties_freestyle.
+00354620: 5649 4557 4c41 5945 525f 5054 5f66 7265  VIEWLAYER_PT_fre
+00354630: 6573 7479 6c65 5f6c 696e 6573 6574 5f76  estyle_lineset_v
+00354640: 6973 6962 696c 7479 2720 3d20 4e6f 6e65  isibilty' = None
+00354650: 0a0a 5649 4557 4c41 5945 525f 5054 5f66  ..VIEWLAYER_PT_f
+00354660: 7265 6573 7479 6c65 5f6c 696e 6573 7479  reestyle_linesty
+00354670: 6c65 5f61 6c70 6861 3a20 2762 6c5f 7569  le_alpha: 'bl_ui
+00354680: 2e70 726f 7065 7274 6965 735f 6672 6565  .properties_free
+00354690: 7374 796c 652e 5649 4557 4c41 5945 525f  style.VIEWLAYER_
+003546a0: 5054 5f66 7265 6573 7479 6c65 5f6c 696e  PT_freestyle_lin
+003546b0: 6573 7479 6c65 5f61 6c70 6861 2720 3d20  estyle_alpha' = 
+003546c0: 4e6f 6e65 0a0a 5649 4557 4c41 5945 525f  None..VIEWLAYER_
+003546d0: 5054 5f66 7265 6573 7479 6c65 5f6c 696e  PT_freestyle_lin
+003546e0: 6573 7479 6c65 5f63 6f6c 6f72 3a20 2762  estyle_color: 'b
+003546f0: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
+00354700: 6672 6565 7374 796c 652e 5649 4557 4c41  freestyle.VIEWLA
+00354710: 5945 525f 5054 5f66 7265 6573 7479 6c65  YER_PT_freestyle
+00354720: 5f6c 696e 6573 7479 6c65 5f63 6f6c 6f72  _linestyle_color
+00354730: 2720 3d20 4e6f 6e65 0a0a 5649 4557 4c41  ' = None..VIEWLA
+00354740: 5945 525f 5054 5f66 7265 6573 7479 6c65  YER_PT_freestyle
+00354750: 5f6c 696e 6573 7479 6c65 5f67 656f 6d65  _linestyle_geome
+00354760: 7472 793a 2027 626c 5f75 692e 7072 6f70  try: 'bl_ui.prop
+00354770: 6572 7469 6573 5f66 7265 6573 7479 6c65  erties_freestyle
+00354780: 2e56 4945 574c 4159 4552 5f50 545f 6672  .VIEWLAYER_PT_fr
+00354790: 6565 7374 796c 655f 6c69 6e65 7374 796c  eestyle_linestyl
+003547a0: 655f 6765 6f6d 6574 7279 2720 3d20 4e6f  e_geometry' = No
+003547b0: 6e65 0a0a 5649 4557 4c41 5945 525f 5054  ne..VIEWLAYER_PT
+003547c0: 5f66 7265 6573 7479 6c65 5f6c 696e 6573  _freestyle_lines
+003547d0: 7479 6c65 5f73 7472 6f6b 6573 3a20 2762  tyle_strokes: 'b
+003547e0: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
+003547f0: 6672 6565 7374 796c 652e 5649 4557 4c41  freestyle.VIEWLA
+00354800: 5945 525f 5054 5f66 7265 6573 7479 6c65  YER_PT_freestyle
+00354810: 5f6c 696e 6573 7479 6c65 5f73 7472 6f6b  _linestyle_strok
+00354820: 6573 2720 3d20 4e6f 6e65 0a0a 5649 4557  es' = None..VIEW
+00354830: 4c41 5945 525f 5054 5f66 7265 6573 7479  LAYER_PT_freesty
+00354840: 6c65 5f6c 696e 6573 7479 6c65 5f73 7472  le_linestyle_str
+00354850: 6f6b 6573 5f63 6861 696e 696e 673a 2027  okes_chaining: '
+00354860: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+00354870: 5f66 7265 6573 7479 6c65 2e56 4945 574c  _freestyle.VIEWL
+00354880: 4159 4552 5f50 545f 6672 6565 7374 796c  AYER_PT_freestyl
+00354890: 655f 6c69 6e65 7374 796c 655f 7374 726f  e_linestyle_stro
+003548a0: 6b65 735f 6368 6169 6e69 6e67 2720 3d20  kes_chaining' = 
+003548b0: 4e6f 6e65 0a0a 5649 4557 4c41 5945 525f  None..VIEWLAYER_
+003548c0: 5054 5f66 7265 6573 7479 6c65 5f6c 696e  PT_freestyle_lin
+003548d0: 6573 7479 6c65 5f73 7472 6f6b 6573 5f64  estyle_strokes_d
+003548e0: 6173 6865 646c 696e 653a 2027 626c 5f75  ashedline: 'bl_u
+003548f0: 692e 7072 6f70 6572 7469 6573 5f66 7265  i.properties_fre
+00354900: 6573 7479 6c65 2e56 4945 574c 4159 4552  estyle.VIEWLAYER
+00354910: 5f50 545f 6672 6565 7374 796c 655f 6c69  _PT_freestyle_li
+00354920: 6e65 7374 796c 655f 7374 726f 6b65 735f  nestyle_strokes_
+00354930: 6461 7368 6564 6c69 6e65 2720 3d20 4e6f  dashedline' = No
+00354940: 6e65 0a0a 5649 4557 4c41 5945 525f 5054  ne..VIEWLAYER_PT
+00354950: 5f66 7265 6573 7479 6c65 5f6c 696e 6573  _freestyle_lines
+00354960: 7479 6c65 5f73 7472 6f6b 6573 5f73 656c  tyle_strokes_sel
+00354970: 6563 7469 6f6e 3a20 2762 6c5f 7569 2e70  ection: 'bl_ui.p
+00354980: 726f 7065 7274 6965 735f 6672 6565 7374  roperties_freest
+00354990: 796c 652e 5649 4557 4c41 5945 525f 5054  yle.VIEWLAYER_PT
+003549a0: 5f66 7265 6573 7479 6c65 5f6c 696e 6573  _freestyle_lines
+003549b0: 7479 6c65 5f73 7472 6f6b 6573 5f73 656c  tyle_strokes_sel
+003549c0: 6563 7469 6f6e 2720 3d20 4e6f 6e65 0a0a  ection' = None..
+003549d0: 5649 4557 4c41 5945 525f 5054 5f66 7265  VIEWLAYER_PT_fre
+003549e0: 6573 7479 6c65 5f6c 696e 6573 7479 6c65  estyle_linestyle
+003549f0: 5f73 7472 6f6b 6573 5f73 6f72 7469 6e67  _strokes_sorting
+00354a00: 3a20 2762 6c5f 7569 2e70 726f 7065 7274  : 'bl_ui.propert
+00354a10: 6965 735f 6672 6565 7374 796c 652e 5649  ies_freestyle.VI
+00354a20: 4557 4c41 5945 525f 5054 5f66 7265 6573  EWLAYER_PT_frees
+00354a30: 7479 6c65 5f6c 696e 6573 7479 6c65 5f73  tyle_linestyle_s
+00354a40: 7472 6f6b 6573 5f73 6f72 7469 6e67 2720  trokes_sorting' 
+00354a50: 3d20 4e6f 6e65 0a0a 5649 4557 4c41 5945  = None..VIEWLAYE
+00354a60: 525f 5054 5f66 7265 6573 7479 6c65 5f6c  R_PT_freestyle_l
+00354a70: 696e 6573 7479 6c65 5f73 7472 6f6b 6573  inestyle_strokes
+00354a80: 5f73 706c 6974 7469 6e67 3a20 2762 6c5f  _splitting: 'bl_
+00354a90: 7569 2e70 726f 7065 7274 6965 735f 6672  ui.properties_fr
+00354aa0: 6565 7374 796c 652e 5649 4557 4c41 5945  eestyle.VIEWLAYE
+00354ab0: 525f 5054 5f66 7265 6573 7479 6c65 5f6c  R_PT_freestyle_l
+00354ac0: 696e 6573 7479 6c65 5f73 7472 6f6b 6573  inestyle_strokes
+00354ad0: 5f73 706c 6974 7469 6e67 2720 3d20 4e6f  _splitting' = No
+00354ae0: 6e65 0a0a 5649 4557 4c41 5945 525f 5054  ne..VIEWLAYER_PT
+00354af0: 5f66 7265 6573 7479 6c65 5f6c 696e 6573  _freestyle_lines
+00354b00: 7479 6c65 5f73 7472 6f6b 6573 5f73 706c  tyle_strokes_spl
+00354b10: 6974 7469 6e67 5f70 6174 7465 726e 3a20  itting_pattern: 
+00354b20: 2762 6c5f 7569 2e70 726f 7065 7274 6965  'bl_ui.propertie
+00354b30: 735f 6672 6565 7374 796c 652e 5649 4557  s_freestyle.VIEW
+00354b40: 4c41 5945 525f 5054 5f66 7265 6573 7479  LAYER_PT_freesty
+00354b50: 6c65 5f6c 696e 6573 7479 6c65 5f73 7472  le_linestyle_str
+00354b60: 6f6b 6573 5f73 706c 6974 7469 6e67 5f70  okes_splitting_p
+00354b70: 6174 7465 726e 2720 3d20 4e6f 6e65 0a0a  attern' = None..
+00354b80: 5649 4557 4c41 5945 525f 5054 5f66 7265  VIEWLAYER_PT_fre
+00354b90: 6573 7479 6c65 5f6c 696e 6573 7479 6c65  estyle_linestyle
+00354ba0: 5f74 6578 7475 7265 3a20 2762 6c5f 7569  _texture: 'bl_ui
+00354bb0: 2e70 726f 7065 7274 6965 735f 6672 6565  .properties_free
+00354bc0: 7374 796c 652e 5649 4557 4c41 5945 525f  style.VIEWLAYER_
+00354bd0: 5054 5f66 7265 6573 7479 6c65 5f6c 696e  PT_freestyle_lin
+00354be0: 6573 7479 6c65 5f74 6578 7475 7265 2720  estyle_texture' 
+00354bf0: 3d20 4e6f 6e65 0a0a 5649 4557 4c41 5945  = None..VIEWLAYE
+00354c00: 525f 5054 5f66 7265 6573 7479 6c65 5f6c  R_PT_freestyle_l
+00354c10: 696e 6573 7479 6c65 5f74 6869 636b 6e65  inestyle_thickne
+00354c20: 7373 3a20 2762 6c5f 7569 2e70 726f 7065  ss: 'bl_ui.prope
+00354c30: 7274 6965 735f 6672 6565 7374 796c 652e  rties_freestyle.
+00354c40: 5649 4557 4c41 5945 525f 5054 5f66 7265  VIEWLAYER_PT_fre
+00354c50: 6573 7479 6c65 5f6c 696e 6573 7479 6c65  estyle_linestyle
+00354c60: 5f74 6869 636b 6e65 7373 2720 3d20 4e6f  _thickness' = No
+00354c70: 6e65 0a0a 5649 4557 4c41 5945 525f 5054  ne..VIEWLAYER_PT
+00354c80: 5f66 7265 6573 7479 6c65 5f73 7479 6c65  _freestyle_style
+00354c90: 5f6d 6f64 756c 6573 3a20 2762 6c5f 7569  _modules: 'bl_ui
+00354ca0: 2e70 726f 7065 7274 6965 735f 6672 6565  .properties_free
+00354cb0: 7374 796c 652e 5649 4557 4c41 5945 525f  style.VIEWLAYER_
+00354cc0: 5054 5f66 7265 6573 7479 6c65 5f73 7479  PT_freestyle_sty
+00354cd0: 6c65 5f6d 6f64 756c 6573 2720 3d20 4e6f  le_modules' = No
+00354ce0: 6e65 0a0a 5649 4557 4c41 5945 525f 5054  ne..VIEWLAYER_PT
+00354cf0: 5f6c 6179 6572 3a20 2762 6c5f 7569 2e70  _layer: 'bl_ui.p
 00354d00: 726f 7065 7274 6965 735f 7669 6577 5f6c  roperties_view_l
 00354d10: 6179 6572 2e56 4945 574c 4159 4552 5f50  ayer.VIEWLAYER_P
-00354d20: 545f 6c61 7965 725f 6375 7374 6f6d 5f70  T_layer_custom_p
-00354d30: 726f 7073 2720 3d20 4e6f 6e65 0a0a 5649  rops' = None..VI
-00354d40: 4557 4c41 5945 525f 5054 5f6c 6179 6572  EWLAYER_PT_layer
-00354d50: 5f70 6173 7365 733a 2027 626c 5f75 692e  _passes: 'bl_ui.
-00354d60: 7072 6f70 6572 7469 6573 5f76 6965 775f  properties_view_
-00354d70: 6c61 7965 722e 5649 4557 4c41 5945 525f  layer.VIEWLAYER_
-00354d80: 5054 5f6c 6179 6572 5f70 6173 7365 7327  PT_layer_passes'
-00354d90: 203d 204e 6f6e 650a 0a56 4945 574c 4159   = None..VIEWLAY
-00354da0: 4552 5f50 545f 6c61 7965 725f 7061 7373  ER_PT_layer_pass
-00354db0: 6573 5f61 6f76 3a20 2762 6c5f 7569 2e70  es_aov: 'bl_ui.p
-00354dc0: 726f 7065 7274 6965 735f 7669 6577 5f6c  roperties_view_l
-00354dd0: 6179 6572 2e56 4945 574c 4159 4552 5f50  ayer.VIEWLAYER_P
-00354de0: 545f 6c61 7965 725f 7061 7373 6573 5f61  T_layer_passes_a
-00354df0: 6f76 2720 3d20 4e6f 6e65 0a0a 5649 4557  ov' = None..VIEW
-00354e00: 4c41 5945 525f 5054 5f6c 6179 6572 5f70  LAYER_PT_layer_p
-00354e10: 6173 7365 735f 6372 7970 746f 6d61 7474  asses_cryptomatt
-00354e20: 653a 2027 626c 5f75 692e 7072 6f70 6572  e: 'bl_ui.proper
-00354e30: 7469 6573 5f76 6965 775f 6c61 7965 722e  ties_view_layer.
-00354e40: 5649 4557 4c41 5945 525f 5054 5f6c 6179  VIEWLAYER_PT_lay
-00354e50: 6572 5f70 6173 7365 735f 6372 7970 746f  er_passes_crypto
-00354e60: 6d61 7474 6527 203d 204e 6f6e 650a 0a56  matte' = None..V
-00354e70: 4945 574c 4159 4552 5f50 545f 6c61 7965  IEWLAYER_PT_laye
-00354e80: 725f 7061 7373 6573 5f6c 6967 6874 6772  r_passes_lightgr
-00354e90: 6f75 7073 3a20 2762 6c5f 7569 2e70 726f  oups: 'bl_ui.pro
-00354ea0: 7065 7274 6965 735f 7669 6577 5f6c 6179  perties_view_lay
-00354eb0: 6572 2e56 4945 574c 4159 4552 5f50 545f  er.VIEWLAYER_PT_
-00354ec0: 6c61 7965 725f 7061 7373 6573 5f6c 6967  layer_passes_lig
-00354ed0: 6874 6772 6f75 7073 2720 3d20 4e6f 6e65  htgroups' = None
-00354ee0: 0a0a 5649 4557 4c41 5945 525f 554c 5f61  ..VIEWLAYER_UL_a
-00354ef0: 6f76 3a20 2762 6c5f 7569 2e70 726f 7065  ov: 'bl_ui.prope
-00354f00: 7274 6965 735f 7669 6577 5f6c 6179 6572  rties_view_layer
-00354f10: 2e56 4945 574c 4159 4552 5f55 4c5f 616f  .VIEWLAYER_UL_ao
-00354f20: 7627 203d 204e 6f6e 650a 0a56 4945 574c  v' = None..VIEWL
-00354f30: 4159 4552 5f55 4c5f 6c69 6e65 7365 7473  AYER_UL_linesets
-00354f40: 3a20 2762 6c5f 7569 2e70 726f 7065 7274  : 'bl_ui.propert
-00354f50: 6965 735f 6672 6565 7374 796c 652e 5649  ies_freestyle.VI
-00354f60: 4557 4c41 5945 525f 554c 5f6c 696e 6573  EWLAYER_UL_lines
-00354f70: 6574 7327 203d 204e 6f6e 650a 0a56 4f4c  ets' = None..VOL
-00354f80: 554d 455f 554c 5f67 7269 6473 3a20 2762  UME_UL_grids: 'b
-00354f90: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
-00354fa0: 6461 7461 5f76 6f6c 756d 652e 564f 4c55  data_volume.VOLU
-00354fb0: 4d45 5f55 4c5f 6772 6964 7327 203d 204e  ME_UL_grids' = N
-00354fc0: 6f6e 650a 0a57 4d5f 4d54 5f6f 7065 7261  one..WM_MT_opera
-00354fd0: 746f 725f 7072 6573 6574 733a 2027 626c  tor_presets: 'bl
-00354fe0: 5f6f 7065 7261 746f 7273 2e70 7265 7365  _operators.prese
-00354ff0: 7473 2e57 4d5f 4d54 5f6f 7065 7261 746f  ts.WM_MT_operato
-00355000: 725f 7072 6573 6574 7327 203d 204e 6f6e  r_presets' = Non
-00355010: 650a 0a57 4d5f 4d54 5f73 706c 6173 683a  e..WM_MT_splash:
-00355020: 2027 626c 5f6f 7065 7261 746f 7273 2e77   'bl_operators.w
-00355030: 6d2e 574d 5f4d 545f 7370 6c61 7368 2720  m.WM_MT_splash' 
-00355040: 3d20 4e6f 6e65 0a0a 574d 5f4d 545f 7370  = None..WM_MT_sp
-00355050: 6c61 7368 5f61 626f 7574 3a20 2762 6c5f  lash_about: 'bl_
-00355060: 6f70 6572 6174 6f72 732e 776d 2e57 4d5f  operators.wm.WM_
-00355070: 4d54 5f73 706c 6173 685f 6162 6f75 7427  MT_splash_about'
-00355080: 203d 204e 6f6e 650a 0a57 4d5f 4d54 5f73   = None..WM_MT_s
-00355090: 706c 6173 685f 7175 6963 6b5f 7365 7475  plash_quick_setu
-003550a0: 703a 2027 626c 5f6f 7065 7261 746f 7273  p: 'bl_operators
-003550b0: 2e77 6d2e 574d 5f4d 545f 7370 6c61 7368  .wm.WM_MT_splash
-003550c0: 5f71 7569 636b 5f73 6574 7570 2720 3d20  _quick_setup' = 
-003550d0: 4e6f 6e65 0a0a 574d 5f4d 545f 746f 6f6c  None..WM_MT_tool
-003550e0: 7379 7374 656d 5f73 7562 6d65 6e75 3a20  system_submenu: 
-003550f0: 2762 6c5f 7569 2e73 7061 6365 5f74 6f6f  'bl_ui.space_too
-00355100: 6c73 7973 7465 6d5f 636f 6d6d 6f6e 2e57  lsystem_common.W
-00355110: 4d5f 4d54 5f74 6f6f 6c73 7973 7465 6d5f  M_MT_toolsystem_
-00355120: 7375 626d 656e 7527 203d 204e 6f6e 650a  submenu' = None.
-00355130: 0a57 4d5f 4f54 5f62 6174 6368 5f72 656e  .WM_OT_batch_ren
-00355140: 616d 653a 2027 626c 5f6f 7065 7261 746f  ame: 'bl_operato
-00355150: 7273 2e77 6d2e 574d 5f4f 545f 6261 7463  rs.wm.WM_OT_batc
-00355160: 685f 7265 6e61 6d65 2720 3d20 4e6f 6e65  h_rename' = None
-00355170: 0a0a 574d 5f4f 545f 626c 656e 645f 7374  ..WM_OT_blend_st
-00355180: 7269 6e67 735f 7574 6638 5f76 616c 6964  rings_utf8_valid
-00355190: 6174 653a 2027 626c 5f6f 7065 7261 746f  ate: 'bl_operato
-003551a0: 7273 2e66 696c 652e 574d 5f4f 545f 626c  rs.file.WM_OT_bl
-003551b0: 656e 645f 7374 7269 6e67 735f 7574 6638  end_strings_utf8
-003551c0: 5f76 616c 6964 6174 6527 203d 204e 6f6e  _validate' = Non
-003551d0: 650a 0a57 4d5f 4f54 5f63 6f6e 7465 7874  e..WM_OT_context
-003551e0: 5f63 6f6c 6c65 6374 696f 6e5f 626f 6f6c  _collection_bool
-003551f0: 6561 6e5f 7365 743a 2027 626c 5f6f 7065  ean_set: 'bl_ope
-00355200: 7261 746f 7273 2e77 6d2e 574d 5f4f 545f  rators.wm.WM_OT_
-00355210: 636f 6e74 6578 745f 636f 6c6c 6563 7469  context_collecti
-00355220: 6f6e 5f62 6f6f 6c65 616e 5f73 6574 2720  on_boolean_set' 
-00355230: 3d20 4e6f 6e65 0a0a 574d 5f4f 545f 636f  = None..WM_OT_co
-00355240: 6e74 6578 745f 6379 636c 655f 6172 7261  ntext_cycle_arra
-00355250: 793a 2027 626c 5f6f 7065 7261 746f 7273  y: 'bl_operators
+00354d20: 545f 6c61 7965 7227 203d 204e 6f6e 650a  T_layer' = None.
+00354d30: 0a56 4945 574c 4159 4552 5f50 545f 6c61  .VIEWLAYER_PT_la
+00354d40: 7965 725f 6375 7374 6f6d 5f70 726f 7073  yer_custom_props
+00354d50: 3a20 2762 6c5f 7569 2e70 726f 7065 7274  : 'bl_ui.propert
+00354d60: 6965 735f 7669 6577 5f6c 6179 6572 2e56  ies_view_layer.V
+00354d70: 4945 574c 4159 4552 5f50 545f 6c61 7965  IEWLAYER_PT_laye
+00354d80: 725f 6375 7374 6f6d 5f70 726f 7073 2720  r_custom_props' 
+00354d90: 3d20 4e6f 6e65 0a0a 5649 4557 4c41 5945  = None..VIEWLAYE
+00354da0: 525f 5054 5f6c 6179 6572 5f70 6173 7365  R_PT_layer_passe
+00354db0: 733a 2027 626c 5f75 692e 7072 6f70 6572  s: 'bl_ui.proper
+00354dc0: 7469 6573 5f76 6965 775f 6c61 7965 722e  ties_view_layer.
+00354dd0: 5649 4557 4c41 5945 525f 5054 5f6c 6179  VIEWLAYER_PT_lay
+00354de0: 6572 5f70 6173 7365 7327 203d 204e 6f6e  er_passes' = Non
+00354df0: 650a 0a56 4945 574c 4159 4552 5f50 545f  e..VIEWLAYER_PT_
+00354e00: 6c61 7965 725f 7061 7373 6573 5f61 6f76  layer_passes_aov
+00354e10: 3a20 2762 6c5f 7569 2e70 726f 7065 7274  : 'bl_ui.propert
+00354e20: 6965 735f 7669 6577 5f6c 6179 6572 2e56  ies_view_layer.V
+00354e30: 4945 574c 4159 4552 5f50 545f 6c61 7965  IEWLAYER_PT_laye
+00354e40: 725f 7061 7373 6573 5f61 6f76 2720 3d20  r_passes_aov' = 
+00354e50: 4e6f 6e65 0a0a 5649 4557 4c41 5945 525f  None..VIEWLAYER_
+00354e60: 5054 5f6c 6179 6572 5f70 6173 7365 735f  PT_layer_passes_
+00354e70: 6372 7970 746f 6d61 7474 653a 2027 626c  cryptomatte: 'bl
+00354e80: 5f75 692e 7072 6f70 6572 7469 6573 5f76  _ui.properties_v
+00354e90: 6965 775f 6c61 7965 722e 5649 4557 4c41  iew_layer.VIEWLA
+00354ea0: 5945 525f 5054 5f6c 6179 6572 5f70 6173  YER_PT_layer_pas
+00354eb0: 7365 735f 6372 7970 746f 6d61 7474 6527  ses_cryptomatte'
+00354ec0: 203d 204e 6f6e 650a 0a56 4945 574c 4159   = None..VIEWLAY
+00354ed0: 4552 5f50 545f 6c61 7965 725f 7061 7373  ER_PT_layer_pass
+00354ee0: 6573 5f6c 6967 6874 6772 6f75 7073 3a20  es_lightgroups: 
+00354ef0: 2762 6c5f 7569 2e70 726f 7065 7274 6965  'bl_ui.propertie
+00354f00: 735f 7669 6577 5f6c 6179 6572 2e56 4945  s_view_layer.VIE
+00354f10: 574c 4159 4552 5f50 545f 6c61 7965 725f  WLAYER_PT_layer_
+00354f20: 7061 7373 6573 5f6c 6967 6874 6772 6f75  passes_lightgrou
+00354f30: 7073 2720 3d20 4e6f 6e65 0a0a 5649 4557  ps' = None..VIEW
+00354f40: 4c41 5945 525f 554c 5f61 6f76 3a20 2762  LAYER_UL_aov: 'b
+00354f50: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
+00354f60: 7669 6577 5f6c 6179 6572 2e56 4945 574c  view_layer.VIEWL
+00354f70: 4159 4552 5f55 4c5f 616f 7627 203d 204e  AYER_UL_aov' = N
+00354f80: 6f6e 650a 0a56 4945 574c 4159 4552 5f55  one..VIEWLAYER_U
+00354f90: 4c5f 6c69 6e65 7365 7473 3a20 2762 6c5f  L_linesets: 'bl_
+00354fa0: 7569 2e70 726f 7065 7274 6965 735f 6672  ui.properties_fr
+00354fb0: 6565 7374 796c 652e 5649 4557 4c41 5945  eestyle.VIEWLAYE
+00354fc0: 525f 554c 5f6c 696e 6573 6574 7327 203d  R_UL_linesets' =
+00354fd0: 204e 6f6e 650a 0a56 4f4c 554d 455f 554c   None..VOLUME_UL
+00354fe0: 5f67 7269 6473 3a20 2762 6c5f 7569 2e70  _grids: 'bl_ui.p
+00354ff0: 726f 7065 7274 6965 735f 6461 7461 5f76  roperties_data_v
+00355000: 6f6c 756d 652e 564f 4c55 4d45 5f55 4c5f  olume.VOLUME_UL_
+00355010: 6772 6964 7327 203d 204e 6f6e 650a 0a57  grids' = None..W
+00355020: 4d5f 4d54 5f6f 7065 7261 746f 725f 7072  M_MT_operator_pr
+00355030: 6573 6574 733a 2027 626c 5f6f 7065 7261  esets: 'bl_opera
+00355040: 746f 7273 2e70 7265 7365 7473 2e57 4d5f  tors.presets.WM_
+00355050: 4d54 5f6f 7065 7261 746f 725f 7072 6573  MT_operator_pres
+00355060: 6574 7327 203d 204e 6f6e 650a 0a57 4d5f  ets' = None..WM_
+00355070: 4d54 5f73 706c 6173 683a 2027 626c 5f6f  MT_splash: 'bl_o
+00355080: 7065 7261 746f 7273 2e77 6d2e 574d 5f4d  perators.wm.WM_M
+00355090: 545f 7370 6c61 7368 2720 3d20 4e6f 6e65  T_splash' = None
+003550a0: 0a0a 574d 5f4d 545f 7370 6c61 7368 5f61  ..WM_MT_splash_a
+003550b0: 626f 7574 3a20 2762 6c5f 6f70 6572 6174  bout: 'bl_operat
+003550c0: 6f72 732e 776d 2e57 4d5f 4d54 5f73 706c  ors.wm.WM_MT_spl
+003550d0: 6173 685f 6162 6f75 7427 203d 204e 6f6e  ash_about' = Non
+003550e0: 650a 0a57 4d5f 4d54 5f73 706c 6173 685f  e..WM_MT_splash_
+003550f0: 7175 6963 6b5f 7365 7475 703a 2027 626c  quick_setup: 'bl
+00355100: 5f6f 7065 7261 746f 7273 2e77 6d2e 574d  _operators.wm.WM
+00355110: 5f4d 545f 7370 6c61 7368 5f71 7569 636b  _MT_splash_quick
+00355120: 5f73 6574 7570 2720 3d20 4e6f 6e65 0a0a  _setup' = None..
+00355130: 574d 5f4d 545f 746f 6f6c 7379 7374 656d  WM_MT_toolsystem
+00355140: 5f73 7562 6d65 6e75 3a20 2762 6c5f 7569  _submenu: 'bl_ui
+00355150: 2e73 7061 6365 5f74 6f6f 6c73 7973 7465  .space_toolsyste
+00355160: 6d5f 636f 6d6d 6f6e 2e57 4d5f 4d54 5f74  m_common.WM_MT_t
+00355170: 6f6f 6c73 7973 7465 6d5f 7375 626d 656e  oolsystem_submen
+00355180: 7527 203d 204e 6f6e 650a 0a57 4d5f 4f54  u' = None..WM_OT
+00355190: 5f62 6174 6368 5f72 656e 616d 653a 2027  _batch_rename: '
+003551a0: 626c 5f6f 7065 7261 746f 7273 2e77 6d2e  bl_operators.wm.
+003551b0: 574d 5f4f 545f 6261 7463 685f 7265 6e61  WM_OT_batch_rena
+003551c0: 6d65 2720 3d20 4e6f 6e65 0a0a 574d 5f4f  me' = None..WM_O
+003551d0: 545f 626c 656e 645f 7374 7269 6e67 735f  T_blend_strings_
+003551e0: 7574 6638 5f76 616c 6964 6174 653a 2027  utf8_validate: '
+003551f0: 626c 5f6f 7065 7261 746f 7273 2e66 696c  bl_operators.fil
+00355200: 652e 574d 5f4f 545f 626c 656e 645f 7374  e.WM_OT_blend_st
+00355210: 7269 6e67 735f 7574 6638 5f76 616c 6964  rings_utf8_valid
+00355220: 6174 6527 203d 204e 6f6e 650a 0a57 4d5f  ate' = None..WM_
+00355230: 4f54 5f63 6f6e 7465 7874 5f63 6f6c 6c65  OT_context_colle
+00355240: 6374 696f 6e5f 626f 6f6c 6561 6e5f 7365  ction_boolean_se
+00355250: 743a 2027 626c 5f6f 7065 7261 746f 7273  t: 'bl_operators
 00355260: 2e77 6d2e 574d 5f4f 545f 636f 6e74 6578  .wm.WM_OT_contex
-00355270: 745f 6379 636c 655f 6172 7261 7927 203d  t_cycle_array' =
-00355280: 204e 6f6e 650a 0a57 4d5f 4f54 5f63 6f6e   None..WM_OT_con
-00355290: 7465 7874 5f63 7963 6c65 5f65 6e75 6d3a  text_cycle_enum:
-003552a0: 2027 626c 5f6f 7065 7261 746f 7273 2e77   'bl_operators.w
-003552b0: 6d2e 574d 5f4f 545f 636f 6e74 6578 745f  m.WM_OT_context_
-003552c0: 6379 636c 655f 656e 756d 2720 3d20 4e6f  cycle_enum' = No
-003552d0: 6e65 0a0a 574d 5f4f 545f 636f 6e74 6578  ne..WM_OT_contex
-003552e0: 745f 6379 636c 655f 696e 743a 2027 626c  t_cycle_int: 'bl
-003552f0: 5f6f 7065 7261 746f 7273 2e77 6d2e 574d  _operators.wm.WM
-00355300: 5f4f 545f 636f 6e74 6578 745f 6379 636c  _OT_context_cycl
-00355310: 655f 696e 7427 203d 204e 6f6e 650a 0a57  e_int' = None..W
-00355320: 4d5f 4f54 5f63 6f6e 7465 7874 5f6d 656e  M_OT_context_men
-00355330: 755f 656e 756d 3a20 2762 6c5f 6f70 6572  u_enum: 'bl_oper
-00355340: 6174 6f72 732e 776d 2e57 4d5f 4f54 5f63  ators.wm.WM_OT_c
-00355350: 6f6e 7465 7874 5f6d 656e 755f 656e 756d  ontext_menu_enum
-00355360: 2720 3d20 4e6f 6e65 0a0a 574d 5f4f 545f  ' = None..WM_OT_
-00355370: 636f 6e74 6578 745f 6d6f 6461 6c5f 6d6f  context_modal_mo
-00355380: 7573 653a 2027 626c 5f6f 7065 7261 746f  use: 'bl_operato
-00355390: 7273 2e77 6d2e 574d 5f4f 545f 636f 6e74  rs.wm.WM_OT_cont
-003553a0: 6578 745f 6d6f 6461 6c5f 6d6f 7573 6527  ext_modal_mouse'
-003553b0: 203d 204e 6f6e 650a 0a57 4d5f 4f54 5f63   = None..WM_OT_c
-003553c0: 6f6e 7465 7874 5f70 6965 5f65 6e75 6d3a  ontext_pie_enum:
-003553d0: 2027 626c 5f6f 7065 7261 746f 7273 2e77   'bl_operators.w
-003553e0: 6d2e 574d 5f4f 545f 636f 6e74 6578 745f  m.WM_OT_context_
-003553f0: 7069 655f 656e 756d 2720 3d20 4e6f 6e65  pie_enum' = None
-00355400: 0a0a 574d 5f4f 545f 636f 6e74 6578 745f  ..WM_OT_context_
-00355410: 7363 616c 655f 666c 6f61 743a 2027 626c  scale_float: 'bl
-00355420: 5f6f 7065 7261 746f 7273 2e77 6d2e 574d  _operators.wm.WM
-00355430: 5f4f 545f 636f 6e74 6578 745f 7363 616c  _OT_context_scal
-00355440: 655f 666c 6f61 7427 203d 204e 6f6e 650a  e_float' = None.
-00355450: 0a57 4d5f 4f54 5f63 6f6e 7465 7874 5f73  .WM_OT_context_s
-00355460: 6361 6c65 5f69 6e74 3a20 2762 6c5f 6f70  cale_int: 'bl_op
-00355470: 6572 6174 6f72 732e 776d 2e57 4d5f 4f54  erators.wm.WM_OT
-00355480: 5f63 6f6e 7465 7874 5f73 6361 6c65 5f69  _context_scale_i
-00355490: 6e74 2720 3d20 4e6f 6e65 0a0a 574d 5f4f  nt' = None..WM_O
-003554a0: 545f 636f 6e74 6578 745f 7365 745f 626f  T_context_set_bo
-003554b0: 6f6c 6561 6e3a 2027 626c 5f6f 7065 7261  olean: 'bl_opera
-003554c0: 746f 7273 2e77 6d2e 574d 5f4f 545f 636f  tors.wm.WM_OT_co
-003554d0: 6e74 6578 745f 7365 745f 626f 6f6c 6561  ntext_set_boolea
-003554e0: 6e27 203d 204e 6f6e 650a 0a57 4d5f 4f54  n' = None..WM_OT
-003554f0: 5f63 6f6e 7465 7874 5f73 6574 5f65 6e75  _context_set_enu
-00355500: 6d3a 2027 626c 5f6f 7065 7261 746f 7273  m: 'bl_operators
-00355510: 2e77 6d2e 574d 5f4f 545f 636f 6e74 6578  .wm.WM_OT_contex
-00355520: 745f 7365 745f 656e 756d 2720 3d20 4e6f  t_set_enum' = No
-00355530: 6e65 0a0a 574d 5f4f 545f 636f 6e74 6578  ne..WM_OT_contex
-00355540: 745f 7365 745f 666c 6f61 743a 2027 626c  t_set_float: 'bl
-00355550: 5f6f 7065 7261 746f 7273 2e77 6d2e 574d  _operators.wm.WM
-00355560: 5f4f 545f 636f 6e74 6578 745f 7365 745f  _OT_context_set_
-00355570: 666c 6f61 7427 203d 204e 6f6e 650a 0a57  float' = None..W
-00355580: 4d5f 4f54 5f63 6f6e 7465 7874 5f73 6574  M_OT_context_set
-00355590: 5f69 643a 2027 626c 5f6f 7065 7261 746f  _id: 'bl_operato
-003555a0: 7273 2e77 6d2e 574d 5f4f 545f 636f 6e74  rs.wm.WM_OT_cont
-003555b0: 6578 745f 7365 745f 6964 2720 3d20 4e6f  ext_set_id' = No
-003555c0: 6e65 0a0a 574d 5f4f 545f 636f 6e74 6578  ne..WM_OT_contex
-003555d0: 745f 7365 745f 696e 743a 2027 626c 5f6f  t_set_int: 'bl_o
-003555e0: 7065 7261 746f 7273 2e77 6d2e 574d 5f4f  perators.wm.WM_O
-003555f0: 545f 636f 6e74 6578 745f 7365 745f 696e  T_context_set_in
-00355600: 7427 203d 204e 6f6e 650a 0a57 4d5f 4f54  t' = None..WM_OT
-00355610: 5f63 6f6e 7465 7874 5f73 6574 5f73 7472  _context_set_str
-00355620: 696e 673a 2027 626c 5f6f 7065 7261 746f  ing: 'bl_operato
-00355630: 7273 2e77 6d2e 574d 5f4f 545f 636f 6e74  rs.wm.WM_OT_cont
-00355640: 6578 745f 7365 745f 7374 7269 6e67 2720  ext_set_string' 
-00355650: 3d20 4e6f 6e65 0a0a 574d 5f4f 545f 636f  = None..WM_OT_co
-00355660: 6e74 6578 745f 7365 745f 7661 6c75 653a  ntext_set_value:
-00355670: 2027 626c 5f6f 7065 7261 746f 7273 2e77   'bl_operators.w
-00355680: 6d2e 574d 5f4f 545f 636f 6e74 6578 745f  m.WM_OT_context_
-00355690: 7365 745f 7661 6c75 6527 203d 204e 6f6e  set_value' = Non
-003556a0: 650a 0a57 4d5f 4f54 5f63 6f6e 7465 7874  e..WM_OT_context
-003556b0: 5f74 6f67 676c 653a 2027 626c 5f6f 7065  _toggle: 'bl_ope
-003556c0: 7261 746f 7273 2e77 6d2e 574d 5f4f 545f  rators.wm.WM_OT_
-003556d0: 636f 6e74 6578 745f 746f 6767 6c65 2720  context_toggle' 
-003556e0: 3d20 4e6f 6e65 0a0a 574d 5f4f 545f 636f  = None..WM_OT_co
-003556f0: 6e74 6578 745f 746f 6767 6c65 5f65 6e75  ntext_toggle_enu
-00355700: 6d3a 2027 626c 5f6f 7065 7261 746f 7273  m: 'bl_operators
-00355710: 2e77 6d2e 574d 5f4f 545f 636f 6e74 6578  .wm.WM_OT_contex
-00355720: 745f 746f 6767 6c65 5f65 6e75 6d27 203d  t_toggle_enum' =
-00355730: 204e 6f6e 650a 0a57 4d5f 4f54 5f64 6f63   None..WM_OT_doc
-00355740: 5f76 6965 773a 2027 626c 5f6f 7065 7261  _view: 'bl_opera
-00355750: 746f 7273 2e77 6d2e 574d 5f4f 545f 646f  tors.wm.WM_OT_do
-00355760: 635f 7669 6577 2720 3d20 4e6f 6e65 0a0a  c_view' = None..
-00355770: 574d 5f4f 545f 646f 635f 7669 6577 5f6d  WM_OT_doc_view_m
-00355780: 616e 7561 6c3a 2027 626c 5f6f 7065 7261  anual: 'bl_opera
-00355790: 746f 7273 2e77 6d2e 574d 5f4f 545f 646f  tors.wm.WM_OT_do
-003557a0: 635f 7669 6577 5f6d 616e 7561 6c27 203d  c_view_manual' =
-003557b0: 204e 6f6e 650a 0a57 4d5f 4f54 5f64 726f   None..WM_OT_dro
-003557c0: 705f 626c 656e 645f 6669 6c65 3a20 2762  p_blend_file: 'b
-003557d0: 6c5f 6f70 6572 6174 6f72 732e 776d 2e57  l_operators.wm.W
-003557e0: 4d5f 4f54 5f64 726f 705f 626c 656e 645f  M_OT_drop_blend_
-003557f0: 6669 6c65 2720 3d20 4e6f 6e65 0a0a 574d  file' = None..WM
-00355800: 5f4f 545f 6f70 6572 6174 6f72 5f63 6865  _OT_operator_che
-00355810: 6174 5f73 6865 6574 3a20 2762 6c5f 6f70  at_sheet: 'bl_op
-00355820: 6572 6174 6f72 732e 776d 2e57 4d5f 4f54  erators.wm.WM_OT
-00355830: 5f6f 7065 7261 746f 725f 6368 6561 745f  _operator_cheat_
-00355840: 7368 6565 7427 203d 204e 6f6e 650a 0a57  sheet' = None..W
-00355850: 4d5f 4f54 5f6f 7065 7261 746f 725f 7069  M_OT_operator_pi
-00355860: 655f 656e 756d 3a20 2762 6c5f 6f70 6572  e_enum: 'bl_oper
-00355870: 6174 6f72 732e 776d 2e57 4d5f 4f54 5f6f  ators.wm.WM_OT_o
-00355880: 7065 7261 746f 725f 7069 655f 656e 756d  perator_pie_enum
-00355890: 2720 3d20 4e6f 6e65 0a0a 574d 5f4f 545f  ' = None..WM_OT_
-003558a0: 6f77 6e65 725f 6469 7361 626c 653a 2027  owner_disable: '
-003558b0: 626c 5f6f 7065 7261 746f 7273 2e77 6d2e  bl_operators.wm.
-003558c0: 574d 5f4f 545f 6f77 6e65 725f 6469 7361  WM_OT_owner_disa
-003558d0: 626c 6527 203d 204e 6f6e 650a 0a57 4d5f  ble' = None..WM_
-003558e0: 4f54 5f6f 776e 6572 5f65 6e61 626c 653a  OT_owner_enable:
-003558f0: 2027 626c 5f6f 7065 7261 746f 7273 2e77   'bl_operators.w
-00355900: 6d2e 574d 5f4f 545f 6f77 6e65 725f 656e  m.WM_OT_owner_en
-00355910: 6162 6c65 2720 3d20 4e6f 6e65 0a0a 574d  able' = None..WM
-00355920: 5f4f 545f 7061 7468 5f6f 7065 6e3a 2027  _OT_path_open: '
-00355930: 626c 5f6f 7065 7261 746f 7273 2e77 6d2e  bl_operators.wm.
-00355940: 574d 5f4f 545f 7061 7468 5f6f 7065 6e27  WM_OT_path_open'
-00355950: 203d 204e 6f6e 650a 0a57 4d5f 4f54 5f70   = None..WM_OT_p
-00355960: 7265 7669 6577 735f 6261 7463 685f 636c  reviews_batch_cl
-00355970: 6561 723a 2027 626c 5f6f 7065 7261 746f  ear: 'bl_operato
-00355980: 7273 2e66 696c 652e 574d 5f4f 545f 7072  rs.file.WM_OT_pr
-00355990: 6576 6965 7773 5f62 6174 6368 5f63 6c65  eviews_batch_cle
-003559a0: 6172 2720 3d20 4e6f 6e65 0a0a 574d 5f4f  ar' = None..WM_O
-003559b0: 545f 7072 6576 6965 7773 5f62 6174 6368  T_previews_batch
-003559c0: 5f67 656e 6572 6174 653a 2027 626c 5f6f  _generate: 'bl_o
-003559d0: 7065 7261 746f 7273 2e66 696c 652e 574d  perators.file.WM
-003559e0: 5f4f 545f 7072 6576 6965 7773 5f62 6174  _OT_previews_bat
-003559f0: 6368 5f67 656e 6572 6174 6527 203d 204e  ch_generate' = N
-00355a00: 6f6e 650a 0a57 4d5f 4f54 5f70 726f 7065  one..WM_OT_prope
-00355a10: 7274 6965 735f 6164 643a 2027 626c 5f6f  rties_add: 'bl_o
-00355a20: 7065 7261 746f 7273 2e77 6d2e 574d 5f4f  perators.wm.WM_O
-00355a30: 545f 7072 6f70 6572 7469 6573 5f61 6464  T_properties_add
-00355a40: 2720 3d20 4e6f 6e65 0a0a 574d 5f4f 545f  ' = None..WM_OT_
-00355a50: 7072 6f70 6572 7469 6573 5f63 6f6e 7465  properties_conte
-00355a60: 7874 5f63 6861 6e67 653a 2027 626c 5f6f  xt_change: 'bl_o
-00355a70: 7065 7261 746f 7273 2e77 6d2e 574d 5f4f  perators.wm.WM_O
-00355a80: 545f 7072 6f70 6572 7469 6573 5f63 6f6e  T_properties_con
-00355a90: 7465 7874 5f63 6861 6e67 6527 203d 204e  text_change' = N
-00355aa0: 6f6e 650a 0a57 4d5f 4f54 5f70 726f 7065  one..WM_OT_prope
-00355ab0: 7274 6965 735f 6564 6974 3a20 2762 6c5f  rties_edit: 'bl_
-00355ac0: 6f70 6572 6174 6f72 732e 776d 2e57 4d5f  operators.wm.WM_
-00355ad0: 4f54 5f70 726f 7065 7274 6965 735f 6564  OT_properties_ed
-00355ae0: 6974 2720 3d20 4e6f 6e65 0a0a 574d 5f4f  it' = None..WM_O
-00355af0: 545f 7072 6f70 6572 7469 6573 5f65 6469  T_properties_edi
-00355b00: 745f 7661 6c75 653a 2027 626c 5f6f 7065  t_value: 'bl_ope
-00355b10: 7261 746f 7273 2e77 6d2e 574d 5f4f 545f  rators.wm.WM_OT_
-00355b20: 7072 6f70 6572 7469 6573 5f65 6469 745f  properties_edit_
-00355b30: 7661 6c75 6527 203d 204e 6f6e 650a 0a57  value' = None..W
-00355b40: 4d5f 4f54 5f70 726f 7065 7274 6965 735f  M_OT_properties_
-00355b50: 7265 6d6f 7665 3a20 2762 6c5f 6f70 6572  remove: 'bl_oper
-00355b60: 6174 6f72 732e 776d 2e57 4d5f 4f54 5f70  ators.wm.WM_OT_p
-00355b70: 726f 7065 7274 6965 735f 7265 6d6f 7665  roperties_remove
-00355b80: 2720 3d20 4e6f 6e65 0a0a 574d 5f4f 545f  ' = None..WM_OT_
-00355b90: 7379 7369 6e66 6f3a 2027 626c 5f6f 7065  sysinfo: 'bl_ope
-00355ba0: 7261 746f 7273 2e77 6d2e 574d 5f4f 545f  rators.wm.WM_OT_
-00355bb0: 7379 7369 6e66 6f27 203d 204e 6f6e 650a  sysinfo' = None.
-00355bc0: 0a57 4d5f 4f54 5f74 6f6f 6c5f 7365 745f  .WM_OT_tool_set_
-00355bd0: 6279 5f69 643a 2027 626c 5f6f 7065 7261  by_id: 'bl_opera
-00355be0: 746f 7273 2e77 6d2e 574d 5f4f 545f 746f  tors.wm.WM_OT_to
-00355bf0: 6f6c 5f73 6574 5f62 795f 6964 2720 3d20  ol_set_by_id' = 
-00355c00: 4e6f 6e65 0a0a 574d 5f4f 545f 746f 6f6c  None..WM_OT_tool
-00355c10: 5f73 6574 5f62 795f 696e 6465 783a 2027  _set_by_index: '
-00355c20: 626c 5f6f 7065 7261 746f 7273 2e77 6d2e  bl_operators.wm.
-00355c30: 574d 5f4f 545f 746f 6f6c 5f73 6574 5f62  WM_OT_tool_set_b
-00355c40: 795f 696e 6465 7827 203d 204e 6f6e 650a  y_index' = None.
-00355c50: 0a57 4d5f 4f54 5f74 6f6f 6c62 6172 3a20  .WM_OT_toolbar: 
-00355c60: 2762 6c5f 6f70 6572 6174 6f72 732e 776d  'bl_operators.wm
-00355c70: 2e57 4d5f 4f54 5f74 6f6f 6c62 6172 2720  .WM_OT_toolbar' 
-00355c80: 3d20 4e6f 6e65 0a0a 574d 5f4f 545f 746f  = None..WM_OT_to
-00355c90: 6f6c 6261 725f 6661 6c6c 6261 636b 5f70  olbar_fallback_p
-00355ca0: 6965 3a20 2762 6c5f 6f70 6572 6174 6f72  ie: 'bl_operator
-00355cb0: 732e 776d 2e57 4d5f 4f54 5f74 6f6f 6c62  s.wm.WM_OT_toolb
-00355cc0: 6172 5f66 616c 6c62 6163 6b5f 7069 6527  ar_fallback_pie'
-00355cd0: 203d 204e 6f6e 650a 0a57 4d5f 4f54 5f74   = None..WM_OT_t
-00355ce0: 6f6f 6c62 6172 5f70 726f 6d70 743a 2027  oolbar_prompt: '
-00355cf0: 626c 5f6f 7065 7261 746f 7273 2e77 6d2e  bl_operators.wm.
-00355d00: 574d 5f4f 545f 746f 6f6c 6261 725f 7072  WM_OT_toolbar_pr
-00355d10: 6f6d 7074 2720 3d20 4e6f 6e65 0a0a 574d  ompt' = None..WM
-00355d20: 5f4f 545f 7572 6c5f 6f70 656e 3a20 2762  _OT_url_open: 'b
-00355d30: 6c5f 6f70 6572 6174 6f72 732e 776d 2e57  l_operators.wm.W
-00355d40: 4d5f 4f54 5f75 726c 5f6f 7065 6e27 203d  M_OT_url_open' =
-00355d50: 204e 6f6e 650a 0a57 4d5f 4f54 5f75 726c   None..WM_OT_url
-00355d60: 5f6f 7065 6e5f 7072 6573 6574 3a20 2762  _open_preset: 'b
-00355d70: 6c5f 6f70 6572 6174 6f72 732e 776d 2e57  l_operators.wm.W
-00355d80: 4d5f 4f54 5f75 726c 5f6f 7065 6e5f 7072  M_OT_url_open_pr
-00355d90: 6573 6574 2720 3d20 4e6f 6e65 0a0a 574f  eset' = None..WO
-00355da0: 524b 5350 4143 455f 5054 5f61 6464 6f6e  RKSPACE_PT_addon
-00355db0: 733a 2027 626c 5f75 692e 7072 6f70 6572  s: 'bl_ui.proper
-00355dc0: 7469 6573 5f77 6f72 6b73 7061 6365 2e57  ties_workspace.W
-00355dd0: 4f52 4b53 5041 4345 5f50 545f 6164 646f  ORKSPACE_PT_addo
-00355de0: 6e73 2720 3d20 4e6f 6e65 0a0a 574f 524b  ns' = None..WORK
-00355df0: 5350 4143 455f 5054 5f63 7573 746f 6d5f  SPACE_PT_custom_
-00355e00: 7072 6f70 733a 2027 626c 5f75 692e 7072  props: 'bl_ui.pr
-00355e10: 6f70 6572 7469 6573 5f77 6f72 6b73 7061  operties_workspa
-00355e20: 6365 2e57 4f52 4b53 5041 4345 5f50 545f  ce.WORKSPACE_PT_
-00355e30: 6375 7374 6f6d 5f70 726f 7073 2720 3d20  custom_props' = 
+00355270: 745f 636f 6c6c 6563 7469 6f6e 5f62 6f6f  t_collection_boo
+00355280: 6c65 616e 5f73 6574 2720 3d20 4e6f 6e65  lean_set' = None
+00355290: 0a0a 574d 5f4f 545f 636f 6e74 6578 745f  ..WM_OT_context_
+003552a0: 6379 636c 655f 6172 7261 793a 2027 626c  cycle_array: 'bl
+003552b0: 5f6f 7065 7261 746f 7273 2e77 6d2e 574d  _operators.wm.WM
+003552c0: 5f4f 545f 636f 6e74 6578 745f 6379 636c  _OT_context_cycl
+003552d0: 655f 6172 7261 7927 203d 204e 6f6e 650a  e_array' = None.
+003552e0: 0a57 4d5f 4f54 5f63 6f6e 7465 7874 5f63  .WM_OT_context_c
+003552f0: 7963 6c65 5f65 6e75 6d3a 2027 626c 5f6f  ycle_enum: 'bl_o
+00355300: 7065 7261 746f 7273 2e77 6d2e 574d 5f4f  perators.wm.WM_O
+00355310: 545f 636f 6e74 6578 745f 6379 636c 655f  T_context_cycle_
+00355320: 656e 756d 2720 3d20 4e6f 6e65 0a0a 574d  enum' = None..WM
+00355330: 5f4f 545f 636f 6e74 6578 745f 6379 636c  _OT_context_cycl
+00355340: 655f 696e 743a 2027 626c 5f6f 7065 7261  e_int: 'bl_opera
+00355350: 746f 7273 2e77 6d2e 574d 5f4f 545f 636f  tors.wm.WM_OT_co
+00355360: 6e74 6578 745f 6379 636c 655f 696e 7427  ntext_cycle_int'
+00355370: 203d 204e 6f6e 650a 0a57 4d5f 4f54 5f63   = None..WM_OT_c
+00355380: 6f6e 7465 7874 5f6d 656e 755f 656e 756d  ontext_menu_enum
+00355390: 3a20 2762 6c5f 6f70 6572 6174 6f72 732e  : 'bl_operators.
+003553a0: 776d 2e57 4d5f 4f54 5f63 6f6e 7465 7874  wm.WM_OT_context
+003553b0: 5f6d 656e 755f 656e 756d 2720 3d20 4e6f  _menu_enum' = No
+003553c0: 6e65 0a0a 574d 5f4f 545f 636f 6e74 6578  ne..WM_OT_contex
+003553d0: 745f 6d6f 6461 6c5f 6d6f 7573 653a 2027  t_modal_mouse: '
+003553e0: 626c 5f6f 7065 7261 746f 7273 2e77 6d2e  bl_operators.wm.
+003553f0: 574d 5f4f 545f 636f 6e74 6578 745f 6d6f  WM_OT_context_mo
+00355400: 6461 6c5f 6d6f 7573 6527 203d 204e 6f6e  dal_mouse' = Non
+00355410: 650a 0a57 4d5f 4f54 5f63 6f6e 7465 7874  e..WM_OT_context
+00355420: 5f70 6965 5f65 6e75 6d3a 2027 626c 5f6f  _pie_enum: 'bl_o
+00355430: 7065 7261 746f 7273 2e77 6d2e 574d 5f4f  perators.wm.WM_O
+00355440: 545f 636f 6e74 6578 745f 7069 655f 656e  T_context_pie_en
+00355450: 756d 2720 3d20 4e6f 6e65 0a0a 574d 5f4f  um' = None..WM_O
+00355460: 545f 636f 6e74 6578 745f 7363 616c 655f  T_context_scale_
+00355470: 666c 6f61 743a 2027 626c 5f6f 7065 7261  float: 'bl_opera
+00355480: 746f 7273 2e77 6d2e 574d 5f4f 545f 636f  tors.wm.WM_OT_co
+00355490: 6e74 6578 745f 7363 616c 655f 666c 6f61  ntext_scale_floa
+003554a0: 7427 203d 204e 6f6e 650a 0a57 4d5f 4f54  t' = None..WM_OT
+003554b0: 5f63 6f6e 7465 7874 5f73 6361 6c65 5f69  _context_scale_i
+003554c0: 6e74 3a20 2762 6c5f 6f70 6572 6174 6f72  nt: 'bl_operator
+003554d0: 732e 776d 2e57 4d5f 4f54 5f63 6f6e 7465  s.wm.WM_OT_conte
+003554e0: 7874 5f73 6361 6c65 5f69 6e74 2720 3d20  xt_scale_int' = 
+003554f0: 4e6f 6e65 0a0a 574d 5f4f 545f 636f 6e74  None..WM_OT_cont
+00355500: 6578 745f 7365 745f 626f 6f6c 6561 6e3a  ext_set_boolean:
+00355510: 2027 626c 5f6f 7065 7261 746f 7273 2e77   'bl_operators.w
+00355520: 6d2e 574d 5f4f 545f 636f 6e74 6578 745f  m.WM_OT_context_
+00355530: 7365 745f 626f 6f6c 6561 6e27 203d 204e  set_boolean' = N
+00355540: 6f6e 650a 0a57 4d5f 4f54 5f63 6f6e 7465  one..WM_OT_conte
+00355550: 7874 5f73 6574 5f65 6e75 6d3a 2027 626c  xt_set_enum: 'bl
+00355560: 5f6f 7065 7261 746f 7273 2e77 6d2e 574d  _operators.wm.WM
+00355570: 5f4f 545f 636f 6e74 6578 745f 7365 745f  _OT_context_set_
+00355580: 656e 756d 2720 3d20 4e6f 6e65 0a0a 574d  enum' = None..WM
+00355590: 5f4f 545f 636f 6e74 6578 745f 7365 745f  _OT_context_set_
+003555a0: 666c 6f61 743a 2027 626c 5f6f 7065 7261  float: 'bl_opera
+003555b0: 746f 7273 2e77 6d2e 574d 5f4f 545f 636f  tors.wm.WM_OT_co
+003555c0: 6e74 6578 745f 7365 745f 666c 6f61 7427  ntext_set_float'
+003555d0: 203d 204e 6f6e 650a 0a57 4d5f 4f54 5f63   = None..WM_OT_c
+003555e0: 6f6e 7465 7874 5f73 6574 5f69 643a 2027  ontext_set_id: '
+003555f0: 626c 5f6f 7065 7261 746f 7273 2e77 6d2e  bl_operators.wm.
+00355600: 574d 5f4f 545f 636f 6e74 6578 745f 7365  WM_OT_context_se
+00355610: 745f 6964 2720 3d20 4e6f 6e65 0a0a 574d  t_id' = None..WM
+00355620: 5f4f 545f 636f 6e74 6578 745f 7365 745f  _OT_context_set_
+00355630: 696e 743a 2027 626c 5f6f 7065 7261 746f  int: 'bl_operato
+00355640: 7273 2e77 6d2e 574d 5f4f 545f 636f 6e74  rs.wm.WM_OT_cont
+00355650: 6578 745f 7365 745f 696e 7427 203d 204e  ext_set_int' = N
+00355660: 6f6e 650a 0a57 4d5f 4f54 5f63 6f6e 7465  one..WM_OT_conte
+00355670: 7874 5f73 6574 5f73 7472 696e 673a 2027  xt_set_string: '
+00355680: 626c 5f6f 7065 7261 746f 7273 2e77 6d2e  bl_operators.wm.
+00355690: 574d 5f4f 545f 636f 6e74 6578 745f 7365  WM_OT_context_se
+003556a0: 745f 7374 7269 6e67 2720 3d20 4e6f 6e65  t_string' = None
+003556b0: 0a0a 574d 5f4f 545f 636f 6e74 6578 745f  ..WM_OT_context_
+003556c0: 7365 745f 7661 6c75 653a 2027 626c 5f6f  set_value: 'bl_o
+003556d0: 7065 7261 746f 7273 2e77 6d2e 574d 5f4f  perators.wm.WM_O
+003556e0: 545f 636f 6e74 6578 745f 7365 745f 7661  T_context_set_va
+003556f0: 6c75 6527 203d 204e 6f6e 650a 0a57 4d5f  lue' = None..WM_
+00355700: 4f54 5f63 6f6e 7465 7874 5f74 6f67 676c  OT_context_toggl
+00355710: 653a 2027 626c 5f6f 7065 7261 746f 7273  e: 'bl_operators
+00355720: 2e77 6d2e 574d 5f4f 545f 636f 6e74 6578  .wm.WM_OT_contex
+00355730: 745f 746f 6767 6c65 2720 3d20 4e6f 6e65  t_toggle' = None
+00355740: 0a0a 574d 5f4f 545f 636f 6e74 6578 745f  ..WM_OT_context_
+00355750: 746f 6767 6c65 5f65 6e75 6d3a 2027 626c  toggle_enum: 'bl
+00355760: 5f6f 7065 7261 746f 7273 2e77 6d2e 574d  _operators.wm.WM
+00355770: 5f4f 545f 636f 6e74 6578 745f 746f 6767  _OT_context_togg
+00355780: 6c65 5f65 6e75 6d27 203d 204e 6f6e 650a  le_enum' = None.
+00355790: 0a57 4d5f 4f54 5f64 6f63 5f76 6965 773a  .WM_OT_doc_view:
+003557a0: 2027 626c 5f6f 7065 7261 746f 7273 2e77   'bl_operators.w
+003557b0: 6d2e 574d 5f4f 545f 646f 635f 7669 6577  m.WM_OT_doc_view
+003557c0: 2720 3d20 4e6f 6e65 0a0a 574d 5f4f 545f  ' = None..WM_OT_
+003557d0: 646f 635f 7669 6577 5f6d 616e 7561 6c3a  doc_view_manual:
+003557e0: 2027 626c 5f6f 7065 7261 746f 7273 2e77   'bl_operators.w
+003557f0: 6d2e 574d 5f4f 545f 646f 635f 7669 6577  m.WM_OT_doc_view
+00355800: 5f6d 616e 7561 6c27 203d 204e 6f6e 650a  _manual' = None.
+00355810: 0a57 4d5f 4f54 5f64 726f 705f 626c 656e  .WM_OT_drop_blen
+00355820: 645f 6669 6c65 3a20 2762 6c5f 6f70 6572  d_file: 'bl_oper
+00355830: 6174 6f72 732e 776d 2e57 4d5f 4f54 5f64  ators.wm.WM_OT_d
+00355840: 726f 705f 626c 656e 645f 6669 6c65 2720  rop_blend_file' 
+00355850: 3d20 4e6f 6e65 0a0a 574d 5f4f 545f 6f70  = None..WM_OT_op
+00355860: 6572 6174 6f72 5f63 6865 6174 5f73 6865  erator_cheat_she
+00355870: 6574 3a20 2762 6c5f 6f70 6572 6174 6f72  et: 'bl_operator
+00355880: 732e 776d 2e57 4d5f 4f54 5f6f 7065 7261  s.wm.WM_OT_opera
+00355890: 746f 725f 6368 6561 745f 7368 6565 7427  tor_cheat_sheet'
+003558a0: 203d 204e 6f6e 650a 0a57 4d5f 4f54 5f6f   = None..WM_OT_o
+003558b0: 7065 7261 746f 725f 7069 655f 656e 756d  perator_pie_enum
+003558c0: 3a20 2762 6c5f 6f70 6572 6174 6f72 732e  : 'bl_operators.
+003558d0: 776d 2e57 4d5f 4f54 5f6f 7065 7261 746f  wm.WM_OT_operato
+003558e0: 725f 7069 655f 656e 756d 2720 3d20 4e6f  r_pie_enum' = No
+003558f0: 6e65 0a0a 574d 5f4f 545f 6f77 6e65 725f  ne..WM_OT_owner_
+00355900: 6469 7361 626c 653a 2027 626c 5f6f 7065  disable: 'bl_ope
+00355910: 7261 746f 7273 2e77 6d2e 574d 5f4f 545f  rators.wm.WM_OT_
+00355920: 6f77 6e65 725f 6469 7361 626c 6527 203d  owner_disable' =
+00355930: 204e 6f6e 650a 0a57 4d5f 4f54 5f6f 776e   None..WM_OT_own
+00355940: 6572 5f65 6e61 626c 653a 2027 626c 5f6f  er_enable: 'bl_o
+00355950: 7065 7261 746f 7273 2e77 6d2e 574d 5f4f  perators.wm.WM_O
+00355960: 545f 6f77 6e65 725f 656e 6162 6c65 2720  T_owner_enable' 
+00355970: 3d20 4e6f 6e65 0a0a 574d 5f4f 545f 7061  = None..WM_OT_pa
+00355980: 7468 5f6f 7065 6e3a 2027 626c 5f6f 7065  th_open: 'bl_ope
+00355990: 7261 746f 7273 2e77 6d2e 574d 5f4f 545f  rators.wm.WM_OT_
+003559a0: 7061 7468 5f6f 7065 6e27 203d 204e 6f6e  path_open' = Non
+003559b0: 650a 0a57 4d5f 4f54 5f70 7265 7669 6577  e..WM_OT_preview
+003559c0: 735f 6261 7463 685f 636c 6561 723a 2027  s_batch_clear: '
+003559d0: 626c 5f6f 7065 7261 746f 7273 2e66 696c  bl_operators.fil
+003559e0: 652e 574d 5f4f 545f 7072 6576 6965 7773  e.WM_OT_previews
+003559f0: 5f62 6174 6368 5f63 6c65 6172 2720 3d20  _batch_clear' = 
+00355a00: 4e6f 6e65 0a0a 574d 5f4f 545f 7072 6576  None..WM_OT_prev
+00355a10: 6965 7773 5f62 6174 6368 5f67 656e 6572  iews_batch_gener
+00355a20: 6174 653a 2027 626c 5f6f 7065 7261 746f  ate: 'bl_operato
+00355a30: 7273 2e66 696c 652e 574d 5f4f 545f 7072  rs.file.WM_OT_pr
+00355a40: 6576 6965 7773 5f62 6174 6368 5f67 656e  eviews_batch_gen
+00355a50: 6572 6174 6527 203d 204e 6f6e 650a 0a57  erate' = None..W
+00355a60: 4d5f 4f54 5f70 726f 7065 7274 6965 735f  M_OT_properties_
+00355a70: 6164 643a 2027 626c 5f6f 7065 7261 746f  add: 'bl_operato
+00355a80: 7273 2e77 6d2e 574d 5f4f 545f 7072 6f70  rs.wm.WM_OT_prop
+00355a90: 6572 7469 6573 5f61 6464 2720 3d20 4e6f  erties_add' = No
+00355aa0: 6e65 0a0a 574d 5f4f 545f 7072 6f70 6572  ne..WM_OT_proper
+00355ab0: 7469 6573 5f63 6f6e 7465 7874 5f63 6861  ties_context_cha
+00355ac0: 6e67 653a 2027 626c 5f6f 7065 7261 746f  nge: 'bl_operato
+00355ad0: 7273 2e77 6d2e 574d 5f4f 545f 7072 6f70  rs.wm.WM_OT_prop
+00355ae0: 6572 7469 6573 5f63 6f6e 7465 7874 5f63  erties_context_c
+00355af0: 6861 6e67 6527 203d 204e 6f6e 650a 0a57  hange' = None..W
+00355b00: 4d5f 4f54 5f70 726f 7065 7274 6965 735f  M_OT_properties_
+00355b10: 6564 6974 3a20 2762 6c5f 6f70 6572 6174  edit: 'bl_operat
+00355b20: 6f72 732e 776d 2e57 4d5f 4f54 5f70 726f  ors.wm.WM_OT_pro
+00355b30: 7065 7274 6965 735f 6564 6974 2720 3d20  perties_edit' = 
+00355b40: 4e6f 6e65 0a0a 574d 5f4f 545f 7072 6f70  None..WM_OT_prop
+00355b50: 6572 7469 6573 5f65 6469 745f 7661 6c75  erties_edit_valu
+00355b60: 653a 2027 626c 5f6f 7065 7261 746f 7273  e: 'bl_operators
+00355b70: 2e77 6d2e 574d 5f4f 545f 7072 6f70 6572  .wm.WM_OT_proper
+00355b80: 7469 6573 5f65 6469 745f 7661 6c75 6527  ties_edit_value'
+00355b90: 203d 204e 6f6e 650a 0a57 4d5f 4f54 5f70   = None..WM_OT_p
+00355ba0: 726f 7065 7274 6965 735f 7265 6d6f 7665  roperties_remove
+00355bb0: 3a20 2762 6c5f 6f70 6572 6174 6f72 732e  : 'bl_operators.
+00355bc0: 776d 2e57 4d5f 4f54 5f70 726f 7065 7274  wm.WM_OT_propert
+00355bd0: 6965 735f 7265 6d6f 7665 2720 3d20 4e6f  ies_remove' = No
+00355be0: 6e65 0a0a 574d 5f4f 545f 7379 7369 6e66  ne..WM_OT_sysinf
+00355bf0: 6f3a 2027 626c 5f6f 7065 7261 746f 7273  o: 'bl_operators
+00355c00: 2e77 6d2e 574d 5f4f 545f 7379 7369 6e66  .wm.WM_OT_sysinf
+00355c10: 6f27 203d 204e 6f6e 650a 0a57 4d5f 4f54  o' = None..WM_OT
+00355c20: 5f74 6f6f 6c5f 7365 745f 6279 5f69 643a  _tool_set_by_id:
+00355c30: 2027 626c 5f6f 7065 7261 746f 7273 2e77   'bl_operators.w
+00355c40: 6d2e 574d 5f4f 545f 746f 6f6c 5f73 6574  m.WM_OT_tool_set
+00355c50: 5f62 795f 6964 2720 3d20 4e6f 6e65 0a0a  _by_id' = None..
+00355c60: 574d 5f4f 545f 746f 6f6c 5f73 6574 5f62  WM_OT_tool_set_b
+00355c70: 795f 696e 6465 783a 2027 626c 5f6f 7065  y_index: 'bl_ope
+00355c80: 7261 746f 7273 2e77 6d2e 574d 5f4f 545f  rators.wm.WM_OT_
+00355c90: 746f 6f6c 5f73 6574 5f62 795f 696e 6465  tool_set_by_inde
+00355ca0: 7827 203d 204e 6f6e 650a 0a57 4d5f 4f54  x' = None..WM_OT
+00355cb0: 5f74 6f6f 6c62 6172 3a20 2762 6c5f 6f70  _toolbar: 'bl_op
+00355cc0: 6572 6174 6f72 732e 776d 2e57 4d5f 4f54  erators.wm.WM_OT
+00355cd0: 5f74 6f6f 6c62 6172 2720 3d20 4e6f 6e65  _toolbar' = None
+00355ce0: 0a0a 574d 5f4f 545f 746f 6f6c 6261 725f  ..WM_OT_toolbar_
+00355cf0: 6661 6c6c 6261 636b 5f70 6965 3a20 2762  fallback_pie: 'b
+00355d00: 6c5f 6f70 6572 6174 6f72 732e 776d 2e57  l_operators.wm.W
+00355d10: 4d5f 4f54 5f74 6f6f 6c62 6172 5f66 616c  M_OT_toolbar_fal
+00355d20: 6c62 6163 6b5f 7069 6527 203d 204e 6f6e  lback_pie' = Non
+00355d30: 650a 0a57 4d5f 4f54 5f74 6f6f 6c62 6172  e..WM_OT_toolbar
+00355d40: 5f70 726f 6d70 743a 2027 626c 5f6f 7065  _prompt: 'bl_ope
+00355d50: 7261 746f 7273 2e77 6d2e 574d 5f4f 545f  rators.wm.WM_OT_
+00355d60: 746f 6f6c 6261 725f 7072 6f6d 7074 2720  toolbar_prompt' 
+00355d70: 3d20 4e6f 6e65 0a0a 574d 5f4f 545f 7572  = None..WM_OT_ur
+00355d80: 6c5f 6f70 656e 3a20 2762 6c5f 6f70 6572  l_open: 'bl_oper
+00355d90: 6174 6f72 732e 776d 2e57 4d5f 4f54 5f75  ators.wm.WM_OT_u
+00355da0: 726c 5f6f 7065 6e27 203d 204e 6f6e 650a  rl_open' = None.
+00355db0: 0a57 4d5f 4f54 5f75 726c 5f6f 7065 6e5f  .WM_OT_url_open_
+00355dc0: 7072 6573 6574 3a20 2762 6c5f 6f70 6572  preset: 'bl_oper
+00355dd0: 6174 6f72 732e 776d 2e57 4d5f 4f54 5f75  ators.wm.WM_OT_u
+00355de0: 726c 5f6f 7065 6e5f 7072 6573 6574 2720  rl_open_preset' 
+00355df0: 3d20 4e6f 6e65 0a0a 574f 524b 5350 4143  = None..WORKSPAC
+00355e00: 455f 5054 5f61 6464 6f6e 733a 2027 626c  E_PT_addons: 'bl
+00355e10: 5f75 692e 7072 6f70 6572 7469 6573 5f77  _ui.properties_w
+00355e20: 6f72 6b73 7061 6365 2e57 4f52 4b53 5041  orkspace.WORKSPA
+00355e30: 4345 5f50 545f 6164 646f 6e73 2720 3d20  CE_PT_addons' = 
 00355e40: 4e6f 6e65 0a0a 574f 524b 5350 4143 455f  None..WORKSPACE_
-00355e50: 5054 5f6d 6169 6e3a 2027 626c 5f75 692e  PT_main: 'bl_ui.
-00355e60: 7072 6f70 6572 7469 6573 5f77 6f72 6b73  properties_works
-00355e70: 7061 6365 2e57 4f52 4b53 5041 4345 5f50  pace.WORKSPACE_P
-00355e80: 545f 6d61 696e 2720 3d20 4e6f 6e65 0a0a  T_main' = None..
-00355e90: 574f 524c 445f 5054 5f63 6f6e 7465 7874  WORLD_PT_context
-00355ea0: 5f77 6f72 6c64 3a20 2762 6c5f 7569 2e70  _world: 'bl_ui.p
-00355eb0: 726f 7065 7274 6965 735f 776f 726c 642e  roperties_world.
-00355ec0: 574f 524c 445f 5054 5f63 6f6e 7465 7874  WORLD_PT_context
-00355ed0: 5f77 6f72 6c64 2720 3d20 4e6f 6e65 0a0a  _world' = None..
-00355ee0: 574f 524c 445f 5054 5f63 7573 746f 6d5f  WORLD_PT_custom_
-00355ef0: 7072 6f70 733a 2027 626c 5f75 692e 7072  props: 'bl_ui.pr
-00355f00: 6f70 6572 7469 6573 5f77 6f72 6c64 2e57  operties_world.W
-00355f10: 4f52 4c44 5f50 545f 6375 7374 6f6d 5f70  ORLD_PT_custom_p
-00355f20: 726f 7073 2720 3d20 4e6f 6e65 0a0a 574f  rops' = None..WO
-00355f30: 524c 445f 5054 5f76 6965 7770 6f72 745f  RLD_PT_viewport_
-00355f40: 6469 7370 6c61 793a 2027 626c 5f75 692e  display: 'bl_ui.
-00355f50: 7072 6f70 6572 7469 6573 5f77 6f72 6c64  properties_world
-00355f60: 2e57 4f52 4c44 5f50 545f 7669 6577 706f  .WORLD_PT_viewpo
-00355f70: 7274 5f64 6973 706c 6179 2720 3d20 4e6f  rt_display' = No
-00355f80: 6e65 0a                                  ne.
+00355e50: 5054 5f63 7573 746f 6d5f 7072 6f70 733a  PT_custom_props:
+00355e60: 2027 626c 5f75 692e 7072 6f70 6572 7469   'bl_ui.properti
+00355e70: 6573 5f77 6f72 6b73 7061 6365 2e57 4f52  es_workspace.WOR
+00355e80: 4b53 5041 4345 5f50 545f 6375 7374 6f6d  KSPACE_PT_custom
+00355e90: 5f70 726f 7073 2720 3d20 4e6f 6e65 0a0a  _props' = None..
+00355ea0: 574f 524b 5350 4143 455f 5054 5f6d 6169  WORKSPACE_PT_mai
+00355eb0: 6e3a 2027 626c 5f75 692e 7072 6f70 6572  n: 'bl_ui.proper
+00355ec0: 7469 6573 5f77 6f72 6b73 7061 6365 2e57  ties_workspace.W
+00355ed0: 4f52 4b53 5041 4345 5f50 545f 6d61 696e  ORKSPACE_PT_main
+00355ee0: 2720 3d20 4e6f 6e65 0a0a 574f 524c 445f  ' = None..WORLD_
+00355ef0: 5054 5f63 6f6e 7465 7874 5f77 6f72 6c64  PT_context_world
+00355f00: 3a20 2762 6c5f 7569 2e70 726f 7065 7274  : 'bl_ui.propert
+00355f10: 6965 735f 776f 726c 642e 574f 524c 445f  ies_world.WORLD_
+00355f20: 5054 5f63 6f6e 7465 7874 5f77 6f72 6c64  PT_context_world
+00355f30: 2720 3d20 4e6f 6e65 0a0a 574f 524c 445f  ' = None..WORLD_
+00355f40: 5054 5f63 7573 746f 6d5f 7072 6f70 733a  PT_custom_props:
+00355f50: 2027 626c 5f75 692e 7072 6f70 6572 7469   'bl_ui.properti
+00355f60: 6573 5f77 6f72 6c64 2e57 4f52 4c44 5f50  es_world.WORLD_P
+00355f70: 545f 6375 7374 6f6d 5f70 726f 7073 2720  T_custom_props' 
+00355f80: 3d20 4e6f 6e65 0a0a 574f 524c 445f 5054  = None..WORLD_PT
+00355f90: 5f76 6965 7770 6f72 745f 6469 7370 6c61  _viewport_displa
+00355fa0: 793a 2027 626c 5f75 692e 7072 6f70 6572  y: 'bl_ui.proper
+00355fb0: 7469 6573 5f77 6f72 6c64 2e57 4f52 4c44  ties_world.WORLD
+00355fc0: 5f50 545f 7669 6577 706f 7274 5f64 6973  _PT_viewport_dis
+00355fd0: 706c 6179 2720 3d20 4e6f 6e65 0a         play' = None.
```

### Comparing `fake-bpy-module-latest-20230703/bpy/utils/__init__.py` & `fake-bpy-module-latest-20230704/bpy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/utils/previews.py` & `fake-bpy-module-latest-20230704/bpy/utils/previews.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy/utils/units.py` & `fake-bpy-module-latest-20230704/bpy/utils/units.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy_extras/anim_utils.py` & `fake-bpy-module-latest-20230704/bpy_extras/anim_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,16 +108,16 @@
     '''
 
     pass
 
 
 def bake_action_objects_iter(
         object_action_pairs: typing.
-        Union['bpy.types.Object', 'bpy.types.Action', 'bpy.types.Sequence'],
+        Union['bpy.types.Sequence', 'bpy.types.Action', 'bpy.types.Object'],
         **kwargs):
     ''' An coroutine that bakes actions for multiple objects.
 
     :param object_action_pairs: Sequence of object action tuples, action is the destination for the baked data. When None a new action will be created.
-    :type object_action_pairs: typing.Union['bpy.types.Object', 'bpy.types.Action', 'bpy.types.Sequence']
+    :type object_action_pairs: typing.Union['bpy.types.Sequence', 'bpy.types.Action', 'bpy.types.Object']
     '''
 
     pass
```

### Comparing `fake-bpy-module-latest-20230703/bpy_extras/image_utils.py` & `fake-bpy-module-latest-20230704/bpy_extras/image_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy_extras/io_utils.py` & `fake-bpy-module-latest-20230704/bpy_extras/io_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy_extras/mesh_utils.py` & `fake-bpy-module-latest-20230704/bpy_extras/mesh_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy_extras/node_shader_utils.py` & `fake-bpy-module-latest-20230704/bpy_extras/node_shader_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy_extras/object_utils.py` & `fake-bpy-module-latest-20230704/bpy_extras/object_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy_extras/view3d_utils.py` & `fake-bpy-module-latest-20230704/bpy_extras/view3d_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy_extras/wm_utils/progress_report.py` & `fake-bpy-module-latest-20230704/bpy_extras/wm_utils/progress_report.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/bpy_types.py` & `fake-bpy-module-latest-20230704/bpy_types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/fake_bpy_module_latest.egg-info/PKG-INFO` & `fake-bpy-module-latest-20230704/fake_bpy_module_latest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: fake-bpy-module-latest
-Version: 20230703
+Version: 20230704
 Summary: Collection of the fake Blender Python API module for the code completion.
 Home-page: https://github.com/nutti/fake-bpy-module
 Author: nutti
 Author-email: nutti.metro@gmail.com
 Maintainer: nutti
 Maintainer-email: nutti.metro@gmail.com
 License: MIT
```

### Comparing `fake-bpy-module-latest-20230703/fake_bpy_module_latest.egg-info/SOURCES.txt` & `fake-bpy-module-latest-20230704/fake_bpy_module_latest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/freestyle/chainingiterators.py` & `fake-bpy-module-latest-20230704/freestyle/chainingiterators.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/freestyle/functions.py` & `fake-bpy-module-latest-20230704/freestyle/functions.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/freestyle/predicates.py` & `fake-bpy-module-latest-20230704/freestyle/predicates.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/freestyle/shaders.py` & `fake-bpy-module-latest-20230704/freestyle/shaders.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/freestyle/types.py` & `fake-bpy-module-latest-20230704/freestyle/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/freestyle/utils/ContextFunctions.py` & `fake-bpy-module-latest-20230704/freestyle/utils/ContextFunctions.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/freestyle/utils/__init__.py` & `fake-bpy-module-latest-20230704/freestyle/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/gpu/capabilities.py` & `fake-bpy-module-latest-20230704/gpu/capabilities.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/gpu/matrix.py` & `fake-bpy-module-latest-20230704/gpu/matrix.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/gpu/platform.py` & `fake-bpy-module-latest-20230704/gpu/platform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/gpu/shader.py` & `fake-bpy-module-latest-20230704/gpu/shader.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/gpu/state.py` & `fake-bpy-module-latest-20230704/gpu/state.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/gpu/texture.py` & `fake-bpy-module-latest-20230704/gpu/texture.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/gpu/types.py` & `fake-bpy-module-latest-20230704/gpu/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/gpu_extras/batch.py` & `fake-bpy-module-latest-20230704/gpu_extras/batch.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/gpu_extras/presets.py` & `fake-bpy-module-latest-20230704/gpu_extras/presets.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/idprop/types.py` & `fake-bpy-module-latest-20230704/idprop/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/imbuf/__init__.py` & `fake-bpy-module-latest-20230704/imbuf/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/imbuf/types.py` & `fake-bpy-module-latest-20230704/imbuf/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/keyingsets_builtins.py` & `fake-bpy-module-latest-20230704/keyingsets_builtins.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/keyingsets_utils.py` & `fake-bpy-module-latest-20230704/keyingsets_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/mathutils/__init__.py` & `fake-bpy-module-latest-20230704/mathutils/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/mathutils/bvhtree.py` & `fake-bpy-module-latest-20230704/mathutils/bvhtree.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/mathutils/geometry.py` & `fake-bpy-module-latest-20230704/mathutils/geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/mathutils/kdtree.py` & `fake-bpy-module-latest-20230704/mathutils/kdtree.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/mathutils/noise.py` & `fake-bpy-module-latest-20230704/mathutils/noise.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/nodeitems_builtins.py` & `fake-bpy-module-latest-20230704/nodeitems_builtins.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/nodeitems_utils.py` & `fake-bpy-module-latest-20230704/nodeitems_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/rna_info.py` & `fake-bpy-module-latest-20230704/rna_info.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/rna_keymap_ui.py` & `fake-bpy-module-latest-20230704/rna_keymap_ui.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/rna_prop_ui.py` & `fake-bpy-module-latest-20230704/rna_prop_ui.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/rna_xml.py` & `fake-bpy-module-latest-20230704/rna_xml.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230703/setup.py` & `fake-bpy-module-latest-20230704/setup.py`

 * *Files identical despite different names*

