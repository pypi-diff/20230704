# Comparing `tmp/minecraft-resource-pack-1.3.3.tar.gz` & `tmp/minecraft-resource-pack-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\a\Minecraft-Model-Reader\Minecraft-Model-Reader\dist\.tmp-bgck7h7e\minecraft-resource-pack-1.3.3.tar", last modified: Fri Dec  9 11:24:11 2022, max compression
+gzip compressed data, was "D:\a\Minecraft-Model-Reader\Minecraft-Model-Reader\dist\.tmp-pvausvur\minecraft-resource-pack-1.3.4.tar", last modified: Tue Jul  4 08:40:04 2023, max compression
```

## Comparing `minecraft-resource-pack-1.3.3.tar` & `minecraft-resource-pack-1.3.4.tar`

### file list

```diff
@@ -1,506 +1,503 @@
-drwxrwxrwx   0        0        0        0 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/
--rw-rw-rw-   0        0        0     6954 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/LICENSE
--rw-rw-rw-   0        0        0      236 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/MANIFEST.in
--rw-rw-rw-   0        0        0      487 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/
--rw-rw-rw-   0        0        0      452 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/__pyinstaller/
--rw-rw-rw-   0        0        0       43 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/__pyinstaller/__init__.py
--rw-rw-rw-   0        0        0      112 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/__pyinstaller/hook-minecraft_model_reader.py
--rw-rw-rw-   0        0        0      518 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/_version.py
-drwxrwxrwx   0        0        0        0 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/
--rw-rw-rw-   0        0        0      186 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/amulet/
--rw-rw-rw-   0        0        0        0 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/amulet/__init__.py
--rw-rw-rw-   0        0        0    18894 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/amulet/block.py
--rw-rw-rw-   0        0        0     6410 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/comment_json.py
-drwxrwxrwx   0        0        0        0 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/image/
--rw-rw-rw-   0        0        0      189 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/image/__init__.py
--rw-rw-rw-   0        0        0      176 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/image/missing_no.png
--rw-rw-rw-   0        0        0    11085 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/image/missing_pack_java.png
-drwxrwxrwx   0        0        0        0 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/mesh/
--rw-rw-rw-   0        0        0        0 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/mesh/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/mesh/block/
--rw-rw-rw-   0        0        0       35 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/mesh/block/__init__.py
--rw-rw-rw-   0        0        0    13838 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/mesh/block/block_mesh.py
--rw-rw-rw-   0        0        0     4764 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/mesh/block/cube.py
--rw-rw-rw-   0        0        0      545 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/mesh/block/missing_block.py
--rw-rw-rw-   0        0        0      507 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/mesh/util.py
-drwxrwxrwx   0        0        0        0 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/
--rw-rw-rw-   0        0        0     1908 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/base/
--rw-rw-rw-   0        0        0      105 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/base/__init__.py
--rw-rw-rw-   0        0        0     1128 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/base/resource_pack.py
--rw-rw-rw-   0        0        0     3142 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/base/resource_pack_manager.py
-drwxrwxrwx   0        0        0        0 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/
--rw-rw-rw-   0        0        0      111 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/__init__.py
--rw-rw-rw-   0        0        0  2864161 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/block_palette.json
-drwxrwxrwx   0        0        0        0 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/
--rw-rw-rw-   0        0        0     1065 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/__init__.py
--rw-rw-rw-   0        0        0     1027 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/air.py
--rw-rw-rw-   0        0        0      905 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/base_blockshape.py
--rw-rw-rw-   0        0        0      736 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/bubble_column.py
--rw-rw-rw-   0        0        0     1099 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cake.py
--rw-rw-rw-   0        0        0     1443 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/chest.py
--rw-rw-rw-   0        0        0     1439 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/comparator.py
--rw-rw-rw-   0        0        0     5340 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cross_texture.py
--rw-rw-rw-   0        0        0      449 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cross_texture0.py
--rw-rw-rw-   0        0        0      373 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cross_texture_green.py
--rw-rw-rw-   0        0        0      781 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cube.py
--rw-rw-rw-   0        0        0      688 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/default.py
--rw-rw-rw-   0        0        0     1179 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door.py
--rw-rw-rw-   0        0        0      340 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door1.py
--rw-rw-rw-   0        0        0      340 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door2.py
--rw-rw-rw-   0        0        0      340 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door3.py
--rw-rw-rw-   0        0        0      340 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door4.py
--rw-rw-rw-   0        0        0      340 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door5.py
--rw-rw-rw-   0        0        0      340 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door6.py
--rw-rw-rw-   0        0        0     1225 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/double_plant.py
--rw-rw-rw-   0        0        0      666 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/enchanting_table.py
--rw-rw-rw-   0        0        0      644 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/farmland.py
--rw-rw-rw-   0        0        0      654 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/fence.py
--rw-rw-rw-   0        0        0     1616 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/flat.py
--rw-rw-rw-   0        0        0     1620 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/flat_wall.py
--rw-rw-rw-   0        0        0     1264 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/furnace.py
--rw-rw-rw-   0        0        0      364 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/furnace_lit.py
--rw-rw-rw-   0        0        0      822 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/green_cube.py
--rw-rw-rw-   0        0        0      912 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/ladder.py
--rw-rw-rw-   0        0        0      333 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/lilypad.py
--rw-rw-rw-   0        0        0     1976 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/partial_block.py
--rw-rw-rw-   0        0        0     1318 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/piston.py
--rw-rw-rw-   0        0        0     2160 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/piston_arm.py
--rw-rw-rw-   0        0        0      654 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/portal_frame.py
--rw-rw-rw-   0        0        0      984 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pressure_plate.py
--rw-rw-rw-   0        0        0     1008 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pumpkin.py
--rw-rw-rw-   0        0        0      374 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pumpkin_carved.py
--rw-rw-rw-   0        0        0      365 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pumpkin_lit.py
--rw-rw-rw-   0        0        0      334 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/red_dust.py
--rw-rw-rw-   0        0        0     1506 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/repeater.py
--rw-rw-rw-   0        0        0     1079 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/slab.py
--rw-rw-rw-   0        0        0      444 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/slab_double.py
--rw-rw-rw-   0        0        0     1209 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/tree.py
--rw-rw-rw-   0        0        0      448 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/turtle_egg.py
--rw-rw-rw-   0        0        0     1477 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/vine.py
--rw-rw-rw-   0        0        0      645 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/wall.py
--rw-rw-rw-   0        0        0      876 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/water.py
--rw-rw-rw-   0        0        0    23188 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes.json
--rw-rw-rw-   0        0        0     5219 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/download_resources.py
--rw-rw-rw-   0        0        0     1441 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/resource_pack.py
--rw-rw-rw-   0        0        0    13473 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/resource_pack_manager.py
-drwxrwxrwx   0        0        0        0 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/resource_packs/
-drwxrwxrwx   0        0        0        0 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/resource_packs/bedrock_vanilla_fix/
--rw-rw-rw-   0        0        0      967 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/resource_packs/bedrock_vanilla_fix/blocks.json
--rw-rw-rw-   0        0        0      555 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/resource_packs/bedrock_vanilla_fix/manifest.json
--rw-rw-rw-   0        0        0    32642 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/resource_packs/bedrock_vanilla_fix/pack_icon.png
-drwxrwxrwx   0        0        0        0 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/resource_packs/bedrock_vanilla_fix/textures/
-drwxrwxrwx   0        0        0        0 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/resource_packs/bedrock_vanilla_fix/textures/blocks/
--rw-rw-rw-   0        0        0      580 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/resource_packs/bedrock_vanilla_fix/textures/blocks/grass_carried.png
--rw-rw-rw-   0        0        0      408 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/resource_packs/bedrock_vanilla_fix/textures/blocks/grass_side_carried.png
--rw-rw-rw-   0        0        0      927 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/resource_packs/bedrock_vanilla_fix/textures/blocks/water.png
--rw-rw-rw-   0        0        0      428 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/resource_packs/bedrock_vanilla_fix/textures/terrain_texture.json
--rw-rw-rw-   0        0        0      446 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/sort_blockshapes.py
-drwxrwxrwx   0        0        0        0 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/
--rw-rw-rw-   0        0        0      105 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/__init__.py
--rw-rw-rw-   0        0        0     6500 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/download_resources.py
--rw-rw-rw-   0        0        0     1687 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_pack.py
--rw-rw-rw-   0        0        0    22130 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_pack_manager.py
-drwxrwxrwx   0        0        0        0 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/
-drwxrwxrwx   0        0        0        0 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/
-drwxrwxrwx   0        0        0        0 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/
-drwxrwxrwx   0        0        0        0 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/
-drwxrwxrwx   0        0        0        0 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/
--rw-rw-rw-   0        0        0     1153 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/acacia_sign.json
--rw-rw-rw-   0        0        0      322 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/acacia_wall_sign.json
--rw-rw-rw-   0        0        0     1137 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/birch_sign.json
--rw-rw-rw-   0        0        0      318 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/birch_wall_sign.json
--rw-rw-rw-   0        0        0     1169 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/black_banner.json
--rw-rw-rw-   0        0        0      685 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/black_bed.json
--rw-rw-rw-   0        0        0      326 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/black_wall_banner.json
--rw-rw-rw-   0        0        0     1153 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/blue_banner.json
--rw-rw-rw-   0        0        0      677 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/blue_bed.json
--rw-rw-rw-   0        0        0      322 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/blue_wall_banner.json
--rw-rw-rw-   0        0        0     1169 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/brown_banner.json
--rw-rw-rw-   0        0        0      685 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/brown_bed.json
--rw-rw-rw-   0        0        0      326 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/brown_wall_banner.json
--rw-rw-rw-   0        0        0      888 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/chest.json
--rw-rw-rw-   0        0        0     1265 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/creeper_head.json
--rw-rw-rw-   0        0        0      326 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/creeper_wall_head.json
--rw-rw-rw-   0        0        0     1169 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/crimson_sign.json
--rw-rw-rw-   0        0        0      326 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/crimson_wall_sign.json
--rw-rw-rw-   0        0        0     1153 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/cyan_banner.json
--rw-rw-rw-   0        0        0      677 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/cyan_bed.json
--rw-rw-rw-   0        0        0      322 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/cyan_wall_banner.json
--rw-rw-rw-   0        0        0     1185 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/dark_oak_sign.json
--rw-rw-rw-   0        0        0      330 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/dark_oak_wall_sign.json
--rw-rw-rw-   0        0        0     1249 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/dragon_head.json
--rw-rw-rw-   0        0        0      322 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/dragon_wall_head.json
--rw-rw-rw-   0        0        0      282 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/ender_chest.json
--rw-rw-rw-   0        0        0     1153 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/gray_banner.json
--rw-rw-rw-   0        0        0      677 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/gray_bed.json
--rw-rw-rw-   0        0        0      322 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/gray_wall_banner.json
--rw-rw-rw-   0        0        0     1169 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/green_banner.json
--rw-rw-rw-   0        0        0      685 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/green_bed.json
--rw-rw-rw-   0        0        0      326 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/green_wall_banner.json
--rw-rw-rw-   0        0        0     1153 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/jungle_sign.json
--rw-rw-rw-   0        0        0      322 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/jungle_wall_sign.json
--rw-rw-rw-   0        0        0      947 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/light.json
--rw-rw-rw-   0        0        0     1249 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/light_blue_banner.json
--rw-rw-rw-   0        0        0      725 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/light_blue_bed.json
--rw-rw-rw-   0        0        0      346 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/light_blue_wall_banner.json
--rw-rw-rw-   0        0        0     1249 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/light_gray_banner.json
--rw-rw-rw-   0        0        0      725 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/light_gray_bed.json
--rw-rw-rw-   0        0        0      346 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/light_gray_wall_banner.json
--rw-rw-rw-   0        0        0     1153 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/lime_banner.json
--rw-rw-rw-   0        0        0      677 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/lime_bed.json
--rw-rw-rw-   0        0        0      322 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/lime_wall_banner.json
--rw-rw-rw-   0        0        0     1201 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/magenta_banner.json
--rw-rw-rw-   0        0        0      701 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/magenta_bed.json
--rw-rw-rw-   0        0        0      334 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/magenta_wall_banner.json
--rw-rw-rw-   0        0        0     1185 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/mangrove_sign.json
--rw-rw-rw-   0        0        0      330 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/mangrove_wall_sign.json
--rw-rw-rw-   0        0        0     1105 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/oak_sign.json
--rw-rw-rw-   0        0        0      310 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/oak_wall_sign.json
--rw-rw-rw-   0        0        0     1185 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/orange_banner.json
--rw-rw-rw-   0        0        0      693 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/orange_bed.json
--rw-rw-rw-   0        0        0      330 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/orange_wall_banner.json
--rw-rw-rw-   0        0        0     1153 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/pink_banner.json
--rw-rw-rw-   0        0        0      677 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/pink_bed.json
--rw-rw-rw-   0        0        0      322 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/pink_wall_banner.json
--rw-rw-rw-   0        0        0     1249 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/player_head.json
--rw-rw-rw-   0        0        0      322 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/player_wall_head.json
--rw-rw-rw-   0        0        0     1185 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/purple_banner.json
--rw-rw-rw-   0        0        0      693 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/purple_bed.json
--rw-rw-rw-   0        0        0      330 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/purple_wall_banner.json
--rw-rw-rw-   0        0        0     1137 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/red_banner.json
--rw-rw-rw-   0        0        0      669 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/red_bed.json
--rw-rw-rw-   0        0        0      318 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/red_wall_banner.json
--rw-rw-rw-   0        0        0     1281 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/skeleton_skull.json
--rw-rw-rw-   0        0        0      330 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/skeleton_wall_skull.json
--rw-rw-rw-   0        0        0     1153 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/spruce_sign.json
--rw-rw-rw-   0        0        0      322 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/spruce_wall_sign.json
--rw-rw-rw-   0        0        0       84 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/structure_void.json
--rw-rw-rw-   0        0        0      984 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/trapped_chest.json
--rw-rw-rw-   0        0        0     1153 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/warped_sign.json
--rw-rw-rw-   0        0        0      322 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/warped_wall_sign.json
--rw-rw-rw-   0        0        0     1169 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/white_banner.json
--rw-rw-rw-   0        0        0      685 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/white_bed.json
--rw-rw-rw-   0        0        0      326 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/white_wall_banner.json
--rw-rw-rw-   0        0        0     1393 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/wither_skeleton_skull.json
--rw-rw-rw-   0        0        0      358 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/wither_skeleton_wall_skull.json
--rw-rw-rw-   0        0        0     1185 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/yellow_banner.json
--rw-rw-rw-   0        0        0      693 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/yellow_bed.json
--rw-rw-rw-   0        0        0      330 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/yellow_wall_banner.json
--rw-rw-rw-   0        0        0     1249 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/zombie_head.json
--rw-rw-rw-   0        0        0      322 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/zombie_wall_head.json
-drwxrwxrwx   0        0        0        0 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/
-drwxrwxrwx   0        0        0        0 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/
-drwxrwxrwx   0        0        0        0 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/
--rw-rw-rw-   0        0        0     1862 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/banner_0.json
--rw-rw-rw-   0        0        0     1874 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/banner_1.json
--rw-rw-rw-   0        0        0     1865 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/banner_2.json
--rw-rw-rw-   0        0        0     1871 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/banner_3.json
--rw-rw-rw-   0        0        0      102 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/black_0.json
--rw-rw-rw-   0        0        0      102 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/black_1.json
--rw-rw-rw-   0        0        0      102 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/black_2.json
--rw-rw-rw-   0        0        0      102 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/black_3.json
--rw-rw-rw-   0        0        0      101 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/blue_0.json
--rw-rw-rw-   0        0        0      101 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/blue_1.json
--rw-rw-rw-   0        0        0      101 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/blue_2.json
--rw-rw-rw-   0        0        0      101 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/blue_3.json
--rw-rw-rw-   0        0        0      102 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/brown_0.json
--rw-rw-rw-   0        0        0      102 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/brown_1.json
--rw-rw-rw-   0        0        0      102 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/brown_2.json
--rw-rw-rw-   0        0        0      102 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/brown_3.json
--rw-rw-rw-   0        0        0      101 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/cyan_0.json
--rw-rw-rw-   0        0        0      101 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/cyan_1.json
--rw-rw-rw-   0        0        0      101 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/cyan_2.json
--rw-rw-rw-   0        0        0      101 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/cyan_3.json
--rw-rw-rw-   0        0        0      101 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/gray_0.json
--rw-rw-rw-   0        0        0      101 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/gray_1.json
--rw-rw-rw-   0        0        0      101 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/gray_2.json
--rw-rw-rw-   0        0        0      101 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/gray_3.json
--rw-rw-rw-   0        0        0      102 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/green_0.json
--rw-rw-rw-   0        0        0      102 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/green_1.json
--rw-rw-rw-   0        0        0      102 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/green_2.json
--rw-rw-rw-   0        0        0      102 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/green_3.json
--rw-rw-rw-   0        0        0      107 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/light_blue_0.json
--rw-rw-rw-   0        0        0      107 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/light_blue_1.json
--rw-rw-rw-   0        0        0      107 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/light_blue_2.json
--rw-rw-rw-   0        0        0      107 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/light_blue_3.json
--rw-rw-rw-   0        0        0      107 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/light_gray_0.json
--rw-rw-rw-   0        0        0      107 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/light_gray_1.json
--rw-rw-rw-   0        0        0      107 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/light_gray_2.json
--rw-rw-rw-   0        0        0      107 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/light_gray_3.json
--rw-rw-rw-   0        0        0      101 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/lime_0.json
--rw-rw-rw-   0        0        0      101 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/lime_1.json
--rw-rw-rw-   0        0        0      101 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/lime_2.json
--rw-rw-rw-   0        0        0      101 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/lime_3.json
--rw-rw-rw-   0        0        0      104 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/magenta_0.json
--rw-rw-rw-   0        0        0      104 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/magenta_1.json
--rw-rw-rw-   0        0        0      104 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/magenta_2.json
--rw-rw-rw-   0        0        0      104 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/magenta_3.json
--rw-rw-rw-   0        0        0      103 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/orange_0.json
--rw-rw-rw-   0        0        0      103 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/orange_1.json
--rw-rw-rw-   0        0        0      103 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/orange_2.json
--rw-rw-rw-   0        0        0      103 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/orange_3.json
--rw-rw-rw-   0        0        0      101 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/pink_0.json
--rw-rw-rw-   0        0        0      101 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/pink_1.json
--rw-rw-rw-   0        0        0      101 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/pink_2.json
--rw-rw-rw-   0        0        0      101 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/pink_3.json
--rw-rw-rw-   0        0        0      103 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/purple_0.json
--rw-rw-rw-   0        0        0      103 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/purple_1.json
--rw-rw-rw-   0        0        0      103 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/purple_2.json
--rw-rw-rw-   0        0        0      103 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/purple_3.json
--rw-rw-rw-   0        0        0      100 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/red_0.json
--rw-rw-rw-   0        0        0      100 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/red_1.json
--rw-rw-rw-   0        0        0      100 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/red_2.json
--rw-rw-rw-   0        0        0      100 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/red_3.json
--rw-rw-rw-   0        0        0      102 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/white_0.json
--rw-rw-rw-   0        0        0      102 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/white_1.json
--rw-rw-rw-   0        0        0      102 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/white_2.json
--rw-rw-rw-   0        0        0      102 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/white_3.json
--rw-rw-rw-   0        0        0      103 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/yellow_0.json
--rw-rw-rw-   0        0        0      103 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/yellow_1.json
--rw-rw-rw-   0        0        0      103 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/yellow_2.json
--rw-rw-rw-   0        0        0      103 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/yellow_3.json
--rw-rw-rw-   0        0        0      133 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/barrier.json
-drwxrwxrwx   0        0        0        0 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bed/
--rw-rw-rw-   0        0        0       83 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bed/black_foot.json
--rw-rw-rw-   0        0        0       83 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bed/black_head.json
--rw-rw-rw-   0        0        0       82 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bed/blue_foot.json
--rw-rw-rw-   0        0        0       82 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bed/blue_head.json
--rw-rw-rw-   0        0        0       83 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bed/brown_foot.json
--rw-rw-rw-   0        0        0       83 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bed/brown_head.json
--rw-rw-rw-   0        0        0       82 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bed/cyan_foot.json
--rw-rw-rw-   0        0        0       82 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bed/cyan_head.json
--rw-rw-rw-   0        0        0       82 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bed/gray_foot.json
--rw-rw-rw-   0        0        0       82 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bed/gray_head.json
--rw-rw-rw-   0        0        0       83 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bed/green_foot.json
--rw-rw-rw-   0        0        0       83 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bed/green_head.json
--rw-rw-rw-   0        0        0       88 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bed/light_blue_foot.json
--rw-rw-rw-   0        0        0       88 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bed/light_blue_head.json
--rw-rw-rw-   0        0        0       88 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bed/light_gray_foot.json
--rw-rw-rw-   0        0        0       88 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bed/light_gray_head.json
--rw-rw-rw-   0        0        0       82 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bed/lime_foot.json
--rw-rw-rw-   0        0        0       82 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bed/lime_head.json
--rw-rw-rw-   0        0        0       85 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bed/magenta_foot.json
--rw-rw-rw-   0        0        0       85 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bed/magenta_head.json
--rw-rw-rw-   0        0        0       84 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bed/orange_foot.json
--rw-rw-rw-   0        0        0       84 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bed/orange_head.json
--rw-rw-rw-   0        0        0       82 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bed/pink_foot.json
--rw-rw-rw-   0        0        0       82 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bed/pink_head.json
--rw-rw-rw-   0        0        0       84 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bed/purple_foot.json
--rw-rw-rw-   0        0        0       84 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bed/purple_head.json
--rw-rw-rw-   0        0        0       81 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bed/red_foot.json
--rw-rw-rw-   0        0        0       81 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bed/red_head.json
--rw-rw-rw-   0        0        0       83 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bed/white_foot.json
--rw-rw-rw-   0        0        0       83 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bed/white_head.json
--rw-rw-rw-   0        0        0       84 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bed/yellow_foot.json
--rw-rw-rw-   0        0        0       84 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bed/yellow_head.json
--rw-rw-rw-   0        0        0     1525 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bed_foot.json
--rw-rw-rw-   0        0        0     1535 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bed_head.json
--rw-rw-rw-   0        0        0     1610 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bell_between_walls.json
--rw-rw-rw-   0        0        0     1507 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bell_ceiling.json
--rw-rw-rw-   0        0        0     2669 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bell_floor.json
--rw-rw-rw-   0        0        0     1592 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bell_wall.json
--rw-rw-rw-   0        0        0      153 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/black_shulker_box.json
--rw-rw-rw-   0        0        0      151 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/blue_shulker_box.json
--rw-rw-rw-   0        0        0      153 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/brown_shulker_box.json
--rw-rw-rw-   0        0        0      105 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/chest.json
--rw-rw-rw-   0        0        0     1855 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/chest_base.json
--rw-rw-rw-   0        0        0      115 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/chest_left.json
--rw-rw-rw-   0        0        0     1537 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/chest_left_base.json
--rw-rw-rw-   0        0        0      117 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/chest_right.json
--rw-rw-rw-   0        0        0     1527 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/chest_right_base.json
--rw-rw-rw-   0        0        0      579 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/conduit.json
--rw-rw-rw-   0        0        0      151 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/cyan_shulker_box.json
--rw-rw-rw-   0        0        0      139 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/end_portal.json
--rw-rw-rw-   0        0        0      104 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/ender_chest.json
--rw-rw-rw-   0        0        0      151 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/gray_shulker_box.json
--rw-rw-rw-   0        0        0      153 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/green_shulker_box.json
-drwxrwxrwx   0        0        0        0 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/
-drwxrwxrwx   0        0        0        0 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/
--rw-rw-rw-   0        0        0       99 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/creeper_0.json
--rw-rw-rw-   0        0        0       99 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/creeper_1.json
--rw-rw-rw-   0        0        0       99 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/creeper_2.json
--rw-rw-rw-   0        0        0       99 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/creeper_3.json
--rw-rw-rw-   0        0        0     4816 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_0.json
--rw-rw-rw-   0        0        0     4831 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_1.json
--rw-rw-rw-   0        0        0     4810 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_2.json
--rw-rw-rw-   0        0        0     4824 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_3.json
--rw-rw-rw-   0        0        0      592 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_0.json
--rw-rw-rw-   0        0        0      660 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_1.json
--rw-rw-rw-   0        0        0      657 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_2.json
--rw-rw-rw-   0        0        0      659 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_3.json
--rw-rw-rw-   0        0        0      656 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_0.json
--rw-rw-rw-   0        0        0      660 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_1.json
--rw-rw-rw-   0        0        0      657 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_2.json
--rw-rw-rw-   0        0        0      659 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_3.json
--rw-rw-rw-   0        0        0       90 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/player_0.json
--rw-rw-rw-   0        0        0       90 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/player_1.json
--rw-rw-rw-   0        0        0       90 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/player_2.json
--rw-rw-rw-   0        0        0       90 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/player_3.json
--rw-rw-rw-   0        0        0      101 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/skeleton_0.json
--rw-rw-rw-   0        0        0      101 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/skeleton_1.json
--rw-rw-rw-   0        0        0      101 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/skeleton_2.json
--rw-rw-rw-   0        0        0      101 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/skeleton_3.json
--rw-rw-rw-   0        0        0      108 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/wither_skeleton_0.json
--rw-rw-rw-   0        0        0      108 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/wither_skeleton_1.json
--rw-rw-rw-   0        0        0      108 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/wither_skeleton_2.json
--rw-rw-rw-   0        0        0      108 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/wither_skeleton_3.json
--rw-rw-rw-   0        0        0       98 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/zombie_0.json
--rw-rw-rw-   0        0        0       98 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/zombie_1.json
--rw-rw-rw-   0        0        0       98 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/zombie_2.json
--rw-rw-rw-   0        0        0       98 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/zombie_3.json
-drwxrwxrwx   0        0        0        0 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/wall/
--rw-rw-rw-   0        0        0       96 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/wall/creeper.json
--rw-rw-rw-   0        0        0     3870 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/wall/dragon.json
--rw-rw-rw-   0        0        0      559 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/wall/head.json
--rw-rw-rw-   0        0        0      559 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/wall/head2.json
--rw-rw-rw-   0        0        0       87 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/wall/player.json
--rw-rw-rw-   0        0        0       98 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/wall/skeleton.json
--rw-rw-rw-   0        0        0      105 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/wall/wither_skeleton.json
--rw-rw-rw-   0        0        0       95 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/wall/zombie.json
--rw-rw-rw-   0        0        0      134 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/lava.json
-drwxrwxrwx   0        0        0        0 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/light/
--rw-rw-rw-   0        0        0      133 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/light/level_0.json
--rw-rw-rw-   0        0        0      133 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/light/level_1.json
--rw-rw-rw-   0        0        0      133 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/light/level_10.json
--rw-rw-rw-   0        0        0      133 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/light/level_11.json
--rw-rw-rw-   0        0        0      133 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/light/level_12.json
--rw-rw-rw-   0        0        0      133 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/light/level_13.json
--rw-rw-rw-   0        0        0      133 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/light/level_14.json
--rw-rw-rw-   0        0        0      133 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/light/level_15.json
--rw-rw-rw-   0        0        0      133 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/light/level_2.json
--rw-rw-rw-   0        0        0      133 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/light/level_3.json
--rw-rw-rw-   0        0        0      133 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/light/level_4.json
--rw-rw-rw-   0        0        0      133 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/light/level_5.json
--rw-rw-rw-   0        0        0      133 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/light/level_6.json
--rw-rw-rw-   0        0        0      133 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/light/level_7.json
--rw-rw-rw-   0        0        0      133 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/light/level_8.json
--rw-rw-rw-   0        0        0      133 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/light/level_9.json
--rw-rw-rw-   0        0        0      163 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/light_blue_shulker_box.json
--rw-rw-rw-   0        0        0      163 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/light_gray_shulker_box.json
--rw-rw-rw-   0        0        0      151 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/lime_shulker_box.json
--rw-rw-rw-   0        0        0      157 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/magenta_shulker_box.json
--rw-rw-rw-   0        0        0      151 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/moving_piston.json
--rw-rw-rw-   0        0        0      155 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/orange_shulker_box.json
--rw-rw-rw-   0        0        0      151 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/pink_shulker_box.json
--rw-rw-rw-   0        0        0      155 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/purple_shulker_box.json
--rw-rw-rw-   0        0        0      149 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/red_shulker_box.json
--rw-rw-rw-   0        0        0      141 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/shulker_box.json
-drwxrwxrwx   0        0        0        0 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/
--rw-rw-rw-   0        0        0      127 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/acacia_0.json
--rw-rw-rw-   0        0        0      127 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/acacia_1.json
--rw-rw-rw-   0        0        0      127 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/acacia_2.json
--rw-rw-rw-   0        0        0      127 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/acacia_3.json
--rw-rw-rw-   0        0        0      125 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/birch_0.json
--rw-rw-rw-   0        0        0      125 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/birch_1.json
--rw-rw-rw-   0        0        0      125 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/birch_2.json
--rw-rw-rw-   0        0        0      125 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/birch_3.json
--rw-rw-rw-   0        0        0      129 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/crimson_0.json
--rw-rw-rw-   0        0        0      129 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/crimson_1.json
--rw-rw-rw-   0        0        0      129 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/crimson_2.json
--rw-rw-rw-   0        0        0      129 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/crimson_3.json
--rw-rw-rw-   0        0        0      131 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/dark_oak_0.json
--rw-rw-rw-   0        0        0      131 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/dark_oak_1.json
--rw-rw-rw-   0        0        0      131 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/dark_oak_2.json
--rw-rw-rw-   0        0        0      131 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/dark_oak_3.json
--rw-rw-rw-   0        0        0      127 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/jungle_0.json
--rw-rw-rw-   0        0        0      127 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/jungle_1.json
--rw-rw-rw-   0        0        0      127 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/jungle_2.json
--rw-rw-rw-   0        0        0      127 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/jungle_3.json
--rw-rw-rw-   0        0        0      131 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/mangrove_0.json
--rw-rw-rw-   0        0        0      131 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/mangrove_1.json
--rw-rw-rw-   0        0        0      131 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/mangrove_2.json
--rw-rw-rw-   0        0        0      131 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/mangrove_3.json
--rw-rw-rw-   0        0        0      121 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/oak_0.json
--rw-rw-rw-   0        0        0      121 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/oak_1.json
--rw-rw-rw-   0        0        0      121 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/oak_2.json
--rw-rw-rw-   0        0        0      121 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/oak_3.json
--rw-rw-rw-   0        0        0     1184 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/sign_0.json
--rw-rw-rw-   0        0        0     1173 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/sign_1.json
--rw-rw-rw-   0        0        0     1167 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/sign_2.json
--rw-rw-rw-   0        0        0     1171 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/sign_3.json
--rw-rw-rw-   0        0        0      127 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/spruce_0.json
--rw-rw-rw-   0        0        0      127 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/spruce_1.json
--rw-rw-rw-   0        0        0      127 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/spruce_2.json
--rw-rw-rw-   0        0        0      127 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/spruce_3.json
--rw-rw-rw-   0        0        0      127 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/warped_0.json
--rw-rw-rw-   0        0        0      127 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/warped_1.json
--rw-rw-rw-   0        0        0      127 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/warped_2.json
--rw-rw-rw-   0        0        0      127 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/warped_3.json
--rw-rw-rw-   0        0        0      147 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/structure_void.json
--rw-rw-rw-   0        0        0      106 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/trapped_chest.json
--rw-rw-rw-   0        0        0      116 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/trapped_chest_left.json
--rw-rw-rw-   0        0        0      118 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/trapped_chest_right.json
-drwxrwxrwx   0        0        0        0 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/wall_banner/
--rw-rw-rw-   0        0        0       98 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/wall_banner/black.json
--rw-rw-rw-   0        0        0       97 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/wall_banner/blue.json
--rw-rw-rw-   0        0        0       98 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/wall_banner/brown.json
--rw-rw-rw-   0        0        0       97 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/wall_banner/cyan.json
--rw-rw-rw-   0        0        0       97 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/wall_banner/gray.json
--rw-rw-rw-   0        0        0       98 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/wall_banner/green.json
--rw-rw-rw-   0        0        0      103 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/wall_banner/light_blue.json
--rw-rw-rw-   0        0        0      103 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/wall_banner/light_gray.json
--rw-rw-rw-   0        0        0       97 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/wall_banner/lime.json
--rw-rw-rw-   0        0        0      100 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/wall_banner/magenta.json
--rw-rw-rw-   0        0        0       99 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/wall_banner/orange.json
--rw-rw-rw-   0        0        0       97 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/wall_banner/pink.json
--rw-rw-rw-   0        0        0       99 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/wall_banner/purple.json
--rw-rw-rw-   0        0        0       96 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/wall_banner/red.json
--rw-rw-rw-   0        0        0       98 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/wall_banner/white.json
--rw-rw-rw-   0        0        0       99 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/wall_banner/yellow.json
--rw-rw-rw-   0        0        0     1208 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/wall_banner.json
-drwxrwxrwx   0        0        0        0 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/wall_sign/
--rw-rw-rw-   0        0        0      135 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/wall_sign/acacia.json
--rw-rw-rw-   0        0        0      133 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/wall_sign/birch.json
--rw-rw-rw-   0        0        0      137 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/wall_sign/crimson.json
--rw-rw-rw-   0        0        0      139 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/wall_sign/dark_oak.json
--rw-rw-rw-   0        0        0      135 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/wall_sign/jungle.json
--rw-rw-rw-   0        0        0      139 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/wall_sign/mangrove.json
--rw-rw-rw-   0        0        0      129 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/wall_sign/oak.json
--rw-rw-rw-   0        0        0      135 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/wall_sign/spruce.json
--rw-rw-rw-   0        0        0      588 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/wall_sign/wall_sign.json
--rw-rw-rw-   0        0        0      135 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/wall_sign/warped.json
--rw-rw-rw-   0        0        0      135 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/water.json
--rw-rw-rw-   0        0        0      153 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/white_shulker_box.json
--rw-rw-rw-   0        0        0      155 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/yellow_shulker_box.json
-drwxrwxrwx   0        0        0        0 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/
-drwxrwxrwx   0        0        0        0 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/
-drwxrwxrwx   0        0        0        0 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/banner/
--rw-rw-rw-   0        0        0     2769 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_black.png
--rw-rw-rw-   0        0        0     3786 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_blue.png
--rw-rw-rw-   0        0        0     3707 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_brown.png
--rw-rw-rw-   0        0        0     3813 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_cyan.png
--rw-rw-rw-   0        0        0     3518 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_gray.png
--rw-rw-rw-   0        0        0     3751 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_green.png
--rw-rw-rw-   0        0        0     4220 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_light_blue.png
--rw-rw-rw-   0        0        0     3953 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_light_gray.png
--rw-rw-rw-   0        0        0     4151 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_lime.png
--rw-rw-rw-   0        0        0     4178 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_magenta.png
--rw-rw-rw-   0        0        0     4298 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_orange.png
--rw-rw-rw-   0        0        0     4205 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_pink.png
--rw-rw-rw-   0        0        0     4056 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_purple.png
--rw-rw-rw-   0        0        0     3790 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_red.png
--rw-rw-rw-   0        0        0     3985 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_white.png
--rw-rw-rw-   0        0        0     4457 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_yellow.png
--rw-rw-rw-   0        0        0      651 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/barrier.png
--rw-rw-rw-   0        0        0     1265 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/end_portal.png
--rw-rw-rw-   0        0        0     1286 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/lava.png
--rw-rw-rw-   0        0        0     1405 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/structure_void.png
--rw-rw-rw-   0        0        0      927 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/water.png
--rw-rw-rw-   0        0        0      117 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/pack.mcmeta
--rw-rw-rw-   0        0        0    22749 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/pack.png
--rw-rw-rw-   0        0        0      299 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/unknown_resource_pack.py
-drwxrwxrwx   0        0        0        0 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_resource_pack.egg-info/
--rw-rw-rw-   0        0        0      487 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_resource_pack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    53805 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_resource_pack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_resource_pack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_resource_pack.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-12-09 11:24:10.000000 minecraft-resource-pack-1.3.3/minecraft_resource_pack.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      156 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_resource_pack.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/minecraft_resource_pack.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      135 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/pyproject.toml
--rw-rw-rw-   0        0        0     1167 2022-12-09 11:24:11.000000 minecraft-resource-pack-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0      142 2022-12-09 11:23:33.000000 minecraft-resource-pack-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:40:04.000000 minecraft-resource-pack-1.3.4/
+-rw-rw-rw-   0        0        0     6954 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/LICENSE
+-rw-rw-rw-   0        0        0      236 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      487 2023-07-04 08:40:04.000000 minecraft-resource-pack-1.3.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-04 08:40:04.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/
+-rw-rw-rw-   0        0        0      910 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:40:01.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/__pyinstaller/
+-rw-rw-rw-   0        0        0       43 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/__pyinstaller/__init__.py
+-rw-rw-rw-   0        0        0      112 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/__pyinstaller/hook-minecraft_model_reader.py
+-rw-rw-rw-   0        0        0      518 2023-07-04 08:40:04.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/_version.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:40:01.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/
+-rw-rw-rw-   0        0        0      186 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:40:01.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/amulet/
+-rw-rw-rw-   0        0        0        0 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/amulet/__init__.py
+-rw-rw-rw-   0        0        0    18894 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/amulet/block.py
+-rw-rw-rw-   0        0        0     6410 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/comment_json.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:40:01.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/image/
+-rw-rw-rw-   0        0        0      189 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/image/__init__.py
+-rw-rw-rw-   0        0        0      176 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/image/missing_no.png
+-rw-rw-rw-   0        0        0    11085 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/image/missing_pack_java.png
+drwxrwxrwx   0        0        0        0 2023-07-04 08:40:01.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/mesh/
+-rw-rw-rw-   0        0        0        0 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/mesh/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:40:01.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/mesh/block/
+-rw-rw-rw-   0        0        0       35 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/mesh/block/__init__.py
+-rw-rw-rw-   0        0        0    13838 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/mesh/block/block_mesh.py
+-rw-rw-rw-   0        0        0     4764 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/mesh/block/cube.py
+-rw-rw-rw-   0        0        0      545 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/mesh/block/missing_block.py
+-rw-rw-rw-   0        0        0      507 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/mesh/util.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:40:01.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/
+-rw-rw-rw-   0        0        0     1908 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:40:01.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/base/
+-rw-rw-rw-   0        0        0      105 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/base/__init__.py
+-rw-rw-rw-   0        0        0     1128 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/base/resource_pack.py
+-rw-rw-rw-   0        0        0     2908 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/base/resource_pack_manager.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:40:02.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/
+-rw-rw-rw-   0        0        0      111 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:40:02.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/
+-rw-rw-rw-   0        0        0      967 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/blocks.json
+-rw-rw-rw-   0        0        0      555 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/manifest.json
+-rw-rw-rw-   0        0        0    32642 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/pack_icon.png
+drwxrwxrwx   0        0        0        0 2023-07-04 08:40:02.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/
+drwxrwxrwx   0        0        0        0 2023-07-04 08:40:03.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/blocks/
+-rw-rw-rw-   0        0        0      580 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/blocks/grass_carried.png
+-rw-rw-rw-   0        0        0      408 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/blocks/grass_side_carried.png
+-rw-rw-rw-   0        0        0      927 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/blocks/water.png
+-rw-rw-rw-   0        0        0      428 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/terrain_texture.json
+-rw-rw-rw-   0        0        0  2864161 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/block_palette.json
+drwxrwxrwx   0        0        0        0 2023-07-04 08:40:04.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/
+-rw-rw-rw-   0        0        0     1065 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/__init__.py
+-rw-rw-rw-   0        0        0     1027 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/air.py
+-rw-rw-rw-   0        0        0      905 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/base_blockshape.py
+-rw-rw-rw-   0        0        0      736 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/bubble_column.py
+-rw-rw-rw-   0        0        0     1099 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cake.py
+-rw-rw-rw-   0        0        0     1443 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/chest.py
+-rw-rw-rw-   0        0        0     1439 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/comparator.py
+-rw-rw-rw-   0        0        0     5340 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cross_texture.py
+-rw-rw-rw-   0        0        0      449 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cross_texture0.py
+-rw-rw-rw-   0        0        0      373 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cross_texture_green.py
+-rw-rw-rw-   0        0        0      781 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cube.py
+-rw-rw-rw-   0        0        0      688 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/default.py
+-rw-rw-rw-   0        0        0     1179 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door.py
+-rw-rw-rw-   0        0        0      340 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door1.py
+-rw-rw-rw-   0        0        0      340 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door2.py
+-rw-rw-rw-   0        0        0      340 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door3.py
+-rw-rw-rw-   0        0        0      340 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door4.py
+-rw-rw-rw-   0        0        0      340 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door5.py
+-rw-rw-rw-   0        0        0      340 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door6.py
+-rw-rw-rw-   0        0        0     1225 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/double_plant.py
+-rw-rw-rw-   0        0        0      666 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/enchanting_table.py
+-rw-rw-rw-   0        0        0      644 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/farmland.py
+-rw-rw-rw-   0        0        0      654 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/fence.py
+-rw-rw-rw-   0        0        0     1616 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/flat.py
+-rw-rw-rw-   0        0        0     1620 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/flat_wall.py
+-rw-rw-rw-   0        0        0     1264 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/furnace.py
+-rw-rw-rw-   0        0        0      364 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/furnace_lit.py
+-rw-rw-rw-   0        0        0      822 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/green_cube.py
+-rw-rw-rw-   0        0        0      912 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/ladder.py
+-rw-rw-rw-   0        0        0      333 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/lilypad.py
+-rw-rw-rw-   0        0        0     1976 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/partial_block.py
+-rw-rw-rw-   0        0        0     1318 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/piston.py
+-rw-rw-rw-   0        0        0     2160 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/piston_arm.py
+-rw-rw-rw-   0        0        0      654 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/portal_frame.py
+-rw-rw-rw-   0        0        0      984 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pressure_plate.py
+-rw-rw-rw-   0        0        0     1008 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pumpkin.py
+-rw-rw-rw-   0        0        0      374 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pumpkin_carved.py
+-rw-rw-rw-   0        0        0      365 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pumpkin_lit.py
+-rw-rw-rw-   0        0        0      334 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/red_dust.py
+-rw-rw-rw-   0        0        0     1506 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/repeater.py
+-rw-rw-rw-   0        0        0     1079 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/slab.py
+-rw-rw-rw-   0        0        0      444 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/slab_double.py
+-rw-rw-rw-   0        0        0     1209 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/tree.py
+-rw-rw-rw-   0        0        0      448 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/turtle_egg.py
+-rw-rw-rw-   0        0        0     1477 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/vine.py
+-rw-rw-rw-   0        0        0      645 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/wall.py
+-rw-rw-rw-   0        0        0      876 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/water.py
+-rw-rw-rw-   0        0        0    23188 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes.json
+-rw-rw-rw-   0        0        0     5220 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/download_resources.py
+-rw-rw-rw-   0        0        0     1441 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/resource_pack.py
+-rw-rw-rw-   0        0        0    13738 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/resource_pack_manager.py
+-rw-rw-rw-   0        0        0      446 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/sort_blockshapes.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:40:04.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/
+-rw-rw-rw-   0        0        0      105 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/__init__.py
+-rw-rw-rw-   0        0        0     6399 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/download_resources.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:40:04.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/
+drwxrwxrwx   0        0        0        0 2023-07-04 08:40:01.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/
+drwxrwxrwx   0        0        0        0 2023-07-04 08:40:01.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/
+drwxrwxrwx   0        0        0        0 2023-07-04 08:40:04.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/
+-rw-rw-rw-   0        0        0     1153 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/acacia_sign.json
+-rw-rw-rw-   0        0        0      322 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/acacia_wall_sign.json
+-rw-rw-rw-   0        0        0     1137 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/birch_sign.json
+-rw-rw-rw-   0        0        0      318 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/birch_wall_sign.json
+-rw-rw-rw-   0        0        0     1169 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/black_banner.json
+-rw-rw-rw-   0        0        0      685 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/black_bed.json
+-rw-rw-rw-   0        0        0      326 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/black_wall_banner.json
+-rw-rw-rw-   0        0        0     1153 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/blue_banner.json
+-rw-rw-rw-   0        0        0      677 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/blue_bed.json
+-rw-rw-rw-   0        0        0      322 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/blue_wall_banner.json
+-rw-rw-rw-   0        0        0     1169 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/brown_banner.json
+-rw-rw-rw-   0        0        0      685 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/brown_bed.json
+-rw-rw-rw-   0        0        0      326 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/brown_wall_banner.json
+-rw-rw-rw-   0        0        0      888 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/chest.json
+-rw-rw-rw-   0        0        0     1265 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/creeper_head.json
+-rw-rw-rw-   0        0        0      326 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/creeper_wall_head.json
+-rw-rw-rw-   0        0        0     1169 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/crimson_sign.json
+-rw-rw-rw-   0        0        0      326 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/crimson_wall_sign.json
+-rw-rw-rw-   0        0        0     1153 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/cyan_banner.json
+-rw-rw-rw-   0        0        0      677 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/cyan_bed.json
+-rw-rw-rw-   0        0        0      322 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/cyan_wall_banner.json
+-rw-rw-rw-   0        0        0     1185 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/dark_oak_sign.json
+-rw-rw-rw-   0        0        0      330 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/dark_oak_wall_sign.json
+-rw-rw-rw-   0        0        0     1249 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/dragon_head.json
+-rw-rw-rw-   0        0        0      322 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/dragon_wall_head.json
+-rw-rw-rw-   0        0        0      282 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/ender_chest.json
+-rw-rw-rw-   0        0        0     1153 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/gray_banner.json
+-rw-rw-rw-   0        0        0      677 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/gray_bed.json
+-rw-rw-rw-   0        0        0      322 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/gray_wall_banner.json
+-rw-rw-rw-   0        0        0     1169 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/green_banner.json
+-rw-rw-rw-   0        0        0      685 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/green_bed.json
+-rw-rw-rw-   0        0        0      326 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/green_wall_banner.json
+-rw-rw-rw-   0        0        0     1153 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/jungle_sign.json
+-rw-rw-rw-   0        0        0      322 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/jungle_wall_sign.json
+-rw-rw-rw-   0        0        0      947 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light.json
+-rw-rw-rw-   0        0        0     1249 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_blue_banner.json
+-rw-rw-rw-   0        0        0      725 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_blue_bed.json
+-rw-rw-rw-   0        0        0      346 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_blue_wall_banner.json
+-rw-rw-rw-   0        0        0     1249 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_gray_banner.json
+-rw-rw-rw-   0        0        0      725 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_gray_bed.json
+-rw-rw-rw-   0        0        0      346 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_gray_wall_banner.json
+-rw-rw-rw-   0        0        0     1153 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/lime_banner.json
+-rw-rw-rw-   0        0        0      677 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/lime_bed.json
+-rw-rw-rw-   0        0        0      322 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/lime_wall_banner.json
+-rw-rw-rw-   0        0        0     1201 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/magenta_banner.json
+-rw-rw-rw-   0        0        0      701 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/magenta_bed.json
+-rw-rw-rw-   0        0        0      334 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/magenta_wall_banner.json
+-rw-rw-rw-   0        0        0     1185 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/mangrove_sign.json
+-rw-rw-rw-   0        0        0      330 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/mangrove_wall_sign.json
+-rw-rw-rw-   0        0        0     1105 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/oak_sign.json
+-rw-rw-rw-   0        0        0      310 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/oak_wall_sign.json
+-rw-rw-rw-   0        0        0     1185 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/orange_banner.json
+-rw-rw-rw-   0        0        0      693 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/orange_bed.json
+-rw-rw-rw-   0        0        0      330 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/orange_wall_banner.json
+-rw-rw-rw-   0        0        0     1153 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/pink_banner.json
+-rw-rw-rw-   0        0        0      677 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/pink_bed.json
+-rw-rw-rw-   0        0        0      322 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/pink_wall_banner.json
+-rw-rw-rw-   0        0        0     1249 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/player_head.json
+-rw-rw-rw-   0        0        0      322 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/player_wall_head.json
+-rw-rw-rw-   0        0        0     1185 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/purple_banner.json
+-rw-rw-rw-   0        0        0      693 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/purple_bed.json
+-rw-rw-rw-   0        0        0      330 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/purple_wall_banner.json
+-rw-rw-rw-   0        0        0     1137 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/red_banner.json
+-rw-rw-rw-   0        0        0      669 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/red_bed.json
+-rw-rw-rw-   0        0        0      318 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/red_wall_banner.json
+-rw-rw-rw-   0        0        0     1281 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/skeleton_skull.json
+-rw-rw-rw-   0        0        0      330 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/skeleton_wall_skull.json
+-rw-rw-rw-   0        0        0     1153 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/spruce_sign.json
+-rw-rw-rw-   0        0        0      322 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/spruce_wall_sign.json
+-rw-rw-rw-   0        0        0       84 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/structure_void.json
+-rw-rw-rw-   0        0        0      984 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/trapped_chest.json
+-rw-rw-rw-   0        0        0     1153 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/warped_sign.json
+-rw-rw-rw-   0        0        0      322 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/warped_wall_sign.json
+-rw-rw-rw-   0        0        0     1169 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/white_banner.json
+-rw-rw-rw-   0        0        0      685 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/white_bed.json
+-rw-rw-rw-   0        0        0      326 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/white_wall_banner.json
+-rw-rw-rw-   0        0        0     1393 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/wither_skeleton_skull.json
+-rw-rw-rw-   0        0        0      358 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/wither_skeleton_wall_skull.json
+-rw-rw-rw-   0        0        0     1185 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/yellow_banner.json
+-rw-rw-rw-   0        0        0      693 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/yellow_bed.json
+-rw-rw-rw-   0        0        0      330 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/yellow_wall_banner.json
+-rw-rw-rw-   0        0        0     1249 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/zombie_head.json
+-rw-rw-rw-   0        0        0      322 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/zombie_wall_head.json
+drwxrwxrwx   0        0        0        0 2023-07-04 08:40:01.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/
+drwxrwxrwx   0        0        0        0 2023-07-04 08:40:04.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/
+drwxrwxrwx   0        0        0        0 2023-07-04 08:40:04.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/
+-rw-rw-rw-   0        0        0     1862 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_0.json
+-rw-rw-rw-   0        0        0     1874 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_1.json
+-rw-rw-rw-   0        0        0     1865 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_2.json
+-rw-rw-rw-   0        0        0     1871 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_3.json
+-rw-rw-rw-   0        0        0      102 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/black_0.json
+-rw-rw-rw-   0        0        0      102 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/black_1.json
+-rw-rw-rw-   0        0        0      102 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/black_2.json
+-rw-rw-rw-   0        0        0      102 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/black_3.json
+-rw-rw-rw-   0        0        0      101 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/blue_0.json
+-rw-rw-rw-   0        0        0      101 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/blue_1.json
+-rw-rw-rw-   0        0        0      101 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/blue_2.json
+-rw-rw-rw-   0        0        0      101 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/blue_3.json
+-rw-rw-rw-   0        0        0      102 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/brown_0.json
+-rw-rw-rw-   0        0        0      102 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/brown_1.json
+-rw-rw-rw-   0        0        0      102 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/brown_2.json
+-rw-rw-rw-   0        0        0      102 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/brown_3.json
+-rw-rw-rw-   0        0        0      101 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/cyan_0.json
+-rw-rw-rw-   0        0        0      101 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/cyan_1.json
+-rw-rw-rw-   0        0        0      101 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/cyan_2.json
+-rw-rw-rw-   0        0        0      101 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/cyan_3.json
+-rw-rw-rw-   0        0        0      101 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/gray_0.json
+-rw-rw-rw-   0        0        0      101 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/gray_1.json
+-rw-rw-rw-   0        0        0      101 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/gray_2.json
+-rw-rw-rw-   0        0        0      101 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/gray_3.json
+-rw-rw-rw-   0        0        0      102 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/green_0.json
+-rw-rw-rw-   0        0        0      102 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/green_1.json
+-rw-rw-rw-   0        0        0      102 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/green_2.json
+-rw-rw-rw-   0        0        0      102 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/green_3.json
+-rw-rw-rw-   0        0        0      107 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_blue_0.json
+-rw-rw-rw-   0        0        0      107 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_blue_1.json
+-rw-rw-rw-   0        0        0      107 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_blue_2.json
+-rw-rw-rw-   0        0        0      107 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_blue_3.json
+-rw-rw-rw-   0        0        0      107 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_gray_0.json
+-rw-rw-rw-   0        0        0      107 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_gray_1.json
+-rw-rw-rw-   0        0        0      107 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_gray_2.json
+-rw-rw-rw-   0        0        0      107 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_gray_3.json
+-rw-rw-rw-   0        0        0      101 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/lime_0.json
+-rw-rw-rw-   0        0        0      101 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/lime_1.json
+-rw-rw-rw-   0        0        0      101 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/lime_2.json
+-rw-rw-rw-   0        0        0      101 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/lime_3.json
+-rw-rw-rw-   0        0        0      104 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/magenta_0.json
+-rw-rw-rw-   0        0        0      104 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/magenta_1.json
+-rw-rw-rw-   0        0        0      104 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/magenta_2.json
+-rw-rw-rw-   0        0        0      104 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/magenta_3.json
+-rw-rw-rw-   0        0        0      103 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/orange_0.json
+-rw-rw-rw-   0        0        0      103 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/orange_1.json
+-rw-rw-rw-   0        0        0      103 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/orange_2.json
+-rw-rw-rw-   0        0        0      103 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/orange_3.json
+-rw-rw-rw-   0        0        0      101 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/pink_0.json
+-rw-rw-rw-   0        0        0      101 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/pink_1.json
+-rw-rw-rw-   0        0        0      101 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/pink_2.json
+-rw-rw-rw-   0        0        0      101 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/pink_3.json
+-rw-rw-rw-   0        0        0      103 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/purple_0.json
+-rw-rw-rw-   0        0        0      103 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/purple_1.json
+-rw-rw-rw-   0        0        0      103 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/purple_2.json
+-rw-rw-rw-   0        0        0      103 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/purple_3.json
+-rw-rw-rw-   0        0        0      100 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/red_0.json
+-rw-rw-rw-   0        0        0      100 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/red_1.json
+-rw-rw-rw-   0        0        0      100 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/red_2.json
+-rw-rw-rw-   0        0        0      100 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/red_3.json
+-rw-rw-rw-   0        0        0      102 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/white_0.json
+-rw-rw-rw-   0        0        0      102 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/white_1.json
+-rw-rw-rw-   0        0        0      102 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/white_2.json
+-rw-rw-rw-   0        0        0      102 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/white_3.json
+-rw-rw-rw-   0        0        0      103 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/yellow_0.json
+-rw-rw-rw-   0        0        0      103 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/yellow_1.json
+-rw-rw-rw-   0        0        0      103 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/yellow_2.json
+-rw-rw-rw-   0        0        0      103 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/yellow_3.json
+-rw-rw-rw-   0        0        0      133 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/barrier.json
+drwxrwxrwx   0        0        0        0 2023-07-04 08:40:04.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/
+-rw-rw-rw-   0        0        0       83 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/black_foot.json
+-rw-rw-rw-   0        0        0       83 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/black_head.json
+-rw-rw-rw-   0        0        0       82 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/blue_foot.json
+-rw-rw-rw-   0        0        0       82 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/blue_head.json
+-rw-rw-rw-   0        0        0       83 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/brown_foot.json
+-rw-rw-rw-   0        0        0       83 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/brown_head.json
+-rw-rw-rw-   0        0        0       82 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/cyan_foot.json
+-rw-rw-rw-   0        0        0       82 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/cyan_head.json
+-rw-rw-rw-   0        0        0       82 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/gray_foot.json
+-rw-rw-rw-   0        0        0       82 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/gray_head.json
+-rw-rw-rw-   0        0        0       83 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/green_foot.json
+-rw-rw-rw-   0        0        0       83 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/green_head.json
+-rw-rw-rw-   0        0        0       88 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/light_blue_foot.json
+-rw-rw-rw-   0        0        0       88 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/light_blue_head.json
+-rw-rw-rw-   0        0        0       88 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/light_gray_foot.json
+-rw-rw-rw-   0        0        0       88 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/light_gray_head.json
+-rw-rw-rw-   0        0        0       82 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/lime_foot.json
+-rw-rw-rw-   0        0        0       82 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/lime_head.json
+-rw-rw-rw-   0        0        0       85 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/magenta_foot.json
+-rw-rw-rw-   0        0        0       85 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/magenta_head.json
+-rw-rw-rw-   0        0        0       84 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/orange_foot.json
+-rw-rw-rw-   0        0        0       84 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/orange_head.json
+-rw-rw-rw-   0        0        0       82 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/pink_foot.json
+-rw-rw-rw-   0        0        0       82 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/pink_head.json
+-rw-rw-rw-   0        0        0       84 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/purple_foot.json
+-rw-rw-rw-   0        0        0       84 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/purple_head.json
+-rw-rw-rw-   0        0        0       81 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/red_foot.json
+-rw-rw-rw-   0        0        0       81 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/red_head.json
+-rw-rw-rw-   0        0        0       83 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/white_foot.json
+-rw-rw-rw-   0        0        0       83 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/white_head.json
+-rw-rw-rw-   0        0        0       84 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/yellow_foot.json
+-rw-rw-rw-   0        0        0       84 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/yellow_head.json
+-rw-rw-rw-   0        0        0     1525 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed_foot.json
+-rw-rw-rw-   0        0        0     1535 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed_head.json
+-rw-rw-rw-   0        0        0     1610 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_between_walls.json
+-rw-rw-rw-   0        0        0     1507 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_ceiling.json
+-rw-rw-rw-   0        0        0     2669 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_floor.json
+-rw-rw-rw-   0        0        0     1592 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_wall.json
+-rw-rw-rw-   0        0        0      153 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/black_shulker_box.json
+-rw-rw-rw-   0        0        0      151 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/blue_shulker_box.json
+-rw-rw-rw-   0        0        0      153 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/brown_shulker_box.json
+-rw-rw-rw-   0        0        0      105 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest.json
+-rw-rw-rw-   0        0        0     1855 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_base.json
+-rw-rw-rw-   0        0        0      115 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_left.json
+-rw-rw-rw-   0        0        0     1537 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_left_base.json
+-rw-rw-rw-   0        0        0      117 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_right.json
+-rw-rw-rw-   0        0        0     1527 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_right_base.json
+-rw-rw-rw-   0        0        0      579 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/conduit.json
+-rw-rw-rw-   0        0        0      151 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/cyan_shulker_box.json
+-rw-rw-rw-   0        0        0      139 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/end_portal.json
+-rw-rw-rw-   0        0        0      104 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/ender_chest.json
+-rw-rw-rw-   0        0        0      151 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/gray_shulker_box.json
+-rw-rw-rw-   0        0        0      153 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/green_shulker_box.json
+drwxrwxrwx   0        0        0        0 2023-07-04 08:40:01.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/
+drwxrwxrwx   0        0        0        0 2023-07-04 08:40:04.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/
+-rw-rw-rw-   0        0        0       99 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/creeper_0.json
+-rw-rw-rw-   0        0        0       99 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/creeper_1.json
+-rw-rw-rw-   0        0        0       99 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/creeper_2.json
+-rw-rw-rw-   0        0        0       99 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/creeper_3.json
+-rw-rw-rw-   0        0        0     4816 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_0.json
+-rw-rw-rw-   0        0        0     4831 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_1.json
+-rw-rw-rw-   0        0        0     4810 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_2.json
+-rw-rw-rw-   0        0        0     4824 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_3.json
+-rw-rw-rw-   0        0        0      592 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_0.json
+-rw-rw-rw-   0        0        0      660 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_1.json
+-rw-rw-rw-   0        0        0      657 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_2.json
+-rw-rw-rw-   0        0        0      659 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_3.json
+-rw-rw-rw-   0        0        0      656 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_0.json
+-rw-rw-rw-   0        0        0      660 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_1.json
+-rw-rw-rw-   0        0        0      657 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_2.json
+-rw-rw-rw-   0        0        0      659 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_3.json
+-rw-rw-rw-   0        0        0       90 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/player_0.json
+-rw-rw-rw-   0        0        0       90 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/player_1.json
+-rw-rw-rw-   0        0        0       90 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/player_2.json
+-rw-rw-rw-   0        0        0       90 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/player_3.json
+-rw-rw-rw-   0        0        0      101 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/skeleton_0.json
+-rw-rw-rw-   0        0        0      101 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/skeleton_1.json
+-rw-rw-rw-   0        0        0      101 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/skeleton_2.json
+-rw-rw-rw-   0        0        0      101 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/skeleton_3.json
+-rw-rw-rw-   0        0        0      108 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/wither_skeleton_0.json
+-rw-rw-rw-   0        0        0      108 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/wither_skeleton_1.json
+-rw-rw-rw-   0        0        0      108 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/wither_skeleton_2.json
+-rw-rw-rw-   0        0        0      108 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/wither_skeleton_3.json
+-rw-rw-rw-   0        0        0       98 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/zombie_0.json
+-rw-rw-rw-   0        0        0       98 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/zombie_1.json
+-rw-rw-rw-   0        0        0       98 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/zombie_2.json
+-rw-rw-rw-   0        0        0       98 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/zombie_3.json
+drwxrwxrwx   0        0        0        0 2023-07-04 08:40:04.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/
+-rw-rw-rw-   0        0        0       96 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/creeper.json
+-rw-rw-rw-   0        0        0     3870 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/dragon.json
+-rw-rw-rw-   0        0        0      559 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/head.json
+-rw-rw-rw-   0        0        0      559 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/head2.json
+-rw-rw-rw-   0        0        0       87 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/player.json
+-rw-rw-rw-   0        0        0       98 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/skeleton.json
+-rw-rw-rw-   0        0        0      105 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/wither_skeleton.json
+-rw-rw-rw-   0        0        0       95 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/zombie.json
+-rw-rw-rw-   0        0        0      134 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/lava.json
+drwxrwxrwx   0        0        0        0 2023-07-04 08:40:04.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/
+-rw-rw-rw-   0        0        0      133 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_0.json
+-rw-rw-rw-   0        0        0      133 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_1.json
+-rw-rw-rw-   0        0        0      133 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_10.json
+-rw-rw-rw-   0        0        0      133 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_11.json
+-rw-rw-rw-   0        0        0      133 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_12.json
+-rw-rw-rw-   0        0        0      133 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_13.json
+-rw-rw-rw-   0        0        0      133 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_14.json
+-rw-rw-rw-   0        0        0      133 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_15.json
+-rw-rw-rw-   0        0        0      133 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_2.json
+-rw-rw-rw-   0        0        0      133 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_3.json
+-rw-rw-rw-   0        0        0      133 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_4.json
+-rw-rw-rw-   0        0        0      133 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_5.json
+-rw-rw-rw-   0        0        0      133 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_6.json
+-rw-rw-rw-   0        0        0      133 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_7.json
+-rw-rw-rw-   0        0        0      133 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_8.json
+-rw-rw-rw-   0        0        0      133 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_9.json
+-rw-rw-rw-   0        0        0      163 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light_blue_shulker_box.json
+-rw-rw-rw-   0        0        0      163 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light_gray_shulker_box.json
+-rw-rw-rw-   0        0        0      151 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/lime_shulker_box.json
+-rw-rw-rw-   0        0        0      157 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/magenta_shulker_box.json
+-rw-rw-rw-   0        0        0      151 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/moving_piston.json
+-rw-rw-rw-   0        0        0      155 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/orange_shulker_box.json
+-rw-rw-rw-   0        0        0      151 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/pink_shulker_box.json
+-rw-rw-rw-   0        0        0      155 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/purple_shulker_box.json
+-rw-rw-rw-   0        0        0      149 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/red_shulker_box.json
+-rw-rw-rw-   0        0        0      141 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/shulker_box.json
+drwxrwxrwx   0        0        0        0 2023-07-04 08:40:04.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/
+-rw-rw-rw-   0        0        0      127 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/acacia_0.json
+-rw-rw-rw-   0        0        0      127 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/acacia_1.json
+-rw-rw-rw-   0        0        0      127 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/acacia_2.json
+-rw-rw-rw-   0        0        0      127 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/acacia_3.json
+-rw-rw-rw-   0        0        0      125 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/birch_0.json
+-rw-rw-rw-   0        0        0      125 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/birch_1.json
+-rw-rw-rw-   0        0        0      125 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/birch_2.json
+-rw-rw-rw-   0        0        0      125 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/birch_3.json
+-rw-rw-rw-   0        0        0      129 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/crimson_0.json
+-rw-rw-rw-   0        0        0      129 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/crimson_1.json
+-rw-rw-rw-   0        0        0      129 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/crimson_2.json
+-rw-rw-rw-   0        0        0      129 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/crimson_3.json
+-rw-rw-rw-   0        0        0      131 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/dark_oak_0.json
+-rw-rw-rw-   0        0        0      131 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/dark_oak_1.json
+-rw-rw-rw-   0        0        0      131 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/dark_oak_2.json
+-rw-rw-rw-   0        0        0      131 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/dark_oak_3.json
+-rw-rw-rw-   0        0        0      127 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/jungle_0.json
+-rw-rw-rw-   0        0        0      127 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/jungle_1.json
+-rw-rw-rw-   0        0        0      127 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/jungle_2.json
+-rw-rw-rw-   0        0        0      127 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/jungle_3.json
+-rw-rw-rw-   0        0        0      131 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/mangrove_0.json
+-rw-rw-rw-   0        0        0      131 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/mangrove_1.json
+-rw-rw-rw-   0        0        0      131 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/mangrove_2.json
+-rw-rw-rw-   0        0        0      131 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/mangrove_3.json
+-rw-rw-rw-   0        0        0      121 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/oak_0.json
+-rw-rw-rw-   0        0        0      121 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/oak_1.json
+-rw-rw-rw-   0        0        0      121 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/oak_2.json
+-rw-rw-rw-   0        0        0      121 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/oak_3.json
+-rw-rw-rw-   0        0        0     1184 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_0.json
+-rw-rw-rw-   0        0        0     1173 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_1.json
+-rw-rw-rw-   0        0        0     1167 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_2.json
+-rw-rw-rw-   0        0        0     1171 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_3.json
+-rw-rw-rw-   0        0        0      127 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/spruce_0.json
+-rw-rw-rw-   0        0        0      127 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/spruce_1.json
+-rw-rw-rw-   0        0        0      127 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/spruce_2.json
+-rw-rw-rw-   0        0        0      127 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/spruce_3.json
+-rw-rw-rw-   0        0        0      127 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/warped_0.json
+-rw-rw-rw-   0        0        0      127 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/warped_1.json
+-rw-rw-rw-   0        0        0      127 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/warped_2.json
+-rw-rw-rw-   0        0        0      127 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/warped_3.json
+-rw-rw-rw-   0        0        0      147 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/structure_void.json
+-rw-rw-rw-   0        0        0      106 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/trapped_chest.json
+-rw-rw-rw-   0        0        0      116 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/trapped_chest_left.json
+-rw-rw-rw-   0        0        0      118 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/trapped_chest_right.json
+drwxrwxrwx   0        0        0        0 2023-07-04 08:40:04.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/
+-rw-rw-rw-   0        0        0       98 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/black.json
+-rw-rw-rw-   0        0        0       97 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/blue.json
+-rw-rw-rw-   0        0        0       98 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/brown.json
+-rw-rw-rw-   0        0        0       97 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/cyan.json
+-rw-rw-rw-   0        0        0       97 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/gray.json
+-rw-rw-rw-   0        0        0       98 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/green.json
+-rw-rw-rw-   0        0        0      103 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/light_blue.json
+-rw-rw-rw-   0        0        0      103 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/light_gray.json
+-rw-rw-rw-   0        0        0       97 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/lime.json
+-rw-rw-rw-   0        0        0      100 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/magenta.json
+-rw-rw-rw-   0        0        0       99 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/orange.json
+-rw-rw-rw-   0        0        0       97 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/pink.json
+-rw-rw-rw-   0        0        0       99 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/purple.json
+-rw-rw-rw-   0        0        0       96 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/red.json
+-rw-rw-rw-   0        0        0       98 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/white.json
+-rw-rw-rw-   0        0        0       99 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/yellow.json
+-rw-rw-rw-   0        0        0     1208 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner.json
+drwxrwxrwx   0        0        0        0 2023-07-04 08:40:04.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/
+-rw-rw-rw-   0        0        0      135 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/acacia.json
+-rw-rw-rw-   0        0        0      133 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/birch.json
+-rw-rw-rw-   0        0        0      137 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/crimson.json
+-rw-rw-rw-   0        0        0      139 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/dark_oak.json
+-rw-rw-rw-   0        0        0      135 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/jungle.json
+-rw-rw-rw-   0        0        0      139 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/mangrove.json
+-rw-rw-rw-   0        0        0      129 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/oak.json
+-rw-rw-rw-   0        0        0      135 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/spruce.json
+-rw-rw-rw-   0        0        0      588 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/wall_sign.json
+-rw-rw-rw-   0        0        0      135 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/warped.json
+-rw-rw-rw-   0        0        0      135 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/water.json
+-rw-rw-rw-   0        0        0      153 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/white_shulker_box.json
+-rw-rw-rw-   0        0        0      155 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/yellow_shulker_box.json
+drwxrwxrwx   0        0        0        0 2023-07-04 08:40:01.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/
+drwxrwxrwx   0        0        0        0 2023-07-04 08:40:04.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/
+drwxrwxrwx   0        0        0        0 2023-07-04 08:40:04.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/
+-rw-rw-rw-   0        0        0     2769 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_black.png
+-rw-rw-rw-   0        0        0     3786 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_blue.png
+-rw-rw-rw-   0        0        0     3707 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_brown.png
+-rw-rw-rw-   0        0        0     3813 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_cyan.png
+-rw-rw-rw-   0        0        0     3518 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_gray.png
+-rw-rw-rw-   0        0        0     3751 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_green.png
+-rw-rw-rw-   0        0        0     4220 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_light_blue.png
+-rw-rw-rw-   0        0        0     3953 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_light_gray.png
+-rw-rw-rw-   0        0        0     4151 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_lime.png
+-rw-rw-rw-   0        0        0     4178 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_magenta.png
+-rw-rw-rw-   0        0        0     4298 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_orange.png
+-rw-rw-rw-   0        0        0     4205 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_pink.png
+-rw-rw-rw-   0        0        0     4056 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_purple.png
+-rw-rw-rw-   0        0        0     3790 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_red.png
+-rw-rw-rw-   0        0        0     3985 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_white.png
+-rw-rw-rw-   0        0        0     4457 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_yellow.png
+-rw-rw-rw-   0        0        0      651 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/barrier.png
+-rw-rw-rw-   0        0        0     1265 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/end_portal.png
+-rw-rw-rw-   0        0        0     1286 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/lava.png
+-rw-rw-rw-   0        0        0     1405 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/structure_void.png
+-rw-rw-rw-   0        0        0      927 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/water.png
+-rw-rw-rw-   0        0        0    22749 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/pack.png
+-rw-rw-rw-   0        0        0     1687 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/resource_pack.py
+-rw-rw-rw-   0        0        0    22308 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/resource_pack_manager.py
+-rw-rw-rw-   0        0        0      299 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/unknown_resource_pack.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:40:04.000000 minecraft-resource-pack-1.3.4/minecraft_resource_pack.egg-info/
+-rw-rw-rw-   0        0        0      487 2023-07-04 08:40:01.000000 minecraft-resource-pack-1.3.4/minecraft_resource_pack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    48090 2023-07-04 08:40:01.000000 minecraft-resource-pack-1.3.4/minecraft_resource_pack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 08:40:01.000000 minecraft-resource-pack-1.3.4/minecraft_resource_pack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-07-04 08:40:01.000000 minecraft-resource-pack-1.3.4/minecraft_resource_pack.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-07-04 08:40:00.000000 minecraft-resource-pack-1.3.4/minecraft_resource_pack.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      174 2023-07-04 08:40:01.000000 minecraft-resource-pack-1.3.4/minecraft_resource_pack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-07-04 08:40:01.000000 minecraft-resource-pack-1.3.4/minecraft_resource_pack.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      135 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/pyproject.toml
+-rw-rw-rw-   0        0        0     1187 2023-07-04 08:40:04.000000 minecraft-resource-pack-1.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      142 2023-07-04 08:39:10.000000 minecraft-resource-pack-1.3.4/setup.py
```

### Comparing `minecraft-resource-pack-1.3.3/LICENSE` & `minecraft-resource-pack-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/_version.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/_version.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
 {
- "date": "2022-10-27T10:18:50+0100",
+ "date": "2023-07-02T15:46:08+0100",
  "dirty": false,
  "error": null,
- "full-revisionid": "b09b9e98435d64c3c8015aacf1350c4a1440706e",
- "version": "1.3.3"
+ "full-revisionid": "3a0a6c59446d06d4fd7d2e3ce716fe3258a50c39",
+ "version": "1.3.4"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/amulet/block.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/amulet/block.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/comment_json.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/comment_json.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/image/missing_pack_java.png` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/image/missing_pack_java.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/mesh/block/block_mesh.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/mesh/block/block_mesh.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/mesh/block/cube.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/mesh/block/cube.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/mesh/block/missing_block.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/mesh/block/missing_block.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/__init__.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/__init__.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/base/resource_pack.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/base/resource_pack.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/base/resource_pack_manager.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/base/resource_pack_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,24 +24,19 @@
 
     def _unload(self):
         """Clear all loaded resources."""
         self._texture_is_transparent.clear()
         self._cached_models.clear()
 
     def _load_transparency_cache(self, path: str):
-        if os.path.isfile(
-            os.path.join(os.path.dirname(path), "transparency_cache.json")
-        ):
-            try:
-                with open(
-                    os.path.join(os.path.dirname(path), "transparency_cache.json")
-                ) as f:
-                    self._texture_is_transparent = json.load(f)
-            except:
-                pass
+        try:
+            with open(path) as f:
+                self._texture_is_transparent = json.load(f)
+        except:
+            pass
 
     def _load_iter(self) -> Generator[float, None, None]:
         """Load resources."""
         raise NotImplementedError
 
     def reload(self) -> Generator[float, None, None]:
         """Unload and reload resources"""
```

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/block_palette.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/block_palette.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/__init__.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/__init__.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/air.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/air.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/base_blockshape.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/base_blockshape.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/bubble_column.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/bubble_column.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cake.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cake.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/chest.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/chest.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/comparator.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/comparator.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cross_texture.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cross_texture.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cube.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cube.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/default.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/default.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/double_plant.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/double_plant.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/enchanting_table.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/enchanting_table.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/farmland.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/farmland.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/fence.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/fence.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/flat.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/flat.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/flat_wall.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/flat_wall.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/furnace.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/furnace.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/green_cube.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/green_cube.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/ladder.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/ladder.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/partial_block.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/partial_block.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/piston.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/piston.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/piston_arm.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/piston_arm.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/portal_frame.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/portal_frame.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pressure_plate.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pressure_plate.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pumpkin.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pumpkin.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/repeater.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/repeater.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/slab.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/slab.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/tree.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/tree.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/vine.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/vine.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/wall.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/wall.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/water.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/water.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/blockshapes.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/blockshapes.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/download_resources.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/download_resources.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 import os
-import shutil
-import zipfile
-import json
-from urllib.request import urlopen
-import io
-from typing import Generator
+
+# import shutil
+# import zipfile
+# import json
+# from urllib.request import urlopen
+# import io
+from typing import Generator, Optional
 import logging
 
-import minecraft_model_reader
 from minecraft_model_reader.api.resource_pack import BedrockResourcePack
 
-RESOURCE_PACK_DIR = os.path.join(
-    minecraft_model_reader.path, "api", "resource_pack", "bedrock", "resource_packs"
-)
-
 log = logging.getLogger(__name__)
 
 
 def generator_unpacker(gen: Generator):
     try:
         while True:
             next(gen)
@@ -26,15 +22,17 @@
 
 
 def get_latest() -> BedrockResourcePack:
     return generator_unpacker(get_latest_iter())
 
 
 def get_latest_iter() -> Generator[float, None, BedrockResourcePack]:
-    vanilla_rp_path = os.path.join(RESOURCE_PACK_DIR, "bedrock_vanilla")
+    vanilla_rp_path = os.path.join(
+        os.environ["CACHE_DIR"], "resource_packs", "bedrock", "vanilla"
+    )
     yield 0
     # new_version = launcher_manifest["latest"]["release"]
     # if new_version is None:
     #     if os.path.isdir(vanilla_rp_path):
     #         log.error(
     #             "Could not download the launcher manifest. The resource pack seems to be present so using that."
     #         )
@@ -52,23 +50,23 @@
     #         else:
     #             yield from _remove_and_download_iter(vanilla_rp_path, new_version)
     #     else:
     #         yield from _remove_and_download_iter(vanilla_rp_path, new_version)
     return BedrockResourcePack(vanilla_rp_path)
 
 
-_bedrock_vanilla_fix = None
-_bedrock_vanilla_latest = None
+_bedrock_vanilla_fix: Optional[BedrockResourcePack] = None
+_bedrock_vanilla_latest: Optional[BedrockResourcePack] = None
 
 
-def get_bedrock_vanilla_fix():
+def get_bedrock_vanilla_fix() -> BedrockResourcePack:
     global _bedrock_vanilla_fix
     if _bedrock_vanilla_fix is None:
         _bedrock_vanilla_fix = BedrockResourcePack(
-            os.path.join(RESOURCE_PACK_DIR, "bedrock_vanilla_fix")
+            os.path.join(os.path.dirname(__file__), "bedrock_vanilla_fix")
         )
     return _bedrock_vanilla_fix
 
 
 def get_bedrock_vanilla_latest():
     global _bedrock_vanilla_latest
     if _bedrock_vanilla_latest is None:
```

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/resource_pack.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/resource_pack.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/resource_pack_manager.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/resource_pack_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,20 +7,23 @@
 from minecraft_model_reader.api import Block, comment_json
 from minecraft_model_reader.api.resource_pack import BaseResourcePackManager
 from minecraft_model_reader.api.resource_pack.bedrock import BedrockResourcePack
 from minecraft_model_reader.api.mesh.block.block_mesh import BlockMesh
 from .blockshapes import BlockShapeClasses
 
 
-def _load_data() -> Tuple[
-    Dict[str, str],
-    Dict[
-        str, Tuple[Tuple[Tuple[str, str], ...], Dict[Tuple[Union[str, int], ...], int]]
-    ],
-]:
+def _load_data() -> (
+    Tuple[
+        Dict[str, str],
+        Dict[
+            str,
+            Tuple[Tuple[Tuple[str, str], ...], Dict[Tuple[Union[str, int], ...], int]],
+        ],
+    ]
+):
     with open(os.path.join(os.path.dirname(__file__), "blockshapes.json")) as f:
         _block_shapes = comment_json.load(f)
 
     _aux_values = {}
     with open(os.path.join(os.path.dirname(__file__), "block_palette.json")) as f:
         _block_palette = comment_json.load(f)
     for block in _block_palette["blocks"]:
@@ -122,15 +125,22 @@
                 os.stat(texture_path)[8],
                 bool(texture_is_transparent),
             )
         return texture_path
 
     def _load_iter(self) -> Generator[float, None, None]:
         self._block_shapes.update(BlockShapes)  # add the default block shapes
-        self._load_transparency_cache(__file__)
+
+        transparency_cache_path = os.path.join(
+            os.environ["CACHE_DIR"],
+            "resource_packs",
+            "bedrock",
+            "transparency_cache.json",
+        )
+        self._load_transparency_cache(transparency_cache_path)
 
         self._textures["missing_no"] = self._check_texture("missing")
 
         pack_count = len(self._packs)
 
         for pack_index, pack in enumerate(self._packs):
             pack_progress = pack_index / pack_count
@@ -212,17 +222,16 @@
                                         block_id = "minecraft:" + block_id
                                     self._blocks[block_id] = data.get("textures")
                                 yield sub_progress + (model_index) / (
                                     model_count * pack_count * 2
                                 )
             yield pack_progress + 1
 
-        with open(
-            os.path.join(os.path.dirname(__file__), "transparency_cache.json"), "w"
-        ) as f:
+        os.makedirs(os.path.dirname(transparency_cache_path), exist_ok=True)
+        with open(transparency_cache_path, "w") as f:
             json.dump(self._texture_is_transparent, f)
 
     @property
     def textures(self) -> Tuple[str, ...]:
         """Returns a tuple of all the texture paths in the resource pack."""
         return tuple(self._textures.values())
```

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/resource_packs/bedrock_vanilla_fix/blocks.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/blocks.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/resource_packs/bedrock_vanilla_fix/manifest.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/manifest.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/resource_packs/bedrock_vanilla_fix/pack_icon.png` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/pack_icon.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/resource_packs/bedrock_vanilla_fix/textures/blocks/grass_carried.png` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/blocks/grass_carried.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/bedrock/resource_packs/bedrock_vanilla_fix/textures/blocks/water.png` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/blocks/water.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/download_resources.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/download_resources.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,22 +3,18 @@
 import zipfile
 import json
 from urllib.request import urlopen
 import io
 from typing import Generator, List
 import logging
 
-import minecraft_model_reader
 from minecraft_model_reader.api.resource_pack import JavaResourcePack
 
 log = logging.getLogger(__name__)
 
-RESOURCE_PACK_DIR = os.path.join(
-    minecraft_model_reader.path, "api", "resource_pack", "java", "resource_packs"
-)
 launcher_manifest = None
 INCLUDE_SNAPSHOT = False
 
 
 def get_launcher_manifest() -> dict:
     global launcher_manifest
     if launcher_manifest is None:
@@ -46,15 +42,17 @@
 def get_latest_iter() -> Generator[float, None, JavaResourcePack]:
     """Download the latest resource pack if required.
 
     :return: The loaded Java resource pack.
     :raises:
         Exception: If the
     """
-    vanilla_rp_path = os.path.join(RESOURCE_PACK_DIR, "java_vanilla")
+    vanilla_rp_path = os.path.join(
+        os.environ["CACHE_DIR"], "resource_packs", "java", "vanilla"
+    )
     try:
         if INCLUDE_SNAPSHOT:
             new_version = get_launcher_manifest()["latest"]["snapshot"]
         else:
             new_version = get_launcher_manifest()["latest"]["release"]
     except Exception as e:
         if os.path.isdir(vanilla_rp_path):
@@ -79,15 +77,15 @@
 _java_vanilla_latest = None
 
 
 def get_java_vanilla_fix():
     global _java_vanilla_fix
     if _java_vanilla_fix is None:
         _java_vanilla_fix = JavaResourcePack(
-            os.path.join(RESOURCE_PACK_DIR, "java_vanilla_fix")
+            os.path.join(os.path.dirname(__file__), "java_vanilla_fix")
         )
     return _java_vanilla_fix
 
 
 def get_java_vanilla_latest():
     global _java_vanilla_latest
     if _java_vanilla_latest is None:
```

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_pack.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/resource_pack.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_pack_manager.py` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/resource_pack_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,19 @@
         self._textures.clear()
         self._texture_is_transparent.clear()
         self._model_files.clear()
 
     def _load_iter(self) -> Generator[float, None, None]:
         blockstate_file_paths: Dict[Tuple[str, str], str] = {}
         model_file_paths: Dict[Tuple[str, str], str] = {}
-        self._load_transparency_cache(__file__)
+
+        transparency_cache_path = os.path.join(
+            os.environ["CACHE_DIR"], "resource_packs", "java", "transparency_cache.json"
+        )
+        self._load_transparency_cache(transparency_cache_path)
 
         self._textures[("minecraft", "missing_no")] = self.missing_no
 
         pack_count = len(self._packs)
 
         for pack_index, pack in enumerate(self._packs):
             # pack_format=2 textures/blocks, textures/items - case sensitive
@@ -167,17 +171,16 @@
                     ).split(os.sep)
                     rel_path = "/".join(rel_path_list)[:-5]
                     model_file_paths[
                         (namespace, rel_path.replace(os.sep, "/"))
                     ] = model_path
                     yield sub_progress + (model_index) / (model_count * pack_count * 3)
 
-        with open(
-            os.path.join(os.path.dirname(__file__), "transparency_cache.json"), "w"
-        ) as f:
+        os.makedirs(os.path.dirname(transparency_cache_path), exist_ok=True)
+        with open(transparency_cache_path, "w") as f:
             json.dump(self._texture_is_transparent, f)
 
         for key, path in blockstate_file_paths.items():
             with open(path) as fi:
                 try:
                     self._blockstate_files[key] = json.load(fi)
                 except json.JSONDecodeError:
```

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/acacia_sign.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/acacia_sign.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/birch_sign.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/birch_sign.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/black_banner.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/black_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/black_bed.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/black_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/blue_banner.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/blue_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/blue_bed.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/blue_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/brown_banner.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/brown_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/brown_bed.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/brown_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/chest.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/chest.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/creeper_head.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/creeper_head.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/crimson_sign.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/crimson_sign.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/cyan_banner.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/cyan_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/cyan_bed.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/cyan_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/dark_oak_sign.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/dark_oak_sign.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/dragon_head.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/dragon_head.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/gray_banner.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/gray_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/gray_bed.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/gray_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/green_banner.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/green_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/green_bed.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/green_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/jungle_sign.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/jungle_sign.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/light.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/light_blue_banner.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_blue_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/light_blue_bed.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_blue_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/light_gray_banner.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_gray_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/light_gray_bed.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_gray_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/lime_banner.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/lime_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/lime_bed.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/lime_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/magenta_banner.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/magenta_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/magenta_bed.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/magenta_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/mangrove_sign.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/mangrove_sign.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/oak_sign.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/oak_sign.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/orange_banner.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/orange_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/orange_bed.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/orange_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/pink_banner.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/pink_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/pink_bed.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/pink_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/player_head.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/player_head.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/purple_banner.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/purple_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/purple_bed.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/purple_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/red_banner.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/red_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/red_bed.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/red_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/skeleton_skull.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/skeleton_skull.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/spruce_sign.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/spruce_sign.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/trapped_chest.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/trapped_chest.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/warped_sign.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/warped_sign.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/white_banner.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/white_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/white_bed.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/white_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/wither_skeleton_skull.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/wither_skeleton_skull.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/yellow_banner.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/yellow_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/yellow_bed.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/yellow_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/blockstates/zombie_head.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/zombie_head.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/banner_0.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_0.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/banner_1.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_1.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/banner_2.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_2.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/banner/banner_3.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_3.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bed_foot.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed_foot.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bed_head.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed_head.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bell_between_walls.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_between_walls.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bell_ceiling.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_ceiling.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bell_floor.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_floor.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/bell_wall.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_wall.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/chest_base.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_base.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/chest_left_base.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_left_base.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/chest_right_base.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_right_base.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/conduit.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/conduit.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_0.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_0.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_1.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_1.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_2.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_2.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_3.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_3.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_0.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_0.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_1.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_1.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_2.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_2.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_3.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_3.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_0.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_0.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_1.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_1.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_2.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_2.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_3.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_3.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/wall/dragon.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/dragon.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/wall/head.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/head.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/head/wall/head2.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/head2.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/sign_0.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_0.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/sign_1.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_1.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/sign_2.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_2.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/sign/sign_3.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_3.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/wall_banner.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/models/block/wall_sign/wall_sign.json` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/wall_sign.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_black.png` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_black.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_blue.png` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_blue.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_brown.png` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_brown.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_cyan.png` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_cyan.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_gray.png` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_gray.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_green.png` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_green.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_light_blue.png` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_light_blue.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_light_gray.png` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_light_gray.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_lime.png` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_lime.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_magenta.png` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_magenta.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_orange.png` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_orange.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_pink.png` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_pink.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_purple.png` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_purple.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_red.png` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_red.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_white.png` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_white.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_yellow.png` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_yellow.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/barrier.png` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/barrier.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/end_portal.png` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/end_portal.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/lava.png` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/lava.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/structure_void.png` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/structure_void.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/assets/minecraft/textures/block/water.png` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/water.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/minecraft_model_reader/api/resource_pack/java/resource_packs/java_vanilla_fix/pack.png` & `minecraft-resource-pack-1.3.4/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/pack.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.3.3/setup.cfg` & `minecraft-resource-pack-1.3.4/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -30,44 +30,46 @@
 000001d0: 7564 655f 7061 636b 6167 655f 6461 7461  ude_package_data
 000001e0: 203d 2054 7275 650d 0a70 7974 686f 6e5f   = True..python_
 000001f0: 7265 7175 6972 6573 203d 207e 3d33 2e36  requires = ~=3.6
 00000200: 0d0a 696e 7374 616c 6c5f 7265 7175 6972  ..install_requir
 00000210: 6573 203d 200d 0a09 5069 6c6c 6f77 3e3d  es = ...Pillow>=
 00000220: 372e 310d 0a09 6e75 6d70 793e 3d31 2e31  7.1...numpy>=1.1
 00000230: 370d 0a09 616d 756c 6574 2d6e 6274 7e3d  7...amulet-nbt~=
-00000240: 322e 300d 0a0d 0a5b 6f70 7469 6f6e 732e  2.0....[options.
-00000250: 7061 636b 6167 6573 2e66 696e 645d 0d0a  packages.find]..
-00000260: 696e 636c 7564 6520 3d20 6d69 6e65 6372  include = minecr
-00000270: 6166 745f 6d6f 6465 6c5f 7265 6164 6572  aft_model_reader
-00000280: 2a0d 0a0d 0a5b 6f70 7469 6f6e 732e 6578  *....[options.ex
-00000290: 7472 6173 5f72 6571 7569 7265 5d0d 0a64  tras_require]..d
-000002a0: 6f63 7320 3d20 0d0a 0953 7068 696e 783e  ocs = ...Sphinx>
-000002b0: 3d31 2e37 2e34 0d0a 0973 7068 696e 782d  =1.7.4...sphinx-
-000002c0: 6175 746f 646f 632d 7479 7065 6869 6e74  autodoc-typehint
-000002d0: 733e 3d31 2e33 2e30 0d0a 0973 7068 696e  s>=1.3.0...sphin
-000002e0: 785f 7274 645f 7468 656d 653e 3d30 2e33  x_rtd_theme>=0.3
-000002f0: 2e31 0d0a 6465 7620 3d20 0d0a 0962 6c61  .1..dev = ...bla
-00000300: 636b 3e3d 3232 2e33 0d0a 0970 7265 5f63  ck>=22.3...pre_c
-00000310: 6f6d 6d69 743e 3d31 2e31 312e 310d 0a0d  ommit>=1.11.1...
-00000320: 0a5b 6f70 7469 6f6e 732e 656e 7472 795f  .[options.entry_
-00000330: 706f 696e 7473 5d0d 0a70 7969 6e73 7461  points]..pyinsta
-00000340: 6c6c 6572 3430 203d 200d 0a09 686f 6f6b  ller40 = ...hook
-00000350: 2d64 6972 7320 3d20 6d69 6e65 6372 6166  -dirs = minecraf
-00000360: 745f 6d6f 6465 6c5f 7265 6164 6572 2e5f  t_model_reader._
-00000370: 5f70 7969 6e73 7461 6c6c 6572 3a67 6574  _pyinstaller:get
-00000380: 5f68 6f6f 6b5f 6469 7273 0d0a 0d0a 5b76  _hook_dirs....[v
-00000390: 6572 7369 6f6e 6565 725d 0d0a 5643 5320  ersioneer]..VCS 
-000003a0: 3d20 6769 740d 0a73 7479 6c65 203d 2070  = git..style = p
-000003b0: 6570 3434 300d 0a76 6572 7369 6f6e 6669  ep440..versionfi
-000003c0: 6c65 5f73 6f75 7263 6520 3d20 6d69 6e65  le_source = mine
-000003d0: 6372 6166 745f 6d6f 6465 6c5f 7265 6164  craft_model_read
-000003e0: 6572 2f5f 7665 7273 696f 6e2e 7079 0d0a  er/_version.py..
-000003f0: 7665 7273 696f 6e66 696c 655f 6275 696c  versionfile_buil
-00000400: 6420 3d20 6d69 6e65 6372 6166 745f 6d6f  d = minecraft_mo
-00000410: 6465 6c5f 7265 6164 6572 2f5f 7665 7273  del_reader/_vers
-00000420: 696f 6e2e 7079 0d0a 7461 675f 7072 6566  ion.py..tag_pref
-00000430: 6978 203d 200d 0a70 6172 656e 7464 6972  ix = ..parentdir
-00000440: 5f70 7265 6669 7820 3d20 6d69 6e65 6372  _prefix = minecr
-00000450: 6166 745f 6d6f 6465 6c5f 7265 6164 6572  aft_model_reader
-00000460: 2d0d 0a0d 0a5b 6567 675f 696e 666f 5d0d  -....[egg_info].
-00000470: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
-00000480: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
+00000240: 322e 300d 0a09 706c 6174 666f 726d 6469  2.0...platformdi
+00000250: 7273 7e3d 332e 310d 0a0d 0a5b 6f70 7469  rs~=3.1....[opti
+00000260: 6f6e 732e 7061 636b 6167 6573 2e66 696e  ons.packages.fin
+00000270: 645d 0d0a 696e 636c 7564 6520 3d20 6d69  d]..include = mi
+00000280: 6e65 6372 6166 745f 6d6f 6465 6c5f 7265  necraft_model_re
+00000290: 6164 6572 2a0d 0a0d 0a5b 6f70 7469 6f6e  ader*....[option
+000002a0: 732e 6578 7472 6173 5f72 6571 7569 7265  s.extras_require
+000002b0: 5d0d 0a64 6f63 7320 3d20 0d0a 0953 7068  ]..docs = ...Sph
+000002c0: 696e 783e 3d31 2e37 2e34 0d0a 0973 7068  inx>=1.7.4...sph
+000002d0: 696e 782d 6175 746f 646f 632d 7479 7065  inx-autodoc-type
+000002e0: 6869 6e74 733e 3d31 2e33 2e30 0d0a 0973  hints>=1.3.0...s
+000002f0: 7068 696e 785f 7274 645f 7468 656d 653e  phinx_rtd_theme>
+00000300: 3d30 2e33 2e31 0d0a 6465 7620 3d20 0d0a  =0.3.1..dev = ..
+00000310: 0962 6c61 636b 3e3d 3232 2e33 0d0a 0970  .black>=22.3...p
+00000320: 7265 5f63 6f6d 6d69 743e 3d31 2e31 312e  re_commit>=1.11.
+00000330: 310d 0a0d 0a5b 6f70 7469 6f6e 732e 656e  1....[options.en
+00000340: 7472 795f 706f 696e 7473 5d0d 0a70 7969  try_points]..pyi
+00000350: 6e73 7461 6c6c 6572 3430 203d 200d 0a09  nstaller40 = ...
+00000360: 686f 6f6b 2d64 6972 7320 3d20 6d69 6e65  hook-dirs = mine
+00000370: 6372 6166 745f 6d6f 6465 6c5f 7265 6164  craft_model_read
+00000380: 6572 2e5f 5f70 7969 6e73 7461 6c6c 6572  er.__pyinstaller
+00000390: 3a67 6574 5f68 6f6f 6b5f 6469 7273 0d0a  :get_hook_dirs..
+000003a0: 0d0a 5b76 6572 7369 6f6e 6565 725d 0d0a  ..[versioneer]..
+000003b0: 5643 5320 3d20 6769 740d 0a73 7479 6c65  VCS = git..style
+000003c0: 203d 2070 6570 3434 300d 0a76 6572 7369   = pep440..versi
+000003d0: 6f6e 6669 6c65 5f73 6f75 7263 6520 3d20  onfile_source = 
+000003e0: 6d69 6e65 6372 6166 745f 6d6f 6465 6c5f  minecraft_model_
+000003f0: 7265 6164 6572 2f5f 7665 7273 696f 6e2e  reader/_version.
+00000400: 7079 0d0a 7665 7273 696f 6e66 696c 655f  py..versionfile_
+00000410: 6275 696c 6420 3d20 6d69 6e65 6372 6166  build = minecraf
+00000420: 745f 6d6f 6465 6c5f 7265 6164 6572 2f5f  t_model_reader/_
+00000430: 7665 7273 696f 6e2e 7079 0d0a 7461 675f  version.py..tag_
+00000440: 7072 6566 6978 203d 200d 0a70 6172 656e  prefix = ..paren
+00000450: 7464 6972 5f70 7265 6669 7820 3d20 6d69  tdir_prefix = mi
+00000460: 6e65 6372 6166 745f 6d6f 6465 6c5f 7265  necraft_model_re
+00000470: 6164 6572 2d0d 0a0d 0a5b 6567 675f 696e  ader-....[egg_in
+00000480: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
+00000490: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
+000004a0: 0a0d 0a                                  ...
```

