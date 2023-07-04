# Comparing `tmp/chunkipy-0.0.2-py3-none-any.whl.zip` & `tmp/chunkipy-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 8440 bytes, number of entries: 9
+Zip file size: 9069 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat       86 b- defN 23-Jul-03 17:21 chunkipy/__init__.py
--rw-rw-rw-  2.0 fat     4198 b- defN 23-Jul-03 17:11 chunkipy/text_chunker.py
+-rw-rw-rw-  2.0 fat     3796 b- defN 23-Jul-04 06:12 chunkipy/text_chunker.py
 -rw-rw-rw-  2.0 fat      897 b- defN 23-Jul-03 17:17 chunkipy/text_splitter.py
 -rw-rw-rw-  2.0 fat      434 b- defN 23-Jul-03 17:09 chunkipy/tokens_estimators.py
--rw-rw-rw-  2.0 fat     1069 b- defN 23-Jul-03 21:25 chunkipy-0.0.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    13965 b- defN 23-Jul-03 21:25 chunkipy-0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-03 21:25 chunkipy-0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-03 21:25 chunkipy-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      713 b- defN 23-Jul-03 21:25 chunkipy-0.0.2.dist-info/RECORD
-9 files, 21463 bytes uncompressed, 7210 bytes compressed:  66.4%
+-rw-rw-rw-  2.0 fat     1069 b- defN 23-Jul-04 06:33 chunkipy-0.0.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    16638 b- defN 23-Jul-04 06:33 chunkipy-0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-04 06:33 chunkipy-0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-04 06:33 chunkipy-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      713 b- defN 23-Jul-04 06:33 chunkipy-0.0.3.dist-info/RECORD
+9 files, 23734 bytes uncompressed, 7839 bytes compressed:  67.0%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: chunkipy/text_splitter.py
 Comment: 
 
 Filename: chunkipy/tokens_estimators.py
 Comment: 
 
-Filename: chunkipy-0.0.2.dist-info/LICENSE
+Filename: chunkipy-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: chunkipy-0.0.2.dist-info/METADATA
+Filename: chunkipy-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: chunkipy-0.0.2.dist-info/WHEEL
+Filename: chunkipy-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: chunkipy-0.0.2.dist-info/top_level.txt
+Filename: chunkipy-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: chunkipy-0.0.2.dist-info/RECORD
+Filename: chunkipy-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## chunkipy/text_chunker.py

```diff
@@ -1,7 +1,8 @@
+from collections import deque
 from typing import Callable, List
 
 from chunkipy.text_splitter import *
 from chunkipy.tokens_estimators import TokenEstimator, WordTokenEstimator, CharTokenEstimator
 
 SPLIT_STRATEGIES = (
     split_by_sentences,
@@ -27,30 +28,25 @@
         self.token_estimator = token_estimator if tokens is True else CharTokenEstimator()
         self.split_strategies = split_strategies
 
     def chunk(self, text):
         text_parts = []
         text_elem_count = self.token_estimator.estimate_tokens(text)
         if text_elem_count > self.chunk_size:
-            chunks = self.segment(text)
+            chunks = self._split_text_and_build_chunks(text)
             text_parts.extend(chunks)
         else:
             text_parts.append(text)
         return text_parts
 
-    def segment(self, text):
-        if self.tokens is False:
-            return self._split_text_and_build_chunks(text)
-        return self._split_text_and_build_chunks(text)
-
     def _split_text_and_build_chunks(self, text):
-        text_parts_and_counts = self._split_text(text)
+        text_parts_and_counts = self.split_text(text)
         return self._build_chunks(text_parts_and_counts)
 
-    def _split_text(self, text):
+    def split_text(self, text):
         split_strategy = 0
         yield from self._validate_and_split(text, split_strategy)
 
     def _validate_and_split(self, text, split_strategy):
         split_funct = self.split_strategies[split_strategy]
         logging.debug(f"Split Strategy: {split_funct}")
         text_parts = split_funct(text)
@@ -61,43 +57,42 @@
                     and elements_count_in_text_part > self.chunk_size:
                 yield from self._validate_and_split(text_part, split_strategy+1)
             else:
                 yield text_part, elements_count_in_text_part
 
     def _build_chunks(self, text_parts_and_counts):
         chunks = []
+
         chunk_element_count = 0
-        chunk = ""
+        chunk = []
         overlap_count = 0
-        overlapping = []
+        overlapping = deque()
+
         for text_part, elements_count in text_parts_and_counts:
             if chunk_element_count + elements_count <= self.chunk_size:
                 chunk_element_count += elements_count
-                chunk += text_part
+                chunk.append(text_part)
                 if self.overlap_size > 0:
                     while overlap_count + elements_count > self.overlap_size and overlapping:
-                        _, first_overlapping_count = overlapping.pop(0)
+                        _, first_overlapping_count = overlapping.popleft()
                         overlap_count -= first_overlapping_count
-                    if elements_count <= self.overlap_size:
-                        overlap_count += elements_count
-                        overlapping.append((text_part, elements_count))
             else:
-                chunks.append(chunk.strip())
+                chunks.append("".join(chunk).strip())
                 chunk_element_count = 0
-                chunk = ""
+                chunk = []
                 if self.overlap_size > 0:
                     overlapping_text = "".join([t[0] for t in overlapping])
                     chunk_element_count = overlap_count
-                    chunk = overlapping_text
-                    print(overlap_count, overlapping_text)
+                    chunk = [overlapping_text]
                     overlap_count = 0
-                    overlapping = []
-                    if elements_count <= self.overlap_size:
-                        overlap_count += elements_count
-                        overlapping.append((text_part, elements_count))
+                    overlapping = deque()
 
                 chunk_element_count += elements_count
                 chunk += text_part
 
-        chunks.append(chunk.strip())
-        return [chunk for chunk in chunks if chunk != '' and ' ']
+            if elements_count <= self.overlap_size:
+                overlap_count += elements_count
+                overlapping.append((text_part, elements_count))
+
+        chunks.append("".join(chunk).strip())
+        return chunks
```

