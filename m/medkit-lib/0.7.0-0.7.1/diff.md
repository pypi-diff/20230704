# Comparing `tmp/medkit_lib-0.7.0.tar.gz` & `tmp/medkit_lib-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medkit_lib-0.7.0.tar", max compression
+gzip compressed data, was "medkit_lib-0.7.1.tar", max compression
```

## Comparing `medkit_lib-0.7.0.tar` & `medkit_lib-0.7.1.tar`

### file list

```diff
@@ -1,128 +1,128 @@
--rw-r--r--   0        0        0     1077 2023-03-23 15:19:08.254089 medkit_lib-0.7.0/LICENSE
--rw-r--r--   0        0        0     1087 2023-06-19 15:44:01.756861 medkit_lib-0.7.0/README.md
--rw-r--r--   0        0        0      173 2023-04-04 06:31:49.436370 medkit_lib-0.7.0/medkit/__init__.py
--rw-r--r--   0        0        0       61 2023-03-23 15:19:08.258090 medkit_lib-0.7.0/medkit/audio/__init__.py
--rw-r--r--   0        0        0      248 2023-04-04 06:31:49.436370 medkit_lib-0.7.0/medkit/audio/preprocessing/__init__.py
--rw-r--r--   0        0        0     2236 2023-03-23 15:19:08.258090 medkit_lib-0.7.0/medkit/audio/preprocessing/downmixer.py
--rw-r--r--   0        0        0     2460 2023-03-23 15:19:08.258090 medkit_lib-0.7.0/medkit/audio/preprocessing/power_normalizer.py
--rw-r--r--   0        0        0     2482 2023-04-21 12:33:02.946744 medkit_lib-0.7.0/medkit/audio/preprocessing/resampler.py
--rw-r--r--   0        0        0      250 2023-04-04 06:31:49.440370 medkit_lib-0.7.0/medkit/audio/segmentation/__init__.py
--rw-r--r--   0        0        0     6530 2023-04-21 12:33:02.946744 medkit_lib-0.7.0/medkit/audio/segmentation/pa_speaker_detector.py
--rw-r--r--   0        0        0     7416 2023-04-21 12:33:02.946744 medkit_lib-0.7.0/medkit/audio/segmentation/webrtc_voice_detector.py
--rw-r--r--   0        0        0      554 2023-04-04 06:31:49.460371 medkit_lib-0.7.0/medkit/audio/transcription/__init__.py
--rw-r--r--   0        0        0     7168 2023-03-23 15:19:08.258090 medkit_lib-0.7.0/medkit/audio/transcription/doc_transcriber.py
--rw-r--r--   0        0        0     3821 2023-04-21 12:33:02.950744 medkit_lib-0.7.0/medkit/audio/transcription/hf_transcriber_function.py
--rw-r--r--   0        0        0     4562 2023-04-21 12:33:02.950744 medkit_lib-0.7.0/medkit/audio/transcription/sb_transcriber_function.py
--rw-r--r--   0        0        0     4776 2023-03-23 15:19:08.262090 medkit_lib-0.7.0/medkit/audio/transcription/transcribed_document.py
--rw-r--r--   0        0        0     1489 2023-03-23 15:19:08.262090 medkit_lib-0.7.0/medkit/core/__init__.py
--rw-r--r--   0        0        0     7827 2023-04-20 16:18:05.215523 medkit_lib-0.7.0/medkit/core/_prov_graph.py
--rw-r--r--   0        0        0     1200 2023-03-23 15:19:08.262090 medkit_lib-0.7.0/medkit/core/annotation.py
--rw-r--r--   0        0        0     4665 2023-03-28 15:25:00.537196 medkit_lib-0.7.0/medkit/core/annotation_container.py
--rw-r--r--   0        0        0     2969 2023-04-21 08:20:44.049464 medkit_lib-0.7.0/medkit/core/attribute.py
--rw-r--r--   0        0        0     3052 2023-03-28 15:25:00.537196 medkit_lib-0.7.0/medkit/core/attribute_container.py
--rw-r--r--   0        0        0      514 2023-03-23 15:19:08.262090 medkit_lib-0.7.0/medkit/core/audio/__init__.py
--rw-r--r--   0        0        0     3712 2023-06-19 16:04:31.637932 medkit_lib-0.7.0/medkit/core/audio/annotation.py
--rw-r--r--   0        0        0     1534 2023-03-23 15:19:08.262090 medkit_lib-0.7.0/medkit/core/audio/annotation_container.py
--rw-r--r--   0        0        0    10898 2023-03-23 15:19:08.262090 medkit_lib-0.7.0/medkit/core/audio/audio_buffer.py
--rw-r--r--   0        0        0     4016 2023-03-23 15:19:08.262090 medkit_lib-0.7.0/medkit/core/audio/document.py
--rw-r--r--   0        0        0      963 2023-03-23 15:19:08.262090 medkit_lib-0.7.0/medkit/core/audio/operation.py
--rw-r--r--   0        0        0      973 2023-03-23 15:19:08.262090 medkit_lib-0.7.0/medkit/core/audio/span.py
--rw-r--r--   0        0        0     1750 2023-03-23 15:19:08.262090 medkit_lib-0.7.0/medkit/core/collection.py
--rw-r--r--   0        0        0      575 2023-03-23 15:19:08.262090 medkit_lib-0.7.0/medkit/core/conversion.py
--rw-r--r--   0        0        0      475 2023-03-23 15:19:08.262090 medkit_lib-0.7.0/medkit/core/data_item.py
--rw-r--r--   0        0        0     4719 2023-03-23 15:19:08.262090 medkit_lib-0.7.0/medkit/core/dict_conv.py
--rw-r--r--   0        0        0     3951 2023-03-23 15:19:08.262090 medkit_lib-0.7.0/medkit/core/doc_pipeline.py
--rw-r--r--   0        0        0      825 2023-03-23 15:19:08.262090 medkit_lib-0.7.0/medkit/core/document.py
--rw-r--r--   0        0        0       96 2023-03-23 15:19:08.262090 medkit_lib-0.7.0/medkit/core/id.py
--rw-r--r--   0        0        0     2404 2023-03-23 15:19:08.262090 medkit_lib-0.7.0/medkit/core/operation.py
--rw-r--r--   0        0        0     1042 2023-03-23 15:19:08.262090 medkit_lib-0.7.0/medkit/core/operation_desc.py
--rw-r--r--   0        0        0    13044 2023-03-23 15:19:08.262090 medkit_lib-0.7.0/medkit/core/pipeline.py
--rw-r--r--   0        0        0     1470 2023-03-23 15:19:08.262090 medkit_lib-0.7.0/medkit/core/prov_store.py
--rw-r--r--   0        0        0    10886 2023-06-23 09:52:38.445241 medkit_lib-0.7.0/medkit/core/prov_tracer.py
--rw-r--r--   0        0        0     2396 2023-03-23 15:19:08.262090 medkit_lib-0.7.0/medkit/core/store.py
--rw-r--r--   0        0        0      883 2023-03-23 15:19:08.266090 medkit_lib-0.7.0/medkit/core/text/__init__.py
--rw-r--r--   0        0        0     8728 2023-04-04 06:31:49.484372 medkit_lib-0.7.0/medkit/core/text/annotation.py
--rw-r--r--   0        0        0     5316 2023-03-23 15:19:08.266090 medkit_lib-0.7.0/medkit/core/text/annotation_container.py
--rw-r--r--   0        0        0     4854 2023-03-23 15:19:08.266090 medkit_lib-0.7.0/medkit/core/text/document.py
--rw-r--r--   0        0        0     1334 2023-03-23 15:19:08.266090 medkit_lib-0.7.0/medkit/core/text/entity_attribute_container.py
--rw-r--r--   0        0        0     3244 2023-04-21 08:20:44.049464 medkit_lib-0.7.0/medkit/core/text/entity_norm_attribute.py
--rw-r--r--   0        0        0     6471 2023-06-26 11:51:07.023156 medkit_lib-0.7.0/medkit/core/text/operation.py
--rw-r--r--   0        0        0     3147 2023-03-23 15:19:08.266090 medkit_lib-0.7.0/medkit/core/text/span.py
--rw-r--r--   0        0        0    18208 2023-03-23 15:19:08.266090 medkit_lib-0.7.0/medkit/core/text/span_utils.py
--rw-r--r--   0        0        0    11691 2023-03-23 15:19:08.266090 medkit_lib-0.7.0/medkit/core/text/utils.py
--rw-r--r--   0        0        0     1462 2023-03-23 15:19:08.266090 medkit_lib-0.7.0/medkit/core/utils.py
--rw-r--r--   0        0        0      401 2023-06-23 09:29:59.689283 medkit_lib-0.7.0/medkit/io/__init__.py
--rw-r--r--   0        0        0    16195 2023-03-23 15:19:08.266090 medkit_lib-0.7.0/medkit/io/_brat_utils.py
--rw-r--r--   0        0        0    21166 2023-04-21 08:20:44.049464 medkit_lib-0.7.0/medkit/io/brat.py
--rw-r--r--   0        0        0      649 2023-03-23 15:19:08.266090 medkit_lib-0.7.0/medkit/io/medkit_json/__init__.py
--rw-r--r--   0        0        0     1235 2023-03-23 15:19:08.266090 medkit_lib-0.7.0/medkit/io/medkit_json/_common.py
--rw-r--r--   0        0        0     6302 2023-06-22 10:48:53.614279 medkit_lib-0.7.0/medkit/io/medkit_json/audio.py
--rw-r--r--   0        0        0     6292 2023-06-22 10:48:53.614279 medkit_lib-0.7.0/medkit/io/medkit_json/text.py
--rw-r--r--   0        0        0    12123 2023-03-23 15:19:08.266090 medkit_lib-0.7.0/medkit/io/rttm.py
--rw-r--r--   0        0        0     7750 2023-04-21 12:33:02.950744 medkit_lib-0.7.0/medkit/io/spacy.py
--rw-r--r--   0        0        0      152 2023-03-23 15:19:08.266090 medkit_lib-0.7.0/medkit/text/__init__.py
--rw-r--r--   0        0        0      590 2023-03-23 15:19:08.266090 medkit_lib-0.7.0/medkit/text/context/__init__.py
--rw-r--r--   0        0        0     9607 2023-06-23 13:22:26.490265 medkit_lib-0.7.0/medkit/text/context/family_detector.py
--rw-r--r--   0        0        0      790 2023-03-23 15:19:08.266090 medkit_lib-0.7.0/medkit/text/context/family_detector_default_rules.yml
--rw-r--r--   0        0        0    14243 2023-06-23 13:22:26.490265 medkit_lib-0.7.0/medkit/text/context/hypothesis_detector.py
--rw-r--r--   0        0        0      905 2023-03-23 15:19:08.270090 medkit_lib-0.7.0/medkit/text/context/hypothesis_detector_example_rules.yml
--rw-r--r--   0        0        0   307270 2023-03-23 15:19:08.270090 medkit_lib-0.7.0/medkit/text/context/hypothesis_detector_example_verbs.yml
--rw-r--r--   0        0        0     9134 2023-06-23 13:22:26.490265 medkit_lib-0.7.0/medkit/text/context/negation_detector.py
--rw-r--r--   0        0        0     4101 2023-03-23 15:19:08.270090 medkit_lib-0.7.0/medkit/text/context/negation_detector_default_rules.yml
--rw-r--r--   0        0        0      304 2023-05-23 14:37:42.934717 medkit_lib-0.7.0/medkit/text/metrics/__init__.py
--rw-r--r--   0        0        0     9422 2023-05-23 14:37:42.934717 medkit_lib-0.7.0/medkit/text/metrics/ner.py
--rw-r--r--   0        0        0     1320 2023-06-19 16:04:31.637932 medkit_lib-0.7.0/medkit/text/ner/__init__.py
--rw-r--r--   0        0        0     3795 2023-04-21 08:20:44.049464 medkit_lib-0.7.0/medkit/text/ner/adicap_norm_attribute.py
--rw-r--r--   0        0        0    11470 2023-04-21 08:20:44.049464 medkit_lib-0.7.0/medkit/text/ner/date_attribute.py
--rw-r--r--   0        0        0     5527 2023-04-20 16:18:05.219523 medkit_lib-0.7.0/medkit/text/ner/duckling_matcher.py
--rw-r--r--   0        0        0     6534 2023-04-21 12:33:02.950744 medkit_lib-0.7.0/medkit/text/ner/hf_entity_matcher.py
--rw-r--r--   0        0        0     8175 2023-05-23 14:37:42.934717 medkit_lib-0.7.0/medkit/text/ner/hf_entity_matcher_trainable.py
--rw-r--r--   0        0        0     7082 2023-05-23 14:37:42.934717 medkit_lib-0.7.0/medkit/text/ner/hf_tokenization_utils.py
--rw-r--r--   0        0        0     5993 2023-05-23 16:01:44.808582 medkit_lib-0.7.0/medkit/text/ner/iamsystem_matcher.py
--rw-r--r--   0        0        0    13006 2023-06-19 16:04:31.637932 medkit_lib-0.7.0/medkit/text/ner/quick_umls_matcher.py
--rw-r--r--   0        0        0    12788 2023-06-23 13:22:26.490265 medkit_lib-0.7.0/medkit/text/ner/regexp_matcher.py
--rw-r--r--   0        0        0    22942 2023-03-23 15:19:08.270090 medkit_lib-0.7.0/medkit/text/ner/regexp_matcher_default_rules.yml
--rw-r--r--   0        0        0     5154 2023-04-21 08:20:44.049464 medkit_lib-0.7.0/medkit/text/ner/tnm_attribute.py
--rw-r--r--   0        0        0    17079 2023-06-19 16:04:31.637932 medkit_lib-0.7.0/medkit/text/ner/umls_coder_normalizer.py
--rw-r--r--   0        0        0     2791 2023-04-21 08:20:44.049464 medkit_lib-0.7.0/medkit/text/ner/umls_norm_attribute.py
--rw-r--r--   0        0        0     5468 2023-03-23 15:19:08.270090 medkit_lib-0.7.0/medkit/text/ner/umls_semgroups_v04.txt
--rw-r--r--   0        0        0     4365 2023-06-19 16:04:31.637932 medkit_lib-0.7.0/medkit/text/ner/umls_utils.py
--rw-r--r--   0        0        0      169 2023-05-30 15:09:33.847172 medkit_lib-0.7.0/medkit/text/postprocessing/__init__.py
--rw-r--r--   0        0        0     1742 2023-05-30 15:09:33.847172 medkit_lib-0.7.0/medkit/text/postprocessing/alignment_utils.py
--rw-r--r--   0        0        0     2212 2023-05-30 15:09:33.847172 medkit_lib-0.7.0/medkit/text/postprocessing/attribute_duplicator.py
--rw-r--r--   0        0        0      639 2023-06-19 16:04:31.641932 medkit_lib-0.7.0/medkit/text/preprocessing/__init__.py
--rw-r--r--   0        0        0     3074 2023-06-19 15:44:01.764862 medkit_lib-0.7.0/medkit/text/preprocessing/char_replacer.py
--rw-r--r--   0        0        0     2374 2023-06-19 15:44:01.764862 medkit_lib-0.7.0/medkit/text/preprocessing/char_rules.py
--rw-r--r--   0        0        0    13519 2023-06-19 16:04:31.641932 medkit_lib-0.7.0/medkit/text/preprocessing/duplicate_finder.py
--rw-r--r--   0        0        0     5393 2023-03-23 15:19:08.274090 medkit_lib-0.7.0/medkit/text/preprocessing/eds_cleaner.py
--rw-r--r--   0        0        0     3199 2023-06-19 15:44:01.764862 medkit_lib-0.7.0/medkit/text/preprocessing/normalizer.py
--rw-r--r--   0        0        0      202 2023-04-04 06:31:49.492373 medkit_lib-0.7.0/medkit/text/relations/__init__.py
--rw-r--r--   0        0        0     9639 2023-04-21 12:33:02.950744 medkit_lib-0.7.0/medkit/text/relations/syntactic_relation_extractor.py
--rw-r--r--   0        0        0      475 2023-05-05 09:23:06.369871 medkit_lib-0.7.0/medkit/text/segmentation/__init__.py
--rw-r--r--   0        0        0    13452 2023-03-23 15:19:08.274090 medkit_lib-0.7.0/medkit/text/segmentation/default_section_definition.yml
--rw-r--r--   0        0        0      629 2023-05-05 09:23:06.369871 medkit_lib-0.7.0/medkit/text/segmentation/default_syntagma_definition.yml
--rw-r--r--   0        0        0     3731 2023-04-21 12:33:02.950744 medkit_lib-0.7.0/medkit/text/segmentation/rush_sentence_tokenizer.py
--rw-r--r--   0        0        0    23436 2023-03-23 15:19:08.274090 medkit_lib-0.7.0/medkit/text/segmentation/rush_sentence_tokenizer_default_rules.tsv
--rw-r--r--   0        0        0     8836 2023-05-15 07:18:23.883719 medkit_lib-0.7.0/medkit/text/segmentation/section_tokenizer.py
--rw-r--r--   0        0        0     4765 2023-04-05 07:40:19.924515 medkit_lib-0.7.0/medkit/text/segmentation/sentence_tokenizer.py
--rw-r--r--   0        0        0     5798 2023-05-15 07:18:23.883719 medkit_lib-0.7.0/medkit/text/segmentation/syntagma_tokenizer.py
--rw-r--r--   0        0        0     1821 2023-05-05 09:23:06.377871 medkit_lib-0.7.0/medkit/text/segmentation/tokenizer_utils.py
--rw-r--r--   0        0        0      669 2023-04-21 12:33:02.950744 medkit_lib-0.7.0/medkit/text/spacy/__init__.py
--rw-r--r--   0        0        0     4203 2023-03-23 15:19:08.274090 medkit_lib-0.7.0/medkit/text/spacy/displacy_utils.py
--rw-r--r--   0        0        0     5765 2023-04-21 08:20:44.049464 medkit_lib-0.7.0/medkit/text/spacy/doc_pipeline.py
--rw-r--r--   0        0        0    15636 2023-04-21 08:20:44.049464 medkit_lib-0.7.0/medkit/text/spacy/edsnlp.py
--rw-r--r--   0        0        0     5136 2023-04-21 08:20:44.049464 medkit_lib-0.7.0/medkit/text/spacy/pipeline.py
--rw-r--r--   0        0        0    18167 2023-04-21 08:20:44.049464 medkit_lib-0.7.0/medkit/text/spacy/spacy_utils.py
--rw-r--r--   0        0        0      180 2023-04-04 06:31:49.500373 medkit_lib-0.7.0/medkit/text/translation/__init__.py
--rw-r--r--   0        0        0    15478 2023-04-21 12:33:02.950744 medkit_lib-0.7.0/medkit/text/translation/hf_translator.py
--rw-r--r--   0        0        0      205 2023-06-26 11:51:07.023156 medkit_lib-0.7.0/medkit/tools/__init__.py
--rw-r--r--   0        0        0     5450 2023-06-26 11:51:07.023156 medkit_lib-0.7.0/medkit/tools/_save_prov_to_dot.py
--rw-r--r--   0        0        0     1198 2023-04-21 12:33:02.950744 medkit_lib-0.7.0/medkit/tools/hf_utils.py
--rw-r--r--   0        0        0      765 2023-04-21 12:33:02.950744 medkit_lib-0.7.0/medkit/training/__init__.py
--rw-r--r--   0        0        0     3822 2023-03-23 15:19:08.278091 medkit_lib-0.7.0/medkit/training/callbacks.py
--rw-r--r--   0        0        0     1987 2023-04-20 16:18:05.231523 medkit_lib-0.7.0/medkit/training/trainable_component.py
--rw-r--r--   0        0        0    11628 2023-05-23 14:37:42.938717 medkit_lib-0.7.0/medkit/training/trainer.py
--rw-r--r--   0        0        0     1998 2023-06-02 09:06:36.988920 medkit_lib-0.7.0/medkit/training/trainer_config.py
--rw-r--r--   0        0        0     2404 2023-03-23 15:19:08.278091 medkit_lib-0.7.0/medkit/training/utils.py
--rw-r--r--   0        0        0     3895 2023-06-26 15:42:53.840424 medkit_lib-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     5065 1970-01-01 00:00:00.000000 medkit_lib-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-03-23 15:19:08.254089 medkit_lib-0.7.1/LICENSE
+-rw-r--r--   0        0        0     1087 2023-06-19 15:44:01.756861 medkit_lib-0.7.1/README.md
+-rw-r--r--   0        0        0      173 2023-04-04 06:31:49.436370 medkit_lib-0.7.1/medkit/__init__.py
+-rw-r--r--   0        0        0       61 2023-03-23 15:19:08.258090 medkit_lib-0.7.1/medkit/audio/__init__.py
+-rw-r--r--   0        0        0      248 2023-04-04 06:31:49.436370 medkit_lib-0.7.1/medkit/audio/preprocessing/__init__.py
+-rw-r--r--   0        0        0     2236 2023-03-23 15:19:08.258090 medkit_lib-0.7.1/medkit/audio/preprocessing/downmixer.py
+-rw-r--r--   0        0        0     2460 2023-03-23 15:19:08.258090 medkit_lib-0.7.1/medkit/audio/preprocessing/power_normalizer.py
+-rw-r--r--   0        0        0     2482 2023-04-21 12:33:02.946744 medkit_lib-0.7.1/medkit/audio/preprocessing/resampler.py
+-rw-r--r--   0        0        0      250 2023-04-04 06:31:49.440370 medkit_lib-0.7.1/medkit/audio/segmentation/__init__.py
+-rw-r--r--   0        0        0     6530 2023-04-21 12:33:02.946744 medkit_lib-0.7.1/medkit/audio/segmentation/pa_speaker_detector.py
+-rw-r--r--   0        0        0     7416 2023-04-21 12:33:02.946744 medkit_lib-0.7.1/medkit/audio/segmentation/webrtc_voice_detector.py
+-rw-r--r--   0        0        0      554 2023-06-27 14:10:01.377546 medkit_lib-0.7.1/medkit/audio/transcription/__init__.py
+-rw-r--r--   0        0        0     7168 2023-06-27 14:10:01.377546 medkit_lib-0.7.1/medkit/audio/transcription/doc_transcriber.py
+-rw-r--r--   0        0        0     3821 2023-06-27 14:10:01.377546 medkit_lib-0.7.1/medkit/audio/transcription/hf_transcriber_function.py
+-rw-r--r--   0        0        0     4562 2023-06-27 14:10:01.377546 medkit_lib-0.7.1/medkit/audio/transcription/sb_transcriber_function.py
+-rw-r--r--   0        0        0     4776 2023-06-27 14:10:01.377546 medkit_lib-0.7.1/medkit/audio/transcription/transcribed_document.py
+-rw-r--r--   0        0        0     1489 2023-06-30 10:02:39.792293 medkit_lib-0.7.1/medkit/core/__init__.py
+-rw-r--r--   0        0        0     7827 2023-04-20 16:18:05.215523 medkit_lib-0.7.1/medkit/core/_prov_graph.py
+-rw-r--r--   0        0        0     1200 2023-03-23 15:19:08.262090 medkit_lib-0.7.1/medkit/core/annotation.py
+-rw-r--r--   0        0        0     4665 2023-03-28 15:25:00.537196 medkit_lib-0.7.1/medkit/core/annotation_container.py
+-rw-r--r--   0        0        0     2969 2023-04-21 08:20:44.049464 medkit_lib-0.7.1/medkit/core/attribute.py
+-rw-r--r--   0        0        0     3052 2023-03-28 15:25:00.537196 medkit_lib-0.7.1/medkit/core/attribute_container.py
+-rw-r--r--   0        0        0      514 2023-03-23 15:19:08.262090 medkit_lib-0.7.1/medkit/core/audio/__init__.py
+-rw-r--r--   0        0        0     3712 2023-07-04 12:59:59.260001 medkit_lib-0.7.1/medkit/core/audio/annotation.py
+-rw-r--r--   0        0        0     1534 2023-03-23 15:19:08.262090 medkit_lib-0.7.1/medkit/core/audio/annotation_container.py
+-rw-r--r--   0        0        0    10898 2023-03-23 15:19:08.262090 medkit_lib-0.7.1/medkit/core/audio/audio_buffer.py
+-rw-r--r--   0        0        0     4016 2023-06-30 10:02:39.792293 medkit_lib-0.7.1/medkit/core/audio/document.py
+-rw-r--r--   0        0        0      963 2023-03-23 15:19:08.262090 medkit_lib-0.7.1/medkit/core/audio/operation.py
+-rw-r--r--   0        0        0      973 2023-03-23 15:19:08.262090 medkit_lib-0.7.1/medkit/core/audio/span.py
+-rw-r--r--   0        0        0     1750 2023-03-23 15:19:08.262090 medkit_lib-0.7.1/medkit/core/collection.py
+-rw-r--r--   0        0        0      575 2023-03-23 15:19:08.262090 medkit_lib-0.7.1/medkit/core/conversion.py
+-rw-r--r--   0        0        0      475 2023-03-23 15:19:08.262090 medkit_lib-0.7.1/medkit/core/data_item.py
+-rw-r--r--   0        0        0     4719 2023-03-23 15:19:08.262090 medkit_lib-0.7.1/medkit/core/dict_conv.py
+-rw-r--r--   0        0        0     3951 2023-03-23 15:19:08.262090 medkit_lib-0.7.1/medkit/core/doc_pipeline.py
+-rw-r--r--   0        0        0      825 2023-03-23 15:19:08.262090 medkit_lib-0.7.1/medkit/core/document.py
+-rw-r--r--   0        0        0       96 2023-06-30 10:02:39.792293 medkit_lib-0.7.1/medkit/core/id.py
+-rw-r--r--   0        0        0     2404 2023-03-23 15:19:08.262090 medkit_lib-0.7.1/medkit/core/operation.py
+-rw-r--r--   0        0        0     1042 2023-03-23 15:19:08.262090 medkit_lib-0.7.1/medkit/core/operation_desc.py
+-rw-r--r--   0        0        0    13044 2023-03-23 15:19:08.262090 medkit_lib-0.7.1/medkit/core/pipeline.py
+-rw-r--r--   0        0        0     1470 2023-03-23 15:19:08.262090 medkit_lib-0.7.1/medkit/core/prov_store.py
+-rw-r--r--   0        0        0    11205 2023-07-04 12:59:59.264001 medkit_lib-0.7.1/medkit/core/prov_tracer.py
+-rw-r--r--   0        0        0     2396 2023-03-23 15:19:08.262090 medkit_lib-0.7.1/medkit/core/store.py
+-rw-r--r--   0        0        0      883 2023-03-23 15:19:08.266090 medkit_lib-0.7.1/medkit/core/text/__init__.py
+-rw-r--r--   0        0        0     8728 2023-04-04 06:31:49.484372 medkit_lib-0.7.1/medkit/core/text/annotation.py
+-rw-r--r--   0        0        0     5316 2023-03-23 15:19:08.266090 medkit_lib-0.7.1/medkit/core/text/annotation_container.py
+-rw-r--r--   0        0        0     4854 2023-06-30 10:02:39.792293 medkit_lib-0.7.1/medkit/core/text/document.py
+-rw-r--r--   0        0        0     1334 2023-03-23 15:19:08.266090 medkit_lib-0.7.1/medkit/core/text/entity_attribute_container.py
+-rw-r--r--   0        0        0     3244 2023-04-21 08:20:44.049464 medkit_lib-0.7.1/medkit/core/text/entity_norm_attribute.py
+-rw-r--r--   0        0        0     6471 2023-06-26 11:51:07.023156 medkit_lib-0.7.1/medkit/core/text/operation.py
+-rw-r--r--   0        0        0     3147 2023-03-23 15:19:08.266090 medkit_lib-0.7.1/medkit/core/text/span.py
+-rw-r--r--   0        0        0    18208 2023-03-23 15:19:08.266090 medkit_lib-0.7.1/medkit/core/text/span_utils.py
+-rw-r--r--   0        0        0    11691 2023-03-23 15:19:08.266090 medkit_lib-0.7.1/medkit/core/text/utils.py
+-rw-r--r--   0        0        0     1462 2023-03-23 15:19:08.266090 medkit_lib-0.7.1/medkit/core/utils.py
+-rw-r--r--   0        0        0      401 2023-06-30 10:02:39.792293 medkit_lib-0.7.1/medkit/io/__init__.py
+-rw-r--r--   0        0        0    16195 2023-03-23 15:19:08.266090 medkit_lib-0.7.1/medkit/io/_brat_utils.py
+-rw-r--r--   0        0        0    21166 2023-06-30 10:02:39.792293 medkit_lib-0.7.1/medkit/io/brat.py
+-rw-r--r--   0        0        0      649 2023-03-23 15:19:08.266090 medkit_lib-0.7.1/medkit/io/medkit_json/__init__.py
+-rw-r--r--   0        0        0     1235 2023-03-23 15:19:08.266090 medkit_lib-0.7.1/medkit/io/medkit_json/_common.py
+-rw-r--r--   0        0        0     6302 2023-07-04 12:59:59.264001 medkit_lib-0.7.1/medkit/io/medkit_json/audio.py
+-rw-r--r--   0        0        0     6292 2023-07-04 12:59:59.264001 medkit_lib-0.7.1/medkit/io/medkit_json/text.py
+-rw-r--r--   0        0        0    12123 2023-06-27 14:10:01.377546 medkit_lib-0.7.1/medkit/io/rttm.py
+-rw-r--r--   0        0        0     7750 2023-04-21 12:33:02.950744 medkit_lib-0.7.1/medkit/io/spacy.py
+-rw-r--r--   0        0        0      152 2023-03-23 15:19:08.266090 medkit_lib-0.7.1/medkit/text/__init__.py
+-rw-r--r--   0        0        0      590 2023-03-23 15:19:08.266090 medkit_lib-0.7.1/medkit/text/context/__init__.py
+-rw-r--r--   0        0        0    10224 2023-07-04 12:59:59.264001 medkit_lib-0.7.1/medkit/text/context/family_detector.py
+-rw-r--r--   0        0        0      790 2023-03-23 15:19:08.266090 medkit_lib-0.7.1/medkit/text/context/family_detector_default_rules.yml
+-rw-r--r--   0        0        0    14864 2023-07-04 12:59:59.264001 medkit_lib-0.7.1/medkit/text/context/hypothesis_detector.py
+-rw-r--r--   0        0        0      905 2023-03-23 15:19:08.270090 medkit_lib-0.7.1/medkit/text/context/hypothesis_detector_example_rules.yml
+-rw-r--r--   0        0        0   307270 2023-03-23 15:19:08.270090 medkit_lib-0.7.1/medkit/text/context/hypothesis_detector_example_verbs.yml
+-rw-r--r--   0        0        0     9753 2023-07-04 12:59:59.264001 medkit_lib-0.7.1/medkit/text/context/negation_detector.py
+-rw-r--r--   0        0        0     4101 2023-03-23 15:19:08.270090 medkit_lib-0.7.1/medkit/text/context/negation_detector_default_rules.yml
+-rw-r--r--   0        0        0      304 2023-05-23 14:37:42.934717 medkit_lib-0.7.1/medkit/text/metrics/__init__.py
+-rw-r--r--   0        0        0     9422 2023-05-23 14:37:42.934717 medkit_lib-0.7.1/medkit/text/metrics/ner.py
+-rw-r--r--   0        0        0     1320 2023-07-04 12:59:59.264001 medkit_lib-0.7.1/medkit/text/ner/__init__.py
+-rw-r--r--   0        0        0     3795 2023-04-21 08:20:44.049464 medkit_lib-0.7.1/medkit/text/ner/adicap_norm_attribute.py
+-rw-r--r--   0        0        0    11470 2023-04-21 08:20:44.049464 medkit_lib-0.7.1/medkit/text/ner/date_attribute.py
+-rw-r--r--   0        0        0     5527 2023-04-20 16:18:05.219523 medkit_lib-0.7.1/medkit/text/ner/duckling_matcher.py
+-rw-r--r--   0        0        0     6534 2023-04-21 12:33:02.950744 medkit_lib-0.7.1/medkit/text/ner/hf_entity_matcher.py
+-rw-r--r--   0        0        0     8175 2023-05-23 14:37:42.934717 medkit_lib-0.7.1/medkit/text/ner/hf_entity_matcher_trainable.py
+-rw-r--r--   0        0        0     7082 2023-05-23 14:37:42.934717 medkit_lib-0.7.1/medkit/text/ner/hf_tokenization_utils.py
+-rw-r--r--   0        0        0     5993 2023-05-23 16:01:44.808582 medkit_lib-0.7.1/medkit/text/ner/iamsystem_matcher.py
+-rw-r--r--   0        0        0    13006 2023-07-04 12:59:59.264001 medkit_lib-0.7.1/medkit/text/ner/quick_umls_matcher.py
+-rw-r--r--   0        0        0    13404 2023-07-04 12:59:59.264001 medkit_lib-0.7.1/medkit/text/ner/regexp_matcher.py
+-rw-r--r--   0        0        0    22942 2023-03-23 15:19:08.270090 medkit_lib-0.7.1/medkit/text/ner/regexp_matcher_default_rules.yml
+-rw-r--r--   0        0        0     5154 2023-04-21 08:20:44.049464 medkit_lib-0.7.1/medkit/text/ner/tnm_attribute.py
+-rw-r--r--   0        0        0    17607 2023-07-04 12:59:59.264001 medkit_lib-0.7.1/medkit/text/ner/umls_coder_normalizer.py
+-rw-r--r--   0        0        0     2791 2023-04-21 08:20:44.049464 medkit_lib-0.7.1/medkit/text/ner/umls_norm_attribute.py
+-rw-r--r--   0        0        0     5468 2023-03-23 15:19:08.270090 medkit_lib-0.7.1/medkit/text/ner/umls_semgroups_v04.txt
+-rw-r--r--   0        0        0     4365 2023-07-04 12:59:59.264001 medkit_lib-0.7.1/medkit/text/ner/umls_utils.py
+-rw-r--r--   0        0        0      169 2023-05-30 15:09:33.847172 medkit_lib-0.7.1/medkit/text/postprocessing/__init__.py
+-rw-r--r--   0        0        0     1742 2023-05-30 15:09:33.847172 medkit_lib-0.7.1/medkit/text/postprocessing/alignment_utils.py
+-rw-r--r--   0        0        0     2212 2023-05-30 15:09:33.847172 medkit_lib-0.7.1/medkit/text/postprocessing/attribute_duplicator.py
+-rw-r--r--   0        0        0      639 2023-07-04 12:59:59.268001 medkit_lib-0.7.1/medkit/text/preprocessing/__init__.py
+-rw-r--r--   0        0        0     3074 2023-06-19 15:44:01.764862 medkit_lib-0.7.1/medkit/text/preprocessing/char_replacer.py
+-rw-r--r--   0        0        0     2374 2023-06-19 15:44:01.764862 medkit_lib-0.7.1/medkit/text/preprocessing/char_rules.py
+-rw-r--r--   0        0        0    13519 2023-07-04 12:59:59.268001 medkit_lib-0.7.1/medkit/text/preprocessing/duplicate_finder.py
+-rw-r--r--   0        0        0     5393 2023-03-23 15:19:08.274090 medkit_lib-0.7.1/medkit/text/preprocessing/eds_cleaner.py
+-rw-r--r--   0        0        0     3199 2023-06-19 15:44:01.764862 medkit_lib-0.7.1/medkit/text/preprocessing/normalizer.py
+-rw-r--r--   0        0        0      202 2023-04-04 06:31:49.492373 medkit_lib-0.7.1/medkit/text/relations/__init__.py
+-rw-r--r--   0        0        0     9639 2023-04-21 12:33:02.950744 medkit_lib-0.7.1/medkit/text/relations/syntactic_relation_extractor.py
+-rw-r--r--   0        0        0      475 2023-05-05 09:23:06.369871 medkit_lib-0.7.1/medkit/text/segmentation/__init__.py
+-rw-r--r--   0        0        0    13452 2023-03-23 15:19:08.274090 medkit_lib-0.7.1/medkit/text/segmentation/default_section_definition.yml
+-rw-r--r--   0        0        0      629 2023-05-05 09:23:06.369871 medkit_lib-0.7.1/medkit/text/segmentation/default_syntagma_definition.yml
+-rw-r--r--   0        0        0     3731 2023-04-21 12:33:02.950744 medkit_lib-0.7.1/medkit/text/segmentation/rush_sentence_tokenizer.py
+-rw-r--r--   0        0        0    23436 2023-03-23 15:19:08.274090 medkit_lib-0.7.1/medkit/text/segmentation/rush_sentence_tokenizer_default_rules.tsv
+-rw-r--r--   0        0        0     8836 2023-05-15 07:18:23.883719 medkit_lib-0.7.1/medkit/text/segmentation/section_tokenizer.py
+-rw-r--r--   0        0        0     4765 2023-04-05 07:40:19.924515 medkit_lib-0.7.1/medkit/text/segmentation/sentence_tokenizer.py
+-rw-r--r--   0        0        0     5798 2023-05-15 07:18:23.883719 medkit_lib-0.7.1/medkit/text/segmentation/syntagma_tokenizer.py
+-rw-r--r--   0        0        0     1821 2023-05-05 09:23:06.377871 medkit_lib-0.7.1/medkit/text/segmentation/tokenizer_utils.py
+-rw-r--r--   0        0        0      669 2023-04-21 12:33:02.950744 medkit_lib-0.7.1/medkit/text/spacy/__init__.py
+-rw-r--r--   0        0        0     4203 2023-03-23 15:19:08.274090 medkit_lib-0.7.1/medkit/text/spacy/displacy_utils.py
+-rw-r--r--   0        0        0     5765 2023-04-21 08:20:44.049464 medkit_lib-0.7.1/medkit/text/spacy/doc_pipeline.py
+-rw-r--r--   0        0        0    15636 2023-04-21 08:20:44.049464 medkit_lib-0.7.1/medkit/text/spacy/edsnlp.py
+-rw-r--r--   0        0        0     5136 2023-04-21 08:20:44.049464 medkit_lib-0.7.1/medkit/text/spacy/pipeline.py
+-rw-r--r--   0        0        0    18167 2023-06-30 10:02:39.792293 medkit_lib-0.7.1/medkit/text/spacy/spacy_utils.py
+-rw-r--r--   0        0        0      180 2023-04-04 06:31:49.500373 medkit_lib-0.7.1/medkit/text/translation/__init__.py
+-rw-r--r--   0        0        0    15478 2023-04-21 12:33:02.950744 medkit_lib-0.7.1/medkit/text/translation/hf_translator.py
+-rw-r--r--   0        0        0      205 2023-07-04 12:59:59.268001 medkit_lib-0.7.1/medkit/tools/__init__.py
+-rw-r--r--   0        0        0     5450 2023-07-04 12:59:59.268001 medkit_lib-0.7.1/medkit/tools/_save_prov_to_dot.py
+-rw-r--r--   0        0        0     1198 2023-04-21 12:33:02.950744 medkit_lib-0.7.1/medkit/tools/hf_utils.py
+-rw-r--r--   0        0        0      765 2023-04-21 12:33:02.950744 medkit_lib-0.7.1/medkit/training/__init__.py
+-rw-r--r--   0        0        0     3822 2023-03-23 15:19:08.278091 medkit_lib-0.7.1/medkit/training/callbacks.py
+-rw-r--r--   0        0        0     1987 2023-04-20 16:18:05.231523 medkit_lib-0.7.1/medkit/training/trainable_component.py
+-rw-r--r--   0        0        0    11628 2023-05-23 14:37:42.938717 medkit_lib-0.7.1/medkit/training/trainer.py
+-rw-r--r--   0        0        0     1998 2023-06-02 09:06:36.988920 medkit_lib-0.7.1/medkit/training/trainer_config.py
+-rw-r--r--   0        0        0     2404 2023-03-23 15:19:08.278091 medkit_lib-0.7.1/medkit/training/utils.py
+-rw-r--r--   0        0        0     3895 2023-07-04 12:59:59.272001 medkit_lib-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     5065 1970-01-01 00:00:00.000000 medkit_lib-0.7.1/PKG-INFO
```

### Comparing `medkit_lib-0.7.0/LICENSE` & `medkit_lib-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/README.md` & `medkit_lib-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/audio/preprocessing/downmixer.py` & `medkit_lib-0.7.1/medkit/audio/preprocessing/downmixer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/audio/preprocessing/power_normalizer.py` & `medkit_lib-0.7.1/medkit/audio/preprocessing/power_normalizer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/audio/preprocessing/resampler.py` & `medkit_lib-0.7.1/medkit/audio/preprocessing/resampler.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/audio/segmentation/pa_speaker_detector.py` & `medkit_lib-0.7.1/medkit/audio/segmentation/pa_speaker_detector.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/audio/segmentation/webrtc_voice_detector.py` & `medkit_lib-0.7.1/medkit/audio/segmentation/webrtc_voice_detector.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/audio/transcription/__init__.py` & `medkit_lib-0.7.1/medkit/audio/transcription/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/audio/transcription/doc_transcriber.py` & `medkit_lib-0.7.1/medkit/audio/transcription/doc_transcriber.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/audio/transcription/hf_transcriber_function.py` & `medkit_lib-0.7.1/medkit/audio/transcription/hf_transcriber_function.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/audio/transcription/sb_transcriber_function.py` & `medkit_lib-0.7.1/medkit/audio/transcription/sb_transcriber_function.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/audio/transcription/transcribed_document.py` & `medkit_lib-0.7.1/medkit/audio/transcription/transcribed_document.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/core/__init__.py` & `medkit_lib-0.7.1/medkit/core/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/core/_prov_graph.py` & `medkit_lib-0.7.1/medkit/core/_prov_graph.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/core/annotation.py` & `medkit_lib-0.7.1/medkit/core/annotation.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/core/annotation_container.py` & `medkit_lib-0.7.1/medkit/core/annotation_container.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/core/attribute.py` & `medkit_lib-0.7.1/medkit/core/attribute.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/core/attribute_container.py` & `medkit_lib-0.7.1/medkit/core/attribute_container.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/core/audio/__init__.py` & `medkit_lib-0.7.1/medkit/core/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/core/audio/annotation.py` & `medkit_lib-0.7.1/medkit/core/audio/annotation.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/core/audio/annotation_container.py` & `medkit_lib-0.7.1/medkit/core/audio/annotation_container.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/core/audio/audio_buffer.py` & `medkit_lib-0.7.1/medkit/core/audio/audio_buffer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/core/audio/document.py` & `medkit_lib-0.7.1/medkit/core/audio/document.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/core/audio/operation.py` & `medkit_lib-0.7.1/medkit/core/audio/operation.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/core/audio/span.py` & `medkit_lib-0.7.1/medkit/core/audio/span.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/core/collection.py` & `medkit_lib-0.7.1/medkit/core/collection.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/core/conversion.py` & `medkit_lib-0.7.1/medkit/core/conversion.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/core/dict_conv.py` & `medkit_lib-0.7.1/medkit/core/dict_conv.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/core/doc_pipeline.py` & `medkit_lib-0.7.1/medkit/core/doc_pipeline.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/core/document.py` & `medkit_lib-0.7.1/medkit/core/document.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/core/operation.py` & `medkit_lib-0.7.1/medkit/core/operation.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/core/operation_desc.py` & `medkit_lib-0.7.1/medkit/core/operation_desc.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/core/pipeline.py` & `medkit_lib-0.7.1/medkit/core/pipeline.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/core/prov_store.py` & `medkit_lib-0.7.1/medkit/core/prov_store.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/core/prov_tracer.py` & `medkit_lib-0.7.1/medkit/core/prov_tracer.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,14 +214,21 @@
             Id of the data item.
 
         Returns
         -------
         Prov
             Provenance info about the data item.
         """
+        if not self._graph.has_node(data_item_id):
+            raise ValueError(
+                f"No provenance info available for data item with id {data_item_id}."
+                " Make sure the id is valid and provenance tracking was enabled for"
+                " the operation that generated it."
+            )
+
         node = self._graph.get_node(data_item_id)
         return self._build_prov_from_node(node)
 
     def get_provs(self) -> List[Prov]:
         """Return all provenance information about all data items known to the tracer.
 
         .. note::
