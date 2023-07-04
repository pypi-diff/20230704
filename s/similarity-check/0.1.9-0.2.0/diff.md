# Comparing `tmp/similarity_check-0.1.9.tar.gz` & `tmp/similarity_check-0.2.0.tar.gz`

## Comparing `similarity_check-0.1.9.tar` & `similarity_check-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 similarity_check-0.1.9/setup.cfg
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 similarity_check-0.1.9/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 similarity_check-0.1.9/src/similarity_check/__init__.py
--rw-r--r--   0        0        0    23554 2020-02-02 00:00:00.000000 similarity_check-0.1.9/src/similarity_check/checkers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 similarity_check-0.1.9/LICENSE
--rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 similarity_check-0.1.9/README.md
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 similarity_check-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     8984 2020-02-02 00:00:00.000000 similarity_check-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 similarity_check-0.2.0/setup.cfg
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 similarity_check-0.2.0/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 similarity_check-0.2.0/src/similarity_check/__init__.py
+-rw-r--r--   0        0        0    23682 2020-02-02 00:00:00.000000 similarity_check-0.2.0/src/similarity_check/checkers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 similarity_check-0.2.0/LICENSE
+-rw-r--r--   0        0        0     8984 2020-02-02 00:00:00.000000 similarity_check-0.2.0/README.md
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 similarity_check-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     9312 2020-02-02 00:00:00.000000 similarity_check-0.2.0/PKG-INFO
```

### Comparing `similarity_check-0.1.9/setup.cfg` & `similarity_check-0.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 696d 696c 6172 6974 795f 6368   = similarity_ch
 00000020: 6563 6b0d 0a64 6573 6372 6970 7469 6f6e  eck..description
 00000030: 203d 2070 6163 6b61 6765 2066 6f72 206d   = package for m
 00000040: 6561 7375 7269 6e67 2074 6865 2073 696d  easuring the sim
 00000050: 696c 6172 6974 7920 6f66 2074 776f 2074  ilarity of two t
 00000060: 6578 7473 0d0a 7665 7273 696f 6e20 3d20  exts..version = 
-00000070: 302e 312e 390d 0a6c 6f6e 675f 6465 7363  0.1.9..long_desc
+00000070: 302e 322e 300d 0a6c 6f6e 675f 6465 7363  0.2.0..long_desc
 00000080: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
 00000090: 5245 4144 4d45 2e6d 640d 0a6c 6f6e 675f  README.md..long_
 000000a0: 6465 7363 7269 7074 696f 6e5f 636f 6e74  description_cont
 000000b0: 656e 745f 7479 7065 203d 2074 6578 742f  ent_type = text/
 000000c0: 6d61 726b 646f 776e 0d0a 6175 7468 6f72  markdown..author
 000000d0: 203d 206d 6573 6861 7269 0d0a 6175 7468   = meshari..auth
 000000e0: 6f72 5f65 6d61 696c 203d 206d 6573 6861  or_email = mesha
```

### Comparing `similarity_check-0.1.9/src/similarity_check/checkers.py` & `similarity_check-0.2.0/src/similarity_check/checkers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,28 @@
-from typing import Union, List
+from typing import Union, List, Optional, Dict
 from nltk.stem import PorterStemmer
 import numpy as np
 import pandas as pd
 from nltk.corpus import stopwords
 from nltk import download
 from gensim.models import KeyedVectors
 import gensim.downloader as api
 from sentence_transformers import SentenceTransformer, util, InputExample, losses, models
 from string import punctuation
 from nltk.stem import PorterStemmer
 from nltk.stem.isri import ISRIStemmer
 from tqdm import tqdm
 from collections import Counter
+from huggingface_hub.utils._errors import HTTPError
 download('stopwords')
-
-
-def preprocess(sentence: str, remove_punct: bool, remove_stop_words: bool, stemm: bool, lang: str='en') -> str: 
-    if lang.lower() == 'en':
-        ps = PorterStemmer()
-        # remove punctuations
-        if not remove_punct:
-            sentence = sentence.translate(str.maketrans('', '', punctuation))
-        # remove stop words and stem
-        if remove_stop_words and stemm:
-            stop_words = stopwords.words('english')
-            return ' '.join([ps.stem(w) for w in sentence.lower().split() if w not in stop_words])
-        # stem only
-        elif not remove_stop_words and stemm:
-            return ' '.join([ps.stem(w) for w in sentence.lower().split()])
-        else:
-            # lower case and remove extra white spaces
-            return ' '.join([w for w in sentence.lower().split()])
-    elif lang.lower() == 'ar':
-        st = ISRIStemmer()
-        # remove punctuations
-        if not remove_punct:
-            sentence = sentence.translate(str.maketrans('', '', punctuation))
-        # remove stop words and stem
-        if remove_stop_words and stemm:
-            download('stopwords')
-            stop_words = stopwords.words('arabic')
-            return ' '.join([st.stem(w) for w in sentence.lower().split() if w not in stop_words])
-        # stem only
-        elif not remove_stop_words and stemm:
-            return ' '.join([st.stem(w) for w in sentence.lower().split()])
-        else:
-            # lower case and remove extra white spaces
-            return ' '.join([w for w in sentence.lower().split()])
-    else:
-        raise Exception('non recognized language please specify either en|ar')
         
 
 def preprocess(sentence: str, remove_punct: bool, remove_stop_words: bool, stemm: bool, lang: str='en') -> str: 