## Comparing `chunkipy-0.0.2.dist-info/LICENSE` & `chunkipy-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `chunkipy-0.0.2.dist-info/METADATA` & `chunkipy-0.0.3.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chunkipy
-Version: 0.0.2
+Version: 0.0.3
 Summary: Chunkipy is an easy-to-use library for chunking text based on the tokenizer function you provide.
 Home-page: https://github.com/gioelecrispo/chunkipy.git
 Author: Gioele Crispo
 Author-email: crispogioele@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -40,21 +40,23 @@
 
 ## Motivation and Features
 `chunkipy` was created to address the need within the field of natural language processing (NLP)
 to chunk text so that it does not exceed the input size of **neural networks** such as BERT,
 but it could be used for several other use cases.
 
 The library offers some useful features:
-- **Tokenizer function**: unlike other text chunking libraries, `chunkipy` offers the possibility of
-  providing a tokenizer function, in order to build the chunks taking into account the tokenizer
+- **Token estimation**: unlike other text chunking libraries, `chunkipy` offers the possibility of
+  providing a token estimator function, in order to build the chunks taking into account the tokenizer
   that will use those chunks.
 - **Split text into meaningful sentences**: in its default configuration, `chunkipy`,
   in creating the chunks, avoids cutting sentences, and always tries to have a complete and syntactically correct sentence.
   This is achieved through the use of the `stanza` library, which utilizes semantic models to cut text
   into meaningful sentences.
