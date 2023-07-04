# Comparing `tmp/chai-guanaco-1.0.0.tar.gz` & `tmp/chai-guanaco-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chai-guanaco-1.0.0.tar", last modified: Tue Jun 27 20:37:04 2023, max compression
+gzip compressed data, was "dist/chai-guanaco-1.0.1.tar", last modified: Tue Jul  4 20:10:36 2023, max compression
```

## Comparing `chai-guanaco-1.0.0.tar` & `chai-guanaco-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,25 @@
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-06-27 20:37:04.000000 chai-guanaco-1.0.0/
--rw-rw-r--   0 tom       (1002) tom       (1002)     9736 2023-06-27 20:37:04.000000 chai-guanaco-1.0.0/PKG-INFO
--rw-rw-r--   0 tom       (1002) tom       (1002)     8242 2023-06-27 20:36:12.000000 chai-guanaco-1.0.0/README.md
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-06-27 20:37:04.000000 chai-guanaco-1.0.0/chai_guanaco.egg-info/
--rw-rw-r--   0 tom       (1002) tom       (1002)     9736 2023-06-27 20:37:04.000000 chai-guanaco-1.0.0/chai_guanaco.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1002) tom       (1002)      452 2023-06-27 20:37:04.000000 chai-guanaco-1.0.0/chai_guanaco.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1002) tom       (1002)        1 2023-06-27 20:37:04.000000 chai-guanaco-1.0.0/chai_guanaco.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1002) tom       (1002)        1 2023-06-27 20:37:04.000000 chai-guanaco-1.0.0/chai_guanaco.egg-info/not-zip-safe
--rw-rw-r--   0 tom       (1002) tom       (1002)        9 2023-06-27 20:37:04.000000 chai-guanaco-1.0.0/chai_guanaco.egg-info/requires.txt
--rw-rw-r--   0 tom       (1002) tom       (1002)       13 2023-06-27 20:37:04.000000 chai-guanaco-1.0.0/chai_guanaco.egg-info/top_level.txt
--rw-rw-r--   0 tom       (1002) tom       (1002)       38 2023-06-27 20:37:04.000000 chai-guanaco-1.0.0/setup.cfg
--rw-rw-r--   0 tom       (1002) tom       (1002)      746 2023-06-27 20:36:41.000000 chai-guanaco-1.0.0/setup.py
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-06-27 20:37:04.000000 chai-guanaco-1.0.0/src/
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-06-27 20:37:04.000000 chai-guanaco-1.0.0/src/chai_guanaco/
--rw-rw-r--   0 tom       (1002) tom       (1002)        0 2023-06-23 00:07:47.000000 chai-guanaco-1.0.0/src/chai_guanaco/__init__.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     3368 2023-06-27 20:36:12.000000 chai-guanaco-1.0.0/src/chai_guanaco/feedback.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     3653 2023-06-27 20:36:12.000000 chai-guanaco-1.0.0/src/chai_guanaco/submit.py
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-06-27 20:37:04.000000 chai-guanaco-1.0.0/tests/
--rw-rw-r--   0 tom       (1002) tom       (1002)     3454 2023-06-27 20:36:12.000000 chai-guanaco-1.0.0/tests/test_feedback.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     5396 2023-06-27 17:00:52.000000 chai-guanaco-1.0.0/tests/test_submit.py
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-04 20:10:36.000000 chai-guanaco-1.0.1/
+-rw-rw-r--   0 tom       (1002) tom       (1002)     9561 2023-07-04 20:10:36.000000 chai-guanaco-1.0.1/PKG-INFO
+-rw-rw-r--   0 tom       (1002) tom       (1002)     8091 2023-07-04 17:14:25.000000 chai-guanaco-1.0.1/README.md
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-04 20:10:36.000000 chai-guanaco-1.0.1/chai_guanaco.egg-info/
+-rw-rw-r--   0 tom       (1002) tom       (1002)     9561 2023-07-04 20:10:36.000000 chai-guanaco-1.0.1/chai_guanaco.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1002) tom       (1002)      644 2023-07-04 20:10:36.000000 chai-guanaco-1.0.1/chai_guanaco.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1002) tom       (1002)        1 2023-07-04 20:10:36.000000 chai-guanaco-1.0.1/chai_guanaco.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1002) tom       (1002)       61 2023-07-04 20:10:36.000000 chai-guanaco-1.0.1/chai_guanaco.egg-info/entry_points.txt
+-rw-rw-r--   0 tom       (1002) tom       (1002)        1 2023-07-04 20:10:36.000000 chai-guanaco-1.0.1/chai_guanaco.egg-info/not-zip-safe
+-rw-rw-r--   0 tom       (1002) tom       (1002)       22 2023-07-04 20:10:36.000000 chai-guanaco-1.0.1/chai_guanaco.egg-info/requires.txt
+-rw-rw-r--   0 tom       (1002) tom       (1002)       13 2023-07-04 20:10:36.000000 chai-guanaco-1.0.1/chai_guanaco.egg-info/top_level.txt
+-rw-rw-r--   0 tom       (1002) tom       (1002)       22 2023-07-04 18:16:45.000000 chai-guanaco-1.0.1/requirements.txt
+-rw-rw-r--   0 tom       (1002) tom       (1002)       38 2023-07-04 20:10:36.000000 chai-guanaco-1.0.1/setup.cfg
+-rw-rw-r--   0 tom       (1002) tom       (1002)      925 2023-07-04 20:10:31.000000 chai-guanaco-1.0.1/setup.py
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-04 20:10:36.000000 chai-guanaco-1.0.1/src/
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-04 20:10:36.000000 chai-guanaco-1.0.1/src/chai_guanaco/
+-rw-rw-r--   0 tom       (1002) tom       (1002)      188 2023-07-04 18:51:04.000000 chai-guanaco-1.0.1/src/chai_guanaco/__init__.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     3220 2023-07-04 17:14:25.000000 chai-guanaco-1.0.1/src/chai_guanaco/feedback.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1966 2023-07-04 18:51:57.000000 chai-guanaco-1.0.1/src/chai_guanaco/login_cli.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     6659 2023-07-04 20:06:57.000000 chai-guanaco-1.0.1/src/chai_guanaco/submit.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)      496 2023-07-04 17:14:25.000000 chai-guanaco-1.0.1/src/chai_guanaco/utils.py
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-04 20:10:36.000000 chai-guanaco-1.0.1/tests/
+-rw-rw-r--   0 tom       (1002) tom       (1002)     3454 2023-06-27 20:36:12.000000 chai-guanaco-1.0.1/tests/test_feedback.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     2842 2023-07-04 17:14:25.000000 chai-guanaco-1.0.1/tests/test_login.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     6235 2023-07-04 17:14:25.000000 chai-guanaco-1.0.1/tests/test_submit.py
```

### Comparing `chai-guanaco-1.0.0/PKG-INFO` & `chai-guanaco-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chai-guanaco
-Version: 1.0.0
+Version: 1.0.1
 Summary: Chai Guanaco
 Home-page: https://www.chai-research.com
 Author: Chai Research Corp.
 Author-email: hello@chai-research.com
 License: MIT
 Description: [![Guanaco Banner](https://imgur.com/wJHIeAU.png)](https://www.chai-research.com/competition.html)
         
@@ -42,117 +42,114 @@
         ## 🚀 Getting Started
         
         **Getting Developer Key**
         
         Join the [competition discord](https://discord.gg/7mXdjAkw2s), introduce yourself and ask for a developer key. Login-based authentication is coming next 🤗
         
         
-        **Submitting A Model**
+        **Installation**
         
         Use [pip](https://github.com/pypa/pip) to install the Chai Guanaco package
         
         ```sh
         pip install chai-guanaco
         ```
         
+        For one-off authentication run the following in your terminal:
+        
+        ```sh
+        chai-guanaco login
+        ```
+        
+        And pass in your developer key when prompted, you can always logout using `chai-guanaco logout`.
+        
+        **Model Submission**
+        
         Upload any GPT-J 6B based language model *with a tokenizer* to huggingface, i.e. [EleutherAI/gpt-j-6b](https://huggingface.co/EleutherAI/gpt-j-6b). Read [this guide](https://huggingface.co/docs/transformers/model_sharing) if you are unsure. Click the *Use in Transformers* button in huggingface to get the your huggingface model ID (i.e. "EleutherAI/gpt-j-6b")
         
         To submit model simply run:
         
         ```python
-        from chai_guanaco.submit import submit_model
+        import chai_guanaco as chai
         
         model_url = "EleutherAI/gpt-j-6b" # Your model URL
-        developer_key = "CR_XXXX" # Your developer key
+        
         generation_params = {'temperature': 0.75, 'repetition_penalty': 1.13, 'top_p': 0, "top_k": 0}
         submission_parameters = {'model_repo': model_url, 'generation_params': generation_params}
-        response = submit_model(submission_parameters, developer_key)
-        submission_id = response['submission_id']
-        print(submission_id)
-        ````
-        which outputs your submission id, unique to your model submission.
-        
-        To verify the status of a submission, you can use the following command:
         
-        ```python
-        from chai_guanaco.submit import get_model_info
+        submitter = chai.ModelSubmitter()
+        submission_id = submitter.submit(submission_parameters)
+        ````
         
-        model_info = get_model_info(submission_id, developer_key)
-        print(model_info)
-        ```
-        Once the `status` field shows `success` it means your model has been successfully submitted. A submission typically takes around 10 minutes for the tritonisation process to complete.
+        This will display an animation while your model is being deployed, a typical
+        deployment takes approximately 10 minutes.
         
         **Getting User Feedback**
         
         Once your model has been submitted, it is automatically deployed to the Chai Platform where real-life users will evaluate your model performance. To view their feedback, run:
         
         ```python
-        from chai_guanaco.feedback import get_feedback
-        
-        model_feedback = get_feedback(submission_id, developer_key)
-        print(model_feedback.df)
-        ```
-        
-        Here, you will find a pandas dataframe with all the user feedback for your model, including the conversation each user has had with your model.
-        
-        You can print samples from your model's user feedbacks by running
-        
-        ```python
+        model_feedback = chai.get_feedback(submission_id)
         model_feedback.sample()
         ```
         
-        Which will print out a user's conversation, together with meta information associated with the conversation (i.e. rating and user feedback).
+        Which will print out one of the users' conversation, together with meta information associated with the conversation (i.e. rating and user feedback).
         
-        (Advanced): You can also access the raw feedback data by running
+        To get all the feedback for your model, run...
         
         ```python
-        raw_data = model_feedback.raw_data
+        df = model_feedback.df
+        print(df)
         ```
         
+        This outputs a Pandas `DataFrame`, where each row corresponds to a user conversation with your model, together with their feedback.
         
         **Getting Live Leaderboard**
         
         To see how your model performs against other models, run:
         ```python
-        from chai_guanaco.feedback import display_leaderboard
-        
-        display_leaderboard(developer_key)
+        chai.display_leaderboard()
         ```
         which prints out the current leaderboard, with your models positions highlighted
         
         **Re-Submitting Models**
         
         Because it is a competition, you are allowed to test a single model at any given time. However, you can deactivate a model and submit a new one. To do this, simply run:
         
         ```python
-        from chai_guanaco.submit import deactivate_model
-        
-        deactivate_model(submission_id, developer_key)
+        chai.deactivate_model(submission_id)
         ```
         Which will deactive your model, don't worry, all the model feedback will still be saved, it just means the model will no longer be exposed to users. You can then re-submit by repeating the model submission step.
         
         **Retrieve Your Model Submission IDs**
         
         In case you have forgotten your submission ids / want to view all past submissions, run:
         
         ```python
-        from chai_guanaco.submit import get_my_submissions
-        
-        submission_ids = get_my_submissions(developer_key)
+        submission_ids = chai.get_my_submissions()
         print(submission_ids)
         ```
         Here you will see all your model submission_ids along with their status, which is either `failed`, `inactive` or `deployed`.
         
+        **Advanced Usage**
+        - This package caches various data, such as your developer key, in the folder `~/.chai-guanaco`. To change this, you can set the environment variable `GUANACO_DATA_DIR` to point to a different folder. You may need to re-run `chai-guanaco login` to update the cached developer key.
+        - You can also access the raw feedback data by running
+        	```python
+        	model_feedback = chai.get_feedback(submission_id)
+        	raw_data = model_feedback.raw_data
+        	```
+        
+        
         
         ## Resources
         |                                                                        |                                                                                                 |
         | ---------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------|
         | 📒 [Fine tuning guide](https://huggingface.co/docs/transformers/training) | Guide on language model finetuning                                                           |
         | 💾 [Datasets](https://dataset-ideas.tiiny.site/) | Curated list of open-sourced datasets to get started with finetuning                                                  |
-        | 💖 [Guanaco Discord](https://haystack.deepset.ai/tutorials)                   | Our Guanaco competition discord                                                          |
+        | 💖 [Guanaco Discord](https://discord.gg/7mXdjAkw2s)                   | Our Guanaco competition discord                                                          |
         |🚀 [Deepspeed Guide](https://huggingface.co/docs/transformers/main_classes/deepspeed)     | Guide for training with Deepspeed (faster training without GPU bottleneck)    |
         |💬 [Example Conversations](https://huggingface.co/docs/transformers/main_classes/deepspeed)     | Here you can find 1000 example conversations from the Chai Platform     |
         | ⚒️ [Build with us](https://boards.greenhouse.io/nexus/jobs/5319721003)| If you think what we are building is cool, join us!|
         
         
         ## 🦙 Hosted & Sponsored By
```

### Comparing `chai-guanaco-1.0.0/README.md` & `chai-guanaco-1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -34,117 +34,114 @@
 ## 🚀 Getting Started
 
 **Getting Developer Key**
 
 Join the [competition discord](https://discord.gg/7mXdjAkw2s), introduce yourself and ask for a developer key. Login-based authentication is coming next 🤗
 
 
-**Submitting A Model**
+**Installation**
 
 Use [pip](https://github.com/pypa/pip) to install the Chai Guanaco package
 
 ```sh
 pip install chai-guanaco
 ```
 
+For one-off authentication run the following in your terminal:
+
+```sh
+chai-guanaco login
+```
+
+And pass in your developer key when prompted, you can always logout using `chai-guanaco logout`.
+
+**Model Submission**
+
 Upload any GPT-J 6B based language model *with a tokenizer* to huggingface, i.e. [EleutherAI/gpt-j-6b](https://huggingface.co/EleutherAI/gpt-j-6b). Read [this guide](https://huggingface.co/docs/transformers/model_sharing) if you are unsure. Click the *Use in Transformers* button in huggingface to get the your huggingface model ID (i.e. "EleutherAI/gpt-j-6b")
 
 To submit model simply run:
 
 ```python
-from chai_guanaco.submit import submit_model
+import chai_guanaco as chai
 
 model_url = "EleutherAI/gpt-j-6b" # Your model URL
-developer_key = "CR_XXXX" # Your developer key
+
 generation_params = {'temperature': 0.75, 'repetition_penalty': 1.13, 'top_p': 0, "top_k": 0}
 submission_parameters = {'model_repo': model_url, 'generation_params': generation_params}
-response = submit_model(submission_parameters, developer_key)
-submission_id = response['submission_id']
-print(submission_id)
-````
-which outputs your submission id, unique to your model submission.
-
-To verify the status of a submission, you can use the following command:
 
-```python
-from chai_guanaco.submit import get_model_info
+submitter = chai.ModelSubmitter()
+submission_id = submitter.submit(submission_parameters)
+````
 
-model_info = get_model_info(submission_id, developer_key)
-print(model_info)
-```
-Once the `status` field shows `success` it means your model has been successfully submitted. A submission typically takes around 10 minutes for the tritonisation process to complete.
+This will display an animation while your model is being deployed, a typical
+deployment takes approximately 10 minutes.
 
 **Getting User Feedback**
 
 Once your model has been submitted, it is automatically deployed to the Chai Platform where real-life users will evaluate your model performance. To view their feedback, run:
 
 ```python
-from chai_guanaco.feedback import get_feedback
-
-model_feedback = get_feedback(submission_id, developer_key)
-print(model_feedback.df)
-```
-
-Here, you will find a pandas dataframe with all the user feedback for your model, including the conversation each user has had with your model.
-
-You can print samples from your model's user feedbacks by running
-
-```python
+model_feedback = chai.get_feedback(submission_id)
 model_feedback.sample()
 ```
 
-Which will print out a user's conversation, together with meta information associated with the conversation (i.e. rating and user feedback).
+Which will print out one of the users' conversation, together with meta information associated with the conversation (i.e. rating and user feedback).
 
-(Advanced): You can also access the raw feedback data by running
+To get all the feedback for your model, run...
 
 ```python
-raw_data = model_feedback.raw_data
+df = model_feedback.df
+print(df)
 ```
 
+This outputs a Pandas `DataFrame`, where each row corresponds to a user conversation with your model, together with their feedback.
 
 **Getting Live Leaderboard**
 
 To see how your model performs against other models, run:
 ```python
-from chai_guanaco.feedback import display_leaderboard
-
-display_leaderboard(developer_key)
+chai.display_leaderboard()
 ```
 which prints out the current leaderboard, with your models positions highlighted
 
 **Re-Submitting Models**
 
 Because it is a competition, you are allowed to test a single model at any given time. However, you can deactivate a model and submit a new one. To do this, simply run:
 
 ```python
-from chai_guanaco.submit import deactivate_model
-
-deactivate_model(submission_id, developer_key)
+chai.deactivate_model(submission_id)
 ```
 Which will deactive your model, don't worry, all the model feedback will still be saved, it just means the model will no longer be exposed to users. You can then re-submit by repeating the model submission step.
 
 **Retrieve Your Model Submission IDs**
 
 In case you have forgotten your submission ids / want to view all past submissions, run:
 
 ```python
-from chai_guanaco.submit import get_my_submissions
-
-submission_ids = get_my_submissions(developer_key)
+submission_ids = chai.get_my_submissions()
 print(submission_ids)
 ```
 Here you will see all your model submission_ids along with their status, which is either `failed`, `inactive` or `deployed`.
 
+**Advanced Usage**
+- This package caches various data, such as your developer key, in the folder `~/.chai-guanaco`. To change this, you can set the environment variable `GUANACO_DATA_DIR` to point to a different folder. You may need to re-run `chai-guanaco login` to update the cached developer key.
+- You can also access the raw feedback data by running
+	```python
+	model_feedback = chai.get_feedback(submission_id)
+	raw_data = model_feedback.raw_data
+	```
+
+
 
 ## Resources
 |                                                                        |                                                                                                 |
 | ---------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------|
 | 📒 [Fine tuning guide](https://huggingface.co/docs/transformers/training) | Guide on language model finetuning                                                           |
 | 💾 [Datasets](https://dataset-ideas.tiiny.site/) | Curated list of open-sourced datasets to get started with finetuning                                                  |
-| 💖 [Guanaco Discord](https://haystack.deepset.ai/tutorials)                   | Our Guanaco competition discord                                                          |
+| 💖 [Guanaco Discord](https://discord.gg/7mXdjAkw2s)                   | Our Guanaco competition discord                                                          |
 |🚀 [Deepspeed Guide](https://huggingface.co/docs/transformers/main_classes/deepspeed)     | Guide for training with Deepspeed (faster training without GPU bottleneck)    |
 |💬 [Example Conversations](https://huggingface.co/docs/transformers/main_classes/deepspeed)     | Here you can find 1000 example conversations from the Chai Platform     |
 | ⚒️ [Build with us](https://boards.greenhouse.io/nexus/jobs/5319721003)| If you think what we are building is cool, join us!|
 
 
 ## 🦙 Hosted & Sponsored By
```

### Comparing `chai-guanaco-1.0.0/chai_guanaco.egg-info/PKG-INFO` & `chai-guanaco-1.0.1/chai_guanaco.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chai-guanaco
-Version: 1.0.0
+Version: 1.0.1
 Summary: Chai Guanaco
 Home-page: https://www.chai-research.com
 Author: Chai Research Corp.
 Author-email: hello@chai-research.com
 License: MIT
 Description: [![Guanaco Banner](https://imgur.com/wJHIeAU.png)](https://www.chai-research.com/competition.html)
         
@@ -42,117 +42,114 @@
         ## 🚀 Getting Started
         
         **Getting Developer Key**
         
         Join the [competition discord](https://discord.gg/7mXdjAkw2s), introduce yourself and ask for a developer key. Login-based authentication is coming next 🤗
         
         
-        **Submitting A Model**
+        **Installation**
         
         Use [pip](https://github.com/pypa/pip) to install the Chai Guanaco package
         
         ```sh
         pip install chai-guanaco
         ```
         
+        For one-off authentication run the following in your terminal:
+        
+        ```sh
+        chai-guanaco login
+        ```
+        
+        And pass in your developer key when prompted, you can always logout using `chai-guanaco logout`.
+        
+        **Model Submission**
+        
         Upload any GPT-J 6B based language model *with a tokenizer* to huggingface, i.e. [EleutherAI/gpt-j-6b](https://huggingface.co/EleutherAI/gpt-j-6b). Read [this guide](https://huggingface.co/docs/transformers/model_sharing) if you are unsure. Click the *Use in Transformers* button in huggingface to get the your huggingface model ID (i.e. "EleutherAI/gpt-j-6b")
         
         To submit model simply run:
         
         ```python
-        from chai_guanaco.submit import submit_model
+        import chai_guanaco as chai
         
         model_url = "EleutherAI/gpt-j-6b" # Your model URL
-        developer_key = "CR_XXXX" # Your developer key
+        
         generation_params = {'temperature': 0.75, 'repetition_penalty': 1.13, 'top_p': 0, "top_k": 0}
         submission_parameters = {'model_repo': model_url, 'generation_params': generation_params}
-        response = submit_model(submission_parameters, developer_key)
-        submission_id = response['submission_id']
-        print(submission_id)
-        ````
-        which outputs your submission id, unique to your model submission.
-        
-        To verify the status of a submission, you can use the following command:
         
-        ```python
-        from chai_guanaco.submit import get_model_info
+        submitter = chai.ModelSubmitter()
+        submission_id = submitter.submit(submission_parameters)
+        ````
         
-        model_info = get_model_info(submission_id, developer_key)
-        print(model_info)
-        ```
-        Once the `status` field shows `success` it means your model has been successfully submitted. A submission typically takes around 10 minutes for the tritonisation process to complete.
+        This will display an animation while your model is being deployed, a typical
+        deployment takes approximately 10 minutes.
         
         **Getting User Feedback**
         
         Once your model has been submitted, it is automatically deployed to the Chai Platform where real-life users will evaluate your model performance. To view their feedback, run:
         
         ```python
-        from chai_guanaco.feedback import get_feedback
-        
-        model_feedback = get_feedback(submission_id, developer_key)
-        print(model_feedback.df)
-        ```
-        
-        Here, you will find a pandas dataframe with all the user feedback for your model, including the conversation each user has had with your model.
-        
-        You can print samples from your model's user feedbacks by running
-        
-        ```python
+        model_feedback = chai.get_feedback(submission_id)
         model_feedback.sample()
         ```
         
-        Which will print out a user's conversation, together with meta information associated with the conversation (i.e. rating and user feedback).
+        Which will print out one of the users' conversation, together with meta information associated with the conversation (i.e. rating and user feedback).
         
-        (Advanced): You can also access the raw feedback data by running
+        To get all the feedback for your model, run...
         
         ```python
-        raw_data = model_feedback.raw_data
+        df = model_feedback.df
+        print(df)
         ```
         
+        This outputs a Pandas `DataFrame`, where each row corresponds to a user conversation with your model, together with their feedback.
         
         **Getting Live Leaderboard**
         
         To see how your model performs against other models, run:
         ```python
-        from chai_guanaco.feedback import display_leaderboard
-        
-        display_leaderboard(developer_key)
+        chai.display_leaderboard()
         ```
         which prints out the current leaderboard, with your models positions highlighted
         
         **Re-Submitting Models**
         
         Because it is a competition, you are allowed to test a single model at any given time. However, you can deactivate a model and submit a new one. To do this, simply run:
         
         ```python
-        from chai_guanaco.submit import deactivate_model
-        
-        deactivate_model(submission_id, developer_key)
+        chai.deactivate_model(submission_id)
         ```
         Which will deactive your model, don't worry, all the model feedback will still be saved, it just means the model will no longer be exposed to users. You can then re-submit by repeating the model submission step.
         
         **Retrieve Your Model Submission IDs**
         
         In case you have forgotten your submission ids / want to view all past submissions, run:
         
         ```python
-        from chai_guanaco.submit import get_my_submissions
-        
-        submission_ids = get_my_submissions(developer_key)
+        submission_ids = chai.get_my_submissions()
         print(submission_ids)
         ```
         Here you will see all your model submission_ids along with their status, which is either `failed`, `inactive` or `deployed`.
         
+        **Advanced Usage**
+        - This package caches various data, such as your developer key, in the folder `~/.chai-guanaco`. To change this, you can set the environment variable `GUANACO_DATA_DIR` to point to a different folder. You may need to re-run `chai-guanaco login` to update the cached developer key.
+        - You can also access the raw feedback data by running
+        	```python
+        	model_feedback = chai.get_feedback(submission_id)
+        	raw_data = model_feedback.raw_data
+        	```
+        
+        
         
         ## Resources
         |                                                                        |                                                                                                 |
         | ---------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------|
         | 📒 [Fine tuning guide](https://huggingface.co/docs/transformers/training) | Guide on language model finetuning                                                           |
         | 💾 [Datasets](https://dataset-ideas.tiiny.site/) | Curated list of open-sourced datasets to get started with finetuning                                                  |
-        | 💖 [Guanaco Discord](https://haystack.deepset.ai/tutorials)                   | Our Guanaco competition discord                                                          |
+        | 💖 [Guanaco Discord](https://discord.gg/7mXdjAkw2s)                   | Our Guanaco competition discord                                                          |
         |🚀 [Deepspeed Guide](https://huggingface.co/docs/transformers/main_classes/deepspeed)     | Guide for training with Deepspeed (faster training without GPU bottleneck)    |
         |💬 [Example Conversations](https://huggingface.co/docs/transformers/main_classes/deepspeed)     | Here you can find 1000 example conversations from the Chai Platform     |
         | ⚒️ [Build with us](https://boards.greenhouse.io/nexus/jobs/5319721003)| If you think what we are building is cool, join us!|
         
         
         ## 🦙 Hosted & Sponsored By
```

### Comparing `chai-guanaco-1.0.0/setup.py` & `chai-guanaco-1.0.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 from pathlib import Path
 import os
 from setuptools import find_packages, setup
 
 current_dir = Path(__file__).parent
 long_description = (current_dir / "README.md").read_text()
 
+with open('requirements.txt') as f:
+    requirements = f.read().splitlines()
+
 if os.environ.get('CI_COMMIT_TAG', None):
     version = os.environ['CI_COMMIT_TAG']
 else:
-    version = "1.0.0"
+    version = "1.0.1"
 
 setup(
     name='chai-guanaco',
     version=version,
     description='Chai Guanaco',
     author='Chai Research Corp.',
     author_email='hello@chai-research.com',
     license='MIT',
     packages=["chai_guanaco"],
     package_dir={"chai_guanaco": "./src/chai_guanaco/"},
     url='https://www.chai-research.com',
     zip_safe=False,
     long_description=long_description,
     long_description_content_type='text/markdown',
-    install_requires=['requests']
+    install_requires=requirements,
+    entry_points={
+        'console_scripts': ['chai-guanaco = chai_guanaco.login_cli:cli'],
+    },
 )
```

### Comparing `chai-guanaco-1.0.0/src/chai_guanaco/feedback.py` & `chai-guanaco-1.0.1/src/chai_guanaco/feedback.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import requests
 
 import pandas as pd
 
+from chai_guanaco.utils import print_color
+from chai_guanaco.login_cli import auto_authenticate
+
 
 BASE_URL = "https://guanaco-feedback.chai-research.com"
 FEEDBACK_ENDPOINT = "/feedback/{submission_id}"
 
 FEEDBACK_URL = BASE_URL + FEEDBACK_ENDPOINT
 
 
@@ -22,27 +25,22 @@
     def sample(self):
         df = self.df
         single_row = df.sample()
         self.pprint_row(single_row)
 
     def pprint_row(self, row):
         data = row.to_dict(orient='records')[0]
-        self._print_color('### Conversation ###', 'yellow')
+        print_color('### Conversation ###', 'yellow')
         print(data['conversation'])
-        self._print_color('###', 'yellow')
+        print_color('###', 'yellow')
         thumbs_up = "👍" if data['thumbs_up'] else "👎"
-        self._print_color(f'Feedback {thumbs_up}: {data["feedback"]}', 'green')
-        self._print_color(f'Conversation ID: {data["conversation_id"]}', 'blue')
-        self._print_color(f'User ID: {data["user_id"]}', 'blue')
-        self._print_color(f'Bot ID: {data["bot_id"]}', 'blue')
-
-    def _print_color(self, text, color):
-        colors = {'blue': '\033[94m', 'cyan': '\033[96m', 'green': '\033[92m', 'yellow': '\033[93m'}
-        assert color in colors.keys()
-        print(f'{colors[color]}{text}\033[0m')
+        print_color(f'Feedback {thumbs_up}: {data["feedback"]}', 'green')
+        print_color(f'Conversation ID: {data["conversation_id"]}', 'blue')
+        print_color(f'User ID: {data["user_id"]}', 'blue')
+        print_color(f'Bot ID: {data["bot_id"]}', 'blue')
 
     def _extract_feedback_as_rows(self, feedback):
         rows = [self._extract_feedback_data(cid, data) for cid, data in feedback.items()]
         return rows
 
     def _extract_feedback_data(self, convo_id, message_data):
         convo = self._extract_conversation_from_messages(message_data['messages'])
@@ -81,15 +79,16 @@
     def _get_sender_tag(self, message):
         sender = message['sender']['name'].strip()
         if message['deleted']:
             sender = f'{sender} (deleted)'
         return sender
 
 
-def get_feedback(submission_id: str, developer_key: str):
+@auto_authenticate
+def get_feedback(submission_id: str, developer_key=None):
     headers = {
         "developer_key": developer_key,
     }
     url = FEEDBACK_URL.format(submission_id=submission_id)
     resp = requests.get(url, headers=headers)
     assert resp.status_code == 200, resp.json()
     feedback = Feedback(resp.json())
```

### Comparing `chai-guanaco-1.0.0/tests/test_feedback.py` & `chai-guanaco-1.0.1/tests/test_feedback.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.0/tests/test_submit.py` & `chai-guanaco-1.0.1/tests/test_submit.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,15 +13,24 @@
         yield func
 
 
 @pytest.fixture(autouse="session")
 def mock_get():
     with patch("chai_guanaco.submit.requests.get") as func:
         func.return_value.status_code = 200
-        func.return_value.json.return_value = {"name_123456": {'status': 'pending'}}
+        func.return_value.json.return_value = {'name_123456': {'status': 'pending'}}
+        yield func
+
+
+@pytest.fixture()
+def mock_get_pending_to_success():
+    responses = [{'status': 'pending'}] * 2 + [{'status': 'deployed'}]
+    with patch("chai_guanaco.submit.requests.get") as func:
+        func.return_value.status_code = 200
+        func.return_value.json.side_effect = responses
         yield func
 
 
 @pytest.fixture()
 def mock_submission():
     submission = {
         "model_repo": "ChaiML/test_model",
@@ -32,14 +41,25 @@
             "repetition_penalty": 1.0,
         },
         "formatter": "PygmalionFormatter",
     }
     return submission
 
 
+def test_model_submitter(mock_submission, mock_post, mock_get_pending_to_success):
+    model_submitter = submit.ModelSubmitter("mock-key")
+    model_submitter._sleep_time = 0
+    model_submitter._get_request_interval = 1
+    submission_id = model_submitter.submit(mock_submission)
+    headers = {"Authorization": "Bearer mock-key"}
+    mock_post.assert_called_once_with(url=submit.SUBMISSION_URL, json=mock_submission, headers=headers)
+    assert mock_get_pending_to_success.call_count == 3
+    assert submission_id == "name_123456"
+
+
 def test_client(mock_post, mock_submission):
     response = submit.submit_model(mock_submission, developer_key="mock-key")
     expected_submission_id = "name_123456"
     assert response == {"submission_id": expected_submission_id}
 
 
 def test_submit_client_posts_with_correct_payload(mock_post, mock_submission):
```

