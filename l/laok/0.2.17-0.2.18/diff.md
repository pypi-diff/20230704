# Comparing `tmp/laok-0.2.17.tar.gz` & `tmp/laok-0.2.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laok-0.2.17.tar", last modified: Fri May  5 09:26:37 2023, max compression
+gzip compressed data, was "laok-0.2.18.tar", last modified: Tue Jul  4 02:41:42 2023, max compression
```

## Comparing `laok-0.2.17.tar` & `laok-0.2.18.tar`

### file list

```diff
@@ -1,176 +1,200 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.359424 laok-0.2.17/
--rw-rw-rw-   0        0        0      217 2023-05-05 09:26:37.358426 laok-0.2.17/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.261685 laok-0.2.17/laok/
--rw-rw-rw-   0        0        0       21 2023-04-23 12:49:06.000000 laok-0.2.17/laok/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.269662 laok-0.2.17/laok/base/
--rw-rw-rw-   0        0        0      252 2023-05-04 14:39:27.000000 laok-0.2.17/laok/base/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.270661 laok-0.2.17/laok/base/alg/
--rw-rw-rw-   0        0        0       26 2023-04-20 13:21:17.000000 laok-0.2.17/laok/base/alg/__init__.py
--rw-rw-rw-   0        0        0     4923 2023-04-20 13:20:53.000000 laok-0.2.17/laok/base/alg/addict.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.272653 laok-0.2.17/laok/base/conf/
--rw-rw-rw-   0        0        0        0 2023-04-19 14:38:53.000000 laok-0.2.17/laok/base/conf/__init__.py
--rw-rw-rw-   0        0        0      360 2023-04-19 14:40:47.000000 laok-0.2.17/laok/base/conf/conf_global.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.275646 laok-0.2.17/laok/base/dataset/
--rw-rw-rw-   0        0        0        0 2023-04-21 04:27:16.000000 laok-0.2.17/laok/base/dataset/__init__.py
--rw-rw-rw-   0        0        0     6406 2023-04-21 04:29:54.000000 laok-0.2.17/laok/base/dataset/cvt_voc_yolo.py
--rw-rw-rw-   0        0        0     2405 2019-09-12 10:55:17.000000 laok-0.2.17/laok/base/dataset/darknet-voc2yolo.py
--rw-rw-rw-   0        0        0     2241 2019-02-18 15:12:05.000000 laok-0.2.17/laok/base/dataset/voc_label.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.277643 laok-0.2.17/laok/base/dtime/
--rw-rw-rw-   0        0        0       47 2022-10-21 10:13:37.000000 laok-0.2.17/laok/base/dtime/__init__.py
--rw-rw-rw-   0        0        0      556 2022-11-17 01:18:56.000000 laok-0.2.17/laok/base/dtime/datetime_.py
--rw-rw-rw-   0        0        0     2727 2023-04-19 11:27:09.000000 laok-0.2.17/laok/base/dtime/timer.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.283626 laok-0.2.17/laok/base/fs/
--rw-rw-rw-   0        0        0      134 2023-05-04 11:06:57.000000 laok-0.2.17/laok/base/fs/__init__.py
--rw-rw-rw-   0        0        0     1740 2023-04-19 09:22:34.000000 laok-0.2.17/laok/base/fs/fdata.py
--rw-rw-rw-   0        0        0     2937 2022-11-03 16:22:33.000000 laok-0.2.17/laok/base/fs/fname.py
--rw-rw-rw-   0        0        0     4393 2023-05-04 14:09:33.000000 laok-0.2.17/laok/base/fs/fpath.py
--rw-rw-rw-   0        0        0     1785 2023-05-04 11:06:06.000000 laok-0.2.17/laok/base/fs/fsearch.py
--rw-rw-rw-   0        0        0     2819 2023-05-05 03:57:37.000000 laok-0.2.17/laok/base/fs/fwalk.py
--rw-rw-rw-   0        0        0     1413 2023-04-19 09:23:34.000000 laok-0.2.17/laok/base/fs/name_index.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.284624 laok-0.2.17/laok/base/func/
--rw-rw-rw-   0        0        0        0 2023-04-19 08:09:16.000000 laok-0.2.17/laok/base/func/__init__.py
--rw-rw-rw-   0        0        0     1871 2022-10-21 10:13:37.000000 laok-0.2.17/laok/base/func/print_info.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.286619 laok-0.2.17/laok/base/log/
--rw-rw-rw-   0        0        0       50 2023-04-19 14:41:08.000000 laok-0.2.17/laok/base/log/__init__.py
--rw-rw-rw-   0        0        0     2185 2023-04-19 14:41:16.000000 laok-0.2.17/laok/base/log/log.py
--rw-rw-rw-   0        0        0      672 2023-04-19 14:43:17.000000 laok-0.2.17/laok/base/log/log_default.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.289610 laok-0.2.17/laok/base/net/
--rw-rw-rw-   0        0        0       45 2023-05-04 14:42:06.000000 laok-0.2.17/laok/base/net/__init__.py
--rw-rw-rw-   0        0        0      691 2022-09-23 00:45:15.000000 laok-0.2.17/laok/base/net/ip.py
--rw-rw-rw-   0        0        0     2654 2023-04-20 15:19:59.000000 laok-0.2.17/laok/base/net/requests_.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.290607 laok-0.2.17/laok/base/parallel/
--rw-rw-rw-   0        0        0       20 2022-10-21 10:13:37.000000 laok-0.2.17/laok/base/parallel/__init__.py
--rw-rw-rw-   0        0        0     2010 2023-04-20 15:21:46.000000 laok-0.2.17/laok/base/parallel/pool.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.295594 laok-0.2.17/laok/base/ser/
--rw-rw-rw-   0        0        0      136 2023-04-25 06:35:56.000000 laok-0.2.17/laok/base/ser/__init__.py
--rw-rw-rw-   0        0        0     1367 2023-04-25 06:50:06.000000 laok-0.2.17/laok/base/ser/_json.py
--rw-rw-rw-   0        0        0      750 2023-04-20 13:46:22.000000 laok-0.2.17/laok/base/ser/_marshal.py
--rw-rw-rw-   0        0        0      621 2023-04-25 06:50:29.000000 laok-0.2.17/laok/base/ser/_pickle.py
--rw-rw-rw-   0        0        0      719 2023-04-25 06:50:29.000000 laok-0.2.17/laok/base/ser/numpy_.py
--rw-rw-rw-   0        0        0      778 2023-04-25 06:50:29.000000 laok-0.2.17/laok/base/ser/torch_.py
--rw-rw-rw-   0        0        0     1361 2023-04-25 06:50:39.000000 laok-0.2.17/laok/base/ser/yaml_.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.298587 laok-0.2.17/laok/base/str/
--rw-rw-rw-   0        0        0       65 2023-04-21 09:32:10.000000 laok-0.2.17/laok/base/str/__init__.py
--rw-rw-rw-   0        0        0      429 2023-04-21 09:32:29.000000 laok-0.2.17/laok/base/str/fmt.py
--rw-rw-rw-   0        0        0     1924 2023-04-19 08:08:18.000000 laok-0.2.17/laok/base/str/misc.py
--rw-rw-rw-   0        0        0     2599 2023-04-21 09:30:50.000000 laok-0.2.17/laok/base/str/print_info.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.300581 laok-0.2.17/laok/base/sys_/
--rw-rw-rw-   0        0        0       26 2023-05-04 15:23:17.000000 laok-0.2.17/laok/base/sys_/__init__.py
--rw-rw-rw-   0        0        0      518 2023-05-04 15:23:10.000000 laok-0.2.17/laok/base/sys_/platform_.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.302576 laok-0.2.17/laok/base/test/
--rw-rw-rw-   0        0        0       43 2022-10-21 10:13:37.000000 laok-0.2.17/laok/base/test/__init__.py
--rw-rw-rw-   0        0        0     8032 2023-04-19 15:30:44.000000 laok-0.2.17/laok/base/test/_dump.py
--rw-rw-rw-   0        0        0     4551 2023-03-03 02:51:53.000000 laok-0.2.17/laok/base/test/_run.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.303573 laok-0.2.17/laok/cv2d/
--rw-rw-rw-   0        0        0       22 2023-04-21 08:27:09.000000 laok-0.2.17/laok/cv2d/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.304573 laok-0.2.17/laok/cv3d/
--rw-rw-rw-   0        0        0       64 2023-04-21 09:21:19.000000 laok-0.2.17/laok/cv3d/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.305568 laok-0.2.17/laok/cv3d/io/
--rw-rw-rw-   0        0        0       24 2023-04-21 09:18:03.000000 laok-0.2.17/laok/cv3d/io/__init__.py
--rw-rw-rw-   0        0        0      832 2023-04-25 06:52:21.000000 laok-0.2.17/laok/cv3d/io/_simple.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.306565 laok-0.2.17/laok/cv3d/show/
--rw-rw-rw-   0        0        0       21 2023-04-21 09:20:03.000000 laok-0.2.17/laok/cv3d/show/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.307563 laok-0.2.17/laok/cv3d/show/vtk_/
--rw-rw-rw-   0        0        0      804 2023-04-21 09:21:01.000000 laok-0.2.17/laok/cv3d/show/vtk_/__init__.py
--rw-rw-rw-   0        0        0     3916 2022-10-21 10:13:38.000000 laok-0.2.17/laok/cv3d/show/vtk_/win.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.314544 laok-0.2.17/laok/cv3d/trans/
--rw-rw-rw-   0        0        0      192 2023-04-28 03:50:43.000000 laok-0.2.17/laok/cv3d/trans/__init__.py
--rw-rw-rw-   0        0        0      895 2023-04-25 05:31:18.000000 laok-0.2.17/laok/cv3d/trans/_dropout.py
--rw-rw-rw-   0        0        0      726 2023-04-25 05:40:44.000000 laok-0.2.17/laok/cv3d/trans/_jitter.py
--rw-rw-rw-   0        0        0      660 2023-04-25 03:33:54.000000 laok-0.2.17/laok/cv3d/trans/_normal.py
--rw-rw-rw-   0        0        0     5025 2023-04-27 08:53:41.000000 laok-0.2.17/laok/cv3d/trans/_rotate.py
--rw-rw-rw-   0        0        0     2164 2023-04-28 03:50:24.000000 laok-0.2.17/laok/cv3d/trans/_sample.py
--rw-rw-rw-   0        0        0      618 2023-04-25 02:57:52.000000 laok-0.2.17/laok/cv3d/trans/_scale.py
--rw-rw-rw-   0        0        0      485 2023-04-25 03:05:55.000000 laok-0.2.17/laok/cv3d/trans/_torch.py
--rw-rw-rw-   0        0        0      680 2023-04-25 05:38:23.000000 laok-0.2.17/laok/cv3d/trans/_translate.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.315541 laok-0.2.17/laok/dnn/
--rw-rw-rw-   0        0        0       87 2023-04-23 12:48:28.000000 laok-0.2.17/laok/dnn/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.316539 laok-0.2.17/laok/dnn/backbones/
--rw-rw-rw-   0        0        0        0 2023-04-21 09:12:33.000000 laok-0.2.17/laok/dnn/backbones/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.317536 laok-0.2.17/laok/dnn/dataset/
--rw-rw-rw-   0        0        0       58 2023-04-25 06:10:55.000000 laok-0.2.17/laok/dnn/dataset/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.317536 laok-0.2.17/laok/dnn/dataset/cld/
--rw-rw-rw-   0        0        0        0 2023-04-21 09:12:33.000000 laok-0.2.17/laok/dnn/dataset/cld/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.318534 laok-0.2.17/laok/dnn/dataset/img/
--rw-rw-rw-   0        0        0        0 2023-04-21 09:12:33.000000 laok-0.2.17/laok/dnn/dataset/img/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.319530 laok-0.2.17/laok/dnn/dataset/txt/
--rw-rw-rw-   0        0        0       38 2023-04-25 06:10:39.000000 laok-0.2.17/laok/dnn/dataset/txt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.321526 laok-0.2.17/laok/dnn/head/
--rw-rw-rw-   0        0        0        0 2023-04-21 09:12:33.000000 laok-0.2.17/laok/dnn/head/__init__.py
--rw-rw-rw-   0        0        0     1090 2023-04-23 13:35:33.000000 laok-0.2.17/laok/dnn/head/classify.py
--rw-rw-rw-   0        0        0     3178 2023-04-23 13:32:56.000000 laok-0.2.17/laok/dnn/head/detect.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.322522 laok-0.2.17/laok/dnn/layer/
--rw-rw-rw-   0        0        0        0 2023-04-21 09:12:33.000000 laok-0.2.17/laok/dnn/layer/__init__.py
--rw-rw-rw-   0        0        0     2903 2023-04-25 02:35:22.000000 laok-0.2.17/laok/dnn/layer/pooling.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.323520 laok-0.2.17/laok/dnn/loss/
--rw-rw-rw-   0        0        0        0 2023-04-21 09:12:33.000000 laok-0.2.17/laok/dnn/loss/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.324517 laok-0.2.17/laok/dnn/model/
--rw-rw-rw-   0        0        0        0 2023-04-21 09:12:33.000000 laok-0.2.17/laok/dnn/model/__init__.py
--rw-rw-rw-   0        0        0      364 2023-04-23 13:41:53.000000 laok-0.2.17/laok/dnn/model/_torch_vision.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.325514 laok-0.2.17/laok/dnn/neck/
--rw-rw-rw-   0        0        0        0 2023-04-21 09:12:33.000000 laok-0.2.17/laok/dnn/neck/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.326511 laok-0.2.17/laok/ext/
--rw-rw-rw-   0        0        0        0 2023-03-10 09:11:01.000000 laok-0.2.17/laok/ext/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.327509 laok-0.2.17/laok/ext/flask_/
--rw-rw-rw-   0        0        0       42 2023-04-19 15:05:48.000000 laok-0.2.17/laok/ext/flask_/__init__.py
--rw-rw-rw-   0        0        0      395 2023-04-19 15:05:30.000000 laok-0.2.17/laok/ext/flask_/app.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.329503 laok-0.2.17/laok/ext/flask_/basic/
--rw-rw-rw-   0        0        0       22 2023-04-19 15:06:08.000000 laok-0.2.17/laok/ext/flask_/basic/__init__.py
--rw-rw-rw-   0        0        0      633 2023-04-19 15:38:09.000000 laok-0.2.17/laok/ext/flask_/basic/views.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.330501 laok-0.2.17/laok/ext/numpy_/
--rw-rw-rw-   0        0        0        0 2023-04-20 14:21:33.000000 laok-0.2.17/laok/ext/numpy_/__init__.py
--rw-rw-rw-   0        0        0     3022 2023-04-19 07:45:14.000000 laok-0.2.17/laok/ext/onnx_.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.330501 laok-0.2.17/laok/ext/torch_/
--rw-rw-rw-   0        0        0       88 2023-04-19 08:20:33.000000 laok-0.2.17/laok/ext/torch_/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.332496 laok-0.2.17/laok/ext/torch_/datasets/
--rw-rw-rw-   0        0        0        0 2022-10-21 10:13:37.000000 laok-0.2.17/laok/ext/torch_/datasets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.335489 laok-0.2.17/laok/ext/torch_/datasets/kitti/
--rw-rw-rw-   0        0        0        0 2022-10-21 10:13:37.000000 laok-0.2.17/laok/ext/torch_/datasets/kitti/__init__.py
--rw-rw-rw-   0        0        0    12031 2022-11-03 16:22:33.000000 laok-0.2.17/laok/ext/torch_/datasets/kitti/kitti.py
--rw-rw-rw-   0        0        0    27294 2022-10-28 06:48:12.000000 laok-0.2.17/laok/ext/torch_/datasets/kitti/obj.py
--rw-rw-rw-   0        0        0    26349 2022-11-03 16:22:33.000000 laok-0.2.17/laok/ext/torch_/datasets/kitti/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.339477 laok-0.2.17/laok/ext/torch_/datasets/model_net/
--rw-rw-rw-   0        0        0      954 2022-11-03 16:22:33.000000 laok-0.2.17/laok/ext/torch_/datasets/model_net/__init__.py
--rw-rw-rw-   0        0        0     3721 2022-11-03 16:22:33.000000 laok-0.2.17/laok/ext/torch_/datasets/model_net/model_net.py
--rw-rw-rw-   0        0        0     4467 2022-11-03 16:22:33.000000 laok-0.2.17/laok/ext/torch_/datasets/model_net/model_net_ineratia.py
--rw-rw-rw-   0        0        0     3895 2022-11-03 16:22:33.000000 laok-0.2.17/laok/ext/torch_/datasets/model_net/model_net_normals.py
--rw-rw-rw-   0        0        0     4553 2022-11-03 16:22:33.000000 laok-0.2.17/laok/ext/torch_/datasets/model_net/model_net_normals_diff.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.340474 laok-0.2.17/laok/ext/torch_/datasets/shape_net/
--rw-rw-rw-   0        0        0        0 2022-10-21 10:13:37.000000 laok-0.2.17/laok/ext/torch_/datasets/shape_net/__init__.py
--rw-rw-rw-   0        0        0     5463 2022-10-21 10:13:37.000000 laok-0.2.17/laok/ext/torch_/datasets/shape_net/shape_net.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.342469 laok-0.2.17/laok/ext/torch_/datasets/stanford_indoor/
--rw-rw-rw-   0        0        0        0 2022-10-21 10:13:37.000000 laok-0.2.17/laok/ext/torch_/datasets/stanford_indoor/__init__.py
--rw-rw-rw-   0        0        0    11035 2022-10-12 15:00:14.000000 laok-0.2.17/laok/ext/torch_/datasets/stanford_indoor/_stanford_indoor.py
--rw-rw-rw-   0        0        0     2811 2022-11-02 07:35:53.000000 laok-0.2.17/laok/ext/torch_/datasets/ustc_lidar.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.345461 laok-0.2.17/laok/ext/torch_/io/
--rw-rw-rw-   0        0        0       80 2022-10-21 10:13:37.000000 laok-0.2.17/laok/ext/torch_/io/__init__.py
--rw-rw-rw-   0        0        0      732 2022-10-21 10:13:37.000000 laok-0.2.17/laok/ext/torch_/io/img.py
--rw-rw-rw-   0        0        0      844 2022-10-21 10:13:37.000000 laok-0.2.17/laok/ext/torch_/io/jit.py
--rw-rw-rw-   0        0        0     1344 2022-10-21 10:13:37.000000 laok-0.2.17/laok/ext/torch_/io/model.py
--rw-rw-rw-   0        0        0      466 2022-10-21 10:13:37.000000 laok-0.2.17/laok/ext/torch_/io/onnx.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.349452 laok-0.2.17/laok/ext/torch_/op/
--rw-rw-rw-   0        0        0       70 2023-04-19 08:22:19.000000 laok-0.2.17/laok/ext/torch_/op/__init__.py
--rw-rw-rw-   0        0        0      965 2023-04-19 08:22:06.000000 laok-0.2.17/laok/ext/torch_/op/device.py
--rw-rw-rw-   0        0        0     1703 2023-04-19 08:27:44.000000 laok-0.2.17/laok/ext/torch_/op/module.py
--rw-rw-rw-   0        0        0     1403 2023-04-19 08:25:22.000000 laok-0.2.17/laok/ext/torch_/op/print_info.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.354437 laok-0.2.17/laok/ext/torch_/trainval/
--rw-rw-rw-   0        0        0       89 2022-10-21 10:13:37.000000 laok-0.2.17/laok/ext/torch_/trainval/__init__.py
--rw-rw-rw-   0        0        0     3943 2023-04-19 09:12:20.000000 laok-0.2.17/laok/ext/torch_/trainval/check_point.py
--rw-rw-rw-   0        0        0     2280 2023-04-19 09:25:29.000000 laok-0.2.17/laok/ext/torch_/trainval/infer.py
--rw-rw-rw-   0        0        0     2848 2023-04-19 08:44:39.000000 laok-0.2.17/laok/ext/torch_/trainval/train.py
--rw-rw-rw-   0        0        0     2308 2023-04-19 09:08:59.000000 laok-0.2.17/laok/ext/torch_/trainval/val.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.355435 laok-0.2.17/laok/ml/
--rw-rw-rw-   0        0        0        0 2023-04-21 09:13:48.000000 laok-0.2.17/laok/ml/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.355435 laok-0.2.17/laok/tool/
--rw-rw-rw-   0        0        0        0 2023-05-04 12:52:02.000000 laok-0.2.17/laok/tool/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.357429 laok-0.2.17/laok/tool/ultralytics_/
--rw-rw-rw-   0        0        0       28 2023-05-04 12:43:29.000000 laok-0.2.17/laok/tool/ultralytics_/__init__.py
--rw-rw-rw-   0        0        0      100 2023-05-04 12:56:44.000000 laok-0.2.17/laok/tool/ultralytics_/__main__.py
--rw-rw-rw-   0        0        0     2094 2023-05-04 14:42:16.000000 laok-0.2.17/laok/tool/ultralytics_/train_det.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.267669 laok-0.2.17/laok.egg-info/
--rw-rw-rw-   0        0        0      217 2023-05-05 09:26:36.000000 laok-0.2.17/laok.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3661 2023-05-05 09:26:37.000000 laok-0.2.17/laok.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 09:26:36.000000 laok-0.2.17/laok.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-05 09:26:36.000000 laok-0.2.17/laok.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 09:26:37.359424 laok-0.2.17/setup.cfg
--rw-rw-rw-   0        0        0      325 2023-05-05 09:24:17.000000 laok-0.2.17/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.576877 laok-0.2.18/
+-rw-rw-rw-   0        0        0      217 2023-07-04 02:41:42.576877 laok-0.2.18/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.383395 laok-0.2.18/laok/
+-rw-rw-rw-   0        0        0       21 2023-06-01 07:56:50.000000 laok-0.2.18/laok/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.389380 laok-0.2.18/laok/base/
+-rw-rw-rw-   0        0        0      248 2023-06-06 13:49:22.000000 laok-0.2.18/laok/base/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.391374 laok-0.2.18/laok/base/alg/
+-rw-rw-rw-   0        0        0       26 2023-04-20 13:21:17.000000 laok-0.2.18/laok/base/alg/__init__.py
+-rw-rw-rw-   0        0        0     4923 2023-04-20 13:20:53.000000 laok-0.2.18/laok/base/alg/addict.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.396360 laok-0.2.18/laok/base/conf/
+-rw-rw-rw-   0        0        0       32 2023-06-10 01:32:44.000000 laok-0.2.18/laok/base/conf/__init__.py
+-rw-rw-rw-   0        0        0      360 2023-04-19 14:40:47.000000 laok-0.2.18/laok/base/conf/conf_global.py
+-rw-rw-rw-   0        0        0     3022 2023-06-10 01:32:49.000000 laok-0.2.18/laok/base/conf/factory.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.400349 laok-0.2.18/laok/base/dataset/
+-rw-rw-rw-   0        0        0        0 2023-04-21 04:27:16.000000 laok-0.2.18/laok/base/dataset/__init__.py
+-rw-rw-rw-   0        0        0     6406 2023-04-21 04:29:54.000000 laok-0.2.18/laok/base/dataset/cvt_voc_yolo.py
+-rw-rw-rw-   0        0        0     2405 2019-09-12 10:55:17.000000 laok-0.2.18/laok/base/dataset/darknet-voc2yolo.py
+-rw-rw-rw-   0        0        0     2241 2019-02-18 15:12:05.000000 laok-0.2.18/laok/base/dataset/voc_label.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.404338 laok-0.2.18/laok/base/dtime/
+-rw-rw-rw-   0        0        0       47 2022-10-21 10:13:37.000000 laok-0.2.18/laok/base/dtime/__init__.py
+-rw-rw-rw-   0        0        0      556 2022-11-17 01:18:56.000000 laok-0.2.18/laok/base/dtime/datetime_.py
+-rw-rw-rw-   0        0        0     2727 2023-04-19 11:27:09.000000 laok-0.2.18/laok/base/dtime/timer.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.411320 laok-0.2.18/laok/base/fs/
+-rw-rw-rw-   0        0        0      134 2023-05-04 11:06:57.000000 laok-0.2.18/laok/base/fs/__init__.py
+-rw-rw-rw-   0        0        0     2591 2023-06-27 16:15:40.000000 laok-0.2.18/laok/base/fs/fdata.py
+-rw-rw-rw-   0        0        0     2937 2022-11-03 16:22:33.000000 laok-0.2.18/laok/base/fs/fname.py
+-rw-rw-rw-   0        0        0     4629 2023-06-27 16:03:41.000000 laok-0.2.18/laok/base/fs/fpath.py
+-rw-rw-rw-   0        0        0     1785 2023-05-04 11:06:06.000000 laok-0.2.18/laok/base/fs/fsearch.py
+-rw-rw-rw-   0        0        0     2819 2023-05-05 03:57:37.000000 laok-0.2.18/laok/base/fs/fwalk.py
+-rw-rw-rw-   0        0        0     1413 2023-04-19 09:23:34.000000 laok-0.2.18/laok/base/fs/name_index.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.413315 laok-0.2.18/laok/base/log/
+-rw-rw-rw-   0        0        0       50 2023-04-19 14:41:08.000000 laok-0.2.18/laok/base/log/__init__.py
+-rw-rw-rw-   0        0        0     2185 2023-04-19 14:41:16.000000 laok-0.2.18/laok/base/log/log.py
+-rw-rw-rw-   0        0        0      672 2023-04-19 14:43:17.000000 laok-0.2.18/laok/base/log/log_default.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.417303 laok-0.2.18/laok/base/net/
+-rw-rw-rw-   0        0        0       78 2023-06-06 16:23:58.000000 laok-0.2.18/laok/base/net/__init__.py
+-rw-rw-rw-   0        0        0      691 2022-09-23 00:45:15.000000 laok-0.2.18/laok/base/net/ip.py
+-rw-rw-rw-   0        0        0     3792 2023-06-27 10:59:29.000000 laok-0.2.18/laok/base/net/requests_.py
+-rw-rw-rw-   0        0        0     1200 2023-06-27 10:55:31.000000 laok-0.2.18/laok/base/net/url.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.420296 laok-0.2.18/laok/base/paral/
+-rw-rw-rw-   0        0        0       20 2022-10-21 10:13:37.000000 laok-0.2.18/laok/base/paral/__init__.py
+-rw-rw-rw-   0        0        0     2010 2023-04-20 15:21:46.000000 laok-0.2.18/laok/base/paral/pool.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.424289 laok-0.2.18/laok/base/pkg/
+-rw-rw-rw-   0        0        0       32 2023-07-03 15:46:47.000000 laok-0.2.18/laok/base/pkg/__init__.py
+-rw-rw-rw-   0        0        0    27875 2023-07-03 15:50:30.000000 laok-0.2.18/laok/base/pkg/_lazy.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.433261 laok-0.2.18/laok/base/ser/
+-rw-rw-rw-   0        0        0      156 2023-06-06 14:13:13.000000 laok-0.2.18/laok/base/ser/__init__.py
+-rw-rw-rw-   0        0        0     1367 2023-04-25 06:50:06.000000 laok-0.2.18/laok/base/ser/json_.py
+-rw-rw-rw-   0        0        0      750 2023-04-20 13:46:22.000000 laok-0.2.18/laok/base/ser/marshal_.py
+-rw-rw-rw-   0        0        0      676 2023-06-01 07:58:10.000000 laok-0.2.18/laok/base/ser/numpy_.py
+-rw-rw-rw-   0        0        0      621 2023-04-25 06:50:29.000000 laok-0.2.18/laok/base/ser/pickle_.py
+-rw-rw-rw-   0        0        0     1369 2023-06-10 01:42:11.000000 laok-0.2.18/laok/base/ser/torch_.py
+-rw-rw-rw-   0        0        0     1452 2023-06-06 17:03:52.000000 laok-0.2.18/laok/base/ser/xml_.py
+-rw-rw-rw-   0        0        0     1341 2023-06-01 07:57:17.000000 laok-0.2.18/laok/base/ser/yaml_.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.443234 laok-0.2.18/laok/base/str/
+-rw-rw-rw-   0        0        0       84 2023-06-10 01:11:15.000000 laok-0.2.18/laok/base/str/__init__.py
+-rw-rw-rw-   0        0        0      735 2023-06-10 01:09:44.000000 laok-0.2.18/laok/base/str/cvt.py
+-rw-rw-rw-   0        0        0      427 2023-06-10 01:10:45.000000 laok-0.2.18/laok/base/str/fmt.py
+-rw-rw-rw-   0        0        0     1705 2023-06-10 01:10:56.000000 laok-0.2.18/laok/base/str/misc.py
+-rw-rw-rw-   0        0        0     2588 2023-06-01 07:58:57.000000 laok-0.2.18/laok/base/str/print_info.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.446226 laok-0.2.18/laok/base/syst/
+-rw-rw-rw-   0        0        0       74 2023-07-03 11:23:20.000000 laok-0.2.18/laok/base/syst/__init__.py
+-rw-rw-rw-   0        0        0      518 2023-05-04 15:23:10.000000 laok-0.2.18/laok/base/syst/platform_.py
+-rw-rw-rw-   0        0        0     1871 2022-10-21 10:13:37.000000 laok-0.2.18/laok/base/syst/print_info.py
+-rw-rw-rw-   0        0        0      380 2023-07-03 11:23:24.000000 laok-0.2.18/laok/base/syst/sys_.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.451216 laok-0.2.18/laok/base/test/
+-rw-rw-rw-   0        0        0       43 2022-10-21 10:13:37.000000 laok-0.2.18/laok/base/test/__init__.py
+-rw-rw-rw-   0        0        0     8046 2023-06-01 03:25:20.000000 laok-0.2.18/laok/base/test/_dump.py
+-rw-rw-rw-   0        0        0     4551 2023-06-01 05:41:11.000000 laok-0.2.18/laok/base/test/_run.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.452212 laok-0.2.18/laok/cv2d/
+-rw-rw-rw-   0        0        0       62 2023-05-12 07:14:57.000000 laok-0.2.18/laok/cv2d/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.461186 laok-0.2.18/laok/cv2d/cvt/
+-rw-rw-rw-   0        0        0       86 2022-11-15 13:19:23.000000 laok-0.2.18/laok/cv2d/cvt/__init__.py
+-rw-rw-rw-   0        0        0     2974 2022-11-15 13:18:48.000000 laok-0.2.18/laok/cv2d/cvt/cv2_.py
+-rw-rw-rw-   0        0        0     2075 2022-10-16 09:36:58.000000 laok-0.2.18/laok/cv2d/cvt/misc_.py
+-rw-rw-rw-   0        0        0      430 2022-09-04 16:11:38.000000 laok-0.2.18/laok/cv2d/cvt/pil_.py
+-rw-rw-rw-   0        0        0      469 2022-09-04 16:11:47.000000 laok-0.2.18/laok/cv2d/cvt/sk_.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.465175 laok-0.2.18/laok/cv2d/draw/
+-rw-rw-rw-   0        0        0       45 2022-10-24 11:22:11.000000 laok-0.2.18/laok/cv2d/draw/__init__.py
+-rw-rw-rw-   0        0        0     8383 2022-10-18 15:38:38.000000 laok-0.2.18/laok/cv2d/draw/color.py
+-rw-rw-rw-   0        0        0      975 2023-06-01 05:40:03.000000 laok-0.2.18/laok/cv2d/draw/cv2_.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.469167 laok-0.2.18/laok/cv2d/io/
+-rw-rw-rw-   0        0        0       42 2023-05-12 07:11:13.000000 laok-0.2.18/laok/cv2d/io/__init__.py
+-rw-rw-rw-   0        0        0     3226 2023-06-06 13:44:51.000000 laok-0.2.18/laok/cv2d/io/cv2_.py
+-rw-rw-rw-   0        0        0      592 2023-06-06 13:41:32.000000 laok-0.2.18/laok/cv2d/io/pil_.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.473156 laok-0.2.18/laok/cv2d/morph/
+-rw-rw-rw-   0        0        0       21 2023-05-12 07:10:07.000000 laok-0.2.18/laok/cv2d/morph/__init__.py
+-rw-rw-rw-   0        0        0     3471 2023-06-06 13:41:42.000000 laok-0.2.18/laok/cv2d/morph/cv2_.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.478143 laok-0.2.18/laok/cv2d/show/
+-rw-rw-rw-   0        0        0       63 2023-05-12 07:14:23.000000 laok-0.2.18/laok/cv2d/show/__init__.py
+-rw-rw-rw-   0        0        0     1164 2023-06-06 13:42:01.000000 laok-0.2.18/laok/cv2d/show/cv2_.py
+-rw-rw-rw-   0        0        0        0 2023-05-12 08:19:43.000000 laok-0.2.18/laok/cv2d/show/pil_.py
+-rw-rw-rw-   0        0        0     1057 2023-07-03 15:41:51.000000 laok-0.2.18/laok/cv2d/show/plt_.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.480136 laok-0.2.18/laok/cv3d/
+-rw-rw-rw-   0        0        0       64 2023-04-21 09:21:19.000000 laok-0.2.18/laok/cv3d/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.483132 laok-0.2.18/laok/cv3d/io/
+-rw-rw-rw-   0        0        0       24 2023-04-21 09:18:03.000000 laok-0.2.18/laok/cv3d/io/__init__.py
+-rw-rw-rw-   0        0        0      832 2023-04-25 06:52:21.000000 laok-0.2.18/laok/cv3d/io/_simple.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.484130 laok-0.2.18/laok/cv3d/show/
+-rw-rw-rw-   0        0        0       21 2023-04-21 09:20:03.000000 laok-0.2.18/laok/cv3d/show/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.489121 laok-0.2.18/laok/cv3d/show/vtk_/
+-rw-rw-rw-   0        0        0      804 2023-04-21 09:21:01.000000 laok-0.2.18/laok/cv3d/show/vtk_/__init__.py
+-rw-rw-rw-   0        0        0     3916 2022-10-21 10:13:38.000000 laok-0.2.18/laok/cv3d/show/vtk_/win.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.504075 laok-0.2.18/laok/cv3d/trans/
+-rw-rw-rw-   0        0        0      220 2023-06-16 08:02:42.000000 laok-0.2.18/laok/cv3d/trans/__init__.py
+-rw-rw-rw-   0        0        0      895 2023-04-25 05:31:18.000000 laok-0.2.18/laok/cv3d/trans/_dropout.py
+-rw-rw-rw-   0        0        0      726 2023-04-25 05:40:44.000000 laok-0.2.18/laok/cv3d/trans/_jitter.py
+-rw-rw-rw-   0        0        0      660 2023-04-25 03:33:54.000000 laok-0.2.18/laok/cv3d/trans/_normal.py
+-rw-rw-rw-   0        0        0     5025 2023-04-27 08:53:41.000000 laok-0.2.18/laok/cv3d/trans/_rotate.py
+-rw-rw-rw-   0        0        0     2164 2023-04-28 03:50:24.000000 laok-0.2.18/laok/cv3d/trans/_sample.py
+-rw-rw-rw-   0        0        0      618 2023-04-25 02:57:52.000000 laok-0.2.18/laok/cv3d/trans/_scale.py
+-rw-rw-rw-   0        0        0      585 2023-06-16 09:05:52.000000 laok-0.2.18/laok/cv3d/trans/_swap_filed.py
+-rw-rw-rw-   0        0        0      485 2023-04-25 03:05:55.000000 laok-0.2.18/laok/cv3d/trans/_torch.py
+-rw-rw-rw-   0        0        0      680 2023-04-25 05:38:23.000000 laok-0.2.18/laok/cv3d/trans/_translate.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.507065 laok-0.2.18/laok/dnn/
+-rw-rw-rw-   0        0        0       87 2023-04-23 12:48:28.000000 laok-0.2.18/laok/dnn/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.510056 laok-0.2.18/laok/dnn/backbones/
+-rw-rw-rw-   0        0        0        0 2023-04-21 09:12:33.000000 laok-0.2.18/laok/dnn/backbones/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.512051 laok-0.2.18/laok/dnn/dataset/
+-rw-rw-rw-   0        0        0       58 2023-04-25 06:10:55.000000 laok-0.2.18/laok/dnn/dataset/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.514055 laok-0.2.18/laok/dnn/dataset/cld/
+-rw-rw-rw-   0        0        0        0 2023-04-21 09:12:33.000000 laok-0.2.18/laok/dnn/dataset/cld/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.515044 laok-0.2.18/laok/dnn/dataset/img/
+-rw-rw-rw-   0        0        0        0 2023-04-21 09:12:33.000000 laok-0.2.18/laok/dnn/dataset/img/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.517037 laok-0.2.18/laok/dnn/dataset/txt/
+-rw-rw-rw-   0        0        0       38 2023-04-25 06:10:39.000000 laok-0.2.18/laok/dnn/dataset/txt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.522024 laok-0.2.18/laok/dnn/head/
+-rw-rw-rw-   0        0        0        0 2023-04-21 09:12:33.000000 laok-0.2.18/laok/dnn/head/__init__.py
+-rw-rw-rw-   0        0        0     1090 2023-04-23 13:35:33.000000 laok-0.2.18/laok/dnn/head/classify.py
+-rw-rw-rw-   0        0        0     3178 2023-04-23 13:32:56.000000 laok-0.2.18/laok/dnn/head/detect.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.524019 laok-0.2.18/laok/dnn/layer/
+-rw-rw-rw-   0        0        0        0 2023-04-21 09:12:33.000000 laok-0.2.18/laok/dnn/layer/__init__.py
+-rw-rw-rw-   0        0        0     2903 2023-04-25 02:35:22.000000 laok-0.2.18/laok/dnn/layer/pooling.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.525018 laok-0.2.18/laok/dnn/loss/
+-rw-rw-rw-   0        0        0        0 2023-04-21 09:12:33.000000 laok-0.2.18/laok/dnn/loss/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.529006 laok-0.2.18/laok/dnn/model/
+-rw-rw-rw-   0        0        0        0 2023-04-21 09:12:33.000000 laok-0.2.18/laok/dnn/model/__init__.py
+-rw-rw-rw-   0        0        0      364 2023-04-23 13:41:53.000000 laok-0.2.18/laok/dnn/model/_torch_vision.py
+-rw-rw-rw-   0        0        0        0 2023-05-25 08:13:53.000000 laok-0.2.18/laok/dnn/model/arc_face.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.530003 laok-0.2.18/laok/dnn/neck/
+-rw-rw-rw-   0        0        0        0 2023-04-21 09:12:33.000000 laok-0.2.18/laok/dnn/neck/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.532995 laok-0.2.18/laok/ext/
+-rw-rw-rw-   0        0        0        0 2023-03-10 09:11:01.000000 laok-0.2.18/laok/ext/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.536991 laok-0.2.18/laok/ext/flask_/
+-rw-rw-rw-   0        0        0       42 2023-04-19 15:05:48.000000 laok-0.2.18/laok/ext/flask_/__init__.py
+-rw-rw-rw-   0        0        0      395 2023-04-19 15:05:30.000000 laok-0.2.18/laok/ext/flask_/app.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.538979 laok-0.2.18/laok/ext/flask_/basic/
+-rw-rw-rw-   0        0        0       22 2023-04-19 15:06:08.000000 laok-0.2.18/laok/ext/flask_/basic/__init__.py
+-rw-rw-rw-   0        0        0      633 2023-04-19 15:38:09.000000 laok-0.2.18/laok/ext/flask_/basic/views.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.539976 laok-0.2.18/laok/ext/numpy_/
+-rw-rw-rw-   0        0        0        0 2023-04-20 14:21:33.000000 laok-0.2.18/laok/ext/numpy_/__init__.py
+-rw-rw-rw-   0        0        0     3022 2023-04-19 07:45:14.000000 laok-0.2.18/laok/ext/onnx_.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.540975 laok-0.2.18/laok/ext/torch_/
+-rw-rw-rw-   0        0        0       88 2023-04-19 08:20:33.000000 laok-0.2.18/laok/ext/torch_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.543965 laok-0.2.18/laok/ext/torch_/datasets/
+-rw-rw-rw-   0        0        0        0 2022-10-21 10:13:37.000000 laok-0.2.18/laok/ext/torch_/datasets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.547957 laok-0.2.18/laok/ext/torch_/datasets/kitti/
+-rw-rw-rw-   0        0        0        0 2022-10-21 10:13:37.000000 laok-0.2.18/laok/ext/torch_/datasets/kitti/__init__.py
+-rw-rw-rw-   0        0        0    12031 2022-11-03 16:22:33.000000 laok-0.2.18/laok/ext/torch_/datasets/kitti/kitti.py
+-rw-rw-rw-   0        0        0    27294 2022-10-28 06:48:12.000000 laok-0.2.18/laok/ext/torch_/datasets/kitti/obj.py
+-rw-rw-rw-   0        0        0    26349 2022-11-03 16:22:33.000000 laok-0.2.18/laok/ext/torch_/datasets/kitti/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.555933 laok-0.2.18/laok/ext/torch_/datasets/model_net/
+-rw-rw-rw-   0        0        0      954 2022-11-03 16:22:33.000000 laok-0.2.18/laok/ext/torch_/datasets/model_net/__init__.py
+-rw-rw-rw-   0        0        0     3721 2022-11-03 16:22:33.000000 laok-0.2.18/laok/ext/torch_/datasets/model_net/model_net.py
+-rw-rw-rw-   0        0        0     4467 2022-11-03 16:22:33.000000 laok-0.2.18/laok/ext/torch_/datasets/model_net/model_net_ineratia.py
+-rw-rw-rw-   0        0        0     3895 2022-11-03 16:22:33.000000 laok-0.2.18/laok/ext/torch_/datasets/model_net/model_net_normals.py
+-rw-rw-rw-   0        0        0     4553 2022-11-03 16:22:33.000000 laok-0.2.18/laok/ext/torch_/datasets/model_net/model_net_normals_diff.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.557927 laok-0.2.18/laok/ext/torch_/datasets/shape_net/
+-rw-rw-rw-   0        0        0        0 2022-10-21 10:13:37.000000 laok-0.2.18/laok/ext/torch_/datasets/shape_net/__init__.py
+-rw-rw-rw-   0        0        0     5463 2022-10-21 10:13:37.000000 laok-0.2.18/laok/ext/torch_/datasets/shape_net/shape_net.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.559922 laok-0.2.18/laok/ext/torch_/datasets/stanford_indoor/
+-rw-rw-rw-   0        0        0        0 2022-10-21 10:13:37.000000 laok-0.2.18/laok/ext/torch_/datasets/stanford_indoor/__init__.py
+-rw-rw-rw-   0        0        0    11035 2022-10-12 15:00:14.000000 laok-0.2.18/laok/ext/torch_/datasets/stanford_indoor/_stanford_indoor.py
+-rw-rw-rw-   0        0        0     2811 2022-11-02 07:35:53.000000 laok-0.2.18/laok/ext/torch_/datasets/ustc_lidar.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.564909 laok-0.2.18/laok/ext/torch_/io/
+-rw-rw-rw-   0        0        0       80 2022-10-21 10:13:37.000000 laok-0.2.18/laok/ext/torch_/io/__init__.py
+-rw-rw-rw-   0        0        0      732 2022-10-21 10:13:37.000000 laok-0.2.18/laok/ext/torch_/io/img.py
+-rw-rw-rw-   0        0        0      844 2022-10-21 10:13:37.000000 laok-0.2.18/laok/ext/torch_/io/jit.py
+-rw-rw-rw-   0        0        0     1344 2022-10-21 10:13:37.000000 laok-0.2.18/laok/ext/torch_/io/model.py
+-rw-rw-rw-   0        0        0      466 2022-10-21 10:13:37.000000 laok-0.2.18/laok/ext/torch_/io/onnx.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.568900 laok-0.2.18/laok/ext/torch_/op/
+-rw-rw-rw-   0        0        0       70 2023-04-19 08:22:19.000000 laok-0.2.18/laok/ext/torch_/op/__init__.py
+-rw-rw-rw-   0        0        0      965 2023-04-19 08:22:06.000000 laok-0.2.18/laok/ext/torch_/op/device.py
+-rw-rw-rw-   0        0        0     1703 2023-04-19 08:27:44.000000 laok-0.2.18/laok/ext/torch_/op/module.py
+-rw-rw-rw-   0        0        0     1403 2023-04-19 08:25:22.000000 laok-0.2.18/laok/ext/torch_/op/print_info.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.574882 laok-0.2.18/laok/ext/torch_/trainval/
+-rw-rw-rw-   0        0        0       89 2022-10-21 10:13:37.000000 laok-0.2.18/laok/ext/torch_/trainval/__init__.py
+-rw-rw-rw-   0        0        0     3943 2023-04-19 09:12:20.000000 laok-0.2.18/laok/ext/torch_/trainval/check_point.py
+-rw-rw-rw-   0        0        0     2280 2023-04-19 09:25:29.000000 laok-0.2.18/laok/ext/torch_/trainval/infer.py
+-rw-rw-rw-   0        0        0     2848 2023-04-19 08:44:39.000000 laok-0.2.18/laok/ext/torch_/trainval/train.py
+-rw-rw-rw-   0        0        0     2308 2023-04-19 09:08:59.000000 laok-0.2.18/laok/ext/torch_/trainval/val.py
+-rw-rw-rw-   0        0        0     2310 2023-07-04 02:40:34.000000 laok-0.2.18/laok/ext/ultralytics_.py
+-rw-rw-rw-   0        0        0      649 2023-07-03 15:46:51.000000 laok-0.2.18/laok/third_lib.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.388381 laok-0.2.18/laok.egg-info/
+-rw-rw-rw-   0        0        0      217 2023-07-04 02:41:42.000000 laok-0.2.18/laok.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4146 2023-07-04 02:41:42.000000 laok-0.2.18/laok.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 02:41:42.000000 laok-0.2.18/laok.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-04 02:41:42.000000 laok-0.2.18/laok.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 02:41:42.576877 laok-0.2.18/setup.cfg
+-rw-rw-rw-   0        0        0      325 2023-07-04 02:36:00.000000 laok-0.2.18/setup.py
```

### Comparing `laok-0.2.17/laok/base/alg/addict.py` & `laok-0.2.18/laok/base/alg/addict.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/base/dataset/cvt_voc_yolo.py` & `laok-0.2.18/laok/base/dataset/cvt_voc_yolo.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/base/dataset/darknet-voc2yolo.py` & `laok-0.2.18/laok/base/dataset/darknet-voc2yolo.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/base/dataset/voc_label.py` & `laok-0.2.18/laok/base/dataset/voc_label.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/base/dtime/datetime_.py` & `laok-0.2.18/laok/base/dtime/datetime_.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/base/dtime/timer.py` & `laok-0.2.18/laok/base/dtime/timer.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/base/fs/fdata.py` & `laok-0.2.18/laok/base/fs/fdata.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 # -*- coding: utf-8 -*-
 '''
 Created on 2022/10/16 10:05:28
 
 @author: LiuKuan
 @copyright: Apache License, Version 2.0
 '''
