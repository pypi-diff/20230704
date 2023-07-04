# Comparing `tmp/pysiml-0.2.9.dev202306270535-py3-none-any.whl.zip` & `tmp/pysiml-0.2.9.dev202307040514-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 173407 bytes, number of entries: 142
+Zip file size: 178872 bytes, number of entries: 147
 -rw-r--r--  2.0 unx     1520 b- defN 80-Jan-01 00:00 pyproject.toml
 -rw-r--r--  2.0 unx      638 b- defN 80-Jan-01 00:00 siml/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 siml/__main__/__init__.py
 -rw-r--r--  2.0 unx      900 b- defN 80-Jan-01 00:00 siml/__main__/convert_interim_data.py
 -rw-r--r--  2.0 unx     1400 b- defN 80-Jan-01 00:00 siml/__main__/convert_raw_data.py
 -rw-r--r--  2.0 unx     1742 b- defN 80-Jan-01 00:00 siml/__main__/optimize.py
 -rw-r--r--  2.0 unx     8663 b- defN 80-Jan-01 00:00 siml/__main__/plot_losses.py
@@ -98,47 +98,52 @@
 -rw-r--r--  2.0 unx     1012 b- defN 80-Jan-01 00:00 siml/preprocessing/siml_scalers/scaler_result_save.py
 -rw-r--r--  2.0 unx     4367 b- defN 80-Jan-01 00:00 siml/preprocessing/siml_scalers/scaler_wrapper.py
 -rw-r--r--  2.0 unx      154 b- defN 80-Jan-01 00:00 siml/services/__init__.py
 -rw-r--r--  2.0 unx     2342 b- defN 80-Jan-01 00:00 siml/services/environment.py
 -rw-r--r--  2.0 unx      279 b- defN 80-Jan-01 00:00 siml/services/inference/__init__.py
 -rw-r--r--  2.0 unx     2587 b- defN 80-Jan-01 00:00 siml/services/inference/core_inferer.py
 -rw-r--r--  2.0 unx     1818 b- defN 80-Jan-01 00:00 siml/services/inference/data_loader_builder.py
--rw-r--r--  2.0 unx     2619 b- defN 80-Jan-01 00:00 siml/services/inference/engine_bulider.py
+-rw-r--r--  2.0 unx     2619 b- defN 80-Jan-01 00:00 siml/services/inference/engine_builder.py
 -rw-r--r--  2.0 unx     5750 b- defN 80-Jan-01 00:00 siml/services/inference/inner_setting.py
 -rw-r--r--  2.0 unx     4710 b- defN 80-Jan-01 00:00 siml/services/inference/metrics_builder.py
 -rw-r--r--  2.0 unx      203 b- defN 80-Jan-01 00:00 siml/services/inference/postprocessing/__init__.py
 -rw-r--r--  2.0 unx     5603 b- defN 80-Jan-01 00:00 siml/services/inference/postprocessing/post_fem_data.py
 -rw-r--r--  2.0 unx     4979 b- defN 80-Jan-01 00:00 siml/services/inference/postprocessing/postprocessor.py
 -rw-r--r--  2.0 unx     7052 b- defN 80-Jan-01 00:00 siml/services/inference/postprocessing/save_processor.py
 -rw-r--r--  2.0 unx     1082 b- defN 80-Jan-01 00:00 siml/services/inference/record_object.py
--rw-r--r--  2.0 unx     2634 b- defN 80-Jan-01 00:00 siml/services/model_builder.py
+-rw-r--r--  2.0 unx     3161 b- defN 80-Jan-01 00:00 siml/services/model_builder.py
 -rw-r--r--  2.0 unx     4978 b- defN 80-Jan-01 00:00 siml/services/model_selector.py
 -rw-r--r--  2.0 unx     7124 b- defN 80-Jan-01 00:00 siml/services/path_rules.py
 -rw-r--r--  2.0 unx      200 b- defN 80-Jan-01 00:00 siml/services/training/__init__.py
--rw-r--r--  2.0 unx     2653 b- defN 80-Jan-01 00:00 siml/services/training/inner_settings.py
+-rw-r--r--  2.0 unx     7389 b- defN 80-Jan-01 00:00 siml/services/training/data_loader_builder.py
+-rw-r--r--  2.0 unx     7993 b- defN 80-Jan-01 00:00 siml/services/training/engine_builder.py
+-rw-r--r--  2.0 unx     7134 b- defN 80-Jan-01 00:00 siml/services/training/events_assigners.py
+-rw-r--r--  2.0 unx     3084 b- defN 80-Jan-01 00:00 siml/services/training/inner_settings.py
 -rw-r--r--  2.0 unx      775 b- defN 80-Jan-01 00:00 siml/services/training/logging_items/__init__.py
 -rw-r--r--  2.0 unx     4198 b- defN 80-Jan-01 00:00 siml/services/training/logging_items/logging_items.py
--rw-r--r--  2.0 unx     5695 b- defN 80-Jan-01 00:00 siml/services/training/training_logger.py
--rw-r--r--  2.0 unx    50394 b- defN 80-Jan-01 00:00 siml/setting.py
+-rw-r--r--  2.0 unx     2729 b- defN 80-Jan-01 00:00 siml/services/training/tensor_spliter.py
+-rw-r--r--  2.0 unx     9217 b- defN 80-Jan-01 00:00 siml/services/training/trainers_builder.py
+-rw-r--r--  2.0 unx     6633 b- defN 80-Jan-01 00:00 siml/services/training/training_logger.py
+-rw-r--r--  2.0 unx    52787 b- defN 80-Jan-01 00:00 siml/setting.py
 -rw-r--r--  2.0 unx      163 b- defN 80-Jan-01 00:00 siml/siml_variables/__init__.py
 -rw-r--r--  2.0 unx      594 b- defN 80-Jan-01 00:00 siml/siml_variables/array_variables/__init__.py
 -rw-r--r--  2.0 unx     1573 b- defN 80-Jan-01 00:00 siml/siml_variables/array_variables/interface_wrapper.py
 -rw-r--r--  2.0 unx     1398 b- defN 80-Jan-01 00:00 siml/siml_variables/array_variables/ndarray_wrapper.py
 -rw-r--r--  2.0 unx     1809 b- defN 80-Jan-01 00:00 siml/siml_variables/array_variables/sparce_array_wrapper.py
 -rw-r--r--  2.0 unx     4156 b- defN 80-Jan-01 00:00 siml/siml_variables/tensor_variables/tensor_variables.py
 -rw-r--r--  2.0 unx    12967 b- defN 80-Jan-01 00:00 siml/study.py
--rw-r--r--  2.0 unx    33627 b- defN 80-Jan-01 00:00 siml/trainer.py
+-rw-r--r--  2.0 unx    10653 b- defN 80-Jan-01 00:00 siml/trainer.py
 -rw-r--r--  2.0 unx      211 b- defN 80-Jan-01 00:00 siml/update_functions/__init__.py
 -rw-r--r--  2.0 unx     1774 b- defN 80-Jan-01 00:00 siml/update_functions/element_batch_update.py
 -rw-r--r--  2.0 unx     3623 b- defN 80-Jan-01 00:00 siml/update_functions/pseudo_batch_update.py
 -rw-r--r--  2.0 unx     2702 b- defN 80-Jan-01 00:00 siml/update_functions/standard_update.py
 -rw-r--r--  2.0 unx      429 b- defN 80-Jan-01 00:00 siml/update_functions/update_interface.py
 -rw-r--r--  2.0 unx    23027 b- defN 80-Jan-01 00:00 siml/util.py
 -rw-r--r--  2.0 unx       37 b- defN 80-Jan-01 00:00 siml/utils/__init__.py
 -rw-r--r--  2.0 unx     7682 b- defN 80-Jan-01 00:00 siml/utils/fem_data_utils.py
 -rw-r--r--  2.0 unx     1247 b- defN 80-Jan-01 00:00 siml/utils/timer.py
--rw-r--r--  2.0 unx    11431 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202306270535.dist-info/LICENSE
--rw-r--r--  2.0 unx     1638 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202306270535.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202306270535.dist-info/WHEEL
--rw-r--r--  2.0 unx      388 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202306270535.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx    12969 b- defN 16-Jan-01 00:00 pysiml-0.2.9.dev202306270535.dist-info/RECORD
-142 files, 610884 bytes uncompressed, 152675 bytes compressed:  75.0%
+-rw-r--r--  2.0 unx    11431 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202307040514.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1638 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202307040514.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202307040514.dist-info/WHEEL
+-rw-r--r--  2.0 unx      388 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202307040514.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx    13463 b- defN 16-Jan-01 00:00 pysiml-0.2.9.dev202307040514.dist-info/RECORD
+147 files, 627155 bytes uncompressed, 157342 bytes compressed:  74.9%
```

## zipnote {}

```diff
@@ -303,15 +303,15 @@
 
 Filename: siml/services/inference/core_inferer.py
 Comment: 
 
 Filename: siml/services/inference/data_loader_builder.py
 Comment: 
 
-Filename: siml/services/inference/engine_bulider.py
+Filename: siml/services/inference/engine_builder.py
 Comment: 
 
 Filename: siml/services/inference/inner_setting.py
 Comment: 
 
 Filename: siml/services/inference/metrics_builder.py
 Comment: 