+- **Smart Overlapping**: `chunkipy` offers the possibility to define an `overlap_percentage` and create overlapping chunks to
+  preserve the context along chunks. 
 - **Flexibility in choosing split strategies**: Additionally, `chunkipy` offers complete flexibility
   in choosing how to split, allowing users to define their own text splitting function or choose from a list
   of pre-defined splitting strategies.
 
 By default, `chunkipy` uses `stanza` are main text splitting method; however, if `stanza` produces
 sentences with a number of tokens greater than the chunk size, other split strategy are used.
 Here the list of predefined strategies, sorted by priority (the first one is executed first,
@@ -125,19 +127,57 @@
 Chunk 2, num of tokens 129: -> The Spanish and the Portuguese revolted in the Peninsular War aided by a British army, culminating in defeat for Napoleon's marshals. Napoleon launched an invasion of Russia in the summer of 1812. The resulting campaign witnessed the catastrophic retreat of Napoleon's Grande ArmÃ©e. In 1813, Prussia and Austria joined Russian forces in a Sixth Coalition against France, resulting in a large coalition army defeating Napoleon at the Battle of Leipzig. The coalition invaded France and captured Paris, forcing Napoleon to abdicate in April 1814. He was exiled to the island of Elba, between Corsica and Italy. In France, the Bourbons were restored to power.
 ```
 
 As you can see, `chunkipy` created chunks smaller than the given input size,
 `512`, counted the tokens using BERT's tokenizer, and didn't cut sentences in half,
 producing syntactically correct chunks of text.
 
-You can also use `TextChunker`'s `segment()` method to split a text into smaller parts
+You can also use `TextChunker`'s `split_text()` method to split a text into smaller parts
 without actually creating the chunks.
 This can be useful, for example, when you want to apply further processing to
 the text parts before creating the final chunks.
 
+### Overlapping
+`TextChunker` provides you with the *overlap* functionality.
+The system aims to ensure that the last text parts of each segment do not exceed the maximum token limit defined for overlap. 
+For example, if the `chunk_size` is set to 100 and the `overlap_percentage` is 0.1, the maximum number of overlapping tokens is 10. 
+Consequently, if there are sentences or text parts that fit within this token limit, they are added at the beginning of the next segment. 
+If not, they are skipped to maintain a good ratio between overlap and content. 
+
+```python
+text_chunker = TextChunker(50, tokens=True, overlap_percent=0.3)
+
+# Set up test input
+text = "In this unit test, we are evaluating the overlapping functionality." \
+       "This is a feature of the TextChunker class, which is important for a proper context keeping. The " \
+       "goal is to ensure that overlapping chunks are generated correctly. For this purpose, we have chosen a " \
+       "long text that exceeds 100 tokens. By setting the overlap_percent to 0.3, we expect the " \
+       "generated chunks to have an overlap of approximately 30%. This will help us verify the effectiveness " \
+       "of the overlapping feature. The TextChunker class should be able to handle this scenario and " \
+       "produce the expected results. Let's proceed with running the test and asserting the generated chunks " \
+       "for proper overlap. "
+
+# Generate chunks with overlapping
+chunks = text_chunker.chunk(text)
+
+# Print the resulting chunks
+for i, chunk in enumerate(chunks):
+    print(f"Chunk {i + 1}: {chunk}")
+```
+
+
+This would output:
+
+```
+Chunk 1: In this unit test, we are evaluating the overlapping functionality. This is a feature of the TextChunker class, which is important for a proper context keeping. The goal is to ensure that overlapping chunks are generated correctly. For this purpose, we have chosen a long text that exceeds 100 tokens.
+Chunk 2: For this purpose, we have chosen a long text that exceeds 100 tokens. By setting the overlap_percent to 0.3, we expect the generated chunks to have an overlap of approximately 30%. This will help us verify the effectiveness of the overlapping feature.
+Chunk 3: This will help us verify the effectiveness of the overlapping feature. The TextChunker class should be able to handle this scenario and produce the expected results. Let's proceed with running the test and asserting the generated chunks for proper overlap.
+
+```
+
 
 ### Provide a custom text split strategy
 If you don't want to use `stanza` or you need to use your custom text splitting logic,
 you can provide it in the constructor, as shown in this example:
 
 ```python
 from chunkipy import TextChunker
```

## Comparing `chunkipy-0.0.2.dist-info/RECORD` & `chunkipy-0.0.3.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 chunkipy/__init__.py,sha256=0nMSIymF2RIit4jp4pqdXoNI4Bojj9-MLi0PLByfrhk,86
-chunkipy/text_chunker.py,sha256=i0UiieiicHh8iH8SlVHKm4GXgLjT9xpHTBHw2uD3CHw,4198
+chunkipy/text_chunker.py,sha256=B3ie4P5aauz1uS4D7brT_oJDTJmHbgo-Oqs4db4SM1w,3796
 chunkipy/text_splitter.py,sha256=-jlp31ReCwYo3ypqILYazzoJIPcmYAj7UxWa9qOLF_E,897
 chunkipy/tokens_estimators.py,sha256=e1KX7DyewAyywsHtiSU--guOAo3-1PeakcpHAE-HDJ4,434
-chunkipy-0.0.2.dist-info/LICENSE,sha256=_wBjFfYGBhxQN7mQRcdJeL7Tu9DN99Mqh39E986RxAc,1069
-chunkipy-0.0.2.dist-info/METADATA,sha256=-mfONefC48iAHsL8UJ5uj1Z1Ea8oC60oTCnnZnbWSpA,13965
-chunkipy-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-chunkipy-0.0.2.dist-info/top_level.txt,sha256=byM7-_1_q53IbJOldyfA7F603fM55rAUnYFihMJ8ETE,9
-chunkipy-0.0.2.dist-info/RECORD,,
+chunkipy-0.0.3.dist-info/LICENSE,sha256=_wBjFfYGBhxQN7mQRcdJeL7Tu9DN99Mqh39E986RxAc,1069
+chunkipy-0.0.3.dist-info/METADATA,sha256=tMKDWiaL4JzhxmrL2XjBXyShvGN7-EpIOI2cFaQfGGM,16638
+chunkipy-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+chunkipy-0.0.3.dist-info/top_level.txt,sha256=byM7-_1_q53IbJOldyfA7F603fM55rAUnYFihMJ8ETE,9
+chunkipy-0.0.3.dist-info/RECORD,,
```