+from .fpath import path_exist
 # ===============================================================================
 r'''
 '''
 # ===============================================================================
 __all__ = ['file_read_text', 'file_write_text', 'file_read_lines', 'file_write_lines',
-           'file_read_bin', 'file_write_bin',
+           'file_read_bin', 'file_read_chunk', 'file_write_bin',
            'file_text_reader', 'file_bin_reader',
-           'file_bin_writer', 'file_text_writer'
+           'file_bin_writer', 'file_text_writer',
+           'file_list_merge'
            ]
 
 def file_text_reader(fname, encoding='utf8'):
     return open(fname, mode='r', encoding=encoding)
 
 def file_bin_reader(fname):
     return open(fname, mode='rb')
@@ -28,31 +30,55 @@
 def file_bin_writer(fname):
     return open(fname, mode='wb')
 
 def file_read_text(fname, encoding='utf8'):
     with open(fname, mode='r', encoding=encoding) as f:
         return f.read()
 
-def file_write_text(text, fname, encoding='utf8'):
+def file_write_text(fname, text, encoding='utf8', skip_exist=False):
+    if skip_exist and path_exist(fname):
+        return
     with open(fname, mode='w', encoding=encoding) as f:
         f.write(text)
 
-def file_read_lines(fname, encoding='utf8', strip = True):
+def file_read_lines(fname, encoding='utf8', strip = True, skip_empty=False):
     with open(fname, mode='r', encoding=encoding) as f:
         for line in f:
             if strip:
                 line = line.strip()