+    # print(sentence)
+    sentence = str(sentence) # ensure all sentences are string, even if they are some texts with number only
     if lang.lower() == 'en':
         ps = PorterStemmer()
         # remove punctuations
         if remove_punct:
             sentence = sentence.translate(str.maketrans('', '', punctuation))
         # remove stop words and stem
         if remove_stop_words and stemm:
@@ -87,55 +54,67 @@
         raise Exception('non recognized language please specify either en|ar')
 
     
 class sentence_tranformer_checker():
     def __init__(
         self, 
         targets: Union[List[str], pd.DataFrame], 
-        target_group: Union[List[str], pd.DataFrame]=None,
-        target_col: str=None, 
-        device: str = None,
-        model: SentenceTransformer=None, 
-        lang: str='en', 
-        only_include: List[str]=None,
-        encode_batch = 32,
-        encode_target = True,
-        remove_punct: bool=True, 
-        remove_stop_words: bool=True, 
-        stemm: bool=False
+        target_group: Optional[Union[List[str], pd.DataFrame]]=None,
+        target_cols: Optional[List[str]]=None, 
+        device: Optional[str] = None,
+        model: Optional[str]=None, 
+        lang: Optional[str]='en', 
+        only_include: Optional[List[str]]=None,
+        encode_batch: Optional[int] = 32,
+        encode_target: Optional[bool] = True,
+        show_prograss: Optional[bool] = False,
+        remove_punct: Optional[bool]=True, 
+        remove_stop_words: Optional[bool]=True, 
+        stemm: Optional[bool]=False
     ):    
         """
         parameters:
             targets: dataframe or list of targets text to compare with.
             target_group (optional): goups ids for the target to match only a single target for each group, can either provide list of ids,
             or the column name in the target dataframe.
-            target_col (partially optional): the target column name used to match, *must be specified for dataframe matching*.
+            target_cols (partially optional): the target column names used to match, *must be specified for dataframe matching*.
             device: the device to do the encoding on operations in (cpu|cuda),
-            model (optional): a sentence tranformer model object, to use instead of the default one, for more [details](https://www.sbert.net/).
+            model (optional): a string of the sentence tranformer model, to use instead of the default one, for more [details](https://www.sbert.net/).
             lang (optional): the languge of the model ('en'|'ar').
             only_include (optional): used only for dataframe matching, allow providing a list of column names to only include for the target matches, provide empty list to get only target_col.
             encode_batch (optional): the number of sentences to encode in a batch.
             encode_target: boolean flag to indicate whatever to enocde the targets when initilizing the object (to cache target encoding).
             remove_punct: boolean flag to indicate whatever to remove punctuations. 
             remove_stop_words: boolean flag to indicate whatever to remove stop words.
             stemm: boolean flag to indicate whatever to do stemming.
         """
 
         self.encode_batch = encode_batch
         self.remove_punct = remove_punct
         self.remove_stop_words = remove_stop_words
         self.stemm = stemm
         self.lang = lang 
-        self.device = device.lower()
+        self.show_prograss = show_prograss
+
+        if isinstance(target_cols, str):
+            target_cols = [target_cols]
+            
+        if device is None:
+            self.device = None
+        else:
+            self.device = device.lower()
 
         if isinstance(targets, pd.DataFrame):
-            self.use_frames = True
-    
-            if target_col not in targets.columns:
-                raise KeyError('target_col not found in target DataFrame cloumns')
+            targets = targets.copy(deep=True)
+
+            for target_col in target_cols:
+                if target_col not in targets.columns:
+                    raise KeyError('target_col not found in target DataFrame cloumns')
+                else:
+                    targets.loc[:, target_col] = targets[target_col].fillna('')
 
             if target_group is not None:
                 if isinstance(target_group, str):
                     if target_group not in targets.columns:
                         raise KeyError('target_group not found in target DataFrame cloumns')
                     self.group_ids = targets[target_group].tolist()
                 else:
@@ -143,257 +122,253 @@
             else:
                 self.group_ids = None
                 
             if only_include is not None:
                 for col_name in only_include:
                     if col_name not in targets.columns:       
                         raise KeyError(f'only_include value:({col_name}) not found not found in target DataFrame cloumns')    
-                only_include.insert(0, target_col)
+                for target_col in target_cols:
+                    only_include.insert(0, target_col)
                 
                 targets = targets.loc[:, only_include]
+                
 
             self.target_df = targets.reset_index(drop=True)
-            self.target_names = [preprocess(sent, self.remove_punct, self.remove_stop_words, self.stemm, self.lang) for sent in targets[target_col].tolist()]
-        else:
+            self.targets = {target_col: [preprocess(sent, self.remove_punct, self.remove_stop_words, self.stemm, self.lang) for sent in targets[target_col].tolist()] for target_col in target_cols}
+        elif isinstance(targets, list):
             if isinstance(target_group, list):
                 self.group_ids = target_group
             else:
                 if target_group is None:
                     self.group_ids = target_group
                 else:
-                    raise TypeError('if target are a list entered groups must also be a list')
+                    raise TypeError('if target are a list, provided groups must also be a list')
         
             if not targets:
                 raise TypeError('Targets are empty') 
 
-            self.use_frames = False
-            self.target_names = [preprocess(sent, self.remove_punct, self.remove_stop_words, self.stemm, self.lang) for sent in targets]
-
-        if pd.isnull(self.target_names).any():
-            raise ValueError('Targets contain null values')
+            self.target_df = pd.DataFrame({'target': targets})
+            self.targets = {'target': [preprocess(sent, self.remove_punct, self.remove_stop_words, self.stemm, self.lang) for sent in targets]}
+        else:
+            msg = f'targets must be a dataframe or a list, instead a source of type {str(type(targets))} was passed'
+            raise TypeError(msg)
 
-        self.model = model
-        self.model.device = device
+        # for target in self.targets.values():
+        #     if pd.isnull(target).any():
+        #         raise ValueError('Targets contain null values')
+
+        if model is not None:
+            try:
+                self.model = SentenceTransformer(model, device=self.device)
+            except HTTPError:
+                raise HTTPError('entered model name is not defined')
         # if no model is provided use the default model
-        if model is None:
-            print('initializing the model...')
+        else:
+            if self.show_prograss:
+                print('initializing the model...')
             if lang.lower() == 'en':
-                self.model = SentenceTransformer('all-MiniLM-L6-v2', device=device)
-                print('done...')
+                self.model = SentenceTransformer('all-MiniLM-L6-v2', device=self.device)
+                if self.show_prograss:
+                    print('done...')
             else:
-                self.model = SentenceTransformer('distiluse-base-multilingual-cased-v1', device=device)
-                print('done...')
-
+                self.model = SentenceTransformer('distiluse-base-multilingual-cased-v1', device=self.device)
+                if self.show_prograss:
+                    print('done...')
+    
         if encode_target:  
-            print('enocding targets: ')
-            self.encoded_targets = self.model.encode(self.target_names, batch_size=self.encode_batch, show_progress_bar=True,  normalize_embeddings=True) # encode the targets
+            if self.show_prograss:
+                print('enocding targets: ')
+            self.encoded_targets = {(k): (self.model.encode(v, batch_size=self.encode_batch, show_progress_bar=self.show_prograss,  normalize_embeddings=True)) for k, v in self.targets.items()} # encode the targets
 
 
-    # used to make sure that if the object targets are updated, the cached targets are deleted
+
+    # used to make sure that if the object targets are updated, the cached targets embeddings are deleted
     def __setattr__(self, key, value):
         # self.key = value
-        if key == 'target_names' or key == 'target_df':
+        if key == 'targets' or key == 'target_df':
             if hasattr(self, 'encoded_targets'):
                 del self.encoded_targets     
         super().__setattr__(key, value)
 
 
     def match(
         self, 
         source: Union[List[str], pd.DataFrame], 
-        source_col: str=None, 
-        topn: int=1, 
-        return_match_idx: bool=False, 
-        threshold: float=0.5, 
-        batch_size: int=128
+        source_mapping: Optional[Union[str, List]]=None, 
+        topn: Optional[int]=1, 
+        threshold: Optional[float]=0.5, 
+        batch_size: Optional[int]=128
     ) -> pd.DataFrame:
         '''
         Main match function. return only the top candidate for every source string.
         parameters:
             source: dataframe or list of input texts to find closest match for.
-            source_col (partially optional): the source column name used to match, *must be specified for dataframe matching*.
+            source_mapping (partially optional) *must be specified for dataframe matching*: a list with each element being a tuple with the following three values (the target column name, source column name, the weight for this match), if a string is passed it and one target was only passed it will be mapped to the that target, with a the full weight of 1.0, note that the the overall weights must equal 1.0.
             topn: number of matches to return.
             threshold: the lowest threeshold to ignore matches below it.
-            return_match_idx: return an extra column for each match containing the index of the match within the target_names.
             batch_size: the size of the batch in inputs to match with targets (to limit space usage).
         returns:
-            a data frame with 3 columns (source, target, score), and two extra columns for each extra match (target_2, score_2 ...), and an optional extra column for each match containg the match index, if return_match_idxs set to True.
+            a data frame with 3 columns (source, target, score), and two extra columns for each extra match (target_2, score_2 ...)
         ''' 
         if isinstance(source, pd.DataFrame) and not hasattr(self, 'target_df'):
-            raise TypeError('if target is a dataframe source must also be a dataframe')
+            msg = 'if target is a dataframe source must also be a dataframe'
+            raise TypeError(msg)
 
-        if isinstance(source, list) and hasattr(self, 'target_df'):
-            source = pd.DataFrame({source_col: source})
+        if len(self.targets) == 1 and isinstance(source_mapping, str):
+            source_mapping = [(list(self.targets.keys())[0], source_mapping, 1)]
 
         if isinstance(source, pd.DataFrame):
