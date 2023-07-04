# Comparing `tmp/drillvision-0.1.0.tar.gz` & `tmp/drillvision-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drillvision-0.1.0.tar", last modified: Fri Jun 30 15:15:10 2023, max compression
+gzip compressed data, was "drillvision-0.1.1.tar", last modified: Tue Jul  4 13:11:03 2023, max compression
```

## Comparing `drillvision-0.1.0.tar` & `drillvision-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:15:10.163065 drillvision-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-30 15:13:18.000000 drillvision-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-06-30 15:15:10.163065 drillvision-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-06-30 15:13:18.000000 drillvision-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:15:10.159064 drillvision-0.1.0/drillvision.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-06-30 15:15:10.000000 drillvision-0.1.0/drillvision.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-30 15:15:10.000000 drillvision-0.1.0/drillvision.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 15:15:10.000000 drillvision-0.1.0/drillvision.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-30 15:15:10.000000 drillvision-0.1.0/drillvision.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-30 15:15:10.000000 drillvision-0.1.0/drillvision.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:15:10.159064 drillvision-0.1.0/neural_network_model/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-30 15:13:18.000000 drillvision-0.1.0/neural_network_model/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:13:18.000000 drillvision-0.1.0/neural_network_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29087 2023-06-30 15:13:18.000000 drillvision-0.1.0/neural_network_model/bit_vision.py
--rw-r--r--   0 runner    (1001) docker     (123)    62009 2023-06-30 15:13:18.000000 drillvision-0.1.0/neural_network_model/cam.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     7698 2023-06-30 15:13:18.000000 drillvision-0.1.0/neural_network_model/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    15052 2023-06-30 15:13:18.000000 drillvision-0.1.0/neural_network_model/process_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-30 15:13:18.000000 drillvision-0.1.0/neural_network_model/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-30 15:13:18.000000 drillvision-0.1.0/neural_network_model/script_run_all.py
--rw-r--r--   0 runner    (1001) docker     (123)    30130 2023-06-30 15:13:18.000000 drillvision-0.1.0/neural_network_model/transfer_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-30 15:13:18.000000 drillvision-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-30 15:13:18.000000 drillvision-0.1.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-30 15:13:18.000000 drillvision-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 15:15:10.163065 drillvision-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-30 15:13:18.000000 drillvision-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:11:02.997164 drillvision-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-04 13:09:15.000000 drillvision-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8694 2023-07-04 13:11:02.997164 drillvision-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-07-04 13:09:15.000000 drillvision-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:11:02.997164 drillvision-0.1.1/drillvision.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8694 2023-07-04 13:11:02.000000 drillvision-0.1.1/drillvision.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-04 13:11:02.000000 drillvision-0.1.1/drillvision.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 13:11:02.000000 drillvision-0.1.1/drillvision.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-04 13:11:02.000000 drillvision-0.1.1/drillvision.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-04 13:11:02.000000 drillvision-0.1.1/drillvision.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:11:02.997164 drillvision-0.1.1/neural_network_model/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-04 13:09:15.000000 drillvision-0.1.1/neural_network_model/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:09:15.000000 drillvision-0.1.1/neural_network_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29087 2023-07-04 13:09:15.000000 drillvision-0.1.1/neural_network_model/bit_vision.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62009 2023-07-04 13:09:15.000000 drillvision-0.1.1/neural_network_model/cam.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-07-04 13:09:15.000000 drillvision-0.1.1/neural_network_model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15052 2023-07-04 13:09:15.000000 drillvision-0.1.1/neural_network_model/process_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-07-04 13:09:15.000000 drillvision-0.1.1/neural_network_model/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-04 13:09:15.000000 drillvision-0.1.1/neural_network_model/script_run_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30943 2023-07-04 13:09:15.000000 drillvision-0.1.1/neural_network_model/transfer_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-07-04 13:09:15.000000 drillvision-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-04 13:09:15.000000 drillvision-0.1.1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-04 13:09:15.000000 drillvision-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 13:11:02.997164 drillvision-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-04 13:09:15.000000 drillvision-0.1.1/setup.py
```

### Comparing `drillvision-0.1.0/PKG-INFO` & `drillvision-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drillvision
-Version: 0.1.0
+Version: 0.1.1
 Summary: DrillBitVision
 Home-page: https://github.com/Atashnezhad/DrillBitVision
 Author: Amin Atashnezhad
 Author-email: atashnezhad2@gmail.com
 License: BSD-3
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -12,16 +12,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 
 # Drill Bit Classifier
 
 [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-360/)