```

### Comparing `medkit_lib-0.7.0/medkit/core/store.py` & `medkit_lib-0.7.1/medkit/core/store.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/core/text/__init__.py` & `medkit_lib-0.7.1/medkit/core/text/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/core/text/annotation.py` & `medkit_lib-0.7.1/medkit/core/text/annotation.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/core/text/annotation_container.py` & `medkit_lib-0.7.1/medkit/core/text/annotation_container.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/core/text/document.py` & `medkit_lib-0.7.1/medkit/core/text/document.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/core/text/entity_attribute_container.py` & `medkit_lib-0.7.1/medkit/core/text/entity_attribute_container.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/core/text/entity_norm_attribute.py` & `medkit_lib-0.7.1/medkit/core/text/entity_norm_attribute.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/core/text/operation.py` & `medkit_lib-0.7.1/medkit/core/text/operation.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/core/text/span.py` & `medkit_lib-0.7.1/medkit/core/text/span.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/core/text/span_utils.py` & `medkit_lib-0.7.1/medkit/core/text/span_utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/core/text/utils.py` & `medkit_lib-0.7.1/medkit/core/text/utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/core/utils.py` & `medkit_lib-0.7.1/medkit/core/utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/io/_brat_utils.py` & `medkit_lib-0.7.1/medkit/io/_brat_utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/io/brat.py` & `medkit_lib-0.7.1/medkit/io/brat.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/io/medkit_json/__init__.py` & `medkit_lib-0.7.1/medkit/io/medkit_json/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/io/medkit_json/_common.py` & `medkit_lib-0.7.1/medkit/io/medkit_json/_common.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/io/medkit_json/audio.py` & `medkit_lib-0.7.1/medkit/io/medkit_json/audio.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/io/medkit_json/text.py` & `medkit_lib-0.7.1/medkit/io/medkit_json/text.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/io/rttm.py` & `medkit_lib-0.7.1/medkit/io/rttm.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/io/spacy.py` & `medkit_lib-0.7.1/medkit/io/spacy.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/context/__init__.py` & `medkit_lib-0.7.1/medkit/text/context/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/context/family_detector.py` & `medkit_lib-0.7.1/medkit/text/context/family_detector.py`

 * *Files 4% similar despite different names*

```diff
@@ -259,7 +259,30 @@
                     "Some rules have ids and other do not. Please provide either ids"
                     " for all rules or no ids at all"
                 )
             if len(set(r.id for r in rules)) != len(rules):
                 raise ValueError(
                     "Some rules have the same id, each rule must have a unique id"
                 )