-            self.use_frames = True
-    
-            if source_col not in source.columns:
-                raise KeyError('source_col not found in source DataFrame cloumns')
+            source = source.copy(deep=True)
 
+            overall_weight = 0.0
+            for _, source_col, weight in source_mapping:
+                if source_col not in source.columns:
+                    msg = f'the following source_col ({source_col}) not found in source DataFrame cloumns'
+                    raise KeyError(msg)
+                else:
+                    source.loc[:, source_col] = source.fillna('')
+                overall_weight += weight
+                
+            if overall_weight != 1.0:
+                msg = f'the sum of the provided weights must equal 1.0, the provided weights sum is: {overall_weight}'
+                raise ValueError(msg)
+            
             self.source_df = source.reset_index(drop=True)
-            self.source_names = [preprocess(sent, self.remove_punct, self.remove_stop_words, self.stemm, self.lang) for sent in source[source_col].tolist()]
+            sources = {source_col: [preprocess(sent, self.remove_punct, self.remove_stop_words, self.stemm, self.lang) for sent in source[source_col].tolist()] for _, source_col, __ in source_mapping}
+        elif isinstance(source, list):
+            source = pd.DataFrame({'source': source})
+            self.source_df = source
+            if not source_mapping:
+                if len(self.targets) > 1:
+                    msg = 'there are multiple target columns to map with the source, please provide a costume source_mapping, or adjust the target columns to one specific columns'
+                    raise ValueError(msg)
+                source_mapping = [(list(self.targets.keys())[0], 'source', 1)]
+            sources = {source_col: [preprocess(sent, self.remove_punct, self.remove_stop_words, self.stemm, self.lang) for sent in source[source_col].tolist()] for _, source_col, __ in source_mapping}
         else:
-            if not source:
-                raise TypeError('Inputs are empty')
-
-            self.use_frames = False
-            self.source_names = [preprocess(sent, self.remove_punct, self.remove_stop_words, self.stemm, self.lang) for sent in source]
+            msg = f'source must be a dataframe or a list, instead a source of type {str(type(source))} was passed'
+            raise TypeError(msg)
+        # else:
+        #     self.source_df = pd.DataFrame({'source': source})
+        #     sources = {'source': [preprocess(sent, self.remove_punct, self.remove_stop_words, self.stemm, self.lang) for sent in source]}
 
         if not hasattr(self, 'encoded_targets'):
-            print('enocding targets: ')
-            encoded_targets = self.model.encode(self.target_names, batch_size=self.encode_batch, show_progress_bar=True,  normalize_embeddings=True) # encode the targets
+            if self.show_prograss:
+                print('enocding targets: ')
+            encoded_targets = {(k): (self.model.encode(v, batch_size=self.encode_batch, show_progress_bar=self.show_prograss,  normalize_embeddings=True)) for k, v in self.targets.items()} # encode the targets
         else:
             encoded_targets = self.encoded_targets
 
-        targets = np.full((len(self.source_names), topn), None)
-        top_cosine = np.full((len(self.source_names), topn), None)
-        match_idxs = np.full((len(self.source_names), topn), None)
-
-        print('matching prograss:')
-        for i in tqdm(range(0, len(self.source_names), batch_size)):
-            encoded_inputs = self.model.encode(self.source_names[i:i+batch_size], batch_size=self.encode_batch, normalize_embeddings=True) # encode the inputs
+        inputs_length = len(list(sources.values())[0])
+        targets_length = len(list(self.targets.values())[0])
 
-            batch_targets, batch_top_cosine, batch_match_idxs = self.max_cosine_sim(encoded_inputs, encoded_targets , topn, threshold)
-            targets[i:i+batch_size, :] = batch_targets
+        top_cosine = np.full((inputs_length, topn), None)
+        match_idxs = np.full((inputs_length, topn), None)
+
+        if self.show_prograss:
+            print('matching prograss:')
+
+        for i in tqdm(range(0, inputs_length, batch_size), disable=(not self.show_prograss)):
+            encoded_inputs = {(k): (self.model.encode(v[i:i+batch_size], batch_size=self.encode_batch, normalize_embeddings=True)) for k, v in sources.items()} # encode the inputs
+            batch_inputs_length = len(list(encoded_inputs.values())[0])
+            # encoded_inputs = self.model.encode(self.source_names[i:i+batch_size], batch_size=self.encode_batch, normalize_embeddings=True) # encode the inputs
+    
+            batch_top_cosine, batch_match_idxs = self.max_cosine_sim(encoded_inputs, encoded_targets, source_mapping , topn, threshold, batch_inputs_length, targets_length)
             top_cosine[i:i+batch_size, :] = batch_top_cosine
             match_idxs[i:i+batch_size, :] = batch_match_idxs
         
-        match_output = self._make_matchdf(targets, top_cosine, match_idxs, topn, return_match_idx)
+        match_output = self._make_matchdf(top_cosine, match_idxs, inputs_length)
 
         return match_output
 
 