-[![Downloads](https://static.pepy.tech/personalized-badge/drillvision?period=total&units=international_system&left_color=grey&right_color=red&left_text=Downloads)](https://pepy.tech/project/drillvision)
 ![GitHub CI](https://github.com/Atashnezhad/DrillBitVision/actions/workflows/main.yml/badge.svg)
+[![Downloads](https://static.pepy.tech/badge/drillvision)](https://pepy.tech/project/drillvision)
 
 The Drill Bit Classifier is an app that uses a Convolutional Neural Network (CNN) to 
 classify images of drill bits. The app can be used by machinists and engineers to 
 quickly and accurately identify the type of drill bit required for a particular job.
 
 ## Description:
 ### Preprocessing Module
@@ -166,15 +166,15 @@
 from pathlib import Path
 
 
 transfer_model = TransferModel(
         dataset_address=Path(__file__).parent / "dataset"
     )
 
-transfer_model.plot_classes_number()
+transfer_model.plot_classes_number(figure_folder_path=Path(__file__).parent / "figures")
 transfer_model.analyze_image_names()
 transfer_model.plot_data_images(num_rows=3, num_cols=3)
 transfer_model.train_model()
 transfer_model.plot_metrics_results()
 transfer_model.results()
 transfer_model.predcit_test()
 transfer_model.grad_cam_viz(num_rows=3, num_cols=2)
```

### Comparing `drillvision-0.1.0/README.md` & `drillvision-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Drill Bit Classifier
 
 [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-360/)
-[![Downloads](https://static.pepy.tech/personalized-badge/drillvision?period=total&units=international_system&left_color=grey&right_color=red&left_text=Downloads)](https://pepy.tech/project/drillvision)
 ![GitHub CI](https://github.com/Atashnezhad/DrillBitVision/actions/workflows/main.yml/badge.svg)
+[![Downloads](https://static.pepy.tech/badge/drillvision)](https://pepy.tech/project/drillvision)
 
 The Drill Bit Classifier is an app that uses a Convolutional Neural Network (CNN) to 
 classify images of drill bits. The app can be used by machinists and engineers to 
 quickly and accurately identify the type of drill bit required for a particular job.
 
 ## Description:
 ### Preprocessing Module
@@ -151,15 +151,15 @@
 from pathlib import Path
 
 
 transfer_model = TransferModel(
         dataset_address=Path(__file__).parent / "dataset"
     )
 
-transfer_model.plot_classes_number()
+transfer_model.plot_classes_number(figure_folder_path=Path(__file__).parent / "figures")
 transfer_model.analyze_image_names()
 transfer_model.plot_data_images(num_rows=3, num_cols=3)
 transfer_model.train_model()
 transfer_model.plot_metrics_results()
 transfer_model.results()
 transfer_model.predcit_test()
 transfer_model.grad_cam_viz(num_rows=3, num_cols=2)
```

### Comparing `drillvision-0.1.0/drillvision.egg-info/PKG-INFO` & `drillvision-0.1.1/drillvision.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drillvision
-Version: 0.1.0
+Version: 0.1.1
 Summary: DrillBitVision
 Home-page: https://github.com/Atashnezhad/DrillBitVision
 Author: Amin Atashnezhad
 Author-email: atashnezhad2@gmail.com
 License: BSD-3
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -12,16 +12,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 
 # Drill Bit Classifier
 
 [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-360/)
-[![Downloads](https://static.pepy.tech/personalized-badge/drillvision?period=total&units=international_system&left_color=grey&right_color=red&left_text=Downloads)](https://pepy.tech/project/drillvision)
 ![GitHub CI](https://github.com/Atashnezhad/DrillBitVision/actions/workflows/main.yml/badge.svg)
+[![Downloads](https://static.pepy.tech/badge/drillvision)](https://pepy.tech/project/drillvision)
 
 The Drill Bit Classifier is an app that uses a Convolutional Neural Network (CNN) to 
 classify images of drill bits. The app can be used by machinists and engineers to 
 quickly and accurately identify the type of drill bit required for a particular job.
 
 ## Description:
 ### Preprocessing Module
@@ -166,15 +166,15 @@
 from pathlib import Path
 
 
 transfer_model = TransferModel(
         dataset_address=Path(__file__).parent / "dataset"
     )
 
-transfer_model.plot_classes_number()
+transfer_model.plot_classes_number(figure_folder_path=Path(__file__).parent / "figures")
 transfer_model.analyze_image_names()
 transfer_model.plot_data_images(num_rows=3, num_cols=3)
 transfer_model.train_model()
 transfer_model.plot_metrics_results()
 transfer_model.results()
 transfer_model.predcit_test()
 transfer_model.grad_cam_viz(num_rows=3, num_cols=2)
```

### Comparing `drillvision-0.1.0/drillvision.egg-info/SOURCES.txt` & `drillvision-0.1.1/drillvision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drillvision-0.1.0/neural_network_model/bit_vision.py` & `drillvision-0.1.1/neural_network_model/bit_vision.py`

 * *Files identical despite different names*

### Comparing `drillvision-0.1.0/neural_network_model/cam.jpg` & `drillvision-0.1.1/neural_network_model/cam.jpg`

 * *Files identical despite different names*

### Comparing `drillvision-0.1.0/neural_network_model/model.py` & `drillvision-0.1.1/neural_network_model/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -225,14 +225,17 @@
     TRAIN_SIZE: float = 0.9
     SHUFFLE: bool = True
     RANDOM_STATE: int = 1
 
     # training
     VALIDATION_SPLIT: float = 0.1
 
+    # model save location
+    MODEL_SAVE_LOCATION: str = (Path(__file__).parent / ".." / "deep_model").resolve()
+
     # MobileNetV2 network details
     WEIGHTS: str = "imagenet"
     POOLING: str = "avg"
     INCLUDE_TOP: bool = False
 
     DENSE_LAYER_ACTIVATION: str = "relu"
```

### Comparing `drillvision-0.1.0/neural_network_model/process_data.py` & `drillvision-0.1.1/neural_network_model/process_data.py`

 * *Files identical despite different names*

### Comparing `drillvision-0.1.0/neural_network_model/s3.py` & `drillvision-0.1.1/neural_network_model/s3.py`

 * *Files identical despite different names*

### Comparing `drillvision-0.1.0/neural_network_model/script_run_all.py` & `drillvision-0.1.1/neural_network_model/script_run_all.py`

 * *Files identical despite different names*

### Comparing `drillvision-0.1.0/neural_network_model/transfer_learning.py` & `drillvision-0.1.1/neural_network_model/transfer_learning.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,28 +30,29 @@
 logger.setLevel(logging.INFO)
 
 
 class TransferModel(Preprocessing, BitVision):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
+        self.model_save_path: str = TRANSFER_LEARNING_SETTING.MODEL_SAVE_LOCATION
         self.image_df: pd.DataFrame = None
 
         self._prepare_data()
 
         self.model: tf.keras.Model = None
         self.model_history: tf.keras.callbacks.History = None
 
         self.pred: np.ndarray = None
 
     def _prepare_data(
-        self,
-        print_data_head=False,
-        x_col=TRANSFER_LEARNING_SETTING.DF_X_COL_NAME,
-        y_col=TRANSFER_LEARNING_SETTING.DF_Y_COL_NAME,
+            self,
+            print_data_head=False,
+            x_col=TRANSFER_LEARNING_SETTING.DF_X_COL_NAME,
+            y_col=TRANSFER_LEARNING_SETTING.DF_Y_COL_NAME,
     ):
         """
         Prepare the data for the model
         :param print_data_head: print the head of the data
         :param x_col: column name for the filepaths
         :param y_col: column name for the labels
         :return: None
@@ -75,19 +76,19 @@
         self.image_df = image_df
         if print_data_head:
             print(self.image_df.head(3))
         # log the data was prepared
         logging.info("Data was prepared")
 
     def plot_classes_number(
-        self,
-        figsize=(10, 5),
-        x_rotation=0,
-        palette="Greens_r",
-        **kwargs,
+            self,
+            figsize=(10, 5),
+            x_rotation=0,
+            palette="Greens_r",
+            **kwargs,
     ) -> None:
         """
         Plot the number of images per species
         :param figsize: size of the figure
         :param x_rotation: rotation of the x-axis
         :param palette: color palette
         :param kwargs: figure_folder_path
@@ -123,22 +124,22 @@
         plt.title("How many images per classes are given in the data?")
         plt.tight_layout()
         # save the plot in the figures folder
         plt.savefig(figure_folder_path / "classes_number.png")
         plt.show()
 
     def analyze_image_names(
-        self,
-        figsize=(20, 22),
-        figsize_2=(10, 7),
-        cmap_2="YlGnBu",
-        size=15,
-        label_size=25,
-        num_cluster=5,
-        **kwargs,
+            self,
+            figsize=(20, 22),
+            figsize_2=(10, 7),
+            cmap_2="YlGnBu",
+            size=15,
+            label_size=25,
+            num_cluster=5,
+            **kwargs,
     ) -> None:
         """
         Analyze the image names if there is any pattern in the names
         :param figsize: size of the figure
         :param figsize_2: size of the second figure
         :param cmap_2: color map of the second figure
         :param size: size of the scatter points
@@ -255,15 +256,15 @@
         )
         plt.tight_layout()
         # save the plot in the figures folder
         plt.savefig(figure_folder_path / "cluster_number_per_class.png")
         plt.show()
 
     def plot_data_images(
-        self, num_rows=None, num_cols=None, figsize=(15, 10), **kwargs
+            self, num_rows=None, num_cols=None, figsize=(15, 10), **kwargs
     ):
         """
         Plot the images in a grid
         :param num_rows: number of rows in the grid
         :param num_cols: number of columns in the grid
         :param figsize: size of the figure
         :param kwargs: figure_folder_path
@@ -461,21 +462,25 @@
             train_generator,
             test_generator,
             train_images,
             val_images,
             test_images,
         )
 
-    def train_model(self, epochs=10, batch_size=32):
+    def train_model(self, epochs=10, batch_size=32, **kwargs):
         """
         Train the model
-        :param num_categories: number of categories in the dataset
         :param epochs: number of epochs
         :param batch_size: batch size
+        kwargs:
+            model_save_location: location to save the model default is self.model_save_location
         """
+        if kwargs.get("model_save_location"):
+            self.model_save_path = kwargs.get("model_save_path")
+        model_name = kwargs.get("model_name", "tf_model.h5")
 
         # check number of subfolders in the self.image_df
         folder_path = self.dataset_address  # Replace with the path to your folder
         # Create a Path object for the specified folder
         folder = Path(folder_path)
         # Count the number of subfolders
         num_categories = sum(item.is_dir() for item in folder.iterdir())
@@ -529,15 +534,16 @@
                     restore_best_weights=restore_best_weights,
                 )
             ],
         )
         self.model = model
         self.model_history = history
         # save the model
-        self.model.save(self.model_address)
+        self.model_save_path = os.path.join(self.model_save_path, model_name)
+        self.model.save(self.model_save_path)
 
     def plot_metrics_results(self, **kwargs):
         figure_folder_path = kwargs.get(
             "figure_folder_path", Path(__file__).parent / ".." / "figures"
         )
         # check if the folder exists if not create it
         if not figure_folder_path.exists():
@@ -585,26 +591,33 @@
         TransferModel.printmd(
             "## Accuracy on the test set: {:.2f}%".format(results[1] * 100)
         )
 
         print(" ## Test Loss: {:.5f}".format(results[0]))
         print("## Accuracy on the test set: {:.2f}%".format(results[1] * 100))
 
-    def predcit_test(self, **kwargs):
+    def predcit_test(self, model_path: str = None, **kwargs):
         (
             train_generator,
             test_generator,
             train_images,
             val_images,
             test_images,
         ) = self._create_gen()
 
         figure_folder_path = kwargs.get(
             "figure_folder_path", Path(__file__).parent / ".." / "figures"
         )
+
+        # Load the model
+        # here we check if the model_path path is provided and load it otherwise we use the self.model
+        # which is the model trained in the train method in the memory
+        if model_path is not None:
+            self.model = tf.keras.models.load_model(model_path)
+
         # check if the folder exists if not create it
         if not figure_folder_path.exists():
             os.makedirs(figure_folder_path)
 
         # Predict the label of the test_images
         pred = self.model.predict(test_images)
         pred = np.argmax(pred, axis=1)
@@ -640,15 +653,15 @@
         array = tf.keras.preprocessing.image.img_to_array(img)
         # We add a dimension to transform our array into a "batch"
         # of size "size"
         array = np.expand_dims(array, axis=0)
         return array
 
     def _make_gradcam_heatmap(
-        self, img_array, model, last_conv_layer_name, pred_index=None
+            self, img_array, model, last_conv_layer_name, pred_index=None
     ):
         # First, we create a model that maps the input image to the activations
         # of the last conv layer as well as the output predictions
         grad_model = tf.keras.models.Model(
             [model.inputs], [model.get_layer(last_conv_layer_name).output, model.output]
         )
 
@@ -676,20 +689,20 @@
         heatmap = tf.squeeze(heatmap)
 
         # For visualization purpose, we will also normalize the heatmap between 0 & 1
         heatmap = tf.maximum(heatmap, 0) / tf.math.reduce_max(heatmap)
         return heatmap.numpy()
 
     def _save_and_display_gradcam(
-        self,
-        img_path,
-        heatmap,
-        cam_name="transf_cam.jpg",
-        alpha=0.4,
-        **kwargs,
+            self,
+            img_path,
+            heatmap,
+            cam_name="transf_cam.jpg",
+            alpha=0.4,
+            **kwargs,
     ):
         """
         Args:
             img_path: path to our image
             heatmap: the heatmap of our image
         Keyword Args:
             cam_name: name of the cam (default: transf_cam.jpg)
```

### Comparing `drillvision-0.1.0/pyproject.toml` & `drillvision-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `drillvision-0.1.0/setup.py` & `drillvision-0.1.1/setup.py`

 * *Files identical despite different names*

