# Comparing `tmp/tokenmonster-1.0.tar.gz` & `tmp/tokenmonster-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokenmonster-1.0.tar", last modified: Mon Jul  3 08:20:56 2023, max compression
+gzip compressed data, was "tokenmonster-1.0.1.tar", last modified: Tue Jul  4 14:27:30 2023, max compression
```

## Comparing `tokenmonster-1.0.tar` & `tokenmonster-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:20:56.888289 tokenmonster-1.0/
--rw-r--r--   0 root         (0) root         (0)      312 2023-07-03 08:20:56.888289 tokenmonster-1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 08:20:56.888289 tokenmonster-1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      386 2023-07-02 14:48:16.000000 tokenmonster-1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:20:56.888289 tokenmonster-1.0/tokenmonster.egg-info/
--rw-r--r--   0 root         (0) root         (0)      312 2023-07-03 08:20:56.000000 tokenmonster-1.0/tokenmonster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      168 2023-07-03 08:20:56.000000 tokenmonster-1.0/tokenmonster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 08:20:56.000000 tokenmonster-1.0/tokenmonster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-03 08:20:56.000000 tokenmonster-1.0/tokenmonster.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    36651 2023-07-03 08:16:48.000000 tokenmonster-1.0/tokenmonster.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 14:27:30.036541 tokenmonster-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)    13932 2023-07-04 14:27:30.036541 tokenmonster-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14073 2023-07-04 14:20:37.000000 tokenmonster-1.0.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-04 14:27:30.036541 tokenmonster-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      550 2023-07-04 14:26:38.000000 tokenmonster-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 14:27:30.036541 tokenmonster-1.0.1/tokenmonster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13932 2023-07-04 14:27:30.000000 tokenmonster-1.0.1/tokenmonster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      178 2023-07-04 14:27:30.000000 tokenmonster-1.0.1/tokenmonster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 14:27:30.000000 tokenmonster-1.0.1/tokenmonster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-04 14:27:30.000000 tokenmonster-1.0.1/tokenmonster.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    36658 2023-07-04 14:07:40.000000 tokenmonster-1.0.1/tokenmonster.py
```

### Comparing `tokenmonster-1.0/tokenmonster.py` & `tokenmonster-1.0.1/tokenmonster.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         """
         A nested class for decoding streams of tokens in sequence.
 
         This class takes tokens and decodes them to generate human-readable strings.
 
         Usage:
             vocab = TokenMonster("english-32000-balanced-v1")
-            decoder = vocab.Decoder()
+            decoder = vocab.decoder()
             decoded_string = decoder.decode(tokens)
             decoded_string += decoder.decode(more_tokens)
         """
 
         def __init__(self, parent):
             self.parent = parent
             self.id = TokenMonster._communicate(5, parent.id, 0)
@@ -165,21 +165,21 @@
         """
         Returns true if the vocabulary has capcode enabled.
         """
         return self.capcode
     
     def charset(self):
         """
-        Returns one of "UTF-8", "UTF-16", or "Binary"
+        Returns one of "UTF-8", "UTF-16", or "None"
         """
         if self.charset == 1:
             return "UTF-8"
         elif self.charset == 2:
             return "UTF-16"
-        return "Binary"
+        return "None"
     
     def decode(self, tokens):
         """
         Decodes tokens into a string.
 
         Only use this "decode" method if you are decoding a complete "batch" or complete "conversation".
         For decoding an incomplete batch sequentially (as the tokens become available) instead
@@ -328,15 +328,15 @@
         Parameters:
             string or list of strings: A string or bytes string, or list of strings or bytes strings.
 
         Returns:
             list of dictionaries where the index is the token ID and each is a dictionary of:
                 token (string): the token including capcode encoding
                 token_decoded (string): the same token decoded from it's capcode form
-                type (int): the type of token (0 = regular, 1 = byte, 2 = special)
+                type (int): the type of token (0 = regular, 1 = byte, 2 = special, 3 = UNK)
                 score (float): token's representation in the dataset used to train the vocabulary
 
         Usage:
             tokens = vocab.tokenize(text)
         """
         if self.dictionary is not None:
             return self.dictionary
@@ -575,22 +575,22 @@
 
     def add_special_token(self, token):
         """
         Add one or more special tokens. This also changes the token IDs. See "modify".
         """
         return self.modify(token, None, None, 0)
     
-    def resize(self, val):
+    def resize(self, size):
         """
         Changes the size of the vocabulary. This also changes the token IDs. See "modify".
 
         A vocabulary can be enlarged as well reduced in size. Only the worst performing
         tokens are removed when reducing.
         """
-        return self.modify(None, None, None, val)
+        return self.modify(None, None, None, size)
     
     def enable_unk_token(self):
         """
         Enables the UNK token.
         The UNK token can be added or removed without affecting the rest of the vocabulary.
         If enabled, the UNK token appears whenever there is a character that is not in the vocabulary.
         Note that the UNK token will not be enabled if all possible characters have tokens.
```