+            if skip_empty:
+                if not line :
+                    continue
             yield line
 
-def file_write_lines(lines, fname, encoding='utf8', line_append='\n'):
+def file_write_lines(fname, lines, encoding='utf8', line_append='\n', skip_exist=False):
+    if skip_exist and path_exist(fname):
+        return
+
     with open(fname, mode='w', encoding=encoding) as f:
         for line in lines:
             f.write(line + line_append)
 
 def file_read_bin(fname):
     with open(fname, mode='rb') as f:
         return f.read()
 
-def file_write_bin(data, fname):
+def file_read_chunk(fname, buf_size=1e6):
+    buf_size = int(buf_size)
+    with open(fname, mode='rb') as f:
+        while True:
+            data = f.read(buf_size)
+            if not data:
+                break
+            yield data
+
+def file_write_bin(fname, data, skip_exist=False):
+    if skip_exist and path_exist(fname):
+        return
     with open(fname, mode='wb') as f:
         f.write(data)
 
+def file_list_merge(file_list, dst_file, buf_size=4e6):
+    with file_bin_writer(dst_file) as df:
+        for fname in file_list:
+            for data in file_read_chunk(fname):
+                df.write(data)
```

### Comparing `laok-0.2.17/laok/base/fs/fname.py` & `laok-0.2.18/laok/base/fs/fname.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/base/fs/fpath.py` & `laok-0.2.18/laok/base/fs/fpath.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 __all__ = [ 'path_rename', 'path_native', 'path_unix', 'path_win', 'path_relative',
             'path_parent', 'path_make', 'path_make_parent',
             'path_join', 'path_abs', 'path_exist',
             'file_size', 'path_is_file', 'path_is_dir',
             'path_basename', 'path_stem', 'path_ext','path_add_ext', 'path_rm_ext',
             'path_replace_ext', 'path_replace_stem', 'path_replace_basename', 'path_replace_parent',
             'dirs_delete', 'file_delete',
+            'path_deco_stem',
             'work_dir_scope', 'path_set_cur', 'path_get_cur',
             'files_env', 'file_env', 'path_exe_files', 'path_exe_file',
             ]
 
 def path_rename(old_name, new_name):
     os.rename(old_name, new_name)
 
