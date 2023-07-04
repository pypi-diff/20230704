# Comparing `tmp/spacy-experimental-0.6.2.tar.gz` & `tmp/spacy-experimental-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacy-experimental-0.6.2.tar", last modified: Tue Feb 14 08:58:26 2023, max compression
+gzip compressed data, was "spacy-experimental-0.6.3.tar", last modified: Tue Jul  4 08:57:31 2023, max compression
```

## Comparing `spacy-experimental-0.6.2.tar` & `spacy-experimental-0.6.3.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-14 08:58:26.050443 spacy-experimental-0.6.2/
--rw-r--r--   0 vsts      (1001) docker     (122)     1083 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      154 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)    11954 2023-02-14 08:58:26.050443 spacy-experimental-0.6.2/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)    11594 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)      119 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)     3627 2023-02-14 08:58:26.050443 spacy-experimental-0.6.2/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)     3408 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-14 08:58:26.042442 spacy-experimental-0.6.2/spacy_experimental/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-14 08:58:26.046442 spacy-experimental-0.6.2/spacy_experimental/biaffine_parser/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/biaffine_parser/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11211 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/biaffine_parser/arc_labeler.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)    10260 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/biaffine_parser/arc_predicter.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)     3774 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/biaffine_parser/bilinear.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1727 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/biaffine_parser/eval.py
--rw-r--r--   0 vsts      (1001) docker     (122)      484 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/biaffine_parser/mst.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)    12533 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/biaffine_parser/mst.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)     4358 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/biaffine_parser/pairwise_bilinear.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1337 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/biaffine_parser/pytorch_bilinear.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4069 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/biaffine_parser/pytorch_pairwise_bilinear.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-14 08:58:26.046442 spacy-experimental-0.6.2/spacy_experimental/biaffine_parser/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/biaffine_parser/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4658 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/biaffine_parser/tests/test_arc_labeler.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4002 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/biaffine_parser/tests/test_arc_predicter.py
--rw-r--r--   0 vsts      (1001) docker     (122)    17586 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/biaffine_parser/tests/test_mst.py
--rw-r--r--   0 vsts      (1001) docker     (122)      353 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/biaffine_parser/util.hh
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-14 08:58:26.046442 spacy-experimental-0.6.2/spacy_experimental/char_tokenizer/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/char_tokenizer/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4180 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/char_tokenizer/char_ner_tokenizer.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)      758 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/char_tokenizer/char_pretokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5732 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/char_tokenizer/char_tagger_tokenizer.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)      604 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/char_tokenizer/scorers.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-14 08:58:26.046442 spacy-experimental-0.6.2/spacy_experimental/char_tokenizer/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/char_tokenizer/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1160 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/char_tokenizer/tests/test_char_tokenizers.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-14 08:58:26.046442 spacy-experimental-0.6.2/spacy_experimental/coref/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/coref/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    14861 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/coref/coref_component.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3639 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/coref/coref_model.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7391 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/coref/coref_scorer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6890 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/coref/coref_util.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10529 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/coref/pytorch_coref_model.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4430 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/coref/pytorch_span_resolver_model.py
--rw-r--r--   0 vsts      (1001) docker     (122)    14537 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/coref/span_resolver_component.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4696 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/coref/span_resolver_model.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-14 08:58:26.046442 spacy-experimental-0.6.2/spacy_experimental/coref/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/coref/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7951 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/coref/tests/test_coref.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9952 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/coref/tests/test_span_resolver.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-14 08:58:26.050443 spacy-experimental-0.6.2/spacy_experimental/span_finder/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/span_finder/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12769 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/span_finder/span_finder_component.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1321 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/span_finder/span_finder_model.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1127 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/span_finder/span_finder_suggester.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-14 08:58:26.050443 spacy-experimental-0.6.2/spacy_experimental/span_finder/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/span_finder/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5324 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/span_finder/tests/test_span_finder.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-14 08:58:26.050443 spacy-experimental-0.6.2/spacy_experimental/span_suggesters/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/span_suggesters/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1811 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/span_suggesters/chunk_suggester.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1091 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/span_suggesters/merge_suggesters.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1762 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/span_suggesters/sentence_suggester.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2246 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/span_suggesters/subtree_suggester.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-14 08:58:26.050443 spacy-experimental-0.6.2/spacy_experimental/span_suggesters/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/span_suggesters/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5471 2023-02-14 08:58:00.000000 spacy-experimental-0.6.2/spacy_experimental/span_suggesters/tests/test_suggesters.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-14 08:58:26.042442 spacy-experimental-0.6.2/spacy_experimental.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)    11954 2023-02-14 08:58:26.000000 spacy-experimental-0.6.2/spacy_experimental.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     2784 2023-02-14 08:58:26.000000 spacy-experimental-0.6.2/spacy_experimental.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-02-14 08:58:26.000000 spacy-experimental-0.6.2/spacy_experimental.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)     3012 2023-02-14 08:58:26.000000 spacy-experimental-0.6.2/spacy_experimental.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-02-14 08:58:26.000000 spacy-experimental-0.6.2/spacy_experimental.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)       42 2023-02-14 08:58:26.000000 spacy-experimental-0.6.2/spacy_experimental.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       19 2023-02-14 08:58:26.000000 spacy-experimental-0.6.2/spacy_experimental.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-04 08:57:31.275370 spacy-experimental-0.6.3/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1083 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      154 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)    11922 2023-07-04 08:57:31.275370 spacy-experimental-0.6.3/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)    11562 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      119 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     3755 2023-07-04 08:57:31.275370 spacy-experimental-0.6.3/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)     3408 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-04 08:57:31.263370 spacy-experimental-0.6.3/spacy_experimental/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-04 08:57:31.267370 spacy-experimental-0.6.3/spacy_experimental/biaffine_parser/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/biaffine_parser/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11211 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/biaffine_parser/arc_labeler.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)    10260 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/biaffine_parser/arc_predicter.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)     3979 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/biaffine_parser/bilinear.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1727 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/biaffine_parser/eval.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      484 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/biaffine_parser/mst.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)    12533 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/biaffine_parser/mst.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)     4614 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/biaffine_parser/pairwise_bilinear.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1337 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/biaffine_parser/pytorch_bilinear.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4087 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/biaffine_parser/pytorch_pairwise_bilinear.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-04 08:57:31.267370 spacy-experimental-0.6.3/spacy_experimental/biaffine_parser/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/biaffine_parser/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4658 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/biaffine_parser/tests/test_arc_labeler.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4002 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/biaffine_parser/tests/test_arc_predicter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    17586 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/biaffine_parser/tests/test_mst.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      353 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/biaffine_parser/util.hh
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-04 08:57:31.267370 spacy-experimental-0.6.3/spacy_experimental/char_tokenizer/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/char_tokenizer/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4180 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/char_tokenizer/char_ner_tokenizer.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)      758 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/char_tokenizer/char_pretokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5732 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/char_tokenizer/char_tagger_tokenizer.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)      604 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/char_tokenizer/scorers.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-04 08:57:31.267370 spacy-experimental-0.6.3/spacy_experimental/char_tokenizer/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/char_tokenizer/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1160 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/char_tokenizer/tests/test_char_tokenizers.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-04 08:57:31.271370 spacy-experimental-0.6.3/spacy_experimental/coref/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/coref/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    14884 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/coref/coref_component.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3827 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/coref/coref_model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7391 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/coref/coref_scorer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6933 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/coref/coref_util.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10529 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/coref/pytorch_coref_model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4430 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/coref/pytorch_span_resolver_model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    14537 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/coref/span_resolver_component.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4914 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/coref/span_resolver_model.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-04 08:57:31.271370 spacy-experimental-0.6.3/spacy_experimental/coref/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/coref/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7951 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/coref/tests/test_coref.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9952 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/coref/tests/test_span_resolver.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-04 08:57:31.271370 spacy-experimental-0.6.3/spacy_experimental/span_finder/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/span_finder/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12763 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/span_finder/span_finder_component.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1188 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/span_finder/span_finder_model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1127 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/span_finder/span_finder_suggester.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-04 08:57:31.271370 spacy-experimental-0.6.3/spacy_experimental/span_finder/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/span_finder/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5324 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/span_finder/tests/test_span_finder.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-04 08:57:31.275370 spacy-experimental-0.6.3/spacy_experimental/span_suggesters/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/span_suggesters/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1811 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/span_suggesters/chunk_suggester.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1085 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/span_suggesters/merge_suggesters.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1762 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/span_suggesters/sentence_suggester.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2246 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/span_suggesters/subtree_suggester.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-04 08:57:31.275370 spacy-experimental-0.6.3/spacy_experimental/span_suggesters/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/span_suggesters/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5471 2023-07-04 08:57:00.000000 spacy-experimental-0.6.3/spacy_experimental/span_suggesters/tests/test_suggesters.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-04 08:57:31.267370 spacy-experimental-0.6.3/spacy_experimental.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)    11922 2023-07-04 08:57:31.000000 spacy-experimental-0.6.3/spacy_experimental.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     2784 2023-07-04 08:57:31.000000 spacy-experimental-0.6.3/spacy_experimental.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-04 08:57:31.000000 spacy-experimental-0.6.3/spacy_experimental.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)     3012 2023-07-04 08:57:31.000000 spacy-experimental-0.6.3/spacy_experimental.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-04 08:57:30.000000 spacy-experimental-0.6.3/spacy_experimental.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)       42 2023-07-04 08:57:31.000000 spacy-experimental-0.6.3/spacy_experimental.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       19 2023-07-04 08:57:31.000000 spacy-experimental-0.6.3/spacy_experimental.egg-info/top_level.txt
```

### Comparing `spacy-experimental-0.6.2/LICENSE` & `spacy-experimental-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spacy-experimental-0.6.2/PKG-INFO` & `spacy-experimental-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy-experimental
-Version: 0.6.2
+Version: 0.6.3
 Summary: Cutting-edge experimental spaCy components and features
 Home-page: https://github.com/explosion/spacy-experimental
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -15,15 +15,15 @@
 
 # spacy-experimental: Cutting-edge experimental spaCy components and features
 
 This package includes experimental components and features for
 [spaCy](https://spacy.io) v3.x, for example model architectures, pipeline
 components and utilities.
 
-[![Azure Pipelines](https://img.shields.io/azure-devops/build/explosion-ai/public/26/master.svg?logo=azure-pipelines&style=flat-square&label=build)](https://dev.azure.com/explosion-ai/public/_build?definitionId=26)
+[![tests](https://github.com/explosion/spacy-experimental/actions/workflows/tests.yml/badge.svg)](https://github.com/explosion/spacy-experimental/actions/workflows/tests.yml)
 [![pypi Version](https://img.shields.io/pypi/v/spacy-experimental.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/spacy-experimental/)
 
 ## Installation
 
 Install with `pip`:
 
 ```bash
@@ -75,18 +75,18 @@
 
 The two tokenizers currently reset any existing tag or entity annotation
 respectively in the process of retokenizing.
 
 #### Character-based tagger tokenizer
 
 In the tagger version `experimental_char_tagger_tokenizer`, the tagging problem
-is represented internally with character-level tags for token start (`T`),
-token internal (`I`), and outside a token (`O`). This representation comes from
-[Elephant: Sequence Labeling for Word and Sentence
-Segmentation](https://aclanthology.org/D13-1146/) (Evang et al., 2013).
+is represented internally with character-level tags for token start (`T`), token
+internal (`I`), and outside a token (`O`). This representation comes from
+[Elephant: Sequence Labeling for Word and Sentence Segmentation](https://aclanthology.org/D13-1146/)
+(Evang et al., 2013).
 
 ```none
 This is a sentence.
 TIIIOTIOTOTIIIIIIIT
 ```
 
 With the option `annotate_sents`, `S` replaces `T` for the first token in each
@@ -214,16 +214,16 @@
 factory = "experimental_arc_predicter"
 
 [components.experimental_arc_labeler]
 factory = "experimental_arc_labeler"
 ```
 
 The arc predicter requires that a previous component (such as `senter`) sets
-sentence boundaries during training. Therefore, such a component must be
-added to `annotating_components`:
+sentence boundaries during training. Therefore, such a component must be added
+to `annotating_components`:
 
 ```ini
 [training]
 annotating_components = ["senter"]
 ```
 
 The [biaffine parser sample project](projects/biaffine_parser) provides an
@@ -234,18 +234,22 @@
 The SpanFinder is a new experimental component that identifies span boundaries
 by tagging potential start and end tokens. It's an ML approach to suggest
 candidate spans with higher precision.
 
 `SpanFinder` uses the following parameters:
 
 - `threshold`: Probability threshold for predicted spans.
-- `predicted_key`: Name of the [SpanGroup](https://spacy.io/api/spangroup) the predicted spans are saved to.
-- `training_key`: Name of the [SpanGroup](https://spacy.io/api/spangroup) the training spans are read from.
-- `max_length`: Max length of the predicted spans. No limit when set to `0`. Defaults to `0`.
-- `min_length`: Min length of the predicted spans. No limit when set to `0`. Defaults to `0`.
+- `predicted_key`: Name of the [SpanGroup](https://spacy.io/api/spangroup) the
+  predicted spans are saved to.
+- `training_key`: Name of the [SpanGroup](https://spacy.io/api/spangroup) the
+  training spans are read from.
+- `max_length`: Max length of the predicted spans. No limit when set to `0`.
+  Defaults to `0`.
+- `min_length`: Min length of the predicted spans. No limit when set to `0`.
+  Defaults to `0`.
 
 Here is a config excerpt for the `SpanFinder` together with a `SpanCategorizer`:
 
 ```ini
 [nlp]
 lang = "en"
 pipeline = ["tok2vec","span_finder","spancat"]
@@ -325,21 +329,28 @@
 width = ${components.tok2vec.model.encode.width}
 
 [components.spancat.suggester]
 @misc = "spacy-experimental.span_finder_suggester.v1"
 predicted_key = ${components.span_finder.predicted_key}
 ```
 
-This package includes a [spaCy project](./projects/span_finder) which shows how to train and use the `SpanFinder` together with `SpanCategorizer`.
+This package includes a [spaCy project](./projects/span_finder) which shows how
+to train and use the `SpanFinder` together with `SpanCategorizer`.
 
 ### Coreference Components
 
-The [CoreferenceResolver](https://spacy.io/api/coref) and [SpanResolver](https://spacy.io/api/span-resolver) are designed to be used together to build a corerefence pipeline, which allows you to identify which spans in a document refer to the same thing. Each component also includes an architecture and scorer. For more details, see their pages in the main spaCy docs.
+The [CoreferenceResolver](https://spacy.io/api/coref) and
+[SpanResolver](https://spacy.io/api/span-resolver) are designed to be used
+together to build a corerefence pipeline, which allows you to identify which
+spans in a document refer to the same thing. Each component also includes an
+architecture and scorer. For more details, see their pages in the main spaCy
+docs.
 
-For an example of how to build a pipeline with the components, see the [example coref project](https://github.com/explosion/projects/tree/v3/experimental/coref).
+For an example of how to build a pipeline with the components, see the
+[example coref project](https://github.com/explosion/projects/tree/v3/experimental/coref).
 
 ## Architectures
 
 None currently.
 
 ## Other
 
@@ -354,32 +365,37 @@
 - `spacy-experimental.tokenizer_senter_scorer.v1`: Score tokenization and
   sentence segmentation.
 
 ### Misc
 
 Suggester functions for spancat:
 
-**Subtree suggester**: Uses dependency annotation to suggest tokens with their syntactic descendants.
+**Subtree suggester**: Uses dependency annotation to suggest tokens with their
+syntactic descendants.
 
 - `spacy-experimental.subtree_suggester.v1`
 - `spacy-experimental.ngram_subtree_suggester.v1`
 
-**Chunk suggester**: Suggests noun chunks using the noun chunk iterator, which requires POS and dependency annotation.
+**Chunk suggester**: Suggests noun chunks using the noun chunk iterator, which
+requires POS and dependency annotation.
 
 - `spacy-experimental.chunk_suggester.v1`
 - `spacy-experimental.ngram_chunk_suggester.v1`
 
 **Sentence suggester**: Uses sentence boundaries to suggest sentence spans.
 
 - `spacy-experimental.sentence_suggester.v1`
 - `spacy-experimental.ngram_sentence_suggester.v1`
 
-The package also contains a [`merge_suggesters`](spacy_experimental/span_suggesters/merge_suggesters.py) function which can be used to combine suggestions from multiple suggesters.
+The package also contains a
+[`merge_suggesters`](spacy_experimental/span_suggesters/merge_suggesters.py)
+function which can be used to combine suggestions from multiple suggesters.
 
-Here are two config excerpts for using the `subtree suggester` with and without the ngram functionality:
+Here are two config excerpts for using the `subtree suggester` with and without
+the ngram functionality:
 
 ```
 [components.spancat.suggester]
 @misc = "spacy-experimental.subtree_suggester.v1"
 ```
 
 ```
@@ -388,17 +404,17 @@
 sizes = [1, 2, 3]
 ```
 
 Note that all the suggester functions are registered in `@misc`.
 
 ## Bug reports and issues
 
-Please report bugs in the [spaCy issue
-tracker](https://github.com/explosion/spaCy/issues) or open a new thread on the
-[discussion board](https://github.com/explosion/spaCy/discussions) for other
-issues.
+Please report bugs in the
+[spaCy issue tracker](https://github.com/explosion/spaCy/issues) or open a new
+thread on the [discussion board](https://github.com/explosion/spaCy/discussions)
+for other issues.
 
 ## Older documentation
 
-See the READMEs in earlier [tagged
-versions](https://github.com/explosion/spacy-experimental/tags) for details
-about components in earlier releases.
+See the READMEs in earlier
+[tagged versions](https://github.com/explosion/spacy-experimental/tags) for
+details about components in earlier releases.
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1 Name: spacy-experimental Version: 0.6.2 Summary: Cutting-
+Metadata-Version: 2.1 Name: spacy-experimental Version: 0.6.3 Summary: Cutting-
 edge experimental spaCy components and features Home-page: https://github.com/
 explosion/spacy-experimental Author: Explosion Author-email:
 contact@explosion.ai License: MIT Requires-Python: >=3.6 Description-Content-
 Type: text/markdown Provides-Extra: torch License-File: LICENSE [https://
 explosion.ai/assets/img/logo.svg] # spacy-experimental: Cutting-edge
 experimental spaCy components and features This package includes experimental
 components and features for [spaCy](https://spacy.io) v3.x, for example model
-architectures, pipeline components and utilities. [![Azure Pipelines](https://
-img.shields.io/azure-devops/build/explosion-ai/public/26/master.svg?logo=azure-
-pipelines&style=flat-square&label=build)](https://dev.azure.com/explosion-ai/
-public/_build?definitionId=26) [![pypi Version](https://img.shields.io/pypi/v/
-spacy-experimental.svg?style=flat-square&logo=pypi&logoColor=white)](https://
-pypi.org/project/spacy-experimental/) ## Installation Install with `pip`:
-```bash python -m pip install -U pip setuptools wheel python -m pip install
-spacy-experimental ``` ## Using spacy-experimental Components and features may
-be modified or removed in any release, so always specify the exact version as a
-package requirement if you're experimenting with a particular component, e.g.:
-``` spacy-experimental==0.147.0 ``` Then you can add the experimental
-components to your config or import from `spacy_experimental`: ```ini
+architectures, pipeline components and utilities. [![tests](https://github.com/
+explosion/spacy-experimental/actions/workflows/tests.yml/badge.svg)](https://
+github.com/explosion/spacy-experimental/actions/workflows/tests.yml) [![pypi
+Version](https://img.shields.io/pypi/v/spacy-experimental.svg?style=flat-
+square&logo=pypi&logoColor=white)](https://pypi.org/project/spacy-experimental/
+) ## Installation Install with `pip`: ```bash python -m pip install -U pip
+setuptools wheel python -m pip install spacy-experimental ``` ## Using spacy-
+experimental Components and features may be modified or removed in any release,
+so always specify the exact version as a package requirement if you're
+experimenting with a particular component, e.g.: ``` spacy-
+experimental==0.147.0 ``` Then you can add the experimental components to your
+config or import from `spacy_experimental`: ```ini
 [components.experimental_char_ner_tokenizer] factory =
 "experimental_char_ner_tokenizer" ``` ## Components ### Trainable character-
 based tokenizers Two trainable tokenizers represent tokenization as a sequence
 tagging problem over individual characters and use the existing spaCy tagger
 and NER architectures to perform the tagging. In the spaCy pipeline, a simple
 "pretokenizer" is applied as the pipeline tokenizer to split each doc into
 individual characters and the trainable tokenizer is a pipeline component that
```

### Comparing `spacy-experimental-0.6.2/README.md` & `spacy-experimental-0.6.3/spacy_experimental.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,29 @@
+Metadata-Version: 2.1
+Name: spacy-experimental
+Version: 0.6.3
+Summary: Cutting-edge experimental spaCy components and features
+Home-page: https://github.com/explosion/spacy-experimental
+Author: Explosion
+Author-email: contact@explosion.ai
+License: MIT
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: torch
+License-File: LICENSE
+
 <a href="https://explosion.ai"><img src="https://explosion.ai/assets/img/logo.svg" width="125" height="125" align="right" /></a>
 
 # spacy-experimental: Cutting-edge experimental spaCy components and features
 
 This package includes experimental components and features for
 [spaCy](https://spacy.io) v3.x, for example model architectures, pipeline
 components and utilities.
 
-[![Azure Pipelines](https://img.shields.io/azure-devops/build/explosion-ai/public/26/master.svg?logo=azure-pipelines&style=flat-square&label=build)](https://dev.azure.com/explosion-ai/public/_build?definitionId=26)
+[![tests](https://github.com/explosion/spacy-experimental/actions/workflows/tests.yml/badge.svg)](https://github.com/explosion/spacy-experimental/actions/workflows/tests.yml)
 [![pypi Version](https://img.shields.io/pypi/v/spacy-experimental.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/spacy-experimental/)
 
 ## Installation
 
 Install with `pip`:
 
 ```bash
@@ -62,18 +75,18 @@
 
 The two tokenizers currently reset any existing tag or entity annotation
 respectively in the process of retokenizing.
 
 #### Character-based tagger tokenizer
 
 In the tagger version `experimental_char_tagger_tokenizer`, the tagging problem
-is represented internally with character-level tags for token start (`T`),
-token internal (`I`), and outside a token (`O`). This representation comes from
-[Elephant: Sequence Labeling for Word and Sentence
-Segmentation](https://aclanthology.org/D13-1146/) (Evang et al., 2013).
+is represented internally with character-level tags for token start (`T`), token
+internal (`I`), and outside a token (`O`). This representation comes from
+[Elephant: Sequence Labeling for Word and Sentence Segmentation](https://aclanthology.org/D13-1146/)
+(Evang et al., 2013).
 
 ```none
 This is a sentence.
 TIIIOTIOTOTIIIIIIIT
 ```
 
 With the option `annotate_sents`, `S` replaces `T` for the first token in each
@@ -201,16 +214,16 @@
 factory = "experimental_arc_predicter"
 
 [components.experimental_arc_labeler]
 factory = "experimental_arc_labeler"
 ```
 
 The arc predicter requires that a previous component (such as `senter`) sets
-sentence boundaries during training. Therefore, such a component must be
-added to `annotating_components`:
+sentence boundaries during training. Therefore, such a component must be added
+to `annotating_components`:
 
 ```ini
 [training]
 annotating_components = ["senter"]
 ```
 
 The [biaffine parser sample project](projects/biaffine_parser) provides an
@@ -221,18 +234,22 @@
 The SpanFinder is a new experimental component that identifies span boundaries
 by tagging potential start and end tokens. It's an ML approach to suggest
 candidate spans with higher precision.
 
 `SpanFinder` uses the following parameters:
 
 - `threshold`: Probability threshold for predicted spans.
-- `predicted_key`: Name of the [SpanGroup](https://spacy.io/api/spangroup) the predicted spans are saved to.
-- `training_key`: Name of the [SpanGroup](https://spacy.io/api/spangroup) the training spans are read from.
-- `max_length`: Max length of the predicted spans. No limit when set to `0`. Defaults to `0`.
-- `min_length`: Min length of the predicted spans. No limit when set to `0`. Defaults to `0`.
+- `predicted_key`: Name of the [SpanGroup](https://spacy.io/api/spangroup) the
+  predicted spans are saved to.
+- `training_key`: Name of the [SpanGroup](https://spacy.io/api/spangroup) the
+  training spans are read from.
+- `max_length`: Max length of the predicted spans. No limit when set to `0`.
+  Defaults to `0`.
+- `min_length`: Min length of the predicted spans. No limit when set to `0`.
+  Defaults to `0`.
 
 Here is a config excerpt for the `SpanFinder` together with a `SpanCategorizer`:
 
 ```ini
 [nlp]
 lang = "en"
 pipeline = ["tok2vec","span_finder","spancat"]
@@ -312,21 +329,28 @@
 width = ${components.tok2vec.model.encode.width}
 
 [components.spancat.suggester]
 @misc = "spacy-experimental.span_finder_suggester.v1"
 predicted_key = ${components.span_finder.predicted_key}
 ```
 
-This package includes a [spaCy project](./projects/span_finder) which shows how to train and use the `SpanFinder` together with `SpanCategorizer`.
+This package includes a [spaCy project](./projects/span_finder) which shows how
+to train and use the `SpanFinder` together with `SpanCategorizer`.
 
 ### Coreference Components
 
-The [CoreferenceResolver](https://spacy.io/api/coref) and [SpanResolver](https://spacy.io/api/span-resolver) are designed to be used together to build a corerefence pipeline, which allows you to identify which spans in a document refer to the same thing. Each component also includes an architecture and scorer. For more details, see their pages in the main spaCy docs.
+The [CoreferenceResolver](https://spacy.io/api/coref) and
+[SpanResolver](https://spacy.io/api/span-resolver) are designed to be used
+together to build a corerefence pipeline, which allows you to identify which
+spans in a document refer to the same thing. Each component also includes an
+architecture and scorer. For more details, see their pages in the main spaCy
+docs.
 
-For an example of how to build a pipeline with the components, see the [example coref project](https://github.com/explosion/projects/tree/v3/experimental/coref).
+For an example of how to build a pipeline with the components, see the
+[example coref project](https://github.com/explosion/projects/tree/v3/experimental/coref).
 
 ## Architectures
 
 None currently.
 
 ## Other
 
@@ -341,32 +365,37 @@
 - `spacy-experimental.tokenizer_senter_scorer.v1`: Score tokenization and
   sentence segmentation.
 
 ### Misc
 
 Suggester functions for spancat:
 
-**Subtree suggester**: Uses dependency annotation to suggest tokens with their syntactic descendants.
+**Subtree suggester**: Uses dependency annotation to suggest tokens with their
+syntactic descendants.
 
 - `spacy-experimental.subtree_suggester.v1`
 - `spacy-experimental.ngram_subtree_suggester.v1`
 
-**Chunk suggester**: Suggests noun chunks using the noun chunk iterator, which requires POS and dependency annotation.
+**Chunk suggester**: Suggests noun chunks using the noun chunk iterator, which
+requires POS and dependency annotation.
 
 - `spacy-experimental.chunk_suggester.v1`
 - `spacy-experimental.ngram_chunk_suggester.v1`
 
 **Sentence suggester**: Uses sentence boundaries to suggest sentence spans.
 
 - `spacy-experimental.sentence_suggester.v1`
 - `spacy-experimental.ngram_sentence_suggester.v1`
 
-The package also contains a [`merge_suggesters`](spacy_experimental/span_suggesters/merge_suggesters.py) function which can be used to combine suggestions from multiple suggesters.
+The package also contains a
+[`merge_suggesters`](spacy_experimental/span_suggesters/merge_suggesters.py)
+function which can be used to combine suggestions from multiple suggesters.
 
-Here are two config excerpts for using the `subtree suggester` with and without the ngram functionality:
+Here are two config excerpts for using the `subtree suggester` with and without
+the ngram functionality:
 
 ```
 [components.spancat.suggester]
 @misc = "spacy-experimental.subtree_suggester.v1"
 ```
 
 ```
@@ -375,17 +404,17 @@
 sizes = [1, 2, 3]
 ```
 
 Note that all the suggester functions are registered in `@misc`.
 
 ## Bug reports and issues
 
-Please report bugs in the [spaCy issue
-tracker](https://github.com/explosion/spaCy/issues) or open a new thread on the
-[discussion board](https://github.com/explosion/spaCy/discussions) for other
-issues.
+Please report bugs in the
+[spaCy issue tracker](https://github.com/explosion/spaCy/issues) or open a new
+thread on the [discussion board](https://github.com/explosion/spaCy/discussions)
+for other issues.
 
 ## Older documentation
 
-See the READMEs in earlier [tagged
-versions](https://github.com/explosion/spacy-experimental/tags) for details
-about components in earlier releases.
+See the READMEs in earlier
+[tagged versions](https://github.com/explosion/spacy-experimental/tags) for
+details about components in earlier releases.
```

#### html2text {}

```diff
@@ -1,22 +1,27 @@
-[https://explosion.ai/assets/img/logo.svg] # spacy-experimental: Cutting-edge
+Metadata-Version: 2.1 Name: spacy-experimental Version: 0.6.3 Summary: Cutting-
+edge experimental spaCy components and features Home-page: https://github.com/
+explosion/spacy-experimental Author: Explosion Author-email:
+contact@explosion.ai License: MIT Requires-Python: >=3.6 Description-Content-
+Type: text/markdown Provides-Extra: torch License-File: LICENSE [https://
+explosion.ai/assets/img/logo.svg] # spacy-experimental: Cutting-edge
 experimental spaCy components and features This package includes experimental
 components and features for [spaCy](https://spacy.io) v3.x, for example model
-architectures, pipeline components and utilities. [![Azure Pipelines](https://
-img.shields.io/azure-devops/build/explosion-ai/public/26/master.svg?logo=azure-
-pipelines&style=flat-square&label=build)](https://dev.azure.com/explosion-ai/
-public/_build?definitionId=26) [![pypi Version](https://img.shields.io/pypi/v/
-spacy-experimental.svg?style=flat-square&logo=pypi&logoColor=white)](https://
-pypi.org/project/spacy-experimental/) ## Installation Install with `pip`:
-```bash python -m pip install -U pip setuptools wheel python -m pip install
-spacy-experimental ``` ## Using spacy-experimental Components and features may
-be modified or removed in any release, so always specify the exact version as a
-package requirement if you're experimenting with a particular component, e.g.:
-``` spacy-experimental==0.147.0 ``` Then you can add the experimental
-components to your config or import from `spacy_experimental`: ```ini
+architectures, pipeline components and utilities. [![tests](https://github.com/
+explosion/spacy-experimental/actions/workflows/tests.yml/badge.svg)](https://
+github.com/explosion/spacy-experimental/actions/workflows/tests.yml) [![pypi
+Version](https://img.shields.io/pypi/v/spacy-experimental.svg?style=flat-
+square&logo=pypi&logoColor=white)](https://pypi.org/project/spacy-experimental/
+) ## Installation Install with `pip`: ```bash python -m pip install -U pip
+setuptools wheel python -m pip install spacy-experimental ``` ## Using spacy-
+experimental Components and features may be modified or removed in any release,
+so always specify the exact version as a package requirement if you're
+experimenting with a particular component, e.g.: ``` spacy-
+experimental==0.147.0 ``` Then you can add the experimental components to your
+config or import from `spacy_experimental`: ```ini
 [components.experimental_char_ner_tokenizer] factory =
 "experimental_char_ner_tokenizer" ``` ## Components ### Trainable character-
 based tokenizers Two trainable tokenizers represent tokenization as a sequence
 tagging problem over individual characters and use the existing spaCy tagger
 and NER architectures to perform the tagging. In the spaCy pipeline, a simple
 "pretokenizer" is applied as the pipeline tokenizer to split each doc into
 individual characters and the trainable tokenizer is a pipeline component that
```

### Comparing `spacy-experimental-0.6.2/setup.cfg` & `spacy-experimental-0.6.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [metadata]
-version = 0.6.2
+version = 0.6.3
 description = Cutting-edge experimental spaCy components and features
 url = https://github.com/explosion/spacy-experimental
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 license_file = LICENSE
 long_description = file: README.md
 long_description_content_type = text/markdown
 
 [options]
 zip_safe = false
 python_requires = >=3.6
 install_requires = 
-	spacy>=3.3.0,<3.6.0
+	spacy>=3.3.0,<3.7.0
 
 [options.entry_points]
 spacy_architectures = 
 	spacy-experimental.Bilinear.v1 = spacy_experimental.biaffine_parser.bilinear:build_bilinear
 	spacy-experimental.PairwiseBilinear.v1 = spacy_experimental.biaffine_parser.pairwise_bilinear:build_pairwise_bilinear
 	spacy-experimental.SpanFinder.v1 = spacy_experimental.span_finder.span_finder_model:build_finder_model
 	spacy-experimental.Coref.v1 = spacy_experimental.coref.coref_model:build_coref_model
@@ -55,11 +55,17 @@
 
 [bdist_wheel]
 universal = false
 
 [sdist]
 formats = gztar
 
+[mypy]
+ignore_missing_imports = True
+no_implicit_optional = True
+plugins = pydantic.mypy, thinc.mypy
+allow_redefinition = True
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `spacy-experimental-0.6.2/setup.py` & `spacy-experimental-0.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `spacy-experimental-0.6.2/spacy_experimental/biaffine_parser/arc_labeler.pyx` & `spacy-experimental-0.6.3/spacy_experimental/biaffine_parser/arc_labeler.pyx`

 * *Files identical despite different names*

### Comparing `spacy-experimental-0.6.2/spacy_experimental/biaffine_parser/arc_predicter.pyx` & `spacy-experimental-0.6.3/spacy_experimental/biaffine_parser/arc_predicter.pyx`

 * *Files identical despite different names*

### Comparing `spacy-experimental-0.6.2/spacy_experimental/biaffine_parser/bilinear.py` & `spacy-experimental-0.6.3/spacy_experimental/biaffine_parser/bilinear.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from thinc.api import with_getitem, xp2torch
 from thinc.shims.pytorch_grad_scaler import PyTorchGradScaler
 from thinc.types import ArgsKwargs, Floats2d, Ints1d
 
 
 # Ensure that the spacy-experimental package can register entry points without
 # Torch installed.
+PyTorchBilinearModel: Optional[type]
 try:
     from .pytorch_bilinear import BilinearModel as PyTorchBilinearModel
 except ImportError:
     PyTorchBilinearModel = None
 
 
 def build_bilinear(
@@ -43,29 +44,32 @@
             "dropout_rate": dropout,
             "hidden_width": hidden_width,
             "mixed_precision": mixed_precision,
             "grad_scaler": grad_scaler,
         },
     )
 
-    model = chain(
+    model: Model[Tuple[List[Doc], Ints1d], Floats2d] = chain(
         cast(
             Model[Tuple[List[Doc], Ints1d], Tuple[Floats2d, Ints1d]],
             with_getitem(
                 0, chain(tok2vec, cast(Model[List[Floats2d], Floats2d], list2array()))
             ),
         ),
         bilinear,
     )
     model.set_ref("bilinear", bilinear)
 
     return model
 
 
 def bilinear_init(model: Model, X=None, Y=None):
+    if PyTorchBilinearModel is None:
+        raise ImportError("BiLinear layer requires PyTorch: pip install thinc[torch]")
+
     if model.layers:
         return
 
     if X is not None and model.has_dim("nI") is None:
         model.set_dim("nI", get_width(X))
     if Y is not None and model.has_dim("nO") is None:
         model.set_dim("nO", get_width(Y))
```

### Comparing `spacy-experimental-0.6.2/spacy_experimental/biaffine_parser/eval.py` & `spacy-experimental-0.6.3/spacy_experimental/biaffine_parser/eval.py`

 * *Files identical despite different names*

### Comparing `spacy-experimental-0.6.2/spacy_experimental/biaffine_parser/mst.pyx` & `spacy-experimental-0.6.3/spacy_experimental/biaffine_parser/mst.pyx`

 * *Files identical despite different names*

### Comparing `spacy-experimental-0.6.2/spacy_experimental/biaffine_parser/pairwise_bilinear.py` & `spacy-experimental-0.6.3/spacy_experimental/biaffine_parser/pairwise_bilinear.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-from typing import List, Optional, Tuple, cast
+from typing import List, Optional, Tuple, Union, cast
 
 from spacy import registry
 from spacy.tokens.doc import Doc
 from thinc.api import Model, chain, get_width, list2array, torch2xp
 from thinc.api import with_getitem, xp2torch
 from thinc.shims.pytorch_grad_scaler import PyTorchGradScaler
 from thinc.types import ArgsKwargs, Floats2d, Floats3d, Floats4d, Ints1d
 
 # Ensure that the spacy-experimental package can register entry points without
 # Torch installed.
+PyTorchPairwiseBilinearModel: Optional[type]
 try:
     from .pytorch_pairwise_bilinear import (
         PairwiseBilinearModel as PyTorchPairwiseBilinearModel,
     )
 except ImportError:
     PyTorchPairwiseBilinearModel = None
 
@@ -33,42 +34,47 @@
 
     nI = None
     if tok2vec.has_dim("nO") is True:
         nI = tok2vec.get_dim("nO")
 
     pairwise_bilinear: Model[Tuple[Floats2d, Ints1d], Floats2d] = Model(
         "pairwise_bilinear",
-        forward=pairswise_bilinear_forward,
+        forward=pairwise_bilinear_forward,
         init=pairwise_bilinear_init,
         dims={"nI": nI, "nO": nO},
         attrs={
             # We currently do not update dropout when dropout_rate is
             # changed, since we cannot access the underlying model.
             "dropout_rate": dropout,
             "hidden_width": hidden_width,
             "mixed_precision": mixed_precision,
             "grad_scaler": grad_scaler,
         },
     )
 
-    model = chain(
+    model: Model[Tuple[List[Doc], Ints1d], Floats2d] = chain(
         cast(
             Model[Tuple[List[Doc], Ints1d], Tuple[Floats2d, Ints1d]],
             with_getitem(
                 0, chain(tok2vec, cast(Model[List[Floats2d], Floats2d], list2array()))
             ),
         ),
         pairwise_bilinear,
     )
     model.set_ref("pairwise_bilinear", pairwise_bilinear)
 
     return model
 
 
 def pairwise_bilinear_init(model: Model, X=None, Y=None):
+    if PyTorchPairwiseBilinearModel is None:
+        raise ImportError(
+            "PairwiseBiLinear layer requires PyTorch: pip install thinc[torch]"
+        )
+
     if model.layers:
         return
 
     if X is not None and model.has_dim("nI") is None:
         model.set_dim("nI", get_width(X))
     if Y is not None and model.has_dim("nO") is None:
         model.set_dim("nO", get_width(Y))
@@ -90,15 +96,15 @@
             convert_outputs=convert_outputs,
             mixed_precision=mixed_precision,
             grad_scaler=grad_scaler,
         )
     ]
 
 
-def pairswise_bilinear_forward(model: Model, X, is_train: bool):
+def pairwise_bilinear_forward(model: Model, X, is_train: bool):
     return model.layers[0](X, is_train)
 
 
 def convert_inputs(
     model: Model, X_lenghts: Tuple[Floats2d, Ints1d], is_train: bool = False
 ):
     flatten = model.ops.flatten
@@ -124,15 +130,15 @@
     flatten = model.ops.flatten
     unflatten = model.ops.unflatten
     pad = model.ops.pad
     unpad = model.ops.unpad
 
     (_, lengths), Y_t = inputs_outputs
 
-    def convert_for_torch_backward(dY: Tuple[Floats2d, Floats3d]) -> ArgsKwargs:
+    def convert_for_torch_backward(dY: Union[Floats3d, Floats4d]) -> ArgsKwargs:
         dY_t = xp2torch(pad(unflatten(dY, lengths)))
         return ArgsKwargs(
             args=([Y_t],),
             kwargs={"grad_tensors": [dY_t]},
         )
 
     Y = cast(Floats4d, torch2xp(Y_t))
```

### Comparing `spacy-experimental-0.6.2/spacy_experimental/biaffine_parser/pytorch_bilinear.py` & `spacy-experimental-0.6.3/spacy_experimental/biaffine_parser/pytorch_bilinear.py`

 * *Files identical despite different names*

### Comparing `spacy-experimental-0.6.2/spacy_experimental/biaffine_parser/pytorch_pairwise_bilinear.py` & `spacy-experimental-0.6.3/spacy_experimental/biaffine_parser/pytorch_pairwise_bilinear.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         dropout: float = 0.1,
         hidden_width: int = 128,
     ):
         super(PairwiseBilinearModel, self).__init__()
 
         self.head = nn.Linear(nI, hidden_width)
         self.dependent = nn.Linear(nI, hidden_width)
-        self.bilinear = PairwiseBilinear(hidden_width, nO)
+        self.pairwise_bilinear = PairwiseBilinear(hidden_width, nO)
         self.activation = activation
         self._dropout = VariationalDropout(dropout)
 
     @property
     def dropout(self) -> float:
         return self._dropout.p
 
@@ -107,15 +107,15 @@
         # Create representations of tokens as heads and dependents.
         head = self._dropout(self.activation(self.head(x)))
         dependent = self._dropout(self.activation(self.dependent(x)))
 
         # Compute biaffine attention matrix. This computes from the hidden
         # representations of the shape [batch_size, seq_len, hidden_width] the
         # attention matrices [batch_size, seq_len, seq_len, n_O].
-        logits = self.bilinear(head, dependent)
+        logits = self.pairwise_bilinear(head, dependent)
 
         # Mask out head candidates that are padding time steps. The logits mask
         # has shape [batch_size, seq_len], we reshape it to [batch_size, 1,
         # seq_len] to mask out the head predictions.
         logits += logits_mask
 
         # If there is only one output feature, remove the last dimension.
```

### Comparing `spacy-experimental-0.6.2/spacy_experimental/biaffine_parser/tests/test_arc_labeler.py` & `spacy-experimental-0.6.3/spacy_experimental/biaffine_parser/tests/test_arc_labeler.py`

 * *Files identical despite different names*

### Comparing `spacy-experimental-0.6.2/spacy_experimental/biaffine_parser/tests/test_arc_predicter.py` & `spacy-experimental-0.6.3/spacy_experimental/biaffine_parser/tests/test_arc_predicter.py`

 * *Files identical despite different names*

### Comparing `spacy-experimental-0.6.2/spacy_experimental/biaffine_parser/tests/test_mst.py` & `spacy-experimental-0.6.3/spacy_experimental/biaffine_parser/tests/test_mst.py`

 * *Files identical despite different names*

### Comparing `spacy-experimental-0.6.2/spacy_experimental/char_tokenizer/char_ner_tokenizer.pyx` & `spacy-experimental-0.6.3/spacy_experimental/char_tokenizer/char_ner_tokenizer.pyx`

 * *Files identical despite different names*

### Comparing `spacy-experimental-0.6.2/spacy_experimental/char_tokenizer/char_pretokenizer.py` & `spacy-experimental-0.6.3/spacy_experimental/char_tokenizer/char_pretokenizer.py`

 * *Files identical despite different names*

### Comparing `spacy-experimental-0.6.2/spacy_experimental/char_tokenizer/char_tagger_tokenizer.pyx` & `spacy-experimental-0.6.3/spacy_experimental/char_tokenizer/char_tagger_tokenizer.pyx`

 * *Files identical despite different names*

### Comparing `spacy-experimental-0.6.2/spacy_experimental/char_tokenizer/scorers.py` & `spacy-experimental-0.6.3/spacy_experimental/char_tokenizer/scorers.py`

 * *Files identical despite different names*

### Comparing `spacy-experimental-0.6.2/spacy_experimental/char_tokenizer/tests/test_char_tokenizers.py` & `spacy-experimental-0.6.3/spacy_experimental/char_tokenizer/tests/test_char_tokenizers.py`

 * *Files identical despite different names*

### Comparing `spacy-experimental-0.6.2/spacy_experimental/coref/coref_component.py` & `spacy-experimental-0.6.3/spacy_experimental/coref/coref_component.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,15 @@
         Return the list of predicted clusters.
 
         docs (Iterable[Doc]): The documents to predict.
         RETURNS (List[MentionClusters]): The model's prediction for each document.
 
         DOCS: https://spacy.io/api/coref#predict
         """
-        out = []
+        out: List[MentionClusters] = []
         for doc in docs:
             if len(doc) < 2:
                 # no coref in docs with 0 or 1 token
                 out.append([])
                 continue
 
             scores, idxs = self.model.predict([doc])
```

### Comparing `spacy-experimental-0.6.2/spacy_experimental/coref/coref_model.py` & `spacy-experimental-0.6.3/spacy_experimental/coref/coref_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from typing import List, Tuple, Callable, cast
+from typing import Callable, List, Optional, Tuple, cast
 
 from thinc.api import Model, chain, get_width
 from thinc.api import PyTorchWrapper, ArgsKwargs
 from thinc.types import Floats2d, Ints2d
 from thinc.util import xp2torch, torch2xp
 
 from spacy.tokens import Doc
 
+CorefClusterer: Optional[type]
 try:
     from .pytorch_coref_model import CorefClusterer
 except ImportError:
     CorefClusterer = None
 
 
 def build_coref_model(
@@ -47,14 +48,19 @@
 
         model = tok2vec >> coref_clusterer
         model.set_ref("coref_clusterer", coref_clusterer)
     return model
 
 
 def coref_init(model: Model, X=None, Y=None):
+    if CorefClusterer is None:
+        raise ImportError(
+            "CorefClusterer layer requires PyTorch: pip install thinc[torch]"
+        )
+
     if model.layers:
         return
 
     if X is not None and model.has_dim("nI") is None:
         model.set_dim("nI", get_width(X))
 
     hidden_size = model.attrs["hidden_size"]
```

### Comparing `spacy-experimental-0.6.2/spacy_experimental/coref/coref_scorer.py` & `spacy-experimental-0.6.3/spacy_experimental/coref/coref_scorer.py`

 * *Files identical despite different names*

### Comparing `spacy-experimental-0.6.2/spacy_experimental/coref/coref_util.py` & `spacy-experimental-0.6.3/spacy_experimental/coref/coref_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Tuple, Dict
+from typing import Dict, List, Optional, Tuple
 from thinc.types import Ints1d, Ints2d, Floats2d
 from thinc.api import NumpyOps
 from spacy.language import Language
 from spacy.tokens import Doc
 
 # type alias to make writing this less tedious
 MentionClusters = List[List[Tuple[int, int]]]
@@ -94,15 +94,15 @@
 # from model.py, refactored to be non-member
 def get_predicted_clusters(
     xp,
     span_starts: Ints1d,
     span_ends: Ints1d,
     antecedent_idx: Ints2d,
     antecedent_scores: Floats2d,
-):
+) -> MentionClusters:
     """Convert predictions to usable cluster data.
 
     return values:
 
     clusters: a list of spans (i, j) that are a cluster
 
     Note that not all spans will be in the final output; spans with no
@@ -111,16 +111,16 @@
     # Get predicted antecedents
     ops = NumpyOps()
     predicted_antecedents = ops.asarray(
         get_predicted_antecedents(xp, antecedent_idx, antecedent_scores)
     ).tolist()
 
     # Get predicted clusters
-    mention_to_cluster_id = {}
-    predicted_clusters = []
+    mention_to_cluster_id: Dict[Tuple[int, int], int] = {}
+    predicted_clusters: MentionClusters = []
     for i, predicted_idx in enumerate(predicted_antecedents):
         if predicted_idx < 0:
             continue
         assert i > predicted_idx, f"span idx: {i}; antecedent idx: {predicted_idx}"
         # Check antecedent's cluster
         antecedent = (int(span_starts[predicted_idx]), int(span_ends[predicted_idx]))
         antecedent_cluster_id = mention_to_cluster_id.get(antecedent, -1)
@@ -129,27 +129,26 @@
             predicted_clusters.append([antecedent])
             mention_to_cluster_id[antecedent] = antecedent_cluster_id
         # Add mention to cluster
         mention = (int(span_starts[i]), int(span_ends[i]))
         predicted_clusters[antecedent_cluster_id].append(mention)
         mention_to_cluster_id[mention] = antecedent_cluster_id
 
-    predicted_clusters = [tuple(c) for c in predicted_clusters]
     return predicted_clusters
 
 
 def create_head_span_idxs(ops, doclen: int):
     """Helper function to create single-token span indices."""
     aa = ops.xp.arange(0, doclen)
     bb = ops.xp.arange(0, doclen) + 1
     return ops.asarray2i([aa, bb]).T
 
 
 def get_clusters_from_doc(
-    doc: Doc, *, use_heads: bool = False, prefix: str = None
+    doc: Doc, *, use_heads: bool = False, prefix: Optional[str] = None
 ) -> List[List[Tuple[int, int]]]:
     """Convert the span clusters in a Doc to simple integer tuple lists. The
     ints are char spans, to be tokenization independent.
 
     If `use_heads` is True, then the heads (roots) of the spans will be used.
 
     If a `prefix` is provided, then only spans matching the prefix will be used.
@@ -196,14 +195,15 @@
             ment2cid[ment] = cid
 
     ll = len(ments)
     ops = NumpyOps()
     cpu_ments = ops.asarray(ments)
 
     out = ops.alloc2f(ll, ll)
+    cid: Optional[int]
     for ii, ment in enumerate(cpu_ments):
         cid = ment2cid.get((int(ment[0]), int(ment[1])))
         if cid is None:
             # this is not in a cluster so it has no antecedent
             continue
 
         # this might change if no real antecedent is a candidate
```

### Comparing `spacy-experimental-0.6.2/spacy_experimental/coref/pytorch_coref_model.py` & `spacy-experimental-0.6.3/spacy_experimental/coref/pytorch_coref_model.py`

 * *Files identical despite different names*

### Comparing `spacy-experimental-0.6.2/spacy_experimental/coref/pytorch_span_resolver_model.py` & `spacy-experimental-0.6.3/spacy_experimental/coref/pytorch_span_resolver_model.py`

 * *Files identical despite different names*

### Comparing `spacy-experimental-0.6.2/spacy_experimental/coref/span_resolver_component.py` & `spacy-experimental-0.6.3/spacy_experimental/coref/span_resolver_component.py`

 * *Files identical despite different names*

### Comparing `spacy-experimental-0.6.2/spacy_experimental/coref/span_resolver_model.py` & `spacy-experimental-0.6.3/spacy_experimental/coref/span_resolver_model.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-from typing import List, Tuple, cast
+from typing import List, Optional, Tuple, cast
 import warnings
 
 from thinc.api import Model, chain, tuplify, get_width
 from thinc.api import PyTorchWrapper, ArgsKwargs
 from thinc.types import Floats2d, Ints1d
 from thinc.util import torch, xp2torch, torch2xp
 
 from spacy.tokens import Doc
 from .coref_util import get_sentence_ids, MentionClusters, matches_coref_prefix
 
+SpanResolverModel: Optional[type]
 try:
     from .pytorch_span_resolver_model import SpanResolverModel
 except ImportError:
     SpanResolverModel = None
 
 
 def build_span_resolver(
@@ -21,15 +22,17 @@
     distance_embedding_size: int,
     conv_channels: int,
     window_size: int,
     max_distance: int,
     prefix: str,
 ) -> Model[List[Doc], List[MentionClusters]]:
     if SpanResolverModel is None:
-        raise ImportError("SpanResolver requires PyTorch: pip install thinc[torch]")
+        raise ImportError(
+            "SpanResolverModel requires PyTorch: pip install thinc[torch]"
+        )
 
     nI = None
 
     with Model.define_operators({">>": chain, "&": tuplify}):
         span_resolver: Model[List[Floats2d], List[Floats2d]] = Model(
             "span_resolver",
             forward=span_resolver_forward,
@@ -47,14 +50,19 @@
         model = (tok2vec & head_info) >> span_resolver
         model.set_ref("span_resolver", span_resolver)
 
     return model
 
 
 def span_resolver_init(model: Model, X=None, Y=None):
+    if SpanResolverModel is None:
+        raise ImportError(
+            "SpanResolverModel requires PyTorch: pip install thinc[torch]"
+        )
+
     if model.layers:
         return
 
     if X is not None and model.has_dim("nI") is None:
         model.set_dim("nI", get_width(X))
 
     hidden_size = model.attrs["hidden_size"]
```

### Comparing `spacy-experimental-0.6.2/spacy_experimental/coref/tests/test_coref.py` & `spacy-experimental-0.6.3/spacy_experimental/coref/tests/test_coref.py`

 * *Files identical despite different names*

### Comparing `spacy-experimental-0.6.2/spacy_experimental/coref/tests/test_span_resolver.py` & `spacy-experimental-0.6.3/spacy_experimental/coref/tests/test_span_resolver.py`

 * *Files identical despite different names*

### Comparing `spacy-experimental-0.6.2/spacy_experimental/span_finder/span_finder_component.py` & `spacy-experimental-0.6.3/spacy_experimental/span_finder/span_finder_component.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         f"span_finder_{DEFAULT_PREDICTED_KEY}_p": 0.0,
         f"span_finder_{DEFAULT_PREDICTED_KEY}_r": 0.0,
     },
 )
 def make_span_finder(
     nlp: Language,
     name: str,
-    model: Model[List[Doc], Floats2d],
+    model: Model[Iterable[Doc], Floats2d],
     scorer: Optional[Callable],
     threshold: float,
     max_length: int,
     min_length: int,
     predicted_key: str = DEFAULT_PREDICTED_KEY,
     training_key: str = DEFAULT_TRAINING_KEY,
 ) -> "SpanFinder":
@@ -87,15 +87,15 @@
         from
     max_length (int): Max length of the produced spans (no max limitation when
         set to 0)
     min_length (int): Min length of the produced spans (no min limitation when
         set to 0)
     """
     return SpanFinder(
-        nlp.vocab,
+        nlp,
         model=model,
         threshold=threshold,
         name=name,
         scorer=scorer,
         max_length=max_length,
         min_length=min_length,
         predicted_key=predicted_key,
@@ -146,15 +146,15 @@
 
 class SpanFinder(TrainablePipe):
     """Pipeline that learns span boundaries"""
 
     def __init__(
         self,
         nlp: Language,
-        model: Model[List[Doc], Floats2d],
+        model: Model[Iterable[Doc], Floats2d],
         name: str = "span_finder",
         *,
         threshold: float = 0.5,
         max_length: int = 0,
         min_length: int = 0,
         scorer: Optional[Callable] = partial(
             span_finder_score,
@@ -172,15 +172,15 @@
             positive.
         scorer (Optional[Callable]): The scoring method.
         predicted_key (str): Name of the span group the candidate spans are saved to
         training_key (str): Name of the span group the training spans are read from
         max_length (int): Max length of the produced spans (unlimited when set to 0)
         min_length (int): Min length of the produced spans (unlimited when set to 0)
         """
-        self.vocab = nlp
+        self.vocab = nlp.vocab
         self.threshold = threshold
         self.max_length = max_length
         self.min_length = min_length
         self.predicted_key = predicted_key
         self.training_key = training_key
         self.model = model
         self.name = name
@@ -255,27 +255,27 @@
         loss, d_scores = self.get_loss(examples, scores)
         backprop_scores(d_scores)
         if sgd is not None:
             self.finish_update(sgd)
         losses[self.name] += loss
         return losses
 
-    def get_loss(self, examples, scores) -> Tuple[float, float]:
+    def get_loss(self, examples, scores) -> Tuple[float, Floats2d]:
         """Find the loss and gradient of loss for the batch of documents and
         their predicted scores.
         examples (Iterable[Examples]): The batch of examples.
         scores: Scores representing the model's predictions.
         RETURNS (Tuple[float, float]): The loss and the gradient.
         """
         reference_truths = self._get_aligned_truth_scores(examples)
-        d_scores = scores - self.model.ops.asarray(reference_truths, dtype=float32)
+        d_scores = scores - self.model.ops.asarray2f(reference_truths)
         loss = float((d_scores**2).sum())
         return loss, d_scores
 
-    def _get_aligned_truth_scores(self, examples) -> Tuple[Floats2d, Floats2d]:
+    def _get_aligned_truth_scores(self, examples) -> List[Tuple[int, int]]:
         """Align scores of the predictions to the references for calculating the loss"""
         # TODO: handle misaligned (None) alignments
         # TODO: handle cases with differing whitespace in texts
         reference_truths = []
 
         for eg in examples:
             start_indices = set()
@@ -294,15 +294,15 @@
                         1 if token.idx in start_indices else 0,
                         1 if token.idx + len(token) in end_indices else 0,
                     )
                 )
 
         return reference_truths
 
-    def _get_reference(self, docs) -> Floats2d:
+    def _get_reference(self, docs) -> List[Tuple[int, int]]:
         """Create a reference list of token probabilities"""
         reference_probabilities = []
         for doc in docs:
             start_indices = set()
             end_indices = set()
 
             if self.training_key in doc.spans:
@@ -336,11 +336,11 @@
 
         for eg in get_examples():
             if len(subbatch) < 10:
                 subbatch.append(eg)
 
         if subbatch:
             docs = [eg.reference for eg in subbatch]
-            Y = self.model.ops.asarray(self._get_reference(docs), dtype=float32)
+            Y = self.model.ops.asarray2f(self._get_reference(docs))
             self.model.initialize(X=docs, Y=Y)
         else:
             self.model.initialize()
```

### Comparing `spacy-experimental-0.6.2/spacy_experimental/span_finder/span_finder_suggester.py` & `spacy-experimental-0.6.3/spacy_experimental/span_finder/span_finder_suggester.py`

 * *Files identical despite different names*

### Comparing `spacy-experimental-0.6.2/spacy_experimental/span_finder/tests/test_span_finder.py` & `spacy-experimental-0.6.3/spacy_experimental/span_finder/tests/test_span_finder.py`

 * *Files identical despite different names*

### Comparing `spacy-experimental-0.6.2/spacy_experimental/span_suggesters/chunk_suggester.py` & `spacy-experimental-0.6.3/spacy_experimental/span_suggesters/chunk_suggester.py`

 * *Files identical despite different names*

### Comparing `spacy-experimental-0.6.2/spacy_experimental/span_suggesters/merge_suggesters.py` & `spacy-experimental-0.6.3/spacy_experimental/span_suggesters/merge_suggesters.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,23 @@
 from thinc.types import Ragged, Ints1d
 
 
 def merge_suggestions(suggestions: List[Ragged], ops: Optional[Ops] = None) -> Ragged:
     if ops is None:
         ops = get_current_ops()
 
-    spans = []
-    lengths = []
-
     if len(suggestions) == 0:
-        lengths_array = cast(Ints1d, ops.asarray(lengths, dtype="i"))
+        lengths_array = cast(Ints1d, ops.asarray([], dtype="i"))
         return Ragged(ops.xp.zeros((0, 0), dtype="i"), lengths_array)
 
     len_docs = len(suggestions[0])
     assert all(len_docs == len(x) for x in suggestions)
 
+    spans = []
+    lengths = []
     for i in range(len_docs):
         combined = ops.xp.vstack([s[i].data for s in suggestions if len(s[i].data) > 0])
         uniqued = numpy.unique(ops.to_numpy(combined), axis=0)
         spans.append(ops.asarray(uniqued))
         lengths.append(uniqued.shape[0])
 
     lengths_array = cast(Ints1d, ops.asarray(lengths, dtype="i"))
```

### Comparing `spacy-experimental-0.6.2/spacy_experimental/span_suggesters/sentence_suggester.py` & `spacy-experimental-0.6.3/spacy_experimental/span_suggesters/sentence_suggester.py`

 * *Files identical despite different names*

### Comparing `spacy-experimental-0.6.2/spacy_experimental/span_suggesters/subtree_suggester.py` & `spacy-experimental-0.6.3/spacy_experimental/span_suggesters/subtree_suggester.py`

 * *Files identical despite different names*

### Comparing `spacy-experimental-0.6.2/spacy_experimental/span_suggesters/tests/test_suggesters.py` & `spacy-experimental-0.6.3/spacy_experimental/span_suggesters/tests/test_suggesters.py`

 * *Files identical despite different names*

### Comparing `spacy-experimental-0.6.2/spacy_experimental.egg-info/PKG-INFO` & `spacy-experimental-0.6.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,16 @@
-Metadata-Version: 2.1
-Name: spacy-experimental
-Version: 0.6.2
-Summary: Cutting-edge experimental spaCy components and features
-Home-page: https://github.com/explosion/spacy-experimental
-Author: Explosion
-Author-email: contact@explosion.ai
-License: MIT
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: torch
-License-File: LICENSE
-
 <a href="https://explosion.ai"><img src="https://explosion.ai/assets/img/logo.svg" width="125" height="125" align="right" /></a>
 
 # spacy-experimental: Cutting-edge experimental spaCy components and features
 
 This package includes experimental components and features for
 [spaCy](https://spacy.io) v3.x, for example model architectures, pipeline
 components and utilities.
 
-[![Azure Pipelines](https://img.shields.io/azure-devops/build/explosion-ai/public/26/master.svg?logo=azure-pipelines&style=flat-square&label=build)](https://dev.azure.com/explosion-ai/public/_build?definitionId=26)
+[![tests](https://github.com/explosion/spacy-experimental/actions/workflows/tests.yml/badge.svg)](https://github.com/explosion/spacy-experimental/actions/workflows/tests.yml)
 [![pypi Version](https://img.shields.io/pypi/v/spacy-experimental.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/spacy-experimental/)
 
 ## Installation
 
 Install with `pip`:
 
 ```bash
@@ -75,18 +62,18 @@
 
 The two tokenizers currently reset any existing tag or entity annotation
 respectively in the process of retokenizing.
 
 #### Character-based tagger tokenizer
 
 In the tagger version `experimental_char_tagger_tokenizer`, the tagging problem
-is represented internally with character-level tags for token start (`T`),
-token internal (`I`), and outside a token (`O`). This representation comes from
-[Elephant: Sequence Labeling for Word and Sentence
-Segmentation](https://aclanthology.org/D13-1146/) (Evang et al., 2013).
+is represented internally with character-level tags for token start (`T`), token
+internal (`I`), and outside a token (`O`). This representation comes from
+[Elephant: Sequence Labeling for Word and Sentence Segmentation](https://aclanthology.org/D13-1146/)
+(Evang et al., 2013).
 
 ```none
 This is a sentence.
 TIIIOTIOTOTIIIIIIIT
 ```
 
 With the option `annotate_sents`, `S` replaces `T` for the first token in each
@@ -214,16 +201,16 @@
 factory = "experimental_arc_predicter"
 
 [components.experimental_arc_labeler]
 factory = "experimental_arc_labeler"
 ```
 
 The arc predicter requires that a previous component (such as `senter`) sets
-sentence boundaries during training. Therefore, such a component must be
-added to `annotating_components`:
+sentence boundaries during training. Therefore, such a component must be added
+to `annotating_components`:
 
 ```ini
 [training]
 annotating_components = ["senter"]
 ```
 
 The [biaffine parser sample project](projects/biaffine_parser) provides an
@@ -234,18 +221,22 @@
 The SpanFinder is a new experimental component that identifies span boundaries
 by tagging potential start and end tokens. It's an ML approach to suggest
 candidate spans with higher precision.
 
 `SpanFinder` uses the following parameters:
 
 - `threshold`: Probability threshold for predicted spans.
-- `predicted_key`: Name of the [SpanGroup](https://spacy.io/api/spangroup) the predicted spans are saved to.
-- `training_key`: Name of the [SpanGroup](https://spacy.io/api/spangroup) the training spans are read from.
-- `max_length`: Max length of the predicted spans. No limit when set to `0`. Defaults to `0`.
-- `min_length`: Min length of the predicted spans. No limit when set to `0`. Defaults to `0`.
+- `predicted_key`: Name of the [SpanGroup](https://spacy.io/api/spangroup) the
+  predicted spans are saved to.
+- `training_key`: Name of the [SpanGroup](https://spacy.io/api/spangroup) the
+  training spans are read from.
+- `max_length`: Max length of the predicted spans. No limit when set to `0`.
+  Defaults to `0`.
+- `min_length`: Min length of the predicted spans. No limit when set to `0`.
+  Defaults to `0`.
 
 Here is a config excerpt for the `SpanFinder` together with a `SpanCategorizer`:
 
 ```ini
 [nlp]
 lang = "en"
 pipeline = ["tok2vec","span_finder","spancat"]
@@ -325,21 +316,28 @@
 width = ${components.tok2vec.model.encode.width}
 
 [components.spancat.suggester]
 @misc = "spacy-experimental.span_finder_suggester.v1"
 predicted_key = ${components.span_finder.predicted_key}
 ```
 
-This package includes a [spaCy project](./projects/span_finder) which shows how to train and use the `SpanFinder` together with `SpanCategorizer`.
+This package includes a [spaCy project](./projects/span_finder) which shows how
+to train and use the `SpanFinder` together with `SpanCategorizer`.
 
 ### Coreference Components
 
-The [CoreferenceResolver](https://spacy.io/api/coref) and [SpanResolver](https://spacy.io/api/span-resolver) are designed to be used together to build a corerefence pipeline, which allows you to identify which spans in a document refer to the same thing. Each component also includes an architecture and scorer. For more details, see their pages in the main spaCy docs.
+The [CoreferenceResolver](https://spacy.io/api/coref) and
+[SpanResolver](https://spacy.io/api/span-resolver) are designed to be used
+together to build a corerefence pipeline, which allows you to identify which
+spans in a document refer to the same thing. Each component also includes an
+architecture and scorer. For more details, see their pages in the main spaCy
+docs.
 
-For an example of how to build a pipeline with the components, see the [example coref project](https://github.com/explosion/projects/tree/v3/experimental/coref).
+For an example of how to build a pipeline with the components, see the
+[example coref project](https://github.com/explosion/projects/tree/v3/experimental/coref).
 
 ## Architectures
 
 None currently.
 
 ## Other
 
@@ -354,32 +352,37 @@
 - `spacy-experimental.tokenizer_senter_scorer.v1`: Score tokenization and
   sentence segmentation.
 
 ### Misc
 
 Suggester functions for spancat:
 
-**Subtree suggester**: Uses dependency annotation to suggest tokens with their syntactic descendants.
+**Subtree suggester**: Uses dependency annotation to suggest tokens with their
+syntactic descendants.
 
 - `spacy-experimental.subtree_suggester.v1`
 - `spacy-experimental.ngram_subtree_suggester.v1`
 
-**Chunk suggester**: Suggests noun chunks using the noun chunk iterator, which requires POS and dependency annotation.
+**Chunk suggester**: Suggests noun chunks using the noun chunk iterator, which
+requires POS and dependency annotation.
 
 - `spacy-experimental.chunk_suggester.v1`
 - `spacy-experimental.ngram_chunk_suggester.v1`
 
 **Sentence suggester**: Uses sentence boundaries to suggest sentence spans.
 
 - `spacy-experimental.sentence_suggester.v1`
 - `spacy-experimental.ngram_sentence_suggester.v1`
 
-The package also contains a [`merge_suggesters`](spacy_experimental/span_suggesters/merge_suggesters.py) function which can be used to combine suggestions from multiple suggesters.
+The package also contains a
+[`merge_suggesters`](spacy_experimental/span_suggesters/merge_suggesters.py)
+function which can be used to combine suggestions from multiple suggesters.
 
-Here are two config excerpts for using the `subtree suggester` with and without the ngram functionality:
+Here are two config excerpts for using the `subtree suggester` with and without
+the ngram functionality:
 
 ```
 [components.spancat.suggester]
 @misc = "spacy-experimental.subtree_suggester.v1"
 ```
 
 ```
@@ -388,17 +391,17 @@
 sizes = [1, 2, 3]
 ```
 
 Note that all the suggester functions are registered in `@misc`.
 
 ## Bug reports and issues
 
-Please report bugs in the [spaCy issue
-tracker](https://github.com/explosion/spaCy/issues) or open a new thread on the
-[discussion board](https://github.com/explosion/spaCy/discussions) for other
-issues.
+Please report bugs in the
+[spaCy issue tracker](https://github.com/explosion/spaCy/issues) or open a new
+thread on the [discussion board](https://github.com/explosion/spaCy/discussions)
+for other issues.
 
 ## Older documentation
 
-See the READMEs in earlier [tagged
-versions](https://github.com/explosion/spacy-experimental/tags) for details
-about components in earlier releases.
+See the READMEs in earlier
+[tagged versions](https://github.com/explosion/spacy-experimental/tags) for
+details about components in earlier releases.
```

#### html2text {}

```diff
@@ -1,27 +1,22 @@
-Metadata-Version: 2.1 Name: spacy-experimental Version: 0.6.2 Summary: Cutting-
-edge experimental spaCy components and features Home-page: https://github.com/
-explosion/spacy-experimental Author: Explosion Author-email:
-contact@explosion.ai License: MIT Requires-Python: >=3.6 Description-Content-
-Type: text/markdown Provides-Extra: torch License-File: LICENSE [https://
-explosion.ai/assets/img/logo.svg] # spacy-experimental: Cutting-edge
+[https://explosion.ai/assets/img/logo.svg] # spacy-experimental: Cutting-edge
 experimental spaCy components and features This package includes experimental
 components and features for [spaCy](https://spacy.io) v3.x, for example model
-architectures, pipeline components and utilities. [![Azure Pipelines](https://
-img.shields.io/azure-devops/build/explosion-ai/public/26/master.svg?logo=azure-
-pipelines&style=flat-square&label=build)](https://dev.azure.com/explosion-ai/
-public/_build?definitionId=26) [![pypi Version](https://img.shields.io/pypi/v/
-spacy-experimental.svg?style=flat-square&logo=pypi&logoColor=white)](https://
-pypi.org/project/spacy-experimental/) ## Installation Install with `pip`:
-```bash python -m pip install -U pip setuptools wheel python -m pip install
-spacy-experimental ``` ## Using spacy-experimental Components and features may
-be modified or removed in any release, so always specify the exact version as a
-package requirement if you're experimenting with a particular component, e.g.:
-``` spacy-experimental==0.147.0 ``` Then you can add the experimental
-components to your config or import from `spacy_experimental`: ```ini
+architectures, pipeline components and utilities. [![tests](https://github.com/
+explosion/spacy-experimental/actions/workflows/tests.yml/badge.svg)](https://
+github.com/explosion/spacy-experimental/actions/workflows/tests.yml) [![pypi
+Version](https://img.shields.io/pypi/v/spacy-experimental.svg?style=flat-
+square&logo=pypi&logoColor=white)](https://pypi.org/project/spacy-experimental/
+) ## Installation Install with `pip`: ```bash python -m pip install -U pip
+setuptools wheel python -m pip install spacy-experimental ``` ## Using spacy-
+experimental Components and features may be modified or removed in any release,
+so always specify the exact version as a package requirement if you're
+experimenting with a particular component, e.g.: ``` spacy-
+experimental==0.147.0 ``` Then you can add the experimental components to your
+config or import from `spacy_experimental`: ```ini
 [components.experimental_char_ner_tokenizer] factory =
 "experimental_char_ner_tokenizer" ``` ## Components ### Trainable character-
 based tokenizers Two trainable tokenizers represent tokenization as a sequence
 tagging problem over individual characters and use the existing spaCy tagger
 and NER architectures to perform the tagging. In the spaCy pipeline, a simple
 "pretokenizer" is applied as the pipeline tokenizer to split each doc into
 individual characters and the trainable tokenizer is a pipeline component that
```

### Comparing `spacy-experimental-0.6.2/spacy_experimental.egg-info/SOURCES.txt` & `spacy-experimental-0.6.3/spacy_experimental.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spacy-experimental-0.6.2/spacy_experimental.egg-info/entry_points.txt` & `spacy-experimental-0.6.3/spacy_experimental.egg-info/entry_points.txt`

 * *Files identical despite different names*