+
+    @staticmethod
+    def save_rules(
+        rules: List[FamilyDetectorRule],
+        path_to_rules: Path,
+        encoding: Optional[str] = None,
+    ):
+        """
+        Store rules in a yml file
+
+        Parameters
+        ----------
+        rules
+            The rules to save
+        path_to_rules
+            Path to a .yml file that will contain the rules
+        encoding
+            Encoding of the .yml file
+        """
+
+        with open(path_to_rules, mode="w", encoding=encoding) as f:
+            rules_data = [dataclasses.asdict(r) for r in rules]
+            rules = yaml.safe_dump(rules_data, f)
```

### Comparing `medkit_lib-0.7.0/medkit/text/context/family_detector_default_rules.yml` & `medkit_lib-0.7.1/medkit/text/context/family_detector_default_rules.yml`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/context/hypothesis_detector.py` & `medkit_lib-0.7.1/medkit/text/context/hypothesis_detector.py`

 * *Files 3% similar despite different names*

```diff
@@ -380,7 +380,30 @@
                     "Some rules have ids and other do not. Please provide either ids"
                     " for all rules or no ids at all"
                 )
             if len(set(r.id for r in rules)) != len(rules):
                 raise ValueError(
                     "Some rules have the same uid, each rule must have a unique uid"
                 )
+
+    @staticmethod
+    def save_rules(
+        rules: List[HypothesisDetectorRule],
+        path_to_rules: Path,
+        encoding: Optional[str] = None,
+    ):
+        """
+        Store rules in a yml file
+
+        Parameters
+        ----------
+        rules
+            The rules to save
+        path_to_rules
+            Path to a .yml file that will contain the rules
+        encoding
+            Encoding of the .yml file
+        """
+
+        with open(path_to_rules, mode="w", encoding=encoding) as f:
+            rules_data = [dataclasses.asdict(r) for r in rules]
+            rules = yaml.safe_dump(rules_data, f)
```