@@ -110,14 +111,19 @@
     return path_unix(new_file)
 
 def path_replace_stem(file_path, basename):
     _dir, _fname = opath.split(file_path)
     _basename, _ext = opath.splitext(_fname)
     return path_join(_dir, basename + _ext)
 
+def path_deco_stem(file_path, preffix='', suffix=''):
+    _dir, _fname = opath.split(file_path)
+    _basename, _ext = opath.splitext(_fname)
+    return path_join(_dir, preffix + _basename + suffix + _ext)
+
 def path_replace_basename(file_path, filename):
     _dir, _fname = opath.split(file_path)
     return path_join(_dir, filename)
 
 def path_replace_parent(file_path, parent):
     _dir, _fname = opath.split(file_path)
     return path_join(parent, _fname)
```

### Comparing `laok-0.2.17/laok/base/fs/fsearch.py` & `laok-0.2.18/laok/base/fs/fsearch.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/base/fs/fwalk.py` & `laok-0.2.18/laok/base/fs/fwalk.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/base/fs/name_index.py` & `laok-0.2.18/laok/base/fs/name_index.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/base/func/print_info.py` & `laok-0.2.18/laok/base/syst/print_info.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/base/log/log.py` & `laok-0.2.18/laok/base/log/log.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/base/log/log_default.py` & `laok-0.2.18/laok/base/log/log_default.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/base/net/ip.py` & `laok-0.2.18/laok/base/net/ip.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/base/parallel/pool.py` & `laok-0.2.18/laok/base/paral/pool.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/base/ser/_json.py` & `laok-0.2.18/laok/base/ser/json_.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/base/ser/_marshal.py` & `laok-0.2.18/laok/base/ser/marshal_.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/base/ser/_pickle.py` & `laok-0.2.18/laok/base/ser/pickle_.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/base/ser/numpy_.py` & `laok-0.2.18/laok/base/ser/numpy_.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*-
 '''
 Created on 2023/4/25 14:32:07
 @author: LiuKuan
 @copyright: Apache License, Version 2.0
 '''
