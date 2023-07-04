# Comparing `tmp/engression-0.0.0.dev0.tar.gz` & `tmp/engression-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "engression-0.0.0.dev0.tar", last modified: Sun Jul  2 14:50:34 2023, max compression
+gzip compressed data, was "engression-0.0.1.tar", last modified: Tue Jul  4 07:09:22 2023, max compression
```

## Comparing `engression-0.0.0.dev0.tar` & `engression-0.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 shenxi   (571559) staff       (20)        0 2023-07-02 14:50:34.526590 engression-0.0.0.dev0/
--rw-r--r--   0 shenxi   (571559) staff       (20)     1227 2023-07-02 14:50:34.526480 engression-0.0.0.dev0/PKG-INFO
--rw-r--r--   0 shenxi   (571559) staff       (20)      846 2023-07-01 19:21:22.000000 engression-0.0.0.dev0/README.md
-drwxr-xr-x   0 shenxi   (571559) staff       (20)        0 2023-07-02 14:50:34.524951 engression-0.0.0.dev0/engression/
--rw-r--r--   0 shenxi   (571559) staff       (20)      365 2023-07-02 07:57:11.000000 engression-0.0.0.dev0/engression/__init__.py
-drwxr-xr-x   0 shenxi   (571559) staff       (20)        0 2023-07-02 14:50:34.526191 engression-0.0.0.dev0/engression/data/
--rw-r--r--   0 shenxi   (571559) staff       (20)        0 2023-07-01 15:22:34.000000 engression-0.0.0.dev0/engression/data/__init__.py
--rw-r--r--   0 shenxi   (571559) staff       (20)     1980 2023-07-01 15:22:34.000000 engression-0.0.0.dev0/engression/data/loader.py
--rw-r--r--   0 shenxi   (571559) staff       (20)     2673 2023-07-01 15:22:34.000000 engression-0.0.0.dev0/engression/data/simulator.py
--rw-r--r--   0 shenxi   (571559) staff       (20)    16497 2023-07-02 14:02:03.000000 engression-0.0.0.dev0/engression/engression.py
--rw-r--r--   0 shenxi   (571559) staff       (20)    12725 2023-07-02 07:57:03.000000 engression-0.0.0.dev0/engression/engression_bagged.py
--rw-r--r--   0 shenxi   (571559) staff       (20)     2026 2023-07-02 12:42:28.000000 engression-0.0.0.dev0/engression/loss_func.py
--rw-r--r--   0 shenxi   (571559) staff       (20)     6999 2023-07-02 12:36:08.000000 engression-0.0.0.dev0/engression/models.py
--rw-r--r--   0 shenxi   (571559) staff       (20)     1910 2023-07-02 13:49:25.000000 engression-0.0.0.dev0/engression/utils.py
-drwxr-xr-x   0 shenxi   (571559) staff       (20)        0 2023-07-02 14:50:34.525603 engression-0.0.0.dev0/engression.egg-info/
--rw-r--r--   0 shenxi   (571559) staff       (20)     1227 2023-07-02 14:50:34.000000 engression-0.0.0.dev0/engression.egg-info/PKG-INFO
--rw-r--r--   0 shenxi   (571559) staff       (20)      415 2023-07-02 14:50:34.000000 engression-0.0.0.dev0/engression.egg-info/SOURCES.txt
--rw-r--r--   0 shenxi   (571559) staff       (20)        1 2023-07-02 14:50:34.000000 engression-0.0.0.dev0/engression.egg-info/dependency_links.txt
--rw-r--r--   0 shenxi   (571559) staff       (20)       23 2023-07-02 14:50:34.000000 engression-0.0.0.dev0/engression.egg-info/requires.txt
--rw-r--r--   0 shenxi   (571559) staff       (20)       11 2023-07-02 14:50:34.000000 engression-0.0.0.dev0/engression.egg-info/top_level.txt
--rw-r--r--   0 shenxi   (571559) staff       (20)       38 2023-07-02 14:50:34.526625 engression-0.0.0.dev0/setup.cfg
--rw-r--r--   0 shenxi   (571559) staff       (20)      736 2023-07-02 14:22:02.000000 engression-0.0.0.dev0/setup.py
+drwxr-xr-x   0 shenxi   (571559) staff       (20)        0 2023-07-04 07:09:22.821675 engression-0.0.1/
+-rw-r--r--   0 shenxi   (571559) staff       (20)     2377 2023-07-04 07:09:22.821554 engression-0.0.1/PKG-INFO
+-rw-r--r--   0 shenxi   (571559) staff       (20)     2117 2023-07-04 07:06:20.000000 engression-0.0.1/README.md
+drwxr-xr-x   0 shenxi   (571559) staff       (20)        0 2023-07-04 07:09:22.820129 engression-0.0.1/engression/
+-rw-r--r--   0 shenxi   (571559) staff       (20)      365 2023-07-02 07:57:11.000000 engression-0.0.1/engression/__init__.py
+drwxr-xr-x   0 shenxi   (571559) staff       (20)        0 2023-07-04 07:09:22.821290 engression-0.0.1/engression/data/
+-rw-r--r--   0 shenxi   (571559) staff       (20)        0 2023-07-01 15:22:34.000000 engression-0.0.1/engression/data/__init__.py
+-rw-r--r--   0 shenxi   (571559) staff       (20)     1980 2023-07-01 15:22:34.000000 engression-0.0.1/engression/data/loader.py
+-rw-r--r--   0 shenxi   (571559) staff       (20)     2673 2023-07-01 15:22:34.000000 engression-0.0.1/engression/data/simulator.py
+-rw-r--r--   0 shenxi   (571559) staff       (20)    17701 2023-07-03 08:33:47.000000 engression-0.0.1/engression/engression.py
+-rw-r--r--   0 shenxi   (571559) staff       (20)    12725 2023-07-02 07:57:03.000000 engression-0.0.1/engression/engression_bagged.py
+-rw-r--r--   0 shenxi   (571559) staff       (20)     2026 2023-07-02 12:42:28.000000 engression-0.0.1/engression/loss_func.py
+-rw-r--r--   0 shenxi   (571559) staff       (20)     6999 2023-07-02 12:36:08.000000 engression-0.0.1/engression/models.py
+-rw-r--r--   0 shenxi   (571559) staff       (20)     1910 2023-07-02 13:49:25.000000 engression-0.0.1/engression/utils.py
+drwxr-xr-x   0 shenxi   (571559) staff       (20)        0 2023-07-04 07:09:22.820829 engression-0.0.1/engression.egg-info/
+-rw-r--r--   0 shenxi   (571559) staff       (20)     2377 2023-07-04 07:09:22.000000 engression-0.0.1/engression.egg-info/PKG-INFO
+-rw-r--r--   0 shenxi   (571559) staff       (20)      415 2023-07-04 07:09:22.000000 engression-0.0.1/engression.egg-info/SOURCES.txt
+-rw-r--r--   0 shenxi   (571559) staff       (20)        1 2023-07-04 07:09:22.000000 engression-0.0.1/engression.egg-info/dependency_links.txt
+-rw-r--r--   0 shenxi   (571559) staff       (20)       23 2023-07-04 07:09:22.000000 engression-0.0.1/engression.egg-info/requires.txt
+-rw-r--r--   0 shenxi   (571559) staff       (20)       11 2023-07-04 07:09:22.000000 engression-0.0.1/engression.egg-info/top_level.txt
+-rw-r--r--   0 shenxi   (571559) staff       (20)       38 2023-07-04 07:09:22.821713 engression-0.0.1/setup.cfg
+-rw-r--r--   0 shenxi   (571559) staff       (20)      599 2023-07-04 07:09:04.000000 engression-0.0.1/setup.py
```

### Comparing `engression-0.0.0.dev0/engression/data/loader.py` & `engression-0.0.1/engression/data/loader.py`

 * *Files identical despite different names*

### Comparing `engression-0.0.0.dev0/engression/data/simulator.py` & `engression-0.0.1/engression/data/simulator.py`

 * *Files identical despite different names*

### Comparing `engression-0.0.0.dev0/engression/engression.py` & `engression-0.0.1/engression/engression.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,16 +19,16 @@
             out_dim (int): output dimension
             num_layer (int, optional): number of layers. Defaults to 2.
             hidden_dim (int, optional): number of neurons per layer. Defaults to 100.
             noise_dim (int, optional): noise dimension. Defaults to 100.
             lr (float, optional): learning rate. Defaults to 0.001.
             num_epoches (int, optional): number of epoches. Defaults to 500.
             batch_size (int, optional): batch size. Defaults to None, referring to the full batch.