### Comparing `medkit_lib-0.7.0/medkit/text/context/hypothesis_detector_example_rules.yml` & `medkit_lib-0.7.1/medkit/text/context/hypothesis_detector_example_rules.yml`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/context/hypothesis_detector_example_verbs.yml` & `medkit_lib-0.7.1/medkit/text/context/hypothesis_detector_example_verbs.yml`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/context/negation_detector.py` & `medkit_lib-0.7.1/medkit/text/context/negation_detector.py`

 * *Files 4% similar despite different names*

```diff
@@ -251,7 +251,30 @@
                     "Some rules have ids and other do not. Please provide either ids"
                     " for all rules or no ids at all"
                 )
             if len(set(r.id for r in rules)) != len(rules):
                 raise ValueError(
                     "Some rules have the same uid, each rule must have a unique uid"
                 )
+
+    @staticmethod
+    def save_rules(
+        rules: List[NegationDetectorRule],
+        path_to_rules: Path,
+        encoding: Optional[str] = None,
+    ):
+        """
+        Store rules in a yml file
+
+        Parameters
+        ----------
+        rules
+            The rules to save
+        path_to_rules
+            Path to a .yml file that will contain the rules
+        encoding
+            Encoding of the .yml file
+        """
+
+        with open(path_to_rules, mode="w", encoding=encoding) as f:
+            rules_data = [dataclasses.asdict(r) for r in rules]
+            rules = yaml.safe_dump(rules_data, f)
```