+from laok.third_lib import np
 #===============================================================================
 r'''
 '''
 #===============================================================================
 __all__ = ['load_np_file', 'save_np_file', 'save_npz_file']
-
 def load_np_file(filename, encoding='ASCII'):
-    import numpy as np
     return np.load(filename, encoding=encoding)
 
 def save_np_file(filename, arr):
-    import numpy as np
     return np.save(filename, arr)
 
 def save_npz_file(filename, *args, **kwds):
-    import numpy as np
     return np.savez(filename, *args, **kwds)
```

### Comparing `laok-0.2.17/laok/base/ser/yaml_.py` & `laok-0.2.18/laok/base/ser/yaml_.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,39 +2,36 @@
 # -*- coding: utf-8 -*-
 '''
 Created on 2022/10/17 19:56:46
 
 @author: LiuKuan
 @copyright: Apache License, Version 2.0
 '''
+from laok.third_lib import yaml
 from collections import OrderedDict
 from ..alg import Dict
 # ===============================================================================
 r'''
 '''
 # ===============================================================================
 __all__ = ['save_yaml_file', 'load_yaml_file']
 
 def save_yaml_file(filename, obj, indent=2, **kws):
-    import yaml
     with open(filename, mode='w', encoding='utf8') as f:
         if isinstance(obj, (OrderedDict, Dict) ):
             _dict_dump(obj, f, indent=indent, **kws)
         else:
             yaml.safe_dump(data=obj, stream=f, indent=indent,**kws)
     return True
 