-            device (str or torch.device, optional): device. Defaults to "cpu". Choices = ["cpu", "cuda"].
-            standardize (bool, optional): whether to standardize data. Defaults to True.
+            device (str or torch.device, optional): device. Defaults to "cpu". Choices = ["cpu", "gpu", "cuda"].
+            standardize (bool, optional): whether to standardize data for training. Defaults to True.
         """
         super().__init__()
         self.num_layer = num_layer
         self.hidden_dim = hidden_dim
         self.noise_dim = noise_dim
         self.lr = lr
         self.num_epoches = num_epoches
@@ -138,75 +138,77 @@
             x (torch.Tensor): training data of predictors.
             y (torch.Tensor): trainging data of responses.
             num_epoches (int, optional): number of training epochs. Defaults to None.
             batch_size (int, optional): batch size for mini-batch SGD. Defaults to 512.
             print_every_nepoch (int, optional): print losses every print_every_nepoch number of epochs. Defaults to 100.
             print_times_per_epoch (int, optional): print losses for print_times_per_epoch times per epoch. Defaults to 1.
             standardize (bool, optional): standardize the data. Defaults to True.
+            verbose (bool, optional): whether to print losses and info. Defaults to True.
         """
         self.train_mode()
         if num_epoches is None:
             num_epoches = self.num_epoches
         if batch_size is None:
             batch_size = self.batch_size
         if standardize:
             self.standardize = standardize
             
         x = vectorize(x)
         y = vectorize(y)
         x = x.to(self.device)
         y = y.to(self.device)