### Comparing `medkit_lib-0.7.0/medkit/text/context/negation_detector_default_rules.yml` & `medkit_lib-0.7.1/medkit/text/context/negation_detector_default_rules.yml`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/metrics/ner.py` & `medkit_lib-0.7.1/medkit/text/metrics/ner.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/ner/__init__.py` & `medkit_lib-0.7.1/medkit/text/ner/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/ner/adicap_norm_attribute.py` & `medkit_lib-0.7.1/medkit/text/ner/adicap_norm_attribute.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/ner/date_attribute.py` & `medkit_lib-0.7.1/medkit/text/ner/date_attribute.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/ner/duckling_matcher.py` & `medkit_lib-0.7.1/medkit/text/ner/duckling_matcher.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/ner/hf_entity_matcher.py` & `medkit_lib-0.7.1/medkit/text/ner/hf_entity_matcher.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/ner/hf_entity_matcher_trainable.py` & `medkit_lib-0.7.1/medkit/text/ner/hf_entity_matcher_trainable.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/ner/hf_tokenization_utils.py` & `medkit_lib-0.7.1/medkit/text/ner/hf_tokenization_utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/ner/iamsystem_matcher.py` & `medkit_lib-0.7.1/medkit/text/ner/iamsystem_matcher.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/ner/quick_umls_matcher.py` & `medkit_lib-0.7.1/medkit/text/ner/quick_umls_matcher.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/ner/regexp_matcher.py` & `medkit_lib-0.7.1/medkit/text/ner/regexp_matcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -365,7 +365,30 @@
                     "Some rules have ids and other do not. Please provide either ids"
                     " for all rules or no ids at all"
                 )
             if len(set(r.id for r in rules)) != len(rules):
                 raise ValueError(
                     "Some rules have the same id, each rule must have a unique id"
                 )