-
 def load_yaml_file(filename, **kws):
-    import yaml
     with open(filename, encoding='utf8') as f:
         return yaml.safe_load(f, **kws)
 
 def _dict_dump(data, stream=None, **kwds):
-    import yaml
     class DictDumper(yaml.Dumper):
         pass
 
     def _dict_representer(dumper, data):
         return dumper.represent_mapping(yaml.resolver.BaseResolver.DEFAULT_MAPPING_TAG, data.items())
 
     DictDumper.add_representer(OrderedDict, _dict_representer)
```

### Comparing `laok-0.2.17/laok/base/str/misc.py` & `laok-0.2.18/laok/base/str/misc.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,22 +8,16 @@
 '''
 from io import StringIO
 from pprint import pprint
 #===============================================================================
 '''     
 '''
 #===============================================================================
-__all__ = ['float_value', 'pprint_str', 'val_to_list',
-           'size_to_str', 'dict_to_str', 'parse_index_list']
-
-def float_value(val, default=None):
-    try:
-        return float(val)
-    except:
-        return default
+__all__ = [ 'pprint_str', 'val_to_list',
+            'dict_to_str', 'parse_index_list']
 
 def pprint_str(obj, indent=4, width=80, depth=None, compact=False, sort_dicts=True):
     s = StringIO()
     pprint(obj, s, indent=indent, width=width, depth=depth, compact=compact, sort_dicts=sort_dicts)
     return s.getvalue()
 
 def val_to_list(val, sep=';'):
@@ -31,16 +25,15 @@
         return ()
     if isinstance(val, (list,tuple)):
         return val
     if isinstance(val, str):
         return val.split(sep)
     return val
 
-def size_to_str(sizes):
-    return "(" + ", ".join( str(sz) for sz in sizes)  + ")";
+
 
 def dict_to_str(obj, start=10, stop=10):
     sz = len(obj)
     _istart = start
     _iend = sz - stop
     _once = True
```

### Comparing `laok-0.2.17/laok/base/str/print_info.py` & `laok-0.2.18/laok/base/str/print_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 '''
 Created on 2022/8/31 20:14:34
 
 @author: LiuKuan
 @copyright: Apache License, Version 2.0
 '''
 import sys, types
-import inspect as inspect
+import inspect
 from pprint import pprint
 # ===============================================================================
 r'''提供一些调试方便的函数
 '''
 # ===============================================================================
 __all__ = ['pprint', 'print_args','print_eval',
            'print_type', 'print_repr', 'print_signature',
```

### Comparing `laok-0.2.17/laok/base/sys_/platform_.py` & `laok-0.2.18/laok/base/syst/platform_.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/base/test/_dump.py` & `laok-0.2.18/laok/base/test/_dump.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,41 +75,41 @@
         else:
             all_Attr.append(item)
 
     if all_ModuleType:
         stream.write('##### module\n')
         for k,v in all_ModuleType:
             if dump_format is None:
-                stream.write('\t# %s[%s]\n' % (k, _val_doc(v)))
+                stream.write('  # %s[%s]\n' % (k, _val_doc(v)))
             else:
-                stream.write('%s #[%s]\n' % (k, _val_doc(v)))
+                stream.write('  %s #[%s]\n' % (k, _val_doc(v)))
 
     if all_Class:
         stream.write('##### class\n')
         for k,v in all_Class:
             if dump_format is None:
-                stream.write('# %s[%s]\n' % (k, _val_doc(v)))
+                stream.write('  # %s[%s]\n' % (k, _val_doc(v)))
             else:
-                stream.write('%s #[%s]\n' % (k, _val_doc(v)))
+                stream.write('  %s #[%s]\n' % (k, _val_doc(v)))
 
     if all_Attr:
         stream.write('##### attr\n')
         for k,v in all_Attr:
             if dump_format is None or (k.startswith('__') and k.endswith('__')):
-                stream.write('# %s[%s] [%s]\n' % (k, _val_str(v), _val_doc(v)))
+                stream.write('  # %s[%s] [%s]\n' % (k, _val_str(v), _val_doc(v)))
             else:
-                stream.write('%s #[%s] [%s]\n' % (k, _val_str(v), _val_doc(v)))
+                stream.write('  %s #[%s] [%s]\n' % (k, _val_str(v), _val_doc(v)))
 
     if all_Funcs:
         stream.write('##### func\n')
         for k,v in all_Funcs:
             if dump_format is None:
-                stream.write('# %s%s [%s]\n' % (k, _func_signature(v), _val_doc(v)))
+                stream.write('  # %s%s [%s]\n' % (k, _func_signature(v), _val_doc(v)))
             else:
-                stream.write('%s #%s [%s]\n' % (k, _func_signature(v), _val_doc(v)))
+                stream.write('  %s #%s [%s]\n' % (k, _func_signature(v), _val_doc(v)))
     stream.write("\n")
 
 def _val_str(v):
     return str(v).replace('\n', ' ').replace('\r', ' ')[0:100]
 
 def _val_doc(v):
     if isinstance(v, str):
```

### Comparing `laok-0.2.17/laok/base/test/_run.py` & `laok-0.2.18/laok/base/test/_run.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/cv3d/io/_simple.py` & `laok-0.2.18/laok/cv3d/io/_simple.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/cv3d/show/vtk_/__init__.py` & `laok-0.2.18/laok/cv3d/show/vtk_/__init__.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/cv3d/show/vtk_/win.py` & `laok-0.2.18/laok/cv3d/show/vtk_/win.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/cv3d/trans/_dropout.py` & `laok-0.2.18/laok/cv3d/trans/_dropout.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/cv3d/trans/_jitter.py` & `laok-0.2.18/laok/cv3d/trans/_jitter.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/cv3d/trans/_normal.py` & `laok-0.2.18/laok/cv3d/trans/_normal.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/cv3d/trans/_rotate.py` & `laok-0.2.18/laok/cv3d/trans/_rotate.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/cv3d/trans/_sample.py` & `laok-0.2.18/laok/cv3d/trans/_sample.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/cv3d/trans/_scale.py` & `laok-0.2.18/laok/cv3d/trans/_scale.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/cv3d/trans/_translate.py` & `laok-0.2.18/laok/cv3d/trans/_translate.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/dnn/head/classify.py` & `laok-0.2.18/laok/dnn/head/classify.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/dnn/head/detect.py` & `laok-0.2.18/laok/dnn/head/detect.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/dnn/layer/pooling.py` & `laok-0.2.18/laok/dnn/layer/pooling.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/ext/flask_/basic/views.py` & `laok-0.2.18/laok/ext/flask_/basic/views.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/ext/onnx_.py` & `laok-0.2.18/laok/ext/onnx_.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/ext/torch_/datasets/kitti/kitti.py` & `laok-0.2.18/laok/ext/torch_/datasets/kitti/kitti.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/ext/torch_/datasets/kitti/obj.py` & `laok-0.2.18/laok/ext/torch_/datasets/kitti/obj.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/ext/torch_/datasets/kitti/utils.py` & `laok-0.2.18/laok/ext/torch_/datasets/kitti/utils.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/ext/torch_/datasets/model_net/__init__.py` & `laok-0.2.18/laok/ext/torch_/datasets/model_net/__init__.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/ext/torch_/datasets/model_net/model_net.py` & `laok-0.2.18/laok/ext/torch_/datasets/model_net/model_net.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/ext/torch_/datasets/model_net/model_net_ineratia.py` & `laok-0.2.18/laok/ext/torch_/datasets/model_net/model_net_ineratia.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/ext/torch_/datasets/model_net/model_net_normals.py` & `laok-0.2.18/laok/ext/torch_/datasets/model_net/model_net_normals.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/ext/torch_/datasets/model_net/model_net_normals_diff.py` & `laok-0.2.18/laok/ext/torch_/datasets/model_net/model_net_normals_diff.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/ext/torch_/datasets/shape_net/shape_net.py` & `laok-0.2.18/laok/ext/torch_/datasets/shape_net/shape_net.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/ext/torch_/datasets/stanford_indoor/_stanford_indoor.py` & `laok-0.2.18/laok/ext/torch_/datasets/stanford_indoor/_stanford_indoor.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/ext/torch_/datasets/ustc_lidar.py` & `laok-0.2.18/laok/ext/torch_/datasets/ustc_lidar.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/ext/torch_/io/img.py` & `laok-0.2.18/laok/ext/torch_/io/img.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/ext/torch_/io/jit.py` & `laok-0.2.18/laok/ext/torch_/io/jit.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/ext/torch_/io/model.py` & `laok-0.2.18/laok/ext/torch_/io/model.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/ext/torch_/op/device.py` & `laok-0.2.18/laok/ext/torch_/op/device.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/ext/torch_/op/module.py` & `laok-0.2.18/laok/ext/torch_/op/module.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/ext/torch_/op/print_info.py` & `laok-0.2.18/laok/ext/torch_/op/print_info.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/ext/torch_/trainval/check_point.py` & `laok-0.2.18/laok/ext/torch_/trainval/check_point.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/ext/torch_/trainval/infer.py` & `laok-0.2.18/laok/ext/torch_/trainval/infer.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/ext/torch_/trainval/train.py` & `laok-0.2.18/laok/ext/torch_/trainval/train.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/ext/torch_/trainval/val.py` & `laok-0.2.18/laok/ext/torch_/trainval/val.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.17/laok/tool/ultralytics_/train_det.py` & `laok-0.2.18/laok/ext/ultralytics_.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*-
 '''
 Created on 2023/5/4 20:27:02
 @author: LiuKuan
 @copyright: Apache License, Version 2.0
 '''
-import os, laok
+import laok
+from laok.cv2d.io import fix_cv_read
 from ultralytics import YOLO
 #===============================================================================
-r'''
+r'''支持 yolo训练的脚本
+需要 文件夹 root_dir下:
+                ---- xxx.pt
+                ---- xxx.names
+                ---- Image/
 '''
 #===============================================================================