-    def max_cosine_sim(self, encoded_inputs, encoded_targets,  topn, threshold):
-        if len(encoded_inputs.shape) == 1:
-            a = a.unsqueeze(0)
+    def max_cosine_sim(self, encoded_inputs, encoded_targets, source_mapping, topn, threshold, inputs_length, targets_length):
+        scores = np.zeros((inputs_length, targets_length), dtype=np.float32) # initialize with zeros
+  
+        for combinition_target, combinition_input, weight in source_mapping:
+            if len(encoded_inputs[combinition_input].shape) == 1:
+                encoded_inputs[combinition_input] = np.expand_dims(encoded_inputs[combinition_input], axis=0)
 
-        if len(encoded_targets.shape) == 1:
-            b = b.unsqueeze(0)
+            if len(encoded_targets[combinition_target].shape) == 1:
+                encoded_targets[combinition_target] = np.expand_dims(encoded_targets[combinition_target], axis=0)
 
-        scores = np.matmul(encoded_inputs, encoded_targets.T)
+            scores += np.matmul(encoded_inputs[combinition_input], encoded_targets[combinition_target].T) * weight
 
         if self.group_ids is None:
-            max_matches = min((len(self.target_names)-1, topn))
+            max_matches = min((targets_length-1, topn))
         else:
-            max_matches = min((len(self.target_names)-1, topn * Counter(self.group_ids).most_common()[0][1]))
+            max_matches = min((targets_length-1, topn * Counter(self.group_ids).most_common()[0][1]))
         
         top_sorted_idxs = np.argpartition(scores, -max_matches, axis=1)[:, -max_matches:] 
         
         # resort the result as the partition sort doesn't completly sort the result
         for i, idxs in enumerate(top_sorted_idxs):
             top_sorted_idxs[i, :] = top_sorted_idxs[i, np.argsort(-scores[i, idxs])]
 
-        targets = np.full((encoded_inputs.shape[0], topn), None)
-        max_cosines = np.full((encoded_inputs.shape[0], topn), None)
-        match_idxs = np.full((encoded_inputs.shape[0], topn), None)
+        max_cosines = np.full((inputs_length, topn), None)
+        match_idxs = np.full((inputs_length, topn), None)
             
         # loop over top results to extract the index, target, and score for each match
         if self.group_ids is not None:
             for i, row in enumerate(top_sorted_idxs):
                 column_id = 0
                 previous_group_id = float('inf')
                 for highest_score_idx in row:
                     if column_id >= topn or scores[i, highest_score_idx] < threshold:
                         break
                     if self.group_ids[highest_score_idx] == previous_group_id:
                         continue
                     match_idxs[i, column_id] = highest_score_idx
-                    targets[i, column_id] = self.target_names[highest_score_idx]
                     max_cosines[i, column_id] = scores[i, highest_score_idx]
                     
                     column_id += 1
                     previous_group_id = self.group_ids[highest_score_idx]
         else:
             for i, row in enumerate(top_sorted_idxs):
                 column_id = 0
                 for highest_score_idx in row:
                     if column_id >= topn or scores[i, highest_score_idx] < threshold:
                         break
                     match_idxs[i, column_id] = highest_score_idx
-                    targets[i, column_id] = self.target_names[highest_score_idx]
                     max_cosines[i, column_id] = scores[i, highest_score_idx]
                     
                     column_id += 1
-        return targets, max_cosines, match_idxs
+                    
+        return max_cosines, match_idxs
 
 
-    def _make_matchdf(self, targets, top_cosine, match_idxs, topn, return_match_idx)-> pd.DataFrame:
+    def _make_matchdf(self, top_cosine, match_idxs, inputs_length)-> pd.DataFrame:
         ''' Build dataframe for result return '''
-        if self.use_frames:
-            arr_temp = np.full((len(self.source_names), len(self.target_df.columns)+1), None)
+        arr_temp = np.full((inputs_length, len(self.target_df.columns)+1), None)
 
-            for i, (match_idx, score) in enumerate(zip(match_idxs.T[0], top_cosine.T[0])):
+        for i, (match_idx, score) in enumerate(zip(match_idxs.T[0], top_cosine.T[0])):
+            if match_idx in self.target_df.index:
+                    temp = self.target_df.iloc[match_idx].tolist()
+                    temp.insert(0, score)
+                    arr_temp[i, :] = temp
+
+        cols = self.target_df.columns.tolist() 
+        cols.insert(0, 'score_1')
+        match_df= pd.DataFrame(arr_temp, columns=cols)
+
+        # concat targets matches into one dataframe
+        for match_num in range(1, len(match_idxs.T)):
+            arr_temp = np.full((inputs_length, len(self.target_df.columns)+1), None)
+            for i, (match_idx, score) in enumerate(zip(match_idxs.T[match_num], top_cosine.T[match_num])):
                 if match_idx in self.target_df.index:
-                     temp = self.target_df.iloc[match_idx].tolist()
-                     temp.insert(0, score)
-                     arr_temp[i, :] = temp
+                    temp = self.target_df.iloc[match_idx].tolist()
+                    temp.insert(0, score)
+                    arr_temp[i, :] = temp
 
             cols = self.target_df.columns.tolist() 