+
+    @staticmethod
+    def save_rules(
+        rules: List[RegexpMatcherRule],
+        path_to_rules: Path,
+        encoding: Optional[str] = None,
+    ):
+        """
+        Store rules in a yml file
+
+        Parameters
+        ----------
+        rules
+            The rules to save
+        path_to_rules
+            Path to a .yml file that will contain the rules
+        encoding
+            Encoding of the .yml file
+        """
+
+        with open(path_to_rules, mode="w", encoding=encoding) as f:
+            rules_data = [dataclasses.asdict(r) for r in rules]
+            rules = yaml.safe_dump(rules_data, f)
```

### Comparing `medkit_lib-0.7.0/medkit/text/ner/regexp_matcher_default_rules.yml` & `medkit_lib-0.7.1/medkit/text/ner/regexp_matcher_default_rules.yml`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/ner/tnm_attribute.py` & `medkit_lib-0.7.1/medkit/text/ner/tnm_attribute.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/ner/umls_coder_normalizer.py` & `medkit_lib-0.7.1/medkit/text/ner/umls_coder_normalizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -397,14 +397,24 @@
         **kwargs,
     ):
         super().__init__(model, tokenizer, *args, **kwargs)
 
         self.summary_method = summary_method
         self.normalize = normalize
 
+    def _ensure_tensor_on_device(self, inputs, device):
+        """
+        Hack to force tensors to be kept on pipeline device. The base hugging
+        face pipeline tries to move the model outputs back to the cpu before
+        returning them but we want to keep them on the gpu if they are, because
+        we want to still be on the gpu when doing big similarity matrix multiplication
+        between entities embeddings and umls embeddings
+        """
+        return super()._ensure_tensor_on_device(inputs, self.device)
+
     def preprocess(self, inputs, truncation=True) -> Dict[str, torch.Tensor]:
         return self.tokenizer(
             inputs,
             max_length=32,
             add_special_tokens=True,
             truncation=truncation,
             padding="max_length",
```