-__all__ = ['train_det']
 
 def _gen_data(root_dir, filename = None):
-    root_dir = os.path.abspath(root_dir)
+    root_dir = laok.path_abs(root_dir)
     names_file = laok.path_search_cur_ext(root_dir, ".txt;.names")
     dataset = laok.Dict()
     dataset.path = laok.path_native(root_dir)
     dataset.train = 'Image'
     dataset.val = 'Image'
     dataset.test = ''
     dataset.names = list(laok.file_read_lines(names_file))
     if filename is None:
         filename = laok.path_replace_ext(names_file, ".yaml")
-    laok.save_yaml_file(filename, dataset, indent=4)
+    laok.save_yaml_file(filename, dataset, indent=4, encoding='utf8')
     return filename
 
-def train_det(root_dir=None, model_file=None, data_file=None, imgsz=(512, 1248), epochs=100, batch=16, **kwargs):
-    if root_dir is None:
-        root_dir = os.path.abspath(os.getcwd())
+def train_det(root_dir, model_file=None, data_file=None, imgsz=(512, 1248), epochs=100, batch=16, **kwargs):
     print(f'root_dir: {root_dir}')
 
     if model_file is None:
         model_file = laok.path_search_cur_ext(root_dir, ".pt")
     print(f'model_file: {model_file}')
 