-        if self.standardize: 
-            print("Data is standardized during training only; the printed training losses are on the standardized scale, \n" +
-                  "while during evaluation, the predictions, evaluation metrics, and plots will be on the original scale.\n")
+        if self.standardize and verbose: 
+            print("Data is standardized for training only; the printed training losses are on the standardized scale. \n" +
+                  "However during evaluation, the predictions, evaluation metrics, and plots will be on the original scale.\n")
             x, y = self._standardize_data_and_record_stats(x, y)
         
         if batch_size >= x.size(0)//2:
-            print("Batch is larger than half of the sample size. Training based on full-batch gradient descent.")
+            if verbose:
+                print("Batch is larger than half of the sample size. Training based on full-batch gradient descent.")
             self.batch_size = x.size(0)
             for epoch_idx in range(num_epoches):
                 self.model.zero_grad()
                 y_sample1 = self.model(x)
                 y_sample2 = self.model(x)
-                loss, loss1, loss2 = energy_loss_two_sample(y, y_sample1, y_sample2, verbose=verbose)
+                loss, loss1, loss2 = energy_loss_two_sample(y, y_sample1, y_sample2, verbose=True)
                 loss.backward()
                 self.optimizer.step()
-                if epoch_idx == 0 or  (epoch_idx + 1) % print_every_nepoch == 0:
+                if (epoch_idx == 0 or  (epoch_idx + 1) % print_every_nepoch == 0) and verbose:
                     print("[Epoch {} ({:.0f}%)] energy-loss: {:.4f},  E(|Y-Yhat|): {:.4f},  E(|Yhat-Yhat'|): {:.4f}".format(
                         epoch_idx + 1, 100 * epoch_idx / num_epoches, loss.item(), loss1.item(), loss2.item()))
         else:
             train_loader = make_dataloader(x, y, batch_size=batch_size, shuffle=True)
-            print("Training based on mini-batch gradient descent with a batch size of {}.".format(batch_size))
+            if verbose:
+                print("Training based on mini-batch gradient descent with a batch size of {}.".format(batch_size))
             for epoch_idx in range(num_epoches):
                 for batch_idx, (x_batch, y_batch) in enumerate(train_loader):
                     self.model.zero_grad()
                     y_sample1 = self.model(x_batch)
                     y_sample2 = self.model(x_batch)
-                    loss, loss1, loss2 = energy_loss_two_sample(y_batch, y_sample1, y_sample2, verbose=verbose)
-                    # loss = (y_batch - y_sample1).pow(2).mean()
+                    loss, loss1, loss2 = energy_loss_two_sample(y_batch, y_sample1, y_sample2, verbose=True)
                     loss.backward()
                     self.optimizer.step()