@@ -339,23 +339,38 @@
 
 Filename: siml/services/path_rules.py
 Comment: 
 
 Filename: siml/services/training/__init__.py
 Comment: 
 
+Filename: siml/services/training/data_loader_builder.py
+Comment: 
+
+Filename: siml/services/training/engine_builder.py
+Comment: 
+
+Filename: siml/services/training/events_assigners.py
+Comment: 
+
 Filename: siml/services/training/inner_settings.py
 Comment: 
 
 Filename: siml/services/training/logging_items/__init__.py
 Comment: 
 
 Filename: siml/services/training/logging_items/logging_items.py
 Comment: 
 
+Filename: siml/services/training/tensor_spliter.py
+Comment: 
+
+Filename: siml/services/training/trainers_builder.py
+Comment: 
+
 Filename: siml/services/training/training_logger.py
 Comment: 
 
 Filename: siml/setting.py
 Comment: 
 
 Filename: siml/siml_variables/__init__.py
@@ -405,23 +420,23 @@
 
 Filename: siml/utils/fem_data_utils.py
 Comment: 
 
 Filename: siml/utils/timer.py
 Comment: 
 
-Filename: pysiml-0.2.9.dev202306270535.dist-info/LICENSE
+Filename: pysiml-0.2.9.dev202307040514.dist-info/LICENSE
 Comment: 
 
-Filename: pysiml-0.2.9.dev202306270535.dist-info/METADATA
+Filename: pysiml-0.2.9.dev202307040514.dist-info/METADATA
 Comment: 
 
-Filename: pysiml-0.2.9.dev202306270535.dist-info/WHEEL
+Filename: pysiml-0.2.9.dev202307040514.dist-info/WHEEL
 Comment: 
 
-Filename: pysiml-0.2.9.dev202306270535.dist-info/entry_points.txt
+Filename: pysiml-0.2.9.dev202307040514.dist-info/entry_points.txt
 Comment: 
 
-Filename: pysiml-0.2.9.dev202306270535.dist-info/RECORD
+Filename: pysiml-0.2.9.dev202307040514.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyproject.toml

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysiml"
-version = "0.2.9.dev202306270535"
+version = "0.2.9.dev202307040514"
 description = "SiML - a Simulation ML library"
 license = "Apache-2.0"
 authors = ["RICOS Co. Ltd."]
 readme = "README.md"
 repository = "https://github.com/ricosjp/pysiml"
 documentation = "https://ricosjp.github.io/pysiml/"
 packages = [
```

## siml/services/inference/core_inferer.py

```diff
@@ -5,15 +5,15 @@
 from torch.utils.data import DataLoader
 
 from siml import networks, setting
 from siml.inferer import ModelEnvironmentSetting
 from siml.loss_operations import ILossCalculator
 from siml.services.model_builder import ModelBuilder
 
-from .engine_bulider import InferenceEngineBuilder
+from .engine_builder import InferenceEngineBuilder
 from .metrics_builder import MetricsBuilder
 from .postprocessing import PostProcessor
 
 
 class CoreInferer():
     def __init__(
         self,
```

## siml/services/model_builder.py

```diff
@@ -19,27 +19,48 @@
         self._env_setting = env_setting
 
     @property
     def state_dict_strict(self) -> bool:
         return self._trainer_setting.state_dict_strict
 
     def create_initialized(self) -> networks.Network:
+        """Create initialized network object
+
+        Returns
+        -------
+        networks.Network
+            network object
+        """
         model = networks.Network(self._model_setting, self._trainer_setting)
         if self._env_setting.data_parallel:
             model = data_parallel.DataParallel(model)
 
         device = self._env_setting.get_device()
         model.to(device)
         return model
 
     def create_loaded(
         self,
         checkpoint_file: pathlib.Path,
         decrypt_key: Optional[bytes] = None
-    ):
+    ) -> networks.Network:
+        """Create network object loaded from checkpoint file
+
+        Parameters
+        ----------
+        checkpoint_file : pathlib.Path
+            Path to checkpoint file
+        decrypt_key : Optional[bytes], optional
+            decrpt byte key, by default None
+
+        Returns
+        -------
+        networks.Network
+            network object
+        """
         siml_file = SimlFileBuilder.checkpoint_file(checkpoint_file)
         print(f"Load snapshot file: {siml_file.file_path}")
 
         model = self.create_initialized()
         model_state_dict = self._load_model_state_dict(
             siml_file, model=model, decrypt_key=decrypt_key
         )
```

## siml/services/training/inner_settings.py

```diff
@@ -1,28 +1,39 @@
 from typing import Any, Union
 
+import pydantic
 import pydantic.dataclasses as dc
 
 from siml.path_like_objects import SimlDirectory
 from siml.setting import MainSetting, TrainerSetting
 
 
 # HACK
 # In the future, this setting is merged to setting.TrainerSetting
 @dc.dataclass(init=True)
 class InnerTrainingSetting:
     # HACK: To Avoid recursive validation by pydantic, Any type is used.
-    main_settings: Union[MainSetting, Any]
+    main_setting: Union[MainSetting, Any]
 
     class Config:
         arbitrary_types_allowed = True
 
+    @pydantic.root_validator
+    def _check_not_empty_variables_names(cls, values):
+        # HACK: Check in the training settings
+        main_setting: MainSetting = values["main_setting"]
+        if len(main_setting.trainer.input_names) == 0:
+            raise ValueError('No input_names fed')
+        if len(main_setting.trainer.output_names) == 0:
+            raise ValueError('No output_names fed')
+        return values
+
     @property
     def trainer_setting(self) -> TrainerSetting:
-        return self.main_settings.trainer
+        return self.main_setting.trainer
 
     @property
     def log_file_path(self):
         return self.trainer_setting.output_directory / 'log.csv'
 
     @property
     def loss_figure_path(self):
@@ -42,31 +53,31 @@
                 'at the same time.'
                 'pretrain_directory: '
                 f'{self.trainer_setting.pretrain_directory},'
                 f'restart directory: {self.trainer_setting.restart_directory}'
             )
 
     def _load_restart_settings(self, only_model: bool = False) -> None:
-        key = self.main_settings.get_crypt_key()
+        key = self.main_setting.get_crypt_key()
         restart_directory = self.trainer_setting.restart_directory
         output_directory = self.trainer_setting.output_directory
 
-        siml_dir = SimlDirectory(self.main_settings.trainer.restart_directory)
+        siml_dir = SimlDirectory(self.main_setting.trainer.restart_directory)
         restart_setting = MainSetting.read_settings_yaml(
             settings_yaml=siml_dir.find_yaml_file("settings").file_path,
             decrypt_key=key
         )
         if only_model:
-            self.main_settings.model = restart_setting.model
+            self.main_setting.model = restart_setting.model
         else:
-            self.main_settings = restart_setting
+            self.main_setting = restart_setting
 
         # Overwrite
         # Copy only output_direcoty and crypt key
-        self.main_settings.trainer.output_directory = output_directory
-        self.main_settings.trainer.model_key = key
-        self.main_settings.data.encrypt_key = key
-        self.main_settings.inferer.model_key = key
+        self.main_setting.trainer.output_directory = output_directory
+        self.main_setting.trainer.model_key = key
+        self.main_setting.data.encrypt_key = key
+        self.main_setting.inferer.model_key = key
 
         # restart
-        self.main_settings.trainer.restart_directory = restart_directory
-        self.main_settings.trainer.pretrain_directory = None
+        self.main_setting.trainer.restart_directory = restart_directory
+        self.main_setting.trainer.pretrain_directory = None
```

## siml/services/training/training_logger.py

```diff
@@ -1,13 +1,17 @@
 import pathlib
 
 import matplotlib.pyplot as plt
 import pandas as pd
+from torch.optim import Optimizer
 
+from siml.networks import Network
+from siml.path_like_objects import SimlFileBuilder
 from siml.services.training.logging_items import ILoggingItem, create_logitems