-            cols.insert(0, 'score_1')
-            match_df= pd.DataFrame(arr_temp, columns=cols)
-
-            # concat targets matches into one dataframe
-            for match_num in range(1, len(match_idxs.T)):
-                arr_temp = np.full((len(self.source_names), len(self.target_df.columns)+1), None)
-                for i, (match_idx, score) in enumerate(zip(match_idxs.T[match_num], top_cosine.T[match_num])):
-                    if match_idx in self.target_df.index:
-                        temp = self.target_df.iloc[match_idx].tolist()
-                        temp.insert(0, score)
-                        arr_temp[i, :] = temp
-
-                cols = self.target_df.columns.tolist() 
-                cols.insert(0, f'score_{match_num+1}')
-                df_temp= pd.DataFrame(arr_temp, columns=cols)
-                match_df = match_df.merge(df_temp, left_index=True, right_index=True, suffixes=(f'_{match_num}', f'_{match_num+1}'))
-
-            # merge matches with source
-            match_df = self.source_df.reset_index(drop=True).merge(match_df, left_index=True, right_index=True, suffixes=(f'_source', f'_target'))
-        elif not return_match_idx:
-            match_list = []
-
-            for source, top_scores, targets in zip(self.source_names, top_cosine, targets):
-                row = []
-                row.append(source)
-                # loop over results of multi matches
-                for top_score, target in zip(top_scores, targets):
-                    row.append(top_score)
-                    row.append(target)
-
-                match_list.append(tuple(row))
-
-            # prepare columns names
-            colnames = ['source', 'score', 'prediction']
-            
-            for i in range(2, topn+1):
-                colnames.append(f'score_{i}')
-                colnames.append(f'prediction_{i}')
-                
-            match_df = pd.DataFrame(match_list, columns=colnames)
-        else:
-            match_list = []
-            for source, top_scores, targets, match_idxs in zip(self.source_names, top_cosine, targets, match_idxs):
-                row = []
-                row.append(source)
-                # loop over results of multi matches
-                for top_score, target, match_idx in zip(top_scores, targets, match_idxs):
-                    row.append(top_score) 
-                    row.append(target)
-                    row.append(match_idx)
-                match_list.append(tuple(row))
-
-            # prepare columns names
-            colnames = ['source', 'score', 'prediction', 'match_idx']
-            
-            for i in range(2, topn+1):
-                colnames.append(f'score_{i}')
-                colnames.append(f'prediction_{i}')
-                colnames.append(f'match_idx_{i}')
+            cols.insert(0, f'score_{match_num+1}')
+            df_temp= pd.DataFrame(arr_temp, columns=cols)
+            match_df = match_df.merge(df_temp, left_index=True, right_index=True, suffixes=(f'_{match_num}', f'_{match_num+1}'))
 
-            match_df = pd.DataFrame(match_list, columns=colnames)  
+        # merge matches with source
+        match_df = self.source_df.reset_index(drop=True).merge(match_df, left_index=True, right_index=True, suffixes=(f'_source', f'_target'))
 
         return match_df
 
 
 class word_mover_distance():
     def __init__(self, source_names, target_names, model):
         if not source_names:
```

### Comparing `similarity_check-0.1.9/README.md` & `similarity_check-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -11,57 +11,56 @@
 ```
 
 ## Usage
 ### sentence tranformer
 #### documentation
 * sentence_tranformer(
         targets: Union[List[str], pd.DataFrame], 
-        target_group: Union[List[str], pd.DataFrame]=None,
-        target_col: str=None, 
-        device: str = None,
-        model: SentenceTransformer=None, 
-        lang: str='en', 
-        only_include: List[str]=None,
-        encode_batch = 32,
-        encode_target = True,
-        remove_punct: bool=True, 
-        remove_stop_words: bool=True, 
-        stemm: bool=False
+        target_group: Optional[Union[List[str], pd.DataFrame]]=None,
+        target_cols: Optional[str]=None, 
+        device: Optional[str] = None,
+        model: Optional[str]=None, 
+        lang: Optional[str]='en', 
+        only_include: Optional[List[str]]=None,
+        encode_batch: Optional[int] = 32,
+        encode_target: Optional[bool] = True,
+        remove_punct: Optional[bool]=True, 
+        remove_stop_words: Optional[bool]=True, 
+        stemm: Optional[bool]=False
   ):
   * parameters:
     * targets: dataframe or list of targets text to compare with.
     * target_group (optional): goups ids for the target to match only a single target for each group, can either provide list of ids,
     * or the column name in the target dataframe.
-    * target_col (partially optional): the target column name used to match, *must be specified for dataframe matching*.
+    * target_cols (partially optional): the target column names used to match, *must be specified for dataframe matching*.
     * device: the device to do the encoding on operations in (cpu|cuda),
-    * model (optional): a sentence tranformer model object, to use instead of the default one, for more [details](https://www.sbert.net/).
+    * model (optional): a string of the sentence tranformer model, to use instead of the default one, for more [details](https://www.sbert.net/).
     * lang (optional): the languge of the model ('en'|'ar').
     * only_include (optional): used only for dataframe matching, allow providing a list of column names to only include for the target matches, provide empty list to get only target_col.
     * encode_batch (optional): the number of sentences to encode in a batch.
     * encode_target: boolean flag to indicate whatever to enocde the targets when initilizing the object (to cache target encoding).
     * remove_punct: boolean flag to indicate whatever to remove punctuations. 
     * remove_stop_words: boolean flag to indicate whatever to remove stop words.
     * stemm: boolean flag to indicate whatever to do stemming.
 * sentence_tranformer.match(
-        source: Union[list[str], pd.DataFrame], 
-        source_col: str=None, 
-        topn: int=1, 
-        threshold: float=0.5, 
-        return_match_idx: bool=False, 
-        batch_size: int=128
+        source: Union[List[str], pd.DataFrame], 
+        source_mapping: Optional[Union[str, List]]=None, 
+        topn: Optional[int]=1, 
+        return_match_idx: Optional[bool]=False, 
+        threshold: Optional[float]=0.5, 
+        batch_size: Optional[int]=128
     ) -> pd.DataFrame:
   * parameters:
     * source: dataframe or list of input texts to find closest match for.
-    * source_col (partially optional): the source column name used to match, *must be specified for dataframe matching*.
+    * source_mapping (partially optional) *must be specified for dataframe matching*: a list with each element being a tuple with the following three values (the target column name, source column name, the weight for this match), if a string is passed it and one target was only passed it will be mapped to the that target, with a the full weight of 1.0, note that the the overall weights must equal 1.0.
     * topn: number of matches to return.
-    * threshold: the lowest threeshold to ignore matches below it.
-    * return_match_idx: return an extra column for each match containing the index of the match within the target_names.
-    * batch_size: the size of the batch in inputs to match with targets (to limit space usage).
+    * threshold: the lowest threeshold for a match, matches below it are ignored.
+    * batch_size: the size of the batch in inputs to match with targets (to limit space/memory usage).
   * returns:
-    * a data frame with 3 columns (source, target, score), and two extra columns for each extra match (target_2, score_2 ...), and an optional extra column for each match containg the match index, if return_match_idxs set to True.
+    * a data frame with 3 main values (source, target columns, score), and two extra values for each extra match (target columns, score_2, target columns, score_3 ...)
 #### examples
 the given examples will only use english to present the output in the correct format, if you like to use arabic matching change the lang attribute of the sentence_tranformer object to 'ar'.
 ##### using lists
 ```python
 from similarity_check.checkers import sentence_tranformer_checker
 
 X = ['test', 'remove test']
@@ -95,16 +94,16 @@
     'new_id': [1, 2, 3],
     'tags': ['pos', 'neg', 'pos'],
     'num': [10, 22, 40],
     'day': [3, 5, 2],
 }
 )
 
-st = sentence_tranformer_checker(y, target_col='new_text',target_group='tags', only_include=['new_id'])
-match_df = st.match(X, source_col='text', topn=4, threshold=0.6, batch_size=1)
+st = sentence_tranformer_checker(y, target_cols='new_text',target_group='tags', only_include=['new_id'])
+match_df = st.match(X, source_mapping={'new_text': ('text', 1)}, topn=4, threshold=0.6, batch_size=1)
 ```
 output:
 | text        |   id |   score_1 | new_text_1    |   new_id_1 |   score_2 | new_text_2   |   new_id_2 |   score_3 | new_text_3    |   new_id_3 | score_4   | new_text_4   | new_id_4   |
 |:------------|-----:|----------:|:--------------|-----------:|----------:|:-------------|-----------:|----------:|:--------------|-----------:|:----------|:-------------|:-----------|
 | test        |    1 |  0.922843 | tests         |          1 |  0.908599 | testing      |          3 |  0.721023 | stop the test |          2 |           |              |            |
 | remove test |    2 |  0.728872 | stop the test |          2 |           |              |            |           |               |            |           |              |            |
```

### Comparing `similarity_check-0.1.9/pyproject.toml` & `similarity_check-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "similarity_check"
-version = "0.1.9"
+version = "0.2.0"
 authors = [
   { name="meshari", email="meshari34343@gmail.com" },
 ]
 description = "package for measuring the similarity of two texts"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `similarity_check-0.1.9/PKG-INFO` & `similarity_check-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: similarity_check
-Version: 0.1.9
+Version: 0.2.0
 Summary: package for measuring the similarity of two texts
 Author-email: meshari <meshari34343@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -27,57 +27,56 @@
 ```
 
 ## Usage
 ### sentence tranformer
 #### documentation
 * sentence_tranformer(
         targets: Union[List[str], pd.DataFrame], 
-        target_group: Union[List[str], pd.DataFrame]=None,
-        target_col: str=None, 
-        device: str = None,
-        model: SentenceTransformer=None, 
-        lang: str='en', 
-        only_include: List[str]=None,
-        encode_batch = 32,
-        encode_target = True,
-        remove_punct: bool=True, 
-        remove_stop_words: bool=True, 
-        stemm: bool=False
+        target_group: Optional[Union[List[str], pd.DataFrame]]=None,
+        target_cols: Optional[str]=None, 
+        device: Optional[str] = None,
+        model: Optional[str]=None, 
+        lang: Optional[str]='en', 
+        only_include: Optional[List[str]]=None,
+        encode_batch: Optional[int] = 32,
+        encode_target: Optional[bool] = True,
+        remove_punct: Optional[bool]=True, 
+        remove_stop_words: Optional[bool]=True, 
+        stemm: Optional[bool]=False
   ):
   * parameters:
     * targets: dataframe or list of targets text to compare with.
     * target_group (optional): goups ids for the target to match only a single target for each group, can either provide list of ids,
     * or the column name in the target dataframe.