+    fix_cv_read()
     with laok.work_dir_scope(root_dir):
         data_file = _gen_data(root_dir, data_file)
         print(f'data_file: {data_file}' )
 
         model = YOLO(model_file)  # load a pretrained model (recommended for training)
         kwargs['task'] = 'detect'
 
@@ -48,9 +51,12 @@
         kwargs.setdefault('save_crop', True)
         kwargs.setdefault('amp', False)
         if laok.is_windows():
             kwargs.setdefault('workers', 0)
         model.train(data=data_file, epochs=epochs, imgsz=imgsz, batch=batch, **kwargs)
         best_model = laok.path_search_under_file(model.trainer.save_dir, 'best.pt')
         model2 = YOLO(best_model)  # load a custom trained
-        model2.export(format='onnx', imgsz=imgsz)
+        model2.export(format='onnx', opset=12, dynamic = False, imgsz=imgsz)
 
+if __name__ == '__main__':
+    import fire as _fire
+    _fire.Fire(train_det)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `laok-0.2.17/laok.egg-info/SOURCES.txt` & `laok-0.2.18/laok.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,72 +1,97 @@
 setup.py
 laok/__init__.py
+laok/third_lib.py
 laok.egg-info/PKG-INFO
 laok.egg-info/SOURCES.txt
 laok.egg-info/dependency_links.txt
 laok.egg-info/top_level.txt
 laok/base/__init__.py
 laok/base/alg/__init__.py
 laok/base/alg/addict.py
 laok/base/conf/__init__.py
 laok/base/conf/conf_global.py
+laok/base/conf/factory.py
 laok/base/dataset/__init__.py
 laok/base/dataset/cvt_voc_yolo.py
 laok/base/dataset/darknet-voc2yolo.py
 laok/base/dataset/voc_label.py
 laok/base/dtime/__init__.py
 laok/base/dtime/datetime_.py
 laok/base/dtime/timer.py
 laok/base/fs/__init__.py
 laok/base/fs/fdata.py
 laok/base/fs/fname.py
 laok/base/fs/fpath.py
 laok/base/fs/fsearch.py
 laok/base/fs/fwalk.py
 laok/base/fs/name_index.py
-laok/base/func/__init__.py
-laok/base/func/print_info.py
 laok/base/log/__init__.py
 laok/base/log/log.py
 laok/base/log/log_default.py
 laok/base/net/__init__.py
 laok/base/net/ip.py
 laok/base/net/requests_.py
-laok/base/parallel/__init__.py
-laok/base/parallel/pool.py
+laok/base/net/url.py
+laok/base/paral/__init__.py
+laok/base/paral/pool.py
+laok/base/pkg/__init__.py
+laok/base/pkg/_lazy.py
 laok/base/ser/__init__.py
-laok/base/ser/_json.py
-laok/base/ser/_marshal.py
-laok/base/ser/_pickle.py
+laok/base/ser/json_.py
+laok/base/ser/marshal_.py
 laok/base/ser/numpy_.py
+laok/base/ser/pickle_.py
 laok/base/ser/torch_.py
+laok/base/ser/xml_.py
 laok/base/ser/yaml_.py
 laok/base/str/__init__.py
+laok/base/str/cvt.py
 laok/base/str/fmt.py
 laok/base/str/misc.py
 laok/base/str/print_info.py
-laok/base/sys_/__init__.py
-laok/base/sys_/platform_.py
+laok/base/syst/__init__.py
+laok/base/syst/platform_.py
+laok/base/syst/print_info.py
+laok/base/syst/sys_.py
 laok/base/test/__init__.py
 laok/base/test/_dump.py
 laok/base/test/_run.py
 laok/cv2d/__init__.py
+laok/cv2d/cvt/__init__.py
+laok/cv2d/cvt/cv2_.py
+laok/cv2d/cvt/misc_.py
+laok/cv2d/cvt/pil_.py
+laok/cv2d/cvt/sk_.py
+laok/cv2d/draw/__init__.py
+laok/cv2d/draw/color.py
+laok/cv2d/draw/cv2_.py
+laok/cv2d/io/__init__.py
+laok/cv2d/io/cv2_.py
+laok/cv2d/io/pil_.py
+laok/cv2d/morph/__init__.py
+laok/cv2d/morph/cv2_.py
+laok/cv2d/show/__init__.py
+laok/cv2d/show/cv2_.py
+laok/cv2d/show/pil_.py
+laok/cv2d/show/plt_.py
 laok/cv3d/__init__.py
 laok/cv3d/io/__init__.py
 laok/cv3d/io/_simple.py
 laok/cv3d/show/__init__.py
 laok/cv3d/show/vtk_/__init__.py
 laok/cv3d/show/vtk_/win.py
 laok/cv3d/trans/__init__.py
 laok/cv3d/trans/_dropout.py
 laok/cv3d/trans/_jitter.py
 laok/cv3d/trans/_normal.py
 laok/cv3d/trans/_rotate.py
 laok/cv3d/trans/_sample.py
 laok/cv3d/trans/_scale.py
+laok/cv3d/trans/_swap_filed.py
 laok/cv3d/trans/_torch.py
 laok/cv3d/trans/_translate.py
 laok/dnn/__init__.py
 laok/dnn/backbones/__init__.py
 laok/dnn/dataset/__init__.py
 laok/dnn/dataset/cld/__init__.py
 laok/dnn/dataset/img/__init__.py
@@ -75,17 +100,19 @@
 laok/dnn/head/classify.py
 laok/dnn/head/detect.py
 laok/dnn/layer/__init__.py
 laok/dnn/layer/pooling.py
 laok/dnn/loss/__init__.py
 laok/dnn/model/__init__.py
 laok/dnn/model/_torch_vision.py
+laok/dnn/model/arc_face.py
 laok/dnn/neck/__init__.py
 laok/ext/__init__.py
 laok/ext/onnx_.py
+laok/ext/ultralytics_.py
 laok/ext/flask_/__init__.py
 laok/ext/flask_/app.py
 laok/ext/flask_/basic/__init__.py
 laok/ext/flask_/basic/views.py
 laok/ext/numpy_/__init__.py
 laok/ext/torch_/__init__.py
 laok/ext/torch_/datasets/__init__.py
@@ -112,13 +139,8 @@
 laok/ext/torch_/op/device.py
 laok/ext/torch_/op/module.py
 laok/ext/torch_/op/print_info.py
 laok/ext/torch_/trainval/__init__.py
 laok/ext/torch_/trainval/check_point.py
 laok/ext/torch_/trainval/infer.py
 laok/ext/torch_/trainval/train.py
-laok/ext/torch_/trainval/val.py
-laok/ml/__init__.py
-laok/tool/__init__.py
-laok/tool/ultralytics_/__init__.py
-laok/tool/ultralytics_/__main__.py
-laok/tool/ultralytics_/train_det.py
+laok/ext/torch_/trainval/val.py
```