-                    if epoch_idx == 0 or (epoch_idx + 1) % print_every_nepoch == 0:
+                    if (epoch_idx == 0 or (epoch_idx + 1) % print_every_nepoch == 0) and verbose:
                         if (batch_idx + 1) % (len(train_loader) // print_times_per_epoch) == 0:
                             print("[Epoch {} ({:.0f}%), batch {}]: energy-loss: {:.4f},  E(|Y-Yhat|): {:.4f},  E(|Yhat-Yhat'|): {:.4f}".format(
                                 epoch_idx + 1, 100 * epoch_idx / num_epoches, batch_idx + 1, loss.item(), loss1.item(), loss2.item()))
-                            # print("[Epoch {}, batch {}]: loss: {:.4f}".format(
-                            #     epoch_idx + 1, batch_idx + 1, loss.item()))
 
         # Evaluate performance on the training data (on the original scale)
         self.model.eval()
         x, y = self.unstandardize_data(y, x)
         self.tr_loss = self.eval_loss(x, y, loss_type="energy", verbose=True)
         
-        print("\nTraining loss on the original (non-standardized) scale:\n" +
-              "\tEnergy-loss: {:.4f},  E(|Y-Yhat|): {:.4f},  E(|Yhat-Yhat'|): {:.4f}".format(
-                  self.tr_loss[0], self.tr_loss[1], self.tr_loss[2]))
-        
-        print("\nPrediction-loss E(|Y-Yhat|) and variance-loss E(|Yhat-Yhat'|) should ideally be equally large" +
-              "\n-- consider training for more epochs or adjusting hyperparameters if there is a mismatch ")
+        if verbose:
+            print("\nTraining loss on the original (non-standardized) scale:\n" +
+                "\tEnergy-loss: {:.4f},  E(|Y-Yhat|): {:.4f},  E(|Yhat-Yhat'|): {:.4f}".format(
+                    self.tr_loss[0], self.tr_loss[1], self.tr_loss[2]))
+            
+        if verbose:
+            print("\nPrediction-loss E(|Y-Yhat|) and variance-loss E(|Yhat-Yhat'|) should ideally be equally large" +
+                "\n-- consider training for more epochs or adjusting hyperparameters if there is a mismatch ")
     
     def predict(self, x, target="mean", sample_size=100):
         """Point prediction.
 
         Args:
             x (torch.Tensor): data of predictors.
             target (str or float or list, optional): single-valued functional to predict. float refers to the quantiles. Defaults to ["mean"].
@@ -346,13 +348,33 @@
 
 def engression(x, y, 
                num_layer=2, hidden_dim=100, noise_dim=100,
                lr=0.001, num_epoches=500, batch_size=None, 
                print_every_nepoch=100, print_times_per_epoch=1,
                device="cpu", standardize=True,
                verbose=True): 
+    """engression function.
+
+    Args:
+        x (torch.Tensor): training data of predictors.
+        y (torch.Tensor): training data of responses.
+        num_layer (int, optional): number of layers. Defaults to 2.
+        hidden_dim (int, optional): number of neurons per layer. Defaults to 100.
+        noise_dim (int, optional): noise dimension. Defaults to 100.
+        lr (float, optional): learning rate. Defaults to 0.001.
+        num_epoches (int, optional): number of epochs. Defaults to 500.
+        batch_size (int, optional): batch size. Defaults to None.
+        print_every_nepoch (int, optional): print losses every print_every_nepoch number of epochs. Defaults to 100.
+        print_times_per_epoch (int, optional): print losses for print_times_per_epoch times per epoch. Defaults to 1.
+        device (str, torch.device, optional): device. Defaults to "cpu". Choices = ["cpu", "gpu", "cuda"].
+        standardize (bool, optional):  whether to standardize data for training. Defaults to True.
+        verbose (bool, optional): whether to print losses and info. Defaults to True.
+
+    Returns:
+        Engressor object: a fitted engression model.
+    """
     engressor = Engressor(in_dim=x.shape[1], out_dim=y.shape[1], num_layer=num_layer, hidden_dim=hidden_dim, noise_dim=noise_dim, 
                           lr=lr, num_epoches=num_epoches, batch_size=batch_size, device=device, standardize=standardize)
     engressor.train(x, y, num_epoches=num_epoches, batch_size=batch_size, 
                     print_every_nepoch=print_every_nepoch, print_times_per_epoch=print_times_per_epoch, 
                     standardize=standardize, verbose=verbose)
     return engressor
```

### Comparing `engression-0.0.0.dev0/engression/engression_bagged.py` & `engression-0.0.1/engression/engression_bagged.py`

 * *Files identical despite different names*

### Comparing `engression-0.0.0.dev0/engression/loss_func.py` & `engression-0.0.1/engression/loss_func.py`

 * *Files identical despite different names*

### Comparing `engression-0.0.0.dev0/engression/models.py` & `engression-0.0.1/engression/models.py`

 * *Files identical despite different names*

### Comparing `engression-0.0.0.dev0/engression/utils.py` & `engression-0.0.1/engression/utils.py`

 * *Files identical despite different names*