+from siml.setting import TrainerSetting
 
 
 class LogRecordItems:
     def __init__(
         self,
         *,
         epoch: int,
@@ -57,15 +61,15 @@
         return headers
 
     def output_header(self) -> str:
         strings = [
             v.format(padding_margin=self._display_margin)
             for v in self._headers
         ]
-        return "".join(strings)
+        return "\n" + "".join(strings)
 
     def output(self, log_record: LogRecordItems) -> str:
         strings = [
             log_record.epoch.format(padding_margin=self._display_margin),
             log_record.train_loss.format(
                 formatter=".5e", padding_margin=self._display_margin
             ),
@@ -171,7 +175,31 @@
                 label=f"validation/{k}")
         plt.xlabel('epoch')
         plt.ylabel('loss')
         plt.yscale('log')
         plt.legend()
         plt.savefig(self._loss_figure_path)
         plt.close(fig)
+
+    def save_model(
+        self,
+        epoch: int,
+        model: Network,
+        optimizer: Optimizer,
+        validation_loss: float,
+        trainer_setting: TrainerSetting
+    ) -> None:
+        enc_ext = ".enc" if trainer_setting.model_key is not None else ""
+        file_path = trainer_setting.output_directory / \
+            pathlib.Path(f"snapshot_epoch_{epoch}.pth{enc_ext}")
+        siml_file = SimlFileBuilder.checkpoint_file(file_path)
+
+        data = {
+            'epoch': epoch,
+            'validation_loss': validation_loss,
+            'model_state_dict': model.state_dict(),
+            'optimizer_state_dict': optimizer.state_dict()
+        }
+        siml_file.save(
+            data,
+            encrypt_key=trainer_setting.model_key
+        )
```

## siml/setting.py

```diff
@@ -1,14 +1,15 @@
+import itertools
 import dataclasses as dc
 import io
 import os
 import typing
 from enum import Enum
 from pathlib import Path
-from typing import Optional
+from typing import Optional, Union
 
 import numpy as np
 import optuna
 import yaml
 
 from siml import util
 from siml.path_like_objects import SimlFileBuilder
@@ -687,14 +688,53 @@
 
     @property
     def variable_information(self):
         out_dict = self.inputs.to_dict()
         out_dict.update(self.outputs.to_dict())
         return out_dict
 
+    @property
+    def input_is_dict(self):
+        return isinstance(self.inputs.variables, dict)
+
+    @property
+    def output_is_dict(self):
+        return isinstance(self.outputs.variables, dict)
+
+    @property
+    def input_names_list(self):
+        return self._convert_to_list(self.input_names)
+
+    @property
+    def output_names_list(self):
+        return self._convert_to_list(self.output_names)
+
+    @property
+    def overwrite_restart_mode(self):
+        if self.restart_directory is None:
+            return False
+
+        if self.output_directory == self.restart_directory:
+            return True
+
+        return False
+
+    def _convert_to_list(self, values: Union[list, dict[str, list]]):
+        if isinstance(values, list):
+            return values
+        if isinstance(values, dict):
+            _list = [
+                v for v in values.values()
+            ]
+            return list(itertools.chain.from_iterable(_list))
+
+        raise NotImplementedError(
+            f"Unknown data type: {type(values)}"
+        )
+
     def determine_element_wise(self) -> bool:
         if self.time_series:
             return False
         if self.element_wise or self.simplified_model:
             return True
 
         return False
@@ -711,14 +751,51 @@
         if self.suffix is None:
             suffix_string = ''
         else:
             suffix_string = f"_{self.suffix}"
         self.output_directory = base \
             / f"{self.name}{suffix_string}{id_string}_{util.date_string()}"
 
+    def determine_batch_sizes(self) -> tuple[int, int]:
+        element_wise = self.determine_element_wise()
+        if element_wise:
+            if self.element_batch_size > 0:
+                return (
+                    self.element_batch_size,
+                    self.validation_element_batch_size
+                )
+            if self.simplified_model:
+                return self.batch_size, self.validation_batch_size
+            raise ValueError(
+                'element_batch_size is '
+                f"{self.element_batch_size} < 1 "
+                'while element_wise is set to be true.')
+
+        if self.element_batch_size > 1 and self.batch_size > 1:
+            raise ValueError(
+                'batch_size cannot be > 1 when element_batch_size > 1.')
+
+        return self.batch_size, self.validation_batch_size
+
+    def get_input_time_series_keys(self) -> list[str]:
+        if not isinstance(self.inputs.time_series, dict):
+            return []
+        return [
+            k for k, v in self.inputs.time_series.items()
+            if np.any(v)
+        ]
+
+    def get_output_time_series_keys(self) -> list[str]:
+        if not isinstance(self.outputs.time_series, dict):
+            return []
+        return [
+            k for k, v in self.outputs.time_series.items()
+            if np.any(v)
+        ]
+
 
 @dc.dataclass
 class InfererSetting(TypedDataClass):
     """
     model: pathlib.Path optional
         Model directory, file path, or buffer. If not fed,
         TrainerSetting.pretrain_directory will be used.
```

## siml/trainer.py

```diff
@@ -1,31 +1,28 @@
-import enum
-import io
-import random
-from typing import Callable
+from typing import Callable, Union
 
-import ignite
 import numpy as np
-import optuna
-import torch
-import yaml
+from ignite.engine import Engine, State
 from torch import Tensor
-from tqdm import tqdm
+from torch.optim import Optimizer
+from torch.utils.data import DataLoader
 
-from siml.loss_operations import LossCalculatorBuilder
+from siml.loss_operations import LossCalculatorBuilder, ILossCalculator
+from siml.networks import Network
 from siml.services.environment import ModelEnvironmentSetting
-from siml.services.model_builder import ModelBuilder
-from siml.services.model_selector import ModelSelectorBuilder
-from siml.services.training import (InnerTrainingSetting, LogRecordItems,
+from siml.services.training import (InnerTrainingSetting,
                                     SimlTrainingConsoleLogger,
                                     SimlTrainingFileLogger)
-from siml.siml_variables import siml_tensor_variables
+from siml.services.training.data_loader_builder import DataLoaderBuilder
+from siml.services.training.events_assigners import (TrainerEventsAssigner,
+                                                     ValidationEventsAssigner)
+from siml.services.training.trainers_builder import TrainersBuilder
 from siml.utils.timer import SimlStopWatch
 
-from . import datasets, setting, update_functions, util
+from . import datasets, setting, util
 
 
 class Trainer:
 
     def __init__(self,
                  main_settings: setting.MainSetting,
                  *,
@@ -47,794 +44,242 @@
         --------
         None
         """
 
         if not isinstance(main_settings, setting.MainSetting):
             raise ValueError(
                 f"Unknown type for settings: {main_settings.__class__}")
-        self.inference_mode = False
+
         self.user_loss_function_dic = user_loss_function_dic
 
-        inner_setting = InnerTrainingSetting(main_settings=main_settings)
+        self._inner_setting = InnerTrainingSetting(main_setting=main_settings)
         # HACK: temporarly hack. Better to handle as a inner setting.
-        self.setting = inner_setting.main_settings
-        overwrite_restart_mode = self._overwrite_restart_mode()
+        self.setting = self._inner_setting.main_setting
 
         self.optuna_trial = optuna_trial
         self._env_setting = self._create_model_env_setting()
-
-        self.prepare_training()
-        self._console_logger = SimlTrainingConsoleLogger(
-            display_margin=self.setting.trainer.display_mergin,
-            loss_keys=self.model.get_loss_keys()
+        self._collate_fn = self._create_collate_fn()
+        self._data_loader_builder = DataLoaderBuilder(
+            main_setting=self.setting,
+            collate_fn=self._collate_fn,
+            decrypt_key=self.setting.get_crypt_key()
         )
-        self._file_logger = SimlTrainingFileLogger(
-            file_path=inner_setting.log_file_path,
-            loss_figure_path=inner_setting.loss_figure_path,
-            loss_keys=self.model.get_loss_keys(),
-            continue_mode=overwrite_restart_mode
+        self._loss_calculator = LossCalculatorBuilder.create(
+            trainer_setting=self.setting.trainer,
+            user_loss_function_dic=self.user_loss_function_dic
         )
-        time_offset = self._file_logger.read_offset_start_time()
-        self._stop_watch = SimlStopWatch(offset=time_offset)
+        self._trainers_builder = self._create_trainers_builder(
+            prepare_batch=self._collate_fn.prepare_batch,
+            loss_calculator=self._loss_calculator
+        )
+
+        # SET IN _initialize_state()
+        self.train_loader: DataLoader = None
+        self.validation_loader: DataLoader = None
+        self.test_loader: DataLoader = None
+        self._model: Network = None
+        self._optimizer: Optimizer = None
+        self._trainer: Engine = None
+        self._evaluator: Engine = None
+        self._console_logger: SimlTrainingConsoleLogger = None
+        self._file_logger: SimlTrainingFileLogger = None
+        self._stop_watch: SimlStopWatch = None
 
-    def _create_model_env_setting(self) -> ModelEnvironmentSetting:
-        trainer_setting = self.setting.trainer
-        _model_env = ModelEnvironmentSetting(
-            gpu_id=trainer_setting.gpu_id,
-            seed=trainer_setting.seed,
-            data_parallel=trainer_setting.data_parallel,
-            model_parallel=trainer_setting.model_parallel,
-            time_series=trainer_setting.time_series
-        )
-        return _model_env
+        # Prepare
+        self._env_setting.set_seed()
+        self._initialize_state()
 
-    def train(self, draw_model: bool = True):
-        """Perform training.
+    def train(self, draw_model: bool = True) -> float:
+        """Start training
 
         Parameters
         ----------
-        None
+        draw_model : bool, optional
+            If True, output figure of models, by default True
 
         Returns
-        --------
-        loss: float
-            Loss value after training.
+        -------
+        float
+            loss for validaiton data
         """
+        self._prepare_files_and_dirs(draw_model=draw_model)
+        validation_loss = self._run_training()
+        return validation_loss
 
-        print(f"Output directory: {self.setting.trainer.output_directory}")
-        overwrite_restart_mode = self._overwrite_restart_mode()
-
-        self.setting.trainer.output_directory.mkdir(
-            parents=True, exist_ok=True
-        )
-        if self.setting.trainer.draw_network and draw_model:
-            self.model.draw(self.setting.trainer.output_directory)
-
-        yaml_file_name = f"restart_settings_{util.date_string()}.yml" \
-            if overwrite_restart_mode else "settings.yml"
-        setting.write_yaml(
-            self.setting,
-            self.setting.trainer.output_directory / yaml_file_name,
-            key=self.setting.trainer.model_key)
-
-        print(self._console_logger.output_header())
-        self._file_logger.write_header_if_needed()
-        self._stop_watch.start()
-
-        self.pbar = self.create_pbar(
-            len(self.train_loader) * self.setting.trainer.log_trigger_epoch)
-
-        self.trainer.run(
-            self.train_loader, max_epochs=self.setting.trainer.n_epoch)
-        self.pbar.close()
+    def evaluate(
+        self,
+        evaluate_test: bool = False,
+        load_best_model: bool = False
+    ) -> tuple[State, Union[State, None], Union[State, None]]:
+        """Evaluate model performance
 
-        df = self._file_logger.read_history()
-        validation_loss = np.min(df['validation_loss'])
+        Parameters
+        ----------
+        evaluate_test : bool, optional
+            If True, evaluation by test dataset is performed, by default False
+        load_best_model : bool, optional
+            If True, best model is used to evaluate, by default False
 
-        return validation_loss
+        Returns
+        -------
+        tuple[State, Union[State, None], Union[State, None]]
+            ignite State objects for train, validation and test dataset 
+        """
 
-    def evaluate(self, evaluate_test=False, load_best_model=False):
         if load_best_model:
             self.setting.trainer.pretrain_directory \
                 = self.setting.trainer.output_directory
-            self.model = self._setup_model()
-        train_state = self.evaluator.run(self.train_loader)
+            self._initialize_state()
+        train_state = self._evaluator.run(self.train_loader)
         if len(self.validation_loader) > 0:
-            validation_state = self.evaluator.run(self.validation_loader)
+            validation_state = self._evaluator.run(self.validation_loader)
         else:
             validation_state = None
 
         if evaluate_test:
-            test_state = self.evaluator.run(self.test_loader)
-            return train_state, validation_state, test_state
+            test_state = self._evaluator.run(self.test_loader)
         else:
-            return train_state, validation_state
-
-    def _overwrite_restart_mode(self) -> bool:
-        if self.setting.trainer.restart_directory is None:
-            return False
+            test_state = None
+        return train_state, validation_state, test_state
 
-        if self.setting.trainer.output_directory == \
-                self.setting.trainer.restart_directory:
-            return True
-
-        return False
-
-    def prepare_training(self):
-        self._env_setting.set_seed()
+    def _initialize_state(self):
+        # Initialize state
+        self.train_loader, self.validation_loader, self.test_loader = \
+            self._data_loader_builder.create()
+        self._trainer, self._evaluator, self._model, self._optimizer =\
+            self._trainers_builder.create(epoch_length=len(self.train_loader))
 
-        if len(self.setting.trainer.input_names) == 0:
-            raise ValueError('No input_names fed')
-        if len(self.setting.trainer.output_names) == 0:
-            raise ValueError('No output_names fed')
-
-        # Define model
-        self.model = self._setup_model()
-
-        self.element_wise = self.setting.trainer.determine_element_wise()
-        self.loss = LossCalculatorBuilder.create(
-            trainer_setting=self.setting.trainer,
-            user_loss_function_dic=self.user_loss_function_dic
+        self._console_logger, self._file_logger = self._setup_loggers(
+            self._model
         )
+        self._stop_watch = self._setup_stopwatch(self._file_logger)
 
-        # Manage settings
-        if self.optuna_trial is None \
-                and self.setting.trainer.prune:
-            self.setting.trainer.prune = False
-            print('No optuna.trial fed. Set prune = False.')
-
-        # Manage restart and pretrain
-        self._generate_trainer()
-        self._load_restart_model_if_needed()
-
-        # Expand data directories
-        self.setting.data.train = self.train_loader.dataset.data_directories
-        self.setting.data.validation \
-            = self.validation_loader.dataset.data_directories
-        self.setting.data.test = self.test_loader.dataset.data_directories
-
-        return
-
-    def output_stats(self):
-        dict_stats = {
-            name: self._calculate_stats(parameter)
-            for name, parameter in self.model.named_parameters()}
-        iteration = self.trainer.state.iteration
-        epoch = self.trainer.state.epoch
-        dict_stats.update({
-            'iteration': self.trainer.state.iteration,
-            'epoch': self.trainer.state.epoch,
-            'epoch_length': self.trainer.state.epoch_length})
-
-        file_name = self.setting.trainer.output_directory \
-            / f"stats_epoch{epoch}_iteration{iteration}.yml"
-        with open(file_name, 'w') as f:
-            yaml.dump(dict_stats, f)
-        return dict_stats
-
-    def _calculate_stats(self, parameter):
-        dict_stats = {}
-        if parameter.grad is not None:
-            dict_stats.update(
-                self._calculate_tensor_stats(parameter.grad, 'grad_'))
-        dict_stats.update(self._calculate_tensor_stats(parameter, ''))
-        return dict_stats
-
-    def _calculate_tensor_stats(self, tensor, prefix):
-        numpy_tensor = tensor.detach().cpu().numpy()
-        abs_numpy_tensor = np.abs(numpy_tensor)
-        return {
-            f"{prefix}mean": float(np.mean(numpy_tensor)),
-            f"{prefix}std": float(np.std(numpy_tensor)),
-            f"{prefix}max": float(np.max(numpy_tensor)),
-            f"{prefix}min": float(np.min(numpy_tensor)),
-            f"{prefix}absmax": float(np.max(abs_numpy_tensor)),
-            f"{prefix}absmin": float(np.min(abs_numpy_tensor)),
-        }
-
-    def _generate_trainer(self):
-
-        if self.element_wise:
-            if self.setting.trainer.element_batch_size > 0:
-                batch_size = self.setting.trainer.element_batch_size
-                validation_batch_size = \
-                    self.setting.trainer.validation_element_batch_size
-            else:
-                if self.setting.trainer.simplified_model:
-                    batch_size = self.setting.trainer.batch_size
-                    validation_batch_size \
-                        = self.setting.trainer.validation_batch_size
-                else:
-                    raise ValueError(
-                        'element_batch_size is '
-                        f"{self.setting.trainer.element_batch_size} < 1 "
-                        'while element_wise is set to be true.')
-        else:
-            if self.setting.trainer.element_batch_size > 1 \
-                    and self.setting.trainer.batch_size > 1:
-                raise ValueError(
-                    'batch_size cannot be > 1 when element_batch_size > 1.')
-            batch_size = self.setting.trainer.batch_size
-            validation_batch_size = self.setting.trainer.validation_batch_size
-
-        if len(self.setting.trainer.split_ratio) > 0:
-            develop_dataset = datasets.LazyDataset(
-                self.setting.trainer.input_names,
-                self.setting.trainer.output_names,
-                self.setting.data.develop,
-                recursive=self.setting.trainer.recursive,
-                decrypt_key=self.setting.data.encrypt_key)
-
-            train, validation, test = util.split_data(
-                develop_dataset.data_directories,
-                **self.setting.trainer.split_ratio)
-            self.setting.data.train = train
-            self.setting.data.validation = validation
-            self.setting.data.test = test
-
-        input_is_dict = isinstance(
-            self.setting.trainer.inputs.variables, dict)
-        output_is_dict = isinstance(
-            self.setting.trainer.outputs.variables, dict)
-        if isinstance(self.setting.trainer.inputs.time_series, dict):
-            self.input_time_series_keys = [
-                k for k, v in self.setting.trainer.inputs.time_series.items()
-                if np.any(v)]
-        else:
-            self.input_time_series_keys = []
-        if isinstance(self.setting.trainer.outputs.time_series, dict):
-            self.output_time_series_keys = [
-                k for k, v in self.setting.trainer.outputs.time_series.items()
-                if np.any(v)]
-        else:
-            self.output_time_series_keys = []
-        self.input_time_slices = self.setting.trainer.inputs.time_slice
-        self.output_time_slices = self.setting.trainer.outputs.time_slice
-        self.collate_fn = datasets.CollateFunctionGenerator(
-            time_series=self.setting.trainer.time_series,
-            dict_input=input_is_dict, dict_output=output_is_dict,
-            use_support=self.setting.trainer.support_inputs,
-            element_wise=self.element_wise,
-            data_parallel=self.setting.trainer.data_parallel,
-            input_time_series_keys=self.input_time_series_keys,
-            output_time_series_keys=self.output_time_series_keys,
-            input_time_slices=self.input_time_slices,
-            output_time_slices=self.output_time_slices)
-        self.prepare_batch = self.collate_fn.prepare_batch
-
-        if self.setting.trainer.lazy:
-            self.train_loader, self.validation_loader, self.test_loader = \
-                self._get_data_loaders(
-                    datasets.LazyDataset, batch_size, validation_batch_size,
-                    decrypt_key=self.setting.data.encrypt_key)
-        else:
-            if self.element_wise:
-                self.train_loader, self.validation_loader, self.test_loader = \
-                    self._get_data_loaders(
-                        datasets.ElementWiseDataset, batch_size,
-                        validation_batch_size,
-                        decrypt_key=self.setting.data.encrypt_key)
-            else:
-                self.train_loader, self.validation_loader, self.test_loader = \
-                    self._get_data_loaders(
-                        datasets.OnMemoryDataset, batch_size,
-                        validation_batch_size,
-                        decrypt_key=self.setting.data.encrypt_key)
-        self._check_data_dimension(self.setting.trainer.input_names)
-        self._check_data_dimension(self.setting.trainer.output_names)
-
-        self.optimizer = self._create_optimizer()
-
-        self.trainer = self._create_supervised_trainer()
-        self.evaluator = self._create_supervised_evaluator()
-
-        self.desc = "loss: {:.5e}"
-        # trainer_tick = max(len(self.train_loader) // 100, 1)
-        trainer_tick = 1
-
-        @self.trainer.on(ignite.engine.Events.ITERATION_COMPLETED)
-        def log_training_loss(engine):
-            self.pbar.desc = self.desc.format(engine.state.output)
-            self.pbar.update(trainer_tick)
-            return
-
-        self.evaluator_desc = "evaluating"
-        # evaluator_tick = max(
-        #     (len(self.train_loader) + len(self.validation_loader)) // 100, 1)
-        evaluator_tick = 1
-
-        @self.evaluator.on(
-            ignite.engine.Events.ITERATION_COMPLETED(every=evaluator_tick))
-        def log_evaluation(engine):
-            self.evaluation_pbar.desc = self.evaluator_desc
-            self.evaluation_pbar.update(evaluator_tick)
-            return
-
-        @self.trainer.on(
-            ignite.engine.Events.EPOCH_COMPLETED(
-                every=self.setting.trainer.log_trigger_epoch))
-        def log_training_results(engine):
-            self.pbar.close()
-
-            self.evaluation_pbar = tqdm(
-                initial=0, leave=False,
-                total=len(self.train_loader) + len(self.validation_loader),
-                desc=self.evaluator_desc, ncols=80, ascii=True)
-            self.evaluator.run(self.train_loader)
-            train_loss = self.evaluator.state.metrics['loss']
-            train_other_losses = {
-                k: v for k, v in self.evaluator.state.metrics.items()
-                if k != 'loss'}
-
-            if len(self.validation_loader) > 0:
-                self.evaluator.run(self.validation_loader)
-                validation_loss = self.evaluator.state.metrics['loss']
-                validation_other_losses = {
-                    k: v for k, v in self.evaluator.state.metrics.items()
-                    if k != 'loss'}
-            else:
-                validation_loss = np.nan
-                validation_other_losses = {}
-            self.evaluation_pbar.close()
-
-            log_record = LogRecordItems(
-                epoch=engine.state.epoch,
-                train_loss=train_loss,
-                train_other_losses=train_other_losses,
-                validation_loss=validation_loss,
-                validation_other_losses=validation_other_losses,
-                elapsed_time=self._stop_watch.watch()
-            )
-
-            # Print log
-            tqdm.write(self._console_logger.output(log_record))
-
-            self.pbar = self.create_pbar(
-                len(self.train_loader)
-                * self.setting.trainer.log_trigger_epoch)
-            self.pbar.n = self.pbar.last_print_n = 0
-
-            # Save checkpoint
-            self.save_model(engine, validation_loss)
-
-            # Write log
-            self._file_logger.write(log_record)
-
-            # Plot
-            self._file_logger.save_figure()
-            return
-
-        # Add early stopping
-        class StopTriggerEvents(enum.Enum):
-            EVALUATED = 'evaluated'
-
-        @self.trainer.on(
-            ignite.engine.Events.EPOCH_COMPLETED(
-                every=self.setting.trainer.stop_trigger_epoch))
-        def fire_stop_trigger(engine):
-            self.evaluator.fire_event(StopTriggerEvents.EVALUATED)
-            return
-
-        def score_function(engine):
-            return -engine.state.metrics['loss']
-
-        self.evaluator.register_events(*StopTriggerEvents)
-        self.early_stopping_handler = ignite.handlers.EarlyStopping(
-            patience=self.setting.trainer.patience,
-            score_function=score_function,
-            trainer=self.trainer)
-        self.evaluator.add_event_handler(
-            StopTriggerEvents.EVALUATED, self.early_stopping_handler)
-
-        # Add pruning setting
-        if self.optuna_trial is not None:
-            pruning_handler = optuna.integration.PyTorchIgnitePruningHandler(
-                self.optuna_trial, 'loss', self.trainer)
-            self.evaluator.add_event_handler(
-                StopTriggerEvents.EVALUATED, pruning_handler)
-
-        return
-
-    def save_model(self, engine, validation_loss):
-        if self.setting.trainer.model_key is None:
-            torch.save(
-                {
-                    'epoch': engine.state.epoch,
-                    'validation_loss': validation_loss,
-                    'model_state_dict': self.model.state_dict(),
-                    'optimizer_state_dict': self.optimizer.state_dict()
-                },
-                self.setting.trainer.output_directory
-                / f"snapshot_epoch_{engine.state.epoch}.pth")
-        else:
-            b = io.BytesIO()
-            torch.save(
-                {
-                    'epoch': engine.state.epoch,
-                    'validation_loss': validation_loss,
-                    'model_state_dict': self.model.state_dict(),
-                    'optimizer_state_dict': self.optimizer.state_dict()
-                },
-                b)
-            util.encrypt_file(
-                self.setting.trainer.model_key,
-                self.setting.trainer.output_directory
-                / f"snapshot_epoch_{engine.state.epoch}.pth.enc",
-                b)
-        return
-
-    def create_pbar(self, total):
-        return tqdm(
-            initial=0, leave=False,
-            total=len(self.train_loader)
-            * self.setting.trainer.log_trigger_epoch,
-            desc=self.desc.format(0), ncols=80, ascii=True)
-
-    def _select_step_update_function(
-        self
-    ) -> update_functions.IStepUpdateFunction:
-        if self.setting.trainer.pseudo_batch_size >= 1:
-            return update_functions.PseudoBatchStep(
-                batch_size=self.setting.trainer.pseudo_batch_size,
-                loss_func=self.loss,
-                other_loss_func=self._calculate_other_loss,
-                split_data_func=self._split_data_if_needed,
-                device=self._env_setting.get_device(),
-                output_device=self._env_setting.get_output_device(),
-                loss_slice=self.setting.trainer.loss_slice,
-                time_series_split=self.setting.trainer.time_series_split,
-                clip_grad_norm=self.setting.trainer.clip_grad_norm,
-                clip_grad_value=self.setting.trainer.clip_grad_value
-            )
-        elif not self.element_wise \
-                and self.setting.trainer.element_batch_size > 0:
-            return update_functions.ElementBatchUpdate(
-                element_batch_size=self.setting.trainer.element_batch_size,
-                loss_func=self.loss,
-                other_loss_func=self._calculate_other_loss,
-                split_data_func=self._split_data_if_needed,
-                clip_grad_norm=self.setting.trainer.clip_grad_norm,
-                clip_grad_value=self.setting.trainer.clip_grad_value
-            )
-        else:
-            return update_functions.StandardUpdate(
-                loss_func=self.loss,
-                other_loss_func=self._calculate_other_loss,
-                split_data_func=self._split_data_if_needed,
-                device=self._env_setting.get_device(),
-                output_device=self._env_setting.get_output_device(),
-                loss_slice=self.setting.trainer.loss_slice,
-                time_series_split=self.setting.trainer.time_series_split,
-                clip_grad_norm=self.setting.trainer.clip_grad_norm,
-                clip_grad_value=self.setting.trainer.clip_grad_value
-            )
-
-    def _create_supervised_trainer(self):
-
-        update_function = self._select_step_update_function()
-
-        def update_model(engine, batch):
-            self.model.train()
-            if self.setting.trainer.time_series_split is None:
-                input_device = self._env_setting.get_device()
-                support_device = self._env_setting.get_device()
-                output_device = self._env_setting.get_output_device()
-            else:
-                input_device = 'cpu'
-                support_device = self._env_setting.get_device()
-                output_device = 'cpu'
-            x, y = self.prepare_batch(
-                batch, device=input_device, output_device=output_device,
-                support_device=support_device,
-                non_blocking=self.setting.trainer.non_blocking)
-            loss = update_function(x, y, self.model, self.optimizer)
-            if self.setting.trainer.output_stats:
-                self.output_stats()
-            return loss
-
-        return ignite.engine.Engine(update_model)
-
-    def _split_data_if_needed(self, x, y, time_series_split):
-        if time_series_split is None:
-            return [x], [y]
-        split_x_tensors = self._split_core(
-            x['x'], self.input_time_series_keys, time_series_split)
-        split_xs = [
-            {
-                'x': split_x_tensor,
-                'original_shapes':
-                self._update_original_shapes(
-                    split_x_tensor, x['original_shapes']),
-                'supports': x['supports']}
-            for split_x_tensor in split_x_tensors]
-        split_ys = self._split_core(
-            y, self.output_time_series_keys, time_series_split)
-        return split_xs, split_ys
-
-    def _update_original_shapes(self, x, previous_shapes):
-        if previous_shapes is None:
-            return None
-        if isinstance(x, torch.Tensor):
-            previous_shapes[:, 0] = len(x)
-            return previous_shapes
-        elif isinstance(x, dict):
-            return {
-                k: self._update_original_shapes(v, previous_shapes[k])
-                for k, v in x.items()}
-        else:
-            raise ValueError(f"Invalid format: {x}")
-
-    def _split_core(self, x, time_series_keys, time_series_split):
-        if isinstance(x, torch.Tensor):
-            len_x = len(x)
-        elif isinstance(x, dict):
-            lens = np.array([
-                len(v) for k, v in x.items() if k in time_series_keys])
-            if not np.all(lens == lens[0]):
-                raise ValueError(
-                    f"Time series length mismatch: {time_series_keys}, {lens}")
-            len_x = lens[0]
-        else:
-            raise ValueError(f"Invalid format: {x}")
-
-        start, step, length = time_series_split
-        range_ = range(start, len_x - length + 1, step)
-
-        if isinstance(x, torch.Tensor):
-            return [x[s:s+length] for s in range_]
-
-        elif isinstance(x, dict):
-            return [{
-                k:
-                v[s:s+length] if k in time_series_keys
-                else v for k, v in x.items()} for s in range_]
-
-        else:
-            raise ValueError(f"Invalid format: {x}")
-
-    def _calculate_other_loss(self, model, y_pred, y, original_shapes=None):
-        if original_shapes is None:
-            original_shapes = [y_pred.shape]
-        loss = 0.
-        loss_coeffs = model.get_loss_coeffs()
-        for loss_key, loss_value in model.get_losses().items():
-            if 'residual' in loss_key:
-                loss += loss_value * loss_coeffs[loss_key]
-            else:
-                raise ValueError(f"Unexpected loss_key: {loss_key}")
-        return loss
-
-    def _create_supervised_evaluator(self):
-
-        def _inference(engine, batch):
-            self.model.eval()
-            if self.setting.trainer.time_series_split_evaluation is None:
-                input_device = self._env_setting.get_device()
-                support_device = self._env_setting.get_device()
-            else:
-                input_device = 'cpu'
-                support_device = self._env_setting.get_device()
-
-            with torch.no_grad():
-                x, y = self.prepare_batch(
-                    batch, device=input_device,
-                    output_device='cpu',
-                    support_device=support_device,
-                    non_blocking=self.setting.trainer.non_blocking)
-                split_xs, split_ys = self._split_data_if_needed(
-                    x, y,
-                    self.setting.trainer.time_series_split_evaluation)
-
-                y_pred = []
-                device = self._env_setting.get_device()
-                for split_x in split_xs:
-                    siml_x = siml_tensor_variables(split_x['x'])
-                    split_x['x'] = siml_x.send(device).get_values()
-                    y_pred.append(self.model(split_x))
-
-                if self.setting.trainer.time_series_split_evaluation is None:
-                    original_shapes = x['original_shapes']
-                else:
-                    cat_x = util.cat_time_series(
-                        [split_x['x'] for split_x in split_xs],
-                        time_series_keys=self.input_time_series_keys)
-                    original_shapes = self._update_original_shapes(
-                        cat_x, x['original_shapes'])
-                y_pred = util.cat_time_series(
-                    y_pred, time_series_keys=self.output_time_series_keys)
-
-                ans_y = util.cat_time_series(
-                    split_ys,
-                    time_series_keys=self.output_time_series_keys
-                )
-                ans_siml_y = siml_tensor_variables(ans_y)
-                output_device = self._env_setting.get_output_device()
-                y = ans_siml_y.send(output_device).get_values()
-                return y_pred, y, {
-                    'original_shapes': original_shapes,
-                    'model': self.model}
-
-        evaluator_engine = ignite.engine.Engine(_inference)
-
-        metrics = {'loss': ignite.metrics.Loss(self.loss)}
-        for loss_key in self.model.get_loss_keys():
-            metrics.update({loss_key: self._generate_metric(loss_key)})
-
-        for name, metric in metrics.items():
-            metric.attach(evaluator_engine, name)
-        return evaluator_engine
-
-    def _generate_metric(self, loss_key):
-        if 'residual' in loss_key:
-            def gather_loss_key(x):
-                model = x[2]['model']
-                return model.get_losses()[loss_key]
-            metric = ignite.metrics.Average(output_transform=gather_loss_key)
-        else:
-            raise ValueError(f"Unexpected loss type: {loss_key}")
-        return metric
+        # HACK: NEED to be called last
+        self._assign_trainer_events(self._trainer)
+        self._assign_evaluator_events(self._evaluator)
 
-    def _seed_worker(worker_id) -> None:
-        worker_seed = torch.initial_seed() % 2**32
-        np.random.seed(worker_seed)
-        random.seed(worker_seed)
-
-    def _get_data_loaders(
-            self, dataset_generator, batch_size, validation_batch_size=None,
-            decrypt_key=None):
-        if validation_batch_size is None:
-            validation_batch_size = batch_size
-
-        x_variable_names = self.setting.trainer.input_names
-        y_variable_names = self.setting.trainer.output_names
-        train_directories = self.setting.data.train
-        validation_directories = self.setting.data.validation
-        test_directories = self.setting.data.test
-        supports = self.setting.trainer.support_inputs
-        num_workers = self.setting.trainer.num_workers
-        recursive = self.setting.trainer.recursive
-
-        train_dataset = dataset_generator(
-            x_variable_names, y_variable_names,
-            train_directories, supports=supports, num_workers=num_workers,
-            recursive=recursive, decrypt_key=decrypt_key)
-        validation_dataset = dataset_generator(
-            x_variable_names, y_variable_names,
-            validation_directories, supports=supports, num_workers=num_workers,
-            recursive=recursive, allow_no_data=True, decrypt_key=decrypt_key)
-        test_dataset = dataset_generator(
-            x_variable_names, y_variable_names,
-            test_directories, supports=supports, num_workers=num_workers,
-            recursive=recursive, allow_no_data=True, decrypt_key=decrypt_key)
-
-        random_generator = torch.Generator()
-        random_generator.manual_seed(self.setting.trainer.seed)
-
-        print(f"num_workers for data_loader: {num_workers}")
-        train_loader = torch.utils.data.DataLoader(
-            train_dataset,
-            collate_fn=self.collate_fn,
-            batch_size=batch_size,
-            shuffle=True,
-            num_workers=num_workers,
-            worker_init_fn=self._seed_worker,
-            generator=random_generator
-        )
-        validation_loader = torch.utils.data.DataLoader(
-            validation_dataset,
-            collate_fn=self.collate_fn,
-            batch_size=validation_batch_size,
-            shuffle=False,
-            num_workers=num_workers,
-            worker_init_fn=self._seed_worker,
-            generator=random_generator
-        )
-        test_loader = torch.utils.data.DataLoader(
-            test_dataset,
-            collate_fn=self.collate_fn,
-            batch_size=validation_batch_size,
-            shuffle=False,
-            num_workers=num_workers,
-            worker_init_fn=self._seed_worker,
-            generator=random_generator
-        )
-
-        return train_loader, validation_loader, test_loader
-
-    def _create_optimizer(self):
-        optimizer_name = self.setting.trainer.optimizer.lower()
-        if optimizer_name == 'adam':
-            return torch.optim.Adam(
-                self.model.parameters(),
-                **self.setting.trainer.optimizer_setting)
-        elif optimizer_name == 'adamw':
-            return torch.optim.AdamW(
-                self.model.parameters(),
-                **self.setting.trainer.optimizer_setting)
-        else:
-            raise ValueError(f"Unknown optimizer name: {optimizer_name}")
+    def _prepare_files_and_dirs(self, draw_model: bool = True):
+        # setup Directory
+        self.setting.trainer.output_directory.mkdir(
+            parents=True, exist_ok=True
+        )
+        if self.setting.trainer.draw_network and draw_model:
+            self._model.draw(self.setting.trainer.output_directory)
+        self._write_settings_yaml()
 
-    def _check_data_dimension(self, variable_names):
-        data_directory = self.train_loader.dataset.data_directories[0]
+    def _write_settings_yaml(self):
+        overwrite_restart_mode = self.setting.trainer.overwrite_restart_mode
+        yaml_file_name = f"restart_settings_{util.date_string()}.yml" \
+            if overwrite_restart_mode else "settings.yml"
+        setting.write_yaml(
+            self.setting,
+            self.setting.trainer.output_directory / yaml_file_name,
+            key=self.setting.trainer.model_key
+        )
 
-        if isinstance(variable_names, dict):
-            for value in variable_names.values():
-                for variable_name in value:
-                    self._check_single_variable_dimension(
-                        data_directory, variable_name)
-
-        elif isinstance(variable_names, list):
-            for variable_name in variable_names:
-                self._check_single_variable_dimension(
-                    data_directory, variable_name)
+    def _run_training(self):
+        # start logging
+        print(self._console_logger.output_header())
+        self._file_logger.write_header_if_needed()
+        self._stop_watch.start()
 
-        else:
-            raise ValueError(f"Unexpected variable_names: {variable_names}")
+        self._trainer.run(
+            self.train_loader,
+            max_epochs=self.setting.trainer.n_epoch
+        )
+        df = self._file_logger.read_history()
+        validation_loss = np.min(df['validation_loss'])
+        return validation_loss
 
-    def _check_single_variable_dimension(self, data_directory, variable_name):
-        loaded_variable = util.load_variable(
-            data_directory, variable_name,
-            decrypt_key=self.setting.data.encrypt_key)
-        shape = loaded_variable.shape
-        variable_information = self.setting.trainer.variable_information[
-            variable_name]
-        if len(shape) == 2:
-            if shape[-1] != variable_information['dim']:
-                raise ValueError(
-                    f"{variable_name} dimension incorrect: "
-                    f"{shape} vs {variable_information['dim']}")
-        else:
-            pass
-        return
+    def _setup_loggers(
+        self,
+        model: Network
+    ) -> tuple[SimlTrainingConsoleLogger, SimlTrainingFileLogger]:
+        console_logger = SimlTrainingConsoleLogger(
+            display_margin=self.setting.trainer.display_mergin,
+            loss_keys=model.get_loss_keys()
+        )
+        file_logger = SimlTrainingFileLogger(
+            file_path=self._inner_setting.log_file_path,
+            loss_figure_path=self._inner_setting.loss_figure_path,
+            loss_keys=model.get_loss_keys(),
+            continue_mode=self.setting.trainer.overwrite_restart_mode
+        )
+        return console_logger, file_logger
+
+    def _setup_stopwatch(self, file_logger: SimlTrainingFileLogger):
+        time_offset = file_logger.read_offset_start_time()
+        stop_watch = SimlStopWatch(offset=time_offset)
+        return stop_watch
 
-    def _setup_model(self):
-        model_loader = ModelBuilder(
-            model_setting=self.setting.model,
+    def _assign_trainer_events(self, trainer: Engine) -> None:
+        train_events = TrainerEventsAssigner(
+            trainer_setting=self.setting.trainer,
+            file_logger=self._file_logger,
+            console_logger=self._console_logger,
+            train_loader=self.train_loader,
+            validation_loader=self.validation_loader,
+            evaluator=self._evaluator,
+            model=self._model,
+            optimizer=self._optimizer,
+            timer=self._stop_watch
+        )
+        train_events.assign_handlers(trainer)
+
+    def _assign_evaluator_events(self, evaluator: Engine) -> None:
+        evaluator_events = ValidationEventsAssigner(
+            file_logger=self._file_logger,
+            console_logger=self._console_logger,
+            log_trigger_epoch=self.setting.trainer.log_trigger_epoch,
+            train_loader=self.train_loader,
+            validation_loader=self.validation_loader,
+            trainer=self._trainer,
+            model=self._model,
             trainer_setting=self.setting.trainer,
-            env_setting=self._env_setting
+            timer=self._stop_watch
         )
-        if self.setting.trainer.pretrain_directory is None:
-            return model_loader.create_initialized()
-
-        selector = ModelSelectorBuilder.create(
-            self.setting.trainer.snapshot_choise_method
+        evaluator_events.assign_handlers(
+            evaluator, self.optuna_trial
         )
-        snapshot_file = selector.select_model(
-            self.setting.trainer.pretrain_directory)
 
-        return model_loader.create_loaded(
-            snapshot_file.file_path,
-            decrypt_key=self.setting.get_crypt_key()
+    def _create_model_env_setting(self) -> ModelEnvironmentSetting:
+        trainer_setting = self.setting.trainer
+        _model_env = ModelEnvironmentSetting(
+            gpu_id=trainer_setting.gpu_id,
+            seed=trainer_setting.seed,
+            data_parallel=trainer_setting.data_parallel,
+            model_parallel=trainer_setting.model_parallel,
+            time_series=trainer_setting.time_series
         )
+        return _model_env
 
-    def _load_restart_model_if_needed(self):
-        if self.setting.trainer.restart_directory is None:
-            return
-
-        selector = ModelSelectorBuilder.create('latest')
-        snapshot_file = selector.select_model(
-            self.setting.trainer.restart_directory
-        )
-        checkpoint = snapshot_file.load(
-            device=self._env_setting.get_device(),
+    def _create_collate_fn(self):
+        tr_setting = self.setting.trainer
+
+        collate_fn = datasets.CollateFunctionGenerator(
+            time_series=tr_setting.time_series,
+            dict_input=tr_setting.input_is_dict,
+            dict_output=tr_setting.output_is_dict,
+            use_support=tr_setting.support_inputs,
+            element_wise=tr_setting.determine_element_wise(),
+            data_parallel=tr_setting.data_parallel,
+            input_time_series_keys=tr_setting.get_input_time_series_keys(),
+            output_time_series_keys=tr_setting.get_output_time_series_keys(),
+            input_time_slices=tr_setting.inputs.time_slice,
+            output_time_slices=tr_setting.outputs.time_slice
+        )
+        return collate_fn
+
+    def _create_trainers_builder(
+        self,
+        prepare_batch: Callable,
+        loss_calculator: ILossCalculator
+    ):
+        trainers_builder = TrainersBuilder(
+            trainer_setting=self.setting.trainer,
+            model_setting=self.setting.model,
+            env_setting=self._env_setting,
+            prepare_batch_function=prepare_batch,
+            loss_function=loss_calculator,
             decrypt_key=self.setting.get_crypt_key()
         )
-
-        self.model.load_state_dict(checkpoint['model_state_dict'])
-        self.optimizer.load_state_dict(checkpoint['optimizer_state_dict'])
-        self.trainer.load_state_dict({
-            'epoch': checkpoint['epoch'],
-            'validation_loss': checkpoint['validation_loss'],
-            'seed': self.setting.trainer.seed,
-            'max_epochs': self.setting.trainer.n_epoch,
-            'epoch_length': len(self.train_loader),
-        })
-
-        if self.setting.trainer.n_epoch == checkpoint['epoch']:
-            raise FileExistsError(
-                "Checkpoint at last epoch exists. "
-                "Model to restart has already finished"
-            )
-
-        # self.loss = checkpoint['loss']
-        print(f"{snapshot_file.file_path} loaded for restart.")
-        return
+        return trainers_builder
```

## Comparing `siml/services/inference/engine_bulider.py` & `siml/services/inference/engine_builder.py`

 * *Files identical despite different names*

## Comparing `pysiml-0.2.9.dev202306270535.dist-info/LICENSE` & `pysiml-0.2.9.dev202307040514.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pysiml-0.2.9.dev202306270535.dist-info/METADATA` & `pysiml-0.2.9.dev202307040514.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysiml
-Version: 0.2.9.dev202306270535
+Version: 0.2.9.dev202307040514
 Summary: SiML - a Simulation ML library
 Home-page: https://github.com/ricosjp/pysiml
 License: Apache-2.0
 Author: RICOS Co. Ltd.
 Requires-Python: >=3.9,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `pysiml-0.2.9.dev202306270535.dist-info/RECORD` & `pysiml-0.2.9.dev202307040514.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-pyproject.toml,sha256=-4x-cnSu1Yi9sIZR59o8KE8J4YenmKm2blVPBZ66XZk,1520
+pyproject.toml,sha256=bUwTI0ASk1HRlyK_veOxzfJbzdgi9q8OonWAv7-BcD4,1520
 siml/__init__.py,sha256=mC61oSLHO5F6zXHhOrzH51R-vkH0mL4MShhSBiRRe6s,638
 siml/__main__/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 siml/__main__/convert_interim_data.py,sha256=jA6GD7BlnsEjARcln3UBwXlFj64BeFALAmgD1ohBkqo,900
 siml/__main__/convert_raw_data.py,sha256=VNVOyx9lChopF2Q-9OXtN_-MtfBsyjS_JvFwCjdkv0c,1400
 siml/__main__/optimize.py,sha256=6HALn60Mxh4GUiPbSXjvrdpkoQ4NgYSzCHCBRbli4W0,1742
 siml/__main__/plot_losses.py,sha256=0uMsoPN-xR0JhPg0WzSQL5GbD80ovuFO12eVpc0x6Xc,8663
 siml/__main__/prepare_preprocess_converters.py,sha256=w_rzic--RUyISagQOJw_5-oEkOFEKXUN7G1TkTOxd8g,927
@@ -95,48 +95,53 @@
 siml/preprocessing/siml_scalers/scale_functions/standard_scaler.py,sha256=qvyUGXXw4j60xGw0RwXUaHaYlnVZHR9XB_DFkayySBg,570
 siml/preprocessing/siml_scalers/scale_functions/user_defined_scaler.py,sha256=GFwX9UyJ6z9iTy8XiiJgvlv65W6dBRZ8bDLV2sECdTs,865
 siml/preprocessing/siml_scalers/scaler_result_save.py,sha256=9ZD7dibMlteAZvpePfsK5sEAhf4VMadAMclKJpypz54,1012
 siml/preprocessing/siml_scalers/scaler_wrapper.py,sha256=_YoFh6KXCS093l-CjMw8hxvy3pO0GxdMcwCj9uZwJ0o,4367
 siml/services/__init__.py,sha256=UfdYF0fGhc34bu7gPjTSCQgkD0Hnlaavx4AI5yc9iaA,154
 siml/services/environment.py,sha256=oi0GhoCxvI6HtIYPYa0D6JAh2RdD9Ao0jeeV2pVUykQ,2342
 siml/services/inference/__init__.py,sha256=bCltATxDFTamdw_d4jpVP68ZfKUpguExJsDqLUbzVgk,279
-siml/services/inference/core_inferer.py,sha256=NUx1mGojvBlIr0ukDRMzv9hG57hC4Gv2Zso1FPBsyyI,2587
+siml/services/inference/core_inferer.py,sha256=EkfbyqjFwOL9G2jH-UMZuruDDFBeDgmtHa4R9Ae3GUk,2587
 siml/services/inference/data_loader_builder.py,sha256=5FhUabZ39P1yEODpM3pPduFLAyriyexB_qUHmPuJ7NU,1818
-siml/services/inference/engine_bulider.py,sha256=y6K7J_nhK1-3f2Cj3vNQiNh4yzda79ury12RaCFBovE,2619
+siml/services/inference/engine_builder.py,sha256=y6K7J_nhK1-3f2Cj3vNQiNh4yzda79ury12RaCFBovE,2619
 siml/services/inference/inner_setting.py,sha256=sw3_Priovxo87tcfgBObvm6MY--1QAahM-KG4qz244M,5750
 siml/services/inference/metrics_builder.py,sha256=I8ORAOZO4Mf5b0AaPCfpdu0ieqx1peuKkW9Z9H8RaAY,4710
 siml/services/inference/postprocessing/__init__.py,sha256=txubVxvNDftzgw3M05LP2GPmwvvJZCZKJcU02q4iiqs,203
 siml/services/inference/postprocessing/post_fem_data.py,sha256=8apB2-cUyssum_6BOx9uVUhmNNvBjoXRnSWn4w4aJ-A,5603
 siml/services/inference/postprocessing/postprocessor.py,sha256=lnHod9-Wa87QLb4ZMq7cOOeRxFjKQYq4NeuPaTHD6Nk,4979
 siml/services/inference/postprocessing/save_processor.py,sha256=oJVxJJplyH8dLiYIpG1GJWD_Y58RwrnAwlqNt_dLuA0,7052
 siml/services/inference/record_object.py,sha256=9cSmtHyNuVwtQbAxkMoUOhCg7TQ6fgyFFwWqyBJ3Gw4,1082
-siml/services/model_builder.py,sha256=xffry-tULPkx89KSMEI_Ng2ZUngOHWvQNWkFbFntICI,2634
+siml/services/model_builder.py,sha256=N1TH7yARLchn4ZuXQA9-hoGmqVUkHcPUU0D77Gc0kt0,3161
 siml/services/model_selector.py,sha256=q2oXdJcujaOa6Y_HFHZ1emxkNaRN00BAGi_kc0zXmvE,4978
 siml/services/path_rules.py,sha256=fPNdpXcf8GZtI6ZfMrEkKcdo0JkxxPNmnvohbY1evI8,7124
 siml/services/training/__init__.py,sha256=nuxgfAYieJxucFOKJXwdICJuyvUhHdKjup0okMU8ULk,200
-siml/services/training/inner_settings.py,sha256=uSzxV3ftVhefUt1jjsKR_R5lkB5HzQ2VuOboakZZYuk,2653
+siml/services/training/data_loader_builder.py,sha256=pV5j63xz1zyss9HsGKQf20i_dE_t2-QecGDVaRc2gh4,7389
+siml/services/training/engine_builder.py,sha256=3zsc_B5Uk8BZOnDtOK3VEb9MmlS5S6PdTX3Qd-7IXH8,7993
+siml/services/training/events_assigners.py,sha256=bWyGoqWiyVkHXbRf3BNL0LQnbVexjUpcJDRq6BvqAGA,7134
+siml/services/training/inner_settings.py,sha256=bexDtmR5EECIXXjaYdR7NZ7phs-UYC6QL-wgu5epGDw,3084
 siml/services/training/logging_items/__init__.py,sha256=1Njqc0eCpuwo6mzxDv2iRhhvslHG3yfH3oHnCgc3FMc,775
 siml/services/training/logging_items/logging_items.py,sha256=hQMvAImDg2YpHFY8qIj72ICZRW6pgNZ4qdZi4hll2kE,4198
-siml/services/training/training_logger.py,sha256=SuSwfUy5klWCelKkWh39lTA2PNoAFGS0eJNTLNGiWQs,5695
-siml/setting.py,sha256=0DQ9_jJ7PCwgLwghIwrJwi0xtVfGr1YcxFQtw9Gt59U,50394
+siml/services/training/tensor_spliter.py,sha256=pezCbe50ODgef-jjOYTVH-DERN3muv1OZuBq39fzbB4,2729
+siml/services/training/trainers_builder.py,sha256=4bcE_npNBCGzCQAq3K0a_MOgklnIOr59eqZtk0Oe4cA,9217
+siml/services/training/training_logger.py,sha256=C7hz_xCGzV9ms-kv3M67TnPK-wx-AQ8DcKVituJ5LwE,6633
+siml/setting.py,sha256=L3WsnrAo-Te420XxTpHSkVTEvTKv6C0WXXWO3dorJHM,52787
 siml/siml_variables/__init__.py,sha256=Nt8iJ0yLPBJpg1o6K_b5Qr-go5iurvC9FnHxI4lD6eg,163
 siml/siml_variables/array_variables/__init__.py,sha256=Y2syJXtd98L-Z3kRTCOlCEVZffc-xBbuMIS1uv3ekQU,594
 siml/siml_variables/array_variables/interface_wrapper.py,sha256=Wi0GcuEexwx6sqTqVcBCtWo2K7kw_LQN6LOdoXnNFYw,1573
 siml/siml_variables/array_variables/ndarray_wrapper.py,sha256=oNOfbQu_5twQZq9AM_NEWcbswnCzASAEGzCPpUXcujM,1398
 siml/siml_variables/array_variables/sparce_array_wrapper.py,sha256=yyWwfuKHn686-aQemDMIgcig4K9a6XC-HCTYETJS0O8,1809
 siml/siml_variables/tensor_variables/tensor_variables.py,sha256=Nh3W1ft6FbGID7cp88lw2VyVVxTkrx_1ovI_I2DFSX0,4156
 siml/study.py,sha256=Sc8DBdT3ni3mcHICtURUmjDslCkSf7T6lCqADogoRs4,12967
-siml/trainer.py,sha256=DRORw3ji0m_XJWwuVtTuAfUtHfJ0TYW1kDgAkGtDlAI,33627
+siml/trainer.py,sha256=5GBxNYpDDfmxG_p6MkZxbZvFSDRMjSFo1EYqGF-kl6E,10653
 siml/update_functions/__init__.py,sha256=fQY19xMEhZv7k6flZPBmhIgLl3uHuBWkay-YCFfaY64,211
 siml/update_functions/element_batch_update.py,sha256=93_L9jl4D9lFQXmEX1Lo8l4n3rDf1wdZljPJIQd9rUs,1774
 siml/update_functions/pseudo_batch_update.py,sha256=7PS6SEXOMB57uaJQhZ8VrtEiIkDF59JE1c6yyrKL3YY,3623
 siml/update_functions/standard_update.py,sha256=jIgeQ_c9R1dgcxDQWzx-w5TkJ7naDKmNi_WUFFchxc4,2702
 siml/update_functions/update_interface.py,sha256=O1fGrE21iXckz7NTOTDNlyQ4rll1SQDehdc_Kk5we0Q,429
 siml/util.py,sha256=AzvnYN1svE28ioHGPgMjkpiK35hCA5m5qwFEDb3agHA,23027
 siml/utils/__init__.py,sha256=DVdxWEBXfapWAWNM0jUouKJzru4RyK2ru2QheBmrm_s,37
 siml/utils/fem_data_utils.py,sha256=LDB_MxYPg_WELl6D_az9ikMZxAF5Ml5qKUXR2CnuxvE,7682
 siml/utils/timer.py,sha256=DEDtrmFpFqiGRykErkLMnwZ3tWUsOsarubnN40kwb6I,1247
-pysiml-0.2.9.dev202306270535.dist-info/LICENSE,sha256=Ok4O8jxCIpLhGZjTNzgBW8V8xITF_SUVEp1juLijZpA,11431
-pysiml-0.2.9.dev202306270535.dist-info/METADATA,sha256=M7OtrGBdMCWHTNDzXuzqq9zUArPKEjYdS-KeoUgtgLk,1638
-pysiml-0.2.9.dev202306270535.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-pysiml-0.2.9.dev202306270535.dist-info/entry_points.txt,sha256=zXU0Gd56XeUfgaeG-CGXcYaTpORSU6kVeQ_vVvjIFPs,388
-pysiml-0.2.9.dev202306270535.dist-info/RECORD,,
+pysiml-0.2.9.dev202307040514.dist-info/LICENSE,sha256=Ok4O8jxCIpLhGZjTNzgBW8V8xITF_SUVEp1juLijZpA,11431
+pysiml-0.2.9.dev202307040514.dist-info/METADATA,sha256=f1L-eWRQgVtMOnG-7cShn_mR1rB3tH4b3OZYGrINIZ0,1638
+pysiml-0.2.9.dev202307040514.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+pysiml-0.2.9.dev202307040514.dist-info/entry_points.txt,sha256=zXU0Gd56XeUfgaeG-CGXcYaTpORSU6kVeQ_vVvjIFPs,388
+pysiml-0.2.9.dev202307040514.dist-info/RECORD,,
```