### Comparing `medkit_lib-0.7.0/medkit/text/ner/umls_norm_attribute.py` & `medkit_lib-0.7.1/medkit/text/ner/umls_norm_attribute.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/ner/umls_semgroups_v04.txt` & `medkit_lib-0.7.1/medkit/text/ner/umls_semgroups_v04.txt`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/ner/umls_utils.py` & `medkit_lib-0.7.1/medkit/text/ner/umls_utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/postprocessing/alignment_utils.py` & `medkit_lib-0.7.1/medkit/text/postprocessing/alignment_utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/postprocessing/attribute_duplicator.py` & `medkit_lib-0.7.1/medkit/text/postprocessing/attribute_duplicator.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/preprocessing/__init__.py` & `medkit_lib-0.7.1/medkit/text/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/preprocessing/char_replacer.py` & `medkit_lib-0.7.1/medkit/text/preprocessing/char_replacer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/preprocessing/char_rules.py` & `medkit_lib-0.7.1/medkit/text/preprocessing/char_rules.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/preprocessing/duplicate_finder.py` & `medkit_lib-0.7.1/medkit/text/preprocessing/duplicate_finder.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/preprocessing/eds_cleaner.py` & `medkit_lib-0.7.1/medkit/text/preprocessing/eds_cleaner.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/preprocessing/normalizer.py` & `medkit_lib-0.7.1/medkit/text/preprocessing/normalizer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/relations/syntactic_relation_extractor.py` & `medkit_lib-0.7.1/medkit/text/relations/syntactic_relation_extractor.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/segmentation/default_section_definition.yml` & `medkit_lib-0.7.1/medkit/text/segmentation/default_section_definition.yml`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/segmentation/default_syntagma_definition.yml` & `medkit_lib-0.7.1/medkit/text/segmentation/default_syntagma_definition.yml`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/segmentation/rush_sentence_tokenizer.py` & `medkit_lib-0.7.1/medkit/text/segmentation/rush_sentence_tokenizer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/segmentation/rush_sentence_tokenizer_default_rules.tsv` & `medkit_lib-0.7.1/medkit/text/segmentation/rush_sentence_tokenizer_default_rules.tsv`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/segmentation/section_tokenizer.py` & `medkit_lib-0.7.1/medkit/text/segmentation/section_tokenizer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/segmentation/sentence_tokenizer.py` & `medkit_lib-0.7.1/medkit/text/segmentation/sentence_tokenizer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/segmentation/syntagma_tokenizer.py` & `medkit_lib-0.7.1/medkit/text/segmentation/syntagma_tokenizer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/segmentation/tokenizer_utils.py` & `medkit_lib-0.7.1/medkit/text/segmentation/tokenizer_utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/spacy/__init__.py` & `medkit_lib-0.7.1/medkit/text/spacy/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/spacy/displacy_utils.py` & `medkit_lib-0.7.1/medkit/text/spacy/displacy_utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/spacy/doc_pipeline.py` & `medkit_lib-0.7.1/medkit/text/spacy/doc_pipeline.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/spacy/edsnlp.py` & `medkit_lib-0.7.1/medkit/text/spacy/edsnlp.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/spacy/pipeline.py` & `medkit_lib-0.7.1/medkit/text/spacy/pipeline.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/spacy/spacy_utils.py` & `medkit_lib-0.7.1/medkit/text/spacy/spacy_utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/text/translation/hf_translator.py` & `medkit_lib-0.7.1/medkit/text/translation/hf_translator.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/tools/_save_prov_to_dot.py` & `medkit_lib-0.7.1/medkit/tools/_save_prov_to_dot.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/tools/hf_utils.py` & `medkit_lib-0.7.1/medkit/tools/hf_utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/training/__init__.py` & `medkit_lib-0.7.1/medkit/training/__init__.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/training/callbacks.py` & `medkit_lib-0.7.1/medkit/training/callbacks.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/training/trainable_component.py` & `medkit_lib-0.7.1/medkit/training/trainable_component.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/training/trainer.py` & `medkit_lib-0.7.1/medkit/training/trainer.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/training/trainer_config.py` & `medkit_lib-0.7.1/medkit/training/trainer_config.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/medkit/training/utils.py` & `medkit_lib-0.7.1/medkit/training/utils.py`

 * *Files identical despite different names*

### Comparing `medkit_lib-0.7.0/pyproject.toml` & `medkit_lib-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "medkit-lib"
-version = "0.7.0"
+version = "0.7.1"
 description = "A Python library for a learning health system"
 readme = "README.md"
 repository = "https://gitlab.inria.fr/heka/medkit/"
 documentation = "https://heka.gitlabpages.inria.fr/medkit/"
 authors = ["HeKA Research Team"]
 maintainers = [
     "medkit-maintainers <medkit-maintainers@inria.fr>"
```

### Comparing `medkit_lib-0.7.0/PKG-INFO` & `medkit_lib-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medkit-lib
-Version: 0.7.0
+Version: 0.7.1
 Summary: A Python library for a learning health system
 Home-page: https://gitlab.inria.fr/heka/medkit/
 License: MIT
 Author: HeKA Research Team
 Maintainer: medkit-maintainers
 Maintainer-email: medkit-maintainers@inria.fr
 Requires-Python: >=3.7.1,<4.0
```