-    * target_col (partially optional): the target column name used to match, *must be specified for dataframe matching*.
+    * target_cols (partially optional): the target column names used to match, *must be specified for dataframe matching*.
     * device: the device to do the encoding on operations in (cpu|cuda),
-    * model (optional): a sentence tranformer model object, to use instead of the default one, for more [details](https://www.sbert.net/).
+    * model (optional): a string of the sentence tranformer model, to use instead of the default one, for more [details](https://www.sbert.net/).
     * lang (optional): the languge of the model ('en'|'ar').
     * only_include (optional): used only for dataframe matching, allow providing a list of column names to only include for the target matches, provide empty list to get only target_col.
     * encode_batch (optional): the number of sentences to encode in a batch.
     * encode_target: boolean flag to indicate whatever to enocde the targets when initilizing the object (to cache target encoding).
     * remove_punct: boolean flag to indicate whatever to remove punctuations. 
     * remove_stop_words: boolean flag to indicate whatever to remove stop words.
     * stemm: boolean flag to indicate whatever to do stemming.
 * sentence_tranformer.match(
-        source: Union[list[str], pd.DataFrame], 
-        source_col: str=None, 
-        topn: int=1, 
-        threshold: float=0.5, 
-        return_match_idx: bool=False, 
-        batch_size: int=128
+        source: Union[List[str], pd.DataFrame], 
+        source_mapping: Optional[Union[str, List]]=None, 
+        topn: Optional[int]=1, 
+        return_match_idx: Optional[bool]=False, 
+        threshold: Optional[float]=0.5, 
+        batch_size: Optional[int]=128
     ) -> pd.DataFrame:
   * parameters:
     * source: dataframe or list of input texts to find closest match for.
-    * source_col (partially optional): the source column name used to match, *must be specified for dataframe matching*.
+    * source_mapping (partially optional) *must be specified for dataframe matching*: a list with each element being a tuple with the following three values (the target column name, source column name, the weight for this match), if a string is passed it and one target was only passed it will be mapped to the that target, with a the full weight of 1.0, note that the the overall weights must equal 1.0.
     * topn: number of matches to return.
-    * threshold: the lowest threeshold to ignore matches below it.
-    * return_match_idx: return an extra column for each match containing the index of the match within the target_names.
-    * batch_size: the size of the batch in inputs to match with targets (to limit space usage).
+    * threshold: the lowest threeshold for a match, matches below it are ignored.
+    * batch_size: the size of the batch in inputs to match with targets (to limit space/memory usage).
   * returns:
-    * a data frame with 3 columns (source, target, score), and two extra columns for each extra match (target_2, score_2 ...), and an optional extra column for each match containg the match index, if return_match_idxs set to True.
+    * a data frame with 3 main values (source, target columns, score), and two extra values for each extra match (target columns, score_2, target columns, score_3 ...)
 #### examples
 the given examples will only use english to present the output in the correct format, if you like to use arabic matching change the lang attribute of the sentence_tranformer object to 'ar'.
 ##### using lists
 ```python
 from similarity_check.checkers import sentence_tranformer_checker
 
 X = ['test', 'remove test']
@@ -111,16 +110,16 @@
     'new_id': [1, 2, 3],
     'tags': ['pos', 'neg', 'pos'],
     'num': [10, 22, 40],
     'day': [3, 5, 2],
 }
 )
 
-st = sentence_tranformer_checker(y, target_col='new_text',target_group='tags', only_include=['new_id'])
-match_df = st.match(X, source_col='text', topn=4, threshold=0.6, batch_size=1)
+st = sentence_tranformer_checker(y, target_cols='new_text',target_group='tags', only_include=['new_id'])
+match_df = st.match(X, source_mapping={'new_text': ('text', 1)}, topn=4, threshold=0.6, batch_size=1)
 ```
 output:
 | text        |   id |   score_1 | new_text_1    |   new_id_1 |   score_2 | new_text_2   |   new_id_2 |   score_3 | new_text_3    |   new_id_3 | score_4   | new_text_4   | new_id_4   |
 |:------------|-----:|----------:|:--------------|-----------:|----------:|:-------------|-----------:|----------:|:--------------|-----------:|:----------|:-------------|:-----------|
 | test        |    1 |  0.922843 | tests         |          1 |  0.908599 | testing      |          3 |  0.721023 | stop the test |          2 |           |              |            |
 | remove test |    2 |  0.728872 | stop the test |          2 |           |              |            |           |               |            |           |              |            |
```

